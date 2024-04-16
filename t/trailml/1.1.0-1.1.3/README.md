# Comparing `tmp/trailml-1.1.0.tar.gz` & `tmp/trailml-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trailml-1.1.0.tar", last modified: Mon Mar 11 09:11:13 2024, max compression
+gzip compressed data, was "trailml-1.1.3.tar", last modified: Mon Apr 15 08:38:42 2024, max compression
```

## Comparing `trailml-1.1.0.tar` & `trailml-1.1.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:11:13.835872 trailml-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-03-11 09:11:13.835872 trailml-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-11 09:11:06.000000 trailml-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-11 09:11:06.000000 trailml-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 09:11:13.835872 trailml-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:11:13.831872 trailml-1.1.0/trail/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-11 09:11:06.000000 trailml-1.1.0/trail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:11:13.831872 trailml-1.1.0/trail/exception/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 09:11:06.000000 trailml-1.1.0/trail/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-11 09:11:06.000000 trailml-1.1.0/trail/exception/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-11 09:11:06.000000 trailml-1.1.0/trail/exception/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-11 09:11:06.000000 trailml-1.1.0/trail/exception/trail.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-11 09:11:06.000000 trailml-1.1.0/trail/exception/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:11:13.831872 trailml-1.1.0/trail/libconfig/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-11 09:11:06.000000 trailml-1.1.0/trail/libconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-11 09:11:06.000000 trailml-1.1.0/trail/libconfig/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-03-11 09:11:06.000000 trailml-1.1.0/trail/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-03-11 09:11:06.000000 trailml-1.1.0/trail/trail.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:11:13.831872 trailml-1.1.0/trail/userconfig/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-11 09:11:06.000000 trailml-1.1.0/trail/userconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-03-11 09:11:06.000000 trailml-1.1.0/trail/userconfig/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-03-11 09:11:06.000000 trailml-1.1.0/trail/userconfig/init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:11:13.835872 trailml-1.1.0/trail/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 09:11:06.000000 trailml-1.1.0/trail/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-03-11 09:11:06.000000 trailml-1.1.0/trail/util/add_test_coverage_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-11 09:11:06.000000 trailml-1.1.0/trail/util/add_test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-03-11 09:11:06.000000 trailml-1.1.0/trail/util/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-11 09:11:06.000000 trailml-1.1.0/trail/util/gql_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-11 09:11:06.000000 trailml-1.1.0/trail/util/new_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-03-11 09:11:06.000000 trailml-1.1.0/trail/util/upload_artifacts_from_notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-03-11 09:11:06.000000 trailml-1.1.0/trail/util/uploads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:11:13.835872 trailml-1.1.0/trailml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-03-11 09:11:13.000000 trailml-1.1.0/trailml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-11 09:11:13.000000 trailml-1.1.0/trailml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 09:11:13.000000 trailml-1.1.0/trailml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-11 09:11:13.000000 trailml-1.1.0/trailml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-11 09:11:13.000000 trailml-1.1.0/trailml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-11 09:11:13.000000 trailml-1.1.0/trailml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:38:42.850130 trailml-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-15 08:38:42.850130 trailml-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-15 08:38:36.000000 trailml-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-15 08:38:36.000000 trailml-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:38:42.850130 trailml-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:38:42.842130 trailml-1.1.3/trail/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-15 08:38:36.000000 trailml-1.1.3/trail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:38:42.846130 trailml-1.1.3/trail/exception/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:38:36.000000 trailml-1.1.3/trail/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-15 08:38:36.000000 trailml-1.1.3/trail/exception/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 08:38:36.000000 trailml-1.1.3/trail/exception/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-15 08:38:36.000000 trailml-1.1.3/trail/exception/trail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-15 08:38:36.000000 trailml-1.1.3/trail/exception/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:38:42.846130 trailml-1.1.3/trail/libconfig/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-15 08:38:36.000000 trailml-1.1.3/trail/libconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-15 08:38:36.000000 trailml-1.1.3/trail/libconfig/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-15 08:38:36.000000 trailml-1.1.3/trail/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12017 2024-04-15 08:38:36.000000 trailml-1.1.3/trail/trail.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:38:42.846130 trailml-1.1.3/trail/userconfig/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-15 08:38:36.000000 trailml-1.1.3/trail/userconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-15 08:38:36.000000 trailml-1.1.3/trail/userconfig/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-15 08:38:36.000000 trailml-1.1.3/trail/userconfig/init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:38:42.846130 trailml-1.1.3/trail/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:38:36.000000 trailml-1.1.3/trail/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-15 08:38:36.000000 trailml-1.1.3/trail/util/add_test_coverage_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-15 08:38:36.000000 trailml-1.1.3/trail/util/add_test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-15 08:38:36.000000 trailml-1.1.3/trail/util/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-15 08:38:36.000000 trailml-1.1.3/trail/util/gql_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-15 08:38:36.000000 trailml-1.1.3/trail/util/new_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-15 08:38:36.000000 trailml-1.1.3/trail/util/upload_artifacts_from_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-04-15 08:38:36.000000 trailml-1.1.3/trail/util/uploads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:38:42.850130 trailml-1.1.3/trailml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-15 08:38:42.000000 trailml-1.1.3/trailml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-15 08:38:42.000000 trailml-1.1.3/trailml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:38:42.000000 trailml-1.1.3/trailml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 08:38:42.000000 trailml-1.1.3/trailml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 08:38:42.000000 trailml-1.1.3/trailml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 08:38:42.000000 trailml-1.1.3/trailml.egg-info/top_level.txt
```

### Comparing `trailml-1.1.0/PKG-INFO` & `trailml-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trailml
-Version: 1.1.0
+Version: 1.1.3
 Summary: Trail ML library
 Author-email: Trail ML <python@trail-ml.com>
 Project-URL: Homepage, https://trail-ml.com
 Project-URL: Bug Tracker, https://github.com/trail-ml/bugtracker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,15 @@
 Requires-Dist: aiohttp
 Requires-Dist: mlflow
 Requires-Dist: pyrebase4
 Requires-Dist: PyYAML
 Requires-Dist: requests-toolbelt==0.10.1
 Requires-Dist: sentry-sdk
 Requires-Dist: tqdm
+Requires-Dist: nbformat
 
 # Trail
 
 Trail brings more transparency to your ML experiments.
 Start by using MLflow to track experiments and follow the steps below.
 
 # Installation
```

### Comparing `trailml-1.1.0/README.md` & `trailml-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `trailml-1.1.0/pyproject.toml` & `trailml-1.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "trailml"
-version = "1.1.0"
+version = "1.1.3"
 authors = [
   { name="Trail ML", email="python@trail-ml.com" },
 ]
 description = "Trail ML library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -20,15 +20,16 @@
     "gql",
     "aiohttp",
     "mlflow",
     "pyrebase4",
     "PyYAML",
     "requests-toolbelt==0.10.1",
     "sentry-sdk",
-    "tqdm"
+    "tqdm",
+    'nbformat'
 ]
 
 [project.urls]
 "Homepage" = "https://trail-ml.com"
 "Bug Tracker" = "https://github.com/trail-ml/bugtracker/issues"
 
 [project.scripts]
```

### Comparing `trailml-1.1.0/trail/__init__.py` & `trailml-1.1.3/trail/__init__.py`

 * *Files identical despite different names*

### Comparing `trailml-1.1.0/trail/libconfig/config.py` & `trailml-1.1.3/trail/libconfig/config.py`

 * *Files identical despite different names*

### Comparing `trailml-1.1.0/trail/main.py` & `trailml-1.1.3/trail/main.py`

 * *Files identical despite different names*

### Comparing `trailml-1.1.0/trail/trail.py` & `trailml-1.1.3/trail/trail.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 import sys
 import time
 from collections import defaultdict
 from typing import Union
 
 import mlflow
 import sentry_sdk
-from gql import gql
-from gql.transport.exceptions import TransportQueryError
 from mlflow.entities import Run
 from mlflow.tracking import MlflowClient
 
 from trail.exception.trail import RemoteTrailException, TrailUnavailableException
 from trail.userconfig import userconfig
 from trail.util import uploads
 
@@ -161,24 +159,24 @@
 
             return build_gql_client()
 
         return self.__client
 
     def _execute(
             self,
-            document: str,
+            query: str,
             variable_values: dict,
             error_message: Union[str, None] = None
     ):
         try:
             return self._client.execute(
-                document=gql(document),
+                query=query,
                 variable_values=variable_values,
             )
-        except TransportQueryError as e:
+        except Exception as e:
             if is_development_environment():
                 raise RemoteTrailException(error_message or "") from e
             else:
                 sentry_sdk.capture_exception(e)
 
             if error_message:
                 print(RemoteTrailException(error_message), file=sys.stderr)
@@ -205,15 +203,15 @@
         for key, value in converted_params.items():
             try:
                 converted_params[key] = float(value)
             except ValueError as e:
                 sentry_sdk.capture_exception(e)
 
         result = self._execute(
-            document=self.ADD_EXPERIMENT_MUTATION,
+            query=self.ADD_EXPERIMENT_MUTATION,
             variable_values={
                 "projectId": self._project_id,
                 "parentExperimentId": self._parent_experiment_id,
                 "title": self._experiment_title,
                 "comments": "",
                 "instanceRunParameters": converted_params,
                 "instanceRunMetrics": run.data.metrics,
@@ -250,15 +248,15 @@
         for metric in metrics:
             metrics_history.append({"metricName": metric, "history": metrics[metric]})
 
         return metrics_history
 
     def _upload_artifact(self, data: bytes, name: str, tags: list, call_site_key: str):
         self._execute(
-            document=self.PUT_ARTIFACT_MUTATION,
+            query=self.PUT_ARTIFACT_MUTATION,
             variable_values={
                 "experimentId": self._parent_experiment_id,
                 "name": name,
                 "base64Data": base64.b64encode(data).decode(),
                 "tags": tags,
                 "callSiteKey": call_site_key,
             },
```

### Comparing `trailml-1.1.0/trail/userconfig/__init__.py` & `trailml-1.1.3/trail/userconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `trailml-1.1.0/trail/userconfig/config.py` & `trailml-1.1.3/trail/userconfig/config.py`

 * *Files identical despite different names*

### Comparing `trailml-1.1.0/trail/userconfig/init.py` & `trailml-1.1.3/trail/userconfig/init.py`

 * *Files identical despite different names*

### Comparing `trailml-1.1.0/trail/util/add_test_coverage_results.py` & `trailml-1.1.3/trail/util/add_test_coverage_results.py`

 * *Files identical despite different names*

### Comparing `trailml-1.1.0/trail/util/add_test_results.py` & `trailml-1.1.3/trail/util/add_test_results.py`

 * *Files identical despite different names*

### Comparing `trailml-1.1.0/trail/util/auth.py` & `trailml-1.1.3/trail/util/auth.py`

 * *Files identical despite different names*

### Comparing `trailml-1.1.0/trail/util/upload_artifacts_from_notebook.py` & `trailml-1.1.3/trail/util/upload_artifacts_from_notebook.py`

 * *Files identical despite different names*

### Comparing `trailml-1.1.0/trail/util/uploads.py` & `trailml-1.1.3/trail/util/uploads.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import os
 import sys
 from enum import Enum
 from pathlib import Path
 
 import requests
 import sentry_sdk
-from gql import gql
 from gql.transport.exceptions import TransportQueryError
 from requests import RequestException
 from tqdm import tqdm
 
 from trail.exception.trail import RemoteTrailException, \
     TrailUnavailableException
 from trail.exception.upload import UploadError
@@ -146,15 +145,15 @@
         "projectId": project_id,
         "files": files,
         "experimentId": experiment_id,
     }
     client = build_gql_client()
     try:
         response = client.execute(
-            document=gql(ADD_SOURCE_FILES_MUTATION),
+            query=ADD_SOURCE_FILES_MUTATION,
             variable_values=variables,
         )
         return response['addSourceFiles']['presignedUrls']
 
     except TransportQueryError as e:
         if is_development_environment():
             raise RemoteTrailException("Could not register files in terra") from e
```

### Comparing `trailml-1.1.0/trailml.egg-info/PKG-INFO` & `trailml-1.1.3/trailml.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trailml
-Version: 1.1.0
+Version: 1.1.3
 Summary: Trail ML library
 Author-email: Trail ML <python@trail-ml.com>
 Project-URL: Homepage, https://trail-ml.com
 Project-URL: Bug Tracker, https://github.com/trail-ml/bugtracker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,15 @@
 Requires-Dist: aiohttp
 Requires-Dist: mlflow
 Requires-Dist: pyrebase4
 Requires-Dist: PyYAML
 Requires-Dist: requests-toolbelt==0.10.1
 Requires-Dist: sentry-sdk
 Requires-Dist: tqdm
+Requires-Dist: nbformat
 
 # Trail
 
 Trail brings more transparency to your ML experiments.
 Start by using MLflow to track experiments and follow the steps below.
 
 # Installation
```

### Comparing `trailml-1.1.0/trailml.egg-info/SOURCES.txt` & `trailml-1.1.3/trailml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

