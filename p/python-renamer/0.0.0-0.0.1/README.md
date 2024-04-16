# Comparing `tmp/python_renamer-0.0.0.tar.gz` & `tmp/python_renamer-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_renamer-0.0.0.tar", max compression
+gzip compressed data, was "python_renamer-0.0.1.tar", max compression
```

## Comparing `python_renamer-0.0.0.tar` & `python_renamer-0.0.1.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_renamer-0.0.0/LICENSE
--rw-r--r--   0        0        0     1221 2024-04-16 13:54:03.543807 python_renamer-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      173 2024-04-16 13:46:07.773538 python_renamer-0.0.0/readme.md
--rw-r--r--   0        0        0     1984 2024-04-16 13:51:08.896856 python_renamer-0.0.0/renamer.py
--rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 python_renamer-0.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_renamer-0.0.1/LICENSE
+-rw-r--r--   0        0        0     1218 2024-04-16 14:54:06.310258 python_renamer-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      173 2024-04-16 13:46:07.773538 python_renamer-0.0.1/readme.md
+-rw-r--r--   0        0        0     4397 2024-04-16 15:30:07.707022 python_renamer-0.0.1/renamer/__init__.py
+-rw-r--r--   0        0        0       40 2024-04-16 13:57:48.775855 python_renamer-0.0.1/renamer/__main__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_renamer-0.0.1/renamer/py.typed
+-rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 python_renamer-0.0.1/PKG-INFO
```

### Comparing `python_renamer-0.0.0/LICENSE` & `python_renamer-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_renamer-0.0.0/pyproject.toml` & `python_renamer-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-renamer"
-version = "0.0.0"
+version = "0.0.1"
 description = "Python batch renamer."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-renamer"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-renamer"
 keywords = ["rename", "batch", "renamer"]
@@ -34,8 +34,8 @@
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.packages]]
-include = "renamer.py"
+include = "renamer"
```

### Comparing `python_renamer-0.0.0/PKG-INFO` & `python_renamer-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-renamer
-Version: 0.0.0
+Version: 0.0.1
 Summary: Python batch renamer.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-renamer
 License: MIT
 Keywords: rename,batch,renamer
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

