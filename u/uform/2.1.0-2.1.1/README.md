# Comparing `tmp/uform-2.1.0.tar.gz` & `tmp/uform-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uform-2.1.0.tar", last modified: Sun Apr 14 00:51:21 2024, max compression
+gzip compressed data, was "uform-2.1.1.tar", last modified: Tue Apr 16 03:56:09 2024, max compression
```

## Comparing `uform-2.1.0.tar` & `uform-2.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:51:21.702597 uform-2.1.0/
--rwxr-xr-x   0 runner    (1001) docker     (127)    11357 2024-04-14 00:51:14.000000 uform-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    27269 2024-04-14 00:51:21.698597 uform-2.1.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    25346 2024-04-14 00:51:14.000000 uform-2.1.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2656 2024-04-14 00:51:14.000000 uform-2.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:51:21.694597 uform-2.1.0/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:51:21.698597 uform-2.1.0/python/uform/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1963 2024-04-14 00:51:14.000000 uform-2.1.0/python/uform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-14 00:51:14.000000 uform-2.1.0/python/uform/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-04-14 00:51:14.000000 uform-2.1.0/python/uform/gen_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-14 00:51:14.000000 uform-2.1.0/python/uform/numpy_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-04-14 00:51:14.000000 uform-2.1.0/python/uform/onnx_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-14 00:51:14.000000 uform-2.1.0/python/uform/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-04-14 00:51:14.000000 uform-2.1.0/python/uform/torch_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-14 00:51:14.000000 uform-2.1.0/python/uform/torch_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:51:21.698597 uform-2.1.0/python/uform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27269 2024-04-14 00:51:21.000000 uform-2.1.0/python/uform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-14 00:51:21.000000 uform-2.1.0/python/uform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 00:51:21.000000 uform-2.1.0/python/uform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-14 00:51:21.000000 uform-2.1.0/python/uform.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-14 00:51:21.000000 uform-2.1.0/python/uform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 00:51:21.000000 uform-2.1.0/python/uform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 00:51:21.702597 uform-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:56:09.698954 uform-2.1.1/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11357 2024-04-16 03:56:05.000000 uform-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    27269 2024-04-16 03:56:09.698954 uform-2.1.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25346 2024-04-16 03:56:05.000000 uform-2.1.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2656 2024-04-16 03:56:05.000000 uform-2.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:56:09.694954 uform-2.1.1/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:56:09.698954 uform-2.1.1/python/uform/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1963 2024-04-16 03:56:05.000000 uform-2.1.1/python/uform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-16 03:56:05.000000 uform-2.1.1/python/uform/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16130 2024-04-16 03:56:05.000000 uform-2.1.1/python/uform/gen_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-16 03:56:05.000000 uform-2.1.1/python/uform/numpy_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-04-16 03:56:05.000000 uform-2.1.1/python/uform/onnx_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-16 03:56:05.000000 uform-2.1.1/python/uform/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-04-16 03:56:05.000000 uform-2.1.1/python/uform/torch_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-16 03:56:05.000000 uform-2.1.1/python/uform/torch_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:56:09.698954 uform-2.1.1/python/uform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27269 2024-04-16 03:56:09.000000 uform-2.1.1/python/uform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-16 03:56:09.000000 uform-2.1.1/python/uform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:56:09.000000 uform-2.1.1/python/uform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 03:56:09.000000 uform-2.1.1/python/uform.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-16 03:56:09.000000 uform-2.1.1/python/uform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 03:56:09.000000 uform-2.1.1/python/uform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 03:56:09.698954 uform-2.1.1/setup.cfg
```

### Comparing `uform-2.1.0/LICENSE` & `uform-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uform-2.1.0/PKG-INFO` & `uform-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uform
-Version: 2.1.0
+Version: 2.1.1
 Summary: Pocket-Sized Multimodal AI for Content Understanding and Generation
 Author-email: Ash Vardanian <ash.vardanian@unum.cloud>, Mikhail Kim <mike.kim@unum.cloud>, Vladimir Orshulevich <vladimir.orshulevich@unum.cloud>
 Maintainer-email: Unum Cloud <info@unum.cloud>
 Project-URL: Homepage, https://github.com/unum-cloud/uform
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: Chinese (Simplified)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: uform Version: 2.1.0 Summary: Pocket-Sized
+Metadata-Version: 2.1 Name: uform Version: 2.1.1 Summary: Pocket-Sized
 Multimodal AI for Content Understanding and Generation Author-email: Ash
 Vardanian
 unum.cloud>, Mikhail Kim
 unum.cloud>, Vladimir Orshulevich
 unum.cloud> Maintainer-email: Unum Cloud
 unum.cloud> Project-URL: Homepage, https://github.com/unum-cloud/uform
 Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
```

### Comparing `uform-2.1.0/README.md` & `uform-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `uform-2.1.0/pyproject.toml` & `uform-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 description = "Pocket-Sized Multimodal AI for Content Understanding and Generation"
 maintainers = [
     {email = "info@unum.cloud", name = "Unum Cloud"},
 ]
 name = "uform"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "2.1.0"
+version = "2.1.1"
 
 [project.scripts]
 uform-chat = "uform.chat:main"
 
 [project.optional-dependencies]
 torch = ["torch>=1.13.1", "torchvision", "transformers>=4.36.2"]
 onnx = ["onnx>=1.15.0", "onnxruntime>=1.17.1", "numpy"]
```

### Comparing `uform-2.1.0/python/uform/__init__.py` & `uform-2.1.1/python/uform/__init__.py`

 * *Files identical despite different names*

### Comparing `uform-2.1.0/python/uform/chat.py` & `uform-2.1.1/python/uform/chat.py`

 * *Files identical despite different names*

### Comparing `uform-2.1.0/python/uform/gen_model.py` & `uform-2.1.1/python/uform/gen_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from transformers.modeling_outputs import CausalLMOutputWithPast
 from transformers.modeling_utils import PreTrainedModel
 from transformers.models.auto.modeling_auto import (AutoModel,
                                                     AutoModelForCausalLM)
 from transformers.processing_utils import ProcessorMixin
 from transformers.tokenization_utils_base import BatchEncoding
 
-from uform.models import VisualEncoder
+from uform.torch_models import VisualEncoder
 
 IMAGENET_MEAN = (0.48145466, 0.4578275, 0.40821073)
 IMAGENET_STD = (0.26862954, 0.26130258, 0.27577711)
 
 
 def convert_to_rgb(image):
     return image.convert("RGB")
```

### Comparing `uform-2.1.0/python/uform/numpy_preprocessor.py` & `uform-2.1.1/python/uform/numpy_preprocessor.py`

 * *Files identical despite different names*

### Comparing `uform-2.1.0/python/uform/onnx_models.py` & `uform-2.1.1/python/uform/onnx_models.py`

 * *Files identical despite different names*

### Comparing `uform-2.1.0/python/uform/preprocessing.py` & `uform-2.1.1/python/uform/preprocessing.py`

 * *Files identical despite different names*

### Comparing `uform-2.1.0/python/uform/torch_models.py` & `uform-2.1.1/python/uform/torch_models.py`

 * *Files identical despite different names*

### Comparing `uform-2.1.0/python/uform/torch_preprocessor.py` & `uform-2.1.1/python/uform/torch_preprocessor.py`

 * *Files identical despite different names*

### Comparing `uform-2.1.0/python/uform.egg-info/PKG-INFO` & `uform-2.1.1/python/uform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uform
-Version: 2.1.0
+Version: 2.1.1
 Summary: Pocket-Sized Multimodal AI for Content Understanding and Generation
 Author-email: Ash Vardanian <ash.vardanian@unum.cloud>, Mikhail Kim <mike.kim@unum.cloud>, Vladimir Orshulevich <vladimir.orshulevich@unum.cloud>
 Maintainer-email: Unum Cloud <info@unum.cloud>
 Project-URL: Homepage, https://github.com/unum-cloud/uform
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: Chinese (Simplified)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: uform Version: 2.1.0 Summary: Pocket-Sized
+Metadata-Version: 2.1 Name: uform Version: 2.1.1 Summary: Pocket-Sized
 Multimodal AI for Content Understanding and Generation Author-email: Ash
 Vardanian
 unum.cloud>, Mikhail Kim
 unum.cloud>, Vladimir Orshulevich
 unum.cloud> Maintainer-email: Unum Cloud
 unum.cloud> Project-URL: Homepage, https://github.com/unum-cloud/uform
 Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
```

