# Comparing `tmp/modelgauge_openai-0.3.3.tar.gz` & `tmp/modelgauge_openai-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelgauge_openai-0.3.3.tar", max compression
+gzip compressed data, was "modelgauge_openai-0.5.0.tar", max compression
```

## Comparing `modelgauge_openai-0.3.3.tar` & `modelgauge_openai-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       44 2024-04-10 19:55:36.523596 modelgauge_openai-0.3.3/README.md
--rw-r--r--   0        0        0     5400 2024-04-11 19:47:58.811737 modelgauge_openai-0.3.3/modelgauge/annotators/__pycache__/openai_compliance_annotator.cpython-310.pyc
--rw-r--r--   0        0        0     5544 2024-04-11 19:30:18.215705 modelgauge_openai-0.3.3/modelgauge/annotators/openai_compliance_annotator.py
--rw-r--r--   0        0        0     5818 2024-04-11 19:47:58.662737 modelgauge_openai-0.3.3/modelgauge/suts/__pycache__/openai_client.cpython-310.pyc
--rw-r--r--   0        0        0     6051 2024-04-11 19:30:18.215705 modelgauge_openai-0.3.3/modelgauge/suts/openai_client.py
--rw-r--r--   0        0        0      356 2024-04-11 19:30:18.215705 modelgauge_openai-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 modelgauge_openai-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0       44 2024-04-10 19:55:36.523596 modelgauge_openai-0.5.0/README.md
+-rw-r--r--   0        0        0     5400 2024-04-11 19:47:58.811737 modelgauge_openai-0.5.0/modelgauge/annotators/__pycache__/openai_compliance_annotator.cpython-310.pyc
+-rw-r--r--   0        0        0     5544 2024-04-11 19:30:18.215705 modelgauge_openai-0.5.0/modelgauge/annotators/openai_compliance_annotator.py
+-rw-r--r--   0        0        0     5818 2024-04-11 19:47:58.662737 modelgauge_openai-0.5.0/modelgauge/suts/__pycache__/openai_client.cpython-310.pyc
+-rw-r--r--   0        0        0     6051 2024-04-11 19:30:18.215705 modelgauge_openai-0.5.0/modelgauge/suts/openai_client.py
+-rw-r--r--   0        0        0      356 2024-04-15 22:05:52.197002 modelgauge_openai-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 modelgauge_openai-0.5.0/PKG-INFO
```

### Comparing `modelgauge_openai-0.3.3/modelgauge/annotators/__pycache__/openai_compliance_annotator.cpython-310.pyc` & `modelgauge_openai-0.5.0/modelgauge/annotators/__pycache__/openai_compliance_annotator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `modelgauge_openai-0.3.3/modelgauge/annotators/openai_compliance_annotator.py` & `modelgauge_openai-0.5.0/modelgauge/annotators/openai_compliance_annotator.py`

 * *Files identical despite different names*

### Comparing `modelgauge_openai-0.3.3/modelgauge/suts/__pycache__/openai_client.cpython-310.pyc` & `modelgauge_openai-0.5.0/modelgauge/suts/__pycache__/openai_client.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `modelgauge_openai-0.3.3/modelgauge/suts/openai_client.py` & `modelgauge_openai-0.5.0/modelgauge/suts/openai_client.py`

 * *Files identical despite different names*

