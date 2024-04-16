# Comparing `tmp/cool_ml-0.0.0.tar.gz` & `tmp/cool_ml-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cool_ml-0.0.0.tar", last modified: Mon Apr 15 13:41:26 2024, max compression
+gzip compressed data, was "cool_ml-0.0.1.tar", last modified: Tue Apr 16 11:58:44 2024, max compression
```

## Comparing `cool_ml-0.0.0.tar` & `cool_ml-0.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:41:26.274952 cool_ml-0.0.0/
--rw-r--r--   0 root         (0) root         (0)     3566 2024-04-15 13:41:26.270952 cool_ml-0.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2913 2024-04-15 13:41:10.000000 cool_ml-0.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 13:41:26.274952 cool_ml-0.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1371 2024-04-15 13:41:10.000000 cool_ml-0.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:41:26.270952 cool_ml-0.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:41:26.270952 cool_ml-0.0.0/src/cool_ml.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3566 2024-04-15 13:41:26.000000 cool_ml-0.0.0/src/cool_ml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      192 2024-04-15 13:41:26.000000 cool_ml-0.0.0/src/cool_ml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 13:41:26.000000 cool_ml-0.0.0/src/cool_ml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-15 13:41:26.000000 cool_ml-0.0.0/src/cool_ml.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 13:41:26.000000 cool_ml-0.0.0/src/cool_ml.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 11:58:44.358595 cool_ml-0.0.1/
+-rw-r--r--   0 root         (0) root         (0)     3566 2024-04-16 11:58:44.358595 cool_ml-0.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2913 2024-04-16 11:58:27.000000 cool_ml-0.0.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 11:58:44.358595 cool_ml-0.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2024-04-16 11:58:27.000000 cool_ml-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 11:58:44.354595 cool_ml-0.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 11:58:44.358595 cool_ml-0.0.1/src/cool_ml.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3566 2024-04-16 11:58:44.000000 cool_ml-0.0.1/src/cool_ml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      192 2024-04-16 11:58:44.000000 cool_ml-0.0.1/src/cool_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 11:58:44.000000 cool_ml-0.0.1/src/cool_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-16 11:58:44.000000 cool_ml-0.0.1/src/cool_ml.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 11:58:44.000000 cool_ml-0.0.1/src/cool_ml.egg-info/top_level.txt
```

### Comparing `cool_ml-0.0.0/PKG-INFO` & `cool_ml-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cool_ml
-Version: 0.0.0
+Version: 0.0.1
 Summary: Cool ML is a machine learning workflow developed to optimize thermionic double-assymmetric barrier heterostructures based on semiconductors
 Home-page: https://gitlab.citius.usc.es/julian.garcia.fernandez/cool_ml
 Author: 
 Author-email: 
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -35,15 +35,15 @@
     sudo apt update
     sudo apt install python3-pip
 
 **Instalation of MLFoMpy via pip3**
 
 For basic usage of the tool (figure of merit extraction), install the tool using pip3:
 
-    pip3 install cool_ml
+    pip3 install cool-ml
 
 and check the library is installed by importing it from a **python3 terminal**:
 
     import cool_ml
 
 Unless an error comes up, Cool ML is now installed on your environment.
```

### Comparing `cool_ml-0.0.0/README.md` & `cool_ml-0.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     sudo apt update
     sudo apt install python3-pip
 
 **Instalation of MLFoMpy via pip3**
 
 For basic usage of the tool (figure of merit extraction), install the tool using pip3:
 
-    pip3 install cool_ml
+    pip3 install cool-ml
 
 and check the library is installed by importing it from a **python3 terminal**:
 
     import cool_ml
 
 Unless an error comes up, Cool ML is now installed on your environment.
```

### Comparing `cool_ml-0.0.0/setup.py` & `cool_ml-0.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description=''
     with open(Path(Path(__file__).parent,'README.md'), 'r') as fh:
         long_description=fh.read()
     return long_description
 
 setuptools.setup(
     name='cool_ml',
-    version='0.0.0',
+    version='0.0.1',
     description='Cool ML is a machine learning workflow developed to optimize thermionic double-assymmetric barrier heterostructures based on semiconductors',
     long_description=get_long_description(),
     long_description_content_type='text/markdown',
     author='',
     author_email='',
     url='https://gitlab.citius.usc.es/julian.garcia.fernandez/cool_ml',
     setup_requires=['setuptools','numpy','pathlib '],
```

### Comparing `cool_ml-0.0.0/src/cool_ml.egg-info/PKG-INFO` & `cool_ml-0.0.1/src/cool_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cool-ml
-Version: 0.0.0
+Version: 0.0.1
 Summary: Cool ML is a machine learning workflow developed to optimize thermionic double-assymmetric barrier heterostructures based on semiconductors
 Home-page: https://gitlab.citius.usc.es/julian.garcia.fernandez/cool_ml
 Author: 
 Author-email: 
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -35,15 +35,15 @@
     sudo apt update
     sudo apt install python3-pip
 
 **Instalation of MLFoMpy via pip3**
 
 For basic usage of the tool (figure of merit extraction), install the tool using pip3:
 
-    pip3 install cool_ml
+    pip3 install cool-ml
 
 and check the library is installed by importing it from a **python3 terminal**:
 
     import cool_ml
 
 Unless an error comes up, Cool ML is now installed on your environment.
```

