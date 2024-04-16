# Comparing `tmp/langfun-0.0.2.dev20240414.tar.gz` & `tmp/langfun-0.0.2.dev20240415.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langfun-0.0.2.dev20240414.tar", last modified: Sun Apr 14 08:26:14 2024, max compression
+gzip compressed data, was "langfun-0.0.2.dev20240415.tar", last modified: Mon Apr 15 08:03:06 2024, max compression
```

## Comparing `langfun-0.0.2.dev20240414.tar` & `langfun-0.0.2.dev20240415.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:26:14.194536 langfun-0.0.2.dev20240414/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-14 08:26:14.194536 langfun-0.0.2.dev20240414/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:26:14.174535 langfun-0.0.2.dev20240414/langfun/
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:26:14.182536 langfun-0.0.2.dev20240414/langfun/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:26:14.182536 langfun-0.0.2.dev20240414/langfun/core/coding/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/coding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:26:14.182536 langfun-0.0.2.dev20240414/langfun/core/coding/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/coding/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/coding/python/correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/coding/python/correction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/coding/python/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/coding/python/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/coding/python/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/coding/python/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/coding/python/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/coding/python/generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/coding/python/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/coding/python/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/coding/python/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/coding/python/permissions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9674 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/component_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:26:14.186535 langfun-0.0.2.dev20240414/langfun/core/eval/
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    55328 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/eval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21540 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/eval/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/eval/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/eval/matching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/eval/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/eval/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/langfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/langfunc_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17185 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/language_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/language_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:26:14.186535 langfun-0.0.2.dev20240414/langfun/core/llms/
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/llms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:26:14.186535 langfun-0.0.2.dev20240414/langfun/core/llms/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/llms/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/llms/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/llms/cache/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/llms/cache/in_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/llms/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/llms/fake_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/llms/google_genai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/llms/google_genai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/llms/llama_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/llms/llama_cpp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11680 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/llms/openai_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:26:14.186535 langfun-0.0.2.dev20240414/langfun/core/memories/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/memories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/memories/conversation_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/memories/conversation_history_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/message_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:26:14.190536 langfun-0.0.2.dev20240414/langfun/core/modalities/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/modalities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/modalities/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/modalities/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/modalities/mime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/modalities/mime_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/modalities/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/modalities/video_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/modality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/modality_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/natural_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/natural_language_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/sampling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:26:14.194536 langfun-0.0.2.dev20240414/langfun/core/structured/
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/structured/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19249 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/structured/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/structured/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/structured/description_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/structured/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/structured/mapping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/structured/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20846 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/structured/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/structured/prompting.py
--rw-r--r--   0 runner    (1001) docker     (127)    19894 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/structured/prompting_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    25057 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/structured/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/structured/schema_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/structured/schema_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22360 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/structured/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/structured/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/structured/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/subscription_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17662 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    13572 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/template_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:26:14.194536 langfun-0.0.2.dev20240414/langfun/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/templates/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/templates/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/templates/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/templates/conversation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/templates/demonstration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/templates/demonstration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/templates/selfplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/templates/selfplay_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/text_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/langfun/core/text_formatting_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:26:14.194536 langfun-0.0.2.dev20240414/langfun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-14 08:26:14.000000 langfun-0.0.2.dev20240414/langfun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-14 08:26:14.000000 langfun-0.0.2.dev20240414/langfun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 08:26:14.000000 langfun-0.0.2.dev20240414/langfun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-14 08:26:14.000000 langfun-0.0.2.dev20240414/langfun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 08:26:14.000000 langfun-0.0.2.dev20240414/langfun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 08:26:14.194536 langfun-0.0.2.dev20240414/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-14 08:25:54.000000 langfun-0.0.2.dev20240414/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:06.931171 langfun-0.0.2.dev20240415/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-15 08:03:06.931171 langfun-0.0.2.dev20240415/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:06.911171 langfun-0.0.2.dev20240415/langfun/
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:06.919170 langfun-0.0.2.dev20240415/langfun/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:06.919170 langfun-0.0.2.dev20240415/langfun/core/coding/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/coding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:06.919170 langfun-0.0.2.dev20240415/langfun/core/coding/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/coding/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/coding/python/correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/coding/python/correction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/coding/python/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/coding/python/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/coding/python/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/coding/python/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/coding/python/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/coding/python/generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/coding/python/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/coding/python/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/coding/python/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/coding/python/permissions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9674 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:06.923171 langfun-0.0.2.dev20240415/langfun/core/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55359 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/eval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21592 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/eval/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/eval/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/eval/matching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/eval/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/eval/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/langfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/langfunc_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17510 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/language_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:06.923171 langfun-0.0.2.dev20240415/langfun/core/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/llms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:06.923171 langfun-0.0.2.dev20240415/langfun/core/llms/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/llms/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/llms/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/llms/cache/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/llms/cache/in_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/llms/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/llms/fake_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/llms/google_genai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/llms/google_genai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/llms/llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/llms/llama_cpp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11463 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/llms/openai_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:06.923171 langfun-0.0.2.dev20240415/langfun/core/memories/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/memories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/memories/conversation_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/memories/conversation_history_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/message_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:06.927171 langfun-0.0.2.dev20240415/langfun/core/modalities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/modalities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/modalities/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/modalities/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/modalities/mime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/modalities/mime_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/modalities/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/modalities/video_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/modality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/modality_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/natural_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/natural_language_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/sampling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:06.927171 langfun-0.0.2.dev20240415/langfun/core/structured/
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/structured/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19301 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/structured/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/structured/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/structured/description_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/structured/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/structured/mapping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/structured/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20980 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/structured/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/structured/prompting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19945 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/structured/prompting_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25057 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/structured/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/structured/schema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/structured/schema_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22360 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/structured/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/structured/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/structured/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/subscription_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17662 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13572 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/template_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:06.931171 langfun-0.0.2.dev20240415/langfun/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/templates/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/templates/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/templates/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/templates/conversation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/templates/demonstration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/templates/demonstration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/templates/selfplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/templates/selfplay_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/text_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/langfun/core/text_formatting_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:06.931171 langfun-0.0.2.dev20240415/langfun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-15 08:03:06.000000 langfun-0.0.2.dev20240415/langfun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-15 08:03:06.000000 langfun-0.0.2.dev20240415/langfun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:03:06.000000 langfun-0.0.2.dev20240415/langfun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-15 08:03:06.000000 langfun-0.0.2.dev20240415/langfun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 08:03:06.000000 langfun-0.0.2.dev20240415/langfun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:03:06.931171 langfun-0.0.2.dev20240415/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-15 08:02:48.000000 langfun-0.0.2.dev20240415/setup.py
```

### Comparing `langfun-0.0.2.dev20240414/LICENSE` & `langfun-0.0.2.dev20240415/LICENSE`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/PKG-INFO` & `langfun-0.0.2.dev20240415/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240414
+Version: 0.0.2.dev20240415
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240414/README.md` & `langfun-0.0.2.dev20240415/README.md`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/__init__.py` & `langfun-0.0.2.dev20240415/langfun/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/__init__.py` & `langfun-0.0.2.dev20240415/langfun/core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 from langfun.core.modality import Modality
 from langfun.core.modality import ModalityRef
 
 # Interfaces for languge models.
 from langfun.core.language_model import LanguageModel
 from langfun.core.language_model import LMSample
 from langfun.core.language_model import LMSamplingOptions
+from langfun.core.language_model import LMSamplingUsage
 from langfun.core.language_model import LMSamplingResult
 from langfun.core.language_model import LMScoringResult
 from langfun.core.language_model import LMCache
 from langfun.core.language_model import LMDebugMode
 
 # Components for building agents.
 from langfun.core.memory import Memory
```

### Comparing `langfun-0.0.2.dev20240414/langfun/core/coding/__init__.py` & `langfun-0.0.2.dev20240415/langfun/core/coding/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/coding/python/__init__.py` & `langfun-0.0.2.dev20240415/langfun/core/coding/python/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/coding/python/correction.py` & `langfun-0.0.2.dev20240415/langfun/core/coding/python/correction.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/coding/python/correction_test.py` & `langfun-0.0.2.dev20240415/langfun/core/coding/python/correction_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/coding/python/errors.py` & `langfun-0.0.2.dev20240415/langfun/core/coding/python/errors.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/coding/python/errors_test.py` & `langfun-0.0.2.dev20240415/langfun/core/coding/python/errors_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/coding/python/execution.py` & `langfun-0.0.2.dev20240415/langfun/core/coding/python/execution.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/coding/python/execution_test.py` & `langfun-0.0.2.dev20240415/langfun/core/coding/python/execution_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/coding/python/generation.py` & `langfun-0.0.2.dev20240415/langfun/core/coding/python/generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/coding/python/generation_test.py` & `langfun-0.0.2.dev20240415/langfun/core/coding/python/generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/coding/python/parsing.py` & `langfun-0.0.2.dev20240415/langfun/core/coding/python/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/coding/python/parsing_test.py` & `langfun-0.0.2.dev20240415/langfun/core/coding/python/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/coding/python/permissions.py` & `langfun-0.0.2.dev20240415/langfun/core/coding/python/permissions.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/coding/python/permissions_test.py` & `langfun-0.0.2.dev20240415/langfun/core/coding/python/permissions_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/component.py` & `langfun-0.0.2.dev20240415/langfun/core/component.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/component_test.py` & `langfun-0.0.2.dev20240415/langfun/core/component_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/concurrent.py` & `langfun-0.0.2.dev20240415/langfun/core/concurrent.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/concurrent_test.py` & `langfun-0.0.2.dev20240415/langfun/core/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/console.py` & `langfun-0.0.2.dev20240415/langfun/core/console.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/console_test.py` & `langfun-0.0.2.dev20240415/langfun/core/console_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/eval/__init__.py` & `langfun-0.0.2.dev20240415/langfun/core/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/eval/base.py` & `langfun-0.0.2.dev20240415/langfun/core/eval/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1561,14 +1561,15 @@
     task_results = {}
     for task in sorted(self.tasks(), key=lambda cls: cls.__name__):
       results = []
       for entry in self.select(task=task).evaluations:
         results.append(
             pg.Dict(
                 experiment=entry,
+                dir=entry.dir,
                 metrics=entry.result.metrics if entry.result else None,
             )
         )
       task_results[task.__name__] = results
     return task_results
 
   def save(self, file: str, pivot_field: str | None = None) -> None:
```

### Comparing `langfun-0.0.2.dev20240414/langfun/core/eval/base_test.py` & `langfun-0.0.2.dev20240415/langfun/core/eval/base_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,14 +190,15 @@
         s.dryrun_output,
         lf.AIMessage(
             text='Solution(final_answer=2)',
             result=Solution(2),
             cache_seed=0,
             score=1.0,
             logprobs=None,
+            usage=lf.LMSamplingUsage(387, 24, 411),
             tags=['lm-response', 'lm-output', 'transformed'],
         ),
     )
 
   def test_run(self):
     lm = fake.StaticSequence([
         'Solution(final_answer=2)',
```

### Comparing `langfun-0.0.2.dev20240414/langfun/core/eval/matching.py` & `langfun-0.0.2.dev20240415/langfun/core/eval/matching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/eval/matching_test.py` & `langfun-0.0.2.dev20240415/langfun/core/eval/matching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/eval/scoring.py` & `langfun-0.0.2.dev20240415/langfun/core/eval/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/eval/scoring_test.py` & `langfun-0.0.2.dev20240415/langfun/core/eval/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/langfunc.py` & `langfun-0.0.2.dev20240415/langfun/core/langfunc.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/langfunc_test.py` & `langfun-0.0.2.dev20240415/langfun/core/langfunc_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,17 @@
 
     i = l.render()
     self.assertEqual(i, 'Hello')
     self.assertEqual(i, message.UserMessage('Hello'))
     self.assertEqual(i.tags, ['rendered'])
 
     r = l()
-    self.assertEqual(r, message.AIMessage('Hello!!!', score=0.0, logprobs=None))
+    self.assertEqual(
+        r, message.AIMessage('Hello!!!', score=0.0, logprobs=None, usage=None)
+    )
     self.assertEqual(r.tags, ['lm-response', 'lm-output'])
     self.assertEqual(r.source, message.UserMessage('Hello'))
     self.assertEqual(r.source.tags, ['rendered', 'lm-input'])
 
     self.assertEqual(str(l), 'Hello')
     print(repr(l))
     self.assertEqual(
@@ -102,15 +104,15 @@
     l = LangFunc('Hello')
     with component.context(lm=ExcitedEchoer()):
       self.assertEqual(l, 'Hello')
       self.assertEqual(l.natural_language_format(), 'Hello')
       self.assertEqual(l.render(), 'Hello')
       r = l()
       self.assertEqual(
-          r, message.AIMessage('Hello!!!', score=0.0, logprobs=None)
+          r, message.AIMessage('Hello!!!', score=0.0, logprobs=None, usage=None)
       )
       self.assertEqual(r.tags, ['lm-response', 'lm-output'])
 
     self.assertEqual(str(l), 'Hello')
 
     with self.assertRaisesRegex(
         AttributeError, '`lm` is not found under its context'
```

### Comparing `langfun-0.0.2.dev20240414/langfun/core/language_model.py` & `langfun-0.0.2.dev20240415/langfun/core/language_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,25 +43,38 @@
 
   logprobs: Annotated[
       list[tuple[str, float, list[tuple[str, float]]]] | None,
       '(token, log prob, top tokens and their probs).',
   ] = None
 
 
+class LMSamplingUsage(pg.Object):
+  """Usage information per completion."""
+
+  prompt_tokens: int
+  completion_tokens: int
+  total_tokens: int
+
+
 class LMSamplingResult(pg.Object):
   """Language model response."""
 
   samples: Annotated[
       list[LMSample],
       (
           'Multiple samples of the same prompt, sorted by their score. '
           'The first candidate has the highest score.'
       ),
   ] = []
 
+  usage: Annotated[
+      LMSamplingUsage | None,
+      'Usage information. Currently only OpenAI models are supported.',
+  ] = None
+
 
 class LMSamplingOptions(component.Component):
   """Language model sampling options."""
 
   temperature: Annotated[
       float | None,
       (
@@ -420,14 +433,16 @@
       result = self.sample(
           [prompt], sampling_options=sampling_options, cache_seed=cache_seed
       )[0]
       response = result.samples[0].response
       logprobs = result.samples[0].logprobs
       response.set('score', result.samples[0].score)
       response.metadata.logprobs = logprobs
+      response.metadata.usage = result.usage
+
       elapse = time.time() - request_start
       self._debug(prompt, response, call_counter, elapse)
       return response
 
   def _debug(
       self,
       prompt: message_lib.Message,
```

### Comparing `langfun-0.0.2.dev20240414/langfun/core/language_model_test.py` & `langfun-0.0.2.dev20240415/langfun/core/language_model_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -34,17 +34,27 @@
               prompts: list[message_lib.Message]
               ) -> list[lm_lib.LMSamplingResult]:
     context = pg.Dict(attempt=0)
 
     def fake_sample(prompts):
       if context.attempt >= self.failures_before_attempt:
         return [
-            lm_lib.LMSamplingResult([lm_lib.LMSample(  # pylint: disable=g-complex-comprehension
-                response=prompt.text * self.sampling_options.top_k,
-                score=self.sampling_options.temperature or -1.0)])
+            lm_lib.LMSamplingResult(
+                [
+                    lm_lib.LMSample(  # pylint: disable=g-complex-comprehension
+                        response=prompt.text * self.sampling_options.top_k,
+                        score=self.sampling_options.temperature or -1.0,
+                    )
+                ],
+                usage=lm_lib.LMSamplingUsage(
+                    prompt_tokens=100,
+                    completion_tokens=100,
+                    total_tokens=200,
+                ),
+            )
             for prompt in prompts
         ]
       context.attempt += 1
       raise ValueError('Failed to sample prompts.')
 
     return concurrent.with_retry(
         fake_sample,
@@ -96,77 +106,108 @@
     self.assertEqual(lm.max_attempts, 2)
 
   def test_sample(self):
     lm = MockModel(top_k=1)
     self.assertEqual(
         lm.sample(prompts=['foo', 'bar']),
         [
-            lm_lib.LMSamplingResult([lm_lib.LMSample('foo', score=-1.0)]),
-            lm_lib.LMSamplingResult([lm_lib.LMSample('bar', score=-1.0)]),
+            lm_lib.LMSamplingResult(
+                [lm_lib.LMSample('foo', score=-1.0)],
+                usage=lm_lib.LMSamplingUsage(100, 100, 200),
+            ),
+            lm_lib.LMSamplingResult(
+                [lm_lib.LMSample('bar', score=-1.0)],
+                usage=lm_lib.LMSamplingUsage(100, 100, 200),
+            ),
         ],
     )
     # Test override sampling_options.
     self.assertEqual(
         lm.sample(
             prompts=['foo', 'bar'],
             sampling_options=lm_lib.LMSamplingOptions(top_k=2, temperature=0.5),
         ),
         [
             lm_lib.LMSamplingResult(
-                [lm_lib.LMSample('foo' * 2, score=0.5)]
+                [lm_lib.LMSample('foo' * 2, score=0.5)],
+                usage=lm_lib.LMSamplingUsage(100, 100, 200),
             ),
             lm_lib.LMSamplingResult(
-                [lm_lib.LMSample('bar' * 2, score=0.5)]
+                [lm_lib.LMSample('bar' * 2, score=0.5)],
+                usage=lm_lib.LMSamplingUsage(100, 100, 200),
             ),
         ],
     )
     # Test override individual flags within sampling_options.
     self.assertEqual(
         lm.sample(prompts=['foo', 'bar'], temperature=1.0),
         [
-            lm_lib.LMSamplingResult([lm_lib.LMSample('foo', score=1.0)]),
-            lm_lib.LMSamplingResult([lm_lib.LMSample('bar', score=1.0)]),
+            lm_lib.LMSamplingResult(
+                [lm_lib.LMSample('foo', score=1.0)],
+                usage=lm_lib.LMSamplingUsage(100, 100, 200),
+            ),
+            lm_lib.LMSamplingResult(
+                [lm_lib.LMSample('bar', score=1.0)],
+                usage=lm_lib.LMSamplingUsage(100, 100, 200),
+            ),
         ],
     )
     self.assertEqual(
         lm.sample(prompts=['foo', 'bar'], top_k=2, temperature=0.7),
         [
             lm_lib.LMSamplingResult(
-                [lm_lib.LMSample('foo' * 2, score=0.7)]
+                [lm_lib.LMSample('foo' * 2, score=0.7)],
+                usage=lm_lib.LMSamplingUsage(100, 100, 200),
             ),
             lm_lib.LMSamplingResult(
-                [lm_lib.LMSample('bar' * 2, score=0.7)]
+                [lm_lib.LMSample('bar' * 2, score=0.7)],
+                usage=lm_lib.LMSamplingUsage(100, 100, 200),
             ),
         ],
     )
 
   def test_call(self):
     lm = MockModel(sampling_options=lm_lib.LMSamplingOptions(top_k=1))
     response = lm(prompt='foo')
     self.assertEqual(response.text, 'foo')
     self.assertEqual(response.score, -1.0)
+    self.assertIsNone(response.logprobs)
+    self.assertEqual(response.usage, lm_lib.LMSamplingUsage(100, 100, 200))
 
     # Test override sampling_options.
     self.assertEqual(
         lm('foo', sampling_options=lm_lib.LMSamplingOptions(top_k=2)), 'foo' * 2
     )
     # Test override individual flags within sampling_options.
     self.assertEqual(lm('foo', top_k=2), 'foo' * 2)
 
   def test_using_cache(self):
     cache = in_memory.InMemory()
     lm = MockModel(cache=cache, top_k=1)
     self.assertEqual(
         lm.sample(prompts=['foo', 'bar']),
         [
-            lm_lib.LMSamplingResult([lm_lib.LMSample(
-                message_lib.AIMessage('foo', cache_seed=0), score=-1.0)]),
-            lm_lib.LMSamplingResult([lm_lib.LMSample(
-                message_lib.AIMessage('bar', cache_seed=0), score=-1.0)]),
-        ])
+            lm_lib.LMSamplingResult(
+                [
+                    lm_lib.LMSample(
+                        message_lib.AIMessage('foo', cache_seed=0), score=-1.0
+                    )
+                ],
+                usage=lm_lib.LMSamplingUsage(100, 100, 200),
+            ),
+            lm_lib.LMSamplingResult(
+                [
+                    lm_lib.LMSample(
+                        message_lib.AIMessage('bar', cache_seed=0), score=-1.0
+                    )
+                ],
+                usage=lm_lib.LMSamplingUsage(100, 100, 200),
+            ),
+        ],
+    )
     self.assertEqual(cache.stats.num_queries, 2)
     self.assertEqual(cache.stats.num_hits, 0)
     self.assertEqual(cache.stats.num_updates, 2)
 
     self.assertEqual(lm('foo'), 'foo')
     self.assertEqual(lm('bar'), 'bar')
     self.assertEqual(cache.stats.num_queries, 4)
@@ -177,18 +218,30 @@
     self.assertEqual(lm('foo', cache_seed=None), 'foo')
     self.assertEqual(cache.stats.num_queries, 4)
     self.assertEqual(cache.stats.num_updates, 2)
 
     self.assertEqual(
         lm.sample(prompts=['foo', 'baz'], temperature=1.0),
         [
-            lm_lib.LMSamplingResult([lm_lib.LMSample(
-                message_lib.AIMessage('foo', cache_seed=0), score=1.0)]),
-            lm_lib.LMSamplingResult([lm_lib.LMSample(
-                message_lib.AIMessage('baz', cache_seed=0), score=1.0)]),
+            lm_lib.LMSamplingResult(
+                [
+                    lm_lib.LMSample(
+                        message_lib.AIMessage('foo', cache_seed=0), score=1.0
+                    )
+                ],
+                usage=lm_lib.LMSamplingUsage(100, 100, 200),
+            ),
+            lm_lib.LMSamplingResult(
+                [
+                    lm_lib.LMSample(
+                        message_lib.AIMessage('baz', cache_seed=0), score=1.0
+                    )
+                ],
+                usage=lm_lib.LMSamplingUsage(100, 100, 200),
+            ),
         ],
     )
     self.assertEqual(cache.stats.num_queries, 6)
     self.assertEqual(cache.stats.num_hits, 2)
     self.assertEqual(cache.stats.num_updates, 4)
 
     self.assertEqual(lm('baz', temperature=1.0), 'baz')
```

### Comparing `langfun-0.0.2.dev20240414/langfun/core/llms/__init__.py` & `langfun-0.0.2.dev20240415/langfun/core/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/llms/cache/__init__.py` & `langfun-0.0.2.dev20240415/langfun/core/llms/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/llms/cache/base.py` & `langfun-0.0.2.dev20240415/langfun/core/llms/cache/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/llms/cache/in_memory.py` & `langfun-0.0.2.dev20240415/langfun/core/llms/cache/in_memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/llms/cache/in_memory_test.py` & `langfun-0.0.2.dev20240415/langfun/core/llms/cache/in_memory_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,18 +58,27 @@
             ('b', (None, None, 1, 40, None, None), 0),
             ('c', (None, None, 1, 40, None, None), 0),
         ],
     )
 
     def cache_entry(response_text, cache_seed=0):
       return base.LMCacheEntry(
-          lf.LMSamplingResult([
-              lf.LMSample(
-                  lf.AIMessage(response_text, cache_seed=cache_seed), score=1.0)
-          ])
+          lf.LMSamplingResult(
+              [
+                  lf.LMSample(
+                      lf.AIMessage(response_text, cache_seed=cache_seed),
+                      score=1.0
+                  )
+              ],
+              usage=lf.LMSamplingUsage(
+                  1,
+                  len(response_text),
+                  len(response_text) + 1,
+              )
+          )
       )
 
     self.assertEqual(
         list(cache.values()),
         [
             cache_entry('1'),
             cache_entry('2', 1),
```

### Comparing `langfun-0.0.2.dev20240414/langfun/core/llms/fake_test.py` & `langfun-0.0.2.dev20240415/langfun/core/llms/fake_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,20 @@
 
 
 class EchoTest(unittest.TestCase):
 
   def test_sample(self):
     lm = fakelm.Echo()
     self.assertEqual(
-        lm.sample(['hi']), [lf.LMSamplingResult([lf.LMSample('hi', 1.0)])]
+        lm.sample(['hi']),
+        [
+            lf.LMSamplingResult(
+                [lf.LMSample('hi', 1.0)],
+                lf.LMSamplingUsage(2, 2, 4))
+        ]
     )
 
   def test_call(self):
     string_io = io.StringIO()
     lm = fakelm.Echo(debug=True)
     with contextlib.redirect_stdout(string_io):
       self.assertEqual(lm('hi'), 'hi')
@@ -49,19 +54,29 @@
 class StaticResponseTest(unittest.TestCase):
 
   def test_sample(self):
     canned_response = "I'm sorry, I can't help you with that."
     lm = fakelm.StaticResponse(canned_response)
     self.assertEqual(
         lm.sample(['hi']),
-        [lf.LMSamplingResult([lf.LMSample(canned_response, 1.0)])],
+        [
+            lf.LMSamplingResult(
+                [lf.LMSample(canned_response, 1.0)],
+                usage=lf.LMSamplingUsage(2, 38, 40)
+            )
+        ],
     )
     self.assertEqual(
         lm.sample(['Tell me a joke.']),
-        [lf.LMSamplingResult([lf.LMSample(canned_response, 1.0)])],
+        [
+            lf.LMSamplingResult(
+                [lf.LMSample(canned_response, 1.0)],
+                usage=lf.LMSamplingUsage(15, 38, 53)
+            )
+        ],
     )
 
   def test_call(self):
     string_io = io.StringIO()
     canned_response = "I'm sorry, I can't help you with that."
     lm = fakelm.StaticResponse(canned_response, debug=True)
 
@@ -81,16 +96,22 @@
         'Hi': 'Hello',
         'How are you?': 'I am fine, how about you?',
     }, temperature=0.5)
     self.assertEqual(lm.sampling_options.temperature, 0.5)
     self.assertEqual(
         lm.sample(['Hi', 'How are you?']),
         [
-            lf.LMSamplingResult([lf.LMSample('Hello', 1.0)]),
-            lf.LMSamplingResult([lf.LMSample('I am fine, how about you?', 1.0)])
+            lf.LMSamplingResult(
+                [lf.LMSample('Hello', 1.0)],
+                usage=lf.LMSamplingUsage(2, 5, 7)
+            ),
+            lf.LMSamplingResult(
+                [lf.LMSample('I am fine, how about you?', 1.0)],
+                usage=lf.LMSamplingUsage(12, 25, 37)
+            )
         ]
     )
     with self.assertRaises(KeyError):
       _ = lm.sample(['I am not in the table.'])
 
 
 class StaticSequenceTest(unittest.TestCase):
@@ -100,16 +121,22 @@
         'Hello',
         'I am fine, how about you?',
     ], temperature=0.5)
     self.assertEqual(lm.sampling_options.temperature, 0.5)
     self.assertEqual(
         lm.sample(['Hi', 'How are you?']),
         [
-            lf.LMSamplingResult([lf.LMSample('Hello', 1.0)]),
-            lf.LMSamplingResult([lf.LMSample('I am fine, how about you?', 1.0)])
+            lf.LMSamplingResult(
+                [lf.LMSample('Hello', 1.0)],
+                usage=lf.LMSamplingUsage(2, 5, 7)
+            ),
+            lf.LMSamplingResult(
+                [lf.LMSample('I am fine, how about you?', 1.0)],
+                usage=lf.LMSamplingUsage(12, 25, 37)
+            )
         ]
     )
     with self.assertRaises(IndexError):
       _ = lm.sample(['No next one.'])
 
 
 if __name__ == '__main__':
```

### Comparing `langfun-0.0.2.dev20240414/langfun/core/llms/google_genai.py` & `langfun-0.0.2.dev20240415/langfun/core/llms/google_genai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/llms/google_genai_test.py` & `langfun-0.0.2.dev20240415/langfun/core/llms/google_genai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/llms/llama_cpp.py` & `langfun-0.0.2.dev20240415/langfun/core/llms/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/llms/llama_cpp_test.py` & `langfun-0.0.2.dev20240415/langfun/core/llms/llama_cpp_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/llms/openai.py` & `langfun-0.0.2.dev20240415/langfun/core/llms/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,28 +22,14 @@
 from langfun.core import modalities as lf_modalities
 import openai
 from openai import error as openai_error
 from openai import openai_object
 import pyglove as pg
 
 
-class Usage(pg.Object):
-  """Usage information per completion."""
-
-  prompt_tokens: int
-  completion_tokens: int
-  total_tokens: int
-
-
-class LMSamplingResult(lf.LMSamplingResult):
-  """LMSamplingResult with usage information."""
-
-  usage: Usage | None = None
-
-
 SUPPORTED_MODELS_AND_SETTINGS = [
     # Model name, max concurrent requests.
     # The concurrent requests is estimated by TPM/RPM from
     # https://platform.openai.com/account/limits
     # GPT-4 Turbo models.
     ('gpt-4-turbo-preview', 1),  # GPT-4 Turbo.
     ('gpt-4-0125-preview', 1),  # GPT-4 Turbo
@@ -177,44 +163,45 @@
       args['max_tokens'] = options.max_tokens
     if options.top_p is not None:
       args['top_p'] = options.top_p
     if options.stop:
       args['stop'] = options.stop
     return args
 
-  def _sample(self, prompts: list[lf.Message]) -> list[LMSamplingResult]:
+  def _sample(self, prompts: list[lf.Message]) -> list[lf.LMSamplingResult]:
     assert self._api_initialized
     if self.is_chat_model:
       return self._chat_complete_batch(prompts)
     else:
       return self._complete_batch(prompts)
 
   def _complete_batch(
-      self, prompts: list[lf.Message]) -> list[LMSamplingResult]:
+      self, prompts: list[lf.Message]
+  ) -> list[lf.LMSamplingResult]:
 
     def _open_ai_completion(prompts):
       response = openai.Completion.create(
           prompt=[p.text for p in prompts],
           **self._get_request_args(self.sampling_options),
       )
       response = cast(openai_object.OpenAIObject, response)
       # Parse response.
       samples_by_index = collections.defaultdict(list)
       for choice in response.choices:
         samples_by_index[choice.index].append(
             lf.LMSample(choice.text.strip(), score=choice.logprobs or 0.0)
         )
 
-      usage = Usage(
+      usage = lf.LMSamplingUsage(
           prompt_tokens=response.usage.prompt_tokens,
           completion_tokens=response.usage.completion_tokens,
           total_tokens=response.usage.total_tokens,
       )
       return [
-          LMSamplingResult(
+          lf.LMSamplingResult(
               samples_by_index[index], usage=usage if index == 0 else None
           )
           for index in sorted(samples_by_index.keys())
       ]
 
     return self._parallel_execute_with_currency_control(
         _open_ai_completion,
@@ -227,15 +214,15 @@
             (openai_error.APIError,
              '.*The server had an error processing your request'),
         ),
     )[0]
 
   def _chat_complete_batch(
       self, prompts: list[lf.Message]
-  ) -> list[LMSamplingResult]:
+  ) -> list[lf.LMSamplingResult]:
     def _open_ai_chat_completion(prompt: lf.Message):
       if self.multimodal:
         content = []
         for chunk in prompt.chunk():
           if isinstance(chunk, str):
             item = dict(type='text', text=chunk)
           elif isinstance(chunk, lf_modalities.Image) and chunk.uri:
@@ -268,17 +255,17 @@
             lf.LMSample(
                 choice.message.content,
                 score=0.0,
                 logprobs=logprobs,
             )
         )
 
-      return LMSamplingResult(
+      return lf.LMSamplingResult(
           samples=samples,
-          usage=Usage(
+          usage=lf.LMSamplingUsage(
               prompt_tokens=response.usage.prompt_tokens,
               completion_tokens=response.usage.completion_tokens,
               total_tokens=response.usage.total_tokens,
           ),
       )
 
     return self._parallel_execute_with_currency_control(
```

### Comparing `langfun-0.0.2.dev20240414/langfun/core/llms/openai_test.py` & `langfun-0.0.2.dev20240415/langfun/core/llms/openai_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,36 +28,42 @@
   for i, _ in enumerate(prompt):
     for k in range(n):
       choices.append(pg.Dict(
           index=i,
           text=f'Sample {k} for prompt {i}.',
           logprobs=k / 10,
       ))
-  return pg.Dict(choices=choices, usage=openai.Usage(
-      prompt_tokens=100,
-      completion_tokens=100,
-      total_tokens=200,
-  ))
+  return pg.Dict(
+      choices=choices,
+      usage=lf.LMSamplingUsage(
+          prompt_tokens=100,
+          completion_tokens=100,
+          total_tokens=200,
+      ),
+  )
 
 
 def mock_chat_completion_query(messages, *, n=1, **kwargs):
   del messages, kwargs
   choices = []
   for k in range(n):
     choices.append(pg.Dict(
         message=pg.Dict(
             content=f'Sample {k} for message.'
         ),
         logprobs=None,
     ))
-  return pg.Dict(choices=choices, usage=openai.Usage(
-      prompt_tokens=100,
-      completion_tokens=100,
-      total_tokens=200,
-  ))
+  return pg.Dict(
+      choices=choices,
+      usage=lf.LMSamplingUsage(
+          prompt_tokens=100,
+          completion_tokens=100,
+          total_tokens=200,
+      ),
+  )
 
 
 def mock_chat_completion_query_vision(messages, *, n=1, **kwargs):
   del kwargs
   choices = []
   urls = [
       c['image_url'] for c in messages[0]['content'] if c['type'] == 'image_url'
@@ -65,19 +71,22 @@
   for k in range(n):
     choices.append(pg.Dict(
         message=pg.Dict(
             content=f'Sample {k} for message: {"".join(urls)}'
         ),
         logprobs=None,
     ))
-  return pg.Dict(choices=choices, usage=openai.Usage(
-      prompt_tokens=100,
-      completion_tokens=100,
-      total_tokens=200,
-  ))
+  return pg.Dict(
+      choices=choices,
+      usage=lf.LMSamplingUsage(
+          prompt_tokens=100,
+          completion_tokens=100,
+          total_tokens=200,
+      ),
+  )
 
 
 class OpenaiTest(unittest.TestCase):
   """Tests for OpenAI language model."""
 
   def test_model_id(self):
     self.assertEqual(
@@ -165,59 +174,90 @@
       mock_completion.side_effect = mock_completion_query
       lm = openai.OpenAI(api_key='test_key', model='text-davinci-003')
       results = lm.sample(
           ['hello', 'bye'], sampling_options=lf.LMSamplingOptions(n=3)
       )
 
     self.assertEqual(len(results), 2)
-    self.assertEqual(results[0], openai.LMSamplingResult([
-        lf.LMSample('Sample 0 for prompt 0.', score=0.0),
-        lf.LMSample('Sample 1 for prompt 0.', score=0.1),
-        lf.LMSample('Sample 2 for prompt 0.', score=0.2),
-    ], usage=openai.Usage(
-        prompt_tokens=100, completion_tokens=100, total_tokens=200)))
-
-    self.assertEqual(results[1], openai.LMSamplingResult([
-        lf.LMSample('Sample 0 for prompt 1.', score=0.0),
-        lf.LMSample('Sample 1 for prompt 1.', score=0.1),
-        lf.LMSample('Sample 2 for prompt 1.', score=0.2),
-    ]))
+    self.assertEqual(
+        results[0],
+        lf.LMSamplingResult(
+            [
+                lf.LMSample('Sample 0 for prompt 0.', score=0.0),
+                lf.LMSample('Sample 1 for prompt 0.', score=0.1),
+                lf.LMSample('Sample 2 for prompt 0.', score=0.2),
+            ],
+            usage=lf.LMSamplingUsage(
+                prompt_tokens=100, completion_tokens=100, total_tokens=200
+            ),
+        ),
+    )
+
+    self.assertEqual(
+        results[1],
+        lf.LMSamplingResult([
+            lf.LMSample('Sample 0 for prompt 1.', score=0.0),
+            lf.LMSample('Sample 1 for prompt 1.', score=0.1),
+            lf.LMSample('Sample 2 for prompt 1.', score=0.2),
+        ]),
+    )
 
   def test_sample_chat_completion(self):
     with mock.patch('openai.ChatCompletion.create') as mock_chat_completion:
       mock_chat_completion.side_effect = mock_chat_completion_query
       lm = openai.OpenAI(api_key='test_key', model='gpt-4')
       results = lm.sample(
           ['hello', 'bye'], sampling_options=lf.LMSamplingOptions(n=3)
       )
 
     self.assertEqual(len(results), 2)
-    self.assertEqual(results[0], openai.LMSamplingResult([
-        lf.LMSample('Sample 0 for message.', score=0.0),
-        lf.LMSample('Sample 1 for message.', score=0.0),
-        lf.LMSample('Sample 2 for message.', score=0.0),
-    ], usage=openai.Usage(
-        prompt_tokens=100, completion_tokens=100, total_tokens=200)))
-    self.assertEqual(results[1], openai.LMSamplingResult([
-        lf.LMSample('Sample 0 for message.', score=0.0),
-        lf.LMSample('Sample 1 for message.', score=0.0),
-        lf.LMSample('Sample 2 for message.', score=0.0),
-    ], usage=openai.Usage(
-        prompt_tokens=100, completion_tokens=100, total_tokens=200)))
+    self.assertEqual(
+        results[0],
+        lf.LMSamplingResult(
+            [
+                lf.LMSample('Sample 0 for message.', score=0.0),
+                lf.LMSample('Sample 1 for message.', score=0.0),
+                lf.LMSample('Sample 2 for message.', score=0.0),
+            ],
+            usage=lf.LMSamplingUsage(
+                prompt_tokens=100, completion_tokens=100, total_tokens=200
+            ),
+        ),
+    )
+    self.assertEqual(
+        results[1],
+        lf.LMSamplingResult(
+            [
+                lf.LMSample('Sample 0 for message.', score=0.0),
+                lf.LMSample('Sample 1 for message.', score=0.0),
+                lf.LMSample('Sample 2 for message.', score=0.0),
+            ],
+            usage=lf.LMSamplingUsage(
+                prompt_tokens=100, completion_tokens=100, total_tokens=200
+            ),
+        ),
+    )
 
   def test_sample_with_contextual_options(self):
     with mock.patch('openai.Completion.create') as mock_completion:
       mock_completion.side_effect = mock_completion_query
       lm = openai.OpenAI(api_key='test_key', model='text-davinci-003')
       with lf.use_settings(sampling_options=lf.LMSamplingOptions(n=2)):
         results = lm.sample(['hello'])
 
     self.assertEqual(len(results), 1)
-    self.assertEqual(results[0], openai.LMSamplingResult([
-        lf.LMSample('Sample 0 for prompt 0.', score=0.0),
-        lf.LMSample('Sample 1 for prompt 0.', score=0.1),
-    ], usage=openai.Usage(
-        prompt_tokens=100, completion_tokens=100, total_tokens=200)))
+    self.assertEqual(
+        results[0],
+        lf.LMSamplingResult(
+            [
+                lf.LMSample('Sample 0 for prompt 0.', score=0.0),
+                lf.LMSample('Sample 1 for prompt 0.', score=0.1),
+            ],
+            usage=lf.LMSamplingUsage(
+                prompt_tokens=100, completion_tokens=100, total_tokens=200
+            ),
+        ),
+    )
 
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `langfun-0.0.2.dev20240414/langfun/core/memories/__init__.py` & `langfun-0.0.2.dev20240415/langfun/core/memories/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/memories/conversation_history.py` & `langfun-0.0.2.dev20240415/langfun/core/memories/conversation_history.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/memories/conversation_history_test.py` & `langfun-0.0.2.dev20240415/langfun/core/memories/conversation_history_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/memory.py` & `langfun-0.0.2.dev20240415/langfun/core/memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/message.py` & `langfun-0.0.2.dev20240415/langfun/core/message.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/message_test.py` & `langfun-0.0.2.dev20240415/langfun/core/message_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/modalities/__init__.py` & `langfun-0.0.2.dev20240415/langfun/core/modalities/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/modalities/image.py` & `langfun-0.0.2.dev20240415/langfun/core/modalities/image.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/modalities/image_test.py` & `langfun-0.0.2.dev20240415/langfun/core/modalities/image_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/modalities/mime.py` & `langfun-0.0.2.dev20240415/langfun/core/modalities/mime.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/modalities/mime_test.py` & `langfun-0.0.2.dev20240415/langfun/core/modalities/mime_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/modalities/video.py` & `langfun-0.0.2.dev20240415/langfun/core/modalities/video.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/modalities/video_test.py` & `langfun-0.0.2.dev20240415/langfun/core/modalities/video_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/modality.py` & `langfun-0.0.2.dev20240415/langfun/core/modality.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/modality_test.py` & `langfun-0.0.2.dev20240415/langfun/core/modality_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/natural_language.py` & `langfun-0.0.2.dev20240415/langfun/core/natural_language.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/natural_language_test.py` & `langfun-0.0.2.dev20240415/langfun/core/natural_language_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/sampling.py` & `langfun-0.0.2.dev20240415/langfun/core/sampling.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/sampling_test.py` & `langfun-0.0.2.dev20240415/langfun/core/sampling_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/structured/__init__.py` & `langfun-0.0.2.dev20240415/langfun/core/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/structured/completion.py` & `langfun-0.0.2.dev20240415/langfun/core/structured/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/structured/completion_test.py` & `langfun-0.0.2.dev20240415/langfun/core/structured/completion_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -579,14 +579,15 @@
             lm=fake.StaticSequence(['Activity(description="foo")']),
             returns_message=True),
         lf.AIMessage(
             text='Activity(description="foo")',
             result=Activity(description='foo'),
             score=1.0,
             logprobs=None,
+            usage=lf.LMSamplingUsage(553, 27, 580),
             tags=['lm-response', 'lm-output', 'transformed']
         )
     )
 
   def test_using_the_same_lm_instance(self):
     lm = fake.StaticSequence(['Activity(description="foo")'])
     self.assertEqual(
```

### Comparing `langfun-0.0.2.dev20240414/langfun/core/structured/description.py` & `langfun-0.0.2.dev20240415/langfun/core/structured/description.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/structured/description_test.py` & `langfun-0.0.2.dev20240415/langfun/core/structured/description_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/structured/mapping.py` & `langfun-0.0.2.dev20240415/langfun/core/structured/mapping.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/structured/mapping_test.py` & `langfun-0.0.2.dev20240415/langfun/core/structured/mapping_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/structured/parsing.py` & `langfun-0.0.2.dev20240415/langfun/core/structured/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/structured/parsing_test.py` & `langfun-0.0.2.dev20240415/langfun/core/structured/parsing_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,21 +276,23 @@
     self.assertEqual(parsing.parse('the answer is 1', int, lm=lm), 1)
     self.assertEqual(
         parsing.parse(
             'the answer is 1', int, user_prompt='what is 0 + 1?', lm=lm
         ),
         1,
     )
+    r = parsing.parse(
+        'the answer is 1', int, user_prompt='what is 0 + 1?', lm=lm,
+        returns_message=True
+    )
     self.assertEqual(
-        parsing.parse(
-            'the answer is 1', int, user_prompt='what is 0 + 1?', lm=lm,
-            returns_message=True
-        ),
+        r,
         lf.AIMessage(
             '1', score=1.0, result=1, logprobs=None,
+            usage=lf.LMSamplingUsage(652, 1, 653),
             tags=['lm-response', 'lm-output', 'transformed']
         ),
     )
 
 
 class ParseStructureJsonTest(unittest.TestCase):
 
@@ -630,21 +632,26 @@
 
     with lf.context(lm=fake.StaticSequence(['three', '3'])):
       self.assertEqual(
           parsing.call(lf.LangFunc('Compute {{x}} + {{y}}', x=1, y=2), int), 3
       )
 
   def test_call_with_returning_message(self):
+    r = parsing.call(
+        'Compute 1 + 2', int, lm=fake.StaticSequence(['three', '3']),
+        returns_message=True
+    )
     self.assertEqual(
-        parsing.call(
-            'Compute 1 + 2', int, lm=fake.StaticSequence(['three', '3']),
-            returns_message=True
-        ),
+        r,
         lf.AIMessage(
-            '3', result=3, score=1.0, logprobs=None,
+            '3',
+            result=3,
+            score=1.0,
+            logprobs=None,
+            usage=lf.LMSamplingUsage(315, 1, 316),
             tags=['lm-response', 'lm-output', 'transformed']
         ),
     )
 
   def test_call_with_parsing_args(self):
     self.assertEqual(
         parsing.call(
```

### Comparing `langfun-0.0.2.dev20240414/langfun/core/structured/prompting.py` & `langfun-0.0.2.dev20240415/langfun/core/structured/prompting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/structured/prompting_test.py` & `langfun-0.0.2.dev20240415/langfun/core/structured/prompting_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
             'what is 1 + 0', int, lm=lm.clone(), returns_message=True
         ),
         lf.AIMessage(
             '1',
             result=1,
             score=1.0,
             logprobs=None,
+            usage=lf.LMSamplingUsage(323, 1, 324),
             tags=['lm-response', 'lm-output', 'transformed'],
         ),
     )
     self.assertEqual(
         prompting.query(
             lf.Template('what is {{x}} + {{y}}'), int, x=1, y=0, lm=lm.clone()
         ),
```

### Comparing `langfun-0.0.2.dev20240414/langfun/core/structured/schema.py` & `langfun-0.0.2.dev20240415/langfun/core/structured/schema.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/structured/schema_generation.py` & `langfun-0.0.2.dev20240415/langfun/core/structured/schema_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/structured/schema_generation_test.py` & `langfun-0.0.2.dev20240415/langfun/core/structured/schema_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/structured/schema_test.py` & `langfun-0.0.2.dev20240415/langfun/core/structured/schema_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/structured/scoring.py` & `langfun-0.0.2.dev20240415/langfun/core/structured/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/structured/scoring_test.py` & `langfun-0.0.2.dev20240415/langfun/core/structured/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/subscription.py` & `langfun-0.0.2.dev20240415/langfun/core/subscription.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/subscription_test.py` & `langfun-0.0.2.dev20240415/langfun/core/subscription_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/template.py` & `langfun-0.0.2.dev20240415/langfun/core/template.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/template_test.py` & `langfun-0.0.2.dev20240415/langfun/core/template_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/templates/__init__.py` & `langfun-0.0.2.dev20240415/langfun/core/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/templates/completion.py` & `langfun-0.0.2.dev20240415/langfun/core/templates/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/templates/completion_test.py` & `langfun-0.0.2.dev20240415/langfun/core/templates/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/templates/conversation.py` & `langfun-0.0.2.dev20240415/langfun/core/templates/conversation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/templates/conversation_test.py` & `langfun-0.0.2.dev20240415/langfun/core/templates/conversation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/templates/demonstration.py` & `langfun-0.0.2.dev20240415/langfun/core/templates/demonstration.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/templates/demonstration_test.py` & `langfun-0.0.2.dev20240415/langfun/core/templates/demonstration_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/templates/selfplay.py` & `langfun-0.0.2.dev20240415/langfun/core/templates/selfplay.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/templates/selfplay_test.py` & `langfun-0.0.2.dev20240415/langfun/core/templates/selfplay_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,22 +52,26 @@
 
 class SelfPlayTest(unittest.TestCase):
 
   def test_play(self):
     g = NumberGuess(target_num=10)
 
     with lf.context(lm=NumberGuesser(guesses=[50, 20, 5, 10])):
-      self.assertEqual(g(), lf.AIMessage('10', score=0.0, logprobs=None))
+      self.assertEqual(
+          g(), lf.AIMessage('10', score=0.0, logprobs=None, usage=None)
+      )
 
     self.assertEqual(g.num_turns, 4)
 
   def test_play_with_num_turns(self):
     g = NumberGuess(target_num=10, max_turns=10)
 
     with lf.context(lm=NumberGuesser(guesses=[50, 20, 5, 2, 5, 4])):
-      self.assertEqual(g(), lf.AIMessage('2', score=0.0, logprobs=None))
+      self.assertEqual(
+          g(), lf.AIMessage('2', score=0.0, logprobs=None, usage=None)
+      )
 
     self.assertEqual(g.num_turns, 10)
 
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `langfun-0.0.2.dev20240414/langfun/core/text_formatting.py` & `langfun-0.0.2.dev20240415/langfun/core/text_formatting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun/core/text_formatting_test.py` & `langfun-0.0.2.dev20240415/langfun/core/text_formatting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/langfun.egg-info/PKG-INFO` & `langfun-0.0.2.dev20240415/langfun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240414
+Version: 0.0.2.dev20240415
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240414/langfun.egg-info/SOURCES.txt` & `langfun-0.0.2.dev20240415/langfun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240414/setup.py` & `langfun-0.0.2.dev20240415/setup.py`

 * *Files identical despite different names*

