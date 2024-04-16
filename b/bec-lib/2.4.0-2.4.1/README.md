# Comparing `tmp/bec_lib-2.4.0.tar.gz` & `tmp/bec_lib-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_lib-2.4.0.tar", last modified: Mon Apr 15 14:54:22 2024, max compression
+gzip compressed data, was "bec_lib-2.4.1.tar", last modified: Tue Apr 16 09:05:02 2024, max compression
```

## Comparing `bec_lib-2.4.0.tar` & `bec_lib-2.4.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:54:22.634084 bec_lib-2.4.0/
--rw-r--r--   0 root         (0) root         (0)     3013 2024-04-15 14:54:22.634084 bec_lib-2.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2616 2024-04-15 09:27:53.000000 bec_lib-2.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:54:22.632084 bec_lib-2.4.0/bec_lib/
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3901 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/alarm_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     3663 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/async_data.py
--rw-rw-rw-   0 root         (0) root         (0)      356 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/bec_errors.py
--rw-rw-rw-   0 root         (0) root         (0)    11292 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/bec_service.py
--rw-rw-rw-   0 root         (0) root         (0)     7247 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/bl_checks.py
--rw-rw-rw-   0 root         (0) root         (0)     2426 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/bl_conditions.py
--rw-rw-rw-   0 root         (0) root         (0)     5994 2024-04-15 14:14:14.000000 bec_lib-2.4.0/bec_lib/callback_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1293 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/channel_monitor.py
--rw-rw-rw-   0 root         (0) root         (0)     9378 2024-04-15 14:14:14.000000 bec_lib-2.4.0/bec_lib/client.py
--rw-rw-rw-   0 root         (0) root         (0)     9055 2024-04-15 14:14:14.000000 bec_lib-2.4.0/bec_lib/config_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:54:22.633084 bec_lib-2.4.0/bec_lib/configs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 14:54:11.000000 bec_lib-2.4.0/bec_lib/configs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    38908 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/configs/demo_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)   289604 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/configs/openapi_schema.json
--rw-rw-rw-   0 root         (0) root         (0)     4747 2024-04-15 14:14:14.000000 bec_lib-2.4.0/bec_lib/connector.py
--rw-rw-rw-   0 root         (0) root         (0)    12816 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/dap_plugin_objects.py
--rw-rw-rw-   0 root         (0) root         (0)     3935 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/dap_plugins.py
--rw-rw-rw-   0 root         (0) root         (0)    30828 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/device.py
--rw-rw-rw-   0 root         (0) root         (0)    23274 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/devicemanager.py
--rw-rw-rw-   0 root         (0) root         (0)    37595 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/endpoints.py
--rw-rw-rw-   0 root         (0) root         (0)     9233 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/file_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/lmfit_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2546 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/logbook_connector.py
--rw-rw-rw-   0 root         (0) root         (0)     7455 2024-04-15 14:14:14.000000 bec_lib-2.4.0/bec_lib/logger.py
--rw-rw-rw-   0 root         (0) root         (0)    20005 2024-04-15 14:14:14.000000 bec_lib-2.4.0/bec_lib/messages.py
--rw-rw-rw-   0 root         (0) root         (0)     5027 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/numpy_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)     5177 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/observer.py
--rw-rw-rw-   0 root         (0) root         (0)     2844 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/pdf_writer.py
--rw-rw-rw-   0 root         (0) root         (0)     7491 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/queue_items.py
--rw-rw-rw-   0 root         (0) root         (0)    39020 2024-04-15 14:14:14.000000 bec_lib-2.4.0/bec_lib/redis_connector.py
--rw-rw-rw-   0 root         (0) root         (0)     5664 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/request_items.py
--rw-rw-rw-   0 root         (0) root         (0)     6526 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/scan_data.py
--rw-rw-rw-   0 root         (0) root         (0)    10892 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/scan_items.py
--rw-rw-rw-   0 root         (0) root         (0)     8573 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/scan_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     6097 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/scan_report.py
--rw-rw-rw-   0 root         (0) root         (0)    17027 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/scans.py
--rw-rw-rw-   0 root         (0) root         (0)     1147 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/scibec_validator.py
--rw-rw-rw-   0 root         (0) root         (0)    10200 2024-04-15 14:14:14.000000 bec_lib-2.4.0/bec_lib/serialization.py
--rw-rw-rw-   0 root         (0) root         (0)     3126 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/service_config.py
--rw-rw-rw-   0 root         (0) root         (0)     4688 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/signature_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:54:22.633084 bec_lib-2.4.0/bec_lib/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 14:54:11.000000 bec_lib-2.4.0/bec_lib/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8004 2024-04-15 14:14:14.000000 bec_lib-2.4.0/bec_lib/tests/end2end_fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)     1594 2024-04-15 13:12:21.000000 bec_lib-2.4.0/bec_lib/tests/fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)    41009 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/tests/test_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      323 2024-04-15 09:27:53.000000 bec_lib-2.4.0/bec_lib/tests/test_service_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    23224 2024-04-15 14:14:14.000000 bec_lib-2.4.0/bec_lib/tests/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5541 2024-04-15 14:14:14.000000 bec_lib-2.4.0/bec_lib/user_scripts_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     7636 2024-04-15 13:12:21.000000 bec_lib-2.4.0/bec_lib/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 14:54:22.634084 bec_lib-2.4.0/bec_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3013 2024-04-15 14:54:22.000000 bec_lib-2.4.0/bec_lib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1506 2024-04-15 14:54:22.000000 bec_lib-2.4.0/bec_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 14:54:22.000000 bec_lib-2.4.0/bec_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      183 2024-04-15 14:54:22.000000 bec_lib-2.4.0/bec_lib.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      258 2024-04-15 14:54:22.000000 bec_lib-2.4.0/bec_lib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-15 14:54:22.000000 bec_lib-2.4.0/bec_lib.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-04-15 14:54:22.635084 bec_lib-2.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1341 2024-04-15 14:54:20.000000 bec_lib-2.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 09:05:02.232884 bec_lib-2.4.1/
+-rw-r--r--   0 root         (0) root         (0)     3013 2024-04-16 09:05:02.232884 bec_lib-2.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2616 2024-04-16 09:04:50.000000 bec_lib-2.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 09:05:02.230883 bec_lib-2.4.1/bec_lib/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3901 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/alarm_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     3663 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/async_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/bec_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    11292 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/bec_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     7247 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/bl_checks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2426 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/bl_conditions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5994 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/callback_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/channel_monitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     9378 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     9055 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/config_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 09:05:02.231883 bec_lib-2.4.1/bec_lib/configs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/configs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    38908 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/configs/demo_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)   289604 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/configs/openapi_schema.json
+-rw-rw-rw-   0 root         (0) root         (0)     4747 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/connector.py
+-rw-rw-rw-   0 root         (0) root         (0)    12816 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/dap_plugin_objects.py
+-rw-rw-rw-   0 root         (0) root         (0)     3935 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/dap_plugins.py
+-rw-rw-rw-   0 root         (0) root         (0)    30828 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/device.py
+-rw-rw-rw-   0 root         (0) root         (0)    23274 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/devicemanager.py
+-rw-rw-rw-   0 root         (0) root         (0)    37595 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/endpoints.py
+-rw-rw-rw-   0 root         (0) root         (0)     9233 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/file_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/lmfit_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2546 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/logbook_connector.py
+-rw-rw-rw-   0 root         (0) root         (0)     7455 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)    20005 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     5027 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/numpy_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     5177 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/observer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2844 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/pdf_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     7491 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/queue_items.py
+-rw-rw-rw-   0 root         (0) root         (0)    39020 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/redis_connector.py
+-rw-rw-rw-   0 root         (0) root         (0)     5664 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/request_items.py
+-rw-rw-rw-   0 root         (0) root         (0)     6526 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/scan_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    10892 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/scan_items.py
+-rw-rw-rw-   0 root         (0) root         (0)     8573 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/scan_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     6097 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/scan_report.py
+-rw-rw-rw-   0 root         (0) root         (0)    17027 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/scans.py
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/scibec_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)    10200 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)     3126 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/service_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     4688 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/signature_serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 09:05:02.231883 bec_lib-2.4.1/bec_lib/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8004 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/tests/end2end_fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)     1594 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/tests/fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)    41009 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/tests/test_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      323 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/tests/test_service_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    23224 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/tests/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5541 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/user_scripts_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     7636 2024-04-16 09:04:50.000000 bec_lib-2.4.1/bec_lib/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 09:05:02.232884 bec_lib-2.4.1/bec_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3013 2024-04-16 09:05:02.000000 bec_lib-2.4.1/bec_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1506 2024-04-16 09:05:02.000000 bec_lib-2.4.1/bec_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 09:05:02.000000 bec_lib-2.4.1/bec_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      183 2024-04-16 09:05:02.000000 bec_lib-2.4.1/bec_lib.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      258 2024-04-16 09:05:02.000000 bec_lib-2.4.1/bec_lib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 09:05:02.000000 bec_lib-2.4.1/bec_lib.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-04-16 09:05:02.233884 bec_lib-2.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2024-04-16 09:04:59.000000 bec_lib-2.4.1/setup.py
```

### Comparing `bec_lib-2.4.0/PKG-INFO` & `bec_lib-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bec_lib
-Version: 2.4.0
+Version: 2.4.1
 Summary: BEC library
 Home-page: https://gitlab.psi.ch/bec/bec
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
```

### Comparing `bec_lib-2.4.0/README.md` & `bec_lib-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/__init__.py` & `bec_lib-2.4.1/bec_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/alarm_handler.py` & `bec_lib-2.4.1/bec_lib/alarm_handler.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/async_data.py` & `bec_lib-2.4.1/bec_lib/async_data.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/bec_service.py` & `bec_lib-2.4.1/bec_lib/bec_service.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/bl_checks.py` & `bec_lib-2.4.1/bec_lib/bl_checks.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/bl_conditions.py` & `bec_lib-2.4.1/bec_lib/bl_conditions.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/callback_handler.py` & `bec_lib-2.4.1/bec_lib/callback_handler.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/channel_monitor.py` & `bec_lib-2.4.1/bec_lib/channel_monitor.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/client.py` & `bec_lib-2.4.1/bec_lib/client.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/config_helper.py` & `bec_lib-2.4.1/bec_lib/config_helper.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/configs/demo_config.yaml` & `bec_lib-2.4.1/bec_lib/configs/demo_config.yaml`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/configs/openapi_schema.json` & `bec_lib-2.4.1/bec_lib/configs/openapi_schema.json`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/connector.py` & `bec_lib-2.4.1/bec_lib/connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/dap_plugin_objects.py` & `bec_lib-2.4.1/bec_lib/dap_plugin_objects.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/dap_plugins.py` & `bec_lib-2.4.1/bec_lib/dap_plugins.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/device.py` & `bec_lib-2.4.1/bec_lib/device.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/devicemanager.py` & `bec_lib-2.4.1/bec_lib/devicemanager.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/endpoints.py` & `bec_lib-2.4.1/bec_lib/endpoints.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/file_utils.py` & `bec_lib-2.4.1/bec_lib/file_utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/lmfit_serializer.py` & `bec_lib-2.4.1/bec_lib/lmfit_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/logbook_connector.py` & `bec_lib-2.4.1/bec_lib/logbook_connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/logger.py` & `bec_lib-2.4.1/bec_lib/logger.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/messages.py` & `bec_lib-2.4.1/bec_lib/messages.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/numpy_encoder.py` & `bec_lib-2.4.1/bec_lib/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/observer.py` & `bec_lib-2.4.1/bec_lib/observer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/pdf_writer.py` & `bec_lib-2.4.1/bec_lib/pdf_writer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/queue_items.py` & `bec_lib-2.4.1/bec_lib/queue_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/redis_connector.py` & `bec_lib-2.4.1/bec_lib/redis_connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/request_items.py` & `bec_lib-2.4.1/bec_lib/request_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/scan_data.py` & `bec_lib-2.4.1/bec_lib/scan_data.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/scan_items.py` & `bec_lib-2.4.1/bec_lib/scan_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/scan_manager.py` & `bec_lib-2.4.1/bec_lib/scan_manager.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/scan_report.py` & `bec_lib-2.4.1/bec_lib/scan_report.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/scans.py` & `bec_lib-2.4.1/bec_lib/scans.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/scibec_validator.py` & `bec_lib-2.4.1/bec_lib/scibec_validator.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/serialization.py` & `bec_lib-2.4.1/bec_lib/serialization.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/service_config.py` & `bec_lib-2.4.1/bec_lib/service_config.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/signature_serializer.py` & `bec_lib-2.4.1/bec_lib/signature_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/tests/end2end_fixtures.py` & `bec_lib-2.4.1/bec_lib/tests/end2end_fixtures.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/tests/fixtures.py` & `bec_lib-2.4.1/bec_lib/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/tests/test_config.yaml` & `bec_lib-2.4.1/bec_lib/tests/test_config.yaml`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/tests/utils.py` & `bec_lib-2.4.1/bec_lib/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/user_scripts_mixin.py` & `bec_lib-2.4.1/bec_lib/user_scripts_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib/utils.py` & `bec_lib-2.4.1/bec_lib/utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/bec_lib.egg-info/PKG-INFO` & `bec_lib-2.4.1/bec_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bec-lib
-Version: 2.4.0
+Version: 2.4.1
 Summary: BEC library
 Home-page: https://gitlab.psi.ch/bec/bec
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
```

### Comparing `bec_lib-2.4.0/bec_lib.egg-info/SOURCES.txt` & `bec_lib-2.4.1/bec_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec_lib-2.4.0/setup.py` & `bec_lib-2.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-__version__ = "2.4.0"
+__version__ = "2.4.1"
 
 if __name__ == "__main__":
     setup(
         install_requires=[
             "hiredis",
             "louie",
             "numpy",
```

