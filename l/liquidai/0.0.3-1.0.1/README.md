# Comparing `tmp/liquidai-0.0.3.tar.gz` & `tmp/liquidai-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liquidai-0.0.3.tar", last modified: Wed Dec 20 02:22:45 2023, max compression
+gzip compressed data, was "liquidai-1.0.1.tar", last modified: Tue Apr 16 21:21:30 2024, max compression
```

## Comparing `liquidai-0.0.3.tar` & `liquidai-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 mathias   (1000) mathias   (1000)        0 2023-12-20 02:22:45.722420 liquidai-0.0.3/
--rw-rw-r--   0 mathias   (1000) mathias   (1000)    11357 2023-12-01 21:11:25.000000 liquidai-0.0.3/LICENSE
--rw-r--r--   0 mathias   (1000) mathias   (1000)    16806 2023-12-20 02:22:45.722420 liquidai-0.0.3/PKG-INFO
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     3305 2023-12-08 02:08:11.000000 liquidai-0.0.3/README.md
-drwxrwxr-x   0 mathias   (1000) mathias   (1000)        0 2023-12-20 02:22:45.718420 liquidai-0.0.3/liquidai/
--rw-rw-r--   0 mathias   (1000) mathias   (1000)       35 2023-12-05 00:15:31.000000 liquidai-0.0.3/liquidai/__init__.py
--rw-rw-r--   0 mathias   (1000) mathias   (1000)     5595 2023-12-20 02:19:41.000000 liquidai-0.0.3/liquidai/client.py
-drwxrwxr-x   0 mathias   (1000) mathias   (1000)        0 2023-12-20 02:22:45.722420 liquidai-0.0.3/liquidai.egg-info/
--rw-r--r--   0 mathias   (1000) mathias   (1000)    16806 2023-12-20 02:22:45.000000 liquidai-0.0.3/liquidai.egg-info/PKG-INFO
--rw-rw-r--   0 mathias   (1000) mathias   (1000)      231 2023-12-20 02:22:45.000000 liquidai-0.0.3/liquidai.egg-info/SOURCES.txt
--rw-rw-r--   0 mathias   (1000) mathias   (1000)        1 2023-12-20 02:22:45.000000 liquidai-0.0.3/liquidai.egg-info/dependency_links.txt
--rw-rw-r--   0 mathias   (1000) mathias   (1000)        6 2023-12-20 02:22:45.000000 liquidai-0.0.3/liquidai.egg-info/requires.txt
--rw-rw-r--   0 mathias   (1000) mathias   (1000)        9 2023-12-20 02:22:45.000000 liquidai-0.0.3/liquidai.egg-info/top_level.txt
--rw-rw-r--   0 mathias   (1000) mathias   (1000)      710 2023-12-20 02:22:06.000000 liquidai-0.0.3/pyproject.toml
--rw-rw-r--   0 mathias   (1000) mathias   (1000)       38 2023-12-20 02:22:45.722420 liquidai-0.0.3/setup.cfg
+drwxrwxr-x   0 mathias   (1000) mathias   (1000)        0 2024-04-16 21:21:30.127659 liquidai-1.0.1/
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)    11357 2023-12-01 21:11:25.000000 liquidai-1.0.1/LICENSE
+-rw-r--r--   0 mathias   (1000) mathias   (1000)    17325 2024-04-16 21:21:30.127659 liquidai-1.0.1/PKG-INFO
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     3794 2024-04-16 21:21:04.000000 liquidai-1.0.1/README.md
+drwxrwxr-x   0 mathias   (1000) mathias   (1000)        0 2024-04-16 21:21:30.127659 liquidai-1.0.1/liquidai/
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)       35 2023-12-05 00:15:31.000000 liquidai-1.0.1/liquidai/__init__.py
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)     5847 2024-04-16 21:21:04.000000 liquidai-1.0.1/liquidai/client.py
+drwxrwxr-x   0 mathias   (1000) mathias   (1000)        0 2024-04-16 21:21:30.127659 liquidai-1.0.1/liquidai.egg-info/
+-rw-r--r--   0 mathias   (1000) mathias   (1000)    17325 2024-04-16 21:21:30.000000 liquidai-1.0.1/liquidai.egg-info/PKG-INFO
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)      231 2024-04-16 21:21:30.000000 liquidai-1.0.1/liquidai.egg-info/SOURCES.txt
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)        1 2024-04-16 21:21:30.000000 liquidai-1.0.1/liquidai.egg-info/dependency_links.txt
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)        6 2024-04-16 21:21:30.000000 liquidai-1.0.1/liquidai.egg-info/requires.txt
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)        9 2024-04-16 21:21:30.000000 liquidai-1.0.1/liquidai.egg-info/top_level.txt
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)      760 2024-04-16 21:21:23.000000 liquidai-1.0.1/pyproject.toml
+-rw-rw-r--   0 mathias   (1000) mathias   (1000)       38 2024-04-16 21:21:30.127659 liquidai-1.0.1/setup.cfg
```

### Comparing `liquidai-0.0.3/LICENSE` & `liquidai-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `liquidai-0.0.3/PKG-INFO` & `liquidai-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: liquidai
-Version: 0.0.3
+Version: 1.0.1
 Summary: Client library for the Liquid AI API
-Author-email: Mathias Lechner <mathias@liquid.ai>
+Author-email: Mathias Lechner <mathias@liquid.ai>, Kelvin He <kelvin@liquid.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
@@ -219,38 +219,46 @@
 # Python Client for the Liquid API
 
 ## 📦 Installation
 ```bash
 pip install -U liquidai
 ```
 
-## 💬 Basic Usage
+## OpenAI compatible API
+For openai and langchain compatible apis like `/chat/completions` and `/embeddings`. 
 
-To access the API you need to set the environment variables `LIQUID_URL` and `LIQUID_API_KEY` to the UR and your API key of your Liquid AI subscription respectively.
-You can find your API key in the My Account page of the Liquid platform (left bottom icon in the navigation bar).
+Examples:
+- [openai](https://github.com/Liquid4All/liquid_client/tree/main/examples/openai/chat_completion.ipynb)
+- [langchain](https://github.com/Liquid4All/liquid_client/tree/main/examples/langchain/chat_openai.ipynb)
+
+## 💬 Other liquid api endpoints
+For retrieval augmentation enabled liquidai api endpoints like `/complete` with files as arguments.
+
+To access these APIs you need to set the environment variables `LIQUID_URL` and `LIQUID_API_KEY` to the UR and your API key of your Liquid AI subscription respectively.
+You can find your API key in the profile tab of the Liquid platform (left bottom icon in the navigation bar).
 
 🔐 **API Keys** The most secure way to set the environment variables, which the Liquid client will automatically use.
 ```bash
-export LIQUID_URL="https://...."
+export LIQUID_URL="https://labs.liquid.ai/api/v1"
 export LIQUID_API_KEY="9cba1....."
 ```
 
-Alternatively, you can also pass the `api_url` and `api_key` parameters to the `Client` constructor.
+Alternatively, you can also pass the `base_url` and `api_key` parameters to the `Client` constructor.
 ```python
 # Create a client object with the API URL and API key
 client = Client()
 print("Models: ", client.list_models()) # List all models
 # Create a conversation with the model (a list of messages)
 chat = [{"role": "user", "content": "Hello world in python!"}]
 response = client.complete(chat)
 print(f"Response: {response['message']['content']}")
 ```
 Output:
 ```
->>> Models:  ['liquid0']
+>>> Models:  ['liquid-beacon-1.0']
 >>> Response: Here is how to code a Hello World program in Python: print("Hello, world!")
 ```
 
 Multi-turn conversations:
 ```python
 chat.append(response["message"]) # add assistant message to conversation
 chat.append({"role": "user", "content": "And in C++?"})
@@ -314,12 +322,12 @@
 ```
 >>> Deleted test.txt
 >>> Files: []
 ```
 
 ## 📌 Full Examples
 
-- [Quickstart](https://github.com/Liquid4All/liquid_client/tree/main/examples/hello_world.py) Full example of the basic usage described above.
-- [AI2 Reasoning Challenge](https://github.com/Liquid4All/liquid_client/tree/main/examples/run_ai2rc.py) Runs the AI2 Reasoning Challenge via the Liquid platform.
-- [Code clone detection benchmark](https://github.com/Liquid4All/liquid_client/blob/main/examples/code_clone_detection.py) Runs part of the Codegluex code clone detection benchmark
+- [Quickstart](https://github.com/Liquid4All/liquid_client/tree/main/examples/liquid_api.ipynb) Full example of the basic usage described above.
+- [AI2 Reasoning Challenge](https://github.com/Liquid4All/liquid_client/tree/main/examples/evals/run_ai2rc.py) Runs the AI2 Reasoning Challenge via the Liquid platform.
+- [Code clone detection benchmark](https://github.com/Liquid4All/liquid_client/blob/main/examples/evals/code_clone_detection.py) Runs part of the Codegluex code clone detection benchmark
 - [Upload multiple files](https://github.com/Liquid4All/liquid_client/tree/main/examples/upload_folder.py) Script to upload a folder of files to the Liquid platform.
```

### Comparing `liquidai-0.0.3/README.md` & `liquidai-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 # Python Client for the Liquid API
 
 ## 📦 Installation
 ```bash
 pip install -U liquidai
 ```
 
-## 💬 Basic Usage
+## OpenAI compatible API
+For openai and langchain compatible apis like `/chat/completions` and `/embeddings`. 
 
-To access the API you need to set the environment variables `LIQUID_URL` and `LIQUID_API_KEY` to the UR and your API key of your Liquid AI subscription respectively.
-You can find your API key in the My Account page of the Liquid platform (left bottom icon in the navigation bar).
+Examples:
+- [openai](https://github.com/Liquid4All/liquid_client/tree/main/examples/openai/chat_completion.ipynb)
+- [langchain](https://github.com/Liquid4All/liquid_client/tree/main/examples/langchain/chat_openai.ipynb)
+
+## 💬 Other liquid api endpoints
+For retrieval augmentation enabled liquidai api endpoints like `/complete` with files as arguments.
+
+To access these APIs you need to set the environment variables `LIQUID_URL` and `LIQUID_API_KEY` to the UR and your API key of your Liquid AI subscription respectively.
+You can find your API key in the profile tab of the Liquid platform (left bottom icon in the navigation bar).
 
 🔐 **API Keys** The most secure way to set the environment variables, which the Liquid client will automatically use.
 ```bash
-export LIQUID_URL="https://...."
+export LIQUID_URL="https://labs.liquid.ai/api/v1"
 export LIQUID_API_KEY="9cba1....."
 ```
 
-Alternatively, you can also pass the `api_url` and `api_key` parameters to the `Client` constructor.
+Alternatively, you can also pass the `base_url` and `api_key` parameters to the `Client` constructor.
 ```python
 # Create a client object with the API URL and API key
 client = Client()
 print("Models: ", client.list_models()) # List all models
 # Create a conversation with the model (a list of messages)
 chat = [{"role": "user", "content": "Hello world in python!"}]
 response = client.complete(chat)
 print(f"Response: {response['message']['content']}")
 ```
 Output:
 ```
->>> Models:  ['liquid0']
+>>> Models:  ['liquid-beacon-1.0']
 >>> Response: Here is how to code a Hello World program in Python: print("Hello, world!")
 ```
 
 Multi-turn conversations:
 ```python
 chat.append(response["message"]) # add assistant message to conversation
 chat.append({"role": "user", "content": "And in C++?"})
@@ -96,12 +104,12 @@
 ```
 >>> Deleted test.txt
 >>> Files: []
 ```
 
 ## 📌 Full Examples
 
-- [Quickstart](https://github.com/Liquid4All/liquid_client/tree/main/examples/hello_world.py) Full example of the basic usage described above.
-- [AI2 Reasoning Challenge](https://github.com/Liquid4All/liquid_client/tree/main/examples/run_ai2rc.py) Runs the AI2 Reasoning Challenge via the Liquid platform.
-- [Code clone detection benchmark](https://github.com/Liquid4All/liquid_client/blob/main/examples/code_clone_detection.py) Runs part of the Codegluex code clone detection benchmark
+- [Quickstart](https://github.com/Liquid4All/liquid_client/tree/main/examples/liquid_api.ipynb) Full example of the basic usage described above.
+- [AI2 Reasoning Challenge](https://github.com/Liquid4All/liquid_client/tree/main/examples/evals/run_ai2rc.py) Runs the AI2 Reasoning Challenge via the Liquid platform.
+- [Code clone detection benchmark](https://github.com/Liquid4All/liquid_client/blob/main/examples/evals/code_clone_detection.py) Runs part of the Codegluex code clone detection benchmark
 - [Upload multiple files](https://github.com/Liquid4All/liquid_client/tree/main/examples/upload_folder.py) Script to upload a folder of files to the Liquid platform.
```

### Comparing `liquidai-0.0.3/liquidai/client.py` & `liquidai-1.0.1/liquidai/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import httpx
 import os
+import json
 
 
 class Client:
     def __init__(self, base_url=None, api_key=None):
         if base_url is None:
             if "LIQUID_URL" not in os.environ:
                 raise ValueError(
@@ -12,14 +13,18 @@
             base_url = os.environ["LIQUID_URL"]
         if api_key is None:
             if "LIQUID_API_KEY" not in os.environ:
                 raise ValueError(
                     "API key not found. Please set LIQUID_API_KEY environment variable or pass in the api_key argument."
                 )
             api_key = os.environ["LIQUID_API_KEY"]
+        if base_url.endswith("#"):
+            base_url = base_url[:-1]
+        if base_url.endswith("/"):
+            base_url = base_url[:-1]
         self.base_url = base_url
         self.api_key = api_key
         self.client = httpx.Client(headers={"X-API-Key": self.api_key})
 
     def _check_for_errors(self, response):
         if response.status_code == 404:
             raise FileNotFoundError("Error: " + response.text)
@@ -34,64 +39,66 @@
         elif response.status_code != 200:
             raise ValueError("Error: " + response.text)
 
     def list_models(self):
         """List all available models.
         returns: A list of model names"""
 
-        response = self.client.get(self.base_url + "/api/list_models")
+        response = self.client.get(self.base_url + "/list_models")
         self._check_for_errors(response)
         response = response.json()
         return response
 
     def delete_file(self, filename):
         """Deletes a file.
         filename: The name of the file to delete."""
+        payload = json.dumps({"name": filename})  # Manually prepare the JSON payload
 
         response = self.client.post(
-            self.base_url + "/api/delete_file",
-            json={"filename": filename},
+            self.base_url + "/delete_file",
+            json={"name": filename},
         )
         self._check_for_errors(response)
         response = response.json()
         return response
 
     def list_files(self):
         """List all files stored on the server by the user.
         returns: A list of filenames"""
 
         response = self.client.get(
-            self.base_url + "/api/list_files",
+            self.base_url + "/list_files",
         )
         self._check_for_errors(response)
         response = response.json()
         return response
 
     def upload_file(self, path, filename=None):
         """Uploads a file to the server.
         path: The path to the file to upload.
         filename: The name of the file to upload. If None, the basename of path is used.
         """
 
         if filename is None:
             filename = os.path.basename(path)
         with open(path, "rb") as f:
+            print(f)
             response = self.client.post(
-                self.base_url + "/api/upload_file",
+                self.base_url + "/upload_file",
                 files={"file": (filename, f)},
                 timeout=60,
             )
         self._check_for_errors(response)
         response = response.json()
         return response
 
     def complete(
         self,
         messages,
-        model="auto",
+        model="liquid-beacon-1.0",
         max_new_tokens=384,
         top_p=0.9,
         temperature=0.9,
         top_k=0,
     ):
         """Completes a conversation.
         messages: A list of messages. Each message is a dictionary with the following keys: role, content, files.
@@ -104,15 +111,15 @@
             "model": model,
             "max_new_tokens": max_new_tokens,
             "top_p": top_p,
             "temperature": temperature,
             "top_k": top_k,
         }
         response = self.client.post(
-            self.base_url + "/api/complete",
+            self.base_url + "/complete",
             json=data,
             timeout=60,
         )
         self._check_for_errors(response)
         response = response.json()
         if response["status"] == "error":
             raise ValueError("Error: " + response["message"])
```

### Comparing `liquidai-0.0.3/liquidai.egg-info/PKG-INFO` & `liquidai-1.0.1/liquidai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: liquidai
-Version: 0.0.3
+Version: 1.0.1
 Summary: Client library for the Liquid AI API
-Author-email: Mathias Lechner <mathias@liquid.ai>
+Author-email: Mathias Lechner <mathias@liquid.ai>, Kelvin He <kelvin@liquid.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
@@ -219,38 +219,46 @@
 # Python Client for the Liquid API
 
 ## 📦 Installation
 ```bash
 pip install -U liquidai
 ```
 
-## 💬 Basic Usage
+## OpenAI compatible API
+For openai and langchain compatible apis like `/chat/completions` and `/embeddings`. 
 
-To access the API you need to set the environment variables `LIQUID_URL` and `LIQUID_API_KEY` to the UR and your API key of your Liquid AI subscription respectively.
-You can find your API key in the My Account page of the Liquid platform (left bottom icon in the navigation bar).
+Examples:
+- [openai](https://github.com/Liquid4All/liquid_client/tree/main/examples/openai/chat_completion.ipynb)
+- [langchain](https://github.com/Liquid4All/liquid_client/tree/main/examples/langchain/chat_openai.ipynb)
+
+## 💬 Other liquid api endpoints
+For retrieval augmentation enabled liquidai api endpoints like `/complete` with files as arguments.
+
+To access these APIs you need to set the environment variables `LIQUID_URL` and `LIQUID_API_KEY` to the UR and your API key of your Liquid AI subscription respectively.
+You can find your API key in the profile tab of the Liquid platform (left bottom icon in the navigation bar).
 
 🔐 **API Keys** The most secure way to set the environment variables, which the Liquid client will automatically use.
 ```bash
-export LIQUID_URL="https://...."
+export LIQUID_URL="https://labs.liquid.ai/api/v1"
 export LIQUID_API_KEY="9cba1....."
 ```
 
-Alternatively, you can also pass the `api_url` and `api_key` parameters to the `Client` constructor.
+Alternatively, you can also pass the `base_url` and `api_key` parameters to the `Client` constructor.
 ```python
 # Create a client object with the API URL and API key
 client = Client()
 print("Models: ", client.list_models()) # List all models
 # Create a conversation with the model (a list of messages)
 chat = [{"role": "user", "content": "Hello world in python!"}]
 response = client.complete(chat)
 print(f"Response: {response['message']['content']}")
 ```
 Output:
 ```
->>> Models:  ['liquid0']
+>>> Models:  ['liquid-beacon-1.0']
 >>> Response: Here is how to code a Hello World program in Python: print("Hello, world!")
 ```
 
 Multi-turn conversations:
 ```python
 chat.append(response["message"]) # add assistant message to conversation
 chat.append({"role": "user", "content": "And in C++?"})
@@ -314,12 +322,12 @@
 ```
 >>> Deleted test.txt
 >>> Files: []
 ```
 
 ## 📌 Full Examples
 
-- [Quickstart](https://github.com/Liquid4All/liquid_client/tree/main/examples/hello_world.py) Full example of the basic usage described above.
-- [AI2 Reasoning Challenge](https://github.com/Liquid4All/liquid_client/tree/main/examples/run_ai2rc.py) Runs the AI2 Reasoning Challenge via the Liquid platform.
-- [Code clone detection benchmark](https://github.com/Liquid4All/liquid_client/blob/main/examples/code_clone_detection.py) Runs part of the Codegluex code clone detection benchmark
+- [Quickstart](https://github.com/Liquid4All/liquid_client/tree/main/examples/liquid_api.ipynb) Full example of the basic usage described above.
+- [AI2 Reasoning Challenge](https://github.com/Liquid4All/liquid_client/tree/main/examples/evals/run_ai2rc.py) Runs the AI2 Reasoning Challenge via the Liquid platform.
+- [Code clone detection benchmark](https://github.com/Liquid4All/liquid_client/blob/main/examples/evals/code_clone_detection.py) Runs part of the Codegluex code clone detection benchmark
 - [Upload multiple files](https://github.com/Liquid4All/liquid_client/tree/main/examples/upload_folder.py) Script to upload a folder of files to the Liquid platform.
```

### Comparing `liquidai-0.0.3/pyproject.toml` & `liquidai-1.0.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["liquidai"]
 
 [project]
 name = "liquidai"
-version = "0.0.3"
+version = "1.0.1"
 dependencies = [
   "httpx",
 ]
 requires-python = ">=3.6"
 authors = [
   {name = "Mathias Lechner", email = "mathias@liquid.ai"},
+  {name = "Kelvin He", email = "kelvin@liquid.ai"}
 ]
 description = "Client library for the Liquid AI API"
 readme = "README.md"
 license = {file = "LICENSE", name = "Apache License 2.0"}
 keywords = ["liquidai", "api",]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python"
 ]
 
 [project.urls]
 Homepage = "https://liquid.ai"
 Documentation = "https://readthedocs.org"
 Repository = "https://github.com/Liquid4All/liquid_client"
-
```

