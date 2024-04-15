# Comparing `tmp/anstrip-0.1.0.post1.tar.gz` & `tmp/anstrip-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anstrip-0.1.0.post1.tar", last modified: Sun Apr 14 12:31:23 2024, max compression
+gzip compressed data, was "anstrip-0.2.0.tar", last modified: Mon Apr 15 22:37:23 2024, max compression
```

## Comparing `anstrip-0.1.0.post1.tar` & `anstrip-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-14 12:31:23.264402 anstrip-0.1.0.post1/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1061 2024-04-14 10:56:07.000000 anstrip-0.1.0.post1/LICENSE
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2318 2024-04-14 12:31:23.261068 anstrip-0.1.0.post1/PKG-INFO
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      501 2024-04-14 12:29:33.000000 anstrip-0.1.0.post1/README.md
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      590 2024-04-14 12:30:53.000000 anstrip-0.1.0.post1/pyproject.toml
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       38 2024-04-14 12:31:23.264402 anstrip-0.1.0.post1/setup.cfg
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-14 12:31:23.261068 anstrip-0.1.0.post1/src/
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-14 12:31:23.261068 anstrip-0.1.0.post1/src/anstrip/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     3515 2024-04-14 12:29:40.000000 anstrip-0.1.0.post1/src/anstrip/__init__.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2696 2024-04-14 12:18:27.000000 anstrip-0.1.0.post1/src/anstrip/__init__.pyi
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        0 2024-04-14 11:16:28.000000 anstrip-0.1.0.post1/src/anstrip/py.typed
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-14 12:31:23.261068 anstrip-0.1.0.post1/src/anstrip.egg-info/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2318 2024-04-14 12:31:23.000000 anstrip-0.1.0.post1/src/anstrip.egg-info/PKG-INFO
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      276 2024-04-14 12:31:23.000000 anstrip-0.1.0.post1/src/anstrip.egg-info/SOURCES.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        1 2024-04-14 12:31:23.000000 anstrip-0.1.0.post1/src/anstrip.egg-info/dependency_links.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       58 2024-04-14 12:31:23.000000 anstrip-0.1.0.post1/src/anstrip.egg-info/requires.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        8 2024-04-14 12:31:23.000000 anstrip-0.1.0.post1/src/anstrip.egg-info/top_level.txt
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-15 22:37:23.612928 anstrip-0.2.0/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1061 2024-04-14 10:56:07.000000 anstrip-0.2.0/LICENSE
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2397 2024-04-15 22:37:23.612928 anstrip-0.2.0/PKG-INFO
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      586 2024-04-14 12:38:35.000000 anstrip-0.2.0/README.md
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      588 2024-04-15 22:37:07.000000 anstrip-0.2.0/pyproject.toml
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       38 2024-04-15 22:37:23.612928 anstrip-0.2.0/setup.cfg
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-15 22:37:23.609595 anstrip-0.2.0/src/
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-15 22:37:23.612928 anstrip-0.2.0/src/anstrip/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     3505 2024-04-15 22:37:07.000000 anstrip-0.2.0/src/anstrip/__init__.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2691 2024-04-15 22:37:07.000000 anstrip-0.2.0/src/anstrip/__init__.pyi
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        0 2024-04-14 11:16:28.000000 anstrip-0.2.0/src/anstrip/py.typed
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-15 22:37:23.612928 anstrip-0.2.0/src/anstrip.egg-info/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2397 2024-04-15 22:37:23.000000 anstrip-0.2.0/src/anstrip.egg-info/PKG-INFO
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      276 2024-04-15 22:37:23.000000 anstrip-0.2.0/src/anstrip.egg-info/SOURCES.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        1 2024-04-15 22:37:23.000000 anstrip-0.2.0/src/anstrip.egg-info/dependency_links.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       58 2024-04-15 22:37:23.000000 anstrip-0.2.0/src/anstrip.egg-info/requires.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        8 2024-04-15 22:37:23.000000 anstrip-0.2.0/src/anstrip.egg-info/top_level.txt
```

### Comparing `anstrip-0.1.0.post1/LICENSE` & `anstrip-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anstrip-0.1.0.post1/PKG-INFO` & `anstrip-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anstrip
-Version: 0.1.0.post1
+Version: 0.2.0
 Summary: anstrip is a minimal library to strip ANSI sequences from strings.
 Author-email: Qexat <contact@qexat.com>
 License: MIT License
         
         Copyright (c) 2024 Qexat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,14 +34,16 @@
 Requires-Dist: coverage>=7.4; extra == "dev"
 Requires-Dist: pyright>=1.1; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # anstrip
 
+[![PyPI](https://img.shields.io/pypi/v/anstrip)](https://pypi.org/project/anstrip/)
+
 anstrip is a minimal library to strip ANSI sequences from strings.
 
 It provides:
 
 - `PATTERN`, the regex pattern used by the functions of anstrip
 - `strip`, a function to remove all the escape sequences from a string
 - `auto_strip`, a function that is similar to `strip`, except that it only removes if the output is a TTY
```

### Comparing `anstrip-0.1.0.post1/pyproject.toml` & `anstrip-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "anstrip"
 description = "anstrip is a minimal library to strip ANSI sequences from strings."
-version = "0.1.0-1"
+version = "0.2.0"
 readme = "README.md"
 keywords = ["ansi", "escape sequence", "SGR", "ECMA", "strip"]
 requires-python = ">=3.10"
 
 
 [project.optional-dependencies]
 dev = ["pytest>=7.4", "coverage>=7.4", "pyright>=1.1", "build", "twine"]
```

### Comparing `anstrip-0.1.0.post1/src/anstrip/__init__.py` & `anstrip-0.2.0/src/anstrip/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import sys
 import typing
 
 __all__ = [
     "PATTERN",
     "strip",
     "auto_strip",
-    "auto_print",
+    "print",
     "printed_length",
 ]
 
 _P = typing.ParamSpec("_P")
 
 # Based on <https://github.com/chalk/ansi-regex/blob/main/index.js>
 # The license of `ansi-regex` can be found in the `3rdparty` directory
@@ -82,15 +82,15 @@
         return inner
 
     if string_or_function is not None:
         return decorator(string_or_function)
     return decorator
 
 
-def auto_print(
+def print(
     *values: object,
     sep: str | None = None,
     end: str | None = None,
     file: typing.TextIO | None = None,
     flush: bool = False,
 ) -> None:
     """
```

### Comparing `anstrip-0.1.0.post1/src/anstrip/__init__.pyi` & `anstrip-0.2.0/src/anstrip/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     ... def pretty_integer(value: int) -> str:
     ...     return f"\\x1b[1;96m{value}\\x1b[22;39m"
 
     >>> pretty_integer(42)
     '42'
     """
 
-def auto_print(
+def print(
     *values: object,
     sep: str | None = None,
     end: str | None = None,
     file: typing.TextIO | None = None,
     flush: bool = False,
 ) -> None: ...
 def printed_length(string: str) -> int: ...
```

### Comparing `anstrip-0.1.0.post1/src/anstrip.egg-info/PKG-INFO` & `anstrip-0.2.0/src/anstrip.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anstrip
-Version: 0.1.0.post1
+Version: 0.2.0
 Summary: anstrip is a minimal library to strip ANSI sequences from strings.
 Author-email: Qexat <contact@qexat.com>
 License: MIT License
         
         Copyright (c) 2024 Qexat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,14 +34,16 @@
 Requires-Dist: coverage>=7.4; extra == "dev"
 Requires-Dist: pyright>=1.1; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # anstrip
 
+[![PyPI](https://img.shields.io/pypi/v/anstrip)](https://pypi.org/project/anstrip/)
+
 anstrip is a minimal library to strip ANSI sequences from strings.
 
 It provides:
 
 - `PATTERN`, the regex pattern used by the functions of anstrip
 - `strip`, a function to remove all the escape sequences from a string
 - `auto_strip`, a function that is similar to `strip`, except that it only removes if the output is a TTY
```

