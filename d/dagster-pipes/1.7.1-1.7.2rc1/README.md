# Comparing `tmp/dagster-pipes-1.7.1.tar.gz` & `tmp/dagster-pipes-1.7.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-pipes-1.7.1.tar", last modified: Thu Apr 11 18:05:11 2024, max compression
+gzip compressed data, was "dagster-pipes-1.7.2rc1.tar", last modified: Tue Apr 16 17:51:22 2024, max compression
```

## Comparing `dagster-pipes-1.7.1.tar` & `dagster-pipes-1.7.2rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:05:11.546383 dagster-pipes-1.7.1/
--rw-r--r--   0 root         (0) root         (0)    11348 2024-04-11 18:04:19.000000 dagster-pipes-1.7.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-11 18:04:19.000000 dagster-pipes-1.7.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      794 2024-04-11 18:05:11.546383 dagster-pipes-1.7.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      125 2024-04-11 18:04:19.000000 dagster-pipes-1.7.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:05:11.546383 dagster-pipes-1.7.1/dagster_pipes/
--rw-r--r--   0 root         (0) root         (0)    48163 2024-04-11 18:04:19.000000 dagster-pipes-1.7.1/dagster_pipes/__init__.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-11 18:04:19.000000 dagster-pipes-1.7.1/dagster_pipes/py.typed
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-11 18:04:19.000000 dagster-pipes-1.7.1/dagster_pipes/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:05:11.546383 dagster-pipes-1.7.1/dagster_pipes.egg-info/
--rw-r--r--   0 root         (0) root         (0)      794 2024-04-11 18:05:11.000000 dagster-pipes-1.7.1/dagster_pipes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      306 2024-04-11 18:05:11.000000 dagster-pipes-1.7.1/dagster_pipes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:05:11.000000 dagster-pipes-1.7.1/dagster_pipes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:05:11.000000 dagster-pipes-1.7.1/dagster_pipes.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-11 18:05:11.000000 dagster-pipes-1.7.1/dagster_pipes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      160 2024-04-11 18:05:11.550383 dagster-pipes-1.7.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1313 2024-04-11 18:04:19.000000 dagster-pipes-1.7.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:22.183205 dagster-pipes-1.7.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    11348 2024-04-16 17:50:34.000000 dagster-pipes-1.7.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-16 17:50:34.000000 dagster-pipes-1.7.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      797 2024-04-16 17:51:22.183205 dagster-pipes-1.7.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      125 2024-04-16 17:50:34.000000 dagster-pipes-1.7.2rc1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:22.183205 dagster-pipes-1.7.2rc1/dagster_pipes/
+-rw-r--r--   0 root         (0) root         (0)    48163 2024-04-16 17:50:34.000000 dagster-pipes-1.7.2rc1/dagster_pipes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-16 17:50:34.000000 dagster-pipes-1.7.2rc1/dagster_pipes/py.typed
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-16 17:50:34.000000 dagster-pipes-1.7.2rc1/dagster_pipes/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:22.183205 dagster-pipes-1.7.2rc1/dagster_pipes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      797 2024-04-16 17:51:22.000000 dagster-pipes-1.7.2rc1/dagster_pipes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      306 2024-04-16 17:51:22.000000 dagster-pipes-1.7.2rc1/dagster_pipes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:51:22.000000 dagster-pipes-1.7.2rc1/dagster_pipes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:51:22.000000 dagster-pipes-1.7.2rc1/dagster_pipes.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-16 17:51:22.000000 dagster-pipes-1.7.2rc1/dagster_pipes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      160 2024-04-16 17:51:22.187205 dagster-pipes-1.7.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1313 2024-04-16 17:50:34.000000 dagster-pipes-1.7.2rc1/setup.py
```

### Comparing `dagster-pipes-1.7.1/LICENSE` & `dagster-pipes-1.7.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-pipes-1.7.1/PKG-INFO` & `dagster-pipes-1.7.2rc1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-pipes
-Version: 1.7.1
+Version: 1.7.2rc1
 Summary: Toolkit for Dagster integrations with transform logic outside of Dagster
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-pipes
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-pipes-1.7.1/dagster_pipes/__init__.py` & `dagster-pipes-1.7.2rc1/dagster_pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-pipes-1.7.1/dagster_pipes.egg-info/PKG-INFO` & `dagster-pipes-1.7.2rc1/dagster_pipes.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-pipes
-Version: 1.7.1
+Version: 1.7.2rc1
 Summary: Toolkit for Dagster integrations with transform logic outside of Dagster
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-pipes
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-pipes-1.7.1/setup.py` & `dagster-pipes-1.7.2rc1/setup.py`

 * *Files identical despite different names*

