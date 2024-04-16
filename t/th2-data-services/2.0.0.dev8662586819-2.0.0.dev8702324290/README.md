# Comparing `tmp/th2_data_services-2.0.0.dev8662586819.tar.gz` & `tmp/th2_data_services-2.0.0.dev8702324290.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services-2.0.0.dev8662586819.tar", last modified: Fri Apr 12 13:10:30 2024, max compression
+gzip compressed data, was "dist/th2_data_services-2.0.0.dev8702324290.tar", last modified: Tue Apr 16 08:23:11 2024, max compression
```

## Comparing `th2_data_services-2.0.0.dev8662586819.tar` & `th2_data_services-2.0.0.dev8702324290.tar`

### file list

```diff
@@ -1,79 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    36010 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    29605 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-12 13:10:20.000000 th2_data_services-2.0.0.dev8662586819/package_info.json
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/_internal/perf_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/config/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    42456 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/etc_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    16095 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/event_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    26153 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/parent_event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/utils/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/_is_sorted_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    16455 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/aggregation_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/az_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/categorizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/decode_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/totals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/experimental.py
--rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/json_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/message_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/message_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/message_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/message_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22242 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/path_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/perfect_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    28895 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/script_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/sse_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/stream_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/stream_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/stream_utils/stream_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/total_category_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/viewer_structs/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/viewer_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/viewer_structs/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    36010 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    35047 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 08:22:58.000000 th2_data_services-2.0.0.dev8702324290/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/_internal/perf_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41567 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/dummy/data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/etc_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/event_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26246 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/parent_event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/utils/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/_is_sorted_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16455 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/aggregation_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/az_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/categorizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/decode_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/totals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/json_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/message_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/message_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/message_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/message_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22242 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/path_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/perfect_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28895 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/script_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/sse_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/stream_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/stream_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/stream_utils/stream_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/total_category_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/viewer_structs/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/viewer_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/viewer_structs/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services.egg-info/top_level.txt
```

### Comparing `th2_data_services-2.0.0.dev8662586819/PKG-INFO` & `th2_data_services-2.0.0.dev8702324290/th2_data_services.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 325f  : 2.1.Name: th2_
-00000020: 6461 7461 5f73 6572 7669 6365 730a 5665  data_services.Ve
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 322d  : 2.1.Name: th2-
+00000020: 6461 7461 2d73 6572 7669 6365 730a 5665  data-services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3836 3632 3538 3638 3139 0a53 756d 6d61  8662586819.Summa
+00000040: 3837 3032 3332 3432 3930 0a53 756d 6d61  8702324290.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
@@ -316,1936 +316,2347 @@
 000013b0: 6174 6574 696d 6520 696d 706f 7274 2064  atetime import d
 000013c0: 6174 6574 696d 650a 2020 2020 2020 2020  atetime.        
 000013d0: 0a20 2020 2020 2020 2066 726f 6d20 7468  .        from th
 000013e0: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
 000013f0: 6461 7461 2069 6d70 6f72 7420 4461 7461  data import Data
 00001400: 0a20 2020 2020 2020 2066 726f 6d20 7468  .        from th
 00001410: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
-00001420: 6576 656e 745f 7472 6565 2069 6d70 6f72  event_tree impor
-00001430: 7420 280a 2020 2020 2020 2020 2020 2020  t (.            
-00001440: 4576 656e 7454 7265 652c 0a20 2020 2020  EventTree,.     
-00001450: 2020 2020 2020 2045 7665 6e74 5472 6565         EventTree
-00001460: 436f 6c6c 6563 7469 6f6e 2c0a 2020 2020  Collection,.    
-00001470: 2020 2020 2020 2020 5061 7265 6e74 4576          ParentEv
-00001480: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
-00001490: 6e2c 0a20 2020 2020 2020 2020 2020 2049  n,.            I
-000014a0: 4554 4344 7269 7665 722c 0a20 2020 2020  ETCDriver,.     
-000014b0: 2020 2029 0a20 2020 2020 2020 2066 726f     ).        fro
-000014c0: 6d20 7468 325f 6461 7461 5f73 6572 7669  m th2_data_servi
-000014d0: 6365 732e 696e 7465 7266 6163 6573 2069  ces.interfaces i
-000014e0: 6d70 6f72 7420 4944 6174 6153 6f75 7263  mport IDataSourc
-000014f0: 650a 2020 2020 2020 2020 6672 6f6d 2074  e.        from t
-00001500: 6832 5f64 6174 615f 7365 7276 6963 6573  h2_data_services
-00001510: 2e75 7469 6c73 2e63 6f6e 7665 7274 6572  .utils.converter
-00001520: 7320 696d 706f 7274 2028 0a20 2020 2020  s import (.     
-00001530: 2020 2020 2020 2044 6174 6574 696d 6543         DatetimeC
-00001540: 6f6e 7665 7274 6572 2c0a 2020 2020 2020  onverter,.      
-00001550: 2020 2020 2020 4461 7465 7469 6d65 5374        DatetimeSt
-00001560: 7269 6e67 436f 6e76 6572 7465 722c 0a20  ringConverter,. 
-00001570: 2020 2020 2020 2020 2020 2050 726f 746f             Proto
-00001580: 6275 6654 696d 6573 7461 6d70 436f 6e76  bufTimestampConv
-00001590: 6572 7465 722c 0a20 2020 2020 2020 2020  erter,.         
-000015a0: 2020 2054 6832 5469 6d65 7374 616d 7043     Th2TimestampC
-000015b0: 6f6e 7665 7274 6572 2c0a 2020 2020 2020  onverter,.      
-000015c0: 2020 290a 2020 2020 2020 2020 0a20 2020    ).        .   
-000015d0: 2020 2020 2023 205b 305d 204c 6962 2063       # [0] Lib c
-000015e0: 6f6e 6669 6775 7261 7469 6f6e 0a20 2020  onfiguration.   
-000015f0: 2020 2020 2023 205b 302e 315d 2049 6e74       # [0.1] Int
-00001600: 6572 6163 7469 7665 206f 7220 5363 7269  eractive or Scri
-00001610: 7074 206d 6f64 650a 2020 2020 2020 2020  pt mode.        
-00001620: 2320 4966 2079 6f75 2075 7365 2074 6865  # If you use the
-00001630: 206c 6962 2069 6e20 696e 7465 7261 6374   lib in interact
-00001640: 6976 6520 6d6f 6465 2028 6a75 7079 7465  ive mode (jupyte
-00001650: 722c 2069 7079 7468 6f6e 2920 6974 2773  r, ipython) it's
-00001660: 2072 6563 6f6d 6d65 6e64 6564 2074 6f20   recommended to 
-00001670: 7365 7420 7468 6520 7370 6563 6961 6c0a  set the special.
-00001680: 2020 2020 2020 2020 2320 676c 6f62 616c          # global
-00001690: 2070 6172 616d 6574 6572 2074 6f20 5472   parameter to Tr
-000016a0: 7565 2e20 4974 276c 6c20 6b65 6570 2063  ue. It'll keep c
-000016b0: 6163 6865 2066 696c 6573 2069 6620 736f  ache files if so
-000016c0: 6d65 7468 696e 6720 7765 6e74 2077 726f  mething went wro
-000016d0: 6e67 2e0a 2020 2020 2020 2020 6672 6f6d  ng..        from
-000016e0: 2074 6832 5f64 6174 615f 7365 7276 6963   th2_data_servic
-000016f0: 6573 2e63 6f6e 6669 6720 696d 706f 7274  es.config import
-00001700: 206f 7074 696f 6e73 0a20 2020 2020 2020   options.       
-00001710: 200a 2020 2020 2020 2020 6f70 7469 6f6e   .        option
-00001720: 732e 494e 5445 5241 4354 4956 455f 4d4f  s.INTERACTIVE_MO
-00001730: 4445 203d 2054 7275 650a 2020 2020 2020  DE = True.      
-00001740: 2020 0a20 2020 2020 2020 2023 2053 6f6d    .        # Som
-00001750: 6520 6578 616d 706c 6520 6461 7461 0a20  e example data. 
-00001760: 2020 2020 2020 2065 7665 6e74 7320 3d20         events = 
-00001770: 4461 7461 280a 2020 2020 2020 2020 2020  Data(.          
-00001780: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
-00001790: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-000017a0: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
-000017b0: 4964 223a 2022 6465 6d6f 5f62 6f6f 6b5f  Id": "demo_book_
-000017c0: 313a 7468 322d 7363 6f70 653a 3230 3233  1:th2-scope:2023
-000017d0: 3031 3035 3133 3537 3035 3536 3038 3733  0105135705560873
-000017e0: 3030 303a 6436 3165 3933 3061 2d38 6430  000:d61e930a-8d0
-000017f0: 302d 3131 6564 2d61 6131 612d 6433 3461  0-11ed-aa1a-d34a
-00001800: 3631 3535 3135 3264 5f31 222c 0a20 2020  6155152d_1",.   
-00001810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001820: 2022 6261 7463 6849 6422 3a20 4e6f 6e65   "batchId": None
-00001830: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001840: 2020 2020 2020 2269 7342 6174 6368 6564        "isBatched
-00001850: 223a 2046 616c 7365 2c0a 2020 2020 2020  ": False,.      
-00001860: 2020 2020 2020 2020 2020 2020 2020 2265                "e
-00001870: 7665 6e74 4e61 6d65 223a 2022 5365 7420  ventName": "Set 
-00001880: 6f66 2061 7574 6f2d 6765 6e65 7261 7465  of auto-generate
-00001890: 6420 6576 656e 7473 2066 6f72 2064 7320  d events for ds 
-000018a0: 6c69 6220 7465 7374 696e 6722 2c0a 2020  lib testing",.  
+00001420: 6475 6d6d 7920 696d 706f 7274 2044 756d  dummy import Dum
+00001430: 6d79 4461 7461 536f 7572 6365 0a20 2020  myDataSource.   
+00001440: 2020 2020 2066 726f 6d20 7468 325f 6461       from th2_da
+00001450: 7461 5f73 6572 7669 6365 732e 6576 656e  ta_services.even
+00001460: 745f 7472 6565 2069 6d70 6f72 7420 280a  t_tree import (.
+00001470: 2020 2020 2020 2020 2020 2020 4576 656e              Even
+00001480: 7454 7265 652c 0a20 2020 2020 2020 2020  tTree,.         
+00001490: 2020 2045 7665 6e74 5472 6565 436f 6c6c     EventTreeColl
+000014a0: 6563 7469 6f6e 2c0a 2020 2020 2020 2020  ection,.        
+000014b0: 2020 2020 5061 7265 6e74 4576 656e 7454      ParentEventT
+000014c0: 7265 6543 6f6c 6c65 6374 696f 6e2c 0a20  reeCollection,. 
+000014d0: 2020 2020 2020 2020 2020 2049 4554 4344             IETCD
+000014e0: 7269 7665 722c 0a20 2020 2020 2020 2029  river,.        )
+000014f0: 0a20 2020 2020 2020 2066 726f 6d20 7468  .        from th
+00001500: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
+00001510: 696e 7465 7266 6163 6573 2069 6d70 6f72  interfaces impor
+00001520: 7420 4944 6174 6153 6f75 7263 650a 2020  t IDataSource.  
+00001530: 2020 2020 2020 6672 6f6d 2074 6832 5f64        from th2_d
+00001540: 6174 615f 7365 7276 6963 6573 2e75 7469  ata_services.uti
+00001550: 6c73 2e63 6f6e 7665 7274 6572 7320 696d  ls.converters im
+00001560: 706f 7274 2028 0a20 2020 2020 2020 2020  port (.         
+00001570: 2020 2044 6174 6574 696d 6543 6f6e 7665     DatetimeConve
+00001580: 7274 6572 2c0a 2020 2020 2020 2020 2020  rter,.          
+00001590: 2020 4461 7465 7469 6d65 5374 7269 6e67    DatetimeString
+000015a0: 436f 6e76 6572 7465 722c 0a20 2020 2020  Converter,.     
+000015b0: 2020 2020 2020 2050 726f 746f 6275 6654         ProtobufT
+000015c0: 696d 6573 7461 6d70 436f 6e76 6572 7465  imestampConverte
+000015d0: 722c 0a20 2020 2020 2020 2020 2020 2054  r,.            T
+000015e0: 6832 5469 6d65 7374 616d 7043 6f6e 7665  h2TimestampConve
+000015f0: 7274 6572 2c0a 2020 2020 2020 2020 290a  rter,.        ).
+00001600: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001610: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
+00001620: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001630: 2323 2323 2323 230a 2020 2020 2020 2020  #######.        
+00001640: 2320 5b30 5d20 4c69 6220 636f 6e66 6967  # [0] Lib config
+00001650: 7572 6174 696f 6e0a 2020 2020 2020 2020  uration.        
+00001660: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001670: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001680: 2323 2323 2323 0a20 2020 2020 2020 200a  ######.        .
+00001690: 2020 2020 2020 2020 2320 5b30 2e31 5d20          # [0.1] 
+000016a0: 496e 7465 7261 6374 6976 6520 6f72 2053  Interactive or S
+000016b0: 6372 6970 7420 6d6f 6465 0a20 2020 2020  cript mode.     
+000016c0: 2020 2023 2049 6620 796f 7520 7573 6520     # If you use 
+000016d0: 7468 6520 6c69 6220 696e 2069 6e74 6572  the lib in inter
+000016e0: 6163 7469 7665 206d 6f64 6520 286a 7570  active mode (jup
+000016f0: 7974 6572 2c20 6970 7974 686f 6e29 2069  yter, ipython) i
+00001700: 7427 7320 7265 636f 6d6d 656e 6465 6420  t's recommended 
+00001710: 746f 2073 6574 2074 6865 2073 7065 6369  to set the speci
+00001720: 616c 0a20 2020 2020 2020 2023 2067 6c6f  al.        # glo
+00001730: 6261 6c20 7061 7261 6d65 7465 7220 746f  bal parameter to
+00001740: 2054 7275 652e 2049 7427 6c6c 206b 6565   True. It'll kee
+00001750: 7020 6361 6368 6520 6669 6c65 7320 6966  p cache files if
+00001760: 2073 6f6d 6574 6869 6e67 2077 656e 7420   something went 
+00001770: 7772 6f6e 672e 0a20 2020 2020 2020 2066  wrong..        f
+00001780: 726f 6d20 7468 325f 6461 7461 5f73 6572  rom th2_data_ser
+00001790: 7669 6365 732e 636f 6e66 6967 2069 6d70  vices.config imp
+000017a0: 6f72 7420 6f70 7469 6f6e 730a 2020 2020  ort options.    
+000017b0: 2020 2020 0a20 2020 2020 2020 206f 7074      .        opt
+000017c0: 696f 6e73 2e49 4e54 4552 4143 5449 5645  ions.INTERACTIVE
+000017d0: 5f4d 4f44 4520 3d20 5472 7565 0a20 2020  _MODE = True.   
+000017e0: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+000017f0: 536f 6d65 2065 7861 6d70 6c65 2064 6174  Some example dat
+00001800: 610a 2020 2020 2020 2020 6576 656e 7473  a.        events
+00001810: 203d 2044 6174 6128 0a20 2020 2020 2020   = Data(.       
+00001820: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
+00001830: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00001840: 2020 2020 2020 2020 2020 2020 2022 6576               "ev
+00001850: 656e 7449 6422 3a20 2264 656d 6f5f 626f  entId": "demo_bo
+00001860: 6f6b 5f31 3a74 6832 2d73 636f 7065 3a32  ok_1:th2-scope:2
+00001870: 3032 3330 3130 3531 3335 3730 3535 3630  0230105135705560
+00001880: 3837 3330 3030 3a64 3631 6539 3330 612d  873000:d61e930a-
+00001890: 3864 3030 2d31 3165 642d 6161 3161 2d64  8d00-11ed-aa1a-d
+000018a0: 3334 6136 3135 3531 3532 645f 3122 2c0a  34a6155152d_1",.
 000018b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018c0: 2020 2265 7665 6e74 5479 7065 223a 2022    "eventType": "
-000018d0: 6473 2d6c 6962 2d74 6573 742d 6576 656e  ds-lib-test-even
-000018e0: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-000018f0: 2020 2020 2020 2020 2265 6e64 5469 6d65          "endTime
-00001900: 7374 616d 7022 3a20 7b22 6570 6f63 6853  stamp": {"epochS
-00001910: 6563 6f6e 6422 3a20 3136 3732 3932 3730  econd": 16729270
-00001920: 3235 2c20 226e 616e 6f22 3a20 3536 3137  25, "nano": 5617
-00001930: 3531 3030 307d 2c0a 2020 2020 2020 2020  51000},.        
-00001940: 2020 2020 2020 2020 2020 2020 2273 7461              "sta
-00001950: 7274 5469 6d65 7374 616d 7022 3a20 7b22  rtTimestamp": {"
-00001960: 6570 6f63 6853 6563 6f6e 6422 3a20 3136  epochSecond": 16
-00001970: 3732 3932 3730 3235 2c20 226e 616e 6f22  72927025, "nano"
-00001980: 3a20 3536 3038 3733 3030 307d 2c0a 2020  : 560873000},.  
-00001990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019a0: 2020 2270 6172 656e 7445 7665 6e74 4964    "parentEventId
-000019b0: 223a 204e 6f6e 652c 0a20 2020 2020 2020  ": None,.       
-000019c0: 2020 2020 2020 2020 2020 2020 2022 7375               "su
-000019d0: 6363 6573 7366 756c 223a 2054 7275 652c  ccessful": True,
-000019e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000019f0: 2020 2020 2022 626f 6f6b 4964 223a 2022       "bookId": "
-00001a00: 6465 6d6f 5f62 6f6f 6b5f 3122 2c0a 2020  demo_book_1",.  
-00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a20: 2020 2273 636f 7065 223a 2022 7468 322d    "scope": "th2-
-00001a30: 7363 6f70 6522 2c0a 2020 2020 2020 2020  scope",.        
-00001a40: 2020 2020 2020 2020 2020 2020 2261 7474              "att
-00001a50: 6163 6865 644d 6573 7361 6765 4964 7322  achedMessageIds"
-00001a60: 3a20 5b5d 2c0a 2020 2020 2020 2020 2020  : [],.          
-00001a70: 2020 2020 2020 2020 2020 2262 6f64 7922            "body"
-00001a80: 3a20 5b5d 2c0a 2020 2020 2020 2020 2020  : [],.          
-00001a90: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00001aa0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-00001ab0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001ac0: 6576 656e 7449 6422 3a20 2264 656d 6f5f  eventId": "demo_
-00001ad0: 626f 6f6b 5f31 3a74 6832 2d73 636f 7065  book_1:th2-scope
-00001ae0: 3a32 3032 3330 3130 3531 3335 3730 3535  :202301051357055
-00001af0: 3633 3532 3230 3030 3a39 6164 6262 3365  63522000:9adbb3e
-00001b00: 302d 3566 3862 2d34 6332 382d 6132 6163  0-5f8b-4c28-a2ac
-00001b10: 2d37 3336 3165 3866 6137 3034 633e 6465  -7361e8fa704c>de
-00001b20: 6d6f 5f62 6f6f 6b5f 313a 7468 322d 7363  mo_book_1:th2-sc
-00001b30: 6f70 653a 3230 3233 3031 3035 3133 3537  ope:202301051357
-00001b40: 3035 3536 3335 3232 3030 303a 6436 3165  05563522000:d61e
-00001b50: 3933 3061 2d38 6430 302d 3131 6564 2d61  930a-8d00-11ed-a
-00001b60: 6131 612d 6433 3461 3631 3535 3135 3264  a1a-d34a6155152d
-00001b70: 5f32 222c 0a20 2020 2020 2020 2020 2020  _2",.           
-00001b80: 2020 2020 2020 2020 2022 6261 7463 6849           "batchI
-00001b90: 6422 3a20 2264 656d 6f5f 626f 6f6b 5f31  d": "demo_book_1
-00001ba0: 3a74 6832 2d73 636f 7065 3a32 3032 3330  :th2-scope:20230
-00001bb0: 3130 3531 3335 3730 3535 3633 3532 3230  1051357055635220
-00001bc0: 3030 3a39 6164 6262 3365 302d 3566 3862  00:9adbb3e0-5f8b
-00001bd0: 2d34 6332 382d 6132 6163 2d37 3336 3165  -4c28-a2ac-7361e
-00001be0: 3866 6137 3034 6322 2c0a 2020 2020 2020  8fa704c",.      
-00001bf0: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-00001c00: 7342 6174 6368 6564 223a 2054 7275 652c  sBatched": True,
-00001c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001c20: 2020 2020 2022 6576 656e 744e 616d 6522       "eventName"
-00001c30: 3a20 2250 6c61 696e 2065 7665 6e74 2031  : "Plain event 1
-00001c40: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00001c50: 2020 2020 2020 2022 6576 656e 7454 7970         "eventTyp
-00001c60: 6522 3a20 2264 732d 6c69 622d 7465 7374  e": "ds-lib-test
-00001c70: 2d65 7665 6e74 222c 0a20 2020 2020 2020  -event",.       
-00001c80: 2020 2020 2020 2020 2020 2020 2022 656e               "en
-00001c90: 6454 696d 6573 7461 6d70 223a 207b 2265  dTimestamp": {"e
-00001ca0: 706f 6368 5365 636f 6e64 223a 2031 3637  pochSecond": 167
-00001cb0: 3239 3237 3032 352c 2022 6e61 6e6f 223a  2927025, "nano":
-00001cc0: 2035 3633 3634 3030 3030 7d2c 0a20 2020   563640000},.   
-00001cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ce0: 2022 7374 6172 7454 696d 6573 7461 6d70   "startTimestamp
-00001cf0: 223a 207b 2265 706f 6368 5365 636f 6e64  ": {"epochSecond
-00001d00: 223a 2031 3637 3239 3237 3032 352c 2022  ": 1672927025, "
-00001d10: 6e61 6e6f 223a 2035 3633 3532 3230 3030  nano": 563522000
-00001d20: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00001d30: 2020 2020 2020 2022 7061 7265 6e74 4576         "parentEv
-00001d40: 656e 7449 6422 3a20 2264 656d 6f5f 626f  entId": "demo_bo
-00001d50: 6f6b 5f31 3a74 6832 2d73 636f 7065 3a32  ok_1:th2-scope:2
-00001d60: 3032 3330 3130 3531 3335 3730 3535 3630  0230105135705560
-00001d70: 3837 3330 3030 3a64 3631 6539 3330 612d  873000:d61e930a-
-00001d80: 3864 3030 2d31 3165 642d 6161 3161 2d64  8d00-11ed-aa1a-d
-00001d90: 3334 6136 3135 3531 3532 645f 3122 2c0a  34a6155152d_1",.
-00001da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001db0: 2020 2020 2273 7563 6365 7373 6675 6c22      "successful"
-00001dc0: 3a20 5472 7565 2c0a 2020 2020 2020 2020  : True,.        
-00001dd0: 2020 2020 2020 2020 2020 2020 2262 6f6f              "boo
-00001de0: 6b49 6422 3a20 2264 656d 6f5f 626f 6f6b  kId": "demo_book
-00001df0: 5f31 222c 0a20 2020 2020 2020 2020 2020  _1",.           
-00001e00: 2020 2020 2020 2020 2022 7363 6f70 6522           "scope"
-00001e10: 3a20 2274 6832 2d73 636f 7065 222c 0a20  : "th2-scope",. 
-00001e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e30: 2020 2022 6174 7461 6368 6564 4d65 7373     "attachedMess
-00001e40: 6167 6549 6473 223a 205b 5d2c 0a20 2020  ageIds": [],.   
-00001e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e60: 2022 626f 6479 223a 207b 2274 7970 6522   "body": {"type"
-00001e70: 3a20 226d 6573 7361 6765 222c 2022 6461  : "message", "da
-00001e80: 7461 223a 2022 6473 2d6c 6962 2074 6573  ta": "ds-lib tes
-00001e90: 7420 626f 6479 227d 2c0a 2020 2020 2020  t body"},.      
-00001ea0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00001eb0: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
-00001ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ed0: 2020 2022 6576 656e 7449 6422 3a20 2264     "eventId": "d
-00001ee0: 656d 6f5f 626f 6f6b 5f31 3a74 6832 2d73  emo_book_1:th2-s
-00001ef0: 636f 7065 3a32 3032 3330 3130 3531 3335  cope:20230105135
-00001f00: 3730 3535 3633 3532 3230 3030 3a39 6164  705563522000:9ad
-00001f10: 6262 3365 302d 3566 3862 2d34 6332 382d  bb3e0-5f8b-4c28-
-00001f20: 6132 6163 2d37 3336 3165 3866 6137 3034  a2ac-7361e8fa704
-00001f30: 633e 6465 6d6f 5f62 6f6f 6b5f 313a 7468  c>demo_book_1:th
-00001f40: 322d 7363 6f70 653a 3230 3233 3031 3035  2-scope:20230105
-00001f50: 3133 3537 3035 3536 3337 3537 3030 303a  135705563757000:
-00001f60: 6436 3165 3933 3061 2d38 6430 302d 3131  d61e930a-8d00-11
-00001f70: 6564 2d61 6131 612d 6433 3461 3631 3535  ed-aa1a-d34a6155
-00001f80: 3135 3264 5f33 222c 0a20 2020 2020 2020  152d_3",.       
-00001f90: 2020 2020 2020 2020 2020 2020 2022 6261               "ba
-00001fa0: 7463 6849 6422 3a20 2264 656d 6f5f 626f  tchId": "demo_bo
-00001fb0: 6f6b 5f31 3a74 6832 2d73 636f 7065 3a32  ok_1:th2-scope:2
-00001fc0: 3032 3330 3130 3531 3335 3730 3535 3633  0230105135705563
-00001fd0: 3532 3230 3030 3a39 6164 6262 3365 302d  522000:9adbb3e0-
-00001fe0: 3566 3862 2d34 6332 382d 6132 6163 2d37  5f8b-4c28-a2ac-7
-00001ff0: 3336 3165 3866 6137 3034 6322 2c0a 2020  361e8fa704c",.  
-00002000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002010: 2020 2269 7342 6174 6368 6564 223a 2054    "isBatched": T
-00002020: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-00002030: 2020 2020 2020 2020 2022 6576 656e 744e           "eventN
-00002040: 616d 6522 3a20 2250 6c61 696e 2065 7665  ame": "Plain eve
-00002050: 6e74 2032 222c 0a20 2020 2020 2020 2020  nt 2",.         
-00002060: 2020 2020 2020 2020 2020 2022 6576 656e             "even
-00002070: 7454 7970 6522 3a20 2264 732d 6c69 622d  tType": "ds-lib-
-00002080: 7465 7374 2d65 7665 6e74 222c 0a20 2020  test-event",.   
-00002090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020a0: 2022 656e 6454 696d 6573 7461 6d70 223a   "endTimestamp":
-000020b0: 207b 2265 706f 6368 5365 636f 6e64 223a   {"epochSecond":
-000020c0: 2031 3637 3239 3237 3032 352c 2022 6e61   1672927025, "na
-000020d0: 6e6f 223a 2035 3633 3739 3130 3030 7d2c  no": 563791000},
-000020e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000020f0: 2020 2020 2022 7374 6172 7454 696d 6573       "startTimes
-00002100: 7461 6d70 223a 207b 2265 706f 6368 5365  tamp": {"epochSe
-00002110: 636f 6e64 223a 2031 3637 3239 3237 3032  cond": 167292702
-00002120: 352c 2022 6e61 6e6f 223a 2035 3633 3735  5, "nano": 56375
-00002130: 3730 3030 7d2c 0a20 2020 2020 2020 2020  7000},.         
-00002140: 2020 2020 2020 2020 2020 2022 7061 7265             "pare
-00002150: 6e74 4576 656e 7449 6422 3a20 2264 656d  ntEventId": "dem
-00002160: 6f5f 626f 6f6b 5f31 3a74 6832 2d73 636f  o_book_1:th2-sco
-00002170: 7065 3a32 3032 3330 3130 3531 3335 3730  pe:2023010513570
-00002180: 3535 3630 3837 3330 3030 3a64 3631 6539  5560873000:d61e9
-00002190: 3330 612d 3864 3030 2d31 3165 642d 6161  30a-8d00-11ed-aa
-000021a0: 3161 2d64 3334 6136 3135 3531 3532 645f  1a-d34a6155152d_
-000021b0: 3122 2c0a 2020 2020 2020 2020 2020 2020  1",.            
-000021c0: 2020 2020 2020 2020 2273 7563 6365 7373          "success
-000021d0: 6675 6c22 3a20 5472 7565 2c0a 2020 2020  ful": True,.    
-000021e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021f0: 2262 6f6f 6b49 6422 3a20 2264 656d 6f5f  "bookId": "demo_
-00002200: 626f 6f6b 5f31 222c 0a20 2020 2020 2020  book_1",.       
-00002210: 2020 2020 2020 2020 2020 2020 2022 7363               "sc
-00002220: 6f70 6522 3a20 2274 6832 2d73 636f 7065  ope": "th2-scope
-00002230: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00002240: 2020 2020 2020 2022 6174 7461 6368 6564         "attached
-00002250: 4d65 7373 6167 6549 6473 223a 205b 5d2c  MessageIds": [],
-00002260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002270: 2020 2020 2022 626f 6479 223a 207b 2274       "body": {"t
-00002280: 7970 6522 3a20 226d 6573 7361 6765 222c  ype": "message",
-00002290: 2022 6461 7461 223a 2022 6473 2d6c 6962   "data": "ds-lib
-000022a0: 2074 6573 7420 626f 6479 227d 2c0a 2020   test body"},.  
-000022b0: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-000022c0: 0a20 2020 2020 2020 2020 2020 205d 0a20  .            ]. 
-000022d0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000022e0: 200a 2020 2020 2020 2020 2320 5b31 5d20   .        # [1] 
-000022f0: 576f 726b 696e 6720 7769 7468 2061 2044  Working with a D
-00002300: 6174 6120 6f62 6a65 6374 2e0a 2020 2020  ata object..    
-00002310: 2020 2020 2320 5b31 2e31 5d20 4669 6c74      # [1.1] Filt
-00002320: 6572 2e0a 2020 2020 2020 2020 6669 6c74  er..        filt
-00002330: 6572 6564 5f65 7665 6e74 733a 2044 6174  ered_events: Dat
-00002340: 6120 3d20 6576 656e 7473 2e66 696c 7465  a = events.filte
-00002350: 7228 6c61 6d62 6461 2065 3a20 655b 2262  r(lambda e: e["b
-00002360: 6f64 7922 5d20 213d 205b 5d29 2020 2320  ody"] != [])  # 
-00002370: 4669 6c74 6572 2065 7665 6e74 7320 7769  Filter events wi
-00002380: 7468 2065 6d70 7479 2062 6f64 792e 0a20  th empty body.. 
-00002390: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000023a0: 0a20 2020 2020 2020 2023 205b 312e 325d  .        # [1.2]
-000023b0: 204d 6170 2e0a 2020 2020 2020 2020 6465   Map..        de
-000023c0: 6620 7472 616e 7366 6f72 6d5f 6675 6e63  f transform_func
-000023d0: 7469 6f6e 2872 6563 6f72 6429 3a0a 2020  tion(record):.  
-000023e0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000023f0: 207b 2265 7665 6e74 4e61 6d65 223a 2072   {"eventName": r
-00002400: 6563 6f72 645b 2265 7665 6e74 4e61 6d65  ecord["eventName
-00002410: 225d 2c20 2273 7563 6365 7373 6675 6c22  "], "successful"
-00002420: 3a20 7265 636f 7264 5b22 7375 6363 6573  : record["succes
-00002430: 7366 756c 225d 7d0a 2020 2020 2020 2020  sful"]}.        
-00002440: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00002450: 2020 6669 6c74 6572 6564 5f61 6e64 5f6d    filtered_and_m
-00002460: 6170 7065 645f 6576 656e 7473 203d 2066  apped_events = f
-00002470: 696c 7465 7265 645f 6576 656e 7473 2e6d  iltered_events.m
-00002480: 6170 2874 7261 6e73 666f 726d 5f66 756e  ap(transform_fun
-00002490: 6374 696f 6e29 0a20 2020 2020 2020 200a  ction).        .
-000024a0: 2020 2020 2020 2020 2320 5b31 2e33 5d20          # [1.3] 
-000024b0: 4461 7461 2070 6970 656c 696e 652e 0a20  Data pipeline.. 
-000024c0: 2020 2020 2020 2023 2020 2020 2020 2049         #       I
-000024d0: 6e73 7465 6164 206f 6620 646f 696e 6720  nstead of doing 
-000024e0: 6461 7461 2074 7261 6e73 666f 726d 6174  data transformat
-000024f0: 696f 6e73 2073 7465 7020 6279 2073 7465  ions step by ste
-00002500: 7020 796f 7520 6361 6e20 646f 2069 7420  p you can do it 
-00002510: 696e 206f 6e65 206c 696e 652e 0a20 2020  in one line..   
-00002520: 2020 2020 2066 696c 7465 7265 645f 616e       filtered_an
-00002530: 645f 6d61 7070 6564 5f65 7665 6e74 735f  d_mapped_events_
-00002540: 6279 5f70 6970 656c 696e 6520 3d20 6576  by_pipeline = ev
-00002550: 656e 7473 2e66 696c 7465 7228 6c61 6d62  ents.filter(lamb
-00002560: 6461 2065 3a20 655b 2262 6f64 7922 5d20  da e: e["body"] 
-00002570: 213d 205b 5d29 2e6d 6170 280a 2020 2020  != []).map(.    
-00002580: 2020 2020 2020 2020 7472 616e 7366 6f72          transfor
-00002590: 6d5f 6675 6e63 7469 6f6e 0a20 2020 2020  m_function.     
-000025a0: 2020 2029 0a20 2020 2020 2020 2023 2043     ).        # C
-000025b0: 6f6e 7465 6e74 206f 6620 7468 6573 6520  ontent of these 
-000025c0: 7477 6f20 4461 7461 206f 626a 6563 7473  two Data objects
-000025d0: 2073 686f 756c 6420 6265 2065 7175 616c   should be equal
-000025e0: 2e0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
-000025f0: 206c 6973 7428 6669 6c74 6572 6564 5f61   list(filtered_a
-00002600: 6e64 5f6d 6170 7065 645f 6576 656e 7473  nd_mapped_events
-00002610: 2920 3d3d 206c 6973 7428 6669 6c74 6572  ) == list(filter
-00002620: 6564 5f61 6e64 5f6d 6170 7065 645f 6576  ed_and_mapped_ev
-00002630: 656e 7473 5f62 795f 7069 7065 6c69 6e65  ents_by_pipeline
-00002640: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-00002650: 2020 2023 205b 312e 345d 2053 6966 742e     # [1.4] Sift.
-00002660: 2053 6b69 7020 7468 6520 6669 7273 7420   Skip the first 
-00002670: 6665 7720 6974 656d 7320 6f72 206c 696d  few items or lim
-00002680: 6974 2074 6865 6d2e 0a20 2020 2020 2020  it them..       
-00002690: 2064 6174 6120 3d20 4461 7461 285b 312c   data = Data([1,
-000026a0: 2032 2c20 332c 2034 2c20 352c 2036 2c20   2, 3, 4, 5, 6, 
-000026b0: 372c 2038 2c20 392c 2031 302c 2031 312c  7, 8, 9, 10, 11,
-000026c0: 2031 322c 2031 332c 2031 342c 2031 355d   12, 13, 14, 15]
-000026d0: 290a 2020 2020 2020 2020 6974 656d 735f  ).        items_
-000026e0: 6672 6f6d 5f31 315f 746f 5f65 6e64 3a20  from_11_to_end: 
-000026f0: 4765 6e65 7261 746f 7220 3d20 6461 7461  Generator = data
-00002700: 2e73 6966 7428 736b 6970 3d31 3029 0a20  .sift(skip=10). 
-00002710: 2020 2020 2020 206f 6e6c 795f 6669 7273         only_firs
-00002720: 745f 3130 5f69 7465 6d73 3a20 4765 6e65  t_10_items: Gene
-00002730: 7261 746f 7220 3d20 6461 7461 2e73 6966  rator = data.sif
-00002740: 7428 6c69 6d69 743d 3130 290a 2020 2020  t(limit=10).    
-00002750: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-00002760: 312e 355d 2043 6861 6e67 696e 6720 6361  1.5] Changing ca
-00002770: 6368 6520 7374 6174 7573 2e0a 2020 2020  che status..    
-00002780: 2020 2020 6576 656e 7473 2e75 7365 5f63      events.use_c
-00002790: 6163 6865 2854 7275 6529 0a20 2020 2020  ache(True).     
-000027a0: 2020 2023 206f 7220 6a75 7374 0a20 2020     # or just.   
-000027b0: 2020 2020 2065 7665 6e74 732e 7573 655f       events.use_
-000027c0: 6361 6368 6528 2920 2023 2049 6620 796f  cache()  # If yo
-000027d0: 7520 7761 6e74 2074 6f20 6163 7469 7661  u want to activa
-000027e0: 7465 2063 6163 6865 2e0a 2020 2020 2020  te cache..      
-000027f0: 2020 2320 5b31 2e36 5d20 5761 6c6b 2074    # [1.6] Walk t
-00002800: 6872 6f75 6768 2064 6174 612e 0a20 2020  hrough data..   
-00002810: 2020 2020 2066 6f72 2065 7665 6e74 2069       for event i
-00002820: 6e20 6576 656e 7473 3a0a 2020 2020 2020  n events:.      
-00002830: 2020 2020 2020 2320 446f 2073 6f6d 6574        # Do somet
-00002840: 6869 6e67 2077 6974 6820 6576 656e 7420  hing with event 
-00002850: 2865 7665 6e74 2069 7320 6120 6469 6374  (event is a dict
-00002860: 292e 0a20 2020 2020 2020 2020 2020 2070  )..            p
-00002870: 7269 6e74 2865 7665 6e74 290a 2020 2020  rint(event).    
-00002880: 2020 2020 2320 4166 7465 7220 6669 7273      # After firs
-00002890: 7420 6974 6572 6174 696f 6e20 7468 6520  t iteration the 
-000028a0: 6576 656e 7473 2068 6173 2061 2063 6163  events has a cac
-000028b0: 6865 2066 696c 652e 0a20 2020 2020 2020  he file..       
-000028c0: 2023 204e 6f77 2074 6865 7920 7769 6c6c   # Now they will
-000028d0: 2062 6520 7573 6564 2069 6e20 7468 6520   be used in the 
-000028e0: 6361 6368 6520 696e 2074 6865 206e 6578  cache in the nex
-000028f0: 7420 6974 6572 6174 696f 6e2e 0a20 2020  t iteration..   
-00002900: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
-00002910: 5b31 2e37 5d20 4765 7420 6e75 6d62 6572  [1.7] Get number
-00002920: 206f 6620 7468 6520 656c 656d 656e 7473   of the elements
-00002930: 2069 6e20 7468 6520 4461 7461 206f 626a   in the Data obj
-00002940: 6563 742e 0a20 2020 2020 2020 206e 756d  ect..        num
-00002950: 6265 725f 6f66 5f65 7665 6e74 7320 3d20  ber_of_events = 
-00002960: 6576 656e 7473 2e6c 656e 0a20 2020 2020  events.len.     
-00002970: 2020 200a 2020 2020 2020 2020 2320 5b31     .        # [1
-00002980: 2e38 5d20 4368 6563 6b20 7468 6174 2044  .8] Check that D
-00002990: 6174 6120 6f62 6a65 6374 2069 736e 2774  ata object isn't
-000029a0: 2065 6d70 7479 2e0a 2020 2020 2020 2020   empty..        
-000029b0: 2320 5468 6520 6461 7461 2073 6f75 7263  # The data sourc
-000029c0: 6520 7368 6f75 6c64 2062 6520 6e6f 7420  e should be not 
-000029d0: 656d 7074 792e 0a20 2020 2020 2020 2061  empty..        a
-000029e0: 7373 6572 7420 6576 656e 7473 2e69 735f  ssert events.is_
-000029f0: 656d 7074 7920 6973 2046 616c 7365 0a20  empty is False. 
-00002a00: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00002a10: 2320 5b31 2e39 5d20 436f 6e76 6572 7420  # [1.9] Convert 
-00002a20: 4461 7461 206f 626a 6563 7420 746f 2074  Data object to t
-00002a30: 6865 206c 6973 7420 6f66 2065 6c65 6d65  he list of eleme
-00002a40: 6e74 7328 6576 656e 7473 206f 7220 6d65  nts(events or me
-00002a50: 7373 6167 6573 292e 0a20 2020 2020 2020  ssages)..       
-00002a60: 2023 2042 6520 6361 7265 6675 6c2c 2074   # Be careful, t
-00002a70: 6869 7320 6361 6e20 7461 6b65 2074 6f6f  his can take too
-00002a80: 206d 7563 6820 6d65 6d6f 7279 2e0a 2020   much memory..  
-00002a90: 2020 2020 2020 6576 656e 7473 5f6c 6973        events_lis
-00002aa0: 7420 3d20 6c69 7374 2865 7665 6e74 7329  t = list(events)
-00002ab0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00002ac0: 2020 2320 5b31 2e31 305d 2054 6865 2063    # [1.10] The c
-00002ad0: 6163 6865 2069 6e68 6572 6974 616e 6365  ache inheritance
-00002ae0: 2e0a 2020 2020 2020 2020 2320 4372 6561  ..        # Crea
-00002af0: 7465 7320 6120 6e65 7720 4461 7461 206f  tes a new Data o
-00002b00: 626a 6563 7420 7468 6174 2077 696c 6c20  bject that will 
-00002b10: 7573 6520 6361 6368 6520 6672 6f6d 2074  use cache from t
-00002b20: 6865 2065 7665 6e74 7320 4461 7461 206f  he events Data o
-00002b30: 626a 6563 742e 0a20 2020 2020 2020 2065  bject..        e
-00002b40: 7665 6e74 735f 6669 6c74 6572 6564 3a20  vents_filtered: 
-00002b50: 4461 7461 203d 2065 7665 6e74 732e 6669  Data = events.fi
-00002b60: 6c74 6572 286c 616d 6264 6120 7265 636f  lter(lambda reco
-00002b70: 7264 3a20 7265 636f 7264 2e67 6574 2822  rd: record.get("
-00002b80: 6261 7463 6849 6422 2929 0a20 2020 2020  batchId")).     
-00002b90: 2020 200a 2020 2020 2020 2020 2320 4e65     .        # Ne
-00002ba0: 7720 4461 7461 206f 626a 6563 7473 2064  w Data objects d
-00002bb0: 6f6e 2774 2075 7365 2074 6865 6972 206f  on't use their o
-00002bc0: 776e 2063 6163 6865 2062 7920 6465 6661  wn cache by defa
-00002bd0: 756c 7420 6275 7420 7573 6520 7468 6520  ult but use the 
-00002be0: 6361 6368 6520 6f66 2074 6865 2070 6172  cache of the par
-00002bf0: 656e 7420 4461 7461 206f 626a 6563 742e  ent Data object.
-00002c00: 0a20 2020 2020 2020 2023 2055 7365 2075  .        # Use u
-00002c10: 7365 5f63 6163 6865 206d 6574 686f 6420  se_cache method 
-00002c20: 746f 2061 6374 6976 6174 6520 6361 6368  to activate cach
-00002c30: 696e 672e 0a20 2020 2020 2020 2023 2041  ing..        # A
-00002c40: 6674 6572 2074 6861 742c 2074 6865 2044  fter that, the D
-00002c50: 6174 6120 6f62 6a65 6374 2077 696c 6c20  ata object will 
-00002c60: 6372 6561 7465 2069 7473 206f 776e 2063  create its own c
-00002c70: 6163 6865 2066 696c 652e 0a20 2020 2020  ache file..     
-00002c80: 2020 2065 7665 6e74 735f 6669 6c74 6572     events_filter
-00002c90: 6564 2e75 7365 5f63 6163 6865 2829 0a20  ed.use_cache(). 
-00002ca0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00002cb0: 6c69 7374 2865 7665 6e74 735f 6669 6c74  list(events_filt
-00002cc0: 6572 6564 2920 2023 204a 7573 7420 746f  ered)  # Just to
-00002cd0: 2069 7465 7261 7465 2044 6174 6120 6f62   iterate Data ob
-00002ce0: 6a65 6374 2028 6361 6368 6520 6669 6c65  ject (cache file
-00002cf0: 2077 696c 6c20 6265 2063 7265 6174 6564   will be created
-00002d00: 292e 0a20 2020 2020 2020 200a 2020 2020  )..        .    
-00002d10: 2020 2020 6669 6c74 6572 6564 5f65 7665      filtered_eve
-00002d20: 6e74 735f 7479 7065 7320 3d20 6576 656e  nts_types = even
-00002d30: 7473 5f66 696c 7465 7265 642e 6d61 7028  ts_filtered.map(
-00002d40: 6c61 6d62 6461 2072 6563 6f72 643a 207b  lambda record: {
-00002d50: 2265 7665 6e74 5479 7065 223a 2072 6563  "eventType": rec
-00002d60: 6f72 642e 6765 7428 2265 7665 6e74 5479  ord.get("eventTy
-00002d70: 7065 2229 7d29 0a20 2020 2020 2020 200a  pe")}).        .
-00002d80: 2020 2020 2020 2020 6576 656e 7473 5f77          events_w
-00002d90: 6974 686f 7574 5f74 7970 6573 5f77 6974  ithout_types_wit
-00002da0: 685f 6261 7463 6820 3d20 6669 6c74 6572  h_batch = filter
-00002db0: 6564 5f65 7665 6e74 735f 7479 7065 732e  ed_events_types.
-00002dc0: 6669 6c74 6572 280a 2020 2020 2020 2020  filter(.        
-00002dd0: 2020 2020 6c61 6d62 6461 2072 6563 6f72      lambda recor
-00002de0: 643a 206e 6f74 2072 6563 6f72 642e 6765  d: not record.ge
-00002df0: 7428 2265 7665 6e74 5479 7065 2229 0a20  t("eventType"). 
-00002e00: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00002e10: 2065 7665 6e74 735f 7769 7468 6f75 745f   events_without_
-00002e20: 7479 7065 735f 7769 7468 5f62 6174 6368  types_with_batch
-00002e30: 2e75 7365 5f63 6163 6865 2829 0a20 2020  .use_cache().   
-00002e40: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
-00002e50: 5b31 2e31 315d 2044 6174 6120 6f62 6a65  [1.11] Data obje
-00002e60: 6374 7320 6a6f 696e 696e 672e 0a20 2020  cts joining..   
-00002e70: 2020 2020 2023 2059 6f75 2068 6176 6520       # You have 
-00002e80: 7468 6520 666f 6c6c 6f77 696e 6720 3320  the following 3 
-00002e90: 4461 7461 206f 626a 6563 7473 2e0a 2020  Data objects..  
-00002ea0: 2020 2020 2020 6431 203d 2044 6174 6128        d1 = Data(
-00002eb0: 5b31 2c20 322c 2033 5d29 0a20 2020 2020  [1, 2, 3]).     
-00002ec0: 2020 2064 3220 3d20 4461 7461 285b 2261     d2 = Data(["a
-00002ed0: 222c 207b 2269 6422 3a20 3132 337d 2c20  ", {"id": 123}, 
-00002ee0: 2263 225d 290a 2020 2020 2020 2020 6433  "c"]).        d3
-00002ef0: 203d 2044 6174 6128 5b37 2c20 382c 2039   = Data([7, 8, 9
-00002f00: 5d29 0a20 2020 2020 2020 2023 2059 6f75  ]).        # You
-00002f10: 2063 616e 206a 6f69 6e20 4461 7461 206f   can join Data o
-00002f20: 626a 6563 7473 2069 6e20 666f 6c6c 6f77  bjects in follow
-00002f30: 696e 6720 7761 7973 2e0a 2020 2020 2020  ing ways..      
-00002f40: 2020 2320 506c 6561 7365 206e 6f74 652c    # Please note,
-00002f50: 206e 6577 2044 6174 6120 6f62 6a65 6374   new Data object
-00002f60: 2077 696c 6c20 6861 7665 2063 6163 6865   will have cache
-00002f70: 2073 7461 7475 7320 3d3d 2046 616c 7365   status == False
-00002f80: 2e0a 2020 2020 2020 2020 6461 7461 5f76  ..        data_v
-00002f90: 6961 5f69 6e69 7420 3d20 4461 7461 285b  ia_init = Data([
-00002fa0: 6431 2c20 6432 2c20 6433 5d29 0a20 2020  d1, d2, d3]).   
-00002fb0: 2020 2020 2064 6174 615f 7669 615f 6164       data_via_ad
-00002fc0: 6420 3d20 6431 202b 2064 3220 2b20 6433  d = d1 + d2 + d3
-00002fd0: 0a20 2020 2020 2020 2064 6174 615f 7769  .        data_wi
-00002fe0: 7468 5f6e 6f6e 5f64 6174 615f 6f62 6a5f  th_non_data_obj_
-00002ff0: 7669 615f 696e 6974 203d 2044 6174 6128  via_init = Data(
-00003000: 5b64 312c 205b 2261 222c 207b 2269 6422  [d1, ["a", {"id"
-00003010: 3a20 3132 337d 2c20 2263 225d 2c20 6433  : 123}, "c"], d3
-00003020: 5d29 0a20 2020 2020 2020 2064 6174 615f  ]).        data_
-00003030: 7769 7468 5f6e 6f6e 5f64 6174 615f 6f62  with_non_data_ob
-00003040: 6a5f 7669 615f 6164 6420 3d20 6431 202b  j_via_add = d1 +
-00003050: 205b 2261 222c 207b 2269 6422 3a20 3132   ["a", {"id": 12
-00003060: 337d 2c20 2263 225d 202b 2064 330a 2020  3}, "c"] + d3.  
-00003070: 2020 2020 2020 2320 596f 7520 6361 6e20        # You can 
-00003080: 6a6f 696e 2063 7572 7265 6e74 2044 6174  join current Dat
-00003090: 6120 6f62 6a65 6374 206f 6e20 706c 6163  a object on plac
-000030a0: 6520 7573 696e 6720 2b3d 2e0a 2020 2020  e using +=..    
-000030b0: 2020 2020 2320 4974 2077 696c 6c20 6b65      # It will ke
-000030c0: 6570 2063 6163 6865 2073 7461 7475 732e  ep cache status.
-000030d0: 0a20 2020 2020 2020 2064 3120 2b3d 2064  .        d1 += d
-000030e0: 3320 2023 2064 3120 7769 6c6c 2062 6563  3  # d1 will bec
-000030f0: 6f6d 6520 4461 7461 285b 312c 322c 332c  ome Data([1,2,3,
-00003100: 372c 382c 395d 290a 2020 2020 2020 2020  7,8,9]).        
-00003110: 0a20 2020 2020 2020 2023 205b 312e 3132  .        # [1.12
-00003120: 5d20 4275 696c 6420 616e 6420 7265 6164  ] Build and read
-00003130: 2044 6174 6120 6f62 6a65 6374 2063 6163   Data object cac
-00003140: 6865 2066 696c 6573 2e0a 2020 2020 2020  he files..      
-00003150: 2020 6576 656e 7473 2e62 7569 6c64 5f63    events.build_c
-00003160: 6163 6865 2822 6361 6368 655f 6669 6c65  ache("cache_file
-00003170: 6e61 6d65 5f6f 725f 7061 7468 2229 0a20  name_or_path"). 
-00003180: 2020 2020 2020 2064 6174 615f 6f62 6a5f         data_obj_
-00003190: 6672 6f6d 5f63 6163 6865 203d 2044 6174  from_cache = Dat
-000031a0: 612e 6672 6f6d 5f63 6163 6865 5f66 696c  a.from_cache_fil
-000031b0: 6528 2263 6163 6865 5f66 696c 656e 616d  e("cache_filenam
-000031c0: 655f 6f72 5f70 6174 6822 290a 2020 2020  e_or_path").    
-000031d0: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-000031e0: 312e 3133 5d20 4368 6563 6b20 6966 2044  1.13] Check if D
-000031f0: 6174 6120 6973 2073 6f72 7465 642e 0a20  ata is sorted.. 
-00003200: 2020 2020 2020 2069 735f 736f 7274 6564         is_sorted
-00003210: 203d 2065 7665 6e74 732e 6973 5f73 6f72   = events.is_sor
-00003220: 7465 6428 6c61 6d62 6461 2065 3a20 655b  ted(lambda e: e[
-00003230: 2273 7461 7274 5469 6d65 7374 616d 7022  "startTimestamp"
-00003240: 5d5b 2265 706f 6368 5365 636f 6e64 225d  ]["epochSecond"]
-00003250: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-00003260: 2020 2023 205b 325d 2057 6f72 6b69 6e67     # [2] Working
-00003270: 2077 6974 6820 636f 6e76 6572 7465 7273   with converters
-00003280: 2e0a 2020 2020 2020 2020 2320 5468 6572  ..        # Ther
-00003290: 6520 6172 6520 6375 7272 656e 746c 7920  e are currently 
-000032a0: 7468 7265 6520 696d 706c 656d 656e 7461  three implementa
-000032b0: 7469 6f6e 7320 6f66 2049 5469 6d65 7374  tions of ITimest
-000032c0: 616d 7043 6f6e 7665 7274 6572 2063 6c61  ampConverter cla
-000032d0: 7373 3a20 4461 7465 7469 6d65 436f 6e76  ss: DatetimeConv
-000032e0: 6572 7465 2c20 4461 7465 7469 6d65 5374  erte, DatetimeSt
-000032f0: 7269 6e67 436f 6e76 6572 7465 7220 616e  ringConverter an
-00003300: 6420 5072 6f74 6f62 7566 5469 6d65 7374  d ProtobufTimest
-00003310: 616d 7043 6f6e 7665 7274 6572 2e0a 2020  ampConverter..  
-00003320: 2020 2020 2020 2320 5468 6579 2061 6c6c        # They all
-00003330: 2069 6d70 6c65 6d65 6e74 2073 616d 6520   implement same 
-00003340: 6d65 7468 6f64 7320 6672 6f6d 2062 6173  methods from bas
-00003350: 6520 636c 6173 732e 0a20 2020 2020 2020  e class..       
-00003360: 2023 204e 6f74 6520 7468 6174 2073 6f6d   # Note that som
-00003370: 6520 6163 6375 7261 6379 206d 6179 2062  e accuracy may b
-00003380: 6520 6c6f 7374 2064 7572 696e 6720 636f  e lost during co
-00003390: 6e76 6572 7369 6f6e 2e0a 2020 2020 2020  nversion..      
-000033a0: 2020 2320 4966 2066 6f72 2065 7861 6d70    # If for examp
-000033b0: 6c65 2079 6f75 2075 7365 2074 6f5f 6d69  le you use to_mi
-000033c0: 6372 6f73 6563 6f6e 6473 206e 616e 6f73  croseconds nanos
-000033d0: 6563 6f6e 6473 2077 696c 6c20 6265 2063  econds will be c
-000033e0: 7574 206f 6666 2069 6e73 7465 6164 206f  ut off instead o
-000033f0: 6620 726f 756e 6469 6e67 2e0a 2020 2020  f rounding..    
-00003400: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-00003410: 322e 315d 2044 6174 6574 696d 6543 6f6e  2.1] DatetimeCon
-00003420: 7665 7274 6572 2e0a 2020 2020 2020 2020  verter..        
-00003430: 2320 4461 7465 7469 6d65 436f 6e76 6572  # DatetimeConver
-00003440: 7465 7220 7461 6b65 7320 6461 7465 7469  ter takes dateti
-00003450: 6d65 2e64 6174 6574 696d 6520 6f62 6a65  me.datetime obje
-00003460: 6374 2061 7320 696e 7075 742e 0a20 2020  ct as input..   
-00003470: 2020 2020 200a 2020 2020 2020 2020 6461       .        da
-00003480: 7465 7469 6d65 5f6f 626a 203d 2064 6174  tetime_obj = dat
-00003490: 6574 696d 6528 7965 6172 3d32 3032 332c  etime(year=2023,
-000034a0: 206d 6f6e 7468 3d31 2c20 6461 793d 352c   month=1, day=5,
-000034b0: 2068 6f75 723d 3134 2c20 6d69 6e75 7465   hour=14, minute
-000034c0: 3d33 382c 2073 6563 6f6e 643d 3235 2c20  =38, second=25, 
-000034d0: 6d69 6372 6f73 6563 6f6e 643d 3134 3630  microsecond=1460
-000034e0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-000034f0: 2020 2023 2049 7420 6861 7320 6d65 7468     # It has meth
-00003500: 6f64 7320 7468 6174 2072 6574 7572 6e20  ods that return 
-00003510: 7468 6520 6461 7465 7469 6d65 2069 6e20  the datetime in 
-00003520: 6469 6666 6572 656e 7420 666f 726d 6173  different formas
-00003530: 3a0a 2020 2020 2020 2020 0a20 2020 2020  :.        .     
-00003540: 2020 2064 6174 655f 6d73 203d 2044 6174     date_ms = Dat
-00003550: 6574 696d 6543 6f6e 7665 7274 6572 2e74  etimeConverter.t
-00003560: 6f5f 6d69 6c6c 6973 6563 6f6e 6473 2864  o_milliseconds(d
-00003570: 6174 6574 696d 655f 6f62 6a29 0a20 2020  atetime_obj).   
-00003580: 2020 2020 2064 6174 655f 7573 203d 2044       date_us = D
-00003590: 6174 6574 696d 6543 6f6e 7665 7274 6572  atetimeConverter
-000035a0: 2e74 6f5f 6d69 6372 6f73 6563 6f6e 6473  .to_microseconds
-000035b0: 2864 6174 6574 696d 655f 6f62 6a29 0a20  (datetime_obj). 
-000035c0: 2020 2020 2020 2023 2043 6f6e 7665 7274         # Convert
-000035d0: 696e 6720 746f 206e 616e 6f73 6563 6f6e  ing to nanosecon
-000035e0: 6473 206a 7573 7473 2061 6464 7320 7468  ds justs adds th
-000035f0: 7265 6520 7472 6169 6c69 6e67 207a 6572  ree trailing zer
-00003600: 6f73 2061 7320 6461 7465 7469 6d65 206f  os as datetime o
-00003610: 626a 6563 7420 646f 6573 6e27 7420 6861  bject doesn't ha
-00003620: 7665 206e 616e 6f73 6563 6f6e 6473 2e0a  ve nanoseconds..
-00003630: 2020 2020 2020 2020 6461 7465 5f6e 7320          date_ns 
-00003640: 3d20 4461 7465 7469 6d65 436f 6e76 6572  = DatetimeConver
-00003650: 7465 722e 746f 5f6e 616e 6f73 6563 6f6e  ter.to_nanosecon
-00003660: 6473 2864 6174 6574 696d 655f 6f62 6a29  ds(datetime_obj)
-00003670: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00003680: 2020 2320 5b32 2e32 5d20 4461 7465 7469    # [2.2] Dateti
-00003690: 6d65 5374 7269 6e67 436f 6e76 6572 7465  meStringConverte
-000036a0: 720a 2020 2020 2020 2020 2320 4461 7465  r.        # Date
-000036b0: 7469 6d65 5374 7269 6e67 436f 6e76 6572  timeStringConver
-000036c0: 7465 7220 7461 6b65 7320 7374 7269 6e67  ter takes string
-000036d0: 2069 6e20 2279 7979 792d 4d4d 2d64 6454   in "yyyy-MM-ddT
-000036e0: 4848 3a6d 6d3a 7373 5b2e 5353 5353 5353  HH:mm:ss[.SSSSSS
-000036f0: 5353 535d 5a22 2066 6f72 6d61 742e 0a20  SSS]Z" format.. 
-00003700: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00003710: 6461 7465 5f73 7472 696e 6720 3d20 2232  date_string = "2
-00003720: 3032 332d 3031 2d30 3554 3134 3a33 383a  023-01-05T14:38:
-00003730: 3235 2e30 3031 3436 5a22 0a20 2020 2020  25.00146Z".     
-00003740: 2020 200a 2020 2020 2020 2020 2320 5765     .        # We
-00003750: 2068 6176 6520 7361 6d65 206d 6574 686f   have same metho
-00003760: 6473 2061 7320 696e 2044 6174 6574 696d  ds as in Datetim
-00003770: 6543 6f6e 7665 7274 6572 0a20 2020 2020  eConverter.     
-00003780: 2020 2064 6174 655f 6d73 5f66 726f 6d5f     date_ms_from_
-00003790: 7374 7269 6e67 203d 2044 6174 6574 696d  string = Datetim
-000037a0: 6553 7472 696e 6743 6f6e 7665 7274 6572  eStringConverter
-000037b0: 2e74 6f5f 6d69 6c6c 6973 6563 6f6e 6473  .to_milliseconds
-000037c0: 2864 6174 655f 7374 7269 6e67 290a 2020  (date_string).  
-000037d0: 2020 2020 2020 6461 7465 5f75 735f 6672        date_us_fr
-000037e0: 6f6d 5f73 7472 696e 6720 3d20 4461 7465  om_string = Date
-000037f0: 7469 6d65 5374 7269 6e67 436f 6e76 6572  timeStringConver
-00003800: 7465 722e 746f 5f6d 6963 726f 7365 636f  ter.to_microseco
-00003810: 6e64 7328 6461 7465 5f73 7472 696e 6729  nds(date_string)
-00003820: 0a20 2020 2020 2020 2064 6174 655f 6e73  .        date_ns
-00003830: 5f66 726f 6d5f 7374 7269 6e67 203d 2044  _from_string = D
-00003840: 6174 6574 696d 6553 7472 696e 6743 6f6e  atetimeStringCon
-00003850: 7665 7274 6572 2e74 6f5f 6e61 6e6f 7365  verter.to_nanose
-00003860: 636f 6e64 7328 6461 7465 5f73 7472 696e  conds(date_strin
-00003870: 6729 0a20 2020 2020 2020 200a 2020 2020  g).        .    
-00003880: 2020 2020 2320 5765 2063 616e 2061 6c73      # We can als
-00003890: 6f20 6765 7420 6461 7465 7469 6d65 206f  o get datetime o
-000038a0: 626a 6563 7420 6672 6f6d 2073 7472 696e  bject from strin
-000038b0: 670a 2020 2020 2020 2020 6461 7465 7469  g.        dateti
-000038c0: 6d65 5f66 726f 6d5f 7374 7269 6e67 203d  me_from_string =
-000038d0: 2044 6174 6574 696d 6553 7472 696e 6743   DatetimeStringC
-000038e0: 6f6e 7665 7274 6572 2e74 6f5f 6461 7465  onverter.to_date
-000038f0: 7469 6d65 2864 6174 655f 7374 7269 6e67  time(date_string
-00003900: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-00003910: 2020 2023 205b 322e 335d 2050 726f 746f     # [2.3] Proto
-00003920: 6275 6654 696d 6573 7461 6d70 436f 6e76  bufTimestampConv
-00003930: 6572 7465 720a 2020 2020 2020 2020 2320  erter.        # 
-00003940: 5072 6f74 6f62 7566 2074 696d 6573 7461  Protobuf timesta
-00003950: 6d70 7320 6d75 7374 2062 6520 696e 2066  mps must be in f
-00003960: 6f72 6d20 7b22 6570 6f63 6853 6563 6f6e  orm {"epochSecon
-00003970: 6422 3a20 7365 636f 6e64 732c 2022 6e61  d": seconds, "na
-00003980: 6e6f 223a 206e 616e 6f73 6563 6f6e 6473  no": nanoseconds
-00003990: 7d0a 2020 2020 2020 2020 0a20 2020 2020  }.        .     
-000039a0: 2020 2070 726f 746f 6275 665f 7469 6d65     protobuf_time
-000039b0: 7374 616d 7020 3d20 7b22 6570 6f63 6853  stamp = {"epochS
-000039c0: 6563 6f6e 6422 3a20 3136 3732 3932 3935  econd": 16729295
-000039d0: 3035 2c20 226e 616e 6f22 3a20 315f 3436  05, "nano": 1_46
-000039e0: 305f 3030 307d 0a20 2020 2020 2020 200a  0_000}.        .
-000039f0: 2020 2020 2020 2020 6461 7465 5f6d 735f          date_ms_
-00003a00: 6672 6f6d 5f74 696d 6573 7461 6d70 203d  from_timestamp =
-00003a10: 2050 726f 746f 6275 6654 696d 6573 7461   ProtobufTimesta
-00003a20: 6d70 436f 6e76 6572 7465 722e 746f 5f6d  mpConverter.to_m
-00003a30: 696c 6c69 7365 636f 6e64 7328 7072 6f74  illiseconds(prot
-00003a40: 6f62 7566 5f74 696d 6573 7461 6d70 290a  obuf_timestamp).
-00003a50: 2020 2020 2020 2020 6461 7465 5f75 735f          date_us_
-00003a60: 6672 6f6d 5f74 696d 6573 7461 6d70 203d  from_timestamp =
-00003a70: 2050 726f 746f 6275 6654 696d 6573 7461   ProtobufTimesta
-00003a80: 6d70 436f 6e76 6572 7465 722e 746f 5f6d  mpConverter.to_m
-00003a90: 6963 726f 7365 636f 6e64 7328 7072 6f74  icroseconds(prot
-00003aa0: 6f62 7566 5f74 696d 6573 7461 6d70 290a  obuf_timestamp).
-00003ab0: 2020 2020 2020 2020 6461 7465 5f6e 735f          date_ns_
-00003ac0: 6672 6f6d 5f74 696d 6573 7461 6d70 203d  from_timestamp =
-00003ad0: 2050 726f 746f 6275 6654 696d 6573 7461   ProtobufTimesta
-00003ae0: 6d70 436f 6e76 6572 7465 722e 746f 5f6e  mpConverter.to_n
-00003af0: 616e 6f73 6563 6f6e 6473 2870 726f 746f  anoseconds(proto
-00003b00: 6275 665f 7469 6d65 7374 616d 7029 0a20  buf_timestamp). 
-00003b10: 2020 2020 2020 2064 6174 6574 696d 655f         datetime_
-00003b20: 6672 6f6d 5f74 696d 6573 7461 6d70 203d  from_timestamp =
-00003b30: 2050 726f 746f 6275 6654 696d 6573 7461   ProtobufTimesta
-00003b40: 6d70 436f 6e76 6572 7465 722e 746f 5f64  mpConverter.to_d
-00003b50: 6174 6574 696d 6528 7072 6f74 6f62 7566  atetime(protobuf
-00003b60: 5f74 696d 6573 7461 6d70 290a 2020 2020  _timestamp).    
-00003b70: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-00003b80: 335d 2057 6f72 6b69 6e67 2077 6974 6820  3] Working with 
-00003b90: 4576 656e 7454 7265 6520 616e 6420 4576  EventTree and Ev
-00003ba0: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
-00003bb0: 6e2e 0a20 2020 2020 2020 200a 2020 2020  n..        .    
-00003bc0: 2020 2020 2320 5b33 2e31 5d20 4275 696c      # [3.1] Buil
-00003bd0: 6420 6120 6375 7374 6f6d 2045 7665 6e74  d a custom Event
-00003be0: 5472 6565 0a20 2020 2020 2020 2023 2054  Tree.        # T
-00003bf0: 6f20 6372 6561 7465 2061 6e20 4576 656e  o create an Even
-00003c00: 7454 7265 6520 6f62 6a65 6374 2079 6f75  tTree object you
-00003c10: 206e 6565 6420 746f 2070 726f 7669 6465   need to provide
-00003c20: 206e 616d 652c 2069 6420 616e 6420 6461   name, id and da
-00003c30: 7461 206f 6620 7468 6520 726f 6f74 2065  ta of the root e
-00003c40: 7665 6e74 2e0a 2020 2020 2020 2020 7472  vent..        tr
-00003c50: 6565 203d 2045 7665 6e74 5472 6565 2865  ee = EventTree(e
-00003c60: 7665 6e74 5f6e 616d 653d 2272 6f6f 7420  vent_name="root 
-00003c70: 6576 656e 7422 2c20 6576 656e 745f 6964  event", event_id
-00003c80: 3d22 726f 6f74 5f69 6422 2c20 6461 7461  ="root_id", data
-00003c90: 3d7b 2264 6174 6122 3a20 5b31 2c20 322c  ={"data": [1, 2,
-00003ca0: 2033 2c20 342c 2035 5d7d 290a 2020 2020   3, 4, 5]}).    
-00003cb0: 2020 2020 0a20 2020 2020 2020 2023 2054      .        # T
-00003cc0: 6f20 6164 6420 6e65 7720 6e6f 6465 2075  o add new node u
-00003cd0: 7365 2061 7070 656e 645f 6576 656e 742e  se append_event.
-00003ce0: 2070 6172 656e 745f 6964 2069 7320 6e65   parent_id is ne
-00003cf0: 6365 7373 6172 792c 2064 6174 6120 6973  cessary, data is
-00003d00: 206f 7074 696f 6e61 6c2e 0a20 2020 2020   optional..     
-00003d10: 2020 2074 7265 652e 6170 7065 6e64 5f65     tree.append_e
-00003d20: 7665 6e74 2865 7665 6e74 5f6e 616d 653d  vent(event_name=
-00003d30: 2241 222c 2065 7665 6e74 5f69 643d 2241  "A", event_id="A
-00003d40: 5f69 6422 2c20 6461 7461 3d4e 6f6e 652c  _id", data=None,
-00003d50: 2070 6172 656e 745f 6964 3d22 726f 6f74   parent_id="root
-00003d60: 5f69 6422 290a 2020 2020 2020 2020 0a20  _id").        . 
-00003d70: 2020 2020 2020 2023 205b 332e 335d 2042         # [3.3] B
-00003d80: 7569 6c64 696e 6720 7468 6520 4576 656e  uilding the Even
-00003d90: 7454 7265 6543 6f6c 6c65 6374 696f 6e2e  tTreeCollection.
-00003da0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00003db0: 2020 2320 4966 2079 6f75 2064 6f6e 2774    # If you don't
-00003dc0: 2073 7065 6369 6679 2064 6174 615f 736f   specify data_so
-00003dd0: 7572 6365 2066 6f72 2074 6865 2064 7269  urce for the dri
-00003de0: 7665 7220 7468 656e 2069 7420 776f 6e27  ver then it won'
-00003df0: 7420 7265 636f 7665 7220 6465 7461 6368  t recover detach
-00003e00: 6564 2065 7665 6e74 732e 0a20 2020 2020  ed events..     
-00003e10: 2020 2064 7269 7665 723a 2049 4554 4344     driver: IETCD
-00003e20: 7269 7665 7220 2023 2059 6f75 2073 686f  river  # You sho
-00003e30: 756c 6420 696e 6974 2045 5443 4472 6976  uld init ETCDriv
-00003e40: 6572 206f 626a 6563 742e 2045 2e67 2e20  er object. E.g. 
-00003e50: 6672 6f6d 204c 7744 5020 6d6f 6475 6c65  from LwDP module
-00003e60: 206f 7220 796f 7572 2063 7573 746f 6d20   or your custom 
-00003e70: 636c 6173 732e 0a20 2020 2020 2020 2065  class..        e
-00003e80: 7463 203d 2045 7665 6e74 5472 6565 436f  tc = EventTreeCo
-00003e90: 6c6c 6563 7469 6f6e 2864 7269 7665 7229  llection(driver)
-00003ea0: 0a20 2020 2020 2020 2065 7463 2e62 7569  .        etc.bui
-00003eb0: 6c64 2865 7665 6e74 7329 0a20 2020 2020  ld(events).     
-00003ec0: 2020 200a 2020 2020 2020 2020 2320 4465     .        # De
-00003ed0: 7461 6368 6564 2065 7665 6e74 7320 6973  tached events is
-00003ee0: 6e27 7420 656d 7074 792e 0a20 2020 2020  n't empty..     
-00003ef0: 2020 2061 7373 6572 7420 6574 632e 6765     assert etc.ge
-00003f00: 745f 6465 7461 6368 6564 5f65 7665 6e74  t_detached_event
-00003f10: 7328 290a 2020 2020 2020 2020 0a20 2020  s().        .   
-00003f20: 2020 2020 2065 7463 203d 2045 7665 6e74       etc = Event
-00003f30: 5472 6565 436f 6c6c 6563 7469 6f6e 2864  TreeCollection(d
-00003f40: 7269 7665 7229 0a20 2020 2020 2020 2023  river).        #
-00003f50: 2044 6574 6163 6865 6420 6576 656e 7473   Detached events
-00003f60: 2061 7265 2065 6d70 7479 2062 6563 6175   are empty becau
-00003f70: 7365 2074 6865 7920 7765 7265 2072 6563  se they were rec
-00003f80: 6f76 6572 6564 2e0a 2020 2020 2020 2020  overed..        
-00003f90: 6173 7365 7274 206e 6f74 2065 7463 2e67  assert not etc.g
-00003fa0: 6574 5f64 6574 6163 6865 645f 6576 656e  et_detached_even
-00003fb0: 7473 2829 0a20 2020 2020 2020 200a 2020  ts().        .  
-00003fc0: 2020 2020 2020 2320 5468 6520 636f 6c6c        # The coll
-00003fd0: 6563 7469 6f6e 2068 6173 2045 7665 6e74  ection has Event
-00003fe0: 5472 6565 7320 6561 6368 2077 6974 6820  Trees each with 
-00003ff0: 6120 7472 6565 206f 6620 6576 656e 7473  a tree of events
-00004000: 2e0a 2020 2020 2020 2020 2320 5573 696e  ..        # Usin
-00004010: 6720 436f 6c6c 6563 7469 6f6e 2061 6e64  g Collection and
-00004020: 2045 7665 6e74 5472 6565 732c 2079 6f75   EventTrees, you
-00004030: 2063 616e 2077 6f72 6b20 666c 6578 6962   can work flexib
-00004040: 6c79 2077 6974 6820 6576 656e 7473 2e0a  ly with events..
-00004050: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00004060: 2023 205b 332e 332e 315d 2047 6574 206c   # [3.3.1] Get l
-00004070: 6561 7665 7320 6f66 2061 6c6c 2074 7265  eaves of all tre
-00004080: 6573 2e0a 2020 2020 2020 2020 6c65 6176  es..        leav
-00004090: 6573 3a20 5475 706c 655b 6469 6374 5d20  es: Tuple[dict] 
-000040a0: 3d20 6574 632e 6765 745f 6c65 6176 6573  = etc.get_leaves
-000040b0: 2829 0a20 2020 2020 2020 200a 2020 2020  ().        .    
-000040c0: 2020 2020 2320 5b33 2e33 2e32 5d20 4765      # [3.3.2] Ge
-000040d0: 7420 726f 6f74 7320 6964 7320 6f66 2061  t roots ids of a
-000040e0: 6c6c 2074 7265 6573 2e0a 2020 2020 2020  ll trees..      
-000040f0: 2020 726f 6f74 733a 204c 6973 745b 7374    roots: List[st
-00004100: 725d 203d 2065 7463 2e67 6574 5f72 6f6f  r] = etc.get_roo
-00004110: 7473 5f69 6473 2829 0a20 2020 2020 2020  ts_ids().       
-00004120: 200a 2020 2020 2020 2020 2320 5b33 2e33   .        # [3.3
-00004130: 2e33 5d20 4669 6e64 2061 6e20 6576 656e  .3] Find an even
-00004140: 7420 696e 2061 6c6c 2074 7265 6573 2e0a  t in all trees..
-00004150: 2020 2020 2020 2020 6669 6e64 5f65 7665          find_eve
-00004160: 6e74 3a20 4f70 7469 6f6e 616c 5b64 6963  nt: Optional[dic
-00004170: 745d 203d 2065 7463 2e66 696e 6428 6c61  t] = etc.find(la
-00004180: 6d62 6461 2065 7665 6e74 3a20 2253 656e  mbda event: "Sen
-00004190: 6420 6d65 7373 6167 6522 2069 6e20 6576  d message" in ev
-000041a0: 656e 745b 2265 7665 6e74 5479 7065 225d  ent["eventType"]
-000041b0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-000041c0: 2020 2023 205b 332e 332e 345d 2046 696e     # [3.3.4] Fin
-000041d0: 6420 616c 6c20 6576 656e 7473 2069 6e20  d all events in 
-000041e0: 616c 6c20 7472 6565 732e 2054 6865 7265  all trees. There
-000041f0: 2069 7320 616c 736f 2069 7465 7261 626c   is also iterabl
-00004200: 6520 7665 7273 696f 6e20 2766 696e 6461  e version 'finda
-00004210: 6c6c 5f69 7465 7227 2e0a 2020 2020 2020  ll_iter'..      
-00004220: 2020 6669 6e64 5f65 7665 6e74 733a 204c    find_events: L
-00004230: 6973 745b 6469 6374 5d20 3d20 6574 632e  ist[dict] = etc.
-00004240: 6669 6e64 616c 6c28 6c61 6d62 6461 2065  findall(lambda e
-00004250: 7665 6e74 3a20 6576 656e 745b 2273 7563  vent: event["suc
-00004260: 6365 7373 6675 6c22 5d20 6973 2054 7275  cessful"] is Tru
-00004270: 6529 0a20 2020 2020 2020 200a 2020 2020  e).        .    
-00004280: 2020 2020 2320 5b33 2e33 2e35 5d20 4669      # [3.3.5] Fi
-00004290: 6e64 2061 6e20 616e 6365 7374 6f72 206f  nd an ancestor o
-000042a0: 6620 7468 6520 6576 656e 742e 0a20 2020  f the event..   
-000042b0: 2020 2020 2061 6e63 6573 746f 723a 204f       ancestor: O
-000042c0: 7074 696f 6e61 6c5b 6469 6374 5d20 3d20  ptional[dict] = 
-000042d0: 6574 632e 6669 6e64 5f61 6e63 6573 746f  etc.find_ancesto
-000042e0: 7228 0a20 2020 2020 2020 2020 2020 2022  r(.            "
-000042f0: 3862 6265 3337 3137 2d63 6635 392d 3131  8bbe3717-cf59-11
-00004300: 6562 2d61 3366 372d 3039 3466 3930 3463  eb-a3f7-094f904c
-00004310: 3361 3632 222c 2066 696c 7465 723d 6c61  3a62", filter=la
-00004320: 6d62 6461 2065 7665 6e74 3a20 2252 6f6f  mbda event: "Roo
-00004330: 7445 7665 6e74 2220 696e 2065 7665 6e74  tEvent" in event
-00004340: 5b22 6576 656e 744e 616d 6522 5d0a 2020  ["eventName"].  
-00004350: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00004360: 0a20 2020 2020 2020 2023 205b 332e 332e  .        # [3.3.
-00004370: 365d 2047 6574 2063 6869 6c64 7265 6e20  6] Get children 
-00004380: 6f66 2074 6865 2065 7665 6e74 2e20 5468  of the event. Th
-00004390: 6572 6520 6973 2061 6c73 6f20 6974 6572  ere is also iter
-000043a0: 6162 6c65 2076 6572 7369 6f6e 2027 6765  able version 'ge
-000043b0: 745f 6368 696c 6472 656e 5f69 7465 7227  t_children_iter'
-000043c0: 2e0a 2020 2020 2020 2020 6368 696c 6472  ..        childr
-000043d0: 656e 3a20 5475 706c 655b 6469 6374 5d20  en: Tuple[dict] 
-000043e0: 3d20 6574 632e 6765 745f 6368 696c 6472  = etc.get_childr
-000043f0: 656e 2822 3831 3434 3232 6531 2d39 6336  en("814422e1-9c6
-00004400: 382d 3131 6562 2d38 3539 382d 3639 3165  8-11eb-8598-691e
-00004410: 6264 3766 3431 3364 2229 0a20 2020 2020  bd7f413d").     
-00004420: 2020 200a 2020 2020 2020 2020 2320 5b33     .        # [3
-00004430: 2e33 2e37 5d20 4765 7420 7375 6274 7265  .3.7] Get subtre
-00004440: 6520 666f 7220 7370 6563 6966 6965 6420  e for specified 
-00004450: 6576 656e 742e 0a20 2020 2020 2020 2073  event..        s
-00004460: 7562 7472 6565 3a20 4576 656e 7454 7265  ubtree: EventTre
-00004470: 6520 3d20 6574 632e 6765 745f 7375 6274  e = etc.get_subt
-00004480: 7265 6528 2238 6532 3337 3734 642d 6366  ree("8e23774d-cf
-00004490: 3539 2d31 3165 622d 6136 6533 2d35 3562  59-11eb-a6e3-55b
-000044a0: 6664 6232 6233 6632 3122 290a 2020 2020  fdb2b3f21").    
-000044b0: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-000044c0: 332e 332e 385d 2047 6574 2066 756c 6c20  3.3.8] Get full 
-000044d0: 7061 7468 2074 6f20 7468 6520 6576 656e  path to the even
-000044e0: 742e 0a20 2020 2020 2020 2023 204c 6f6f  t..        # Loo
-000044f0: 6b73 206c 696b 6520 5b61 6e63 6573 746f  ks like [ancesto
-00004500: 725f 726f 6f74 2c20 616e 6365 7374 6f72  r_root, ancestor
-00004510: 5f6c 6576 656c 312c 2061 6e63 6573 746f  _level1, ancesto
-00004520: 725f 6c65 7665 6c32 2c20 6576 656e 745d  r_level2, event]
-00004530: 0a20 2020 2020 2020 2065 7665 6e74 5f70  .        event_p
-00004540: 6174 683a 204c 6973 745b 6469 6374 5d20  ath: List[dict] 
-00004550: 3d20 6574 632e 6765 745f 6675 6c6c 5f70  = etc.get_full_p
-00004560: 6174 6828 2238 6532 3532 3466 612d 6366  ath("8e2524fa-cf
-00004570: 3539 2d31 3165 622d 6133 6637 2d30 3934  59-11eb-a3f7-094
-00004580: 6639 3034 6333 6136 3222 290a 2020 2020  f904c3a62").    
-00004590: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-000045a0: 332e 332e 395d 2047 6574 2070 6172 656e  3.3.9] Get paren
-000045b0: 7420 6f66 2074 6865 2065 7665 6e74 2e0a  t of the event..
-000045c0: 2020 2020 2020 2020 7061 7265 6e74 203d          parent =
-000045d0: 2065 7463 2e67 6574 5f70 6172 656e 7428   etc.get_parent(
-000045e0: 2238 6532 3532 3466 612d 6366 3539 2d31  "8e2524fa-cf59-1
-000045f0: 3165 622d 6133 6637 2d30 3934 6639 3034  1eb-a3f7-094f904
-00004600: 6333 6136 3222 290a 2020 2020 2020 2020  c3a62").        
-00004610: 0a20 2020 2020 2020 2023 205b 332e 332e  .        # [3.3.
-00004620: 3130 5d20 4170 7065 6e64 206e 6577 2065  10] Append new e
-00004630: 7665 6e74 2074 6f20 7468 6520 636f 6c6c  vent to the coll
-00004640: 6563 7469 6f6e 2e0a 2020 2020 2020 2020  ection..        
-00004650: 6574 632e 6170 7065 6e64 5f65 7665 6e74  etc.append_event
-00004660: 280a 2020 2020 2020 2020 2020 2020 6576  (.            ev
-00004670: 656e 743d 7b0a 2020 2020 2020 2020 2020  ent={.          
-00004680: 2020 2020 2020 2265 7665 6e74 4964 223a        "eventId":
-00004690: 2022 6132 3066 3565 6634 2d63 3366 652d   "a20f5ef4-c3fe-
-000046a0: 6262 3130 2d61 3239 632d 6464 3364 3738  bb10-a29c-dd3d78
-000046b0: 3439 3039 6562 222c 0a20 2020 2020 2020  4909eb",.       
-000046c0: 2020 2020 2020 2020 2022 7061 7265 6e74           "parent
-000046d0: 4576 656e 7449 6422 3a20 2238 6532 3532  EventId": "8e252
-000046e0: 3466 612d 6366 3539 2d31 3165 622d 6133  4fa-cf59-11eb-a3
-000046f0: 6637 2d30 3934 6639 3034 6333 6136 3222  f7-094f904c3a62"
-00004700: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00004710: 2020 2265 7665 6e74 4e61 6d65 223a 2022    "eventName": "
-00004720: 5374 7562 4576 656e 7422 2c0a 2020 2020  StubEvent",.    
-00004730: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00004740: 2020 290a 2020 2020 2020 2020 0a20 2020    ).        .   
-00004750: 2020 2020 2023 205b 332e 332e 3131 5d20       # [3.3.11] 
-00004760: 5368 6f77 2074 6865 2065 6e74 6972 6520  Show the entire 
-00004770: 636f 6c6c 6563 7469 6f6e 2e0a 2020 2020  collection..    
-00004780: 2020 2020 6574 632e 7368 6f77 2829 0a20      etc.show(). 
-00004790: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000047a0: 2320 5b33 2e34 5d20 576f 726b 696e 6720  # [3.4] Working 
-000047b0: 7769 7468 2074 6865 2045 7665 6e74 5472  with the EventTr
-000047c0: 6565 2e0a 2020 2020 2020 2020 2320 4576  ee..        # Ev
-000047d0: 656e 7454 7265 6520 6861 7320 7468 6520  entTree has the 
-000047e0: 7361 6d65 206d 6574 686f 6473 2061 7320  same methods as 
-000047f0: 4576 656e 7454 7265 6543 6f6c 6c65 6374  EventTreeCollect
-00004800: 696f 6e2c 2062 7574 206f 6e6c 7920 666f  ion, but only fo
-00004810: 7220 6974 7320 6f77 6e20 7472 6565 2e0a  r its own tree..
-00004820: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00004830: 2023 205b 332e 342e 315d 2047 6574 2063   # [3.4.1] Get c
-00004840: 6f6c 6c65 6374 696f 6e20 7472 6565 732e  ollection trees.
-00004850: 0a20 2020 2020 2020 2074 7265 6573 3a20  .        trees: 
-00004860: 4c69 7374 5b45 7665 6e74 5472 6565 5d20  List[EventTree] 
-00004870: 3d20 6574 632e 6765 745f 7472 6565 7328  = etc.get_trees(
-00004880: 290a 2020 2020 2020 2020 7472 6565 3a20  ).        tree: 
-00004890: 4576 656e 7454 7265 6520 3d20 7472 6565  EventTree = tree
-000048a0: 735b 305d 0a20 2020 2020 2020 200a 2020  s[0].        .  
-000048b0: 2020 2020 2020 2320 4275 7420 4576 656e        # But Even
-000048c0: 7454 7265 6520 7072 6f76 6964 6573 2061  tTree provides a
-000048d0: 2077 6f72 6b20 7769 7468 2074 6865 2074   work with the t
-000048e0: 7265 652c 2062 7574 2064 6f65 7320 6e6f  ree, but does no
-000048f0: 7420 6d6f 6469 6679 2069 742e 0a20 2020  t modify it..   
-00004900: 2020 2020 2023 2049 6620 796f 7520 7761       # If you wa
-00004910: 6e74 2074 6f20 6d6f 6469 6679 2074 6865  nt to modify the
-00004920: 2074 7265 652c 2075 7365 2045 7665 6e74   tree, use Event
-00004930: 5472 6565 436f 6c6c 6563 7469 6f6e 732e  TreeCollections.
-00004940: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00004950: 2020 2320 5b33 2e35 5d20 576f 726b 696e    # [3.5] Workin
-00004960: 6720 7769 7468 2050 6172 656e 746c 6573  g with Parentles
-00004970: 7354 7265 652e 0a20 2020 2020 2020 2023  sTree..        #
-00004980: 2050 6172 656e 746c 6573 7354 7265 6520   ParentlessTree 
-00004990: 6973 2045 7665 6e74 5472 6565 2077 6869  is EventTree whi
-000049a0: 6368 2068 6173 2064 6574 6163 6865 6420  ch has detached 
-000049b0: 6576 656e 7473 2077 6974 6820 7374 7562  events with stub
-000049c0: 732e 0a20 2020 2020 2020 2070 6172 656e  s..        paren
-000049d0: 746c 6573 735f 7472 6565 733a 204c 6973  tless_trees: Lis
-000049e0: 745b 4576 656e 7454 7265 655d 203d 2065  t[EventTree] = e
-000049f0: 7463 2e67 6574 5f70 6172 656e 746c 6573  tc.get_parentles
-00004a00: 735f 7472 6565 7328 290a 2020 2020 2020  s_trees().      
-00004a10: 2020 0a20 2020 2020 2020 2023 205b 332e    .        # [3.
-00004a20: 365d 2057 6f72 6b69 6e67 2077 6974 6820  6] Working with 
-00004a30: 5061 7265 6e74 4576 656e 7454 7265 6543  ParentEventTreeC
-00004a40: 6f6c 6c65 6374 696f 6e2e 0a20 2020 2020  ollection..     
-00004a50: 2020 2023 2050 6172 656e 7445 7665 6e74     # ParentEvent
-00004a60: 5472 6565 436f 6c6c 6563 7469 6f6e 2069  TreeCollection i
-00004a70: 7320 6120 7472 6565 2063 6f6c 6c65 6374  s a tree collect
-00004a80: 696f 6e20 6c69 6b65 2045 7665 6e74 5472  ion like EventTr
-00004a90: 6565 436f 6c6c 6563 7469 6f6e 2c0a 2020  eeCollection,.  
-00004aa0: 2020 2020 2020 2320 6275 7420 6974 2068        # but it h
-00004ab0: 6173 206f 6e6c 7920 6576 656e 7473 2074  as only events t
-00004ac0: 6861 7420 6861 7665 2072 6566 6572 656e  hat have referen
-00004ad0: 6365 732e 0a20 2020 2020 2020 2064 6174  ces..        dat
-00004ae0: 615f 736f 7572 6365 3a20 4944 6174 6153  a_source: IDataS
-00004af0: 6f75 7263 6520 2023 2059 6f75 2073 686f  ource  # You sho
-00004b00: 756c 6420 696e 6974 2044 6174 6153 6f75  uld init DataSou
-00004b10: 7263 6520 6f62 6a65 6374 2e20 452e 672e  rce object. E.g.
-00004b20: 2066 726f 6d20 4c77 4450 206d 6f64 756c   from LwDP modul
-00004b30: 652e 0a20 2020 2020 2020 2023 2045 5443  e..        # ETC
-00004b40: 4472 6976 6572 2068 6572 6520 6973 2061  Driver here is a
-00004b50: 2073 7475 622c 2061 6374 7561 6c6c 7920   stub, actually 
-00004b60: 7468 6520 6c69 6220 646f 6e27 7420 6861  the lib don't ha
-00004b70: 7665 2073 7563 6820 636c 6173 732e 0a20  ve such class.. 
-00004b80: 2020 2020 2020 2023 2059 6f75 2063 616e         # You can
-00004b90: 2074 616b 6520 6974 2069 6e20 4c77 4450   take it in LwDP
-00004ba0: 206d 6f64 756c 6520 6f72 2063 7265 6174   module or creat
-00004bb0: 6520 796f 7572 7365 6c66 2063 6c61 7373  e yourself class
-00004bc0: 2069 6620 796f 7520 6861 7665 2073 6f6d   if you have som
-00004bd0: 6520 7370 6563 6961 6c20 6576 656e 7473  e special events
-00004be0: 2073 7472 7563 7475 7265 2e0a 2020 2020   structure..    
-00004bf0: 2020 2020 6672 6f6d 2074 6832 5f64 6174      from th2_dat
-00004c00: 615f 7365 7276 6963 6573 2e64 6174 615f  a_services.data_
-00004c10: 736f 7572 6365 2e6c 7764 702e 6576 656e  source.lwdp.even
-00004c20: 745f 7472 6565 2069 6d70 6f72 7420 4874  t_tree import Ht
-00004c30: 7470 4554 4344 7269 7665 7220 6173 2045  tpETCDriver as E
-00004c40: 5443 4472 6976 6572 0a20 2020 2020 2020  TCDriver.       
-00004c50: 200a 2020 2020 2020 2020 6472 6976 6572   .        driver
-00004c60: 203d 2045 5443 4472 6976 6572 2864 6174   = ETCDriver(dat
-00004c70: 615f 736f 7572 6365 3d64 6174 615f 736f  a_source=data_so
-00004c80: 7572 6365 290a 2020 2020 2020 2020 6574  urce).        et
-00004c90: 6320 3d20 5061 7265 6e74 4576 656e 7454  c = ParentEventT
-00004ca0: 7265 6543 6f6c 6c65 6374 696f 6e28 6472  reeCollection(dr
-00004cb0: 6976 6572 290a 2020 2020 2020 2020 6574  iver).        et
-00004cc0: 632e 6275 696c 6428 6576 656e 7473 290a  c.build(events).
-00004cd0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00004ce0: 2065 7463 2e73 686f 7728 290a 2020 2020   etc.show().    
-00004cf0: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-00004d00: 345d 2046 6965 6c64 2052 6573 6f6c 7665  4] Field Resolve
-00004d10: 7273 0a20 2020 2020 2020 2023 2050 6c65  rs.        # Ple
-00004d20: 6173 6520 7265 6164 2060 4669 656c 6420  ase read `Field 
-00004d30: 5265 736f 6c76 6572 7360 2062 6c6f 636b  Resolvers` block
-00004d40: 2069 6e20 7265 6164 6d65 2066 6972 7374   in readme first
-00004d50: 2e0a 2020 2020 2020 2020 2320 5b34 2e31  ..        # [4.1
-00004d60: 5d20 5573 6167 6520 6578 616d 706c 6520  ] Usage example 
-00004d70: 6672 6f6d 2063 6c69 656e 7420 636f 6465  from client code
-00004d80: 0a20 2020 2020 2020 2066 726f 6d20 7468  .        from th
-00004d90: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
-00004da0: 6461 7461 5f73 6f75 7263 6520 696d 706f  data_source impo
-00004db0: 7274 2028 0a20 2020 2020 2020 2020 2020  rt (.           
-00004dc0: 206c 7764 702c 0a20 2020 2020 2020 2029   lwdp,.        )
-00004dd0: 2020 2320 6c77 6470 2064 6174 615f 736f    # lwdp data_so
-00004de0: 7572 6365 2069 6e69 7469 616c 697a 6520  urce initialize 
-00004df0: 7468 325f 6461 7461 5f73 6572 7669 6365  th2_data_service
-00004e00: 732e 636f 6e66 6967 2064 7572 696e 6720  s.config during 
-00004e10: 696d 706f 7274 2e0a 2020 2020 2020 2020  import..        
-00004e20: 6672 6f6d 2074 6832 5f64 6174 615f 7365  from th2_data_se
-00004e30: 7276 6963 6573 2e63 6f6e 6669 6720 696d  rvices.config im
-00004e40: 706f 7274 206f 7074 696f 6e73 2061 7320  port options as 
-00004e50: 6f5f 0a20 2020 2020 2020 200a 2020 2020  o_.        .    
-00004e60: 2020 2020 666f 7220 6d20 696e 2064 6174      for m in dat
-00004e70: 613a 0a20 2020 2020 2020 2020 2020 206f  a:.            o
-00004e80: 5f2e 6d66 722e 6578 7061 6e64 5f6d 6573  _.mfr.expand_mes
-00004e90: 7361 6765 286d 2920 2023 206d 6672 202d  sage(m)  # mfr -
-00004ea0: 2073 7461 6e64 7320 666f 7220 4d65 7373   stands for Mess
-00004eb0: 6167 6546 6965 6c64 5265 736f 6c76 6572  ageFieldResolver
-00004ec0: 0a20 2020 2020 2020 2020 2020 2023 206f  .            # o
-00004ed0: 720a 2020 2020 2020 2020 2020 2020 6f5f  r.            o_
-00004ee0: 2e65 6d66 722e 6578 7061 6e64 5f6d 6573  .emfr.expand_mes
-00004ef0: 7361 6765 286d 2920 2023 2065 6d66 7220  sage(m)  # emfr 
-00004f00: 2d20 7374 616e 6473 2066 6f72 2045 7870  - stands for Exp
-00004f10: 616e 6465 644d 6573 7361 6765 4669 656c  andedMessageFiel
-00004f20: 6452 6573 6f6c 7665 720a 2020 2020 2020  dResolver.      
-00004f30: 2020 0a20 2020 2020 2020 2023 205b 342e    .        # [4.
-00004f40: 325d 204c 6962 7261 7269 6573 2075 7361  2] Libraries usa
-00004f50: 6765 2e0a 2020 2020 2020 2020 2320 446f  ge..        # Do
-00004f60: 6e27 7420 696d 706f 7274 2065 7861 6374  n't import exact
-00004f70: 2072 6573 6f6c 7665 7273 2069 6d70 6c65   resolvers imple
-00004f80: 6d65 6e74 6174 696f 6e20 706c 6561 7365  mentation please
-00004f90: 2069 6e20 796f 7572 2063 6f64 652e 0a20   in your code.. 
-00004fa0: 2020 2020 2020 2023 2041 6c6c 6f77 2079         # Allow y
-00004fb0: 6f75 7220 636c 6965 6e74 2074 6f20 646f  our client to do
-00004fc0: 2069 7420 696e 7374 6561 642e 0a20 2020   it instead..   
-00004fd0: 2020 2020 2023 204a 7573 7420 696d 706f       # Just impo
-00004fe0: 7274 2060 6f70 7469 6f6e 7360 2066 726f  rt `options` fro
-00004ff0: 6d20 6074 6832 5f64 6174 615f 7365 7276  m `th2_data_serv
-00005000: 6963 6573 2e63 6f6e 6669 6760 2061 6e64  ices.config` and
-00005010: 2075 7365 2069 742e 0a20 2020 2020 2020   use it..       
-00005020: 2066 726f 6d20 7468 325f 6461 7461 5f73   from th2_data_s
-00005030: 6572 7669 6365 732e 636f 6e66 6967 2069  ervices.config i
-00005040: 6d70 6f72 7420 6f70 7469 6f6e 7320 6173  mport options as
-00005050: 206f 5f0a 2020 2020 2020 2020 0a20 2020   o_.        .   
-00005060: 2020 2020 2066 6f72 206d 2069 6e20 6461       for m in da
-00005070: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
-00005080: 6f5f 2e6d 6672 2e65 7870 616e 645f 6d65  o_.mfr.expand_me
-00005090: 7373 6167 6528 6d29 0a20 2020 2020 2020  ssage(m).       
-000050a0: 2020 2020 2023 206f 720a 2020 2020 2020       # or.      
-000050b0: 2020 2020 2020 6f5f 2e65 6d66 722e 6578        o_.emfr.ex
-000050c0: 7061 6e64 5f6d 6573 7361 6765 286d 290a  pand_message(m).
-000050d0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000050e0: 2023 204d 6f72 6520 7465 6368 2064 6574   # More tech det
-000050f0: 6169 6c73 3a0a 2020 2020 2020 2020 2320  ails:.        # 
-00005100: 2020 496e 2074 6869 7320 6361 7365 2c20    In this case, 
-00005110: 7468 6572 6520 6973 206e 6f20 6c69 6e65  there is no line
-00005120: 2060 6672 6f6d 2074 6832 5f64 6174 615f   `from th2_data_
-00005130: 7365 7276 6963 6573 2e64 6174 615f 736f  services.data_so
-00005140: 7572 6365 2069 6d70 6f72 7420 6c77 6470  urce import lwdp
-00005150: 2060 0a20 2020 2020 2020 2023 2020 2062   `.        #   b
-00005160: 6563 6175 7365 2077 6520 7368 6f75 6c64  ecause we should
-00005170: 206e 6f74 2063 686f 6f73 6520 666f 7220   not choose for 
-00005180: 7468 6520 7573 6572 2077 6869 6368 2064  the user which d
-00005190: 6174 6120 736f 7572 6365 2074 6f20 7573  ata source to us
-000051a0: 652e 0a20 2020 2020 2020 2023 2020 2057  e..        #   W
-000051b0: 6520 646f 206e 6f74 206b 6e6f 7720 7768  e do not know wh
-000051c0: 6174 2068 6520 7769 6c6c 2063 686f 6f73  at he will choos
-000051d0: 652c 2074 6865 7265 666f 7265 2077 6520  e, therefore we 
-000051e0: 6d75 7374 2073 696d 706c 7920 6163 6365  must simply acce
-000051f0: 7373 0a20 2020 2020 2020 2023 2020 2074  ss.        #   t
-00005200: 6865 2069 6e74 6572 6661 6365 2c20 7768  he interface, wh
-00005210: 6963 6820 7769 6c6c 2062 6520 696e 6974  ich will be init
-00005220: 6961 6c69 7a65 6420 6279 2074 6865 2075  ialized by the u
-00005230: 7365 722e 0a20 2020 2020 2020 200a 2020  ser..        .  
-00005240: 2020 2020 2020 2320 5b35 5d20 5573 696e        # [5] Usin
-00005250: 6720 7574 696c 6974 7920 6675 6e63 7469  g utility functi
-00005260: 6f6e 732e 0a20 2020 2020 2020 2066 726f  ons..        fro
-00005270: 6d20 7468 325f 6461 7461 5f73 6572 7669  m th2_data_servi
-00005280: 6365 732e 7574 696c 732e 6576 656e 745f  ces.utils.event_
-00005290: 7574 696c 732e 6672 6571 7565 6e63 6965  utils.frequencie
-000052a0: 7320 696d 706f 7274 2067 6574 5f63 6174  s import get_cat
-000052b0: 6567 6f72 795f 6672 6571 7565 6e63 6965  egory_frequencie
-000052c0: 7332 0a20 2020 2020 2020 2066 726f 6d20  s2.        from 
-000052d0: 7468 325f 6461 7461 5f73 6572 7669 6365  th2_data_service
-000052e0: 732e 7574 696c 732e 6576 656e 745f 7574  s.utils.event_ut
-000052f0: 696c 732e 746f 7461 6c73 2069 6d70 6f72  ils.totals impor
-00005300: 7420 6765 745f 6361 7465 676f 7279 5f74  t get_category_t
-00005310: 6f74 616c 7332 0a20 2020 2020 2020 2066  otals2.        f
-00005320: 726f 6d20 7468 325f 6461 7461 5f73 6572  rom th2_data_ser
-00005330: 7669 6365 732e 7574 696c 732e 6361 7465  vices.utils.cate
-00005340: 676f 7279 2069 6d70 6f72 7420 4361 7465  gory import Cate
-00005350: 676f 7279 0a20 2020 2020 2020 2066 726f  gory.        fro
-00005360: 6d20 7468 325f 6461 7461 5f73 6572 7669  m th2_data_servi
-00005370: 6365 732e 7574 696c 732e 6576 656e 745f  ces.utils.event_
-00005380: 7574 696c 732e 6576 656e 745f 7574 696c  utils.event_util
-00005390: 7320 696d 706f 7274 2069 735f 736f 7274  s import is_sort
-000053a0: 6564 0a20 2020 2020 2020 200a 2020 2020  ed.        .    
-000053b0: 2020 2020 2320 5b35 2e31 5d20 4765 7420      # [5.1] Get 
-000053c0: 7468 6520 7175 616e 7469 7469 6573 206f  the quantities o
-000053d0: 6620 6576 656e 7473 2066 6f72 2064 6966  f events for dif
-000053e0: 6665 7265 6e74 2063 6174 6567 6f72 6965  ferent categorie
-000053f0: 732e 0a20 2020 2020 2020 206d 6574 7269  s..        metri
-00005400: 6373 203d 205b 0a20 2020 2020 2020 2020  cs = [.         
-00005410: 2020 2043 6174 6567 6f72 7928 2264 6174     Category("dat
-00005420: 6522 2c20 6c61 6d62 6461 206d 3a20 5468  e", lambda m: Th
-00005430: 3254 696d 6573 7461 6d70 436f 6e76 6572  2TimestampConver
-00005440: 7465 722e 746f 5f64 6174 6574 696d 6528  ter.to_datetime(
-00005450: 6d5b 2273 7461 7274 5469 6d65 7374 616d  m["startTimestam
-00005460: 7022 5d29 2e64 6174 6528 2929 2c0a 2020  p"]).date()),.  
-00005470: 2020 2020 2020 2020 2020 4361 7465 676f            Catego
-00005480: 7279 2822 7374 6174 7573 222c 206c 616d  ry("status", lam
-00005490: 6264 6120 6d3a 206d 5b22 7375 6363 6573  bda m: m["succes
-000054a0: 7366 756c 225d 292c 0a20 2020 2020 2020  sful"]),.       
-000054b0: 205d 0a20 2020 2020 2020 2063 6174 6567   ].        categ
-000054c0: 6f72 795f 746f 7461 6c73 203d 2067 6574  ory_totals = get
-000054d0: 5f63 6174 6567 6f72 795f 746f 7461 6c73  _category_totals
-000054e0: 3228 6576 656e 7473 2c20 6d65 7472 6963  2(events, metric
-000054f0: 7329 0a20 2020 2020 2020 2022 2222 0a20  s).        """. 
-00005500: 2020 2020 2020 202b 2d2d 2d2d 2d2d 2d2d         +--------
-00005510: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  +------------+--
-00005520: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00005530: 2d2d 2b0a 2020 2020 2020 2020 7c20 2020  --+.        |   
-00005540: 2020 2020 207c 2064 6174 6520 2020 2020       | date     
-00005550: 2020 7c20 7374 6174 7573 2020 207c 2020    | status   |  
-00005560: 2063 6f75 6e74 207c 0a20 2020 2020 2020   count |.       
-00005570: 202b 3d3d 3d3d 3d3d 3d3d 2b3d 3d3d 3d3d   +========+=====
-00005580: 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d  =======+========
-00005590: 3d3d 2b3d 3d3d 3d3d 3d3d 3d3d 2b0a 2020  ==+=========+.  
-000055a0: 2020 2020 2020 7c20 2020 2020 2020 207c        |        |
-000055b0: 2032 3032 332d 3031 2d30 3520 7c20 5472   2023-01-05 | Tr
-000055c0: 7565 2020 2020 207c 2020 2020 2020 2033  ue     |       3
-000055d0: 207c 0a20 2020 2020 2020 202b 2d2d 2d2d   |.        +----
-000055e0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-000055f0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  -+----------+---
-00005600: 2d2d 2d2d 2d2d 2b0a 2020 2020 2020 2020  ------+.        
-00005610: 7c20 636f 756e 7420 207c 2020 2020 2020  | count  |      
-00005620: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00005630: 207c 2020 2020 2020 2031 207c 0a20 2020   |       1 |.   
-00005640: 2020 2020 202b 2d2d 2d2d 2d2d 2d2d 2b2d       +--------+-
-00005650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
-00005660: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
-00005670: 2b0a 2020 2020 2020 2020 7c20 746f 7461  +.        | tota
-00005680: 6c73 207c 2020 2020 2020 2020 2020 2020  ls |            
-00005690: 7c20 312f 3020 2020 2020 207c 2020 2020  | 1/0      |    
-000056a0: 2020 2033 207c 0a20 2020 2020 2020 202b     3 |.        +
-000056b0: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-000056c0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
-000056d0: 2b2d 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020  +---------+.    
-000056e0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000056f0: 0a20 2020 2020 2020 2023 205b 352e 325d  .        # [5.2]
-00005700: 2047 6574 2074 6865 206e 756d 6265 7220   Get the number 
-00005710: 6f66 2065 7665 6e74 7320 7769 7468 2073  of events with s
-00005720: 7461 7475 7320 7375 6363 6573 7366 756c  tatus successful
-00005730: 2e0a 2020 2020 2020 2020 6361 7465 676f  ..        catego
-00005740: 7279 203d 2043 6174 6567 6f72 7928 2273  ry = Category("s
-00005750: 7461 7475 7322 2c20 6c61 6d62 6461 206d  tatus", lambda m
-00005760: 3a20 6d5b 2273 7563 6365 7373 6675 6c22  : m["successful"
-00005770: 5d29 0a20 2020 2020 2020 2063 6174 6567  ]).        categ
-00005780: 6f72 795f 6672 6571 7565 6e63 6965 7320  ory_frequencies 
-00005790: 3d20 6765 745f 6361 7465 676f 7279 5f66  = get_category_f
-000057a0: 7265 7175 656e 6369 6573 3228 6576 656e  requencies2(even
-000057b0: 7473 2c20 6361 7465 676f 7279 290a 2020  ts, category).  
-000057c0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000057d0: 2020 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d    +--------+----
-000057e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000057f0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-00005800: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-00005810: 2b0a 2020 2020 2020 2020 7c20 2020 2020  +.        |     
-00005820: 2020 207c 2074 696d 6573 7461 6d70 5f73     | timestamp_s
-00005830: 7461 7274 2020 2020 207c 2074 696d 6573  tart     | times
-00005840: 7461 6d70 5f65 6e64 2020 2020 2020 207c  tamp_end       |
-00005850: 2020 2054 7275 6520 7c0a 2020 2020 2020     True |.      
-00005860: 2020 2b3d 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d    +========+====
-00005870: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00005880: 3d2b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  =+==============
-00005890: 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d  =======+========
-000058a0: 2b0a 2020 2020 2020 2020 7c20 2020 2020  +.        |     
-000058b0: 2020 207c 2032 3032 332d 3031 2d30 3554     | 2023-01-05T
-000058c0: 3133 3a35 373a 3035 207c 2032 3032 332d  13:57:05 | 2023-
-000058d0: 3031 2d30 3554 3133 3a35 373a 3036 207c  01-05T13:57:06 |
-000058e0: 2020 2020 2020 3320 7c0a 2020 2020 2020        3 |.      
-000058f0: 2020 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d    +--------+----
-00005900: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005910: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-00005920: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-00005930: 2b0a 2020 2020 2020 2020 7c20 636f 756e  +.        | coun
-00005940: 7420 207c 2020 2020 2020 2020 2020 2020  t  |            
-00005950: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00005960: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00005970: 2020 2020 2020 3120 7c0a 2020 2020 2020        1 |.      
-00005980: 2020 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d    +--------+----
-00005990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000059a0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-000059b0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-000059c0: 2b0a 2020 2020 2020 2020 7c20 746f 7461  +.        | tota
-000059d0: 6c73 207c 2020 2020 2020 2020 2020 2020  ls |            
-000059e0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-000059f0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00005a00: 2020 2020 2020 3320 7c0a 2020 2020 2020        3 |.      
-00005a10: 2020 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d    +--------+----
-00005a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005a30: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-00005a40: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-00005a50: 2b0a 2020 2020 2020 2020 2222 220a 2020  +.        """.  
-00005a60: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-00005a70: 205b 352e 335d 2043 6865 636b 2069 6620   [5.3] Check if 
-00005a80: 6576 656e 7473 2061 7265 2073 6f72 7465  events are sorte
-00005a90: 642e 0a20 2020 2020 2020 2072 6573 756c  d..        resul
-00005aa0: 7420 3d20 6973 5f73 6f72 7465 6428 6576  t = is_sorted(ev
-00005ab0: 656e 7473 290a 2020 2020 2020 2020 6060  ents).        ``
-00005ac0: 600a 2020 2020 2020 2020 3c21 2d2d 2065  `.        <!-- e
-00005ad0: 6e64 2067 6574 5f73 7461 7274 6564 5f65  nd get_started_e
-00005ae0: 7861 6d70 6c65 2e70 7920 2d2d 3e0a 2020  xample.py -->.  
-00005af0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-00005b00: 2320 322e 332e 2053 686f 7274 2074 6865  # 2.3. Short the
-00005b10: 6f72 790a 2020 2020 2020 2020 0a20 2020  ory.        .   
-00005b20: 2020 2020 2054 6865 206c 6962 7261 7279       The library
-00005b30: 2070 726f 7669 6465 7320 746f 6f6c 7320   provides tools 
-00005b40: 666f 7220 6861 6e64 6c69 6e67 2073 7472  for handling str
-00005b50: 6561 6d20 6461 7461 2e20 5768 6174 2773  eam data. What's
-00005b60: 2061 2073 7472 6561 6d3f 2049 7427 7320   a stream? It's 
-00005b70: 6120 7365 7175 656e 6365 206f 6620 656c  a sequence of el
-00005b80: 656d 656e 7473 2066 726f 6d20 6120 736f  ements from a so
-00005b90: 7572 6365 2074 6861 740a 2020 2020 2020  urce that.      
-00005ba0: 2020 7375 7070 6f72 7473 2061 6767 7265    supports aggre
-00005bb0: 6761 7465 206f 7065 7261 7469 6f6e 732e  gate operations.
-00005bc0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00005bd0: 2020 2323 2320 5465 726d 730a 2020 2020    ### Terms.    
-00005be0: 2020 2020 0a20 2020 2020 2020 202d 202a      .        - *
-00005bf0: 2a44 6174 6120 6f62 6a65 6374 2a2a 3a20  *Data object**: 
-00005c00: 416e 2069 6e73 7461 6e63 6520 6f66 2060  An instance of `
-00005c10: 4461 7461 6020 636c 6173 7320 7768 6963  Data` class whic
-00005c20: 6820 6973 2077 7261 7070 6572 2075 6e64  h is wrapper und
-00005c30: 6572 2073 7472 6561 6d2e 0a20 2020 2020  er stream..     
-00005c40: 2020 202d 202a 2a53 6571 7565 6e63 6520     - **Sequence 
-00005c50: 6f66 2065 6c65 6d65 6e74 732a 2a3a 0a20  of elements**:. 
-00005c60: 2020 2020 2020 2020 2041 205f 4461 7461           A _Data
-00005c70: 206f 626a 6563 745f 2070 726f 7669 6465   object_ provide
-00005c80: 7320 616e 2069 6e74 6572 6661 6365 2074  s an interface t
-00005c90: 6f20 6120 7365 7175 656e 6365 6420 7365  o a sequenced se
-00005ca0: 7420 6f66 2076 616c 7565 7320 6f66 2061  t of values of a
-00005cb0: 2073 7065 6369 6669 6320 656c 656d 656e   specific elemen
-00005cc0: 7420 7479 7065 2e20 5374 7265 616d 2069  t type. Stream i
-00005cd0: 6e73 6964 6520 7468 6520 5f44 6174 610a  nside the _Data.
-00005ce0: 2020 2020 2020 2020 2020 6f62 6a65 6374            object
-00005cf0: 5f20 2a2a 646f 6e19 7420 6163 7475 616c  _ **don.t actual
-00005d00: 6c79 2073 746f 7265 2a2a 2065 6c65 6d65  ly store** eleme
-00005d10: 6e74 733b 2074 6865 7920 6172 6520 636f  nts; they are co
-00005d20: 6d70 7574 6564 206f 6e20 6465 6d61 6e64  mputed on demand
-00005d30: 2e0a 2020 2020 2020 2020 2d20 2a2a 6461  ..        - **da
-00005d40: 7461 2073 6f75 7263 652a 2a20 2865 7861  ta source** (exa
-00005d50: 6374 6c79 2069 6e20 736d 616c 6c20 6c65  ctly in small le
-00005d60: 7474 6572 7329 3a0a 2020 2020 2020 2020  tters):.        
-00005d70: 2020 416e 7920 736f 7572 6365 206f 6620    Any source of 
-00005d80: 6461 7461 2e20 452e 672e 205b 4c69 6768  data. E.g. [Ligh
-00005d90: 7477 6569 6768 7420 4461 7461 2050 726f  tweight Data Pro
-00005da0: 7669 6465 725d 2868 7474 7073 3a2f 2f67  vider](https://g
-00005db0: 6974 6875 622e 636f 6d2f 7468 322d 6e65  ithub.com/th2-ne
-00005dc0: 742f 7468 322d 6c77 2d64 6174 612d 7072  t/th2-lw-data-pr
-00005dd0: 6f76 6964 6572 292c 2063 6f6c 6c65 6374  ovider), collect
-00005de0: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
-00005df0: 6172 7261 7973 2c20 6f72 2049 2f4f 2072  arrays, or I/O r
-00005e00: 6573 6f75 7263 6573 2e0a 2020 2020 2020  esources..      
-00005e10: 2020 2d20 2a2a 4461 7461 536f 7572 6365    - **DataSource
-00005e20: 2a2a 3a0a 2020 2020 2020 2020 2020 4120  **:.          A 
-00005e30: 636c 6173 7320 7468 6174 2069 7320 616e  class that is an
-00005e40: 2069 6e74 6572 6d65 6469 6174 6520 6c69   intermediate li
-00005e50: 6e6b 2062 6574 7765 656e 2074 6865 2053  nk between the S
-00005e60: 6f75 7263 6541 5049 2061 6e64 2043 6f6d  ourceAPI and Com
-00005e70: 6d61 6e64 732e 0a20 2020 2020 2020 202d  mands..        -
-00005e80: 202a 2a53 6f75 7263 6541 5049 2a2a 3a0a   **SourceAPI**:.
-00005e90: 2020 2020 2020 2020 2020 4561 6368 2073            Each s
-00005ea0: 6f75 7263 6520 6861 7320 6974 7320 6f77  ource has its ow
-00005eb0: 6e20 4150 4920 746f 2072 6574 7269 6576  n API to retriev
-00005ec0: 6520 6461 7461 2e20 536f 7572 6365 4150  e data. SourceAP
-00005ed0: 4920 6973 2061 2063 6c61 7373 2074 6861  I is a class tha
-00005ee0: 7420 7072 6f76 6964 6520 4150 4920 666f  t provide API fo
-00005ef0: 7220 736f 6d65 2064 6174 6120 736f 7572  r some data sour
-00005f00: 6365 2e0a 2020 2020 2020 2020 2d20 2a2a  ce..        - **
-00005f10: 436f 6d6d 616e 6473 2a2a 3a0a 2020 2020  Commands**:.    
-00005f20: 2020 2020 2020 436c 6173 7365 7320 7468        Classes th
-00005f30: 6174 2070 726f 7669 6465 2075 7365 722d  at provide user-
-00005f40: 6672 6965 6e64 6c79 2069 6e74 6572 6661  friendly interfa
-00005f50: 6365 7320 666f 7220 6765 7474 696e 6720  ces for getting 
-00005f60: 736f 6d65 2064 6174 6120 6672 6f6d 2044  some data from D
-00005f70: 6174 6153 6f75 7263 652e 2043 6f6d 6d61  ataSource. Comma
-00005f80: 6e64 7320 7573 6520 5f53 6f75 7263 6541  nds use _SourceA
-00005f90: 5049 5f20 746f 0a20 2020 2020 2020 2020  PI_ to.         
-00005fa0: 2061 6368 6965 7665 2069 742e 0a20 2020   achieve it..   
-00005fb0: 2020 2020 202d 202a 2a41 6461 7074 6572       - **Adapter
-00005fc0: 732a 2a3a 0a20 2020 2020 2020 2020 2049  s**:.          I
-00005fd0: 7427 7320 7369 6d69 6c61 7220 746f 2066  t's similar to f
-00005fe0: 756e 6374 696f 6e20 666f 7220 6044 6174  unction for `Dat
-00005ff0: 612e 6d61 7060 206d 6574 686f 642e 2041  a.map` method. A
-00006000: 646f 7074 6162 6c65 2063 6f6d 6d61 6e64  doptable command
-00006010: 7320 7573 6564 2069 7420 746f 2075 7064  s used it to upd
-00006020: 6174 6520 7468 6520 6461 7461 2073 7472  ate the data str
-00006030: 6561 6d2e 0a20 2020 2020 2020 202d 202a  eam..        - *
-00006040: 2a41 6767 7265 6761 7465 206f 7065 7261  *Aggregate opera
-00006050: 7469 6f6e 732a 2a3a 0a20 2020 2020 2020  tions**:.       
-00006060: 2020 2043 6f6d 6d6f 6e20 6f70 6572 6174     Common operat
-00006070: 696f 6e73 2073 7563 6820 6173 2066 696c  ions such as fil
-00006080: 7465 722c 206d 6170 2c20 6c69 6d69 7420  ter, map, limit 
-00006090: 616e 6420 736f 206f 6e2e 0a20 2020 2020  and so on..     
-000060a0: 2020 202d 202a 2a57 6f72 6b66 6c6f 772a     - **Workflow*
-000060b0: 2a3a 2041 6e20 6f72 6465 7265 6420 7365  *: An ordered se
-000060c0: 7420 6f66 205f 4167 6772 6567 6174 6520  t of _Aggregate 
-000060d0: 6f70 6572 6174 696f 6e73 5f2e 0a20 2020  operations_..   
-000060e0: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-000060f0: 2320 436f 6e63 6570 740a 2020 2020 2020  # Concept.      
-00006100: 2020 0a20 2020 2020 2020 2054 6865 206c    .        The l
-00006110: 6962 7261 7279 2064 6573 6372 6962 6573  ibrary describes
-00006120: 2074 6865 2068 6967 682d 6c65 7665 6c20   the high-level 
-00006130: 696e 7465 7266 6163 6573 2060 4953 6f75  interfaces `ISou
-00006140: 7263 6541 5049 602c 2060 4944 6174 6153  rceAPI`, `IDataS
-00006150: 6f75 7263 6560 2c20 6049 436f 6d6d 616e  ource`, `IComman
-00006160: 6460 2c20 6049 4164 6170 7465 7260 2e0a  d`, `IAdapter`..
-00006170: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00006180: 2041 6e79 2064 6174 6120 736f 7572 6365   Any data source
-00006190: 206d 7573 7420 6265 2064 6573 6372 6962   must be describ
-000061a0: 6564 2062 7920 7468 6520 6049 4461 7461  ed by the `IData
-000061b0: 536f 7572 6365 6020 6162 7374 7261 6374  Source` abstract
-000061c0: 2063 6c61 7373 2e20 5468 6573 6520 6361   class. These ca
-000061d0: 6e20 6265 205f 4669 6c65 4461 7461 536f  n be _FileDataSo
-000061e0: 7572 6365 5f2c 0a20 2020 2020 2020 205f  urce_,.        _
-000061f0: 4353 5644 6174 6153 6f75 7263 655f 2c20  CSVDataSource_, 
-00006200: 5f44 4244 6174 6153 6f75 7263 655f 2061  _DBDataSource_ a
-00006210: 6e64 206f 7468 6572 2e0a 2020 2020 2020  nd other..      
-00006220: 2020 0a20 2020 2020 2020 2055 7375 616c    .        Usual
-00006230: 6c79 2c20 6461 7461 2073 6f75 7263 6573  ly, data sources
-00006240: 2068 6176 6520 736f 6d65 206b 696e 6420   have some kind 
-00006250: 6f66 2041 5049 2e20 4461 7461 6261 7365  of API. Database
-00006260: 7320 2d20 7072 6f76 6964 6520 5351 4c20  s - provide SQL 
-00006270: 6c61 6e67 7561 6765 2c20 7768 656e 2077  language, when w
-00006280: 6f72 6b69 6e67 2077 6974 6820 6120 6669  orking with a fi
-00006290: 6c65 2c20 796f 7520 6361 6e20 7265 6164  le, you can read
-000062a0: 0a20 2020 2020 2020 206c 696e 6520 6279  .        line by
-000062b0: 206c 696e 652c 2065 7463 2e20 5468 6973   line, etc. This
-000062c0: 2041 5049 2069 7320 6465 7363 7269 6265   API is describe
-000062d0: 6420 6279 2074 6865 2060 4953 6f75 7263  d by the `ISourc
-000062e0: 6541 5049 6020 636c 6173 732e 2042 6563  eAPI` class. Bec
-000062f0: 6175 7365 2064 6966 6665 7265 6e74 2076  ause different v
-00006300: 6572 7369 6f6e 7320 6f66 2074 6865 2073  ersions of the s
-00006310: 616d 6520 6461 7461 2073 6f75 7263 650a  ame data source.
-00006320: 2020 2020 2020 2020 6d61 7920 6861 7665          may have
-00006330: 2064 6966 6665 7265 6e74 2041 5049 2c20   different API, 
-00006340: 6974 2069 7320 6265 7474 6572 2074 6f20  it is better to 
-00006350: 6372 6561 7465 2061 2063 6c61 7373 2066  create a class f
-00006360: 6f72 2065 6163 6820 7665 7273 696f 6e2e  or each version.
-00006370: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00006380: 2020 4765 6e65 7261 6c6c 792c 2064 6174    Generally, dat
-00006390: 6120 736f 7572 6365 2041 5049 7320 6172  a source APIs ar
-000063a0: 6520 6869 6464 656e 2062 6568 696e 6420  e hidden behind 
-000063b0: 636f 6e76 656e 6965 6e74 2069 6e74 6572  convenient inter
-000063c0: 6661 6365 732e 2054 6865 2072 6f6c 6520  faces. The role 
-000063d0: 6f66 2074 6865 7365 2069 6e74 6572 6661  of these interfa
-000063e0: 6365 7320 6973 2070 6c61 7965 640a 2020  ces is played.  
-000063f0: 2020 2020 2020 6279 2060 4943 6f6d 6d61        by `IComma
-00006400: 6e64 6020 636c 6173 7365 732e 0a20 2020  nd` classes..   
-00006410: 2020 2020 200a 2020 2020 2020 2020 6049       .        `I
-00006420: 4164 6170 7465 7260 2063 6c61 7373 6573  Adapter` classes
-00006430: 2074 7261 6e73 666f 726d 2064 6174 6120   transform data 
-00006440: 7374 7265 616d 206c 696b 6520 6675 6e63  stream like func
-00006450: 7469 6f6e 7320 666f 7220 6044 6174 612e  tions for `Data.
-00006460: 6d61 7060 206d 6574 686f 642e 2045 7373  map` method. Ess
-00006470: 656e 7469 616c 6c79 2069 7427 7320 7468  entially it's th
-00006480: 6520 7361 6d65 2074 6869 6e67 2062 7574  e same thing but
-00006490: 206d 6f72 650a 2020 2020 2020 2020 666c   more.        fl
-000064a0: 6578 6962 6c65 2e0a 2020 2020 2020 2020  exible..        
-000064b0: 0a20 2020 2020 2020 2046 6f72 2065 7861  .        For exa
-000064c0: 6d70 6c65 2c20 4c77 4450 2044 6174 6153  mple, LwDP DataS
-000064d0: 6f75 7263 6528 6874 7470 733a 2f2f 6769  ource(https://gi
-000064e0: 7468 7562 2e63 6f6d 2f74 6832 2d6e 6574  thub.com/th2-net
-000064f0: 2f74 6832 2d64 732d 736f 7572 6365 2d6c  /th2-ds-source-l
-00006500: 7764 7029 2075 7365 7320 7468 6573 6520  wdp) uses these 
-00006510: 6162 7374 7261 6374 2063 6c61 7373 6573  abstract classes
-00006520: 2074 6f20 6275 696c 6420 6974 7320 696d   to build its im
-00006530: 706c 656d 656e 7461 7469 6f6e 2e59 6f75  plementation.You
-00006540: 2063 616e 2065 6173 696c 7920 6372 6561   can easily crea
-00006550: 7465 2079 6f75 7220 6f77 6e20 756e 6971  te your own uniq
-00006560: 7565 2063 6f6d 6d61 6e64 7320 666f 7220  ue commands for 
-00006570: 5f4c 7744 5020 4461 7461 536f 7572 6365  _LwDP DataSource
-00006580: 5f2c 2061 7320 7765 6c6c 2061 7320 656e  _, as well as en
-00006590: 7469 7265 0a20 2020 2020 2020 205f 4461  tire.        _Da
-000065a0: 7461 536f 7572 6365 5f20 636c 6173 7365  taSource_ classe
-000065b0: 732e 205b 4865 7265 2069 7320 6120 646f  s. [Here is a do
-000065c0: 6375 6d65 6e74 6174 696f 6e5d 2864 6f63  cumentation](doc
-000065d0: 756d 656e 7461 7469 6f6e 2f64 6174 6173  umentation/datas
-000065e0: 6f75 7263 652e 6d64 2920 6f6e 2068 6f77  ource.md) on how
-000065f0: 2074 6f20 696d 706c 656d 656e 7420 7468   to implement th
-00006600: 6573 6520 696e 7465 7266 6163 6573 2e0a  ese interfaces..
-00006610: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00006620: 2021 5b44 6174 6120 7374 7265 616d 2070   ![Data stream p
-00006630: 6970 656c 696e 655d 2864 6f63 756d 656e  ipeline](documen
-00006640: 7461 7469 6f6e 2f69 6d67 2f63 6f6e 6365  tation/img/conce
-00006650: 7074 2e70 6e67 290a 2020 2020 2020 2020  pt.png).        
-00006660: 0a20 2020 2020 2020 2023 2323 2053 7472  .        ### Str
-00006670: 6561 6d20 6f70 6572 6174 696f 6e73 0a20  eam operations. 
-00006680: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006690: 4675 7274 6865 726d 6f72 652c 2073 7472  Furthermore, str
-000066a0: 6561 6d20 6f70 6572 6174 696f 6e73 2068  eam operations h
-000066b0: 6176 6520 7477 6f20 6675 6e64 616d 656e  ave two fundamen
-000066c0: 7461 6c20 6368 6172 6163 7465 7269 7374  tal characterist
-000066d0: 6963 7320 7468 6174 206d 616b 6520 7468  ics that make th
-000066e0: 656d 2076 6572 7920 6469 6666 6572 656e  em very differen
-000066f0: 7420 6672 6f6d 2063 6f6c 6c65 6374 696f  t from collectio
-00006700: 6e0a 2020 2020 2020 2020 6f70 6572 6174  n.        operat
-00006710: 696f 6e73 3a20 5f50 6970 656c 696e 696e  ions: _Pipelinin
-00006720: 675f 2061 6e64 205f 496e 7465 726e 616c  g_ and _Internal
-00006730: 2069 7465 7261 7469 6f6e 5f2e 0a20 2020   iteration_..   
-00006740: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-00006750: 2323 2050 6970 656c 696e 696e 670a 2020  ## Pipelining.  
-00006760: 2020 2020 2020 0a20 2020 2020 2020 204d        .        M
-00006770: 616e 7920 7374 7265 616d 206f 7065 7261  any stream opera
-00006780: 7469 6f6e 7320 7265 7475 726e 2061 2073  tions return a s
-00006790: 7472 6561 6d20 7468 656d 7365 6c76 6573  tream themselves
-000067a0: 2e20 5468 6973 2061 6c6c 6f77 7320 6f70  . This allows op
-000067b0: 6572 6174 696f 6e73 2074 6f20 6265 2063  erations to be c
-000067c0: 6861 696e 6564 2074 6f20 666f 726d 2061  hained to form a
-000067d0: 206c 6172 6765 7220 7069 7065 6c69 6e65   larger pipeline
-000067e0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-000067f0: 2020 2021 5b44 6174 6120 7374 7265 616d     ![Data stream
-00006800: 2070 6970 656c 696e 655d 2864 6f63 756d   pipeline](docum
-00006810: 656e 7461 7469 6f6e 2f69 6d67 2f64 6174  entation/img/dat
-00006820: 615f 7374 7265 616d 5f70 6970 656c 696e  a_stream_pipelin
-00006830: 652e 706e 6729 0a20 2020 2020 2020 200a  e.png).        .
-00006840: 2020 2020 2020 2020 2323 2323 2049 6e74          #### Int
-00006850: 6572 6e61 6c20 6974 6572 6174 696f 6e0a  ernal iteration.
+000018c0: 2020 2020 2262 6174 6368 4964 223a 204e      "batchId": N
+000018d0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+000018e0: 2020 2020 2020 2020 2022 6973 4261 7463           "isBatc
+000018f0: 6865 6422 3a20 4661 6c73 652c 0a20 2020  hed": False,.   
+00001900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001910: 2022 6576 656e 744e 616d 6522 3a20 2253   "eventName": "S
+00001920: 6574 206f 6620 6175 746f 2d67 656e 6572  et of auto-gener
+00001930: 6174 6564 2065 7665 6e74 7320 666f 7220  ated events for 
+00001940: 6473 206c 6962 2074 6573 7469 6e67 222c  ds lib testing",
+00001950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001960: 2020 2020 2022 6576 656e 7454 7970 6522       "eventType"
+00001970: 3a20 2264 732d 6c69 622d 7465 7374 2d65  : "ds-lib-test-e
+00001980: 7665 6e74 222c 0a20 2020 2020 2020 2020  vent",.         
+00001990: 2020 2020 2020 2020 2020 2022 656e 6454             "endT
+000019a0: 696d 6573 7461 6d70 223a 207b 2265 706f  imestamp": {"epo
+000019b0: 6368 5365 636f 6e64 223a 2031 3637 3239  chSecond": 16729
+000019c0: 3237 3032 352c 2022 6e61 6e6f 223a 2035  27025, "nano": 5
+000019d0: 3631 3735 3130 3030 7d2c 0a20 2020 2020  61751000},.     
+000019e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000019f0: 7374 6172 7454 696d 6573 7461 6d70 223a  startTimestamp":
+00001a00: 207b 2265 706f 6368 5365 636f 6e64 223a   {"epochSecond":
+00001a10: 2031 3637 3239 3237 3032 352c 2022 6e61   1672927025, "na
+00001a20: 6e6f 223a 2035 3630 3837 3330 3030 7d2c  no": 560873000},
+00001a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001a40: 2020 2020 2022 7061 7265 6e74 4576 656e       "parentEven
+00001a50: 7449 6422 3a20 4e6f 6e65 2c0a 2020 2020  tId": None,.    
+00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a70: 2273 7563 6365 7373 6675 6c22 3a20 5472  "successful": Tr
+00001a80: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00001a90: 2020 2020 2020 2020 2262 6f6f 6b49 6422          "bookId"
+00001aa0: 3a20 2264 656d 6f5f 626f 6f6b 5f31 222c  : "demo_book_1",
+00001ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001ac0: 2020 2020 2022 7363 6f70 6522 3a20 2274       "scope": "t
+00001ad0: 6832 2d73 636f 7065 222c 0a20 2020 2020  h2-scope",.     
+00001ae0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001af0: 6174 7461 6368 6564 4d65 7373 6167 6549  attachedMessageI
+00001b00: 6473 223a 205b 5d2c 0a20 2020 2020 2020  ds": [],.       
+00001b10: 2020 2020 2020 2020 2020 2020 2022 626f               "bo
+00001b20: 6479 223a 205b 5d2c 0a20 2020 2020 2020  dy": [],.       
+00001b30: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00001b40: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+00001b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b60: 2020 2265 7665 6e74 4964 223a 2022 6465    "eventId": "de
+00001b70: 6d6f 5f62 6f6f 6b5f 313a 7468 322d 7363  mo_book_1:th2-sc
+00001b80: 6f70 653a 3230 3233 3031 3035 3133 3537  ope:202301051357
+00001b90: 3035 3536 3335 3232 3030 303a 3961 6462  05563522000:9adb
+00001ba0: 6233 6530 2d35 6638 622d 3463 3238 2d61  b3e0-5f8b-4c28-a
+00001bb0: 3261 632d 3733 3631 6538 6661 3730 3463  2ac-7361e8fa704c
+00001bc0: 3e64 656d 6f5f 626f 6f6b 5f31 3a74 6832  >demo_book_1:th2
+00001bd0: 2d73 636f 7065 3a32 3032 3330 3130 3531  -scope:202301051
+00001be0: 3335 3730 3535 3633 3532 3230 3030 3a64  35705563522000:d
+00001bf0: 3631 6539 3330 612d 3864 3030 2d31 3165  61e930a-8d00-11e
+00001c00: 642d 6161 3161 2d64 3334 6136 3135 3531  d-aa1a-d34a61551
+00001c10: 3532 645f 3222 2c0a 2020 2020 2020 2020  52d_2",.        
+00001c20: 2020 2020 2020 2020 2020 2020 2262 6174              "bat
+00001c30: 6368 4964 223a 2022 6465 6d6f 5f62 6f6f  chId": "demo_boo
+00001c40: 6b5f 313a 7468 322d 7363 6f70 653a 3230  k_1:th2-scope:20
+00001c50: 3233 3031 3035 3133 3537 3035 3536 3335  2301051357055635
+00001c60: 3232 3030 303a 3961 6462 6233 6530 2d35  22000:9adbb3e0-5
+00001c70: 6638 622d 3463 3238 2d61 3261 632d 3733  f8b-4c28-a2ac-73
+00001c80: 3631 6538 6661 3730 3463 222c 0a20 2020  61e8fa704c",.   
+00001c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ca0: 2022 6973 4261 7463 6865 6422 3a20 5472   "isBatched": Tr
+00001cb0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00001cc0: 2020 2020 2020 2020 2265 7665 6e74 4e61          "eventNa
+00001cd0: 6d65 223a 2022 506c 6169 6e20 6576 656e  me": "Plain even
+00001ce0: 7420 3122 2c0a 2020 2020 2020 2020 2020  t 1",.          
+00001cf0: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
+00001d00: 5479 7065 223a 2022 6473 2d6c 6962 2d74  Type": "ds-lib-t
+00001d10: 6573 742d 6576 656e 7422 2c0a 2020 2020  est-event",.    
+00001d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d30: 2265 6e64 5469 6d65 7374 616d 7022 3a20  "endTimestamp": 
+00001d40: 7b22 6570 6f63 6853 6563 6f6e 6422 3a20  {"epochSecond": 
+00001d50: 3136 3732 3932 3730 3235 2c20 226e 616e  1672927025, "nan
+00001d60: 6f22 3a20 3536 3336 3430 3030 307d 2c0a  o": 563640000},.
+00001d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d80: 2020 2020 2273 7461 7274 5469 6d65 7374      "startTimest
+00001d90: 616d 7022 3a20 7b22 6570 6f63 6853 6563  amp": {"epochSec
+00001da0: 6f6e 6422 3a20 3136 3732 3932 3730 3235  ond": 1672927025
+00001db0: 2c20 226e 616e 6f22 3a20 3536 3335 3232  , "nano": 563522
+00001dc0: 3030 307d 2c0a 2020 2020 2020 2020 2020  000},.          
+00001dd0: 2020 2020 2020 2020 2020 2270 6172 656e            "paren
+00001de0: 7445 7665 6e74 4964 223a 2022 6465 6d6f  tEventId": "demo
+00001df0: 5f62 6f6f 6b5f 313a 7468 322d 7363 6f70  _book_1:th2-scop
+00001e00: 653a 3230 3233 3031 3035 3133 3537 3035  e:20230105135705
+00001e10: 3536 3038 3733 3030 303a 6436 3165 3933  560873000:d61e93
+00001e20: 3061 2d38 6430 302d 3131 6564 2d61 6131  0a-8d00-11ed-aa1
+00001e30: 612d 6433 3461 3631 3535 3135 3264 5f31  a-d34a6155152d_1
+00001e40: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001e50: 2020 2020 2020 2022 7375 6363 6573 7366         "successf
+00001e60: 756c 223a 2054 7275 652c 0a20 2020 2020  ul": True,.     
+00001e70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001e80: 626f 6f6b 4964 223a 2022 6465 6d6f 5f62  bookId": "demo_b
+00001e90: 6f6f 6b5f 3122 2c0a 2020 2020 2020 2020  ook_1",.        
+00001ea0: 2020 2020 2020 2020 2020 2020 2273 636f              "sco
+00001eb0: 7065 223a 2022 7468 322d 7363 6f70 6522  pe": "th2-scope"
+00001ec0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001ed0: 2020 2020 2020 2261 7474 6163 6865 644d        "attachedM
+00001ee0: 6573 7361 6765 4964 7322 3a20 5b5d 2c0a  essageIds": [],.
+00001ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f00: 2020 2020 2262 6f64 7922 3a20 7b22 7479      "body": {"ty
+00001f10: 7065 223a 2022 6d65 7373 6167 6522 2c20  pe": "message", 
+00001f20: 2264 6174 6122 3a20 2264 732d 6c69 6220  "data": "ds-lib 
+00001f30: 7465 7374 2062 6f64 7922 7d2c 0a20 2020  test body"},.   
+00001f40: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
+00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f60: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00001f70: 2020 2020 2020 2265 7665 6e74 4964 223a        "eventId":
+00001f80: 2022 6465 6d6f 5f62 6f6f 6b5f 313a 7468   "demo_book_1:th
+00001f90: 322d 7363 6f70 653a 3230 3233 3031 3035  2-scope:20230105
+00001fa0: 3133 3537 3035 3536 3335 3232 3030 303a  135705563522000:
+00001fb0: 3961 6462 6233 6530 2d35 6638 622d 3463  9adbb3e0-5f8b-4c
+00001fc0: 3238 2d61 3261 632d 3733 3631 6538 6661  28-a2ac-7361e8fa
+00001fd0: 3730 3463 3e64 656d 6f5f 626f 6f6b 5f31  704c>demo_book_1
+00001fe0: 3a74 6832 2d73 636f 7065 3a32 3032 3330  :th2-scope:20230
+00001ff0: 3130 3531 3335 3730 3535 3633 3735 3730  1051357055637570
+00002000: 3030 3a64 3631 6539 3330 612d 3864 3030  00:d61e930a-8d00
+00002010: 2d31 3165 642d 6161 3161 2d64 3334 6136  -11ed-aa1a-d34a6
+00002020: 3135 3531 3532 645f 3322 2c0a 2020 2020  155152d_3",.    
+00002030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002040: 2262 6174 6368 4964 223a 2022 6465 6d6f  "batchId": "demo
+00002050: 5f62 6f6f 6b5f 313a 7468 322d 7363 6f70  _book_1:th2-scop
+00002060: 653a 3230 3233 3031 3035 3133 3537 3035  e:20230105135705
+00002070: 3536 3335 3232 3030 303a 3961 6462 6233  563522000:9adbb3
+00002080: 6530 2d35 6638 622d 3463 3238 2d61 3261  e0-5f8b-4c28-a2a
+00002090: 632d 3733 3631 6538 6661 3730 3463 222c  c-7361e8fa704c",
+000020a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000020b0: 2020 2020 2022 6973 4261 7463 6865 6422       "isBatched"
+000020c0: 3a20 5472 7565 2c0a 2020 2020 2020 2020  : True,.        
+000020d0: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
+000020e0: 6e74 4e61 6d65 223a 2022 506c 6169 6e20  ntName": "Plain 
+000020f0: 6576 656e 7420 3222 2c0a 2020 2020 2020  event 2",.      
+00002100: 2020 2020 2020 2020 2020 2020 2020 2265                "e
+00002110: 7665 6e74 5479 7065 223a 2022 6473 2d6c  ventType": "ds-l
+00002120: 6962 2d74 6573 742d 6576 656e 7422 2c0a  ib-test-event",.
+00002130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002140: 2020 2020 2265 6e64 5469 6d65 7374 616d      "endTimestam
+00002150: 7022 3a20 7b22 6570 6f63 6853 6563 6f6e  p": {"epochSecon
+00002160: 6422 3a20 3136 3732 3932 3730 3235 2c20  d": 1672927025, 
+00002170: 226e 616e 6f22 3a20 3536 3337 3931 3030  "nano": 56379100
+00002180: 307d 2c0a 2020 2020 2020 2020 2020 2020  0},.            
+00002190: 2020 2020 2020 2020 2273 7461 7274 5469          "startTi
+000021a0: 6d65 7374 616d 7022 3a20 7b22 6570 6f63  mestamp": {"epoc
+000021b0: 6853 6563 6f6e 6422 3a20 3136 3732 3932  hSecond": 167292
+000021c0: 3730 3235 2c20 226e 616e 6f22 3a20 3536  7025, "nano": 56
+000021d0: 3337 3537 3030 307d 2c0a 2020 2020 2020  3757000},.      
+000021e0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+000021f0: 6172 656e 7445 7665 6e74 4964 223a 2022  arentEventId": "
+00002200: 6465 6d6f 5f62 6f6f 6b5f 313a 7468 322d  demo_book_1:th2-
+00002210: 7363 6f70 653a 3230 3233 3031 3035 3133  scope:2023010513
+00002220: 3537 3035 3536 3038 3733 3030 303a 6436  5705560873000:d6
+00002230: 3165 3933 3061 2d38 6430 302d 3131 6564  1e930a-8d00-11ed
+00002240: 2d61 6131 612d 6433 3461 3631 3535 3135  -aa1a-d34a615515
+00002250: 3264 5f31 222c 0a20 2020 2020 2020 2020  2d_1",.         
+00002260: 2020 2020 2020 2020 2020 2022 7375 6363             "succ
+00002270: 6573 7366 756c 223a 2054 7275 652c 0a20  essful": True,. 
+00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002290: 2020 2022 626f 6f6b 4964 223a 2022 6465     "bookId": "de
+000022a0: 6d6f 5f62 6f6f 6b5f 3122 2c0a 2020 2020  mo_book_1",.    
+000022b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022c0: 2273 636f 7065 223a 2022 7468 322d 7363  "scope": "th2-sc
+000022d0: 6f70 6522 2c0a 2020 2020 2020 2020 2020  ope",.          
+000022e0: 2020 2020 2020 2020 2020 2261 7474 6163            "attac
+000022f0: 6865 644d 6573 7361 6765 4964 7322 3a20  hedMessageIds": 
+00002300: 5b5d 2c0a 2020 2020 2020 2020 2020 2020  [],.            
+00002310: 2020 2020 2020 2020 2262 6f64 7922 3a20          "body": 
+00002320: 7b22 7479 7065 223a 2022 6d65 7373 6167  {"type": "messag
+00002330: 6522 2c20 2264 6174 6122 3a20 2264 732d  e", "data": "ds-
+00002340: 6c69 6220 7465 7374 2062 6f64 7922 7d2c  lib test body"},
+00002350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002360: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00002370: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00002380: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
+00002390: 4964 223a 2022 6661 6b65 2d65 7665 6e74  Id": "fake-event
+000023a0: 4964 222c 0a20 2020 2020 2020 2020 2020  Id",.           
+000023b0: 2020 2020 2020 2020 2022 6261 7463 6849           "batchI
+000023c0: 6422 3a20 2266 616b 652d 6261 7463 6849  d": "fake-batchI
+000023d0: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
+000023e0: 2020 2020 2020 2020 2269 7342 6174 6368          "isBatch
+000023f0: 6564 223a 2054 7275 652c 0a20 2020 2020  ed": True,.     
+00002400: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002410: 6576 656e 744e 616d 6522 3a20 2246 616b  eventName": "Fak
+00002420: 6520 6576 656e 7422 2c0a 2020 2020 2020  e event",.      
+00002430: 2020 2020 2020 2020 2020 2020 2020 2265                "e
+00002440: 7665 6e74 5479 7065 223a 2022 6473 2d6c  ventType": "ds-l
+00002450: 6962 2d74 6573 742d 6576 656e 7422 2c0a  ib-test-event",.
+00002460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002470: 2020 2020 2265 6e64 5469 6d65 7374 616d      "endTimestam
+00002480: 7022 3a20 7b22 6570 6f63 6853 6563 6f6e  p": {"epochSecon
+00002490: 6422 3a20 3136 3732 3932 3730 3335 2c20  d": 1672927035, 
+000024a0: 226e 616e 6f22 3a20 3536 3337 3931 3030  "nano": 56379100
+000024b0: 307d 2c0a 2020 2020 2020 2020 2020 2020  0},.            
+000024c0: 2020 2020 2020 2020 2273 7461 7274 5469          "startTi
+000024d0: 6d65 7374 616d 7022 3a20 7b22 6570 6f63  mestamp": {"epoc
+000024e0: 6853 6563 6f6e 6422 3a20 3136 3732 3932  hSecond": 167292
+000024f0: 3733 3235 2c20 226e 616e 6f22 3a20 3536  7325, "nano": 56
+00002500: 3337 3537 3030 307d 2c0a 2020 2020 2020  3757000},.      
+00002510: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+00002520: 6172 656e 7445 7665 6e74 4964 223a 2022  arentEventId": "
+00002530: 6e6f 745f 6578 6973 7473 5f69 6e5f 7468  not_exists_in_th
+00002540: 655f 6576 656e 7473 5f73 7472 6561 6d22  e_events_stream"
+00002550: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002560: 2020 2020 2020 2273 7563 6365 7373 6675        "successfu
+00002570: 6c22 3a20 4661 6c73 652c 0a20 2020 2020  l": False,.     
+00002580: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002590: 626f 6f6b 4964 223a 2022 6465 6d6f 5f62  bookId": "demo_b
+000025a0: 6f6f 6b5f 3122 2c0a 2020 2020 2020 2020  ook_1",.        
+000025b0: 2020 2020 2020 2020 2020 2020 2273 636f              "sco
+000025c0: 7065 223a 2022 7468 322d 7363 6f70 6522  pe": "th2-scope"
+000025d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000025e0: 2020 2020 2020 2261 7474 6163 6865 644d        "attachedM
+000025f0: 6573 7361 6765 4964 7322 3a20 5b5d 2c0a  essageIds": [],.
+00002600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002610: 2020 2020 2262 6f64 7922 3a20 7b22 7479      "body": {"ty
+00002620: 7065 223a 2022 6d65 7373 6167 6522 2c20  pe": "message", 
+00002630: 2264 6174 6122 3a20 2264 732d 6c69 6220  "data": "ds-lib 
+00002640: 7465 7374 2062 6f64 7922 7d2c 0a20 2020  test body"},.   
+00002650: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
+00002660: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
+00002670: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00002680: 0a20 2020 2020 2020 2023 2323 2323 2323  .        #######
+00002690: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000026a0: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
+000026b0: 2020 2020 2020 2020 2320 5b31 5d20 576f          # [1] Wo
+000026c0: 726b 696e 6720 7769 7468 2061 2044 6174  rking with a Dat
+000026d0: 6120 6f62 6a65 6374 2e0a 2020 2020 2020  a object..      
+000026e0: 2020 2323 2323 2323 2323 2323 2323 2323    ##############
+000026f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002700: 2323 2323 2323 2323 0a20 2020 2020 2020  ########.       
+00002710: 200a 2020 2020 2020 2020 2320 5b31 2e31   .        # [1.1
+00002720: 5d20 4669 6c74 6572 2e0a 2020 2020 2020  ] Filter..      
+00002730: 2020 6669 6c74 6572 6564 5f65 7665 6e74    filtered_event
+00002740: 733a 2044 6174 6120 3d20 6576 656e 7473  s: Data = events
+00002750: 2e66 696c 7465 7228 6c61 6d62 6461 2065  .filter(lambda e
+00002760: 3a20 655b 2262 6f64 7922 5d20 213d 205b  : e["body"] != [
+00002770: 5d29 2020 2320 4669 6c74 6572 2065 7665  ])  # Filter eve
+00002780: 6e74 7320 7769 7468 2065 6d70 7479 2062  nts with empty b
+00002790: 6f64 792e 0a20 2020 2020 2020 200a 2020  ody..        .  
+000027a0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+000027b0: 205b 312e 325d 204d 6170 2e0a 2020 2020   [1.2] Map..    
+000027c0: 2020 2020 6465 6620 7472 616e 7366 6f72      def transfor
+000027d0: 6d5f 6675 6e63 7469 6f6e 2872 6563 6f72  m_function(recor
+000027e0: 6429 3a0a 2020 2020 2020 2020 2020 2020  d):.            
+000027f0: 7265 7475 726e 207b 2265 7665 6e74 4e61  return {"eventNa
+00002800: 6d65 223a 2072 6563 6f72 645b 2265 7665  me": record["eve
+00002810: 6e74 4e61 6d65 225d 2c20 2273 7563 6365  ntName"], "succe
+00002820: 7373 6675 6c22 3a20 7265 636f 7264 5b22  ssful": record["
+00002830: 7375 6363 6573 7366 756c 225d 7d0a 2020  successful"]}.  
+00002840: 2020 2020 2020 0a20 2020 2020 2020 200a        .        .
+00002850: 2020 2020 2020 2020 6669 6c74 6572 6564          filtered
+00002860: 5f61 6e64 5f6d 6170 7065 645f 6576 656e  _and_mapped_even
+00002870: 7473 203d 2066 696c 7465 7265 645f 6576  ts = filtered_ev
+00002880: 656e 7473 2e6d 6170 2874 7261 6e73 666f  ents.map(transfo
+00002890: 726d 5f66 756e 6374 696f 6e29 0a20 2020  rm_function).   
+000028a0: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+000028b0: 5b31 2e33 5d20 4461 7461 2070 6970 656c  [1.3] Data pipel
+000028c0: 696e 652e 0a20 2020 2020 2020 2023 2020  ine..        #  
+000028d0: 2020 2020 2049 6e73 7465 6164 206f 6620       Instead of 
+000028e0: 646f 696e 6720 6461 7461 2074 7261 6e73  doing data trans
+000028f0: 666f 726d 6174 696f 6e73 2073 7465 7020  formations step 
+00002900: 6279 2073 7465 7020 796f 7520 6361 6e20  by step you can 
+00002910: 646f 2069 7420 696e 206f 6e65 206c 696e  do it in one lin
+00002920: 652e 0a20 2020 2020 2020 2066 696c 7465  e..        filte
+00002930: 7265 645f 616e 645f 6d61 7070 6564 5f65  red_and_mapped_e
+00002940: 7665 6e74 735f 6279 5f70 6970 656c 696e  vents_by_pipelin
+00002950: 6520 3d20 6576 656e 7473 2e66 696c 7465  e = events.filte
+00002960: 7228 6c61 6d62 6461 2065 3a20 655b 2262  r(lambda e: e["b
+00002970: 6f64 7922 5d20 213d 205b 5d29 2e6d 6170  ody"] != []).map
+00002980: 280a 2020 2020 2020 2020 2020 2020 7472  (.            tr
+00002990: 616e 7366 6f72 6d5f 6675 6e63 7469 6f6e  ansform_function
+000029a0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+000029b0: 2020 2023 2043 6f6e 7465 6e74 206f 6620     # Content of 
+000029c0: 7468 6573 6520 7477 6f20 4461 7461 206f  these two Data o
+000029d0: 626a 6563 7473 2073 686f 756c 6420 6265  bjects should be
+000029e0: 2065 7175 616c 2e0a 2020 2020 2020 2020   equal..        
+000029f0: 6173 7365 7274 206c 6973 7428 6669 6c74  assert list(filt
+00002a00: 6572 6564 5f61 6e64 5f6d 6170 7065 645f  ered_and_mapped_
+00002a10: 6576 656e 7473 2920 3d3d 206c 6973 7428  events) == list(
+00002a20: 6669 6c74 6572 6564 5f61 6e64 5f6d 6170  filtered_and_map
+00002a30: 7065 645f 6576 656e 7473 5f62 795f 7069  ped_events_by_pi
+00002a40: 7065 6c69 6e65 290a 2020 2020 2020 2020  peline).        
+00002a50: 0a20 2020 2020 2020 2023 205b 312e 345d  .        # [1.4]
+00002a60: 2053 6966 742e 2053 6b69 7020 7468 6520   Sift. Skip the 
+00002a70: 6669 7273 7420 6665 7720 6974 656d 7320  first few items 
+00002a80: 6f72 206c 696d 6974 2074 6865 6d2e 0a20  or limit them.. 
+00002a90: 2020 2020 2020 2064 6174 6120 3d20 4461         data = Da
+00002aa0: 7461 285b 312c 2032 2c20 332c 2034 2c20  ta([1, 2, 3, 4, 
+00002ab0: 352c 2036 2c20 372c 2038 2c20 392c 2031  5, 6, 7, 8, 9, 1
+00002ac0: 302c 2031 312c 2031 322c 2031 332c 2031  0, 11, 12, 13, 1
+00002ad0: 342c 2031 355d 290a 2020 2020 2020 2020  4, 15]).        
+00002ae0: 6974 656d 735f 6672 6f6d 5f31 315f 746f  items_from_11_to
+00002af0: 5f65 6e64 3a20 4765 6e65 7261 746f 7220  _end: Generator 
+00002b00: 3d20 6461 7461 2e73 6966 7428 736b 6970  = data.sift(skip
+00002b10: 3d31 3029 0a20 2020 2020 2020 206f 6e6c  =10).        onl
+00002b20: 795f 6669 7273 745f 3130 5f69 7465 6d73  y_first_10_items
+00002b30: 3a20 4765 6e65 7261 746f 7220 3d20 6461  : Generator = da
+00002b40: 7461 2e73 6966 7428 6c69 6d69 743d 3130  ta.sift(limit=10
+00002b50: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+00002b60: 2020 2023 205b 312e 355d 2043 6861 6e67     # [1.5] Chang
+00002b70: 696e 6720 6361 6368 6520 7374 6174 7573  ing cache status
+00002b80: 2e0a 2020 2020 2020 2020 6576 656e 7473  ..        events
+00002b90: 2e75 7365 5f63 6163 6865 2854 7275 6529  .use_cache(True)
+00002ba0: 0a20 2020 2020 2020 2023 206f 7220 6a75  .        # or ju
+00002bb0: 7374 0a20 2020 2020 2020 2065 7665 6e74  st.        event
+00002bc0: 732e 7573 655f 6361 6368 6528 2920 2023  s.use_cache()  #
+00002bd0: 2049 6620 796f 7520 7761 6e74 2074 6f20   If you want to 
+00002be0: 6163 7469 7661 7465 2063 6163 6865 2e0a  activate cache..
+00002bf0: 2020 2020 2020 2020 2320 5b31 2e36 5d20          # [1.6] 
+00002c00: 5761 6c6b 2074 6872 6f75 6768 2064 6174  Walk through dat
+00002c10: 612e 0a20 2020 2020 2020 2066 6f72 2065  a..        for e
+00002c20: 7665 6e74 2069 6e20 6576 656e 7473 3a0a  vent in events:.
+00002c30: 2020 2020 2020 2020 2020 2020 2320 446f              # Do
+00002c40: 2073 6f6d 6574 6869 6e67 2077 6974 6820   something with 
+00002c50: 6576 656e 7420 2865 7665 6e74 2069 7320  event (event is 
+00002c60: 6120 6469 6374 292e 0a20 2020 2020 2020  a dict)..       
+00002c70: 2020 2020 2070 7269 6e74 2865 7665 6e74       print(event
+00002c80: 290a 2020 2020 2020 2020 2320 4166 7465  ).        # Afte
+00002c90: 7220 6669 7273 7420 6974 6572 6174 696f  r first iteratio
+00002ca0: 6e20 7468 6520 6576 656e 7473 2068 6173  n the events has
+00002cb0: 2061 2063 6163 6865 2066 696c 652e 0a20   a cache file.. 
+00002cc0: 2020 2020 2020 2023 204e 6f77 2074 6865         # Now the
+00002cd0: 7920 7769 6c6c 2062 6520 7573 6564 2069  y will be used i
+00002ce0: 6e20 7468 6520 6361 6368 6520 696e 2074  n the cache in t
+00002cf0: 6865 206e 6578 7420 6974 6572 6174 696f  he next iteratio
+00002d00: 6e2e 0a20 2020 2020 2020 200a 2020 2020  n..        .    
+00002d10: 2020 2020 2320 5b31 2e37 5d20 4765 7420      # [1.7] Get 
+00002d20: 6e75 6d62 6572 206f 6620 7468 6520 656c  number of the el
+00002d30: 656d 656e 7473 2069 6e20 7468 6520 4461  ements in the Da
+00002d40: 7461 206f 626a 6563 742e 0a20 2020 2020  ta object..     
+00002d50: 2020 206e 756d 6265 725f 6f66 5f65 7665     number_of_eve
+00002d60: 6e74 7320 3d20 6576 656e 7473 2e6c 656e  nts = events.len
+00002d70: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00002d80: 2020 2320 5b31 2e38 5d20 4368 6563 6b20    # [1.8] Check 
+00002d90: 7468 6174 2044 6174 6120 6f62 6a65 6374  that Data object
+00002da0: 2069 736e 2774 2065 6d70 7479 2e0a 2020   isn't empty..  
+00002db0: 2020 2020 2020 2320 5468 6520 6461 7461        # The data
+00002dc0: 2073 6f75 7263 6520 7368 6f75 6c64 2062   source should b
+00002dd0: 6520 6e6f 7420 656d 7074 792e 0a20 2020  e not empty..   
+00002de0: 2020 2020 2061 7373 6572 7420 6576 656e       assert even
+00002df0: 7473 2e69 735f 656d 7074 7920 6973 2046  ts.is_empty is F
+00002e00: 616c 7365 0a20 2020 2020 2020 200a 2020  alse.        .  
+00002e10: 2020 2020 2020 2320 5b31 2e39 5d20 436f        # [1.9] Co
+00002e20: 6e76 6572 7420 4461 7461 206f 626a 6563  nvert Data objec
+00002e30: 7420 746f 2074 6865 206c 6973 7420 6f66  t to the list of
+00002e40: 2065 6c65 6d65 6e74 7328 6576 656e 7473   elements(events
+00002e50: 206f 7220 6d65 7373 6167 6573 292e 0a20   or messages).. 
+00002e60: 2020 2020 2020 2023 2042 6520 6361 7265         # Be care
+00002e70: 6675 6c2c 2074 6869 7320 6361 6e20 7461  ful, this can ta
+00002e80: 6b65 2074 6f6f 206d 7563 6820 6d65 6d6f  ke too much memo
+00002e90: 7279 2e0a 2020 2020 2020 2020 6576 656e  ry..        even
+00002ea0: 7473 5f6c 6973 7420 3d20 6c69 7374 2865  ts_list = list(e
+00002eb0: 7665 6e74 7329 0a20 2020 2020 2020 200a  vents).        .
+00002ec0: 2020 2020 2020 2020 2320 5b31 2e31 305d          # [1.10]
+00002ed0: 2054 6865 2063 6163 6865 2069 6e68 6572   The cache inher
+00002ee0: 6974 616e 6365 2e0a 2020 2020 2020 2020  itance..        
+00002ef0: 2320 4372 6561 7465 7320 6120 6e65 7720  # Creates a new 
+00002f00: 4461 7461 206f 626a 6563 7420 7468 6174  Data object that
+00002f10: 2077 696c 6c20 7573 6520 6361 6368 6520   will use cache 
+00002f20: 6672 6f6d 2074 6865 2065 7665 6e74 7320  from the events 
+00002f30: 4461 7461 206f 626a 6563 742e 0a20 2020  Data object..   
+00002f40: 2020 2020 2065 7665 6e74 735f 6669 6c74       events_filt
+00002f50: 6572 6564 3a20 4461 7461 203d 2065 7665  ered: Data = eve
+00002f60: 6e74 732e 6669 6c74 6572 286c 616d 6264  nts.filter(lambd
+00002f70: 6120 7265 636f 7264 3a20 7265 636f 7264  a record: record
+00002f80: 2e67 6574 2822 6261 7463 6849 6422 2929  .get("batchId"))
+00002f90: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00002fa0: 2020 2320 4e65 7720 4461 7461 206f 626a    # New Data obj
+00002fb0: 6563 7473 2064 6f6e 2774 2075 7365 2074  ects don't use t
+00002fc0: 6865 6972 206f 776e 2063 6163 6865 2062  heir own cache b
+00002fd0: 7920 6465 6661 756c 7420 6275 7420 7573  y default but us
+00002fe0: 6520 7468 6520 6361 6368 6520 6f66 2074  e the cache of t
+00002ff0: 6865 2070 6172 656e 7420 4461 7461 206f  he parent Data o
+00003000: 626a 6563 742e 0a20 2020 2020 2020 2023  bject..        #
+00003010: 2055 7365 2075 7365 5f63 6163 6865 206d   Use use_cache m
+00003020: 6574 686f 6420 746f 2061 6374 6976 6174  ethod to activat
+00003030: 6520 6361 6368 696e 672e 0a20 2020 2020  e caching..     
+00003040: 2020 2023 2041 6674 6572 2074 6861 742c     # After that,
+00003050: 2074 6865 2044 6174 6120 6f62 6a65 6374   the Data object
+00003060: 2077 696c 6c20 6372 6561 7465 2069 7473   will create its
+00003070: 206f 776e 2063 6163 6865 2066 696c 652e   own cache file.
+00003080: 0a20 2020 2020 2020 2065 7665 6e74 735f  .        events_
+00003090: 6669 6c74 6572 6564 2e75 7365 5f63 6163  filtered.use_cac
+000030a0: 6865 2829 0a20 2020 2020 2020 200a 2020  he().        .  
+000030b0: 2020 2020 2020 6c69 7374 2865 7665 6e74        list(event
+000030c0: 735f 6669 6c74 6572 6564 2920 2023 204a  s_filtered)  # J
+000030d0: 7573 7420 746f 2069 7465 7261 7465 2044  ust to iterate D
+000030e0: 6174 6120 6f62 6a65 6374 2028 6361 6368  ata object (cach
+000030f0: 6520 6669 6c65 2077 696c 6c20 6265 2063  e file will be c
+00003100: 7265 6174 6564 292e 0a20 2020 2020 2020  reated)..       
+00003110: 200a 2020 2020 2020 2020 6669 6c74 6572   .        filter
+00003120: 6564 5f65 7665 6e74 735f 7479 7065 7320  ed_events_types 
+00003130: 3d20 6576 656e 7473 5f66 696c 7465 7265  = events_filtere
+00003140: 642e 6d61 7028 6c61 6d62 6461 2072 6563  d.map(lambda rec
+00003150: 6f72 643a 207b 2265 7665 6e74 5479 7065  ord: {"eventType
+00003160: 223a 2072 6563 6f72 642e 6765 7428 2265  ": record.get("e
+00003170: 7665 6e74 5479 7065 2229 7d29 0a20 2020  ventType")}).   
+00003180: 2020 2020 200a 2020 2020 2020 2020 6576       .        ev
+00003190: 656e 7473 5f77 6974 686f 7574 5f74 7970  ents_without_typ
+000031a0: 6573 5f77 6974 685f 6261 7463 6820 3d20  es_with_batch = 
+000031b0: 6669 6c74 6572 6564 5f65 7665 6e74 735f  filtered_events_
+000031c0: 7479 7065 732e 6669 6c74 6572 280a 2020  types.filter(.  
+000031d0: 2020 2020 2020 2020 2020 6c61 6d62 6461            lambda
+000031e0: 2072 6563 6f72 643a 206e 6f74 2072 6563   record: not rec
+000031f0: 6f72 642e 6765 7428 2265 7665 6e74 5479  ord.get("eventTy
+00003200: 7065 2229 0a20 2020 2020 2020 2029 0a20  pe").        ). 
+00003210: 2020 2020 2020 2065 7665 6e74 735f 7769         events_wi
+00003220: 7468 6f75 745f 7479 7065 735f 7769 7468  thout_types_with
+00003230: 5f62 6174 6368 2e75 7365 5f63 6163 6865  _batch.use_cache
+00003240: 2829 0a20 2020 2020 2020 200a 2020 2020  ().        .    
+00003250: 2020 2020 2320 5b31 2e31 315d 2044 6174      # [1.11] Dat
+00003260: 6120 6f62 6a65 6374 7320 6a6f 696e 696e  a objects joinin
+00003270: 672e 0a20 2020 2020 2020 2023 2059 6f75  g..        # You
+00003280: 2068 6176 6520 7468 6520 666f 6c6c 6f77   have the follow
+00003290: 696e 6720 3320 4461 7461 206f 626a 6563  ing 3 Data objec
+000032a0: 7473 2e0a 2020 2020 2020 2020 6431 203d  ts..        d1 =
+000032b0: 2044 6174 6128 5b31 2c20 322c 2033 5d29   Data([1, 2, 3])
+000032c0: 0a20 2020 2020 2020 2064 3220 3d20 4461  .        d2 = Da
+000032d0: 7461 285b 2261 222c 207b 2269 6422 3a20  ta(["a", {"id": 
+000032e0: 3132 337d 2c20 2263 225d 290a 2020 2020  123}, "c"]).    
+000032f0: 2020 2020 6433 203d 2044 6174 6128 5b37      d3 = Data([7
+00003300: 2c20 382c 2039 5d29 0a20 2020 2020 2020  , 8, 9]).       
+00003310: 2023 2059 6f75 2063 616e 206a 6f69 6e20   # You can join 
+00003320: 4461 7461 206f 626a 6563 7473 2069 6e20  Data objects in 
+00003330: 666f 6c6c 6f77 696e 6720 7761 7973 2e0a  following ways..
+00003340: 2020 2020 2020 2020 2320 506c 6561 7365          # Please
+00003350: 206e 6f74 652c 206e 6577 2044 6174 6120   note, new Data 
+00003360: 6f62 6a65 6374 2077 696c 6c20 6861 7665  object will have
+00003370: 2063 6163 6865 2073 7461 7475 7320 3d3d   cache status ==
+00003380: 2046 616c 7365 2e0a 2020 2020 2020 2020   False..        
+00003390: 6461 7461 5f76 6961 5f69 6e69 7420 3d20  data_via_init = 
+000033a0: 4461 7461 285b 6431 2c20 6432 2c20 6433  Data([d1, d2, d3
+000033b0: 5d29 0a20 2020 2020 2020 2064 6174 615f  ]).        data_
+000033c0: 7669 615f 6164 6420 3d20 6431 202b 2064  via_add = d1 + d
+000033d0: 3220 2b20 6433 0a20 2020 2020 2020 2064  2 + d3.        d
+000033e0: 6174 615f 7769 7468 5f6e 6f6e 5f64 6174  ata_with_non_dat
+000033f0: 615f 6f62 6a5f 7669 615f 696e 6974 203d  a_obj_via_init =
+00003400: 2044 6174 6128 5b64 312c 205b 2261 222c   Data([d1, ["a",
+00003410: 207b 2269 6422 3a20 3132 337d 2c20 2263   {"id": 123}, "c
+00003420: 225d 2c20 6433 5d29 0a20 2020 2020 2020  "], d3]).       
+00003430: 2064 6174 615f 7769 7468 5f6e 6f6e 5f64   data_with_non_d
+00003440: 6174 615f 6f62 6a5f 7669 615f 6164 6420  ata_obj_via_add 
+00003450: 3d20 6431 202b 205b 2261 222c 207b 2269  = d1 + ["a", {"i
+00003460: 6422 3a20 3132 337d 2c20 2263 225d 202b  d": 123}, "c"] +
+00003470: 2064 330a 2020 2020 2020 2020 2320 596f   d3.        # Yo
+00003480: 7520 6361 6e20 6a6f 696e 2063 7572 7265  u can join curre
+00003490: 6e74 2044 6174 6120 6f62 6a65 6374 206f  nt Data object o
+000034a0: 6e20 706c 6163 6520 7573 696e 6720 2b3d  n place using +=
+000034b0: 2e0a 2020 2020 2020 2020 2320 4974 2077  ..        # It w
+000034c0: 696c 6c20 6b65 6570 2063 6163 6865 2073  ill keep cache s
+000034d0: 7461 7475 732e 0a20 2020 2020 2020 2064  tatus..        d
+000034e0: 3120 2b3d 2064 3320 2023 2064 3120 7769  1 += d3  # d1 wi
+000034f0: 6c6c 2062 6563 6f6d 6520 4461 7461 285b  ll become Data([
+00003500: 312c 322c 332c 372c 382c 395d 290a 2020  1,2,3,7,8,9]).  
+00003510: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00003520: 205b 312e 3132 5d20 4275 696c 6420 616e   [1.12] Build an
+00003530: 6420 7265 6164 2044 6174 6120 6f62 6a65  d read Data obje
+00003540: 6374 2063 6163 6865 2066 696c 6573 2e0a  ct cache files..
+00003550: 2020 2020 2020 2020 6576 656e 7473 2e62          events.b
+00003560: 7569 6c64 5f63 6163 6865 2822 6361 6368  uild_cache("cach
+00003570: 655f 6669 6c65 6e61 6d65 5f6f 725f 7061  e_filename_or_pa
+00003580: 7468 2229 0a20 2020 2020 2020 2064 6174  th").        dat
+00003590: 615f 6f62 6a5f 6672 6f6d 5f63 6163 6865  a_obj_from_cache
+000035a0: 203d 2044 6174 612e 6672 6f6d 5f63 6163   = Data.from_cac
+000035b0: 6865 5f66 696c 6528 2263 6163 6865 5f66  he_file("cache_f
+000035c0: 696c 656e 616d 655f 6f72 5f70 6174 6822  ilename_or_path"
+000035d0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+000035e0: 2020 2023 205b 312e 3133 5d20 4368 6563     # [1.13] Chec
+000035f0: 6b20 6966 2044 6174 6120 6973 2073 6f72  k if Data is sor
+00003600: 7465 642e 0a20 2020 2020 2020 2023 2054  ted..        # T
+00003610: 6861 7420 7769 6c6c 2072 6574 7572 6e20  hat will return 
+00003620: 616e 206f 626a 6563 7420 6069 735f 736f  an object `is_so
+00003630: 7274 6564 6020 7468 6174 2063 6f6e 7461  rted` that conta
+00003640: 696e 7320 696e 666f 726d 6174 696f 6e0a  ins information.
+00003650: 2020 2020 2020 2020 2320 2020 312e 2073          #   1. s
+00003660: 7461 7475 7320 2d2d 2073 6f72 7465 6420  tatus -- sorted 
+00003670: 6f72 206e 6f74 0a20 2020 2020 2020 2023  or not.        #
+00003680: 2020 2032 2e20 6669 7273 745f 756e 736f     2. first_unso
+00003690: 7274 6564 202d 2d20 7468 6520 696e 6465  rted -- the inde
+000036a0: 7820 6f66 2074 6865 2066 6972 7374 2075  x of the first u
+000036b0: 6e73 6f72 7465 6420 656c 656d 656e 740a  nsorted element.
+000036c0: 2020 2020 2020 2020 6973 5f73 6f72 7465          is_sorte
+000036d0: 6420 3d20 6576 656e 7473 2e69 735f 736f  d = events.is_so
+000036e0: 7274 6564 286c 616d 6264 6120 653a 2065  rted(lambda e: e
+000036f0: 5b22 7374 6172 7454 696d 6573 7461 6d70  ["startTimestamp
+00003700: 225d 5b22 6570 6f63 6853 6563 6f6e 6422  "]["epochSecond"
+00003710: 5d29 0a20 2020 2020 2020 200a 2020 2020  ]).        .    
+00003720: 2020 2020 2320 596f 7520 6361 6e20 7573      # You can us
+00003730: 6520 7468 6973 206f 626a 6563 7420 6173  e this object as
+00003740: 2075 7375 616c 2062 6f6f 6c20 7661 7269   usual bool vari
+00003750: 6162 6c65 2e0a 2020 2020 2020 2020 6966  able..        if
+00003760: 2069 735f 736f 7274 6564 3a0a 2020 2020   is_sorted:.    
+00003770: 2020 2020 2020 2020 7072 696e 7428 2265          print("e
+00003780: 7665 6e74 7320 4461 7461 206f 626a 2069  vents Data obj i
+00003790: 7320 736f 7274 6564 2122 290a 2020 2020  s sorted!").    
+000037a0: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
+000037b0: 312e 3134 5d20 5573 6520 6044 6174 612e  1.14] Use `Data.
+000037c0: 7368 6f77 2829 6020 746f 206c 6f6f 6b20  show()` to look 
+000037d0: 6174 2074 6865 2066 6972 7374 204e 206d  at the first N m
+000037e0: 6573 7361 6765 7320 696e 2074 6865 2073  essages in the s
+000037f0: 7472 6561 6d2e 0a20 2020 2020 2020 2064  tream..        d
+00003800: 6174 615f 7769 7468 5f6e 6f6e 5f64 6174  ata_with_non_dat
+00003810: 615f 6f62 6a5f 7669 615f 6164 642e 7368  a_obj_via_add.sh
+00003820: 6f77 286e 3d36 290a 2020 2020 2020 2020  ow(n=6).        
+00003830: 2320 5769 6c6c 2070 7269 6e74 0a20 2020  # Will print.   
+00003840: 2020 2020 2023 202d 2d2d 2d2d 2d2d 2d2d       # ---------
+00003850: 2d2d 2d2d 2050 7269 6e74 6564 2066 6972  ---- Printed fir
+00003860: 7374 2036 2072 6563 6f72 6473 202d 2d2d  st 6 records ---
+00003870: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00003880: 2020 2023 205b 315d 202d 2d2d 2d2d 2d0a     # [1] ------.
+00003890: 2020 2020 2020 2020 2320 310a 2020 2020          # 1.    
+000038a0: 2020 2020 2320 5b32 5d20 2d2d 2d2d 2d2d      # [2] ------
+000038b0: 0a20 2020 2020 2020 2023 2032 0a20 2020  .        # 2.   
+000038c0: 2020 2020 2023 205b 335d 202d 2d2d 2d2d       # [3] -----
+000038d0: 2d0a 2020 2020 2020 2020 2320 330a 2020  -.        # 3.  
+000038e0: 2020 2020 2020 2320 5b34 5d20 2d2d 2d2d        # [4] ----
+000038f0: 2d2d 0a20 2020 2020 2020 2023 2027 6127  --.        # 'a'
+00003900: 0a20 2020 2020 2020 2023 205b 355d 202d  .        # [5] -
+00003910: 2d2d 2d2d 2d0a 2020 2020 2020 2020 2320  -----.        # 
+00003920: 7b27 6964 273a 2031 3233 7d0a 2020 2020  {'id': 123}.    
+00003930: 2020 2020 2320 5b36 5d20 2d2d 2d2d 2d2d      # [6] ------
+00003940: 0a20 2020 2020 2020 2023 2027 6327 0a20  .        # 'c'. 
+00003950: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00003960: 2320 5b31 2e31 355d 2059 6f75 2063 616e  # [1.15] You can
+00003970: 2072 656d 6f76 6520 7468 6520 6361 6368   remove the cach
+00003980: 6520 6669 6c65 206f 6620 7468 6520 4461  e file of the Da
+00003990: 7461 206f 626a 6563 742c 2069 6620 7265  ta object, if re
+000039a0: 7175 6972 6564 2e0a 2020 2020 2020 2020  quired..        
+000039b0: 6461 7461 5f6f 626a 5f66 726f 6d5f 6361  data_obj_from_ca
+000039c0: 6368 652e 636c 6561 725f 6361 6368 6528  che.clear_cache(
+000039d0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+000039e0: 2020 2023 2323 2323 2323 2323 2323 2323     #############
+000039f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00003a00: 2323 2323 2323 2323 230a 2020 2020 2020  #########.      
+00003a10: 2020 2320 5b32 5d20 576f 726b 696e 6720    # [2] Working 
+00003a20: 7769 7468 2063 6f6e 7665 7274 6572 732e  with converters.
+00003a30: 0a20 2020 2020 2020 2023 2323 2323 2323  .        #######
+00003a40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00003a50: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
+00003a60: 2020 2020 2020 2020 2320 5468 6572 6520          # There 
+00003a70: 6172 6520 6375 7272 656e 746c 7920 7468  are currently th
+00003a80: 7265 6520 696d 706c 656d 656e 7461 7469  ree implementati
+00003a90: 6f6e 7320 6f66 2049 5469 6d65 7374 616d  ons of ITimestam
+00003aa0: 7043 6f6e 7665 7274 6572 2063 6c61 7373  pConverter class
+00003ab0: 3a20 4461 7465 7469 6d65 436f 6e76 6572  : DatetimeConver
+00003ac0: 7465 2c20 4461 7465 7469 6d65 5374 7269  te, DatetimeStri
+00003ad0: 6e67 436f 6e76 6572 7465 7220 616e 6420  ngConverter and 
+00003ae0: 5072 6f74 6f62 7566 5469 6d65 7374 616d  ProtobufTimestam
+00003af0: 7043 6f6e 7665 7274 6572 2e0a 2020 2020  pConverter..    
+00003b00: 2020 2020 2320 5468 6579 2061 6c6c 2069      # They all i
+00003b10: 6d70 6c65 6d65 6e74 2073 616d 6520 6d65  mplement same me
+00003b20: 7468 6f64 7320 6672 6f6d 2062 6173 6520  thods from base 
+00003b30: 636c 6173 732e 0a20 2020 2020 2020 2023  class..        #
+00003b40: 204e 6f74 6520 7468 6174 2073 6f6d 6520   Note that some 
+00003b50: 6163 6375 7261 6379 206d 6179 2062 6520  accuracy may be 
+00003b60: 6c6f 7374 2064 7572 696e 6720 636f 6e76  lost during conv
+00003b70: 6572 7369 6f6e 2e0a 2020 2020 2020 2020  ersion..        
+00003b80: 2320 4966 2066 6f72 2065 7861 6d70 6c65  # If for example
+00003b90: 2079 6f75 2075 7365 2074 6f5f 6d69 6372   you use to_micr
+00003ba0: 6f73 6563 6f6e 6473 206e 616e 6f73 6563  oseconds nanosec
+00003bb0: 6f6e 6473 2077 696c 6c20 6265 2063 7574  onds will be cut
+00003bc0: 206f 6666 2069 6e73 7465 6164 206f 6620   off instead of 
+00003bd0: 726f 756e 6469 6e67 2e0a 2020 2020 2020  rounding..      
+00003be0: 2020 0a20 2020 2020 2020 2023 205b 322e    .        # [2.
+00003bf0: 315d 2044 6174 6574 696d 6543 6f6e 7665  1] DatetimeConve
+00003c00: 7274 6572 2e0a 2020 2020 2020 2020 2320  rter..        # 
+00003c10: 4461 7465 7469 6d65 436f 6e76 6572 7465  DatetimeConverte
+00003c20: 7220 7461 6b65 7320 6461 7465 7469 6d65  r takes datetime
+00003c30: 2e64 6174 6574 696d 6520 6f62 6a65 6374  .datetime object
+00003c40: 2061 7320 696e 7075 742e 0a20 2020 2020   as input..     
+00003c50: 2020 200a 2020 2020 2020 2020 6461 7465     .        date
+00003c60: 7469 6d65 5f6f 626a 203d 2064 6174 6574  time_obj = datet
+00003c70: 696d 6528 7965 6172 3d32 3032 332c 206d  ime(year=2023, m
+00003c80: 6f6e 7468 3d31 2c20 6461 793d 352c 2068  onth=1, day=5, h
+00003c90: 6f75 723d 3134 2c20 6d69 6e75 7465 3d33  our=14, minute=3
+00003ca0: 382c 2073 6563 6f6e 643d 3235 2c20 6d69  8, second=25, mi
+00003cb0: 6372 6f73 6563 6f6e 643d 3134 3630 290a  crosecond=1460).
+00003cc0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00003cd0: 2023 2049 7420 6861 7320 6d65 7468 6f64   # It has method
+00003ce0: 7320 7468 6174 2072 6574 7572 6e20 7468  s that return th
+00003cf0: 6520 6461 7465 7469 6d65 2069 6e20 6469  e datetime in di
+00003d00: 6666 6572 656e 7420 666f 726d 6173 3a0a  fferent formas:.
+00003d10: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00003d20: 2064 6174 655f 6d73 203d 2044 6174 6574   date_ms = Datet
+00003d30: 696d 6543 6f6e 7665 7274 6572 2e74 6f5f  imeConverter.to_
+00003d40: 6d69 6c6c 6973 6563 6f6e 6473 2864 6174  milliseconds(dat
+00003d50: 6574 696d 655f 6f62 6a29 0a20 2020 2020  etime_obj).     
+00003d60: 2020 2064 6174 655f 7573 203d 2044 6174     date_us = Dat
+00003d70: 6574 696d 6543 6f6e 7665 7274 6572 2e74  etimeConverter.t
+00003d80: 6f5f 6d69 6372 6f73 6563 6f6e 6473 2864  o_microseconds(d
+00003d90: 6174 6574 696d 655f 6f62 6a29 0a20 2020  atetime_obj).   
+00003da0: 2020 2020 2023 2043 6f6e 7665 7274 696e       # Convertin
+00003db0: 6720 746f 206e 616e 6f73 6563 6f6e 6473  g to nanoseconds
+00003dc0: 206a 7573 7473 2061 6464 7320 7468 7265   justs adds thre
+00003dd0: 6520 7472 6169 6c69 6e67 207a 6572 6f73  e trailing zeros
+00003de0: 2061 7320 6461 7465 7469 6d65 206f 626a   as datetime obj
+00003df0: 6563 7420 646f 6573 6e27 7420 6861 7665  ect doesn't have
+00003e00: 206e 616e 6f73 6563 6f6e 6473 2e0a 2020   nanoseconds..  
+00003e10: 2020 2020 2020 6461 7465 5f6e 7320 3d20        date_ns = 
+00003e20: 4461 7465 7469 6d65 436f 6e76 6572 7465  DatetimeConverte
+00003e30: 722e 746f 5f6e 616e 6f73 6563 6f6e 6473  r.to_nanoseconds
+00003e40: 2864 6174 6574 696d 655f 6f62 6a29 0a20  (datetime_obj). 
+00003e50: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00003e60: 2320 5b32 2e32 5d20 4461 7465 7469 6d65  # [2.2] Datetime
+00003e70: 5374 7269 6e67 436f 6e76 6572 7465 720a  StringConverter.
+00003e80: 2020 2020 2020 2020 2320 4461 7465 7469          # Dateti
+00003e90: 6d65 5374 7269 6e67 436f 6e76 6572 7465  meStringConverte
+00003ea0: 7220 7461 6b65 7320 7374 7269 6e67 2069  r takes string i
+00003eb0: 6e20 2279 7979 792d 4d4d 2d64 6454 4848  n "yyyy-MM-ddTHH
+00003ec0: 3a6d 6d3a 7373 5b2e 5353 5353 5353 5353  :mm:ss[.SSSSSSSS
+00003ed0: 535d 5a22 2066 6f72 6d61 742e 0a20 2020  S]Z" format..   
+00003ee0: 2020 2020 200a 2020 2020 2020 2020 6461       .        da
+00003ef0: 7465 5f73 7472 696e 6720 3d20 2232 3032  te_string = "202
+00003f00: 332d 3031 2d30 3554 3134 3a33 383a 3235  3-01-05T14:38:25
+00003f10: 2e30 3031 3436 5a22 0a20 2020 2020 2020  .00146Z".       
+00003f20: 200a 2020 2020 2020 2020 2320 5765 2068   .        # We h
+00003f30: 6176 6520 7361 6d65 206d 6574 686f 6473  ave same methods
+00003f40: 2061 7320 696e 2044 6174 6574 696d 6543   as in DatetimeC
+00003f50: 6f6e 7665 7274 6572 0a20 2020 2020 2020  onverter.       
+00003f60: 2064 6174 655f 6d73 5f66 726f 6d5f 7374   date_ms_from_st
+00003f70: 7269 6e67 203d 2044 6174 6574 696d 6553  ring = DatetimeS
+00003f80: 7472 696e 6743 6f6e 7665 7274 6572 2e74  tringConverter.t
+00003f90: 6f5f 6d69 6c6c 6973 6563 6f6e 6473 2864  o_milliseconds(d
+00003fa0: 6174 655f 7374 7269 6e67 290a 2020 2020  ate_string).    
+00003fb0: 2020 2020 6461 7465 5f75 735f 6672 6f6d      date_us_from
+00003fc0: 5f73 7472 696e 6720 3d20 4461 7465 7469  _string = Dateti
+00003fd0: 6d65 5374 7269 6e67 436f 6e76 6572 7465  meStringConverte
+00003fe0: 722e 746f 5f6d 6963 726f 7365 636f 6e64  r.to_microsecond
+00003ff0: 7328 6461 7465 5f73 7472 696e 6729 0a20  s(date_string). 
+00004000: 2020 2020 2020 2064 6174 655f 6e73 5f66         date_ns_f
+00004010: 726f 6d5f 7374 7269 6e67 203d 2044 6174  rom_string = Dat
+00004020: 6574 696d 6553 7472 696e 6743 6f6e 7665  etimeStringConve
+00004030: 7274 6572 2e74 6f5f 6e61 6e6f 7365 636f  rter.to_nanoseco
+00004040: 6e64 7328 6461 7465 5f73 7472 696e 6729  nds(date_string)
+00004050: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00004060: 2020 2320 5765 2063 616e 2061 6c73 6f20    # We can also 
+00004070: 6765 7420 6461 7465 7469 6d65 206f 626a  get datetime obj
+00004080: 6563 7420 6672 6f6d 2073 7472 696e 670a  ect from string.
+00004090: 2020 2020 2020 2020 6461 7465 7469 6d65          datetime
+000040a0: 5f66 726f 6d5f 7374 7269 6e67 203d 2044  _from_string = D
+000040b0: 6174 6574 696d 6553 7472 696e 6743 6f6e  atetimeStringCon
+000040c0: 7665 7274 6572 2e74 6f5f 6461 7465 7469  verter.to_dateti
+000040d0: 6d65 2864 6174 655f 7374 7269 6e67 290a  me(date_string).
+000040e0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000040f0: 2023 205b 322e 335d 2050 726f 746f 6275   # [2.3] Protobu
+00004100: 6654 696d 6573 7461 6d70 436f 6e76 6572  fTimestampConver
+00004110: 7465 720a 2020 2020 2020 2020 2320 5072  ter.        # Pr
+00004120: 6f74 6f62 7566 2074 696d 6573 7461 6d70  otobuf timestamp
+00004130: 7320 6d75 7374 2062 6520 696e 2066 6f72  s must be in for
+00004140: 6d20 7b22 6570 6f63 6853 6563 6f6e 6422  m {"epochSecond"
+00004150: 3a20 7365 636f 6e64 732c 2022 6e61 6e6f  : seconds, "nano
+00004160: 223a 206e 616e 6f73 6563 6f6e 6473 7d0a  ": nanoseconds}.
+00004170: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00004180: 2070 726f 746f 6275 665f 7469 6d65 7374   protobuf_timest
+00004190: 616d 7020 3d20 7b22 6570 6f63 6853 6563  amp = {"epochSec
+000041a0: 6f6e 6422 3a20 3136 3732 3932 3935 3035  ond": 1672929505
+000041b0: 2c20 226e 616e 6f22 3a20 315f 3436 305f  , "nano": 1_460_
+000041c0: 3030 307d 0a20 2020 2020 2020 200a 2020  000}.        .  
+000041d0: 2020 2020 2020 6461 7465 5f6d 735f 6672        date_ms_fr
+000041e0: 6f6d 5f74 696d 6573 7461 6d70 203d 2050  om_timestamp = P
+000041f0: 726f 746f 6275 6654 696d 6573 7461 6d70  rotobufTimestamp
+00004200: 436f 6e76 6572 7465 722e 746f 5f6d 696c  Converter.to_mil
+00004210: 6c69 7365 636f 6e64 7328 7072 6f74 6f62  liseconds(protob
+00004220: 7566 5f74 696d 6573 7461 6d70 290a 2020  uf_timestamp).  
+00004230: 2020 2020 2020 6461 7465 5f75 735f 6672        date_us_fr
+00004240: 6f6d 5f74 696d 6573 7461 6d70 203d 2050  om_timestamp = P
+00004250: 726f 746f 6275 6654 696d 6573 7461 6d70  rotobufTimestamp
+00004260: 436f 6e76 6572 7465 722e 746f 5f6d 6963  Converter.to_mic
+00004270: 726f 7365 636f 6e64 7328 7072 6f74 6f62  roseconds(protob
+00004280: 7566 5f74 696d 6573 7461 6d70 290a 2020  uf_timestamp).  
+00004290: 2020 2020 2020 6461 7465 5f6e 735f 6672        date_ns_fr
+000042a0: 6f6d 5f74 696d 6573 7461 6d70 203d 2050  om_timestamp = P
+000042b0: 726f 746f 6275 6654 696d 6573 7461 6d70  rotobufTimestamp
+000042c0: 436f 6e76 6572 7465 722e 746f 5f6e 616e  Converter.to_nan
+000042d0: 6f73 6563 6f6e 6473 2870 726f 746f 6275  oseconds(protobu
+000042e0: 665f 7469 6d65 7374 616d 7029 0a20 2020  f_timestamp).   
+000042f0: 2020 2020 2064 6174 6574 696d 655f 6672       datetime_fr
+00004300: 6f6d 5f74 696d 6573 7461 6d70 203d 2050  om_timestamp = P
+00004310: 726f 746f 6275 6654 696d 6573 7461 6d70  rotobufTimestamp
+00004320: 436f 6e76 6572 7465 722e 746f 5f64 6174  Converter.to_dat
+00004330: 6574 696d 6528 7072 6f74 6f62 7566 5f74  etime(protobuf_t
+00004340: 696d 6573 7461 6d70 290a 2020 2020 2020  imestamp).      
+00004350: 2020 0a20 2020 2020 2020 2023 2323 2323    .        #####
+00004360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004380: 230a 2020 2020 2020 2020 2320 5b33 5d20  #.        # [3] 
+00004390: 576f 726b 696e 6720 7769 7468 2045 7665  Working with Eve
+000043a0: 6e74 5472 6565 2061 6e64 2045 7665 6e74  ntTree and Event
+000043b0: 5472 6565 436f 6c6c 6563 7469 6f6e 2e0a  TreeCollection..
+000043c0: 2020 2020 2020 2020 2323 2323 2323 2323          ########
+000043d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000043e0: 2323 2323 2323 2323 2323 2323 2323 0a20  ##############. 
+000043f0: 2020 2020 2020 2023 2043 616e 2062 6520         # Can be 
+00004400: 7573 6566 756c 2069 6620 796f 7520 6861  useful if you ha
+00004410: 7665 2064 6174 612d 7374 7265 616d 2077  ve data-stream w
+00004420: 6974 6820 3c20 3130 306b 2065 6c65 6d65  ith < 100k eleme
+00004430: 6e74 732c 206f 7468 6572 7769 7365 2069  nts, otherwise i
+00004440: 740a 2020 2020 2020 2020 2320 7461 6b65  t.        # take
+00004450: 7320 746f 6f20 6d75 6368 2052 414d 2e0a  s too much RAM..
+00004460: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00004470: 2023 205b 332e 315d 2042 7569 6c64 2061   # [3.1] Build a
+00004480: 2063 7573 746f 6d20 4576 656e 7454 7265   custom EventTre
+00004490: 650a 2020 2020 2020 2020 2320 546f 2063  e.        # To c
+000044a0: 7265 6174 6520 616e 2045 7665 6e74 5472  reate an EventTr
+000044b0: 6565 206f 626a 6563 7420 796f 7520 6e65  ee object you ne
+000044c0: 6564 2074 6f20 7072 6f76 6964 6520 6e61  ed to provide na
+000044d0: 6d65 2c20 6964 2061 6e64 2064 6174 6120  me, id and data 
+000044e0: 6f66 2074 6865 2072 6f6f 7420 6576 656e  of the root even
+000044f0: 742e 0a20 2020 2020 2020 2074 7265 6520  t..        tree 
+00004500: 3d20 4576 656e 7454 7265 6528 6576 656e  = EventTree(even
+00004510: 745f 6e61 6d65 3d22 726f 6f74 2065 7665  t_name="root eve
+00004520: 6e74 222c 2065 7665 6e74 5f69 643d 2272  nt", event_id="r
+00004530: 6f6f 745f 6964 222c 2064 6174 613d 7b22  oot_id", data={"
+00004540: 6461 7461 223a 205b 312c 2032 2c20 332c  data": [1, 2, 3,
+00004550: 2034 2c20 355d 7d29 0a20 2020 2020 2020   4, 5]}).       
+00004560: 200a 2020 2020 2020 2020 2320 546f 2061   .        # To a
+00004570: 6464 206e 6577 206e 6f64 6520 7573 6520  dd new node use 
+00004580: 6170 7065 6e64 5f65 7665 6e74 2e20 7061  append_event. pa
+00004590: 7265 6e74 5f69 6420 6973 206e 6563 6573  rent_id is neces
+000045a0: 7361 7279 2c20 6461 7461 2069 7320 6f70  sary, data is op
+000045b0: 7469 6f6e 616c 2e0a 2020 2020 2020 2020  tional..        
+000045c0: 7472 6565 2e61 7070 656e 645f 6576 656e  tree.append_even
+000045d0: 7428 6576 656e 745f 6e61 6d65 3d22 4122  t(event_name="A"
+000045e0: 2c20 6576 656e 745f 6964 3d22 415f 6964  , event_id="A_id
+000045f0: 222c 2064 6174 613d 4e6f 6e65 2c20 7061  ", data=None, pa
+00004600: 7265 6e74 5f69 643d 2272 6f6f 745f 6964  rent_id="root_id
+00004610: 2229 0a20 2020 2020 2020 200a 2020 2020  ").        .    
+00004620: 2020 2020 2320 5b33 2e33 5d20 4275 696c      # [3.3] Buil
+00004630: 6469 6e67 2074 6865 2045 7665 6e74 5472  ding the EventTr
+00004640: 6565 436f 6c6c 6563 7469 6f6e 2e0a 2020  eeCollection..  
+00004650: 2020 2020 2020 6461 7461 5f73 6f75 7263        data_sourc
+00004660: 653a 2049 4461 7461 536f 7572 6365 2020  e: IDataSource  
+00004670: 2320 596f 7520 7368 6f75 6c64 2069 6e69  # You should ini
+00004680: 7420 4461 7461 536f 7572 6365 206f 626a  t DataSource obj
+00004690: 6563 742e 2045 2e67 2e20 6672 6f6d 204c  ect. E.g. from L
+000046a0: 7744 5020 6d6f 6475 6c65 2e0a 2020 2020  wDP module..    
+000046b0: 2020 2020 6461 7461 5f73 6f75 7263 6520      data_source 
+000046c0: 3d20 4475 6d6d 7944 6174 6153 6f75 7263  = DummyDataSourc
+000046d0: 6528 2920 2023 204e 6f74 6521 2057 6520  e()  # Note! We 
+000046e0: 7573 6520 6661 6b65 2044 5320 6865 7265  use fake DS here
+000046f0: 2e0a 2020 2020 2020 2020 2320 4554 4344  ..        # ETCD
+00004700: 7269 7665 7220 6865 7265 2069 7320 6120  river here is a 
+00004710: 7374 7562 2c20 6163 7475 616c 6c79 2074  stub, actually t
+00004720: 6865 206c 6962 2064 6f65 736e 2774 2068  he lib doesn't h
+00004730: 6176 6520 7375 6368 2061 2063 6c61 7373  ave such a class
+00004740: 2e0a 2020 2020 2020 2020 2320 596f 7520  ..        # You 
+00004750: 6361 6e20 7461 6b65 2069 7420 696e 204c  can take it in L
+00004760: 7744 5020 6d6f 6475 6c65 206f 7220 6372  wDP module or cr
+00004770: 6561 7465 2079 6f75 7273 656c 6620 636c  eate yourself cl
+00004780: 6173 7320 6966 2079 6f75 2068 6176 6520  ass if you have 
+00004790: 736f 6d65 2073 7065 6369 616c 2065 7665  some special eve
+000047a0: 6e74 7320 7374 7275 6374 7572 652e 0a20  nts structure.. 
+000047b0: 2020 2020 2020 2066 726f 6d20 7468 325f         from th2_
+000047c0: 6461 7461 5f73 6572 7669 6365 732e 6461  data_services.da
+000047d0: 7461 5f73 6f75 7263 652e 6c77 6470 2e65  ta_source.lwdp.e
+000047e0: 7665 6e74 5f74 7265 6520 696d 706f 7274  vent_tree import
+000047f0: 2048 7474 7045 5443 4472 6976 6572 2061   HttpETCDriver a
+00004800: 7320 4554 4344 7269 7665 720a 2020 2020  s ETCDriver.    
+00004810: 2020 2020 0a20 2020 2020 2020 2023 2049      .        # I
+00004820: 6620 796f 7520 646f 6e27 7420 7370 6563  f you don't spec
+00004830: 6966 7920 6461 7461 5f73 6f75 7263 6520  ify data_source 
+00004840: 666f 7220 7468 6520 6472 6976 6572 2074  for the driver t
+00004850: 6865 6e20 6974 2077 6f6e 2774 2072 6563  hen it won't rec
+00004860: 6f76 6572 2064 6574 6163 6865 6420 6576  over detached ev
+00004870: 656e 7473 2e0a 2020 2020 2020 2020 6472  ents..        dr
+00004880: 6976 6572 3a20 4945 5443 4472 6976 6572  iver: IETCDriver
+00004890: 2020 2320 596f 7520 7368 6f75 6c64 2069    # You should i
+000048a0: 6e69 7420 4554 4344 7269 7665 7220 6f62  nit ETCDriver ob
+000048b0: 6a65 6374 2e20 452e 672e 2066 726f 6d20  ject. E.g. from 
+000048c0: 4c77 4450 206d 6f64 756c 6520 6f72 2079  LwDP module or y
+000048d0: 6f75 7220 6375 7374 6f6d 2063 6c61 7373  our custom class
+000048e0: 2e0a 2020 2020 2020 2020 6472 6976 6572  ..        driver
+000048f0: 203d 2045 5443 4472 6976 6572 2864 6174   = ETCDriver(dat
+00004900: 615f 736f 7572 6365 3d64 6174 615f 736f  a_source=data_so
+00004910: 7572 6365 2c20 7573 655f 7374 7562 3d54  urce, use_stub=T
+00004920: 7275 6529 0a20 2020 2020 2020 200a 2020  rue).        .  
+00004930: 2020 2020 2020 6574 6320 3d20 4576 656e        etc = Even
+00004940: 7454 7265 6543 6f6c 6c65 6374 696f 6e28  tTreeCollection(
+00004950: 6472 6976 6572 290a 2020 2020 2020 2020  driver).        
+00004960: 6574 632e 6275 696c 6428 6576 656e 7473  etc.build(events
+00004970: 290a 2020 2020 2020 2020 6574 632e 7368  ).        etc.sh
+00004980: 6f77 2829 0a20 2020 2020 2020 2023 2049  ow().        # I
+00004990: 7427 6c6c 2070 7269 6e74 2074 6865 2066  t'll print the f
+000049a0: 6f6c 6c6f 7769 6e67 3a0a 2020 2020 2020  ollowing:.      
+000049b0: 2020 2320 5365 7420 6f66 2061 7574 6f2d    # Set of auto-
+000049c0: 6765 6e65 7261 7465 6420 6576 656e 7473  generated events
+000049d0: 2066 6f72 2064 7320 6c69 6220 7465 7374   for ds lib test
+000049e0: 696e 670a 2020 2020 2020 2020 2320 e294  ing.        # ..
+000049f0: 9ce2 9480 e294 8020 506c 6169 6e20 6576  ....... Plain ev
+00004a00: 656e 7420 310a 2020 2020 2020 2020 2320  ent 1.        # 
+00004a10: e294 94e2 9480 e294 8020 506c 6169 6e20  ......... Plain 
+00004a20: 6576 656e 7420 320a 2020 2020 2020 2020  event 2.        
+00004a30: 0a20 2020 2020 2020 2070 7269 6e74 2865  .        print(e
+00004a40: 7463 290a 2020 2020 2020 2020 2320 4576  tc).        # Ev
+00004a50: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
+00004a60: 6e28 7472 6565 733d 312c 2065 7665 6e74  n(trees=1, event
+00004a70: 733d 335b 7472 6565 733d 332c 2064 6574  s=3[trees=3, det
+00004a80: 6163 6865 643d 305d 290a 2020 2020 2020  ached=0]).      
+00004a90: 2020 0a20 2020 2020 2020 2023 2044 6574    .        # Det
+00004aa0: 6163 6865 6420 6576 656e 7473 2069 736e  ached events isn
+00004ab0: 2774 2065 6d70 7479 2e0a 2020 2020 2020  't empty..      
+00004ac0: 2020 6173 7365 7274 2065 7463 2e67 6574    assert etc.get
+00004ad0: 5f64 6574 6163 6865 645f 6576 656e 7473  _detached_events
+00004ae0: 2829 2020 2320 7265 7475 726e 7320 6c69  ()  # returns li
+00004af0: 7374 206f 6620 6465 7461 6368 6564 5f65  st of detached_e
+00004b00: 7665 6e74 732e 0a20 2020 2020 2020 200a  vents..        .
+00004b10: 2020 2020 2020 2020 2320 7265 636f 7665          # recove
+00004b20: 725f 756e 6b6e 6f77 6e5f 6576 656e 7473  r_unknown_events
+00004b30: 202d 2d20 7573 6564 2074 6f20 7265 636f   -- used to reco
+00004b40: 7665 7220 736f 6d65 2065 7665 6e74 7320  ver some events 
+00004b50: 7061 7265 6e74 732e 0a20 2020 2020 2020  parents..       
+00004b60: 2023 2054 6861 7420 776f 6e27 7420 776f   # That won't wo
+00004b70: 726b 2077 6974 6820 4475 6d6d 7944 6174  rk with DummyDat
+00004b80: 6153 6f75 7263 652c 2073 6f20 7761 7320  aSource, so was 
+00004b90: 636f 6d6d 656e 7465 640a 2020 2020 2020  commented.      
+00004ba0: 2020 2320 6574 632e 7265 636f 7665 725f    # etc.recover_
+00004bb0: 756e 6b6e 6f77 6e5f 6576 656e 7473 2829  unknown_events()
+00004bc0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00004bd0: 2020 2320 4166 7465 7220 7468 6174 2074    # After that t
+00004be0: 6865 2064 6574 6163 6865 6420 6576 656e  he detached even
+00004bf0: 7473 2073 686f 756c 6420 6265 2065 6d70  ts should be emp
+00004c00: 7479 2062 6563 6175 7365 2074 6865 7920  ty because they 
+00004c10: 7765 7265 2072 6563 6f76 6572 6564 2e0a  were recovered..
+00004c20: 2020 2020 2020 2020 2320 6173 7365 7274          # assert
+00004c30: 206e 6f74 2065 7463 2e67 6574 5f64 6574   not etc.get_det
+00004c40: 6163 6865 645f 6576 656e 7473 2829 0a20  ached_events(). 
+00004c50: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00004c60: 2320 2d2d 2d2d 2d0a 2020 2020 2020 2020  # -----.        
+00004c70: 0a20 2020 2020 2020 2023 2054 6865 2063  .        # The c
+00004c80: 6f6c 6c65 6374 696f 6e20 6861 7320 4576  ollection has Ev
+00004c90: 656e 7454 7265 6573 2065 6163 6820 7769  entTrees each wi
+00004ca0: 7468 2061 2074 7265 6520 6f66 2065 7665  th a tree of eve
+00004cb0: 6e74 732e 0a20 2020 2020 2020 2023 2055  nts..        # U
+00004cc0: 7369 6e67 2043 6f6c 6c65 6374 696f 6e20  sing Collection 
+00004cd0: 616e 6420 4576 656e 7454 7265 6573 2c20  and EventTrees, 
+00004ce0: 796f 7520 6361 6e20 776f 726b 2066 6c65  you can work fle
+00004cf0: 7869 626c 7920 7769 7468 2065 7665 6e74  xibly with event
+00004d00: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
+00004d10: 2020 2020 2320 5b33 2e33 2e31 5d20 4765      # [3.3.1] Ge
+00004d20: 7420 6c65 6176 6573 206f 6620 616c 6c20  t leaves of all 
+00004d30: 7472 6565 732e 0a20 2020 2020 2020 206c  trees..        l
+00004d40: 6561 7665 733a 2054 7570 6c65 5b64 6963  eaves: Tuple[dic
+00004d50: 745d 203d 2065 7463 2e67 6574 5f6c 6561  t] = etc.get_lea
+00004d60: 7665 7328 2920 2023 2052 6574 7572 6e73  ves()  # Returns
+00004d70: 2061 2074 7570 6c65 206f 6620 6c65 6176   a tuple of leav
+00004d80: 6573 2065 7665 6e74 730a 2020 2020 2020  es events.      
+00004d90: 2020 0a20 2020 2020 2020 2023 205b 332e    .        # [3.
+00004da0: 332e 325d 2047 6574 2072 6f6f 7473 2069  3.2] Get roots i
+00004db0: 6473 206f 6620 616c 6c20 7472 6565 732e  ds of all trees.
+00004dc0: 0a20 2020 2020 2020 2072 6f6f 7473 3a20  .        roots: 
+00004dd0: 4c69 7374 5b73 7472 5d20 3d20 6574 632e  List[str] = etc.
+00004de0: 6765 745f 726f 6f74 735f 6964 7328 290a  get_roots_ids().
+00004df0: 2020 2020 2020 2020 2320 5265 7475 726e          # Return
+00004e00: 7320 7468 6520 6c69 7374 206f 6620 726f  s the list of ro
+00004e10: 6f74 2049 6473 3a0a 2020 2020 2020 2020  ot Ids:.        
+00004e20: 2320 5b27 6465 6d6f 5f62 6f6f 6b5f 313a  # ['demo_book_1:
+00004e30: 7468 322d 7363 6f70 653a 3230 3233 3031  th2-scope:202301
+00004e40: 3035 3133 3537 3035 3536 3038 3733 3030  0513570556087300
+00004e50: 303a 6436 3165 3933 3061 2d38 6430 302d  0:d61e930a-8d00-
+00004e60: 3131 6564 2d61 6131 612d 6433 3461 3631  11ed-aa1a-d34a61
+00004e70: 3535 3135 3264 5f31 275d 0a20 2020 2020  55152d_1'].     
+00004e80: 2020 200a 2020 2020 2020 2020 2320 5b33     .        # [3
+00004e90: 2e33 2e33 5d20 4669 6e64 2061 6e20 6576  .3.3] Find an ev
+00004ea0: 656e 7420 696e 2061 6c6c 2074 7265 6573  ent in all trees
+00004eb0: 2e0a 2020 2020 2020 2020 6669 6e64 5f65  ..        find_e
+00004ec0: 7665 6e74 3a20 4f70 7469 6f6e 616c 5b64  vent: Optional[d
+00004ed0: 6963 745d 203d 2065 7463 2e66 696e 6428  ict] = etc.find(
+00004ee0: 6c61 6d62 6461 2065 7665 6e74 3a20 2253  lambda event: "S
+00004ef0: 656e 6420 6d65 7373 6167 6522 2069 6e20  end message" in 
+00004f00: 6576 656e 745b 2265 7665 6e74 5479 7065  event["eventType
+00004f10: 225d 290a 2020 2020 2020 2020 0a20 2020  "]).        .   
+00004f20: 2020 2020 2023 205b 332e 332e 345d 2046       # [3.3.4] F
+00004f30: 696e 6420 616c 6c20 6576 656e 7473 2069  ind all events i
+00004f40: 6e20 616c 6c20 7472 6565 732e 2054 6865  n all trees. The
+00004f50: 7265 2069 7320 616c 736f 2069 7465 7261  re is also itera
+00004f60: 626c 6520 7665 7273 696f 6e20 2766 696e  ble version 'fin
+00004f70: 6461 6c6c 5f69 7465 7227 2e0a 2020 2020  dall_iter'..    
+00004f80: 2020 2020 6669 6e64 5f65 7665 6e74 733a      find_events:
+00004f90: 204c 6973 745b 6469 6374 5d20 3d20 6574   List[dict] = et
+00004fa0: 632e 6669 6e64 616c 6c28 6c61 6d62 6461  c.findall(lambda
+00004fb0: 2065 7665 6e74 3a20 6576 656e 745b 2273   event: event["s
+00004fc0: 7563 6365 7373 6675 6c22 5d20 6973 2054  uccessful"] is T
+00004fd0: 7275 6529 0a20 2020 2020 2020 200a 2020  rue).        .  
+00004fe0: 2020 2020 2020 2320 5b33 2e33 2e35 5d20        # [3.3.5] 
+00004ff0: 4669 6e64 2061 6e20 616e 6365 7374 6f72  Find an ancestor
+00005000: 206f 6620 7468 6520 6576 656e 742e 0a20   of the event.. 
+00005010: 2020 2020 2020 2061 6e63 6573 746f 723a         ancestor:
+00005020: 204f 7074 696f 6e61 6c5b 6469 6374 5d20   Optional[dict] 
+00005030: 3d20 6574 632e 6669 6e64 5f61 6e63 6573  = etc.find_ances
+00005040: 746f 7228 0a20 2020 2020 2020 2020 2020  tor(.           
+00005050: 2022 6465 6d6f 5f62 6f6f 6b5f 313a 7468   "demo_book_1:th
+00005060: 322d 7363 6f70 653a 3230 3233 3031 3035  2-scope:20230105
+00005070: 3133 3537 3035 3536 3038 3733 3030 303a  135705560873000:
+00005080: 6436 3165 3933 3061 2d38 6430 302d 3131  d61e930a-8d00-11
+00005090: 6564 2d61 6131 612d 6433 3461 3631 3535  ed-aa1a-d34a6155
+000050a0: 3135 3264 5f31 222c 0a20 2020 2020 2020  152d_1",.       
+000050b0: 2020 2020 2066 696c 7465 723d 6c61 6d62       filter=lamb
+000050c0: 6461 2065 7665 6e74 3a20 2252 6f6f 7445  da event: "RootE
+000050d0: 7665 6e74 2220 696e 2065 7665 6e74 5b22  vent" in event["
+000050e0: 6576 656e 744e 616d 6522 5d2c 0a20 2020  eventName"],.   
+000050f0: 2020 2020 2029 0a20 2020 2020 2020 200a       ).        .
+00005100: 2020 2020 2020 2020 2320 5b33 2e33 2e36          # [3.3.6
+00005110: 5d20 4765 7420 6368 696c 6472 656e 206f  ] Get children o
+00005120: 6620 7468 6520 6576 656e 742e 2054 6865  f the event. The
+00005130: 7265 2069 7320 616c 736f 2069 7465 7261  re is also itera
+00005140: 626c 6520 7665 7273 696f 6e20 2767 6574  ble version 'get
+00005150: 5f63 6869 6c64 7265 6e5f 6974 6572 272e  _children_iter'.
+00005160: 0a20 2020 2020 2020 2063 6869 6c64 7265  .        childre
+00005170: 6e3a 2054 7570 6c65 5b64 6963 745d 203d  n: Tuple[dict] =
+00005180: 2065 7463 2e67 6574 5f63 6869 6c64 7265   etc.get_childre
+00005190: 6e28 0a20 2020 2020 2020 2020 2020 2022  n(.            "
+000051a0: 6465 6d6f 5f62 6f6f 6b5f 313a 7468 322d  demo_book_1:th2-
+000051b0: 7363 6f70 653a 3230 3233 3031 3035 3133  scope:2023010513
+000051c0: 3537 3035 3536 3038 3733 3030 303a 6436  5705560873000:d6
+000051d0: 3165 3933 3061 2d38 6430 302d 3131 6564  1e930a-8d00-11ed
+000051e0: 2d61 6131 612d 6433 3461 3631 3535 3135  -aa1a-d34a615515
+000051f0: 3264 5f31 220a 2020 2020 2020 2020 290a  2d_1".        ).
+00005200: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00005210: 2023 205b 332e 332e 375d 2047 6574 2073   # [3.3.7] Get s
+00005220: 7562 7472 6565 2066 6f72 2073 7065 6369  ubtree for speci
+00005230: 6669 6564 2065 7665 6e74 2e0a 2020 2020  fied event..    
+00005240: 2020 2020 7375 6274 7265 653a 2045 7665      subtree: Eve
+00005250: 6e74 5472 6565 203d 2065 7463 2e67 6574  ntTree = etc.get
+00005260: 5f73 7562 7472 6565 280a 2020 2020 2020  _subtree(.      
+00005270: 2020 2020 2020 2264 656d 6f5f 626f 6f6b        "demo_book
+00005280: 5f31 3a74 6832 2d73 636f 7065 3a32 3032  _1:th2-scope:202
+00005290: 3330 3130 3531 3335 3730 3535 3630 3837  3010513570556087
+000052a0: 3330 3030 3a64 3631 6539 3330 612d 3864  3000:d61e930a-8d
+000052b0: 3030 2d31 3165 642d 6161 3161 2d64 3334  00-11ed-aa1a-d34
+000052c0: 6136 3135 3531 3532 645f 3122 0a20 2020  a6155152d_1".   
+000052d0: 2020 2020 2029 0a20 2020 2020 2020 200a       ).        .
+000052e0: 2020 2020 2020 2020 2320 5b33 2e33 2e38          # [3.3.8
+000052f0: 5d20 4765 7420 6675 6c6c 2070 6174 6820  ] Get full path 
+00005300: 746f 2074 6865 2065 7665 6e74 2e0a 2020  to the event..  
+00005310: 2020 2020 2020 2320 4c6f 6f6b 7320 6c69        # Looks li
+00005320: 6b65 205b 616e 6365 7374 6f72 5f72 6f6f  ke [ancestor_roo
+00005330: 742c 2061 6e63 6573 746f 725f 6c65 7665  t, ancestor_leve
+00005340: 6c31 2c20 616e 6365 7374 6f72 5f6c 6576  l1, ancestor_lev
+00005350: 656c 322c 2065 7665 6e74 5d0a 2020 2020  el2, event].    
+00005360: 2020 2020 6576 656e 745f 7061 7468 3a20      event_path: 
+00005370: 4c69 7374 5b64 6963 745d 203d 2065 7463  List[dict] = etc
+00005380: 2e67 6574 5f66 756c 6c5f 7061 7468 280a  .get_full_path(.
+00005390: 2020 2020 2020 2020 2020 2020 2264 656d              "dem
+000053a0: 6f5f 626f 6f6b 5f31 3a74 6832 2d73 636f  o_book_1:th2-sco
+000053b0: 7065 3a32 3032 3330 3130 3531 3335 3730  pe:2023010513570
+000053c0: 3535 3630 3837 3330 3030 3a64 3631 6539  5560873000:d61e9
+000053d0: 3330 612d 3864 3030 2d31 3165 642d 6161  30a-8d00-11ed-aa
+000053e0: 3161 2d64 3334 6136 3135 3531 3532 645f  1a-d34a6155152d_
+000053f0: 3122 0a20 2020 2020 2020 2029 0a20 2020  1".        ).   
+00005400: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+00005410: 5b33 2e33 2e39 5d20 4765 7420 7061 7265  [3.3.9] Get pare
+00005420: 6e74 206f 6620 7468 6520 6576 656e 742e  nt of the event.
+00005430: 0a20 2020 2020 2020 2070 6172 656e 7420  .        parent 
+00005440: 3d20 6574 632e 6765 745f 7061 7265 6e74  = etc.get_parent
+00005450: 280a 2020 2020 2020 2020 2020 2020 2264  (.            "d
+00005460: 656d 6f5f 626f 6f6b 5f31 3a74 6832 2d73  emo_book_1:th2-s
+00005470: 636f 7065 3a32 3032 3330 3130 3531 3335  cope:20230105135
+00005480: 3730 3535 3630 3837 3330 3030 3a64 3631  705560873000:d61
+00005490: 6539 3330 612d 3864 3030 2d31 3165 642d  e930a-8d00-11ed-
+000054a0: 6161 3161 2d64 3334 6136 3135 3531 3532  aa1a-d34a6155152
+000054b0: 645f 3122 0a20 2020 2020 2020 2029 0a20  d_1".        ). 
+000054c0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000054d0: 2320 5b33 2e33 2e31 305d 2041 7070 656e  # [3.3.10] Appen
+000054e0: 6420 6e65 7720 6576 656e 7420 746f 2074  d new event to t
+000054f0: 6865 2063 6f6c 6c65 6374 696f 6e2e 0a20  he collection.. 
+00005500: 2020 2020 2020 2065 7463 2e61 7070 656e         etc.appen
+00005510: 645f 6576 656e 7428 0a20 2020 2020 2020  d_event(.       
+00005520: 2020 2020 2065 7665 6e74 3d7b 0a20 2020       event={.   
+00005530: 2020 2020 2020 2020 2020 2020 2022 6576               "ev
+00005540: 656e 7449 6422 3a20 2261 3230 6635 6566  entId": "a20f5ef
+00005550: 342d 6333 6665 2d62 6231 302d 6132 3963  4-c3fe-bb10-a29c
+00005560: 2d64 6433 6437 3834 3930 3965 6222 2c0a  -dd3d784909eb",.
+00005570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005580: 2270 6172 656e 7445 7665 6e74 4964 223a  "parentEventId":
+00005590: 2022 3865 3235 3234 6661 2d63 6635 392d   "8e2524fa-cf59-
+000055a0: 3131 6562 2d61 3366 372d 3039 3466 3930  11eb-a3f7-094f90
+000055b0: 3463 3361 3632 222c 0a20 2020 2020 2020  4c3a62",.       
+000055c0: 2020 2020 2020 2020 2022 6576 656e 744e           "eventN
+000055d0: 616d 6522 3a20 2253 7475 6245 7665 6e74  ame": "StubEvent
+000055e0: 222c 0a20 2020 2020 2020 2020 2020 207d  ",.            }
+000055f0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00005600: 2020 200a 2020 2020 2020 2020 2320 5b33     .        # [3
+00005610: 2e33 2e31 315d 2053 686f 7720 7468 6520  .3.11] Show the 
+00005620: 656e 7469 7265 2063 6f6c 6c65 6374 696f  entire collectio
+00005630: 6e2e 0a20 2020 2020 2020 2065 7463 2e73  n..        etc.s
+00005640: 686f 7728 290a 2020 2020 2020 2020 2320  how().        # 
+00005650: 4974 276c 6c20 7072 696e 7420 7468 6520  It'll print the 
+00005660: 666f 6c6c 6f77 696e 673a 0a20 2020 2020  following:.     
+00005670: 2020 2023 2053 6574 206f 6620 6175 746f     # Set of auto
+00005680: 2d67 656e 6572 6174 6564 2065 7665 6e74  -generated event
+00005690: 7320 666f 7220 6473 206c 6962 2074 6573  s for ds lib tes
+000056a0: 7469 6e67 0a20 2020 2020 2020 2023 20e2  ting.        # .
+000056b0: 949c e294 80e2 9480 2050 6c61 696e 2065  ........ Plain e
+000056c0: 7665 6e74 2031 0a20 2020 2020 2020 2023  vent 1.        #
+000056d0: 20e2 9494 e294 80e2 9480 2050 6c61 696e   ......... Plain
+000056e0: 2065 7665 6e74 2032 0a20 2020 2020 2020   event 2.       
+000056f0: 200a 2020 2020 2020 2020 2320 4173 2079   .        # As y
+00005700: 6f75 2063 616e 2073 6565 2c20 6e6f 7468  ou can see, noth
+00005710: 696e 6720 7761 7320 6368 616e 6765 642c  ing was changed,
+00005720: 2062 7574 2077 6520 6164 6465 6420 7468   but we added th
+00005730: 6520 6e65 7720 6576 656e 7421 0a20 2020  e new event!.   
+00005740: 2020 2020 2023 206c 6574 2773 206c 6f6f       # let's loo
+00005750: 6b20 6174 2074 6865 2073 756d 6d61 7279  k at the summary
+00005760: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00005770: 2020 2070 7269 6e74 2865 7463 2e73 756d     print(etc.sum
+00005780: 6d61 7279 2829 2920 2023 2074 6865 2073  mary())  # the s
+00005790: 616d 6520 6173 206a 7573 7420 7072 696e  ame as just prin
+000057a0: 7428 6574 6329 0a20 2020 2020 2020 2023  t(etc).        #
+000057b0: 2045 7665 6e74 5472 6565 436f 6c6c 6563   EventTreeCollec
+000057c0: 7469 6f6e 2874 7265 6573 3d31 2c20 6576  tion(trees=1, ev
+000057d0: 656e 7473 3d35 5b74 7265 6573 3d33 2c20  ents=5[trees=3, 
+000057e0: 6465 7461 6368 6564 3d32 5d29 0a20 2020  detached=2]).   
+000057f0: 2020 2020 2023 2059 6f75 2063 616e 2073       # You can s
+00005800: 6565 2074 6861 7420 6974 2077 6173 2061  ee that it was a
+00005810: 6464 6564 2074 6f20 6465 7461 6368 6564  dded to detached
+00005820: 2e20 5468 6174 2773 2077 6879 2079 6f75  . That's why you
+00005830: 2064 6f6e 2774 2073 6565 2074 6865 2065   don't see the e
+00005840: 7665 6e74 0a20 2020 2020 2020 2023 2076  vent.        # v
+00005850: 6961 2060 7368 6f77 2829 602e 2060 7368  ia `show()`. `sh
+00005860: 6f77 2829 6020 7072 696e 7473 206f 6e6c  ow()` prints onl
+00005870: 7920 5472 6565 7321 0a20 2020 2020 2020  y Trees!.       
+00005880: 2023 2055 7365 2060 6574 632e 6765 745f   # Use `etc.get_
+00005890: 7061 7265 6e74 6c65 7373 5f74 7265 6573  parentless_trees
+000058a0: 2829 6020 746f 2063 6f6e 7665 7274 2064  ()` to convert d
+000058b0: 6574 6163 6865 6420 6576 656e 7473 2074  etached events t
+000058c0: 6f20 7472 6565 732e 0a20 2020 2020 2020  o trees..       
+000058d0: 2023 204d 6f72 6520 696e 666f 726d 6174   # More informat
+000058e0: 696f 6e20 6265 6c6f 7720 696e 2074 6865  ion below in the
+000058f0: 2063 6f72 7265 7370 6f6e 6469 6e67 2073   corresponding s
+00005900: 6563 7469 6f6e 2e0a 2020 2020 2020 2020  ection..        
+00005910: 0a20 2020 2020 2020 2023 202d 2d2d 2d2d  .        # -----
+00005920: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00005930: 2020 2320 5b33 2e34 5d20 576f 726b 696e    # [3.4] Workin
+00005940: 6720 7769 7468 2074 6865 2045 7665 6e74  g with the Event
+00005950: 5472 6565 2e0a 2020 2020 2020 2020 2320  Tree..        # 
+00005960: 4576 656e 7454 7265 6520 6861 7320 7468  EventTree has th
+00005970: 6520 7361 6d65 206d 6574 686f 6473 2061  e same methods a
+00005980: 7320 4576 656e 7454 7265 6543 6f6c 6c65  s EventTreeColle
+00005990: 6374 696f 6e2c 2062 7574 206f 6e6c 7920  ction, but only 
+000059a0: 666f 7220 6974 7320 6f77 6e20 7472 6565  for its own tree
+000059b0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+000059c0: 2020 2023 205b 332e 342e 315d 2047 6574     # [3.4.1] Get
+000059d0: 2061 2063 6f6c 6c65 6374 696f 6e20 6f66   a collection of
+000059e0: 2074 7265 6573 2e0a 2020 2020 2020 2020   trees..        
+000059f0: 7472 6565 733a 204c 6973 745b 4576 656e  trees: List[Even
+00005a00: 7454 7265 655d 203d 2065 7463 2e67 6574  tTree] = etc.get
+00005a10: 5f74 7265 6573 2829 0a20 2020 2020 2020  _trees().       
+00005a20: 2074 7265 653a 2045 7665 6e74 5472 6565   tree: EventTree
+00005a30: 203d 2074 7265 6573 5b30 5d0a 2020 2020   = trees[0].    
+00005a40: 2020 2020 0a20 2020 2020 2020 2023 2042      .        # B
+00005a50: 7574 2045 7665 6e74 5472 6565 2070 726f  ut EventTree pro
+00005a60: 7669 6465 7320 6120 776f 726b 2077 6974  vides a work wit
+00005a70: 6820 7468 6520 7472 6565 2c20 6275 7420  h the tree, but 
+00005a80: 646f 6573 206e 6f74 206d 6f64 6966 7920  does not modify 
+00005a90: 6974 2e0a 2020 2020 2020 2020 2320 4966  it..        # If
+00005aa0: 2079 6f75 2077 616e 7420 746f 206d 6f64   you want to mod
+00005ab0: 6966 7920 7468 6520 7472 6565 2c20 7573  ify the tree, us
+00005ac0: 6520 4576 656e 7454 7265 6543 6f6c 6c65  e EventTreeColle
+00005ad0: 6374 696f 6e73 2e0a 2020 2020 2020 2020  ctions..        
+00005ae0: 0a20 2020 2020 2020 2023 205b 332e 355d  .        # [3.5]
+00005af0: 2057 6f72 6b69 6e67 2077 6974 6820 5061   Working with Pa
+00005b00: 7265 6e74 6c65 7373 5472 6565 2e0a 2020  rentlessTree..  
+00005b10: 2020 2020 2020 2320 5061 7265 6e74 6c65        # Parentle
+00005b20: 7373 5472 6565 2069 7320 616e 2045 7665  ssTree is an Eve
+00005b30: 6e74 5472 6565 2074 6861 7420 6861 7320  ntTree that has 
+00005b40: 6465 7461 6368 6564 2065 7665 6e74 7320  detached events 
+00005b50: 7769 7468 2073 7475 6273 2e0a 2020 2020  with stubs..    
+00005b60: 2020 2020 7061 7265 6e74 6c65 7373 5f74      parentless_t
+00005b70: 7265 6573 3a20 4c69 7374 5b45 7665 6e74  rees: List[Event
+00005b80: 5472 6565 5d20 3d20 6574 632e 6765 745f  Tree] = etc.get_
+00005b90: 7061 7265 6e74 6c65 7373 5f74 7265 6573  parentless_trees
+00005ba0: 2829 0a20 2020 2020 2020 2070 7269 6e74  ().        print
+00005bb0: 2822 7061 7265 6e74 6c65 7373 5f74 7265  ("parentless_tre
+00005bc0: 6573 2063 6f6e 7461 696e 733a 2229 0a20  es contains:"). 
+00005bd0: 2020 2020 2020 2070 7269 6e74 2870 6172         print(par
+00005be0: 656e 746c 6573 735f 7472 6565 7329 0a20  entless_trees). 
+00005bf0: 2020 2020 2020 2023 205b 4576 656e 7454         # [EventT
+00005c00: 7265 6528 6e61 6d65 3d27 3c42 726f 6b65  ree(name='<Broke
+00005c10: 6e45 7665 6e74 3e27 2c20 726f 6f74 5f69  nEvent>', root_i
+00005c20: 643d 276e 6f74 5f65 7869 7374 735f 696e  d='not_exists_in
+00005c30: 5f74 6865 5f65 7665 6e74 735f 7374 7265  _the_events_stre
+00005c40: 616d 272c 2065 7665 6e74 733d 3229 2c0a  am', events=2),.
+00005c50: 2020 2020 2020 2020 2320 2045 7665 6e74          #  Event
+00005c60: 5472 6565 286e 616d 653d 273c 4272 6f6b  Tree(name='<Brok
+00005c70: 656e 4576 656e 743e 272c 2072 6f6f 745f  enEvent>', root_
+00005c80: 6964 3d27 3865 3235 3234 6661 2d63 6635  id='8e2524fa-cf5
+00005c90: 392d 3131 6562 2d61 3366 372d 3039 3466  9-11eb-a3f7-094f
+00005ca0: 3930 3463 3361 3632 272c 2065 7665 6e74  904c3a62', event
+00005cb0: 733d 3229 5d0a 2020 2020 2020 2020 0a20  s=2)].        . 
+00005cc0: 2020 2020 2020 2070 7269 6e74 2822 5c6e         print("\n
+00005cd0: 2220 2265 7463 2061 6674 6572 2060 6765  " "etc after `ge
+00005ce0: 745f 7061 7265 6e74 6c65 7373 5f74 7265  t_parentless_tre
+00005cf0: 6573 603a 2229 0a20 2020 2020 2020 2070  es`:").        p
+00005d00: 7269 6e74 2865 7463 2e73 756d 6d61 7279  rint(etc.summary
+00005d10: 2829 290a 2020 2020 2020 2020 2320 4576  ()).        # Ev
+00005d20: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
+00005d30: 6e28 7472 6565 733d 335b 7265 6775 6c61  n(trees=3[regula
+00005d40: 723d 312c 2070 6172 656e 746c 6573 733d  r=1, parentless=
+00005d50: 325d 2c20 6576 656e 7473 3d37 5b74 7265  2], events=7[tre
+00005d60: 6573 3d37 2c20 6465 7461 6368 6564 3d30  es=7, detached=0
+00005d70: 5d29 270a 2020 2020 2020 2020 6574 632e  ])'.        etc.
+00005d80: 7368 6f77 2829 0a20 2020 2020 2020 2023  show().        #
+00005d90: 2053 6574 206f 6620 6175 746f 2d67 656e   Set of auto-gen
+00005da0: 6572 6174 6564 2065 7665 6e74 7320 666f  erated events fo
+00005db0: 7220 6473 206c 6962 2074 6573 7469 6e67  r ds lib testing
+00005dc0: 0a20 2020 2020 2020 2023 20e2 949c e294  .        # .....
+00005dd0: 80e2 9480 2050 6c61 696e 2065 7665 6e74  .... Plain event
+00005de0: 2031 0a20 2020 2020 2020 2023 20e2 9494   1.        # ...
+00005df0: e294 80e2 9480 2050 6c61 696e 2065 7665  ...... Plain eve
+00005e00: 6e74 2032 0a20 2020 2020 2020 2023 203c  nt 2.        # <
+00005e10: 4272 6f6b 656e 4576 656e 743e 0a20 2020  BrokenEvent>.   
+00005e20: 2020 2020 2023 20e2 9494 e294 80e2 9480       # .........
+00005e30: 2046 616b 6520 6576 656e 740a 2020 2020   Fake event.    
+00005e40: 2020 2020 2320 3c42 726f 6b65 6e45 7665      # <BrokenEve
+00005e50: 6e74 3e0a 2020 2020 2020 2020 2320 e294  nt>.        # ..
+00005e60: 94e2 9480 e294 8020 5374 7562 4576 656e  ....... StubEven
+00005e70: 7420 2020 203c 2d2d 2d20 7468 6520 6576  t    <--- the ev
+00005e80: 656e 7420 7468 6174 2077 6173 2061 6464  ent that was add
+00005e90: 6564 2061 626f 7665 0a20 2020 2020 2020  ed above.       
+00005ea0: 200a 2020 2020 2020 2020 2320 5b33 2e36   .        # [3.6
+00005eb0: 5d20 576f 726b 696e 6720 7769 7468 2050  ] Working with P
+00005ec0: 6172 656e 7445 7665 6e74 5472 6565 436f  arentEventTreeCo
+00005ed0: 6c6c 6563 7469 6f6e 2e0a 2020 2020 2020  llection..      
+00005ee0: 2020 2320 5061 7265 6e74 4576 656e 7454    # ParentEventT
+00005ef0: 7265 6543 6f6c 6c65 6374 696f 6e20 6973  reeCollection is
+00005f00: 2061 2074 7265 6520 636f 6c6c 6563 7469   a tree collecti
+00005f10: 6f6e 206c 696b 6520 4576 656e 7454 7265  on like EventTre
+00005f20: 6543 6f6c 6c65 6374 696f 6e2c 0a20 2020  eCollection,.   
+00005f30: 2020 2020 2023 2062 7574 2069 7420 6861       # but it ha
+00005f40: 7320 6f6e 6c79 2065 7665 6e74 7320 7468  s only events th
+00005f50: 6174 2068 6176 6520 7265 6665 7265 6e63  at have referenc
+00005f60: 6573 2e0a 2020 2020 2020 2020 6461 7461  es..        data
+00005f70: 5f73 6f75 7263 653a 2049 4461 7461 536f  _source: IDataSo
+00005f80: 7572 6365 2020 2320 596f 7520 7368 6f75  urce  # You shou
+00005f90: 6c64 2069 6e69 7420 4461 7461 536f 7572  ld init DataSour
+00005fa0: 6365 206f 626a 6563 742e 2045 2e67 2e20  ce object. E.g. 
+00005fb0: 6672 6f6d 204c 7744 5020 6d6f 6475 6c65  from LwDP module
+00005fc0: 2e0a 2020 2020 2020 2020 6461 7461 5f73  ..        data_s
+00005fd0: 6f75 7263 6520 3d20 4475 6d6d 7944 6174  ource = DummyDat
+00005fe0: 6153 6f75 7263 6528 2920 2023 204e 6f74  aSource()  # Not
+00005ff0: 6521 2057 6520 7573 6520 6661 6b65 2044  e! We use fake D
+00006000: 5320 6865 7265 2e0a 2020 2020 2020 2020  S here..        
+00006010: 2320 4554 4344 7269 7665 7220 6865 7265  # ETCDriver here
+00006020: 2069 7320 6120 7374 7562 2c20 6163 7475   is a stub, actu
+00006030: 616c 6c79 2074 6865 206c 6962 2064 6f65  ally the lib doe
+00006040: 736e 2774 2068 6176 6520 7375 6368 2061  sn't have such a
+00006050: 2063 6c61 7373 2e0a 2020 2020 2020 2020   class..        
+00006060: 2320 596f 7520 6361 6e20 7461 6b65 2069  # You can take i
+00006070: 7420 696e 204c 7744 5020 6d6f 6475 6c65  t in LwDP module
+00006080: 206f 7220 6372 6561 7465 2079 6f75 7273   or create yours
+00006090: 656c 6620 636c 6173 7320 6966 2079 6f75  elf class if you
+000060a0: 2068 6176 6520 736f 6d65 2073 7065 6369   have some speci
+000060b0: 616c 2065 7665 6e74 7320 7374 7275 6374  al events struct
+000060c0: 7572 652e 0a20 2020 2020 2020 2066 726f  ure..        fro
+000060d0: 6d20 7468 325f 6461 7461 5f73 6572 7669  m th2_data_servi
+000060e0: 6365 732e 6461 7461 5f73 6f75 7263 652e  ces.data_source.
+000060f0: 6c77 6470 2e65 7665 6e74 5f74 7265 6520  lwdp.event_tree 
+00006100: 696d 706f 7274 2048 7474 7045 5443 4472  import HttpETCDr
+00006110: 6976 6572 2061 7320 4554 4344 7269 7665  iver as ETCDrive
+00006120: 720a 2020 2020 2020 2020 0a20 2020 2020  r.        .     
+00006130: 2020 2064 7269 7665 7220 3d20 4554 4344     driver = ETCD
+00006140: 7269 7665 7228 6461 7461 5f73 6f75 7263  river(data_sourc
+00006150: 653d 6461 7461 5f73 6f75 7263 6529 0a20  e=data_source). 
+00006160: 2020 2020 2020 2070 6574 6320 3d20 5061         petc = Pa
+00006170: 7265 6e74 4576 656e 7454 7265 6543 6f6c  rentEventTreeCol
+00006180: 6c65 6374 696f 6e28 6472 6976 6572 290a  lection(driver).
+00006190: 2020 2020 2020 2020 7065 7463 2e62 7569          petc.bui
+000061a0: 6c64 2865 7665 6e74 7329 0a20 2020 2020  ld(events).     
+000061b0: 2020 200a 2020 2020 2020 2020 7065 7463     .        petc
+000061c0: 2e73 686f 7728 290a 2020 2020 2020 2020  .show().        
+000061d0: 7065 7463 2e73 756d 6d61 7279 2829 0a20  petc.summary(). 
+000061e0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000061f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006200: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006210: 2323 2323 2323 0a20 2020 2020 2020 2023  ######.        #
+00006220: 205b 345d 2046 6965 6c64 2052 6573 6f6c   [4] Field Resol
+00006230: 7665 7273 0a20 2020 2020 2020 2023 2323  vers.        ###
+00006240: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006250: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006260: 2323 230a 2020 2020 2020 2020 2320 506c  ###.        # Pl
+00006270: 6561 7365 2072 6561 6420 6046 6965 6c64  ease read `Field
+00006280: 2052 6573 6f6c 7665 7273 6020 626c 6f63   Resolvers` bloc
+00006290: 6b20 696e 2072 6561 646d 6520 6669 7273  k in readme firs
+000062a0: 742e 0a20 2020 2020 2020 200a 2020 2020  t..        .    
+000062b0: 2020 2020 2320 5b34 2e31 5d20 5573 6167      # [4.1] Usag
+000062c0: 6520 6578 616d 706c 6520 6672 6f6d 2063  e example from c
+000062d0: 6c69 656e 7420 636f 6465 0a20 2020 2020  lient code.     
+000062e0: 2020 2066 726f 6d20 7468 325f 6461 7461     from th2_data
+000062f0: 5f73 6572 7669 6365 732e 6461 7461 5f73  _services.data_s
+00006300: 6f75 7263 6520 696d 706f 7274 2028 0a20  ource import (. 
+00006310: 2020 2020 2020 2020 2020 206c 7764 702c             lwdp,
+00006320: 0a20 2020 2020 2020 2029 2020 2320 6c77  .        )  # lw
+00006330: 6470 2064 6174 615f 736f 7572 6365 2069  dp data_source i
+00006340: 6e69 7469 616c 697a 6520 7468 325f 6461  nitialize th2_da
+00006350: 7461 5f73 6572 7669 6365 732e 636f 6e66  ta_services.conf
+00006360: 6967 2064 7572 696e 6720 696d 706f 7274  ig during import
+00006370: 2e0a 2020 2020 2020 2020 6672 6f6d 2074  ..        from t
+00006380: 6832 5f64 6174 615f 7365 7276 6963 6573  h2_data_services
+00006390: 2e63 6f6e 6669 6720 696d 706f 7274 206f  .config import o
+000063a0: 7074 696f 6e73 2061 7320 6f5f 0a20 2020  ptions as o_.   
+000063b0: 2020 2020 2066 726f 6d20 7468 325f 6461       from th2_da
+000063c0: 7461 5f73 6572 7669 6365 732e 6461 7461  ta_services.data
+000063d0: 5f73 6f75 7263 652e 6c77 6470 2e73 7475  _source.lwdp.stu
+000063e0: 625f 6275 696c 6465 7220 696d 706f 7274  b_builder import
+000063f0: 2068 7474 705f 6d65 7373 6167 655f 7374   http_message_st
+00006400: 7562 5f62 7569 6c64 6572 0a20 2020 2020  ub_builder.     
+00006410: 2020 200a 2020 2020 2020 2020 6661 6b65     .        fake
+00006420: 5f64 6174 6120 3d20 5b0a 2020 2020 2020  _data = [.      
+00006430: 2020 2020 2020 6874 7470 5f6d 6573 7361        http_messa
+00006440: 6765 5f73 7475 625f 6275 696c 6465 722e  ge_stub_builder.
+00006450: 6275 696c 6428 7b22 6d65 7373 6167 6549  build({"messageI
+00006460: 6422 3a20 2261 222c 2022 6d65 7373 6167  d": "a", "messag
+00006470: 6554 7970 6522 3a20 2252 6f6f 7422 7d29  eType": "Root"})
+00006480: 2c0a 2020 2020 2020 2020 2020 2020 6874  ,.            ht
+00006490: 7470 5f6d 6573 7361 6765 5f73 7475 625f  tp_message_stub_
+000064a0: 6275 696c 6465 722e 6275 696c 6428 7b22  builder.build({"
+000064b0: 6d65 7373 6167 6549 6422 3a20 2262 222c  messageId": "b",
+000064c0: 2022 6d65 7373 6167 6554 7970 6522 3a20   "messageType": 
+000064d0: 224e 6577 227d 292c 0a20 2020 2020 2020  "New"}),.       
+000064e0: 2020 2020 2068 7474 705f 6d65 7373 6167       http_messag
+000064f0: 655f 7374 7562 5f62 7569 6c64 6572 2e62  e_stub_builder.b
+00006500: 7569 6c64 287b 226d 6573 7361 6765 4964  uild({"messageId
+00006510: 223a 2022 6322 2c20 226d 6573 7361 6765  ": "c", "message
+00006520: 5479 7065 223a 2022 416d 656e 6422 7d29  Type": "Amend"})
+00006530: 2c0a 2020 2020 2020 2020 2020 2020 6874  ,.            ht
+00006540: 7470 5f6d 6573 7361 6765 5f73 7475 625f  tp_message_stub_
+00006550: 6275 696c 6465 722e 6275 696c 6428 7b22  builder.build({"
+00006560: 6d65 7373 6167 6549 6422 3a20 2264 222c  messageId": "d",
+00006570: 2022 6d65 7373 6167 6554 7970 6522 3a20   "messageType": 
+00006580: 2243 616e 6365 6c22 7d29 2c0a 2020 2020  "Cancel"}),.    
+00006590: 2020 2020 5d0a 2020 2020 2020 2020 6661      ].        fa
+000065a0: 6b65 5f64 6174 615f 6f62 6a20 3d20 4461  ke_data_obj = Da
+000065b0: 7461 2866 616b 655f 6461 7461 290a 2020  ta(fake_data).  
+000065c0: 2020 2020 2020 0a20 2020 2020 2020 2066        .        f
+000065d0: 6f72 206d 2069 6e20 6661 6b65 5f64 6174  or m in fake_dat
+000065e0: 615f 6f62 6a3a 0a20 2020 2020 2020 2020  a_obj:.         
+000065f0: 2020 206f 5f2e 6d66 722e 6578 7061 6e64     o_.mfr.expand
+00006600: 5f6d 6573 7361 6765 286d 2920 2023 206d  _message(m)  # m
+00006610: 6672 202d 2073 7461 6e64 7320 666f 7220  fr - stands for 
+00006620: 4d65 7373 6167 6546 6965 6c64 5265 736f  MessageFieldReso
+00006630: 6c76 6572 0a20 2020 2020 2020 2023 206f  lver.        # o
+00006640: 720a 2020 2020 2020 2020 666f 7220 6d20  r.        for m 
+00006650: 696e 2066 616b 655f 6461 7461 5f6f 626a  in fake_data_obj
+00006660: 2e6d 6170 286f 5f2e 6d66 722e 6578 7061  .map(o_.mfr.expa
+00006670: 6e64 5f6d 6573 7361 6765 293a 0a20 2020  nd_message):.   
+00006680: 2020 2020 2020 2020 2070 6173 730a 2020           pass.  
+00006690: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+000066a0: 205b 342e 325d 204c 6962 7261 7269 6573   [4.2] Libraries
+000066b0: 2075 7361 6765 2e0a 2020 2020 2020 2020   usage..        
+000066c0: 2320 446f 6e27 7420 696d 706f 7274 2065  # Don't import e
+000066d0: 7861 6374 2072 6573 6f6c 7665 7273 2069  xact resolvers i
+000066e0: 6d70 6c65 6d65 6e74 6174 696f 6e20 696e  mplementation in
+000066f0: 2079 6f75 7220 636f 6465 2c20 706c 6561   your code, plea
+00006700: 7365 2e0a 2020 2020 2020 2020 2320 416c  se..        # Al
+00006710: 6c6f 7720 796f 7572 2063 6c69 656e 7420  low your client 
+00006720: 746f 2064 6f20 6974 2069 6e73 7465 6164  to do it instead
+00006730: 2e0a 2020 2020 2020 2020 2320 4a75 7374  ..        # Just
+00006740: 2069 6d70 6f72 7420 606f 7074 696f 6e73   import `options
+00006750: 6020 6672 6f6d 2060 7468 325f 6461 7461  ` from `th2_data
+00006760: 5f73 6572 7669 6365 732e 636f 6e66 6967  _services.config
+00006770: 6020 616e 6420 7573 6520 6974 2e0a 2020  ` and use it..  
+00006780: 2020 2020 2020 6672 6f6d 2074 6832 5f64        from th2_d
+00006790: 6174 615f 7365 7276 6963 6573 2e63 6f6e  ata_services.con
+000067a0: 6669 6720 696d 706f 7274 206f 7074 696f  fig import optio
+000067b0: 6e73 2061 7320 6f5f 0a20 2020 2020 2020  ns as o_.       
+000067c0: 200a 2020 2020 2020 2020 666f 7220 6d20   .        for m 
+000067d0: 696e 2066 616b 655f 6461 7461 5f6f 626a  in fake_data_obj
+000067e0: 3a0a 2020 2020 2020 2020 2020 2020 6f5f  :.            o_
+000067f0: 2e6d 6672 2e65 7870 616e 645f 6d65 7373  .mfr.expand_mess
+00006800: 6167 6528 6d29 0a20 2020 2020 2020 2023  age(m).        #
+00006810: 206f 720a 2020 2020 2020 2020 666f 7220   or.        for 
+00006820: 6d20 696e 2066 616b 655f 6461 7461 5f6f  m in fake_data_o
+00006830: 626a 2e6d 6170 286f 5f2e 6d66 722e 6578  bj.map(o_.mfr.ex
+00006840: 7061 6e64 5f6d 6573 7361 6765 293a 0a20  pand_message):. 
+00006850: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
 00006860: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00006870: 2049 6e20 636f 6e74 7261 7374 2074 6f20   In contrast to 
-00006880: 636f 6c6c 6563 7469 6f6e 732c 2077 6869  collections, whi
-00006890: 6368 2061 7265 2069 7465 7261 7465 6420  ch are iterated 
-000068a0: 6578 706c 6963 6974 6c79 2028 6578 7465  explicitly (exte
-000068b0: 726e 616c 2069 7465 7261 7469 6f6e 292c  rnal iteration),
-000068c0: 2073 7472 6561 6d20 6f70 6572 6174 696f   stream operatio
-000068d0: 6e73 2064 6f20 7468 6520 6974 6572 6174  ns do the iterat
-000068e0: 696f 6e0a 2020 2020 2020 2020 6265 6869  ion.        behi
-000068f0: 6e64 2074 6865 2073 6365 6e65 7320 666f  nd the scenes fo
-00006900: 7220 796f 752e 204e 6f74 652c 2069 7420  r you. Note, it 
-00006910: 646f 6573 6e27 7420 6d65 616e 2079 6f75  doesn't mean you
-00006920: 2063 616e 6e6f 7420 6974 6572 6174 6520   cannot iterate 
-00006930: 7468 6520 5f44 6174 6120 6f62 6a65 6374  the _Data object
-00006940: 5f2e 0a20 2020 2020 2020 200a 2020 2020  _..        .    
-00006950: 2020 2020 0a20 2020 2020 2020 2023 2323      .        ###
-00006960: 2044 6174 6120 6974 6572 6174 696f 6e0a   Data iteration.
-00006970: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00006980: 2054 6865 2044 6174 6120 6f62 6a65 6374   The Data object
-00006990: 2063 6f6e 7374 7275 6374 6f72 206d 6574   constructor met
-000069a0: 686f 6420 7461 6b65 7320 696e 2061 7320  hod takes in as 
-000069b0: 6172 6775 6d65 6e74 2065 6974 6865 7220  argument either 
-000069c0: 616e 2069 7465 7261 746f 7220 6f76 6572  an iterator over
-000069d0: 206f 626a 6563 7473 206f 7220 6120 6765   objects or a ge
-000069e0: 6e65 7261 746f 7220 6675 6e63 7469 6f6e  nerator function
-000069f0: 2e0a 2020 2020 2020 2020 5468 6520 4461  ..        The Da
-00006a00: 7461 206f 626a 6563 7420 6974 6572 6174  ta object iterat
-00006a10: 6f72 2068 616e 646c 6573 2065 6163 6820  or handles each 
-00006a20: 6974 656d 2069 6e20 7468 6973 2069 7465  item in this ite
-00006a30: 7261 746f 7220 6f72 2067 656e 6572 6174  rator or generat
-00006a40: 6f72 2061 7320 7468 6579 2061 7265 2c20  or as they are, 
-00006a50: 6d65 616e 696e 6720 6974 2064 6f65 736e  meaning it doesn
-00006a60: 2774 2074 7279 2074 6f20 7265 6164 2074  't try to read t
-00006a70: 6865 2063 6f6e 7465 6e74 206f 6620 6974  he content of it
-00006a80: 656d 206f 7220 7265 7475 726e 2074 6865  em or return the
-00006a90: 6d20 6d6f 6469 6669 6564 2069 6e20 616e  m modified in an
-00006aa0: 7920 7761 792c 2069 6e73 7465 6164 2072  y way, instead r
-00006ab0: 6574 7572 6e73 2074 6865 2069 7465 6d20  eturns the item 
-00006ac0: 6974 7365 6c66 2e0a 2020 2020 2020 2020  itself..        
-00006ad0: 5468 6520 6f6e 6c79 2065 7863 6570 7469  The only excepti
-00006ae0: 6f6e 2074 6f20 7468 6973 2069 7320 7768  on to this is wh
-00006af0: 656e 2044 6174 6120 6f62 6a65 6374 2069  en Data object i
-00006b00: 7320 6275 696c 7420 7573 696e 6720 6974  s built using it
-00006b10: 6572 6174 6f72 206f 7220 6765 6e65 7261  erator or genera
-00006b20: 746f 7220 6f76 6572 206f 7468 6572 2044  tor over other D
-00006b30: 6174 6120 6f62 6a65 6374 732e 204e 6f74  ata objects. Not
-00006b40: 6520 7468 6174 2074 6869 7320 6974 6572  e that this iter
-00006b50: 6174 6f72 206f 7220 6765 6e65 7261 746f  ator or generato
-00006b60: 7220 6d75 7374 206f 6e6c 7920 6265 2079  r must only be y
-00006b70: 6965 6c64 696e 6720 4461 7461 206f 626a  ielding Data obj
-00006b80: 6563 7473 2061 6e64 206e 6f74 6869 6e67  ects and nothing
-00006b90: 2065 6c73 652e 2049 6620 7765 2062 7569   else. If we bui
-00006ba0: 6c64 2066 726f 6d20 6120 6d69 7820 6f66  ld from a mix of
-00006bb0: 2044 6174 6120 6f62 6a65 6374 7320 616e   Data objects an
-00006bc0: 6420 736f 6d65 206f 7468 6572 2074 7970  d some other typ
-00006bd0: 6573 2c20 4461 7461 206f 626a 6563 7473  es, Data objects
-00006be0: 2720 636f 6e74 656e 7420 776f 6e27 7420  ' content won't 
-00006bf0: 6265 2072 6561 6420 616e 6420 696e 7374  be read and inst
-00006c00: 6561 6420 6974 2077 696c 6c20 6265 2072  ead it will be r
-00006c10: 6574 7572 6e65 6420 6173 2044 6174 6120  eturned as Data 
-00006c20: 6f62 6a65 6374 2069 7473 656c 662e 0a20  object itself.. 
-00006c30: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006c40: 536d 616c 6c20 6578 616d 706c 6520 746f  Small example to
-00006c50: 2064 656d 6f6e 7374 7261 7465 3a0a 2020   demonstrate:.  
-00006c60: 2020 2020 2020 0a20 2020 2020 2020 2060        .        `
-00006c70: 6060 7079 7468 6f6e 0a20 2020 2020 2020  ``python.       
-00006c80: 2066 726f 6d20 7468 325f 6461 7461 5f73   from th2_data_s
-00006c90: 6572 7669 6365 732e 6461 7461 2069 6d70  ervices.data imp
-00006ca0: 6f72 7420 4461 7461 0a20 2020 2020 2020  ort Data.       
-00006cb0: 200a 2020 2020 2020 2020 6431 203d 2044   .        d1 = D
-00006cc0: 6174 6128 5b31 2c32 2c33 5d29 0a20 2020  ata([1,2,3]).   
-00006cd0: 2020 2020 2064 3220 3d20 4461 7461 285b       d2 = Data([
-00006ce0: 342c 352c 365d 290a 2020 2020 2020 2020  4,5,6]).        
-00006cf0: 0a20 2020 2020 2020 206f 6e6c 795f 6461  .        only_da
-00006d00: 7461 5f6f 626a 6563 7473 203d 2044 6174  ta_objects = Dat
-00006d10: 6128 5b64 312c 6432 5d29 2023 2057 696c  a([d1,d2]) # Wil
-00006d20: 6c20 6974 6572 6174 6520 6173 2031 2c32  l iterate as 1,2
-00006d30: 2c33 2c34 2c35 2c36 0a20 2020 2020 2020  ,3,4,5,6.       
-00006d40: 2064 6174 615f 616e 645f 6c69 7374 203d   data_and_list =
-00006d50: 2044 6174 6128 5b64 312c 5b34 2c35 2c36   Data([d1,[4,5,6
-00006d60: 5d5d 2920 2320 5769 6c6c 2069 7465 7261  ]]) # Will itera
-00006d70: 7465 2061 7320 6431 2c20 5b34 2c35 2c36  te as d1, [4,5,6
-00006d80: 5d0a 2020 2020 2020 2020 6461 7461 5f61  ].        data_a
-00006d90: 6e64 5f6e 756d 6265 7273 203d 2044 6174  nd_numbers = Dat
-00006da0: 6128 5b64 312c 342c 352c 365d 2920 2320  a([d1,4,5,6]) # 
-00006db0: 5769 6c6c 2069 7465 7261 7465 2061 7320  Will iterate as 
-00006dc0: 6431 2c34 2c35 2c36 0a20 2020 2020 2020  d1,4,5,6.       
-00006dd0: 206c 6973 7473 5f6f 6e6c 7920 3d20 4461   lists_only = Da
-00006de0: 7461 285b 312c 322c 335d 2c5b 342c 352c  ta([1,2,3],[4,5,
-00006df0: 365d 2920 2320 5769 6c6c 2069 7465 7261  6]) # Will itera
-00006e00: 7465 2061 7320 5b31 2c32 2c33 5d2c 5b34  te as [1,2,3],[4
-00006e10: 2c35 2c36 5d0a 2020 2020 2020 2020 0a20  ,5,6].        . 
-00006e20: 2020 2020 2020 2023 2049 6620 7765 2077         # If we w
-00006e30: 616e 7420 746f 2069 7465 7261 7465 206f  ant to iterate o
-00006e40: 7665 7220 636f 6e74 656e 7420 6f66 206c  ver content of l
-00006e50: 6973 7420 6f66 206c 6973 7473 2c20 7765  ist of lists, we
-00006e60: 2073 686f 756c 6420 6669 7273 7420 6372   should first cr
-00006e70: 6561 7465 2044 6174 6120 6f62 6a65 6374  eate Data object
-00006e80: 7320 6672 6f6d 2074 6865 6d2c 0a20 2020  s from them,.   
-00006e90: 2020 2020 2023 2074 6865 6e20 7573 6520       # then use 
-00006ea0: 7468 656d 2074 6f20 636f 6e73 7472 7563  them to construc
-00006eb0: 7420 6e65 7720 4461 7461 206f 626a 6563  t new Data objec
-00006ec0: 7420 6173 2069 6e20 6361 7365 206f 6620  t as in case of 
-00006ed0: 6431 2061 6e64 2064 322c 2063 7265 6174  d1 and d2, creat
-00006ee0: 696e 6720 276f 6e6c 795f 6461 7461 5f6f  ing 'only_data_o
-00006ef0: 626a 6563 7473 2720 696e 2074 6869 7320  bjects' in this 
-00006f00: 6578 616d 706c 652e 0a20 2020 2020 2020  example..       
-00006f10: 2060 6060 0a20 2020 2020 2020 2020 0a20   ```.         . 
-00006f20: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006f30: 2323 2320 4461 7461 2063 6163 6869 6e67  ### Data caching
-00006f40: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00006f50: 2020 5468 6520 5f44 6174 6120 6f62 6a65    The _Data obje
-00006f60: 6374 5f20 7072 6f76 6964 6573 2074 6865  ct_ provides the
-00006f70: 2061 6269 6c69 7479 2074 6f20 7573 6520   ability to use 
-00006f80: 7468 6520 6361 6368 652e 2054 6865 2063  the cache. The c
-00006f90: 6163 6865 2077 6f72 6b73 2066 6f72 2065  ache works for e
-00006fa0: 6163 6820 5f44 6174 6120 6f62 6a65 6374  ach _Data object
-00006fb0: 5f2c 2074 6861 7420 6973 2c20 796f 7520  _, that is, you 
-00006fc0: 6368 6f6f 7365 0a20 2020 2020 2020 2077  choose.        w
-00006fd0: 6869 6368 205f 4461 7461 206f 626a 6563  hich _Data objec
-00006fe0: 745f 2079 6f75 2077 616e 7420 746f 2073  t_ you want to s
-00006ff0: 6176 652e 2054 6865 205f 4461 7461 206f  ave. The _Data o
-00007000: 626a 6563 745f 2063 6163 6865 2069 7320  bject_ cache is 
-00007010: 7361 7665 6420 6166 7465 7220 7468 6520  saved after the 
-00007020: 6669 7273 7420 6974 6572 6174 696f 6e2c  first iteration,
-00007030: 2062 7574 2074 6865 2069 7465 7261 7469   but the iterati
-00007040: 6f6e 0a20 2020 2020 2020 2073 6f75 7263  on.        sourc
-00007050: 6520 6d61 7920 6265 2064 6966 6665 7265  e may be differe
-00007060: 6e74 2e0a 2020 2020 2020 2020 0a20 2020  nt..        .   
-00007070: 2020 2020 2049 6620 796f 7520 646f 6e27       If you don'
-00007080: 7420 7573 6520 7468 6520 6361 6368 652c  t use the cache,
-00007090: 2079 6f75 7220 736f 7572 6365 2077 696c   your source wil
-000070a0: 6c20 6265 2074 6865 2064 6174 6120 736f  l be the data so
-000070b0: 7572 6365 2079 6f75 2068 6176 6520 696e  urce you have in
-000070c0: 2074 6865 205f 4461 7461 204f 626a 6563   the _Data Objec
-000070d0: 745f 2e20 4275 7420 6966 2079 6f75 2075  t_. But if you u
-000070e0: 7365 2074 6865 2063 6163 6865 2c0a 2020  se the cache,.  
-000070f0: 2020 2020 2020 796f 7572 2073 6f75 7263        your sourc
-00007100: 6520 6361 6e20 6265 2074 6865 2064 6174  e can be the dat
-00007110: 6120 736f 7572 6365 2c20 7468 6520 7061  a source, the pa
-00007120: 7265 6e74 2063 6163 6865 2c20 6f72 206f  rent cache, or o
-00007130: 776e 2063 6163 6865 3a0a 2020 2020 2020  wn cache:.      
-00007140: 2020 0a20 2020 2020 2020 202a 2054 6865    .        * The
-00007150: 2064 6174 6120 736f 7572 6365 3a0a 2020   data source:.  
-00007160: 2020 2020 2020 2020 4966 2074 6865 205f          If the _
-00007170: 4461 7461 204f 626a 6563 745f 2064 6f65  Data Object_ doe
-00007180: 736e 2774 2068 6176 6520 6120 7061 7265  sn't have a pare
-00007190: 6e74 2063 6163 6865 2061 6e64 2069 7473  nt cache and its
-000071a0: 2063 6163 6865 2e0a 2020 2020 2020 2020   cache..        
-000071b0: 2a20 5468 6520 7061 7265 6e74 2063 6163  * The parent cac
-000071c0: 6865 3a0a 2020 2020 2020 2020 2020 4966  he:.          If
-000071d0: 2074 6865 205f 4461 7461 204f 626a 6563   the _Data Objec
-000071e0: 745f 2068 6173 2061 2070 6172 656e 7420  t_ has a parent 
-000071f0: 6361 6368 652e 2049 7420 646f 6573 6e27  cache. It doesn'
-00007200: 7420 6d61 7474 6572 2077 6861 7420 706f  t matter what po
-00007210: 7369 7469 6f6e 2074 6865 2070 6172 656e  sition the paren
-00007220: 7420 6361 6368 6520 6861 7320 696e 2069  t cache has in i
-00007230: 6e68 6572 6974 616e 6365 2e0a 2020 2020  nheritance..    
-00007240: 2020 2020 2020 5f44 6174 6120 4f62 6a65        _Data Obje
-00007250: 6374 5f20 756e 6465 7273 7461 6e64 7320  ct_ understands 
-00007260: 7768 6f73 6520 6361 6368 6520 6974 2069  whose cache it i
-00007270: 7320 616e 6420 6578 6563 7574 6573 2074  s and executes t
-00007280: 6865 2070 6172 7420 6f66 2074 6865 2077  he part of the w
-00007290: 6f72 6b66 6c6f 7720 7468 6174 2077 6173  orkflow that was
-000072a0: 206e 6f74 2065 7865 6375 7465 642e 0a20   not executed.. 
-000072b0: 2020 2020 2020 202a 2054 6865 206f 776e         * The own
-000072c0: 2063 6163 6865 3a0a 2020 2020 2020 2020   cache:.        
-000072d0: 2020 4966 2069 7420 6973 206e 6f74 2074    If it is not t
-000072e0: 6865 2066 6972 7374 2069 7465 7261 7469  he first iterati
-000072f0: 6f6e 206f 6620 7468 6973 2044 6174 6120  on of this Data 
-00007300: 6f62 6a65 6374 2e0a 2020 2020 2020 2020  object..        
-00007310: 0a20 2020 2020 2020 204e 6f74 6520 7468  .        Note th
-00007320: 6174 2074 6865 2063 6163 6865 2073 7461  at the cache sta
-00007330: 7465 206f 6620 7468 6520 4461 7461 206f  te of the Data o
-00007340: 626a 6563 7420 6973 206e 6f74 2069 6e68  bject is not inh
-00007350: 6572 6974 6564 2e0a 2020 2020 2020 2020  erited..        
-00007360: 0a20 2020 2020 2020 2023 2323 2320 466f  .        #### Fo
-00007370: 7263 6564 2063 6163 6869 6e67 0a20 2020  rced caching.   
-00007380: 2020 2020 2059 6f75 2063 616e 2074 656c       You can tel
-00007390: 6c20 4453 2074 6f20 6361 6368 6520 6461  l DS to cache da
-000073a0: 7461 2074 6f20 7370 6563 6966 6963 2063  ta to specific c
-000073b0: 6163 6865 2066 696c 652c 2077 6869 6368  ache file, which
-000073c0: 2077 6f6e 2774 2062 6520 6465 6c65 7465   won't be delete
-000073d0: 6420 6166 7465 7220 7363 7269 7074 2065  d after script e
-000073e0: 6e64 2e0a 2020 2020 2020 2020 596f 7520  nd..        You 
-000073f0: 6361 6e20 7365 6520 6578 616d 706c 6520  can see example 
-00007400: 696e 2031 2e31 3220 7365 6374 696f 6e20  in 1.12 section 
-00007410: 6f66 205b 6765 745f 7374 6172 7465 645f  of [get_started_
-00007420: 6578 616d 706c 655d 2865 7861 6d70 6c65  example](example
-00007430: 732f 6765 745f 7374 6172 7465 645f 6578  s/get_started_ex
-00007440: 616d 706c 652e 7079 292e 0a20 2020 2020  ample.py)..     
-00007450: 2020 200a 2020 2020 2020 2020 0a20 2020     .        .   
-00007460: 2020 2020 2023 2323 2045 7665 6e74 5472       ### EventTr
-00007470: 6565 2061 6e64 2063 6f6c 6c65 6374 696f  ee and collectio
-00007480: 6e73 0a20 2020 2020 2020 200a 2020 2020  ns.        .    
-00007490: 2020 2020 2323 2323 2045 7665 6e74 5472      #### EventTr
-000074a0: 6565 0a20 2020 2020 2020 200a 2020 2020  ee.        .    
-000074b0: 2020 2020 6045 7665 6e74 5472 6565 6020      `EventTree` 
-000074c0: 6973 2061 2074 7265 652d 6261 7365 6420  is a tree-based 
-000074d0: 6461 7461 2073 7472 7563 7475 7265 206f  data structure o
-000074e0: 6620 6576 656e 7473 2e20 4974 2061 6c6c  f events. It all
-000074f0: 6f77 7320 796f 7520 6765 7420 6368 696c  ows you get chil
-00007500: 6472 656e 2061 6e64 2070 6172 656e 7473  dren and parents
-00007510: 206f 6620 6576 656e 742c 0a20 2020 2020   of event,.     
-00007520: 2020 2064 6973 706c 6179 2074 7265 652c     display tree,
-00007530: 2067 6574 2066 756c 6c20 7061 7468 2074   get full path t
-00007540: 6f20 6576 656e 7420 6574 632e 0a20 2020  o event etc..   
-00007550: 2020 2020 200a 2020 2020 2020 2020 4465       .        De
-00007560: 7461 696c 733a 0a20 2020 2020 2020 200a  tails:.        .
-00007570: 2020 2020 2020 2020 2a20 6045 7665 6e74          * `Event
-00007580: 5472 6565 6020 636f 6e74 6169 6e73 2061  Tree` contains a
-00007590: 6c6c 2065 7665 6e74 7320 696e 206d 656d  ll events in mem
-000075a0: 6f72 792e 0a20 2020 2020 2020 202a 2054  ory..        * T
-000075b0: 7265 6520 6861 7320 736f 6d65 2069 6d70  ree has some imp
-000075c0: 6f72 7461 6e74 2074 6572 6d73 3a0a 2020  ortant terms:.  
-000075d0: 2020 2020 2020 2020 2020 312e 205f 416e            1. _An
-000075e0: 6365 7374 6f72 5f20 6973 2061 6e79 2072  cestor_ is any r
-000075f0: 656c 6174 6976 6520 6f66 2074 6865 2065  elative of the e
-00007600: 7665 6e74 2075 7020 7468 6520 7472 6565  vent up the tree
-00007610: 2028 6772 616e 6470 6172 656e 742c 2070   (grandparent, p
-00007620: 6172 656e 7420 6574 632e 292e 0a20 2020  arent etc.)..   
-00007630: 2020 2020 2020 2020 2032 2e20 5f50 6172           2. _Par
-00007640: 656e 745f 2069 7320 6f6e 6c79 2074 6865  ent_ is only the
-00007650: 2066 6972 7374 2072 656c 6174 6976 6520   first relative 
-00007660: 6f66 2074 6865 2065 7665 6e74 2075 7020  of the event up 
-00007670: 7468 6520 7472 6565 2e0a 2020 2020 2020  the tree..      
-00007680: 2020 2020 2020 332e 205f 4368 696c 645f        3. _Child_
-00007690: 2069 7320 7468 6520 6669 7273 7420 7265   is the first re
-000076a0: 6c61 7469 7665 206f 6620 7468 6520 6576  lative of the ev
-000076b0: 656e 7420 646f 776e 2074 6865 2074 7265  ent down the tre
-000076c0: 652e 0a20 2020 2020 2020 200a 2020 2020  e..        .    
-000076d0: 2020 2020 5461 6b65 2061 206c 6f6f 6b20      Take a look 
-000076e0: 6174 2074 6865 2066 6f6c 6c6f 7769 6e67  at the following
-000076f0: 2048 544d 4c20 7472 6565 2074 6f20 756e   HTML tree to un
-00007700: 6465 7273 7461 6e64 2074 6865 6d2e 0a20  derstand them.. 
-00007710: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00007720: 2020 2060 6060 0a20 2020 2020 2020 2020     ```.         
-00007730: 2020 203c 626f 6479 3e20 3c21 2d2d 2061     <body> <!-- a
-00007740: 6e63 6573 746f 7220 2867 7261 6e64 7061  ncestor (grandpa
-00007750: 7265 6e74 292c 2062 7574 206e 6f74 2070  rent), but not p
-00007760: 6172 656e 7420 2d2d 3e0a 2020 2020 2020  arent -->.      
-00007770: 2020 2020 2020 2020 2020 3c64 6976 3e20            <div> 
-00007780: 3c21 2d2d 2070 6172 656e 7420 2620 616e  <!-- parent & an
-00007790: 6365 7374 6f72 202d 2d3e 0a20 2020 2020  cestor -->.     
-000077a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000077b0: 703e 4865 6c6c 6f2c 2077 6f72 6c64 213c  p>Hello, world!<
-000077c0: 2f70 3e20 3c21 2d2d 2063 6869 6c64 202d  /p> <!-- child -
-000077d0: 2d3e 0a20 2020 2020 2020 2020 2020 2020  ->.             
-000077e0: 2020 2020 2020 203c 703e 476f 6f64 6279         <p>Goodby
-000077f0: 6521 3c2f 703e 203c 212d 2d20 7369 626c  e!</p> <!-- sibl
-00007800: 696e 6720 2d2d 3e0a 2020 2020 2020 2020  ing -->.        
-00007810: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00007820: 2020 2020 2020 2020 2020 203c 2f62 6f64             </bod
-00007830: 793e 0a20 2020 2020 2020 2020 2020 6060  y>.           ``
-00007840: 600a 2020 2020 2020 2020 0a20 2020 2020  `.        .     
-00007850: 2020 2023 2323 2320 436f 6c6c 6563 7469     #### Collecti
-00007860: 6f6e 730a 2020 2020 2020 2020 0a20 2020  ons.        .   
-00007870: 2020 2020 202a 2a45 7665 6e74 5472 6565       **EventTree
-00007880: 436f 6c6c 6563 7469 6f6e 2a2a 2069 7320  Collection** is 
-00007890: 6120 636f 6c6c 6563 7469 6f6e 206f 6620  a collection of 
-000078a0: 4576 656e 7454 7265 6573 2e20 5468 6520  EventTrees. The 
-000078b0: 636f 6c6c 6563 7469 6f6e 2062 7569 6c64  collection build
-000078c0: 7320 6120 6665 7720 5f45 7665 6e74 5472  s a few _EventTr
-000078d0: 6565 5f20 6279 2070 6173 7365 6420 5f44  ee_ by passed _D
-000078e0: 6174 610a 2020 2020 2020 2020 6f62 6a65  ata.        obje
-000078f0: 6374 5f2e 2041 6c74 686f 7567 6820 796f  ct_. Although yo
-00007900: 7520 6361 6e20 6368 616e 6765 2074 6865  u can change the
-00007910: 2074 7265 6520 6469 7265 6374 6c79 2c20   tree directly, 
-00007920: 6974 2773 2062 6574 7465 7220 746f 2064  it's better to d
-00007930: 6f20 6974 2074 6872 6f75 6768 2063 6f6c  o it through col
-00007940: 6c65 6374 696f 6e73 2062 6563 6175 7365  lections because
-00007950: 2074 6865 7920 6172 6520 6177 6172 6520   they are aware 
-00007960: 6f66 0a20 2020 2020 2020 2060 6465 7461  of.        `deta
-00007970: 6368 6564 5f65 7665 6e74 7360 2061 6e64  ched_events` and
-00007980: 2063 616e 2073 6f6c 7665 2073 6f6d 6520   can solve some 
-00007990: 6576 656e 7473 2064 6570 656e 6465 6e63  events dependenc
-000079a0: 6965 732e 2054 6865 2063 6f6c 6c65 6374  ies. The collect
-000079b0: 696f 6e20 6861 7320 7369 6d69 6c61 7220  ion has similar 
-000079c0: 6665 6174 7572 6573 206c 696b 6520 6120  features like a 
-000079d0: 7369 6e67 6c65 205f 4576 656e 7454 7265  single _EventTre
-000079e0: 655f 0a20 2020 2020 2020 2062 7574 2061  e_.        but a
-000079f0: 7070 6c79 696e 6720 7468 656d 2066 6f72  pplying them for
-00007a00: 2061 6c6c 205f 4576 656e 7454 7265 6573   all _EventTrees
-00007a10: 5f2e 0a20 2020 2020 2020 200a 2020 2020  _..        .    
-00007a20: 2020 2020 2a2a 5061 7265 6e74 4576 656e      **ParentEven
-00007a30: 7454 7265 6543 6f6c 6c65 6374 696f 6e2a  tTreeCollection*
-00007a40: 2a20 6973 2061 2063 6f6c 6c65 6374 696f  * is a collectio
-00007a50: 6e20 7369 6d69 6c61 7220 746f 205f 4576  n similar to _Ev
-00007a60: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
-00007a70: 6e5f 2062 7574 2063 6f6e 7461 696e 696e  n_ but containin
-00007a80: 6720 6f6e 6c79 2070 6172 656e 7420 6576  g only parent ev
-00007a90: 656e 7473 2074 6861 740a 2020 2020 2020  ents that.      
-00007aa0: 2020 6172 6520 7265 6665 7265 6e63 6564    are referenced
-00007ab0: 2069 6e20 7468 6520 6461 7461 2073 7472   in the data str
-00007ac0: 6561 6d2e 2054 6865 2063 6f6c 6c65 6374  eam. The collect
-00007ad0: 696f 6e20 6861 7320 6665 6174 7572 6573  ion has features
-00007ae0: 2073 696d 696c 6172 2074 6f20 5f45 7665   similar to _Eve
-00007af0: 6e74 5472 6565 436f 6c6c 6563 7469 6f6e  ntTreeCollection
-00007b00: 5f2e 0a20 2020 2020 2020 200a 2020 2020  _..        .    
-00007b10: 2020 2020 4465 7461 696c 733a 0a20 2020      Details:.   
-00007b20: 2020 2020 200a 2020 2020 2020 2020 2a20       .        * 
-00007b30: 546f 2075 7365 2045 5420 636f 6c6c 6563  To use ET collec
-00007b40: 7469 6f6e 7320 796f 7520 6e65 6564 2074  tions you need t
-00007b50: 6f20 696e 6974 6961 6c69 7a65 2074 6865  o initialize the
-00007b60: 6d20 6279 205f 4554 4344 7269 7665 725f  m by _ETCDriver_
-00007b70: 2e20 4461 7461 2073 6f75 7263 6573 2075  . Data sources u
-00007b80: 7375 616c 6c79 2070 726f 7669 6465 2074  sually provide t
-00007b90: 6865 6d2e 0a20 2020 2020 2020 2020 2059  hem..          Y
-00007ba0: 6f75 2063 616e 2063 7265 6174 6520 6974  ou can create it
-00007bb0: 2062 7920 796f 7572 7365 6c66 2064 6570   by yourself dep
-00007bc0: 656e 6469 6e67 206f 6e20 796f 7572 2064  ending on your d
-00007bd0: 6174 6120 7374 7275 6374 7572 652e 0a20  ata structure.. 
-00007be0: 2020 2020 2020 202a 2054 6865 2063 6f6c         * The col
-00007bf0: 6c65 6374 696f 6e20 6861 7320 6120 6665  lection has a fe
-00007c00: 6174 7572 6520 746f 2072 6563 6f76 6572  ature to recover
-00007c10: 2065 7665 6e74 732e 2041 6c6c 2065 7665   events. All eve
-00007c20: 6e74 7320 7468 6174 2061 7265 206e 6f74  nts that are not
-00007c30: 2069 6e20 7468 6520 7265 6365 6976 6564   in the received
-00007c40: 2064 6174 6120 7374 7265 616d 2c20 6275   data stream, bu
-00007c50: 7420 7768 6963 6820 6172 650a 2020 2020  t which are.    
-00007c60: 2020 2020 2020 7265 6665 7265 6e63 6564        referenced
-00007c70: 2077 696c 6c20 6265 206c 6f61 6465 6420   will be loaded 
-00007c80: 6672 6f6d 2074 6865 2064 6174 6120 736f  from the data so
-00007c90: 7572 6365 2e0a 2020 2020 2020 2020 2a20  urce..        * 
-00007ca0: 596f 7520 6361 6e20 7461 6b65 2060 6465  You can take `de
-00007cb0: 7461 6368 6564 5f65 7665 6e74 7360 2074  tached_events` t
-00007cc0: 6f20 7365 6520 7768 6963 6820 6576 656e  o see which even
-00007cd0: 7473 2061 7265 206d 6973 7369 6e67 2e0a  ts are missing..
-00007ce0: 2020 2020 2020 2020 2a20 4966 2079 6f75          * If you
-00007cf0: 2077 616e 742c 2079 6f75 2063 616e 2062   want, you can b
-00007d00: 7569 6c64 2070 6172 656e 746c 6573 7320  uild parentless 
-00007d10: 7472 6565 7320 7768 6572 6520 7468 6520  trees where the 
-00007d20: 6d69 7373 696e 6720 6576 656e 7473 2061  missing events a
-00007d30: 7265 2073 7475 6262 6564 2069 6e73 7465  re stubbed inste
-00007d40: 6164 2e20 4a75 7374 0a20 2020 2020 2020  ad. Just.       
-00007d50: 2020 2075 7365 2060 6765 745f 7061 7265     use `get_pare
-00007d60: 6e74 6c65 7373 5f74 7265 6573 2829 602e  ntless_trees()`.
-00007d70: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00007d80: 2020 5265 7175 6972 656d 656e 7473 3a0a    Requirements:.
-00007d90: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00007da0: 2031 2e20 4576 656e 7473 2070 726f 7669   1. Events provi
-00007db0: 6465 6420 746f 2045 5443 2068 6176 6520  ded to ETC have 
-00007dc0: 746f 2068 6176 6520 6065 7665 6e74 5f6e  to have `event_n
-00007dd0: 616d 6560 2c20 6065 7665 6e74 5f69 6460  ame`, `event_id`
-00007de0: 2c20 6070 6172 656e 745f 6576 656e 745f  , `parent_event_
-00007df0: 6964 6020 6669 656c 6473 2e20 5468 6579  id` fields. They
-00007e00: 0a20 2020 2020 2020 2063 616e 2068 6176  .        can hav
-00007e10: 6520 616e 6f74 6865 7220 6e61 6d65 7320  e another names 
-00007e20: 2869 7420 7265 736f 6c76 6573 2069 6e20  (it resolves in 
-00007e30: 7468 6520 6472 6976 6572 292e 0a20 2020  the driver)..   
-00007e40: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-00007e50: 2323 2048 696e 7473 0a20 2020 2020 2020  ## Hints.       
-00007e60: 200a 2020 2020 2020 2020 2a20 5265 6d6f   .        * Remo
-00007e70: 7665 2061 6c6c 2075 6e6e 6563 6573 7361  ve all unnecessa
-00007e80: 7279 2066 6965 6c64 7320 6672 6f6d 2065  ry fields from e
-00007e90: 7665 6e74 7320 6265 666f 7265 2070 6173  vents before pas
-00007ea0: 7369 6e67 2074 6f20 6120 5f63 6f6c 6c65  sing to a _colle
-00007eb0: 6374 696f 6e5f 2074 6f20 7265 6475 6365  ction_ to reduce
-00007ec0: 206d 656d 6f72 7920 7573 6167 652e 0a20   memory usage.. 
-00007ed0: 2020 2020 2020 202a 2055 7365 2060 7368         * Use `sh
-00007ee0: 6f77 2829 6020 6d65 7468 6f64 2074 6f20  ow()` method to 
-00007ef0: 7072 696e 7420 7468 6520 7472 6565 2069  print the tree i
-00007f00: 6e20 7472 6565 2d6c 696b 6520 7669 6577  n tree-like view
-00007f10: 2e0a 2020 2020 2020 2020 2a20 4e6f 7465  ..        * Note
-00007f20: 2074 6861 7420 7468 6520 6067 6574 5f78   that the `get_x
-00007f30: 6020 6d65 7468 6f64 7320 7769 6c6c 2072  ` methods will r
-00007f40: 6169 7365 2061 6e20 6578 6365 7074 696f  aise an exceptio
-00007f50: 6e20 6966 2079 6f75 2070 6173 7320 616e  n if you pass an
-00007f60: 2075 6e6b 6e6f 776e 2065 7665 6e74 2069   unknown event i
-00007f70: 642c 2075 6e6c 696b 6520 7468 6520 6066  d, unlike the `f
-00007f80: 696e 645f 7860 206d 6574 686f 6473 2028  ind_x` methods (
-00007f90: 0a20 2020 2020 2020 2020 2074 6865 7920  .          they 
-00007fa0: 7265 7475 726e 204e 6f6e 6529 2e0a 2020  return None)..  
-00007fb0: 2020 2020 2020 2a20 4966 2079 6f75 2077        * If you w
-00007fc0: 616e 7420 746f 206b 6e6f 7720 7468 6174  ant to know that
-00007fd0: 2073 7065 6369 6669 6564 2065 7665 6e74   specified event
-00007fe0: 2065 7869 7374 732c 2075 7365 2074 6865   exists, use the
-00007ff0: 2070 7974 686f 6e20 6069 6e60 206b 6579   python `in` key
-00008000: 776f 7264 2028 652e 672e 2060 2765 7665  word (e.g. `'eve
-00008010: 6e74 2d69 6427 2069 6e20 6576 656e 7473  nt-id' in events
-00008020: 5f74 7265 6560 292e 0a20 2020 2020 2020  _tree`)..       
-00008030: 202a 2055 7365 2074 6865 2070 7974 686f   * Use the pytho
-00008040: 6e20 606c 656e 6020 6b65 7977 6f72 6420  n `len` keyword 
-00008050: 746f 2067 6574 2065 7665 6e74 7320 6e75  to get events nu
-00008060: 6d62 6572 2069 6e20 7468 6520 7472 6565  mber in the tree
-00008070: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00008080: 2020 2023 2323 2046 6965 6c64 2052 6573     ### Field Res
-00008090: 6f6c 7665 7273 0a20 2020 2020 2020 2049  olvers.        I
-000080a0: 6e74 6572 6661 6365 2063 616e 2062 6520  nterface can be 
-000080b0: 666f 756e 6420 696e 2060 7468 325f 6461  found in `th2_da
-000080c0: 7461 5f73 6572 7669 6365 732f 696e 7465  ta_services/inte
-000080d0: 7266 6163 6573 2f75 7469 6c73 2f72 6573  rfaces/utils/res
-000080e0: 6f6c 7665 722e 7079 602e 2020 0a20 2020  olver.py`.  .   
-000080f0: 2020 2020 2041 6c6c 2064 6174 612d 736f       All data-so
-00008100: 7572 6365 7320 7368 6f75 6c64 2069 6d70  urces should imp
-00008110: 6c65 6d65 6e74 2074 6865 6d2e 0a20 2020  lement them..   
-00008120: 2020 2020 200a 2020 2020 2020 2020 5468       .        Th
-00008130: 6520 6964 6561 206f 6620 7573 696e 6720  e idea of using 
-00008140: 7265 736f 6c76 6572 733a 0a20 2020 2020  resolvers:.     
-00008150: 2020 2049 7420 736f 6c76 6573 2074 6865     It solves the
-00008160: 2070 726f 626c 656d 206f 6620 6861 7669   problem of havi
-00008170: 6e67 2061 2066 6577 2044 6174 6153 6f75  ng a few DataSou
-00008180: 7263 6573 2077 6974 6820 7369 6d69 6c61  rces with simila
-00008190: 7220 6461 7461 2c0a 2020 2020 2020 2020  r data,.        
-000081a0: 6275 7420 7769 7468 2064 6966 6665 7265  but with differe
-000081b0: 6e74 2077 6179 7320 746f 2067 6574 2069  nt ways to get i
-000081c0: 742e 0a20 2020 2020 2020 200a 2020 2020  t..        .    
-000081d0: 2020 2020 5468 6573 6520 636c 6173 7365      These classe
-000081e0: 7320 7072 6f76 6964 6520 796f 7520 6765  s provide you ge
-000081f0: 7474 6572 206d 6574 686f 6473 2e0a 2020  tter methods..  
-00008200: 2020 2020 2020 5573 696e 6720 7468 6573        Using thes
-00008210: 6520 636c 6173 7365 7320 616c 6c6f 7773  e classes allows
-00008220: 2079 6f75 2074 6f20 6672 6565 6c79 2073   you to freely s
-00008230: 7769 7463 6820 6265 7477 6565 6e20 6469  witch between di
-00008240: 6666 6572 656e 7420 6461 7461 0a20 2020  fferent data.   
-00008250: 2020 2020 2066 6f72 6d61 7473 2061 6e64       formats and
-00008260: 2064 6f6e 2774 2063 6861 6e67 6520 796f   don't change yo
-00008270: 7572 2063 6f64 652e 0a20 2020 2020 2020  ur code..       
-00008280: 200a 2020 2020 2020 2020 5265 736f 6c76   .        Resolv
-00008290: 6572 7320 736f 6c76 6520 7468 6520 7072  ers solve the pr
-000082a0: 6f62 6c65 6d20 6f66 2064 6174 612d 666f  oblem of data-fo
-000082b0: 726d 6174 206d 6967 7261 7469 6f6e 2e0a  rmat migration..
-000082c0: 2020 2020 2020 2020 2d20 6669 656c 6473          - fields
-000082d0: 2070 6c61 6365 2063 616e 2062 6520 6368   place can be ch
-000082e0: 616e 6765 640a 2020 2020 2020 2020 2d20  anged.        - 
-000082f0: 6669 656c 6473 206e 616d 6573 2063 616e  fields names can
-00008300: 2062 6520 6368 616e 6765 640a 2020 2020   be changed.    
-00008310: 2020 2020 0a20 2020 2020 2020 2052 6573      .        Res
-00008320: 6f6c 7665 7273 2063 616e 2077 6f72 6b20  olvers can work 
-00008330: 6f6e 6c79 2077 6974 6820 6f6e 6520 6576  only with one ev
-00008340: 656e 742f 6d65 7373 6167 652e 0a20 2020  ent/message..   
-00008350: 2020 2020 2049 7420 6d65 616e 732c 2069       It means, i
-00008360: 6620 796f 7572 206d 6573 7361 6765 2068  f your message h
-00008370: 6173 2073 7562 2d6d 6573 7361 6765 7320  as sub-messages 
-00008380: 286c 696b 6520 7468 322d 6d65 7373 6167  (like th2-messag
-00008390: 6573 2069 6e20 6c77 6470 2920 6974 200a  es in lwdp) it .
-000083a0: 2020 2020 2020 2020 776f 6e27 7420 776f          won't wo
-000083b0: 726b 2c20 6265 6361 7573 6520 7265 736f  rk, because reso
-000083c0: 6c76 6572 2077 696c 6c20 6e6f 7420 6b6e  lver will not kn
-000083d0: 6f77 2077 6974 6820 7768 6963 6820 7375  ow with which su
-000083e0: 622d 6d65 7373 6167 6520 7368 6f75 6c64  b-message should
-000083f0: 2069 7420 776f 726b 2e20 0a20 2020 2020   it work. .     
-00008400: 2020 200a 2020 2020 2020 2020 2a2a 576f     .        **Wo
-00008410: 726b 6172 6f75 6e64 2a2a 2020 0a20 2020  rkaround**  .   
-00008420: 2020 2020 2031 2e20 4578 7061 6e64 2061       1. Expand a
-00008430: 6c6c 2079 6f75 7220 6d65 7373 6167 6573  ll your messages
-00008440: 202d 3e20 606e 6577 5f64 203d 2079 6f75   -> `new_d = you
-00008450: 725f 6461 7461 2e6d 6170 284d 6573 7361  r_data.map(Messa
-00008460: 6765 4669 656c 6452 6573 6f6c 7665 722e  geFieldResolver.
-00008470: 6578 7061 6e64 5f6d 6573 7361 6765 2960  expand_message)`
-00008480: 0a20 2020 2020 2020 2032 2e20 5573 6520  .        2. Use 
-00008490: 6045 7870 616e 6465 644d 6573 7361 6765  `ExpandedMessage
-000084a0: 4669 656c 6452 6573 6f6c 7665 7260 2069  FieldResolver` i
-000084b0: 6e73 7465 6164 206f 6620 7573 7561 6c20  nstead of usual 
-000084c0: 604d 6573 7361 6765 4669 656c 6452 6573  `MessageFieldRes
-000084d0: 6f6c 7665 7260 2077 6865 6e20 0a20 2020  olver` when .   
-000084e0: 2020 2020 2020 2020 2079 6f75 2074 616b           you tak
-000084f0: 6520 6669 656c 6473 2066 6f72 2065 7870  e fields for exp
-00008500: 616e 6465 6420 6d65 7373 6167 6573 2e0a  anded messages..
-00008510: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00008520: 202a 2a49 6d70 6c65 6d65 6e74 6174 696f   **Implementatio
-00008530: 6e20 6164 7669 6365 3a2a 2a0a 2020 2020  n advice:**.    
-00008540: 2020 2020 312e 2072 6169 7365 204e 6f74      1. raise Not
-00008550: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
-00008560: 202d 2d20 6966 2079 6f75 7220 496d 706c   -- if your Impl
-00008570: 656d 656e 7461 7469 6f6e 2064 6f65 736e  ementation doesn
-00008580: 2774 2073 7570 706f 7274 2074 6869 7320  't support this 
-00008590: 6765 7474 6572 2e0a 2020 2020 2020 2020  getter..        
-000085a0: 0a20 2020 2020 2020 202a 2a50 6572 666f  .        **Perfo
-000085b0: 726d 616e 6365 2069 6d70 6163 743a 2a2a  rmance impact:**
-000085c0: 0a20 2020 2020 2020 202d 2049 7420 6120  .        - It a 
-000085d0: 6269 7420 736c 6f77 6572 2074 6861 6e20  bit slower than 
-000085e0: 7573 696e 6720 6e61 6b65 6420 6669 656c  using naked fiel
-000085f0: 6420 6163 6365 7373 2060 6469 6374 5b27  d access `dict['
-00008600: 6b65 7927 5d60 2e0a 2020 2020 2020 2020  key']`..        
-00008610: 0a20 2020 2020 2020 2023 2320 322e 342e  .        ## 2.4.
-00008620: 204c 696e 6b73 0a20 2020 2020 2020 200a   Links.        .
-00008630: 2020 2020 2020 2020 2d20 5b52 6570 6f72          - [Repor
-00008640: 7420 4461 7461 2050 726f 7669 6465 725d  t Data Provider]
-00008650: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00008660: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
-00008670: 7270 742d 6461 7461 2d70 726f 7669 6465  rpt-data-provide
-00008680: 7229 0a20 2020 2020 2020 202d 205b 5468  r).        - [Th
-00008690: 3220 4461 7461 2053 6572 7669 6365 7320  2 Data Services 
-000086a0: 5574 696c 735d 2868 7474 7073 3a2f 2f67  Utils](https://g
-000086b0: 6974 6875 622e 636f 6d2f 7468 322d 6e65  ithub.com/th2-ne
-000086c0: 742f 7468 322d 6461 7461 2d73 6572 7669  t/th2-data-servi
-000086d0: 6365 732d 7574 696c 7329 0a20 2020 2020  ces-utils).     
-000086e0: 2020 200a 2020 2020 2020 2020 2320 332e     .        # 3.
-000086f0: 2042 6573 7420 7072 6163 7469 6365 730a   Best practices.
-00008700: 2020 2020 2020 2020 4465 7065 6e64 696e          Dependin
-00008710: 6720 6f6e 2068 6f77 2079 6f75 2077 6f72  g on how you wor
-00008720: 6b20 7769 7468 2060 4461 7461 206f 626a  k with `Data obj
-00008730: 6563 7460 2c20 6974 2063 616e 2062 6520  ect`, it can be 
-00008740: 736c 6f77 206f 6620 6661 7374 2e0a 2020  slow of fast..  
-00008750: 2020 2020 2020 4173 2077 6974 6820 6120        As with a 
-00008760: 7265 6c61 7469 6f6e 616c 2064 6174 6162  relational datab
-00008770: 6173 652c 2079 6f75 2063 616e 2077 7269  ase, you can wri
-00008780: 7465 2061 2071 7565 7279 2074 6861 7420  te a query that 
-00008790: 7769 6c6c 2072 6574 7572 6e20 6461 7461  will return data
-000087a0: 2073 6c6f 776c 7920 6f72 2071 7569 636b   slowly or quick
-000087b0: 6c79 2c0a 2020 2020 2020 2020 7468 6520  ly,.        the 
-000087c0: 7361 6d65 2077 6865 6e20 776f 726b 696e  same when workin
-000087d0: 6720 7769 7468 2061 2060 4461 7461 206f  g with a `Data o
-000087e0: 626a 6563 7460 2e0a 2020 2020 2020 2020  bject`..        
-000087f0: 0a20 2020 2020 2020 2046 6f6c 6c6f 7720  .        Follow 
-00008800: 7468 6520 7275 6c65 7320 746f 206d 616b  the rules to mak
-00008810: 6520 796f 7572 2077 6f72 6b20 7769 7468  e your work with
-00008820: 2044 6174 6120 6f62 6a65 6374 2066 6173   Data object fas
-00008830: 743a 0a20 2020 2020 2020 2031 2e20 5573  t:.        1. Us
-00008840: 6520 6044 6174 612e 7573 655f 6361 6368  e `Data.use_cach
-00008850: 6528 2960 2069 6620 796f 7520 6974 6572  e()` if you iter
-00008860: 6174 6520 6461 7461 206d 6f72 6520 7468  ate data more th
-00008870: 616e 206f 6e65 2074 696d 652e 0a20 2020  an one time..   
-00008880: 2020 2020 2032 2e20 5472 7920 746f 2064       2. Try to d
-00008890: 6f6e 2774 2069 7465 7261 7465 206f 6e65  on't iterate one
-000088a0: 2060 4461 7461 206f 626a 6563 7460 2069   `Data object` i
-000088b0: 6e73 6964 6520 7468 6520 6f74 6865 7220  nside the other 
-000088c0: 6f6e 652e 0a20 2020 2020 2020 2020 2020  one..           
-000088d0: 4966 2079 6f75 2073 686f 756c 6420 746f  If you should to
-000088e0: 2064 6f20 6974 2c20 7573 6520 7368 6f72   do it, use shor
-000088f0: 7420 6044 6174 6120 6f62 6a65 6374 6020  t `Data object` 
-00008900: 6669 7273 7420 616e 6420 6c6f 6e67 2060  first and long `
-00008910: 4461 7461 206f 626a 6563 7460 2069 6e73  Data object` ins
-00008920: 6964 6520 7468 6520 6c6f 6f70 2e0a 2020  ide the loop..  
-00008930: 2020 2020 2020 2020 2049 7427 6c6c 2061           It'll a
-00008940: 6c6c 6f77 2079 6f75 206f 7065 6e20 7468  llow you open th
-00008950: 6520 6361 6368 6520 6669 6c65 206f 7220  e cache file or 
-00008960: 6372 6561 7465 2061 2072 6571 7565 7374  create a request
-00008970: 2074 6f20 6044 6174 6120 736f 7572 6365   to `Data source
-00008980: 6020 6c65 7373 206e 756d 6265 7220 6f66  ` less number of
-00008990: 2074 696d 6573 2e0a 2020 2020 2020 2020   times..        
-000089a0: 0a20 2020 2020 2020 2023 2034 2e20 4f66  .        # 4. Of
-000089b0: 6669 6369 616c 2044 6174 6153 6f75 7263  ficial DataSourc
-000089c0: 6520 696d 706c 656d 656e 7461 7469 6f6e  e implementation
-000089d0: 730a 2020 2020 2020 2020 0a20 2020 2020  s.        .     
-000089e0: 2020 202d 205b 4c69 6768 7477 6569 6768     - [Lightweigh
-000089f0: 7420 4461 7461 2050 726f 7669 6465 7220  t Data Provider 
-00008a00: 4461 7461 2053 6f75 7263 655d 2868 7474  Data Source](htt
-00008a10: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00008a20: 7468 322d 6e65 742f 7468 322d 6473 2d73  th2-net/th2-ds-s
-00008a30: 6f75 7263 652d 6c77 6470 290a 2020 2020  ource-lwdp).    
-00008a40: 2020 2020 0a20 2020 2020 2020 200a 2020      .        .  
-00008a50: 2020 2020 2020 2320 352e 2041 5049 0a20        # 5. API. 
-00008a60: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00008a70: 4966 2079 6f75 2061 7265 206c 6f6f 6b69  If you are looki
-00008a80: 6e67 2066 6f72 2063 6c61 7373 6573 2064  ng for classes d
-00008a90: 6573 6372 6970 7469 6f6e 2073 6565 2074  escription see t
-00008aa0: 6865 205b 4150 4920 446f 6375 6d65 6e74  he [API Document
-00008ab0: 6174 696f 6e5d 2864 6f63 756d 656e 7461  ation](documenta
-00008ac0: 7469 6f6e 2f61 7069 2f69 6e64 6578 2e6d  tion/api/index.m
-00008ad0: 6429 2e0a 2020 2020 2020 2020 0a20 2020  d)..        .   
-00008ae0: 2020 2020 2023 2036 2e20 4578 616d 706c       # 6. Exampl
-00008af0: 6573 0a20 2020 2020 2020 200a 2020 2020  es.        .    
-00008b00: 2020 2020 2d20 5b67 6574 5f73 7461 7274      - [get_start
-00008b10: 6564 5f65 7861 6d70 6c65 2e70 795d 2865  ed_example.py](e
-00008b20: 7861 6d70 6c65 732f 6765 745f 7374 6172  xamples/get_star
-00008b30: 7465 645f 6578 616d 706c 652e 7079 290a  ted_example.py).
-00008b40: 2020 2020 2020 2020 0a50 6c61 7466 6f72          .Platfor
-00008b50: 6d3a 2055 4e4b 4e4f 574e 0a52 6571 7569  m: UNKNOWN.Requi
-00008b60: 7265 732d 5079 7468 6f6e 3a20 3e3d 332e  res-Python: >=3.
-00008b70: 370a 4465 7363 7269 7074 696f 6e2d 436f  7.Description-Co
-00008b80: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
-00008b90: 2f6d 6172 6b64 6f77 6e0a 5072 6f76 6964  /markdown.Provid
-00008ba0: 6573 2d45 7874 7261 3a20 7264 700a 5072  es-Extra: rdp.Pr
-00008bb0: 6f76 6964 6573 2d45 7874 7261 3a20 7264  ovides-Extra: rd
-00008bc0: 7035 0a50 726f 7669 6465 732d 4578 7472  p5.Provides-Extr
-00008bd0: 613a 2072 6470 360a 5072 6f76 6964 6573  a: rdp6.Provides
-00008be0: 2d45 7874 7261 3a20 6c77 6470 0a50 726f  -Extra: lwdp.Pro
-00008bf0: 7669 6465 732d 4578 7472 613a 206c 7764  vides-Extra: lwd
-00008c00: 7031 0a50 726f 7669 6465 732d 4578 7472  p1.Provides-Extr
-00008c10: 613a 206c 7764 7032 0a50 726f 7669 6465  a: lwdp2.Provide
-00008c20: 732d 4578 7472 613a 206c 7764 7033 0a50  s-Extra: lwdp3.P
-00008c30: 726f 7669 6465 732d 4578 7472 613a 206c  rovides-Extra: l
-00008c40: 7764 702d 6465 760a 5072 6f76 6964 6573  wdp-dev.Provides
-00008c50: 2d45 7874 7261 3a20 7574 696c 732d 7270  -Extra: utils-rp
-00008c60: 742d 7669 6577 6572 0a50 726f 7669 6465  t-viewer.Provide
-00008c70: 732d 4578 7472 613a 2075 7469 6c73 2d72  s-Extra: utils-r
-00008c80: 7074 2d76 6965 7765 7235 0a50 726f 7669  pt-viewer5.Provi
-00008c90: 6465 732d 4578 7472 613a 2075 7469 6c73  des-Extra: utils
-00008ca0: 2d61 6476 616e 6365 640a                 -advanced.
+00006870: 2023 204d 6f72 6520 7465 6368 2064 6574   # More tech det
+00006880: 6169 6c73 3a0a 2020 2020 2020 2020 2320  ails:.        # 
+00006890: 2020 496e 2074 6869 7320 6361 7365 2c20    In this case, 
+000068a0: 7468 6572 6520 6973 206e 6f20 6c69 6e65  there is no line
+000068b0: 2060 6672 6f6d 2074 6832 5f64 6174 615f   `from th2_data_
+000068c0: 7365 7276 6963 6573 2e64 6174 615f 736f  services.data_so
+000068d0: 7572 6365 2069 6d70 6f72 7420 6c77 6470  urce import lwdp
+000068e0: 2060 0a20 2020 2020 2020 2023 2020 2062   `.        #   b
+000068f0: 6563 6175 7365 2077 6520 7368 6f75 6c64  ecause we should
+00006900: 206e 6f74 2063 686f 6f73 6520 666f 7220   not choose for 
+00006910: 7468 6520 7573 6572 2077 6869 6368 2061  the user which a
+00006920: 2064 6174 6120 736f 7572 6365 2074 6f20   data source to 
+00006930: 7573 652e 0a20 2020 2020 2020 2023 2020  use..        #  
+00006940: 2057 6520 646f 206e 6f74 206b 6e6f 7720   We do not know 
+00006950: 7768 6174 2068 6520 7769 6c6c 2063 686f  what he will cho
+00006960: 6f73 652c 2074 6865 7265 666f 7265 2c20  ose, therefore, 
+00006970: 7765 206d 7573 7420 7369 6d70 6c79 2061  we must simply a
+00006980: 6363 6573 730a 2020 2020 2020 2020 2320  ccess.        # 
+00006990: 2020 7468 6520 696e 7465 7266 6163 652c    the interface,
+000069a0: 2077 6869 6368 2077 696c 6c20 6265 2069   which will be i
+000069b0: 6e69 7469 616c 697a 6564 2062 7920 7468  nitialized by th
+000069c0: 6520 7573 6572 2e0a 2020 2020 2020 2020  e user..        
+000069d0: 0a20 2020 2020 2020 2023 2323 2323 2323  .        #######
+000069e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000069f0: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
+00006a00: 2020 2020 2020 2020 2320 5b35 5d20 5573          # [5] Us
+00006a10: 696e 6720 7574 696c 6974 7920 6675 6e63  ing utility func
+00006a20: 7469 6f6e 732e 0a20 2020 2020 2020 2023  tions..        #
+00006a30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006a40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006a50: 2323 2323 230a 2020 2020 2020 2020 6672  #####.        fr
+00006a60: 6f6d 2074 6832 5f64 6174 615f 7365 7276  om th2_data_serv
+00006a70: 6963 6573 2e75 7469 6c73 2e65 7665 6e74  ices.utils.event
+00006a80: 5f75 7469 6c73 2e66 7265 7175 656e 6369  _utils.frequenci
+00006a90: 6573 2069 6d70 6f72 7420 6765 745f 6361  es import get_ca
+00006aa0: 7465 676f 7279 5f66 7265 7175 656e 6369  tegory_frequenci
+00006ab0: 6573 320a 2020 2020 2020 2020 6672 6f6d  es2.        from
+00006ac0: 2074 6832 5f64 6174 615f 7365 7276 6963   th2_data_servic
+00006ad0: 6573 2e75 7469 6c73 2e65 7665 6e74 5f75  es.utils.event_u
+00006ae0: 7469 6c73 2e74 6f74 616c 7320 696d 706f  tils.totals impo
+00006af0: 7274 2067 6574 5f63 6174 6567 6f72 795f  rt get_category_
+00006b00: 746f 7461 6c73 320a 2020 2020 2020 2020  totals2.        
+00006b10: 6672 6f6d 2074 6832 5f64 6174 615f 7365  from th2_data_se
+00006b20: 7276 6963 6573 2e75 7469 6c73 2e63 6174  rvices.utils.cat
+00006b30: 6567 6f72 7920 696d 706f 7274 2043 6174  egory import Cat
+00006b40: 6567 6f72 790a 2020 2020 2020 2020 6672  egory.        fr
+00006b50: 6f6d 2074 6832 5f64 6174 615f 7365 7276  om th2_data_serv
+00006b60: 6963 6573 2e75 7469 6c73 2e65 7665 6e74  ices.utils.event
+00006b70: 5f75 7469 6c73 2e65 7665 6e74 5f75 7469  _utils.event_uti
+00006b80: 6c73 2069 6d70 6f72 7420 6973 5f73 6f72  ls import is_sor
+00006b90: 7465 640a 2020 2020 2020 2020 0a20 2020  ted.        .   
+00006ba0: 2020 2020 2023 205b 352e 315d 2047 6574       # [5.1] Get
+00006bb0: 2074 6865 2071 7561 6e74 6974 6965 7320   the quantities 
+00006bc0: 6f66 2065 7665 6e74 7320 666f 7220 6469  of events for di
+00006bd0: 6666 6572 656e 7420 6361 7465 676f 7269  fferent categori
+00006be0: 6573 2e0a 2020 2020 2020 2020 6d65 7472  es..        metr
+00006bf0: 6963 7320 3d20 5b0a 2020 2020 2020 2020  ics = [.        
+00006c00: 2020 2020 4361 7465 676f 7279 2822 6461      Category("da
+00006c10: 7465 222c 206c 616d 6264 6120 6d3a 2054  te", lambda m: T
+00006c20: 6832 5469 6d65 7374 616d 7043 6f6e 7665  h2TimestampConve
+00006c30: 7274 6572 2e74 6f5f 6461 7465 7469 6d65  rter.to_datetime
+00006c40: 286d 5b22 7374 6172 7454 696d 6573 7461  (m["startTimesta
+00006c50: 6d70 225d 292e 6461 7465 2829 292c 0a20  mp"]).date()),. 
+00006c60: 2020 2020 2020 2020 2020 2043 6174 6567             Categ
+00006c70: 6f72 7928 2273 7461 7475 7322 2c20 6c61  ory("status", la
+00006c80: 6d62 6461 206d 3a20 6d5b 2273 7563 6365  mbda m: m["succe
+00006c90: 7373 6675 6c22 5d29 2c0a 2020 2020 2020  ssful"]),.      
+00006ca0: 2020 5d0a 2020 2020 2020 2020 6361 7465    ].        cate
+00006cb0: 676f 7279 5f74 6f74 616c 7320 3d20 6765  gory_totals = ge
+00006cc0: 745f 6361 7465 676f 7279 5f74 6f74 616c  t_category_total
+00006cd0: 7332 2865 7665 6e74 732c 206d 6574 7269  s2(events, metri
+00006ce0: 6373 290a 2020 2020 2020 2020 7072 696e  cs).        prin
+00006cf0: 7428 6361 7465 676f 7279 5f74 6f74 616c  t(category_total
+00006d00: 7329 0a20 2020 2020 2020 2022 2222 0a20  s).        """. 
+00006d10: 2020 2020 2020 202b 2d2d 2d2d 2d2d 2d2d         +--------
+00006d20: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  +------------+--
+00006d30: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00006d40: 2d2d 2b0a 2020 2020 2020 2020 7c20 2020  --+.        |   
+00006d50: 2020 2020 207c 2064 6174 6520 2020 2020       | date     
+00006d60: 2020 7c20 7374 6174 7573 2020 207c 2020    | status   |  
+00006d70: 2063 6f75 6e74 207c 0a20 2020 2020 2020   count |.       
+00006d80: 202b 3d3d 3d3d 3d3d 3d3d 2b3d 3d3d 3d3d   +========+=====
+00006d90: 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d  =======+========
+00006da0: 3d3d 2b3d 3d3d 3d3d 3d3d 3d3d 2b0a 2020  ==+=========+.  
+00006db0: 2020 2020 2020 7c20 2020 2020 2020 207c        |        |
+00006dc0: 2032 3032 332d 3031 2d30 3520 7c20 5472   2023-01-05 | Tr
+00006dd0: 7565 2020 2020 207c 2020 2020 2020 2033  ue     |       3
+00006de0: 207c 0a20 2020 2020 2020 202b 2d2d 2d2d   |.        +----
+00006df0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
+00006e00: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  -+----------+---
+00006e10: 2d2d 2d2d 2d2d 2b0a 2020 2020 2020 2020  ------+.        
+00006e20: 7c20 2020 2020 2020 207c 2032 3032 332d  |        | 2023-
+00006e30: 3031 2d30 3520 7c20 4661 6c73 6520 2020  01-05 | False   
+00006e40: 207c 2020 2020 2020 2031 207c 0a20 2020   |       1 |.   
+00006e50: 2020 2020 202b 2d2d 2d2d 2d2d 2d2d 2b2d       +--------+-
+00006e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+00006e70: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+00006e80: 2b0a 2020 2020 2020 2020 7c20 636f 756e  +.        | coun
+00006e90: 7420 207c 2020 2020 2020 2020 2020 2020  t  |            
+00006ea0: 7c20 2020 2020 2020 2020 207c 2020 2020  |          |    
+00006eb0: 2020 2032 207c 0a20 2020 2020 2020 202b     2 |.        +
+00006ec0: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00006ed0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+00006ee0: 2b2d 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020  +---------+.    
+00006ef0: 2020 2020 7c20 746f 7461 6c73 207c 2020      | totals |  
+00006f00: 2020 2020 2020 2020 2020 7c20 312f 3120            | 1/1 
+00006f10: 2020 2020 207c 2020 2020 2020 2034 207c       |       4 |
+00006f20: 0a20 2020 2020 2020 202b 2d2d 2d2d 2d2d  .        +------
+00006f30: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  --+------------+
+00006f40: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
+00006f50: 2d2d 2d2d 2b0a 2020 2020 2020 2020 2222  ----+.        ""
+00006f60: 220a 2020 2020 2020 2020 0a20 2020 2020  ".        .     
+00006f70: 2020 2023 205b 352e 325d 2047 6574 2074     # [5.2] Get t
+00006f80: 6865 206e 756d 6265 7220 6f66 2065 7665  he number of eve
+00006f90: 6e74 7320 7769 7468 2073 7461 7475 7320  nts with status 
+00006fa0: 7375 6363 6573 7366 756c 2e0a 2020 2020  successful..    
+00006fb0: 2020 2020 6361 7465 676f 7279 203d 2043      category = C
+00006fc0: 6174 6567 6f72 7928 2273 7461 7475 7322  ategory("status"
+00006fd0: 2c20 6c61 6d62 6461 206d 3a20 6d5b 2273  , lambda m: m["s
+00006fe0: 7563 6365 7373 6675 6c22 5d29 0a20 2020  uccessful"]).   
+00006ff0: 2020 2020 2063 6174 6567 6f72 795f 6672       category_fr
+00007000: 6571 7565 6e63 6965 7320 3d20 6765 745f  equencies = get_
+00007010: 6361 7465 676f 7279 5f66 7265 7175 656e  category_frequen
+00007020: 6369 6573 3228 6576 656e 7473 2c20 6361  cies2(events, ca
+00007030: 7465 676f 7279 290a 2020 2020 2020 2020  tegory).        
+00007040: 7072 696e 7428 6361 7465 676f 7279 5f66  print(category_f
+00007050: 7265 7175 656e 6369 6573 290a 2020 2020  requencies).    
+00007060: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00007070: 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  +--------+------
+00007080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+00007090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000070a0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b  -----+---------+
+000070b0: 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020 2020  --------+.      
+000070c0: 2020 7c20 2020 2020 2020 207c 2074 696d    |        | tim
+000070d0: 6573 7461 6d70 5f73 7461 7274 2020 2020  estamp_start    
+000070e0: 207c 2074 696d 6573 7461 6d70 5f65 6e64   | timestamp_end
+000070f0: 2020 2020 2020 207c 2046 616c 7365 2020         | False  
+00007100: 207c 2020 2054 7275 6520 7c0a 2020 2020   |   True |.    
+00007110: 2020 2020 2b3d 3d3d 3d3d 3d3d 3d2b 3d3d      +========+==
+00007120: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007130: 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ===+============
+00007140: 3d3d 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d  =========+======
+00007150: 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d 2b0a 2020  ===+========+.  
+00007160: 2020 2020 2020 7c20 2020 2020 2020 207c        |        |
+00007170: 2032 3032 332d 3031 2d30 3554 3133 3a35   2023-01-05T13:5
+00007180: 373a 3035 207c 2032 3032 332d 3031 2d30  7:05 | 2023-01-0
+00007190: 3554 3133 3a35 373a 3036 207c 2030 2020  5T13:57:06 | 0  
+000071a0: 2020 2020 207c 2020 2020 2020 3320 7c0a       |      3 |.
+000071b0: 2020 2020 2020 2020 2b2d 2d2d 2d2d 2d2d          +-------
+000071c0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
+000071d0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+000071e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+000071f0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+00007200: 2b0a 2020 2020 2020 2020 7c20 2020 2020  +.        |     
+00007210: 2020 207c 2032 3032 332d 3031 2d30 3554     | 2023-01-05T
+00007220: 3134 3a30 323a 3035 207c 2032 3032 332d  14:02:05 | 2023-
+00007230: 3031 2d30 3554 3134 3a30 323a 3036 207c  01-05T14:02:06 |
+00007240: 2031 2020 2020 2020 207c 2020 2020 2020   1       |      
+00007250: 3020 7c0a 2020 2020 2020 2020 2b2d 2d2d  0 |.        +---
+00007260: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+00007270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+00007280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007290: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -+---------+----
+000072a0: 2d2d 2d2d 2b0a 2020 2020 2020 2020 7c20  ----+.        | 
+000072b0: 636f 756e 7420 207c 2020 2020 2020 2020  count  |        
+000072c0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+000072d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072e0: 2020 207c 2020 2020 2020 2020 207c 2020     |         |  
+000072f0: 2020 2020 3220 7c0a 2020 2020 2020 2020      2 |.        
+00007300: 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  +--------+------
+00007310: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+00007320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007330: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b  -----+---------+
+00007340: 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020 2020  --------+.      
+00007350: 2020 7c20 746f 7461 6c73 207c 2020 2020    | totals |    
+00007360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007370: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+00007380: 2020 2020 2020 207c 2031 2020 2020 2020         | 1      
+00007390: 207c 2020 2020 2020 3320 7c0a 2020 2020   |      3 |.    
+000073a0: 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d      +--------+--
+000073b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000073c0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
+000073d0: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
+000073e0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2b0a 2020  ---+--------+.  
+000073f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00007400: 2020 0a20 2020 2020 2020 2023 205b 352e    .        # [5.
+00007410: 335d 2043 6865 636b 2069 6620 6576 656e  3] Check if even
+00007420: 7473 2061 7265 2073 6f72 7465 642e 0a20  ts are sorted.. 
+00007430: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00007440: 6973 5f73 6f72 7465 6428 6576 656e 7473  is_sorted(events
+00007450: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+00007460: 7265 7375 6c74 290a 2020 2020 2020 2020  result).        
+00007470: 6060 600a 2020 2020 2020 2020 3c21 2d2d  ```.        <!--
+00007480: 2065 6e64 2067 6574 5f73 7461 7274 6564   end get_started
+00007490: 5f65 7861 6d70 6c65 2e70 7920 2d2d 3e0a  _example.py -->.
+000074a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000074b0: 2023 2320 322e 332e 2053 686f 7274 2074   ## 2.3. Short t
+000074c0: 6865 6f72 790a 2020 2020 2020 2020 0a20  heory.        . 
+000074d0: 2020 2020 2020 2054 6865 206c 6962 7261         The libra
+000074e0: 7279 2070 726f 7669 6465 7320 746f 6f6c  ry provides tool
+000074f0: 7320 666f 7220 6861 6e64 6c69 6e67 2073  s for handling s
+00007500: 7472 6561 6d20 6461 7461 2e20 5768 6174  tream data. What
+00007510: 2773 2061 2073 7472 6561 6d3f 2049 7427  's a stream? It'
+00007520: 7320 6120 7365 7175 656e 6365 206f 6620  s a sequence of 
+00007530: 656c 656d 656e 7473 2066 726f 6d20 6120  elements from a 
+00007540: 736f 7572 6365 2074 6861 740a 2020 2020  source that.    
+00007550: 2020 2020 7375 7070 6f72 7473 2061 6767      supports agg
+00007560: 7265 6761 7465 206f 7065 7261 7469 6f6e  regate operation
+00007570: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
+00007580: 2020 2020 2323 2320 5465 726d 730a 2020      ### Terms.  
+00007590: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
+000075a0: 202a 2a44 6174 6120 6f62 6a65 6374 2a2a   **Data object**
+000075b0: 3a20 416e 2069 6e73 7461 6e63 6520 6f66  : An instance of
+000075c0: 2060 4461 7461 6020 636c 6173 7320 7768   `Data` class wh
+000075d0: 6963 6820 6973 2077 7261 7070 6572 2075  ich is wrapper u
+000075e0: 6e64 6572 2073 7472 6561 6d2e 0a20 2020  nder stream..   
+000075f0: 2020 2020 202d 202a 2a53 6571 7565 6e63       - **Sequenc
+00007600: 6520 6f66 2065 6c65 6d65 6e74 732a 2a3a  e of elements**:
+00007610: 0a20 2020 2020 2020 2020 2041 205f 4461  .          A _Da
+00007620: 7461 206f 626a 6563 745f 2070 726f 7669  ta object_ provi
+00007630: 6465 7320 616e 2069 6e74 6572 6661 6365  des an interface
+00007640: 2074 6f20 6120 7365 7175 656e 6365 6420   to a sequenced 
+00007650: 7365 7420 6f66 2076 616c 7565 7320 6f66  set of values of
+00007660: 2061 2073 7065 6369 6669 6320 656c 656d   a specific elem
+00007670: 656e 7420 7479 7065 2e20 5374 7265 616d  ent type. Stream
+00007680: 2069 6e73 6964 6520 7468 6520 5f44 6174   inside the _Dat
+00007690: 610a 2020 2020 2020 2020 2020 6f62 6a65  a.          obje
+000076a0: 6374 5f20 2a2a 646f 6e19 7420 6163 7475  ct_ **don.t actu
+000076b0: 616c 6c79 2073 746f 7265 2a2a 2065 6c65  ally store** ele
+000076c0: 6d65 6e74 733b 2074 6865 7920 6172 6520  ments; they are 
+000076d0: 636f 6d70 7574 6564 206f 6e20 6465 6d61  computed on dema
+000076e0: 6e64 2e0a 2020 2020 2020 2020 2d20 2a2a  nd..        - **
+000076f0: 6461 7461 2073 6f75 7263 652a 2a20 2865  data source** (e
+00007700: 7861 6374 6c79 2069 6e20 736d 616c 6c20  xactly in small 
+00007710: 6c65 7474 6572 7329 3a0a 2020 2020 2020  letters):.      
+00007720: 2020 2020 416e 7920 736f 7572 6365 206f      Any source o
+00007730: 6620 6461 7461 2e20 452e 672e 205b 4c69  f data. E.g. [Li
+00007740: 6768 7477 6569 6768 7420 4461 7461 2050  ghtweight Data P
+00007750: 726f 7669 6465 725d 2868 7474 7073 3a2f  rovider](https:/
+00007760: 2f67 6974 6875 622e 636f 6d2f 7468 322d  /github.com/th2-
+00007770: 6e65 742f 7468 322d 6c77 2d64 6174 612d  net/th2-lw-data-
+00007780: 7072 6f76 6964 6572 292c 2063 6f6c 6c65  provider), colle
+00007790: 6374 696f 6e73 2c0a 2020 2020 2020 2020  ctions,.        
+000077a0: 2020 6172 7261 7973 2c20 6f72 2049 2f4f    arrays, or I/O
+000077b0: 2072 6573 6f75 7263 6573 2e0a 2020 2020   resources..    
+000077c0: 2020 2020 2d20 2a2a 4461 7461 536f 7572      - **DataSour
+000077d0: 6365 2a2a 3a0a 2020 2020 2020 2020 2020  ce**:.          
+000077e0: 4120 636c 6173 7320 7468 6174 2069 7320  A class that is 
+000077f0: 616e 2069 6e74 6572 6d65 6469 6174 6520  an intermediate 
+00007800: 6c69 6e6b 2062 6574 7765 656e 2074 6865  link between the
+00007810: 2053 6f75 7263 6541 5049 2061 6e64 2043   SourceAPI and C
+00007820: 6f6d 6d61 6e64 732e 0a20 2020 2020 2020  ommands..       
+00007830: 202d 202a 2a53 6f75 7263 6541 5049 2a2a   - **SourceAPI**
+00007840: 3a0a 2020 2020 2020 2020 2020 4561 6368  :.          Each
+00007850: 2073 6f75 7263 6520 6861 7320 6974 7320   source has its 
+00007860: 6f77 6e20 4150 4920 746f 2072 6574 7269  own API to retri
+00007870: 6576 6520 6461 7461 2e20 536f 7572 6365  eve data. Source
+00007880: 4150 4920 6973 2061 2063 6c61 7373 2074  API is a class t
+00007890: 6861 7420 7072 6f76 6964 6520 4150 4920  hat provide API 
+000078a0: 666f 7220 736f 6d65 2064 6174 6120 736f  for some data so
+000078b0: 7572 6365 2e0a 2020 2020 2020 2020 2d20  urce..        - 
+000078c0: 2a2a 436f 6d6d 616e 6473 2a2a 3a0a 2020  **Commands**:.  
+000078d0: 2020 2020 2020 2020 436c 6173 7365 7320          Classes 
+000078e0: 7468 6174 2070 726f 7669 6465 2075 7365  that provide use
+000078f0: 722d 6672 6965 6e64 6c79 2069 6e74 6572  r-friendly inter
+00007900: 6661 6365 7320 666f 7220 6765 7474 696e  faces for gettin
+00007910: 6720 736f 6d65 2064 6174 6120 6672 6f6d  g some data from
+00007920: 2044 6174 6153 6f75 7263 652e 2043 6f6d   DataSource. Com
+00007930: 6d61 6e64 7320 7573 6520 5f53 6f75 7263  mands use _Sourc
+00007940: 6541 5049 5f20 746f 0a20 2020 2020 2020  eAPI_ to.       
+00007950: 2020 2061 6368 6965 7665 2069 742e 0a20     achieve it.. 
+00007960: 2020 2020 2020 202d 202a 2a41 6461 7074         - **Adapt
+00007970: 6572 732a 2a3a 0a20 2020 2020 2020 2020  ers**:.         
+00007980: 2049 7427 7320 7369 6d69 6c61 7220 746f   It's similar to
+00007990: 2066 756e 6374 696f 6e20 666f 7220 6044   function for `D
+000079a0: 6174 612e 6d61 7060 206d 6574 686f 642e  ata.map` method.
+000079b0: 2041 646f 7074 6162 6c65 2063 6f6d 6d61   Adoptable comma
+000079c0: 6e64 7320 7573 6564 2069 7420 746f 2075  nds used it to u
+000079d0: 7064 6174 6520 7468 6520 6461 7461 2073  pdate the data s
+000079e0: 7472 6561 6d2e 0a20 2020 2020 2020 202d  tream..        -
+000079f0: 202a 2a41 6767 7265 6761 7465 206f 7065   **Aggregate ope
+00007a00: 7261 7469 6f6e 732a 2a3a 0a20 2020 2020  rations**:.     
+00007a10: 2020 2020 2043 6f6d 6d6f 6e20 6f70 6572       Common oper
+00007a20: 6174 696f 6e73 2073 7563 6820 6173 2066  ations such as f
+00007a30: 696c 7465 722c 206d 6170 2c20 6c69 6d69  ilter, map, limi
+00007a40: 7420 616e 6420 736f 206f 6e2e 0a20 2020  t and so on..   
+00007a50: 2020 2020 202d 202a 2a57 6f72 6b66 6c6f       - **Workflo
+00007a60: 772a 2a3a 2041 6e20 6f72 6465 7265 6420  w**: An ordered 
+00007a70: 7365 7420 6f66 205f 4167 6772 6567 6174  set of _Aggregat
+00007a80: 6520 6f70 6572 6174 696f 6e73 5f2e 0a20  e operations_.. 
+00007a90: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00007aa0: 2323 2320 436f 6e63 6570 740a 2020 2020  ### Concept.    
+00007ab0: 2020 2020 0a20 2020 2020 2020 2054 6865      .        The
+00007ac0: 206c 6962 7261 7279 2064 6573 6372 6962   library describ
+00007ad0: 6573 2074 6865 2068 6967 682d 6c65 7665  es the high-leve
+00007ae0: 6c20 696e 7465 7266 6163 6573 2060 4953  l interfaces `IS
+00007af0: 6f75 7263 6541 5049 602c 2060 4944 6174  ourceAPI`, `IDat
+00007b00: 6153 6f75 7263 6560 2c20 6049 436f 6d6d  aSource`, `IComm
+00007b10: 616e 6460 2c20 6049 4164 6170 7465 7260  and`, `IAdapter`
+00007b20: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00007b30: 2020 2041 6e79 2064 6174 6120 736f 7572     Any data sour
+00007b40: 6365 206d 7573 7420 6265 2064 6573 6372  ce must be descr
+00007b50: 6962 6564 2062 7920 7468 6520 6049 4461  ibed by the `IDa
+00007b60: 7461 536f 7572 6365 6020 6162 7374 7261  taSource` abstra
+00007b70: 6374 2063 6c61 7373 2e20 5468 6573 6520  ct class. These 
+00007b80: 6361 6e20 6265 205f 4669 6c65 4461 7461  can be _FileData
+00007b90: 536f 7572 6365 5f2c 0a20 2020 2020 2020  Source_,.       
+00007ba0: 205f 4353 5644 6174 6153 6f75 7263 655f   _CSVDataSource_
+00007bb0: 2c20 5f44 4244 6174 6153 6f75 7263 655f  , _DBDataSource_
+00007bc0: 2061 6e64 206f 7468 6572 2e0a 2020 2020   and other..    
+00007bd0: 2020 2020 0a20 2020 2020 2020 2055 7375      .        Usu
+00007be0: 616c 6c79 2c20 6461 7461 2073 6f75 7263  ally, data sourc
+00007bf0: 6573 2068 6176 6520 736f 6d65 206b 696e  es have some kin
+00007c00: 6420 6f66 2041 5049 2e20 4461 7461 6261  d of API. Databa
+00007c10: 7365 7320 2d20 7072 6f76 6964 6520 5351  ses - provide SQ
+00007c20: 4c20 6c61 6e67 7561 6765 2c20 7768 656e  L language, when
+00007c30: 2077 6f72 6b69 6e67 2077 6974 6820 6120   working with a 
+00007c40: 6669 6c65 2c20 796f 7520 6361 6e20 7265  file, you can re
+00007c50: 6164 0a20 2020 2020 2020 206c 696e 6520  ad.        line 
+00007c60: 6279 206c 696e 652c 2065 7463 2e20 5468  by line, etc. Th
+00007c70: 6973 2041 5049 2069 7320 6465 7363 7269  is API is descri
+00007c80: 6265 6420 6279 2074 6865 2060 4953 6f75  bed by the `ISou
+00007c90: 7263 6541 5049 6020 636c 6173 732e 2042  rceAPI` class. B
+00007ca0: 6563 6175 7365 2064 6966 6665 7265 6e74  ecause different
+00007cb0: 2076 6572 7369 6f6e 7320 6f66 2074 6865   versions of the
+00007cc0: 2073 616d 6520 6461 7461 2073 6f75 7263   same data sourc
+00007cd0: 650a 2020 2020 2020 2020 6d61 7920 6861  e.        may ha
+00007ce0: 7665 2064 6966 6665 7265 6e74 2041 5049  ve different API
+00007cf0: 2c20 6974 2069 7320 6265 7474 6572 2074  , it is better t
+00007d00: 6f20 6372 6561 7465 2061 2063 6c61 7373  o create a class
+00007d10: 2066 6f72 2065 6163 6820 7665 7273 696f   for each versio
+00007d20: 6e2e 0a20 2020 2020 2020 200a 2020 2020  n..        .    
+00007d30: 2020 2020 4765 6e65 7261 6c6c 792c 2064      Generally, d
+00007d40: 6174 6120 736f 7572 6365 2041 5049 7320  ata source APIs 
+00007d50: 6172 6520 6869 6464 656e 2062 6568 696e  are hidden behin
+00007d60: 6420 636f 6e76 656e 6965 6e74 2069 6e74  d convenient int
+00007d70: 6572 6661 6365 732e 2054 6865 2072 6f6c  erfaces. The rol
+00007d80: 6520 6f66 2074 6865 7365 2069 6e74 6572  e of these inter
+00007d90: 6661 6365 7320 6973 2070 6c61 7965 640a  faces is played.
+00007da0: 2020 2020 2020 2020 6279 2060 4943 6f6d          by `ICom
+00007db0: 6d61 6e64 6020 636c 6173 7365 732e 0a20  mand` classes.. 
+00007dc0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00007dd0: 6049 4164 6170 7465 7260 2063 6c61 7373  `IAdapter` class
+00007de0: 6573 2074 7261 6e73 666f 726d 2064 6174  es transform dat
+00007df0: 6120 7374 7265 616d 206c 696b 6520 6675  a stream like fu
+00007e00: 6e63 7469 6f6e 7320 666f 7220 6044 6174  nctions for `Dat
+00007e10: 612e 6d61 7060 206d 6574 686f 642e 2045  a.map` method. E
+00007e20: 7373 656e 7469 616c 6c79 2069 7427 7320  ssentially it's 
+00007e30: 7468 6520 7361 6d65 2074 6869 6e67 2062  the same thing b
+00007e40: 7574 206d 6f72 650a 2020 2020 2020 2020  ut more.        
+00007e50: 666c 6578 6962 6c65 2e0a 2020 2020 2020  flexible..      
+00007e60: 2020 0a20 2020 2020 2020 2046 6f72 2065    .        For e
+00007e70: 7861 6d70 6c65 2c20 4c77 4450 2044 6174  xample, LwDP Dat
+00007e80: 6153 6f75 7263 6528 6874 7470 733a 2f2f  aSource(https://
+00007e90: 6769 7468 7562 2e63 6f6d 2f74 6832 2d6e  github.com/th2-n
+00007ea0: 6574 2f74 6832 2d64 732d 736f 7572 6365  et/th2-ds-source
+00007eb0: 2d6c 7764 7029 2075 7365 7320 7468 6573  -lwdp) uses thes
+00007ec0: 6520 6162 7374 7261 6374 2063 6c61 7373  e abstract class
+00007ed0: 6573 2074 6f20 6275 696c 6420 6974 7320  es to build its 
+00007ee0: 696d 706c 656d 656e 7461 7469 6f6e 2e59  implementation.Y
+00007ef0: 6f75 2063 616e 2065 6173 696c 7920 6372  ou can easily cr
+00007f00: 6561 7465 2079 6f75 7220 6f77 6e20 756e  eate your own un
+00007f10: 6971 7565 2063 6f6d 6d61 6e64 7320 666f  ique commands fo
+00007f20: 7220 5f4c 7744 5020 4461 7461 536f 7572  r _LwDP DataSour
+00007f30: 6365 5f2c 2061 7320 7765 6c6c 2061 7320  ce_, as well as 
+00007f40: 656e 7469 7265 0a20 2020 2020 2020 205f  entire.        _
+00007f50: 4461 7461 536f 7572 6365 5f20 636c 6173  DataSource_ clas
+00007f60: 7365 732e 205b 4865 7265 2069 7320 6120  ses. [Here is a 
+00007f70: 646f 6375 6d65 6e74 6174 696f 6e5d 2864  documentation](d
+00007f80: 6f63 756d 656e 7461 7469 6f6e 2f64 6174  ocumentation/dat
+00007f90: 6173 6f75 7263 652e 6d64 2920 6f6e 2068  asource.md) on h
+00007fa0: 6f77 2074 6f20 696d 706c 656d 656e 7420  ow to implement 
+00007fb0: 7468 6573 6520 696e 7465 7266 6163 6573  these interfaces
+00007fc0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00007fd0: 2020 2021 5b44 6174 6120 7374 7265 616d     ![Data stream
+00007fe0: 2070 6970 656c 696e 655d 2864 6f63 756d   pipeline](docum
+00007ff0: 656e 7461 7469 6f6e 2f69 6d67 2f63 6f6e  entation/img/con
+00008000: 6365 7074 2e70 6e67 290a 2020 2020 2020  cept.png).      
+00008010: 2020 0a20 2020 2020 2020 2023 2323 2053    .        ### S
+00008020: 7472 6561 6d20 6f70 6572 6174 696f 6e73  tream operations
+00008030: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00008040: 2020 4675 7274 6865 726d 6f72 652c 2073    Furthermore, s
+00008050: 7472 6561 6d20 6f70 6572 6174 696f 6e73  tream operations
+00008060: 2068 6176 6520 7477 6f20 6675 6e64 616d   have two fundam
+00008070: 656e 7461 6c20 6368 6172 6163 7465 7269  ental characteri
+00008080: 7374 6963 7320 7468 6174 206d 616b 6520  stics that make 
+00008090: 7468 656d 2076 6572 7920 6469 6666 6572  them very differ
+000080a0: 656e 7420 6672 6f6d 2063 6f6c 6c65 6374  ent from collect
+000080b0: 696f 6e0a 2020 2020 2020 2020 6f70 6572  ion.        oper
+000080c0: 6174 696f 6e73 3a20 5f50 6970 656c 696e  ations: _Pipelin
+000080d0: 696e 675f 2061 6e64 205f 496e 7465 726e  ing_ and _Intern
+000080e0: 616c 2069 7465 7261 7469 6f6e 5f2e 0a20  al iteration_.. 
+000080f0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00008100: 2323 2323 2050 6970 656c 696e 696e 670a  #### Pipelining.
+00008110: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00008120: 204d 616e 7920 7374 7265 616d 206f 7065   Many stream ope
+00008130: 7261 7469 6f6e 7320 7265 7475 726e 2061  rations return a
+00008140: 2073 7472 6561 6d20 7468 656d 7365 6c76   stream themselv
+00008150: 6573 2e20 5468 6973 2061 6c6c 6f77 7320  es. This allows 
+00008160: 6f70 6572 6174 696f 6e73 2074 6f20 6265  operations to be
+00008170: 2063 6861 696e 6564 2074 6f20 666f 726d   chained to form
+00008180: 2061 206c 6172 6765 7220 7069 7065 6c69   a larger pipeli
+00008190: 6e65 2e0a 2020 2020 2020 2020 0a20 2020  ne..        .   
+000081a0: 2020 2020 2021 5b44 6174 6120 7374 7265       ![Data stre
+000081b0: 616d 2070 6970 656c 696e 655d 2864 6f63  am pipeline](doc
+000081c0: 756d 656e 7461 7469 6f6e 2f69 6d67 2f64  umentation/img/d
+000081d0: 6174 615f 7374 7265 616d 5f70 6970 656c  ata_stream_pipel
+000081e0: 696e 652e 706e 6729 0a20 2020 2020 2020  ine.png).       
+000081f0: 200a 2020 2020 2020 2020 2323 2323 2049   .        #### I
+00008200: 6e74 6572 6e61 6c20 6974 6572 6174 696f  nternal iteratio
+00008210: 6e0a 2020 2020 2020 2020 0a20 2020 2020  n.        .     
+00008220: 2020 2049 6e20 636f 6e74 7261 7374 2074     In contrast t
+00008230: 6f20 636f 6c6c 6563 7469 6f6e 732c 2077  o collections, w
+00008240: 6869 6368 2061 7265 2069 7465 7261 7465  hich are iterate
+00008250: 6420 6578 706c 6963 6974 6c79 2028 6578  d explicitly (ex
+00008260: 7465 726e 616c 2069 7465 7261 7469 6f6e  ternal iteration
+00008270: 292c 2073 7472 6561 6d20 6f70 6572 6174  ), stream operat
+00008280: 696f 6e73 2064 6f20 7468 6520 6974 6572  ions do the iter
+00008290: 6174 696f 6e0a 2020 2020 2020 2020 6265  ation.        be
+000082a0: 6869 6e64 2074 6865 2073 6365 6e65 7320  hind the scenes 
+000082b0: 666f 7220 796f 752e 204e 6f74 652c 2069  for you. Note, i
+000082c0: 7420 646f 6573 6e27 7420 6d65 616e 2079  t doesn't mean y
+000082d0: 6f75 2063 616e 6e6f 7420 6974 6572 6174  ou cannot iterat
+000082e0: 6520 7468 6520 5f44 6174 6120 6f62 6a65  e the _Data obje
+000082f0: 6374 5f2e 0a20 2020 2020 2020 200a 2020  ct_..        .  
+00008300: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00008310: 2323 2044 6174 6120 6974 6572 6174 696f  ## Data iteratio
+00008320: 6e0a 2020 2020 2020 2020 0a20 2020 2020  n.        .     
+00008330: 2020 2054 6865 2044 6174 6120 6f62 6a65     The Data obje
+00008340: 6374 2063 6f6e 7374 7275 6374 6f72 206d  ct constructor m
+00008350: 6574 686f 6420 7461 6b65 7320 696e 2061  ethod takes in a
+00008360: 7320 6172 6775 6d65 6e74 2065 6974 6865  s argument eithe
+00008370: 7220 616e 2069 7465 7261 746f 7220 6f76  r an iterator ov
+00008380: 6572 206f 626a 6563 7473 206f 7220 6120  er objects or a 
+00008390: 6765 6e65 7261 746f 7220 6675 6e63 7469  generator functi
+000083a0: 6f6e 2e0a 2020 2020 2020 2020 5468 6520  on..        The 
+000083b0: 4461 7461 206f 626a 6563 7420 6974 6572  Data object iter
+000083c0: 6174 6f72 2068 616e 646c 6573 2065 6163  ator handles eac
+000083d0: 6820 6974 656d 2069 6e20 7468 6973 2069  h item in this i
+000083e0: 7465 7261 746f 7220 6f72 2067 656e 6572  terator or gener
+000083f0: 6174 6f72 2061 7320 7468 6579 2061 7265  ator as they are
+00008400: 2c20 6d65 616e 696e 6720 6974 2064 6f65  , meaning it doe
+00008410: 736e 2774 2074 7279 2074 6f20 7265 6164  sn't try to read
+00008420: 2074 6865 2063 6f6e 7465 6e74 206f 6620   the content of 
+00008430: 6974 656d 206f 7220 7265 7475 726e 2074  item or return t
+00008440: 6865 6d20 6d6f 6469 6669 6564 2069 6e20  hem modified in 
+00008450: 616e 7920 7761 792c 2069 6e73 7465 6164  any way, instead
+00008460: 2072 6574 7572 6e73 2074 6865 2069 7465   returns the ite
+00008470: 6d20 6974 7365 6c66 2e0a 2020 2020 2020  m itself..      
+00008480: 2020 5468 6520 6f6e 6c79 2065 7863 6570    The only excep
+00008490: 7469 6f6e 2074 6f20 7468 6973 2069 7320  tion to this is 
+000084a0: 7768 656e 2044 6174 6120 6f62 6a65 6374  when Data object
+000084b0: 2069 7320 6275 696c 7420 7573 696e 6720   is built using 
+000084c0: 6974 6572 6174 6f72 206f 7220 6765 6e65  iterator or gene
+000084d0: 7261 746f 7220 6f76 6572 206f 7468 6572  rator over other
+000084e0: 2044 6174 6120 6f62 6a65 6374 732e 204e   Data objects. N
+000084f0: 6f74 6520 7468 6174 2074 6869 7320 6974  ote that this it
+00008500: 6572 6174 6f72 206f 7220 6765 6e65 7261  erator or genera
+00008510: 746f 7220 6d75 7374 206f 6e6c 7920 6265  tor must only be
+00008520: 2079 6965 6c64 696e 6720 4461 7461 206f   yielding Data o
+00008530: 626a 6563 7473 2061 6e64 206e 6f74 6869  bjects and nothi
+00008540: 6e67 2065 6c73 652e 2049 6620 7765 2062  ng else. If we b
+00008550: 7569 6c64 2066 726f 6d20 6120 6d69 7820  uild from a mix 
+00008560: 6f66 2044 6174 6120 6f62 6a65 6374 7320  of Data objects 
+00008570: 616e 6420 736f 6d65 206f 7468 6572 2074  and some other t
+00008580: 7970 6573 2c20 4461 7461 206f 626a 6563  ypes, Data objec
+00008590: 7473 2720 636f 6e74 656e 7420 776f 6e27  ts' content won'
+000085a0: 7420 6265 2072 6561 6420 616e 6420 696e  t be read and in
+000085b0: 7374 6561 6420 6974 2077 696c 6c20 6265  stead it will be
+000085c0: 2072 6574 7572 6e65 6420 6173 2044 6174   returned as Dat
+000085d0: 6120 6f62 6a65 6374 2069 7473 656c 662e  a object itself.
+000085e0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000085f0: 2020 536d 616c 6c20 6578 616d 706c 6520    Small example 
+00008600: 746f 2064 656d 6f6e 7374 7261 7465 3a0a  to demonstrate:.
+00008610: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00008620: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
+00008630: 2020 2066 726f 6d20 7468 325f 6461 7461     from th2_data
+00008640: 5f73 6572 7669 6365 732e 6461 7461 2069  _services.data i
+00008650: 6d70 6f72 7420 4461 7461 0a20 2020 2020  mport Data.     
+00008660: 2020 200a 2020 2020 2020 2020 6431 203d     .        d1 =
+00008670: 2044 6174 6128 5b31 2c32 2c33 5d29 0a20   Data([1,2,3]). 
+00008680: 2020 2020 2020 2064 3220 3d20 4461 7461         d2 = Data
+00008690: 285b 342c 352c 365d 290a 2020 2020 2020  ([4,5,6]).      
+000086a0: 2020 0a20 2020 2020 2020 206f 6e6c 795f    .        only_
+000086b0: 6461 7461 5f6f 626a 6563 7473 203d 2044  data_objects = D
+000086c0: 6174 6128 5b64 312c 6432 5d29 2023 2057  ata([d1,d2]) # W
+000086d0: 696c 6c20 6974 6572 6174 6520 6173 2031  ill iterate as 1
+000086e0: 2c32 2c33 2c34 2c35 2c36 0a20 2020 2020  ,2,3,4,5,6.     
+000086f0: 2020 2064 6174 615f 616e 645f 6c69 7374     data_and_list
+00008700: 203d 2044 6174 6128 5b64 312c 5b34 2c35   = Data([d1,[4,5
+00008710: 2c36 5d5d 2920 2320 5769 6c6c 2069 7465  ,6]]) # Will ite
+00008720: 7261 7465 2061 7320 6431 2c20 5b34 2c35  rate as d1, [4,5
+00008730: 2c36 5d0a 2020 2020 2020 2020 6461 7461  ,6].        data
+00008740: 5f61 6e64 5f6e 756d 6265 7273 203d 2044  _and_numbers = D
+00008750: 6174 6128 5b64 312c 342c 352c 365d 2920  ata([d1,4,5,6]) 
+00008760: 2320 5769 6c6c 2069 7465 7261 7465 2061  # Will iterate a
+00008770: 7320 6431 2c34 2c35 2c36 0a20 2020 2020  s d1,4,5,6.     
+00008780: 2020 206c 6973 7473 5f6f 6e6c 7920 3d20     lists_only = 
+00008790: 4461 7461 285b 312c 322c 335d 2c5b 342c  Data([1,2,3],[4,
+000087a0: 352c 365d 2920 2320 5769 6c6c 2069 7465  5,6]) # Will ite
+000087b0: 7261 7465 2061 7320 5b31 2c32 2c33 5d2c  rate as [1,2,3],
+000087c0: 5b34 2c35 2c36 5d0a 2020 2020 2020 2020  [4,5,6].        
+000087d0: 0a20 2020 2020 2020 2023 2049 6620 7765  .        # If we
+000087e0: 2077 616e 7420 746f 2069 7465 7261 7465   want to iterate
+000087f0: 206f 7665 7220 636f 6e74 656e 7420 6f66   over content of
+00008800: 206c 6973 7420 6f66 206c 6973 7473 2c20   list of lists, 
+00008810: 7765 2073 686f 756c 6420 6669 7273 7420  we should first 
+00008820: 6372 6561 7465 2044 6174 6120 6f62 6a65  create Data obje
+00008830: 6374 7320 6672 6f6d 2074 6865 6d2c 0a20  cts from them,. 
+00008840: 2020 2020 2020 2023 2074 6865 6e20 7573         # then us
+00008850: 6520 7468 656d 2074 6f20 636f 6e73 7472  e them to constr
+00008860: 7563 7420 6e65 7720 4461 7461 206f 626a  uct new Data obj
+00008870: 6563 7420 6173 2069 6e20 6361 7365 206f  ect as in case o
+00008880: 6620 6431 2061 6e64 2064 322c 2063 7265  f d1 and d2, cre
+00008890: 6174 696e 6720 276f 6e6c 795f 6461 7461  ating 'only_data
+000088a0: 5f6f 626a 6563 7473 2720 696e 2074 6869  _objects' in thi
+000088b0: 7320 6578 616d 706c 652e 0a20 2020 2020  s example..     
+000088c0: 2020 2060 6060 0a20 2020 2020 2020 2020     ```.         
+000088d0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000088e0: 2020 2323 2320 4461 7461 2063 6163 6869    ### Data cachi
+000088f0: 6e67 0a20 2020 2020 2020 200a 2020 2020  ng.        .    
+00008900: 2020 2020 5468 6520 5f44 6174 6120 6f62      The _Data ob
+00008910: 6a65 6374 5f20 7072 6f76 6964 6573 2074  ject_ provides t
+00008920: 6865 2061 6269 6c69 7479 2074 6f20 7573  he ability to us
+00008930: 6520 7468 6520 6361 6368 652e 2054 6865  e the cache. The
+00008940: 2063 6163 6865 2077 6f72 6b73 2066 6f72   cache works for
+00008950: 2065 6163 6820 5f44 6174 6120 6f62 6a65   each _Data obje
+00008960: 6374 5f2c 2074 6861 7420 6973 2c20 796f  ct_, that is, yo
+00008970: 7520 6368 6f6f 7365 0a20 2020 2020 2020  u choose.       
+00008980: 2077 6869 6368 205f 4461 7461 206f 626a   which _Data obj
+00008990: 6563 745f 2079 6f75 2077 616e 7420 746f  ect_ you want to
+000089a0: 2073 6176 652e 2054 6865 205f 4461 7461   save. The _Data
+000089b0: 206f 626a 6563 745f 2063 6163 6865 2069   object_ cache i
+000089c0: 7320 7361 7665 6420 6166 7465 7220 7468  s saved after th
+000089d0: 6520 6669 7273 7420 6974 6572 6174 696f  e first iteratio
+000089e0: 6e2c 2062 7574 2074 6865 2069 7465 7261  n, but the itera
+000089f0: 7469 6f6e 0a20 2020 2020 2020 2073 6f75  tion.        sou
+00008a00: 7263 6520 6d61 7920 6265 2064 6966 6665  rce may be diffe
+00008a10: 7265 6e74 2e0a 2020 2020 2020 2020 0a20  rent..        . 
+00008a20: 2020 2020 2020 2049 6620 796f 7520 646f         If you do
+00008a30: 6e27 7420 7573 6520 7468 6520 6361 6368  n't use the cach
+00008a40: 652c 2079 6f75 7220 736f 7572 6365 2077  e, your source w
+00008a50: 696c 6c20 6265 2074 6865 2064 6174 6120  ill be the data 
+00008a60: 736f 7572 6365 2079 6f75 2068 6176 6520  source you have 
+00008a70: 696e 2074 6865 205f 4461 7461 204f 626a  in the _Data Obj
+00008a80: 6563 745f 2e20 4275 7420 6966 2079 6f75  ect_. But if you
+00008a90: 2075 7365 2074 6865 2063 6163 6865 2c0a   use the cache,.
+00008aa0: 2020 2020 2020 2020 796f 7572 2073 6f75          your sou
+00008ab0: 7263 6520 6361 6e20 6265 2074 6865 2064  rce can be the d
+00008ac0: 6174 6120 736f 7572 6365 2c20 7468 6520  ata source, the 
+00008ad0: 7061 7265 6e74 2063 6163 6865 2c20 6f72  parent cache, or
+00008ae0: 206f 776e 2063 6163 6865 3a0a 2020 2020   own cache:.    
+00008af0: 2020 2020 0a20 2020 2020 2020 202a 2054      .        * T
+00008b00: 6865 2064 6174 6120 736f 7572 6365 3a0a  he data source:.
+00008b10: 2020 2020 2020 2020 2020 4966 2074 6865            If the
+00008b20: 205f 4461 7461 204f 626a 6563 745f 2064   _Data Object_ d
+00008b30: 6f65 736e 2774 2068 6176 6520 6120 7061  oesn't have a pa
+00008b40: 7265 6e74 2063 6163 6865 2061 6e64 2069  rent cache and i
+00008b50: 7473 2063 6163 6865 2e0a 2020 2020 2020  ts cache..      
+00008b60: 2020 2a20 5468 6520 7061 7265 6e74 2063    * The parent c
+00008b70: 6163 6865 3a0a 2020 2020 2020 2020 2020  ache:.          
+00008b80: 4966 2074 6865 205f 4461 7461 204f 626a  If the _Data Obj
+00008b90: 6563 745f 2068 6173 2061 2070 6172 656e  ect_ has a paren
+00008ba0: 7420 6361 6368 652e 2049 7420 646f 6573  t cache. It does
+00008bb0: 6e27 7420 6d61 7474 6572 2077 6861 7420  n't matter what 
+00008bc0: 706f 7369 7469 6f6e 2074 6865 2070 6172  position the par
+00008bd0: 656e 7420 6361 6368 6520 6861 7320 696e  ent cache has in
+00008be0: 2069 6e68 6572 6974 616e 6365 2e0a 2020   inheritance..  
+00008bf0: 2020 2020 2020 2020 5f44 6174 6120 4f62          _Data Ob
+00008c00: 6a65 6374 5f20 756e 6465 7273 7461 6e64  ject_ understand
+00008c10: 7320 7768 6f73 6520 6361 6368 6520 6974  s whose cache it
+00008c20: 2069 7320 616e 6420 6578 6563 7574 6573   is and executes
+00008c30: 2074 6865 2070 6172 7420 6f66 2074 6865   the part of the
+00008c40: 2077 6f72 6b66 6c6f 7720 7468 6174 2077   workflow that w
+00008c50: 6173 206e 6f74 2065 7865 6375 7465 642e  as not executed.
+00008c60: 0a20 2020 2020 2020 202a 2054 6865 206f  .        * The o
+00008c70: 776e 2063 6163 6865 3a0a 2020 2020 2020  wn cache:.      
+00008c80: 2020 2020 4966 2069 7420 6973 206e 6f74      If it is not
+00008c90: 2074 6865 2066 6972 7374 2069 7465 7261   the first itera
+00008ca0: 7469 6f6e 206f 6620 7468 6973 2044 6174  tion of this Dat
+00008cb0: 6120 6f62 6a65 6374 2e0a 2020 2020 2020  a object..      
+00008cc0: 2020 0a20 2020 2020 2020 204e 6f74 6520    .        Note 
+00008cd0: 7468 6174 2074 6865 2063 6163 6865 2073  that the cache s
+00008ce0: 7461 7465 206f 6620 7468 6520 4461 7461  tate of the Data
+00008cf0: 206f 626a 6563 7420 6973 206e 6f74 2069   object is not i
+00008d00: 6e68 6572 6974 6564 2e0a 2020 2020 2020  nherited..      
+00008d10: 2020 0a20 2020 2020 2020 2023 2323 2320    .        #### 
+00008d20: 466f 7263 6564 2063 6163 6869 6e67 0a20  Forced caching. 
+00008d30: 2020 2020 2020 2059 6f75 2063 616e 2074         You can t
+00008d40: 656c 6c20 4453 2074 6f20 6361 6368 6520  ell DS to cache 
+00008d50: 6461 7461 2074 6f20 7370 6563 6966 6963  data to specific
+00008d60: 2063 6163 6865 2066 696c 652c 2077 6869   cache file, whi
+00008d70: 6368 2077 6f6e 2774 2062 6520 6465 6c65  ch won't be dele
+00008d80: 7465 6420 6166 7465 7220 7363 7269 7074  ted after script
+00008d90: 2065 6e64 2e0a 2020 2020 2020 2020 596f   end..        Yo
+00008da0: 7520 6361 6e20 7365 6520 6578 616d 706c  u can see exampl
+00008db0: 6520 696e 2031 2e31 3220 7365 6374 696f  e in 1.12 sectio
+00008dc0: 6e20 6f66 205b 6765 745f 7374 6172 7465  n of [get_starte
+00008dd0: 645f 6578 616d 706c 655d 2865 7861 6d70  d_example](examp
+00008de0: 6c65 732f 6765 745f 7374 6172 7465 645f  les/get_started_
+00008df0: 6578 616d 706c 652e 7079 292e 0a20 2020  example.py)..   
+00008e00: 2020 2020 200a 2020 2020 2020 2020 0a20       .        . 
+00008e10: 2020 2020 2020 2023 2323 2045 7665 6e74         ### Event
+00008e20: 5472 6565 2061 6e64 2063 6f6c 6c65 6374  Tree and collect
+00008e30: 696f 6e73 0a20 2020 2020 2020 200a 2020  ions.        .  
+00008e40: 2020 2020 2020 2323 2323 2045 7665 6e74        #### Event
+00008e50: 5472 6565 0a20 2020 2020 2020 200a 2020  Tree.        .  
+00008e60: 2020 2020 2020 6045 7665 6e74 5472 6565        `EventTree
+00008e70: 6020 6973 2061 2074 7265 652d 6261 7365  ` is a tree-base
+00008e80: 6420 6461 7461 2073 7472 7563 7475 7265  d data structure
+00008e90: 206f 6620 6576 656e 7473 2e20 4974 2061   of events. It a
+00008ea0: 6c6c 6f77 7320 796f 7520 6765 7420 6368  llows you get ch
+00008eb0: 696c 6472 656e 2061 6e64 2070 6172 656e  ildren and paren
+00008ec0: 7473 206f 6620 6576 656e 742c 0a20 2020  ts of event,.   
+00008ed0: 2020 2020 2064 6973 706c 6179 2074 7265       display tre
+00008ee0: 652c 2067 6574 2066 756c 6c20 7061 7468  e, get full path
+00008ef0: 2074 6f20 6576 656e 7420 6574 632e 0a20   to event etc.. 
+00008f00: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00008f10: 4465 7461 696c 733a 0a20 2020 2020 2020  Details:.       
+00008f20: 200a 2020 2020 2020 2020 2a20 6045 7665   .        * `Eve
+00008f30: 6e74 5472 6565 6020 636f 6e74 6169 6e73  ntTree` contains
+00008f40: 2061 6c6c 2065 7665 6e74 7320 696e 206d   all events in m
+00008f50: 656d 6f72 792e 0a20 2020 2020 2020 202a  emory..        *
+00008f60: 2054 7265 6520 6861 7320 736f 6d65 2069   Tree has some i
+00008f70: 6d70 6f72 7461 6e74 2074 6572 6d73 3a0a  mportant terms:.
+00008f80: 2020 2020 2020 2020 2020 2020 312e 205f              1. _
+00008f90: 416e 6365 7374 6f72 5f20 6973 2061 6e79  Ancestor_ is any
+00008fa0: 2072 656c 6174 6976 6520 6f66 2074 6865   relative of the
+00008fb0: 2065 7665 6e74 2075 7020 7468 6520 7472   event up the tr
+00008fc0: 6565 2028 6772 616e 6470 6172 656e 742c  ee (grandparent,
+00008fd0: 2070 6172 656e 7420 6574 632e 292e 0a20   parent etc.).. 
+00008fe0: 2020 2020 2020 2020 2020 2032 2e20 5f50             2. _P
+00008ff0: 6172 656e 745f 2069 7320 6f6e 6c79 2074  arent_ is only t
+00009000: 6865 2066 6972 7374 2072 656c 6174 6976  he first relativ
+00009010: 6520 6f66 2074 6865 2065 7665 6e74 2075  e of the event u
+00009020: 7020 7468 6520 7472 6565 2e0a 2020 2020  p the tree..    
+00009030: 2020 2020 2020 2020 332e 205f 4368 696c          3. _Chil
+00009040: 645f 2069 7320 7468 6520 6669 7273 7420  d_ is the first 
+00009050: 7265 6c61 7469 7665 206f 6620 7468 6520  relative of the 
+00009060: 6576 656e 7420 646f 776e 2074 6865 2074  event down the t
+00009070: 7265 652e 0a20 2020 2020 2020 200a 2020  ree..        .  
+00009080: 2020 2020 2020 5461 6b65 2061 206c 6f6f        Take a loo
+00009090: 6b20 6174 2074 6865 2066 6f6c 6c6f 7769  k at the followi
+000090a0: 6e67 2048 544d 4c20 7472 6565 2074 6f20  ng HTML tree to 
+000090b0: 756e 6465 7273 7461 6e64 2074 6865 6d2e  understand them.
+000090c0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000090d0: 2020 2020 2060 6060 0a20 2020 2020 2020       ```.       
+000090e0: 2020 2020 203c 626f 6479 3e20 3c21 2d2d       <body> <!--
+000090f0: 2061 6e63 6573 746f 7220 2867 7261 6e64   ancestor (grand
+00009100: 7061 7265 6e74 292c 2062 7574 206e 6f74  parent), but not
+00009110: 2070 6172 656e 7420 2d2d 3e0a 2020 2020   parent -->.    
+00009120: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00009130: 3e20 3c21 2d2d 2070 6172 656e 7420 2620  > <!-- parent & 
+00009140: 616e 6365 7374 6f72 202d 2d3e 0a20 2020  ancestor -->.   
+00009150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009160: 203c 703e 4865 6c6c 6f2c 2077 6f72 6c64   <p>Hello, world
+00009170: 213c 2f70 3e20 3c21 2d2d 2063 6869 6c64  !</p> <!-- child
+00009180: 202d 2d3e 0a20 2020 2020 2020 2020 2020   -->.           
+00009190: 2020 2020 2020 2020 203c 703e 476f 6f64           <p>Good
+000091a0: 6279 6521 3c2f 703e 203c 212d 2d20 7369  bye!</p> <!-- si
+000091b0: 626c 696e 6720 2d2d 3e0a 2020 2020 2020  bling -->.      
+000091c0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+000091d0: 0a20 2020 2020 2020 2020 2020 203c 2f62  .            </b
+000091e0: 6f64 793e 0a20 2020 2020 2020 2020 2020  ody>.           
+000091f0: 6060 600a 2020 2020 2020 2020 0a20 2020  ```.        .   
+00009200: 2020 2020 2023 2323 2320 436f 6c6c 6563       #### Collec
+00009210: 7469 6f6e 730a 2020 2020 2020 2020 0a20  tions.        . 
+00009220: 2020 2020 2020 202a 2a45 7665 6e74 5472         **EventTr
+00009230: 6565 436f 6c6c 6563 7469 6f6e 2a2a 2069  eeCollection** i
+00009240: 7320 6120 636f 6c6c 6563 7469 6f6e 206f  s a collection o
+00009250: 6620 4576 656e 7454 7265 6573 2e20 5468  f EventTrees. Th
+00009260: 6520 636f 6c6c 6563 7469 6f6e 2062 7569  e collection bui
+00009270: 6c64 7320 6120 6665 7720 5f45 7665 6e74  lds a few _Event
+00009280: 5472 6565 5f20 6279 2070 6173 7365 6420  Tree_ by passed 
+00009290: 5f44 6174 610a 2020 2020 2020 2020 6f62  _Data.        ob
+000092a0: 6a65 6374 5f2e 2041 6c74 686f 7567 6820  ject_. Although 
+000092b0: 796f 7520 6361 6e20 6368 616e 6765 2074  you can change t
+000092c0: 6865 2074 7265 6520 6469 7265 6374 6c79  he tree directly
+000092d0: 2c20 6974 2773 2062 6574 7465 7220 746f  , it's better to
+000092e0: 2064 6f20 6974 2074 6872 6f75 6768 2063   do it through c
+000092f0: 6f6c 6c65 6374 696f 6e73 2062 6563 6175  ollections becau
+00009300: 7365 2074 6865 7920 6172 6520 6177 6172  se they are awar
+00009310: 6520 6f66 0a20 2020 2020 2020 2060 6465  e of.        `de
+00009320: 7461 6368 6564 5f65 7665 6e74 7360 2061  tached_events` a
+00009330: 6e64 2063 616e 2073 6f6c 7665 2073 6f6d  nd can solve som
+00009340: 6520 6576 656e 7473 2064 6570 656e 6465  e events depende
+00009350: 6e63 6965 732e 2054 6865 2063 6f6c 6c65  ncies. The colle
+00009360: 6374 696f 6e20 6861 7320 7369 6d69 6c61  ction has simila
+00009370: 7220 6665 6174 7572 6573 206c 696b 6520  r features like 
+00009380: 6120 7369 6e67 6c65 205f 4576 656e 7454  a single _EventT
+00009390: 7265 655f 0a20 2020 2020 2020 2062 7574  ree_.        but
+000093a0: 2061 7070 6c79 696e 6720 7468 656d 2066   applying them f
+000093b0: 6f72 2061 6c6c 205f 4576 656e 7454 7265  or all _EventTre
+000093c0: 6573 5f2e 0a20 2020 2020 2020 200a 2020  es_..        .  
+000093d0: 2020 2020 2020 2a2a 5061 7265 6e74 4576        **ParentEv
+000093e0: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
+000093f0: 6e2a 2a20 6973 2061 2063 6f6c 6c65 6374  n** is a collect
+00009400: 696f 6e20 7369 6d69 6c61 7220 746f 205f  ion similar to _
+00009410: 4576 656e 7454 7265 6543 6f6c 6c65 6374  EventTreeCollect
+00009420: 696f 6e5f 2062 7574 2063 6f6e 7461 696e  ion_ but contain
+00009430: 696e 6720 6f6e 6c79 2070 6172 656e 7420  ing only parent 
+00009440: 6576 656e 7473 2074 6861 740a 2020 2020  events that.    
+00009450: 2020 2020 6172 6520 7265 6665 7265 6e63      are referenc
+00009460: 6564 2069 6e20 7468 6520 6461 7461 2073  ed in the data s
+00009470: 7472 6561 6d2e 2054 6865 2063 6f6c 6c65  tream. The colle
+00009480: 6374 696f 6e20 6861 7320 6665 6174 7572  ction has featur
+00009490: 6573 2073 696d 696c 6172 2074 6f20 5f45  es similar to _E
+000094a0: 7665 6e74 5472 6565 436f 6c6c 6563 7469  ventTreeCollecti
+000094b0: 6f6e 5f2e 0a20 2020 2020 2020 200a 2020  on_..        .  
+000094c0: 2020 2020 2020 4465 7461 696c 733a 0a20        Details:. 
+000094d0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000094e0: 2a20 546f 2075 7365 2045 5420 636f 6c6c  * To use ET coll
+000094f0: 6563 7469 6f6e 7320 796f 7520 6e65 6564  ections you need
+00009500: 2074 6f20 696e 6974 6961 6c69 7a65 2074   to initialize t
+00009510: 6865 6d20 6279 205f 4554 4344 7269 7665  hem by _ETCDrive
+00009520: 725f 2e20 4461 7461 2073 6f75 7263 6573  r_. Data sources
+00009530: 2075 7375 616c 6c79 2070 726f 7669 6465   usually provide
+00009540: 2074 6865 6d2e 0a20 2020 2020 2020 2020   them..         
+00009550: 2059 6f75 2063 616e 2063 7265 6174 6520   You can create 
+00009560: 6974 2062 7920 796f 7572 7365 6c66 2064  it by yourself d
+00009570: 6570 656e 6469 6e67 206f 6e20 796f 7572  epending on your
+00009580: 2064 6174 6120 7374 7275 6374 7572 652e   data structure.
+00009590: 0a20 2020 2020 2020 202a 2054 6865 2063  .        * The c
+000095a0: 6f6c 6c65 6374 696f 6e20 6861 7320 6120  ollection has a 
+000095b0: 6665 6174 7572 6520 746f 2072 6563 6f76  feature to recov
+000095c0: 6572 2065 7665 6e74 732e 2041 6c6c 2065  er events. All e
+000095d0: 7665 6e74 7320 7468 6174 2061 7265 206e  vents that are n
+000095e0: 6f74 2069 6e20 7468 6520 7265 6365 6976  ot in the receiv
+000095f0: 6564 2064 6174 6120 7374 7265 616d 2c20  ed data stream, 
+00009600: 6275 7420 7768 6963 6820 6172 650a 2020  but which are.  
+00009610: 2020 2020 2020 2020 7265 6665 7265 6e63          referenc
+00009620: 6564 2077 696c 6c20 6265 206c 6f61 6465  ed will be loade
+00009630: 6420 6672 6f6d 2074 6865 2064 6174 6120  d from the data 
+00009640: 736f 7572 6365 2e0a 2020 2020 2020 2020  source..        
+00009650: 2a20 596f 7520 6361 6e20 7461 6b65 2060  * You can take `
+00009660: 6465 7461 6368 6564 5f65 7665 6e74 7360  detached_events`
+00009670: 2074 6f20 7365 6520 7768 6963 6820 6576   to see which ev
+00009680: 656e 7473 2061 7265 206d 6973 7369 6e67  ents are missing
+00009690: 2e0a 2020 2020 2020 2020 2a20 4966 2079  ..        * If y
+000096a0: 6f75 2077 616e 742c 2079 6f75 2063 616e  ou want, you can
+000096b0: 2062 7569 6c64 2070 6172 656e 746c 6573   build parentles
+000096c0: 7320 7472 6565 7320 7768 6572 6520 7468  s trees where th
+000096d0: 6520 6d69 7373 696e 6720 6576 656e 7473  e missing events
+000096e0: 2061 7265 2073 7475 6262 6564 2069 6e73   are stubbed ins
+000096f0: 7465 6164 2e20 4a75 7374 0a20 2020 2020  tead. Just.     
+00009700: 2020 2020 2075 7365 2060 6765 745f 7061       use `get_pa
+00009710: 7265 6e74 6c65 7373 5f74 7265 6573 2829  rentless_trees()
+00009720: 602e 0a20 2020 2020 2020 200a 2020 2020  `..        .    
+00009730: 2020 2020 5265 7175 6972 656d 656e 7473      Requirements
+00009740: 3a0a 2020 2020 2020 2020 0a20 2020 2020  :.        .     
+00009750: 2020 2031 2e20 4576 656e 7473 2070 726f     1. Events pro
+00009760: 7669 6465 6420 746f 2045 5443 2068 6176  vided to ETC hav
+00009770: 6520 746f 2068 6176 6520 6065 7665 6e74  e to have `event
+00009780: 5f6e 616d 6560 2c20 6065 7665 6e74 5f69  _name`, `event_i
+00009790: 6460 2c20 6070 6172 656e 745f 6576 656e  d`, `parent_even
+000097a0: 745f 6964 6020 6669 656c 6473 2e20 5468  t_id` fields. Th
+000097b0: 6579 0a20 2020 2020 2020 2063 616e 2068  ey.        can h
+000097c0: 6176 6520 616e 6f74 6865 7220 6e61 6d65  ave another name
+000097d0: 7320 2869 7420 7265 736f 6c76 6573 2069  s (it resolves i
+000097e0: 6e20 7468 6520 6472 6976 6572 292e 0a20  n the driver).. 
+000097f0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00009800: 2323 2323 2048 696e 7473 0a20 2020 2020  #### Hints.     
+00009810: 2020 200a 2020 2020 2020 2020 2a20 5265     .        * Re
+00009820: 6d6f 7665 2061 6c6c 2075 6e6e 6563 6573  move all unneces
+00009830: 7361 7279 2066 6965 6c64 7320 6672 6f6d  sary fields from
+00009840: 2065 7665 6e74 7320 6265 666f 7265 2070   events before p
+00009850: 6173 7369 6e67 2074 6f20 6120 5f63 6f6c  assing to a _col
+00009860: 6c65 6374 696f 6e5f 2074 6f20 7265 6475  lection_ to redu
+00009870: 6365 206d 656d 6f72 7920 7573 6167 652e  ce memory usage.
+00009880: 0a20 2020 2020 2020 202a 2055 7365 2060  .        * Use `
+00009890: 7368 6f77 2829 6020 6d65 7468 6f64 2074  show()` method t
+000098a0: 6f20 7072 696e 7420 7468 6520 7472 6565  o print the tree
+000098b0: 2069 6e20 7472 6565 2d6c 696b 6520 7669   in tree-like vi
+000098c0: 6577 2e0a 2020 2020 2020 2020 2a20 4e6f  ew..        * No
+000098d0: 7465 2074 6861 7420 7468 6520 6067 6574  te that the `get
+000098e0: 5f78 6020 6d65 7468 6f64 7320 7769 6c6c  _x` methods will
+000098f0: 2072 6169 7365 2061 6e20 6578 6365 7074   raise an except
+00009900: 696f 6e20 6966 2079 6f75 2070 6173 7320  ion if you pass 
+00009910: 616e 2075 6e6b 6e6f 776e 2065 7665 6e74  an unknown event
+00009920: 2069 642c 2075 6e6c 696b 6520 7468 6520   id, unlike the 
+00009930: 6066 696e 645f 7860 206d 6574 686f 6473  `find_x` methods
+00009940: 2028 0a20 2020 2020 2020 2020 2074 6865   (.          the
+00009950: 7920 7265 7475 726e 204e 6f6e 6529 2e0a  y return None)..
+00009960: 2020 2020 2020 2020 2a20 4966 2079 6f75          * If you
+00009970: 2077 616e 7420 746f 206b 6e6f 7720 7468   want to know th
+00009980: 6174 2073 7065 6369 6669 6564 2065 7665  at specified eve
+00009990: 6e74 2065 7869 7374 732c 2075 7365 2074  nt exists, use t
+000099a0: 6865 2070 7974 686f 6e20 6069 6e60 206b  he python `in` k
+000099b0: 6579 776f 7264 2028 652e 672e 2060 2765  eyword (e.g. `'e
+000099c0: 7665 6e74 2d69 6427 2069 6e20 6576 656e  vent-id' in even
+000099d0: 7473 5f74 7265 6560 292e 0a20 2020 2020  ts_tree`)..     
+000099e0: 2020 202a 2055 7365 2074 6865 2070 7974     * Use the pyt
+000099f0: 686f 6e20 606c 656e 6020 6b65 7977 6f72  hon `len` keywor
+00009a00: 6420 746f 2067 6574 2065 7665 6e74 7320  d to get events 
+00009a10: 6e75 6d62 6572 2069 6e20 7468 6520 7472  number in the tr
+00009a20: 6565 2e0a 2020 2020 2020 2020 0a20 2020  ee..        .   
+00009a30: 2020 2020 2023 2323 2046 6965 6c64 2052       ### Field R
+00009a40: 6573 6f6c 7665 7273 0a20 2020 2020 2020  esolvers.       
+00009a50: 2049 6e74 6572 6661 6365 2063 616e 2062   Interface can b
+00009a60: 6520 666f 756e 6420 696e 2060 7468 325f  e found in `th2_
+00009a70: 6461 7461 5f73 6572 7669 6365 732f 696e  data_services/in
+00009a80: 7465 7266 6163 6573 2f75 7469 6c73 2f72  terfaces/utils/r
+00009a90: 6573 6f6c 7665 722e 7079 602e 2020 0a20  esolver.py`.  . 
+00009aa0: 2020 2020 2020 2041 6c6c 2064 6174 612d         All data-
+00009ab0: 736f 7572 6365 7320 7368 6f75 6c64 2069  sources should i
+00009ac0: 6d70 6c65 6d65 6e74 2074 6865 6d2e 0a20  mplement them.. 
+00009ad0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00009ae0: 5468 6520 6964 6561 206f 6620 7573 696e  The idea of usin
+00009af0: 6720 7265 736f 6c76 6572 733a 0a20 2020  g resolvers:.   
+00009b00: 2020 2020 2049 7420 736f 6c76 6573 2074       It solves t
+00009b10: 6865 2070 726f 626c 656d 206f 6620 6861  he problem of ha
+00009b20: 7669 6e67 2061 2066 6577 2044 6174 6153  ving a few DataS
+00009b30: 6f75 7263 6573 2077 6974 6820 7369 6d69  ources with simi
+00009b40: 6c61 7220 6461 7461 2c0a 2020 2020 2020  lar data,.      
+00009b50: 2020 6275 7420 7769 7468 2064 6966 6665    but with diffe
+00009b60: 7265 6e74 2077 6179 7320 746f 2067 6574  rent ways to get
+00009b70: 2069 742e 0a20 2020 2020 2020 200a 2020   it..        .  
+00009b80: 2020 2020 2020 5468 6573 6520 636c 6173        These clas
+00009b90: 7365 7320 7072 6f76 6964 6520 796f 7520  ses provide you 
+00009ba0: 6765 7474 6572 206d 6574 686f 6473 2e0a  getter methods..
+00009bb0: 2020 2020 2020 2020 5573 696e 6720 7468          Using th
+00009bc0: 6573 6520 636c 6173 7365 7320 616c 6c6f  ese classes allo
+00009bd0: 7773 2079 6f75 2074 6f20 6672 6565 6c79  ws you to freely
+00009be0: 2073 7769 7463 6820 6265 7477 6565 6e20   switch between 
+00009bf0: 6469 6666 6572 656e 7420 6461 7461 0a20  different data. 
+00009c00: 2020 2020 2020 2066 6f72 6d61 7473 2061         formats a
+00009c10: 6e64 2064 6f6e 2774 2063 6861 6e67 6520  nd don't change 
+00009c20: 796f 7572 2063 6f64 652e 0a20 2020 2020  your code..     
+00009c30: 2020 200a 2020 2020 2020 2020 5265 736f     .        Reso
+00009c40: 6c76 6572 7320 736f 6c76 6520 7468 6520  lvers solve the 
+00009c50: 7072 6f62 6c65 6d20 6f66 2064 6174 612d  problem of data-
+00009c60: 666f 726d 6174 206d 6967 7261 7469 6f6e  format migration
+00009c70: 2e0a 2020 2020 2020 2020 2d20 6669 656c  ..        - fiel
+00009c80: 6473 2070 6c61 6365 2063 616e 2062 6520  ds place can be 
+00009c90: 6368 616e 6765 640a 2020 2020 2020 2020  changed.        
+00009ca0: 2d20 6669 656c 6473 206e 616d 6573 2063  - fields names c
+00009cb0: 616e 2062 6520 6368 616e 6765 640a 2020  an be changed.  
+00009cc0: 2020 2020 2020 0a20 2020 2020 2020 2052        .        R
+00009cd0: 6573 6f6c 7665 7273 2063 616e 2077 6f72  esolvers can wor
+00009ce0: 6b20 6f6e 6c79 2077 6974 6820 6f6e 6520  k only with one 
+00009cf0: 6576 656e 742f 6d65 7373 6167 652e 0a20  event/message.. 
+00009d00: 2020 2020 2020 2049 7420 6d65 616e 732c         It means,
+00009d10: 2069 6620 796f 7572 206d 6573 7361 6765   if your message
+00009d20: 2068 6173 2073 7562 2d6d 6573 7361 6765   has sub-message
+00009d30: 7320 286c 696b 6520 7468 322d 6d65 7373  s (like th2-mess
+00009d40: 6167 6573 2069 6e20 6c77 6470 2920 6974  ages in lwdp) it
+00009d50: 200a 2020 2020 2020 2020 776f 6e27 7420   .        won't 
+00009d60: 776f 726b 2c20 6265 6361 7573 6520 7265  work, because re
+00009d70: 736f 6c76 6572 2077 696c 6c20 6e6f 7420  solver will not 
+00009d80: 6b6e 6f77 2077 6974 6820 7768 6963 6820  know with which 
+00009d90: 7375 622d 6d65 7373 6167 6520 7368 6f75  sub-message shou
+00009da0: 6c64 2069 7420 776f 726b 2e20 0a20 2020  ld it work. .   
+00009db0: 2020 2020 200a 2020 2020 2020 2020 2a2a       .        **
+00009dc0: 576f 726b 6172 6f75 6e64 2a2a 2020 0a20  Workaround**  . 
+00009dd0: 2020 2020 2020 2031 2e20 4578 7061 6e64         1. Expand
+00009de0: 2061 6c6c 2079 6f75 7220 6d65 7373 6167   all your messag
+00009df0: 6573 202d 3e20 606e 6577 5f64 203d 2079  es -> `new_d = y
+00009e00: 6f75 725f 6461 7461 2e6d 6170 284d 6573  our_data.map(Mes
+00009e10: 7361 6765 4669 656c 6452 6573 6f6c 7665  sageFieldResolve
+00009e20: 722e 6578 7061 6e64 5f6d 6573 7361 6765  r.expand_message
+00009e30: 2960 0a20 2020 2020 2020 2032 2e20 5573  )`.        2. Us
+00009e40: 6520 6045 7870 616e 6465 644d 6573 7361  e `ExpandedMessa
+00009e50: 6765 4669 656c 6452 6573 6f6c 7665 7260  geFieldResolver`
+00009e60: 2069 6e73 7465 6164 206f 6620 7573 7561   instead of usua
+00009e70: 6c20 604d 6573 7361 6765 4669 656c 6452  l `MessageFieldR
+00009e80: 6573 6f6c 7665 7260 2077 6865 6e20 0a20  esolver` when . 
+00009e90: 2020 2020 2020 2020 2020 2079 6f75 2074             you t
+00009ea0: 616b 6520 6669 656c 6473 2066 6f72 2065  ake fields for e
+00009eb0: 7870 616e 6465 6420 6d65 7373 6167 6573  xpanded messages
+00009ec0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00009ed0: 2020 202a 2a49 6d70 6c65 6d65 6e74 6174     **Implementat
+00009ee0: 696f 6e20 6164 7669 6365 3a2a 2a0a 2020  ion advice:**.  
+00009ef0: 2020 2020 2020 312e 2072 6169 7365 204e        1. raise N
+00009f00: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
+00009f10: 6f72 202d 2d20 6966 2079 6f75 7220 496d  or -- if your Im
+00009f20: 706c 656d 656e 7461 7469 6f6e 2064 6f65  plementation doe
+00009f30: 736e 2774 2073 7570 706f 7274 2074 6869  sn't support thi
+00009f40: 7320 6765 7474 6572 2e0a 2020 2020 2020  s getter..      
+00009f50: 2020 0a20 2020 2020 2020 202a 2a50 6572    .        **Per
+00009f60: 666f 726d 616e 6365 2069 6d70 6163 743a  formance impact:
+00009f70: 2a2a 0a20 2020 2020 2020 202d 2049 7420  **.        - It 
+00009f80: 6120 6269 7420 736c 6f77 6572 2074 6861  a bit slower tha
+00009f90: 6e20 7573 696e 6720 6e61 6b65 6420 6669  n using naked fi
+00009fa0: 656c 6420 6163 6365 7373 2060 6469 6374  eld access `dict
+00009fb0: 5b27 6b65 7927 5d60 2e0a 2020 2020 2020  ['key']`..      
+00009fc0: 2020 0a20 2020 2020 2020 2023 2320 322e    .        ## 2.
+00009fd0: 342e 204c 696e 6b73 0a20 2020 2020 2020  4. Links.       
+00009fe0: 200a 2020 2020 2020 2020 2d20 5b52 6570   .        - [Rep
+00009ff0: 6f72 7420 4461 7461 2050 726f 7669 6465  ort Data Provide
+0000a000: 725d 2868 7474 7073 3a2f 2f67 6974 6875  r](https://githu
+0000a010: 622e 636f 6d2f 7468 322d 6e65 742f 7468  b.com/th2-net/th
+0000a020: 322d 7270 742d 6461 7461 2d70 726f 7669  2-rpt-data-provi
+0000a030: 6465 7229 0a20 2020 2020 2020 202d 205b  der).        - [
+0000a040: 5468 3220 4461 7461 2053 6572 7669 6365  Th2 Data Service
+0000a050: 7320 5574 696c 735d 2868 7474 7073 3a2f  s Utils](https:/
+0000a060: 2f67 6974 6875 622e 636f 6d2f 7468 322d  /github.com/th2-
+0000a070: 6e65 742f 7468 322d 6461 7461 2d73 6572  net/th2-data-ser
+0000a080: 7669 6365 732d 7574 696c 7329 0a20 2020  vices-utils).   
+0000a090: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+0000a0a0: 332e 2042 6573 7420 7072 6163 7469 6365  3. Best practice
+0000a0b0: 730a 2020 2020 2020 2020 4465 7065 6e64  s.        Depend
+0000a0c0: 696e 6720 6f6e 2068 6f77 2079 6f75 2077  ing on how you w
+0000a0d0: 6f72 6b20 7769 7468 2060 4461 7461 206f  ork with `Data o
+0000a0e0: 626a 6563 7460 2c20 6974 2063 616e 2062  bject`, it can b
+0000a0f0: 6520 736c 6f77 206f 6620 6661 7374 2e0a  e slow of fast..
+0000a100: 2020 2020 2020 2020 4173 2077 6974 6820          As with 
+0000a110: 6120 7265 6c61 7469 6f6e 616c 2064 6174  a relational dat
+0000a120: 6162 6173 652c 2079 6f75 2063 616e 2077  abase, you can w
+0000a130: 7269 7465 2061 2071 7565 7279 2074 6861  rite a query tha
+0000a140: 7420 7769 6c6c 2072 6574 7572 6e20 6461  t will return da
+0000a150: 7461 2073 6c6f 776c 7920 6f72 2071 7569  ta slowly or qui
+0000a160: 636b 6c79 2c0a 2020 2020 2020 2020 7468  ckly,.        th
+0000a170: 6520 7361 6d65 2077 6865 6e20 776f 726b  e same when work
+0000a180: 696e 6720 7769 7468 2061 2060 4461 7461  ing with a `Data
+0000a190: 206f 626a 6563 7460 2e0a 2020 2020 2020   object`..      
+0000a1a0: 2020 0a20 2020 2020 2020 2046 6f6c 6c6f    .        Follo
+0000a1b0: 7720 7468 6520 7275 6c65 7320 746f 206d  w the rules to m
+0000a1c0: 616b 6520 796f 7572 2077 6f72 6b20 7769  ake your work wi
+0000a1d0: 7468 2044 6174 6120 6f62 6a65 6374 2066  th Data object f
+0000a1e0: 6173 743a 0a20 2020 2020 2020 2031 2e20  ast:.        1. 
+0000a1f0: 5573 6520 6044 6174 612e 7573 655f 6361  Use `Data.use_ca
+0000a200: 6368 6528 2960 2069 6620 796f 7520 6974  che()` if you it
+0000a210: 6572 6174 6520 6461 7461 206d 6f72 6520  erate data more 
+0000a220: 7468 616e 206f 6e65 2074 696d 652e 0a20  than one time.. 
+0000a230: 2020 2020 2020 2032 2e20 5472 7920 746f         2. Try to
+0000a240: 2064 6f6e 2774 2069 7465 7261 7465 206f   don't iterate o
+0000a250: 6e65 2060 4461 7461 206f 626a 6563 7460  ne `Data object`
+0000a260: 2069 6e73 6964 6520 7468 6520 6f74 6865   inside the othe
+0000a270: 7220 6f6e 652e 0a20 2020 2020 2020 2020  r one..         
+0000a280: 2020 4966 2079 6f75 2073 686f 756c 6420    If you should 
+0000a290: 746f 2064 6f20 6974 2c20 7573 6520 7368  to do it, use sh
+0000a2a0: 6f72 7420 6044 6174 6120 6f62 6a65 6374  ort `Data object
+0000a2b0: 6020 6669 7273 7420 616e 6420 6c6f 6e67  ` first and long
+0000a2c0: 2060 4461 7461 206f 626a 6563 7460 2069   `Data object` i
+0000a2d0: 6e73 6964 6520 7468 6520 6c6f 6f70 2e0a  nside the loop..
+0000a2e0: 2020 2020 2020 2020 2020 2049 7427 6c6c             It'll
+0000a2f0: 2061 6c6c 6f77 2079 6f75 206f 7065 6e20   allow you open 
+0000a300: 7468 6520 6361 6368 6520 6669 6c65 206f  the cache file o
+0000a310: 7220 6372 6561 7465 2061 2072 6571 7565  r create a reque
+0000a320: 7374 2074 6f20 6044 6174 6120 736f 7572  st to `Data sour
+0000a330: 6365 6020 6c65 7373 206e 756d 6265 7220  ce` less number 
+0000a340: 6f66 2074 696d 6573 2e0a 2020 2020 2020  of times..      
+0000a350: 2020 0a20 2020 2020 2020 2023 2034 2e20    .        # 4. 
+0000a360: 4f66 6669 6369 616c 2044 6174 6153 6f75  Official DataSou
+0000a370: 7263 6520 696d 706c 656d 656e 7461 7469  rce implementati
+0000a380: 6f6e 730a 2020 2020 2020 2020 0a20 2020  ons.        .   
+0000a390: 2020 2020 202d 205b 4c69 6768 7477 6569       - [Lightwei
+0000a3a0: 6768 7420 4461 7461 2050 726f 7669 6465  ght Data Provide
+0000a3b0: 7220 4461 7461 2053 6f75 7263 655d 2868  r Data Source](h
+0000a3c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0000a3d0: 6d2f 7468 322d 6e65 742f 7468 322d 6473  m/th2-net/th2-ds
+0000a3e0: 2d73 6f75 7263 652d 6c77 6470 290a 2020  -source-lwdp).  
+0000a3f0: 2020 2020 2020 0a20 2020 2020 2020 200a        .        .
+0000a400: 2020 2020 2020 2020 2320 352e 2041 5049          # 5. API
+0000a410: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+0000a420: 2020 4966 2079 6f75 2061 7265 206c 6f6f    If you are loo
+0000a430: 6b69 6e67 2066 6f72 2063 6c61 7373 6573  king for classes
+0000a440: 2064 6573 6372 6970 7469 6f6e 2073 6565   description see
+0000a450: 2074 6865 205b 4150 4920 446f 6375 6d65   the [API Docume
+0000a460: 6e74 6174 696f 6e5d 2864 6f63 756d 656e  ntation](documen
+0000a470: 7461 7469 6f6e 2f61 7069 2f69 6e64 6578  tation/api/index
+0000a480: 2e6d 6429 2e0a 2020 2020 2020 2020 0a20  .md)..        . 
+0000a490: 2020 2020 2020 2023 2036 2e20 4578 616d         # 6. Exam
+0000a4a0: 706c 6573 0a20 2020 2020 2020 200a 2020  ples.        .  
+0000a4b0: 2020 2020 2020 2d20 5b67 6574 5f73 7461        - [get_sta
+0000a4c0: 7274 6564 5f65 7861 6d70 6c65 2e70 795d  rted_example.py]
+0000a4d0: 2865 7861 6d70 6c65 732f 6765 745f 7374  (examples/get_st
+0000a4e0: 6172 7465 645f 6578 616d 706c 652e 7079  arted_example.py
+0000a4f0: 290a 2020 2020 2020 2020 0a50 6c61 7466  ).        .Platf
+0000a500: 6f72 6d3a 2055 4e4b 4e4f 574e 0a52 6571  orm: UNKNOWN.Req
+0000a510: 7569 7265 732d 5079 7468 6f6e 3a20 3e3d  uires-Python: >=
+0000a520: 332e 370a 4465 7363 7269 7074 696f 6e2d  3.7.Description-
+0000a530: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
+0000a540: 7874 2f6d 6172 6b64 6f77 6e0a 5072 6f76  xt/markdown.Prov
+0000a550: 6964 6573 2d45 7874 7261 3a20 7264 700a  ides-Extra: rdp.
+0000a560: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+0000a570: 7264 7035 0a50 726f 7669 6465 732d 4578  rdp5.Provides-Ex
+0000a580: 7472 613a 2072 6470 360a 5072 6f76 6964  tra: rdp6.Provid
+0000a590: 6573 2d45 7874 7261 3a20 6c77 6470 0a50  es-Extra: lwdp.P
+0000a5a0: 726f 7669 6465 732d 4578 7472 613a 206c  rovides-Extra: l
+0000a5b0: 7764 7031 0a50 726f 7669 6465 732d 4578  wdp1.Provides-Ex
+0000a5c0: 7472 613a 206c 7764 7032 0a50 726f 7669  tra: lwdp2.Provi
+0000a5d0: 6465 732d 4578 7472 613a 206c 7764 7033  des-Extra: lwdp3
+0000a5e0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
+0000a5f0: 206c 7764 702d 6465 760a 5072 6f76 6964   lwdp-dev.Provid
+0000a600: 6573 2d45 7874 7261 3a20 7574 696c 732d  es-Extra: utils-
+0000a610: 7270 742d 7669 6577 6572 0a50 726f 7669  rpt-viewer.Provi
+0000a620: 6465 732d 4578 7472 613a 2075 7469 6c73  des-Extra: utils
+0000a630: 2d72 7074 2d76 6965 7765 7235 0a50 726f  -rpt-viewer5.Pro
+0000a640: 7669 6465 732d 4578 7472 613a 2075 7469  vides-Extra: uti
+0000a650: 6c73 2d61 6476 616e 6365 640a            ls-advanced.
```

### Comparing `th2_data_services-2.0.0.dev8662586819/README.md` & `th2_data_services-2.0.0.dev8702324290/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -239,1613 +239,1953 @@
 00000ee0: 706c 652c 204c 6973 742c 204f 7074 696f  ple, List, Optio
 00000ef0: 6e61 6c2c 2047 656e 6572 6174 6f72 0a66  nal, Generator.f
 00000f00: 726f 6d20 6461 7465 7469 6d65 2069 6d70  rom datetime imp
 00000f10: 6f72 7420 6461 7465 7469 6d65 0a0a 6672  ort datetime..fr
 00000f20: 6f6d 2074 6832 5f64 6174 615f 7365 7276  om th2_data_serv
 00000f30: 6963 6573 2e64 6174 6120 696d 706f 7274  ices.data import
 00000f40: 2044 6174 610a 6672 6f6d 2074 6832 5f64   Data.from th2_d
-00000f50: 6174 615f 7365 7276 6963 6573 2e65 7665  ata_services.eve
-00000f60: 6e74 5f74 7265 6520 696d 706f 7274 2028  nt_tree import (
-00000f70: 0a20 2020 2045 7665 6e74 5472 6565 2c0a  .    EventTree,.
-00000f80: 2020 2020 4576 656e 7454 7265 6543 6f6c      EventTreeCol
-00000f90: 6c65 6374 696f 6e2c 0a20 2020 2050 6172  lection,.    Par
-00000fa0: 656e 7445 7665 6e74 5472 6565 436f 6c6c  entEventTreeColl
-00000fb0: 6563 7469 6f6e 2c0a 2020 2020 4945 5443  ection,.    IETC
-00000fc0: 4472 6976 6572 2c0a 290a 6672 6f6d 2074  Driver,.).from t
-00000fd0: 6832 5f64 6174 615f 7365 7276 6963 6573  h2_data_services
-00000fe0: 2e69 6e74 6572 6661 6365 7320 696d 706f  .interfaces impo
-00000ff0: 7274 2049 4461 7461 536f 7572 6365 0a66  rt IDataSource.f
-00001000: 726f 6d20 7468 325f 6461 7461 5f73 6572  rom th2_data_ser
-00001010: 7669 6365 732e 7574 696c 732e 636f 6e76  vices.utils.conv
-00001020: 6572 7465 7273 2069 6d70 6f72 7420 280a  erters import (.
-00001030: 2020 2020 4461 7465 7469 6d65 436f 6e76      DatetimeConv
-00001040: 6572 7465 722c 0a20 2020 2044 6174 6574  erter,.    Datet
-00001050: 696d 6553 7472 696e 6743 6f6e 7665 7274  imeStringConvert
-00001060: 6572 2c0a 2020 2020 5072 6f74 6f62 7566  er,.    Protobuf
-00001070: 5469 6d65 7374 616d 7043 6f6e 7665 7274  TimestampConvert
-00001080: 6572 2c0a 2020 2020 5468 3254 696d 6573  er,.    Th2Times
-00001090: 7461 6d70 436f 6e76 6572 7465 722c 0a29  tampConverter,.)
-000010a0: 0a0a 2320 5b30 5d20 4c69 6220 636f 6e66  ..# [0] Lib conf
-000010b0: 6967 7572 6174 696f 6e0a 2320 5b30 2e31  iguration.# [0.1
-000010c0: 5d20 496e 7465 7261 6374 6976 6520 6f72  ] Interactive or
-000010d0: 2053 6372 6970 7420 6d6f 6465 0a23 2049   Script mode.# I
-000010e0: 6620 796f 7520 7573 6520 7468 6520 6c69  f you use the li
-000010f0: 6220 696e 2069 6e74 6572 6163 7469 7665  b in interactive
-00001100: 206d 6f64 6520 286a 7570 7974 6572 2c20   mode (jupyter, 
-00001110: 6970 7974 686f 6e29 2069 7427 7320 7265  ipython) it's re
-00001120: 636f 6d6d 656e 6465 6420 746f 2073 6574  commended to set
-00001130: 2074 6865 2073 7065 6369 616c 0a23 2067   the special.# g
-00001140: 6c6f 6261 6c20 7061 7261 6d65 7465 7220  lobal parameter 
-00001150: 746f 2054 7275 652e 2049 7427 6c6c 206b  to True. It'll k
-00001160: 6565 7020 6361 6368 6520 6669 6c65 7320  eep cache files 
-00001170: 6966 2073 6f6d 6574 6869 6e67 2077 656e  if something wen
-00001180: 7420 7772 6f6e 672e 0a66 726f 6d20 7468  t wrong..from th
-00001190: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
-000011a0: 636f 6e66 6967 2069 6d70 6f72 7420 6f70  config import op
-000011b0: 7469 6f6e 730a 0a6f 7074 696f 6e73 2e49  tions..options.I
-000011c0: 4e54 4552 4143 5449 5645 5f4d 4f44 4520  NTERACTIVE_MODE 
-000011d0: 3d20 5472 7565 0a0a 2320 536f 6d65 2065  = True..# Some e
-000011e0: 7861 6d70 6c65 2064 6174 610a 6576 656e  xample data.even
-000011f0: 7473 203d 2044 6174 6128 0a20 2020 205b  ts = Data(.    [
-00001200: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
-00001210: 2020 2020 2020 2022 6576 656e 7449 6422         "eventId"
-00001220: 3a20 2264 656d 6f5f 626f 6f6b 5f31 3a74  : "demo_book_1:t
-00001230: 6832 2d73 636f 7065 3a32 3032 3330 3130  h2-scope:2023010
-00001240: 3531 3335 3730 3535 3630 3837 3330 3030  5135705560873000
-00001250: 3a64 3631 6539 3330 612d 3864 3030 2d31  :d61e930a-8d00-1
-00001260: 3165 642d 6161 3161 2d64 3334 6136 3135  1ed-aa1a-d34a615
-00001270: 3531 3532 645f 3122 2c0a 2020 2020 2020  5152d_1",.      
-00001280: 2020 2020 2020 2262 6174 6368 4964 223a        "batchId":
-00001290: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-000012a0: 2020 2022 6973 4261 7463 6865 6422 3a20     "isBatched": 
-000012b0: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
-000012c0: 2020 2022 6576 656e 744e 616d 6522 3a20     "eventName": 
-000012d0: 2253 6574 206f 6620 6175 746f 2d67 656e  "Set of auto-gen
-000012e0: 6572 6174 6564 2065 7665 6e74 7320 666f  erated events fo
-000012f0: 7220 6473 206c 6962 2074 6573 7469 6e67  r ds lib testing
-00001300: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00001310: 6576 656e 7454 7970 6522 3a20 2264 732d  eventType": "ds-
-00001320: 6c69 622d 7465 7374 2d65 7665 6e74 222c  lib-test-event",
-00001330: 0a20 2020 2020 2020 2020 2020 2022 656e  .            "en
-00001340: 6454 696d 6573 7461 6d70 223a 207b 2265  dTimestamp": {"e
-00001350: 706f 6368 5365 636f 6e64 223a 2031 3637  pochSecond": 167
-00001360: 3239 3237 3032 352c 2022 6e61 6e6f 223a  2927025, "nano":
-00001370: 2035 3631 3735 3130 3030 7d2c 0a20 2020   561751000},.   
-00001380: 2020 2020 2020 2020 2022 7374 6172 7454           "startT
-00001390: 696d 6573 7461 6d70 223a 207b 2265 706f  imestamp": {"epo
-000013a0: 6368 5365 636f 6e64 223a 2031 3637 3239  chSecond": 16729
-000013b0: 3237 3032 352c 2022 6e61 6e6f 223a 2035  27025, "nano": 5
-000013c0: 3630 3837 3330 3030 7d2c 0a20 2020 2020  60873000},.     
-000013d0: 2020 2020 2020 2022 7061 7265 6e74 4576         "parentEv
-000013e0: 656e 7449 6422 3a20 4e6f 6e65 2c0a 2020  entId": None,.  
-000013f0: 2020 2020 2020 2020 2020 2273 7563 6365            "succe
-00001400: 7373 6675 6c22 3a20 5472 7565 2c0a 2020  ssful": True,.  
-00001410: 2020 2020 2020 2020 2020 2262 6f6f 6b49            "bookI
-00001420: 6422 3a20 2264 656d 6f5f 626f 6f6b 5f31  d": "demo_book_1
-00001430: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00001440: 7363 6f70 6522 3a20 2274 6832 2d73 636f  scope": "th2-sco
-00001450: 7065 222c 0a20 2020 2020 2020 2020 2020  pe",.           
-00001460: 2022 6174 7461 6368 6564 4d65 7373 6167   "attachedMessag
-00001470: 6549 6473 223a 205b 5d2c 0a20 2020 2020  eIds": [],.     
-00001480: 2020 2020 2020 2022 626f 6479 223a 205b         "body": [
-00001490: 5d2c 0a20 2020 2020 2020 207d 2c0a 2020  ],.        },.  
-000014a0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-000014b0: 2020 2020 2265 7665 6e74 4964 223a 2022      "eventId": "
-000014c0: 6465 6d6f 5f62 6f6f 6b5f 313a 7468 322d  demo_book_1:th2-
-000014d0: 7363 6f70 653a 3230 3233 3031 3035 3133  scope:2023010513
-000014e0: 3537 3035 3536 3335 3232 3030 303a 3961  5705563522000:9a
-000014f0: 6462 6233 6530 2d35 6638 622d 3463 3238  dbb3e0-5f8b-4c28
-00001500: 2d61 3261 632d 3733 3631 6538 6661 3730  -a2ac-7361e8fa70
-00001510: 3463 3e64 656d 6f5f 626f 6f6b 5f31 3a74  4c>demo_book_1:t
-00001520: 6832 2d73 636f 7065 3a32 3032 3330 3130  h2-scope:2023010
-00001530: 3531 3335 3730 3535 3633 3532 3230 3030  5135705563522000
-00001540: 3a64 3631 6539 3330 612d 3864 3030 2d31  :d61e930a-8d00-1
-00001550: 3165 642d 6161 3161 2d64 3334 6136 3135  1ed-aa1a-d34a615
-00001560: 3531 3532 645f 3222 2c0a 2020 2020 2020  5152d_2",.      
-00001570: 2020 2020 2020 2262 6174 6368 4964 223a        "batchId":
-00001580: 2022 6465 6d6f 5f62 6f6f 6b5f 313a 7468   "demo_book_1:th
-00001590: 322d 7363 6f70 653a 3230 3233 3031 3035  2-scope:20230105
-000015a0: 3133 3537 3035 3536 3335 3232 3030 303a  135705563522000:
-000015b0: 3961 6462 6233 6530 2d35 6638 622d 3463  9adbb3e0-5f8b-4c
-000015c0: 3238 2d61 3261 632d 3733 3631 6538 6661  28-a2ac-7361e8fa
-000015d0: 3730 3463 222c 0a20 2020 2020 2020 2020  704c",.         
-000015e0: 2020 2022 6973 4261 7463 6865 6422 3a20     "isBatched": 
-000015f0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-00001600: 2020 2265 7665 6e74 4e61 6d65 223a 2022    "eventName": "
-00001610: 506c 6169 6e20 6576 656e 7420 3122 2c0a  Plain event 1",.
-00001620: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
-00001630: 6e74 5479 7065 223a 2022 6473 2d6c 6962  ntType": "ds-lib
-00001640: 2d74 6573 742d 6576 656e 7422 2c0a 2020  -test-event",.  
-00001650: 2020 2020 2020 2020 2020 2265 6e64 5469            "endTi
-00001660: 6d65 7374 616d 7022 3a20 7b22 6570 6f63  mestamp": {"epoc
-00001670: 6853 6563 6f6e 6422 3a20 3136 3732 3932  hSecond": 167292
-00001680: 3730 3235 2c20 226e 616e 6f22 3a20 3536  7025, "nano": 56
-00001690: 3336 3430 3030 307d 2c0a 2020 2020 2020  3640000},.      
-000016a0: 2020 2020 2020 2273 7461 7274 5469 6d65        "startTime
-000016b0: 7374 616d 7022 3a20 7b22 6570 6f63 6853  stamp": {"epochS
-000016c0: 6563 6f6e 6422 3a20 3136 3732 3932 3730  econd": 16729270
-000016d0: 3235 2c20 226e 616e 6f22 3a20 3536 3335  25, "nano": 5635
-000016e0: 3232 3030 307d 2c0a 2020 2020 2020 2020  22000},.        
-000016f0: 2020 2020 2270 6172 656e 7445 7665 6e74      "parentEvent
-00001700: 4964 223a 2022 6465 6d6f 5f62 6f6f 6b5f  Id": "demo_book_
-00001710: 313a 7468 322d 7363 6f70 653a 3230 3233  1:th2-scope:2023
-00001720: 3031 3035 3133 3537 3035 3536 3038 3733  0105135705560873
-00001730: 3030 303a 6436 3165 3933 3061 2d38 6430  000:d61e930a-8d0
-00001740: 302d 3131 6564 2d61 6131 612d 6433 3461  0-11ed-aa1a-d34a
-00001750: 3631 3535 3135 3264 5f31 222c 0a20 2020  6155152d_1",.   
-00001760: 2020 2020 2020 2020 2022 7375 6363 6573           "succes
-00001770: 7366 756c 223a 2054 7275 652c 0a20 2020  sful": True,.   
-00001780: 2020 2020 2020 2020 2022 626f 6f6b 4964           "bookId
-00001790: 223a 2022 6465 6d6f 5f62 6f6f 6b5f 3122  ": "demo_book_1"
-000017a0: 2c0a 2020 2020 2020 2020 2020 2020 2273  ,.            "s
-000017b0: 636f 7065 223a 2022 7468 322d 7363 6f70  cope": "th2-scop
-000017c0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-000017d0: 2261 7474 6163 6865 644d 6573 7361 6765  "attachedMessage
-000017e0: 4964 7322 3a20 5b5d 2c0a 2020 2020 2020  Ids": [],.      
-000017f0: 2020 2020 2020 2262 6f64 7922 3a20 7b22        "body": {"
-00001800: 7479 7065 223a 2022 6d65 7373 6167 6522  type": "message"
-00001810: 2c20 2264 6174 6122 3a20 2264 732d 6c69  , "data": "ds-li
-00001820: 6220 7465 7374 2062 6f64 7922 7d2c 0a20  b test body"},. 
-00001830: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00001840: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-00001850: 2265 7665 6e74 4964 223a 2022 6465 6d6f  "eventId": "demo
-00001860: 5f62 6f6f 6b5f 313a 7468 322d 7363 6f70  _book_1:th2-scop
-00001870: 653a 3230 3233 3031 3035 3133 3537 3035  e:20230105135705
-00001880: 3536 3335 3232 3030 303a 3961 6462 6233  563522000:9adbb3
-00001890: 6530 2d35 6638 622d 3463 3238 2d61 3261  e0-5f8b-4c28-a2a
-000018a0: 632d 3733 3631 6538 6661 3730 3463 3e64  c-7361e8fa704c>d
-000018b0: 656d 6f5f 626f 6f6b 5f31 3a74 6832 2d73  emo_book_1:th2-s
-000018c0: 636f 7065 3a32 3032 3330 3130 3531 3335  cope:20230105135
-000018d0: 3730 3535 3633 3735 3730 3030 3a64 3631  705563757000:d61
-000018e0: 6539 3330 612d 3864 3030 2d31 3165 642d  e930a-8d00-11ed-
-000018f0: 6161 3161 2d64 3334 6136 3135 3531 3532  aa1a-d34a6155152
-00001900: 645f 3322 2c0a 2020 2020 2020 2020 2020  d_3",.          
-00001910: 2020 2262 6174 6368 4964 223a 2022 6465    "batchId": "de
-00001920: 6d6f 5f62 6f6f 6b5f 313a 7468 322d 7363  mo_book_1:th2-sc
-00001930: 6f70 653a 3230 3233 3031 3035 3133 3537  ope:202301051357
-00001940: 3035 3536 3335 3232 3030 303a 3961 6462  05563522000:9adb
-00001950: 6233 6530 2d35 6638 622d 3463 3238 2d61  b3e0-5f8b-4c28-a
-00001960: 3261 632d 3733 3631 6538 6661 3730 3463  2ac-7361e8fa704c
-00001970: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00001980: 6973 4261 7463 6865 6422 3a20 5472 7565  isBatched": True
-00001990: 2c0a 2020 2020 2020 2020 2020 2020 2265  ,.            "e
-000019a0: 7665 6e74 4e61 6d65 223a 2022 506c 6169  ventName": "Plai
-000019b0: 6e20 6576 656e 7420 3222 2c0a 2020 2020  n event 2",.    
-000019c0: 2020 2020 2020 2020 2265 7665 6e74 5479          "eventTy
-000019d0: 7065 223a 2022 6473 2d6c 6962 2d74 6573  pe": "ds-lib-tes
-000019e0: 742d 6576 656e 7422 2c0a 2020 2020 2020  t-event",.      
-000019f0: 2020 2020 2020 2265 6e64 5469 6d65 7374        "endTimest
-00001a00: 616d 7022 3a20 7b22 6570 6f63 6853 6563  amp": {"epochSec
-00001a10: 6f6e 6422 3a20 3136 3732 3932 3730 3235  ond": 1672927025
-00001a20: 2c20 226e 616e 6f22 3a20 3536 3337 3931  , "nano": 563791
-00001a30: 3030 307d 2c0a 2020 2020 2020 2020 2020  000},.          
-00001a40: 2020 2273 7461 7274 5469 6d65 7374 616d    "startTimestam
-00001a50: 7022 3a20 7b22 6570 6f63 6853 6563 6f6e  p": {"epochSecon
-00001a60: 6422 3a20 3136 3732 3932 3730 3235 2c20  d": 1672927025, 
-00001a70: 226e 616e 6f22 3a20 3536 3337 3537 3030  "nano": 56375700
-00001a80: 307d 2c0a 2020 2020 2020 2020 2020 2020  0},.            
-00001a90: 2270 6172 656e 7445 7665 6e74 4964 223a  "parentEventId":
-00001aa0: 2022 6465 6d6f 5f62 6f6f 6b5f 313a 7468   "demo_book_1:th
-00001ab0: 322d 7363 6f70 653a 3230 3233 3031 3035  2-scope:20230105
-00001ac0: 3133 3537 3035 3536 3038 3733 3030 303a  135705560873000:
-00001ad0: 6436 3165 3933 3061 2d38 6430 302d 3131  d61e930a-8d00-11
-00001ae0: 6564 2d61 6131 612d 6433 3461 3631 3535  ed-aa1a-d34a6155
-00001af0: 3135 3264 5f31 222c 0a20 2020 2020 2020  152d_1",.       
-00001b00: 2020 2020 2022 7375 6363 6573 7366 756c       "successful
-00001b10: 223a 2054 7275 652c 0a20 2020 2020 2020  ": True,.       
-00001b20: 2020 2020 2022 626f 6f6b 4964 223a 2022       "bookId": "
-00001b30: 6465 6d6f 5f62 6f6f 6b5f 3122 2c0a 2020  demo_book_1",.  
-00001b40: 2020 2020 2020 2020 2020 2273 636f 7065            "scope
-00001b50: 223a 2022 7468 322d 7363 6f70 6522 2c0a  ": "th2-scope",.
-00001b60: 2020 2020 2020 2020 2020 2020 2261 7474              "att
-00001b70: 6163 6865 644d 6573 7361 6765 4964 7322  achedMessageIds"
-00001b80: 3a20 5b5d 2c0a 2020 2020 2020 2020 2020  : [],.          
-00001b90: 2020 2262 6f64 7922 3a20 7b22 7479 7065    "body": {"type
-00001ba0: 223a 2022 6d65 7373 6167 6522 2c20 2264  ": "message", "d
-00001bb0: 6174 6122 3a20 2264 732d 6c69 6220 7465  ata": "ds-lib te
-00001bc0: 7374 2062 6f64 7922 7d2c 0a20 2020 2020  st body"},.     
-00001bd0: 2020 207d 2c0a 2020 2020 5d0a 290a 0a23     },.    ].)..#
-00001be0: 205b 315d 2057 6f72 6b69 6e67 2077 6974   [1] Working wit
-00001bf0: 6820 6120 4461 7461 206f 626a 6563 742e  h a Data object.
-00001c00: 0a23 205b 312e 315d 2046 696c 7465 722e  .# [1.1] Filter.
-00001c10: 0a66 696c 7465 7265 645f 6576 656e 7473  .filtered_events
-00001c20: 3a20 4461 7461 203d 2065 7665 6e74 732e  : Data = events.
-00001c30: 6669 6c74 6572 286c 616d 6264 6120 653a  filter(lambda e:
-00001c40: 2065 5b22 626f 6479 225d 2021 3d20 5b5d   e["body"] != []
-00001c50: 2920 2023 2046 696c 7465 7220 6576 656e  )  # Filter even
-00001c60: 7473 2077 6974 6820 656d 7074 7920 626f  ts with empty bo
-00001c70: 6479 2e0a 0a0a 2320 5b31 2e32 5d20 4d61  dy....# [1.2] Ma
-00001c80: 702e 0a64 6566 2074 7261 6e73 666f 726d  p..def transform
-00001c90: 5f66 756e 6374 696f 6e28 7265 636f 7264  _function(record
-00001ca0: 293a 0a20 2020 2072 6574 7572 6e20 7b22  ):.    return {"
-00001cb0: 6576 656e 744e 616d 6522 3a20 7265 636f  eventName": reco
-00001cc0: 7264 5b22 6576 656e 744e 616d 6522 5d2c  rd["eventName"],
-00001cd0: 2022 7375 6363 6573 7366 756c 223a 2072   "successful": r
-00001ce0: 6563 6f72 645b 2273 7563 6365 7373 6675  ecord["successfu
-00001cf0: 6c22 5d7d 0a0a 0a66 696c 7465 7265 645f  l"]}...filtered_
-00001d00: 616e 645f 6d61 7070 6564 5f65 7665 6e74  and_mapped_event
-00001d10: 7320 3d20 6669 6c74 6572 6564 5f65 7665  s = filtered_eve
-00001d20: 6e74 732e 6d61 7028 7472 616e 7366 6f72  nts.map(transfor
-00001d30: 6d5f 6675 6e63 7469 6f6e 290a 0a23 205b  m_function)..# [
-00001d40: 312e 335d 2044 6174 6120 7069 7065 6c69  1.3] Data pipeli
-00001d50: 6e65 2e0a 2320 2020 2020 2020 496e 7374  ne..#       Inst
-00001d60: 6561 6420 6f66 2064 6f69 6e67 2064 6174  ead of doing dat
-00001d70: 6120 7472 616e 7366 6f72 6d61 7469 6f6e  a transformation
-00001d80: 7320 7374 6570 2062 7920 7374 6570 2079  s step by step y
-00001d90: 6f75 2063 616e 2064 6f20 6974 2069 6e20  ou can do it in 
-00001da0: 6f6e 6520 6c69 6e65 2e0a 6669 6c74 6572  one line..filter
-00001db0: 6564 5f61 6e64 5f6d 6170 7065 645f 6576  ed_and_mapped_ev
-00001dc0: 656e 7473 5f62 795f 7069 7065 6c69 6e65  ents_by_pipeline
-00001dd0: 203d 2065 7665 6e74 732e 6669 6c74 6572   = events.filter
-00001de0: 286c 616d 6264 6120 653a 2065 5b22 626f  (lambda e: e["bo
-00001df0: 6479 225d 2021 3d20 5b5d 292e 6d61 7028  dy"] != []).map(
-00001e00: 0a20 2020 2074 7261 6e73 666f 726d 5f66  .    transform_f
-00001e10: 756e 6374 696f 6e0a 290a 2320 436f 6e74  unction.).# Cont
-00001e20: 656e 7420 6f66 2074 6865 7365 2074 776f  ent of these two
-00001e30: 2044 6174 6120 6f62 6a65 6374 7320 7368   Data objects sh
-00001e40: 6f75 6c64 2062 6520 6571 7561 6c2e 0a61  ould be equal..a
-00001e50: 7373 6572 7420 6c69 7374 2866 696c 7465  ssert list(filte
-00001e60: 7265 645f 616e 645f 6d61 7070 6564 5f65  red_and_mapped_e
-00001e70: 7665 6e74 7329 203d 3d20 6c69 7374 2866  vents) == list(f
-00001e80: 696c 7465 7265 645f 616e 645f 6d61 7070  iltered_and_mapp
-00001e90: 6564 5f65 7665 6e74 735f 6279 5f70 6970  ed_events_by_pip
-00001ea0: 656c 696e 6529 0a0a 2320 5b31 2e34 5d20  eline)..# [1.4] 
-00001eb0: 5369 6674 2e20 536b 6970 2074 6865 2066  Sift. Skip the f
-00001ec0: 6972 7374 2066 6577 2069 7465 6d73 206f  irst few items o
-00001ed0: 7220 6c69 6d69 7420 7468 656d 2e0a 6461  r limit them..da
-00001ee0: 7461 203d 2044 6174 6128 5b31 2c20 322c  ta = Data([1, 2,
-00001ef0: 2033 2c20 342c 2035 2c20 362c 2037 2c20   3, 4, 5, 6, 7, 
-00001f00: 382c 2039 2c20 3130 2c20 3131 2c20 3132  8, 9, 10, 11, 12
-00001f10: 2c20 3133 2c20 3134 2c20 3135 5d29 0a69  , 13, 14, 15]).i
-00001f20: 7465 6d73 5f66 726f 6d5f 3131 5f74 6f5f  tems_from_11_to_
-00001f30: 656e 643a 2047 656e 6572 6174 6f72 203d  end: Generator =
-00001f40: 2064 6174 612e 7369 6674 2873 6b69 703d   data.sift(skip=
-00001f50: 3130 290a 6f6e 6c79 5f66 6972 7374 5f31  10).only_first_1
-00001f60: 305f 6974 656d 733a 2047 656e 6572 6174  0_items: Generat
-00001f70: 6f72 203d 2064 6174 612e 7369 6674 286c  or = data.sift(l
-00001f80: 696d 6974 3d31 3029 0a0a 2320 5b31 2e35  imit=10)..# [1.5
-00001f90: 5d20 4368 616e 6769 6e67 2063 6163 6865  ] Changing cache
-00001fa0: 2073 7461 7475 732e 0a65 7665 6e74 732e   status..events.
-00001fb0: 7573 655f 6361 6368 6528 5472 7565 290a  use_cache(True).
-00001fc0: 2320 6f72 206a 7573 740a 6576 656e 7473  # or just.events
-00001fd0: 2e75 7365 5f63 6163 6865 2829 2020 2320  .use_cache()  # 
-00001fe0: 4966 2079 6f75 2077 616e 7420 746f 2061  If you want to a
-00001ff0: 6374 6976 6174 6520 6361 6368 652e 0a23  ctivate cache..#
-00002000: 205b 312e 365d 2057 616c 6b20 7468 726f   [1.6] Walk thro
-00002010: 7567 6820 6461 7461 2e0a 666f 7220 6576  ugh data..for ev
-00002020: 656e 7420 696e 2065 7665 6e74 733a 0a20  ent in events:. 
-00002030: 2020 2023 2044 6f20 736f 6d65 7468 696e     # Do somethin
-00002040: 6720 7769 7468 2065 7665 6e74 2028 6576  g with event (ev
-00002050: 656e 7420 6973 2061 2064 6963 7429 2e0a  ent is a dict)..
-00002060: 2020 2020 7072 696e 7428 6576 656e 7429      print(event)
-00002070: 0a23 2041 6674 6572 2066 6972 7374 2069  .# After first i
-00002080: 7465 7261 7469 6f6e 2074 6865 2065 7665  teration the eve
-00002090: 6e74 7320 6861 7320 6120 6361 6368 6520  nts has a cache 
-000020a0: 6669 6c65 2e0a 2320 4e6f 7720 7468 6579  file..# Now they
-000020b0: 2077 696c 6c20 6265 2075 7365 6420 696e   will be used in
-000020c0: 2074 6865 2063 6163 6865 2069 6e20 7468   the cache in th
-000020d0: 6520 6e65 7874 2069 7465 7261 7469 6f6e  e next iteration
-000020e0: 2e0a 0a23 205b 312e 375d 2047 6574 206e  ...# [1.7] Get n
-000020f0: 756d 6265 7220 6f66 2074 6865 2065 6c65  umber of the ele
-00002100: 6d65 6e74 7320 696e 2074 6865 2044 6174  ments in the Dat
-00002110: 6120 6f62 6a65 6374 2e0a 6e75 6d62 6572  a object..number
-00002120: 5f6f 665f 6576 656e 7473 203d 2065 7665  _of_events = eve
-00002130: 6e74 732e 6c65 6e0a 0a23 205b 312e 385d  nts.len..# [1.8]
-00002140: 2043 6865 636b 2074 6861 7420 4461 7461   Check that Data
-00002150: 206f 626a 6563 7420 6973 6e27 7420 656d   object isn't em
-00002160: 7074 792e 0a23 2054 6865 2064 6174 6120  pty..# The data 
-00002170: 736f 7572 6365 2073 686f 756c 6420 6265  source should be
-00002180: 206e 6f74 2065 6d70 7479 2e0a 6173 7365   not empty..asse
-00002190: 7274 2065 7665 6e74 732e 6973 5f65 6d70  rt events.is_emp
-000021a0: 7479 2069 7320 4661 6c73 650a 0a23 205b  ty is False..# [
-000021b0: 312e 395d 2043 6f6e 7665 7274 2044 6174  1.9] Convert Dat
-000021c0: 6120 6f62 6a65 6374 2074 6f20 7468 6520  a object to the 
-000021d0: 6c69 7374 206f 6620 656c 656d 656e 7473  list of elements
-000021e0: 2865 7665 6e74 7320 6f72 206d 6573 7361  (events or messa
-000021f0: 6765 7329 2e0a 2320 4265 2063 6172 6566  ges)..# Be caref
-00002200: 756c 2c20 7468 6973 2063 616e 2074 616b  ul, this can tak
-00002210: 6520 746f 6f20 6d75 6368 206d 656d 6f72  e too much memor
-00002220: 792e 0a65 7665 6e74 735f 6c69 7374 203d  y..events_list =
-00002230: 206c 6973 7428 6576 656e 7473 290a 0a23   list(events)..#
-00002240: 205b 312e 3130 5d20 5468 6520 6361 6368   [1.10] The cach
-00002250: 6520 696e 6865 7269 7461 6e63 652e 0a23  e inheritance..#
-00002260: 2043 7265 6174 6573 2061 206e 6577 2044   Creates a new D
-00002270: 6174 6120 6f62 6a65 6374 2074 6861 7420  ata object that 
-00002280: 7769 6c6c 2075 7365 2063 6163 6865 2066  will use cache f
-00002290: 726f 6d20 7468 6520 6576 656e 7473 2044  rom the events D
-000022a0: 6174 6120 6f62 6a65 6374 2e0a 6576 656e  ata object..even
-000022b0: 7473 5f66 696c 7465 7265 643a 2044 6174  ts_filtered: Dat
-000022c0: 6120 3d20 6576 656e 7473 2e66 696c 7465  a = events.filte
-000022d0: 7228 6c61 6d62 6461 2072 6563 6f72 643a  r(lambda record:
-000022e0: 2072 6563 6f72 642e 6765 7428 2262 6174   record.get("bat
-000022f0: 6368 4964 2229 290a 0a23 204e 6577 2044  chId"))..# New D
-00002300: 6174 6120 6f62 6a65 6374 7320 646f 6e27  ata objects don'
-00002310: 7420 7573 6520 7468 6569 7220 6f77 6e20  t use their own 
-00002320: 6361 6368 6520 6279 2064 6566 6175 6c74  cache by default
-00002330: 2062 7574 2075 7365 2074 6865 2063 6163   but use the cac
-00002340: 6865 206f 6620 7468 6520 7061 7265 6e74  he of the parent
-00002350: 2044 6174 6120 6f62 6a65 6374 2e0a 2320   Data object..# 
-00002360: 5573 6520 7573 655f 6361 6368 6520 6d65  Use use_cache me
-00002370: 7468 6f64 2074 6f20 6163 7469 7661 7465  thod to activate
-00002380: 2063 6163 6869 6e67 2e0a 2320 4166 7465   caching..# Afte
-00002390: 7220 7468 6174 2c20 7468 6520 4461 7461  r that, the Data
-000023a0: 206f 626a 6563 7420 7769 6c6c 2063 7265   object will cre
-000023b0: 6174 6520 6974 7320 6f77 6e20 6361 6368  ate its own cach
-000023c0: 6520 6669 6c65 2e0a 6576 656e 7473 5f66  e file..events_f
-000023d0: 696c 7465 7265 642e 7573 655f 6361 6368  iltered.use_cach
-000023e0: 6528 290a 0a6c 6973 7428 6576 656e 7473  e()..list(events
-000023f0: 5f66 696c 7465 7265 6429 2020 2320 4a75  _filtered)  # Ju
-00002400: 7374 2074 6f20 6974 6572 6174 6520 4461  st to iterate Da
-00002410: 7461 206f 626a 6563 7420 2863 6163 6865  ta object (cache
-00002420: 2066 696c 6520 7769 6c6c 2062 6520 6372   file will be cr
-00002430: 6561 7465 6429 2e0a 0a66 696c 7465 7265  eated)...filtere
-00002440: 645f 6576 656e 7473 5f74 7970 6573 203d  d_events_types =
-00002450: 2065 7665 6e74 735f 6669 6c74 6572 6564   events_filtered
-00002460: 2e6d 6170 286c 616d 6264 6120 7265 636f  .map(lambda reco
-00002470: 7264 3a20 7b22 6576 656e 7454 7970 6522  rd: {"eventType"
-00002480: 3a20 7265 636f 7264 2e67 6574 2822 6576  : record.get("ev
-00002490: 656e 7454 7970 6522 297d 290a 0a65 7665  entType")})..eve
-000024a0: 6e74 735f 7769 7468 6f75 745f 7479 7065  nts_without_type
-000024b0: 735f 7769 7468 5f62 6174 6368 203d 2066  s_with_batch = f
-000024c0: 696c 7465 7265 645f 6576 656e 7473 5f74  iltered_events_t
-000024d0: 7970 6573 2e66 696c 7465 7228 0a20 2020  ypes.filter(.   
-000024e0: 206c 616d 6264 6120 7265 636f 7264 3a20   lambda record: 
-000024f0: 6e6f 7420 7265 636f 7264 2e67 6574 2822  not record.get("
-00002500: 6576 656e 7454 7970 6522 290a 290a 6576  eventType").).ev
-00002510: 656e 7473 5f77 6974 686f 7574 5f74 7970  ents_without_typ
-00002520: 6573 5f77 6974 685f 6261 7463 682e 7573  es_with_batch.us
-00002530: 655f 6361 6368 6528 290a 0a23 205b 312e  e_cache()..# [1.
-00002540: 3131 5d20 4461 7461 206f 626a 6563 7473  11] Data objects
-00002550: 206a 6f69 6e69 6e67 2e0a 2320 596f 7520   joining..# You 
-00002560: 6861 7665 2074 6865 2066 6f6c 6c6f 7769  have the followi
-00002570: 6e67 2033 2044 6174 6120 6f62 6a65 6374  ng 3 Data object
-00002580: 732e 0a64 3120 3d20 4461 7461 285b 312c  s..d1 = Data([1,
-00002590: 2032 2c20 335d 290a 6432 203d 2044 6174   2, 3]).d2 = Dat
-000025a0: 6128 5b22 6122 2c20 7b22 6964 223a 2031  a(["a", {"id": 1
-000025b0: 3233 7d2c 2022 6322 5d29 0a64 3320 3d20  23}, "c"]).d3 = 
-000025c0: 4461 7461 285b 372c 2038 2c20 395d 290a  Data([7, 8, 9]).
-000025d0: 2320 596f 7520 6361 6e20 6a6f 696e 2044  # You can join D
-000025e0: 6174 6120 6f62 6a65 6374 7320 696e 2066  ata objects in f
-000025f0: 6f6c 6c6f 7769 6e67 2077 6179 732e 0a23  ollowing ways..#
-00002600: 2050 6c65 6173 6520 6e6f 7465 2c20 6e65   Please note, ne
-00002610: 7720 4461 7461 206f 626a 6563 7420 7769  w Data object wi
-00002620: 6c6c 2068 6176 6520 6361 6368 6520 7374  ll have cache st
-00002630: 6174 7573 203d 3d20 4661 6c73 652e 0a64  atus == False..d
-00002640: 6174 615f 7669 615f 696e 6974 203d 2044  ata_via_init = D
-00002650: 6174 6128 5b64 312c 2064 322c 2064 335d  ata([d1, d2, d3]
-00002660: 290a 6461 7461 5f76 6961 5f61 6464 203d  ).data_via_add =
-00002670: 2064 3120 2b20 6432 202b 2064 330a 6461   d1 + d2 + d3.da
-00002680: 7461 5f77 6974 685f 6e6f 6e5f 6461 7461  ta_with_non_data
-00002690: 5f6f 626a 5f76 6961 5f69 6e69 7420 3d20  _obj_via_init = 
-000026a0: 4461 7461 285b 6431 2c20 5b22 6122 2c20  Data([d1, ["a", 
-000026b0: 7b22 6964 223a 2031 3233 7d2c 2022 6322  {"id": 123}, "c"
-000026c0: 5d2c 2064 335d 290a 6461 7461 5f77 6974  ], d3]).data_wit
-000026d0: 685f 6e6f 6e5f 6461 7461 5f6f 626a 5f76  h_non_data_obj_v
-000026e0: 6961 5f61 6464 203d 2064 3120 2b20 5b22  ia_add = d1 + ["
-000026f0: 6122 2c20 7b22 6964 223a 2031 3233 7d2c  a", {"id": 123},
-00002700: 2022 6322 5d20 2b20 6433 0a23 2059 6f75   "c"] + d3.# You
-00002710: 2063 616e 206a 6f69 6e20 6375 7272 656e   can join curren
-00002720: 7420 4461 7461 206f 626a 6563 7420 6f6e  t Data object on
-00002730: 2070 6c61 6365 2075 7369 6e67 202b 3d2e   place using +=.
-00002740: 0a23 2049 7420 7769 6c6c 206b 6565 7020  .# It will keep 
-00002750: 6361 6368 6520 7374 6174 7573 2e0a 6431  cache status..d1
-00002760: 202b 3d20 6433 2020 2320 6431 2077 696c   += d3  # d1 wil
-00002770: 6c20 6265 636f 6d65 2044 6174 6128 5b31  l become Data([1
-00002780: 2c32 2c33 2c37 2c38 2c39 5d29 0a0a 2320  ,2,3,7,8,9])..# 
-00002790: 5b31 2e31 325d 2042 7569 6c64 2061 6e64  [1.12] Build and
-000027a0: 2072 6561 6420 4461 7461 206f 626a 6563   read Data objec
-000027b0: 7420 6361 6368 6520 6669 6c65 732e 0a65  t cache files..e
-000027c0: 7665 6e74 732e 6275 696c 645f 6361 6368  vents.build_cach
-000027d0: 6528 2263 6163 6865 5f66 696c 656e 616d  e("cache_filenam
-000027e0: 655f 6f72 5f70 6174 6822 290a 6461 7461  e_or_path").data
-000027f0: 5f6f 626a 5f66 726f 6d5f 6361 6368 6520  _obj_from_cache 
-00002800: 3d20 4461 7461 2e66 726f 6d5f 6361 6368  = Data.from_cach
-00002810: 655f 6669 6c65 2822 6361 6368 655f 6669  e_file("cache_fi
-00002820: 6c65 6e61 6d65 5f6f 725f 7061 7468 2229  lename_or_path")
-00002830: 0a0a 2320 5b31 2e31 335d 2043 6865 636b  ..# [1.13] Check
-00002840: 2069 6620 4461 7461 2069 7320 736f 7274   if Data is sort
-00002850: 6564 2e0a 6973 5f73 6f72 7465 6420 3d20  ed..is_sorted = 
-00002860: 6576 656e 7473 2e69 735f 736f 7274 6564  events.is_sorted
-00002870: 286c 616d 6264 6120 653a 2065 5b22 7374  (lambda e: e["st
-00002880: 6172 7454 696d 6573 7461 6d70 225d 5b22  artTimestamp"]["
-00002890: 6570 6f63 6853 6563 6f6e 6422 5d29 0a0a  epochSecond"])..
-000028a0: 2320 5b32 5d20 576f 726b 696e 6720 7769  # [2] Working wi
-000028b0: 7468 2063 6f6e 7665 7274 6572 732e 0a23  th converters..#
-000028c0: 2054 6865 7265 2061 7265 2063 7572 7265   There are curre
-000028d0: 6e74 6c79 2074 6872 6565 2069 6d70 6c65  ntly three imple
-000028e0: 6d65 6e74 6174 696f 6e73 206f 6620 4954  mentations of IT
-000028f0: 696d 6573 7461 6d70 436f 6e76 6572 7465  imestampConverte
-00002900: 7220 636c 6173 733a 2044 6174 6574 696d  r class: Datetim
-00002910: 6543 6f6e 7665 7274 652c 2044 6174 6574  eConverte, Datet
-00002920: 696d 6553 7472 696e 6743 6f6e 7665 7274  imeStringConvert
-00002930: 6572 2061 6e64 2050 726f 746f 6275 6654  er and ProtobufT
-00002940: 696d 6573 7461 6d70 436f 6e76 6572 7465  imestampConverte
-00002950: 722e 0a23 2054 6865 7920 616c 6c20 696d  r..# They all im
-00002960: 706c 656d 656e 7420 7361 6d65 206d 6574  plement same met
-00002970: 686f 6473 2066 726f 6d20 6261 7365 2063  hods from base c
-00002980: 6c61 7373 2e0a 2320 4e6f 7465 2074 6861  lass..# Note tha
-00002990: 7420 736f 6d65 2061 6363 7572 6163 7920  t some accuracy 
-000029a0: 6d61 7920 6265 206c 6f73 7420 6475 7269  may be lost duri
-000029b0: 6e67 2063 6f6e 7665 7273 696f 6e2e 0a23  ng conversion..#
-000029c0: 2049 6620 666f 7220 6578 616d 706c 6520   If for example 
-000029d0: 796f 7520 7573 6520 746f 5f6d 6963 726f  you use to_micro
-000029e0: 7365 636f 6e64 7320 6e61 6e6f 7365 636f  seconds nanoseco
-000029f0: 6e64 7320 7769 6c6c 2062 6520 6375 7420  nds will be cut 
-00002a00: 6f66 6620 696e 7374 6561 6420 6f66 2072  off instead of r
-00002a10: 6f75 6e64 696e 672e 0a0a 2320 5b32 2e31  ounding...# [2.1
-00002a20: 5d20 4461 7465 7469 6d65 436f 6e76 6572  ] DatetimeConver
-00002a30: 7465 722e 0a23 2044 6174 6574 696d 6543  ter..# DatetimeC
-00002a40: 6f6e 7665 7274 6572 2074 616b 6573 2064  onverter takes d
-00002a50: 6174 6574 696d 652e 6461 7465 7469 6d65  atetime.datetime
-00002a60: 206f 626a 6563 7420 6173 2069 6e70 7574   object as input
-00002a70: 2e0a 0a64 6174 6574 696d 655f 6f62 6a20  ...datetime_obj 
-00002a80: 3d20 6461 7465 7469 6d65 2879 6561 723d  = datetime(year=
-00002a90: 3230 3233 2c20 6d6f 6e74 683d 312c 2064  2023, month=1, d
-00002aa0: 6179 3d35 2c20 686f 7572 3d31 342c 206d  ay=5, hour=14, m
-00002ab0: 696e 7574 653d 3338 2c20 7365 636f 6e64  inute=38, second
-00002ac0: 3d32 352c 206d 6963 726f 7365 636f 6e64  =25, microsecond
-00002ad0: 3d31 3436 3029 0a0a 2320 4974 2068 6173  =1460)..# It has
-00002ae0: 206d 6574 686f 6473 2074 6861 7420 7265   methods that re
-00002af0: 7475 726e 2074 6865 2064 6174 6574 696d  turn the datetim
-00002b00: 6520 696e 2064 6966 6665 7265 6e74 2066  e in different f
-00002b10: 6f72 6d61 733a 0a0a 6461 7465 5f6d 7320  ormas:..date_ms 
-00002b20: 3d20 4461 7465 7469 6d65 436f 6e76 6572  = DatetimeConver
-00002b30: 7465 722e 746f 5f6d 696c 6c69 7365 636f  ter.to_milliseco
-00002b40: 6e64 7328 6461 7465 7469 6d65 5f6f 626a  nds(datetime_obj
-00002b50: 290a 6461 7465 5f75 7320 3d20 4461 7465  ).date_us = Date
-00002b60: 7469 6d65 436f 6e76 6572 7465 722e 746f  timeConverter.to
-00002b70: 5f6d 6963 726f 7365 636f 6e64 7328 6461  _microseconds(da
-00002b80: 7465 7469 6d65 5f6f 626a 290a 2320 436f  tetime_obj).# Co
-00002b90: 6e76 6572 7469 6e67 2074 6f20 6e61 6e6f  nverting to nano
-00002ba0: 7365 636f 6e64 7320 6a75 7374 7320 6164  seconds justs ad
-00002bb0: 6473 2074 6872 6565 2074 7261 696c 696e  ds three trailin
-00002bc0: 6720 7a65 726f 7320 6173 2064 6174 6574  g zeros as datet
-00002bd0: 696d 6520 6f62 6a65 6374 2064 6f65 736e  ime object doesn
-00002be0: 2774 2068 6176 6520 6e61 6e6f 7365 636f  't have nanoseco
-00002bf0: 6e64 732e 0a64 6174 655f 6e73 203d 2044  nds..date_ns = D
-00002c00: 6174 6574 696d 6543 6f6e 7665 7274 6572  atetimeConverter
-00002c10: 2e74 6f5f 6e61 6e6f 7365 636f 6e64 7328  .to_nanoseconds(
-00002c20: 6461 7465 7469 6d65 5f6f 626a 290a 0a23  datetime_obj)..#
-00002c30: 205b 322e 325d 2044 6174 6574 696d 6553   [2.2] DatetimeS
-00002c40: 7472 696e 6743 6f6e 7665 7274 6572 0a23  tringConverter.#
-00002c50: 2044 6174 6574 696d 6553 7472 696e 6743   DatetimeStringC
-00002c60: 6f6e 7665 7274 6572 2074 616b 6573 2073  onverter takes s
-00002c70: 7472 696e 6720 696e 2022 7979 7979 2d4d  tring in "yyyy-M
-00002c80: 4d2d 6464 5448 483a 6d6d 3a73 735b 2e53  M-ddTHH:mm:ss[.S
-00002c90: 5353 5353 5353 5353 5d5a 2220 666f 726d  SSSSSSSS]Z" form
-00002ca0: 6174 2e0a 0a64 6174 655f 7374 7269 6e67  at...date_string
-00002cb0: 203d 2022 3230 3233 2d30 312d 3035 5431   = "2023-01-05T1
-00002cc0: 343a 3338 3a32 352e 3030 3134 365a 220a  4:38:25.00146Z".
-00002cd0: 0a23 2057 6520 6861 7665 2073 616d 6520  .# We have same 
-00002ce0: 6d65 7468 6f64 7320 6173 2069 6e20 4461  methods as in Da
-00002cf0: 7465 7469 6d65 436f 6e76 6572 7465 720a  tetimeConverter.
-00002d00: 6461 7465 5f6d 735f 6672 6f6d 5f73 7472  date_ms_from_str
-00002d10: 696e 6720 3d20 4461 7465 7469 6d65 5374  ing = DatetimeSt
-00002d20: 7269 6e67 436f 6e76 6572 7465 722e 746f  ringConverter.to
-00002d30: 5f6d 696c 6c69 7365 636f 6e64 7328 6461  _milliseconds(da
-00002d40: 7465 5f73 7472 696e 6729 0a64 6174 655f  te_string).date_
-00002d50: 7573 5f66 726f 6d5f 7374 7269 6e67 203d  us_from_string =
-00002d60: 2044 6174 6574 696d 6553 7472 696e 6743   DatetimeStringC
-00002d70: 6f6e 7665 7274 6572 2e74 6f5f 6d69 6372  onverter.to_micr
-00002d80: 6f73 6563 6f6e 6473 2864 6174 655f 7374  oseconds(date_st
-00002d90: 7269 6e67 290a 6461 7465 5f6e 735f 6672  ring).date_ns_fr
-00002da0: 6f6d 5f73 7472 696e 6720 3d20 4461 7465  om_string = Date
-00002db0: 7469 6d65 5374 7269 6e67 436f 6e76 6572  timeStringConver
-00002dc0: 7465 722e 746f 5f6e 616e 6f73 6563 6f6e  ter.to_nanosecon
-00002dd0: 6473 2864 6174 655f 7374 7269 6e67 290a  ds(date_string).
-00002de0: 0a23 2057 6520 6361 6e20 616c 736f 2067  .# We can also g
-00002df0: 6574 2064 6174 6574 696d 6520 6f62 6a65  et datetime obje
-00002e00: 6374 2066 726f 6d20 7374 7269 6e67 0a64  ct from string.d
-00002e10: 6174 6574 696d 655f 6672 6f6d 5f73 7472  atetime_from_str
-00002e20: 696e 6720 3d20 4461 7465 7469 6d65 5374  ing = DatetimeSt
-00002e30: 7269 6e67 436f 6e76 6572 7465 722e 746f  ringConverter.to
-00002e40: 5f64 6174 6574 696d 6528 6461 7465 5f73  _datetime(date_s
-00002e50: 7472 696e 6729 0a0a 2320 5b32 2e33 5d20  tring)..# [2.3] 
-00002e60: 5072 6f74 6f62 7566 5469 6d65 7374 616d  ProtobufTimestam
-00002e70: 7043 6f6e 7665 7274 6572 0a23 2050 726f  pConverter.# Pro
-00002e80: 746f 6275 6620 7469 6d65 7374 616d 7073  tobuf timestamps
-00002e90: 206d 7573 7420 6265 2069 6e20 666f 726d   must be in form
-00002ea0: 207b 2265 706f 6368 5365 636f 6e64 223a   {"epochSecond":
-00002eb0: 2073 6563 6f6e 6473 2c20 226e 616e 6f22   seconds, "nano"
-00002ec0: 3a20 6e61 6e6f 7365 636f 6e64 737d 0a0a  : nanoseconds}..
-00002ed0: 7072 6f74 6f62 7566 5f74 696d 6573 7461  protobuf_timesta
-00002ee0: 6d70 203d 207b 2265 706f 6368 5365 636f  mp = {"epochSeco
-00002ef0: 6e64 223a 2031 3637 3239 3239 3530 352c  nd": 1672929505,
-00002f00: 2022 6e61 6e6f 223a 2031 5f34 3630 5f30   "nano": 1_460_0
-00002f10: 3030 7d0a 0a64 6174 655f 6d73 5f66 726f  00}..date_ms_fro
-00002f20: 6d5f 7469 6d65 7374 616d 7020 3d20 5072  m_timestamp = Pr
-00002f30: 6f74 6f62 7566 5469 6d65 7374 616d 7043  otobufTimestampC
-00002f40: 6f6e 7665 7274 6572 2e74 6f5f 6d69 6c6c  onverter.to_mill
-00002f50: 6973 6563 6f6e 6473 2870 726f 746f 6275  iseconds(protobu
-00002f60: 665f 7469 6d65 7374 616d 7029 0a64 6174  f_timestamp).dat
-00002f70: 655f 7573 5f66 726f 6d5f 7469 6d65 7374  e_us_from_timest
-00002f80: 616d 7020 3d20 5072 6f74 6f62 7566 5469  amp = ProtobufTi
-00002f90: 6d65 7374 616d 7043 6f6e 7665 7274 6572  mestampConverter
-00002fa0: 2e74 6f5f 6d69 6372 6f73 6563 6f6e 6473  .to_microseconds
-00002fb0: 2870 726f 746f 6275 665f 7469 6d65 7374  (protobuf_timest
-00002fc0: 616d 7029 0a64 6174 655f 6e73 5f66 726f  amp).date_ns_fro
-00002fd0: 6d5f 7469 6d65 7374 616d 7020 3d20 5072  m_timestamp = Pr
-00002fe0: 6f74 6f62 7566 5469 6d65 7374 616d 7043  otobufTimestampC
-00002ff0: 6f6e 7665 7274 6572 2e74 6f5f 6e61 6e6f  onverter.to_nano
-00003000: 7365 636f 6e64 7328 7072 6f74 6f62 7566  seconds(protobuf
-00003010: 5f74 696d 6573 7461 6d70 290a 6461 7465  _timestamp).date
-00003020: 7469 6d65 5f66 726f 6d5f 7469 6d65 7374  time_from_timest
-00003030: 616d 7020 3d20 5072 6f74 6f62 7566 5469  amp = ProtobufTi
-00003040: 6d65 7374 616d 7043 6f6e 7665 7274 6572  mestampConverter
-00003050: 2e74 6f5f 6461 7465 7469 6d65 2870 726f  .to_datetime(pro
-00003060: 746f 6275 665f 7469 6d65 7374 616d 7029  tobuf_timestamp)
-00003070: 0a0a 2320 5b33 5d20 576f 726b 696e 6720  ..# [3] Working 
-00003080: 7769 7468 2045 7665 6e74 5472 6565 2061  with EventTree a
-00003090: 6e64 2045 7665 6e74 5472 6565 436f 6c6c  nd EventTreeColl
-000030a0: 6563 7469 6f6e 2e0a 0a23 205b 332e 315d  ection...# [3.1]
-000030b0: 2042 7569 6c64 2061 2063 7573 746f 6d20   Build a custom 
-000030c0: 4576 656e 7454 7265 650a 2320 546f 2063  EventTree.# To c
-000030d0: 7265 6174 6520 616e 2045 7665 6e74 5472  reate an EventTr
-000030e0: 6565 206f 626a 6563 7420 796f 7520 6e65  ee object you ne
-000030f0: 6564 2074 6f20 7072 6f76 6964 6520 6e61  ed to provide na
-00003100: 6d65 2c20 6964 2061 6e64 2064 6174 6120  me, id and data 
-00003110: 6f66 2074 6865 2072 6f6f 7420 6576 656e  of the root even
-00003120: 742e 0a74 7265 6520 3d20 4576 656e 7454  t..tree = EventT
-00003130: 7265 6528 6576 656e 745f 6e61 6d65 3d22  ree(event_name="
-00003140: 726f 6f74 2065 7665 6e74 222c 2065 7665  root event", eve
-00003150: 6e74 5f69 643d 2272 6f6f 745f 6964 222c  nt_id="root_id",
-00003160: 2064 6174 613d 7b22 6461 7461 223a 205b   data={"data": [
-00003170: 312c 2032 2c20 332c 2034 2c20 355d 7d29  1, 2, 3, 4, 5]})
-00003180: 0a0a 2320 546f 2061 6464 206e 6577 206e  ..# To add new n
-00003190: 6f64 6520 7573 6520 6170 7065 6e64 5f65  ode use append_e
-000031a0: 7665 6e74 2e20 7061 7265 6e74 5f69 6420  vent. parent_id 
-000031b0: 6973 206e 6563 6573 7361 7279 2c20 6461  is necessary, da
-000031c0: 7461 2069 7320 6f70 7469 6f6e 616c 2e0a  ta is optional..
-000031d0: 7472 6565 2e61 7070 656e 645f 6576 656e  tree.append_even
-000031e0: 7428 6576 656e 745f 6e61 6d65 3d22 4122  t(event_name="A"
-000031f0: 2c20 6576 656e 745f 6964 3d22 415f 6964  , event_id="A_id
-00003200: 222c 2064 6174 613d 4e6f 6e65 2c20 7061  ", data=None, pa
-00003210: 7265 6e74 5f69 643d 2272 6f6f 745f 6964  rent_id="root_id
-00003220: 2229 0a0a 2320 5b33 2e33 5d20 4275 696c  ")..# [3.3] Buil
-00003230: 6469 6e67 2074 6865 2045 7665 6e74 5472  ding the EventTr
-00003240: 6565 436f 6c6c 6563 7469 6f6e 2e0a 0a23  eeCollection...#
-00003250: 2049 6620 796f 7520 646f 6e27 7420 7370   If you don't sp
-00003260: 6563 6966 7920 6461 7461 5f73 6f75 7263  ecify data_sourc
-00003270: 6520 666f 7220 7468 6520 6472 6976 6572  e for the driver
-00003280: 2074 6865 6e20 6974 2077 6f6e 2774 2072   then it won't r
-00003290: 6563 6f76 6572 2064 6574 6163 6865 6420  ecover detached 
-000032a0: 6576 656e 7473 2e0a 6472 6976 6572 3a20  events..driver: 
-000032b0: 4945 5443 4472 6976 6572 2020 2320 596f  IETCDriver  # Yo
-000032c0: 7520 7368 6f75 6c64 2069 6e69 7420 4554  u should init ET
-000032d0: 4344 7269 7665 7220 6f62 6a65 6374 2e20  CDriver object. 
-000032e0: 452e 672e 2066 726f 6d20 4c77 4450 206d  E.g. from LwDP m
-000032f0: 6f64 756c 6520 6f72 2079 6f75 7220 6375  odule or your cu
-00003300: 7374 6f6d 2063 6c61 7373 2e0a 6574 6320  stom class..etc 
-00003310: 3d20 4576 656e 7454 7265 6543 6f6c 6c65  = EventTreeColle
-00003320: 6374 696f 6e28 6472 6976 6572 290a 6574  ction(driver).et
-00003330: 632e 6275 696c 6428 6576 656e 7473 290a  c.build(events).
-00003340: 0a23 2044 6574 6163 6865 6420 6576 656e  .# Detached even
-00003350: 7473 2069 736e 2774 2065 6d70 7479 2e0a  ts isn't empty..
-00003360: 6173 7365 7274 2065 7463 2e67 6574 5f64  assert etc.get_d
-00003370: 6574 6163 6865 645f 6576 656e 7473 2829  etached_events()
-00003380: 0a0a 6574 6320 3d20 4576 656e 7454 7265  ..etc = EventTre
-00003390: 6543 6f6c 6c65 6374 696f 6e28 6472 6976  eCollection(driv
-000033a0: 6572 290a 2320 4465 7461 6368 6564 2065  er).# Detached e
-000033b0: 7665 6e74 7320 6172 6520 656d 7074 7920  vents are empty 
-000033c0: 6265 6361 7573 6520 7468 6579 2077 6572  because they wer
-000033d0: 6520 7265 636f 7665 7265 642e 0a61 7373  e recovered..ass
-000033e0: 6572 7420 6e6f 7420 6574 632e 6765 745f  ert not etc.get_
-000033f0: 6465 7461 6368 6564 5f65 7665 6e74 7328  detached_events(
-00003400: 290a 0a23 2054 6865 2063 6f6c 6c65 6374  )..# The collect
-00003410: 696f 6e20 6861 7320 4576 656e 7454 7265  ion has EventTre
-00003420: 6573 2065 6163 6820 7769 7468 2061 2074  es each with a t
-00003430: 7265 6520 6f66 2065 7665 6e74 732e 0a23  ree of events..#
-00003440: 2055 7369 6e67 2043 6f6c 6c65 6374 696f   Using Collectio
-00003450: 6e20 616e 6420 4576 656e 7454 7265 6573  n and EventTrees
-00003460: 2c20 796f 7520 6361 6e20 776f 726b 2066  , you can work f
-00003470: 6c65 7869 626c 7920 7769 7468 2065 7665  lexibly with eve
-00003480: 6e74 732e 0a0a 2320 5b33 2e33 2e31 5d20  nts...# [3.3.1] 
-00003490: 4765 7420 6c65 6176 6573 206f 6620 616c  Get leaves of al
-000034a0: 6c20 7472 6565 732e 0a6c 6561 7665 733a  l trees..leaves:
-000034b0: 2054 7570 6c65 5b64 6963 745d 203d 2065   Tuple[dict] = e
-000034c0: 7463 2e67 6574 5f6c 6561 7665 7328 290a  tc.get_leaves().
-000034d0: 0a23 205b 332e 332e 325d 2047 6574 2072  .# [3.3.2] Get r
-000034e0: 6f6f 7473 2069 6473 206f 6620 616c 6c20  oots ids of all 
-000034f0: 7472 6565 732e 0a72 6f6f 7473 3a20 4c69  trees..roots: Li
-00003500: 7374 5b73 7472 5d20 3d20 6574 632e 6765  st[str] = etc.ge
-00003510: 745f 726f 6f74 735f 6964 7328 290a 0a23  t_roots_ids()..#
-00003520: 205b 332e 332e 335d 2046 696e 6420 616e   [3.3.3] Find an
-00003530: 2065 7665 6e74 2069 6e20 616c 6c20 7472   event in all tr
-00003540: 6565 732e 0a66 696e 645f 6576 656e 743a  ees..find_event:
-00003550: 204f 7074 696f 6e61 6c5b 6469 6374 5d20   Optional[dict] 
-00003560: 3d20 6574 632e 6669 6e64 286c 616d 6264  = etc.find(lambd
-00003570: 6120 6576 656e 743a 2022 5365 6e64 206d  a event: "Send m
-00003580: 6573 7361 6765 2220 696e 2065 7665 6e74  essage" in event
-00003590: 5b22 6576 656e 7454 7970 6522 5d29 0a0a  ["eventType"])..
-000035a0: 2320 5b33 2e33 2e34 5d20 4669 6e64 2061  # [3.3.4] Find a
-000035b0: 6c6c 2065 7665 6e74 7320 696e 2061 6c6c  ll events in all
-000035c0: 2074 7265 6573 2e20 5468 6572 6520 6973   trees. There is
-000035d0: 2061 6c73 6f20 6974 6572 6162 6c65 2076   also iterable v
-000035e0: 6572 7369 6f6e 2027 6669 6e64 616c 6c5f  ersion 'findall_
-000035f0: 6974 6572 272e 0a66 696e 645f 6576 656e  iter'..find_even
-00003600: 7473 3a20 4c69 7374 5b64 6963 745d 203d  ts: List[dict] =
-00003610: 2065 7463 2e66 696e 6461 6c6c 286c 616d   etc.findall(lam
-00003620: 6264 6120 6576 656e 743a 2065 7665 6e74  bda event: event
-00003630: 5b22 7375 6363 6573 7366 756c 225d 2069  ["successful"] i
-00003640: 7320 5472 7565 290a 0a23 205b 332e 332e  s True)..# [3.3.
-00003650: 355d 2046 696e 6420 616e 2061 6e63 6573  5] Find an ances
-00003660: 746f 7220 6f66 2074 6865 2065 7665 6e74  tor of the event
-00003670: 2e0a 616e 6365 7374 6f72 3a20 4f70 7469  ..ancestor: Opti
-00003680: 6f6e 616c 5b64 6963 745d 203d 2065 7463  onal[dict] = etc
-00003690: 2e66 696e 645f 616e 6365 7374 6f72 280a  .find_ancestor(.
-000036a0: 2020 2020 2238 6262 6533 3731 372d 6366      "8bbe3717-cf
-000036b0: 3539 2d31 3165 622d 6133 6637 2d30 3934  59-11eb-a3f7-094
-000036c0: 6639 3034 6333 6136 3222 2c20 6669 6c74  f904c3a62", filt
-000036d0: 6572 3d6c 616d 6264 6120 6576 656e 743a  er=lambda event:
-000036e0: 2022 526f 6f74 4576 656e 7422 2069 6e20   "RootEvent" in 
-000036f0: 6576 656e 745b 2265 7665 6e74 4e61 6d65  event["eventName
-00003700: 225d 0a29 0a0a 2320 5b33 2e33 2e36 5d20  "].)..# [3.3.6] 
-00003710: 4765 7420 6368 696c 6472 656e 206f 6620  Get children of 
-00003720: 7468 6520 6576 656e 742e 2054 6865 7265  the event. There
-00003730: 2069 7320 616c 736f 2069 7465 7261 626c   is also iterabl
-00003740: 6520 7665 7273 696f 6e20 2767 6574 5f63  e version 'get_c
-00003750: 6869 6c64 7265 6e5f 6974 6572 272e 0a63  hildren_iter'..c
-00003760: 6869 6c64 7265 6e3a 2054 7570 6c65 5b64  hildren: Tuple[d
-00003770: 6963 745d 203d 2065 7463 2e67 6574 5f63  ict] = etc.get_c
-00003780: 6869 6c64 7265 6e28 2238 3134 3432 3265  hildren("814422e
-00003790: 312d 3963 3638 2d31 3165 622d 3835 3938  1-9c68-11eb-8598
-000037a0: 2d36 3931 6562 6437 6634 3133 6422 290a  -691ebd7f413d").
-000037b0: 0a23 205b 332e 332e 375d 2047 6574 2073  .# [3.3.7] Get s
-000037c0: 7562 7472 6565 2066 6f72 2073 7065 6369  ubtree for speci
-000037d0: 6669 6564 2065 7665 6e74 2e0a 7375 6274  fied event..subt
-000037e0: 7265 653a 2045 7665 6e74 5472 6565 203d  ree: EventTree =
-000037f0: 2065 7463 2e67 6574 5f73 7562 7472 6565   etc.get_subtree
-00003800: 2822 3865 3233 3737 3464 2d63 6635 392d  ("8e23774d-cf59-
-00003810: 3131 6562 2d61 3665 332d 3535 6266 6462  11eb-a6e3-55bfdb
-00003820: 3262 3366 3231 2229 0a0a 2320 5b33 2e33  2b3f21")..# [3.3
-00003830: 2e38 5d20 4765 7420 6675 6c6c 2070 6174  .8] Get full pat
-00003840: 6820 746f 2074 6865 2065 7665 6e74 2e0a  h to the event..
-00003850: 2320 4c6f 6f6b 7320 6c69 6b65 205b 616e  # Looks like [an
-00003860: 6365 7374 6f72 5f72 6f6f 742c 2061 6e63  cestor_root, anc
-00003870: 6573 746f 725f 6c65 7665 6c31 2c20 616e  estor_level1, an
-00003880: 6365 7374 6f72 5f6c 6576 656c 322c 2065  cestor_level2, e
-00003890: 7665 6e74 5d0a 6576 656e 745f 7061 7468  vent].event_path
-000038a0: 3a20 4c69 7374 5b64 6963 745d 203d 2065  : List[dict] = e
-000038b0: 7463 2e67 6574 5f66 756c 6c5f 7061 7468  tc.get_full_path
-000038c0: 2822 3865 3235 3234 6661 2d63 6635 392d  ("8e2524fa-cf59-
-000038d0: 3131 6562 2d61 3366 372d 3039 3466 3930  11eb-a3f7-094f90
-000038e0: 3463 3361 3632 2229 0a0a 2320 5b33 2e33  4c3a62")..# [3.3
-000038f0: 2e39 5d20 4765 7420 7061 7265 6e74 206f  .9] Get parent o
-00003900: 6620 7468 6520 6576 656e 742e 0a70 6172  f the event..par
-00003910: 656e 7420 3d20 6574 632e 6765 745f 7061  ent = etc.get_pa
-00003920: 7265 6e74 2822 3865 3235 3234 6661 2d63  rent("8e2524fa-c
-00003930: 6635 392d 3131 6562 2d61 3366 372d 3039  f59-11eb-a3f7-09
-00003940: 3466 3930 3463 3361 3632 2229 0a0a 2320  4f904c3a62")..# 
-00003950: 5b33 2e33 2e31 305d 2041 7070 656e 6420  [3.3.10] Append 
-00003960: 6e65 7720 6576 656e 7420 746f 2074 6865  new event to the
-00003970: 2063 6f6c 6c65 6374 696f 6e2e 0a65 7463   collection..etc
-00003980: 2e61 7070 656e 645f 6576 656e 7428 0a20  .append_event(. 
-00003990: 2020 2065 7665 6e74 3d7b 0a20 2020 2020     event={.     
-000039a0: 2020 2022 6576 656e 7449 6422 3a20 2261     "eventId": "a
-000039b0: 3230 6635 6566 342d 6333 6665 2d62 6231  20f5ef4-c3fe-bb1
-000039c0: 302d 6132 3963 2d64 6433 6437 3834 3930  0-a29c-dd3d78490
-000039d0: 3965 6222 2c0a 2020 2020 2020 2020 2270  9eb",.        "p
-000039e0: 6172 656e 7445 7665 6e74 4964 223a 2022  arentEventId": "
-000039f0: 3865 3235 3234 6661 2d63 6635 392d 3131  8e2524fa-cf59-11
-00003a00: 6562 2d61 3366 372d 3039 3466 3930 3463  eb-a3f7-094f904c
-00003a10: 3361 3632 222c 0a20 2020 2020 2020 2022  3a62",.        "
-00003a20: 6576 656e 744e 616d 6522 3a20 2253 7475  eventName": "Stu
-00003a30: 6245 7665 6e74 222c 0a20 2020 207d 0a29  bEvent",.    }.)
-00003a40: 0a0a 2320 5b33 2e33 2e31 315d 2053 686f  ..# [3.3.11] Sho
-00003a50: 7720 7468 6520 656e 7469 7265 2063 6f6c  w the entire col
-00003a60: 6c65 6374 696f 6e2e 0a65 7463 2e73 686f  lection..etc.sho
-00003a70: 7728 290a 0a23 205b 332e 345d 2057 6f72  w()..# [3.4] Wor
-00003a80: 6b69 6e67 2077 6974 6820 7468 6520 4576  king with the Ev
-00003a90: 656e 7454 7265 652e 0a23 2045 7665 6e74  entTree..# Event
-00003aa0: 5472 6565 2068 6173 2074 6865 2073 616d  Tree has the sam
-00003ab0: 6520 6d65 7468 6f64 7320 6173 2045 7665  e methods as Eve
-00003ac0: 6e74 5472 6565 436f 6c6c 6563 7469 6f6e  ntTreeCollection
-00003ad0: 2c20 6275 7420 6f6e 6c79 2066 6f72 2069  , but only for i
-00003ae0: 7473 206f 776e 2074 7265 652e 0a0a 2320  ts own tree...# 
-00003af0: 5b33 2e34 2e31 5d20 4765 7420 636f 6c6c  [3.4.1] Get coll
-00003b00: 6563 7469 6f6e 2074 7265 6573 2e0a 7472  ection trees..tr
-00003b10: 6565 733a 204c 6973 745b 4576 656e 7454  ees: List[EventT
-00003b20: 7265 655d 203d 2065 7463 2e67 6574 5f74  ree] = etc.get_t
-00003b30: 7265 6573 2829 0a74 7265 653a 2045 7665  rees().tree: Eve
-00003b40: 6e74 5472 6565 203d 2074 7265 6573 5b30  ntTree = trees[0
-00003b50: 5d0a 0a23 2042 7574 2045 7665 6e74 5472  ]..# But EventTr
-00003b60: 6565 2070 726f 7669 6465 7320 6120 776f  ee provides a wo
-00003b70: 726b 2077 6974 6820 7468 6520 7472 6565  rk with the tree
-00003b80: 2c20 6275 7420 646f 6573 206e 6f74 206d  , but does not m
-00003b90: 6f64 6966 7920 6974 2e0a 2320 4966 2079  odify it..# If y
-00003ba0: 6f75 2077 616e 7420 746f 206d 6f64 6966  ou want to modif
-00003bb0: 7920 7468 6520 7472 6565 2c20 7573 6520  y the tree, use 
-00003bc0: 4576 656e 7454 7265 6543 6f6c 6c65 6374  EventTreeCollect
-00003bd0: 696f 6e73 2e0a 0a23 205b 332e 355d 2057  ions...# [3.5] W
-00003be0: 6f72 6b69 6e67 2077 6974 6820 5061 7265  orking with Pare
-00003bf0: 6e74 6c65 7373 5472 6565 2e0a 2320 5061  ntlessTree..# Pa
-00003c00: 7265 6e74 6c65 7373 5472 6565 2069 7320  rentlessTree is 
-00003c10: 4576 656e 7454 7265 6520 7768 6963 6820  EventTree which 
-00003c20: 6861 7320 6465 7461 6368 6564 2065 7665  has detached eve
-00003c30: 6e74 7320 7769 7468 2073 7475 6273 2e0a  nts with stubs..
-00003c40: 7061 7265 6e74 6c65 7373 5f74 7265 6573  parentless_trees
-00003c50: 3a20 4c69 7374 5b45 7665 6e74 5472 6565  : List[EventTree
-00003c60: 5d20 3d20 6574 632e 6765 745f 7061 7265  ] = etc.get_pare
-00003c70: 6e74 6c65 7373 5f74 7265 6573 2829 0a0a  ntless_trees()..
-00003c80: 2320 5b33 2e36 5d20 576f 726b 696e 6720  # [3.6] Working 
-00003c90: 7769 7468 2050 6172 656e 7445 7665 6e74  with ParentEvent
-00003ca0: 5472 6565 436f 6c6c 6563 7469 6f6e 2e0a  TreeCollection..
-00003cb0: 2320 5061 7265 6e74 4576 656e 7454 7265  # ParentEventTre
-00003cc0: 6543 6f6c 6c65 6374 696f 6e20 6973 2061  eCollection is a
-00003cd0: 2074 7265 6520 636f 6c6c 6563 7469 6f6e   tree collection
-00003ce0: 206c 696b 6520 4576 656e 7454 7265 6543   like EventTreeC
-00003cf0: 6f6c 6c65 6374 696f 6e2c 0a23 2062 7574  ollection,.# but
-00003d00: 2069 7420 6861 7320 6f6e 6c79 2065 7665   it has only eve
-00003d10: 6e74 7320 7468 6174 2068 6176 6520 7265  nts that have re
-00003d20: 6665 7265 6e63 6573 2e0a 6461 7461 5f73  ferences..data_s
-00003d30: 6f75 7263 653a 2049 4461 7461 536f 7572  ource: IDataSour
-00003d40: 6365 2020 2320 596f 7520 7368 6f75 6c64  ce  # You should
-00003d50: 2069 6e69 7420 4461 7461 536f 7572 6365   init DataSource
-00003d60: 206f 626a 6563 742e 2045 2e67 2e20 6672   object. E.g. fr
-00003d70: 6f6d 204c 7744 5020 6d6f 6475 6c65 2e0a  om LwDP module..
-00003d80: 2320 4554 4344 7269 7665 7220 6865 7265  # ETCDriver here
-00003d90: 2069 7320 6120 7374 7562 2c20 6163 7475   is a stub, actu
-00003da0: 616c 6c79 2074 6865 206c 6962 2064 6f6e  ally the lib don
-00003db0: 2774 2068 6176 6520 7375 6368 2063 6c61  't have such cla
-00003dc0: 7373 2e0a 2320 596f 7520 6361 6e20 7461  ss..# You can ta
-00003dd0: 6b65 2069 7420 696e 204c 7744 5020 6d6f  ke it in LwDP mo
-00003de0: 6475 6c65 206f 7220 6372 6561 7465 2079  dule or create y
-00003df0: 6f75 7273 656c 6620 636c 6173 7320 6966  ourself class if
-00003e00: 2079 6f75 2068 6176 6520 736f 6d65 2073   you have some s
-00003e10: 7065 6369 616c 2065 7665 6e74 7320 7374  pecial events st
-00003e20: 7275 6374 7572 652e 0a66 726f 6d20 7468  ructure..from th
-00003e30: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
-00003e40: 6461 7461 5f73 6f75 7263 652e 6c77 6470  data_source.lwdp
-00003e50: 2e65 7665 6e74 5f74 7265 6520 696d 706f  .event_tree impo
-00003e60: 7274 2048 7474 7045 5443 4472 6976 6572  rt HttpETCDriver
-00003e70: 2061 7320 4554 4344 7269 7665 720a 0a64   as ETCDriver..d
-00003e80: 7269 7665 7220 3d20 4554 4344 7269 7665  river = ETCDrive
-00003e90: 7228 6461 7461 5f73 6f75 7263 653d 6461  r(data_source=da
-00003ea0: 7461 5f73 6f75 7263 6529 0a65 7463 203d  ta_source).etc =
-00003eb0: 2050 6172 656e 7445 7665 6e74 5472 6565   ParentEventTree
-00003ec0: 436f 6c6c 6563 7469 6f6e 2864 7269 7665  Collection(drive
-00003ed0: 7229 0a65 7463 2e62 7569 6c64 2865 7665  r).etc.build(eve
-00003ee0: 6e74 7329 0a0a 6574 632e 7368 6f77 2829  nts)..etc.show()
-00003ef0: 0a0a 2320 5b34 5d20 4669 656c 6420 5265  ..# [4] Field Re
-00003f00: 736f 6c76 6572 730a 2320 506c 6561 7365  solvers.# Please
-00003f10: 2072 6561 6420 6046 6965 6c64 2052 6573   read `Field Res
-00003f20: 6f6c 7665 7273 6020 626c 6f63 6b20 696e  olvers` block in
-00003f30: 2072 6561 646d 6520 6669 7273 742e 0a23   readme first..#
-00003f40: 205b 342e 315d 2055 7361 6765 2065 7861   [4.1] Usage exa
-00003f50: 6d70 6c65 2066 726f 6d20 636c 6965 6e74  mple from client
-00003f60: 2063 6f64 650a 6672 6f6d 2074 6832 5f64   code.from th2_d
-00003f70: 6174 615f 7365 7276 6963 6573 2e64 6174  ata_services.dat
-00003f80: 615f 736f 7572 6365 2069 6d70 6f72 7420  a_source import 
-00003f90: 280a 2020 2020 6c77 6470 2c0a 2920 2023  (.    lwdp,.)  #
-00003fa0: 206c 7764 7020 6461 7461 5f73 6f75 7263   lwdp data_sourc
-00003fb0: 6520 696e 6974 6961 6c69 7a65 2074 6832  e initialize th2
-00003fc0: 5f64 6174 615f 7365 7276 6963 6573 2e63  _data_services.c
-00003fd0: 6f6e 6669 6720 6475 7269 6e67 2069 6d70  onfig during imp
-00003fe0: 6f72 742e 0a66 726f 6d20 7468 325f 6461  ort..from th2_da
-00003ff0: 7461 5f73 6572 7669 6365 732e 636f 6e66  ta_services.conf
-00004000: 6967 2069 6d70 6f72 7420 6f70 7469 6f6e  ig import option
-00004010: 7320 6173 206f 5f0a 0a66 6f72 206d 2069  s as o_..for m i
-00004020: 6e20 6461 7461 3a0a 2020 2020 6f5f 2e6d  n data:.    o_.m
-00004030: 6672 2e65 7870 616e 645f 6d65 7373 6167  fr.expand_messag
-00004040: 6528 6d29 2020 2320 6d66 7220 2d20 7374  e(m)  # mfr - st
-00004050: 616e 6473 2066 6f72 204d 6573 7361 6765  ands for Message
-00004060: 4669 656c 6452 6573 6f6c 7665 720a 2020  FieldResolver.  
-00004070: 2020 2320 6f72 0a20 2020 206f 5f2e 656d    # or.    o_.em
-00004080: 6672 2e65 7870 616e 645f 6d65 7373 6167  fr.expand_messag
-00004090: 6528 6d29 2020 2320 656d 6672 202d 2073  e(m)  # emfr - s
-000040a0: 7461 6e64 7320 666f 7220 4578 7061 6e64  tands for Expand
-000040b0: 6564 4d65 7373 6167 6546 6965 6c64 5265  edMessageFieldRe
-000040c0: 736f 6c76 6572 0a0a 2320 5b34 2e32 5d20  solver..# [4.2] 
-000040d0: 4c69 6272 6172 6965 7320 7573 6167 652e  Libraries usage.
-000040e0: 0a23 2044 6f6e 2774 2069 6d70 6f72 7420  .# Don't import 
-000040f0: 6578 6163 7420 7265 736f 6c76 6572 7320  exact resolvers 
-00004100: 696d 706c 656d 656e 7461 7469 6f6e 2070  implementation p
-00004110: 6c65 6173 6520 696e 2079 6f75 7220 636f  lease in your co
-00004120: 6465 2e0a 2320 416c 6c6f 7720 796f 7572  de..# Allow your
-00004130: 2063 6c69 656e 7420 746f 2064 6f20 6974   client to do it
-00004140: 2069 6e73 7465 6164 2e0a 2320 4a75 7374   instead..# Just
-00004150: 2069 6d70 6f72 7420 606f 7074 696f 6e73   import `options
-00004160: 6020 6672 6f6d 2060 7468 325f 6461 7461  ` from `th2_data
-00004170: 5f73 6572 7669 6365 732e 636f 6e66 6967  _services.config
-00004180: 6020 616e 6420 7573 6520 6974 2e0a 6672  ` and use it..fr
-00004190: 6f6d 2074 6832 5f64 6174 615f 7365 7276  om th2_data_serv
-000041a0: 6963 6573 2e63 6f6e 6669 6720 696d 706f  ices.config impo
-000041b0: 7274 206f 7074 696f 6e73 2061 7320 6f5f  rt options as o_
-000041c0: 0a0a 666f 7220 6d20 696e 2064 6174 613a  ..for m in data:
-000041d0: 0a20 2020 206f 5f2e 6d66 722e 6578 7061  .    o_.mfr.expa
-000041e0: 6e64 5f6d 6573 7361 6765 286d 290a 2020  nd_message(m).  
-000041f0: 2020 2320 6f72 0a20 2020 206f 5f2e 656d    # or.    o_.em
-00004200: 6672 2e65 7870 616e 645f 6d65 7373 6167  fr.expand_messag
-00004210: 6528 6d29 0a0a 2320 4d6f 7265 2074 6563  e(m)..# More tec
-00004220: 6820 6465 7461 696c 733a 0a23 2020 2049  h details:.#   I
-00004230: 6e20 7468 6973 2063 6173 652c 2074 6865  n this case, the
-00004240: 7265 2069 7320 6e6f 206c 696e 6520 6066  re is no line `f
-00004250: 726f 6d20 7468 325f 6461 7461 5f73 6572  rom th2_data_ser
-00004260: 7669 6365 732e 6461 7461 5f73 6f75 7263  vices.data_sourc
-00004270: 6520 696d 706f 7274 206c 7764 7020 600a  e import lwdp `.
-00004280: 2320 2020 6265 6361 7573 6520 7765 2073  #   because we s
-00004290: 686f 756c 6420 6e6f 7420 6368 6f6f 7365  hould not choose
-000042a0: 2066 6f72 2074 6865 2075 7365 7220 7768   for the user wh
-000042b0: 6963 6820 6461 7461 2073 6f75 7263 6520  ich data source 
-000042c0: 746f 2075 7365 2e0a 2320 2020 5765 2064  to use..#   We d
-000042d0: 6f20 6e6f 7420 6b6e 6f77 2077 6861 7420  o not know what 
-000042e0: 6865 2077 696c 6c20 6368 6f6f 7365 2c20  he will choose, 
-000042f0: 7468 6572 6566 6f72 6520 7765 206d 7573  therefore we mus
-00004300: 7420 7369 6d70 6c79 2061 6363 6573 730a  t simply access.
-00004310: 2320 2020 7468 6520 696e 7465 7266 6163  #   the interfac
-00004320: 652c 2077 6869 6368 2077 696c 6c20 6265  e, which will be
-00004330: 2069 6e69 7469 616c 697a 6564 2062 7920   initialized by 
-00004340: 7468 6520 7573 6572 2e0a 0a23 205b 355d  the user...# [5]
-00004350: 2055 7369 6e67 2075 7469 6c69 7479 2066   Using utility f
-00004360: 756e 6374 696f 6e73 2e0a 6672 6f6d 2074  unctions..from t
-00004370: 6832 5f64 6174 615f 7365 7276 6963 6573  h2_data_services
-00004380: 2e75 7469 6c73 2e65 7665 6e74 5f75 7469  .utils.event_uti
-00004390: 6c73 2e66 7265 7175 656e 6369 6573 2069  ls.frequencies i
-000043a0: 6d70 6f72 7420 6765 745f 6361 7465 676f  mport get_catego
-000043b0: 7279 5f66 7265 7175 656e 6369 6573 320a  ry_frequencies2.
-000043c0: 6672 6f6d 2074 6832 5f64 6174 615f 7365  from th2_data_se
-000043d0: 7276 6963 6573 2e75 7469 6c73 2e65 7665  rvices.utils.eve
-000043e0: 6e74 5f75 7469 6c73 2e74 6f74 616c 7320  nt_utils.totals 
-000043f0: 696d 706f 7274 2067 6574 5f63 6174 6567  import get_categ
-00004400: 6f72 795f 746f 7461 6c73 320a 6672 6f6d  ory_totals2.from
-00004410: 2074 6832 5f64 6174 615f 7365 7276 6963   th2_data_servic
-00004420: 6573 2e75 7469 6c73 2e63 6174 6567 6f72  es.utils.categor
-00004430: 7920 696d 706f 7274 2043 6174 6567 6f72  y import Categor
-00004440: 790a 6672 6f6d 2074 6832 5f64 6174 615f  y.from th2_data_
-00004450: 7365 7276 6963 6573 2e75 7469 6c73 2e65  services.utils.e
-00004460: 7665 6e74 5f75 7469 6c73 2e65 7665 6e74  vent_utils.event
-00004470: 5f75 7469 6c73 2069 6d70 6f72 7420 6973  _utils import is
-00004480: 5f73 6f72 7465 640a 0a23 205b 352e 315d  _sorted..# [5.1]
-00004490: 2047 6574 2074 6865 2071 7561 6e74 6974   Get the quantit
-000044a0: 6965 7320 6f66 2065 7665 6e74 7320 666f  ies of events fo
-000044b0: 7220 6469 6666 6572 656e 7420 6361 7465  r different cate
-000044c0: 676f 7269 6573 2e0a 6d65 7472 6963 7320  gories..metrics 
-000044d0: 3d20 5b0a 2020 2020 4361 7465 676f 7279  = [.    Category
-000044e0: 2822 6461 7465 222c 206c 616d 6264 6120  ("date", lambda 
-000044f0: 6d3a 2054 6832 5469 6d65 7374 616d 7043  m: Th2TimestampC
-00004500: 6f6e 7665 7274 6572 2e74 6f5f 6461 7465  onverter.to_date
-00004510: 7469 6d65 286d 5b22 7374 6172 7454 696d  time(m["startTim
-00004520: 6573 7461 6d70 225d 292e 6461 7465 2829  estamp"]).date()
-00004530: 292c 0a20 2020 2043 6174 6567 6f72 7928  ),.    Category(
-00004540: 2273 7461 7475 7322 2c20 6c61 6d62 6461  "status", lambda
-00004550: 206d 3a20 6d5b 2273 7563 6365 7373 6675   m: m["successfu
-00004560: 6c22 5d29 2c0a 5d0a 6361 7465 676f 7279  l"]),.].category
-00004570: 5f74 6f74 616c 7320 3d20 6765 745f 6361  _totals = get_ca
-00004580: 7465 676f 7279 5f74 6f74 616c 7332 2865  tegory_totals2(e
-00004590: 7665 6e74 732c 206d 6574 7269 6373 290a  vents, metrics).
-000045a0: 2222 220a 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d  """.+--------+--
-000045b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
-000045c0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b  -----+---------+
-000045d0: 0a7c 2020 2020 2020 2020 7c20 6461 7465  .|        | date
-000045e0: 2020 2020 2020 207c 2073 7461 7475 7320         | status 
-000045f0: 2020 7c20 2020 636f 756e 7420 7c0a 2b3d    |   count |.+=
-00004600: 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d  =======+========
-00004610: 3d3d 3d3d 2b3d 3d3d 3d3d 3d3d 3d3d 3d2b  ====+==========+
-00004620: 3d3d 3d3d 3d3d 3d3d 3d2b 0a7c 2020 2020  =========+.|    
-00004630: 2020 2020 7c20 3230 3233 2d30 312d 3035      | 2023-01-05
-00004640: 207c 2054 7275 6520 2020 2020 7c20 2020   | True     |   
-00004650: 2020 2020 3320 7c0a 2b2d 2d2d 2d2d 2d2d      3 |.+-------
-00004660: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  -+------------+-
-00004670: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
-00004680: 2d2d 2d2b 0a7c 2063 6f75 6e74 2020 7c20  ---+.| count  | 
-00004690: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-000046a0: 2020 2020 2020 7c20 2020 2020 2020 3120        |       1 
-000046b0: 7c0a 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  |.+--------+----
-000046c0: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-000046d0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c  ---+---------+.|
-000046e0: 2074 6f74 616c 7320 7c20 2020 2020 2020   totals |       
-000046f0: 2020 2020 207c 2031 2f30 2020 2020 2020       | 1/0      
-00004700: 7c20 2020 2020 2020 3320 7c0a 2b2d 2d2d  |       3 |.+---
-00004710: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
-00004720: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  --+----------+--
-00004730: 2d2d 2d2d 2d2d 2d2b 0a22 2222 0a0a 2320  -------+."""..# 
-00004740: 5b35 2e32 5d20 4765 7420 7468 6520 6e75  [5.2] Get the nu
-00004750: 6d62 6572 206f 6620 6576 656e 7473 2077  mber of events w
-00004760: 6974 6820 7374 6174 7573 2073 7563 6365  ith status succe
-00004770: 7373 6675 6c2e 0a63 6174 6567 6f72 7920  ssful..category 
-00004780: 3d20 4361 7465 676f 7279 2822 7374 6174  = Category("stat
-00004790: 7573 222c 206c 616d 6264 6120 6d3a 206d  us", lambda m: m
-000047a0: 5b22 7375 6363 6573 7366 756c 225d 290a  ["successful"]).
-000047b0: 6361 7465 676f 7279 5f66 7265 7175 656e  category_frequen
-000047c0: 6369 6573 203d 2067 6574 5f63 6174 6567  cies = get_categ
-000047d0: 6f72 795f 6672 6571 7565 6e63 6965 7332  ory_frequencies2
-000047e0: 2865 7665 6e74 732c 2063 6174 6567 6f72  (events, categor
-000047f0: 7929 0a22 2222 0a2b 2d2d 2d2d 2d2d 2d2d  y).""".+--------
-00004800: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-00004810: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
-00004820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
-00004830: 2d2d 2d2d 2d2b 0a7c 2020 2020 2020 2020  -----+.|        
-00004840: 7c20 7469 6d65 7374 616d 705f 7374 6172  | timestamp_star
-00004850: 7420 2020 2020 7c20 7469 6d65 7374 616d  t     | timestam
-00004860: 705f 656e 6420 2020 2020 2020 7c20 2020  p_end       |   
-00004870: 5472 7565 207c 0a2b 3d3d 3d3d 3d3d 3d3d  True |.+========
-00004880: 2b3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  +===============
-00004890: 3d3d 3d3d 3d3d 2b3d 3d3d 3d3d 3d3d 3d3d  ======+=========
-000048a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2b3d 3d3d  ============+===
-000048b0: 3d3d 3d3d 3d2b 0a7c 2020 2020 2020 2020  =====+.|        
-000048c0: 7c20 3230 3233 2d30 312d 3035 5431 333a  | 2023-01-05T13:
-000048d0: 3537 3a30 3520 7c20 3230 3233 2d30 312d  57:05 | 2023-01-
-000048e0: 3035 5431 333a 3537 3a30 3620 7c20 2020  05T13:57:06 |   
-000048f0: 2020 2033 207c 0a2b 2d2d 2d2d 2d2d 2d2d     3 |.+--------
-00004900: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-00004910: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
-00004920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
-00004930: 2d2d 2d2d 2d2b 0a7c 2063 6f75 6e74 2020  -----+.| count  
-00004940: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00004950: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00004960: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00004970: 2020 2031 207c 0a2b 2d2d 2d2d 2d2d 2d2d     1 |.+--------
-00004980: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-00004990: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
-000049a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
-000049b0: 2d2d 2d2d 2d2b 0a7c 2074 6f74 616c 7320  -----+.| totals 
-000049c0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-000049d0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-000049e0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-000049f0: 2020 2033 207c 0a2b 2d2d 2d2d 2d2d 2d2d     3 |.+--------
-00004a00: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-00004a10: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
-00004a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
-00004a30: 2d2d 2d2d 2d2b 0a22 2222 0a0a 2320 5b35  -----+."""..# [5
-00004a40: 2e33 5d20 4368 6563 6b20 6966 2065 7665  .3] Check if eve
-00004a50: 6e74 7320 6172 6520 736f 7274 6564 2e0a  nts are sorted..
-00004a60: 7265 7375 6c74 203d 2069 735f 736f 7274  result = is_sort
-00004a70: 6564 2865 7665 6e74 7329 0a60 6060 0a3c  ed(events).```.<
-00004a80: 212d 2d20 656e 6420 6765 745f 7374 6172  !-- end get_star
-00004a90: 7465 645f 6578 616d 706c 652e 7079 202d  ted_example.py -
-00004aa0: 2d3e 0a0a 2323 2032 2e33 2e20 5368 6f72  ->..## 2.3. Shor
-00004ab0: 7420 7468 656f 7279 0a0a 5468 6520 6c69  t theory..The li
-00004ac0: 6272 6172 7920 7072 6f76 6964 6573 2074  brary provides t
-00004ad0: 6f6f 6c73 2066 6f72 2068 616e 646c 696e  ools for handlin
-00004ae0: 6720 7374 7265 616d 2064 6174 612e 2057  g stream data. W
-00004af0: 6861 7427 7320 6120 7374 7265 616d 3f20  hat's a stream? 
-00004b00: 4974 2773 2061 2073 6571 7565 6e63 6520  It's a sequence 
-00004b10: 6f66 2065 6c65 6d65 6e74 7320 6672 6f6d  of elements from
-00004b20: 2061 2073 6f75 7263 6520 7468 6174 0a73   a source that.s
-00004b30: 7570 706f 7274 7320 6167 6772 6567 6174  upports aggregat
-00004b40: 6520 6f70 6572 6174 696f 6e73 2e0a 0a23  e operations...#
-00004b50: 2323 2054 6572 6d73 0a0a 2d20 2a2a 4461  ## Terms..- **Da
-00004b60: 7461 206f 626a 6563 742a 2a3a 2041 6e20  ta object**: An 
-00004b70: 696e 7374 616e 6365 206f 6620 6044 6174  instance of `Dat
-00004b80: 6160 2063 6c61 7373 2077 6869 6368 2069  a` class which i
-00004b90: 7320 7772 6170 7065 7220 756e 6465 7220  s wrapper under 
-00004ba0: 7374 7265 616d 2e0a 2d20 2a2a 5365 7175  stream..- **Sequ
-00004bb0: 656e 6365 206f 6620 656c 656d 656e 7473  ence of elements
-00004bc0: 2a2a 3a0a 2020 4120 5f44 6174 6120 6f62  **:.  A _Data ob
-00004bd0: 6a65 6374 5f20 7072 6f76 6964 6573 2061  ject_ provides a
-00004be0: 6e20 696e 7465 7266 6163 6520 746f 2061  n interface to a
-00004bf0: 2073 6571 7565 6e63 6564 2073 6574 206f   sequenced set o
-00004c00: 6620 7661 6c75 6573 206f 6620 6120 7370  f values of a sp
-00004c10: 6563 6966 6963 2065 6c65 6d65 6e74 2074  ecific element t
-00004c20: 7970 652e 2053 7472 6561 6d20 696e 7369  ype. Stream insi
-00004c30: 6465 2074 6865 205f 4461 7461 0a20 206f  de the _Data.  o
-00004c40: 626a 6563 745f 202a 2a64 6f6e 1974 2061  bject_ **don.t a
-00004c50: 6374 7561 6c6c 7920 7374 6f72 652a 2a20  ctually store** 
-00004c60: 656c 656d 656e 7473 3b20 7468 6579 2061  elements; they a
-00004c70: 7265 2063 6f6d 7075 7465 6420 6f6e 2064  re computed on d
-00004c80: 656d 616e 642e 0a2d 202a 2a64 6174 6120  emand..- **data 
-00004c90: 736f 7572 6365 2a2a 2028 6578 6163 746c  source** (exactl
-00004ca0: 7920 696e 2073 6d61 6c6c 206c 6574 7465  y in small lette
-00004cb0: 7273 293a 0a20 2041 6e79 2073 6f75 7263  rs):.  Any sourc
-00004cc0: 6520 6f66 2064 6174 612e 2045 2e67 2e20  e of data. E.g. 
-00004cd0: 5b4c 6967 6874 7765 6967 6874 2044 6174  [Lightweight Dat
-00004ce0: 6120 5072 6f76 6964 6572 5d28 6874 7470  a Provider](http
-00004cf0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
-00004d00: 6832 2d6e 6574 2f74 6832 2d6c 772d 6461  h2-net/th2-lw-da
-00004d10: 7461 2d70 726f 7669 6465 7229 2c20 636f  ta-provider), co
-00004d20: 6c6c 6563 7469 6f6e 732c 0a20 2061 7272  llections,.  arr
-00004d30: 6179 732c 206f 7220 492f 4f20 7265 736f  ays, or I/O reso
-00004d40: 7572 6365 732e 0a2d 202a 2a44 6174 6153  urces..- **DataS
-00004d50: 6f75 7263 652a 2a3a 0a20 2041 2063 6c61  ource**:.  A cla
-00004d60: 7373 2074 6861 7420 6973 2061 6e20 696e  ss that is an in
-00004d70: 7465 726d 6564 6961 7465 206c 696e 6b20  termediate link 
-00004d80: 6265 7477 6565 6e20 7468 6520 536f 7572  between the Sour
-00004d90: 6365 4150 4920 616e 6420 436f 6d6d 616e  ceAPI and Comman
-00004da0: 6473 2e0a 2d20 2a2a 536f 7572 6365 4150  ds..- **SourceAP
-00004db0: 492a 2a3a 0a20 2045 6163 6820 736f 7572  I**:.  Each sour
-00004dc0: 6365 2068 6173 2069 7473 206f 776e 2041  ce has its own A
-00004dd0: 5049 2074 6f20 7265 7472 6965 7665 2064  PI to retrieve d
-00004de0: 6174 612e 2053 6f75 7263 6541 5049 2069  ata. SourceAPI i
-00004df0: 7320 6120 636c 6173 7320 7468 6174 2070  s a class that p
-00004e00: 726f 7669 6465 2041 5049 2066 6f72 2073  rovide API for s
-00004e10: 6f6d 6520 6461 7461 2073 6f75 7263 652e  ome data source.
-00004e20: 0a2d 202a 2a43 6f6d 6d61 6e64 732a 2a3a  .- **Commands**:
-00004e30: 0a20 2043 6c61 7373 6573 2074 6861 7420  .  Classes that 
-00004e40: 7072 6f76 6964 6520 7573 6572 2d66 7269  provide user-fri
-00004e50: 656e 646c 7920 696e 7465 7266 6163 6573  endly interfaces
-00004e60: 2066 6f72 2067 6574 7469 6e67 2073 6f6d   for getting som
-00004e70: 6520 6461 7461 2066 726f 6d20 4461 7461  e data from Data
-00004e80: 536f 7572 6365 2e20 436f 6d6d 616e 6473  Source. Commands
-00004e90: 2075 7365 205f 536f 7572 6365 4150 495f   use _SourceAPI_
-00004ea0: 2074 6f0a 2020 6163 6869 6576 6520 6974   to.  achieve it
-00004eb0: 2e0a 2d20 2a2a 4164 6170 7465 7273 2a2a  ..- **Adapters**
-00004ec0: 3a0a 2020 4974 2773 2073 696d 696c 6172  :.  It's similar
-00004ed0: 2074 6f20 6675 6e63 7469 6f6e 2066 6f72   to function for
-00004ee0: 2060 4461 7461 2e6d 6170 6020 6d65 7468   `Data.map` meth
-00004ef0: 6f64 2e20 4164 6f70 7461 626c 6520 636f  od. Adoptable co
-00004f00: 6d6d 616e 6473 2075 7365 6420 6974 2074  mmands used it t
-00004f10: 6f20 7570 6461 7465 2074 6865 2064 6174  o update the dat
-00004f20: 6120 7374 7265 616d 2e0a 2d20 2a2a 4167  a stream..- **Ag
-00004f30: 6772 6567 6174 6520 6f70 6572 6174 696f  gregate operatio
-00004f40: 6e73 2a2a 3a0a 2020 436f 6d6d 6f6e 206f  ns**:.  Common o
-00004f50: 7065 7261 7469 6f6e 7320 7375 6368 2061  perations such a
-00004f60: 7320 6669 6c74 6572 2c20 6d61 702c 206c  s filter, map, l
-00004f70: 696d 6974 2061 6e64 2073 6f20 6f6e 2e0a  imit and so on..
-00004f80: 2d20 2a2a 576f 726b 666c 6f77 2a2a 3a20  - **Workflow**: 
-00004f90: 416e 206f 7264 6572 6564 2073 6574 206f  An ordered set o
-00004fa0: 6620 5f41 6767 7265 6761 7465 206f 7065  f _Aggregate ope
-00004fb0: 7261 7469 6f6e 735f 2e0a 0a23 2323 2043  rations_...### C
-00004fc0: 6f6e 6365 7074 0a0a 5468 6520 6c69 6272  oncept..The libr
-00004fd0: 6172 7920 6465 7363 7269 6265 7320 7468  ary describes th
-00004fe0: 6520 6869 6768 2d6c 6576 656c 2069 6e74  e high-level int
-00004ff0: 6572 6661 6365 7320 6049 536f 7572 6365  erfaces `ISource
-00005000: 4150 4960 2c20 6049 4461 7461 536f 7572  API`, `IDataSour
-00005010: 6365 602c 2060 4943 6f6d 6d61 6e64 602c  ce`, `ICommand`,
-00005020: 2060 4941 6461 7074 6572 602e 0a0a 416e   `IAdapter`...An
-00005030: 7920 6461 7461 2073 6f75 7263 6520 6d75  y data source mu
-00005040: 7374 2062 6520 6465 7363 7269 6265 6420  st be described 
-00005050: 6279 2074 6865 2060 4944 6174 6153 6f75  by the `IDataSou
-00005060: 7263 6560 2061 6273 7472 6163 7420 636c  rce` abstract cl
-00005070: 6173 732e 2054 6865 7365 2063 616e 2062  ass. These can b
-00005080: 6520 5f46 696c 6544 6174 6153 6f75 7263  e _FileDataSourc
-00005090: 655f 2c0a 5f43 5356 4461 7461 536f 7572  e_,._CSVDataSour
-000050a0: 6365 5f2c 205f 4442 4461 7461 536f 7572  ce_, _DBDataSour
-000050b0: 6365 5f20 616e 6420 6f74 6865 722e 0a0a  ce_ and other...
-000050c0: 5573 7561 6c6c 792c 2064 6174 6120 736f  Usually, data so
-000050d0: 7572 6365 7320 6861 7665 2073 6f6d 6520  urces have some 
-000050e0: 6b69 6e64 206f 6620 4150 492e 2044 6174  kind of API. Dat
-000050f0: 6162 6173 6573 202d 2070 726f 7669 6465  abases - provide
-00005100: 2053 514c 206c 616e 6775 6167 652c 2077   SQL language, w
-00005110: 6865 6e20 776f 726b 696e 6720 7769 7468  hen working with
-00005120: 2061 2066 696c 652c 2079 6f75 2063 616e   a file, you can
-00005130: 2072 6561 640a 6c69 6e65 2062 7920 6c69   read.line by li
-00005140: 6e65 2c20 6574 632e 2054 6869 7320 4150  ne, etc. This AP
-00005150: 4920 6973 2064 6573 6372 6962 6564 2062  I is described b
-00005160: 7920 7468 6520 6049 536f 7572 6365 4150  y the `ISourceAP
-00005170: 4960 2063 6c61 7373 2e20 4265 6361 7573  I` class. Becaus
-00005180: 6520 6469 6666 6572 656e 7420 7665 7273  e different vers
-00005190: 696f 6e73 206f 6620 7468 6520 7361 6d65  ions of the same
-000051a0: 2064 6174 6120 736f 7572 6365 0a6d 6179   data source.may
-000051b0: 2068 6176 6520 6469 6666 6572 656e 7420   have different 
-000051c0: 4150 492c 2069 7420 6973 2062 6574 7465  API, it is bette
-000051d0: 7220 746f 2063 7265 6174 6520 6120 636c  r to create a cl
-000051e0: 6173 7320 666f 7220 6561 6368 2076 6572  ass for each ver
-000051f0: 7369 6f6e 2e0a 0a47 656e 6572 616c 6c79  sion...Generally
-00005200: 2c20 6461 7461 2073 6f75 7263 6520 4150  , data source AP
-00005210: 4973 2061 7265 2068 6964 6465 6e20 6265  Is are hidden be
-00005220: 6869 6e64 2063 6f6e 7665 6e69 656e 7420  hind convenient 
-00005230: 696e 7465 7266 6163 6573 2e20 5468 6520  interfaces. The 
-00005240: 726f 6c65 206f 6620 7468 6573 6520 696e  role of these in
-00005250: 7465 7266 6163 6573 2069 7320 706c 6179  terfaces is play
-00005260: 6564 0a62 7920 6049 436f 6d6d 616e 6460  ed.by `ICommand`
-00005270: 2063 6c61 7373 6573 2e0a 0a60 4941 6461   classes...`IAda
-00005280: 7074 6572 6020 636c 6173 7365 7320 7472  pter` classes tr
-00005290: 616e 7366 6f72 6d20 6461 7461 2073 7472  ansform data str
-000052a0: 6561 6d20 6c69 6b65 2066 756e 6374 696f  eam like functio
-000052b0: 6e73 2066 6f72 2060 4461 7461 2e6d 6170  ns for `Data.map
-000052c0: 6020 6d65 7468 6f64 2e20 4573 7365 6e74  ` method. Essent
-000052d0: 6961 6c6c 7920 6974 2773 2074 6865 2073  ially it's the s
-000052e0: 616d 6520 7468 696e 6720 6275 7420 6d6f  ame thing but mo
-000052f0: 7265 0a66 6c65 7869 626c 652e 0a0a 466f  re.flexible...Fo
-00005300: 7220 6578 616d 706c 652c 204c 7744 5020  r example, LwDP 
-00005310: 4461 7461 536f 7572 6365 2868 7474 7073  DataSource(https
-00005320: 3a2f 2f67 6974 6875 622e 636f 6d2f 7468  ://github.com/th
-00005330: 322d 6e65 742f 7468 322d 6473 2d73 6f75  2-net/th2-ds-sou
-00005340: 7263 652d 6c77 6470 2920 7573 6573 2074  rce-lwdp) uses t
-00005350: 6865 7365 2061 6273 7472 6163 7420 636c  hese abstract cl
-00005360: 6173 7365 7320 746f 2062 7569 6c64 2069  asses to build i
-00005370: 7473 2069 6d70 6c65 6d65 6e74 6174 696f  ts implementatio
-00005380: 6e2e 596f 7520 6361 6e20 6561 7369 6c79  n.You can easily
-00005390: 2063 7265 6174 6520 796f 7572 206f 776e   create your own
-000053a0: 2075 6e69 7175 6520 636f 6d6d 616e 6473   unique commands
-000053b0: 2066 6f72 205f 4c77 4450 2044 6174 6153   for _LwDP DataS
-000053c0: 6f75 7263 655f 2c20 6173 2077 656c 6c20  ource_, as well 
-000053d0: 6173 2065 6e74 6972 650a 5f44 6174 6153  as entire._DataS
-000053e0: 6f75 7263 655f 2063 6c61 7373 6573 2e20  ource_ classes. 
-000053f0: 5b48 6572 6520 6973 2061 2064 6f63 756d  [Here is a docum
-00005400: 656e 7461 7469 6f6e 5d28 646f 6375 6d65  entation](docume
-00005410: 6e74 6174 696f 6e2f 6461 7461 736f 7572  ntation/datasour
-00005420: 6365 2e6d 6429 206f 6e20 686f 7720 746f  ce.md) on how to
-00005430: 2069 6d70 6c65 6d65 6e74 2074 6865 7365   implement these
-00005440: 2069 6e74 6572 6661 6365 732e 0a0a 215b   interfaces...![
-00005450: 4461 7461 2073 7472 6561 6d20 7069 7065  Data stream pipe
-00005460: 6c69 6e65 5d28 646f 6375 6d65 6e74 6174  line](documentat
-00005470: 696f 6e2f 696d 672f 636f 6e63 6570 742e  ion/img/concept.
-00005480: 706e 6729 0a0a 2323 2320 5374 7265 616d  png)..### Stream
-00005490: 206f 7065 7261 7469 6f6e 730a 0a46 7572   operations..Fur
-000054a0: 7468 6572 6d6f 7265 2c20 7374 7265 616d  thermore, stream
-000054b0: 206f 7065 7261 7469 6f6e 7320 6861 7665   operations have
-000054c0: 2074 776f 2066 756e 6461 6d65 6e74 616c   two fundamental
-000054d0: 2063 6861 7261 6374 6572 6973 7469 6373   characteristics
-000054e0: 2074 6861 7420 6d61 6b65 2074 6865 6d20   that make them 
-000054f0: 7665 7279 2064 6966 6665 7265 6e74 2066  very different f
-00005500: 726f 6d20 636f 6c6c 6563 7469 6f6e 0a6f  rom collection.o
-00005510: 7065 7261 7469 6f6e 733a 205f 5069 7065  perations: _Pipe
-00005520: 6c69 6e69 6e67 5f20 616e 6420 5f49 6e74  lining_ and _Int
-00005530: 6572 6e61 6c20 6974 6572 6174 696f 6e5f  ernal iteration_
-00005540: 2e0a 0a23 2323 2320 5069 7065 6c69 6e69  ...#### Pipelini
-00005550: 6e67 0a0a 4d61 6e79 2073 7472 6561 6d20  ng..Many stream 
-00005560: 6f70 6572 6174 696f 6e73 2072 6574 7572  operations retur
-00005570: 6e20 6120 7374 7265 616d 2074 6865 6d73  n a stream thems
-00005580: 656c 7665 732e 2054 6869 7320 616c 6c6f  elves. This allo
-00005590: 7773 206f 7065 7261 7469 6f6e 7320 746f  ws operations to
-000055a0: 2062 6520 6368 6169 6e65 6420 746f 2066   be chained to f
-000055b0: 6f72 6d20 6120 6c61 7267 6572 2070 6970  orm a larger pip
-000055c0: 656c 696e 652e 0a0a 215b 4461 7461 2073  eline...![Data s
-000055d0: 7472 6561 6d20 7069 7065 6c69 6e65 5d28  tream pipeline](
-000055e0: 646f 6375 6d65 6e74 6174 696f 6e2f 696d  documentation/im
-000055f0: 672f 6461 7461 5f73 7472 6561 6d5f 7069  g/data_stream_pi
-00005600: 7065 6c69 6e65 2e70 6e67 290a 0a23 2323  peline.png)..###
-00005610: 2320 496e 7465 726e 616c 2069 7465 7261  # Internal itera
-00005620: 7469 6f6e 0a0a 496e 2063 6f6e 7472 6173  tion..In contras
-00005630: 7420 746f 2063 6f6c 6c65 6374 696f 6e73  t to collections
-00005640: 2c20 7768 6963 6820 6172 6520 6974 6572  , which are iter
-00005650: 6174 6564 2065 7870 6c69 6369 746c 7920  ated explicitly 
-00005660: 2865 7874 6572 6e61 6c20 6974 6572 6174  (external iterat
-00005670: 696f 6e29 2c20 7374 7265 616d 206f 7065  ion), stream ope
-00005680: 7261 7469 6f6e 7320 646f 2074 6865 2069  rations do the i
-00005690: 7465 7261 7469 6f6e 0a62 6568 696e 6420  teration.behind 
-000056a0: 7468 6520 7363 656e 6573 2066 6f72 2079  the scenes for y
-000056b0: 6f75 2e20 4e6f 7465 2c20 6974 2064 6f65  ou. Note, it doe
-000056c0: 736e 2774 206d 6561 6e20 796f 7520 6361  sn't mean you ca
-000056d0: 6e6e 6f74 2069 7465 7261 7465 2074 6865  nnot iterate the
-000056e0: 205f 4461 7461 206f 626a 6563 745f 2e0a   _Data object_..
-000056f0: 0a0a 2323 2320 4461 7461 2069 7465 7261  ..### Data itera
-00005700: 7469 6f6e 0a0a 5468 6520 4461 7461 206f  tion..The Data o
-00005710: 626a 6563 7420 636f 6e73 7472 7563 746f  bject constructo
-00005720: 7220 6d65 7468 6f64 2074 616b 6573 2069  r method takes i
-00005730: 6e20 6173 2061 7267 756d 656e 7420 6569  n as argument ei
-00005740: 7468 6572 2061 6e20 6974 6572 6174 6f72  ther an iterator
-00005750: 206f 7665 7220 6f62 6a65 6374 7320 6f72   over objects or
-00005760: 2061 2067 656e 6572 6174 6f72 2066 756e   a generator fun
-00005770: 6374 696f 6e2e 0a54 6865 2044 6174 6120  ction..The Data 
-00005780: 6f62 6a65 6374 2069 7465 7261 746f 7220  object iterator 
-00005790: 6861 6e64 6c65 7320 6561 6368 2069 7465  handles each ite
-000057a0: 6d20 696e 2074 6869 7320 6974 6572 6174  m in this iterat
-000057b0: 6f72 206f 7220 6765 6e65 7261 746f 7220  or or generator 
-000057c0: 6173 2074 6865 7920 6172 652c 206d 6561  as they are, mea
-000057d0: 6e69 6e67 2069 7420 646f 6573 6e27 7420  ning it doesn't 
-000057e0: 7472 7920 746f 2072 6561 6420 7468 6520  try to read the 
-000057f0: 636f 6e74 656e 7420 6f66 2069 7465 6d20  content of item 
-00005800: 6f72 2072 6574 7572 6e20 7468 656d 206d  or return them m
-00005810: 6f64 6966 6965 6420 696e 2061 6e79 2077  odified in any w
-00005820: 6179 2c20 696e 7374 6561 6420 7265 7475  ay, instead retu
-00005830: 726e 7320 7468 6520 6974 656d 2069 7473  rns the item its
-00005840: 656c 662e 0a54 6865 206f 6e6c 7920 6578  elf..The only ex
-00005850: 6365 7074 696f 6e20 746f 2074 6869 7320  ception to this 
-00005860: 6973 2077 6865 6e20 4461 7461 206f 626a  is when Data obj
-00005870: 6563 7420 6973 2062 7569 6c74 2075 7369  ect is built usi
-00005880: 6e67 2069 7465 7261 746f 7220 6f72 2067  ng iterator or g
-00005890: 656e 6572 6174 6f72 206f 7665 7220 6f74  enerator over ot
-000058a0: 6865 7220 4461 7461 206f 626a 6563 7473  her Data objects
-000058b0: 2e20 4e6f 7465 2074 6861 7420 7468 6973  . Note that this
-000058c0: 2069 7465 7261 746f 7220 6f72 2067 656e   iterator or gen
-000058d0: 6572 6174 6f72 206d 7573 7420 6f6e 6c79  erator must only
-000058e0: 2062 6520 7969 656c 6469 6e67 2044 6174   be yielding Dat
-000058f0: 6120 6f62 6a65 6374 7320 616e 6420 6e6f  a objects and no
-00005900: 7468 696e 6720 656c 7365 2e20 4966 2077  thing else. If w
-00005910: 6520 6275 696c 6420 6672 6f6d 2061 206d  e build from a m
-00005920: 6978 206f 6620 4461 7461 206f 626a 6563  ix of Data objec
-00005930: 7473 2061 6e64 2073 6f6d 6520 6f74 6865  ts and some othe
-00005940: 7220 7479 7065 732c 2044 6174 6120 6f62  r types, Data ob
-00005950: 6a65 6374 7327 2063 6f6e 7465 6e74 2077  jects' content w
-00005960: 6f6e 2774 2062 6520 7265 6164 2061 6e64  on't be read and
-00005970: 2069 6e73 7465 6164 2069 7420 7769 6c6c   instead it will
-00005980: 2062 6520 7265 7475 726e 6564 2061 7320   be returned as 
-00005990: 4461 7461 206f 626a 6563 7420 6974 7365  Data object itse
-000059a0: 6c66 2e0a 0a53 6d61 6c6c 2065 7861 6d70  lf...Small examp
-000059b0: 6c65 2074 6f20 6465 6d6f 6e73 7472 6174  le to demonstrat
-000059c0: 653a 0a0a 6060 6070 7974 686f 6e0a 6672  e:..```python.fr
-000059d0: 6f6d 2074 6832 5f64 6174 615f 7365 7276  om th2_data_serv
-000059e0: 6963 6573 2e64 6174 6120 696d 706f 7274  ices.data import
-000059f0: 2044 6174 610a 0a64 3120 3d20 4461 7461   Data..d1 = Data
-00005a00: 285b 312c 322c 335d 290a 6432 203d 2044  ([1,2,3]).d2 = D
-00005a10: 6174 6128 5b34 2c35 2c36 5d29 0a0a 6f6e  ata([4,5,6])..on
-00005a20: 6c79 5f64 6174 615f 6f62 6a65 6374 7320  ly_data_objects 
-00005a30: 3d20 4461 7461 285b 6431 2c64 325d 2920  = Data([d1,d2]) 
-00005a40: 2320 5769 6c6c 2069 7465 7261 7465 2061  # Will iterate a
-00005a50: 7320 312c 322c 332c 342c 352c 360a 6461  s 1,2,3,4,5,6.da
-00005a60: 7461 5f61 6e64 5f6c 6973 7420 3d20 4461  ta_and_list = Da
-00005a70: 7461 285b 6431 2c5b 342c 352c 365d 5d29  ta([d1,[4,5,6]])
-00005a80: 2023 2057 696c 6c20 6974 6572 6174 6520   # Will iterate 
-00005a90: 6173 2064 312c 205b 342c 352c 365d 0a64  as d1, [4,5,6].d
-00005aa0: 6174 615f 616e 645f 6e75 6d62 6572 7320  ata_and_numbers 
-00005ab0: 3d20 4461 7461 285b 6431 2c34 2c35 2c36  = Data([d1,4,5,6
-00005ac0: 5d29 2023 2057 696c 6c20 6974 6572 6174  ]) # Will iterat
-00005ad0: 6520 6173 2064 312c 342c 352c 360a 6c69  e as d1,4,5,6.li
-00005ae0: 7374 735f 6f6e 6c79 203d 2044 6174 6128  sts_only = Data(
-00005af0: 5b31 2c32 2c33 5d2c 5b34 2c35 2c36 5d29  [1,2,3],[4,5,6])
-00005b00: 2023 2057 696c 6c20 6974 6572 6174 6520   # Will iterate 
-00005b10: 6173 205b 312c 322c 335d 2c5b 342c 352c  as [1,2,3],[4,5,
-00005b20: 365d 0a0a 2320 4966 2077 6520 7761 6e74  6]..# If we want
-00005b30: 2074 6f20 6974 6572 6174 6520 6f76 6572   to iterate over
-00005b40: 2063 6f6e 7465 6e74 206f 6620 6c69 7374   content of list
-00005b50: 206f 6620 6c69 7374 732c 2077 6520 7368   of lists, we sh
-00005b60: 6f75 6c64 2066 6972 7374 2063 7265 6174  ould first creat
-00005b70: 6520 4461 7461 206f 626a 6563 7473 2066  e Data objects f
-00005b80: 726f 6d20 7468 656d 2c0a 2320 7468 656e  rom them,.# then
-00005b90: 2075 7365 2074 6865 6d20 746f 2063 6f6e   use them to con
-00005ba0: 7374 7275 6374 206e 6577 2044 6174 6120  struct new Data 
-00005bb0: 6f62 6a65 6374 2061 7320 696e 2063 6173  object as in cas
-00005bc0: 6520 6f66 2064 3120 616e 6420 6432 2c20  e of d1 and d2, 
-00005bd0: 6372 6561 7469 6e67 2027 6f6e 6c79 5f64  creating 'only_d
-00005be0: 6174 615f 6f62 6a65 6374 7327 2069 6e20  ata_objects' in 
-00005bf0: 7468 6973 2065 7861 6d70 6c65 2e0a 6060  this example..``
-00005c00: 600a 200a 0a23 2323 2044 6174 6120 6361  `. ..### Data ca
-00005c10: 6368 696e 670a 0a54 6865 205f 4461 7461  ching..The _Data
-00005c20: 206f 626a 6563 745f 2070 726f 7669 6465   object_ provide
-00005c30: 7320 7468 6520 6162 696c 6974 7920 746f  s the ability to
-00005c40: 2075 7365 2074 6865 2063 6163 6865 2e20   use the cache. 
-00005c50: 5468 6520 6361 6368 6520 776f 726b 7320  The cache works 
-00005c60: 666f 7220 6561 6368 205f 4461 7461 206f  for each _Data o
-00005c70: 626a 6563 745f 2c20 7468 6174 2069 732c  bject_, that is,
-00005c80: 2079 6f75 2063 686f 6f73 650a 7768 6963   you choose.whic
-00005c90: 6820 5f44 6174 6120 6f62 6a65 6374 5f20  h _Data object_ 
-00005ca0: 796f 7520 7761 6e74 2074 6f20 7361 7665  you want to save
-00005cb0: 2e20 5468 6520 5f44 6174 6120 6f62 6a65  . The _Data obje
-00005cc0: 6374 5f20 6361 6368 6520 6973 2073 6176  ct_ cache is sav
-00005cd0: 6564 2061 6674 6572 2074 6865 2066 6972  ed after the fir
-00005ce0: 7374 2069 7465 7261 7469 6f6e 2c20 6275  st iteration, bu
-00005cf0: 7420 7468 6520 6974 6572 6174 696f 6e0a  t the iteration.
-00005d00: 736f 7572 6365 206d 6179 2062 6520 6469  source may be di
-00005d10: 6666 6572 656e 742e 0a0a 4966 2079 6f75  fferent...If you
-00005d20: 2064 6f6e 2774 2075 7365 2074 6865 2063   don't use the c
-00005d30: 6163 6865 2c20 796f 7572 2073 6f75 7263  ache, your sourc
-00005d40: 6520 7769 6c6c 2062 6520 7468 6520 6461  e will be the da
-00005d50: 7461 2073 6f75 7263 6520 796f 7520 6861  ta source you ha
-00005d60: 7665 2069 6e20 7468 6520 5f44 6174 6120  ve in the _Data 
-00005d70: 4f62 6a65 6374 5f2e 2042 7574 2069 6620  Object_. But if 
-00005d80: 796f 7520 7573 6520 7468 6520 6361 6368  you use the cach
-00005d90: 652c 0a79 6f75 7220 736f 7572 6365 2063  e,.your source c
-00005da0: 616e 2062 6520 7468 6520 6461 7461 2073  an be the data s
-00005db0: 6f75 7263 652c 2074 6865 2070 6172 656e  ource, the paren
-00005dc0: 7420 6361 6368 652c 206f 7220 6f77 6e20  t cache, or own 
-00005dd0: 6361 6368 653a 0a0a 2a20 5468 6520 6461  cache:..* The da
-00005de0: 7461 2073 6f75 7263 653a 0a20 2049 6620  ta source:.  If 
-00005df0: 7468 6520 5f44 6174 6120 4f62 6a65 6374  the _Data Object
-00005e00: 5f20 646f 6573 6e27 7420 6861 7665 2061  _ doesn't have a
-00005e10: 2070 6172 656e 7420 6361 6368 6520 616e   parent cache an
-00005e20: 6420 6974 7320 6361 6368 652e 0a2a 2054  d its cache..* T
-00005e30: 6865 2070 6172 656e 7420 6361 6368 653a  he parent cache:
-00005e40: 0a20 2049 6620 7468 6520 5f44 6174 6120  .  If the _Data 
-00005e50: 4f62 6a65 6374 5f20 6861 7320 6120 7061  Object_ has a pa
-00005e60: 7265 6e74 2063 6163 6865 2e20 4974 2064  rent cache. It d
-00005e70: 6f65 736e 2774 206d 6174 7465 7220 7768  oesn't matter wh
-00005e80: 6174 2070 6f73 6974 696f 6e20 7468 6520  at position the 
-00005e90: 7061 7265 6e74 2063 6163 6865 2068 6173  parent cache has
-00005ea0: 2069 6e20 696e 6865 7269 7461 6e63 652e   in inheritance.
-00005eb0: 0a20 205f 4461 7461 204f 626a 6563 745f  .  _Data Object_
-00005ec0: 2075 6e64 6572 7374 616e 6473 2077 686f   understands who
-00005ed0: 7365 2063 6163 6865 2069 7420 6973 2061  se cache it is a
-00005ee0: 6e64 2065 7865 6375 7465 7320 7468 6520  nd executes the 
-00005ef0: 7061 7274 206f 6620 7468 6520 776f 726b  part of the work
-00005f00: 666c 6f77 2074 6861 7420 7761 7320 6e6f  flow that was no
-00005f10: 7420 6578 6563 7574 6564 2e0a 2a20 5468  t executed..* Th
-00005f20: 6520 6f77 6e20 6361 6368 653a 0a20 2049  e own cache:.  I
-00005f30: 6620 6974 2069 7320 6e6f 7420 7468 6520  f it is not the 
-00005f40: 6669 7273 7420 6974 6572 6174 696f 6e20  first iteration 
-00005f50: 6f66 2074 6869 7320 4461 7461 206f 626a  of this Data obj
-00005f60: 6563 742e 0a0a 4e6f 7465 2074 6861 7420  ect...Note that 
-00005f70: 7468 6520 6361 6368 6520 7374 6174 6520  the cache state 
-00005f80: 6f66 2074 6865 2044 6174 6120 6f62 6a65  of the Data obje
-00005f90: 6374 2069 7320 6e6f 7420 696e 6865 7269  ct is not inheri
-00005fa0: 7465 642e 0a0a 2323 2323 2046 6f72 6365  ted...#### Force
-00005fb0: 6420 6361 6368 696e 670a 596f 7520 6361  d caching.You ca
-00005fc0: 6e20 7465 6c6c 2044 5320 746f 2063 6163  n tell DS to cac
-00005fd0: 6865 2064 6174 6120 746f 2073 7065 6369  he data to speci
-00005fe0: 6669 6320 6361 6368 6520 6669 6c65 2c20  fic cache file, 
-00005ff0: 7768 6963 6820 776f 6e27 7420 6265 2064  which won't be d
-00006000: 656c 6574 6564 2061 6674 6572 2073 6372  eleted after scr
-00006010: 6970 7420 656e 642e 0a59 6f75 2063 616e  ipt end..You can
-00006020: 2073 6565 2065 7861 6d70 6c65 2069 6e20   see example in 
-00006030: 312e 3132 2073 6563 7469 6f6e 206f 6620  1.12 section of 
-00006040: 5b67 6574 5f73 7461 7274 6564 5f65 7861  [get_started_exa
-00006050: 6d70 6c65 5d28 6578 616d 706c 6573 2f67  mple](examples/g
-00006060: 6574 5f73 7461 7274 6564 5f65 7861 6d70  et_started_examp
-00006070: 6c65 2e70 7929 2e0a 0a0a 2323 2320 4576  le.py)....### Ev
-00006080: 656e 7454 7265 6520 616e 6420 636f 6c6c  entTree and coll
-00006090: 6563 7469 6f6e 730a 0a23 2323 2320 4576  ections..#### Ev
-000060a0: 656e 7454 7265 650a 0a60 4576 656e 7454  entTree..`EventT
-000060b0: 7265 6560 2069 7320 6120 7472 6565 2d62  ree` is a tree-b
-000060c0: 6173 6564 2064 6174 6120 7374 7275 6374  ased data struct
-000060d0: 7572 6520 6f66 2065 7665 6e74 732e 2049  ure of events. I
-000060e0: 7420 616c 6c6f 7773 2079 6f75 2067 6574  t allows you get
-000060f0: 2063 6869 6c64 7265 6e20 616e 6420 7061   children and pa
-00006100: 7265 6e74 7320 6f66 2065 7665 6e74 2c0a  rents of event,.
-00006110: 6469 7370 6c61 7920 7472 6565 2c20 6765  display tree, ge
-00006120: 7420 6675 6c6c 2070 6174 6820 746f 2065  t full path to e
-00006130: 7665 6e74 2065 7463 2e0a 0a44 6574 6169  vent etc...Detai
-00006140: 6c73 3a0a 0a2a 2060 4576 656e 7454 7265  ls:..* `EventTre
-00006150: 6560 2063 6f6e 7461 696e 7320 616c 6c20  e` contains all 
-00006160: 6576 656e 7473 2069 6e20 6d65 6d6f 7279  events in memory
-00006170: 2e0a 2a20 5472 6565 2068 6173 2073 6f6d  ..* Tree has som
-00006180: 6520 696d 706f 7274 616e 7420 7465 726d  e important term
-00006190: 733a 0a20 2020 2031 2e20 5f41 6e63 6573  s:.    1. _Ances
-000061a0: 746f 725f 2069 7320 616e 7920 7265 6c61  tor_ is any rela
-000061b0: 7469 7665 206f 6620 7468 6520 6576 656e  tive of the even
-000061c0: 7420 7570 2074 6865 2074 7265 6520 2867  t up the tree (g
-000061d0: 7261 6e64 7061 7265 6e74 2c20 7061 7265  randparent, pare
-000061e0: 6e74 2065 7463 2e29 2e0a 2020 2020 322e  nt etc.)..    2.
-000061f0: 205f 5061 7265 6e74 5f20 6973 206f 6e6c   _Parent_ is onl
-00006200: 7920 7468 6520 6669 7273 7420 7265 6c61  y the first rela
-00006210: 7469 7665 206f 6620 7468 6520 6576 656e  tive of the even
-00006220: 7420 7570 2074 6865 2074 7265 652e 0a20  t up the tree.. 
-00006230: 2020 2033 2e20 5f43 6869 6c64 5f20 6973     3. _Child_ is
-00006240: 2074 6865 2066 6972 7374 2072 656c 6174   the first relat
-00006250: 6976 6520 6f66 2074 6865 2065 7665 6e74  ive of the event
-00006260: 2064 6f77 6e20 7468 6520 7472 6565 2e0a   down the tree..
-00006270: 0a54 616b 6520 6120 6c6f 6f6b 2061 7420  .Take a look at 
-00006280: 7468 6520 666f 6c6c 6f77 696e 6720 4854  the following HT
-00006290: 4d4c 2074 7265 6520 746f 2075 6e64 6572  ML tree to under
-000062a0: 7374 616e 6420 7468 656d 2e0a 0a20 2020  stand them...   
-000062b0: 6060 600a 2020 2020 3c62 6f64 793e 203c  ```.    <body> <
-000062c0: 212d 2d20 616e 6365 7374 6f72 2028 6772  !-- ancestor (gr
-000062d0: 616e 6470 6172 656e 7429 2c20 6275 7420  andparent), but 
-000062e0: 6e6f 7420 7061 7265 6e74 202d 2d3e 0a20  not parent -->. 
-000062f0: 2020 2020 2020 203c 6469 763e 203c 212d         <div> <!-
-00006300: 2d20 7061 7265 6e74 2026 2061 6e63 6573  - parent & ances
-00006310: 746f 7220 2d2d 3e0a 2020 2020 2020 2020  tor -->.        
-00006320: 2020 2020 3c70 3e48 656c 6c6f 2c20 776f      <p>Hello, wo
-00006330: 726c 6421 3c2f 703e 203c 212d 2d20 6368  rld!</p> <!-- ch
-00006340: 696c 6420 2d2d 3e0a 2020 2020 2020 2020  ild -->.        
-00006350: 2020 2020 3c70 3e47 6f6f 6462 7965 213c      <p>Goodbye!<
-00006360: 2f70 3e20 3c21 2d2d 2073 6962 6c69 6e67  /p> <!-- sibling
-00006370: 202d 2d3e 0a20 2020 2020 2020 203c 2f64   -->.        </d
-00006380: 6976 3e0a 2020 2020 3c2f 626f 6479 3e0a  iv>.    </body>.
-00006390: 2020 2060 6060 0a0a 2323 2323 2043 6f6c     ```..#### Col
-000063a0: 6c65 6374 696f 6e73 0a0a 2a2a 4576 656e  lections..**Even
-000063b0: 7454 7265 6543 6f6c 6c65 6374 696f 6e2a  tTreeCollection*
-000063c0: 2a20 6973 2061 2063 6f6c 6c65 6374 696f  * is a collectio
-000063d0: 6e20 6f66 2045 7665 6e74 5472 6565 732e  n of EventTrees.
-000063e0: 2054 6865 2063 6f6c 6c65 6374 696f 6e20   The collection 
-000063f0: 6275 696c 6473 2061 2066 6577 205f 4576  builds a few _Ev
-00006400: 656e 7454 7265 655f 2062 7920 7061 7373  entTree_ by pass
-00006410: 6564 205f 4461 7461 0a6f 626a 6563 745f  ed _Data.object_
-00006420: 2e20 416c 7468 6f75 6768 2079 6f75 2063  . Although you c
-00006430: 616e 2063 6861 6e67 6520 7468 6520 7472  an change the tr
-00006440: 6565 2064 6972 6563 746c 792c 2069 7427  ee directly, it'
-00006450: 7320 6265 7474 6572 2074 6f20 646f 2069  s better to do i
-00006460: 7420 7468 726f 7567 6820 636f 6c6c 6563  t through collec
-00006470: 7469 6f6e 7320 6265 6361 7573 6520 7468  tions because th
-00006480: 6579 2061 7265 2061 7761 7265 206f 660a  ey are aware of.
-00006490: 6064 6574 6163 6865 645f 6576 656e 7473  `detached_events
-000064a0: 6020 616e 6420 6361 6e20 736f 6c76 6520  ` and can solve 
-000064b0: 736f 6d65 2065 7665 6e74 7320 6465 7065  some events depe
-000064c0: 6e64 656e 6369 6573 2e20 5468 6520 636f  ndencies. The co
-000064d0: 6c6c 6563 7469 6f6e 2068 6173 2073 696d  llection has sim
-000064e0: 696c 6172 2066 6561 7475 7265 7320 6c69  ilar features li
-000064f0: 6b65 2061 2073 696e 676c 6520 5f45 7665  ke a single _Eve
-00006500: 6e74 5472 6565 5f0a 6275 7420 6170 706c  ntTree_.but appl
-00006510: 7969 6e67 2074 6865 6d20 666f 7220 616c  ying them for al
-00006520: 6c20 5f45 7665 6e74 5472 6565 735f 2e0a  l _EventTrees_..
-00006530: 0a2a 2a50 6172 656e 7445 7665 6e74 5472  .**ParentEventTr
-00006540: 6565 436f 6c6c 6563 7469 6f6e 2a2a 2069  eeCollection** i
-00006550: 7320 6120 636f 6c6c 6563 7469 6f6e 2073  s a collection s
-00006560: 696d 696c 6172 2074 6f20 5f45 7665 6e74  imilar to _Event
-00006570: 5472 6565 436f 6c6c 6563 7469 6f6e 5f20  TreeCollection_ 
-00006580: 6275 7420 636f 6e74 6169 6e69 6e67 206f  but containing o
-00006590: 6e6c 7920 7061 7265 6e74 2065 7665 6e74  nly parent event
-000065a0: 7320 7468 6174 0a61 7265 2072 6566 6572  s that.are refer
-000065b0: 656e 6365 6420 696e 2074 6865 2064 6174  enced in the dat
-000065c0: 6120 7374 7265 616d 2e20 5468 6520 636f  a stream. The co
-000065d0: 6c6c 6563 7469 6f6e 2068 6173 2066 6561  llection has fea
-000065e0: 7475 7265 7320 7369 6d69 6c61 7220 746f  tures similar to
-000065f0: 205f 4576 656e 7454 7265 6543 6f6c 6c65   _EventTreeColle
-00006600: 6374 696f 6e5f 2e0a 0a44 6574 6169 6c73  ction_...Details
-00006610: 3a0a 0a2a 2054 6f20 7573 6520 4554 2063  :..* To use ET c
-00006620: 6f6c 6c65 6374 696f 6e73 2079 6f75 206e  ollections you n
-00006630: 6565 6420 746f 2069 6e69 7469 616c 697a  eed to initializ
-00006640: 6520 7468 656d 2062 7920 5f45 5443 4472  e them by _ETCDr
-00006650: 6976 6572 5f2e 2044 6174 6120 736f 7572  iver_. Data sour
-00006660: 6365 7320 7573 7561 6c6c 7920 7072 6f76  ces usually prov
-00006670: 6964 6520 7468 656d 2e0a 2020 596f 7520  ide them..  You 
-00006680: 6361 6e20 6372 6561 7465 2069 7420 6279  can create it by
-00006690: 2079 6f75 7273 656c 6620 6465 7065 6e64   yourself depend
-000066a0: 696e 6720 6f6e 2079 6f75 7220 6461 7461  ing on your data
-000066b0: 2073 7472 7563 7475 7265 2e0a 2a20 5468   structure..* Th
-000066c0: 6520 636f 6c6c 6563 7469 6f6e 2068 6173  e collection has
-000066d0: 2061 2066 6561 7475 7265 2074 6f20 7265   a feature to re
-000066e0: 636f 7665 7220 6576 656e 7473 2e20 416c  cover events. Al
-000066f0: 6c20 6576 656e 7473 2074 6861 7420 6172  l events that ar
-00006700: 6520 6e6f 7420 696e 2074 6865 2072 6563  e not in the rec
-00006710: 6569 7665 6420 6461 7461 2073 7472 6561  eived data strea
-00006720: 6d2c 2062 7574 2077 6869 6368 2061 7265  m, but which are
-00006730: 0a20 2072 6566 6572 656e 6365 6420 7769  .  referenced wi
-00006740: 6c6c 2062 6520 6c6f 6164 6564 2066 726f  ll be loaded fro
-00006750: 6d20 7468 6520 6461 7461 2073 6f75 7263  m the data sourc
-00006760: 652e 0a2a 2059 6f75 2063 616e 2074 616b  e..* You can tak
-00006770: 6520 6064 6574 6163 6865 645f 6576 656e  e `detached_even
-00006780: 7473 6020 746f 2073 6565 2077 6869 6368  ts` to see which
-00006790: 2065 7665 6e74 7320 6172 6520 6d69 7373   events are miss
-000067a0: 696e 672e 0a2a 2049 6620 796f 7520 7761  ing..* If you wa
-000067b0: 6e74 2c20 796f 7520 6361 6e20 6275 696c  nt, you can buil
-000067c0: 6420 7061 7265 6e74 6c65 7373 2074 7265  d parentless tre
-000067d0: 6573 2077 6865 7265 2074 6865 206d 6973  es where the mis
-000067e0: 7369 6e67 2065 7665 6e74 7320 6172 6520  sing events are 
-000067f0: 7374 7562 6265 6420 696e 7374 6561 642e  stubbed instead.
-00006800: 204a 7573 740a 2020 7573 6520 6067 6574   Just.  use `get
-00006810: 5f70 6172 656e 746c 6573 735f 7472 6565  _parentless_tree
-00006820: 7328 2960 2e0a 0a52 6571 7569 7265 6d65  s()`...Requireme
-00006830: 6e74 733a 0a0a 312e 2045 7665 6e74 7320  nts:..1. Events 
-00006840: 7072 6f76 6964 6564 2074 6f20 4554 4320  provided to ETC 
-00006850: 6861 7665 2074 6f20 6861 7665 2060 6576  have to have `ev
-00006860: 656e 745f 6e61 6d65 602c 2060 6576 656e  ent_name`, `even
-00006870: 745f 6964 602c 2060 7061 7265 6e74 5f65  t_id`, `parent_e
-00006880: 7665 6e74 5f69 6460 2066 6965 6c64 732e  vent_id` fields.
-00006890: 2054 6865 790a 6361 6e20 6861 7665 2061   They.can have a
-000068a0: 6e6f 7468 6572 206e 616d 6573 2028 6974  nother names (it
-000068b0: 2072 6573 6f6c 7665 7320 696e 2074 6865   resolves in the
-000068c0: 2064 7269 7665 7229 2e0a 0a23 2323 2320   driver)...#### 
-000068d0: 4869 6e74 730a 0a2a 2052 656d 6f76 6520  Hints..* Remove 
-000068e0: 616c 6c20 756e 6e65 6365 7373 6172 7920  all unnecessary 
-000068f0: 6669 656c 6473 2066 726f 6d20 6576 656e  fields from even
-00006900: 7473 2062 6566 6f72 6520 7061 7373 696e  ts before passin
-00006910: 6720 746f 2061 205f 636f 6c6c 6563 7469  g to a _collecti
-00006920: 6f6e 5f20 746f 2072 6564 7563 6520 6d65  on_ to reduce me
-00006930: 6d6f 7279 2075 7361 6765 2e0a 2a20 5573  mory usage..* Us
-00006940: 6520 6073 686f 7728 2960 206d 6574 686f  e `show()` metho
-00006950: 6420 746f 2070 7269 6e74 2074 6865 2074  d to print the t
-00006960: 7265 6520 696e 2074 7265 652d 6c69 6b65  ree in tree-like
-00006970: 2076 6965 772e 0a2a 204e 6f74 6520 7468   view..* Note th
-00006980: 6174 2074 6865 2060 6765 745f 7860 206d  at the `get_x` m
-00006990: 6574 686f 6473 2077 696c 6c20 7261 6973  ethods will rais
-000069a0: 6520 616e 2065 7863 6570 7469 6f6e 2069  e an exception i
-000069b0: 6620 796f 7520 7061 7373 2061 6e20 756e  f you pass an un
-000069c0: 6b6e 6f77 6e20 6576 656e 7420 6964 2c20  known event id, 
-000069d0: 756e 6c69 6b65 2074 6865 2060 6669 6e64  unlike the `find
-000069e0: 5f78 6020 6d65 7468 6f64 7320 280a 2020  _x` methods (.  
-000069f0: 7468 6579 2072 6574 7572 6e20 4e6f 6e65  they return None
-00006a00: 292e 0a2a 2049 6620 796f 7520 7761 6e74  )..* If you want
-00006a10: 2074 6f20 6b6e 6f77 2074 6861 7420 7370   to know that sp
-00006a20: 6563 6966 6965 6420 6576 656e 7420 6578  ecified event ex
-00006a30: 6973 7473 2c20 7573 6520 7468 6520 7079  ists, use the py
-00006a40: 7468 6f6e 2060 696e 6020 6b65 7977 6f72  thon `in` keywor
-00006a50: 6420 2865 2e67 2e20 6027 6576 656e 742d  d (e.g. `'event-
-00006a60: 6964 2720 696e 2065 7665 6e74 735f 7472  id' in events_tr
-00006a70: 6565 6029 2e0a 2a20 5573 6520 7468 6520  ee`)..* Use the 
-00006a80: 7079 7468 6f6e 2060 6c65 6e60 206b 6579  python `len` key
-00006a90: 776f 7264 2074 6f20 6765 7420 6576 656e  word to get even
-00006aa0: 7473 206e 756d 6265 7220 696e 2074 6865  ts number in the
-00006ab0: 2074 7265 652e 0a0a 2323 2320 4669 656c   tree...### Fiel
-00006ac0: 6420 5265 736f 6c76 6572 730a 496e 7465  d Resolvers.Inte
-00006ad0: 7266 6163 6520 6361 6e20 6265 2066 6f75  rface can be fou
-00006ae0: 6e64 2069 6e20 6074 6832 5f64 6174 615f  nd in `th2_data_
-00006af0: 7365 7276 6963 6573 2f69 6e74 6572 6661  services/interfa
-00006b00: 6365 732f 7574 696c 732f 7265 736f 6c76  ces/utils/resolv
-00006b10: 6572 2e70 7960 2e20 200a 416c 6c20 6461  er.py`.  .All da
-00006b20: 7461 2d73 6f75 7263 6573 2073 686f 756c  ta-sources shoul
-00006b30: 6420 696d 706c 656d 656e 7420 7468 656d  d implement them
-00006b40: 2e0a 0a54 6865 2069 6465 6120 6f66 2075  ...The idea of u
-00006b50: 7369 6e67 2072 6573 6f6c 7665 7273 3a0a  sing resolvers:.
-00006b60: 4974 2073 6f6c 7665 7320 7468 6520 7072  It solves the pr
-00006b70: 6f62 6c65 6d20 6f66 2068 6176 696e 6720  oblem of having 
-00006b80: 6120 6665 7720 4461 7461 536f 7572 6365  a few DataSource
-00006b90: 7320 7769 7468 2073 696d 696c 6172 2064  s with similar d
-00006ba0: 6174 612c 0a62 7574 2077 6974 6820 6469  ata,.but with di
-00006bb0: 6666 6572 656e 7420 7761 7973 2074 6f20  fferent ways to 
-00006bc0: 6765 7420 6974 2e0a 0a54 6865 7365 2063  get it...These c
-00006bd0: 6c61 7373 6573 2070 726f 7669 6465 2079  lasses provide y
-00006be0: 6f75 2067 6574 7465 7220 6d65 7468 6f64  ou getter method
-00006bf0: 732e 0a55 7369 6e67 2074 6865 7365 2063  s..Using these c
-00006c00: 6c61 7373 6573 2061 6c6c 6f77 7320 796f  lasses allows yo
-00006c10: 7520 746f 2066 7265 656c 7920 7377 6974  u to freely swit
-00006c20: 6368 2062 6574 7765 656e 2064 6966 6665  ch between diffe
-00006c30: 7265 6e74 2064 6174 610a 666f 726d 6174  rent data.format
-00006c40: 7320 616e 6420 646f 6e27 7420 6368 616e  s and don't chan
-00006c50: 6765 2079 6f75 7220 636f 6465 2e0a 0a52  ge your code...R
-00006c60: 6573 6f6c 7665 7273 2073 6f6c 7665 2074  esolvers solve t
-00006c70: 6865 2070 726f 626c 656d 206f 6620 6461  he problem of da
-00006c80: 7461 2d66 6f72 6d61 7420 6d69 6772 6174  ta-format migrat
-00006c90: 696f 6e2e 0a2d 2066 6965 6c64 7320 706c  ion..- fields pl
-00006ca0: 6163 6520 6361 6e20 6265 2063 6861 6e67  ace can be chang
-00006cb0: 6564 0a2d 2066 6965 6c64 7320 6e61 6d65  ed.- fields name
-00006cc0: 7320 6361 6e20 6265 2063 6861 6e67 6564  s can be changed
-00006cd0: 0a0a 5265 736f 6c76 6572 7320 6361 6e20  ..Resolvers can 
-00006ce0: 776f 726b 206f 6e6c 7920 7769 7468 206f  work only with o
-00006cf0: 6e65 2065 7665 6e74 2f6d 6573 7361 6765  ne event/message
-00006d00: 2e0a 4974 206d 6561 6e73 2c20 6966 2079  ..It means, if y
-00006d10: 6f75 7220 6d65 7373 6167 6520 6861 7320  our message has 
-00006d20: 7375 622d 6d65 7373 6167 6573 2028 6c69  sub-messages (li
-00006d30: 6b65 2074 6832 2d6d 6573 7361 6765 7320  ke th2-messages 
-00006d40: 696e 206c 7764 7029 2069 7420 0a77 6f6e  in lwdp) it .won
-00006d50: 2774 2077 6f72 6b2c 2062 6563 6175 7365  't work, because
-00006d60: 2072 6573 6f6c 7665 7220 7769 6c6c 206e   resolver will n
-00006d70: 6f74 206b 6e6f 7720 7769 7468 2077 6869  ot know with whi
-00006d80: 6368 2073 7562 2d6d 6573 7361 6765 2073  ch sub-message s
-00006d90: 686f 756c 6420 6974 2077 6f72 6b2e 200a  hould it work. .
-00006da0: 0a2a 2a57 6f72 6b61 726f 756e 642a 2a20  .**Workaround** 
-00006db0: 200a 312e 2045 7870 616e 6420 616c 6c20   .1. Expand all 
-00006dc0: 796f 7572 206d 6573 7361 6765 7320 2d3e  your messages ->
-00006dd0: 2060 6e65 775f 6420 3d20 796f 7572 5f64   `new_d = your_d
-00006de0: 6174 612e 6d61 7028 4d65 7373 6167 6546  ata.map(MessageF
-00006df0: 6965 6c64 5265 736f 6c76 6572 2e65 7870  ieldResolver.exp
-00006e00: 616e 645f 6d65 7373 6167 6529 600a 322e  and_message)`.2.
-00006e10: 2055 7365 2060 4578 7061 6e64 6564 4d65   Use `ExpandedMe
-00006e20: 7373 6167 6546 6965 6c64 5265 736f 6c76  ssageFieldResolv
-00006e30: 6572 6020 696e 7374 6561 6420 6f66 2075  er` instead of u
-00006e40: 7375 616c 2060 4d65 7373 6167 6546 6965  sual `MessageFie
-00006e50: 6c64 5265 736f 6c76 6572 6020 7768 656e  ldResolver` when
-00006e60: 200a 2020 2020 796f 7520 7461 6b65 2066   .    you take f
-00006e70: 6965 6c64 7320 666f 7220 6578 7061 6e64  ields for expand
-00006e80: 6564 206d 6573 7361 6765 732e 0a0a 2a2a  ed messages...**
-00006e90: 496d 706c 656d 656e 7461 7469 6f6e 2061  Implementation a
-00006ea0: 6476 6963 653a 2a2a 0a31 2e20 7261 6973  dvice:**.1. rais
-00006eb0: 6520 4e6f 7449 6d70 6c65 6d65 6e74 6564  e NotImplemented
-00006ec0: 4572 726f 7220 2d2d 2069 6620 796f 7572  Error -- if your
-00006ed0: 2049 6d70 6c65 6d65 6e74 6174 696f 6e20   Implementation 
-00006ee0: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
-00006ef0: 7468 6973 2067 6574 7465 722e 0a0a 2a2a  this getter...**
-00006f00: 5065 7266 6f72 6d61 6e63 6520 696d 7061  Performance impa
-00006f10: 6374 3a2a 2a0a 2d20 4974 2061 2062 6974  ct:**.- It a bit
-00006f20: 2073 6c6f 7765 7220 7468 616e 2075 7369   slower than usi
-00006f30: 6e67 206e 616b 6564 2066 6965 6c64 2061  ng naked field a
-00006f40: 6363 6573 7320 6064 6963 745b 276b 6579  ccess `dict['key
-00006f50: 275d 602e 0a0a 2323 2032 2e34 2e20 4c69  ']`...## 2.4. Li
-00006f60: 6e6b 730a 0a2d 205b 5265 706f 7274 2044  nks..- [Report D
-00006f70: 6174 6120 5072 6f76 6964 6572 5d28 6874  ata Provider](ht
-00006f80: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00006f90: 2f74 6832 2d6e 6574 2f74 6832 2d72 7074  /th2-net/th2-rpt
-00006fa0: 2d64 6174 612d 7072 6f76 6964 6572 290a  -data-provider).
-00006fb0: 2d20 5b54 6832 2044 6174 6120 5365 7276  - [Th2 Data Serv
-00006fc0: 6963 6573 2055 7469 6c73 5d28 6874 7470  ices Utils](http
-00006fd0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
-00006fe0: 6832 2d6e 6574 2f74 6832 2d64 6174 612d  h2-net/th2-data-
-00006ff0: 7365 7276 6963 6573 2d75 7469 6c73 290a  services-utils).
-00007000: 0a23 2033 2e20 4265 7374 2070 7261 6374  .# 3. Best pract
-00007010: 6963 6573 0a44 6570 656e 6469 6e67 206f  ices.Depending o
-00007020: 6e20 686f 7720 796f 7520 776f 726b 2077  n how you work w
-00007030: 6974 6820 6044 6174 6120 6f62 6a65 6374  ith `Data object
-00007040: 602c 2069 7420 6361 6e20 6265 2073 6c6f  `, it can be slo
-00007050: 7720 6f66 2066 6173 742e 0a41 7320 7769  w of fast..As wi
-00007060: 7468 2061 2072 656c 6174 696f 6e61 6c20  th a relational 
-00007070: 6461 7461 6261 7365 2c20 796f 7520 6361  database, you ca
-00007080: 6e20 7772 6974 6520 6120 7175 6572 7920  n write a query 
-00007090: 7468 6174 2077 696c 6c20 7265 7475 726e  that will return
-000070a0: 2064 6174 6120 736c 6f77 6c79 206f 7220   data slowly or 
-000070b0: 7175 6963 6b6c 792c 0a74 6865 2073 616d  quickly,.the sam
-000070c0: 6520 7768 656e 2077 6f72 6b69 6e67 2077  e when working w
-000070d0: 6974 6820 6120 6044 6174 6120 6f62 6a65  ith a `Data obje
-000070e0: 6374 602e 0a0a 466f 6c6c 6f77 2074 6865  ct`...Follow the
-000070f0: 2072 756c 6573 2074 6f20 6d61 6b65 2079   rules to make y
-00007100: 6f75 7220 776f 726b 2077 6974 6820 4461  our work with Da
-00007110: 7461 206f 626a 6563 7420 6661 7374 3a0a  ta object fast:.
-00007120: 312e 2055 7365 2060 4461 7461 2e75 7365  1. Use `Data.use
-00007130: 5f63 6163 6865 2829 6020 6966 2079 6f75  _cache()` if you
-00007140: 2069 7465 7261 7465 2064 6174 6120 6d6f   iterate data mo
-00007150: 7265 2074 6861 6e20 6f6e 6520 7469 6d65  re than one time
-00007160: 2e0a 322e 2054 7279 2074 6f20 646f 6e27  ..2. Try to don'
-00007170: 7420 6974 6572 6174 6520 6f6e 6520 6044  t iterate one `D
-00007180: 6174 6120 6f62 6a65 6374 6020 696e 7369  ata object` insi
-00007190: 6465 2074 6865 206f 7468 6572 206f 6e65  de the other one
-000071a0: 2e0a 2020 2049 6620 796f 7520 7368 6f75  ..   If you shou
-000071b0: 6c64 2074 6f20 646f 2069 742c 2075 7365  ld to do it, use
-000071c0: 2073 686f 7274 2060 4461 7461 206f 626a   short `Data obj
-000071d0: 6563 7460 2066 6972 7374 2061 6e64 206c  ect` first and l
-000071e0: 6f6e 6720 6044 6174 6120 6f62 6a65 6374  ong `Data object
-000071f0: 6020 696e 7369 6465 2074 6865 206c 6f6f  ` inside the loo
-00007200: 702e 0a20 2020 4974 276c 6c20 616c 6c6f  p..   It'll allo
-00007210: 7720 796f 7520 6f70 656e 2074 6865 2063  w you open the c
-00007220: 6163 6865 2066 696c 6520 6f72 2063 7265  ache file or cre
-00007230: 6174 6520 6120 7265 7175 6573 7420 746f  ate a request to
-00007240: 2060 4461 7461 2073 6f75 7263 6560 206c   `Data source` l
-00007250: 6573 7320 6e75 6d62 6572 206f 6620 7469  ess number of ti
-00007260: 6d65 732e 0a0a 2320 342e 204f 6666 6963  mes...# 4. Offic
-00007270: 6961 6c20 4461 7461 536f 7572 6365 2069  ial DataSource i
-00007280: 6d70 6c65 6d65 6e74 6174 696f 6e73 0a0a  mplementations..
-00007290: 2d20 5b4c 6967 6874 7765 6967 6874 2044  - [Lightweight D
-000072a0: 6174 6120 5072 6f76 6964 6572 2044 6174  ata Provider Dat
-000072b0: 6120 536f 7572 6365 5d28 6874 7470 733a  a Source](https:
-000072c0: 2f2f 6769 7468 7562 2e63 6f6d 2f74 6832  //github.com/th2
-000072d0: 2d6e 6574 2f74 6832 2d64 732d 736f 7572  -net/th2-ds-sour
-000072e0: 6365 2d6c 7764 7029 0a0a 0a23 2035 2e20  ce-lwdp)...# 5. 
-000072f0: 4150 490a 0a49 6620 796f 7520 6172 6520  API..If you are 
-00007300: 6c6f 6f6b 696e 6720 666f 7220 636c 6173  looking for clas
-00007310: 7365 7320 6465 7363 7269 7074 696f 6e20  ses description 
-00007320: 7365 6520 7468 6520 5b41 5049 2044 6f63  see the [API Doc
-00007330: 756d 656e 7461 7469 6f6e 5d28 646f 6375  umentation](docu
-00007340: 6d65 6e74 6174 696f 6e2f 6170 692f 696e  mentation/api/in
-00007350: 6465 782e 6d64 292e 0a0a 2320 362e 2045  dex.md)...# 6. E
-00007360: 7861 6d70 6c65 730a 0a2d 205b 6765 745f  xamples..- [get_
-00007370: 7374 6172 7465 645f 6578 616d 706c 652e  started_example.
-00007380: 7079 5d28 6578 616d 706c 6573 2f67 6574  py](examples/get
-00007390: 5f73 7461 7274 6564 5f65 7861 6d70 6c65  _started_example
-000073a0: 2e70 7929 0a                             .py).
+00000f50: 6174 615f 7365 7276 6963 6573 2e64 756d  ata_services.dum
+00000f60: 6d79 2069 6d70 6f72 7420 4475 6d6d 7944  my import DummyD
+00000f70: 6174 6153 6f75 7263 650a 6672 6f6d 2074  ataSource.from t
+00000f80: 6832 5f64 6174 615f 7365 7276 6963 6573  h2_data_services
+00000f90: 2e65 7665 6e74 5f74 7265 6520 696d 706f  .event_tree impo
+00000fa0: 7274 2028 0a20 2020 2045 7665 6e74 5472  rt (.    EventTr
+00000fb0: 6565 2c0a 2020 2020 4576 656e 7454 7265  ee,.    EventTre
+00000fc0: 6543 6f6c 6c65 6374 696f 6e2c 0a20 2020  eCollection,.   
+00000fd0: 2050 6172 656e 7445 7665 6e74 5472 6565   ParentEventTree
+00000fe0: 436f 6c6c 6563 7469 6f6e 2c0a 2020 2020  Collection,.    
+00000ff0: 4945 5443 4472 6976 6572 2c0a 290a 6672  IETCDriver,.).fr
+00001000: 6f6d 2074 6832 5f64 6174 615f 7365 7276  om th2_data_serv
+00001010: 6963 6573 2e69 6e74 6572 6661 6365 7320  ices.interfaces 
+00001020: 696d 706f 7274 2049 4461 7461 536f 7572  import IDataSour
+00001030: 6365 0a66 726f 6d20 7468 325f 6461 7461  ce.from th2_data
+00001040: 5f73 6572 7669 6365 732e 7574 696c 732e  _services.utils.
+00001050: 636f 6e76 6572 7465 7273 2069 6d70 6f72  converters impor
+00001060: 7420 280a 2020 2020 4461 7465 7469 6d65  t (.    Datetime
+00001070: 436f 6e76 6572 7465 722c 0a20 2020 2044  Converter,.    D
+00001080: 6174 6574 696d 6553 7472 696e 6743 6f6e  atetimeStringCon
+00001090: 7665 7274 6572 2c0a 2020 2020 5072 6f74  verter,.    Prot
+000010a0: 6f62 7566 5469 6d65 7374 616d 7043 6f6e  obufTimestampCon
+000010b0: 7665 7274 6572 2c0a 2020 2020 5468 3254  verter,.    Th2T
+000010c0: 696d 6573 7461 6d70 436f 6e76 6572 7465  imestampConverte
+000010d0: 722c 0a29 0a0a 2323 2323 2323 2323 2323  r,.)..##########
+000010e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000010f0: 2323 2323 2323 2323 2323 2323 0a23 205b  ############.# [
+00001100: 305d 204c 6962 2063 6f6e 6669 6775 7261  0] Lib configura
+00001110: 7469 6f6e 0a23 2323 2323 2323 2323 2323  tion.###########
+00001120: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001130: 2323 2323 2323 2323 2323 230a 0a23 205b  ###########..# [
+00001140: 302e 315d 2049 6e74 6572 6163 7469 7665  0.1] Interactive
+00001150: 206f 7220 5363 7269 7074 206d 6f64 650a   or Script mode.
+00001160: 2320 4966 2079 6f75 2075 7365 2074 6865  # If you use the
+00001170: 206c 6962 2069 6e20 696e 7465 7261 6374   lib in interact
+00001180: 6976 6520 6d6f 6465 2028 6a75 7079 7465  ive mode (jupyte
+00001190: 722c 2069 7079 7468 6f6e 2920 6974 2773  r, ipython) it's
+000011a0: 2072 6563 6f6d 6d65 6e64 6564 2074 6f20   recommended to 
+000011b0: 7365 7420 7468 6520 7370 6563 6961 6c0a  set the special.
+000011c0: 2320 676c 6f62 616c 2070 6172 616d 6574  # global paramet
+000011d0: 6572 2074 6f20 5472 7565 2e20 4974 276c  er to True. It'l
+000011e0: 6c20 6b65 6570 2063 6163 6865 2066 696c  l keep cache fil
+000011f0: 6573 2069 6620 736f 6d65 7468 696e 6720  es if something 
+00001200: 7765 6e74 2077 726f 6e67 2e0a 6672 6f6d  went wrong..from
+00001210: 2074 6832 5f64 6174 615f 7365 7276 6963   th2_data_servic
+00001220: 6573 2e63 6f6e 6669 6720 696d 706f 7274  es.config import
+00001230: 206f 7074 696f 6e73 0a0a 6f70 7469 6f6e   options..option
+00001240: 732e 494e 5445 5241 4354 4956 455f 4d4f  s.INTERACTIVE_MO
+00001250: 4445 203d 2054 7275 650a 0a23 2053 6f6d  DE = True..# Som
+00001260: 6520 6578 616d 706c 6520 6461 7461 0a65  e example data.e
+00001270: 7665 6e74 7320 3d20 4461 7461 280a 2020  vents = Data(.  
+00001280: 2020 5b0a 2020 2020 2020 2020 7b0a 2020    [.        {.  
+00001290: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
+000012a0: 4964 223a 2022 6465 6d6f 5f62 6f6f 6b5f  Id": "demo_book_
+000012b0: 313a 7468 322d 7363 6f70 653a 3230 3233  1:th2-scope:2023
+000012c0: 3031 3035 3133 3537 3035 3536 3038 3733  0105135705560873
+000012d0: 3030 303a 6436 3165 3933 3061 2d38 6430  000:d61e930a-8d0
+000012e0: 302d 3131 6564 2d61 6131 612d 6433 3461  0-11ed-aa1a-d34a
+000012f0: 3631 3535 3135 3264 5f31 222c 0a20 2020  6155152d_1",.   
+00001300: 2020 2020 2020 2020 2022 6261 7463 6849           "batchI
+00001310: 6422 3a20 4e6f 6e65 2c0a 2020 2020 2020  d": None,.      
+00001320: 2020 2020 2020 2269 7342 6174 6368 6564        "isBatched
+00001330: 223a 2046 616c 7365 2c0a 2020 2020 2020  ": False,.      
+00001340: 2020 2020 2020 2265 7665 6e74 4e61 6d65        "eventName
+00001350: 223a 2022 5365 7420 6f66 2061 7574 6f2d  ": "Set of auto-
+00001360: 6765 6e65 7261 7465 6420 6576 656e 7473  generated events
+00001370: 2066 6f72 2064 7320 6c69 6220 7465 7374   for ds lib test
+00001380: 696e 6722 2c0a 2020 2020 2020 2020 2020  ing",.          
+00001390: 2020 2265 7665 6e74 5479 7065 223a 2022    "eventType": "
+000013a0: 6473 2d6c 6962 2d74 6573 742d 6576 656e  ds-lib-test-even
+000013b0: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+000013c0: 2265 6e64 5469 6d65 7374 616d 7022 3a20  "endTimestamp": 
+000013d0: 7b22 6570 6f63 6853 6563 6f6e 6422 3a20  {"epochSecond": 
+000013e0: 3136 3732 3932 3730 3235 2c20 226e 616e  1672927025, "nan
+000013f0: 6f22 3a20 3536 3137 3531 3030 307d 2c0a  o": 561751000},.
+00001400: 2020 2020 2020 2020 2020 2020 2273 7461              "sta
+00001410: 7274 5469 6d65 7374 616d 7022 3a20 7b22  rtTimestamp": {"
+00001420: 6570 6f63 6853 6563 6f6e 6422 3a20 3136  epochSecond": 16
+00001430: 3732 3932 3730 3235 2c20 226e 616e 6f22  72927025, "nano"
+00001440: 3a20 3536 3038 3733 3030 307d 2c0a 2020  : 560873000},.  
+00001450: 2020 2020 2020 2020 2020 2270 6172 656e            "paren
+00001460: 7445 7665 6e74 4964 223a 204e 6f6e 652c  tEventId": None,
+00001470: 0a20 2020 2020 2020 2020 2020 2022 7375  .            "su
+00001480: 6363 6573 7366 756c 223a 2054 7275 652c  ccessful": True,
+00001490: 0a20 2020 2020 2020 2020 2020 2022 626f  .            "bo
+000014a0: 6f6b 4964 223a 2022 6465 6d6f 5f62 6f6f  okId": "demo_boo
+000014b0: 6b5f 3122 2c0a 2020 2020 2020 2020 2020  k_1",.          
+000014c0: 2020 2273 636f 7065 223a 2022 7468 322d    "scope": "th2-
+000014d0: 7363 6f70 6522 2c0a 2020 2020 2020 2020  scope",.        
+000014e0: 2020 2020 2261 7474 6163 6865 644d 6573      "attachedMes
+000014f0: 7361 6765 4964 7322 3a20 5b5d 2c0a 2020  sageIds": [],.  
+00001500: 2020 2020 2020 2020 2020 2262 6f64 7922            "body"
+00001510: 3a20 5b5d 2c0a 2020 2020 2020 2020 7d2c  : [],.        },
+00001520: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
+00001530: 2020 2020 2020 2022 6576 656e 7449 6422         "eventId"
+00001540: 3a20 2264 656d 6f5f 626f 6f6b 5f31 3a74  : "demo_book_1:t
+00001550: 6832 2d73 636f 7065 3a32 3032 3330 3130  h2-scope:2023010
+00001560: 3531 3335 3730 3535 3633 3532 3230 3030  5135705563522000
+00001570: 3a39 6164 6262 3365 302d 3566 3862 2d34  :9adbb3e0-5f8b-4
+00001580: 6332 382d 6132 6163 2d37 3336 3165 3866  c28-a2ac-7361e8f
+00001590: 6137 3034 633e 6465 6d6f 5f62 6f6f 6b5f  a704c>demo_book_
+000015a0: 313a 7468 322d 7363 6f70 653a 3230 3233  1:th2-scope:2023
+000015b0: 3031 3035 3133 3537 3035 3536 3335 3232  0105135705563522
+000015c0: 3030 303a 6436 3165 3933 3061 2d38 6430  000:d61e930a-8d0
+000015d0: 302d 3131 6564 2d61 6131 612d 6433 3461  0-11ed-aa1a-d34a
+000015e0: 3631 3535 3135 3264 5f32 222c 0a20 2020  6155152d_2",.   
+000015f0: 2020 2020 2020 2020 2022 6261 7463 6849           "batchI
+00001600: 6422 3a20 2264 656d 6f5f 626f 6f6b 5f31  d": "demo_book_1
+00001610: 3a74 6832 2d73 636f 7065 3a32 3032 3330  :th2-scope:20230
+00001620: 3130 3531 3335 3730 3535 3633 3532 3230  1051357055635220
+00001630: 3030 3a39 6164 6262 3365 302d 3566 3862  00:9adbb3e0-5f8b
+00001640: 2d34 6332 382d 6132 6163 2d37 3336 3165  -4c28-a2ac-7361e
+00001650: 3866 6137 3034 6322 2c0a 2020 2020 2020  8fa704c",.      
+00001660: 2020 2020 2020 2269 7342 6174 6368 6564        "isBatched
+00001670: 223a 2054 7275 652c 0a20 2020 2020 2020  ": True,.       
+00001680: 2020 2020 2022 6576 656e 744e 616d 6522       "eventName"
+00001690: 3a20 2250 6c61 696e 2065 7665 6e74 2031  : "Plain event 1
+000016a0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000016b0: 6576 656e 7454 7970 6522 3a20 2264 732d  eventType": "ds-
+000016c0: 6c69 622d 7465 7374 2d65 7665 6e74 222c  lib-test-event",
+000016d0: 0a20 2020 2020 2020 2020 2020 2022 656e  .            "en
+000016e0: 6454 696d 6573 7461 6d70 223a 207b 2265  dTimestamp": {"e
+000016f0: 706f 6368 5365 636f 6e64 223a 2031 3637  pochSecond": 167
+00001700: 3239 3237 3032 352c 2022 6e61 6e6f 223a  2927025, "nano":
+00001710: 2035 3633 3634 3030 3030 7d2c 0a20 2020   563640000},.   
+00001720: 2020 2020 2020 2020 2022 7374 6172 7454           "startT
+00001730: 696d 6573 7461 6d70 223a 207b 2265 706f  imestamp": {"epo
+00001740: 6368 5365 636f 6e64 223a 2031 3637 3239  chSecond": 16729
+00001750: 3237 3032 352c 2022 6e61 6e6f 223a 2035  27025, "nano": 5
+00001760: 3633 3532 3230 3030 7d2c 0a20 2020 2020  63522000},.     
+00001770: 2020 2020 2020 2022 7061 7265 6e74 4576         "parentEv
+00001780: 656e 7449 6422 3a20 2264 656d 6f5f 626f  entId": "demo_bo
+00001790: 6f6b 5f31 3a74 6832 2d73 636f 7065 3a32  ok_1:th2-scope:2
+000017a0: 3032 3330 3130 3531 3335 3730 3535 3630  0230105135705560
+000017b0: 3837 3330 3030 3a64 3631 6539 3330 612d  873000:d61e930a-
+000017c0: 3864 3030 2d31 3165 642d 6161 3161 2d64  8d00-11ed-aa1a-d
+000017d0: 3334 6136 3135 3531 3532 645f 3122 2c0a  34a6155152d_1",.
+000017e0: 2020 2020 2020 2020 2020 2020 2273 7563              "suc
+000017f0: 6365 7373 6675 6c22 3a20 5472 7565 2c0a  cessful": True,.
+00001800: 2020 2020 2020 2020 2020 2020 2262 6f6f              "boo
+00001810: 6b49 6422 3a20 2264 656d 6f5f 626f 6f6b  kId": "demo_book
+00001820: 5f31 222c 0a20 2020 2020 2020 2020 2020  _1",.           
+00001830: 2022 7363 6f70 6522 3a20 2274 6832 2d73   "scope": "th2-s
+00001840: 636f 7065 222c 0a20 2020 2020 2020 2020  cope",.         
+00001850: 2020 2022 6174 7461 6368 6564 4d65 7373     "attachedMess
+00001860: 6167 6549 6473 223a 205b 5d2c 0a20 2020  ageIds": [],.   
+00001870: 2020 2020 2020 2020 2022 626f 6479 223a           "body":
+00001880: 207b 2274 7970 6522 3a20 226d 6573 7361   {"type": "messa
+00001890: 6765 222c 2022 6461 7461 223a 2022 6473  ge", "data": "ds
+000018a0: 2d6c 6962 2074 6573 7420 626f 6479 227d  -lib test body"}
+000018b0: 2c0a 2020 2020 2020 2020 7d2c 0a20 2020  ,.        },.   
+000018c0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+000018d0: 2020 2022 6576 656e 7449 6422 3a20 2264     "eventId": "d
+000018e0: 656d 6f5f 626f 6f6b 5f31 3a74 6832 2d73  emo_book_1:th2-s
+000018f0: 636f 7065 3a32 3032 3330 3130 3531 3335  cope:20230105135
+00001900: 3730 3535 3633 3532 3230 3030 3a39 6164  705563522000:9ad
+00001910: 6262 3365 302d 3566 3862 2d34 6332 382d  bb3e0-5f8b-4c28-
+00001920: 6132 6163 2d37 3336 3165 3866 6137 3034  a2ac-7361e8fa704
+00001930: 633e 6465 6d6f 5f62 6f6f 6b5f 313a 7468  c>demo_book_1:th
+00001940: 322d 7363 6f70 653a 3230 3233 3031 3035  2-scope:20230105
+00001950: 3133 3537 3035 3536 3337 3537 3030 303a  135705563757000:
+00001960: 6436 3165 3933 3061 2d38 6430 302d 3131  d61e930a-8d00-11
+00001970: 6564 2d61 6131 612d 6433 3461 3631 3535  ed-aa1a-d34a6155
+00001980: 3135 3264 5f33 222c 0a20 2020 2020 2020  152d_3",.       
+00001990: 2020 2020 2022 6261 7463 6849 6422 3a20       "batchId": 
+000019a0: 2264 656d 6f5f 626f 6f6b 5f31 3a74 6832  "demo_book_1:th2
+000019b0: 2d73 636f 7065 3a32 3032 3330 3130 3531  -scope:202301051
+000019c0: 3335 3730 3535 3633 3532 3230 3030 3a39  35705563522000:9
+000019d0: 6164 6262 3365 302d 3566 3862 2d34 6332  adbb3e0-5f8b-4c2
+000019e0: 382d 6132 6163 2d37 3336 3165 3866 6137  8-a2ac-7361e8fa7
+000019f0: 3034 6322 2c0a 2020 2020 2020 2020 2020  04c",.          
+00001a00: 2020 2269 7342 6174 6368 6564 223a 2054    "isBatched": T
+00001a10: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00001a20: 2022 6576 656e 744e 616d 6522 3a20 2250   "eventName": "P
+00001a30: 6c61 696e 2065 7665 6e74 2032 222c 0a20  lain event 2",. 
+00001a40: 2020 2020 2020 2020 2020 2022 6576 656e             "even
+00001a50: 7454 7970 6522 3a20 2264 732d 6c69 622d  tType": "ds-lib-
+00001a60: 7465 7374 2d65 7665 6e74 222c 0a20 2020  test-event",.   
+00001a70: 2020 2020 2020 2020 2022 656e 6454 696d           "endTim
+00001a80: 6573 7461 6d70 223a 207b 2265 706f 6368  estamp": {"epoch
+00001a90: 5365 636f 6e64 223a 2031 3637 3239 3237  Second": 1672927
+00001aa0: 3032 352c 2022 6e61 6e6f 223a 2035 3633  025, "nano": 563
+00001ab0: 3739 3130 3030 7d2c 0a20 2020 2020 2020  791000},.       
+00001ac0: 2020 2020 2022 7374 6172 7454 696d 6573       "startTimes
+00001ad0: 7461 6d70 223a 207b 2265 706f 6368 5365  tamp": {"epochSe
+00001ae0: 636f 6e64 223a 2031 3637 3239 3237 3032  cond": 167292702
+00001af0: 352c 2022 6e61 6e6f 223a 2035 3633 3735  5, "nano": 56375
+00001b00: 3730 3030 7d2c 0a20 2020 2020 2020 2020  7000},.         
+00001b10: 2020 2022 7061 7265 6e74 4576 656e 7449     "parentEventI
+00001b20: 6422 3a20 2264 656d 6f5f 626f 6f6b 5f31  d": "demo_book_1
+00001b30: 3a74 6832 2d73 636f 7065 3a32 3032 3330  :th2-scope:20230
+00001b40: 3130 3531 3335 3730 3535 3630 3837 3330  1051357055608730
+00001b50: 3030 3a64 3631 6539 3330 612d 3864 3030  00:d61e930a-8d00
+00001b60: 2d31 3165 642d 6161 3161 2d64 3334 6136  -11ed-aa1a-d34a6
+00001b70: 3135 3531 3532 645f 3122 2c0a 2020 2020  155152d_1",.    
+00001b80: 2020 2020 2020 2020 2273 7563 6365 7373          "success
+00001b90: 6675 6c22 3a20 5472 7565 2c0a 2020 2020  ful": True,.    
+00001ba0: 2020 2020 2020 2020 2262 6f6f 6b49 6422          "bookId"
+00001bb0: 3a20 2264 656d 6f5f 626f 6f6b 5f31 222c  : "demo_book_1",
+00001bc0: 0a20 2020 2020 2020 2020 2020 2022 7363  .            "sc
+00001bd0: 6f70 6522 3a20 2274 6832 2d73 636f 7065  ope": "th2-scope
+00001be0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00001bf0: 6174 7461 6368 6564 4d65 7373 6167 6549  attachedMessageI
+00001c00: 6473 223a 205b 5d2c 0a20 2020 2020 2020  ds": [],.       
+00001c10: 2020 2020 2022 626f 6479 223a 207b 2274       "body": {"t
+00001c20: 7970 6522 3a20 226d 6573 7361 6765 222c  ype": "message",
+00001c30: 2022 6461 7461 223a 2022 6473 2d6c 6962   "data": "ds-lib
+00001c40: 2074 6573 7420 626f 6479 227d 2c0a 2020   test body"},.  
+00001c50: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00001c60: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00001c70: 6576 656e 7449 6422 3a20 2266 616b 652d  eventId": "fake-
+00001c80: 6576 656e 7449 6422 2c0a 2020 2020 2020  eventId",.      
+00001c90: 2020 2020 2020 2262 6174 6368 4964 223a        "batchId":
+00001ca0: 2022 6661 6b65 2d62 6174 6368 4964 222c   "fake-batchId",
+00001cb0: 0a20 2020 2020 2020 2020 2020 2022 6973  .            "is
+00001cc0: 4261 7463 6865 6422 3a20 5472 7565 2c0a  Batched": True,.
+00001cd0: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
+00001ce0: 6e74 4e61 6d65 223a 2022 4661 6b65 2065  ntName": "Fake e
+00001cf0: 7665 6e74 222c 0a20 2020 2020 2020 2020  vent",.         
+00001d00: 2020 2022 6576 656e 7454 7970 6522 3a20     "eventType": 
+00001d10: 2264 732d 6c69 622d 7465 7374 2d65 7665  "ds-lib-test-eve
+00001d20: 6e74 222c 0a20 2020 2020 2020 2020 2020  nt",.           
+00001d30: 2022 656e 6454 696d 6573 7461 6d70 223a   "endTimestamp":
+00001d40: 207b 2265 706f 6368 5365 636f 6e64 223a   {"epochSecond":
+00001d50: 2031 3637 3239 3237 3033 352c 2022 6e61   1672927035, "na
+00001d60: 6e6f 223a 2035 3633 3739 3130 3030 7d2c  no": 563791000},
+00001d70: 0a20 2020 2020 2020 2020 2020 2022 7374  .            "st
+00001d80: 6172 7454 696d 6573 7461 6d70 223a 207b  artTimestamp": {
+00001d90: 2265 706f 6368 5365 636f 6e64 223a 2031  "epochSecond": 1
+00001da0: 3637 3239 3237 3332 352c 2022 6e61 6e6f  672927325, "nano
+00001db0: 223a 2035 3633 3735 3730 3030 7d2c 0a20  ": 563757000},. 
+00001dc0: 2020 2020 2020 2020 2020 2022 7061 7265             "pare
+00001dd0: 6e74 4576 656e 7449 6422 3a20 226e 6f74  ntEventId": "not
+00001de0: 5f65 7869 7374 735f 696e 5f74 6865 5f65  _exists_in_the_e
+00001df0: 7665 6e74 735f 7374 7265 616d 222c 0a20  vents_stream",. 
+00001e00: 2020 2020 2020 2020 2020 2022 7375 6363             "succ
+00001e10: 6573 7366 756c 223a 2046 616c 7365 2c0a  essful": False,.
+00001e20: 2020 2020 2020 2020 2020 2020 2262 6f6f              "boo
+00001e30: 6b49 6422 3a20 2264 656d 6f5f 626f 6f6b  kId": "demo_book
+00001e40: 5f31 222c 0a20 2020 2020 2020 2020 2020  _1",.           
+00001e50: 2022 7363 6f70 6522 3a20 2274 6832 2d73   "scope": "th2-s
+00001e60: 636f 7065 222c 0a20 2020 2020 2020 2020  cope",.         
+00001e70: 2020 2022 6174 7461 6368 6564 4d65 7373     "attachedMess
+00001e80: 6167 6549 6473 223a 205b 5d2c 0a20 2020  ageIds": [],.   
+00001e90: 2020 2020 2020 2020 2022 626f 6479 223a           "body":
+00001ea0: 207b 2274 7970 6522 3a20 226d 6573 7361   {"type": "messa
+00001eb0: 6765 222c 2022 6461 7461 223a 2022 6473  ge", "data": "ds
+00001ec0: 2d6c 6962 2074 6573 7420 626f 6479 227d  -lib test body"}
+00001ed0: 2c0a 2020 2020 2020 2020 7d2c 0a20 2020  ,.        },.   
+00001ee0: 205d 0a29 0a0a 2323 2323 2323 2323 2323   ].)..##########
+00001ef0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001f00: 2323 2323 2323 2323 2323 2323 0a23 205b  ############.# [
+00001f10: 315d 2057 6f72 6b69 6e67 2077 6974 6820  1] Working with 
+00001f20: 6120 4461 7461 206f 626a 6563 742e 0a23  a Data object..#
+00001f30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001f40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001f50: 2323 2323 230a 0a23 205b 312e 315d 2046  #####..# [1.1] F
+00001f60: 696c 7465 722e 0a66 696c 7465 7265 645f  ilter..filtered_
+00001f70: 6576 656e 7473 3a20 4461 7461 203d 2065  events: Data = e
+00001f80: 7665 6e74 732e 6669 6c74 6572 286c 616d  vents.filter(lam
+00001f90: 6264 6120 653a 2065 5b22 626f 6479 225d  bda e: e["body"]
+00001fa0: 2021 3d20 5b5d 2920 2023 2046 696c 7465   != [])  # Filte
+00001fb0: 7220 6576 656e 7473 2077 6974 6820 656d  r events with em
+00001fc0: 7074 7920 626f 6479 2e0a 0a0a 2320 5b31  pty body....# [1
+00001fd0: 2e32 5d20 4d61 702e 0a64 6566 2074 7261  .2] Map..def tra
+00001fe0: 6e73 666f 726d 5f66 756e 6374 696f 6e28  nsform_function(
+00001ff0: 7265 636f 7264 293a 0a20 2020 2072 6574  record):.    ret
+00002000: 7572 6e20 7b22 6576 656e 744e 616d 6522  urn {"eventName"
+00002010: 3a20 7265 636f 7264 5b22 6576 656e 744e  : record["eventN
+00002020: 616d 6522 5d2c 2022 7375 6363 6573 7366  ame"], "successf
+00002030: 756c 223a 2072 6563 6f72 645b 2273 7563  ul": record["suc
+00002040: 6365 7373 6675 6c22 5d7d 0a0a 0a66 696c  cessful"]}...fil
+00002050: 7465 7265 645f 616e 645f 6d61 7070 6564  tered_and_mapped
+00002060: 5f65 7665 6e74 7320 3d20 6669 6c74 6572  _events = filter
+00002070: 6564 5f65 7665 6e74 732e 6d61 7028 7472  ed_events.map(tr
+00002080: 616e 7366 6f72 6d5f 6675 6e63 7469 6f6e  ansform_function
+00002090: 290a 0a23 205b 312e 335d 2044 6174 6120  )..# [1.3] Data 
+000020a0: 7069 7065 6c69 6e65 2e0a 2320 2020 2020  pipeline..#     
+000020b0: 2020 496e 7374 6561 6420 6f66 2064 6f69    Instead of doi
+000020c0: 6e67 2064 6174 6120 7472 616e 7366 6f72  ng data transfor
+000020d0: 6d61 7469 6f6e 7320 7374 6570 2062 7920  mations step by 
+000020e0: 7374 6570 2079 6f75 2063 616e 2064 6f20  step you can do 
+000020f0: 6974 2069 6e20 6f6e 6520 6c69 6e65 2e0a  it in one line..
+00002100: 6669 6c74 6572 6564 5f61 6e64 5f6d 6170  filtered_and_map
+00002110: 7065 645f 6576 656e 7473 5f62 795f 7069  ped_events_by_pi
+00002120: 7065 6c69 6e65 203d 2065 7665 6e74 732e  peline = events.
+00002130: 6669 6c74 6572 286c 616d 6264 6120 653a  filter(lambda e:
+00002140: 2065 5b22 626f 6479 225d 2021 3d20 5b5d   e["body"] != []
+00002150: 292e 6d61 7028 0a20 2020 2074 7261 6e73  ).map(.    trans
+00002160: 666f 726d 5f66 756e 6374 696f 6e0a 290a  form_function.).
+00002170: 2320 436f 6e74 656e 7420 6f66 2074 6865  # Content of the
+00002180: 7365 2074 776f 2044 6174 6120 6f62 6a65  se two Data obje
+00002190: 6374 7320 7368 6f75 6c64 2062 6520 6571  cts should be eq
+000021a0: 7561 6c2e 0a61 7373 6572 7420 6c69 7374  ual..assert list
+000021b0: 2866 696c 7465 7265 645f 616e 645f 6d61  (filtered_and_ma
+000021c0: 7070 6564 5f65 7665 6e74 7329 203d 3d20  pped_events) == 
+000021d0: 6c69 7374 2866 696c 7465 7265 645f 616e  list(filtered_an
+000021e0: 645f 6d61 7070 6564 5f65 7665 6e74 735f  d_mapped_events_
+000021f0: 6279 5f70 6970 656c 696e 6529 0a0a 2320  by_pipeline)..# 
+00002200: 5b31 2e34 5d20 5369 6674 2e20 536b 6970  [1.4] Sift. Skip
+00002210: 2074 6865 2066 6972 7374 2066 6577 2069   the first few i
+00002220: 7465 6d73 206f 7220 6c69 6d69 7420 7468  tems or limit th
+00002230: 656d 2e0a 6461 7461 203d 2044 6174 6128  em..data = Data(
+00002240: 5b31 2c20 322c 2033 2c20 342c 2035 2c20  [1, 2, 3, 4, 5, 
+00002250: 362c 2037 2c20 382c 2039 2c20 3130 2c20  6, 7, 8, 9, 10, 
+00002260: 3131 2c20 3132 2c20 3133 2c20 3134 2c20  11, 12, 13, 14, 
+00002270: 3135 5d29 0a69 7465 6d73 5f66 726f 6d5f  15]).items_from_
+00002280: 3131 5f74 6f5f 656e 643a 2047 656e 6572  11_to_end: Gener
+00002290: 6174 6f72 203d 2064 6174 612e 7369 6674  ator = data.sift
+000022a0: 2873 6b69 703d 3130 290a 6f6e 6c79 5f66  (skip=10).only_f
+000022b0: 6972 7374 5f31 305f 6974 656d 733a 2047  irst_10_items: G
+000022c0: 656e 6572 6174 6f72 203d 2064 6174 612e  enerator = data.
+000022d0: 7369 6674 286c 696d 6974 3d31 3029 0a0a  sift(limit=10)..
+000022e0: 2320 5b31 2e35 5d20 4368 616e 6769 6e67  # [1.5] Changing
+000022f0: 2063 6163 6865 2073 7461 7475 732e 0a65   cache status..e
+00002300: 7665 6e74 732e 7573 655f 6361 6368 6528  vents.use_cache(
+00002310: 5472 7565 290a 2320 6f72 206a 7573 740a  True).# or just.
+00002320: 6576 656e 7473 2e75 7365 5f63 6163 6865  events.use_cache
+00002330: 2829 2020 2320 4966 2079 6f75 2077 616e  ()  # If you wan
+00002340: 7420 746f 2061 6374 6976 6174 6520 6361  t to activate ca
+00002350: 6368 652e 0a23 205b 312e 365d 2057 616c  che..# [1.6] Wal
+00002360: 6b20 7468 726f 7567 6820 6461 7461 2e0a  k through data..
+00002370: 666f 7220 6576 656e 7420 696e 2065 7665  for event in eve
+00002380: 6e74 733a 0a20 2020 2023 2044 6f20 736f  nts:.    # Do so
+00002390: 6d65 7468 696e 6720 7769 7468 2065 7665  mething with eve
+000023a0: 6e74 2028 6576 656e 7420 6973 2061 2064  nt (event is a d
+000023b0: 6963 7429 2e0a 2020 2020 7072 696e 7428  ict)..    print(
+000023c0: 6576 656e 7429 0a23 2041 6674 6572 2066  event).# After f
+000023d0: 6972 7374 2069 7465 7261 7469 6f6e 2074  irst iteration t
+000023e0: 6865 2065 7665 6e74 7320 6861 7320 6120  he events has a 
+000023f0: 6361 6368 6520 6669 6c65 2e0a 2320 4e6f  cache file..# No
+00002400: 7720 7468 6579 2077 696c 6c20 6265 2075  w they will be u
+00002410: 7365 6420 696e 2074 6865 2063 6163 6865  sed in the cache
+00002420: 2069 6e20 7468 6520 6e65 7874 2069 7465   in the next ite
+00002430: 7261 7469 6f6e 2e0a 0a23 205b 312e 375d  ration...# [1.7]
+00002440: 2047 6574 206e 756d 6265 7220 6f66 2074   Get number of t
+00002450: 6865 2065 6c65 6d65 6e74 7320 696e 2074  he elements in t
+00002460: 6865 2044 6174 6120 6f62 6a65 6374 2e0a  he Data object..
+00002470: 6e75 6d62 6572 5f6f 665f 6576 656e 7473  number_of_events
+00002480: 203d 2065 7665 6e74 732e 6c65 6e0a 0a23   = events.len..#
+00002490: 205b 312e 385d 2043 6865 636b 2074 6861   [1.8] Check tha
+000024a0: 7420 4461 7461 206f 626a 6563 7420 6973  t Data object is
+000024b0: 6e27 7420 656d 7074 792e 0a23 2054 6865  n't empty..# The
+000024c0: 2064 6174 6120 736f 7572 6365 2073 686f   data source sho
+000024d0: 756c 6420 6265 206e 6f74 2065 6d70 7479  uld be not empty
+000024e0: 2e0a 6173 7365 7274 2065 7665 6e74 732e  ..assert events.
+000024f0: 6973 5f65 6d70 7479 2069 7320 4661 6c73  is_empty is Fals
+00002500: 650a 0a23 205b 312e 395d 2043 6f6e 7665  e..# [1.9] Conve
+00002510: 7274 2044 6174 6120 6f62 6a65 6374 2074  rt Data object t
+00002520: 6f20 7468 6520 6c69 7374 206f 6620 656c  o the list of el
+00002530: 656d 656e 7473 2865 7665 6e74 7320 6f72  ements(events or
+00002540: 206d 6573 7361 6765 7329 2e0a 2320 4265   messages)..# Be
+00002550: 2063 6172 6566 756c 2c20 7468 6973 2063   careful, this c
+00002560: 616e 2074 616b 6520 746f 6f20 6d75 6368  an take too much
+00002570: 206d 656d 6f72 792e 0a65 7665 6e74 735f   memory..events_
+00002580: 6c69 7374 203d 206c 6973 7428 6576 656e  list = list(even
+00002590: 7473 290a 0a23 205b 312e 3130 5d20 5468  ts)..# [1.10] Th
+000025a0: 6520 6361 6368 6520 696e 6865 7269 7461  e cache inherita
+000025b0: 6e63 652e 0a23 2043 7265 6174 6573 2061  nce..# Creates a
+000025c0: 206e 6577 2044 6174 6120 6f62 6a65 6374   new Data object
+000025d0: 2074 6861 7420 7769 6c6c 2075 7365 2063   that will use c
+000025e0: 6163 6865 2066 726f 6d20 7468 6520 6576  ache from the ev
+000025f0: 656e 7473 2044 6174 6120 6f62 6a65 6374  ents Data object
+00002600: 2e0a 6576 656e 7473 5f66 696c 7465 7265  ..events_filtere
+00002610: 643a 2044 6174 6120 3d20 6576 656e 7473  d: Data = events
+00002620: 2e66 696c 7465 7228 6c61 6d62 6461 2072  .filter(lambda r
+00002630: 6563 6f72 643a 2072 6563 6f72 642e 6765  ecord: record.ge
+00002640: 7428 2262 6174 6368 4964 2229 290a 0a23  t("batchId"))..#
+00002650: 204e 6577 2044 6174 6120 6f62 6a65 6374   New Data object
+00002660: 7320 646f 6e27 7420 7573 6520 7468 6569  s don't use thei
+00002670: 7220 6f77 6e20 6361 6368 6520 6279 2064  r own cache by d
+00002680: 6566 6175 6c74 2062 7574 2075 7365 2074  efault but use t
+00002690: 6865 2063 6163 6865 206f 6620 7468 6520  he cache of the 
+000026a0: 7061 7265 6e74 2044 6174 6120 6f62 6a65  parent Data obje
+000026b0: 6374 2e0a 2320 5573 6520 7573 655f 6361  ct..# Use use_ca
+000026c0: 6368 6520 6d65 7468 6f64 2074 6f20 6163  che method to ac
+000026d0: 7469 7661 7465 2063 6163 6869 6e67 2e0a  tivate caching..
+000026e0: 2320 4166 7465 7220 7468 6174 2c20 7468  # After that, th
+000026f0: 6520 4461 7461 206f 626a 6563 7420 7769  e Data object wi
+00002700: 6c6c 2063 7265 6174 6520 6974 7320 6f77  ll create its ow
+00002710: 6e20 6361 6368 6520 6669 6c65 2e0a 6576  n cache file..ev
+00002720: 656e 7473 5f66 696c 7465 7265 642e 7573  ents_filtered.us
+00002730: 655f 6361 6368 6528 290a 0a6c 6973 7428  e_cache()..list(
+00002740: 6576 656e 7473 5f66 696c 7465 7265 6429  events_filtered)
+00002750: 2020 2320 4a75 7374 2074 6f20 6974 6572    # Just to iter
+00002760: 6174 6520 4461 7461 206f 626a 6563 7420  ate Data object 
+00002770: 2863 6163 6865 2066 696c 6520 7769 6c6c  (cache file will
+00002780: 2062 6520 6372 6561 7465 6429 2e0a 0a66   be created)...f
+00002790: 696c 7465 7265 645f 6576 656e 7473 5f74  iltered_events_t
+000027a0: 7970 6573 203d 2065 7665 6e74 735f 6669  ypes = events_fi
+000027b0: 6c74 6572 6564 2e6d 6170 286c 616d 6264  ltered.map(lambd
+000027c0: 6120 7265 636f 7264 3a20 7b22 6576 656e  a record: {"even
+000027d0: 7454 7970 6522 3a20 7265 636f 7264 2e67  tType": record.g
+000027e0: 6574 2822 6576 656e 7454 7970 6522 297d  et("eventType")}
+000027f0: 290a 0a65 7665 6e74 735f 7769 7468 6f75  )..events_withou
+00002800: 745f 7479 7065 735f 7769 7468 5f62 6174  t_types_with_bat
+00002810: 6368 203d 2066 696c 7465 7265 645f 6576  ch = filtered_ev
+00002820: 656e 7473 5f74 7970 6573 2e66 696c 7465  ents_types.filte
+00002830: 7228 0a20 2020 206c 616d 6264 6120 7265  r(.    lambda re
+00002840: 636f 7264 3a20 6e6f 7420 7265 636f 7264  cord: not record
+00002850: 2e67 6574 2822 6576 656e 7454 7970 6522  .get("eventType"
+00002860: 290a 290a 6576 656e 7473 5f77 6974 686f  ).).events_witho
+00002870: 7574 5f74 7970 6573 5f77 6974 685f 6261  ut_types_with_ba
+00002880: 7463 682e 7573 655f 6361 6368 6528 290a  tch.use_cache().
+00002890: 0a23 205b 312e 3131 5d20 4461 7461 206f  .# [1.11] Data o
+000028a0: 626a 6563 7473 206a 6f69 6e69 6e67 2e0a  bjects joining..
+000028b0: 2320 596f 7520 6861 7665 2074 6865 2066  # You have the f
+000028c0: 6f6c 6c6f 7769 6e67 2033 2044 6174 6120  ollowing 3 Data 
+000028d0: 6f62 6a65 6374 732e 0a64 3120 3d20 4461  objects..d1 = Da
+000028e0: 7461 285b 312c 2032 2c20 335d 290a 6432  ta([1, 2, 3]).d2
+000028f0: 203d 2044 6174 6128 5b22 6122 2c20 7b22   = Data(["a", {"
+00002900: 6964 223a 2031 3233 7d2c 2022 6322 5d29  id": 123}, "c"])
+00002910: 0a64 3320 3d20 4461 7461 285b 372c 2038  .d3 = Data([7, 8
+00002920: 2c20 395d 290a 2320 596f 7520 6361 6e20  , 9]).# You can 
+00002930: 6a6f 696e 2044 6174 6120 6f62 6a65 6374  join Data object
+00002940: 7320 696e 2066 6f6c 6c6f 7769 6e67 2077  s in following w
+00002950: 6179 732e 0a23 2050 6c65 6173 6520 6e6f  ays..# Please no
+00002960: 7465 2c20 6e65 7720 4461 7461 206f 626a  te, new Data obj
+00002970: 6563 7420 7769 6c6c 2068 6176 6520 6361  ect will have ca
+00002980: 6368 6520 7374 6174 7573 203d 3d20 4661  che status == Fa
+00002990: 6c73 652e 0a64 6174 615f 7669 615f 696e  lse..data_via_in
+000029a0: 6974 203d 2044 6174 6128 5b64 312c 2064  it = Data([d1, d
+000029b0: 322c 2064 335d 290a 6461 7461 5f76 6961  2, d3]).data_via
+000029c0: 5f61 6464 203d 2064 3120 2b20 6432 202b  _add = d1 + d2 +
+000029d0: 2064 330a 6461 7461 5f77 6974 685f 6e6f   d3.data_with_no
+000029e0: 6e5f 6461 7461 5f6f 626a 5f76 6961 5f69  n_data_obj_via_i
+000029f0: 6e69 7420 3d20 4461 7461 285b 6431 2c20  nit = Data([d1, 
+00002a00: 5b22 6122 2c20 7b22 6964 223a 2031 3233  ["a", {"id": 123
+00002a10: 7d2c 2022 6322 5d2c 2064 335d 290a 6461  }, "c"], d3]).da
+00002a20: 7461 5f77 6974 685f 6e6f 6e5f 6461 7461  ta_with_non_data
+00002a30: 5f6f 626a 5f76 6961 5f61 6464 203d 2064  _obj_via_add = d
+00002a40: 3120 2b20 5b22 6122 2c20 7b22 6964 223a  1 + ["a", {"id":
+00002a50: 2031 3233 7d2c 2022 6322 5d20 2b20 6433   123}, "c"] + d3
+00002a60: 0a23 2059 6f75 2063 616e 206a 6f69 6e20  .# You can join 
+00002a70: 6375 7272 656e 7420 4461 7461 206f 626a  current Data obj
+00002a80: 6563 7420 6f6e 2070 6c61 6365 2075 7369  ect on place usi
+00002a90: 6e67 202b 3d2e 0a23 2049 7420 7769 6c6c  ng +=..# It will
+00002aa0: 206b 6565 7020 6361 6368 6520 7374 6174   keep cache stat
+00002ab0: 7573 2e0a 6431 202b 3d20 6433 2020 2320  us..d1 += d3  # 
+00002ac0: 6431 2077 696c 6c20 6265 636f 6d65 2044  d1 will become D
+00002ad0: 6174 6128 5b31 2c32 2c33 2c37 2c38 2c39  ata([1,2,3,7,8,9
+00002ae0: 5d29 0a0a 2320 5b31 2e31 325d 2042 7569  ])..# [1.12] Bui
+00002af0: 6c64 2061 6e64 2072 6561 6420 4461 7461  ld and read Data
+00002b00: 206f 626a 6563 7420 6361 6368 6520 6669   object cache fi
+00002b10: 6c65 732e 0a65 7665 6e74 732e 6275 696c  les..events.buil
+00002b20: 645f 6361 6368 6528 2263 6163 6865 5f66  d_cache("cache_f
+00002b30: 696c 656e 616d 655f 6f72 5f70 6174 6822  ilename_or_path"
+00002b40: 290a 6461 7461 5f6f 626a 5f66 726f 6d5f  ).data_obj_from_
+00002b50: 6361 6368 6520 3d20 4461 7461 2e66 726f  cache = Data.fro
+00002b60: 6d5f 6361 6368 655f 6669 6c65 2822 6361  m_cache_file("ca
+00002b70: 6368 655f 6669 6c65 6e61 6d65 5f6f 725f  che_filename_or_
+00002b80: 7061 7468 2229 0a0a 2320 5b31 2e31 335d  path")..# [1.13]
+00002b90: 2043 6865 636b 2069 6620 4461 7461 2069   Check if Data i
+00002ba0: 7320 736f 7274 6564 2e0a 2320 5468 6174  s sorted..# That
+00002bb0: 2077 696c 6c20 7265 7475 726e 2061 6e20   will return an 
+00002bc0: 6f62 6a65 6374 2060 6973 5f73 6f72 7465  object `is_sorte
+00002bd0: 6460 2074 6861 7420 636f 6e74 6169 6e73  d` that contains
+00002be0: 2069 6e66 6f72 6d61 7469 6f6e 0a23 2020   information.#  
+00002bf0: 2031 2e20 7374 6174 7573 202d 2d20 736f   1. status -- so
+00002c00: 7274 6564 206f 7220 6e6f 740a 2320 2020  rted or not.#   
+00002c10: 322e 2066 6972 7374 5f75 6e73 6f72 7465  2. first_unsorte
+00002c20: 6420 2d2d 2074 6865 2069 6e64 6578 206f  d -- the index o
+00002c30: 6620 7468 6520 6669 7273 7420 756e 736f  f the first unso
+00002c40: 7274 6564 2065 6c65 6d65 6e74 0a69 735f  rted element.is_
+00002c50: 736f 7274 6564 203d 2065 7665 6e74 732e  sorted = events.
+00002c60: 6973 5f73 6f72 7465 6428 6c61 6d62 6461  is_sorted(lambda
+00002c70: 2065 3a20 655b 2273 7461 7274 5469 6d65   e: e["startTime
+00002c80: 7374 616d 7022 5d5b 2265 706f 6368 5365  stamp"]["epochSe
+00002c90: 636f 6e64 225d 290a 0a23 2059 6f75 2063  cond"])..# You c
+00002ca0: 616e 2075 7365 2074 6869 7320 6f62 6a65  an use this obje
+00002cb0: 6374 2061 7320 7573 7561 6c20 626f 6f6c  ct as usual bool
+00002cc0: 2076 6172 6961 626c 652e 0a69 6620 6973   variable..if is
+00002cd0: 5f73 6f72 7465 643a 0a20 2020 2070 7269  _sorted:.    pri
+00002ce0: 6e74 2822 6576 656e 7473 2044 6174 6120  nt("events Data 
+00002cf0: 6f62 6a20 6973 2073 6f72 7465 6421 2229  obj is sorted!")
+00002d00: 0a0a 2320 5b31 2e31 345d 2055 7365 2060  ..# [1.14] Use `
+00002d10: 4461 7461 2e73 686f 7728 2960 2074 6f20  Data.show()` to 
+00002d20: 6c6f 6f6b 2061 7420 7468 6520 6669 7273  look at the firs
+00002d30: 7420 4e20 6d65 7373 6167 6573 2069 6e20  t N messages in 
+00002d40: 7468 6520 7374 7265 616d 2e0a 6461 7461  the stream..data
+00002d50: 5f77 6974 685f 6e6f 6e5f 6461 7461 5f6f  _with_non_data_o
+00002d60: 626a 5f76 6961 5f61 6464 2e73 686f 7728  bj_via_add.show(
+00002d70: 6e3d 3629 0a23 2057 696c 6c20 7072 696e  n=6).# Will prin
+00002d80: 740a 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  t.# ------------
+00002d90: 2d20 5072 696e 7465 6420 6669 7273 7420  - Printed first 
+00002da0: 3620 7265 636f 7264 7320 2d2d 2d2d 2d2d  6 records ------
+00002db0: 2d2d 2d2d 2d2d 2d0a 2320 5b31 5d20 2d2d  -------.# [1] --
+00002dc0: 2d2d 2d2d 0a23 2031 0a23 205b 325d 202d  ----.# 1.# [2] -
+00002dd0: 2d2d 2d2d 2d0a 2320 320a 2320 5b33 5d20  -----.# 2.# [3] 
+00002de0: 2d2d 2d2d 2d2d 0a23 2033 0a23 205b 345d  ------.# 3.# [4]
+00002df0: 202d 2d2d 2d2d 2d0a 2320 2761 270a 2320   ------.# 'a'.# 
+00002e00: 5b35 5d20 2d2d 2d2d 2d2d 0a23 207b 2769  [5] ------.# {'i
+00002e10: 6427 3a20 3132 337d 0a23 205b 365d 202d  d': 123}.# [6] -
+00002e20: 2d2d 2d2d 2d0a 2320 2763 270a 0a23 205b  -----.# 'c'..# [
+00002e30: 312e 3135 5d20 596f 7520 6361 6e20 7265  1.15] You can re
+00002e40: 6d6f 7665 2074 6865 2063 6163 6865 2066  move the cache f
+00002e50: 696c 6520 6f66 2074 6865 2044 6174 6120  ile of the Data 
+00002e60: 6f62 6a65 6374 2c20 6966 2072 6571 7569  object, if requi
+00002e70: 7265 642e 0a64 6174 615f 6f62 6a5f 6672  red..data_obj_fr
+00002e80: 6f6d 5f63 6163 6865 2e63 6c65 6172 5f63  om_cache.clear_c
+00002e90: 6163 6865 2829 0a0a 2323 2323 2323 2323  ache()..########
+00002ea0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002eb0: 2323 2323 2323 2323 2323 2323 2323 0a23  ##############.#
+00002ec0: 205b 325d 2057 6f72 6b69 6e67 2077 6974   [2] Working wit
+00002ed0: 6820 636f 6e76 6572 7465 7273 2e0a 2323  h converters..##
+00002ee0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002ef0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002f00: 2323 2323 0a23 2054 6865 7265 2061 7265  ####.# There are
+00002f10: 2063 7572 7265 6e74 6c79 2074 6872 6565   currently three
+00002f20: 2069 6d70 6c65 6d65 6e74 6174 696f 6e73   implementations
+00002f30: 206f 6620 4954 696d 6573 7461 6d70 436f   of ITimestampCo
+00002f40: 6e76 6572 7465 7220 636c 6173 733a 2044  nverter class: D
+00002f50: 6174 6574 696d 6543 6f6e 7665 7274 652c  atetimeConverte,
+00002f60: 2044 6174 6574 696d 6553 7472 696e 6743   DatetimeStringC
+00002f70: 6f6e 7665 7274 6572 2061 6e64 2050 726f  onverter and Pro
+00002f80: 746f 6275 6654 696d 6573 7461 6d70 436f  tobufTimestampCo
+00002f90: 6e76 6572 7465 722e 0a23 2054 6865 7920  nverter..# They 
+00002fa0: 616c 6c20 696d 706c 656d 656e 7420 7361  all implement sa
+00002fb0: 6d65 206d 6574 686f 6473 2066 726f 6d20  me methods from 
+00002fc0: 6261 7365 2063 6c61 7373 2e0a 2320 4e6f  base class..# No
+00002fd0: 7465 2074 6861 7420 736f 6d65 2061 6363  te that some acc
+00002fe0: 7572 6163 7920 6d61 7920 6265 206c 6f73  uracy may be los
+00002ff0: 7420 6475 7269 6e67 2063 6f6e 7665 7273  t during convers
+00003000: 696f 6e2e 0a23 2049 6620 666f 7220 6578  ion..# If for ex
+00003010: 616d 706c 6520 796f 7520 7573 6520 746f  ample you use to
+00003020: 5f6d 6963 726f 7365 636f 6e64 7320 6e61  _microseconds na
+00003030: 6e6f 7365 636f 6e64 7320 7769 6c6c 2062  noseconds will b
+00003040: 6520 6375 7420 6f66 6620 696e 7374 6561  e cut off instea
+00003050: 6420 6f66 2072 6f75 6e64 696e 672e 0a0a  d of rounding...
+00003060: 2320 5b32 2e31 5d20 4461 7465 7469 6d65  # [2.1] Datetime
+00003070: 436f 6e76 6572 7465 722e 0a23 2044 6174  Converter..# Dat
+00003080: 6574 696d 6543 6f6e 7665 7274 6572 2074  etimeConverter t
+00003090: 616b 6573 2064 6174 6574 696d 652e 6461  akes datetime.da
+000030a0: 7465 7469 6d65 206f 626a 6563 7420 6173  tetime object as
+000030b0: 2069 6e70 7574 2e0a 0a64 6174 6574 696d   input...datetim
+000030c0: 655f 6f62 6a20 3d20 6461 7465 7469 6d65  e_obj = datetime
+000030d0: 2879 6561 723d 3230 3233 2c20 6d6f 6e74  (year=2023, mont
+000030e0: 683d 312c 2064 6179 3d35 2c20 686f 7572  h=1, day=5, hour
+000030f0: 3d31 342c 206d 696e 7574 653d 3338 2c20  =14, minute=38, 
+00003100: 7365 636f 6e64 3d32 352c 206d 6963 726f  second=25, micro
+00003110: 7365 636f 6e64 3d31 3436 3029 0a0a 2320  second=1460)..# 
+00003120: 4974 2068 6173 206d 6574 686f 6473 2074  It has methods t
+00003130: 6861 7420 7265 7475 726e 2074 6865 2064  hat return the d
+00003140: 6174 6574 696d 6520 696e 2064 6966 6665  atetime in diffe
+00003150: 7265 6e74 2066 6f72 6d61 733a 0a0a 6461  rent formas:..da
+00003160: 7465 5f6d 7320 3d20 4461 7465 7469 6d65  te_ms = Datetime
+00003170: 436f 6e76 6572 7465 722e 746f 5f6d 696c  Converter.to_mil
+00003180: 6c69 7365 636f 6e64 7328 6461 7465 7469  liseconds(dateti
+00003190: 6d65 5f6f 626a 290a 6461 7465 5f75 7320  me_obj).date_us 
+000031a0: 3d20 4461 7465 7469 6d65 436f 6e76 6572  = DatetimeConver
+000031b0: 7465 722e 746f 5f6d 6963 726f 7365 636f  ter.to_microseco
+000031c0: 6e64 7328 6461 7465 7469 6d65 5f6f 626a  nds(datetime_obj
+000031d0: 290a 2320 436f 6e76 6572 7469 6e67 2074  ).# Converting t
+000031e0: 6f20 6e61 6e6f 7365 636f 6e64 7320 6a75  o nanoseconds ju
+000031f0: 7374 7320 6164 6473 2074 6872 6565 2074  sts adds three t
+00003200: 7261 696c 696e 6720 7a65 726f 7320 6173  railing zeros as
+00003210: 2064 6174 6574 696d 6520 6f62 6a65 6374   datetime object
+00003220: 2064 6f65 736e 2774 2068 6176 6520 6e61   doesn't have na
+00003230: 6e6f 7365 636f 6e64 732e 0a64 6174 655f  noseconds..date_
+00003240: 6e73 203d 2044 6174 6574 696d 6543 6f6e  ns = DatetimeCon
+00003250: 7665 7274 6572 2e74 6f5f 6e61 6e6f 7365  verter.to_nanose
+00003260: 636f 6e64 7328 6461 7465 7469 6d65 5f6f  conds(datetime_o
+00003270: 626a 290a 0a23 205b 322e 325d 2044 6174  bj)..# [2.2] Dat
+00003280: 6574 696d 6553 7472 696e 6743 6f6e 7665  etimeStringConve
+00003290: 7274 6572 0a23 2044 6174 6574 696d 6553  rter.# DatetimeS
+000032a0: 7472 696e 6743 6f6e 7665 7274 6572 2074  tringConverter t
+000032b0: 616b 6573 2073 7472 696e 6720 696e 2022  akes string in "
+000032c0: 7979 7979 2d4d 4d2d 6464 5448 483a 6d6d  yyyy-MM-ddTHH:mm
+000032d0: 3a73 735b 2e53 5353 5353 5353 5353 5d5a  :ss[.SSSSSSSSS]Z
+000032e0: 2220 666f 726d 6174 2e0a 0a64 6174 655f  " format...date_
+000032f0: 7374 7269 6e67 203d 2022 3230 3233 2d30  string = "2023-0
+00003300: 312d 3035 5431 343a 3338 3a32 352e 3030  1-05T14:38:25.00
+00003310: 3134 365a 220a 0a23 2057 6520 6861 7665  146Z"..# We have
+00003320: 2073 616d 6520 6d65 7468 6f64 7320 6173   same methods as
+00003330: 2069 6e20 4461 7465 7469 6d65 436f 6e76   in DatetimeConv
+00003340: 6572 7465 720a 6461 7465 5f6d 735f 6672  erter.date_ms_fr
+00003350: 6f6d 5f73 7472 696e 6720 3d20 4461 7465  om_string = Date
+00003360: 7469 6d65 5374 7269 6e67 436f 6e76 6572  timeStringConver
+00003370: 7465 722e 746f 5f6d 696c 6c69 7365 636f  ter.to_milliseco
+00003380: 6e64 7328 6461 7465 5f73 7472 696e 6729  nds(date_string)
+00003390: 0a64 6174 655f 7573 5f66 726f 6d5f 7374  .date_us_from_st
+000033a0: 7269 6e67 203d 2044 6174 6574 696d 6553  ring = DatetimeS
+000033b0: 7472 696e 6743 6f6e 7665 7274 6572 2e74  tringConverter.t
+000033c0: 6f5f 6d69 6372 6f73 6563 6f6e 6473 2864  o_microseconds(d
+000033d0: 6174 655f 7374 7269 6e67 290a 6461 7465  ate_string).date
+000033e0: 5f6e 735f 6672 6f6d 5f73 7472 696e 6720  _ns_from_string 
+000033f0: 3d20 4461 7465 7469 6d65 5374 7269 6e67  = DatetimeString
+00003400: 436f 6e76 6572 7465 722e 746f 5f6e 616e  Converter.to_nan
+00003410: 6f73 6563 6f6e 6473 2864 6174 655f 7374  oseconds(date_st
+00003420: 7269 6e67 290a 0a23 2057 6520 6361 6e20  ring)..# We can 
+00003430: 616c 736f 2067 6574 2064 6174 6574 696d  also get datetim
+00003440: 6520 6f62 6a65 6374 2066 726f 6d20 7374  e object from st
+00003450: 7269 6e67 0a64 6174 6574 696d 655f 6672  ring.datetime_fr
+00003460: 6f6d 5f73 7472 696e 6720 3d20 4461 7465  om_string = Date
+00003470: 7469 6d65 5374 7269 6e67 436f 6e76 6572  timeStringConver
+00003480: 7465 722e 746f 5f64 6174 6574 696d 6528  ter.to_datetime(
+00003490: 6461 7465 5f73 7472 696e 6729 0a0a 2320  date_string)..# 
+000034a0: 5b32 2e33 5d20 5072 6f74 6f62 7566 5469  [2.3] ProtobufTi
+000034b0: 6d65 7374 616d 7043 6f6e 7665 7274 6572  mestampConverter
+000034c0: 0a23 2050 726f 746f 6275 6620 7469 6d65  .# Protobuf time
+000034d0: 7374 616d 7073 206d 7573 7420 6265 2069  stamps must be i
+000034e0: 6e20 666f 726d 207b 2265 706f 6368 5365  n form {"epochSe
+000034f0: 636f 6e64 223a 2073 6563 6f6e 6473 2c20  cond": seconds, 
+00003500: 226e 616e 6f22 3a20 6e61 6e6f 7365 636f  "nano": nanoseco
+00003510: 6e64 737d 0a0a 7072 6f74 6f62 7566 5f74  nds}..protobuf_t
+00003520: 696d 6573 7461 6d70 203d 207b 2265 706f  imestamp = {"epo
+00003530: 6368 5365 636f 6e64 223a 2031 3637 3239  chSecond": 16729
+00003540: 3239 3530 352c 2022 6e61 6e6f 223a 2031  29505, "nano": 1
+00003550: 5f34 3630 5f30 3030 7d0a 0a64 6174 655f  _460_000}..date_
+00003560: 6d73 5f66 726f 6d5f 7469 6d65 7374 616d  ms_from_timestam
+00003570: 7020 3d20 5072 6f74 6f62 7566 5469 6d65  p = ProtobufTime
+00003580: 7374 616d 7043 6f6e 7665 7274 6572 2e74  stampConverter.t
+00003590: 6f5f 6d69 6c6c 6973 6563 6f6e 6473 2870  o_milliseconds(p
+000035a0: 726f 746f 6275 665f 7469 6d65 7374 616d  rotobuf_timestam
+000035b0: 7029 0a64 6174 655f 7573 5f66 726f 6d5f  p).date_us_from_
+000035c0: 7469 6d65 7374 616d 7020 3d20 5072 6f74  timestamp = Prot
+000035d0: 6f62 7566 5469 6d65 7374 616d 7043 6f6e  obufTimestampCon
+000035e0: 7665 7274 6572 2e74 6f5f 6d69 6372 6f73  verter.to_micros
+000035f0: 6563 6f6e 6473 2870 726f 746f 6275 665f  econds(protobuf_
+00003600: 7469 6d65 7374 616d 7029 0a64 6174 655f  timestamp).date_
+00003610: 6e73 5f66 726f 6d5f 7469 6d65 7374 616d  ns_from_timestam
+00003620: 7020 3d20 5072 6f74 6f62 7566 5469 6d65  p = ProtobufTime
+00003630: 7374 616d 7043 6f6e 7665 7274 6572 2e74  stampConverter.t
+00003640: 6f5f 6e61 6e6f 7365 636f 6e64 7328 7072  o_nanoseconds(pr
+00003650: 6f74 6f62 7566 5f74 696d 6573 7461 6d70  otobuf_timestamp
+00003660: 290a 6461 7465 7469 6d65 5f66 726f 6d5f  ).datetime_from_
+00003670: 7469 6d65 7374 616d 7020 3d20 5072 6f74  timestamp = Prot
+00003680: 6f62 7566 5469 6d65 7374 616d 7043 6f6e  obufTimestampCon
+00003690: 7665 7274 6572 2e74 6f5f 6461 7465 7469  verter.to_dateti
+000036a0: 6d65 2870 726f 746f 6275 665f 7469 6d65  me(protobuf_time
+000036b0: 7374 616d 7029 0a0a 2323 2323 2323 2323  stamp)..########
+000036c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000036d0: 2323 2323 2323 2323 2323 2323 2323 0a23  ##############.#
+000036e0: 205b 335d 2057 6f72 6b69 6e67 2077 6974   [3] Working wit
+000036f0: 6820 4576 656e 7454 7265 6520 616e 6420  h EventTree and 
+00003700: 4576 656e 7454 7265 6543 6f6c 6c65 6374  EventTreeCollect
+00003710: 696f 6e2e 0a23 2323 2323 2323 2323 2323  ion..###########
+00003720: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00003730: 2323 2323 2323 2323 2323 230a 2320 4361  ###########.# Ca
+00003740: 6e20 6265 2075 7365 6675 6c20 6966 2079  n be useful if y
+00003750: 6f75 2068 6176 6520 6461 7461 2d73 7472  ou have data-str
+00003760: 6561 6d20 7769 7468 203c 2031 3030 6b20  eam with < 100k 
+00003770: 656c 656d 656e 7473 2c20 6f74 6865 7277  elements, otherw
+00003780: 6973 6520 6974 0a23 2074 616b 6573 2074  ise it.# takes t
+00003790: 6f6f 206d 7563 6820 5241 4d2e 0a0a 2320  oo much RAM...# 
+000037a0: 5b33 2e31 5d20 4275 696c 6420 6120 6375  [3.1] Build a cu
+000037b0: 7374 6f6d 2045 7665 6e74 5472 6565 0a23  stom EventTree.#
+000037c0: 2054 6f20 6372 6561 7465 2061 6e20 4576   To create an Ev
+000037d0: 656e 7454 7265 6520 6f62 6a65 6374 2079  entTree object y
+000037e0: 6f75 206e 6565 6420 746f 2070 726f 7669  ou need to provi
+000037f0: 6465 206e 616d 652c 2069 6420 616e 6420  de name, id and 
+00003800: 6461 7461 206f 6620 7468 6520 726f 6f74  data of the root
+00003810: 2065 7665 6e74 2e0a 7472 6565 203d 2045   event..tree = E
+00003820: 7665 6e74 5472 6565 2865 7665 6e74 5f6e  ventTree(event_n
+00003830: 616d 653d 2272 6f6f 7420 6576 656e 7422  ame="root event"
+00003840: 2c20 6576 656e 745f 6964 3d22 726f 6f74  , event_id="root
+00003850: 5f69 6422 2c20 6461 7461 3d7b 2264 6174  _id", data={"dat
+00003860: 6122 3a20 5b31 2c20 322c 2033 2c20 342c  a": [1, 2, 3, 4,
+00003870: 2035 5d7d 290a 0a23 2054 6f20 6164 6420   5]})..# To add 
+00003880: 6e65 7720 6e6f 6465 2075 7365 2061 7070  new node use app
+00003890: 656e 645f 6576 656e 742e 2070 6172 656e  end_event. paren
+000038a0: 745f 6964 2069 7320 6e65 6365 7373 6172  t_id is necessar
+000038b0: 792c 2064 6174 6120 6973 206f 7074 696f  y, data is optio
+000038c0: 6e61 6c2e 0a74 7265 652e 6170 7065 6e64  nal..tree.append
+000038d0: 5f65 7665 6e74 2865 7665 6e74 5f6e 616d  _event(event_nam
+000038e0: 653d 2241 222c 2065 7665 6e74 5f69 643d  e="A", event_id=
+000038f0: 2241 5f69 6422 2c20 6461 7461 3d4e 6f6e  "A_id", data=Non
+00003900: 652c 2070 6172 656e 745f 6964 3d22 726f  e, parent_id="ro
+00003910: 6f74 5f69 6422 290a 0a23 205b 332e 335d  ot_id")..# [3.3]
+00003920: 2042 7569 6c64 696e 6720 7468 6520 4576   Building the Ev
+00003930: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
+00003940: 6e2e 0a64 6174 615f 736f 7572 6365 3a20  n..data_source: 
+00003950: 4944 6174 6153 6f75 7263 6520 2023 2059  IDataSource  # Y
+00003960: 6f75 2073 686f 756c 6420 696e 6974 2044  ou should init D
+00003970: 6174 6153 6f75 7263 6520 6f62 6a65 6374  ataSource object
+00003980: 2e20 452e 672e 2066 726f 6d20 4c77 4450  . E.g. from LwDP
+00003990: 206d 6f64 756c 652e 0a64 6174 615f 736f   module..data_so
+000039a0: 7572 6365 203d 2044 756d 6d79 4461 7461  urce = DummyData
+000039b0: 536f 7572 6365 2829 2020 2320 4e6f 7465  Source()  # Note
+000039c0: 2120 5765 2075 7365 2066 616b 6520 4453  ! We use fake DS
+000039d0: 2068 6572 652e 0a23 2045 5443 4472 6976   here..# ETCDriv
+000039e0: 6572 2068 6572 6520 6973 2061 2073 7475  er here is a stu
+000039f0: 622c 2061 6374 7561 6c6c 7920 7468 6520  b, actually the 
+00003a00: 6c69 6220 646f 6573 6e27 7420 6861 7665  lib doesn't have
+00003a10: 2073 7563 6820 6120 636c 6173 732e 0a23   such a class..#
+00003a20: 2059 6f75 2063 616e 2074 616b 6520 6974   You can take it
+00003a30: 2069 6e20 4c77 4450 206d 6f64 756c 6520   in LwDP module 
+00003a40: 6f72 2063 7265 6174 6520 796f 7572 7365  or create yourse
+00003a50: 6c66 2063 6c61 7373 2069 6620 796f 7520  lf class if you 
+00003a60: 6861 7665 2073 6f6d 6520 7370 6563 6961  have some specia
+00003a70: 6c20 6576 656e 7473 2073 7472 7563 7475  l events structu
+00003a80: 7265 2e0a 6672 6f6d 2074 6832 5f64 6174  re..from th2_dat
+00003a90: 615f 7365 7276 6963 6573 2e64 6174 615f  a_services.data_
+00003aa0: 736f 7572 6365 2e6c 7764 702e 6576 656e  source.lwdp.even
+00003ab0: 745f 7472 6565 2069 6d70 6f72 7420 4874  t_tree import Ht
+00003ac0: 7470 4554 4344 7269 7665 7220 6173 2045  tpETCDriver as E
+00003ad0: 5443 4472 6976 6572 0a0a 2320 4966 2079  TCDriver..# If y
+00003ae0: 6f75 2064 6f6e 2774 2073 7065 6369 6679  ou don't specify
+00003af0: 2064 6174 615f 736f 7572 6365 2066 6f72   data_source for
+00003b00: 2074 6865 2064 7269 7665 7220 7468 656e   the driver then
+00003b10: 2069 7420 776f 6e27 7420 7265 636f 7665   it won't recove
+00003b20: 7220 6465 7461 6368 6564 2065 7665 6e74  r detached event
+00003b30: 732e 0a64 7269 7665 723a 2049 4554 4344  s..driver: IETCD
+00003b40: 7269 7665 7220 2023 2059 6f75 2073 686f  river  # You sho
+00003b50: 756c 6420 696e 6974 2045 5443 4472 6976  uld init ETCDriv
+00003b60: 6572 206f 626a 6563 742e 2045 2e67 2e20  er object. E.g. 
+00003b70: 6672 6f6d 204c 7744 5020 6d6f 6475 6c65  from LwDP module
+00003b80: 206f 7220 796f 7572 2063 7573 746f 6d20   or your custom 
+00003b90: 636c 6173 732e 0a64 7269 7665 7220 3d20  class..driver = 
+00003ba0: 4554 4344 7269 7665 7228 6461 7461 5f73  ETCDriver(data_s
+00003bb0: 6f75 7263 653d 6461 7461 5f73 6f75 7263  ource=data_sourc
+00003bc0: 652c 2075 7365 5f73 7475 623d 5472 7565  e, use_stub=True
+00003bd0: 290a 0a65 7463 203d 2045 7665 6e74 5472  )..etc = EventTr
+00003be0: 6565 436f 6c6c 6563 7469 6f6e 2864 7269  eeCollection(dri
+00003bf0: 7665 7229 0a65 7463 2e62 7569 6c64 2865  ver).etc.build(e
+00003c00: 7665 6e74 7329 0a65 7463 2e73 686f 7728  vents).etc.show(
+00003c10: 290a 2320 4974 276c 6c20 7072 696e 7420  ).# It'll print 
+00003c20: 7468 6520 666f 6c6c 6f77 696e 673a 0a23  the following:.#
+00003c30: 2053 6574 206f 6620 6175 746f 2d67 656e   Set of auto-gen
+00003c40: 6572 6174 6564 2065 7665 6e74 7320 666f  erated events fo
+00003c50: 7220 6473 206c 6962 2074 6573 7469 6e67  r ds lib testing
+00003c60: 0a23 20e2 949c e294 80e2 9480 2050 6c61  .# ......... Pla
+00003c70: 696e 2065 7665 6e74 2031 0a23 20e2 9494  in event 1.# ...
+00003c80: e294 80e2 9480 2050 6c61 696e 2065 7665  ...... Plain eve
+00003c90: 6e74 2032 0a0a 7072 696e 7428 6574 6329  nt 2..print(etc)
+00003ca0: 0a23 2045 7665 6e74 5472 6565 436f 6c6c  .# EventTreeColl
+00003cb0: 6563 7469 6f6e 2874 7265 6573 3d31 2c20  ection(trees=1, 
+00003cc0: 6576 656e 7473 3d33 5b74 7265 6573 3d33  events=3[trees=3
+00003cd0: 2c20 6465 7461 6368 6564 3d30 5d29 0a0a  , detached=0])..
+00003ce0: 2320 4465 7461 6368 6564 2065 7665 6e74  # Detached event
+00003cf0: 7320 6973 6e27 7420 656d 7074 792e 0a61  s isn't empty..a
+00003d00: 7373 6572 7420 6574 632e 6765 745f 6465  ssert etc.get_de
+00003d10: 7461 6368 6564 5f65 7665 6e74 7328 2920  tached_events() 
+00003d20: 2023 2072 6574 7572 6e73 206c 6973 7420   # returns list 
+00003d30: 6f66 2064 6574 6163 6865 645f 6576 656e  of detached_even
+00003d40: 7473 2e0a 0a23 2072 6563 6f76 6572 5f75  ts...# recover_u
+00003d50: 6e6b 6e6f 776e 5f65 7665 6e74 7320 2d2d  nknown_events --
+00003d60: 2075 7365 6420 746f 2072 6563 6f76 6572   used to recover
+00003d70: 2073 6f6d 6520 6576 656e 7473 2070 6172   some events par
+00003d80: 656e 7473 2e0a 2320 5468 6174 2077 6f6e  ents..# That won
+00003d90: 2774 2077 6f72 6b20 7769 7468 2044 756d  't work with Dum
+00003da0: 6d79 4461 7461 536f 7572 6365 2c20 736f  myDataSource, so
+00003db0: 2077 6173 2063 6f6d 6d65 6e74 6564 0a23   was commented.#
+00003dc0: 2065 7463 2e72 6563 6f76 6572 5f75 6e6b   etc.recover_unk
+00003dd0: 6e6f 776e 5f65 7665 6e74 7328 290a 0a23  nown_events()..#
+00003de0: 2041 6674 6572 2074 6861 7420 7468 6520   After that the 
+00003df0: 6465 7461 6368 6564 2065 7665 6e74 7320  detached events 
+00003e00: 7368 6f75 6c64 2062 6520 656d 7074 7920  should be empty 
+00003e10: 6265 6361 7573 6520 7468 6579 2077 6572  because they wer
+00003e20: 6520 7265 636f 7665 7265 642e 0a23 2061  e recovered..# a
+00003e30: 7373 6572 7420 6e6f 7420 6574 632e 6765  ssert not etc.ge
+00003e40: 745f 6465 7461 6368 6564 5f65 7665 6e74  t_detached_event
+00003e50: 7328 290a 0a23 202d 2d2d 2d2d 0a0a 2320  s()..# -----..# 
+00003e60: 5468 6520 636f 6c6c 6563 7469 6f6e 2068  The collection h
+00003e70: 6173 2045 7665 6e74 5472 6565 7320 6561  as EventTrees ea
+00003e80: 6368 2077 6974 6820 6120 7472 6565 206f  ch with a tree o
+00003e90: 6620 6576 656e 7473 2e0a 2320 5573 696e  f events..# Usin
+00003ea0: 6720 436f 6c6c 6563 7469 6f6e 2061 6e64  g Collection and
+00003eb0: 2045 7665 6e74 5472 6565 732c 2079 6f75   EventTrees, you
+00003ec0: 2063 616e 2077 6f72 6b20 666c 6578 6962   can work flexib
+00003ed0: 6c79 2077 6974 6820 6576 656e 7473 2e0a  ly with events..
+00003ee0: 0a23 205b 332e 332e 315d 2047 6574 206c  .# [3.3.1] Get l
+00003ef0: 6561 7665 7320 6f66 2061 6c6c 2074 7265  eaves of all tre
+00003f00: 6573 2e0a 6c65 6176 6573 3a20 5475 706c  es..leaves: Tupl
+00003f10: 655b 6469 6374 5d20 3d20 6574 632e 6765  e[dict] = etc.ge
+00003f20: 745f 6c65 6176 6573 2829 2020 2320 5265  t_leaves()  # Re
+00003f30: 7475 726e 7320 6120 7475 706c 6520 6f66  turns a tuple of
+00003f40: 206c 6561 7665 7320 6576 656e 7473 0a0a   leaves events..
+00003f50: 2320 5b33 2e33 2e32 5d20 4765 7420 726f  # [3.3.2] Get ro
+00003f60: 6f74 7320 6964 7320 6f66 2061 6c6c 2074  ots ids of all t
+00003f70: 7265 6573 2e0a 726f 6f74 733a 204c 6973  rees..roots: Lis
+00003f80: 745b 7374 725d 203d 2065 7463 2e67 6574  t[str] = etc.get
+00003f90: 5f72 6f6f 7473 5f69 6473 2829 0a23 2052  _roots_ids().# R
+00003fa0: 6574 7572 6e73 2074 6865 206c 6973 7420  eturns the list 
+00003fb0: 6f66 2072 6f6f 7420 4964 733a 0a23 205b  of root Ids:.# [
+00003fc0: 2764 656d 6f5f 626f 6f6b 5f31 3a74 6832  'demo_book_1:th2
+00003fd0: 2d73 636f 7065 3a32 3032 3330 3130 3531  -scope:202301051
+00003fe0: 3335 3730 3535 3630 3837 3330 3030 3a64  35705560873000:d
+00003ff0: 3631 6539 3330 612d 3864 3030 2d31 3165  61e930a-8d00-11e
+00004000: 642d 6161 3161 2d64 3334 6136 3135 3531  d-aa1a-d34a61551
+00004010: 3532 645f 3127 5d0a 0a23 205b 332e 332e  52d_1']..# [3.3.
+00004020: 335d 2046 696e 6420 616e 2065 7665 6e74  3] Find an event
+00004030: 2069 6e20 616c 6c20 7472 6565 732e 0a66   in all trees..f
+00004040: 696e 645f 6576 656e 743a 204f 7074 696f  ind_event: Optio
+00004050: 6e61 6c5b 6469 6374 5d20 3d20 6574 632e  nal[dict] = etc.
+00004060: 6669 6e64 286c 616d 6264 6120 6576 656e  find(lambda even
+00004070: 743a 2022 5365 6e64 206d 6573 7361 6765  t: "Send message
+00004080: 2220 696e 2065 7665 6e74 5b22 6576 656e  " in event["even
+00004090: 7454 7970 6522 5d29 0a0a 2320 5b33 2e33  tType"])..# [3.3
+000040a0: 2e34 5d20 4669 6e64 2061 6c6c 2065 7665  .4] Find all eve
+000040b0: 6e74 7320 696e 2061 6c6c 2074 7265 6573  nts in all trees
+000040c0: 2e20 5468 6572 6520 6973 2061 6c73 6f20  . There is also 
+000040d0: 6974 6572 6162 6c65 2076 6572 7369 6f6e  iterable version
+000040e0: 2027 6669 6e64 616c 6c5f 6974 6572 272e   'findall_iter'.
+000040f0: 0a66 696e 645f 6576 656e 7473 3a20 4c69  .find_events: Li
+00004100: 7374 5b64 6963 745d 203d 2065 7463 2e66  st[dict] = etc.f
+00004110: 696e 6461 6c6c 286c 616d 6264 6120 6576  indall(lambda ev
+00004120: 656e 743a 2065 7665 6e74 5b22 7375 6363  ent: event["succ
+00004130: 6573 7366 756c 225d 2069 7320 5472 7565  essful"] is True
+00004140: 290a 0a23 205b 332e 332e 355d 2046 696e  )..# [3.3.5] Fin
+00004150: 6420 616e 2061 6e63 6573 746f 7220 6f66  d an ancestor of
+00004160: 2074 6865 2065 7665 6e74 2e0a 616e 6365   the event..ance
+00004170: 7374 6f72 3a20 4f70 7469 6f6e 616c 5b64  stor: Optional[d
+00004180: 6963 745d 203d 2065 7463 2e66 696e 645f  ict] = etc.find_
+00004190: 616e 6365 7374 6f72 280a 2020 2020 2264  ancestor(.    "d
+000041a0: 656d 6f5f 626f 6f6b 5f31 3a74 6832 2d73  emo_book_1:th2-s
+000041b0: 636f 7065 3a32 3032 3330 3130 3531 3335  cope:20230105135
+000041c0: 3730 3535 3630 3837 3330 3030 3a64 3631  705560873000:d61
+000041d0: 6539 3330 612d 3864 3030 2d31 3165 642d  e930a-8d00-11ed-
+000041e0: 6161 3161 2d64 3334 6136 3135 3531 3532  aa1a-d34a6155152
+000041f0: 645f 3122 2c0a 2020 2020 6669 6c74 6572  d_1",.    filter
+00004200: 3d6c 616d 6264 6120 6576 656e 743a 2022  =lambda event: "
+00004210: 526f 6f74 4576 656e 7422 2069 6e20 6576  RootEvent" in ev
+00004220: 656e 745b 2265 7665 6e74 4e61 6d65 225d  ent["eventName"]
+00004230: 2c0a 290a 0a23 205b 332e 332e 365d 2047  ,.)..# [3.3.6] G
+00004240: 6574 2063 6869 6c64 7265 6e20 6f66 2074  et children of t
+00004250: 6865 2065 7665 6e74 2e20 5468 6572 6520  he event. There 
+00004260: 6973 2061 6c73 6f20 6974 6572 6162 6c65  is also iterable
+00004270: 2076 6572 7369 6f6e 2027 6765 745f 6368   version 'get_ch
+00004280: 696c 6472 656e 5f69 7465 7227 2e0a 6368  ildren_iter'..ch
+00004290: 696c 6472 656e 3a20 5475 706c 655b 6469  ildren: Tuple[di
+000042a0: 6374 5d20 3d20 6574 632e 6765 745f 6368  ct] = etc.get_ch
+000042b0: 696c 6472 656e 280a 2020 2020 2264 656d  ildren(.    "dem
+000042c0: 6f5f 626f 6f6b 5f31 3a74 6832 2d73 636f  o_book_1:th2-sco
+000042d0: 7065 3a32 3032 3330 3130 3531 3335 3730  pe:2023010513570
+000042e0: 3535 3630 3837 3330 3030 3a64 3631 6539  5560873000:d61e9
+000042f0: 3330 612d 3864 3030 2d31 3165 642d 6161  30a-8d00-11ed-aa
+00004300: 3161 2d64 3334 6136 3135 3531 3532 645f  1a-d34a6155152d_
+00004310: 3122 0a29 0a0a 2320 5b33 2e33 2e37 5d20  1".)..# [3.3.7] 
+00004320: 4765 7420 7375 6274 7265 6520 666f 7220  Get subtree for 
+00004330: 7370 6563 6966 6965 6420 6576 656e 742e  specified event.
+00004340: 0a73 7562 7472 6565 3a20 4576 656e 7454  .subtree: EventT
+00004350: 7265 6520 3d20 6574 632e 6765 745f 7375  ree = etc.get_su
+00004360: 6274 7265 6528 0a20 2020 2022 6465 6d6f  btree(.    "demo
+00004370: 5f62 6f6f 6b5f 313a 7468 322d 7363 6f70  _book_1:th2-scop
+00004380: 653a 3230 3233 3031 3035 3133 3537 3035  e:20230105135705
+00004390: 3536 3038 3733 3030 303a 6436 3165 3933  560873000:d61e93
+000043a0: 3061 2d38 6430 302d 3131 6564 2d61 6131  0a-8d00-11ed-aa1
+000043b0: 612d 6433 3461 3631 3535 3135 3264 5f31  a-d34a6155152d_1
+000043c0: 220a 290a 0a23 205b 332e 332e 385d 2047  ".)..# [3.3.8] G
+000043d0: 6574 2066 756c 6c20 7061 7468 2074 6f20  et full path to 
+000043e0: 7468 6520 6576 656e 742e 0a23 204c 6f6f  the event..# Loo
+000043f0: 6b73 206c 696b 6520 5b61 6e63 6573 746f  ks like [ancesto
+00004400: 725f 726f 6f74 2c20 616e 6365 7374 6f72  r_root, ancestor
+00004410: 5f6c 6576 656c 312c 2061 6e63 6573 746f  _level1, ancesto
+00004420: 725f 6c65 7665 6c32 2c20 6576 656e 745d  r_level2, event]
+00004430: 0a65 7665 6e74 5f70 6174 683a 204c 6973  .event_path: Lis
+00004440: 745b 6469 6374 5d20 3d20 6574 632e 6765  t[dict] = etc.ge
+00004450: 745f 6675 6c6c 5f70 6174 6828 0a20 2020  t_full_path(.   
+00004460: 2022 6465 6d6f 5f62 6f6f 6b5f 313a 7468   "demo_book_1:th
+00004470: 322d 7363 6f70 653a 3230 3233 3031 3035  2-scope:20230105
+00004480: 3133 3537 3035 3536 3038 3733 3030 303a  135705560873000:
+00004490: 6436 3165 3933 3061 2d38 6430 302d 3131  d61e930a-8d00-11
+000044a0: 6564 2d61 6131 612d 6433 3461 3631 3535  ed-aa1a-d34a6155
+000044b0: 3135 3264 5f31 220a 290a 0a23 205b 332e  152d_1".)..# [3.
+000044c0: 332e 395d 2047 6574 2070 6172 656e 7420  3.9] Get parent 
+000044d0: 6f66 2074 6865 2065 7665 6e74 2e0a 7061  of the event..pa
+000044e0: 7265 6e74 203d 2065 7463 2e67 6574 5f70  rent = etc.get_p
+000044f0: 6172 656e 7428 0a20 2020 2022 6465 6d6f  arent(.    "demo
+00004500: 5f62 6f6f 6b5f 313a 7468 322d 7363 6f70  _book_1:th2-scop
+00004510: 653a 3230 3233 3031 3035 3133 3537 3035  e:20230105135705
+00004520: 3536 3038 3733 3030 303a 6436 3165 3933  560873000:d61e93
+00004530: 3061 2d38 6430 302d 3131 6564 2d61 6131  0a-8d00-11ed-aa1
+00004540: 612d 6433 3461 3631 3535 3135 3264 5f31  a-d34a6155152d_1
+00004550: 220a 290a 0a23 205b 332e 332e 3130 5d20  ".)..# [3.3.10] 
+00004560: 4170 7065 6e64 206e 6577 2065 7665 6e74  Append new event
+00004570: 2074 6f20 7468 6520 636f 6c6c 6563 7469   to the collecti
+00004580: 6f6e 2e0a 6574 632e 6170 7065 6e64 5f65  on..etc.append_e
+00004590: 7665 6e74 280a 2020 2020 6576 656e 743d  vent(.    event=
+000045a0: 7b0a 2020 2020 2020 2020 2265 7665 6e74  {.        "event
+000045b0: 4964 223a 2022 6132 3066 3565 6634 2d63  Id": "a20f5ef4-c
+000045c0: 3366 652d 6262 3130 2d61 3239 632d 6464  3fe-bb10-a29c-dd
+000045d0: 3364 3738 3439 3039 6562 222c 0a20 2020  3d784909eb",.   
+000045e0: 2020 2020 2022 7061 7265 6e74 4576 656e       "parentEven
+000045f0: 7449 6422 3a20 2238 6532 3532 3466 612d  tId": "8e2524fa-
+00004600: 6366 3539 2d31 3165 622d 6133 6637 2d30  cf59-11eb-a3f7-0
+00004610: 3934 6639 3034 6333 6136 3222 2c0a 2020  94f904c3a62",.  
+00004620: 2020 2020 2020 2265 7665 6e74 4e61 6d65        "eventName
+00004630: 223a 2022 5374 7562 4576 656e 7422 2c0a  ": "StubEvent",.
+00004640: 2020 2020 7d0a 290a 0a23 205b 332e 332e      }.)..# [3.3.
+00004650: 3131 5d20 5368 6f77 2074 6865 2065 6e74  11] Show the ent
+00004660: 6972 6520 636f 6c6c 6563 7469 6f6e 2e0a  ire collection..
+00004670: 6574 632e 7368 6f77 2829 0a23 2049 7427  etc.show().# It'
+00004680: 6c6c 2070 7269 6e74 2074 6865 2066 6f6c  ll print the fol
+00004690: 6c6f 7769 6e67 3a0a 2320 5365 7420 6f66  lowing:.# Set of
+000046a0: 2061 7574 6f2d 6765 6e65 7261 7465 6420   auto-generated 
+000046b0: 6576 656e 7473 2066 6f72 2064 7320 6c69  events for ds li
+000046c0: 6220 7465 7374 696e 670a 2320 e294 9ce2  b testing.# ....
+000046d0: 9480 e294 8020 506c 6169 6e20 6576 656e  ..... Plain even
+000046e0: 7420 310a 2320 e294 94e2 9480 e294 8020  t 1.# ......... 
+000046f0: 506c 6169 6e20 6576 656e 7420 320a 0a23  Plain event 2..#
+00004700: 2041 7320 796f 7520 6361 6e20 7365 652c   As you can see,
+00004710: 206e 6f74 6869 6e67 2077 6173 2063 6861   nothing was cha
+00004720: 6e67 6564 2c20 6275 7420 7765 2061 6464  nged, but we add
+00004730: 6564 2074 6865 206e 6577 2065 7665 6e74  ed the new event
+00004740: 210a 2320 6c65 7427 7320 6c6f 6f6b 2061  !.# let's look a
+00004750: 7420 7468 6520 7375 6d6d 6172 792e 0a0a  t the summary...
+00004760: 7072 696e 7428 6574 632e 7375 6d6d 6172  print(etc.summar
+00004770: 7928 2929 2020 2320 7468 6520 7361 6d65  y())  # the same
+00004780: 2061 7320 6a75 7374 2070 7269 6e74 2865   as just print(e
+00004790: 7463 290a 2320 4576 656e 7454 7265 6543  tc).# EventTreeC
+000047a0: 6f6c 6c65 6374 696f 6e28 7472 6565 733d  ollection(trees=
+000047b0: 312c 2065 7665 6e74 733d 355b 7472 6565  1, events=5[tree
+000047c0: 733d 332c 2064 6574 6163 6865 643d 325d  s=3, detached=2]
+000047d0: 290a 2320 596f 7520 6361 6e20 7365 6520  ).# You can see 
+000047e0: 7468 6174 2069 7420 7761 7320 6164 6465  that it was adde
+000047f0: 6420 746f 2064 6574 6163 6865 642e 2054  d to detached. T
+00004800: 6861 7427 7320 7768 7920 796f 7520 646f  hat's why you do
+00004810: 6e27 7420 7365 6520 7468 6520 6576 656e  n't see the even
+00004820: 740a 2320 7669 6120 6073 686f 7728 2960  t.# via `show()`
+00004830: 2e20 6073 686f 7728 2960 2070 7269 6e74  . `show()` print
+00004840: 7320 6f6e 6c79 2054 7265 6573 210a 2320  s only Trees!.# 
+00004850: 5573 6520 6065 7463 2e67 6574 5f70 6172  Use `etc.get_par
+00004860: 656e 746c 6573 735f 7472 6565 7328 2960  entless_trees()`
+00004870: 2074 6f20 636f 6e76 6572 7420 6465 7461   to convert deta
+00004880: 6368 6564 2065 7665 6e74 7320 746f 2074  ched events to t
+00004890: 7265 6573 2e0a 2320 4d6f 7265 2069 6e66  rees..# More inf
+000048a0: 6f72 6d61 7469 6f6e 2062 656c 6f77 2069  ormation below i
+000048b0: 6e20 7468 6520 636f 7272 6573 706f 6e64  n the correspond
+000048c0: 696e 6720 7365 6374 696f 6e2e 0a0a 2320  ing section...# 
+000048d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a23  --------------.#
+000048e0: 205b 332e 345d 2057 6f72 6b69 6e67 2077   [3.4] Working w
+000048f0: 6974 6820 7468 6520 4576 656e 7454 7265  ith the EventTre
+00004900: 652e 0a23 2045 7665 6e74 5472 6565 2068  e..# EventTree h
+00004910: 6173 2074 6865 2073 616d 6520 6d65 7468  as the same meth
+00004920: 6f64 7320 6173 2045 7665 6e74 5472 6565  ods as EventTree
+00004930: 436f 6c6c 6563 7469 6f6e 2c20 6275 7420  Collection, but 
+00004940: 6f6e 6c79 2066 6f72 2069 7473 206f 776e  only for its own
+00004950: 2074 7265 652e 0a0a 2320 5b33 2e34 2e31   tree...# [3.4.1
+00004960: 5d20 4765 7420 6120 636f 6c6c 6563 7469  ] Get a collecti
+00004970: 6f6e 206f 6620 7472 6565 732e 0a74 7265  on of trees..tre
+00004980: 6573 3a20 4c69 7374 5b45 7665 6e74 5472  es: List[EventTr
+00004990: 6565 5d20 3d20 6574 632e 6765 745f 7472  ee] = etc.get_tr
+000049a0: 6565 7328 290a 7472 6565 3a20 4576 656e  ees().tree: Even
+000049b0: 7454 7265 6520 3d20 7472 6565 735b 305d  tTree = trees[0]
+000049c0: 0a0a 2320 4275 7420 4576 656e 7454 7265  ..# But EventTre
+000049d0: 6520 7072 6f76 6964 6573 2061 2077 6f72  e provides a wor
+000049e0: 6b20 7769 7468 2074 6865 2074 7265 652c  k with the tree,
+000049f0: 2062 7574 2064 6f65 7320 6e6f 7420 6d6f   but does not mo
+00004a00: 6469 6679 2069 742e 0a23 2049 6620 796f  dify it..# If yo
+00004a10: 7520 7761 6e74 2074 6f20 6d6f 6469 6679  u want to modify
+00004a20: 2074 6865 2074 7265 652c 2075 7365 2045   the tree, use E
+00004a30: 7665 6e74 5472 6565 436f 6c6c 6563 7469  ventTreeCollecti
+00004a40: 6f6e 732e 0a0a 2320 5b33 2e35 5d20 576f  ons...# [3.5] Wo
+00004a50: 726b 696e 6720 7769 7468 2050 6172 656e  rking with Paren
+00004a60: 746c 6573 7354 7265 652e 0a23 2050 6172  tlessTree..# Par
+00004a70: 656e 746c 6573 7354 7265 6520 6973 2061  entlessTree is a
+00004a80: 6e20 4576 656e 7454 7265 6520 7468 6174  n EventTree that
+00004a90: 2068 6173 2064 6574 6163 6865 6420 6576   has detached ev
+00004aa0: 656e 7473 2077 6974 6820 7374 7562 732e  ents with stubs.
+00004ab0: 0a70 6172 656e 746c 6573 735f 7472 6565  .parentless_tree
+00004ac0: 733a 204c 6973 745b 4576 656e 7454 7265  s: List[EventTre
+00004ad0: 655d 203d 2065 7463 2e67 6574 5f70 6172  e] = etc.get_par
+00004ae0: 656e 746c 6573 735f 7472 6565 7328 290a  entless_trees().
+00004af0: 7072 696e 7428 2270 6172 656e 746c 6573  print("parentles
+00004b00: 735f 7472 6565 7320 636f 6e74 6169 6e73  s_trees contains
+00004b10: 3a22 290a 7072 696e 7428 7061 7265 6e74  :").print(parent
+00004b20: 6c65 7373 5f74 7265 6573 290a 2320 5b45  less_trees).# [E
+00004b30: 7665 6e74 5472 6565 286e 616d 653d 273c  ventTree(name='<
+00004b40: 4272 6f6b 656e 4576 656e 743e 272c 2072  BrokenEvent>', r
+00004b50: 6f6f 745f 6964 3d27 6e6f 745f 6578 6973  oot_id='not_exis
+00004b60: 7473 5f69 6e5f 7468 655f 6576 656e 7473  ts_in_the_events
+00004b70: 5f73 7472 6561 6d27 2c20 6576 656e 7473  _stream', events
+00004b80: 3d32 292c 0a23 2020 4576 656e 7454 7265  =2),.#  EventTre
+00004b90: 6528 6e61 6d65 3d27 3c42 726f 6b65 6e45  e(name='<BrokenE
+00004ba0: 7665 6e74 3e27 2c20 726f 6f74 5f69 643d  vent>', root_id=
+00004bb0: 2738 6532 3532 3466 612d 6366 3539 2d31  '8e2524fa-cf59-1
+00004bc0: 3165 622d 6133 6637 2d30 3934 6639 3034  1eb-a3f7-094f904
+00004bd0: 6333 6136 3227 2c20 6576 656e 7473 3d32  c3a62', events=2
+00004be0: 295d 0a0a 7072 696e 7428 225c 6e22 2022  )]..print("\n" "
+00004bf0: 6574 6320 6166 7465 7220 6067 6574 5f70  etc after `get_p
+00004c00: 6172 656e 746c 6573 735f 7472 6565 7360  arentless_trees`
+00004c10: 3a22 290a 7072 696e 7428 6574 632e 7375  :").print(etc.su
+00004c20: 6d6d 6172 7928 2929 0a23 2045 7665 6e74  mmary()).# Event
+00004c30: 5472 6565 436f 6c6c 6563 7469 6f6e 2874  TreeCollection(t
+00004c40: 7265 6573 3d33 5b72 6567 756c 6172 3d31  rees=3[regular=1
+00004c50: 2c20 7061 7265 6e74 6c65 7373 3d32 5d2c  , parentless=2],
+00004c60: 2065 7665 6e74 733d 375b 7472 6565 733d   events=7[trees=
+00004c70: 372c 2064 6574 6163 6865 643d 305d 2927  7, detached=0])'
+00004c80: 0a65 7463 2e73 686f 7728 290a 2320 5365  .etc.show().# Se
+00004c90: 7420 6f66 2061 7574 6f2d 6765 6e65 7261  t of auto-genera
+00004ca0: 7465 6420 6576 656e 7473 2066 6f72 2064  ted events for d
+00004cb0: 7320 6c69 6220 7465 7374 696e 670a 2320  s lib testing.# 
+00004cc0: e294 9ce2 9480 e294 8020 506c 6169 6e20  ......... Plain 
+00004cd0: 6576 656e 7420 310a 2320 e294 94e2 9480  event 1.# ......
+00004ce0: e294 8020 506c 6169 6e20 6576 656e 7420  ... Plain event 
+00004cf0: 320a 2320 3c42 726f 6b65 6e45 7665 6e74  2.# <BrokenEvent
+00004d00: 3e0a 2320 e294 94e2 9480 e294 8020 4661  >.# ......... Fa
+00004d10: 6b65 2065 7665 6e74 0a23 203c 4272 6f6b  ke event.# <Brok
+00004d20: 656e 4576 656e 743e 0a23 20e2 9494 e294  enEvent>.# .....
+00004d30: 80e2 9480 2053 7475 6245 7665 6e74 2020  .... StubEvent  
+00004d40: 2020 3c2d 2d2d 2074 6865 2065 7665 6e74    <--- the event
+00004d50: 2074 6861 7420 7761 7320 6164 6465 6420   that was added 
+00004d60: 6162 6f76 650a 0a23 205b 332e 365d 2057  above..# [3.6] W
+00004d70: 6f72 6b69 6e67 2077 6974 6820 5061 7265  orking with Pare
+00004d80: 6e74 4576 656e 7454 7265 6543 6f6c 6c65  ntEventTreeColle
+00004d90: 6374 696f 6e2e 0a23 2050 6172 656e 7445  ction..# ParentE
+00004da0: 7665 6e74 5472 6565 436f 6c6c 6563 7469  ventTreeCollecti
+00004db0: 6f6e 2069 7320 6120 7472 6565 2063 6f6c  on is a tree col
+00004dc0: 6c65 6374 696f 6e20 6c69 6b65 2045 7665  lection like Eve
+00004dd0: 6e74 5472 6565 436f 6c6c 6563 7469 6f6e  ntTreeCollection
+00004de0: 2c0a 2320 6275 7420 6974 2068 6173 206f  ,.# but it has o
+00004df0: 6e6c 7920 6576 656e 7473 2074 6861 7420  nly events that 
+00004e00: 6861 7665 2072 6566 6572 656e 6365 732e  have references.
+00004e10: 0a64 6174 615f 736f 7572 6365 3a20 4944  .data_source: ID
+00004e20: 6174 6153 6f75 7263 6520 2023 2059 6f75  ataSource  # You
+00004e30: 2073 686f 756c 6420 696e 6974 2044 6174   should init Dat
+00004e40: 6153 6f75 7263 6520 6f62 6a65 6374 2e20  aSource object. 
+00004e50: 452e 672e 2066 726f 6d20 4c77 4450 206d  E.g. from LwDP m
+00004e60: 6f64 756c 652e 0a64 6174 615f 736f 7572  odule..data_sour
+00004e70: 6365 203d 2044 756d 6d79 4461 7461 536f  ce = DummyDataSo
+00004e80: 7572 6365 2829 2020 2320 4e6f 7465 2120  urce()  # Note! 
+00004e90: 5765 2075 7365 2066 616b 6520 4453 2068  We use fake DS h
+00004ea0: 6572 652e 0a23 2045 5443 4472 6976 6572  ere..# ETCDriver
+00004eb0: 2068 6572 6520 6973 2061 2073 7475 622c   here is a stub,
+00004ec0: 2061 6374 7561 6c6c 7920 7468 6520 6c69   actually the li
+00004ed0: 6220 646f 6573 6e27 7420 6861 7665 2073  b doesn't have s
+00004ee0: 7563 6820 6120 636c 6173 732e 0a23 2059  uch a class..# Y
+00004ef0: 6f75 2063 616e 2074 616b 6520 6974 2069  ou can take it i
+00004f00: 6e20 4c77 4450 206d 6f64 756c 6520 6f72  n LwDP module or
+00004f10: 2063 7265 6174 6520 796f 7572 7365 6c66   create yourself
+00004f20: 2063 6c61 7373 2069 6620 796f 7520 6861   class if you ha
+00004f30: 7665 2073 6f6d 6520 7370 6563 6961 6c20  ve some special 
+00004f40: 6576 656e 7473 2073 7472 7563 7475 7265  events structure
+00004f50: 2e0a 6672 6f6d 2074 6832 5f64 6174 615f  ..from th2_data_
+00004f60: 7365 7276 6963 6573 2e64 6174 615f 736f  services.data_so
+00004f70: 7572 6365 2e6c 7764 702e 6576 656e 745f  urce.lwdp.event_
+00004f80: 7472 6565 2069 6d70 6f72 7420 4874 7470  tree import Http
+00004f90: 4554 4344 7269 7665 7220 6173 2045 5443  ETCDriver as ETC
+00004fa0: 4472 6976 6572 0a0a 6472 6976 6572 203d  Driver..driver =
+00004fb0: 2045 5443 4472 6976 6572 2864 6174 615f   ETCDriver(data_
+00004fc0: 736f 7572 6365 3d64 6174 615f 736f 7572  source=data_sour
+00004fd0: 6365 290a 7065 7463 203d 2050 6172 656e  ce).petc = Paren
+00004fe0: 7445 7665 6e74 5472 6565 436f 6c6c 6563  tEventTreeCollec
+00004ff0: 7469 6f6e 2864 7269 7665 7229 0a70 6574  tion(driver).pet
+00005000: 632e 6275 696c 6428 6576 656e 7473 290a  c.build(events).
+00005010: 0a70 6574 632e 7368 6f77 2829 0a70 6574  .petc.show().pet
+00005020: 632e 7375 6d6d 6172 7928 290a 0a23 2323  c.summary()..###
+00005030: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00005040: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00005050: 2323 230a 2320 5b34 5d20 4669 656c 6420  ###.# [4] Field 
+00005060: 5265 736f 6c76 6572 730a 2323 2323 2323  Resolvers.######
+00005070: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00005080: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00005090: 0a23 2050 6c65 6173 6520 7265 6164 2060  .# Please read `
+000050a0: 4669 656c 6420 5265 736f 6c76 6572 7360  Field Resolvers`
+000050b0: 2062 6c6f 636b 2069 6e20 7265 6164 6d65   block in readme
+000050c0: 2066 6972 7374 2e0a 0a23 205b 342e 315d   first...# [4.1]
+000050d0: 2055 7361 6765 2065 7861 6d70 6c65 2066   Usage example f
+000050e0: 726f 6d20 636c 6965 6e74 2063 6f64 650a  rom client code.
+000050f0: 6672 6f6d 2074 6832 5f64 6174 615f 7365  from th2_data_se
+00005100: 7276 6963 6573 2e64 6174 615f 736f 7572  rvices.data_sour
+00005110: 6365 2069 6d70 6f72 7420 280a 2020 2020  ce import (.    
+00005120: 6c77 6470 2c0a 2920 2023 206c 7764 7020  lwdp,.)  # lwdp 
+00005130: 6461 7461 5f73 6f75 7263 6520 696e 6974  data_source init
+00005140: 6961 6c69 7a65 2074 6832 5f64 6174 615f  ialize th2_data_
+00005150: 7365 7276 6963 6573 2e63 6f6e 6669 6720  services.config 
+00005160: 6475 7269 6e67 2069 6d70 6f72 742e 0a66  during import..f
+00005170: 726f 6d20 7468 325f 6461 7461 5f73 6572  rom th2_data_ser
+00005180: 7669 6365 732e 636f 6e66 6967 2069 6d70  vices.config imp
+00005190: 6f72 7420 6f70 7469 6f6e 7320 6173 206f  ort options as o
+000051a0: 5f0a 6672 6f6d 2074 6832 5f64 6174 615f  _.from th2_data_
+000051b0: 7365 7276 6963 6573 2e64 6174 615f 736f  services.data_so
+000051c0: 7572 6365 2e6c 7764 702e 7374 7562 5f62  urce.lwdp.stub_b
+000051d0: 7569 6c64 6572 2069 6d70 6f72 7420 6874  uilder import ht
+000051e0: 7470 5f6d 6573 7361 6765 5f73 7475 625f  tp_message_stub_
+000051f0: 6275 696c 6465 720a 0a66 616b 655f 6461  builder..fake_da
+00005200: 7461 203d 205b 0a20 2020 2068 7474 705f  ta = [.    http_
+00005210: 6d65 7373 6167 655f 7374 7562 5f62 7569  message_stub_bui
+00005220: 6c64 6572 2e62 7569 6c64 287b 226d 6573  lder.build({"mes
+00005230: 7361 6765 4964 223a 2022 6122 2c20 226d  sageId": "a", "m
+00005240: 6573 7361 6765 5479 7065 223a 2022 526f  essageType": "Ro
+00005250: 6f74 227d 292c 0a20 2020 2068 7474 705f  ot"}),.    http_
+00005260: 6d65 7373 6167 655f 7374 7562 5f62 7569  message_stub_bui
+00005270: 6c64 6572 2e62 7569 6c64 287b 226d 6573  lder.build({"mes
+00005280: 7361 6765 4964 223a 2022 6222 2c20 226d  sageId": "b", "m
+00005290: 6573 7361 6765 5479 7065 223a 2022 4e65  essageType": "Ne
+000052a0: 7722 7d29 2c0a 2020 2020 6874 7470 5f6d  w"}),.    http_m
+000052b0: 6573 7361 6765 5f73 7475 625f 6275 696c  essage_stub_buil
+000052c0: 6465 722e 6275 696c 6428 7b22 6d65 7373  der.build({"mess
+000052d0: 6167 6549 6422 3a20 2263 222c 2022 6d65  ageId": "c", "me
+000052e0: 7373 6167 6554 7970 6522 3a20 2241 6d65  ssageType": "Ame
+000052f0: 6e64 227d 292c 0a20 2020 2068 7474 705f  nd"}),.    http_
+00005300: 6d65 7373 6167 655f 7374 7562 5f62 7569  message_stub_bui
+00005310: 6c64 6572 2e62 7569 6c64 287b 226d 6573  lder.build({"mes
+00005320: 7361 6765 4964 223a 2022 6422 2c20 226d  sageId": "d", "m
+00005330: 6573 7361 6765 5479 7065 223a 2022 4361  essageType": "Ca
+00005340: 6e63 656c 227d 292c 0a5d 0a66 616b 655f  ncel"}),.].fake_
+00005350: 6461 7461 5f6f 626a 203d 2044 6174 6128  data_obj = Data(
+00005360: 6661 6b65 5f64 6174 6129 0a0a 666f 7220  fake_data)..for 
+00005370: 6d20 696e 2066 616b 655f 6461 7461 5f6f  m in fake_data_o
+00005380: 626a 3a0a 2020 2020 6f5f 2e6d 6672 2e65  bj:.    o_.mfr.e
+00005390: 7870 616e 645f 6d65 7373 6167 6528 6d29  xpand_message(m)
+000053a0: 2020 2320 6d66 7220 2d20 7374 616e 6473    # mfr - stands
+000053b0: 2066 6f72 204d 6573 7361 6765 4669 656c   for MessageFiel
+000053c0: 6452 6573 6f6c 7665 720a 2320 6f72 0a66  dResolver.# or.f
+000053d0: 6f72 206d 2069 6e20 6661 6b65 5f64 6174  or m in fake_dat
+000053e0: 615f 6f62 6a2e 6d61 7028 6f5f 2e6d 6672  a_obj.map(o_.mfr
+000053f0: 2e65 7870 616e 645f 6d65 7373 6167 6529  .expand_message)
+00005400: 3a0a 2020 2020 7061 7373 0a0a 2320 5b34  :.    pass..# [4
+00005410: 2e32 5d20 4c69 6272 6172 6965 7320 7573  .2] Libraries us
+00005420: 6167 652e 0a23 2044 6f6e 2774 2069 6d70  age..# Don't imp
+00005430: 6f72 7420 6578 6163 7420 7265 736f 6c76  ort exact resolv
+00005440: 6572 7320 696d 706c 656d 656e 7461 7469  ers implementati
+00005450: 6f6e 2069 6e20 796f 7572 2063 6f64 652c  on in your code,
+00005460: 2070 6c65 6173 652e 0a23 2041 6c6c 6f77   please..# Allow
+00005470: 2079 6f75 7220 636c 6965 6e74 2074 6f20   your client to 
+00005480: 646f 2069 7420 696e 7374 6561 642e 0a23  do it instead..#
+00005490: 204a 7573 7420 696d 706f 7274 2060 6f70   Just import `op
+000054a0: 7469 6f6e 7360 2066 726f 6d20 6074 6832  tions` from `th2
+000054b0: 5f64 6174 615f 7365 7276 6963 6573 2e63  _data_services.c
+000054c0: 6f6e 6669 6760 2061 6e64 2075 7365 2069  onfig` and use i
+000054d0: 742e 0a66 726f 6d20 7468 325f 6461 7461  t..from th2_data
+000054e0: 5f73 6572 7669 6365 732e 636f 6e66 6967  _services.config
+000054f0: 2069 6d70 6f72 7420 6f70 7469 6f6e 7320   import options 
+00005500: 6173 206f 5f0a 0a66 6f72 206d 2069 6e20  as o_..for m in 
+00005510: 6661 6b65 5f64 6174 615f 6f62 6a3a 0a20  fake_data_obj:. 
+00005520: 2020 206f 5f2e 6d66 722e 6578 7061 6e64     o_.mfr.expand
+00005530: 5f6d 6573 7361 6765 286d 290a 2320 6f72  _message(m).# or
+00005540: 0a66 6f72 206d 2069 6e20 6661 6b65 5f64  .for m in fake_d
+00005550: 6174 615f 6f62 6a2e 6d61 7028 6f5f 2e6d  ata_obj.map(o_.m
+00005560: 6672 2e65 7870 616e 645f 6d65 7373 6167  fr.expand_messag
+00005570: 6529 3a0a 2020 2020 7061 7373 0a0a 2320  e):.    pass..# 
+00005580: 4d6f 7265 2074 6563 6820 6465 7461 696c  More tech detail
+00005590: 733a 0a23 2020 2049 6e20 7468 6973 2063  s:.#   In this c
+000055a0: 6173 652c 2074 6865 7265 2069 7320 6e6f  ase, there is no
+000055b0: 206c 696e 6520 6066 726f 6d20 7468 325f   line `from th2_
+000055c0: 6461 7461 5f73 6572 7669 6365 732e 6461  data_services.da
+000055d0: 7461 5f73 6f75 7263 6520 696d 706f 7274  ta_source import
+000055e0: 206c 7764 7020 600a 2320 2020 6265 6361   lwdp `.#   beca
+000055f0: 7573 6520 7765 2073 686f 756c 6420 6e6f  use we should no
+00005600: 7420 6368 6f6f 7365 2066 6f72 2074 6865  t choose for the
+00005610: 2075 7365 7220 7768 6963 6820 6120 6461   user which a da
+00005620: 7461 2073 6f75 7263 6520 746f 2075 7365  ta source to use
+00005630: 2e0a 2320 2020 5765 2064 6f20 6e6f 7420  ..#   We do not 
+00005640: 6b6e 6f77 2077 6861 7420 6865 2077 696c  know what he wil
+00005650: 6c20 6368 6f6f 7365 2c20 7468 6572 6566  l choose, theref
+00005660: 6f72 652c 2077 6520 6d75 7374 2073 696d  ore, we must sim
+00005670: 706c 7920 6163 6365 7373 0a23 2020 2074  ply access.#   t
+00005680: 6865 2069 6e74 6572 6661 6365 2c20 7768  he interface, wh
+00005690: 6963 6820 7769 6c6c 2062 6520 696e 6974  ich will be init
+000056a0: 6961 6c69 7a65 6420 6279 2074 6865 2075  ialized by the u
+000056b0: 7365 722e 0a0a 2323 2323 2323 2323 2323  ser...##########
+000056c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000056d0: 2323 2323 2323 2323 2323 2323 0a23 205b  ############.# [
+000056e0: 355d 2055 7369 6e67 2075 7469 6c69 7479  5] Using utility
+000056f0: 2066 756e 6374 696f 6e73 2e0a 2323 2323   functions..####
+00005700: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00005710: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00005720: 2323 0a66 726f 6d20 7468 325f 6461 7461  ##.from th2_data
+00005730: 5f73 6572 7669 6365 732e 7574 696c 732e  _services.utils.
+00005740: 6576 656e 745f 7574 696c 732e 6672 6571  event_utils.freq
+00005750: 7565 6e63 6965 7320 696d 706f 7274 2067  uencies import g
+00005760: 6574 5f63 6174 6567 6f72 795f 6672 6571  et_category_freq
+00005770: 7565 6e63 6965 7332 0a66 726f 6d20 7468  uencies2.from th
+00005780: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
+00005790: 7574 696c 732e 6576 656e 745f 7574 696c  utils.event_util
+000057a0: 732e 746f 7461 6c73 2069 6d70 6f72 7420  s.totals import 
+000057b0: 6765 745f 6361 7465 676f 7279 5f74 6f74  get_category_tot
+000057c0: 616c 7332 0a66 726f 6d20 7468 325f 6461  als2.from th2_da
+000057d0: 7461 5f73 6572 7669 6365 732e 7574 696c  ta_services.util
+000057e0: 732e 6361 7465 676f 7279 2069 6d70 6f72  s.category impor
+000057f0: 7420 4361 7465 676f 7279 0a66 726f 6d20  t Category.from 
+00005800: 7468 325f 6461 7461 5f73 6572 7669 6365  th2_data_service
+00005810: 732e 7574 696c 732e 6576 656e 745f 7574  s.utils.event_ut
+00005820: 696c 732e 6576 656e 745f 7574 696c 7320  ils.event_utils 
+00005830: 696d 706f 7274 2069 735f 736f 7274 6564  import is_sorted
+00005840: 0a0a 2320 5b35 2e31 5d20 4765 7420 7468  ..# [5.1] Get th
+00005850: 6520 7175 616e 7469 7469 6573 206f 6620  e quantities of 
+00005860: 6576 656e 7473 2066 6f72 2064 6966 6665  events for diffe
+00005870: 7265 6e74 2063 6174 6567 6f72 6965 732e  rent categories.
+00005880: 0a6d 6574 7269 6373 203d 205b 0a20 2020  .metrics = [.   
+00005890: 2043 6174 6567 6f72 7928 2264 6174 6522   Category("date"
+000058a0: 2c20 6c61 6d62 6461 206d 3a20 5468 3254  , lambda m: Th2T
+000058b0: 696d 6573 7461 6d70 436f 6e76 6572 7465  imestampConverte
+000058c0: 722e 746f 5f64 6174 6574 696d 6528 6d5b  r.to_datetime(m[
+000058d0: 2273 7461 7274 5469 6d65 7374 616d 7022  "startTimestamp"
+000058e0: 5d29 2e64 6174 6528 2929 2c0a 2020 2020  ]).date()),.    
+000058f0: 4361 7465 676f 7279 2822 7374 6174 7573  Category("status
+00005900: 222c 206c 616d 6264 6120 6d3a 206d 5b22  ", lambda m: m["
+00005910: 7375 6363 6573 7366 756c 225d 292c 0a5d  successful"]),.]
+00005920: 0a63 6174 6567 6f72 795f 746f 7461 6c73  .category_totals
+00005930: 203d 2067 6574 5f63 6174 6567 6f72 795f   = get_category_
+00005940: 746f 7461 6c73 3228 6576 656e 7473 2c20  totals2(events, 
+00005950: 6d65 7472 6963 7329 0a70 7269 6e74 2863  metrics).print(c
+00005960: 6174 6567 6f72 795f 746f 7461 6c73 290a  ategory_totals).
+00005970: 2222 220a 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d  """.+--------+--
+00005980: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
+00005990: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b  -----+---------+
+000059a0: 0a7c 2020 2020 2020 2020 7c20 6461 7465  .|        | date
+000059b0: 2020 2020 2020 207c 2073 7461 7475 7320         | status 
+000059c0: 2020 7c20 2020 636f 756e 7420 7c0a 2b3d    |   count |.+=
+000059d0: 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d  =======+========
+000059e0: 3d3d 3d3d 2b3d 3d3d 3d3d 3d3d 3d3d 3d2b  ====+==========+
+000059f0: 3d3d 3d3d 3d3d 3d3d 3d2b 0a7c 2020 2020  =========+.|    
+00005a00: 2020 2020 7c20 3230 3233 2d30 312d 3035      | 2023-01-05
+00005a10: 207c 2054 7275 6520 2020 2020 7c20 2020   | True     |   
+00005a20: 2020 2020 3320 7c0a 2b2d 2d2d 2d2d 2d2d      3 |.+-------
+00005a30: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  -+------------+-
+00005a40: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
+00005a50: 2d2d 2d2b 0a7c 2020 2020 2020 2020 7c20  ---+.|        | 
+00005a60: 3230 3233 2d30 312d 3035 207c 2046 616c  2023-01-05 | Fal
+00005a70: 7365 2020 2020 7c20 2020 2020 2020 3120  se    |       1 
+00005a80: 7c0a 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  |.+--------+----
+00005a90: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00005aa0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c  ---+---------+.|
+00005ab0: 2063 6f75 6e74 2020 7c20 2020 2020 2020   count  |       
+00005ac0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00005ad0: 7c20 2020 2020 2020 3220 7c0a 2b2d 2d2d  |       2 |.+---
+00005ae0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+00005af0: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  --+----------+--
+00005b00: 2d2d 2d2d 2d2d 2d2b 0a7c 2074 6f74 616c  -------+.| total
+00005b10: 7320 7c20 2020 2020 2020 2020 2020 207c  s |            |
+00005b20: 2031 2f31 2020 2020 2020 7c20 2020 2020   1/1      |     
+00005b30: 2020 3420 7c0a 2b2d 2d2d 2d2d 2d2d 2d2b    4 |.+--------+
+00005b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+00005b50: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+00005b60: 2d2b 0a22 2222 0a0a 2320 5b35 2e32 5d20  -+."""..# [5.2] 
+00005b70: 4765 7420 7468 6520 6e75 6d62 6572 206f  Get the number o
+00005b80: 6620 6576 656e 7473 2077 6974 6820 7374  f events with st
+00005b90: 6174 7573 2073 7563 6365 7373 6675 6c2e  atus successful.
+00005ba0: 0a63 6174 6567 6f72 7920 3d20 4361 7465  .category = Cate
+00005bb0: 676f 7279 2822 7374 6174 7573 222c 206c  gory("status", l
+00005bc0: 616d 6264 6120 6d3a 206d 5b22 7375 6363  ambda m: m["succ
+00005bd0: 6573 7366 756c 225d 290a 6361 7465 676f  essful"]).catego
+00005be0: 7279 5f66 7265 7175 656e 6369 6573 203d  ry_frequencies =
+00005bf0: 2067 6574 5f63 6174 6567 6f72 795f 6672   get_category_fr
+00005c00: 6571 7565 6e63 6965 7332 2865 7665 6e74  equencies2(event
+00005c10: 732c 2063 6174 6567 6f72 7929 0a70 7269  s, category).pri
+00005c20: 6e74 2863 6174 6567 6f72 795f 6672 6571  nt(category_freq
+00005c30: 7565 6e63 6965 7329 0a22 2222 0a2b 2d2d  uencies).""".+--
+00005c40: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+00005c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+00005c60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005c70: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  --+---------+---
+00005c80: 2d2d 2d2d 2d2b 0a7c 2020 2020 2020 2020  -----+.|        
+00005c90: 7c20 7469 6d65 7374 616d 705f 7374 6172  | timestamp_star
+00005ca0: 7420 2020 2020 7c20 7469 6d65 7374 616d  t     | timestam
+00005cb0: 705f 656e 6420 2020 2020 2020 7c20 4661  p_end       | Fa
+00005cc0: 6c73 6520 2020 7c20 2020 5472 7565 207c  lse   |   True |
+00005cd0: 0a2b 3d3d 3d3d 3d3d 3d3d 2b3d 3d3d 3d3d  .+========+=====
+00005ce0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00005cf0: 2b3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  +===============
+00005d00: 3d3d 3d3d 3d3d 2b3d 3d3d 3d3d 3d3d 3d3d  ======+=========
+00005d10: 2b3d 3d3d 3d3d 3d3d 3d2b 0a7c 2020 2020  +========+.|    
+00005d20: 2020 2020 7c20 3230 3233 2d30 312d 3035      | 2023-01-05
+00005d30: 5431 333a 3537 3a30 3520 7c20 3230 3233  T13:57:05 | 2023
+00005d40: 2d30 312d 3035 5431 333a 3537 3a30 3620  -01-05T13:57:06 
+00005d50: 7c20 3020 2020 2020 2020 7c20 2020 2020  | 0       |     
+00005d60: 2033 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2b2d   3 |.+--------+-
+00005d70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005d80: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
+00005d90: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
+00005da0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2b 0a7c  ----+--------+.|
+00005db0: 2020 2020 2020 2020 7c20 3230 3233 2d30          | 2023-0
+00005dc0: 312d 3035 5431 343a 3032 3a30 3520 7c20  1-05T14:02:05 | 
+00005dd0: 3230 3233 2d30 312d 3035 5431 343a 3032  2023-01-05T14:02
+00005de0: 3a30 3620 7c20 3120 2020 2020 2020 7c20  :06 | 1       | 
+00005df0: 2020 2020 2030 207c 0a2b 2d2d 2d2d 2d2d       0 |.+------
+00005e00: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
+00005e10: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00005e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
+00005e30: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00005e40: 2d2b 0a7c 2063 6f75 6e74 2020 7c20 2020  -+.| count  |   
+00005e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e60: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+00005e70: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00005e80: 2020 7c20 2020 2020 2032 207c 0a2b 2d2d    |      2 |.+--
+00005e90: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+00005ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+00005eb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005ec0: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  --+---------+---
+00005ed0: 2d2d 2d2d 2d2b 0a7c 2074 6f74 616c 7320  -----+.| totals 
+00005ee0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00005ef0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00005f00: 2020 2020 2020 2020 2020 2020 7c20 3120              | 1 
+00005f10: 2020 2020 2020 7c20 2020 2020 2033 207c        |      3 |
+00005f20: 0a2b 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  .+--------+-----
+00005f30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005f40: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
+00005f50: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+00005f60: 2b2d 2d2d 2d2d 2d2d 2d2b 0a22 2222 0a0a  +--------+."""..
+00005f70: 2320 5b35 2e33 5d20 4368 6563 6b20 6966  # [5.3] Check if
+00005f80: 2065 7665 6e74 7320 6172 6520 736f 7274   events are sort
+00005f90: 6564 2e0a 7265 7375 6c74 203d 2069 735f  ed..result = is_
+00005fa0: 736f 7274 6564 2865 7665 6e74 7329 0a70  sorted(events).p
+00005fb0: 7269 6e74 2872 6573 756c 7429 0a60 6060  rint(result).```
+00005fc0: 0a3c 212d 2d20 656e 6420 6765 745f 7374  .<!-- end get_st
+00005fd0: 6172 7465 645f 6578 616d 706c 652e 7079  arted_example.py
+00005fe0: 202d 2d3e 0a0a 2323 2032 2e33 2e20 5368   -->..## 2.3. Sh
+00005ff0: 6f72 7420 7468 656f 7279 0a0a 5468 6520  ort theory..The 
+00006000: 6c69 6272 6172 7920 7072 6f76 6964 6573  library provides
+00006010: 2074 6f6f 6c73 2066 6f72 2068 616e 646c   tools for handl
+00006020: 696e 6720 7374 7265 616d 2064 6174 612e  ing stream data.
+00006030: 2057 6861 7427 7320 6120 7374 7265 616d   What's a stream
+00006040: 3f20 4974 2773 2061 2073 6571 7565 6e63  ? It's a sequenc
+00006050: 6520 6f66 2065 6c65 6d65 6e74 7320 6672  e of elements fr
+00006060: 6f6d 2061 2073 6f75 7263 6520 7468 6174  om a source that
+00006070: 0a73 7570 706f 7274 7320 6167 6772 6567  .supports aggreg
+00006080: 6174 6520 6f70 6572 6174 696f 6e73 2e0a  ate operations..
+00006090: 0a23 2323 2054 6572 6d73 0a0a 2d20 2a2a  .### Terms..- **
+000060a0: 4461 7461 206f 626a 6563 742a 2a3a 2041  Data object**: A
+000060b0: 6e20 696e 7374 616e 6365 206f 6620 6044  n instance of `D
+000060c0: 6174 6160 2063 6c61 7373 2077 6869 6368  ata` class which
+000060d0: 2069 7320 7772 6170 7065 7220 756e 6465   is wrapper unde
+000060e0: 7220 7374 7265 616d 2e0a 2d20 2a2a 5365  r stream..- **Se
+000060f0: 7175 656e 6365 206f 6620 656c 656d 656e  quence of elemen
+00006100: 7473 2a2a 3a0a 2020 4120 5f44 6174 6120  ts**:.  A _Data 
+00006110: 6f62 6a65 6374 5f20 7072 6f76 6964 6573  object_ provides
+00006120: 2061 6e20 696e 7465 7266 6163 6520 746f   an interface to
+00006130: 2061 2073 6571 7565 6e63 6564 2073 6574   a sequenced set
+00006140: 206f 6620 7661 6c75 6573 206f 6620 6120   of values of a 
+00006150: 7370 6563 6966 6963 2065 6c65 6d65 6e74  specific element
+00006160: 2074 7970 652e 2053 7472 6561 6d20 696e   type. Stream in
+00006170: 7369 6465 2074 6865 205f 4461 7461 0a20  side the _Data. 
+00006180: 206f 626a 6563 745f 202a 2a64 6f6e 1974   object_ **don.t
+00006190: 2061 6374 7561 6c6c 7920 7374 6f72 652a   actually store*
+000061a0: 2a20 656c 656d 656e 7473 3b20 7468 6579  * elements; they
+000061b0: 2061 7265 2063 6f6d 7075 7465 6420 6f6e   are computed on
+000061c0: 2064 656d 616e 642e 0a2d 202a 2a64 6174   demand..- **dat
+000061d0: 6120 736f 7572 6365 2a2a 2028 6578 6163  a source** (exac
+000061e0: 746c 7920 696e 2073 6d61 6c6c 206c 6574  tly in small let
+000061f0: 7465 7273 293a 0a20 2041 6e79 2073 6f75  ters):.  Any sou
+00006200: 7263 6520 6f66 2064 6174 612e 2045 2e67  rce of data. E.g
+00006210: 2e20 5b4c 6967 6874 7765 6967 6874 2044  . [Lightweight D
+00006220: 6174 6120 5072 6f76 6964 6572 5d28 6874  ata Provider](ht
+00006230: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00006240: 2f74 6832 2d6e 6574 2f74 6832 2d6c 772d  /th2-net/th2-lw-
+00006250: 6461 7461 2d70 726f 7669 6465 7229 2c20  data-provider), 
+00006260: 636f 6c6c 6563 7469 6f6e 732c 0a20 2061  collections,.  a
+00006270: 7272 6179 732c 206f 7220 492f 4f20 7265  rrays, or I/O re
+00006280: 736f 7572 6365 732e 0a2d 202a 2a44 6174  sources..- **Dat
+00006290: 6153 6f75 7263 652a 2a3a 0a20 2041 2063  aSource**:.  A c
+000062a0: 6c61 7373 2074 6861 7420 6973 2061 6e20  lass that is an 
+000062b0: 696e 7465 726d 6564 6961 7465 206c 696e  intermediate lin
+000062c0: 6b20 6265 7477 6565 6e20 7468 6520 536f  k between the So
+000062d0: 7572 6365 4150 4920 616e 6420 436f 6d6d  urceAPI and Comm
+000062e0: 616e 6473 2e0a 2d20 2a2a 536f 7572 6365  ands..- **Source
+000062f0: 4150 492a 2a3a 0a20 2045 6163 6820 736f  API**:.  Each so
+00006300: 7572 6365 2068 6173 2069 7473 206f 776e  urce has its own
+00006310: 2041 5049 2074 6f20 7265 7472 6965 7665   API to retrieve
+00006320: 2064 6174 612e 2053 6f75 7263 6541 5049   data. SourceAPI
+00006330: 2069 7320 6120 636c 6173 7320 7468 6174   is a class that
+00006340: 2070 726f 7669 6465 2041 5049 2066 6f72   provide API for
+00006350: 2073 6f6d 6520 6461 7461 2073 6f75 7263   some data sourc
+00006360: 652e 0a2d 202a 2a43 6f6d 6d61 6e64 732a  e..- **Commands*
+00006370: 2a3a 0a20 2043 6c61 7373 6573 2074 6861  *:.  Classes tha
+00006380: 7420 7072 6f76 6964 6520 7573 6572 2d66  t provide user-f
+00006390: 7269 656e 646c 7920 696e 7465 7266 6163  riendly interfac
+000063a0: 6573 2066 6f72 2067 6574 7469 6e67 2073  es for getting s
+000063b0: 6f6d 6520 6461 7461 2066 726f 6d20 4461  ome data from Da
+000063c0: 7461 536f 7572 6365 2e20 436f 6d6d 616e  taSource. Comman
+000063d0: 6473 2075 7365 205f 536f 7572 6365 4150  ds use _SourceAP
+000063e0: 495f 2074 6f0a 2020 6163 6869 6576 6520  I_ to.  achieve 
+000063f0: 6974 2e0a 2d20 2a2a 4164 6170 7465 7273  it..- **Adapters
+00006400: 2a2a 3a0a 2020 4974 2773 2073 696d 696c  **:.  It's simil
+00006410: 6172 2074 6f20 6675 6e63 7469 6f6e 2066  ar to function f
+00006420: 6f72 2060 4461 7461 2e6d 6170 6020 6d65  or `Data.map` me
+00006430: 7468 6f64 2e20 4164 6f70 7461 626c 6520  thod. Adoptable 
+00006440: 636f 6d6d 616e 6473 2075 7365 6420 6974  commands used it
+00006450: 2074 6f20 7570 6461 7465 2074 6865 2064   to update the d
+00006460: 6174 6120 7374 7265 616d 2e0a 2d20 2a2a  ata stream..- **
+00006470: 4167 6772 6567 6174 6520 6f70 6572 6174  Aggregate operat
+00006480: 696f 6e73 2a2a 3a0a 2020 436f 6d6d 6f6e  ions**:.  Common
+00006490: 206f 7065 7261 7469 6f6e 7320 7375 6368   operations such
+000064a0: 2061 7320 6669 6c74 6572 2c20 6d61 702c   as filter, map,
+000064b0: 206c 696d 6974 2061 6e64 2073 6f20 6f6e   limit and so on
+000064c0: 2e0a 2d20 2a2a 576f 726b 666c 6f77 2a2a  ..- **Workflow**
+000064d0: 3a20 416e 206f 7264 6572 6564 2073 6574  : An ordered set
+000064e0: 206f 6620 5f41 6767 7265 6761 7465 206f   of _Aggregate o
+000064f0: 7065 7261 7469 6f6e 735f 2e0a 0a23 2323  perations_...###
+00006500: 2043 6f6e 6365 7074 0a0a 5468 6520 6c69   Concept..The li
+00006510: 6272 6172 7920 6465 7363 7269 6265 7320  brary describes 
+00006520: 7468 6520 6869 6768 2d6c 6576 656c 2069  the high-level i
+00006530: 6e74 6572 6661 6365 7320 6049 536f 7572  nterfaces `ISour
+00006540: 6365 4150 4960 2c20 6049 4461 7461 536f  ceAPI`, `IDataSo
+00006550: 7572 6365 602c 2060 4943 6f6d 6d61 6e64  urce`, `ICommand
+00006560: 602c 2060 4941 6461 7074 6572 602e 0a0a  `, `IAdapter`...
+00006570: 416e 7920 6461 7461 2073 6f75 7263 6520  Any data source 
+00006580: 6d75 7374 2062 6520 6465 7363 7269 6265  must be describe
+00006590: 6420 6279 2074 6865 2060 4944 6174 6153  d by the `IDataS
+000065a0: 6f75 7263 6560 2061 6273 7472 6163 7420  ource` abstract 
+000065b0: 636c 6173 732e 2054 6865 7365 2063 616e  class. These can
+000065c0: 2062 6520 5f46 696c 6544 6174 6153 6f75   be _FileDataSou
+000065d0: 7263 655f 2c0a 5f43 5356 4461 7461 536f  rce_,._CSVDataSo
+000065e0: 7572 6365 5f2c 205f 4442 4461 7461 536f  urce_, _DBDataSo
+000065f0: 7572 6365 5f20 616e 6420 6f74 6865 722e  urce_ and other.
+00006600: 0a0a 5573 7561 6c6c 792c 2064 6174 6120  ..Usually, data 
+00006610: 736f 7572 6365 7320 6861 7665 2073 6f6d  sources have som
+00006620: 6520 6b69 6e64 206f 6620 4150 492e 2044  e kind of API. D
+00006630: 6174 6162 6173 6573 202d 2070 726f 7669  atabases - provi
+00006640: 6465 2053 514c 206c 616e 6775 6167 652c  de SQL language,
+00006650: 2077 6865 6e20 776f 726b 696e 6720 7769   when working wi
+00006660: 7468 2061 2066 696c 652c 2079 6f75 2063  th a file, you c
+00006670: 616e 2072 6561 640a 6c69 6e65 2062 7920  an read.line by 
+00006680: 6c69 6e65 2c20 6574 632e 2054 6869 7320  line, etc. This 
+00006690: 4150 4920 6973 2064 6573 6372 6962 6564  API is described
+000066a0: 2062 7920 7468 6520 6049 536f 7572 6365   by the `ISource
+000066b0: 4150 4960 2063 6c61 7373 2e20 4265 6361  API` class. Beca
+000066c0: 7573 6520 6469 6666 6572 656e 7420 7665  use different ve
+000066d0: 7273 696f 6e73 206f 6620 7468 6520 7361  rsions of the sa
+000066e0: 6d65 2064 6174 6120 736f 7572 6365 0a6d  me data source.m
+000066f0: 6179 2068 6176 6520 6469 6666 6572 656e  ay have differen
+00006700: 7420 4150 492c 2069 7420 6973 2062 6574  t API, it is bet
+00006710: 7465 7220 746f 2063 7265 6174 6520 6120  ter to create a 
+00006720: 636c 6173 7320 666f 7220 6561 6368 2076  class for each v
+00006730: 6572 7369 6f6e 2e0a 0a47 656e 6572 616c  ersion...General
+00006740: 6c79 2c20 6461 7461 2073 6f75 7263 6520  ly, data source 
+00006750: 4150 4973 2061 7265 2068 6964 6465 6e20  APIs are hidden 
+00006760: 6265 6869 6e64 2063 6f6e 7665 6e69 656e  behind convenien
+00006770: 7420 696e 7465 7266 6163 6573 2e20 5468  t interfaces. Th
+00006780: 6520 726f 6c65 206f 6620 7468 6573 6520  e role of these 
+00006790: 696e 7465 7266 6163 6573 2069 7320 706c  interfaces is pl
+000067a0: 6179 6564 0a62 7920 6049 436f 6d6d 616e  ayed.by `IComman
+000067b0: 6460 2063 6c61 7373 6573 2e0a 0a60 4941  d` classes...`IA
+000067c0: 6461 7074 6572 6020 636c 6173 7365 7320  dapter` classes 
+000067d0: 7472 616e 7366 6f72 6d20 6461 7461 2073  transform data s
+000067e0: 7472 6561 6d20 6c69 6b65 2066 756e 6374  tream like funct
+000067f0: 696f 6e73 2066 6f72 2060 4461 7461 2e6d  ions for `Data.m
+00006800: 6170 6020 6d65 7468 6f64 2e20 4573 7365  ap` method. Esse
+00006810: 6e74 6961 6c6c 7920 6974 2773 2074 6865  ntially it's the
+00006820: 2073 616d 6520 7468 696e 6720 6275 7420   same thing but 
+00006830: 6d6f 7265 0a66 6c65 7869 626c 652e 0a0a  more.flexible...
+00006840: 466f 7220 6578 616d 706c 652c 204c 7744  For example, LwD
+00006850: 5020 4461 7461 536f 7572 6365 2868 7474  P DataSource(htt
+00006860: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00006870: 7468 322d 6e65 742f 7468 322d 6473 2d73  th2-net/th2-ds-s
+00006880: 6f75 7263 652d 6c77 6470 2920 7573 6573  ource-lwdp) uses
+00006890: 2074 6865 7365 2061 6273 7472 6163 7420   these abstract 
+000068a0: 636c 6173 7365 7320 746f 2062 7569 6c64  classes to build
+000068b0: 2069 7473 2069 6d70 6c65 6d65 6e74 6174   its implementat
+000068c0: 696f 6e2e 596f 7520 6361 6e20 6561 7369  ion.You can easi
+000068d0: 6c79 2063 7265 6174 6520 796f 7572 206f  ly create your o
+000068e0: 776e 2075 6e69 7175 6520 636f 6d6d 616e  wn unique comman
+000068f0: 6473 2066 6f72 205f 4c77 4450 2044 6174  ds for _LwDP Dat
+00006900: 6153 6f75 7263 655f 2c20 6173 2077 656c  aSource_, as wel
+00006910: 6c20 6173 2065 6e74 6972 650a 5f44 6174  l as entire._Dat
+00006920: 6153 6f75 7263 655f 2063 6c61 7373 6573  aSource_ classes
+00006930: 2e20 5b48 6572 6520 6973 2061 2064 6f63  . [Here is a doc
+00006940: 756d 656e 7461 7469 6f6e 5d28 646f 6375  umentation](docu
+00006950: 6d65 6e74 6174 696f 6e2f 6461 7461 736f  mentation/dataso
+00006960: 7572 6365 2e6d 6429 206f 6e20 686f 7720  urce.md) on how 
+00006970: 746f 2069 6d70 6c65 6d65 6e74 2074 6865  to implement the
+00006980: 7365 2069 6e74 6572 6661 6365 732e 0a0a  se interfaces...
+00006990: 215b 4461 7461 2073 7472 6561 6d20 7069  ![Data stream pi
+000069a0: 7065 6c69 6e65 5d28 646f 6375 6d65 6e74  peline](document
+000069b0: 6174 696f 6e2f 696d 672f 636f 6e63 6570  ation/img/concep
+000069c0: 742e 706e 6729 0a0a 2323 2320 5374 7265  t.png)..### Stre
+000069d0: 616d 206f 7065 7261 7469 6f6e 730a 0a46  am operations..F
+000069e0: 7572 7468 6572 6d6f 7265 2c20 7374 7265  urthermore, stre
+000069f0: 616d 206f 7065 7261 7469 6f6e 7320 6861  am operations ha
+00006a00: 7665 2074 776f 2066 756e 6461 6d65 6e74  ve two fundament
+00006a10: 616c 2063 6861 7261 6374 6572 6973 7469  al characteristi
+00006a20: 6373 2074 6861 7420 6d61 6b65 2074 6865  cs that make the
+00006a30: 6d20 7665 7279 2064 6966 6665 7265 6e74  m very different
+00006a40: 2066 726f 6d20 636f 6c6c 6563 7469 6f6e   from collection
+00006a50: 0a6f 7065 7261 7469 6f6e 733a 205f 5069  .operations: _Pi
+00006a60: 7065 6c69 6e69 6e67 5f20 616e 6420 5f49  pelining_ and _I
+00006a70: 6e74 6572 6e61 6c20 6974 6572 6174 696f  nternal iteratio
+00006a80: 6e5f 2e0a 0a23 2323 2320 5069 7065 6c69  n_...#### Pipeli
+00006a90: 6e69 6e67 0a0a 4d61 6e79 2073 7472 6561  ning..Many strea
+00006aa0: 6d20 6f70 6572 6174 696f 6e73 2072 6574  m operations ret
+00006ab0: 7572 6e20 6120 7374 7265 616d 2074 6865  urn a stream the
+00006ac0: 6d73 656c 7665 732e 2054 6869 7320 616c  mselves. This al
+00006ad0: 6c6f 7773 206f 7065 7261 7469 6f6e 7320  lows operations 
+00006ae0: 746f 2062 6520 6368 6169 6e65 6420 746f  to be chained to
+00006af0: 2066 6f72 6d20 6120 6c61 7267 6572 2070   form a larger p
+00006b00: 6970 656c 696e 652e 0a0a 215b 4461 7461  ipeline...![Data
+00006b10: 2073 7472 6561 6d20 7069 7065 6c69 6e65   stream pipeline
+00006b20: 5d28 646f 6375 6d65 6e74 6174 696f 6e2f  ](documentation/
+00006b30: 696d 672f 6461 7461 5f73 7472 6561 6d5f  img/data_stream_
+00006b40: 7069 7065 6c69 6e65 2e70 6e67 290a 0a23  pipeline.png)..#
+00006b50: 2323 2320 496e 7465 726e 616c 2069 7465  ### Internal ite
+00006b60: 7261 7469 6f6e 0a0a 496e 2063 6f6e 7472  ration..In contr
+00006b70: 6173 7420 746f 2063 6f6c 6c65 6374 696f  ast to collectio
+00006b80: 6e73 2c20 7768 6963 6820 6172 6520 6974  ns, which are it
+00006b90: 6572 6174 6564 2065 7870 6c69 6369 746c  erated explicitl
+00006ba0: 7920 2865 7874 6572 6e61 6c20 6974 6572  y (external iter
+00006bb0: 6174 696f 6e29 2c20 7374 7265 616d 206f  ation), stream o
+00006bc0: 7065 7261 7469 6f6e 7320 646f 2074 6865  perations do the
+00006bd0: 2069 7465 7261 7469 6f6e 0a62 6568 696e   iteration.behin
+00006be0: 6420 7468 6520 7363 656e 6573 2066 6f72  d the scenes for
+00006bf0: 2079 6f75 2e20 4e6f 7465 2c20 6974 2064   you. Note, it d
+00006c00: 6f65 736e 2774 206d 6561 6e20 796f 7520  oesn't mean you 
+00006c10: 6361 6e6e 6f74 2069 7465 7261 7465 2074  cannot iterate t
+00006c20: 6865 205f 4461 7461 206f 626a 6563 745f  he _Data object_
+00006c30: 2e0a 0a0a 2323 2320 4461 7461 2069 7465  ....### Data ite
+00006c40: 7261 7469 6f6e 0a0a 5468 6520 4461 7461  ration..The Data
+00006c50: 206f 626a 6563 7420 636f 6e73 7472 7563   object construc
+00006c60: 746f 7220 6d65 7468 6f64 2074 616b 6573  tor method takes
+00006c70: 2069 6e20 6173 2061 7267 756d 656e 7420   in as argument 
+00006c80: 6569 7468 6572 2061 6e20 6974 6572 6174  either an iterat
+00006c90: 6f72 206f 7665 7220 6f62 6a65 6374 7320  or over objects 
+00006ca0: 6f72 2061 2067 656e 6572 6174 6f72 2066  or a generator f
+00006cb0: 756e 6374 696f 6e2e 0a54 6865 2044 6174  unction..The Dat
+00006cc0: 6120 6f62 6a65 6374 2069 7465 7261 746f  a object iterato
+00006cd0: 7220 6861 6e64 6c65 7320 6561 6368 2069  r handles each i
+00006ce0: 7465 6d20 696e 2074 6869 7320 6974 6572  tem in this iter
+00006cf0: 6174 6f72 206f 7220 6765 6e65 7261 746f  ator or generato
+00006d00: 7220 6173 2074 6865 7920 6172 652c 206d  r as they are, m
+00006d10: 6561 6e69 6e67 2069 7420 646f 6573 6e27  eaning it doesn'
+00006d20: 7420 7472 7920 746f 2072 6561 6420 7468  t try to read th
+00006d30: 6520 636f 6e74 656e 7420 6f66 2069 7465  e content of ite
+00006d40: 6d20 6f72 2072 6574 7572 6e20 7468 656d  m or return them
+00006d50: 206d 6f64 6966 6965 6420 696e 2061 6e79   modified in any
+00006d60: 2077 6179 2c20 696e 7374 6561 6420 7265   way, instead re
+00006d70: 7475 726e 7320 7468 6520 6974 656d 2069  turns the item i
+00006d80: 7473 656c 662e 0a54 6865 206f 6e6c 7920  tself..The only 
+00006d90: 6578 6365 7074 696f 6e20 746f 2074 6869  exception to thi
+00006da0: 7320 6973 2077 6865 6e20 4461 7461 206f  s is when Data o
+00006db0: 626a 6563 7420 6973 2062 7569 6c74 2075  bject is built u
+00006dc0: 7369 6e67 2069 7465 7261 746f 7220 6f72  sing iterator or
+00006dd0: 2067 656e 6572 6174 6f72 206f 7665 7220   generator over 
+00006de0: 6f74 6865 7220 4461 7461 206f 626a 6563  other Data objec
+00006df0: 7473 2e20 4e6f 7465 2074 6861 7420 7468  ts. Note that th
+00006e00: 6973 2069 7465 7261 746f 7220 6f72 2067  is iterator or g
+00006e10: 656e 6572 6174 6f72 206d 7573 7420 6f6e  enerator must on
+00006e20: 6c79 2062 6520 7969 656c 6469 6e67 2044  ly be yielding D
+00006e30: 6174 6120 6f62 6a65 6374 7320 616e 6420  ata objects and 
+00006e40: 6e6f 7468 696e 6720 656c 7365 2e20 4966  nothing else. If
+00006e50: 2077 6520 6275 696c 6420 6672 6f6d 2061   we build from a
+00006e60: 206d 6978 206f 6620 4461 7461 206f 626a   mix of Data obj
+00006e70: 6563 7473 2061 6e64 2073 6f6d 6520 6f74  ects and some ot
+00006e80: 6865 7220 7479 7065 732c 2044 6174 6120  her types, Data 
+00006e90: 6f62 6a65 6374 7327 2063 6f6e 7465 6e74  objects' content
+00006ea0: 2077 6f6e 2774 2062 6520 7265 6164 2061   won't be read a
+00006eb0: 6e64 2069 6e73 7465 6164 2069 7420 7769  nd instead it wi
+00006ec0: 6c6c 2062 6520 7265 7475 726e 6564 2061  ll be returned a
+00006ed0: 7320 4461 7461 206f 626a 6563 7420 6974  s Data object it
+00006ee0: 7365 6c66 2e0a 0a53 6d61 6c6c 2065 7861  self...Small exa
+00006ef0: 6d70 6c65 2074 6f20 6465 6d6f 6e73 7472  mple to demonstr
+00006f00: 6174 653a 0a0a 6060 6070 7974 686f 6e0a  ate:..```python.
+00006f10: 6672 6f6d 2074 6832 5f64 6174 615f 7365  from th2_data_se
+00006f20: 7276 6963 6573 2e64 6174 6120 696d 706f  rvices.data impo
+00006f30: 7274 2044 6174 610a 0a64 3120 3d20 4461  rt Data..d1 = Da
+00006f40: 7461 285b 312c 322c 335d 290a 6432 203d  ta([1,2,3]).d2 =
+00006f50: 2044 6174 6128 5b34 2c35 2c36 5d29 0a0a   Data([4,5,6])..
+00006f60: 6f6e 6c79 5f64 6174 615f 6f62 6a65 6374  only_data_object
+00006f70: 7320 3d20 4461 7461 285b 6431 2c64 325d  s = Data([d1,d2]
+00006f80: 2920 2320 5769 6c6c 2069 7465 7261 7465  ) # Will iterate
+00006f90: 2061 7320 312c 322c 332c 342c 352c 360a   as 1,2,3,4,5,6.
+00006fa0: 6461 7461 5f61 6e64 5f6c 6973 7420 3d20  data_and_list = 
+00006fb0: 4461 7461 285b 6431 2c5b 342c 352c 365d  Data([d1,[4,5,6]
+00006fc0: 5d29 2023 2057 696c 6c20 6974 6572 6174  ]) # Will iterat
+00006fd0: 6520 6173 2064 312c 205b 342c 352c 365d  e as d1, [4,5,6]
+00006fe0: 0a64 6174 615f 616e 645f 6e75 6d62 6572  .data_and_number
+00006ff0: 7320 3d20 4461 7461 285b 6431 2c34 2c35  s = Data([d1,4,5
+00007000: 2c36 5d29 2023 2057 696c 6c20 6974 6572  ,6]) # Will iter
+00007010: 6174 6520 6173 2064 312c 342c 352c 360a  ate as d1,4,5,6.
+00007020: 6c69 7374 735f 6f6e 6c79 203d 2044 6174  lists_only = Dat
+00007030: 6128 5b31 2c32 2c33 5d2c 5b34 2c35 2c36  a([1,2,3],[4,5,6
+00007040: 5d29 2023 2057 696c 6c20 6974 6572 6174  ]) # Will iterat
+00007050: 6520 6173 205b 312c 322c 335d 2c5b 342c  e as [1,2,3],[4,
+00007060: 352c 365d 0a0a 2320 4966 2077 6520 7761  5,6]..# If we wa
+00007070: 6e74 2074 6f20 6974 6572 6174 6520 6f76  nt to iterate ov
+00007080: 6572 2063 6f6e 7465 6e74 206f 6620 6c69  er content of li
+00007090: 7374 206f 6620 6c69 7374 732c 2077 6520  st of lists, we 
+000070a0: 7368 6f75 6c64 2066 6972 7374 2063 7265  should first cre
+000070b0: 6174 6520 4461 7461 206f 626a 6563 7473  ate Data objects
+000070c0: 2066 726f 6d20 7468 656d 2c0a 2320 7468   from them,.# th
+000070d0: 656e 2075 7365 2074 6865 6d20 746f 2063  en use them to c
+000070e0: 6f6e 7374 7275 6374 206e 6577 2044 6174  onstruct new Dat
+000070f0: 6120 6f62 6a65 6374 2061 7320 696e 2063  a object as in c
+00007100: 6173 6520 6f66 2064 3120 616e 6420 6432  ase of d1 and d2
+00007110: 2c20 6372 6561 7469 6e67 2027 6f6e 6c79  , creating 'only
+00007120: 5f64 6174 615f 6f62 6a65 6374 7327 2069  _data_objects' i
+00007130: 6e20 7468 6973 2065 7861 6d70 6c65 2e0a  n this example..
+00007140: 6060 600a 200a 0a23 2323 2044 6174 6120  ```. ..### Data 
+00007150: 6361 6368 696e 670a 0a54 6865 205f 4461  caching..The _Da
+00007160: 7461 206f 626a 6563 745f 2070 726f 7669  ta object_ provi
+00007170: 6465 7320 7468 6520 6162 696c 6974 7920  des the ability 
+00007180: 746f 2075 7365 2074 6865 2063 6163 6865  to use the cache
+00007190: 2e20 5468 6520 6361 6368 6520 776f 726b  . The cache work
+000071a0: 7320 666f 7220 6561 6368 205f 4461 7461  s for each _Data
+000071b0: 206f 626a 6563 745f 2c20 7468 6174 2069   object_, that i
+000071c0: 732c 2079 6f75 2063 686f 6f73 650a 7768  s, you choose.wh
+000071d0: 6963 6820 5f44 6174 6120 6f62 6a65 6374  ich _Data object
+000071e0: 5f20 796f 7520 7761 6e74 2074 6f20 7361  _ you want to sa
+000071f0: 7665 2e20 5468 6520 5f44 6174 6120 6f62  ve. The _Data ob
+00007200: 6a65 6374 5f20 6361 6368 6520 6973 2073  ject_ cache is s
+00007210: 6176 6564 2061 6674 6572 2074 6865 2066  aved after the f
+00007220: 6972 7374 2069 7465 7261 7469 6f6e 2c20  irst iteration, 
+00007230: 6275 7420 7468 6520 6974 6572 6174 696f  but the iteratio
+00007240: 6e0a 736f 7572 6365 206d 6179 2062 6520  n.source may be 
+00007250: 6469 6666 6572 656e 742e 0a0a 4966 2079  different...If y
+00007260: 6f75 2064 6f6e 2774 2075 7365 2074 6865  ou don't use the
+00007270: 2063 6163 6865 2c20 796f 7572 2073 6f75   cache, your sou
+00007280: 7263 6520 7769 6c6c 2062 6520 7468 6520  rce will be the 
+00007290: 6461 7461 2073 6f75 7263 6520 796f 7520  data source you 
+000072a0: 6861 7665 2069 6e20 7468 6520 5f44 6174  have in the _Dat
+000072b0: 6120 4f62 6a65 6374 5f2e 2042 7574 2069  a Object_. But i
+000072c0: 6620 796f 7520 7573 6520 7468 6520 6361  f you use the ca
+000072d0: 6368 652c 0a79 6f75 7220 736f 7572 6365  che,.your source
+000072e0: 2063 616e 2062 6520 7468 6520 6461 7461   can be the data
+000072f0: 2073 6f75 7263 652c 2074 6865 2070 6172   source, the par
+00007300: 656e 7420 6361 6368 652c 206f 7220 6f77  ent cache, or ow
+00007310: 6e20 6361 6368 653a 0a0a 2a20 5468 6520  n cache:..* The 
+00007320: 6461 7461 2073 6f75 7263 653a 0a20 2049  data source:.  I
+00007330: 6620 7468 6520 5f44 6174 6120 4f62 6a65  f the _Data Obje
+00007340: 6374 5f20 646f 6573 6e27 7420 6861 7665  ct_ doesn't have
+00007350: 2061 2070 6172 656e 7420 6361 6368 6520   a parent cache 
+00007360: 616e 6420 6974 7320 6361 6368 652e 0a2a  and its cache..*
+00007370: 2054 6865 2070 6172 656e 7420 6361 6368   The parent cach
+00007380: 653a 0a20 2049 6620 7468 6520 5f44 6174  e:.  If the _Dat
+00007390: 6120 4f62 6a65 6374 5f20 6861 7320 6120  a Object_ has a 
+000073a0: 7061 7265 6e74 2063 6163 6865 2e20 4974  parent cache. It
+000073b0: 2064 6f65 736e 2774 206d 6174 7465 7220   doesn't matter 
+000073c0: 7768 6174 2070 6f73 6974 696f 6e20 7468  what position th
+000073d0: 6520 7061 7265 6e74 2063 6163 6865 2068  e parent cache h
+000073e0: 6173 2069 6e20 696e 6865 7269 7461 6e63  as in inheritanc
+000073f0: 652e 0a20 205f 4461 7461 204f 626a 6563  e..  _Data Objec
+00007400: 745f 2075 6e64 6572 7374 616e 6473 2077  t_ understands w
+00007410: 686f 7365 2063 6163 6865 2069 7420 6973  hose cache it is
+00007420: 2061 6e64 2065 7865 6375 7465 7320 7468   and executes th
+00007430: 6520 7061 7274 206f 6620 7468 6520 776f  e part of the wo
+00007440: 726b 666c 6f77 2074 6861 7420 7761 7320  rkflow that was 
+00007450: 6e6f 7420 6578 6563 7574 6564 2e0a 2a20  not executed..* 
+00007460: 5468 6520 6f77 6e20 6361 6368 653a 0a20  The own cache:. 
+00007470: 2049 6620 6974 2069 7320 6e6f 7420 7468   If it is not th
+00007480: 6520 6669 7273 7420 6974 6572 6174 696f  e first iteratio
+00007490: 6e20 6f66 2074 6869 7320 4461 7461 206f  n of this Data o
+000074a0: 626a 6563 742e 0a0a 4e6f 7465 2074 6861  bject...Note tha
+000074b0: 7420 7468 6520 6361 6368 6520 7374 6174  t the cache stat
+000074c0: 6520 6f66 2074 6865 2044 6174 6120 6f62  e of the Data ob
+000074d0: 6a65 6374 2069 7320 6e6f 7420 696e 6865  ject is not inhe
+000074e0: 7269 7465 642e 0a0a 2323 2323 2046 6f72  rited...#### For
+000074f0: 6365 6420 6361 6368 696e 670a 596f 7520  ced caching.You 
+00007500: 6361 6e20 7465 6c6c 2044 5320 746f 2063  can tell DS to c
+00007510: 6163 6865 2064 6174 6120 746f 2073 7065  ache data to spe
+00007520: 6369 6669 6320 6361 6368 6520 6669 6c65  cific cache file
+00007530: 2c20 7768 6963 6820 776f 6e27 7420 6265  , which won't be
+00007540: 2064 656c 6574 6564 2061 6674 6572 2073   deleted after s
+00007550: 6372 6970 7420 656e 642e 0a59 6f75 2063  cript end..You c
+00007560: 616e 2073 6565 2065 7861 6d70 6c65 2069  an see example i
+00007570: 6e20 312e 3132 2073 6563 7469 6f6e 206f  n 1.12 section o
+00007580: 6620 5b67 6574 5f73 7461 7274 6564 5f65  f [get_started_e
+00007590: 7861 6d70 6c65 5d28 6578 616d 706c 6573  xample](examples
+000075a0: 2f67 6574 5f73 7461 7274 6564 5f65 7861  /get_started_exa
+000075b0: 6d70 6c65 2e70 7929 2e0a 0a0a 2323 2320  mple.py)....### 
+000075c0: 4576 656e 7454 7265 6520 616e 6420 636f  EventTree and co
+000075d0: 6c6c 6563 7469 6f6e 730a 0a23 2323 2320  llections..#### 
+000075e0: 4576 656e 7454 7265 650a 0a60 4576 656e  EventTree..`Even
+000075f0: 7454 7265 6560 2069 7320 6120 7472 6565  tTree` is a tree
+00007600: 2d62 6173 6564 2064 6174 6120 7374 7275  -based data stru
+00007610: 6374 7572 6520 6f66 2065 7665 6e74 732e  cture of events.
+00007620: 2049 7420 616c 6c6f 7773 2079 6f75 2067   It allows you g
+00007630: 6574 2063 6869 6c64 7265 6e20 616e 6420  et children and 
+00007640: 7061 7265 6e74 7320 6f66 2065 7665 6e74  parents of event
+00007650: 2c0a 6469 7370 6c61 7920 7472 6565 2c20  ,.display tree, 
+00007660: 6765 7420 6675 6c6c 2070 6174 6820 746f  get full path to
+00007670: 2065 7665 6e74 2065 7463 2e0a 0a44 6574   event etc...Det
+00007680: 6169 6c73 3a0a 0a2a 2060 4576 656e 7454  ails:..* `EventT
+00007690: 7265 6560 2063 6f6e 7461 696e 7320 616c  ree` contains al
+000076a0: 6c20 6576 656e 7473 2069 6e20 6d65 6d6f  l events in memo
+000076b0: 7279 2e0a 2a20 5472 6565 2068 6173 2073  ry..* Tree has s
+000076c0: 6f6d 6520 696d 706f 7274 616e 7420 7465  ome important te
+000076d0: 726d 733a 0a20 2020 2031 2e20 5f41 6e63  rms:.    1. _Anc
+000076e0: 6573 746f 725f 2069 7320 616e 7920 7265  estor_ is any re
+000076f0: 6c61 7469 7665 206f 6620 7468 6520 6576  lative of the ev
+00007700: 656e 7420 7570 2074 6865 2074 7265 6520  ent up the tree 
+00007710: 2867 7261 6e64 7061 7265 6e74 2c20 7061  (grandparent, pa
+00007720: 7265 6e74 2065 7463 2e29 2e0a 2020 2020  rent etc.)..    
+00007730: 322e 205f 5061 7265 6e74 5f20 6973 206f  2. _Parent_ is o
+00007740: 6e6c 7920 7468 6520 6669 7273 7420 7265  nly the first re
+00007750: 6c61 7469 7665 206f 6620 7468 6520 6576  lative of the ev
+00007760: 656e 7420 7570 2074 6865 2074 7265 652e  ent up the tree.
+00007770: 0a20 2020 2033 2e20 5f43 6869 6c64 5f20  .    3. _Child_ 
+00007780: 6973 2074 6865 2066 6972 7374 2072 656c  is the first rel
+00007790: 6174 6976 6520 6f66 2074 6865 2065 7665  ative of the eve
+000077a0: 6e74 2064 6f77 6e20 7468 6520 7472 6565  nt down the tree
+000077b0: 2e0a 0a54 616b 6520 6120 6c6f 6f6b 2061  ...Take a look a
+000077c0: 7420 7468 6520 666f 6c6c 6f77 696e 6720  t the following 
+000077d0: 4854 4d4c 2074 7265 6520 746f 2075 6e64  HTML tree to und
+000077e0: 6572 7374 616e 6420 7468 656d 2e0a 0a20  erstand them... 
+000077f0: 2020 6060 600a 2020 2020 3c62 6f64 793e    ```.    <body>
+00007800: 203c 212d 2d20 616e 6365 7374 6f72 2028   <!-- ancestor (
+00007810: 6772 616e 6470 6172 656e 7429 2c20 6275  grandparent), bu
+00007820: 7420 6e6f 7420 7061 7265 6e74 202d 2d3e  t not parent -->
+00007830: 0a20 2020 2020 2020 203c 6469 763e 203c  .        <div> <
+00007840: 212d 2d20 7061 7265 6e74 2026 2061 6e63  !-- parent & anc
+00007850: 6573 746f 7220 2d2d 3e0a 2020 2020 2020  estor -->.      
+00007860: 2020 2020 2020 3c70 3e48 656c 6c6f 2c20        <p>Hello, 
+00007870: 776f 726c 6421 3c2f 703e 203c 212d 2d20  world!</p> <!-- 
+00007880: 6368 696c 6420 2d2d 3e0a 2020 2020 2020  child -->.      
+00007890: 2020 2020 2020 3c70 3e47 6f6f 6462 7965        <p>Goodbye
+000078a0: 213c 2f70 3e20 3c21 2d2d 2073 6962 6c69  !</p> <!-- sibli
+000078b0: 6e67 202d 2d3e 0a20 2020 2020 2020 203c  ng -->.        <
+000078c0: 2f64 6976 3e0a 2020 2020 3c2f 626f 6479  /div>.    </body
+000078d0: 3e0a 2020 2060 6060 0a0a 2323 2323 2043  >.   ```..#### C
+000078e0: 6f6c 6c65 6374 696f 6e73 0a0a 2a2a 4576  ollections..**Ev
+000078f0: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
+00007900: 6e2a 2a20 6973 2061 2063 6f6c 6c65 6374  n** is a collect
+00007910: 696f 6e20 6f66 2045 7665 6e74 5472 6565  ion of EventTree
+00007920: 732e 2054 6865 2063 6f6c 6c65 6374 696f  s. The collectio
+00007930: 6e20 6275 696c 6473 2061 2066 6577 205f  n builds a few _
+00007940: 4576 656e 7454 7265 655f 2062 7920 7061  EventTree_ by pa
+00007950: 7373 6564 205f 4461 7461 0a6f 626a 6563  ssed _Data.objec
+00007960: 745f 2e20 416c 7468 6f75 6768 2079 6f75  t_. Although you
+00007970: 2063 616e 2063 6861 6e67 6520 7468 6520   can change the 
+00007980: 7472 6565 2064 6972 6563 746c 792c 2069  tree directly, i
+00007990: 7427 7320 6265 7474 6572 2074 6f20 646f  t's better to do
+000079a0: 2069 7420 7468 726f 7567 6820 636f 6c6c   it through coll
+000079b0: 6563 7469 6f6e 7320 6265 6361 7573 6520  ections because 
+000079c0: 7468 6579 2061 7265 2061 7761 7265 206f  they are aware o
+000079d0: 660a 6064 6574 6163 6865 645f 6576 656e  f.`detached_even
+000079e0: 7473 6020 616e 6420 6361 6e20 736f 6c76  ts` and can solv
+000079f0: 6520 736f 6d65 2065 7665 6e74 7320 6465  e some events de
+00007a00: 7065 6e64 656e 6369 6573 2e20 5468 6520  pendencies. The 
+00007a10: 636f 6c6c 6563 7469 6f6e 2068 6173 2073  collection has s
+00007a20: 696d 696c 6172 2066 6561 7475 7265 7320  imilar features 
+00007a30: 6c69 6b65 2061 2073 696e 676c 6520 5f45  like a single _E
+00007a40: 7665 6e74 5472 6565 5f0a 6275 7420 6170  ventTree_.but ap
+00007a50: 706c 7969 6e67 2074 6865 6d20 666f 7220  plying them for 
+00007a60: 616c 6c20 5f45 7665 6e74 5472 6565 735f  all _EventTrees_
+00007a70: 2e0a 0a2a 2a50 6172 656e 7445 7665 6e74  ...**ParentEvent
+00007a80: 5472 6565 436f 6c6c 6563 7469 6f6e 2a2a  TreeCollection**
+00007a90: 2069 7320 6120 636f 6c6c 6563 7469 6f6e   is a collection
+00007aa0: 2073 696d 696c 6172 2074 6f20 5f45 7665   similar to _Eve
+00007ab0: 6e74 5472 6565 436f 6c6c 6563 7469 6f6e  ntTreeCollection
+00007ac0: 5f20 6275 7420 636f 6e74 6169 6e69 6e67  _ but containing
+00007ad0: 206f 6e6c 7920 7061 7265 6e74 2065 7665   only parent eve
+00007ae0: 6e74 7320 7468 6174 0a61 7265 2072 6566  nts that.are ref
+00007af0: 6572 656e 6365 6420 696e 2074 6865 2064  erenced in the d
+00007b00: 6174 6120 7374 7265 616d 2e20 5468 6520  ata stream. The 
+00007b10: 636f 6c6c 6563 7469 6f6e 2068 6173 2066  collection has f
+00007b20: 6561 7475 7265 7320 7369 6d69 6c61 7220  eatures similar 
+00007b30: 746f 205f 4576 656e 7454 7265 6543 6f6c  to _EventTreeCol
+00007b40: 6c65 6374 696f 6e5f 2e0a 0a44 6574 6169  lection_...Detai
+00007b50: 6c73 3a0a 0a2a 2054 6f20 7573 6520 4554  ls:..* To use ET
+00007b60: 2063 6f6c 6c65 6374 696f 6e73 2079 6f75   collections you
+00007b70: 206e 6565 6420 746f 2069 6e69 7469 616c   need to initial
+00007b80: 697a 6520 7468 656d 2062 7920 5f45 5443  ize them by _ETC
+00007b90: 4472 6976 6572 5f2e 2044 6174 6120 736f  Driver_. Data so
+00007ba0: 7572 6365 7320 7573 7561 6c6c 7920 7072  urces usually pr
+00007bb0: 6f76 6964 6520 7468 656d 2e0a 2020 596f  ovide them..  Yo
+00007bc0: 7520 6361 6e20 6372 6561 7465 2069 7420  u can create it 
+00007bd0: 6279 2079 6f75 7273 656c 6620 6465 7065  by yourself depe
+00007be0: 6e64 696e 6720 6f6e 2079 6f75 7220 6461  nding on your da
+00007bf0: 7461 2073 7472 7563 7475 7265 2e0a 2a20  ta structure..* 
+00007c00: 5468 6520 636f 6c6c 6563 7469 6f6e 2068  The collection h
+00007c10: 6173 2061 2066 6561 7475 7265 2074 6f20  as a feature to 
+00007c20: 7265 636f 7665 7220 6576 656e 7473 2e20  recover events. 
+00007c30: 416c 6c20 6576 656e 7473 2074 6861 7420  All events that 
+00007c40: 6172 6520 6e6f 7420 696e 2074 6865 2072  are not in the r
+00007c50: 6563 6569 7665 6420 6461 7461 2073 7472  eceived data str
+00007c60: 6561 6d2c 2062 7574 2077 6869 6368 2061  eam, but which a
+00007c70: 7265 0a20 2072 6566 6572 656e 6365 6420  re.  referenced 
+00007c80: 7769 6c6c 2062 6520 6c6f 6164 6564 2066  will be loaded f
+00007c90: 726f 6d20 7468 6520 6461 7461 2073 6f75  rom the data sou
+00007ca0: 7263 652e 0a2a 2059 6f75 2063 616e 2074  rce..* You can t
+00007cb0: 616b 6520 6064 6574 6163 6865 645f 6576  ake `detached_ev
+00007cc0: 656e 7473 6020 746f 2073 6565 2077 6869  ents` to see whi
+00007cd0: 6368 2065 7665 6e74 7320 6172 6520 6d69  ch events are mi
+00007ce0: 7373 696e 672e 0a2a 2049 6620 796f 7520  ssing..* If you 
+00007cf0: 7761 6e74 2c20 796f 7520 6361 6e20 6275  want, you can bu
+00007d00: 696c 6420 7061 7265 6e74 6c65 7373 2074  ild parentless t
+00007d10: 7265 6573 2077 6865 7265 2074 6865 206d  rees where the m
+00007d20: 6973 7369 6e67 2065 7665 6e74 7320 6172  issing events ar
+00007d30: 6520 7374 7562 6265 6420 696e 7374 6561  e stubbed instea
+00007d40: 642e 204a 7573 740a 2020 7573 6520 6067  d. Just.  use `g
+00007d50: 6574 5f70 6172 656e 746c 6573 735f 7472  et_parentless_tr
+00007d60: 6565 7328 2960 2e0a 0a52 6571 7569 7265  ees()`...Require
+00007d70: 6d65 6e74 733a 0a0a 312e 2045 7665 6e74  ments:..1. Event
+00007d80: 7320 7072 6f76 6964 6564 2074 6f20 4554  s provided to ET
+00007d90: 4320 6861 7665 2074 6f20 6861 7665 2060  C have to have `
+00007da0: 6576 656e 745f 6e61 6d65 602c 2060 6576  event_name`, `ev
+00007db0: 656e 745f 6964 602c 2060 7061 7265 6e74  ent_id`, `parent
+00007dc0: 5f65 7665 6e74 5f69 6460 2066 6965 6c64  _event_id` field
+00007dd0: 732e 2054 6865 790a 6361 6e20 6861 7665  s. They.can have
+00007de0: 2061 6e6f 7468 6572 206e 616d 6573 2028   another names (
+00007df0: 6974 2072 6573 6f6c 7665 7320 696e 2074  it resolves in t
+00007e00: 6865 2064 7269 7665 7229 2e0a 0a23 2323  he driver)...###
+00007e10: 2320 4869 6e74 730a 0a2a 2052 656d 6f76  # Hints..* Remov
+00007e20: 6520 616c 6c20 756e 6e65 6365 7373 6172  e all unnecessar
+00007e30: 7920 6669 656c 6473 2066 726f 6d20 6576  y fields from ev
+00007e40: 656e 7473 2062 6566 6f72 6520 7061 7373  ents before pass
+00007e50: 696e 6720 746f 2061 205f 636f 6c6c 6563  ing to a _collec
+00007e60: 7469 6f6e 5f20 746f 2072 6564 7563 6520  tion_ to reduce 
+00007e70: 6d65 6d6f 7279 2075 7361 6765 2e0a 2a20  memory usage..* 
+00007e80: 5573 6520 6073 686f 7728 2960 206d 6574  Use `show()` met
+00007e90: 686f 6420 746f 2070 7269 6e74 2074 6865  hod to print the
+00007ea0: 2074 7265 6520 696e 2074 7265 652d 6c69   tree in tree-li
+00007eb0: 6b65 2076 6965 772e 0a2a 204e 6f74 6520  ke view..* Note 
+00007ec0: 7468 6174 2074 6865 2060 6765 745f 7860  that the `get_x`
+00007ed0: 206d 6574 686f 6473 2077 696c 6c20 7261   methods will ra
+00007ee0: 6973 6520 616e 2065 7863 6570 7469 6f6e  ise an exception
+00007ef0: 2069 6620 796f 7520 7061 7373 2061 6e20   if you pass an 
+00007f00: 756e 6b6e 6f77 6e20 6576 656e 7420 6964  unknown event id
+00007f10: 2c20 756e 6c69 6b65 2074 6865 2060 6669  , unlike the `fi
+00007f20: 6e64 5f78 6020 6d65 7468 6f64 7320 280a  nd_x` methods (.
+00007f30: 2020 7468 6579 2072 6574 7572 6e20 4e6f    they return No
+00007f40: 6e65 292e 0a2a 2049 6620 796f 7520 7761  ne)..* If you wa
+00007f50: 6e74 2074 6f20 6b6e 6f77 2074 6861 7420  nt to know that 
+00007f60: 7370 6563 6966 6965 6420 6576 656e 7420  specified event 
+00007f70: 6578 6973 7473 2c20 7573 6520 7468 6520  exists, use the 
+00007f80: 7079 7468 6f6e 2060 696e 6020 6b65 7977  python `in` keyw
+00007f90: 6f72 6420 2865 2e67 2e20 6027 6576 656e  ord (e.g. `'even
+00007fa0: 742d 6964 2720 696e 2065 7665 6e74 735f  t-id' in events_
+00007fb0: 7472 6565 6029 2e0a 2a20 5573 6520 7468  tree`)..* Use th
+00007fc0: 6520 7079 7468 6f6e 2060 6c65 6e60 206b  e python `len` k
+00007fd0: 6579 776f 7264 2074 6f20 6765 7420 6576  eyword to get ev
+00007fe0: 656e 7473 206e 756d 6265 7220 696e 2074  ents number in t
+00007ff0: 6865 2074 7265 652e 0a0a 2323 2320 4669  he tree...### Fi
+00008000: 656c 6420 5265 736f 6c76 6572 730a 496e  eld Resolvers.In
+00008010: 7465 7266 6163 6520 6361 6e20 6265 2066  terface can be f
+00008020: 6f75 6e64 2069 6e20 6074 6832 5f64 6174  ound in `th2_dat
+00008030: 615f 7365 7276 6963 6573 2f69 6e74 6572  a_services/inter
+00008040: 6661 6365 732f 7574 696c 732f 7265 736f  faces/utils/reso
+00008050: 6c76 6572 2e70 7960 2e20 200a 416c 6c20  lver.py`.  .All 
+00008060: 6461 7461 2d73 6f75 7263 6573 2073 686f  data-sources sho
+00008070: 756c 6420 696d 706c 656d 656e 7420 7468  uld implement th
+00008080: 656d 2e0a 0a54 6865 2069 6465 6120 6f66  em...The idea of
+00008090: 2075 7369 6e67 2072 6573 6f6c 7665 7273   using resolvers
+000080a0: 3a0a 4974 2073 6f6c 7665 7320 7468 6520  :.It solves the 
+000080b0: 7072 6f62 6c65 6d20 6f66 2068 6176 696e  problem of havin
+000080c0: 6720 6120 6665 7720 4461 7461 536f 7572  g a few DataSour
+000080d0: 6365 7320 7769 7468 2073 696d 696c 6172  ces with similar
+000080e0: 2064 6174 612c 0a62 7574 2077 6974 6820   data,.but with 
+000080f0: 6469 6666 6572 656e 7420 7761 7973 2074  different ways t
+00008100: 6f20 6765 7420 6974 2e0a 0a54 6865 7365  o get it...These
+00008110: 2063 6c61 7373 6573 2070 726f 7669 6465   classes provide
+00008120: 2079 6f75 2067 6574 7465 7220 6d65 7468   you getter meth
+00008130: 6f64 732e 0a55 7369 6e67 2074 6865 7365  ods..Using these
+00008140: 2063 6c61 7373 6573 2061 6c6c 6f77 7320   classes allows 
+00008150: 796f 7520 746f 2066 7265 656c 7920 7377  you to freely sw
+00008160: 6974 6368 2062 6574 7765 656e 2064 6966  itch between dif
+00008170: 6665 7265 6e74 2064 6174 610a 666f 726d  ferent data.form
+00008180: 6174 7320 616e 6420 646f 6e27 7420 6368  ats and don't ch
+00008190: 616e 6765 2079 6f75 7220 636f 6465 2e0a  ange your code..
+000081a0: 0a52 6573 6f6c 7665 7273 2073 6f6c 7665  .Resolvers solve
+000081b0: 2074 6865 2070 726f 626c 656d 206f 6620   the problem of 
+000081c0: 6461 7461 2d66 6f72 6d61 7420 6d69 6772  data-format migr
+000081d0: 6174 696f 6e2e 0a2d 2066 6965 6c64 7320  ation..- fields 
+000081e0: 706c 6163 6520 6361 6e20 6265 2063 6861  place can be cha
+000081f0: 6e67 6564 0a2d 2066 6965 6c64 7320 6e61  nged.- fields na
+00008200: 6d65 7320 6361 6e20 6265 2063 6861 6e67  mes can be chang
+00008210: 6564 0a0a 5265 736f 6c76 6572 7320 6361  ed..Resolvers ca
+00008220: 6e20 776f 726b 206f 6e6c 7920 7769 7468  n work only with
+00008230: 206f 6e65 2065 7665 6e74 2f6d 6573 7361   one event/messa
+00008240: 6765 2e0a 4974 206d 6561 6e73 2c20 6966  ge..It means, if
+00008250: 2079 6f75 7220 6d65 7373 6167 6520 6861   your message ha
+00008260: 7320 7375 622d 6d65 7373 6167 6573 2028  s sub-messages (
+00008270: 6c69 6b65 2074 6832 2d6d 6573 7361 6765  like th2-message
+00008280: 7320 696e 206c 7764 7029 2069 7420 0a77  s in lwdp) it .w
+00008290: 6f6e 2774 2077 6f72 6b2c 2062 6563 6175  on't work, becau
+000082a0: 7365 2072 6573 6f6c 7665 7220 7769 6c6c  se resolver will
+000082b0: 206e 6f74 206b 6e6f 7720 7769 7468 2077   not know with w
+000082c0: 6869 6368 2073 7562 2d6d 6573 7361 6765  hich sub-message
+000082d0: 2073 686f 756c 6420 6974 2077 6f72 6b2e   should it work.
+000082e0: 200a 0a2a 2a57 6f72 6b61 726f 756e 642a   ..**Workaround*
+000082f0: 2a20 200a 312e 2045 7870 616e 6420 616c  *  .1. Expand al
+00008300: 6c20 796f 7572 206d 6573 7361 6765 7320  l your messages 
+00008310: 2d3e 2060 6e65 775f 6420 3d20 796f 7572  -> `new_d = your
+00008320: 5f64 6174 612e 6d61 7028 4d65 7373 6167  _data.map(Messag
+00008330: 6546 6965 6c64 5265 736f 6c76 6572 2e65  eFieldResolver.e
+00008340: 7870 616e 645f 6d65 7373 6167 6529 600a  xpand_message)`.
+00008350: 322e 2055 7365 2060 4578 7061 6e64 6564  2. Use `Expanded
+00008360: 4d65 7373 6167 6546 6965 6c64 5265 736f  MessageFieldReso
+00008370: 6c76 6572 6020 696e 7374 6561 6420 6f66  lver` instead of
+00008380: 2075 7375 616c 2060 4d65 7373 6167 6546   usual `MessageF
+00008390: 6965 6c64 5265 736f 6c76 6572 6020 7768  ieldResolver` wh
+000083a0: 656e 200a 2020 2020 796f 7520 7461 6b65  en .    you take
+000083b0: 2066 6965 6c64 7320 666f 7220 6578 7061   fields for expa
+000083c0: 6e64 6564 206d 6573 7361 6765 732e 0a0a  nded messages...
+000083d0: 2a2a 496d 706c 656d 656e 7461 7469 6f6e  **Implementation
+000083e0: 2061 6476 6963 653a 2a2a 0a31 2e20 7261   advice:**.1. ra
+000083f0: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
+00008400: 6564 4572 726f 7220 2d2d 2069 6620 796f  edError -- if yo
+00008410: 7572 2049 6d70 6c65 6d65 6e74 6174 696f  ur Implementatio
+00008420: 6e20 646f 6573 6e27 7420 7375 7070 6f72  n doesn't suppor
+00008430: 7420 7468 6973 2067 6574 7465 722e 0a0a  t this getter...
+00008440: 2a2a 5065 7266 6f72 6d61 6e63 6520 696d  **Performance im
+00008450: 7061 6374 3a2a 2a0a 2d20 4974 2061 2062  pact:**.- It a b
+00008460: 6974 2073 6c6f 7765 7220 7468 616e 2075  it slower than u
+00008470: 7369 6e67 206e 616b 6564 2066 6965 6c64  sing naked field
+00008480: 2061 6363 6573 7320 6064 6963 745b 276b   access `dict['k
+00008490: 6579 275d 602e 0a0a 2323 2032 2e34 2e20  ey']`...## 2.4. 
+000084a0: 4c69 6e6b 730a 0a2d 205b 5265 706f 7274  Links..- [Report
+000084b0: 2044 6174 6120 5072 6f76 6964 6572 5d28   Data Provider](
+000084c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000084d0: 6f6d 2f74 6832 2d6e 6574 2f74 6832 2d72  om/th2-net/th2-r
+000084e0: 7074 2d64 6174 612d 7072 6f76 6964 6572  pt-data-provider
+000084f0: 290a 2d20 5b54 6832 2044 6174 6120 5365  ).- [Th2 Data Se
+00008500: 7276 6963 6573 2055 7469 6c73 5d28 6874  rvices Utils](ht
+00008510: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00008520: 2f74 6832 2d6e 6574 2f74 6832 2d64 6174  /th2-net/th2-dat
+00008530: 612d 7365 7276 6963 6573 2d75 7469 6c73  a-services-utils
+00008540: 290a 0a23 2033 2e20 4265 7374 2070 7261  )..# 3. Best pra
+00008550: 6374 6963 6573 0a44 6570 656e 6469 6e67  ctices.Depending
+00008560: 206f 6e20 686f 7720 796f 7520 776f 726b   on how you work
+00008570: 2077 6974 6820 6044 6174 6120 6f62 6a65   with `Data obje
+00008580: 6374 602c 2069 7420 6361 6e20 6265 2073  ct`, it can be s
+00008590: 6c6f 7720 6f66 2066 6173 742e 0a41 7320  low of fast..As 
+000085a0: 7769 7468 2061 2072 656c 6174 696f 6e61  with a relationa
+000085b0: 6c20 6461 7461 6261 7365 2c20 796f 7520  l database, you 
+000085c0: 6361 6e20 7772 6974 6520 6120 7175 6572  can write a quer
+000085d0: 7920 7468 6174 2077 696c 6c20 7265 7475  y that will retu
+000085e0: 726e 2064 6174 6120 736c 6f77 6c79 206f  rn data slowly o
+000085f0: 7220 7175 6963 6b6c 792c 0a74 6865 2073  r quickly,.the s
+00008600: 616d 6520 7768 656e 2077 6f72 6b69 6e67  ame when working
+00008610: 2077 6974 6820 6120 6044 6174 6120 6f62   with a `Data ob
+00008620: 6a65 6374 602e 0a0a 466f 6c6c 6f77 2074  ject`...Follow t
+00008630: 6865 2072 756c 6573 2074 6f20 6d61 6b65  he rules to make
+00008640: 2079 6f75 7220 776f 726b 2077 6974 6820   your work with 
+00008650: 4461 7461 206f 626a 6563 7420 6661 7374  Data object fast
+00008660: 3a0a 312e 2055 7365 2060 4461 7461 2e75  :.1. Use `Data.u
+00008670: 7365 5f63 6163 6865 2829 6020 6966 2079  se_cache()` if y
+00008680: 6f75 2069 7465 7261 7465 2064 6174 6120  ou iterate data 
+00008690: 6d6f 7265 2074 6861 6e20 6f6e 6520 7469  more than one ti
+000086a0: 6d65 2e0a 322e 2054 7279 2074 6f20 646f  me..2. Try to do
+000086b0: 6e27 7420 6974 6572 6174 6520 6f6e 6520  n't iterate one 
+000086c0: 6044 6174 6120 6f62 6a65 6374 6020 696e  `Data object` in
+000086d0: 7369 6465 2074 6865 206f 7468 6572 206f  side the other o
+000086e0: 6e65 2e0a 2020 2049 6620 796f 7520 7368  ne..   If you sh
+000086f0: 6f75 6c64 2074 6f20 646f 2069 742c 2075  ould to do it, u
+00008700: 7365 2073 686f 7274 2060 4461 7461 206f  se short `Data o
+00008710: 626a 6563 7460 2066 6972 7374 2061 6e64  bject` first and
+00008720: 206c 6f6e 6720 6044 6174 6120 6f62 6a65   long `Data obje
+00008730: 6374 6020 696e 7369 6465 2074 6865 206c  ct` inside the l
+00008740: 6f6f 702e 0a20 2020 4974 276c 6c20 616c  oop..   It'll al
+00008750: 6c6f 7720 796f 7520 6f70 656e 2074 6865  low you open the
+00008760: 2063 6163 6865 2066 696c 6520 6f72 2063   cache file or c
+00008770: 7265 6174 6520 6120 7265 7175 6573 7420  reate a request 
+00008780: 746f 2060 4461 7461 2073 6f75 7263 6560  to `Data source`
+00008790: 206c 6573 7320 6e75 6d62 6572 206f 6620   less number of 
+000087a0: 7469 6d65 732e 0a0a 2320 342e 204f 6666  times...# 4. Off
+000087b0: 6963 6961 6c20 4461 7461 536f 7572 6365  icial DataSource
+000087c0: 2069 6d70 6c65 6d65 6e74 6174 696f 6e73   implementations
+000087d0: 0a0a 2d20 5b4c 6967 6874 7765 6967 6874  ..- [Lightweight
+000087e0: 2044 6174 6120 5072 6f76 6964 6572 2044   Data Provider D
+000087f0: 6174 6120 536f 7572 6365 5d28 6874 7470  ata Source](http
+00008800: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
+00008810: 6832 2d6e 6574 2f74 6832 2d64 732d 736f  h2-net/th2-ds-so
+00008820: 7572 6365 2d6c 7764 7029 0a0a 0a23 2035  urce-lwdp)...# 5
+00008830: 2e20 4150 490a 0a49 6620 796f 7520 6172  . API..If you ar
+00008840: 6520 6c6f 6f6b 696e 6720 666f 7220 636c  e looking for cl
+00008850: 6173 7365 7320 6465 7363 7269 7074 696f  asses descriptio
+00008860: 6e20 7365 6520 7468 6520 5b41 5049 2044  n see the [API D
+00008870: 6f63 756d 656e 7461 7469 6f6e 5d28 646f  ocumentation](do
+00008880: 6375 6d65 6e74 6174 696f 6e2f 6170 692f  cumentation/api/
+00008890: 696e 6465 782e 6d64 292e 0a0a 2320 362e  index.md)...# 6.
+000088a0: 2045 7861 6d70 6c65 730a 0a2d 205b 6765   Examples..- [ge
+000088b0: 745f 7374 6172 7465 645f 6578 616d 706c  t_started_exampl
+000088c0: 652e 7079 5d28 6578 616d 706c 6573 2f67  e.py](examples/g
+000088d0: 6574 5f73 7461 7274 6564 5f65 7861 6d70  et_started_examp
+000088e0: 6c65 2e70 7929 0a                        le.py).
```

### Comparing `th2_data_services-2.0.0.dev8662586819/setup.py` & `th2_data_services-2.0.0.dev8702324290/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/_internal/__init__.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/_internal/perf_tests.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/_internal/perf_tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 
 @calculate_time(return_as_last_value=True)
 def _build_cache_file(data_obj: Data, filename):
     ftype = filename.split(".")[-1]
     if ftype == "pickle":
         data_obj.build_cache(filename)
     elif ftype == "jsons":
-        data_obj.to_jsons(filename)
+        data_obj.to_json_lines(filename)
     elif ftype == "gz":
-        data_obj.to_jsons(filename, gzip=True)
+        data_obj.to_json_lines(filename, gzip=True)
 
 
 def _read_from_cache_file(filename):
     ftype = filename.split(".")[-1]
     if ftype == "pickle":
         return Data.from_cache_file(filename)
     elif ftype == "jsons":
@@ -42,34 +42,42 @@
 
 @calculate_time(return_as_last_value=True)
 def _iter_data_obj(do: Data):
     for o in do:
         pass
 
 
+@calculate_time(return_as_last_value=True)
+def _iter_data_obj_with_3_filters(do: Data):
+    for o in do.filter(lambda x: True).filter(lambda x: True).filter(lambda x: True):
+        pass
+
+
 def _test_xx(data_obj: Data):
     filenames = ["cache_test.pickle", "cache_test.jsons", "cache_test.jsons.gz"]
 
     try:
-        data_obj.use_cache()
+        # data_obj.use_cache()
         do_len = data_obj.len
 
         print("Store cache files for test:")
         for filename in filenames:
             print(f"  -> {filename}", end="")
             val, calc_time = _build_cache_file(data_obj, filename)
             print(f"  --  {calc_time} s")
 
         print()
         print(f"Data length: {do_len}")
         for filename in filenames:
             print(f"Iterate {'.'.join(filename.split('.')[1:])}:", end="")
             data_obj_file = _read_from_cache_file(filename)
             _, calc_time = _iter_data_obj(data_obj_file)
-            print(f"  --  {calc_time} s")
+            print(f"  --  {calc_time} s", end="")
+            _, calc_time = _iter_data_obj_with_3_filters(data_obj_file)
+            print(f", with 3 filters  --  {calc_time} s")
 
         print()
 
     except:
         print("\nException")
         print("Remove cache files")
         for filename in filenames:
@@ -112,16 +120,16 @@
         arg = sys.argv[1]
         cache_files_reading_speed(arg)
     else:
         # cache_files_reading_speed()
         # cache_files_reading_speed(
         #     data=Data([1, 2, 3, 4, 5, 6, 7, 8, 9, 0])
         # )
-        cache_files_reading_speed(
-            data=Data.from_cache_file(
-                "C:/Users/admin/exactpro/prj/th2/pickles/cache_2.5kk_events.pickle"
-            ).limit(5)
-        )
-
         # cache_files_reading_speed(
+        #     data=Data.from_cache_file(
         #         "C:/Users/admin/exactpro/prj/th2/pickles/cache_2.5kk_events.pickle"
+        #     ).limit(5)
         # )
+
+        cache_files_reading_speed(
+            "C:/Users/admin/exactpro/prj/th2/pickles/cache_2.5kk_events.pickle"
+        )
```

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/config/__init__.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/config/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/config/config.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/config/config.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/data.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 from th2_data_services.utils.path_utils import check_if_filename_valid, check_if_file_exists
 from deprecated.classic import deprecated
 
 
 DataIterValues = TypeVar("DataIterValues")
 DataGenerator = Generator[DataIterValues, None, None]
 DataSet = Union[Iterator, Callable[..., DataGenerator], List[Iterable], Iterable]
-WorkFlow = List[Dict[str, Union[Callable, str]]]
 
 
 def _build_limit_callback(num) -> Callable:
     def callback(r):
         callback.pushed += 1
         if callback.pushed > num:
             raise StopIteration(r)
@@ -85,24 +84,24 @@
 
 
 @dataclass
 class WfLimitRecord(WfRecord):
     limit: int
 
 
-class Workflow:
+class DataWorkflow:
     def __init__(self):
         """Data object workflow."""
         self._data: List[WfRecord] = []
 
     def __bool__(self):
         return bool(self._data)
 
     def __str__(self):
-        return f"Workflow({pprint.pformat(self._data)})"
+        return f"DataWorkflow({pprint.pformat(self._data)})"
 
     def __repr__(self):
         return str(self)
 
     def add(self, wfr: WfRecord):
         """Add callback to workflow.
 
@@ -114,23 +113,15 @@
         """
         self._data.append(wfr)
         return self
 
     # def update(self, upd_func: Callable[[List[WfRecord]], List[WfRecord]]):
     #     self._data = upd_func(self._data)
 
-    # def _apply_record(self, record):
-    #     for wfr in self._data:
-    #         # print(f"apply '{wfr.type}' for '{record}'")
-    #         record = wfr.callback(record)
-    #         # print(f"\t --> '{record}'")
-    #
-    #     return record
-
-    def apply_records(self, records):
+    def apply_records(self, records: Iterator):
         """Execute workflow against some stream.
 
         Args:
             records: some stream.
 
         Yields:
             workflow-handled records.
@@ -151,34 +142,14 @@
         several times in the loops.
         """
         for wfr in self._data:
             if isinstance(wfr, WfLimitRecord):
                 wfr.callback = _build_limit_callback(wfr.limit)
 
 
-# TODO
-#   Хочется уметь менять состояние дата объекта во время итерации
-
-
-# def show_message_if_exception_decorator(callback):
-#     def wrapper(stream):
-#         try:
-#             for record in stream:
-#                 yield from callback(stream)
-#         except Exception:
-#             try:
-#                 print("Exception during handling the message: \n" f"{pprint.pformat(record)}")
-#             except UnboundLocalError:
-#                 pass
-#
-#             raise
-#
-#     return wrapper
-
-
 class Data(Generic[DataIterValues]):
     """A wrapper for data/data_stream.
 
     The class provides methods for working with data as a stream.
 
     Such an approach to data analysis called streaming transformation.
     """
@@ -204,27 +175,27 @@
                 "are iterates only once. "
                 "Expected data types: Iterator, Callable[..., DataGenerator], List[Iterator]",
                 RuntimeWarning,
                 stacklevel=2,
             )
 
         if self._is_iterables_list(data):
-            self._data_stream = self._create_data_set_from_iterables(data)
+            self._data_source = self._create_data_set_from_iterables(data)
         else:
-            self._data_stream = data
+            self._data_source = data
 
         self._id = id(self)
         self._cache_filename = f"{self._id}_{time()}.pickle"
         self._cache_path = Path("temp", self._cache_filename).resolve().absolute()
         self._pending_cache_path = (
             self._cache_path.with_name("[PENDING]" + self._cache_filename).resolve().absolute()
         )
         self._cache_file_obj = None
         self._len = None
-        self.workflow = Workflow()
+        self.workflow = DataWorkflow()
 
         self._length_hint = None  # The value is populated when we use limit method.
         self._cache_status = cache
         # We use finalize instead of __del__ because __del__ won't be executed sometimes.
         # Read more about __del__ problems here: https://stackoverflow.com/a/2452895
         self._finalizer = finalize(self, self.__remove)
         # LOG         self._logger = _DataLogger(logger, {"id": self._id})
@@ -283,25 +254,37 @@
 
     def _copy_cache_file(self, new_name):
         from shutil import copy2
 
         copy2(self.get_cache_filepath(), new_name)
 
     def __copy__(self):
-        obj = Data(self._data_stream, pickle_version=self._pickle_version)
+        if self._cache_status and self.is_cache_file_exists():
+
+            def read_from_existed_cache():
+                if self.is_cache_file_exists():
+                    yield from self.__load_file(self.get_cache_filepath())
+                else:
+                    yield from self._build_data_source()
+
+            data_source = read_from_existed_cache
+        else:
+            data_source = self._data_source
+
+        obj = Data(data_source, pickle_version=self._pickle_version)
         obj._set_metadata(self.metadata)
         obj.workflow = copy.deepcopy(self.workflow)
 
         return obj
 
     def __remove(self):
         """Data class destructor."""
-        if self.__is_cache_file_exists() and not self._read_from_external_cache_file:
+        if self.is_cache_file_exists() and not self._read_from_external_cache_file:
             self.__delete_cache()
-        del self._data_stream
+        del self._data_source
 
     def __delete_cache(self) -> None:
         """Removes cache file."""
         path = self.get_cache_filepath()
         if path.exists():
             # LOG             self._logger.debug("Deleting cache file '%s'" % path)
             path.unlink()
@@ -344,15 +327,15 @@
         else:
             # 2**13, though 8 - is a default value in CPython.
             # We usually have large number of data.
             return 8192
 
     def _iter_logic(self):
         interruption = True
-        if self._cache_status and self.__is_cache_file_exists():
+        if self._cache_status and self.is_cache_file_exists():
             is_data_writes_cache = False
         else:
             # FIXME -- bug -- мы считаем что мы пишем файл, когда он уже существует а мы его просто читаем
             is_data_writes_cache = True
 
         try:
             for record in self.__load_data(self._cache_status):
@@ -402,54 +385,54 @@
             for record in self._iter_logic():
                 self._len += 1
                 yield record
         else:
             # Do not calculate self._len if it is not None.
             yield from self._iter_logic()
 
-    def _build_workflow(self, workflow: Workflow):
+    def _build_workflow(self, workflow: DataWorkflow):
         """Updates limit callbacks each time when Data object is iterated.
 
         It used to have the possibility to iterate the same Data object
         several times in the loops.
         """
         new_workflow = copy.deepcopy(workflow)
         new_workflow.refresh_limit_callbacks()
 
         return new_workflow
 
-    def _build_data_stream(self):
-        return self._data_stream() if callable(self._data_stream) else self._data_stream
+    def _build_data_source(self):
+        return self._data_source() if callable(self._data_source) else self._data_source
 
     def __load_data(self, cache: bool) -> DataGenerator:
         """Loads data from cache or data.
 
         Args:
             cache: Flag if you what to write and read from cache.
 
         Returns:
             obj: Generator
         """
-        if cache and self.__is_cache_file_exists():
+        if cache and self.is_cache_file_exists():
             # LOG             self._logger.info("Iterating using own cache file '%s'" % self.get_cache_filepath())
-            data_stream = self.__load_file(self.get_cache_filepath())
-            yield from data_stream
+            data_source = self.__load_file(self.get_cache_filepath())
+            yield from data_source
         else:
-            data_stream = self._build_data_stream()  # we do it for every iterable data object.
+            data_source = self._build_data_source()  # we do it for every iterable data object.
             workflow = self._build_workflow(self.workflow)
 
             if self.__check_file_recording():
                 # Do not read from the cache file if it has PENDING status (if the file is not filled yet).
                 # It used to handle case when Data object iterates in the loop several times.
                 cache = False
 
             if workflow:
-                iteration_obj = workflow.apply_records(data_stream)
+                iteration_obj = workflow.apply_records(data_source)
             else:
-                iteration_obj = data_stream
+                iteration_obj = data_source
 
             if cache:
                 filepath = self.get_pending_cache_filepath()
                 filepath.parent.mkdir(exist_ok=True)
                 # LOG             self._logger.debug("Recording cache file '%s'" % filepath)
                 self._cache_file_obj = open(filepath, "wb")
 
@@ -470,78 +453,32 @@
 
         Returns:
             bool: File recording status.
         """
         path = self.get_pending_cache_filepath()
         return path.is_file()
 
-    def __is_cache_file_exists(self) -> bool:
-        """Checks whether cache file exist."""
+    def is_cache_file_exists(self) -> bool:
+        """Returns whether cache file exists or not."""
         path = self.get_cache_filepath()
         r = path.is_file()
         # LOG         self._logger.debug("Cache file exists" if r else "Cache file doesn't exist")
         return r
 
     def __load_file(self, filepath: Path) -> DataGenerator:
         """Loads records from pickle file.
 
         Args:
             filepath: Filepath.
 
         Yields:
             obj: Generator records.
         """
-        if not filepath.exists():
-            raise FileNotFoundError(f"{filepath} doesn't exist")
-
-        if not filepath.is_file():
-            raise FileExistsError(f"{filepath} isn't file")
-
+        check_if_file_exists(filepath)
         yield from _iter_pickle_file_logic(filepath)
-        # with open(filepath, "rb") as file:
-        #     while True:
-        #         try:
-        #             decoded_data = pickle.load(file)
-        #             yield decoded_data
-        #         except EOFError:
-        #             break
-        #         except pickle.UnpicklingError:
-        #             print(f"Cannot read {filepath} cache file")
-        #             raise
-
-    # def _process_step(self, step: dict, record):
-    #     res = step["callback"](record)
-    #     # LOG         self._logger.debug("    - step '%s' -> %s", step["type"], res)
-    #     return res
-
-    # def __apply_workflow(
-    #     self, record: Any, workflow: WorkFlow
-    # ) -> Optional[Union[dict, List[dict]]]:
-    #     """Creates generator records with apply workflow.
-    #
-    #     Returns:
-    #         obj: Generator records.
-    #
-    #     """
-    #     # LOG         self._logger.debug("Apply workflow for %s", record)
-    #     for step in workflow:
-    #         try:
-    #             # TODO -2 -- мы каждый раз делаем step["callback"](record)
-    #             # TODO -3 -- по факту мы сейчас не используем воркфлоу, а ка
-    #             #  каждый раз создаём новый дата объект
-    #             #   у этого есть минусы -- эксепшен с итерациями,
-    #             #   и когда много объектов вложены доуг в друга, это медленно работает
-    #             record = self._process_step(step, record)
-    #             if record is None:
-    #                 break  # Break workflow iteration if step result is None.
-    #         except StopIteration:
-    #             raise
-    #
-    #     # LOG         self._logger.debug("-> %s", record)
-    #     return record
 
     @property
     def metadata(self):
         return self.__metadata
 
     @property
     def len(self) -> int:
@@ -799,28 +736,73 @@
             file: Path to file.
 
         """
         with open(file, "w") as txt_file:
             for record in self:
                 txt_file.write(f"{pprint.pformat(record)}\n" + ("-" * 50) + "\n")
 
-    def show(self, n=5, print_=True):
-        print("------------- Printed first 5 records -------------")
-        for index, record in enumerate(self):
-            if index == n:
+    def _show_print_one_line(self, index, idx_print, extra_prints: dict, record):
+        if idx_print:
+            print(f"[{index}] ------")
+
+        for field_name, func in extra_prints.items():
+            try:
+                val = func(record)
+            except Exception as e:
+                val = f"FUNC_ERROR ({e})"
+            print(f"{field_name}: {val}")
+
+        pprint.pprint(record)
+
+    def show(
+        self, n: int = 5, idx_print: bool = True, extra_prints: Optional[Dict[str, Callable]] = None
+    ):
+        """Prints first N records in human-readable format.
+
+        Args:
+            n: number of elements to print.
+                Use -1, if you want to print the whole stream.
+            idx_print:
+                - True - will print message index before the message (Default)
+                - False - will Not print message index before the message
+            extra_prints:
+                Sometimes you want to highlight some fields in the message.
+                This parameter allows you to do this.
+                It will print extra print before the message.
+                E.g.:
+                    extra_prints = {
+                        'SendingTime': get_sending_time_human_func,
+                        'TransactTime': get_sending_time_human_func,
+                    }
+
+        Returns:
+            None
+        """
+        if extra_prints is None:
+            extra_prints = {}
+
+        if n == -1:
+            print(f"------------- Printed all stream records -------------")
+            for index, record in enumerate(self, start=1):
+                self._show_print_one_line(index, idx_print, extra_prints, record)
+
+        print(f"------------- Printed first {n} records -------------")
+        for index, record in enumerate(self, start=1):
+            if index > n:
                 break
-            pprint.pprint(record)
+
+            self._show_print_one_line(index, idx_print, extra_prints, record)
 
     def build_cache(self, filename, pickle_version: Optional[int] = None):
         """Creates cache file with provided name.
 
         Important:
             If the Data object cache status is True, it'll iterate itself. As a result the cache file
              will be created and copied.
-            When you will iterate the Data object next time, it'll iterate created cache file.
+            When you iterate the Data object next time, it'll iterate created cache file.
 
             NOTE! If you build cache file, Data.cache_status was False and after that you'll set
              Data.cache_status == TRUE -- the Data object WON'T iterate build file because it doesn't
              keep the path to built cache file..
 
         Args:
             filename: Name or path to cache file.
@@ -832,15 +814,15 @@
         status, reason = check_if_filename_valid(path_name)
         if not status:
             raise Exception(f"Cannot build cache file. {reason}")
 
         if pickle_version is None:
             pickle_version = self._pickle_version
 
-        if self.__is_cache_file_exists():
+        if self.is_cache_file_exists():
             self._copy_cache_file(filename)
         else:
             gc.disable()  # https://exactpro.atlassian.net/browse/TH2-4775
             if self._cache_status:
                 _ = self.len  # Just to iterate
                 self._copy_cache_file(filename)
             else:
@@ -856,15 +838,15 @@
         """Clears related to data object cache file.
 
         This function won't remove external cache file.
         """
         if self._read_from_external_cache_file:
             raise Exception("It's not possible to remove external cache file via this method")
         else:
-            if self.__is_cache_file_exists():
+            if self.is_cache_file_exists():
                 self.__delete_cache()
 
     @classmethod
     def from_cache_file(cls, filename, pickle_version: int = o.DEFAULT_PICKLE_VERSION) -> "Data":
         """Creates Data object from cache file with the provided name.
 
         Args:
@@ -878,15 +860,15 @@
         Raises:
             FileNotFoundError if provided file does not exist.
 
         """
         check_if_file_exists(filename)
 
         path = Path(filename).resolve()
-        data_obj = cls(_iter_pickle_cache_file(path, pickle_version))
+        data_obj = cls(_iter_pickle_cache_builder(path))
         data_obj.update_metadata({"source_file": path})
         data_obj._pickle_version = pickle_version
         return data_obj
 
     @classmethod
     def from_json(cls, filename, buffer_limit=250, gzip=False) -> "Data[dict]":
         """Creates Data object from json-lines file with provided name.
@@ -965,15 +947,14 @@
         Returns:
             Data: Data object.
 
         Raises:
             FileNotFoundError if provided file does not exist.
 
         """
-        # TODO - bug here TH2-4930 - new data object doesn't work with limit method
         check_if_file_exists(filename)
         data = cls(_iter_csv(filename, header, header_first_line, mode, delimiter))
         data.update_metadata({"source_file": filename})
         return data
 
     def _set_metadata(self, metadata: Dict) -> None:
         """Set metadata of object to metadata argument.
@@ -1201,13 +1182,13 @@
             except EOFError:
                 break
             except pickle.UnpicklingError:
                 print(f"Cannot read {filepath} cache file")
                 raise
 
 
-def _iter_pickle_cache_file(filepath: Path, pickle_version: int):
-    def iter_json_file_wrapper(*args, **kwargs):
+def _iter_pickle_cache_builder(filepath: Path):
+    def iter_pickle_cache(*args, **kwargs):
         """Wrapper function that allows passing arguments to the generator."""
         return _iter_pickle_file_logic(filepath)
 
-    return iter_json_file_wrapper
+    return iter_pickle_cache
```

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/__init__.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/etc_driver.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/event_tree.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/event_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,26 +216,31 @@
         """
         try:
             for child in self._tree.children(id):
                 yield child.data
         except NodeIDAbsentError:
             raise EventIdNotInTree(id)
 
-    def get_parent(self, id: str) -> Th2Event:
+    def get_parent(self, id: str) -> Optional[Th2Event]:
         """Returns a parent for the event by its id.
 
+        Returns None if the provided ID is a root of the tree.
+
         Args:
             id: Event id.
 
         Raises:
             EventIdNotInTree: If event id is not in the tree.
         """
         try:
             parent = self._tree.parent(id)
 
+            if self.get_root_id() == id:
+                return None
+
             if parent is None:
                 raise EventIdNotInTree(id)
 
             return parent.data
         except NodeIDAbsentError:
             raise EventIdNotInTree(id)
```

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/event_tree_collection.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/event_tree_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,15 +417,16 @@
                 except EventIdNotInTree:
                     continue
         raise EventIdNotInTree(id)
 
     def get_children_iter(self, id: str) -> Generator[Th2Event, None, None]:
         """Yields children of the event by its id.
 
-        This method applicable only for trees (regular or parentless), not for detached events.
+        This method is applicable only for trees (regular or parentless),
+        not for detached events.
 
         Args:
             id: Event id.
 
         Raises:
             EventIdNotInTree: If event id is not in the trees.
         """
@@ -442,22 +443,24 @@
                     yield from tree.get_children_iter(id)
                     is_iter = True
                 except EventIdNotInTree:
                     continue
         if not is_iter:
             raise EventIdNotInTree(id)
 
-    def get_parent(self, id: str) -> Th2Event:
+    def get_parent(self, id: str) -> Optional[Th2Event]:
         """Returns a parent of the event by its id.
 
+        Returns None if the provided ID is a root of any of the trees in ETC.
+
         Args:
             id: Event id.
 
         Raises:
-            NodeIDAbsentError: If event id is not in the trees.
+            EventIdNotInTree: If event id is not in the tree.
         """
         for tree in self._roots:
             try:
                 return tree.get_parent(id)
             except EventIdNotInTree:
                 continue
         if self._detached_nodes:
@@ -471,14 +474,15 @@
                     return event
         if self._parentless is not None:
             for tree in self._parentless:
                 try:
                     return tree.get_parent(id)
                 except EventIdNotInTree:
                     continue
+
         raise EventIdNotInTree(id)
 
     def get_full_path(self, id: str, field: str = None) -> List[Union[str, Th2Event]]:  # noqa: D412
         """Returns the full path for the event by its id in the right order.
 
         This method applicable only for trees (regular or parentless), not for detached events.
 
@@ -708,15 +712,15 @@
             preprocessor: the function that will be executed for each recovered event before store.
 
         """
         previous_detached_events = list(self._detached_parent_ids())
         while previous_detached_events:
             events = self._driver.get_events_by_id_from_source(ids=self._detached_parent_ids())
             if preprocessor is not None:
-                events = preprocessor(preprocessor)
+                events = preprocessor(events)
 
             for event in events:
                 if not self._driver.get_event_name(event) == self._driver.stub_event_name():
                     self.append_event(event)
 
             dp_ids = list(self._detached_parent_ids())
             if previous_detached_events == dp_ids:
```

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/exceptions.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/parent_event_tree_collection.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/parent_event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/exceptions.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/__init__.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/adapter.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/command.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/data_source.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/source_api.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/struct.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/stub_builder.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/utils/__init__.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/utils/converter.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/utils/converter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/utils/resolver.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/utils/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/_is_sorted_result.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/_is_sorted_result.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/_json.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/_json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/_types.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/_types.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/aggregation_classes.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/aggregation_classes.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/az_tree.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/az_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/categorizers.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/categorizers.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/category.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/category.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/converters.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/converters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/decode_error_handler.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/decode_error_handler.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/display.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/__init__.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/display.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/event_utils.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/event_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/frequencies.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/select.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/select.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/totals.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/totals.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/experimental.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/experimental.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/json_tree.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/json_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/message_utils/__init__.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/message_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/message_utils/frequencies.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/message_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/message_utils/message_utils.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/message_utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/misc_utils.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/path_utils.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/path_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,17 +73,21 @@
     Args:
         filename: string.
 
     Raises:
         FileNotFoundError: if file doesn't exist.
         ValueError: if filename contains illegal characters.
     """
+    fp = Path(filename).resolve()
     try:
-        if not Path(filename).resolve().exists():
-            raise FileNotFoundError(f"{filename} doesn't exist")
+        if not fp.exists():
+            raise FileNotFoundError(f"{fp} doesn't exist")
+
+        if not fp.is_file():
+            raise FileExistsError(f"{fp} isn't file")
     except OSError as e:
         if os.name == "nt" and e.winerror == 123:
             illegal_characters = set([char for char in filename if char in r'\/:*?"<>|'])
             illegal_characters_str = ", ".join(illegal_characters)
             raise ValueError(
                 f"Invalid file path: {filename}. "
                 f"It contains illegal characters: {illegal_characters_str}"
```

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/perfect_table.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/perfect_table.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/script_report_utils.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/script_report_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/sse_client.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/stream_utils/__init__.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/stream_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/stream_utils/stream_utils.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/stream_utils/stream_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/time.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/time.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/total_category_calculator.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/total_category_calculator.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/viewer_structs/__init__.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/viewer_structs/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/viewer_structs/verification.py` & `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/viewer_structs/verification.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services.egg-info/PKG-INFO` & `th2_data_services-2.0.0.dev8702324290/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 322d  : 2.1.Name: th2-
-00000020: 6461 7461 2d73 6572 7669 6365 730a 5665  data-services.Ve
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 325f  : 2.1.Name: th2_
+00000020: 6461 7461 5f73 6572 7669 6365 730a 5665  data_services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3836 3632 3538 3638 3139 0a53 756d 6d61  8662586819.Summa
+00000040: 3837 3032 3332 3432 3930 0a53 756d 6d61  8702324290.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
@@ -316,1936 +316,2347 @@
 000013b0: 6174 6574 696d 6520 696d 706f 7274 2064  atetime import d
 000013c0: 6174 6574 696d 650a 2020 2020 2020 2020  atetime.        
 000013d0: 0a20 2020 2020 2020 2066 726f 6d20 7468  .        from th
 000013e0: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
 000013f0: 6461 7461 2069 6d70 6f72 7420 4461 7461  data import Data
 00001400: 0a20 2020 2020 2020 2066 726f 6d20 7468  .        from th
 00001410: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
-00001420: 6576 656e 745f 7472 6565 2069 6d70 6f72  event_tree impor
-00001430: 7420 280a 2020 2020 2020 2020 2020 2020  t (.            
-00001440: 4576 656e 7454 7265 652c 0a20 2020 2020  EventTree,.     
-00001450: 2020 2020 2020 2045 7665 6e74 5472 6565         EventTree
-00001460: 436f 6c6c 6563 7469 6f6e 2c0a 2020 2020  Collection,.    
-00001470: 2020 2020 2020 2020 5061 7265 6e74 4576          ParentEv
-00001480: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
-00001490: 6e2c 0a20 2020 2020 2020 2020 2020 2049  n,.            I
-000014a0: 4554 4344 7269 7665 722c 0a20 2020 2020  ETCDriver,.     
-000014b0: 2020 2029 0a20 2020 2020 2020 2066 726f     ).        fro
-000014c0: 6d20 7468 325f 6461 7461 5f73 6572 7669  m th2_data_servi
-000014d0: 6365 732e 696e 7465 7266 6163 6573 2069  ces.interfaces i
-000014e0: 6d70 6f72 7420 4944 6174 6153 6f75 7263  mport IDataSourc
-000014f0: 650a 2020 2020 2020 2020 6672 6f6d 2074  e.        from t
-00001500: 6832 5f64 6174 615f 7365 7276 6963 6573  h2_data_services
-00001510: 2e75 7469 6c73 2e63 6f6e 7665 7274 6572  .utils.converter
-00001520: 7320 696d 706f 7274 2028 0a20 2020 2020  s import (.     
-00001530: 2020 2020 2020 2044 6174 6574 696d 6543         DatetimeC
-00001540: 6f6e 7665 7274 6572 2c0a 2020 2020 2020  onverter,.      
-00001550: 2020 2020 2020 4461 7465 7469 6d65 5374        DatetimeSt
-00001560: 7269 6e67 436f 6e76 6572 7465 722c 0a20  ringConverter,. 
-00001570: 2020 2020 2020 2020 2020 2050 726f 746f             Proto
-00001580: 6275 6654 696d 6573 7461 6d70 436f 6e76  bufTimestampConv
-00001590: 6572 7465 722c 0a20 2020 2020 2020 2020  erter,.         
-000015a0: 2020 2054 6832 5469 6d65 7374 616d 7043     Th2TimestampC
-000015b0: 6f6e 7665 7274 6572 2c0a 2020 2020 2020  onverter,.      
-000015c0: 2020 290a 2020 2020 2020 2020 0a20 2020    ).        .   
-000015d0: 2020 2020 2023 205b 305d 204c 6962 2063       # [0] Lib c
-000015e0: 6f6e 6669 6775 7261 7469 6f6e 0a20 2020  onfiguration.   
-000015f0: 2020 2020 2023 205b 302e 315d 2049 6e74       # [0.1] Int
-00001600: 6572 6163 7469 7665 206f 7220 5363 7269  eractive or Scri
-00001610: 7074 206d 6f64 650a 2020 2020 2020 2020  pt mode.        
-00001620: 2320 4966 2079 6f75 2075 7365 2074 6865  # If you use the
-00001630: 206c 6962 2069 6e20 696e 7465 7261 6374   lib in interact
-00001640: 6976 6520 6d6f 6465 2028 6a75 7079 7465  ive mode (jupyte
-00001650: 722c 2069 7079 7468 6f6e 2920 6974 2773  r, ipython) it's
-00001660: 2072 6563 6f6d 6d65 6e64 6564 2074 6f20   recommended to 
-00001670: 7365 7420 7468 6520 7370 6563 6961 6c0a  set the special.
-00001680: 2020 2020 2020 2020 2320 676c 6f62 616c          # global
-00001690: 2070 6172 616d 6574 6572 2074 6f20 5472   parameter to Tr
-000016a0: 7565 2e20 4974 276c 6c20 6b65 6570 2063  ue. It'll keep c
-000016b0: 6163 6865 2066 696c 6573 2069 6620 736f  ache files if so
-000016c0: 6d65 7468 696e 6720 7765 6e74 2077 726f  mething went wro
-000016d0: 6e67 2e0a 2020 2020 2020 2020 6672 6f6d  ng..        from
-000016e0: 2074 6832 5f64 6174 615f 7365 7276 6963   th2_data_servic
-000016f0: 6573 2e63 6f6e 6669 6720 696d 706f 7274  es.config import
-00001700: 206f 7074 696f 6e73 0a20 2020 2020 2020   options.       
-00001710: 200a 2020 2020 2020 2020 6f70 7469 6f6e   .        option
-00001720: 732e 494e 5445 5241 4354 4956 455f 4d4f  s.INTERACTIVE_MO
-00001730: 4445 203d 2054 7275 650a 2020 2020 2020  DE = True.      
-00001740: 2020 0a20 2020 2020 2020 2023 2053 6f6d    .        # Som
-00001750: 6520 6578 616d 706c 6520 6461 7461 0a20  e example data. 
-00001760: 2020 2020 2020 2065 7665 6e74 7320 3d20         events = 
-00001770: 4461 7461 280a 2020 2020 2020 2020 2020  Data(.          
-00001780: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
-00001790: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-000017a0: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
-000017b0: 4964 223a 2022 6465 6d6f 5f62 6f6f 6b5f  Id": "demo_book_
-000017c0: 313a 7468 322d 7363 6f70 653a 3230 3233  1:th2-scope:2023
-000017d0: 3031 3035 3133 3537 3035 3536 3038 3733  0105135705560873
-000017e0: 3030 303a 6436 3165 3933 3061 2d38 6430  000:d61e930a-8d0
-000017f0: 302d 3131 6564 2d61 6131 612d 6433 3461  0-11ed-aa1a-d34a
-00001800: 3631 3535 3135 3264 5f31 222c 0a20 2020  6155152d_1",.   
-00001810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001820: 2022 6261 7463 6849 6422 3a20 4e6f 6e65   "batchId": None
-00001830: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001840: 2020 2020 2020 2269 7342 6174 6368 6564        "isBatched
-00001850: 223a 2046 616c 7365 2c0a 2020 2020 2020  ": False,.      
-00001860: 2020 2020 2020 2020 2020 2020 2020 2265                "e
-00001870: 7665 6e74 4e61 6d65 223a 2022 5365 7420  ventName": "Set 
-00001880: 6f66 2061 7574 6f2d 6765 6e65 7261 7465  of auto-generate
-00001890: 6420 6576 656e 7473 2066 6f72 2064 7320  d events for ds 
-000018a0: 6c69 6220 7465 7374 696e 6722 2c0a 2020  lib testing",.  
+00001420: 6475 6d6d 7920 696d 706f 7274 2044 756d  dummy import Dum
+00001430: 6d79 4461 7461 536f 7572 6365 0a20 2020  myDataSource.   
+00001440: 2020 2020 2066 726f 6d20 7468 325f 6461       from th2_da
+00001450: 7461 5f73 6572 7669 6365 732e 6576 656e  ta_services.even
+00001460: 745f 7472 6565 2069 6d70 6f72 7420 280a  t_tree import (.
+00001470: 2020 2020 2020 2020 2020 2020 4576 656e              Even
+00001480: 7454 7265 652c 0a20 2020 2020 2020 2020  tTree,.         
+00001490: 2020 2045 7665 6e74 5472 6565 436f 6c6c     EventTreeColl
+000014a0: 6563 7469 6f6e 2c0a 2020 2020 2020 2020  ection,.        
+000014b0: 2020 2020 5061 7265 6e74 4576 656e 7454      ParentEventT
+000014c0: 7265 6543 6f6c 6c65 6374 696f 6e2c 0a20  reeCollection,. 
+000014d0: 2020 2020 2020 2020 2020 2049 4554 4344             IETCD
+000014e0: 7269 7665 722c 0a20 2020 2020 2020 2029  river,.        )
+000014f0: 0a20 2020 2020 2020 2066 726f 6d20 7468  .        from th
+00001500: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
+00001510: 696e 7465 7266 6163 6573 2069 6d70 6f72  interfaces impor
+00001520: 7420 4944 6174 6153 6f75 7263 650a 2020  t IDataSource.  
+00001530: 2020 2020 2020 6672 6f6d 2074 6832 5f64        from th2_d
+00001540: 6174 615f 7365 7276 6963 6573 2e75 7469  ata_services.uti
+00001550: 6c73 2e63 6f6e 7665 7274 6572 7320 696d  ls.converters im
+00001560: 706f 7274 2028 0a20 2020 2020 2020 2020  port (.         
+00001570: 2020 2044 6174 6574 696d 6543 6f6e 7665     DatetimeConve
+00001580: 7274 6572 2c0a 2020 2020 2020 2020 2020  rter,.          
+00001590: 2020 4461 7465 7469 6d65 5374 7269 6e67    DatetimeString
+000015a0: 436f 6e76 6572 7465 722c 0a20 2020 2020  Converter,.     
+000015b0: 2020 2020 2020 2050 726f 746f 6275 6654         ProtobufT
+000015c0: 696d 6573 7461 6d70 436f 6e76 6572 7465  imestampConverte
+000015d0: 722c 0a20 2020 2020 2020 2020 2020 2054  r,.            T
+000015e0: 6832 5469 6d65 7374 616d 7043 6f6e 7665  h2TimestampConve
+000015f0: 7274 6572 2c0a 2020 2020 2020 2020 290a  rter,.        ).
+00001600: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001610: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
+00001620: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001630: 2323 2323 2323 230a 2020 2020 2020 2020  #######.        
+00001640: 2320 5b30 5d20 4c69 6220 636f 6e66 6967  # [0] Lib config
+00001650: 7572 6174 696f 6e0a 2020 2020 2020 2020  uration.        
+00001660: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001670: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001680: 2323 2323 2323 0a20 2020 2020 2020 200a  ######.        .
+00001690: 2020 2020 2020 2020 2320 5b30 2e31 5d20          # [0.1] 
+000016a0: 496e 7465 7261 6374 6976 6520 6f72 2053  Interactive or S
+000016b0: 6372 6970 7420 6d6f 6465 0a20 2020 2020  cript mode.     
+000016c0: 2020 2023 2049 6620 796f 7520 7573 6520     # If you use 
+000016d0: 7468 6520 6c69 6220 696e 2069 6e74 6572  the lib in inter
+000016e0: 6163 7469 7665 206d 6f64 6520 286a 7570  active mode (jup
+000016f0: 7974 6572 2c20 6970 7974 686f 6e29 2069  yter, ipython) i
+00001700: 7427 7320 7265 636f 6d6d 656e 6465 6420  t's recommended 
+00001710: 746f 2073 6574 2074 6865 2073 7065 6369  to set the speci
+00001720: 616c 0a20 2020 2020 2020 2023 2067 6c6f  al.        # glo
+00001730: 6261 6c20 7061 7261 6d65 7465 7220 746f  bal parameter to
+00001740: 2054 7275 652e 2049 7427 6c6c 206b 6565   True. It'll kee
+00001750: 7020 6361 6368 6520 6669 6c65 7320 6966  p cache files if
+00001760: 2073 6f6d 6574 6869 6e67 2077 656e 7420   something went 
+00001770: 7772 6f6e 672e 0a20 2020 2020 2020 2066  wrong..        f
+00001780: 726f 6d20 7468 325f 6461 7461 5f73 6572  rom th2_data_ser
+00001790: 7669 6365 732e 636f 6e66 6967 2069 6d70  vices.config imp
+000017a0: 6f72 7420 6f70 7469 6f6e 730a 2020 2020  ort options.    
+000017b0: 2020 2020 0a20 2020 2020 2020 206f 7074      .        opt
+000017c0: 696f 6e73 2e49 4e54 4552 4143 5449 5645  ions.INTERACTIVE
+000017d0: 5f4d 4f44 4520 3d20 5472 7565 0a20 2020  _MODE = True.   
+000017e0: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+000017f0: 536f 6d65 2065 7861 6d70 6c65 2064 6174  Some example dat
+00001800: 610a 2020 2020 2020 2020 6576 656e 7473  a.        events
+00001810: 203d 2044 6174 6128 0a20 2020 2020 2020   = Data(.       
+00001820: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
+00001830: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00001840: 2020 2020 2020 2020 2020 2020 2022 6576               "ev
+00001850: 656e 7449 6422 3a20 2264 656d 6f5f 626f  entId": "demo_bo
+00001860: 6f6b 5f31 3a74 6832 2d73 636f 7065 3a32  ok_1:th2-scope:2
+00001870: 3032 3330 3130 3531 3335 3730 3535 3630  0230105135705560
+00001880: 3837 3330 3030 3a64 3631 6539 3330 612d  873000:d61e930a-
+00001890: 3864 3030 2d31 3165 642d 6161 3161 2d64  8d00-11ed-aa1a-d
+000018a0: 3334 6136 3135 3531 3532 645f 3122 2c0a  34a6155152d_1",.
 000018b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018c0: 2020 2265 7665 6e74 5479 7065 223a 2022    "eventType": "
-000018d0: 6473 2d6c 6962 2d74 6573 742d 6576 656e  ds-lib-test-even
-000018e0: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-000018f0: 2020 2020 2020 2020 2265 6e64 5469 6d65          "endTime
-00001900: 7374 616d 7022 3a20 7b22 6570 6f63 6853  stamp": {"epochS
-00001910: 6563 6f6e 6422 3a20 3136 3732 3932 3730  econd": 16729270
-00001920: 3235 2c20 226e 616e 6f22 3a20 3536 3137  25, "nano": 5617
-00001930: 3531 3030 307d 2c0a 2020 2020 2020 2020  51000},.        
-00001940: 2020 2020 2020 2020 2020 2020 2273 7461              "sta
-00001950: 7274 5469 6d65 7374 616d 7022 3a20 7b22  rtTimestamp": {"
-00001960: 6570 6f63 6853 6563 6f6e 6422 3a20 3136  epochSecond": 16
-00001970: 3732 3932 3730 3235 2c20 226e 616e 6f22  72927025, "nano"
-00001980: 3a20 3536 3038 3733 3030 307d 2c0a 2020  : 560873000},.  
-00001990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019a0: 2020 2270 6172 656e 7445 7665 6e74 4964    "parentEventId
-000019b0: 223a 204e 6f6e 652c 0a20 2020 2020 2020  ": None,.       
-000019c0: 2020 2020 2020 2020 2020 2020 2022 7375               "su
-000019d0: 6363 6573 7366 756c 223a 2054 7275 652c  ccessful": True,
-000019e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000019f0: 2020 2020 2022 626f 6f6b 4964 223a 2022       "bookId": "
-00001a00: 6465 6d6f 5f62 6f6f 6b5f 3122 2c0a 2020  demo_book_1",.  
-00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a20: 2020 2273 636f 7065 223a 2022 7468 322d    "scope": "th2-
-00001a30: 7363 6f70 6522 2c0a 2020 2020 2020 2020  scope",.        
-00001a40: 2020 2020 2020 2020 2020 2020 2261 7474              "att
-00001a50: 6163 6865 644d 6573 7361 6765 4964 7322  achedMessageIds"
-00001a60: 3a20 5b5d 2c0a 2020 2020 2020 2020 2020  : [],.          
-00001a70: 2020 2020 2020 2020 2020 2262 6f64 7922            "body"
-00001a80: 3a20 5b5d 2c0a 2020 2020 2020 2020 2020  : [],.          
-00001a90: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00001aa0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-00001ab0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001ac0: 6576 656e 7449 6422 3a20 2264 656d 6f5f  eventId": "demo_
-00001ad0: 626f 6f6b 5f31 3a74 6832 2d73 636f 7065  book_1:th2-scope
-00001ae0: 3a32 3032 3330 3130 3531 3335 3730 3535  :202301051357055
-00001af0: 3633 3532 3230 3030 3a39 6164 6262 3365  63522000:9adbb3e
-00001b00: 302d 3566 3862 2d34 6332 382d 6132 6163  0-5f8b-4c28-a2ac
-00001b10: 2d37 3336 3165 3866 6137 3034 633e 6465  -7361e8fa704c>de
-00001b20: 6d6f 5f62 6f6f 6b5f 313a 7468 322d 7363  mo_book_1:th2-sc
-00001b30: 6f70 653a 3230 3233 3031 3035 3133 3537  ope:202301051357
-00001b40: 3035 3536 3335 3232 3030 303a 6436 3165  05563522000:d61e
-00001b50: 3933 3061 2d38 6430 302d 3131 6564 2d61  930a-8d00-11ed-a
-00001b60: 6131 612d 6433 3461 3631 3535 3135 3264  a1a-d34a6155152d
-00001b70: 5f32 222c 0a20 2020 2020 2020 2020 2020  _2",.           
-00001b80: 2020 2020 2020 2020 2022 6261 7463 6849           "batchI
-00001b90: 6422 3a20 2264 656d 6f5f 626f 6f6b 5f31  d": "demo_book_1
-00001ba0: 3a74 6832 2d73 636f 7065 3a32 3032 3330  :th2-scope:20230
-00001bb0: 3130 3531 3335 3730 3535 3633 3532 3230  1051357055635220
-00001bc0: 3030 3a39 6164 6262 3365 302d 3566 3862  00:9adbb3e0-5f8b
-00001bd0: 2d34 6332 382d 6132 6163 2d37 3336 3165  -4c28-a2ac-7361e
-00001be0: 3866 6137 3034 6322 2c0a 2020 2020 2020  8fa704c",.      
-00001bf0: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-00001c00: 7342 6174 6368 6564 223a 2054 7275 652c  sBatched": True,
-00001c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001c20: 2020 2020 2022 6576 656e 744e 616d 6522       "eventName"
-00001c30: 3a20 2250 6c61 696e 2065 7665 6e74 2031  : "Plain event 1
-00001c40: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00001c50: 2020 2020 2020 2022 6576 656e 7454 7970         "eventTyp
-00001c60: 6522 3a20 2264 732d 6c69 622d 7465 7374  e": "ds-lib-test
-00001c70: 2d65 7665 6e74 222c 0a20 2020 2020 2020  -event",.       
-00001c80: 2020 2020 2020 2020 2020 2020 2022 656e               "en
-00001c90: 6454 696d 6573 7461 6d70 223a 207b 2265  dTimestamp": {"e
-00001ca0: 706f 6368 5365 636f 6e64 223a 2031 3637  pochSecond": 167
-00001cb0: 3239 3237 3032 352c 2022 6e61 6e6f 223a  2927025, "nano":
-00001cc0: 2035 3633 3634 3030 3030 7d2c 0a20 2020   563640000},.   
-00001cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ce0: 2022 7374 6172 7454 696d 6573 7461 6d70   "startTimestamp
-00001cf0: 223a 207b 2265 706f 6368 5365 636f 6e64  ": {"epochSecond
-00001d00: 223a 2031 3637 3239 3237 3032 352c 2022  ": 1672927025, "
-00001d10: 6e61 6e6f 223a 2035 3633 3532 3230 3030  nano": 563522000
-00001d20: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00001d30: 2020 2020 2020 2022 7061 7265 6e74 4576         "parentEv
-00001d40: 656e 7449 6422 3a20 2264 656d 6f5f 626f  entId": "demo_bo
-00001d50: 6f6b 5f31 3a74 6832 2d73 636f 7065 3a32  ok_1:th2-scope:2
-00001d60: 3032 3330 3130 3531 3335 3730 3535 3630  0230105135705560
-00001d70: 3837 3330 3030 3a64 3631 6539 3330 612d  873000:d61e930a-
-00001d80: 3864 3030 2d31 3165 642d 6161 3161 2d64  8d00-11ed-aa1a-d
-00001d90: 3334 6136 3135 3531 3532 645f 3122 2c0a  34a6155152d_1",.
-00001da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001db0: 2020 2020 2273 7563 6365 7373 6675 6c22      "successful"
-00001dc0: 3a20 5472 7565 2c0a 2020 2020 2020 2020  : True,.        
-00001dd0: 2020 2020 2020 2020 2020 2020 2262 6f6f              "boo
-00001de0: 6b49 6422 3a20 2264 656d 6f5f 626f 6f6b  kId": "demo_book
-00001df0: 5f31 222c 0a20 2020 2020 2020 2020 2020  _1",.           
-00001e00: 2020 2020 2020 2020 2022 7363 6f70 6522           "scope"
-00001e10: 3a20 2274 6832 2d73 636f 7065 222c 0a20  : "th2-scope",. 
-00001e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e30: 2020 2022 6174 7461 6368 6564 4d65 7373     "attachedMess
-00001e40: 6167 6549 6473 223a 205b 5d2c 0a20 2020  ageIds": [],.   
-00001e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e60: 2022 626f 6479 223a 207b 2274 7970 6522   "body": {"type"
-00001e70: 3a20 226d 6573 7361 6765 222c 2022 6461  : "message", "da
-00001e80: 7461 223a 2022 6473 2d6c 6962 2074 6573  ta": "ds-lib tes
-00001e90: 7420 626f 6479 227d 2c0a 2020 2020 2020  t body"},.      
-00001ea0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00001eb0: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
-00001ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ed0: 2020 2022 6576 656e 7449 6422 3a20 2264     "eventId": "d
-00001ee0: 656d 6f5f 626f 6f6b 5f31 3a74 6832 2d73  emo_book_1:th2-s
-00001ef0: 636f 7065 3a32 3032 3330 3130 3531 3335  cope:20230105135
-00001f00: 3730 3535 3633 3532 3230 3030 3a39 6164  705563522000:9ad
-00001f10: 6262 3365 302d 3566 3862 2d34 6332 382d  bb3e0-5f8b-4c28-
-00001f20: 6132 6163 2d37 3336 3165 3866 6137 3034  a2ac-7361e8fa704
-00001f30: 633e 6465 6d6f 5f62 6f6f 6b5f 313a 7468  c>demo_book_1:th
-00001f40: 322d 7363 6f70 653a 3230 3233 3031 3035  2-scope:20230105
-00001f50: 3133 3537 3035 3536 3337 3537 3030 303a  135705563757000:
-00001f60: 6436 3165 3933 3061 2d38 6430 302d 3131  d61e930a-8d00-11
-00001f70: 6564 2d61 6131 612d 6433 3461 3631 3535  ed-aa1a-d34a6155
-00001f80: 3135 3264 5f33 222c 0a20 2020 2020 2020  152d_3",.       
-00001f90: 2020 2020 2020 2020 2020 2020 2022 6261               "ba
-00001fa0: 7463 6849 6422 3a20 2264 656d 6f5f 626f  tchId": "demo_bo
-00001fb0: 6f6b 5f31 3a74 6832 2d73 636f 7065 3a32  ok_1:th2-scope:2
-00001fc0: 3032 3330 3130 3531 3335 3730 3535 3633  0230105135705563
-00001fd0: 3532 3230 3030 3a39 6164 6262 3365 302d  522000:9adbb3e0-
-00001fe0: 3566 3862 2d34 6332 382d 6132 6163 2d37  5f8b-4c28-a2ac-7
-00001ff0: 3336 3165 3866 6137 3034 6322 2c0a 2020  361e8fa704c",.  
-00002000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002010: 2020 2269 7342 6174 6368 6564 223a 2054    "isBatched": T
-00002020: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-00002030: 2020 2020 2020 2020 2022 6576 656e 744e           "eventN
-00002040: 616d 6522 3a20 2250 6c61 696e 2065 7665  ame": "Plain eve
-00002050: 6e74 2032 222c 0a20 2020 2020 2020 2020  nt 2",.         
-00002060: 2020 2020 2020 2020 2020 2022 6576 656e             "even
-00002070: 7454 7970 6522 3a20 2264 732d 6c69 622d  tType": "ds-lib-
-00002080: 7465 7374 2d65 7665 6e74 222c 0a20 2020  test-event",.   
-00002090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020a0: 2022 656e 6454 696d 6573 7461 6d70 223a   "endTimestamp":
-000020b0: 207b 2265 706f 6368 5365 636f 6e64 223a   {"epochSecond":
-000020c0: 2031 3637 3239 3237 3032 352c 2022 6e61   1672927025, "na
-000020d0: 6e6f 223a 2035 3633 3739 3130 3030 7d2c  no": 563791000},
-000020e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000020f0: 2020 2020 2022 7374 6172 7454 696d 6573       "startTimes
-00002100: 7461 6d70 223a 207b 2265 706f 6368 5365  tamp": {"epochSe
-00002110: 636f 6e64 223a 2031 3637 3239 3237 3032  cond": 167292702
-00002120: 352c 2022 6e61 6e6f 223a 2035 3633 3735  5, "nano": 56375
-00002130: 3730 3030 7d2c 0a20 2020 2020 2020 2020  7000},.         
-00002140: 2020 2020 2020 2020 2020 2022 7061 7265             "pare
-00002150: 6e74 4576 656e 7449 6422 3a20 2264 656d  ntEventId": "dem
-00002160: 6f5f 626f 6f6b 5f31 3a74 6832 2d73 636f  o_book_1:th2-sco
-00002170: 7065 3a32 3032 3330 3130 3531 3335 3730  pe:2023010513570
-00002180: 3535 3630 3837 3330 3030 3a64 3631 6539  5560873000:d61e9
-00002190: 3330 612d 3864 3030 2d31 3165 642d 6161  30a-8d00-11ed-aa
-000021a0: 3161 2d64 3334 6136 3135 3531 3532 645f  1a-d34a6155152d_
-000021b0: 3122 2c0a 2020 2020 2020 2020 2020 2020  1",.            
-000021c0: 2020 2020 2020 2020 2273 7563 6365 7373          "success
-000021d0: 6675 6c22 3a20 5472 7565 2c0a 2020 2020  ful": True,.    
-000021e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021f0: 2262 6f6f 6b49 6422 3a20 2264 656d 6f5f  "bookId": "demo_
-00002200: 626f 6f6b 5f31 222c 0a20 2020 2020 2020  book_1",.       
-00002210: 2020 2020 2020 2020 2020 2020 2022 7363               "sc
-00002220: 6f70 6522 3a20 2274 6832 2d73 636f 7065  ope": "th2-scope
-00002230: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00002240: 2020 2020 2020 2022 6174 7461 6368 6564         "attached
-00002250: 4d65 7373 6167 6549 6473 223a 205b 5d2c  MessageIds": [],
-00002260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002270: 2020 2020 2022 626f 6479 223a 207b 2274       "body": {"t
-00002280: 7970 6522 3a20 226d 6573 7361 6765 222c  ype": "message",
-00002290: 2022 6461 7461 223a 2022 6473 2d6c 6962   "data": "ds-lib
-000022a0: 2074 6573 7420 626f 6479 227d 2c0a 2020   test body"},.  
-000022b0: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-000022c0: 0a20 2020 2020 2020 2020 2020 205d 0a20  .            ]. 
-000022d0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000022e0: 200a 2020 2020 2020 2020 2320 5b31 5d20   .        # [1] 
-000022f0: 576f 726b 696e 6720 7769 7468 2061 2044  Working with a D
-00002300: 6174 6120 6f62 6a65 6374 2e0a 2020 2020  ata object..    
-00002310: 2020 2020 2320 5b31 2e31 5d20 4669 6c74      # [1.1] Filt
-00002320: 6572 2e0a 2020 2020 2020 2020 6669 6c74  er..        filt
-00002330: 6572 6564 5f65 7665 6e74 733a 2044 6174  ered_events: Dat
-00002340: 6120 3d20 6576 656e 7473 2e66 696c 7465  a = events.filte
-00002350: 7228 6c61 6d62 6461 2065 3a20 655b 2262  r(lambda e: e["b
-00002360: 6f64 7922 5d20 213d 205b 5d29 2020 2320  ody"] != [])  # 
-00002370: 4669 6c74 6572 2065 7665 6e74 7320 7769  Filter events wi
-00002380: 7468 2065 6d70 7479 2062 6f64 792e 0a20  th empty body.. 
-00002390: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000023a0: 0a20 2020 2020 2020 2023 205b 312e 325d  .        # [1.2]
-000023b0: 204d 6170 2e0a 2020 2020 2020 2020 6465   Map..        de
-000023c0: 6620 7472 616e 7366 6f72 6d5f 6675 6e63  f transform_func
-000023d0: 7469 6f6e 2872 6563 6f72 6429 3a0a 2020  tion(record):.  
-000023e0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000023f0: 207b 2265 7665 6e74 4e61 6d65 223a 2072   {"eventName": r
-00002400: 6563 6f72 645b 2265 7665 6e74 4e61 6d65  ecord["eventName
-00002410: 225d 2c20 2273 7563 6365 7373 6675 6c22  "], "successful"
-00002420: 3a20 7265 636f 7264 5b22 7375 6363 6573  : record["succes
-00002430: 7366 756c 225d 7d0a 2020 2020 2020 2020  sful"]}.        
-00002440: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00002450: 2020 6669 6c74 6572 6564 5f61 6e64 5f6d    filtered_and_m
-00002460: 6170 7065 645f 6576 656e 7473 203d 2066  apped_events = f
-00002470: 696c 7465 7265 645f 6576 656e 7473 2e6d  iltered_events.m
-00002480: 6170 2874 7261 6e73 666f 726d 5f66 756e  ap(transform_fun
-00002490: 6374 696f 6e29 0a20 2020 2020 2020 200a  ction).        .
-000024a0: 2020 2020 2020 2020 2320 5b31 2e33 5d20          # [1.3] 
-000024b0: 4461 7461 2070 6970 656c 696e 652e 0a20  Data pipeline.. 
-000024c0: 2020 2020 2020 2023 2020 2020 2020 2049         #       I
-000024d0: 6e73 7465 6164 206f 6620 646f 696e 6720  nstead of doing 
-000024e0: 6461 7461 2074 7261 6e73 666f 726d 6174  data transformat
-000024f0: 696f 6e73 2073 7465 7020 6279 2073 7465  ions step by ste
-00002500: 7020 796f 7520 6361 6e20 646f 2069 7420  p you can do it 
-00002510: 696e 206f 6e65 206c 696e 652e 0a20 2020  in one line..   
-00002520: 2020 2020 2066 696c 7465 7265 645f 616e       filtered_an
-00002530: 645f 6d61 7070 6564 5f65 7665 6e74 735f  d_mapped_events_
-00002540: 6279 5f70 6970 656c 696e 6520 3d20 6576  by_pipeline = ev
-00002550: 656e 7473 2e66 696c 7465 7228 6c61 6d62  ents.filter(lamb
-00002560: 6461 2065 3a20 655b 2262 6f64 7922 5d20  da e: e["body"] 
-00002570: 213d 205b 5d29 2e6d 6170 280a 2020 2020  != []).map(.    
-00002580: 2020 2020 2020 2020 7472 616e 7366 6f72          transfor
-00002590: 6d5f 6675 6e63 7469 6f6e 0a20 2020 2020  m_function.     
-000025a0: 2020 2029 0a20 2020 2020 2020 2023 2043     ).        # C
-000025b0: 6f6e 7465 6e74 206f 6620 7468 6573 6520  ontent of these 
-000025c0: 7477 6f20 4461 7461 206f 626a 6563 7473  two Data objects
-000025d0: 2073 686f 756c 6420 6265 2065 7175 616c   should be equal
-000025e0: 2e0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
-000025f0: 206c 6973 7428 6669 6c74 6572 6564 5f61   list(filtered_a
-00002600: 6e64 5f6d 6170 7065 645f 6576 656e 7473  nd_mapped_events
-00002610: 2920 3d3d 206c 6973 7428 6669 6c74 6572  ) == list(filter
-00002620: 6564 5f61 6e64 5f6d 6170 7065 645f 6576  ed_and_mapped_ev
-00002630: 656e 7473 5f62 795f 7069 7065 6c69 6e65  ents_by_pipeline
-00002640: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-00002650: 2020 2023 205b 312e 345d 2053 6966 742e     # [1.4] Sift.
-00002660: 2053 6b69 7020 7468 6520 6669 7273 7420   Skip the first 
-00002670: 6665 7720 6974 656d 7320 6f72 206c 696d  few items or lim
-00002680: 6974 2074 6865 6d2e 0a20 2020 2020 2020  it them..       
-00002690: 2064 6174 6120 3d20 4461 7461 285b 312c   data = Data([1,
-000026a0: 2032 2c20 332c 2034 2c20 352c 2036 2c20   2, 3, 4, 5, 6, 
-000026b0: 372c 2038 2c20 392c 2031 302c 2031 312c  7, 8, 9, 10, 11,
-000026c0: 2031 322c 2031 332c 2031 342c 2031 355d   12, 13, 14, 15]
-000026d0: 290a 2020 2020 2020 2020 6974 656d 735f  ).        items_
-000026e0: 6672 6f6d 5f31 315f 746f 5f65 6e64 3a20  from_11_to_end: 
-000026f0: 4765 6e65 7261 746f 7220 3d20 6461 7461  Generator = data
-00002700: 2e73 6966 7428 736b 6970 3d31 3029 0a20  .sift(skip=10). 
-00002710: 2020 2020 2020 206f 6e6c 795f 6669 7273         only_firs
-00002720: 745f 3130 5f69 7465 6d73 3a20 4765 6e65  t_10_items: Gene
-00002730: 7261 746f 7220 3d20 6461 7461 2e73 6966  rator = data.sif
-00002740: 7428 6c69 6d69 743d 3130 290a 2020 2020  t(limit=10).    
-00002750: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-00002760: 312e 355d 2043 6861 6e67 696e 6720 6361  1.5] Changing ca
-00002770: 6368 6520 7374 6174 7573 2e0a 2020 2020  che status..    
-00002780: 2020 2020 6576 656e 7473 2e75 7365 5f63      events.use_c
-00002790: 6163 6865 2854 7275 6529 0a20 2020 2020  ache(True).     
-000027a0: 2020 2023 206f 7220 6a75 7374 0a20 2020     # or just.   
-000027b0: 2020 2020 2065 7665 6e74 732e 7573 655f       events.use_
-000027c0: 6361 6368 6528 2920 2023 2049 6620 796f  cache()  # If yo
-000027d0: 7520 7761 6e74 2074 6f20 6163 7469 7661  u want to activa
-000027e0: 7465 2063 6163 6865 2e0a 2020 2020 2020  te cache..      
-000027f0: 2020 2320 5b31 2e36 5d20 5761 6c6b 2074    # [1.6] Walk t
-00002800: 6872 6f75 6768 2064 6174 612e 0a20 2020  hrough data..   
-00002810: 2020 2020 2066 6f72 2065 7665 6e74 2069       for event i
-00002820: 6e20 6576 656e 7473 3a0a 2020 2020 2020  n events:.      
-00002830: 2020 2020 2020 2320 446f 2073 6f6d 6574        # Do somet
-00002840: 6869 6e67 2077 6974 6820 6576 656e 7420  hing with event 
-00002850: 2865 7665 6e74 2069 7320 6120 6469 6374  (event is a dict
-00002860: 292e 0a20 2020 2020 2020 2020 2020 2070  )..            p
-00002870: 7269 6e74 2865 7665 6e74 290a 2020 2020  rint(event).    
-00002880: 2020 2020 2320 4166 7465 7220 6669 7273      # After firs
-00002890: 7420 6974 6572 6174 696f 6e20 7468 6520  t iteration the 
-000028a0: 6576 656e 7473 2068 6173 2061 2063 6163  events has a cac
-000028b0: 6865 2066 696c 652e 0a20 2020 2020 2020  he file..       
-000028c0: 2023 204e 6f77 2074 6865 7920 7769 6c6c   # Now they will
-000028d0: 2062 6520 7573 6564 2069 6e20 7468 6520   be used in the 
-000028e0: 6361 6368 6520 696e 2074 6865 206e 6578  cache in the nex
-000028f0: 7420 6974 6572 6174 696f 6e2e 0a20 2020  t iteration..   
-00002900: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
-00002910: 5b31 2e37 5d20 4765 7420 6e75 6d62 6572  [1.7] Get number
-00002920: 206f 6620 7468 6520 656c 656d 656e 7473   of the elements
-00002930: 2069 6e20 7468 6520 4461 7461 206f 626a   in the Data obj
-00002940: 6563 742e 0a20 2020 2020 2020 206e 756d  ect..        num
-00002950: 6265 725f 6f66 5f65 7665 6e74 7320 3d20  ber_of_events = 
-00002960: 6576 656e 7473 2e6c 656e 0a20 2020 2020  events.len.     
-00002970: 2020 200a 2020 2020 2020 2020 2320 5b31     .        # [1
-00002980: 2e38 5d20 4368 6563 6b20 7468 6174 2044  .8] Check that D
-00002990: 6174 6120 6f62 6a65 6374 2069 736e 2774  ata object isn't
-000029a0: 2065 6d70 7479 2e0a 2020 2020 2020 2020   empty..        
-000029b0: 2320 5468 6520 6461 7461 2073 6f75 7263  # The data sourc
-000029c0: 6520 7368 6f75 6c64 2062 6520 6e6f 7420  e should be not 
-000029d0: 656d 7074 792e 0a20 2020 2020 2020 2061  empty..        a
-000029e0: 7373 6572 7420 6576 656e 7473 2e69 735f  ssert events.is_
-000029f0: 656d 7074 7920 6973 2046 616c 7365 0a20  empty is False. 
-00002a00: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00002a10: 2320 5b31 2e39 5d20 436f 6e76 6572 7420  # [1.9] Convert 
-00002a20: 4461 7461 206f 626a 6563 7420 746f 2074  Data object to t
-00002a30: 6865 206c 6973 7420 6f66 2065 6c65 6d65  he list of eleme
-00002a40: 6e74 7328 6576 656e 7473 206f 7220 6d65  nts(events or me
-00002a50: 7373 6167 6573 292e 0a20 2020 2020 2020  ssages)..       
-00002a60: 2023 2042 6520 6361 7265 6675 6c2c 2074   # Be careful, t
-00002a70: 6869 7320 6361 6e20 7461 6b65 2074 6f6f  his can take too
-00002a80: 206d 7563 6820 6d65 6d6f 7279 2e0a 2020   much memory..  
-00002a90: 2020 2020 2020 6576 656e 7473 5f6c 6973        events_lis
-00002aa0: 7420 3d20 6c69 7374 2865 7665 6e74 7329  t = list(events)
-00002ab0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00002ac0: 2020 2320 5b31 2e31 305d 2054 6865 2063    # [1.10] The c
-00002ad0: 6163 6865 2069 6e68 6572 6974 616e 6365  ache inheritance
-00002ae0: 2e0a 2020 2020 2020 2020 2320 4372 6561  ..        # Crea
-00002af0: 7465 7320 6120 6e65 7720 4461 7461 206f  tes a new Data o
-00002b00: 626a 6563 7420 7468 6174 2077 696c 6c20  bject that will 
-00002b10: 7573 6520 6361 6368 6520 6672 6f6d 2074  use cache from t
-00002b20: 6865 2065 7665 6e74 7320 4461 7461 206f  he events Data o
-00002b30: 626a 6563 742e 0a20 2020 2020 2020 2065  bject..        e
-00002b40: 7665 6e74 735f 6669 6c74 6572 6564 3a20  vents_filtered: 
-00002b50: 4461 7461 203d 2065 7665 6e74 732e 6669  Data = events.fi
-00002b60: 6c74 6572 286c 616d 6264 6120 7265 636f  lter(lambda reco
-00002b70: 7264 3a20 7265 636f 7264 2e67 6574 2822  rd: record.get("
-00002b80: 6261 7463 6849 6422 2929 0a20 2020 2020  batchId")).     
-00002b90: 2020 200a 2020 2020 2020 2020 2320 4e65     .        # Ne
-00002ba0: 7720 4461 7461 206f 626a 6563 7473 2064  w Data objects d
-00002bb0: 6f6e 2774 2075 7365 2074 6865 6972 206f  on't use their o
-00002bc0: 776e 2063 6163 6865 2062 7920 6465 6661  wn cache by defa
-00002bd0: 756c 7420 6275 7420 7573 6520 7468 6520  ult but use the 
-00002be0: 6361 6368 6520 6f66 2074 6865 2070 6172  cache of the par
-00002bf0: 656e 7420 4461 7461 206f 626a 6563 742e  ent Data object.
-00002c00: 0a20 2020 2020 2020 2023 2055 7365 2075  .        # Use u
-00002c10: 7365 5f63 6163 6865 206d 6574 686f 6420  se_cache method 
-00002c20: 746f 2061 6374 6976 6174 6520 6361 6368  to activate cach
-00002c30: 696e 672e 0a20 2020 2020 2020 2023 2041  ing..        # A
-00002c40: 6674 6572 2074 6861 742c 2074 6865 2044  fter that, the D
-00002c50: 6174 6120 6f62 6a65 6374 2077 696c 6c20  ata object will 
-00002c60: 6372 6561 7465 2069 7473 206f 776e 2063  create its own c
-00002c70: 6163 6865 2066 696c 652e 0a20 2020 2020  ache file..     
-00002c80: 2020 2065 7665 6e74 735f 6669 6c74 6572     events_filter
-00002c90: 6564 2e75 7365 5f63 6163 6865 2829 0a20  ed.use_cache(). 
-00002ca0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00002cb0: 6c69 7374 2865 7665 6e74 735f 6669 6c74  list(events_filt
-00002cc0: 6572 6564 2920 2023 204a 7573 7420 746f  ered)  # Just to
-00002cd0: 2069 7465 7261 7465 2044 6174 6120 6f62   iterate Data ob
-00002ce0: 6a65 6374 2028 6361 6368 6520 6669 6c65  ject (cache file
-00002cf0: 2077 696c 6c20 6265 2063 7265 6174 6564   will be created
-00002d00: 292e 0a20 2020 2020 2020 200a 2020 2020  )..        .    
-00002d10: 2020 2020 6669 6c74 6572 6564 5f65 7665      filtered_eve
-00002d20: 6e74 735f 7479 7065 7320 3d20 6576 656e  nts_types = even
-00002d30: 7473 5f66 696c 7465 7265 642e 6d61 7028  ts_filtered.map(
-00002d40: 6c61 6d62 6461 2072 6563 6f72 643a 207b  lambda record: {
-00002d50: 2265 7665 6e74 5479 7065 223a 2072 6563  "eventType": rec
-00002d60: 6f72 642e 6765 7428 2265 7665 6e74 5479  ord.get("eventTy
-00002d70: 7065 2229 7d29 0a20 2020 2020 2020 200a  pe")}).        .
-00002d80: 2020 2020 2020 2020 6576 656e 7473 5f77          events_w
-00002d90: 6974 686f 7574 5f74 7970 6573 5f77 6974  ithout_types_wit
-00002da0: 685f 6261 7463 6820 3d20 6669 6c74 6572  h_batch = filter
-00002db0: 6564 5f65 7665 6e74 735f 7479 7065 732e  ed_events_types.
-00002dc0: 6669 6c74 6572 280a 2020 2020 2020 2020  filter(.        
-00002dd0: 2020 2020 6c61 6d62 6461 2072 6563 6f72      lambda recor
-00002de0: 643a 206e 6f74 2072 6563 6f72 642e 6765  d: not record.ge
-00002df0: 7428 2265 7665 6e74 5479 7065 2229 0a20  t("eventType"). 
-00002e00: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00002e10: 2065 7665 6e74 735f 7769 7468 6f75 745f   events_without_
-00002e20: 7479 7065 735f 7769 7468 5f62 6174 6368  types_with_batch
-00002e30: 2e75 7365 5f63 6163 6865 2829 0a20 2020  .use_cache().   
-00002e40: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
-00002e50: 5b31 2e31 315d 2044 6174 6120 6f62 6a65  [1.11] Data obje
-00002e60: 6374 7320 6a6f 696e 696e 672e 0a20 2020  cts joining..   
-00002e70: 2020 2020 2023 2059 6f75 2068 6176 6520       # You have 
-00002e80: 7468 6520 666f 6c6c 6f77 696e 6720 3320  the following 3 
-00002e90: 4461 7461 206f 626a 6563 7473 2e0a 2020  Data objects..  
-00002ea0: 2020 2020 2020 6431 203d 2044 6174 6128        d1 = Data(
-00002eb0: 5b31 2c20 322c 2033 5d29 0a20 2020 2020  [1, 2, 3]).     
-00002ec0: 2020 2064 3220 3d20 4461 7461 285b 2261     d2 = Data(["a
-00002ed0: 222c 207b 2269 6422 3a20 3132 337d 2c20  ", {"id": 123}, 
-00002ee0: 2263 225d 290a 2020 2020 2020 2020 6433  "c"]).        d3
-00002ef0: 203d 2044 6174 6128 5b37 2c20 382c 2039   = Data([7, 8, 9
-00002f00: 5d29 0a20 2020 2020 2020 2023 2059 6f75  ]).        # You
-00002f10: 2063 616e 206a 6f69 6e20 4461 7461 206f   can join Data o
-00002f20: 626a 6563 7473 2069 6e20 666f 6c6c 6f77  bjects in follow
-00002f30: 696e 6720 7761 7973 2e0a 2020 2020 2020  ing ways..      
-00002f40: 2020 2320 506c 6561 7365 206e 6f74 652c    # Please note,
-00002f50: 206e 6577 2044 6174 6120 6f62 6a65 6374   new Data object
-00002f60: 2077 696c 6c20 6861 7665 2063 6163 6865   will have cache
-00002f70: 2073 7461 7475 7320 3d3d 2046 616c 7365   status == False
-00002f80: 2e0a 2020 2020 2020 2020 6461 7461 5f76  ..        data_v
-00002f90: 6961 5f69 6e69 7420 3d20 4461 7461 285b  ia_init = Data([
-00002fa0: 6431 2c20 6432 2c20 6433 5d29 0a20 2020  d1, d2, d3]).   
-00002fb0: 2020 2020 2064 6174 615f 7669 615f 6164       data_via_ad
-00002fc0: 6420 3d20 6431 202b 2064 3220 2b20 6433  d = d1 + d2 + d3
-00002fd0: 0a20 2020 2020 2020 2064 6174 615f 7769  .        data_wi
-00002fe0: 7468 5f6e 6f6e 5f64 6174 615f 6f62 6a5f  th_non_data_obj_
-00002ff0: 7669 615f 696e 6974 203d 2044 6174 6128  via_init = Data(
-00003000: 5b64 312c 205b 2261 222c 207b 2269 6422  [d1, ["a", {"id"
-00003010: 3a20 3132 337d 2c20 2263 225d 2c20 6433  : 123}, "c"], d3
-00003020: 5d29 0a20 2020 2020 2020 2064 6174 615f  ]).        data_
-00003030: 7769 7468 5f6e 6f6e 5f64 6174 615f 6f62  with_non_data_ob
-00003040: 6a5f 7669 615f 6164 6420 3d20 6431 202b  j_via_add = d1 +
-00003050: 205b 2261 222c 207b 2269 6422 3a20 3132   ["a", {"id": 12
-00003060: 337d 2c20 2263 225d 202b 2064 330a 2020  3}, "c"] + d3.  
-00003070: 2020 2020 2020 2320 596f 7520 6361 6e20        # You can 
-00003080: 6a6f 696e 2063 7572 7265 6e74 2044 6174  join current Dat
-00003090: 6120 6f62 6a65 6374 206f 6e20 706c 6163  a object on plac
-000030a0: 6520 7573 696e 6720 2b3d 2e0a 2020 2020  e using +=..    
-000030b0: 2020 2020 2320 4974 2077 696c 6c20 6b65      # It will ke
-000030c0: 6570 2063 6163 6865 2073 7461 7475 732e  ep cache status.
-000030d0: 0a20 2020 2020 2020 2064 3120 2b3d 2064  .        d1 += d
-000030e0: 3320 2023 2064 3120 7769 6c6c 2062 6563  3  # d1 will bec
-000030f0: 6f6d 6520 4461 7461 285b 312c 322c 332c  ome Data([1,2,3,
-00003100: 372c 382c 395d 290a 2020 2020 2020 2020  7,8,9]).        
-00003110: 0a20 2020 2020 2020 2023 205b 312e 3132  .        # [1.12
-00003120: 5d20 4275 696c 6420 616e 6420 7265 6164  ] Build and read
-00003130: 2044 6174 6120 6f62 6a65 6374 2063 6163   Data object cac
-00003140: 6865 2066 696c 6573 2e0a 2020 2020 2020  he files..      
-00003150: 2020 6576 656e 7473 2e62 7569 6c64 5f63    events.build_c
-00003160: 6163 6865 2822 6361 6368 655f 6669 6c65  ache("cache_file
-00003170: 6e61 6d65 5f6f 725f 7061 7468 2229 0a20  name_or_path"). 
-00003180: 2020 2020 2020 2064 6174 615f 6f62 6a5f         data_obj_
-00003190: 6672 6f6d 5f63 6163 6865 203d 2044 6174  from_cache = Dat
-000031a0: 612e 6672 6f6d 5f63 6163 6865 5f66 696c  a.from_cache_fil
-000031b0: 6528 2263 6163 6865 5f66 696c 656e 616d  e("cache_filenam
-000031c0: 655f 6f72 5f70 6174 6822 290a 2020 2020  e_or_path").    
-000031d0: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-000031e0: 312e 3133 5d20 4368 6563 6b20 6966 2044  1.13] Check if D
-000031f0: 6174 6120 6973 2073 6f72 7465 642e 0a20  ata is sorted.. 
-00003200: 2020 2020 2020 2069 735f 736f 7274 6564         is_sorted
-00003210: 203d 2065 7665 6e74 732e 6973 5f73 6f72   = events.is_sor
-00003220: 7465 6428 6c61 6d62 6461 2065 3a20 655b  ted(lambda e: e[
-00003230: 2273 7461 7274 5469 6d65 7374 616d 7022  "startTimestamp"
-00003240: 5d5b 2265 706f 6368 5365 636f 6e64 225d  ]["epochSecond"]
-00003250: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-00003260: 2020 2023 205b 325d 2057 6f72 6b69 6e67     # [2] Working
-00003270: 2077 6974 6820 636f 6e76 6572 7465 7273   with converters
-00003280: 2e0a 2020 2020 2020 2020 2320 5468 6572  ..        # Ther
-00003290: 6520 6172 6520 6375 7272 656e 746c 7920  e are currently 
-000032a0: 7468 7265 6520 696d 706c 656d 656e 7461  three implementa
-000032b0: 7469 6f6e 7320 6f66 2049 5469 6d65 7374  tions of ITimest
-000032c0: 616d 7043 6f6e 7665 7274 6572 2063 6c61  ampConverter cla
-000032d0: 7373 3a20 4461 7465 7469 6d65 436f 6e76  ss: DatetimeConv
-000032e0: 6572 7465 2c20 4461 7465 7469 6d65 5374  erte, DatetimeSt
-000032f0: 7269 6e67 436f 6e76 6572 7465 7220 616e  ringConverter an
-00003300: 6420 5072 6f74 6f62 7566 5469 6d65 7374  d ProtobufTimest
-00003310: 616d 7043 6f6e 7665 7274 6572 2e0a 2020  ampConverter..  
-00003320: 2020 2020 2020 2320 5468 6579 2061 6c6c        # They all
-00003330: 2069 6d70 6c65 6d65 6e74 2073 616d 6520   implement same 
-00003340: 6d65 7468 6f64 7320 6672 6f6d 2062 6173  methods from bas
-00003350: 6520 636c 6173 732e 0a20 2020 2020 2020  e class..       
-00003360: 2023 204e 6f74 6520 7468 6174 2073 6f6d   # Note that som
-00003370: 6520 6163 6375 7261 6379 206d 6179 2062  e accuracy may b
-00003380: 6520 6c6f 7374 2064 7572 696e 6720 636f  e lost during co
-00003390: 6e76 6572 7369 6f6e 2e0a 2020 2020 2020  nversion..      
-000033a0: 2020 2320 4966 2066 6f72 2065 7861 6d70    # If for examp
-000033b0: 6c65 2079 6f75 2075 7365 2074 6f5f 6d69  le you use to_mi
-000033c0: 6372 6f73 6563 6f6e 6473 206e 616e 6f73  croseconds nanos
-000033d0: 6563 6f6e 6473 2077 696c 6c20 6265 2063  econds will be c
-000033e0: 7574 206f 6666 2069 6e73 7465 6164 206f  ut off instead o
-000033f0: 6620 726f 756e 6469 6e67 2e0a 2020 2020  f rounding..    
-00003400: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-00003410: 322e 315d 2044 6174 6574 696d 6543 6f6e  2.1] DatetimeCon
-00003420: 7665 7274 6572 2e0a 2020 2020 2020 2020  verter..        
-00003430: 2320 4461 7465 7469 6d65 436f 6e76 6572  # DatetimeConver
-00003440: 7465 7220 7461 6b65 7320 6461 7465 7469  ter takes dateti
-00003450: 6d65 2e64 6174 6574 696d 6520 6f62 6a65  me.datetime obje
-00003460: 6374 2061 7320 696e 7075 742e 0a20 2020  ct as input..   
-00003470: 2020 2020 200a 2020 2020 2020 2020 6461       .        da
-00003480: 7465 7469 6d65 5f6f 626a 203d 2064 6174  tetime_obj = dat
-00003490: 6574 696d 6528 7965 6172 3d32 3032 332c  etime(year=2023,
-000034a0: 206d 6f6e 7468 3d31 2c20 6461 793d 352c   month=1, day=5,
-000034b0: 2068 6f75 723d 3134 2c20 6d69 6e75 7465   hour=14, minute
-000034c0: 3d33 382c 2073 6563 6f6e 643d 3235 2c20  =38, second=25, 
-000034d0: 6d69 6372 6f73 6563 6f6e 643d 3134 3630  microsecond=1460
-000034e0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-000034f0: 2020 2023 2049 7420 6861 7320 6d65 7468     # It has meth
-00003500: 6f64 7320 7468 6174 2072 6574 7572 6e20  ods that return 
-00003510: 7468 6520 6461 7465 7469 6d65 2069 6e20  the datetime in 
-00003520: 6469 6666 6572 656e 7420 666f 726d 6173  different formas
-00003530: 3a0a 2020 2020 2020 2020 0a20 2020 2020  :.        .     
-00003540: 2020 2064 6174 655f 6d73 203d 2044 6174     date_ms = Dat
-00003550: 6574 696d 6543 6f6e 7665 7274 6572 2e74  etimeConverter.t
-00003560: 6f5f 6d69 6c6c 6973 6563 6f6e 6473 2864  o_milliseconds(d
-00003570: 6174 6574 696d 655f 6f62 6a29 0a20 2020  atetime_obj).   
-00003580: 2020 2020 2064 6174 655f 7573 203d 2044       date_us = D
-00003590: 6174 6574 696d 6543 6f6e 7665 7274 6572  atetimeConverter
-000035a0: 2e74 6f5f 6d69 6372 6f73 6563 6f6e 6473  .to_microseconds
-000035b0: 2864 6174 6574 696d 655f 6f62 6a29 0a20  (datetime_obj). 
-000035c0: 2020 2020 2020 2023 2043 6f6e 7665 7274         # Convert
-000035d0: 696e 6720 746f 206e 616e 6f73 6563 6f6e  ing to nanosecon
-000035e0: 6473 206a 7573 7473 2061 6464 7320 7468  ds justs adds th
-000035f0: 7265 6520 7472 6169 6c69 6e67 207a 6572  ree trailing zer
-00003600: 6f73 2061 7320 6461 7465 7469 6d65 206f  os as datetime o
-00003610: 626a 6563 7420 646f 6573 6e27 7420 6861  bject doesn't ha
-00003620: 7665 206e 616e 6f73 6563 6f6e 6473 2e0a  ve nanoseconds..
-00003630: 2020 2020 2020 2020 6461 7465 5f6e 7320          date_ns 
-00003640: 3d20 4461 7465 7469 6d65 436f 6e76 6572  = DatetimeConver
-00003650: 7465 722e 746f 5f6e 616e 6f73 6563 6f6e  ter.to_nanosecon
-00003660: 6473 2864 6174 6574 696d 655f 6f62 6a29  ds(datetime_obj)
-00003670: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00003680: 2020 2320 5b32 2e32 5d20 4461 7465 7469    # [2.2] Dateti
-00003690: 6d65 5374 7269 6e67 436f 6e76 6572 7465  meStringConverte
-000036a0: 720a 2020 2020 2020 2020 2320 4461 7465  r.        # Date
-000036b0: 7469 6d65 5374 7269 6e67 436f 6e76 6572  timeStringConver
-000036c0: 7465 7220 7461 6b65 7320 7374 7269 6e67  ter takes string
-000036d0: 2069 6e20 2279 7979 792d 4d4d 2d64 6454   in "yyyy-MM-ddT
-000036e0: 4848 3a6d 6d3a 7373 5b2e 5353 5353 5353  HH:mm:ss[.SSSSSS
-000036f0: 5353 535d 5a22 2066 6f72 6d61 742e 0a20  SSS]Z" format.. 
-00003700: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00003710: 6461 7465 5f73 7472 696e 6720 3d20 2232  date_string = "2
-00003720: 3032 332d 3031 2d30 3554 3134 3a33 383a  023-01-05T14:38:
-00003730: 3235 2e30 3031 3436 5a22 0a20 2020 2020  25.00146Z".     
-00003740: 2020 200a 2020 2020 2020 2020 2320 5765     .        # We
-00003750: 2068 6176 6520 7361 6d65 206d 6574 686f   have same metho
-00003760: 6473 2061 7320 696e 2044 6174 6574 696d  ds as in Datetim
-00003770: 6543 6f6e 7665 7274 6572 0a20 2020 2020  eConverter.     
-00003780: 2020 2064 6174 655f 6d73 5f66 726f 6d5f     date_ms_from_
-00003790: 7374 7269 6e67 203d 2044 6174 6574 696d  string = Datetim
-000037a0: 6553 7472 696e 6743 6f6e 7665 7274 6572  eStringConverter
-000037b0: 2e74 6f5f 6d69 6c6c 6973 6563 6f6e 6473  .to_milliseconds
-000037c0: 2864 6174 655f 7374 7269 6e67 290a 2020  (date_string).  
-000037d0: 2020 2020 2020 6461 7465 5f75 735f 6672        date_us_fr
-000037e0: 6f6d 5f73 7472 696e 6720 3d20 4461 7465  om_string = Date
-000037f0: 7469 6d65 5374 7269 6e67 436f 6e76 6572  timeStringConver
-00003800: 7465 722e 746f 5f6d 6963 726f 7365 636f  ter.to_microseco
-00003810: 6e64 7328 6461 7465 5f73 7472 696e 6729  nds(date_string)
-00003820: 0a20 2020 2020 2020 2064 6174 655f 6e73  .        date_ns
-00003830: 5f66 726f 6d5f 7374 7269 6e67 203d 2044  _from_string = D
-00003840: 6174 6574 696d 6553 7472 696e 6743 6f6e  atetimeStringCon
-00003850: 7665 7274 6572 2e74 6f5f 6e61 6e6f 7365  verter.to_nanose
-00003860: 636f 6e64 7328 6461 7465 5f73 7472 696e  conds(date_strin
-00003870: 6729 0a20 2020 2020 2020 200a 2020 2020  g).        .    
-00003880: 2020 2020 2320 5765 2063 616e 2061 6c73      # We can als
-00003890: 6f20 6765 7420 6461 7465 7469 6d65 206f  o get datetime o
-000038a0: 626a 6563 7420 6672 6f6d 2073 7472 696e  bject from strin
-000038b0: 670a 2020 2020 2020 2020 6461 7465 7469  g.        dateti
-000038c0: 6d65 5f66 726f 6d5f 7374 7269 6e67 203d  me_from_string =
-000038d0: 2044 6174 6574 696d 6553 7472 696e 6743   DatetimeStringC
-000038e0: 6f6e 7665 7274 6572 2e74 6f5f 6461 7465  onverter.to_date
-000038f0: 7469 6d65 2864 6174 655f 7374 7269 6e67  time(date_string
-00003900: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-00003910: 2020 2023 205b 322e 335d 2050 726f 746f     # [2.3] Proto
-00003920: 6275 6654 696d 6573 7461 6d70 436f 6e76  bufTimestampConv
-00003930: 6572 7465 720a 2020 2020 2020 2020 2320  erter.        # 
-00003940: 5072 6f74 6f62 7566 2074 696d 6573 7461  Protobuf timesta
-00003950: 6d70 7320 6d75 7374 2062 6520 696e 2066  mps must be in f
-00003960: 6f72 6d20 7b22 6570 6f63 6853 6563 6f6e  orm {"epochSecon
-00003970: 6422 3a20 7365 636f 6e64 732c 2022 6e61  d": seconds, "na
-00003980: 6e6f 223a 206e 616e 6f73 6563 6f6e 6473  no": nanoseconds
-00003990: 7d0a 2020 2020 2020 2020 0a20 2020 2020  }.        .     
-000039a0: 2020 2070 726f 746f 6275 665f 7469 6d65     protobuf_time
-000039b0: 7374 616d 7020 3d20 7b22 6570 6f63 6853  stamp = {"epochS
-000039c0: 6563 6f6e 6422 3a20 3136 3732 3932 3935  econd": 16729295
-000039d0: 3035 2c20 226e 616e 6f22 3a20 315f 3436  05, "nano": 1_46
-000039e0: 305f 3030 307d 0a20 2020 2020 2020 200a  0_000}.        .
-000039f0: 2020 2020 2020 2020 6461 7465 5f6d 735f          date_ms_
-00003a00: 6672 6f6d 5f74 696d 6573 7461 6d70 203d  from_timestamp =
-00003a10: 2050 726f 746f 6275 6654 696d 6573 7461   ProtobufTimesta
-00003a20: 6d70 436f 6e76 6572 7465 722e 746f 5f6d  mpConverter.to_m
-00003a30: 696c 6c69 7365 636f 6e64 7328 7072 6f74  illiseconds(prot
-00003a40: 6f62 7566 5f74 696d 6573 7461 6d70 290a  obuf_timestamp).
-00003a50: 2020 2020 2020 2020 6461 7465 5f75 735f          date_us_
-00003a60: 6672 6f6d 5f74 696d 6573 7461 6d70 203d  from_timestamp =
-00003a70: 2050 726f 746f 6275 6654 696d 6573 7461   ProtobufTimesta
-00003a80: 6d70 436f 6e76 6572 7465 722e 746f 5f6d  mpConverter.to_m
-00003a90: 6963 726f 7365 636f 6e64 7328 7072 6f74  icroseconds(prot
-00003aa0: 6f62 7566 5f74 696d 6573 7461 6d70 290a  obuf_timestamp).
-00003ab0: 2020 2020 2020 2020 6461 7465 5f6e 735f          date_ns_
-00003ac0: 6672 6f6d 5f74 696d 6573 7461 6d70 203d  from_timestamp =
-00003ad0: 2050 726f 746f 6275 6654 696d 6573 7461   ProtobufTimesta
-00003ae0: 6d70 436f 6e76 6572 7465 722e 746f 5f6e  mpConverter.to_n
-00003af0: 616e 6f73 6563 6f6e 6473 2870 726f 746f  anoseconds(proto
-00003b00: 6275 665f 7469 6d65 7374 616d 7029 0a20  buf_timestamp). 
-00003b10: 2020 2020 2020 2064 6174 6574 696d 655f         datetime_
-00003b20: 6672 6f6d 5f74 696d 6573 7461 6d70 203d  from_timestamp =
-00003b30: 2050 726f 746f 6275 6654 696d 6573 7461   ProtobufTimesta
-00003b40: 6d70 436f 6e76 6572 7465 722e 746f 5f64  mpConverter.to_d
-00003b50: 6174 6574 696d 6528 7072 6f74 6f62 7566  atetime(protobuf
-00003b60: 5f74 696d 6573 7461 6d70 290a 2020 2020  _timestamp).    
-00003b70: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-00003b80: 335d 2057 6f72 6b69 6e67 2077 6974 6820  3] Working with 
-00003b90: 4576 656e 7454 7265 6520 616e 6420 4576  EventTree and Ev
-00003ba0: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
-00003bb0: 6e2e 0a20 2020 2020 2020 200a 2020 2020  n..        .    
-00003bc0: 2020 2020 2320 5b33 2e31 5d20 4275 696c      # [3.1] Buil
-00003bd0: 6420 6120 6375 7374 6f6d 2045 7665 6e74  d a custom Event
-00003be0: 5472 6565 0a20 2020 2020 2020 2023 2054  Tree.        # T
-00003bf0: 6f20 6372 6561 7465 2061 6e20 4576 656e  o create an Even
-00003c00: 7454 7265 6520 6f62 6a65 6374 2079 6f75  tTree object you
-00003c10: 206e 6565 6420 746f 2070 726f 7669 6465   need to provide
-00003c20: 206e 616d 652c 2069 6420 616e 6420 6461   name, id and da
-00003c30: 7461 206f 6620 7468 6520 726f 6f74 2065  ta of the root e
-00003c40: 7665 6e74 2e0a 2020 2020 2020 2020 7472  vent..        tr
-00003c50: 6565 203d 2045 7665 6e74 5472 6565 2865  ee = EventTree(e
-00003c60: 7665 6e74 5f6e 616d 653d 2272 6f6f 7420  vent_name="root 
-00003c70: 6576 656e 7422 2c20 6576 656e 745f 6964  event", event_id
-00003c80: 3d22 726f 6f74 5f69 6422 2c20 6461 7461  ="root_id", data
-00003c90: 3d7b 2264 6174 6122 3a20 5b31 2c20 322c  ={"data": [1, 2,
-00003ca0: 2033 2c20 342c 2035 5d7d 290a 2020 2020   3, 4, 5]}).    
-00003cb0: 2020 2020 0a20 2020 2020 2020 2023 2054      .        # T
-00003cc0: 6f20 6164 6420 6e65 7720 6e6f 6465 2075  o add new node u
-00003cd0: 7365 2061 7070 656e 645f 6576 656e 742e  se append_event.
-00003ce0: 2070 6172 656e 745f 6964 2069 7320 6e65   parent_id is ne
-00003cf0: 6365 7373 6172 792c 2064 6174 6120 6973  cessary, data is
-00003d00: 206f 7074 696f 6e61 6c2e 0a20 2020 2020   optional..     
-00003d10: 2020 2074 7265 652e 6170 7065 6e64 5f65     tree.append_e
-00003d20: 7665 6e74 2865 7665 6e74 5f6e 616d 653d  vent(event_name=
-00003d30: 2241 222c 2065 7665 6e74 5f69 643d 2241  "A", event_id="A
-00003d40: 5f69 6422 2c20 6461 7461 3d4e 6f6e 652c  _id", data=None,
-00003d50: 2070 6172 656e 745f 6964 3d22 726f 6f74   parent_id="root
-00003d60: 5f69 6422 290a 2020 2020 2020 2020 0a20  _id").        . 
-00003d70: 2020 2020 2020 2023 205b 332e 335d 2042         # [3.3] B
-00003d80: 7569 6c64 696e 6720 7468 6520 4576 656e  uilding the Even
-00003d90: 7454 7265 6543 6f6c 6c65 6374 696f 6e2e  tTreeCollection.
-00003da0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00003db0: 2020 2320 4966 2079 6f75 2064 6f6e 2774    # If you don't
-00003dc0: 2073 7065 6369 6679 2064 6174 615f 736f   specify data_so
-00003dd0: 7572 6365 2066 6f72 2074 6865 2064 7269  urce for the dri
-00003de0: 7665 7220 7468 656e 2069 7420 776f 6e27  ver then it won'
-00003df0: 7420 7265 636f 7665 7220 6465 7461 6368  t recover detach
-00003e00: 6564 2065 7665 6e74 732e 0a20 2020 2020  ed events..     
-00003e10: 2020 2064 7269 7665 723a 2049 4554 4344     driver: IETCD
-00003e20: 7269 7665 7220 2023 2059 6f75 2073 686f  river  # You sho
-00003e30: 756c 6420 696e 6974 2045 5443 4472 6976  uld init ETCDriv
-00003e40: 6572 206f 626a 6563 742e 2045 2e67 2e20  er object. E.g. 
-00003e50: 6672 6f6d 204c 7744 5020 6d6f 6475 6c65  from LwDP module
-00003e60: 206f 7220 796f 7572 2063 7573 746f 6d20   or your custom 
-00003e70: 636c 6173 732e 0a20 2020 2020 2020 2065  class..        e
-00003e80: 7463 203d 2045 7665 6e74 5472 6565 436f  tc = EventTreeCo
-00003e90: 6c6c 6563 7469 6f6e 2864 7269 7665 7229  llection(driver)
-00003ea0: 0a20 2020 2020 2020 2065 7463 2e62 7569  .        etc.bui
-00003eb0: 6c64 2865 7665 6e74 7329 0a20 2020 2020  ld(events).     
-00003ec0: 2020 200a 2020 2020 2020 2020 2320 4465     .        # De
-00003ed0: 7461 6368 6564 2065 7665 6e74 7320 6973  tached events is
-00003ee0: 6e27 7420 656d 7074 792e 0a20 2020 2020  n't empty..     
-00003ef0: 2020 2061 7373 6572 7420 6574 632e 6765     assert etc.ge
-00003f00: 745f 6465 7461 6368 6564 5f65 7665 6e74  t_detached_event
-00003f10: 7328 290a 2020 2020 2020 2020 0a20 2020  s().        .   
-00003f20: 2020 2020 2065 7463 203d 2045 7665 6e74       etc = Event
-00003f30: 5472 6565 436f 6c6c 6563 7469 6f6e 2864  TreeCollection(d
-00003f40: 7269 7665 7229 0a20 2020 2020 2020 2023  river).        #
-00003f50: 2044 6574 6163 6865 6420 6576 656e 7473   Detached events
-00003f60: 2061 7265 2065 6d70 7479 2062 6563 6175   are empty becau
-00003f70: 7365 2074 6865 7920 7765 7265 2072 6563  se they were rec
-00003f80: 6f76 6572 6564 2e0a 2020 2020 2020 2020  overed..        
-00003f90: 6173 7365 7274 206e 6f74 2065 7463 2e67  assert not etc.g
-00003fa0: 6574 5f64 6574 6163 6865 645f 6576 656e  et_detached_even
-00003fb0: 7473 2829 0a20 2020 2020 2020 200a 2020  ts().        .  
-00003fc0: 2020 2020 2020 2320 5468 6520 636f 6c6c        # The coll
-00003fd0: 6563 7469 6f6e 2068 6173 2045 7665 6e74  ection has Event
-00003fe0: 5472 6565 7320 6561 6368 2077 6974 6820  Trees each with 
-00003ff0: 6120 7472 6565 206f 6620 6576 656e 7473  a tree of events
-00004000: 2e0a 2020 2020 2020 2020 2320 5573 696e  ..        # Usin
-00004010: 6720 436f 6c6c 6563 7469 6f6e 2061 6e64  g Collection and
-00004020: 2045 7665 6e74 5472 6565 732c 2079 6f75   EventTrees, you
-00004030: 2063 616e 2077 6f72 6b20 666c 6578 6962   can work flexib
-00004040: 6c79 2077 6974 6820 6576 656e 7473 2e0a  ly with events..
-00004050: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00004060: 2023 205b 332e 332e 315d 2047 6574 206c   # [3.3.1] Get l
-00004070: 6561 7665 7320 6f66 2061 6c6c 2074 7265  eaves of all tre
-00004080: 6573 2e0a 2020 2020 2020 2020 6c65 6176  es..        leav
-00004090: 6573 3a20 5475 706c 655b 6469 6374 5d20  es: Tuple[dict] 
-000040a0: 3d20 6574 632e 6765 745f 6c65 6176 6573  = etc.get_leaves
-000040b0: 2829 0a20 2020 2020 2020 200a 2020 2020  ().        .    
-000040c0: 2020 2020 2320 5b33 2e33 2e32 5d20 4765      # [3.3.2] Ge
-000040d0: 7420 726f 6f74 7320 6964 7320 6f66 2061  t roots ids of a
-000040e0: 6c6c 2074 7265 6573 2e0a 2020 2020 2020  ll trees..      
-000040f0: 2020 726f 6f74 733a 204c 6973 745b 7374    roots: List[st
-00004100: 725d 203d 2065 7463 2e67 6574 5f72 6f6f  r] = etc.get_roo
-00004110: 7473 5f69 6473 2829 0a20 2020 2020 2020  ts_ids().       
-00004120: 200a 2020 2020 2020 2020 2320 5b33 2e33   .        # [3.3
-00004130: 2e33 5d20 4669 6e64 2061 6e20 6576 656e  .3] Find an even
-00004140: 7420 696e 2061 6c6c 2074 7265 6573 2e0a  t in all trees..
-00004150: 2020 2020 2020 2020 6669 6e64 5f65 7665          find_eve
-00004160: 6e74 3a20 4f70 7469 6f6e 616c 5b64 6963  nt: Optional[dic
-00004170: 745d 203d 2065 7463 2e66 696e 6428 6c61  t] = etc.find(la
-00004180: 6d62 6461 2065 7665 6e74 3a20 2253 656e  mbda event: "Sen
-00004190: 6420 6d65 7373 6167 6522 2069 6e20 6576  d message" in ev
-000041a0: 656e 745b 2265 7665 6e74 5479 7065 225d  ent["eventType"]
-000041b0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-000041c0: 2020 2023 205b 332e 332e 345d 2046 696e     # [3.3.4] Fin
-000041d0: 6420 616c 6c20 6576 656e 7473 2069 6e20  d all events in 
-000041e0: 616c 6c20 7472 6565 732e 2054 6865 7265  all trees. There
-000041f0: 2069 7320 616c 736f 2069 7465 7261 626c   is also iterabl
-00004200: 6520 7665 7273 696f 6e20 2766 696e 6461  e version 'finda
-00004210: 6c6c 5f69 7465 7227 2e0a 2020 2020 2020  ll_iter'..      
-00004220: 2020 6669 6e64 5f65 7665 6e74 733a 204c    find_events: L
-00004230: 6973 745b 6469 6374 5d20 3d20 6574 632e  ist[dict] = etc.
-00004240: 6669 6e64 616c 6c28 6c61 6d62 6461 2065  findall(lambda e
-00004250: 7665 6e74 3a20 6576 656e 745b 2273 7563  vent: event["suc
-00004260: 6365 7373 6675 6c22 5d20 6973 2054 7275  cessful"] is Tru
-00004270: 6529 0a20 2020 2020 2020 200a 2020 2020  e).        .    
-00004280: 2020 2020 2320 5b33 2e33 2e35 5d20 4669      # [3.3.5] Fi
-00004290: 6e64 2061 6e20 616e 6365 7374 6f72 206f  nd an ancestor o
-000042a0: 6620 7468 6520 6576 656e 742e 0a20 2020  f the event..   
-000042b0: 2020 2020 2061 6e63 6573 746f 723a 204f       ancestor: O
-000042c0: 7074 696f 6e61 6c5b 6469 6374 5d20 3d20  ptional[dict] = 
-000042d0: 6574 632e 6669 6e64 5f61 6e63 6573 746f  etc.find_ancesto
-000042e0: 7228 0a20 2020 2020 2020 2020 2020 2022  r(.            "
-000042f0: 3862 6265 3337 3137 2d63 6635 392d 3131  8bbe3717-cf59-11
-00004300: 6562 2d61 3366 372d 3039 3466 3930 3463  eb-a3f7-094f904c
-00004310: 3361 3632 222c 2066 696c 7465 723d 6c61  3a62", filter=la
-00004320: 6d62 6461 2065 7665 6e74 3a20 2252 6f6f  mbda event: "Roo
-00004330: 7445 7665 6e74 2220 696e 2065 7665 6e74  tEvent" in event
-00004340: 5b22 6576 656e 744e 616d 6522 5d0a 2020  ["eventName"].  
-00004350: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00004360: 0a20 2020 2020 2020 2023 205b 332e 332e  .        # [3.3.
-00004370: 365d 2047 6574 2063 6869 6c64 7265 6e20  6] Get children 
-00004380: 6f66 2074 6865 2065 7665 6e74 2e20 5468  of the event. Th
-00004390: 6572 6520 6973 2061 6c73 6f20 6974 6572  ere is also iter
-000043a0: 6162 6c65 2076 6572 7369 6f6e 2027 6765  able version 'ge
-000043b0: 745f 6368 696c 6472 656e 5f69 7465 7227  t_children_iter'
-000043c0: 2e0a 2020 2020 2020 2020 6368 696c 6472  ..        childr
-000043d0: 656e 3a20 5475 706c 655b 6469 6374 5d20  en: Tuple[dict] 
-000043e0: 3d20 6574 632e 6765 745f 6368 696c 6472  = etc.get_childr
-000043f0: 656e 2822 3831 3434 3232 6531 2d39 6336  en("814422e1-9c6
-00004400: 382d 3131 6562 2d38 3539 382d 3639 3165  8-11eb-8598-691e
-00004410: 6264 3766 3431 3364 2229 0a20 2020 2020  bd7f413d").     
-00004420: 2020 200a 2020 2020 2020 2020 2320 5b33     .        # [3
-00004430: 2e33 2e37 5d20 4765 7420 7375 6274 7265  .3.7] Get subtre
-00004440: 6520 666f 7220 7370 6563 6966 6965 6420  e for specified 
-00004450: 6576 656e 742e 0a20 2020 2020 2020 2073  event..        s
-00004460: 7562 7472 6565 3a20 4576 656e 7454 7265  ubtree: EventTre
-00004470: 6520 3d20 6574 632e 6765 745f 7375 6274  e = etc.get_subt
-00004480: 7265 6528 2238 6532 3337 3734 642d 6366  ree("8e23774d-cf
-00004490: 3539 2d31 3165 622d 6136 6533 2d35 3562  59-11eb-a6e3-55b
-000044a0: 6664 6232 6233 6632 3122 290a 2020 2020  fdb2b3f21").    
-000044b0: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-000044c0: 332e 332e 385d 2047 6574 2066 756c 6c20  3.3.8] Get full 
-000044d0: 7061 7468 2074 6f20 7468 6520 6576 656e  path to the even
-000044e0: 742e 0a20 2020 2020 2020 2023 204c 6f6f  t..        # Loo
-000044f0: 6b73 206c 696b 6520 5b61 6e63 6573 746f  ks like [ancesto
-00004500: 725f 726f 6f74 2c20 616e 6365 7374 6f72  r_root, ancestor
-00004510: 5f6c 6576 656c 312c 2061 6e63 6573 746f  _level1, ancesto
-00004520: 725f 6c65 7665 6c32 2c20 6576 656e 745d  r_level2, event]
-00004530: 0a20 2020 2020 2020 2065 7665 6e74 5f70  .        event_p
-00004540: 6174 683a 204c 6973 745b 6469 6374 5d20  ath: List[dict] 
-00004550: 3d20 6574 632e 6765 745f 6675 6c6c 5f70  = etc.get_full_p
-00004560: 6174 6828 2238 6532 3532 3466 612d 6366  ath("8e2524fa-cf
-00004570: 3539 2d31 3165 622d 6133 6637 2d30 3934  59-11eb-a3f7-094
-00004580: 6639 3034 6333 6136 3222 290a 2020 2020  f904c3a62").    
-00004590: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-000045a0: 332e 332e 395d 2047 6574 2070 6172 656e  3.3.9] Get paren
-000045b0: 7420 6f66 2074 6865 2065 7665 6e74 2e0a  t of the event..
-000045c0: 2020 2020 2020 2020 7061 7265 6e74 203d          parent =
-000045d0: 2065 7463 2e67 6574 5f70 6172 656e 7428   etc.get_parent(
-000045e0: 2238 6532 3532 3466 612d 6366 3539 2d31  "8e2524fa-cf59-1
-000045f0: 3165 622d 6133 6637 2d30 3934 6639 3034  1eb-a3f7-094f904
-00004600: 6333 6136 3222 290a 2020 2020 2020 2020  c3a62").        
-00004610: 0a20 2020 2020 2020 2023 205b 332e 332e  .        # [3.3.
-00004620: 3130 5d20 4170 7065 6e64 206e 6577 2065  10] Append new e
-00004630: 7665 6e74 2074 6f20 7468 6520 636f 6c6c  vent to the coll
-00004640: 6563 7469 6f6e 2e0a 2020 2020 2020 2020  ection..        
-00004650: 6574 632e 6170 7065 6e64 5f65 7665 6e74  etc.append_event
-00004660: 280a 2020 2020 2020 2020 2020 2020 6576  (.            ev
-00004670: 656e 743d 7b0a 2020 2020 2020 2020 2020  ent={.          
-00004680: 2020 2020 2020 2265 7665 6e74 4964 223a        "eventId":
-00004690: 2022 6132 3066 3565 6634 2d63 3366 652d   "a20f5ef4-c3fe-
-000046a0: 6262 3130 2d61 3239 632d 6464 3364 3738  bb10-a29c-dd3d78
-000046b0: 3439 3039 6562 222c 0a20 2020 2020 2020  4909eb",.       
-000046c0: 2020 2020 2020 2020 2022 7061 7265 6e74           "parent
-000046d0: 4576 656e 7449 6422 3a20 2238 6532 3532  EventId": "8e252
-000046e0: 3466 612d 6366 3539 2d31 3165 622d 6133  4fa-cf59-11eb-a3
-000046f0: 6637 2d30 3934 6639 3034 6333 6136 3222  f7-094f904c3a62"
-00004700: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00004710: 2020 2265 7665 6e74 4e61 6d65 223a 2022    "eventName": "
-00004720: 5374 7562 4576 656e 7422 2c0a 2020 2020  StubEvent",.    
-00004730: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00004740: 2020 290a 2020 2020 2020 2020 0a20 2020    ).        .   
-00004750: 2020 2020 2023 205b 332e 332e 3131 5d20       # [3.3.11] 
-00004760: 5368 6f77 2074 6865 2065 6e74 6972 6520  Show the entire 
-00004770: 636f 6c6c 6563 7469 6f6e 2e0a 2020 2020  collection..    
-00004780: 2020 2020 6574 632e 7368 6f77 2829 0a20      etc.show(). 
-00004790: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000047a0: 2320 5b33 2e34 5d20 576f 726b 696e 6720  # [3.4] Working 
-000047b0: 7769 7468 2074 6865 2045 7665 6e74 5472  with the EventTr
-000047c0: 6565 2e0a 2020 2020 2020 2020 2320 4576  ee..        # Ev
-000047d0: 656e 7454 7265 6520 6861 7320 7468 6520  entTree has the 
-000047e0: 7361 6d65 206d 6574 686f 6473 2061 7320  same methods as 
-000047f0: 4576 656e 7454 7265 6543 6f6c 6c65 6374  EventTreeCollect
-00004800: 696f 6e2c 2062 7574 206f 6e6c 7920 666f  ion, but only fo
-00004810: 7220 6974 7320 6f77 6e20 7472 6565 2e0a  r its own tree..
-00004820: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00004830: 2023 205b 332e 342e 315d 2047 6574 2063   # [3.4.1] Get c
-00004840: 6f6c 6c65 6374 696f 6e20 7472 6565 732e  ollection trees.
-00004850: 0a20 2020 2020 2020 2074 7265 6573 3a20  .        trees: 
-00004860: 4c69 7374 5b45 7665 6e74 5472 6565 5d20  List[EventTree] 
-00004870: 3d20 6574 632e 6765 745f 7472 6565 7328  = etc.get_trees(
-00004880: 290a 2020 2020 2020 2020 7472 6565 3a20  ).        tree: 
-00004890: 4576 656e 7454 7265 6520 3d20 7472 6565  EventTree = tree
-000048a0: 735b 305d 0a20 2020 2020 2020 200a 2020  s[0].        .  
-000048b0: 2020 2020 2020 2320 4275 7420 4576 656e        # But Even
-000048c0: 7454 7265 6520 7072 6f76 6964 6573 2061  tTree provides a
-000048d0: 2077 6f72 6b20 7769 7468 2074 6865 2074   work with the t
-000048e0: 7265 652c 2062 7574 2064 6f65 7320 6e6f  ree, but does no
-000048f0: 7420 6d6f 6469 6679 2069 742e 0a20 2020  t modify it..   
-00004900: 2020 2020 2023 2049 6620 796f 7520 7761       # If you wa
-00004910: 6e74 2074 6f20 6d6f 6469 6679 2074 6865  nt to modify the
-00004920: 2074 7265 652c 2075 7365 2045 7665 6e74   tree, use Event
-00004930: 5472 6565 436f 6c6c 6563 7469 6f6e 732e  TreeCollections.
-00004940: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00004950: 2020 2320 5b33 2e35 5d20 576f 726b 696e    # [3.5] Workin
-00004960: 6720 7769 7468 2050 6172 656e 746c 6573  g with Parentles
-00004970: 7354 7265 652e 0a20 2020 2020 2020 2023  sTree..        #
-00004980: 2050 6172 656e 746c 6573 7354 7265 6520   ParentlessTree 
-00004990: 6973 2045 7665 6e74 5472 6565 2077 6869  is EventTree whi
-000049a0: 6368 2068 6173 2064 6574 6163 6865 6420  ch has detached 
-000049b0: 6576 656e 7473 2077 6974 6820 7374 7562  events with stub
-000049c0: 732e 0a20 2020 2020 2020 2070 6172 656e  s..        paren
-000049d0: 746c 6573 735f 7472 6565 733a 204c 6973  tless_trees: Lis
-000049e0: 745b 4576 656e 7454 7265 655d 203d 2065  t[EventTree] = e
-000049f0: 7463 2e67 6574 5f70 6172 656e 746c 6573  tc.get_parentles
-00004a00: 735f 7472 6565 7328 290a 2020 2020 2020  s_trees().      
-00004a10: 2020 0a20 2020 2020 2020 2023 205b 332e    .        # [3.
-00004a20: 365d 2057 6f72 6b69 6e67 2077 6974 6820  6] Working with 
-00004a30: 5061 7265 6e74 4576 656e 7454 7265 6543  ParentEventTreeC
-00004a40: 6f6c 6c65 6374 696f 6e2e 0a20 2020 2020  ollection..     
-00004a50: 2020 2023 2050 6172 656e 7445 7665 6e74     # ParentEvent
-00004a60: 5472 6565 436f 6c6c 6563 7469 6f6e 2069  TreeCollection i
-00004a70: 7320 6120 7472 6565 2063 6f6c 6c65 6374  s a tree collect
-00004a80: 696f 6e20 6c69 6b65 2045 7665 6e74 5472  ion like EventTr
-00004a90: 6565 436f 6c6c 6563 7469 6f6e 2c0a 2020  eeCollection,.  
-00004aa0: 2020 2020 2020 2320 6275 7420 6974 2068        # but it h
-00004ab0: 6173 206f 6e6c 7920 6576 656e 7473 2074  as only events t
-00004ac0: 6861 7420 6861 7665 2072 6566 6572 656e  hat have referen
-00004ad0: 6365 732e 0a20 2020 2020 2020 2064 6174  ces..        dat
-00004ae0: 615f 736f 7572 6365 3a20 4944 6174 6153  a_source: IDataS
-00004af0: 6f75 7263 6520 2023 2059 6f75 2073 686f  ource  # You sho
-00004b00: 756c 6420 696e 6974 2044 6174 6153 6f75  uld init DataSou
-00004b10: 7263 6520 6f62 6a65 6374 2e20 452e 672e  rce object. E.g.
-00004b20: 2066 726f 6d20 4c77 4450 206d 6f64 756c   from LwDP modul
-00004b30: 652e 0a20 2020 2020 2020 2023 2045 5443  e..        # ETC
-00004b40: 4472 6976 6572 2068 6572 6520 6973 2061  Driver here is a
-00004b50: 2073 7475 622c 2061 6374 7561 6c6c 7920   stub, actually 
-00004b60: 7468 6520 6c69 6220 646f 6e27 7420 6861  the lib don't ha
-00004b70: 7665 2073 7563 6820 636c 6173 732e 0a20  ve such class.. 
-00004b80: 2020 2020 2020 2023 2059 6f75 2063 616e         # You can
-00004b90: 2074 616b 6520 6974 2069 6e20 4c77 4450   take it in LwDP
-00004ba0: 206d 6f64 756c 6520 6f72 2063 7265 6174   module or creat
-00004bb0: 6520 796f 7572 7365 6c66 2063 6c61 7373  e yourself class
-00004bc0: 2069 6620 796f 7520 6861 7665 2073 6f6d   if you have som
-00004bd0: 6520 7370 6563 6961 6c20 6576 656e 7473  e special events
-00004be0: 2073 7472 7563 7475 7265 2e0a 2020 2020   structure..    
-00004bf0: 2020 2020 6672 6f6d 2074 6832 5f64 6174      from th2_dat
-00004c00: 615f 7365 7276 6963 6573 2e64 6174 615f  a_services.data_
-00004c10: 736f 7572 6365 2e6c 7764 702e 6576 656e  source.lwdp.even
-00004c20: 745f 7472 6565 2069 6d70 6f72 7420 4874  t_tree import Ht
-00004c30: 7470 4554 4344 7269 7665 7220 6173 2045  tpETCDriver as E
-00004c40: 5443 4472 6976 6572 0a20 2020 2020 2020  TCDriver.       
-00004c50: 200a 2020 2020 2020 2020 6472 6976 6572   .        driver
-00004c60: 203d 2045 5443 4472 6976 6572 2864 6174   = ETCDriver(dat
-00004c70: 615f 736f 7572 6365 3d64 6174 615f 736f  a_source=data_so
-00004c80: 7572 6365 290a 2020 2020 2020 2020 6574  urce).        et
-00004c90: 6320 3d20 5061 7265 6e74 4576 656e 7454  c = ParentEventT
-00004ca0: 7265 6543 6f6c 6c65 6374 696f 6e28 6472  reeCollection(dr
-00004cb0: 6976 6572 290a 2020 2020 2020 2020 6574  iver).        et
-00004cc0: 632e 6275 696c 6428 6576 656e 7473 290a  c.build(events).
-00004cd0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00004ce0: 2065 7463 2e73 686f 7728 290a 2020 2020   etc.show().    
-00004cf0: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-00004d00: 345d 2046 6965 6c64 2052 6573 6f6c 7665  4] Field Resolve
-00004d10: 7273 0a20 2020 2020 2020 2023 2050 6c65  rs.        # Ple
-00004d20: 6173 6520 7265 6164 2060 4669 656c 6420  ase read `Field 
-00004d30: 5265 736f 6c76 6572 7360 2062 6c6f 636b  Resolvers` block
-00004d40: 2069 6e20 7265 6164 6d65 2066 6972 7374   in readme first
-00004d50: 2e0a 2020 2020 2020 2020 2320 5b34 2e31  ..        # [4.1
-00004d60: 5d20 5573 6167 6520 6578 616d 706c 6520  ] Usage example 
-00004d70: 6672 6f6d 2063 6c69 656e 7420 636f 6465  from client code
-00004d80: 0a20 2020 2020 2020 2066 726f 6d20 7468  .        from th
-00004d90: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
-00004da0: 6461 7461 5f73 6f75 7263 6520 696d 706f  data_source impo
-00004db0: 7274 2028 0a20 2020 2020 2020 2020 2020  rt (.           
-00004dc0: 206c 7764 702c 0a20 2020 2020 2020 2029   lwdp,.        )
-00004dd0: 2020 2320 6c77 6470 2064 6174 615f 736f    # lwdp data_so
-00004de0: 7572 6365 2069 6e69 7469 616c 697a 6520  urce initialize 
-00004df0: 7468 325f 6461 7461 5f73 6572 7669 6365  th2_data_service
-00004e00: 732e 636f 6e66 6967 2064 7572 696e 6720  s.config during 
-00004e10: 696d 706f 7274 2e0a 2020 2020 2020 2020  import..        
-00004e20: 6672 6f6d 2074 6832 5f64 6174 615f 7365  from th2_data_se
-00004e30: 7276 6963 6573 2e63 6f6e 6669 6720 696d  rvices.config im
-00004e40: 706f 7274 206f 7074 696f 6e73 2061 7320  port options as 
-00004e50: 6f5f 0a20 2020 2020 2020 200a 2020 2020  o_.        .    
-00004e60: 2020 2020 666f 7220 6d20 696e 2064 6174      for m in dat
-00004e70: 613a 0a20 2020 2020 2020 2020 2020 206f  a:.            o
-00004e80: 5f2e 6d66 722e 6578 7061 6e64 5f6d 6573  _.mfr.expand_mes
-00004e90: 7361 6765 286d 2920 2023 206d 6672 202d  sage(m)  # mfr -
-00004ea0: 2073 7461 6e64 7320 666f 7220 4d65 7373   stands for Mess
-00004eb0: 6167 6546 6965 6c64 5265 736f 6c76 6572  ageFieldResolver
-00004ec0: 0a20 2020 2020 2020 2020 2020 2023 206f  .            # o
-00004ed0: 720a 2020 2020 2020 2020 2020 2020 6f5f  r.            o_
-00004ee0: 2e65 6d66 722e 6578 7061 6e64 5f6d 6573  .emfr.expand_mes
-00004ef0: 7361 6765 286d 2920 2023 2065 6d66 7220  sage(m)  # emfr 
-00004f00: 2d20 7374 616e 6473 2066 6f72 2045 7870  - stands for Exp
-00004f10: 616e 6465 644d 6573 7361 6765 4669 656c  andedMessageFiel
-00004f20: 6452 6573 6f6c 7665 720a 2020 2020 2020  dResolver.      
-00004f30: 2020 0a20 2020 2020 2020 2023 205b 342e    .        # [4.
-00004f40: 325d 204c 6962 7261 7269 6573 2075 7361  2] Libraries usa
-00004f50: 6765 2e0a 2020 2020 2020 2020 2320 446f  ge..        # Do
-00004f60: 6e27 7420 696d 706f 7274 2065 7861 6374  n't import exact
-00004f70: 2072 6573 6f6c 7665 7273 2069 6d70 6c65   resolvers imple
-00004f80: 6d65 6e74 6174 696f 6e20 706c 6561 7365  mentation please
-00004f90: 2069 6e20 796f 7572 2063 6f64 652e 0a20   in your code.. 
-00004fa0: 2020 2020 2020 2023 2041 6c6c 6f77 2079         # Allow y
-00004fb0: 6f75 7220 636c 6965 6e74 2074 6f20 646f  our client to do
-00004fc0: 2069 7420 696e 7374 6561 642e 0a20 2020   it instead..   
-00004fd0: 2020 2020 2023 204a 7573 7420 696d 706f       # Just impo
-00004fe0: 7274 2060 6f70 7469 6f6e 7360 2066 726f  rt `options` fro
-00004ff0: 6d20 6074 6832 5f64 6174 615f 7365 7276  m `th2_data_serv
-00005000: 6963 6573 2e63 6f6e 6669 6760 2061 6e64  ices.config` and
-00005010: 2075 7365 2069 742e 0a20 2020 2020 2020   use it..       
-00005020: 2066 726f 6d20 7468 325f 6461 7461 5f73   from th2_data_s
-00005030: 6572 7669 6365 732e 636f 6e66 6967 2069  ervices.config i
-00005040: 6d70 6f72 7420 6f70 7469 6f6e 7320 6173  mport options as
-00005050: 206f 5f0a 2020 2020 2020 2020 0a20 2020   o_.        .   
-00005060: 2020 2020 2066 6f72 206d 2069 6e20 6461       for m in da
-00005070: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
-00005080: 6f5f 2e6d 6672 2e65 7870 616e 645f 6d65  o_.mfr.expand_me
-00005090: 7373 6167 6528 6d29 0a20 2020 2020 2020  ssage(m).       
-000050a0: 2020 2020 2023 206f 720a 2020 2020 2020       # or.      
-000050b0: 2020 2020 2020 6f5f 2e65 6d66 722e 6578        o_.emfr.ex
-000050c0: 7061 6e64 5f6d 6573 7361 6765 286d 290a  pand_message(m).
-000050d0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000050e0: 2023 204d 6f72 6520 7465 6368 2064 6574   # More tech det
-000050f0: 6169 6c73 3a0a 2020 2020 2020 2020 2320  ails:.        # 
-00005100: 2020 496e 2074 6869 7320 6361 7365 2c20    In this case, 
-00005110: 7468 6572 6520 6973 206e 6f20 6c69 6e65  there is no line
-00005120: 2060 6672 6f6d 2074 6832 5f64 6174 615f   `from th2_data_
-00005130: 7365 7276 6963 6573 2e64 6174 615f 736f  services.data_so
-00005140: 7572 6365 2069 6d70 6f72 7420 6c77 6470  urce import lwdp
-00005150: 2060 0a20 2020 2020 2020 2023 2020 2062   `.        #   b
-00005160: 6563 6175 7365 2077 6520 7368 6f75 6c64  ecause we should
-00005170: 206e 6f74 2063 686f 6f73 6520 666f 7220   not choose for 
-00005180: 7468 6520 7573 6572 2077 6869 6368 2064  the user which d
-00005190: 6174 6120 736f 7572 6365 2074 6f20 7573  ata source to us
-000051a0: 652e 0a20 2020 2020 2020 2023 2020 2057  e..        #   W
-000051b0: 6520 646f 206e 6f74 206b 6e6f 7720 7768  e do not know wh
-000051c0: 6174 2068 6520 7769 6c6c 2063 686f 6f73  at he will choos
-000051d0: 652c 2074 6865 7265 666f 7265 2077 6520  e, therefore we 
-000051e0: 6d75 7374 2073 696d 706c 7920 6163 6365  must simply acce
-000051f0: 7373 0a20 2020 2020 2020 2023 2020 2074  ss.        #   t
-00005200: 6865 2069 6e74 6572 6661 6365 2c20 7768  he interface, wh
-00005210: 6963 6820 7769 6c6c 2062 6520 696e 6974  ich will be init
-00005220: 6961 6c69 7a65 6420 6279 2074 6865 2075  ialized by the u
-00005230: 7365 722e 0a20 2020 2020 2020 200a 2020  ser..        .  
-00005240: 2020 2020 2020 2320 5b35 5d20 5573 696e        # [5] Usin
-00005250: 6720 7574 696c 6974 7920 6675 6e63 7469  g utility functi
-00005260: 6f6e 732e 0a20 2020 2020 2020 2066 726f  ons..        fro
-00005270: 6d20 7468 325f 6461 7461 5f73 6572 7669  m th2_data_servi
-00005280: 6365 732e 7574 696c 732e 6576 656e 745f  ces.utils.event_
-00005290: 7574 696c 732e 6672 6571 7565 6e63 6965  utils.frequencie
-000052a0: 7320 696d 706f 7274 2067 6574 5f63 6174  s import get_cat
-000052b0: 6567 6f72 795f 6672 6571 7565 6e63 6965  egory_frequencie
-000052c0: 7332 0a20 2020 2020 2020 2066 726f 6d20  s2.        from 
-000052d0: 7468 325f 6461 7461 5f73 6572 7669 6365  th2_data_service
-000052e0: 732e 7574 696c 732e 6576 656e 745f 7574  s.utils.event_ut
-000052f0: 696c 732e 746f 7461 6c73 2069 6d70 6f72  ils.totals impor
-00005300: 7420 6765 745f 6361 7465 676f 7279 5f74  t get_category_t
-00005310: 6f74 616c 7332 0a20 2020 2020 2020 2066  otals2.        f
-00005320: 726f 6d20 7468 325f 6461 7461 5f73 6572  rom th2_data_ser
-00005330: 7669 6365 732e 7574 696c 732e 6361 7465  vices.utils.cate
-00005340: 676f 7279 2069 6d70 6f72 7420 4361 7465  gory import Cate
-00005350: 676f 7279 0a20 2020 2020 2020 2066 726f  gory.        fro
-00005360: 6d20 7468 325f 6461 7461 5f73 6572 7669  m th2_data_servi
-00005370: 6365 732e 7574 696c 732e 6576 656e 745f  ces.utils.event_
-00005380: 7574 696c 732e 6576 656e 745f 7574 696c  utils.event_util
-00005390: 7320 696d 706f 7274 2069 735f 736f 7274  s import is_sort
-000053a0: 6564 0a20 2020 2020 2020 200a 2020 2020  ed.        .    
-000053b0: 2020 2020 2320 5b35 2e31 5d20 4765 7420      # [5.1] Get 
-000053c0: 7468 6520 7175 616e 7469 7469 6573 206f  the quantities o
-000053d0: 6620 6576 656e 7473 2066 6f72 2064 6966  f events for dif
-000053e0: 6665 7265 6e74 2063 6174 6567 6f72 6965  ferent categorie
-000053f0: 732e 0a20 2020 2020 2020 206d 6574 7269  s..        metri
-00005400: 6373 203d 205b 0a20 2020 2020 2020 2020  cs = [.         
-00005410: 2020 2043 6174 6567 6f72 7928 2264 6174     Category("dat
-00005420: 6522 2c20 6c61 6d62 6461 206d 3a20 5468  e", lambda m: Th
-00005430: 3254 696d 6573 7461 6d70 436f 6e76 6572  2TimestampConver
-00005440: 7465 722e 746f 5f64 6174 6574 696d 6528  ter.to_datetime(
-00005450: 6d5b 2273 7461 7274 5469 6d65 7374 616d  m["startTimestam
-00005460: 7022 5d29 2e64 6174 6528 2929 2c0a 2020  p"]).date()),.  
-00005470: 2020 2020 2020 2020 2020 4361 7465 676f            Catego
-00005480: 7279 2822 7374 6174 7573 222c 206c 616d  ry("status", lam
-00005490: 6264 6120 6d3a 206d 5b22 7375 6363 6573  bda m: m["succes
-000054a0: 7366 756c 225d 292c 0a20 2020 2020 2020  sful"]),.       
-000054b0: 205d 0a20 2020 2020 2020 2063 6174 6567   ].        categ
-000054c0: 6f72 795f 746f 7461 6c73 203d 2067 6574  ory_totals = get
-000054d0: 5f63 6174 6567 6f72 795f 746f 7461 6c73  _category_totals
-000054e0: 3228 6576 656e 7473 2c20 6d65 7472 6963  2(events, metric
-000054f0: 7329 0a20 2020 2020 2020 2022 2222 0a20  s).        """. 
-00005500: 2020 2020 2020 202b 2d2d 2d2d 2d2d 2d2d         +--------
-00005510: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  +------------+--
-00005520: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00005530: 2d2d 2b0a 2020 2020 2020 2020 7c20 2020  --+.        |   
-00005540: 2020 2020 207c 2064 6174 6520 2020 2020       | date     
-00005550: 2020 7c20 7374 6174 7573 2020 207c 2020    | status   |  
-00005560: 2063 6f75 6e74 207c 0a20 2020 2020 2020   count |.       
-00005570: 202b 3d3d 3d3d 3d3d 3d3d 2b3d 3d3d 3d3d   +========+=====
-00005580: 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d  =======+========
-00005590: 3d3d 2b3d 3d3d 3d3d 3d3d 3d3d 2b0a 2020  ==+=========+.  
-000055a0: 2020 2020 2020 7c20 2020 2020 2020 207c        |        |
-000055b0: 2032 3032 332d 3031 2d30 3520 7c20 5472   2023-01-05 | Tr
-000055c0: 7565 2020 2020 207c 2020 2020 2020 2033  ue     |       3
-000055d0: 207c 0a20 2020 2020 2020 202b 2d2d 2d2d   |.        +----
-000055e0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-000055f0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  -+----------+---
-00005600: 2d2d 2d2d 2d2d 2b0a 2020 2020 2020 2020  ------+.        
-00005610: 7c20 636f 756e 7420 207c 2020 2020 2020  | count  |      
-00005620: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00005630: 207c 2020 2020 2020 2031 207c 0a20 2020   |       1 |.   
-00005640: 2020 2020 202b 2d2d 2d2d 2d2d 2d2d 2b2d       +--------+-
-00005650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
-00005660: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
-00005670: 2b0a 2020 2020 2020 2020 7c20 746f 7461  +.        | tota
-00005680: 6c73 207c 2020 2020 2020 2020 2020 2020  ls |            
-00005690: 7c20 312f 3020 2020 2020 207c 2020 2020  | 1/0      |    
-000056a0: 2020 2033 207c 0a20 2020 2020 2020 202b     3 |.        +
-000056b0: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-000056c0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
-000056d0: 2b2d 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020  +---------+.    
-000056e0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000056f0: 0a20 2020 2020 2020 2023 205b 352e 325d  .        # [5.2]
-00005700: 2047 6574 2074 6865 206e 756d 6265 7220   Get the number 
-00005710: 6f66 2065 7665 6e74 7320 7769 7468 2073  of events with s
-00005720: 7461 7475 7320 7375 6363 6573 7366 756c  tatus successful
-00005730: 2e0a 2020 2020 2020 2020 6361 7465 676f  ..        catego
-00005740: 7279 203d 2043 6174 6567 6f72 7928 2273  ry = Category("s
-00005750: 7461 7475 7322 2c20 6c61 6d62 6461 206d  tatus", lambda m
-00005760: 3a20 6d5b 2273 7563 6365 7373 6675 6c22  : m["successful"
-00005770: 5d29 0a20 2020 2020 2020 2063 6174 6567  ]).        categ
-00005780: 6f72 795f 6672 6571 7565 6e63 6965 7320  ory_frequencies 
-00005790: 3d20 6765 745f 6361 7465 676f 7279 5f66  = get_category_f
-000057a0: 7265 7175 656e 6369 6573 3228 6576 656e  requencies2(even
-000057b0: 7473 2c20 6361 7465 676f 7279 290a 2020  ts, category).  
-000057c0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000057d0: 2020 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d    +--------+----
-000057e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000057f0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-00005800: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-00005810: 2b0a 2020 2020 2020 2020 7c20 2020 2020  +.        |     
-00005820: 2020 207c 2074 696d 6573 7461 6d70 5f73     | timestamp_s
-00005830: 7461 7274 2020 2020 207c 2074 696d 6573  tart     | times
-00005840: 7461 6d70 5f65 6e64 2020 2020 2020 207c  tamp_end       |
-00005850: 2020 2054 7275 6520 7c0a 2020 2020 2020     True |.      
-00005860: 2020 2b3d 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d    +========+====
-00005870: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00005880: 3d2b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  =+==============
-00005890: 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d  =======+========
-000058a0: 2b0a 2020 2020 2020 2020 7c20 2020 2020  +.        |     
-000058b0: 2020 207c 2032 3032 332d 3031 2d30 3554     | 2023-01-05T
-000058c0: 3133 3a35 373a 3035 207c 2032 3032 332d  13:57:05 | 2023-
-000058d0: 3031 2d30 3554 3133 3a35 373a 3036 207c  01-05T13:57:06 |
-000058e0: 2020 2020 2020 3320 7c0a 2020 2020 2020        3 |.      
-000058f0: 2020 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d    +--------+----
-00005900: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005910: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-00005920: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-00005930: 2b0a 2020 2020 2020 2020 7c20 636f 756e  +.        | coun
-00005940: 7420 207c 2020 2020 2020 2020 2020 2020  t  |            
-00005950: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00005960: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00005970: 2020 2020 2020 3120 7c0a 2020 2020 2020        1 |.      
-00005980: 2020 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d    +--------+----
-00005990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000059a0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-000059b0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-000059c0: 2b0a 2020 2020 2020 2020 7c20 746f 7461  +.        | tota
-000059d0: 6c73 207c 2020 2020 2020 2020 2020 2020  ls |            
-000059e0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-000059f0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00005a00: 2020 2020 2020 3320 7c0a 2020 2020 2020        3 |.      
-00005a10: 2020 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d    +--------+----
-00005a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005a30: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-00005a40: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-00005a50: 2b0a 2020 2020 2020 2020 2222 220a 2020  +.        """.  
-00005a60: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-00005a70: 205b 352e 335d 2043 6865 636b 2069 6620   [5.3] Check if 
-00005a80: 6576 656e 7473 2061 7265 2073 6f72 7465  events are sorte
-00005a90: 642e 0a20 2020 2020 2020 2072 6573 756c  d..        resul
-00005aa0: 7420 3d20 6973 5f73 6f72 7465 6428 6576  t = is_sorted(ev
-00005ab0: 656e 7473 290a 2020 2020 2020 2020 6060  ents).        ``
-00005ac0: 600a 2020 2020 2020 2020 3c21 2d2d 2065  `.        <!-- e
-00005ad0: 6e64 2067 6574 5f73 7461 7274 6564 5f65  nd get_started_e
-00005ae0: 7861 6d70 6c65 2e70 7920 2d2d 3e0a 2020  xample.py -->.  
-00005af0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-00005b00: 2320 322e 332e 2053 686f 7274 2074 6865  # 2.3. Short the
-00005b10: 6f72 790a 2020 2020 2020 2020 0a20 2020  ory.        .   
-00005b20: 2020 2020 2054 6865 206c 6962 7261 7279       The library
-00005b30: 2070 726f 7669 6465 7320 746f 6f6c 7320   provides tools 
-00005b40: 666f 7220 6861 6e64 6c69 6e67 2073 7472  for handling str
-00005b50: 6561 6d20 6461 7461 2e20 5768 6174 2773  eam data. What's
-00005b60: 2061 2073 7472 6561 6d3f 2049 7427 7320   a stream? It's 
-00005b70: 6120 7365 7175 656e 6365 206f 6620 656c  a sequence of el
-00005b80: 656d 656e 7473 2066 726f 6d20 6120 736f  ements from a so
-00005b90: 7572 6365 2074 6861 740a 2020 2020 2020  urce that.      
-00005ba0: 2020 7375 7070 6f72 7473 2061 6767 7265    supports aggre
-00005bb0: 6761 7465 206f 7065 7261 7469 6f6e 732e  gate operations.
-00005bc0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00005bd0: 2020 2323 2320 5465 726d 730a 2020 2020    ### Terms.    
-00005be0: 2020 2020 0a20 2020 2020 2020 202d 202a      .        - *
-00005bf0: 2a44 6174 6120 6f62 6a65 6374 2a2a 3a20  *Data object**: 
-00005c00: 416e 2069 6e73 7461 6e63 6520 6f66 2060  An instance of `
-00005c10: 4461 7461 6020 636c 6173 7320 7768 6963  Data` class whic
-00005c20: 6820 6973 2077 7261 7070 6572 2075 6e64  h is wrapper und
-00005c30: 6572 2073 7472 6561 6d2e 0a20 2020 2020  er stream..     
-00005c40: 2020 202d 202a 2a53 6571 7565 6e63 6520     - **Sequence 
-00005c50: 6f66 2065 6c65 6d65 6e74 732a 2a3a 0a20  of elements**:. 
-00005c60: 2020 2020 2020 2020 2041 205f 4461 7461           A _Data
-00005c70: 206f 626a 6563 745f 2070 726f 7669 6465   object_ provide
-00005c80: 7320 616e 2069 6e74 6572 6661 6365 2074  s an interface t
-00005c90: 6f20 6120 7365 7175 656e 6365 6420 7365  o a sequenced se
-00005ca0: 7420 6f66 2076 616c 7565 7320 6f66 2061  t of values of a
-00005cb0: 2073 7065 6369 6669 6320 656c 656d 656e   specific elemen
-00005cc0: 7420 7479 7065 2e20 5374 7265 616d 2069  t type. Stream i
-00005cd0: 6e73 6964 6520 7468 6520 5f44 6174 610a  nside the _Data.
-00005ce0: 2020 2020 2020 2020 2020 6f62 6a65 6374            object
-00005cf0: 5f20 2a2a 646f 6e19 7420 6163 7475 616c  _ **don.t actual
-00005d00: 6c79 2073 746f 7265 2a2a 2065 6c65 6d65  ly store** eleme
-00005d10: 6e74 733b 2074 6865 7920 6172 6520 636f  nts; they are co
-00005d20: 6d70 7574 6564 206f 6e20 6465 6d61 6e64  mputed on demand
-00005d30: 2e0a 2020 2020 2020 2020 2d20 2a2a 6461  ..        - **da
-00005d40: 7461 2073 6f75 7263 652a 2a20 2865 7861  ta source** (exa
-00005d50: 6374 6c79 2069 6e20 736d 616c 6c20 6c65  ctly in small le
-00005d60: 7474 6572 7329 3a0a 2020 2020 2020 2020  tters):.        
-00005d70: 2020 416e 7920 736f 7572 6365 206f 6620    Any source of 
-00005d80: 6461 7461 2e20 452e 672e 205b 4c69 6768  data. E.g. [Ligh
-00005d90: 7477 6569 6768 7420 4461 7461 2050 726f  tweight Data Pro
-00005da0: 7669 6465 725d 2868 7474 7073 3a2f 2f67  vider](https://g
-00005db0: 6974 6875 622e 636f 6d2f 7468 322d 6e65  ithub.com/th2-ne
-00005dc0: 742f 7468 322d 6c77 2d64 6174 612d 7072  t/th2-lw-data-pr
-00005dd0: 6f76 6964 6572 292c 2063 6f6c 6c65 6374  ovider), collect
-00005de0: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
-00005df0: 6172 7261 7973 2c20 6f72 2049 2f4f 2072  arrays, or I/O r
-00005e00: 6573 6f75 7263 6573 2e0a 2020 2020 2020  esources..      
-00005e10: 2020 2d20 2a2a 4461 7461 536f 7572 6365    - **DataSource
-00005e20: 2a2a 3a0a 2020 2020 2020 2020 2020 4120  **:.          A 
-00005e30: 636c 6173 7320 7468 6174 2069 7320 616e  class that is an
-00005e40: 2069 6e74 6572 6d65 6469 6174 6520 6c69   intermediate li
-00005e50: 6e6b 2062 6574 7765 656e 2074 6865 2053  nk between the S
-00005e60: 6f75 7263 6541 5049 2061 6e64 2043 6f6d  ourceAPI and Com
-00005e70: 6d61 6e64 732e 0a20 2020 2020 2020 202d  mands..        -
-00005e80: 202a 2a53 6f75 7263 6541 5049 2a2a 3a0a   **SourceAPI**:.
-00005e90: 2020 2020 2020 2020 2020 4561 6368 2073            Each s
-00005ea0: 6f75 7263 6520 6861 7320 6974 7320 6f77  ource has its ow
-00005eb0: 6e20 4150 4920 746f 2072 6574 7269 6576  n API to retriev
-00005ec0: 6520 6461 7461 2e20 536f 7572 6365 4150  e data. SourceAP
-00005ed0: 4920 6973 2061 2063 6c61 7373 2074 6861  I is a class tha
-00005ee0: 7420 7072 6f76 6964 6520 4150 4920 666f  t provide API fo
-00005ef0: 7220 736f 6d65 2064 6174 6120 736f 7572  r some data sour
-00005f00: 6365 2e0a 2020 2020 2020 2020 2d20 2a2a  ce..        - **
-00005f10: 436f 6d6d 616e 6473 2a2a 3a0a 2020 2020  Commands**:.    
-00005f20: 2020 2020 2020 436c 6173 7365 7320 7468        Classes th
-00005f30: 6174 2070 726f 7669 6465 2075 7365 722d  at provide user-
-00005f40: 6672 6965 6e64 6c79 2069 6e74 6572 6661  friendly interfa
-00005f50: 6365 7320 666f 7220 6765 7474 696e 6720  ces for getting 
-00005f60: 736f 6d65 2064 6174 6120 6672 6f6d 2044  some data from D
-00005f70: 6174 6153 6f75 7263 652e 2043 6f6d 6d61  ataSource. Comma
-00005f80: 6e64 7320 7573 6520 5f53 6f75 7263 6541  nds use _SourceA
-00005f90: 5049 5f20 746f 0a20 2020 2020 2020 2020  PI_ to.         
-00005fa0: 2061 6368 6965 7665 2069 742e 0a20 2020   achieve it..   
-00005fb0: 2020 2020 202d 202a 2a41 6461 7074 6572       - **Adapter
-00005fc0: 732a 2a3a 0a20 2020 2020 2020 2020 2049  s**:.          I
-00005fd0: 7427 7320 7369 6d69 6c61 7220 746f 2066  t's similar to f
-00005fe0: 756e 6374 696f 6e20 666f 7220 6044 6174  unction for `Dat
-00005ff0: 612e 6d61 7060 206d 6574 686f 642e 2041  a.map` method. A
-00006000: 646f 7074 6162 6c65 2063 6f6d 6d61 6e64  doptable command
-00006010: 7320 7573 6564 2069 7420 746f 2075 7064  s used it to upd
-00006020: 6174 6520 7468 6520 6461 7461 2073 7472  ate the data str
-00006030: 6561 6d2e 0a20 2020 2020 2020 202d 202a  eam..        - *
-00006040: 2a41 6767 7265 6761 7465 206f 7065 7261  *Aggregate opera
-00006050: 7469 6f6e 732a 2a3a 0a20 2020 2020 2020  tions**:.       
-00006060: 2020 2043 6f6d 6d6f 6e20 6f70 6572 6174     Common operat
-00006070: 696f 6e73 2073 7563 6820 6173 2066 696c  ions such as fil
-00006080: 7465 722c 206d 6170 2c20 6c69 6d69 7420  ter, map, limit 
-00006090: 616e 6420 736f 206f 6e2e 0a20 2020 2020  and so on..     
-000060a0: 2020 202d 202a 2a57 6f72 6b66 6c6f 772a     - **Workflow*
-000060b0: 2a3a 2041 6e20 6f72 6465 7265 6420 7365  *: An ordered se
-000060c0: 7420 6f66 205f 4167 6772 6567 6174 6520  t of _Aggregate 
-000060d0: 6f70 6572 6174 696f 6e73 5f2e 0a20 2020  operations_..   
-000060e0: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-000060f0: 2320 436f 6e63 6570 740a 2020 2020 2020  # Concept.      
-00006100: 2020 0a20 2020 2020 2020 2054 6865 206c    .        The l
-00006110: 6962 7261 7279 2064 6573 6372 6962 6573  ibrary describes
-00006120: 2074 6865 2068 6967 682d 6c65 7665 6c20   the high-level 
-00006130: 696e 7465 7266 6163 6573 2060 4953 6f75  interfaces `ISou
-00006140: 7263 6541 5049 602c 2060 4944 6174 6153  rceAPI`, `IDataS
-00006150: 6f75 7263 6560 2c20 6049 436f 6d6d 616e  ource`, `IComman
-00006160: 6460 2c20 6049 4164 6170 7465 7260 2e0a  d`, `IAdapter`..
-00006170: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00006180: 2041 6e79 2064 6174 6120 736f 7572 6365   Any data source
-00006190: 206d 7573 7420 6265 2064 6573 6372 6962   must be describ
-000061a0: 6564 2062 7920 7468 6520 6049 4461 7461  ed by the `IData
-000061b0: 536f 7572 6365 6020 6162 7374 7261 6374  Source` abstract
-000061c0: 2063 6c61 7373 2e20 5468 6573 6520 6361   class. These ca
-000061d0: 6e20 6265 205f 4669 6c65 4461 7461 536f  n be _FileDataSo
-000061e0: 7572 6365 5f2c 0a20 2020 2020 2020 205f  urce_,.        _
-000061f0: 4353 5644 6174 6153 6f75 7263 655f 2c20  CSVDataSource_, 
-00006200: 5f44 4244 6174 6153 6f75 7263 655f 2061  _DBDataSource_ a
-00006210: 6e64 206f 7468 6572 2e0a 2020 2020 2020  nd other..      
-00006220: 2020 0a20 2020 2020 2020 2055 7375 616c    .        Usual
-00006230: 6c79 2c20 6461 7461 2073 6f75 7263 6573  ly, data sources
-00006240: 2068 6176 6520 736f 6d65 206b 696e 6420   have some kind 
-00006250: 6f66 2041 5049 2e20 4461 7461 6261 7365  of API. Database
-00006260: 7320 2d20 7072 6f76 6964 6520 5351 4c20  s - provide SQL 
-00006270: 6c61 6e67 7561 6765 2c20 7768 656e 2077  language, when w
-00006280: 6f72 6b69 6e67 2077 6974 6820 6120 6669  orking with a fi
-00006290: 6c65 2c20 796f 7520 6361 6e20 7265 6164  le, you can read
-000062a0: 0a20 2020 2020 2020 206c 696e 6520 6279  .        line by
-000062b0: 206c 696e 652c 2065 7463 2e20 5468 6973   line, etc. This
-000062c0: 2041 5049 2069 7320 6465 7363 7269 6265   API is describe
-000062d0: 6420 6279 2074 6865 2060 4953 6f75 7263  d by the `ISourc
-000062e0: 6541 5049 6020 636c 6173 732e 2042 6563  eAPI` class. Bec
-000062f0: 6175 7365 2064 6966 6665 7265 6e74 2076  ause different v
-00006300: 6572 7369 6f6e 7320 6f66 2074 6865 2073  ersions of the s
-00006310: 616d 6520 6461 7461 2073 6f75 7263 650a  ame data source.
-00006320: 2020 2020 2020 2020 6d61 7920 6861 7665          may have
-00006330: 2064 6966 6665 7265 6e74 2041 5049 2c20   different API, 
-00006340: 6974 2069 7320 6265 7474 6572 2074 6f20  it is better to 
-00006350: 6372 6561 7465 2061 2063 6c61 7373 2066  create a class f
-00006360: 6f72 2065 6163 6820 7665 7273 696f 6e2e  or each version.
-00006370: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00006380: 2020 4765 6e65 7261 6c6c 792c 2064 6174    Generally, dat
-00006390: 6120 736f 7572 6365 2041 5049 7320 6172  a source APIs ar
-000063a0: 6520 6869 6464 656e 2062 6568 696e 6420  e hidden behind 
-000063b0: 636f 6e76 656e 6965 6e74 2069 6e74 6572  convenient inter
-000063c0: 6661 6365 732e 2054 6865 2072 6f6c 6520  faces. The role 
-000063d0: 6f66 2074 6865 7365 2069 6e74 6572 6661  of these interfa
-000063e0: 6365 7320 6973 2070 6c61 7965 640a 2020  ces is played.  
-000063f0: 2020 2020 2020 6279 2060 4943 6f6d 6d61        by `IComma
-00006400: 6e64 6020 636c 6173 7365 732e 0a20 2020  nd` classes..   
-00006410: 2020 2020 200a 2020 2020 2020 2020 6049       .        `I
-00006420: 4164 6170 7465 7260 2063 6c61 7373 6573  Adapter` classes
-00006430: 2074 7261 6e73 666f 726d 2064 6174 6120   transform data 
-00006440: 7374 7265 616d 206c 696b 6520 6675 6e63  stream like func
-00006450: 7469 6f6e 7320 666f 7220 6044 6174 612e  tions for `Data.
-00006460: 6d61 7060 206d 6574 686f 642e 2045 7373  map` method. Ess
-00006470: 656e 7469 616c 6c79 2069 7427 7320 7468  entially it's th
-00006480: 6520 7361 6d65 2074 6869 6e67 2062 7574  e same thing but
-00006490: 206d 6f72 650a 2020 2020 2020 2020 666c   more.        fl
-000064a0: 6578 6962 6c65 2e0a 2020 2020 2020 2020  exible..        
-000064b0: 0a20 2020 2020 2020 2046 6f72 2065 7861  .        For exa
-000064c0: 6d70 6c65 2c20 4c77 4450 2044 6174 6153  mple, LwDP DataS
-000064d0: 6f75 7263 6528 6874 7470 733a 2f2f 6769  ource(https://gi
-000064e0: 7468 7562 2e63 6f6d 2f74 6832 2d6e 6574  thub.com/th2-net
-000064f0: 2f74 6832 2d64 732d 736f 7572 6365 2d6c  /th2-ds-source-l
-00006500: 7764 7029 2075 7365 7320 7468 6573 6520  wdp) uses these 
-00006510: 6162 7374 7261 6374 2063 6c61 7373 6573  abstract classes
-00006520: 2074 6f20 6275 696c 6420 6974 7320 696d   to build its im
-00006530: 706c 656d 656e 7461 7469 6f6e 2e59 6f75  plementation.You
-00006540: 2063 616e 2065 6173 696c 7920 6372 6561   can easily crea
-00006550: 7465 2079 6f75 7220 6f77 6e20 756e 6971  te your own uniq
-00006560: 7565 2063 6f6d 6d61 6e64 7320 666f 7220  ue commands for 
-00006570: 5f4c 7744 5020 4461 7461 536f 7572 6365  _LwDP DataSource
-00006580: 5f2c 2061 7320 7765 6c6c 2061 7320 656e  _, as well as en
-00006590: 7469 7265 0a20 2020 2020 2020 205f 4461  tire.        _Da
-000065a0: 7461 536f 7572 6365 5f20 636c 6173 7365  taSource_ classe
-000065b0: 732e 205b 4865 7265 2069 7320 6120 646f  s. [Here is a do
-000065c0: 6375 6d65 6e74 6174 696f 6e5d 2864 6f63  cumentation](doc
-000065d0: 756d 656e 7461 7469 6f6e 2f64 6174 6173  umentation/datas
-000065e0: 6f75 7263 652e 6d64 2920 6f6e 2068 6f77  ource.md) on how
-000065f0: 2074 6f20 696d 706c 656d 656e 7420 7468   to implement th
-00006600: 6573 6520 696e 7465 7266 6163 6573 2e0a  ese interfaces..
-00006610: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00006620: 2021 5b44 6174 6120 7374 7265 616d 2070   ![Data stream p
-00006630: 6970 656c 696e 655d 2864 6f63 756d 656e  ipeline](documen
-00006640: 7461 7469 6f6e 2f69 6d67 2f63 6f6e 6365  tation/img/conce
-00006650: 7074 2e70 6e67 290a 2020 2020 2020 2020  pt.png).        
-00006660: 0a20 2020 2020 2020 2023 2323 2053 7472  .        ### Str
-00006670: 6561 6d20 6f70 6572 6174 696f 6e73 0a20  eam operations. 
-00006680: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006690: 4675 7274 6865 726d 6f72 652c 2073 7472  Furthermore, str
-000066a0: 6561 6d20 6f70 6572 6174 696f 6e73 2068  eam operations h
-000066b0: 6176 6520 7477 6f20 6675 6e64 616d 656e  ave two fundamen
-000066c0: 7461 6c20 6368 6172 6163 7465 7269 7374  tal characterist
-000066d0: 6963 7320 7468 6174 206d 616b 6520 7468  ics that make th
-000066e0: 656d 2076 6572 7920 6469 6666 6572 656e  em very differen
-000066f0: 7420 6672 6f6d 2063 6f6c 6c65 6374 696f  t from collectio
-00006700: 6e0a 2020 2020 2020 2020 6f70 6572 6174  n.        operat
-00006710: 696f 6e73 3a20 5f50 6970 656c 696e 696e  ions: _Pipelinin
-00006720: 675f 2061 6e64 205f 496e 7465 726e 616c  g_ and _Internal
-00006730: 2069 7465 7261 7469 6f6e 5f2e 0a20 2020   iteration_..   
-00006740: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-00006750: 2323 2050 6970 656c 696e 696e 670a 2020  ## Pipelining.  
-00006760: 2020 2020 2020 0a20 2020 2020 2020 204d        .        M
-00006770: 616e 7920 7374 7265 616d 206f 7065 7261  any stream opera
-00006780: 7469 6f6e 7320 7265 7475 726e 2061 2073  tions return a s
-00006790: 7472 6561 6d20 7468 656d 7365 6c76 6573  tream themselves
-000067a0: 2e20 5468 6973 2061 6c6c 6f77 7320 6f70  . This allows op
-000067b0: 6572 6174 696f 6e73 2074 6f20 6265 2063  erations to be c
-000067c0: 6861 696e 6564 2074 6f20 666f 726d 2061  hained to form a
-000067d0: 206c 6172 6765 7220 7069 7065 6c69 6e65   larger pipeline
-000067e0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-000067f0: 2020 2021 5b44 6174 6120 7374 7265 616d     ![Data stream
-00006800: 2070 6970 656c 696e 655d 2864 6f63 756d   pipeline](docum
-00006810: 656e 7461 7469 6f6e 2f69 6d67 2f64 6174  entation/img/dat
-00006820: 615f 7374 7265 616d 5f70 6970 656c 696e  a_stream_pipelin
-00006830: 652e 706e 6729 0a20 2020 2020 2020 200a  e.png).        .
-00006840: 2020 2020 2020 2020 2323 2323 2049 6e74          #### Int
-00006850: 6572 6e61 6c20 6974 6572 6174 696f 6e0a  ernal iteration.
+000018c0: 2020 2020 2262 6174 6368 4964 223a 204e      "batchId": N
+000018d0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+000018e0: 2020 2020 2020 2020 2022 6973 4261 7463           "isBatc
+000018f0: 6865 6422 3a20 4661 6c73 652c 0a20 2020  hed": False,.   
+00001900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001910: 2022 6576 656e 744e 616d 6522 3a20 2253   "eventName": "S
+00001920: 6574 206f 6620 6175 746f 2d67 656e 6572  et of auto-gener
+00001930: 6174 6564 2065 7665 6e74 7320 666f 7220  ated events for 
+00001940: 6473 206c 6962 2074 6573 7469 6e67 222c  ds lib testing",
+00001950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001960: 2020 2020 2022 6576 656e 7454 7970 6522       "eventType"
+00001970: 3a20 2264 732d 6c69 622d 7465 7374 2d65  : "ds-lib-test-e
+00001980: 7665 6e74 222c 0a20 2020 2020 2020 2020  vent",.         
+00001990: 2020 2020 2020 2020 2020 2022 656e 6454             "endT
+000019a0: 696d 6573 7461 6d70 223a 207b 2265 706f  imestamp": {"epo
+000019b0: 6368 5365 636f 6e64 223a 2031 3637 3239  chSecond": 16729
+000019c0: 3237 3032 352c 2022 6e61 6e6f 223a 2035  27025, "nano": 5
+000019d0: 3631 3735 3130 3030 7d2c 0a20 2020 2020  61751000},.     
+000019e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000019f0: 7374 6172 7454 696d 6573 7461 6d70 223a  startTimestamp":
+00001a00: 207b 2265 706f 6368 5365 636f 6e64 223a   {"epochSecond":
+00001a10: 2031 3637 3239 3237 3032 352c 2022 6e61   1672927025, "na
+00001a20: 6e6f 223a 2035 3630 3837 3330 3030 7d2c  no": 560873000},
+00001a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001a40: 2020 2020 2022 7061 7265 6e74 4576 656e       "parentEven
+00001a50: 7449 6422 3a20 4e6f 6e65 2c0a 2020 2020  tId": None,.    
+00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a70: 2273 7563 6365 7373 6675 6c22 3a20 5472  "successful": Tr
+00001a80: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00001a90: 2020 2020 2020 2020 2262 6f6f 6b49 6422          "bookId"
+00001aa0: 3a20 2264 656d 6f5f 626f 6f6b 5f31 222c  : "demo_book_1",
+00001ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001ac0: 2020 2020 2022 7363 6f70 6522 3a20 2274       "scope": "t
+00001ad0: 6832 2d73 636f 7065 222c 0a20 2020 2020  h2-scope",.     
+00001ae0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001af0: 6174 7461 6368 6564 4d65 7373 6167 6549  attachedMessageI
+00001b00: 6473 223a 205b 5d2c 0a20 2020 2020 2020  ds": [],.       
+00001b10: 2020 2020 2020 2020 2020 2020 2022 626f               "bo
+00001b20: 6479 223a 205b 5d2c 0a20 2020 2020 2020  dy": [],.       
+00001b30: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00001b40: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+00001b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b60: 2020 2265 7665 6e74 4964 223a 2022 6465    "eventId": "de
+00001b70: 6d6f 5f62 6f6f 6b5f 313a 7468 322d 7363  mo_book_1:th2-sc
+00001b80: 6f70 653a 3230 3233 3031 3035 3133 3537  ope:202301051357
+00001b90: 3035 3536 3335 3232 3030 303a 3961 6462  05563522000:9adb
+00001ba0: 6233 6530 2d35 6638 622d 3463 3238 2d61  b3e0-5f8b-4c28-a
+00001bb0: 3261 632d 3733 3631 6538 6661 3730 3463  2ac-7361e8fa704c
+00001bc0: 3e64 656d 6f5f 626f 6f6b 5f31 3a74 6832  >demo_book_1:th2
+00001bd0: 2d73 636f 7065 3a32 3032 3330 3130 3531  -scope:202301051
+00001be0: 3335 3730 3535 3633 3532 3230 3030 3a64  35705563522000:d
+00001bf0: 3631 6539 3330 612d 3864 3030 2d31 3165  61e930a-8d00-11e
+00001c00: 642d 6161 3161 2d64 3334 6136 3135 3531  d-aa1a-d34a61551
+00001c10: 3532 645f 3222 2c0a 2020 2020 2020 2020  52d_2",.        
+00001c20: 2020 2020 2020 2020 2020 2020 2262 6174              "bat
+00001c30: 6368 4964 223a 2022 6465 6d6f 5f62 6f6f  chId": "demo_boo
+00001c40: 6b5f 313a 7468 322d 7363 6f70 653a 3230  k_1:th2-scope:20
+00001c50: 3233 3031 3035 3133 3537 3035 3536 3335  2301051357055635
+00001c60: 3232 3030 303a 3961 6462 6233 6530 2d35  22000:9adbb3e0-5
+00001c70: 6638 622d 3463 3238 2d61 3261 632d 3733  f8b-4c28-a2ac-73
+00001c80: 3631 6538 6661 3730 3463 222c 0a20 2020  61e8fa704c",.   
+00001c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ca0: 2022 6973 4261 7463 6865 6422 3a20 5472   "isBatched": Tr
+00001cb0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00001cc0: 2020 2020 2020 2020 2265 7665 6e74 4e61          "eventNa
+00001cd0: 6d65 223a 2022 506c 6169 6e20 6576 656e  me": "Plain even
+00001ce0: 7420 3122 2c0a 2020 2020 2020 2020 2020  t 1",.          
+00001cf0: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
+00001d00: 5479 7065 223a 2022 6473 2d6c 6962 2d74  Type": "ds-lib-t
+00001d10: 6573 742d 6576 656e 7422 2c0a 2020 2020  est-event",.    
+00001d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d30: 2265 6e64 5469 6d65 7374 616d 7022 3a20  "endTimestamp": 
+00001d40: 7b22 6570 6f63 6853 6563 6f6e 6422 3a20  {"epochSecond": 
+00001d50: 3136 3732 3932 3730 3235 2c20 226e 616e  1672927025, "nan
+00001d60: 6f22 3a20 3536 3336 3430 3030 307d 2c0a  o": 563640000},.
+00001d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d80: 2020 2020 2273 7461 7274 5469 6d65 7374      "startTimest
+00001d90: 616d 7022 3a20 7b22 6570 6f63 6853 6563  amp": {"epochSec
+00001da0: 6f6e 6422 3a20 3136 3732 3932 3730 3235  ond": 1672927025
+00001db0: 2c20 226e 616e 6f22 3a20 3536 3335 3232  , "nano": 563522
+00001dc0: 3030 307d 2c0a 2020 2020 2020 2020 2020  000},.          
+00001dd0: 2020 2020 2020 2020 2020 2270 6172 656e            "paren
+00001de0: 7445 7665 6e74 4964 223a 2022 6465 6d6f  tEventId": "demo
+00001df0: 5f62 6f6f 6b5f 313a 7468 322d 7363 6f70  _book_1:th2-scop
+00001e00: 653a 3230 3233 3031 3035 3133 3537 3035  e:20230105135705
+00001e10: 3536 3038 3733 3030 303a 6436 3165 3933  560873000:d61e93
+00001e20: 3061 2d38 6430 302d 3131 6564 2d61 6131  0a-8d00-11ed-aa1
+00001e30: 612d 6433 3461 3631 3535 3135 3264 5f31  a-d34a6155152d_1
+00001e40: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001e50: 2020 2020 2020 2022 7375 6363 6573 7366         "successf
+00001e60: 756c 223a 2054 7275 652c 0a20 2020 2020  ul": True,.     
+00001e70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001e80: 626f 6f6b 4964 223a 2022 6465 6d6f 5f62  bookId": "demo_b
+00001e90: 6f6f 6b5f 3122 2c0a 2020 2020 2020 2020  ook_1",.        
+00001ea0: 2020 2020 2020 2020 2020 2020 2273 636f              "sco
+00001eb0: 7065 223a 2022 7468 322d 7363 6f70 6522  pe": "th2-scope"
+00001ec0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001ed0: 2020 2020 2020 2261 7474 6163 6865 644d        "attachedM
+00001ee0: 6573 7361 6765 4964 7322 3a20 5b5d 2c0a  essageIds": [],.
+00001ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f00: 2020 2020 2262 6f64 7922 3a20 7b22 7479      "body": {"ty
+00001f10: 7065 223a 2022 6d65 7373 6167 6522 2c20  pe": "message", 
+00001f20: 2264 6174 6122 3a20 2264 732d 6c69 6220  "data": "ds-lib 
+00001f30: 7465 7374 2062 6f64 7922 7d2c 0a20 2020  test body"},.   
+00001f40: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
+00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f60: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00001f70: 2020 2020 2020 2265 7665 6e74 4964 223a        "eventId":
+00001f80: 2022 6465 6d6f 5f62 6f6f 6b5f 313a 7468   "demo_book_1:th
+00001f90: 322d 7363 6f70 653a 3230 3233 3031 3035  2-scope:20230105
+00001fa0: 3133 3537 3035 3536 3335 3232 3030 303a  135705563522000:
+00001fb0: 3961 6462 6233 6530 2d35 6638 622d 3463  9adbb3e0-5f8b-4c
+00001fc0: 3238 2d61 3261 632d 3733 3631 6538 6661  28-a2ac-7361e8fa
+00001fd0: 3730 3463 3e64 656d 6f5f 626f 6f6b 5f31  704c>demo_book_1
+00001fe0: 3a74 6832 2d73 636f 7065 3a32 3032 3330  :th2-scope:20230
+00001ff0: 3130 3531 3335 3730 3535 3633 3735 3730  1051357055637570
+00002000: 3030 3a64 3631 6539 3330 612d 3864 3030  00:d61e930a-8d00
+00002010: 2d31 3165 642d 6161 3161 2d64 3334 6136  -11ed-aa1a-d34a6
+00002020: 3135 3531 3532 645f 3322 2c0a 2020 2020  155152d_3",.    
+00002030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002040: 2262 6174 6368 4964 223a 2022 6465 6d6f  "batchId": "demo
+00002050: 5f62 6f6f 6b5f 313a 7468 322d 7363 6f70  _book_1:th2-scop
+00002060: 653a 3230 3233 3031 3035 3133 3537 3035  e:20230105135705
+00002070: 3536 3335 3232 3030 303a 3961 6462 6233  563522000:9adbb3
+00002080: 6530 2d35 6638 622d 3463 3238 2d61 3261  e0-5f8b-4c28-a2a
+00002090: 632d 3733 3631 6538 6661 3730 3463 222c  c-7361e8fa704c",
+000020a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000020b0: 2020 2020 2022 6973 4261 7463 6865 6422       "isBatched"
+000020c0: 3a20 5472 7565 2c0a 2020 2020 2020 2020  : True,.        
+000020d0: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
+000020e0: 6e74 4e61 6d65 223a 2022 506c 6169 6e20  ntName": "Plain 
+000020f0: 6576 656e 7420 3222 2c0a 2020 2020 2020  event 2",.      
+00002100: 2020 2020 2020 2020 2020 2020 2020 2265                "e
+00002110: 7665 6e74 5479 7065 223a 2022 6473 2d6c  ventType": "ds-l
+00002120: 6962 2d74 6573 742d 6576 656e 7422 2c0a  ib-test-event",.
+00002130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002140: 2020 2020 2265 6e64 5469 6d65 7374 616d      "endTimestam
+00002150: 7022 3a20 7b22 6570 6f63 6853 6563 6f6e  p": {"epochSecon
+00002160: 6422 3a20 3136 3732 3932 3730 3235 2c20  d": 1672927025, 
+00002170: 226e 616e 6f22 3a20 3536 3337 3931 3030  "nano": 56379100
+00002180: 307d 2c0a 2020 2020 2020 2020 2020 2020  0},.            
+00002190: 2020 2020 2020 2020 2273 7461 7274 5469          "startTi
+000021a0: 6d65 7374 616d 7022 3a20 7b22 6570 6f63  mestamp": {"epoc
+000021b0: 6853 6563 6f6e 6422 3a20 3136 3732 3932  hSecond": 167292
+000021c0: 3730 3235 2c20 226e 616e 6f22 3a20 3536  7025, "nano": 56
+000021d0: 3337 3537 3030 307d 2c0a 2020 2020 2020  3757000},.      
+000021e0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+000021f0: 6172 656e 7445 7665 6e74 4964 223a 2022  arentEventId": "
+00002200: 6465 6d6f 5f62 6f6f 6b5f 313a 7468 322d  demo_book_1:th2-
+00002210: 7363 6f70 653a 3230 3233 3031 3035 3133  scope:2023010513
+00002220: 3537 3035 3536 3038 3733 3030 303a 6436  5705560873000:d6
+00002230: 3165 3933 3061 2d38 6430 302d 3131 6564  1e930a-8d00-11ed
+00002240: 2d61 6131 612d 6433 3461 3631 3535 3135  -aa1a-d34a615515
+00002250: 3264 5f31 222c 0a20 2020 2020 2020 2020  2d_1",.         
+00002260: 2020 2020 2020 2020 2020 2022 7375 6363             "succ
+00002270: 6573 7366 756c 223a 2054 7275 652c 0a20  essful": True,. 
+00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002290: 2020 2022 626f 6f6b 4964 223a 2022 6465     "bookId": "de
+000022a0: 6d6f 5f62 6f6f 6b5f 3122 2c0a 2020 2020  mo_book_1",.    
+000022b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022c0: 2273 636f 7065 223a 2022 7468 322d 7363  "scope": "th2-sc
+000022d0: 6f70 6522 2c0a 2020 2020 2020 2020 2020  ope",.          
+000022e0: 2020 2020 2020 2020 2020 2261 7474 6163            "attac
+000022f0: 6865 644d 6573 7361 6765 4964 7322 3a20  hedMessageIds": 
+00002300: 5b5d 2c0a 2020 2020 2020 2020 2020 2020  [],.            
+00002310: 2020 2020 2020 2020 2262 6f64 7922 3a20          "body": 
+00002320: 7b22 7479 7065 223a 2022 6d65 7373 6167  {"type": "messag
+00002330: 6522 2c20 2264 6174 6122 3a20 2264 732d  e", "data": "ds-
+00002340: 6c69 6220 7465 7374 2062 6f64 7922 7d2c  lib test body"},
+00002350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002360: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00002370: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00002380: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
+00002390: 4964 223a 2022 6661 6b65 2d65 7665 6e74  Id": "fake-event
+000023a0: 4964 222c 0a20 2020 2020 2020 2020 2020  Id",.           
+000023b0: 2020 2020 2020 2020 2022 6261 7463 6849           "batchI
+000023c0: 6422 3a20 2266 616b 652d 6261 7463 6849  d": "fake-batchI
+000023d0: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
+000023e0: 2020 2020 2020 2020 2269 7342 6174 6368          "isBatch
+000023f0: 6564 223a 2054 7275 652c 0a20 2020 2020  ed": True,.     
+00002400: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002410: 6576 656e 744e 616d 6522 3a20 2246 616b  eventName": "Fak
+00002420: 6520 6576 656e 7422 2c0a 2020 2020 2020  e event",.      
+00002430: 2020 2020 2020 2020 2020 2020 2020 2265                "e
+00002440: 7665 6e74 5479 7065 223a 2022 6473 2d6c  ventType": "ds-l
+00002450: 6962 2d74 6573 742d 6576 656e 7422 2c0a  ib-test-event",.
+00002460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002470: 2020 2020 2265 6e64 5469 6d65 7374 616d      "endTimestam
+00002480: 7022 3a20 7b22 6570 6f63 6853 6563 6f6e  p": {"epochSecon
+00002490: 6422 3a20 3136 3732 3932 3730 3335 2c20  d": 1672927035, 
+000024a0: 226e 616e 6f22 3a20 3536 3337 3931 3030  "nano": 56379100
+000024b0: 307d 2c0a 2020 2020 2020 2020 2020 2020  0},.            
+000024c0: 2020 2020 2020 2020 2273 7461 7274 5469          "startTi
+000024d0: 6d65 7374 616d 7022 3a20 7b22 6570 6f63  mestamp": {"epoc
+000024e0: 6853 6563 6f6e 6422 3a20 3136 3732 3932  hSecond": 167292
+000024f0: 3733 3235 2c20 226e 616e 6f22 3a20 3536  7325, "nano": 56
+00002500: 3337 3537 3030 307d 2c0a 2020 2020 2020  3757000},.      
+00002510: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+00002520: 6172 656e 7445 7665 6e74 4964 223a 2022  arentEventId": "
+00002530: 6e6f 745f 6578 6973 7473 5f69 6e5f 7468  not_exists_in_th
+00002540: 655f 6576 656e 7473 5f73 7472 6561 6d22  e_events_stream"
+00002550: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002560: 2020 2020 2020 2273 7563 6365 7373 6675        "successfu
+00002570: 6c22 3a20 4661 6c73 652c 0a20 2020 2020  l": False,.     
+00002580: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002590: 626f 6f6b 4964 223a 2022 6465 6d6f 5f62  bookId": "demo_b
+000025a0: 6f6f 6b5f 3122 2c0a 2020 2020 2020 2020  ook_1",.        
+000025b0: 2020 2020 2020 2020 2020 2020 2273 636f              "sco
+000025c0: 7065 223a 2022 7468 322d 7363 6f70 6522  pe": "th2-scope"
+000025d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000025e0: 2020 2020 2020 2261 7474 6163 6865 644d        "attachedM
+000025f0: 6573 7361 6765 4964 7322 3a20 5b5d 2c0a  essageIds": [],.
+00002600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002610: 2020 2020 2262 6f64 7922 3a20 7b22 7479      "body": {"ty
+00002620: 7065 223a 2022 6d65 7373 6167 6522 2c20  pe": "message", 
+00002630: 2264 6174 6122 3a20 2264 732d 6c69 6220  "data": "ds-lib 
+00002640: 7465 7374 2062 6f64 7922 7d2c 0a20 2020  test body"},.   
+00002650: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
+00002660: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
+00002670: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00002680: 0a20 2020 2020 2020 2023 2323 2323 2323  .        #######
+00002690: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000026a0: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
+000026b0: 2020 2020 2020 2020 2320 5b31 5d20 576f          # [1] Wo
+000026c0: 726b 696e 6720 7769 7468 2061 2044 6174  rking with a Dat
+000026d0: 6120 6f62 6a65 6374 2e0a 2020 2020 2020  a object..      
+000026e0: 2020 2323 2323 2323 2323 2323 2323 2323    ##############
+000026f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002700: 2323 2323 2323 2323 0a20 2020 2020 2020  ########.       
+00002710: 200a 2020 2020 2020 2020 2320 5b31 2e31   .        # [1.1
+00002720: 5d20 4669 6c74 6572 2e0a 2020 2020 2020  ] Filter..      
+00002730: 2020 6669 6c74 6572 6564 5f65 7665 6e74    filtered_event
+00002740: 733a 2044 6174 6120 3d20 6576 656e 7473  s: Data = events
+00002750: 2e66 696c 7465 7228 6c61 6d62 6461 2065  .filter(lambda e
+00002760: 3a20 655b 2262 6f64 7922 5d20 213d 205b  : e["body"] != [
+00002770: 5d29 2020 2320 4669 6c74 6572 2065 7665  ])  # Filter eve
+00002780: 6e74 7320 7769 7468 2065 6d70 7479 2062  nts with empty b
+00002790: 6f64 792e 0a20 2020 2020 2020 200a 2020  ody..        .  
+000027a0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+000027b0: 205b 312e 325d 204d 6170 2e0a 2020 2020   [1.2] Map..    
+000027c0: 2020 2020 6465 6620 7472 616e 7366 6f72      def transfor
+000027d0: 6d5f 6675 6e63 7469 6f6e 2872 6563 6f72  m_function(recor
+000027e0: 6429 3a0a 2020 2020 2020 2020 2020 2020  d):.            
+000027f0: 7265 7475 726e 207b 2265 7665 6e74 4e61  return {"eventNa
+00002800: 6d65 223a 2072 6563 6f72 645b 2265 7665  me": record["eve
+00002810: 6e74 4e61 6d65 225d 2c20 2273 7563 6365  ntName"], "succe
+00002820: 7373 6675 6c22 3a20 7265 636f 7264 5b22  ssful": record["
+00002830: 7375 6363 6573 7366 756c 225d 7d0a 2020  successful"]}.  
+00002840: 2020 2020 2020 0a20 2020 2020 2020 200a        .        .
+00002850: 2020 2020 2020 2020 6669 6c74 6572 6564          filtered
+00002860: 5f61 6e64 5f6d 6170 7065 645f 6576 656e  _and_mapped_even
+00002870: 7473 203d 2066 696c 7465 7265 645f 6576  ts = filtered_ev
+00002880: 656e 7473 2e6d 6170 2874 7261 6e73 666f  ents.map(transfo
+00002890: 726d 5f66 756e 6374 696f 6e29 0a20 2020  rm_function).   
+000028a0: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+000028b0: 5b31 2e33 5d20 4461 7461 2070 6970 656c  [1.3] Data pipel
+000028c0: 696e 652e 0a20 2020 2020 2020 2023 2020  ine..        #  
+000028d0: 2020 2020 2049 6e73 7465 6164 206f 6620       Instead of 
+000028e0: 646f 696e 6720 6461 7461 2074 7261 6e73  doing data trans
+000028f0: 666f 726d 6174 696f 6e73 2073 7465 7020  formations step 
+00002900: 6279 2073 7465 7020 796f 7520 6361 6e20  by step you can 
+00002910: 646f 2069 7420 696e 206f 6e65 206c 696e  do it in one lin
+00002920: 652e 0a20 2020 2020 2020 2066 696c 7465  e..        filte
+00002930: 7265 645f 616e 645f 6d61 7070 6564 5f65  red_and_mapped_e
+00002940: 7665 6e74 735f 6279 5f70 6970 656c 696e  vents_by_pipelin
+00002950: 6520 3d20 6576 656e 7473 2e66 696c 7465  e = events.filte
+00002960: 7228 6c61 6d62 6461 2065 3a20 655b 2262  r(lambda e: e["b
+00002970: 6f64 7922 5d20 213d 205b 5d29 2e6d 6170  ody"] != []).map
+00002980: 280a 2020 2020 2020 2020 2020 2020 7472  (.            tr
+00002990: 616e 7366 6f72 6d5f 6675 6e63 7469 6f6e  ansform_function
+000029a0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+000029b0: 2020 2023 2043 6f6e 7465 6e74 206f 6620     # Content of 
+000029c0: 7468 6573 6520 7477 6f20 4461 7461 206f  these two Data o
+000029d0: 626a 6563 7473 2073 686f 756c 6420 6265  bjects should be
+000029e0: 2065 7175 616c 2e0a 2020 2020 2020 2020   equal..        
+000029f0: 6173 7365 7274 206c 6973 7428 6669 6c74  assert list(filt
+00002a00: 6572 6564 5f61 6e64 5f6d 6170 7065 645f  ered_and_mapped_
+00002a10: 6576 656e 7473 2920 3d3d 206c 6973 7428  events) == list(
+00002a20: 6669 6c74 6572 6564 5f61 6e64 5f6d 6170  filtered_and_map
+00002a30: 7065 645f 6576 656e 7473 5f62 795f 7069  ped_events_by_pi
+00002a40: 7065 6c69 6e65 290a 2020 2020 2020 2020  peline).        
+00002a50: 0a20 2020 2020 2020 2023 205b 312e 345d  .        # [1.4]
+00002a60: 2053 6966 742e 2053 6b69 7020 7468 6520   Sift. Skip the 
+00002a70: 6669 7273 7420 6665 7720 6974 656d 7320  first few items 
+00002a80: 6f72 206c 696d 6974 2074 6865 6d2e 0a20  or limit them.. 
+00002a90: 2020 2020 2020 2064 6174 6120 3d20 4461         data = Da
+00002aa0: 7461 285b 312c 2032 2c20 332c 2034 2c20  ta([1, 2, 3, 4, 
+00002ab0: 352c 2036 2c20 372c 2038 2c20 392c 2031  5, 6, 7, 8, 9, 1
+00002ac0: 302c 2031 312c 2031 322c 2031 332c 2031  0, 11, 12, 13, 1
+00002ad0: 342c 2031 355d 290a 2020 2020 2020 2020  4, 15]).        
+00002ae0: 6974 656d 735f 6672 6f6d 5f31 315f 746f  items_from_11_to
+00002af0: 5f65 6e64 3a20 4765 6e65 7261 746f 7220  _end: Generator 
+00002b00: 3d20 6461 7461 2e73 6966 7428 736b 6970  = data.sift(skip
+00002b10: 3d31 3029 0a20 2020 2020 2020 206f 6e6c  =10).        onl
+00002b20: 795f 6669 7273 745f 3130 5f69 7465 6d73  y_first_10_items
+00002b30: 3a20 4765 6e65 7261 746f 7220 3d20 6461  : Generator = da
+00002b40: 7461 2e73 6966 7428 6c69 6d69 743d 3130  ta.sift(limit=10
+00002b50: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+00002b60: 2020 2023 205b 312e 355d 2043 6861 6e67     # [1.5] Chang
+00002b70: 696e 6720 6361 6368 6520 7374 6174 7573  ing cache status
+00002b80: 2e0a 2020 2020 2020 2020 6576 656e 7473  ..        events
+00002b90: 2e75 7365 5f63 6163 6865 2854 7275 6529  .use_cache(True)
+00002ba0: 0a20 2020 2020 2020 2023 206f 7220 6a75  .        # or ju
+00002bb0: 7374 0a20 2020 2020 2020 2065 7665 6e74  st.        event
+00002bc0: 732e 7573 655f 6361 6368 6528 2920 2023  s.use_cache()  #
+00002bd0: 2049 6620 796f 7520 7761 6e74 2074 6f20   If you want to 
+00002be0: 6163 7469 7661 7465 2063 6163 6865 2e0a  activate cache..
+00002bf0: 2020 2020 2020 2020 2320 5b31 2e36 5d20          # [1.6] 
+00002c00: 5761 6c6b 2074 6872 6f75 6768 2064 6174  Walk through dat
+00002c10: 612e 0a20 2020 2020 2020 2066 6f72 2065  a..        for e
+00002c20: 7665 6e74 2069 6e20 6576 656e 7473 3a0a  vent in events:.
+00002c30: 2020 2020 2020 2020 2020 2020 2320 446f              # Do
+00002c40: 2073 6f6d 6574 6869 6e67 2077 6974 6820   something with 
+00002c50: 6576 656e 7420 2865 7665 6e74 2069 7320  event (event is 
+00002c60: 6120 6469 6374 292e 0a20 2020 2020 2020  a dict)..       
+00002c70: 2020 2020 2070 7269 6e74 2865 7665 6e74       print(event
+00002c80: 290a 2020 2020 2020 2020 2320 4166 7465  ).        # Afte
+00002c90: 7220 6669 7273 7420 6974 6572 6174 696f  r first iteratio
+00002ca0: 6e20 7468 6520 6576 656e 7473 2068 6173  n the events has
+00002cb0: 2061 2063 6163 6865 2066 696c 652e 0a20   a cache file.. 
+00002cc0: 2020 2020 2020 2023 204e 6f77 2074 6865         # Now the
+00002cd0: 7920 7769 6c6c 2062 6520 7573 6564 2069  y will be used i
+00002ce0: 6e20 7468 6520 6361 6368 6520 696e 2074  n the cache in t
+00002cf0: 6865 206e 6578 7420 6974 6572 6174 696f  he next iteratio
+00002d00: 6e2e 0a20 2020 2020 2020 200a 2020 2020  n..        .    
+00002d10: 2020 2020 2320 5b31 2e37 5d20 4765 7420      # [1.7] Get 
+00002d20: 6e75 6d62 6572 206f 6620 7468 6520 656c  number of the el
+00002d30: 656d 656e 7473 2069 6e20 7468 6520 4461  ements in the Da
+00002d40: 7461 206f 626a 6563 742e 0a20 2020 2020  ta object..     
+00002d50: 2020 206e 756d 6265 725f 6f66 5f65 7665     number_of_eve
+00002d60: 6e74 7320 3d20 6576 656e 7473 2e6c 656e  nts = events.len
+00002d70: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00002d80: 2020 2320 5b31 2e38 5d20 4368 6563 6b20    # [1.8] Check 
+00002d90: 7468 6174 2044 6174 6120 6f62 6a65 6374  that Data object
+00002da0: 2069 736e 2774 2065 6d70 7479 2e0a 2020   isn't empty..  
+00002db0: 2020 2020 2020 2320 5468 6520 6461 7461        # The data
+00002dc0: 2073 6f75 7263 6520 7368 6f75 6c64 2062   source should b
+00002dd0: 6520 6e6f 7420 656d 7074 792e 0a20 2020  e not empty..   
+00002de0: 2020 2020 2061 7373 6572 7420 6576 656e       assert even
+00002df0: 7473 2e69 735f 656d 7074 7920 6973 2046  ts.is_empty is F
+00002e00: 616c 7365 0a20 2020 2020 2020 200a 2020  alse.        .  
+00002e10: 2020 2020 2020 2320 5b31 2e39 5d20 436f        # [1.9] Co
+00002e20: 6e76 6572 7420 4461 7461 206f 626a 6563  nvert Data objec
+00002e30: 7420 746f 2074 6865 206c 6973 7420 6f66  t to the list of
+00002e40: 2065 6c65 6d65 6e74 7328 6576 656e 7473   elements(events
+00002e50: 206f 7220 6d65 7373 6167 6573 292e 0a20   or messages).. 
+00002e60: 2020 2020 2020 2023 2042 6520 6361 7265         # Be care
+00002e70: 6675 6c2c 2074 6869 7320 6361 6e20 7461  ful, this can ta
+00002e80: 6b65 2074 6f6f 206d 7563 6820 6d65 6d6f  ke too much memo
+00002e90: 7279 2e0a 2020 2020 2020 2020 6576 656e  ry..        even
+00002ea0: 7473 5f6c 6973 7420 3d20 6c69 7374 2865  ts_list = list(e
+00002eb0: 7665 6e74 7329 0a20 2020 2020 2020 200a  vents).        .
+00002ec0: 2020 2020 2020 2020 2320 5b31 2e31 305d          # [1.10]
+00002ed0: 2054 6865 2063 6163 6865 2069 6e68 6572   The cache inher
+00002ee0: 6974 616e 6365 2e0a 2020 2020 2020 2020  itance..        
+00002ef0: 2320 4372 6561 7465 7320 6120 6e65 7720  # Creates a new 
+00002f00: 4461 7461 206f 626a 6563 7420 7468 6174  Data object that
+00002f10: 2077 696c 6c20 7573 6520 6361 6368 6520   will use cache 
+00002f20: 6672 6f6d 2074 6865 2065 7665 6e74 7320  from the events 
+00002f30: 4461 7461 206f 626a 6563 742e 0a20 2020  Data object..   
+00002f40: 2020 2020 2065 7665 6e74 735f 6669 6c74       events_filt
+00002f50: 6572 6564 3a20 4461 7461 203d 2065 7665  ered: Data = eve
+00002f60: 6e74 732e 6669 6c74 6572 286c 616d 6264  nts.filter(lambd
+00002f70: 6120 7265 636f 7264 3a20 7265 636f 7264  a record: record
+00002f80: 2e67 6574 2822 6261 7463 6849 6422 2929  .get("batchId"))
+00002f90: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00002fa0: 2020 2320 4e65 7720 4461 7461 206f 626a    # New Data obj
+00002fb0: 6563 7473 2064 6f6e 2774 2075 7365 2074  ects don't use t
+00002fc0: 6865 6972 206f 776e 2063 6163 6865 2062  heir own cache b
+00002fd0: 7920 6465 6661 756c 7420 6275 7420 7573  y default but us
+00002fe0: 6520 7468 6520 6361 6368 6520 6f66 2074  e the cache of t
+00002ff0: 6865 2070 6172 656e 7420 4461 7461 206f  he parent Data o
+00003000: 626a 6563 742e 0a20 2020 2020 2020 2023  bject..        #
+00003010: 2055 7365 2075 7365 5f63 6163 6865 206d   Use use_cache m
+00003020: 6574 686f 6420 746f 2061 6374 6976 6174  ethod to activat
+00003030: 6520 6361 6368 696e 672e 0a20 2020 2020  e caching..     
+00003040: 2020 2023 2041 6674 6572 2074 6861 742c     # After that,
+00003050: 2074 6865 2044 6174 6120 6f62 6a65 6374   the Data object
+00003060: 2077 696c 6c20 6372 6561 7465 2069 7473   will create its
+00003070: 206f 776e 2063 6163 6865 2066 696c 652e   own cache file.
+00003080: 0a20 2020 2020 2020 2065 7665 6e74 735f  .        events_
+00003090: 6669 6c74 6572 6564 2e75 7365 5f63 6163  filtered.use_cac
+000030a0: 6865 2829 0a20 2020 2020 2020 200a 2020  he().        .  
+000030b0: 2020 2020 2020 6c69 7374 2865 7665 6e74        list(event
+000030c0: 735f 6669 6c74 6572 6564 2920 2023 204a  s_filtered)  # J
+000030d0: 7573 7420 746f 2069 7465 7261 7465 2044  ust to iterate D
+000030e0: 6174 6120 6f62 6a65 6374 2028 6361 6368  ata object (cach
+000030f0: 6520 6669 6c65 2077 696c 6c20 6265 2063  e file will be c
+00003100: 7265 6174 6564 292e 0a20 2020 2020 2020  reated)..       
+00003110: 200a 2020 2020 2020 2020 6669 6c74 6572   .        filter
+00003120: 6564 5f65 7665 6e74 735f 7479 7065 7320  ed_events_types 
+00003130: 3d20 6576 656e 7473 5f66 696c 7465 7265  = events_filtere
+00003140: 642e 6d61 7028 6c61 6d62 6461 2072 6563  d.map(lambda rec
+00003150: 6f72 643a 207b 2265 7665 6e74 5479 7065  ord: {"eventType
+00003160: 223a 2072 6563 6f72 642e 6765 7428 2265  ": record.get("e
+00003170: 7665 6e74 5479 7065 2229 7d29 0a20 2020  ventType")}).   
+00003180: 2020 2020 200a 2020 2020 2020 2020 6576       .        ev
+00003190: 656e 7473 5f77 6974 686f 7574 5f74 7970  ents_without_typ
+000031a0: 6573 5f77 6974 685f 6261 7463 6820 3d20  es_with_batch = 
+000031b0: 6669 6c74 6572 6564 5f65 7665 6e74 735f  filtered_events_
+000031c0: 7479 7065 732e 6669 6c74 6572 280a 2020  types.filter(.  
+000031d0: 2020 2020 2020 2020 2020 6c61 6d62 6461            lambda
+000031e0: 2072 6563 6f72 643a 206e 6f74 2072 6563   record: not rec
+000031f0: 6f72 642e 6765 7428 2265 7665 6e74 5479  ord.get("eventTy
+00003200: 7065 2229 0a20 2020 2020 2020 2029 0a20  pe").        ). 
+00003210: 2020 2020 2020 2065 7665 6e74 735f 7769         events_wi
+00003220: 7468 6f75 745f 7479 7065 735f 7769 7468  thout_types_with
+00003230: 5f62 6174 6368 2e75 7365 5f63 6163 6865  _batch.use_cache
+00003240: 2829 0a20 2020 2020 2020 200a 2020 2020  ().        .    
+00003250: 2020 2020 2320 5b31 2e31 315d 2044 6174      # [1.11] Dat
+00003260: 6120 6f62 6a65 6374 7320 6a6f 696e 696e  a objects joinin
+00003270: 672e 0a20 2020 2020 2020 2023 2059 6f75  g..        # You
+00003280: 2068 6176 6520 7468 6520 666f 6c6c 6f77   have the follow
+00003290: 696e 6720 3320 4461 7461 206f 626a 6563  ing 3 Data objec
+000032a0: 7473 2e0a 2020 2020 2020 2020 6431 203d  ts..        d1 =
+000032b0: 2044 6174 6128 5b31 2c20 322c 2033 5d29   Data([1, 2, 3])
+000032c0: 0a20 2020 2020 2020 2064 3220 3d20 4461  .        d2 = Da
+000032d0: 7461 285b 2261 222c 207b 2269 6422 3a20  ta(["a", {"id": 
+000032e0: 3132 337d 2c20 2263 225d 290a 2020 2020  123}, "c"]).    
+000032f0: 2020 2020 6433 203d 2044 6174 6128 5b37      d3 = Data([7
+00003300: 2c20 382c 2039 5d29 0a20 2020 2020 2020  , 8, 9]).       
+00003310: 2023 2059 6f75 2063 616e 206a 6f69 6e20   # You can join 
+00003320: 4461 7461 206f 626a 6563 7473 2069 6e20  Data objects in 
+00003330: 666f 6c6c 6f77 696e 6720 7761 7973 2e0a  following ways..
+00003340: 2020 2020 2020 2020 2320 506c 6561 7365          # Please
+00003350: 206e 6f74 652c 206e 6577 2044 6174 6120   note, new Data 
+00003360: 6f62 6a65 6374 2077 696c 6c20 6861 7665  object will have
+00003370: 2063 6163 6865 2073 7461 7475 7320 3d3d   cache status ==
+00003380: 2046 616c 7365 2e0a 2020 2020 2020 2020   False..        
+00003390: 6461 7461 5f76 6961 5f69 6e69 7420 3d20  data_via_init = 
+000033a0: 4461 7461 285b 6431 2c20 6432 2c20 6433  Data([d1, d2, d3
+000033b0: 5d29 0a20 2020 2020 2020 2064 6174 615f  ]).        data_
+000033c0: 7669 615f 6164 6420 3d20 6431 202b 2064  via_add = d1 + d
+000033d0: 3220 2b20 6433 0a20 2020 2020 2020 2064  2 + d3.        d
+000033e0: 6174 615f 7769 7468 5f6e 6f6e 5f64 6174  ata_with_non_dat
+000033f0: 615f 6f62 6a5f 7669 615f 696e 6974 203d  a_obj_via_init =
+00003400: 2044 6174 6128 5b64 312c 205b 2261 222c   Data([d1, ["a",
+00003410: 207b 2269 6422 3a20 3132 337d 2c20 2263   {"id": 123}, "c
+00003420: 225d 2c20 6433 5d29 0a20 2020 2020 2020  "], d3]).       
+00003430: 2064 6174 615f 7769 7468 5f6e 6f6e 5f64   data_with_non_d
+00003440: 6174 615f 6f62 6a5f 7669 615f 6164 6420  ata_obj_via_add 
+00003450: 3d20 6431 202b 205b 2261 222c 207b 2269  = d1 + ["a", {"i
+00003460: 6422 3a20 3132 337d 2c20 2263 225d 202b  d": 123}, "c"] +
+00003470: 2064 330a 2020 2020 2020 2020 2320 596f   d3.        # Yo
+00003480: 7520 6361 6e20 6a6f 696e 2063 7572 7265  u can join curre
+00003490: 6e74 2044 6174 6120 6f62 6a65 6374 206f  nt Data object o
+000034a0: 6e20 706c 6163 6520 7573 696e 6720 2b3d  n place using +=
+000034b0: 2e0a 2020 2020 2020 2020 2320 4974 2077  ..        # It w
+000034c0: 696c 6c20 6b65 6570 2063 6163 6865 2073  ill keep cache s
+000034d0: 7461 7475 732e 0a20 2020 2020 2020 2064  tatus..        d
+000034e0: 3120 2b3d 2064 3320 2023 2064 3120 7769  1 += d3  # d1 wi
+000034f0: 6c6c 2062 6563 6f6d 6520 4461 7461 285b  ll become Data([
+00003500: 312c 322c 332c 372c 382c 395d 290a 2020  1,2,3,7,8,9]).  
+00003510: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00003520: 205b 312e 3132 5d20 4275 696c 6420 616e   [1.12] Build an
+00003530: 6420 7265 6164 2044 6174 6120 6f62 6a65  d read Data obje
+00003540: 6374 2063 6163 6865 2066 696c 6573 2e0a  ct cache files..
+00003550: 2020 2020 2020 2020 6576 656e 7473 2e62          events.b
+00003560: 7569 6c64 5f63 6163 6865 2822 6361 6368  uild_cache("cach
+00003570: 655f 6669 6c65 6e61 6d65 5f6f 725f 7061  e_filename_or_pa
+00003580: 7468 2229 0a20 2020 2020 2020 2064 6174  th").        dat
+00003590: 615f 6f62 6a5f 6672 6f6d 5f63 6163 6865  a_obj_from_cache
+000035a0: 203d 2044 6174 612e 6672 6f6d 5f63 6163   = Data.from_cac
+000035b0: 6865 5f66 696c 6528 2263 6163 6865 5f66  he_file("cache_f
+000035c0: 696c 656e 616d 655f 6f72 5f70 6174 6822  ilename_or_path"
+000035d0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+000035e0: 2020 2023 205b 312e 3133 5d20 4368 6563     # [1.13] Chec
+000035f0: 6b20 6966 2044 6174 6120 6973 2073 6f72  k if Data is sor
+00003600: 7465 642e 0a20 2020 2020 2020 2023 2054  ted..        # T
+00003610: 6861 7420 7769 6c6c 2072 6574 7572 6e20  hat will return 
+00003620: 616e 206f 626a 6563 7420 6069 735f 736f  an object `is_so
+00003630: 7274 6564 6020 7468 6174 2063 6f6e 7461  rted` that conta
+00003640: 696e 7320 696e 666f 726d 6174 696f 6e0a  ins information.
+00003650: 2020 2020 2020 2020 2320 2020 312e 2073          #   1. s
+00003660: 7461 7475 7320 2d2d 2073 6f72 7465 6420  tatus -- sorted 
+00003670: 6f72 206e 6f74 0a20 2020 2020 2020 2023  or not.        #
+00003680: 2020 2032 2e20 6669 7273 745f 756e 736f     2. first_unso
+00003690: 7274 6564 202d 2d20 7468 6520 696e 6465  rted -- the inde
+000036a0: 7820 6f66 2074 6865 2066 6972 7374 2075  x of the first u
+000036b0: 6e73 6f72 7465 6420 656c 656d 656e 740a  nsorted element.
+000036c0: 2020 2020 2020 2020 6973 5f73 6f72 7465          is_sorte
+000036d0: 6420 3d20 6576 656e 7473 2e69 735f 736f  d = events.is_so
+000036e0: 7274 6564 286c 616d 6264 6120 653a 2065  rted(lambda e: e
+000036f0: 5b22 7374 6172 7454 696d 6573 7461 6d70  ["startTimestamp
+00003700: 225d 5b22 6570 6f63 6853 6563 6f6e 6422  "]["epochSecond"
+00003710: 5d29 0a20 2020 2020 2020 200a 2020 2020  ]).        .    
+00003720: 2020 2020 2320 596f 7520 6361 6e20 7573      # You can us
+00003730: 6520 7468 6973 206f 626a 6563 7420 6173  e this object as
+00003740: 2075 7375 616c 2062 6f6f 6c20 7661 7269   usual bool vari
+00003750: 6162 6c65 2e0a 2020 2020 2020 2020 6966  able..        if
+00003760: 2069 735f 736f 7274 6564 3a0a 2020 2020   is_sorted:.    
+00003770: 2020 2020 2020 2020 7072 696e 7428 2265          print("e
+00003780: 7665 6e74 7320 4461 7461 206f 626a 2069  vents Data obj i
+00003790: 7320 736f 7274 6564 2122 290a 2020 2020  s sorted!").    
+000037a0: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
+000037b0: 312e 3134 5d20 5573 6520 6044 6174 612e  1.14] Use `Data.
+000037c0: 7368 6f77 2829 6020 746f 206c 6f6f 6b20  show()` to look 
+000037d0: 6174 2074 6865 2066 6972 7374 204e 206d  at the first N m
+000037e0: 6573 7361 6765 7320 696e 2074 6865 2073  essages in the s
+000037f0: 7472 6561 6d2e 0a20 2020 2020 2020 2064  tream..        d
+00003800: 6174 615f 7769 7468 5f6e 6f6e 5f64 6174  ata_with_non_dat
+00003810: 615f 6f62 6a5f 7669 615f 6164 642e 7368  a_obj_via_add.sh
+00003820: 6f77 286e 3d36 290a 2020 2020 2020 2020  ow(n=6).        
+00003830: 2320 5769 6c6c 2070 7269 6e74 0a20 2020  # Will print.   
+00003840: 2020 2020 2023 202d 2d2d 2d2d 2d2d 2d2d       # ---------
+00003850: 2d2d 2d2d 2050 7269 6e74 6564 2066 6972  ---- Printed fir
+00003860: 7374 2036 2072 6563 6f72 6473 202d 2d2d  st 6 records ---
+00003870: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00003880: 2020 2023 205b 315d 202d 2d2d 2d2d 2d0a     # [1] ------.
+00003890: 2020 2020 2020 2020 2320 310a 2020 2020          # 1.    
+000038a0: 2020 2020 2320 5b32 5d20 2d2d 2d2d 2d2d      # [2] ------
+000038b0: 0a20 2020 2020 2020 2023 2032 0a20 2020  .        # 2.   
+000038c0: 2020 2020 2023 205b 335d 202d 2d2d 2d2d       # [3] -----
+000038d0: 2d0a 2020 2020 2020 2020 2320 330a 2020  -.        # 3.  
+000038e0: 2020 2020 2020 2320 5b34 5d20 2d2d 2d2d        # [4] ----
+000038f0: 2d2d 0a20 2020 2020 2020 2023 2027 6127  --.        # 'a'
+00003900: 0a20 2020 2020 2020 2023 205b 355d 202d  .        # [5] -
+00003910: 2d2d 2d2d 2d0a 2020 2020 2020 2020 2320  -----.        # 
+00003920: 7b27 6964 273a 2031 3233 7d0a 2020 2020  {'id': 123}.    
+00003930: 2020 2020 2320 5b36 5d20 2d2d 2d2d 2d2d      # [6] ------
+00003940: 0a20 2020 2020 2020 2023 2027 6327 0a20  .        # 'c'. 
+00003950: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00003960: 2320 5b31 2e31 355d 2059 6f75 2063 616e  # [1.15] You can
+00003970: 2072 656d 6f76 6520 7468 6520 6361 6368   remove the cach
+00003980: 6520 6669 6c65 206f 6620 7468 6520 4461  e file of the Da
+00003990: 7461 206f 626a 6563 742c 2069 6620 7265  ta object, if re
+000039a0: 7175 6972 6564 2e0a 2020 2020 2020 2020  quired..        
+000039b0: 6461 7461 5f6f 626a 5f66 726f 6d5f 6361  data_obj_from_ca
+000039c0: 6368 652e 636c 6561 725f 6361 6368 6528  che.clear_cache(
+000039d0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+000039e0: 2020 2023 2323 2323 2323 2323 2323 2323     #############
+000039f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00003a00: 2323 2323 2323 2323 230a 2020 2020 2020  #########.      
+00003a10: 2020 2320 5b32 5d20 576f 726b 696e 6720    # [2] Working 
+00003a20: 7769 7468 2063 6f6e 7665 7274 6572 732e  with converters.
+00003a30: 0a20 2020 2020 2020 2023 2323 2323 2323  .        #######
+00003a40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00003a50: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
+00003a60: 2020 2020 2020 2020 2320 5468 6572 6520          # There 
+00003a70: 6172 6520 6375 7272 656e 746c 7920 7468  are currently th
+00003a80: 7265 6520 696d 706c 656d 656e 7461 7469  ree implementati
+00003a90: 6f6e 7320 6f66 2049 5469 6d65 7374 616d  ons of ITimestam
+00003aa0: 7043 6f6e 7665 7274 6572 2063 6c61 7373  pConverter class
+00003ab0: 3a20 4461 7465 7469 6d65 436f 6e76 6572  : DatetimeConver
+00003ac0: 7465 2c20 4461 7465 7469 6d65 5374 7269  te, DatetimeStri
+00003ad0: 6e67 436f 6e76 6572 7465 7220 616e 6420  ngConverter and 
+00003ae0: 5072 6f74 6f62 7566 5469 6d65 7374 616d  ProtobufTimestam
+00003af0: 7043 6f6e 7665 7274 6572 2e0a 2020 2020  pConverter..    
+00003b00: 2020 2020 2320 5468 6579 2061 6c6c 2069      # They all i
+00003b10: 6d70 6c65 6d65 6e74 2073 616d 6520 6d65  mplement same me
+00003b20: 7468 6f64 7320 6672 6f6d 2062 6173 6520  thods from base 
+00003b30: 636c 6173 732e 0a20 2020 2020 2020 2023  class..        #
+00003b40: 204e 6f74 6520 7468 6174 2073 6f6d 6520   Note that some 
+00003b50: 6163 6375 7261 6379 206d 6179 2062 6520  accuracy may be 
+00003b60: 6c6f 7374 2064 7572 696e 6720 636f 6e76  lost during conv
+00003b70: 6572 7369 6f6e 2e0a 2020 2020 2020 2020  ersion..        
+00003b80: 2320 4966 2066 6f72 2065 7861 6d70 6c65  # If for example
+00003b90: 2079 6f75 2075 7365 2074 6f5f 6d69 6372   you use to_micr
+00003ba0: 6f73 6563 6f6e 6473 206e 616e 6f73 6563  oseconds nanosec
+00003bb0: 6f6e 6473 2077 696c 6c20 6265 2063 7574  onds will be cut
+00003bc0: 206f 6666 2069 6e73 7465 6164 206f 6620   off instead of 
+00003bd0: 726f 756e 6469 6e67 2e0a 2020 2020 2020  rounding..      
+00003be0: 2020 0a20 2020 2020 2020 2023 205b 322e    .        # [2.
+00003bf0: 315d 2044 6174 6574 696d 6543 6f6e 7665  1] DatetimeConve
+00003c00: 7274 6572 2e0a 2020 2020 2020 2020 2320  rter..        # 
+00003c10: 4461 7465 7469 6d65 436f 6e76 6572 7465  DatetimeConverte
+00003c20: 7220 7461 6b65 7320 6461 7465 7469 6d65  r takes datetime
+00003c30: 2e64 6174 6574 696d 6520 6f62 6a65 6374  .datetime object
+00003c40: 2061 7320 696e 7075 742e 0a20 2020 2020   as input..     
+00003c50: 2020 200a 2020 2020 2020 2020 6461 7465     .        date
+00003c60: 7469 6d65 5f6f 626a 203d 2064 6174 6574  time_obj = datet
+00003c70: 696d 6528 7965 6172 3d32 3032 332c 206d  ime(year=2023, m
+00003c80: 6f6e 7468 3d31 2c20 6461 793d 352c 2068  onth=1, day=5, h
+00003c90: 6f75 723d 3134 2c20 6d69 6e75 7465 3d33  our=14, minute=3
+00003ca0: 382c 2073 6563 6f6e 643d 3235 2c20 6d69  8, second=25, mi
+00003cb0: 6372 6f73 6563 6f6e 643d 3134 3630 290a  crosecond=1460).
+00003cc0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00003cd0: 2023 2049 7420 6861 7320 6d65 7468 6f64   # It has method
+00003ce0: 7320 7468 6174 2072 6574 7572 6e20 7468  s that return th
+00003cf0: 6520 6461 7465 7469 6d65 2069 6e20 6469  e datetime in di
+00003d00: 6666 6572 656e 7420 666f 726d 6173 3a0a  fferent formas:.
+00003d10: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00003d20: 2064 6174 655f 6d73 203d 2044 6174 6574   date_ms = Datet
+00003d30: 696d 6543 6f6e 7665 7274 6572 2e74 6f5f  imeConverter.to_
+00003d40: 6d69 6c6c 6973 6563 6f6e 6473 2864 6174  milliseconds(dat
+00003d50: 6574 696d 655f 6f62 6a29 0a20 2020 2020  etime_obj).     
+00003d60: 2020 2064 6174 655f 7573 203d 2044 6174     date_us = Dat
+00003d70: 6574 696d 6543 6f6e 7665 7274 6572 2e74  etimeConverter.t
+00003d80: 6f5f 6d69 6372 6f73 6563 6f6e 6473 2864  o_microseconds(d
+00003d90: 6174 6574 696d 655f 6f62 6a29 0a20 2020  atetime_obj).   
+00003da0: 2020 2020 2023 2043 6f6e 7665 7274 696e       # Convertin
+00003db0: 6720 746f 206e 616e 6f73 6563 6f6e 6473  g to nanoseconds
+00003dc0: 206a 7573 7473 2061 6464 7320 7468 7265   justs adds thre
+00003dd0: 6520 7472 6169 6c69 6e67 207a 6572 6f73  e trailing zeros
+00003de0: 2061 7320 6461 7465 7469 6d65 206f 626a   as datetime obj
+00003df0: 6563 7420 646f 6573 6e27 7420 6861 7665  ect doesn't have
+00003e00: 206e 616e 6f73 6563 6f6e 6473 2e0a 2020   nanoseconds..  
+00003e10: 2020 2020 2020 6461 7465 5f6e 7320 3d20        date_ns = 
+00003e20: 4461 7465 7469 6d65 436f 6e76 6572 7465  DatetimeConverte
+00003e30: 722e 746f 5f6e 616e 6f73 6563 6f6e 6473  r.to_nanoseconds
+00003e40: 2864 6174 6574 696d 655f 6f62 6a29 0a20  (datetime_obj). 
+00003e50: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00003e60: 2320 5b32 2e32 5d20 4461 7465 7469 6d65  # [2.2] Datetime
+00003e70: 5374 7269 6e67 436f 6e76 6572 7465 720a  StringConverter.
+00003e80: 2020 2020 2020 2020 2320 4461 7465 7469          # Dateti
+00003e90: 6d65 5374 7269 6e67 436f 6e76 6572 7465  meStringConverte
+00003ea0: 7220 7461 6b65 7320 7374 7269 6e67 2069  r takes string i
+00003eb0: 6e20 2279 7979 792d 4d4d 2d64 6454 4848  n "yyyy-MM-ddTHH
+00003ec0: 3a6d 6d3a 7373 5b2e 5353 5353 5353 5353  :mm:ss[.SSSSSSSS
+00003ed0: 535d 5a22 2066 6f72 6d61 742e 0a20 2020  S]Z" format..   
+00003ee0: 2020 2020 200a 2020 2020 2020 2020 6461       .        da
+00003ef0: 7465 5f73 7472 696e 6720 3d20 2232 3032  te_string = "202
+00003f00: 332d 3031 2d30 3554 3134 3a33 383a 3235  3-01-05T14:38:25
+00003f10: 2e30 3031 3436 5a22 0a20 2020 2020 2020  .00146Z".       
+00003f20: 200a 2020 2020 2020 2020 2320 5765 2068   .        # We h
+00003f30: 6176 6520 7361 6d65 206d 6574 686f 6473  ave same methods
+00003f40: 2061 7320 696e 2044 6174 6574 696d 6543   as in DatetimeC
+00003f50: 6f6e 7665 7274 6572 0a20 2020 2020 2020  onverter.       
+00003f60: 2064 6174 655f 6d73 5f66 726f 6d5f 7374   date_ms_from_st
+00003f70: 7269 6e67 203d 2044 6174 6574 696d 6553  ring = DatetimeS
+00003f80: 7472 696e 6743 6f6e 7665 7274 6572 2e74  tringConverter.t
+00003f90: 6f5f 6d69 6c6c 6973 6563 6f6e 6473 2864  o_milliseconds(d
+00003fa0: 6174 655f 7374 7269 6e67 290a 2020 2020  ate_string).    
+00003fb0: 2020 2020 6461 7465 5f75 735f 6672 6f6d      date_us_from
+00003fc0: 5f73 7472 696e 6720 3d20 4461 7465 7469  _string = Dateti
+00003fd0: 6d65 5374 7269 6e67 436f 6e76 6572 7465  meStringConverte
+00003fe0: 722e 746f 5f6d 6963 726f 7365 636f 6e64  r.to_microsecond
+00003ff0: 7328 6461 7465 5f73 7472 696e 6729 0a20  s(date_string). 
+00004000: 2020 2020 2020 2064 6174 655f 6e73 5f66         date_ns_f
+00004010: 726f 6d5f 7374 7269 6e67 203d 2044 6174  rom_string = Dat
+00004020: 6574 696d 6553 7472 696e 6743 6f6e 7665  etimeStringConve
+00004030: 7274 6572 2e74 6f5f 6e61 6e6f 7365 636f  rter.to_nanoseco
+00004040: 6e64 7328 6461 7465 5f73 7472 696e 6729  nds(date_string)
+00004050: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00004060: 2020 2320 5765 2063 616e 2061 6c73 6f20    # We can also 
+00004070: 6765 7420 6461 7465 7469 6d65 206f 626a  get datetime obj
+00004080: 6563 7420 6672 6f6d 2073 7472 696e 670a  ect from string.
+00004090: 2020 2020 2020 2020 6461 7465 7469 6d65          datetime
+000040a0: 5f66 726f 6d5f 7374 7269 6e67 203d 2044  _from_string = D
+000040b0: 6174 6574 696d 6553 7472 696e 6743 6f6e  atetimeStringCon
+000040c0: 7665 7274 6572 2e74 6f5f 6461 7465 7469  verter.to_dateti
+000040d0: 6d65 2864 6174 655f 7374 7269 6e67 290a  me(date_string).
+000040e0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000040f0: 2023 205b 322e 335d 2050 726f 746f 6275   # [2.3] Protobu
+00004100: 6654 696d 6573 7461 6d70 436f 6e76 6572  fTimestampConver
+00004110: 7465 720a 2020 2020 2020 2020 2320 5072  ter.        # Pr
+00004120: 6f74 6f62 7566 2074 696d 6573 7461 6d70  otobuf timestamp
+00004130: 7320 6d75 7374 2062 6520 696e 2066 6f72  s must be in for
+00004140: 6d20 7b22 6570 6f63 6853 6563 6f6e 6422  m {"epochSecond"
+00004150: 3a20 7365 636f 6e64 732c 2022 6e61 6e6f  : seconds, "nano
+00004160: 223a 206e 616e 6f73 6563 6f6e 6473 7d0a  ": nanoseconds}.
+00004170: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00004180: 2070 726f 746f 6275 665f 7469 6d65 7374   protobuf_timest
+00004190: 616d 7020 3d20 7b22 6570 6f63 6853 6563  amp = {"epochSec
+000041a0: 6f6e 6422 3a20 3136 3732 3932 3935 3035  ond": 1672929505
+000041b0: 2c20 226e 616e 6f22 3a20 315f 3436 305f  , "nano": 1_460_
+000041c0: 3030 307d 0a20 2020 2020 2020 200a 2020  000}.        .  
+000041d0: 2020 2020 2020 6461 7465 5f6d 735f 6672        date_ms_fr
+000041e0: 6f6d 5f74 696d 6573 7461 6d70 203d 2050  om_timestamp = P
+000041f0: 726f 746f 6275 6654 696d 6573 7461 6d70  rotobufTimestamp
+00004200: 436f 6e76 6572 7465 722e 746f 5f6d 696c  Converter.to_mil
+00004210: 6c69 7365 636f 6e64 7328 7072 6f74 6f62  liseconds(protob
+00004220: 7566 5f74 696d 6573 7461 6d70 290a 2020  uf_timestamp).  
+00004230: 2020 2020 2020 6461 7465 5f75 735f 6672        date_us_fr
+00004240: 6f6d 5f74 696d 6573 7461 6d70 203d 2050  om_timestamp = P
+00004250: 726f 746f 6275 6654 696d 6573 7461 6d70  rotobufTimestamp
+00004260: 436f 6e76 6572 7465 722e 746f 5f6d 6963  Converter.to_mic
+00004270: 726f 7365 636f 6e64 7328 7072 6f74 6f62  roseconds(protob
+00004280: 7566 5f74 696d 6573 7461 6d70 290a 2020  uf_timestamp).  
+00004290: 2020 2020 2020 6461 7465 5f6e 735f 6672        date_ns_fr
+000042a0: 6f6d 5f74 696d 6573 7461 6d70 203d 2050  om_timestamp = P
+000042b0: 726f 746f 6275 6654 696d 6573 7461 6d70  rotobufTimestamp
+000042c0: 436f 6e76 6572 7465 722e 746f 5f6e 616e  Converter.to_nan
+000042d0: 6f73 6563 6f6e 6473 2870 726f 746f 6275  oseconds(protobu
+000042e0: 665f 7469 6d65 7374 616d 7029 0a20 2020  f_timestamp).   
+000042f0: 2020 2020 2064 6174 6574 696d 655f 6672       datetime_fr
+00004300: 6f6d 5f74 696d 6573 7461 6d70 203d 2050  om_timestamp = P
+00004310: 726f 746f 6275 6654 696d 6573 7461 6d70  rotobufTimestamp
+00004320: 436f 6e76 6572 7465 722e 746f 5f64 6174  Converter.to_dat
+00004330: 6574 696d 6528 7072 6f74 6f62 7566 5f74  etime(protobuf_t
+00004340: 696d 6573 7461 6d70 290a 2020 2020 2020  imestamp).      
+00004350: 2020 0a20 2020 2020 2020 2023 2323 2323    .        #####
+00004360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004380: 230a 2020 2020 2020 2020 2320 5b33 5d20  #.        # [3] 
+00004390: 576f 726b 696e 6720 7769 7468 2045 7665  Working with Eve
+000043a0: 6e74 5472 6565 2061 6e64 2045 7665 6e74  ntTree and Event
+000043b0: 5472 6565 436f 6c6c 6563 7469 6f6e 2e0a  TreeCollection..
+000043c0: 2020 2020 2020 2020 2323 2323 2323 2323          ########
+000043d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000043e0: 2323 2323 2323 2323 2323 2323 2323 0a20  ##############. 
+000043f0: 2020 2020 2020 2023 2043 616e 2062 6520         # Can be 
+00004400: 7573 6566 756c 2069 6620 796f 7520 6861  useful if you ha
+00004410: 7665 2064 6174 612d 7374 7265 616d 2077  ve data-stream w
+00004420: 6974 6820 3c20 3130 306b 2065 6c65 6d65  ith < 100k eleme
+00004430: 6e74 732c 206f 7468 6572 7769 7365 2069  nts, otherwise i
+00004440: 740a 2020 2020 2020 2020 2320 7461 6b65  t.        # take
+00004450: 7320 746f 6f20 6d75 6368 2052 414d 2e0a  s too much RAM..
+00004460: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00004470: 2023 205b 332e 315d 2042 7569 6c64 2061   # [3.1] Build a
+00004480: 2063 7573 746f 6d20 4576 656e 7454 7265   custom EventTre
+00004490: 650a 2020 2020 2020 2020 2320 546f 2063  e.        # To c
+000044a0: 7265 6174 6520 616e 2045 7665 6e74 5472  reate an EventTr
+000044b0: 6565 206f 626a 6563 7420 796f 7520 6e65  ee object you ne
+000044c0: 6564 2074 6f20 7072 6f76 6964 6520 6e61  ed to provide na
+000044d0: 6d65 2c20 6964 2061 6e64 2064 6174 6120  me, id and data 
+000044e0: 6f66 2074 6865 2072 6f6f 7420 6576 656e  of the root even
+000044f0: 742e 0a20 2020 2020 2020 2074 7265 6520  t..        tree 
+00004500: 3d20 4576 656e 7454 7265 6528 6576 656e  = EventTree(even
+00004510: 745f 6e61 6d65 3d22 726f 6f74 2065 7665  t_name="root eve
+00004520: 6e74 222c 2065 7665 6e74 5f69 643d 2272  nt", event_id="r
+00004530: 6f6f 745f 6964 222c 2064 6174 613d 7b22  oot_id", data={"
+00004540: 6461 7461 223a 205b 312c 2032 2c20 332c  data": [1, 2, 3,
+00004550: 2034 2c20 355d 7d29 0a20 2020 2020 2020   4, 5]}).       
+00004560: 200a 2020 2020 2020 2020 2320 546f 2061   .        # To a
+00004570: 6464 206e 6577 206e 6f64 6520 7573 6520  dd new node use 
+00004580: 6170 7065 6e64 5f65 7665 6e74 2e20 7061  append_event. pa
+00004590: 7265 6e74 5f69 6420 6973 206e 6563 6573  rent_id is neces
+000045a0: 7361 7279 2c20 6461 7461 2069 7320 6f70  sary, data is op
+000045b0: 7469 6f6e 616c 2e0a 2020 2020 2020 2020  tional..        
+000045c0: 7472 6565 2e61 7070 656e 645f 6576 656e  tree.append_even
+000045d0: 7428 6576 656e 745f 6e61 6d65 3d22 4122  t(event_name="A"
+000045e0: 2c20 6576 656e 745f 6964 3d22 415f 6964  , event_id="A_id
+000045f0: 222c 2064 6174 613d 4e6f 6e65 2c20 7061  ", data=None, pa
+00004600: 7265 6e74 5f69 643d 2272 6f6f 745f 6964  rent_id="root_id
+00004610: 2229 0a20 2020 2020 2020 200a 2020 2020  ").        .    
+00004620: 2020 2020 2320 5b33 2e33 5d20 4275 696c      # [3.3] Buil
+00004630: 6469 6e67 2074 6865 2045 7665 6e74 5472  ding the EventTr
+00004640: 6565 436f 6c6c 6563 7469 6f6e 2e0a 2020  eeCollection..  
+00004650: 2020 2020 2020 6461 7461 5f73 6f75 7263        data_sourc
+00004660: 653a 2049 4461 7461 536f 7572 6365 2020  e: IDataSource  
+00004670: 2320 596f 7520 7368 6f75 6c64 2069 6e69  # You should ini
+00004680: 7420 4461 7461 536f 7572 6365 206f 626a  t DataSource obj
+00004690: 6563 742e 2045 2e67 2e20 6672 6f6d 204c  ect. E.g. from L
+000046a0: 7744 5020 6d6f 6475 6c65 2e0a 2020 2020  wDP module..    
+000046b0: 2020 2020 6461 7461 5f73 6f75 7263 6520      data_source 
+000046c0: 3d20 4475 6d6d 7944 6174 6153 6f75 7263  = DummyDataSourc
+000046d0: 6528 2920 2023 204e 6f74 6521 2057 6520  e()  # Note! We 
+000046e0: 7573 6520 6661 6b65 2044 5320 6865 7265  use fake DS here
+000046f0: 2e0a 2020 2020 2020 2020 2320 4554 4344  ..        # ETCD
+00004700: 7269 7665 7220 6865 7265 2069 7320 6120  river here is a 
+00004710: 7374 7562 2c20 6163 7475 616c 6c79 2074  stub, actually t
+00004720: 6865 206c 6962 2064 6f65 736e 2774 2068  he lib doesn't h
+00004730: 6176 6520 7375 6368 2061 2063 6c61 7373  ave such a class
+00004740: 2e0a 2020 2020 2020 2020 2320 596f 7520  ..        # You 
+00004750: 6361 6e20 7461 6b65 2069 7420 696e 204c  can take it in L
+00004760: 7744 5020 6d6f 6475 6c65 206f 7220 6372  wDP module or cr
+00004770: 6561 7465 2079 6f75 7273 656c 6620 636c  eate yourself cl
+00004780: 6173 7320 6966 2079 6f75 2068 6176 6520  ass if you have 
+00004790: 736f 6d65 2073 7065 6369 616c 2065 7665  some special eve
+000047a0: 6e74 7320 7374 7275 6374 7572 652e 0a20  nts structure.. 
+000047b0: 2020 2020 2020 2066 726f 6d20 7468 325f         from th2_
+000047c0: 6461 7461 5f73 6572 7669 6365 732e 6461  data_services.da
+000047d0: 7461 5f73 6f75 7263 652e 6c77 6470 2e65  ta_source.lwdp.e
+000047e0: 7665 6e74 5f74 7265 6520 696d 706f 7274  vent_tree import
+000047f0: 2048 7474 7045 5443 4472 6976 6572 2061   HttpETCDriver a
+00004800: 7320 4554 4344 7269 7665 720a 2020 2020  s ETCDriver.    
+00004810: 2020 2020 0a20 2020 2020 2020 2023 2049      .        # I
+00004820: 6620 796f 7520 646f 6e27 7420 7370 6563  f you don't spec
+00004830: 6966 7920 6461 7461 5f73 6f75 7263 6520  ify data_source 
+00004840: 666f 7220 7468 6520 6472 6976 6572 2074  for the driver t
+00004850: 6865 6e20 6974 2077 6f6e 2774 2072 6563  hen it won't rec
+00004860: 6f76 6572 2064 6574 6163 6865 6420 6576  over detached ev
+00004870: 656e 7473 2e0a 2020 2020 2020 2020 6472  ents..        dr
+00004880: 6976 6572 3a20 4945 5443 4472 6976 6572  iver: IETCDriver
+00004890: 2020 2320 596f 7520 7368 6f75 6c64 2069    # You should i
+000048a0: 6e69 7420 4554 4344 7269 7665 7220 6f62  nit ETCDriver ob
+000048b0: 6a65 6374 2e20 452e 672e 2066 726f 6d20  ject. E.g. from 
+000048c0: 4c77 4450 206d 6f64 756c 6520 6f72 2079  LwDP module or y
+000048d0: 6f75 7220 6375 7374 6f6d 2063 6c61 7373  our custom class
+000048e0: 2e0a 2020 2020 2020 2020 6472 6976 6572  ..        driver
+000048f0: 203d 2045 5443 4472 6976 6572 2864 6174   = ETCDriver(dat
+00004900: 615f 736f 7572 6365 3d64 6174 615f 736f  a_source=data_so
+00004910: 7572 6365 2c20 7573 655f 7374 7562 3d54  urce, use_stub=T
+00004920: 7275 6529 0a20 2020 2020 2020 200a 2020  rue).        .  
+00004930: 2020 2020 2020 6574 6320 3d20 4576 656e        etc = Even
+00004940: 7454 7265 6543 6f6c 6c65 6374 696f 6e28  tTreeCollection(
+00004950: 6472 6976 6572 290a 2020 2020 2020 2020  driver).        
+00004960: 6574 632e 6275 696c 6428 6576 656e 7473  etc.build(events
+00004970: 290a 2020 2020 2020 2020 6574 632e 7368  ).        etc.sh
+00004980: 6f77 2829 0a20 2020 2020 2020 2023 2049  ow().        # I
+00004990: 7427 6c6c 2070 7269 6e74 2074 6865 2066  t'll print the f
+000049a0: 6f6c 6c6f 7769 6e67 3a0a 2020 2020 2020  ollowing:.      
+000049b0: 2020 2320 5365 7420 6f66 2061 7574 6f2d    # Set of auto-
+000049c0: 6765 6e65 7261 7465 6420 6576 656e 7473  generated events
+000049d0: 2066 6f72 2064 7320 6c69 6220 7465 7374   for ds lib test
+000049e0: 696e 670a 2020 2020 2020 2020 2320 e294  ing.        # ..
+000049f0: 9ce2 9480 e294 8020 506c 6169 6e20 6576  ....... Plain ev
+00004a00: 656e 7420 310a 2020 2020 2020 2020 2320  ent 1.        # 
+00004a10: e294 94e2 9480 e294 8020 506c 6169 6e20  ......... Plain 
+00004a20: 6576 656e 7420 320a 2020 2020 2020 2020  event 2.        
+00004a30: 0a20 2020 2020 2020 2070 7269 6e74 2865  .        print(e
+00004a40: 7463 290a 2020 2020 2020 2020 2320 4576  tc).        # Ev
+00004a50: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
+00004a60: 6e28 7472 6565 733d 312c 2065 7665 6e74  n(trees=1, event
+00004a70: 733d 335b 7472 6565 733d 332c 2064 6574  s=3[trees=3, det
+00004a80: 6163 6865 643d 305d 290a 2020 2020 2020  ached=0]).      
+00004a90: 2020 0a20 2020 2020 2020 2023 2044 6574    .        # Det
+00004aa0: 6163 6865 6420 6576 656e 7473 2069 736e  ached events isn
+00004ab0: 2774 2065 6d70 7479 2e0a 2020 2020 2020  't empty..      
+00004ac0: 2020 6173 7365 7274 2065 7463 2e67 6574    assert etc.get
+00004ad0: 5f64 6574 6163 6865 645f 6576 656e 7473  _detached_events
+00004ae0: 2829 2020 2320 7265 7475 726e 7320 6c69  ()  # returns li
+00004af0: 7374 206f 6620 6465 7461 6368 6564 5f65  st of detached_e
+00004b00: 7665 6e74 732e 0a20 2020 2020 2020 200a  vents..        .
+00004b10: 2020 2020 2020 2020 2320 7265 636f 7665          # recove
+00004b20: 725f 756e 6b6e 6f77 6e5f 6576 656e 7473  r_unknown_events
+00004b30: 202d 2d20 7573 6564 2074 6f20 7265 636f   -- used to reco
+00004b40: 7665 7220 736f 6d65 2065 7665 6e74 7320  ver some events 
+00004b50: 7061 7265 6e74 732e 0a20 2020 2020 2020  parents..       
+00004b60: 2023 2054 6861 7420 776f 6e27 7420 776f   # That won't wo
+00004b70: 726b 2077 6974 6820 4475 6d6d 7944 6174  rk with DummyDat
+00004b80: 6153 6f75 7263 652c 2073 6f20 7761 7320  aSource, so was 
+00004b90: 636f 6d6d 656e 7465 640a 2020 2020 2020  commented.      
+00004ba0: 2020 2320 6574 632e 7265 636f 7665 725f    # etc.recover_
+00004bb0: 756e 6b6e 6f77 6e5f 6576 656e 7473 2829  unknown_events()
+00004bc0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00004bd0: 2020 2320 4166 7465 7220 7468 6174 2074    # After that t
+00004be0: 6865 2064 6574 6163 6865 6420 6576 656e  he detached even
+00004bf0: 7473 2073 686f 756c 6420 6265 2065 6d70  ts should be emp
+00004c00: 7479 2062 6563 6175 7365 2074 6865 7920  ty because they 
+00004c10: 7765 7265 2072 6563 6f76 6572 6564 2e0a  were recovered..
+00004c20: 2020 2020 2020 2020 2320 6173 7365 7274          # assert
+00004c30: 206e 6f74 2065 7463 2e67 6574 5f64 6574   not etc.get_det
+00004c40: 6163 6865 645f 6576 656e 7473 2829 0a20  ached_events(). 
+00004c50: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00004c60: 2320 2d2d 2d2d 2d0a 2020 2020 2020 2020  # -----.        
+00004c70: 0a20 2020 2020 2020 2023 2054 6865 2063  .        # The c
+00004c80: 6f6c 6c65 6374 696f 6e20 6861 7320 4576  ollection has Ev
+00004c90: 656e 7454 7265 6573 2065 6163 6820 7769  entTrees each wi
+00004ca0: 7468 2061 2074 7265 6520 6f66 2065 7665  th a tree of eve
+00004cb0: 6e74 732e 0a20 2020 2020 2020 2023 2055  nts..        # U
+00004cc0: 7369 6e67 2043 6f6c 6c65 6374 696f 6e20  sing Collection 
+00004cd0: 616e 6420 4576 656e 7454 7265 6573 2c20  and EventTrees, 
+00004ce0: 796f 7520 6361 6e20 776f 726b 2066 6c65  you can work fle
+00004cf0: 7869 626c 7920 7769 7468 2065 7665 6e74  xibly with event
+00004d00: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
+00004d10: 2020 2020 2320 5b33 2e33 2e31 5d20 4765      # [3.3.1] Ge
+00004d20: 7420 6c65 6176 6573 206f 6620 616c 6c20  t leaves of all 
+00004d30: 7472 6565 732e 0a20 2020 2020 2020 206c  trees..        l
+00004d40: 6561 7665 733a 2054 7570 6c65 5b64 6963  eaves: Tuple[dic
+00004d50: 745d 203d 2065 7463 2e67 6574 5f6c 6561  t] = etc.get_lea
+00004d60: 7665 7328 2920 2023 2052 6574 7572 6e73  ves()  # Returns
+00004d70: 2061 2074 7570 6c65 206f 6620 6c65 6176   a tuple of leav
+00004d80: 6573 2065 7665 6e74 730a 2020 2020 2020  es events.      
+00004d90: 2020 0a20 2020 2020 2020 2023 205b 332e    .        # [3.
+00004da0: 332e 325d 2047 6574 2072 6f6f 7473 2069  3.2] Get roots i
+00004db0: 6473 206f 6620 616c 6c20 7472 6565 732e  ds of all trees.
+00004dc0: 0a20 2020 2020 2020 2072 6f6f 7473 3a20  .        roots: 
+00004dd0: 4c69 7374 5b73 7472 5d20 3d20 6574 632e  List[str] = etc.
+00004de0: 6765 745f 726f 6f74 735f 6964 7328 290a  get_roots_ids().
+00004df0: 2020 2020 2020 2020 2320 5265 7475 726e          # Return
+00004e00: 7320 7468 6520 6c69 7374 206f 6620 726f  s the list of ro
+00004e10: 6f74 2049 6473 3a0a 2020 2020 2020 2020  ot Ids:.        
+00004e20: 2320 5b27 6465 6d6f 5f62 6f6f 6b5f 313a  # ['demo_book_1:
+00004e30: 7468 322d 7363 6f70 653a 3230 3233 3031  th2-scope:202301
+00004e40: 3035 3133 3537 3035 3536 3038 3733 3030  0513570556087300
+00004e50: 303a 6436 3165 3933 3061 2d38 6430 302d  0:d61e930a-8d00-
+00004e60: 3131 6564 2d61 6131 612d 6433 3461 3631  11ed-aa1a-d34a61
+00004e70: 3535 3135 3264 5f31 275d 0a20 2020 2020  55152d_1'].     
+00004e80: 2020 200a 2020 2020 2020 2020 2320 5b33     .        # [3
+00004e90: 2e33 2e33 5d20 4669 6e64 2061 6e20 6576  .3.3] Find an ev
+00004ea0: 656e 7420 696e 2061 6c6c 2074 7265 6573  ent in all trees
+00004eb0: 2e0a 2020 2020 2020 2020 6669 6e64 5f65  ..        find_e
+00004ec0: 7665 6e74 3a20 4f70 7469 6f6e 616c 5b64  vent: Optional[d
+00004ed0: 6963 745d 203d 2065 7463 2e66 696e 6428  ict] = etc.find(
+00004ee0: 6c61 6d62 6461 2065 7665 6e74 3a20 2253  lambda event: "S
+00004ef0: 656e 6420 6d65 7373 6167 6522 2069 6e20  end message" in 
+00004f00: 6576 656e 745b 2265 7665 6e74 5479 7065  event["eventType
+00004f10: 225d 290a 2020 2020 2020 2020 0a20 2020  "]).        .   
+00004f20: 2020 2020 2023 205b 332e 332e 345d 2046       # [3.3.4] F
+00004f30: 696e 6420 616c 6c20 6576 656e 7473 2069  ind all events i
+00004f40: 6e20 616c 6c20 7472 6565 732e 2054 6865  n all trees. The
+00004f50: 7265 2069 7320 616c 736f 2069 7465 7261  re is also itera
+00004f60: 626c 6520 7665 7273 696f 6e20 2766 696e  ble version 'fin
+00004f70: 6461 6c6c 5f69 7465 7227 2e0a 2020 2020  dall_iter'..    
+00004f80: 2020 2020 6669 6e64 5f65 7665 6e74 733a      find_events:
+00004f90: 204c 6973 745b 6469 6374 5d20 3d20 6574   List[dict] = et
+00004fa0: 632e 6669 6e64 616c 6c28 6c61 6d62 6461  c.findall(lambda
+00004fb0: 2065 7665 6e74 3a20 6576 656e 745b 2273   event: event["s
+00004fc0: 7563 6365 7373 6675 6c22 5d20 6973 2054  uccessful"] is T
+00004fd0: 7275 6529 0a20 2020 2020 2020 200a 2020  rue).        .  
+00004fe0: 2020 2020 2020 2320 5b33 2e33 2e35 5d20        # [3.3.5] 
+00004ff0: 4669 6e64 2061 6e20 616e 6365 7374 6f72  Find an ancestor
+00005000: 206f 6620 7468 6520 6576 656e 742e 0a20   of the event.. 
+00005010: 2020 2020 2020 2061 6e63 6573 746f 723a         ancestor:
+00005020: 204f 7074 696f 6e61 6c5b 6469 6374 5d20   Optional[dict] 
+00005030: 3d20 6574 632e 6669 6e64 5f61 6e63 6573  = etc.find_ances
+00005040: 746f 7228 0a20 2020 2020 2020 2020 2020  tor(.           
+00005050: 2022 6465 6d6f 5f62 6f6f 6b5f 313a 7468   "demo_book_1:th
+00005060: 322d 7363 6f70 653a 3230 3233 3031 3035  2-scope:20230105
+00005070: 3133 3537 3035 3536 3038 3733 3030 303a  135705560873000:
+00005080: 6436 3165 3933 3061 2d38 6430 302d 3131  d61e930a-8d00-11
+00005090: 6564 2d61 6131 612d 6433 3461 3631 3535  ed-aa1a-d34a6155
+000050a0: 3135 3264 5f31 222c 0a20 2020 2020 2020  152d_1",.       
+000050b0: 2020 2020 2066 696c 7465 723d 6c61 6d62       filter=lamb
+000050c0: 6461 2065 7665 6e74 3a20 2252 6f6f 7445  da event: "RootE
+000050d0: 7665 6e74 2220 696e 2065 7665 6e74 5b22  vent" in event["
+000050e0: 6576 656e 744e 616d 6522 5d2c 0a20 2020  eventName"],.   
+000050f0: 2020 2020 2029 0a20 2020 2020 2020 200a       ).        .
+00005100: 2020 2020 2020 2020 2320 5b33 2e33 2e36          # [3.3.6
+00005110: 5d20 4765 7420 6368 696c 6472 656e 206f  ] Get children o
+00005120: 6620 7468 6520 6576 656e 742e 2054 6865  f the event. The
+00005130: 7265 2069 7320 616c 736f 2069 7465 7261  re is also itera
+00005140: 626c 6520 7665 7273 696f 6e20 2767 6574  ble version 'get
+00005150: 5f63 6869 6c64 7265 6e5f 6974 6572 272e  _children_iter'.
+00005160: 0a20 2020 2020 2020 2063 6869 6c64 7265  .        childre
+00005170: 6e3a 2054 7570 6c65 5b64 6963 745d 203d  n: Tuple[dict] =
+00005180: 2065 7463 2e67 6574 5f63 6869 6c64 7265   etc.get_childre
+00005190: 6e28 0a20 2020 2020 2020 2020 2020 2022  n(.            "
+000051a0: 6465 6d6f 5f62 6f6f 6b5f 313a 7468 322d  demo_book_1:th2-
+000051b0: 7363 6f70 653a 3230 3233 3031 3035 3133  scope:2023010513
+000051c0: 3537 3035 3536 3038 3733 3030 303a 6436  5705560873000:d6
+000051d0: 3165 3933 3061 2d38 6430 302d 3131 6564  1e930a-8d00-11ed
+000051e0: 2d61 6131 612d 6433 3461 3631 3535 3135  -aa1a-d34a615515
+000051f0: 3264 5f31 220a 2020 2020 2020 2020 290a  2d_1".        ).
+00005200: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00005210: 2023 205b 332e 332e 375d 2047 6574 2073   # [3.3.7] Get s
+00005220: 7562 7472 6565 2066 6f72 2073 7065 6369  ubtree for speci
+00005230: 6669 6564 2065 7665 6e74 2e0a 2020 2020  fied event..    
+00005240: 2020 2020 7375 6274 7265 653a 2045 7665      subtree: Eve
+00005250: 6e74 5472 6565 203d 2065 7463 2e67 6574  ntTree = etc.get
+00005260: 5f73 7562 7472 6565 280a 2020 2020 2020  _subtree(.      
+00005270: 2020 2020 2020 2264 656d 6f5f 626f 6f6b        "demo_book
+00005280: 5f31 3a74 6832 2d73 636f 7065 3a32 3032  _1:th2-scope:202
+00005290: 3330 3130 3531 3335 3730 3535 3630 3837  3010513570556087
+000052a0: 3330 3030 3a64 3631 6539 3330 612d 3864  3000:d61e930a-8d
+000052b0: 3030 2d31 3165 642d 6161 3161 2d64 3334  00-11ed-aa1a-d34
+000052c0: 6136 3135 3531 3532 645f 3122 0a20 2020  a6155152d_1".   
+000052d0: 2020 2020 2029 0a20 2020 2020 2020 200a       ).        .
+000052e0: 2020 2020 2020 2020 2320 5b33 2e33 2e38          # [3.3.8
+000052f0: 5d20 4765 7420 6675 6c6c 2070 6174 6820  ] Get full path 
+00005300: 746f 2074 6865 2065 7665 6e74 2e0a 2020  to the event..  
+00005310: 2020 2020 2020 2320 4c6f 6f6b 7320 6c69        # Looks li
+00005320: 6b65 205b 616e 6365 7374 6f72 5f72 6f6f  ke [ancestor_roo
+00005330: 742c 2061 6e63 6573 746f 725f 6c65 7665  t, ancestor_leve
+00005340: 6c31 2c20 616e 6365 7374 6f72 5f6c 6576  l1, ancestor_lev
+00005350: 656c 322c 2065 7665 6e74 5d0a 2020 2020  el2, event].    
+00005360: 2020 2020 6576 656e 745f 7061 7468 3a20      event_path: 
+00005370: 4c69 7374 5b64 6963 745d 203d 2065 7463  List[dict] = etc
+00005380: 2e67 6574 5f66 756c 6c5f 7061 7468 280a  .get_full_path(.
+00005390: 2020 2020 2020 2020 2020 2020 2264 656d              "dem
+000053a0: 6f5f 626f 6f6b 5f31 3a74 6832 2d73 636f  o_book_1:th2-sco
+000053b0: 7065 3a32 3032 3330 3130 3531 3335 3730  pe:2023010513570
+000053c0: 3535 3630 3837 3330 3030 3a64 3631 6539  5560873000:d61e9
+000053d0: 3330 612d 3864 3030 2d31 3165 642d 6161  30a-8d00-11ed-aa
+000053e0: 3161 2d64 3334 6136 3135 3531 3532 645f  1a-d34a6155152d_
+000053f0: 3122 0a20 2020 2020 2020 2029 0a20 2020  1".        ).   
+00005400: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+00005410: 5b33 2e33 2e39 5d20 4765 7420 7061 7265  [3.3.9] Get pare
+00005420: 6e74 206f 6620 7468 6520 6576 656e 742e  nt of the event.
+00005430: 0a20 2020 2020 2020 2070 6172 656e 7420  .        parent 
+00005440: 3d20 6574 632e 6765 745f 7061 7265 6e74  = etc.get_parent
+00005450: 280a 2020 2020 2020 2020 2020 2020 2264  (.            "d
+00005460: 656d 6f5f 626f 6f6b 5f31 3a74 6832 2d73  emo_book_1:th2-s
+00005470: 636f 7065 3a32 3032 3330 3130 3531 3335  cope:20230105135
+00005480: 3730 3535 3630 3837 3330 3030 3a64 3631  705560873000:d61
+00005490: 6539 3330 612d 3864 3030 2d31 3165 642d  e930a-8d00-11ed-
+000054a0: 6161 3161 2d64 3334 6136 3135 3531 3532  aa1a-d34a6155152
+000054b0: 645f 3122 0a20 2020 2020 2020 2029 0a20  d_1".        ). 
+000054c0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000054d0: 2320 5b33 2e33 2e31 305d 2041 7070 656e  # [3.3.10] Appen
+000054e0: 6420 6e65 7720 6576 656e 7420 746f 2074  d new event to t
+000054f0: 6865 2063 6f6c 6c65 6374 696f 6e2e 0a20  he collection.. 
+00005500: 2020 2020 2020 2065 7463 2e61 7070 656e         etc.appen
+00005510: 645f 6576 656e 7428 0a20 2020 2020 2020  d_event(.       
+00005520: 2020 2020 2065 7665 6e74 3d7b 0a20 2020       event={.   
+00005530: 2020 2020 2020 2020 2020 2020 2022 6576               "ev
+00005540: 656e 7449 6422 3a20 2261 3230 6635 6566  entId": "a20f5ef
+00005550: 342d 6333 6665 2d62 6231 302d 6132 3963  4-c3fe-bb10-a29c
+00005560: 2d64 6433 6437 3834 3930 3965 6222 2c0a  -dd3d784909eb",.
+00005570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005580: 2270 6172 656e 7445 7665 6e74 4964 223a  "parentEventId":
+00005590: 2022 3865 3235 3234 6661 2d63 6635 392d   "8e2524fa-cf59-
+000055a0: 3131 6562 2d61 3366 372d 3039 3466 3930  11eb-a3f7-094f90
+000055b0: 3463 3361 3632 222c 0a20 2020 2020 2020  4c3a62",.       
+000055c0: 2020 2020 2020 2020 2022 6576 656e 744e           "eventN
+000055d0: 616d 6522 3a20 2253 7475 6245 7665 6e74  ame": "StubEvent
+000055e0: 222c 0a20 2020 2020 2020 2020 2020 207d  ",.            }
+000055f0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00005600: 2020 200a 2020 2020 2020 2020 2320 5b33     .        # [3
+00005610: 2e33 2e31 315d 2053 686f 7720 7468 6520  .3.11] Show the 
+00005620: 656e 7469 7265 2063 6f6c 6c65 6374 696f  entire collectio
+00005630: 6e2e 0a20 2020 2020 2020 2065 7463 2e73  n..        etc.s
+00005640: 686f 7728 290a 2020 2020 2020 2020 2320  how().        # 
+00005650: 4974 276c 6c20 7072 696e 7420 7468 6520  It'll print the 
+00005660: 666f 6c6c 6f77 696e 673a 0a20 2020 2020  following:.     
+00005670: 2020 2023 2053 6574 206f 6620 6175 746f     # Set of auto
+00005680: 2d67 656e 6572 6174 6564 2065 7665 6e74  -generated event
+00005690: 7320 666f 7220 6473 206c 6962 2074 6573  s for ds lib tes
+000056a0: 7469 6e67 0a20 2020 2020 2020 2023 20e2  ting.        # .
+000056b0: 949c e294 80e2 9480 2050 6c61 696e 2065  ........ Plain e
+000056c0: 7665 6e74 2031 0a20 2020 2020 2020 2023  vent 1.        #
+000056d0: 20e2 9494 e294 80e2 9480 2050 6c61 696e   ......... Plain
+000056e0: 2065 7665 6e74 2032 0a20 2020 2020 2020   event 2.       
+000056f0: 200a 2020 2020 2020 2020 2320 4173 2079   .        # As y
+00005700: 6f75 2063 616e 2073 6565 2c20 6e6f 7468  ou can see, noth
+00005710: 696e 6720 7761 7320 6368 616e 6765 642c  ing was changed,
+00005720: 2062 7574 2077 6520 6164 6465 6420 7468   but we added th
+00005730: 6520 6e65 7720 6576 656e 7421 0a20 2020  e new event!.   
+00005740: 2020 2020 2023 206c 6574 2773 206c 6f6f       # let's loo
+00005750: 6b20 6174 2074 6865 2073 756d 6d61 7279  k at the summary
+00005760: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00005770: 2020 2070 7269 6e74 2865 7463 2e73 756d     print(etc.sum
+00005780: 6d61 7279 2829 2920 2023 2074 6865 2073  mary())  # the s
+00005790: 616d 6520 6173 206a 7573 7420 7072 696e  ame as just prin
+000057a0: 7428 6574 6329 0a20 2020 2020 2020 2023  t(etc).        #
+000057b0: 2045 7665 6e74 5472 6565 436f 6c6c 6563   EventTreeCollec
+000057c0: 7469 6f6e 2874 7265 6573 3d31 2c20 6576  tion(trees=1, ev
+000057d0: 656e 7473 3d35 5b74 7265 6573 3d33 2c20  ents=5[trees=3, 
+000057e0: 6465 7461 6368 6564 3d32 5d29 0a20 2020  detached=2]).   
+000057f0: 2020 2020 2023 2059 6f75 2063 616e 2073       # You can s
+00005800: 6565 2074 6861 7420 6974 2077 6173 2061  ee that it was a
+00005810: 6464 6564 2074 6f20 6465 7461 6368 6564  dded to detached
+00005820: 2e20 5468 6174 2773 2077 6879 2079 6f75  . That's why you
+00005830: 2064 6f6e 2774 2073 6565 2074 6865 2065   don't see the e
+00005840: 7665 6e74 0a20 2020 2020 2020 2023 2076  vent.        # v
+00005850: 6961 2060 7368 6f77 2829 602e 2060 7368  ia `show()`. `sh
+00005860: 6f77 2829 6020 7072 696e 7473 206f 6e6c  ow()` prints onl
+00005870: 7920 5472 6565 7321 0a20 2020 2020 2020  y Trees!.       
+00005880: 2023 2055 7365 2060 6574 632e 6765 745f   # Use `etc.get_
+00005890: 7061 7265 6e74 6c65 7373 5f74 7265 6573  parentless_trees
+000058a0: 2829 6020 746f 2063 6f6e 7665 7274 2064  ()` to convert d
+000058b0: 6574 6163 6865 6420 6576 656e 7473 2074  etached events t
+000058c0: 6f20 7472 6565 732e 0a20 2020 2020 2020  o trees..       
+000058d0: 2023 204d 6f72 6520 696e 666f 726d 6174   # More informat
+000058e0: 696f 6e20 6265 6c6f 7720 696e 2074 6865  ion below in the
+000058f0: 2063 6f72 7265 7370 6f6e 6469 6e67 2073   corresponding s
+00005900: 6563 7469 6f6e 2e0a 2020 2020 2020 2020  ection..        
+00005910: 0a20 2020 2020 2020 2023 202d 2d2d 2d2d  .        # -----
+00005920: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00005930: 2020 2320 5b33 2e34 5d20 576f 726b 696e    # [3.4] Workin
+00005940: 6720 7769 7468 2074 6865 2045 7665 6e74  g with the Event
+00005950: 5472 6565 2e0a 2020 2020 2020 2020 2320  Tree..        # 
+00005960: 4576 656e 7454 7265 6520 6861 7320 7468  EventTree has th
+00005970: 6520 7361 6d65 206d 6574 686f 6473 2061  e same methods a
+00005980: 7320 4576 656e 7454 7265 6543 6f6c 6c65  s EventTreeColle
+00005990: 6374 696f 6e2c 2062 7574 206f 6e6c 7920  ction, but only 
+000059a0: 666f 7220 6974 7320 6f77 6e20 7472 6565  for its own tree
+000059b0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+000059c0: 2020 2023 205b 332e 342e 315d 2047 6574     # [3.4.1] Get
+000059d0: 2061 2063 6f6c 6c65 6374 696f 6e20 6f66   a collection of
+000059e0: 2074 7265 6573 2e0a 2020 2020 2020 2020   trees..        
+000059f0: 7472 6565 733a 204c 6973 745b 4576 656e  trees: List[Even
+00005a00: 7454 7265 655d 203d 2065 7463 2e67 6574  tTree] = etc.get
+00005a10: 5f74 7265 6573 2829 0a20 2020 2020 2020  _trees().       
+00005a20: 2074 7265 653a 2045 7665 6e74 5472 6565   tree: EventTree
+00005a30: 203d 2074 7265 6573 5b30 5d0a 2020 2020   = trees[0].    
+00005a40: 2020 2020 0a20 2020 2020 2020 2023 2042      .        # B
+00005a50: 7574 2045 7665 6e74 5472 6565 2070 726f  ut EventTree pro
+00005a60: 7669 6465 7320 6120 776f 726b 2077 6974  vides a work wit
+00005a70: 6820 7468 6520 7472 6565 2c20 6275 7420  h the tree, but 
+00005a80: 646f 6573 206e 6f74 206d 6f64 6966 7920  does not modify 
+00005a90: 6974 2e0a 2020 2020 2020 2020 2320 4966  it..        # If
+00005aa0: 2079 6f75 2077 616e 7420 746f 206d 6f64   you want to mod
+00005ab0: 6966 7920 7468 6520 7472 6565 2c20 7573  ify the tree, us
+00005ac0: 6520 4576 656e 7454 7265 6543 6f6c 6c65  e EventTreeColle
+00005ad0: 6374 696f 6e73 2e0a 2020 2020 2020 2020  ctions..        
+00005ae0: 0a20 2020 2020 2020 2023 205b 332e 355d  .        # [3.5]
+00005af0: 2057 6f72 6b69 6e67 2077 6974 6820 5061   Working with Pa
+00005b00: 7265 6e74 6c65 7373 5472 6565 2e0a 2020  rentlessTree..  
+00005b10: 2020 2020 2020 2320 5061 7265 6e74 6c65        # Parentle
+00005b20: 7373 5472 6565 2069 7320 616e 2045 7665  ssTree is an Eve
+00005b30: 6e74 5472 6565 2074 6861 7420 6861 7320  ntTree that has 
+00005b40: 6465 7461 6368 6564 2065 7665 6e74 7320  detached events 
+00005b50: 7769 7468 2073 7475 6273 2e0a 2020 2020  with stubs..    
+00005b60: 2020 2020 7061 7265 6e74 6c65 7373 5f74      parentless_t
+00005b70: 7265 6573 3a20 4c69 7374 5b45 7665 6e74  rees: List[Event
+00005b80: 5472 6565 5d20 3d20 6574 632e 6765 745f  Tree] = etc.get_
+00005b90: 7061 7265 6e74 6c65 7373 5f74 7265 6573  parentless_trees
+00005ba0: 2829 0a20 2020 2020 2020 2070 7269 6e74  ().        print
+00005bb0: 2822 7061 7265 6e74 6c65 7373 5f74 7265  ("parentless_tre
+00005bc0: 6573 2063 6f6e 7461 696e 733a 2229 0a20  es contains:"). 
+00005bd0: 2020 2020 2020 2070 7269 6e74 2870 6172         print(par
+00005be0: 656e 746c 6573 735f 7472 6565 7329 0a20  entless_trees). 
+00005bf0: 2020 2020 2020 2023 205b 4576 656e 7454         # [EventT
+00005c00: 7265 6528 6e61 6d65 3d27 3c42 726f 6b65  ree(name='<Broke
+00005c10: 6e45 7665 6e74 3e27 2c20 726f 6f74 5f69  nEvent>', root_i
+00005c20: 643d 276e 6f74 5f65 7869 7374 735f 696e  d='not_exists_in
+00005c30: 5f74 6865 5f65 7665 6e74 735f 7374 7265  _the_events_stre
+00005c40: 616d 272c 2065 7665 6e74 733d 3229 2c0a  am', events=2),.
+00005c50: 2020 2020 2020 2020 2320 2045 7665 6e74          #  Event
+00005c60: 5472 6565 286e 616d 653d 273c 4272 6f6b  Tree(name='<Brok
+00005c70: 656e 4576 656e 743e 272c 2072 6f6f 745f  enEvent>', root_
+00005c80: 6964 3d27 3865 3235 3234 6661 2d63 6635  id='8e2524fa-cf5
+00005c90: 392d 3131 6562 2d61 3366 372d 3039 3466  9-11eb-a3f7-094f
+00005ca0: 3930 3463 3361 3632 272c 2065 7665 6e74  904c3a62', event
+00005cb0: 733d 3229 5d0a 2020 2020 2020 2020 0a20  s=2)].        . 
+00005cc0: 2020 2020 2020 2070 7269 6e74 2822 5c6e         print("\n
+00005cd0: 2220 2265 7463 2061 6674 6572 2060 6765  " "etc after `ge
+00005ce0: 745f 7061 7265 6e74 6c65 7373 5f74 7265  t_parentless_tre
+00005cf0: 6573 603a 2229 0a20 2020 2020 2020 2070  es`:").        p
+00005d00: 7269 6e74 2865 7463 2e73 756d 6d61 7279  rint(etc.summary
+00005d10: 2829 290a 2020 2020 2020 2020 2320 4576  ()).        # Ev
+00005d20: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
+00005d30: 6e28 7472 6565 733d 335b 7265 6775 6c61  n(trees=3[regula
+00005d40: 723d 312c 2070 6172 656e 746c 6573 733d  r=1, parentless=
+00005d50: 325d 2c20 6576 656e 7473 3d37 5b74 7265  2], events=7[tre
+00005d60: 6573 3d37 2c20 6465 7461 6368 6564 3d30  es=7, detached=0
+00005d70: 5d29 270a 2020 2020 2020 2020 6574 632e  ])'.        etc.
+00005d80: 7368 6f77 2829 0a20 2020 2020 2020 2023  show().        #
+00005d90: 2053 6574 206f 6620 6175 746f 2d67 656e   Set of auto-gen
+00005da0: 6572 6174 6564 2065 7665 6e74 7320 666f  erated events fo
+00005db0: 7220 6473 206c 6962 2074 6573 7469 6e67  r ds lib testing
+00005dc0: 0a20 2020 2020 2020 2023 20e2 949c e294  .        # .....
+00005dd0: 80e2 9480 2050 6c61 696e 2065 7665 6e74  .... Plain event
+00005de0: 2031 0a20 2020 2020 2020 2023 20e2 9494   1.        # ...
+00005df0: e294 80e2 9480 2050 6c61 696e 2065 7665  ...... Plain eve
+00005e00: 6e74 2032 0a20 2020 2020 2020 2023 203c  nt 2.        # <
+00005e10: 4272 6f6b 656e 4576 656e 743e 0a20 2020  BrokenEvent>.   
+00005e20: 2020 2020 2023 20e2 9494 e294 80e2 9480       # .........
+00005e30: 2046 616b 6520 6576 656e 740a 2020 2020   Fake event.    
+00005e40: 2020 2020 2320 3c42 726f 6b65 6e45 7665      # <BrokenEve
+00005e50: 6e74 3e0a 2020 2020 2020 2020 2320 e294  nt>.        # ..
+00005e60: 94e2 9480 e294 8020 5374 7562 4576 656e  ....... StubEven
+00005e70: 7420 2020 203c 2d2d 2d20 7468 6520 6576  t    <--- the ev
+00005e80: 656e 7420 7468 6174 2077 6173 2061 6464  ent that was add
+00005e90: 6564 2061 626f 7665 0a20 2020 2020 2020  ed above.       
+00005ea0: 200a 2020 2020 2020 2020 2320 5b33 2e36   .        # [3.6
+00005eb0: 5d20 576f 726b 696e 6720 7769 7468 2050  ] Working with P
+00005ec0: 6172 656e 7445 7665 6e74 5472 6565 436f  arentEventTreeCo
+00005ed0: 6c6c 6563 7469 6f6e 2e0a 2020 2020 2020  llection..      
+00005ee0: 2020 2320 5061 7265 6e74 4576 656e 7454    # ParentEventT
+00005ef0: 7265 6543 6f6c 6c65 6374 696f 6e20 6973  reeCollection is
+00005f00: 2061 2074 7265 6520 636f 6c6c 6563 7469   a tree collecti
+00005f10: 6f6e 206c 696b 6520 4576 656e 7454 7265  on like EventTre
+00005f20: 6543 6f6c 6c65 6374 696f 6e2c 0a20 2020  eCollection,.   
+00005f30: 2020 2020 2023 2062 7574 2069 7420 6861       # but it ha
+00005f40: 7320 6f6e 6c79 2065 7665 6e74 7320 7468  s only events th
+00005f50: 6174 2068 6176 6520 7265 6665 7265 6e63  at have referenc
+00005f60: 6573 2e0a 2020 2020 2020 2020 6461 7461  es..        data
+00005f70: 5f73 6f75 7263 653a 2049 4461 7461 536f  _source: IDataSo
+00005f80: 7572 6365 2020 2320 596f 7520 7368 6f75  urce  # You shou
+00005f90: 6c64 2069 6e69 7420 4461 7461 536f 7572  ld init DataSour
+00005fa0: 6365 206f 626a 6563 742e 2045 2e67 2e20  ce object. E.g. 
+00005fb0: 6672 6f6d 204c 7744 5020 6d6f 6475 6c65  from LwDP module
+00005fc0: 2e0a 2020 2020 2020 2020 6461 7461 5f73  ..        data_s
+00005fd0: 6f75 7263 6520 3d20 4475 6d6d 7944 6174  ource = DummyDat
+00005fe0: 6153 6f75 7263 6528 2920 2023 204e 6f74  aSource()  # Not
+00005ff0: 6521 2057 6520 7573 6520 6661 6b65 2044  e! We use fake D
+00006000: 5320 6865 7265 2e0a 2020 2020 2020 2020  S here..        
+00006010: 2320 4554 4344 7269 7665 7220 6865 7265  # ETCDriver here
+00006020: 2069 7320 6120 7374 7562 2c20 6163 7475   is a stub, actu
+00006030: 616c 6c79 2074 6865 206c 6962 2064 6f65  ally the lib doe
+00006040: 736e 2774 2068 6176 6520 7375 6368 2061  sn't have such a
+00006050: 2063 6c61 7373 2e0a 2020 2020 2020 2020   class..        
+00006060: 2320 596f 7520 6361 6e20 7461 6b65 2069  # You can take i
+00006070: 7420 696e 204c 7744 5020 6d6f 6475 6c65  t in LwDP module
+00006080: 206f 7220 6372 6561 7465 2079 6f75 7273   or create yours
+00006090: 656c 6620 636c 6173 7320 6966 2079 6f75  elf class if you
+000060a0: 2068 6176 6520 736f 6d65 2073 7065 6369   have some speci
+000060b0: 616c 2065 7665 6e74 7320 7374 7275 6374  al events struct
+000060c0: 7572 652e 0a20 2020 2020 2020 2066 726f  ure..        fro
+000060d0: 6d20 7468 325f 6461 7461 5f73 6572 7669  m th2_data_servi
+000060e0: 6365 732e 6461 7461 5f73 6f75 7263 652e  ces.data_source.
+000060f0: 6c77 6470 2e65 7665 6e74 5f74 7265 6520  lwdp.event_tree 
+00006100: 696d 706f 7274 2048 7474 7045 5443 4472  import HttpETCDr
+00006110: 6976 6572 2061 7320 4554 4344 7269 7665  iver as ETCDrive
+00006120: 720a 2020 2020 2020 2020 0a20 2020 2020  r.        .     
+00006130: 2020 2064 7269 7665 7220 3d20 4554 4344     driver = ETCD
+00006140: 7269 7665 7228 6461 7461 5f73 6f75 7263  river(data_sourc
+00006150: 653d 6461 7461 5f73 6f75 7263 6529 0a20  e=data_source). 
+00006160: 2020 2020 2020 2070 6574 6320 3d20 5061         petc = Pa
+00006170: 7265 6e74 4576 656e 7454 7265 6543 6f6c  rentEventTreeCol
+00006180: 6c65 6374 696f 6e28 6472 6976 6572 290a  lection(driver).
+00006190: 2020 2020 2020 2020 7065 7463 2e62 7569          petc.bui
+000061a0: 6c64 2865 7665 6e74 7329 0a20 2020 2020  ld(events).     
+000061b0: 2020 200a 2020 2020 2020 2020 7065 7463     .        petc
+000061c0: 2e73 686f 7728 290a 2020 2020 2020 2020  .show().        
+000061d0: 7065 7463 2e73 756d 6d61 7279 2829 0a20  petc.summary(). 
+000061e0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000061f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006200: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006210: 2323 2323 2323 0a20 2020 2020 2020 2023  ######.        #
+00006220: 205b 345d 2046 6965 6c64 2052 6573 6f6c   [4] Field Resol
+00006230: 7665 7273 0a20 2020 2020 2020 2023 2323  vers.        ###
+00006240: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006250: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006260: 2323 230a 2020 2020 2020 2020 2320 506c  ###.        # Pl
+00006270: 6561 7365 2072 6561 6420 6046 6965 6c64  ease read `Field
+00006280: 2052 6573 6f6c 7665 7273 6020 626c 6f63   Resolvers` bloc
+00006290: 6b20 696e 2072 6561 646d 6520 6669 7273  k in readme firs
+000062a0: 742e 0a20 2020 2020 2020 200a 2020 2020  t..        .    
+000062b0: 2020 2020 2320 5b34 2e31 5d20 5573 6167      # [4.1] Usag
+000062c0: 6520 6578 616d 706c 6520 6672 6f6d 2063  e example from c
+000062d0: 6c69 656e 7420 636f 6465 0a20 2020 2020  lient code.     
+000062e0: 2020 2066 726f 6d20 7468 325f 6461 7461     from th2_data
+000062f0: 5f73 6572 7669 6365 732e 6461 7461 5f73  _services.data_s
+00006300: 6f75 7263 6520 696d 706f 7274 2028 0a20  ource import (. 
+00006310: 2020 2020 2020 2020 2020 206c 7764 702c             lwdp,
+00006320: 0a20 2020 2020 2020 2029 2020 2320 6c77  .        )  # lw
+00006330: 6470 2064 6174 615f 736f 7572 6365 2069  dp data_source i
+00006340: 6e69 7469 616c 697a 6520 7468 325f 6461  nitialize th2_da
+00006350: 7461 5f73 6572 7669 6365 732e 636f 6e66  ta_services.conf
+00006360: 6967 2064 7572 696e 6720 696d 706f 7274  ig during import
+00006370: 2e0a 2020 2020 2020 2020 6672 6f6d 2074  ..        from t
+00006380: 6832 5f64 6174 615f 7365 7276 6963 6573  h2_data_services
+00006390: 2e63 6f6e 6669 6720 696d 706f 7274 206f  .config import o
+000063a0: 7074 696f 6e73 2061 7320 6f5f 0a20 2020  ptions as o_.   
+000063b0: 2020 2020 2066 726f 6d20 7468 325f 6461       from th2_da
+000063c0: 7461 5f73 6572 7669 6365 732e 6461 7461  ta_services.data
+000063d0: 5f73 6f75 7263 652e 6c77 6470 2e73 7475  _source.lwdp.stu
+000063e0: 625f 6275 696c 6465 7220 696d 706f 7274  b_builder import
+000063f0: 2068 7474 705f 6d65 7373 6167 655f 7374   http_message_st
+00006400: 7562 5f62 7569 6c64 6572 0a20 2020 2020  ub_builder.     
+00006410: 2020 200a 2020 2020 2020 2020 6661 6b65     .        fake
+00006420: 5f64 6174 6120 3d20 5b0a 2020 2020 2020  _data = [.      
+00006430: 2020 2020 2020 6874 7470 5f6d 6573 7361        http_messa
+00006440: 6765 5f73 7475 625f 6275 696c 6465 722e  ge_stub_builder.
+00006450: 6275 696c 6428 7b22 6d65 7373 6167 6549  build({"messageI
+00006460: 6422 3a20 2261 222c 2022 6d65 7373 6167  d": "a", "messag
+00006470: 6554 7970 6522 3a20 2252 6f6f 7422 7d29  eType": "Root"})
+00006480: 2c0a 2020 2020 2020 2020 2020 2020 6874  ,.            ht
+00006490: 7470 5f6d 6573 7361 6765 5f73 7475 625f  tp_message_stub_
+000064a0: 6275 696c 6465 722e 6275 696c 6428 7b22  builder.build({"
+000064b0: 6d65 7373 6167 6549 6422 3a20 2262 222c  messageId": "b",
+000064c0: 2022 6d65 7373 6167 6554 7970 6522 3a20   "messageType": 
+000064d0: 224e 6577 227d 292c 0a20 2020 2020 2020  "New"}),.       
+000064e0: 2020 2020 2068 7474 705f 6d65 7373 6167       http_messag
+000064f0: 655f 7374 7562 5f62 7569 6c64 6572 2e62  e_stub_builder.b
+00006500: 7569 6c64 287b 226d 6573 7361 6765 4964  uild({"messageId
+00006510: 223a 2022 6322 2c20 226d 6573 7361 6765  ": "c", "message
+00006520: 5479 7065 223a 2022 416d 656e 6422 7d29  Type": "Amend"})
+00006530: 2c0a 2020 2020 2020 2020 2020 2020 6874  ,.            ht
+00006540: 7470 5f6d 6573 7361 6765 5f73 7475 625f  tp_message_stub_
+00006550: 6275 696c 6465 722e 6275 696c 6428 7b22  builder.build({"
+00006560: 6d65 7373 6167 6549 6422 3a20 2264 222c  messageId": "d",
+00006570: 2022 6d65 7373 6167 6554 7970 6522 3a20   "messageType": 
+00006580: 2243 616e 6365 6c22 7d29 2c0a 2020 2020  "Cancel"}),.    
+00006590: 2020 2020 5d0a 2020 2020 2020 2020 6661      ].        fa
+000065a0: 6b65 5f64 6174 615f 6f62 6a20 3d20 4461  ke_data_obj = Da
+000065b0: 7461 2866 616b 655f 6461 7461 290a 2020  ta(fake_data).  
+000065c0: 2020 2020 2020 0a20 2020 2020 2020 2066        .        f
+000065d0: 6f72 206d 2069 6e20 6661 6b65 5f64 6174  or m in fake_dat
+000065e0: 615f 6f62 6a3a 0a20 2020 2020 2020 2020  a_obj:.         
+000065f0: 2020 206f 5f2e 6d66 722e 6578 7061 6e64     o_.mfr.expand
+00006600: 5f6d 6573 7361 6765 286d 2920 2023 206d  _message(m)  # m
+00006610: 6672 202d 2073 7461 6e64 7320 666f 7220  fr - stands for 
+00006620: 4d65 7373 6167 6546 6965 6c64 5265 736f  MessageFieldReso
+00006630: 6c76 6572 0a20 2020 2020 2020 2023 206f  lver.        # o
+00006640: 720a 2020 2020 2020 2020 666f 7220 6d20  r.        for m 
+00006650: 696e 2066 616b 655f 6461 7461 5f6f 626a  in fake_data_obj
+00006660: 2e6d 6170 286f 5f2e 6d66 722e 6578 7061  .map(o_.mfr.expa
+00006670: 6e64 5f6d 6573 7361 6765 293a 0a20 2020  nd_message):.   
+00006680: 2020 2020 2020 2020 2070 6173 730a 2020           pass.  
+00006690: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+000066a0: 205b 342e 325d 204c 6962 7261 7269 6573   [4.2] Libraries
+000066b0: 2075 7361 6765 2e0a 2020 2020 2020 2020   usage..        
+000066c0: 2320 446f 6e27 7420 696d 706f 7274 2065  # Don't import e
+000066d0: 7861 6374 2072 6573 6f6c 7665 7273 2069  xact resolvers i
+000066e0: 6d70 6c65 6d65 6e74 6174 696f 6e20 696e  mplementation in
+000066f0: 2079 6f75 7220 636f 6465 2c20 706c 6561   your code, plea
+00006700: 7365 2e0a 2020 2020 2020 2020 2320 416c  se..        # Al
+00006710: 6c6f 7720 796f 7572 2063 6c69 656e 7420  low your client 
+00006720: 746f 2064 6f20 6974 2069 6e73 7465 6164  to do it instead
+00006730: 2e0a 2020 2020 2020 2020 2320 4a75 7374  ..        # Just
+00006740: 2069 6d70 6f72 7420 606f 7074 696f 6e73   import `options
+00006750: 6020 6672 6f6d 2060 7468 325f 6461 7461  ` from `th2_data
+00006760: 5f73 6572 7669 6365 732e 636f 6e66 6967  _services.config
+00006770: 6020 616e 6420 7573 6520 6974 2e0a 2020  ` and use it..  
+00006780: 2020 2020 2020 6672 6f6d 2074 6832 5f64        from th2_d
+00006790: 6174 615f 7365 7276 6963 6573 2e63 6f6e  ata_services.con
+000067a0: 6669 6720 696d 706f 7274 206f 7074 696f  fig import optio
+000067b0: 6e73 2061 7320 6f5f 0a20 2020 2020 2020  ns as o_.       
+000067c0: 200a 2020 2020 2020 2020 666f 7220 6d20   .        for m 
+000067d0: 696e 2066 616b 655f 6461 7461 5f6f 626a  in fake_data_obj
+000067e0: 3a0a 2020 2020 2020 2020 2020 2020 6f5f  :.            o_
+000067f0: 2e6d 6672 2e65 7870 616e 645f 6d65 7373  .mfr.expand_mess
+00006800: 6167 6528 6d29 0a20 2020 2020 2020 2023  age(m).        #
+00006810: 206f 720a 2020 2020 2020 2020 666f 7220   or.        for 
+00006820: 6d20 696e 2066 616b 655f 6461 7461 5f6f  m in fake_data_o
+00006830: 626a 2e6d 6170 286f 5f2e 6d66 722e 6578  bj.map(o_.mfr.ex
+00006840: 7061 6e64 5f6d 6573 7361 6765 293a 0a20  pand_message):. 
+00006850: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
 00006860: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00006870: 2049 6e20 636f 6e74 7261 7374 2074 6f20   In contrast to 
-00006880: 636f 6c6c 6563 7469 6f6e 732c 2077 6869  collections, whi
-00006890: 6368 2061 7265 2069 7465 7261 7465 6420  ch are iterated 
-000068a0: 6578 706c 6963 6974 6c79 2028 6578 7465  explicitly (exte
-000068b0: 726e 616c 2069 7465 7261 7469 6f6e 292c  rnal iteration),
-000068c0: 2073 7472 6561 6d20 6f70 6572 6174 696f   stream operatio
-000068d0: 6e73 2064 6f20 7468 6520 6974 6572 6174  ns do the iterat
-000068e0: 696f 6e0a 2020 2020 2020 2020 6265 6869  ion.        behi
-000068f0: 6e64 2074 6865 2073 6365 6e65 7320 666f  nd the scenes fo
-00006900: 7220 796f 752e 204e 6f74 652c 2069 7420  r you. Note, it 
-00006910: 646f 6573 6e27 7420 6d65 616e 2079 6f75  doesn't mean you
-00006920: 2063 616e 6e6f 7420 6974 6572 6174 6520   cannot iterate 
-00006930: 7468 6520 5f44 6174 6120 6f62 6a65 6374  the _Data object
-00006940: 5f2e 0a20 2020 2020 2020 200a 2020 2020  _..        .    
-00006950: 2020 2020 0a20 2020 2020 2020 2023 2323      .        ###
-00006960: 2044 6174 6120 6974 6572 6174 696f 6e0a   Data iteration.
-00006970: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00006980: 2054 6865 2044 6174 6120 6f62 6a65 6374   The Data object
-00006990: 2063 6f6e 7374 7275 6374 6f72 206d 6574   constructor met
-000069a0: 686f 6420 7461 6b65 7320 696e 2061 7320  hod takes in as 
-000069b0: 6172 6775 6d65 6e74 2065 6974 6865 7220  argument either 
-000069c0: 616e 2069 7465 7261 746f 7220 6f76 6572  an iterator over
-000069d0: 206f 626a 6563 7473 206f 7220 6120 6765   objects or a ge
-000069e0: 6e65 7261 746f 7220 6675 6e63 7469 6f6e  nerator function
-000069f0: 2e0a 2020 2020 2020 2020 5468 6520 4461  ..        The Da
-00006a00: 7461 206f 626a 6563 7420 6974 6572 6174  ta object iterat
-00006a10: 6f72 2068 616e 646c 6573 2065 6163 6820  or handles each 
-00006a20: 6974 656d 2069 6e20 7468 6973 2069 7465  item in this ite
-00006a30: 7261 746f 7220 6f72 2067 656e 6572 6174  rator or generat
-00006a40: 6f72 2061 7320 7468 6579 2061 7265 2c20  or as they are, 
-00006a50: 6d65 616e 696e 6720 6974 2064 6f65 736e  meaning it doesn
-00006a60: 2774 2074 7279 2074 6f20 7265 6164 2074  't try to read t
-00006a70: 6865 2063 6f6e 7465 6e74 206f 6620 6974  he content of it
-00006a80: 656d 206f 7220 7265 7475 726e 2074 6865  em or return the
-00006a90: 6d20 6d6f 6469 6669 6564 2069 6e20 616e  m modified in an
-00006aa0: 7920 7761 792c 2069 6e73 7465 6164 2072  y way, instead r
-00006ab0: 6574 7572 6e73 2074 6865 2069 7465 6d20  eturns the item 
-00006ac0: 6974 7365 6c66 2e0a 2020 2020 2020 2020  itself..        
-00006ad0: 5468 6520 6f6e 6c79 2065 7863 6570 7469  The only excepti
-00006ae0: 6f6e 2074 6f20 7468 6973 2069 7320 7768  on to this is wh
-00006af0: 656e 2044 6174 6120 6f62 6a65 6374 2069  en Data object i
-00006b00: 7320 6275 696c 7420 7573 696e 6720 6974  s built using it
-00006b10: 6572 6174 6f72 206f 7220 6765 6e65 7261  erator or genera
-00006b20: 746f 7220 6f76 6572 206f 7468 6572 2044  tor over other D
-00006b30: 6174 6120 6f62 6a65 6374 732e 204e 6f74  ata objects. Not
-00006b40: 6520 7468 6174 2074 6869 7320 6974 6572  e that this iter
-00006b50: 6174 6f72 206f 7220 6765 6e65 7261 746f  ator or generato
-00006b60: 7220 6d75 7374 206f 6e6c 7920 6265 2079  r must only be y
-00006b70: 6965 6c64 696e 6720 4461 7461 206f 626a  ielding Data obj
-00006b80: 6563 7473 2061 6e64 206e 6f74 6869 6e67  ects and nothing
-00006b90: 2065 6c73 652e 2049 6620 7765 2062 7569   else. If we bui
-00006ba0: 6c64 2066 726f 6d20 6120 6d69 7820 6f66  ld from a mix of
-00006bb0: 2044 6174 6120 6f62 6a65 6374 7320 616e   Data objects an
-00006bc0: 6420 736f 6d65 206f 7468 6572 2074 7970  d some other typ
-00006bd0: 6573 2c20 4461 7461 206f 626a 6563 7473  es, Data objects
-00006be0: 2720 636f 6e74 656e 7420 776f 6e27 7420  ' content won't 
-00006bf0: 6265 2072 6561 6420 616e 6420 696e 7374  be read and inst
-00006c00: 6561 6420 6974 2077 696c 6c20 6265 2072  ead it will be r
-00006c10: 6574 7572 6e65 6420 6173 2044 6174 6120  eturned as Data 
-00006c20: 6f62 6a65 6374 2069 7473 656c 662e 0a20  object itself.. 
-00006c30: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006c40: 536d 616c 6c20 6578 616d 706c 6520 746f  Small example to
-00006c50: 2064 656d 6f6e 7374 7261 7465 3a0a 2020   demonstrate:.  
-00006c60: 2020 2020 2020 0a20 2020 2020 2020 2060        .        `
-00006c70: 6060 7079 7468 6f6e 0a20 2020 2020 2020  ``python.       
-00006c80: 2066 726f 6d20 7468 325f 6461 7461 5f73   from th2_data_s
-00006c90: 6572 7669 6365 732e 6461 7461 2069 6d70  ervices.data imp
-00006ca0: 6f72 7420 4461 7461 0a20 2020 2020 2020  ort Data.       
-00006cb0: 200a 2020 2020 2020 2020 6431 203d 2044   .        d1 = D
-00006cc0: 6174 6128 5b31 2c32 2c33 5d29 0a20 2020  ata([1,2,3]).   
-00006cd0: 2020 2020 2064 3220 3d20 4461 7461 285b       d2 = Data([
-00006ce0: 342c 352c 365d 290a 2020 2020 2020 2020  4,5,6]).        
-00006cf0: 0a20 2020 2020 2020 206f 6e6c 795f 6461  .        only_da
-00006d00: 7461 5f6f 626a 6563 7473 203d 2044 6174  ta_objects = Dat
-00006d10: 6128 5b64 312c 6432 5d29 2023 2057 696c  a([d1,d2]) # Wil
-00006d20: 6c20 6974 6572 6174 6520 6173 2031 2c32  l iterate as 1,2
-00006d30: 2c33 2c34 2c35 2c36 0a20 2020 2020 2020  ,3,4,5,6.       
-00006d40: 2064 6174 615f 616e 645f 6c69 7374 203d   data_and_list =
-00006d50: 2044 6174 6128 5b64 312c 5b34 2c35 2c36   Data([d1,[4,5,6
-00006d60: 5d5d 2920 2320 5769 6c6c 2069 7465 7261  ]]) # Will itera
-00006d70: 7465 2061 7320 6431 2c20 5b34 2c35 2c36  te as d1, [4,5,6
-00006d80: 5d0a 2020 2020 2020 2020 6461 7461 5f61  ].        data_a
-00006d90: 6e64 5f6e 756d 6265 7273 203d 2044 6174  nd_numbers = Dat
-00006da0: 6128 5b64 312c 342c 352c 365d 2920 2320  a([d1,4,5,6]) # 
-00006db0: 5769 6c6c 2069 7465 7261 7465 2061 7320  Will iterate as 
-00006dc0: 6431 2c34 2c35 2c36 0a20 2020 2020 2020  d1,4,5,6.       
-00006dd0: 206c 6973 7473 5f6f 6e6c 7920 3d20 4461   lists_only = Da
-00006de0: 7461 285b 312c 322c 335d 2c5b 342c 352c  ta([1,2,3],[4,5,
-00006df0: 365d 2920 2320 5769 6c6c 2069 7465 7261  6]) # Will itera
-00006e00: 7465 2061 7320 5b31 2c32 2c33 5d2c 5b34  te as [1,2,3],[4
-00006e10: 2c35 2c36 5d0a 2020 2020 2020 2020 0a20  ,5,6].        . 
-00006e20: 2020 2020 2020 2023 2049 6620 7765 2077         # If we w
-00006e30: 616e 7420 746f 2069 7465 7261 7465 206f  ant to iterate o
-00006e40: 7665 7220 636f 6e74 656e 7420 6f66 206c  ver content of l
-00006e50: 6973 7420 6f66 206c 6973 7473 2c20 7765  ist of lists, we
-00006e60: 2073 686f 756c 6420 6669 7273 7420 6372   should first cr
-00006e70: 6561 7465 2044 6174 6120 6f62 6a65 6374  eate Data object
-00006e80: 7320 6672 6f6d 2074 6865 6d2c 0a20 2020  s from them,.   
-00006e90: 2020 2020 2023 2074 6865 6e20 7573 6520       # then use 
-00006ea0: 7468 656d 2074 6f20 636f 6e73 7472 7563  them to construc
-00006eb0: 7420 6e65 7720 4461 7461 206f 626a 6563  t new Data objec
-00006ec0: 7420 6173 2069 6e20 6361 7365 206f 6620  t as in case of 
-00006ed0: 6431 2061 6e64 2064 322c 2063 7265 6174  d1 and d2, creat
-00006ee0: 696e 6720 276f 6e6c 795f 6461 7461 5f6f  ing 'only_data_o
-00006ef0: 626a 6563 7473 2720 696e 2074 6869 7320  bjects' in this 
-00006f00: 6578 616d 706c 652e 0a20 2020 2020 2020  example..       
-00006f10: 2060 6060 0a20 2020 2020 2020 2020 0a20   ```.         . 
-00006f20: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006f30: 2323 2320 4461 7461 2063 6163 6869 6e67  ### Data caching
-00006f40: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00006f50: 2020 5468 6520 5f44 6174 6120 6f62 6a65    The _Data obje
-00006f60: 6374 5f20 7072 6f76 6964 6573 2074 6865  ct_ provides the
-00006f70: 2061 6269 6c69 7479 2074 6f20 7573 6520   ability to use 
-00006f80: 7468 6520 6361 6368 652e 2054 6865 2063  the cache. The c
-00006f90: 6163 6865 2077 6f72 6b73 2066 6f72 2065  ache works for e
-00006fa0: 6163 6820 5f44 6174 6120 6f62 6a65 6374  ach _Data object
-00006fb0: 5f2c 2074 6861 7420 6973 2c20 796f 7520  _, that is, you 
-00006fc0: 6368 6f6f 7365 0a20 2020 2020 2020 2077  choose.        w
-00006fd0: 6869 6368 205f 4461 7461 206f 626a 6563  hich _Data objec
-00006fe0: 745f 2079 6f75 2077 616e 7420 746f 2073  t_ you want to s
-00006ff0: 6176 652e 2054 6865 205f 4461 7461 206f  ave. The _Data o
-00007000: 626a 6563 745f 2063 6163 6865 2069 7320  bject_ cache is 
-00007010: 7361 7665 6420 6166 7465 7220 7468 6520  saved after the 
-00007020: 6669 7273 7420 6974 6572 6174 696f 6e2c  first iteration,
-00007030: 2062 7574 2074 6865 2069 7465 7261 7469   but the iterati
-00007040: 6f6e 0a20 2020 2020 2020 2073 6f75 7263  on.        sourc
-00007050: 6520 6d61 7920 6265 2064 6966 6665 7265  e may be differe
-00007060: 6e74 2e0a 2020 2020 2020 2020 0a20 2020  nt..        .   
-00007070: 2020 2020 2049 6620 796f 7520 646f 6e27       If you don'
-00007080: 7420 7573 6520 7468 6520 6361 6368 652c  t use the cache,
-00007090: 2079 6f75 7220 736f 7572 6365 2077 696c   your source wil
-000070a0: 6c20 6265 2074 6865 2064 6174 6120 736f  l be the data so
-000070b0: 7572 6365 2079 6f75 2068 6176 6520 696e  urce you have in
-000070c0: 2074 6865 205f 4461 7461 204f 626a 6563   the _Data Objec
-000070d0: 745f 2e20 4275 7420 6966 2079 6f75 2075  t_. But if you u
-000070e0: 7365 2074 6865 2063 6163 6865 2c0a 2020  se the cache,.  
-000070f0: 2020 2020 2020 796f 7572 2073 6f75 7263        your sourc
-00007100: 6520 6361 6e20 6265 2074 6865 2064 6174  e can be the dat
-00007110: 6120 736f 7572 6365 2c20 7468 6520 7061  a source, the pa
-00007120: 7265 6e74 2063 6163 6865 2c20 6f72 206f  rent cache, or o
-00007130: 776e 2063 6163 6865 3a0a 2020 2020 2020  wn cache:.      
-00007140: 2020 0a20 2020 2020 2020 202a 2054 6865    .        * The
-00007150: 2064 6174 6120 736f 7572 6365 3a0a 2020   data source:.  
-00007160: 2020 2020 2020 2020 4966 2074 6865 205f          If the _
-00007170: 4461 7461 204f 626a 6563 745f 2064 6f65  Data Object_ doe
-00007180: 736e 2774 2068 6176 6520 6120 7061 7265  sn't have a pare
-00007190: 6e74 2063 6163 6865 2061 6e64 2069 7473  nt cache and its
-000071a0: 2063 6163 6865 2e0a 2020 2020 2020 2020   cache..        
-000071b0: 2a20 5468 6520 7061 7265 6e74 2063 6163  * The parent cac
-000071c0: 6865 3a0a 2020 2020 2020 2020 2020 4966  he:.          If
-000071d0: 2074 6865 205f 4461 7461 204f 626a 6563   the _Data Objec
-000071e0: 745f 2068 6173 2061 2070 6172 656e 7420  t_ has a parent 
-000071f0: 6361 6368 652e 2049 7420 646f 6573 6e27  cache. It doesn'
-00007200: 7420 6d61 7474 6572 2077 6861 7420 706f  t matter what po
-00007210: 7369 7469 6f6e 2074 6865 2070 6172 656e  sition the paren
-00007220: 7420 6361 6368 6520 6861 7320 696e 2069  t cache has in i
-00007230: 6e68 6572 6974 616e 6365 2e0a 2020 2020  nheritance..    
-00007240: 2020 2020 2020 5f44 6174 6120 4f62 6a65        _Data Obje
-00007250: 6374 5f20 756e 6465 7273 7461 6e64 7320  ct_ understands 
-00007260: 7768 6f73 6520 6361 6368 6520 6974 2069  whose cache it i
-00007270: 7320 616e 6420 6578 6563 7574 6573 2074  s and executes t
-00007280: 6865 2070 6172 7420 6f66 2074 6865 2077  he part of the w
-00007290: 6f72 6b66 6c6f 7720 7468 6174 2077 6173  orkflow that was
-000072a0: 206e 6f74 2065 7865 6375 7465 642e 0a20   not executed.. 
-000072b0: 2020 2020 2020 202a 2054 6865 206f 776e         * The own
-000072c0: 2063 6163 6865 3a0a 2020 2020 2020 2020   cache:.        
-000072d0: 2020 4966 2069 7420 6973 206e 6f74 2074    If it is not t
-000072e0: 6865 2066 6972 7374 2069 7465 7261 7469  he first iterati
-000072f0: 6f6e 206f 6620 7468 6973 2044 6174 6120  on of this Data 
-00007300: 6f62 6a65 6374 2e0a 2020 2020 2020 2020  object..        
-00007310: 0a20 2020 2020 2020 204e 6f74 6520 7468  .        Note th
-00007320: 6174 2074 6865 2063 6163 6865 2073 7461  at the cache sta
-00007330: 7465 206f 6620 7468 6520 4461 7461 206f  te of the Data o
-00007340: 626a 6563 7420 6973 206e 6f74 2069 6e68  bject is not inh
-00007350: 6572 6974 6564 2e0a 2020 2020 2020 2020  erited..        
-00007360: 0a20 2020 2020 2020 2023 2323 2320 466f  .        #### Fo
-00007370: 7263 6564 2063 6163 6869 6e67 0a20 2020  rced caching.   
-00007380: 2020 2020 2059 6f75 2063 616e 2074 656c       You can tel
-00007390: 6c20 4453 2074 6f20 6361 6368 6520 6461  l DS to cache da
-000073a0: 7461 2074 6f20 7370 6563 6966 6963 2063  ta to specific c
-000073b0: 6163 6865 2066 696c 652c 2077 6869 6368  ache file, which
-000073c0: 2077 6f6e 2774 2062 6520 6465 6c65 7465   won't be delete
-000073d0: 6420 6166 7465 7220 7363 7269 7074 2065  d after script e
-000073e0: 6e64 2e0a 2020 2020 2020 2020 596f 7520  nd..        You 
-000073f0: 6361 6e20 7365 6520 6578 616d 706c 6520  can see example 
-00007400: 696e 2031 2e31 3220 7365 6374 696f 6e20  in 1.12 section 
-00007410: 6f66 205b 6765 745f 7374 6172 7465 645f  of [get_started_
-00007420: 6578 616d 706c 655d 2865 7861 6d70 6c65  example](example
-00007430: 732f 6765 745f 7374 6172 7465 645f 6578  s/get_started_ex
-00007440: 616d 706c 652e 7079 292e 0a20 2020 2020  ample.py)..     
-00007450: 2020 200a 2020 2020 2020 2020 0a20 2020     .        .   
-00007460: 2020 2020 2023 2323 2045 7665 6e74 5472       ### EventTr
-00007470: 6565 2061 6e64 2063 6f6c 6c65 6374 696f  ee and collectio
-00007480: 6e73 0a20 2020 2020 2020 200a 2020 2020  ns.        .    
-00007490: 2020 2020 2323 2323 2045 7665 6e74 5472      #### EventTr
-000074a0: 6565 0a20 2020 2020 2020 200a 2020 2020  ee.        .    
-000074b0: 2020 2020 6045 7665 6e74 5472 6565 6020      `EventTree` 
-000074c0: 6973 2061 2074 7265 652d 6261 7365 6420  is a tree-based 
-000074d0: 6461 7461 2073 7472 7563 7475 7265 206f  data structure o
-000074e0: 6620 6576 656e 7473 2e20 4974 2061 6c6c  f events. It all
-000074f0: 6f77 7320 796f 7520 6765 7420 6368 696c  ows you get chil
-00007500: 6472 656e 2061 6e64 2070 6172 656e 7473  dren and parents
-00007510: 206f 6620 6576 656e 742c 0a20 2020 2020   of event,.     
-00007520: 2020 2064 6973 706c 6179 2074 7265 652c     display tree,
-00007530: 2067 6574 2066 756c 6c20 7061 7468 2074   get full path t
-00007540: 6f20 6576 656e 7420 6574 632e 0a20 2020  o event etc..   
-00007550: 2020 2020 200a 2020 2020 2020 2020 4465       .        De
-00007560: 7461 696c 733a 0a20 2020 2020 2020 200a  tails:.        .
-00007570: 2020 2020 2020 2020 2a20 6045 7665 6e74          * `Event
-00007580: 5472 6565 6020 636f 6e74 6169 6e73 2061  Tree` contains a
-00007590: 6c6c 2065 7665 6e74 7320 696e 206d 656d  ll events in mem
-000075a0: 6f72 792e 0a20 2020 2020 2020 202a 2054  ory..        * T
-000075b0: 7265 6520 6861 7320 736f 6d65 2069 6d70  ree has some imp
-000075c0: 6f72 7461 6e74 2074 6572 6d73 3a0a 2020  ortant terms:.  
-000075d0: 2020 2020 2020 2020 2020 312e 205f 416e            1. _An
-000075e0: 6365 7374 6f72 5f20 6973 2061 6e79 2072  cestor_ is any r
-000075f0: 656c 6174 6976 6520 6f66 2074 6865 2065  elative of the e
-00007600: 7665 6e74 2075 7020 7468 6520 7472 6565  vent up the tree
-00007610: 2028 6772 616e 6470 6172 656e 742c 2070   (grandparent, p
-00007620: 6172 656e 7420 6574 632e 292e 0a20 2020  arent etc.)..   
-00007630: 2020 2020 2020 2020 2032 2e20 5f50 6172           2. _Par
-00007640: 656e 745f 2069 7320 6f6e 6c79 2074 6865  ent_ is only the
-00007650: 2066 6972 7374 2072 656c 6174 6976 6520   first relative 
-00007660: 6f66 2074 6865 2065 7665 6e74 2075 7020  of the event up 
-00007670: 7468 6520 7472 6565 2e0a 2020 2020 2020  the tree..      
-00007680: 2020 2020 2020 332e 205f 4368 696c 645f        3. _Child_
-00007690: 2069 7320 7468 6520 6669 7273 7420 7265   is the first re
-000076a0: 6c61 7469 7665 206f 6620 7468 6520 6576  lative of the ev
-000076b0: 656e 7420 646f 776e 2074 6865 2074 7265  ent down the tre
-000076c0: 652e 0a20 2020 2020 2020 200a 2020 2020  e..        .    
-000076d0: 2020 2020 5461 6b65 2061 206c 6f6f 6b20      Take a look 
-000076e0: 6174 2074 6865 2066 6f6c 6c6f 7769 6e67  at the following
-000076f0: 2048 544d 4c20 7472 6565 2074 6f20 756e   HTML tree to un
-00007700: 6465 7273 7461 6e64 2074 6865 6d2e 0a20  derstand them.. 
-00007710: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00007720: 2020 2060 6060 0a20 2020 2020 2020 2020     ```.         
-00007730: 2020 203c 626f 6479 3e20 3c21 2d2d 2061     <body> <!-- a
-00007740: 6e63 6573 746f 7220 2867 7261 6e64 7061  ncestor (grandpa
-00007750: 7265 6e74 292c 2062 7574 206e 6f74 2070  rent), but not p
-00007760: 6172 656e 7420 2d2d 3e0a 2020 2020 2020  arent -->.      
-00007770: 2020 2020 2020 2020 2020 3c64 6976 3e20            <div> 
-00007780: 3c21 2d2d 2070 6172 656e 7420 2620 616e  <!-- parent & an
-00007790: 6365 7374 6f72 202d 2d3e 0a20 2020 2020  cestor -->.     
-000077a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000077b0: 703e 4865 6c6c 6f2c 2077 6f72 6c64 213c  p>Hello, world!<
-000077c0: 2f70 3e20 3c21 2d2d 2063 6869 6c64 202d  /p> <!-- child -
-000077d0: 2d3e 0a20 2020 2020 2020 2020 2020 2020  ->.             
-000077e0: 2020 2020 2020 203c 703e 476f 6f64 6279         <p>Goodby
-000077f0: 6521 3c2f 703e 203c 212d 2d20 7369 626c  e!</p> <!-- sibl
-00007800: 696e 6720 2d2d 3e0a 2020 2020 2020 2020  ing -->.        
-00007810: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00007820: 2020 2020 2020 2020 2020 203c 2f62 6f64             </bod
-00007830: 793e 0a20 2020 2020 2020 2020 2020 6060  y>.           ``
-00007840: 600a 2020 2020 2020 2020 0a20 2020 2020  `.        .     
-00007850: 2020 2023 2323 2320 436f 6c6c 6563 7469     #### Collecti
-00007860: 6f6e 730a 2020 2020 2020 2020 0a20 2020  ons.        .   
-00007870: 2020 2020 202a 2a45 7665 6e74 5472 6565       **EventTree
-00007880: 436f 6c6c 6563 7469 6f6e 2a2a 2069 7320  Collection** is 
-00007890: 6120 636f 6c6c 6563 7469 6f6e 206f 6620  a collection of 
-000078a0: 4576 656e 7454 7265 6573 2e20 5468 6520  EventTrees. The 
-000078b0: 636f 6c6c 6563 7469 6f6e 2062 7569 6c64  collection build
-000078c0: 7320 6120 6665 7720 5f45 7665 6e74 5472  s a few _EventTr
-000078d0: 6565 5f20 6279 2070 6173 7365 6420 5f44  ee_ by passed _D
-000078e0: 6174 610a 2020 2020 2020 2020 6f62 6a65  ata.        obje
-000078f0: 6374 5f2e 2041 6c74 686f 7567 6820 796f  ct_. Although yo
-00007900: 7520 6361 6e20 6368 616e 6765 2074 6865  u can change the
-00007910: 2074 7265 6520 6469 7265 6374 6c79 2c20   tree directly, 
-00007920: 6974 2773 2062 6574 7465 7220 746f 2064  it's better to d
-00007930: 6f20 6974 2074 6872 6f75 6768 2063 6f6c  o it through col
-00007940: 6c65 6374 696f 6e73 2062 6563 6175 7365  lections because
-00007950: 2074 6865 7920 6172 6520 6177 6172 6520   they are aware 
-00007960: 6f66 0a20 2020 2020 2020 2060 6465 7461  of.        `deta
-00007970: 6368 6564 5f65 7665 6e74 7360 2061 6e64  ched_events` and
-00007980: 2063 616e 2073 6f6c 7665 2073 6f6d 6520   can solve some 
-00007990: 6576 656e 7473 2064 6570 656e 6465 6e63  events dependenc
-000079a0: 6965 732e 2054 6865 2063 6f6c 6c65 6374  ies. The collect
-000079b0: 696f 6e20 6861 7320 7369 6d69 6c61 7220  ion has similar 
-000079c0: 6665 6174 7572 6573 206c 696b 6520 6120  features like a 
-000079d0: 7369 6e67 6c65 205f 4576 656e 7454 7265  single _EventTre
-000079e0: 655f 0a20 2020 2020 2020 2062 7574 2061  e_.        but a
-000079f0: 7070 6c79 696e 6720 7468 656d 2066 6f72  pplying them for
-00007a00: 2061 6c6c 205f 4576 656e 7454 7265 6573   all _EventTrees
-00007a10: 5f2e 0a20 2020 2020 2020 200a 2020 2020  _..        .    
-00007a20: 2020 2020 2a2a 5061 7265 6e74 4576 656e      **ParentEven
-00007a30: 7454 7265 6543 6f6c 6c65 6374 696f 6e2a  tTreeCollection*
-00007a40: 2a20 6973 2061 2063 6f6c 6c65 6374 696f  * is a collectio
-00007a50: 6e20 7369 6d69 6c61 7220 746f 205f 4576  n similar to _Ev
-00007a60: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
-00007a70: 6e5f 2062 7574 2063 6f6e 7461 696e 696e  n_ but containin
-00007a80: 6720 6f6e 6c79 2070 6172 656e 7420 6576  g only parent ev
-00007a90: 656e 7473 2074 6861 740a 2020 2020 2020  ents that.      
-00007aa0: 2020 6172 6520 7265 6665 7265 6e63 6564    are referenced
-00007ab0: 2069 6e20 7468 6520 6461 7461 2073 7472   in the data str
-00007ac0: 6561 6d2e 2054 6865 2063 6f6c 6c65 6374  eam. The collect
-00007ad0: 696f 6e20 6861 7320 6665 6174 7572 6573  ion has features
-00007ae0: 2073 696d 696c 6172 2074 6f20 5f45 7665   similar to _Eve
-00007af0: 6e74 5472 6565 436f 6c6c 6563 7469 6f6e  ntTreeCollection
-00007b00: 5f2e 0a20 2020 2020 2020 200a 2020 2020  _..        .    
-00007b10: 2020 2020 4465 7461 696c 733a 0a20 2020      Details:.   
-00007b20: 2020 2020 200a 2020 2020 2020 2020 2a20       .        * 
-00007b30: 546f 2075 7365 2045 5420 636f 6c6c 6563  To use ET collec
-00007b40: 7469 6f6e 7320 796f 7520 6e65 6564 2074  tions you need t
-00007b50: 6f20 696e 6974 6961 6c69 7a65 2074 6865  o initialize the
-00007b60: 6d20 6279 205f 4554 4344 7269 7665 725f  m by _ETCDriver_
-00007b70: 2e20 4461 7461 2073 6f75 7263 6573 2075  . Data sources u
-00007b80: 7375 616c 6c79 2070 726f 7669 6465 2074  sually provide t
-00007b90: 6865 6d2e 0a20 2020 2020 2020 2020 2059  hem..          Y
-00007ba0: 6f75 2063 616e 2063 7265 6174 6520 6974  ou can create it
-00007bb0: 2062 7920 796f 7572 7365 6c66 2064 6570   by yourself dep
-00007bc0: 656e 6469 6e67 206f 6e20 796f 7572 2064  ending on your d
-00007bd0: 6174 6120 7374 7275 6374 7572 652e 0a20  ata structure.. 
-00007be0: 2020 2020 2020 202a 2054 6865 2063 6f6c         * The col
-00007bf0: 6c65 6374 696f 6e20 6861 7320 6120 6665  lection has a fe
-00007c00: 6174 7572 6520 746f 2072 6563 6f76 6572  ature to recover
-00007c10: 2065 7665 6e74 732e 2041 6c6c 2065 7665   events. All eve
-00007c20: 6e74 7320 7468 6174 2061 7265 206e 6f74  nts that are not
-00007c30: 2069 6e20 7468 6520 7265 6365 6976 6564   in the received
-00007c40: 2064 6174 6120 7374 7265 616d 2c20 6275   data stream, bu
-00007c50: 7420 7768 6963 6820 6172 650a 2020 2020  t which are.    
-00007c60: 2020 2020 2020 7265 6665 7265 6e63 6564        referenced
-00007c70: 2077 696c 6c20 6265 206c 6f61 6465 6420   will be loaded 
-00007c80: 6672 6f6d 2074 6865 2064 6174 6120 736f  from the data so
-00007c90: 7572 6365 2e0a 2020 2020 2020 2020 2a20  urce..        * 
-00007ca0: 596f 7520 6361 6e20 7461 6b65 2060 6465  You can take `de
-00007cb0: 7461 6368 6564 5f65 7665 6e74 7360 2074  tached_events` t
-00007cc0: 6f20 7365 6520 7768 6963 6820 6576 656e  o see which even
-00007cd0: 7473 2061 7265 206d 6973 7369 6e67 2e0a  ts are missing..
-00007ce0: 2020 2020 2020 2020 2a20 4966 2079 6f75          * If you
-00007cf0: 2077 616e 742c 2079 6f75 2063 616e 2062   want, you can b
-00007d00: 7569 6c64 2070 6172 656e 746c 6573 7320  uild parentless 
-00007d10: 7472 6565 7320 7768 6572 6520 7468 6520  trees where the 
-00007d20: 6d69 7373 696e 6720 6576 656e 7473 2061  missing events a
-00007d30: 7265 2073 7475 6262 6564 2069 6e73 7465  re stubbed inste
-00007d40: 6164 2e20 4a75 7374 0a20 2020 2020 2020  ad. Just.       
-00007d50: 2020 2075 7365 2060 6765 745f 7061 7265     use `get_pare
-00007d60: 6e74 6c65 7373 5f74 7265 6573 2829 602e  ntless_trees()`.
-00007d70: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00007d80: 2020 5265 7175 6972 656d 656e 7473 3a0a    Requirements:.
-00007d90: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00007da0: 2031 2e20 4576 656e 7473 2070 726f 7669   1. Events provi
-00007db0: 6465 6420 746f 2045 5443 2068 6176 6520  ded to ETC have 
-00007dc0: 746f 2068 6176 6520 6065 7665 6e74 5f6e  to have `event_n
-00007dd0: 616d 6560 2c20 6065 7665 6e74 5f69 6460  ame`, `event_id`
-00007de0: 2c20 6070 6172 656e 745f 6576 656e 745f  , `parent_event_
-00007df0: 6964 6020 6669 656c 6473 2e20 5468 6579  id` fields. They
-00007e00: 0a20 2020 2020 2020 2063 616e 2068 6176  .        can hav
-00007e10: 6520 616e 6f74 6865 7220 6e61 6d65 7320  e another names 
-00007e20: 2869 7420 7265 736f 6c76 6573 2069 6e20  (it resolves in 
-00007e30: 7468 6520 6472 6976 6572 292e 0a20 2020  the driver)..   
-00007e40: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-00007e50: 2323 2048 696e 7473 0a20 2020 2020 2020  ## Hints.       
-00007e60: 200a 2020 2020 2020 2020 2a20 5265 6d6f   .        * Remo
-00007e70: 7665 2061 6c6c 2075 6e6e 6563 6573 7361  ve all unnecessa
-00007e80: 7279 2066 6965 6c64 7320 6672 6f6d 2065  ry fields from e
-00007e90: 7665 6e74 7320 6265 666f 7265 2070 6173  vents before pas
-00007ea0: 7369 6e67 2074 6f20 6120 5f63 6f6c 6c65  sing to a _colle
-00007eb0: 6374 696f 6e5f 2074 6f20 7265 6475 6365  ction_ to reduce
-00007ec0: 206d 656d 6f72 7920 7573 6167 652e 0a20   memory usage.. 
-00007ed0: 2020 2020 2020 202a 2055 7365 2060 7368         * Use `sh
-00007ee0: 6f77 2829 6020 6d65 7468 6f64 2074 6f20  ow()` method to 
-00007ef0: 7072 696e 7420 7468 6520 7472 6565 2069  print the tree i
-00007f00: 6e20 7472 6565 2d6c 696b 6520 7669 6577  n tree-like view
-00007f10: 2e0a 2020 2020 2020 2020 2a20 4e6f 7465  ..        * Note
-00007f20: 2074 6861 7420 7468 6520 6067 6574 5f78   that the `get_x
-00007f30: 6020 6d65 7468 6f64 7320 7769 6c6c 2072  ` methods will r
-00007f40: 6169 7365 2061 6e20 6578 6365 7074 696f  aise an exceptio
-00007f50: 6e20 6966 2079 6f75 2070 6173 7320 616e  n if you pass an
-00007f60: 2075 6e6b 6e6f 776e 2065 7665 6e74 2069   unknown event i
-00007f70: 642c 2075 6e6c 696b 6520 7468 6520 6066  d, unlike the `f
-00007f80: 696e 645f 7860 206d 6574 686f 6473 2028  ind_x` methods (
-00007f90: 0a20 2020 2020 2020 2020 2074 6865 7920  .          they 
-00007fa0: 7265 7475 726e 204e 6f6e 6529 2e0a 2020  return None)..  
-00007fb0: 2020 2020 2020 2a20 4966 2079 6f75 2077        * If you w
-00007fc0: 616e 7420 746f 206b 6e6f 7720 7468 6174  ant to know that
-00007fd0: 2073 7065 6369 6669 6564 2065 7665 6e74   specified event
-00007fe0: 2065 7869 7374 732c 2075 7365 2074 6865   exists, use the
-00007ff0: 2070 7974 686f 6e20 6069 6e60 206b 6579   python `in` key
-00008000: 776f 7264 2028 652e 672e 2060 2765 7665  word (e.g. `'eve
-00008010: 6e74 2d69 6427 2069 6e20 6576 656e 7473  nt-id' in events
-00008020: 5f74 7265 6560 292e 0a20 2020 2020 2020  _tree`)..       
-00008030: 202a 2055 7365 2074 6865 2070 7974 686f   * Use the pytho
-00008040: 6e20 606c 656e 6020 6b65 7977 6f72 6420  n `len` keyword 
-00008050: 746f 2067 6574 2065 7665 6e74 7320 6e75  to get events nu
-00008060: 6d62 6572 2069 6e20 7468 6520 7472 6565  mber in the tree
-00008070: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00008080: 2020 2023 2323 2046 6965 6c64 2052 6573     ### Field Res
-00008090: 6f6c 7665 7273 0a20 2020 2020 2020 2049  olvers.        I
-000080a0: 6e74 6572 6661 6365 2063 616e 2062 6520  nterface can be 
-000080b0: 666f 756e 6420 696e 2060 7468 325f 6461  found in `th2_da
-000080c0: 7461 5f73 6572 7669 6365 732f 696e 7465  ta_services/inte
-000080d0: 7266 6163 6573 2f75 7469 6c73 2f72 6573  rfaces/utils/res
-000080e0: 6f6c 7665 722e 7079 602e 2020 0a20 2020  olver.py`.  .   
-000080f0: 2020 2020 2041 6c6c 2064 6174 612d 736f       All data-so
-00008100: 7572 6365 7320 7368 6f75 6c64 2069 6d70  urces should imp
-00008110: 6c65 6d65 6e74 2074 6865 6d2e 0a20 2020  lement them..   
-00008120: 2020 2020 200a 2020 2020 2020 2020 5468       .        Th
-00008130: 6520 6964 6561 206f 6620 7573 696e 6720  e idea of using 
-00008140: 7265 736f 6c76 6572 733a 0a20 2020 2020  resolvers:.     
-00008150: 2020 2049 7420 736f 6c76 6573 2074 6865     It solves the
-00008160: 2070 726f 626c 656d 206f 6620 6861 7669   problem of havi
-00008170: 6e67 2061 2066 6577 2044 6174 6153 6f75  ng a few DataSou
-00008180: 7263 6573 2077 6974 6820 7369 6d69 6c61  rces with simila
-00008190: 7220 6461 7461 2c0a 2020 2020 2020 2020  r data,.        
-000081a0: 6275 7420 7769 7468 2064 6966 6665 7265  but with differe
-000081b0: 6e74 2077 6179 7320 746f 2067 6574 2069  nt ways to get i
-000081c0: 742e 0a20 2020 2020 2020 200a 2020 2020  t..        .    
-000081d0: 2020 2020 5468 6573 6520 636c 6173 7365      These classe
-000081e0: 7320 7072 6f76 6964 6520 796f 7520 6765  s provide you ge
-000081f0: 7474 6572 206d 6574 686f 6473 2e0a 2020  tter methods..  
-00008200: 2020 2020 2020 5573 696e 6720 7468 6573        Using thes
-00008210: 6520 636c 6173 7365 7320 616c 6c6f 7773  e classes allows
-00008220: 2079 6f75 2074 6f20 6672 6565 6c79 2073   you to freely s
-00008230: 7769 7463 6820 6265 7477 6565 6e20 6469  witch between di
-00008240: 6666 6572 656e 7420 6461 7461 0a20 2020  fferent data.   
-00008250: 2020 2020 2066 6f72 6d61 7473 2061 6e64       formats and
-00008260: 2064 6f6e 2774 2063 6861 6e67 6520 796f   don't change yo
-00008270: 7572 2063 6f64 652e 0a20 2020 2020 2020  ur code..       
-00008280: 200a 2020 2020 2020 2020 5265 736f 6c76   .        Resolv
-00008290: 6572 7320 736f 6c76 6520 7468 6520 7072  ers solve the pr
-000082a0: 6f62 6c65 6d20 6f66 2064 6174 612d 666f  oblem of data-fo
-000082b0: 726d 6174 206d 6967 7261 7469 6f6e 2e0a  rmat migration..
-000082c0: 2020 2020 2020 2020 2d20 6669 656c 6473          - fields
-000082d0: 2070 6c61 6365 2063 616e 2062 6520 6368   place can be ch
-000082e0: 616e 6765 640a 2020 2020 2020 2020 2d20  anged.        - 
-000082f0: 6669 656c 6473 206e 616d 6573 2063 616e  fields names can
-00008300: 2062 6520 6368 616e 6765 640a 2020 2020   be changed.    
-00008310: 2020 2020 0a20 2020 2020 2020 2052 6573      .        Res
-00008320: 6f6c 7665 7273 2063 616e 2077 6f72 6b20  olvers can work 
-00008330: 6f6e 6c79 2077 6974 6820 6f6e 6520 6576  only with one ev
-00008340: 656e 742f 6d65 7373 6167 652e 0a20 2020  ent/message..   
-00008350: 2020 2020 2049 7420 6d65 616e 732c 2069       It means, i
-00008360: 6620 796f 7572 206d 6573 7361 6765 2068  f your message h
-00008370: 6173 2073 7562 2d6d 6573 7361 6765 7320  as sub-messages 
-00008380: 286c 696b 6520 7468 322d 6d65 7373 6167  (like th2-messag
-00008390: 6573 2069 6e20 6c77 6470 2920 6974 200a  es in lwdp) it .
-000083a0: 2020 2020 2020 2020 776f 6e27 7420 776f          won't wo
-000083b0: 726b 2c20 6265 6361 7573 6520 7265 736f  rk, because reso
-000083c0: 6c76 6572 2077 696c 6c20 6e6f 7420 6b6e  lver will not kn
-000083d0: 6f77 2077 6974 6820 7768 6963 6820 7375  ow with which su
-000083e0: 622d 6d65 7373 6167 6520 7368 6f75 6c64  b-message should
-000083f0: 2069 7420 776f 726b 2e20 0a20 2020 2020   it work. .     
-00008400: 2020 200a 2020 2020 2020 2020 2a2a 576f     .        **Wo
-00008410: 726b 6172 6f75 6e64 2a2a 2020 0a20 2020  rkaround**  .   
-00008420: 2020 2020 2031 2e20 4578 7061 6e64 2061       1. Expand a
-00008430: 6c6c 2079 6f75 7220 6d65 7373 6167 6573  ll your messages
-00008440: 202d 3e20 606e 6577 5f64 203d 2079 6f75   -> `new_d = you
-00008450: 725f 6461 7461 2e6d 6170 284d 6573 7361  r_data.map(Messa
-00008460: 6765 4669 656c 6452 6573 6f6c 7665 722e  geFieldResolver.
-00008470: 6578 7061 6e64 5f6d 6573 7361 6765 2960  expand_message)`
-00008480: 0a20 2020 2020 2020 2032 2e20 5573 6520  .        2. Use 
-00008490: 6045 7870 616e 6465 644d 6573 7361 6765  `ExpandedMessage
-000084a0: 4669 656c 6452 6573 6f6c 7665 7260 2069  FieldResolver` i
-000084b0: 6e73 7465 6164 206f 6620 7573 7561 6c20  nstead of usual 
-000084c0: 604d 6573 7361 6765 4669 656c 6452 6573  `MessageFieldRes
-000084d0: 6f6c 7665 7260 2077 6865 6e20 0a20 2020  olver` when .   
-000084e0: 2020 2020 2020 2020 2079 6f75 2074 616b           you tak
-000084f0: 6520 6669 656c 6473 2066 6f72 2065 7870  e fields for exp
-00008500: 616e 6465 6420 6d65 7373 6167 6573 2e0a  anded messages..
-00008510: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00008520: 202a 2a49 6d70 6c65 6d65 6e74 6174 696f   **Implementatio
-00008530: 6e20 6164 7669 6365 3a2a 2a0a 2020 2020  n advice:**.    
-00008540: 2020 2020 312e 2072 6169 7365 204e 6f74      1. raise Not
-00008550: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
-00008560: 202d 2d20 6966 2079 6f75 7220 496d 706c   -- if your Impl
-00008570: 656d 656e 7461 7469 6f6e 2064 6f65 736e  ementation doesn
-00008580: 2774 2073 7570 706f 7274 2074 6869 7320  't support this 
-00008590: 6765 7474 6572 2e0a 2020 2020 2020 2020  getter..        
-000085a0: 0a20 2020 2020 2020 202a 2a50 6572 666f  .        **Perfo
-000085b0: 726d 616e 6365 2069 6d70 6163 743a 2a2a  rmance impact:**
-000085c0: 0a20 2020 2020 2020 202d 2049 7420 6120  .        - It a 
-000085d0: 6269 7420 736c 6f77 6572 2074 6861 6e20  bit slower than 
-000085e0: 7573 696e 6720 6e61 6b65 6420 6669 656c  using naked fiel
-000085f0: 6420 6163 6365 7373 2060 6469 6374 5b27  d access `dict['
-00008600: 6b65 7927 5d60 2e0a 2020 2020 2020 2020  key']`..        
-00008610: 0a20 2020 2020 2020 2023 2320 322e 342e  .        ## 2.4.
-00008620: 204c 696e 6b73 0a20 2020 2020 2020 200a   Links.        .
-00008630: 2020 2020 2020 2020 2d20 5b52 6570 6f72          - [Repor
-00008640: 7420 4461 7461 2050 726f 7669 6465 725d  t Data Provider]
-00008650: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00008660: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
-00008670: 7270 742d 6461 7461 2d70 726f 7669 6465  rpt-data-provide
-00008680: 7229 0a20 2020 2020 2020 202d 205b 5468  r).        - [Th
-00008690: 3220 4461 7461 2053 6572 7669 6365 7320  2 Data Services 
-000086a0: 5574 696c 735d 2868 7474 7073 3a2f 2f67  Utils](https://g
-000086b0: 6974 6875 622e 636f 6d2f 7468 322d 6e65  ithub.com/th2-ne
-000086c0: 742f 7468 322d 6461 7461 2d73 6572 7669  t/th2-data-servi
-000086d0: 6365 732d 7574 696c 7329 0a20 2020 2020  ces-utils).     
-000086e0: 2020 200a 2020 2020 2020 2020 2320 332e     .        # 3.
-000086f0: 2042 6573 7420 7072 6163 7469 6365 730a   Best practices.
-00008700: 2020 2020 2020 2020 4465 7065 6e64 696e          Dependin
-00008710: 6720 6f6e 2068 6f77 2079 6f75 2077 6f72  g on how you wor
-00008720: 6b20 7769 7468 2060 4461 7461 206f 626a  k with `Data obj
-00008730: 6563 7460 2c20 6974 2063 616e 2062 6520  ect`, it can be 
-00008740: 736c 6f77 206f 6620 6661 7374 2e0a 2020  slow of fast..  
-00008750: 2020 2020 2020 4173 2077 6974 6820 6120        As with a 
-00008760: 7265 6c61 7469 6f6e 616c 2064 6174 6162  relational datab
-00008770: 6173 652c 2079 6f75 2063 616e 2077 7269  ase, you can wri
-00008780: 7465 2061 2071 7565 7279 2074 6861 7420  te a query that 
-00008790: 7769 6c6c 2072 6574 7572 6e20 6461 7461  will return data
-000087a0: 2073 6c6f 776c 7920 6f72 2071 7569 636b   slowly or quick
-000087b0: 6c79 2c0a 2020 2020 2020 2020 7468 6520  ly,.        the 
-000087c0: 7361 6d65 2077 6865 6e20 776f 726b 696e  same when workin
-000087d0: 6720 7769 7468 2061 2060 4461 7461 206f  g with a `Data o
-000087e0: 626a 6563 7460 2e0a 2020 2020 2020 2020  bject`..        
-000087f0: 0a20 2020 2020 2020 2046 6f6c 6c6f 7720  .        Follow 
-00008800: 7468 6520 7275 6c65 7320 746f 206d 616b  the rules to mak
-00008810: 6520 796f 7572 2077 6f72 6b20 7769 7468  e your work with
-00008820: 2044 6174 6120 6f62 6a65 6374 2066 6173   Data object fas
-00008830: 743a 0a20 2020 2020 2020 2031 2e20 5573  t:.        1. Us
-00008840: 6520 6044 6174 612e 7573 655f 6361 6368  e `Data.use_cach
-00008850: 6528 2960 2069 6620 796f 7520 6974 6572  e()` if you iter
-00008860: 6174 6520 6461 7461 206d 6f72 6520 7468  ate data more th
-00008870: 616e 206f 6e65 2074 696d 652e 0a20 2020  an one time..   
-00008880: 2020 2020 2032 2e20 5472 7920 746f 2064       2. Try to d
-00008890: 6f6e 2774 2069 7465 7261 7465 206f 6e65  on't iterate one
-000088a0: 2060 4461 7461 206f 626a 6563 7460 2069   `Data object` i
-000088b0: 6e73 6964 6520 7468 6520 6f74 6865 7220  nside the other 
-000088c0: 6f6e 652e 0a20 2020 2020 2020 2020 2020  one..           
-000088d0: 4966 2079 6f75 2073 686f 756c 6420 746f  If you should to
-000088e0: 2064 6f20 6974 2c20 7573 6520 7368 6f72   do it, use shor
-000088f0: 7420 6044 6174 6120 6f62 6a65 6374 6020  t `Data object` 
-00008900: 6669 7273 7420 616e 6420 6c6f 6e67 2060  first and long `
-00008910: 4461 7461 206f 626a 6563 7460 2069 6e73  Data object` ins
-00008920: 6964 6520 7468 6520 6c6f 6f70 2e0a 2020  ide the loop..  
-00008930: 2020 2020 2020 2020 2049 7427 6c6c 2061           It'll a
-00008940: 6c6c 6f77 2079 6f75 206f 7065 6e20 7468  llow you open th
-00008950: 6520 6361 6368 6520 6669 6c65 206f 7220  e cache file or 
-00008960: 6372 6561 7465 2061 2072 6571 7565 7374  create a request
-00008970: 2074 6f20 6044 6174 6120 736f 7572 6365   to `Data source
-00008980: 6020 6c65 7373 206e 756d 6265 7220 6f66  ` less number of
-00008990: 2074 696d 6573 2e0a 2020 2020 2020 2020   times..        
-000089a0: 0a20 2020 2020 2020 2023 2034 2e20 4f66  .        # 4. Of
-000089b0: 6669 6369 616c 2044 6174 6153 6f75 7263  ficial DataSourc
-000089c0: 6520 696d 706c 656d 656e 7461 7469 6f6e  e implementation
-000089d0: 730a 2020 2020 2020 2020 0a20 2020 2020  s.        .     
-000089e0: 2020 202d 205b 4c69 6768 7477 6569 6768     - [Lightweigh
-000089f0: 7420 4461 7461 2050 726f 7669 6465 7220  t Data Provider 
-00008a00: 4461 7461 2053 6f75 7263 655d 2868 7474  Data Source](htt
-00008a10: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00008a20: 7468 322d 6e65 742f 7468 322d 6473 2d73  th2-net/th2-ds-s
-00008a30: 6f75 7263 652d 6c77 6470 290a 2020 2020  ource-lwdp).    
-00008a40: 2020 2020 0a20 2020 2020 2020 200a 2020      .        .  
-00008a50: 2020 2020 2020 2320 352e 2041 5049 0a20        # 5. API. 
-00008a60: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00008a70: 4966 2079 6f75 2061 7265 206c 6f6f 6b69  If you are looki
-00008a80: 6e67 2066 6f72 2063 6c61 7373 6573 2064  ng for classes d
-00008a90: 6573 6372 6970 7469 6f6e 2073 6565 2074  escription see t
-00008aa0: 6865 205b 4150 4920 446f 6375 6d65 6e74  he [API Document
-00008ab0: 6174 696f 6e5d 2864 6f63 756d 656e 7461  ation](documenta
-00008ac0: 7469 6f6e 2f61 7069 2f69 6e64 6578 2e6d  tion/api/index.m
-00008ad0: 6429 2e0a 2020 2020 2020 2020 0a20 2020  d)..        .   
-00008ae0: 2020 2020 2023 2036 2e20 4578 616d 706c       # 6. Exampl
-00008af0: 6573 0a20 2020 2020 2020 200a 2020 2020  es.        .    
-00008b00: 2020 2020 2d20 5b67 6574 5f73 7461 7274      - [get_start
-00008b10: 6564 5f65 7861 6d70 6c65 2e70 795d 2865  ed_example.py](e
-00008b20: 7861 6d70 6c65 732f 6765 745f 7374 6172  xamples/get_star
-00008b30: 7465 645f 6578 616d 706c 652e 7079 290a  ted_example.py).
-00008b40: 2020 2020 2020 2020 0a50 6c61 7466 6f72          .Platfor
-00008b50: 6d3a 2055 4e4b 4e4f 574e 0a52 6571 7569  m: UNKNOWN.Requi
-00008b60: 7265 732d 5079 7468 6f6e 3a20 3e3d 332e  res-Python: >=3.
-00008b70: 370a 4465 7363 7269 7074 696f 6e2d 436f  7.Description-Co
-00008b80: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
-00008b90: 2f6d 6172 6b64 6f77 6e0a 5072 6f76 6964  /markdown.Provid
-00008ba0: 6573 2d45 7874 7261 3a20 7264 700a 5072  es-Extra: rdp.Pr
-00008bb0: 6f76 6964 6573 2d45 7874 7261 3a20 7264  ovides-Extra: rd
-00008bc0: 7035 0a50 726f 7669 6465 732d 4578 7472  p5.Provides-Extr
-00008bd0: 613a 2072 6470 360a 5072 6f76 6964 6573  a: rdp6.Provides
-00008be0: 2d45 7874 7261 3a20 6c77 6470 0a50 726f  -Extra: lwdp.Pro
-00008bf0: 7669 6465 732d 4578 7472 613a 206c 7764  vides-Extra: lwd
-00008c00: 7031 0a50 726f 7669 6465 732d 4578 7472  p1.Provides-Extr
-00008c10: 613a 206c 7764 7032 0a50 726f 7669 6465  a: lwdp2.Provide
-00008c20: 732d 4578 7472 613a 206c 7764 7033 0a50  s-Extra: lwdp3.P
-00008c30: 726f 7669 6465 732d 4578 7472 613a 206c  rovides-Extra: l
-00008c40: 7764 702d 6465 760a 5072 6f76 6964 6573  wdp-dev.Provides
-00008c50: 2d45 7874 7261 3a20 7574 696c 732d 7270  -Extra: utils-rp
-00008c60: 742d 7669 6577 6572 0a50 726f 7669 6465  t-viewer.Provide
-00008c70: 732d 4578 7472 613a 2075 7469 6c73 2d72  s-Extra: utils-r
-00008c80: 7074 2d76 6965 7765 7235 0a50 726f 7669  pt-viewer5.Provi
-00008c90: 6465 732d 4578 7472 613a 2075 7469 6c73  des-Extra: utils
-00008ca0: 2d61 6476 616e 6365 640a                 -advanced.
+00006870: 2023 204d 6f72 6520 7465 6368 2064 6574   # More tech det
+00006880: 6169 6c73 3a0a 2020 2020 2020 2020 2320  ails:.        # 
+00006890: 2020 496e 2074 6869 7320 6361 7365 2c20    In this case, 
+000068a0: 7468 6572 6520 6973 206e 6f20 6c69 6e65  there is no line
+000068b0: 2060 6672 6f6d 2074 6832 5f64 6174 615f   `from th2_data_
+000068c0: 7365 7276 6963 6573 2e64 6174 615f 736f  services.data_so
+000068d0: 7572 6365 2069 6d70 6f72 7420 6c77 6470  urce import lwdp
+000068e0: 2060 0a20 2020 2020 2020 2023 2020 2062   `.        #   b
+000068f0: 6563 6175 7365 2077 6520 7368 6f75 6c64  ecause we should
+00006900: 206e 6f74 2063 686f 6f73 6520 666f 7220   not choose for 
+00006910: 7468 6520 7573 6572 2077 6869 6368 2061  the user which a
+00006920: 2064 6174 6120 736f 7572 6365 2074 6f20   data source to 
+00006930: 7573 652e 0a20 2020 2020 2020 2023 2020  use..        #  
+00006940: 2057 6520 646f 206e 6f74 206b 6e6f 7720   We do not know 
+00006950: 7768 6174 2068 6520 7769 6c6c 2063 686f  what he will cho
+00006960: 6f73 652c 2074 6865 7265 666f 7265 2c20  ose, therefore, 
+00006970: 7765 206d 7573 7420 7369 6d70 6c79 2061  we must simply a
+00006980: 6363 6573 730a 2020 2020 2020 2020 2320  ccess.        # 
+00006990: 2020 7468 6520 696e 7465 7266 6163 652c    the interface,
+000069a0: 2077 6869 6368 2077 696c 6c20 6265 2069   which will be i
+000069b0: 6e69 7469 616c 697a 6564 2062 7920 7468  nitialized by th
+000069c0: 6520 7573 6572 2e0a 2020 2020 2020 2020  e user..        
+000069d0: 0a20 2020 2020 2020 2023 2323 2323 2323  .        #######
+000069e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000069f0: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
+00006a00: 2020 2020 2020 2020 2320 5b35 5d20 5573          # [5] Us
+00006a10: 696e 6720 7574 696c 6974 7920 6675 6e63  ing utility func
+00006a20: 7469 6f6e 732e 0a20 2020 2020 2020 2023  tions..        #
+00006a30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006a40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006a50: 2323 2323 230a 2020 2020 2020 2020 6672  #####.        fr
+00006a60: 6f6d 2074 6832 5f64 6174 615f 7365 7276  om th2_data_serv
+00006a70: 6963 6573 2e75 7469 6c73 2e65 7665 6e74  ices.utils.event
+00006a80: 5f75 7469 6c73 2e66 7265 7175 656e 6369  _utils.frequenci
+00006a90: 6573 2069 6d70 6f72 7420 6765 745f 6361  es import get_ca
+00006aa0: 7465 676f 7279 5f66 7265 7175 656e 6369  tegory_frequenci
+00006ab0: 6573 320a 2020 2020 2020 2020 6672 6f6d  es2.        from
+00006ac0: 2074 6832 5f64 6174 615f 7365 7276 6963   th2_data_servic
+00006ad0: 6573 2e75 7469 6c73 2e65 7665 6e74 5f75  es.utils.event_u
+00006ae0: 7469 6c73 2e74 6f74 616c 7320 696d 706f  tils.totals impo
+00006af0: 7274 2067 6574 5f63 6174 6567 6f72 795f  rt get_category_
+00006b00: 746f 7461 6c73 320a 2020 2020 2020 2020  totals2.        
+00006b10: 6672 6f6d 2074 6832 5f64 6174 615f 7365  from th2_data_se
+00006b20: 7276 6963 6573 2e75 7469 6c73 2e63 6174  rvices.utils.cat
+00006b30: 6567 6f72 7920 696d 706f 7274 2043 6174  egory import Cat
+00006b40: 6567 6f72 790a 2020 2020 2020 2020 6672  egory.        fr
+00006b50: 6f6d 2074 6832 5f64 6174 615f 7365 7276  om th2_data_serv
+00006b60: 6963 6573 2e75 7469 6c73 2e65 7665 6e74  ices.utils.event
+00006b70: 5f75 7469 6c73 2e65 7665 6e74 5f75 7469  _utils.event_uti
+00006b80: 6c73 2069 6d70 6f72 7420 6973 5f73 6f72  ls import is_sor
+00006b90: 7465 640a 2020 2020 2020 2020 0a20 2020  ted.        .   
+00006ba0: 2020 2020 2023 205b 352e 315d 2047 6574       # [5.1] Get
+00006bb0: 2074 6865 2071 7561 6e74 6974 6965 7320   the quantities 
+00006bc0: 6f66 2065 7665 6e74 7320 666f 7220 6469  of events for di
+00006bd0: 6666 6572 656e 7420 6361 7465 676f 7269  fferent categori
+00006be0: 6573 2e0a 2020 2020 2020 2020 6d65 7472  es..        metr
+00006bf0: 6963 7320 3d20 5b0a 2020 2020 2020 2020  ics = [.        
+00006c00: 2020 2020 4361 7465 676f 7279 2822 6461      Category("da
+00006c10: 7465 222c 206c 616d 6264 6120 6d3a 2054  te", lambda m: T
+00006c20: 6832 5469 6d65 7374 616d 7043 6f6e 7665  h2TimestampConve
+00006c30: 7274 6572 2e74 6f5f 6461 7465 7469 6d65  rter.to_datetime
+00006c40: 286d 5b22 7374 6172 7454 696d 6573 7461  (m["startTimesta
+00006c50: 6d70 225d 292e 6461 7465 2829 292c 0a20  mp"]).date()),. 
+00006c60: 2020 2020 2020 2020 2020 2043 6174 6567             Categ
+00006c70: 6f72 7928 2273 7461 7475 7322 2c20 6c61  ory("status", la
+00006c80: 6d62 6461 206d 3a20 6d5b 2273 7563 6365  mbda m: m["succe
+00006c90: 7373 6675 6c22 5d29 2c0a 2020 2020 2020  ssful"]),.      
+00006ca0: 2020 5d0a 2020 2020 2020 2020 6361 7465    ].        cate
+00006cb0: 676f 7279 5f74 6f74 616c 7320 3d20 6765  gory_totals = ge
+00006cc0: 745f 6361 7465 676f 7279 5f74 6f74 616c  t_category_total
+00006cd0: 7332 2865 7665 6e74 732c 206d 6574 7269  s2(events, metri
+00006ce0: 6373 290a 2020 2020 2020 2020 7072 696e  cs).        prin
+00006cf0: 7428 6361 7465 676f 7279 5f74 6f74 616c  t(category_total
+00006d00: 7329 0a20 2020 2020 2020 2022 2222 0a20  s).        """. 
+00006d10: 2020 2020 2020 202b 2d2d 2d2d 2d2d 2d2d         +--------
+00006d20: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  +------------+--
+00006d30: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00006d40: 2d2d 2b0a 2020 2020 2020 2020 7c20 2020  --+.        |   
+00006d50: 2020 2020 207c 2064 6174 6520 2020 2020       | date     
+00006d60: 2020 7c20 7374 6174 7573 2020 207c 2020    | status   |  
+00006d70: 2063 6f75 6e74 207c 0a20 2020 2020 2020   count |.       
+00006d80: 202b 3d3d 3d3d 3d3d 3d3d 2b3d 3d3d 3d3d   +========+=====
+00006d90: 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d  =======+========
+00006da0: 3d3d 2b3d 3d3d 3d3d 3d3d 3d3d 2b0a 2020  ==+=========+.  
+00006db0: 2020 2020 2020 7c20 2020 2020 2020 207c        |        |
+00006dc0: 2032 3032 332d 3031 2d30 3520 7c20 5472   2023-01-05 | Tr
+00006dd0: 7565 2020 2020 207c 2020 2020 2020 2033  ue     |       3
+00006de0: 207c 0a20 2020 2020 2020 202b 2d2d 2d2d   |.        +----
+00006df0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
+00006e00: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  -+----------+---
+00006e10: 2d2d 2d2d 2d2d 2b0a 2020 2020 2020 2020  ------+.        
+00006e20: 7c20 2020 2020 2020 207c 2032 3032 332d  |        | 2023-
+00006e30: 3031 2d30 3520 7c20 4661 6c73 6520 2020  01-05 | False   
+00006e40: 207c 2020 2020 2020 2031 207c 0a20 2020   |       1 |.   
+00006e50: 2020 2020 202b 2d2d 2d2d 2d2d 2d2d 2b2d       +--------+-
+00006e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+00006e70: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+00006e80: 2b0a 2020 2020 2020 2020 7c20 636f 756e  +.        | coun
+00006e90: 7420 207c 2020 2020 2020 2020 2020 2020  t  |            
+00006ea0: 7c20 2020 2020 2020 2020 207c 2020 2020  |          |    
+00006eb0: 2020 2032 207c 0a20 2020 2020 2020 202b     2 |.        +
+00006ec0: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00006ed0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+00006ee0: 2b2d 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020  +---------+.    
+00006ef0: 2020 2020 7c20 746f 7461 6c73 207c 2020      | totals |  
+00006f00: 2020 2020 2020 2020 2020 7c20 312f 3120            | 1/1 
+00006f10: 2020 2020 207c 2020 2020 2020 2034 207c       |       4 |
+00006f20: 0a20 2020 2020 2020 202b 2d2d 2d2d 2d2d  .        +------
+00006f30: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  --+------------+
+00006f40: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
+00006f50: 2d2d 2d2d 2b0a 2020 2020 2020 2020 2222  ----+.        ""
+00006f60: 220a 2020 2020 2020 2020 0a20 2020 2020  ".        .     
+00006f70: 2020 2023 205b 352e 325d 2047 6574 2074     # [5.2] Get t
+00006f80: 6865 206e 756d 6265 7220 6f66 2065 7665  he number of eve
+00006f90: 6e74 7320 7769 7468 2073 7461 7475 7320  nts with status 
+00006fa0: 7375 6363 6573 7366 756c 2e0a 2020 2020  successful..    
+00006fb0: 2020 2020 6361 7465 676f 7279 203d 2043      category = C
+00006fc0: 6174 6567 6f72 7928 2273 7461 7475 7322  ategory("status"
+00006fd0: 2c20 6c61 6d62 6461 206d 3a20 6d5b 2273  , lambda m: m["s
+00006fe0: 7563 6365 7373 6675 6c22 5d29 0a20 2020  uccessful"]).   
+00006ff0: 2020 2020 2063 6174 6567 6f72 795f 6672       category_fr
+00007000: 6571 7565 6e63 6965 7320 3d20 6765 745f  equencies = get_
+00007010: 6361 7465 676f 7279 5f66 7265 7175 656e  category_frequen
+00007020: 6369 6573 3228 6576 656e 7473 2c20 6361  cies2(events, ca
+00007030: 7465 676f 7279 290a 2020 2020 2020 2020  tegory).        
+00007040: 7072 696e 7428 6361 7465 676f 7279 5f66  print(category_f
+00007050: 7265 7175 656e 6369 6573 290a 2020 2020  requencies).    
+00007060: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00007070: 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  +--------+------
+00007080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+00007090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000070a0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b  -----+---------+
+000070b0: 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020 2020  --------+.      
+000070c0: 2020 7c20 2020 2020 2020 207c 2074 696d    |        | tim
+000070d0: 6573 7461 6d70 5f73 7461 7274 2020 2020  estamp_start    
+000070e0: 207c 2074 696d 6573 7461 6d70 5f65 6e64   | timestamp_end
+000070f0: 2020 2020 2020 207c 2046 616c 7365 2020         | False  
+00007100: 207c 2020 2054 7275 6520 7c0a 2020 2020   |   True |.    
+00007110: 2020 2020 2b3d 3d3d 3d3d 3d3d 3d2b 3d3d      +========+==
+00007120: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007130: 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ===+============
+00007140: 3d3d 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d  =========+======
+00007150: 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d 2b0a 2020  ===+========+.  
+00007160: 2020 2020 2020 7c20 2020 2020 2020 207c        |        |
+00007170: 2032 3032 332d 3031 2d30 3554 3133 3a35   2023-01-05T13:5
+00007180: 373a 3035 207c 2032 3032 332d 3031 2d30  7:05 | 2023-01-0
+00007190: 3554 3133 3a35 373a 3036 207c 2030 2020  5T13:57:06 | 0  
+000071a0: 2020 2020 207c 2020 2020 2020 3320 7c0a       |      3 |.
+000071b0: 2020 2020 2020 2020 2b2d 2d2d 2d2d 2d2d          +-------
+000071c0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
+000071d0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+000071e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+000071f0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+00007200: 2b0a 2020 2020 2020 2020 7c20 2020 2020  +.        |     
+00007210: 2020 207c 2032 3032 332d 3031 2d30 3554     | 2023-01-05T
+00007220: 3134 3a30 323a 3035 207c 2032 3032 332d  14:02:05 | 2023-
+00007230: 3031 2d30 3554 3134 3a30 323a 3036 207c  01-05T14:02:06 |
+00007240: 2031 2020 2020 2020 207c 2020 2020 2020   1       |      
+00007250: 3020 7c0a 2020 2020 2020 2020 2b2d 2d2d  0 |.        +---
+00007260: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+00007270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+00007280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007290: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -+---------+----
+000072a0: 2d2d 2d2d 2b0a 2020 2020 2020 2020 7c20  ----+.        | 
+000072b0: 636f 756e 7420 207c 2020 2020 2020 2020  count  |        
+000072c0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+000072d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072e0: 2020 207c 2020 2020 2020 2020 207c 2020     |         |  
+000072f0: 2020 2020 3220 7c0a 2020 2020 2020 2020      2 |.        
+00007300: 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  +--------+------
+00007310: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+00007320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007330: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b  -----+---------+
+00007340: 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020 2020  --------+.      
+00007350: 2020 7c20 746f 7461 6c73 207c 2020 2020    | totals |    
+00007360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007370: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+00007380: 2020 2020 2020 207c 2031 2020 2020 2020         | 1      
+00007390: 207c 2020 2020 2020 3320 7c0a 2020 2020   |      3 |.    
+000073a0: 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d      +--------+--
+000073b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000073c0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
+000073d0: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
+000073e0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2b0a 2020  ---+--------+.  
+000073f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00007400: 2020 0a20 2020 2020 2020 2023 205b 352e    .        # [5.
+00007410: 335d 2043 6865 636b 2069 6620 6576 656e  3] Check if even
+00007420: 7473 2061 7265 2073 6f72 7465 642e 0a20  ts are sorted.. 
+00007430: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00007440: 6973 5f73 6f72 7465 6428 6576 656e 7473  is_sorted(events
+00007450: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+00007460: 7265 7375 6c74 290a 2020 2020 2020 2020  result).        
+00007470: 6060 600a 2020 2020 2020 2020 3c21 2d2d  ```.        <!--
+00007480: 2065 6e64 2067 6574 5f73 7461 7274 6564   end get_started
+00007490: 5f65 7861 6d70 6c65 2e70 7920 2d2d 3e0a  _example.py -->.
+000074a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000074b0: 2023 2320 322e 332e 2053 686f 7274 2074   ## 2.3. Short t
+000074c0: 6865 6f72 790a 2020 2020 2020 2020 0a20  heory.        . 
+000074d0: 2020 2020 2020 2054 6865 206c 6962 7261         The libra
+000074e0: 7279 2070 726f 7669 6465 7320 746f 6f6c  ry provides tool
+000074f0: 7320 666f 7220 6861 6e64 6c69 6e67 2073  s for handling s
+00007500: 7472 6561 6d20 6461 7461 2e20 5768 6174  tream data. What
+00007510: 2773 2061 2073 7472 6561 6d3f 2049 7427  's a stream? It'
+00007520: 7320 6120 7365 7175 656e 6365 206f 6620  s a sequence of 
+00007530: 656c 656d 656e 7473 2066 726f 6d20 6120  elements from a 
+00007540: 736f 7572 6365 2074 6861 740a 2020 2020  source that.    
+00007550: 2020 2020 7375 7070 6f72 7473 2061 6767      supports agg
+00007560: 7265 6761 7465 206f 7065 7261 7469 6f6e  regate operation
+00007570: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
+00007580: 2020 2020 2323 2320 5465 726d 730a 2020      ### Terms.  
+00007590: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
+000075a0: 202a 2a44 6174 6120 6f62 6a65 6374 2a2a   **Data object**
+000075b0: 3a20 416e 2069 6e73 7461 6e63 6520 6f66  : An instance of
+000075c0: 2060 4461 7461 6020 636c 6173 7320 7768   `Data` class wh
+000075d0: 6963 6820 6973 2077 7261 7070 6572 2075  ich is wrapper u
+000075e0: 6e64 6572 2073 7472 6561 6d2e 0a20 2020  nder stream..   
+000075f0: 2020 2020 202d 202a 2a53 6571 7565 6e63       - **Sequenc
+00007600: 6520 6f66 2065 6c65 6d65 6e74 732a 2a3a  e of elements**:
+00007610: 0a20 2020 2020 2020 2020 2041 205f 4461  .          A _Da
+00007620: 7461 206f 626a 6563 745f 2070 726f 7669  ta object_ provi
+00007630: 6465 7320 616e 2069 6e74 6572 6661 6365  des an interface
+00007640: 2074 6f20 6120 7365 7175 656e 6365 6420   to a sequenced 
+00007650: 7365 7420 6f66 2076 616c 7565 7320 6f66  set of values of
+00007660: 2061 2073 7065 6369 6669 6320 656c 656d   a specific elem
+00007670: 656e 7420 7479 7065 2e20 5374 7265 616d  ent type. Stream
+00007680: 2069 6e73 6964 6520 7468 6520 5f44 6174   inside the _Dat
+00007690: 610a 2020 2020 2020 2020 2020 6f62 6a65  a.          obje
+000076a0: 6374 5f20 2a2a 646f 6e19 7420 6163 7475  ct_ **don.t actu
+000076b0: 616c 6c79 2073 746f 7265 2a2a 2065 6c65  ally store** ele
+000076c0: 6d65 6e74 733b 2074 6865 7920 6172 6520  ments; they are 
+000076d0: 636f 6d70 7574 6564 206f 6e20 6465 6d61  computed on dema
+000076e0: 6e64 2e0a 2020 2020 2020 2020 2d20 2a2a  nd..        - **
+000076f0: 6461 7461 2073 6f75 7263 652a 2a20 2865  data source** (e
+00007700: 7861 6374 6c79 2069 6e20 736d 616c 6c20  xactly in small 
+00007710: 6c65 7474 6572 7329 3a0a 2020 2020 2020  letters):.      
+00007720: 2020 2020 416e 7920 736f 7572 6365 206f      Any source o
+00007730: 6620 6461 7461 2e20 452e 672e 205b 4c69  f data. E.g. [Li
+00007740: 6768 7477 6569 6768 7420 4461 7461 2050  ghtweight Data P
+00007750: 726f 7669 6465 725d 2868 7474 7073 3a2f  rovider](https:/
+00007760: 2f67 6974 6875 622e 636f 6d2f 7468 322d  /github.com/th2-
+00007770: 6e65 742f 7468 322d 6c77 2d64 6174 612d  net/th2-lw-data-
+00007780: 7072 6f76 6964 6572 292c 2063 6f6c 6c65  provider), colle
+00007790: 6374 696f 6e73 2c0a 2020 2020 2020 2020  ctions,.        
+000077a0: 2020 6172 7261 7973 2c20 6f72 2049 2f4f    arrays, or I/O
+000077b0: 2072 6573 6f75 7263 6573 2e0a 2020 2020   resources..    
+000077c0: 2020 2020 2d20 2a2a 4461 7461 536f 7572      - **DataSour
+000077d0: 6365 2a2a 3a0a 2020 2020 2020 2020 2020  ce**:.          
+000077e0: 4120 636c 6173 7320 7468 6174 2069 7320  A class that is 
+000077f0: 616e 2069 6e74 6572 6d65 6469 6174 6520  an intermediate 
+00007800: 6c69 6e6b 2062 6574 7765 656e 2074 6865  link between the
+00007810: 2053 6f75 7263 6541 5049 2061 6e64 2043   SourceAPI and C
+00007820: 6f6d 6d61 6e64 732e 0a20 2020 2020 2020  ommands..       
+00007830: 202d 202a 2a53 6f75 7263 6541 5049 2a2a   - **SourceAPI**
+00007840: 3a0a 2020 2020 2020 2020 2020 4561 6368  :.          Each
+00007850: 2073 6f75 7263 6520 6861 7320 6974 7320   source has its 
+00007860: 6f77 6e20 4150 4920 746f 2072 6574 7269  own API to retri
+00007870: 6576 6520 6461 7461 2e20 536f 7572 6365  eve data. Source
+00007880: 4150 4920 6973 2061 2063 6c61 7373 2074  API is a class t
+00007890: 6861 7420 7072 6f76 6964 6520 4150 4920  hat provide API 
+000078a0: 666f 7220 736f 6d65 2064 6174 6120 736f  for some data so
+000078b0: 7572 6365 2e0a 2020 2020 2020 2020 2d20  urce..        - 
+000078c0: 2a2a 436f 6d6d 616e 6473 2a2a 3a0a 2020  **Commands**:.  
+000078d0: 2020 2020 2020 2020 436c 6173 7365 7320          Classes 
+000078e0: 7468 6174 2070 726f 7669 6465 2075 7365  that provide use
+000078f0: 722d 6672 6965 6e64 6c79 2069 6e74 6572  r-friendly inter
+00007900: 6661 6365 7320 666f 7220 6765 7474 696e  faces for gettin
+00007910: 6720 736f 6d65 2064 6174 6120 6672 6f6d  g some data from
+00007920: 2044 6174 6153 6f75 7263 652e 2043 6f6d   DataSource. Com
+00007930: 6d61 6e64 7320 7573 6520 5f53 6f75 7263  mands use _Sourc
+00007940: 6541 5049 5f20 746f 0a20 2020 2020 2020  eAPI_ to.       
+00007950: 2020 2061 6368 6965 7665 2069 742e 0a20     achieve it.. 
+00007960: 2020 2020 2020 202d 202a 2a41 6461 7074         - **Adapt
+00007970: 6572 732a 2a3a 0a20 2020 2020 2020 2020  ers**:.         
+00007980: 2049 7427 7320 7369 6d69 6c61 7220 746f   It's similar to
+00007990: 2066 756e 6374 696f 6e20 666f 7220 6044   function for `D
+000079a0: 6174 612e 6d61 7060 206d 6574 686f 642e  ata.map` method.
+000079b0: 2041 646f 7074 6162 6c65 2063 6f6d 6d61   Adoptable comma
+000079c0: 6e64 7320 7573 6564 2069 7420 746f 2075  nds used it to u
+000079d0: 7064 6174 6520 7468 6520 6461 7461 2073  pdate the data s
+000079e0: 7472 6561 6d2e 0a20 2020 2020 2020 202d  tream..        -
+000079f0: 202a 2a41 6767 7265 6761 7465 206f 7065   **Aggregate ope
+00007a00: 7261 7469 6f6e 732a 2a3a 0a20 2020 2020  rations**:.     
+00007a10: 2020 2020 2043 6f6d 6d6f 6e20 6f70 6572       Common oper
+00007a20: 6174 696f 6e73 2073 7563 6820 6173 2066  ations such as f
+00007a30: 696c 7465 722c 206d 6170 2c20 6c69 6d69  ilter, map, limi
+00007a40: 7420 616e 6420 736f 206f 6e2e 0a20 2020  t and so on..   
+00007a50: 2020 2020 202d 202a 2a57 6f72 6b66 6c6f       - **Workflo
+00007a60: 772a 2a3a 2041 6e20 6f72 6465 7265 6420  w**: An ordered 
+00007a70: 7365 7420 6f66 205f 4167 6772 6567 6174  set of _Aggregat
+00007a80: 6520 6f70 6572 6174 696f 6e73 5f2e 0a20  e operations_.. 
+00007a90: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00007aa0: 2323 2320 436f 6e63 6570 740a 2020 2020  ### Concept.    
+00007ab0: 2020 2020 0a20 2020 2020 2020 2054 6865      .        The
+00007ac0: 206c 6962 7261 7279 2064 6573 6372 6962   library describ
+00007ad0: 6573 2074 6865 2068 6967 682d 6c65 7665  es the high-leve
+00007ae0: 6c20 696e 7465 7266 6163 6573 2060 4953  l interfaces `IS
+00007af0: 6f75 7263 6541 5049 602c 2060 4944 6174  ourceAPI`, `IDat
+00007b00: 6153 6f75 7263 6560 2c20 6049 436f 6d6d  aSource`, `IComm
+00007b10: 616e 6460 2c20 6049 4164 6170 7465 7260  and`, `IAdapter`
+00007b20: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00007b30: 2020 2041 6e79 2064 6174 6120 736f 7572     Any data sour
+00007b40: 6365 206d 7573 7420 6265 2064 6573 6372  ce must be descr
+00007b50: 6962 6564 2062 7920 7468 6520 6049 4461  ibed by the `IDa
+00007b60: 7461 536f 7572 6365 6020 6162 7374 7261  taSource` abstra
+00007b70: 6374 2063 6c61 7373 2e20 5468 6573 6520  ct class. These 
+00007b80: 6361 6e20 6265 205f 4669 6c65 4461 7461  can be _FileData
+00007b90: 536f 7572 6365 5f2c 0a20 2020 2020 2020  Source_,.       
+00007ba0: 205f 4353 5644 6174 6153 6f75 7263 655f   _CSVDataSource_
+00007bb0: 2c20 5f44 4244 6174 6153 6f75 7263 655f  , _DBDataSource_
+00007bc0: 2061 6e64 206f 7468 6572 2e0a 2020 2020   and other..    
+00007bd0: 2020 2020 0a20 2020 2020 2020 2055 7375      .        Usu
+00007be0: 616c 6c79 2c20 6461 7461 2073 6f75 7263  ally, data sourc
+00007bf0: 6573 2068 6176 6520 736f 6d65 206b 696e  es have some kin
+00007c00: 6420 6f66 2041 5049 2e20 4461 7461 6261  d of API. Databa
+00007c10: 7365 7320 2d20 7072 6f76 6964 6520 5351  ses - provide SQ
+00007c20: 4c20 6c61 6e67 7561 6765 2c20 7768 656e  L language, when
+00007c30: 2077 6f72 6b69 6e67 2077 6974 6820 6120   working with a 
+00007c40: 6669 6c65 2c20 796f 7520 6361 6e20 7265  file, you can re
+00007c50: 6164 0a20 2020 2020 2020 206c 696e 6520  ad.        line 
+00007c60: 6279 206c 696e 652c 2065 7463 2e20 5468  by line, etc. Th
+00007c70: 6973 2041 5049 2069 7320 6465 7363 7269  is API is descri
+00007c80: 6265 6420 6279 2074 6865 2060 4953 6f75  bed by the `ISou
+00007c90: 7263 6541 5049 6020 636c 6173 732e 2042  rceAPI` class. B
+00007ca0: 6563 6175 7365 2064 6966 6665 7265 6e74  ecause different
+00007cb0: 2076 6572 7369 6f6e 7320 6f66 2074 6865   versions of the
+00007cc0: 2073 616d 6520 6461 7461 2073 6f75 7263   same data sourc
+00007cd0: 650a 2020 2020 2020 2020 6d61 7920 6861  e.        may ha
+00007ce0: 7665 2064 6966 6665 7265 6e74 2041 5049  ve different API
+00007cf0: 2c20 6974 2069 7320 6265 7474 6572 2074  , it is better t
+00007d00: 6f20 6372 6561 7465 2061 2063 6c61 7373  o create a class
+00007d10: 2066 6f72 2065 6163 6820 7665 7273 696f   for each versio
+00007d20: 6e2e 0a20 2020 2020 2020 200a 2020 2020  n..        .    
+00007d30: 2020 2020 4765 6e65 7261 6c6c 792c 2064      Generally, d
+00007d40: 6174 6120 736f 7572 6365 2041 5049 7320  ata source APIs 
+00007d50: 6172 6520 6869 6464 656e 2062 6568 696e  are hidden behin
+00007d60: 6420 636f 6e76 656e 6965 6e74 2069 6e74  d convenient int
+00007d70: 6572 6661 6365 732e 2054 6865 2072 6f6c  erfaces. The rol
+00007d80: 6520 6f66 2074 6865 7365 2069 6e74 6572  e of these inter
+00007d90: 6661 6365 7320 6973 2070 6c61 7965 640a  faces is played.
+00007da0: 2020 2020 2020 2020 6279 2060 4943 6f6d          by `ICom
+00007db0: 6d61 6e64 6020 636c 6173 7365 732e 0a20  mand` classes.. 
+00007dc0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00007dd0: 6049 4164 6170 7465 7260 2063 6c61 7373  `IAdapter` class
+00007de0: 6573 2074 7261 6e73 666f 726d 2064 6174  es transform dat
+00007df0: 6120 7374 7265 616d 206c 696b 6520 6675  a stream like fu
+00007e00: 6e63 7469 6f6e 7320 666f 7220 6044 6174  nctions for `Dat
+00007e10: 612e 6d61 7060 206d 6574 686f 642e 2045  a.map` method. E
+00007e20: 7373 656e 7469 616c 6c79 2069 7427 7320  ssentially it's 
+00007e30: 7468 6520 7361 6d65 2074 6869 6e67 2062  the same thing b
+00007e40: 7574 206d 6f72 650a 2020 2020 2020 2020  ut more.        
+00007e50: 666c 6578 6962 6c65 2e0a 2020 2020 2020  flexible..      
+00007e60: 2020 0a20 2020 2020 2020 2046 6f72 2065    .        For e
+00007e70: 7861 6d70 6c65 2c20 4c77 4450 2044 6174  xample, LwDP Dat
+00007e80: 6153 6f75 7263 6528 6874 7470 733a 2f2f  aSource(https://
+00007e90: 6769 7468 7562 2e63 6f6d 2f74 6832 2d6e  github.com/th2-n
+00007ea0: 6574 2f74 6832 2d64 732d 736f 7572 6365  et/th2-ds-source
+00007eb0: 2d6c 7764 7029 2075 7365 7320 7468 6573  -lwdp) uses thes
+00007ec0: 6520 6162 7374 7261 6374 2063 6c61 7373  e abstract class
+00007ed0: 6573 2074 6f20 6275 696c 6420 6974 7320  es to build its 
+00007ee0: 696d 706c 656d 656e 7461 7469 6f6e 2e59  implementation.Y
+00007ef0: 6f75 2063 616e 2065 6173 696c 7920 6372  ou can easily cr
+00007f00: 6561 7465 2079 6f75 7220 6f77 6e20 756e  eate your own un
+00007f10: 6971 7565 2063 6f6d 6d61 6e64 7320 666f  ique commands fo
+00007f20: 7220 5f4c 7744 5020 4461 7461 536f 7572  r _LwDP DataSour
+00007f30: 6365 5f2c 2061 7320 7765 6c6c 2061 7320  ce_, as well as 
+00007f40: 656e 7469 7265 0a20 2020 2020 2020 205f  entire.        _
+00007f50: 4461 7461 536f 7572 6365 5f20 636c 6173  DataSource_ clas
+00007f60: 7365 732e 205b 4865 7265 2069 7320 6120  ses. [Here is a 
+00007f70: 646f 6375 6d65 6e74 6174 696f 6e5d 2864  documentation](d
+00007f80: 6f63 756d 656e 7461 7469 6f6e 2f64 6174  ocumentation/dat
+00007f90: 6173 6f75 7263 652e 6d64 2920 6f6e 2068  asource.md) on h
+00007fa0: 6f77 2074 6f20 696d 706c 656d 656e 7420  ow to implement 
+00007fb0: 7468 6573 6520 696e 7465 7266 6163 6573  these interfaces
+00007fc0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00007fd0: 2020 2021 5b44 6174 6120 7374 7265 616d     ![Data stream
+00007fe0: 2070 6970 656c 696e 655d 2864 6f63 756d   pipeline](docum
+00007ff0: 656e 7461 7469 6f6e 2f69 6d67 2f63 6f6e  entation/img/con
+00008000: 6365 7074 2e70 6e67 290a 2020 2020 2020  cept.png).      
+00008010: 2020 0a20 2020 2020 2020 2023 2323 2053    .        ### S
+00008020: 7472 6561 6d20 6f70 6572 6174 696f 6e73  tream operations
+00008030: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00008040: 2020 4675 7274 6865 726d 6f72 652c 2073    Furthermore, s
+00008050: 7472 6561 6d20 6f70 6572 6174 696f 6e73  tream operations
+00008060: 2068 6176 6520 7477 6f20 6675 6e64 616d   have two fundam
+00008070: 656e 7461 6c20 6368 6172 6163 7465 7269  ental characteri
+00008080: 7374 6963 7320 7468 6174 206d 616b 6520  stics that make 
+00008090: 7468 656d 2076 6572 7920 6469 6666 6572  them very differ
+000080a0: 656e 7420 6672 6f6d 2063 6f6c 6c65 6374  ent from collect
+000080b0: 696f 6e0a 2020 2020 2020 2020 6f70 6572  ion.        oper
+000080c0: 6174 696f 6e73 3a20 5f50 6970 656c 696e  ations: _Pipelin
+000080d0: 696e 675f 2061 6e64 205f 496e 7465 726e  ing_ and _Intern
+000080e0: 616c 2069 7465 7261 7469 6f6e 5f2e 0a20  al iteration_.. 
+000080f0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00008100: 2323 2323 2050 6970 656c 696e 696e 670a  #### Pipelining.
+00008110: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00008120: 204d 616e 7920 7374 7265 616d 206f 7065   Many stream ope
+00008130: 7261 7469 6f6e 7320 7265 7475 726e 2061  rations return a
+00008140: 2073 7472 6561 6d20 7468 656d 7365 6c76   stream themselv
+00008150: 6573 2e20 5468 6973 2061 6c6c 6f77 7320  es. This allows 
+00008160: 6f70 6572 6174 696f 6e73 2074 6f20 6265  operations to be
+00008170: 2063 6861 696e 6564 2074 6f20 666f 726d   chained to form
+00008180: 2061 206c 6172 6765 7220 7069 7065 6c69   a larger pipeli
+00008190: 6e65 2e0a 2020 2020 2020 2020 0a20 2020  ne..        .   
+000081a0: 2020 2020 2021 5b44 6174 6120 7374 7265       ![Data stre
+000081b0: 616d 2070 6970 656c 696e 655d 2864 6f63  am pipeline](doc
+000081c0: 756d 656e 7461 7469 6f6e 2f69 6d67 2f64  umentation/img/d
+000081d0: 6174 615f 7374 7265 616d 5f70 6970 656c  ata_stream_pipel
+000081e0: 696e 652e 706e 6729 0a20 2020 2020 2020  ine.png).       
+000081f0: 200a 2020 2020 2020 2020 2323 2323 2049   .        #### I
+00008200: 6e74 6572 6e61 6c20 6974 6572 6174 696f  nternal iteratio
+00008210: 6e0a 2020 2020 2020 2020 0a20 2020 2020  n.        .     
+00008220: 2020 2049 6e20 636f 6e74 7261 7374 2074     In contrast t
+00008230: 6f20 636f 6c6c 6563 7469 6f6e 732c 2077  o collections, w
+00008240: 6869 6368 2061 7265 2069 7465 7261 7465  hich are iterate
+00008250: 6420 6578 706c 6963 6974 6c79 2028 6578  d explicitly (ex
+00008260: 7465 726e 616c 2069 7465 7261 7469 6f6e  ternal iteration
+00008270: 292c 2073 7472 6561 6d20 6f70 6572 6174  ), stream operat
+00008280: 696f 6e73 2064 6f20 7468 6520 6974 6572  ions do the iter
+00008290: 6174 696f 6e0a 2020 2020 2020 2020 6265  ation.        be
+000082a0: 6869 6e64 2074 6865 2073 6365 6e65 7320  hind the scenes 
+000082b0: 666f 7220 796f 752e 204e 6f74 652c 2069  for you. Note, i
+000082c0: 7420 646f 6573 6e27 7420 6d65 616e 2079  t doesn't mean y
+000082d0: 6f75 2063 616e 6e6f 7420 6974 6572 6174  ou cannot iterat
+000082e0: 6520 7468 6520 5f44 6174 6120 6f62 6a65  e the _Data obje
+000082f0: 6374 5f2e 0a20 2020 2020 2020 200a 2020  ct_..        .  
+00008300: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00008310: 2323 2044 6174 6120 6974 6572 6174 696f  ## Data iteratio
+00008320: 6e0a 2020 2020 2020 2020 0a20 2020 2020  n.        .     
+00008330: 2020 2054 6865 2044 6174 6120 6f62 6a65     The Data obje
+00008340: 6374 2063 6f6e 7374 7275 6374 6f72 206d  ct constructor m
+00008350: 6574 686f 6420 7461 6b65 7320 696e 2061  ethod takes in a
+00008360: 7320 6172 6775 6d65 6e74 2065 6974 6865  s argument eithe
+00008370: 7220 616e 2069 7465 7261 746f 7220 6f76  r an iterator ov
+00008380: 6572 206f 626a 6563 7473 206f 7220 6120  er objects or a 
+00008390: 6765 6e65 7261 746f 7220 6675 6e63 7469  generator functi
+000083a0: 6f6e 2e0a 2020 2020 2020 2020 5468 6520  on..        The 
+000083b0: 4461 7461 206f 626a 6563 7420 6974 6572  Data object iter
+000083c0: 6174 6f72 2068 616e 646c 6573 2065 6163  ator handles eac
+000083d0: 6820 6974 656d 2069 6e20 7468 6973 2069  h item in this i
+000083e0: 7465 7261 746f 7220 6f72 2067 656e 6572  terator or gener
+000083f0: 6174 6f72 2061 7320 7468 6579 2061 7265  ator as they are
+00008400: 2c20 6d65 616e 696e 6720 6974 2064 6f65  , meaning it doe
+00008410: 736e 2774 2074 7279 2074 6f20 7265 6164  sn't try to read
+00008420: 2074 6865 2063 6f6e 7465 6e74 206f 6620   the content of 
+00008430: 6974 656d 206f 7220 7265 7475 726e 2074  item or return t
+00008440: 6865 6d20 6d6f 6469 6669 6564 2069 6e20  hem modified in 
+00008450: 616e 7920 7761 792c 2069 6e73 7465 6164  any way, instead
+00008460: 2072 6574 7572 6e73 2074 6865 2069 7465   returns the ite
+00008470: 6d20 6974 7365 6c66 2e0a 2020 2020 2020  m itself..      
+00008480: 2020 5468 6520 6f6e 6c79 2065 7863 6570    The only excep
+00008490: 7469 6f6e 2074 6f20 7468 6973 2069 7320  tion to this is 
+000084a0: 7768 656e 2044 6174 6120 6f62 6a65 6374  when Data object
+000084b0: 2069 7320 6275 696c 7420 7573 696e 6720   is built using 
+000084c0: 6974 6572 6174 6f72 206f 7220 6765 6e65  iterator or gene
+000084d0: 7261 746f 7220 6f76 6572 206f 7468 6572  rator over other
+000084e0: 2044 6174 6120 6f62 6a65 6374 732e 204e   Data objects. N
+000084f0: 6f74 6520 7468 6174 2074 6869 7320 6974  ote that this it
+00008500: 6572 6174 6f72 206f 7220 6765 6e65 7261  erator or genera
+00008510: 746f 7220 6d75 7374 206f 6e6c 7920 6265  tor must only be
+00008520: 2079 6965 6c64 696e 6720 4461 7461 206f   yielding Data o
+00008530: 626a 6563 7473 2061 6e64 206e 6f74 6869  bjects and nothi
+00008540: 6e67 2065 6c73 652e 2049 6620 7765 2062  ng else. If we b
+00008550: 7569 6c64 2066 726f 6d20 6120 6d69 7820  uild from a mix 
+00008560: 6f66 2044 6174 6120 6f62 6a65 6374 7320  of Data objects 
+00008570: 616e 6420 736f 6d65 206f 7468 6572 2074  and some other t
+00008580: 7970 6573 2c20 4461 7461 206f 626a 6563  ypes, Data objec
+00008590: 7473 2720 636f 6e74 656e 7420 776f 6e27  ts' content won'
+000085a0: 7420 6265 2072 6561 6420 616e 6420 696e  t be read and in
+000085b0: 7374 6561 6420 6974 2077 696c 6c20 6265  stead it will be
+000085c0: 2072 6574 7572 6e65 6420 6173 2044 6174   returned as Dat
+000085d0: 6120 6f62 6a65 6374 2069 7473 656c 662e  a object itself.
+000085e0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000085f0: 2020 536d 616c 6c20 6578 616d 706c 6520    Small example 
+00008600: 746f 2064 656d 6f6e 7374 7261 7465 3a0a  to demonstrate:.
+00008610: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00008620: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
+00008630: 2020 2066 726f 6d20 7468 325f 6461 7461     from th2_data
+00008640: 5f73 6572 7669 6365 732e 6461 7461 2069  _services.data i
+00008650: 6d70 6f72 7420 4461 7461 0a20 2020 2020  mport Data.     
+00008660: 2020 200a 2020 2020 2020 2020 6431 203d     .        d1 =
+00008670: 2044 6174 6128 5b31 2c32 2c33 5d29 0a20   Data([1,2,3]). 
+00008680: 2020 2020 2020 2064 3220 3d20 4461 7461         d2 = Data
+00008690: 285b 342c 352c 365d 290a 2020 2020 2020  ([4,5,6]).      
+000086a0: 2020 0a20 2020 2020 2020 206f 6e6c 795f    .        only_
+000086b0: 6461 7461 5f6f 626a 6563 7473 203d 2044  data_objects = D
+000086c0: 6174 6128 5b64 312c 6432 5d29 2023 2057  ata([d1,d2]) # W
+000086d0: 696c 6c20 6974 6572 6174 6520 6173 2031  ill iterate as 1
+000086e0: 2c32 2c33 2c34 2c35 2c36 0a20 2020 2020  ,2,3,4,5,6.     
+000086f0: 2020 2064 6174 615f 616e 645f 6c69 7374     data_and_list
+00008700: 203d 2044 6174 6128 5b64 312c 5b34 2c35   = Data([d1,[4,5
+00008710: 2c36 5d5d 2920 2320 5769 6c6c 2069 7465  ,6]]) # Will ite
+00008720: 7261 7465 2061 7320 6431 2c20 5b34 2c35  rate as d1, [4,5
+00008730: 2c36 5d0a 2020 2020 2020 2020 6461 7461  ,6].        data
+00008740: 5f61 6e64 5f6e 756d 6265 7273 203d 2044  _and_numbers = D
+00008750: 6174 6128 5b64 312c 342c 352c 365d 2920  ata([d1,4,5,6]) 
+00008760: 2320 5769 6c6c 2069 7465 7261 7465 2061  # Will iterate a
+00008770: 7320 6431 2c34 2c35 2c36 0a20 2020 2020  s d1,4,5,6.     
+00008780: 2020 206c 6973 7473 5f6f 6e6c 7920 3d20     lists_only = 
+00008790: 4461 7461 285b 312c 322c 335d 2c5b 342c  Data([1,2,3],[4,
+000087a0: 352c 365d 2920 2320 5769 6c6c 2069 7465  5,6]) # Will ite
+000087b0: 7261 7465 2061 7320 5b31 2c32 2c33 5d2c  rate as [1,2,3],
+000087c0: 5b34 2c35 2c36 5d0a 2020 2020 2020 2020  [4,5,6].        
+000087d0: 0a20 2020 2020 2020 2023 2049 6620 7765  .        # If we
+000087e0: 2077 616e 7420 746f 2069 7465 7261 7465   want to iterate
+000087f0: 206f 7665 7220 636f 6e74 656e 7420 6f66   over content of
+00008800: 206c 6973 7420 6f66 206c 6973 7473 2c20   list of lists, 
+00008810: 7765 2073 686f 756c 6420 6669 7273 7420  we should first 
+00008820: 6372 6561 7465 2044 6174 6120 6f62 6a65  create Data obje
+00008830: 6374 7320 6672 6f6d 2074 6865 6d2c 0a20  cts from them,. 
+00008840: 2020 2020 2020 2023 2074 6865 6e20 7573         # then us
+00008850: 6520 7468 656d 2074 6f20 636f 6e73 7472  e them to constr
+00008860: 7563 7420 6e65 7720 4461 7461 206f 626a  uct new Data obj
+00008870: 6563 7420 6173 2069 6e20 6361 7365 206f  ect as in case o
+00008880: 6620 6431 2061 6e64 2064 322c 2063 7265  f d1 and d2, cre
+00008890: 6174 696e 6720 276f 6e6c 795f 6461 7461  ating 'only_data
+000088a0: 5f6f 626a 6563 7473 2720 696e 2074 6869  _objects' in thi
+000088b0: 7320 6578 616d 706c 652e 0a20 2020 2020  s example..     
+000088c0: 2020 2060 6060 0a20 2020 2020 2020 2020     ```.         
+000088d0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000088e0: 2020 2323 2320 4461 7461 2063 6163 6869    ### Data cachi
+000088f0: 6e67 0a20 2020 2020 2020 200a 2020 2020  ng.        .    
+00008900: 2020 2020 5468 6520 5f44 6174 6120 6f62      The _Data ob
+00008910: 6a65 6374 5f20 7072 6f76 6964 6573 2074  ject_ provides t
+00008920: 6865 2061 6269 6c69 7479 2074 6f20 7573  he ability to us
+00008930: 6520 7468 6520 6361 6368 652e 2054 6865  e the cache. The
+00008940: 2063 6163 6865 2077 6f72 6b73 2066 6f72   cache works for
+00008950: 2065 6163 6820 5f44 6174 6120 6f62 6a65   each _Data obje
+00008960: 6374 5f2c 2074 6861 7420 6973 2c20 796f  ct_, that is, yo
+00008970: 7520 6368 6f6f 7365 0a20 2020 2020 2020  u choose.       
+00008980: 2077 6869 6368 205f 4461 7461 206f 626a   which _Data obj
+00008990: 6563 745f 2079 6f75 2077 616e 7420 746f  ect_ you want to
+000089a0: 2073 6176 652e 2054 6865 205f 4461 7461   save. The _Data
+000089b0: 206f 626a 6563 745f 2063 6163 6865 2069   object_ cache i
+000089c0: 7320 7361 7665 6420 6166 7465 7220 7468  s saved after th
+000089d0: 6520 6669 7273 7420 6974 6572 6174 696f  e first iteratio
+000089e0: 6e2c 2062 7574 2074 6865 2069 7465 7261  n, but the itera
+000089f0: 7469 6f6e 0a20 2020 2020 2020 2073 6f75  tion.        sou
+00008a00: 7263 6520 6d61 7920 6265 2064 6966 6665  rce may be diffe
+00008a10: 7265 6e74 2e0a 2020 2020 2020 2020 0a20  rent..        . 
+00008a20: 2020 2020 2020 2049 6620 796f 7520 646f         If you do
+00008a30: 6e27 7420 7573 6520 7468 6520 6361 6368  n't use the cach
+00008a40: 652c 2079 6f75 7220 736f 7572 6365 2077  e, your source w
+00008a50: 696c 6c20 6265 2074 6865 2064 6174 6120  ill be the data 
+00008a60: 736f 7572 6365 2079 6f75 2068 6176 6520  source you have 
+00008a70: 696e 2074 6865 205f 4461 7461 204f 626a  in the _Data Obj
+00008a80: 6563 745f 2e20 4275 7420 6966 2079 6f75  ect_. But if you
+00008a90: 2075 7365 2074 6865 2063 6163 6865 2c0a   use the cache,.
+00008aa0: 2020 2020 2020 2020 796f 7572 2073 6f75          your sou
+00008ab0: 7263 6520 6361 6e20 6265 2074 6865 2064  rce can be the d
+00008ac0: 6174 6120 736f 7572 6365 2c20 7468 6520  ata source, the 
+00008ad0: 7061 7265 6e74 2063 6163 6865 2c20 6f72  parent cache, or
+00008ae0: 206f 776e 2063 6163 6865 3a0a 2020 2020   own cache:.    
+00008af0: 2020 2020 0a20 2020 2020 2020 202a 2054      .        * T
+00008b00: 6865 2064 6174 6120 736f 7572 6365 3a0a  he data source:.
+00008b10: 2020 2020 2020 2020 2020 4966 2074 6865            If the
+00008b20: 205f 4461 7461 204f 626a 6563 745f 2064   _Data Object_ d
+00008b30: 6f65 736e 2774 2068 6176 6520 6120 7061  oesn't have a pa
+00008b40: 7265 6e74 2063 6163 6865 2061 6e64 2069  rent cache and i
+00008b50: 7473 2063 6163 6865 2e0a 2020 2020 2020  ts cache..      
+00008b60: 2020 2a20 5468 6520 7061 7265 6e74 2063    * The parent c
+00008b70: 6163 6865 3a0a 2020 2020 2020 2020 2020  ache:.          
+00008b80: 4966 2074 6865 205f 4461 7461 204f 626a  If the _Data Obj
+00008b90: 6563 745f 2068 6173 2061 2070 6172 656e  ect_ has a paren
+00008ba0: 7420 6361 6368 652e 2049 7420 646f 6573  t cache. It does
+00008bb0: 6e27 7420 6d61 7474 6572 2077 6861 7420  n't matter what 
+00008bc0: 706f 7369 7469 6f6e 2074 6865 2070 6172  position the par
+00008bd0: 656e 7420 6361 6368 6520 6861 7320 696e  ent cache has in
+00008be0: 2069 6e68 6572 6974 616e 6365 2e0a 2020   inheritance..  
+00008bf0: 2020 2020 2020 2020 5f44 6174 6120 4f62          _Data Ob
+00008c00: 6a65 6374 5f20 756e 6465 7273 7461 6e64  ject_ understand
+00008c10: 7320 7768 6f73 6520 6361 6368 6520 6974  s whose cache it
+00008c20: 2069 7320 616e 6420 6578 6563 7574 6573   is and executes
+00008c30: 2074 6865 2070 6172 7420 6f66 2074 6865   the part of the
+00008c40: 2077 6f72 6b66 6c6f 7720 7468 6174 2077   workflow that w
+00008c50: 6173 206e 6f74 2065 7865 6375 7465 642e  as not executed.
+00008c60: 0a20 2020 2020 2020 202a 2054 6865 206f  .        * The o
+00008c70: 776e 2063 6163 6865 3a0a 2020 2020 2020  wn cache:.      
+00008c80: 2020 2020 4966 2069 7420 6973 206e 6f74      If it is not
+00008c90: 2074 6865 2066 6972 7374 2069 7465 7261   the first itera
+00008ca0: 7469 6f6e 206f 6620 7468 6973 2044 6174  tion of this Dat
+00008cb0: 6120 6f62 6a65 6374 2e0a 2020 2020 2020  a object..      
+00008cc0: 2020 0a20 2020 2020 2020 204e 6f74 6520    .        Note 
+00008cd0: 7468 6174 2074 6865 2063 6163 6865 2073  that the cache s
+00008ce0: 7461 7465 206f 6620 7468 6520 4461 7461  tate of the Data
+00008cf0: 206f 626a 6563 7420 6973 206e 6f74 2069   object is not i
+00008d00: 6e68 6572 6974 6564 2e0a 2020 2020 2020  nherited..      
+00008d10: 2020 0a20 2020 2020 2020 2023 2323 2320    .        #### 
+00008d20: 466f 7263 6564 2063 6163 6869 6e67 0a20  Forced caching. 
+00008d30: 2020 2020 2020 2059 6f75 2063 616e 2074         You can t
+00008d40: 656c 6c20 4453 2074 6f20 6361 6368 6520  ell DS to cache 
+00008d50: 6461 7461 2074 6f20 7370 6563 6966 6963  data to specific
+00008d60: 2063 6163 6865 2066 696c 652c 2077 6869   cache file, whi
+00008d70: 6368 2077 6f6e 2774 2062 6520 6465 6c65  ch won't be dele
+00008d80: 7465 6420 6166 7465 7220 7363 7269 7074  ted after script
+00008d90: 2065 6e64 2e0a 2020 2020 2020 2020 596f   end..        Yo
+00008da0: 7520 6361 6e20 7365 6520 6578 616d 706c  u can see exampl
+00008db0: 6520 696e 2031 2e31 3220 7365 6374 696f  e in 1.12 sectio
+00008dc0: 6e20 6f66 205b 6765 745f 7374 6172 7465  n of [get_starte
+00008dd0: 645f 6578 616d 706c 655d 2865 7861 6d70  d_example](examp
+00008de0: 6c65 732f 6765 745f 7374 6172 7465 645f  les/get_started_
+00008df0: 6578 616d 706c 652e 7079 292e 0a20 2020  example.py)..   
+00008e00: 2020 2020 200a 2020 2020 2020 2020 0a20       .        . 
+00008e10: 2020 2020 2020 2023 2323 2045 7665 6e74         ### Event
+00008e20: 5472 6565 2061 6e64 2063 6f6c 6c65 6374  Tree and collect
+00008e30: 696f 6e73 0a20 2020 2020 2020 200a 2020  ions.        .  
+00008e40: 2020 2020 2020 2323 2323 2045 7665 6e74        #### Event
+00008e50: 5472 6565 0a20 2020 2020 2020 200a 2020  Tree.        .  
+00008e60: 2020 2020 2020 6045 7665 6e74 5472 6565        `EventTree
+00008e70: 6020 6973 2061 2074 7265 652d 6261 7365  ` is a tree-base
+00008e80: 6420 6461 7461 2073 7472 7563 7475 7265  d data structure
+00008e90: 206f 6620 6576 656e 7473 2e20 4974 2061   of events. It a
+00008ea0: 6c6c 6f77 7320 796f 7520 6765 7420 6368  llows you get ch
+00008eb0: 696c 6472 656e 2061 6e64 2070 6172 656e  ildren and paren
+00008ec0: 7473 206f 6620 6576 656e 742c 0a20 2020  ts of event,.   
+00008ed0: 2020 2020 2064 6973 706c 6179 2074 7265       display tre
+00008ee0: 652c 2067 6574 2066 756c 6c20 7061 7468  e, get full path
+00008ef0: 2074 6f20 6576 656e 7420 6574 632e 0a20   to event etc.. 
+00008f00: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00008f10: 4465 7461 696c 733a 0a20 2020 2020 2020  Details:.       
+00008f20: 200a 2020 2020 2020 2020 2a20 6045 7665   .        * `Eve
+00008f30: 6e74 5472 6565 6020 636f 6e74 6169 6e73  ntTree` contains
+00008f40: 2061 6c6c 2065 7665 6e74 7320 696e 206d   all events in m
+00008f50: 656d 6f72 792e 0a20 2020 2020 2020 202a  emory..        *
+00008f60: 2054 7265 6520 6861 7320 736f 6d65 2069   Tree has some i
+00008f70: 6d70 6f72 7461 6e74 2074 6572 6d73 3a0a  mportant terms:.
+00008f80: 2020 2020 2020 2020 2020 2020 312e 205f              1. _
+00008f90: 416e 6365 7374 6f72 5f20 6973 2061 6e79  Ancestor_ is any
+00008fa0: 2072 656c 6174 6976 6520 6f66 2074 6865   relative of the
+00008fb0: 2065 7665 6e74 2075 7020 7468 6520 7472   event up the tr
+00008fc0: 6565 2028 6772 616e 6470 6172 656e 742c  ee (grandparent,
+00008fd0: 2070 6172 656e 7420 6574 632e 292e 0a20   parent etc.).. 
+00008fe0: 2020 2020 2020 2020 2020 2032 2e20 5f50             2. _P
+00008ff0: 6172 656e 745f 2069 7320 6f6e 6c79 2074  arent_ is only t
+00009000: 6865 2066 6972 7374 2072 656c 6174 6976  he first relativ
+00009010: 6520 6f66 2074 6865 2065 7665 6e74 2075  e of the event u
+00009020: 7020 7468 6520 7472 6565 2e0a 2020 2020  p the tree..    
+00009030: 2020 2020 2020 2020 332e 205f 4368 696c          3. _Chil
+00009040: 645f 2069 7320 7468 6520 6669 7273 7420  d_ is the first 
+00009050: 7265 6c61 7469 7665 206f 6620 7468 6520  relative of the 
+00009060: 6576 656e 7420 646f 776e 2074 6865 2074  event down the t
+00009070: 7265 652e 0a20 2020 2020 2020 200a 2020  ree..        .  
+00009080: 2020 2020 2020 5461 6b65 2061 206c 6f6f        Take a loo
+00009090: 6b20 6174 2074 6865 2066 6f6c 6c6f 7769  k at the followi
+000090a0: 6e67 2048 544d 4c20 7472 6565 2074 6f20  ng HTML tree to 
+000090b0: 756e 6465 7273 7461 6e64 2074 6865 6d2e  understand them.
+000090c0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000090d0: 2020 2020 2060 6060 0a20 2020 2020 2020       ```.       
+000090e0: 2020 2020 203c 626f 6479 3e20 3c21 2d2d       <body> <!--
+000090f0: 2061 6e63 6573 746f 7220 2867 7261 6e64   ancestor (grand
+00009100: 7061 7265 6e74 292c 2062 7574 206e 6f74  parent), but not
+00009110: 2070 6172 656e 7420 2d2d 3e0a 2020 2020   parent -->.    
+00009120: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00009130: 3e20 3c21 2d2d 2070 6172 656e 7420 2620  > <!-- parent & 
+00009140: 616e 6365 7374 6f72 202d 2d3e 0a20 2020  ancestor -->.   
+00009150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009160: 203c 703e 4865 6c6c 6f2c 2077 6f72 6c64   <p>Hello, world
+00009170: 213c 2f70 3e20 3c21 2d2d 2063 6869 6c64  !</p> <!-- child
+00009180: 202d 2d3e 0a20 2020 2020 2020 2020 2020   -->.           
+00009190: 2020 2020 2020 2020 203c 703e 476f 6f64           <p>Good
+000091a0: 6279 6521 3c2f 703e 203c 212d 2d20 7369  bye!</p> <!-- si
+000091b0: 626c 696e 6720 2d2d 3e0a 2020 2020 2020  bling -->.      
+000091c0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+000091d0: 0a20 2020 2020 2020 2020 2020 203c 2f62  .            </b
+000091e0: 6f64 793e 0a20 2020 2020 2020 2020 2020  ody>.           
+000091f0: 6060 600a 2020 2020 2020 2020 0a20 2020  ```.        .   
+00009200: 2020 2020 2023 2323 2320 436f 6c6c 6563       #### Collec
+00009210: 7469 6f6e 730a 2020 2020 2020 2020 0a20  tions.        . 
+00009220: 2020 2020 2020 202a 2a45 7665 6e74 5472         **EventTr
+00009230: 6565 436f 6c6c 6563 7469 6f6e 2a2a 2069  eeCollection** i
+00009240: 7320 6120 636f 6c6c 6563 7469 6f6e 206f  s a collection o
+00009250: 6620 4576 656e 7454 7265 6573 2e20 5468  f EventTrees. Th
+00009260: 6520 636f 6c6c 6563 7469 6f6e 2062 7569  e collection bui
+00009270: 6c64 7320 6120 6665 7720 5f45 7665 6e74  lds a few _Event
+00009280: 5472 6565 5f20 6279 2070 6173 7365 6420  Tree_ by passed 
+00009290: 5f44 6174 610a 2020 2020 2020 2020 6f62  _Data.        ob
+000092a0: 6a65 6374 5f2e 2041 6c74 686f 7567 6820  ject_. Although 
+000092b0: 796f 7520 6361 6e20 6368 616e 6765 2074  you can change t
+000092c0: 6865 2074 7265 6520 6469 7265 6374 6c79  he tree directly
+000092d0: 2c20 6974 2773 2062 6574 7465 7220 746f  , it's better to
+000092e0: 2064 6f20 6974 2074 6872 6f75 6768 2063   do it through c
+000092f0: 6f6c 6c65 6374 696f 6e73 2062 6563 6175  ollections becau
+00009300: 7365 2074 6865 7920 6172 6520 6177 6172  se they are awar
+00009310: 6520 6f66 0a20 2020 2020 2020 2060 6465  e of.        `de
+00009320: 7461 6368 6564 5f65 7665 6e74 7360 2061  tached_events` a
+00009330: 6e64 2063 616e 2073 6f6c 7665 2073 6f6d  nd can solve som
+00009340: 6520 6576 656e 7473 2064 6570 656e 6465  e events depende
+00009350: 6e63 6965 732e 2054 6865 2063 6f6c 6c65  ncies. The colle
+00009360: 6374 696f 6e20 6861 7320 7369 6d69 6c61  ction has simila
+00009370: 7220 6665 6174 7572 6573 206c 696b 6520  r features like 
+00009380: 6120 7369 6e67 6c65 205f 4576 656e 7454  a single _EventT
+00009390: 7265 655f 0a20 2020 2020 2020 2062 7574  ree_.        but
+000093a0: 2061 7070 6c79 696e 6720 7468 656d 2066   applying them f
+000093b0: 6f72 2061 6c6c 205f 4576 656e 7454 7265  or all _EventTre
+000093c0: 6573 5f2e 0a20 2020 2020 2020 200a 2020  es_..        .  
+000093d0: 2020 2020 2020 2a2a 5061 7265 6e74 4576        **ParentEv
+000093e0: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
+000093f0: 6e2a 2a20 6973 2061 2063 6f6c 6c65 6374  n** is a collect
+00009400: 696f 6e20 7369 6d69 6c61 7220 746f 205f  ion similar to _
+00009410: 4576 656e 7454 7265 6543 6f6c 6c65 6374  EventTreeCollect
+00009420: 696f 6e5f 2062 7574 2063 6f6e 7461 696e  ion_ but contain
+00009430: 696e 6720 6f6e 6c79 2070 6172 656e 7420  ing only parent 
+00009440: 6576 656e 7473 2074 6861 740a 2020 2020  events that.    
+00009450: 2020 2020 6172 6520 7265 6665 7265 6e63      are referenc
+00009460: 6564 2069 6e20 7468 6520 6461 7461 2073  ed in the data s
+00009470: 7472 6561 6d2e 2054 6865 2063 6f6c 6c65  tream. The colle
+00009480: 6374 696f 6e20 6861 7320 6665 6174 7572  ction has featur
+00009490: 6573 2073 696d 696c 6172 2074 6f20 5f45  es similar to _E
+000094a0: 7665 6e74 5472 6565 436f 6c6c 6563 7469  ventTreeCollecti
+000094b0: 6f6e 5f2e 0a20 2020 2020 2020 200a 2020  on_..        .  
+000094c0: 2020 2020 2020 4465 7461 696c 733a 0a20        Details:. 
+000094d0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000094e0: 2a20 546f 2075 7365 2045 5420 636f 6c6c  * To use ET coll
+000094f0: 6563 7469 6f6e 7320 796f 7520 6e65 6564  ections you need
+00009500: 2074 6f20 696e 6974 6961 6c69 7a65 2074   to initialize t
+00009510: 6865 6d20 6279 205f 4554 4344 7269 7665  hem by _ETCDrive
+00009520: 725f 2e20 4461 7461 2073 6f75 7263 6573  r_. Data sources
+00009530: 2075 7375 616c 6c79 2070 726f 7669 6465   usually provide
+00009540: 2074 6865 6d2e 0a20 2020 2020 2020 2020   them..         
+00009550: 2059 6f75 2063 616e 2063 7265 6174 6520   You can create 
+00009560: 6974 2062 7920 796f 7572 7365 6c66 2064  it by yourself d
+00009570: 6570 656e 6469 6e67 206f 6e20 796f 7572  epending on your
+00009580: 2064 6174 6120 7374 7275 6374 7572 652e   data structure.
+00009590: 0a20 2020 2020 2020 202a 2054 6865 2063  .        * The c
+000095a0: 6f6c 6c65 6374 696f 6e20 6861 7320 6120  ollection has a 
+000095b0: 6665 6174 7572 6520 746f 2072 6563 6f76  feature to recov
+000095c0: 6572 2065 7665 6e74 732e 2041 6c6c 2065  er events. All e
+000095d0: 7665 6e74 7320 7468 6174 2061 7265 206e  vents that are n
+000095e0: 6f74 2069 6e20 7468 6520 7265 6365 6976  ot in the receiv
+000095f0: 6564 2064 6174 6120 7374 7265 616d 2c20  ed data stream, 
+00009600: 6275 7420 7768 6963 6820 6172 650a 2020  but which are.  
+00009610: 2020 2020 2020 2020 7265 6665 7265 6e63          referenc
+00009620: 6564 2077 696c 6c20 6265 206c 6f61 6465  ed will be loade
+00009630: 6420 6672 6f6d 2074 6865 2064 6174 6120  d from the data 
+00009640: 736f 7572 6365 2e0a 2020 2020 2020 2020  source..        
+00009650: 2a20 596f 7520 6361 6e20 7461 6b65 2060  * You can take `
+00009660: 6465 7461 6368 6564 5f65 7665 6e74 7360  detached_events`
+00009670: 2074 6f20 7365 6520 7768 6963 6820 6576   to see which ev
+00009680: 656e 7473 2061 7265 206d 6973 7369 6e67  ents are missing
+00009690: 2e0a 2020 2020 2020 2020 2a20 4966 2079  ..        * If y
+000096a0: 6f75 2077 616e 742c 2079 6f75 2063 616e  ou want, you can
+000096b0: 2062 7569 6c64 2070 6172 656e 746c 6573   build parentles
+000096c0: 7320 7472 6565 7320 7768 6572 6520 7468  s trees where th
+000096d0: 6520 6d69 7373 696e 6720 6576 656e 7473  e missing events
+000096e0: 2061 7265 2073 7475 6262 6564 2069 6e73   are stubbed ins
+000096f0: 7465 6164 2e20 4a75 7374 0a20 2020 2020  tead. Just.     
+00009700: 2020 2020 2075 7365 2060 6765 745f 7061       use `get_pa
+00009710: 7265 6e74 6c65 7373 5f74 7265 6573 2829  rentless_trees()
+00009720: 602e 0a20 2020 2020 2020 200a 2020 2020  `..        .    
+00009730: 2020 2020 5265 7175 6972 656d 656e 7473      Requirements
+00009740: 3a0a 2020 2020 2020 2020 0a20 2020 2020  :.        .     
+00009750: 2020 2031 2e20 4576 656e 7473 2070 726f     1. Events pro
+00009760: 7669 6465 6420 746f 2045 5443 2068 6176  vided to ETC hav
+00009770: 6520 746f 2068 6176 6520 6065 7665 6e74  e to have `event
+00009780: 5f6e 616d 6560 2c20 6065 7665 6e74 5f69  _name`, `event_i
+00009790: 6460 2c20 6070 6172 656e 745f 6576 656e  d`, `parent_even
+000097a0: 745f 6964 6020 6669 656c 6473 2e20 5468  t_id` fields. Th
+000097b0: 6579 0a20 2020 2020 2020 2063 616e 2068  ey.        can h
+000097c0: 6176 6520 616e 6f74 6865 7220 6e61 6d65  ave another name
+000097d0: 7320 2869 7420 7265 736f 6c76 6573 2069  s (it resolves i
+000097e0: 6e20 7468 6520 6472 6976 6572 292e 0a20  n the driver).. 
+000097f0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00009800: 2323 2323 2048 696e 7473 0a20 2020 2020  #### Hints.     
+00009810: 2020 200a 2020 2020 2020 2020 2a20 5265     .        * Re
+00009820: 6d6f 7665 2061 6c6c 2075 6e6e 6563 6573  move all unneces
+00009830: 7361 7279 2066 6965 6c64 7320 6672 6f6d  sary fields from
+00009840: 2065 7665 6e74 7320 6265 666f 7265 2070   events before p
+00009850: 6173 7369 6e67 2074 6f20 6120 5f63 6f6c  assing to a _col
+00009860: 6c65 6374 696f 6e5f 2074 6f20 7265 6475  lection_ to redu
+00009870: 6365 206d 656d 6f72 7920 7573 6167 652e  ce memory usage.
+00009880: 0a20 2020 2020 2020 202a 2055 7365 2060  .        * Use `
+00009890: 7368 6f77 2829 6020 6d65 7468 6f64 2074  show()` method t
+000098a0: 6f20 7072 696e 7420 7468 6520 7472 6565  o print the tree
+000098b0: 2069 6e20 7472 6565 2d6c 696b 6520 7669   in tree-like vi
+000098c0: 6577 2e0a 2020 2020 2020 2020 2a20 4e6f  ew..        * No
+000098d0: 7465 2074 6861 7420 7468 6520 6067 6574  te that the `get
+000098e0: 5f78 6020 6d65 7468 6f64 7320 7769 6c6c  _x` methods will
+000098f0: 2072 6169 7365 2061 6e20 6578 6365 7074   raise an except
+00009900: 696f 6e20 6966 2079 6f75 2070 6173 7320  ion if you pass 
+00009910: 616e 2075 6e6b 6e6f 776e 2065 7665 6e74  an unknown event
+00009920: 2069 642c 2075 6e6c 696b 6520 7468 6520   id, unlike the 
+00009930: 6066 696e 645f 7860 206d 6574 686f 6473  `find_x` methods
+00009940: 2028 0a20 2020 2020 2020 2020 2074 6865   (.          the
+00009950: 7920 7265 7475 726e 204e 6f6e 6529 2e0a  y return None)..
+00009960: 2020 2020 2020 2020 2a20 4966 2079 6f75          * If you
+00009970: 2077 616e 7420 746f 206b 6e6f 7720 7468   want to know th
+00009980: 6174 2073 7065 6369 6669 6564 2065 7665  at specified eve
+00009990: 6e74 2065 7869 7374 732c 2075 7365 2074  nt exists, use t
+000099a0: 6865 2070 7974 686f 6e20 6069 6e60 206b  he python `in` k
+000099b0: 6579 776f 7264 2028 652e 672e 2060 2765  eyword (e.g. `'e
+000099c0: 7665 6e74 2d69 6427 2069 6e20 6576 656e  vent-id' in even
+000099d0: 7473 5f74 7265 6560 292e 0a20 2020 2020  ts_tree`)..     
+000099e0: 2020 202a 2055 7365 2074 6865 2070 7974     * Use the pyt
+000099f0: 686f 6e20 606c 656e 6020 6b65 7977 6f72  hon `len` keywor
+00009a00: 6420 746f 2067 6574 2065 7665 6e74 7320  d to get events 
+00009a10: 6e75 6d62 6572 2069 6e20 7468 6520 7472  number in the tr
+00009a20: 6565 2e0a 2020 2020 2020 2020 0a20 2020  ee..        .   
+00009a30: 2020 2020 2023 2323 2046 6965 6c64 2052       ### Field R
+00009a40: 6573 6f6c 7665 7273 0a20 2020 2020 2020  esolvers.       
+00009a50: 2049 6e74 6572 6661 6365 2063 616e 2062   Interface can b
+00009a60: 6520 666f 756e 6420 696e 2060 7468 325f  e found in `th2_
+00009a70: 6461 7461 5f73 6572 7669 6365 732f 696e  data_services/in
+00009a80: 7465 7266 6163 6573 2f75 7469 6c73 2f72  terfaces/utils/r
+00009a90: 6573 6f6c 7665 722e 7079 602e 2020 0a20  esolver.py`.  . 
+00009aa0: 2020 2020 2020 2041 6c6c 2064 6174 612d         All data-
+00009ab0: 736f 7572 6365 7320 7368 6f75 6c64 2069  sources should i
+00009ac0: 6d70 6c65 6d65 6e74 2074 6865 6d2e 0a20  mplement them.. 
+00009ad0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00009ae0: 5468 6520 6964 6561 206f 6620 7573 696e  The idea of usin
+00009af0: 6720 7265 736f 6c76 6572 733a 0a20 2020  g resolvers:.   
+00009b00: 2020 2020 2049 7420 736f 6c76 6573 2074       It solves t
+00009b10: 6865 2070 726f 626c 656d 206f 6620 6861  he problem of ha
+00009b20: 7669 6e67 2061 2066 6577 2044 6174 6153  ving a few DataS
+00009b30: 6f75 7263 6573 2077 6974 6820 7369 6d69  ources with simi
+00009b40: 6c61 7220 6461 7461 2c0a 2020 2020 2020  lar data,.      
+00009b50: 2020 6275 7420 7769 7468 2064 6966 6665    but with diffe
+00009b60: 7265 6e74 2077 6179 7320 746f 2067 6574  rent ways to get
+00009b70: 2069 742e 0a20 2020 2020 2020 200a 2020   it..        .  
+00009b80: 2020 2020 2020 5468 6573 6520 636c 6173        These clas
+00009b90: 7365 7320 7072 6f76 6964 6520 796f 7520  ses provide you 
+00009ba0: 6765 7474 6572 206d 6574 686f 6473 2e0a  getter methods..
+00009bb0: 2020 2020 2020 2020 5573 696e 6720 7468          Using th
+00009bc0: 6573 6520 636c 6173 7365 7320 616c 6c6f  ese classes allo
+00009bd0: 7773 2079 6f75 2074 6f20 6672 6565 6c79  ws you to freely
+00009be0: 2073 7769 7463 6820 6265 7477 6565 6e20   switch between 
+00009bf0: 6469 6666 6572 656e 7420 6461 7461 0a20  different data. 
+00009c00: 2020 2020 2020 2066 6f72 6d61 7473 2061         formats a
+00009c10: 6e64 2064 6f6e 2774 2063 6861 6e67 6520  nd don't change 
+00009c20: 796f 7572 2063 6f64 652e 0a20 2020 2020  your code..     
+00009c30: 2020 200a 2020 2020 2020 2020 5265 736f     .        Reso
+00009c40: 6c76 6572 7320 736f 6c76 6520 7468 6520  lvers solve the 
+00009c50: 7072 6f62 6c65 6d20 6f66 2064 6174 612d  problem of data-
+00009c60: 666f 726d 6174 206d 6967 7261 7469 6f6e  format migration
+00009c70: 2e0a 2020 2020 2020 2020 2d20 6669 656c  ..        - fiel
+00009c80: 6473 2070 6c61 6365 2063 616e 2062 6520  ds place can be 
+00009c90: 6368 616e 6765 640a 2020 2020 2020 2020  changed.        
+00009ca0: 2d20 6669 656c 6473 206e 616d 6573 2063  - fields names c
+00009cb0: 616e 2062 6520 6368 616e 6765 640a 2020  an be changed.  
+00009cc0: 2020 2020 2020 0a20 2020 2020 2020 2052        .        R
+00009cd0: 6573 6f6c 7665 7273 2063 616e 2077 6f72  esolvers can wor
+00009ce0: 6b20 6f6e 6c79 2077 6974 6820 6f6e 6520  k only with one 
+00009cf0: 6576 656e 742f 6d65 7373 6167 652e 0a20  event/message.. 
+00009d00: 2020 2020 2020 2049 7420 6d65 616e 732c         It means,
+00009d10: 2069 6620 796f 7572 206d 6573 7361 6765   if your message
+00009d20: 2068 6173 2073 7562 2d6d 6573 7361 6765   has sub-message
+00009d30: 7320 286c 696b 6520 7468 322d 6d65 7373  s (like th2-mess
+00009d40: 6167 6573 2069 6e20 6c77 6470 2920 6974  ages in lwdp) it
+00009d50: 200a 2020 2020 2020 2020 776f 6e27 7420   .        won't 
+00009d60: 776f 726b 2c20 6265 6361 7573 6520 7265  work, because re
+00009d70: 736f 6c76 6572 2077 696c 6c20 6e6f 7420  solver will not 
+00009d80: 6b6e 6f77 2077 6974 6820 7768 6963 6820  know with which 
+00009d90: 7375 622d 6d65 7373 6167 6520 7368 6f75  sub-message shou
+00009da0: 6c64 2069 7420 776f 726b 2e20 0a20 2020  ld it work. .   
+00009db0: 2020 2020 200a 2020 2020 2020 2020 2a2a       .        **
+00009dc0: 576f 726b 6172 6f75 6e64 2a2a 2020 0a20  Workaround**  . 
+00009dd0: 2020 2020 2020 2031 2e20 4578 7061 6e64         1. Expand
+00009de0: 2061 6c6c 2079 6f75 7220 6d65 7373 6167   all your messag
+00009df0: 6573 202d 3e20 606e 6577 5f64 203d 2079  es -> `new_d = y
+00009e00: 6f75 725f 6461 7461 2e6d 6170 284d 6573  our_data.map(Mes
+00009e10: 7361 6765 4669 656c 6452 6573 6f6c 7665  sageFieldResolve
+00009e20: 722e 6578 7061 6e64 5f6d 6573 7361 6765  r.expand_message
+00009e30: 2960 0a20 2020 2020 2020 2032 2e20 5573  )`.        2. Us
+00009e40: 6520 6045 7870 616e 6465 644d 6573 7361  e `ExpandedMessa
+00009e50: 6765 4669 656c 6452 6573 6f6c 7665 7260  geFieldResolver`
+00009e60: 2069 6e73 7465 6164 206f 6620 7573 7561   instead of usua
+00009e70: 6c20 604d 6573 7361 6765 4669 656c 6452  l `MessageFieldR
+00009e80: 6573 6f6c 7665 7260 2077 6865 6e20 0a20  esolver` when . 
+00009e90: 2020 2020 2020 2020 2020 2079 6f75 2074             you t
+00009ea0: 616b 6520 6669 656c 6473 2066 6f72 2065  ake fields for e
+00009eb0: 7870 616e 6465 6420 6d65 7373 6167 6573  xpanded messages
+00009ec0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00009ed0: 2020 202a 2a49 6d70 6c65 6d65 6e74 6174     **Implementat
+00009ee0: 696f 6e20 6164 7669 6365 3a2a 2a0a 2020  ion advice:**.  
+00009ef0: 2020 2020 2020 312e 2072 6169 7365 204e        1. raise N
+00009f00: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
+00009f10: 6f72 202d 2d20 6966 2079 6f75 7220 496d  or -- if your Im
+00009f20: 706c 656d 656e 7461 7469 6f6e 2064 6f65  plementation doe
+00009f30: 736e 2774 2073 7570 706f 7274 2074 6869  sn't support thi
+00009f40: 7320 6765 7474 6572 2e0a 2020 2020 2020  s getter..      
+00009f50: 2020 0a20 2020 2020 2020 202a 2a50 6572    .        **Per
+00009f60: 666f 726d 616e 6365 2069 6d70 6163 743a  formance impact:
+00009f70: 2a2a 0a20 2020 2020 2020 202d 2049 7420  **.        - It 
+00009f80: 6120 6269 7420 736c 6f77 6572 2074 6861  a bit slower tha
+00009f90: 6e20 7573 696e 6720 6e61 6b65 6420 6669  n using naked fi
+00009fa0: 656c 6420 6163 6365 7373 2060 6469 6374  eld access `dict
+00009fb0: 5b27 6b65 7927 5d60 2e0a 2020 2020 2020  ['key']`..      
+00009fc0: 2020 0a20 2020 2020 2020 2023 2320 322e    .        ## 2.
+00009fd0: 342e 204c 696e 6b73 0a20 2020 2020 2020  4. Links.       
+00009fe0: 200a 2020 2020 2020 2020 2d20 5b52 6570   .        - [Rep
+00009ff0: 6f72 7420 4461 7461 2050 726f 7669 6465  ort Data Provide
+0000a000: 725d 2868 7474 7073 3a2f 2f67 6974 6875  r](https://githu
+0000a010: 622e 636f 6d2f 7468 322d 6e65 742f 7468  b.com/th2-net/th
+0000a020: 322d 7270 742d 6461 7461 2d70 726f 7669  2-rpt-data-provi
+0000a030: 6465 7229 0a20 2020 2020 2020 202d 205b  der).        - [
+0000a040: 5468 3220 4461 7461 2053 6572 7669 6365  Th2 Data Service
+0000a050: 7320 5574 696c 735d 2868 7474 7073 3a2f  s Utils](https:/
+0000a060: 2f67 6974 6875 622e 636f 6d2f 7468 322d  /github.com/th2-
+0000a070: 6e65 742f 7468 322d 6461 7461 2d73 6572  net/th2-data-ser
+0000a080: 7669 6365 732d 7574 696c 7329 0a20 2020  vices-utils).   
+0000a090: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+0000a0a0: 332e 2042 6573 7420 7072 6163 7469 6365  3. Best practice
+0000a0b0: 730a 2020 2020 2020 2020 4465 7065 6e64  s.        Depend
+0000a0c0: 696e 6720 6f6e 2068 6f77 2079 6f75 2077  ing on how you w
+0000a0d0: 6f72 6b20 7769 7468 2060 4461 7461 206f  ork with `Data o
+0000a0e0: 626a 6563 7460 2c20 6974 2063 616e 2062  bject`, it can b
+0000a0f0: 6520 736c 6f77 206f 6620 6661 7374 2e0a  e slow of fast..
+0000a100: 2020 2020 2020 2020 4173 2077 6974 6820          As with 
+0000a110: 6120 7265 6c61 7469 6f6e 616c 2064 6174  a relational dat
+0000a120: 6162 6173 652c 2079 6f75 2063 616e 2077  abase, you can w
+0000a130: 7269 7465 2061 2071 7565 7279 2074 6861  rite a query tha
+0000a140: 7420 7769 6c6c 2072 6574 7572 6e20 6461  t will return da
+0000a150: 7461 2073 6c6f 776c 7920 6f72 2071 7569  ta slowly or qui
+0000a160: 636b 6c79 2c0a 2020 2020 2020 2020 7468  ckly,.        th
+0000a170: 6520 7361 6d65 2077 6865 6e20 776f 726b  e same when work
+0000a180: 696e 6720 7769 7468 2061 2060 4461 7461  ing with a `Data
+0000a190: 206f 626a 6563 7460 2e0a 2020 2020 2020   object`..      
+0000a1a0: 2020 0a20 2020 2020 2020 2046 6f6c 6c6f    .        Follo
+0000a1b0: 7720 7468 6520 7275 6c65 7320 746f 206d  w the rules to m
+0000a1c0: 616b 6520 796f 7572 2077 6f72 6b20 7769  ake your work wi
+0000a1d0: 7468 2044 6174 6120 6f62 6a65 6374 2066  th Data object f
+0000a1e0: 6173 743a 0a20 2020 2020 2020 2031 2e20  ast:.        1. 
+0000a1f0: 5573 6520 6044 6174 612e 7573 655f 6361  Use `Data.use_ca
+0000a200: 6368 6528 2960 2069 6620 796f 7520 6974  che()` if you it
+0000a210: 6572 6174 6520 6461 7461 206d 6f72 6520  erate data more 
+0000a220: 7468 616e 206f 6e65 2074 696d 652e 0a20  than one time.. 
+0000a230: 2020 2020 2020 2032 2e20 5472 7920 746f         2. Try to
+0000a240: 2064 6f6e 2774 2069 7465 7261 7465 206f   don't iterate o
+0000a250: 6e65 2060 4461 7461 206f 626a 6563 7460  ne `Data object`
+0000a260: 2069 6e73 6964 6520 7468 6520 6f74 6865   inside the othe
+0000a270: 7220 6f6e 652e 0a20 2020 2020 2020 2020  r one..         
+0000a280: 2020 4966 2079 6f75 2073 686f 756c 6420    If you should 
+0000a290: 746f 2064 6f20 6974 2c20 7573 6520 7368  to do it, use sh
+0000a2a0: 6f72 7420 6044 6174 6120 6f62 6a65 6374  ort `Data object
+0000a2b0: 6020 6669 7273 7420 616e 6420 6c6f 6e67  ` first and long
+0000a2c0: 2060 4461 7461 206f 626a 6563 7460 2069   `Data object` i
+0000a2d0: 6e73 6964 6520 7468 6520 6c6f 6f70 2e0a  nside the loop..
+0000a2e0: 2020 2020 2020 2020 2020 2049 7427 6c6c             It'll
+0000a2f0: 2061 6c6c 6f77 2079 6f75 206f 7065 6e20   allow you open 
+0000a300: 7468 6520 6361 6368 6520 6669 6c65 206f  the cache file o
+0000a310: 7220 6372 6561 7465 2061 2072 6571 7565  r create a reque
+0000a320: 7374 2074 6f20 6044 6174 6120 736f 7572  st to `Data sour
+0000a330: 6365 6020 6c65 7373 206e 756d 6265 7220  ce` less number 
+0000a340: 6f66 2074 696d 6573 2e0a 2020 2020 2020  of times..      
+0000a350: 2020 0a20 2020 2020 2020 2023 2034 2e20    .        # 4. 
+0000a360: 4f66 6669 6369 616c 2044 6174 6153 6f75  Official DataSou
+0000a370: 7263 6520 696d 706c 656d 656e 7461 7469  rce implementati
+0000a380: 6f6e 730a 2020 2020 2020 2020 0a20 2020  ons.        .   
+0000a390: 2020 2020 202d 205b 4c69 6768 7477 6569       - [Lightwei
+0000a3a0: 6768 7420 4461 7461 2050 726f 7669 6465  ght Data Provide
+0000a3b0: 7220 4461 7461 2053 6f75 7263 655d 2868  r Data Source](h
+0000a3c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0000a3d0: 6d2f 7468 322d 6e65 742f 7468 322d 6473  m/th2-net/th2-ds
+0000a3e0: 2d73 6f75 7263 652d 6c77 6470 290a 2020  -source-lwdp).  
+0000a3f0: 2020 2020 2020 0a20 2020 2020 2020 200a        .        .
+0000a400: 2020 2020 2020 2020 2320 352e 2041 5049          # 5. API
+0000a410: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+0000a420: 2020 4966 2079 6f75 2061 7265 206c 6f6f    If you are loo
+0000a430: 6b69 6e67 2066 6f72 2063 6c61 7373 6573  king for classes
+0000a440: 2064 6573 6372 6970 7469 6f6e 2073 6565   description see
+0000a450: 2074 6865 205b 4150 4920 446f 6375 6d65   the [API Docume
+0000a460: 6e74 6174 696f 6e5d 2864 6f63 756d 656e  ntation](documen
+0000a470: 7461 7469 6f6e 2f61 7069 2f69 6e64 6578  tation/api/index
+0000a480: 2e6d 6429 2e0a 2020 2020 2020 2020 0a20  .md)..        . 
+0000a490: 2020 2020 2020 2023 2036 2e20 4578 616d         # 6. Exam
+0000a4a0: 706c 6573 0a20 2020 2020 2020 200a 2020  ples.        .  
+0000a4b0: 2020 2020 2020 2d20 5b67 6574 5f73 7461        - [get_sta
+0000a4c0: 7274 6564 5f65 7861 6d70 6c65 2e70 795d  rted_example.py]
+0000a4d0: 2865 7861 6d70 6c65 732f 6765 745f 7374  (examples/get_st
+0000a4e0: 6172 7465 645f 6578 616d 706c 652e 7079  arted_example.py
+0000a4f0: 290a 2020 2020 2020 2020 0a50 6c61 7466  ).        .Platf
+0000a500: 6f72 6d3a 2055 4e4b 4e4f 574e 0a52 6571  orm: UNKNOWN.Req
+0000a510: 7569 7265 732d 5079 7468 6f6e 3a20 3e3d  uires-Python: >=
+0000a520: 332e 370a 4465 7363 7269 7074 696f 6e2d  3.7.Description-
+0000a530: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
+0000a540: 7874 2f6d 6172 6b64 6f77 6e0a 5072 6f76  xt/markdown.Prov
+0000a550: 6964 6573 2d45 7874 7261 3a20 7264 700a  ides-Extra: rdp.
+0000a560: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+0000a570: 7264 7035 0a50 726f 7669 6465 732d 4578  rdp5.Provides-Ex
+0000a580: 7472 613a 2072 6470 360a 5072 6f76 6964  tra: rdp6.Provid
+0000a590: 6573 2d45 7874 7261 3a20 6c77 6470 0a50  es-Extra: lwdp.P
+0000a5a0: 726f 7669 6465 732d 4578 7472 613a 206c  rovides-Extra: l
+0000a5b0: 7764 7031 0a50 726f 7669 6465 732d 4578  wdp1.Provides-Ex
+0000a5c0: 7472 613a 206c 7764 7032 0a50 726f 7669  tra: lwdp2.Provi
+0000a5d0: 6465 732d 4578 7472 613a 206c 7764 7033  des-Extra: lwdp3
+0000a5e0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
+0000a5f0: 206c 7764 702d 6465 760a 5072 6f76 6964   lwdp-dev.Provid
+0000a600: 6573 2d45 7874 7261 3a20 7574 696c 732d  es-Extra: utils-
+0000a610: 7270 742d 7669 6577 6572 0a50 726f 7669  rpt-viewer.Provi
+0000a620: 6465 732d 4578 7472 613a 2075 7469 6c73  des-Extra: utils
+0000a630: 2d72 7074 2d76 6965 7765 7235 0a50 726f  -rpt-viewer5.Pro
+0000a640: 7669 6465 732d 4578 7472 613a 2075 7469  vides-Extra: uti
+0000a650: 6c73 2d61 6476 616e 6365 640a            ls-advanced.
```

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services.egg-info/SOURCES.txt` & `th2_data_services-2.0.0.dev8702324290/th2_data_services.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 th2_data_services.egg-info/dependency_links.txt
 th2_data_services.egg-info/requires.txt
 th2_data_services.egg-info/top_level.txt
 th2_data_services/_internal/__init__.py
 th2_data_services/_internal/perf_tests.py
 th2_data_services/config/__init__.py
 th2_data_services/config/config.py
+th2_data_services/dummy/__init__.py
+th2_data_services/dummy/data_source.py
 th2_data_services/event_tree/__init__.py
 th2_data_services/event_tree/etc_driver.py
 th2_data_services/event_tree/event_tree.py
 th2_data_services/event_tree/event_tree_collection.py
 th2_data_services/event_tree/exceptions.py
 th2_data_services/event_tree/parent_event_tree_collection.py
 th2_data_services/interfaces/__init__.py
```

### Comparing `th2_data_services-2.0.0.dev8662586819/th2_data_services.egg-info/requires.txt` & `th2_data_services-2.0.0.dev8702324290/th2_data_services.egg-info/requires.txt`

 * *Files identical despite different names*

