# Comparing `tmp/konfuzio_sdk-0.3.3.dev20240410112634.tar.gz` & `tmp/konfuzio_sdk-0.3.3.dev20240415090556.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konfuzio_sdk-0.3.3.dev20240410112634.tar", last modified: Thu Apr 11 03:25:46 2024, max compression
+gzip compressed data, was "konfuzio_sdk-0.3.3.dev20240415090556.tar", last modified: Tue Apr 16 03:26:56 2024, max compression
```

## Comparing `konfuzio_sdk-0.3.3.dev20240410112634.tar` & `konfuzio_sdk-0.3.3.dev20240415090556.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:25:46.696192 konfuzio_sdk-0.3.3.dev20240410112634/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-11 03:25:37.000000 konfuzio_sdk-0.3.3.dev20240410112634/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-04-11 03:25:46.696192 konfuzio_sdk-0.3.3.dev20240410112634/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-04-11 03:25:37.000000 konfuzio_sdk-0.3.3.dev20240410112634/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:25:46.688192 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33726 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)   202907 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    44747 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/extras.py
--rw-r--r--   0 runner    (1001) docker     (127)    27450 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)    27029 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/settings_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:25:46.688192 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13180 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/tokenizer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15231 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/tokenizer/paragraph_and_sentence.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/tokenizer/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:25:46.692192 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/trainer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    75617 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/trainer/document_categorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    51309 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/trainer/file_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/trainer/image.py
--rw-r--r--   0 runner    (1001) docker     (127)   101643 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/trainer/information_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/trainer/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/trainer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    37377 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:25:46.692192 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-04-11 03:25:46.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-11 03:25:46.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:25:46.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-11 03:25:46.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-11 03:25:46.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 03:25:46.000000 konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 03:25:46.696192 konfuzio_sdk-0.3.3.dev20240410112634/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:25:46.692192 konfuzio_sdk-0.3.3.dev20240410112634/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    22465 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)   167058 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    80271 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/tests/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/tests/test_extras.py
--rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/tests/test_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    41449 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/tests/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/tests/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/tests/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    20678 2024-04-11 03:25:38.000000 konfuzio_sdk-0.3.3.dev20240410112634/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:26:56.622106 konfuzio_sdk-0.3.3.dev20240415090556/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-04-16 03:26:56.622106 konfuzio_sdk-0.3.3.dev20240415090556/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:26:56.614107 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33726 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)   202907 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44747 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27450 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27029 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/settings_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:26:56.614107 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13180 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/tokenizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15231 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/tokenizer/paragraph_and_sentence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/tokenizer/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:26:56.614107 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75617 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/document_categorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51309 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/file_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101643 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/information_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37377 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:26:56.618106 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-04-16 03:26:56.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-16 03:26:56.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:26:56.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 03:26:56.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-16 03:26:56.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 03:26:56.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 03:26:56.622106 konfuzio_sdk-0.3.3.dev20240415090556/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:26:56.618106 konfuzio_sdk-0.3.3.dev20240415090556/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    22568 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)   167058 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80271 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/tests/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/tests/test_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/tests/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41449 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/tests/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/tests/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20678 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/tests/test_utils.py
```

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/LICENSE.md` & `konfuzio_sdk-0.3.3.dev20240415090556/LICENSE.md`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/PKG-INFO` & `konfuzio_sdk-0.3.3.dev20240415090556/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konfuzio_sdk
-Version: 0.3.3.dev20240410112634
+Version: 0.3.3.dev20240415090556
 Summary: Konfuzio Software Development Kit
 Home-page: https://github.com/konfuzio-ai/konfuzio-sdk/
 Author: Helm & Nagel GmbH
 Author-email: info@helm-nagel.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: certifi==2023.7.22
```

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/README.md` & `konfuzio_sdk-0.3.3.dev20240415090556/README.md`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/api.py` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/api.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/cli.py` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/data.py` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/data.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/evaluate.py` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/evaluate.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/extras.py` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/extras.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/normalize.py` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/normalize.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/regex.py` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/samples.py` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/samples.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/settings_importer.py` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/settings_importer.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/tokenizer/base.py` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/tokenizer/base.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/tokenizer/paragraph_and_sentence.py` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/tokenizer/paragraph_and_sentence.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/tokenizer/regex.py` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/tokenizer/regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/trainer/base.py` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/base.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/trainer/document_categorization.py` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/document_categorization.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/trainer/file_splitting.py` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/file_splitting.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/trainer/image.py` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/image.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/trainer/information_extraction.py` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/information_extraction.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/trainer/tokenization.py` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/tokenization.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/trainer/utils.py` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/urls.py` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/urls.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk/utils.py` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk.egg-info/PKG-INFO` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konfuzio_sdk
-Version: 0.3.3.dev20240410112634
+Version: 0.3.3.dev20240415090556
 Summary: Konfuzio Software Development Kit
 Home-page: https://github.com/konfuzio-ai/konfuzio-sdk/
 Author: Helm & Nagel GmbH
 Author-email: info@helm-nagel.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: certifi==2023.7.22
```

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk.egg-info/SOURCES.txt` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/konfuzio_sdk.egg-info/requires.txt` & `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/setup.py` & `konfuzio_sdk-0.3.3.dev20240415090556/setup.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/tests/test_api.py` & `konfuzio_sdk-0.3.3.dev20240415090556/tests/test_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Validate API functions."""
+
 import datetime
 import json
 import logging
 import os
 import sys
 import unittest
 from unittest.mock import patch
@@ -104,14 +105,15 @@
         data = get_meta_of_files(project_id=TEST_PROJECT_ID)
         assert set(data[0].keys()) == {
             'id',
             'project',
             'document_set',
             'number_of_pages',
             'data_file_name',
+            'data_file_producer',
             'file_url',
             'thumbnail_url',
             'ocr_time',
             'categorization_time',
             'extraction_time',
             'processing_time',
             'extraction_url',
@@ -164,14 +166,15 @@
             'callback_status_code',
             'category_confidence',
             'category_is_revised',
             'status_data',
             'labeling_available',
             'is_reviewed',
             'text',
+            'data_file_producer',
             'category',
             'dataset_status',
             'pages',
             'annotation_sets',
             'assignee',
             'created_by',
             'created_at',
@@ -200,14 +203,15 @@
             'callback_status_code',
             'category_confidence',
             'category_is_revised',
             'status_data',
             'labeling_available',
             'is_reviewed',
             'text',
+            'data_file_producer',
             'category',
             'dataset_status',
             'pages',
             'annotation_sets',
             'assignee',
             'created_by',
             'created_at',
```

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/tests/test_cli.py` & `konfuzio_sdk-0.3.3.dev20240415090556/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/tests/test_data.py` & `konfuzio_sdk-0.3.3.dev20240415090556/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/tests/test_evaluate.py` & `konfuzio_sdk-0.3.3.dev20240415090556/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/tests/test_extras.py` & `konfuzio_sdk-0.3.3.dev20240415090556/tests/test_extras.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/tests/test_normalize.py` & `konfuzio_sdk-0.3.3.dev20240415090556/tests/test_normalize.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/tests/test_regex.py` & `konfuzio_sdk-0.3.3.dev20240415090556/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/tests/test_samples.py` & `konfuzio_sdk-0.3.3.dev20240415090556/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/tests/test_urls.py` & `konfuzio_sdk-0.3.3.dev20240415090556/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240410112634/tests/test_utils.py` & `konfuzio_sdk-0.3.3.dev20240415090556/tests/test_utils.py`

 * *Files identical despite different names*

