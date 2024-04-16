# Comparing `tmp/superagent_py-0.2.29.tar.gz` & `tmp/superagent_py-0.2.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superagent_py-0.2.29.tar", max compression
+gzip compressed data, was "superagent_py-0.2.30.tar", max compression
```

## Comparing `superagent_py-0.2.29.tar` & `superagent_py-0.2.30.tar`

### file list

```diff
@@ -1,99 +1,99 @@
--rw-r--r--   0        0        0     1073 2024-04-13 03:51:47.321519 superagent_py-0.2.29/LICENSE
--rw-r--r--   0        0        0     3946 2024-04-13 03:51:47.321519 superagent_py-0.2.29/README.md
--rw-r--r--   0        0        0      434 2024-04-13 03:51:47.321519 superagent_py-0.2.29/pyproject.toml
--rw-r--r--   0        0        0     3944 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/__init__.py
--rw-r--r--   0        0        0     6143 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/client.py
--rw-r--r--   0        0        0      790 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/core/api_error.py
--rw-r--r--   0        0        0     1732 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/core/file.py
--rw-r--r--   0        0        0     4882 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/core/request_options.py
--rw-r--r--   0        0        0      166 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/environment.py
--rw-r--r--   0        0        0      170 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/py.typed
--rw-r--r--   0        0        0      333 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/resources/agent/__init__.py
--rw-r--r--   0        0        0    71786 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/resources/agent/client.py
--rw-r--r--   0        0        0       65 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/resources/api_key/__init__.py
--rw-r--r--   0        0        0    17585 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/resources/api_key/client.py
--rw-r--r--   0        0        0       65 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/resources/api_user/__init__.py
--rw-r--r--   0        0        0    17007 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/resources/api_user/client.py
--rw-r--r--   0        0        0       65 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/resources/datasource/__init__.py
--rw-r--r--   0        0        0    23365 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/resources/datasource/client.py
--rw-r--r--   0        0        0       65 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/resources/llm/__init__.py
--rw-r--r--   0        0        0    17465 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/resources/llm/client.py
--rw-r--r--   0        0        0       65 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/resources/tool/__init__.py
--rw-r--r--   0        0        0    26029 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/resources/tool/client.py
--rw-r--r--   0        0        0       65 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/resources/vector_database/__init__.py
--rw-r--r--   0        0        0    18052 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/resources/vector_database/client.py
--rw-r--r--   0        0        0       65 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/resources/workflow/__init__.py
--rw-r--r--   0        0        0    43000 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/resources/workflow/client.py
--rw-r--r--   0        0        0       65 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/resources/workflow_config/__init__.py
--rw-r--r--   0        0        0     8456 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/resources/workflow_config/client.py
--rw-r--r--   0        0        0     5337 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/__init__.py
--rw-r--r--   0        0        0     1028 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/agent_datasosurce_list.py
--rw-r--r--   0        0        0     1007 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/agent_list.py
--rw-r--r--   0        0        0     1003 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/agent_tool_list.py
--rw-r--r--   0        0        0      708 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/agent_type.py
--rw-r--r--   0        0        0      977 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/api_key_create.py
--rw-r--r--   0        0        0     1435 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/api_key_create_model.py
--rw-r--r--   0        0        0      991 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/api_key_list.py
--rw-r--r--   0        0        0      879 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/app_models_request_api_key.py
--rw-r--r--   0        0        0     1231 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/app_models_request_api_user.py
--rw-r--r--   0        0        0     1436 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/app_models_request_datasource.py
--rw-r--r--   0        0        0     1042 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/app_models_request_llm.py
--rw-r--r--   0        0        0      989 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/app_models_request_vector_db.py
--rw-r--r--   0        0        0      902 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/app_models_request_workflow.py
--rw-r--r--   0        0        0      984 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/app_models_request_workflow_step.py
--rw-r--r--   0        0        0      986 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/app_models_response_agent.py
--rw-r--r--   0        0        0      934 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/app_models_response_agent_invoke.py
--rw-r--r--   0        0        0      991 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/app_models_response_api_key.py
--rw-r--r--   0        0        0      995 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/app_models_response_api_user.py
--rw-r--r--   0        0        0     1006 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/app_models_response_datasource.py
--rw-r--r--   0        0        0      978 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/app_models_response_llm.py
--rw-r--r--   0        0        0      982 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/app_models_response_tool.py
--rw-r--r--   0        0        0      999 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/app_models_response_vector_db.py
--rw-r--r--   0        0        0      998 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/app_models_response_workflow.py
--rw-r--r--   0        0        0     1015 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/app_models_response_workflow_step.py
--rw-r--r--   0        0        0     1027 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/datasource_list.py
--rw-r--r--   0        0        0      696 2024-04-13 03:51:47.321519 superagent_py-0.2.29/src/superagent/types/datasource_status.py
--rw-r--r--   0        0        0     2649 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/datasource_type.py
--rw-r--r--   0        0        0      560 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/embeddings_model_provider.py
--rw-r--r--   0        0        0     1013 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/function_definition.py
--rw-r--r--   0        0        0      973 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/http_validation_error.py
--rw-r--r--   0        0        0      978 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/llm_list.py
--rw-r--r--   0        0        0     2237 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/llm_model.py
--rw-r--r--   0        0        0      943 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/llm_params.py
--rw-r--r--   0        0        0     1325 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/llm_provider.py
--rw-r--r--   0        0        0     1248 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/open_ai_assistant_parameters.py
--rw-r--r--   0        0        0     1240 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/open_ai_assistant_parameters_tools_item.py
--rw-r--r--   0        0        0     2658 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/prisma_models_agent.py
--rw-r--r--   0        0        0     1560 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/prisma_models_agent_datasource.py
--rw-r--r--   0        0        0     1497 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/prisma_models_agent_llm.py
--rw-r--r--   0        0        0     1506 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/prisma_models_agent_tool.py
--rw-r--r--   0        0        0     1480 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/prisma_models_api_key.py
--rw-r--r--   0        0        0     2497 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/prisma_models_api_user.py
--rw-r--r--   0        0        0     2170 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/prisma_models_datasource.py
--rw-r--r--   0        0        0     1696 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/prisma_models_llm.py
--rw-r--r--   0        0        0     1826 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/prisma_models_tool.py
--rw-r--r--   0        0        0     1687 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/prisma_models_vector_db.py
--rw-r--r--   0        0        0     1814 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/prisma_models_workflow.py
--rw-r--r--   0        0        0     1645 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/prisma_models_workflow_step.py
--rw-r--r--   0        0        0      864 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/tool_assistant_tools_code.py
--rw-r--r--   0        0        0      978 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/tool_assistant_tools_function.py
--rw-r--r--   0        0        0      869 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/tool_assistant_tools_retrieval.py
--rw-r--r--   0        0        0     1003 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/tool_list.py
--rw-r--r--   0        0        0     3767 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/tool_type.py
--rw-r--r--   0        0        0      992 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      999 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/vector_db_list.py
--rw-r--r--   0        0        0     1003 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/vector_db_provider.py
--rw-r--r--   0        0        0     1667 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/workflow_config.py
--rw-r--r--   0        0        0     1019 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/workflow_list.py
--rw-r--r--   0        0        0     1015 2024-04-13 03:51:47.325519 superagent_py-0.2.29/src/superagent/types/workflow_step_list.py
--rw-r--r--   0        0        0     4443 1970-01-01 00:00:00.000000 superagent_py-0.2.29/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-16 04:23:53.937070 superagent_py-0.2.30/LICENSE
+-rw-r--r--   0        0        0     3946 2024-04-16 04:23:53.937070 superagent_py-0.2.30/README.md
+-rw-r--r--   0        0        0      434 2024-04-16 04:23:53.937070 superagent_py-0.2.30/pyproject.toml
+-rw-r--r--   0        0        0     3944 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/__init__.py
+-rw-r--r--   0        0        0     6143 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/client.py
+-rw-r--r--   0        0        0      790 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/core/api_error.py
+-rw-r--r--   0        0        0     1732 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/core/file.py
+-rw-r--r--   0        0        0     4882 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/core/http_client.py
+-rw-r--r--   0        0        0     3799 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/core/request_options.py
+-rw-r--r--   0        0        0      166 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/environment.py
+-rw-r--r--   0        0        0      170 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/py.typed
+-rw-r--r--   0        0        0      333 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/resources/agent/__init__.py
+-rw-r--r--   0        0        0    71786 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/resources/agent/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/resources/api_key/__init__.py
+-rw-r--r--   0        0        0    17585 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/resources/api_key/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/resources/api_user/__init__.py
+-rw-r--r--   0        0        0    17007 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/resources/api_user/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/resources/datasource/__init__.py
+-rw-r--r--   0        0        0    23365 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/resources/datasource/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/resources/llm/__init__.py
+-rw-r--r--   0        0        0    17465 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/resources/llm/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/resources/tool/__init__.py
+-rw-r--r--   0        0        0    26029 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/resources/tool/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/resources/vector_database/__init__.py
+-rw-r--r--   0        0        0    18052 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/resources/vector_database/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/resources/workflow/__init__.py
+-rw-r--r--   0        0        0    43000 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/resources/workflow/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/resources/workflow_config/__init__.py
+-rw-r--r--   0        0        0     8456 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/resources/workflow_config/client.py
+-rw-r--r--   0        0        0     5337 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/__init__.py
+-rw-r--r--   0        0        0     1028 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/agent_datasosurce_list.py
+-rw-r--r--   0        0        0     1007 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/agent_list.py
+-rw-r--r--   0        0        0     1003 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/agent_tool_list.py
+-rw-r--r--   0        0        0      708 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/agent_type.py
+-rw-r--r--   0        0        0      977 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/api_key_create.py
+-rw-r--r--   0        0        0     1435 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/api_key_create_model.py
+-rw-r--r--   0        0        0      991 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/api_key_list.py
+-rw-r--r--   0        0        0      879 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/app_models_request_api_key.py
+-rw-r--r--   0        0        0     1231 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/app_models_request_api_user.py
+-rw-r--r--   0        0        0     1436 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/app_models_request_datasource.py
+-rw-r--r--   0        0        0     1042 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/app_models_request_llm.py
+-rw-r--r--   0        0        0      989 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/app_models_request_vector_db.py
+-rw-r--r--   0        0        0      902 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/app_models_request_workflow.py
+-rw-r--r--   0        0        0      984 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/app_models_request_workflow_step.py
+-rw-r--r--   0        0        0      986 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/app_models_response_agent.py
+-rw-r--r--   0        0        0      934 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/app_models_response_agent_invoke.py
+-rw-r--r--   0        0        0      991 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/app_models_response_api_key.py
+-rw-r--r--   0        0        0      995 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/app_models_response_api_user.py
+-rw-r--r--   0        0        0     1006 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/app_models_response_datasource.py
+-rw-r--r--   0        0        0      978 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/app_models_response_llm.py
+-rw-r--r--   0        0        0      982 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/app_models_response_tool.py
+-rw-r--r--   0        0        0      999 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/app_models_response_vector_db.py
+-rw-r--r--   0        0        0      998 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/app_models_response_workflow.py
+-rw-r--r--   0        0        0     1015 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/app_models_response_workflow_step.py
+-rw-r--r--   0        0        0     1027 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/datasource_list.py
+-rw-r--r--   0        0        0      696 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/datasource_status.py
+-rw-r--r--   0        0        0     2649 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/datasource_type.py
+-rw-r--r--   0        0        0      560 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/embeddings_model_provider.py
+-rw-r--r--   0        0        0     1013 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/function_definition.py
+-rw-r--r--   0        0        0      973 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/http_validation_error.py
+-rw-r--r--   0        0        0      978 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/llm_list.py
+-rw-r--r--   0        0        0     2237 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/llm_model.py
+-rw-r--r--   0        0        0      943 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/llm_params.py
+-rw-r--r--   0        0        0     1325 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/llm_provider.py
+-rw-r--r--   0        0        0     1248 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/open_ai_assistant_parameters.py
+-rw-r--r--   0        0        0     1240 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/open_ai_assistant_parameters_tools_item.py
+-rw-r--r--   0        0        0     2658 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/prisma_models_agent.py
+-rw-r--r--   0        0        0     1560 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/prisma_models_agent_datasource.py
+-rw-r--r--   0        0        0     1497 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/prisma_models_agent_llm.py
+-rw-r--r--   0        0        0     1506 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/prisma_models_agent_tool.py
+-rw-r--r--   0        0        0     1480 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/prisma_models_api_key.py
+-rw-r--r--   0        0        0     2497 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/prisma_models_api_user.py
+-rw-r--r--   0        0        0     2170 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/prisma_models_datasource.py
+-rw-r--r--   0        0        0     1696 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/prisma_models_llm.py
+-rw-r--r--   0        0        0     1826 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/prisma_models_tool.py
+-rw-r--r--   0        0        0     1687 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/prisma_models_vector_db.py
+-rw-r--r--   0        0        0     1814 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/prisma_models_workflow.py
+-rw-r--r--   0        0        0     1645 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/prisma_models_workflow_step.py
+-rw-r--r--   0        0        0      864 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/tool_assistant_tools_code.py
+-rw-r--r--   0        0        0      978 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/tool_assistant_tools_function.py
+-rw-r--r--   0        0        0      869 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/tool_assistant_tools_retrieval.py
+-rw-r--r--   0        0        0     1003 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/tool_list.py
+-rw-r--r--   0        0        0     3767 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/tool_type.py
+-rw-r--r--   0        0        0      992 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      999 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/vector_db_list.py
+-rw-r--r--   0        0        0     1003 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/vector_db_provider.py
+-rw-r--r--   0        0        0     1667 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/workflow_config.py
+-rw-r--r--   0        0        0     1019 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/workflow_list.py
+-rw-r--r--   0        0        0     1015 2024-04-16 04:23:53.937070 superagent_py-0.2.30/src/superagent/types/workflow_step_list.py
+-rw-r--r--   0        0        0     4443 1970-01-01 00:00:00.000000 superagent_py-0.2.30/PKG-INFO
```

### Comparing `superagent_py-0.2.29/LICENSE` & `superagent_py-0.2.30/LICENSE`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/README.md` & `superagent_py-0.2.30/README.md`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/__init__.py` & `superagent_py-0.2.30/src/superagent/__init__.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/client.py` & `superagent_py-0.2.30/src/superagent/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/core/__init__.py` & `superagent_py-0.2.30/src/superagent/core/__init__.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/core/client_wrapper.py` & `superagent_py-0.2.30/src/superagent/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self._token = token
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "superagent-py",
-            "X-Fern-SDK-Version": "v0.2.29",
+            "X-Fern-SDK-Version": "v0.2.30",
         }
         token = self._get_token()
         if token is not None:
             headers["Authorization"] = f"Bearer {token}"
         return headers
 
     def _get_token(self) -> typing.Optional[str]:
```

### Comparing `superagent_py-0.2.29/src/superagent/core/datetime_utils.py` & `superagent_py-0.2.30/src/superagent/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/core/file.py` & `superagent_py-0.2.30/src/superagent/core/file.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/core/http_client.py` & `superagent_py-0.2.30/src/superagent/core/http_client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/core/jsonable_encoder.py` & `superagent_py-0.2.30/src/superagent/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/core/request_options.py` & `superagent_py-0.2.30/src/superagent/core/request_options.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/resources/agent/client.py` & `superagent_py-0.2.30/src/superagent/resources/agent/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/resources/api_key/client.py` & `superagent_py-0.2.30/src/superagent/resources/api_key/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/resources/api_user/client.py` & `superagent_py-0.2.30/src/superagent/resources/api_user/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/resources/datasource/client.py` & `superagent_py-0.2.30/src/superagent/resources/datasource/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/resources/llm/client.py` & `superagent_py-0.2.30/src/superagent/resources/llm/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/resources/tool/client.py` & `superagent_py-0.2.30/src/superagent/resources/tool/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/resources/vector_database/client.py` & `superagent_py-0.2.30/src/superagent/resources/vector_database/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/resources/workflow/client.py` & `superagent_py-0.2.30/src/superagent/resources/workflow/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/resources/workflow_config/client.py` & `superagent_py-0.2.30/src/superagent/resources/workflow_config/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/__init__.py` & `superagent_py-0.2.30/src/superagent/types/__init__.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/agent_datasosurce_list.py` & `superagent_py-0.2.30/src/superagent/types/agent_datasosurce_list.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/agent_list.py` & `superagent_py-0.2.30/src/superagent/types/agent_list.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/agent_tool_list.py` & `superagent_py-0.2.30/src/superagent/types/agent_tool_list.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/agent_type.py` & `superagent_py-0.2.30/src/superagent/types/agent_type.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/api_key_create.py` & `superagent_py-0.2.30/src/superagent/types/api_key_create.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/api_key_create_model.py` & `superagent_py-0.2.30/src/superagent/types/api_key_create_model.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/api_key_list.py` & `superagent_py-0.2.30/src/superagent/types/api_key_list.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/app_models_request_api_key.py` & `superagent_py-0.2.30/src/superagent/types/app_models_request_api_key.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/app_models_request_api_user.py` & `superagent_py-0.2.30/src/superagent/types/app_models_request_api_user.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/app_models_request_datasource.py` & `superagent_py-0.2.30/src/superagent/types/app_models_request_datasource.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/app_models_request_llm.py` & `superagent_py-0.2.30/src/superagent/types/app_models_request_llm.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/app_models_request_vector_db.py` & `superagent_py-0.2.30/src/superagent/types/app_models_request_vector_db.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/app_models_request_workflow.py` & `superagent_py-0.2.30/src/superagent/types/app_models_request_workflow.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/app_models_request_workflow_step.py` & `superagent_py-0.2.30/src/superagent/types/app_models_request_workflow_step.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/app_models_response_agent.py` & `superagent_py-0.2.30/src/superagent/types/app_models_response_agent.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/app_models_response_agent_invoke.py` & `superagent_py-0.2.30/src/superagent/types/app_models_response_agent_invoke.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/app_models_response_api_key.py` & `superagent_py-0.2.30/src/superagent/types/app_models_response_api_key.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/app_models_response_api_user.py` & `superagent_py-0.2.30/src/superagent/types/app_models_response_api_user.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/app_models_response_datasource.py` & `superagent_py-0.2.30/src/superagent/types/app_models_response_datasource.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/app_models_response_llm.py` & `superagent_py-0.2.30/src/superagent/types/app_models_response_llm.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/app_models_response_tool.py` & `superagent_py-0.2.30/src/superagent/types/app_models_response_tool.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/app_models_response_vector_db.py` & `superagent_py-0.2.30/src/superagent/types/app_models_response_vector_db.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/app_models_response_workflow.py` & `superagent_py-0.2.30/src/superagent/types/app_models_response_workflow.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/app_models_response_workflow_step.py` & `superagent_py-0.2.30/src/superagent/types/app_models_response_workflow_step.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/datasource_list.py` & `superagent_py-0.2.30/src/superagent/types/datasource_list.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/datasource_status.py` & `superagent_py-0.2.30/src/superagent/types/datasource_status.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/datasource_type.py` & `superagent_py-0.2.30/src/superagent/types/datasource_type.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/embeddings_model_provider.py` & `superagent_py-0.2.30/src/superagent/types/embeddings_model_provider.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/function_definition.py` & `superagent_py-0.2.30/src/superagent/types/function_definition.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/http_validation_error.py` & `superagent_py-0.2.30/src/superagent/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/llm_list.py` & `superagent_py-0.2.30/src/superagent/types/llm_list.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/llm_model.py` & `superagent_py-0.2.30/src/superagent/types/llm_model.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/llm_params.py` & `superagent_py-0.2.30/src/superagent/types/llm_params.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/llm_provider.py` & `superagent_py-0.2.30/src/superagent/types/llm_provider.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/open_ai_assistant_parameters.py` & `superagent_py-0.2.30/src/superagent/types/open_ai_assistant_parameters.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/open_ai_assistant_parameters_tools_item.py` & `superagent_py-0.2.30/src/superagent/types/open_ai_assistant_parameters_tools_item.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/prisma_models_agent.py` & `superagent_py-0.2.30/src/superagent/types/prisma_models_agent.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/prisma_models_agent_datasource.py` & `superagent_py-0.2.30/src/superagent/types/prisma_models_agent_datasource.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/prisma_models_agent_llm.py` & `superagent_py-0.2.30/src/superagent/types/prisma_models_agent_llm.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/prisma_models_agent_tool.py` & `superagent_py-0.2.30/src/superagent/types/prisma_models_agent_tool.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/prisma_models_api_key.py` & `superagent_py-0.2.30/src/superagent/types/prisma_models_api_key.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/prisma_models_api_user.py` & `superagent_py-0.2.30/src/superagent/types/prisma_models_api_user.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/prisma_models_datasource.py` & `superagent_py-0.2.30/src/superagent/types/prisma_models_datasource.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/prisma_models_llm.py` & `superagent_py-0.2.30/src/superagent/types/prisma_models_llm.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/prisma_models_tool.py` & `superagent_py-0.2.30/src/superagent/types/prisma_models_tool.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/prisma_models_vector_db.py` & `superagent_py-0.2.30/src/superagent/types/prisma_models_vector_db.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/prisma_models_workflow.py` & `superagent_py-0.2.30/src/superagent/types/prisma_models_workflow.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/prisma_models_workflow_step.py` & `superagent_py-0.2.30/src/superagent/types/prisma_models_workflow_step.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/tool_assistant_tools_code.py` & `superagent_py-0.2.30/src/superagent/types/tool_assistant_tools_code.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/tool_assistant_tools_function.py` & `superagent_py-0.2.30/src/superagent/types/tool_assistant_tools_function.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/tool_assistant_tools_retrieval.py` & `superagent_py-0.2.30/src/superagent/types/tool_assistant_tools_retrieval.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/tool_list.py` & `superagent_py-0.2.30/src/superagent/types/tool_list.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/tool_type.py` & `superagent_py-0.2.30/src/superagent/types/tool_type.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/validation_error.py` & `superagent_py-0.2.30/src/superagent/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/vector_db_list.py` & `superagent_py-0.2.30/src/superagent/types/vector_db_list.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/vector_db_provider.py` & `superagent_py-0.2.30/src/superagent/types/vector_db_provider.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/workflow_config.py` & `superagent_py-0.2.30/src/superagent/types/workflow_config.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/workflow_list.py` & `superagent_py-0.2.30/src/superagent/types/workflow_list.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/src/superagent/types/workflow_step_list.py` & `superagent_py-0.2.30/src/superagent/types/workflow_step_list.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.2.29/PKG-INFO` & `superagent_py-0.2.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superagent-py
-Version: 0.2.29
+Version: 0.2.30
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

