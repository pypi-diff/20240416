# Comparing `tmp/syntrac_opentelemetry_instrumentation_bedrock-0.0.1.tar.gz` & `tmp/syntrac_opentelemetry_instrumentation_bedrock-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntrac_opentelemetry_instrumentation_bedrock-0.0.1.tar", max compression
+gzip compressed data, was "syntrac_opentelemetry_instrumentation_bedrock-0.0.2.tar", max compression
```

## Comparing `syntrac_opentelemetry_instrumentation_bedrock-0.0.1.tar` & `syntrac_opentelemetry_instrumentation_bedrock-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1170 2024-03-31 06:33:54.370785 syntrac_opentelemetry_instrumentation_bedrock-0.0.1/README.md
--rw-r--r--   0        0        0     2260 2024-03-31 06:33:54.693973 syntrac_opentelemetry_instrumentation_bedrock-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     7590 2024-03-31 06:33:54.373303 syntrac_opentelemetry_instrumentation_bedrock-0.0.1/syntrac_opentelemetry/instrumentation/bedrock/__init__.py
--rw-r--r--   0        0        0     1670 2024-03-31 06:33:54.374727 syntrac_opentelemetry_instrumentation_bedrock-0.0.1/syntrac_opentelemetry/instrumentation/bedrock/reusable_streaming_body.py
--rw-r--r--   0        0        0       22 2024-03-31 06:33:54.374911 syntrac_opentelemetry_instrumentation_bedrock-0.0.1/syntrac_opentelemetry/instrumentation/bedrock/version.py
--rw-r--r--   0        0        0     2873 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_bedrock-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1170 2024-04-16 14:24:10.847837 syntrac_opentelemetry_instrumentation_bedrock-0.0.2/README.md
+-rw-r--r--   0        0        0      983 2024-04-16 14:24:10.854579 syntrac_opentelemetry_instrumentation_bedrock-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7590 2024-04-16 14:24:10.849840 syntrac_opentelemetry_instrumentation_bedrock-0.0.2/syntrac_opentelemetry/instrumentation/bedrock/__init__.py
+-rw-r--r--   0        0        0     1670 2024-04-16 14:24:10.851061 syntrac_opentelemetry_instrumentation_bedrock-0.0.2/syntrac_opentelemetry/instrumentation/bedrock/reusable_streaming_body.py
+-rw-r--r--   0        0        0       22 2024-04-16 14:24:10.851174 syntrac_opentelemetry_instrumentation_bedrock-0.0.2/syntrac_opentelemetry/instrumentation/bedrock/version.py
+-rw-r--r--   0        0        0     2239 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_bedrock-0.0.2/PKG-INFO
```

### Comparing `syntrac_opentelemetry_instrumentation_bedrock-0.0.1/README.md` & `syntrac_opentelemetry_instrumentation_bedrock-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_bedrock-0.0.1/syntrac_opentelemetry/instrumentation/bedrock/__init__.py` & `syntrac_opentelemetry_instrumentation_bedrock-0.0.2/syntrac_opentelemetry/instrumentation/bedrock/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_bedrock-0.0.1/syntrac_opentelemetry/instrumentation/bedrock/reusable_streaming_body.py` & `syntrac_opentelemetry_instrumentation_bedrock-0.0.2/syntrac_opentelemetry/instrumentation/bedrock/reusable_streaming_body.py`

 * *Files identical despite different names*

