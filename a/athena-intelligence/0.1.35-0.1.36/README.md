# Comparing `tmp/athena_intelligence-0.1.35.tar.gz` & `tmp/athena_intelligence-0.1.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athena_intelligence-0.1.35.tar", max compression
+gzip compressed data, was "athena_intelligence-0.1.36.tar", max compression
```

## Comparing `athena_intelligence-0.1.35.tar` & `athena_intelligence-0.1.36.tar`

### file list

```diff
@@ -1,45 +1,48 @@
--rw-r--r--   0        0        0     4235 2024-04-13 22:01:26.444142 athena_intelligence-0.1.35/README.md
--rw-r--r--   0        0        0      435 2024-04-13 22:01:26.444142 athena_intelligence-0.1.35/pyproject.toml
--rw-r--r--   0        0        0      905 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/__init__.py
--rw-r--r--   0        0        0     4806 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/base_client.py
--rw-r--r--   0        0        0     3576 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/client.py
--rw-r--r--   0        0        0      790 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/core/api_error.py
--rw-r--r--   0        0        0     1198 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/core/file.py
--rw-r--r--   0        0        0     4882 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/core/request_options.py
--rw-r--r--   0        0        0       65 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/dataset/__init__.py
--rw-r--r--   0        0        0     6087 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/dataset/client.py
--rw-r--r--   0        0        0      165 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/environment.py
--rw-r--r--   0        0        0      170 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0       65 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/message/__init__.py
--rw-r--r--   0        0        0    12185 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/message/client.py
--rw-r--r--   0        0        0     3998 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/polling_message_client.py
--rw-r--r--   0        0        0        0 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/py.typed
--rw-r--r--   0        0        0       65 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/query/__init__.py
--rw-r--r--   0        0        0     6243 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/query/client.py
--rw-r--r--   0        0        0       65 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/report/__init__.py
--rw-r--r--   0        0        0     6528 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/report/client.py
--rw-r--r--   0        0        0       65 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/snippet/__init__.py
--rw-r--r--   0        0        0     6087 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/snippet/client.py
--rw-r--r--   0        0        0      918 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/types/__init__.py
--rw-r--r--   0        0        0     1014 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/types/dataset.py
--rw-r--r--   0        0        0      989 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/types/get_datasets_response.py
--rw-r--r--   0        0        0      989 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/types/get_snippets_response.py
--rw-r--r--   0        0        0      973 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/types/http_validation_error.py
--rw-r--r--   0        0        0      865 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/types/message_out.py
--rw-r--r--   0        0        0     1051 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/types/message_out_dto.py
--rw-r--r--   0        0        0     2545 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/types/model.py
--rw-r--r--   0        0        0      946 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/types/report.py
--rw-r--r--   0        0        0     1126 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/types/snippet.py
--rw-r--r--   0        0        0      900 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/types/sql_results.py
--rw-r--r--   0        0        0      672 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/types/status_enum.py
--rw-r--r--   0        0        0     1422 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/types/tools.py
--rw-r--r--   0        0        0      992 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-13 22:01:26.448142 athena_intelligence-0.1.35/src/athena/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.35/PKG-INFO
+-rw-r--r--   0        0        0     4235 2024-04-16 20:06:14.200793 athena_intelligence-0.1.36/README.md
+-rw-r--r--   0        0        0      435 2024-04-16 20:06:14.200793 athena_intelligence-0.1.36/pyproject.toml
+-rw-r--r--   0        0        0      959 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/__init__.py
+-rw-r--r--   0        0        0     5014 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/base_client.py
+-rw-r--r--   0        0        0     3576 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/client.py
+-rw-r--r--   0        0        0      790 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/core/api_error.py
+-rw-r--r--   0        0        0     1198 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/core/file.py
+-rw-r--r--   0        0        0     4882 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/core/http_client.py
+-rw-r--r--   0        0        0     3799 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/core/request_options.py
+-rw-r--r--   0        0        0       65 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/dataset/__init__.py
+-rw-r--r--   0        0        0     6087 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/dataset/client.py
+-rw-r--r--   0        0        0      165 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/environment.py
+-rw-r--r--   0        0        0      170 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0       65 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/message/__init__.py
+-rw-r--r--   0        0        0    12185 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/message/client.py
+-rw-r--r--   0        0        0     3998 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/polling_message_client.py
+-rw-r--r--   0        0        0        0 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/py.typed
+-rw-r--r--   0        0        0       65 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/query/__init__.py
+-rw-r--r--   0        0        0     6243 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/query/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/report/__init__.py
+-rw-r--r--   0        0        0     6528 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/report/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/search/__init__.py
+-rw-r--r--   0        0        0    12255 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/search/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/snippet/__init__.py
+-rw-r--r--   0        0        0     6087 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/snippet/client.py
+-rw-r--r--   0        0        0      969 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/types/__init__.py
+-rw-r--r--   0        0        0     1014 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/types/dataset.py
+-rw-r--r--   0        0        0      989 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/types/get_datasets_response.py
+-rw-r--r--   0        0        0      989 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/types/get_snippets_response.py
+-rw-r--r--   0        0        0      973 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/types/http_validation_error.py
+-rw-r--r--   0        0        0      865 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/types/message_out.py
+-rw-r--r--   0        0        0     1051 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/types/message_out_dto.py
+-rw-r--r--   0        0        0     2545 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/types/model.py
+-rw-r--r--   0        0        0      946 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/types/report.py
+-rw-r--r--   0        0        0     1126 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/types/snippet.py
+-rw-r--r--   0        0        0      900 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/types/sql_results.py
+-rw-r--r--   0        0        0      672 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/types/status_enum.py
+-rw-r--r--   0        0        0     1422 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/types/tools.py
+-rw-r--r--   0        0        0      893 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/types/url_result.py
+-rw-r--r--   0        0        0      992 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-16 20:06:14.204793 athena_intelligence-0.1.36/src/athena/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.36/PKG-INFO
```

### Comparing `athena_intelligence-0.1.35/README.md` & `athena_intelligence-0.1.36/README.md`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/__init__.py` & `athena_intelligence-0.1.36/src/athena/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,19 +9,20 @@
     MessageOutDto,
     Model,
     Report,
     Snippet,
     SqlResults,
     StatusEnum,
     Tools,
+    UrlResult,
     ValidationError,
     ValidationErrorLocItem,
 )
 from .errors import UnprocessableEntityError
-from . import dataset, message, query, report, snippet
+from . import dataset, message, query, report, search, snippet
 from .environment import AthenaEnvironment
 
 __all__ = [
     "AthenaEnvironment",
     "Dataset",
     "GetDatasetsResponse",
     "GetSnippetsResponse",
@@ -31,15 +32,17 @@
     "Model",
     "Report",
     "Snippet",
     "SqlResults",
     "StatusEnum",
     "Tools",
     "UnprocessableEntityError",
+    "UrlResult",
     "ValidationError",
     "ValidationErrorLocItem",
     "dataset",
     "message",
     "query",
     "report",
+    "search",
     "snippet",
 ]
```

### Comparing `athena_intelligence-0.1.35/src/athena/base_client.py` & `athena_intelligence-0.1.36/src/athena/base_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from .core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .dataset.client import AsyncDatasetClient, DatasetClient
 from .environment import AthenaEnvironment
 from .message.client import AsyncMessageClient, MessageClient
 from .query.client import AsyncQueryClient, QueryClient
 from .report.client import AsyncReportClient, ReportClient
+from .search.client import AsyncSearchClient, SearchClient
 from .snippet.client import AsyncSnippetClient, SnippetClient
 
 
 class BaseAthena:
     """
     Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
 
@@ -52,14 +53,15 @@
             httpx_client=httpx.Client(timeout=timeout) if httpx_client is None else httpx_client,
         )
         self.message = MessageClient(client_wrapper=self._client_wrapper)
         self.dataset = DatasetClient(client_wrapper=self._client_wrapper)
         self.snippet = SnippetClient(client_wrapper=self._client_wrapper)
         self.report = ReportClient(client_wrapper=self._client_wrapper)
         self.query = QueryClient(client_wrapper=self._client_wrapper)
+        self.search = SearchClient(client_wrapper=self._client_wrapper)
 
 
 class AsyncBaseAthena:
     """
     Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
 
     Parameters:
@@ -97,14 +99,15 @@
             httpx_client=httpx.AsyncClient(timeout=timeout) if httpx_client is None else httpx_client,
         )
         self.message = AsyncMessageClient(client_wrapper=self._client_wrapper)
         self.dataset = AsyncDatasetClient(client_wrapper=self._client_wrapper)
         self.snippet = AsyncSnippetClient(client_wrapper=self._client_wrapper)
         self.report = AsyncReportClient(client_wrapper=self._client_wrapper)
         self.query = AsyncQueryClient(client_wrapper=self._client_wrapper)
+        self.search = AsyncSearchClient(client_wrapper=self._client_wrapper)
 
 
 def _get_base_url(*, base_url: typing.Optional[str] = None, environment: AthenaEnvironment) -> str:
     if base_url is not None:
         return base_url
     elif environment is not None:
         return environment.value
```

### Comparing `athena_intelligence-0.1.35/src/athena/client.py` & `athena_intelligence-0.1.36/src/athena/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/core/__init__.py` & `athena_intelligence-0.1.36/src/athena/core/__init__.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/core/client_wrapper.py` & `athena_intelligence-0.1.36/src/athena/core/client_wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self.api_key = api_key
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "athena-intelligence",
-            "X-Fern-SDK-Version": "0.1.35",
+            "X-Fern-SDK-Version": "0.1.36",
         }
         headers["X-API-KEY"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `athena_intelligence-0.1.35/src/athena/core/datetime_utils.py` & `athena_intelligence-0.1.36/src/athena/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/core/file.py` & `athena_intelligence-0.1.36/src/athena/core/file.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/core/http_client.py` & `athena_intelligence-0.1.36/src/athena/core/http_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/core/jsonable_encoder.py` & `athena_intelligence-0.1.36/src/athena/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/core/request_options.py` & `athena_intelligence-0.1.36/src/athena/core/request_options.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/dataset/client.py` & `athena_intelligence-0.1.36/src/athena/dataset/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/message/client.py` & `athena_intelligence-0.1.36/src/athena/message/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/polling_message_client.py` & `athena_intelligence-0.1.36/src/athena/polling_message_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/query/client.py` & `athena_intelligence-0.1.36/src/athena/query/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/report/client.py` & `athena_intelligence-0.1.36/src/athena/report/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/snippet/client.py` & `athena_intelligence-0.1.36/src/athena/snippet/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/types/__init__.py` & `athena_intelligence-0.1.36/src/athena/types/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .message_out_dto import MessageOutDto
 from .model import Model
 from .report import Report
 from .snippet import Snippet
 from .sql_results import SqlResults
 from .status_enum import StatusEnum
 from .tools import Tools
+from .url_result import UrlResult
 from .validation_error import ValidationError
 from .validation_error_loc_item import ValidationErrorLocItem
 
 __all__ = [
     "Dataset",
     "GetDatasetsResponse",
     "GetSnippetsResponse",
@@ -24,10 +25,11 @@
     "MessageOutDto",
     "Model",
     "Report",
     "Snippet",
     "SqlResults",
     "StatusEnum",
     "Tools",
+    "UrlResult",
     "ValidationError",
     "ValidationErrorLocItem",
 ]
```

### Comparing `athena_intelligence-0.1.35/src/athena/types/dataset.py` & `athena_intelligence-0.1.36/src/athena/types/dataset.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/types/get_datasets_response.py` & `athena_intelligence-0.1.36/src/athena/types/get_datasets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/types/get_snippets_response.py` & `athena_intelligence-0.1.36/src/athena/types/get_snippets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/types/http_validation_error.py` & `athena_intelligence-0.1.36/src/athena/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/types/message_out.py` & `athena_intelligence-0.1.36/src/athena/types/message_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/types/message_out_dto.py` & `athena_intelligence-0.1.36/src/athena/types/message_out_dto.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/types/model.py` & `athena_intelligence-0.1.36/src/athena/types/model.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/types/report.py` & `athena_intelligence-0.1.36/src/athena/types/report.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/types/snippet.py` & `athena_intelligence-0.1.36/src/athena/types/snippet.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/types/sql_results.py` & `athena_intelligence-0.1.36/src/athena/types/sql_results.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/types/status_enum.py` & `athena_intelligence-0.1.36/src/athena/types/status_enum.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/types/tools.py` & `athena_intelligence-0.1.36/src/athena/types/tools.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/src/athena/types/validation_error.py` & `athena_intelligence-0.1.36/src/athena/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.35/PKG-INFO` & `athena_intelligence-0.1.36/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athena-intelligence
-Version: 0.1.35
+Version: 0.1.36
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

