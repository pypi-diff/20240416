# Comparing `tmp/pyweatherfr-5.2.2.tar.gz` & `tmp/pyweatherfr-5.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherfr-5.2.2.tar", last modified: Mon Apr 15 20:41:39 2024, max compression
+gzip compressed data, was "pyweatherfr-5.2.3.tar", last modified: Tue Apr 16 07:23:47 2024, max compression
```

## Comparing `pyweatherfr-5.2.2.tar` & `pyweatherfr-5.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:41:39.195191 pyweatherfr-5.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-15 20:40:55.000000 pyweatherfr-5.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-15 20:41:39.195191 pyweatherfr-5.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-15 20:40:55.000000 pyweatherfr-5.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-15 20:40:55.000000 pyweatherfr-5.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:41:39.191192 pyweatherfr-5.2.2/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-15 20:40:55.000000 pyweatherfr-5.2.2/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-15 20:40:55.000000 pyweatherfr-5.2.2/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    44284 2024-04-15 20:40:55.000000 pyweatherfr-5.2.2/pyweatherfr/pyweatherfr.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-15 20:40:55.000000 pyweatherfr-5.2.2/pyweatherfr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:41:39.191192 pyweatherfr-5.2.2/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-15 20:41:39.000000 pyweatherfr-5.2.2/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-15 20:41:39.000000 pyweatherfr-5.2.2/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:41:39.000000 pyweatherfr-5.2.2/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-15 20:41:39.000000 pyweatherfr-5.2.2/pyweatherfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:40:59.000000 pyweatherfr-5.2.2/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-15 20:41:39.000000 pyweatherfr-5.2.2/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 20:41:39.000000 pyweatherfr-5.2.2/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:41:39.195191 pyweatherfr-5.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-15 20:40:55.000000 pyweatherfr-5.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:23:47.135275 pyweatherfr-5.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-16 07:23:03.000000 pyweatherfr-5.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-16 07:23:47.135275 pyweatherfr-5.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-16 07:23:03.000000 pyweatherfr-5.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-16 07:23:03.000000 pyweatherfr-5.2.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:23:47.135275 pyweatherfr-5.2.3/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-16 07:23:03.000000 pyweatherfr-5.2.3/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-16 07:23:03.000000 pyweatherfr-5.2.3/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44338 2024-04-16 07:23:03.000000 pyweatherfr-5.2.3/pyweatherfr/pyweatherfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-16 07:23:03.000000 pyweatherfr-5.2.3/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:23:47.135275 pyweatherfr-5.2.3/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-16 07:23:47.000000 pyweatherfr-5.2.3/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-16 07:23:47.000000 pyweatherfr-5.2.3/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:23:47.000000 pyweatherfr-5.2.3/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-16 07:23:47.000000 pyweatherfr-5.2.3/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:23:08.000000 pyweatherfr-5.2.3/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-16 07:23:47.000000 pyweatherfr-5.2.3/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 07:23:47.000000 pyweatherfr-5.2.3/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 07:23:47.135275 pyweatherfr-5.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-16 07:23:03.000000 pyweatherfr-5.2.3/setup.py
```

### Comparing `pyweatherfr-5.2.2/LICENSE.txt` & `pyweatherfr-5.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.2.2/PKG-INFO` & `pyweatherfr-5.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.2.2
+Version: 5.2.3
 Summary: pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.2.2/README.md` & `pyweatherfr-5.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.2.2/pyweatherfr/args.py` & `pyweatherfr-5.2.3/pyweatherfr/args.py`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.2.2/pyweatherfr/pyweatherfr.py` & `pyweatherfr-5.2.3/pyweatherfr/pyweatherfr.py`

 * *Files 1% similar despite different names*

```diff
@@ -724,18 +724,20 @@
         data = json.loads(resultat)
         print_debug(str(json.dumps(data, indent=4,ensure_ascii=False)))
         ville = data["city"]
         if ville is None:
             ville=""
         lat = str(data["latitude"])
         long = str(data["longitude"])
-        dpt = str(data["state"])
+        dpt = data["state"]
         if dpt is None:
             dpt=""
         country = str(data["country_name"])
+        if country is None:
+            country=""        
         return ville, dpt, lat, long, country
 
 
 
 
 def obtain_city_data_from_gps():
     print_debug(
```

### Comparing `pyweatherfr-5.2.2/pyweatherfr.egg-info/PKG-INFO` & `pyweatherfr-5.2.3/pyweatherfr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.2.2
+Version: 5.2.3
 Summary: pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.2.2/setup.py` & `pyweatherfr-5.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="5.2.2",
+    version="5.2.3",
     description="pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
```

