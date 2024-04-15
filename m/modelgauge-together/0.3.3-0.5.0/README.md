# Comparing `tmp/modelgauge_together-0.3.3.tar.gz` & `tmp/modelgauge_together-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelgauge_together-0.3.3.tar", max compression
+gzip compressed data, was "modelgauge_together-0.5.0.tar", max compression
```

## Comparing `modelgauge_together-0.3.3.tar` & `modelgauge_together-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       49 2024-04-10 19:55:36.527596 modelgauge_together-0.3.3/README.md
--rw-r--r--   0        0        0     7543 2024-04-11 19:47:59.729737 modelgauge_together-0.3.3/modelgauge/annotators/__pycache__/llama_guard_annotator.cpython-310.pyc
--rw-r--r--   0        0        0     7741 2024-04-11 19:30:18.217705 modelgauge_together-0.3.3/modelgauge/annotators/llama_guard_annotator.py
--rw-r--r--   0        0        0     1099 2024-04-11 19:48:00.798737 modelgauge_together-0.3.3/modelgauge/suts/__pycache__/together_cli.cpython-310.pyc
--rw-r--r--   0        0        0    12635 2024-04-11 19:47:59.665737 modelgauge_together-0.3.3/modelgauge/suts/__pycache__/together_client.cpython-310.pyc
--rw-r--r--   0        0        0     1132 2024-04-11 19:30:18.218705 modelgauge_together-0.3.3/modelgauge/suts/together_cli.py
--rw-r--r--   0        0        0    12718 2024-04-11 19:30:18.218705 modelgauge_together-0.3.3/modelgauge/suts/together_client.py
--rw-r--r--   0        0        0      397 2024-04-11 19:30:18.218705 modelgauge_together-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 modelgauge_together-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0       49 2024-04-10 19:55:36.527596 modelgauge_together-0.5.0/README.md
+-rw-r--r--   0        0        0     7543 2024-04-11 19:47:59.729737 modelgauge_together-0.5.0/modelgauge/annotators/__pycache__/llama_guard_annotator.cpython-310.pyc
+-rw-r--r--   0        0        0     7741 2024-04-11 19:30:18.217705 modelgauge_together-0.5.0/modelgauge/annotators/llama_guard_annotator.py
+-rw-r--r--   0        0        0     1099 2024-04-11 19:48:00.798737 modelgauge_together-0.5.0/modelgauge/suts/__pycache__/together_cli.cpython-310.pyc
+-rw-r--r--   0        0        0    12635 2024-04-11 19:47:59.665737 modelgauge_together-0.5.0/modelgauge/suts/__pycache__/together_client.cpython-310.pyc
+-rw-r--r--   0        0        0     1132 2024-04-11 19:30:18.218705 modelgauge_together-0.5.0/modelgauge/suts/together_cli.py
+-rw-r--r--   0        0        0    12718 2024-04-11 19:30:18.218705 modelgauge_together-0.5.0/modelgauge/suts/together_client.py
+-rw-r--r--   0        0        0      397 2024-04-15 22:05:52.198001 modelgauge_together-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 modelgauge_together-0.5.0/PKG-INFO
```

### Comparing `modelgauge_together-0.3.3/modelgauge/annotators/__pycache__/llama_guard_annotator.cpython-310.pyc` & `modelgauge_together-0.5.0/modelgauge/annotators/__pycache__/llama_guard_annotator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `modelgauge_together-0.3.3/modelgauge/annotators/llama_guard_annotator.py` & `modelgauge_together-0.5.0/modelgauge/annotators/llama_guard_annotator.py`

 * *Files identical despite different names*

### Comparing `modelgauge_together-0.3.3/modelgauge/suts/__pycache__/together_cli.cpython-310.pyc` & `modelgauge_together-0.5.0/modelgauge/suts/__pycache__/together_cli.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `modelgauge_together-0.3.3/modelgauge/suts/__pycache__/together_client.cpython-310.pyc` & `modelgauge_together-0.5.0/modelgauge/suts/__pycache__/together_client.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `modelgauge_together-0.3.3/modelgauge/suts/together_cli.py` & `modelgauge_together-0.5.0/modelgauge/suts/together_cli.py`

 * *Files identical despite different names*

### Comparing `modelgauge_together-0.3.3/modelgauge/suts/together_client.py` & `modelgauge_together-0.5.0/modelgauge/suts/together_client.py`

 * *Files identical despite different names*

### Comparing `modelgauge_together-0.3.3/PKG-INFO` & `modelgauge_together-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelgauge-together
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

