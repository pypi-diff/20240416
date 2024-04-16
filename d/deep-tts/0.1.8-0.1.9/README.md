# Comparing `tmp/deep_tts-0.1.8.tar.gz` & `tmp/deep_tts-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_tts-0.1.8.tar", max compression
+gzip compressed data, was "deep_tts-0.1.9.tar", max compression
```

## Comparing `deep_tts-0.1.8.tar` & `deep_tts-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0      627 2024-03-25 08:32:50.119841 deep_tts-0.1.8/README.md
--rw-r--r--   0        0        0      115 2024-03-22 15:33:43.579957 deep_tts-0.1.8/deep_tts/__init__.py
--rw-r--r--   0        0        0     3057 2024-03-25 08:32:33.580967 deep_tts-0.1.8/deep_tts/common.py
--rw-r--r--   0        0        0      923 2024-03-25 08:31:52.367737 deep_tts-0.1.8/deep_tts/data_models.py
--rw-r--r--   0        0        0        0 2024-03-25 07:49:15.094901 deep_tts-0.1.8/deep_tts/py.typed
--rw-r--r--   0        0        0      495 2024-03-25 08:42:34.027254 deep_tts-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1285 1970-01-01 00:00:00.000000 deep_tts-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      627 2024-03-25 08:32:50.119841 deep_tts-0.1.9/README.md
+-rw-r--r--   0        0        0      115 2024-03-22 15:33:43.579957 deep_tts-0.1.9/deep_tts/__init__.py
+-rw-r--r--   0        0        0     3057 2024-03-25 08:32:33.580967 deep_tts-0.1.9/deep_tts/common.py
+-rw-r--r--   0        0        0      923 2024-03-25 08:31:52.367737 deep_tts-0.1.9/deep_tts/data_models.py
+-rw-r--r--   0        0        0      495 2024-03-25 08:50:19.468786 deep_tts-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1285 1970-01-01 00:00:00.000000 deep_tts-0.1.9/PKG-INFO
```

### Comparing `deep_tts-0.1.8/README.md` & `deep_tts-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `deep_tts-0.1.8/deep_tts/common.py` & `deep_tts-0.1.9/deep_tts/common.py`

 * *Files identical despite different names*

### Comparing `deep_tts-0.1.8/deep_tts/data_models.py` & `deep_tts-0.1.9/deep_tts/data_models.py`

 * *Files identical despite different names*

### Comparing `deep_tts-0.1.8/PKG-INFO` & `deep_tts-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep-tts
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: xfeng
 Author-email: it.support@deepgrain.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

