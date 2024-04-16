# Comparing `tmp/haggregate-3.0.2.tar.gz` & `tmp/haggregate-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haggregate-3.0.2.tar", last modified: Wed Dec 20 11:14:37 2023, max compression
+gzip compressed data, was "haggregate-3.0.3.tar", last modified: Tue Apr 16 20:05:17 2024, max compression
```

## Comparing `haggregate-3.0.2.tar` & `haggregate-3.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-12-20 11:14:37.104996 haggregate-3.0.2/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1476 2023-12-20 11:08:57.000000 haggregate-3.0.2/HISTORY.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)       23 2022-12-03 16:55:59.000000 haggregate-3.0.2/LICENSE
--rw-r--r--   0 anthony   (1000) anthony   (1000)      199 2022-03-05 20:41:23.000000 haggregate-3.0.2/MANIFEST.in
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3041 2023-12-20 11:14:37.104996 haggregate-3.0.2/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      736 2022-03-05 20:41:23.000000 haggregate-3.0.2/README.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-12-20 11:14:37.100996 haggregate-3.0.2/docs/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3931 2022-03-05 20:41:23.000000 haggregate-3.0.2/docs/api.rst
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     5163 2022-03-05 20:41:23.000000 haggregate-3.0.2/docs/conf.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1230 2022-12-03 16:55:59.000000 haggregate-3.0.2/docs/copyright.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)       28 2022-03-05 20:41:23.000000 haggregate-3.0.2/docs/history.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      174 2022-11-13 20:46:58.000000 haggregate-3.0.2/docs/index.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8445 2022-03-05 20:41:23.000000 haggregate-3.0.2/docs/usage.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-12-20 11:14:37.100996 haggregate-3.0.2/haggregate/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      177 2023-12-20 11:13:18.000000 haggregate-3.0.2/haggregate/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3038 2022-12-03 16:55:59.000000 haggregate-3.0.2/haggregate/cli.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4949 2022-12-03 06:06:47.000000 haggregate-3.0.2/haggregate/haggregate.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)   399470 2022-12-03 16:57:22.000000 haggregate-3.0.2/haggregate/regularize.c
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-12-20 11:14:37.100996 haggregate-3.0.2/haggregate.egg-info/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3041 2023-12-20 11:14:36.000000 haggregate-3.0.2/haggregate.egg-info/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      568 2023-12-20 11:14:37.000000 haggregate-3.0.2/haggregate.egg-info/SOURCES.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2023-12-20 11:14:36.000000 haggregate-3.0.2/haggregate.egg-info/dependency_links.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       51 2023-12-20 11:14:36.000000 haggregate-3.0.2/haggregate.egg-info/entry_points.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2022-11-13 10:11:23.000000 haggregate-3.0.2/haggregate.egg-info/not-zip-safe
--rw-r--r--   0 anthony   (1000) anthony   (1000)       30 2023-12-20 11:14:36.000000 haggregate-3.0.2/haggregate.egg-info/requires.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       11 2023-12-20 11:14:36.000000 haggregate-3.0.2/haggregate.egg-info/top_level.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2023-12-20 11:14:37.104996 haggregate-3.0.2/setup.cfg
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     3134 2023-12-20 11:08:57.000000 haggregate-3.0.2/setup.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-12-20 11:14:37.104996 haggregate-3.0.2/tests/
--rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2022-03-05 20:41:23.000000 haggregate-3.0.2/tests/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4867 2022-12-03 16:58:54.000000 haggregate-3.0.2/tests/test_cli.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    11181 2022-12-03 16:55:59.000000 haggregate-3.0.2/tests/test_haggregate.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7021 2022-12-03 16:55:59.000000 haggregate-3.0.2/tests/test_regularize.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 20:05:17.310176 haggregate-3.0.3/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1539 2024-04-16 20:04:26.000000 haggregate-3.0.3/HISTORY.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       23 2022-12-03 16:55:59.000000 haggregate-3.0.3/LICENSE
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      199 2022-03-05 20:41:23.000000 haggregate-3.0.3/MANIFEST.in
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3104 2024-04-16 20:05:17.310176 haggregate-3.0.3/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      736 2022-03-05 20:41:23.000000 haggregate-3.0.3/README.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 20:05:17.310176 haggregate-3.0.3/docs/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3931 2022-03-05 20:41:23.000000 haggregate-3.0.3/docs/api.rst
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     5163 2022-03-05 20:41:23.000000 haggregate-3.0.3/docs/conf.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1230 2022-12-03 16:55:59.000000 haggregate-3.0.3/docs/copyright.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       28 2022-03-05 20:41:23.000000 haggregate-3.0.3/docs/history.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      174 2022-11-13 20:46:58.000000 haggregate-3.0.3/docs/index.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8445 2022-03-05 20:41:23.000000 haggregate-3.0.3/docs/usage.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 20:05:17.310176 haggregate-3.0.3/haggregate/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      177 2024-04-16 20:04:41.000000 haggregate-3.0.3/haggregate/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3038 2024-04-16 20:02:25.000000 haggregate-3.0.3/haggregate/cli.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4949 2022-12-03 06:06:47.000000 haggregate-3.0.3/haggregate/haggregate.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   399470 2022-12-03 16:57:22.000000 haggregate-3.0.3/haggregate/regularize.c
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 20:05:17.310176 haggregate-3.0.3/haggregate.egg-info/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3104 2024-04-16 20:05:17.000000 haggregate-3.0.3/haggregate.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      568 2024-04-16 20:05:17.000000 haggregate-3.0.3/haggregate.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-04-16 20:05:17.000000 haggregate-3.0.3/haggregate.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       51 2024-04-16 20:05:17.000000 haggregate-3.0.3/haggregate.egg-info/entry_points.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2022-11-13 10:11:23.000000 haggregate-3.0.3/haggregate.egg-info/not-zip-safe
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       30 2024-04-16 20:05:17.000000 haggregate-3.0.3/haggregate.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       11 2024-04-16 20:05:17.000000 haggregate-3.0.3/haggregate.egg-info/top_level.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2024-04-16 20:05:17.310176 haggregate-3.0.3/setup.cfg
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     3134 2024-04-16 20:04:26.000000 haggregate-3.0.3/setup.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 20:05:17.310176 haggregate-3.0.3/tests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2022-03-05 20:41:23.000000 haggregate-3.0.3/tests/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4867 2022-12-03 16:58:54.000000 haggregate-3.0.3/tests/test_cli.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    11181 2022-12-03 16:55:59.000000 haggregate-3.0.3/tests/test_haggregate.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7021 2022-12-03 16:55:59.000000 haggregate-3.0.3/tests/test_regularize.py
```

### Comparing `haggregate-3.0.2/HISTORY.rst` & `haggregate-3.0.3/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+3.0.3 (2024-04-16)
+==================
+
+- Allow htimeseries 7.
+
 3.0.2 (2023-12-20)
 ==================
 
 - Allow htimeseries 6.
 
 3.0.1 (2022-12-03)
 ==================
```

### Comparing `haggregate-3.0.2/PKG-INFO` & `haggregate-3.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haggregate
-Version: 3.0.2
+Version: 3.0.3
 Summary: Aggregates htimeseries to larger steps
 Home-page: https://github.com/openmeteo/haggregate
 Author: Antonis Christofides
 Author-email: antonis@antonischristofides.com
 License: GNU General Public License v3
 Keywords: haggregate
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 Requires-Dist: Click<9,>=7
-Requires-Dist: htimeseries<7,>=4
+Requires-Dist: htimeseries<8,>=4
 
 ==========
 haggregate
 ==========
 
 
 .. image:: https://img.shields.io/pypi/v/haggregate.svg
@@ -46,14 +46,19 @@
 * Documentation: https://haggregate.readthedocs.io.
 
 
 =======
 History
 =======
 
+3.0.3 (2024-04-16)
+==================
+
+- Allow htimeseries 7.
+
 3.0.2 (2023-12-20)
 ==================
 
 - Allow htimeseries 6.
 
 3.0.1 (2022-12-03)
 ==================
```

### Comparing `haggregate-3.0.2/README.rst` & `haggregate-3.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `haggregate-3.0.2/docs/api.rst` & `haggregate-3.0.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `haggregate-3.0.2/docs/conf.py` & `haggregate-3.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `haggregate-3.0.2/docs/copyright.rst` & `haggregate-3.0.3/docs/copyright.rst`

 * *Files identical despite different names*

### Comparing `haggregate-3.0.2/docs/usage.rst` & `haggregate-3.0.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `haggregate-3.0.2/haggregate/cli.py` & `haggregate-3.0.3/haggregate/cli.py`

 * *Files identical despite different names*

### Comparing `haggregate-3.0.2/haggregate/haggregate.py` & `haggregate-3.0.3/haggregate/haggregate.py`

 * *Files identical despite different names*

### Comparing `haggregate-3.0.2/haggregate/regularize.c` & `haggregate-3.0.3/haggregate/regularize.c`

 * *Files identical despite different names*

### Comparing `haggregate-3.0.2/haggregate.egg-info/PKG-INFO` & `haggregate-3.0.3/haggregate.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haggregate
-Version: 3.0.2
+Version: 3.0.3
 Summary: Aggregates htimeseries to larger steps
 Home-page: https://github.com/openmeteo/haggregate
 Author: Antonis Christofides
 Author-email: antonis@antonischristofides.com
 License: GNU General Public License v3
 Keywords: haggregate
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 Requires-Dist: Click<9,>=7
-Requires-Dist: htimeseries<7,>=4
+Requires-Dist: htimeseries<8,>=4
 
 ==========
 haggregate
 ==========
 
 
 .. image:: https://img.shields.io/pypi/v/haggregate.svg
@@ -46,14 +46,19 @@
 * Documentation: https://haggregate.readthedocs.io.
 
 
 =======
 History
 =======
 
+3.0.3 (2024-04-16)
+==================
+
+- Allow htimeseries 7.
+
 3.0.2 (2023-12-20)
 ==================
 
 - Allow htimeseries 6.
 
 3.0.1 (2022-12-03)
 ==================
```

### Comparing `haggregate-3.0.2/haggregate.egg-info/SOURCES.txt` & `haggregate-3.0.3/haggregate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `haggregate-3.0.2/setup.py` & `haggregate-3.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open("README.rst") as readme_file:
     readme = readme_file.read()
 
 with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
-requirements = ["Click>=7,<9", "htimeseries>=4,<7"]
+requirements = ["Click>=7,<9", "htimeseries>=4,<8"]
 
 setup_requirements = ["cython>=0.29,<0.30"]
 
 test_requirements = []
 
 
 def use_cython():
```

### Comparing `haggregate-3.0.2/tests/test_cli.py` & `haggregate-3.0.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `haggregate-3.0.2/tests/test_haggregate.py` & `haggregate-3.0.3/tests/test_haggregate.py`

 * *Files identical despite different names*

### Comparing `haggregate-3.0.2/tests/test_regularize.py` & `haggregate-3.0.3/tests/test_regularize.py`

 * *Files identical despite different names*

