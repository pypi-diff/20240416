# Comparing `tmp/literalai-0.0.503.tar.gz` & `tmp/literalai-0.0.504.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "literalai-0.0.503.tar", last modified: Mon Apr 15 16:09:47 2024, max compression
+gzip compressed data, was "literalai-0.0.504.tar", last modified: Tue Apr 16 10:19:40 2024, max compression
```

## Comparing `literalai-0.0.503.tar` & `literalai-0.0.504.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:09:47.049658 literalai-0.0.503/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 16:09:39.000000 literalai-0.0.503/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-15 16:09:47.049658 literalai-0.0.503/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-15 16:09:39.000000 literalai-0.0.503/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:09:47.045658 literalai-0.0.503/literalai/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:09:47.049658 literalai-0.0.503/literalai/api/
--rw-r--r--   0 runner    (1001) docker     (127)    40320 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/api/attachment_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/api/dataset_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/api/generation_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20051 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/api/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/api/prompt_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/api/score_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/api/step_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/api/thread_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/api/user_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:09:47.049658 literalai-0.0.503/literalai/callback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/callback/langchain_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     6713 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/dataset_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/event_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:09:47.049658 literalai-0.0.503/literalai/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18352 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/instrumentation/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/my_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     9788 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-15 16:09:39.000000 literalai-0.0.503/literalai/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:09:47.045658 literalai-0.0.503/literalai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-15 16:09:46.000000 literalai-0.0.503/literalai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-15 16:09:47.000000 literalai-0.0.503/literalai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:09:46.000000 literalai-0.0.503/literalai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-15 16:09:46.000000 literalai-0.0.503/literalai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-15 16:09:46.000000 literalai-0.0.503/literalai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 16:09:47.049658 literalai-0.0.503/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-15 16:09:39.000000 literalai-0.0.503/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:09:47.049658 literalai-0.0.503/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:09:39.000000 literalai-0.0.503/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:19:40.664760 literalai-0.0.504/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 10:19:33.000000 literalai-0.0.504/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-16 10:19:40.664760 literalai-0.0.504/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-16 10:19:33.000000 literalai-0.0.504/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:19:40.660760 literalai-0.0.504/literalai/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:19:40.664760 literalai-0.0.504/literalai/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    40320 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/api/attachment_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/api/dataset_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/api/generation_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20094 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/api/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/api/prompt_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/api/score_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/api/step_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/api/thread_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/api/user_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:19:40.664760 literalai-0.0.504/literalai/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/callback/langchain_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6713 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/dataset_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/event_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:19:40.664760 literalai-0.0.504/literalai/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18352 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/instrumentation/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/my_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9788 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-16 10:19:33.000000 literalai-0.0.504/literalai/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:19:40.660760 literalai-0.0.504/literalai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-16 10:19:40.000000 literalai-0.0.504/literalai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-16 10:19:40.000000 literalai-0.0.504/literalai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 10:19:40.000000 literalai-0.0.504/literalai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-16 10:19:40.000000 literalai-0.0.504/literalai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-16 10:19:40.000000 literalai-0.0.504/literalai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 10:19:40.664760 literalai-0.0.504/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-16 10:19:33.000000 literalai-0.0.504/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:19:40.664760 literalai-0.0.504/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:19:33.000000 literalai-0.0.504/tests/__init__.py
```

### Comparing `literalai-0.0.503/LICENSE` & `literalai-0.0.504/LICENSE`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/README.md` & `literalai-0.0.504/README.md`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai/api/__init__.py` & `literalai-0.0.504/literalai/api/__init__.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai/api/attachment_helpers.py` & `literalai-0.0.504/literalai/api/attachment_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai/api/dataset_helpers.py` & `literalai-0.0.504/literalai/api/dataset_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai/api/generation_helpers.py` & `literalai-0.0.504/literalai/api/generation_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai/api/gql.py` & `literalai-0.0.504/literalai/api/gql.py`

 * *Files 0% similar despite different names*

```diff
@@ -606,24 +606,26 @@
     $input: Json,
     $output: Json,
     $metadata: Json,
     $name: String,
     $startTime: DateTime,
     $endTime: DateTime,
     $parentId: String,
+    $tags: [String!],
 ) {
     updateStep(
         id: $id,
         type: $type,
         startTime: $startTime,
         endTime: $endTime,
         input: $input,
         output: $output,
         metadata: $metadata,
         name: $name,
+        tags: $tags,
         parentId: $parentId,
     ) {    
 """
     + STEP_FIELDS
     + """
     }
 }
```

### Comparing `literalai-0.0.503/literalai/api/prompt_helpers.py` & `literalai-0.0.504/literalai/api/prompt_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai/api/score_helpers.py` & `literalai-0.0.504/literalai/api/score_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai/api/step_helpers.py` & `literalai-0.0.504/literalai/api/step_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai/api/thread_helpers.py` & `literalai-0.0.504/literalai/api/thread_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai/api/user_helpers.py` & `literalai-0.0.504/literalai/api/user_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai/callback/langchain_callback.py` & `literalai-0.0.504/literalai/callback/langchain_callback.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai/client.py` & `literalai-0.0.504/literalai/client.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai/dataset.py` & `literalai-0.0.504/literalai/dataset.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai/dataset_experiment.py` & `literalai-0.0.504/literalai/dataset_experiment.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai/dataset_item.py` & `literalai-0.0.504/literalai/dataset_item.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai/event_processor.py` & `literalai-0.0.504/literalai/event_processor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import asyncio
 import queue
+import logging
+import traceback
 import threading
 import time
 from typing import TYPE_CHECKING, List
 
+logger = logging.getLogger(__name__)
+
 if TYPE_CHECKING:
     from literalai.api import LiteralAPI
     from literalai.step import StepDict
 
+DEFAULT_SLEEP_TIME = 0.2
 
 # to_thread is a backport of asyncio.to_thread from Python 3.9
 async def to_thread(func, /, *args, **kwargs):
     import contextvars
     import functools
 
     loop = asyncio.get_running_loop()
@@ -51,42 +56,44 @@
                     # Attempt to get events with a timeout
                     event = self.event_queue.get(timeout=0.5)
                     batch.append(event)
             except queue.Empty:
                 # No more events at the moment, proceed with processing what's in the batch
                 pass
 
-            # Process the batch if any events are present
+            # Process the batch if any events are present - in a separate thread
             if batch:
                 self._process_batch(batch)
 
             # Stop if the stop_event is set and the queue is empty
             if self.stop_event.is_set() and self.event_queue.empty():
                 break
 
+    def _try_process_batch(self, batch):
+        try:
+            return self.api.send_steps(batch)
+        except Exception:
+            logger.error(f"Failed to send steps: {traceback.format_exc()}")
+        return None
+
     def _process_batch(self, batch):
-        res = self.api.send_steps(
-            steps=batch,
-        )
-        # simple one-try retry in case of network failure (no retry on graphql errors)
-        if not res:
-            time.sleep(0.5)
-            self.api.send_steps(
-                steps=batch,
-            )
-            return
+        # Simple one-try retry in case of network failure (no retry on graphql errors)
+        retries = 0
+        while not self._try_process_batch(batch) and retries < 1:
+            retries += 1
+            time.sleep(DEFAULT_SLEEP_TIME)
 
     def flush_and_stop(self):
         self.stop_event.set()
         if not self.disabled:
             self.processing_thread.join()
 
     async def aflush(self):
         while not self.event_queue.empty():
-            await asyncio.sleep(0.2)
+            await asyncio.sleep(DEFAULT_SLEEP_TIME)
 
     def flush(self):
         while not self.event_queue.empty():
             time.sleep(0.2)
 
     def __del__(self):
         self.flush_and_stop()
```

### Comparing `literalai-0.0.503/literalai/filter.py` & `literalai-0.0.504/literalai/filter.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai/helper.py` & `literalai-0.0.504/literalai/helper.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai/instrumentation/openai.py` & `literalai-0.0.504/literalai/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai/message.py` & `literalai-0.0.504/literalai/message.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai/my_types.py` & `literalai-0.0.504/literalai/my_types.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai/prompt.py` & `literalai-0.0.504/literalai/prompt.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai/requirements.py` & `literalai-0.0.504/literalai/requirements.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai/step.py` & `literalai-0.0.504/literalai/step.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai/thread.py` & `literalai-0.0.504/literalai/thread.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import inspect
+import logging
+import traceback
 import uuid
 from functools import wraps
 from typing import TYPE_CHECKING, Callable, Dict, List, Optional, TypedDict
 
 from literalai.context import active_thread_var
 from literalai.my_types import UserDict
 from literalai.step import Step, StepDict
 
 if TYPE_CHECKING:
     from literalai.client import BaseLiteralClient
 
+logger = logging.getLogger(__name__)
+
 
 class ThreadDict(TypedDict, total=False):
     id: Optional[str]
     name: Optional[str]
     metadata: Optional[Dict]
     tags: Optional[List[str]]
     createdAt: Optional[str]
@@ -120,15 +124,18 @@
         if metadata := thread_data.get("metadata"):
             thread_data_to_upsert["metadata"] = metadata
         if tags := thread_data.get("tags"):
             thread_data_to_upsert["tags"] = tags
         if participant_id := thread_data.get("participant_id"):
             thread_data_to_upsert["participant_id"] = participant_id
 
-        self.client.to_sync().api.upsert_thread(**thread_data_to_upsert)
+        try:
+            self.client.to_sync().api.upsert_thread(**thread_data_to_upsert)
+        except Exception:
+            logger.error(f"Failed to upsert thread: {traceback.format_exc()}")
 
     def __call__(self, func):
         return thread_decorator(
             self.client, func=func, name=self.name, ctx_manager=self
         )
 
     def __enter__(self) -> "Optional[Thread]":
```

### Comparing `literalai-0.0.503/literalai/wrappers.py` & `literalai-0.0.504/literalai/wrappers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.503/literalai.egg-info/SOURCES.txt` & `literalai-0.0.504/literalai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

