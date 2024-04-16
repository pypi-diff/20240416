# Comparing `tmp/vision_agent-0.0.53.tar.gz` & `tmp/vision_agent-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_agent-0.0.53.tar", max compression
+gzip compressed data, was "vision_agent-0.1.1.tar", max compression
```

## Comparing `vision_agent-0.0.53.tar` & `vision_agent-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0    11357 2024-04-15 20:53:19.442906 vision_agent-0.0.53/LICENSE
--rw-r--r--   0        0        0     5035 2024-04-15 20:53:19.442906 vision_agent-0.0.53/README.md
--rw-r--r--   0        0        0     2166 2024-04-15 20:53:20.006911 vision_agent-0.0.53/pyproject.toml
--rw-r--r--   0        0        0      229 2024-04-15 20:53:19.454906 vision_agent-0.0.53/vision_agent/__init__.py
--rw-r--r--   0        0        0      127 2024-04-15 20:53:19.454906 vision_agent-0.0.53/vision_agent/agent/__init__.py
--rw-r--r--   0        0        0      529 2024-04-15 20:53:19.454906 vision_agent-0.0.53/vision_agent/agent/agent.py
--rw-r--r--   0        0        0    11511 2024-04-15 20:53:19.454906 vision_agent-0.0.53/vision_agent/agent/easytool.py
--rw-r--r--   0        0        0     4519 2024-04-15 20:53:19.454906 vision_agent-0.0.53/vision_agent/agent/easytool_prompts.py
--rw-r--r--   0        0        0    10101 2024-04-15 20:53:19.454906 vision_agent-0.0.53/vision_agent/agent/reflexion.py
--rw-r--r--   0        0        0     9342 2024-04-15 20:53:19.454906 vision_agent-0.0.53/vision_agent/agent/reflexion_prompts.py
--rw-r--r--   0        0        0    19765 2024-04-15 20:53:19.458906 vision_agent-0.0.53/vision_agent/agent/vision_agent.py
--rw-r--r--   0        0        0     6567 2024-04-15 20:53:19.458906 vision_agent-0.0.53/vision_agent/agent/vision_agent_prompts.py
--rw-r--r--   0        0        0       46 2024-04-15 20:53:19.458906 vision_agent-0.0.53/vision_agent/data/__init__.py
--rw-r--r--   0        0        0     5122 2024-04-15 20:53:19.458906 vision_agent-0.0.53/vision_agent/data/data.py
--rw-r--r--   0        0        0       75 2024-04-15 20:53:19.458906 vision_agent-0.0.53/vision_agent/emb/__init__.py
--rw-r--r--   0        0        0     1375 2024-04-15 20:53:19.458906 vision_agent-0.0.53/vision_agent/emb/emb.py
--rw-r--r--   0        0        0        0 2024-04-15 20:53:19.458906 vision_agent-0.0.53/vision_agent/fonts/__init__.py
--rw-r--r--   0        0        0  1594400 2024-04-15 20:53:19.466906 vision_agent-0.0.53/vision_agent/fonts/default_font_ch_en.ttf
--rw-r--r--   0        0        0     4786 2024-04-15 20:53:19.466906 vision_agent-0.0.53/vision_agent/image_utils.py
--rw-r--r--   0        0        0       48 2024-04-15 20:53:19.466906 vision_agent-0.0.53/vision_agent/llm/__init__.py
--rw-r--r--   0        0        0     5024 2024-04-15 20:53:19.466906 vision_agent-0.0.53/vision_agent/llm/llm.py
--rw-r--r--   0        0        0       67 2024-04-15 20:53:19.466906 vision_agent-0.0.53/vision_agent/lmm/__init__.py
--rw-r--r--   0        0        0     9535 2024-04-15 20:53:19.466906 vision_agent-0.0.53/vision_agent/lmm/lmm.py
--rw-r--r--   0        0        0      253 2024-04-15 20:53:19.466906 vision_agent-0.0.53/vision_agent/tools/__init__.py
--rw-r--r--   0        0        0     1430 2024-04-15 20:53:19.466906 vision_agent-0.0.53/vision_agent/tools/prompts.py
--rw-r--r--   0        0        0    27045 2024-04-15 20:53:19.466906 vision_agent-0.0.53/vision_agent/tools/tools.py
--rw-r--r--   0        0        0     7476 2024-04-15 20:53:19.466906 vision_agent-0.0.53/vision_agent/tools/video.py
--rw-r--r--   0        0        0     6184 1970-01-01 00:00:00.000000 vision_agent-0.0.53/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-15 23:07:52.039178 vision_agent-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5035 2024-04-15 23:07:52.039178 vision_agent-0.1.1/README.md
+-rw-r--r--   0        0        0     2219 2024-04-15 23:07:52.603175 vision_agent-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      229 2024-04-15 23:07:52.051178 vision_agent-0.1.1/vision_agent/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-15 23:07:52.051178 vision_agent-0.1.1/vision_agent/agent/__init__.py
+-rw-r--r--   0        0        0      529 2024-04-15 23:07:52.051178 vision_agent-0.1.1/vision_agent/agent/agent.py
+-rw-r--r--   0        0        0    11511 2024-04-15 23:07:52.051178 vision_agent-0.1.1/vision_agent/agent/easytool.py
+-rw-r--r--   0        0        0     4519 2024-04-15 23:07:52.051178 vision_agent-0.1.1/vision_agent/agent/easytool_prompts.py
+-rw-r--r--   0        0        0    10101 2024-04-15 23:07:52.051178 vision_agent-0.1.1/vision_agent/agent/reflexion.py
+-rw-r--r--   0        0        0     9342 2024-04-15 23:07:52.051178 vision_agent-0.1.1/vision_agent/agent/reflexion_prompts.py
+-rw-r--r--   0        0        0    19764 2024-04-15 23:07:52.051178 vision_agent-0.1.1/vision_agent/agent/vision_agent.py
+-rw-r--r--   0        0        0     6567 2024-04-15 23:07:52.051178 vision_agent-0.1.1/vision_agent/agent/vision_agent_prompts.py
+-rw-r--r--   0        0        0       46 2024-04-15 23:07:52.051178 vision_agent-0.1.1/vision_agent/data/__init__.py
+-rw-r--r--   0        0        0     5122 2024-04-15 23:07:52.051178 vision_agent-0.1.1/vision_agent/data/data.py
+-rw-r--r--   0        0        0       75 2024-04-15 23:07:52.051178 vision_agent-0.1.1/vision_agent/emb/__init__.py
+-rw-r--r--   0        0        0     1375 2024-04-15 23:07:52.051178 vision_agent-0.1.1/vision_agent/emb/emb.py
+-rw-r--r--   0        0        0        0 2024-04-15 23:07:52.051178 vision_agent-0.1.1/vision_agent/fonts/__init__.py
+-rw-r--r--   0        0        0  1594400 2024-04-15 23:07:52.063178 vision_agent-0.1.1/vision_agent/fonts/default_font_ch_en.ttf
+-rw-r--r--   0        0        0     4786 2024-04-15 23:07:52.063178 vision_agent-0.1.1/vision_agent/image_utils.py
+-rw-r--r--   0        0        0       48 2024-04-15 23:07:52.063178 vision_agent-0.1.1/vision_agent/llm/__init__.py
+-rw-r--r--   0        0        0     5024 2024-04-15 23:07:52.063178 vision_agent-0.1.1/vision_agent/llm/llm.py
+-rw-r--r--   0        0        0       67 2024-04-15 23:07:52.063178 vision_agent-0.1.1/vision_agent/lmm/__init__.py
+-rw-r--r--   0        0        0     9535 2024-04-15 23:07:52.063178 vision_agent-0.1.1/vision_agent/lmm/lmm.py
+-rw-r--r--   0        0        0      253 2024-04-15 23:07:52.063178 vision_agent-0.1.1/vision_agent/tools/__init__.py
+-rw-r--r--   0        0        0     1430 2024-04-15 23:07:52.063178 vision_agent-0.1.1/vision_agent/tools/prompts.py
+-rw-r--r--   0        0        0    25589 2024-04-15 23:07:52.063178 vision_agent-0.1.1/vision_agent/tools/tools.py
+-rw-r--r--   0        0        0     7476 2024-04-15 23:07:52.063178 vision_agent-0.1.1/vision_agent/tools/video.py
+-rw-r--r--   0        0        0     1792 2024-04-15 23:07:52.063178 vision_agent-0.1.1/vision_agent/type_defs.py
+-rw-r--r--   0        0        0     6233 1970-01-01 00:00:00.000000 vision_agent-0.1.1/PKG-INFO
```

### Comparing `vision_agent-0.0.53/LICENSE` & `vision_agent-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.53/README.md` & `vision_agent-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.53/pyproject.toml` & `vision_agent-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vision-agent"
-version = "0.0.53"
+version = "0.1.1"
 description = "Toolset for Vision Agent"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "vision_agent"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
@@ -27,14 +27,15 @@
 torch = "2.1.*"  # 2.2 causes sentence-transformers to seg fault
 sentence-transformers = "2.*"
 openai = "1.*"
 typing_extensions = "4.*"
 moviepy = "1.*"
 opencv-python-headless = "4.*"
 tabulate = "^0.9.0"
+pydantic-settings = "^2.2.1"
 
 [tool.poetry.group.dev.dependencies]
 autoflake = "1.*"
 pytest = "7.*"
 black = ">=23,<25"
 flake8 = "5.*"
 isort = "5.*"
@@ -45,14 +46,15 @@
 data-science-types = "^0.2.23"
 types-tqdm = "^4.65.0.1"
 setuptools = "^68.0.0"
 mkdocs = "^1.5.3"
 mkdocstrings = {extras = ["python"], version = "^0.23.0"}
 mkdocs-material = "^9.4.2"
 types-tabulate = "^0.9.0.20240106"
+scikit-image = "<0.23.1"
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = "INFO"
 log_cli_format = "%(asctime)s [%(levelname)s] %(message)s (%(filename)s:%(lineno)s)"
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
```

### Comparing `vision_agent-0.0.53/vision_agent/agent/agent.py` & `vision_agent-0.1.1/vision_agent/agent/agent.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.53/vision_agent/agent/easytool.py` & `vision_agent-0.1.1/vision_agent/agent/easytool.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.53/vision_agent/agent/easytool_prompts.py` & `vision_agent-0.1.1/vision_agent/agent/easytool_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.53/vision_agent/agent/reflexion.py` & `vision_agent-0.1.1/vision_agent/agent/reflexion.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.53/vision_agent/agent/reflexion_prompts.py` & `vision_agent-0.1.1/vision_agent/agent/reflexion_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.53/vision_agent/agent/vision_agent.py` & `vision_agent-0.1.1/vision_agent/agent/vision_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -472,15 +472,15 @@
             self.log_progress(f"Reflection: {reflection}")
             if parse_reflect(reflection):
                 break
             else:
                 reflections += "\n" + reflection
         # '<END>' is a symbol to indicate the end of the chat, which is useful for streaming logs.
         self.log_progress(
-            f"The Vision Agent has concluded this chat. <ANSWER>{final_answer}</<ANSWER>"
+            f"The Vision Agent has concluded this chat. <ANSWER>{final_answer}</ANSWER>"
         )
 
         if visualize_output:
             visualized_output = all_tool_results[-1]["visualized_output"]
             for image in visualized_output:
                 Image.open(image).show()
```

### Comparing `vision_agent-0.0.53/vision_agent/agent/vision_agent_prompts.py` & `vision_agent-0.1.1/vision_agent/agent/vision_agent_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.53/vision_agent/data/data.py` & `vision_agent-0.1.1/vision_agent/data/data.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.53/vision_agent/emb/emb.py` & `vision_agent-0.1.1/vision_agent/emb/emb.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.53/vision_agent/fonts/default_font_ch_en.ttf` & `vision_agent-0.1.1/vision_agent/fonts/default_font_ch_en.ttf`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.53/vision_agent/image_utils.py` & `vision_agent-0.1.1/vision_agent/image_utils.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.53/vision_agent/llm/llm.py` & `vision_agent-0.1.1/vision_agent/llm/llm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.53/vision_agent/lmm/lmm.py` & `vision_agent-0.1.1/vision_agent/lmm/lmm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.53/vision_agent/tools/prompts.py` & `vision_agent-0.1.1/vision_agent/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.53/vision_agent/tools/tools.py` & `vision_agent-0.1.1/vision_agent/tools/tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,16 +8,19 @@
 import numpy as np
 import requests
 from PIL import Image
 from PIL.Image import Image as ImageType
 
 from vision_agent.image_utils import convert_to_b64, get_image_size
 from vision_agent.tools.video import extract_frames_from_video
+from vision_agent.type_defs import LandingaiAPIKey
 
 _LOGGER = logging.getLogger(__name__)
+_LND_API_KEY = LandingaiAPIKey().api_key
+_LND_API_URL = "https://api.dev.landing.ai/v1/agent"
 
 
 def normalize_bbox(
     bbox: List[Union[int, float]], image_size: Tuple[int, ...]
 ) -> List[float]:
     r"""Normalize the bounding box coordinates to be between 0 and 1."""
     x1, y1, x2, y2 = bbox
@@ -76,16 +79,14 @@
     -------
         >>> import vision_agent as va
         >>> clip = va.tools.CLIP()
         >>> clip("red line, yellow dot", "ct_scan1.jpg"))
         [{"labels": ["red line", "yellow dot"], "scores": [0.98, 0.02]}]
     """
 
-    _ENDPOINT = "https://soi4ewr6fjqqdf5vuss6rrilee0kumxq.lambda-url.us-east-2.on.aws"
-
     name = "clip_"
     description = "'clip_' is a tool that can classify any image given a set of input names or tags. It returns a list of the input names along with their probability scores."
     usage = {
         "required_parameters": [
             {"name": "prompt", "type": "str"},
             {"name": "image", "type": "str"},
         ],
@@ -121,47 +122,31 @@
         """
         image_b64 = convert_to_b64(image)
         data = {
             "prompt": prompt,
             "image": image_b64,
             "tool": "closed_set_image_classification",
         }
-        res = requests.post(
-            self._ENDPOINT,
-            headers={"Content-Type": "application/json"},
-            json=data,
-        )
-        resp_json: Dict[str, Any] = res.json()
-        if (
-            "statusCode" in resp_json and resp_json["statusCode"] != 200
-        ) or "statusCode" not in resp_json:
-            _LOGGER.error(f"Request failed: {resp_json}")
-            raise ValueError(f"Request failed: {resp_json}")
-
-        resp_json["data"]["scores"] = [
-            round(prob, 4) for prob in resp_json["data"]["scores"]
-        ]
-
-        return resp_json["data"]  # type: ignore
+        resp_data = _send_inference_request(data, "tools")
+        resp_data["scores"] = [round(prob, 4) for prob in resp_data["scores"]]
+        return resp_data
 
 
 class ImageCaption(Tool):
     r"""ImageCaption is a tool that can caption an image based on its contents
     or tags.
 
     Example
     -------
         >>> import vision_agent as va
         >>> caption = va.tools.ImageCaption()
         >>> caption("image1.jpg")
         {'text': ['a box of orange and white socks']}
     """
 
-    _ENDPOINT = "https://soi4ewr6fjqqdf5vuss6rrilee0kumxq.lambda-url.us-east-2.on.aws"
-
     name = "image_caption_"
     description = "'image_caption_' is a tool that can caption an image based on its contents or tags. It returns a text describing the image"
     usage = {
         "required_parameters": [
             {"name": "image", "type": "str"},
         ],
         "examples": [
@@ -193,27 +178,15 @@
             A list of dictionaries containing the labels and scores. Each dictionary contains the classification result for an image. E.g. [{"labels": ["red line", "yellow dot"], "scores": [0.98, 0.02]}]
         """
         image_b64 = convert_to_b64(image)
         data = {
             "image": image_b64,
             "tool": "image_captioning",
         }
-        res = requests.post(
-            self._ENDPOINT,
-            headers={"Content-Type": "application/json"},
-            json=data,
-        )
-        resp_json: Dict[str, Any] = res.json()
-        if (
-            "statusCode" in resp_json and resp_json["statusCode"] != 200
-        ) or "statusCode" not in resp_json:
-            _LOGGER.error(f"Request failed: {resp_json}")
-            raise ValueError(f"Request failed: {resp_json}")
-
-        return resp_json["data"]  # type: ignore
+        return _send_inference_request(data, "tools")
 
 
 class GroundingDINO(Tool):
     r"""Grounding DINO is a tool that can detect arbitrary objects with inputs such as
     category names or referring expressions.
 
     Example
@@ -222,16 +195,14 @@
         >>> t = va.tools.GroundingDINO()
         >>> t("red line. yellow dot", "ct_scan1.jpg")
         [{'labels': ['red line', 'yellow dot'],
         'bboxes': [[0.38, 0.15, 0.59, 0.7], [0.48, 0.25, 0.69, 0.71]],
         'scores': [0.98, 0.02]}]
     """
 
-    _ENDPOINT = "https://soi4ewr6fjqqdf5vuss6rrilee0kumxq.lambda-url.us-east-2.on.aws"
-
     name = "grounding_dino_"
     description = "'grounding_dino_' is a tool that can detect arbitrary objects with inputs such as category names or referring expressions. It returns a list of bounding boxes, label names and associated probability scores."
     usage = {
         "required_parameters": [
             {"name": "prompt", "type": "str"},
             {"name": "image", "type": "str"},
         ],
@@ -286,32 +257,21 @@
         image_b64 = convert_to_b64(image)
         request_data = {
             "prompt": prompt,
             "image": image_b64,
             "tool": "visual_grounding",
             "kwargs": {"box_threshold": box_threshold, "iou_threshold": iou_threshold},
         }
-        res = requests.post(
-            self._ENDPOINT,
-            headers={"Content-Type": "application/json"},
-            json=request_data,
-        )
-        resp_json: Dict[str, Any] = res.json()
-        if (
-            "statusCode" in resp_json and resp_json["statusCode"] != 200
-        ) or "statusCode" not in resp_json:
-            _LOGGER.error(f"Request failed: {resp_json}")
-            raise ValueError(f"Request failed: {resp_json}")
-        data: Dict[str, Any] = resp_json["data"]
+        data: Dict[str, Any] = _send_inference_request(request_data, "tools")
         if "bboxes" in data:
             data["bboxes"] = [normalize_bbox(box, image_size) for box in data["bboxes"]]
         if "scores" in data:
             data["scores"] = [round(score, 2) for score in data["scores"]]
         if "labels" in data:
-            data["labels"] = [label for label in data["labels"]]
+            data["labels"] = list(data["labels"])
         data["size"] = (image_size[1], image_size[0])
         return data
 
 
 class GroundingSAM(Tool):
     r"""Grounding SAM is a tool that can detect and segment arbitrary objects with
     inputs such as category names or referring expressions.
@@ -331,16 +291,14 @@
         array([[0, 0, 0, ..., 0, 0, 0],
            [0, 0, 0, ..., 0, 0, 0],
            ...,
            [1, 1, 1, ..., 1, 1, 1],
            [1, 1, 1, ..., 1, 1, 1]], dtype=uint8)]}]
     """
 
-    _ENDPOINT = "https://soi4ewr6fjqqdf5vuss6rrilee0kumxq.lambda-url.us-east-2.on.aws"
-
     name = "grounding_sam_"
     description = "'grounding_sam_' is a tool that can detect arbitrary objects with inputs such as category names or referring expressions. It returns a list of bounding boxes, label names and masks file names and associated probability scores."
     usage = {
         "required_parameters": [
             {"name": "prompt", "type": "str"},
             {"name": "image", "type": "str"},
         ],
@@ -395,26 +353,15 @@
         image_b64 = convert_to_b64(image)
         request_data = {
             "prompt": prompt,
             "image": image_b64,
             "tool": "visual_grounding_segment",
             "kwargs": {"box_threshold": box_threshold, "iou_threshold": iou_threshold},
         }
-        res = requests.post(
-            self._ENDPOINT,
-            headers={"Content-Type": "application/json"},
-            json=request_data,
-        )
-        resp_json: Dict[str, Any] = res.json()
-        if (
-            "statusCode" in resp_json and resp_json["statusCode"] != 200
-        ) or "statusCode" not in resp_json:
-            _LOGGER.error(f"Request failed: {resp_json}")
-            raise ValueError(f"Request failed: {resp_json}")
-        data: Dict[str, Any] = resp_json["data"]
+        data: Dict[str, Any] = _send_inference_request(request_data, "tools")
         ret_pred: Dict[str, List] = {"labels": [], "bboxes": [], "masks": []}
         if "bboxes" in data:
             ret_pred["bboxes"] = [
                 normalize_bbox(box, image_size) for box in data["bboxes"]
             ]
         if "masks" in data:
             ret_pred["masks"] = [
@@ -710,7 +657,24 @@
             BboxIoU,
             SegIoU,
             Calculator,
         ]
     )
     if (hasattr(c, "name") and hasattr(c, "description") and hasattr(c, "usage"))
 }
+
+
+def _send_inference_request(
+    payload: Dict[str, Any], endpoint_name: str
+) -> Dict[str, Any]:
+    res = requests.post(
+        f"{_LND_API_URL}/model/{endpoint_name}",
+        headers={
+            "Content-Type": "application/json",
+            "apikey": _LND_API_KEY,
+        },
+        json=payload,
+    )
+    if res.status_code != 200:
+        _LOGGER.error(f"Request failed: {res.text}")
+        raise ValueError(f"Request failed: {res.text}")
+    return res.json()["data"]  # type: ignore
```

### Comparing `vision_agent-0.0.53/vision_agent/tools/video.py` & `vision_agent-0.1.1/vision_agent/tools/video.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.53/PKG-INFO` & `vision_agent-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-agent
-Version: 0.0.53
+Version: 0.1.1
 Summary: Toolset for Vision Agent
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -12,14 +12,15 @@
 Requires-Dist: faiss-cpu (>=1.0.0,<2.0.0)
 Requires-Dist: moviepy (>=1.0.0,<2.0.0)
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
 Requires-Dist: openai (>=1.0.0,<2.0.0)
 Requires-Dist: opencv-python-headless (>=4.0.0,<5.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: pillow (>=10.0.0,<11.0.0)
+Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: requests (>=2.0.0,<3.0.0)
 Requires-Dist: sentence-transformers (>=2.0.0,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: torch (>=2.1.0,<2.2.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
 Requires-Dist: typing_extensions (>=4.0.0,<5.0.0)
 Project-URL: Homepage, https://landing.ai
```

