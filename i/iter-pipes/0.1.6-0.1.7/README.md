# Comparing `tmp/iter_pipes-0.1.6.tar.gz` & `tmp/iter_pipes-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iter_pipes-0.1.6.tar", max compression
+gzip compressed data, was "iter_pipes-0.1.7.tar", max compression
```

## Comparing `iter_pipes-0.1.6.tar` & `iter_pipes-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2024-03-21 11:53:58.514451 iter_pipes-0.1.6/LICENSE
--rw-r--r--   0        0        0     7044 2024-03-21 11:53:58.514451 iter_pipes-0.1.6/README.md
--rw-r--r--   0        0        0       28 2024-03-21 11:53:58.514451 iter_pipes-0.1.6/iter_pipes/__init__.py
--rw-r--r--   0        0        0     5531 2024-03-21 11:53:58.514451 iter_pipes-0.1.6/iter_pipes/functional.py
--rw-r--r--   0        0        0     5353 2024-03-21 11:53:58.514451 iter_pipes-0.1.6/iter_pipes/main.py
--rw-r--r--   0        0        0     1066 2024-03-21 11:53:58.514451 iter_pipes-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     7780 1970-01-01 00:00:00.000000 iter_pipes-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-16 07:44:59.865729 iter_pipes-0.1.7/LICENSE
+-rw-r--r--   0        0        0     7044 2024-04-16 07:44:59.865729 iter_pipes-0.1.7/README.md
+-rw-r--r--   0        0        0       28 2024-04-16 07:44:59.865729 iter_pipes-0.1.7/iter_pipes/__init__.py
+-rw-r--r--   0        0        0     6049 2024-04-16 07:44:59.865729 iter_pipes-0.1.7/iter_pipes/functional.py
+-rw-r--r--   0        0        0     6321 2024-04-16 07:44:59.865729 iter_pipes-0.1.7/iter_pipes/main.py
+-rw-r--r--   0        0        0     1071 2024-04-16 07:44:59.865729 iter_pipes-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     7780 1970-01-01 00:00:00.000000 iter_pipes-0.1.7/PKG-INFO
```

### Comparing `iter_pipes-0.1.6/LICENSE` & `iter_pipes-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `iter_pipes-0.1.6/README.md` & `iter_pipes-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `iter_pipes-0.1.6/iter_pipes/functional.py` & `iter_pipes-0.1.7/iter_pipes/functional.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 ]
 
 T = TypeVar("T")
 V = TypeVar("V")
 U = TypeVar("U")
 W = TypeVar("W")
 X = TypeVar("X")
+Y = TypeVar("Y")
+Z = TypeVar("Z")
 
 
 raw_filter = filter
 
 
 Step = Callable[[Iterable[T]], Iterable[V]]
 
@@ -75,77 +77,95 @@
         ):
             yield from step([x[0] for x in batch_iterator])
 
     return f
 
 
 @overload
-def filter(step: Callable[[V], TypeGuard[W]]) -> Step[V, W]:
-    ...
+def filter(step: Callable[[V], TypeGuard[W]]) -> Step[V, W]: ...
 
 
 @overload
-def filter(step: Callable[[V], bool]) -> Step[V, V]:
-    ...
+def filter(step: Callable[[V], bool]) -> Step[V, V]: ...
 
 
 def filter(step: Callable[[V], bool]) -> Step[V, V]:  # type: ignore
     return partial(raw_filter, step)  # type: ignore
 
 
 @overload
 def branch(
     step1: Step[T, U] | None,
     step2: Step[T, V],
     pick_first: Literal[True],
     max_inflight: int | None = ...,
-) -> Step[T, U]:
-    ...
+) -> Step[T, U]: ...
 
 
 @overload
 def branch(
     step1: Step[T, U],
     step2: Step[T, V],
     pick_first: Literal[False] | None,
     max_inflight: int | None = ...,
-) -> Step[T, V | U]:
-    ...
+) -> Step[T, V | U]: ...
 
 
 @overload
 def branch(
     step1: Step[T, U],
     step2: Step[T, V],
     step3: Step[T, W],
     pick_first: Literal[False] | None,
     max_inflight: int | None = ...,
-) -> Step[T, V | U | W]:
-    ...
+) -> Step[T, V | U | W]: ...
 
 
 @overload
-def branch(  # noqa: PLR0913
+def branch(
+    step1: Step[T, U],
+    step2: Step[T, V],
+    step3: Step[T, W],
+    step4: Step[T, X],
+    pick_first: Literal[False] | None,
+    max_inflight: int | None = ...,
+) -> Step[T, V | U | W | X]: ...
+
+
+@overload
+def branch(
     step1: Step[T, U],
     step2: Step[T, V],
     step3: Step[T, W],
     step4: Step[T, X],
+    step5: Step[T, Y],
     pick_first: Literal[False] | None,
     max_inflight: int | None = ...,
-) -> Step[T, V | U | W | X]:
-    ...
+) -> Step[T, V | U | W | X | Y]: ...
+
+
+@overload
+def branch(
+    step1: Step[T, U],
+    step2: Step[T, V],
+    step3: Step[T, W],
+    step4: Step[T, X],
+    step5: Step[T, Y],
+    step6: Step[T, Z],
+    pick_first: Literal[False] | None,
+    max_inflight: int | None = ...,
+) -> Step[T, V | U | W | X | Y | Z]: ...
 
 
 @overload
 def branch(
     *steps: Step[T, Any] | None,
     pick_first: Literal[False] | None,
     max_inflight: int | None = ...,
-) -> Step[T, Any]:
-    ...
+) -> Step[T, Any]: ...
 
 
 def branch(  # type: ignore
     *steps: Step[T, Any] | None,
     max_inflight: int = 1000,
     pick_first: bool = False,
 ) -> Step[T, Any]:
```

### Comparing `iter_pipes-0.1.6/pyproject.toml` & `iter_pipes-0.1.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "iter-pipes"
-version = "0.1.6"
+version = "0.1.7"
 description = "Functional pythonic pipelines for iterables."
 authors = ["brightnetwork <dev@brightnetwork.co.uk>"]
 repository = "https://github.com/brightnetwork/iter-pipes"
 homepage = "https://github.com/brightnetwork/iter-pipes"
 documentation = "https://github.com/brightnetwork/iter-pipes"
 keywords = ["iterable", "pipes", "collection"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.1.4"
-mypy = "^1.6.1"
-pytest = "^7.4.3"
-pyright = "^1.1.336"
+ruff = "^0.3.3"
+mypy = "^1.9.0"
+pytest = "^8.1.1"
+pyright = "^1.1.355"
 pytest-cov = "^4.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.ruff]
+[tool.ruff.lint]
 select = ["ALL"]
 ignore = ["INP001", "D", "COM", "PGH", "ANN101", "ANN204", "A003", "TRY", "EM101", "A001", "ISC001", "C901"]
 
 [tool.ruff.lint.extend-per-file-ignores]
 "tests/**" = ["ANN201", "S101", "FA102", "PLR2004"]
 
 [tool.coverage.report]
```

### Comparing `iter_pipes-0.1.6/PKG-INFO` & `iter_pipes-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iter-pipes
-Version: 0.1.6
+Version: 0.1.7
 Summary: Functional pythonic pipelines for iterables.
 Home-page: https://github.com/brightnetwork/iter-pipes
 License: MIT
 Keywords: iterable,pipes,collection
 Author: brightnetwork
 Author-email: dev@brightnetwork.co.uk
 Requires-Python: >=3.10,<4.0
```

