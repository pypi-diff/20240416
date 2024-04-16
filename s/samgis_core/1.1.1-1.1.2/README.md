# Comparing `tmp/samgis_core-1.1.1.tar.gz` & `tmp/samgis_core-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samgis_core-1.1.1.tar", max compression
+gzip compressed data, was "samgis_core-1.1.2.tar", max compression
```

## Comparing `samgis_core-1.1.1.tar` & `samgis_core-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      262 2024-01-27 16:18:49.002975 samgis_core-1.1.1/README.md
--rw-r--r--   0        0        0      632 2024-04-16 15:50:41.347379 samgis_core-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      351 2024-01-31 18:31:46.678851 samgis_core-1.1.1/samgis_core/__init__.py
--rw-r--r--   0        0        0       94 2024-04-15 09:18:13.959941 samgis_core-1.1.1/samgis_core/__version__.py
--rw-r--r--   0        0        0       57 2024-01-26 19:56:25.000000 samgis_core-1.1.1/samgis_core/prediction_api/__init__.py
--rw-r--r--   0        0        0    15324 2024-04-16 14:31:35.337069 samgis_core-1.1.1/samgis_core/prediction_api/sam_onnx.py
--rw-r--r--   0        0        0       32 2024-01-26 19:56:25.000000 samgis_core-1.1.1/samgis_core/utilities/__init__.py
--rw-r--r--   0        0        0      157 2024-01-27 14:15:17.000000 samgis_core-1.1.1/samgis_core/utilities/constants.py
--rw-r--r--   0        0        0      650 2024-04-15 21:25:49.690475 samgis_core-1.1.1/samgis_core/utilities/fastapi_logger.py
--rw-r--r--   0        0        0     2749 2024-01-26 20:33:06.000000 samgis_core-1.1.1/samgis_core/utilities/serialize.py
--rw-r--r--   0        0        0      659 2024-04-16 13:20:43.686978 samgis_core-1.1.1/samgis_core/utilities/type_hints.py
--rw-r--r--   0        0        0     2434 2024-01-27 14:15:17.000000 samgis_core-1.1.1/samgis_core/utilities/utilities.py
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 samgis_core-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      262 2024-01-27 16:18:49.002975 samgis_core-1.1.2/README.md
+-rw-r--r--   0        0        0      632 2024-04-16 19:06:29.883454 samgis_core-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      351 2024-01-31 18:31:46.678851 samgis_core-1.1.2/samgis_core/__init__.py
+-rw-r--r--   0        0        0       94 2024-04-15 09:18:13.959941 samgis_core-1.1.2/samgis_core/__version__.py
+-rw-r--r--   0        0        0       57 2024-01-26 19:56:25.000000 samgis_core-1.1.2/samgis_core/prediction_api/__init__.py
+-rw-r--r--   0        0        0    15320 2024-04-16 18:51:41.442736 samgis_core-1.1.2/samgis_core/prediction_api/sam_onnx.py
+-rw-r--r--   0        0        0       32 2024-01-26 19:56:25.000000 samgis_core-1.1.2/samgis_core/utilities/__init__.py
+-rw-r--r--   0        0        0      157 2024-01-27 14:15:17.000000 samgis_core-1.1.2/samgis_core/utilities/constants.py
+-rw-r--r--   0        0        0      650 2024-04-15 21:25:49.690475 samgis_core-1.1.2/samgis_core/utilities/fastapi_logger.py
+-rw-r--r--   0        0        0     2689 2024-04-16 18:49:10.489577 samgis_core-1.1.2/samgis_core/utilities/serialize.py
+-rw-r--r--   0        0        0      845 2024-04-16 18:51:41.468695 samgis_core-1.1.2/samgis_core/utilities/type_hints.py
+-rw-r--r--   0        0        0     2434 2024-01-27 14:15:17.000000 samgis_core-1.1.2/samgis_core/utilities/utilities.py
+-rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 samgis_core-1.1.2/PKG-INFO
```

### Comparing `samgis_core-1.1.1/pyproject.toml` & `samgis_core-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "samgis_core"
-version = "1.1.1"
+version = "1.1.2"
 description = "SamGIS CORE"
 authors = ["alessandro trinca tornidor <alessandro@trinca.tornidor.com>"]
 license = "MIT license"
 readme = "README.md"
 
 [metadata]
 name = "samgis_core"
-version = "1.1.1"
+version = "1.1.2"
 
 [tool.poetry.dependencies]
 numpy = "1.25.2"
 pillow = "^10.2.0"
 python = "~3.10"
 onnxruntime = "1.16.3"
 opencv-python-headless = "4.8.1.78"
```

### Comparing `samgis_core-1.1.1/samgis_core/prediction_api/sam_onnx.py` & `samgis_core-1.1.2/samgis_core/prediction_api/sam_onnx.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from cv2 import INTER_LINEAR, warpAffine
 from numpy import array as np_array, uint8, zeros, ndarray
 from numpy import concatenate, float32, linalg, matmul, ones
 from onnxruntime import get_available_providers, InferenceSession
 
 from samgis_core import app_logger, MODEL_FOLDER
 from samgis_core.utilities.constants import DEFAULT_INPUT_SHAPE, MODEL_ENCODER_NAME, MODEL_DECODER_NAME
-from samgis_core.utilities.type_hints import PIL_Image, list_dict, tuple_ndarr_int, EmbeddingDict, EmbeddingImage
+from samgis_core.utilities.type_hints import PIL_Image, ListDict, TupleNdarrayInt, EmbeddingDict, EmbeddingImage
 
 
 class SegmentAnythingONNX:
     """Segmentation model using SegmentAnything"""
 
     def __init__(self, encoder_model_path, decoder_model_path) -> None:
         self.target_size = DEFAULT_INPUT_SHAPE[1]
@@ -253,16 +253,16 @@
             prompt,
         )
 
         return masks
 
 
 def get_raster_inference(
-        img: PIL_Image or ndarray, prompt: list_dict, models_instance: SegmentAnythingONNX, model_name: str
-) -> tuple_ndarr_int:
+        img: PIL_Image or ndarray, prompt: ListDict, models_instance: SegmentAnythingONNX, model_name: str
+) -> TupleNdarrayInt:
     """
     Get inference output for a given image using a SegmentAnythingONNX model
 
     Args:
         img: input PIL Image
         prompt: list of prompt dict
         models_instance: SegmentAnythingONNX instance model
@@ -314,15 +314,15 @@
                         f"DECODER {MODEL_DECODER_NAME} from {MODEL_FOLDER}: Creating embedding...")
         embedding = models_instance.encode(np_img)
         embedding_dict[embedding_key] = embedding
     return embedding_dict
 
 
 def get_raster_inference_using_existing_embedding(
-        embedding: dict, prompt: list_dict, models_instance: SegmentAnythingONNX) -> tuple_ndarr_int:
+        embedding: dict, prompt: ListDict, models_instance: SegmentAnythingONNX) -> TupleNdarrayInt:
     """
     Get inference output for a given image using a SegmentAnythingONNX model, using an existing embedding instead of a
     new ndarray or PIL image
 
     Args:
         embedding: dict
         prompt: list of prompt dict
@@ -341,16 +341,16 @@
         app_logger.debug(f"{n}th of prediction_masks shape {inference_out.shape}"
                          f" => mask shape:{mask.shape}, {mask.dtype}.")
         mask[m > 0.0] = 255
     return mask, len_inference_out
 
 
 def get_raster_inference_with_embedding_from_dict(
-        img: PIL_Image or ndarray, prompt: list_dict, models_instance: SegmentAnythingONNX, model_name: str,
-        embedding_key: str, embedding_dict: dict) -> tuple_ndarr_int:
+        img: PIL_Image or ndarray, prompt: ListDict, models_instance: SegmentAnythingONNX, model_name: str,
+        embedding_key: str, embedding_dict: dict) -> TupleNdarrayInt:
     """
     Get inference output using a SegmentAnythingONNX model, but get the image embedding from the given embedding dict
      instead of creating a new embedding. This function needs the img argument to update the embedding dict if necessary
 
     Args:
         img: input PIL Image
         prompt: list of prompt dict
```

### Comparing `samgis_core-1.1.1/samgis_core/utilities/fastapi_logger.py` & `samgis_core-1.1.2/samgis_core/utilities/fastapi_logger.py`

 * *Files identical despite different names*

### Comparing `samgis_core-1.1.1/samgis_core/utilities/serialize.py` & `samgis_core-1.1.2/samgis_core/utilities/serialize.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Serialize objects"""
 from typing import Mapping
 
 from samgis_core import app_logger
-from samgis_core.utilities.type_hints import dict_str, dict_str_any
 
 
 def serialize(obj: any, include_none: bool = False):
     """
     Return the input object into a serializable one
 
     Args:
@@ -70,15 +69,15 @@
     return res
 
 
 def _serialize_list(ls: list, include_none: bool) -> list:
     return [_serialize(elem, include_none) for elem in ls]
 
 
-def _serialize_bytes(b: bytes) -> dict_str:
+def _serialize_bytes(b: bytes) -> dict[str, str]:
     import base64
     encoded = base64.b64encode(b)
     return {"value": encoded.decode('ascii'), "type": "bytes"}
 
 
-def _serialize_exception(e: Exception) -> dict_str_any:
+def _serialize_exception(e: Exception) -> dict[str, str]:
     return {"msg": str(e), "type": str(type(e)), **e.__dict__}
```

### Comparing `samgis_core-1.1.1/samgis_core/utilities/utilities.py` & `samgis_core-1.1.2/samgis_core/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `samgis_core-1.1.1/PKG-INFO` & `samgis_core-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samgis_core
-Version: 1.1.1
+Version: 1.1.2
 Summary: SamGIS CORE
 License: MIT
 Author: alessandro trinca tornidor
 Author-email: alessandro@trinca.tornidor.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

