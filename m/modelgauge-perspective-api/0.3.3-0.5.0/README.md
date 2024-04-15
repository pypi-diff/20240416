# Comparing `tmp/modelgauge_perspective_api-0.3.3.tar.gz` & `tmp/modelgauge_perspective_api-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelgauge_perspective_api-0.3.3.tar", max compression
+gzip compressed data, was "modelgauge_perspective_api-0.5.0.tar", max compression
```

## Comparing `modelgauge_perspective_api-0.3.3.tar` & `modelgauge_perspective_api-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       43 2024-04-10 19:55:36.524596 modelgauge_perspective_api-0.3.3/README.md
--rw-r--r--   0        0        0    10678 2024-04-11 19:47:58.854737 modelgauge_perspective_api-0.3.3/modelgauge/annotators/__pycache__/perspective_api.cpython-310.pyc
--rw-r--r--   0        0        0    11672 2024-04-11 19:30:18.215705 modelgauge_perspective_api-0.3.3/modelgauge/annotators/perspective_api.py
--rw-r--r--   0        0        0      393 2024-04-12 18:56:17.756891 modelgauge_perspective_api-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      532 1970-01-01 00:00:00.000000 modelgauge_perspective_api-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0       43 2024-04-10 19:55:36.524596 modelgauge_perspective_api-0.5.0/README.md
+-rw-r--r--   0        0        0    10678 2024-04-11 19:47:58.854737 modelgauge_perspective_api-0.5.0/modelgauge/annotators/__pycache__/perspective_api.cpython-310.pyc
+-rw-r--r--   0        0        0    11672 2024-04-11 19:30:18.215705 modelgauge_perspective_api-0.5.0/modelgauge/annotators/perspective_api.py
+-rw-r--r--   0        0        0      393 2024-04-15 22:05:52.197002 modelgauge_perspective_api-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      532 1970-01-01 00:00:00.000000 modelgauge_perspective_api-0.5.0/PKG-INFO
```

### Comparing `modelgauge_perspective_api-0.3.3/modelgauge/annotators/__pycache__/perspective_api.cpython-310.pyc` & `modelgauge_perspective_api-0.5.0/modelgauge/annotators/__pycache__/perspective_api.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `modelgauge_perspective_api-0.3.3/modelgauge/annotators/perspective_api.py` & `modelgauge_perspective_api-0.5.0/modelgauge/annotators/perspective_api.py`

 * *Files identical despite different names*

### Comparing `modelgauge_perspective_api-0.3.3/PKG-INFO` & `modelgauge_perspective_api-0.5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelgauge-perspective-api
-Version: 0.3.3
+Version: 0.5.0
 Summary: 
 Author: MLCommons AI Safety
 Author-email: ai-safety-engineering@mlcommons.org
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

