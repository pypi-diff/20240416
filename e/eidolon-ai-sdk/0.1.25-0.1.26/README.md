# Comparing `tmp/eidolon_ai_sdk-0.1.25.tar.gz` & `tmp/eidolon_ai_sdk-0.1.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eidolon_ai_sdk-0.1.25.tar", max compression
+gzip compressed data, was "eidolon_ai_sdk-0.1.26.tar", max compression
```

## Comparing `eidolon_ai_sdk-0.1.25.tar` & `eidolon_ai_sdk-0.1.26.tar`

### file list

```diff
@@ -1,136 +1,143 @@
--rw-r--r--   0        0        0     2569 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/README.md
--rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/__init__.py
--rw-r--r--   0        0        0     2415 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/agent.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/__init__.py
--rw-r--r--   0        0        0     4645 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/document_manager.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
--rw-r--r--   0        0        0      971 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
--rw-r--r--   0        0        0     3405 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
--rw-r--r--   0        0        0     4173 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
--rw-r--r--   0        0        0     2805 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
--rw-r--r--   0        0        0     4510 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
--rw-r--r--   0        0        0      448 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
--rw-r--r--   0        0        0     3699 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
--rw-r--r--   0        0        0     2053 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
--rw-r--r--   0        0        0     3212 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
--rw-r--r--   0        0        0     1647 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
--rw-r--r--   0        0        0     1328 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
--rw-r--r--   0        0        0     3356 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
--rw-r--r--   0        0        0     1400 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
--rw-r--r--   0        0        0     1398 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
--rw-r--r--   0        0        0     4786 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
--rw-r--r--   0        0        0    43465 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
--rw-r--r--   0        0        0     5516 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/generic_agent.py
--rw-r--r--   0        0        0     1998 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/openai_whisper_agent.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/__init__.py
--rw-r--r--   0        0        0     2078 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
--rw-r--r--   0        0        0     1444 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
--rw-r--r--   0        0        0     2339 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
--rw-r--r--   0        0        0      559 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
--rw-r--r--   0        0        0     2939 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/retriever.py
--rw-r--r--   0        0        0     3640 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
--rw-r--r--   0        0        0    11421 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/simple_agent.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/__init__.py
--rw-r--r--   0        0        0     1825 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/checker.py
--rw-r--r--   0        0        0     2468 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/controller.py
--rw-r--r--   0        0        0     1503 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/memory.py
--rw-r--r--   0        0        0     1423 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/prompts.py
--rw-r--r--   0        0        0      364 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/thought.py
--rw-r--r--   0        0        0     4951 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
--rw-r--r--   0        0        0     7614 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
--rw-r--r--   0        0        0     4446 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent_os.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/bin/__init__.py
--rwxr-xr-x   0        0        0     9444 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/bin/agent_creator.py
--rw-r--r--   0        0        0     7578 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/bin/agent_http_server.py
--rwxr-xr-x   0        0        0     3789 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/bin/replay.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/__init__.py
--rw-r--r--   0        0        0     8297 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/code_builtins.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/components/__init__.py
--rw-r--r--   0        0        0     2223 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/components/opentelemetry.py
--rw-r--r--   0        0        0     4256 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/components/usage.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/logic_units/__init__.py
--rw-r--r--   0        0        0     5662 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/logic_units/web_search.py
--rw-r--r--   0        0        0      239 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
--rw-r--r--   0        0        0      236 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
--rw-r--r--   0        0        0      242 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
--rw-r--r--   0        0        0      181 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/resources/machine.yaml
--rw-r--r--   0        0        0      231 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
--rw-r--r--   0        0        0      257 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
--rw-r--r--   0        0        0      231 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
--rw-r--r--   0        0        0      235 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/resources/openai_35.yaml
--rw-r--r--   0        0        0      234 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/resources/openai_4.yaml
--rw-r--r--   0        0        0        0 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/__init__.py
--rw-r--r--   0        0        0     1843 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/agent_call_history.py
--rw-r--r--   0        0        0     4293 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/agent_cpu.py
--rw-r--r--   0        0        0     2956 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/agent_io.py
--rw-r--r--   0        0        0     7916 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/agents_logic_unit.py
--rw-r--r--   0        0        0      292 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/call_context.py
--rw-r--r--   0        0        0     2833 2024-04-12 15:34:22.087282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/conversation_memory_unit.py
--rw-r--r--   0        0        0     8231 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/conversational_agent_cpu.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/llm/__init__.py
--rw-r--r--   0        0        0    10036 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
--rw-r--r--   0        0        0    12148 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
--rw-r--r--   0        0        0    12773 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
--rw-r--r--   0        0        0     3119 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
--rw-r--r--   0        0        0     1679 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/llm_message.py
--rw-r--r--   0        0        0     1910 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/llm_unit.py
--rw-r--r--   0        0        0     4199 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/logic_unit.py
--rw-r--r--   0        0        0     3541 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/memory_unit.py
--rw-r--r--   0        0        0      825 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/processing_unit.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/io/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/__init__.py
--rw-r--r--   0        0        0     1157 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/agent_memory.py
--rw-r--r--   0        0        0     5309 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/chroma_vector_store.py
--rw-r--r--   0        0        0      641 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/document.py
--rw-r--r--   0        0        0     2620 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/embeddings.py
--rw-r--r--   0        0        0     2517 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/file_memory.py
--rw-r--r--   0        0        0     4220 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/file_system_vector_store.py
--rw-r--r--   0        0        0     3912 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/in_memory_file_memory.py
--rw-r--r--   0        0        0     5780 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/local_file_memory.py
--rw-r--r--   0        0        0     4837 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/local_symbolic_memory.py
--rw-r--r--   0        0        0     3762 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
--rw-r--r--   0        0        0      996 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/noop_memory.py
--rw-r--r--   0        0        0     1976 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/s3_file_memory.py
--rw-r--r--   0        0        0     5413 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/semantic_memory.py
--rw-r--r--   0        0        0      869 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/similarity_memory.py
--rw-r--r--   0        0        0     1516 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/vector_store.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/__init__.py
--rw-r--r--   0        0        0      771 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/authentication_processor.py
--rw-r--r--   0        0        0     2091 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/azure_authorizer.py
--rw-r--r--   0        0        0     1231 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/functional_authorizer.py
--rw-r--r--   0        0        0     2001 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/google_auth.py
--rw-r--r--   0        0        0     1867 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/jwt_processor.py
--rw-r--r--   0        0        0      484 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/okta_authorizor.py
--rw-r--r--   0        0        0     1076 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/permissions.py
--rw-r--r--   0        0        0     2462 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/process_authorizer.py
--rw-r--r--   0        0        0     1780 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/security_manager.py
--rw-r--r--   0        0        0     1052 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/security_middleware.py
--rw-r--r--   0        0        0      428 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/user.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/__init__.py
--rw-r--r--   0        0        0     1377 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/agent_contract.py
--rw-r--r--   0        0        0    20899 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/agent_controller.py
--rw-r--r--   0        0        0    13397 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/agent_machine.py
--rw-r--r--   0        0        0     1149 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/dynamic_middleware.py
--rw-r--r--   0        0        0     3432 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/fn_handler.py
--rw-r--r--   0        0        0     3911 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/process_file_system.py
--rw-r--r--   0        0        0     4275 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/processes.py
--rw-r--r--   0        0        0     6895 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/reference_model.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/resources/__init__.py
--rw-r--r--   0        0        0      314 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/resources/agent_resource.py
--rw-r--r--   0        0        0      414 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/resources/machine_resource.py
--rw-r--r--   0        0        0      684 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/resources/reference_resource.py
--rw-r--r--   0        0        0     1663 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/resources/resources_base.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/__init__.py
--rw-r--r--   0        0        0      509 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/async_wrapper.py
--rw-r--r--   0        0        0     2806 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/class_utils.py
--rw-r--r--   0        0        0     3812 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/replay.py
--rw-r--r--   0        0        0     6483 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/schema_to_model.py
--rw-r--r--   0        0        0      900 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/str_utils.py
--rw-r--r--   0        0        0     3445 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/stream_collector.py
--rw-r--r--   0        0        0      565 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/logging.conf
--rw-r--r--   0        0        0     2003 2024-04-12 15:34:22.091282 eidolon_ai_sdk-0.1.25/pyproject.toml
--rw-r--r--   0        0        0     4759 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.25/PKG-INFO
+-rw-r--r--   0        0        0     2569 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/__init__.py
+-rw-r--r--   0        0        0     2400 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/agent.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/__init__.py
+-rw-r--r--   0        0        0     3025 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/document_manager.py
+-rw-r--r--   0        0        0     2710 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/document_processor.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
+-rw-r--r--   0        0        0      971 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
+-rw-r--r--   0        0        0     3405 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
+-rw-r--r--   0        0        0     4173 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
+-rw-r--r--   0        0        0     2805 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
+-rw-r--r--   0        0        0     4519 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
+-rw-r--r--   0        0        0      448 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
+-rw-r--r--   0        0        0     3699 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
+-rw-r--r--   0        0        0     2053 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
+-rw-r--r--   0        0        0     3212 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
+-rw-r--r--   0        0        0     1647 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
+-rw-r--r--   0        0        0     1328 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
+-rw-r--r--   0        0        0     3356 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
+-rw-r--r--   0        0        0     1400 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
+-rw-r--r--   0        0        0     1398 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
+-rw-r--r--   0        0        0     4786 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
+-rw-r--r--   0        0        0    43465 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
+-rw-r--r--   0        0        0     4825 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/generic_agent.py
+-rw-r--r--   0        0        0     1924 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/openai_whisper_agent.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/__init__.py
+-rw-r--r--   0        0        0     2078 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
+-rw-r--r--   0        0        0     1434 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
+-rw-r--r--   0        0        0     2329 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
+-rw-r--r--   0        0        0      559 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
+-rw-r--r--   0        0        0     2904 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/retriever.py
+-rw-r--r--   0        0        0     3721 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
+-rw-r--r--   0        0        0    12896 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/simple_agent.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/__init__.py
+-rw-r--r--   0        0        0     1815 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/checker.py
+-rw-r--r--   0        0        0     2468 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/controller.py
+-rw-r--r--   0        0        0     1503 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/memory.py
+-rw-r--r--   0        0        0     1423 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/prompts.py
+-rw-r--r--   0        0        0      364 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/thought.py
+-rw-r--r--   0        0        0     4951 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
+-rw-r--r--   0        0        0     7614 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
+-rw-r--r--   0        0        0     4563 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent_os.py
+-rw-r--r--   0        0        0    12721 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent_os_interfaces.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/bin/__init__.py
+-rwxr-xr-x   0        0        0     9444 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/bin/agent_creator.py
+-rw-r--r--   0        0        0     7743 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/bin/agent_http_server.py
+-rwxr-xr-x   0        0        0     3789 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/bin/replay.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/__init__.py
+-rw-r--r--   0        0        0     8742 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/code_builtins.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/components/__init__.py
+-rw-r--r--   0        0        0     2223 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/components/opentelemetry.py
+-rw-r--r--   0        0        0     4256 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/components/usage.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/logic_units/__init__.py
+-rw-r--r--   0        0        0     5662 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/logic_units/web_search.py
+-rw-r--r--   0        0        0      234 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
+-rw-r--r--   0        0        0      231 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
+-rw-r--r--   0        0        0      237 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
+-rw-r--r--   0        0        0      181 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/resources/machine.yaml
+-rw-r--r--   0        0        0      226 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
+-rw-r--r--   0        0        0      252 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
+-rw-r--r--   0        0        0      226 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
+-rw-r--r--   0        0        0      225 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/resources/openai_35.yaml
+-rw-r--r--   0        0        0      229 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/resources/openai_4.yaml
+-rw-r--r--   0        0        0        0 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/__init__.py
+-rw-r--r--   0        0        0     1843 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/agent_call_history.py
+-rw-r--r--   0        0        0     4638 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/agent_cpu.py
+-rw-r--r--   0        0        0     2474 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/agent_io.py
+-rw-r--r--   0        0        0     7916 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/agents_logic_unit.py
+-rw-r--r--   0        0        0     1641 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/audio_unit.py
+-rw-r--r--   0        0        0      292 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/call_context.py
+-rw-r--r--   0        0        0     2833 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/conversation_memory_unit.py
+-rw-r--r--   0        0        0    14068 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/conversational_apu.py
+-rw-r--r--   0        0        0     1856 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/image_unit.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm/__init__.py
+-rw-r--r--   0        0        0    11215 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
+-rw-r--r--   0        0        0    13115 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
+-rw-r--r--   0        0        0     6166 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py
+-rw-r--r--   0        0        0     5631 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py
+-rw-r--r--   0        0        0    10361 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
+-rw-r--r--   0        0        0     3375 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
+-rw-r--r--   0        0        0     3930 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm_message.py
+-rw-r--r--   0        0        0     3443 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm_unit.py
+-rw-r--r--   0        0        0     4199 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/logic_unit.py
+-rw-r--r--   0        0        0     3541 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/memory_unit.py
+-rw-r--r--   0        0        0      825 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/processing_unit.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/io/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/__init__.py
+-rw-r--r--   0        0        0     1193 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/agent_memory.py
+-rw-r--r--   0        0        0     5309 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/chroma_vector_store.py
+-rw-r--r--   0        0        0      641 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/document.py
+-rw-r--r--   0        0        0     2620 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/embeddings.py
+-rw-r--r--   0        0        0      907 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/file_memory.py
+-rw-r--r--   0        0        0     4203 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/file_system_vector_store.py
+-rw-r--r--   0        0        0     3974 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/in_memory_file_memory.py
+-rw-r--r--   0        0        0     5788 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/local_file_memory.py
+-rw-r--r--   0        0        0     4845 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/local_symbolic_memory.py
+-rw-r--r--   0        0        0     3770 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
+-rw-r--r--   0        0        0      996 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/noop_memory.py
+-rw-r--r--   0        0        0     1984 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/s3_file_memory.py
+-rw-r--r--   0        0        0      975 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/semantic_memory.py
+-rw-r--r--   0        0        0     2809 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/similarity_memory.py
+-rw-r--r--   0        0        0     1516 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/vector_store.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/__init__.py
+-rw-r--r--   0        0        0      771 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/authentication_processor.py
+-rw-r--r--   0        0        0     2091 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/azure_authorizer.py
+-rw-r--r--   0        0        0     1277 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/functional_authorizer.py
+-rw-r--r--   0        0        0     2001 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/google_auth.py
+-rw-r--r--   0        0        0     1867 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/jwt_processor.py
+-rw-r--r--   0        0        0      484 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/okta_authorizor.py
+-rw-r--r--   0        0        0     1017 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/permissions.py
+-rw-r--r--   0        0        0     2508 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/process_authorizer.py
+-rw-r--r--   0        0        0     2977 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/security_manager.py
+-rw-r--r--   0        0        0     1035 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/security_middleware.py
+-rw-r--r--   0        0        0      428 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/user.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/__init__.py
+-rw-r--r--   0        0        0     1377 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/agent_contract.py
+-rw-r--r--   0        0        0    21672 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/agent_controller.py
+-rw-r--r--   0        0        0    13943 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/agent_machine.py
+-rw-r--r--   0        0        0     1149 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/dynamic_middleware.py
+-rw-r--r--   0        0        0     3432 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/fn_handler.py
+-rw-r--r--   0        0        0     4880 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/process_file_system.py
+-rw-r--r--   0        0        0     4275 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/processes.py
+-rw-r--r--   0        0        0     6895 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/reference_model.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/resources/__init__.py
+-rw-r--r--   0        0        0      314 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/resources/agent_resource.py
+-rw-r--r--   0        0        0      414 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/resources/machine_resource.py
+-rw-r--r--   0        0        0      684 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/resources/reference_resource.py
+-rw-r--r--   0        0        0     1663 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/resources/resources_base.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/__init__.py
+-rw-r--r--   0        0        0      509 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/async_wrapper.py
+-rw-r--r--   0        0        0     2806 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/class_utils.py
+-rw-r--r--   0        0        0     1604 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/image_utils.py
+-rw-r--r--   0        0        0     3812 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/replay.py
+-rw-r--r--   0        0        0     6483 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/schema_to_model.py
+-rw-r--r--   0        0        0      900 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/str_utils.py
+-rw-r--r--   0        0        0     3445 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/stream_collector.py
+-rw-r--r--   0        0        0      565 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/logging.conf
+-rw-r--r--   0        0        0     2030 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/pyproject.toml
+-rw-r--r--   0        0        0     4807 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.26/PKG-INFO
```

### Comparing `eidolon_ai_sdk-0.1.25/README.md` & `eidolon_ai_sdk-0.1.26/README.md`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/agent.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import annotations
 
 import typing
 from pydantic import BaseModel
 from typing import List, TypeVar, Generic
 
-from eidolon_ai_sdk.cpu.agent_cpu import AgentCPU
+from eidolon_ai_sdk.cpu.agent_cpu import APU
 from eidolon_ai_sdk.cpu.agents_logic_unit import (
     AgentsLogicUnit,
     AgentsLogicUnitSpec,
 )
 from eidolon_ai_sdk.system.fn_handler import FnHandler, register_handler
 from eidolon_ai_sdk.system.reference_model import Specable, AnnotatedReference
 
 
 class AgentSpec(BaseModel):
-    cpu: AnnotatedReference[AgentCPU]
+    cpu: AnnotatedReference[APU]
     agent_refs: List[str] = []
 
 
 class Agent(Specable[AgentSpec]):
-    cpu: AgentCPU
+    cpu: APU
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.cpu = self.spec.cpu.instantiate()
         if self.spec.agent_refs and hasattr(self.cpu, "logic_units"):
             self.cpu.logic_units.append(
                 AgentsLogicUnit(
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         if guess_type and mimetype is None:
             import filetype
 
             mimetype = filetype.guess_mime(data)
             if mimetype is None and path is not None:
                 mimetype = mimetypes.guess_type(path)[0]
             if mimetype is None:
-                if path.endswith(".md"):
+                if path and path.endswith(".md"):
                     mimetype = "text/x-markdown"
                 else:
                     mimetype = "text/plain"
 
         return cls(
             data=data,
             path=path,
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/generic_agent.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/generic_agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from typing import Annotated, Dict, Any, Literal, Type, Union
 
 from fastapi import Body
 from jinja2 import Environment, StrictUndefined, meta
 from pydantic import BaseModel, field_validator, Field, model_validator
 from pydantic_core import to_jsonable_python
 
+from eidolon_ai_client.events import AgentStateEvent
 from eidolon_ai_sdk.agent.agent import (
     Agent,
     register_action,
     AgentState,
     AgentSpec,
     register_program,
 )
-from eidolon_ai_sdk.cpu.agent_io import UserTextCPUMessage, SystemCPUMessage, ImageCPUMessage
-from eidolon_ai_client.events import AgentStateEvent
+from eidolon_ai_sdk.cpu.agent_io import UserTextAPUMessage, SystemAPUMessage
 from eidolon_ai_sdk.system.fn_handler import FnHandler
 from eidolon_ai_sdk.system.reference_model import Specable
 from eidolon_ai_sdk.util.schema_to_model import schema_to_model
 
 
 class GenericAgentSpec(AgentSpec):
     description: str
@@ -68,23 +68,14 @@
     properties: Dict[str, Any] = {}
     if spec.input_schema:
         properties["body"] = dict(
             type="object",
             properties=spec.input_schema,
         )
     required = ["body"]
-    if spec.files == "single" or spec.files == "single-optional":
-        properties["file"] = dict(type="string", format="binary")
-        if spec.files == "single":
-            required.append("file")
-    elif spec.files == "multiple":
-        properties["file"] = dict(type="array", items=dict(type="string", format="binary"))
-        required.append("file")
-    elif "files" in properties:
-        del properties["file"]
     schema = {"type": "object", "properties": properties, "required": required}
     return schema_to_model(schema, f"{handler.name.capitalize()}InputModel")
 
 
 def make_output_schema(agent: object, handler: FnHandler) -> Type[Any]:
     # noinspection PyUnresolvedReferences
     spec = agent.spec
@@ -102,39 +93,33 @@
         output_model=make_output_schema,
         description=make_description,
     )
     async def question(self, process_id, **kwargs) -> AgentState[Any]:
         body = dict(datetime_iso=datetime.now().isoformat())
         body.update(kwargs.get("body") or {})
         body = to_jsonable_python(body)
-        files = kwargs.get("file", [])
-        if not isinstance(files, list):
-            files = [files]
 
         env = Environment(undefined=StrictUndefined)
         t = await self.cpu.main_thread(process_id)
         await t.set_boot_messages(
-            prompts=[SystemCPUMessage(prompt=(env.from_string(self.spec.system_prompt).render(**body)))],
+            prompts=[SystemAPUMessage(prompt=(env.from_string(self.spec.system_prompt).render(**body)))],
         )
 
         # pull out any kwargs that are UploadFile and put them in a list of UserImageCPUMessage
         image_messages = []
-        for file in files:
-            if file:
-                image_messages.append(ImageCPUMessage(image=file.file, prompt=file.filename))
 
         response = t.stream_request(
             prompts=[
-                UserTextCPUMessage(prompt=(env.from_string(self.spec.user_prompt).render(**body))),
+                UserTextAPUMessage(prompt=(env.from_string(self.spec.user_prompt).render(**body))),
                 *image_messages,
             ],
             output_format=self.spec.output_schema,
         )
         async for event in response:
             yield event
         yield AgentStateEvent(state="idle")
 
     @register_action("idle", "http_error")
     async def respond(self, process_id, statement: Annotated[str, Body(embed=True)]) -> AgentState[Any]:
         t = await self.cpu.main_thread(process_id)
-        response = await t.run_request([UserTextCPUMessage(prompt=statement)], self.spec.output_schema)
+        response = await t.run_request([UserTextAPUMessage(prompt=statement)], self.spec.output_schema)
         return AgentState(name="idle", data=response)
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/openai_whisper_agent.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/openai_whisper_agent.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from typing import Annotated
 
 from fastapi import Body
 
+from eidolon_ai_client.events import FileHandle
 from eidolon_ai_sdk.agent.agent import AgentSpec, Agent, register_program
 from eidolon_ai_sdk.agent_os import AgentOS
 from eidolon_ai_sdk.cpu.llm.open_ai_speech import OpenAiSpeech
-from eidolon_ai_sdk.system.process_file_system import FileHandle
 from eidolon_ai_sdk.system.processes import ProcessDoc
 from eidolon_ai_sdk.system.reference_model import AnnotatedReference, Specable
 
 
 class AutonomousSpeechAgentSpec(AgentSpec):
     speech_llm: AnnotatedReference[OpenAiSpeech]
 
 
 class AutonomousSpeechAgent(Agent, Specable[AutonomousSpeechAgentSpec]):
     speech_llm: OpenAiSpeech
 
     def __init__(self, spec: AutonomousSpeechAgentSpec):
         super().__init__(spec=spec)
-        self.speech_llm = self.spec.speech_llm.instantiate()
+        self.speech_llm = self.spec.speech_llm.instantiate(processing_unit_locator=None)
         self.cpu = self.spec.cpu.instantiate()
 
     @register_program()
     async def speech_to_text(
         self, process_id, audio: Annotated[FileHandle, Body(description="The audio file", embed=True)]
     ):
         await ProcessDoc.set_delete_on_terminate(process_id, True)
@@ -41,8 +41,8 @@
     @register_program()
     async def text_to_speech(
         self, process_id: str, text: Annotated[str, Body(description="The text to speak", embed=True)]
     ) -> FileHandle:
         audio_result = await self.speech_llm.text_to_speech(text)
         file_id = await AgentOS.process_file_system.write_file(process_id, audio_result, {"mimetype": "audio/mpeg"})
 
-        return FileHandle(machineURL=AgentOS.current_machine_url(), process_id=process_id, file_id=file_id)
+        return file_id
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import uuid
 from jinja2 import Environment, StrictUndefined
 from pydantic import Field
 from typing import List
 
 from eidolon_ai_sdk.agent.retriever_agent.question_transformer import QuestionTransformerSpec, QuestionTransformer
-from eidolon_ai_sdk.cpu.agent_cpu import AgentCPU
-from eidolon_ai_sdk.cpu.agent_io import UserTextCPUMessage
+from eidolon_ai_sdk.cpu.agent_cpu import APU
+from eidolon_ai_sdk.cpu.agent_io import UserTextAPUMessage
 from eidolon_ai_sdk.system.reference_model import Specable, AnnotatedReference
 
 
 class HydeQuestionTransformerSpec(QuestionTransformerSpec):
-    cpu: AnnotatedReference[AgentCPU]
+    cpu: AnnotatedReference[APU]
     prompt: str = Field(
         default="Please write a passage to answer the question \nQuestion: {{question}}?\nPassage:",
         description="The prompt to be used for the question transformer. This should be a template where the user question is the field {{question}}",
     )
 
 
 class HydeQuestionTransformer(QuestionTransformer, Specable[HydeQuestionTransformerSpec]):
@@ -23,10 +23,10 @@
         self.cpu = self.spec.cpu.instantiate()
         self.cpu.record_memory = False
 
     async def transform(self, question: str) -> List[str]:
         thread = await self.cpu.main_thread(str(uuid.uuid4()))
         env = Environment(undefined=StrictUndefined)
         userPrompt = env.from_string(self.spec.prompt).render(question=question)
-        response = await thread.run_request(prompts=[UserTextCPUMessage(prompt=userPrompt)], output_format="str")
+        response = await thread.run_request(prompts=[UserTextAPUMessage(prompt=userPrompt)], output_format="str")
 
         return [response]
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import uuid
 from jinja2 import Environment, StrictUndefined
 from pydantic import Field, BaseModel
 from typing import List
 
 from eidolon_ai_sdk.agent.retriever_agent.question_transformer import QuestionTransformerSpec, QuestionTransformer
-from eidolon_ai_sdk.cpu.agent_cpu import AgentCPU
-from eidolon_ai_sdk.cpu.agent_io import UserTextCPUMessage
+from eidolon_ai_sdk.cpu.agent_cpu import APU
+from eidolon_ai_sdk.cpu.agent_io import UserTextAPUMessage
 from eidolon_ai_sdk.system.reference_model import Specable, AnnotatedReference
 
 
 class MultiQuestionTransformerSpec(QuestionTransformerSpec):
-    cpu: AnnotatedReference[AgentCPU]
+    cpu: AnnotatedReference[APU]
     keep_original: bool = Field(default=True, description="Whether to keep the original question in the output")
     number_to_generate: int = Field(default=3, description="The number of questions to generate")
     prompt: str = Field(
         default="""You are an AI language model assistant. Your task is to generate {{number_to_generate}} different versions of the given user 
     question to retrieve relevant documents from a vector  database. By generating multiple perspectives on the user question, 
     your goal is to help the user overcome some of the limitations of distance-based similarity search. Provide these alternative 
     questions separated by newlines. Original question: {{question}}""",
@@ -35,14 +35,14 @@
     async def transform(self, question: str) -> List[str]:
         thread = await self.cpu.main_thread(str(uuid.uuid4()))
         env = Environment(undefined=StrictUndefined)
         userPrompt = env.from_string(self.spec.prompt).render(
             question=question, number_to_generate=self.spec.number_to_generate
         )
         response = await thread.run_request(
-            prompts=[UserTextCPUMessage(prompt=userPrompt)], output_format=QuestionList.model_json_schema()
+            prompts=[UserTextAPUMessage(prompt=userPrompt)], output_format=QuestionList.model_json_schema()
         )
 
         if self.spec.keep_original:
             return [question] + response["questions"]
         else:
             return response.questions
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/retriever.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/retriever.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,25 +52,25 @@
             rerank_questions[question] = {doc.id: doc.score for doc in docs}
 
         reranked_docs = await self.document_reranker.rerank(rerank_questions)
 
         # now limit reranked_docs to max_num_results
         reranked_docs = reranked_docs[: self.spec.max_num_results]
 
-        docs = AgentOS.similarity_memory.vector_store.get_docs(
+        docs = AgentOS.similarity_memory.get_docs(
             vector_collection_name, [doc[0] for doc in reranked_docs]
         )
         summaries = []
         async for doc in docs:
             file_path = doc.metadata["source"]
             summaries.append(
                 DocSummary(id=doc.id, file_name=file_path.split("/")[-1], file_path=file_path, text=doc.page_content)
             )
 
         return summaries
 
     async def _embed_question(self, vector_collection_name, question):
-        embedded_q = await AgentOS.similarity_memory.embedder.embed_text(question)
-        results_ = await AgentOS.similarity_memory.vector_store.raw_query(
+        embedded_q = await AgentOS.similarity_memory.embed_text(question)
+        results_ = await AgentOS.similarity_memory.raw_query(
             vector_collection_name, embedded_q, self.spec.max_num_results
         )
         return results_
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         return value
 
 
 class RetrieverAgent(Retriever, Specable[RetrieverAgentSpec]):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.document_manager = self.spec.document_manager.instantiate()
+        self.document_manager.collection_name = f"doc_contents_{self.spec.name}"
 
     @register_program()
     async def list_files(self) -> AgentState[List[str]]:
         """
         List the files in the document store.
         :return: The response from the cpu
         """
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/simple_agent.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/simple_agent.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,74 +5,93 @@
 
 from fastapi import Body
 from jinja2 import Environment, meta, StrictUndefined
 from openai import BaseModel
 from pydantic import field_validator, model_validator
 from pydantic_core import to_jsonable_python
 
-from eidolon_ai_client.events import AgentStateEvent, StreamEvent, StringOutputEvent
+from eidolon_ai_client.events import AgentStateEvent, StreamEvent, StringOutputEvent, UserInputEvent, FileHandle
+from eidolon_ai_client.util.logger import logger
 from eidolon_ai_client.util.request_context import RequestContext
 from eidolon_ai_sdk.agent.agent import register_action
-from eidolon_ai_sdk.cpu.agent_cpu import AgentCPU
-from eidolon_ai_sdk.cpu.agent_io import SystemCPUMessage, ImageCPUMessage, UserTextCPUMessage
+from eidolon_ai_sdk.agent.doc_manager.document_processor import DocumentProcessor
+from eidolon_ai_sdk.cpu.agent_cpu import APU
+from eidolon_ai_sdk.cpu.agent_io import SystemAPUMessage, UserTextAPUMessage, AttachedFileMessage
 from eidolon_ai_sdk.cpu.agents_logic_unit import AgentsLogicUnitSpec, AgentsLogicUnit
 from eidolon_ai_sdk.system.processes import ProcessDoc
 from eidolon_ai_sdk.system.reference_model import Specable, AnnotatedReference
 from eidolon_ai_sdk.util.schema_to_model import schema_to_model
 
 
 class ActionDefinition(BaseModel):
     name: str = "converse"
     description: Optional[str] = None
     user_prompt: str = "{{ body }}"
     input_schema: dict = None
     output_schema: Union[Literal["str"], Dict[str, Any]] = "str"
-    files: Literal["disable", "single-optional", "single", "multiple"] = "disable"
+    allow_file_upload: bool = False
+    # allow all types for text, image, audio, word, pdf, json, etc
+    supported_mime_types: List[str] = []  # an empty list means all types are supported
     allowed_states: List[str] = ["initialized", "idle", "http_error"]
     output_state: str = "idle"
 
     @field_validator("input_schema")
     def validate_prompt_properties(cls, input_dict):
         if not isinstance(input_dict, dict):
             raise ValueError("prompt_properties must be a dict")
         for k, v in input_dict.items():
             if isinstance(v, dict):
                 if v.get("format") == "binary":
                     raise ValueError(
-                        "prompt_properties cannot contain format = 'binary' fields. Use the files option instead"
+                        "prompt_properties cannot contain format = 'binary' fields."
                     )
         return input_dict
 
+    @field_validator("supported_mime_types")
+    def validate_supported_mime_types(cls, supported_mime_types):
+        if not isinstance(supported_mime_types, list):
+            raise ValueError("supported_mime_types must be a List[str]")
+        if not supported_mime_types:
+            return supported_mime_types
+
+        all_mime_types = {"application/json", "text/plain", "image/*", "audio/*", "application/pdf", "application/msword",
+                          "application/vnd.openxmlformats-officedocument.wordprocessingml.document", "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
+                          "application/vnd.ms-excel", "application/vnd.ms-powerpoint", "application/vnd.openxmlformats-officedocument.presentationml.presentation"}
+        bad_types = []
+        for mime_type in supported_mime_types:
+            if mime_type not in all_mime_types:
+                bad_types.append(mime_type)
+        if bad_types:
+            raise ValueError(f"supported_mime_types contains unsupported entries: {bad_types}")
+
+        return supported_mime_types
+
     def make_input_schema(self, agent, handler):
         properties: Dict[str, Any] = {}
         required = []
         user_vars = meta.find_undeclared_variables(Environment().parse(self.user_prompt))
         # pop out any reserved keywords we will inject
         if "datetime_iso" in user_vars:
             user_vars.remove("datetime_iso")
         if self.input_schema is not None:
             properties["body"] = dict(type="object", properties=self.input_schema)
             required.append("body")
-        elif len(user_vars) == 1 and "body" in user_vars and not agent.spec.cpus:
+        elif len(user_vars) == 1 and "body" in user_vars and not agent.spec.apus and not self.allow_file_upload:
             properties["body"] = dict(type="string", default=Body(..., media_type="text/plain"))
             required.append("body")
         elif user_vars:
             props = {v: dict(type="string") for v in user_vars}
             properties["body"] = dict(type="object", properties=props)
             required.append("body")
 
-        if self.files == "single-optional":
-            properties["file"] = dict(type="string", format="binary")
-        elif self.files == "single":
-            properties["file"] = dict(type="string", format="binary")
-            required.append("file")
-        elif self.files == "multiple":
-            properties["file"] = dict(type="array", items=dict(type="string", format="binary"))
-        if agent.spec.cpus:
-            cpu_names = [cpu.title for cpu in agent.spec.cpus]
+        if self.allow_file_upload:
+            properties["body"]["properties"]["attached_files"] = dict(type="array", items=FileHandle.model_json_schema())
+
+        if agent.spec.apus:
+            cpu_names = [cpu.title for cpu in agent.spec.apus]
             default = agent.cpu.title
             properties["body"]["properties"]["execute_on_cpu"] = dict(type="string", enum=cpu_names, default=default)
             if "required" not in properties["body"]:
                 properties["body"]["required"] = []
             properties["body"]["required"].append("execute_on_cpu")
 
         schema = {"type": "object", "properties": properties, "required": required}
@@ -83,73 +102,76 @@
             raise ValueError("output_schema must be specified")
         model_name = f"{handler.name.capitalize()}{self.name.capitalize()}OutputModel"
         return str if self.output_schema == "str" else schema_to_model(self.output_schema, model_name)
 
 
 class NamedCPU(BaseModel):
     title: Optional[str] = None
-    cpu: AnnotatedReference[AgentCPU]
+    apu: AnnotatedReference[APU]
     default: bool = False
 
 
 class SimpleAgentSpec(BaseModel):
     description: Optional[str] = None
     system_prompt: str = "You are a helpful assistant"
     agent_refs: List[str] = []
     actions: List[ActionDefinition] = [ActionDefinition()]
-    cpu: AnnotatedReference[AgentCPU] = None
-    cpus: Optional[List[NamedCPU]] = []
+    apu: AnnotatedReference[APU] = None
+    apus: List[NamedCPU] = []
     title_generation_mode: Literal["none", "on_request"] = "on_request"
+    doc_processor: AnnotatedReference[DocumentProcessor]
 
     @model_validator(mode="before")
     def validate_cpu(cls, value):
-        if "cpu" in value and "cpus" in value:
-            raise ValueError("Cannot specify both cpu and cpus")
+        if "cpu" in value:
+            logger.warning("cpu is deprecated, use apu instead")
+            value["apu"] = value.pop("cpu")
+        if "apu" in value and "apus" in value:
+            raise ValueError("Cannot specify both apu and apus")
         return value
 
     # noinspection PyTypeChecker
     @model_validator(mode="after")
     def validate_cpus(self):
-        if self.cpus:
-            self.cpu = None
+        if self.apus:
+            self.apu = None
         return self
 
 
 class SimpleAgent(Specable[SimpleAgentSpec]):
     generate_title_prompt = ("You are generating a title for a conversation. Consider the context and content of the discussion or text. "
                              "Create a concise, relevant, and accurate representation of the main topic or theme in the content."
                              "Create a title that draws insiration from key phrases or ideas in the content. "
                              "The title should be no longer than 5 words. Do not wrap the title in quotes. Answer only with the title. The prompt for the conversation is:\n")
 
     def __init__(self, spec):
         super().__init__(spec=spec)
-        if self.spec.cpu:
-            self.cpu = self.spec.cpu.instantiate()
+        if self.spec.apu:
+            self.cpu = self.spec.apu.instantiate()
             self.cpu.title = self.cpu.__class__.__name__
             self._register_refs_logic_unit(self.cpu, self.spec.agent_refs)
         else:
             self.cpus = []
-            for cpu_spec in self.spec.cpus:
-                cpu = cpu_spec.cpu.instantiate()
+            for cpu_spec in self.spec.apus:
+                apu = cpu_spec.apu.instantiate()
                 # todo - add title from metadata
-                cpu.title = cpu_spec.title or cpu.__class__.__name__
+                apu.title = cpu_spec.title or apu.__class__.__name__
                 if cpu_spec.default:
-                    cpu.default = True
-                    self.cpu = cpu
-                self._register_refs_logic_unit(cpu, self.spec.agent_refs)
-                self.cpus.append(cpu)
+                    apu.default = True
+                    self.cpu = apu
+                self._register_refs_logic_unit(apu, self.spec.agent_refs)
+                self.cpus.append(apu)
 
         if self.spec.title_generation_mode == "on_request":
             # add a title generation action
             action = ActionDefinition(
                 name="generate_title",
                 description="Generate a title for the conversation",
                 user_prompt=self.generate_title_prompt + "{{ body }}",
                 output_schema="str",
-                files="disable",
                 allowed_states=["initialized", "idle"],
                 output_state="idle",
             )
 
             setattr(
                 self,
                 action.name,
@@ -182,15 +204,15 @@
                     processing_unit_locator=cpu,
                     spec=AgentsLogicUnitSpec(agents=agent_refs),
                 )
             )
 
     async def create_process(self, process_id):
         t = await self.cpu.main_thread(process_id)
-        await t.set_boot_messages(prompts=[SystemCPUMessage(prompt=self.spec.system_prompt)])
+        await t.set_boot_messages(prompts=[SystemAPUMessage(prompt=self.spec.system_prompt)])
 
     @staticmethod
     def _act_wrapper(action, action_fn):
         async def fn(self, process_id, **kwargs):
             async for e in action_fn(self, action, process_id, **kwargs):
                 yield e
 
@@ -198,38 +220,41 @@
 
     async def _act(self, action: ActionDefinition, process_id, **kwargs) -> AsyncIterable[StreamEvent]:
         execute_on_cpu = None
         request_body = to_jsonable_python(kwargs.get("body") or {})
         if "execute_on_cpu" in request_body:
             execute_on_cpu = request_body.pop("execute_on_cpu")
 
+        attached_files: List[FileHandle] = []
+        attached_files_messages = []
+        if "attached_files" in request_body:
+            # add a new file handle message
+            attached_files = request_body.pop("attached_files") or []
+            for file in attached_files:
+                attached_files_messages.append(AttachedFileMessage(file=file, include_directly=True))
+
         body = dict(datetime_iso=datetime.now().isoformat(), body=str(request_body))
         if isinstance(request_body, dict):
             body.update(request_body)
 
-        files = kwargs.get("file", []) or []
-        if not isinstance(files, list):
-            files = [files]
-
-        image_messages = [ImageCPUMessage(image=file.file, prompt=file.filename) for file in files if file]
-
         env = Environment(undefined=StrictUndefined)
-        text_message = UserTextCPUMessage(prompt=env.from_string(action.user_prompt).render(**body))
+        text_message = UserTextAPUMessage(prompt=env.from_string(action.user_prompt).render(**body))
 
         if execute_on_cpu:
             cpu = self.cpu
             for named_cpu in self.cpus:
                 if named_cpu.title == execute_on_cpu:
                     cpu = named_cpu
                     break
         else:
             cpu = self.cpu
 
+        yield UserInputEvent(input=request_body, files=attached_files)
         thread = await cpu.main_thread(process_id)
-        response = thread.stream_request(output_format=action.output_schema, prompts=[*image_messages, text_message])
+        response = thread.stream_request(output_format=action.output_schema, prompts=[*attached_files_messages, text_message])
 
         async for event in response:
             yield event
         yield AgentStateEvent(state=action.output_state)
 
     async def _gen_title(self, action: ActionDefinition, process_id, **kwargs) -> AsyncIterable[StreamEvent]:
         last_state = RequestContext.get("__last_state__")
@@ -241,26 +266,25 @@
             execute_on_cpu = request_body.pop("execute_on_cpu")
 
         body = dict(datetime_iso=datetime.now().isoformat(), body=str(request_body))
         if isinstance(request_body, dict):
             body.update(request_body)
 
         env = Environment(undefined=StrictUndefined)
-        text_message = UserTextCPUMessage(prompt=env.from_string(action.user_prompt).render(**body))
+        text_message = UserTextAPUMessage(prompt=env.from_string(action.user_prompt).render(**body))
 
         if execute_on_cpu:
             cpu = self.cpu
             for named_cpu in self.cpus:
                 if named_cpu.title == execute_on_cpu:
                     cpu = named_cpu
                     break
         else:
             cpu = self.cpu
 
-        title_message = UserTextCPUMessage(prompt=self.generate_title_prompt + text_message.prompt)
+        title_message = UserTextAPUMessage(prompt=self.generate_title_prompt + text_message.prompt)
         response = await (await cpu.new_thread(process_id)).run_request(prompts=[title_message])
         await process_obj.update(title=response)
 
         yield StringOutputEvent(content=response)
         # return to the previous state
-        print(process_obj.state)
         yield AgentStateEvent(state=last_state)
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/checker.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/checker.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import List
 
 from jinja2 import StrictUndefined, Environment
 from pydantic import Field, BaseModel
 
-from eidolon_ai_sdk.cpu.agent_cpu import AgentCPU
-from eidolon_ai_sdk.cpu.agent_io import UserTextCPUMessage
+from eidolon_ai_sdk.cpu.agent_cpu import APU
+from eidolon_ai_sdk.cpu.agent_io import UserTextAPUMessage
 from eidolon_ai_sdk.agent.tot_agent.prompts import CHECKER_PROMPT
 from eidolon_ai_sdk.agent.tot_agent.thought import ThoughtValidity
 from eidolon_ai_sdk.system.reference_model import Specable
 
 
 class TotCheckerConfig(BaseModel):
     prompt: str = CHECKER_PROMPT
     examples: str = ""
 
 
 class ToTChecker(Specable[TotCheckerConfig]):
     spec: TotCheckerConfig
-    cpu: AgentCPU
+    cpu: APU
 
     def __init__(self, cpu, spec):
         super().__init__(spec)
         self.cpu = cpu
         self.spec = spec
 
     """
@@ -50,12 +50,12 @@
                 thoughts=thoughts,
                 examples=self.spec.examples,
             )
         )
 
         thread = await self.cpu.new_thread(process_id)
         resp = await thread.run_request(
-            prompts=[UserTextCPUMessage(prompt=checker_prompt)],
+            prompts=[UserTextAPUMessage(prompt=checker_prompt)],
             output_format=ThoughtValidity.model_json_schema(),
         )
 
         return ThoughtValidity.model_validate(resp)
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/controller.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/controller.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/memory.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/prompts.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/prompts.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/thought_generators.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/thought_generators.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 from abc import abstractmethod
 from typing import Any, Dict, List, Callable, Awaitable
 
 from jinja2 import StrictUndefined, Environment
 from pydantic import Field, BaseModel
 
-from eidolon_ai_sdk.cpu.agent_io import SystemCPUMessage, UserTextCPUMessage, CPUMessageTypes
+from eidolon_ai_sdk.cpu.agent_io import SystemAPUMessage, UserTextAPUMessage, CPUMessageTypes
 from eidolon_ai_sdk.cpu.llm_message import UserMessage, LLMMessage
 from eidolon_ai_sdk.agent.tot_agent.prompts import (
     POST_AMBLE,
     THOUGHTS,
     PREAMBLE,
     POST_AMBLE_MULTI,
 )
@@ -46,19 +46,19 @@
         thoughts_tuple = tuple(thoughts_path)
         preamble_txt = self.env.from_string(self.spec.preamble).render(thoughts=thoughts_tuple, n=self.spec.num_children)
         thoughts_txt = self.env.from_string(self.spec.thoughts).render(thoughts=thoughts_tuple, n=self.spec.num_children)
         post_amble_txt = self.env.from_string(self.spec.post_amble).render(
             thoughts=thoughts_tuple, n=self.spec.num_children
         )
         return (
-            [SystemCPUMessage(prompt=preamble_txt)],
+            [SystemAPUMessage(prompt=preamble_txt)],
             [
-                UserTextCPUMessage(prompt=user_message),
-                UserTextCPUMessage(prompt=thoughts_txt),
-                UserTextCPUMessage(prompt=post_amble_txt),
+                UserTextAPUMessage(prompt=user_message),
+                UserTextAPUMessage(prompt=thoughts_txt),
+                UserTextAPUMessage(prompt=post_amble_txt),
             ],
         )
 
     @abstractmethod
     async def next_thought(
         self,
         user_message: str,
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent/tot_agent/tot_agent.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/tot_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from eidolon_ai_sdk.agent.tot_agent.checker import ToTChecker
 from eidolon_ai_sdk.agent.tot_agent.controller import ToTController
 from eidolon_ai_sdk.agent.tot_agent.memory import ToTDFSMemory
 from eidolon_ai_sdk.agent.tot_agent.thought import Thought
 from eidolon_ai_sdk.agent.tot_agent.thought_generators import (
     ThoughtGenerationStrategy,
 )
-from eidolon_ai_sdk.cpu.agent_io import UserTextCPUMessage
+from eidolon_ai_sdk.cpu.agent_io import UserTextAPUMessage
 from eidolon_ai_sdk.cpu.llm_message import LLMMessage
 from eidolon_ai_sdk.system.reference_model import Specable, AnnotatedReference
 from eidolon_ai_client.util.logger import logger
 from eidolon_ai_sdk.util.schema_to_model import schema_to_model
 
 
 class ToTAgentConfig(AgentSpec):
@@ -140,16 +140,16 @@
             thought = Thought(text=thought_text, validity=thought_validity.validity)
             self.tot_memory.store(thought)
             self.log_thought(thought, level)
             if thought.validity == "VALID":
                 mainThread = await self.cpu.main_thread(process_id)
                 # go back to llm now with the tree of thoughts and the requested output format
                 conversation = [
-                    UserTextCPUMessage(prompt=question),
-                    UserTextCPUMessage(prompt="THOUGHTS\n\n" + ("\n".join(thoughts_path + [thought_text]))),
+                    UserTextAPUMessage(prompt=question),
+                    UserTextAPUMessage(prompt="THOUGHTS\n\n" + ("\n".join(thoughts_path + [thought_text]))),
                 ]
                 resp = await mainThread.run_request(conversation, self.spec.output_schema)
                 return TotResponse(answer=resp, thoughts=thoughts_path)
             thoughts_path = self.tot_controller.thoughts(self.tot_memory)
 
         synopsis = self.tot_controller.exploration_synopsis(self.tot_memory)
         if self.spec.fallback == "ERROR":
@@ -158,16 +158,16 @@
                 detail=dict(
                     error=f"Could not find a valid thought within {self.spec.num_iterations} iterations.",
                     remaining_thoughts=synopsis,
                 ),
             )
         elif self.spec.fallback == "LLM":
             conversation = [
-                UserTextCPUMessage(prompt=question),
-                UserTextCPUMessage(
+                UserTextAPUMessage(prompt=question),
+                UserTextAPUMessage(
                     prompt="You have had some helpful thoughts on the question. Please use them to provide an answer\n\n"
                     + str(synopsis)
                 ),
             ]
             thread = await self.cpu.new_thread(process_id)
             resp = await thread.run_request(conversation, self.spec.output_schema)
             return TotResponse(answer=resp, thoughts=thoughts_path)
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/agent_os.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent_os.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from __future__ import annotations
 
 import os
-
 import pathlib
 from typing import Dict, Tuple, TypeVar, Type
 
-from eidolon_ai_sdk.system.resources.resources_base import load_resources, Resource
 from eidolon_ai_client.util.logger import logger
+from eidolon_ai_sdk.agent_os_interfaces import ProcessFileSystem, FileMemory, SymbolicMemory, SecurityManager, SimilarityMemory
+from eidolon_ai_sdk.system.resources.resources_base import load_resources, Resource
 
 T = TypeVar("T", bound="Resource")  # noqa: F821
 S = TypeVar("S", bound="BaseModel")  # noqa: F821
 
 
 class AgentOS:
     _resources: Dict[str, Dict[str, Tuple["Resource", str]]] = ...  # noqa: F821
-    file_memory: "FileMemory" = ...  # noqa: F821
-    symbolic_memory: "SymbolicMemory" = ...  # noqa: F821
-    similarity_memory: "SimilarityMemory" = ...  # noqa: F821
-    security_manager: "SecurityManager" = ...  # noqa: F821
-    process_file_system: "ProcessFileSystem" = ...  # noqa: F821
+    file_memory: FileMemory = ...  # noqa: F821
+    symbolic_memory: SymbolicMemory = ...  # noqa: F821
+    similarity_memory: SimilarityMemory = ...  # noqa: F821
+    security_manager: SecurityManager = ...  # noqa: F821
+    process_file_system: ProcessFileSystem = ...  # noqa: F821
 
     @staticmethod
     def current_machine_url() -> str:
         return os.environ.get("EIDOLON_LOCAL_MACHINE", "http://localhost:8080")
 
     @classmethod
     def _get_or_load_resources(cls) -> Dict[str, Dict[str, Tuple[Resource, str]]]:
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/bin/agent_creator.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/bin/agent_creator.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/bin/agent_http_server.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/bin/agent_http_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,26 +206,30 @@
         log_level=log_level_str,
         reload=args.reload,
     )
 
 
 # noinspection PyTypeChecker
 def start_app(lifespan):
-    _app = FastAPI(lifespan=lifespan)
-    _app.add_middleware(DynamicMiddleware)
-    _app.add_middleware(ContextMiddleware)
-    _app.add_middleware(
-        CORSMiddleware,
-        allow_origins=["*"],
-        allow_credentials=True,
-        allow_methods=["*"],
-        allow_headers=["*"],
-    )
-    _app.add_middleware(SecurityMiddleware)
-    _app.add_middleware(LoggingMiddleware)
-    _app.add_exception_handler(PermissionException, permission_exception_handler)
-    FastAPIInstrumentor.instrument_app(_app)
-    return _app
+    try:
+        _app = FastAPI(lifespan=lifespan)
+        _app.add_middleware(DynamicMiddleware)
+        _app.add_middleware(ContextMiddleware)
+        _app.add_middleware(
+            CORSMiddleware,
+            allow_origins=["*"],
+            allow_credentials=True,
+            allow_methods=["*"],
+            allow_headers=["*"],
+        )
+        _app.add_middleware(SecurityMiddleware)
+        _app.add_middleware(LoggingMiddleware)
+        _app.add_exception_handler(PermissionException, permission_exception_handler)
+        FastAPIInstrumentor.instrument_app(_app)
+        return _app
+    except Exception as e:
+        logger.exception("Failed to start FastAPI", e)
+        raise
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/bin/replay.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/bin/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/code_builtins.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/code_builtins.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from opentelemetry.exporter.otlp.proto.grpc.trace_exporter import OTLPSpanExporter
 from opentelemetry.sdk.trace import SpanProcessor
 from opentelemetry.sdk.trace.export import BatchSpanProcessor, SpanExporter
 from opentelemetry.sdk.trace.sampling import Sampler
 
 from eidolon_ai_client.util.logger import logger
 from eidolon_ai_sdk.agent.doc_manager.document_manager import DocumentManager
+from eidolon_ai_sdk.agent.doc_manager.document_processor import DocumentProcessor
 from eidolon_ai_sdk.agent.doc_manager.loaders.base_loader import DocumentLoader
 from eidolon_ai_sdk.agent.doc_manager.loaders.filesystem_loader import FilesystemLoader
 from eidolon_ai_sdk.agent.doc_manager.loaders.github_loader import GitHubLoader
 from eidolon_ai_sdk.agent.doc_manager.parsers.auto_parser import AutoParser
 from eidolon_ai_sdk.agent.doc_manager.parsers.base_parser import DocumentParser
 from eidolon_ai_sdk.agent.doc_manager.transformer.auto_transformer import AutoTransformer
 from eidolon_ai_sdk.agent.doc_manager.transformer.document_transformer import DocumentTransformer
@@ -26,47 +27,47 @@
 from eidolon_ai_sdk.agent.simple_agent import SimpleAgent
 from eidolon_ai_sdk.agent.tot_agent.checker import ToTChecker
 from eidolon_ai_sdk.agent.tot_agent.thought_generators import ThoughtGenerationStrategy, ProposePromptStrategy
 from eidolon_ai_sdk.agent.tot_agent.tot_agent import TreeOfThoughtsAgent
 from eidolon_ai_sdk.builtins.components.opentelemetry import OpenTelemetryManager, CustomSampler, NoopSpanExporter
 from eidolon_ai_sdk.builtins.components.usage import UsageMiddleware
 from eidolon_ai_sdk.builtins.logic_units.web_search import WebSearch, Browser, Search
-from eidolon_ai_sdk.cpu.agent_cpu import AgentCPU
+from eidolon_ai_sdk.cpu.agent_cpu import APU
 from eidolon_ai_sdk.cpu.agent_io import IOUnit
 from eidolon_ai_sdk.cpu.conversation_memory_unit import RawMemoryUnit
-from eidolon_ai_sdk.cpu.conversational_agent_cpu import ConversationalAgentCPU
+from eidolon_ai_sdk.cpu.conversational_apu import ConversationalAPU
+from eidolon_ai_sdk.agent_os_interfaces import FileMemory, SymbolicMemory, SimilarityMemory, SecurityManager
 from eidolon_ai_sdk.cpu.llm.anthropic_llm_unit import AnthropicLLMUnit
 from eidolon_ai_sdk.cpu.llm.mistral_llm_unit import MistralGPT
+from eidolon_ai_sdk.cpu.llm.open_ai_connection_handler import OpenAIConnectionHandler, AzureOpenAIConnectionHandler
 from eidolon_ai_sdk.cpu.llm.open_ai_llm_unit import OpenAIGPT
 from eidolon_ai_sdk.cpu.llm.open_ai_speech import OpenAiSpeech
 from eidolon_ai_sdk.cpu.llm_unit import LLMUnit
 from eidolon_ai_sdk.cpu.memory_unit import MemoryUnit
 from eidolon_ai_sdk.memory.s3_file_memory import S3FileMemory
 from eidolon_ai_sdk.security.azure_authorizer import AzureJWTProcessor
 from eidolon_ai_sdk.security.google_auth import GoogleJWTProcessor
 from eidolon_ai_sdk.system.dynamic_middleware import Middleware, MultiMiddleware
-from eidolon_ai_sdk.system.process_file_system import ProcessFileSystem
+from eidolon_ai_sdk.system.process_file_system import ProcessFileSystem, ProcessFileSystemImpl
 from eidolon_ai_usage_client.client import UsageClient
 
 try:
     from eidolon_ai_sdk.memory.chroma_vector_store import ChromaVectorStore
 except ImportError:
     logger.warning("Error, ChromaVectorStore is not available")
     ChromaVectorStore = None
 
 from eidolon_ai_sdk.memory.embeddings import NoopEmbedding, Embedding, OpenAIEmbedding
-from eidolon_ai_sdk.memory.file_memory import FileMemory
 from eidolon_ai_sdk.memory.local_file_memory import LocalFileMemory
 from eidolon_ai_sdk.memory.local_symbolic_memory import LocalSymbolicMemory
 from eidolon_ai_sdk.memory.mongo_symbolic_memory import MongoSymbolicMemory
 from eidolon_ai_sdk.memory.noop_memory import NoopVectorStore
-from eidolon_ai_sdk.memory.semantic_memory import SymbolicMemory
-from eidolon_ai_sdk.memory.similarity_memory import SimilarityMemory
+from eidolon_ai_sdk.memory.similarity_memory import SimilarityMemoryImpl
 from eidolon_ai_sdk.memory.vector_store import VectorStore
-from eidolon_ai_sdk.security.security_manager import SecurityManager
+from eidolon_ai_sdk.security.security_manager import SecurityManagerImpl
 from eidolon_ai_sdk.security.functional_authorizer import (
     FunctionalAuthorizer,
     NoopFunctionalAuth,
     GlobPatternFunctionalAuthorizer,
 )
 from eidolon_ai_sdk.security.process_authorizer import ProcessAuthorizer, PrivateAuthorizer
 from eidolon_ai_sdk.security.authentication_processor import AuthenticationProcessor, NoopAuthProcessor
@@ -102,15 +103,16 @@
     Tuples map the name of the first element to the name of the second.
     Single types map the name of first element to it's fqn.
     """
 
     builtin_list = [
         AgentMachine,
         # security manager
-        SecurityManager,
+        (SecurityManager, SecurityManagerImpl),
+        SecurityManagerImpl,
         (AuthenticationProcessor, NoopAuthProcessor),
         NoopAuthProcessor,
         GoogleJWTProcessor,
         AzureJWTProcessor,
         (ProcessAuthorizer, PrivateAuthorizer),
         PrivateAuthorizer,
         (FunctionalAuthorizer, NoopFunctionalAuth),
@@ -120,16 +122,16 @@
         ("Agent", SimpleAgent),
         SimpleAgent,
         GenericAgent,  # deprecated
         TreeOfThoughtsAgent,
         RetrieverAgent,
         AutonomousSpeechAgent,
         # cpu
-        (AgentCPU, ConversationalAgentCPU),
-        ConversationalAgentCPU,
+        (APU, ConversationalAPU),
+        ConversationalAPU,
         # cpu components
         IOUnit,
         (LLMUnit, OpenAIGPT),
         OpenAIGPT,
         MistralGPT,
         AnthropicLLMUnit,
         (MemoryUnit, RawMemoryUnit),
@@ -141,15 +143,16 @@
         # machine components
         (SymbolicMemory, MongoSymbolicMemory),
         MongoSymbolicMemory,
         LocalSymbolicMemory,
         (FileMemory, LocalFileMemory),
         LocalFileMemory,
         S3FileMemory,
-        SimilarityMemory,
+        (SimilarityMemory, SimilarityMemoryImpl),
+        SimilarityMemoryImpl,
         (Embedding, OpenAIEmbedding),
         NoopEmbedding,
         OpenAIEmbedding,
         (VectorStore, ChromaVectorStore),
         NoopVectorStore,
         ChromaVectorStore,
         # middleware
@@ -161,32 +164,36 @@
         (SpanExporter, NoopSpanExporter),
         NoopSpanExporter,
         OTLPSpanExporter,
         (Sampler, CustomSampler),
         CustomSampler,
         (SpanProcessor, BatchSpanProcessor),
         BatchSpanProcessor,
-        ProcessFileSystem,
+        (ProcessFileSystem, ProcessFileSystemImpl),
+        ProcessFileSystemImpl,
         # sub components
         (DocumentParser, AutoParser),
         AutoParser,
         (DocumentTransformer, AutoTransformer),
         AutoTransformer,
         (ThoughtGenerationStrategy, ProposePromptStrategy),
         ProposePromptStrategy,
         (QuestionTransformer, MultiQuestionTransformer),
         MultiQuestionTransformer,
         (DocumentReranker, RAGFusionReranker),
         RAGFusionReranker,
         (DocumentLoader, FilesystemLoader),
+        DocumentProcessor,
         DocumentManager,
         FilesystemLoader,
         GitHubLoader,
         ToTChecker,
         OpenAiSpeech,
         AsyncOpenAI,
         AsyncAzureOpenAI,
         UsageClient,
+        OpenAIConnectionHandler,
+        AzureOpenAIConnectionHandler,
         # config objects
         ReplayConfig,
     ]
     return [_to_resource(maybe_tuple) for maybe_tuple in builtin_list if maybe_tuple]
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/components/opentelemetry.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/components/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/components/usage.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/components/usage.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/builtins/logic_units/web_search.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/logic_units/web_search.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/agent_call_history.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/agent_call_history.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/agent_cpu.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/agent_cpu.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,29 +7,44 @@
 
 from eidolon_ai_sdk.cpu.agent_io import CPUMessageTypes
 from eidolon_ai_sdk.cpu.call_context import CallContext
 from eidolon_ai_client.events import StreamEvent, convert_output_object, ObjectOutputEvent, ErrorEvent, StringOutputEvent
 from eidolon_ai_sdk.system.reference_model import Specable
 
 
-class AgentCPUSpec(BaseModel):
+class APUCapabilities(BaseModel):
+    input_context_limit: int
+    output_context_limit: int
+    supports_tools: bool
+    supports_image_input: bool
+    supports_audio_input: bool
+    supports_file_search: bool
+    supports_image_generation: bool
+    supports_audio_generation: bool
+
+
+class APUSpec(BaseModel):
     max_num_function_calls: int = Field(
         10,
         description="The maximum number of function calls to make in a single request.",
     )
 
 
-class AgentCPU(Specable[AgentCPUSpec], ABC):
+class APU(Specable[APUSpec], ABC):
     title: str
 
     def __init__(self, spec: T, **kwargs: object):
         super().__init__(spec, **kwargs)
         self.title = "default"
 
     @abstractmethod
+    def get_capabilities(self) -> APUCapabilities:
+        pass
+
+    @abstractmethod
     async def set_boot_messages(self, call_context: CallContext, boot_messages: List[CPUMessageTypes]):
         pass
 
     @abstractmethod
     async def schedule_request(
         self,
         call_context: CallContext,
@@ -60,17 +75,17 @@
 
 
 T = TypeVar("T")
 
 
 class Thread:
     _call_context: CallContext
-    _cpu: AgentCPU
+    _cpu: APU
 
-    def __init__(self, call_context: CallContext, cpu: AgentCPU):
+    def __init__(self, call_context: CallContext, cpu: APU):
         self._call_context = call_context
         self._cpu = cpu
 
     async def set_boot_messages(
         self,
         prompts: List[CPUMessageTypes],
     ):
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/agent_io.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/agent_io.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,91 +1,78 @@
 from __future__ import annotations
 
 import asyncio
-import uuid
 from abc import abstractmethod, ABC
-from io import IOBase
 from typing import List, Any, Dict, Literal
 
 from pydantic import BaseModel
 
+from eidolon_ai_client.events import FileHandle
 from eidolon_ai_sdk.agent_os import AgentOS
 from eidolon_ai_sdk.cpu.call_context import CallContext
 from eidolon_ai_sdk.cpu.llm_message import (
     UserMessageText,
     SystemMessage,
-    UserMessageImageURL,
     UserMessage,
-    LLMMessage,
+    LLMMessage, UserMessageFileHandle,
 )
 from eidolon_ai_sdk.cpu.processing_unit import ProcessingUnit
-from eidolon_ai_sdk.memory.file_memory import FileMemory
 
 
 class ResponseHandler(ABC):
     @abstractmethod
     async def handle(self, process_id: str, response: Dict[str, Any]):
         pass
 
 
-class CPUMessage(BaseModel):
+class APUMessage(BaseModel):
     type: str
-    prompt: str
-    is_boot_prompt: bool = False
 
 
-class UserTextCPUMessage(CPUMessage):
+class UserTextAPUMessage(APUMessage):
     type: Literal["user"] = "user"
+    prompt: str
+    is_boot_prompt: bool = False
 
 
-class SystemCPUMessage(CPUMessage):
+class SystemAPUMessage(APUMessage):
     type: Literal["system"] = "system"
     is_boot_prompt: bool = True
+    prompt: str
 
 
-class ImageCPUMessage(CPUMessage):
-    type: Literal["image_url"] = "image"
-    image: IOBase
-
-    class Config:
-        arbitrary_types_allowed = True
+class AttachedFileMessage(APUMessage):
+    type: Literal["image_url"] = "file"
+    file: FileHandle
+    include_directly: bool
 
 
-CPUMessageTypes = UserTextCPUMessage | SystemCPUMessage | ImageCPUMessage
+CPUMessageTypes = UserTextAPUMessage | SystemAPUMessage | AttachedFileMessage
 
 
 class IOUnit(ProcessingUnit):
     async def process_request(self, call_context: CallContext, prompts: List[CPUMessageTypes]) -> List[LLMMessage]:
         # convert the prompts to a list of strings
         conv_messages = []
         user_message_parts = []
         for prompt in prompts:
             if prompt.type == "user":
                 user_message_parts.append(UserMessageText(text=prompt.prompt))
             elif prompt.type == "system":
                 conv_messages.append(SystemMessage(content=prompt.prompt))
-            elif prompt.type == "image":
-                file_memory = AgentOS.file_memory
-                image_file: IOBase = prompt.image
-                # read the prompt.image file into memory
-                image_data = image_file.read()
-                base_loc = f"uploaded_images/{call_context.process_id}/{call_context.thread_id or 'main'}"
-                tmp_path = f"{base_loc}/{uuid.uuid4()}"
-                await file_memory.mkdir(base_loc, exist_ok=True)
-                await file_memory.write_file(tmp_path, image_data)
-                user_message_parts.append(UserMessageImageURL(image_url=tmp_path))
+            elif prompt.type == "file":
+                user_message_parts.append(await UserMessageFileHandle.create(file=prompt.file, process_id=call_context.process_id, include_directly=prompt.include_directly))
             else:
                 raise ValueError(f"Unknown prompt type {prompt.type}")
 
         if len(user_message_parts) > 0:
             conv_messages.append(UserMessage(content=user_message_parts))
 
         return conv_messages
 
     async def process_response(self, call_context: CallContext, response: Any):
         return response
 
     @classmethod
     async def delete_process(cls, process_id: str):
-        memory: FileMemory = AgentOS.file_memory
-        found = await memory.glob(f"uploaded_images/{process_id}/**/*")
-        await asyncio.gather(*[memory.delete_file(file) for file in found])
+        found = await AgentOS.file_memory.glob(f"uploaded_images/{process_id}/**/*")
+        await asyncio.gather(*[AgentOS.file_memory.delete_file(file) for file in found])
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/agents_logic_unit.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/agents_logic_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/conversation_memory_unit.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/conversation_memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from io import BytesIO
 from typing import List, Optional, Union, Literal, Dict, Any, AsyncIterator
 
 import yaml
 from PIL import Image
 from anthropic import AsyncAnthropic, APIConnectionError, RateLimitError, APIStatusError
 from fastapi import HTTPException
-from pydantic import Field, BaseModel
+from pydantic import Field
 
 from eidolon_ai_client.events import (
     StringOutputEvent,
     ObjectOutputEvent,
     ToolCall,
 )
 from eidolon_ai_client.util.logger import logger as eidolon_logger
@@ -21,15 +21,15 @@
 from eidolon_ai_sdk.cpu.llm_message import (
     LLMMessage,
     AssistantMessage,
     ToolResponseMessage,
     UserMessage,
     SystemMessage,
 )
-from eidolon_ai_sdk.cpu.llm_unit import LLMUnit, LLMCallFunction
+from eidolon_ai_sdk.cpu.llm_unit import LLMUnit, LLMCallFunction, LLMModel, LLMUnitSpec
 from eidolon_ai_sdk.system.reference_model import Specable
 from eidolon_ai_sdk.util.replay import replayable
 
 logger = eidolon_logger.getChild("llm_unit")
 
 
 def scale_dimensions(width, height, max_size=2048, min_size=768):
@@ -121,32 +121,65 @@
             "tool_call_id": message.tool_call_id,
             "content": json.dumps(message.result),
         }
     else:
         raise ValueError(f"Unknown message type {message.type}")
 
 
-class AnthropicLLMUnitSpec(BaseModel):
+class AnthropicLLMUnitSpec(LLMUnitSpec):
     model: str = Field(default="claude-3-opus-20240229", description="The model to use for the LLM.")
     temperature: float = 0.3
     max_tokens: Optional[int] = None
     client_args: dict = {}
 
 
 class AnthropicLLMUnit(LLMUnit, Specable[AnthropicLLMUnitSpec]):
-    model: str
     temperature: float
 
     def __init__(self, **kwargs):
+        super().__init__(**kwargs)
         LLMUnit.__init__(self, **kwargs)
         Specable.__init__(self, **kwargs)
 
-        self.model = self.spec.model
         self.temperature = self.spec.temperature
 
+    def get_models(self) -> List[LLMModel]:
+        if self.spec.supported_models:
+            return self.spec.supported_models
+
+        return [
+            LLMModel(
+                human_name="Claude Opus",
+                name="claude-3-opus-20240229",
+                input_context_limit=200000,
+                output_context_limit=4096,
+                supports_tools=False,
+                supports_image_input=True,
+                supports_audio_input=False,
+            ),
+            LLMModel(
+                human_name="Claude Sonnet",
+                name="claude-3-sonnet-20240229",
+                input_context_limit=200000,
+                output_context_limit=4096,
+                supports_tools=False,
+                supports_image_input=True,
+                supports_audio_input=False,
+            ),
+            LLMModel(
+                human_name="Claude Haiku",
+                name="claude-3-haiku-20240307",
+                input_context_limit=200000,
+                output_context_limit=4096,
+                supports_tools=False,
+                supports_image_input=True,
+                supports_audio_input=False,
+            )
+        ]
+
     async def execute_llm(
             self,
             call_context: CallContext,
             messages: List[LLMMessage],
             tools: List[LLMCallFunction],
             output_format: Union[Literal["str"], Dict[str, Any]],
     ) -> AsyncIterator[AssistantMessage]:
@@ -189,15 +222,15 @@
     async def _build_request(self, inMessages, inTools, output_format):
         # tools = await self._build_tools(inTools)
         tools = []
         system_prompt = "\n".join([message.content for message in inMessages if isinstance(message, SystemMessage)])
         messages = [await convert_to_llm(message) for message in inMessages if not isinstance(message, SystemMessage)]
         request = {
             "messages": messages,
-            "model": self.model,
+            "model": self.model.name,
             "temperature": self.temperature,
         }
         if system_prompt:
             request["system"] = system_prompt
 
         if output_format == "str" or output_format["type"] == "string":
             is_string = True
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import json
 import logging
-from enum import Enum
 from io import BytesIO
 from typing import List, Optional, Union, Literal, Dict, Any, AsyncIterator, cast
 
 import yaml
 from PIL import Image
 from fastapi import HTTPException
 from mistralai.async_client import MistralAsyncClient
 from mistralai.exceptions import MistralConnectionException, MistralAPIStatusException, MistralAPIException
 from mistralai.models.chat_completion import ChatCompletionStreamResponse, ResponseFormat, ResponseFormats, Function
-from pydantic import Field, BaseModel
+from pydantic import Field
 
 from eidolon_ai_client.events import (
     StringOutputEvent,
     ObjectOutputEvent,
     LLMToolCallRequestEvent,
     ToolCall,
 )
@@ -23,15 +22,15 @@
 from eidolon_ai_sdk.cpu.llm_message import (
     LLMMessage,
     AssistantMessage,
     ToolResponseMessage,
     UserMessage,
     SystemMessage,
 )
-from eidolon_ai_sdk.cpu.llm_unit import LLMUnit, LLMCallFunction
+from eidolon_ai_sdk.cpu.llm_unit import LLMUnit, LLMCallFunction, LLMModel, LLMUnitSpec
 from eidolon_ai_sdk.system.reference_model import Specable
 from eidolon_ai_sdk.util.replay import replayable
 
 logger = eidolon_logger.getChild("llm_unit")
 
 
 def scale_dimensions(width, height, max_size=2048, min_size=768):
@@ -113,34 +112,62 @@
             "tool_call_id": message.tool_call_id,
             "content": json.dumps(message.result),
         }
     else:
         raise ValueError(f"Unknown message type {message.type}")
 
 
-class MistralModelEnum(str, Enum):
-    MistralTiny = "mistral-tiny-latest"
-    MistralSmall = "mistral-small-latest"
-    MistralMedium = "mistral-medium-latest"
-    MistralLarge = "mistral-large-latest"
-
-
-class MistralGPTSpec(BaseModel):
-    model: MistralModelEnum = Field(default=MistralModelEnum.MistralMedium, description="The model to use for the LLM.")
+class MistralGPTSpec(LLMUnitSpec):
+    model: str = Field(default="mistral-large-latest", description="The model to use for the LLM.")
     temperature: float = 0.3
     force_json: bool = True
     max_tokens: Optional[int] = None
     client_args: dict = {}
 
 
 class MistralGPT(LLMUnit, Specable[MistralGPTSpec]):
     def __init__(self, **kwargs):
+        super().__init__(**kwargs)
         LLMUnit.__init__(self, **kwargs)
         Specable.__init__(self, **kwargs)
 
+    def get_models(self) -> List[LLMModel]:
+        if self.spec.supported_models:
+            return self.spec.supported_models
+
+        return [
+            LLMModel(
+                human_name="Mistral Large",
+                name="mistral-large-latest",
+                input_context_limit=32000,
+                output_context_limit=4096,
+                supports_tools=True,
+                supports_image_input=False,
+                supports_audio_input=False,
+            ),
+            LLMModel(
+                human_name="Mistral Medium",
+                name="mistral-medium-latest",
+                input_context_limit=32000,
+                output_context_limit=4096,
+                supports_tools=False,
+                supports_image_input=False,
+                supports_audio_input=False,
+            ),
+            LLMModel(
+                human_name="Mistral Small",
+                name="mistral-small-latest",
+                input_context_limit=32000,
+                output_context_limit=4096,
+                supports_tools=False,
+                supports_image_input=False,
+                supports_audio_input=False,
+            )
+        ]
+
     async def execute_llm(
             self,
             call_context: CallContext,
             messages: List[LLMMessage],
             tools: List[LLMCallFunction],
             output_format: Union[Literal["str"], Dict[str, Any]],
     ) -> AsyncIterator[AssistantMessage]:
@@ -209,15 +236,15 @@
             raise HTTPException(502, f"Mistral Error: {e.message}") from e
 
     async def _build_request(self, inMessages, inTools, output_format):
         tools = await self._build_tools(inTools)
         messages = [await convert_to_mistral(message) for message in inMessages]
         request = {
             "messages": messages,
-            "model": str(self.spec.model.value),
+            "model": str(self.model.name),
             "temperature": self.spec.temperature,
         }
         if output_format == "str" or output_format["type"] == "string":
             is_string = True
         else:
             is_string = False
             force_json_msg = (
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/llm/open_ai_speech.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm/open_ai_speech.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Optional, Literal
 
 from openai import AsyncOpenAI
-from pydantic import Field, BaseModel
+from pydantic import Field
 
+from eidolon_ai_sdk.cpu.audio_unit import AudioUnit, AudioUnitSpec
 from eidolon_ai_sdk.system.reference_model import Specable
 
 
-class OpenAiSpeechSpec(BaseModel):
+class OpenAiSpeechSpec(AudioUnitSpec):
     text_to_speech_model: Literal["tts-1", "tts-1-hd"] = Field(
         default="tts-1-hd", description="The model to use for text to speech."
     )
     text_to_speech_voice: Literal["alloy", "echo", "fable", "onyx", "nova", "shimmer"] = Field(
         default="alloy", description="The voice to use for text to speech."
     )
     speech_to_text_model: Literal["whisper-1"] = Field(
@@ -18,31 +19,33 @@
     )
     speech_to_text_temperature: float = Field(
         default=0.3,
         description="The sampling temperature, between 0 and 1. Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic. If set to 0, the model will use log probability to automatically increase the temperature until certain thresholds are hit.",
     )
 
 
-class OpenAiSpeech(Specable[OpenAiSpeechSpec]):
+class OpenAiSpeech(AudioUnit, Specable[OpenAiSpeechSpec]):
     model: str
     temperature: float
     llm: AsyncOpenAI = None
 
     def __init__(self, spec: OpenAiSpeechSpec, **kwargs):
         super().__init__(spec, **kwargs)
+        Specable.__init__(self, spec, **kwargs)
 
     async def text_to_speech(self, text: str, response_format: str = "mp3") -> bytes:
         """
         Converts text to speech.
 
         Args:
             text (str): The text to convert to speech.
 
         Returns:
             bytes: The audio data.
+            :param text:
             :param response_format: Response audio format. Legal values are ["mp3", "opus", "aac", "flac", "wav", "pcm"].  Defaults to "mp3".
         """
         if not self.llm:
             self.llm = AsyncOpenAI()
 
         response = await self.llm.audio.speech.create(
             model=self.spec.text_to_speech_model,
@@ -61,14 +64,18 @@
 
         Args:
             audio (bytes): The audio data.
             prompt (Optional[str], optional): An optional text to guide the model's style or continue a previous audio segment. Defaults to None.
             language (Optional[str], optional): The language of the input audio. Supplying the input language in ISO-639-1 format will improve accuracy and latency.
         Returns:
             str: The text.
+            :param audio:
+            :param language:
+            :param prompt:
+            :param mime_type:
         """
         if not self.llm:
             self.llm = AsyncOpenAI()
         request = {
             "file": ("audio", audio, mime_type),
             "model": self.spec.speech_to_text_model,
             "temperature": self.spec.speech_to_text_temperature,
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/logic_unit.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/logic_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/memory_unit.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/cpu/processing_unit.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/processing_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/chroma_vector_store.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/chroma_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/document.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/document.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/embeddings.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/file_system_vector_store.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/file_system_vector_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import abstractmethod
-from pydantic import Field, BaseModel
 from typing import List, Dict, Optional, Sequence, Any, Iterable
 
+from pydantic import Field, BaseModel
+
 from eidolon_ai_sdk.agent_os import AgentOS
 from eidolon_ai_sdk.memory.document import Document, EmbeddedDocument
 from eidolon_ai_sdk.memory.vector_store import QueryItem, VectorStore
 from eidolon_ai_sdk.system.reference_model import Specable
 
 
 class FileSystemVectorStoreSpec(BaseModel):
@@ -49,15 +50,15 @@
     ) -> List[QueryItem]:
         pass
 
     async def add(self, collection: str, docs: Sequence[Document]):
         await AgentOS.file_memory.mkdir(self.spec.root_document_directory + "/" + collection, exist_ok=True)
         # Asynchronously collect embedded documents
         embeddedDocs = []
-        async for embeddedDoc in AgentOS.similarity_memory.embedder.embed(docs):
+        async for embeddedDoc in AgentOS.similarity_memory.embed(docs):
             embeddedDocs.append(embeddedDoc)
         await self.add_embedding(collection, embeddedDocs)
         for doc in docs:
             await AgentOS.file_memory.write_file(
                 self.spec.root_document_directory + "/" + collection + "/" + doc.id,
                 doc.page_content.encode(),
             )
@@ -70,15 +71,15 @@
     async def query(
         self,
         collection: str,
         query: str,
         num_results: int,
         metadata_where: Optional[Dict[str, str]] = None,
     ) -> List[Document]:
-        text = await AgentOS.similarity_memory.embedder.embed_text(query)
+        text = await AgentOS.similarity_memory.embed_text(query)
         results = await self.query_embedding(collection, text, num_results, metadata_where, False)
         returnDocuments = []
         for result in results:
             returnDocuments.append(
                 Document(
                     id=result.id,
                     metadata=result.metadata,
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/in_memory_file_memory.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/in_memory_file_memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from pathlib import Path
 
 from pydantic import Field, BaseModel
 
-from eidolon_ai_sdk.memory.file_memory import FileMemory
+from eidolon_ai_sdk.memory.file_memory import FileMemoryBase
 from eidolon_ai_sdk.system.reference_model import Specable
 
 
 class InMemoryFileMemoryConfig(BaseModel):
     pass
 
 
-class InMemoryFileMemory(FileMemory, Specable[InMemoryFileMemoryConfig]):
+class InMemoryFileMemory(FileMemoryBase, Specable[InMemoryFileMemoryConfig]):
     def __init__(self, spec: InMemoryFileMemoryConfig):
         super().__init__(spec)
         self.root_dir = Path("/").resolve()
         self.files = {}
         self.spec = spec
 
     """
@@ -103,14 +103,17 @@
         safe_file_path = self.resolve(file_name)
 
         print(f"Checking if {safe_file_path} exists")
         print(f"Files: {self.files}")
         # Check if the file exists
         return self.files.get(safe_file_path) is not None
 
+    async def glob(self, pattern: str):
+        pass
+
     async def start(self):
         """
         Starts the memory implementation. Noop for this implementation.
         """
         pass
 
     async def stop(self):
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/local_file_memory.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/local_file_memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import glob
 from pathlib import Path
 
 from pydantic import Field, field_validator, BaseModel
 
-from eidolon_ai_sdk.memory.file_memory import FileMemory
+from eidolon_ai_sdk.memory.file_memory import FileMemoryBase
 from eidolon_ai_sdk.system.reference_model import Specable
 from eidolon_ai_sdk.util.async_wrapper import make_async
 from eidolon_ai_client.util.logger import logger
 from eidolon_ai_sdk.util.str_utils import replace_env_var_in_string
 
 
 class LocalFileMemoryConfig(BaseModel):
@@ -30,15 +30,15 @@
         # You could also check if path exists and is a directory if necessary
         if path.is_file():
             raise ValueError(f"The root_dir must be a directory. Received: {inValue}->{value}")
 
         return inValue
 
 
-class LocalFileMemory(FileMemory, Specable[LocalFileMemoryConfig]):
+class LocalFileMemory(FileMemoryBase, Specable[LocalFileMemoryConfig]):
     def __init__(self, spec: LocalFileMemoryConfig):
         super().__init__(spec)
         self.root_dir = Path(replace_env_var_in_string(spec.root_dir)).resolve()
 
     """
     A FileMemory implementation that stores files on the local filesystem.
     """
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/local_symbolic_memory.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/local_symbolic_memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from copy import deepcopy
 from typing import Any, Union, List, Dict, AsyncIterable, Optional
 
 from bson import ObjectId
 from pymongo.errors import DuplicateKeyError
 
-from eidolon_ai_sdk.memory.semantic_memory import SymbolicMemory
+from eidolon_ai_sdk.memory.semantic_memory import SymbolicMemoryBase
 
 
-class LocalSymbolicMemory(SymbolicMemory):
+class LocalSymbolicMemory(SymbolicMemoryBase):
     db = {}
 
     async def start(self):
         LocalSymbolicMemory.db = {}
 
     async def stop(self):
         LocalSymbolicMemory.db = {}
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/mongo_symbolic_memory.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/mongo_symbolic_memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 # noinspection PyPackageRequirements
 from contextvars import ContextVar
 from typing import Any, Optional, AsyncIterable, Union, Dict, List
 
 from motor.motor_asyncio import AsyncIOMotorDatabase, AsyncIOMotorClient
 from pydantic import Field, BaseModel
 
-from eidolon_ai_sdk.memory.semantic_memory import SymbolicMemory
+from eidolon_ai_sdk.memory.semantic_memory import SymbolicMemoryBase
 from eidolon_ai_sdk.system.reference_model import Specable
 
 
 class MongoSymbolicMemoryConfig(BaseModel):
     mongo_connection_string: str = Field(
         default=os.environ.get("MONGO_CONNECTION_STR", "mongodb://localhost:27017/?directConnection=true"), description="The connection string to the MongoDB instance."
     )
     mongo_database_name: str = Field(default=os.environ.get("MONGO_DATABASE_NAME", "eidolon"), description="The name of the MongoDB database to use.")
 
 
-class MongoSymbolicMemory(SymbolicMemory, Specable[MongoSymbolicMemoryConfig]):
+class MongoSymbolicMemory(SymbolicMemoryBase, Specable[MongoSymbolicMemoryConfig]):
     mongo_connection_string: Optional[str]
     mongo_database_name: str
     _database: Optional[ContextVar]
 
     def __init__(self, spec: MongoSymbolicMemoryConfig):
         super().__init__(spec)
         self.mongo_connection_string = spec.mongo_connection_string
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/noop_memory.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/noop_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/s3_file_memory.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/s3_file_memory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import fnmatch
 from io import BytesIO
 
 import boto3
 from pydantic import BaseModel
 
-from eidolon_ai_sdk.memory.file_memory import FileMemory
+from eidolon_ai_sdk.memory.file_memory import FileMemoryBase
 from eidolon_ai_sdk.util.async_wrapper import make_async
 
 
-class S3FileMemory(BaseModel, FileMemory):
+class S3FileMemory(BaseModel, FileMemoryBase):
     bucket: str
     region: str = "us-east-1"
     kwargs: dict = {}
     create_bucket_on_startup: bool = False
     _client = None
 
     def __init__(self, **kwargs):
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/memory/vector_store.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/authentication_processor.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/authentication_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/azure_authorizer.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/azure_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/functional_authorizer.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/functional_authorizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import fnmatch
 from abc import abstractmethod
 from typing import Set
 
-from eidolon_ai_sdk.security.permissions import Permission, PermissionException
+from eidolon_ai_sdk.security.permissions import PermissionException
+from eidolon_ai_sdk.agent_os_interfaces import Permission
 from eidolon_ai_sdk.security.user import User
 
 
 class FunctionalAuthorizer:
     @abstractmethod
     async def check_functional_perms(self, permissions: Set[Permission], target):
         pass
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/google_auth.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/google_auth.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/jwt_processor.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/jwt_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/permissions.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/permissions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from __future__ import annotations
 
-from typing import Set, Optional, Literal
+from typing import Set, Optional
 
 from starlette.requests import Request
 from starlette.responses import JSONResponse
 
 from eidolon_ai_client.util.logger import logger
+from eidolon_ai_sdk.agent_os_interfaces import Permission
 
 
 class PermissionException(Exception):
     missing: Set[Permission]
     process: Optional[str]
 
     def __init__(self, missing: Permission | Set[Permission], process: Optional[str] = None):
         self.missing = {missing} if isinstance(missing, str) else missing
         self.process = process
         reason = "Missing Resource Permission: " if process else "Missing Permission: "
         super().__init__(reason + ", ".join(self.missing))
 
 
-Permission = Literal["create", "read", "update", "delete"]  # probably expands to include concept of know
-
-
 def permission_exception_handler(request: Request, exc: PermissionException):
     logger.warning(str(exc))
     if "read" in exc.missing and exc.process:
         return JSONResponse(status_code=404, content={"detail": "Process Not Found"})
     return JSONResponse(status_code=403, content={"detail": str(exc)})
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/process_authorizer.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/process_authorizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import Set, List
 
 from eidolon_ai_sdk.agent_os import AgentOS
-from eidolon_ai_sdk.security.permissions import Permission, PermissionException
+from eidolon_ai_sdk.security.permissions import PermissionException
+from eidolon_ai_sdk.agent_os_interfaces import Permission
 from eidolon_ai_sdk.security.user import User
 from eidolon_ai_sdk.system.processes import MongoDoc
 
 
 class ProcessAuthorizer(ABC):
     @abstractmethod
     async def check_process_perms(self, permissions: Set[Permission], agent: str, process_id: str):
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/security_manager.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/security_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from __future__ import annotations
 
 from typing import Optional, Set
 
 from pydantic import BaseModel
+from starlette.requests import Request
 
 from eidolon_ai_sdk.security.authentication_processor import AuthenticationProcessor
 from eidolon_ai_sdk.security.functional_authorizer import FunctionalAuthorizer
-from eidolon_ai_sdk.security.permissions import Permission
+from eidolon_ai_sdk.agent_os_interfaces import Permission, SecurityManager
 from eidolon_ai_sdk.security.process_authorizer import ProcessAuthorizer
+from eidolon_ai_sdk.security.user import User
 from eidolon_ai_sdk.system.reference_model import Specable, AnnotatedReference
 
 
 class SecurityManagerSpec(BaseModel):
     authentication_processor: AnnotatedReference[AuthenticationProcessor]
     functional_authorizer: AnnotatedReference[FunctionalAuthorizer]
     process_authorizer: AnnotatedReference[ProcessAuthorizer]
 
     safe_paths: Set[str] = {"/system/health", "/docs", "/favicon.ico", "/openapi.json"}
 
 
-class SecurityManager(Specable[SecurityManagerSpec]):
+class SecurityManagerImpl(Specable[SecurityManagerSpec], SecurityManager):
     authentication_processor: AuthenticationProcessor
     functional_authorizer: FunctionalAuthorizer
     process_authorizer: ProcessAuthorizer
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.authentication_processor = self.spec.authentication_processor.instantiate()
@@ -33,7 +35,29 @@
     async def check_permissions(
         self, permissions: Permission | Set[Permission], agent: str, process_id: Optional[str] = None
     ):
         permissions = {permissions} if isinstance(permissions, str) else permissions
         await self.functional_authorizer.check_functional_perms(permissions, f"agents/{agent}/processes")
         if process_id:
             await self.process_authorizer.check_process_perms(permissions, agent, process_id)
+
+    async def check_auth(self, request: Request) -> User:
+        """
+        Check the request for expected authentication and stores information in context as needed for authorization.
+
+        :return User: the authenticated user
+        :raises HTTPException: if the request is not authenticated
+        """
+        return await self.authentication_processor.check_auth(request)
+
+    async def check_process_perms(self, permissions: Set[Permission], agent: str, process_id: str):
+        """
+        Checks if the authenticated user has the specified permission(s) to the provided agent process.
+        :raises PermissionException: If the agent does not have the required permissions.
+        """
+        return await self.process_authorizer.check_process_perms(permissions, agent, process_id)
+
+    async def record_process(self, agent: str, resource_id: str):
+        """
+        Called when a process is created. Should propagate any state needed for future resource checks.
+        """
+        return await self.process_authorizer.record_process(agent, resource_id)
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/security/security_middleware.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/security_middleware.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from fastapi import HTTPException
 from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
 from starlette.requests import Request
 from starlette.responses import Response, JSONResponse
 
 from eidolon_ai_client.util.logger import logger
 from eidolon_ai_sdk.agent_os import AgentOS
-from eidolon_ai_sdk.security.security_manager import SecurityManager
+from eidolon_ai_sdk.security.security_manager import SecurityManagerImpl
 from eidolon_ai_sdk.security.user import User
 
 
 class SecurityMiddleware(BaseHTTPMiddleware):
     async def dispatch(self, request: Request, call_next: RequestResponseEndpoint) -> Response:
-        security: SecurityManager = AgentOS.security_manager
+        security: SecurityManagerImpl = AgentOS.security_manager
         if request.url.path not in security.spec.safe_paths:
             try:
-                user = await security.authentication_processor.check_auth(request)
+                user = await security.check_auth(request)
                 User.set_current(user)
             except HTTPException as e:
                 logger.info(f"Auth Denied: {e.detail}")
                 return JSONResponse(status_code=e.status_code, content={"detail": e.detail})
         return await call_next(request)
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/agent_contract.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/agent_contract.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/agent_controller.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/agent_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     CanceledEvent,
 )
 from eidolon_ai_client.util.logger import logger
 from eidolon_ai_client.util.request_context import RequestContext
 from eidolon_ai_sdk.agent.agent import AgentState
 from eidolon_ai_sdk.agent_os import AgentOS
 from eidolon_ai_sdk.cpu.agent_call_history import AgentCallHistory
-from eidolon_ai_sdk.security.security_manager import SecurityManager
+from eidolon_ai_sdk.security.security_manager import SecurityManagerImpl
 from eidolon_ai_sdk.system.agent_contract import (
     SyncStateResponse,
     StateSummary,
     DeleteProcessResponse,
 )
 from eidolon_ai_sdk.system.fn_handler import FnHandler, get_handlers
 from eidolon_ai_sdk.system.processes import ProcessDoc, store_events, load_events
@@ -48,15 +48,15 @@
 
 
 # todo, agent controller has become a mega impl, we should break up responsibilities
 class AgentController:
     name: str
     agent: object
     actions: typing.Dict[str, FnHandler]
-    security: SecurityManager
+    security: SecurityManagerImpl
 
     def __init__(self, name, agent):
         self.name = name
         self.actions = {}
         self.agent = agent
         for handler in get_handlers(self.agent):
             if handler.name in self.actions:
@@ -228,15 +228,37 @@
     async def agent_event_stream(self, handler, process, last_state, **kwargs) -> AsyncIterator[StreamEvent]:
         is_async_gen = inspect.isasyncgenfunction(handler.fn)
         stream = handler.fn(self.agent, **kwargs) if is_async_gen else self.stream_agent_fn(handler, **kwargs)
         events_to_store = []
         ended = False
         transitioned = False
         try:
-            async for event in self.stream_agent_iterator(stream, process, handler.name, kwargs):
+            # allow the agent send a custom user input event or a custom start event
+            user_input_event_seen = False
+            start_event_seen = False
+            async for event in self.stream_agent_iterator(stream, process):
+                if event.is_root_and_type(UserInputEvent):
+                    user_input_event_seen = True
+                elif not user_input_event_seen:
+                    user_input_event_seen = True
+                    output_event = UserInputEvent(input=to_jsonable_python(kwargs, fallback=str))
+                    events_to_store.append(output_event)
+                    yield output_event
+                if event.is_root_and_type(StartAgentCallEvent):
+                    start_event_seen = True
+                elif not start_event_seen and not event.is_root_and_type(UserInputEvent):
+                    start_event_seen = True
+                    output_event = StartAgentCallEvent(
+                        machine=AgentOS.current_machine_url(),
+                        agent_name=self.name,
+                        call_name=handler.name,
+                        process_id=process.record_id,
+                    )
+                    events_to_store.append(output_event)
+                    yield output_event
                 if not ended:
                     ended = event.is_root_end_event()
                     transitioned = event.is_root_and_type(AgentStateEvent)
                     if (
                         isinstance(event, StringOutputEvent)
                         and events_to_store
                         and isinstance(events_to_store[-1], StringOutputEvent)
@@ -264,28 +286,19 @@
             latest_record = await self.get_latest_process_event(process.record_id)
             if latest_record.delete_on_terminate and latest_record.state == "terminated":
                 await self._delete_process(process.record_id)
 
     async def stream_agent_iterator(
         self,
         stream: AsyncIterator[StreamEvent],
-        process: ProcessDoc,
-        call_name,
-        user_input: typing.Dict[str, typing.Any],
+        process: ProcessDoc
     ) -> AsyncIterator[StreamEvent]:
         state_change = None
         seen_end = False
         try:
-            yield UserInputEvent(input=to_jsonable_python(user_input, fallback=str))
-            yield StartAgentCallEvent(
-                machine=AgentOS.current_machine_url(),
-                agent_name=self.name,
-                call_name=call_name,
-                process_id=process.record_id,
-            )
             async for event in stream:
                 if event.is_root_and_type(ErrorEvent):
                     logger.warning("Error event received")
                 if not seen_end:
                     seen_end = event.is_root_end_event()
                     if event.is_root_and_type(AgentStateEvent):
                         state_change = True
@@ -376,15 +389,15 @@
         """
         Create a new process. Use this method first to get a process id before calling any other action
         :param title: An optional title for the process
         :return:
         """
         await self.security.check_permissions({"read", "create"}, self.name)
         process = await self._create_process(state="initialized", title=title)
-        await self.security.process_authorizer.record_process(self.name, process.record_id)
+        await self.security.record_process(self.name, process.record_id)
         return JSONResponse(
             StateSummary(
                 agent=self.name,
                 process_id=process.record_id,
                 state=process.state,
                 available_actions=self.get_available_actions(process.state),
                 title=process.title,
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/agent_machine.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/agent_machine.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 import typing
 from contextlib import contextmanager
-from fastapi import FastAPI, Request, Body, Header
-from pydantic import BaseModel, Field
 from typing import List, Optional, Annotated, Literal, cast
 
+from fastapi import FastAPI, Request, Body, Header
+from pydantic import BaseModel, Field
 from starlette.responses import JSONResponse, Response
 
 from eidolon_ai_client.client import ProcessStatus
+from eidolon_ai_client.events import FileHandle
 from eidolon_ai_client.util.logger import logger
+from eidolon_ai_sdk.agent_os_interfaces import FileMemory, SymbolicMemory, SimilarityMemory, SecurityManager
 from eidolon_ai_sdk.memory.agent_memory import AgentMemory
 from .agent_contract import StateSummary, CreateProcessArgs, DeleteProcessResponse, ListProcessesResponse
 from .agent_controller import AgentController
+from .process_file_system import ProcessFileSystem
 from .processes import ProcessDoc
 from .reference_model import AnnotatedReference, Specable
 from .resources.agent_resource import AgentResource
 from .resources.resources_base import Resource
 from ..agent_os import AgentOS
 from ..cpu.agent_call_history import AgentCallHistory
-from ..memory.file_memory import FileMemory
-from ..memory.semantic_memory import SymbolicMemory
-from ..memory.similarity_memory import SimilarityMemory
 from ..security.permissions import PermissionException
-from eidolon_ai_sdk.system.process_file_system import ProcessFileSystem
-from ..security.security_manager import SecurityManager
 
 
 class MachineSpec(BaseModel):
     symbolic_memory: AnnotatedReference[SymbolicMemory] = Field(description="The Symbolic Memory implementation.")
     file_memory: AnnotatedReference[FileMemory] = Field(desciption="The File Memory implementation.")
     similarity_memory: AnnotatedReference[SimilarityMemory] = Field(description="The Vector Memory implementation.")
     security_manager: AnnotatedReference[SecurityManager] = Field(description="The Security Manager implementation.")
@@ -110,27 +108,35 @@
         )
 
         # Add routes for the process filesystem
         app.add_api_route(
             "/processes/{process_id}/files",
             endpoint=self.upload_file,
             methods=["POST"],
-            response_model=typing.Dict[str, str],
+            response_model=FileHandle,
             tags=["files"],
         )
 
         app.add_api_route(
             "/processes/{process_id}/files/{file_id}",
             endpoint=self.download_file,
             methods=["GET"],
             response_model=bytes,
             tags=["files"],
         )
 
         app.add_api_route(
+            "/processes/{process_id}/files/{file_id}/metadata",
+            endpoint=self.set_metadata,
+            methods=["POST"],
+            response_model=FileHandle,
+            tags=["files"],
+        )
+
+        app.add_api_route(
             "/processes/{process_id}/files/{file_id}",
             endpoint=self._delete_file,
             methods=["DELETE"],
             response_model=None,
             tags=["files"],
         )
 
@@ -166,17 +172,28 @@
         :param process_id:
         :param file_bytes:
         :return: The file id that was written
         """
         file_md = None
         if mime_type:
             file_md = {"mime_type": mime_type}
+        file_id = await self.process_file_system.write_file(process_id, file_bytes, file_md)
+        return JSONResponse(
+            content=file_id.model_dump(), status_code=200
+        )
+
+    async def set_metadata(self, process_id: str, file_id: str, file_md: dict):
+        """
+        Set metadata for a file
+        :param file_id:
+        :param process_id:
+        """
+        file_id = await self.process_file_system.set_metadata(process_id, file_id, file_md)
         return JSONResponse(
-            content={"file_id": await self.process_file_system.write_file(process_id, file_bytes, file_md)},
-            status_code=200,
+            content=file_id.model_dump(), status_code=200
         )
 
     async def download_file(self, process_id: str, file_id: str):
         """
         Download a file for this process
         :param process_id:
         :param file_id:
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/dynamic_middleware.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/dynamic_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/fn_handler.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/fn_handler.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/process_file_system.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/process_file_system.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,32 @@
 import asyncio
 import json
 from pathlib import Path
-from typing import cast, Optional, Dict, Tuple
+from typing import Optional, Dict, Tuple
 from uuid import uuid4
 
 from pydantic import BaseModel
 
+from eidolon_ai_client.events import FileHandle
 from eidolon_ai_sdk.agent_os import AgentOS
-from eidolon_ai_sdk.memory.file_memory import FileMemory
+from eidolon_ai_sdk.agent_os_interfaces import ProcessFileSystem
 from eidolon_ai_sdk.system.reference_model import Specable
 
 
-class FileHandle(BaseModel):
-    machineURL: str
-    process_id: str
-    file_id: str
-
-
 class ProcessFileSystemSpec(BaseModel):
     root: str = "processes"
 
 
-class ProcessFileSystem(Specable[ProcessFileSystemSpec]):
+class ProcessFileSystemImpl(Specable[ProcessFileSystemSpec], ProcessFileSystem):
     root: str
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.root = self.spec.root
 
-    def file_memory(self):
-        return cast(FileMemory, AgentOS.file_memory)
-
     async def start(self):
         """
         Starts the memory implementation.
         """
         pass
 
     async def stop(self):
@@ -47,55 +39,77 @@
         """
         Reads the contents of a file for the given process_id and file_id
         :param process_id:
         :param file_id:
         :return:
         """
         path = str(Path(self.root, process_id, file_id))
-        exists = await self.file_memory().exists(path)
+        exists = await AgentOS.file_memory.exists(path)
         if not exists:
             return None
         file_md = None
-        if await self.file_memory().exists(path + ".md"):
-            file_md = json.loads((await self.file_memory().read_file(path + ".md")).decode())
-        return await self.file_memory().read_file(path), file_md
+        if await AgentOS.file_memory.exists(path + ".md"):
+            file_md = json.loads((await AgentOS.file_memory.read_file(path + ".md")).decode())
+        return await AgentOS.file_memory.read_file(path), file_md
 
-    async def write_file(self, process_id: str, file_contents: bytes, file_md: Optional[Dict[str, any]] = None) -> str:
+    async def write_file(self, process_id: str, file_contents: bytes, file_md: Optional[Dict[str, any]] = None) -> FileHandle:
         """
         Writes the given `file_contents` to a new file within the context of the process_id.
         :param file_md:
         :param process_id:
         :param file_contents:
         :return:
         """
         file_id = uuid4().hex
-        await self.file_memory().mkdir(str(Path(self.root, process_id)), exist_ok=True)
-        await self.file_memory().write_file(str(Path(self.root, process_id, file_id)), file_contents)
+        await AgentOS.file_memory.mkdir(str(Path(self.root, process_id)), exist_ok=True)
+        await AgentOS.file_memory.write_file(str(Path(self.root, process_id, file_id)), file_contents)
         md_to_write = {
             "process_id": process_id,
             "file_id": file_id
         }
         if file_md:
             md_to_write.update(file_md)
         path = str(Path(self.root, process_id, file_id + ".md"))
-        await self.file_memory().write_file(path, json.dumps(md_to_write).encode())
-        return file_id
+        await AgentOS.file_memory.write_file(path, json.dumps(md_to_write).encode())
+        return FileHandle(machineURL=AgentOS.current_machine_url(), process_id=process_id, file_id=file_id, metadata=md_to_write)
+
+    async def set_metadata(self, process_id: str, file_id: str, metadata: Dict[str, any]):
+        """
+        Sets the metadata for the file specified by `file_id` within the context of the process_id.
+        :param process_id:
+        :param file_id:
+        :param metadata:
+        :return:
+        """
+        path = str(Path(self.root, process_id, file_id + ".md"))
+        # read the contents of the metadata file
+        # update the metadata
+        # write the metadata back to the file
+        exists = await AgentOS.file_memory.exists(path)
+        if not exists:
+            file_md = {}
+        else:
+            contents = await AgentOS.file_memory.read_file(path)
+            file_md = json.loads(contents)
+        file_md.update(metadata)
+        await AgentOS.file_memory.write_file(path, json.dumps(file_md).encode())
+        return FileHandle(machineURL=AgentOS.current_machine_url(), process_id=process_id, file_id=file_id, metadata=file_md)
 
     async def delete_file(self, process_id: str, file_id: str):
         """
         Deletes the file specified by `file_id` within the context of the process_id.
         :param process_id:
         :param file_id:
         :return:
         """
         path = str(Path(self.root, process_id, file_id))
-        exists = await self.file_memory().exists(path)
+        exists = await AgentOS.file_memory.exists(path)
         if not exists:
             return None
-        await self.file_memory().delete_file(path)
+        await AgentOS.file_memory.delete_file(path)
         return "deleted"
 
     async def list_files(self, process_id: str, include_only_index: bool):
         path = Path(self.root, process_id)
         files = await AgentOS.file_memory.glob(f"{path}/*.md")
         for file in files:
             contents = await AgentOS.file_memory.read_file(file)
@@ -106,12 +120,11 @@
     @classmethod
     async def delete_process(cls, process_id: str):
         """
         Deletes the entire process directory
         :param process_id:
         :return:
         """
-        memory: FileMemory = AgentOS.file_memory
         pfs: ProcessFileSystem = AgentOS.process_file_system
         process_path = str(Path(pfs.root, process_id))
-        found = await memory.glob(f"{process_path}/**/*")
-        await asyncio.gather(*[memory.delete_file(file) for file in found])
+        found = await AgentOS.file_memory.glob(f"{process_path}/**/*")
+        await asyncio.gather(*[AgentOS.file_memory.delete_file(file) for file in found])
```

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/processes.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/processes.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/reference_model.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/reference_model.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/resources/reference_resource.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/resources/reference_resource.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/system/resources/resources_base.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/resources/resources_base.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/class_utils.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/class_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/replay.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/schema_to_model.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/schema_to_model.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/str_utils.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/str_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/eidolon_ai_sdk/util/stream_collector.py` & `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/stream_collector.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/logging.conf` & `eidolon_ai_sdk-0.1.26/logging.conf`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.25/pyproject.toml` & `eidolon_ai_sdk-0.1.26/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eidolon-ai-sdk"
-version = "0.1.25"
+version = "0.1.26"
 description = "An Open Source Agent Services Framework"
 authors = ["Luke Lalor <lukehlalor@gmail.com>"]
 readme = "README.md"
 include = ["logging.conf"]
 
 [tool.poetry.urls]
 Github = "https://github.com/eidolon-ai/eidolon"
@@ -52,14 +52,15 @@
 opentelemetry-instrumentation-logging = "^0.44b0"
 opentelemetry-sdk = "^1.23.0"
 eidolon-ai-mistralai = "^0.1.6a"
 eidolon-ai-client = "^0.1.5"
 eidolon-ai-usage-client =  "^0.1.0"
 boto3 = "^1.34.74"
 boto3-stubs = {extras = ["essential"], version = "^1.34.74"}
+azure-identity = "^1.16.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.4"
 pylint = "^3.0.3"
 ruff = "^0.1.7"
 pytest-recording = "^0.13.1"
 pytest-asyncio = "^0.23.4"
```

### Comparing `eidolon_ai_sdk-0.1.25/PKG-INFO` & `eidolon_ai_sdk-0.1.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: eidolon-ai-sdk
-Version: 0.1.25
+Version: 0.1.26
 Summary: An Open Source Agent Services Framework
 Author: Luke Lalor
 Author-email: lukehlalor@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anthropic (>=0.21.3,<0.22.0)
 Requires-Dist: authlib (>=1.3.0,<2.0.0)
+Requires-Dist: azure-identity (>=1.16.0,<2.0.0)
 Requires-Dist: boto3 (>=1.34.74,<2.0.0)
 Requires-Dist: boto3-stubs[essential] (>=1.34.74,<2.0.0)
 Requires-Dist: chromadb (>=0.4.18,<0.5.0)
 Requires-Dist: dill (>=0.3.8,<0.4.0)
 Requires-Dist: eidolon-ai-client (>=0.1.5,<0.2.0)
 Requires-Dist: eidolon-ai-mistralai (>=0.1.6a,<0.2.0)
 Requires-Dist: eidolon-ai-usage-client (>=0.1.0,<0.2.0)
```

