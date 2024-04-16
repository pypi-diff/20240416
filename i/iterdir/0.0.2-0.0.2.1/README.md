# Comparing `tmp/iterdir-0.0.2.tar.gz` & `tmp/iterdir-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterdir-0.0.2.tar", max compression
+gzip compressed data, was "iterdir-0.0.2.1.tar", max compression
```

## Comparing `iterdir-0.0.2.tar` & `iterdir-0.0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 iterdir-0.0.2/LICENSE
--rw-r--r--   0        0        0     8191 2024-04-16 09:48:51.211506 iterdir-0.0.2/iterdir.py
--rw-r--r--   0        0        0     1071 2024-04-16 09:18:44.352955 iterdir-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      152 2024-04-16 08:39:39.205664 iterdir-0.0.2/readme.md
--rw-r--r--   0        0        0     1616 1970-01-01 00:00:00.000000 iterdir-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 iterdir-0.0.2.1/LICENSE
+-rw-r--r--   0        0        0     8056 2024-04-16 11:00:53.760552 iterdir-0.0.2.1/iterdir.py
+-rw-r--r--   0        0        0     1073 2024-04-16 11:02:37.973543 iterdir-0.0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      152 2024-04-16 08:39:39.205664 iterdir-0.0.2.1/readme.md
+-rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 iterdir-0.0.2.1/PKG-INFO
```

### Comparing `iterdir-0.0.2/LICENSE` & `iterdir-0.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iterdir-0.0.2/iterdir.py` & `iterdir-0.0.2.1/iterdir.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,28 +226,24 @@
     /, 
     topdown: Optional[bool] = True, 
     min_depth: int = 1, 
     max_depth: int = 1, 
     predicate: Optional[Callable[..., Optional[bool]]] = None, 
     onerror: Optional[bool] = None, 
     follow_symlinks: bool = False, 
-    follow_direct_relatives: bool = True, 
 ) -> Iterator:
     if top is None:
         top = DirEntry(".")
     is_dir: Callable[[bytes | str | PathLike], bool]
     if follow_symlinks:
-        if follow_direct_relatives:
-            is_dir = isdir
-        else:
-            realtop = realpath(top)
-            is_dir = lambda p, /: (
-                isdir(p) and 
-                commonpath((realtop, rp := realpath(p))) not in (realtop, rp) # type: ignore
-            )
+        realtop = realpath(top)
+        is_dir = lambda p, /: (isdir(p) and (
+            not islink(p) or
+            commonpath(t := (realtop, realpath(p))) not in t # type: ignore
+        ))
     else:
         is_dir = lambda p, /: not islink(p) and isdir(p)
     iter_dir: Callable
     if isinstance(top, DirEntry):
         iter_dir = scandir
     elif isinstance(top, Path):
         iter_dir = Path.iterdir
```

### Comparing `iterdir-0.0.2/pyproject.toml` & `iterdir-0.0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iterdir"
-version = "0.0.2"
+version = "0.0.2.1"
 description = "iterdir."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iterdir"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iterdir"
 keywords = ["iterdir", "traverse"]
```

### Comparing `iterdir-0.0.2/PKG-INFO` & `iterdir-0.0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterdir
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: iterdir.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iterdir
 License: MIT
 Keywords: iterdir,traverse
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
```

