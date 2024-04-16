# Comparing `tmp/syntrac_opentelemetry_semantic_conventions_ai-0.0.1.tar.gz` & `tmp/syntrac_opentelemetry_semantic_conventions_ai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntrac_opentelemetry_semantic_conventions_ai-0.0.1.tar", max compression
+gzip compressed data, was "syntrac_opentelemetry_semantic_conventions_ai-0.0.2.tar", max compression
```

## Comparing `syntrac_opentelemetry_semantic_conventions_ai-0.0.1.tar` & `syntrac_opentelemetry_semantic_conventions_ai-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      356 2024-03-29 08:47:12.989594 syntrac_opentelemetry_semantic_conventions_ai-0.0.1/README.md
--rw-r--r--   0        0        0      693 2024-03-29 08:47:13.298580 syntrac_opentelemetry_semantic_conventions_ai-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2627 2024-03-29 08:47:12.992227 syntrac_opentelemetry_semantic_conventions_ai-0.0.1/syntrac_opentelemetry/semconv/ai/__init__.py
--rw-r--r--   0        0        0       22 2024-03-29 08:47:12.992919 syntrac_opentelemetry_semantic_conventions_ai-0.0.1/syntrac_opentelemetry/semconv/ai/version.py
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 syntrac_opentelemetry_semantic_conventions_ai-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      356 2024-04-16 14:18:19.541066 syntrac_opentelemetry_semantic_conventions_ai-0.0.2/README.md
+-rw-r--r--   0        0        0      693 2024-04-16 14:18:19.546339 syntrac_opentelemetry_semantic_conventions_ai-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2627 2024-04-16 14:18:19.542759 syntrac_opentelemetry_semantic_conventions_ai-0.0.2/syntrac_opentelemetry/semconv/ai/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-16 14:18:19.543413 syntrac_opentelemetry_semantic_conventions_ai-0.0.2/syntrac_opentelemetry/semconv/ai/version.py
+-rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 syntrac_opentelemetry_semantic_conventions_ai-0.0.2/PKG-INFO
```

### Comparing `syntrac_opentelemetry_semantic_conventions_ai-0.0.1/pyproject.toml` & `syntrac_opentelemetry_semantic_conventions_ai-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = [ "if TYPE_CHECKING:" ]
 show_missing = true
 
 [tool.poetry]
 name = "syntrac-opentelemetry-semantic-conventions-ai"
-version = "0.0.1"
+version = "0.0.2"
 description = "OpenTelemetry Semantic Conventions Extension for Large Language Models"
 authors = [ "Vuong Ngo <vuongngo.pd@gmail.com>" ]
 license = "Apache-2.0"
 readme = "README.md"
 
   [[tool.poetry.packages]]
   include = "syntrac_opentelemetry/semconv/ai"
```

### Comparing `syntrac_opentelemetry_semantic_conventions_ai-0.0.1/syntrac_opentelemetry/semconv/ai/__init__.py` & `syntrac_opentelemetry_semantic_conventions_ai-0.0.2/syntrac_opentelemetry/semconv/ai/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_semantic_conventions_ai-0.0.1/PKG-INFO` & `syntrac_opentelemetry_semantic_conventions_ai-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syntrac-opentelemetry-semantic-conventions-ai
-Version: 0.0.1
+Version: 0.0.2
 Summary: OpenTelemetry Semantic Conventions Extension for Large Language Models
 License: Apache-2.0
 Author: Vuong Ngo
 Author-email: vuongngo.pd@gmail.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

