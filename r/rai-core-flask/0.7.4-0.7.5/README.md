# Comparing `tmp/rai_core_flask-0.7.4.tar.gz` & `tmp/rai_core_flask-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rai_core_flask-0.7.4.tar", last modified: Thu Feb 15 17:57:06 2024, max compression
+gzip compressed data, was "rai_core_flask-0.7.5.tar", last modified: Tue Apr 16 05:43:29 2024, max compression
```

## Comparing `rai_core_flask-0.7.4.tar` & `rai_core_flask-0.7.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:57:06.741058 rai_core_flask-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-02-15 17:56:48.000000 rai_core_flask-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-15 17:56:48.000000 rai_core_flask-0.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-02-15 17:57:06.741058 rai_core_flask-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-02-15 17:56:48.000000 rai_core_flask-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:57:06.737058 rai_core_flask-0.7.4/rai_core_flask/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-15 17:56:48.000000 rai_core_flask-0.7.4/rai_core_flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-02-15 17:56:48.000000 rai_core_flask-0.7.4/rai_core_flask/environment_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:57:06.741058 rai_core_flask-0.7.4/rai_core_flask/environments/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-02-15 17:56:48.000000 rai_core_flask-0.7.4/rai_core_flask/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-02-15 17:56:48.000000 rai_core_flask-0.7.4/rai_core_flask/environments/azure_nb_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-02-15 17:56:48.000000 rai_core_flask-0.7.4/rai_core_flask/environments/base_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-02-15 17:56:48.000000 rai_core_flask-0.7.4/rai_core_flask/environments/credentialed_vm_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-02-15 17:56:48.000000 rai_core_flask-0.7.4/rai_core_flask/environments/databricks_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-02-15 17:56:48.000000 rai_core_flask-0.7.4/rai_core_flask/environments/local_ipython_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-02-15 17:56:48.000000 rai_core_flask-0.7.4/rai_core_flask/environments/public_vm_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-02-15 17:56:48.000000 rai_core_flask-0.7.4/rai_core_flask/flask_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:57:06.741058 rai_core_flask-0.7.4/rai_core_flask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-02-15 17:57:06.000000 rai_core_flask-0.7.4/rai_core_flask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-02-15 17:57:06.000000 rai_core_flask-0.7.4/rai_core_flask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 17:57:06.000000 rai_core_flask-0.7.4/rai_core_flask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-15 17:57:06.000000 rai_core_flask-0.7.4/rai_core_flask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-15 17:57:06.000000 rai_core_flask-0.7.4/rai_core_flask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-15 17:56:48.000000 rai_core_flask-0.7.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 17:57:06.741058 rai_core_flask-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-02-15 17:56:48.000000 rai_core_flask-0.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:57:06.741058 rai_core_flask-0.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-02-15 17:56:48.000000 rai_core_flask-0.7.4/tests/test_environment_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-02-15 17:56:48.000000 rai_core_flask-0.7.4/tests/test_flask_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:43:29.235754 rai_core_flask-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-16 05:43:11.000000 rai_core_flask-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 05:43:11.000000 rai_core_flask-0.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-16 05:43:29.235754 rai_core_flask-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-16 05:43:11.000000 rai_core_flask-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:43:29.231754 rai_core_flask-0.7.5/rai_core_flask/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-16 05:43:11.000000 rai_core_flask-0.7.5/rai_core_flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-16 05:43:11.000000 rai_core_flask-0.7.5/rai_core_flask/environment_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:43:29.235754 rai_core_flask-0.7.5/rai_core_flask/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-16 05:43:11.000000 rai_core_flask-0.7.5/rai_core_flask/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-16 05:43:11.000000 rai_core_flask-0.7.5/rai_core_flask/environments/azure_nb_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-16 05:43:11.000000 rai_core_flask-0.7.5/rai_core_flask/environments/base_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-16 05:43:11.000000 rai_core_flask-0.7.5/rai_core_flask/environments/credentialed_vm_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-16 05:43:11.000000 rai_core_flask-0.7.5/rai_core_flask/environments/databricks_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-16 05:43:11.000000 rai_core_flask-0.7.5/rai_core_flask/environments/local_ipython_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-16 05:43:11.000000 rai_core_flask-0.7.5/rai_core_flask/environments/public_vm_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-16 05:43:11.000000 rai_core_flask-0.7.5/rai_core_flask/flask_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:43:29.235754 rai_core_flask-0.7.5/rai_core_flask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-16 05:43:29.000000 rai_core_flask-0.7.5/rai_core_flask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-16 05:43:29.000000 rai_core_flask-0.7.5/rai_core_flask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 05:43:29.000000 rai_core_flask-0.7.5/rai_core_flask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-16 05:43:29.000000 rai_core_flask-0.7.5/rai_core_flask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 05:43:29.000000 rai_core_flask-0.7.5/rai_core_flask.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-16 05:43:11.000000 rai_core_flask-0.7.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 05:43:29.235754 rai_core_flask-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-16 05:43:11.000000 rai_core_flask-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:43:29.235754 rai_core_flask-0.7.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-16 05:43:11.000000 rai_core_flask-0.7.5/tests/test_environment_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-16 05:43:11.000000 rai_core_flask-0.7.5/tests/test_flask_helper.py
```

### Comparing `rai_core_flask-0.7.4/LICENSE` & `rai_core_flask-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rai_core_flask-0.7.4/PKG-INFO` & `rai_core_flask-0.7.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rai_core_flask
-Version: 0.7.4
+Version: 0.7.5
 Summary: Responsible AI Core Flask Wrapper
 Home-page: 
 Author: Roman Lutz, Ke Xu, Xavier Fernandes
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -19,15 +19,15 @@
 Requires-Dist: flask-socketio
 Requires-Dist: ipython<=7.16.3; python_version <= "3.6"
 Requires-Dist: ipython>=7.31.1; python_version > "3.6"
 Requires-Dist: itsdangerous>=2.0.1
 Requires-Dist: greenlet>=1.1.2
 Requires-Dist: gevent>=21.12.0
 Requires-Dist: markupsafe<=2.1.2
-Requires-Dist: Werkzeug<=2.2.3
+Requires-Dist: Werkzeug<=3.0.2
 Provides-Extra: dev
 
 # rai_core_flask
 
 Provide environment detection for enabling Flask server without configuring at instantiation. Environments are implemented as classes that will either return None if the environment check fails, or return an object with all the appropriate environment settings if the check passes. The flask service can then use it to build out urls, attach required headers, and render inline visualizations with the correct methods.
 
 ## Installation
```

### Comparing `rai_core_flask-0.7.4/README.md` & `rai_core_flask-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `rai_core_flask-0.7.4/rai_core_flask/environment_detector.py` & `rai_core_flask-0.7.5/rai_core_flask/environment_detector.py`

 * *Files identical despite different names*

### Comparing `rai_core_flask-0.7.4/rai_core_flask/environments/__init__.py` & `rai_core_flask-0.7.5/rai_core_flask/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `rai_core_flask-0.7.4/rai_core_flask/environments/azure_nb_environment.py` & `rai_core_flask-0.7.5/rai_core_flask/environments/azure_nb_environment.py`

 * *Files identical despite different names*

### Comparing `rai_core_flask-0.7.4/rai_core_flask/environments/credentialed_vm_environment.py` & `rai_core_flask-0.7.5/rai_core_flask/environments/credentialed_vm_environment.py`

 * *Files identical despite different names*

### Comparing `rai_core_flask-0.7.4/rai_core_flask/environments/databricks_environment.py` & `rai_core_flask-0.7.5/rai_core_flask/environments/databricks_environment.py`

 * *Files identical despite different names*

### Comparing `rai_core_flask-0.7.4/rai_core_flask/environments/local_ipython_environment.py` & `rai_core_flask-0.7.5/rai_core_flask/environments/local_ipython_environment.py`

 * *Files identical despite different names*

### Comparing `rai_core_flask-0.7.4/rai_core_flask/environments/public_vm_environment.py` & `rai_core_flask-0.7.5/rai_core_flask/environments/public_vm_environment.py`

 * *Files identical despite different names*

### Comparing `rai_core_flask-0.7.4/rai_core_flask/flask_helper.py` & `rai_core_flask-0.7.5/rai_core_flask/flask_helper.py`

 * *Files identical despite different names*

### Comparing `rai_core_flask-0.7.4/rai_core_flask.egg-info/PKG-INFO` & `rai_core_flask-0.7.5/rai_core_flask.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rai_core_flask
-Version: 0.7.4
+Version: 0.7.5
 Summary: Responsible AI Core Flask Wrapper
 Home-page: 
 Author: Roman Lutz, Ke Xu, Xavier Fernandes
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -19,15 +19,15 @@
 Requires-Dist: flask-socketio
 Requires-Dist: ipython<=7.16.3; python_version <= "3.6"
 Requires-Dist: ipython>=7.31.1; python_version > "3.6"
 Requires-Dist: itsdangerous>=2.0.1
 Requires-Dist: greenlet>=1.1.2
 Requires-Dist: gevent>=21.12.0
 Requires-Dist: markupsafe<=2.1.2
-Requires-Dist: Werkzeug<=2.2.3
+Requires-Dist: Werkzeug<=3.0.2
 Provides-Extra: dev
 
 # rai_core_flask
 
 Provide environment detection for enabling Flask server without configuring at instantiation. Environments are implemented as classes that will either return None if the environment check fails, or return an object with all the appropriate environment settings if the check passes. The flask service can then use it to build out urls, attach required headers, and render inline visualizations with the correct methods.
 
 ## Installation
```

### Comparing `rai_core_flask-0.7.4/rai_core_flask.egg-info/SOURCES.txt` & `rai_core_flask-0.7.5/rai_core_flask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rai_core_flask-0.7.4/setup.py` & `rai_core_flask-0.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Microsoft Corporation
 # Licensed under the MIT license.
 
 import setuptools
 
 # The version must be incremented every time we push an update to pypi (but
 # not before)
-VERSION = "0.7.4"
+VERSION = "0.7.5"
 
 # supply contents of our README file as our package's long description
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 requirements = []
```

### Comparing `rai_core_flask-0.7.4/tests/test_environment_detector.py` & `rai_core_flask-0.7.5/tests/test_environment_detector.py`

 * *Files identical despite different names*

### Comparing `rai_core_flask-0.7.4/tests/test_flask_helper.py` & `rai_core_flask-0.7.5/tests/test_flask_helper.py`

 * *Files identical despite different names*

