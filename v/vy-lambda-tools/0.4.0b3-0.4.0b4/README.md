# Comparing `tmp/vy_lambda_tools-0.4.0b3.tar.gz` & `tmp/vy_lambda_tools-0.4.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vy_lambda_tools-0.4.0b3.tar", max compression
+gzip compressed data, was "vy_lambda_tools-0.4.0b4.tar", max compression
```

## Comparing `vy_lambda_tools-0.4.0b3.tar` & `vy_lambda_tools-0.4.0b4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       88 2024-04-05 10:27:48.000000 vy_lambda_tools-0.4.0b3/README.adoc
--rw-r--r--   0        0        0      607 2024-04-05 10:27:48.000000 vy_lambda_tools-0.4.0b3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-05 10:27:48.000000 vy_lambda_tools-0.4.0b3/vy_lambda_tools/__init__.py
--rw-r--r--   0        0        0      904 2024-04-05 10:27:48.000000 vy_lambda_tools-0.4.0b3/vy_lambda_tools/configuration.py
--rw-r--r--   0        0        0      217 2024-04-05 10:27:48.000000 vy_lambda_tools-0.4.0b3/vy_lambda_tools/feature_flag/__init__.py
--rw-r--r--   0        0        0     1988 2024-04-05 10:27:48.000000 vy_lambda_tools-0.4.0b3/vy_lambda_tools/feature_flag/base.py
--rw-r--r--   0        0        0     3519 2024-04-05 10:27:48.000000 vy_lambda_tools-0.4.0b3/vy_lambda_tools/feature_flag/providers.py
--rw-r--r--   0        0        0      312 2024-04-05 10:27:48.000000 vy_lambda_tools-0.4.0b3/vy_lambda_tools/handlers/__init__.py
--rw-r--r--   0        0        0     3990 2024-04-05 10:27:48.000000 vy_lambda_tools-0.4.0b3/vy_lambda_tools/handlers/api_gateway.py
--rw-r--r--   0        0        0     1205 2024-04-05 10:27:48.000000 vy_lambda_tools-0.4.0b3/vy_lambda_tools/handlers/dynamodb.py
--rw-r--r--   0        0        0      857 2024-04-05 10:27:48.000000 vy_lambda_tools-0.4.0b3/vy_lambda_tools/handlers/handler.py
--rw-r--r--   0        0        0     2850 2024-04-05 10:27:48.000000 vy_lambda_tools-0.4.0b3/vy_lambda_tools/handlers/sqs.py
--rw-r--r--   0        0        0     2360 2024-04-05 10:27:48.000000 vy_lambda_tools-0.4.0b3/vy_lambda_tools/instrumentation.py
--rw-r--r--   0        0        0        0 2024-04-05 10:27:48.000000 vy_lambda_tools-0.4.0b3/vy_lambda_tools/py.typed
--rw-r--r--   0        0        0     7217 2024-04-05 10:27:48.000000 vy_lambda_tools-0.4.0b3/vy_lambda_tools/routing.py
--rw-r--r--   0        0        0     4476 2024-04-05 10:27:48.000000 vy_lambda_tools-0.4.0b3/vy_lambda_tools/test_helpers.py
--rw-r--r--   0        0        0      421 2024-04-05 10:27:48.000000 vy_lambda_tools-0.4.0b3/vy_lambda_tools/types.py
--rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 vy_lambda_tools-0.4.0b3/PKG-INFO
+-rw-r--r--   0        0        0       88 2024-04-16 12:43:15.000000 vy_lambda_tools-0.4.0b4/README.adoc
+-rw-r--r--   0        0        0      607 2024-04-16 12:43:15.000000 vy_lambda_tools-0.4.0b4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 12:43:15.000000 vy_lambda_tools-0.4.0b4/vy_lambda_tools/__init__.py
+-rw-r--r--   0        0        0      904 2024-04-16 12:43:15.000000 vy_lambda_tools-0.4.0b4/vy_lambda_tools/configuration.py
+-rw-r--r--   0        0        0      217 2024-04-16 12:43:15.000000 vy_lambda_tools-0.4.0b4/vy_lambda_tools/feature_flag/__init__.py
+-rw-r--r--   0        0        0     1988 2024-04-16 12:43:15.000000 vy_lambda_tools-0.4.0b4/vy_lambda_tools/feature_flag/base.py
+-rw-r--r--   0        0        0     3519 2024-04-16 12:43:15.000000 vy_lambda_tools-0.4.0b4/vy_lambda_tools/feature_flag/providers.py
+-rw-r--r--   0        0        0      312 2024-04-16 12:43:15.000000 vy_lambda_tools-0.4.0b4/vy_lambda_tools/handlers/__init__.py
+-rw-r--r--   0        0        0     3990 2024-04-16 12:43:15.000000 vy_lambda_tools-0.4.0b4/vy_lambda_tools/handlers/api_gateway.py
+-rw-r--r--   0        0        0     1205 2024-04-16 12:43:15.000000 vy_lambda_tools-0.4.0b4/vy_lambda_tools/handlers/dynamodb.py
+-rw-r--r--   0        0        0      857 2024-04-16 12:43:15.000000 vy_lambda_tools-0.4.0b4/vy_lambda_tools/handlers/handler.py
+-rw-r--r--   0        0        0     2850 2024-04-16 12:43:15.000000 vy_lambda_tools-0.4.0b4/vy_lambda_tools/handlers/sqs.py
+-rw-r--r--   0        0        0     2360 2024-04-16 12:43:15.000000 vy_lambda_tools-0.4.0b4/vy_lambda_tools/instrumentation.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:43:15.000000 vy_lambda_tools-0.4.0b4/vy_lambda_tools/py.typed
+-rw-r--r--   0        0        0     7217 2024-04-16 12:43:15.000000 vy_lambda_tools-0.4.0b4/vy_lambda_tools/routing.py
+-rw-r--r--   0        0        0     4476 2024-04-16 12:43:15.000000 vy_lambda_tools-0.4.0b4/vy_lambda_tools/test_helpers.py
+-rw-r--r--   0        0        0      446 2024-04-16 12:43:15.000000 vy_lambda_tools-0.4.0b4/vy_lambda_tools/types.py
+-rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 vy_lambda_tools-0.4.0b4/PKG-INFO
```

### Comparing `vy_lambda_tools-0.4.0b3/pyproject.toml` & `vy_lambda_tools-0.4.0b4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vy-lambda-tools"
-version = "0.4.0b3"
+version = "0.4.0b4"
 description = ""
 authors = ["Nicolas Harlem Eide <nicolas@harlemeide.net>"]
 readme = "README.adoc"
 packages = [{include = "vy_lambda_tools"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `vy_lambda_tools-0.4.0b3/vy_lambda_tools/configuration.py` & `vy_lambda_tools-0.4.0b4/vy_lambda_tools/configuration.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.0b3/vy_lambda_tools/feature_flag/base.py` & `vy_lambda_tools-0.4.0b4/vy_lambda_tools/feature_flag/base.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.0b3/vy_lambda_tools/feature_flag/providers.py` & `vy_lambda_tools-0.4.0b4/vy_lambda_tools/feature_flag/providers.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.0b3/vy_lambda_tools/handlers/api_gateway.py` & `vy_lambda_tools-0.4.0b4/vy_lambda_tools/handlers/api_gateway.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.0b3/vy_lambda_tools/handlers/dynamodb.py` & `vy_lambda_tools-0.4.0b4/vy_lambda_tools/handlers/dynamodb.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.0b3/vy_lambda_tools/handlers/handler.py` & `vy_lambda_tools-0.4.0b4/vy_lambda_tools/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.0b3/vy_lambda_tools/handlers/sqs.py` & `vy_lambda_tools-0.4.0b4/vy_lambda_tools/handlers/sqs.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.0b3/vy_lambda_tools/instrumentation.py` & `vy_lambda_tools-0.4.0b4/vy_lambda_tools/instrumentation.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.0b3/vy_lambda_tools/routing.py` & `vy_lambda_tools-0.4.0b4/vy_lambda_tools/routing.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.0b3/vy_lambda_tools/test_helpers.py` & `vy_lambda_tools-0.4.0b4/vy_lambda_tools/test_helpers.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.4.0b3/PKG-INFO` & `vy_lambda_tools-0.4.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vy-lambda-tools
-Version: 0.4.0b3
+Version: 0.4.0b4
 Summary: 
 Author: Nicolas Harlem Eide
 Author-email: nicolas@harlemeide.net
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

