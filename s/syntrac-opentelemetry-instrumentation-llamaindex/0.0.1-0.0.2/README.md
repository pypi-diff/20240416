# Comparing `tmp/syntrac_opentelemetry_instrumentation_llamaindex-0.0.1.tar.gz` & `tmp/syntrac_opentelemetry_instrumentation_llamaindex-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntrac_opentelemetry_instrumentation_llamaindex-0.0.1.tar", max compression
+gzip compressed data, was "syntrac_opentelemetry_instrumentation_llamaindex-0.0.2.tar", max compression
```

## Comparing `syntrac_opentelemetry_instrumentation_llamaindex-0.0.1.tar` & `syntrac_opentelemetry_instrumentation_llamaindex-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1171 2024-03-31 06:42:14.679337 syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/README.md
--rw-r--r--   0        0        0     3681 2024-03-31 06:42:15.078915 syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2197 2024-03-31 06:42:14.682888 syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/syntrac_opentelemetry/instrumentation/llamaindex/__init__.py
--rw-r--r--   0        0        0     2252 2024-03-31 06:42:14.686087 syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/syntrac_opentelemetry/instrumentation/llamaindex/base_agent_instrumentor.py
--rw-r--r--   0        0        0     2061 2024-03-31 06:42:14.686211 syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/syntrac_opentelemetry/instrumentation/llamaindex/base_embedding_instrumentor.py
--rw-r--r--   0        0        0     1961 2024-03-31 06:42:14.686336 syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/syntrac_opentelemetry/instrumentation/llamaindex/base_retriever_instrumentor.py
--rw-r--r--   0        0        0     1980 2024-03-31 06:42:14.686455 syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/syntrac_opentelemetry/instrumentation/llamaindex/base_synthesizer_instrumentor.py
--rw-r--r--   0        0        0     2365 2024-03-31 06:42:14.686570 syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/syntrac_opentelemetry/instrumentation/llamaindex/base_tool_instrumentor.py
--rw-r--r--   0        0        0     5704 2024-03-31 06:42:14.686689 syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/syntrac_opentelemetry/instrumentation/llamaindex/custom_llm_instrumentor.py
--rw-r--r--   0        0        0     2103 2024-03-31 06:42:14.686883 syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/syntrac_opentelemetry/instrumentation/llamaindex/query_pipeline_instrumentor.py
--rw-r--r--   0        0        0     2234 2024-03-31 06:42:14.687010 syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/syntrac_opentelemetry/instrumentation/llamaindex/retriever_query_engine_instrumentor.py
--rw-r--r--   0        0        0      685 2024-03-31 06:42:14.687132 syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/syntrac_opentelemetry/instrumentation/llamaindex/utils.py
--rw-r--r--   0        0        0       22 2024-03-31 06:42:14.687244 syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/syntrac_opentelemetry/instrumentation/llamaindex/version.py
--rw-r--r--   0        0        0     3604 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1171 2024-04-16 14:33:17.741490 syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/README.md
+-rw-r--r--   0        0        0     1240 2024-04-16 14:33:17.752304 syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2197 2024-04-16 14:33:17.744403 syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/syntrac_opentelemetry/instrumentation/llamaindex/__init__.py
+-rw-r--r--   0        0        0     2252 2024-04-16 14:33:17.746785 syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/syntrac_opentelemetry/instrumentation/llamaindex/base_agent_instrumentor.py
+-rw-r--r--   0        0        0     2061 2024-04-16 14:33:17.746907 syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/syntrac_opentelemetry/instrumentation/llamaindex/base_embedding_instrumentor.py
+-rw-r--r--   0        0        0     1961 2024-04-16 14:33:17.747029 syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/syntrac_opentelemetry/instrumentation/llamaindex/base_retriever_instrumentor.py
+-rw-r--r--   0        0        0     1980 2024-04-16 14:33:17.747155 syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/syntrac_opentelemetry/instrumentation/llamaindex/base_synthesizer_instrumentor.py
+-rw-r--r--   0        0        0     2365 2024-04-16 14:33:17.747264 syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/syntrac_opentelemetry/instrumentation/llamaindex/base_tool_instrumentor.py
+-rw-r--r--   0        0        0     5704 2024-04-16 14:33:17.747376 syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/syntrac_opentelemetry/instrumentation/llamaindex/custom_llm_instrumentor.py
+-rw-r--r--   0        0        0     2103 2024-04-16 14:33:17.747543 syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/syntrac_opentelemetry/instrumentation/llamaindex/query_pipeline_instrumentor.py
+-rw-r--r--   0        0        0     2234 2024-04-16 14:33:17.747666 syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/syntrac_opentelemetry/instrumentation/llamaindex/retriever_query_engine_instrumentor.py
+-rw-r--r--   0        0        0      685 2024-04-16 14:33:17.747775 syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/syntrac_opentelemetry/instrumentation/llamaindex/utils.py
+-rw-r--r--   0        0        0       22 2024-04-16 14:33:17.747886 syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/syntrac_opentelemetry/instrumentation/llamaindex/version.py
+-rw-r--r--   0        0        0     2364 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/PKG-INFO
```

### Comparing `syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/README.md` & `syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/syntrac_opentelemetry/instrumentation/llamaindex/__init__.py` & `syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/syntrac_opentelemetry/instrumentation/llamaindex/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/syntrac_opentelemetry/instrumentation/llamaindex/base_agent_instrumentor.py` & `syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/syntrac_opentelemetry/instrumentation/llamaindex/base_agent_instrumentor.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/syntrac_opentelemetry/instrumentation/llamaindex/base_embedding_instrumentor.py` & `syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/syntrac_opentelemetry/instrumentation/llamaindex/base_embedding_instrumentor.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/syntrac_opentelemetry/instrumentation/llamaindex/base_retriever_instrumentor.py` & `syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/syntrac_opentelemetry/instrumentation/llamaindex/base_retriever_instrumentor.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/syntrac_opentelemetry/instrumentation/llamaindex/base_synthesizer_instrumentor.py` & `syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/syntrac_opentelemetry/instrumentation/llamaindex/base_synthesizer_instrumentor.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/syntrac_opentelemetry/instrumentation/llamaindex/base_tool_instrumentor.py` & `syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/syntrac_opentelemetry/instrumentation/llamaindex/base_tool_instrumentor.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/syntrac_opentelemetry/instrumentation/llamaindex/custom_llm_instrumentor.py` & `syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/syntrac_opentelemetry/instrumentation/llamaindex/custom_llm_instrumentor.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/syntrac_opentelemetry/instrumentation/llamaindex/query_pipeline_instrumentor.py` & `syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/syntrac_opentelemetry/instrumentation/llamaindex/query_pipeline_instrumentor.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/syntrac_opentelemetry/instrumentation/llamaindex/retriever_query_engine_instrumentor.py` & `syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/syntrac_opentelemetry/instrumentation/llamaindex/retriever_query_engine_instrumentor.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_llamaindex-0.0.1/syntrac_opentelemetry/instrumentation/llamaindex/utils.py` & `syntrac_opentelemetry_instrumentation_llamaindex-0.0.2/syntrac_opentelemetry/instrumentation/llamaindex/utils.py`

 * *Files identical despite different names*

