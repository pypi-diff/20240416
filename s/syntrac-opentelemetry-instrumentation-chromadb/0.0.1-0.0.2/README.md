# Comparing `tmp/syntrac_opentelemetry_instrumentation_chromadb-0.0.1.tar.gz` & `tmp/syntrac_opentelemetry_instrumentation_chromadb-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntrac_opentelemetry_instrumentation_chromadb-0.0.1.tar", max compression
+gzip compressed data, was "syntrac_opentelemetry_instrumentation_chromadb-0.0.2.tar", max compression
```

## Comparing `syntrac_opentelemetry_instrumentation_chromadb-0.0.1.tar` & `syntrac_opentelemetry_instrumentation_chromadb-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      603 2024-03-31 06:26:26.592259 syntrac_opentelemetry_instrumentation_chromadb-0.0.1/README.md
--rw-r--r--   0        0        0     2452 2024-03-31 06:26:26.958696 syntrac_opentelemetry_instrumentation_chromadb-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3029 2024-03-31 06:26:26.597813 syntrac_opentelemetry_instrumentation_chromadb-0.0.1/syntrac_opentelemetry/instrumentation/chromadb/__init__.py
--rw-r--r--   0        0        0       22 2024-03-31 06:26:26.600512 syntrac_opentelemetry_instrumentation_chromadb-0.0.1/syntrac_opentelemetry/instrumentation/chromadb/version.py
--rw-r--r--   0        0        0     9602 2024-03-31 06:26:26.600683 syntrac_opentelemetry_instrumentation_chromadb-0.0.1/syntrac_opentelemetry/instrumentation/chromadb/wrapper.py
--rw-r--r--   0        0        0     2343 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_chromadb-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      603 2024-04-16 14:25:04.468837 syntrac_opentelemetry_instrumentation_chromadb-0.0.2/README.md
+-rw-r--r--   0        0        0     1173 2024-04-16 14:25:04.477552 syntrac_opentelemetry_instrumentation_chromadb-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3029 2024-04-16 14:25:04.471473 syntrac_opentelemetry_instrumentation_chromadb-0.0.2/syntrac_opentelemetry/instrumentation/chromadb/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-16 14:25:04.472631 syntrac_opentelemetry_instrumentation_chromadb-0.0.2/syntrac_opentelemetry/instrumentation/chromadb/version.py
+-rw-r--r--   0        0        0     9600 2024-04-16 14:25:04.472752 syntrac_opentelemetry_instrumentation_chromadb-0.0.2/syntrac_opentelemetry/instrumentation/chromadb/wrapper.py
+-rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_chromadb-0.0.2/PKG-INFO
```

### Comparing `syntrac_opentelemetry_instrumentation_chromadb-0.0.1/README.md` & `syntrac_opentelemetry_instrumentation_chromadb-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_chromadb-0.0.1/syntrac_opentelemetry/instrumentation/chromadb/__init__.py` & `syntrac_opentelemetry_instrumentation_chromadb-0.0.2/syntrac_opentelemetry/instrumentation/chromadb/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_chromadb-0.0.1/syntrac_opentelemetry/instrumentation/chromadb/wrapper.py` & `syntrac_opentelemetry_instrumentation_chromadb-0.0.2/syntrac_opentelemetry/instrumentation/chromadb/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,15 +195,15 @@
         [
             {"id": 1, "distance": 0.3,  "document": "retrieved text", "metadata": "some metadata text",
             {"id": 2, "distance" 0.5, , "document": "retrieved text2": "another metadata text",
             {"id": 3, "distance": 0.6, "document": ..., "metadata": ...
         ]
 
     If you'd like to understand better why, please read the discussions on PR #370:
-    https://github.com/syntrac/openllmetry/pull/370
+    https://github.com/syntracAI/syntrac/pull/370
 
     The goal is to set a canonical format which we call as a Semantic Convention.
     """
     zipped = itertools.zip_longest(
         kwargs.get("ids", []),
         kwargs.get("distances", []),
         kwargs.get("metadatas", []),
```

