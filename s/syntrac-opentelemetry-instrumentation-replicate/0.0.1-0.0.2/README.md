# Comparing `tmp/syntrac_opentelemetry_instrumentation_replicate-0.0.1.tar.gz` & `tmp/syntrac_opentelemetry_instrumentation_replicate-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntrac_opentelemetry_instrumentation_replicate-0.0.1.tar", max compression
+gzip compressed data, was "syntrac_opentelemetry_instrumentation_replicate-0.0.2.tar", max compression
```

## Comparing `syntrac_opentelemetry_instrumentation_replicate-0.0.1.tar` & `syntrac_opentelemetry_instrumentation_replicate-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1201 2024-03-31 06:44:12.987369 syntrac_opentelemetry_instrumentation_replicate-0.0.1/README.md
--rw-r--r--   0        0        0     2463 2024-03-31 06:44:13.255634 syntrac_opentelemetry_instrumentation_replicate-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6390 2024-03-31 06:44:12.989250 syntrac_opentelemetry_instrumentation_replicate-0.0.1/syntrac_opentelemetry/instrumentation/replicate/__init__.py
--rw-r--r--   0        0        0       22 2024-03-31 06:44:12.990232 syntrac_opentelemetry_instrumentation_replicate-0.0.1/syntrac_opentelemetry/instrumentation/replicate/version.py
--rw-r--r--   0        0        0     2943 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_replicate-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1201 2024-04-16 14:34:40.465294 syntrac_opentelemetry_instrumentation_replicate-0.0.2/README.md
+-rw-r--r--   0        0        0     1186 2024-04-16 14:34:40.472432 syntrac_opentelemetry_instrumentation_replicate-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6390 2024-04-16 14:34:40.467548 syntrac_opentelemetry_instrumentation_replicate-0.0.2/syntrac_opentelemetry/instrumentation/replicate/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-16 14:34:40.468387 syntrac_opentelemetry_instrumentation_replicate-0.0.2/syntrac_opentelemetry/instrumentation/replicate/version.py
+-rw-r--r--   0        0        0     2309 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_replicate-0.0.2/PKG-INFO
```

### Comparing `syntrac_opentelemetry_instrumentation_replicate-0.0.1/README.md` & `syntrac_opentelemetry_instrumentation_replicate-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_replicate-0.0.1/syntrac_opentelemetry/instrumentation/replicate/__init__.py` & `syntrac_opentelemetry_instrumentation_replicate-0.0.2/syntrac_opentelemetry/instrumentation/replicate/__init__.py`

 * *Files identical despite different names*

