# Comparing `tmp/ths_mongo_training_tools-0.1.7.tar.gz` & `tmp/ths_mongo_training_tools-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/tim/Downloads/myhexin/data_processing/ths_mongo_training_tools/dist/.tmp-l7lc5c7p/ths_mongo_training_tools-0.1.7.tar", last modified: Tue Apr 16 02:09:12 2024, max compression
+gzip compressed data, was "/Users/tim/Downloads/myhexin/data_processing/ths_mongo_training_tools/dist/.tmp-w95y85rs/ths_mongo_training_tools-0.1.8.tar", last modified: Tue Apr 16 02:15:13 2024, max compression
```

## Comparing `ths_mongo_training_tools-0.1.7.tar` & `ths_mongo_training_tools-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2024-04-16 02:09:12.800548 ths_mongo_training_tools-0.1.7/
--rw-r--r--   0 tim        (501) staff       (20)      788 2024-04-16 02:09:12.800360 ths_mongo_training_tools-0.1.7/PKG-INFO
--rw-r--r--   0 tim        (501) staff       (20)       38 2024-04-16 02:09:12.800592 ths_mongo_training_tools-0.1.7/setup.cfg
--rw-r--r--   0 tim        (501) staff       (20)      930 2024-04-16 02:08:54.000000 ths_mongo_training_tools-0.1.7/setup.py
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2024-04-16 02:09:12.800174 ths_mongo_training_tools-0.1.7/ths_mongo_training_tools.egg-info/
--rw-r--r--   0 tim        (501) staff       (20)      788 2024-04-16 02:09:12.000000 ths_mongo_training_tools-0.1.7/ths_mongo_training_tools.egg-info/PKG-INFO
--rw-r--r--   0 tim        (501) staff       (20)      247 2024-04-16 02:09:12.000000 ths_mongo_training_tools-0.1.7/ths_mongo_training_tools.egg-info/SOURCES.txt
--rw-r--r--   0 tim        (501) staff       (20)        1 2024-04-16 02:09:12.000000 ths_mongo_training_tools-0.1.7/ths_mongo_training_tools.egg-info/dependency_links.txt
--rw-r--r--   0 tim        (501) staff       (20)        8 2024-04-16 02:09:12.000000 ths_mongo_training_tools-0.1.7/ths_mongo_training_tools.egg-info/requires.txt
--rw-r--r--   0 tim        (501) staff       (20)        1 2024-04-16 02:09:12.000000 ths_mongo_training_tools-0.1.7/ths_mongo_training_tools.egg-info/top_level.txt
+drwxr-xr-x   0 tim        (501) staff       (20)        0 2024-04-16 02:15:13.194115 ths_mongo_training_tools-0.1.8/
+-rw-r--r--   0 tim        (501) staff       (20)      788 2024-04-16 02:15:13.193923 ths_mongo_training_tools-0.1.8/PKG-INFO
+-rw-r--r--   0 tim        (501) staff       (20)       38 2024-04-16 02:15:13.194160 ths_mongo_training_tools-0.1.8/setup.cfg
+-rw-r--r--   0 tim        (501) staff       (20)      930 2024-04-16 02:14:52.000000 ths_mongo_training_tools-0.1.8/setup.py
+drwxr-xr-x   0 tim        (501) staff       (20)        0 2024-04-16 02:15:13.193740 ths_mongo_training_tools-0.1.8/ths_mongo_training_tools.egg-info/
+-rw-r--r--   0 tim        (501) staff       (20)      788 2024-04-16 02:15:13.000000 ths_mongo_training_tools-0.1.8/ths_mongo_training_tools.egg-info/PKG-INFO
+-rw-r--r--   0 tim        (501) staff       (20)      247 2024-04-16 02:15:13.000000 ths_mongo_training_tools-0.1.8/ths_mongo_training_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 tim        (501) staff       (20)        1 2024-04-16 02:15:13.000000 ths_mongo_training_tools-0.1.8/ths_mongo_training_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 tim        (501) staff       (20)        8 2024-04-16 02:15:13.000000 ths_mongo_training_tools-0.1.8/ths_mongo_training_tools.egg-info/requires.txt
+-rw-r--r--   0 tim        (501) staff       (20)        1 2024-04-16 02:15:13.000000 ths_mongo_training_tools-0.1.8/ths_mongo_training_tools.egg-info/top_level.txt
```

### Comparing `ths_mongo_training_tools-0.1.7/PKG-INFO` & `ths_mongo_training_tools-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ths-mongo-training-tools
-Version: 0.1.7
+Version: 0.1.8
 Summary: Speech training status control
 Author: Tim Zhou
 Author-email: zhouyuntao110@gmail.com
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `ths_mongo_training_tools-0.1.7/setup.py` & `ths_mongo_training_tools-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ths-mongo-training-tools',
-    version='0.1.7',
+    version='0.1.8',
     author='Tim Zhou',
     author_email='zhouyuntao110@gmail.com',
     description='Speech training status control',
     packages=find_packages(),
     install_requires=[
         'pymongo'
     ],
```

### Comparing `ths_mongo_training_tools-0.1.7/ths_mongo_training_tools.egg-info/PKG-INFO` & `ths_mongo_training_tools-0.1.8/ths_mongo_training_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ths-mongo-training-tools
-Version: 0.1.7
+Version: 0.1.8
 Summary: Speech training status control
 Author: Tim Zhou
 Author-email: zhouyuntao110@gmail.com
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
```

