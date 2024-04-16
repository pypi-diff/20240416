# Comparing `tmp/lunaticoastro_dragonfly_controller-0.3.0.tar.gz` & `tmp/lunaticoastro_dragonfly_controller-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lunaticoastro_dragonfly_controller-0.3.0.tar", max compression
+gzip compressed data, was "lunaticoastro_dragonfly_controller-0.5.0.tar", max compression
```

## Comparing `lunaticoastro_dragonfly_controller-0.3.0.tar` & `lunaticoastro_dragonfly_controller-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2024-04-16 00:21:29.388517 lunaticoastro_dragonfly_controller-0.3.0/LICENSE
--rw-r--r--   0        0        0     2831 2024-04-16 00:21:29.388517 lunaticoastro_dragonfly_controller-0.3.0/README.md
--rw-r--r--   0        0        0     8644 2024-04-16 00:21:29.388517 lunaticoastro_dragonfly_controller-0.3.0/dragonfly_dome/controller.py
--rw-r--r--   0        0        0     1349 2024-04-16 00:21:29.388517 lunaticoastro_dragonfly_controller-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3429 1970-01-01 00:00:00.000000 lunaticoastro_dragonfly_controller-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-16 00:28:53.804105 lunaticoastro_dragonfly_controller-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2831 2024-04-16 00:28:53.804105 lunaticoastro_dragonfly_controller-0.5.0/README.md
+-rw-r--r--   0        0        0     8644 2024-04-16 00:28:53.804105 lunaticoastro_dragonfly_controller-0.5.0/dragonfly_dome/controller.py
+-rw-r--r--   0        0        0     1349 2024-04-16 00:28:53.804105 lunaticoastro_dragonfly_controller-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3429 1970-01-01 00:00:00.000000 lunaticoastro_dragonfly_controller-0.5.0/PKG-INFO
```

### Comparing `lunaticoastro_dragonfly_controller-0.3.0/LICENSE` & `lunaticoastro_dragonfly_controller-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lunaticoastro_dragonfly_controller-0.3.0/README.md` & `lunaticoastro_dragonfly_controller-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `lunaticoastro_dragonfly_controller-0.3.0/dragonfly_dome/controller.py` & `lunaticoastro_dragonfly_controller-0.5.0/dragonfly_dome/controller.py`

 * *Files identical despite different names*

### Comparing `lunaticoastro_dragonfly_controller-0.3.0/pyproject.toml` & `lunaticoastro_dragonfly_controller-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lunaticoastro-dragonfly-controller"
-version = "0.3.0"
+version = "0.5.0"
 description = "Python Lib to control lunaticoastro dragonfly"
 readme = "README.md"
 authors = ["Robert Bradley <robbrad182@gmail.com>"]
 packages = [
     { include = "dragonfly_dome", from = "." },
 ]
```

### Comparing `lunaticoastro_dragonfly_controller-0.3.0/PKG-INFO` & `lunaticoastro_dragonfly_controller-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lunaticoastro-dragonfly-controller
-Version: 0.3.0
+Version: 0.5.0
 Summary: Python Lib to control lunaticoastro dragonfly
 Author: Robert Bradley
 Author-email: robbrad182@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

