# Comparing `tmp/substrate-120240411.0.5.tar.gz` & `tmp/substrate-120240416.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrate-120240411.0.5.tar", max compression
+gzip compressed data, was "substrate-120240416.0.5.tar", max compression
```

## Comparing `substrate-120240411.0.5.tar` & `substrate-120240416.0.5.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-120240411.0.5/LICENSE
--rw-r--r--   0        0        0       45 2024-03-19 21:55:57.200047 substrate-120240411.0.5/README.md
--rw-r--r--   0        0        0     2023 2024-04-15 03:37:56.646268 substrate-120240411.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 19:17:25.000000 substrate-120240411.0.5/substrate/.keep
--rw-r--r--   0        0        0       17 2024-04-14 20:21:27.000000 substrate-120240411.0.5/substrate/GEN_VERSION
--rw-r--r--   0        0        0     2048 2024-04-14 20:21:28.000000 substrate-120240411.0.5/substrate/__init__.py
--rw-r--r--   0        0        0     5762 2024-04-15 03:37:11.134607 substrate-120240411.0.5/substrate/_client.py
--rw-r--r--   0        0        0       30 2024-03-13 14:46:31.829473 substrate-120240411.0.5/substrate/_version.py
--rw-r--r--   0        0        0        1 2024-04-14 21:12:46.459958 substrate-120240411.0.5/substrate/core/__init__.py
--rw-r--r--   0        0        0       27 2024-04-14 21:12:46.459837 substrate-120240411.0.5/substrate/core/_version.py
--rw-r--r--   0        0        0     1535 2024-04-14 21:12:46.460219 substrate-120240411.0.5/substrate/core/base_future.py
--rw-r--r--   0        0        0        0 2024-04-14 21:12:46.460602 substrate-120240411.0.5/substrate/core/client/__init__.py
--rw-r--r--   0        0        0     1750 2024-04-14 21:12:46.460706 substrate-120240411.0.5/substrate/core/client/find_futures_client.py
--rw-r--r--   0        0        0     2697 2024-04-14 21:12:46.460832 substrate-120240411.0.5/substrate/core/client/future.py
--rw-r--r--   0        0        0     1212 2024-04-14 21:12:46.460537 substrate-120240411.0.5/substrate/core/client/graph.py
--rw-r--r--   0        0        0     1149 2024-04-14 21:12:46.460085 substrate-120240411.0.5/substrate/core/coregraph.py
--rw-r--r--   0        0        0     1989 2024-04-14 21:12:46.459382 substrate-120240411.0.5/substrate/core/corenode.py
--rw-r--r--   0        0        0     1227 2024-04-14 21:12:46.460350 substrate-120240411.0.5/substrate/core/future_directive.py
--rw-r--r--   0        0        0      894 2024-04-14 21:12:46.459221 substrate-120240411.0.5/substrate/core/id_generator.py
--rw-r--r--   0        0        0    37511 2024-04-14 21:12:46.459592 substrate-120240411.0.5/substrate/core/models.py
--rw-r--r--   0        0        0     2332 2024-04-14 21:12:46.459081 substrate-120240411.0.5/substrate/core/sb.py
--rw-r--r--   0        0        0    31945 2024-04-14 20:21:25.000000 substrate-120240411.0.5/substrate/dataclass_models.py
--rw-r--r--   0        0        0    42701 2024-04-14 20:21:27.000000 substrate-120240411.0.5/substrate/future_dataclass_models.py
--rw-r--r--   0        0        0    59500 2024-04-14 20:21:28.000000 substrate-120240411.0.5/substrate/nodes.py
--rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-120240411.0.5/substrate/py.typed
--rw-r--r--   0        0        0     1647 2024-04-05 21:20:49.456063 substrate-120240411.0.5/substrate/substrate.py
--rw-r--r--   0        0        0    34991 2024-04-14 20:21:24.000000 substrate-120240411.0.5/substrate/typeddict_models.py
--rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 substrate-120240411.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-120240416.0.5/LICENSE
+-rw-r--r--   0        0        0       45 2024-03-19 21:55:57.200047 substrate-120240416.0.5/README.md
+-rw-r--r--   0        0        0     2023 2024-04-16 21:23:44.744816 substrate-120240416.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 19:17:25.000000 substrate-120240416.0.5/substrate/.keep
+-rw-r--r--   0        0        0       17 2024-04-16 21:23:08.000000 substrate-120240416.0.5/substrate/GEN_VERSION
+-rw-r--r--   0        0        0     2048 2024-04-16 21:23:09.000000 substrate-120240416.0.5/substrate/__init__.py
+-rw-r--r--   0        0        0     6010 2024-04-16 20:07:00.739333 substrate-120240416.0.5/substrate/_client.py
+-rw-r--r--   0        0        0       30 2024-03-13 14:46:31.829473 substrate-120240416.0.5/substrate/_version.py
+-rw-r--r--   0        0        0        1 2024-04-16 21:23:27.826516 substrate-120240416.0.5/substrate/core/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-16 21:23:27.826379 substrate-120240416.0.5/substrate/core/_version.py
+-rw-r--r--   0        0        0     1535 2024-04-16 21:23:27.826967 substrate-120240416.0.5/substrate/core/base_future.py
+-rw-r--r--   0        0        0        0 2024-04-16 21:23:27.827571 substrate-120240416.0.5/substrate/core/client/__init__.py
+-rw-r--r--   0        0        0     1750 2024-04-16 21:23:27.827722 substrate-120240416.0.5/substrate/core/client/find_futures_client.py
+-rw-r--r--   0        0        0     2697 2024-04-16 21:23:27.827901 substrate-120240416.0.5/substrate/core/client/future.py
+-rw-r--r--   0        0        0     1212 2024-04-16 21:23:27.827319 substrate-120240416.0.5/substrate/core/client/graph.py
+-rw-r--r--   0        0        0     1149 2024-04-16 21:23:27.826777 substrate-120240416.0.5/substrate/core/coregraph.py
+-rw-r--r--   0        0        0     2186 2024-04-16 21:23:27.825560 substrate-120240416.0.5/substrate/core/corenode.py
+-rw-r--r--   0        0        0     1227 2024-04-16 21:23:27.827149 substrate-120240416.0.5/substrate/core/future_directive.py
+-rw-r--r--   0        0        0      894 2024-04-16 21:23:27.825332 substrate-120240416.0.5/substrate/core/id_generator.py
+-rw-r--r--   0        0        0    38450 2024-04-16 21:23:27.825854 substrate-120240416.0.5/substrate/core/models.py
+-rw-r--r--   0        0        0     2332 2024-04-16 21:23:27.825185 substrate-120240416.0.5/substrate/core/sb.py
+-rw-r--r--   0        0        0    32587 2024-04-16 21:23:06.000000 substrate-120240416.0.5/substrate/dataclass_models.py
+-rw-r--r--   0        0        0    43578 2024-04-16 21:23:08.000000 substrate-120240416.0.5/substrate/future_dataclass_models.py
+-rw-r--r--   0        0        0    40555 2024-04-16 21:23:09.000000 substrate-120240416.0.5/substrate/nodes.py
+-rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-120240416.0.5/substrate/py.typed
+-rw-r--r--   0        0        0     1490 2024-04-16 20:07:00.739577 substrate-120240416.0.5/substrate/substrate.py
+-rw-r--r--   0        0        0     1041 2024-04-16 20:45:00.388800 substrate-120240416.0.5/substrate/substrate_response.py
+-rw-r--r--   0        0        0    35749 2024-04-16 21:23:05.000000 substrate-120240416.0.5/substrate/typeddict_models.py
+-rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 substrate-120240416.0.5/PKG-INFO
```

### Comparing `substrate-120240411.0.5/LICENSE` & `substrate-120240416.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `substrate-120240411.0.5/pyproject.toml` & `substrate-120240416.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "substrate"
-version = "120240411.0.5"
+version = "120240416.0.5"
 description = "Substrate Python SDK"
 readme = "README.md"
 authors = [ "vprtwn <ben@substrate.run>", "liamgriffiths <liam@substrate.run>",]
 [[tool.poetry.packages]]
 include = "substrate"
 
 [tool.pyright]
```

### Comparing `substrate-120240411.0.5/substrate/__init__.py` & `substrate-120240416.0.5/substrate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 ꩜ Substrate Python SDK
 
-20240411.20240414
+20240416.20240416
 """
 
 from .nodes import (
     CLIP,
     XTTSV2,
     JinaV2,
     BigLaMa,
```

### Comparing `substrate-120240411.0.5/substrate/_client.py` & `substrate-120240416.0.5/substrate/_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,24 +137,33 @@
     @property
     def elapsed(self) -> datetime.timedelta:
         """The time taken for the complete request/response cycle to complete."""
         return self.http_response.elapsed
 
 
 class APIClient:
-    api_key: str
-    base_url: str
+    _api_key: str
+    _base_url: str
     _client: httpx.Client
     _async_client: httpx.AsyncClient
     _version: str
+    _backend: str
+    _additional_headers: Dict[str, Any]
 
-    def __init__(self, api_key: str, base_url: str, backend: str) -> None:
-        self.api_key = api_key
-        self.base_url = base_url
-        self.backend = backend
+    def __init__(
+        self,
+        api_key: str,
+        base_url: str,
+        backend: str,
+        additional_headers: Dict[str, Any] = {},
+    ) -> None:
+        self._api_key = api_key
+        self._base_url = base_url
+        self._backend = backend
+        self._additional_headers = additional_headers
         timeout = httpx.Timeout(60.0)  # default is 5s
         self._client = httpx.Client(timeout=timeout)
         self._async_client = httpx.AsyncClient(timeout=timeout)
         self._version = __version__
 
     @property
     def user_agent(self) -> str:
@@ -181,27 +190,28 @@
 
     @property
     def default_headers(self) -> Dict[str, str]:
         return {
             "Accept": "application/json",
             "Content-Type": "application/json",
             "User-Agent": self.user_agent,
-            "X-Substrate-Backend": self.backend,
+            "X-Substrate-Backend": self._backend,
             **self.platform_headers,
             **self.auth_headers,
+            **self._additional_headers,
         }
 
     def post_compose(self, dag: Dict[str, Any]) -> APIResponse:
-        url = f"{self.base_url}/compose"
+        url = f"{self._base_url}/compose"
         body = {"dag": dag}
         http_response = self._client.post(url, headers=self.default_headers, json=body)
         res = APIResponse(http_response=http_response)
         res.request = body
         return res
 
     async def async_post_compose(self, dag: Dict[str, Any]) -> APIResponse:
-        url = f"{self.base_url}/compose"
+        url = f"{self._base_url}/compose"
         body = {"dag": dag}
         http_response = await self._async_client.post(url, headers=self.default_headers, json=body)
         res = APIResponse(http_response=http_response)
         res.request = body
         return res
```

### Comparing `substrate-120240411.0.5/substrate/core/base_future.py` & `substrate-120240416.0.5/substrate/core/base_future.py`

 * *Files identical despite different names*

### Comparing `substrate-120240411.0.5/substrate/core/client/find_futures_client.py` & `substrate-120240416.0.5/substrate/core/client/find_futures_client.py`

 * *Files identical despite different names*

### Comparing `substrate-120240411.0.5/substrate/core/client/future.py` & `substrate-120240416.0.5/substrate/core/client/future.py`

 * *Files identical despite different names*

### Comparing `substrate-120240411.0.5/substrate/core/client/graph.py` & `substrate-120240416.0.5/substrate/core/client/graph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240411.0.5/substrate/core/coregraph.py` & `substrate-120240416.0.5/substrate/core/coregraph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240411.0.5/substrate/core/corenode.py` & `substrate-120240416.0.5/substrate/core/corenode.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 CORE ꩜ SUBSTRATE
 """
-from typing import List, Optional
+from typing import Any, List, Type, Optional
 
 import networkx as nx
 
 from .base_future import BaseFuture
 from .id_generator import IDGenerator
 from .client.future import TracedFuture
 from .future_directive import TraceDirective
@@ -24,14 +24,21 @@
         if attr:
             self.args = BaseFuture.replace_futures_with_placeholder(attr)
         else:
             self.args = {}
         self.SG.add_node(self, **self.args)
         self.futures_from_args: List[BaseFuture] = find_futures_client(attr)
 
+    @property
+    def out_type(self) -> Type[Any]:
+        """
+        Get the typed output of this node using `response.get(node, node.out_type)`
+        """
+        return Type[None]
+
     def to_dict(self):
         return {
             "id": self.id,
             "node": self.node,
             "args": self.args,
             **({"_should_output_globally": self._should_output_globally} if self._should_output_globally else {}),
             **({"_global_output_keys": self._global_output_keys} if self._global_output_keys else {}),
```

### Comparing `substrate-120240411.0.5/substrate/core/future_directive.py` & `substrate-120240416.0.5/substrate/core/future_directive.py`

 * *Files identical despite different names*

### Comparing `substrate-120240411.0.5/substrate/core/id_generator.py` & `substrate-120240416.0.5/substrate/core/id_generator.py`

 * *Files identical despite different names*

### Comparing `substrate-120240411.0.5/substrate/core/models.py` & `substrate-120240416.0.5/substrate/core/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,19 +99,23 @@
     """
 
 
 class MultiGenerateTextIn(BaseModel):
     class Config:
         extra = Extra.allow
 
-    prompt: str
+    prompt: Optional[str] = None
     """
     Input prompt.
     """
-    num_choices: Annotated[int, Field(ge=1, le=8)]
+    batch_prompts: Optional[List[str]] = None
+    """
+    Batch input prompts.
+    """
+    num_choices: Annotated[int, Field(ge=1, le=8)] = 1
     """
     Number of choices to generate.
     """
     temperature: Annotated[float, Field(ge=0.0, le=1.0)] = 0.4
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
@@ -121,37 +125,51 @@
     """
     node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
-class MultiGenerateTextOut(BaseModel):
+class MultiGenerateTextOutput(BaseModel):
     class Config:
         extra = Extra.allow
 
     choices: List[GenerateTextOut]
     """
     Response choices.
     """
 
 
+class MultiGenerateTextOut(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    outputs: List[MultiGenerateTextOutput]
+    """
+    A single output for `prompt`, or multiple outputs for `batch_prompts`.
+    """
+
+
 class MultiGenerateJSONIn(BaseModel):
     class Config:
         extra = Extra.allow
 
-    prompt: str
+    prompt: Optional[str] = None
     """
     Input prompt.
     """
     json_schema: Dict[str, Any]
     """
     JSON schema to guide `json_object` response.
     """
-    num_choices: Annotated[int, Field(ge=1, le=8)]
+    batch_prompts: Optional[List[str]] = None
+    """
+    Batch input prompts.
+    """
+    num_choices: Annotated[int, Field(ge=1, le=8)] = 2
     """
     Number of choices to generate.
     """
     temperature: Annotated[float, Field(ge=0.0, le=1.0)] = 0.4
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
@@ -161,40 +179,54 @@
     """
     node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
-class MultiGenerateJSONOut(BaseModel):
+class MultiGenerateJSONOutput(BaseModel):
     class Config:
         extra = Extra.allow
 
     choices: List[GenerateJSONOut]
     """
     Response choices.
     """
 
 
+class MultiGenerateJSONOut(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    outputs: List[MultiGenerateJSONOutput]
+    """
+    A single output for `prompt`, or multiple outputs for `batch_prompts`.
+    """
+
+
 class Mistral7BInstructIn(BaseModel):
     class Config:
         extra = Extra.allow
 
-    prompt: str
+    prompt: Optional[str] = None
     """
     Input prompt.
     """
-    num_choices: Annotated[int, Field(ge=1, le=8)]
+    num_choices: Annotated[int, Field(ge=1, le=8)] = 1
     """
     Number of choices to generate.
     """
     json_schema: Optional[Dict[str, Any]] = None
     """
     JSON schema to guide response.
     """
+    batch_prompts: Optional[List[str]] = None
+    """
+    Batch input prompts.
+    """
     temperature: Annotated[Optional[float], Field(ge=0.0, le=1.0)] = None
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
@@ -211,24 +243,34 @@
     """
     json_object: Optional[Dict[str, Any]] = None
     """
     JSON response, if `json_schema` was provided.
     """
 
 
-class Mistral7BInstructOut(BaseModel):
+class Mistral7BInstructOutput(BaseModel):
     class Config:
         extra = Extra.allow
 
     choices: List[Mistral7BInstructChoice]
     """
     Response choices.
     """
 
 
+class Mistral7BInstructOut(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    outputs: List[Mistral7BInstructOutput]
+    """
+    A single output for `prompt`, or multiple outputs for `batch_prompts`.
+    """
+
+
 class GenerateTextVisionIn(BaseModel):
     class Config:
         extra = Extra.allow
 
     prompt: str
     """
     Text prompt.
@@ -365,19 +407,19 @@
     """
     Number of images to generate.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    height: Annotated[int, Field(ge=640, le=1536)] = 1024
+    height: Annotated[int, Field(ge=256, le=1536)] = 1024
     """
     Height of output image, in pixels.
     """
-    width: Annotated[int, Field(ge=640, le=1536)] = 1024
+    width: Annotated[int, Field(ge=256, le=1536)] = 1024
     """
     Width of output image, in pixels.
     """
     seeds: Optional[List[int]] = None
     """
     Seeds for deterministic generation. Default is a random seed.
     """
@@ -427,19 +469,19 @@
     """
     Number of images to generate.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    height: Optional[int] = None
+    height: Annotated[int, Field(ge=256, le=1536)] = 1024
     """
     Height of output image, in pixels.
     """
-    width: Optional[int] = None
+    width: Annotated[int, Field(ge=256, le=1536)] = 1024
     """
     Width of output image, in pixels.
     """
     seeds: Optional[List[int]] = None
     """
     Seeds for deterministic generation. Default is a random seed.
     """
@@ -467,31 +509,31 @@
     """
     Image prompt.
     """
     num_images: Annotated[int, Field(ge=1, le=8)]
     """
     Number of images to generate.
     """
-    ip_adapter_scale: Annotated[Optional[float], Field(ge=0.0)] = None
+    ip_adapter_scale: Annotated[float, Field(ge=0.0, le=1.0)] = 0.5
     """
     Controls the influence of the image prompt on the generated output.
     """
     negative_prompt: Optional[str] = None
     """
     Negative input prompt.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    width: Optional[int] = None
+    width: Annotated[int, Field(ge=640, le=1536)] = 1024
     """
     Width of output image, in pixels.
     """
-    height: Optional[int] = None
+    height: Annotated[int, Field(ge=640, le=1536)] = 1024
     """
     Height of output image, in pixels.
     """
     seeds: Optional[List[int]] = None
     """
     Random noise seeds. Default is random seeds for each generation.
     """
@@ -535,15 +577,15 @@
     """
     Negative input prompt.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    conditioning_scale: Annotated[Optional[float], Field(ge=0.0)] = None
+    conditioning_scale: Annotated[float, Field(ge=0.0, le=1.0)] = 0.5
     """
     Controls the influence of the input image on the generated output.
     """
     seeds: Optional[List[int]] = None
     """
     Random noise seeds. Default is random seeds for each generation.
     """
@@ -663,15 +705,15 @@
     """
     Negative input prompt.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    strength: Annotated[float, Field(ge=0.0, le=1.0)] = 1
+    strength: Annotated[float, Field(ge=0.0, le=1.0)] = 0.8
     """
     Controls the strength of the generation process.
     """
     seeds: Optional[List[int]] = None
     """
     Random noise seeds. Default is random seeds for each generation.
     """
@@ -1369,18 +1411,14 @@
     class Config:
         extra = Extra.allow
 
     items: List[EmbedTextOrImageItem]
     """
     Items to embed.
     """
-    embedded_metadata_keys: Optional[List[str]] = None
-    """
-    Choose keys from `metadata` to embed with text, when embedding and storing text documents.
-    """
     store: Optional[str] = None
     """
     [Vector store](/docs/vector-stores) identifier.
     """
 
 
 class CLIPOut(BaseModel):
@@ -1399,15 +1437,15 @@
 
     name: Annotated[str, Field(max_length=63, min_length=1)]
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
-    Selected embedding model
+    Selected embedding model.
     """
     m: Annotated[int, Field(ge=1, le=64)] = 16
     """
     The max number of connections per layer for the index.
     """
     ef_construction: Annotated[int, Field(ge=1, le=128)] = 64
     """
@@ -1425,15 +1463,15 @@
 
     name: Annotated[str, Field(max_length=63, min_length=1)]
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
-    Selected embedding model
+    Selected embedding model.
     """
     m: Annotated[int, Field(ge=1, le=64)]
     """
     The max number of connections per layer for the index.
     """
     ef_construction: Annotated[int, Field(ge=1, le=128)]
     """
@@ -1468,29 +1506,29 @@
 
     name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
-    Selected embedding model
+    Selected embedding model.
     """
 
 
 class DeleteVectorStoreOut(BaseModel):
     class Config:
         extra = Extra.allow
 
     name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
-    Selected embedding model
+    Selected embedding model.
     """
 
 
 class Vector(BaseModel):
     """
     Canonical representation of document with embedding vector.
     """
@@ -1518,15 +1556,15 @@
 
     name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
-    Selected embedding model
+    Selected embedding model.
     """
     ids: Annotated[List[str], Field(max_items=100)]
     """
     Document IDs to retrieve.
     """
 
 
@@ -1584,15 +1622,15 @@
 
     name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
-    Selected embedding model
+    Selected embedding model.
     """
     vectors: Annotated[List[UpdateVectorParams], Field(max_items=100)]
     """
     Vectors to upsert.
     """
 
 
@@ -1602,15 +1640,15 @@
 
     name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
-    Selected embedding model
+    Selected embedding model.
     """
     ids: Annotated[List[str], Field(max_items=100)]
     """
     Document IDs to delete.
     """
 
 
@@ -1620,31 +1658,31 @@
 
     name: str
     """
     Vector store to query against.
     """
     model: Literal["jina-v2", "clip"]
     """
-    Selected embedding model
+    Selected embedding model.
     """
-    query_ids: Optional[List[str]] = None
+    query_strings: Optional[List[str]] = None
     """
-    Document IDs to use for the query.
+    Texts to embed and use for the query.
     """
     query_image_uris: Optional[List[str]] = None
     """
     Image URIs to embed and use for the query.
     """
     query_vectors: Optional[List[List[float]]] = None
     """
-    Vector to use for the query.
+    Vectors to use for the query.
     """
-    query_strings: Optional[List[str]] = None
+    query_ids: Optional[List[str]] = None
     """
-    Texts to embed and use for the query.
+    Document IDs to use for the query.
     """
     top_k: Annotated[int, Field(ge=1, le=1000)] = 10
     """
     Number of results to return.
     """
     ef_search: Annotated[int, Field(ge=1, le=1000)] = 40
     """
@@ -1700,13 +1738,13 @@
     """
     name: Optional[str] = None
     """
     Vector store name.
     """
     model: Optional[Literal["jina-v2", "clip"]] = None
     """
-    Selected embedding model
+    Selected embedding model.
     """
     metric: Optional[Literal["cosine", "l2", "inner"]] = None
     """
     The distance metric used for the query.
     """
```

### Comparing `substrate-120240411.0.5/substrate/core/sb.py` & `substrate-120240416.0.5/substrate/core/sb.py`

 * *Files identical despite different names*

### Comparing `substrate-120240411.0.5/substrate/dataclass_models.py` & `substrate-120240416.0.5/substrate/dataclass_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,19 +86,23 @@
     """
     JSON response.
     """
 
 
 @dataclass
 class MultiGenerateTextIn:
-    prompt: str
+    prompt: Optional[str] = None
     """
     Input prompt.
     """
-    num_choices: int
+    batch_prompts: Optional[List[str]] = None
+    """
+    Batch input prompts.
+    """
+    num_choices: int = 1
     """
     Number of choices to generate.
     """
     temperature: float = 0.4
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
@@ -109,32 +113,44 @@
     node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
 @dataclass
-class MultiGenerateTextOut:
+class MultiGenerateTextOutput:
     choices: List[GenerateTextOut]
     """
     Response choices.
     """
 
 
 @dataclass
-class MultiGenerateJSONIn:
-    prompt: str
+class MultiGenerateTextOut:
+    outputs: List[MultiGenerateTextOutput]
     """
-    Input prompt.
+    A single output for `prompt`, or multiple outputs for `batch_prompts`.
     """
+
+
+@dataclass
+class MultiGenerateJSONIn:
     json_schema: Dict[str, Any]
     """
     JSON schema to guide `json_object` response.
     """
-    num_choices: int
+    prompt: Optional[str] = None
+    """
+    Input prompt.
+    """
+    batch_prompts: Optional[List[str]] = None
+    """
+    Batch input prompts.
+    """
+    num_choices: int = 2
     """
     Number of choices to generate.
     """
     temperature: float = 0.4
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
@@ -145,35 +161,47 @@
     node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
 @dataclass
-class MultiGenerateJSONOut:
+class MultiGenerateJSONOutput:
     choices: List[GenerateJSONOut]
     """
     Response choices.
     """
 
 
 @dataclass
+class MultiGenerateJSONOut:
+    outputs: List[MultiGenerateJSONOutput]
+    """
+    A single output for `prompt`, or multiple outputs for `batch_prompts`.
+    """
+
+
+@dataclass
 class Mistral7BInstructIn:
-    prompt: str
+    prompt: Optional[str] = None
     """
     Input prompt.
     """
-    num_choices: int
+    num_choices: int = 1
     """
     Number of choices to generate.
     """
     json_schema: Optional[Dict[str, Any]] = None
     """
     JSON schema to guide response.
     """
+    batch_prompts: Optional[List[str]] = None
+    """
+    Batch input prompts.
+    """
     temperature: Optional[float] = None
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
@@ -189,22 +217,30 @@
     json_object: Optional[Dict[str, Any]] = None
     """
     JSON response, if `json_schema` was provided.
     """
 
 
 @dataclass
-class Mistral7BInstructOut:
+class Mistral7BInstructOutput:
     choices: List[Mistral7BInstructChoice]
     """
     Response choices.
     """
 
 
 @dataclass
+class Mistral7BInstructOut:
+    outputs: List[Mistral7BInstructOutput]
+    """
+    A single output for `prompt`, or multiple outputs for `batch_prompts`.
+    """
+
+
+@dataclass
 class GenerateTextVisionIn:
     prompt: str
     """
     Text prompt.
     """
     image_uris: List[str]
     """
@@ -378,19 +414,19 @@
     """
     Number of images to generate.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    height: Optional[int] = None
+    height: int = 1024
     """
     Height of output image, in pixels.
     """
-    width: Optional[int] = None
+    width: int = 1024
     """
     Width of output image, in pixels.
     """
     seeds: Optional[List[int]] = None
     """
     Seeds for deterministic generation. Default is a random seed.
     """
@@ -414,31 +450,31 @@
     """
     Number of images to generate.
     """
     image_prompt_uri: Optional[str] = None
     """
     Image prompt.
     """
-    ip_adapter_scale: Optional[float] = None
+    ip_adapter_scale: float = 0.5
     """
     Controls the influence of the image prompt on the generated output.
     """
     negative_prompt: Optional[str] = None
     """
     Negative input prompt.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    width: Optional[int] = None
+    width: int = 1024
     """
     Width of output image, in pixels.
     """
-    height: Optional[int] = None
+    height: int = 1024
     """
     Height of output image, in pixels.
     """
     seeds: Optional[List[int]] = None
     """
     Random noise seeds. Default is random seeds for each generation.
     """
@@ -478,15 +514,15 @@
     """
     Negative input prompt.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    conditioning_scale: Optional[float] = None
+    conditioning_scale: float = 0.5
     """
     Controls the influence of the input image on the generated output.
     """
     seeds: Optional[List[int]] = None
     """
     Random noise seeds. Default is random seeds for each generation.
     """
@@ -594,15 +630,15 @@
     """
     Negative input prompt.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    strength: float = 1
+    strength: float = 0.8
     """
     Controls the strength of the generation process.
     """
     seeds: Optional[List[int]] = None
     """
     Random noise seeds. Default is random seeds for each generation.
     """
@@ -1214,18 +1250,14 @@
 
 @dataclass
 class CLIPIn:
     items: List[EmbedTextOrImageItem]
     """
     Items to embed.
     """
-    embedded_metadata_keys: Optional[List[str]] = None
-    """
-    Choose keys from `metadata` to embed with text, when embedding and storing text documents.
-    """
     store: Optional[str] = None
     """
     [Vector store](/docs/vector-stores) identifier.
     """
 
 
 @dataclass
@@ -1240,15 +1272,15 @@
 class CreateVectorStoreIn:
     name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
-    Selected embedding model
+    Selected embedding model.
     """
     m: int = 16
     """
     The max number of connections per layer for the index.
     """
     ef_construction: int = 64
     """
@@ -1264,15 +1296,15 @@
 class CreateVectorStoreOut:
     name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
-    Selected embedding model
+    Selected embedding model.
     """
     m: int
     """
     The max number of connections per layer for the index.
     """
     ef_construction: int
     """
@@ -1301,27 +1333,27 @@
 class DeleteVectorStoreIn:
     name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
-    Selected embedding model
+    Selected embedding model.
     """
 
 
 @dataclass
 class DeleteVectorStoreOut:
     name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
-    Selected embedding model
+    Selected embedding model.
     """
 
 
 @dataclass
 class Vector:
     """
     Canonical representation of document with embedding vector.
@@ -1345,15 +1377,15 @@
 class FetchVectorsIn:
     name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
-    Selected embedding model
+    Selected embedding model.
     """
     ids: List[str]
     """
     Document IDs to retrieve.
     """
 
 
@@ -1401,15 +1433,15 @@
 class UpdateVectorsIn:
     name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
-    Selected embedding model
+    Selected embedding model.
     """
     vectors: List[UpdateVectorParams]
     """
     Vectors to upsert.
     """
 
 
@@ -1417,15 +1449,15 @@
 class DeleteVectorsIn:
     name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
-    Selected embedding model
+    Selected embedding model.
     """
     ids: List[str]
     """
     Document IDs to delete.
     """
 
 
@@ -1433,31 +1465,31 @@
 class QueryVectorStoreIn:
     name: str
     """
     Vector store to query against.
     """
     model: Literal["jina-v2", "clip"]
     """
-    Selected embedding model
+    Selected embedding model.
     """
-    query_ids: Optional[List[str]] = None
+    query_strings: Optional[List[str]] = None
     """
-    Document IDs to use for the query.
+    Texts to embed and use for the query.
     """
     query_image_uris: Optional[List[str]] = None
     """
     Image URIs to embed and use for the query.
     """
     query_vectors: Optional[List[List[float]]] = None
     """
-    Vector to use for the query.
+    Vectors to use for the query.
     """
-    query_strings: Optional[List[str]] = None
+    query_ids: Optional[List[str]] = None
     """
-    Texts to embed and use for the query.
+    Document IDs to use for the query.
     """
     top_k: int = 10
     """
     Number of results to return.
     """
     ef_search: int = 40
     """
@@ -1509,13 +1541,13 @@
     """
     name: Optional[str] = None
     """
     Vector store name.
     """
     model: Optional[Literal["jina-v2", "clip"]] = None
     """
-    Selected embedding model
+    Selected embedding model.
     """
     metric: Optional[Literal["cosine", "l2", "inner"]] = None
     """
     The distance metric used for the query.
     """
```

### Comparing `substrate-120240411.0.5/substrate/future_dataclass_models.py` & `substrate-120240416.0.5/substrate/future_dataclass_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,20 +124,25 @@
 
 @dataclass
 class FutureMultiGenerateTextIn:
     """
     (Future reference)
     """
 
-    prompt: str
+    prompt: Optional[str] = None
     """
     (Future reference)
     Input prompt.
     """
-    num_choices: int
+    batch_prompts: Optional[List[str]] = None
+    """
+    (Future reference)
+    Batch input prompts.
+    """
+    num_choices: int = 1
     """
     (Future reference)
     Number of choices to generate.
     """
     temperature: float = 0.4
     """
     (Future reference)
@@ -152,43 +157,61 @@
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
-class FutureMultiGenerateTextOut:
+class MultiGenerateTextOutput:
     """
     (Future reference)
     """
 
     choices: List[FutureGenerateTextOut]
     """
     (Future reference)
     Response choices.
     """
 
 
 @dataclass
-class FutureMultiGenerateJSONIn:
+class FutureMultiGenerateTextOut:
     """
     (Future reference)
     """
 
-    prompt: str
+    outputs: List[MultiGenerateTextOutput]
     """
     (Future reference)
-    Input prompt.
+    A single output for `prompt`, or multiple outputs for `batch_prompts`.
     """
+
+
+@dataclass
+class FutureMultiGenerateJSONIn:
+    """
+    (Future reference)
+    """
+
     json_schema: Dict[str, Any]
     """
     (Future reference)
     JSON schema to guide `json_object` response.
     """
-    num_choices: int
+    prompt: Optional[str] = None
+    """
+    (Future reference)
+    Input prompt.
+    """
+    batch_prompts: Optional[List[str]] = None
+    """
+    (Future reference)
+    Batch input prompts.
+    """
+    num_choices: int = 2
     """
     (Future reference)
     Number of choices to generate.
     """
     temperature: float = 0.4
     """
     (Future reference)
@@ -203,47 +226,65 @@
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
-class FutureMultiGenerateJSONOut:
+class MultiGenerateJSONOutput:
     """
     (Future reference)
     """
 
     choices: List[FutureGenerateJSONOut]
     """
     (Future reference)
     Response choices.
     """
 
 
 @dataclass
+class FutureMultiGenerateJSONOut:
+    """
+    (Future reference)
+    """
+
+    outputs: List[MultiGenerateJSONOutput]
+    """
+    (Future reference)
+    A single output for `prompt`, or multiple outputs for `batch_prompts`.
+    """
+
+
+@dataclass
 class FutureMistral7BInstructIn:
     """
     (Future reference)
     """
 
-    prompt: str
+    prompt: Optional[str] = None
     """
     (Future reference)
     Input prompt.
     """
-    num_choices: int
+    num_choices: int = 1
     """
     (Future reference)
     Number of choices to generate.
     """
     json_schema: Optional[Dict[str, Any]] = None
     """
     (Future reference)
     JSON schema to guide response.
     """
+    batch_prompts: Optional[List[str]] = None
+    """
+    (Future reference)
+    Batch input prompts.
+    """
     temperature: Optional[float] = None
     """
     (Future reference)
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
@@ -267,27 +308,40 @@
     """
     (Future reference)
     JSON response, if `json_schema` was provided.
     """
 
 
 @dataclass
-class FutureMistral7BInstructOut:
+class Mistral7BInstructOutput:
     """
     (Future reference)
     """
 
     choices: List[Mistral7BInstructChoice]
     """
     (Future reference)
     Response choices.
     """
 
 
 @dataclass
+class FutureMistral7BInstructOut:
+    """
+    (Future reference)
+    """
+
+    outputs: List[Mistral7BInstructOutput]
+    """
+    (Future reference)
+    A single output for `prompt`, or multiple outputs for `batch_prompts`.
+    """
+
+
+@dataclass
 class FutureGenerateTextVisionIn:
     """
     (Future reference)
     """
 
     prompt: str
     """
@@ -543,20 +597,20 @@
     Number of images to generate.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    height: Optional[int] = None
+    height: int = 1024
     """
     (Future reference)
     Height of output image, in pixels.
     """
-    width: Optional[int] = None
+    width: int = 1024
     """
     (Future reference)
     Width of output image, in pixels.
     """
     seeds: Optional[List[int]] = None
     """
     (Future reference)
@@ -594,35 +648,35 @@
     Number of images to generate.
     """
     image_prompt_uri: Optional[str] = None
     """
     (Future reference)
     Image prompt.
     """
-    ip_adapter_scale: Optional[float] = None
+    ip_adapter_scale: float = 0.5
     """
     (Future reference)
     Controls the influence of the image prompt on the generated output.
     """
     negative_prompt: Optional[str] = None
     """
     (Future reference)
     Negative input prompt.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    width: Optional[int] = None
+    width: int = 1024
     """
     (Future reference)
     Width of output image, in pixels.
     """
-    height: Optional[int] = None
+    height: int = 1024
     """
     (Future reference)
     Height of output image, in pixels.
     """
     seeds: Optional[List[int]] = None
     """
     (Future reference)
@@ -680,15 +734,15 @@
     Negative input prompt.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    conditioning_scale: Optional[float] = None
+    conditioning_scale: float = 0.5
     """
     (Future reference)
     Controls the influence of the input image on the generated output.
     """
     seeds: Optional[List[int]] = None
     """
     (Future reference)
@@ -843,15 +897,15 @@
     Negative input prompt.
     """
     store: Optional[str] = None
     """
     (Future reference)
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
     """
-    strength: float = 1
+    strength: float = 0.8
     """
     (Future reference)
     Controls the strength of the generation process.
     """
     seeds: Optional[List[int]] = None
     """
     (Future reference)
@@ -1747,19 +1801,14 @@
     """
 
     items: List[EmbedTextOrImageItem]
     """
     (Future reference)
     Items to embed.
     """
-    embedded_metadata_keys: Optional[List[str]] = None
-    """
-    (Future reference)
-    Choose keys from `metadata` to embed with text, when embedding and storing text documents.
-    """
     store: Optional[str] = None
     """
     (Future reference)
     [Vector store](/docs/vector-stores) identifier.
     """
 
 
@@ -1786,15 +1835,15 @@
     """
     (Future reference)
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     (Future reference)
-    Selected embedding model
+    Selected embedding model.
     """
     m: int = 16
     """
     (Future reference)
     The max number of connections per layer for the index.
     """
     ef_construction: int = 64
@@ -1819,15 +1868,15 @@
     """
     (Future reference)
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     (Future reference)
-    Selected embedding model
+    Selected embedding model.
     """
     m: int
     """
     (Future reference)
     The max number of connections per layer for the index.
     """
     ef_construction: int
@@ -1874,15 +1923,15 @@
     """
     (Future reference)
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     (Future reference)
-    Selected embedding model
+    Selected embedding model.
     """
 
 
 @dataclass
 class FutureDeleteVectorStoreOut:
     """
     (Future reference)
@@ -1892,15 +1941,15 @@
     """
     (Future reference)
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     (Future reference)
-    Selected embedding model
+    Selected embedding model.
     """
 
 
 @dataclass
 class Vector:
     """
     (Future reference)
@@ -1934,15 +1983,15 @@
     """
     (Future reference)
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     (Future reference)
-    Selected embedding model
+    Selected embedding model.
     """
     ids: List[str]
     """
     (Future reference)
     Document IDs to retrieve.
     """
 
@@ -2019,15 +2068,15 @@
     """
     (Future reference)
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     (Future reference)
-    Selected embedding model
+    Selected embedding model.
     """
     vectors: List[UpdateVectorParams]
     """
     (Future reference)
     Vectors to upsert.
     """
 
@@ -2042,15 +2091,15 @@
     """
     (Future reference)
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     (Future reference)
-    Selected embedding model
+    Selected embedding model.
     """
     ids: List[str]
     """
     (Future reference)
     Document IDs to delete.
     """
 
@@ -2065,35 +2114,35 @@
     """
     (Future reference)
     Vector store to query against.
     """
     model: Literal["jina-v2", "clip"]
     """
     (Future reference)
-    Selected embedding model
+    Selected embedding model.
     """
-    query_ids: Optional[List[str]] = None
+    query_strings: Optional[List[str]] = None
     """
     (Future reference)
-    Document IDs to use for the query.
+    Texts to embed and use for the query.
     """
     query_image_uris: Optional[List[str]] = None
     """
     (Future reference)
     Image URIs to embed and use for the query.
     """
     query_vectors: Optional[List[List[float]]] = None
     """
     (Future reference)
-    Vector to use for the query.
+    Vectors to use for the query.
     """
-    query_strings: Optional[List[str]] = None
+    query_ids: Optional[List[str]] = None
     """
     (Future reference)
-    Texts to embed and use for the query.
+    Document IDs to use for the query.
     """
     top_k: int = 10
     """
     (Future reference)
     Number of results to return.
     """
     ef_search: int = 40
@@ -2166,14 +2215,14 @@
     """
     (Future reference)
     Vector store name.
     """
     model: Optional[Literal["jina-v2", "clip"]] = None
     """
     (Future reference)
-    Selected embedding model
+    Selected embedding model.
     """
     metric: Optional[Literal["cosine", "l2", "inner"]] = None
     """
     (Future reference)
     The distance metric used for the query.
     """
```

### Comparing `substrate-120240411.0.5/substrate/nodes.py` & `substrate-120240416.0.5/substrate/nodes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 ꩜ Substrate
 @GENERATED FILE
-20240411.20240414
+20240416.20240416
 """
+from typing import Type
 
-from .substrate import SubstrateResponse
 from .core.corenode import CoreNode
 from .dataclass_models import (
     CLIPOut,
     JinaV2Out,
     XTTSV2Out,
     BigLaMaOut,
     DISISNetOut,
@@ -148,30 +148,17 @@
         Output fields: `future.text` (optional)
 
         https://substrate.run/library#GenerateText
         """
         super().__init__(**args)
         self.node = "GenerateText"
 
-    def output(self, response: SubstrateResponse) -> GenerateTextOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.text` (optional)
-
-        https://substrate.run/library#GenerateText
-        """
-        klass = GenerateTextOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[GenerateTextOut]:
+        return GenerateTextOut
 
     @property
     def future(self) -> FutureGenerateTextOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.text` (optional)
@@ -186,46 +173,33 @@
     Generate multiple text choices using a language model.
 
     https://substrate.run/library#MultiGenerateText
     """
 
     def __init__(self, args: MultiGenerateTextIn):
         """
-        Input arguments: `prompt`, `num_choices`, `temperature` (optional), `max_tokens` (optional), `node` (optional)
+        Input arguments: `prompt` (optional), `batch_prompts` (optional), `num_choices` (optional), `temperature` (optional), `max_tokens` (optional), `node` (optional)
 
-        Output fields: `future.choices`
+        Output fields: `future.outputs`
 
         https://substrate.run/library#MultiGenerateText
         """
         super().__init__(**args)
         self.node = "MultiGenerateText"
 
-    def output(self, response: SubstrateResponse) -> MultiGenerateTextOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.choices`
-
-        https://substrate.run/library#MultiGenerateText
-        """
-        klass = MultiGenerateTextOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[MultiGenerateTextOut]:
+        return MultiGenerateTextOut
 
     @property
     def future(self) -> FutureMultiGenerateTextOut:  # type: ignore
         """
         Future reference to this node's output.
 
-        Output fields: `future.choices`
+        Output fields: `future.outputs`
 
         https://substrate.run/library#MultiGenerateText
         """
         return super().future  # type: ignore
 
 
 class GenerateJSON(CoreNode):
@@ -242,30 +216,17 @@
         Output fields: `future.json_object` (optional)
 
         https://substrate.run/library#GenerateJSON
         """
         super().__init__(**args)
         self.node = "GenerateJSON"
 
-    def output(self, response: SubstrateResponse) -> GenerateJSONOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.json_object` (optional)
-
-        https://substrate.run/library#GenerateJSON
-        """
-        klass = GenerateJSONOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[GenerateJSONOut]:
+        return GenerateJSONOut
 
     @property
     def future(self) -> FutureGenerateJSONOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.json_object` (optional)
@@ -280,46 +241,33 @@
     Generate multiple JSON choices using a language model.
 
     https://substrate.run/library#MultiGenerateJSON
     """
 
     def __init__(self, args: MultiGenerateJSONIn):
         """
-        Input arguments: `prompt`, `json_schema`, `num_choices`, `temperature` (optional), `max_tokens` (optional), `node` (optional)
+        Input arguments: `prompt` (optional), `json_schema`, `batch_prompts` (optional), `num_choices` (optional), `temperature` (optional), `max_tokens` (optional), `node` (optional)
 
-        Output fields: `future.choices`
+        Output fields: `future.outputs`
 
         https://substrate.run/library#MultiGenerateJSON
         """
         super().__init__(**args)
         self.node = "MultiGenerateJSON"
 
-    def output(self, response: SubstrateResponse) -> MultiGenerateJSONOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.choices`
-
-        https://substrate.run/library#MultiGenerateJSON
-        """
-        klass = MultiGenerateJSONOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[MultiGenerateJSONOut]:
+        return MultiGenerateJSONOut
 
     @property
     def future(self) -> FutureMultiGenerateJSONOut:  # type: ignore
         """
         Future reference to this node's output.
 
-        Output fields: `future.choices`
+        Output fields: `future.outputs`
 
         https://substrate.run/library#MultiGenerateJSON
         """
         return super().future  # type: ignore
 
 
 class GenerateTextVision(CoreNode):
@@ -336,30 +284,17 @@
         Output fields: `future.text`
 
         https://substrate.run/library#GenerateTextVision
         """
         super().__init__(**args)
         self.node = "GenerateTextVision"
 
-    def output(self, response: SubstrateResponse) -> GenerateTextVisionOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.text`
-
-        https://substrate.run/library#GenerateTextVision
-        """
-        klass = GenerateTextVisionOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[GenerateTextVisionOut]:
+        return GenerateTextVisionOut
 
     @property
     def future(self) -> FutureGenerateTextVisionOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.text`
@@ -374,46 +309,33 @@
     Generate text using [Mistral 7B Instruct](https://mistral.ai/news/announcing-mistral-7b).
 
     https://substrate.run/library#Mistral7BInstruct
     """
 
     def __init__(self, args: Mistral7BInstructIn):
         """
-        Input arguments: `prompt`, `num_choices`, `json_schema` (optional), `temperature` (optional), `max_tokens` (optional)
+        Input arguments: `prompt` (optional), `num_choices` (optional), `json_schema` (optional), `batch_prompts` (optional), `temperature` (optional), `max_tokens` (optional)
 
-        Output fields: `future.choices`
+        Output fields: `future.outputs`
 
         https://substrate.run/library#Mistral7BInstruct
         """
         super().__init__(**args)
         self.node = "Mistral7BInstruct"
 
-    def output(self, response: SubstrateResponse) -> Mistral7BInstructOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.choices`
-
-        https://substrate.run/library#Mistral7BInstruct
-        """
-        klass = Mistral7BInstructOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[Mistral7BInstructOut]:
+        return Mistral7BInstructOut
 
     @property
     def future(self) -> FutureMistral7BInstructOut:  # type: ignore
         """
         Future reference to this node's output.
 
-        Output fields: `future.choices`
+        Output fields: `future.outputs`
 
         https://substrate.run/library#Mistral7BInstruct
         """
         return super().future  # type: ignore
 
 
 class Firellava13B(CoreNode):
@@ -430,30 +352,17 @@
         Output fields: `future.text`
 
         https://substrate.run/library#Firellava13B
         """
         super().__init__(**args)
         self.node = "Firellava13B"
 
-    def output(self, response: SubstrateResponse) -> Firellava13BOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.text`
-
-        https://substrate.run/library#Firellava13B
-        """
-        klass = Firellava13BOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[Firellava13BOut]:
+        return Firellava13BOut
 
     @property
     def future(self) -> FutureFirellava13BOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.text`
@@ -477,30 +386,17 @@
         Output fields: `future.image_uri`
 
         https://substrate.run/library#GenerateImage
         """
         super().__init__(**args)
         self.node = "GenerateImage"
 
-    def output(self, response: SubstrateResponse) -> GenerateImageOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.image_uri`
-
-        https://substrate.run/library#GenerateImage
-        """
-        klass = GenerateImageOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[GenerateImageOut]:
+        return GenerateImageOut
 
     @property
     def future(self) -> FutureGenerateImageOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.image_uri`
@@ -524,30 +420,17 @@
         Output fields: `future.outputs`
 
         https://substrate.run/library#MultiGenerateImage
         """
         super().__init__(**args)
         self.node = "MultiGenerateImage"
 
-    def output(self, response: SubstrateResponse) -> MultiGenerateImageOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.outputs`
-
-        https://substrate.run/library#MultiGenerateImage
-        """
-        klass = MultiGenerateImageOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[MultiGenerateImageOut]:
+        return MultiGenerateImageOut
 
     @property
     def future(self) -> FutureMultiGenerateImageOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.outputs`
@@ -571,30 +454,17 @@
         Output fields: `future.image_uri`
 
         https://substrate.run/library#GenerativeEditImage
         """
         super().__init__(**args)
         self.node = "GenerativeEditImage"
 
-    def output(self, response: SubstrateResponse) -> GenerativeEditImageOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.image_uri`
-
-        https://substrate.run/library#GenerativeEditImage
-        """
-        klass = GenerativeEditImageOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[GenerativeEditImageOut]:
+        return GenerativeEditImageOut
 
     @property
     def future(self) -> FutureGenerativeEditImageOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.image_uri`
@@ -618,30 +488,17 @@
         Output fields: `future.outputs`
 
         https://substrate.run/library#MultiGenerativeEditImage
         """
         super().__init__(**args)
         self.node = "MultiGenerativeEditImage"
 
-    def output(self, response: SubstrateResponse) -> MultiGenerativeEditImageOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.outputs`
-
-        https://substrate.run/library#MultiGenerativeEditImage
-        """
-        klass = MultiGenerativeEditImageOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[MultiGenerativeEditImageOut]:
+        return MultiGenerativeEditImageOut
 
     @property
     def future(self) -> FutureMultiGenerativeEditImageOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.outputs`
@@ -665,30 +522,17 @@
         Output fields: `future.outputs`
 
         https://substrate.run/library#StableDiffusionXL
         """
         super().__init__(**args)
         self.node = "StableDiffusionXL"
 
-    def output(self, response: SubstrateResponse) -> StableDiffusionXLOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.outputs`
-
-        https://substrate.run/library#StableDiffusionXL
-        """
-        klass = StableDiffusionXLOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[StableDiffusionXLOut]:
+        return StableDiffusionXLOut
 
     @property
     def future(self) -> FutureStableDiffusionXLOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.outputs`
@@ -712,30 +556,17 @@
         Output fields: `future.outputs`
 
         https://substrate.run/library#StableDiffusionXLLightning
         """
         super().__init__(**args)
         self.node = "StableDiffusionXLLightning"
 
-    def output(self, response: SubstrateResponse) -> StableDiffusionXLLightningOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.outputs`
-
-        https://substrate.run/library#StableDiffusionXLLightning
-        """
-        klass = StableDiffusionXLLightningOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[StableDiffusionXLLightningOut]:
+        return StableDiffusionXLLightningOut
 
     @property
     def future(self) -> FutureStableDiffusionXLLightningOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.outputs`
@@ -759,30 +590,17 @@
         Output fields: `future.outputs`
 
         https://substrate.run/library#StableDiffusionXLInpaint
         """
         super().__init__(**args)
         self.node = "StableDiffusionXLInpaint"
 
-    def output(self, response: SubstrateResponse) -> StableDiffusionXLInpaintOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.outputs`
-
-        https://substrate.run/library#StableDiffusionXLInpaint
-        """
-        klass = StableDiffusionXLInpaintOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[StableDiffusionXLInpaintOut]:
+        return StableDiffusionXLInpaintOut
 
     @property
     def future(self) -> FutureStableDiffusionXLInpaintOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.outputs`
@@ -806,30 +624,17 @@
         Output fields: `future.outputs`
 
         https://substrate.run/library#StableDiffusionXLControlNet
         """
         super().__init__(**args)
         self.node = "StableDiffusionXLControlNet"
 
-    def output(self, response: SubstrateResponse) -> StableDiffusionXLControlNetOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.outputs`
-
-        https://substrate.run/library#StableDiffusionXLControlNet
-        """
-        klass = StableDiffusionXLControlNetOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[StableDiffusionXLControlNetOut]:
+        return StableDiffusionXLControlNetOut
 
     @property
     def future(self) -> FutureStableDiffusionXLControlNetOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.outputs`
@@ -853,30 +658,17 @@
         Output fields: `future.outputs`
 
         https://substrate.run/library#StableDiffusionXLIPAdapter
         """
         super().__init__(**args)
         self.node = "StableDiffusionXLIPAdapter"
 
-    def output(self, response: SubstrateResponse) -> StableDiffusionXLIPAdapterOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.outputs`
-
-        https://substrate.run/library#StableDiffusionXLIPAdapter
-        """
-        klass = StableDiffusionXLIPAdapterOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[StableDiffusionXLIPAdapterOut]:
+        return StableDiffusionXLIPAdapterOut
 
     @property
     def future(self) -> FutureStableDiffusionXLIPAdapterOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.outputs`
@@ -900,30 +692,17 @@
         Output fields: `future.text`, `future.segments` (optional), `future.chapters` (optional)
 
         https://substrate.run/library#TranscribeMedia
         """
         super().__init__(**args)
         self.node = "TranscribeMedia"
 
-    def output(self, response: SubstrateResponse) -> TranscribeMediaOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.text`, `future.segments` (optional), `future.chapters` (optional)
-
-        https://substrate.run/library#TranscribeMedia
-        """
-        klass = TranscribeMediaOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[TranscribeMediaOut]:
+        return TranscribeMediaOut
 
     @property
     def future(self) -> FutureTranscribeMediaOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.text`, `future.segments` (optional), `future.chapters` (optional)
@@ -947,30 +726,17 @@
         Output fields: `future.audio_uri`
 
         https://substrate.run/library#GenerateSpeech
         """
         super().__init__(**args)
         self.node = "GenerateSpeech"
 
-    def output(self, response: SubstrateResponse) -> GenerateSpeechOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.audio_uri`
-
-        https://substrate.run/library#GenerateSpeech
-        """
-        klass = GenerateSpeechOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[GenerateSpeechOut]:
+        return GenerateSpeechOut
 
     @property
     def future(self) -> FutureGenerateSpeechOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.audio_uri`
@@ -994,30 +760,17 @@
         Output fields: `future.audio_uri`
 
         https://substrate.run/library#XTTSV2
         """
         super().__init__(**args)
         self.node = "XTTSV2"
 
-    def output(self, response: SubstrateResponse) -> XTTSV2Out:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.audio_uri`
-
-        https://substrate.run/library#XTTSV2
-        """
-        klass = XTTSV2Out
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[XTTSV2Out]:
+        return XTTSV2Out
 
     @property
     def future(self) -> FutureXTTSV2Out:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.audio_uri`
@@ -1041,30 +794,17 @@
         Output fields: `future.image_uri`
 
         https://substrate.run/library#RemoveBackground
         """
         super().__init__(**args)
         self.node = "RemoveBackground"
 
-    def output(self, response: SubstrateResponse) -> RemoveBackgroundOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.image_uri`
-
-        https://substrate.run/library#RemoveBackground
-        """
-        klass = RemoveBackgroundOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[RemoveBackgroundOut]:
+        return RemoveBackgroundOut
 
     @property
     def future(self) -> FutureRemoveBackgroundOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.image_uri`
@@ -1088,30 +828,17 @@
         Output fields: `future.image_uri`
 
         https://substrate.run/library#FillMask
         """
         super().__init__(**args)
         self.node = "FillMask"
 
-    def output(self, response: SubstrateResponse) -> FillMaskOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.image_uri`
-
-        https://substrate.run/library#FillMask
-        """
-        klass = FillMaskOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[FillMaskOut]:
+        return FillMaskOut
 
     @property
     def future(self) -> FutureFillMaskOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.image_uri`
@@ -1135,30 +862,17 @@
         Output fields: `future.image_uri`
 
         https://substrate.run/library#UpscaleImage
         """
         super().__init__(**args)
         self.node = "UpscaleImage"
 
-    def output(self, response: SubstrateResponse) -> UpscaleImageOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.image_uri`
-
-        https://substrate.run/library#UpscaleImage
-        """
-        klass = UpscaleImageOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[UpscaleImageOut]:
+        return UpscaleImageOut
 
     @property
     def future(self) -> FutureUpscaleImageOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.image_uri`
@@ -1182,30 +896,17 @@
         Output fields: `future.mask_image_uri`
 
         https://substrate.run/library#SegmentUnderPoint
         """
         super().__init__(**args)
         self.node = "SegmentUnderPoint"
 
-    def output(self, response: SubstrateResponse) -> SegmentUnderPointOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.mask_image_uri`
-
-        https://substrate.run/library#SegmentUnderPoint
-        """
-        klass = SegmentUnderPointOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[SegmentUnderPointOut]:
+        return SegmentUnderPointOut
 
     @property
     def future(self) -> FutureSegmentUnderPointOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.mask_image_uri`
@@ -1229,30 +930,17 @@
         Output fields: `future.image_uri`
 
         https://substrate.run/library#DISISNet
         """
         super().__init__(**args)
         self.node = "DISISNet"
 
-    def output(self, response: SubstrateResponse) -> DISISNetOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.image_uri`
-
-        https://substrate.run/library#DISISNet
-        """
-        klass = DISISNetOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[DISISNetOut]:
+        return DISISNetOut
 
     @property
     def future(self) -> FutureDISISNetOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.image_uri`
@@ -1276,30 +964,17 @@
         Output fields: `future.image_uri`
 
         https://substrate.run/library#BigLaMa
         """
         super().__init__(**args)
         self.node = "BigLaMa"
 
-    def output(self, response: SubstrateResponse) -> BigLaMaOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.image_uri`
-
-        https://substrate.run/library#BigLaMa
-        """
-        klass = BigLaMaOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[BigLaMaOut]:
+        return BigLaMaOut
 
     @property
     def future(self) -> FutureBigLaMaOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.image_uri`
@@ -1323,30 +998,17 @@
         Output fields: `future.image_uri`
 
         https://substrate.run/library#RealESRGAN
         """
         super().__init__(**args)
         self.node = "RealESRGAN"
 
-    def output(self, response: SubstrateResponse) -> RealESRGANOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.image_uri`
-
-        https://substrate.run/library#RealESRGAN
-        """
-        klass = RealESRGANOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[RealESRGANOut]:
+        return RealESRGANOut
 
     @property
     def future(self) -> FutureRealESRGANOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.image_uri`
@@ -1370,30 +1032,17 @@
         Output fields: `future.mask_image_uri`
 
         https://substrate.run/library#SegmentAnything
         """
         super().__init__(**args)
         self.node = "SegmentAnything"
 
-    def output(self, response: SubstrateResponse) -> SegmentAnythingOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.mask_image_uri`
-
-        https://substrate.run/library#SegmentAnything
-        """
-        klass = SegmentAnythingOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[SegmentAnythingOut]:
+        return SegmentAnythingOut
 
     @property
     def future(self) -> FutureSegmentAnythingOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.mask_image_uri`
@@ -1417,30 +1066,17 @@
         Output fields: `future.embedding`
 
         https://substrate.run/library#EmbedText
         """
         super().__init__(**args)
         self.node = "EmbedText"
 
-    def output(self, response: SubstrateResponse) -> EmbedTextOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.embedding`
-
-        https://substrate.run/library#EmbedText
-        """
-        klass = EmbedTextOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[EmbedTextOut]:
+        return EmbedTextOut
 
     @property
     def future(self) -> FutureEmbedTextOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.embedding`
@@ -1464,30 +1100,17 @@
         Output fields: `future.embeddings`
 
         https://substrate.run/library#MultiEmbedText
         """
         super().__init__(**args)
         self.node = "MultiEmbedText"
 
-    def output(self, response: SubstrateResponse) -> MultiEmbedTextOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.embeddings`
-
-        https://substrate.run/library#MultiEmbedText
-        """
-        klass = MultiEmbedTextOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[MultiEmbedTextOut]:
+        return MultiEmbedTextOut
 
     @property
     def future(self) -> FutureMultiEmbedTextOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.embeddings`
@@ -1511,30 +1134,17 @@
         Output fields: `future.embedding`
 
         https://substrate.run/library#EmbedImage
         """
         super().__init__(**args)
         self.node = "EmbedImage"
 
-    def output(self, response: SubstrateResponse) -> EmbedImageOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.embedding`
-
-        https://substrate.run/library#EmbedImage
-        """
-        klass = EmbedImageOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[EmbedImageOut]:
+        return EmbedImageOut
 
     @property
     def future(self) -> FutureEmbedImageOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.embedding`
@@ -1558,30 +1168,17 @@
         Output fields: `future.embeddings`
 
         https://substrate.run/library#MultiEmbedImage
         """
         super().__init__(**args)
         self.node = "MultiEmbedImage"
 
-    def output(self, response: SubstrateResponse) -> MultiEmbedImageOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.embeddings`
-
-        https://substrate.run/library#MultiEmbedImage
-        """
-        klass = MultiEmbedImageOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[MultiEmbedImageOut]:
+        return MultiEmbedImageOut
 
     @property
     def future(self) -> FutureMultiEmbedImageOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.embeddings`
@@ -1605,30 +1202,17 @@
         Output fields: `future.embeddings`
 
         https://substrate.run/library#JinaV2
         """
         super().__init__(**args)
         self.node = "JinaV2"
 
-    def output(self, response: SubstrateResponse) -> JinaV2Out:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.embeddings`
-
-        https://substrate.run/library#JinaV2
-        """
-        klass = JinaV2Out
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[JinaV2Out]:
+        return JinaV2Out
 
     @property
     def future(self) -> FutureJinaV2Out:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.embeddings`
@@ -1643,39 +1227,26 @@
     Generate embeddings for text or images using [CLIP](https://openai.com/research/clip).
 
     https://substrate.run/library#CLIP
     """
 
     def __init__(self, args: CLIPIn):
         """
-        Input arguments: `items`, `embedded_metadata_keys` (optional), `store` (optional)
+        Input arguments: `items`, `store` (optional)
 
         Output fields: `future.embeddings`
 
         https://substrate.run/library#CLIP
         """
         super().__init__(**args)
         self.node = "CLIP"
 
-    def output(self, response: SubstrateResponse) -> CLIPOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.embeddings`
-
-        https://substrate.run/library#CLIP
-        """
-        klass = CLIPOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[CLIPOut]:
+        return CLIPOut
 
     @property
     def future(self) -> FutureCLIPOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.embeddings`
@@ -1699,30 +1270,17 @@
         Output fields: `future.name`, `future.model`, `future.m`, `future.ef_construction`, `future.metric`
 
         https://substrate.run/library#CreateVectorStore
         """
         super().__init__(**args)
         self.node = "CreateVectorStore"
 
-    def output(self, response: SubstrateResponse) -> CreateVectorStoreOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.name`, `future.model`, `future.m`, `future.ef_construction`, `future.metric`
-
-        https://substrate.run/library#CreateVectorStore
-        """
-        klass = CreateVectorStoreOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[CreateVectorStoreOut]:
+        return CreateVectorStoreOut
 
     @property
     def future(self) -> FutureCreateVectorStoreOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.name`, `future.model`, `future.m`, `future.ef_construction`, `future.metric`
@@ -1746,30 +1304,17 @@
         Output fields: `future.stores` (optional)
 
         https://substrate.run/library#ListVectorStores
         """
         super().__init__(**args)
         self.node = "ListVectorStores"
 
-    def output(self, response: SubstrateResponse) -> ListVectorStoresOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.stores` (optional)
-
-        https://substrate.run/library#ListVectorStores
-        """
-        klass = ListVectorStoresOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[ListVectorStoresOut]:
+        return ListVectorStoresOut
 
     @property
     def future(self) -> FutureListVectorStoresOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.stores` (optional)
@@ -1793,30 +1338,17 @@
         Output fields: `future.name`, `future.model`
 
         https://substrate.run/library#DeleteVectorStore
         """
         super().__init__(**args)
         self.node = "DeleteVectorStore"
 
-    def output(self, response: SubstrateResponse) -> DeleteVectorStoreOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.name`, `future.model`
-
-        https://substrate.run/library#DeleteVectorStore
-        """
-        klass = DeleteVectorStoreOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[DeleteVectorStoreOut]:
+        return DeleteVectorStoreOut
 
     @property
     def future(self) -> FutureDeleteVectorStoreOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.name`, `future.model`
@@ -1831,39 +1363,26 @@
     Query a vector store for similar vectors.
 
     https://substrate.run/library#QueryVectorStore
     """
 
     def __init__(self, args: QueryVectorStoreIn):
         """
-        Input arguments: `name`, `model`, `query_ids` (optional), `query_image_uris` (optional), `query_vectors` (optional), `query_strings` (optional), `top_k` (optional), `ef_search` (optional), `include_values` (optional), `include_metadata` (optional), `filters` (optional), `metric` (optional)
+        Input arguments: `name`, `model`, `query_strings` (optional), `query_image_uris` (optional), `query_vectors` (optional), `query_ids` (optional), `top_k` (optional), `ef_search` (optional), `include_values` (optional), `include_metadata` (optional), `filters` (optional), `metric` (optional)
 
         Output fields: `future.results`, `future.name` (optional), `future.model` (optional), `future.metric` (optional)
 
         https://substrate.run/library#QueryVectorStore
         """
         super().__init__(**args)
         self.node = "QueryVectorStore"
 
-    def output(self, response: SubstrateResponse) -> QueryVectorStoreOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.results`, `future.name` (optional), `future.model` (optional), `future.metric` (optional)
-
-        https://substrate.run/library#QueryVectorStore
-        """
-        klass = QueryVectorStoreOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[QueryVectorStoreOut]:
+        return QueryVectorStoreOut
 
     @property
     def future(self) -> FutureQueryVectorStoreOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.results`, `future.name` (optional), `future.model` (optional), `future.metric` (optional)
@@ -1887,30 +1406,17 @@
         Output fields: `future.vectors`
 
         https://substrate.run/library#FetchVectors
         """
         super().__init__(**args)
         self.node = "FetchVectors"
 
-    def output(self, response: SubstrateResponse) -> FetchVectorsOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.vectors`
-
-        https://substrate.run/library#FetchVectors
-        """
-        klass = FetchVectorsOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[FetchVectorsOut]:
+        return FetchVectorsOut
 
     @property
     def future(self) -> FutureFetchVectorsOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.vectors`
@@ -1934,30 +1440,17 @@
         Output fields: `future.count`
 
         https://substrate.run/library#UpdateVectors
         """
         super().__init__(**args)
         self.node = "UpdateVectors"
 
-    def output(self, response: SubstrateResponse) -> UpdateVectorsOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.count`
-
-        https://substrate.run/library#UpdateVectors
-        """
-        klass = UpdateVectorsOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[UpdateVectorsOut]:
+        return UpdateVectorsOut
 
     @property
     def future(self) -> FutureUpdateVectorsOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.count`
@@ -1981,30 +1474,17 @@
         Output fields: `future.count`
 
         https://substrate.run/library#DeleteVectors
         """
         super().__init__(**args)
         self.node = "DeleteVectors"
 
-    def output(self, response: SubstrateResponse) -> DeleteVectorsOut:
-        """
-        Retrieve this node's output from a response.
-
-        Output fields: `future.count`
-
-        https://substrate.run/library#DeleteVectors
-        """
-        klass = DeleteVectorsOut
-        json = response.api_response.json
-        if json and json.get("data"):
-            data = json["data"]
-            node_id = self.id
-            if data.get(self.id):
-                return klass(**data[self.id])
-        raise ValueError(f"Node {self.id} not found in response")
+    @property
+    def out_type(self) -> Type[DeleteVectorsOut]:
+        return DeleteVectorsOut
 
     @property
     def future(self) -> FutureDeleteVectorsOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.count`
```

### Comparing `substrate-120240411.0.5/substrate/typeddict_models.py` & `substrate-120240416.0.5/substrate/typeddict_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,19 +81,23 @@
     (Optional) JSON response.
     """
 
 
 class MultiGenerateTextIn(TypedDict):
     prompt: NotRequired[str]
     """
-    Input prompt.
+    (Optional) Input prompt.
+    """
+    batch_prompts: NotRequired[List[str]]
+    """
+    (Optional) Batch input prompts.
     """
     num_choices: NotRequired[int]
     """
-    Number of choices to generate.
+    (Optional) Number of choices to generate.
     """
     temperature: NotRequired[float]
     """
     (Optional) Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: NotRequired[int]
     """
@@ -101,33 +105,44 @@
     """
     node: NotRequired[Literal["Mistral7BInstruct"]]
     """
     (Optional) Selected node.
     """
 
 
-class MultiGenerateTextOut(TypedDict):
+class MultiGenerateTextOutput(TypedDict):
     choices: NotRequired[List[GenerateTextOut]]
     """
     Response choices.
     """
 
 
+class MultiGenerateTextOut(TypedDict):
+    outputs: NotRequired[List[MultiGenerateTextOutput]]
+    """
+    A single output for `prompt`, or multiple outputs for `batch_prompts`.
+    """
+
+
 class MultiGenerateJSONIn(TypedDict):
     prompt: NotRequired[str]
     """
-    Input prompt.
+    (Optional) Input prompt.
     """
     json_schema: NotRequired[Dict[str, Any]]
     """
     JSON schema to guide `json_object` response.
     """
+    batch_prompts: NotRequired[List[str]]
+    """
+    (Optional) Batch input prompts.
+    """
     num_choices: NotRequired[int]
     """
-    Number of choices to generate.
+    (Optional) Number of choices to generate.
     """
     temperature: NotRequired[float]
     """
     (Optional) Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: NotRequired[int]
     """
@@ -135,34 +150,45 @@
     """
     node: NotRequired[Literal["Mistral7BInstruct"]]
     """
     (Optional) Selected node.
     """
 
 
-class MultiGenerateJSONOut(TypedDict):
+class MultiGenerateJSONOutput(TypedDict):
     choices: NotRequired[List[GenerateJSONOut]]
     """
     Response choices.
     """
 
 
+class MultiGenerateJSONOut(TypedDict):
+    outputs: NotRequired[List[MultiGenerateJSONOutput]]
+    """
+    A single output for `prompt`, or multiple outputs for `batch_prompts`.
+    """
+
+
 class Mistral7BInstructIn(TypedDict):
     prompt: NotRequired[str]
     """
-    Input prompt.
+    (Optional) Input prompt.
     """
     num_choices: NotRequired[int]
     """
-    Number of choices to generate.
+    (Optional) Number of choices to generate.
     """
     json_schema: NotRequired[Dict[str, Any]]
     """
     (Optional) JSON schema to guide response.
     """
+    batch_prompts: NotRequired[List[str]]
+    """
+    (Optional) Batch input prompts.
+    """
     temperature: NotRequired[float]
     """
     (Optional) Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: NotRequired[int]
     """
     (Optional) Maximum number of tokens to generate.
@@ -176,21 +202,28 @@
     """
     json_object: NotRequired[Dict[str, Any]]
     """
     (Optional) JSON response, if `json_schema` was provided.
     """
 
 
-class Mistral7BInstructOut(TypedDict):
+class Mistral7BInstructOutput(TypedDict):
     choices: NotRequired[List[Mistral7BInstructChoice]]
     """
     Response choices.
     """
 
 
+class Mistral7BInstructOut(TypedDict):
+    outputs: NotRequired[List[Mistral7BInstructOutput]]
+    """
+    A single output for `prompt`, or multiple outputs for `batch_prompts`.
+    """
+
+
 class GenerateTextVisionIn(TypedDict):
     prompt: NotRequired[str]
     """
     Text prompt.
     """
     image_uris: NotRequired[List[str]]
     """
@@ -1136,18 +1169,14 @@
 
 
 class CLIPIn(TypedDict):
     items: NotRequired[List[EmbedTextOrImageItem]]
     """
     Items to embed.
     """
-    embedded_metadata_keys: NotRequired[List[str]]
-    """
-    (Optional) Choose keys from `metadata` to embed with text, when embedding and storing text documents.
-    """
     store: NotRequired[str]
     """
     (Optional) [Vector store](/docs/vector-stores) identifier.
     """
 
 
 class CLIPOut(TypedDict):
@@ -1160,15 +1189,15 @@
 class CreateVectorStoreIn(TypedDict):
     name: NotRequired[str]
     """
     Vector store name.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
-    Selected embedding model
+    Selected embedding model.
     """
     m: NotRequired[int]
     """
     (Optional) The max number of connections per layer for the index.
     """
     ef_construction: NotRequired[int]
     """
@@ -1183,15 +1212,15 @@
 class CreateVectorStoreOut(TypedDict):
     name: NotRequired[str]
     """
     Vector store name.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
-    Selected embedding model
+    Selected embedding model.
     """
     m: NotRequired[int]
     """
     The max number of connections per layer for the index.
     """
     ef_construction: NotRequired[int]
     """
@@ -1217,26 +1246,26 @@
 class DeleteVectorStoreIn(TypedDict):
     name: NotRequired[str]
     """
     Vector store name.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
-    Selected embedding model
+    Selected embedding model.
     """
 
 
 class DeleteVectorStoreOut(TypedDict):
     name: NotRequired[str]
     """
     Vector store name.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
-    Selected embedding model
+    Selected embedding model.
     """
 
 
 class Vector(TypedDict):
     """
     Canonical representation of document with embedding vector.
     """
@@ -1258,15 +1287,15 @@
 class FetchVectorsIn(TypedDict):
     name: NotRequired[str]
     """
     Vector store name.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
-    Selected embedding model
+    Selected embedding model.
     """
     ids: NotRequired[List[str]]
     """
     Document IDs to retrieve.
     """
 
 
@@ -1309,61 +1338,61 @@
 class UpdateVectorsIn(TypedDict):
     name: NotRequired[str]
     """
     Vector store name.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
-    Selected embedding model
+    Selected embedding model.
     """
     vectors: NotRequired[List[UpdateVectorParams]]
     """
     Vectors to upsert.
     """
 
 
 class DeleteVectorsIn(TypedDict):
     name: NotRequired[str]
     """
     Vector store name.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
-    Selected embedding model
+    Selected embedding model.
     """
     ids: NotRequired[List[str]]
     """
     Document IDs to delete.
     """
 
 
 class QueryVectorStoreIn(TypedDict):
     name: NotRequired[str]
     """
     Vector store to query against.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
-    Selected embedding model
+    Selected embedding model.
     """
-    query_ids: NotRequired[List[str]]
+    query_strings: NotRequired[List[str]]
     """
-    (Optional) Document IDs to use for the query.
+    (Optional) Texts to embed and use for the query.
     """
     query_image_uris: NotRequired[List[str]]
     """
     (Optional) Image URIs to embed and use for the query.
     """
     query_vectors: NotRequired[List[List[float]]]
     """
-    (Optional) Vector to use for the query.
+    (Optional) Vectors to use for the query.
     """
-    query_strings: NotRequired[List[str]]
+    query_ids: NotRequired[List[str]]
     """
-    (Optional) Texts to embed and use for the query.
+    (Optional) Document IDs to use for the query.
     """
     top_k: NotRequired[int]
     """
     (Optional) Number of results to return.
     """
     ef_search: NotRequired[int]
     """
@@ -1413,13 +1442,13 @@
     """
     name: NotRequired[str]
     """
     (Optional) Vector store name.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
-    (Optional) Selected embedding model
+    (Optional) Selected embedding model.
     """
     metric: NotRequired[Literal["cosine", "l2", "inner"]]
     """
     (Optional) The distance metric used for the query.
     """
```

### Comparing `substrate-120240411.0.5/PKG-INFO` & `substrate-120240416.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrate
-Version: 120240411.0.5
+Version: 120240416.0.5
 Summary: Substrate Python SDK
 Author: vprtwn
 Author-email: ben@substrate.run
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

