# Comparing `tmp/harry_potter_yonier-1.3.tar.gz` & `tmp/harry_potter_yonier-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harry_potter_yonier-1.3.tar", last modified: Tue Apr 16 04:45:52 2024, max compression
+gzip compressed data, was "harry_potter_yonier-1.4.tar", last modified: Tue Apr 16 04:49:24 2024, max compression
```

## Comparing `harry_potter_yonier-1.3.tar` & `harry_potter_yonier-1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2024-04-16 04:45:52.391138 harry_potter_yonier-1.3/
--rw-r--r--   0 neo       (1000) neo       (1000)     1061 2024-04-16 03:01:09.000000 harry_potter_yonier-1.3/LICENSE.txt
--rw-r--r--   0 neo       (1000) neo       (1000)      690 2024-04-16 04:45:52.391138 harry_potter_yonier-1.3/PKG-INFO
--rw-r--r--   0 neo       (1000) neo       (1000)       57 2024-04-16 00:38:48.000000 harry_potter_yonier-1.3/README.md
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2024-04-16 04:45:52.390138 harry_potter_yonier-1.3/harry_potter_yonier/
--rw-r--r--   0 neo       (1000) neo       (1000)      115 2024-04-16 03:58:52.000000 harry_potter_yonier-1.3/harry_potter_yonier/__init__.py
--rw-r--r--   0 neo       (1000) neo       (1000)      936 2024-04-16 04:29:20.000000 harry_potter_yonier-1.3/harry_potter_yonier/__main__.py
--rw-r--r--   0 neo       (1000) neo       (1000)      885 2024-04-16 04:45:05.000000 harry_potter_yonier-1.3/harry_potter_yonier/get_one_person.py
--rw-r--r--   0 neo       (1000) neo       (1000)      508 2024-04-16 03:58:17.000000 harry_potter_yonier-1.3/harry_potter_yonier/get_person.py
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2024-04-16 04:45:52.391138 harry_potter_yonier-1.3/harry_potter_yonier.egg-info/
--rw-r--r--   0 neo       (1000) neo       (1000)      690 2024-04-16 04:45:52.000000 harry_potter_yonier-1.3/harry_potter_yonier.egg-info/PKG-INFO
--rw-r--r--   0 neo       (1000) neo       (1000)      426 2024-04-16 04:45:52.000000 harry_potter_yonier-1.3/harry_potter_yonier.egg-info/SOURCES.txt
--rw-r--r--   0 neo       (1000) neo       (1000)        1 2024-04-16 04:45:52.000000 harry_potter_yonier-1.3/harry_potter_yonier.egg-info/dependency_links.txt
--rw-r--r--   0 neo       (1000) neo       (1000)       62 2024-04-16 04:45:52.000000 harry_potter_yonier-1.3/harry_potter_yonier.egg-info/entry_points.txt
--rw-r--r--   0 neo       (1000) neo       (1000)        9 2024-04-16 04:45:52.000000 harry_potter_yonier-1.3/harry_potter_yonier.egg-info/requires.txt
--rw-r--r--   0 neo       (1000) neo       (1000)       20 2024-04-16 04:45:52.000000 harry_potter_yonier-1.3/harry_potter_yonier.egg-info/top_level.txt
--rw-r--r--   0 neo       (1000) neo       (1000)       38 2024-04-16 04:45:52.391138 harry_potter_yonier-1.3/setup.cfg
--rw-r--r--   0 neo       (1000) neo       (1000)     1199 2024-04-16 04:28:30.000000 harry_potter_yonier-1.3/setup.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2024-04-16 04:49:24.998047 harry_potter_yonier-1.4/
+-rw-r--r--   0 neo       (1000) neo       (1000)     1061 2024-04-16 03:01:09.000000 harry_potter_yonier-1.4/LICENSE.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)      690 2024-04-16 04:49:24.998047 harry_potter_yonier-1.4/PKG-INFO
+-rw-r--r--   0 neo       (1000) neo       (1000)       57 2024-04-16 00:38:48.000000 harry_potter_yonier-1.4/README.md
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2024-04-16 04:49:24.997047 harry_potter_yonier-1.4/harry_potter_yonier/
+-rw-r--r--   0 neo       (1000) neo       (1000)      115 2024-04-16 03:58:52.000000 harry_potter_yonier-1.4/harry_potter_yonier/__init__.py
+-rw-r--r--   0 neo       (1000) neo       (1000)      936 2024-04-16 04:29:20.000000 harry_potter_yonier-1.4/harry_potter_yonier/__main__.py
+-rw-r--r--   0 neo       (1000) neo       (1000)      885 2024-04-16 04:45:05.000000 harry_potter_yonier-1.4/harry_potter_yonier/get_one_person.py
+-rw-r--r--   0 neo       (1000) neo       (1000)      508 2024-04-16 03:58:17.000000 harry_potter_yonier-1.4/harry_potter_yonier/get_person.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2024-04-16 04:49:24.997047 harry_potter_yonier-1.4/harry_potter_yonier.egg-info/
+-rw-r--r--   0 neo       (1000) neo       (1000)      690 2024-04-16 04:49:24.000000 harry_potter_yonier-1.4/harry_potter_yonier.egg-info/PKG-INFO
+-rw-r--r--   0 neo       (1000) neo       (1000)      426 2024-04-16 04:49:24.000000 harry_potter_yonier-1.4/harry_potter_yonier.egg-info/SOURCES.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)        1 2024-04-16 04:49:24.000000 harry_potter_yonier-1.4/harry_potter_yonier.egg-info/dependency_links.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)       70 2024-04-16 04:49:24.000000 harry_potter_yonier-1.4/harry_potter_yonier.egg-info/entry_points.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)        9 2024-04-16 04:49:24.000000 harry_potter_yonier-1.4/harry_potter_yonier.egg-info/requires.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)       20 2024-04-16 04:49:24.000000 harry_potter_yonier-1.4/harry_potter_yonier.egg-info/top_level.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)       38 2024-04-16 04:49:24.998047 harry_potter_yonier-1.4/setup.cfg
+-rw-r--r--   0 neo       (1000) neo       (1000)     1207 2024-04-16 04:49:07.000000 harry_potter_yonier-1.4/setup.py
```

### Comparing `harry_potter_yonier-1.3/LICENSE.txt` & `harry_potter_yonier-1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `harry_potter_yonier-1.3/PKG-INFO` & `harry_potter_yonier-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harry_potter_yonier
-Version: 1.3
+Version: 1.4
 Summary: Permite consumir el API de Harry Potter para obtener o listar personajes
 Home-page: https://github.com/YonierGomez/harrypotter_python
 Author: Yonier Asprilla
 Author-email: yoonier13@gmail.com
 License: MIT
 Keywords: harrypotter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `harry_potter_yonier-1.3/harry_potter_yonier/__main__.py` & `harry_potter_yonier-1.4/harry_potter_yonier/__main__.py`

 * *Files identical despite different names*

### Comparing `harry_potter_yonier-1.3/harry_potter_yonier/get_one_person.py` & `harry_potter_yonier-1.4/harry_potter_yonier/get_one_person.py`

 * *Files identical despite different names*

### Comparing `harry_potter_yonier-1.3/harry_potter_yonier.egg-info/PKG-INFO` & `harry_potter_yonier-1.4/harry_potter_yonier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harry_potter_yonier
-Version: 1.3
+Version: 1.4
 Summary: Permite consumir el API de Harry Potter para obtener o listar personajes
 Home-page: https://github.com/YonierGomez/harrypotter_python
 Author: Yonier Asprilla
 Author-email: yoonier13@gmail.com
 License: MIT
 Keywords: harrypotter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `harry_potter_yonier-1.3/setup.py` & `harry_potter_yonier-1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from pathlib import Path # > 3.6
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = 'v1.3'
+VERSION = 'v1.4'
 DESCRIPTION = 'Permite consumir el API de Harry Potter para obtener o listar personajes'
 PACKAGE_NAME = 'harry_potter_yonier'
 AUTHOR = 'Yonier Asprilla'
 EMAIL = 'yoonier13@gmail.com'
 GITHUB_URL = 'https://github.com/YonierGomez/harrypotter_python'
 
 setup(
     name = PACKAGE_NAME,
     packages = [PACKAGE_NAME],
     entry_points={
         "console_scripts":
-            ["yonierpotter=harry_potter_yonier.__main__"]
+            ["yonierpotter=harry_potter_yonier.__main__:call_me"]
     },
     version = VERSION,
     license='MIT',
     description = DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     author = AUTHOR,
```

