# Comparing `tmp/vision_agent-0.0.52.tar.gz` & `tmp/vision_agent-0.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_agent-0.0.52.tar", max compression
+gzip compressed data, was "vision_agent-0.0.53.tar", max compression
```

## Comparing `vision_agent-0.0.52.tar` & `vision_agent-0.0.53.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2024-04-12 22:07:37.665620 vision_agent-0.0.52/LICENSE
--rw-r--r--   0        0        0     5035 2024-04-12 22:07:37.665620 vision_agent-0.0.52/README.md
--rw-r--r--   0        0        0     2166 2024-04-12 22:07:38.269629 vision_agent-0.0.52/pyproject.toml
--rw-r--r--   0        0        0      229 2024-04-12 22:07:37.677621 vision_agent-0.0.52/vision_agent/__init__.py
--rw-r--r--   0        0        0      127 2024-04-12 22:07:37.677621 vision_agent-0.0.52/vision_agent/agent/__init__.py
--rw-r--r--   0        0        0      529 2024-04-12 22:07:37.677621 vision_agent-0.0.52/vision_agent/agent/agent.py
--rw-r--r--   0        0        0    11511 2024-04-12 22:07:37.677621 vision_agent-0.0.52/vision_agent/agent/easytool.py
--rw-r--r--   0        0        0     4519 2024-04-12 22:07:37.677621 vision_agent-0.0.52/vision_agent/agent/easytool_prompts.py
--rw-r--r--   0        0        0    10101 2024-04-12 22:07:37.677621 vision_agent-0.0.52/vision_agent/agent/reflexion.py
--rw-r--r--   0        0        0     9342 2024-04-12 22:07:37.677621 vision_agent-0.0.52/vision_agent/agent/reflexion_prompts.py
--rw-r--r--   0        0        0    19765 2024-04-12 22:07:37.677621 vision_agent-0.0.52/vision_agent/agent/vision_agent.py
--rw-r--r--   0        0        0     6567 2024-04-12 22:07:37.677621 vision_agent-0.0.52/vision_agent/agent/vision_agent_prompts.py
--rw-r--r--   0        0        0       46 2024-04-12 22:07:37.677621 vision_agent-0.0.52/vision_agent/data/__init__.py
--rw-r--r--   0        0        0     5122 2024-04-12 22:07:37.677621 vision_agent-0.0.52/vision_agent/data/data.py
--rw-r--r--   0        0        0       75 2024-04-12 22:07:37.677621 vision_agent-0.0.52/vision_agent/emb/__init__.py
--rw-r--r--   0        0        0     1375 2024-04-12 22:07:37.677621 vision_agent-0.0.52/vision_agent/emb/emb.py
--rw-r--r--   0        0        0        0 2024-04-12 22:07:37.677621 vision_agent-0.0.52/vision_agent/fonts/__init__.py
--rw-r--r--   0        0        0  1594400 2024-04-12 22:07:37.689621 vision_agent-0.0.52/vision_agent/fonts/default_font_ch_en.ttf
--rw-r--r--   0        0        0     4786 2024-04-12 22:07:37.689621 vision_agent-0.0.52/vision_agent/image_utils.py
--rw-r--r--   0        0        0       48 2024-04-12 22:07:37.689621 vision_agent-0.0.52/vision_agent/llm/__init__.py
--rw-r--r--   0        0        0     5024 2024-04-12 22:07:37.689621 vision_agent-0.0.52/vision_agent/llm/llm.py
--rw-r--r--   0        0        0       67 2024-04-12 22:07:37.689621 vision_agent-0.0.52/vision_agent/lmm/__init__.py
--rw-r--r--   0        0        0     9535 2024-04-12 22:07:37.689621 vision_agent-0.0.52/vision_agent/lmm/lmm.py
--rw-r--r--   0        0        0      235 2024-04-12 22:07:37.689621 vision_agent-0.0.52/vision_agent/tools/__init__.py
--rw-r--r--   0        0        0     1430 2024-04-12 22:07:37.689621 vision_agent-0.0.52/vision_agent/tools/prompts.py
--rw-r--r--   0        0        0    24583 2024-04-12 22:07:37.689621 vision_agent-0.0.52/vision_agent/tools/tools.py
--rw-r--r--   0        0        0     7476 2024-04-12 22:07:37.689621 vision_agent-0.0.52/vision_agent/tools/video.py
--rw-r--r--   0        0        0     6184 1970-01-01 00:00:00.000000 vision_agent-0.0.52/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-15 20:53:19.442906 vision_agent-0.0.53/LICENSE
+-rw-r--r--   0        0        0     5035 2024-04-15 20:53:19.442906 vision_agent-0.0.53/README.md
+-rw-r--r--   0        0        0     2166 2024-04-15 20:53:20.006911 vision_agent-0.0.53/pyproject.toml
+-rw-r--r--   0        0        0      229 2024-04-15 20:53:19.454906 vision_agent-0.0.53/vision_agent/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-15 20:53:19.454906 vision_agent-0.0.53/vision_agent/agent/__init__.py
+-rw-r--r--   0        0        0      529 2024-04-15 20:53:19.454906 vision_agent-0.0.53/vision_agent/agent/agent.py
+-rw-r--r--   0        0        0    11511 2024-04-15 20:53:19.454906 vision_agent-0.0.53/vision_agent/agent/easytool.py
+-rw-r--r--   0        0        0     4519 2024-04-15 20:53:19.454906 vision_agent-0.0.53/vision_agent/agent/easytool_prompts.py
+-rw-r--r--   0        0        0    10101 2024-04-15 20:53:19.454906 vision_agent-0.0.53/vision_agent/agent/reflexion.py
+-rw-r--r--   0        0        0     9342 2024-04-15 20:53:19.454906 vision_agent-0.0.53/vision_agent/agent/reflexion_prompts.py
+-rw-r--r--   0        0        0    19765 2024-04-15 20:53:19.458906 vision_agent-0.0.53/vision_agent/agent/vision_agent.py
+-rw-r--r--   0        0        0     6567 2024-04-15 20:53:19.458906 vision_agent-0.0.53/vision_agent/agent/vision_agent_prompts.py
+-rw-r--r--   0        0        0       46 2024-04-15 20:53:19.458906 vision_agent-0.0.53/vision_agent/data/__init__.py
+-rw-r--r--   0        0        0     5122 2024-04-15 20:53:19.458906 vision_agent-0.0.53/vision_agent/data/data.py
+-rw-r--r--   0        0        0       75 2024-04-15 20:53:19.458906 vision_agent-0.0.53/vision_agent/emb/__init__.py
+-rw-r--r--   0        0        0     1375 2024-04-15 20:53:19.458906 vision_agent-0.0.53/vision_agent/emb/emb.py
+-rw-r--r--   0        0        0        0 2024-04-15 20:53:19.458906 vision_agent-0.0.53/vision_agent/fonts/__init__.py
+-rw-r--r--   0        0        0  1594400 2024-04-15 20:53:19.466906 vision_agent-0.0.53/vision_agent/fonts/default_font_ch_en.ttf
+-rw-r--r--   0        0        0     4786 2024-04-15 20:53:19.466906 vision_agent-0.0.53/vision_agent/image_utils.py
+-rw-r--r--   0        0        0       48 2024-04-15 20:53:19.466906 vision_agent-0.0.53/vision_agent/llm/__init__.py
+-rw-r--r--   0        0        0     5024 2024-04-15 20:53:19.466906 vision_agent-0.0.53/vision_agent/llm/llm.py
+-rw-r--r--   0        0        0       67 2024-04-15 20:53:19.466906 vision_agent-0.0.53/vision_agent/lmm/__init__.py
+-rw-r--r--   0        0        0     9535 2024-04-15 20:53:19.466906 vision_agent-0.0.53/vision_agent/lmm/lmm.py
+-rw-r--r--   0        0        0      253 2024-04-15 20:53:19.466906 vision_agent-0.0.53/vision_agent/tools/__init__.py
+-rw-r--r--   0        0        0     1430 2024-04-15 20:53:19.466906 vision_agent-0.0.53/vision_agent/tools/prompts.py
+-rw-r--r--   0        0        0    27045 2024-04-15 20:53:19.466906 vision_agent-0.0.53/vision_agent/tools/tools.py
+-rw-r--r--   0        0        0     7476 2024-04-15 20:53:19.466906 vision_agent-0.0.53/vision_agent/tools/video.py
+-rw-r--r--   0        0        0     6184 1970-01-01 00:00:00.000000 vision_agent-0.0.53/PKG-INFO
```

### Comparing `vision_agent-0.0.52/LICENSE` & `vision_agent-0.0.53/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.52/README.md` & `vision_agent-0.0.53/README.md`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.52/pyproject.toml` & `vision_agent-0.0.53/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vision-agent"
-version = "0.0.52"
+version = "0.0.53"
 description = "Toolset for Vision Agent"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "vision_agent"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `vision_agent-0.0.52/vision_agent/agent/agent.py` & `vision_agent-0.0.53/vision_agent/agent/agent.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.52/vision_agent/agent/easytool.py` & `vision_agent-0.0.53/vision_agent/agent/easytool.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.52/vision_agent/agent/easytool_prompts.py` & `vision_agent-0.0.53/vision_agent/agent/easytool_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.52/vision_agent/agent/reflexion.py` & `vision_agent-0.0.53/vision_agent/agent/reflexion.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.52/vision_agent/agent/reflexion_prompts.py` & `vision_agent-0.0.53/vision_agent/agent/reflexion_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.52/vision_agent/agent/vision_agent.py` & `vision_agent-0.0.53/vision_agent/agent/vision_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,15 @@
     """
 
     def __init__(
         self,
         task_model: Optional[Union[LLM, LMM]] = None,
         answer_model: Optional[Union[LLM, LMM]] = None,
         reflect_model: Optional[Union[LLM, LMM]] = None,
-        max_retries: int = 3,
+        max_retries: int = 2,
         verbose: bool = False,
         report_progress_callback: Optional[Callable[[str], None]] = None,
     ):
         """VisionAgent constructor.
 
         Parameters
             task_model: the model to use for task decomposition.
```

### Comparing `vision_agent-0.0.52/vision_agent/agent/vision_agent_prompts.py` & `vision_agent-0.0.53/vision_agent/agent/vision_agent_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.52/vision_agent/data/data.py` & `vision_agent-0.0.53/vision_agent/data/data.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.52/vision_agent/emb/emb.py` & `vision_agent-0.0.53/vision_agent/emb/emb.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.52/vision_agent/fonts/default_font_ch_en.ttf` & `vision_agent-0.0.53/vision_agent/fonts/default_font_ch_en.ttf`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.52/vision_agent/image_utils.py` & `vision_agent-0.0.53/vision_agent/image_utils.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.52/vision_agent/llm/llm.py` & `vision_agent-0.0.53/vision_agent/llm/llm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.52/vision_agent/lmm/lmm.py` & `vision_agent-0.0.53/vision_agent/lmm/lmm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.52/vision_agent/tools/prompts.py` & `vision_agent-0.0.53/vision_agent/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.52/vision_agent/tools/tools.py` & `vision_agent-0.0.53/vision_agent/tools/tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -140,14 +140,82 @@
         resp_json["data"]["scores"] = [
             round(prob, 4) for prob in resp_json["data"]["scores"]
         ]
 
         return resp_json["data"]  # type: ignore
 
 
+class ImageCaption(Tool):
+    r"""ImageCaption is a tool that can caption an image based on its contents
+    or tags.
+
+    Example
+    -------
+        >>> import vision_agent as va
+        >>> caption = va.tools.ImageCaption()
+        >>> caption("image1.jpg")
+        {'text': ['a box of orange and white socks']}
+    """
+
+    _ENDPOINT = "https://soi4ewr6fjqqdf5vuss6rrilee0kumxq.lambda-url.us-east-2.on.aws"
+
+    name = "image_caption_"
+    description = "'image_caption_' is a tool that can caption an image based on its contents or tags. It returns a text describing the image"
+    usage = {
+        "required_parameters": [
+            {"name": "image", "type": "str"},
+        ],
+        "examples": [
+            {
+                "scenario": "Can you describe this image ? Image name: cat.jpg",
+                "parameters": {"image": "cat.jpg"},
+            },
+            {
+                "scenario": "Can you caption this image with their main contents ? Image name: cat_dog.jpg",
+                "parameters": {"image": "cat_dog.jpg"},
+            },
+            {
+                "scenario": "Can you build me a image captioning tool ? Image name: shirts.jpg",
+                "parameters": {
+                    "image": "shirts.jpg",
+                },
+            },
+        ],
+    }
+
+    # TODO: Add support for input multiple images, which aligns with the output type.
+    def __call__(self, image: Union[str, ImageType]) -> Dict:
+        """Invoke the Image captioning model.
+
+        Parameters:
+            image: the input image to caption.
+
+        Returns:
+            A list of dictionaries containing the labels and scores. Each dictionary contains the classification result for an image. E.g. [{"labels": ["red line", "yellow dot"], "scores": [0.98, 0.02]}]
+        """
+        image_b64 = convert_to_b64(image)
+        data = {
+            "image": image_b64,
+            "tool": "image_captioning",
+        }
+        res = requests.post(
+            self._ENDPOINT,
+            headers={"Content-Type": "application/json"},
+            json=data,
+        )
+        resp_json: Dict[str, Any] = res.json()
+        if (
+            "statusCode" in resp_json and resp_json["statusCode"] != 200
+        ) or "statusCode" not in resp_json:
+            _LOGGER.error(f"Request failed: {resp_json}")
+            raise ValueError(f"Request failed: {resp_json}")
+
+        return resp_json["data"]  # type: ignore
+
+
 class GroundingDINO(Tool):
     r"""Grounding DINO is a tool that can detect arbitrary objects with inputs such as
     category names or referring expressions.
 
     Example
     -------
         >>> import vision_agent as va
@@ -627,14 +695,15 @@
 
 TOOLS = {
     i: {"name": c.name, "description": c.description, "usage": c.usage, "class": c}
     for i, c in enumerate(
         [
             NoOp,
             CLIP,
+            ImageCaption,
             GroundingDINO,
             AgentGroundingSAM,
             ExtractFrames,
             Counter,
             Crop,
             BboxArea,
             SegArea,
```

### Comparing `vision_agent-0.0.52/vision_agent/tools/video.py` & `vision_agent-0.0.53/vision_agent/tools/video.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.52/PKG-INFO` & `vision_agent-0.0.53/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-agent
-Version: 0.0.52
+Version: 0.0.53
 Summary: Toolset for Vision Agent
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

