# Comparing `tmp/aibridge_test-0.2.9.tar.gz` & `tmp/aibridge_test-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aibridge_test-0.2.9.tar", last modified: Thu Apr 11 11:23:16 2024, max compression
+gzip compressed data, was "aibridge_test-0.3.0.tar", last modified: Tue Apr 16 09:32:48 2024, max compression
```

## Comparing `aibridge_test-0.2.9.tar` & `aibridge_test-0.3.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 11:23:16.654936 aibridge_test-0.2.9/
-drwxrwxrwx   0        0        0        0 2024-04-11 11:23:15.277304 aibridge_test-0.2.9/AIBridge/
--rw-rw-rw-   0        0        0     1575 2024-04-04 08:38:44.000000 aibridge_test-0.2.9/AIBridge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:23:15.550299 aibridge_test-0.2.9/AIBridge/ai_services/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/ai_services/__init__.py
--rw-rw-rw-   0        0        0     9311 2024-04-11 09:50:53.000000 aibridge_test-0.2.9/AIBridge/ai_services/ai21labs_text.py
--rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/ai_services/ai_abstraction.py
--rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/ai_services/ai_services_response.py
--rw-rw-rw-   0        0        0    13501 2024-04-11 09:51:01.000000 aibridge_test-0.2.9/AIBridge/ai_services/anthropic_ai.py
--rw-rw-rw-   0        0        0    12216 2024-04-11 09:51:03.000000 aibridge_test-0.2.9/AIBridge/ai_services/cohere_llm.py
--rw-rw-rw-   0        0        0    14353 2024-04-11 09:47:06.000000 aibridge_test-0.2.9/AIBridge/ai_services/geminin_services.py
--rw-rw-rw-   0        0        0     3580 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/ai_services/image_optimisaton.py
--rw-rw-rw-   0        0        0     7514 2024-01-22 04:54:52.000000 aibridge_test-0.2.9/AIBridge/ai_services/openai_images.py
--rw-rw-rw-   0        0        0    11817 2024-04-11 09:46:41.000000 aibridge_test-0.2.9/AIBridge/ai_services/openai_services.py
--rw-rw-rw-   0        0        0     2947 2024-04-01 10:21:53.000000 aibridge_test-0.2.9/AIBridge/ai_services/palm_chat.py
--rw-rw-rw-   0        0        0     9196 2024-04-02 05:11:27.000000 aibridge_test-0.2.9/AIBridge/ai_services/palm_text.py
--rw-rw-rw-   0        0        0     2024 2024-04-04 04:17:16.000000 aibridge_test-0.2.9/AIBridge/ai_services/process_mq.py
--rw-rw-rw-   0        0        0    10350 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/ai_services/stable_diffusion_image.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:23:15.581300 aibridge_test-0.2.9/AIBridge/constant/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/constant/__init__.py
--rw-rw-rw-   0        0        0     7561 2024-04-08 06:59:23.000000 aibridge_test-0.2.9/AIBridge/constant/common.py
--rw-rw-rw-   0        0        0      914 2024-04-05 09:37:33.000000 aibridge_test-0.2.9/AIBridge/constant/constant.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:23:15.706308 aibridge_test-0.2.9/AIBridge/database/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/database/__init__.py
--rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/database/db_layer.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:23:15.726300 aibridge_test-0.2.9/AIBridge/database/models/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/database/models/__init__.py
--rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/database/models/ai_response.py
--rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/database/models/prompts.py
--rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/database/models/variables.py
--rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/database/no_sql_service.py
--rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/database/session.py
--rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/database/sql_service.py
--rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/database/table_oprations.py
--rw-rw-rw-   0        0        0     1161 2024-04-04 03:54:10.000000 aibridge_test-0.2.9/AIBridge/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:23:15.884299 aibridge_test-0.2.9/AIBridge/output_validation/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/output_validation/__init__.py
--rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/output_validation/active_validator.py
--rw-rw-rw-   0        0        0     1613 2024-04-04 09:51:39.000000 aibridge_test-0.2.9/AIBridge/output_validation/convertors.py
--rw-rw-rw-   0        0        0     5866 2024-04-04 10:12:50.000000 aibridge_test-0.2.9/AIBridge/output_validation/validations.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:23:16.220302 aibridge_test-0.2.9/AIBridge/prompts/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/prompts/__init__.py
--rw-rw-rw-   0        0        0     3143 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/prompts/prompt_completion.py
--rw-rw-rw-   0        0        0     3896 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/prompts/prompts_save.py
--rw-rw-rw-   0        0        0     2733 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/prompts/prompts_varibales.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:23:16.354298 aibridge_test-0.2.9/AIBridge/queue_integration/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/queue_integration/__init__.py
--rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/queue_integration/assign_queue.py
--rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/queue_integration/message_queue.py
--rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/queue_integration/queue_model.py
--rw-rw-rw-   0        0        0     6965 2024-04-04 04:16:23.000000 aibridge_test-0.2.9/AIBridge/queue_integration/response_class.py
--rw-rw-rw-   0        0        0     2945 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/setconfig.py
--rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/LICENSE
--rw-rw-rw-   0        0        0    21534 2024-04-11 11:23:16.644868 aibridge_test-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 11:23:16.642872 aibridge_test-0.2.9/aibridge_test.egg-info/
--rw-rw-rw-   0        0        0    21534 2024-04-11 11:23:14.000000 aibridge_test-0.2.9/aibridge_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1768 2024-04-11 11:23:15.000000 aibridge_test-0.2.9/aibridge_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 11:23:14.000000 aibridge_test-0.2.9/aibridge_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      228 2024-04-11 11:23:14.000000 aibridge_test-0.2.9/aibridge_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-11 11:23:14.000000 aibridge_test-0.2.9/aibridge_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 11:23:16.654936 aibridge_test-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     2863 2024-04-11 11:12:45.000000 aibridge_test-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:32:48.373476 aibridge_test-0.3.0/
+drwxrwxrwx   0        0        0        0 2024-04-16 09:32:46.680517 aibridge_test-0.3.0/AIBridge/
+-rw-rw-rw-   0        0        0     1575 2024-04-04 08:38:44.000000 aibridge_test-0.3.0/AIBridge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:32:47.493468 aibridge_test-0.3.0/AIBridge/ai_services/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/ai_services/__init__.py
+-rw-rw-rw-   0        0        0     9311 2024-04-11 09:50:53.000000 aibridge_test-0.3.0/AIBridge/ai_services/ai21labs_text.py
+-rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/ai_services/ai_abstraction.py
+-rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/ai_services/ai_services_response.py
+-rw-rw-rw-   0        0        0    13501 2024-04-11 09:51:01.000000 aibridge_test-0.3.0/AIBridge/ai_services/anthropic_ai.py
+-rw-rw-rw-   0        0        0    12216 2024-04-11 09:51:03.000000 aibridge_test-0.3.0/AIBridge/ai_services/cohere_llm.py
+-rw-rw-rw-   0        0        0    14353 2024-04-11 09:47:06.000000 aibridge_test-0.3.0/AIBridge/ai_services/geminin_services.py
+-rw-rw-rw-   0        0        0     3580 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/ai_services/image_optimisaton.py
+-rw-rw-rw-   0        0        0     7514 2024-01-22 04:54:52.000000 aibridge_test-0.3.0/AIBridge/ai_services/openai_images.py
+-rw-rw-rw-   0        0        0    11817 2024-04-11 09:46:41.000000 aibridge_test-0.3.0/AIBridge/ai_services/openai_services.py
+-rw-rw-rw-   0        0        0     2947 2024-04-01 10:21:53.000000 aibridge_test-0.3.0/AIBridge/ai_services/palm_chat.py
+-rw-rw-rw-   0        0        0     9196 2024-04-02 05:11:27.000000 aibridge_test-0.3.0/AIBridge/ai_services/palm_text.py
+-rw-rw-rw-   0        0        0     2024 2024-04-04 04:17:16.000000 aibridge_test-0.3.0/AIBridge/ai_services/process_mq.py
+-rw-rw-rw-   0        0        0    10350 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/ai_services/stable_diffusion_image.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:32:47.603468 aibridge_test-0.3.0/AIBridge/constant/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/constant/__init__.py
+-rw-rw-rw-   0        0        0     7755 2024-04-16 09:20:57.000000 aibridge_test-0.3.0/AIBridge/constant/common.py
+-rw-rw-rw-   0        0        0      914 2024-04-05 09:37:33.000000 aibridge_test-0.3.0/AIBridge/constant/constant.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:32:47.888467 aibridge_test-0.3.0/AIBridge/database/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/database/__init__.py
+-rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/database/db_layer.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:32:47.902466 aibridge_test-0.3.0/AIBridge/database/models/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/database/models/__init__.py
+-rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/database/models/ai_response.py
+-rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/database/models/prompts.py
+-rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/database/models/variables.py
+-rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/database/no_sql_service.py
+-rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/database/session.py
+-rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/database/sql_service.py
+-rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/database/table_oprations.py
+-rw-rw-rw-   0        0        0     1161 2024-04-04 03:54:10.000000 aibridge_test-0.3.0/AIBridge/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:32:47.921477 aibridge_test-0.3.0/AIBridge/output_validation/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/output_validation/__init__.py
+-rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/output_validation/active_validator.py
+-rw-rw-rw-   0        0        0     1613 2024-04-04 09:51:39.000000 aibridge_test-0.3.0/AIBridge/output_validation/convertors.py
+-rw-rw-rw-   0        0        0     5866 2024-04-04 10:12:50.000000 aibridge_test-0.3.0/AIBridge/output_validation/validations.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:32:48.038484 aibridge_test-0.3.0/AIBridge/prompts/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/prompts/__init__.py
+-rw-rw-rw-   0        0        0     3143 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/prompts/prompt_completion.py
+-rw-rw-rw-   0        0        0     3896 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/prompts/prompts_save.py
+-rw-rw-rw-   0        0        0     2733 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/prompts/prompts_varibales.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:32:48.065472 aibridge_test-0.3.0/AIBridge/queue_integration/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/queue_integration/__init__.py
+-rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/queue_integration/assign_queue.py
+-rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/queue_integration/message_queue.py
+-rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/AIBridge/queue_integration/queue_model.py
+-rw-rw-rw-   0        0        0     6965 2024-04-04 04:16:23.000000 aibridge_test-0.3.0/AIBridge/queue_integration/response_class.py
+-rw-rw-rw-   0        0        0     2945 2024-04-16 09:21:15.000000 aibridge_test-0.3.0/AIBridge/setconfig.py
+-rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0    21534 2024-04-16 09:32:48.346469 aibridge_test-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 09:32:48.339470 aibridge_test-0.3.0/aibridge_test.egg-info/
+-rw-rw-rw-   0        0        0    21534 2024-04-16 09:32:46.000000 aibridge_test-0.3.0/aibridge_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1768 2024-04-16 09:32:46.000000 aibridge_test-0.3.0/aibridge_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 09:32:46.000000 aibridge_test-0.3.0/aibridge_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      228 2024-04-16 09:32:46.000000 aibridge_test-0.3.0/aibridge_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-16 09:32:46.000000 aibridge_test-0.3.0/aibridge_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 09:32:48.385470 aibridge_test-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2863 2024-04-16 09:31:23.000000 aibridge_test-0.3.0/setup.py
```

### Comparing `aibridge_test-0.2.9/AIBridge/__init__.py` & `aibridge_test-0.3.0/AIBridge/__init__.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/ai_services/ai21labs_text.py` & `aibridge_test-0.3.0/AIBridge/ai_services/ai21labs_text.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/ai_services/ai_services_response.py` & `aibridge_test-0.3.0/AIBridge/ai_services/ai_services_response.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/ai_services/anthropic_ai.py` & `aibridge_test-0.3.0/AIBridge/ai_services/anthropic_ai.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/ai_services/cohere_llm.py` & `aibridge_test-0.3.0/AIBridge/ai_services/cohere_llm.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/ai_services/geminin_services.py` & `aibridge_test-0.3.0/AIBridge/ai_services/geminin_services.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/ai_services/image_optimisaton.py` & `aibridge_test-0.3.0/AIBridge/ai_services/image_optimisaton.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/ai_services/openai_images.py` & `aibridge_test-0.3.0/AIBridge/ai_services/openai_images.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/ai_services/openai_services.py` & `aibridge_test-0.3.0/AIBridge/ai_services/openai_services.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/ai_services/palm_chat.py` & `aibridge_test-0.3.0/AIBridge/ai_services/palm_chat.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/ai_services/palm_text.py` & `aibridge_test-0.3.0/AIBridge/ai_services/palm_text.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/ai_services/process_mq.py` & `aibridge_test-0.3.0/AIBridge/ai_services/process_mq.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/ai_services/stable_diffusion_image.py` & `aibridge_test-0.3.0/AIBridge/ai_services/stable_diffusion_image.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/constant/common.py` & `aibridge_test-0.3.0/AIBridge/constant/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,19 @@
     )
     return prompt
 
 
 def parse_api_key(ai_service):
     if ai_service not in config:
         raise ConfigException("ai_service not found in config file")
-    return config[ai_service][0]["key"]
+    for ext in PRIORITY:
+        if ext in config[ai_service]:
+            if config[ai_service][ext]:
+                return config[ai_service][ext][0]
+    raise ConfigException(f" {ai_service} api_key not found in config file")
 
 
 def get_no_sql_obj():
     databse_uri = config["database_uri"]
     if "mongodb" in databse_uri:
         return Mongodb()
```

### Comparing `aibridge_test-0.2.9/AIBridge/constant/constant.py` & `aibridge_test-0.3.0/AIBridge/constant/constant.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/database/db_layer.py` & `aibridge_test-0.3.0/AIBridge/database/db_layer.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/database/no_sql_service.py` & `aibridge_test-0.3.0/AIBridge/database/no_sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/database/session.py` & `aibridge_test-0.3.0/AIBridge/database/session.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/database/sql_service.py` & `aibridge_test-0.3.0/AIBridge/database/sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/exceptions.py` & `aibridge_test-0.3.0/AIBridge/exceptions.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/output_validation/convertors.py` & `aibridge_test-0.3.0/AIBridge/output_validation/convertors.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/output_validation/validations.py` & `aibridge_test-0.3.0/AIBridge/output_validation/validations.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/prompts/prompt_completion.py` & `aibridge_test-0.3.0/AIBridge/prompts/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/prompts/prompts_save.py` & `aibridge_test-0.3.0/AIBridge/prompts/prompts_save.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/prompts/prompts_varibales.py` & `aibridge_test-0.3.0/AIBridge/prompts/prompts_varibales.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/queue_integration/message_queue.py` & `aibridge_test-0.3.0/AIBridge/queue_integration/message_queue.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/queue_integration/queue_model.py` & `aibridge_test-0.3.0/AIBridge/queue_integration/queue_model.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/queue_integration/response_class.py` & `aibridge_test-0.3.0/AIBridge/queue_integration/response_class.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/AIBridge/setconfig.py` & `aibridge_test-0.3.0/AIBridge/setconfig.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/LICENSE` & `aibridge_test-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/PKG-INFO` & `aibridge_test-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.2.9
+Version: 0.3.0
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aibridge_test-0.2.9/README.md` & `aibridge_test-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/aibridge_test.egg-info/PKG-INFO` & `aibridge_test-0.3.0/aibridge_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.2.9
+Version: 0.3.0
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aibridge_test-0.2.9/aibridge_test.egg-info/SOURCES.txt` & `aibridge_test-0.3.0/aibridge_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.9/setup.py` & `aibridge_test-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = "aibridge_test"
 DESCRIPTION = 'Bridge for LLM"s'
 URL = "https://github.com/me/myproject"
 EMAIL = "ashish.tilekar@opsfuse.com"
 AUTHOR = "Ashish Tilekar"
 REQUIRES_PYTHON = ">=3.9.0"
-VERSION = "0.2.9"
+VERSION = "0.3.0"
 REQUIRED = [
     "openai<=1.7.1",
     "SQLAlchemy>=2.0.19",
     "redis>=4.6.0",
     "PyYAML>=6.0.1",
     "Jinja2>=3.1.2",
     "pymongo>=4.4.1",
```

