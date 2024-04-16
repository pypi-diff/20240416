# Comparing `tmp/langchain_benchmarks-0.0.8.tar.gz` & `tmp/langchain_benchmarks-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_benchmarks-0.0.8.tar", max compression
+gzip compressed data, was "langchain_benchmarks-0.0.9.tar", max compression
```

## Comparing `langchain_benchmarks-0.0.8.tar` & `langchain_benchmarks-0.0.9.tar`

### file list

```diff
@@ -1,56 +1,66 @@
--rw-r--r--   0        0        0     1069 2023-12-12 16:39:45.835391 langchain_benchmarks-0.0.8/LICENSE
--rw-r--r--   0        0        0     3102 2023-12-12 16:39:45.835391 langchain_benchmarks-0.0.8/README.md
--rw-r--r--   0        0        0        5 2023-12-12 16:39:45.879391 langchain_benchmarks-0.0.8/langchain_benchmarks/.gitignore
--rw-r--r--   0        0        0      375 2023-12-12 16:39:45.879391 langchain_benchmarks-0.0.8/langchain_benchmarks/__init__.py
--rw-r--r--   0        0        0      282 2023-12-12 16:39:45.879391 langchain_benchmarks-0.0.8/langchain_benchmarks/extraction/__init__.py
--rw-r--r--   0        0        0     1767 2023-12-12 16:39:45.879391 langchain_benchmarks-0.0.8/langchain_benchmarks/extraction/evaluators.py
--rw-r--r--   0        0        0     2397 2023-12-12 16:39:45.879391 langchain_benchmarks-0.0.8/langchain_benchmarks/extraction/implementations.py
--rw-r--r--   0        0        0        0 2023-12-12 16:39:45.879391 langchain_benchmarks-0.0.8/langchain_benchmarks/extraction/tasks/__init__.py
--rw-r--r--   0        0        0     1497 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/extraction/tasks/chat_extraction/__init__.py
--rw-r--r--   0        0        0     5550 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/extraction/tasks/chat_extraction/evaluators.py
--rw-r--r--   0        0        0     3728 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/extraction/tasks/chat_extraction/schema.py
--rw-r--r--   0        0        0     2058 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/extraction/tasks/email_task.py
--rw-r--r--   0        0        0     7736 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/model_registration.py
--rw-r--r--   0        0        0        6 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/.gitignore
--rw-r--r--   0        0        0      207 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/__init__.py
--rw-r--r--   0        0        0     4696 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/evaluators.py
--rw-r--r--   0        0        0        6 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/.gitignore
--rw-r--r--   0        0        0      443 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/__init__.py
--rw-r--r--   0        0        0      474 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/langchain_docs/README.md
--rw-r--r--   0        0        0      343 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/langchain_docs/__init__.py
--rw-r--r--   0        0        0    12473 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/langchain_docs/_ingest_docs.py
--rw-r--r--   0        0        0      141 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/langchain_docs/architectures/__init__.py
--rw-r--r--   0        0        0      994 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/langchain_docs/architectures/chain_registry.py
--rw-r--r--   0        0        0     4281 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/langchain_docs/architectures/crqa.py
--rw-r--r--   0        0        0       23 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/langchain_docs/indexing/.gitignore
--rw-r--r--   0        0        0      157 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/langchain_docs/indexing/__init__.py
--rw-r--r--   0        0        0     4205 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/langchain_docs/indexing/retriever_registry.py
--rw-r--r--   0        0        0     1310 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/langchain_docs/task.py
--rw-r--r--   0        0        0      149 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/multi_modal_slide_decks/__init__.py
--rw-r--r--   0        0        0      149 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/multi_modal_slide_decks/indexing/__init__.py
--rw-r--r--   0        0        0     1188 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/multi_modal_slide_decks/indexing/retriever_registry.py
--rw-r--r--   0        0        0      751 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/multi_modal_slide_decks/task.py
--rw-r--r--   0        0        0      317 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/semi_structured_reports/__init__.py
--rw-r--r--   0        0        0        6 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/semi_structured_reports/indexing/.gitignore
--rw-r--r--   0        0        0      187 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/semi_structured_reports/indexing/__init__.py
--rw-r--r--   0        0        0     6054 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/semi_structured_reports/indexing/retriever_registry.py
--rw-r--r--   0        0        0     1099 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/semi_structured_reports/task.py
--rw-r--r--   0        0        0        0 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/utils/__init__.py
--rw-r--r--   0        0        0      579 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/utils/_downloading.py
--rw-r--r--   0        0        0    10409 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/rag/utils/indexing.py
--rw-r--r--   0        0        0      951 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/registration.py
--rw-r--r--   0        0        0    15607 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/schema.py
--rw-r--r--   0        0        0      103 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/tool_usage/README.md
--rw-r--r--   0        0        0      307 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/tool_usage/__init__.py
--rw-r--r--   0        0        0     4838 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/tool_usage/agents.py
--rw-r--r--   0        0        0     7338 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/tool_usage/evaluators.py
--rw-r--r--   0        0        0     1083 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/tool_usage/prompts.py
--rw-r--r--   0        0        0        0 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/tool_usage/tasks/__init__.py
--rw-r--r--   0        0        0     7061 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/tool_usage/tasks/multiverse_math.py
--rw-r--r--   0        0        0    12336 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/tool_usage/tasks/relational_data.py
--rw-r--r--   0        0        0     4301 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/tool_usage/tasks/type_writer.py
--rw-r--r--   0        0        0     4665 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/tool_usage/tasks/type_writer_26_funcs.py
--rw-r--r--   0        0        0        0 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/utils/__init__.py
--rw-r--r--   0        0        0     4747 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/langchain_benchmarks/utils/_langsmith.py
--rw-r--r--   0        0        0     2096 2023-12-12 16:39:45.883391 langchain_benchmarks-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3735 1970-01-01 00:00:00.000000 langchain_benchmarks-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-12-14 18:25:53.963461 langchain_benchmarks-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3102 2023-12-14 18:25:53.963461 langchain_benchmarks-0.0.9/README.md
+-rw-r--r--   0        0        0        5 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/.gitignore
+-rw-r--r--   0        0        0      745 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/__init__.py
+-rw-r--r--   0        0        0      282 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/extraction/__init__.py
+-rw-r--r--   0        0        0     1767 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/extraction/evaluators.py
+-rw-r--r--   0        0        0     2397 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/extraction/implementations.py
+-rw-r--r--   0        0        0        0 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/extraction/tasks/__init__.py
+-rw-r--r--   0        0        0     1497 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/extraction/tasks/chat_extraction/__init__.py
+-rw-r--r--   0        0        0     5550 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/extraction/tasks/chat_extraction/evaluators.py
+-rw-r--r--   0        0        0     3728 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/extraction/tasks/chat_extraction/schema.py
+-rw-r--r--   0        0        0     2058 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/extraction/tasks/email_task.py
+-rw-r--r--   0        0        0     7765 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/model_registration.py
+-rw-r--r--   0        0        0        6 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/.gitignore
+-rw-r--r--   0        0        0      207 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/__init__.py
+-rw-r--r--   0        0        0     4696 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/evaluators.py
+-rw-r--r--   0        0        0        6 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/.gitignore
+-rw-r--r--   0        0        0      443 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/__init__.py
+-rw-r--r--   0        0        0      474 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/langchain_docs/README.md
+-rw-r--r--   0        0        0      343 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/langchain_docs/__init__.py
+-rw-r--r--   0        0        0    12473 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/langchain_docs/_ingest_docs.py
+-rw-r--r--   0        0        0      141 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/langchain_docs/architectures/__init__.py
+-rw-r--r--   0        0        0      994 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/langchain_docs/architectures/chain_registry.py
+-rw-r--r--   0        0        0     4281 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/langchain_docs/architectures/crqa.py
+-rw-r--r--   0        0        0       23 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/langchain_docs/indexing/.gitignore
+-rw-r--r--   0        0        0      157 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/langchain_docs/indexing/__init__.py
+-rw-r--r--   0        0        0     4205 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/langchain_docs/indexing/retriever_registry.py
+-rw-r--r--   0        0        0     1310 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/langchain_docs/task.py
+-rw-r--r--   0        0        0      149 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/multi_modal_slide_decks/__init__.py
+-rw-r--r--   0        0        0      149 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/multi_modal_slide_decks/indexing/__init__.py
+-rw-r--r--   0        0        0     1188 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/multi_modal_slide_decks/indexing/retriever_registry.py
+-rw-r--r--   0        0        0      751 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/multi_modal_slide_decks/task.py
+-rw-r--r--   0        0        0      317 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/semi_structured_reports/__init__.py
+-rw-r--r--   0        0        0        6 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/semi_structured_reports/indexing/.gitignore
+-rw-r--r--   0        0        0      187 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/semi_structured_reports/indexing/__init__.py
+-rw-r--r--   0        0        0     6054 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/semi_structured_reports/indexing/retriever_registry.py
+-rw-r--r--   0        0        0     1099 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/semi_structured_reports/task.py
+-rw-r--r--   0        0        0        0 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/utils/__init__.py
+-rw-r--r--   0        0        0      579 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/utils/_downloading.py
+-rw-r--r--   0        0        0    10409 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rag/utils/indexing.py
+-rw-r--r--   0        0        0     4006 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/rate_limiting.py
+-rw-r--r--   0        0        0      951 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/registration.py
+-rw-r--r--   0        0        0    15772 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/schema.py
+-rw-r--r--   0        0        0      103 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/README.md
+-rw-r--r--   0        0        0      307 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/__init__.py
+-rw-r--r--   0        0        0      364 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/agents/__init__.py
+-rw-r--r--   0        0        0     2451 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/agents/adapters.py
+-rw-r--r--   0        0        0        0 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/agents/experimental/__init__.py
+-rw-r--r--   0        0        0     4475 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/agents/experimental/agent.py
+-rw-r--r--   0        0        0     7619 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/agents/experimental/encoder.py
+-rw-r--r--   0        0        0     3078 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/agents/experimental/factory.py
+-rw-r--r--   0        0        0     4221 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/agents/experimental/parser.py
+-rw-r--r--   0        0        0     1171 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/agents/experimental/prompts.py
+-rw-r--r--   0        0        0     1625 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/agents/experimental/tool_utils.py
+-rw-r--r--   0        0        0     2930 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/agents/openai_functions.py
+-rw-r--r--   0        0        0     7338 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/evaluators.py
+-rw-r--r--   0        0        0     1083 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/prompts.py
+-rw-r--r--   0        0        0        0 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/tasks/__init__.py
+-rw-r--r--   0        0        0     7061 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/tasks/multiverse_math.py
+-rw-r--r--   0        0        0    12336 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/tasks/relational_data.py
+-rw-r--r--   0        0        0     4301 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/tasks/type_writer.py
+-rw-r--r--   0        0        0     4665 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/tasks/type_writer_26_funcs.py
+-rw-r--r--   0        0        0        0 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/utils/__init__.py
+-rw-r--r--   0        0        0     4747 2023-12-14 18:25:54.011460 langchain_benchmarks-0.0.9/langchain_benchmarks/utils/_langsmith.py
+-rw-r--r--   0        0        0     1932 2023-12-14 18:25:54.015460 langchain_benchmarks-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3735 1970-01-01 00:00:00.000000 langchain_benchmarks-0.0.9/PKG-INFO
```

### Comparing `langchain_benchmarks-0.0.8/LICENSE` & `langchain_benchmarks-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/README.md` & `langchain_benchmarks-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/extraction/evaluators.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/extraction/evaluators.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/extraction/implementations.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/extraction/implementations.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/extraction/tasks/chat_extraction/__init__.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/extraction/tasks/chat_extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/extraction/tasks/chat_extraction/evaluators.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/extraction/tasks/chat_extraction/evaluators.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/extraction/tasks/chat_extraction/schema.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/extraction/tasks/chat_extraction/schema.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/extraction/tasks/email_task.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/extraction/tasks/email_task.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/model_registration.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/model_registration.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,29 +190,28 @@
         description="70b parameter LlamaChat model",
         params={
             "model": "accounts/fireworks/models/llama-v2-70b-chat",
         },
     ),
     RegisteredModel(
         provider="fireworks",
-        name="mixtral-8x7b-fw-chat",
-        description="8x7b parameter mixture of experts Mistral model, adapted for Chats",
-        type="chat",
+        name="yi-34b-200k-fw",
+        type="llm",
+        description=" 4B LLM model from 01.ai, with context window 200k.",
         params={
-            "model": "accounts/fireworks/models/mixtral-8x7b-fw-chat",
+            "model": "accounts/fireworks/models/yi-34b-200k",
         },
     ),
     RegisteredModel(
         provider="fireworks",
-        name="mixtral-8x7b-fw-llm",
-        description="8x7b parameter mixture of experts Mistral model",
+        name="mixtral-8x7b-instruct-fw",
+        description="Mistral MoE 8x7B Instruct v0.1 model with Sparse "
+        "Mixture of Experts. Fine tuned for instruction following",
         type="llm",
-        params={
-            "model": "accounts/fireworks/models/mixtral-8x7b",
-        },
+        params={"model": "accounts/fireworks/models/mixtral-8x7b-instruct"},
     ),
 ]
 
 _ANTHROPIC_MODELS = [
     RegisteredModel(
         provider="anthropic",
         name="claude-2",
```

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/rag/evaluators.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/rag/evaluators.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/langchain_docs/_ingest_docs.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/langchain_docs/_ingest_docs.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/langchain_docs/architectures/chain_registry.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/langchain_docs/architectures/chain_registry.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/langchain_docs/architectures/crqa.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/langchain_docs/architectures/crqa.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/langchain_docs/indexing/retriever_registry.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/langchain_docs/indexing/retriever_registry.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/langchain_docs/task.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/langchain_docs/task.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/multi_modal_slide_decks/indexing/retriever_registry.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/multi_modal_slide_decks/indexing/retriever_registry.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/multi_modal_slide_decks/task.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/multi_modal_slide_decks/task.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/semi_structured_reports/indexing/retriever_registry.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/semi_structured_reports/indexing/retriever_registry.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/rag/tasks/semi_structured_reports/task.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/rag/tasks/semi_structured_reports/task.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/rag/utils/_downloading.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/rag/utils/_downloading.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/rag/utils/indexing.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/rag/utils/indexing.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/registration.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/registration.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/schema.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,15 +253,15 @@
 
 Provider = Literal["fireworks", "openai", "anthropic"]
 ModelType = Literal["chat", "llm"]
 AUTHORIZED_NAMESPACES = {"langchain"}
 
 
 def _get_model_class_from_path(
-    path: str
+    path: str,
 ) -> Union[Type[BaseChatModel], Type[BaseLanguageModel]]:
     """Get the class of the model."""
     module_name, attribute_name = path.rsplit(".", 1)
     top_namespace = path.split(".")[0]
 
     if top_namespace not in AUTHORIZED_NAMESPACES:
         raise ValueError(
@@ -442,14 +442,18 @@
         ]
         return tabulate(table, headers=headers, tablefmt="unsafehtml")
 
     def __len__(self) -> int:
         """Return the number of tasks in the registry."""
         return len(self.registered_models)
 
+    def __contains__(self, item: Any) -> bool:
+        """Return whether the registry contains the given model."""
+        return self.get_model(item) is not None
+
     def __iter__(self) -> Iterable[RegisteredModel]:
         """Iterate over the tasks in the registry."""
         return iter(self.registered_models)
 
     def __getitem__(
         self, key: Union[int, str, slice]
     ) -> Union[RegisteredModel, ModelRegistry]:
```

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/tool_usage/evaluators.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/evaluators.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/tool_usage/prompts.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/prompts.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/tool_usage/tasks/multiverse_math.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/tasks/multiverse_math.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/tool_usage/tasks/relational_data.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/tasks/relational_data.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/tool_usage/tasks/type_writer.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/tasks/type_writer.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/tool_usage/tasks/type_writer_26_funcs.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/tool_usage/tasks/type_writer_26_funcs.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/langchain_benchmarks/utils/_langsmith.py` & `langchain_benchmarks-0.0.9/langchain_benchmarks/utils/_langsmith.py`

 * *Files identical despite different names*

### Comparing `langchain_benchmarks-0.0.8/pyproject.toml` & `langchain_benchmarks-0.0.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-benchmarks"
-version = "0.0.8"
+version = "0.0.9"
 description = "🦜💪 Flex those feathers!"
 authors = ["LangChain AI"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
@@ -37,32 +37,30 @@
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 pytest-asyncio = "^0.21.1"
 pytest-mock = "^3.11.1"
 pytest-socket = "^0.6.0"
 pytest-watch = "^4.2.0"
 pytest-timeout = "^2.2.0"
+freezegun = "^1.3.1"
 
 
 [tool.ruff]
 select = [
     "E",  # pycodestyle
     "F",  # pyflakes
     "I",  # isort
 ]
 extend-include = ["*.ipynb"]
 
 # Same as Black.
 line-length = 88
 
 [tool.ruff.isort]
-# TODO(Team): Temporary to make isort work with examples.
-# examples assume langserve is available as a 3rd party package
-# For simplicity we'll define it as first party for now can update later.
-known-first-party = ["langserve"]
+known-first-party = ["langchain-benchmarks"]
 
 [tool.mypy]
 disallow_untyped_defs = "True"
 ignore_missing_imports = "True"
 
 [tool.coverage.run]
 omit = [
```

### Comparing `langchain_benchmarks-0.0.8/PKG-INFO` & `langchain_benchmarks-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-benchmarks
-Version: 0.0.8
+Version: 0.0.9
 Summary: 🦜💪 Flex those feathers!
 License: MIT
 Author: LangChain AI
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

