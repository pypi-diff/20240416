# Comparing `tmp/hahomematic-2024.4.7.tar.gz` & `tmp/hahomematic-2024.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2024.4.7.tar", last modified: Sat Apr 13 16:20:10 2024, max compression
+gzip compressed data, was "hahomematic-2024.4.8.tar", last modified: Tue Apr 16 10:12:15 2024, max compression
```

## Comparing `hahomematic-2024.4.7.tar` & `hahomematic-2024.4.8.tar`

### file list

```diff
@@ -1,106 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.983527 hahomematic-2024.4.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-13 16:20:10.983527 hahomematic-2024.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.971527 hahomematic-2024.4.7/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.971527 hahomematic-2024.4.7/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14782 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)    17024 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)    27508 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/caches/visibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.975527 hahomematic-2024.4.7/hahomematic/central/
--rw-r--r--   0 runner    (1001) docker     (127)    57490 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/central/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/central/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9107 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/central/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.975527 hahomematic-2024.4.7/hahomematic/client/
--rw-r--r--   0 runner    (1001) docker     (127)    41418 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34449 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/client/json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/client/xml_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14634 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/performance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.975527 hahomematic-2024.4.7/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.975527 hahomematic-2024.4.7/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26201 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    24315 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (127)    30029 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    44592 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    33450 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    28706 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.979527 hahomematic-2024.4.7/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.979527 hahomematic-2024.4.7/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (127)    14073 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.979527 hahomematic-2024.4.7/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic/support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.983527 hahomematic-2024.4.7/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-13 16:20:10.000000 hahomematic-2024.4.7/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-13 16:20:10.000000 hahomematic-2024.4.7/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 16:20:10.000000 hahomematic-2024.4.7/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 16:20:10.000000 hahomematic-2024.4.7/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-13 16:20:10.000000 hahomematic-2024.4.7/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-13 16:20:10.000000 hahomematic-2024.4.7/hahomematic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.979527 hahomematic-2024.4.7/hahomematic_support/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10275 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/hahomematic_support/client_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    19048 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-13 16:20:10.983527 hahomematic-2024.4.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:10.983527 hahomematic-2024.4.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (127)    26302 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_central.py
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_central_pydevccu.py
--rw-r--r--   0 runner    (1001) docker     (127)    14837 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_climate.py
--rw-r--r--   0 runner    (1001) docker     (127)    26701 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_cover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    31975 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    14347 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-13 16:19:46.000000 hahomematic-2024.4.7/tests/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:12:15.491319 hahomematic-2024.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-16 10:12:15.491319 hahomematic-2024.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:12:15.475319 hahomematic-2024.4.8/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/async_support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:12:15.475319 hahomematic-2024.4.8/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17824 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27542 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/caches/visibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:12:15.475319 hahomematic-2024.4.8/hahomematic/central/
+-rw-r--r--   0 runner    (1001) docker     (127)    54211 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/central/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/central/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/central/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:12:15.479319 hahomematic-2024.4.8/hahomematic/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    42079 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34886 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/client/json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/client/xml_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14686 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/performance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:12:15.479319 hahomematic-2024.4.8/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:12:15.483319 hahomematic-2024.4.8/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26219 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24315 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30029 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12704 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44592 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33530 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29231 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:12:15.483319 hahomematic-2024.4.8/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:12:15.483319 hahomematic-2024.4.8/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14073 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:12:15.487319 hahomematic-2024.4.8/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     9732 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic/support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:12:15.491319 hahomematic-2024.4.8/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-16 10:12:15.000000 hahomematic-2024.4.8/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-16 10:12:15.000000 hahomematic-2024.4.8/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 10:12:15.000000 hahomematic-2024.4.8/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 10:12:15.000000 hahomematic-2024.4.8/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-16 10:12:15.000000 hahomematic-2024.4.8/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-16 10:12:15.000000 hahomematic-2024.4.8/hahomematic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:12:15.487319 hahomematic-2024.4.8/hahomematic_support/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10649 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/hahomematic_support/client_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18951 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-16 10:12:15.491319 hahomematic-2024.4.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:12:15.491319 hahomematic-2024.4.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/tests/test_binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26329 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/tests/test_central.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/tests/test_central_pydevccu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14900 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/tests/test_climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26891 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/tests/test_cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/tests/test_json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32422 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/tests/test_siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14347 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/tests/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/tests/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-16 10:11:48.000000 hahomematic-2024.4.8/tests/test_text.py
```

### Comparing `hahomematic-2024.4.7/LICENSE` & `hahomematic-2024.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/PKG-INFO` & `hahomematic-2024.4.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.4.7
+Version: 2024.4.8
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.4.7/README.md` & `hahomematic-2024.4.8/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/__init__.py` & `hahomematic-2024.4.8/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/caches/dynamic.py` & `hahomematic-2024.4.8/hahomematic/caches/dynamic.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,35 +4,135 @@
 
 from collections.abc import Mapping
 from datetime import datetime
 import logging
 from typing import Any, Final, cast
 
 from hahomematic import central as hmcu
-from hahomematic.config import PING_PONG_MISMATCH_COUNT, PING_PONG_MISMATCH_COUNT_TTL
+from hahomematic.config import (
+    LAST_COMMAND_SEND_STORE_TIMEOUT,
+    PING_PONG_MISMATCH_COUNT,
+    PING_PONG_MISMATCH_COUNT_TTL,
+)
 from hahomematic.const import (
     EVENT_DATA,
     EVENT_INSTANCE_NAME,
     EVENT_INTERFACE_ID,
     EVENT_PONG_MISMATCH_COUNT,
     EVENT_TYPE,
     INIT_DATETIME,
     MAX_CACHE_AGE,
     NO_CACHE_ENTRY,
     CallSource,
     EventType,
     InterfaceEventType,
     InterfaceName,
+    ParamsetKey,
 )
 from hahomematic.platforms.device import HmDevice
-from hahomematic.support import changed_within_seconds
+from hahomematic.support import changed_within_seconds, get_channel_no, get_device_address
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 
+class CommandCache:
+    """Cache for send commands."""
+
+    def __init__(self, interface_id: str) -> None:
+        """Init command cache."""
+        self._interface_id: Final = interface_id
+        # (paramset_key, device_address, channel_no, parameter)
+        self._last_send_command: Final[
+            dict[tuple[str, str, int | None, str], tuple[Any, datetime]]
+        ] = {}
+
+    def add_set_value(
+        self,
+        channel_address: str,
+        parameter: str,
+        value: Any,
+    ) -> None:
+        """Add data from set value command."""
+        key = (
+            ParamsetKey.VALUES.value,
+            get_device_address(channel_address),
+            get_channel_no(channel_address),
+            parameter,
+        )
+        self._last_send_command[key] = (value, datetime.now())
+
+    def add_put_paramset(
+        self,
+        channel_address: str,
+        paramset_key: str,
+        values: dict[str, Any],
+    ) -> None:
+        """Add data from put paramset command."""
+
+        for parameter, value in values.items():
+            key = (
+                paramset_key,
+                get_device_address(channel_address),
+                get_channel_no(channel_address),
+                parameter,
+            )
+            self._last_send_command[key] = (value, datetime.now())
+
+    def get_last_value_send(
+        self,
+        paramset_key: str,
+        channel_address: str,
+        parameter: str,
+        max_age: int = LAST_COMMAND_SEND_STORE_TIMEOUT,
+    ) -> Any:
+        """Return the last send values."""
+        key = (
+            paramset_key,
+            get_device_address(channel_address),
+            get_channel_no(channel_address),
+            parameter,
+        )
+        if result := self._last_send_command.get(key):
+            value, last_send_dt = result
+            if last_send_dt and changed_within_seconds(last_change=last_send_dt, max_age=max_age):
+                return value
+            self.remove_last_value_send(
+                paramset_key=paramset_key,
+                channel_address=channel_address,
+                parameter=parameter,
+                max_age=max_age,
+            )
+        return None
+
+    def remove_last_value_send(
+        self,
+        paramset_key: str,
+        channel_address: str,
+        parameter: str,
+        value: Any = None,
+        max_age: int = LAST_COMMAND_SEND_STORE_TIMEOUT,
+    ) -> None:
+        """Remove the last send value."""
+        key = (
+            paramset_key,
+            get_device_address(channel_address),
+            get_channel_no(channel_address),
+            parameter,
+        )
+
+        if result := self._last_send_command.get(key):
+            stored_value, last_send_dt = result
+            if changed_within_seconds(last_change=last_send_dt, max_age=max_age) or (
+                value and stored_value != value
+            ):
+                return
+
+            del self._last_send_command[key]
+
+
 class DeviceDetailsCache:
     """Cache for device/channel details."""
 
     def __init__(self, central: hmcu.CentralUnit) -> None:
         """Init the device details cache."""
         self._central: Final = central
         self._channel_rooms: Final[dict[str, set[str]]] = {}
@@ -41,15 +141,15 @@
         self._interface_cache: Final[dict[str, str]] = {}
         self._names_cache: Final[dict[str, str]] = {}
         self._last_refreshed = INIT_DATETIME
 
     async def load(self, direct_call: bool = False) -> None:
         """Fetch names from backend."""
         if direct_call is False and changed_within_seconds(
-            last_change=self._last_refreshed, max_age=(MAX_CACHE_AGE / 2)
+            last_change=self._last_refreshed, max_age=int(MAX_CACHE_AGE / 2)
         ):
             return
         self.clear()
         _LOGGER.debug("load: Loading names for %s", self._central.name)
         if client := self._central.primary_client:
             await client.fetch_device_details()
         _LOGGER.debug("load: Loading rooms for %s", self._central.name)
@@ -152,15 +252,15 @@
             self.clear()
             return True
         return False
 
     async def load(self, direct_call: bool = False) -> None:
         """Fetch data from backend."""
         if direct_call is False and changed_within_seconds(
-            last_change=self._last_refreshed, max_age=(MAX_CACHE_AGE / 2)
+            last_change=self._last_refreshed, max_age=int(MAX_CACHE_AGE / 2)
         ):
             return
         self.clear()
         _LOGGER.debug("load: Loading device data for %s", self._central.name)
         for client in self._central.clients:
             await client.fetch_all_device_data()
```

### Comparing `hahomematic-2024.4.7/hahomematic/caches/persistent.py` & `hahomematic-2024.4.8/hahomematic/caches/persistent.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,17 @@
                         orjson.dumps(self._persistant_cache, option=orjson.OPT_NON_STR_KEYS)
                     )
                 return DataOperationResult.SAVE_SUCCESS
 
             _LOGGER.debug("save: not saving cache for %s", self._central.name)
             return DataOperationResult.NO_SAVE
 
-        return await self._central.async_add_executor_job(_save)
+        return await self._central.looper.async_add_executor_job(
+            _save, name=f"save-persistent-cache-{self._filename}"
+        )
 
     async def load(self) -> DataOperationResult:
         """Load file from disk into dict."""
 
         def _load() -> DataOperationResult:
             if not check_or_create_directory(self._cache_dir):
                 return DataOperationResult.NO_LOAD
@@ -84,26 +86,28 @@
                 file=os.path.join(self._cache_dir, self._filename),
                 encoding=DEFAULT_ENCODING,
             ) as fptr:
                 self._persistant_cache.clear()
                 self._persistant_cache.update(orjson.loads(fptr.read()))
             return DataOperationResult.LOAD_SUCCESS
 
-        return await self._central.async_add_executor_job(_load)
+        return await self._central.looper.async_add_executor_job(
+            _load, name=f"load-persistent-cache-{self._filename}"
+        )
 
     async def clear(self) -> None:
         """Remove stored file from disk."""
 
         def _clear() -> None:
             check_or_create_directory(self._cache_dir)
             if os.path.exists(os.path.join(self._cache_dir, self._filename)):
                 os.unlink(os.path.join(self._cache_dir, self._filename))
             self._persistant_cache.clear()
 
-        await self._central.async_add_executor_job(_clear)
+        await self._central.looper.async_add_executor_job(_clear, name="clear-persistent-cache")
 
 
 class DeviceDescriptionCache(BasePersistentCache):
     """Cache for device/channel names."""
 
     def __init__(self, central: hmcu.CentralUnit) -> None:
         """Init the device description cache."""
```

### Comparing `hahomematic-2024.4.7/hahomematic/caches/visibility.py` & `hahomematic-2024.4.8/hahomematic/caches/visibility.py`

 * *Files 0% similar despite different names*

```diff
@@ -703,15 +703,15 @@
             except Exception as ex:
                 _LOGGER.warning(
                     "LOAD failed: Could not read unignore file %s",
                     reduce_args(args=ex.args),
                 )
 
         if self._central.config.load_un_ignore:
-            await self._central.async_add_executor_job(_load)
+            await self._central.looper.async_add_executor_job(_load, name="load-unignore-file")
 
         for line in self._raw_un_ignore_list:
             if "#" not in line:
                 self._add_line_to_cache(line)
 
 
 def check_ignore_parameters_is_clean() -> bool:
```

### Comparing `hahomematic-2024.4.7/hahomematic/central/__init__.py` & `hahomematic-2024.4.8/hahomematic/central/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,37 +3,36 @@
 
 This is the python representation of a CCU.
 """
 
 from __future__ import annotations
 
 import asyncio
-from collections.abc import Callable, Collection, Coroutine, Mapping, Set as AbstractSet
-from concurrent.futures._base import CancelledError
+from collections.abc import Callable, Coroutine, Mapping, Set as AbstractSet
 from datetime import datetime
 import logging
 import socket
 import threading
-from time import monotonic, sleep
-from typing import Any, Final, TypeVar, cast
+from time import sleep
+from typing import Any, Final, cast
 
 from aiohttp import ClientSession
 import orjson
 import voluptuous as vol
 
 from hahomematic import client as hmcl, config
+from hahomematic.async_support import Looper, loop_check
 from hahomematic.caches.dynamic import CentralDataCache, DeviceDetailsCache
 from hahomematic.caches.persistent import DeviceDescriptionCache, ParamsetDescriptionCache
 from hahomematic.caches.visibility import ParameterVisibilityCache
 from hahomematic.central import xml_rpc_server as xmlrpc
 from hahomematic.central.decorators import callback_event, callback_system_event
 from hahomematic.client.json_rpc import JsonRpcAioHttpClient
 from hahomematic.client.xml_rpc import XmlRpcProxy
 from hahomematic.const import (
-    BLOCK_LOG_TIMEOUT,
     DATETIME_FORMAT_MILLIS,
     DEFAULT_TLS,
     DEFAULT_VERIFY_TLS,
     ENTITY_EVENTS,
     EVENT_AVAILABLE,
     EVENT_DATA,
     EVENT_INTERFACE_ID,
@@ -63,27 +62,18 @@
 from hahomematic.platforms.device import HmDevice
 from hahomematic.platforms.entity import BaseEntity, CallbackEntity
 from hahomematic.platforms.event import GenericEvent
 from hahomematic.platforms.generic.entity import GenericEntity
 from hahomematic.platforms.hub import Hub
 from hahomematic.platforms.hub.button import HmProgramButton
 from hahomematic.platforms.hub.entity import GenericHubEntity, GenericSystemVariable
-from hahomematic.support import (
-    cancelling,
-    check_config,
-    get_device_address,
-    loop_check,
-    reduce_args,
-)
+from hahomematic.support import check_config, get_device_address, reduce_args
 
 _LOGGER: Final = logging.getLogger(__name__)
 
-_R = TypeVar("_R")
-_T = TypeVar("_T")
-
 # {instance_name, central}
 CENTRAL_INSTANCES: Final[dict[str, CentralUnit]] = {}
 ConnectionProblemIssuer = JsonRpcAioHttpClient | XmlRpcProxy
 
 INTERFACE_EVENT_SCHEMA = vol.Schema(
     {
         vol.Required(EVENT_INTERFACE_ID): str,
@@ -104,15 +94,15 @@
         self._sema_add_devices: Final = asyncio.Semaphore()
         self._tasks: Final[set[asyncio.Future[Any]]] = set()
         # Keep the config for the central
         self.config: Final = central_config
         self._name: Final = central_config.name
         self._model: str | None = None
         self._connection_state: Final = central_config.connection_state
-        self._loop: Final = asyncio.get_running_loop()
+        self._looper = Looper()
         self._xml_rpc_server: Final = (
             xmlrpc.register_xml_rpc_server(
                 local_port=central_config.callback_port or central_config.default_callback_port
             )
             if central_config.enable_server
             else None
         )
@@ -135,15 +125,17 @@
             central=self
         )
 
         self._primary_client: hmcl.Client | None = None
         # {interface_id, client}
         self._clients: Final[dict[str, hmcl.Client]] = {}
         # {{channel_address, parameter}, event_handle}
-        self._entity_event_subscriptions: Final[dict[tuple[str, str], Any]] = {}
+        self._entity_event_subscriptions: Final[
+            dict[tuple[str, str], list[Callable[[Any], Coroutine[Any, Any, None]]]]
+        ] = {}
         # {device_address, device}
         self._devices: Final[dict[str, HmDevice]] = {}
         # {sysvar_name, sysvar_entity}
         self._sysvar_entities: Final[dict[str, GenericSystemVariable]] = {}
         # {sysvar_name, program_button}U
         self._program_buttons: Final[dict[str, HmProgramButton]] = {}
         # store last event received datetime by interface
@@ -219,14 +211,19 @@
         if self._primary_client is not None:
             return self._primary_client
         if client := self._get_primary_client():
             self._primary_client = client
         return self._primary_client
 
     @property
+    def looper(self) -> Looper:
+        """Return the loop support."""
+        return self._looper
+
+    @property
     def model(self) -> str | None:
         """Return the model of the backend."""
         if not self._model and (client := self.primary_client):
             self._model = client.model
         return self._model
 
     @property
@@ -332,15 +329,15 @@
             )
 
         _LOGGER.debug("STOP: Removing instance")
         if self._name in CENTRAL_INSTANCES:
             del CENTRAL_INSTANCES[self._name]
 
         # wait until tasks are finished
-        await self.block_till_done()
+        await self.looper.block_till_done()
 
         while self._has_active_threads:
             await asyncio.sleep(1)
         self._started = False
 
     async def restart_clients(self) -> None:
         """Restart clients."""
@@ -396,15 +393,15 @@
             await self._init_clients()
 
     async def _stop_clients(self) -> None:
         """Stop clients."""
         await self._de_init_clients()
         for client in self._clients.values():
             _LOGGER.debug("STOP_CLIENTS: Stopping %s", client.interface_id)
-            client.stop()
+            await client.stop()
         _LOGGER.debug("STOP_CLIENTS: Clearing existing clients.")
         self._clients.clear()
 
     async def _create_clients(self) -> bool:
         """Create clients for the central unit. Start connection checker afterwards."""
         if len(self._clients) > 0:
             _LOGGER.warning(
@@ -518,15 +515,17 @@
             tmp_socket.close()
             _LOGGER.debug("GET_LOCAL_IP: Got local ip: %s", local_ip)
             return local_ip
 
         callback_ip: str | None = None
         while callback_ip is None:
             try:
-                callback_ip = await self.async_add_executor_job(get_local_ip, self.config.host)
+                callback_ip = await self.looper.async_add_executor_job(
+                    get_local_ip, self.config.host, name="get_local_ip"
+                )
             except HaHomematicException:
                 callback_ip = "127.0.0.1"
             if callback_ip is None:
                 _LOGGER.warning(
                     "GET_LOCAL_IP: Waiting for %i s,", config.CONNECTION_CHECKER_INTERVAL
                 )
                 await asyncio.sleep(config.CONNECTION_CHECKER_INTERVAL)
@@ -850,15 +849,15 @@
                     client.ping_pong_cache.handle_received_pong(
                         pong_ts=datetime.strptime(v_timestamp, DATETIME_FORMAT_MILLIS)
                     )
             return
         if (channel_address, parameter) in self._entity_event_subscriptions:
             try:
                 for callback in self._entity_event_subscriptions[(channel_address, parameter)]:
-                    callback(value)
+                    await callback(value)
             except RuntimeError as rte:  # pragma: no cover
                 _LOGGER.debug(
                     "EVENT: RuntimeError [%s]. Failed to call callback for: %s, %s, %s",
                     reduce_args(args=rte.args),
                     interface_id,
                     channel_address,
                     parameter,
@@ -913,92 +912,14 @@
         if (
             isinstance(entity, (GenericEntity, GenericEvent))
             and entity.supports_events
             and (entity.channel_address, entity.parameter) in self._entity_event_subscriptions
         ):
             del self._entity_event_subscriptions[(entity.channel_address, entity.parameter)]
 
-    async def block_till_done(self) -> None:
-        """Code from HA. Block until all pending work is done."""
-        # To flush out any call_soon_threadsafe
-        await asyncio.sleep(0)
-        start_time: float | None = None
-        current_task = asyncio.current_task()
-        while tasks := [
-            task for task in self._tasks if task is not current_task and not cancelling(task)
-        ]:
-            await self._await_and_log_pending(tasks)
-
-            if start_time is None:
-                # Avoid calling monotonic() until we know
-                # we may need to start logging blocked tasks.
-                start_time = 0
-            elif start_time == 0:
-                # If we have waited twice then we set the start
-                # time
-                start_time = monotonic()
-            elif monotonic() - start_time > BLOCK_LOG_TIMEOUT:
-                # We have waited at least three loops and new tasks
-                # continue to block. At this point we start
-                # logging all waiting tasks.
-                for task in tasks:
-                    _LOGGER.debug("Waiting for task: %s", task)
-
-    async def _await_and_log_pending(self, pending: Collection[asyncio.Future[Any]]) -> None:
-        """Code from HA. Await and log tasks that take a long time."""
-        wait_time = 0
-        while pending:
-            _, pending = await asyncio.wait(pending, timeout=BLOCK_LOG_TIMEOUT)
-            if not pending:
-                return
-            wait_time += BLOCK_LOG_TIMEOUT
-            for task in pending:
-                _LOGGER.debug("Waited %s seconds for task: %s", wait_time, task)
-
-    def create_task(self, target: Coroutine[Any, Any, Any], name: str) -> None:
-        """Add task to the executor pool."""
-        try:
-            self._loop.call_soon_threadsafe(self._async_create_task, target, name)
-        except CancelledError:
-            _LOGGER.debug(
-                "create_task: task cancelled for %s",
-                self._name,
-            )
-            return
-
-    def _async_create_task(self, target: Coroutine[Any, Any, _R], name: str) -> asyncio.Task[_R]:
-        """Create a task from within the event_loop. This method must be run in the event_loop."""
-        task = self._loop.create_task(target, name=name)
-        self._tasks.add(task)
-        task.add_done_callback(self._tasks.remove)
-        return task
-
-    def run_coroutine(self, coro: Coroutine) -> Any:
-        """Call coroutine from sync."""
-        try:
-            return asyncio.run_coroutine_threadsafe(coro, self._loop).result()
-        except CancelledError:  # pragma: no cover
-            _LOGGER.debug(
-                "run_coroutine: coroutine interrupted for %s",
-                self._name,
-            )
-            return None
-
-    def async_add_executor_job(self, target: Callable[..., _T], *args: Any) -> asyncio.Future[_T]:
-        """Add an executor job from within the event_loop."""
-        try:
-            task = self._loop.run_in_executor(None, target, *args)
-            self._tasks.add(task)
-            task.add_done_callback(self._tasks.remove)
-        except (TimeoutError, CancelledError) as err:  # pragma: no cover
-            message = f"async_add_executor_job: task cancelled for {self._name} [{reduce_args(args=err.args)}]"
-            _LOGGER.debug(message)
-            raise HaHomematicException(message) from err
-        return task
-
     async def execute_program(self, pid: str) -> bool:
         """Execute a program on CCU / Homegear."""
         if client := self.primary_client:
             return await client.execute_program(pid=pid)
         return False
 
     async def fetch_sysvar_data(self, include_internal: bool = True) -> None:
@@ -1190,15 +1111,15 @@
     def run(self) -> None:
         """Run the ConnectionChecker thread."""
         _LOGGER.debug(
             "run: Init connection checker to server %s",
             self._central.name,
         )
         while self._active:
-            self._central.run_coroutine(self._check_connection())
+            self._central.looper.run_coroutine(self._check_connection(), name="check_connection")
             if self._active:
                 sleep(config.CONNECTION_CHECKER_INTERVAL)
 
     def stop(self) -> None:
         """To stop the ConnectionChecker."""
         self._active = False
```

### Comparing `hahomematic-2024.4.7/hahomematic/central/decorators.py` & `hahomematic-2024.4.8/hahomematic/central/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                 unit = args[0]
                 central: hmcu.CentralUnit | None = None
                 if isinstance(unit, hmcu.CentralUnit):
                     central = unit
                 if central is None and isinstance(unit, xmlrpc.RPCFunctions):
                     central = unit.get_central(interface_id=str(args[1]))
                 if central:
-                    central.create_task(
+                    central.looper.create_task(
                         _exec_system_event_callback(*args, **kwargs),
                         name="wrapper_system_event_callback",
                     )
             except Exception as ex:
                 _LOGGER.warning(
                     "EXEC_SYSTEM_EVENT_CALLBACK failed: Problem with identifying central: %s",
                     reduce_args(args=ex.args),
```

### Comparing `hahomematic-2024.4.7/hahomematic/central/xml_rpc_server.py` & `hahomematic-2024.4.8/hahomematic/central/xml_rpc_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     def __init__(self, xml_rpc_server: XmlRpcServer) -> None:
         """Init RPCFunctions."""
         self._xml_rpc_server: Final = xml_rpc_server
 
     def event(self, interface_id: str, channel_address: str, parameter: str, value: Any) -> None:
         """If a device emits some sort event, we will handle it here."""
         if central := self.get_central(interface_id):
-            central.create_task(
+            central.looper.create_task(
                 central.event(
                     interface_id=interface_id,
                     channel_address=channel_address,
                     parameter=parameter,
                     value=value,
                 ),
                 name=f"event-{interface_id}-{channel_address}-{parameter}",
@@ -57,26 +57,26 @@
             return central.list_devices(interface_id=interface_id)  # type: ignore[no-any-return]
         return []
 
     def newDevices(self, interface_id: str, device_descriptions: list[dict[str, Any]]) -> None:
         """Add new devices send from backend."""
         central: hmcu.CentralUnit | None
         if central := self.get_central(interface_id):
-            central.create_task(
+            central.looper.create_task(
                 central.add_new_devices(
                     interface_id=interface_id, device_descriptions=tuple(device_descriptions)
                 ),
                 name=f"newDevices-{interface_id}",
             )
 
     def deleteDevices(self, interface_id: str, addresses: list[str]) -> None:
         """Delete devices send from backend."""
         central: hmcu.CentralUnit | None
         if central := self.get_central(interface_id):
-            central.create_task(
+            central.looper.create_task(
                 central.delete_devices(interface_id=interface_id, addresses=tuple(addresses)),
                 name=f"deleteDevices-{interface_id}",
             )
 
     @callback_system_event(system_event=SystemEvent.UPDATE_DEVICE)
     def updateDevice(self, interface_id: str, address: str, hint: int) -> None:
         """
```

### Comparing `hahomematic-2024.4.7/hahomematic/client/__init__.py` & `hahomematic-2024.4.8/hahomematic/client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from abc import ABC, abstractmethod
 import asyncio
 from datetime import datetime
 import logging
 from typing import Any, Final, cast
 
 from hahomematic import central as hmcu
-from hahomematic.caches.dynamic import PingPongCache
+from hahomematic.caches.dynamic import CommandCache, PingPongCache
 from hahomematic.client.xml_rpc import XmlRpcProxy
 from hahomematic.config import CALLBACK_WARN_INTERVAL, RECONNECT_WAIT
 from hahomematic.const import (
     DATETIME_FORMAT_MILLIS,
     EVENT_AVAILABLE,
     EVENT_SECONDS_SINCE_LAST_EVENT,
     HOMEGEAR_SERIAL,
@@ -49,14 +49,15 @@
 class Client(ABC):
     """Client object to access the backends via XML-RPC or JSON-RPC."""
 
     def __init__(self, client_config: _ClientConfig) -> None:
         """Initialize the Client."""
         self._config: Final = client_config
         self.central: Final[hmcu.CentralUnit] = client_config.central
+        self._last_value_send_cache = CommandCache(interface_id=client_config.interface_id)
 
         self._json_rpc_client: Final = client_config.central.json_rpc_client
 
         self.interface: Final = client_config.interface
         self.interface_id: Final = client_config.interface_id
         self.version: Final = client_config.version
         self._available: bool = True
@@ -83,14 +84,19 @@
 
     @property
     def available(self) -> bool:
         """Return the availability of the client."""
         return self._available
 
     @property
+    def last_value_send_cache(self) -> CommandCache:
+        """Return the last value send cache."""
+        return self._last_value_send_cache
+
+    @property
     @abstractmethod
     def model(self) -> str:
         """Return the model of the backend."""
 
     @property
     def ping_pong_cache(self) -> PingPongCache:
         """Return the ping pong cache."""
@@ -203,18 +209,18 @@
             _LOGGER.info(
                 "RECONNECT: re-connected client %s",
                 self.interface_id,
             )
             return True
         return False
 
-    def stop(self) -> None:
+    async def stop(self) -> None:
         """Stop depending services."""
-        self._proxy.stop()
-        self._proxy_read.stop()
+        await self._proxy.stop()
+        await self._proxy_read.stop()
 
     @abstractmethod
     async def fetch_all_device_data(self) -> None:
         """Fetch all device data from CCU."""
 
     @abstractmethod
     async def fetch_device_details(self) -> None:
@@ -420,14 +426,17 @@
         """Set single value on paramset VALUES."""
         try:
             _LOGGER.debug("SET_VALUE: %s, %s, %s", channel_address, parameter, value)
             if rx_mode:
                 await self._proxy.setValue(channel_address, parameter, value, rx_mode)
             else:
                 await self._proxy.setValue(channel_address, parameter, value)
+            self._last_value_send_cache.add_set_value(
+                channel_address=channel_address, parameter=parameter, value=value
+            )
         except BaseHomematicException as ex:
             _LOGGER.warning(
                 "SET_VALUE failed with %s [%s]: %s, %s, %s",
                 ex.name,
                 reduce_args(args=ex.args),
                 channel_address,
                 parameter,
@@ -449,17 +458,17 @@
             return await self._set_value(
                 channel_address=channel_address,
                 parameter=parameter,
                 value=value,
                 rx_mode=rx_mode,
             )
         return await self.put_paramset(
-            address=channel_address,
+            channel_address=channel_address,
             paramset_key=paramset_key,
-            value={parameter: value},
+            values={parameter: value},
             rx_mode=rx_mode,
         )
 
     async def get_paramset(self, address: str, paramset_key: str) -> dict[str, Any]:
         """
         Return a paramset from CCU.
 
@@ -482,39 +491,42 @@
                 paramset_key,
             )
             raise
 
     @measure_execution_time
     async def put_paramset(
         self,
-        address: str,
+        channel_address: str,
         paramset_key: str,
-        value: Any,
+        values: dict[str, Any],
         rx_mode: str | None = None,
     ) -> bool:
         """
         Set paramsets manually.
 
         Address is usually the channel_address,
         but for bidcos devices there is a master paramset at the device.
         """
         try:
-            _LOGGER.debug("PUT_PARAMSET: %s, %s, %s", address, paramset_key, value)
+            _LOGGER.debug("PUT_PARAMSET: %s, %s, %s", channel_address, paramset_key, values)
             if rx_mode:
-                await self._proxy.putParamset(address, paramset_key, value, rx_mode)
+                await self._proxy.putParamset(channel_address, paramset_key, values, rx_mode)
             else:
-                await self._proxy.putParamset(address, paramset_key, value)
+                await self._proxy.putParamset(channel_address, paramset_key, values)
+            self._last_value_send_cache.add_put_paramset(
+                channel_address=channel_address, paramset_key=paramset_key, values=values
+            )
         except BaseHomematicException as ex:
             _LOGGER.warning(
                 "PUT_PARAMSET failed: %s [%s] %s, %s, %s",
                 ex.name,
                 reduce_args(args=ex.args),
-                address,
+                channel_address,
                 paramset_key,
-                value,
+                values,
             )
             return False
         return True
 
     async def fetch_paramset_description(
         self, channel_address: str, paramset_key: str, save_to_file: bool = True
     ) -> None:
```

### Comparing `hahomematic-2024.4.7/hahomematic/client/json_rpc.py` & `hahomematic-2024.4.8/hahomematic/client/json_rpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import re
 from typing import Any, Final
 
 from aiohttp import ClientConnectorCertificateError, ClientError, ClientResponse, ClientSession
 import orjson
 
 from hahomematic import central as hmcu, config
+from hahomematic.async_support import Looper
 from hahomematic.const import (
     CONF_PASSWORD,
     CONF_USERNAME,
     DEFAULT_ENCODING,
     PATH_JSON_RPC,
     REGA_SCRIPT_FETCH_ALL_DEVICE_DATA,
     REGA_SCRIPT_GET_SERIAL,
@@ -38,14 +39,15 @@
     NoConnection,
     UnsupportedException,
 )
 from hahomematic.support import get_tls_context, parse_sys_var, reduce_args
 
 _LOGGER: Final = logging.getLogger(__name__)
 
+
 _CHANNEL_IDS: Final = "channelIds"
 _HAS_EXT_MARKER: Final = "hasExtMarker"
 _ID: Final = "id"
 _IS_ACTIVE: Final = "isActive"
 _IS_INTERNAL: Final = "isInternal"
 _LAST_EXECUTE_TIME: Final = "lastExecuteTime"
 _MAX_VALUE: Final = "maxValue"
@@ -100,14 +102,15 @@
         verify_tls: bool = False,
     ) -> None:
         """Session setup."""
         self._client_session: Final = client_session
         self._connection_state: Final = connection_state
         self._username: Final = username
         self._password: Final = password
+        self._looper = Looper()
         self._tls: Final = tls
         self._tls_context: Final = get_tls_context(verify_tls) if tls else None
         self._url: Final = f"{device_url}{PATH_JSON_RPC}"
         self._script_cache: Final[dict[str, str]] = {}
         self._last_session_id_refresh: datetime | None = None
         self._session_id: str | None = None
         self._supported_methods: tuple[str, ...] | None = None
@@ -234,15 +237,15 @@
 
         if not session_id:
             raise ClientException("Error while logging in")
 
         if self._supported_methods is None:
             await self._check_supported_methods()
 
-        if (script := self._get_script(script_name=script_name)) is None:
+        if (script := await self._get_script(script_name=script_name)) is None:
             raise ClientException(f"Script file for {script_name} does not exist")
 
         if extra_params:
             for variable, value in extra_params.items():
                 script = script.replace(f"##{variable}##", value)
 
         method = JsonRpcMethod.REGA_RUN_SCRIPT
@@ -258,24 +261,32 @@
                 response[_P_RESULT] = orjson.loads(response[_P_RESULT])
         finally:
             if not keep_session:
                 await self._do_logout(session_id=session_id)
 
         return response
 
-    def _get_script(self, script_name: str) -> str | None:
+    async def _get_script(self, script_name: str) -> str | None:
         """Return a script from the script cache. Load if required."""
         if script_name in self._script_cache:
             return self._script_cache[script_name]
 
-        script_file = os.path.join(Path(__file__).resolve().parent, REGA_SCRIPT_PATH, script_name)
-        if script := Path(script_file).read_text(encoding=DEFAULT_ENCODING):
-            self._script_cache[script_name] = script
-            return script
-        return None
+        def _load_script(script_name: str) -> str | None:
+            """Load script from file system."""
+            script_file = os.path.join(
+                Path(__file__).resolve().parent, REGA_SCRIPT_PATH, script_name
+            )
+            if script := Path(script_file).read_text(encoding=DEFAULT_ENCODING):
+                self._script_cache[script_name] = script
+                return script
+            return None
+
+        return await self._looper.async_add_executor_job(
+            _load_script, script_name, name=f"load_script-{script_name}"
+        )
 
     async def _do_post(
         self,
         session_id: bool | str,
         method: JsonRpcMethod,
         extra_params: dict[str, str] | None = None,
         use_default_params: bool = True,
@@ -364,14 +375,15 @@
             # Workaround for bug in CCU
             return orjson.loads((await response.json(encoding="utf-8")).replace("\\", ""))
 
     async def logout(self) -> None:
         """Logout of CCU."""
         iid = "LOGOUT"
         try:
+            await self._looper.block_till_done()
             await self._do_logout(self._session_id)
             self._connection_state.remove_issue(issuer=self, iid=iid)
         except BaseHomematicException as ex:
             self._handle_exception_log(iid=iid, exception=ex)
 
     async def _do_logout(self, session_id: str | None) -> None:
         """Logout of CCU."""
```

### Comparing `hahomematic-2024.4.7/hahomematic/client/xml_rpc.py` & `hahomematic-2024.4.8/hahomematic/client/xml_rpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 """Implementation of a locking ServerProxy for XML-RPC communication."""
 
 from __future__ import annotations
 
-import asyncio
-from collections.abc import Callable, Mapping
+from collections.abc import Mapping
 from concurrent.futures import ThreadPoolExecutor
 from enum import Enum, IntEnum, StrEnum
 import errno
 import logging
 from ssl import SSLError
-from typing import Any, Final, TypeVar
+from typing import Any, Final
 import xmlrpc.client
 
 from hahomematic import central as hmcu
+from hahomematic.async_support import Looper
 from hahomematic.exceptions import (
     AuthFailure,
     BaseHomematicException,
     ClientException,
     NoConnection,
     UnsupportedException,
 )
 from hahomematic.support import get_tls_context, reduce_args
 
 _LOGGER: Final = logging.getLogger(__name__)
 
-_T = TypeVar("_T")
-
 _CONTEXT: Final = "context"
 _ENCODING_ISO_8859_1: Final = "ISO-8859-1"
 _TLS: Final = "tls"
 _VERIFY_TLS: Final = "verify_tls"
 
 
 class XmlRpcMethod(StrEnum):
@@ -69,18 +67,17 @@
         max_workers: int,
         interface_id: str,
         connection_state: hmcu.CentralConnectionState,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         """Initialize new proxy for server and get local ip."""
-        self._tasks: Final[set[asyncio.Future[Any]]] = set()
         self.interface_id: Final = interface_id
         self._connection_state: Final = connection_state
-        self._loop: Final = asyncio.get_running_loop()
+        self._looper: Final = Looper()
         self._proxy_executor: Final = (
             ThreadPoolExecutor(max_workers=max_workers, thread_name_prefix=interface_id)
             if max_workers > 0
             else None
         )
         self._tls: Final[bool] = kwargs.pop(_TLS, False)
         self._verify_tls: Final[bool] = kwargs.pop(_VERIFY_TLS, True)
@@ -102,23 +99,14 @@
             self._supported_methods = tuple(supported_methods)
 
     @property
     def supported_methods(self) -> tuple[str, ...]:
         """Return the supported methods."""
         return self._supported_methods
 
-    def _async_add_proxy_executor_job(
-        self, func: Callable[..., _T], *args: Any
-    ) -> asyncio.Future[_T]:
-        """Add an executor job from within the event_loop for all device related interaction."""
-        task = self._loop.run_in_executor(self._proxy_executor, func, *args)
-        self._tasks.add(task)
-        task.add_done_callback(self._tasks.remove)
-        return task
-
     async def __async_request(self, *args, **kwargs):  # type: ignore[no-untyped-def]
         """Call method on server side."""
         parent = xmlrpc.client.ServerProxy
         try:
             method = args[0]
             if self._supported_methods and method not in self._supported_methods:
                 raise UnsupportedException(
@@ -129,19 +117,21 @@
                 method in _VALID_XMLRPC_COMMANDS_ON_NO_CONNECTION
                 or not self._connection_state.has_issue(  # noqa: E501
                     issuer=self, iid=self.interface_id
                 )
             ):
                 args = _cleanup_args(*args)
                 _LOGGER.debug("__ASYNC_REQUEST: %s", args)
-                result = await self._async_add_proxy_executor_job(
+                result = await self._looper.async_add_executor_job(
                     # pylint: disable=protected-access
                     parent._ServerProxy__request,  # type: ignore[attr-defined]
                     self,
                     *args,
+                    name="xmp_rpc_proxy",
+                    executor=self._proxy_executor,
                 )
                 self._connection_state.remove_issue(issuer=self, iid=self.interface_id)
                 return result
             raise NoConnection(f"No connection to {self.interface_id}")
         except BaseHomematicException:
             raise
         except SSLError as sslerr:
@@ -175,16 +165,17 @@
         except Exception as ex:
             raise ClientException(ex) from ex
 
     def __getattr__(self, *args, **kwargs):  # type: ignore[no-untyped-def]
         """Magic method dispatcher."""
         return xmlrpc.client._Method(self.__async_request, *args, **kwargs)
 
-    def stop(self) -> None:
+    async def stop(self) -> None:
         """Stop depending services."""
+        await self._looper.block_till_done()
         if self._proxy_executor:
             self._proxy_executor.shutdown()
 
 
 def _cleanup_args(*args: Any) -> Any:
     """Cleanup the type of args."""
     if len(args[1]) == 0:
```

### Comparing `hahomematic-2024.4.7/hahomematic/config.py` & `hahomematic-2024.4.8/hahomematic/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Global configuration parameters."""
 
 from __future__ import annotations
 
 from hahomematic.const import (
     DEFAULT_CONNECTION_CHECKER_INTERVAL,
     DEFAULT_JSON_SESSION_AGE,
+    DEFAULT_LAST_COMMAND_SEND_STORE_TIMEOUT,
     DEFAULT_PING_PONG_MISMATCH_COUNT,
     DEFAULT_PING_PONG_MISMATCH_COUNT_TTL,
     DEFAULT_RECONNECT_WAIT,
     DEFAULT_TIMEOUT,
 )
 
 CALLBACK_WARN_INTERVAL = DEFAULT_CONNECTION_CHECKER_INTERVAL * 40
 CONNECTION_CHECKER_INTERVAL = DEFAULT_CONNECTION_CHECKER_INTERVAL
 JSON_SESSION_AGE = DEFAULT_JSON_SESSION_AGE
+LAST_COMMAND_SEND_STORE_TIMEOUT = DEFAULT_LAST_COMMAND_SEND_STORE_TIMEOUT
 PING_PONG_MISMATCH_COUNT = DEFAULT_PING_PONG_MISMATCH_COUNT
 PING_PONG_MISMATCH_COUNT_TTL = DEFAULT_PING_PONG_MISMATCH_COUNT_TTL
 RECONNECT_WAIT = DEFAULT_RECONNECT_WAIT
 TIMEOUT = DEFAULT_TIMEOUT
```

### Comparing `hahomematic-2024.4.7/hahomematic/const.py` & `hahomematic-2024.4.8/hahomematic/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from datetime import datetime
 from enum import Enum, IntEnum, StrEnum
 from typing import Final
 
 DEFAULT_CONNECTION_CHECKER_INTERVAL: Final = 15  # check if connection is available via rpc ping
 DEFAULT_ENCODING: Final = "UTF-8"
 DEFAULT_JSON_SESSION_AGE: Final = 90
+DEFAULT_LAST_COMMAND_SEND_STORE_TIMEOUT: Final = 60
 DEFAULT_PING_PONG_MISMATCH_COUNT: Final = 15
 DEFAULT_PING_PONG_MISMATCH_COUNT_TTL: Final = 300
 DEFAULT_RECONNECT_WAIT: Final = 120  # wait with reconnect after a first ping was successful
 DEFAULT_TIMEOUT: Final = 60  # default timeout for a connection
 DEFAULT_TLS: Final = False
 DEFAULT_VERIFY_TLS: Final = False
```

### Comparing `hahomematic-2024.4.7/hahomematic/exceptions.py` & `hahomematic-2024.4.8/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/hmcli.py` & `hahomematic-2024.4.8/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/performance.py` & `hahomematic-2024.4.8/hahomematic/performance.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/__init__.py` & `hahomematic-2024.4.8/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/custom/__init__.py` & `hahomematic-2024.4.8/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/custom/climate.py` & `hahomematic-2024.4.8/hahomematic/platforms/custom/climate.py`

 * *Files 0% similar despite different names*

```diff
@@ -542,17 +542,17 @@
                 await self._e_active_profile.send_value(value=profile_idx, collector=collector)
 
     async def enable_away_mode_by_calendar(
         self, start: datetime, end: datetime, away_temperature: float
     ) -> None:
         """Enable the away mode by calendar on thermostat."""
         await self._client.put_paramset(
-            address=self._channel_address,
+            channel_address=self._channel_address,
             paramset_key=ParamsetKey.VALUES,
-            value={
+            values={
                 "SET_POINT_MODE": ModeHmIP.AWAY,
                 "SET_POINT_TEMPERATURE": away_temperature,
                 "PARTY_TIME_START": start.strftime(_PARTY_DATE_FORMAT),
                 "PARTY_TIME_END": end.strftime(_PARTY_DATE_FORMAT),
             },
         )
 
@@ -563,17 +563,17 @@
         await self.enable_away_mode_by_calendar(
             start=start, end=end, away_temperature=away_temperature
         )
 
     async def disable_away_mode(self) -> None:
         """Disable the away mode on thermostat."""
         await self._client.put_paramset(
-            address=self._channel_address,
+            channel_address=self._channel_address,
             paramset_key=ParamsetKey.VALUES,
-            value={
+            values={
                 "SET_POINT_MODE": ModeHmIP.AWAY,
                 "PARTY_TIME_START": _PARTY_INIT_DATE,
                 "PARTY_TIME_END": _PARTY_INIT_DATE,
             },
         )
 
     @property
```

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/custom/const.py` & `hahomematic-2024.4.8/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/custom/cover.py` & `hahomematic-2024.4.8/hahomematic/platforms/custom/cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/custom/definition.py` & `hahomematic-2024.4.8/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/custom/entity.py` & `hahomematic-2024.4.8/hahomematic/platforms/custom/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,23 @@
             if (
                 entity_last_refreshed := entity.last_refreshed
             ) and entity_last_refreshed > latest_refreshed:
                 latest_refreshed = entity_last_refreshed
         return latest_refreshed
 
     @property
+    def unconfirmed_last_values_send(self) -> dict[Field, Any]:
+        """Return the unconfirmed values send for the entity."""
+        unconfirmed_values: dict[Field, Any] = {}
+        for field, entity in self._data_entities.items():
+            if (unconfirmed_value := entity.unconfirmed_last_value_send) is not None:
+                unconfirmed_values[field] = unconfirmed_value
+        return unconfirmed_values
+
+    @property
     def has_data_entities(self) -> bool:
         """Return if there are data entities."""
         return len(self._data_entities) > 0
 
     @value_property
     def is_valid(self) -> bool:
         """Return if the state is valid."""
```

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/custom/light.py` & `hahomematic-2024.4.8/hahomematic/platforms/custom/light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/custom/lock.py` & `hahomematic-2024.4.8/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/custom/siren.py` & `hahomematic-2024.4.8/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/custom/support.py` & `hahomematic-2024.4.8/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/custom/switch.py` & `hahomematic-2024.4.8/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/decorators.py` & `hahomematic-2024.4.8/hahomematic/platforms/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/device.py` & `hahomematic-2024.4.8/hahomematic/platforms/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import os
 import random
 from typing import Any, Final
 
 import orjson
 
 from hahomematic import central as hmcu
+from hahomematic.async_support import loop_check
 from hahomematic.const import (
     DEFAULT_DEVICE_DESCRIPTIONS_DIR,
     DEFAULT_PARAMSET_DESCRIPTIONS_DIR,
     ENTITY_EVENTS,
     IDENTIFIER_SEPARATOR,
     INIT_DATETIME,
     NO_CACHE_ENTRY,
@@ -41,21 +42,15 @@
 from hahomematic.platforms.custom import definition as hmed, entity as hmce
 from hahomematic.platforms.decorators import config_property, value_property
 from hahomematic.platforms.entity import BaseEntity, CallbackEntity
 from hahomematic.platforms.event import GenericEvent
 from hahomematic.platforms.generic.entity import GenericEntity
 from hahomematic.platforms.support import PayloadMixin, get_device_name
 from hahomematic.platforms.update import HmUpdate
-from hahomematic.support import (
-    CacheEntry,
-    Channel,
-    check_or_create_directory,
-    loop_check,
-    reduce_args,
-)
+from hahomematic.support import CacheEntry, Channel, check_or_create_directory, reduce_args
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 
 class HmDevice(PayloadMixin):
     """Object to hold information about a device and associated entities."""
 
@@ -542,15 +537,15 @@
 
         async def refresh_data() -> None:
             for refresh_interval in refresh_after_update_intervals:
                 await asyncio.sleep(refresh_interval)
                 await self.central.refresh_firmware_data(device_address=self._device_address)
 
         if refresh_after_update_intervals:
-            self.central.create_task(target=refresh_data(), name="refresh_firmware_data")
+            self.central.looper.create_task(target=refresh_data(), name="refresh_firmware_data")
 
         return update_result
 
     async def load_value_cache(self) -> None:
         """Init the parameter cache."""
         if len(self._generic_entities) > 0:
             await self.value_cache.init_base_entities()
@@ -850,8 +845,10 @@
                 mode="wb",
             ) as fptr:
                 fptr.write(
                     orjson.dumps(data, option=orjson.OPT_INDENT_2 | orjson.OPT_NON_STR_KEYS)
                 )
             return DataOperationResult.SAVE_SUCCESS
 
-        return await self._central.async_add_executor_job(_save)
+        return await self._central.looper.async_add_executor_job(
+            _save, name="save-device-description"
+        )
```

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/entity.py` & `hahomematic-2024.4.8/hahomematic/platforms/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from inspect import getfullargspec
 import logging
 from typing import Any, Final, Generic, TypeVar, cast
 
 import voluptuous as vol
 
 from hahomematic import central as hmcu, client as hmcl, support as hms
+from hahomematic.async_support import loop_check
 from hahomematic.const import (
     EVENT_ADDRESS,
     EVENT_CHANNEL_NO,
     EVENT_DEVICE_TYPE,
     EVENT_INTERFACE_ID,
     EVENT_PARAMETER,
     EVENT_VALUE,
@@ -38,15 +39,15 @@
 from hahomematic.platforms.decorators import config_property, value_property
 from hahomematic.platforms.support import (
     EntityNameData,
     PayloadMixin,
     convert_value,
     generate_channel_unique_id,
 )
-from hahomematic.support import loop_check, reduce_args
+from hahomematic.support import reduce_args
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 _CallableT = TypeVar("_CallableT", bound=Callable[..., Any])
 
 _CONFIGURABLE_CHANNEL: Final[tuple[str, ...]] = (
     "KEY_TRANSCEIVER",
@@ -538,14 +539,26 @@
         return self._last_updated
 
     @value_property
     def last_refreshed(self) -> datetime:
         """Return the last refreshed datetime value."""
         return self._last_refreshed
 
+    @property
+    def unconfirmed_last_value_send(self) -> ParameterT | None:
+        """Return the unconfirmed value send for the entity."""
+        return cast(
+            ParameterT | None,
+            self._client.last_value_send_cache.get_last_value_send(
+                paramset_key=self.paramset_key,
+                channel_address=self.channel_address,
+                parameter=self.parameter,
+            ),
+        )
+
     @value_property
     def old_value(self) -> ParameterT | None:
         """Return the old value of the entity."""
         return self._old_value
 
     @config_property
     def platform(self) -> HmPlatform:
@@ -645,15 +658,15 @@
         if not raw_unit:
             return 1
         if multiplier := _MULTIPLIER_UNIT.get(raw_unit):
             return multiplier
         return 1
 
     @abstractmethod
-    def event(self, value: Any) -> None:
+    async def event(self, value: Any) -> None:
         """Handle event for which this handler has subscribed."""
 
     async def load_entity_value(self, call_source: CallSource, direct_call: bool = False) -> None:
         """Init the entity data."""
         if direct_call is False and hms.changed_within_seconds(last_change=self._last_refreshed):
             return
 
@@ -780,15 +793,17 @@
                             channel_address=channel_address,
                             paramset_key=ParamsetKey.VALUES,
                             parameter=parameter,
                             value=value,
                         ):
                             return False  # pragma: no cover
                 elif not await self._client.put_paramset(
-                    address=channel_address, paramset_key=ParamsetKey.VALUES, value=paramset
+                    channel_address=channel_address,
+                    paramset_key=ParamsetKey.VALUES,
+                    values=paramset,
                 ):
                     return False  # pragma: no cover
         return True
 
 
 def bind_collector(func: _CallableT) -> _CallableT:
     """Decorate function to automatically add collector if not set."""
```

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/event.py` & `hahomematic-2024.4.8/hahomematic/platforms/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 
 from collections.abc import Mapping
 import logging
 from typing import Any, Final
 
 from hahomematic import support as hms
+from hahomematic.async_support import loop_check
 from hahomematic.const import (
     CLICK_EVENTS,
     DEVICE_ERROR_EVENTS,
     ENTITY_EVENTS,
     IMPULSE_EVENTS,
     Description,
     EntityUsage,
@@ -19,15 +20,14 @@
     Operations,
     ParamsetKey,
 )
 from hahomematic.platforms import device as hmd
 from hahomematic.platforms.decorators import config_property
 from hahomematic.platforms.entity import BaseParameterEntity
 from hahomematic.platforms.support import EntityNameData, generate_unique_id, get_event_name
-from hahomematic.support import loop_check
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 
 class GenericEvent(BaseParameterEntity[Any, Any]):
     """Base class for events."""
 
@@ -60,15 +60,15 @@
         return EntityUsage.EVENT if force_enabled else EntityUsage.NO_CREATE
 
     @config_property
     def event_type(self) -> EventType:
         """Return the event_type of the event."""
         return self._event_type
 
-    def event(self, value: Any) -> None:
+    async def event(self, value: Any) -> None:
         """Handle event for which this handler has subscribed."""
         if self.event_type in ENTITY_EVENTS:
             self.fire_entity_updated_callback(parameter=self.parameter.lower())
         self._set_last_updated()
         self.fire_event(value)
 
     @loop_check
@@ -99,15 +99,15 @@
 
 
 class DeviceErrorEvent(GenericEvent):
     """class for handling device error events."""
 
     _event_type = EventType.DEVICE_ERROR
 
-    def event(self, value: Any) -> None:
+    async def event(self, value: Any) -> None:
         """Handle event for which this handler has subscribed."""
 
         old_value, new_value = self.write_value(value=value)
 
         if (
             isinstance(new_value, bool)
             and (
```

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/generic/__init__.py` & `hahomematic-2024.4.8/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/generic/action.py` & `hahomematic-2024.4.8/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2024.4.8/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/generic/button.py` & `hahomematic-2024.4.8/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/generic/entity.py` & `hahomematic-2024.4.8/hahomematic/platforms/generic/entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,37 +44,37 @@
         """Return the entity usage."""
         if self._is_forced_sensor or self._is_un_ignored:
             return EntityUsage.ENTITY
         if (force_enabled := self._enabled_by_channel_operation_mode) is None:
             return self._usage
         return EntityUsage.ENTITY if force_enabled else EntityUsage.NO_CREATE
 
-    def event(self, value: Any) -> None:
+    async def event(self, value: Any) -> None:
         """Handle event for which this entity has subscribed."""
-
+        self.device.client.last_value_send_cache.remove_last_value_send(
+            paramset_key=self.paramset_key,
+            channel_address=self.channel_address,
+            parameter=self.parameter,
+            value=value,
+        )
         old_value, new_value = self.write_value(value=value)
         if old_value == new_value:
             return
 
         # reload paramset_descriptions, if value has changed
         if (
             self._parameter == Parameter.CONFIG_PENDING
             and new_value is False
             and old_value is True
         ):
-            self._central.create_task(
-                self._device.reload_paramset_descriptions(), name="reloadParamsetDescriptions"
-            )
+            await self._device.reload_paramset_descriptions()
 
             for entity in self._device.get_readable_entities(paramset_key=ParamsetKey.MASTER):
-                self._central.create_task(
-                    entity.load_entity_value(
-                        call_source=CallSource.MANUAL_OR_SCHEDULED, direct_call=True
-                    ),
-                    name="reloadMasterData",
+                await entity.load_entity_value(
+                    call_source=CallSource.MANUAL_OR_SCHEDULED, direct_call=True
                 )
 
         # send device availability events
         if self._parameter in (
             Parameter.UN_REACH,
             Parameter.STICKY_UN_REACH,
         ):
```

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/generic/number.py` & `hahomematic-2024.4.8/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/generic/select.py` & `hahomematic-2024.4.8/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/generic/sensor.py` & `hahomematic-2024.4.8/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/generic/switch.py` & `hahomematic-2024.4.8/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/hub/__init__.py` & `hahomematic-2024.4.8/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2024.4.8/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/hub/button.py` & `hahomematic-2024.4.8/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/hub/entity.py` & `hahomematic-2024.4.8/hahomematic/platforms/hub/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/hub/number.py` & `hahomematic-2024.4.8/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/hub/select.py` & `hahomematic-2024.4.8/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/hub/sensor.py` & `hahomematic-2024.4.8/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/hub/text.py` & `hahomematic-2024.4.8/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/support.py` & `hahomematic-2024.4.8/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/platforms/update.py` & `hahomematic-2024.4.8/hahomematic/platforms/update.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2024.4.8/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2024.4.8/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2024.4.8/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/hahomematic/support.py` & `hahomematic-2024.4.8/hahomematic/support.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 """Helper functions used within hahomematic."""
 
 from __future__ import annotations
 
 import asyncio
 import base64
-from collections.abc import Callable, Collection
+from collections.abc import Collection
 import contextlib
 from dataclasses import dataclass
 from datetime import datetime
-from functools import lru_cache, wraps
+from functools import lru_cache
 import logging
 import os
 import re
 import socket
 import ssl
 import sys
-from typing import Any, Final, ParamSpec, TypeVar
+from typing import Any, Final
 
 from hahomematic.const import (
     CCU_PASSWORD_PATTERN,
     FILE_DEVICES,
     FILE_PARAMSETS,
     IDENTIFIER_SEPARATOR,
     INIT_DATETIME,
     MAX_CACHE_AGE,
     NO_CACHE_ENTRY,
     SysvarType,
 )
 from hahomematic.exceptions import BaseHomematicException, HaHomematicException
 
 _LOGGER: Final = logging.getLogger(__name__)
-_P = ParamSpec("_P")
-_R = TypeVar("_R")
 
 
 def reduce_args(args: tuple[Any, ...]) -> tuple[Any, ...] | Any:
     """Return the first arg, if there is only one arg."""
     return args[0] if len(args) == 1 else args
 
 
@@ -180,15 +178,15 @@
         device_address, channel_no = channel_address.split(":")
         if channel_no in (None, "None"):
             return device_address, None
         return device_address, int(channel_no)
     return channel_address, None
 
 
-def changed_within_seconds(last_change: datetime, max_age: int | float = MAX_CACHE_AGE) -> bool:
+def changed_within_seconds(last_change: datetime, max_age: int = MAX_CACHE_AGE) -> bool:
     """Entity has been updated within X minutes."""
     if last_change == INIT_DATETIME:
         return False
     delta = datetime.now() - last_change
     if delta.seconds < max_age:
         return True
     return False
@@ -296,42 +294,14 @@
 
 
 def cancelling(task: asyncio.Future[Any]) -> bool:
     """Return True if task is cancelling."""
     return bool((cancelling_ := getattr(task, "cancelling", None)) and cancelling_())
 
 
-def loop_check(func: Callable[_P, _R]) -> Callable[_P, _R]:
-    """Annotation to mark method as safe to call from within the event loop."""
-
-    _with_loop: set = set()
-
-    @wraps(func)
-    def wrapper_loop_safe(*args: _P.args, **kwargs: _P.kwargs) -> _R:
-        """Wrap loop safe."""
-        return_value = func(*args, **kwargs)
-
-        try:
-            asyncio.get_running_loop()
-            loop_running = True
-        except Exception:
-            loop_running = False
-
-        if not loop_running and func not in _with_loop:
-            _with_loop.add(func)
-            _LOGGER.warning(
-                "Method %s must run in the event_loop. No loop detected.", func.__name__
-            )
-
-        return return_value
-
-    setattr(func, "_loop_safe", True)
-    return wrapper_loop_safe if debug_enabled() else func
-
-
 def debug_enabled() -> bool:
     """Check if debug mode is enabled."""
     try:
         if sys.gettrace() is not None:
             return True
     except AttributeError:
         pass
```

### Comparing `hahomematic-2024.4.7/hahomematic.egg-info/PKG-INFO` & `hahomematic-2024.4.8/hahomematic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.4.7
+Version: 2024.4.8
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.4.7/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2024.4.8/hahomematic.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 hahomematic/__init__.py
+hahomematic/async_support.py
 hahomematic/config.py
 hahomematic/const.py
 hahomematic/exceptions.py
 hahomematic/hmcli.py
 hahomematic/performance.py
 hahomematic/py.typed
 hahomematic/support.py
```

### Comparing `hahomematic-2024.4.7/hahomematic_support/client_local.py` & `hahomematic-2024.4.8/hahomematic_support/client_local.py`

 * *Files 14% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         """Init the proxy has to tell the CCU / Homegear where to send the events."""
         return ProxyInitState.INIT_SUCCESS
 
     async def proxy_de_init(self) -> ProxyInitState:
         """De-init to stop CCU from sending events for this remote."""
         return ProxyInitState.DE_INIT_SUCCESS
 
-    def stop(self) -> None:
+    async def stop(self) -> None:
         """Stop depending services."""
 
     async def fetch_all_device_data(self) -> None:
         """Fetch all device data from CCU."""
 
     async def fetch_device_details(self) -> None:
         """Fetch names from backend."""
@@ -195,14 +195,17 @@
         paramset_key: str,
         parameter: str,
         value: Any,
         rx_mode: str | None = None,
     ) -> bool:
         """Set single value on paramset VALUES."""
         await self.central.event(self.interface_id, channel_address, parameter, value)
+        self._last_value_send_cache.add_set_value(
+            channel_address=channel_address, parameter=parameter, value=value
+        )
         return True
 
     async def get_paramset(self, address: str, paramset_key: str) -> Any:
         """
         Return a paramset from CCU.
 
         Address is usually the channel_address,
@@ -236,27 +239,32 @@
         ):
             self._paramset_descriptions_cache.update(data)
 
         return self._paramset_descriptions_cache.get(address, {}).get(paramset_key)
 
     async def put_paramset(
         self,
-        address: str,
+        channel_address: str,
         paramset_key: str,
-        value: Any,
+        values: Any,
         rx_mode: str | None = None,
     ) -> bool:
         """
         Set paramsets manually.
 
         Address is usually the channel_address,
         but for bidcos devices there is a master paramset at the device.
         """
-        for parameter in value:
-            await self.central.event(self.interface_id, address, parameter, value[parameter])
+        for parameter in values:
+            await self.central.event(
+                self.interface_id, channel_address, parameter, values[parameter]
+            )
+        self._last_value_send_cache.add_put_paramset(
+            channel_address=channel_address, paramset_key=paramset_key, values=values
+        )
         return True
 
     async def _load_all_json_files(
         self,
         anchor: str,
         resource: str,
         include_list: list[str] | None = None,
@@ -285,15 +293,15 @@
         def _load() -> Any | None:
             with open(
                 file=os.path.join(package_path, resource, filename),
                 encoding=DEFAULT_ENCODING,
             ) as fptr:
                 return orjson.loads(fptr.read())
 
-        return await self.central.async_add_executor_job(_load)
+        return await self.central.looper.async_add_executor_job(_load, name="load-json-file")
 
 
 @dataclass(frozen=True, kw_only=True, slots=True)
 class LocalRessources:
     """Dataclass with information for local client."""
 
     address_device_translation: dict[str, str]
```

### Comparing `hahomematic-2024.4.7/pyproject.toml` & `hahomematic-2024.4.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=69.2.0", "wheel~=0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2024.4.7"
+version     = "2024.4.8"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
@@ -498,16 +498,14 @@
     "PT012", # `pytest.raises()` block should contain a single simple statement
     "PT018", # Assertion should be broken down into multiple parts
     #"SIM102", # Use a single if statement instead of nested if statements
     #"SIM108", # Use ternary operator {contents} instead of if-else-block
     "SIM115", # Use context handler for opening files
     "TRY003", # Avoid specifying long messages outside the exception class
     "TRY400", # Use `logging.exception` instead of `logging.error`
-    "UP006", # keep type annotation style as is
-    "UP007", # keep type annotation style as is
     # Ignored due to performance: https://github.com/charliermarsh/ruff/issues/2923
     "UP038", # Use `X | Y` in `isinstance` call instead of `(X, Y)`
     # Ignored due to incompatible with mypy: https://github.com/python/mypy/issues/15238
     "UP040", # Checks for use of TypeAlias annotation for declaring type aliases.
 
     # May conflict with the formatter, https://docs.astral.sh/ruff/formatter/#conflicting-lint-rules
     "W191",
@@ -523,15 +521,15 @@
 
     # Disabled because ruff does not understand type of __all__ generated by a function
     #"PLE0605",
 
     # temporarily disabled
     #"PT019",
     #"PYI024", # Use typing.NamedTuple instead of collections.namedtuple
-    #"RET503",
+    "RET503",
     #"RET502",
     #"RET501",
     #"TRY002",
     "TRY301",
     "PYI041"
 ]
```

### Comparing `hahomematic-2024.4.7/tests/test_action.py` & `hahomematic-2024.4.8/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/tests/test_binary_sensor.py` & `hahomematic-2024.4.8/tests/test_binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/tests/test_button.py` & `hahomematic-2024.4.8/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/tests/test_central.py` & `hahomematic-2024.4.8/tests/test_central.py`

 * *Files 1% similar despite different names*

```diff
@@ -587,27 +587,27 @@
             paramset_key=ParamsetKey.VALUES,
             parameter="LEVEL",
             value=1.0,
         )
     assert len(mock_client.method_calls) == 60
 
     await central.get_client(interface_id=const.INTERFACE_ID).put_paramset(
-        address="123",
+        channel_address="123",
         paramset_key=ParamsetKey.VALUES,
-        value={"LEVEL": 1.0},
+        values={"LEVEL": 1.0},
     )
     assert mock_client.method_calls[-1] == call.put_paramset(
-        address="123", paramset_key="VALUES", value={"LEVEL": 1.0}
+        channel_address="123", paramset_key="VALUES", values={"LEVEL": 1.0}
     )
     assert len(mock_client.method_calls) == 61
     with pytest.raises(HaHomematicException):
         await central.get_client(interface_id="NOT_A_VALID_INTERFACE_ID").put_paramset(
-            address="123",
+            channel_address="123",
             paramset_key=ParamsetKey.VALUES,
-            value={"LEVEL": 1.0},
+            values={"LEVEL": 1.0},
         )
     assert len(mock_client.method_calls) == 61
 
     assert (
         central.get_generic_entity(
             channel_address="VCU6354483:0", parameter="DUTY_CYCLE"
         ).parameter
```

### Comparing `hahomematic-2024.4.7/tests/test_central_pydevccu.py` & `hahomematic-2024.4.8/tests/test_central_pydevccu.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/tests/test_climate.py` & `hahomematic-2024.4.8/tests/test_climate.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     await climate.set_temperature(12.0)
     last_call = call.set_value(
         channel_address="VCU0000054:2",
         paramset_key="VALUES",
         parameter="SETPOINT",
         value=12.0,
     )
-    assert mock_client.method_calls[-1] == last_call
+    assert mock_client.method_calls[-2] == last_call
     assert climate.target_temperature == 12.0
 
     assert climate.current_temperature is None
     await central.event(const.INTERFACE_ID, "VCU0000054:1", "TEMPERATURE", 11.0)
     assert climate.current_temperature == 11.0
 
     assert climate.hvac_mode == HvacMode.HEAT
@@ -75,25 +75,25 @@
     assert climate.preset_mode == PresetMode.NONE
     assert climate.preset_modes == (PresetMode.NONE,)
     assert climate.hvac_action is None
     await central.event(const.INTERFACE_ID, "VCU0000054:1", "TEMPERATURE", 11.0)
 
     # No new method call, because called methods has no implementation
     await climate.set_hvac_mode(HvacMode.HEAT)
-    assert mock_client.method_calls[-1] == last_call
+    assert mock_client.method_calls[-4] == last_call
     await climate.set_preset_mode(PresetMode.NONE)
-    assert mock_client.method_calls[-1] == last_call
+    assert mock_client.method_calls[-4] == last_call
     await climate.enable_away_mode_by_duration(hours=100, away_temperature=17.0)
-    assert mock_client.method_calls[-1] == last_call
+    assert mock_client.method_calls[-4] == last_call
     await climate.enable_away_mode_by_calendar(
         start=datetime.now(), end=datetime.now(), away_temperature=17.0
     )
-    assert mock_client.method_calls[-1] == last_call
+    assert mock_client.method_calls[-4] == last_call
     await climate.disable_away_mode()
-    assert mock_client.method_calls[-1] == last_call
+    assert mock_client.method_calls[-4] == last_call
 
 
 @pytest.mark.asyncio()
 async def test_cerfthermostat(factory: helper.Factory) -> None:
     """Test CeRfThermostat."""
     central, mock_client = await factory.get_default_central(TEST_DEVICES)
     climate: CeRfThermostat = cast(
@@ -109,15 +109,15 @@
     await central.event(const.INTERFACE_ID, "VCU0000050:4", "VALVE_STATE", 10)
     assert climate.hvac_action == HvacAction.HEAT
     await central.event(const.INTERFACE_ID, "VCU0000050:4", "VALVE_STATE", 0)
     assert climate.hvac_action == HvacAction.IDLE
     assert climate.current_humidity is None
     assert climate.target_temperature is None
     await climate.set_temperature(12.0)
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU0000050:4",
         paramset_key="VALUES",
         parameter="SET_TEMPERATURE",
         value=12.0,
     )
     assert climate.target_temperature == 12.0
 
@@ -131,18 +131,18 @@
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000050:4", paramset_key="VALUES", parameter="MANU_MODE", value=12.0
     )
     await central.event(const.INTERFACE_ID, "VCU0000050:4", "CONTROL_MODE", ModeHmIP.MANU.value)
     assert climate.hvac_mode == HvacMode.HEAT
 
     await climate.set_hvac_mode(HvacMode.OFF)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU0000050:4",
+    assert mock_client.method_calls[-2] == call.put_paramset(
+        channel_address="VCU0000050:4",
         paramset_key="VALUES",
-        value={"MANU_MODE": 12.0, "SET_TEMPERATURE": 4.5},
+        values={"MANU_MODE": 12.0, "SET_TEMPERATURE": 4.5},
     )
 
     assert climate.hvac_mode == HvacMode.OFF
     assert climate.hvac_action == HvacAction.OFF
 
     await climate.set_hvac_mode(HvacMode.AUTO)
     assert mock_client.method_calls[-1] == call.set_value(
@@ -245,15 +245,15 @@
 
     assert climate.current_humidity is None
     await central.event(const.INTERFACE_ID, "VCU1769958:1", "HUMIDITY", 75)
     assert climate.current_humidity == 75
 
     assert climate.target_temperature is None
     await climate.set_temperature(12.0)
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU1769958:1",
         paramset_key="VALUES",
         parameter="SET_POINT_TEMPERATURE",
         value=12.0,
     )
     assert climate.target_temperature == 12.0
 
@@ -262,48 +262,48 @@
     assert climate.current_temperature == 11.0
 
     assert climate.hvac_mode == HvacMode.AUTO
     assert climate.hvac_modes == (HvacMode.AUTO, HvacMode.HEAT, HvacMode.OFF)
     assert climate.preset_mode == PresetMode.NONE
 
     await climate.set_hvac_mode(HvacMode.OFF)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU1769958:1",
+    assert mock_client.method_calls[-2] == call.put_paramset(
+        channel_address="VCU1769958:1",
         paramset_key="VALUES",
-        value={"CONTROL_MODE": 1, "SET_POINT_TEMPERATURE": 4.5},
+        values={"CONTROL_MODE": 1, "SET_POINT_TEMPERATURE": 4.5},
     )
     assert climate.hvac_mode == HvacMode.OFF
     assert climate.hvac_action == HvacAction.OFF
 
     await climate.set_hvac_mode(HvacMode.HEAT)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU1769958:1",
+    assert mock_client.method_calls[-2] == call.put_paramset(
+        channel_address="VCU1769958:1",
         paramset_key="VALUES",
-        value={"CONTROL_MODE": 1, "SET_POINT_TEMPERATURE": 5.0},
+        values={"CONTROL_MODE": 1, "SET_POINT_TEMPERATURE": 5.0},
     )
     await central.event(const.INTERFACE_ID, "VCU1769958:1", "SET_POINT_MODE", ModeHmIP.MANU.value)
     assert climate.hvac_mode == HvacMode.HEAT
 
     assert climate.preset_mode == PresetMode.NONE
     assert climate.preset_modes == (
         PresetMode.BOOST,
         PresetMode.NONE,
     )
     await climate.set_preset_mode(PresetMode.BOOST)
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU1769958:1", paramset_key="VALUES", parameter="BOOST_MODE", value=True
     )
     await central.event(const.INTERFACE_ID, "VCU1769958:1", "BOOST_MODE", 1)
     assert climate.preset_mode == PresetMode.BOOST
 
     await climate.set_hvac_mode(HvacMode.AUTO)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU1769958:1",
+    assert mock_client.method_calls[-2] == call.put_paramset(
+        channel_address="VCU1769958:1",
         paramset_key="VALUES",
-        value={"BOOST_MODE": False, "CONTROL_MODE": 0},
+        values={"BOOST_MODE": False, "CONTROL_MODE": 0},
     )
     await central.event(const.INTERFACE_ID, "VCU1769958:1", "SET_POINT_MODE", ModeHmIP.AUTO.value)
     await central.event(const.INTERFACE_ID, "VCU1769958:1", "BOOST_MODE", 1)
     assert climate.hvac_mode == HvacMode.AUTO
     assert climate.preset_modes == (
         PresetMode.BOOST,
         PresetMode.NONE,
@@ -311,59 +311,59 @@
         "week_program_2",
         "week_program_3",
         "week_program_4",
         "week_program_5",
         "week_program_6",
     )
     await climate.set_preset_mode(PresetMode.NONE)
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU1769958:1", paramset_key="VALUES", parameter="BOOST_MODE", value=False
     )
     await central.event(const.INTERFACE_ID, "VCU1769958:1", "SET_POINT_MODE", ModeHmIP.AWAY.value)
     assert climate.preset_mode == PresetMode.AWAY
 
     await central.event(const.INTERFACE_ID, "VCU1769958:1", "SET_POINT_MODE", ModeHmIP.AUTO.value)
     await climate.set_preset_mode(PresetMode.WEEK_PROGRAM_1)
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU1769958:1", paramset_key="VALUES", parameter="ACTIVE_PROFILE", value=1
     )
     assert climate.preset_mode == PresetMode.WEEK_PROGRAM_1
 
     with freeze_time("2023-03-03 08:00:00"):
         await climate.enable_away_mode_by_duration(hours=100, away_temperature=17.0)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU1769958:1",
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU1769958:1",
         paramset_key="VALUES",
-        value={
+        values={
             "SET_POINT_MODE": 2,
             "SET_POINT_TEMPERATURE": 17.0,
             "PARTY_TIME_START": "2023_03_03 07:50",
             "PARTY_TIME_END": "2023_03_07 12:00",
         },
     )
 
     await climate.enable_away_mode_by_calendar(
         start=datetime(2000, 12, 1), end=datetime(2024, 12, 1), away_temperature=17.0
     )
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU1769958:1",
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU1769958:1",
         paramset_key="VALUES",
-        value={
+        values={
             "SET_POINT_MODE": 2,
             "SET_POINT_TEMPERATURE": 17.0,
             "PARTY_TIME_START": "2000_12_01 00:00",
             "PARTY_TIME_END": "2024_12_01 00:00",
         },
     )
 
     await climate.disable_away_mode()
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU1769958:1",
+    assert mock_client.method_calls[-2] == call.put_paramset(
+        channel_address="VCU1769958:1",
         paramset_key="VALUES",
-        value={
+        values={
             "SET_POINT_MODE": 2,
             "PARTY_TIME_START": "2000_01_01 00:00",
             "PARTY_TIME_END": "2000_01_01 00:00",
         },
     )
 
     await central.event(const.INTERFACE_ID, "VCU1769958:1", "BOOST_MODE", 1)
```

### Comparing `hahomematic-2024.4.7/tests/test_cover.py` & `hahomematic-2024.4.8/tests/test_cover.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,32 +44,32 @@
     cover: CeCover = cast(CeCover, helper.get_prepared_custom_entity(central, "VCU8537918", 4))
     assert cover.usage == EntityUsage.CE_PRIMARY
 
     assert cover.current_position == 0
     assert cover._channel_level == _CLOSED_LEVEL
     assert cover.is_closed is True
     await cover.set_position(position=81)
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU8537918:4",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=0.81,
     )
     assert cover.current_position == 81
     assert cover.is_closed is False
     await cover.open()
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU8537918:4",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=1.0,
     )
     assert cover.current_position == 100
     await cover.close()
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU8537918:4",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=_CLOSED_LEVEL,
     )
     assert cover.current_position == 0
 
@@ -160,33 +160,33 @@
     )
     assert cover.usage == EntityUsage.CE_PRIMARY
 
     assert cover.current_position == 0
     assert cover._channel_level == _WD_CLOSED_LEVEL
     assert cover.is_closed is True
     await cover.set_position(position=81)
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU0000350:1",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=0.81,
     )
     assert cover.current_position == 81
     assert cover.is_closed is False
 
     await cover.open()
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU0000350:1",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=_OPEN_LEVEL,
     )
     assert cover.current_position == 100
     await cover.close()
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU0000350:1",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=_WD_CLOSED_LEVEL,
     )
     assert cover.current_position == 0
     assert cover._channel_level == _WD_CLOSED_LEVEL
@@ -306,22 +306,22 @@
     )
 
     await cover.open_tilt()
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _OPEN_LEVEL)
     call_count = len(mock_client.method_calls)
     await cover.open_tilt()
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _OPEN_LEVEL)
-    assert call_count == len(mock_client.method_calls)
+    assert call_count == len(mock_client.method_calls) - 1
 
     await cover.close_tilt()
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _CLOSED_LEVEL)
     call_count = len(mock_client.method_calls)
     await cover.close_tilt()
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _CLOSED_LEVEL)
-    assert call_count == len(mock_client.method_calls)
+    assert call_count == len(mock_client.method_calls) - 1
 
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", 0.4)
     call_count = len(mock_client.method_calls)
     await cover.set_position(tilt_position=40)
     assert call_count == len(mock_client.method_calls)
 
 
@@ -453,67 +453,81 @@
     central, mock_client = await factory.get_default_central(TEST_DEVICES)
     cover: CeIpBlind = cast(CeIpBlind, helper.get_prepared_custom_entity(central, "VCU3560967", 1))
     assert cover.usage == EntityUsage.CE_PRIMARY
 
     assert cover.current_position == 0
     assert cover.current_tilt_position == 0
     await cover.set_position(position=81)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU3560967:1", paramset_key="VALUES", value={"LEVEL_2": 0.0, "LEVEL": 0.81}
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU3560967:1",
+        paramset_key="VALUES",
+        values={"LEVEL_2": 0.0, "LEVEL": 0.81},
     )
     await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", 0.81)
     assert cover.current_position == 81
     assert cover.current_tilt_position == 0
 
     await cover.open()
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU3560967:1", paramset_key="VALUES", value={"LEVEL_2": 1.0, "LEVEL": 1.0}
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU3560967:1",
+        paramset_key="VALUES",
+        values={"LEVEL_2": 1.0, "LEVEL": 1.0},
     )
     await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 1.0)
     await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", 1.0)
     assert cover.current_position == 100
     assert cover.current_tilt_position == 100
 
     await cover.close()
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU3560967:1", paramset_key="VALUES", value={"LEVEL_2": 0.0, "LEVEL": 0.0}
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU3560967:1",
+        paramset_key="VALUES",
+        values={"LEVEL_2": 0.0, "LEVEL": 0.0},
     )
     await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 0.0)
     await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", 0.0)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 0
 
     await cover.open_tilt()
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU3560967:1", paramset_key="VALUES", value={"LEVEL_2": 1.0, "LEVEL": 0.0}
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU3560967:1",
+        paramset_key="VALUES",
+        values={"LEVEL_2": 1.0, "LEVEL": 0.0},
     )
     await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 1.0)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 100
 
     await cover.set_position(tilt_position=45)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU3560967:1", paramset_key="VALUES", value={"LEVEL_2": 0.45, "LEVEL": 0.0}
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU3560967:1",
+        paramset_key="VALUES",
+        values={"LEVEL_2": 0.45, "LEVEL": 0.0},
     )
     await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 0.45)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 45
 
     await cover.close_tilt()
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU3560967:1", paramset_key="VALUES", value={"LEVEL_2": 0.0, "LEVEL": 0.0}
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU3560967:1",
+        paramset_key="VALUES",
+        values={"LEVEL_2": 0.0, "LEVEL": 0.0},
     )
     await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 0.0)
     await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", 0.0)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 0
 
     await cover.set_position(position=10, tilt_position=20)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU3560967:1", paramset_key="VALUES", value={"LEVEL_2": 0.2, "LEVEL": 0.1}
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU3560967:1",
+        paramset_key="VALUES",
+        values={"LEVEL_2": 0.2, "LEVEL": 0.1},
     )
     await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", 0.1)
     await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 0.2)
     assert cover.current_position == 10
     assert cover.current_tilt_position == 20
 
     await central.event(const.INTERFACE_ID, "VCU3560967:1", "ACTIVITY_STATE", 1)
```

### Comparing `hahomematic-2024.4.7/tests/test_decorator.py` & `hahomematic-2024.4.8/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/tests/test_device.py` & `hahomematic-2024.4.8/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/tests/test_entity.py` & `hahomematic-2024.4.8/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/tests/test_event.py` & `hahomematic-2024.4.8/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/tests/test_json_rpc.py` & `hahomematic-2024.4.8/tests/test_json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/tests/test_light.py` & `hahomematic-2024.4.8/tests/test_light.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,64 +51,68 @@
     assert light.supports_transition is True
     assert light.effect is None
     assert light.effects is None
 
     assert light.brightness == 0
     assert light.brightness_pct == 0
     await light.turn_on()
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU1399816:4", paramset_key="VALUES", parameter="LEVEL", value=1.0
     )
     assert light.brightness == 255
     assert light.brightness_pct == 100
     await light.turn_on(brightness=28)
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU1399816:4",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=0.10980392156862745,
     )
     assert light.brightness == 28
     assert light.brightness_pct == 10
     assert light.is_on
 
     assert light.channel_brightness is None
     await central.event(const.INTERFACE_ID, "VCU1399816:3", "LEVEL", 0.4)
     assert light.channel_brightness == 102
 
     await light.turn_on(on_time=5.0, ramp_time=6.0)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU1399816:4",
+    assert mock_client.method_calls[-2] == call.put_paramset(
+        channel_address="VCU1399816:4",
         paramset_key="VALUES",
-        value={"LEVEL": 0.10980392156862745, "RAMP_TIME": 6.0, "ON_TIME": 5.0},
+        values={"LEVEL": 0.10980392156862745, "RAMP_TIME": 6.0, "ON_TIME": 5.0},
     )
     await light.turn_on(on_time=5.0)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU1399816:4",
+    assert mock_client.method_calls[-2] == call.put_paramset(
+        channel_address="VCU1399816:4",
         paramset_key="VALUES",
-        value={"ON_TIME": 5.0, "LEVEL": 0.10980392156862745},
+        values={"ON_TIME": 5.0, "LEVEL": 0.10980392156862745},
     )
 
     await light.turn_off(ramp_time=6.0)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU1399816:4", paramset_key="VALUES", value={"RAMP_TIME": 6.0, "LEVEL": 0.0}
+    assert mock_client.method_calls[-2] == call.put_paramset(
+        channel_address="VCU1399816:4",
+        paramset_key="VALUES",
+        values={"RAMP_TIME": 6.0, "LEVEL": 0.0},
     )
     assert light.brightness == 0
     await light.turn_on()
     assert light.brightness == 255
     await light.turn_off()
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU1399816:4", paramset_key="VALUES", parameter="LEVEL", value=0.0
     )
 
     await light.turn_off()
     light.set_on_time(0.5)
     await light.turn_on()
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU1399816:4", paramset_key="VALUES", value={"ON_TIME": 0.5, "LEVEL": 1.0}
+    assert mock_client.method_calls[-2] == call.put_paramset(
+        channel_address="VCU1399816:4",
+        paramset_key="VALUES",
+        values={"ON_TIME": 0.5, "LEVEL": 1.0},
     )
 
     await light.turn_on()
     call_count = len(mock_client.method_calls)
     await light.turn_on()
     assert call_count == len(mock_client.method_calls)
 
@@ -142,57 +146,57 @@
         "Campfire",
         "Waterfall",
         "TV simulation",
     )
 
     assert light.brightness == 0
     await light.turn_on()
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU3747418:1", paramset_key="VALUES", parameter="LEVEL", value=1.0
     )
     assert light.brightness == 255
     await light.turn_on(brightness=28)
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU3747418:1",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=0.10980392156862745,
     )
     assert light.brightness == 28
     await light.turn_off()
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU3747418:1", paramset_key="VALUES", parameter="LEVEL", value=0.0
     )
     assert light.brightness == 0
 
     assert light.hs_color == (0.0, 0.0)
     await light.turn_on(hs_color=(44.4, 69.3))
-    assert mock_client.method_calls[-2] == call.set_value(
+    assert mock_client.method_calls[-4] == call.set_value(
         channel_address="VCU3747418:2", paramset_key="VALUES", parameter="COLOR", value=25
     )
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU3747418:1", paramset_key="VALUES", parameter="LEVEL", value=1.0
     )
     assert light.hs_color == (45.0, 100)
 
     await light.turn_on(hs_color=(0, 50))
-    assert mock_client.method_calls[-2] == call.set_value(
+    assert mock_client.method_calls[-4] == call.set_value(
         channel_address="VCU3747418:2", paramset_key="VALUES", parameter="COLOR", value=0
     )
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU3747418:1", paramset_key="VALUES", parameter="LEVEL", value=1.0
     )
     assert light.hs_color == (0.0, 100.0)
 
     await light.turn_on(effect="Slow color change")
 
-    assert mock_client.method_calls[-2] == call.set_value(
+    assert mock_client.method_calls[-4] == call.set_value(
         channel_address="VCU3747418:1", paramset_key="VALUES", parameter="LEVEL", value=1.0
     )
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU3747418:3", paramset_key="VALUES", parameter="PROGRAM", value=1
     )
 
     assert light.effect == "Slow color change"
 
     await central.event(const.INTERFACE_ID, "VCU3747418:2", "COLOR", 201)
     assert light.hs_color == (0.0, 0.0)
@@ -206,21 +210,21 @@
 
     await light.turn_off()
     call_count = len(mock_client.method_calls)
     await light.turn_off()
     assert call_count == len(mock_client.method_calls)
 
     await light.turn_on(brightness=28, effect="Slow color change")
-    assert mock_client.method_calls[-2] == call.set_value(
+    assert mock_client.method_calls[-4] == call.set_value(
         channel_address="VCU3747418:1",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=0.10980392156862745,
     )
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU3747418:3", paramset_key="VALUES", parameter="PROGRAM", value=1
     )
 
 
 @pytest.mark.asyncio()
 async def test_cecolortempdimmer(factory: helper.Factory) -> None:
     """Test CeColorTempDimmer."""
@@ -236,41 +240,41 @@
     assert light.supports_effects is False
     assert light.supports_hs_color is False
     assert light.supports_transition is True
     assert light.effect is None
     assert light.effects is None
     assert light.brightness == 0
     await light.turn_on()
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU0000115:1", paramset_key="VALUES", parameter="LEVEL", value=1.0
     )
     assert light.brightness == 255
     await light.turn_on(brightness=28)
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU0000115:1",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=0.10980392156862745,
     )
     assert light.brightness == 28
     await light.turn_off()
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU0000115:1", paramset_key="VALUES", parameter="LEVEL", value=0.0
     )
     assert light.brightness == 0
 
     assert light.color_temp == 500
     await light.turn_on(color_temp=433)
-    assert mock_client.method_calls[-2] == call.set_value(
+    assert mock_client.method_calls[-4] == call.set_value(
         channel_address="VCU0000115:2",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=0.1930835734870317,
     )
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU0000115:1", paramset_key="VALUES", parameter="LEVEL", value=1.0
     )
     assert light.color_temp == 433
 
     await light.turn_on()
     call_count = len(mock_client.method_calls)
     await light.turn_on()
@@ -302,127 +306,127 @@
     assert light.brightness == 0
     assert light.is_on is False
     assert light.color_name == FixedColor.BLACK
     assert light.channel_color_name is None
     assert light.channel_brightness is None
     assert light.channel_hs_color is None
     await light.turn_on()
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU3716619:8", paramset_key="VALUES", value={"COLOR": 7, "LEVEL": 1.0}
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU3716619:8", paramset_key="VALUES", values={"COLOR": 7, "LEVEL": 1.0}
     )
     assert light.brightness == 255
     await light.turn_on(brightness=28)
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU3716619:8",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=0.10980392156862745,
     )
     assert light.brightness == 28
     await light.turn_off()
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU3716619:8", paramset_key="VALUES", parameter="LEVEL", value=0.0
     )
     assert light.brightness == 0
     assert light.color_name == FixedColor.WHITE
 
     await light.turn_on(hs_color=(350, 50))
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU3716619:8", paramset_key="VALUES", value={"COLOR": 4, "LEVEL": 1.0}
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU3716619:8", paramset_key="VALUES", values={"COLOR": 4, "LEVEL": 1.0}
     )
     assert light.color_name == FixedColor.RED
 
     await light.turn_on(hs_color=(0.0, 0.0))
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU3716619:8", paramset_key="VALUES", value={"COLOR": 7, "LEVEL": 1.0}
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU3716619:8", paramset_key="VALUES", values={"COLOR": 7, "LEVEL": 1.0}
     )
     assert light.color_name == FixedColor.WHITE
 
     await light.turn_on(hs_color=(60.0, 50.0))
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU3716619:8", paramset_key="VALUES", value={"COLOR": 6, "LEVEL": 1.0}
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU3716619:8", paramset_key="VALUES", values={"COLOR": 6, "LEVEL": 1.0}
     )
     assert light.color_name == FixedColor.YELLOW
 
     await light.turn_on(hs_color=(120, 50))
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU3716619:8", paramset_key="VALUES", value={"COLOR": 2, "LEVEL": 1.0}
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU3716619:8", paramset_key="VALUES", values={"COLOR": 2, "LEVEL": 1.0}
     )
     assert light.color_name == FixedColor.GREEN
 
     await light.turn_on(hs_color=(180, 50))
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU3716619:8", paramset_key="VALUES", value={"COLOR": 3, "LEVEL": 1.0}
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU3716619:8", paramset_key="VALUES", values={"COLOR": 3, "LEVEL": 1.0}
     )
     assert light.color_name == FixedColor.TURQUOISE
 
     await light.turn_on(hs_color=(240, 50))
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU3716619:8", paramset_key="VALUES", value={"COLOR": 1, "LEVEL": 1.0}
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU3716619:8", paramset_key="VALUES", values={"COLOR": 1, "LEVEL": 1.0}
     )
     assert light.color_name == FixedColor.BLUE
 
     await light.turn_on(hs_color=(300, 50))
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU3716619:8", paramset_key="VALUES", value={"COLOR": 5, "LEVEL": 1.0}
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU3716619:8", paramset_key="VALUES", values={"COLOR": 5, "LEVEL": 1.0}
     )
     assert light.color_name == FixedColor.PURPLE
 
     await central.event(const.INTERFACE_ID, "VCU3716619:7", "LEVEL", 0.5)
     assert light.channel_brightness == 127
 
     await central.event(const.INTERFACE_ID, "VCU3716619:7", "COLOR", 1)
     assert light.channel_hs_color == (240.0, 100.0)
     assert light.channel_color_name == FixedColor.BLUE
 
     await light.turn_off()
     light.set_on_time(18)
     await light.turn_on()
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU3716619:8",
+    assert mock_client.method_calls[-2] == call.put_paramset(
+        channel_address="VCU3716619:8",
         paramset_key="VALUES",
-        value={"DURATION_VALUE": 18, "LEVEL": 1.0},
+        values={"DURATION_VALUE": 18, "LEVEL": 1.0},
     )
 
     await light.turn_off()
     light.set_on_time(17000)
     await light.turn_on()
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU3716619:8",
+    assert mock_client.method_calls[-2] == call.put_paramset(
+        channel_address="VCU3716619:8",
         paramset_key="VALUES",
-        value={"DURATION_UNIT": 1, "DURATION_VALUE": 283, "LEVEL": 1.0},
+        values={"DURATION_UNIT": 1, "DURATION_VALUE": 283, "LEVEL": 1.0},
     )
 
     await light.turn_off()
     light.set_on_time(1000000)
     await light.turn_on()
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU3716619:8",
+    assert mock_client.method_calls[-2] == call.put_paramset(
+        channel_address="VCU3716619:8",
         paramset_key="VALUES",
-        value={"DURATION_UNIT": 2, "DURATION_VALUE": 277, "LEVEL": 1.0},
+        values={"DURATION_UNIT": 2, "DURATION_VALUE": 277, "LEVEL": 1.0},
     )
     await light.turn_on(ramp_time=18)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU3716619:8",
+    assert mock_client.method_calls[-2] == call.put_paramset(
+        channel_address="VCU3716619:8",
         paramset_key="VALUES",
-        value={"RAMP_TIME_VALUE": 18, "LEVEL": 1.0},
+        values={"RAMP_TIME_VALUE": 18, "LEVEL": 1.0},
     )
 
     await light.turn_on(ramp_time=17000)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU3716619:8",
+    assert mock_client.method_calls[-2] == call.put_paramset(
+        channel_address="VCU3716619:8",
         paramset_key="VALUES",
-        value={"RAMP_TIME_UNIT": 1, "RAMP_TIME_VALUE": 283, "LEVEL": 1.0},
+        values={"RAMP_TIME_UNIT": 1, "RAMP_TIME_VALUE": 283, "LEVEL": 1.0},
     )
 
     await light.turn_on(ramp_time=1000000)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU3716619:8",
+    assert mock_client.method_calls[-2] == call.put_paramset(
+        channel_address="VCU3716619:8",
         paramset_key="VALUES",
-        value={"RAMP_TIME_UNIT": 2, "RAMP_TIME_VALUE": 277, "LEVEL": 1.0},
+        values={"RAMP_TIME_UNIT": 2, "RAMP_TIME_VALUE": 277, "LEVEL": 1.0},
     )
 
     await light.turn_on()
     call_count = len(mock_client.method_calls)
     await light.turn_on()
     assert call_count == len(mock_client.method_calls)
 
@@ -460,225 +464,227 @@
         "BILLOW_MIDDLE",
         "BILLOW_FAST",
     )
     assert light.brightness == 0
     assert light.is_on is False
     assert light.color_name == FixedColor.BLACK
     await light.turn_on()
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU4704397:8",
+    assert mock_client.method_calls[-4] == call.put_paramset(
+        channel_address="VCU4704397:8",
         paramset_key="VALUES",
-        value={"COLOR_BEHAVIOUR": 1, "COLOR": 7, "LEVEL": 1.0},
+        values={"COLOR_BEHAVIOUR": 1, "COLOR": 7, "LEVEL": 1.0},
     )
     assert light.brightness == 255
     assert light.color_name == FixedColor.WHITE
 
     await light.turn_on(brightness=100)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU4704397:8",
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU4704397:8",
         paramset_key="VALUES",
-        value={"COLOR_BEHAVIOUR": 1, "LEVEL": 0.39215686274509803},
+        values={"COLOR_BEHAVIOUR": 1, "LEVEL": 0.39215686274509803},
     )
     assert light.brightness == 100
     assert light.color_name == FixedColor.WHITE
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_off()
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU4704397:8", paramset_key="VALUES", parameter="LEVEL", value=0.0
     )
     assert light.brightness == 0
     assert light.color_name == FixedColor.WHITE
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_on(hs_color=(350, 50))
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU4704397:8",
+    assert mock_client.method_calls[-4] == call.put_paramset(
+        channel_address="VCU4704397:8",
         paramset_key="VALUES",
-        value={"COLOR_BEHAVIOUR": 1, "COLOR": 4, "LEVEL": 1.0},
+        values={"COLOR_BEHAVIOUR": 1, "COLOR": 4, "LEVEL": 1.0},
     )
     assert light.brightness == 255
     assert light.color_name == FixedColor.RED
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_on(hs_color=(0.0, 0.0))
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU4704397:8",
+    assert mock_client.method_calls[-4] == call.put_paramset(
+        channel_address="VCU4704397:8",
         paramset_key="VALUES",
-        value={"COLOR_BEHAVIOUR": 1, "COLOR": 7, "LEVEL": 1.0},
+        values={"COLOR_BEHAVIOUR": 1, "COLOR": 7, "LEVEL": 1.0},
     )
     assert light.brightness == 255
     assert light.color_name == FixedColor.WHITE
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_on(hs_color=(60.0, 50.0))
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU4704397:8",
+    assert mock_client.method_calls[-4] == call.put_paramset(
+        channel_address="VCU4704397:8",
         paramset_key="VALUES",
-        value={"COLOR_BEHAVIOUR": 1, "COLOR": 6, "LEVEL": 1.0},
+        values={"COLOR_BEHAVIOUR": 1, "COLOR": 6, "LEVEL": 1.0},
     )
     assert light.brightness == 255
     assert light.color_name == FixedColor.YELLOW
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_on(hs_color=(120, 50))
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU4704397:8",
+    assert mock_client.method_calls[-4] == call.put_paramset(
+        channel_address="VCU4704397:8",
         paramset_key="VALUES",
-        value={"COLOR_BEHAVIOUR": 1, "COLOR": 2, "LEVEL": 1.0},
+        values={"COLOR_BEHAVIOUR": 1, "COLOR": 2, "LEVEL": 1.0},
     )
     assert light.brightness == 255
     assert light.color_name == FixedColor.GREEN
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_on(hs_color=(180, 50))
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU4704397:8",
+    assert mock_client.method_calls[-4] == call.put_paramset(
+        channel_address="VCU4704397:8",
         paramset_key="VALUES",
-        value={"COLOR_BEHAVIOUR": 1, "COLOR": 3, "LEVEL": 1.0},
+        values={"COLOR_BEHAVIOUR": 1, "COLOR": 3, "LEVEL": 1.0},
     )
     assert light.brightness == 255
     assert light.color_name == FixedColor.TURQUOISE
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_on(hs_color=(240, 50))
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU4704397:8",
+    assert mock_client.method_calls[-4] == call.put_paramset(
+        channel_address="VCU4704397:8",
         paramset_key="VALUES",
-        value={"COLOR_BEHAVIOUR": 1, "COLOR": 1, "LEVEL": 1.0},
+        values={"COLOR_BEHAVIOUR": 1, "COLOR": 1, "LEVEL": 1.0},
     )
     assert light.brightness == 255
     assert light.color_name == FixedColor.BLUE
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_on(hs_color=(300, 50))
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU4704397:8",
+    assert mock_client.method_calls[-4] == call.put_paramset(
+        channel_address="VCU4704397:8",
         paramset_key="VALUES",
-        value={"COLOR_BEHAVIOUR": 1, "COLOR": 5, "LEVEL": 1.0},
+        values={"COLOR_BEHAVIOUR": 1, "COLOR": 5, "LEVEL": 1.0},
     )
     assert light.brightness == 255
     assert light.color_name == FixedColor.PURPLE
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_off()
     assert light.brightness == 0
     assert light.color_name == FixedColor.PURPLE
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_on(brightness=100)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU4704397:8",
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU4704397:8",
         paramset_key="VALUES",
-        value={"COLOR_BEHAVIOUR": 1, "LEVEL": 0.39215686274509803},
+        values={"COLOR_BEHAVIOUR": 1, "LEVEL": 0.39215686274509803},
     )
     assert light.brightness == 100
     assert light.color_name == FixedColor.PURPLE
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_on(brightness=33)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU4704397:8",
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU4704397:8",
         paramset_key="VALUES",
-        value={"COLOR_BEHAVIOUR": 1, "LEVEL": 0.12941176470588237},
+        values={"COLOR_BEHAVIOUR": 1, "LEVEL": 0.12941176470588237},
     )
     assert light.brightness == 33
     assert light.color_name == FixedColor.PURPLE
     assert light.effect == ColorBehaviour.ON
 
     await light.turn_on(effect="FLASH_MIDDLE")
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU4704397:8",
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU4704397:8",
         paramset_key="VALUES",
-        value={"COLOR_BEHAVIOUR": 6, "LEVEL": 0.12941176470588237},
+        values={"COLOR_BEHAVIOUR": 6, "LEVEL": 0.12941176470588237},
     )
     assert light.brightness == 33
     assert light.color_name == FixedColor.PURPLE
     assert light.effect == "FLASH_MIDDLE"
 
     await light.turn_on(brightness=66)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU4704397:8",
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU4704397:8",
         paramset_key="VALUES",
-        value={"COLOR_BEHAVIOUR": 6, "LEVEL": 0.25882352941176473},
+        values={"COLOR_BEHAVIOUR": 6, "LEVEL": 0.25882352941176473},
     )
     assert light.brightness == 66
     assert light.color_name == FixedColor.PURPLE
     assert light.effect == "FLASH_MIDDLE"
 
     await light.turn_off()
 
     light.set_on_time(18)
     await light.turn_on()
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU4704397:8",
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU4704397:8",
         paramset_key="VALUES",
-        value={"COLOR_BEHAVIOUR": 6, "DURATION_VALUE": 18, "LEVEL": 1.0},
+        values={"COLOR_BEHAVIOUR": 6, "DURATION_VALUE": 18, "LEVEL": 1.0},
     )
 
     await light.turn_off()
     light.set_on_time(17000)
     await light.turn_on()
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU4704397:8",
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU4704397:8",
         paramset_key="VALUES",
-        value={"COLOR_BEHAVIOUR": 6, "DURATION_UNIT": 1, "DURATION_VALUE": 283, "LEVEL": 1.0},
+        values={"COLOR_BEHAVIOUR": 6, "DURATION_UNIT": 1, "DURATION_VALUE": 283, "LEVEL": 1.0},
     )
 
     await light.turn_off()
     light.set_on_time(1000000)
     await light.turn_on()
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU4704397:8",
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU4704397:8",
         paramset_key="VALUES",
-        value={"COLOR_BEHAVIOUR": 6, "DURATION_UNIT": 2, "DURATION_VALUE": 277, "LEVEL": 1.0},
+        values={"COLOR_BEHAVIOUR": 6, "DURATION_UNIT": 2, "DURATION_VALUE": 277, "LEVEL": 1.0},
     )
     await light.turn_on(ramp_time=18)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU4704397:8",
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU4704397:8",
         paramset_key="VALUES",
-        value={"COLOR_BEHAVIOUR": 6, "RAMP_TIME_VALUE": 18, "LEVEL": 1.0},
+        values={"COLOR_BEHAVIOUR": 6, "RAMP_TIME_VALUE": 18, "LEVEL": 1.0},
     )
 
     await light.turn_on(ramp_time=17000)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU4704397:8",
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU4704397:8",
         paramset_key="VALUES",
-        value={"COLOR_BEHAVIOUR": 6, "RAMP_TIME_UNIT": 1, "RAMP_TIME_VALUE": 283, "LEVEL": 1.0},
+        values={"COLOR_BEHAVIOUR": 6, "RAMP_TIME_UNIT": 1, "RAMP_TIME_VALUE": 283, "LEVEL": 1.0},
     )
 
     await light.turn_on(ramp_time=1000000)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU4704397:8",
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU4704397:8",
         paramset_key="VALUES",
-        value={"COLOR_BEHAVIOUR": 6, "RAMP_TIME_UNIT": 2, "RAMP_TIME_VALUE": 277, "LEVEL": 1.0},
+        values={"COLOR_BEHAVIOUR": 6, "RAMP_TIME_UNIT": 2, "RAMP_TIME_VALUE": 277, "LEVEL": 1.0},
     )
 
     await light.turn_on()
     call_count = len(mock_client.method_calls)
     await light.turn_on()
     assert call_count == len(mock_client.method_calls)
 
     await light.turn_off()
     call_count = len(mock_client.method_calls)
     await light.turn_off()
     assert call_count == len(mock_client.method_calls)
 
     await light.turn_off()
     await light.turn_on(effect="BLINKING_SLOW")
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU4704397:8", paramset_key="VALUES", value={"COLOR_BEHAVIOUR": 2, "LEVEL": 1.0}
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU4704397:8",
+        paramset_key="VALUES",
+        values={"COLOR_BEHAVIOUR": 2, "LEVEL": 1.0},
     )
 
     await light.turn_on(brightness=28)
     await light.turn_on(effect="FLASH_MIDDLE")
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU4704397:8",
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU4704397:8",
         paramset_key="VALUES",
-        value={"COLOR_BEHAVIOUR": 6, "LEVEL": 0.10980392156862745},
+        values={"COLOR_BEHAVIOUR": 6, "LEVEL": 0.10980392156862745},
     )
 
 
 async def test_ceiprgbwlight(factory: helper.Factory) -> None:
     """Test CeIpRGBWLight."""
     central, mock_client = await factory.get_default_central(TEST_DEVICES)
     light: CeIpRGBWLight = cast(
@@ -716,38 +722,38 @@
         "EFFECT_10_END_CURRENT_PROFILE",
         "EFFECT_10_INTERRUPT_CURRENT_PROFILE",
     )
 
     assert light.brightness == 0
 
     await light.turn_on()
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU5629873:1", paramset_key="VALUES", parameter="LEVEL", value=1.0
     )
     assert light.brightness == 255
     await light.turn_on(brightness=28)
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU5629873:1",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=0.10980392156862745,
     )
     assert light.brightness == 28
     await light.turn_off()
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU5629873:1", paramset_key="VALUES", parameter="LEVEL", value=0.0
     )
     assert light.brightness == 0
 
     assert light.color_temp is None
     await light.turn_on(color_temp=300)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU5629873:1",
+    assert mock_client.method_calls[-3] == call.put_paramset(
+        channel_address="VCU5629873:1",
         paramset_key="VALUES",
-        value={"COLOR_TEMPERATURE": 3333, "LEVEL": 1.0},
+        values={"COLOR_TEMPERATURE": 3333, "LEVEL": 1.0},
     )
     assert light.color_temp == 300
 
     await light.turn_on()
     call_count = len(mock_client.method_calls)
     await light.turn_on()
     assert call_count == len(mock_client.method_calls)
@@ -755,39 +761,39 @@
     await light.turn_off()
     call_count = len(mock_client.method_calls)
     await light.turn_off()
     assert call_count == len(mock_client.method_calls)
 
     assert light.hs_color is None
     await light.turn_on(hs_color=(44.4, 69.3))
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU5629873:1",
+    assert mock_client.method_calls[-4] == call.put_paramset(
+        channel_address="VCU5629873:1",
         paramset_key="VALUES",
-        value={"HUE": 44, "SATURATION": 0.693, "LEVEL": 1.0},
+        values={"HUE": 44, "SATURATION": 0.693, "LEVEL": 1.0},
     )
     assert light.hs_color == (44, 69.3)
 
     await light.turn_on(hs_color=(0, 50))
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU5629873:1",
+    assert mock_client.method_calls[-4] == call.put_paramset(
+        channel_address="VCU5629873:1",
         paramset_key="VALUES",
-        value={"HUE": 0, "SATURATION": 0.5, "LEVEL": 1.0},
+        values={"HUE": 0, "SATURATION": 0.5, "LEVEL": 1.0},
     )
     assert light.hs_color == (0.0, 50.0)
 
     await light.turn_on(effect="EFFECT_01_END_CURRENT_PROFILE")
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU5629873:1", paramset_key="VALUES", value={"EFFECT": 1, "LEVEL": 1.0}
+    assert mock_client.method_calls[-2] == call.put_paramset(
+        channel_address="VCU5629873:1", paramset_key="VALUES", values={"EFFECT": 1, "LEVEL": 1.0}
     )
 
     await light.turn_on(hs_color=(44, 66), ramp_time=5)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU5629873:1",
+    assert mock_client.method_calls[-4] == call.put_paramset(
+        channel_address="VCU5629873:1",
         paramset_key=ParamsetKey.VALUES,
-        value={
+        values={
             "HUE": 44,
             "SATURATION": 0.66,
             "DURATION_VALUE": 111600,
             "RAMP_TIME_VALUE": 5,
             "LEVEL": 1.0,
         },
     )
@@ -808,55 +814,55 @@
     assert light.supports_hs_color is True
     assert light.supports_transition is True
     assert light.effect is None
 
     assert light.brightness == 0
     assert light.brightness_pct == 0
     await light.turn_on()
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU9973336:13", paramset_key="VALUES", parameter="LEVEL", value=1.0
     )
     assert light.brightness == 255
     await light.turn_on(brightness=28)
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU9973336:13",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=0.10980392156862745,
     )
     assert light.brightness == 28
     await light.turn_off()
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU9973336:13", paramset_key="VALUES", parameter="LEVEL", value=0.0
     )
     assert light.brightness == 0
 
     assert light.hs_color == (0.0, 0.0)
     await light.turn_on(hs_color=(44.4, 69.3))
-    assert mock_client.method_calls[-2] == call.set_value(
+    assert mock_client.method_calls[-4] == call.set_value(
         channel_address="VCU9973336:15", paramset_key="VALUES", parameter="COLOR", value=25
     )
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU9973336:13", paramset_key="VALUES", parameter="LEVEL", value=1.0
     )
     assert light.hs_color == (45.0, 100)
 
     await light.turn_on(hs_color=(0, 50))
-    assert mock_client.method_calls[-2] == call.set_value(
+    assert mock_client.method_calls[-4] == call.set_value(
         channel_address="VCU9973336:15", paramset_key="VALUES", parameter="COLOR", value=0
     )
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU9973336:13", paramset_key="VALUES", parameter="LEVEL", value=1.0
     )
     assert light.hs_color == (0.0, 100.0)
     await light.turn_on(hs_color=(0, 1))
-    assert mock_client.method_calls[-2] == call.set_value(
+    assert mock_client.method_calls[-4] == call.set_value(
         channel_address="VCU9973336:15", paramset_key="VALUES", parameter="COLOR", value=200
     )
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU9973336:13", paramset_key="VALUES", parameter="LEVEL", value=1.0
     )
     assert light.hs_color == (0.0, 0.0)
     await central.event(const.INTERFACE_ID, "VCU9973336:15", "COLOR", 201)
     assert light.hs_color == (0.0, 0.0)
     await central.event(const.INTERFACE_ID, "VCU9973336:15", "COLOR", None)
     assert light.hs_color == (0.0, 0.0)
```

### Comparing `hahomematic-2024.4.7/tests/test_lock.py` & `hahomematic-2024.4.8/tests/test_lock.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,23 +25,23 @@
     """Test CeRfLock."""
     central, mock_client = await factory.get_default_central(TEST_DEVICES)
     lock: CeRfLock = cast(CeRfLock, helper.get_prepared_custom_entity(central, "VCU0000146", 1))
     assert lock.usage == EntityUsage.CE_PRIMARY
 
     assert lock.is_locked is True
     await lock.unlock()
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU0000146:1",
         paramset_key="VALUES",
         parameter="STATE",
         value=True,
     )
     assert lock.is_locked is False
     await lock.lock()
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU0000146:1",
         paramset_key="VALUES",
         parameter="STATE",
         value=False,
     )
     assert lock.is_locked is True
     await lock.open()
```

### Comparing `hahomematic-2024.4.7/tests/test_number.py` & `hahomematic-2024.4.8/tests/test_number.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         central.get_generic_entity("VCU0000011:3", "LEVEL"),
     )
     assert efloat.usage == EntityUsage.NO_CREATE
     assert efloat.unit == "%"
     assert efloat.values is None
     assert efloat.value is None
     await efloat.send_value(0.3)
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU0000011:3",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=0.3,
     )
     assert efloat.value == 0.3
     await central.event(const.INTERFACE_ID, "VCU0000011:3", "LEVEL", 0.5)
@@ -62,24 +62,24 @@
         central.get_generic_entity("VCU0000054:2", "SETPOINT"),
     )
     assert efloat.usage == EntityUsage.NO_CREATE
     assert efloat.unit == "°C"
     assert efloat.values is None
     assert efloat.value is None
     await efloat.send_value(8.0)
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU0000054:2",
         paramset_key="VALUES",
         parameter="SETPOINT",
         value=8.0,
     )
     assert efloat.value == 8.0
 
     await efloat.send_value("VENT_OPEN")
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU0000054:2",
         paramset_key="VALUES",
         parameter="SETPOINT",
         value=100.0,
     )
     assert efloat.value == 100.0
 
@@ -95,24 +95,24 @@
     assert einteger.usage == EntityUsage.NO_CREATE
     assert einteger.unit is None
     assert einteger.min == 0
     assert einteger.max == 3
     assert einteger.values is None
     assert einteger.value is None
     await einteger.send_value(3)
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU4984404:1",
         paramset_key="VALUES",
         parameter="SET_POINT_MODE",
         value=3,
     )
     assert einteger.value == 3
 
     await einteger.send_value(1.0)
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU4984404:1",
         paramset_key="VALUES",
         parameter="SET_POINT_MODE",
         value=1,
     )
     assert einteger.value == 1
```

### Comparing `hahomematic-2024.4.7/tests/test_select.py` & `hahomematic-2024.4.8/tests/test_select.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,30 +31,30 @@
     assert select.usage == EntityUsage.NO_CREATE
     assert select.unit is None
     assert select.min == "CLOSED"
     assert select.max == "OPEN"
     assert select.values == ("CLOSED", "OPEN")
     assert select.value == "CLOSED"
     await select.send_value("OPEN")
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU6354483:1",
         paramset_key="VALUES",
         parameter="WINDOW_STATE",
         value=1,
     )
     assert select.value == "OPEN"
     await central.event(const.INTERFACE_ID, "VCU6354483:1", "WINDOW_STATE", 0)
     assert select.value == "CLOSED"
 
     await select.send_value(3)
     # do not write. value above max
     assert select.value == "CLOSED"
 
     await select.send_value(1)
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU6354483:1",
         paramset_key="VALUES",
         parameter="WINDOW_STATE",
         value=1,
     )
     # do not write. value above max
     assert select.value == "OPEN"
```

### Comparing `hahomematic-2024.4.7/tests/test_sensor.py` & `hahomematic-2024.4.8/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/tests/test_siren.py` & `hahomematic-2024.4.8/tests/test_siren.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,33 +39,33 @@
 
     await siren.turn_on(
         acoustic_alarm="FREQUENCY_RISING_AND_FALLING",
         optical_alarm="BLINKING_ALTERNATELY_REPEATING",
         duration=30,
     )
     assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU8249617:3",
+        channel_address="VCU8249617:3",
         paramset_key="VALUES",
-        value={
+        values={
             "ACOUSTIC_ALARM_SELECTION": 3,
             "OPTICAL_ALARM_SELECTION": 1,
             "DURATION_UNIT": 0,
             "DURATION_VALUE": 30,
         },
     )
 
     await siren.turn_on(
         acoustic_alarm="FREQUENCY_RISING_AND_FALLING",
         optical_alarm="BLINKING_ALTERNATELY_REPEATING",
         duration=30,
     )
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU8249617:3",
+    assert mock_client.method_calls[-2] == call.put_paramset(
+        channel_address="VCU8249617:3",
         paramset_key="VALUES",
-        value={
+        values={
             "ACOUSTIC_ALARM_SELECTION": 3,
             "OPTICAL_ALARM_SELECTION": 1,
             "DURATION_UNIT": 0,
             "DURATION_VALUE": 30,
         },
     )
 
@@ -81,17 +81,17 @@
             acoustic_alarm="FREQUENCY_RISING_AND_FALLING",
             optical_alarm="not_in_list",
             duration=30,
         )
 
     await siren.turn_off()
     assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU8249617:3",
+        channel_address="VCU8249617:3",
         paramset_key="VALUES",
-        value={
+        values={
             "ACOUSTIC_ALARM_SELECTION": 0,
             "OPTICAL_ALARM_SELECTION": 0,
             "DURATION_UNIT": 0,
             "DURATION_VALUE": 0,
         },
     )
```

### Comparing `hahomematic-2024.4.7/tests/test_support.py` & `hahomematic-2024.4.8/tests/test_support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.7/tests/test_switch.py` & `hahomematic-2024.4.8/tests/test_switch.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,34 +28,38 @@
     switch: CeSwitch = cast(CeSwitch, helper.get_prepared_custom_entity(central, "VCU2128127", 4))
     assert switch.usage == EntityUsage.CE_PRIMARY
 
     await switch.turn_off()
     assert switch.value is False
     assert switch.channel_value is False
     await switch.turn_on()
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU2128127:4", paramset_key="VALUES", parameter="STATE", value=True
     )
     assert switch.value is True
     await switch.turn_off()
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU2128127:4", paramset_key="VALUES", parameter="STATE", value=False
     )
     assert switch.value is False
     await switch.turn_on(on_time=60)
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU2128127:4", paramset_key="VALUES", value={"ON_TIME": 60.0, "STATE": True}
+    assert mock_client.method_calls[-2] == call.put_paramset(
+        channel_address="VCU2128127:4",
+        paramset_key="VALUES",
+        values={"ON_TIME": 60.0, "STATE": True},
     )
     assert switch.value is True
 
     await switch.turn_off()
     switch.set_on_time(35.4)
     await switch.turn_on()
-    assert mock_client.method_calls[-1] == call.put_paramset(
-        address="VCU2128127:4", paramset_key="VALUES", value={"ON_TIME": 35.4, "STATE": True}
+    assert mock_client.method_calls[-2] == call.put_paramset(
+        channel_address="VCU2128127:4",
+        paramset_key="VALUES",
+        values={"ON_TIME": 35.4, "STATE": True},
     )
 
     await switch.turn_on()
     call_count = len(mock_client.method_calls)
     await switch.turn_on()
     assert call_count == len(mock_client.method_calls)
 
@@ -70,37 +74,37 @@
     """Test HmSwitch."""
     central, mock_client = await factory.get_default_central(TEST_DEVICES)
     switch: HmSwitch = cast(HmSwitch, central.get_generic_entity("VCU2128127:4", "STATE"))
     assert switch.usage == EntityUsage.NO_CREATE
 
     assert switch.value is None
     await switch.turn_on()
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU2128127:4",
         paramset_key="VALUES",
         parameter="STATE",
         value=True,
     )
     assert switch.value is True
     await switch.turn_off()
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU2128127:4",
         paramset_key="VALUES",
         parameter="STATE",
         value=False,
     )
     assert switch.value is False
     await switch.turn_on(on_time=60)
-    assert mock_client.method_calls[-2] == call.set_value(
+    assert mock_client.method_calls[-3] == call.set_value(
         channel_address="VCU2128127:4",
         paramset_key="VALUES",
         parameter="ON_TIME",
         value=60.0,
     )
-    assert mock_client.method_calls[-1] == call.set_value(
+    assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU2128127:4",
         paramset_key="VALUES",
         parameter="STATE",
         value=True,
     )
     assert switch.value is True
     await switch.set_on_time(35.4)
```

### Comparing `hahomematic-2024.4.7/tests/test_text.py` & `hahomematic-2024.4.8/tests/test_text.py`

 * *Files identical despite different names*

