# Comparing `tmp/reka_api-1.0.5.tar.gz` & `tmp/reka_api-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reka_api-1.0.5.tar", max compression
+gzip compressed data, was "reka_api-1.0.6.tar", max compression
```

## Comparing `reka_api-1.0.5.tar` & `reka_api-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    25738 2024-04-10 10:10:31.982448 reka_api-1.0.5/LICENSE
--rw-r--r--   0        0        0      149 2024-04-10 10:10:31.982448 reka_api-1.0.5/README.md
--rw-r--r--   0        0        0     1125 2024-04-10 10:10:31.986448 reka_api-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      825 2024-04-10 10:10:31.986448 reka_api-1.0.5/src/reka/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 10:10:31.986448 reka_api-1.0.5/src/reka/api/__init__.py
--rw-r--r--   0        0        0     7403 2024-04-10 10:10:31.986448 reka_api-1.0.5/src/reka/api/chat.py
--rw-r--r--   0        0        0     2401 2024-04-10 10:10:31.986448 reka_api-1.0.5/src/reka/api/completion.py
--rw-r--r--   0        0        0     2077 2024-04-10 10:10:31.986448 reka_api-1.0.5/src/reka/api/dataset.py
--rw-r--r--   0        0        0     2223 2024-04-10 10:10:31.986448 reka_api-1.0.5/src/reka/api/driver.py
--rw-r--r--   0        0        0      694 2024-04-10 10:10:31.986448 reka_api-1.0.5/src/reka/api/job.py
--rw-r--r--   0        0        0      373 2024-04-10 10:10:31.986448 reka_api-1.0.5/src/reka/api/models.py
--rw-r--r--   0        0        0     3563 2024-04-10 10:10:31.986448 reka_api-1.0.5/src/reka/api/retrieval.py
--rw-r--r--   0        0        0     1136 2024-04-10 10:10:31.986448 reka_api-1.0.5/src/reka/errors.py
--rw-r--r--   0        0        0        0 2024-04-10 10:10:31.986448 reka_api-1.0.5/src/reka/py.typed
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 reka_api-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    25738 2024-04-16 10:47:55.120851 reka_api-1.0.6/LICENSE
+-rw-r--r--   0        0        0      149 2024-04-16 10:47:55.120851 reka_api-1.0.6/README.md
+-rw-r--r--   0        0        0     1125 2024-04-16 10:47:55.124851 reka_api-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      825 2024-04-16 10:47:55.124851 reka_api-1.0.6/src/reka/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 10:47:55.124851 reka_api-1.0.6/src/reka/api/__init__.py
+-rw-r--r--   0        0        0     7483 2024-04-16 10:47:55.124851 reka_api-1.0.6/src/reka/api/chat.py
+-rw-r--r--   0        0        0     2481 2024-04-16 10:47:55.124851 reka_api-1.0.6/src/reka/api/completion.py
+-rw-r--r--   0        0        0     2077 2024-04-16 10:47:55.124851 reka_api-1.0.6/src/reka/api/dataset.py
+-rw-r--r--   0        0        0     2223 2024-04-16 10:47:55.124851 reka_api-1.0.6/src/reka/api/driver.py
+-rw-r--r--   0        0        0      694 2024-04-16 10:47:55.124851 reka_api-1.0.6/src/reka/api/job.py
+-rw-r--r--   0        0        0      373 2024-04-16 10:47:55.124851 reka_api-1.0.6/src/reka/api/models.py
+-rw-r--r--   0        0        0     3563 2024-04-16 10:47:55.124851 reka_api-1.0.6/src/reka/api/retrieval.py
+-rw-r--r--   0        0        0     1136 2024-04-16 10:47:55.124851 reka_api-1.0.6/src/reka/errors.py
+-rw-r--r--   0        0        0        0 2024-04-16 10:47:55.124851 reka_api-1.0.6/src/reka/py.typed
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 reka_api-1.0.6/PKG-INFO
```

### Comparing `reka_api-1.0.5/LICENSE` & `reka_api-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.5/pyproject.toml` & `reka_api-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reka-api"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
     "Reka Team <contact@reka.ai>",
 ]
 description = "Reka API"
 readme = "README.md"
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `reka_api-1.0.5/src/reka/__init__.py` & `reka_api-1.0.6/src/reka/__init__.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.5/src/reka/api/chat.py` & `reka_api-1.0.6/src/reka/api/chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 def chat(
     human: Optional[str] = None,
     media_url: Optional[str] = None,
     media_filename: Optional[str] = None,
     conversation_history: Optional[List[HumanTurn | ModelTurn]] = None,
     retrieval_dataset: Optional[str] = None,
-    model_name: str = "default",
+    model_name: str = "reka-flash",
     request_output_len: Optional[int] = None,
     temperature: Optional[float] = None,
     random_seed: Optional[int] = None,
     runtime_top_k: Optional[int] = None,
     runtime_top_p: Optional[float] = None,
     frequency_penalty: Optional[float] = None,
     presence_penalty: Optional[float] = None,
@@ -72,15 +72,15 @@
             first turn (when conversation_history is empty). You can also send base64 media in the format data:image/{image_format};base64,{base64_image}
         media_filename: alternative to the `media_url` parameter, the location of a local file.``
         conversation_history: list of dicts, where each dict has a key "type"
             indicating the speaker, either "human" or "model", and a key "text"
             containing the message from the speaker. If not set, will default to
             an empty history. The first turn may also have "media_url" set.
         retrieval_dataset: Previously uploaded dataset to do retrieval on.
-        model_name: Name of model.
+        model_name: Name of model. You can check available models  with `reka.get_models()`. Defaults to flash.
         request_output_len: Completion length in tokens.
         temperature: Softmax temperature, higher is more diverse.
         random_seed: Seed to obtain different results.
         runtime_top_k: Keep only k top tokens when sampling.
         runtime_top_p: Keep only top p quantile when sampling.
         frequency_penalty: Penalize repetitions. 0 means no penalty.
         presence_penalty: Penalize repetitions. 0 means no penalty.
```

### Comparing `reka_api-1.0.5/src/reka/api/completion.py` & `reka_api-1.0.6/src/reka/api/completion.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import List, Optional, cast
 
 import reka.api.driver as driver
 
 
 def completion(
     prompt: str,
-    model_name: str = "default",
+    model_name: str = "reka-flash",
     request_output_len: Optional[int] = None,
     temperature: Optional[float] = None,
     random_seed: Optional[int] = None,
     runtime_top_k: Optional[int] = None,
     runtime_top_p: Optional[float] = None,
     frequency_penalty: Optional[float] = None,
     presence_penalty: Optional[float] = None,
@@ -28,15 +28,15 @@
     result = reka.completion("What is the capital of the UK?")
     print(completion)  # "The capital of the United Kingdom is London. ..."
     ```
 
     Args:
         prompt: string.
 
-        model_name: Name of model.
+        model_name: Name of model. You can check available models  with `reka.get_models()`. Defaults to flash.
         request_output_len: Completion length in tokens.
         temperature: Softmax temperature, higher is more diverse.
         random_seed: Seed to obtain different results.
         runtime_top_k: Keep only k top tokens when sampling.
         runtime_top_p: Keep only top p quantile when sampling.
         frequency_penalty: Penalize repetition. 0 means no penalty.
         presence_penalty: Penalize repetition. 0 means no penalty.
```

### Comparing `reka_api-1.0.5/src/reka/api/dataset.py` & `reka_api-1.0.6/src/reka/api/dataset.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.5/src/reka/api/driver.py` & `reka_api-1.0.6/src/reka/api/driver.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.5/src/reka/api/job.py` & `reka_api-1.0.6/src/reka/api/job.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.5/src/reka/api/retrieval.py` & `reka_api-1.0.6/src/reka/api/retrieval.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.5/src/reka/errors.py` & `reka_api-1.0.6/src/reka/errors.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.5/PKG-INFO` & `reka_api-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reka-api
-Version: 1.0.5
+Version: 1.0.6
 Summary: Reka API
 Home-page: https://reka.ai/
 Author: Reka Team
 Author-email: contact@reka.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

