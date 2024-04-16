# Comparing `tmp/alida-apis-0.0.1.tar.gz` & `tmp/alida-apis-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alida-apis-0.0.1.tar", last modified: Tue Apr 16 16:00:55 2024, max compression
+gzip compressed data, was "dist/alida-apis-0.0.2.tar", last modified: Tue Apr 16 16:15:27 2024, max compression
```

## Comparing `alida-apis-0.0.1.tar` & `alida-apis-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:00:55.934038 alida-apis-0.0.1/
--rw-r--r--   0 root         (0) root         (0)      422 2024-04-16 16:00:55.934038 alida-apis-0.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-04-16 16:00:44.000000 alida-apis-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:00:55.934038 alida-apis-0.0.1/alida_apis.egg-info/
--rw-r--r--   0 root         (0) root         (0)      422 2024-04-16 16:00:55.000000 alida-apis-0.0.1/alida_apis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      281 2024-04-16 16:00:55.000000 alida-apis-0.0.1/alida_apis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 16:00:55.000000 alida-apis-0.0.1/alida_apis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-16 16:00:55.000000 alida-apis-0.0.1/alida_apis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-16 16:00:55.000000 alida-apis-0.0.1/alida_apis.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:00:55.934038 alida-apis-0.0.1/alidaapis/
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-04-16 16:00:44.000000 alida-apis-0.0.1/alidaapis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10346 2024-04-16 16:00:44.000000 alida-apis-0.0.1/alidaapis/apis.py
--rw-rw-rw-   0 root         (0) root         (0)     4951 2024-04-16 16:00:44.000000 alida-apis-0.0.1/alidaapis/minio_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      351 2024-04-16 16:00:44.000000 alida-apis-0.0.1/alidaapis/utils.py
--rw-rw-rw-   0 root         (0) root         (0)       79 2024-04-16 16:00:55.934038 alida-apis-0.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      597 2024-04-16 16:00:44.000000 alida-apis-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:15:27.837683 alida-apis-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)      422 2024-04-16 16:15:27.837683 alida-apis-0.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-04-16 16:15:17.000000 alida-apis-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:15:27.836683 alida-apis-0.0.2/alida_apis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      422 2024-04-16 16:15:27.000000 alida-apis-0.0.2/alida_apis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      281 2024-04-16 16:15:27.000000 alida-apis-0.0.2/alida_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 16:15:27.000000 alida-apis-0.0.2/alida_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-16 16:15:27.000000 alida-apis-0.0.2/alida_apis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-16 16:15:27.000000 alida-apis-0.0.2/alida_apis.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:15:27.837683 alida-apis-0.0.2/alidaapis/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-16 16:15:17.000000 alida-apis-0.0.2/alidaapis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10346 2024-04-16 16:15:17.000000 alida-apis-0.0.2/alidaapis/apis.py
+-rw-rw-rw-   0 root         (0) root         (0)     4951 2024-04-16 16:15:17.000000 alida-apis-0.0.2/alidaapis/minio_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      351 2024-04-16 16:15:17.000000 alida-apis-0.0.2/alidaapis/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       79 2024-04-16 16:15:27.837683 alida-apis-0.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      597 2024-04-16 16:15:17.000000 alida-apis-0.0.2/setup.py
```

### Comparing `alida-apis-0.0.1/alidaapis/apis.py` & `alida-apis-0.0.2/alidaapis/apis.py`

 * *Files identical despite different names*

### Comparing `alida-apis-0.0.1/alidaapis/minio_utils.py` & `alida-apis-0.0.2/alidaapis/minio_utils.py`

 * *Files identical despite different names*

### Comparing `alida-apis-0.0.1/setup.py` & `alida-apis-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="alida-apis",
-    version="0.0.1",
+    version="0.0.2",
     author="Alida research team",
     author_email="salvatore.cipolla@eng.it",
     description="Python APIs for interaction with ALIDA backend.",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

