# Comparing `tmp/fastdeploy-3.0.8.tar.gz` & `tmp/fastdeploy-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastdeploy-3.0.8.tar", last modified: Tue Mar 12 08:34:16 2024, max compression
+gzip compressed data, was "fastdeploy-3.0.9.tar", last modified: Tue Mar 12 09:03:12 2024, max compression
```

## Comparing `fastdeploy-3.0.8.tar` & `fastdeploy-3.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:34:16.679594 fastdeploy-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-12 08:34:13.000000 fastdeploy-3.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-03-12 08:34:16.679594 fastdeploy-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-03-12 08:34:13.000000 fastdeploy-3.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:34:16.679594 fastdeploy-3.0.8/fastdeploy/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-12 08:34:13.000000 fastdeploy-3.0.8/fastdeploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-03-12 08:34:13.000000 fastdeploy-3.0.8/fastdeploy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8490 2024-03-12 08:34:13.000000 fastdeploy-3.0.8/fastdeploy/_infer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-03-12 08:34:13.000000 fastdeploy-3.0.8/fastdeploy/_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-03-12 08:34:13.000000 fastdeploy-3.0.8/fastdeploy/_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-03-12 08:34:13.000000 fastdeploy-3.0.8/fastdeploy/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 08:34:16.679594 fastdeploy-3.0.8/fastdeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-03-12 08:34:16.000000 fastdeploy-3.0.8/fastdeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-12 08:34:16.000000 fastdeploy-3.0.8/fastdeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 08:34:16.000000 fastdeploy-3.0.8/fastdeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-12 08:34:16.000000 fastdeploy-3.0.8/fastdeploy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-12 08:34:16.000000 fastdeploy-3.0.8/fastdeploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-12 08:34:16.000000 fastdeploy-3.0.8/fastdeploy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 08:34:16.679594 fastdeploy-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-03-12 08:34:13.000000 fastdeploy-3.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 09:03:12.698139 fastdeploy-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-12 09:03:06.000000 fastdeploy-3.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-03-12 09:03:12.698139 fastdeploy-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-03-12 09:03:06.000000 fastdeploy-3.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 09:03:12.698139 fastdeploy-3.0.9/fastdeploy/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-12 09:03:06.000000 fastdeploy-3.0.9/fastdeploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-03-12 09:03:06.000000 fastdeploy-3.0.9/fastdeploy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8490 2024-03-12 09:03:06.000000 fastdeploy-3.0.9/fastdeploy/_infer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-03-12 09:03:06.000000 fastdeploy-3.0.9/fastdeploy/_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10667 2024-03-12 09:03:06.000000 fastdeploy-3.0.9/fastdeploy/_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-03-12 09:03:06.000000 fastdeploy-3.0.9/fastdeploy/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 09:03:12.698139 fastdeploy-3.0.9/fastdeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-03-12 09:03:12.000000 fastdeploy-3.0.9/fastdeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-12 09:03:12.000000 fastdeploy-3.0.9/fastdeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 09:03:12.000000 fastdeploy-3.0.9/fastdeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-12 09:03:12.000000 fastdeploy-3.0.9/fastdeploy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-12 09:03:12.000000 fastdeploy-3.0.9/fastdeploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-12 09:03:12.000000 fastdeploy-3.0.9/fastdeploy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 09:03:12.698139 fastdeploy-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-03-12 09:03:06.000000 fastdeploy-3.0.9/setup.py
```

### Comparing `fastdeploy-3.0.8/LICENSE` & `fastdeploy-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastdeploy-3.0.8/PKG-INFO` & `fastdeploy-3.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastdeploy
-Version: 3.0.8
+Version: 3.0.9
 Summary: Deploy DL/ ML inference pipelines with minimal extra code. 
 Home-page: https://github.com/notAI-tech/fastDeploy
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `fastdeploy-3.0.8/README.md` & `fastdeploy-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fastdeploy-3.0.8/fastdeploy/__main__.py` & `fastdeploy-3.0.9/fastdeploy/__main__.py`

 * *Files identical despite different names*

### Comparing `fastdeploy-3.0.8/fastdeploy/_infer.py` & `fastdeploy-3.0.9/fastdeploy/_infer.py`

 * *Files identical despite different names*

### Comparing `fastdeploy-3.0.8/fastdeploy/_loop.py` & `fastdeploy-3.0.9/fastdeploy/_loop.py`

 * *Files identical despite different names*

### Comparing `fastdeploy-3.0.8/fastdeploy/_rest.py` & `fastdeploy-3.0.9/fastdeploy/_rest.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,53 +134,53 @@
 
             if _temp_sum_of_received_at and _temp_sum_of_predicted_at:
                 avg_actual_total_time_per_req_for_reqs_in_last_x_seconds = (
                     _temp_sum_of_predicted_at - _temp_sum_of_received_at
                 ) / requests_received_in_last_x_seconds_that_are_successful
 
         prometheus_text = f"""
-        # HELP pending_requests The number of pending requests.
-        # TYPE pending_requests gauge
-        pending_requests {_utils.MAIN_INDEX.count(query={"-1.predicted_at": 0, "last_predictor_success": True})}
-
-        # HELP failed_requests The number of failed requests.
-        # TYPE failed_requests gauge
-        failed_requests {_utils.MAIN_INDEX.count(query={"last_predictor_success": False})}
-
-        # HELP successful_requests The number of failed requests.
-        # TYPE successful_requests gauge
-        successful_requests {_utils.MAIN_INDEX.count(query={"-1.predicted_at": {"$ne": 0}, "last_predictor_success": True})}
-
-        # HELP requests_received_in_last_x_seconds The number of requests received in last {_LAST_X_SECONDS} seconds.
-        # TYPE requests_received_in_last_x_seconds gauge
-        requests_received_in_last_x_seconds {requests_received_in_last_x_seconds}
-
-        # HELP requests_received_in_last_x_seconds_that_failed The number of requests received in last {_LAST_X_SECONDS} seconds that failed.
-        # TYPE requests_received_in_last_x_seconds_that_failed gauge
-        requests_received_in_last_x_seconds_that_failed {requests_received_in_last_x_seconds_that_failed}
-
-        # HELP requests_received_in_last_x_seconds_that_are_pending The number of requests received in last {_LAST_X_SECONDS} seconds that are pending.
-        # TYPE requests_received_in_last_x_seconds_that_are_pending gauge
-        requests_received_in_last_x_seconds_that_are_pending {requests_received_in_last_x_seconds_that_are_pending}
-
-        # HELP requests_received_in_last_x_seconds_that_are_successful The number of requests received in last {_LAST_X_SECONDS} seconds that are successful.
-        # TYPE requests_received_in_last_x_seconds_that_are_successful gauge
-        requests_received_in_last_x_seconds_that_are_successful {requests_received_in_last_x_seconds_that_are_successful}
-
-        # HELP avg_total_time_per_req_for_reqs_in_last_x_seconds The average total time per request for requests in last {_LAST_X_SECONDS} seconds.
-        # TYPE avg_total_time_per_req_for_reqs_in_last_x_seconds gauge
-        avg_total_time_per_req_for_reqs_in_last_x_seconds {avg_total_time_per_req_for_reqs_in_last_x_seconds}
-
-        # HELP avg_actual_total_time_per_req_for_reqs_in_last_x_seconds The average actual total time per request for requests in last {_LAST_X_SECONDS} seconds.
-        # TYPE avg_actual_total_time_per_req_for_reqs_in_last_x_seconds gauge
-        avg_actual_total_time_per_req_for_reqs_in_last_x_seconds {avg_actual_total_time_per_req_for_reqs_in_last_x_seconds}
-
-        # HELP requests_received_in_last_x_seconds The number of requests received in last {_LAST_X_SECONDS} seconds.
-        # TYPE requests_received_in_last_x_seconds gauge
-        requests_received_in_last_x_seconds {requests_received_in_last_x_seconds}
+# HELP pending_requests The number of pending requests.
+# TYPE pending_requests gauge
+pending_requests {_utils.MAIN_INDEX.count(query={"-1.predicted_at": 0, "last_predictor_success": True})}
+
+# HELP failed_requests The number of failed requests.
+# TYPE failed_requests gauge
+failed_requests {_utils.MAIN_INDEX.count(query={"last_predictor_success": False})}
+
+# HELP successful_requests The number of failed requests.
+# TYPE successful_requests gauge
+successful_requests {_utils.MAIN_INDEX.count(query={"-1.predicted_at": {"$ne": 0}, "last_predictor_success": True})}
+
+# HELP requests_received_in_last_x_seconds The number of requests received in last {_LAST_X_SECONDS} seconds.
+# TYPE requests_received_in_last_x_seconds gauge
+requests_received_in_last_x_seconds {requests_received_in_last_x_seconds}
+
+# HELP requests_received_in_last_x_seconds_that_failed The number of requests received in last {_LAST_X_SECONDS} seconds that failed.
+# TYPE requests_received_in_last_x_seconds_that_failed gauge
+requests_received_in_last_x_seconds_that_failed {requests_received_in_last_x_seconds_that_failed}
+
+# HELP requests_received_in_last_x_seconds_that_are_pending The number of requests received in last {_LAST_X_SECONDS} seconds that are pending.
+# TYPE requests_received_in_last_x_seconds_that_are_pending gauge
+requests_received_in_last_x_seconds_that_are_pending {requests_received_in_last_x_seconds_that_are_pending}
+
+# HELP requests_received_in_last_x_seconds_that_are_successful The number of requests received in last {_LAST_X_SECONDS} seconds that are successful.
+# TYPE requests_received_in_last_x_seconds_that_are_successful gauge
+requests_received_in_last_x_seconds_that_are_successful {requests_received_in_last_x_seconds_that_are_successful}
+
+# HELP avg_total_time_per_req_for_reqs_in_last_x_seconds The average total time per request for requests in last {_LAST_X_SECONDS} seconds.
+# TYPE avg_total_time_per_req_for_reqs_in_last_x_seconds gauge
+avg_total_time_per_req_for_reqs_in_last_x_seconds {avg_total_time_per_req_for_reqs_in_last_x_seconds}
+
+# HELP avg_actual_total_time_per_req_for_reqs_in_last_x_seconds The average actual total time per request for requests in last {_LAST_X_SECONDS} seconds.
+# TYPE avg_actual_total_time_per_req_for_reqs_in_last_x_seconds gauge
+avg_actual_total_time_per_req_for_reqs_in_last_x_seconds {avg_actual_total_time_per_req_for_reqs_in_last_x_seconds}
+
+# HELP requests_received_in_last_x_seconds The number of requests received in last {_LAST_X_SECONDS} seconds.
+# TYPE requests_received_in_last_x_seconds gauge
+requests_received_in_last_x_seconds {requests_received_in_last_x_seconds}
         """.strip()
 
         resp.status = falcon.HTTP_200
         resp.content_type = "text/plain; version=0.0.4"
         resp.text = prometheus_text
```

### Comparing `fastdeploy-3.0.8/fastdeploy/_utils.py` & `fastdeploy-3.0.9/fastdeploy/_utils.py`

 * *Files identical despite different names*

### Comparing `fastdeploy-3.0.8/fastdeploy.egg-info/PKG-INFO` & `fastdeploy-3.0.9/fastdeploy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastdeploy
-Version: 3.0.8
+Version: 3.0.9
 Summary: Deploy DL/ ML inference pipelines with minimal extra code. 
 Home-page: https://github.com/notAI-tech/fastDeploy
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `fastdeploy-3.0.8/setup.py` & `fastdeploy-3.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "fastdeploy"
 DESCRIPTION = "Deploy DL/ ML inference pipelines with minimal extra code. "
 URL = "https://github.com/notAI-tech/fastDeploy"
 EMAIL = "praneeth@bpraneeth.com"
 AUTHOR = "BEDAPUDI PRANEETH"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "3.0.8"
+VERSION = "3.0.9"
 
 # What packages are required for this module to be executed?
 REQUIRED = ["falcon", "liteindex", "zstandard", "gunicorn[gevent]"]
 
 # What packages are optional?
 EXTRAS = {
     'msgpack': ['msgpack'],
```

