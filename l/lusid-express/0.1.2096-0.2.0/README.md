# Comparing `tmp/lusid_express-0.1.2096.tar.gz` & `tmp/lusid_express-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_express-0.1.2096.tar", last modified: Tue Apr 16 19:54:24 2024, max compression
+gzip compressed data, was "lusid_express-0.2.0.tar", last modified: Tue Apr 16 20:16:36 2024, max compression
```

## Comparing `lusid_express-0.1.2096.tar` & `lusid_express-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 19:54:24.099243 lusid_express-0.1.2096/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-16 19:54:21.000000 lusid_express-0.1.2096/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-04-16 19:54:21.000000 lusid_express-0.1.2096/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6551 2024-04-16 19:54:24.099243 lusid_express-0.1.2096/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5908 2024-04-16 19:54:21.000000 lusid_express-0.1.2096/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 19:54:24.099243 lusid_express-0.1.2096/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1602 2024-04-16 19:54:21.000000 lusid_express-0.1.2096/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 19:54:24.095244 lusid_express-0.1.2096/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 19:54:24.097243 lusid_express-0.1.2096/src/lusid_express/
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-16 19:54:21.000000 lusid_express-0.1.2096/src/lusid_express/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1909 2024-04-16 19:54:21.000000 lusid_express-0.1.2096/src/lusid_express/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 19:54:24.098243 lusid_express-0.1.2096/src/lusid_express/apis/
--rw-rw-rw-   0 root         (0) root         (0)     1414 2024-04-16 19:54:21.000000 lusid_express-0.1.2096/src/lusid_express/apis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 19:54:24.098243 lusid_express-0.1.2096/src/lusid_express/config/
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-16 19:54:21.000000 lusid_express-0.1.2096/src/lusid_express/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 19:54:24.099243 lusid_express-0.1.2096/src/lusid_express/markdown/
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-16 19:54:21.000000 lusid_express-0.1.2096/src/lusid_express/markdown/PRELOADED_VARS.md
--rw-rw-rw-   0 root         (0) root         (0)      298 2024-04-16 19:54:21.000000 lusid_express-0.1.2096/src/lusid_express/markdown/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 19:54:24.098243 lusid_express-0.1.2096/src/lusid_express.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6551 2024-04-16 19:54:24.000000 lusid_express-0.1.2096/src/lusid_express.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      458 2024-04-16 19:54:24.000000 lusid_express-0.1.2096/src/lusid_express.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 19:54:24.000000 lusid_express-0.1.2096/src/lusid_express.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      483 2024-04-16 19:54:24.000000 lusid_express-0.1.2096/src/lusid_express.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-16 19:54:24.000000 lusid_express-0.1.2096/src/lusid_express.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:16:36.634504 lusid_express-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-16 20:16:34.000000 lusid_express-0.2.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-04-16 20:16:34.000000 lusid_express-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6548 2024-04-16 20:16:36.634504 lusid_express-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5908 2024-04-16 20:16:34.000000 lusid_express-0.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 20:16:36.634504 lusid_express-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2024-04-16 20:16:34.000000 lusid_express-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:16:36.631504 lusid_express-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:16:36.632504 lusid_express-0.2.0/src/lusid_express/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-16 20:16:34.000000 lusid_express-0.2.0/src/lusid_express/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1909 2024-04-16 20:16:34.000000 lusid_express-0.2.0/src/lusid_express/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:16:36.633504 lusid_express-0.2.0/src/lusid_express/apis/
+-rw-rw-rw-   0 root         (0) root         (0)     1414 2024-04-16 20:16:34.000000 lusid_express-0.2.0/src/lusid_express/apis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:16:36.633504 lusid_express-0.2.0/src/lusid_express/config/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-16 20:16:34.000000 lusid_express-0.2.0/src/lusid_express/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:16:36.634504 lusid_express-0.2.0/src/lusid_express/markdown/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-16 20:16:34.000000 lusid_express-0.2.0/src/lusid_express/markdown/PRELOADED_VARS.md
+-rw-rw-rw-   0 root         (0) root         (0)      298 2024-04-16 20:16:34.000000 lusid_express-0.2.0/src/lusid_express/markdown/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:16:36.633504 lusid_express-0.2.0/src/lusid_express.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6548 2024-04-16 20:16:36.000000 lusid_express-0.2.0/src/lusid_express.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      458 2024-04-16 20:16:36.000000 lusid_express-0.2.0/src/lusid_express.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:16:36.000000 lusid_express-0.2.0/src/lusid_express.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      468 2024-04-16 20:16:36.000000 lusid_express-0.2.0/src/lusid_express.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-16 20:16:36.000000 lusid_express-0.2.0/src/lusid_express.egg-info/top_level.txt
```

### Comparing `lusid_express-0.1.2096/LICENSE` & `lusid_express-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lusid_express-0.1.2096/PKG-INFO` & `lusid_express-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid_express
-Version: 0.1.2096
+Version: 0.2.0
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_express-0.1.2096/README.md` & `lusid_express-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lusid_express-0.1.2096/setup.py` & `lusid_express-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,30 +8,30 @@
     'lusid-jam==0.1.2',
     'lusid-sdk-preview==1.1.120',
     'fbnlab-preview==0.1.108',
     'finbourne-access-sdk==0.0.3751',
     'finbourne-identity-sdk==0.0.2834',
     'finbourne-insights-sdk-preview==0.0.763',
     'finbourne-sdk-utilities==0.0.10',
-    'lusid-configuration-sdk-preview==0.1.2096',
-    'lusid-drive-sdk-preview==0.1.2096',
-    'lusid-notifications-sdk-preview==0.1.2096',
+    'lusid-configuration-sdk-preview==0.2.0',
+    'lusid-drive-sdk-preview==0.2.0',
+    'lusid-notifications-sdk-preview==0.2.0',
     'lusid-scheduler-sdk-preview==0.0.829',
-    'lusid-workflow-sdk-preview==0.1.2096',
+    'lusid-workflow-sdk-preview==0.2.0',
     'lusidtools==1.0.14',
-    'dve-lumipy-preview==0.1.2096'
+    'dve-lumipy-preview==0.2.0'
 
 ]
 
 
 
 
 setup(
     name='lusid_express',
-    version='0.1.2096',
+    version='0.2.0',
     package_dir={'': 'src'},  # tells setuptools that packages are under src
     packages=find_packages(where='src'),  # tells setuptools to look for packages in src
     install_requires=requirements,
     description='lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.',
     long_description=open('README.md').read(),
     include_package_data=True,  
     long_description_content_type='text/markdown',
```

### Comparing `lusid_express-0.1.2096/src/lusid_express/__main__.py` & `lusid_express-0.2.0/src/lusid_express/__main__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-0.1.2096/src/lusid_express/apis/__init__.py` & `lusid_express-0.2.0/src/lusid_express/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-0.1.2096/src/lusid_express/markdown/PRELOADED_VARS.md` & `lusid_express-0.2.0/src/lusid_express/markdown/PRELOADED_VARS.md`

 * *Files identical despite different names*

### Comparing `lusid_express-0.1.2096/src/lusid_express.egg-info/PKG-INFO` & `lusid_express-0.2.0/src/lusid_express.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-express
-Version: 0.1.2096
+Version: 0.2.0
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```
