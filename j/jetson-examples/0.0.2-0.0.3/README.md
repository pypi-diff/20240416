# Comparing `tmp/jetson-examples-0.0.2.tar.gz` & `tmp/jetson_examples-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jetson-examples-0.0.2.tar", last modified: Fri Apr 12 11:18:31 2024, max compression
+gzip compressed data, was "jetson_examples-0.0.3.tar", last modified: Mon Apr 15 10:08:34 2024, max compression
```

## Comparing `jetson-examples-0.0.2.tar` & `jetson_examples-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 zhixin.luo   (501) staff       (20)        0 2024-04-12 11:18:31.956250 jetson-examples-0.0.2/
--rw-r--r--   0 zhixin.luo   (501) staff       (20)     1066 2024-04-12 06:30:15.000000 jetson-examples-0.0.2/LICENSE
--rw-r--r--   0 zhixin.luo   (501) staff       (20)     2751 2024-04-12 11:18:31.956051 jetson-examples-0.0.2/PKG-INFO
--rw-r--r--   0 zhixin.luo   (501) staff       (20)     2209 2024-04-12 10:10:04.000000 jetson-examples-0.0.2/README.md
-drwxr-xr-x   0 zhixin.luo   (501) staff       (20)        0 2024-04-12 11:18:31.955858 jetson-examples-0.0.2/jetson_examples.egg-info/
--rw-r--r--   0 zhixin.luo   (501) staff       (20)     2751 2024-04-12 11:18:31.000000 jetson-examples-0.0.2/jetson_examples.egg-info/PKG-INFO
--rw-r--r--   0 zhixin.luo   (501) staff       (20)      296 2024-04-12 11:18:31.000000 jetson-examples-0.0.2/jetson_examples.egg-info/SOURCES.txt
--rw-r--r--   0 zhixin.luo   (501) staff       (20)        1 2024-04-12 11:18:31.000000 jetson-examples-0.0.2/jetson_examples.egg-info/dependency_links.txt
--rw-r--r--   0 zhixin.luo   (501) staff       (20)       58 2024-04-12 11:18:31.000000 jetson-examples-0.0.2/jetson_examples.egg-info/entry_points.txt
--rw-r--r--   0 zhixin.luo   (501) staff       (20)       11 2024-04-12 11:18:31.000000 jetson-examples-0.0.2/jetson_examples.egg-info/top_level.txt
--rw-r--r--   0 zhixin.luo   (501) staff       (20)      578 2024-04-12 11:18:27.000000 jetson-examples-0.0.2/pyproject.toml
-drwxr-xr-x   0 zhixin.luo   (501) staff       (20)        0 2024-04-12 11:18:31.955295 jetson-examples-0.0.2/reComputer/
--rw-r--r--   0 zhixin.luo   (501) staff       (20)        0 2024-04-12 06:30:15.000000 jetson-examples-0.0.2/reComputer/__init__.py
--rw-r--r--   0 zhixin.luo   (501) staff       (20)     1109 2024-04-12 08:52:44.000000 jetson-examples-0.0.2/reComputer/main.py
-drwxr-xr-x   0 zhixin.luo   (501) staff       (20)        0 2024-04-12 11:18:31.955541 jetson-examples-0.0.2/scripts/
--rw-r--r--   0 zhixin.luo   (501) staff       (20)     5617 2024-04-12 09:08:57.000000 jetson-examples-0.0.2/scripts/run.sh
--rw-r--r--   0 zhixin.luo   (501) staff       (20)       38 2024-04-12 11:18:31.956298 jetson-examples-0.0.2/setup.cfg
--rw-r--r--   0 zhixin.luo   (501) staff       (20)      284 2024-04-12 06:30:15.000000 jetson-examples-0.0.2/setup.py
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-04-15 10:08:34.277466 jetson_examples-0.0.3/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1066 2024-04-15 02:07:20.000000 jetson_examples-0.0.3/LICENSE
+-rw-r--r--   0 youjiang  (1000) youjiang  (1000)     2751 2024-04-15 10:08:34.277466 jetson_examples-0.0.3/PKG-INFO
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     2209 2024-04-15 02:07:20.000000 jetson_examples-0.0.3/README.md
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-04-15 10:08:34.277466 jetson_examples-0.0.3/jetson_examples.egg-info/
+-rw-r--r--   0 youjiang  (1000) youjiang  (1000)     2751 2024-04-15 10:08:34.000000 jetson_examples-0.0.3/jetson_examples.egg-info/PKG-INFO
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      296 2024-04-15 10:08:34.000000 jetson_examples-0.0.3/jetson_examples.egg-info/SOURCES.txt
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)        1 2024-04-15 10:08:34.000000 jetson_examples-0.0.3/jetson_examples.egg-info/dependency_links.txt
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       58 2024-04-15 10:08:34.000000 jetson_examples-0.0.3/jetson_examples.egg-info/entry_points.txt
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       11 2024-04-15 10:08:34.000000 jetson_examples-0.0.3/jetson_examples.egg-info/top_level.txt
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      578 2024-04-15 10:08:18.000000 jetson_examples-0.0.3/pyproject.toml
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-04-15 10:08:34.277466 jetson_examples-0.0.3/reComputer/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)        0 2024-04-15 02:07:20.000000 jetson_examples-0.0.3/reComputer/__init__.py
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1109 2024-04-15 02:07:20.000000 jetson_examples-0.0.3/reComputer/main.py
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-04-15 10:08:34.277466 jetson_examples-0.0.3/scripts/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)    16260 2024-04-15 10:05:13.000000 jetson_examples-0.0.3/scripts/run.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       38 2024-04-15 10:08:34.277466 jetson_examples-0.0.3/setup.cfg
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      284 2024-04-15 09:54:35.000000 jetson_examples-0.0.3/setup.py
```

### Comparing `jetson-examples-0.0.2/LICENSE` & `jetson_examples-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jetson-examples-0.0.2/PKG-INFO` & `jetson_examples-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetson-examples
-Version: 0.0.2
+Version: 0.0.3
 Summary: run AI on Jetson, all you need is reComputer
 Author-email: luozhixin <zhixin.luo@seeed.cc>
 Project-URL: Homepage, https://github.com/Seeed-Projects/jetson-examples
 Project-URL: Issues, https://github.com/Seeed-Projects/jetson-examples/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jetson-examples-0.0.2/README.md` & `jetson_examples-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `jetson-examples-0.0.2/jetson_examples.egg-info/PKG-INFO` & `jetson_examples-0.0.3/jetson_examples.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetson-examples
-Version: 0.0.2
+Version: 0.0.3
 Summary: run AI on Jetson, all you need is reComputer
 Author-email: luozhixin <zhixin.luo@seeed.cc>
 Project-URL: Homepage, https://github.com/Seeed-Projects/jetson-examples
 Project-URL: Issues, https://github.com/Seeed-Projects/jetson-examples/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jetson-examples-0.0.2/pyproject.toml` & `jetson_examples-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jetson-examples"
-version = "0.0.2"
+version = "0.0.3"
 authors = [{ name = "luozhixin", email = "zhixin.luo@seeed.cc" }]
 description = "run AI on Jetson, all you need is reComputer"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `jetson-examples-0.0.2/reComputer/main.py` & `jetson_examples-0.0.3/reComputer/main.py`

 * *Files identical despite different names*

