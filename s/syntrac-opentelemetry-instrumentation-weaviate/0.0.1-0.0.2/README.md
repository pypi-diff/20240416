# Comparing `tmp/syntrac_opentelemetry_instrumentation_weaviate-0.0.1.tar.gz` & `tmp/syntrac_opentelemetry_instrumentation_weaviate-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntrac_opentelemetry_instrumentation_weaviate-0.0.1.tar", max compression
+gzip compressed data, was "syntrac_opentelemetry_instrumentation_weaviate-0.0.2.tar", max compression
```

## Comparing `syntrac_opentelemetry_instrumentation_weaviate-0.0.1.tar` & `syntrac_opentelemetry_instrumentation_weaviate-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      626 2024-03-31 06:46:13.038707 syntrac_opentelemetry_instrumentation_weaviate-0.0.1/README.md
--rw-r--r--   0        0        0     2465 2024-03-31 06:46:13.334077 syntrac_opentelemetry_instrumentation_weaviate-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4527 2024-03-31 06:46:13.041226 syntrac_opentelemetry_instrumentation_weaviate-0.0.1/syntrac_opentelemetry/instrumentation/weaviate/__init__.py
--rw-r--r--   0        0        0       22 2024-03-31 06:46:13.042608 syntrac_opentelemetry_instrumentation_weaviate-0.0.1/syntrac_opentelemetry/instrumentation/weaviate/version.py
--rw-r--r--   0        0        0     5240 2024-03-31 06:46:13.042748 syntrac_opentelemetry_instrumentation_weaviate-0.0.1/syntrac_opentelemetry/instrumentation/weaviate/wrapper.py
--rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_weaviate-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      626 2024-04-16 14:36:23.460750 syntrac_opentelemetry_instrumentation_weaviate-0.0.2/README.md
+-rw-r--r--   0        0        0     1188 2024-04-16 14:36:23.469226 syntrac_opentelemetry_instrumentation_weaviate-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4527 2024-04-16 14:36:23.463137 syntrac_opentelemetry_instrumentation_weaviate-0.0.2/syntrac_opentelemetry/instrumentation/weaviate/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-16 14:36:23.464190 syntrac_opentelemetry_instrumentation_weaviate-0.0.2/syntrac_opentelemetry/instrumentation/weaviate/version.py
+-rw-r--r--   0        0        0     5240 2024-04-16 14:36:23.464312 syntrac_opentelemetry_instrumentation_weaviate-0.0.2/syntrac_opentelemetry/instrumentation/weaviate/wrapper.py
+-rw-r--r--   0        0        0     1727 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_weaviate-0.0.2/PKG-INFO
```

### Comparing `syntrac_opentelemetry_instrumentation_weaviate-0.0.1/README.md` & `syntrac_opentelemetry_instrumentation_weaviate-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_weaviate-0.0.1/syntrac_opentelemetry/instrumentation/weaviate/__init__.py` & `syntrac_opentelemetry_instrumentation_weaviate-0.0.2/syntrac_opentelemetry/instrumentation/weaviate/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_weaviate-0.0.1/syntrac_opentelemetry/instrumentation/weaviate/wrapper.py` & `syntrac_opentelemetry_instrumentation_weaviate-0.0.2/syntrac_opentelemetry/instrumentation/weaviate/wrapper.py`

 * *Files identical despite different names*

