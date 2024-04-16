# Comparing `tmp/filerev-0.0.1.tar.gz` & `tmp/filerev-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filerev-0.0.1.tar", max compression
+gzip compressed data, was "filerev-0.0.1.1.tar", max compression
```

## Comparing `filerev-0.0.1.tar` & `filerev-0.0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 filerev-0.0.1/LICENSE
--rw-r--r--   0        0        0     1399 2024-04-16 13:14:33.651061 filerev-0.0.1/filerev.py
--rw-r--r--   0        0        0     1095 2024-04-16 13:03:25.776208 filerev-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      173 2024-04-16 13:03:42.719892 filerev-0.0.1/readme.md
--rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 filerev-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 filerev-0.0.1.1/LICENSE
+-rw-r--r--   0        0        0     1399 2024-04-16 13:14:33.651061 filerev-0.0.1.1/filerev.py
+-rw-r--r--   0        0        0     1097 2024-04-16 14:55:05.139268 filerev-0.0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      173 2024-04-16 13:03:42.719892 filerev-0.0.1.1/readme.md
+-rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 filerev-0.0.1.1/PKG-INFO
```

### Comparing `filerev-0.0.1/LICENSE` & `filerev-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `filerev-0.0.1/filerev.py` & `filerev-0.0.1.1/filerev.py`

 * *Files identical despite different names*

### Comparing `filerev-0.0.1/pyproject.toml` & `filerev-0.0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "filerev"
-version = "0.0.1"
+version = "0.0.1.1"
 description = "Reversed iterator for files."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/filerev"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/filerev"
 keywords = ["file", "reverse", "iter"]
```

### Comparing `filerev-0.0.1/PKG-INFO` & `filerev-0.0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filerev
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: Reversed iterator for files.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/filerev
 License: MIT
 Keywords: file,reverse,iter
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
```

