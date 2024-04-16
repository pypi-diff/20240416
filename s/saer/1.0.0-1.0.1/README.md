# Comparing `tmp/saer-1.0.0.tar.gz` & `tmp/saer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saer-1.0.0.tar", last modified: Tue Apr 16 15:11:30 2024, max compression
+gzip compressed data, was "saer-1.0.1.tar", last modified: Tue Apr 16 15:53:31 2024, max compression
```

## Comparing `saer-1.0.0.tar` & `saer-1.0.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:11:30.490819 saer-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-16 15:11:18.000000 saer-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15025 2024-04-16 15:11:30.490819 saer-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14653 2024-04-16 15:11:18.000000 saer-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-16 15:11:18.000000 saer-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:11:30.490819 saer-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:11:30.482818 saer-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:11:30.482818 saer-1.0.0/src/celitech/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:11:30.482818 saer-1.0.0/src/celitech/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/hooks/hook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:11:30.486818 saer-1.0.0/src/celitech/models/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/models/create_purchase_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/models/create_purchase_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/models/edit_purchase_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/models/edit_purchase_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/models/get_esim_device_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/models/get_esim_history_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/models/get_esim_mac_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/models/get_esim_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/models/get_purchase_consumption_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/models/list_destinations_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/models/list_packages_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/models/list_purchases_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/models/top_up_esim_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/models/top_up_esim_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:11:30.486818 saer-1.0.0/src/celitech/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/models/utils/cast_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/models/utils/json_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:11:30.486818 saer-1.0.0/src/celitech/net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:11:30.486818 saer-1.0.0/src/celitech/net/environment/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/net/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/net/environment/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:11:30.486818 saer-1.0.0/src/celitech/net/headers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/net/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/net/headers/base_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:11:30.486818 saer-1.0.0/src/celitech/net/request_chain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/net/request_chain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:11:30.486818 saer-1.0.0/src/celitech/net/request_chain/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/net/request_chain/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/net/request_chain/handlers/base_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/net/request_chain/handlers/hook_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/net/request_chain/handlers/http_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/net/request_chain/handlers/retry_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/net/request_chain/request_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:11:30.486818 saer-1.0.0/src/celitech/net/transport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/net/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/net/transport/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/net/transport/request_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/net/transport/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/net/transport/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/net/transport/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:11:30.490819 saer-1.0.0/src/celitech/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/services/destinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/services/e_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/services/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/services/purchases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:11:30.490819 saer-1.0.0/src/celitech/services/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/services/utils/base_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/services/utils/default_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-04-16 15:11:18.000000 saer-1.0.0/src/celitech/services/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:11:30.490819 saer-1.0.0/src/saer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15025 2024-04-16 15:11:30.000000 saer-1.0.0/src/saer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-16 15:11:30.000000 saer-1.0.0/src/saer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:11:30.000000 saer-1.0.0/src/saer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-16 15:11:30.000000 saer-1.0.0/src/saer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 15:11:30.000000 saer-1.0.0/src/saer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:53:31.445013 saer-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-16 15:53:18.000000 saer-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15025 2024-04-16 15:53:31.445013 saer-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14653 2024-04-16 15:53:18.000000 saer-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-16 15:53:18.000000 saer-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:53:31.445013 saer-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:53:31.437013 saer-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:53:31.437013 saer-1.0.1/src/celitech/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:53:31.437013 saer-1.0.1/src/celitech/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/hooks/hook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:53:31.441013 saer-1.0.1/src/celitech/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/models/create_purchase_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/models/create_purchase_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/models/edit_purchase_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/models/edit_purchase_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/models/get_esim_device_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/models/get_esim_history_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/models/get_esim_mac_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/models/get_esim_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/models/get_purchase_consumption_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/models/list_destinations_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/models/list_packages_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/models/list_purchases_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/models/top_up_esim_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/models/top_up_esim_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:53:31.441013 saer-1.0.1/src/celitech/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/models/utils/cast_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/models/utils/json_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:53:31.441013 saer-1.0.1/src/celitech/net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:53:31.441013 saer-1.0.1/src/celitech/net/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/net/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/net/environment/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:53:31.441013 saer-1.0.1/src/celitech/net/headers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/net/headers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/net/headers/base_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:53:31.441013 saer-1.0.1/src/celitech/net/request_chain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/net/request_chain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:53:31.441013 saer-1.0.1/src/celitech/net/request_chain/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/net/request_chain/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/net/request_chain/handlers/base_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/net/request_chain/handlers/hook_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/net/request_chain/handlers/http_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/net/request_chain/handlers/retry_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/net/request_chain/request_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:53:31.441013 saer-1.0.1/src/celitech/net/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/net/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/net/transport/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/net/transport/request_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/net/transport/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/net/transport/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/net/transport/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:53:31.445013 saer-1.0.1/src/celitech/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/services/destinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/services/e_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/services/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/services/purchases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:53:31.445013 saer-1.0.1/src/celitech/services/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/services/utils/base_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/services/utils/default_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-04-16 15:53:18.000000 saer-1.0.1/src/celitech/services/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:53:31.445013 saer-1.0.1/src/saer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15025 2024-04-16 15:53:31.000000 saer-1.0.1/src/saer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-16 15:53:31.000000 saer-1.0.1/src/saer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:53:31.000000 saer-1.0.1/src/saer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-16 15:53:31.000000 saer-1.0.1/src/saer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 15:53:31.000000 saer-1.0.1/src/saer.egg-info/top_level.txt
```

### Comparing `saer-1.0.0/LICENSE` & `saer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/PKG-INFO` & `saer-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: saer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 
-# Celitech Python SDK 1.0.0
+# Celitech Python SDK 1.0.1
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.0.0
+- SDK version: 1.0.1
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
```

### Comparing `saer-1.0.0/README.md` & `saer-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# Celitech Python SDK 1.0.0
+# Celitech Python SDK 1.0.1
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.0.0
+- SDK version: 1.0.1
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
```

### Comparing `saer-1.0.0/src/celitech/models/__init__.py` & `saer-1.0.1/src/celitech/models/__init__.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/models/base.py` & `saer-1.0.1/src/celitech/models/base.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/models/create_purchase_ok_response.py` & `saer-1.0.1/src/celitech/models/create_purchase_ok_response.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/models/create_purchase_request.py` & `saer-1.0.1/src/celitech/models/create_purchase_request.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/models/edit_purchase_ok_response.py` & `saer-1.0.1/src/celitech/models/edit_purchase_ok_response.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/models/edit_purchase_request.py` & `saer-1.0.1/src/celitech/models/edit_purchase_request.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/models/get_esim_device_ok_response.py` & `saer-1.0.1/src/celitech/models/get_esim_device_ok_response.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/models/get_esim_history_ok_response.py` & `saer-1.0.1/src/celitech/models/get_esim_history_ok_response.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/models/get_esim_mac_ok_response.py` & `saer-1.0.1/src/celitech/models/get_esim_mac_ok_response.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/models/get_esim_ok_response.py` & `saer-1.0.1/src/celitech/models/get_esim_ok_response.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/models/get_purchase_consumption_ok_response.py` & `saer-1.0.1/src/celitech/models/get_purchase_consumption_ok_response.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/models/list_destinations_ok_response.py` & `saer-1.0.1/src/celitech/models/list_destinations_ok_response.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/models/list_packages_ok_response.py` & `saer-1.0.1/src/celitech/models/list_packages_ok_response.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/models/list_purchases_ok_response.py` & `saer-1.0.1/src/celitech/models/list_purchases_ok_response.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/models/top_up_esim_ok_response.py` & `saer-1.0.1/src/celitech/models/top_up_esim_ok_response.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/models/top_up_esim_request.py` & `saer-1.0.1/src/celitech/models/top_up_esim_request.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/models/utils/cast_models.py` & `saer-1.0.1/src/celitech/models/utils/cast_models.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/models/utils/json_map.py` & `saer-1.0.1/src/celitech/models/utils/json_map.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/net/request_chain/handlers/base_handler.py` & `saer-1.0.1/src/celitech/net/request_chain/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/net/request_chain/handlers/hook_handler.py` & `saer-1.0.1/src/celitech/net/request_chain/handlers/hook_handler.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/net/request_chain/handlers/http_handler.py` & `saer-1.0.1/src/celitech/net/request_chain/handlers/http_handler.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/net/request_chain/handlers/retry_handler.py` & `saer-1.0.1/src/celitech/net/request_chain/handlers/retry_handler.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/net/request_chain/request_chain.py` & `saer-1.0.1/src/celitech/net/request_chain/request_chain.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/net/transport/request.py` & `saer-1.0.1/src/celitech/net/transport/request.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/net/transport/request_error.py` & `saer-1.0.1/src/celitech/net/transport/request_error.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/net/transport/response.py` & `saer-1.0.1/src/celitech/net/transport/response.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/net/transport/serializer.py` & `saer-1.0.1/src/celitech/net/transport/serializer.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/net/transport/utils.py` & `saer-1.0.1/src/celitech/net/transport/utils.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/sdk.py` & `saer-1.0.1/src/celitech/sdk.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/services/destinations.py` & `saer-1.0.1/src/celitech/services/destinations.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/services/e_sim.py` & `saer-1.0.1/src/celitech/services/e_sim.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/services/packages.py` & `saer-1.0.1/src/celitech/services/packages.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/services/purchases.py` & `saer-1.0.1/src/celitech/services/purchases.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/services/utils/base_service.py` & `saer-1.0.1/src/celitech/services/utils/base_service.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/services/utils/default_headers.py` & `saer-1.0.1/src/celitech/services/utils/default_headers.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/celitech/services/utils/validator.py` & `saer-1.0.1/src/celitech/services/utils/validator.py`

 * *Files identical despite different names*

### Comparing `saer-1.0.0/src/saer.egg-info/PKG-INFO` & `saer-1.0.1/src/saer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: saer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 
-# Celitech Python SDK 1.0.0
+# Celitech Python SDK 1.0.1
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.0.0
+- SDK version: 1.0.1
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
```

### Comparing `saer-1.0.0/src/saer.egg-info/SOURCES.txt` & `saer-1.0.1/src/saer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

