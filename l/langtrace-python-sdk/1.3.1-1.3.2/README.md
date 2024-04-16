# Comparing `tmp/langtrace_python_sdk-1.3.1.tar.gz` & `tmp/langtrace_python_sdk-1.3.2.tar.gz`

## Comparing `langtrace_python_sdk-1.3.1.tar` & `langtrace_python_sdk-1.3.2.tar`

### file list

```diff
@@ -1,86 +1,88 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/__init__.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/run_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/anthropic_example/__init__.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/anthropic_example/completion.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/chroma_example/__init__.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/chroma_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/cohere_example/__init__.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/cohere_example/chat.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/cohere_example/chat_stream.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/cohere_example/embed_create.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/fastapi_example/basic_route.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/langchain_example/__init__.py
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/langchain_example/basic.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/langchain_example/tool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/llamaindex_example/__init__.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/llamaindex_example/basic.py
--rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/llamaindex_example/data/abramov.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/openai/__init__.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/openai/chat_completion.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/openai/embeddings_create.py
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/openai/function_calling.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/openai/images_generate.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/perplexity_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/pinecone_example/__init__.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/examples/pinecone_example/basic.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/__init__.py
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/langtrace.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/instrumentation/__init__.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/instrumentation/chroma.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/instrumentation/cohere.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/instrumentation/common.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/instrumentation/openai.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/extensions/__init__.py
--rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/extensions/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
--rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/chroma/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
--rw-r--r--   0        0        0    15727 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/cohere/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
--rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
--rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
--rw-r--r--   0        0        0     7959 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
--rw-r--r--   0        0        0    15463 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/openai/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/utils/__init__.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/utils/llm.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/utils/with_root_span.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/tests/__init__.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/tests/utils.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/tests/anthropic/test_anthropic.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/tests/chroma/test_chroma.py
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/tests/langchain/test_langchain.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/tests/langchain/test_langchain_community.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/tests/langchain/test_langchain_core.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/tests/openai/test_chat_completion.py
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/tests/openai/test_image_generation.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/src/tests/pinecone/test_pinecone.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/LICENSE
--rw-r--r--   0        0        0     8044 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/README.md
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     9061 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/__init__.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/run_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/anthropic_example/__init__.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/anthropic_example/completion.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/chroma_example/__init__.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/chroma_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/cohere_example/__init__.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/cohere_example/chat.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/cohere_example/chat_stream.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/cohere_example/embed_create.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/fastapi_example/basic_route.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/hiveagent_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/langchain_example/__init__.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/langchain_example/basic.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/langchain_example/tool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/llamaindex_example/__init__.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/llamaindex_example/agent.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/llamaindex_example/basic.py
+-rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/llamaindex_example/data/abramov.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/openai/__init__.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/openai/chat_completion.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/openai/embeddings_create.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/openai/function_calling.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/openai/images_generate.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/perplexity_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/pinecone_example/__init__.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/examples/pinecone_example/basic.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/__init__.py
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/langtrace.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/constants/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/constants/instrumentation/__init__.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/constants/instrumentation/chroma.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/constants/instrumentation/cohere.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/constants/instrumentation/common.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/constants/instrumentation/openai.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/extensions/__init__.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/extensions/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
+-rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/chroma/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
+-rw-r--r--   0        0        0    16631 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/cohere/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/langchain/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
+-rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
+-rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
+-rw-r--r--   0        0        0     7959 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
+-rw-r--r--   0        0        0    31587 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/openai/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/utils/llm.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/utils/with_root_span.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/tests/__init__.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/tests/utils.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/tests/anthropic/test_anthropic.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/tests/chroma/test_chroma.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/tests/langchain/test_langchain.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/tests/langchain/test_langchain_community.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/tests/langchain/test_langchain_core.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/tests/openai/test_chat_completion.py
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/tests/openai/test_image_generation.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/src/tests/pinecone/test_pinecone.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/LICENSE
+-rw-r--r--   0        0        0     8031 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/README.md
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.3.2/PKG-INFO
```

### Comparing `langtrace_python_sdk-1.3.1/src/run_example.py` & `langtrace_python_sdk-1.3.2/src/run_example.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 # from examples.anthropic_example.completion import messages_create
 
 # from examples.pinecone_example.basic import basic
 # from examples.chroma_example.basic import basic
 # from examples.llamaindex_example.basic import basic
 # from examples.langchain_example.basic import basic
 # from examples.cohere_example.chat import chat_comp
-from examples.cohere_example.embed_create import embed_create
+# from examples.cohere_example.embed_create import embed_create
+from examples.hiveagent_example.basic import basic
+
 # from examples.cohere_example.chat_stream import chat_stream
 
 # from examples.perplexity_example.basic import basic
 
 # load_and_split()
 # rag()
-# basic()
+basic()
 # chat_completion()
 # function_calling()
 # images_generate()
 # embeddings_create()
 # messages_create()
 # chat_comp()
-embed_create()
+# embed_create()
 # chat_stream()
```

### Comparing `langtrace_python_sdk-1.3.1/src/examples/anthropic_example/completion.py` & `langtrace_python_sdk-1.3.2/src/examples/anthropic_example/completion.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dotenv import find_dotenv, load_dotenv
 
 from langtrace_python_sdk import langtrace
 from langtrace_python_sdk import with_langtrace_root_span
 
 _ = load_dotenv(find_dotenv())
 
-langtrace.init(batch=False, debug_log_to_console=True, write_to_langtrace_cloud=False)
+langtrace.init(write_to_langtrace_cloud=False)
 
 @with_langtrace_root_span("messages_create")
 def messages_create():
 
     client = anthropic.Anthropic()
 
     message = client.messages.create(
```

### Comparing `langtrace_python_sdk-1.3.1/src/examples/chroma_example/basic.py` & `langtrace_python_sdk-1.3.2/src/examples/chroma_example/basic.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dotenv import find_dotenv, load_dotenv
 
 from langtrace_python_sdk import langtrace
 from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
 
 _ = load_dotenv(find_dotenv())
 
-langtrace.init(batch=False, debug_log_to_console=True, write_to_langtrace_cloud=False)
+langtrace.init(write_to_langtrace_cloud=False)
 
 
 @with_langtrace_root_span()
 def basic():
     chroma_client = chromadb.Client()
     embedder = embedding_functions.DefaultEmbeddingFunction()
     collection = chroma_client.create_collection(
```

### Comparing `langtrace_python_sdk-1.3.1/src/examples/cohere_example/chat.py` & `langtrace_python_sdk-1.3.2/src/examples/cohere_example/chat.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import cohere
 
 from langtrace_python_sdk import langtrace
 # from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
 
 _ = load_dotenv(find_dotenv())
 
-langtrace.init(batch=False, debug_log_to_console=True, write_to_langtrace_cloud=False)
+langtrace.init(write_to_langtrace_cloud=False)
 
 co = cohere.Client()
 
 
 # @with_langtrace_root_span("chat_create")
 def chat_comp():
     response = co.chat(
```

### Comparing `langtrace_python_sdk-1.3.1/src/examples/cohere_example/chat_stream.py` & `langtrace_python_sdk-1.3.2/src/examples/cohere_example/chat_stream.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from dotenv import find_dotenv, load_dotenv
 import cohere
 
 from langtrace_python_sdk import langtrace
+
 # from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
 
 _ = load_dotenv(find_dotenv())
 
-langtrace.init(batch=False, debug_log_to_console=True, write_to_langtrace_cloud=False)
+langtrace.init(write_to_langtrace_cloud=False)
 
 co = cohere.Client()
 
 
 # @with_langtrace_root_span("chat_stream")
 def chat_stream():
     result = []
```

### Comparing `langtrace_python_sdk-1.3.1/src/examples/cohere_example/embed_create.py` & `langtrace_python_sdk-1.3.2/src/examples/cohere_example/embed_create.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from dotenv import find_dotenv, load_dotenv
 import cohere
 
 from langtrace_python_sdk import langtrace
+
 # from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
 
 _ = load_dotenv(find_dotenv())
 
-langtrace.init(batch=False, debug_log_to_console=True, write_to_langtrace_cloud=False)
+langtrace.init(write_to_langtrace_cloud=False)
 
 co = cohere.Client()
 
 
 # @with_langtrace_root_span("embed_create")
 def embed_create():
     response = co.embed(
-        texts=['hello', 'goodbye'],
-        model='embed-english-v3.0',
-        input_type='classification'
+        texts=["hello", "goodbye"],
+        model="embed-english-v3.0",
+        input_type="classification",
     )
     # print(response)
```

### Comparing `langtrace_python_sdk-1.3.1/src/examples/fastapi_example/basic_route.py` & `langtrace_python_sdk-1.3.2/src/examples/fastapi_example/basic_route.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 from langchain_core.prompts.chat import ChatPromptTemplate
 from langchain_core.runnables import RunnablePassthrough
 from langchain_openai import ChatOpenAI, OpenAIEmbeddings
 from openai import OpenAI
 
 from langtrace_python_sdk import langtrace
 
-langtrace.init(write_to_langtrace_cloud=False, debug_log_to_console=True)
+langtrace.init(write_to_langtrace_cloud=False)
 app = FastAPI()
 client = OpenAI()
 
+
 @app.get("/")
 def root():
     vectorstore = FAISS.from_texts(
-        ["Langtrace helps you ship high quality AI Apps to production."], embedding=OpenAIEmbeddings()
+        ["Langtrace helps you ship high quality AI Apps to production."],
+        embedding=OpenAIEmbeddings(),
     )
     retriever = vectorstore.as_retriever()
 
     template = """Answer the question based only on the following context:{context}
 
         Question: {question}
     """
```

### Comparing `langtrace_python_sdk-1.3.1/src/examples/langchain_example/basic.py` & `langtrace_python_sdk-1.3.2/src/examples/langchain_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/examples/langchain_example/tool.py` & `langtrace_python_sdk-1.3.2/src/examples/langchain_example/tool.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/examples/llamaindex_example/basic.py` & `langtrace_python_sdk-1.3.2/src/examples/llamaindex_example/basic.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from langtrace_python_sdk import langtrace
 from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
 
 _ = load_dotenv(find_dotenv())
 
 
-langtrace.init(batch=False, debug_log_to_console=True, write_to_langtrace_cloud=False)
+langtrace.init(write_to_langtrace_cloud=False)
 
 
 @with_langtrace_root_span()
 def basic():
     documents = SimpleDirectoryReader(
         "src/examples/llamaindex_example/data"
     ).load_data()
```

### Comparing `langtrace_python_sdk-1.3.1/src/examples/llamaindex_example/data/abramov.txt` & `langtrace_python_sdk-1.3.2/src/examples/llamaindex_example/data/abramov.txt`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/examples/openai/chat_completion.py` & `langtrace_python_sdk-1.3.2/src/examples/openai/chat_completion.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from langtrace_python_sdk import langtrace
 from langtrace_python_sdk.utils.with_root_span import (
     with_additional_attributes, with_langtrace_root_span)
 
 _ = load_dotenv(find_dotenv())
 
-langtrace.init()
+langtrace.init(write_to_langtrace_cloud=True)
 client = OpenAI()
 
 
 @with_additional_attributes({"user.id": "1234", "user.feedback.rating": 1})
 def api1():
     response = client.chat.completions.create(
         model="gpt-4",
```

### Comparing `langtrace_python_sdk-1.3.1/src/examples/openai/embeddings_create.py` & `langtrace_python_sdk-1.3.2/src/examples/openai/embeddings_create.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/examples/openai/function_calling.py` & `langtrace_python_sdk-1.3.2/src/examples/openai/function_calling.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from openai import OpenAI
 
 from langtrace_python_sdk import langtrace
 from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
 
 _ = load_dotenv(find_dotenv())
 
-langtrace.init(batch=False, debug_log_to_console=True, write_to_langtrace_cloud=False)
+langtrace.init(write_to_langtrace_cloud=False)
 
 client = OpenAI()
 
 
 student_custom_functions = [
     {
         "name": "extract_student_info",
```

### Comparing `langtrace_python_sdk-1.3.1/src/examples/perplexity_example/basic.py` & `langtrace_python_sdk-1.3.2/src/examples/perplexity_example/basic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from openai import OpenAI
 
 from langtrace_python_sdk import langtrace
 from langtrace_python_sdk.utils.with_root_span import (
-    with_additional_attributes, with_langtrace_root_span)
+    with_additional_attributes,
+    with_langtrace_root_span,
+)
 
 # _ = load_dotenv(find_dotenv())
 
-langtrace.init(batch=False, write_to_langtrace_cloud=False, debug_log_to_console=True)
+langtrace.init(write_to_langtrace_cloud=False)
 client = OpenAI(base_url="https://api.perplexity.ai", api_key="PPLX_API_KEY")
 
 
 @with_additional_attributes({"user.id": "1234", "user.feedback.rating": 1})
 def basic():
     response = client.chat.completions.create(
         model="pplx-70b-online",
         messages=[{"role": "user", "content": "What is the capital of France?"}],
         stream=False,
     )
     print(response)
-    return response
+    return response
```

### Comparing `langtrace_python_sdk-1.3.1/src/examples/pinecone_example/basic.py` & `langtrace_python_sdk-1.3.2/src/examples/pinecone_example/basic.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pinecone import Pinecone
 
 from langtrace_python_sdk import langtrace
 from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
 
 _ = load_dotenv(find_dotenv())
 
-langtrace.init(batch=False, debug_log_to_console=True, write_to_langtrace_cloud=False)
+langtrace.init(write_to_langtrace_cloud=False)
 
 client = OpenAI()
 pinecone = Pinecone()
 
 
 @with_langtrace_root_span()
 def basic():
```

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/langtrace.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/langtrace.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,41 +37,44 @@
 )
 
 
 def init(
     api_key: str = None,
     batch: bool = True,
     write_to_langtrace_cloud: bool = True,
-    debug_log_to_console: bool = False,
     custom_remote_exporter=None,
     api_host: Optional[str] = None,
 ):
     provider = TracerProvider()
 
     remote_write_exporter = (
         LangTraceExporter(api_key, write_to_langtrace_cloud, api_host=api_host)
         if custom_remote_exporter is None
         else custom_remote_exporter
     )
     console_exporter = ConsoleSpanExporter()
     batch_processor_remote = BatchSpanProcessor(remote_write_exporter)
+    simple_processor_remote = SimpleSpanProcessor(remote_write_exporter)
     batch_processor_console = BatchSpanProcessor(console_exporter)
     simple_processor_console = SimpleSpanProcessor(console_exporter)
 
-    if debug_log_to_console:
+    if write_to_langtrace_cloud:
+        provider.add_span_processor(batch_processor_remote)
+    elif custom_remote_exporter is not None:
+        if batch:
+            provider.add_span_processor(batch_processor_remote)
+        else:
+            provider.add_span_processor(simple_processor_remote)
+    else:
         if batch:
             provider.add_span_processor(batch_processor_console)
         else:
             provider.add_span_processor(simple_processor_console)
 
-    if write_to_langtrace_cloud:
-        if batch:
-            provider.add_span_processor(batch_processor_remote)
-        else:
-            raise ValueError("Batching is required for remote write")
+
 
     # Initialize tracer
     trace.set_tracer_provider(provider)
 
     openai_instrumentation = OpenAIInstrumentation()
     pinecone_instrumentation = PineconeInstrumentation()
     llamaindex_instrumentation = LlamaindexInstrumentation()
```

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/instrumentation/chroma.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/constants/instrumentation/chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/instrumentation/common.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/constants/instrumentation/common.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/constants/instrumentation/openai.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/constants/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/extensions/langtrace_exporter.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/extensions/langtrace_exporter.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 import os
 import typing
 
 import requests
 from opentelemetry.sdk.trace.export import ReadableSpan, SpanExporter, SpanExportResult
 from opentelemetry.trace.span import format_trace_id
 
-from langtrace_python_sdk.constants.exporter.langtrace_exporter import LANGTRACE_REMOTE_URL
+from langtrace_python_sdk.constants.exporter.langtrace_exporter import (
+    LANGTRACE_REMOTE_URL,
+)
 
 
 class LangTraceExporter(SpanExporter):
     """
     **LangTraceExporter Class**
 
     This class exports telemetry data in the LangTrace format to a remote URL. It inherits from the `SpanExporter` class in OpenTelemetry.
@@ -44,15 +46,20 @@
 
     * `ValueError`: If the API key is not provided or the URL is missing when `write_to_remote_url` is True.
     """
 
     api_key: str
     write_to_remote_url: bool
 
-    def __init__(self, api_key: str = None, write_to_remote_url: bool = False, api_host: typing.Optional[str] = None) -> None:
+    def __init__(
+        self,
+        api_key: str = None,
+        write_to_remote_url: bool = False,
+        api_host: typing.Optional[str] = None,
+    ) -> None:
         self.api_key = api_key or os.environ.get("LANGTRACE_API_KEY")
         self.write_to_remote_url = write_to_remote_url
         self.api_host: str = api_host or LANGTRACE_REMOTE_URL
 
         if self.write_to_remote_url and not self.api_key:
             raise ValueError("No API key provided")
 
@@ -85,13 +92,14 @@
         # Send data to remote URL
         try:
             requests.post(
                 url=f"{self.api_host}/api/trace",
                 data=json.dumps(data),
                 headers={"Content-Type": "application/json", "x-api-key": self.api_key},
             )
+            print(f"sent to {self.api_host}/api/trace with {len(data)} spans")
             return SpanExportResult.SUCCESS
         except Exception as e:
             return SpanExportResult.FAILURE
 
     def shutdown(self) -> None:
         pass
```

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/anthropic/patch.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/anthropic/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/chroma/patch.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/chroma/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/cohere/patch.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/cohere/patch.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 
 from langtrace.trace_attributes import Event, LLMSpanAttributes
 from opentelemetry import baggage
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
 
 from langtrace_python_sdk.constants.instrumentation.cohere import APIS
-from langtrace_python_sdk.constants.instrumentation.common import (LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY, SERVICE_PROVIDERS)
+from langtrace_python_sdk.constants.instrumentation.common import (
+    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
+    SERVICE_PROVIDERS,
+)
 from langtrace_python_sdk.utils.llm import estimate_tokens
 
 
 def embed_create(original_method, version, tracer):
     """Wrap the `embed_create` method."""
 
     def traced_method(wrapped, instance, args, kwargs):
@@ -29,25 +32,23 @@
             "url.full": APIS["EMBED_CREATE"]["URL"],
             "llm.api": APIS["EMBED_CREATE"]["ENDPOINT"],
             "llm.model": kwargs.get("model"),
             "llm.prompts": "",
             "llm.embedding_dataset_id": kwargs.get("dataset_id"),
             "llm.embedding_input_type": kwargs.get("input_type"),
             "llm.embedding_job_name": kwargs.get("name"),
-            **(extra_attributes if extra_attributes is not None else {})
+            **(extra_attributes if extra_attributes is not None else {}),
         }
 
         attributes = LLMSpanAttributes(**span_attributes)
 
         if kwargs.get("user") is not None:
             attributes.llm_user = kwargs.get("user")
 
-        span = tracer.start_span(
-            APIS["EMBED_CREATE"]["METHOD"], kind=SpanKind.CLIENT
-        )
+        span = tracer.start_span(APIS["EMBED_CREATE"]["METHOD"], kind=SpanKind.CLIENT)
         for field, value in attributes.model_dump(by_alias=True).items():
             if value is not None:
                 span.set_attribute(field, value)
         try:
             # Attempt to call the original method
             result = wrapped(*args, **kwargs)
             span.set_status(StatusCode.OK)
@@ -55,47 +56,46 @@
             return result
 
         except Exception as error:
             span.record_exception(error)
             span.set_status(Status(StatusCode.ERROR, str(error)))
             span.end()
             raise
+
     return traced_method
 
 
 def chat_create(original_method, version, tracer):
     """Wrap the `chat_create` method."""
 
     def traced_method(wrapped, instance, args, kwargs):
         service_provider = SERVICE_PROVIDERS["COHERE"]
 
         message = kwargs.get("message", "")
-        prompts = json.dumps([
-            {
-                "role": "USER",
-                "content": message
-            }
-        ])
+        prompts = json.dumps([{"role": "USER", "content": message}])
         preamble = kwargs.get("preamble")
         if preamble:
             prompts = json.dumps(
-                [{"role": "system", "content": preamble}] + [{"role": "USER", "content": message}]
+                [{"role": "system", "content": preamble}]
+                + [{"role": "USER", "content": message}]
             )
 
         chat_history = kwargs.get("chat_history")
         if chat_history:
             history = [
                 {
                     "message": {
                         "role": (
                             item.get("role") if item.get("role") is not None else "USER"
                         ),
                         "content": (
-                            item.get("message") if item.get("message") is not None else ""
-                        )
+                            item.get("message")
+                            if item.get("message") is not None
+                            else ""
+                        ),
                     }
                 }
                 for item in chat_history
             ]
             prompts = prompts + json.dumps(history)
 
         extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
@@ -104,18 +104,20 @@
             "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "llm",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "url.full": APIS["CHAT_CREATE"]["URL"],
             "llm.api": APIS["CHAT_CREATE"]["ENDPOINT"],
-            "llm.model": kwargs.get("model") if kwargs.get("model") is not None else "command-r",
+            "llm.model": (
+                kwargs.get("model") if kwargs.get("model") is not None else "command-r"
+            ),
             "llm.stream": False,
             "llm.prompts": prompts,
-            **(extra_attributes if extra_attributes is not None else {})
+            **(extra_attributes if extra_attributes is not None else {}),
         }
 
         attributes = LLMSpanAttributes(**span_attributes)
 
         if kwargs.get("temperature") is not None:
             attributes.llm_temperature = kwargs.get("temperature")
         if kwargs.get("max_tokens") is not None:
@@ -142,120 +144,145 @@
         if kwargs.get("tools") is not None:
             # stringify the list of objects
             attributes.llm_tools = json.dumps(kwargs.get("tools"))
         if kwargs.get("tool_results") is not None:
             # stringify the list of objects
             attributes.llm_tool_results = json.dumps(kwargs.get("tool_results"))
 
-        span = tracer.start_span(
-            APIS["CHAT_CREATE"]["METHOD"], kind=SpanKind.CLIENT
-        )
+        span = tracer.start_span(APIS["CHAT_CREATE"]["METHOD"], kind=SpanKind.CLIENT)
 
         # Set the attributes on the span
         for field, value in attributes.model_dump(by_alias=True).items():
             if value is not None:
                 span.set_attribute(field, value)
         try:
             # Attempt to call the original method
             result = wrapped(*args, **kwargs)
 
             # Set the response attributes
-            if (hasattr(result, "generation_id")) and (result.generation_id is not None):
+            if (hasattr(result, "generation_id")) and (
+                result.generation_id is not None
+            ):
                 span.set_attribute("llm.generation_id", result.generation_id)
             if (hasattr(result, "response_id")) and (result.response_id is not None):
                 span.set_attribute("llm.response_id", result.response_id)
-            if (hasattr(result, "is_search_required")) and (result.is_search_required is not None):
+            if (hasattr(result, "is_search_required")) and (
+                result.is_search_required is not None
+            ):
                 span.set_attribute("llm.is_search_required", result.is_search_required)
 
             if kwargs.get("stream") is False or kwargs.get("stream") is None:
                 if hasattr(result, "text") and result.text is not None:
-                    if hasattr(result, "chat_history") and result.chat_history is not None:
+                    if (
+                        hasattr(result, "chat_history")
+                        and result.chat_history is not None
+                    ):
                         responses = [
                             {
                                 "message": {
                                     "role": (
-                                        item.role if hasattr(item, "role") and item.role is not None else "USER"
+                                        item.role
+                                        if hasattr(item, "role")
+                                        and item.role is not None
+                                        else "USER"
                                     ),
                                     "content": (
-                                        item.message if hasattr(item, "message") and item.message is not None else ""
-                                    )
+                                        item.message
+                                        if hasattr(item, "message")
+                                        and item.message is not None
+                                        else ""
+                                    ),
                                 }
                             }
                             for item in result.chat_history
                         ]
                         span.set_attribute("llm.responses", json.dumps(responses))
                     else:
-                        responses = [{
-                            "message": {
-                                "role": "CHATBOT",
-                                "content": result.text
-                            }
-                        }]
+                        responses = [
+                            {"message": {"role": "CHATBOT", "content": result.text}}
+                        ]
                         span.set_attribute("llm.responses", json.dumps(responses))
                 else:
                     responses = []
                     span.set_attribute("llm.responses", json.dumps(responses))
 
                 # Get the usage
                 if hasattr(result, "meta") and result.meta is not None:
-                    if hasattr(result.meta, "billed_units") and result.meta.billed_units is not None:
+                    if (
+                        hasattr(result.meta, "billed_units")
+                        and result.meta.billed_units is not None
+                    ):
                         usage = result.meta.billed_units
                         if usage is not None:
                             usage_dict = {
-                                "input_tokens": usage.input_tokens if usage.input_tokens is not None else 0,
-                                "output_tokens": usage.output_tokens if usage.output_tokens is not None else 0,
-                                "total_tokens": usage.input_tokens + usage.output_tokens if usage.input_tokens is not None and usage.output_tokens is not None else 0,
+                                "input_tokens": (
+                                    usage.input_tokens
+                                    if usage.input_tokens is not None
+                                    else 0
+                                ),
+                                "output_tokens": (
+                                    usage.output_tokens
+                                    if usage.output_tokens is not None
+                                    else 0
+                                ),
+                                "total_tokens": (
+                                    usage.input_tokens + usage.output_tokens
+                                    if usage.input_tokens is not None
+                                    and usage.output_tokens is not None
+                                    else 0
+                                ),
                             }
-                            span.set_attribute("llm.token.counts", json.dumps(usage_dict))
+                            span.set_attribute(
+                                "llm.token.counts", json.dumps(usage_dict)
+                            )
                 span.set_status(StatusCode.OK)
                 span.end()
                 return result
             else:
                 # For older version, stream was passed as a parameter
                 return result
 
         except Exception as error:
             span.record_exception(error)
             span.set_status(Status(StatusCode.ERROR, str(error)))
             span.end()
             raise
+
     return traced_method
 
 
 def chat_stream(original_method, version, tracer):
     """Wrap the `messages_stream` method."""
 
     def traced_method(wrapped, instance, args, kwargs):
         service_provider = SERVICE_PROVIDERS["COHERE"]
 
         message = kwargs.get("message", "")
         prompt_tokens = estimate_tokens(message)
-        prompts = json.dumps([
-            {
-                "role": "USER",
-                "content": message
-            }
-        ])
+        prompts = json.dumps([{"role": "USER", "content": message}])
         preamble = kwargs.get("preamble")
         if preamble:
             prompts = json.dumps(
-                [{"role": "system", "content": preamble}] + [{"role": "USER", "content": message}]
+                [{"role": "system", "content": preamble}]
+                + [{"role": "USER", "content": message}]
             )
 
         chat_history = kwargs.get("chat_history")
         if chat_history:
             history = [
                 {
                     "message": {
                         "role": (
                             item.get("role") if item.get("role") is not None else "USER"
                         ),
                         "content": (
-                            item.get("message") if item.get("message") is not None else ""
-                        )
+                            item.get("message")
+                            if item.get("message") is not None
+                            else ""
+                        ),
                     }
                 }
                 for item in chat_history
             ]
             prompts = prompts + json.dumps(history)
 
         extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
@@ -264,18 +291,20 @@
             "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "llm",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "url.full": APIS["CHAT_STREAM"]["URL"],
             "llm.api": APIS["CHAT_STREAM"]["ENDPOINT"],
-            "llm.model": kwargs.get("model") if kwargs.get("model") is not None else "command-r",
-            "llm.stream": False,
+            "llm.model": (
+                kwargs.get("model") if kwargs.get("model") is not None else "command-r"
+            ),
+            "llm.stream": True,
             "llm.prompts": prompts,
-            **(extra_attributes if extra_attributes is not None else {})
+            **(extra_attributes if extra_attributes is not None else {}),
         }
 
         attributes = LLMSpanAttributes(**span_attributes)
 
         if kwargs.get("temperature") is not None:
             attributes.llm_temperature = kwargs.get("temperature")
         if kwargs.get("max_tokens") is not None:
@@ -302,17 +331,15 @@
         if kwargs.get("tools") is not None:
             # stringify the list of objects
             attributes.llm_tools = json.dumps(kwargs.get("tools"))
         if kwargs.get("tool_results") is not None:
             # stringify the list of objects
             attributes.llm_tool_results = json.dumps(kwargs.get("tool_results"))
 
-        span = tracer.start_span(
-            APIS["CHAT_CREATE"]["METHOD"], kind=SpanKind.CLIENT
-        )
+        span = tracer.start_span(APIS["CHAT_CREATE"]["METHOD"], kind=SpanKind.CLIENT)
         for field, value in attributes.model_dump(by_alias=True).items():
             if value is not None:
                 span.set_attribute(field, value)
         try:
             # Attempt to call the original method
             result = wrapped(*args, **kwargs)
```

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain/patch.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/langchain/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,22 @@
 import inspect
 from typing import Collection
 
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
-from langtrace_python_sdk.instrumentation.llamaindex.patch import generic_patch
+from langtrace_python_sdk.instrumentation.llamaindex.patch import (
+    generic_patch,
+    async_generic_patch,
+)
+
+import logging
+
+logging.basicConfig(level=logging.FATAL)
 
 import logging
 
 logging.basicConfig(level=logging.FATAL)
 
 
 class LlamaindexInstrumentation(BaseInstrumentor):
@@ -58,12 +65,23 @@
                                 f"llamaindex.{name}.{method_name}",
                                 task,
                                 tracer,
                                 version,
                             ),
                         )
 
+                        wrap_function_wrapper(
+                            module_name,
+                            ".".join([name, method_name]),
+                            async_generic_patch(
+                                f"llamaindex.{name}.{method_name}",
+                                task,
+                                tracer,
+                                version,
+                            ),
+                        )
+
     def _instrument_module(self, module_name):
         pass
 
     def _uninstrument(self, **kwargs):
         pass
```

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 from langtrace.trace_attributes import FrameworkSpanAttributes
 from opentelemetry import baggage
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
 
 from langtrace_python_sdk.constants.instrumentation.common import (
-    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY, SERVICE_PROVIDERS)
+    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
+    SERVICE_PROVIDERS,
+)
 
 
 def generic_patch(method, task, tracer, version):
     """
     A generic patch method that wraps a function with a span"""
 
     def traced_method(wrapped, instance, args, kwargs):
@@ -22,15 +24,15 @@
         span_attributes = {
             "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "framework",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "llamaindex.task.name": task,
-            **(extra_attributes if extra_attributes is not None else {})
+            **(extra_attributes if extra_attributes is not None else {}),
         }
 
         attributes = FrameworkSpanAttributes(**span_attributes)
 
         with tracer.start_as_current_span(method, kind=SpanKind.CLIENT) as span:
             for field, value in attributes.model_dump(by_alias=True).items():
                 if value is not None:
@@ -41,13 +43,55 @@
                 span.set_status(StatusCode.OK)
                 return result
             except Exception as e:
                 # Record the exception in the span
                 span.record_exception(e)
 
                 # Set the span status to indicate an error
+                span.set_status(Status(StatusCode.ERROR, str(e)))
+
+                # Reraise the exception to ensure it's not swallowed
+                raise
+
+    return traced_method
+
+
+def async_generic_patch(method, task, tracer, version):
+    """
+    A generic patch method that wraps a function with a span"""
+
+    async def traced_method(wrapped, instance, args, kwargs):
+        service_provider = SERVICE_PROVIDERS["LLAMAINDEX"]
+        extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
+
+        span_attributes = {
+            "langtrace.sdk.name": "langtrace-python-sdk",
+            "langtrace.service.name": service_provider,
+            "langtrace.service.type": "framework",
+            "langtrace.service.version": version,
+            "langtrace.version": "1.0.0",
+            "llamaindex.task.name": task,
+            **(extra_attributes if extra_attributes is not None else {}),
+        }
+
+        attributes = FrameworkSpanAttributes(**span_attributes)
+
+        with tracer.start_as_current_span(method, kind=SpanKind.CLIENT) as span:
+            async for field, value in attributes.model_dump(by_alias=True).items():
+                if value is not None:
+                    span.set_attribute(field, value)
+            try:
+                # Attempt to call the original method
+                result = await wrapped(*args, **kwargs)
+                span.set_status(StatusCode.OK)
+                return result
+            except Exception as e:
+                # Record the exception in the span
+                span.record_exception(e)
+
+                # Set the span status to indicate an error
                 span.set_status(Status(StatusCode.ERROR, str(e)))
 
                 # Reraise the exception to ensure it's not swallowed
                 raise
 
     return traced_method
```

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 from typing import Collection
 
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
 from langtrace_python_sdk.instrumentation.openai.patch import (
+    async_embeddings_create,
+    async_images_generate,
     chat_completions_create,
     embeddings_create,
     images_generate,
+    async_chat_completions_create,
 )
 
 import logging
 
 logging.basicConfig(level=logging.FATAL)
 
 
@@ -21,25 +24,47 @@
     def instrumentation_dependencies(self) -> Collection[str]:
         return ["openai >= 0.27.0"]
 
     def _instrument(self, **kwargs):
         tracer_provider = kwargs.get("tracer_provider")
         tracer = get_tracer(__name__, "", tracer_provider)
         version = importlib.metadata.version("openai")
+
         wrap_function_wrapper(
             "openai.resources.chat.completions",
             "Completions.create",
             chat_completions_create("openai.chat.completions.create", version, tracer),
         )
+
+        wrap_function_wrapper(
+            "openai.resources.chat.completions",
+            "AsyncCompletions.create",
+            async_chat_completions_create(
+                "openai.chat.completions.create_stream", version, tracer
+            ),
+        )
+
         wrap_function_wrapper(
             "openai.resources.images",
             "Images.generate",
             images_generate("openai.images.generate", version, tracer),
         )
+
+        wrap_function_wrapper(
+            "openai.resources.images",
+            "AsyncImages.generate",
+            async_images_generate("openai.images.generate", version, tracer),
+        )
         wrap_function_wrapper(
             "openai.resources.embeddings",
             "Embeddings.create",
             embeddings_create("openai.embeddings.create", version, tracer),
         )
 
+        wrap_function_wrapper(
+            "openai.resources.embeddings",
+            "AsyncEmbeddings.create",
+            async_embeddings_create("openai.embeddings.create", version, tracer),
+        )
+
     def _uninstrument(self, **kwargs):
         pass
```

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/openai/patch.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/openai/patch.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 
 from langtrace.trace_attributes import Event, LLMSpanAttributes
 from opentelemetry import baggage, trace
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
 
 from langtrace_python_sdk.constants.instrumentation.common import (
-    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY, SERVICE_PROVIDERS)
+    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
+    SERVICE_PROVIDERS,
+)
 from langtrace_python_sdk.constants.instrumentation.openai import APIS
-from langtrace_python_sdk.utils.llm import (calculate_prompt_tokens,
-                                            estimate_tokens)
+from langtrace_python_sdk.utils.llm import calculate_prompt_tokens, estimate_tokens
 
 
 def images_generate(original_method, version, tracer):
     """
     Wrap the `generate` method of the `Images` class to trace it.
     """
 
@@ -36,15 +37,15 @@
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "url.full": base_url,
             "llm.api": APIS["IMAGES_GENERATION"]["ENDPOINT"],
             "llm.model": kwargs.get("model"),
             "llm.stream": kwargs.get("stream"),
             "llm.prompts": json.dumps([kwargs.get("prompt", [])]),
-            **(extra_attributes if extra_attributes is not None else {})
+            **(extra_attributes if extra_attributes is not None else {}),
         }
 
         attributes = LLMSpanAttributes(**span_attributes)
 
         with tracer.start_as_current_span(
             APIS["IMAGES_GENERATION"]["METHOD"], kind=SpanKind.CLIENT
         ) as span:
@@ -83,14 +84,86 @@
 
                 # Reraise the exception to ensure it's not swallowed
                 raise
 
     return traced_method
 
 
+def async_images_generate(original_method, version, tracer):
+    """
+    Wrap the `generate` method of the `Images` class to trace it.
+    """
+
+    async def traced_method(wrapped, instance, args, kwargs):
+        base_url = (
+            str(instance._client._base_url)
+            if hasattr(instance, "_client") and hasattr(instance._client, "_base_url")
+            else ""
+        )
+        service_provider = SERVICE_PROVIDERS["OPENAI"]
+        extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
+
+        span_attributes = {
+            "langtrace.sdk.name": "langtrace-python-sdk",
+            "langtrace.service.name": service_provider,
+            "langtrace.service.type": "llm",
+            "langtrace.service.version": version,
+            "langtrace.version": "1.0.0",
+            "url.full": base_url,
+            "llm.api": APIS["IMAGES_GENERATION"]["ENDPOINT"],
+            "llm.model": kwargs.get("model"),
+            "llm.stream": kwargs.get("stream"),
+            "llm.prompts": json.dumps([kwargs.get("prompt", [])]),
+            **(extra_attributes if extra_attributes is not None else {}),
+        }
+
+        attributes = LLMSpanAttributes(**span_attributes)
+
+        with tracer.start_as_current_span(
+            APIS["IMAGES_GENERATION"]["METHOD"], kind=SpanKind.CLIENT
+        ) as span:
+            async for field, value in attributes.model_dump(by_alias=True).items():
+                if value is not None:
+                    span.set_attribute(field, value)
+            try:
+                # Attempt to call the original method
+                result = await wrapped(*args, **kwargs)
+                if kwargs.get("stream") is False or kwargs.get("stream") is None:
+                    data = (
+                        result.data[0]
+                        if hasattr(result, "data") and len(result.data) > 0
+                        else {}
+                    )
+                    response = [
+                        {
+                            "url": data.url if hasattr(data, "url") else "",
+                            "revised_prompt": (
+                                data.revised_prompt
+                                if hasattr(data, "revised_prompt")
+                                else ""
+                            ),
+                        }
+                    ]
+                    span.set_attribute("llm.responses", json.dumps(response))
+
+                span.set_status(StatusCode.OK)
+                return result
+            except Exception as e:
+                # Record the exception in the span
+                span.record_exception(e)
+
+                # Set the span status to indicate an error
+                span.set_status(Status(StatusCode.ERROR, str(e)))
+
+                # Reraise the exception to ensure it's not swallowed
+                raise
+
+    return traced_method
+
+
 def chat_completions_create(original_method, version, tracer):
     """Wrap the `create` method of the `ChatCompletion` class to trace it."""
 
     def traced_method(wrapped, instance, args, kwargs):
         base_url = (
             str(instance._client._base_url)
             if hasattr(instance, "_client") and hasattr(instance._client, "_base_url")
@@ -101,25 +174,52 @@
         if "perplexity" in base_url:
             service_provider = SERVICE_PROVIDERS["PPLX"]
         elif "azure" in base_url:
             service_provider = SERVICE_PROVIDERS["AZURE"]
 
         extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
 
+        # handle tool calls in the kwargs
+        llm_prompts = []
+        for item in kwargs.get("messages", []):
+            if "tool_calls" in item:
+                tool_calls = []
+                for tool_call in item["tool_calls"]:
+                    tool_call_dict = {
+                        "id": tool_call.id if hasattr(tool_call, "id") else "",
+                        "type": tool_call.type if hasattr(tool_call, "type") else "",
+                    }
+                    if hasattr(tool_call, "function"):
+                        tool_call_dict["function"] = {
+                            "name": (
+                                tool_call.function.name
+                                if hasattr(tool_call.function, "name")
+                                else ""
+                            ),
+                            "arguments": (
+                                tool_call.function.arguments
+                                if hasattr(tool_call.function, "arguments")
+                                else ""
+                            ),
+                        }
+                    tool_calls.append(tool_call_dict)
+                item["tool_calls"] = tool_calls
+            llm_prompts.append(item)
+
         span_attributes = {
             "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "llm",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "url.full": base_url,
             "llm.api": APIS["CHAT_COMPLETION"]["ENDPOINT"],
             "llm.prompts": json.dumps(kwargs.get("messages", [])),
             "llm.stream": kwargs.get("stream"),
-            **(extra_attributes if extra_attributes is not None else {})
+            **(extra_attributes if extra_attributes is not None else {}),
         }
 
         attributes = LLMSpanAttributes(**span_attributes)
 
         if kwargs.get("temperature") is not None:
             attributes.llm_temperature = kwargs.get("temperature")
         if kwargs.get("top_p") is not None:
@@ -268,15 +368,233 @@
                     content = []
                 span.add_event(
                     Event.STREAM_OUTPUT.value, {"response": "".join(content)}
                 )
                 result_content.append(content[0] if len(content) > 0 else "")
                 yield chunk
         finally:
+            # Finalize span after processing all chunks
+            span.add_event(Event.STREAM_END.value)
+            span.set_attribute(
+                "llm.token.counts",
+                json.dumps(
+                    {
+                        "input_tokens": prompt_tokens,
+                        "output_tokens": completion_tokens,
+                        "total_tokens": prompt_tokens + completion_tokens,
+                    }
+                ),
+            )
+            span.set_attribute(
+                "llm.responses",
+                json.dumps(
+                    [
+                        {
+                            "message": {
+                                "role": "assistant",
+                                "content": "".join(result_content),
+                            }
+                        }
+                    ]
+                ),
+            )
+            span.set_status(StatusCode.OK)
+            span.end()
 
+    # return the wrapped method
+    return traced_method
+
+
+def async_chat_completions_create(original_method, version, tracer):
+    """Wrap the `create` method of the `ChatCompletion` class to trace it."""
+
+    async def traced_method(wrapped, instance, args, kwargs):
+        base_url = (
+            str(instance._client._base_url)
+            if hasattr(instance, "_client") and hasattr(instance._client, "_base_url")
+            else ""
+        )
+        service_provider = SERVICE_PROVIDERS["OPENAI"]
+        # If base url contains perplexity or azure, set the service provider accordingly
+        if "perplexity" in base_url:
+            service_provider = SERVICE_PROVIDERS["PPLX"]
+        elif "azure" in base_url:
+            service_provider = SERVICE_PROVIDERS["AZURE"]
+
+        extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
+
+        span_attributes = {
+            "langtrace.sdk.name": "langtrace-python-sdk",
+            "langtrace.service.name": service_provider,
+            "langtrace.service.type": "llm",
+            "langtrace.service.version": version,
+            "langtrace.version": "1.0.0",
+            "url.full": base_url,
+            "llm.api": APIS["CHAT_COMPLETION"]["ENDPOINT"],
+            "llm.prompts": json.dumps(kwargs.get("messages", [])),
+            "llm.stream": kwargs.get("stream"),
+            **(extra_attributes if extra_attributes is not None else {}),
+        }
+
+        attributes = LLMSpanAttributes(**span_attributes)
+
+        if kwargs.get("temperature") is not None:
+            attributes.llm_temperature = kwargs.get("temperature")
+        if kwargs.get("top_p") is not None:
+            attributes.llm_top_p = kwargs.get("top_p")
+        if kwargs.get("user") is not None:
+            attributes.llm_user = kwargs.get("user")
+        if kwargs.get("functions") is not None:
+            attributes.llm_function_prompts = json.dumps(kwargs.get("functions"))
+
+        # TODO(Karthik): Gotta figure out how to handle streaming with context
+        # with tracer.start_as_current_span(APIS["CHAT_COMPLETION"]["METHOD"],
+        #                                   kind=SpanKind.CLIENT) as span:
+        span = tracer.start_span(
+            APIS["CHAT_COMPLETION"]["METHOD"], kind=SpanKind.CLIENT
+        )
+        for field, value in attributes.model_dump(by_alias=True).items():
+            if value is not None:
+                span.set_attribute(field, value)
+        try:
+            # Attempt to call the original method
+            result = await wrapped(*args, **kwargs)
+            if kwargs.get("stream") is False or kwargs.get("stream") is None:
+                span.set_attribute("llm.model", result.model)
+                if hasattr(result, "choices") and result.choices is not None:
+                    responses = [
+                        {
+                            "message": {
+                                "role": (
+                                    choice.message.role
+                                    if choice.message and choice.message.role
+                                    else "assistant"
+                                ),
+                                "content": (
+                                    choice.message.content
+                                    if choice.message and choice.message.content
+                                    else (
+                                        choice.message.function_call.arguments
+                                        if choice.message
+                                        and choice.message.function_call.arguments
+                                        else ""
+                                    )
+                                ),
+                                **(
+                                    {
+                                        "content_filter_results": choice[
+                                            "content_filter_results"
+                                        ]
+                                    }
+                                    if "content_filter_results" in choice
+                                    else {}
+                                ),
+                            }
+                        }
+                        for choice in result.choices
+                    ]
+                    span.set_attribute("llm.responses", json.dumps(responses))
+                else:
+                    responses = []
+                    span.set_attribute("llm.responses", json.dumps(responses))
+                if (
+                    hasattr(result, "system_fingerprint")
+                    and result.system_fingerprint is not None
+                ):
+                    span.set_attribute(
+                        "llm.system.fingerprint", result.system_fingerprint
+                    )
+                # Get the usage
+                if hasattr(result, "usage") and result.usage is not None:
+                    usage = result.usage
+                    if usage is not None:
+                        usage_dict = {
+                            "input_tokens": result.usage.prompt_tokens,
+                            "output_tokens": usage.completion_tokens,
+                            "total_tokens": usage.total_tokens,
+                        }
+                        span.set_attribute("llm.token.counts", json.dumps(usage_dict))
+                span.set_status(StatusCode.OK)
+                span.end()
+                return result
+            else:
+                # iterate over kwargs.get("messages", {}) and calculate the prompt tokens
+                prompt_tokens = 0
+                for message in kwargs.get("messages", {}):
+                    prompt_tokens += calculate_prompt_tokens(
+                        json.dumps(message), kwargs.get("model")
+                    )
+
+                # iterate over kwargs.get("functions") and calculate the prompt tokens
+                if kwargs.get("functions") is not None:
+                    for function in kwargs.get("functions"):
+                        prompt_tokens += calculate_prompt_tokens(
+                            json.dumps(function), kwargs.get("model")
+                        )
+
+                return ahandle_streaming_response(
+                    result,
+                    span,
+                    prompt_tokens,
+                    function_call=kwargs.get("functions") is not None,
+                )
+
+        except Exception as error:
+            span.record_exception(error)
+            span.set_status(Status(StatusCode.ERROR, str(error)))
+            span.end()
+            raise
+
+    async def ahandle_streaming_response(
+        result, span, prompt_tokens, function_call=False
+    ):
+        """Process and yield streaming response chunks."""
+        result_content = []
+        span.add_event(Event.STREAM_START.value)
+        completion_tokens = 0
+        try:
+            async for chunk in result:
+                if hasattr(chunk, "model") and chunk.model is not None:
+                    span.set_attribute("llm.model", chunk.model)
+                if hasattr(chunk, "choices") and chunk.choices is not None:
+                    token_counts = [
+                        (
+                            estimate_tokens(choice.delta.content)
+                            if choice.delta and choice.delta.content
+                            else (
+                                estimate_tokens(choice.delta.function_call.arguments)
+                                if choice.delta.function_call
+                                and choice.delta.function_call.arguments
+                                else 0
+                            )
+                        )
+                        for choice in chunk.choices
+                    ]
+                    completion_tokens += sum(token_counts)
+                    content = [
+                        (
+                            choice.delta.content
+                            if choice.delta and choice.delta.content
+                            else (
+                                choice.delta.function_call.arguments
+                                if choice.delta.function_call
+                                and choice.delta.function_call.arguments
+                                else ""
+                            )
+                        )
+                        for choice in chunk.choices
+                    ]
+                else:
+                    content = []
+                span.add_event(
+                    Event.STREAM_OUTPUT.value, {"response": "".join(content)}
+                )
+                result_content.append(content[0] if len(content) > 0 else "")
+                yield chunk
+        finally:
             # Finalize span after processing all chunks
             span.add_event(Event.STREAM_END.value)
             span.set_attribute(
                 "llm.token.counts",
                 json.dumps(
                     {
                         "input_tokens": prompt_tokens,
@@ -326,15 +644,15 @@
             "langtrace.service.type": "llm",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "url.full": base_url,
             "llm.api": APIS["EMBEDDINGS_CREATE"]["ENDPOINT"],
             "llm.model": kwargs.get("model"),
             "llm.prompts": "",
-            **(extra_attributes if extra_attributes is not None else {})
+            **(extra_attributes if extra_attributes is not None else {}),
         }
 
         attributes = LLMSpanAttributes(**span_attributes)
         kwargs.get("encoding_format")
 
         if kwargs.get("encoding_format") is not None:
             attributes.llm_encoding_format = kwargs.get("encoding_format")
@@ -356,13 +674,76 @@
                 span.set_status(StatusCode.OK)
                 return result
             except Exception as e:
                 # Record the exception in the span
                 span.record_exception(e)
 
                 # Set the span status to indicate an error
+                span.set_status(Status(StatusCode.ERROR, str(e)))
+
+                # Reraise the exception to ensure it's not swallowed
+                raise
+
+    return traced_method
+
+
+def async_embeddings_create(original_method, version, tracer):
+    """
+    Wrap the `create` method of the `Embeddings` class to trace it.
+    """
+
+    async def traced_method(wrapped, instance, args, kwargs):
+        base_url = (
+            str(instance._client._base_url)
+            if hasattr(instance, "_client") and hasattr(instance._client, "_base_url")
+            else ""
+        )
+
+        service_provider = SERVICE_PROVIDERS["OPENAI"]
+        extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
+
+        span_attributes = {
+            "langtrace.sdk.name": "langtrace-python-sdk",
+            "langtrace.service.name": service_provider,
+            "langtrace.service.type": "llm",
+            "langtrace.service.version": version,
+            "langtrace.version": "1.0.0",
+            "url.full": base_url,
+            "llm.api": APIS["EMBEDDINGS_CREATE"]["ENDPOINT"],
+            "llm.model": kwargs.get("model"),
+            "llm.prompts": "",
+            **(extra_attributes if extra_attributes is not None else {}),
+        }
+
+        attributes = LLMSpanAttributes(**span_attributes)
+        kwargs.get("encoding_format")
+
+        if kwargs.get("encoding_format") is not None:
+            attributes.llm_encoding_format = kwargs.get("encoding_format")
+        if kwargs.get("dimensions") is not None:
+            attributes["llm.dimensions"] = kwargs.get("dimensions")
+        if kwargs.get("user") is not None:
+            attributes["llm.user"] = kwargs.get("user")
+
+        with tracer.start_as_current_span(
+            APIS["EMBEDDINGS_CREATE"]["METHOD"], kind=SpanKind.CLIENT
+        ) as span:
+
+            async for field, value in attributes.model_dump(by_alias=True).items():
+                if value is not None:
+                    span.set_attribute(field, value)
+            try:
+                # Attempt to call the original method
+                result = await wrapped(*args, **kwargs)
+                span.set_status(StatusCode.OK)
+                return result
+            except Exception as e:
+                # Record the exception in the span
+                span.record_exception(e)
+
+                # Set the span status to indicate an error
                 span.set_status(Status(StatusCode.ERROR, str(e)))
 
                 # Reraise the exception to ensure it's not swallowed
                 raise
 
     return traced_method
```

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/instrumentation/pinecone/patch.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/instrumentation/pinecone/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/utils/llm.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/utils/llm.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/langtrace_python_sdk/utils/with_root_span.py` & `langtrace_python_sdk-1.3.2/src/langtrace_python_sdk/utils/with_root_span.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/tests/utils.py` & `langtrace_python_sdk-1.3.2/src/tests/utils.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/tests/anthropic/test_anthropic.py` & `langtrace_python_sdk-1.3.2/src/tests/anthropic/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/tests/chroma/test_chroma.py` & `langtrace_python_sdk-1.3.2/src/tests/chroma/test_chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/tests/langchain/test_langchain.py` & `langtrace_python_sdk-1.3.2/src/tests/langchain/test_langchain.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/tests/langchain/test_langchain_community.py` & `langtrace_python_sdk-1.3.2/src/tests/langchain/test_langchain_community.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/tests/langchain/test_langchain_core.py` & `langtrace_python_sdk-1.3.2/src/tests/langchain/test_langchain_core.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/tests/openai/test_chat_completion.py` & `langtrace_python_sdk-1.3.2/src/tests/openai/test_chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/tests/openai/test_image_generation.py` & `langtrace_python_sdk-1.3.2/src/tests/openai/test_image_generation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/src/tests/pinecone/test_pinecone.py` & `langtrace_python_sdk-1.3.2/src/tests/pinecone/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/.gitignore` & `langtrace_python_sdk-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/LICENSE` & `langtrace_python_sdk-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.3.1/README.md` & `langtrace_python_sdk-1.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
 ``` python
 pip install langtrace-python-sdk
 ```
 
 ``` python
 from langtrace_python_sdk import langtrace # Must precede any llm module imports
-langtrace.init(write_to_langtrace_cloud=False, batch=False)
+langtrace.init(write_to_langtrace_cloud=False)
 ```
 
 ## Langtrace self hosted custom exporter
 
 Get started by adding simply three lines to your code and see traces being exported to your remote location!
 
 ``` python
```

### Comparing `langtrace_python_sdk-1.3.1/pyproject.toml` & `langtrace_python_sdk-1.3.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,16 @@
     "openai",
     "anthropic",
     "python-dotenv",
     "langchain",
     "langchain-openai",
     "llama-index",
     "langchain-openai",
-    "chromadb"
+    "chromadb",
+    "cohere"
 ]
 
 
 
 [project.urls]
 Homepage = "https://github.com/Scale3-Labs/langtrace-python-sdk"
```

### Comparing `langtrace_python_sdk-1.3.1/PKG-INFO` & `langtrace_python_sdk-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: langtrace-python-sdk
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python SDK for LangTrace
 Project-URL: Homepage, https://github.com/Scale3-Labs/langtrace-python-sdk
 Author-email: Scale3 Labs <engineering@scale3labs.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -15,14 +15,15 @@
 Requires-Dist: opentelemetry-sdk
 Requires-Dist: pinecone-client
 Requires-Dist: tiktoken
 Requires-Dist: trace-attributes
 Provides-Extra: dev
 Requires-Dist: anthropic; extra == 'dev'
 Requires-Dist: chromadb; extra == 'dev'
+Requires-Dist: cohere; extra == 'dev'
 Requires-Dist: langchain; extra == 'dev'
 Requires-Dist: langchain-openai; extra == 'dev'
 Requires-Dist: llama-index; extra == 'dev'
 Requires-Dist: openai; extra == 'dev'
 Requires-Dist: python-dotenv; extra == 'dev'
 Description-Content-Type: text/markdown
 
@@ -140,15 +141,15 @@
 
 ``` python
 pip install langtrace-python-sdk
 ```
 
 ``` python
 from langtrace_python_sdk import langtrace # Must precede any llm module imports
-langtrace.init(write_to_langtrace_cloud=False, batch=False)
+langtrace.init(write_to_langtrace_cloud=False)
 ```
 
 ## Langtrace self hosted custom exporter
 
 Get started by adding simply three lines to your code and see traces being exported to your remote location!
 
 ``` python
```

