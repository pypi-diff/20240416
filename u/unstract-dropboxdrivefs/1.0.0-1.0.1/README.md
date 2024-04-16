# Comparing `tmp/unstract-dropboxdrivefs-1.0.0.tar.gz` & `tmp/unstract-dropboxdrivefs-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstract-dropboxdrivefs-1.0.0.tar", last modified: Mon Oct 30 12:16:24 2023, max compression
+gzip compressed data, was "unstract-dropboxdrivefs-1.0.1.tar", last modified: Tue Apr 16 12:02:19 2024, max compression
```

## Comparing `unstract-dropboxdrivefs-1.0.0.tar` & `unstract-dropboxdrivefs-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 chandru   (1000) chandru   (1000)        0 2023-10-30 12:16:24.013081 unstract-dropboxdrivefs-1.0.0/
--rw-rw-r--   0 chandru   (1000) chandru   (1000)     1528 2023-10-30 11:58:36.000000 unstract-dropboxdrivefs-1.0.0/LICENSE
--rw-rw-r--   0 chandru   (1000) chandru   (1000)       35 2023-10-30 11:58:36.000000 unstract-dropboxdrivefs-1.0.0/MANIFEST.in
--rw-rw-r--   0 chandru   (1000) chandru   (1000)     2481 2023-10-30 12:16:24.013081 unstract-dropboxdrivefs-1.0.0/PKG-INFO
--rw-rw-r--   0 chandru   (1000) chandru   (1000)     1383 2023-10-30 11:58:36.000000 unstract-dropboxdrivefs-1.0.0/README.md
-drwxrwxr-x   0 chandru   (1000) chandru   (1000)        0 2023-10-30 12:16:24.013081 unstract-dropboxdrivefs-1.0.0/dropboxdrivefs/
--rw-rw-r--   0 chandru   (1000) chandru   (1000)       57 2023-10-30 11:58:36.000000 unstract-dropboxdrivefs-1.0.0/dropboxdrivefs/__init__.py
--rw-rw-r--   0 chandru   (1000) chandru   (1000)     6898 2023-10-30 11:58:36.000000 unstract-dropboxdrivefs-1.0.0/dropboxdrivefs/core.py
--rw-rw-r--   0 chandru   (1000) chandru   (1000)       38 2023-10-30 12:16:24.013081 unstract-dropboxdrivefs-1.0.0/setup.cfg
--rw-rw-r--   0 chandru   (1000) chandru   (1000)     1156 2023-10-30 12:05:30.000000 unstract-dropboxdrivefs-1.0.0/setup.py
-drwxrwxr-x   0 chandru   (1000) chandru   (1000)        0 2023-10-30 12:16:24.013081 unstract-dropboxdrivefs-1.0.0/test/
--rw-rw-r--   0 chandru   (1000) chandru   (1000)     3053 2023-10-30 11:58:36.000000 unstract-dropboxdrivefs-1.0.0/test/test.py
-drwxrwxr-x   0 chandru   (1000) chandru   (1000)        0 2023-10-30 12:16:24.013081 unstract-dropboxdrivefs-1.0.0/unstract_dropboxdrivefs.egg-info/
--rw-rw-r--   0 chandru   (1000) chandru   (1000)     2481 2023-10-30 12:16:23.000000 unstract-dropboxdrivefs-1.0.0/unstract_dropboxdrivefs.egg-info/PKG-INFO
--rw-rw-r--   0 chandru   (1000) chandru   (1000)      381 2023-10-30 12:16:24.000000 unstract-dropboxdrivefs-1.0.0/unstract_dropboxdrivefs.egg-info/SOURCES.txt
--rw-rw-r--   0 chandru   (1000) chandru   (1000)        1 2023-10-30 12:16:23.000000 unstract-dropboxdrivefs-1.0.0/unstract_dropboxdrivefs.egg-info/dependency_links.txt
--rw-rw-r--   0 chandru   (1000) chandru   (1000)        1 2023-10-30 12:16:23.000000 unstract-dropboxdrivefs-1.0.0/unstract_dropboxdrivefs.egg-info/not-zip-safe
--rw-rw-r--   0 chandru   (1000) chandru   (1000)       24 2023-10-30 12:16:23.000000 unstract-dropboxdrivefs-1.0.0/unstract_dropboxdrivefs.egg-info/requires.txt
--rw-rw-r--   0 chandru   (1000) chandru   (1000)       15 2023-10-30 12:16:23.000000 unstract-dropboxdrivefs-1.0.0/unstract_dropboxdrivefs.egg-info/top_level.txt
+drwxrwxr-x   0 chandru   (1000) chandru   (1000)        0 2024-04-16 12:02:19.016196 unstract-dropboxdrivefs-1.0.1/
+-rw-rw-r--   0 chandru   (1000) chandru   (1000)     1528 2023-10-30 11:58:36.000000 unstract-dropboxdrivefs-1.0.1/LICENSE
+-rw-rw-r--   0 chandru   (1000) chandru   (1000)       35 2023-10-30 11:58:36.000000 unstract-dropboxdrivefs-1.0.1/MANIFEST.in
+-rw-rw-r--   0 chandru   (1000) chandru   (1000)     1268 2024-04-16 12:02:19.016196 unstract-dropboxdrivefs-1.0.1/PKG-INFO
+-rw-rw-r--   0 chandru   (1000) chandru   (1000)      426 2024-04-16 12:01:09.000000 unstract-dropboxdrivefs-1.0.1/README.md
+drwxrwxr-x   0 chandru   (1000) chandru   (1000)        0 2024-04-16 12:02:19.008196 unstract-dropboxdrivefs-1.0.1/dropboxdrivefs/
+-rw-rw-r--   0 chandru   (1000) chandru   (1000)       57 2023-10-30 11:58:36.000000 unstract-dropboxdrivefs-1.0.1/dropboxdrivefs/__init__.py
+-rw-rw-r--   0 chandru   (1000) chandru   (1000)     6898 2023-10-30 11:58:36.000000 unstract-dropboxdrivefs-1.0.1/dropboxdrivefs/core.py
+-rw-rw-r--   0 chandru   (1000) chandru   (1000)       38 2024-04-16 12:02:19.016196 unstract-dropboxdrivefs-1.0.1/setup.cfg
+-rw-rw-r--   0 chandru   (1000) chandru   (1000)     1156 2024-04-16 12:01:09.000000 unstract-dropboxdrivefs-1.0.1/setup.py
+drwxrwxr-x   0 chandru   (1000) chandru   (1000)        0 2024-04-16 12:02:19.008196 unstract-dropboxdrivefs-1.0.1/test/
+-rw-rw-r--   0 chandru   (1000) chandru   (1000)     3053 2023-10-30 11:58:36.000000 unstract-dropboxdrivefs-1.0.1/test/test.py
+drwxrwxr-x   0 chandru   (1000) chandru   (1000)        0 2024-04-16 12:02:19.012196 unstract-dropboxdrivefs-1.0.1/unstract_dropboxdrivefs.egg-info/
+-rw-rw-r--   0 chandru   (1000) chandru   (1000)     1268 2024-04-16 12:02:18.000000 unstract-dropboxdrivefs-1.0.1/unstract_dropboxdrivefs.egg-info/PKG-INFO
+-rw-rw-r--   0 chandru   (1000) chandru   (1000)      381 2024-04-16 12:02:18.000000 unstract-dropboxdrivefs-1.0.1/unstract_dropboxdrivefs.egg-info/SOURCES.txt
+-rw-rw-r--   0 chandru   (1000) chandru   (1000)        1 2024-04-16 12:02:18.000000 unstract-dropboxdrivefs-1.0.1/unstract_dropboxdrivefs.egg-info/dependency_links.txt
+-rw-rw-r--   0 chandru   (1000) chandru   (1000)        1 2023-10-30 12:16:23.000000 unstract-dropboxdrivefs-1.0.1/unstract_dropboxdrivefs.egg-info/not-zip-safe
+-rw-rw-r--   0 chandru   (1000) chandru   (1000)       24 2024-04-16 12:02:18.000000 unstract-dropboxdrivefs-1.0.1/unstract_dropboxdrivefs.egg-info/requires.txt
+-rw-rw-r--   0 chandru   (1000) chandru   (1000)       15 2024-04-16 12:02:18.000000 unstract-dropboxdrivefs-1.0.1/unstract_dropboxdrivefs.egg-info/top_level.txt
```

### Comparing `unstract-dropboxdrivefs-1.0.0/LICENSE` & `unstract-dropboxdrivefs-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unstract-dropboxdrivefs-1.0.0/dropboxdrivefs/core.py` & `unstract-dropboxdrivefs-1.0.1/dropboxdrivefs/core.py`

 * *Files identical despite different names*

### Comparing `unstract-dropboxdrivefs-1.0.0/setup.py` & `unstract-dropboxdrivefs-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="unstract-dropboxdrivefs",
-    version="1.0.0",
+    version="1.0.1",
     packages=["dropboxdrivefs"],
     install_requires=["fsspec", "requests", "dropbox"],
     author="Zipstack Inc",
     author_email="devsupport@zipstack.com",
     url = "https://github.com/Zipstack/dropboxdrivefs/",
     description="Dropbox implementation by Unstract for fsspec module",
     long_description=long_description,
```

### Comparing `unstract-dropboxdrivefs-1.0.0/test/test.py` & `unstract-dropboxdrivefs-1.0.1/test/test.py`

 * *Files identical despite different names*

