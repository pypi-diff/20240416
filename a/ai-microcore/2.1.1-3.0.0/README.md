# Comparing `tmp/ai_microcore-2.1.1.tar.gz` & `tmp/ai_microcore-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_microcore-2.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ai_microcore-3.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ai_microcore-2.1.1.tar` & `ai_microcore-3.0.0.tar`

### file list

```diff
@@ -1,33 +1,36 @@
--rwxr-xr-x   0        0        0     1091 2023-11-04 16:00:47.197704 ai_microcore-2.1.1/LICENSE
--rwxr-xr-x   0        0        0    11116 2024-04-04 12:54:33.488412 ai_microcore-2.1.1/README.md
--rwxr-xr-x   0        0        0     3708 2024-04-04 12:56:07.187360 ai_microcore-2.1.1/microcore/__init__.py
--rwxr-xr-x   0        0        0     4240 2024-04-04 12:45:56.704857 ai_microcore-2.1.1/microcore/_env.py
--rwxr-xr-x   0        0        0     2984 2023-11-06 21:28:53.896764 ai_microcore-2.1.1/microcore/_llm_functions.py
--rwxr-xr-x   0        0        0      770 2024-03-08 01:17:33.018421 ai_microcore-2.1.1/microcore/_prepare_llm_args.py
--rwxr-xr-x   0        0        0     2319 2024-03-08 00:49:48.900573 ai_microcore-2.1.1/microcore/ai_func/__init__.py
--rwxr-xr-x   0        0        0      314 2023-11-04 16:00:47.368478 ai_microcore-2.1.1/microcore/ai_func/python_ai_func.j2
--rwxr-xr-x   0        0        0      576 2023-11-04 19:26:33.244252 ai_microcore-2.1.1/microcore/ai_modules.py
--rwxr-xr-x   0        0        0     9059 2024-03-11 12:20:49.160112 ai_microcore-2.1.1/microcore/configuration.py
--rwxr-xr-x   0        0        0     3133 2024-02-15 20:01:36.859722 ai_microcore-2.1.1/microcore/embedding_db/__init__.py
--rwxr-xr-x   0        0        0     4565 2024-02-15 19:46:15.503154 ai_microcore-2.1.1/microcore/embedding_db/chromadb.py
--rwxr-xr-x   0        0        0     8369 2024-03-08 00:49:49.038994 ai_microcore-2.1.1/microcore/file_storage.py
--rwxr-xr-x   0        0        0       16 2023-11-06 23:41:28.213361 ai_microcore-2.1.1/microcore/llm/__init__.py
--rwxr-xr-x   0        0        0     4604 2024-03-06 22:50:03.566092 ai_microcore-2.1.1/microcore/llm/_openai_llm_v0.py
--rwxr-xr-x   0        0        0     4992 2024-03-11 12:21:18.049189 ai_microcore-2.1.1/microcore/llm/_openai_llm_v1.py
--rwxr-xr-x   0        0        0     3593 2024-03-12 21:54:00.180696 ai_microcore-2.1.1/microcore/llm/anthropic.py
--rwxr-xr-x   0        0        0     4457 2024-03-31 01:09:15.563970 ai_microcore-2.1.1/microcore/llm/google_genai.py
--rwxr-xr-x   0        0        0     5742 2024-03-31 01:09:15.565017 ai_microcore-2.1.1/microcore/llm/google_vertex_ai.py
--rwxr-xr-x   0        0        0      272 2023-11-06 23:49:42.323932 ai_microcore-2.1.1/microcore/llm/openai_llm.py
--rwxr-xr-x   0        0        0     2452 2024-03-31 01:09:15.565536 ai_microcore-2.1.1/microcore/logging.py
--rwxr-xr-x   0        0        0      642 2024-03-08 00:49:48.881046 ai_microcore-2.1.1/microcore/message_types.py
--rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.559200 ai_microcore-2.1.1/microcore/templating/__init__.py
--rwxr-xr-x   0        0        0      525 2023-11-12 15:43:10.028753 ai_microcore-2.1.1/microcore/templating/jinja2.py
--rwxr-xr-x   0        0        0     1455 2024-03-31 01:09:15.566074 ai_microcore-2.1.1/microcore/text2speech/elevenlabs.py
--rwxr-xr-x   0        0        0     1046 2024-03-11 12:20:49.086082 ai_microcore-2.1.1/microcore/types.py
--rwxr-xr-x   0        0        0     1535 2024-03-31 01:09:15.567119 ai_microcore-2.1.1/microcore/ui.py
--rwxr-xr-x   0        0        0     5381 2024-04-02 14:29:38.872233 ai_microcore-2.1.1/microcore/utils.py
--rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.618937 ai_microcore-2.1.1/microcore/wrappers/__init__.py
--rwxr-xr-x   0        0        0     5056 2024-04-04 11:19:36.573733 ai_microcore-2.1.1/microcore/wrappers/llm_response_wrapper.py
--rwxr-xr-x   0        0        0      480 2024-04-02 14:01:24.033112 ai_microcore-2.1.1/microcore/wrappers/prompt_wrapper.py
--rwxr-xr-x   0        0        0     1287 2023-11-26 19:05:20.640308 ai_microcore-2.1.1/pyproject.toml
--rw-r--r--   0        0        0    11811 1970-01-01 00:00:00.000000 ai_microcore-2.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1091 2023-11-04 16:00:47.197704 ai_microcore-3.0.0/LICENSE
+-rwxr-xr-x   0        0        0    11116 2024-04-04 12:54:33.488412 ai_microcore-3.0.0/README.md
+-rwxr-xr-x   0        0        0     3708 2024-04-16 13:57:50.530488 ai_microcore-3.0.0/microcore/__init__.py
+-rwxr-xr-x   0        0        0     5172 2024-04-16 13:59:44.280985 ai_microcore-3.0.0/microcore/_env.py
+-rwxr-xr-x   0        0        0     2984 2023-11-06 21:28:53.896764 ai_microcore-3.0.0/microcore/_llm_functions.py
+-rwxr-xr-x   0        0        0      770 2024-03-08 01:17:33.018421 ai_microcore-3.0.0/microcore/_prepare_llm_args.py
+-rwxr-xr-x   0        0        0     2319 2024-03-08 00:49:48.900573 ai_microcore-3.0.0/microcore/ai_func/__init__.py
+-rwxr-xr-x   0        0        0      314 2023-11-04 16:00:47.368478 ai_microcore-3.0.0/microcore/ai_func/python_ai_func.j2
+-rwxr-xr-x   0        0        0      576 2023-11-04 19:26:33.244252 ai_microcore-3.0.0/microcore/ai_modules.py
+-rwxr-xr-x   0        0        0    11345 2024-04-16 14:19:14.188938 ai_microcore-3.0.0/microcore/configuration.py
+-rwxr-xr-x   0        0        0     3133 2024-02-15 20:01:36.859722 ai_microcore-3.0.0/microcore/embedding_db/__init__.py
+-rwxr-xr-x   0        0        0     4565 2024-02-15 19:46:15.503154 ai_microcore-3.0.0/microcore/embedding_db/chromadb.py
+-rwxr-xr-x   0        0        0     8369 2024-03-08 00:49:49.038994 ai_microcore-3.0.0/microcore/file_storage.py
+-rwxr-xr-x   0        0        0     3258 2024-04-15 09:53:22.340269 ai_microcore-3.0.0/microcore/json_parsing.py
+-rwxr-xr-x   0        0        0       16 2023-11-06 23:41:28.213361 ai_microcore-3.0.0/microcore/llm/__init__.py
+-rwxr-xr-x   0        0        0     4708 2024-04-16 08:56:56.272317 ai_microcore-3.0.0/microcore/llm/_openai_llm_v0.py
+-rwxr-xr-x   0        0        0     5078 2024-04-16 09:40:54.280341 ai_microcore-3.0.0/microcore/llm/_openai_llm_v1.py
+-rwxr-xr-x   0        0        0     3655 2024-04-16 13:59:52.503374 ai_microcore-3.0.0/microcore/llm/anthropic.py
+-rwxr-xr-x   0        0        0     4479 2024-04-16 09:04:29.151454 ai_microcore-3.0.0/microcore/llm/google_genai.py
+-rwxr-xr-x   0        0        0     5773 2024-04-16 09:04:29.140424 ai_microcore-3.0.0/microcore/llm/google_vertex_ai.py
+-rwxr-xr-x   0        0        0     3229 2024-04-16 14:08:39.822867 ai_microcore-3.0.0/microcore/llm/local_llm.py
+-rwxr-xr-x   0        0        0     2512 2024-04-16 14:10:15.666540 ai_microcore-3.0.0/microcore/llm/local_transformers.py
+-rwxr-xr-x   0        0        0      272 2023-11-06 23:49:42.323932 ai_microcore-3.0.0/microcore/llm/openai_llm.py
+-rwxr-xr-x   0        0        0     2466 2024-04-16 08:13:17.036046 ai_microcore-3.0.0/microcore/logging.py
+-rwxr-xr-x   0        0        0      642 2024-03-08 00:49:48.881046 ai_microcore-3.0.0/microcore/message_types.py
+-rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.559200 ai_microcore-3.0.0/microcore/templating/__init__.py
+-rwxr-xr-x   0        0        0      525 2023-11-12 15:43:10.028753 ai_microcore-3.0.0/microcore/templating/jinja2.py
+-rwxr-xr-x   0        0        0     1455 2024-03-31 01:09:15.566074 ai_microcore-3.0.0/microcore/text2speech/elevenlabs.py
+-rwxr-xr-x   0        0        0     1046 2024-03-11 12:20:49.086082 ai_microcore-3.0.0/microcore/types.py
+-rwxr-xr-x   0        0        0     1535 2024-03-31 01:09:15.567119 ai_microcore-3.0.0/microcore/ui.py
+-rwxr-xr-x   0        0        0     6561 2024-04-16 10:15:22.027885 ai_microcore-3.0.0/microcore/utils.py
+-rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.618937 ai_microcore-3.0.0/microcore/wrappers/__init__.py
+-rwxr-xr-x   0        0        0     1945 2024-04-16 14:05:38.089958 ai_microcore-3.0.0/microcore/wrappers/llm_response_wrapper.py
+-rwxr-xr-x   0        0        0      480 2024-04-02 14:01:24.033112 ai_microcore-3.0.0/microcore/wrappers/prompt_wrapper.py
+-rwxr-xr-x   0        0        0     1287 2023-11-26 19:05:20.640308 ai_microcore-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0    11811 1970-01-01 00:00:00.000000 ai_microcore-3.0.0/PKG-INFO
```

### Comparing `ai_microcore-2.1.1/LICENSE` & `ai_microcore-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_microcore-2.1.1/README.md` & `ai_microcore-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ai_microcore-2.1.1/microcore/__init__.py` & `ai_microcore-3.0.0/microcore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,8 +123,8 @@
     "utils",
     "configuration",
     "types",
     "ui",
     # "wrappers",
 ]
 
-__version__ = "2.1.1"
+__version__ = "3.0.0"
```

### Comparing `ai_microcore-2.1.1/microcore/_env.py` & `ai_microcore-3.0.0/microcore/_env.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import jinja2
 
 from .configuration import Config, ApiType
 from . import AbstractEmbeddingDB
 from .types import TplFunctionType, LLMAsyncFunctionType, LLMFunctionType
 from .templating.jinja2 import make_jinja2_env, make_tpl_function
 from .llm.openai_llm import make_llm_functions as make_openai_llm_functions
+from .llm.local_llm import make_llm_functions as make_local_llm_functions
 
 
 @dataclass
 class Env:
     config: Config = field(default_factory=Config)
     jinja_env: jinja2.Environment = None
     tpl_function: TplFunctionType = None
@@ -32,15 +33,32 @@
         self.init_similarity_search()
 
     def init_templating(self):
         self.jinja_env = make_jinja2_env(self)
         self.tpl_function = make_tpl_function(self)
 
     def init_llm(self):
-        if self.config.LLM_API_TYPE == ApiType.ANTHROPIC:
+        if self.config.LLM_API_TYPE == ApiType.LOCAL_FUNC:
+            self.llm_function, self.llm_async_function = make_local_llm_functions(
+                self.config
+            )
+        elif self.config.LLM_API_TYPE == ApiType.LOCAL_TRANSFORMERS:
+            try:
+                from .llm.local_transformers import (
+                    make_llm_functions as make_transformers_llm_functions,
+                )
+            except ModuleNotFoundError as e:
+                raise ModuleNotFoundError(
+                    "To use local Transformers language models, "
+                    "you need to install the `transformers`, `pytorch` and `accelerate` packages. "
+                ) from e
+            (self.llm_function, self.llm_async_function) = (
+                make_transformers_llm_functions(self.config, self)
+            )
+        elif self.config.LLM_API_TYPE == ApiType.ANTHROPIC:
             try:
                 from .llm.anthropic import (
                     make_llm_functions as make_anthropic_llm_functions,
                 )
             except ModuleNotFoundError as e:
                 raise ModuleNotFoundError(
                     "To use the Anthropic language models, "
```

### Comparing `ai_microcore-2.1.1/microcore/_llm_functions.py` & `ai_microcore-3.0.0/microcore/_llm_functions.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-2.1.1/microcore/_prepare_llm_args.py` & `ai_microcore-3.0.0/microcore/_prepare_llm_args.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-2.1.1/microcore/ai_func/__init__.py` & `ai_microcore-3.0.0/microcore/ai_func/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-2.1.1/microcore/ai_modules.py` & `ai_microcore-3.0.0/microcore/ai_modules.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-2.1.1/microcore/configuration.py` & `ai_microcore-3.0.0/microcore/configuration.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import logging
 import os
 from dataclasses import dataclass, field, fields
 from pathlib import Path
 from typing import Any
+from typing import Union, Callable
 
 import dotenv
 
 _MISSING = object()
 
 TRUE_VALUES = ["1", "TRUE", "YES", "ON", "ENABLED", "Y", "+"]
 """@private"""
@@ -25,15 +27,16 @@
 
 class ApiType:
     """LLM API types"""
 
     OPEN_AI = "open_ai"
     AZURE = "azure"
     """See https://learn.microsoft.com/en-us/azure/ai-services/openai/concepts/models"""
-    LLM = "llm"
+    LOCAL_FUNC = "local"
+    LOCAL_TRANSFORMERS = "local_transformers"
     ANYSCALE = "anyscale"
     """See https://www.anyscale.com/endpoints"""
     DEEP_INFRA = "deep_infra"
     """List of text generation models: https://deepinfra.com/models?type=text-generation"""
     ANTHROPIC = "anthropic"
     GOOGLE_VERTEX_AI = "google_vertex_ai"
     GOOGLE_AI_STUDIO = "google_ai_studio"
@@ -66,14 +69,19 @@
                 _default_dotenv_loaded = True
 
     def _update_from_env(self):
         for f in fields(self):
             if f.metadata.get("_from_env") and getattr(self, f.name) is _MISSING:
                 setattr(self, f.name, os.getenv(f.name.upper(), f.metadata["_default"]))
 
+    def __iter__(self):
+        for f in fields(self):
+            value = getattr(self, f.name)
+            yield f.name, value
+
 
 @dataclass
 class _OpenAIEnvVars:
     # OS Environment variables expected by OpenAI library
     # Will be used as defaults for LLM
     # @todo: implement lib_defaults to take default values from openai lib if available
     OPENAI_API_TYPE: str = from_env(ApiType.OPEN_AI)
@@ -123,20 +131,36 @@
     """
     You may specify here default arguments for the LLM API calls,
      i. e. temperature, max_tokens, etc.
      """
 
     AZURE_DEPLOYMENT_ID: str = from_env()
 
+    INFERENCE_FUNC: Union[Callable, str] = None
+    """Inference function for local models"""
+    CHAT_MODE: bool = None
+    """Is it a chat or completion model"""
+    INIT_PARAMS: dict = field(default_factory=dict)
+    """Custom initialization parameters for the model"""
+
     def __post_init__(self):
         super().__post_init__()
         self._init_llm_options()
         self.validate()
 
+    def is_local_llm_used(self) -> bool:
+        return self.LLM_API_TYPE in (ApiType.LOCAL_FUNC, ApiType.LOCAL_TRANSFORMERS)
+
     def _init_llm_options(self):
+        if self.INFERENCE_FUNC:
+            if not self.LLM_API_TYPE:
+                self.LLM_API_TYPE = ApiType.LOCAL_FUNC
+        if self.is_local_llm_used():
+            return
+
         # Use defaults from ENV variables expected by OpenAI API
         self.LLM_API_TYPE = self.LLM_API_TYPE or self.OPENAI_API_TYPE
         if self.GOOGLE_VERTEX_RESPONSE_VALIDATION is None:
             self.GOOGLE_VERTEX_RESPONSE_VALIDATION = get_bool_from_env(
                 "GOOGLE_VERTEX_RESPONSE_VALIDATION", False
             )
 
@@ -167,21 +191,54 @@
             self.LLM_API_KEY = self.LLM_API_KEY or self.ANTHROPIC_API_KEY
         else:
             self.LLM_API_BASE = self.LLM_API_BASE or self.OPENAI_API_BASE
             self.LLM_API_KEY = self.LLM_API_KEY or self.OPENAI_API_KEY
             self.LLM_API_VERSION = self.LLM_API_VERSION or self.OPENAI_API_VERSION
             self.MODEL = self.MODEL or "gpt-3.5-turbo"
 
+    def _validate_local_llm(self):
+        if self.CHAT_MODE is None:
+            logging.warning(
+                "When using local models, "
+                "(bool)CHAT_MODE configuration option should be explicitly set"
+            )
+        if self.LLM_API_TYPE == ApiType.LOCAL_FUNC:
+            if not self.INFERENCE_FUNC:
+                raise LLMConfigError(
+                    "LLM configuration error: "
+                    "INFERENCE_FUNC should be provided for local models"
+                )
+            if (
+                isinstance(self.INFERENCE_FUNC, str)
+                and self.INFERENCE_FUNC not in globals()
+            ):
+                raise LLMConfigError(
+                    f"LLM configuration error: inference function '{self.INFERENCE_FUNC}' not found"
+                )
+        elif self.LLM_API_TYPE == ApiType.LOCAL_TRANSFORMERS:
+            if not self.MODEL:
+                raise LLMConfigError(
+                    "LLM configuration error: "
+                    "MODEL should be provided for local transformers models"
+                )
+
     def validate(self):
         """
         Validate LLM configuration
 
         Raises:
             LLMConfigError
         """
+        if self.is_local_llm_used():
+            self._validate_local_llm()
+            return
+        if self.INFERENCE_FUNC:
+            raise LLMConfigError(
+                "LLM configuration error: INFERENCE_FUNC should be provided only for local models"
+            )
         if self.LLM_API_TYPE == ApiType.GOOGLE_VERTEX_AI:
             if (
                 not self.GOOGLE_VERTEX_ACCESS_TOKEN
                 and not self.GOOGLE_VERTEX_GCLOUD_AUTH
             ):
                 raise LLMConfigError(
                     "LLM configuration error: "
@@ -239,14 +296,15 @@
     """Used in file system operations, utf-8 by default"""
 
     JINJA2_AUTO_ESCAPE: bool = None
 
     ELEVENLABS_API_KEY: str = from_env()
 
     TEXT_TO_SPEECH_PATH: str | Path = from_env()
+    """Path to the folder with generated voice files"""
 
     def __post_init__(self):
         if self.JINJA2_AUTO_ESCAPE is None:
             self.JINJA2_AUTO_ESCAPE = get_bool_from_env("JINJA2_AUTO_ESCAPE", False)
         super().__post_init__()
         if self.TEXT_TO_SPEECH_PATH is None:
             self.TEXT_TO_SPEECH_PATH = Path(self.STORAGE_PATH) / "voicing"
```

### Comparing `ai_microcore-2.1.1/microcore/embedding_db/__init__.py` & `ai_microcore-3.0.0/microcore/embedding_db/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-2.1.1/microcore/embedding_db/chromadb.py` & `ai_microcore-3.0.0/microcore/embedding_db/chromadb.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-2.1.1/microcore/file_storage.py` & `ai_microcore-3.0.0/microcore/file_storage.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-2.1.1/microcore/llm/_openai_llm_v0.py` & `ai_microcore-3.0.0/microcore/llm/_openai_llm_v0.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     except openai.error.InvalidAPIType:
         api_type = ApiType.OPEN_AI
 
     openai.api_type = api_type
     openai.api_key = config.LLM_API_KEY
     openai.api_base = config.LLM_API_BASE
     openai.api_version = config.LLM_API_VERSION
+    for key, value in config.INIT_PARAMS.items():
+        setattr(openai, key, value)
 
 
 def _prepare_llm_arguments(config: Config, kwargs: dict):
     args = {**config.LLM_DEFAULT_ARGS, **kwargs}
 
     args["model"] = args.get("model", config.MODEL)
 
@@ -76,15 +78,15 @@
 
 
 def make_llm_functions(config: Config) -> tuple[LLMFunctionType, LLMAsyncFunctionType]:
     _configure_open_ai_package(config)
 
     async def allm(prompt, **kwargs):
         args, options = _prepare_llm_arguments(config, kwargs)
-        if is_chat_model(args["model"]):
+        if is_chat_model(args["model"], config):
             response = await openai.ChatCompletion.acreate(
                 messages=prepare_chat_messages(prompt), **args
             )
             if args["stream"]:
                 return await _a_process_streamed_response(
                     response, options["callbacks"], chat_model_used=True
                 )
@@ -101,15 +103,15 @@
                 response, options["callbacks"], chat_model_used=False
             )
 
         return LLMResponse(response.choices[0].text, response)
 
     def llm(prompt, **kwargs):
         args, options = _prepare_llm_arguments(config, kwargs)
-        if is_chat_model(args["model"]):
+        if is_chat_model(args["model"], config):
             response = openai.ChatCompletion.create(
                 messages=prepare_chat_messages(prompt), **args
             )
             if args["stream"]:
                 return _process_streamed_response(
                     response, options["callbacks"], chat_model_used=True
                 )
```

### Comparing `ai_microcore-2.1.1/microcore/llm/_openai_llm_v1.py` & `ai_microcore-3.0.0/microcore/llm/_openai_llm_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,29 +69,31 @@
     if config.LLM_API_TYPE == ApiType.AZURE:
         connection_type = openai.AzureOpenAI
         async_connection_type = openai.AsyncAzureOpenAI
         params = dict(
             api_key=config.LLM_API_KEY,
             azure_endpoint=config.LLM_API_BASE,
             api_version=config.LLM_API_VERSION,
+            **config.INIT_PARAMS
         )
     else:
         connection_type = openai.OpenAI
         async_connection_type = openai.AsyncOpenAI
         params = dict(
             api_key=config.LLM_API_KEY,
             base_url=config.LLM_API_BASE,
+            # **config.INIT_PARAMS
         )
 
     _connection = connection_type(**params)
     _async_connection = async_connection_type(**params)
 
     async def allm(prompt, **kwargs):
         args, options = _prepare_llm_arguments(config, kwargs)
-        if is_chat_model(args["model"]):
+        if is_chat_model(args["model"], config):
             response = await _async_connection.chat.completions.create(
                 messages=prepare_chat_messages(prompt), **args
             )
             if args["stream"]:
                 return await _a_process_streamed_response(
                     response, options["callbacks"], chat_model_used=True
                 )
@@ -108,15 +110,15 @@
                 response, options["callbacks"], chat_model_used=False
             )
 
         return LLMResponse(response.choices[0].text, response.__dict__)
 
     def llm(prompt, **kwargs):
         args, options = _prepare_llm_arguments(config, kwargs)
-        if is_chat_model(args["model"]):
+        if is_chat_model(args["model"], config):
             response = _connection.chat.completions.create(
                 messages=prepare_chat_messages(prompt), **args
             )
             if args["stream"]:
                 return _process_streamed_response(
                     response, options["callbacks"], chat_model_used=True
                 )
```

### Comparing `ai_microcore-2.1.1/microcore/llm/anthropic.py` & `ai_microcore-3.0.0/microcore/llm/anthropic.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             [cb(text_chunk) for cb in callbacks]
     return LLMResponse(response_text, {})
 
 
 def _prepare_llm_arguments(config: Config, kwargs: dict):
     args = {"max_tokens": 1024, **config.LLM_DEFAULT_ARGS, **kwargs}
     args["model"] = args.get("model", config.MODEL)
-    args.pop('seed', None)  # Not supported by Anthropic
+    args.pop("seed", None)  # Not supported by Anthropic
     callbacks: list[callable] = args.pop("callbacks", [])
     if "callback" in args:
         cb = args.pop("callback")
         if cb:
             callbacks.append(cb)
     args["stream"] = bool(callbacks)
     return args, {"callbacks": callbacks}
@@ -59,18 +59,20 @@
     return system, [i for i in prepared_messages if i.get("role") != Role.SYSTEM]
 
 
 def make_llm_functions(config: Config) -> tuple[LLMFunctionType, LLMAsyncFunctionType]:
     sync_client = anthropic.Anthropic(
         api_key=config.LLM_API_KEY,
         base_url=config.LLM_API_BASE,
+        **config.INIT_PARAMS,
     )
     async_client = anthropic.AsyncAnthropic(
         api_key=config.LLM_API_KEY,
         base_url=config.LLM_API_BASE,
+        **config.INIT_PARAMS,
     )
 
     async def allm(prompt, **kwargs):
         args, options = _prepare_llm_arguments(config, kwargs)
         args["system"], args["messages"] = _extract_sys_msg(
             prepare_chat_messages(prompt)
         )
```

### Comparing `ai_microcore-2.1.1/microcore/llm/google_genai.py` & `ai_microcore-3.0.0/microcore/llm/google_genai.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         if text_chunk := chunk.text:
             response_text += text_chunk
             [cb(text_chunk) for cb in callbacks]
     return LLMResponse(response_text, {})
 
 
 def make_llm_functions(config: Config) -> tuple[LLMFunctionType, LLMAsyncFunctionType]:
-    genai.configure(api_key=config.LLM_API_KEY)
+    genai.configure(api_key=config.LLM_API_KEY, **config.INIT_PARAMS)
     if config.GOOGLE_GEMINI_SAFETY_SETTINGS is None:
         # Only new categories
         config.GOOGLE_GEMINI_SAFETY_SETTINGS = {
             HarmCategory.HARM_CATEGORY_HARASSMENT: HarmBlockThreshold.BLOCK_NONE,
             HarmCategory.HARM_CATEGORY_HATE_SPEECH: HarmBlockThreshold.BLOCK_NONE,
             HarmCategory.HARM_CATEGORY_SEXUALLY_EXPLICIT: HarmBlockThreshold.BLOCK_NONE,
             HarmCategory.HARM_CATEGORY_DANGEROUS_CONTENT: HarmBlockThreshold.BLOCK_NONE,
```

### Comparing `ai_microcore-2.1.1/microcore/llm/google_vertex_ai.py` & `ai_microcore-3.0.0/microcore/llm/google_vertex_ai.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,15 @@
             )
     credentials = Credentials(token=config.GOOGLE_VERTEX_ACCESS_TOKEN)
     vertexai.init(
         credentials=credentials,
         project=config.GOOGLE_VERTEX_PROJECT_ID,
         location=config.GOOGLE_VERTEX_LOCATION or None,
         api_endpoint=config.LLM_API_BASE or None,
+        **config.INIT_PARAMS,
     )
 
 
 def make_llm_functions(config: Config) -> tuple[LLMFunctionType, LLMAsyncFunctionType]:
     init_vertex_ai(config)
     if config.GOOGLE_GEMINI_SAFETY_SETTINGS is None:
         config.GOOGLE_GEMINI_SAFETY_SETTINGS = {
```

### Comparing `ai_microcore-2.1.1/microcore/logging.py` & `ai_microcore-3.0.0/microcore/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def _log_request(prompt, **kwargs):
     nl = "\n" if LoggingConfig.DENSE else "\n" + LoggingConfig.INDENT
     model = _resolve_model(**kwargs)
     print(
         f"Requesting LLM {Fore.MAGENTA}{model}{Style.RESET_ALL}:",
         end=" " if LoggingConfig.DENSE else "\n",
     )
-    if is_chat_model(model):
+    if is_chat_model(model, env().config):
         for msg in prepare_chat_messages(prompt):
             role, content = (
                 (msg["role"], msg["content"])
                 if isinstance(msg, dict)
                 else dataclasses.astuple(msg)
             )
             nl2 = "\n" if LoggingConfig.DENSE else nl + LoggingConfig.INDENT
```

### Comparing `ai_microcore-2.1.1/microcore/message_types.py` & `ai_microcore-3.0.0/microcore/message_types.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-2.1.1/microcore/templating/jinja2.py` & `ai_microcore-3.0.0/microcore/templating/jinja2.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-2.1.1/microcore/text2speech/elevenlabs.py` & `ai_microcore-3.0.0/microcore/text2speech/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-2.1.1/microcore/types.py` & `ai_microcore-3.0.0/microcore/types.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-2.1.1/microcore/ui.py` & `ai_microcore-3.0.0/microcore/ui.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-2.1.1/microcore/utils.py` & `ai_microcore-3.0.0/microcore/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 import builtins
 import dataclasses
 import inspect
 import json
 import os
 import sys
 import re
+import subprocess
+from dataclasses import dataclass
 from fnmatch import fnmatch
 from pathlib import Path
+from colorama import Fore
 
+from .configuration import Config
 from .types import BadAIAnswer
 from .message_types import UserMsg, SysMsg, AssistantMsg
 
 
-def is_chat_model(model: str) -> bool:
+def is_chat_model(model: str, config: Config = None) -> bool:
     """Detects if model is chat model or text completion model"""
+    if config and config.CHAT_MODE is not None:
+        return config.CHAT_MODE
     completion_keywords = ["instruct", "davinci", "babbage", "curie", "ada"]
-    return not any(keyword in model.lower() for keyword in completion_keywords)
+    return not any(keyword in str(model).lower() for keyword in completion_keywords)
 
 
 class ConvertableToMessage:
     @property
     def as_user(self) -> UserMsg:
         return UserMsg(str(self))
 
@@ -160,7 +166,44 @@
 
 def is_kaggle() -> bool:
     return "KAGGLE_KERNEL_RUN_TYPE" in os.environ
 
 
 def is_notebook() -> bool:
     return "ipykernel" in sys.modules
+
+
+def is_google_colab() -> bool:
+    return "google.colab" in sys.modules
+
+
+def get_vram_usage(as_string=True, color=Fore.GREEN):
+    @dataclass
+    class _MemUsage:
+        name: str
+        used: int
+        free: int
+        total: int
+
+    cmd = (
+        "nvidia-smi"
+        " --query-gpu=name,memory.used,memory.free,memory.total"
+        " --format=csv,noheader,nounits"
+    )
+    out = subprocess.check_output(cmd, shell=True, text=True).strip()
+
+    mu = [_MemUsage(*[i.strip() for i in line.split(",")]) for line in out.splitlines()]
+    if not as_string:
+        return mu
+    c, r = (color, Fore.RESET) if color else ("", "")
+    return "\n".join(
+        [
+            f"GPU: {c}{i.name}{r}, "
+            f"VRAM: {c}{i.used}{r}/{c}{i.total}{r} MiB used, "
+            f"{c}{i.free}{r} MiB free"
+            for i in mu
+        ]
+    )
+
+
+def show_vram_usage():
+    print(get_vram_usage(as_string=True))
```

### Comparing `ai_microcore-2.1.1/pyproject.toml` & `ai_microcore-3.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ai_microcore-2.1.1/PKG-INFO` & `ai_microcore-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-microcore
-Version: 2.1.1
+Version: 3.0.0
 Summary: # Minimalistic Foundation for AI Applications
 Keywords: llm,large language models,ai,similarity search,ai search,gpt,openai
 Author-email: Vitalii Stepanenko <mail@vitalii.in>
 Maintainer-email: Vitalii Stepanenko <mail@vitalii.in>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ai-microcore Version: 2.1.1 Summary: # Minimalistic
+Metadata-Version: 2.1 Name: ai-microcore Version: 3.0.0 Summary: # Minimalistic
 Foundation for AI Applications Keywords: llm,large language
 models,ai,similarity search,ai search,gpt,openai Author-email: Vitalii
 Stepanenko
 vitalii.in> Maintainer-email: Vitalii Stepanenko
 vitalii.in> Requires-Python: >=3.10 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
```

