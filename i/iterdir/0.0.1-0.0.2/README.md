# Comparing `tmp/iterdir-0.0.1.tar.gz` & `tmp/iterdir-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterdir-0.0.1.tar", max compression
+gzip compressed data, was "iterdir-0.0.2.tar", max compression
```

## Comparing `iterdir-0.0.1.tar` & `iterdir-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 iterdir-0.0.1/LICENSE
--rw-r--r--   0        0        0     7883 2024-04-16 08:33:01.516382 iterdir-0.0.1/iterdir.py
--rw-r--r--   0        0        0     1071 2024-04-16 08:39:01.714627 iterdir-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      152 2024-04-16 08:39:39.205664 iterdir-0.0.1/readme.md
--rw-r--r--   0        0        0     1616 1970-01-01 00:00:00.000000 iterdir-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 iterdir-0.0.2/LICENSE
+-rw-r--r--   0        0        0     8191 2024-04-16 09:48:51.211506 iterdir-0.0.2/iterdir.py
+-rw-r--r--   0        0        0     1071 2024-04-16 09:18:44.352955 iterdir-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      152 2024-04-16 08:39:39.205664 iterdir-0.0.2/readme.md
+-rw-r--r--   0        0        0     1616 1970-01-01 00:00:00.000000 iterdir-0.0.2/PKG-INFO
```

### Comparing `iterdir-0.0.1/LICENSE` & `iterdir-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iterdir-0.0.1/iterdir.py` & `iterdir-0.0.2/iterdir.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 0, 1)
+__version__ = (0, 0, 2)
 __all__ = ["DirEntry", "iterdir"]
 
 from collections import deque
 from collections.abc import Callable, Iterable, Iterator
 from os import fspath, listdir, scandir, stat, DirEntry as _DirEntry, PathLike
-from os.path import abspath, basename, isfile, isdir, islink, join as joinpath
+from os.path import (
+    abspath, commonpath, basename, isfile, isdir, islink, join as joinpath, realpath, 
+)
 from pathlib import Path
 from typing import overload, Generic, Never, Optional, TypeVar
 
 
 AnyStr = TypeVar("AnyStr", bytes, str)
 PathType = TypeVar("PathType", bytes, str, PathLike)
 
@@ -92,15 +94,15 @@
         if min_depth <= 0:
             pred = True if predicate is None else predicate(path)
             if pred is None:
                 return
             elif pred:
                 yield path
             min_depth = 1
-        if depth == 0 and (not is_dir(path) or 0 <= max_depth <= depth):
+        if depth == 0 and (not isdir(path) or 0 <= max_depth <= depth):
             return
         depth += 1
         try:
             for path in iter_dir(path):
                 pred = True if predicate is None else predicate(path)
                 if pred is None:
                     continue
@@ -224,34 +226,40 @@
     /, 
     topdown: Optional[bool] = True, 
     min_depth: int = 1, 
     max_depth: int = 1, 
     predicate: Optional[Callable[..., Optional[bool]]] = None, 
     onerror: Optional[bool] = None, 
     follow_symlinks: bool = False, 
+    follow_direct_relatives: bool = True, 
 ) -> Iterator:
     if top is None:
         top = DirEntry(".")
     is_dir: Callable[[bytes | str | PathLike], bool]
     if follow_symlinks:
-        is_dir = isdir
+        if follow_direct_relatives:
+            is_dir = isdir
+        else:
+            realtop = realpath(top)
+            is_dir = lambda p, /: (
+                isdir(p) and 
+                commonpath((realtop, rp := realpath(p))) not in (realtop, rp) # type: ignore
+            )
     else:
         is_dir = lambda p, /: not islink(p) and isdir(p)
     iter_dir: Callable
     if isinstance(top, DirEntry):
         iter_dir = scandir
     elif isinstance(top, Path):
         iter_dir = Path.iterdir
     else:
         top = fspath(top)
         if not top:
             top = abspath(top)
-        def iter_dir(path, /):
-            for name in listdir(path):
-                yield joinpath(path, name)
+        iter_dir = lambda path, /: (joinpath(path, name) for name in listdir(path))
     if topdown is None:
         return _iterdir_bfs(
             top, 
             is_dir=is_dir, 
             iter_dir=iter_dir, 
             min_depth=min_depth, 
             max_depth=max_depth,
```

### Comparing `iterdir-0.0.1/pyproject.toml` & `iterdir-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iterdir"
-version = "0.0.1"
+version = "0.0.2"
 description = "iterdir."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iterdir"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iterdir"
 keywords = ["iterdir", "traverse"]
```

### Comparing `iterdir-0.0.1/PKG-INFO` & `iterdir-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterdir
-Version: 0.0.1
+Version: 0.0.2
 Summary: iterdir.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iterdir
 License: MIT
 Keywords: iterdir,traverse
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
```

