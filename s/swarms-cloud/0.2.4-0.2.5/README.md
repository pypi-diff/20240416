# Comparing `tmp/swarms_cloud-0.2.4.tar.gz` & `tmp/swarms_cloud-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms_cloud-0.2.4.tar", max compression
+gzip compressed data, was "swarms_cloud-0.2.5.tar", max compression
```

## Comparing `swarms_cloud-0.2.4.tar` & `swarms_cloud-0.2.5.tar`

### file list

```diff
@@ -1,24 +1,28 @@
--rw-r--r--   0        0        0     1074 2023-12-07 23:39:09.988634 swarms_cloud-0.2.4/LICENSE
--rw-r--r--   0        0        0     6558 2024-03-18 03:13:41.692057 swarms_cloud-0.2.4/README.md
--rw-r--r--   0        0        0     1437 2024-03-24 20:34:37.787854 swarms_cloud-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2679 2024-03-24 20:34:24.463794 swarms_cloud-0.2.4/swarms_cloud/__init__.py
--rw-r--r--   0        0        0     2391 2024-03-18 03:18:00.956334 swarms_cloud-0.2.4/swarms_cloud/api_utils.py
--rw-r--r--   0        0        0     3468 2024-03-24 20:33:32.610161 swarms_cloud-0.2.4/swarms_cloud/auth_with_swarms_cloud.py
--rw-r--r--   0        0        0     3127 2024-03-24 19:50:18.076179 swarms_cloud-0.2.4/swarms_cloud/calculate_pricing.py
--rw-r--r--   0        0        0     9262 2024-03-22 00:43:33.383112 swarms_cloud-0.2.4/swarms_cloud/cogvlm.py
--rw-r--r--   0        0        0     5398 2023-12-19 17:39:01.720297 swarms_cloud-0.2.4/swarms_cloud/func_api_wrapper.py
--rw-r--r--   0        0        0     1755 2024-03-20 22:45:22.858447 swarms_cloud-0.2.4/swarms_cloud/log_api_request_to_supabase.py
--rw-r--r--   0        0        0        0 2024-03-18 03:37:43.673019 swarms_cloud-0.2.4/swarms_cloud/loggers/__init__.py
--rw-r--r--   0        0        0     4209 2023-12-09 01:56:05.742032 swarms_cloud-0.2.4/swarms_cloud/loggers/supabase_handler.py
--rw-r--r--   0        0        0     1965 2024-03-10 07:01:44.690761 swarms_cloud-0.2.4/swarms_cloud/loggers/supabase_logger.py
--rw-r--r--   0        0        0        0 2024-03-18 03:32:46.364514 swarms_cloud-0.2.4/swarms_cloud/schema/__init__.py
--rw-r--r--   0        0        0     2315 2024-03-21 00:20:09.255945 swarms_cloud-0.2.4/swarms_cloud/schema/cog_vlm_schemas.py
--rw-r--r--   0        0        0    10148 2024-02-03 17:20:33.472784 swarms_cloud-0.2.4/swarms_cloud/schema/openai_protocol.py
--rw-r--r--   0        0        0     4260 2024-02-24 05:40:08.165528 swarms_cloud-0.2.4/swarms_cloud/schema/openai_spec.py
--rw-r--r--   0        0        0     6046 2024-02-24 08:31:47.339750 swarms_cloud-0.2.4/swarms_cloud/sky_api.py
--rw-r--r--   0        0        0      654 2024-02-25 17:44:35.901179 swarms_cloud-0.2.4/swarms_cloud/stripe_utils.py
--rw-r--r--   0        0        0        0 2024-03-18 03:37:34.039217 swarms_cloud-0.2.4/swarms_cloud/utils/__init__.py
--rw-r--r--   0        0        0     1000 2024-02-25 17:46:23.901523 swarms_cloud-0.2.4/swarms_cloud/utils/api_key_generator.py
--rw-r--r--   0        0        0     1220 2023-12-18 16:16:18.130456 swarms_cloud-0.2.4/swarms_cloud/utils/rate_limiter.py
--rw-r--r--   0        0        0     7734 1970-01-01 00:00:00.000000 swarms_cloud-0.2.4/setup.py
--rw-r--r--   0        0        0     7834 1970-01-01 00:00:00.000000 swarms_cloud-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-16 20:57:09.802958 swarms_cloud-0.2.5/LICENSE
+-rw-r--r--   0        0        0     6558 2024-04-16 20:57:09.803449 swarms_cloud-0.2.5/README.md
+-rw-r--r--   0        0        0     1426 2024-04-16 21:55:15.319242 swarms_cloud-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2558 2024-04-16 20:57:09.899014 swarms_cloud-0.2.5/swarms_cloud/__init__.py
+-rw-r--r--   0        0        0     1340 2024-04-16 20:57:09.899609 swarms_cloud-0.2.5/swarms_cloud/api_utils.py
+-rw-r--r--   0        0        0     3687 2024-04-16 21:41:31.149402 swarms_cloud-0.2.5/swarms_cloud/auth_with_swarms_cloud.py
+-rw-r--r--   0        0        0     3121 2024-04-16 20:57:09.900632 swarms_cloud-0.2.5/swarms_cloud/calculate_pricing.py
+-rw-r--r--   0        0        0     1080 2024-04-16 20:57:09.901139 swarms_cloud-0.2.5/swarms_cloud/check_model_list.py
+-rw-r--r--   0        0        0     5398 2024-04-16 20:57:09.901692 swarms_cloud-0.2.5/swarms_cloud/func_api_wrapper.py
+-rw-r--r--   0        0        0        0 2024-04-16 20:57:09.902213 swarms_cloud-0.2.5/swarms_cloud/loggers/__init__.py
+-rw-r--r--   0        0        0     1931 2024-04-16 21:52:45.325451 swarms_cloud-0.2.5/swarms_cloud/loggers/log_api_request_to_supabase.py
+-rw-r--r--   0        0        0     4209 2024-04-16 20:57:09.903158 swarms_cloud-0.2.5/swarms_cloud/loggers/supabase_handler.py
+-rw-r--r--   0        0        0     1965 2024-04-16 20:57:09.903681 swarms_cloud-0.2.5/swarms_cloud/loggers/supabase_logger.py
+-rw-r--r--   0        0        0      535 2024-04-16 20:57:09.904414 swarms_cloud-0.2.5/swarms_cloud/methods.py
+-rw-r--r--   0        0        0        0 2024-04-16 20:57:09.904808 swarms_cloud-0.2.5/swarms_cloud/schema/__init__.py
+-rw-r--r--   0        0        0     3187 2024-04-16 20:57:09.905303 swarms_cloud-0.2.5/swarms_cloud/schema/auto_swarm_schema.py
+-rw-r--r--   0        0        0     2315 2024-04-16 20:57:09.905841 swarms_cloud-0.2.5/swarms_cloud/schema/cog_vlm_schemas.py
+-rw-r--r--   0        0        0    10148 2024-04-16 20:57:09.907725 swarms_cloud-0.2.5/swarms_cloud/schema/openai_protocol.py
+-rw-r--r--   0        0        0     4260 2024-04-16 20:57:09.908307 swarms_cloud-0.2.5/swarms_cloud/schema/openai_spec.py
+-rw-r--r--   0        0        0     1873 2024-04-16 21:41:31.627938 swarms_cloud-0.2.5/swarms_cloud/schema/text_to_video.py
+-rw-r--r--   0        0        0      654 2024-04-16 20:57:09.909082 swarms_cloud-0.2.5/swarms_cloud/stripe_utils.py
+-rw-r--r--   0        0        0        0 2024-04-16 20:57:09.909373 swarms_cloud-0.2.5/swarms_cloud/utils/__init__.py
+-rw-r--r--   0        0        0     1000 2024-04-16 20:57:09.909741 swarms_cloud-0.2.5/swarms_cloud/utils/api_key_generator.py
+-rw-r--r--   0        0        0      525 2024-04-16 20:57:09.910061 swarms_cloud-0.2.5/swarms_cloud/utils/model_name_fetcher.py
+-rw-r--r--   0        0        0     1220 2024-04-16 20:57:09.910373 swarms_cloud-0.2.5/swarms_cloud/utils/rate_limiter.py
+-rw-r--r--   0        0        0      357 2024-04-16 20:57:09.911908 swarms_cloud-0.2.5/swarms_cloud/verify_swarms_acc.py
+-rw-r--r--   0        0        0     7725 1970-01-01 00:00:00.000000 swarms_cloud-0.2.5/setup.py
+-rw-r--r--   0        0        0     7814 1970-01-01 00:00:00.000000 swarms_cloud-0.2.5/PKG-INFO
```

### Comparing `swarms_cloud-0.2.4/LICENSE` & `swarms_cloud-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms_cloud-0.2.4/README.md` & `swarms_cloud-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `swarms_cloud-0.2.4/pyproject.toml` & `swarms_cloud-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "swarms-cloud"
-version = "0.2.4"
+version = "0.2.5"
 description = "Swarms Cloud - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/swarms-cloud"
 documentation = "https://github.com/kyegomez/swarms-cloud"  # Add this if you have documentation.
 readme = "README.md"  # Assuming you have a README.md
 repository = "https://github.com/kyegomez/swarms-cloud"
@@ -31,15 +31,14 @@
 pydantic = ">2,<3"
 stripe = "*"
 transformers = "*"
 sse-starlette = "2.0.0" 
 uvicorn = "*"
 shortuuid = "*"
 xformers = "*"
-exxa = "*"
 
 [tool.poetry.group.lint.dependencies]
 ruff = ">=0.1.6,<0.4.0"
 types-toml = "^0.10.8.1"
 types-redis = "^4.3.21.6"
 types-pytz = ">=2023.3,<2025.0"
 black = "^23.1.0"
```

### Comparing `swarms_cloud-0.2.4/swarms_cloud/__init__.py` & `swarms_cloud-0.2.5/swarms_cloud/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,27 @@
-from swarms_cloud.api_utils import (
-    VariableInterface,
-    check_api_key,
-    check_request,
-    create_error_response,
-    get_model_list,
-)
 from swarms_cloud.auth_with_swarms_cloud import (
     authenticate_user,
     fetch_api_key_info,
     is_token_valid,
 )
+
+
+from swarms_cloud.check_model_list import (
+    get_model_list,
+    create_error_response,
+    check_request,
+)
+
+
 from swarms_cloud.calculate_pricing import calculate_pricing, count_tokens
 from swarms_cloud.func_api_wrapper import SwarmCloud
-from swarms_cloud.log_api_request_to_supabase import ModelAPILogEntry, log_to_supabase
+from swarms_cloud.loggers.log_api_request_to_supabase import (
+    ModelAPILogEntry,
+    log_to_supabase,
+)
 from swarms_cloud.schema.openai_protocol import (  # noqa: E501
     ChatCompletionRequest,
     ChatCompletionRequestQos,
     ChatCompletionResponse,
     ChatCompletionResponseChoice,
     ChatCompletionResponseStreamChoice,
     ChatCompletionStreamResponse,
@@ -42,24 +47,31 @@
     UsageInfo,
 )
 from swarms_cloud.schema.openai_spec import (
     InputOpenAISpec,
     OpenAIAPIWrapper,
     OutputOpenAISpec,
 )
-from swarms_cloud.sky_api import SkyInterface
 from swarms_cloud.utils.api_key_generator import generate_api_key
 from swarms_cloud.utils.rate_limiter import rate_limiter
 from swarms_cloud.auth_with_swarms_cloud import verify_token
 
+
 __all__ = [
-    "generate_api_key",
+    "authenticate_user",
+    "fetch_api_key_info",
+    "is_token_valid",
+    "get_model_list",
+    "create_error_response",
+    "check_request",
+    "calculate_pricing",
+    "count_tokens",
     "SwarmCloud",
-    "rate_limiter",
-    "SkyInterface",
+    "ModelAPILogEntry",
+    "log_to_supabase",
     "ChatCompletionRequest",
     "ChatCompletionRequestQos",
     "ChatCompletionResponse",
     "ChatCompletionResponseChoice",
     "ChatCompletionResponseStreamChoice",
     "ChatCompletionStreamResponse",
     "ChatMessage",
@@ -73,29 +85,19 @@
     "EmbeddingsRequest",
     "EncodeRequest",
     "EncodeResponse",
     "ErrorResponse",
     "GenerateRequest",
     "GenerateRequestQos",
     "GenerateResponse",
+    "GenerationConfig",
     "ModelCard",
     "ModelList",
     "ModelPermission",
     "UsageInfo",
-    "GenerationConfig",
-    "VariableInterface",
-    "check_api_key",
-    "get_model_list",
-    "create_error_response",
-    "check_request",
     "InputOpenAISpec",
-    "OutputOpenAISpec",
     "OpenAIAPIWrapper",
-    "calculate_pricing",
-    "authenticate_user",
-    "is_token_valid",
-    "count_tokens",
-    "ModelAPILogEntry",
-    "log_to_supabase",
-    "fetch_api_key_info",
+    "OutputOpenAISpec",
+    "generate_api_key",
+    "rate_limiter",
     "verify_token",
 ]
```

### Comparing `swarms_cloud-0.2.4/swarms_cloud/auth_with_swarms_cloud.py` & `swarms_cloud-0.2.5/swarms_cloud/auth_with_swarms_cloud.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,74 @@
 import os
 from dotenv import load_dotenv
 from fastapi import Depends, HTTPException, status, Request
 from fastapi.security import HTTPBearer, HTTPAuthorizationCredentials
-from supabase import create_client, Client
+from supabase import create_client
 
 
 # Load environment variables
 load_dotenv()
 
 # HTTP Bearer
 http_bearer = HTTPBearer()
 
 
-# Supabase client
-supabase_client_init: Client = create_client(
-    supabase_url=os.getenv("SUPABASE_URL"),
-    supabase_key=os.getenv("SUPABASE_KEY"),
-)
-
-
-def is_token_valid(token: str = None, supabase: Client = supabase_client_init) -> bool:
+def is_token_valid(
+    token: str = None,
+    #    supabase: Client = supabase_client_init
+) -> bool:
     """
     Check if a token is valid by querying the Supabase database.
 
     Args:
         token (str): The token to be checked.
         supabase (Client): The Supabase client object.
 
     Returns:
         bool: True if the token is valid, False otherwise.
     """
+    # Supabase client
+    supabase = create_client(
+        supabase_url=os.getenv("SUPABASE_URL"),
+        supabase_key=os.getenv("SUPABASE_KEY"),
+    )
+
     try:
         # Query the Supabase database to check if the token exists in the 'keys' column of the 'swarms_cloud_api_key' table
         response = (
             supabase.table("swarms_cloud_api_keys")
             .select("key")
             .filter("key", "eq", token)
             .execute()
         )
         return response["data"] is not None and len(response["data"]) > 0
     except Exception as error:
         print(f"Error checking token validity: {error}")
         return False
 
 
-def fetch_api_key_info(token: str = None, supabase: Client = supabase_client_init):
+def fetch_api_key_info(
+    token: str = None,
+    # supabase: Client = supabase_client_init
+):
     """
     Fetch the id and user_id of an API key from the Supabase database.
 
     Args:
         token (str): The API key to be checked.
         supabase (Client): The Supabase client object.
 
     Returns:
         dict: A dictionary containing the id and user_id if the API key is valid, None otherwise.
     """
+    # Supabase client
+    supabase = create_client(
+        supabase_url=os.getenv("SUPABASE_URL"),
+        supabase_key=os.getenv("SUPABASE_KEY"),
+    )
     # Query the Supabase database to check if the token exists in the 'keys' column of the 'swarms_cloud_api_key' table
     try:
         response = (
             supabase.table("swarms_cloud_api_keys")
             .select("id", "user_id", "key")
             .filter("key", "eq", token)
             .execute()
@@ -84,31 +94,30 @@
     Returns:
         str: The authentication token.
 
     Raises:
         HTTPException: If the token is invalid.
     """
     token = credentials.credentials
+    token = token.split("Bearer ")[1]
+    token = token.strip()
+    print(token)
     valid = is_token_valid(token)
     print(valid)
     if not is_token_valid(token):
         raise HTTPException(
             status_code=status.HTTP_401_UNAUTHORIZED,
             detail="Invalid token. Please authenticate with a valid token at https://swarms.world/dashboard",
             headers={"WWW-Authenticate": "Bearer"},
         )
     return token
 
 
-
 def verify_token(req: Request):
     token = req.headers["Authorization"]
     # Here your code for verifying the token or whatever you use
     token = token.split("Bearer ")[1]
     token = token.strip()
     valid = is_token_valid(token)
     if valid is False:
-        raise HTTPException(
-            status_code=401,
-            detail="Unauthorized"
-        )
-    return True
+        raise HTTPException(status_code=401, detail="Unauthorized")
+    return True
```

### Comparing `swarms_cloud-0.2.4/swarms_cloud/calculate_pricing.py` & `swarms_cloud-0.2.5/swarms_cloud/calculate_pricing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from typing import Any, List
 
 from PIL import Image
 from transformers import AutoTokenizer, PreTrainedTokenizer
 
 
-def count_tokens(
-    texts: List[str], tokenizer: PreTrainedTokenizer, model: str
-) -> int:
+def count_tokens(texts: List[str], tokenizer: PreTrainedTokenizer, model: str) -> int:
     """
     Counts the total number of tokens in a list of texts using a tokenizer.
 
     Args:
         texts (List[str]): A list of texts to count tokens from.
         tokenizer (PreTrainedTokenizer): The tokenizer to use for tokenization.
         model (str): The name or path of the pre-trained model to use.
```

### Comparing `swarms_cloud-0.2.4/swarms_cloud/func_api_wrapper.py` & `swarms_cloud-0.2.5/swarms_cloud/func_api_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms_cloud-0.2.4/swarms_cloud/log_api_request_to_supabase.py` & `swarms_cloud-0.2.5/swarms_cloud/loggers/log_api_request_to_supabase.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import os
 from pydantic import BaseModel
 from typing import Optional, Dict
 from uuid import UUID
-from supabase import Client
-from swarms_cloud.auth_with_swarms_cloud import supabase_client_init
+from supabase import create_client
+
+# from swarms_cloud.auth_with_swarms_cloud import supabase_client_init
 
 
 class ModelAPILogEntry(BaseModel):
     id: Optional[UUID] = None
     created_at: Optional[str] = None
     user_id: Optional[UUID] = None
     api_key_id: Optional[UUID] = None
@@ -25,26 +27,31 @@
     stream: Optional[bool] = None
     repetition_penalty: Optional[float] = None
 
 
 async def log_to_supabase(
     table_name: str = "swarms_cloud_api_key_activities",
     entry: ModelAPILogEntry = None,
-    supabase: Client = supabase_client_init,
+    # supabase: Client = supabase_client_init,
 ):
     """
     Logs an entry to Supabase.
 
     Args:
         table_name (str, optional): The name of the table to insert the entry into. Defaults to "swarms_cloud_api_key_activities".
         entry (LogEntry, optional): The log entry to be inserted. Defaults to None.
         supabase (Client, optional): The Supabase client instance. Defaults to None.
 
     Returns:
         dict: The response from the Supabase insert operation, or an error message if an exception occurs.
     """
+    # Supabase client
+    supabase = create_client(
+        supabase_url=os.getenv("SUPABASE_URL"),
+        supabase_key=os.getenv("SUPABASE_KEY"),
+    )
     try:
         response = supabase.table(table_name).insert(entry.model_dump()).execute()
         return response
     except Exception as error:
         print(f"Error logging to Supabase: {error}")
         return error
```

### Comparing `swarms_cloud-0.2.4/swarms_cloud/loggers/supabase_handler.py` & `swarms_cloud-0.2.5/swarms_cloud/loggers/supabase_handler.py`

 * *Files identical despite different names*

### Comparing `swarms_cloud-0.2.4/swarms_cloud/loggers/supabase_logger.py` & `swarms_cloud-0.2.5/swarms_cloud/loggers/supabase_logger.py`

 * *Files identical despite different names*

### Comparing `swarms_cloud-0.2.4/swarms_cloud/schema/cog_vlm_schemas.py` & `swarms_cloud-0.2.5/swarms_cloud/schema/cog_vlm_schemas.py`

 * *Files identical despite different names*

### Comparing `swarms_cloud-0.2.4/swarms_cloud/schema/openai_protocol.py` & `swarms_cloud-0.2.5/swarms_cloud/schema/openai_protocol.py`

 * *Files identical despite different names*

### Comparing `swarms_cloud-0.2.4/swarms_cloud/schema/openai_spec.py` & `swarms_cloud-0.2.5/swarms_cloud/schema/openai_spec.py`

 * *Files identical despite different names*

### Comparing `swarms_cloud-0.2.4/swarms_cloud/stripe_utils.py` & `swarms_cloud-0.2.5/swarms_cloud/stripe_utils.py`

 * *Files identical despite different names*

### Comparing `swarms_cloud-0.2.4/swarms_cloud/utils/api_key_generator.py` & `swarms_cloud-0.2.5/swarms_cloud/utils/api_key_generator.py`

 * *Files identical despite different names*

### Comparing `swarms_cloud-0.2.4/swarms_cloud/utils/rate_limiter.py` & `swarms_cloud-0.2.5/swarms_cloud/utils/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `swarms_cloud-0.2.4/setup.py` & `swarms_cloud-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,30 +8,29 @@
  'swarms_cloud.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['einops',
- 'exxa',
  'fastapi==0.110.0',
  'pydantic>2,<3',
  'shortuuid',
  'skypilot',
  'sse-starlette==2.0.0',
  'stripe',
  'swarms',
  'torch',
  'transformers',
  'uvicorn',
  'xformers']
 
 setup_kwargs = {
     'name': 'swarms-cloud',
-    'version': '0.2.4',
+    'version': '0.2.5',
     'description': 'Swarms Cloud - Pytorch',
     'long_description': '[![Multi-Modality](agorabanner.png)](https://discord.gg/qUtxnK2NMf)\n\n# Swarms Cloud\nInfrastructure for scalable, reliable, and economical Multi-Modal Model API serving and deployment. We\'re using terraform to orchestrate infrastructure, FastAPI to host the models. If you\'re into deploying models for millions of people, join our discord and help contribute.\n\n\n# Install\n`pip install swarms-cloud`\n\n# Examples\n\n### Example Python\n```python\nimport requests\nimport base64\nfrom PIL import Image\nfrom io import BytesIO\n\n\n# Convert image to Base64\ndef image_to_base64(image_path):\n    with Image.open(image_path) as image:\n        buffered = BytesIO()\n        image.save(buffered, format="JPEG")\n        img_str = base64.b64encode(buffered.getvalue()).decode("utf-8")\n    return img_str\n\n\n# Replace \'image.jpg\' with the path to your image\nbase64_image = image_to_base64("images/3897e80dcb0601c0.jpg")\ntext_data = {"type": "text", "text": "Describe what is in the image"}\nimage_data = {\n    "type": "image_url",\n    "image_url": {"url": f"data:image/jpeg;base64,{base64_image}"},\n}\n\n# Construct the request data\nrequest_data = {\n    "model": "cogvlm-chat-17b",\n    "messages": [{"role": "user", "content": [text_data, image_data]}],\n    "temperature": 0.8,\n    "top_p": 0.9,\n    "max_tokens": 1024,\n}\n\n# Specify the URL of your FastAPI application\nurl = "https://api.swarms.world/v1/chat/completions"\n\n# Send the request\nresponse = requests.post(url, json=request_data)\n# Print the response from the server\nprint(response.text)\n```\n\n### Example API Request in Node\n```js\nconst fs = require(\'fs\');\nconst https = require(\'https\');\nconst sharp = require(\'sharp\');\n\n// Convert image to Base64\nasync function imageToBase64(imagePath) {\n    try {\n        const imageBuffer = await sharp(imagePath).jpeg().toBuffer();\n        return imageBuffer.toString(\'base64\');\n    } catch (error) {\n        console.error(\'Error converting image to Base64:\', error);\n    }\n}\n\n// Main function to execute the workflow\nasync function main() {\n    const base64Image = await imageToBase64("images/3897e80dcb0601c0.jpg");\n    const textData = { type: "text", text: "Describe what is in the image" };\n    const imageData = {\n        type: "image_url",\n        image_url: { url: `data:image/jpeg;base64,${base64Image}` },\n    };\n\n    // Construct the request data\n    const requestData = JSON.stringify({\n        model: "cogvlm-chat-17b",\n        messages: [{ role: "user", content: [textData, imageData] }],\n        temperature: 0.8,\n        top_p: 0.9,\n        max_tokens: 1024,\n    });\n\n    const options = {\n        hostname: \'api.swarms.world\',\n        path: \'/v1/chat/completions\',\n        method: \'POST\',\n        headers: {\n            \'Content-Type\': \'application/json\',\n            \'Content-Length\': requestData.length,\n        },\n    };\n\n    const req = https.request(options, (res) => {\n        let responseBody = \'\';\n\n        res.on(\'data\', (chunk) => {\n            responseBody += chunk;\n        });\n\n        res.on(\'end\', () => {\n            console.log(\'Response:\', responseBody);\n        });\n    });\n\n    req.on(\'error\', (error) => {\n        console.error(error);\n    });\n\n    req.write(requestData);\n    req.end();\n}\n\nmain();\n```\n\n### Example API Request in Go\n\n```go\npackage main\n\nimport (\n    "bytes"\n    "encoding/base64"\n    "encoding/json"\n    "fmt"\n    "image"\n    "image/jpeg"\n    _ "image/png" // Register PNG format\n    "io"\n    "net/http"\n    "os"\n)\n\n// imageToBase64 converts an image to a Base64-encoded string.\nfunc imageToBase64(imagePath string) (string, error) {\n    file, err := os.Open(imagePath)\n    if err != nil {\n        return "", err\n    }\n    defer file.Close()\n\n    img, _, err := image.Decode(file)\n    if err != nil {\n        return "", err\n    }\n\n    buf := new(bytes.Buffer)\n    err = jpeg.Encode(buf, img, nil)\n    if err != nil {\n        return "", err\n    }\n\n    return base64.StdEncoding.EncodeToString(buf.Bytes()), nil\n}\n\n// main is the entry point of the program.\nfunc main() {\n    base64Image, err := imageToBase64("images/3897e80dcb0601c0.jpg")\n    if err != nil {\n        fmt.Println("Error converting image to Base64:", err)\n        return\n    }\n\n    requestData := map[string]interface{}{\n        "model": "cogvlm-chat-17b",\n        "messages": []map[string]interface{}{\n            {\n                "role":    "user",\n                "content": []map[string]string{{"type": "text", "text": "Describe what is in the image"}, {"type": "image_url", "image_url": {"url": fmt.Sprintf("data:image/jpeg;base64,%s", base64Image)}}},\n            },\n        },\n        "temperature": 0.8,\n        "top_p":       0.9,\n        "max_tokens":  1024,\n    }\n\n    requestBody, err := json.Marshal(requestData)\n    if err != nil {\n        fmt.Println("Error marshaling request data:", err)\n        return\n    }\n\n    url := "https://api.swarms.world/v1/chat/completions"\n    request, err := http.NewRequest("POST", url, bytes.NewBuffer(requestBody))\n    if err != nil {\n        fmt.Println("Error creating request:", err)\n        return\n    }\n\n    request.Header.Set("Content-Type", "application/json")\n\n    client := &http.Client{}\n    response, err := client.Do(request)\n    if err != nil {\n        fmt.Println("Error sending request:", err)\n        return\n    }\n    defer response.Body.Close()\n\n    responseBody, err := io.ReadAll(response.Body)\n    if err != nil {\n        fmt.Println("Error reading response body:", err)\n        return\n    }\n\n    fmt.Println("Response:", string(responseBody))\n}\n```\n\n\n\n\n\n## Calculate Pricing\n```python\nfrom transformers import AutoTokenizer\nfrom swarms_cloud import calculate_pricing\n\n# Initialize the tokenizer\ntokenizer = AutoTokenizer.from_pretrained("gpt2")\n\n# Define the example texts\ntexts = ["This is the first example text.", "This is the second example text."]\n\n# Calculate pricing and retrieve the results\ntotal_tokens, total_sentences, total_words, total_characters, total_paragraphs, cost = calculate_pricing(texts, tokenizer)\n\n# Print the total tokens processed\nprint(f"Total tokens processed: {total_tokens}")\n\n# Print the total cost\nprint(f"Total cost: ${cost:.5f}")\n```\n\n\n## Generate an API key\n```python\nfrom swarms_cloud.api_key_generator import generate_api_key\n\nout = generate_api_key(prefix="sk", length=30)\n\nprint(out)\n\n```\n\n# Stack\n- Backend: FastAPI\n- Skypilot for container management\n- Stripe for payment tracking\n- Postresql for database\n- TensorRT for inference\n- Docker for cluster management\n- Kubernetes for managing and autoscaling docker containers\n- Terraform\n\n\n# License\nMIT\n',
     'author': 'Kye Gomez',
     'author_email': 'kye@apac.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kyegomez/swarms-cloud',
```

### Comparing `swarms_cloud-0.2.4/PKG-INFO` & `swarms_cloud-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms-cloud
-Version: 0.2.4
+Version: 0.2.5
 Summary: Swarms Cloud - Pytorch
 Home-page: https://github.com/kyegomez/swarms-cloud
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.9,<4.0
@@ -14,15 +14,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: einops
-Requires-Dist: exxa
 Requires-Dist: fastapi (==0.110.0)
 Requires-Dist: pydantic (>2,<3)
 Requires-Dist: shortuuid
 Requires-Dist: skypilot
 Requires-Dist: sse-starlette (==2.0.0)
 Requires-Dist: stripe
 Requires-Dist: swarms
```

