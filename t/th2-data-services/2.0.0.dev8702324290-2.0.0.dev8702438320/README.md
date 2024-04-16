# Comparing `tmp/th2_data_services-2.0.0.dev8702324290.tar.gz` & `tmp/th2_data_services-2.0.0.dev8702438320.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services-2.0.0.dev8702324290.tar", last modified: Tue Apr 16 08:23:11 2024, max compression
+gzip compressed data, was "dist/th2_data_services-2.0.0.dev8702438320.tar", last modified: Tue Apr 16 08:31:21 2024, max compression
```

## Comparing `th2_data_services-2.0.0.dev8702324290.tar` & `th2_data_services-2.0.0.dev8702438320.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    35047 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 08:22:58.000000 th2_data_services-2.0.0.dev8702324290/package_info.json
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/_internal/perf_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/config/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    41567 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/dummy/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/dummy/data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/etc_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/event_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    26246 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/parent_event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/utils/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/_is_sorted_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    16455 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/aggregation_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/az_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/categorizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/decode_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/totals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/experimental.py
--rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/json_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/message_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/message_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/message_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/message_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22242 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/path_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/perfect_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    28895 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/script_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/sse_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/stream_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/stream_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/stream_utils/stream_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/total_category_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/viewer_structs/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/viewer_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-04-16 08:22:10.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/viewer_structs/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 08:23:11.000000 th2_data_services-2.0.0.dev8702324290/th2_data_services.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:31:21.000000 th2_data_services-2.0.0.dev8702438320/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-04-16 08:31:21.000000 th2_data_services-2.0.0.dev8702438320/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    35047 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 08:31:08.000000 th2_data_services-2.0.0.dev8702438320/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 08:31:21.000000 th2_data_services-2.0.0.dev8702438320/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:31:21.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:31:21.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/_internal/perf_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:31:21.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41567 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:31:21.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/dummy/data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:31:21.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/event_tree/etc_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/event_tree/event_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26246 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/event_tree/event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/event_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/event_tree/parent_event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:31:21.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/interfaces/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/interfaces/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/interfaces/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:31:21.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/interfaces/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/interfaces/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/interfaces/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/interfaces/utils/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:31:21.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/_is_sorted_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16455 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/aggregation_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/az_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/categorizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/decode_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:31:21.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/event_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/event_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/event_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/event_utils/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/event_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/event_utils/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/event_utils/totals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/json_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:31:21.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/message_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/message_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/message_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/message_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22242 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/path_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/perfect_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28895 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/script_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/sse_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:31:21.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/stream_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/stream_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/stream_utils/stream_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/total_category_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:31:21.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/viewer_structs/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/viewer_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-04-16 08:30:18.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/viewer_structs/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:31:21.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-04-16 08:31:20.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-16 08:31:21.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:31:20.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-16 08:31:20.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 08:31:20.000000 th2_data_services-2.0.0.dev8702438320/th2_data_services.egg-info/top_level.txt
```

### Comparing `th2_data_services-2.0.0.dev8702324290/PKG-INFO` & `th2_data_services-2.0.0.dev8702438320/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 325f  : 2.1.Name: th2_
 00000020: 6461 7461 5f73 6572 7669 6365 730a 5665  data_services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3837 3032 3332 3432 3930 0a53 756d 6d61  8702324290.Summa
+00000040: 3837 3032 3433 3833 3230 0a53 756d 6d61  8702438320.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev8702324290/README.md` & `th2_data_services-2.0.0.dev8702438320/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/setup.py` & `th2_data_services-2.0.0.dev8702438320/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/_internal/__init__.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/_internal/perf_tests.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/_internal/perf_tests.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/config/__init__.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/config/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/config/config.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/config/config.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/data.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/data.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/dummy/__init__.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/dummy/data_source.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/dummy/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/__init__.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/etc_driver.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/event_tree/etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/event_tree.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/event_tree/event_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/event_tree_collection.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/event_tree/event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/exceptions.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/event_tree/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/event_tree/parent_event_tree_collection.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/event_tree/parent_event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/exceptions.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/__init__.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/adapter.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/command.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/data_source.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/source_api.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/struct.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/interfaces/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/stub_builder.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/interfaces/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/utils/__init__.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/interfaces/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/utils/converter.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/interfaces/utils/converter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/interfaces/utils/resolver.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/interfaces/utils/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/_is_sorted_result.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/_is_sorted_result.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/_json.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/_json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/_types.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/_types.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/aggregation_classes.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/aggregation_classes.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/az_tree.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/az_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/categorizers.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/categorizers.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/category.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/category.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/converters.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/converters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/decode_error_handler.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/decode_error_handler.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/display.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/__init__.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/event_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/display.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/event_utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/event_utils.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/event_utils/event_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/frequencies.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/event_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/select.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/event_utils/select.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/event_utils/totals.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/event_utils/totals.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/experimental.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/experimental.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/json_tree.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/json_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/message_utils/__init__.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/message_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/message_utils/frequencies.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/message_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/message_utils/message_utils.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/message_utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/misc_utils.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/path_utils.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/perfect_table.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/perfect_table.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/script_report_utils.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/script_report_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/sse_client.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/stream_utils/__init__.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/stream_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/stream_utils/stream_utils.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/stream_utils/stream_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/time.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/time.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/total_category_calculator.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/total_category_calculator.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/viewer_structs/__init__.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/viewer_structs/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services/utils/viewer_structs/verification.py` & `th2_data_services-2.0.0.dev8702438320/th2_data_services/utils/viewer_structs/verification.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services.egg-info/PKG-INFO` & `th2_data_services-2.0.0.dev8702438320/th2_data_services.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 322d  : 2.1.Name: th2-
 00000020: 6461 7461 2d73 6572 7669 6365 730a 5665  data-services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3837 3032 3332 3432 3930 0a53 756d 6d61  8702324290.Summa
+00000040: 3837 3032 3433 3833 3230 0a53 756d 6d61  8702438320.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services.egg-info/SOURCES.txt` & `th2_data_services-2.0.0.dev8702438320/th2_data_services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8702324290/th2_data_services.egg-info/requires.txt` & `th2_data_services-2.0.0.dev8702438320/th2_data_services.egg-info/requires.txt`

 * *Files identical despite different names*

