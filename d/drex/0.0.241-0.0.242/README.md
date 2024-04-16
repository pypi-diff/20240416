# Comparing `tmp/drex-0.0.241.tar.gz` & `tmp/drex-0.0.242.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drex-0.0.241.tar", last modified: Fri Mar 29 15:57:10 2024, max compression
+gzip compressed data, was "drex-0.0.242.tar", last modified: Tue Apr 16 13:44:01 2024, max compression
```

## Comparing `drex-0.0.241.tar` & `drex-0.0.242.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-03-29 15:57:10.408045 drex-0.0.241/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)       91 2024-03-29 15:43:01.000000 drex-0.0.241/.gitignore
--rw-r--r--   0 domizzi   (1000) domizzi   (1000)      461 2024-03-29 15:57:10.408045 drex-0.0.241/PKG-INFO
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)       97 2024-03-26 19:02:20.000000 drex-0.0.241/README.md
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-03-29 15:57:10.404045 drex-0.0.241/Simulation/
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-03-29 15:57:10.404045 drex-0.0.241/Simulation/src/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      326 2024-03-26 19:02:20.000000 drex-0.0.241/Simulation/src/main.py
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-03-29 15:57:10.404045 drex-0.0.241/data/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2912 2024-03-26 20:01:38.000000 drex-0.0.241/data/10MB.csv
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     7032 2024-03-26 20:01:41.000000 drex-0.0.241/data/1MB.csv
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2903 2024-03-26 20:01:25.000000 drex-0.0.241/data/200MB.csv
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1303 2024-03-26 20:01:44.000000 drex-0.0.241/data/50MB.csv
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-03-29 15:57:10.404045 drex-0.0.241/drex/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:09:29.000000 drex-0.0.241/drex/__init__.py
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-03-29 15:57:10.408045 drex-0.0.241/drex/utils/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:06:13.000000 drex-0.0.241/drex/utils/__init__.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      784 2024-03-26 21:04:00.000000 drex-0.0.241/drex/utils/load_data.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    10547 2024-03-26 19:02:20.000000 drex-0.0.241/drex/utils/poibin.py
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-03-29 15:57:10.408045 drex-0.0.241/drex/utils/reliability/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:06:19.000000 drex-0.0.241/drex/utils/reliability/__init__.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     5214 2024-03-28 16:17:33.000000 drex-0.0.241/drex/utils/reliability/fragment_handler.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     6772 2024-03-28 21:59:40.000000 drex-0.0.241/drex/utils/reliability/ida.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     4913 2024-03-28 16:17:33.000000 drex-0.0.241/drex/utils/reliability/utils.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     5083 2024-03-29 15:36:19.000000 drex-0.0.241/drex/utils/tool_functions.py
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-03-29 15:57:10.408045 drex-0.0.241/drex.egg-info/
--rw-r--r--   0 domizzi   (1000) domizzi   (1000)      461 2024-03-29 15:57:10.000000 drex-0.0.241/drex.egg-info/PKG-INFO
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      542 2024-03-29 15:57:10.000000 drex-0.0.241/drex.egg-info/SOURCES.txt
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        1 2024-03-29 15:57:10.000000 drex-0.0.241/drex.egg-info/dependency_links.txt
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        6 2024-03-29 15:57:10.000000 drex-0.0.241/drex.egg-info/requires.txt
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        5 2024-03-29 15:57:10.000000 drex-0.0.241/drex.egg-info/top_level.txt
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      582 2024-03-29 15:56:49.000000 drex-0.0.241/pyproject.toml
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)       38 2024-03-29 15:57:10.408045 drex-0.0.241/setup.cfg
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-03-29 15:57:10.408045 drex-0.0.241/test/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-29 15:39:56.000000 drex-0.0.241/test/__init__.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1321 2024-03-29 15:42:30.000000 drex-0.0.241/test/drex-test.py
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-16 13:44:01.958234 drex-0.0.242/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)       98 2024-03-29 18:39:48.000000 drex-0.0.242/.gitignore
+-rw-r--r--   0 domizzi   (1000) domizzi   (1000)      720 2024-04-16 13:44:01.958234 drex-0.0.242/PKG-INFO
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      335 2024-04-04 15:50:32.000000 drex-0.0.242/README.md
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-16 13:44:01.958234 drex-0.0.242/data/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2912 2024-03-26 20:01:38.000000 drex-0.0.242/data/10MB.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     7032 2024-03-26 20:01:41.000000 drex-0.0.242/data/1MB.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2903 2024-03-26 20:01:25.000000 drex-0.0.242/data/200MB.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1303 2024-03-26 20:01:44.000000 drex-0.0.242/data/50MB.csv
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-16 13:44:01.958234 drex-0.0.242/drex/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:09:29.000000 drex-0.0.242/drex/__init__.py
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-16 13:44:01.958234 drex-0.0.242/drex/schedulers/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      570 2024-04-15 08:46:06.000000 drex-0.0.242/drex/schedulers/algorithm1.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1418 2024-04-15 08:46:26.000000 drex-0.0.242/drex/schedulers/algorithm2.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     3138 2024-04-15 08:46:34.000000 drex-0.0.242/drex/schedulers/algorithm3.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1647 2024-04-15 08:30:49.000000 drex-0.0.242/drex/schedulers/random.py
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-16 13:44:01.958234 drex-0.0.242/drex/utils/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:06:13.000000 drex-0.0.242/drex/utils/__init__.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      784 2024-03-26 21:04:00.000000 drex-0.0.242/drex/utils/load_data.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    10547 2024-03-26 19:02:20.000000 drex-0.0.242/drex/utils/poibin.py
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-16 13:44:01.958234 drex-0.0.242/drex/utils/reliability/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:06:19.000000 drex-0.0.242/drex/utils/reliability/__init__.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     5214 2024-03-28 16:17:33.000000 drex-0.0.242/drex/utils/reliability/fragment_handler.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     6772 2024-03-28 21:59:40.000000 drex-0.0.242/drex/utils/reliability/ida.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     4913 2024-03-28 16:17:33.000000 drex-0.0.242/drex/utils/reliability/utils.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     5350 2024-04-15 08:30:49.000000 drex-0.0.242/drex/utils/tool_functions.py
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-16 13:44:01.958234 drex-0.0.242/drex.egg-info/
+-rw-r--r--   0 domizzi   (1000) domizzi   (1000)      720 2024-04-16 13:44:01.000000 drex-0.0.242/drex.egg-info/PKG-INFO
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      635 2024-04-16 13:44:01.000000 drex-0.0.242/drex.egg-info/SOURCES.txt
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        1 2024-04-16 13:44:01.000000 drex-0.0.242/drex.egg-info/dependency_links.txt
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)       12 2024-04-16 13:44:01.000000 drex-0.0.242/drex.egg-info/requires.txt
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        5 2024-04-16 13:44:01.000000 drex-0.0.242/drex.egg-info/top_level.txt
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      595 2024-04-16 13:38:39.000000 drex-0.0.242/pyproject.toml
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)       38 2024-04-16 13:44:01.958234 drex-0.0.242/setup.cfg
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-16 13:44:01.958234 drex-0.0.242/test/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-04-01 18:01:10.000000 drex-0.0.242/test/__init__.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2157 2024-04-15 08:38:51.000000 drex-0.0.242/test/drex-test.py
```

### Comparing `drex-0.0.241/data/10MB.csv` & `drex-0.0.242/data/10MB.csv`

 * *Files identical despite different names*

### Comparing `drex-0.0.241/data/1MB.csv` & `drex-0.0.242/data/1MB.csv`

 * *Files identical despite different names*

### Comparing `drex-0.0.241/data/200MB.csv` & `drex-0.0.242/data/200MB.csv`

 * *Files identical despite different names*

### Comparing `drex-0.0.241/data/50MB.csv` & `drex-0.0.242/data/50MB.csv`

 * *Files identical despite different names*

### Comparing `drex-0.0.241/drex/utils/load_data.py` & `drex-0.0.242/drex/utils/load_data.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.241/drex/utils/poibin.py` & `drex-0.0.242/drex/utils/poibin.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.241/drex/utils/reliability/fragment_handler.py` & `drex-0.0.242/drex/utils/reliability/fragment_handler.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.241/drex/utils/reliability/ida.py` & `drex-0.0.242/drex/utils/reliability/ida.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.241/drex/utils/reliability/utils.py` & `drex-0.0.242/drex/utils/reliability/utils.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.241/pyproject.toml` & `drex-0.0.242/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["setuptools>=64.0", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "drex"
-version = "0.0.241"
+version = "0.0.242"
 authors = [
   { name="Maxime, Dante, Haochen", email="dantsanc@pa.uc3m.es" },
 ]
 description = "DRex package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "numpy"
+    "numpy",
+    "scipy"
 ]
 
 [tool.setuptools.packages.find]
 exclude = ["data*", "Simulation*", "test*"]
 namespaces = false
```

