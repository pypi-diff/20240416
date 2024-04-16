# Comparing `tmp/decthings-model-0.0.2.tar.gz` & `tmp/decthings_model-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decthings-model-0.0.2.tar", last modified: Mon Apr  1 23:08:34 2024, max compression
+gzip compressed data, was "decthings_model-0.0.3.tar", last modified: Tue Apr 16 09:15:40 2024, max compression
```

## Comparing `decthings-model-0.0.2.tar` & `decthings_model-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-01 23:08:34.609478 decthings-model-0.0.2/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1066 2024-04-01 19:17:45.000000 decthings-model-0.0.2/LICENSE
--rw-r--r--   0 viktor    (1000) viktor    (1000)     1356 2024-04-01 23:08:34.609478 decthings-model-0.0.2/PKG-INFO
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      921 2024-04-01 22:20:00.000000 decthings-model-0.0.2/README.md
--rw-r--r--   0 viktor    (1000) viktor    (1000)      421 2024-04-01 23:07:15.000000 decthings-model-0.0.2/pyproject.toml
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       38 2024-04-01 23:08:34.609478 decthings-model-0.0.2/setup.cfg
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-01 23:08:34.601478 decthings-model-0.0.2/src/
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-01 23:08:34.605478 decthings-model-0.0.2/src/decthings_model/
--rw-r--r--   0 viktor    (1000) viktor    (1000)        0 2024-04-01 22:16:52.000000 decthings-model-0.0.2/src/decthings_model/__init__.py
--rw-r--r--   0 viktor    (1000) viktor    (1000)       34 2024-04-01 23:05:52.000000 decthings-model-0.0.2/src/decthings_model/__main__.py
--rw-r--r--   0 viktor    (1000) viktor    (1000)    11294 2024-04-01 22:10:32.000000 decthings-model-0.0.2/src/decthings_model/model.py
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-01 23:08:34.605478 decthings-model-0.0.2/src/decthings_model/run/
--rw-r--r--   0 viktor    (1000) viktor    (1000)     6642 2024-04-01 21:49:42.000000 decthings-model-0.0.2/src/decthings_model/run/dataloader.py
--rw-r--r--   0 viktor    (1000) viktor    (1000)    14621 2024-04-01 22:02:51.000000 decthings-model-0.0.2/src/decthings_model/run/run.py
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-01 23:08:34.609478 decthings-model-0.0.2/src/decthings_model.egg-info/
--rw-r--r--   0 viktor    (1000) viktor    (1000)     1356 2024-04-01 23:08:34.000000 decthings-model-0.0.2/src/decthings_model.egg-info/PKG-INFO
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      408 2024-04-01 23:08:34.000000 decthings-model-0.0.2/src/decthings_model.egg-info/SOURCES.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)        1 2024-04-01 23:08:34.000000 decthings-model-0.0.2/src/decthings_model.egg-info/dependency_links.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       21 2024-04-01 23:08:34.000000 decthings-model-0.0.2/src/decthings_model.egg-info/requires.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       16 2024-04-01 23:08:34.000000 decthings-model-0.0.2/src/decthings_model.egg-info/top_level.txt
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-16 09:15:40.666765 decthings_model-0.0.3/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1066 2024-04-16 09:05:15.000000 decthings_model-0.0.3/LICENSE
+-rw-r--r--   0 viktor    (1000) viktor    (1000)     1464 2024-04-16 09:15:40.666765 decthings_model-0.0.3/PKG-INFO
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1029 2024-04-16 09:05:15.000000 decthings_model-0.0.3/README.md
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      421 2024-04-16 09:15:23.000000 decthings_model-0.0.3/pyproject.toml
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       38 2024-04-16 09:15:40.666765 decthings_model-0.0.3/setup.cfg
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-16 09:15:40.666765 decthings_model-0.0.3/src/
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-16 09:15:40.666765 decthings_model-0.0.3/src/decthings_model/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       21 2024-04-16 09:09:55.000000 decthings_model-0.0.3/src/decthings_model/__init__.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       34 2024-04-16 09:05:15.000000 decthings_model-0.0.3/src/decthings_model/__main__.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    11294 2024-04-16 09:05:15.000000 decthings_model-0.0.3/src/decthings_model/model.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-16 09:15:40.666765 decthings_model-0.0.3/src/decthings_model/run/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     6642 2024-04-16 09:05:15.000000 decthings_model-0.0.3/src/decthings_model/run/dataloader.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    14621 2024-04-16 09:05:15.000000 decthings_model-0.0.3/src/decthings_model/run/run.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-16 09:15:40.666765 decthings_model-0.0.3/src/decthings_model.egg-info/
+-rw-r--r--   0 viktor    (1000) viktor    (1000)     1464 2024-04-16 09:15:40.000000 decthings_model-0.0.3/src/decthings_model.egg-info/PKG-INFO
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      408 2024-04-16 09:15:40.000000 decthings_model-0.0.3/src/decthings_model.egg-info/SOURCES.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)        1 2024-04-16 09:15:40.000000 decthings_model-0.0.3/src/decthings_model.egg-info/dependency_links.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       21 2024-04-16 09:15:40.000000 decthings_model-0.0.3/src/decthings_model.egg-info/requires.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       16 2024-04-16 09:15:40.000000 decthings_model-0.0.3/src/decthings_model.egg-info/top_level.txt
```

### Comparing `decthings-model-0.0.2/LICENSE` & `decthings_model-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `decthings-model-0.0.2/PKG-INFO` & `decthings_model-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: decthings-model
-Version: 0.0.2
+Version: 0.0.3
 Summary: Create a Decthings model using Python
 Project-URL: Homepage, https://github.com/decthings/model-py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: decthings-api>=0.0.1
 
 <img src="https://decthings.com/logo.png" alt="decthings logo" width="33%" />
 
 ## Decthings model using Python
 
+[![PyPI version](https://badge.fury.io/py/decthings-model.svg)](https://pypi.org/project/decthings-model/)
+
 Use Python to create a Decthings model.
 
 ### Setup
 
 Create a Decthings model using Python by going to the [create model page](https://app.decthings.com/models/create) on Decthings, and select Python as the language. This package is then by default installed and used within your model.
 
 Manually, you can install this package using `pip3 install decthings-model`.
```

### Comparing `decthings-model-0.0.2/src/decthings_model/model.py` & `decthings_model-0.0.3/src/decthings_model/model.py`

 * *Files identical despite different names*

### Comparing `decthings-model-0.0.2/src/decthings_model/run/dataloader.py` & `decthings_model-0.0.3/src/decthings_model/run/dataloader.py`

 * *Files identical despite different names*

### Comparing `decthings-model-0.0.2/src/decthings_model/run/run.py` & `decthings_model-0.0.3/src/decthings_model/run/run.py`

 * *Files identical despite different names*

### Comparing `decthings-model-0.0.2/src/decthings_model.egg-info/PKG-INFO` & `decthings_model-0.0.3/src/decthings_model.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: decthings-model
-Version: 0.0.2
+Version: 0.0.3
 Summary: Create a Decthings model using Python
 Project-URL: Homepage, https://github.com/decthings/model-py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: decthings-api>=0.0.1
 
 <img src="https://decthings.com/logo.png" alt="decthings logo" width="33%" />
 
 ## Decthings model using Python
 
+[![PyPI version](https://badge.fury.io/py/decthings-model.svg)](https://pypi.org/project/decthings-model/)
+
 Use Python to create a Decthings model.
 
 ### Setup
 
 Create a Decthings model using Python by going to the [create model page](https://app.decthings.com/models/create) on Decthings, and select Python as the language. This package is then by default installed and used within your model.
 
 Manually, you can install this package using `pip3 install decthings-model`.
```

