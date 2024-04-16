# Comparing `tmp/fhirstarter-2.2.2.tar.gz` & `tmp/fhirstarter-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhirstarter-2.2.2.tar", max compression
+gzip compressed data, was "fhirstarter-2.3.0.tar", max compression
```

## Comparing `fhirstarter-2.2.2.tar` & `fhirstarter-2.3.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1071 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/LICENSE.md
--rw-r--r--   0        0        0     7650 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/README.md
--rw-r--r--   0        0        0      618 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/fhirstarter/__init__.py
--rw-r--r--   0        0        0        0 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/fhirstarter/examples/__init__.py
--rw-r--r--   0        0        0      151 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/fhirstarter/examples/config.toml
--rw-r--r--   0        0        0     6464 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/fhirstarter/examples/example.py
--rw-r--r--   0        0        0     6289 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/fhirstarter/exceptions.py
--rw-r--r--   0        0        0       92 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/fhirstarter/fhir_specification/__init__.py
--rw-r--r--   0        0        0    10722 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/fhirstarter/fhir_specification/scripts/create_sequence_data.py
--rw-r--r--   0        0        0        0 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4/__init__.py
--rw-r--r--   0        0        0   392011 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4/examples.zip
--rw-r--r--   0        0        0     2814 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4/extra-search-parameters.json
--rw-r--r--   0        0        0     3334 2024-04-13 04:02:48.301721 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4/resource_types.json
--rw-r--r--   0        0        0   113904 2024-04-13 04:02:48.305722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4/search-parameters.zip
--rw-r--r--   0        0        0        0 2024-04-13 04:02:48.305722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4B/__init__.py
--rw-r--r--   0        0        0   397649 2024-04-13 04:02:48.305722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4B/examples.zip
--rw-r--r--   0        0        0     1800 2024-04-13 04:02:48.305722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4B/extra-search-parameters.json
--rw-r--r--   0        0        0     3081 2024-04-13 04:02:48.305722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4B/resource_types.json
--rw-r--r--   0        0        0   117431 2024-04-13 04:02:48.305722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4B/search-parameters.zip
--rw-r--r--   0        0        0        0 2024-04-13 04:02:48.305722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R5/__init__.py
--rw-r--r--   0        0        0   436165 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R5/examples.zip
--rw-r--r--   0        0        0     2356 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R5/extra-search-parameters.json
--rw-r--r--   0        0        0     3526 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R5/resource_types.json
--rw-r--r--   0        0        0   112399 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R5/search-parameters.zip
--rw-r--r--   0        0        0        0 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/STU3/__init__.py
--rw-r--r--   0        0        0   361150 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/STU3/examples.zip
--rw-r--r--   0        0        0     2624 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/STU3/extra-search-parameters.json
--rw-r--r--   0        0        0     2416 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/STU3/resource_types.json
--rw-r--r--   0        0        0    91155 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/STU3/search-parameters.zip
--rw-r--r--   0        0        0       32 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/__init__.py
--rw-r--r--   0        0        0     4692 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhir_specification/utils.py
--rw-r--r--   0        0        0    22399 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/fhirstarter.py
--rw-r--r--   0        0        0    20633 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/functions.py
--rw-r--r--   0        0        0     3354 2024-04-13 04:02:48.309722 fhirstarter-2.2.2/fhirstarter/interactions.py
--rw-r--r--   0        0        0     3135 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/json_patch.py
--rw-r--r--   0        0        0    10517 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/openapi.py
--rw-r--r--   0        0        0     7222 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/providers.py
--rw-r--r--   0        0        0     1691 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/resources.py
--rw-r--r--   0        0        0     6375 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/search_parameters.py
--rw-r--r--   0        0        0       68 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/testclient.py
--rw-r--r--   0        0        0        0 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/tests/__init__.py
--rw-r--r--   0        0        0     6330 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/tests/config.py
--rw-r--r--   0        0        0     1373 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/tests/conftest.py
--rw-r--r--   0        0        0     1500 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/tests/resources.py
--rw-r--r--   0        0        0     6667 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/tests/test_capability_statement.py
--rw-r--r--   0        0        0     3547 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/tests/test_dependencies.py
--rw-r--r--   0        0        0    10310 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/tests/test_errors.py
--rw-r--r--   0        0        0    14721 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/tests/test_interactions.py
--rw-r--r--   0        0        0    13703 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/tests/test_openapi.py
--rw-r--r--   0        0        0     7438 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/tests/test_utils.py
--rw-r--r--   0        0        0     2552 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/tests/utils.py
--rw-r--r--   0        0        0    18870 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/fhirstarter/utils.py
--rw-r--r--   0        0        0     3050 2024-04-13 04:02:48.313722 fhirstarter-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     9714 1970-01-01 00:00:00.000000 fhirstarter-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-16 16:17:07.300562 fhirstarter-2.3.0/LICENSE.md
+-rw-r--r--   0        0        0     7650 2024-04-16 16:17:07.300562 fhirstarter-2.3.0/README.md
+-rw-r--r--   0        0        0      618 2024-04-16 16:17:07.300562 fhirstarter-2.3.0/fhirstarter/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:17:07.300562 fhirstarter-2.3.0/fhirstarter/examples/__init__.py
+-rw-r--r--   0        0        0      151 2024-04-16 16:17:07.300562 fhirstarter-2.3.0/fhirstarter/examples/config.toml
+-rw-r--r--   0        0        0     6464 2024-04-16 16:17:07.300562 fhirstarter-2.3.0/fhirstarter/examples/example.py
+-rw-r--r--   0        0        0     6289 2024-04-16 16:17:07.300562 fhirstarter-2.3.0/fhirstarter/exceptions.py
+-rw-r--r--   0        0        0       92 2024-04-16 16:17:07.304562 fhirstarter-2.3.0/fhirstarter/fhir_specification/__init__.py
+-rw-r--r--   0        0        0    10722 2024-04-16 16:17:07.304562 fhirstarter-2.3.0/fhirstarter/fhir_specification/scripts/create_sequence_data.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:17:07.304562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4/__init__.py
+-rw-r--r--   0        0        0   392011 2024-04-16 16:17:07.304562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4/examples.zip
+-rw-r--r--   0        0        0     2814 2024-04-16 16:17:07.304562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4/extra-search-parameters.json
+-rw-r--r--   0        0        0     3334 2024-04-16 16:17:07.304562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4/resource_types.json
+-rw-r--r--   0        0        0   113904 2024-04-16 16:17:07.304562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4/search-parameters.zip
+-rw-r--r--   0        0        0        0 2024-04-16 16:17:07.304562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4B/__init__.py
+-rw-r--r--   0        0        0   397649 2024-04-16 16:17:07.304562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4B/examples.zip
+-rw-r--r--   0        0        0     1800 2024-04-16 16:17:07.308562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4B/extra-search-parameters.json
+-rw-r--r--   0        0        0     3081 2024-04-16 16:17:07.308562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4B/resource_types.json
+-rw-r--r--   0        0        0   117431 2024-04-16 16:17:07.308562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4B/search-parameters.zip
+-rw-r--r--   0        0        0        0 2024-04-16 16:17:07.308562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R5/__init__.py
+-rw-r--r--   0        0        0   436165 2024-04-16 16:17:07.308562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R5/examples.zip
+-rw-r--r--   0        0        0     2356 2024-04-16 16:17:07.308562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R5/extra-search-parameters.json
+-rw-r--r--   0        0        0     3526 2024-04-16 16:17:07.308562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R5/resource_types.json
+-rw-r--r--   0        0        0   112399 2024-04-16 16:17:07.308562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R5/search-parameters.zip
+-rw-r--r--   0        0        0        0 2024-04-16 16:17:07.308562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/STU3/__init__.py
+-rw-r--r--   0        0        0   361150 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/STU3/examples.zip
+-rw-r--r--   0        0        0     2624 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/STU3/extra-search-parameters.json
+-rw-r--r--   0        0        0     2416 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/STU3/resource_types.json
+-rw-r--r--   0        0        0    91155 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/STU3/search-parameters.zip
+-rw-r--r--   0        0        0       32 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/__init__.py
+-rw-r--r--   0        0        0     4692 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/fhir_specification/utils.py
+-rw-r--r--   0        0        0    22399 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/fhirstarter.py
+-rw-r--r--   0        0        0    20633 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/functions.py
+-rw-r--r--   0        0        0     3354 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/interactions.py
+-rw-r--r--   0        0        0     3135 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/json_patch.py
+-rw-r--r--   0        0        0    10517 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/openapi.py
+-rw-r--r--   0        0        0     7222 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/providers.py
+-rw-r--r--   0        0        0     1691 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/resources.py
+-rw-r--r--   0        0        0     6375 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/search_parameters.py
+-rw-r--r--   0        0        0       68 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/testclient.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/tests/__init__.py
+-rw-r--r--   0        0        0     6330 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/tests/config.py
+-rw-r--r--   0        0        0     1373 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/tests/conftest.py
+-rw-r--r--   0        0        0     1500 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/tests/resources.py
+-rw-r--r--   0        0        0     6667 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/tests/test_capability_statement.py
+-rw-r--r--   0        0        0     3547 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/tests/test_dependencies.py
+-rw-r--r--   0        0        0    10310 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/tests/test_errors.py
+-rw-r--r--   0        0        0    14721 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/tests/test_interactions.py
+-rw-r--r--   0        0        0    13703 2024-04-16 16:17:07.312562 fhirstarter-2.3.0/fhirstarter/tests/test_openapi.py
+-rw-r--r--   0        0        0     8906 2024-04-16 16:17:07.316562 fhirstarter-2.3.0/fhirstarter/tests/test_utils.py
+-rw-r--r--   0        0        0     2552 2024-04-16 16:17:07.316562 fhirstarter-2.3.0/fhirstarter/tests/utils.py
+-rw-r--r--   0        0        0    21217 2024-04-16 16:17:07.316562 fhirstarter-2.3.0/fhirstarter/utils.py
+-rw-r--r--   0        0        0     3050 2024-04-16 16:17:07.316562 fhirstarter-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9714 1970-01-01 00:00:00.000000 fhirstarter-2.3.0/PKG-INFO
```

### Comparing `fhirstarter-2.2.2/LICENSE.md` & `fhirstarter-2.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/README.md` & `fhirstarter-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/__init__.py` & `fhirstarter-2.3.0/fhirstarter/__init__.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/examples/example.py` & `fhirstarter-2.3.0/fhirstarter/examples/example.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/exceptions.py` & `fhirstarter-2.3.0/fhirstarter/exceptions.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/fhir_specification/scripts/create_sequence_data.py` & `fhirstarter-2.3.0/fhirstarter/fhir_specification/scripts/create_sequence_data.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4/examples.zip` & `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4/examples.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4/extra-search-parameters.json` & `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4/extra-search-parameters.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4/resource_types.json` & `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4/resource_types.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4/search-parameters.zip` & `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4/search-parameters.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4B/examples.zip` & `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4B/examples.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4B/extra-search-parameters.json` & `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4B/extra-search-parameters.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4B/resource_types.json` & `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4B/resource_types.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R4B/search-parameters.zip` & `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R4B/search-parameters.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R5/examples.zip` & `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R5/examples.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R5/extra-search-parameters.json` & `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R5/extra-search-parameters.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R5/resource_types.json` & `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R5/resource_types.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/R5/search-parameters.zip` & `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/R5/search-parameters.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/STU3/examples.zip` & `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/STU3/examples.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/STU3/extra-search-parameters.json` & `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/STU3/extra-search-parameters.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/STU3/resource_types.json` & `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/STU3/resource_types.json`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/fhir_specification/sequences/STU3/search-parameters.zip` & `fhirstarter-2.3.0/fhirstarter/fhir_specification/sequences/STU3/search-parameters.zip`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/fhir_specification/utils.py` & `fhirstarter-2.3.0/fhirstarter/fhir_specification/utils.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/fhirstarter.py` & `fhirstarter-2.3.0/fhirstarter/fhirstarter.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/functions.py` & `fhirstarter-2.3.0/fhirstarter/functions.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/interactions.py` & `fhirstarter-2.3.0/fhirstarter/interactions.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/json_patch.py` & `fhirstarter-2.3.0/fhirstarter/json_patch.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/openapi.py` & `fhirstarter-2.3.0/fhirstarter/openapi.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/providers.py` & `fhirstarter-2.3.0/fhirstarter/providers.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/resources.py` & `fhirstarter-2.3.0/fhirstarter/resources.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/search_parameters.py` & `fhirstarter-2.3.0/fhirstarter/search_parameters.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/tests/config.py` & `fhirstarter-2.3.0/fhirstarter/tests/config.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/tests/conftest.py` & `fhirstarter-2.3.0/fhirstarter/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/tests/resources.py` & `fhirstarter-2.3.0/fhirstarter/tests/resources.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/tests/test_capability_statement.py` & `fhirstarter-2.3.0/fhirstarter/tests/test_capability_statement.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/tests/test_dependencies.py` & `fhirstarter-2.3.0/fhirstarter/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/tests/test_errors.py` & `fhirstarter-2.3.0/fhirstarter/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/tests/test_interactions.py` & `fhirstarter-2.3.0/fhirstarter/tests/test_interactions.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/tests/test_openapi.py` & `fhirstarter-2.3.0/fhirstarter/tests/test_openapi.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/tests/utils.py` & `fhirstarter-2.3.0/fhirstarter/tests/utils.py`

 * *Files identical despite different names*

### Comparing `fhirstarter-2.2.2/fhirstarter/utils.py` & `fhirstarter-2.3.0/fhirstarter/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,101 +1,159 @@
-"""Utility functions for creation of routes and responses."""
+"""Miscellaneous utility functions."""
 
 from dataclasses import dataclass
-from typing import Any, Callable, ClassVar, Dict, Literal, Union
+from typing import Any, Callable, ClassVar, Dict, Literal, Sequence, Union
 
 from fastapi import Request
 from fastapi.responses import JSONResponse, Response
 
 from . import status
 from .fhir_specification.utils import is_resource_type
 from .interactions import ResourceType, SearchTypeInteraction, TypeInteraction
 from .resources import Bundle, OperationOutcome, Resource
 
 
 @dataclass
-class InteractionInfo:
-    resource_type: Union[str, None]
+class ParsedRequest:
+    request_type: Union[Literal["interaction", "operation"], None] = None
+    resource_type: Union[str, None] = None
+    resource_id: Union[str, None] = None
     interaction_type: Union[
         Literal[
             "read", "update", "patch", "delete", "create", "search-type", "capabilities"
         ],
         None,
-    ]
-    resource_id: Union[str, None]
+    ] = None
+    operation_name: Union[str, None] = None
 
 
-def parse_fhir_request(request: Request) -> InteractionInfo:
+def parse_fhir_request(request: Request) -> ParsedRequest:
     """
-    Parse a FHIR request into its component parts, and determine an interaction type.
+    Parse a FHIR request into its component parts, and determine an interaction type or operation
+    name. Return a ParsedRequest object with the information.
+
+    If this function isn't able to identify the request as a FHIR request, then an empty
+    ParsedRequest object will be returned.
 
     Note: This function is currently oriented around specific use cases for this framework.
     Specifically, it will correctly categorize read, update, patch, create, search-type, and
-    capabilities interactions. Further enhancement is needed to support more use cases.
+    capabilities interactions, and will identify operations. Further enhancement is needed to
+    support more use cases.
     """
-    no_info = InteractionInfo(  # type: ignore[call-arg]
-        resource_type=None, interaction_type=None, resource_id=None
-    )
-
     split_path = request.url.path.split("/")
     if not split_path:
-        return no_info
+        return ParsedRequest()
+
+    if split_path[-1].startswith("$"):
+        return _parse_fhir_operation_request(request, split_path)
+    else:
+        return _parse_fhir_interaction_request(request, split_path)
+
 
+def _parse_fhir_operation_request(
+    request: Request, split_path: Sequence[str]
+) -> ParsedRequest:
+    """Parse a potential FHIR operation request."""
+    # The request may be a FHIR operation -- make sure the method is either a GET or POST
+    if request.method not in ("GET", "POST"):
+        return ParsedRequest()
+
+    resource_type = None
     resource_id = None
 
+    # Determine the operation name
+    operation_name = split_path[-1]
+    if operation_name and operation_name[0] == "$":
+        operation_name = operation_name[1:]
+
+    # If neither of these conditions are met, then it's an operation on the base URL
+    path_parts_count = len(split_path)
+    if path_parts_count >= 3 and is_resource_type(split_path[-3]):
+        # Instance operation -- get the resource type and path
+        resource_type = split_path[-3]
+        resource_id = split_path[-2]
+    elif path_parts_count >= 2 and is_resource_type(split_path[-2]):
+        # Type operation -- get the resource type
+        resource_type = split_path[-2]
+
+    return ParsedRequest(  # type: ignore[call-arg]
+        request_type="operation",
+        resource_type=resource_type,
+        resource_id=resource_id,
+        operation_name=operation_name,
+    )
+
+
+def _parse_fhir_interaction_request(
+    request: Request, split_path: Sequence[str]
+) -> ParsedRequest:
+    """Parse a potential FHIR interaction request."""
+    # The request may be a FHIR interaction -- determine what it is based on the request method
+    # and the URL format
+    resource_type = None
+    resource_id = None
+    interaction_type: Union[str, None]
+
+    path_parts_count = len(split_path)
+
     if request.method == "GET":
         if split_path[-1] == "metadata":
-            return InteractionInfo(  # type: ignore[call-arg]
-                resource_type=None, interaction_type="capabilities", resource_id=None
-            )
+            interaction_type = "capabilities"
         elif is_resource_type(split_path[-1]):
             resource_type = split_path[-1]
             interaction_type = "search-type"
-        elif len(split_path) >= 3:
-            resource_type, resource_id = split_path[-2:]
+        elif path_parts_count >= 3:
+            resource_type = split_path[-2]
+            resource_id = split_path[-1]
             interaction_type = "read"
         else:
-            return no_info
+            return ParsedRequest()
     elif request.method == "POST":
         if is_resource_type(split_path[-1]):
             resource_type = split_path[-1]
             interaction_type = "create"
         elif split_path[-1] == "_search":
             resource_type = split_path[-2]
             interaction_type = "search-type"
         else:
-            return no_info
+            return ParsedRequest()
     elif request.method == "PUT":
-        if len(split_path) >= 3:
-            resource_type, resource_id = split_path[-2:]
+        if path_parts_count >= 3:
+            resource_type = split_path[-2]
+            resource_id = split_path[-1]
             interaction_type = "update"
         else:
-            return no_info
+            return ParsedRequest()
     elif request.method == "PATCH":
-        if len(split_path) >= 3:
-            resource_type, resource_id = split_path[-2:]
+        if path_parts_count >= 3:
+            resource_type = split_path[-2]
+            resource_id = split_path[-1]
             interaction_type = "patch"
         else:
-            return no_info
+            return ParsedRequest()
     elif request.method == "DELETE":
-        if len(split_path) >= 3:
-            resource_type, resource_id = split_path[-2:]
+        if path_parts_count >= 3:
+            resource_type = split_path[-2]
+            resource_id = split_path[-1]
             interaction_type = "delete"
         else:
-            return no_info
+            return ParsedRequest()
     else:
-        return no_info
+        return ParsedRequest()
 
-    if not is_resource_type(resource_type):
-        return no_info
+    # If the resource type found is not an actual resource type, then it's not a FHIR
+    # interaction
+    if resource_type and not is_resource_type(resource_type):
+        return ParsedRequest()
 
-    return InteractionInfo(  # type: ignore[call-arg]
+    return ParsedRequest(  # type: ignore[call-arg]
+        request_type="interaction",
         resource_type=resource_type,
-        interaction_type=interaction_type,
         resource_id=resource_id,
+        interaction_type=interaction_type,
     )
 
 
 def make_operation_outcome(
     severity: str, code: str, details_text: str
 ) -> OperationOutcome:
     """Create a simple OperationOutcome given a severity, code, and details."""
@@ -247,15 +305,16 @@
             interaction,
             _ok,
             _unauthorized,
             _forbidden,
             _not_found,
             _internal_server_error,
         ),
-        "operation_id": f"fhirstarter|instance|read|get|{resource_type_str}|{interaction.resource_type.__module__}|{interaction.resource_type.__name__}",
+        "operation_id": f"fhirstarter|instance|read|get|{resource_type_str}|"
+        f"{interaction.resource_type.__module__}|{interaction.resource_type.__name__}",
         "response_model_exclude_none": True,
         **interaction.route_options,
     }
 
 
 def update_route_args(interaction: TypeInteraction[ResourceType]) -> Dict[str, Any]:
     """Provide arguments for creation of a FHIR update API route."""
@@ -275,15 +334,16 @@
             _bad_request,
             _unauthorized,
             _forbidden,
             _not_found,
             _unprocessable_entity,
             _internal_server_error,
         ),
-        "operation_id": f"fhirstarter|instance|update|put|{resource_type_str}|{interaction.resource_type.__module__}|{interaction.resource_type.__name__}",
+        "operation_id": f"fhirstarter|instance|update|put|{resource_type_str}|"
+        f"{interaction.resource_type.__module__}|{interaction.resource_type.__name__}",
         "response_model_exclude_none": True,
         **interaction.route_options,
     }
 
 
 def patch_route_args(interaction: TypeInteraction[ResourceType]) -> Dict[str, Any]:
     """Provide arguments for creation of a FHIR patch API route."""
@@ -304,15 +364,16 @@
             _bad_request,
             _unauthorized,
             _forbidden,
             _not_found,
             _unprocessable_entity,
             _internal_server_error,
         ),
-        "operation_id": f"fhirstarter|instance|patch|patch|{resource_type_str}|{interaction.resource_type.__module__}|{interaction.resource_type.__name__}",
+        "operation_id": f"fhirstarter|instance|patch|patch|{resource_type_str}|"
+        f"{interaction.resource_type.__module__}|{interaction.resource_type.__name__}",
         "response_model_exclude_none": True,
         **interaction.route_options,
     }
 
 
 def delete_route_args(interaction: TypeInteraction[ResourceType]) -> Dict[str, Any]:
     """Provide arguments for creation of a FHIR delete API route."""
@@ -329,15 +390,16 @@
         "responses": _responses(
             interaction,
             _no_content,
             _unauthorized,
             _forbidden,
             _internal_server_error,
         ),
-        "operation_id": f"fhirstarter|instance|delete|delete|{resource_type_str}|{interaction.resource_type.__module__}|{interaction.resource_type.__name__}",
+        "operation_id": f"fhirstarter|instance|delete|delete|{resource_type_str}|"
+        f"{interaction.resource_type.__module__}|{interaction.resource_type.__name__}",
         "response_model_exclude_none": True,
         **interaction.route_options,
     }
 
 
 def create_route_args(interaction: TypeInteraction[ResourceType]) -> Dict[str, Any]:
     """Provide arguments for creation of a FHIR create API route."""
@@ -356,15 +418,16 @@
             _created,
             _bad_request,
             _unauthorized,
             _forbidden,
             _unprocessable_entity,
             _internal_server_error,
         ),
-        "operation_id": f"fhirstarter|type|create|post|{resource_type_str}|{interaction.resource_type.__module__}|{interaction.resource_type.__name__}",
+        "operation_id": f"fhirstarter|type|create|post|{resource_type_str}|"
+        f"{interaction.resource_type.__module__}|{interaction.resource_type.__name__}",
         "response_model_exclude_none": True,
         **interaction.route_options,
     }
 
 
 def search_type_route_args(
     interaction: TypeInteraction[ResourceType], post: bool
@@ -384,15 +447,17 @@
             interaction,
             _ok,
             _bad_request,
             _unauthorized,
             _forbidden,
             _internal_server_error,
         ),
-        "operation_id": f"fhirstarter|type|search-type|{'post' if post else 'get'}|{resource_type_str}|{interaction.resource_type.__module__}|{interaction.resource_type.__name__}",
+        "operation_id": f"fhirstarter|type|search-type|{'post' if post else 'get'}|"
+        f"{resource_type_str}|{interaction.resource_type.__module__}|"
+        f"{interaction.resource_type.__name__}",
         "response_model_exclude_none": True,
         **interaction.route_options,
     }
 
 
 _Responses = Dict[int, Dict[str, Any]]
 
@@ -503,10 +568,11 @@
 
 
 def _internal_server_error(_: TypeInteraction[ResourceType]) -> _Responses:
     """Documentation for an HTTP 500 Internal Server error response."""
     return {
         status.HTTP_500_INTERNAL_SERVER_ERROR: {
             "model": OperationOutcome,
-            "description": f"The server has encountered a situation it does not know how to handle.",
+            "description": f"The server has encountered a situation it does not know how to "
+            "handle.",
         }
     }
```

### Comparing `fhirstarter-2.2.2/pyproject.toml` & `fhirstarter-2.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fhirstarter"
-version = "2.2.2"
+version = "2.3.0"
 description = "An ASGI FHIR API framework built on top of FastAPI and FHIR Resources"
 authors = ["Christopher Sande <christopher.sande@canvasmedical.com>"]
 maintainers = ["Canvas Medical Engineering <engineering@canvasmedical.com>"]
 readme = "README.md"
 homepage = "https://github.com/canvas-medical/fhirstarter"
 repository = "https://github.com/canvas-medical/fhirstarter"
 keywords = ["fhir", "api", "server", "resources", "framework", "fastapi", "healthcare", "hl7"]
```

### Comparing `fhirstarter-2.2.2/PKG-INFO` & `fhirstarter-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhirstarter
-Version: 2.2.2
+Version: 2.3.0
 Summary: An ASGI FHIR API framework built on top of FastAPI and FHIR Resources
 Home-page: https://github.com/canvas-medical/fhirstarter
 Keywords: fhir,api,server,resources,framework,fastapi,healthcare,hl7
 Author: Christopher Sande
 Author-email: christopher.sande@canvasmedical.com
 Maintainer: Canvas Medical Engineering
 Maintainer-email: engineering@canvasmedical.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fhirstarter Version: 2.2.2 Summary: An ASGI FHIR
+Metadata-Version: 2.1 Name: fhirstarter Version: 2.3.0 Summary: An ASGI FHIR
 API framework built on top of FastAPI and FHIR Resources Home-page: https://
 github.com/canvas-medical/fhirstarter Keywords:
 fhir,api,server,resources,framework,fastapi,healthcare,hl7 Author: Christopher
 Sande Author-email: christopher.sande@canvasmedical.com Maintainer: Canvas
 Medical Engineering Maintainer-email: engineering@canvasmedical.com Requires-
 Python: >=3.8.0,<3.13.0 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment Classifier: Framework :: AsyncIO
```

