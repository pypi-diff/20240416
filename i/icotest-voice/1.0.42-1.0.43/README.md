# Comparing `tmp/icotest-voice-1.0.42.tar.gz` & `tmp/icotest_voice-1.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icotest-voice-1.0.42.tar", last modified: Mon Mar 18 14:44:45 2024, max compression
+gzip compressed data, was "icotest_voice-1.0.43.tar", last modified: Mon Apr 15 16:33:30 2024, max compression
```

## Comparing `icotest-voice-1.0.42.tar` & `icotest_voice-1.0.43.tar`

### file list

```diff
@@ -1,58 +1,56 @@
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2024-03-18 14:44:45.368862 icotest-voice-1.0.42/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1067 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/LICENSE
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       18 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/MANIFEST.in
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    11036 2024-03-18 14:44:45.368862 icotest-voice-1.0.42/PKG-INFO
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     9239 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/README.md
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2024-03-18 14:44:45.364862 icotest-voice-1.0.42/docs/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1340 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/docs/Controller.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8694 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/docs/ControllersApi.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1568 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/docs/Device.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    42893 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/docs/DevicesApi.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1244 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/docs/GetTestResultFileList200Response.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1380 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/docs/GetTestResultFileList200ResponseFilesInner.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1008 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/docs/HostConfig.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1087 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/docs/PostDeviceRegisterRequest.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1351 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/docs/Request.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    44152 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/docs/RequestsApi.md
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2024-03-18 14:44:45.364862 icotest-voice-1.0.42/icotest_voice/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1556 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/icotest_voice/__init__.py
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2024-03-18 14:44:45.364862 icotest-voice-1.0.42/icotest_voice/api/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      217 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/icotest_voice/api/__init__.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    41923 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/icotest_voice/api/controllers_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)   207993 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/icotest_voice/api/devices_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)   211723 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/icotest_voice/api/requests_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    24877 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/icotest_voice/api_client.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      674 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/icotest_voice/api_response.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    13895 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/icotest_voice/configuration.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     5399 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/icotest_voice/exceptions.py
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2024-03-18 14:44:45.368862 icotest-voice-1.0.42/icotest_voice/models/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      851 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/icotest_voice/models/__init__.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     4444 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/icotest_voice/models/controller.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     5579 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/icotest_voice/models/device.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     2982 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/icotest_voice/models/get_test_result_file_list200_response.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     2685 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/icotest_voice/models/get_test_result_file_list200_response_files_inner.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3024 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/icotest_voice/models/host_config.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     2527 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/icotest_voice/models/post_device_register_request.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     6551 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/icotest_voice/models/request.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)        0 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/icotest_voice/py.typed
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8246 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/icotest_voice/rest.py
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2024-03-18 14:44:45.368862 icotest-voice-1.0.42/icotest_voice.egg-info/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    11036 2024-03-18 14:44:45.000000 icotest-voice-1.0.42/icotest_voice.egg-info/PKG-INFO
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1508 2024-03-18 14:44:45.000000 icotest-voice-1.0.42/icotest_voice.egg-info/SOURCES.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)        1 2024-03-18 14:44:45.000000 icotest-voice-1.0.42/icotest_voice.egg-info/dependency_links.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      102 2024-03-18 14:44:45.000000 icotest-voice-1.0.42/icotest_voice.egg-info/requires.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       14 2024-03-18 14:44:45.000000 icotest-voice-1.0.42/icotest_voice.egg-info/top_level.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      782 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/pyproject.toml
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       69 2024-03-18 14:44:45.368862 icotest-voice-1.0.42/setup.cfg
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1189 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/setup.py
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2024-03-18 14:44:45.368862 icotest-voice-1.0.42/test/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1761 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/test/test_controller.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1180 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/test/test_controllers_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1989 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/test/test_device.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3245 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/test/test_devices_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1862 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/test/test_get_test_result_file_list200_response.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1763 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/test/test_get_test_result_file_list200_response_files_inner.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1725 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/test/test_host_config.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1503 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/test/test_post_device_register_request.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1937 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/test/test_request.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3763 2024-03-18 14:44:42.000000 icotest-voice-1.0.42/test/test_requests_api.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2024-04-15 16:33:30.503306 icotest_voice-1.0.43/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1067 2024-02-26 13:04:19.000000 icotest_voice-1.0.43/LICENSE
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       18 2024-02-26 13:04:19.000000 icotest_voice-1.0.43/MANIFEST.in
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    10458 2024-04-15 16:33:30.503306 icotest_voice-1.0.43/PKG-INFO
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8870 2024-04-15 16:29:30.000000 icotest_voice-1.0.43/README.md
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2024-04-15 16:33:30.495306 icotest_voice-1.0.43/docs/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1340 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/docs/Controller.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8694 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/docs/ControllersApi.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1568 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/docs/Device.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    45143 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/docs/DevicesApi.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1244 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/docs/GetTestResultFileList200Response.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1380 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/docs/GetTestResultFileList200ResponseFilesInner.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1008 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/docs/HostConfig.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1087 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/docs/PostDeviceRegisterRequest.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1351 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/docs/Request.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    44171 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/docs/RequestsApi.md
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2024-04-15 16:33:30.499306 icotest_voice-1.0.43/icotest_voice/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1556 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/icotest_voice/__init__.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2024-04-15 16:33:30.499306 icotest_voice-1.0.43/icotest_voice/api/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      217 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/icotest_voice/api/__init__.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    41923 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/icotest_voice/api/controllers_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)   219229 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/icotest_voice/api/devices_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)   211723 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/icotest_voice/api/requests_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    24877 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/icotest_voice/api_client.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      674 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/icotest_voice/api_response.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    13895 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/icotest_voice/configuration.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     5399 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/icotest_voice/exceptions.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2024-04-15 16:33:30.499306 icotest_voice-1.0.43/icotest_voice/models/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      851 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/icotest_voice/models/__init__.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     4448 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/icotest_voice/models/controller.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     5587 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/icotest_voice/models/device.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     2982 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/icotest_voice/models/get_test_result_file_list200_response.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     2685 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/icotest_voice/models/get_test_result_file_list200_response_files_inner.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3024 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/icotest_voice/models/host_config.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     2527 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/icotest_voice/models/post_device_register_request.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     6727 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/icotest_voice/models/request.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)        0 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/icotest_voice/py.typed
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8246 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/icotest_voice/rest.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2024-04-15 16:33:30.503306 icotest_voice-1.0.43/icotest_voice.egg-info/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    10458 2024-04-15 16:33:30.000000 icotest_voice-1.0.43/icotest_voice.egg-info/PKG-INFO
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1453 2024-04-15 16:33:30.000000 icotest_voice-1.0.43/icotest_voice.egg-info/SOURCES.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)        1 2024-04-15 16:33:30.000000 icotest_voice-1.0.43/icotest_voice.egg-info/dependency_links.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       14 2024-04-15 16:33:30.000000 icotest_voice-1.0.43/icotest_voice.egg-info/top_level.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      614 2024-04-15 16:33:09.000000 icotest_voice-1.0.43/pyproject.toml
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       38 2024-04-15 16:33:30.503306 icotest_voice-1.0.43/setup.cfg
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2024-04-15 16:33:30.503306 icotest_voice-1.0.43/test/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1761 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/test/test_controller.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1180 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/test/test_controllers_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1989 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/test/test_device.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3402 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/test/test_devices_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1862 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/test/test_get_test_result_file_list200_response.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1763 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/test/test_get_test_result_file_list200_response_files_inner.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1725 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/test/test_host_config.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1503 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/test/test_post_device_register_request.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1937 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/test/test_request.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3763 2024-04-15 16:21:05.000000 icotest_voice-1.0.43/test/test_requests_api.py
```

### Comparing `icotest-voice-1.0.42/LICENSE` & `icotest_voice-1.0.43/LICENSE`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.42/PKG-INFO` & `icotest_voice-1.0.43/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,105 +1,79 @@
 Metadata-Version: 2.1
 Name: icotest-voice
-Version: 1.0.42
+Version: 1.0.43
 Summary: Icotest Voice API
-Home-page: 
-Author: Shaun Hirst
 Author-email: Shaun Hirst <shaun.hirst@3adesign.co.uk>, Ivo Shipkaliev <ivo@3adesign.co.uk>
 License: Copyright © 2024 3ADesign Limited
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Keywords: OpenAPI,OpenAPI-Generator,Icotest Voice
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.4
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: python_dateutil>=2.5.3
-Requires-Dist: urllib3<2.1.0,>=1.25.3
-Requires-Dist: pydantic>=2
-Requires-Dist: typing-extensions>=4.7.1
-Requires-Dist: setuptools>=21.0.0
 
 # icotest-voice
 IcoTest Voice API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.42
-- Package version: 1.0.42
+- API version: 1.0.43
+- Package version: 1.0.43
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
 ### pip install
 
-If the python package is hosted on a repository, you can install directly using:
-
 ```sh
-pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
+pip install icotest-voice
 ```
-(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
-
-Then import the package:
-```python
-import icotest_voice
-```
-
-### Setuptools
-
-Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
-
-```sh
-python setup.py install --user
-```
-(or `sudo python setup.py install` to install the package for all users)
 
 Then import the package:
 ```python
 import icotest_voice
 ```
 
 ### Tests
 
 Execute `pytest` to run the tests.
 
 ## Getting Started
 
-Please follow the [installation procedure](#installation--usage) and then run the following:
+Please follow the installation procedure and then run the following:
 
 ```python
 
 import time
 import icotest_voice
 from icotest_voice.rest import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to https://localhost/icotest_voice
 # See configuration.py for a list of all supported configuration parameters.
 configuration = icotest_voice.Configuration(
     host = "https://localhost/icotest_voice"
 )
 
-
-
 # Enter a context with an instance of the API client
 with icotest_voice.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = icotest_voice.ControllersApi(api_client)
-    controller_id = 'ac331ccb-5841-44ec-9d32-4f4fe0c3c16c' # str | the unique id of the controller
+    controller_id = "ac331ccb-5841-44ec-9d32-4f4fe0c3c16c"  # str: the unique ID of the controller
 
     try:
         # DELETE Controller
         api_instance.delete_controller(controller_id)
     except ApiException as e:
         print("Exception when calling ControllersApi->delete_controller: %s\n" % e)
 
@@ -117,14 +91,15 @@
 *ControllersApi* | [**put_controller**](docs/ControllersApi.md#put_controller) | **PUT** /controllers | PUT controller
 *DevicesApi* | [**delete_device**](docs/DevicesApi.md#delete_device) | **DELETE** /devices | DELETE Device
 *DevicesApi* | [**get_device_status**](docs/DevicesApi.md#get_device_status) | **GET** /devices/{device_id}/status | GET device status
 *DevicesApi* | [**get_devices**](docs/DevicesApi.md#get_devices) | **GET** /devices | GET devices
 *DevicesApi* | [**get_host_config**](docs/DevicesApi.md#get_host_config) | **GET** /host/config | Your GET endpoint
 *DevicesApi* | [**post_device_appium_take_screenshot**](docs/DevicesApi.md#post_device_appium_take_screenshot) | **POST** /devices/{device_id}/APPIUM_take_screenshot | POST APPIUM take screenshot
 *DevicesApi* | [**post_device_dect_get_handset_name**](docs/DevicesApi.md#post_device_dect_get_handset_name) | **POST** /devices/{device_id}/DECT_get_handset_name | POST DECT Get Handset Name
+*DevicesApi* | [**post_device_dect_reset**](docs/DevicesApi.md#post_device_dect_reset) | **POST** /devices/{device_id}/DECT_reset | POST DECT Device Reset
 *DevicesApi* | [**post_device_dect_run_at_cmd**](docs/DevicesApi.md#post_device_dect_run_at_cmd) | **POST** /devices/{device_id}/DECT_run_AT_command | POST DECT Run AT Command
 *DevicesApi* | [**post_device_deregister**](docs/DevicesApi.md#post_device_deregister) | **POST** /devices/{device_id}/deregister | POST deregister device
 *DevicesApi* | [**post_device_end_call**](docs/DevicesApi.md#post_device_end_call) | **POST** /devices/{device_id}/end_call | POST end call
 *DevicesApi* | [**post_device_heartbeat**](docs/DevicesApi.md#post_device_heartbeat) | **POST** /devices/{device_id}/heartbeat | POST Device heartbeat
 *DevicesApi* | [**post_device_make_call**](docs/DevicesApi.md#post_device_make_call) | **POST** /devices/{device_id}/make_call | POST make call
 *DevicesApi* | [**post_device_receive_call**](docs/DevicesApi.md#post_device_receive_call) | **POST** /devices/{device_id}/receive_call | POST receive call
 *DevicesApi* | [**post_device_register**](docs/DevicesApi.md#post_device_register) | **POST** /devices/{device_id}/register | POST register device
```

### Comparing `icotest-voice-1.0.42/README.md` & `icotest_voice-1.0.43/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,77 +1,58 @@
 # icotest-voice
 IcoTest Voice API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.42
-- Package version: 1.0.42
+- API version: 1.0.43
+- Package version: 1.0.43
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
 ### pip install
 
-If the python package is hosted on a repository, you can install directly using:
-
 ```sh
-pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
+pip install icotest-voice
 ```
-(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
-
-Then import the package:
-```python
-import icotest_voice
-```
-
-### Setuptools
-
-Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
-
-```sh
-python setup.py install --user
-```
-(or `sudo python setup.py install` to install the package for all users)
 
 Then import the package:
 ```python
 import icotest_voice
 ```
 
 ### Tests
 
 Execute `pytest` to run the tests.
 
 ## Getting Started
 
-Please follow the [installation procedure](#installation--usage) and then run the following:
+Please follow the installation procedure and then run the following:
 
 ```python
 
 import time
 import icotest_voice
 from icotest_voice.rest import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to https://localhost/icotest_voice
 # See configuration.py for a list of all supported configuration parameters.
 configuration = icotest_voice.Configuration(
     host = "https://localhost/icotest_voice"
 )
 
-
-
 # Enter a context with an instance of the API client
 with icotest_voice.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = icotest_voice.ControllersApi(api_client)
-    controller_id = 'ac331ccb-5841-44ec-9d32-4f4fe0c3c16c' # str | the unique id of the controller
+    controller_id = "ac331ccb-5841-44ec-9d32-4f4fe0c3c16c"  # str: the unique ID of the controller
 
     try:
         # DELETE Controller
         api_instance.delete_controller(controller_id)
     except ApiException as e:
         print("Exception when calling ControllersApi->delete_controller: %s\n" % e)
 
@@ -89,14 +70,15 @@
 *ControllersApi* | [**put_controller**](docs/ControllersApi.md#put_controller) | **PUT** /controllers | PUT controller
 *DevicesApi* | [**delete_device**](docs/DevicesApi.md#delete_device) | **DELETE** /devices | DELETE Device
 *DevicesApi* | [**get_device_status**](docs/DevicesApi.md#get_device_status) | **GET** /devices/{device_id}/status | GET device status
 *DevicesApi* | [**get_devices**](docs/DevicesApi.md#get_devices) | **GET** /devices | GET devices
 *DevicesApi* | [**get_host_config**](docs/DevicesApi.md#get_host_config) | **GET** /host/config | Your GET endpoint
 *DevicesApi* | [**post_device_appium_take_screenshot**](docs/DevicesApi.md#post_device_appium_take_screenshot) | **POST** /devices/{device_id}/APPIUM_take_screenshot | POST APPIUM take screenshot
 *DevicesApi* | [**post_device_dect_get_handset_name**](docs/DevicesApi.md#post_device_dect_get_handset_name) | **POST** /devices/{device_id}/DECT_get_handset_name | POST DECT Get Handset Name
+*DevicesApi* | [**post_device_dect_reset**](docs/DevicesApi.md#post_device_dect_reset) | **POST** /devices/{device_id}/DECT_reset | POST DECT Device Reset
 *DevicesApi* | [**post_device_dect_run_at_cmd**](docs/DevicesApi.md#post_device_dect_run_at_cmd) | **POST** /devices/{device_id}/DECT_run_AT_command | POST DECT Run AT Command
 *DevicesApi* | [**post_device_deregister**](docs/DevicesApi.md#post_device_deregister) | **POST** /devices/{device_id}/deregister | POST deregister device
 *DevicesApi* | [**post_device_end_call**](docs/DevicesApi.md#post_device_end_call) | **POST** /devices/{device_id}/end_call | POST end call
 *DevicesApi* | [**post_device_heartbeat**](docs/DevicesApi.md#post_device_heartbeat) | **POST** /devices/{device_id}/heartbeat | POST Device heartbeat
 *DevicesApi* | [**post_device_make_call**](docs/DevicesApi.md#post_device_make_call) | **POST** /devices/{device_id}/make_call | POST make call
 *DevicesApi* | [**post_device_receive_call**](docs/DevicesApi.md#post_device_receive_call) | **POST** /devices/{device_id}/receive_call | POST receive call
 *DevicesApi* | [**post_device_register**](docs/DevicesApi.md#post_device_register) | **POST** /devices/{device_id}/register | POST register device
```

### Comparing `icotest-voice-1.0.42/docs/Controller.md` & `icotest_voice-1.0.43/docs/Controller.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.42/docs/ControllersApi.md` & `icotest_voice-1.0.43/docs/ControllersApi.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.42/docs/Device.md` & `icotest_voice-1.0.43/docs/Device.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.42/docs/DevicesApi.md` & `icotest_voice-1.0.43/docs/DevicesApi.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 ------------- | ------------- | -------------
 [**delete_device**](DevicesApi.md#delete_device) | **DELETE** /devices | DELETE Device
 [**get_device_status**](DevicesApi.md#get_device_status) | **GET** /devices/{device_id}/status | GET device status
 [**get_devices**](DevicesApi.md#get_devices) | **GET** /devices | GET devices
 [**get_host_config**](DevicesApi.md#get_host_config) | **GET** /host/config | Your GET endpoint
 [**post_device_appium_take_screenshot**](DevicesApi.md#post_device_appium_take_screenshot) | **POST** /devices/{device_id}/APPIUM_take_screenshot | POST APPIUM take screenshot
 [**post_device_dect_get_handset_name**](DevicesApi.md#post_device_dect_get_handset_name) | **POST** /devices/{device_id}/DECT_get_handset_name | POST DECT Get Handset Name
+[**post_device_dect_reset**](DevicesApi.md#post_device_dect_reset) | **POST** /devices/{device_id}/DECT_reset | POST DECT Device Reset
 [**post_device_dect_run_at_cmd**](DevicesApi.md#post_device_dect_run_at_cmd) | **POST** /devices/{device_id}/DECT_run_AT_command | POST DECT Run AT Command
 [**post_device_deregister**](DevicesApi.md#post_device_deregister) | **POST** /devices/{device_id}/deregister | POST deregister device
 [**post_device_end_call**](DevicesApi.md#post_device_end_call) | **POST** /devices/{device_id}/end_call | POST end call
 [**post_device_heartbeat**](DevicesApi.md#post_device_heartbeat) | **POST** /devices/{device_id}/heartbeat | POST Device heartbeat
 [**post_device_make_call**](DevicesApi.md#post_device_make_call) | **POST** /devices/{device_id}/make_call | POST make call
 [**post_device_receive_call**](DevicesApi.md#post_device_receive_call) | **POST** /devices/{device_id}/receive_call | POST receive call
 [**post_device_register**](DevicesApi.md#post_device_register) | **POST** /devices/{device_id}/register | POST register device
@@ -333,15 +334,15 @@
 )
 
 
 # Enter a context with an instance of the API client
 with icotest_voice.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = icotest_voice.DevicesApi(api_client)
-    device_id = 'bc331ccb-5841-44ec-9d32-4f4fe0c3c16c' # str | the unique id of the device
+    device_id = 'device_id_example' # str | the unique id of the device
 
     try:
         # POST APPIUM take screenshot
         api_response = api_instance.post_device_appium_take_screenshot(device_id)
         print("The response of DevicesApi->post_device_appium_take_screenshot:\n")
         pprint(api_response)
     except Exception as e:
@@ -446,14 +447,83 @@
 **200** | Example response |  -  |
 **400** | Device is not a DECT device. |  -  |
 **404** | Device not found. |  -  |
 **500** | Internal Server Error. |  -  |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
+# **post_device_dect_reset**
+> str post_device_dect_reset(device_id)
+
+POST DECT Device Reset
+
+Post a request for a DECT dongle reset (`AT+RSET`). Caution: All DECT devices under the management of the current device's management controller will be reset, even if they are in the middle of an operation (established call)!
+
+### Example
+
+```python
+import time
+import os
+import icotest_voice
+from icotest_voice.rest import ApiException
+from pprint import pprint
+
+# Defining the host is optional and defaults to https://localhost/icotest_voice
+# See configuration.py for a list of all supported configuration parameters.
+configuration = icotest_voice.Configuration(
+    host = "https://localhost/icotest_voice"
+)
+
+
+# Enter a context with an instance of the API client
+with icotest_voice.ApiClient(configuration) as api_client:
+    # Create an instance of the API class
+    api_instance = icotest_voice.DevicesApi(api_client)
+    device_id = 'device_id_example' # str | the unique ID of the DECT device to reset
+
+    try:
+        # POST DECT Device Reset
+        api_response = api_instance.post_device_dect_reset(device_id)
+        print("The response of DevicesApi->post_device_dect_reset:\n")
+        pprint(api_response)
+    except Exception as e:
+        print("Exception when calling DevicesApi->post_device_dect_reset: %s\n" % e)
+```
+
+
+
+### Parameters
+
+Name | Type | Description  | Notes
+------------- | ------------- | ------------- | -------------
+ **device_id** | **str**| the unique ID of the DECT device to reset | 
+
+### Return type
+
+**str**
+
+### Authorization
+
+No authorization required
+
+### HTTP request headers
+
+ - **Content-Type**: Not defined
+ - **Accept**: application/json
+
+### HTTP response details
+| Status code | Description | Response headers |
+|-------------|-------------|------------------|
+**200** | Example response |  -  |
+**400** | Bad Request |  -  |
+**404** | Device Not Found |  -  |
+**500** | Internal Server Error |  -  |
+
+[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
+
 # **post_device_dect_run_at_cmd**
 > str post_device_dect_run_at_cmd(device_id, command)
 
 POST DECT Run AT Command
 
 Post a request to a DECT device to run an arbitrary AT command
```

### Comparing `icotest-voice-1.0.42/docs/GetTestResultFileList200Response.md` & `icotest_voice-1.0.43/docs/GetTestResultFileList200Response.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.42/docs/GetTestResultFileList200ResponseFilesInner.md` & `icotest_voice-1.0.43/docs/GetTestResultFileList200ResponseFilesInner.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.42/docs/HostConfig.md` & `icotest_voice-1.0.43/docs/HostConfig.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.42/docs/PostDeviceRegisterRequest.md` & `icotest_voice-1.0.43/docs/PostDeviceRegisterRequest.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.42/docs/Request.md` & `icotest_voice-1.0.43/docs/Request.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.42/docs/RequestsApi.md` & `icotest_voice-1.0.43/docs/RequestsApi.md`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 )
 
 
 # Enter a context with an instance of the API client
 with icotest_voice.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = icotest_voice.RequestsApi(api_client)
-    device_id = 'device_id_example' # str | the unique ID of the DECT device
+    device_id = 'bc331ccb-5841-44ec-9d32-4f4fe0c3c16d' # str | the unique ID of the DECT device
     commands_type = 'commands_type_example' # str | The type of commands to retrieve: `to_dongle` or `from_dongle`
     commands_num = 56 # int | The number of commands to retrieve
 
     try:
         # DECT Get Last Commands
         api_response = api_instance.dect_get_last_commands(device_id, commands_type, commands_num)
         print("The response of RequestsApi->dect_get_last_commands:\n")
@@ -623,15 +623,15 @@
 )
 
 
 # Enter a context with an instance of the API client
 with icotest_voice.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = icotest_voice.RequestsApi(api_client)
-    request_id = 'bc331ccb-5841-44ec-9d32-4f4fe0c3c16d' # str | the unique id of the request
+    request_id = 'cc331ccb-5841-44ec-9d32-4f4fe0c3c16c' # str | the unique id of the request
 
     try:
         # GET APPIUM retrieve screenshot
         api_response = api_instance.get_appium_retrieve_device_screenshot(request_id)
         print("The response of RequestsApi->get_appium_retrieve_device_screenshot:\n")
         pprint(api_response)
     except Exception as e:
@@ -918,15 +918,15 @@
 )
 
 
 # Enter a context with an instance of the API client
 with icotest_voice.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = icotest_voice.RequestsApi(api_client)
-    controller_id = 'cc331ccb-5841-44ec-9d32-4f4fe0c3c16c' # str | the unique id of a controller
+    controller_id = 'bc331ccb-5841-44ec-9d32-4f4fe0c3c16d' # str | the unique id of a controller
 
     try:
         # GET test result file list
         api_response = api_instance.get_test_result_file_list(controller_id)
         print("The response of RequestsApi->get_test_result_file_list:\n")
         pprint(api_response)
     except Exception as e:
```

### Comparing `icotest-voice-1.0.42/icotest_voice/__init__.py` & `icotest_voice-1.0.43/icotest_voice/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.0.42"
+__version__ = "1.0.43"
 
 # import apis into sdk package
 from icotest_voice.api.controllers_api import ControllersApi
 from icotest_voice.api.devices_api import DevicesApi
 from icotest_voice.api.requests_api import RequestsApi
 
 # import ApiClient
```

### Comparing `icotest-voice-1.0.42/icotest_voice/api/controllers_api.py` & `icotest_voice-1.0.43/icotest_voice/api/controllers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `icotest-voice-1.0.42/icotest_voice/api/devices_api.py` & `icotest_voice-1.0.43/icotest_voice/api/devices_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -1737,14 +1737,284 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
+    def post_device_dect_reset(
+        self,
+        device_id: Annotated[str, Field(min_length=36, strict=True, max_length=36, description="the unique ID of the DECT device to reset")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> str:
+        """POST DECT Device Reset
+
+        Post a request for a DECT dongle reset (`AT+RSET`). Caution: All DECT devices under the management of the current device's management controller will be reset, even if they are in the middle of an operation (established call)!
+
+        :param device_id: the unique ID of the DECT device to reset (required)
+        :type device_id: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._post_device_dect_reset_serialize(
+            device_id=device_id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "str",
+            '400': None,
+            '404': None,
+            '500': None
+            
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def post_device_dect_reset_with_http_info(
+        self,
+        device_id: Annotated[str, Field(min_length=36, strict=True, max_length=36, description="the unique ID of the DECT device to reset")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[str]:
+        """POST DECT Device Reset
+
+        Post a request for a DECT dongle reset (`AT+RSET`). Caution: All DECT devices under the management of the current device's management controller will be reset, even if they are in the middle of an operation (established call)!
+
+        :param device_id: the unique ID of the DECT device to reset (required)
+        :type device_id: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._post_device_dect_reset_serialize(
+            device_id=device_id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "str",
+            '400': None,
+            '404': None,
+            '500': None
+            
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def post_device_dect_reset_without_preload_content(
+        self,
+        device_id: Annotated[str, Field(min_length=36, strict=True, max_length=36, description="the unique ID of the DECT device to reset")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """POST DECT Device Reset
+
+        Post a request for a DECT dongle reset (`AT+RSET`). Caution: All DECT devices under the management of the current device's management controller will be reset, even if they are in the middle of an operation (established call)!
+
+        :param device_id: the unique ID of the DECT device to reset (required)
+        :type device_id: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._post_device_dect_reset_serialize(
+            device_id=device_id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "str",
+            '400': None,
+            '404': None,
+            '500': None
+            
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _post_device_dect_reset_serialize(
+        self,
+        device_id,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> Tuple:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+            
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if device_id is not None:
+            _path_params['device_id'] = device_id
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/devices/{device_id}/DECT_reset',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
     def post_device_dect_run_at_cmd(
         self,
         device_id: Annotated[str, Field(min_length=36, strict=True, max_length=36, description="the unique ID of the DECT device to run the given AT command")],
         command: Annotated[str, Field(min_length=3, strict=True, max_length=256, description="the AT command to run, `RSET` is NOT allowed (do not add \"AT+\", it will be done for you)")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
@@ -2026,15 +2296,15 @@
 
 
 
 
     @validate_call
     def post_device_deregister(
         self,
-        device_id: Annotated[str, Field(strict=True, description="the unique id of the device")],
+        device_id: Annotated[str, Field(min_length=36, strict=True, max_length=36, description="the unique id of the device")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -2099,15 +2369,15 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def post_device_deregister_with_http_info(
         self,
-        device_id: Annotated[str, Field(strict=True, description="the unique id of the device")],
+        device_id: Annotated[str, Field(min_length=36, strict=True, max_length=36, description="the unique id of the device")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -2172,15 +2442,15 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def post_device_deregister_without_preload_content(
         self,
-        device_id: Annotated[str, Field(strict=True, description="the unique id of the device")],
+        device_id: Annotated[str, Field(min_length=36, strict=True, max_length=36, description="the unique id of the device")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -2847,15 +3117,15 @@
 
 
 
 
     @validate_call
     def post_device_make_call(
         self,
-        device_id: Annotated[StrictStr, Field(description="the unique id of the device")],
+        device_id: Annotated[str, Field(min_length=36, strict=True, max_length=36, description="the unique id of the device")],
         phone_number: Annotated[str, Field(strict=True, max_length=40, description="the number to call (add \"i\" before the number for a DECT internal call)")],
         call_duration: Annotated[Optional[Annotated[int, Field(le=65535, strict=True, gt=0)]], Field(description="the duration of the call in seconds (0 is unlimited)")] = None,
         outgoing_recording_file: Annotated[Optional[StrictStr], Field(description="the filename of the recorded call")] = None,
         playback_file: Annotated[Optional[StrictStr], Field(description="the filename of the playback file")] = None,
         playback_loop: Annotated[Optional[StrictBool], Field(description="whether to play the playback file in a loop")] = None,
         wait_time: Annotated[Optional[Annotated[int, Field(strict=True, gt=5)]], Field(description="the duration of the wait time in seconds for the callee to respond")] = None,
         _request_timeout: Union[
@@ -2944,15 +3214,15 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def post_device_make_call_with_http_info(
         self,
-        device_id: Annotated[StrictStr, Field(description="the unique id of the device")],
+        device_id: Annotated[str, Field(min_length=36, strict=True, max_length=36, description="the unique id of the device")],
         phone_number: Annotated[str, Field(strict=True, max_length=40, description="the number to call (add \"i\" before the number for a DECT internal call)")],
         call_duration: Annotated[Optional[Annotated[int, Field(le=65535, strict=True, gt=0)]], Field(description="the duration of the call in seconds (0 is unlimited)")] = None,
         outgoing_recording_file: Annotated[Optional[StrictStr], Field(description="the filename of the recorded call")] = None,
         playback_file: Annotated[Optional[StrictStr], Field(description="the filename of the playback file")] = None,
         playback_loop: Annotated[Optional[StrictBool], Field(description="whether to play the playback file in a loop")] = None,
         wait_time: Annotated[Optional[Annotated[int, Field(strict=True, gt=5)]], Field(description="the duration of the wait time in seconds for the callee to respond")] = None,
         _request_timeout: Union[
@@ -3041,15 +3311,15 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def post_device_make_call_without_preload_content(
         self,
-        device_id: Annotated[StrictStr, Field(description="the unique id of the device")],
+        device_id: Annotated[str, Field(min_length=36, strict=True, max_length=36, description="the unique id of the device")],
         phone_number: Annotated[str, Field(strict=True, max_length=40, description="the number to call (add \"i\" before the number for a DECT internal call)")],
         call_duration: Annotated[Optional[Annotated[int, Field(le=65535, strict=True, gt=0)]], Field(description="the duration of the call in seconds (0 is unlimited)")] = None,
         outgoing_recording_file: Annotated[Optional[StrictStr], Field(description="the filename of the recorded call")] = None,
         playback_file: Annotated[Optional[StrictStr], Field(description="the filename of the playback file")] = None,
         playback_loop: Annotated[Optional[StrictBool], Field(description="whether to play the playback file in a loop")] = None,
         wait_time: Annotated[Optional[Annotated[int, Field(strict=True, gt=5)]], Field(description="the duration of the wait time in seconds for the callee to respond")] = None,
         _request_timeout: Union[
@@ -3225,15 +3495,15 @@
 
 
 
 
     @validate_call
     def post_device_receive_call(
         self,
-        device_id: Annotated[StrictStr, Field(description="the unique id of the device")],
+        device_id: Annotated[str, Field(min_length=36, strict=True, max_length=36, description="the unique id of the device")],
         ring_count: Annotated[Optional[Annotated[int, Field(le=8, strict=True, ge=1)]], Field(description="number of rings before call is picked up")] = None,
         call_duration: Annotated[Optional[Annotated[int, Field(le=65535, strict=True, ge=0)]], Field(description="the duration of the call in seconds (0 is unlimited)")] = None,
         incoming_recording_file: Annotated[Optional[StrictStr], Field(description="the filename of the recorded call")] = None,
         playback_file: Annotated[Optional[StrictStr], Field(description="the filename of the playback file")] = None,
         playback_loop: Annotated[Optional[StrictBool], Field(description="whether to play the playback file in a loop")] = None,
         wait_time: Annotated[Optional[Annotated[int, Field(strict=True, gt=10)]], Field(description="the duration of the wait time in seconds for the caller to make a call")] = None,
         _request_timeout: Union[
@@ -3322,15 +3592,15 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def post_device_receive_call_with_http_info(
         self,
-        device_id: Annotated[StrictStr, Field(description="the unique id of the device")],
+        device_id: Annotated[str, Field(min_length=36, strict=True, max_length=36, description="the unique id of the device")],
         ring_count: Annotated[Optional[Annotated[int, Field(le=8, strict=True, ge=1)]], Field(description="number of rings before call is picked up")] = None,
         call_duration: Annotated[Optional[Annotated[int, Field(le=65535, strict=True, ge=0)]], Field(description="the duration of the call in seconds (0 is unlimited)")] = None,
         incoming_recording_file: Annotated[Optional[StrictStr], Field(description="the filename of the recorded call")] = None,
         playback_file: Annotated[Optional[StrictStr], Field(description="the filename of the playback file")] = None,
         playback_loop: Annotated[Optional[StrictBool], Field(description="whether to play the playback file in a loop")] = None,
         wait_time: Annotated[Optional[Annotated[int, Field(strict=True, gt=10)]], Field(description="the duration of the wait time in seconds for the caller to make a call")] = None,
         _request_timeout: Union[
@@ -3419,15 +3689,15 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def post_device_receive_call_without_preload_content(
         self,
-        device_id: Annotated[StrictStr, Field(description="the unique id of the device")],
+        device_id: Annotated[str, Field(min_length=36, strict=True, max_length=36, description="the unique id of the device")],
         ring_count: Annotated[Optional[Annotated[int, Field(le=8, strict=True, ge=1)]], Field(description="number of rings before call is picked up")] = None,
         call_duration: Annotated[Optional[Annotated[int, Field(le=65535, strict=True, ge=0)]], Field(description="the duration of the call in seconds (0 is unlimited)")] = None,
         incoming_recording_file: Annotated[Optional[StrictStr], Field(description="the filename of the recorded call")] = None,
         playback_file: Annotated[Optional[StrictStr], Field(description="the filename of the playback file")] = None,
         playback_loop: Annotated[Optional[StrictBool], Field(description="whether to play the playback file in a loop")] = None,
         wait_time: Annotated[Optional[Annotated[int, Field(strict=True, gt=10)]], Field(description="the duration of the wait time in seconds for the caller to make a call")] = None,
         _request_timeout: Union[
```

### Comparing `icotest-voice-1.0.42/icotest_voice/api/requests_api.py` & `icotest_voice-1.0.43/icotest_voice/api/requests_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `icotest-voice-1.0.42/icotest_voice/api_client.py` & `icotest_voice-1.0.43/icotest_voice/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -83,15 +83,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.42/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.43/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `icotest-voice-1.0.42/icotest_voice/api_response.py` & `icotest_voice-1.0.43/icotest_voice/api_response.py`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.42/icotest_voice/configuration.py` & `icotest_voice-1.0.43/icotest_voice/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -356,16 +356,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0.42\n"\
-               "SDK Package Version: 1.0.42".\
+               "Version of the API: 1.0.43\n"\
+               "SDK Package Version: 1.0.43".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `icotest-voice-1.0.42/icotest_voice/exceptions.py` & `icotest_voice-1.0.43/icotest_voice/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `icotest-voice-1.0.42/icotest_voice/models/__init__.py` & `icotest_voice-1.0.43/icotest_voice/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `icotest-voice-1.0.42/icotest_voice/models/controller.py` & `icotest_voice-1.0.43/icotest_voice/models/controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -40,16 +40,16 @@
     created: Optional[datetime] = Field(default=None, description="The date the controller was added")
     last_contact: Optional[datetime] = Field(default=None, description="The last contact date time with the controller")
     __properties: ClassVar[List[str]] = ["controller_id", "controller_type", "description", "location", "callback_url", "created", "last_contact"]
 
     @field_validator('controller_id')
     def controller_id_validate_regular_expression(cls, value):
         """Validates the regular expression"""
-        if not re.match(r"[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}", value):
-            raise ValueError(r"must validate the regular expression /[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}/")
+        if not re.match(r"^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$", value):
+            raise ValueError(r"must validate the regular expression /^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$/")
         return value
 
     @field_validator('controller_type')
     def controller_type_validate_enum(cls, value):
         """Validates the enum"""
         if value not in ('dect', 'sip', 'fxo', 'appium'):
             raise ValueError("must be one of enum values ('dect', 'sip', 'fxo', 'appium')")
```

### Comparing `icotest-voice-1.0.42/icotest_voice/models/device.py` & `icotest_voice-1.0.43/icotest_voice/models/device.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -44,30 +44,30 @@
     management_status: Optional[StrictBool] = Field(default=None, description="Management status, if True we run process")
     last_contact: Optional[datetime] = Field(default=None, description="The last contact date time with the controller")
     __properties: ClassVar[List[str]] = ["device_id", "serial_no", "device_type", "url", "created", "updated", "controller_id", "device_status", "callback_port", "management_status", "last_contact"]
 
     @field_validator('device_id')
     def device_id_validate_regular_expression(cls, value):
         """Validates the regular expression"""
-        if not re.match(r"[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}", value):
-            raise ValueError(r"must validate the regular expression /[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}/")
+        if not re.match(r"^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$", value):
+            raise ValueError(r"must validate the regular expression /^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$/")
         return value
 
     @field_validator('device_type')
     def device_type_validate_enum(cls, value):
         """Validates the enum"""
         if value not in ('handset', 'basestation', 'sip', 'fxo', 'appium', 'unknown'):
             raise ValueError("must be one of enum values ('handset', 'basestation', 'sip', 'fxo', 'appium', 'unknown')")
         return value
 
     @field_validator('controller_id')
     def controller_id_validate_regular_expression(cls, value):
         """Validates the regular expression"""
-        if not re.match(r"[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}", value):
-            raise ValueError(r"must validate the regular expression /[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}/")
+        if not re.match(r"^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$", value):
+            raise ValueError(r"must validate the regular expression /^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$/")
         return value
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
```

### Comparing `icotest-voice-1.0.42/icotest_voice/models/get_test_result_file_list200_response.py` & `icotest_voice-1.0.43/icotest_voice/models/get_test_result_file_list200_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `icotest-voice-1.0.42/icotest_voice/models/get_test_result_file_list200_response_files_inner.py` & `icotest_voice-1.0.43/icotest_voice/models/get_test_result_file_list200_response_files_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `icotest-voice-1.0.42/icotest_voice/models/host_config.py` & `icotest_voice-1.0.43/icotest_voice/models/host_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `icotest-voice-1.0.42/icotest_voice/models/post_device_register_request.py` & `icotest_voice-1.0.43/icotest_voice/models/post_device_register_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `icotest-voice-1.0.42/icotest_voice/models/request.py` & `icotest_voice-1.0.43/icotest_voice/models/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -42,50 +42,50 @@
     updated: Optional[datetime] = Field(default=None, description="The date time the request was last updated")
     controller_id: Optional[Annotated[str, Field(min_length=36, strict=True, max_length=36)]] = Field(default=None, description="the unique id of the controller")
     __properties: ClassVar[List[str]] = ["request_id", "device_id", "status", "message", "action", "request_params", "created", "updated", "controller_id"]
 
     @field_validator('request_id')
     def request_id_validate_regular_expression(cls, value):
         """Validates the regular expression"""
-        if not re.match(r"[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}", value):
-            raise ValueError(r"must validate the regular expression /[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}/")
+        if not re.match(r"^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$", value):
+            raise ValueError(r"must validate the regular expression /^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$/")
         return value
 
     @field_validator('device_id')
     def device_id_validate_regular_expression(cls, value):
         """Validates the regular expression"""
         if value is None:
             return value
 
-        if not re.match(r"[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}", value):
-            raise ValueError(r"must validate the regular expression /[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}/")
+        if not re.match(r"^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$", value):
+            raise ValueError(r"must validate the regular expression /^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$/")
         return value
 
     @field_validator('status')
     def status_validate_enum(cls, value):
         """Validates the enum"""
         if value not in ('pending', 'inprogress', 'completed', 'failed', 'suspended'):
             raise ValueError("must be one of enum values ('pending', 'inprogress', 'completed', 'failed', 'suspended')")
         return value
 
     @field_validator('action')
     def action_validate_enum(cls, value):
         """Validates the enum"""
-        if value not in ('register', 'deregister', 'make_call', 'receive_call', 'dect_get_handset_name', 'dect_run_at_cmd', 'dect_get_last_commands', 'scan', 'end_call', 'send_command', 'retrieve_file', 'delete_playback_file', 'upload_playback_file', 'delete_resuts_file', 'delete_results_files_in_range', 'take_screenshot', 'delete_ios_certificates', 'upload_ios_certificates', 'install_ios_webdriveragent'):
-            raise ValueError("must be one of enum values ('register', 'deregister', 'make_call', 'receive_call', 'dect_get_handset_name', 'dect_run_at_cmd', 'dect_get_last_commands', 'scan', 'end_call', 'send_command', 'retrieve_file', 'delete_playback_file', 'upload_playback_file', 'delete_resuts_file', 'delete_results_files_in_range', 'take_screenshot', 'delete_ios_certificates', 'upload_ios_certificates', 'install_ios_webdriveragent')")
+        if value not in ('register', 'deregister', 'make_call', 'receive_call', 'dect_get_handset_name', 'dect_run_at_cmd', 'dect_get_last_commands', 'dect_reset_device', 'scan', 'end_call', 'send_command', 'retrieve_file', 'delete_playback_file', 'upload_playback_file', 'delete_resuts_file', 'delete_results_files_in_range', 'appium_take_screenshot', 'appium_delete_all_screenshots', 'appium_delete_ios_certificates', 'appium_upload_ios_certificates', 'appium_install_ios_webdriveragent'):
+            raise ValueError("must be one of enum values ('register', 'deregister', 'make_call', 'receive_call', 'dect_get_handset_name', 'dect_run_at_cmd', 'dect_get_last_commands', 'dect_reset_device', 'scan', 'end_call', 'send_command', 'retrieve_file', 'delete_playback_file', 'upload_playback_file', 'delete_resuts_file', 'delete_results_files_in_range', 'appium_take_screenshot', 'appium_delete_all_screenshots', 'appium_delete_ios_certificates', 'appium_upload_ios_certificates', 'appium_install_ios_webdriveragent')")
         return value
 
     @field_validator('controller_id')
     def controller_id_validate_regular_expression(cls, value):
         """Validates the regular expression"""
         if value is None:
             return value
 
-        if not re.match(r"[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}", value):
-            raise ValueError(r"must validate the regular expression /[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}/")
+        if not re.match(r"^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$", value):
+            raise ValueError(r"must validate the regular expression /^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$/")
         return value
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
```

### Comparing `icotest-voice-1.0.42/icotest_voice/rest.py` & `icotest_voice-1.0.43/icotest_voice/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `icotest-voice-1.0.42/icotest_voice.egg-info/PKG-INFO` & `icotest_voice-1.0.43/icotest_voice.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,105 +1,79 @@
 Metadata-Version: 2.1
 Name: icotest-voice
-Version: 1.0.42
+Version: 1.0.43
 Summary: Icotest Voice API
-Home-page: 
-Author: Shaun Hirst
 Author-email: Shaun Hirst <shaun.hirst@3adesign.co.uk>, Ivo Shipkaliev <ivo@3adesign.co.uk>
 License: Copyright © 2024 3ADesign Limited
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Keywords: OpenAPI,OpenAPI-Generator,Icotest Voice
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.4
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: python_dateutil>=2.5.3
-Requires-Dist: urllib3<2.1.0,>=1.25.3
-Requires-Dist: pydantic>=2
-Requires-Dist: typing-extensions>=4.7.1
-Requires-Dist: setuptools>=21.0.0
 
 # icotest-voice
 IcoTest Voice API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.42
-- Package version: 1.0.42
+- API version: 1.0.43
+- Package version: 1.0.43
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
 ### pip install
 
-If the python package is hosted on a repository, you can install directly using:
-
 ```sh
-pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
+pip install icotest-voice
 ```
-(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
-
-Then import the package:
-```python
-import icotest_voice
-```
-
-### Setuptools
-
-Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
-
-```sh
-python setup.py install --user
-```
-(or `sudo python setup.py install` to install the package for all users)
 
 Then import the package:
 ```python
 import icotest_voice
 ```
 
 ### Tests
 
 Execute `pytest` to run the tests.
 
 ## Getting Started
 
-Please follow the [installation procedure](#installation--usage) and then run the following:
+Please follow the installation procedure and then run the following:
 
 ```python
 
 import time
 import icotest_voice
 from icotest_voice.rest import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to https://localhost/icotest_voice
 # See configuration.py for a list of all supported configuration parameters.
 configuration = icotest_voice.Configuration(
     host = "https://localhost/icotest_voice"
 )
 
-
-
 # Enter a context with an instance of the API client
 with icotest_voice.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = icotest_voice.ControllersApi(api_client)
-    controller_id = 'ac331ccb-5841-44ec-9d32-4f4fe0c3c16c' # str | the unique id of the controller
+    controller_id = "ac331ccb-5841-44ec-9d32-4f4fe0c3c16c"  # str: the unique ID of the controller
 
     try:
         # DELETE Controller
         api_instance.delete_controller(controller_id)
     except ApiException as e:
         print("Exception when calling ControllersApi->delete_controller: %s\n" % e)
 
@@ -117,14 +91,15 @@
 *ControllersApi* | [**put_controller**](docs/ControllersApi.md#put_controller) | **PUT** /controllers | PUT controller
 *DevicesApi* | [**delete_device**](docs/DevicesApi.md#delete_device) | **DELETE** /devices | DELETE Device
 *DevicesApi* | [**get_device_status**](docs/DevicesApi.md#get_device_status) | **GET** /devices/{device_id}/status | GET device status
 *DevicesApi* | [**get_devices**](docs/DevicesApi.md#get_devices) | **GET** /devices | GET devices
 *DevicesApi* | [**get_host_config**](docs/DevicesApi.md#get_host_config) | **GET** /host/config | Your GET endpoint
 *DevicesApi* | [**post_device_appium_take_screenshot**](docs/DevicesApi.md#post_device_appium_take_screenshot) | **POST** /devices/{device_id}/APPIUM_take_screenshot | POST APPIUM take screenshot
 *DevicesApi* | [**post_device_dect_get_handset_name**](docs/DevicesApi.md#post_device_dect_get_handset_name) | **POST** /devices/{device_id}/DECT_get_handset_name | POST DECT Get Handset Name
+*DevicesApi* | [**post_device_dect_reset**](docs/DevicesApi.md#post_device_dect_reset) | **POST** /devices/{device_id}/DECT_reset | POST DECT Device Reset
 *DevicesApi* | [**post_device_dect_run_at_cmd**](docs/DevicesApi.md#post_device_dect_run_at_cmd) | **POST** /devices/{device_id}/DECT_run_AT_command | POST DECT Run AT Command
 *DevicesApi* | [**post_device_deregister**](docs/DevicesApi.md#post_device_deregister) | **POST** /devices/{device_id}/deregister | POST deregister device
 *DevicesApi* | [**post_device_end_call**](docs/DevicesApi.md#post_device_end_call) | **POST** /devices/{device_id}/end_call | POST end call
 *DevicesApi* | [**post_device_heartbeat**](docs/DevicesApi.md#post_device_heartbeat) | **POST** /devices/{device_id}/heartbeat | POST Device heartbeat
 *DevicesApi* | [**post_device_make_call**](docs/DevicesApi.md#post_device_make_call) | **POST** /devices/{device_id}/make_call | POST make call
 *DevicesApi* | [**post_device_receive_call**](docs/DevicesApi.md#post_device_receive_call) | **POST** /devices/{device_id}/receive_call | POST receive call
 *DevicesApi* | [**post_device_register**](docs/DevicesApi.md#post_device_register) | **POST** /devices/{device_id}/register | POST register device
```

### Comparing `icotest-voice-1.0.42/icotest_voice.egg-info/SOURCES.txt` & `icotest_voice-1.0.43/icotest_voice.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
-setup.py
 docs/Controller.md
 docs/ControllersApi.md
 docs/Device.md
 docs/DevicesApi.md
 docs/GetTestResultFileList200Response.md
 docs/GetTestResultFileList200ResponseFilesInner.md
 docs/HostConfig.md
@@ -20,15 +18,14 @@
 icotest_voice/configuration.py
 icotest_voice/exceptions.py
 icotest_voice/py.typed
 icotest_voice/rest.py
 icotest_voice.egg-info/PKG-INFO
 icotest_voice.egg-info/SOURCES.txt
 icotest_voice.egg-info/dependency_links.txt
-icotest_voice.egg-info/requires.txt
 icotest_voice.egg-info/top_level.txt
 icotest_voice/api/__init__.py
 icotest_voice/api/controllers_api.py
 icotest_voice/api/devices_api.py
 icotest_voice/api/requests_api.py
 icotest_voice/models/__init__.py
 icotest_voice/models/controller.py
```

### Comparing `icotest-voice-1.0.42/pyproject.toml` & `icotest_voice-1.0.43/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "icotest-voice"
-version = "1.0.42"
+version = "1.0.43"
 description = "Icotest Voice API"
 readme = "README.md"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Icotest Voice"]
 authors = [
     { name = "Shaun Hirst", email = "shaun.hirst@3adesign.co.uk" },
     { name = "Ivo Shipkaliev", email = "ivo@3adesign.co.uk" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
-dependencies = [
-    "python_dateutil >= 2.5.3",
-    "urllib3 >= 1.25.3, < 2.1.0",
-    "pydantic >= 2",
-    "typing-extensions >= 4.7.1",
-    "setuptools >= 21.0.0",
-]
-requires-python = ">=3.4"
+requires-python = ">=3.7"
```

### Comparing `icotest-voice-1.0.42/test/test_controller.py` & `icotest_voice-1.0.43/test/test_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `icotest-voice-1.0.42/test/test_controllers_api.py` & `icotest_voice-1.0.43/test/test_controllers_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `icotest-voice-1.0.42/test/test_device.py` & `icotest_voice-1.0.43/test/test_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `icotest-voice-1.0.42/test/test_devices_api.py` & `icotest_voice-1.0.43/test/test_devices_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -65,14 +65,21 @@
     def test_post_device_dect_get_handset_name(self) -> None:
         """Test case for post_device_dect_get_handset_name
 
         POST DECT Get Handset Name
         """
         pass
 
+    def test_post_device_dect_reset(self) -> None:
+        """Test case for post_device_dect_reset
+
+        POST DECT Device Reset
+        """
+        pass
+
     def test_post_device_dect_run_at_cmd(self) -> None:
         """Test case for post_device_dect_run_at_cmd
 
         POST DECT Run AT Command
         """
         pass
```

### Comparing `icotest-voice-1.0.42/test/test_get_test_result_file_list200_response.py` & `icotest_voice-1.0.43/test/test_get_test_result_file_list200_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `icotest-voice-1.0.42/test/test_get_test_result_file_list200_response_files_inner.py` & `icotest_voice-1.0.43/test/test_get_test_result_file_list200_response_files_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `icotest-voice-1.0.42/test/test_host_config.py` & `icotest_voice-1.0.43/test/test_host_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `icotest-voice-1.0.42/test/test_post_device_register_request.py` & `icotest_voice-1.0.43/test/test_post_device_register_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `icotest-voice-1.0.42/test/test_request.py` & `icotest_voice-1.0.43/test/test_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `icotest-voice-1.0.42/test/test_requests_api.py` & `icotest_voice-1.0.43/test/test_requests_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API
 
-    The version of the OpenAPI document: 1.0.42
+    The version of the OpenAPI document: 1.0.43
     Contact: shaun.hirst@3adesign.co.uk
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

