# Comparing `tmp/monday_code-0.0.1.tar.gz` & `tmp/monday_code-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monday_code-0.0.1.tar", last modified: Tue Apr 16 08:03:38 2024, max compression
+gzip compressed data, was "monday_code-0.0.2.tar", last modified: Tue Apr 16 08:20:00 2024, max compression
```

## Comparing `monday_code-0.0.1.tar` & `monday_code-0.0.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:38.908402 monday_code-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-16 08:03:38.908402 monday_code-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-04-16 08:03:33.000000 monday_code-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:38.896402 monday_code-0.0.1/monday_code/
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:38.900402 monday_code-0.0.1/monday_code/api/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21897 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/api/queue_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10463 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/api/secret_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    30670 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/api/secure_storage_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    45643 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/api/storage_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25779 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:38.904402 monday_code-0.0.1/monday_code/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/models/get_by_key_from_storage404_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/models/get_by_key_from_storage500_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/models/increment_counter_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/models/json_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/models/period.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/models/publish_message_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/models/publish_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/models/secure_storage_data_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/models/storage_data_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/models/validate_secret_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/models/validate_secret_response.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-04-16 08:03:33.000000 monday_code-0.0.1/monday_code/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:38.908402 monday_code-0.0.1/monday_code.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-16 08:03:38.000000 monday_code-0.0.1/monday_code.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-16 08:03:38.000000 monday_code-0.0.1/monday_code.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:03:38.000000 monday_code-0.0.1/monday_code.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 08:03:38.000000 monday_code-0.0.1/monday_code.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 08:03:38.000000 monday_code-0.0.1/monday_code.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-16 08:03:33.000000 monday_code-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 08:03:38.908402 monday_code-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-16 08:03:33.000000 monday_code-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:03:38.904402 monday_code-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-16 08:03:33.000000 monday_code-0.0.1/test/test_get_by_key_from_storage404_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-16 08:03:33.000000 monday_code-0.0.1/test/test_get_by_key_from_storage500_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-16 08:03:33.000000 monday_code-0.0.1/test/test_increment_counter_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-16 08:03:33.000000 monday_code-0.0.1/test/test_json_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-16 08:03:33.000000 monday_code-0.0.1/test/test_period.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-16 08:03:33.000000 monday_code-0.0.1/test/test_publish_message_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-16 08:03:33.000000 monday_code-0.0.1/test/test_publish_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-16 08:03:33.000000 monday_code-0.0.1/test/test_queue_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-16 08:03:33.000000 monday_code-0.0.1/test/test_secret_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-16 08:03:33.000000 monday_code-0.0.1/test/test_secure_storage_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-16 08:03:33.000000 monday_code-0.0.1/test/test_secure_storage_data_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-16 08:03:33.000000 monday_code-0.0.1/test/test_storage_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-16 08:03:33.000000 monday_code-0.0.1/test/test_storage_data_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-16 08:03:33.000000 monday_code-0.0.1/test/test_validate_secret_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-16 08:03:33.000000 monday_code-0.0.1/test/test_validate_secret_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:20:00.669873 monday_code-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-04-16 08:20:00.669873 monday_code-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-04-16 08:19:54.000000 monday_code-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:20:00.661873 monday_code-0.0.2/monday_code/
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:20:00.665873 monday_code-0.0.2/monday_code/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21897 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/api/queue_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10463 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/api/secret_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30670 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/api/secure_storage_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45643 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/api/storage_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25779 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:20:00.665873 monday_code-0.0.2/monday_code/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/models/get_by_key_from_storage404_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/models/get_by_key_from_storage500_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/models/increment_counter_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/models/json_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/models/period.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/models/publish_message_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/models/publish_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/models/secure_storage_data_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/models/storage_data_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/models/validate_secret_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/models/validate_secret_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-04-16 08:19:54.000000 monday_code-0.0.2/monday_code/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:20:00.669873 monday_code-0.0.2/monday_code.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-04-16 08:20:00.000000 monday_code-0.0.2/monday_code.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-16 08:20:00.000000 monday_code-0.0.2/monday_code.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:20:00.000000 monday_code-0.0.2/monday_code.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 08:20:00.000000 monday_code-0.0.2/monday_code.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 08:20:00.000000 monday_code-0.0.2/monday_code.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-16 08:19:54.000000 monday_code-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 08:20:00.669873 monday_code-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-16 08:19:54.000000 monday_code-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:20:00.669873 monday_code-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-16 08:19:54.000000 monday_code-0.0.2/test/test_get_by_key_from_storage404_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-16 08:19:54.000000 monday_code-0.0.2/test/test_get_by_key_from_storage500_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-16 08:19:54.000000 monday_code-0.0.2/test/test_increment_counter_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-16 08:19:54.000000 monday_code-0.0.2/test/test_json_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-16 08:19:54.000000 monday_code-0.0.2/test/test_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-16 08:19:54.000000 monday_code-0.0.2/test/test_publish_message_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-16 08:19:54.000000 monday_code-0.0.2/test/test_publish_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-16 08:19:54.000000 monday_code-0.0.2/test/test_queue_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-16 08:19:54.000000 monday_code-0.0.2/test/test_secret_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-16 08:19:54.000000 monday_code-0.0.2/test/test_secure_storage_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-16 08:19:54.000000 monday_code-0.0.2/test/test_secure_storage_data_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-16 08:19:54.000000 monday_code-0.0.2/test/test_storage_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-16 08:19:54.000000 monday_code-0.0.2/test/test_storage_data_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-16 08:19:54.000000 monday_code-0.0.2/test/test_validate_secret_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-16 08:19:54.000000 monday_code-0.0.2/test/test_validate_secret_response.py
```

### Comparing `monday_code-0.0.1/README.md` & `monday_code-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/monday_code/__init__.py` & `monday_code-0.0.2/monday_code/__init__.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/monday_code/api/queue_api.py` & `monday_code-0.0.2/monday_code/api/queue_api.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/monday_code/api/secret_api.py` & `monday_code-0.0.2/monday_code/api/secret_api.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/monday_code/api/secure_storage_api.py` & `monday_code-0.0.2/monday_code/api/secure_storage_api.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/monday_code/api/storage_api.py` & `monday_code-0.0.2/monday_code/api/storage_api.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/monday_code/api_client.py` & `monday_code-0.0.2/monday_code/api_client.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/monday_code/api_response.py` & `monday_code-0.0.2/monday_code/api_response.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/monday_code/configuration.py` & `monday_code-0.0.2/monday_code/configuration.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/monday_code/exceptions.py` & `monday_code-0.0.2/monday_code/exceptions.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/monday_code/models/__init__.py` & `monday_code-0.0.2/monday_code/models/__init__.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/monday_code/models/get_by_key_from_storage404_response.py` & `monday_code-0.0.2/monday_code/models/get_by_key_from_storage404_response.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/monday_code/models/get_by_key_from_storage500_response.py` & `monday_code-0.0.2/monday_code/models/get_by_key_from_storage500_response.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/monday_code/models/increment_counter_params.py` & `monday_code-0.0.2/monday_code/models/increment_counter_params.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/monday_code/models/json_value.py` & `monday_code-0.0.2/monday_code/models/json_value.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/monday_code/models/period.py` & `monday_code-0.0.2/monday_code/models/period.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/monday_code/models/publish_message_params.py` & `monday_code-0.0.2/monday_code/models/publish_message_params.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/monday_code/models/publish_message_response.py` & `monday_code-0.0.2/monday_code/models/publish_message_response.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/monday_code/models/secure_storage_data_contract.py` & `monday_code-0.0.2/monday_code/models/secure_storage_data_contract.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/monday_code/models/storage_data_contract.py` & `monday_code-0.0.2/monday_code/models/storage_data_contract.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/monday_code/models/validate_secret_params.py` & `monday_code-0.0.2/monday_code/models/validate_secret_params.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/monday_code/models/validate_secret_response.py` & `monday_code-0.0.2/monday_code/models/validate_secret_response.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/monday_code/rest.py` & `monday_code-0.0.2/monday_code/rest.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/monday_code.egg-info/SOURCES.txt` & `monday_code-0.0.2/monday_code.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/pyproject.toml` & `monday_code-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/setup.py` & `monday_code-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,34 +17,37 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "monday-code"
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
+# read the contents of your README file
+from pathlib import Path
+
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 setup(
     name=NAME,
     version=VERSION,
     description="mcode-sdk-api",
     author="OpenAPI Generator community",
     author_email="team@openapitools.org",
     url="",
     keywords=["OpenAPI", "OpenAPI-Generator", "mcode-sdk-api"],
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     license="MIT",
-    long_description_content_type='text/markdown',
-    long_description="""\
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
-    """,  # noqa: E501
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     package_data={"monday_code": ["py.typed"]},
 )
```

### Comparing `monday_code-0.0.1/test/test_get_by_key_from_storage404_response.py` & `monday_code-0.0.2/test/test_get_by_key_from_storage404_response.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/test/test_get_by_key_from_storage500_response.py` & `monday_code-0.0.2/test/test_get_by_key_from_storage500_response.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/test/test_increment_counter_params.py` & `monday_code-0.0.2/test/test_increment_counter_params.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/test/test_json_value.py` & `monday_code-0.0.2/test/test_json_value.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/test/test_period.py` & `monday_code-0.0.2/test/test_period.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/test/test_publish_message_params.py` & `monday_code-0.0.2/test/test_publish_message_params.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/test/test_publish_message_response.py` & `monday_code-0.0.2/test/test_publish_message_response.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/test/test_queue_api.py` & `monday_code-0.0.2/test/test_queue_api.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/test/test_secret_api.py` & `monday_code-0.0.2/test/test_secret_api.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/test/test_secure_storage_api.py` & `monday_code-0.0.2/test/test_secure_storage_api.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/test/test_secure_storage_data_contract.py` & `monday_code-0.0.2/test/test_secure_storage_data_contract.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/test/test_storage_api.py` & `monday_code-0.0.2/test/test_storage_api.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/test/test_storage_data_contract.py` & `monday_code-0.0.2/test/test_storage_data_contract.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/test/test_validate_secret_params.py` & `monday_code-0.0.2/test/test_validate_secret_params.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.1/test/test_validate_secret_response.py` & `monday_code-0.0.2/test/test_validate_secret_response.py`

 * *Files identical despite different names*

