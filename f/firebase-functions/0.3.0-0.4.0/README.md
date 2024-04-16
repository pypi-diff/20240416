# Comparing `tmp/firebase_functions-0.3.0.tar.gz` & `tmp/firebase_functions-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firebase_functions-0.3.0.tar", last modified: Tue Apr  9 14:44:12 2024, max compression
+gzip compressed data, was "firebase_functions-0.4.0.tar", last modified: Tue Apr 16 15:19:01 2024, max compression
```

## Comparing `firebase_functions-0.3.0.tar` & `firebase_functions-0.4.0.tar`

### file list

```diff
@@ -1,62 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:44:12.838958 firebase_functions-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-09 14:44:12.838958 firebase_functions-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 14:44:12.838958 firebase_functions-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:44:12.830958 firebase_functions-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:44:12.834958 firebase_functions-0.3.0/src/firebase_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:44:12.834958 firebase_functions-0.3.0/src/firebase_functions/alerts/
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7046 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/alerts/app_distribution_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/alerts/billing_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14187 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/alerts/crashlytics_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/alerts/performance_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/alerts_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10528 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/db_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/eventarc_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)    21756 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/firestore_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/https_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/identity_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    38950 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    13317 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:44:12.834958 firebase_functions-0.3.0/src/firebase_functions/private/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/private/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/private/_alerts_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14003 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/private/_identity_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/private/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/private/path_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/private/serving.py
--rw-r--r--   0 runner    (1001) docker     (127)     9681 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/private/token_verifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/private/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/pubsub_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/remote_config_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/scheduler_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/storage_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/tasks_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/src/firebase_functions/test_lab_fn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:44:12.834958 firebase_functions-0.3.0/src/firebase_functions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-09 14:44:12.000000 firebase_functions-0.3.0/src/firebase_functions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-09 14:44:12.000000 firebase_functions-0.3.0/src/firebase_functions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:44:12.000000 firebase_functions-0.3.0/src/firebase_functions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-09 14:44:12.000000 firebase_functions-0.3.0/src/firebase_functions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 14:44:12.000000 firebase_functions-0.3.0/src/firebase_functions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:44:12.838958 firebase_functions-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/tests/test_eventarc_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/tests/test_firestore_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/tests/test_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/tests/test_path_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/tests/test_pubsub_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/tests/test_remote_config_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/tests/test_scheduler_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/tests/test_tasks_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/tests/test_test_lab_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-04-09 14:43:45.000000 firebase_functions-0.3.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:19:01.489246 firebase_functions-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-16 15:19:01.489246 firebase_functions-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:19:01.489246 firebase_functions-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:19:01.481245 firebase_functions-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:19:01.481245 firebase_functions-0.4.0/src/firebase_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:19:01.485245 firebase_functions-0.4.0/src/firebase_functions/alerts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7046 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/alerts/app_distribution_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/alerts/billing_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14187 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/alerts/crashlytics_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/alerts/performance_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/alerts_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10546 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/db_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/eventarc_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21791 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/firestore_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16604 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/https_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/identity_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38950 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13317 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:19:01.485245 firebase_functions-0.4.0/src/firebase_functions/private/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/private/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/private/_alerts_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14065 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/private/_identity_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/private/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/private/path_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/private/serving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9681 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/private/token_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/private/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/pubsub_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/remote_config_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/scheduler_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12972 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/storage_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/tasks_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8062 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/test_lab_fn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:19:01.485245 firebase_functions-0.4.0/src/firebase_functions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-16 15:19:01.000000 firebase_functions-0.4.0/src/firebase_functions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-16 15:19:01.000000 firebase_functions-0.4.0/src/firebase_functions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:19:01.000000 firebase_functions-0.4.0/src/firebase_functions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-16 15:19:01.000000 firebase_functions-0.4.0/src/firebase_functions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-16 15:19:01.000000 firebase_functions-0.4.0/src/firebase_functions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:19:01.489246 firebase_functions-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_eventarc_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_firestore_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_https_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_identity_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_path_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_pubsub_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_remote_config_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_scheduler_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_storage_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_tasks_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_test_lab_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_util.py
```

### Comparing `firebase_functions-0.3.0/LICENSE` & `firebase_functions-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/PKG-INFO` & `firebase_functions-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebase_functions
-Version: 0.3.0
+Version: 0.4.0
 Summary: Firebase Functions Python SDK
 Home-page: https://github.com/firebase/firebase-functions-python
 Author: Firebase Team
 License: Apache License 2.0
 Keywords: firebase,functions,google,cloud
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `firebase_functions-0.3.0/README.md` & `firebase_functions-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/setup.py` & `firebase_functions-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/src/firebase_functions/__init__.py` & `firebase_functions-0.4.0/src/firebase_functions/private/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,11 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-Firebase Functions for Python.
+Firebase Functions for Python - Private/Internals
 """
-
-__version__ = "0.3.0"
```

### Comparing `firebase_functions-0.3.0/src/firebase_functions/alerts/__init__.py` & `firebase_functions-0.4.0/src/firebase_functions/alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/src/firebase_functions/alerts/app_distribution_fn.py` & `firebase_functions-0.4.0/src/firebase_functions/alerts/app_distribution_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/src/firebase_functions/alerts/billing_fn.py` & `firebase_functions-0.4.0/src/firebase_functions/alerts/billing_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/src/firebase_functions/alerts/crashlytics_fn.py` & `firebase_functions-0.4.0/src/firebase_functions/alerts/crashlytics_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/src/firebase_functions/alerts/performance_fn.py` & `firebase_functions-0.4.0/src/firebase_functions/alerts/performance_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/src/firebase_functions/alerts_fn.py` & `firebase_functions-0.4.0/src/firebase_functions/alerts_fn.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import functools as _functools
 import typing as _typing
 import cloudevents.http as _ce
 from firebase_functions.alerts import FirebaseAlertData
 
 import firebase_functions.private.util as _util
 
-from firebase_functions.core import T, CloudEvent as _CloudEvent
+from firebase_functions.core import T, CloudEvent as _CloudEvent, _with_init
 from firebase_functions.options import FirebaseAlertOptions
 
 # Explicitly import AlertType to make it available in the public API.
 # pylint: disable=unused-import
 from firebase_functions.options import AlertType
 
 
@@ -91,15 +91,15 @@
     options = FirebaseAlertOptions(**kwargs)
 
     def on_alert_published_inner_decorator(func: OnAlertPublishedCallable):
 
         @_functools.wraps(func)
         def on_alert_published_wrapped(raw: _ce.CloudEvent):
             from firebase_functions.private._alerts_fn import alerts_event_from_ce
-            func(alerts_event_from_ce(raw))
+            _with_init(func)(alerts_event_from_ce(raw))
 
         _util.set_func_endpoint_attr(
             on_alert_published_wrapped,
             options._endpoint(func_name=func.__name__),
         )
         return on_alert_published_wrapped
```

### Comparing `firebase_functions-0.3.0/src/firebase_functions/core.py` & `firebase_functions-0.4.0/src/firebase_functions/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 """
 Public code that is shared across modules.
 """
 import dataclasses as _dataclass
 import datetime as _datetime
 import typing as _typing
 
+from . import logger as _logger
+
 T = _typing.TypeVar("T")
 
 
 @_dataclass.dataclass(frozen=True)
 class CloudEvent(_typing.Generic[T]):
     """
     A CloudEvent is the base of a cross-platform format for encoding a serverless event.
@@ -76,7 +78,50 @@
     The state of data before the change.
     """
 
     after: T
     """
     The state of data after the change.
     """
+
+
+_did_init = False
+_init_callback: _typing.Callable[[], _typing.Any] | None = None
+
+
+def init(callback: _typing.Callable[[], _typing.Any]) -> None:
+    """
+     Registers a function that should be run when in a production environment
+     before executing any functions code.
+     Calling this decorator more than once leads to undefined behavior.
+    """
+
+    global _did_init
+    global _init_callback
+
+    if _did_init:
+        _logger.warn(
+            "Setting init callback more than once. Only the most recent callback will be called"
+        )
+
+    _init_callback = callback
+    _did_init = False
+
+
+def _with_init(
+    fn: _typing.Callable[...,
+                         _typing.Any]) -> _typing.Callable[..., _typing.Any]:
+    """
+    A decorator that runs the init callback before running the decorated function.
+    """
+
+    def wrapper(*args, **kwargs):
+        global _did_init
+
+        if not _did_init:
+            if _init_callback is not None:
+                _init_callback()
+            _did_init = True
+
+        return fn(*args, **kwargs)
+
+    return wrapper
```

### Comparing `firebase_functions-0.3.0/src/firebase_functions/db_fn.py` & `firebase_functions-0.4.0/src/firebase_functions/db_fn.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
             event_attributes["time"],
             "%Y-%m-%dT%H:%M:%S.%f%z",
         ),
         data=database_event_data,
         subject=event_attributes["subject"],
         params=params,
     )
-    func(database_event)
+    _core._with_init(func)(database_event)
 
 
 @_util.copy_func_kwargs(DatabaseOptions)
 def on_value_written(**kwargs) -> _typing.Callable[[_C1], _C1]:
     """
     Event handler that triggers when data is created, updated, or deleted in Realtime Database.
```

### Comparing `firebase_functions-0.3.0/src/firebase_functions/eventarc_fn.py` & `firebase_functions-0.4.0/src/firebase_functions/eventarc_fn.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import typing as _typing
 import functools as _functools
 import datetime as _dt
 import cloudevents.http as _ce
 
 import firebase_functions.options as _options
 import firebase_functions.private.util as _util
-from firebase_functions.core import CloudEvent
+from firebase_functions.core import CloudEvent, _with_init
 
 
 @_util.copy_func_kwargs(_options.EventarcTriggerOptions)
 def on_custom_event_published(
     **kwargs
 ) -> _typing.Callable[[_typing.Callable[[CloudEvent], None]], _typing.Callable[
     [CloudEvent], None]]:
@@ -69,15 +69,15 @@
                 if "subject" in event_dict else None,
                 time=_dt.datetime.strptime(
                     event_dict["time"],
                     "%Y-%m-%dT%H:%M:%S.%f%z",
                 ),
                 type=event_dict["type"],
             )
-            func(event)
+            _with_init(func)(event)
 
         _util.set_func_endpoint_attr(
             on_custom_event_published_wrapped,
             options._endpoint(func_name=func.__name__),
         )
         _util.set_required_apis_attr(
             on_custom_event_published_wrapped,
```

### Comparing `firebase_functions-0.3.0/src/firebase_functions/firestore_fn.py` & `firebase_functions-0.4.0/src/firebase_functions/firestore_fn.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,14 +201,16 @@
         type=event_attributes["type"],
         time=event_time,
         data=firestore_event_data,
         subject=event_attributes["subject"],
         params=params,
     )
 
+    func = _core._with_init(func)
+
     if event_type.endswith(".withAuthContext"):
         database_event_with_auth_context = AuthEvent(**vars(database_event),
                                                      auth_type=event_auth_type,
                                                      auth_id=event_auth_id)
         func(database_event_with_auth_context)
     else:
         # mypy cannot infer that the event type is correct, hence the cast
```

### Comparing `firebase_functions-0.3.0/src/firebase_functions/https_fn.py` & `firebase_functions-0.4.0/src/firebase_functions/https_fn.py`

 * *Files 1% similar despite different names*

```diff
@@ -399,15 +399,15 @@
             # Currently, the only real use case for this token is for sending
             # pushes with FCM. In that case, the FCM APIs will validate the token.
             context = _dataclasses.replace(
                 context,
                 instance_id_token=request.headers.get(
                     "Firebase-Instance-ID-Token"),
             )
-        result = func(context)
+        result = _core._with_init(func)(context)
         return _jsonify(result=result)
     # Disable broad exceptions lint since we want to handle all exceptions here
     # and wrap as an HttpsError.
     # pylint: disable=broad-except
     except Exception as err:
         if not isinstance(err, HttpsError):
             _logging.error("Unhandled error: %s", err)
@@ -443,15 +443,15 @@
         @_functools.wraps(func)
         def on_request_wrapped(request: Request) -> Response:
             if options.cors is not None:
                 return _cross_origin(
                     methods=options.cors.cors_methods,
                     origins=options.cors.cors_origins,
                 )(func)(request)
-            return func(request)
+            return _core._with_init(func)(request)
 
         _util.set_func_endpoint_attr(
             on_request_wrapped,
             options._endpoint(func_name=func.__name__),
         )
         return on_request_wrapped
```

### Comparing `firebase_functions-0.3.0/src/firebase_functions/identity_fn.py` & `firebase_functions-0.4.0/src/firebase_functions/identity_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/src/firebase_functions/logger.py` & `firebase_functions-0.4.0/src/firebase_functions/logger.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/src/firebase_functions/options.py` & `firebase_functions-0.4.0/src/firebase_functions/options.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/src/firebase_functions/params.py` & `firebase_functions-0.4.0/src/firebase_functions/params.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/src/firebase_functions/private/__init__.py` & `firebase_functions-0.4.0/src/firebase_functions/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,9 +8,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-Firebase Functions for Python - Private/Internals
+Firebase Functions for Python.
 """
+
+__version__ = "0.4.0"
```

### Comparing `firebase_functions-0.3.0/src/firebase_functions/private/_alerts_fn.py` & `firebase_functions-0.4.0/src/firebase_functions/private/_alerts_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/src/firebase_functions/private/_identity_fn.py` & `firebase_functions-0.4.0/src/firebase_functions/private/_identity_fn.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Cloud functions to handle Eventarc events."""
-
 # pylint: disable=protected-access
 import typing as _typing
 import datetime as _dt
 import time as _time
 import json as _json
+
+from firebase_functions.core import _with_init
 from firebase_functions.https_fn import HttpsError, FunctionsErrorCode
 
 import firebase_functions.private.util as _util
 import firebase_functions.private.token_verifier as _token_verifier
 from flask import (
     Request as _Request,
     Response as _Response,
@@ -347,22 +348,22 @@
             raise HttpsError(FunctionsErrorCode.INVALID_ARGUMENT, "Bad Request")
         if request.json is None or "data" not in request.json:
             _logging.error("Request body is missing data.", request.json)
             raise HttpsError(FunctionsErrorCode.INVALID_ARGUMENT, "Bad Request")
         jwt_token = request.json["data"]["jwt"]
         decoded_token = _token_verifier.verify_auth_blocking_token(jwt_token)
         event = _auth_blocking_event_from_token_data(decoded_token)
-        auth_response: BeforeCreateResponse | BeforeSignInResponse | None = func(
-            event)
+        auth_response: BeforeCreateResponse | BeforeSignInResponse | None = _with_init(
+            func)(event)
         if not auth_response:
             return _jsonify({})
         auth_response_dict = _validate_auth_response(event_type, auth_response)
         result = _generate_response_payload(auth_response_dict)
         return _jsonify(result)
     # Disable broad exceptions lint since we want to handle all exceptions.
     # pylint: disable=broad-except
     except Exception as exception:
         if not isinstance(exception, HttpsError):
-            _logging.error("Unhandled error", exception)
+            _logging.error("Unhandled error %s", exception)
             exception = HttpsError(FunctionsErrorCode.INTERNAL, "INTERNAL")
         status = exception._http_error_code.status
         return _make_response(_jsonify(error=exception._as_dict()), status)
```

### Comparing `firebase_functions-0.3.0/src/firebase_functions/private/manifest.py` & `firebase_functions-0.4.0/src/firebase_functions/private/manifest.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/src/firebase_functions/private/path_pattern.py` & `firebase_functions-0.4.0/src/firebase_functions/private/path_pattern.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/src/firebase_functions/private/serving.py` & `firebase_functions-0.4.0/src/firebase_functions/private/serving.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/src/firebase_functions/private/token_verifier.py` & `firebase_functions-0.4.0/src/firebase_functions/private/token_verifier.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/src/firebase_functions/private/util.py` & `firebase_functions-0.4.0/src/firebase_functions/private/util.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/src/firebase_functions/pubsub_fn.py` & `firebase_functions-0.4.0/src/firebase_functions/pubsub_fn.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import typing as _typing
 import json as _json
 import base64 as _base64
 import cloudevents.http as _ce
 
 import firebase_functions.private.util as _util
 
-from firebase_functions.core import CloudEvent, T
+from firebase_functions.core import CloudEvent, T, _with_init
 from firebase_functions.options import PubSubOptions
 
 
 @_dataclasses.dataclass(frozen=True)
 class Message(_typing.Generic[T]):
     """
     Interface representing a Google Cloud Pub/Sub message.
@@ -147,15 +147,15 @@
         source=event_dict["source"],
         specversion=event_dict["specversion"],
         subject=event_dict["subject"] if "subject" in event_dict else None,
         time=event_dict["time"],
         type=event_dict["type"],
     )
 
-    func(event)
+    _with_init(func)(event)
 
 
 @_util.copy_func_kwargs(PubSubOptions)
 def on_message_published(**kwargs) -> _typing.Callable[[_C1], _C1]:
     """
     Event handler that triggers on a message being published to a Pub/Sub topic.
```

### Comparing `firebase_functions-0.3.0/src/firebase_functions/remote_config_fn.py` & `firebase_functions-0.4.0/src/firebase_functions/remote_config_fn.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import datetime as _dt
 import typing as _typing
 import cloudevents.http as _ce
 import enum as _enum
 
 import firebase_functions.private.util as _util
 
-from firebase_functions.core import CloudEvent
+from firebase_functions.core import CloudEvent, _with_init
 from firebase_functions.options import EventHandlerOptions
 
 
 @_dataclasses.dataclass(frozen=True)
 class ConfigUser:
     """
     All the fields associated with the person/service account that wrote a Remote Config template.
@@ -185,15 +185,15 @@
         time=_dt.datetime.strptime(
             event_dict["time"],
             "%Y-%m-%dT%H:%M:%S.%f%z",
         ),
         type=event_dict["type"],
     )
 
-    func(event)
+    _with_init(func)(event)
 
 
 @_util.copy_func_kwargs(EventHandlerOptions)
 def on_config_updated(**kwargs) -> _typing.Callable[[_C1], _C1]:
     """
     Event handler which triggers when data is updated in a Remote Config.
```

### Comparing `firebase_functions-0.3.0/src/firebase_functions/scheduler_fn.py` & `firebase_functions-0.4.0/src/firebase_functions/scheduler_fn.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from functions_framework import logging as _logging
 from flask import (
     Request as _Request,
     Response as _Response,
     make_response as _make_response,
 )
 
+from firebase_functions.core import _with_init
 # Export for user convenience.
 # pylint: disable=unused-import
 from firebase_functions.options import Timezone
 
 
 @_dataclasses.dataclass(frozen=True)
 class ScheduledEvent:
@@ -104,15 +105,15 @@
                     "%Y-%m-%dT%H:%M:%S%z",
                 )
             event = ScheduledEvent(
                 job_name=request.headers.get("X-CloudScheduler-JobName"),
                 schedule_time=schedule_time,
             )
             try:
-                func(event)
+                _with_init(func)(event)
                 return _make_response()
             # Disable broad exceptions lint since we want to handle all exceptions.
             # pylint: disable=broad-except
             except Exception as exception:
                 _logging.exception(exception)
                 return _make_response(str(exception), 500)
```

### Comparing `firebase_functions-0.3.0/src/firebase_functions/storage_fn.py` & `firebase_functions-0.4.0/src/firebase_functions/storage_fn.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import dataclasses as _dataclasses
 import datetime as _dt
 import functools as _functools
 import typing as _typing
 import cloudevents.http as _ce
 
 import firebase_functions.private.util as _util
-from firebase_functions.core import CloudEvent
+from firebase_functions.core import CloudEvent, _with_init
 from firebase_functions.options import StorageOptions
 
 _event_type_archived = "google.cloud.storage.object.v1.archived"
 _event_type_finalized = "google.cloud.storage.object.v1.finalized"
 _event_type_deleted = "google.cloud.storage.object.v1.deleted"
 _event_type_metadata_updated = "google.cloud.storage.object.v1.metadataUpdated"
 
@@ -251,15 +251,15 @@
         time=_dt.datetime.strptime(
             event_attributes["time"],
             "%Y-%m-%dT%H:%M:%S.%f%z",
         ),
         type=event_attributes["type"],
     )
 
-    func(event)
+    _with_init(func)(event)
 
 
 @_util.copy_func_kwargs(StorageOptions)
 def on_object_archived(**kwargs) -> _typing.Callable[[_C1], _C1]:
     """
     Event handler sent only when a bucket has enabled object versioning.
     This event indicates that the live version of an object has become an
```

### Comparing `firebase_functions-0.3.0/src/firebase_functions/tasks_fn.py` & `firebase_functions-0.4.0/src/firebase_functions/tasks_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/src/firebase_functions/test_lab_fn.py` & `firebase_functions-0.4.0/src/firebase_functions/test_lab_fn.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import datetime as _dt
 import typing as _typing
 import cloudevents.http as _ce
 import enum as _enum
 
 import firebase_functions.private.util as _util
 
-from firebase_functions.core import CloudEvent
+from firebase_functions.core import CloudEvent, _with_init
 from firebase_functions.options import EventHandlerOptions
 
 
 class TestState(str, _enum.Enum):
     """
     Possible test states for a test matrix.
     """
@@ -242,15 +242,15 @@
         time=_dt.datetime.strptime(
             event_dict["time"],
             "%Y-%m-%dT%H:%M:%S.%f%z",
         ),
         type=event_dict["type"],
     )
 
-    func(event)
+    _with_init(func)(event)
 
 
 @_util.copy_func_kwargs(EventHandlerOptions)
 def on_test_matrix_completed(**kwargs) -> _typing.Callable[[_C1], _C1]:
     """
     Event handler which triggers when a Firebase test matrix completes.
```

### Comparing `firebase_functions-0.3.0/src/firebase_functions.egg-info/PKG-INFO` & `firebase_functions-0.4.0/src/firebase_functions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebase-functions
-Version: 0.3.0
+Version: 0.4.0
 Summary: Firebase Functions Python SDK
 Home-page: https://github.com/firebase/firebase-functions-python
 Author: Firebase Team
 License: Apache License 2.0
 Keywords: firebase,functions,google,cloud
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `firebase_functions-0.3.0/src/firebase_functions.egg-info/SOURCES.txt` & `firebase_functions-0.4.0/src/firebase_functions.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -34,20 +34,25 @@
 src/firebase_functions/private/_alerts_fn.py
 src/firebase_functions/private/_identity_fn.py
 src/firebase_functions/private/manifest.py
 src/firebase_functions/private/path_pattern.py
 src/firebase_functions/private/serving.py
 src/firebase_functions/private/token_verifier.py
 src/firebase_functions/private/util.py
+tests/test_db.py
 tests/test_eventarc_fn.py
 tests/test_firestore_fn.py
+tests/test_https_fn.py
+tests/test_identity_fn.py
+tests/test_init.py
 tests/test_logger.py
 tests/test_manifest.py
 tests/test_options.py
 tests/test_params.py
 tests/test_path_pattern.py
 tests/test_pubsub_fn.py
 tests/test_remote_config_fn.py
 tests/test_scheduler_fn.py
+tests/test_storage_fn.py
 tests/test_tasks_fn.py
 tests/test_test_lab_fn.py
 tests/test_util.py
```

### Comparing `firebase_functions-0.3.0/tests/test_eventarc_fn.py` & `firebase_functions-0.4.0/tests/test_eventarc_fn.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Eventarc trigger function tests."""
 import unittest
 from unittest.mock import Mock
+
 from cloudevents.http import CloudEvent as _CloudEvent
+
+from firebase_functions import core
 from firebase_functions.core import CloudEvent
 from firebase_functions.eventarc_fn import on_custom_event_published
 
 
 class TestEventarcFn(unittest.TestCase):
     """
     Test Eventarc trigger functions.
@@ -79,7 +82,38 @@
         self.assertEqual(event_arg.source, "https://example.com/testevent")
         self.assertEqual(event_arg.specversion, "1.0")
         self.assertEqual(event_arg.subject, "test_subject")
         self.assertEqual(
             event_arg.type,
             "firebase.extensions.storage-resize-images.v1.complete",
         )
+
+    def test_calls_init_function(self):
+        hello = None
+
+        @core.init
+        def init():
+            nonlocal hello
+            hello = "world"
+
+        func = Mock(__name__="example_func")
+        raw_event = _CloudEvent(
+            attributes={
+                "specversion": "1.0",
+                "type": "firebase.extensions.storage-resize-images.v1.complete",
+                "source": "https://example.com/testevent",
+                "id": "1234567890",
+                "subject": "test_subject",
+                "time": "2023-03-11T13:25:37.403Z",
+            },
+            data={
+                "some_key": "some_value",
+            },
+        )
+
+        decorated_func = on_custom_event_published(
+            event_type="firebase.extensions.storage-resize-images.v1.complete",
+        )(func)
+
+        decorated_func(raw_event)
+
+        self.assertEqual(hello, "world")
```

### Comparing `firebase_functions-0.3.0/tests/test_firestore_fn.py` & `firebase_functions-0.4.0/tests/test_remote_config_fn.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,90 @@
-"""
-This module contains tests for the firestore_fn module.
-"""
-
-import json
-from unittest import TestCase
-from unittest.mock import MagicMock, Mock, patch
-
-mocked_modules = {
-    "google.cloud.firestore": MagicMock(),
-    "google.cloud.firestore_v1": MagicMock(),
-    "firebase_admin": MagicMock()
-}
+# Copyright 2022 Google Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+"""Remote Config function tests."""
+import unittest
+from unittest.mock import MagicMock
+from cloudevents.http import CloudEvent as _CloudEvent
+
+from firebase_functions.remote_config_fn import (
+    CloudEvent,
+    ConfigUser,
+    ConfigUpdateData,
+    ConfigUpdateOrigin,
+    ConfigUpdateType,
+    on_config_updated,
+    _config_handler,
+)
 
 
-class TestFirestore(TestCase):
+class TestRemoteConfig(unittest.TestCase):
     """
-    firestore_fn tests.
+    Remote Config function tests.
     """
 
-    def test_firestore_endpoint_handler_calls_function_with_correct_args(self):
-        with patch.dict("sys.modules", mocked_modules):
-            from cloudevents.http import CloudEvent
-            from firebase_functions.firestore_fn import _event_type_created_with_auth_context as event_type, \
-                _firestore_endpoint_handler as firestore_endpoint_handler, AuthEvent
-            from firebase_functions.private import path_pattern
-
-            func = Mock(__name__="example_func")
-
-            document_pattern = path_pattern.PathPattern("foo/{bar}")
-            attributes = {
-                "specversion":
-                    "1.0",
-                "type":
-                    event_type,
-                "source":
-                    "https://example.com/testevent",
-                "time":
-                    "2023-03-11T13:25:37.403Z",
-                "subject":
-                    "test_subject",
-                "datacontenttype":
-                    "application/json",
-                "location":
-                    "projects/project-id/databases/(default)/documents/foo/{bar}",
-                "project":
-                    "project-id",
-                "namespace":
-                    "(default)",
-                "document":
-                    "foo/{bar}",
-                "database":
-                    "projects/project-id/databases/(default)",
-                "authtype":
-                    "unauthenticated",
-                "authid":
-                    "foo"
-            }
-            raw_event = CloudEvent(attributes=attributes, data=json.dumps({}))
-
-            firestore_endpoint_handler(func=func,
-                                       event_type=event_type,
-                                       document_pattern=document_pattern,
-                                       raw=raw_event)
-
-            func.assert_called_once()
-
-            event = func.call_args.args[0]
-            self.assertIsNotNone(event)
-            self.assertIsInstance(event, AuthEvent)
-            self.assertEqual(event.auth_type, "unauthenticated")
-            self.assertEqual(event.auth_id, "foo")
+    def test_on_config_updated_decorator(self):
+        """
+        Tests the on_config_updated decorator functionality by checking
+        that the __firebase_endpoint__ attribute is set properly.
+        """
+        func = MagicMock()
+        func.__name__ = "testfn"
+        decorated_func = on_config_updated()(func)
+        endpoint = getattr(decorated_func, "__firebase_endpoint__")
+        self.assertIsNotNone(endpoint)
+        self.assertIsNotNone(endpoint.eventTrigger)
+        self.assertIsNotNone(endpoint.eventTrigger["eventType"])
+
+    def test_config_handler(self):
+        """
+        Tests the _config_handler function, ensuring that it correctly processes
+        the raw event and calls the user-provided function with a properly
+        formatted CloudEvent instance.
+        """
+        func = MagicMock()
+        raw_event = _CloudEvent(
+            attributes={
+                "specversion": "1.0",
+                "type": "com.example.someevent",
+                "source": "https://example.com/someevent",
+                "id": "A234-1234-1234",
+                "time": "2023-03-11T13:25:37.403Z",
+            },
+            data={
+                "versionNumber": 42,
+                "updateTime": "2023-03-11T13:25:37.403Z",
+                "updateUser": {
+                    "name": "John Doe",
+                    "email": "johndoe@example.com",
+                    "imageUrl": "https://example.com/image.jpg"
+                },
+                "description": "Test update",
+                "updateOrigin": "CONSOLE",
+                "updateType": "INCREMENTAL_UPDATE",
+                "rollbackSource": 41
+            })
+
+        _config_handler(func, raw_event)
+
+        func.assert_called_once()
+
+        event_arg = func.call_args.args[0]
+        self.assertIsInstance(event_arg, CloudEvent)
+        self.assertIsInstance(event_arg.data, ConfigUpdateData)
+        self.assertIsInstance(event_arg.data.update_user, ConfigUser)
+        self.assertEqual(event_arg.data.version_number, 42)
+        self.assertEqual(event_arg.data.update_origin,
+                         ConfigUpdateOrigin.CONSOLE)
+        self.assertEqual(event_arg.data.update_type,
+                         ConfigUpdateType.INCREMENTAL_UPDATE)
+        self.assertEqual(event_arg.data.rollback_source, 41)
```

### Comparing `firebase_functions-0.3.0/tests/test_logger.py` & `firebase_functions-0.4.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/tests/test_manifest.py` & `firebase_functions-0.4.0/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/tests/test_options.py` & `firebase_functions-0.4.0/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/tests/test_params.py` & `firebase_functions-0.4.0/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/tests/test_path_pattern.py` & `firebase_functions-0.4.0/tests/test_path_pattern.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.3.0/tests/test_pubsub_fn.py` & `firebase_functions-0.4.0/tests/test_pubsub_fn.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 """PubSub function tests."""
 import unittest
 import datetime as _dt
 from unittest.mock import MagicMock
 from cloudevents.http import CloudEvent as _CloudEvent
 
+from firebase_functions import core
 from firebase_functions.pubsub_fn import (
     Message,
     MessagePublishedData,
     on_message_published,
     _message_handler,
     CloudEvent,
 )
@@ -90,7 +91,41 @@
             ))
         self.assertDictEqual(event_arg.data.message.attributes,
                              {"key": "value"})
         self.assertEqual(event_arg.data.message.data,
                          "eyJ0ZXN0IjogInZhbHVlIn0=")
         self.assertIsNone(event_arg.data.message.ordering_key)
         self.assertEqual(event_arg.data.subscription, "my-subscription")
+
+    def test_calls_init(self):
+        hello = None
+
+        @core.init
+        def init():
+            nonlocal hello
+            hello = "world"
+
+        func = MagicMock()
+        raw_event = _CloudEvent(
+            attributes={
+                "id": "test-message",
+                "source": "https://example.com/pubsub",
+                "specversion": "1.0",
+                "time": "2023-03-11T13:25:37.403Z",
+                "type": "com.example.pubsub.message",
+            },
+            data={
+                "message": {
+                    "attributes": {
+                        "key": "value"
+                    },
+                    "data": "eyJ0ZXN0IjogInZhbHVlIn0=",
+                    "message_id": "message-id-123",
+                    "publish_time": "2023-03-11T13:25:37.403Z",
+                },
+                "subscription": "my-subscription",
+            },
+        )
+
+        _message_handler(func, raw_event)
+
+        self.assertEqual("world", hello)
```

### Comparing `firebase_functions-0.3.0/tests/test_scheduler_fn.py` & `firebase_functions-0.4.0/tests/test_scheduler_fn.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 """Scheduler function tests."""
 import unittest
 from unittest.mock import Mock
 from datetime import datetime
 from flask import Request, Flask
 from werkzeug.test import EnvironBuilder
-from firebase_functions import scheduler_fn
+from firebase_functions import scheduler_fn, core
 
 
 class TestScheduler(unittest.TestCase):
     """
     Scheduler function tests.
     """
 
@@ -114,7 +114,25 @@
                                 side_effect=Exception("Test exception"))
             decorated_func = scheduler_fn.on_schedule(
                 schedule="* * * * *")(example_func)
             response = decorated_func(mock_request)
 
             self.assertEqual(response.status_code, 500)
             self.assertEqual(response.data, b"Test exception")
+
+    def test_calls_init(self):
+        hello = None
+
+        @core.init
+        def init():
+            nonlocal hello
+            hello = "world"
+
+        with Flask(__name__).test_request_context("/"):
+            environ = EnvironBuilder().get_environ()
+            mock_request = Request(environ)
+            example_func = Mock(__name__="example_func")
+            decorated_func = scheduler_fn.on_schedule(
+                schedule="* * * * *")(example_func)
+            decorated_func(mock_request)
+
+            self.assertEqual("world", hello)
```

### Comparing `firebase_functions-0.3.0/tests/test_tasks_fn.py` & `firebase_functions-0.4.0/tests/test_tasks_fn.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Task Queue function tests."""
 import unittest
 
-from unittest.mock import MagicMock
+from unittest.mock import MagicMock, Mock
 from flask import Flask, Request
 from werkzeug.test import EnvironBuilder
+
+from firebase_functions import core
 from firebase_functions.tasks_fn import on_task_dispatched, CallableRequest
 
 
 class TestTasks(unittest.TestCase):
     """
     Task Queue function tests.
     """
@@ -99,7 +101,34 @@
                         "test": "value"
                     },
                 },
             ).get_environ()
             request = Request(environ)
             response = example(request)
             self.assertEqual(response.status_code, 200)
+
+    def test_calls_init(self):
+        hello = None
+
+        @core.init
+        def init():
+            nonlocal hello
+            hello = "world"
+
+        app = Flask(__name__)
+
+        func = Mock(__name__="example_func")
+
+        with app.test_request_context("/"):
+            environ = EnvironBuilder(
+                method="POST",
+                json={
+                    "data": {
+                        "test": "value"
+                    },
+                },
+            ).get_environ()
+            request = Request(environ)
+            decorated_func = on_task_dispatched()(func)
+            decorated_func(request)
+
+            self.assertEqual("world", hello)
```

### Comparing `firebase_functions-0.3.0/tests/test_test_lab_fn.py` & `firebase_functions-0.4.0/tests/test_test_lab_fn.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Test Lab function tests."""
 import unittest
-from unittest.mock import MagicMock
+from unittest.mock import MagicMock, Mock
 from cloudevents.http import CloudEvent as _CloudEvent
 
+from firebase_functions import core
 from firebase_functions.test_lab_fn import (
     CloudEvent,
     TestMatrixCompletedData,
     TestState,
     OutcomeSummary,
     ResultStorage,
     ClientInfo,
@@ -90,7 +91,52 @@
         self.assertIsInstance(event_arg, CloudEvent)
         self.assertIsInstance(event_arg.data, TestMatrixCompletedData)
         self.assertIsInstance(event_arg.data.result_storage, ResultStorage)
         self.assertIsInstance(event_arg.data.client_info, ClientInfo)
         self.assertEqual(event_arg.data.state, TestState.FINISHED)
         self.assertEqual(event_arg.data.outcome_summary, OutcomeSummary.SUCCESS)
         self.assertEqual(event_arg.data.test_matrix_id, "testmatrix-123")
+
+    def test_calls_init(self):
+        hello = None
+
+        @core.init
+        def init():
+            nonlocal hello
+            hello = "world"
+
+        func = Mock(__name__="example_func")
+        raw_event = _CloudEvent(
+            attributes={
+                "specversion": "1.0",
+                "type": "com.example.someevent",
+                "source": "https://example.com/someevent",
+                "id": "A234-1234-1234",
+                "time": "2023-03-11T13:25:37.403Z",
+            },
+            data={
+                "createTime": "2023-03-11T13:25:37.403Z",
+                "state": "FINISHED",
+                "invalidMatrixDetails": "Some details",
+                "outcomeSummary": "SUCCESS",
+                "resultStorage": {
+                    "toolResultsHistory":
+                        "projects/123/histories/456",
+                    "resultsUri":
+                        "https://example.com/results",
+                    "gcsPath":
+                        "gs://bucket/path/to/somewhere",
+                    "toolResultsExecution":
+                        "projects/123/histories/456/executions/789",
+                },
+                "clientInfo": {
+                    "client": "gcloud",
+                },
+                "testMatrixId": "testmatrix-123",
+            })
+
+        decorated_func = on_test_matrix_completed()(func)
+        decorated_func(raw_event)
+
+        func.assert_called_once()
+
+        self.assertEqual("world", hello)
```

### Comparing `firebase_functions-0.3.0/tests/test_util.py` & `firebase_functions-0.4.0/tests/test_util.py`

 * *Files identical despite different names*

