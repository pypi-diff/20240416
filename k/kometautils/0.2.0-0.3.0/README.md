# Comparing `tmp/kometautils-0.2.0.tar.gz` & `tmp/kometautils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kometautils-0.2.0.tar", last modified: Tue Apr 16 18:48:44 2024, max compression
+gzip compressed data, was "kometautils-0.3.0.tar", last modified: Tue Apr 16 18:50:41 2024, max compression
```

## Comparing `kometautils-0.2.0.tar` & `kometautils-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:48:44.003018 kometautils-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 18:48:31.000000 kometautils-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-16 18:48:44.003018 kometautils-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-16 18:48:31.000000 kometautils-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:48:44.003018 kometautils-0.2.0/kometautils/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-16 18:48:31.000000 kometautils-0.2.0/kometautils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-04-16 18:48:31.000000 kometautils-0.2.0/kometautils/args.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-16 18:48:31.000000 kometautils-0.2.0/kometautils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    22117 2024-04-16 18:48:31.000000 kometautils-0.2.0/kometautils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    31561 2024-04-16 18:48:31.000000 kometautils-0.2.0/kometautils/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-16 18:48:31.000000 kometautils-0.2.0/kometautils/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-16 18:48:31.000000 kometautils-0.2.0/kometautils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:48:44.003018 kometautils-0.2.0/kometautils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-16 18:48:43.000000 kometautils-0.2.0/kometautils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-16 18:48:43.000000 kometautils-0.2.0/kometautils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 18:48:43.000000 kometautils-0.2.0/kometautils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-16 18:48:43.000000 kometautils-0.2.0/kometautils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 18:48:43.000000 kometautils-0.2.0/kometautils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 18:48:44.003018 kometautils-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-16 18:48:31.000000 kometautils-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:50:41.468080 kometautils-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 18:50:26.000000 kometautils-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-16 18:50:41.468080 kometautils-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-16 18:50:26.000000 kometautils-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:50:41.464080 kometautils-0.3.0/kometautils/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-16 18:50:26.000000 kometautils-0.3.0/kometautils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-04-16 18:50:26.000000 kometautils-0.3.0/kometautils/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-16 18:50:26.000000 kometautils-0.3.0/kometautils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22117 2024-04-16 18:50:26.000000 kometautils-0.3.0/kometautils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31561 2024-04-16 18:50:26.000000 kometautils-0.3.0/kometautils/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-16 18:50:26.000000 kometautils-0.3.0/kometautils/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-16 18:50:26.000000 kometautils-0.3.0/kometautils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:50:41.468080 kometautils-0.3.0/kometautils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-16 18:50:41.000000 kometautils-0.3.0/kometautils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-16 18:50:41.000000 kometautils-0.3.0/kometautils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 18:50:41.000000 kometautils-0.3.0/kometautils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-16 18:50:41.000000 kometautils-0.3.0/kometautils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 18:50:41.000000 kometautils-0.3.0/kometautils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 18:50:41.468080 kometautils-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-16 18:50:26.000000 kometautils-0.3.0/setup.py
```

### Comparing `kometautils-0.2.0/LICENSE` & `kometautils-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kometautils-0.2.0/PKG-INFO` & `kometautils-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kometautils
-Version: 0.2.0
+Version: 0.3.0
 Summary: Util Methods for Kometa
 Home-page: https://github.com/Kometa-Team/Kometa-Utils
 Author: Nathan Taggart
 Author-email: meisnate12@gmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/Kometa-Team/Kometa-Utils
 Project-URL: Funding, https://github.com/sponsors/meisnate12
```

### Comparing `kometautils-0.2.0/README.rst` & `kometautils-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `kometautils-0.2.0/kometautils/__init__.py` & `kometautils-0.3.0/kometautils/__init__.py`

 * *Files identical despite different names*

### Comparing `kometautils-0.2.0/kometautils/args.py` & `kometautils-0.3.0/kometautils/args.py`

 * *Files identical despite different names*

### Comparing `kometautils-0.2.0/kometautils/logging.py` & `kometautils-0.3.0/kometautils/logging.py`

 * *Files identical despite different names*

### Comparing `kometautils-0.2.0/kometautils/schedule.py` & `kometautils-0.3.0/kometautils/schedule.py`

 * *Files identical despite different names*

### Comparing `kometautils-0.2.0/kometautils/util.py` & `kometautils-0.3.0/kometautils/util.py`

 * *Files identical despite different names*

### Comparing `kometautils-0.2.0/kometautils/yaml.py` & `kometautils-0.3.0/kometautils/yaml.py`

 * *Files identical despite different names*

### Comparing `kometautils-0.2.0/kometautils.egg-info/PKG-INFO` & `kometautils-0.3.0/kometautils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kometautils
-Version: 0.2.0
+Version: 0.3.0
 Summary: Util Methods for Kometa
 Home-page: https://github.com/Kometa-Team/Kometa-Utils
 Author: Nathan Taggart
 Author-email: meisnate12@gmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/Kometa-Team/Kometa-Utils
 Project-URL: Funding, https://github.com/sponsors/meisnate12
```

### Comparing `kometautils-0.2.0/setup.py` & `kometautils-0.3.0/setup.py`

 * *Files identical despite different names*

