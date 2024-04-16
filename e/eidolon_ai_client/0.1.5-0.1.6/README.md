# Comparing `tmp/eidolon_ai_client-0.1.5.tar.gz` & `tmp/eidolon_ai_client-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eidolon_ai_client-0.1.5.tar", max compression
+gzip compressed data, was "eidolon_ai_client-0.1.6.tar", max compression
```

## Comparing `eidolon_ai_client-0.1.5.tar` & `eidolon_ai_client-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2024-03-19 21:53:03.480237 eidolon_ai_client-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-03-19 21:53:03.480237 eidolon_ai_client-0.1.5/eidolon_ai_client/__init__.py
--rw-r--r--   0        0        0     6367 2024-03-19 21:53:03.480237 eidolon_ai_client-0.1.5/eidolon_ai_client/client.py
--rw-r--r--   0        0        0     4812 2024-03-19 21:53:03.480237 eidolon_ai_client-0.1.5/eidolon_ai_client/events.py
--rw-r--r--   0        0        0     2387 2024-03-19 21:53:03.480237 eidolon_ai_client-0.1.5/eidolon_ai_client/group_conversation.py
--rw-r--r--   0        0        0        0 2024-03-19 21:53:03.480237 eidolon_ai_client-0.1.5/eidolon_ai_client/util/__init__.py
--rw-r--r--   0        0        0     3341 2024-03-19 21:53:03.480237 eidolon_ai_client-0.1.5/eidolon_ai_client/util/aiohttp.py
--rw-r--r--   0        0        0      448 2024-03-19 21:53:03.480237 eidolon_ai_client-0.1.5/eidolon_ai_client/util/logger.py
--rw-r--r--   0        0        0     2361 2024-03-19 21:53:03.480237 eidolon_ai_client-0.1.5/eidolon_ai_client/util/request_context.py
--rw-r--r--   0        0        0      424 2024-03-19 21:53:03.480237 eidolon_ai_client-0.1.5/eidolon_ai_client/util/stream_collector.py
--rw-r--r--   0        0        0      541 2024-03-19 21:53:03.480237 eidolon_ai_client-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 eidolon_ai_client-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/__init__.py
+-rw-r--r--   0        0        0     7297 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/client.py
+-rw-r--r--   0        0        0     4987 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/events.py
+-rw-r--r--   0        0        0     2387 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/group_conversation.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/util/__init__.py
+-rw-r--r--   0        0        0     3728 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/util/aiohttp.py
+-rw-r--r--   0        0        0      448 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/util/logger.py
+-rw-r--r--   0        0        0     2361 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/util/request_context.py
+-rw-r--r--   0        0        0      424 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/util/stream_collector.py
+-rw-r--r--   0        0        0      541 2024-04-16 01:18:28.711470 eidolon_ai_client-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 eidolon_ai_client-0.1.6/PKG-INFO
```

### Comparing `eidolon_ai_client-0.1.5/eidolon_ai_client/client.py` & `eidolon_ai_client-0.1.6/eidolon_ai_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import os
 from typing import List, Any, AsyncIterator, Optional
 from urllib.parse import urljoin
 
 import jsonref
 from pydantic import BaseModel, Field, Extra
 
-from eidolon_ai_client.events import StreamEvent, StartAgentCallEvent, AgentStateEvent
-from eidolon_ai_client.util.aiohttp import stream_content, get_content, post_content, delete
+from eidolon_ai_client.events import StreamEvent, StartAgentCallEvent, AgentStateEvent, FileHandle
+from eidolon_ai_client.util.aiohttp import stream_content, get_content, post_content, delete, get_raw
 
 
 def current_machine_url() -> str:
     return os.environ.get("EIDOLON_LOCAL_MACHINE", "http://localhost:8080")
 
 
 class Machine(BaseModel):
@@ -25,15 +25,14 @@
 
     def agent(self, agent_name: str) -> Agent:
         return Agent(machine=self.machine, agent=agent_name)
 
     async def processes(self) -> ProcessesResponse:
         url = urljoin(self.machine, "/processes")
         json_ = await get_content(url)
-        print(json_)
         json_['processes'] = [{"machine":self.machine, **kwargs} for kwargs in json_['processes']]
         return ProcessesResponse(**json_)
 
 
 class Agent(BaseModel):
     machine: str = Field(default_factory=current_machine_url)
     agent: str
@@ -52,15 +51,15 @@
 
     async def processes(self) -> ProcessesResponse:
         url = urljoin(self.machine, "/processes")
         json_ = await get_content(url)
         json_['processes'] = [{"machine":self.machine, **kwargs} for kwargs in json_['processes']]
         return ProcessesResponse(**json_)
 
-    async def run_program(self, action_name: str, body: dict | BaseModel | str | None = None, **kwargs):
+    async def run_program(self, action_name: str, body: dict | BaseModel | str | None = None, **kwargs) -> ProcessStatus:
         process = await self.create_process()
         return await process.action(action_name, body, **kwargs)
 
     async def stream_program(self, action_name: str, body: Optional[Any] = None, **kwargs):
         process = await self.create_process()
         async for event in process.stream_action(action_name, body, **kwargs):
             yield event
@@ -78,14 +77,32 @@
 
 
 class Process(BaseModel):
     machine: str = Field(default_factory=current_machine_url)
     agent: str
     process_id: str
 
+    async def upload_file(self, file_contents: bytes) -> FileHandle:
+        url = urljoin(self.machine, f"processes/{self.process_id}/files")
+        json_ = await post_content(url, content=file_contents, headers={"Content-Type": "application/octet-stream"})
+        return FileHandle.model_validate(json_)
+
+    async def set_metadata(self, file_id: str, metadata: dict):
+        url = urljoin(self.machine, f"processes/{self.process_id}/files/{file_id}/metadata")
+        json_ = await post_content(url, json=metadata)
+        return FileHandle.model_validate(json_)
+
+    async def download_file(self, file_id: str) -> bytes:
+        url = urljoin(self.machine, f"processes/{self.process_id}/files/{file_id}")
+        return await get_raw(url)
+
+    async def delete_file(self, file_id: str) -> None:
+        url = urljoin(self.machine, f"processes/{self.process_id}/files/{file_id}")
+        await delete(url)
+
     async def action(self, action_name: str, body: dict | BaseModel | str | None = None, **kwargs) -> ProcessStatus:
         url = urljoin(self.machine, f"processes/{self.process_id}/agent/{self.agent}/actions/{action_name}")
         args = {
             "url": url, **kwargs
         }
         if body:
             args["json"] = body
```

### Comparing `eidolon_ai_client-0.1.5/eidolon_ai_client/events.py` & `eidolon_ai_client-0.1.6/eidolon_ai_client/events.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 
 from abc import ABC
 from enum import Enum
 from pydantic import BaseModel, TypeAdapter
 from typing import List, TypeVar, Generic, Any, AsyncIterator, Type, Literal, Dict, Optional
 
 
+class FileHandle(BaseModel):
+    machineURL: str
+    process_id: str
+    file_id: str
+    metadata: dict = {}
+
+
 class Category(Enum):
     START = "start"
     INPUT = "input"
     END = "end"
     OUTPUT = "output"
     TRANSFORM = "transform"
 
@@ -17,14 +24,15 @@
 T = TypeVar("T")
 
 
 class BaseStreamEvent(BaseModel, ABC):
     stream_context: Optional[str] = None
     category: Category
     event_type: str
+    metadata: dict = {}
 
     def is_root_event(self):
         return self.stream_context is None
 
     def is_root_and_type(self, event_type: type):
         return self.stream_context is None and isinstance(self, event_type)
 
@@ -42,15 +50,16 @@
 
         return _type_mapping[event_type](**event_dict)
 
 
 class UserInputEvent(BaseStreamEvent):
     category: Literal[Category.INPUT] = Category.INPUT
     event_type: Literal["user_input"] = "user_input"
-    input: Dict[str, Any]
+    input: str | Dict[str, Any]
+    files: List[FileHandle] = []
 
 
 class StartStreamContextEvent(BaseStreamEvent):
     category: Literal[Category.START] = Category.START
     event_type: Literal["context_start"] = "context_start"
     context_id: str
     title: str
```

### Comparing `eidolon_ai_client-0.1.5/eidolon_ai_client/group_conversation.py` & `eidolon_ai_client-0.1.6/eidolon_ai_client/group_conversation.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_client-0.1.5/eidolon_ai_client/util/aiohttp.py` & `eidolon_ai_client-0.1.6/eidolon_ai_client/util/aiohttp.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,16 +16,27 @@
     params = {"url": url, "headers": _headers()}
     async with AsyncClient(timeout=Timeout(5.0, read=600.0)) as client:
         response = await client.get(**params, **kwargs)
         await AgentError.check(response)
         return response.json()
 
 
-async def post_content(url, json: Optional[Any] = None, **kwargs):
+async def get_raw(url: str, **kwargs):
     params = {"url": url, "headers": _headers()}
+    async with AsyncClient(timeout=Timeout(5.0, read=600.0)) as client:
+        response = await client.get(**params, **kwargs)
+        await AgentError.check(response)
+        return response.content
+
+
+async def post_content(url, json: Optional[Any] = None, **kwargs):
+    headers = _headers()
+    if "headers" in kwargs:
+        headers.update(kwargs.pop("headers"))
+    params = {"url": url, "headers": headers}
     if json:
         params["json"] = to_jsonable_python(json)
     async with AsyncClient(timeout=Timeout(5.0, read=600.0)) as client:
         response = await client.post(**params, **kwargs)
         await AgentError.check(response)
         return response.json()
```

### Comparing `eidolon_ai_client-0.1.5/eidolon_ai_client/util/request_context.py` & `eidolon_ai_client-0.1.6/eidolon_ai_client/util/request_context.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_client-0.1.5/pyproject.toml` & `eidolon_ai_client-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eidolon_ai_client"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Luke Lalor <lukehlalor@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 setuptools = "^69.0.2"
```

### Comparing `eidolon_ai_client-0.1.5/PKG-INFO` & `eidolon_ai_client-0.1.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eidolon_ai_client
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Luke Lalor
 Author-email: lukehlalor@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiostream (>=0.5.2,<0.6.0)
```

