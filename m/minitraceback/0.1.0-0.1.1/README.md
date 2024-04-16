# Comparing `tmp/minitraceback-0.1.0.tar.gz` & `tmp/minitraceback-0.1.1.tar.gz`

## Comparing `minitraceback-0.1.0.tar` & `minitraceback-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 minitraceback-0.1.0/.python-version
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 minitraceback-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 minitraceback-0.1.0/requirements.lock
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 minitraceback-0.1.0/src/minitraceback/__init__.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 minitraceback-0.1.0/tests/test_minitraceback.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 minitraceback-0.1.0/tests/sub/__init__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 minitraceback-0.1.0/tests/sub/f.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 minitraceback-0.1.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 minitraceback-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 minitraceback-0.1.0/README.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 minitraceback-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 minitraceback-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 minitraceback-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 minitraceback-0.1.1/.python-version
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 minitraceback-0.1.1/requirements-dev.lock
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 minitraceback-0.1.1/requirements.lock
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 minitraceback-0.1.1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 minitraceback-0.1.1/src/minitraceback/__init__.py
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 minitraceback-0.1.1/tests/test_minitraceback.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 minitraceback-0.1.1/tests/sub/__init__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 minitraceback-0.1.1/tests/sub/f.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 minitraceback-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 minitraceback-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 minitraceback-0.1.1/README.md
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 minitraceback-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 minitraceback-0.1.1/PKG-INFO
```

### Comparing `minitraceback-0.1.0/src/minitraceback/__init__.py` & `minitraceback-0.1.1/src/minitraceback/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -51,23 +51,56 @@
 
 def extract_stack(f, /, *, limit: int | None = None) -> list[FrameInfo]:
     """Extract a traceback from a frame object."""
     frames = itertools.islice(traceback.walk_stack(f), limit)
     return _extract_from(frames)
 
 
-def format_frames(frames: list[FrameInfo], *, indent=0) -> list[str]:
+def format_list(frames: list[FrameInfo], *, indent=0) -> list[str]:
     """Format a list of FrameInfo into a list of strings.
 
     Format is 'filename:lineno funcname'.
     """
     sindent = " " * indent
     return [f"{sindent}{f}:{lineno} {name}" for f, lineno, name in frames]
 
 
+def format_tb(tb, /, *, limit=None) -> list[str]:
+    """Format a traceback from a traceback object."""
+    return format_list(extract_tb(tb, limit=limit), indent=2)
+
+
+def print_tb(tb, /, *, limit=None, file=None):
+    """Print a traceback from a traceback object."""
+    if file is None:
+        file = sys.stderr
+    print(TRACEBACK_HEADER, file=file)
+    for line in format_tb(tb, limit=limit):
+        print(line, file=file)
+
+
+def format_stack(f=None, /, *, limit=None) -> list[str]:
+    """Format a stack trace from a frame object."""
+    if f is None:
+        f = sys._getframe().f_back
+    lines = [TRACEBACK_HEADER] + format_list(extract_stack(f, limit=limit), indent=2)
+    return lines
+
+
+def print_stack(f=None, /, *, limit=None, file=None):
+    """Print a stack trace from a frame object."""
+    if f is None:
+        f = sys._getframe().f_back
+    if file is None:
+        file = sys.stderr
+    print(TRACEBACK_HEADER, file=file)
+    for line in format_list(extract_stack(f, limit=limit), indent=2):
+        print(line, file=file)
+
+
 def format_exception_only(exc: BaseException) -> list[str]:
     """Format an exception without a traceback."""
     exc_type = type(exc)
     exc_type_qualname = exc_type.__qualname__
     exc_type_module = exc_type.__module__
     if exc_type_module == "builtins":
         stype = exc_type_qualname
@@ -84,9 +117,16 @@
 def format_exception(exc, /, *, limit=None) -> list[str]:
     """Format an exception and its traceback."""
     tb = exc.__traceback__
     tbs = extract_tb(tb, limit=limit)
     return [
         *format_exception_only(exc),
         TRACEBACK_HEADER,
-        *format_frames(tbs, indent=2),
+        *format_list(tbs, indent=2),
     ]
+
+
+def print_exception(exc, /, *, limit=None, file=None):
+    """Print an exception and its traceback."""
+    if file is None:
+        file = sys.stderr
+    print("\n".join(format_exception(exc, limit=limit)), file=file)
```

### Comparing `minitraceback-0.1.0/LICENSE.txt` & `minitraceback-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `minitraceback-0.1.0/pyproject.toml` & `minitraceback-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "minitraceback"
-version = "0.1.0"
+version = "0.1.1"
 description = "A minimal traceback formatter for Python."
 authors = [
     { name = "Inada Naoki", email = "songofacandy@gmail.com" }
 ]
 dependencies = []
 readme = "README.md"
 requires-python = ">= 3.8"
```

