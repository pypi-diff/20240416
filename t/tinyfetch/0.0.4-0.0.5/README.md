# Comparing `tmp/tinyfetch-0.0.4.tar.gz` & `tmp/tinyfetch-0.0.5.tar.gz`

## Comparing `tinyfetch-0.0.4.tar` & `tinyfetch-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/.github/workflows/test.yml
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/src/tinyfetch/__init__.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/src/tinyfetch/cli.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/src/tinyfetch/core.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/src/tinyfetch/module.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/tests/test.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/README.md
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 tinyfetch-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 tinyfetch-0.0.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 tinyfetch-0.0.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tinyfetch-0.0.5/src/tinyfetch/__init__.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 tinyfetch-0.0.5/src/tinyfetch/cli.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 tinyfetch-0.0.5/src/tinyfetch/core.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 tinyfetch-0.0.5/src/tinyfetch/module.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyfetch-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 tinyfetch-0.0.5/tests/test.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 tinyfetch-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 tinyfetch-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 tinyfetch-0.0.5/README.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 tinyfetch-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 tinyfetch-0.0.5/PKG-INFO
```

### Comparing `tinyfetch-0.0.4/.github/workflows/publish.yml` & `tinyfetch-0.0.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `tinyfetch-0.0.4/.github/workflows/test.yml` & `tinyfetch-0.0.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `tinyfetch-0.0.4/src/tinyfetch/cli.py` & `tinyfetch-0.0.5/src/tinyfetch/cli.py`

 * *Files identical despite different names*

### Comparing `tinyfetch-0.0.4/src/tinyfetch/core.py` & `tinyfetch-0.0.5/src/tinyfetch/core.py`

 * *Files identical despite different names*

### Comparing `tinyfetch-0.0.4/.gitignore` & `tinyfetch-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `tinyfetch-0.0.4/LICENSE.txt` & `tinyfetch-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tinyfetch-0.0.4/README.md` & `tinyfetch-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tinyfetch-0.0.4/pyproject.toml` & `tinyfetch-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tinyfetch-0.0.4/PKG-INFO` & `tinyfetch-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tinyfetch
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python and system information command-line fetch tool
 Project-URL: Source, https://github.com/beucismis/tinyfetch
 Project-URL: Issues, https://github.com/beucismis/tinyfetch/issues
 Project-URL: Documentation, https://github.com/beucismis/tinyfetch?tab=readme-ov-file#documentation
 Author-email: beucismis <beucismis@tutamail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

