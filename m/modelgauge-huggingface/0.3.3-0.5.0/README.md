# Comparing `tmp/modelgauge_huggingface-0.3.3.tar.gz` & `tmp/modelgauge_huggingface-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelgauge_huggingface-0.3.3.tar", max compression
+gzip compressed data, was "modelgauge_huggingface-0.5.0.tar", max compression
```

## Comparing `modelgauge_huggingface-0.3.3.tar` & `modelgauge_huggingface-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       41 2024-04-10 19:55:36.522596 modelgauge_huggingface-0.3.3/README.md
--rw-r--r--   0        0        0    12709 2024-04-11 19:47:59.782737 modelgauge_huggingface-0.3.3/modelgauge/suts/__pycache__/huggingface_client.cpython-310.pyc
--rw-r--r--   0        0        0    18618 2024-04-11 19:30:18.214705 modelgauge_huggingface-0.3.3/modelgauge/suts/huggingface_client.py
--rw-r--r--   0        0        0      385 2024-04-11 19:30:18.215705 modelgauge_huggingface-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 modelgauge_huggingface-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0       41 2024-04-10 19:55:36.522596 modelgauge_huggingface-0.5.0/README.md
+-rw-r--r--   0        0        0    12709 2024-04-11 19:47:59.782737 modelgauge_huggingface-0.5.0/modelgauge/suts/__pycache__/huggingface_client.cpython-310.pyc
+-rw-r--r--   0        0        0    18618 2024-04-11 19:30:18.214705 modelgauge_huggingface-0.5.0/modelgauge/suts/huggingface_client.py
+-rw-r--r--   0        0        0      385 2024-04-15 22:05:52.197002 modelgauge_huggingface-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 modelgauge_huggingface-0.5.0/PKG-INFO
```

### Comparing `modelgauge_huggingface-0.3.3/modelgauge/suts/__pycache__/huggingface_client.cpython-310.pyc` & `modelgauge_huggingface-0.5.0/modelgauge/suts/__pycache__/huggingface_client.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `modelgauge_huggingface-0.3.3/modelgauge/suts/huggingface_client.py` & `modelgauge_huggingface-0.5.0/modelgauge/suts/huggingface_client.py`

 * *Files identical despite different names*

### Comparing `modelgauge_huggingface-0.3.3/PKG-INFO` & `modelgauge_huggingface-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelgauge-huggingface
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

