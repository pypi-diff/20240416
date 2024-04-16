# Comparing `tmp/freeplay-0.3.0a5.tar.gz` & `tmp/freeplay-0.3.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeplay-0.3.0a5.tar", max compression
+gzip compressed data, was "freeplay-0.3.0a6.tar", max compression
```

## Comparing `freeplay-0.3.0a5.tar` & `freeplay-0.3.0a6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1064 2024-01-03 16:29:40.447184 freeplay-0.3.0a5/LICENSE
--rw-r--r--   0        0        0      884 2024-01-18 21:16:28.148908 freeplay-0.3.0a5/README.md
--rw-r--r--   0        0        0      679 2024-04-02 19:40:56.828622 freeplay-0.3.0a5/pyproject.toml
--rw-r--r--   0        0        0      346 2024-03-21 16:21:06.233651 freeplay-0.3.0a5/src/freeplay/__init__.py
--rw-r--r--   0        0        0     2331 2024-03-13 23:06:12.228513 freeplay-0.3.0a5/src/freeplay/api_support.py
--rw-r--r--   0        0        0      631 2024-01-03 16:29:40.448185 freeplay-0.3.0a5/src/freeplay/errors.py
--rw-r--r--   0        0        0     1479 2024-03-21 16:21:06.234127 freeplay-0.3.0a5/src/freeplay/freeplay.py
--rw-r--r--   0        0        0     3460 2024-03-21 16:21:06.234580 freeplay-0.3.0a5/src/freeplay/freeplay_cli.py
--rw-r--r--   0        0        0      898 2024-01-03 16:29:40.448980 freeplay-0.3.0a5/src/freeplay/llm_parameters.py
--rw-r--r--   0        0        0      384 2024-03-21 16:21:06.234863 freeplay-0.3.0a5/src/freeplay/model.py
--rw-r--r--   0        0        0        0 2024-03-29 20:43:25.126491 freeplay-0.3.0a5/src/freeplay/py.typed
--rw-r--r--   0        0        0        0 2024-03-21 16:21:06.234949 freeplay-0.3.0a5/src/freeplay/resources/__init__.py
--rw-r--r--   0        0        0      527 2024-03-21 16:21:06.235095 freeplay-0.3.0a5/src/freeplay/resources/customer_feedback.py
--rw-r--r--   0        0        0    12400 2024-04-02 19:40:41.570999 freeplay-0.3.0a5/src/freeplay/resources/prompts.py
--rw-r--r--   0        0        0     5412 2024-03-29 20:43:16.999199 freeplay-0.3.0a5/src/freeplay/resources/recordings.py
--rw-r--r--   0        0        0      868 2024-03-21 16:21:06.235825 freeplay-0.3.0a5/src/freeplay/resources/sessions.py
--rw-r--r--   0        0        0     1452 2024-03-21 16:21:06.236038 freeplay-0.3.0a5/src/freeplay/resources/test_runs.py
--rw-r--r--   0        0        0     4532 2024-03-21 16:21:06.236528 freeplay-0.3.0a5/src/freeplay/support.py
--rw-r--r--   0        0        0     2064 2024-03-21 16:21:06.236895 freeplay-0.3.0a5/src/freeplay/utils.py
--rw-r--r--   0        0        0     1604 1970-01-01 00:00:00.000000 freeplay-0.3.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-01-12 20:28:56.461587 freeplay-0.3.0a6/LICENSE
+-rw-r--r--   0        0        0      884 2024-01-30 20:26:04.166910 freeplay-0.3.0a6/README.md
+-rw-r--r--   0        0        0      679 2024-04-16 19:45:25.765844 freeplay-0.3.0a6/pyproject.toml
+-rw-r--r--   0        0        0      346 2024-03-25 14:26:20.961664 freeplay-0.3.0a6/src/freeplay/__init__.py
+-rw-r--r--   0        0        0     2331 2024-03-14 18:04:56.167739 freeplay-0.3.0a6/src/freeplay/api_support.py
+-rw-r--r--   0        0        0      631 2024-01-12 20:28:56.463431 freeplay-0.3.0a6/src/freeplay/errors.py
+-rw-r--r--   0        0        0     1479 2024-03-25 14:26:20.962106 freeplay-0.3.0a6/src/freeplay/freeplay.py
+-rw-r--r--   0        0        0     3460 2024-03-25 14:26:20.962659 freeplay-0.3.0a6/src/freeplay/freeplay_cli.py
+-rw-r--r--   0        0        0      898 2024-01-12 20:28:56.464517 freeplay-0.3.0a6/src/freeplay/llm_parameters.py
+-rw-r--r--   0        0        0      384 2024-03-25 14:26:20.963123 freeplay-0.3.0a6/src/freeplay/model.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:02:09.446684 freeplay-0.3.0a6/src/freeplay/py.typed
+-rw-r--r--   0        0        0        0 2024-03-25 14:26:20.963202 freeplay-0.3.0a6/src/freeplay/resources/__init__.py
+-rw-r--r--   0        0        0      527 2024-03-25 14:26:20.963455 freeplay-0.3.0a6/src/freeplay/resources/customer_feedback.py
+-rw-r--r--   0        0        0    12400 2024-04-16 19:02:09.447259 freeplay-0.3.0a6/src/freeplay/resources/prompts.py
+-rw-r--r--   0        0        0     5412 2024-04-16 19:02:09.447779 freeplay-0.3.0a6/src/freeplay/resources/recordings.py
+-rw-r--r--   0        0        0      868 2024-03-25 14:26:20.963849 freeplay-0.3.0a6/src/freeplay/resources/sessions.py
+-rw-r--r--   0        0        0     1452 2024-03-25 14:26:20.963926 freeplay-0.3.0a6/src/freeplay/resources/test_runs.py
+-rw-r--r--   0        0        0     4532 2024-03-25 14:26:20.964330 freeplay-0.3.0a6/src/freeplay/support.py
+-rw-r--r--   0        0        0     2064 2024-03-25 14:26:20.964602 freeplay-0.3.0a6/src/freeplay/utils.py
+-rw-r--r--   0        0        0     1553 1970-01-01 00:00:00.000000 freeplay-0.3.0a6/PKG-INFO
```

### Comparing `freeplay-0.3.0a5/LICENSE` & `freeplay-0.3.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a5/README.md` & `freeplay-0.3.0a6/README.md`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a5/pyproject.toml` & `freeplay-0.3.0a6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "freeplay"
-version = "0.3.0-alpha.5"
+version = "0.3.0-alpha.6"
 description = ""
 authors = ["FreePlay Engineering <engineering@freeplay.ai>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <4"
```

### Comparing `freeplay-0.3.0a5/src/freeplay/api_support.py` & `freeplay-0.3.0a6/src/freeplay/api_support.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a5/src/freeplay/errors.py` & `freeplay-0.3.0a6/src/freeplay/errors.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a5/src/freeplay/freeplay.py` & `freeplay-0.3.0a6/src/freeplay/freeplay.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a5/src/freeplay/freeplay_cli.py` & `freeplay-0.3.0a6/src/freeplay/freeplay_cli.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a5/src/freeplay/llm_parameters.py` & `freeplay-0.3.0a6/src/freeplay/llm_parameters.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a5/src/freeplay/resources/customer_feedback.py` & `freeplay-0.3.0a6/src/freeplay/resources/customer_feedback.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a5/src/freeplay/resources/prompts.py` & `freeplay-0.3.0a6/src/freeplay/resources/prompts.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a5/src/freeplay/resources/recordings.py` & `freeplay-0.3.0a6/src/freeplay/resources/recordings.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a5/src/freeplay/resources/sessions.py` & `freeplay-0.3.0a6/src/freeplay/resources/sessions.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a5/src/freeplay/resources/test_runs.py` & `freeplay-0.3.0a6/src/freeplay/resources/test_runs.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a5/src/freeplay/support.py` & `freeplay-0.3.0a6/src/freeplay/support.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a5/src/freeplay/utils.py` & `freeplay-0.3.0a6/src/freeplay/utils.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.3.0a5/PKG-INFO` & `freeplay-0.3.0a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: freeplay
-Version: 0.3.0a5
+Version: 0.3.0a6
 Summary: 
 License: MIT
 Author: FreePlay Engineering
 Author-email: engineering@freeplay.ai
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (==8.1.7)
 Requires-Dist: dacite (>=1.8.0,<2.0.0)
 Requires-Dist: pystache (>=0.6.5,<0.7.0)
 Requires-Dist: requests (>=2.20.0,<3.0.0dev)
 Description-Content-Type: text/markdown
 
 # Freeplay Python SDK
```

