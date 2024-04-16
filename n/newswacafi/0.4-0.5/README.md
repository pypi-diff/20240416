# Comparing `tmp/newswacafi-0.4.tar.gz` & `tmp/newswacafi-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newswacafi-0.4.tar", last modified: Tue Apr  9 06:59:55 2024, max compression
+gzip compressed data, was "newswacafi-0.5.tar", last modified: Tue Apr 16 17:40:41 2024, max compression
```

## Comparing `newswacafi-0.4.tar` & `newswacafi-0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-09 06:59:55.863498 newswacafi-0.4/
--rw-r--r--   0 moussier   (501) staff       (20)     1474 2024-04-09 06:59:55.863244 newswacafi-0.4/PKG-INFO
--rw-r--r--   0 moussier   (501) staff       (20)     1000 2024-03-22 09:36:59.000000 newswacafi-0.4/README.md
-drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-09 06:59:55.861161 newswacafi-0.4/examples/
--rw-r--r--   0 moussier   (501) staff       (20)        0 2024-03-20 14:47:19.000000 newswacafi-0.4/examples/__init__.py
--rw-r--r--   0 moussier   (501) staff       (20)      461 2024-03-23 07:09:52.000000 newswacafi-0.4/examples/base.py
-drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-09 06:59:55.861986 newswacafi-0.4/newswacafi/
--rw-r--r--   0 moussier   (501) staff       (20)        0 2024-03-20 13:43:15.000000 newswacafi-0.4/newswacafi/__init__.py
--rw-r--r--   0 moussier   (501) staff       (20)     2023 2024-04-09 06:59:18.000000 newswacafi-0.4/newswacafi/api.py
--rw-r--r--   0 moussier   (501) staff       (20)      445 2024-03-20 14:44:24.000000 newswacafi-0.4/newswacafi/response.py
-drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-09 06:59:55.862944 newswacafi-0.4/newswacafi.egg-info/
--rw-r--r--   0 moussier   (501) staff       (20)     1474 2024-04-09 06:59:55.000000 newswacafi-0.4/newswacafi.egg-info/PKG-INFO
--rw-r--r--   0 moussier   (501) staff       (20)      289 2024-04-09 06:59:55.000000 newswacafi-0.4/newswacafi.egg-info/SOURCES.txt
--rw-r--r--   0 moussier   (501) staff       (20)        1 2024-04-09 06:59:55.000000 newswacafi-0.4/newswacafi.egg-info/dependency_links.txt
--rw-r--r--   0 moussier   (501) staff       (20)        9 2024-04-09 06:59:55.000000 newswacafi-0.4/newswacafi.egg-info/requires.txt
--rw-r--r--   0 moussier   (501) staff       (20)       20 2024-04-09 06:59:55.000000 newswacafi-0.4/newswacafi.egg-info/top_level.txt
--rw-r--r--   0 moussier   (501) staff       (20)       38 2024-04-09 06:59:55.863550 newswacafi-0.4/setup.cfg
--rw-r--r--   0 moussier   (501) staff       (20)      775 2024-04-09 06:59:45.000000 newswacafi-0.4/setup.py
+drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-16 17:40:41.617756 newswacafi-0.5/
+-rw-r--r--   0 moussier   (501) staff       (20)     1474 2024-04-16 17:40:41.617525 newswacafi-0.5/PKG-INFO
+-rw-r--r--   0 moussier   (501) staff       (20)     1000 2024-03-22 09:36:59.000000 newswacafi-0.5/README.md
+drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-16 17:40:41.615446 newswacafi-0.5/examples/
+-rw-r--r--   0 moussier   (501) staff       (20)        0 2024-03-20 14:47:19.000000 newswacafi-0.5/examples/__init__.py
+-rw-r--r--   0 moussier   (501) staff       (20)      461 2024-03-23 07:09:52.000000 newswacafi-0.5/examples/base.py
+drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-16 17:40:41.616129 newswacafi-0.5/newswacafi/
+-rw-r--r--   0 moussier   (501) staff       (20)        0 2024-03-20 13:43:15.000000 newswacafi-0.5/newswacafi/__init__.py
+-rw-r--r--   0 moussier   (501) staff       (20)     2023 2024-04-09 06:59:18.000000 newswacafi-0.5/newswacafi/api.py
+-rw-r--r--   0 moussier   (501) staff       (20)      430 2024-04-16 17:27:17.000000 newswacafi-0.5/newswacafi/response.py
+drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-16 17:40:41.617243 newswacafi-0.5/newswacafi.egg-info/
+-rw-r--r--   0 moussier   (501) staff       (20)     1474 2024-04-16 17:40:41.000000 newswacafi-0.5/newswacafi.egg-info/PKG-INFO
+-rw-r--r--   0 moussier   (501) staff       (20)      289 2024-04-16 17:40:41.000000 newswacafi-0.5/newswacafi.egg-info/SOURCES.txt
+-rw-r--r--   0 moussier   (501) staff       (20)        1 2024-04-16 17:40:41.000000 newswacafi-0.5/newswacafi.egg-info/dependency_links.txt
+-rw-r--r--   0 moussier   (501) staff       (20)        9 2024-04-16 17:40:41.000000 newswacafi-0.5/newswacafi.egg-info/requires.txt
+-rw-r--r--   0 moussier   (501) staff       (20)       20 2024-04-16 17:40:41.000000 newswacafi-0.5/newswacafi.egg-info/top_level.txt
+-rw-r--r--   0 moussier   (501) staff       (20)       38 2024-04-16 17:40:41.617802 newswacafi-0.5/setup.cfg
+-rw-r--r--   0 moussier   (501) staff       (20)      775 2024-04-16 17:30:37.000000 newswacafi-0.5/setup.py
```

### Comparing `newswacafi-0.4/PKG-INFO` & `newswacafi-0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newswacafi
-Version: 0.4
+Version: 0.5
 Summary: Une bibliothèque Python pour interagir avec l'API de Newswacafi.
 Home-page: https://newswacafi.online
 Author: DRC WANALA
 Author-email: contact@newswacafi.online
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `newswacafi-0.4/README.md` & `newswacafi-0.5/README.md`

 * *Files identical despite different names*

### Comparing `newswacafi-0.4/newswacafi/api.py` & `newswacafi-0.5/newswacafi/api.py`

 * *Files identical despite different names*

### Comparing `newswacafi-0.4/newswacafi.egg-info/PKG-INFO` & `newswacafi-0.5/newswacafi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newswacafi
-Version: 0.4
+Version: 0.5
 Summary: Une bibliothèque Python pour interagir avec l'API de Newswacafi.
 Home-page: https://newswacafi.online
 Author: DRC WANALA
 Author-email: contact@newswacafi.online
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `newswacafi-0.4/setup.py` & `newswacafi-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='newswacafi',
-    version='0.4',
+    version='0.5',
     packages=find_packages(),
     install_requires=['requests'],
     author='DRC WANALA',
     author_email='contact@newswacafi.online',
     description='Une bibliothèque Python pour interagir avec l\'API de Newswacafi.',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

