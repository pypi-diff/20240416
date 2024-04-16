# Comparing `tmp/syntrac_opentelemetry_instrumentation_watsonx-0.0.1.tar.gz` & `tmp/syntrac_opentelemetry_instrumentation_watsonx-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntrac_opentelemetry_instrumentation_watsonx-0.0.1.tar", max compression
+gzip compressed data, was "syntrac_opentelemetry_instrumentation_watsonx-0.0.2.tar", max compression
```

## Comparing `syntrac_opentelemetry_instrumentation_watsonx-0.0.1.tar` & `syntrac_opentelemetry_instrumentation_watsonx-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1507 2024-03-31 06:45:46.118247 syntrac_opentelemetry_instrumentation_watsonx-0.0.1/README.md
--rw-r--r--   0        0        0     2078 2024-03-31 06:45:46.389965 syntrac_opentelemetry_instrumentation_watsonx-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    17262 2024-03-31 06:45:46.120638 syntrac_opentelemetry_instrumentation_watsonx-0.0.1/syntrac_opentelemetry/instrumentation/watsonx/__init__.py
--rw-r--r--   0        0        0       22 2024-03-31 06:45:46.122022 syntrac_opentelemetry_instrumentation_watsonx-0.0.1/syntrac_opentelemetry/instrumentation/watsonx/version.py
--rw-r--r--   0        0        0     3208 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_watsonx-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1507 2024-04-16 14:36:00.917817 syntrac_opentelemetry_instrumentation_watsonx-0.0.2/README.md
+-rw-r--r--   0        0        0      801 2024-04-16 14:36:00.924077 syntrac_opentelemetry_instrumentation_watsonx-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    17262 2024-04-16 14:36:00.919796 syntrac_opentelemetry_instrumentation_watsonx-0.0.2/syntrac_opentelemetry/instrumentation/watsonx/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-16 14:36:00.920798 syntrac_opentelemetry_instrumentation_watsonx-0.0.2/syntrac_opentelemetry/instrumentation/watsonx/version.py
+-rw-r--r--   0        0        0     2574 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_watsonx-0.0.2/PKG-INFO
```

### Comparing `syntrac_opentelemetry_instrumentation_watsonx-0.0.1/README.md` & `syntrac_opentelemetry_instrumentation_watsonx-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_watsonx-0.0.1/syntrac_opentelemetry/instrumentation/watsonx/__init__.py` & `syntrac_opentelemetry_instrumentation_watsonx-0.0.2/syntrac_opentelemetry/instrumentation/watsonx/__init__.py`

 * *Files identical despite different names*

