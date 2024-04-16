# Comparing `tmp/syntrac_opentelemetry_instrumentation_anthropic-0.0.1.tar.gz` & `tmp/syntrac_opentelemetry_instrumentation_anthropic-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntrac_opentelemetry_instrumentation_anthropic-0.0.1.tar", max compression
+gzip compressed data, was "syntrac_opentelemetry_instrumentation_anthropic-0.0.2.tar", max compression
```

## Comparing `syntrac_opentelemetry_instrumentation_anthropic-0.0.1.tar` & `syntrac_opentelemetry_instrumentation_anthropic-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1017 2024-03-31 06:30:54.014248 syntrac_opentelemetry_instrumentation_anthropic-0.0.1/README.md
--rw-r--r--   0        0        0     2452 2024-03-31 06:30:54.368063 syntrac_opentelemetry_instrumentation_anthropic-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     7268 2024-03-31 06:30:54.017419 syntrac_opentelemetry_instrumentation_anthropic-0.0.1/syntrac_opentelemetry/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0       22 2024-03-31 06:30:54.018777 syntrac_opentelemetry_instrumentation_anthropic-0.0.1/syntrac_opentelemetry/instrumentation/anthropic/version.py
--rw-r--r--   0        0        0     2756 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_anthropic-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1017 2024-04-16 14:16:02.923032 syntrac_opentelemetry_instrumentation_anthropic-0.0.2/README.md
+-rw-r--r--   0        0        0     1175 2024-04-16 14:16:02.928877 syntrac_opentelemetry_instrumentation_anthropic-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7268 2024-04-16 14:16:02.924397 syntrac_opentelemetry_instrumentation_anthropic-0.0.2/syntrac_opentelemetry/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-16 14:16:02.924994 syntrac_opentelemetry_instrumentation_anthropic-0.0.2/syntrac_opentelemetry/instrumentation/anthropic/version.py
+-rw-r--r--   0        0        0     2122 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_anthropic-0.0.2/PKG-INFO
```

### Comparing `syntrac_opentelemetry_instrumentation_anthropic-0.0.1/README.md` & `syntrac_opentelemetry_instrumentation_anthropic-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_anthropic-0.0.1/syntrac_opentelemetry/instrumentation/anthropic/__init__.py` & `syntrac_opentelemetry_instrumentation_anthropic-0.0.2/syntrac_opentelemetry/instrumentation/anthropic/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_anthropic-0.0.1/PKG-INFO` & `syntrac_opentelemetry_instrumentation_anthropic-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 Metadata-Version: 2.1
 Name: syntrac-opentelemetry-instrumentation-anthropic
-Version: 0.0.1
+Version: 0.0.2
 Summary: OpenTelemetry Anthropic instrumentation
 Home-page: https://github.com/syntracAI/syntrac/tree/main/packages/python/opentelemetry-instrumentation-anthropic
 License: Apache-2.0
 Author: Vuong Ngo
 Author-email: vuongngo.pd@gmail.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: instruments
-Requires-Dist: deprecated (==1.2.14) ; python_version >= "3.9" and python_version < "4"
-Requires-Dist: importlib-metadata (==6.11.0) ; python_version >= "3.9" and python_version < "4"
-Requires-Dist: opentelemetry-api (==1.23.0) ; python_version >= "3.9" and python_version < "4"
-Requires-Dist: opentelemetry-instrumentation (==0.44b0) ; python_version >= "3.9" and python_version < "4"
-Requires-Dist: opentelemetry-semantic-conventions (==0.44b0) ; python_version >= "3.9" and python_version < "4"
-Requires-Dist: setuptools (==69.2.0) ; python_version >= "3.9" and python_version < "4"
-Requires-Dist: syntrac-opentelemetry-semantic-conventions-ai (==0.0.1) ; python_version >= "3.9" and python_version < "4"
-Requires-Dist: wrapt (==1.16.0) ; python_version >= "3.9" and python_version < "4"
-Requires-Dist: zipp (==3.18.1) ; python_version >= "3.9" and python_version < "4"
+Requires-Dist: opentelemetry-api (>=1.23.0,<2.0.0)
+Requires-Dist: opentelemetry-instrumentation (==0.44b0)
+Requires-Dist: opentelemetry-semantic-conventions (==0.44b0)
+Requires-Dist: syntrac-opentelemetry-semantic-conventions-ai (==0.0.1)
 Project-URL: Repository, https://github.com/syntracAI/syntrac/tree/main/packages/python/opentelemetry-instrumentation-anthropic
 Description-Content-Type: text/markdown
 
 # OpenTelemetry Anthropic Instrumentation
 
 This library allows tracing Anthropic prompts and completions sent with the official [Anthropic library](https://github.com/anthropics/anthropic-sdk-python).
```

