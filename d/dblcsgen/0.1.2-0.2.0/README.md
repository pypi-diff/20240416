# Comparing `tmp/dblcsgen-0.1.2.tar.gz` & `tmp/dblcsgen-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dblcsgen-0.1.2.tar", last modified: Sat Apr 13 19:04:19 2024, max compression
+gzip compressed data, was "dblcsgen-0.2.0.tar", last modified: Tue Apr 16 18:26:20 2024, max compression
```

## Comparing `dblcsgen-0.1.2.tar` & `dblcsgen-0.2.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-13 19:04:19.307901 dblcsgen-0.1.2/
--rw-r--r--   0 theneault   (502) staff       (20)    11357 2024-04-13 19:04:17.000000 dblcsgen-0.1.2/LICENSE
--rw-r--r--   0 theneault   (502) staff       (20)    28296 2024-04-13 19:04:19.307657 dblcsgen-0.1.2/PKG-INFO
--rw-r--r--   0 theneault   (502) staff       (20)    14259 2024-04-13 19:04:17.000000 dblcsgen-0.1.2/README.md
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-13 19:04:19.306621 dblcsgen-0.1.2/dblcsgen.egg-info/
--rw-r--r--   0 theneault   (502) staff       (20)    28296 2024-04-13 19:04:19.000000 dblcsgen-0.1.2/dblcsgen.egg-info/PKG-INFO
--rw-r--r--   0 theneault   (502) staff       (20)     2050 2024-04-13 19:04:19.000000 dblcsgen-0.1.2/dblcsgen.egg-info/SOURCES.txt
--rw-r--r--   0 theneault   (502) staff       (20)        1 2024-04-13 19:04:19.000000 dblcsgen-0.1.2/dblcsgen.egg-info/dependency_links.txt
--rw-r--r--   0 theneault   (502) staff       (20)      150 2024-04-13 19:04:19.000000 dblcsgen-0.1.2/dblcsgen.egg-info/requires.txt
--rw-r--r--   0 theneault   (502) staff       (20)        7 2024-04-13 19:04:19.000000 dblcsgen-0.1.2/dblcsgen.egg-info/top_level.txt
--rw-r--r--   0 theneault   (502) staff       (20)     1012 2024-04-13 19:04:12.000000 dblcsgen-0.1.2/pyproject.toml
--rw-r--r--   0 theneault   (502) staff       (20)       38 2024-04-13 19:04:19.307943 dblcsgen-0.1.2/setup.cfg
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-13 19:04:19.294785 dblcsgen-0.1.2/sglang/
--rw-r--r--   0 theneault   (502) staff       (20)       96 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/__init__.py
--rw-r--r--   0 theneault   (502) staff       (20)     4576 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/api.py
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-13 19:04:19.295843 dblcsgen-0.1.2/sglang/backend/
--rw-r--r--   0 theneault   (502) staff       (20)        0 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/backend/__init__.py
--rw-r--r--   0 theneault   (502) staff       (20)     1677 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/backend/anthropic.py
--rw-r--r--   0 theneault   (502) staff       (20)     1831 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/backend/base_backend.py
--rw-r--r--   0 theneault   (502) staff       (20)     9578 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/backend/openai.py
--rw-r--r--   0 theneault   (502) staff       (20)     8319 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/backend/runtime_endpoint.py
--rw-r--r--   0 theneault   (502) staff       (20)     4713 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/backend/vertexai.py
--rw-r--r--   0 theneault   (502) staff       (20)      797 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/global_config.py
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-13 19:04:19.297167 dblcsgen-0.1.2/sglang/lang/
--rw-r--r--   0 theneault   (502) staff       (20)        0 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/lang/__init__.py
--rw-r--r--   0 theneault   (502) staff       (20)     9633 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/lang/chat_template.py
--rw-r--r--   0 theneault   (502) staff       (20)     7527 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/lang/compiler.py
--rw-r--r--   0 theneault   (502) staff       (20)    26999 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/lang/interpreter.py
--rw-r--r--   0 theneault   (502) staff       (20)    13320 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/lang/ir.py
--rw-r--r--   0 theneault   (502) staff       (20)     8260 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/lang/tracer.py
--rw-r--r--   0 theneault   (502) staff       (20)      294 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/launch_server.py
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-13 19:04:19.299313 dblcsgen-0.1.2/sglang/srt/
--rw-r--r--   0 theneault   (502) staff       (20)      227 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/backend_config.py
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-13 19:04:19.299836 dblcsgen-0.1.2/sglang/srt/constrained/
--rw-r--r--   0 theneault   (502) staff       (20)     1236 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/constrained/__init__.py
--rw-r--r--   0 theneault   (502) staff       (20)     1405 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/constrained/base_cache.py
--rw-r--r--   0 theneault   (502) staff       (20)      902 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/constrained/fsm_cache.py
--rw-r--r--   0 theneault   (502) staff       (20)     2482 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/constrained/jump_forward.py
--rw-r--r--   0 theneault   (502) staff       (20)    15496 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/conversation.py
--rw-r--r--   0 theneault   (502) staff       (20)     5285 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/hf_transformers_utils.py
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-13 19:04:19.300862 dblcsgen-0.1.2/sglang/srt/layers/
--rw-r--r--   0 theneault   (502) staff       (20)     5209 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/layers/context_flashattention_nopad.py
--rw-r--r--   0 theneault   (502) staff       (20)    12622 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/layers/extend_attention.py
--rw-r--r--   0 theneault   (502) staff       (20)     6887 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/layers/logits_processor.py
--rw-r--r--   0 theneault   (502) staff       (20)     5597 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/layers/radix_attention.py
--rw-r--r--   0 theneault   (502) staff       (20)     8516 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/layers/token_attention.py
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-13 19:04:19.301535 dblcsgen-0.1.2/sglang/srt/managers/
--rw-r--r--   0 theneault   (502) staff       (20)     3292 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/managers/detokenizer_manager.py
--rw-r--r--   0 theneault   (502) staff       (20)     3670 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/managers/io_struct.py
--rw-r--r--   0 theneault   (502) staff       (20)     4563 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/managers/openai_protocol.py
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-13 19:04:19.302499 dblcsgen-0.1.2/sglang/srt/managers/router/
--rw-r--r--   0 theneault   (502) staff       (20)    19922 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/managers/router/infer_batch.py
--rw-r--r--   0 theneault   (502) staff       (20)     2682 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/managers/router/manager.py
--rw-r--r--   0 theneault   (502) staff       (20)    28007 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/managers/router/model_rpc.py
--rw-r--r--   0 theneault   (502) staff       (20)    16926 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/managers/router/model_runner.py
--rw-r--r--   0 theneault   (502) staff       (20)     6484 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/managers/router/radix_cache.py
--rw-r--r--   0 theneault   (502) staff       (20)     2818 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/managers/router/scheduler.py
--rw-r--r--   0 theneault   (502) staff       (20)     9743 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/managers/tokenizer_manager.py
--rw-r--r--   0 theneault   (502) staff       (20)     3609 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/memory_pool.py
--rw-r--r--   0 theneault   (502) staff       (20)     8889 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/mm_utils.py
--rw-r--r--   0 theneault   (502) staff       (20)     1546 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/model_config.py
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-13 19:04:19.305646 dblcsgen-0.1.2/sglang/srt/models/
--rw-r--r--   0 theneault   (502) staff       (20)    14112 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/models/dbrx.py
--rw-r--r--   0 theneault   (502) staff       (20)    11071 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/models/dbrx_config.py
--rw-r--r--   0 theneault   (502) staff       (20)    11587 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/models/gemma.py
--rw-r--r--   0 theneault   (502) staff       (20)    11611 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/models/llama2.py
--rw-r--r--   0 theneault   (502) staff       (20)    14922 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/models/llava.py
--rw-r--r--   0 theneault   (502) staff       (20)      254 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/models/mistral.py
--rw-r--r--   0 theneault   (502) staff       (20)    13915 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/models/mixtral.py
--rw-r--r--   0 theneault   (502) staff       (20)     9225 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/models/qwen.py
--rw-r--r--   0 theneault   (502) staff       (20)    11307 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/models/qwen2.py
--rw-r--r--   0 theneault   (502) staff       (20)    10816 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/models/stablelm.py
--rw-r--r--   0 theneault   (502) staff       (20)     4414 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/models/yivl.py
--rw-r--r--   0 theneault   (502) staff       (20)     2896 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/sampling_params.py
--rw-r--r--   0 theneault   (502) staff       (20)    27702 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/server.py
--rw-r--r--   0 theneault   (502) staff       (20)     9143 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/server_args.py
--rw-r--r--   0 theneault   (502) staff       (20)     7582 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/srt/utils.py
-drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-13 19:04:19.306389 dblcsgen-0.1.2/sglang/test/
--rw-r--r--   0 theneault   (502) staff       (20)     1592 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/test/test_conversation.py
--rw-r--r--   0 theneault   (502) staff       (20)     1657 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/test/test_openai_protocol.py
--rw-r--r--   0 theneault   (502) staff       (20)    11421 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/test/test_programs.py
--rw-r--r--   0 theneault   (502) staff       (20)     4830 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/test/test_utils.py
--rw-r--r--   0 theneault   (502) staff       (20)     6237 2024-04-13 18:48:15.000000 dblcsgen-0.1.2/sglang/utils.py
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-16 18:26:20.789239 dblcsgen-0.2.0/
+-rw-r--r--   0 theneault   (502) staff       (20)    11357 2024-04-16 18:26:19.000000 dblcsgen-0.2.0/LICENSE
+-rw-r--r--   0 theneault   (502) staff       (20)    28296 2024-04-16 18:26:20.788990 dblcsgen-0.2.0/PKG-INFO
+-rw-r--r--   0 theneault   (502) staff       (20)    14259 2024-04-16 18:26:19.000000 dblcsgen-0.2.0/README.md
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-16 18:26:20.787965 dblcsgen-0.2.0/dblcsgen.egg-info/
+-rw-r--r--   0 theneault   (502) staff       (20)    28296 2024-04-16 18:26:20.000000 dblcsgen-0.2.0/dblcsgen.egg-info/PKG-INFO
+-rw-r--r--   0 theneault   (502) staff       (20)     2050 2024-04-16 18:26:20.000000 dblcsgen-0.2.0/dblcsgen.egg-info/SOURCES.txt
+-rw-r--r--   0 theneault   (502) staff       (20)        1 2024-04-16 18:26:20.000000 dblcsgen-0.2.0/dblcsgen.egg-info/dependency_links.txt
+-rw-r--r--   0 theneault   (502) staff       (20)      150 2024-04-16 18:26:20.000000 dblcsgen-0.2.0/dblcsgen.egg-info/requires.txt
+-rw-r--r--   0 theneault   (502) staff       (20)        7 2024-04-16 18:26:20.000000 dblcsgen-0.2.0/dblcsgen.egg-info/top_level.txt
+-rw-r--r--   0 theneault   (502) staff       (20)     1012 2024-04-16 18:26:04.000000 dblcsgen-0.2.0/pyproject.toml
+-rw-r--r--   0 theneault   (502) staff       (20)       38 2024-04-16 18:26:20.789289 dblcsgen-0.2.0/setup.cfg
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-16 18:26:20.772573 dblcsgen-0.2.0/sglang/
+-rw-r--r--   0 theneault   (502) staff       (20)       96 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/__init__.py
+-rw-r--r--   0 theneault   (502) staff       (20)     4576 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/api.py
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-16 18:26:20.774554 dblcsgen-0.2.0/sglang/backend/
+-rw-r--r--   0 theneault   (502) staff       (20)        0 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/backend/__init__.py
+-rw-r--r--   0 theneault   (502) staff       (20)     1677 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/backend/anthropic.py
+-rw-r--r--   0 theneault   (502) staff       (20)     1831 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/backend/base_backend.py
+-rw-r--r--   0 theneault   (502) staff       (20)     9578 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/backend/openai.py
+-rw-r--r--   0 theneault   (502) staff       (20)     8319 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/backend/runtime_endpoint.py
+-rw-r--r--   0 theneault   (502) staff       (20)     4713 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/backend/vertexai.py
+-rw-r--r--   0 theneault   (502) staff       (20)      797 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/global_config.py
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-16 18:26:20.776363 dblcsgen-0.2.0/sglang/lang/
+-rw-r--r--   0 theneault   (502) staff       (20)        0 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/lang/__init__.py
+-rw-r--r--   0 theneault   (502) staff       (20)     9633 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/lang/chat_template.py
+-rw-r--r--   0 theneault   (502) staff       (20)     7527 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/lang/compiler.py
+-rw-r--r--   0 theneault   (502) staff       (20)    26999 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/lang/interpreter.py
+-rw-r--r--   0 theneault   (502) staff       (20)    13320 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/lang/ir.py
+-rw-r--r--   0 theneault   (502) staff       (20)     8260 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/lang/tracer.py
+-rw-r--r--   0 theneault   (502) staff       (20)      433 2024-04-16 18:25:50.000000 dblcsgen-0.2.0/sglang/launch_server.py
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-16 18:26:20.779218 dblcsgen-0.2.0/sglang/srt/
+-rw-r--r--   0 theneault   (502) staff       (20)      227 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/backend_config.py
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-16 18:26:20.779918 dblcsgen-0.2.0/sglang/srt/constrained/
+-rw-r--r--   0 theneault   (502) staff       (20)     1236 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/constrained/__init__.py
+-rw-r--r--   0 theneault   (502) staff       (20)     1405 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/constrained/base_cache.py
+-rw-r--r--   0 theneault   (502) staff       (20)      902 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/constrained/fsm_cache.py
+-rw-r--r--   0 theneault   (502) staff       (20)     2482 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/constrained/jump_forward.py
+-rw-r--r--   0 theneault   (502) staff       (20)    15496 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/conversation.py
+-rw-r--r--   0 theneault   (502) staff       (20)     5285 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/hf_transformers_utils.py
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-16 18:26:20.780909 dblcsgen-0.2.0/sglang/srt/layers/
+-rw-r--r--   0 theneault   (502) staff       (20)     5209 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/layers/context_flashattention_nopad.py
+-rw-r--r--   0 theneault   (502) staff       (20)    12622 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/layers/extend_attention.py
+-rw-r--r--   0 theneault   (502) staff       (20)     6887 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/layers/logits_processor.py
+-rw-r--r--   0 theneault   (502) staff       (20)     5597 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/layers/radix_attention.py
+-rw-r--r--   0 theneault   (502) staff       (20)     8516 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/layers/token_attention.py
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-16 18:26:20.781773 dblcsgen-0.2.0/sglang/srt/managers/
+-rw-r--r--   0 theneault   (502) staff       (20)     3292 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/managers/detokenizer_manager.py
+-rw-r--r--   0 theneault   (502) staff       (20)     3670 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/managers/io_struct.py
+-rw-r--r--   0 theneault   (502) staff       (20)     4563 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/managers/openai_protocol.py
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-16 18:26:20.783634 dblcsgen-0.2.0/sglang/srt/managers/router/
+-rw-r--r--   0 theneault   (502) staff       (20)    19922 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/managers/router/infer_batch.py
+-rw-r--r--   0 theneault   (502) staff       (20)     2682 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/managers/router/manager.py
+-rw-r--r--   0 theneault   (502) staff       (20)    28007 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/managers/router/model_rpc.py
+-rw-r--r--   0 theneault   (502) staff       (20)    16926 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/managers/router/model_runner.py
+-rw-r--r--   0 theneault   (502) staff       (20)     6484 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/managers/router/radix_cache.py
+-rw-r--r--   0 theneault   (502) staff       (20)     2818 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/managers/router/scheduler.py
+-rw-r--r--   0 theneault   (502) staff       (20)     9743 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/managers/tokenizer_manager.py
+-rw-r--r--   0 theneault   (502) staff       (20)     3609 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/memory_pool.py
+-rw-r--r--   0 theneault   (502) staff       (20)     8889 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/mm_utils.py
+-rw-r--r--   0 theneault   (502) staff       (20)     1546 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/model_config.py
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-16 18:26:20.786838 dblcsgen-0.2.0/sglang/srt/models/
+-rw-r--r--   0 theneault   (502) staff       (20)    14112 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/models/dbrx.py
+-rw-r--r--   0 theneault   (502) staff       (20)    11071 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/models/dbrx_config.py
+-rw-r--r--   0 theneault   (502) staff       (20)    11587 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/models/gemma.py
+-rw-r--r--   0 theneault   (502) staff       (20)    11611 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/models/llama2.py
+-rw-r--r--   0 theneault   (502) staff       (20)    14922 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/models/llava.py
+-rw-r--r--   0 theneault   (502) staff       (20)      254 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/models/mistral.py
+-rw-r--r--   0 theneault   (502) staff       (20)    13915 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/models/mixtral.py
+-rw-r--r--   0 theneault   (502) staff       (20)     9225 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/models/qwen.py
+-rw-r--r--   0 theneault   (502) staff       (20)    11307 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/models/qwen2.py
+-rw-r--r--   0 theneault   (502) staff       (20)    10816 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/models/stablelm.py
+-rw-r--r--   0 theneault   (502) staff       (20)     4414 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/models/yivl.py
+-rw-r--r--   0 theneault   (502) staff       (20)     2896 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/sampling_params.py
+-rw-r--r--   0 theneault   (502) staff       (20)    27702 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/server.py
+-rw-r--r--   0 theneault   (502) staff       (20)     9143 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/server_args.py
+-rw-r--r--   0 theneault   (502) staff       (20)     7582 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/srt/utils.py
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-16 18:26:20.787684 dblcsgen-0.2.0/sglang/test/
+-rw-r--r--   0 theneault   (502) staff       (20)     1592 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/test/test_conversation.py
+-rw-r--r--   0 theneault   (502) staff       (20)     1657 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/test/test_openai_protocol.py
+-rw-r--r--   0 theneault   (502) staff       (20)    11421 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/test/test_programs.py
+-rw-r--r--   0 theneault   (502) staff       (20)     4830 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/test/test_utils.py
+-rw-r--r--   0 theneault   (502) staff       (20)     6237 2024-04-13 18:48:15.000000 dblcsgen-0.2.0/sglang/utils.py
```

### Comparing `dblcsgen-0.1.2/LICENSE` & `dblcsgen-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/PKG-INFO` & `dblcsgen-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dblcsgen
-Version: 0.1.2
+Version: 0.2.0
 Summary: DBLC Fast Structured Generation
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dblcsgen-0.1.2/README.md` & `dblcsgen-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/dblcsgen.egg-info/PKG-INFO` & `dblcsgen-0.2.0/dblcsgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dblcsgen
-Version: 0.1.2
+Version: 0.2.0
 Summary: DBLC Fast Structured Generation
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dblcsgen-0.1.2/dblcsgen.egg-info/SOURCES.txt` & `dblcsgen-0.2.0/dblcsgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/pyproject.toml` & `dblcsgen-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dblcsgen"
-version = "0.1.2"
+version = "0.2.0"
 description = "DBLC Fast Structured Generation"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `dblcsgen-0.1.2/sglang/api.py` & `dblcsgen-0.2.0/sglang/api.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/backend/anthropic.py` & `dblcsgen-0.2.0/sglang/backend/anthropic.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/backend/base_backend.py` & `dblcsgen-0.2.0/sglang/backend/base_backend.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/backend/openai.py` & `dblcsgen-0.2.0/sglang/backend/openai.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/backend/runtime_endpoint.py` & `dblcsgen-0.2.0/sglang/backend/runtime_endpoint.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/backend/vertexai.py` & `dblcsgen-0.2.0/sglang/backend/vertexai.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/global_config.py` & `dblcsgen-0.2.0/sglang/global_config.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/lang/chat_template.py` & `dblcsgen-0.2.0/sglang/lang/chat_template.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/lang/compiler.py` & `dblcsgen-0.2.0/sglang/lang/compiler.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/lang/interpreter.py` & `dblcsgen-0.2.0/sglang/lang/interpreter.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/lang/ir.py` & `dblcsgen-0.2.0/sglang/lang/ir.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/lang/tracer.py` & `dblcsgen-0.2.0/sglang/lang/tracer.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/constrained/__init__.py` & `dblcsgen-0.2.0/sglang/srt/constrained/__init__.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/constrained/base_cache.py` & `dblcsgen-0.2.0/sglang/srt/constrained/base_cache.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/constrained/fsm_cache.py` & `dblcsgen-0.2.0/sglang/srt/constrained/fsm_cache.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/constrained/jump_forward.py` & `dblcsgen-0.2.0/sglang/srt/constrained/jump_forward.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/conversation.py` & `dblcsgen-0.2.0/sglang/srt/conversation.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/hf_transformers_utils.py` & `dblcsgen-0.2.0/sglang/srt/hf_transformers_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/layers/context_flashattention_nopad.py` & `dblcsgen-0.2.0/sglang/srt/layers/context_flashattention_nopad.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/layers/extend_attention.py` & `dblcsgen-0.2.0/sglang/srt/layers/extend_attention.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/layers/logits_processor.py` & `dblcsgen-0.2.0/sglang/srt/layers/logits_processor.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/layers/radix_attention.py` & `dblcsgen-0.2.0/sglang/srt/layers/radix_attention.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/layers/token_attention.py` & `dblcsgen-0.2.0/sglang/srt/layers/token_attention.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/managers/detokenizer_manager.py` & `dblcsgen-0.2.0/sglang/srt/managers/detokenizer_manager.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/managers/io_struct.py` & `dblcsgen-0.2.0/sglang/srt/managers/io_struct.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/managers/openai_protocol.py` & `dblcsgen-0.2.0/sglang/srt/managers/openai_protocol.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/managers/router/infer_batch.py` & `dblcsgen-0.2.0/sglang/srt/managers/router/infer_batch.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/managers/router/manager.py` & `dblcsgen-0.2.0/sglang/srt/managers/router/manager.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/managers/router/model_rpc.py` & `dblcsgen-0.2.0/sglang/srt/managers/router/model_rpc.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/managers/router/model_runner.py` & `dblcsgen-0.2.0/sglang/srt/managers/router/model_runner.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/managers/router/radix_cache.py` & `dblcsgen-0.2.0/sglang/srt/managers/router/radix_cache.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/managers/router/scheduler.py` & `dblcsgen-0.2.0/sglang/srt/managers/router/scheduler.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/managers/tokenizer_manager.py` & `dblcsgen-0.2.0/sglang/srt/managers/tokenizer_manager.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/memory_pool.py` & `dblcsgen-0.2.0/sglang/srt/memory_pool.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/mm_utils.py` & `dblcsgen-0.2.0/sglang/srt/mm_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/model_config.py` & `dblcsgen-0.2.0/sglang/srt/model_config.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/models/dbrx.py` & `dblcsgen-0.2.0/sglang/srt/models/dbrx.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/models/dbrx_config.py` & `dblcsgen-0.2.0/sglang/srt/models/dbrx_config.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/models/gemma.py` & `dblcsgen-0.2.0/sglang/srt/models/gemma.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/models/llama2.py` & `dblcsgen-0.2.0/sglang/srt/models/llama2.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/models/llava.py` & `dblcsgen-0.2.0/sglang/srt/models/llava.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/models/mixtral.py` & `dblcsgen-0.2.0/sglang/srt/models/mixtral.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/models/qwen.py` & `dblcsgen-0.2.0/sglang/srt/models/qwen.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/models/qwen2.py` & `dblcsgen-0.2.0/sglang/srt/models/qwen2.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/models/stablelm.py` & `dblcsgen-0.2.0/sglang/srt/models/stablelm.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/models/yivl.py` & `dblcsgen-0.2.0/sglang/srt/models/yivl.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/sampling_params.py` & `dblcsgen-0.2.0/sglang/srt/sampling_params.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/server.py` & `dblcsgen-0.2.0/sglang/srt/server.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/server_args.py` & `dblcsgen-0.2.0/sglang/srt/server_args.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/srt/utils.py` & `dblcsgen-0.2.0/sglang/srt/utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/test/test_conversation.py` & `dblcsgen-0.2.0/sglang/test/test_conversation.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/test/test_openai_protocol.py` & `dblcsgen-0.2.0/sglang/test/test_openai_protocol.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/test/test_programs.py` & `dblcsgen-0.2.0/sglang/test/test_programs.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/test/test_utils.py` & `dblcsgen-0.2.0/sglang/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.1.2/sglang/utils.py` & `dblcsgen-0.2.0/sglang/utils.py`

 * *Files identical despite different names*

