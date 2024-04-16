# Comparing `tmp/whylogs_container_client-1.0.8.tar.gz` & `tmp/whylogs_container_client-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylogs_container_client-1.0.8.tar", max compression
+gzip compressed data, was "whylogs_container_client-1.0.9.tar", max compression
```

## Comparing `whylogs_container_client-1.0.8.tar` & `whylogs_container_client-1.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     5548 2024-02-29 20:57:58.579066 whylogs_container_client-1.0.8/README.md
--rw-r--r--   0        0        0      582 2024-02-29 20:57:58.579066 whylogs_container_client-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      151 2024-02-29 21:01:39.348187 whylogs_container_client-1.0.8/whylogs_container_client/__init__.py
--rw-r--r--   0        0        0       47 2024-02-29 21:01:39.180187 whylogs_container_client-1.0.8/whylogs_container_client/api/__init__.py
--rw-r--r--   0        0        0        0 2024-02-29 21:01:39.264187 whylogs_container_client-1.0.8/whylogs_container_client/api/llm/__init__.py
--rw-r--r--   0        0        0     6769 2024-02-29 21:01:39.352187 whylogs_container_client-1.0.8/whylogs_container_client/api/llm/evaluate.py
--rw-r--r--   0        0        0     3796 2024-02-29 21:01:39.348187 whylogs_container_client-1.0.8/whylogs_container_client/api/llm/list_metrics.py
--rw-r--r--   0        0        0     4918 2024-02-29 21:01:39.348187 whylogs_container_client-1.0.8/whylogs_container_client/api/llm/log_llm.py
--rw-r--r--   0        0        0     7397 2024-02-29 21:01:39.348187 whylogs_container_client-1.0.8/whylogs_container_client/api/llm/validate_llm.py
--rw-r--r--   0        0        0        0 2024-02-29 21:01:39.272187 whylogs_container_client-1.0.8/whylogs_container_client/api/manage/__init__.py
--rw-r--r--   0        0        0     2176 2024-02-29 21:01:39.356187 whylogs_container_client-1.0.8/whylogs_container_client/api/manage/debug_info.py
--rw-r--r--   0        0        0     2089 2024-02-29 21:01:39.352187 whylogs_container_client-1.0.8/whylogs_container_client/api/manage/health.py
--rw-r--r--   0        0        0     2111 2024-02-29 21:01:39.352187 whylogs_container_client-1.0.8/whylogs_container_client/api/manage/publish.py
--rw-r--r--   0        0        0     3395 2024-02-29 21:01:39.352187 whylogs_container_client-1.0.8/whylogs_container_client/api/manage/status.py
--rw-r--r--   0        0        0        0 2024-02-29 21:01:39.208187 whylogs_container_client-1.0.8/whylogs_container_client/api/profile/__init__.py
--rw-r--r--   0        0        0    12385 2024-02-29 21:01:39.352187 whylogs_container_client-1.0.8/whylogs_container_client/api/profile/log.py
--rw-r--r--   0        0        0     9412 2024-02-29 21:01:39.352187 whylogs_container_client-1.0.8/whylogs_container_client/api/profile/log_embeddings.py
--rw-r--r--   0        0        0     2102 2024-02-29 21:01:39.352187 whylogs_container_client-1.0.8/whylogs_container_client/api/profile/log_pubsub.py
--rw-r--r--   0        0        0     2135 2024-02-29 21:01:39.352187 whylogs_container_client-1.0.8/whylogs_container_client/api/profile/log_pubsub_embedding.py
--rw-r--r--   0        0        0    12131 2024-02-29 21:01:39.348187 whylogs_container_client-1.0.8/whylogs_container_client/client.py
--rw-r--r--   0        0        0      470 2024-02-29 21:01:39.348187 whylogs_container_client-1.0.8/whylogs_container_client/errors.py
--rw-r--r--   0        0        0     1469 2024-02-29 21:01:39.172187 whylogs_container_client-1.0.8/whylogs_container_client/models/__init__.py
--rw-r--r--   0        0        0     1567 2024-02-29 21:01:39.356187 whylogs_container_client-1.0.8/whylogs_container_client/models/available_metrics.py
--rw-r--r--   0        0        0     3539 2024-02-29 21:01:39.356187 whylogs_container_client-1.0.8/whylogs_container_client/models/evaluation_result.py
--rw-r--r--   0        0        0     1296 2024-02-29 21:01:39.356187 whylogs_container_client-1.0.8/whylogs_container_client/models/evaluation_result_metrics_item.py
--rw-r--r--   0        0        0     2193 2024-02-29 21:01:39.360187 whylogs_container_client-1.0.8/whylogs_container_client/models/http_validation_error.py
--rw-r--r--   0        0        0     3757 2024-02-29 21:01:39.352187 whylogs_container_client-1.0.8/whylogs_container_client/models/llm_validate_request.py
--rw-r--r--   0        0        0     2237 2024-02-29 21:01:39.356187 whylogs_container_client-1.0.8/whylogs_container_client/models/log_embedding_request.py
--rw-r--r--   0        0        0     4620 2024-02-29 21:01:39.356187 whylogs_container_client-1.0.8/whylogs_container_client/models/log_embedding_request_embeddings.py
--rw-r--r--   0        0        0     4176 2024-02-29 21:01:39.360187 whylogs_container_client-1.0.8/whylogs_container_client/models/log_multiple.py
--rw-r--r--   0        0        0     2589 2024-02-29 21:01:39.356187 whylogs_container_client-1.0.8/whylogs_container_client/models/log_request.py
--rw-r--r--   0        0        0     3007 2024-02-29 21:01:39.356187 whylogs_container_client-1.0.8/whylogs_container_client/models/logger_status_response.py
--rw-r--r--   0        0        0     2081 2024-02-29 21:01:39.348187 whylogs_container_client-1.0.8/whylogs_container_client/models/process_logger_status_response.py
--rw-r--r--   0        0        0     1885 2024-02-29 21:01:39.360187 whylogs_container_client-1.0.8/whylogs_container_client/models/process_logger_status_response_statuses.py
--rw-r--r--   0        0        0     2655 2024-02-29 21:01:39.360187 whylogs_container_client-1.0.8/whylogs_container_client/models/run_perf.py
--rw-r--r--   0        0        0     1275 2024-02-29 21:01:39.356187 whylogs_container_client-1.0.8/whylogs_container_client/models/run_perf_metrics_time_sec.py
--rw-r--r--   0        0        0     2153 2024-02-29 21:01:39.360187 whylogs_container_client-1.0.8/whylogs_container_client/models/validation_error.py
--rw-r--r--   0        0        0     9593 2024-02-29 21:01:39.360187 whylogs_container_client-1.0.8/whylogs_container_client/models/validation_failure.py
--rw-r--r--   0        0        0     2189 2024-02-29 21:01:39.360187 whylogs_container_client-1.0.8/whylogs_container_client/models/validation_result.py
--rw-r--r--   0        0        0       25 2024-02-29 21:01:39.040187 whylogs_container_client-1.0.8/whylogs_container_client/py.typed
--rw-r--r--   0        0        0      986 2024-02-29 21:01:39.348187 whylogs_container_client-1.0.8/whylogs_container_client/types.py
--rw-r--r--   0        0        0     6232 1970-01-01 00:00:00.000000 whylogs_container_client-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     5548 2024-03-11 18:20:46.714396 whylogs_container_client-1.0.9/README.md
+-rw-r--r--   0        0        0      582 2024-03-11 18:20:46.714396 whylogs_container_client-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      151 2024-03-11 18:23:16.599223 whylogs_container_client-1.0.9/whylogs_container_client/__init__.py
+-rw-r--r--   0        0        0       47 2024-03-11 18:23:16.435222 whylogs_container_client-1.0.9/whylogs_container_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-11 18:23:16.523223 whylogs_container_client-1.0.9/whylogs_container_client/api/llm/__init__.py
+-rw-r--r--   0        0        0     6769 2024-03-11 18:23:16.595223 whylogs_container_client-1.0.9/whylogs_container_client/api/llm/evaluate.py
+-rw-r--r--   0        0        0     3796 2024-03-11 18:23:16.595223 whylogs_container_client-1.0.9/whylogs_container_client/api/llm/list_metrics.py
+-rw-r--r--   0        0        0     4918 2024-03-11 18:23:16.595223 whylogs_container_client-1.0.9/whylogs_container_client/api/llm/log_llm.py
+-rw-r--r--   0        0        0     7397 2024-03-11 18:23:16.595223 whylogs_container_client-1.0.9/whylogs_container_client/api/llm/validate_llm.py
+-rw-r--r--   0        0        0        0 2024-03-11 18:23:16.531223 whylogs_container_client-1.0.9/whylogs_container_client/api/manage/__init__.py
+-rw-r--r--   0        0        0     2176 2024-03-11 18:23:16.595223 whylogs_container_client-1.0.9/whylogs_container_client/api/manage/debug_info.py
+-rw-r--r--   0        0        0     2089 2024-03-11 18:23:16.591223 whylogs_container_client-1.0.9/whylogs_container_client/api/manage/health.py
+-rw-r--r--   0        0        0     2111 2024-03-11 18:23:16.591223 whylogs_container_client-1.0.9/whylogs_container_client/api/manage/publish.py
+-rw-r--r--   0        0        0     3395 2024-03-11 18:23:16.591223 whylogs_container_client-1.0.9/whylogs_container_client/api/manage/status.py
+-rw-r--r--   0        0        0        0 2024-03-11 18:23:16.463223 whylogs_container_client-1.0.9/whylogs_container_client/api/profile/__init__.py
+-rw-r--r--   0        0        0    12385 2024-03-11 18:23:16.599223 whylogs_container_client-1.0.9/whylogs_container_client/api/profile/log.py
+-rw-r--r--   0        0        0     9412 2024-03-11 18:23:16.595223 whylogs_container_client-1.0.9/whylogs_container_client/api/profile/log_embeddings.py
+-rw-r--r--   0        0        0     2102 2024-03-11 18:23:16.599223 whylogs_container_client-1.0.9/whylogs_container_client/api/profile/log_pubsub.py
+-rw-r--r--   0        0        0     2135 2024-03-11 18:23:16.599223 whylogs_container_client-1.0.9/whylogs_container_client/api/profile/log_pubsub_embedding.py
+-rw-r--r--   0        0        0    12131 2024-03-11 18:23:16.599223 whylogs_container_client-1.0.9/whylogs_container_client/client.py
+-rw-r--r--   0        0        0      470 2024-03-11 18:23:16.603223 whylogs_container_client-1.0.9/whylogs_container_client/errors.py
+-rw-r--r--   0        0        0     1469 2024-03-11 18:23:16.423222 whylogs_container_client-1.0.9/whylogs_container_client/models/__init__.py
+-rw-r--r--   0        0        0     1567 2024-03-11 18:23:16.603223 whylogs_container_client-1.0.9/whylogs_container_client/models/available_metrics.py
+-rw-r--r--   0        0        0     3539 2024-03-11 18:23:16.599223 whylogs_container_client-1.0.9/whylogs_container_client/models/evaluation_result.py
+-rw-r--r--   0        0        0     1296 2024-03-11 18:23:16.603223 whylogs_container_client-1.0.9/whylogs_container_client/models/evaluation_result_metrics_item.py
+-rw-r--r--   0        0        0     2193 2024-03-11 18:23:16.603223 whylogs_container_client-1.0.9/whylogs_container_client/models/http_validation_error.py
+-rw-r--r--   0        0        0     3757 2024-03-11 18:23:16.603223 whylogs_container_client-1.0.9/whylogs_container_client/models/llm_validate_request.py
+-rw-r--r--   0        0        0     2237 2024-03-11 18:23:16.603223 whylogs_container_client-1.0.9/whylogs_container_client/models/log_embedding_request.py
+-rw-r--r--   0        0        0     4620 2024-03-11 18:23:16.603223 whylogs_container_client-1.0.9/whylogs_container_client/models/log_embedding_request_embeddings.py
+-rw-r--r--   0        0        0     4176 2024-03-11 18:23:16.599223 whylogs_container_client-1.0.9/whylogs_container_client/models/log_multiple.py
+-rw-r--r--   0        0        0     2589 2024-03-11 18:23:16.599223 whylogs_container_client-1.0.9/whylogs_container_client/models/log_request.py
+-rw-r--r--   0        0        0     3007 2024-03-11 18:23:16.607223 whylogs_container_client-1.0.9/whylogs_container_client/models/logger_status_response.py
+-rw-r--r--   0        0        0     2081 2024-03-11 18:23:16.607223 whylogs_container_client-1.0.9/whylogs_container_client/models/process_logger_status_response.py
+-rw-r--r--   0        0        0     1885 2024-03-11 18:23:16.603223 whylogs_container_client-1.0.9/whylogs_container_client/models/process_logger_status_response_statuses.py
+-rw-r--r--   0        0        0     2655 2024-03-11 18:23:16.607223 whylogs_container_client-1.0.9/whylogs_container_client/models/run_perf.py
+-rw-r--r--   0        0        0     1275 2024-03-11 18:23:16.603223 whylogs_container_client-1.0.9/whylogs_container_client/models/run_perf_metrics_time_sec.py
+-rw-r--r--   0        0        0     2153 2024-03-11 18:23:16.603223 whylogs_container_client-1.0.9/whylogs_container_client/models/validation_error.py
+-rw-r--r--   0        0        0     9593 2024-03-11 18:23:16.607223 whylogs_container_client-1.0.9/whylogs_container_client/models/validation_failure.py
+-rw-r--r--   0        0        0     2189 2024-03-11 18:23:16.603223 whylogs_container_client-1.0.9/whylogs_container_client/models/validation_result.py
+-rw-r--r--   0        0        0       25 2024-03-11 18:23:16.287222 whylogs_container_client-1.0.9/whylogs_container_client/py.typed
+-rw-r--r--   0        0        0      986 2024-03-11 18:23:16.595223 whylogs_container_client-1.0.9/whylogs_container_client/types.py
+-rw-r--r--   0        0        0     6232 1970-01-01 00:00:00.000000 whylogs_container_client-1.0.9/PKG-INFO
```

### Comparing `whylogs_container_client-1.0.8/README.md` & `whylogs_container_client-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/pyproject.toml` & `whylogs_container_client-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whylogs-container-client"
-version = "1.0.8"
+version = "1.0.9"
 description = "A client library for accessing the whylogs python container"
 
 authors = ["Anthony Naddeo <anthony@whylabs.ai>"]
 
 readme = "README.md"
 packages = [
     {include = "whylogs_container_client"},
```

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/api/llm/evaluate.py` & `whylogs_container_client-1.0.9/whylogs_container_client/api/llm/evaluate.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/api/llm/list_metrics.py` & `whylogs_container_client-1.0.9/whylogs_container_client/api/llm/list_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/api/llm/log_llm.py` & `whylogs_container_client-1.0.9/whylogs_container_client/api/llm/log_llm.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/api/llm/validate_llm.py` & `whylogs_container_client-1.0.9/whylogs_container_client/api/llm/validate_llm.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/api/manage/debug_info.py` & `whylogs_container_client-1.0.9/whylogs_container_client/api/manage/debug_info.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/api/manage/health.py` & `whylogs_container_client-1.0.9/whylogs_container_client/api/manage/health.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/api/manage/publish.py` & `whylogs_container_client-1.0.9/whylogs_container_client/api/manage/publish.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/api/manage/status.py` & `whylogs_container_client-1.0.9/whylogs_container_client/api/manage/status.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/api/profile/log.py` & `whylogs_container_client-1.0.9/whylogs_container_client/api/profile/log.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/api/profile/log_embeddings.py` & `whylogs_container_client-1.0.9/whylogs_container_client/api/profile/log_embeddings.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/api/profile/log_pubsub.py` & `whylogs_container_client-1.0.9/whylogs_container_client/api/profile/log_pubsub.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/api/profile/log_pubsub_embedding.py` & `whylogs_container_client-1.0.9/whylogs_container_client/api/profile/log_pubsub_embedding.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/client.py` & `whylogs_container_client-1.0.9/whylogs_container_client/client.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/models/__init__.py` & `whylogs_container_client-1.0.9/whylogs_container_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/models/available_metrics.py` & `whylogs_container_client-1.0.9/whylogs_container_client/models/available_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/models/evaluation_result.py` & `whylogs_container_client-1.0.9/whylogs_container_client/models/evaluation_result.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/models/evaluation_result_metrics_item.py` & `whylogs_container_client-1.0.9/whylogs_container_client/models/evaluation_result_metrics_item.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/models/http_validation_error.py` & `whylogs_container_client-1.0.9/whylogs_container_client/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/models/llm_validate_request.py` & `whylogs_container_client-1.0.9/whylogs_container_client/models/llm_validate_request.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/models/log_embedding_request.py` & `whylogs_container_client-1.0.9/whylogs_container_client/models/log_embedding_request.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/models/log_embedding_request_embeddings.py` & `whylogs_container_client-1.0.9/whylogs_container_client/models/log_embedding_request_embeddings.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/models/log_multiple.py` & `whylogs_container_client-1.0.9/whylogs_container_client/models/log_multiple.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/models/log_request.py` & `whylogs_container_client-1.0.9/whylogs_container_client/models/log_request.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/models/logger_status_response.py` & `whylogs_container_client-1.0.9/whylogs_container_client/models/logger_status_response.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/models/process_logger_status_response.py` & `whylogs_container_client-1.0.9/whylogs_container_client/models/process_logger_status_response.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/models/process_logger_status_response_statuses.py` & `whylogs_container_client-1.0.9/whylogs_container_client/models/process_logger_status_response_statuses.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/models/run_perf.py` & `whylogs_container_client-1.0.9/whylogs_container_client/models/run_perf.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/models/run_perf_metrics_time_sec.py` & `whylogs_container_client-1.0.9/whylogs_container_client/models/run_perf_metrics_time_sec.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/models/validation_error.py` & `whylogs_container_client-1.0.9/whylogs_container_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/models/validation_failure.py` & `whylogs_container_client-1.0.9/whylogs_container_client/models/validation_failure.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/models/validation_result.py` & `whylogs_container_client-1.0.9/whylogs_container_client/models/validation_result.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/whylogs_container_client/types.py` & `whylogs_container_client-1.0.9/whylogs_container_client/types.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_client-1.0.8/PKG-INFO` & `whylogs_container_client-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylogs-container-client
-Version: 1.0.8
+Version: 1.0.9
 Summary: A client library for accessing the whylogs python container
 Author: Anthony Naddeo
 Author-email: anthony@whylabs.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

