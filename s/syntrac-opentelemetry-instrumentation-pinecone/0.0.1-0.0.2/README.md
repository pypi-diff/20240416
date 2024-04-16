# Comparing `tmp/syntrac_opentelemetry_instrumentation_pinecone-0.0.1.tar.gz` & `tmp/syntrac_opentelemetry_instrumentation_pinecone-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntrac_opentelemetry_instrumentation_pinecone-0.0.1.tar", max compression
+gzip compressed data, was "syntrac_opentelemetry_instrumentation_pinecone-0.0.2.tar", max compression
```

## Comparing `syntrac_opentelemetry_instrumentation_pinecone-0.0.1.tar` & `syntrac_opentelemetry_instrumentation_pinecone-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      629 2024-03-31 06:43:13.868077 syntrac_opentelemetry_instrumentation_pinecone-0.0.1/README.md
--rw-r--r--   0        0        0     2465 2024-03-31 06:43:14.174043 syntrac_opentelemetry_instrumentation_pinecone-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     7379 2024-03-31 06:43:13.870447 syntrac_opentelemetry_instrumentation_pinecone-0.0.1/syntrac_opentelemetry/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0       22 2024-03-31 06:43:13.871473 syntrac_opentelemetry_instrumentation_pinecone-0.0.1/syntrac_opentelemetry/instrumentation/pinecone/version.py
--rw-r--r--   0        0        0     2364 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_pinecone-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      629 2024-04-16 14:33:58.696498 syntrac_opentelemetry_instrumentation_pinecone-0.0.2/README.md
+-rw-r--r--   0        0        0     1188 2024-04-16 14:33:58.703589 syntrac_opentelemetry_instrumentation_pinecone-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7379 2024-04-16 14:33:58.698534 syntrac_opentelemetry_instrumentation_pinecone-0.0.2/syntrac_opentelemetry/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-16 14:33:58.699487 syntrac_opentelemetry_instrumentation_pinecone-0.0.2/syntrac_opentelemetry/instrumentation/pinecone/version.py
+-rw-r--r--   0        0        0     1730 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_pinecone-0.0.2/PKG-INFO
```

### Comparing `syntrac_opentelemetry_instrumentation_pinecone-0.0.1/README.md` & `syntrac_opentelemetry_instrumentation_pinecone-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_pinecone-0.0.1/syntrac_opentelemetry/instrumentation/pinecone/__init__.py` & `syntrac_opentelemetry_instrumentation_pinecone-0.0.2/syntrac_opentelemetry/instrumentation/pinecone/__init__.py`

 * *Files identical despite different names*

