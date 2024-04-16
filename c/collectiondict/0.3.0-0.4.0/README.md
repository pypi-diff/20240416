# Comparing `tmp/collectiondict-0.3.0.tar.gz` & `tmp/collectiondict-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collectiondict-0.3.0.tar", max compression
+gzip compressed data, was "collectiondict-0.4.0.tar", max compression
```

## Comparing `collectiondict-0.3.0.tar` & `collectiondict-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1498 2024-04-15 07:29:08.111850 collectiondict-0.3.0/LICENSE
--rw-r--r--   0        0        0      314 2024-04-15 07:29:08.115850 collectiondict-0.3.0/README.md
--rw-r--r--   0        0        0     1530 2024-04-15 07:29:08.115850 collectiondict-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      139 2024-04-15 07:29:08.115850 collectiondict-0.3.0/src/collectiondict/__init__.py
--rw-r--r--   0        0        0     7143 2024-04-15 07:29:08.115850 collectiondict-0.3.0/src/collectiondict/_collectiondict.py
--rw-r--r--   0        0        0     3341 2024-04-15 07:29:08.115850 collectiondict-0.3.0/src/collectiondict/_reverse_mapping.py
--rw-r--r--   0        0        0        0 2024-04-15 07:29:08.115850 collectiondict-0.3.0/src/collectiondict/py.typed
--rw-r--r--   0        0        0     1255 1970-01-01 00:00:00.000000 collectiondict-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1498 2024-04-16 21:15:29.963451 collectiondict-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4669 2024-04-16 21:15:29.963451 collectiondict-0.4.0/README.md
+-rw-r--r--   0        0        0     1531 2024-04-16 21:15:29.963451 collectiondict-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      219 2024-04-16 21:15:29.963451 collectiondict-0.4.0/src/collectiondict/__init__.py
+-rw-r--r--   0        0        0     5909 2024-04-16 21:15:29.963451 collectiondict-0.4.0/src/collectiondict/_collectiondict.py
+-rw-r--r--   0        0        0     2675 2024-04-16 21:15:29.963451 collectiondict-0.4.0/src/collectiondict/_reverse_mapping.py
+-rw-r--r--   0        0        0     2856 2024-04-16 21:15:29.963451 collectiondict-0.4.0/src/collectiondict/_reverse_multimapping.py
+-rw-r--r--   0        0        0        0 2024-04-16 21:15:29.963451 collectiondict-0.4.0/src/collectiondict/py.typed
+-rw-r--r--   0        0        0     5610 1970-01-01 00:00:00.000000 collectiondict-0.4.0/PKG-INFO
```

### Comparing `collectiondict-0.3.0/LICENSE` & `collectiondict-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `collectiondict-0.3.0/pyproject.toml` & `collectiondict-0.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "collectiondict"
-version = "0.3.0"
+version = "0.4.0"
 description = "Helpers to create dictionaries that collect values into collections"
 authors = ["Max Görner <5477952+MaxG87@users.noreply.github.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -40,18 +40,18 @@
 ]
 strict = true
 
 [tool.pytest.ini_options]
 addopts = [
     "--cov", "src",
     "--doctest-modules",
+    "--doctest-glob", "*.md",
     "--cov-branch",
     "--cov-fail-under", "95"
 ]
-testpaths = ["src", "tests"]
 
 [tool.ruff]
 src = [".", "src/"]
 
 [tool.ruff.lint]
 select = ["A", "B", "C", "F", "I", "ISC", "PIE", "PL", "Q", "RUF", "SIM", "TID", "W", "YTT"]
 ignore = ["E", "PLC1901", "SIM117"]
```

### Comparing `collectiondict-0.3.0/src/collectiondict/_collectiondict.py` & `collectiondict-0.4.0/src/collectiondict/_collectiondict.py`

 * *Files 20% similar despite different names*

```diff
@@ -64,36 +64,14 @@
     Create dictionaries that collect values into collections
 
     Given any stream of key-value tuples, this function creates a
     multi-dictionary which maps all values to the corresponding key. Thus,
     `collectiondict(clct, stream)` is similar to `dict(stream)` but does not
     discard values.
 
-    The implementation tries to be memory efficient and performant. Therefore,
-    it is possible to use it on extremely large streams, as long as the end
-    result fits in memory. Thus, if a list of the stream consumes more than
-    half of the available memory, `collectiondict` can still be used.
-    Furthermore, for deduplicating collections, e.g. `set`, the stream could
-    exceed available memory, as long as the key-value pairs do not. One of the
-    examples covers this scenario.
-
-    The supported collections are fixed. Only the built-in collections
-    `Counter`, `frozenset`, `list`, `set`, and `tuple` as well as their
-    subclasses are supported. If a unsupported collection is passed, an
-    exception is raised. However, `mypy` will warn about it.
-
-    Due to the limits of Pythons type annotations, it is not possible to
-    specify the correct return type for the custom classes. Thus, custom
-    classes are supported but the return type is not inferred to be the parent
-    class.
-
-    In order to have the best type inference, it is recommended to **cast**
-    `clct` to specify the value type. Passing a specialised collection class is
-    **not** supported currently. The examples show how to use a cast.
-
     Examples:
     ---------
     Simple usage using `set`:
     >>> collectiondict(set, [("a", 1), ("b", 2), ("a", 3)])
     {'a': {1, 3}, 'b': {2}}
 
     Usage using `frozenset` and a cast to have the best type inference:
```

