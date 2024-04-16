# Comparing `tmp/lunary-1.0.1.tar.gz` & `tmp/lunary-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lunary-1.0.1.tar", max compression
+gzip compressed data, was "lunary-1.0.2.tar", max compression
```

## Comparing `lunary-1.0.1.tar` & `lunary-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,13 @@
--rw-r--r--   0        0        0      604 2024-02-28 21:10:30.380738 lunary-1.0.1/README.md
--rw-r--r--   0        0        0    57251 2024-04-02 01:49:13.753827 lunary-1.0.1/lunary/__init__.py
--rw-r--r--   0        0        0     2221 2024-04-01 02:07:49.605602 lunary-1.0.1/lunary/consumer.py
--rw-r--r--   0        0        0      607 2024-03-13 20:53:32.460623 lunary-1.0.1/lunary/event_queue.py
--rw-r--r--   0        0        0      834 2024-03-03 18:24:22.696583 lunary-1.0.1/lunary/langchain/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0      620 2024-03-03 18:23:24.270210 lunary-1.0.1/lunary/langchain/__pycache__/callback_handler.cpython-312.pyc
--rw-r--r--   0        0        0     2384 2024-03-04 00:09:26.744750 lunary-1.0.1/lunary/openai_utils.py
--rw-r--r--   0        0        0      670 2024-04-01 15:34:21.542269 lunary-1.0.1/lunary/parent.py
--rw-r--r--   0        0        0     1071 2024-04-02 01:49:22.083662 lunary-1.0.1/lunary/parsers.py
--rw-r--r--   0        0        0      425 2024-04-01 02:07:35.888287 lunary-1.0.1/lunary/project.py
--rw-r--r--   0        0        0      378 2024-03-04 00:09:26.744921 lunary-1.0.1/lunary/tags.py
--rw-r--r--   0        0        0      841 2024-03-04 00:09:26.744980 lunary-1.0.1/lunary/thread.py
--rw-r--r--   0        0        0      573 2024-03-04 00:09:26.745039 lunary-1.0.1/lunary/users.py
--rw-r--r--   0        0        0      747 2024-04-02 01:51:54.569858 lunary-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1685 1970-01-01 00:00:00.000000 lunary-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      604 2024-02-28 21:10:30.380738 lunary-1.0.2/README.md
+-rw-r--r--   0        0        0    57524 2024-04-16 01:14:07.135553 lunary-1.0.2/lunary/__init__.py
+-rw-r--r--   0        0        0     2221 2024-04-01 02:07:49.605602 lunary-1.0.2/lunary/consumer.py
+-rw-r--r--   0        0        0      607 2024-03-13 20:53:32.460623 lunary-1.0.2/lunary/event_queue.py
+-rw-r--r--   0        0        0     2384 2024-03-04 00:09:26.744750 lunary-1.0.2/lunary/openai_utils.py
+-rw-r--r--   0        0        0      670 2024-04-01 15:34:21.542269 lunary-1.0.2/lunary/parent.py
+-rw-r--r--   0        0        0     1071 2024-04-02 01:49:22.083662 lunary-1.0.2/lunary/parsers.py
+-rw-r--r--   0        0        0      425 2024-04-01 02:07:35.888287 lunary-1.0.2/lunary/project.py
+-rw-r--r--   0        0        0      378 2024-03-04 00:09:26.744921 lunary-1.0.2/lunary/tags.py
+-rw-r--r--   0        0        0      988 2024-04-16 01:14:00.143808 lunary-1.0.2/lunary/thread.py
+-rw-r--r--   0        0        0      573 2024-03-04 00:09:26.745039 lunary-1.0.2/lunary/users.py
+-rw-r--r--   0        0        0      743 2024-04-16 01:14:15.227402 lunary-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1683 1970-01-01 00:00:00.000000 lunary-1.0.2/PKG-INFO
```

### Comparing `lunary-1.0.1/README.md` & `lunary-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lunary-1.0.1/lunary/__init__.py` & `lunary-1.0.2/lunary/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,83 +168,86 @@
 
 
 def handle_internal_error(e):
     logging.info("[Lunary] Error: ", e)
 
 
 def stream_handler(fn, run_id, name, type, *args, **kwargs):
-    stream = fn(*args, **kwargs)
+    try:
+        stream = fn(*args, **kwargs)
 
-    choices = []
-    tokens = 0
+        choices = []
+        tokens = 0
 
-    for chunk in stream:
-        tokens += 1
-        choice = chunk.choices[0]
-        index = choice.index
-
-        content = choice.delta.content
-        role = choice.delta.role
-        function_call = choice.delta.function_call
-        tool_calls = choice.delta.tool_calls
-
-        if len(choices) <= index:
-            choices.append(
-                {
-                    "message": {
-                        "role": role,
-                        "content": content or "",
-                        "function_call": {},
-                        "tool_calls": [],
+        for chunk in stream:
+            tokens += 1
+            choice = chunk.choices[0]
+            index = choice.index
+
+            content = choice.delta.content
+            role = choice.delta.role
+            function_call = choice.delta.function_call
+            tool_calls = choice.delta.tool_calls
+
+            if len(choices) <= index:
+                choices.append(
+                    {
+                        "message": {
+                            "role": role,
+                            "content": content or "",
+                            "function_call": {},
+                            "tool_calls": [],
+                        }
                     }
-                }
-            )
-
-        if content:
-            choices[index]["message"]["content"] += content
-
-        if role:
-            choices[index]["message"]["role"] = role
-
-        if hasattr(function_call, "name"):
-            choices[index]["message"]["function_call"]["name"] = function_call.name
-
-        if hasattr(function_call, "arguments"):
-            choices[index]["message"]["function_call"].setdefault(
-                "arguments", "")
-            choices[index]["message"]["function_call"][
-                "arguments"
-            ] += function_call.arguments
-
-        if isinstance(tool_calls, list):
-            for tool_call in tool_calls:
-                existing_call_index = next(
-                    (
-                        index
-                        for (index, tc) in enumerate(
-                            choices[index]["message"]["tool_calls"]
-                        )
-                        if tc.index == tool_call.index
-                    ),
-                    -1,
                 )
 
-            if existing_call_index == -1:
-                choices[index]["message"]["tool_calls"].append(tool_call)
+            if content:
+                choices[index]["message"]["content"] += content
+
+            if role:
+                choices[index]["message"]["role"] = role
 
-            else:
-                existing_call = choices[index]["message"]["tool_calls"][
-                    existing_call_index
-                ]
-                if hasattr(tool_call, "function") and hasattr(
-                    tool_call.function, "arguments"
-                ):
-                    existing_call.function.arguments += tool_call.function.arguments
+            if hasattr(function_call, "name"):
+                choices[index]["message"]["function_call"]["name"] = function_call.name
 
-        yield chunk
+            if hasattr(function_call, "arguments"):
+                choices[index]["message"]["function_call"].setdefault(
+                    "arguments", "")
+                choices[index]["message"]["function_call"][
+                    "arguments"
+                ] += function_call.arguments
+
+            if isinstance(tool_calls, list):
+                for tool_call in tool_calls:
+                    existing_call_index = next(
+                        (
+                            index
+                            for (index, tc) in enumerate(
+                                choices[index]["message"]["tool_calls"]
+                            )
+                            if tc.index == tool_call.index
+                        ),
+                        -1,
+                    )
+
+                if existing_call_index == -1:
+                    choices[index]["message"]["tool_calls"].append(tool_call)
+
+                else:
+                    existing_call = choices[index]["message"]["tool_calls"][
+                        existing_call_index
+                    ]
+                    if hasattr(tool_call, "function") and hasattr(
+                        tool_call.function, "arguments"
+                    ):
+                        existing_call.function.arguments += tool_call.function.arguments
+
+            yield chunk
+    finally:
+        stream.close()
 
     output = OpenAIUtils.parse_message(choices[0]["message"])
     track_event(
         type,
         "end",
         run_id,
         name=name,
```

### Comparing `lunary-1.0.1/lunary/consumer.py` & `lunary-1.0.2/lunary/consumer.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.1/lunary/event_queue.py` & `lunary-1.0.2/lunary/event_queue.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.1/lunary/openai_utils.py` & `lunary-1.0.2/lunary/openai_utils.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.1/lunary/parent.py` & `lunary-1.0.2/lunary/parent.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.1/lunary/parsers.py` & `lunary-1.0.2/lunary/parsers.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.1/lunary/thread.py` & `lunary-1.0.2/lunary/thread.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,17 +12,20 @@
 
 class Thread:
     def __init__(self, track_event, id: Optional[str] = None, tags: Optional[List[str]] = None):
         self.id = id or str(uuid.uuid4())
         self.tags = tags
         self.track_event = track_event
 
-    def track_message(self, message: Message, feedback=None) -> str:
+    def track_message(self, message: Message, feedback=None, user_id=None, user_props=None) -> str:
         run_id = message.get("id", str(uuid.uuid4()))
 
         self.track_event("thread", "chat",
                          run_id=run_id,
                          parent_run_id=self.id,
                          thread_tags=self.tags,
                          feedback=feedback,
-                         message=message)
+                         message=message,
+                         user_id=user_id,
+                         user_props=user_props
+                         )
         return run_id
```

### Comparing `lunary-1.0.1/lunary/users.py` & `lunary-1.0.2/lunary/users.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.1/pyproject.toml` & `lunary-1.0.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "lunary"
-version = "1.0.1"
+version = "1.0.2"
 description = "Observability, analytics and evaluations for AI agents and chatbots."
 authors = ["lunary <hello@lunary.ai>"]
 readme = "README.md"
-repository = "https://github.com/lunary/lunary.ai/"
-documentation = "https://lunary.ai/docs/py/usage"
+repository = "https://github.com/lunary-ai/lunary-py"
+documentation = "https://lunary.ai/docs/py"
 keywords = ["Lunary", "lunary.ai", "Langchain", "AI", "Analytics", "Monitoring"]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 requests = "^2.31.0"
 setuptools = "^67.6.2"
 tenacity = "^8.2.3"
```

### Comparing `lunary-1.0.1/PKG-INFO` & `lunary-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: lunary
-Version: 1.0.1
+Version: 1.0.2
 Summary: Observability, analytics and evaluations for AI agents and chatbots.
-Home-page: https://github.com/lunary/lunary.ai/
+Home-page: https://github.com/lunary-ai/lunary-py
 Keywords: Lunary,lunary.ai,Langchain,AI,Analytics,Monitoring
 Author: lunary
 Author-email: hello@lunary.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -16,16 +16,16 @@
 Requires-Dist: opentelemetry-api (>=1.21.0,<2.0.0)
 Requires-Dist: opentelemetry-sdk (>=1.21.0,<2.0.0)
 Requires-Dist: packaging (>=23.2,<24.0)
 Requires-Dist: pyhumps (>=3.8.0,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: setuptools (>=67.6.2,<68.0.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
-Project-URL: Documentation, https://lunary.ai/docs/py/usage
-Project-URL: Repository, https://github.com/lunary/lunary.ai/
+Project-URL: Documentation, https://lunary.ai/docs/py
+Project-URL: Repository, https://github.com/lunary-ai/lunary-py
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 <img src="https://lunary.ai/logo.png" style='border-radius: 12px;' width="50"/> 
 <h1>Lunary Python SDK</h1>
```

