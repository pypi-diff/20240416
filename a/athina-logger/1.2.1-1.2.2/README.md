# Comparing `tmp/athina_logger-1.2.1.tar.gz` & `tmp/athina_logger-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athina_logger-1.2.1.tar", max compression
+gzip compressed data, was "athina_logger-1.2.2.tar", max compression
```

## Comparing `athina_logger-1.2.1.tar` & `athina_logger-1.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     6103 2024-03-20 17:09:51.913295 athina_logger-1.2.1/README.md
--rw-r--r--   0        0        0        0 2024-03-20 17:09:51.913405 athina_logger-1.2.1/athina_logger/__init__.py
--rw-r--r--   0        0        0      244 2024-03-20 17:09:51.913523 athina_logger-1.2.1/athina_logger/api_key.py
--rw-r--r--   0        0        0      626 2024-04-06 02:19:19.299377 athina_logger-1.2.1/athina_logger/athina_meta.py
--rw-r--r--   0        0        0      346 2024-04-11 21:50:15.997677 athina_logger-1.2.1/athina_logger/constants.py
--rw-r--r--   0        0        0      210 2024-03-20 17:09:51.913916 athina_logger-1.2.1/athina_logger/exception/custom_exception.py
--rw-r--r--   0        0        0        0 2024-03-20 17:09:51.914025 athina_logger-1.2.1/athina_logger/feedback/__init__.py
--rw-r--r--   0        0        0     1127 2024-03-20 17:09:51.914195 athina_logger-1.2.1/athina_logger/feedback/user_feedback.py
--rw-r--r--   0        0        0     4235 2024-04-06 02:19:19.299809 athina_logger-1.2.1/athina_logger/inference_logger.py
--rw-r--r--   0        0        0    14226 2024-04-02 05:37:10.002663 athina_logger-1.2.1/athina_logger/langchain_handler.py
--rw-r--r--   0        0        0        0 2024-03-20 17:09:51.914553 athina_logger-1.2.1/athina_logger/log_stream_inference/__init__.py
--rw-r--r--   0        0        0     4943 2024-04-06 02:19:19.299987 athina_logger-1.2.1/athina_logger/log_stream_inference/log_stream_inference.py
--rw-r--r--   0        0        0     7678 2024-04-06 02:19:19.300143 athina_logger-1.2.1/athina_logger/log_stream_inference/openai_chat_completion_stream.py
--rw-r--r--   0        0        0     7004 2024-04-06 02:19:19.300276 athina_logger-1.2.1/athina_logger/log_stream_inference/openai_completion_stream.py
--rw-r--r--   0        0        0    10771 2024-04-06 02:19:19.300668 athina_logger-1.2.1/athina_logger/openai_wrapper.py
--rw-r--r--   0        0        0     1883 2024-03-31 23:05:11.799630 athina_logger-1.2.1/athina_logger/request_helper.py
--rw-r--r--   0        0        0        0 2024-03-31 22:30:00.376453 athina_logger-1.2.1/athina_logger/tracing/__init__.py
--rw-r--r--   0        0        0        0 2024-03-31 22:30:00.406928 athina_logger-1.2.1/athina_logger/tracing/callback/__init__.py
--rw-r--r--   0        0        0    19798 2024-04-13 02:48:04.524470 athina_logger-1.2.1/athina_logger/tracing/callback/langchain.py
--rw-r--r--   0        0        0      755 2024-03-31 22:30:00.403809 athina_logger-1.2.1/athina_logger/tracing/models.py
--rw-r--r--   0        0        0    14103 2024-04-06 02:19:19.300937 athina_logger-1.2.1/athina_logger/tracing/span.py
--rw-r--r--   0        0        0     6864 2024-04-06 02:19:19.301218 athina_logger-1.2.1/athina_logger/tracing/trace.py
--rw-r--r--   0        0        0      260 2024-03-31 22:30:00.379971 athina_logger-1.2.1/athina_logger/tracing/util.py
--rw-r--r--   0        0        0        0 2024-03-20 17:09:51.915369 athina_logger-1.2.1/athina_logger/util/__init__.py
--rw-r--r--   0        0        0    10414 2024-03-31 22:30:00.357924 athina_logger-1.2.1/athina_logger/util/extract_model.py
--rw-r--r--   0        0        0     3259 2024-03-20 17:09:51.915502 athina_logger-1.2.1/athina_logger/util/token_count_helper.py
--rw-r--r--   0        0        0      465 2024-04-13 02:48:04.524967 athina_logger-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     6725 1970-01-01 00:00:00.000000 athina_logger-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     6103 2024-03-20 17:09:51.913295 athina_logger-1.2.2/README.md
+-rw-r--r--   0        0        0        0 2024-03-20 17:09:51.913405 athina_logger-1.2.2/athina_logger/__init__.py
+-rw-r--r--   0        0        0      244 2024-03-20 17:09:51.913523 athina_logger-1.2.2/athina_logger/api_key.py
+-rw-r--r--   0        0        0      626 2024-04-06 02:19:19.299377 athina_logger-1.2.2/athina_logger/athina_meta.py
+-rw-r--r--   0        0        0      346 2024-04-11 21:50:15.997677 athina_logger-1.2.2/athina_logger/constants.py
+-rw-r--r--   0        0        0      210 2024-03-20 17:09:51.913916 athina_logger-1.2.2/athina_logger/exception/custom_exception.py
+-rw-r--r--   0        0        0        0 2024-03-20 17:09:51.914025 athina_logger-1.2.2/athina_logger/feedback/__init__.py
+-rw-r--r--   0        0        0     1127 2024-03-20 17:09:51.914195 athina_logger-1.2.2/athina_logger/feedback/user_feedback.py
+-rw-r--r--   0        0        0     4235 2024-04-06 02:19:19.299809 athina_logger-1.2.2/athina_logger/inference_logger.py
+-rw-r--r--   0        0        0    14226 2024-04-02 05:37:10.002663 athina_logger-1.2.2/athina_logger/langchain_handler.py
+-rw-r--r--   0        0        0        0 2024-03-20 17:09:51.914553 athina_logger-1.2.2/athina_logger/log_stream_inference/__init__.py
+-rw-r--r--   0        0        0     4943 2024-04-06 02:19:19.299987 athina_logger-1.2.2/athina_logger/log_stream_inference/log_stream_inference.py
+-rw-r--r--   0        0        0     7678 2024-04-06 02:19:19.300143 athina_logger-1.2.2/athina_logger/log_stream_inference/openai_chat_completion_stream.py
+-rw-r--r--   0        0        0     7004 2024-04-06 02:19:19.300276 athina_logger-1.2.2/athina_logger/log_stream_inference/openai_completion_stream.py
+-rw-r--r--   0        0        0    10771 2024-04-06 02:19:19.300668 athina_logger-1.2.2/athina_logger/openai_wrapper.py
+-rw-r--r--   0        0        0     1883 2024-03-31 23:05:11.799630 athina_logger-1.2.2/athina_logger/request_helper.py
+-rw-r--r--   0        0        0        0 2024-03-31 22:30:00.376453 athina_logger-1.2.2/athina_logger/tracing/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-31 22:30:00.406928 athina_logger-1.2.2/athina_logger/tracing/callback/__init__.py
+-rw-r--r--   0        0        0    19798 2024-04-13 02:48:04.524470 athina_logger-1.2.2/athina_logger/tracing/callback/langchain.py
+-rw-r--r--   0        0        0      755 2024-03-31 22:30:00.403809 athina_logger-1.2.2/athina_logger/tracing/models.py
+-rw-r--r--   0        0        0    14109 2024-04-16 05:48:26.677022 athina_logger-1.2.2/athina_logger/tracing/span.py
+-rw-r--r--   0        0        0     6907 2024-04-16 05:48:26.678197 athina_logger-1.2.2/athina_logger/tracing/trace.py
+-rw-r--r--   0        0        0      596 2024-04-16 05:48:26.679245 athina_logger-1.2.2/athina_logger/tracing/util.py
+-rw-r--r--   0        0        0        0 2024-03-20 17:09:51.915369 athina_logger-1.2.2/athina_logger/util/__init__.py
+-rw-r--r--   0        0        0    10414 2024-03-31 22:30:00.357924 athina_logger-1.2.2/athina_logger/util/extract_model.py
+-rw-r--r--   0        0        0     3259 2024-03-20 17:09:51.915502 athina_logger-1.2.2/athina_logger/util/token_count_helper.py
+-rw-r--r--   0        0        0      465 2024-04-16 05:48:53.895748 athina_logger-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6725 1970-01-01 00:00:00.000000 athina_logger-1.2.2/PKG-INFO
```

### Comparing `athina_logger-1.2.1/README.md` & `athina_logger-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.1/athina_logger/athina_meta.py` & `athina_logger-1.2.2/athina_logger/athina_meta.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.1/athina_logger/feedback/user_feedback.py` & `athina_logger-1.2.2/athina_logger/feedback/user_feedback.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.1/athina_logger/inference_logger.py` & `athina_logger-1.2.2/athina_logger/inference_logger.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.1/athina_logger/langchain_handler.py` & `athina_logger-1.2.2/athina_logger/langchain_handler.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.1/athina_logger/log_stream_inference/log_stream_inference.py` & `athina_logger-1.2.2/athina_logger/log_stream_inference/log_stream_inference.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.1/athina_logger/log_stream_inference/openai_chat_completion_stream.py` & `athina_logger-1.2.2/athina_logger/log_stream_inference/openai_chat_completion_stream.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.1/athina_logger/log_stream_inference/openai_completion_stream.py` & `athina_logger-1.2.2/athina_logger/log_stream_inference/openai_completion_stream.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.1/athina_logger/openai_wrapper.py` & `athina_logger-1.2.2/athina_logger/openai_wrapper.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.1/athina_logger/request_helper.py` & `athina_logger-1.2.2/athina_logger/request_helper.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.1/athina_logger/tracing/callback/langchain.py` & `athina_logger-1.2.2/athina_logger/tracing/callback/langchain.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.1/athina_logger/tracing/models.py` & `athina_logger-1.2.2/athina_logger/tracing/models.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.1/athina_logger/tracing/span.py` & `athina_logger-1.2.2/athina_logger/tracing/span.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 from typing import Any, Dict, List, Optional, Union
 from .models import SpanModel
-from .util import remove_none_values
+from .util import get_utc_end_time, remove_none_values
 
 class Span:
 
     def __init__(
         self,
         name: str,
         start_time: Optional[datetime.datetime] = None,
@@ -171,15 +171,15 @@
             self._span.output = output
         if duration:
             self._span.duration = duration
         if attributes:
             self._span.attributes.update(attributes)
 
     def end(self, end_time: Optional[datetime.datetime] = None):
-        end_time = end_time or datetime.datetime.utcnow()
+        end_time = get_utc_end_time(end_time)
         if self._span.end_time is None:
             self._span.end_time = end_time.isoformat()
         if self._span.duration is None:
             self._span.duration = int((end_time - datetime.datetime.fromisoformat(self._span.start_time)).total_seconds())
         for child in self._children:
             child.end(end_time)
```

### Comparing `athina_logger-1.2.1/athina_logger/tracing/trace.py` & `athina_logger-1.2.2/athina_logger/tracing/trace.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import datetime
 import threading
 from typing import Any, Dict, List, Optional, Union
 
 from .span import Generation, Span
 from .models import TraceModel
-from .util import remove_none_values
+from .util import get_utc_end_time, remove_none_values
 from athina_logger.api_key import AthinaApiKey
 from athina_logger.constants import API_BASE_URL
 from athina_logger.request_helper import RequestHelper
 
 class Trace(AthinaApiKey):
     _trace: TraceModel
     _spans: list[Span]
@@ -169,19 +169,20 @@
             self._trace.duration = duration
 
     async def _log_trace_async(self, request_dict: Dict[str, Any]):
         RequestHelper.make_post_request(endpoint=f'{API_BASE_URL}/api/v1/trace/sdk', payload=request_dict, headers={
             "athina-api-key": Trace.get_api_key(), "Content-Type": "application/json"
         })
 
-    def end(self, end_time: Optional[datetime.datetime] = datetime.datetime.utcnow()):
-        try:
+    def end(self, end_time: Optional[datetime.datetime] = None):
+        try:      
+            end_time = get_utc_end_time(end_time)
             for span in self._spans:
                 span.end(end_time)
             if self._trace.end_time is None:
-                self._trace.end_time = end_time.utcnow().isoformat()
+                self._trace.end_time = end_time.isoformat()
             if self._trace.duration is None:
                 self._trace.duration = int((end_time - datetime.datetime.fromisoformat(self._trace.start_time)).total_seconds())
             request_dict = remove_none_values(self.to_dict())
             threading.Thread(target=lambda: asyncio.run(self._log_trace_async(request_dict))).start()
         except Exception as e:
             print("Error ending trace: ", e)
```

### Comparing `athina_logger-1.2.1/athina_logger/util/extract_model.py` & `athina_logger-1.2.2/athina_logger/util/extract_model.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.1/athina_logger/util/token_count_helper.py` & `athina_logger-1.2.2/athina_logger/util/token_count_helper.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.1/PKG-INFO` & `athina_logger-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athina-logger
-Version: 1.2.1
+Version: 1.2.2
 Summary: 
 Author: Akshat Gupta
 Author-email: akshat@athina.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

