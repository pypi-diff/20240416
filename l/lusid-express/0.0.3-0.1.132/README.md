# Comparing `tmp/lusid_express-0.0.3.tar.gz` & `tmp/lusid_express-0.1.132.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_express-0.0.3.tar", last modified: Mon Apr 15 22:36:04 2024, max compression
+gzip compressed data, was "lusid_express-0.1.132.tar", last modified: Tue Apr 16 18:08:27 2024, max compression
```

## Comparing `lusid_express-0.0.3.tar` & `lusid_express-0.1.132.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxr-xr-x   0 orlandogcalvo   (501) staff       (20)        0 2024-04-15 22:36:04.852590 lusid_express-0.0.3/
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)     1062 2024-04-15 21:42:24.000000 lusid_express-0.0.3/LICENSE
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)     7230 2024-04-15 22:36:04.852136 lusid_express-0.0.3/PKG-INFO
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)     5908 2024-04-15 20:56:02.000000 lusid_express-0.0.3/README.md
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)       38 2024-04-15 22:36:04.852658 lusid_express-0.0.3/setup.cfg
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)     1594 2024-04-15 22:36:02.000000 lusid_express-0.0.3/setup.py
-drwxr-xr-x   0 orlandogcalvo   (501) staff       (20)        0 2024-04-15 22:36:04.826169 lusid_express-0.0.3/src/
-drwxr-xr-x   0 orlandogcalvo   (501) staff       (20)        0 2024-04-15 22:36:04.833084 lusid_express-0.0.3/src/lusid_express/
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)       30 2024-04-15 19:22:44.000000 lusid_express-0.0.3/src/lusid_express/__init__.py
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)     1909 2024-04-15 21:50:26.000000 lusid_express-0.0.3/src/lusid_express/__main__.py
-drwxr-xr-x   0 orlandogcalvo   (501) staff       (20)        0 2024-04-15 22:36:04.840716 lusid_express-0.0.3/src/lusid_express/apis/
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)     1414 2024-04-15 18:47:54.000000 lusid_express-0.0.3/src/lusid_express/apis/__init__.py
-drwxr-xr-x   0 orlandogcalvo   (501) staff       (20)        0 2024-04-15 22:36:04.842569 lusid_express-0.0.3/src/lusid_express/config/
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)      369 2024-04-15 19:34:41.000000 lusid_express-0.0.3/src/lusid_express/config/__init__.py
-drwxr-xr-x   0 orlandogcalvo   (501) staff       (20)        0 2024-04-15 22:36:04.844119 lusid_express-0.0.3/src/lusid_express/markdown/
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)      298 2024-04-15 20:28:24.000000 lusid_express-0.0.3/src/lusid_express/markdown/__init__.py
-drwxr-xr-x   0 orlandogcalvo   (501) staff       (20)        0 2024-04-15 22:36:04.851658 lusid_express-0.0.3/src/lusid_express.egg-info/
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)     7230 2024-04-15 22:36:04.000000 lusid_express-0.0.3/src/lusid_express.egg-info/PKG-INFO
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)      458 2024-04-15 22:36:04.000000 lusid_express-0.0.3/src/lusid_express.egg-info/SOURCES.txt
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)        1 2024-04-15 22:36:04.000000 lusid_express-0.0.3/src/lusid_express.egg-info/dependency_links.txt
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)      479 2024-04-15 22:36:04.000000 lusid_express-0.0.3/src/lusid_express.egg-info/requires.txt
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)       14 2024-04-15 22:36:04.000000 lusid_express-0.0.3/src/lusid_express.egg-info/top_level.txt
-drwxr-xr-x   0 orlandogcalvo   (501) staff       (20)        0 2024-04-15 22:36:04.851268 lusid_express-0.0.3/tests/
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)     1460 2024-04-15 22:05:27.000000 lusid_express-0.0.3/tests/test_cli.py
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)      532 2024-04-15 21:19:57.000000 lusid_express-0.0.3/tests/test_magic.py
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)      861 2024-04-15 21:19:55.000000 lusid_express-0.0.3/tests/test_vars.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:08:27.503747 lusid_express-0.1.132/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-16 18:08:24.000000 lusid_express-0.1.132/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-04-16 18:08:24.000000 lusid_express-0.1.132/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6550 2024-04-16 18:08:27.503747 lusid_express-0.1.132/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5908 2024-04-16 18:08:24.000000 lusid_express-0.1.132/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 18:08:27.503747 lusid_express-0.1.132/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2024-04-16 18:08:24.000000 lusid_express-0.1.132/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:08:27.499747 lusid_express-0.1.132/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:08:27.501747 lusid_express-0.1.132/src/lusid_express/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-16 18:08:24.000000 lusid_express-0.1.132/src/lusid_express/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1909 2024-04-16 18:08:24.000000 lusid_express-0.1.132/src/lusid_express/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:08:27.502746 lusid_express-0.1.132/src/lusid_express/apis/
+-rw-rw-rw-   0 root         (0) root         (0)     1414 2024-04-16 18:08:24.000000 lusid_express-0.1.132/src/lusid_express/apis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:08:27.502746 lusid_express-0.1.132/src/lusid_express/config/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-16 18:08:24.000000 lusid_express-0.1.132/src/lusid_express/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:08:27.502746 lusid_express-0.1.132/src/lusid_express/markdown/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-16 18:08:24.000000 lusid_express-0.1.132/src/lusid_express/markdown/PRELOADED_VARS.md
+-rw-rw-rw-   0 root         (0) root         (0)      298 2024-04-16 18:08:24.000000 lusid_express-0.1.132/src/lusid_express/markdown/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:08:27.502746 lusid_express-0.1.132/src/lusid_express.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6550 2024-04-16 18:08:27.000000 lusid_express-0.1.132/src/lusid_express.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      458 2024-04-16 18:08:27.000000 lusid_express-0.1.132/src/lusid_express.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 18:08:27.000000 lusid_express-0.1.132/src/lusid_express.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2024-04-16 18:08:27.000000 lusid_express-0.1.132/src/lusid_express.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-16 18:08:27.000000 lusid_express-0.1.132/src/lusid_express.egg-info/top_level.txt
```

### Comparing `lusid_express-0.0.3/LICENSE` & `lusid_express-0.1.132/LICENSE`

 * *Files identical despite different names*

### Comparing `lusid_express-0.0.3/PKG-INFO` & `lusid_express-0.1.132/src/lusid_express.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,23 @@
 Metadata-Version: 2.1
-Name: lusid_express
-Version: 0.0.3
+Name: lusid-express
+Version: 0.1.132
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyyaml
-Requires-Dist: luminesce-sdk-preview==1.14.758
-Requires-Dist: lusid-jam==0.1.2
-Requires-Dist: lusid-sdk-preview==1.1.120
-Requires-Dist: fbnlab-preview==0.1.108
-Requires-Dist: finbourne-access-sdk==0.0.3751
-Requires-Dist: finbourne-identity-sdk==0.0.2834
-Requires-Dist: finbourne-insights-sdk-preview==0.0.763
-Requires-Dist: finbourne-sdk-utilities==0.0.10
-Requires-Dist: lusid-configuration-sdk-preview==0.1.514
-Requires-Dist: lusid-drive-sdk-preview==0.1.617
-Requires-Dist: lusid-notifications-sdk-preview==0.1.923
-Requires-Dist: lusid-scheduler-sdk-preview==0.0.829
-Requires-Dist: lusid-workflow-sdk-preview==0.1.810
-Requires-Dist: lusidtools==1.0.14
-Requires-Dist: dve-lumipy-preview==0.1.1075
 
 
 # lusid-express
 ##### *`lusid-express` is a python package that makes it quick and easy to get started using Lusid and Luminesce.*
 
 
 
@@ -171,7 +157,9 @@
 | Variable Name | Statement         | Description                          |
 |---------------|-------------------|--------------------------------------|
 | lu          | `import lusid as lu` | Main LUSID package                   |
 | lm          | `import lusid.models as lm` | LUSID models module                  |
 | apis         | `import lusid_express.apis as apis` | convenience package providing pre-authenticated api access.                 |
 
 
+
+
```

### Comparing `lusid_express-0.0.3/README.md` & `lusid_express-0.1.132/README.md`

 * *Files identical despite different names*

### Comparing `lusid_express-0.0.3/setup.py` & `lusid_express-0.1.132/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from setuptools import setup, find_packages
 
 
 # List of requirements
 requirements = [
     'pyyaml',
     'luminesce-sdk-preview==1.14.758',
-    'lusid-jam==0.1.2',
+    'lusid-jam==0.1.132',
     'lusid-sdk-preview==1.1.120',
-    'fbnlab-preview==0.1.108',
-    'finbourne-access-sdk==0.0.3751',
+    'fbnlab-preview==0.1.13208',
+    'finbourne-access-sdk==0.1.132751',
     'finbourne-identity-sdk==0.0.2834',
     'finbourne-insights-sdk-preview==0.0.763',
     'finbourne-sdk-utilities==0.0.10',
-    'lusid-configuration-sdk-preview==0.1.514',
-    'lusid-drive-sdk-preview==0.1.617',
-    'lusid-notifications-sdk-preview==0.1.923',
+    'lusid-configuration-sdk-preview==0.1.13214',
+    'lusid-drive-sdk-preview==0.1.13217',
+    'lusid-notifications-sdk-preview==0.1.13223',
     'lusid-scheduler-sdk-preview==0.0.829',
-    'lusid-workflow-sdk-preview==0.1.810',
+    'lusid-workflow-sdk-preview==0.1.13210',
     'lusidtools==1.0.14',
-    'dve-lumipy-preview==0.1.1075'
+    'dve-lumipy-preview==0.1.132075'
 ]
 
 
 
 
 setup(
     name='lusid_express',
-    version='0.0.3',
+    version='0.1.132',
     package_dir={'': 'src'},  # tells setuptools that packages are under src
     packages=find_packages(where='src'),  # tells setuptools to look for packages in src
     install_requires=requirements,
     description='lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.',
     long_description=open('README.md').read(),
     include_package_data=True,  
     long_description_content_type='text/markdown',
```

### Comparing `lusid_express-0.0.3/src/lusid_express/__main__.py` & `lusid_express-0.1.132/src/lusid_express/__main__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-0.0.3/src/lusid_express/apis/__init__.py` & `lusid_express-0.1.132/src/lusid_express/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-0.0.3/src/lusid_express.egg-info/PKG-INFO` & `lusid_express-0.1.132/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,23 @@
 Metadata-Version: 2.1
 Name: lusid_express
-Version: 0.0.3
+Version: 0.1.132
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyyaml
-Requires-Dist: luminesce-sdk-preview==1.14.758
-Requires-Dist: lusid-jam==0.1.2
-Requires-Dist: lusid-sdk-preview==1.1.120
-Requires-Dist: fbnlab-preview==0.1.108
-Requires-Dist: finbourne-access-sdk==0.0.3751
-Requires-Dist: finbourne-identity-sdk==0.0.2834
-Requires-Dist: finbourne-insights-sdk-preview==0.0.763
-Requires-Dist: finbourne-sdk-utilities==0.0.10
-Requires-Dist: lusid-configuration-sdk-preview==0.1.514
-Requires-Dist: lusid-drive-sdk-preview==0.1.617
-Requires-Dist: lusid-notifications-sdk-preview==0.1.923
-Requires-Dist: lusid-scheduler-sdk-preview==0.0.829
-Requires-Dist: lusid-workflow-sdk-preview==0.1.810
-Requires-Dist: lusidtools==1.0.14
-Requires-Dist: dve-lumipy-preview==0.1.1075
 
 
 # lusid-express
 ##### *`lusid-express` is a python package that makes it quick and easy to get started using Lusid and Luminesce.*
 
 
 
@@ -171,7 +157,9 @@
 | Variable Name | Statement         | Description                          |
 |---------------|-------------------|--------------------------------------|
 | lu          | `import lusid as lu` | Main LUSID package                   |
 | lm          | `import lusid.models as lm` | LUSID models module                  |
 | apis         | `import lusid_express.apis as apis` | convenience package providing pre-authenticated api access.                 |
 
 
+
+
```

