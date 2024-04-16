# Comparing `tmp/gpuwidget-0.1.0.tar.gz` & `tmp/gpuwidget-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpuwidget-0.1.0.tar", last modified: Mon Apr 15 07:22:48 2024, max compression
+gzip compressed data, was "gpuwidget-0.1.1.tar", last modified: Tue Apr 16 08:16:14 2024, max compression
```

## Comparing `gpuwidget-0.1.0.tar` & `gpuwidget-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 panwenbo  (1008) chuangxin  (9999)        0 2024-04-15 07:19:50.000131 gpuwidget-0.1.0/
--rw-r--r--   0 panwenbo  (1008) chuangxin  (9999)     7048 2024-04-15 07:22:48.000000 gpuwidget-0.1.0/LICENSE
--rw-r--r--   0 panwenbo  (1008) chuangxin  (9999)    12056 2024-04-15 07:22:48.000000 gpuwidget-0.1.0/PKG-INFO
--rw-r--r--   0 panwenbo  (1008) chuangxin  (9999)     2921 2024-04-15 07:22:48.000000 gpuwidget-0.1.0/README.md
-drwxr-xr-x   0 panwenbo  (1008) chuangxin  (9999)        0 2024-04-15 07:21:16.000000 gpuwidget-0.1.0/gpuwidget/
--rw-r--r--   0 panwenbo  (1008) chuangxin  (9999)       79 2024-04-15 07:22:48.000000 gpuwidget-0.1.0/gpuwidget/__init__.py
--rw-r--r--   0 panwenbo  (1008) chuangxin  (9999)     1152 2024-04-15 07:22:48.000000 gpuwidget-0.1.0/gpuwidget/core.py
--rw-r--r--   0 panwenbo  (1008) chuangxin  (9999)     8565 2024-04-15 07:22:48.000000 gpuwidget-0.1.0/gpuwidget/widgets.py
-drwxr-xr-x   0 panwenbo  (1008) chuangxin  (9999)        0 2024-04-15 07:21:16.000000 gpuwidget-0.1.0/gpuwidget.egg-info/
--rw-r--r--   0 panwenbo  (1008) chuangxin  (9999)    12056 2024-04-15 07:22:48.000000 gpuwidget-0.1.0/gpuwidget.egg-info/PKG-INFO
--rw-r--r--   0 panwenbo  (1008) chuangxin  (9999)      257 2024-04-15 07:22:48.000000 gpuwidget-0.1.0/gpuwidget.egg-info/SOURCES.txt
--rw-r--r--   0 panwenbo  (1008) chuangxin  (9999)        1 2024-04-15 07:22:48.000000 gpuwidget-0.1.0/gpuwidget.egg-info/dependency_links.txt
--rw-r--r--   0 panwenbo  (1008) chuangxin  (9999)       29 2024-04-15 07:22:48.000000 gpuwidget-0.1.0/gpuwidget.egg-info/requires.txt
--rw-r--r--   0 panwenbo  (1008) chuangxin  (9999)       10 2024-04-15 07:22:48.000000 gpuwidget-0.1.0/gpuwidget.egg-info/top_level.txt
--rw-r--r--   0 panwenbo  (1008) chuangxin  (9999)     1217 2024-04-15 07:22:48.000000 gpuwidget-0.1.0/pyproject.toml
--rw-r--r--   0 panwenbo  (1008) chuangxin  (9999)       38 2024-04-15 07:22:48.000000 gpuwidget-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:16:14.278675 gpuwidget-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-16 08:16:04.000000 gpuwidget-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12081 2024-04-16 08:16:14.278675 gpuwidget-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-16 08:16:04.000000 gpuwidget-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:16:14.274675 gpuwidget-0.1.1/gpuwidget/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-16 08:16:04.000000 gpuwidget-0.1.1/gpuwidget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-16 08:16:04.000000 gpuwidget-0.1.1/gpuwidget/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8565 2024-04-16 08:16:04.000000 gpuwidget-0.1.1/gpuwidget/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:16:14.278675 gpuwidget-0.1.1/gpuwidget.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12081 2024-04-16 08:16:14.000000 gpuwidget-0.1.1/gpuwidget.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-16 08:16:14.000000 gpuwidget-0.1.1/gpuwidget.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:16:14.000000 gpuwidget-0.1.1/gpuwidget.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-16 08:16:14.000000 gpuwidget-0.1.1/gpuwidget.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 08:16:14.000000 gpuwidget-0.1.1/gpuwidget.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-16 08:16:04.000000 gpuwidget-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 08:16:14.278675 gpuwidget-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:16:14.278675 gpuwidget-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-16 08:16:04.000000 gpuwidget-0.1.1/tests/test_core.py
```

### Comparing `gpuwidget-0.1.0/LICENSE` & `gpuwidget-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpuwidget-0.1.0/PKG-INFO` & `gpuwidget-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpuwidget
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Jupyter widget for monitoring NVIDIA GPUs.
 Author-email: Wenbo Pan <pixelwenbo@gmail.com>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
             CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
@@ -127,15 +127,15 @@
         
 Project-URL: homepage, https://github.com/bmpixel/gpuwidget
 Project-URL: repository, https://github.com/bmpixel/gpuwidget
 Project-URL: documentation, https://github.com/bmpixel/gpuwidget#readme
 Keywords: jupyter,gpu,monitoring,widget,nvidia
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gpuwidget-0.1.0/README.md` & `gpuwidget-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gpuwidget-0.1.0/gpuwidget/core.py` & `gpuwidget-0.1.1/gpuwidget/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from IPython.display import clear_output, display
 
 from .widgets import GPUStatsApp
 
 
 def is_notebook():
     try:
-        shell = get_ipython().__class__.__name__
+        shell = get_ipython()
+        print("###", shell)
         if shell == "ZMQInteractiveShell":  # jupyter notebook
             return True
         elif shell == "TerminalInteractiveShell":  # iPython
             return False
         elif shell == "Shell":  # Google Colab
             return True
         else:
```

### Comparing `gpuwidget-0.1.0/gpuwidget/widgets.py` & `gpuwidget-0.1.1/gpuwidget/widgets.py`

 * *Files identical despite different names*

### Comparing `gpuwidget-0.1.0/gpuwidget.egg-info/PKG-INFO` & `gpuwidget-0.1.1/gpuwidget.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpuwidget
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Jupyter widget for monitoring NVIDIA GPUs.
 Author-email: Wenbo Pan <pixelwenbo@gmail.com>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
             CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
@@ -127,15 +127,15 @@
         
 Project-URL: homepage, https://github.com/bmpixel/gpuwidget
 Project-URL: repository, https://github.com/bmpixel/gpuwidget
 Project-URL: documentation, https://github.com/bmpixel/gpuwidget#readme
 Keywords: jupyter,gpu,monitoring,widget,nvidia
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gpuwidget-0.1.0/pyproject.toml` & `gpuwidget-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpuwidget"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Jupyter widget for monitoring NVIDIA GPUs."
 readme = "README.md"
 authors = [
     { name = "Wenbo Pan", email = "pixelwenbo@gmail.com" },
 ]
 license = { file = "LICENSE" }
 keywords = ["jupyter", "gpu", "monitoring", "widget", "nvidia"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
+    "License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

