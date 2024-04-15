# Comparing `tmp/lusid_express-0.0.1.tar.gz` & `tmp/lusid_express-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_express-0.0.1.tar", last modified: Mon Apr 15 21:52:33 2024, max compression
+gzip compressed data, was "lusid_express-0.0.2.tar", last modified: Mon Apr 15 22:24:58 2024, max compression
```

## Comparing `lusid_express-0.0.1.tar` & `lusid_express-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,26 @@
-drwxr-xr-x   0 orlandogcalvo   (501) staff       (20)        0 2024-04-15 21:52:33.017879 lusid_express-0.0.1/
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)     1062 2024-04-15 21:42:24.000000 lusid_express-0.0.1/LICENSE
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)     7230 2024-04-15 21:52:33.017106 lusid_express-0.0.1/PKG-INFO
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)     5908 2024-04-15 20:56:02.000000 lusid_express-0.0.1/README.md
-drwxr-xr-x   0 orlandogcalvo   (501) staff       (20)        0 2024-04-15 21:52:33.016355 lusid_express-0.0.1/lusid_express.egg-info/
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)     7230 2024-04-15 21:52:32.000000 lusid_express-0.0.1/lusid_express.egg-info/PKG-INFO
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)      267 2024-04-15 21:52:32.000000 lusid_express-0.0.1/lusid_express.egg-info/SOURCES.txt
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)        1 2024-04-15 21:52:32.000000 lusid_express-0.0.1/lusid_express.egg-info/dependency_links.txt
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)      479 2024-04-15 21:52:32.000000 lusid_express-0.0.1/lusid_express.egg-info/requires.txt
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)        1 2024-04-15 21:52:32.000000 lusid_express-0.0.1/lusid_express.egg-info/top_level.txt
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)       38 2024-04-15 21:52:33.018060 lusid_express-0.0.1/setup.cfg
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)     1425 2024-04-15 21:50:52.000000 lusid_express-0.0.1/setup.py
-drwxr-xr-x   0 orlandogcalvo   (501) staff       (20)        0 2024-04-15 21:52:33.015820 lusid_express-0.0.1/tests/
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)     1025 2024-04-15 21:22:58.000000 lusid_express-0.0.1/tests/test_cli.py
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)      532 2024-04-15 21:19:57.000000 lusid_express-0.0.1/tests/test_magic.py
--rw-r--r--   0 orlandogcalvo   (501) staff       (20)      861 2024-04-15 21:19:55.000000 lusid_express-0.0.1/tests/test_vars.py
+drwxr-xr-x   0 orlandogcalvo   (501) staff       (20)        0 2024-04-15 22:24:58.147924 lusid_express-0.0.2/
+-rw-r--r--   0 orlandogcalvo   (501) staff       (20)     1062 2024-04-15 21:42:24.000000 lusid_express-0.0.2/LICENSE
+-rw-r--r--   0 orlandogcalvo   (501) staff       (20)     7230 2024-04-15 22:24:58.147299 lusid_express-0.0.2/PKG-INFO
+-rw-r--r--   0 orlandogcalvo   (501) staff       (20)     5908 2024-04-15 20:56:02.000000 lusid_express-0.0.2/README.md
+-rw-r--r--   0 orlandogcalvo   (501) staff       (20)       38 2024-04-15 22:24:58.147986 lusid_express-0.0.2/setup.cfg
+-rw-r--r--   0 orlandogcalvo   (501) staff       (20)     1561 2024-04-15 22:23:00.000000 lusid_express-0.0.2/setup.py
+drwxr-xr-x   0 orlandogcalvo   (501) staff       (20)        0 2024-04-15 22:24:58.124104 lusid_express-0.0.2/src/
+drwxr-xr-x   0 orlandogcalvo   (501) staff       (20)        0 2024-04-15 22:24:58.127406 lusid_express-0.0.2/src/lusid_express/
+-rw-r--r--   0 orlandogcalvo   (501) staff       (20)       30 2024-04-15 19:22:44.000000 lusid_express-0.0.2/src/lusid_express/__init__.py
+-rw-r--r--   0 orlandogcalvo   (501) staff       (20)     1909 2024-04-15 21:50:26.000000 lusid_express-0.0.2/src/lusid_express/__main__.py
+drwxr-xr-x   0 orlandogcalvo   (501) staff       (20)        0 2024-04-15 22:24:58.140813 lusid_express-0.0.2/src/lusid_express/apis/
+-rw-r--r--   0 orlandogcalvo   (501) staff       (20)     1414 2024-04-15 18:47:54.000000 lusid_express-0.0.2/src/lusid_express/apis/__init__.py
+drwxr-xr-x   0 orlandogcalvo   (501) staff       (20)        0 2024-04-15 22:24:58.141726 lusid_express-0.0.2/src/lusid_express/config/
+-rw-r--r--   0 orlandogcalvo   (501) staff       (20)      369 2024-04-15 19:34:41.000000 lusid_express-0.0.2/src/lusid_express/config/__init__.py
+drwxr-xr-x   0 orlandogcalvo   (501) staff       (20)        0 2024-04-15 22:24:58.143200 lusid_express-0.0.2/src/lusid_express/markdown/
+-rw-r--r--   0 orlandogcalvo   (501) staff       (20)      298 2024-04-15 20:28:24.000000 lusid_express-0.0.2/src/lusid_express/markdown/__init__.py
+drwxr-xr-x   0 orlandogcalvo   (501) staff       (20)        0 2024-04-15 22:24:58.146821 lusid_express-0.0.2/src/lusid_express.egg-info/
+-rw-r--r--   0 orlandogcalvo   (501) staff       (20)     7230 2024-04-15 22:24:58.000000 lusid_express-0.0.2/src/lusid_express.egg-info/PKG-INFO
+-rw-r--r--   0 orlandogcalvo   (501) staff       (20)      458 2024-04-15 22:24:58.000000 lusid_express-0.0.2/src/lusid_express.egg-info/SOURCES.txt
+-rw-r--r--   0 orlandogcalvo   (501) staff       (20)        1 2024-04-15 22:24:58.000000 lusid_express-0.0.2/src/lusid_express.egg-info/dependency_links.txt
+-rw-r--r--   0 orlandogcalvo   (501) staff       (20)      479 2024-04-15 22:24:58.000000 lusid_express-0.0.2/src/lusid_express.egg-info/requires.txt
+-rw-r--r--   0 orlandogcalvo   (501) staff       (20)       14 2024-04-15 22:24:58.000000 lusid_express-0.0.2/src/lusid_express.egg-info/top_level.txt
+drwxr-xr-x   0 orlandogcalvo   (501) staff       (20)        0 2024-04-15 22:24:58.146327 lusid_express-0.0.2/tests/
+-rw-r--r--   0 orlandogcalvo   (501) staff       (20)     1460 2024-04-15 22:05:27.000000 lusid_express-0.0.2/tests/test_cli.py
+-rw-r--r--   0 orlandogcalvo   (501) staff       (20)      532 2024-04-15 21:19:57.000000 lusid_express-0.0.2/tests/test_magic.py
+-rw-r--r--   0 orlandogcalvo   (501) staff       (20)      861 2024-04-15 21:19:55.000000 lusid_express-0.0.2/tests/test_vars.py
```

### Comparing `lusid_express-0.0.1/LICENSE` & `lusid_express-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lusid_express-0.0.1/PKG-INFO` & `lusid_express-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid_express
-Version: 0.0.1
+Version: 0.0.2
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `lusid_express-0.0.1/README.md` & `lusid_express-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lusid_express-0.0.1/lusid_express.egg-info/PKG-INFO` & `lusid_express-0.0.2/src/lusid_express.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid_express
-Version: 0.0.1
+Version: 0.0.2
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `lusid_express-0.0.1/setup.py` & `lusid_express-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,16 +22,17 @@
 ]
 
 
 
 
 setup(
     name='lusid_express',
-    version='0.0.1',
-    packages=find_packages(),
+    version='0.0.2',
+    package_dir={'': 'src'},  # tells setuptools that packages are under src
+    packages=find_packages(where='src'),  # tells setuptools to look for packages in src
     install_requires=requirements,
     description='lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Orlando Calvo',
     author_email='orlando.calvo@finbourne.com',
     url='https://gitlab.com/orlando.calvo1/lusid-express',
```

### Comparing `lusid_express-0.0.1/tests/test_magic.py` & `lusid_express-0.0.2/tests/test_magic.py`

 * *Files identical despite different names*

### Comparing `lusid_express-0.0.1/tests/test_vars.py` & `lusid_express-0.0.2/tests/test_vars.py`

 * *Files identical despite different names*

