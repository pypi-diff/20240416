# Comparing `tmp/minimax_client-0.5.2.tar.gz` & `tmp/minimax_client-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minimax_client-0.5.2.tar", last modified: Fri Apr 12 07:36:39 2024, max compression
+gzip compressed data, was "minimax_client-0.5.3.tar", last modified: Tue Apr 16 09:13:21 2024, max compression
```

## Comparing `minimax_client-0.5.2.tar` & `minimax_client-0.5.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1076 2024-03-06 04:02:14.299362 minimax_client-0.5.2/LICENSE.md
--rw-r--r--   0        0        0     9360 2024-04-12 07:21:01.123289 minimax_client-0.5.2/README.md
--rw-r--r--   0        0        0     2337 2024-04-12 07:36:39.349466 minimax_client-0.5.2/pyproject.toml
--rw-r--r--   0        0        0       78 2024-03-13 04:59:39.590202 minimax_client-0.5.2/src/minimax_client/__init__.py
--rw-r--r--   0        0        0       47 2024-04-12 07:24:30.326729 minimax_client-0.5.2/src/minimax_client/__version__.py
--rw-r--r--   0        0        0     5995 2024-04-12 06:44:51.187297 minimax_client-0.5.2/src/minimax_client/client.py
--rw-r--r--   0        0        0        0 2024-03-12 08:42:19.334547 minimax_client-0.5.2/src/minimax_client/entities/__init__.py
--rw-r--r--   0        0        0     2623 2024-04-12 05:40:39.242177 minimax_client-0.5.2/src/minimax_client/entities/assistant.py
--rw-r--r--   0        0        0     1431 2024-03-27 06:52:42.426086 minimax_client-0.5.2/src/minimax_client/entities/chat_completion.py
--rw-r--r--   0        0        0      651 2024-03-26 08:25:32.233150 minimax_client-0.5.2/src/minimax_client/entities/common.py
--rw-r--r--   0        0        0      288 2024-03-27 06:51:31.873794 minimax_client-0.5.2/src/minimax_client/entities/embedding.py
--rw-r--r--   0        0        0     1144 2024-03-27 06:50:23.603022 minimax_client-0.5.2/src/minimax_client/entities/file.py
--rw-r--r--   0        0        0     1956 2024-03-27 09:21:05.226495 minimax_client-0.5.2/src/minimax_client/entities/fine_tuning.py
--rw-r--r--   0        0        0      667 2024-04-12 07:35:53.504086 minimax_client-0.5.2/src/minimax_client/entities/thread.py
--rw-r--r--   0        0        0        0 2024-03-12 08:49:51.948241 minimax_client-0.5.2/src/minimax_client/interfaces/__init__.py
--rw-r--r--   0        0        0    23479 2024-04-12 05:59:39.461781 minimax_client-0.5.2/src/minimax_client/interfaces/assistant.py
--rw-r--r--   0        0        0      532 2024-03-15 09:50:38.059327 minimax_client-0.5.2/src/minimax_client/interfaces/base.py
--rw-r--r--   0        0        0     8832 2024-03-21 09:50:23.229159 minimax_client-0.5.2/src/minimax_client/interfaces/chat_completion.py
--rw-r--r--   0        0        0     3168 2024-03-21 09:42:08.928420 minimax_client-0.5.2/src/minimax_client/interfaces/embedding.py
--rw-r--r--   0        0        0     8150 2024-03-27 06:44:53.186708 minimax_client-0.5.2/src/minimax_client/interfaces/file.py
--rw-r--r--   0        0        0    12362 2024-03-27 07:04:43.648435 minimax_client-0.5.2/src/minimax_client/interfaces/fine_tuning.py
--rw-r--r--   0        0        0     4133 2024-04-12 07:20:40.703630 minimax_client-0.5.2/src/minimax_client/interfaces/thread.py
--rw-r--r--   0        0        0        0 2024-03-06 03:45:59.529113 minimax_client-0.5.2/tests/__init__.py
--rw-r--r--   0        0        0     2412 2024-03-25 11:51:29.057995 minimax_client-0.5.2/tests/test_client.py
--rw-r--r--   0        0        0    10420 1970-01-01 00:00:00.000000 minimax_client-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-03-06 04:02:14.299362 minimax_client-0.5.3/LICENSE.md
+-rw-r--r--   0        0        0    11623 2024-04-16 08:49:13.990564 minimax_client-0.5.3/README.md
+-rw-r--r--   0        0        0     2337 2024-04-16 09:13:21.759502 minimax_client-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-03-13 04:59:39.590202 minimax_client-0.5.3/src/minimax_client/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-16 09:12:49.636287 minimax_client-0.5.3/src/minimax_client/__version__.py
+-rw-r--r--   0        0        0     5995 2024-04-12 06:44:51.187297 minimax_client-0.5.3/src/minimax_client/client.py
+-rw-r--r--   0        0        0        0 2024-03-12 08:42:19.334547 minimax_client-0.5.3/src/minimax_client/entities/__init__.py
+-rw-r--r--   0        0        0     2840 2024-04-12 09:41:25.234703 minimax_client-0.5.3/src/minimax_client/entities/assistant.py
+-rw-r--r--   0        0        0     1431 2024-03-27 06:52:42.426086 minimax_client-0.5.3/src/minimax_client/entities/chat_completion.py
+-rw-r--r--   0        0        0      651 2024-03-26 08:25:32.233150 minimax_client-0.5.3/src/minimax_client/entities/common.py
+-rw-r--r--   0        0        0      288 2024-03-27 06:51:31.873794 minimax_client-0.5.3/src/minimax_client/entities/embedding.py
+-rw-r--r--   0        0        0     1144 2024-03-27 06:50:23.603022 minimax_client-0.5.3/src/minimax_client/entities/file.py
+-rw-r--r--   0        0        0     1956 2024-03-27 09:21:05.226495 minimax_client-0.5.3/src/minimax_client/entities/fine_tuning.py
+-rw-r--r--   0        0        0     7233 2024-04-16 09:11:38.581853 minimax_client-0.5.3/src/minimax_client/entities/thread.py
+-rw-r--r--   0        0        0        0 2024-03-12 08:49:51.948241 minimax_client-0.5.3/src/minimax_client/interfaces/__init__.py
+-rw-r--r--   0        0        0    23479 2024-04-12 05:59:39.461781 minimax_client-0.5.3/src/minimax_client/interfaces/assistant.py
+-rw-r--r--   0        0        0      532 2024-03-15 09:50:38.059327 minimax_client-0.5.3/src/minimax_client/interfaces/base.py
+-rw-r--r--   0        0        0     8832 2024-03-21 09:50:23.229159 minimax_client-0.5.3/src/minimax_client/interfaces/chat_completion.py
+-rw-r--r--   0        0        0     3168 2024-03-21 09:42:08.928420 minimax_client-0.5.3/src/minimax_client/interfaces/embedding.py
+-rw-r--r--   0        0        0     8150 2024-03-27 06:44:53.186708 minimax_client-0.5.3/src/minimax_client/interfaces/file.py
+-rw-r--r--   0        0        0    12362 2024-03-27 07:04:43.648435 minimax_client-0.5.3/src/minimax_client/interfaces/fine_tuning.py
+-rw-r--r--   0        0        0    27437 2024-04-16 09:10:10.160861 minimax_client-0.5.3/src/minimax_client/interfaces/thread.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:45:59.529113 minimax_client-0.5.3/tests/__init__.py
+-rw-r--r--   0        0        0     2412 2024-03-25 11:51:29.057995 minimax_client-0.5.3/tests/test_client.py
+-rw-r--r--   0        0        0    12592 1970-01-01 00:00:00.000000 minimax_client-0.5.3/PKG-INFO
```

### Comparing `minimax_client-0.5.2/LICENSE.md` & `minimax_client-0.5.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.2/README.md` & `minimax_client-0.5.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 - Embeddings
 - File
 - Finetune
 - Assistants
     - Assistant
     - Assistant File
     - Thread
+    - Message
+    - Run
 
 ## Prerequisites
 - Python >= 3.8
 - pip (or any other tool that does the same job)
 - Internet connection
 - An API KEY acquired from [MiniMax Open Platform](https://www.minimaxi.com/user-center/basic-information/interface-key)
 
@@ -360,21 +362,110 @@
 resp = client.assistants.files.retrieve(assistant_id=assistant_id, file_id=str(file_id))
 
 resp = client.assistants.files.list(assistant_id=assistant_id, limit=5, order="asc")
 
 resp = client.assistants.files.delete(assistant_id=assistant_id, file_id=str(file_id))
 ```
 
-#### 2.13 Sync call for threads
+#### 2.13 Sync call for assistant threads
 
 ```python
 from minimax_client import MiniMax
 
 
 client = MiniMax(api_key="<YOUR_API_KEY>")
 
 resp = client.threads.create(metadata={"key": "value"})
 
 resp = client.threads.retrieve(thread_id=resp.id)
 
 resp = client.threads.update(thread_id=resp.id, metadata={"key": "value2"})
 ```
+
+#### 2.14 Sync call for assistant messages
+
+```python
+import time
+
+from minimax_client import MiniMax
+
+
+client = MiniMax(api_key="<YOUR_API_KEY>")
+
+resp = client.threads.create(metadata={"key": "value"})
+
+thread_id = resp.id
+
+resp = client.threads.messages.create(
+    thread_id=thread_id, content="Hello", role="user", metadata={"key": "value"}
+)
+
+resp = client.threads.messages.retrieve(thread_id=thread_id, message_id=resp.id)
+
+resp = client.threads.messages.list(thread_id=thread_id, limit=5, order="asc")
+```
+
+#### 2.15 Sync call for assistant runs and run steps
+
+```python
+from minimax_client import MiniMax
+
+
+client = MiniMax(api_key="<YOUR_API_KEY>")
+
+resp = client.assistants.create(
+    model="abab5.5-chat",
+    name="test-assistant",
+    instructions="You are a helpful assistant that can use tools to answer questions.",
+    tools=[
+        {
+            "type": "function",
+            "function": {
+                "name": "get_weather",
+                "description": "get weather",
+                "parameters": {
+                    "type": "object",
+                    "required": ["city"],
+                    "properties": {"city": {"type": "string"}},
+                },
+            },
+        },
+        {"type": "web_search"},
+        {"type": "code_interpreter"},
+    ],
+)
+
+assistant_id = resp.id
+
+resp = client.assistants.retrieve(assistant_id=assistant_id)
+
+print(resp.model_dump())
+
+resp = client.threads.create(metadata={"key1": "value1"})
+
+thread_id = resp.id
+
+client.threads.messages.create(
+    thread_id=thread_id,
+    role="user",
+    content="In the science-fiction 'Three-Body Problem', what is the profession of Wang Miao?",
+)
+
+resp = client.threads.runs.create(thread_id=thread_id, assistant_id=assistant_id)
+
+run_id = resp.id
+
+time.sleep(10)
+
+resp = client.threads.runs.retrieve(run_id=run_id, thread_id=thread_id)
+
+print(resp.model_dump())
+
+resp = client.threads.runs.steps.list(thread_id=thread_id, run_id=run_id, limit=10)
+
+for step in resp.data:
+    resp = client.threads.runs.steps.retrieve(
+        step_id=step.id, thread_id=thread_id, run_id=run_id
+    )
+
+    print(resp.model_dump())
+```
```

### Comparing `minimax_client-0.5.2/pyproject.toml` & `minimax_client-0.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP",
     "Typing :: Typed",
 ]
 dynamic = []
-version = "0.5.2"
+version = "0.5.3"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 dev = [
     "pytest>=8.1.1,<9",
```

### Comparing `minimax_client-0.5.2/src/minimax_client/client.py` & `minimax_client-0.5.3/src/minimax_client/client.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.2/src/minimax_client/entities/assistant.py` & `minimax_client-0.5.3/src/minimax_client/entities/assistant.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,28 @@
 from typing import Dict, List, Literal, Optional
 
 from pydantic import BaseModel, PositiveInt
 
 from minimax_client.entities.common import BareResponse
 
 
+class AssistantToolFunctionParameters(BaseModel):
+    """Assistant Tool Function Parameters"""
+
+    type: Literal["object"]
+    required: List[str]
+    properties: Dict[str, Dict]
+
+
 class AssistantToolFunction(BaseModel):
     """Assistant Tool Function"""
 
     description: str
     name: str
-    parameters: Optional[Dict] = None
+    parameters: Optional[AssistantToolFunctionParameters] = None
 
 
 class AssistantTool(BaseModel):
     """Assistant Tool"""
 
     type: Literal["code_interpreter", "retrieval", "function", "web_search"]
     function: Optional[AssistantToolFunction] = None
```

### Comparing `minimax_client-0.5.2/src/minimax_client/entities/chat_completion.py` & `minimax_client-0.5.3/src/minimax_client/entities/chat_completion.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.2/src/minimax_client/entities/common.py` & `minimax_client-0.5.3/src/minimax_client/entities/common.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.2/src/minimax_client/entities/file.py` & `minimax_client-0.5.3/src/minimax_client/entities/file.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.2/src/minimax_client/entities/fine_tuning.py` & `minimax_client-0.5.3/src/minimax_client/entities/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.2/src/minimax_client/interfaces/assistant.py` & `minimax_client-0.5.3/src/minimax_client/interfaces/assistant.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.2/src/minimax_client/interfaces/base.py` & `minimax_client-0.5.3/src/minimax_client/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.2/src/minimax_client/interfaces/chat_completion.py` & `minimax_client-0.5.3/src/minimax_client/interfaces/chat_completion.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.2/src/minimax_client/interfaces/embedding.py` & `minimax_client-0.5.3/src/minimax_client/interfaces/embedding.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.2/src/minimax_client/interfaces/file.py` & `minimax_client-0.5.3/src/minimax_client/interfaces/file.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.2/src/minimax_client/interfaces/fine_tuning.py` & `minimax_client-0.5.3/src/minimax_client/interfaces/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.2/tests/test_client.py` & `minimax_client-0.5.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.2/PKG-INFO` & `minimax_client-0.5.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: minimax-client
-Version: 0.5.2
+Version: 0.5.3
 Summary: An (unofficial) python native client for easy interaction with MiniMax Open Platform
-Keywords: web api llm
+Keywords: web,api,llm
 Author-Email: Zeyang Lin <4020306+linzeyang@users.noreply.github.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
@@ -49,14 +49,16 @@
 - Embeddings
 - File
 - Finetune
 - Assistants
     - Assistant
     - Assistant File
     - Thread
+    - Message
+    - Run
 
 ## Prerequisites
 - Python >= 3.8
 - pip (or any other tool that does the same job)
 - Internet connection
 - An API KEY acquired from [MiniMax Open Platform](https://www.minimaxi.com/user-center/basic-information/interface-key)
 
@@ -394,21 +396,110 @@
 resp = client.assistants.files.retrieve(assistant_id=assistant_id, file_id=str(file_id))
 
 resp = client.assistants.files.list(assistant_id=assistant_id, limit=5, order="asc")
 
 resp = client.assistants.files.delete(assistant_id=assistant_id, file_id=str(file_id))
 ```
 
-#### 2.13 Sync call for threads
+#### 2.13 Sync call for assistant threads
 
 ```python
 from minimax_client import MiniMax
 
 
 client = MiniMax(api_key="<YOUR_API_KEY>")
 
 resp = client.threads.create(metadata={"key": "value"})
 
 resp = client.threads.retrieve(thread_id=resp.id)
 
 resp = client.threads.update(thread_id=resp.id, metadata={"key": "value2"})
 ```
+
+#### 2.14 Sync call for assistant messages
+
+```python
+import time
+
+from minimax_client import MiniMax
+
+
+client = MiniMax(api_key="<YOUR_API_KEY>")
+
+resp = client.threads.create(metadata={"key": "value"})
+
+thread_id = resp.id
+
+resp = client.threads.messages.create(
+    thread_id=thread_id, content="Hello", role="user", metadata={"key": "value"}
+)
+
+resp = client.threads.messages.retrieve(thread_id=thread_id, message_id=resp.id)
+
+resp = client.threads.messages.list(thread_id=thread_id, limit=5, order="asc")
+```
+
+#### 2.15 Sync call for assistant runs and run steps
+
+```python
+from minimax_client import MiniMax
+
+
+client = MiniMax(api_key="<YOUR_API_KEY>")
+
+resp = client.assistants.create(
+    model="abab5.5-chat",
+    name="test-assistant",
+    instructions="You are a helpful assistant that can use tools to answer questions.",
+    tools=[
+        {
+            "type": "function",
+            "function": {
+                "name": "get_weather",
+                "description": "get weather",
+                "parameters": {
+                    "type": "object",
+                    "required": ["city"],
+                    "properties": {"city": {"type": "string"}},
+                },
+            },
+        },
+        {"type": "web_search"},
+        {"type": "code_interpreter"},
+    ],
+)
+
+assistant_id = resp.id
+
+resp = client.assistants.retrieve(assistant_id=assistant_id)
+
+print(resp.model_dump())
+
+resp = client.threads.create(metadata={"key1": "value1"})
+
+thread_id = resp.id
+
+client.threads.messages.create(
+    thread_id=thread_id,
+    role="user",
+    content="In the science-fiction 'Three-Body Problem', what is the profession of Wang Miao?",
+)
+
+resp = client.threads.runs.create(thread_id=thread_id, assistant_id=assistant_id)
+
+run_id = resp.id
+
+time.sleep(10)
+
+resp = client.threads.runs.retrieve(run_id=run_id, thread_id=thread_id)
+
+print(resp.model_dump())
+
+resp = client.threads.runs.steps.list(thread_id=thread_id, run_id=run_id, limit=10)
+
+for step in resp.data:
+    resp = client.threads.runs.steps.retrieve(
+        step_id=step.id, thread_id=thread_id, run_id=run_id
+    )
+
+    print(resp.model_dump())
+```
```

