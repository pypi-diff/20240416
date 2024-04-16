# Comparing `tmp/deltafi-2.0rc1705080991758.tar.gz` & `tmp/deltafi-2.0rc1712763708188.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltafi-2.0rc1705080991758.tar", max compression
+gzip compressed data, was "deltafi-2.0rc1712763708188.tar", max compression
```

## Comparing `deltafi-2.0rc1705080991758.tar` & `deltafi-2.0rc1712763708188.tar`

### file list

```diff
@@ -1,22 +1,26 @@
--rw-r--r--   0        0        0      189 2023-04-10 13:32:51.621370 deltafi-2.0rc1705080991758/README.md
--rw-r--r--   0        0        0      709 2023-10-18 22:01:19.408525 deltafi-2.0rc1705080991758/deltafi/__init__.py
--rw-r--r--   0        0        0     5305 2024-01-12 17:29:57.481763 deltafi-2.0rc1705080991758/deltafi/action.py
--rw-r--r--   0        0        0     2847 2023-10-25 14:03:47.782289 deltafi-2.0rc1705080991758/deltafi/actioneventqueue.py
--rw-r--r--   0        0        0      865 2024-01-12 17:29:57.482763 deltafi-2.0rc1705080991758/deltafi/actiontype.py
--rw-r--r--   0        0        0    12161 2023-10-25 14:03:47.782289 deltafi-2.0rc1705080991758/deltafi/domain.py
--rw-r--r--   0        0        0     1149 2023-04-26 13:21:52.730906 deltafi-2.0rc1705080991758/deltafi/exception.py
--rw-r--r--   0        0        0     1090 2023-11-15 22:01:12.726378 deltafi-2.0rc1705080991758/deltafi/genericmodel.py
--rw-r--r--   0        0        0     1656 2024-01-12 17:29:57.483763 deltafi-2.0rc1705080991758/deltafi/input.py
--rw-r--r--   0        0        0     2136 2023-04-10 13:32:51.623371 deltafi-2.0rc1705080991758/deltafi/logger.py
--rw-r--r--   0        0        0      967 2023-04-10 13:32:51.623371 deltafi-2.0rc1705080991758/deltafi/metric.py
--rw-r--r--   0        0        0    12956 2024-01-12 17:29:57.484763 deltafi-2.0rc1705080991758/deltafi/plugin.py
--rw-r--r--   0        0        0     7330 2024-01-12 17:29:57.486763 deltafi-2.0rc1705080991758/deltafi/result.py
--rw-r--r--   0        0        0     2740 2023-05-19 17:18:33.056792 deltafi-2.0rc1705080991758/deltafi/storage.py
--rw-r--r--   0        0        0      709 2023-10-18 22:01:19.414525 deltafi-2.0rc1705080991758/deltafi/test_kit/__init__.py
--rw-r--r--   0        0        0     1378 2023-10-18 22:01:19.414525 deltafi-2.0rc1705080991758/deltafi/test_kit/assertions.py
--rw-r--r--   0        0        0     1581 2023-10-18 22:01:19.414525 deltafi-2.0rc1705080991758/deltafi/test_kit/compare_helpers.py
--rw-r--r--   0        0        0      833 2023-10-18 22:01:19.414525 deltafi-2.0rc1705080991758/deltafi/test_kit/constants.py
--rw-r--r--   0        0        0    13062 2024-01-12 17:21:36.473545 deltafi-2.0rc1705080991758/deltafi/test_kit/framework.py
--rw-r--r--   0        0        0     2608 2024-01-12 17:21:36.473545 deltafi-2.0rc1705080991758/deltafi/test_kit/transform.py
--rw-r--r--   0        0        0     1309 2024-01-12 17:36:38.975579 deltafi-2.0rc1705080991758/pyproject.toml
--rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 deltafi-2.0rc1705080991758/PKG-INFO
+-rw-r--r--   0        0        0      189 2023-08-18 18:44:06.655768 deltafi-2.0rc1712763708188/README.md
+-rw-r--r--   0        0        0      709 2023-09-12 19:43:28.655326 deltafi-2.0rc1712763708188/deltafi/__init__.py
+-rw-r--r--   0        0        0     5323 2024-04-10 15:22:52.625810 deltafi-2.0rc1712763708188/deltafi/action.py
+-rw-r--r--   0        0        0     2847 2023-10-25 16:46:16.158339 deltafi-2.0rc1712763708188/deltafi/actioneventqueue.py
+-rw-r--r--   0        0        0      865 2024-04-10 15:22:52.626810 deltafi-2.0rc1712763708188/deltafi/actiontype.py
+-rw-r--r--   0        0        0    11301 2024-04-10 15:22:52.627810 deltafi-2.0rc1712763708188/deltafi/domain.py
+-rw-r--r--   0        0        0      943 2024-04-10 15:22:52.628810 deltafi-2.0rc1712763708188/deltafi/exception.py
+-rw-r--r--   0        0        0     1090 2023-11-15 20:50:55.275227 deltafi-2.0rc1712763708188/deltafi/genericmodel.py
+-rw-r--r--   0        0        0     1656 2024-04-10 15:22:52.630810 deltafi-2.0rc1712763708188/deltafi/input.py
+-rw-r--r--   0        0        0     2136 2023-08-18 18:44:06.656768 deltafi-2.0rc1712763708188/deltafi/logger.py
+-rw-r--r--   0        0        0      967 2023-08-18 18:44:06.656768 deltafi-2.0rc1712763708188/deltafi/metric.py
+-rw-r--r--   0        0        0    12294 2024-04-10 15:22:52.631810 deltafi-2.0rc1712763708188/deltafi/plugin.py
+-rw-r--r--   0        0        0     8177 2024-04-10 15:22:52.633810 deltafi-2.0rc1712763708188/deltafi/result.py
+-rw-r--r--   0        0        0     2740 2023-09-05 12:02:08.690603 deltafi-2.0rc1712763708188/deltafi/storage.py
+-rw-r--r--   0        0        0      709 2023-09-12 19:43:28.657326 deltafi-2.0rc1712763708188/deltafi/test_kit/__init__.py
+-rw-r--r--   0        0        0     1378 2023-09-12 19:43:28.662326 deltafi-2.0rc1712763708188/deltafi/test_kit/assertions.py
+-rw-r--r--   0        0        0     1581 2023-09-12 19:43:28.662326 deltafi-2.0rc1712763708188/deltafi/test_kit/compare_helpers.py
+-rw-r--r--   0        0        0      833 2023-08-18 18:44:06.657768 deltafi-2.0rc1712763708188/deltafi/test_kit/constants.py
+-rw-r--r--   0        0        0     2090 2024-01-29 15:59:31.393845 deltafi-2.0rc1712763708188/deltafi/test_kit/domain.py
+-rw-r--r--   0        0        0     1899 2024-01-29 15:59:31.394845 deltafi-2.0rc1712763708188/deltafi/test_kit/egress.py
+-rw-r--r--   0        0        0     2587 2024-01-29 15:59:31.394845 deltafi-2.0rc1712763708188/deltafi/test_kit/enrich.py
+-rw-r--r--   0        0        0    14602 2024-04-10 15:22:52.633810 deltafi-2.0rc1712763708188/deltafi/test_kit/framework.py
+-rw-r--r--   0        0        0     4085 2024-04-10 15:22:52.634811 deltafi-2.0rc1712763708188/deltafi/test_kit/transform.py
+-rw-r--r--   0        0        0     1933 2024-01-29 15:59:31.395845 deltafi-2.0rc1712763708188/deltafi/test_kit/validate.py
+-rw-r--r--   0        0        0     1310 2024-04-10 15:42:11.789872 deltafi-2.0rc1712763708188/pyproject.toml
+-rw-r--r--   0        0        0     1446 1970-01-01 00:00:00.000000 deltafi-2.0rc1712763708188/PKG-INFO
```

### Comparing `deltafi-2.0rc1705080991758/deltafi/__init__.py` & `deltafi-2.0rc1712763708188/deltafi/__init__.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705080991758/deltafi/action.py` & `deltafi-2.0rc1712763708188/deltafi/action.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 
     def execute(self, context: Context, input_placeholder: Any, params: BaseModel):
         return self.ingress(context, params)
 
 
 class TransformAction(Action, ABC):
     def __init__(self, description: str):
-        super().__init__(ActionType.TRANSFORM, description, (TransformResult, ErrorResult, FilterResult))
+        super().__init__(ActionType.TRANSFORM, description, (TransformResult, TransformResults, ErrorResult, FilterResult))
 
     def build_input(self, context: Context, delta_file_message: DeltaFileMessage):
         return TransformInput(content=delta_file_message.content_list, metadata=delta_file_message.metadata)
 
     def collect(self, transform_inputs: List[TransformInput]):
         all_content = []
         all_metadata = {}
```

### Comparing `deltafi-2.0rc1705080991758/deltafi/actioneventqueue.py` & `deltafi-2.0rc1712763708188/deltafi/actioneventqueue.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705080991758/deltafi/actiontype.py` & `deltafi-2.0rc1712763708188/deltafi/actiontype.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705080991758/deltafi/domain.py` & `deltafi-2.0rc1712763708188/deltafi/domain.py`

 * *Files 4% similar despite different names*

```diff
@@ -292,49 +292,25 @@
         media_type = content['mediaType']
         return Content(name=name,
                        segments=segments,
                        media_type=media_type,
                        content_service=content_service)
 
 
-class Domain(NamedTuple):
-    name: str
-    value: str
-    media_type: str
-
-    @classmethod
-    def from_dict(cls, domain: dict):
-        name = domain['name']
-        if 'value' in domain:
-            value = domain['value']
-        else:
-            value = None
-        media_type = domain['mediaType']
-        return Domain(name=name,
-                      value=value,
-                      media_type=media_type)
-
-
 class DeltaFileMessage(NamedTuple):
     metadata: Dict[str, str]
     content_list: List[Content]
-    domains: List[Domain]
-    enrichments: List[Domain]
 
     @classmethod
     def from_dict(cls, delta_file_message: dict, content_service: ContentService):
         metadata = delta_file_message['metadata']
         content_list = [Content.from_dict(content, content_service) for content in delta_file_message['contentList']]
-        domains = [Domain.from_dict(domain) for domain in delta_file_message['domains']] if 'domains' in delta_file_message else []
-        enrichments = [Domain.from_dict(domain) for domain in delta_file_message['enrichments']] if 'enrichments' in delta_file_message else []
 
         return DeltaFileMessage(metadata=metadata,
-                                content_list=content_list,
-                                domains=domains,
-                                enrichments=enrichments)
+                                content_list=content_list)
 
 
 class Event(NamedTuple):
     delta_file_messages: List[DeltaFileMessage]
     context: Context
     params: dict
     queue_name: str
```

### Comparing `deltafi-2.0rc1705080991758/deltafi/exception.py` & `deltafi-2.0rc1712763708188/deltafi/exception.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,20 +19,10 @@
 
 class ExpectedContentException(RuntimeError):
     def __init__(self, index, size):
         self.index = index
         self.size = size
 
 
-class MissingDomainException(RuntimeError):
-    def __init__(self, name):
-        self.name = name
-
-
-class MissingEnrichmentException(RuntimeError):
-    def __init__(self, name):
-        self.name = name
-
-
 class MissingMetadataException(RuntimeError):
     def __init__(self, key):
         self.key = key
```

### Comparing `deltafi-2.0rc1705080991758/deltafi/genericmodel.py` & `deltafi-2.0rc1712763708188/deltafi/genericmodel.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705080991758/deltafi/input.py` & `deltafi-2.0rc1712763708188/deltafi/input.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705080991758/deltafi/logger.py` & `deltafi-2.0rc1712763708188/deltafi/logger.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705080991758/deltafi/metric.py` & `deltafi-2.0rc1712763708188/deltafi/metric.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705080991758/deltafi/plugin.py` & `deltafi-2.0rc1712763708188/deltafi/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,15 @@
 import inspect
 import pkgutil
 
 from importlib import metadata
 import requests
 from deltafi.actioneventqueue import ActionEventQueue
 from deltafi.domain import Event, ActionExecution
-from deltafi.exception import ExpectedContentException, MissingDomainException, MissingEnrichmentException, \
-    MissingMetadataException
+from deltafi.exception import ExpectedContentException, MissingMetadataException
 from deltafi.logger import get_logger
 from deltafi.result import ErrorResult
 from deltafi.storage import ContentService
 from deltafi.action import Action
 
 
 def _coordinates():
@@ -271,22 +270,14 @@
                 try:
                     result = action.execute_action(event)
                 except ExpectedContentException as e:
                     result = ErrorResult(event.context,
                                          f"Action attempted to look up element {e.index + 1} (index {e.index}) from "
                                          f"content list of size {e.size}",
                                          f"{str(e)}\n{traceback.format_exc()}")
-                except MissingDomainException as e:
-                    result = ErrorResult(event.context,
-                                         f"Action attempted to access domain {e.name}, which does not exist",
-                                         f"{str(e)}\n{traceback.format_exc()}")
-                except MissingEnrichmentException as e:
-                    result = ErrorResult(event.context,
-                                         f"Action attempted to access enrichment {e.name}, which does not exist",
-                                         f"{str(e)}\n{traceback.format_exc()}")
                 except MissingMetadataException as e:
                     result = ErrorResult(event.context,
                                          f"Missing metadata with key {e.key}",
                                          f"{str(e)}\n{traceback.format_exc()}")
                 except BaseException as e:
                     result = ErrorResult(event.context,
                                          f"Action execution {type(e)} exception", f"{str(e)}\n{traceback.format_exc()}")
```

### Comparing `deltafi-2.0rc1705080991758/deltafi/result.py` & `deltafi-2.0rc1712763708188/deltafi/result.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 #
 
 import abc
-from enum import Enum
 import uuid
-from typing import Dict, List
+from enum import Enum
+from typing import NamedTuple
 
 from deltafi.domain import Content, Context
 from deltafi.metric import Metric
 
 ENDPOINT_TAG = "endpoint"
 FILES_OUT = "files_out"
 BYTES_OUT = "bytes_out"
@@ -40,14 +40,15 @@
 
     @abc.abstractmethod
     def response(self):
         pass
 
     def add_metric(self, metric: Metric):
         self.metrics.append(metric)
+        return self
 
 
 class EgressResult(Result):
     def __init__(self, context: Context, destination: str, bytes_egressed: int):
         super().__init__(None, 'EGRESS', context)
         self.add_metric(Metric(FILES_OUT, 1, {ENDPOINT_TAG: destination}))
         self.add_metric(Metric(BYTES_OUT, bytes_egressed, {ENDPOINT_TAG: destination}))
@@ -72,15 +73,15 @@
             'cause': self.error_cause,
             'context': self.error_context,
             'annotations': self.annotations
         }
 
 
 class FilterResult(Result):
-    def __init__(self, context: Context, filtered_cause: str, filtered_context: str=None):
+    def __init__(self, context: Context, filtered_cause: str, filtered_context: str = None):
         super().__init__('filter', 'FILTER', context)
         self.filtered_cause = filtered_cause
         self.filtered_context = filtered_context
         self.annotations = {}
 
     def annotate(self, key: str, value: str):
         self.annotations[key] = value
@@ -174,16 +175,16 @@
         }
 
 
 class TransformResult(Result):
     def __init__(self, context: Context):
         super().__init__('transform', 'TRANSFORM', context)
         self.content = []
-        self.metadata = {}
         self.annotations = {}
+        self.metadata = {}
         self.delete_metadata_keys = []
 
     # content can be a single Content or a List[Content]
     def add_content(self, content):
         if content:
             if type(content) == list:
                 self.content.extend(content)
@@ -216,14 +217,45 @@
         self.annotations[key] = value
         return self
 
     def delete_metadata_key(self, key: str):
         self.delete_metadata_keys.append(key)
         return self
 
-    def response(self):
+    def json(self):
         return {
             'content': [content.json() for content in self.content],
-            'metadata': self.metadata,
             'annotations': self.annotations,
+            'metadata': self.metadata,
             'deleteMetadataKeys': self.delete_metadata_keys
         }
+
+    def response(self):
+        return [self.json()]
+
+
+class NamedTransformResult(NamedTuple):
+    result: TransformResult
+    name: str
+
+    def json(self):
+        j = self.result.json()
+        if self.name is not None:
+            j['name'] = self.name
+        return j
+
+
+class TransformResults(Result):
+    def __init__(self, context: Context):
+        super().__init__('transform', 'TRANSFORM', context)
+        self.named_results = []
+
+    def add_result(self, result: TransformResult, name: str = None):
+        self.named_results.append(NamedTransformResult(result, name))
+        return self
+
+    def response(self):
+        transform_events = []
+        for named_result in self.named_results:
+            json_dict = named_result.json()
+            transform_events.append(json_dict)
+        return transform_events
```

### Comparing `deltafi-2.0rc1705080991758/deltafi/storage.py` & `deltafi-2.0rc1712763708188/deltafi/storage.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705080991758/deltafi/test_kit/__init__.py` & `deltafi-2.0rc1712763708188/deltafi/test_kit/__init__.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705080991758/deltafi/test_kit/assertions.py` & `deltafi-2.0rc1712763708188/deltafi/test_kit/assertions.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705080991758/deltafi/test_kit/compare_helpers.py` & `deltafi-2.0rc1712763708188/deltafi/test_kit/compare_helpers.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705080991758/deltafi/test_kit/constants.py` & `deltafi-2.0rc1712763708188/deltafi/test_kit/constants.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705080991758/deltafi/test_kit/framework.py` & `deltafi-2.0rc1712763708188/deltafi/test_kit/framework.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import uuid
 from abc import ABC
 from importlib.resources import files
 from typing import List
 
 from deltafi.domain import DeltaFileMessage, Event, Content, Context
 from deltafi.logger import get_logger
+from deltafi.metric import Metric
 from deltafi.result import ErrorResult, FilterResult
 from deltafi.storage import Segment
 
 from .assertions import *
 from .compare_helpers import GenericCompareHelper, CompareHelper
 from .constants import *
 
@@ -39,16 +40,15 @@
         file_name (str): The name of file in test/data.
         content_name (str): The name of the content.
         content_type (str): The media type of the content
         offset (int): Offset to use in Segment
         content_bytes (str): Bypass file read, and uses these bytes for content
     """
 
-    def __init__(self, file_name: str, content_name: str = None,
-                 content_type: str = None, offset: int = 0,
+    def __init__(self, file_name: str, content_name: str = None, content_type: str = None, offset: int = 0,
                  content_bytes: str = ""):
         self.file_name = file_name
         if content_name is None:
             self.content_name = file_name
         else:
             self.content_name = content_name
         if content_type is None:
@@ -75,36 +75,29 @@
         self.name = ioc.content_name
         self.content_type = ioc.content_type
         self.offset = ioc.offset
         if data is not None:
             self.data = data
         else:
             self.data = ioc.content_bytes
-        self.segment = Segment.from_dict({
-            "uuid": str(uuid.uuid4()),
-            "offset": self.offset,
-            "size": len(self.data),
-            "did": did
-        })
+        self.segment = Segment.from_dict(
+            {"uuid": str(uuid.uuid4()), "offset": self.offset, "size": len(self.data), "did": did})
 
 
 class InternalContentService:
     def __init__(self):
         self.loaded_content = {}
         self.outputs = {}
 
     def load(self, content_list: List[LoadedContent]):
         for c in content_list:
             self.loaded_content[c.segment.uuid] = c
 
     def put_str(self, did: str, string_data: str):
-        segment = Segment(uuid=str(uuid.uuid4()),
-                          offset=0,
-                          size=len(string_data),
-                          did=did)
+        segment = Segment(uuid=str(uuid.uuid4()), offset=0, size=len(string_data), did=did)
         self.outputs[segment.uuid] = string_data
         return segment
 
     def get_str(self, segments: List[Segment]):
         # TODO: String multiple segment ids together
         seg_id = segments[0].uuid
         return self.loaded_content[seg_id].data
@@ -120,16 +113,15 @@
         :param data: Dict of test case fields
         - action: instance of the action being tested
         - data_dir: str: subdirectory name (e.g., test name) for locating test data files, i.e., test/data/{data_dir)
         - compare_tool: (optional) CompareHelper instanced for comparing output content
         - inputs: (optional) List[IOContent]: input content to action
         - parameters: (optional) Dict: map of action input parameters
         - in_meta: (optional) Dict: map of metadata as input to action
-        - in_domains: (optional) List[Domain]: list of domains as input to action
-        - in_enrichments: (optional) List[Domain]: list of enrichments as input to action
+        - did: (optional): str: overrides random DID
         """
         if "action" in data:
             self.action = data["action"]
         else:
             raise ValueError("action is required")
 
         if "data_dir" in data:
@@ -140,62 +132,81 @@
         if "compare_tool" in data:
             self.compare_tool = data["compare_tool"]
         else:
             self.compare_tool = GenericCompareHelper()
 
         self.inputs = data["inputs"] if "inputs" in data else []
         self.file_name = data["file_name"] if "file_name" in data else "filename"
-        self.outputs = data["outputs"] if "outputs" in data else []
         self.parameters = data["parameters"] if "parameters" in data else {}
         self.in_meta = data["in_meta"] if "in_meta" in data else {}
-        self.in_domains = data["in_domains"] if "in_domains" in data else []
-        self.in_enrichments = data["in_enrichments"] if "in_enrichments" in data else []
+        self.use_did = data["did"] if "did" in data else None
         self.expected_result_type = None
-        self.cause_regex = None
-        self.context_regex = None
+        self.err_or_filt_cause = None
+        self.err_or_filt_context = None
+        self.err_or_filt_annotations = None
+        self.expected_metrics = []
 
-    def expect_error_result(self, cause: str, context: str):
+    def add_metric(self, metric: Metric):
+        self.expected_metrics.append(metric)
+
+    def expect_error_result(self, cause: str, context: str, annotations: Dict = None):
         """
         A Sets the expected output of the action to an Error Result
         :param cause: the expected error cause
         :param context: the expected error context
+        :param annotations (Optional): Dict: the expected annotations
         """
         self.expected_result_type = ErrorResult
-        self.cause_regex = cause
-        self.context_regex = context
+        self.err_or_filt_cause = cause
+        self.err_or_filt_context = context
+        self.err_or_filt_annotations = annotations
 
-    def expect_filter_result(self, cause: str, context: str=None):
+    def expect_filter_result(self, cause: str, context: str = None, annotations: Dict = None):
         """
         A Sets the expected output of the action to a Filter Result
         :param cause: the expected filter cause (message)
-        :param context: the expected error context (optional)
+        :param context (Optional): the expected filter context
+        :param annotations (Optional): Dict: the expected annotations
         """
         self.expected_result_type = FilterResult
-        self.cause_regex = cause
-        self.context_regex = context
+        self.err_or_filt_cause = cause
+        self.err_or_filt_context = context
+        self.err_or_filt_annotations = annotations
 
 
 class ActionTest(ABC):
     def __init__(self, package_name: str):
         """
         Provides structure for testing DeltaFi actions
         Args:
             package_name: name of the actions package for finding resources
         """
         self.content_service = InternalContentService()
         self.did = ""
-        self.expected_outputs = []
         self.loaded_inputs = []
         self.package_name = package_name
         self.res_path = ""
 
-    def __reset__(self):
+    def __reset__(self, did: str):
         self.content_service = InternalContentService()
+<<<<<<< HEAD
+        if did is None:
+            self.did = str(uuid.uuid4())
+        else:
+            self.did = did
+        self.expected_outputs = []
+||||||| parent of 831733c7 (2.0 Refactor)
         self.did = str(uuid.uuid4())
         self.expected_outputs = []
+=======
+        if did is None:
+            self.did = str(uuid.uuid4())
+        else:
+            self.did = did
+>>>>>>> 831733c7 (2.0 Refactor)
         self.loaded_inputs = []
         self.res_path = ""
 
     def load_file(self, ioc: IOContent):
         file_res = self.res_path.joinpath(ioc.file_name)
         with file_res.open("r") as f:
             contents = f.read()
@@ -208,124 +219,138 @@
         # Load inputs
         for input_ioc in test_case.inputs:
             if len(input_ioc.content_bytes) == 0:
                 self.loaded_inputs.append(LoadedContent(self.did, input_ioc, self.load_file(input_ioc)))
             else:
                 self.loaded_inputs.append(LoadedContent(self.did, input_ioc, None))
 
-        # Load expected outputs
-        for output_ioc in test_case.outputs:
-            if len(output_ioc.content_bytes) == 0:
-                self.expected_outputs.append(LoadedContent(self.did, output_ioc, self.load_file(output_ioc)))
-            else:
-                self.expected_outputs.append(LoadedContent(self.did, output_ioc, None))
-
     def make_content_list(self, test_case: TestCaseBase):
         content_list = []
         for loaded_input in self.loaded_inputs:
-            c = Content(name=loaded_input.name,
-                        segments=[loaded_input.segment],
-                        media_type=loaded_input.content_type,
+            c = Content(name=loaded_input.name, segments=[loaded_input.segment], media_type=loaded_input.content_type,
                         content_service=self.content_service)
             content_list.append(c)
             loaded_input.content = c
 
         return content_list
 
     def make_df_msg(self, test_case: TestCaseBase):
         content_list = self.make_content_list(test_case)
         self.content_service.load(self.loaded_inputs)
 
+<<<<<<< HEAD
+        return DeltaFileMessage(
+            metadata=test_case.in_meta,
+            content_list=content_list,
+            domains=test_case.in_domains,
+            enrichments=test_case.in_enrichments)
+||||||| parent of 831733c7 (2.0 Refactor)
         return DeltaFileMessage(metadata=test_case.in_meta,
                                 content_list=content_list,
                                 domains=test_case.in_domains,
                                 enrichments=test_case.in_enrichments)
+=======
+        return DeltaFileMessage(metadata=test_case.in_meta,
+                                content_list=content_list)
+>>>>>>> 831733c7 (2.0 Refactor)
 
     def make_context(self, test_case: TestCaseBase):
         action_name = INGRESS_FLOW + "." + test_case.action.__class__.__name__
-        return Context(did=self.did,
-                       action_flow=INGRESS_FLOW,
-                       action_name=action_name,
-                       source_filename=test_case.file_name,
-                       ingress_flow=INGRESS_FLOW,
-                       egress_flow=EGRESS_FLOW,
-                       system=SYSTEM,
-                       hostname=HOSTNAME,
-                       content_service=self.content_service,
-                       collect=None,
-                       collected_dids=None,
-                       logger=get_logger())
+        return Context(
+            did=self.did,
+            action_flow=INGRESS_FLOW,
+            action_name=action_name,
+            source_filename=test_case.file_name,
+            ingress_flow=INGRESS_FLOW,
+            egress_flow=EGRESS_FLOW,
+            system=SYSTEM,
+            hostname=HOSTNAME,
+            content_service=self.content_service,
+            collect=None,
+            collected_dids=None,
+            logger=get_logger())
 
     def make_event(self, test_case: TestCaseBase):
-        return Event(
-            delta_file_messages=[self.make_df_msg(test_case)],
-            context=self.make_context(test_case),
-            params=test_case.parameters,
-            queue_name="",
-            return_address="")
+        return Event(delta_file_messages=[self.make_df_msg(test_case)], context=self.make_context(test_case),
+                     params=test_case.parameters, queue_name="", return_address="")
 
     def call_action(self, test_case: TestCaseBase):
         self.get_contents(test_case)
         return test_case.action.execute_action(self.make_event(test_case))
 
     def run_and_check_result_type(self, test_case: TestCaseBase, result_type):
-        self.__reset__()
+        self.__reset__(test_case.use_did)
         result = self.call_action(test_case)
 
         if not isinstance(result, result_type):
             raise ValueError(f"Result type {result.__class__.__name__} does not match {result_type.__name__}")
 
         return result
 
     def execute_error(self, test_case: TestCaseBase):
         result = self.run_and_check_result_type(test_case, ErrorResult)
         resp = result.response()
-        assert resp['cause'] == test_case.cause_regex
-        assert resp['context'] == test_case.context_regex
+        assert_equal_with_label(test_case.err_or_filt_cause, resp['cause'], "error cause")
+        if test_case.err_or_filt_context is not None:
+            assert_equal_with_label(test_case.err_or_filt_context, resp['context'], "error context")
+        if test_case.err_or_filt_annotations is not None:
+            assert_keys_and_values(test_case.err_or_filt_annotations, result.annotations)
 
-    def execute_filter(self, test_case):
+    def execute_filter(self, test_case: TestCaseBase):
         result = self.run_and_check_result_type(test_case, FilterResult)
         resp = result.response()
-        assert resp['message'] == test_case.cause_regex
+        assert_equal_with_label(test_case.err_or_filt_cause, resp['message'], "filter cause")
+        if test_case.err_or_filt_context is not None:
+            assert_equal_with_label(test_case.err_or_filt_context, resp['context'], "filter context")
+        if test_case.err_or_filt_annotations is not None:
+            assert_keys_and_values(test_case.err_or_filt_annotations, result.annotations)
 
     def execute(self, test_case: TestCaseBase):
-        if isinstance(test_case.expected_result_type, ErrorResult.__class__):
+        if test_case.expected_result_type == ErrorResult:
             self.execute_error(test_case)
-        elif isinstance(test_case.expected_result_type, FilterResult.__class__):
+        elif test_case.expected_result_type == FilterResult:
             self.execute_filter(test_case)
         else:
             raise ValueError(f"unknown type: {test_case.expected_result_type}")
 
     def compare_content_details(self, expected: LoadedContent, actual: Content):
         assert_equal(expected.content_type, actual.media_type)
         assert_equal(expected.name, actual.name)
 
     def compare_one_content(self, comparitor: CompareHelper, expected: LoadedContent, actual, index):
         self.compare_content_details(expected, actual)
         seg_id = actual.segments[0].uuid
-        comparitor.compare(
-            expected.data,
-            self.content_service.get_output(seg_id),
-            f"Content[{index}]"
-        )
-
-    def compare_all_output(self, comparitor: CompareHelper, content: List):
-        assert_equal_len(self.expected_outputs, content)
-        for index, expected in enumerate(self.expected_outputs):
+        comparitor.compare(expected.data, self.content_service.get_output(seg_id), f"Content[{index}]")
+
+    def compare_content_list(self, comparitor: CompareHelper, expected_outputs: List[IOContent], content: List):
+        assert_equal_len(expected_outputs, content)
+        for index, expected_ioc in enumerate(expected_outputs):
+            if len(expected_ioc.content_bytes) == 0:
+                expected = LoadedContent(self.did, expected_ioc, self.load_file(output_ioc))
+            else:
+                expected = LoadedContent(self.did, expected_ioc, None)
             self.compare_one_content(comparitor, expected, content[index], index)
 
-    def compare_domains(self, comparitor: CompareHelper, expected_items: List[Dict], results: List[Dict]):
-        assert_equal_len(expected_items, results)
-        for index, expected in enumerate(expected_items):
-            actual = results[index]
-            assert_equal(expected['name'], actual['name'])
-            assert_equal(expected['mediaType'], actual['mediaType'])
+    def compare_one_metric(self, expected: Metric, result: Metric):
+        assert expected.name == result.name
+        assert_equal_with_label(expected.value, result.value, expected.name)
+        assert_keys_and_values(expected.tags, result.tags)
 
             expected_value = expected['value']
             if type(expected_value) == str:
                 comparitor.compare(expected_value, actual['value'], f"Domain[{index}]")
             elif type(expected_value) == IOContent:
                 expected_data = self.load_file(expected_value)
                 comparitor.compare(expected_data, actual['value'], f"Domain[{index}]")
             else:
-                raise ValueError(
-                    f"unknown expected_value type: {type(expected_value)}")
+                raise ValueError(f"unknown expected_value type: {type(expected_value)}")
+
+    def compare_one_metric(self, expected: Metric, result: Metric):
+        assert expected.name == result.name
+        assert_equal_with_label(expected.value, result.value, expected.name)
+        assert_keys_and_values(expected.tags, result.tags)
+
+    def compare_metrics(self, expected_metrics: List[Metric], results: List[Metric]):
+        if len(expected_metrics) > 0:
+            assert_equal_len(expected_metrics, results)
+            for index, expected in enumerate(expected_metrics):
+                self.compare_one_metric(expected, results[index])
```

### Comparing `deltafi-2.0rc1705080991758/deltafi/test_kit/transform.py` & `deltafi-2.0rc1712763708188/deltafi/test_kit/validate.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,61 +12,43 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 #
 
-from typing import List
-
-from deltafi.result import TransformResult
+from deltafi.result import ValidateResult
 
 from .assertions import *
 from .framework import TestCaseBase, ActionTest
 
 
-class TransformTestCase(TestCaseBase):
+class ValidateTestCase(TestCaseBase):
     def __init__(self, fields: Dict):
         super().__init__(fields)
-        self.metadata = {}
-        self.delete_metadata_keys = []
-        self.annotations = {}
-
-    def expect_transform_result(self, metadata: Dict, delete_metadata_keys: List[str], annotations: Dict):
-        self.expected_result_type = TransformResult
-        self.metadata = metadata
-        self.delete_metadata_keys = delete_metadata_keys
-        self.annotations = annotations
+
+    def expect_validate_result(self):
+        self.expected_result_type = ValidateResult
 
 
-class TransformActionTest(ActionTest):
+class ValidateActionTest(ActionTest):
     def __init__(self, package_name: str):
         """
-        Provides structure for testing DeltaFi Transform action
+        Provides structure for testing DeltaFi Validate action
         Args:
             package_name: name of the actions package for finding resources
         """
         super().__init__(package_name)
 
-    def transform(self, test_case: TransformTestCase):
-        if test_case.expected_result_type == TransformResult:
-            self.expect_transform_result(test_case)
+    def validate(self, test_case: ValidateTestCase):
+        if test_case.expected_result_type == ValidateResult:
+            self.expect_validate_result(test_case)
         else:
             super().execute(test_case)
 
-    def expect_transform_result(self, test_case: TransformTestCase):
-        result = super().run_and_check_result_type(test_case, TransformResult)
-        self.assert_transform_result(test_case, result)
-
-    def assert_transform_result(self, test_case: TransformTestCase, result: TransformResult):
-        # Check output
-        self.compare_all_output(test_case.compare_tool, result.content)
-
-        # Check metadata
-        assert_keys_and_values(test_case.metadata, result.metadata)
-
-        # Check deleted metadata
-        for key in test_case.delete_metadata_keys:
-            assert_key_in(key, result.delete_metadata_keys)
-
-        # Check annotations
-        assert_keys_and_values(test_case.annotations, result.annotations)
+    def expect_validate_result(self, test_case: ValidateTestCase):
+        result = super().run_and_check_result_type(test_case, ValidateResult)
+        self.assert_validate_result(test_case, result)
+
+    def assert_validate_result(self, test_case: ValidateTestCase, result: ValidateResult):
+        # Check metrics
+        self.compare_metrics(test_case.expected_metrics, result.metrics)
```

### Comparing `deltafi-2.0rc1705080991758/pyproject.toml` & `deltafi-2.0rc1712763708188/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 [tool.poetry]
 name = "deltafi"
-version = "2.0rc1705080991758"
+version = "2.0rc1712763708188"
 description = "SDK for DeltaFi plugins and actions"
 authors = ["DeltaFi <deltafi@systolic.com>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 keywords = ["deltafi"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Software Development",
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10"
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-deepdiff = ">=6.3.1"
+python = "^3.9"
+deepdiff = ">=6.7.1"
 json-logging = ">=1.3.0"
-minio = ">=7.1.17"
-pydantic = ">=2.4.2"
+minio = ">=7.2.3"
+pydantic = ">=2.5.3"
 redis = ">=5.0.1"
 requests = ">=2.31.0"
-urllib3 = ">=2.0.6"
+urllib3 = ">=2.1.0"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = ">=7.4.2"
-pytest-mock = ">=3.11.1"
+pytest = ">=7.4.4"
+pytest-mock = ">=3.12.0"
 mockito = ">=1.4.0"
 
 [tool.poetry.urls]
 'Source Code' = "https://gitlab.com/deltafi/deltafi"
 Documentation = "https://docs.deltafi.org/#/"
 'Bug Reports' = "https://chat.deltafi.org/deltafi/channels/bug-reports"
```

### Comparing `deltafi-2.0rc1705080991758/PKG-INFO` & `deltafi-2.0rc1712763708188/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: deltafi
-Version: 2.0rc1705080991758
+Version: 2.0rc1712763708188
 Summary: SDK for DeltaFi plugins and actions
 License: Apache License, Version 2.0
 Keywords: deltafi
 Author: DeltaFi
 Author-email: deltafi@systolic.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
-Requires-Dist: deepdiff (>=6.3.1)
+Requires-Dist: deepdiff (>=6.7.1)
 Requires-Dist: json-logging (>=1.3.0)
-Requires-Dist: minio (>=7.1.17)
-Requires-Dist: pydantic (>=2.4.2)
+Requires-Dist: minio (>=7.2.3)
+Requires-Dist: pydantic (>=2.5.3)
 Requires-Dist: redis (>=5.0.1)
 Requires-Dist: requests (>=2.31.0)
-Requires-Dist: urllib3 (>=2.0.6)
+Requires-Dist: urllib3 (>=2.1.0)
 Project-URL: Bug Reports, https://chat.deltafi.org/deltafi/channels/bug-reports
 Project-URL: Documentation, https://docs.deltafi.org/#/
 Project-URL: Source Code, https://gitlab.com/deltafi/deltafi
 Description-Content-Type: text/markdown
 
 # DeltaFi Action Kit
```

