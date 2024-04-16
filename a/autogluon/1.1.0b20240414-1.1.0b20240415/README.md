# Comparing `tmp/autogluon-1.1.0b20240414.tar.gz` & `tmp/autogluon-1.1.0b20240415.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-1.1.0b20240414.tar", last modified: Sun Apr 14 10:22:50 2024, max compression
+gzip compressed data, was "autogluon-1.1.0b20240415.tar", last modified: Mon Apr 15 09:05:13 2024, max compression
```

## Comparing `autogluon-1.1.0b20240414.tar` & `autogluon-1.1.0b20240415.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:50.024730 autogluon-1.1.0b20240414/
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-14 10:22:50.024730 autogluon-1.1.0b20240414/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 10:22:50.024730 autogluon-1.1.0b20240414/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-14 10:21:20.000000 autogluon-1.1.0b20240414/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:50.024730 autogluon-1.1.0b20240414/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:50.024730 autogluon-1.1.0b20240414/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:50.024730 autogluon-1.1.0b20240414/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 10:21:20.000000 autogluon-1.1.0b20240414/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:50.024730 autogluon-1.1.0b20240414/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-14 10:22:49.000000 autogluon-1.1.0b20240414/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-14 10:22:50.000000 autogluon-1.1.0b20240414/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 10:22:49.000000 autogluon-1.1.0b20240414/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 10:22:49.000000 autogluon-1.1.0b20240414/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-14 10:22:49.000000 autogluon-1.1.0b20240414/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 10:22:49.000000 autogluon-1.1.0b20240414/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 10:22:49.000000 autogluon-1.1.0b20240414/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:13.132753 autogluon-1.1.0b20240415/
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-15 09:05:13.132753 autogluon-1.1.0b20240415/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 09:05:13.132753 autogluon-1.1.0b20240415/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-15 09:03:37.000000 autogluon-1.1.0b20240415/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:13.132753 autogluon-1.1.0b20240415/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:13.132753 autogluon-1.1.0b20240415/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:13.132753 autogluon-1.1.0b20240415/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 09:03:37.000000 autogluon-1.1.0b20240415/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:05:13.132753 autogluon-1.1.0b20240415/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-15 09:05:13.000000 autogluon-1.1.0b20240415/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-15 09:05:13.000000 autogluon-1.1.0b20240415/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:05:13.000000 autogluon-1.1.0b20240415/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 09:05:13.000000 autogluon-1.1.0b20240415/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-15 09:05:13.000000 autogluon-1.1.0b20240415/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 09:05:13.000000 autogluon-1.1.0b20240415/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:05:13.000000 autogluon-1.1.0b20240415/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-1.1.0b20240414/PKG-INFO` & `autogluon-1.1.0b20240415/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.1.0b20240414
+Version: 1.1.0b20240415
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-1.1.0b20240414/setup.py` & `autogluon-1.1.0b20240415/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-1.1.0b20240414/src/autogluon.egg-info/PKG-INFO` & `autogluon-1.1.0b20240415/src/autogluon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.1.0b20240414
+Version: 1.1.0b20240415
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```
