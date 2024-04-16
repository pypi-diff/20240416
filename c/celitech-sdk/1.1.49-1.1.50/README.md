# Comparing `tmp/celitech-sdk-1.1.49.tar.gz` & `tmp/celitech_sdk-1.1.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celitech-sdk-1.1.49.tar", last modified: Wed Apr 10 15:57:08 2024, max compression
+gzip compressed data, was "celitech_sdk-1.1.50.tar", last modified: Tue Apr 16 08:30:53 2024, max compression
```

## Comparing `celitech-sdk-1.1.49.tar` & `celitech_sdk-1.1.50.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:57:08.536275 celitech-sdk-1.1.49/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15268 2024-04-10 15:57:08.532275 celitech-sdk-1.1.49/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14887 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 15:57:08.536275 celitech-sdk-1.1.49/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:57:08.520275 celitech-sdk-1.1.49/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:57:08.524275 celitech-sdk-1.1.49/src/celitech/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:57:08.524275 celitech-sdk-1.1.49/src/celitech/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/hooks/hook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:57:08.528275 celitech-sdk-1.1.49/src/celitech/models/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/models/create_purchase_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/models/create_purchase_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/models/edit_purchase_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/models/edit_purchase_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/models/get_esim_device_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/models/get_esim_history_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/models/get_esim_mac_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/models/get_esim_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/models/get_purchase_consumption_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/models/list_destinations_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/models/list_packages_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/models/list_purchases_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/models/top_up_esim_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/models/top_up_esim_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:57:08.528275 celitech-sdk-1.1.49/src/celitech/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/models/utils/cast_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/models/utils/json_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:57:08.528275 celitech-sdk-1.1.49/src/celitech/net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:57:08.528275 celitech-sdk-1.1.49/src/celitech/net/environment/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/net/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/net/environment/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:57:08.528275 celitech-sdk-1.1.49/src/celitech/net/headers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/net/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/net/headers/base_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:57:08.528275 celitech-sdk-1.1.49/src/celitech/net/request_chain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/net/request_chain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:57:08.528275 celitech-sdk-1.1.49/src/celitech/net/request_chain/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/net/request_chain/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/net/request_chain/handlers/base_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/net/request_chain/handlers/hook_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/net/request_chain/handlers/http_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/net/request_chain/handlers/retry_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/net/request_chain/request_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:57:08.532275 celitech-sdk-1.1.49/src/celitech/net/transport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/net/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/net/transport/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/net/transport/request_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/net/transport/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/net/transport/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/net/transport/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:57:08.532275 celitech-sdk-1.1.49/src/celitech/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/services/destinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/services/e_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/services/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/services/purchases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:57:08.532275 celitech-sdk-1.1.49/src/celitech/services/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/services/utils/base_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/services/utils/default_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-04-10 15:56:53.000000 celitech-sdk-1.1.49/src/celitech/services/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:57:08.532275 celitech-sdk-1.1.49/src/celitech_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15268 2024-04-10 15:57:08.000000 celitech-sdk-1.1.49/src/celitech_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-10 15:57:08.000000 celitech-sdk-1.1.49/src/celitech_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 15:57:08.000000 celitech-sdk-1.1.49/src/celitech_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 15:57:08.000000 celitech-sdk-1.1.49/src/celitech_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 15:57:08.000000 celitech-sdk-1.1.49/src/celitech_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:53.258398 celitech_sdk-1.1.50/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15044 2024-04-16 08:30:53.258398 celitech_sdk-1.1.50/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 08:30:53.258398 celitech_sdk-1.1.50/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:53.246399 celitech_sdk-1.1.50/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:53.246399 celitech_sdk-1.1.50/src/celitech/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:53.246399 celitech_sdk-1.1.50/src/celitech/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/hooks/hook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:53.250398 celitech_sdk-1.1.50/src/celitech/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/models/create_purchase_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/models/create_purchase_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/models/edit_purchase_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/models/edit_purchase_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/models/get_esim_device_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/models/get_esim_history_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/models/get_esim_mac_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/models/get_esim_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/models/get_purchase_consumption_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/models/list_destinations_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/models/list_packages_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/models/list_purchases_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/models/top_up_esim_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/models/top_up_esim_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:53.250398 celitech_sdk-1.1.50/src/celitech/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/models/utils/cast_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/models/utils/json_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:53.254398 celitech_sdk-1.1.50/src/celitech/net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:53.254398 celitech_sdk-1.1.50/src/celitech/net/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/net/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/net/environment/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:53.254398 celitech_sdk-1.1.50/src/celitech/net/headers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/net/headers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/net/headers/base_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:53.254398 celitech_sdk-1.1.50/src/celitech/net/request_chain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/net/request_chain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:53.254398 celitech_sdk-1.1.50/src/celitech/net/request_chain/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/net/request_chain/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/net/request_chain/handlers/base_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/net/request_chain/handlers/hook_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/net/request_chain/handlers/http_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/net/request_chain/handlers/retry_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/net/request_chain/request_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:53.254398 celitech_sdk-1.1.50/src/celitech/net/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/net/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/net/transport/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/net/transport/request_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/net/transport/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/net/transport/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/net/transport/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:53.258398 celitech_sdk-1.1.50/src/celitech/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/services/destinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/services/e_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/services/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/services/purchases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:53.258398 celitech_sdk-1.1.50/src/celitech/services/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/services/utils/base_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/services/utils/default_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-04-16 08:30:41.000000 celitech_sdk-1.1.50/src/celitech/services/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:53.258398 celitech_sdk-1.1.50/src/celitech_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15044 2024-04-16 08:30:53.000000 celitech_sdk-1.1.50/src/celitech_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-16 08:30:53.000000 celitech_sdk-1.1.50/src/celitech_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:30:53.000000 celitech_sdk-1.1.50/src/celitech_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-16 08:30:53.000000 celitech_sdk-1.1.50/src/celitech_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 08:30:53.000000 celitech_sdk-1.1.50/src/celitech_sdk.egg-info/top_level.txt
```

### Comparing `celitech-sdk-1.1.49/LICENSE` & `celitech_sdk-1.1.50/LICENSE`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/PKG-INFO` & `celitech_sdk-1.1.50/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,13 @@
-Metadata-Version: 2.1
-Name: celitech-sdk
-Version: 1.1.49
-Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.31.0
-
-# Celitech Python SDK 1.1.49
+# Celitech Python SDK 1.1.50
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.49
+- SDK version: 1.1.50
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
@@ -129,18 +119,15 @@
 )
 
 result = sdk.packages.list_packages(
     destination="FRA",
     start_date="2023-11-01",
     end_date="2023-11-20",
     after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
-    limit=20,
-    start_time=8,
-    end_time=2,
-    duration=8.44
+    limit=20
 )
 
 print(result)
 ```
 
 ### PurchasesService
 
@@ -186,17 +173,15 @@
 )
 
 result = sdk.purchases.list_purchases(
     iccid="1111222233334444555",
     after_date="2023-11-01",
     before_date="2023-11-20",
     after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
-    limit=20,
-    after=2.38,
-    before=3.34
+    limit=20
 )
 
 print(result)
 ```
 
 #### **create_purchase**
 
@@ -226,17 +211,15 @@
 
 request_body = CreatePurchaseRequest(**{
     "destination": "FRA",
     "data_limit_in_gb": 1,
     "start_date": "2023-11-01",
     "end_date": "2023-11-20",
     "email": "example@domain.com",
-    "network_brand": "CELITECH",
-    "start_time": 2.37,
-    "end_time": 8.12
+    "network_brand": "CELITECH"
 })
 
 result = sdk.purchases.create_purchase(request_body=request_body)
 
 print(result)
 ```
 
@@ -267,17 +250,15 @@
 )
 
 request_body = TopUpEsimRequest(**{
     "iccid": "1111222233334444555",
     "data_limit_in_gb": 1,
     "start_date": "2023-11-01",
     "end_date": "2023-11-20",
-    "email": "example@domain.com",
-    "start_time": 8.12,
-    "end_time": 4.35
+    "email": "example@domain.com"
 })
 
 result = sdk.purchases.top_up_esim(request_body=request_body)
 
 print(result)
 ```
 
@@ -306,17 +287,15 @@
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
 request_body = EditPurchaseRequest(**{
     "purchase_id": "ae471106-c8b4-42cf-b83a-b061291f2922",
     "start_date": "2023-11-01",
-    "end_date": "2023-11-20",
-    "start_time": 8.76,
-    "end_time": 4.68
+    "end_date": "2023-11-20"
 })
 
 result = sdk.purchases.edit_purchase(request_body=request_body)
 
 print(result)
 ```
```

### Comparing `celitech-sdk-1.1.49/README.md` & `celitech_sdk-1.1.50/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,23 @@
-# Celitech Python SDK 1.1.49
+Metadata-Version: 2.1
+Name: celitech-sdk
+Version: 1.1.50
+Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
+License: MIT
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.31.0
+
+# Celitech Python SDK 1.1.50
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.49
+- SDK version: 1.1.50
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
@@ -119,18 +129,15 @@
 )
 
 result = sdk.packages.list_packages(
     destination="FRA",
     start_date="2023-11-01",
     end_date="2023-11-20",
     after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
-    limit=20,
-    start_time=8,
-    end_time=2,
-    duration=8.44
+    limit=20
 )
 
 print(result)
 ```
 
 ### PurchasesService
 
@@ -176,17 +183,15 @@
 )
 
 result = sdk.purchases.list_purchases(
     iccid="1111222233334444555",
     after_date="2023-11-01",
     before_date="2023-11-20",
     after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
-    limit=20,
-    after=2.38,
-    before=3.34
+    limit=20
 )
 
 print(result)
 ```
 
 #### **create_purchase**
 
@@ -216,17 +221,15 @@
 
 request_body = CreatePurchaseRequest(**{
     "destination": "FRA",
     "data_limit_in_gb": 1,
     "start_date": "2023-11-01",
     "end_date": "2023-11-20",
     "email": "example@domain.com",
-    "network_brand": "CELITECH",
-    "start_time": 2.37,
-    "end_time": 8.12
+    "network_brand": "CELITECH"
 })
 
 result = sdk.purchases.create_purchase(request_body=request_body)
 
 print(result)
 ```
 
@@ -257,17 +260,15 @@
 )
 
 request_body = TopUpEsimRequest(**{
     "iccid": "1111222233334444555",
     "data_limit_in_gb": 1,
     "start_date": "2023-11-01",
     "end_date": "2023-11-20",
-    "email": "example@domain.com",
-    "start_time": 8.12,
-    "end_time": 4.35
+    "email": "example@domain.com"
 })
 
 result = sdk.purchases.top_up_esim(request_body=request_body)
 
 print(result)
 ```
 
@@ -296,17 +297,15 @@
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
 request_body = EditPurchaseRequest(**{
     "purchase_id": "ae471106-c8b4-42cf-b83a-b061291f2922",
     "start_date": "2023-11-01",
-    "end_date": "2023-11-20",
-    "start_time": 8.76,
-    "end_time": 4.68
+    "end_date": "2023-11-20"
 })
 
 result = sdk.purchases.edit_purchase(request_body=request_body)
 
 print(result)
 ```
```

### Comparing `celitech-sdk-1.1.49/src/celitech/hooks/hook.py` & `celitech_sdk-1.1.50/src/celitech/hooks/hook.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-import os
-import time
 import requests
+import os
+from typing import Dict
+import datetime
+
+CURRENT_TOKEN = ""
+CURRENT_EXPIRY = -1
 
 
 class Request:
     def __init__(self, method, url, headers, body=""):
         self.method = method
         self.url = url
         self.headers = headers
@@ -24,70 +28,53 @@
         return "Response(status={}, headers={}, body={})".format(
             self.status, self.headers, self.body
         )
 
 
 class CustomHook:
 
-    def __init__(self):
-        self.CURRENT_TOKEN = None
-        self.CURRENT_EXPIRY = 0
-
-    def before_request(self, request: Request):
+    async def before_request(self, request: Request):
         if request.url.endswith("/oauth/token"):
             return
-
-        # Get the client_id and client_secret from environment variables
-        client_id = os.getenv("CLIENT_ID", "")
-        client_secret = os.getenv("CLIENT_SECRET", "")
+        client_id = os.environ.get("CLIENT_ID", "")
+        client_secret = os.environ.get("CLIENT_SECRET", "")
 
         if not client_id or not client_secret:
             print("Missing CLIENT_ID and/or CLIENT_SECRET environment variables")
             return
-        else:
-            # Check if CURRENT_TOKEN is missing or CURRENT_EXPIRY is in the past
-            if not self.CURRENT_TOKEN or self.CURRENT_EXPIRY < time.time() * 1000:
-                # Assuming Celitech class and its methods are defined appropriately
-                sdk = Celitech(environment=Environment.TOKEN_SERVER)
-
-                # Prepare the request payload for fetching a fresh OAuth token
-                input_data = {
-                    "client_id": client_id,
-                    "client_secret": client_secret,
-                    "grant_type": "client_credentials",
-                }
-
-                # Fetch a fresh OAuth token
-                token_response = self.do_post(request, input_data, "/oauth2/token")
-                expires_in = token_response.get("expires_in")
-                access_token = token_response.get("access_token")
-
-                if not expires_in or not access_token:
-                    print("There is an issue with getting the OAuth token")
-                    return
-
-                self.CURRENT_EXPIRY = time.time() * 1000 + expires_in * 1000
-                self.CURRENT_TOKEN = access_token
-
-            # Set the Bearer token in the request header
-            authorization = f"Bearer {self.CURRENT_TOKEN}"
-            request.headers.update({"Authorization": authorization})
 
-    def do_post(self, request: Request, input_data: dict, url_endpoint: str):
-        full_url = "https://auth.celitech.net/oauth2/token"
+        if not CURRENT_TOKEN or CURRENT_EXPIRY < datetime.datetime.now():
+            input_data = {
+                "client_id": client_id,
+                "client_secret": client_secret,
+                "grant_type": "client_credentials",
+            }
+
+            token_response = await self.doPost(request, input_data, "/oauth2/token")
+            expires_in = token_response["data"].get("expires_in")
+            access_token = token_response["data"].get("access_token")
+
+            if not expires_in or not access_token:
+                print("There is an issue with getting the oauth token")
+                return
+
+            CURRENT_EXPIRY = datetime.datetime.now() + expires_in * 1000
+            CURRENT_TOKEN = access_token
+
+        authorization = f"Bearer {CURRENT_TOKEN}"
+        request.headers.update({"Authorization": authorization})
+
+    def doPost(self, input_data: Dict) -> Dict:
+        full_url = f"https://auth.celitech.net/oauth2/token"
+        headers = {"Content-type": "application/x-www-form-urlencoded"}
 
         try:
-            response = requests.post(
-                full_url,
-                data=input_data,
-                headers={"Content-type": "application/x-www-form-urlencoded"},
-                verify=True,
-            )
-
-            return response.json() if response.ok else None
+            resp = requests.post(full_url, data=input_data, headers=headers)
+            resp.raise_for_status()
+            return resp.json()
         except Exception as error:
             print("Error in posting the request:", error)
             return None
 
     def after_response(self, request: Request, response: Response):
         pass
```

### Comparing `celitech-sdk-1.1.49/src/celitech/models/__init__.py` & `celitech_sdk-1.1.50/src/celitech/models/__init__.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/models/base.py` & `celitech_sdk-1.1.50/src/celitech/models/base.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/models/create_purchase_ok_response.py` & `celitech_sdk-1.1.50/src/celitech/models/create_purchase_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/models/create_purchase_request.py` & `celitech_sdk-1.1.50/src/celitech/models/create_purchase_request.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/models/edit_purchase_ok_response.py` & `celitech_sdk-1.1.50/src/celitech/models/edit_purchase_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/models/edit_purchase_request.py` & `celitech_sdk-1.1.50/src/celitech/models/edit_purchase_request.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/models/get_esim_device_ok_response.py` & `celitech_sdk-1.1.50/src/celitech/models/get_esim_device_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/models/get_esim_history_ok_response.py` & `celitech_sdk-1.1.50/src/celitech/models/get_esim_history_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/models/get_esim_mac_ok_response.py` & `celitech_sdk-1.1.50/src/celitech/models/get_esim_mac_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/models/get_esim_ok_response.py` & `celitech_sdk-1.1.50/src/celitech/models/get_esim_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/models/get_purchase_consumption_ok_response.py` & `celitech_sdk-1.1.50/src/celitech/models/get_purchase_consumption_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/models/list_destinations_ok_response.py` & `celitech_sdk-1.1.50/src/celitech/models/list_destinations_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/models/list_packages_ok_response.py` & `celitech_sdk-1.1.50/src/celitech/models/list_packages_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/models/list_purchases_ok_response.py` & `celitech_sdk-1.1.50/src/celitech/models/list_purchases_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/models/top_up_esim_ok_response.py` & `celitech_sdk-1.1.50/src/celitech/models/top_up_esim_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/models/top_up_esim_request.py` & `celitech_sdk-1.1.50/src/celitech/models/top_up_esim_request.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/models/utils/cast_models.py` & `celitech_sdk-1.1.50/src/celitech/models/utils/cast_models.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/models/utils/json_map.py` & `celitech_sdk-1.1.50/src/celitech/models/utils/json_map.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/net/request_chain/handlers/base_handler.py` & `celitech_sdk-1.1.50/src/celitech/net/request_chain/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/net/request_chain/handlers/hook_handler.py` & `celitech_sdk-1.1.50/src/celitech/net/request_chain/handlers/hook_handler.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/net/request_chain/handlers/http_handler.py` & `celitech_sdk-1.1.50/src/celitech/net/request_chain/handlers/http_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,18 +41,18 @@
                 request.url,
                 headers=request.headers,
                 timeout=self._timeout_in_seconds,
                 **request_args,
             )
             response = Response(result)
 
-            if result.status_code >= 400:
+            if response.status >= 400:
                 return None, RequestError(
-                    message=f"{result.status_code} error in request to: {request.url}",
-                    status_code=result.status_code,
+                    message=f"{response.status} error in request to: {request.url}",
+                    status=response.status,
                     response=response,
                 )
 
             return response, None
         except Timeout:
             return None, RequestError("Request timed out")
```

### Comparing `celitech-sdk-1.1.49/src/celitech/net/request_chain/handlers/retry_handler.py` & `celitech_sdk-1.1.50/src/celitech/net/request_chain/handlers/retry_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,8 +58,8 @@
         :param Optional[Response] response: The response from the previous handler.
         :param Optional[RequestError] error: The error from the previous handler.
         :return: True if the request should be retried, False otherwise.
         :rtype: bool
         """
         if not error:
             return False
-        return error.status_code == 408 or error.status_code >= 500
+        return error.status == 408 or error.status >= 500
```

### Comparing `celitech-sdk-1.1.49/src/celitech/net/request_chain/request_chain.py` & `celitech_sdk-1.1.50/src/celitech/net/request_chain/request_chain.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/net/transport/request.py` & `celitech_sdk-1.1.50/src/celitech/net/transport/request.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/net/transport/request_error.py` & `celitech_sdk-1.1.50/src/celitech/net/transport/request_error.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,51 +3,51 @@
 
 
 class RequestError(IOError):
     """
     Class representing a Request Error.
 
     :ivar bool is_http_error: Indicates if the error is an HTTP error.
-    :ivar int status_code: The status code of the HTTP error.
+    :ivar int status: The status code of the HTTP error.
     :ivar Optional[Response] response: The response associated with the error.
     """
 
     def __init__(
         self,
         message: str,
-        status_code: Optional[int] = None,
+        status: Optional[int] = None,
         response: Optional[Response] = None,
         stack: Optional["RequestError"] = None,
     ):
         """
         Initialize a new instance of RequestError.
 
         :param str message: The error message.
-        :param Optional[int] status_code: The status code of the HTTP error.
+        :param Optional[int] status: The status code of the HTTP error.
         :param Optional[Response] response: The response associated with the error.
         """
         super().__init__(message)
         self.response = response
         self.stack = stack
 
-        if status_code is not None:
-            self.status_code = status_code
+        if status is not None:
+            self.status = status
             self.is_http_error = True
         else:
-            self.status_code = -1
+            self.status = -1
             self.is_http_error = False
 
     def __str__(self):
         """
         Get the string representation of the error.
 
         :return: The string representation of the error.
         :rtype: str
         """
         error_stack = []
         current_error = self
         while current_error is not None:
             error_stack.append(
-                f"Error: {super().__str__()}, Status Code: {current_error.status_code}"
+                f"Error: {super().__str__()}, Status Code: {current_error.status}"
             )
             current_error = current_error.stack
         return "\n".join(error_stack)
```

### Comparing `celitech-sdk-1.1.49/src/celitech/net/transport/response.py` & `celitech_sdk-1.1.50/src/celitech/net/transport/response.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,37 +2,39 @@
 from urllib.parse import parse_qs
 
 
 class Response:
     """
     A simple HTTP response wrapper class using the requests library.
 
-    :ivar int status_code: The status code of the HTTP response.
+    :ivar int status: The status code of the HTTP response.
     :ivar dict headers: The headers of the HTTP response.
     :ivar str body: The body of the HTTP response.
     """
 
     def __init__(self, response: RequestsResponse):
         """
         Initializes a Response object.
 
         :param RequestsResponse response: The requests.Response object.
         """
-        self.status_code = response.status_code
+        self.status = response.status_code
         self.headers = response.headers
         self.body = self._get_response_body(response)
 
     def __str__(self) -> str:
         """
         Return a string representation of the Response object.
 
         :return: A string representation of the Response object.
         :rtype: str
         """
-        return f"Response(status_code={self.status_code}, headers={self.headers}, body={self.body})"
+        return (
+            f"Response(status={self.status}, headers={self.headers}, body={self.body})"
+        )
 
     def _get_response_body(self, response: RequestsResponse) -> str:
         """
         Extracts the response body from a given HTTP response.
 
         This method attempts to parse the response body based on its content type.
         If the content type is JSON, it tries to parse the body as JSON.
```

### Comparing `celitech-sdk-1.1.49/src/celitech/net/transport/serializer.py` & `celitech_sdk-1.1.50/src/celitech/net/transport/serializer.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/net/transport/utils.py` & `celitech_sdk-1.1.50/src/celitech/net/transport/utils.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/sdk.py` & `celitech_sdk-1.1.50/src/celitech/sdk.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/services/destinations.py` & `celitech_sdk-1.1.50/src/celitech/services/destinations.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/services/e_sim.py` & `celitech_sdk-1.1.50/src/celitech/services/e_sim.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/services/packages.py` & `celitech_sdk-1.1.50/src/celitech/services/packages.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/services/purchases.py` & `celitech_sdk-1.1.50/src/celitech/services/purchases.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/services/utils/base_service.py` & `celitech_sdk-1.1.50/src/celitech/services/utils/base_service.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/services/utils/default_headers.py` & `celitech_sdk-1.1.50/src/celitech/services/utils/default_headers.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech/services/utils/validator.py` & `celitech_sdk-1.1.50/src/celitech/services/utils/validator.py`

 * *Files identical despite different names*

### Comparing `celitech-sdk-1.1.49/src/celitech_sdk.egg-info/PKG-INFO` & `celitech_sdk-1.1.50/src/celitech_sdk.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: celitech-sdk
-Version: 1.1.49
+Version: 1.1.50
 Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 
-# Celitech Python SDK 1.1.49
+# Celitech Python SDK 1.1.50
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.49
+- SDK version: 1.1.50
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
@@ -129,18 +129,15 @@
 )
 
 result = sdk.packages.list_packages(
     destination="FRA",
     start_date="2023-11-01",
     end_date="2023-11-20",
     after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
-    limit=20,
-    start_time=8,
-    end_time=2,
-    duration=8.44
+    limit=20
 )
 
 print(result)
 ```
 
 ### PurchasesService
 
@@ -186,17 +183,15 @@
 )
 
 result = sdk.purchases.list_purchases(
     iccid="1111222233334444555",
     after_date="2023-11-01",
     before_date="2023-11-20",
     after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
-    limit=20,
-    after=2.38,
-    before=3.34
+    limit=20
 )
 
 print(result)
 ```
 
 #### **create_purchase**
 
@@ -226,17 +221,15 @@
 
 request_body = CreatePurchaseRequest(**{
     "destination": "FRA",
     "data_limit_in_gb": 1,
     "start_date": "2023-11-01",
     "end_date": "2023-11-20",
     "email": "example@domain.com",
-    "network_brand": "CELITECH",
-    "start_time": 2.37,
-    "end_time": 8.12
+    "network_brand": "CELITECH"
 })
 
 result = sdk.purchases.create_purchase(request_body=request_body)
 
 print(result)
 ```
 
@@ -267,17 +260,15 @@
 )
 
 request_body = TopUpEsimRequest(**{
     "iccid": "1111222233334444555",
     "data_limit_in_gb": 1,
     "start_date": "2023-11-01",
     "end_date": "2023-11-20",
-    "email": "example@domain.com",
-    "start_time": 8.12,
-    "end_time": 4.35
+    "email": "example@domain.com"
 })
 
 result = sdk.purchases.top_up_esim(request_body=request_body)
 
 print(result)
 ```
 
@@ -306,17 +297,15 @@
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
 request_body = EditPurchaseRequest(**{
     "purchase_id": "ae471106-c8b4-42cf-b83a-b061291f2922",
     "start_date": "2023-11-01",
-    "end_date": "2023-11-20",
-    "start_time": 8.76,
-    "end_time": 4.68
+    "end_date": "2023-11-20"
 })
 
 result = sdk.purchases.edit_purchase(request_body=request_body)
 
 print(result)
 ```
```

### Comparing `celitech-sdk-1.1.49/src/celitech_sdk.egg-info/SOURCES.txt` & `celitech_sdk-1.1.50/src/celitech_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

