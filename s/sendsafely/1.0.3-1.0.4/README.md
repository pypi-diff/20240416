# Comparing `tmp/sendsafely-1.0.3.tar.gz` & `tmp/sendsafely-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sendsafely-1.0.3.tar", last modified: Thu Sep 14 13:16:17 2023, max compression
+gzip compressed data, was "sendsafely-1.0.4.tar", last modified: Tue Apr  9 18:32:16 2024, max compression
```

## Comparing `sendsafely-1.0.3.tar` & `sendsafely-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 michaelnowak   (501) staff       (20)        0 2023-09-14 13:16:17.486891 sendsafely-1.0.3/
--rw-r--r--   0 michaelnowak   (501) staff       (20)    22455 2023-09-14 13:15:03.000000 sendsafely-1.0.3/LICENSE.txt
--rw-r--r--   0 michaelnowak   (501) staff       (20)       40 2023-09-14 13:15:03.000000 sendsafely-1.0.3/MANIFEST.in
--rw-r--r--   0 michaelnowak   (501) staff       (20)      524 2023-09-14 13:15:03.000000 sendsafely-1.0.3/NOTICE.txt
--rw-r--r--   0 michaelnowak   (501) staff       (20)     3306 2023-09-14 13:16:17.487350 sendsafely-1.0.3/PKG-INFO
--rw-r--r--   0 michaelnowak   (501) staff       (20)     2484 2023-09-14 13:16:14.000000 sendsafely-1.0.3/README
--rw-r--r--   0 michaelnowak   (501) staff       (20)     2484 2023-09-14 13:15:03.000000 sendsafely-1.0.3/README.md
--rw-r--r--   0 michaelnowak   (501) staff       (20)       27 2023-09-14 13:15:03.000000 sendsafely-1.0.3/requirements.txt
-drwxr-xr-x   0 michaelnowak   (501) staff       (20)        0 2023-09-14 13:16:17.451186 sendsafely-1.0.3/sendsafely/
--rw-r--r--   0 michaelnowak   (501) staff       (20)    16599 2023-09-14 13:15:03.000000 sendsafely-1.0.3/sendsafely/Package.py
--rw-r--r--   0 michaelnowak   (501) staff       (20)      432 2023-09-14 13:15:03.000000 sendsafely-1.0.3/sendsafely/Progress.py
--rw-r--r--   0 michaelnowak   (501) staff       (20)    11543 2023-09-14 13:15:03.000000 sendsafely-1.0.3/sendsafely/SendSafely.py
--rw-r--r--   0 michaelnowak   (501) staff       (20)      317 2023-09-14 13:15:03.000000 sendsafely-1.0.3/sendsafely/__init__.py
--rw-r--r--   0 michaelnowak   (501) staff       (20)     8326 2023-09-14 13:15:03.000000 sendsafely-1.0.3/sendsafely/exceptions.py
--rw-r--r--   0 michaelnowak   (501) staff       (20)    12499 2023-09-14 13:15:03.000000 sendsafely-1.0.3/sendsafely/utilities.py
-drwxr-xr-x   0 michaelnowak   (501) staff       (20)        0 2023-09-14 13:16:17.485747 sendsafely-1.0.3/sendsafely.egg-info/
--rw-r--r--   0 michaelnowak   (501) staff       (20)     3306 2023-09-14 13:16:16.000000 sendsafely-1.0.3/sendsafely.egg-info/PKG-INFO
--rw-r--r--   0 michaelnowak   (501) staff       (20)      398 2023-09-14 13:16:16.000000 sendsafely-1.0.3/sendsafely.egg-info/SOURCES.txt
--rw-r--r--   0 michaelnowak   (501) staff       (20)        1 2023-09-14 13:16:16.000000 sendsafely-1.0.3/sendsafely.egg-info/dependency_links.txt
--rw-r--r--   0 michaelnowak   (501) staff       (20)       14 2023-09-14 13:16:16.000000 sendsafely-1.0.3/sendsafely.egg-info/requires.txt
--rw-r--r--   0 michaelnowak   (501) staff       (20)       11 2023-09-14 13:16:16.000000 sendsafely-1.0.3/sendsafely.egg-info/top_level.txt
--rw-r--r--   0 michaelnowak   (501) staff       (20)      125 2023-09-14 13:16:17.492247 sendsafely-1.0.3/setup.cfg
--rw-r--r--   0 michaelnowak   (501) staff       (20)      872 2023-09-14 13:15:03.000000 sendsafely-1.0.3/setup.py
+drwxr-xr-x   0 michaelnowak   (501) staff       (20)        0 2024-04-09 18:32:16.488313 sendsafely-1.0.4/
+-rw-r--r--   0 michaelnowak   (501) staff       (20)    22455 2023-09-14 13:15:03.000000 sendsafely-1.0.4/LICENSE.txt
+-rw-r--r--   0 michaelnowak   (501) staff       (20)       40 2023-09-14 13:15:03.000000 sendsafely-1.0.4/MANIFEST.in
+-rw-r--r--   0 michaelnowak   (501) staff       (20)      524 2023-09-14 13:15:03.000000 sendsafely-1.0.4/NOTICE.txt
+-rw-r--r--   0 michaelnowak   (501) staff       (20)     3350 2024-04-09 18:32:16.487695 sendsafely-1.0.4/PKG-INFO
+-rw-r--r--   0 michaelnowak   (501) staff       (20)     2484 2024-04-09 18:32:13.000000 sendsafely-1.0.4/README
+-rw-r--r--   0 michaelnowak   (501) staff       (20)     2484 2023-09-14 13:15:03.000000 sendsafely-1.0.4/README.md
+-rw-r--r--   0 michaelnowak   (501) staff       (20)       27 2024-04-09 18:30:02.000000 sendsafely-1.0.4/requirements.txt
+drwxr-xr-x   0 michaelnowak   (501) staff       (20)        0 2024-04-09 18:32:16.458571 sendsafely-1.0.4/sendsafely/
+-rw-r--r--   0 michaelnowak   (501) staff       (20)    16599 2024-04-09 18:29:54.000000 sendsafely-1.0.4/sendsafely/Package.py
+-rw-r--r--   0 michaelnowak   (501) staff       (20)      432 2023-09-14 13:15:03.000000 sendsafely-1.0.4/sendsafely/Progress.py
+-rw-r--r--   0 michaelnowak   (501) staff       (20)    11543 2024-04-09 18:29:54.000000 sendsafely-1.0.4/sendsafely/SendSafely.py
+-rw-r--r--   0 michaelnowak   (501) staff       (20)      317 2023-09-14 13:15:03.000000 sendsafely-1.0.4/sendsafely/__init__.py
+-rw-r--r--   0 michaelnowak   (501) staff       (20)     8326 2023-09-14 13:15:03.000000 sendsafely-1.0.4/sendsafely/exceptions.py
+-rw-r--r--   0 michaelnowak   (501) staff       (20)    12499 2023-09-14 13:15:03.000000 sendsafely-1.0.4/sendsafely/utilities.py
+drwxr-xr-x   0 michaelnowak   (501) staff       (20)        0 2024-04-09 18:32:16.485594 sendsafely-1.0.4/sendsafely.egg-info/
+-rw-r--r--   0 michaelnowak   (501) staff       (20)     3350 2024-04-09 18:32:16.000000 sendsafely-1.0.4/sendsafely.egg-info/PKG-INFO
+-rw-r--r--   0 michaelnowak   (501) staff       (20)      398 2024-04-09 18:32:16.000000 sendsafely-1.0.4/sendsafely.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelnowak   (501) staff       (20)        1 2024-04-09 18:32:16.000000 sendsafely-1.0.4/sendsafely.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelnowak   (501) staff       (20)       14 2024-04-09 18:32:16.000000 sendsafely-1.0.4/sendsafely.egg-info/requires.txt
+-rw-r--r--   0 michaelnowak   (501) staff       (20)       11 2024-04-09 18:32:16.000000 sendsafely-1.0.4/sendsafely.egg-info/top_level.txt
+-rw-r--r--   0 michaelnowak   (501) staff       (20)      125 2024-04-09 18:32:16.496859 sendsafely-1.0.4/setup.cfg
+-rw-r--r--   0 michaelnowak   (501) staff       (20)      872 2024-04-09 18:30:02.000000 sendsafely-1.0.4/setup.py
```

### Comparing `sendsafely-1.0.3/LICENSE.txt` & `sendsafely-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sendsafely-1.0.3/NOTICE.txt` & `sendsafely-1.0.4/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `sendsafely-1.0.3/PKG-INFO` & `sendsafely-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: sendsafely
-Version: 1.0.3
+Version: 1.0.4
 Summary: The SendSafely Client API allows programmatic access to SendSafely and provides a layer of abstraction from our REST API, which requires developers to perform several complex tasks in a correct manner.
 Home-page: https://github.com/SendSafely/Python-Client-API
 Author: SendSafely
 Author-email: support@sendsafely.com
 License: Apache License Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICE.txt
+Requires-Dist: requests
+Requires-Dist: PGPy
 
 # SendSafely Python API
 The SendSafely Python API lets you integrate SendSafely secure data transfer capabilities directly into your Python application. 
 
 ## Quickstart
 The example below shows you how to install the `sendsafely` package, import it as a module, and use it to create a package. Make sure that you have [Python 3 or higher installed, as well as pip and Setuptools](https://packaging.python.org/tutorials/installing-packages/).
```

### Comparing `sendsafely-1.0.3/README` & `sendsafely-1.0.4/README`

 * *Files identical despite different names*

### Comparing `sendsafely-1.0.3/README.md` & `sendsafely-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sendsafely-1.0.3/sendsafely/Package.py` & `sendsafely-1.0.4/sendsafely/Package.py`

 * *Files identical despite different names*

### Comparing `sendsafely-1.0.3/sendsafely/SendSafely.py` & `sendsafely-1.0.4/sendsafely/SendSafely.py`

 * *Files identical despite different names*

### Comparing `sendsafely-1.0.3/sendsafely/exceptions.py` & `sendsafely-1.0.4/sendsafely/exceptions.py`

 * *Files identical despite different names*

### Comparing `sendsafely-1.0.3/sendsafely/utilities.py` & `sendsafely-1.0.4/sendsafely/utilities.py`

 * *Files identical despite different names*

### Comparing `sendsafely-1.0.3/sendsafely.egg-info/PKG-INFO` & `sendsafely-1.0.4/sendsafely.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: sendsafely
-Version: 1.0.3
+Version: 1.0.4
 Summary: The SendSafely Client API allows programmatic access to SendSafely and provides a layer of abstraction from our REST API, which requires developers to perform several complex tasks in a correct manner.
 Home-page: https://github.com/SendSafely/Python-Client-API
 Author: SendSafely
 Author-email: support@sendsafely.com
 License: Apache License Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICE.txt
+Requires-Dist: requests
+Requires-Dist: PGPy
 
 # SendSafely Python API
 The SendSafely Python API lets you integrate SendSafely secure data transfer capabilities directly into your Python application. 
 
 ## Quickstart
 The example below shows you how to install the `sendsafely` package, import it as a module, and use it to create a package. Make sure that you have [Python 3 or higher installed, as well as pip and Setuptools](https://packaging.python.org/tutorials/installing-packages/).
```

### Comparing `sendsafely-1.0.3/setup.py` & `sendsafely-1.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
 	name='sendsafely',
-	version='1.0.3',
+	version='1.0.4',
 	packages=['sendsafely'],
 	description='The SendSafely Client API allows programmatic access to SendSafely and provides a layer of abstraction from our REST API, which requires developers to perform several complex tasks in a correct manner.',
 	long_description_content_type="text/markdown",
 	author='SendSafely',
 	author_email='support@sendsafely.com',
 	url='https://github.com/SendSafely/Python-Client-API',
 	install_requires=[
```

