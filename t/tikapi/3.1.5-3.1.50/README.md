# Comparing `tmp/tikapi-3.1.5.tar.gz` & `tmp/tikapi-3.1.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tikapi-3.1.5.tar", last modified: Tue Oct 17 18:24:38 2023, max compression
+gzip compressed data, was "tikapi-3.1.50.tar", last modified: Tue Apr 16 17:01:41 2024, max compression
```

## Comparing `tikapi-3.1.5.tar` & `tikapi-3.1.50.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-10-17 18:24:38.792561 tikapi-3.1.5/
--rw-rw-rw-   0        0        0       67 2022-12-07 21:27:40.000000 tikapi-3.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1860 2023-10-17 18:24:38.792561 tikapi-3.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1106 2022-08-29 11:23:45.000000 tikapi-3.1.5/README.md
--rw-rw-rw-   0        0        0      121 2023-10-17 18:24:38.793561 tikapi-3.1.5/setup.cfg
--rw-rw-rw-   0        0        0      703 2023-10-17 18:24:05.000000 tikapi-3.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-17 18:24:38.787561 tikapi-3.1.5/tikapi/
--rw-rw-rw-   0        0        0     3228 2023-09-22 16:50:46.000000 tikapi-3.1.5/tikapi/__init__.py
--rw-rw-rw-   0        0        0    89849 2023-10-17 18:24:12.000000 tikapi-3.1.5/tikapi/api.py
-drwxrwxrwx   0        0        0        0 2023-10-17 18:24:38.791562 tikapi-3.1.5/tikapi.egg-info/
--rw-rw-rw-   0        0        0     1860 2023-10-17 18:24:38.000000 tikapi-3.1.5/tikapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-10-17 18:24:38.000000 tikapi-3.1.5/tikapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-17 18:24:38.000000 tikapi-3.1.5/tikapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-07-07 14:30:05.000000 tikapi-3.1.5/tikapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-10-17 18:24:38.000000 tikapi-3.1.5/tikapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-10-17 18:24:38.000000 tikapi-3.1.5/tikapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 17:01:41.904266 tikapi-3.1.50/
+-rw-rw-rw-   0        0        0       67 2022-12-07 21:27:40.000000 tikapi-3.1.50/MANIFEST.in
+-rw-rw-rw-   0        0        0     1861 2024-04-16 17:01:41.904266 tikapi-3.1.50/PKG-INFO
+-rw-rw-rw-   0        0        0     1106 2022-08-29 11:23:45.000000 tikapi-3.1.50/README.md
+-rw-rw-rw-   0        0        0      121 2024-04-16 17:01:41.905266 tikapi-3.1.50/setup.cfg
+-rw-rw-rw-   0        0        0      704 2024-04-16 17:01:19.000000 tikapi-3.1.50/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 17:01:41.899266 tikapi-3.1.50/tikapi/
+-rw-rw-rw-   0        0        0     3228 2023-09-22 16:50:46.000000 tikapi-3.1.50/tikapi/__init__.py
+-rw-rw-rw-   0        0        0    89849 2023-10-17 18:24:12.000000 tikapi-3.1.50/tikapi/api.py
+drwxrwxrwx   0        0        0        0 2024-04-16 17:01:41.903266 tikapi-3.1.50/tikapi.egg-info/
+-rw-rw-rw-   0        0        0     1861 2024-04-16 17:01:41.000000 tikapi-3.1.50/tikapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-04-16 17:01:41.000000 tikapi-3.1.50/tikapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 17:01:41.000000 tikapi-3.1.50/tikapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-07-07 14:30:05.000000 tikapi-3.1.50/tikapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2024-04-16 17:01:41.000000 tikapi-3.1.50/tikapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-16 17:01:41.000000 tikapi-3.1.50/tikapi.egg-info/top_level.txt
```

### Comparing `tikapi-3.1.5/PKG-INFO` & `tikapi-3.1.50/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tikapi
-Version: 3.1.5
+Version: 3.1.50
 Summary: TikAPI | TikTok Unofficial API
 Home-page: https://www.tikapi.io
 Author: TikAPI
 Author-email: contact@tikapi.io
 License: TikAPI
 Description: # Unofficial TikTok API <img src='https://img.shields.io/npm/v/tikapi'> <img src='https://img.shields.io/pypi/v/tikapi'>
```

### Comparing `tikapi-3.1.5/README.md` & `tikapi-3.1.50/README.md`

 * *Files identical despite different names*

### Comparing `tikapi-3.1.5/setup.py` & `tikapi-3.1.50/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 INSTALL_REQUIRES = [
    'requests',
 ]
 
 setup(
     name='tikapi',
-    version='3.1.5',
+    version='3.1.50',
     description='TikAPI | TikTok Unofficial API',
     long_description_content_type="text/markdown",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     license='TikAPI',
     author='TikAPI',
     author_email='contact@tikapi.io',
     url='https://www.tikapi.io',
```

### Comparing `tikapi-3.1.5/tikapi/__init__.py` & `tikapi-3.1.50/tikapi/__init__.py`

 * *Files identical despite different names*

### Comparing `tikapi-3.1.5/tikapi/api.py` & `tikapi-3.1.50/tikapi/api.py`

 * *Files identical despite different names*

### Comparing `tikapi-3.1.5/tikapi.egg-info/PKG-INFO` & `tikapi-3.1.50/tikapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tikapi
-Version: 3.1.5
+Version: 3.1.50
 Summary: TikAPI | TikTok Unofficial API
 Home-page: https://www.tikapi.io
 Author: TikAPI
 Author-email: contact@tikapi.io
 License: TikAPI
 Description: # Unofficial TikTok API <img src='https://img.shields.io/npm/v/tikapi'> <img src='https://img.shields.io/pypi/v/tikapi'>
```

