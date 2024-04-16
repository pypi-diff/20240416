# Comparing `tmp/flowpyter-task-1.1.4.tar.gz` & `tmp/flowpyter-task-1.1.4.post0.dev12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowpyter-task-1.1.4.tar", last modified: Fri Apr  5 12:34:51 2024, max compression
+gzip compressed data, was "flowpyter-task-1.1.4.post0.dev12.tar", last modified: Tue Apr 16 12:42:24 2024, max compression
```

## Comparing `flowpyter-task-1.1.4.tar` & `flowpyter-task-1.1.4.post0.dev12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-05 12:34:51.454042 flowpyter-task-1.1.4/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2024-04-05 12:34:51.000000 flowpyter-task-1.1.4/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1334 2024-04-05 12:34:51.454042 flowpyter-task-1.1.4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2024-04-05 12:34:51.000000 flowpyter-task-1.1.4/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-04-05 12:34:51.000000 flowpyter-task-1.1.4/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      153 2024-04-05 12:34:51.454042 flowpyter-task-1.1.4/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2306 2024-04-05 12:34:51.000000 flowpyter-task-1.1.4/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-05 12:34:51.450042 flowpyter-task-1.1.4/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-05 12:34:51.454042 flowpyter-task-1.1.4/src/flowpyter_task.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1334 2024-04-05 12:34:51.000000 flowpyter-task-1.1.4/src/flowpyter_task.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      590 2024-04-05 12:34:51.000000 flowpyter-task-1.1.4/src/flowpyter_task.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-05 12:34:51.000000 flowpyter-task-1.1.4/src/flowpyter_task.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2024-04-05 12:34:51.000000 flowpyter-task-1.1.4/src/flowpyter_task.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2024-04-05 12:34:51.000000 flowpyter-task-1.1.4/src/flowpyter_task.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-04-05 12:34:51.000000 flowpyter-task-1.1.4/src/flowpyter_task.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-05 12:34:51.000000 flowpyter-task-1.1.4/src/flowpyter_task.egg-info/zip-safe
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-05 12:34:51.454042 flowpyter-task-1.1.4/src/flowpytertask/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      416 2024-04-05 12:34:51.000000 flowpyter-task-1.1.4/src/flowpytertask/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      497 2024-04-05 12:34:51.454042 flowpyter-task-1.1.4/src/flowpytertask/_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17940 2024-04-05 12:34:51.000000 flowpyter-task-1.1.4/src/flowpytertask/flowpytertask.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-05 12:34:51.454042 flowpyter-task-1.1.4/src/flowpytertask/plugins/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      242 2024-04-05 12:34:51.000000 flowpyter-task-1.1.4/src/flowpytertask/plugins/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      237 2024-04-05 12:34:51.000000 flowpyter-task-1.1.4/src/flowpytertask/plugins/base64_jinja.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-05 12:34:51.454042 flowpyter-task-1.1.4/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16165 2024-04-05 12:34:51.000000 flowpyter-task-1.1.4/tests/test_flowpyter_operator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7708 2024-04-05 12:34:51.000000 flowpyter-task-1.1.4/tests/test_integration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    86677 2024-04-05 12:34:51.000000 flowpyter-task-1.1.4/versioneer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-16 12:42:24.099397 flowpyter-task-1.1.4.post0.dev12/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2024-04-16 12:37:59.000000 flowpyter-task-1.1.4.post0.dev12/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1691 2024-04-16 12:42:24.099397 flowpyter-task-1.1.4.post0.dev12/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2024-04-16 12:37:59.000000 flowpyter-task-1.1.4.post0.dev12/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-04-16 12:37:59.000000 flowpyter-task-1.1.4.post0.dev12/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      153 2024-04-16 12:42:24.099397 flowpyter-task-1.1.4.post0.dev12/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2306 2024-04-16 12:37:59.000000 flowpyter-task-1.1.4.post0.dev12/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-16 12:42:24.095397 flowpyter-task-1.1.4.post0.dev12/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-16 12:42:24.099397 flowpyter-task-1.1.4.post0.dev12/src/flowpyter_task.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1691 2024-04-16 12:42:24.000000 flowpyter-task-1.1.4.post0.dev12/src/flowpyter_task.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      590 2024-04-16 12:42:24.000000 flowpyter-task-1.1.4.post0.dev12/src/flowpyter_task.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-16 12:42:24.000000 flowpyter-task-1.1.4.post0.dev12/src/flowpyter_task.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2024-04-16 12:42:24.000000 flowpyter-task-1.1.4.post0.dev12/src/flowpyter_task.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2024-04-16 12:42:24.000000 flowpyter-task-1.1.4.post0.dev12/src/flowpyter_task.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-04-16 12:42:24.000000 flowpyter-task-1.1.4.post0.dev12/src/flowpyter_task.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-16 12:42:24.000000 flowpyter-task-1.1.4.post0.dev12/src/flowpyter_task.egg-info/zip-safe
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-16 12:42:24.095397 flowpyter-task-1.1.4.post0.dev12/src/flowpytertask/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      416 2024-04-16 12:37:59.000000 flowpyter-task-1.1.4.post0.dev12/src/flowpytertask/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      508 2024-04-16 12:42:24.099397 flowpyter-task-1.1.4.post0.dev12/src/flowpytertask/_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17940 2024-04-16 12:37:59.000000 flowpyter-task-1.1.4.post0.dev12/src/flowpytertask/flowpytertask.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-16 12:42:24.099397 flowpyter-task-1.1.4.post0.dev12/src/flowpytertask/plugins/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      242 2024-04-16 12:37:59.000000 flowpyter-task-1.1.4.post0.dev12/src/flowpytertask/plugins/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      237 2024-04-16 12:37:59.000000 flowpyter-task-1.1.4.post0.dev12/src/flowpytertask/plugins/base64_jinja.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-16 12:42:24.099397 flowpyter-task-1.1.4.post0.dev12/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16165 2024-04-16 12:37:59.000000 flowpyter-task-1.1.4.post0.dev12/tests/test_flowpyter_operator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7708 2024-04-16 12:37:59.000000 flowpyter-task-1.1.4.post0.dev12/tests/test_integration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    86677 2024-04-16 12:37:59.000000 flowpyter-task-1.1.4.post0.dev12/versioneer.py
```

### Comparing `flowpyter-task-1.1.4/LICENSE` & `flowpyter-task-1.1.4.post0.dev12/LICENSE`

 * *Files identical despite different names*

### Comparing `flowpyter-task-1.1.4/PKG-INFO` & `flowpyter-task-1.1.4.post0.dev12/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 Metadata-Version: 2.1
 Name: flowpyter-task
-Version: 1.1.4
+Version: 1.1.4.post0.dev12
 Home-page: https://github.com/Flowminder/flowpyter-task
 Author: Flowminder Foundation
 Author-email: flowkit@flowminder.org
 Keywords: mobile telecommunications analysis
 Platform: MacOS X
 Platform: Linux
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: apache_airflow<3,>=2.8.1
+Requires-Dist: apache-airflow-providers-docker
+Requires-Dist: psycopg2-binary
 Provides-Extra: dev
+Requires-Dist: versioneer; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: approvaltests; extra == "test"
+Requires-Dist: pytest-docker; extra == "test"
+Requires-Dist: flowkit_jwt_generator; extra == "test"
 
 # flowpyter-task
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/Flowminder/flowpyter-task/tree/main.svg?style=shield&circle-token=644326d702a0d2ab491c7309515bf8560e370fed)](https://dl.circleci.com/status-badge/redirect/gh/Flowminder/flowpyter-task/tree/main)  [![License: MPL 2.0](https://img.shields.io/github/license/Flowminder/flowpyter-task.svg?style=flat-square)](https://opensource.org/licenses/MPL-2.0) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/python/black)
 
 A minirepo for holding the flowpyter Docker operator for airflow DAGs
```

### Comparing `flowpyter-task-1.1.4/README.md` & `flowpyter-task-1.1.4.post0.dev12/README.md`

 * *Files identical despite different names*

### Comparing `flowpyter-task-1.1.4/setup.py` & `flowpyter-task-1.1.4.post0.dev12/setup.py`

 * *Files identical despite different names*

### Comparing `flowpyter-task-1.1.4/src/flowpyter_task.egg-info/PKG-INFO` & `flowpyter-task-1.1.4.post0.dev12/src/flowpyter_task.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 Metadata-Version: 2.1
 Name: flowpyter-task
-Version: 1.1.4
+Version: 1.1.4.post0.dev12
 Home-page: https://github.com/Flowminder/flowpyter-task
 Author: Flowminder Foundation
 Author-email: flowkit@flowminder.org
 Keywords: mobile telecommunications analysis
 Platform: MacOS X
 Platform: Linux
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: apache_airflow<3,>=2.8.1
+Requires-Dist: apache-airflow-providers-docker
+Requires-Dist: psycopg2-binary
 Provides-Extra: dev
+Requires-Dist: versioneer; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: approvaltests; extra == "test"
+Requires-Dist: pytest-docker; extra == "test"
+Requires-Dist: flowkit_jwt_generator; extra == "test"
 
 # flowpyter-task
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/Flowminder/flowpyter-task/tree/main.svg?style=shield&circle-token=644326d702a0d2ab491c7309515bf8560e370fed)](https://dl.circleci.com/status-badge/redirect/gh/Flowminder/flowpyter-task/tree/main)  [![License: MPL 2.0](https://img.shields.io/github/license/Flowminder/flowpyter-task.svg?style=flat-square)](https://opensource.org/licenses/MPL-2.0) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/python/black)
 
 A minirepo for holding the flowpyter Docker operator for airflow DAGs
```

### Comparing `flowpyter-task-1.1.4/src/flowpyter_task.egg-info/SOURCES.txt` & `flowpyter-task-1.1.4.post0.dev12/src/flowpyter_task.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flowpyter-task-1.1.4/src/flowpytertask/flowpytertask.py` & `flowpyter-task-1.1.4.post0.dev12/src/flowpytertask/flowpytertask.py`

 * *Files identical despite different names*

### Comparing `flowpyter-task-1.1.4/tests/test_flowpyter_operator.py` & `flowpyter-task-1.1.4.post0.dev12/tests/test_flowpyter_operator.py`

 * *Files identical despite different names*

### Comparing `flowpyter-task-1.1.4/tests/test_integration.py` & `flowpyter-task-1.1.4.post0.dev12/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `flowpyter-task-1.1.4/versioneer.py` & `flowpyter-task-1.1.4.post0.dev12/versioneer.py`

 * *Files identical despite different names*

