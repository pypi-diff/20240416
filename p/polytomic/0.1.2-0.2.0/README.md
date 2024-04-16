# Comparing `tmp/polytomic-0.1.2.tar.gz` & `tmp/polytomic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polytomic-0.1.2.tar", max compression
+gzip compressed data, was "polytomic-0.2.0.tar", max compression
```

## Comparing `polytomic-0.1.2.tar` & `polytomic-0.2.0.tar`

### file list

```diff
@@ -1,181 +1,192 @@
--rw-r--r--   0        0        0     1066 2024-04-04 02:07:02.834260 polytomic-0.1.2/LICENSE
--rw-r--r--   0        0        0     1868 2024-04-04 02:07:02.834260 polytomic-0.1.2/README.md
--rw-r--r--   0        0        0      596 2024-04-04 02:07:02.834260 polytomic-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6967 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/__init__.py
--rw-r--r--   0        0        0     7571 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/client.py
--rw-r--r--   0        0        0      790 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/core/api_error.py
--rw-r--r--   0        0        0     2558 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/core/request_options.py
--rw-r--r--   0        0        0      152 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/environment.py
--rw-r--r--   0        0        0      148 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/errors/__init__.py
--rw-r--r--   0        0        0      286 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/errors/unauthorized_error.py
--rw-r--r--   0        0        0        0 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/py.typed
--rw-r--r--   0        0        0      430 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/__init__.py
--rw-r--r--   0        0        0      145 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/bulk_sync/__init__.py
--rw-r--r--   0        0        0    70925 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/bulk_sync/client.py
--rw-r--r--   0        0        0      136 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/bulk_sync/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/bulk_sync/resources/executions/__init__.py
--rw-r--r--   0        0        0    17013 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/bulk_sync/resources/executions/client.py
--rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/bulk_sync/resources/schemas/__init__.py
--rw-r--r--   0        0        0    18162 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/bulk_sync/resources/schemas/client.py
--rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/connections/__init__.py
--rw-r--r--   0        0        0    65762 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/connections/client.py
--rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/events/__init__.py
--rw-r--r--   0        0        0    12416 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/events/client.py
--rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/jobs/__init__.py
--rw-r--r--   0        0        0     5572 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/jobs/client.py
--rw-r--r--   0        0        0      125 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/model_sync/__init__.py
--rw-r--r--   0        0        0    58565 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/model_sync/client.py
--rw-r--r--   0        0        0      116 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/model_sync/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/model_sync/resources/executions/__init__.py
--rw-r--r--   0        0        0    59453 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/model_sync/resources/executions/client.py
--rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/models/__init__.py
--rw-r--r--   0        0        0    34659 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/models/client.py
--rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/organization/__init__.py
--rw-r--r--   0        0        0    30862 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/organization/client.py
--rw-r--r--   0        0        0      137 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/permissions/__init__.py
--rw-r--r--   0        0        0      849 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/permissions/client.py
--rw-r--r--   0        0        0      128 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/permissions/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/permissions/resources/policies/__init__.py
--rw-r--r--   0        0        0    27695 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/permissions/resources/policies/client.py
--rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/permissions/resources/roles/__init__.py
--rw-r--r--   0        0        0    25551 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/permissions/resources/roles/client.py
--rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/schemas/__init__.py
--rw-r--r--   0        0        0     5861 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/schemas/client.py
--rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/users/__init__.py
--rw-r--r--   0        0        0    35157 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/users/client.py
--rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/webhooks/__init__.py
--rw-r--r--   0        0        0    28121 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/webhooks/client.py
--rw-r--r--   0        0        0    10037 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/__init__.py
--rw-r--r--   0        0        0      998 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/activate_sync_envelope.py
--rw-r--r--   0        0        0      906 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/activate_sync_input.py
--rw-r--r--   0        0        0      967 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/activate_sync_output.py
--rw-r--r--   0        0        0      925 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/api_key_response.py
--rw-r--r--   0        0        0      988 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/api_key_response_envelope.py
--rw-r--r--   0        0        0      851 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_discover.py
--rw-r--r--   0        0        0     1756 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_execution_status.py
--rw-r--r--   0        0        0     1004 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_field.py
--rw-r--r--   0        0        0     1134 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_itemized_schedule.py
--rw-r--r--   0        0        0     1152 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_multi_schedule_configuration.py
--rw-r--r--   0        0        0     1407 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_schedule.py
--rw-r--r--   0        0        0     1145 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_schema.py
--rw-r--r--   0        0        0      971 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_schema_envelope.py
--rw-r--r--   0        0        0     1337 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_schema_execution_status.py
--rw-r--r--   0        0        0      763 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_selective_mode.py
--rw-r--r--   0        0        0     1060 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_dest.py
--rw-r--r--   0        0        0      980 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_dest_envelope.py
--rw-r--r--   0        0        0     1456 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_execution.py
--rw-r--r--   0        0        0     1000 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_execution_envelope.py
--rw-r--r--   0        0        0     1005 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_list_envelope.py
--rw-r--r--   0        0        0     1555 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_response.py
--rw-r--r--   0        0        0      996 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_response_envelope.py
--rw-r--r--   0        0        0     1429 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_schema_execution.py
--rw-r--r--   0        0        0     1024 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_source.py
--rw-r--r--   0        0        0      988 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_source_envelope.py
--rw-r--r--   0        0        0      968 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_source_schema_envelope.py
--rw-r--r--   0        0        0     1063 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_source_status.py
--rw-r--r--   0        0        0     1013 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_source_status_envelope.py
--rw-r--r--   0        0        0     1013 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_status_envelope.py
--rw-r--r--   0        0        0     1133 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_status_response.py
--rw-r--r--   0        0        0      987 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/configuration_value.py
--rw-r--r--   0        0        0      976 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connect_card_response.py
--rw-r--r--   0        0        0     1008 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connect_card_response_envelope.py
--rw-r--r--   0        0        0     1039 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connection_list_response_envelope.py
--rw-r--r--   0        0        0     1051 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connection_meta.py
--rw-r--r--   0        0        0     1217 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connection_meta_response.py
--rw-r--r--   0        0        0      981 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connection_parameter_value.py
--rw-r--r--   0        0        0     1090 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connection_parameter_values_resp.py
--rw-r--r--   0        0        0     1088 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connection_parameter_values_response_envelope.py
--rw-r--r--   0        0        0     1022 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connection_response_envelope.py
--rw-r--r--   0        0        0     1344 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connection_response_schema.py
--rw-r--r--   0        0        0     1194 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connection_type.py
--rw-r--r--   0        0        0     1008 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connection_type_response_envelope.py
--rw-r--r--   0        0        0     1023 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connection_type_schema.py
--rw-r--r--   0        0        0     1047 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/create_connection_response_envelope.py
--rw-r--r--   0        0        0     1639 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/create_connection_response_schema.py
--rw-r--r--   0        0        0     1098 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/event.py
--rw-r--r--   0        0        0      941 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/event_types_envelope.py
--rw-r--r--   0        0        0      964 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/events_envelope.py
--rw-r--r--   0        0        0     1045 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/execution_counts.py
--rw-r--r--   0        0        0      992 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/execution_log_response.py
--rw-r--r--   0        0        0     1013 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/execution_logs_response_envelope.py
--rw-r--r--   0        0        0     1867 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/execution_status.py
--rw-r--r--   0        0        0     1019 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/filter.py
--rw-r--r--   0        0        0     1015 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/get_connection_meta_envelope.py
--rw-r--r--   0        0        0     1031 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/get_execution_response_envelope.py
--rw-r--r--   0        0        0     1379 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/get_execution_response_schema.py
--rw-r--r--   0        0        0     1027 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/get_identity_response_envelope.py
--rw-r--r--   0        0        0     1291 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/get_identity_response_schema.py
--rw-r--r--   0        0        0     1058 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/identity.py
--rw-r--r--   0        0        0      963 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/identity_function.py
--rw-r--r--   0        0        0     1143 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/job_response.py
--rw-r--r--   0        0        0      975 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/job_response_envelope.py
--rw-r--r--   0        0        0      118 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/jsonschema_form.py
--rw-r--r--   0        0        0      114 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/label_label.py
--rw-r--r--   0        0        0      980 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/list_bulk_schema.py
--rw-r--r--   0        0        0     1018 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/list_bulk_sync_executions_envelope.py
--rw-r--r--   0        0        0     1045 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/list_execution_response_envelope.py
--rw-r--r--   0        0        0     1017 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/list_model_sync_response_envelope.py
--rw-r--r--   0        0        0     1006 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/list_policies_response_envelope.py
--rw-r--r--   0        0        0      964 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/list_users_envelope.py
--rw-r--r--   0        0        0     1167 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/mode.py
--rw-r--r--   0        0        0     1221 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/model_field.py
--rw-r--r--   0        0        0      984 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/model_field_response.py
--rw-r--r--   0        0        0     1000 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/model_list_response_envelope.py
--rw-r--r--   0        0        0      978 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/model_model_field_request.py
--rw-r--r--   0        0        0     1135 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/model_relation.py
--rw-r--r--   0        0        0      968 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/model_relation_to.py
--rw-r--r--   0        0        0     1652 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/model_response.py
--rw-r--r--   0        0        0     1066 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/model_response_envelope.py
--rw-r--r--   0        0        0     1077 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/model_sync_field.py
--rw-r--r--   0        0        0     1827 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/model_sync_response.py
--rw-r--r--   0        0        0     1000 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/model_sync_response_envelope.py
--rw-r--r--   0        0        0     1086 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/organization.py
--rw-r--r--   0        0        0      978 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/organization_envelope.py
--rw-r--r--   0        0        0      992 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/organizations_envelope.py
--rw-r--r--   0        0        0     1059 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/override.py
--rw-r--r--   0        0        0      959 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/pick_value.py
--rw-r--r--   0        0        0      955 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/policy_action.py
--rw-r--r--   0        0        0     1160 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/policy_response.py
--rw-r--r--   0        0        0      987 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/policy_response_envelope.py
--rw-r--r--   0        0        0     1114 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/relation.py
--rw-r--r--   0        0        0      963 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/relation_to.py
--rw-r--r--   0        0        0     1331 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/rest_err_response.py
--rw-r--r--   0        0        0      996 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/role_list_response_envelope.py
--rw-r--r--   0        0        0     1048 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/role_response.py
--rw-r--r--   0        0        0      979 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/role_response_envelope.py
--rw-r--r--   0        0        0      995 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/run_after.py
--rw-r--r--   0        0        0     1298 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/schedule.py
--rw-r--r--   0        0        0     1669 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/schedule_frequency.py
--rw-r--r--   0        0        0     1037 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/schedule_option_response.py
--rw-r--r--   0        0        0     1020 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/schedule_option_response_envelope.py
--rw-r--r--   0        0        0     1187 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/schedule_schedule_option.py
--rw-r--r--   0        0        0     1051 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/schema.py
--rw-r--r--   0        0        0     1072 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/schema_association.py
--rw-r--r--   0        0        0     1242 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/schema_field.py
--rw-r--r--   0        0        0      977 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/schema_records_response_envelope.py
--rw-r--r--   0        0        0      911 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/source.py
--rw-r--r--   0        0        0     1040 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/start_model_sync_response_envelope.py
--rw-r--r--   0        0        0     1086 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/start_model_sync_response_schema.py
--rw-r--r--   0        0        0     1220 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/supported_mode.py
--rw-r--r--   0        0        0     1476 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/sync_destination_properties.py
--rw-r--r--   0        0        0      996 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/sync_status_envelope.py
--rw-r--r--   0        0        0     1166 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/sync_status_response.py
--rw-r--r--   0        0        0     1149 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/target.py
--rw-r--r--   0        0        0     1487 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/target_field.py
--rw-r--r--   0        0        0     1322 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/target_response.py
--rw-r--r--   0        0        0      987 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/target_response_envelope.py
--rw-r--r--   0        0        0     1038 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/user.py
--rw-r--r--   0        0        0      946 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/user_envelope.py
--rw-r--r--   0        0        0     1098 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/webhook.py
--rw-r--r--   0        0        0      958 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/webhook_envelope.py
--rw-r--r--   0        0        0      975 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/webhook_list_envelope.py
--rw-r--r--   0        0        0      623 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/work_task_status.py
--rw-r--r--   0        0        0       77 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/version.py
--rw-r--r--   0        0        0     2360 1970-01-01 00:00:00.000000 polytomic-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-16 17:49:36.865207 polytomic-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1764 2024-04-16 17:49:36.865207 polytomic-0.2.0/README.md
+-rw-r--r--   0        0        0      596 2024-04-16 17:49:36.869207 polytomic-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7452 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/__init__.py
+-rw-r--r--   0        0        0     7179 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/client.py
+-rw-r--r--   0        0        0      790 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/core/api_error.py
+-rw-r--r--   0        0        0     1936 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/core/http_client.py
+-rw-r--r--   0        0        0     3799 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/core/request_options.py
+-rw-r--r--   0        0        0      152 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/environment.py
+-rw-r--r--   0        0        0      534 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/errors/__init__.py
+-rw-r--r--   0        0        0      348 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/errors/bad_request_error.py
+-rw-r--r--   0        0        0      347 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/errors/forbidden_error.py
+-rw-r--r--   0        0        0      352 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/errors/internal_server_error.py
+-rw-r--r--   0        0        0      346 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/errors/not_found_error.py
+-rw-r--r--   0        0        0      286 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      357 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/py.typed
+-rw-r--r--   0        0        0      460 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/bulk_sync/__init__.py
+-rw-r--r--   0        0        0    75561 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/bulk_sync/client.py
+-rw-r--r--   0        0        0      136 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/bulk_sync/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/bulk_sync/resources/executions/__init__.py
+-rw-r--r--   0        0        0    11087 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/bulk_sync/resources/executions/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/bulk_sync/resources/schemas/__init__.py
+-rw-r--r--   0        0        0    26486 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/bulk_sync/resources/schemas/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/connections/__init__.py
+-rw-r--r--   0        0        0    54184 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/connections/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/events/__init__.py
+-rw-r--r--   0        0        0    13121 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/events/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/identity/__init__.py
+-rw-r--r--   0        0        0     5538 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/identity/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/jobs/__init__.py
+-rw-r--r--   0        0        0     6731 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/jobs/client.py
+-rw-r--r--   0        0        0      125 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/model_sync/__init__.py
+-rw-r--r--   0        0        0    92987 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/model_sync/client.py
+-rw-r--r--   0        0        0      116 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/model_sync/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/model_sync/resources/executions/__init__.py
+-rw-r--r--   0        0        0    23586 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/model_sync/resources/executions/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/models/__init__.py
+-rw-r--r--   0        0        0    38479 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/models/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/organization/__init__.py
+-rw-r--r--   0        0        0    33551 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/organization/client.py
+-rw-r--r--   0        0        0      137 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/permissions/__init__.py
+-rw-r--r--   0        0        0      849 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/permissions/client.py
+-rw-r--r--   0        0        0      128 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/permissions/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/permissions/resources/policies/__init__.py
+-rw-r--r--   0        0        0    32163 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/permissions/resources/policies/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/permissions/resources/roles/__init__.py
+-rw-r--r--   0        0        0    29695 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/permissions/resources/roles/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/schemas/__init__.py
+-rw-r--r--   0        0        0    24085 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/schemas/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/users/__init__.py
+-rw-r--r--   0        0        0    38734 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/users/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/webhooks/__init__.py
+-rw-r--r--   0        0        0    30810 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/resources/webhooks/client.py
+-rw-r--r--   0        0        0    10365 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/__init__.py
+-rw-r--r--   0        0        0      998 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/activate_sync_envelope.py
+-rw-r--r--   0        0        0      906 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/activate_sync_input.py
+-rw-r--r--   0        0        0      967 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/activate_sync_output.py
+-rw-r--r--   0        0        0     1010 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/api_error.py
+-rw-r--r--   0        0        0      925 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/api_key_response.py
+-rw-r--r--   0        0        0      988 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/api_key_response_envelope.py
+-rw-r--r--   0        0        0      851 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_discover.py
+-rw-r--r--   0        0        0     1756 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_execution_status.py
+-rw-r--r--   0        0        0     1004 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_field.py
+-rw-r--r--   0        0        0     1134 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_itemized_schedule.py
+-rw-r--r--   0        0        0     1152 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_multi_schedule_configuration.py
+-rw-r--r--   0        0        0     1407 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_schedule.py
+-rw-r--r--   0        0        0     1145 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_schema.py
+-rw-r--r--   0        0        0      971 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_schema_envelope.py
+-rw-r--r--   0        0        0     1337 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_schema_execution_status.py
+-rw-r--r--   0        0        0      763 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_selective_mode.py
+-rw-r--r--   0        0        0     1060 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_dest.py
+-rw-r--r--   0        0        0      980 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_dest_envelope.py
+-rw-r--r--   0        0        0     1456 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_execution.py
+-rw-r--r--   0        0        0     1000 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_execution_envelope.py
+-rw-r--r--   0        0        0     1005 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_list_envelope.py
+-rw-r--r--   0        0        0     1555 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_response.py
+-rw-r--r--   0        0        0      996 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_response_envelope.py
+-rw-r--r--   0        0        0     1429 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_schema_execution.py
+-rw-r--r--   0        0        0     1024 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_source.py
+-rw-r--r--   0        0        0      988 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_source_envelope.py
+-rw-r--r--   0        0        0      968 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_source_schema_envelope.py
+-rw-r--r--   0        0        0     1063 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_source_status.py
+-rw-r--r--   0        0        0     1013 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_source_status_envelope.py
+-rw-r--r--   0        0        0     1013 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_status_envelope.py
+-rw-r--r--   0        0        0     1133 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/bulk_sync_status_response.py
+-rw-r--r--   0        0        0      987 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/configuration_value.py
+-rw-r--r--   0        0        0      976 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connect_card_response.py
+-rw-r--r--   0        0        0     1008 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connect_card_response_envelope.py
+-rw-r--r--   0        0        0     1039 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connection_list_response_envelope.py
+-rw-r--r--   0        0        0     1051 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connection_meta.py
+-rw-r--r--   0        0        0     1217 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connection_meta_response.py
+-rw-r--r--   0        0        0      981 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connection_parameter_value.py
+-rw-r--r--   0        0        0     1090 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connection_parameter_values_resp.py
+-rw-r--r--   0        0        0     1088 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connection_parameter_values_response_envelope.py
+-rw-r--r--   0        0        0     1022 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connection_response_envelope.py
+-rw-r--r--   0        0        0     1344 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connection_response_schema.py
+-rw-r--r--   0        0        0     1194 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connection_type.py
+-rw-r--r--   0        0        0     1008 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connection_type_response_envelope.py
+-rw-r--r--   0        0        0     1023 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/connection_type_schema.py
+-rw-r--r--   0        0        0     1047 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/create_connection_response_envelope.py
+-rw-r--r--   0        0        0     1639 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/create_connection_response_schema.py
+-rw-r--r--   0        0        0     1098 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/event.py
+-rw-r--r--   0        0        0      941 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/event_types_envelope.py
+-rw-r--r--   0        0        0      964 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/events_envelope.py
+-rw-r--r--   0        0        0     1045 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/execution_counts.py
+-rw-r--r--   0        0        0      992 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/execution_log_response.py
+-rw-r--r--   0        0        0     1013 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/execution_logs_response_envelope.py
+-rw-r--r--   0        0        0     1867 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/execution_status.py
+-rw-r--r--   0        0        0     1019 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/filter.py
+-rw-r--r--   0        0        0     1015 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/get_connection_meta_envelope.py
+-rw-r--r--   0        0        0     1031 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/get_execution_response_envelope.py
+-rw-r--r--   0        0        0     1379 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/get_execution_response_schema.py
+-rw-r--r--   0        0        0     1027 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/get_identity_response_envelope.py
+-rw-r--r--   0        0        0     1291 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/get_identity_response_schema.py
+-rw-r--r--   0        0        0     1037 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/get_model_sync_source_meta_envelope.py
+-rw-r--r--   0        0        0     1058 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/identity.py
+-rw-r--r--   0        0        0      963 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/identity_function.py
+-rw-r--r--   0        0        0     1143 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/job_response.py
+-rw-r--r--   0        0        0      975 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/job_response_envelope.py
+-rw-r--r--   0        0        0      118 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/jsonschema_form.py
+-rw-r--r--   0        0        0      114 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/label_label.py
+-rw-r--r--   0        0        0      980 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/list_bulk_schema.py
+-rw-r--r--   0        0        0     1018 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/list_bulk_sync_executions_envelope.py
+-rw-r--r--   0        0        0     1045 2024-04-16 17:49:36.869207 polytomic-0.2.0/src/polytomic/types/list_execution_response_envelope.py
+-rw-r--r--   0        0        0     1017 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/list_model_sync_response_envelope.py
+-rw-r--r--   0        0        0     1006 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/list_policies_response_envelope.py
+-rw-r--r--   0        0        0      964 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/list_users_envelope.py
+-rw-r--r--   0        0        0     1167 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/mode.py
+-rw-r--r--   0        0        0     1221 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_field.py
+-rw-r--r--   0        0        0      984 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_field_response.py
+-rw-r--r--   0        0        0     1000 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_list_response_envelope.py
+-rw-r--r--   0        0        0      978 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_model_field_request.py
+-rw-r--r--   0        0        0     1135 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_relation.py
+-rw-r--r--   0        0        0      968 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_relation_to.py
+-rw-r--r--   0        0        0     1652 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_response.py
+-rw-r--r--   0        0        0     1066 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_response_envelope.py
+-rw-r--r--   0        0        0     1077 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_sync_field.py
+-rw-r--r--   0        0        0     1827 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_sync_response.py
+-rw-r--r--   0        0        0     1000 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_sync_response_envelope.py
+-rw-r--r--   0        0        0     1210 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/model_sync_source_meta_response.py
+-rw-r--r--   0        0        0     1086 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/organization.py
+-rw-r--r--   0        0        0      978 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/organization_envelope.py
+-rw-r--r--   0        0        0      992 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/organizations_envelope.py
+-rw-r--r--   0        0        0     1059 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/override.py
+-rw-r--r--   0        0        0      959 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/pick_value.py
+-rw-r--r--   0        0        0      955 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/policy_action.py
+-rw-r--r--   0        0        0     1160 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/policy_response.py
+-rw-r--r--   0        0        0      987 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/policy_response_envelope.py
+-rw-r--r--   0        0        0     1114 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/relation.py
+-rw-r--r--   0        0        0      963 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/relation_to.py
+-rw-r--r--   0        0        0     1331 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/rest_err_response.py
+-rw-r--r--   0        0        0      996 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/role_list_response_envelope.py
+-rw-r--r--   0        0        0     1048 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/role_response.py
+-rw-r--r--   0        0        0      979 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/role_response_envelope.py
+-rw-r--r--   0        0        0      995 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/run_after.py
+-rw-r--r--   0        0        0     1298 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/schedule.py
+-rw-r--r--   0        0        0     1669 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/schedule_frequency.py
+-rw-r--r--   0        0        0     1037 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/schedule_option_response.py
+-rw-r--r--   0        0        0     1020 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/schedule_option_response_envelope.py
+-rw-r--r--   0        0        0     1187 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/schedule_schedule_option.py
+-rw-r--r--   0        0        0     1051 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/schema.py
+-rw-r--r--   0        0        0     1072 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/schema_association.py
+-rw-r--r--   0        0        0     1242 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/schema_field.py
+-rw-r--r--   0        0        0      977 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/schema_records_response_envelope.py
+-rw-r--r--   0        0        0      911 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/source.py
+-rw-r--r--   0        0        0     1047 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/source_meta.py
+-rw-r--r--   0        0        0     1040 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/start_model_sync_response_envelope.py
+-rw-r--r--   0        0        0     1086 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/start_model_sync_response_schema.py
+-rw-r--r--   0        0        0     1220 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/supported_mode.py
+-rw-r--r--   0        0        0     1476 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/sync_destination_properties.py
+-rw-r--r--   0        0        0      996 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/sync_status_envelope.py
+-rw-r--r--   0        0        0     1166 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/sync_status_response.py
+-rw-r--r--   0        0        0     1149 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/target.py
+-rw-r--r--   0        0        0     1487 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/target_field.py
+-rw-r--r--   0        0        0     1322 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/target_response.py
+-rw-r--r--   0        0        0      987 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/target_response_envelope.py
+-rw-r--r--   0        0        0     1038 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/user.py
+-rw-r--r--   0        0        0      946 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/user_envelope.py
+-rw-r--r--   0        0        0     1098 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/webhook.py
+-rw-r--r--   0        0        0      958 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/webhook_envelope.py
+-rw-r--r--   0        0        0      975 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/webhook_list_envelope.py
+-rw-r--r--   0        0        0      623 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/types/work_task_status.py
+-rw-r--r--   0        0        0       77 2024-04-16 17:49:36.873207 polytomic-0.2.0/src/polytomic/version.py
+-rw-r--r--   0        0        0     2256 1970-01-01 00:00:00.000000 polytomic-0.2.0/PKG-INFO
```

### Comparing `polytomic-0.1.2/LICENSE` & `polytomic-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/README.md` & `polytomic-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -17,28 +17,26 @@
 <!-- Begin Usage, generated by Fern  -->
 # Usage
 
 ```python
 from polytomic.client import Polytomic
 
 client = Polytomic(
-    x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
     token="YOUR_TOKEN",
 )
 ```
 <!-- End Usage  -->
 
 <!-- Begin Async Usage, generated by Fern  -->
 # Async Client
 
 ```python
 from polytomic.client import AsyncPolytomic
 
 client = AsyncPolytomic(
-    x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
     token="YOUR_TOKEN",
 )
 ```
 <!-- End Async Usage  -->
 
 <!-- Begin Status, generated by Fern  -->
 # Beta Status
```

### Comparing `polytomic-0.1.2/pyproject.toml` & `polytomic-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polytomic"
-version = "0.1.2"
+version = "0.2.0"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "polytomic", from = "src"}
 ]
```

### Comparing `polytomic-0.1.2/src/polytomic/__init__.py` & `polytomic-0.2.0/src/polytomic/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
     ActivateSyncEnvelope,
     ActivateSyncInput,
     ActivateSyncOutput,
+    ApiError,
     ApiKeyResponse,
     ApiKeyResponseEnvelope,
     BulkDiscover,
     BulkExecutionStatus,
     BulkField,
     BulkItemizedSchedule,
     BulkMultiScheduleConfiguration,
@@ -56,14 +57,15 @@
     ExecutionStatus,
     Filter,
     GetConnectionMetaEnvelope,
     GetExecutionResponseEnvelope,
     GetExecutionResponseSchema,
     GetIdentityResponseEnvelope,
     GetIdentityResponseSchema,
+    GetModelSyncSourceMetaEnvelope,
     Identity,
     IdentityFunction,
     JobResponse,
     JobResponseEnvelope,
     JsonschemaForm,
     LabelLabel,
     ListBulkSchema,
@@ -80,14 +82,15 @@
     ModelRelation,
     ModelRelationTo,
     ModelResponse,
     ModelResponseEnvelope,
     ModelSyncField,
     ModelSyncResponse,
     ModelSyncResponseEnvelope,
+    ModelSyncSourceMetaResponse,
     Organization,
     OrganizationEnvelope,
     OrganizationsEnvelope,
     Override,
     PickValue,
     PolicyAction,
     PolicyResponse,
@@ -105,14 +108,15 @@
     ScheduleOptionResponseEnvelope,
     ScheduleScheduleOption,
     Schema,
     SchemaAssociation,
     SchemaField,
     SchemaRecordsResponseEnvelope,
     Source,
+    SourceMeta,
     StartModelSyncResponseEnvelope,
     StartModelSyncResponseSchema,
     SupportedMode,
     SyncDestinationProperties,
     SyncStatusEnvelope,
     SyncStatusResponse,
     Target,
@@ -122,19 +126,27 @@
     User,
     UserEnvelope,
     Webhook,
     WebhookEnvelope,
     WebhookListEnvelope,
     WorkTaskStatus,
 )
-from .errors import UnauthorizedError
+from .errors import (
+    BadRequestError,
+    ForbiddenError,
+    InternalServerError,
+    NotFoundError,
+    UnauthorizedError,
+    UnprocessableEntityError,
+)
 from .resources import (
     bulk_sync,
     connections,
     events,
+    identity,
     jobs,
     model_sync,
     models,
     organization,
     permissions,
     schemas,
     users,
@@ -143,16 +155,18 @@
 from .environment import PolytomicEnvironment
 from .version import __version__
 
 __all__ = [
     "ActivateSyncEnvelope",
     "ActivateSyncInput",
     "ActivateSyncOutput",
+    "ApiError",
     "ApiKeyResponse",
     "ApiKeyResponseEnvelope",
+    "BadRequestError",
     "BulkDiscover",
     "BulkExecutionStatus",
     "BulkField",
     "BulkItemizedSchedule",
     "BulkMultiScheduleConfiguration",
     "BulkSchedule",
     "BulkSchema",
@@ -194,21 +208,24 @@
     "EventTypesEnvelope",
     "EventsEnvelope",
     "ExecutionCounts",
     "ExecutionLogResponse",
     "ExecutionLogsResponseEnvelope",
     "ExecutionStatus",
     "Filter",
+    "ForbiddenError",
     "GetConnectionMetaEnvelope",
     "GetExecutionResponseEnvelope",
     "GetExecutionResponseSchema",
     "GetIdentityResponseEnvelope",
     "GetIdentityResponseSchema",
+    "GetModelSyncSourceMetaEnvelope",
     "Identity",
     "IdentityFunction",
+    "InternalServerError",
     "JobResponse",
     "JobResponseEnvelope",
     "JsonschemaForm",
     "LabelLabel",
     "ListBulkSchema",
     "ListBulkSyncExecutionsEnvelope",
     "ListExecutionResponseEnvelope",
@@ -223,14 +240,16 @@
     "ModelRelation",
     "ModelRelationTo",
     "ModelResponse",
     "ModelResponseEnvelope",
     "ModelSyncField",
     "ModelSyncResponse",
     "ModelSyncResponseEnvelope",
+    "ModelSyncSourceMetaResponse",
+    "NotFoundError",
     "Organization",
     "OrganizationEnvelope",
     "OrganizationsEnvelope",
     "Override",
     "PickValue",
     "PolicyAction",
     "PolicyResponse",
@@ -249,35 +268,38 @@
     "ScheduleOptionResponseEnvelope",
     "ScheduleScheduleOption",
     "Schema",
     "SchemaAssociation",
     "SchemaField",
     "SchemaRecordsResponseEnvelope",
     "Source",
+    "SourceMeta",
     "StartModelSyncResponseEnvelope",
     "StartModelSyncResponseSchema",
     "SupportedMode",
     "SyncDestinationProperties",
     "SyncStatusEnvelope",
     "SyncStatusResponse",
     "Target",
     "TargetField",
     "TargetResponse",
     "TargetResponseEnvelope",
     "UnauthorizedError",
+    "UnprocessableEntityError",
     "User",
     "UserEnvelope",
     "Webhook",
     "WebhookEnvelope",
     "WebhookListEnvelope",
     "WorkTaskStatus",
     "__version__",
     "bulk_sync",
     "connections",
     "events",
+    "identity",
     "jobs",
     "model_sync",
     "models",
     "organization",
     "permissions",
     "schemas",
     "users",
```

### Comparing `polytomic-0.1.2/src/polytomic/client.py` & `polytomic-0.2.0/src/polytomic/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import httpx
 
 from .core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .environment import PolytomicEnvironment
 from .resources.bulk_sync.client import AsyncBulkSyncClient, BulkSyncClient
 from .resources.connections.client import AsyncConnectionsClient, ConnectionsClient
 from .resources.events.client import AsyncEventsClient, EventsClient
+from .resources.identity.client import AsyncIdentityClient, IdentityClient
 from .resources.jobs.client import AsyncJobsClient, JobsClient
 from .resources.model_sync.client import AsyncModelSyncClient, ModelSyncClient
 from .resources.models.client import AsyncModelsClient, ModelsClient
 from .resources.organization.client import AsyncOrganizationClient, OrganizationClient
 from .resources.permissions.client import AsyncPermissionsClient, PermissionsClient
 from .resources.schemas.client import AsyncSchemasClient, SchemasClient
 from .resources.users.client import AsyncUsersClient, UsersClient
@@ -26,116 +27,108 @@
     Parameters:
         - base_url: typing.Optional[str]. The base url to use for requests from the client.
 
         - environment: PolytomicEnvironment. The environment to use for requests from the client. from .environment import PolytomicEnvironment
 
                                              Defaults to PolytomicEnvironment.DEFAULT
 
-        - x_polytomic_version: typing.Optional[typing.Literal["2023-04-25"]].
-
-        - token: typing.Optional[typing.Union[str, typing.Callable[[], str]]].
+        - token: typing.Union[str, typing.Callable[[], str]].
 
         - timeout: typing.Optional[float]. The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
 
         - httpx_client: typing.Optional[httpx.Client]. The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
     ---
     from polytomic.client import Polytomic
 
     client = Polytomic(
-        x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
         token="YOUR_TOKEN",
     )
     """
 
     def __init__(
         self,
         *,
         base_url: typing.Optional[str] = None,
         environment: PolytomicEnvironment = PolytomicEnvironment.DEFAULT,
-        x_polytomic_version: typing.Optional[typing.Literal["2023-04-25"]] = None,
-        token: typing.Optional[typing.Union[str, typing.Callable[[], str]]] = None,
+        token: typing.Union[str, typing.Callable[[], str]],
         timeout: typing.Optional[float] = None,
         httpx_client: typing.Optional[httpx.Client] = None
     ):
         _defaulted_timeout = timeout if timeout is not None else 60 if httpx_client is None else None
         self._client_wrapper = SyncClientWrapper(
             base_url=_get_base_url(base_url=base_url, environment=environment),
-            x_polytomic_version=x_polytomic_version,
             token=token,
             httpx_client=httpx.Client(timeout=_defaulted_timeout) if httpx_client is None else httpx_client,
             timeout=_defaulted_timeout,
         )
         self.bulk_sync = BulkSyncClient(client_wrapper=self._client_wrapper)
         self.connections = ConnectionsClient(client_wrapper=self._client_wrapper)
+        self.model_sync = ModelSyncClient(client_wrapper=self._client_wrapper)
         self.schemas = SchemasClient(client_wrapper=self._client_wrapper)
         self.events = EventsClient(client_wrapper=self._client_wrapper)
         self.jobs = JobsClient(client_wrapper=self._client_wrapper)
+        self.identity = IdentityClient(client_wrapper=self._client_wrapper)
         self.models = ModelsClient(client_wrapper=self._client_wrapper)
         self.organization = OrganizationClient(client_wrapper=self._client_wrapper)
         self.users = UsersClient(client_wrapper=self._client_wrapper)
         self.permissions = PermissionsClient(client_wrapper=self._client_wrapper)
-        self.model_sync = ModelSyncClient(client_wrapper=self._client_wrapper)
         self.webhooks = WebhooksClient(client_wrapper=self._client_wrapper)
 
 
 class AsyncPolytomic:
     """
     Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
 
     Parameters:
         - base_url: typing.Optional[str]. The base url to use for requests from the client.
 
         - environment: PolytomicEnvironment. The environment to use for requests from the client. from .environment import PolytomicEnvironment
 
                                              Defaults to PolytomicEnvironment.DEFAULT
 
-        - x_polytomic_version: typing.Optional[typing.Literal["2023-04-25"]].
-
-        - token: typing.Optional[typing.Union[str, typing.Callable[[], str]]].
+        - token: typing.Union[str, typing.Callable[[], str]].
 
         - timeout: typing.Optional[float]. The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
 
         - httpx_client: typing.Optional[httpx.AsyncClient]. The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
     ---
     from polytomic.client import AsyncPolytomic
 
     client = AsyncPolytomic(
-        x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
         token="YOUR_TOKEN",
     )
     """
 
     def __init__(
         self,
         *,
         base_url: typing.Optional[str] = None,
         environment: PolytomicEnvironment = PolytomicEnvironment.DEFAULT,
-        x_polytomic_version: typing.Optional[typing.Literal["2023-04-25"]] = None,
-        token: typing.Optional[typing.Union[str, typing.Callable[[], str]]] = None,
+        token: typing.Union[str, typing.Callable[[], str]],
         timeout: typing.Optional[float] = None,
         httpx_client: typing.Optional[httpx.AsyncClient] = None
     ):
         _defaulted_timeout = timeout if timeout is not None else 60 if httpx_client is None else None
         self._client_wrapper = AsyncClientWrapper(
             base_url=_get_base_url(base_url=base_url, environment=environment),
-            x_polytomic_version=x_polytomic_version,
             token=token,
             httpx_client=httpx.AsyncClient(timeout=_defaulted_timeout) if httpx_client is None else httpx_client,
             timeout=_defaulted_timeout,
         )
         self.bulk_sync = AsyncBulkSyncClient(client_wrapper=self._client_wrapper)
         self.connections = AsyncConnectionsClient(client_wrapper=self._client_wrapper)
+        self.model_sync = AsyncModelSyncClient(client_wrapper=self._client_wrapper)
         self.schemas = AsyncSchemasClient(client_wrapper=self._client_wrapper)
         self.events = AsyncEventsClient(client_wrapper=self._client_wrapper)
         self.jobs = AsyncJobsClient(client_wrapper=self._client_wrapper)
+        self.identity = AsyncIdentityClient(client_wrapper=self._client_wrapper)
         self.models = AsyncModelsClient(client_wrapper=self._client_wrapper)
         self.organization = AsyncOrganizationClient(client_wrapper=self._client_wrapper)
         self.users = AsyncUsersClient(client_wrapper=self._client_wrapper)
         self.permissions = AsyncPermissionsClient(client_wrapper=self._client_wrapper)
-        self.model_sync = AsyncModelSyncClient(client_wrapper=self._client_wrapper)
         self.webhooks = AsyncWebhooksClient(client_wrapper=self._client_wrapper)
 
 
 def _get_base_url(*, base_url: typing.Optional[str] = None, environment: PolytomicEnvironment) -> str:
     if base_url is not None:
         return base_url
     elif environment is not None:
```

### Comparing `polytomic-0.1.2/src/polytomic/core/__init__.py` & `polytomic-0.2.0/src/polytomic/core/__init__.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/core/datetime_utils.py` & `polytomic-0.2.0/src/polytomic/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/core/file.py` & `polytomic-0.2.0/src/polytomic/core/file.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/core/http_client.py` & `polytomic-0.2.0/src/polytomic/core/http_client.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/core/jsonable_encoder.py` & `polytomic-0.2.0/src/polytomic/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/core/request_options.py` & `polytomic-0.2.0/src/polytomic/core/request_options.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/resources/bulk_sync/client.py` & `polytomic-0.2.0/src/polytomic/resources/bulk_sync/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 # This file was auto-generated from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from ...core.api_error import ApiError
+from ...core.api_error import ApiError as core_api_error_ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ...core.request_options import RequestOptions
+from ...errors.bad_request_error import BadRequestError
+from ...errors.forbidden_error import ForbiddenError
+from ...errors.internal_server_error import InternalServerError
+from ...errors.not_found_error import NotFoundError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...types.activate_sync_envelope import ActivateSyncEnvelope
 from ...types.activate_sync_input import ActivateSyncInput
+from ...types.api_error import ApiError as types_api_error_ApiError
 from ...types.bulk_discover import BulkDiscover
 from ...types.bulk_schedule import BulkSchedule
 from ...types.bulk_sync_dest_envelope import BulkSyncDestEnvelope
+from ...types.bulk_sync_execution_envelope import BulkSyncExecutionEnvelope
 from ...types.bulk_sync_list_envelope import BulkSyncListEnvelope
 from ...types.bulk_sync_response_envelope import BulkSyncResponseEnvelope
 from ...types.bulk_sync_source_envelope import BulkSyncSourceEnvelope
-from ...types.bulk_sync_source_schema_envelope import BulkSyncSourceSchemaEnvelope
-from ...types.bulk_sync_source_status_envelope import BulkSyncSourceStatusEnvelope
 from ...types.bulk_sync_status_envelope import BulkSyncStatusEnvelope
 from ...types.rest_err_response import RestErrResponse
 from .resources.executions.client import AsyncExecutionsClient, ExecutionsClient
 from .resources.schemas.client import AsyncSchemasClient, SchemasClient
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
@@ -36,249 +40,22 @@
 
 class BulkSyncClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
         self.executions = ExecutionsClient(client_wrapper=self._client_wrapper)
         self.schemas = SchemasClient(client_wrapper=self._client_wrapper)
 
-    def get_destination(
-        self, id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> BulkSyncDestEnvelope:
-        """
-        Parameters:
-            - id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.bulk_sync.get_destination(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/dest/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(BulkSyncDestEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_source(
-        self,
-        connection_id: str,
-        *,
-        refresh_schemas: typing.Optional[bool] = None,
-        include_fields: typing.Optional[bool] = None,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> BulkSyncSourceEnvelope:
-        """
-        Parameters:
-            - connection_id: str.
-
-            - refresh_schemas: typing.Optional[bool].
-
-            - include_fields: typing.Optional[bool].
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.bulk_sync.get_source(
-            connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            include_fields=True,
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/source/{jsonable_encoder(connection_id)}"
-            ),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "refresh_schemas": refresh_schemas,
-                        "include_fields": include_fields,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
-                )
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(BulkSyncSourceEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_source_schema(
-        self, connection_id: str, schema_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> BulkSyncSourceSchemaEnvelope:
-        """
-        Parameters:
-            - connection_id: str.
-
-            - schema_id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.bulk_sync.get_source_schema(
-            connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            schema_id="schema_id",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/bulk/source/{jsonable_encoder(connection_id)}/schema/{jsonable_encoder(schema_id)}",
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(BulkSyncSourceSchemaEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_source_status(
-        self, connection_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> BulkSyncSourceStatusEnvelope:
-        """
-        Parameters:
-            - connection_id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.bulk_sync.get_source_status(
-            connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/source/{jsonable_encoder(connection_id)}/status"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(BulkSyncSourceStatusEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
     def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> BulkSyncListEnvelope:
         """
         Parameters:
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         client.bulk_sync.list()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/bulk/syncs"),
@@ -299,19 +76,21 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BulkSyncListEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
         self,
         *,
         active: typing.Optional[bool] = OMIT,
         automatically_add_new_fields: typing.Optional[BulkDiscover] = OMIT,
         automatically_add_new_objects: typing.Optional[BulkDiscover] = OMIT,
@@ -363,22 +142,27 @@
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic import BulkSchedule, ScheduleFrequency
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         client.bulk_sync.create(
             destination_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            name="name",
+            mode="replicate",
+            name="My Bulk Sync",
             schedule=BulkSchedule(
+                day_of_month="1",
+                day_of_week="monday",
                 frequency=ScheduleFrequency.MANUAL,
+                hour="0",
+                minute="0",
+                month="1",
             ),
             source_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _request: typing.Dict[str, typing.Any] = {
             "destination_connection_id": destination_connection_id,
             "name": name,
@@ -431,21 +215,27 @@
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BulkSyncResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(
         self,
         id: str,
         *,
         refresh_schemas: typing.Optional[bool] = None,
         request_options: typing.Optional[RequestOptions] = None,
@@ -457,15 +247,14 @@
             - refresh_schemas: typing.Optional[bool].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         client.bulk_sync.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             refresh_schemas=True,
         )
         """
@@ -498,84 +287,21 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BulkSyncResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def remove(
-        self,
-        id: str,
-        *,
-        refresh_schemas: typing.Optional[bool] = None,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> None:
-        """
-        Parameters:
-            - id: str.
-
-            - refresh_schemas: typing.Optional[bool].
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.bulk_sync.remove(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            refresh_schemas=True,
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "refresh_schemas": refresh_schemas,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
-                )
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def update(
         self,
         id: str,
         *,
         active: typing.Optional[bool] = OMIT,
         automatically_add_new_fields: typing.Optional[BulkDiscover] = OMIT,
@@ -634,23 +360,28 @@
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic import BulkSchedule, ScheduleFrequency
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         client.bulk_sync.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             destination_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            name="name",
+            mode="replicate",
+            name="My Bulk Sync",
             schedule=BulkSchedule(
+                day_of_month="1",
+                day_of_week="monday",
                 frequency=ScheduleFrequency.MANUAL,
+                hour="0",
+                minute="0",
+                month="1",
             ),
             source_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _request: typing.Dict[str, typing.Any] = {
             "destination_connection_id": destination_connection_id,
             "name": name,
@@ -676,15 +407,15 @@
         if policies is not OMIT:
             _request["policies"] = policies
         if schemas is not OMIT:
             _request["schemas"] = schemas
         if source_configuration is not OMIT:
             _request["source_configuration"] = source_configuration
         _response = self._client_wrapper.httpx_client.request(
-            "PATCH",
+            "PUT",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
@@ -703,21 +434,99 @@
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BulkSyncResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 401:
+            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
+
+    def remove(
+        self,
+        id: str,
+        *,
+        refresh_schemas: typing.Optional[bool] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> None:
+        """
+        Parameters:
+            - id: str.
+
+            - refresh_schemas: typing.Optional[bool].
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from polytomic.client import Polytomic
+
+        client = Polytomic(
+            token="YOUR_TOKEN",
+        )
+        client.bulk_sync.remove(
+            id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            refresh_schemas=True,
+        )
+        """
+        _response = self._client_wrapper.httpx_client.request(
+            "DELETE",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}"),
+            params=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        "refresh_schemas": refresh_schemas,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def activate(
         self, id: str, *, request: ActivateSyncInput, request_options: typing.Optional[RequestOptions] = None
     ) -> ActivateSyncEnvelope:
         """
         Parameters:
             - id: str.
@@ -726,15 +535,14 @@
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic import ActivateSyncInput
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         client.bulk_sync.activate(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             request=ActivateSyncInput(
                 active=True,
             ),
@@ -768,45 +576,79 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ActivateSyncEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_status(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> BulkSyncStatusEnvelope:
+    def start(
+        self,
+        id: str,
+        *,
+        resync: typing.Optional[bool] = OMIT,
+        schemas: typing.Optional[typing.Sequence[str]] = OMIT,
+        test: typing.Optional[bool] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> BulkSyncExecutionEnvelope:
         """
         Parameters:
             - id: str.
 
+            - resync: typing.Optional[bool].
+
+            - schemas: typing.Optional[typing.Sequence[str]].
+
+            - test: typing.Optional[bool].
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.bulk_sync.get_status(
+        client.bulk_sync.start(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            resync=False,
+            test=False,
         )
         """
+        _request: typing.Dict[str, typing.Any] = {}
+        if resync is not OMIT:
+            _request["resync"] = resync
+        if schemas is not OMIT:
+            _request["schemas"] = schemas
+        if test is not OMIT:
+            _request["test"] = test
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
+            "POST",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}/status"
+                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}/executions"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -814,52 +656,46 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(BulkSyncStatusEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(BulkSyncExecutionEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-
-class AsyncBulkSyncClient:
-    def __init__(self, *, client_wrapper: AsyncClientWrapper):
-        self._client_wrapper = client_wrapper
-        self.executions = AsyncExecutionsClient(client_wrapper=self._client_wrapper)
-        self.schemas = AsyncSchemasClient(client_wrapper=self._client_wrapper)
-
-    async def get_destination(
-        self, id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> BulkSyncDestEnvelope:
+    def get_status(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> BulkSyncStatusEnvelope:
         """
         Parameters:
             - id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from polytomic.client import AsyncPolytomic
+        from polytomic.client import Polytomic
 
-        client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
+        client = Polytomic(
             token="YOUR_TOKEN",
         )
-        await client.bulk_sync.get_destination(
+        client.bulk_sync.get_status(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
-        _response = await self._client_wrapper.httpx_client.request(
+        _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/dest/{jsonable_encoder(id)}"),
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}/status"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -870,61 +706,60 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(BulkSyncDestEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(BulkSyncStatusEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_source(
+    def get_source(
         self,
-        connection_id: str,
+        id: str,
         *,
-        refresh_schemas: typing.Optional[bool] = None,
         include_fields: typing.Optional[bool] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> BulkSyncSourceEnvelope:
         """
         Parameters:
-            - connection_id: str.
-
-            - refresh_schemas: typing.Optional[bool].
+            - id: str.
 
             - include_fields: typing.Optional[bool].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from polytomic.client import AsyncPolytomic
+        from polytomic.client import Polytomic
 
-        client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
+        client = Polytomic(
             token="YOUR_TOKEN",
         )
-        await client.bulk_sync.get_source(
-            connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        client.bulk_sync.get_source(
+            id="248df4b7-aa70-47b8-a036-33ac447e668d",
             include_fields=True,
         )
         """
-        _response = await self._client_wrapper.httpx_client.request(
+        _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/source/{jsonable_encoder(connection_id)}"
+                f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}/bulksync/source"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
-                        "refresh_schemas": refresh_schemas,
                         "include_fields": include_fields,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
                             else {}
                         ),
                     }
@@ -942,49 +777,50 @@
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BulkSyncSourceEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_source_schema(
-        self, connection_id: str, schema_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> BulkSyncSourceSchemaEnvelope:
+    def get_destination(
+        self, id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> BulkSyncDestEnvelope:
         """
         Parameters:
-            - connection_id: str.
-
-            - schema_id: str.
+            - id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from polytomic.client import AsyncPolytomic
+        from polytomic.client import Polytomic
 
-        client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
+        client = Polytomic(
             token="YOUR_TOKEN",
         )
-        await client.bulk_sync.get_source_schema(
-            connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            schema_id="schema_id",
+        client.bulk_sync.get_destination(
+            id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
-        _response = await self._client_wrapper.httpx_client.request(
+        _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/bulk/source/{jsonable_encoder(connection_id)}/schema/{jsonable_encoder(schema_id)}",
+                f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}/bulksync/target"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -996,83 +832,44 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(BulkSyncSourceSchemaEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(BulkSyncDestEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get_source_status(
-        self, connection_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> BulkSyncSourceStatusEnvelope:
-        """
-        Parameters:
-            - connection_id: str.
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import AsyncPolytomic
 
-        client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.bulk_sync.get_source_status(
-            connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/source/{jsonable_encoder(connection_id)}/status"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(BulkSyncSourceStatusEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+class AsyncBulkSyncClient:
+    def __init__(self, *, client_wrapper: AsyncClientWrapper):
+        self._client_wrapper = client_wrapper
+        self.executions = AsyncExecutionsClient(client_wrapper=self._client_wrapper)
+        self.schemas = AsyncSchemasClient(client_wrapper=self._client_wrapper)
 
     async def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> BulkSyncListEnvelope:
         """
         Parameters:
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         await client.bulk_sync.list()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/bulk/syncs"),
@@ -1093,19 +890,21 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BulkSyncListEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
         self,
         *,
         active: typing.Optional[bool] = OMIT,
         automatically_add_new_fields: typing.Optional[BulkDiscover] = OMIT,
         automatically_add_new_objects: typing.Optional[BulkDiscover] = OMIT,
@@ -1157,22 +956,27 @@
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic import BulkSchedule, ScheduleFrequency
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         await client.bulk_sync.create(
             destination_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            name="name",
+            mode="replicate",
+            name="My Bulk Sync",
             schedule=BulkSchedule(
+                day_of_month="1",
+                day_of_week="monday",
                 frequency=ScheduleFrequency.MANUAL,
+                hour="0",
+                minute="0",
+                month="1",
             ),
             source_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _request: typing.Dict[str, typing.Any] = {
             "destination_connection_id": destination_connection_id,
             "name": name,
@@ -1225,21 +1029,27 @@
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BulkSyncResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(
         self,
         id: str,
         *,
         refresh_schemas: typing.Optional[bool] = None,
         request_options: typing.Optional[RequestOptions] = None,
@@ -1251,15 +1061,14 @@
             - refresh_schemas: typing.Optional[bool].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         await client.bulk_sync.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             refresh_schemas=True,
         )
         """
@@ -1292,84 +1101,21 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BulkSyncResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def remove(
-        self,
-        id: str,
-        *,
-        refresh_schemas: typing.Optional[bool] = None,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> None:
-        """
-        Parameters:
-            - id: str.
-
-            - refresh_schemas: typing.Optional[bool].
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.bulk_sync.remove(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            refresh_schemas=True,
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "refresh_schemas": refresh_schemas,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
-                )
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update(
         self,
         id: str,
         *,
         active: typing.Optional[bool] = OMIT,
         automatically_add_new_fields: typing.Optional[BulkDiscover] = OMIT,
@@ -1428,23 +1174,28 @@
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic import BulkSchedule, ScheduleFrequency
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         await client.bulk_sync.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             destination_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            name="name",
+            mode="replicate",
+            name="My Bulk Sync",
             schedule=BulkSchedule(
+                day_of_month="1",
+                day_of_week="monday",
                 frequency=ScheduleFrequency.MANUAL,
+                hour="0",
+                minute="0",
+                month="1",
             ),
             source_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _request: typing.Dict[str, typing.Any] = {
             "destination_connection_id": destination_connection_id,
             "name": name,
@@ -1470,15 +1221,15 @@
         if policies is not OMIT:
             _request["policies"] = policies
         if schemas is not OMIT:
             _request["schemas"] = schemas
         if source_configuration is not OMIT:
             _request["source_configuration"] = source_configuration
         _response = await self._client_wrapper.httpx_client.request(
-            "PATCH",
+            "PUT",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
@@ -1497,21 +1248,99 @@
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BulkSyncResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 401:
+            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def remove(
+        self,
+        id: str,
+        *,
+        refresh_schemas: typing.Optional[bool] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> None:
+        """
+        Parameters:
+            - id: str.
+
+            - refresh_schemas: typing.Optional[bool].
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from polytomic.client import AsyncPolytomic
+
+        client = AsyncPolytomic(
+            token="YOUR_TOKEN",
+        )
+        await client.bulk_sync.remove(
+            id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            refresh_schemas=True,
+        )
+        """
+        _response = await self._client_wrapper.httpx_client.request(
+            "DELETE",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}"),
+            params=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        "refresh_schemas": refresh_schemas,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def activate(
         self, id: str, *, request: ActivateSyncInput, request_options: typing.Optional[RequestOptions] = None
     ) -> ActivateSyncEnvelope:
         """
         Parameters:
             - id: str.
@@ -1520,15 +1349,14 @@
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic import ActivateSyncInput
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         await client.bulk_sync.activate(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             request=ActivateSyncInput(
                 active=True,
             ),
@@ -1562,33 +1390,117 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ActivateSyncEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def start(
+        self,
+        id: str,
+        *,
+        resync: typing.Optional[bool] = OMIT,
+        schemas: typing.Optional[typing.Sequence[str]] = OMIT,
+        test: typing.Optional[bool] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> BulkSyncExecutionEnvelope:
+        """
+        Parameters:
+            - id: str.
+
+            - resync: typing.Optional[bool].
+
+            - schemas: typing.Optional[typing.Sequence[str]].
+
+            - test: typing.Optional[bool].
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from polytomic.client import AsyncPolytomic
+
+        client = AsyncPolytomic(
+            token="YOUR_TOKEN",
+        )
+        await client.bulk_sync.start(
+            id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            resync=False,
+            test=False,
+        )
+        """
+        _request: typing.Dict[str, typing.Any] = {}
+        if resync is not OMIT:
+            _request["resync"] = resync
+        if schemas is not OMIT:
+            _request["schemas"] = schemas
+        if test is not OMIT:
+            _request["test"] = test
+        _response = await self._client_wrapper.httpx_client.request(
+            "POST",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}/executions"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(BulkSyncExecutionEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 401:
+            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_status(
         self, id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> BulkSyncStatusEnvelope:
         """
         Parameters:
             - id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         await client.bulk_sync.get_status(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
@@ -1613,12 +1525,144 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BulkSyncStatusEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def get_source(
+        self,
+        id: str,
+        *,
+        include_fields: typing.Optional[bool] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> BulkSyncSourceEnvelope:
+        """
+        Parameters:
+            - id: str.
+
+            - include_fields: typing.Optional[bool].
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from polytomic.client import AsyncPolytomic
+
+        client = AsyncPolytomic(
+            token="YOUR_TOKEN",
+        )
+        await client.bulk_sync.get_source(
+            id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            include_fields=True,
+        )
+        """
+        _response = await self._client_wrapper.httpx_client.request(
+            "GET",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}/bulksync/source"
+            ),
+            params=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        "include_fields": include_fields,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(BulkSyncSourceEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 401:
+            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def get_destination(
+        self, id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> BulkSyncDestEnvelope:
+        """
+        Parameters:
+            - id: str.
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from polytomic.client import AsyncPolytomic
+
+        client = AsyncPolytomic(
+            token="YOUR_TOKEN",
+        )
+        await client.bulk_sync.get_destination(
+            id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        )
+        """
+        _response = await self._client_wrapper.httpx_client.request(
+            "GET",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}/bulksync/target"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(BulkSyncDestEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 401:
+            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `polytomic-0.1.2/src/polytomic/resources/bulk_sync/resources/executions/client.py` & `polytomic-0.2.0/src/polytomic/resources/bulk_sync/resources/executions/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 # This file was auto-generated from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from .....core.api_error import ApiError
+from .....core.api_error import ApiError as core_api_error_ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .....core.jsonable_encoder import jsonable_encoder
 from .....core.remove_none_from_dict import remove_none_from_dict
 from .....core.request_options import RequestOptions
+from .....errors.not_found_error import NotFoundError
 from .....errors.unauthorized_error import UnauthorizedError
+from .....types.api_error import ApiError as types_api_error_ApiError
 from .....types.bulk_sync_execution_envelope import BulkSyncExecutionEnvelope
 from .....types.list_bulk_sync_executions_envelope import ListBulkSyncExecutionsEnvelope
 from .....types.rest_err_response import RestErrResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
-# this is used as the default value for optional parameters
-OMIT = typing.cast(typing.Any, ...)
-
 
 class ExecutionsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def list(
         self, id: str, *, request_options: typing.Optional[RequestOptions] = None
@@ -35,15 +34,14 @@
             - id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         client.bulk_sync.executions.list(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
@@ -68,97 +66,21 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListBulkSyncExecutionsEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def start(
-        self,
-        id: str,
-        *,
-        resync: typing.Optional[bool] = OMIT,
-        schemas: typing.Optional[typing.Sequence[str]] = OMIT,
-        test: typing.Optional[bool] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> BulkSyncExecutionEnvelope:
-        """
-        Parameters:
-            - id: str.
-
-            - resync: typing.Optional[bool].
-
-            - schemas: typing.Optional[typing.Sequence[str]].
-
-            - test: typing.Optional[bool].
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.bulk_sync.executions.start(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            resync=False,
-            test=False,
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {}
-        if resync is not OMIT:
-            _request["resync"] = resync
-        if schemas is not OMIT:
-            _request["schemas"] = schemas
-        if test is not OMIT:
-            _request["test"] = test
-        _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}/executions"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(BulkSyncExecutionEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(
         self, id: str, exec_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> BulkSyncExecutionEnvelope:
         """
         Parameters:
             - id: str.
@@ -166,15 +88,14 @@
             - exec_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         client.bulk_sync.executions.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             exec_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
@@ -201,19 +122,21 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BulkSyncExecutionEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncExecutionsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def list(
@@ -224,15 +147,14 @@
             - id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         await client.bulk_sync.executions.list(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
@@ -257,97 +179,21 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListBulkSyncExecutionsEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def start(
-        self,
-        id: str,
-        *,
-        resync: typing.Optional[bool] = OMIT,
-        schemas: typing.Optional[typing.Sequence[str]] = OMIT,
-        test: typing.Optional[bool] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> BulkSyncExecutionEnvelope:
-        """
-        Parameters:
-            - id: str.
-
-            - resync: typing.Optional[bool].
-
-            - schemas: typing.Optional[typing.Sequence[str]].
-
-            - test: typing.Optional[bool].
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.bulk_sync.executions.start(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            resync=False,
-            test=False,
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {}
-        if resync is not OMIT:
-            _request["resync"] = resync
-        if schemas is not OMIT:
-            _request["schemas"] = schemas
-        if test is not OMIT:
-            _request["test"] = test
-        _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}/executions"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(BulkSyncExecutionEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(
         self, id: str, exec_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> BulkSyncExecutionEnvelope:
         """
         Parameters:
             - id: str.
@@ -355,15 +201,14 @@
             - exec_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         await client.bulk_sync.executions.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             exec_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
@@ -390,12 +235,14 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BulkSyncExecutionEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `polytomic-0.1.2/src/polytomic/resources/bulk_sync/resources/schemas/client.py` & `polytomic-0.2.0/src/polytomic/resources/model_sync/resources/executions/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,120 @@
 # This file was auto-generated from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from .....core.api_error import ApiError
+from .....core.api_error import ApiError as core_api_error_ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .....core.jsonable_encoder import jsonable_encoder
 from .....core.remove_none_from_dict import remove_none_from_dict
 from .....core.request_options import RequestOptions
+from .....errors.bad_request_error import BadRequestError
+from .....errors.internal_server_error import InternalServerError
+from .....errors.not_found_error import NotFoundError
 from .....errors.unauthorized_error import UnauthorizedError
-from .....types.bulk_field import BulkField
-from .....types.bulk_schema_envelope import BulkSchemaEnvelope
-from .....types.list_bulk_schema import ListBulkSchema
+from .....types.api_error import ApiError as types_api_error_ApiError
+from .....types.execution_logs_response_envelope import ExecutionLogsResponseEnvelope
+from .....types.get_execution_response_envelope import GetExecutionResponseEnvelope
+from .....types.list_execution_response_envelope import ListExecutionResponseEnvelope
 from .....types.rest_err_response import RestErrResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
-# this is used as the default value for optional parameters
-OMIT = typing.cast(typing.Any, ...)
 
-
-class SchemasClient:
+class ExecutionsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def list(
-        self,
-        id: str,
-        *,
-        filters: typing.Optional[typing.Dict[str, typing.Optional[str]]] = None,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> ListBulkSchema:
+        self, sync_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> ListExecutionResponseEnvelope:
         """
         Parameters:
-            - id: str.
-
-            - filters: typing.Optional[typing.Dict[str, typing.Optional[str]]].
+            - sync_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.bulk_sync.schemas.list(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        client.model_sync.executions.list(
+            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}/schemas"
+                f"{self._client_wrapper.get_base_url()}/", f"api/syncs/{jsonable_encoder(sync_id)}/executions"
             ),
             params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
-                        "filters": jsonable_encoder(filters),
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(ListExecutionResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 401:
+            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
+
+    def get(
+        self, sync_id: str, id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> GetExecutionResponseEnvelope:
+        """
+        Parameters:
+            - sync_id: str.
+
+            - id: str.
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from polytomic.client import Polytomic
+
+        client = Polytomic(
+            token="YOUR_TOKEN",
+        )
+        client.model_sync.executions.get(
+            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        )
+        """
+        _response = self._client_wrapper.httpx_client.request(
+            "GET",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -81,82 +122,60 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ListBulkSchema, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(GetExecutionResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update(
-        self,
-        id: str,
-        schema_id: str,
-        *,
-        enabled: typing.Optional[bool] = OMIT,
-        fields: typing.Optional[typing.Sequence[BulkField]] = OMIT,
-        partition_key: typing.Optional[str] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> BulkSchemaEnvelope:
+    def get_log_urls(
+        self, sync_id: str, id: str, type: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> ExecutionLogsResponseEnvelope:
         """
         Parameters:
-            - id: str.
-
-            - schema_id: str.
+            - sync_id: str.
 
-            - enabled: typing.Optional[bool].
-
-            - fields: typing.Optional[typing.Sequence[BulkField]].
+            - id: str.
 
-            - partition_key: typing.Optional[str].
+            - type: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.bulk_sync.schemas.update(
+        client.model_sync.executions.get_log_urls(
+            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            schema_id="contact",
-            enabled=True,
-            partition_key="email",
+            type="records",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {}
-        if enabled is not OMIT:
-            _request["enabled"] = enabled
-        if fields is not OMIT:
-            _request["fields"] = fields
-        if partition_key is not OMIT:
-            _request["partition_key"] = partition_key
         _response = self._client_wrapper.httpx_client.request(
-            "PATCH",
+            "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
-                f"api/bulk/syncs/{jsonable_encoder(id)}/schemas/{jsonable_encoder(schema_id)}",
+                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/{jsonable_encoder(type)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -164,50 +183,67 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(BulkSchemaEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ExecutionLogsResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(
-        self, id: str, schema_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> BulkSchemaEnvelope:
+    def get_logs(
+        self,
+        sync_id: str,
+        id: str,
+        type: str,
+        filename: str,
+        *,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> None:
         """
         Parameters:
+            - sync_id: str.
+
             - id: str.
 
-            - schema_id: str.
+            - type: str.
+
+            - filename: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.bulk_sync.schemas.get(
+        client.model_sync.executions.get_logs(
+            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            schema_id="Contact",
+            type="records",
+            filename="path/to/file.json",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
-                f"api/bulk/syncs/{jsonable_encoder(id)}/schemas/{jsonable_encoder(schema_id)}",
+                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/{jsonable_encoder(type)}/{jsonable_encoder(filename)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -219,70 +255,116 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(BulkSchemaEnvelope, _response.json())  # type: ignore
+            return
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncSchemasClient:
+class AsyncExecutionsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def list(
-        self,
-        id: str,
-        *,
-        filters: typing.Optional[typing.Dict[str, typing.Optional[str]]] = None,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> ListBulkSchema:
+        self, sync_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> ListExecutionResponseEnvelope:
         """
         Parameters:
-            - id: str.
-
-            - filters: typing.Optional[typing.Dict[str, typing.Optional[str]]].
+            - sync_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.bulk_sync.schemas.list(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        await client.model_sync.executions.list(
+            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}/schemas"
+                f"{self._client_wrapper.get_base_url()}/", f"api/syncs/{jsonable_encoder(sync_id)}/executions"
             ),
             params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
-                        "filters": jsonable_encoder(filters),
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(ListExecutionResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 401:
+            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def get(
+        self, sync_id: str, id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> GetExecutionResponseEnvelope:
+        """
+        Parameters:
+            - sync_id: str.
+
+            - id: str.
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from polytomic.client import AsyncPolytomic
+
+        client = AsyncPolytomic(
+            token="YOUR_TOKEN",
+        )
+        await client.model_sync.executions.get(
+            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        )
+        """
+        _response = await self._client_wrapper.httpx_client.request(
+            "GET",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -290,82 +372,60 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ListBulkSchema, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(GetExecutionResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update(
-        self,
-        id: str,
-        schema_id: str,
-        *,
-        enabled: typing.Optional[bool] = OMIT,
-        fields: typing.Optional[typing.Sequence[BulkField]] = OMIT,
-        partition_key: typing.Optional[str] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> BulkSchemaEnvelope:
+    async def get_log_urls(
+        self, sync_id: str, id: str, type: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> ExecutionLogsResponseEnvelope:
         """
         Parameters:
-            - id: str.
-
-            - schema_id: str.
+            - sync_id: str.
 
-            - enabled: typing.Optional[bool].
-
-            - fields: typing.Optional[typing.Sequence[BulkField]].
+            - id: str.
 
-            - partition_key: typing.Optional[str].
+            - type: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.bulk_sync.schemas.update(
+        await client.model_sync.executions.get_log_urls(
+            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            schema_id="contact",
-            enabled=True,
-            partition_key="email",
+            type="records",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {}
-        if enabled is not OMIT:
-            _request["enabled"] = enabled
-        if fields is not OMIT:
-            _request["fields"] = fields
-        if partition_key is not OMIT:
-            _request["partition_key"] = partition_key
         _response = await self._client_wrapper.httpx_client.request(
-            "PATCH",
+            "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
-                f"api/bulk/syncs/{jsonable_encoder(id)}/schemas/{jsonable_encoder(schema_id)}",
+                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/{jsonable_encoder(type)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -373,50 +433,67 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(BulkSchemaEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ExecutionLogsResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(
-        self, id: str, schema_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> BulkSchemaEnvelope:
+    async def get_logs(
+        self,
+        sync_id: str,
+        id: str,
+        type: str,
+        filename: str,
+        *,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> None:
         """
         Parameters:
+            - sync_id: str.
+
             - id: str.
 
-            - schema_id: str.
+            - type: str.
+
+            - filename: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.bulk_sync.schemas.get(
+        await client.model_sync.executions.get_logs(
+            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            schema_id="Contact",
+            type="records",
+            filename="path/to/file.json",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
-                f"api/bulk/syncs/{jsonable_encoder(id)}/schemas/{jsonable_encoder(schema_id)}",
+                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/{jsonable_encoder(type)}/{jsonable_encoder(filename)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -428,15 +505,21 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(BulkSchemaEnvelope, _response.json())  # type: ignore
+            return
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `polytomic-0.1.2/src/polytomic/resources/connections/client.py` & `polytomic-0.2.0/src/polytomic/resources/connections/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # This file was auto-generated from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from ...core.api_error import ApiError
+from ...core.api_error import ApiError as core_api_error_ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ...core.request_options import RequestOptions
+from ...errors.bad_request_error import BadRequestError
+from ...errors.forbidden_error import ForbiddenError
+from ...errors.internal_server_error import InternalServerError
+from ...errors.not_found_error import NotFoundError
 from ...errors.unauthorized_error import UnauthorizedError
+from ...errors.unprocessable_entity_error import UnprocessableEntityError
+from ...types.api_error import ApiError as types_api_error_ApiError
+from ...types.connect_card_response_envelope import ConnectCardResponseEnvelope
 from ...types.connection_list_response_envelope import ConnectionListResponseEnvelope
 from ...types.connection_parameter_values_response_envelope import ConnectionParameterValuesResponseEnvelope
 from ...types.connection_response_envelope import ConnectionResponseEnvelope
 from ...types.connection_type_response_envelope import ConnectionTypeResponseEnvelope
 from ...types.create_connection_response_envelope import CreateConnectionResponseEnvelope
-from ...types.get_connection_meta_envelope import GetConnectionMetaEnvelope
-from ...types.model_field_response import ModelFieldResponse
 from ...types.rest_err_response import RestErrResponse
-from ...types.target_response_envelope import TargetResponseEnvelope
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 # this is used as the default value for optional parameters
@@ -37,15 +41,14 @@
         """
         Parameters:
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         client.connections.get_types()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/connection_types"),
@@ -66,29 +69,30 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ConnectionTypeResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> ConnectionListResponseEnvelope:
         """
         Parameters:
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         client.connections.list()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/connections"),
@@ -109,19 +113,21 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ConnectionListResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
         self,
         *,
         configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         name: str,
         organization_id: typing.Optional[str] = OMIT,
@@ -148,21 +154,20 @@
             - validate: typing.Optional[bool]. Validate connection configuration.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         client.connections.create(
-            name="My Connection",
+            name="My Postgres Connection",
             redirect_url="https://example.com/oauth_redirect",
-            type="s3",
+            type="postgresql",
             validate=True,
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name, "type": type}
         if configuration is not OMIT:
             _request["configuration"] = configuration
         if organization_id is not OMIT:
@@ -197,44 +202,92 @@
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateConnectionResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    def connect(self, *, request_options: typing.Optional[RequestOptions] = None) -> None:
+    def connect(
+        self,
+        *,
+        connection: typing.Optional[str] = OMIT,
+        name: str,
+        organization_id: typing.Optional[str] = OMIT,
+        redirect_url: str,
+        type: typing.Optional[str] = OMIT,
+        whitelist: typing.Optional[typing.Sequence[str]] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> ConnectCardResponseEnvelope:
         """
         Parameters:
+            - connection: typing.Optional[str].
+
+            - name: str.
+
+            - organization_id: typing.Optional[str].
+
+            - redirect_url: str.
+
+            - type: typing.Optional[str].
+
+            - whitelist: typing.Optional[typing.Sequence[str]].
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.connections.connect()
+        client.connections.connect(
+            connection="248df4b7-aa70-47b8-a036-33ac447e668d",
+            name="Salesforce Connection",
+            redirect_url="redirect_url",
+            type="salesforce",
+        )
         """
+        _request: typing.Dict[str, typing.Any] = {"name": name, "redirect_url": redirect_url}
+        if connection is not OMIT:
+            _request["connection"] = connection
+        if organization_id is not OMIT:
+            _request["organization_id"] = organization_id
+        if type is not OMIT:
+            _request["type"] = type
+        if whitelist is not OMIT:
+            _request["whitelist"] = whitelist
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/connections/connect"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
-            if request_options is not None
-            else None,
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -242,32 +295,41 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic.parse_obj_as(ConnectCardResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 401:
+            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> ConnectionResponseEnvelope:
         """
         Parameters:
             - id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         client.connections.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
@@ -290,80 +352,23 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ConnectionResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def remove(
-        self, id: str, *, force: typing.Optional[bool] = None, request_options: typing.Optional[RequestOptions] = None
-    ) -> None:
-        """
-        Parameters:
-            - id: str.
-
-            - force: typing.Optional[bool].
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.connections.remove(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            force=True,
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "force": force,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
-                )
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def update(
         self,
         id: str,
         *,
         configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         name: str,
@@ -393,22 +398,21 @@
             - validate: typing.Optional[bool]. Validate connection configuration.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         client.connections.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            name="My Connection",
+            name="My Postgres Connection",
             reconnect=False,
-            type="s3",
+            type="postgresql",
             validate=True,
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if configuration is not OMIT:
             _request["configuration"] = configuration
         if organization_id is not OMIT:
@@ -418,15 +422,15 @@
         if reconnect is not OMIT:
             _request["reconnect"] = reconnect
         if type is not OMIT:
             _request["type"] = type
         if validate is not OMIT:
             _request["validate"] = validate
         _response = self._client_wrapper.httpx_client.request(
-            "PATCH",
+            "PUT",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
@@ -445,230 +449,62 @@
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateConnectionResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_parameter_values(
-        self, id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> ConnectionParameterValuesResponseEnvelope:
-        """
-        Parameters:
-            - id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.connections.get_parameter_values(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}/parameter_values"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ConnectionParameterValuesResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_source(
-        self, id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> GetConnectionMetaEnvelope:
-        """
-        Parameters:
-            - id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.connections.get_source(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}/source"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetConnectionMetaEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_source_fields(
-        self,
-        id: str,
-        *,
-        query: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> ModelFieldResponse:
-        """
-        Parameters:
-            - id: str.
-
-            - query: typing.Optional[typing.Dict[str, typing.Any]].
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.connections.get_source_fields(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {}
-        if query is not OMIT:
-            _request["query"] = query
-        _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}/source/fields"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ModelFieldResponse, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_target(
-        self,
-        id: str,
-        *,
-        type: typing.Optional[str] = None,
-        search: typing.Optional[str] = None,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> GetConnectionMetaEnvelope:
+    def remove(
+        self, id: str, *, force: typing.Optional[bool] = None, request_options: typing.Optional[RequestOptions] = None
+    ) -> None:
         """
         Parameters:
             - id: str.
 
-            - type: typing.Optional[str].
-
-            - search: typing.Optional[str].
+            - force: typing.Optional[bool].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.connections.get_target(
+        client.connections.remove(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            type="table",
-            search="public.users",
+            force=True,
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}/target"
-            ),
+            "DELETE",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
-                        "type": type,
-                        "search": search,
+                        "force": force,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
                             else {}
                         ),
                     }
                 )
@@ -684,70 +520,59 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetConnectionMetaEnvelope, _response.json())  # type: ignore
+            return
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_target_fields(
-        self,
-        id: str,
-        *,
-        refresh: typing.Optional[bool] = OMIT,
-        target: str,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> TargetResponseEnvelope:
+    def get_parameter_values(
+        self, id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> ConnectionParameterValuesResponseEnvelope:
         """
         Parameters:
             - id: str.
 
-            - refresh: typing.Optional[bool].
-
-            - target: str.
-
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.connections.get_target_fields(
+        client.connections.get_parameter_values(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            refresh=False,
-            target="database.table",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"target": target}
-        if refresh is not OMIT:
-            _request["refresh"] = refresh
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
+            "GET",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}/target/fields"
+                f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}/parameter_values"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -755,22 +580,26 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(TargetResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ConnectionParameterValuesResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncConnectionsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def get_types(
@@ -779,15 +608,14 @@
         """
         Parameters:
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         await client.connections.get_types()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/connection_types"),
@@ -808,29 +636,30 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ConnectionTypeResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> ConnectionListResponseEnvelope:
         """
         Parameters:
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         await client.connections.list()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/connections"),
@@ -851,19 +680,21 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ConnectionListResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
         self,
         *,
         configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         name: str,
         organization_id: typing.Optional[str] = OMIT,
@@ -890,21 +721,20 @@
             - validate: typing.Optional[bool]. Validate connection configuration.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         await client.connections.create(
-            name="My Connection",
+            name="My Postgres Connection",
             redirect_url="https://example.com/oauth_redirect",
-            type="s3",
+            type="postgresql",
             validate=True,
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name, "type": type}
         if configuration is not OMIT:
             _request["configuration"] = configuration
         if organization_id is not OMIT:
@@ -939,44 +769,92 @@
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateConnectionResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def connect(self, *, request_options: typing.Optional[RequestOptions] = None) -> None:
+    async def connect(
+        self,
+        *,
+        connection: typing.Optional[str] = OMIT,
+        name: str,
+        organization_id: typing.Optional[str] = OMIT,
+        redirect_url: str,
+        type: typing.Optional[str] = OMIT,
+        whitelist: typing.Optional[typing.Sequence[str]] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> ConnectCardResponseEnvelope:
         """
         Parameters:
+            - connection: typing.Optional[str].
+
+            - name: str.
+
+            - organization_id: typing.Optional[str].
+
+            - redirect_url: str.
+
+            - type: typing.Optional[str].
+
+            - whitelist: typing.Optional[typing.Sequence[str]].
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.connections.connect()
+        await client.connections.connect(
+            connection="248df4b7-aa70-47b8-a036-33ac447e668d",
+            name="Salesforce Connection",
+            redirect_url="redirect_url",
+            type="salesforce",
+        )
         """
+        _request: typing.Dict[str, typing.Any] = {"name": name, "redirect_url": redirect_url}
+        if connection is not OMIT:
+            _request["connection"] = connection
+        if organization_id is not OMIT:
+            _request["organization_id"] = organization_id
+        if type is not OMIT:
+            _request["type"] = type
+        if whitelist is not OMIT:
+            _request["whitelist"] = whitelist
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/connections/connect"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
-            if request_options is not None
-            else None,
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -984,34 +862,43 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic.parse_obj_as(ConnectCardResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 401:
+            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(
         self, id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> ConnectionResponseEnvelope:
         """
         Parameters:
             - id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         await client.connections.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
@@ -1034,80 +921,23 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ConnectionResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def remove(
-        self, id: str, *, force: typing.Optional[bool] = None, request_options: typing.Optional[RequestOptions] = None
-    ) -> None:
-        """
-        Parameters:
-            - id: str.
-
-            - force: typing.Optional[bool].
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.connections.remove(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            force=True,
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "force": force,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
-                )
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update(
         self,
         id: str,
         *,
         configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         name: str,
@@ -1137,22 +967,21 @@
             - validate: typing.Optional[bool]. Validate connection configuration.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         await client.connections.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            name="My Connection",
+            name="My Postgres Connection",
             reconnect=False,
-            type="s3",
+            type="postgresql",
             validate=True,
         )
         """
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if configuration is not OMIT:
             _request["configuration"] = configuration
         if organization_id is not OMIT:
@@ -1162,15 +991,15 @@
         if reconnect is not OMIT:
             _request["reconnect"] = reconnect
         if type is not OMIT:
             _request["type"] = type
         if validate is not OMIT:
             _request["validate"] = validate
         _response = await self._client_wrapper.httpx_client.request(
-            "PATCH",
+            "PUT",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
@@ -1189,230 +1018,62 @@
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateConnectionResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get_parameter_values(
-        self, id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> ConnectionParameterValuesResponseEnvelope:
-        """
-        Parameters:
-            - id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.connections.get_parameter_values(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}/parameter_values"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ConnectionParameterValuesResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_source(
-        self, id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> GetConnectionMetaEnvelope:
-        """
-        Parameters:
-            - id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.connections.get_source(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}/source"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetConnectionMetaEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get_source_fields(
-        self,
-        id: str,
-        *,
-        query: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> ModelFieldResponse:
-        """
-        Parameters:
-            - id: str.
-
-            - query: typing.Optional[typing.Dict[str, typing.Any]].
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.connections.get_source_fields(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {}
-        if query is not OMIT:
-            _request["query"] = query
-        _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}/source/fields"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ModelFieldResponse, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get_target(
-        self,
-        id: str,
-        *,
-        type: typing.Optional[str] = None,
-        search: typing.Optional[str] = None,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> GetConnectionMetaEnvelope:
+    async def remove(
+        self, id: str, *, force: typing.Optional[bool] = None, request_options: typing.Optional[RequestOptions] = None
+    ) -> None:
         """
         Parameters:
             - id: str.
 
-            - type: typing.Optional[str].
-
-            - search: typing.Optional[str].
+            - force: typing.Optional[bool].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.connections.get_target(
+        await client.connections.remove(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            type="table",
-            search="public.users",
+            force=True,
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}/target"
-            ),
+            "DELETE",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
-                        "type": type,
-                        "search": search,
+                        "force": force,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
                             else {}
                         ),
                     }
                 )
@@ -1428,70 +1089,59 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetConnectionMetaEnvelope, _response.json())  # type: ignore
+            return
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_target_fields(
-        self,
-        id: str,
-        *,
-        refresh: typing.Optional[bool] = OMIT,
-        target: str,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> TargetResponseEnvelope:
+    async def get_parameter_values(
+        self, id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> ConnectionParameterValuesResponseEnvelope:
         """
         Parameters:
             - id: str.
 
-            - refresh: typing.Optional[bool].
-
-            - target: str.
-
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.connections.get_target_fields(
+        await client.connections.get_parameter_values(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            refresh=False,
-            target="database.table",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"target": target}
-        if refresh is not OMIT:
-            _request["refresh"] = refresh
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
+            "GET",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}/target/fields"
+                f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}/parameter_values"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -1499,15 +1149,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(TargetResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ConnectionParameterValuesResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `polytomic-0.1.2/src/polytomic/resources/events/client.py` & `polytomic-0.2.0/src/polytomic/resources/events/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 # This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from ...core.api_error import ApiError
+from ...core.api_error import ApiError as core_api_error_ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.datetime_utils import serialize_datetime
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ...core.request_options import RequestOptions
+from ...errors.internal_server_error import InternalServerError
 from ...errors.unauthorized_error import UnauthorizedError
+from ...errors.unprocessable_entity_error import UnprocessableEntityError
+from ...types.api_error import ApiError as types_api_error_ApiError
 from ...types.event_types_envelope import EventTypesEnvelope
 from ...types.events_envelope import EventsEnvelope
 from ...types.rest_err_response import RestErrResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class EventsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def api_v_2_get_events(
+    def list(
         self,
         *,
         organization_id: typing.Optional[str] = None,
         type: typing.Optional[str] = None,
         starting_after: typing.Optional[dt.datetime] = None,
         ending_before: typing.Optional[dt.datetime] = None,
         limit: typing.Optional[int] = None,
@@ -51,18 +54,17 @@
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         import datetime
 
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.events.api_v_2_get_events(
+        client.events.list(
             organization_id="248df4b7-aa70-47b8-a036-33ac447e668d",
             starting_after=datetime.datetime.fromisoformat(
                 "2020-01-01 00:00:00+00:00",
             ),
             ending_before=datetime.datetime.fromisoformat(
                 "2020-01-01 00:00:00+00:00",
             ),
@@ -101,32 +103,37 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(EventsEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    def api_v_2_get_event_types(self, *, request_options: typing.Optional[RequestOptions] = None) -> EventTypesEnvelope:
+    def get_types(self, *, request_options: typing.Optional[RequestOptions] = None) -> EventTypesEnvelope:
         """
         Parameters:
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.events.api_v_2_get_event_types()
+        client.events.get_types()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/events_types"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
@@ -147,23 +154,23 @@
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(EventTypesEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncEventsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def api_v_2_get_events(
+    async def list(
         self,
         *,
         organization_id: typing.Optional[str] = None,
         type: typing.Optional[str] = None,
         starting_after: typing.Optional[dt.datetime] = None,
         ending_before: typing.Optional[dt.datetime] = None,
         limit: typing.Optional[int] = None,
@@ -184,18 +191,17 @@
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         import datetime
 
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.events.api_v_2_get_events(
+        await client.events.list(
             organization_id="248df4b7-aa70-47b8-a036-33ac447e668d",
             starting_after=datetime.datetime.fromisoformat(
                 "2020-01-01 00:00:00+00:00",
             ),
             ending_before=datetime.datetime.fromisoformat(
                 "2020-01-01 00:00:00+00:00",
             ),
@@ -234,34 +240,37 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(EventsEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def api_v_2_get_event_types(
-        self, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> EventTypesEnvelope:
+    async def get_types(self, *, request_options: typing.Optional[RequestOptions] = None) -> EventTypesEnvelope:
         """
         Parameters:
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.events.api_v_2_get_event_types()
+        await client.events.get_types()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/events_types"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
@@ -282,9 +291,9 @@
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(EventTypesEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `polytomic-0.1.2/src/polytomic/resources/jobs/client.py` & `polytomic-0.2.0/src/polytomic/resources/identity/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,49 @@
 # This file was auto-generated from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from ...core.api_error import ApiError
+from ...core.api_error import ApiError as core_api_error_ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ...core.request_options import RequestOptions
+from ...errors.internal_server_error import InternalServerError
 from ...errors.unauthorized_error import UnauthorizedError
-from ...types.job_response_envelope import JobResponseEnvelope
+from ...types.api_error import ApiError as types_api_error_ApiError
+from ...types.get_identity_response_envelope import GetIdentityResponseEnvelope
 from ...types.rest_err_response import RestErrResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class JobsClient:
+class IdentityClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def get(
-        self, id: str, type: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> JobResponseEnvelope:
+    def get(self, *, request_options: typing.Optional[RequestOptions] = None) -> GetIdentityResponseEnvelope:
         """
         Parameters:
-            - id: str.
-
-            - type: str.
-
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.jobs.get(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            type="createmodel",
-        )
+        client.identity.get()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/jobs/{jsonable_encoder(type)}/{jsonable_encoder(id)}"
-            ),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/me"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -64,55 +54,45 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(JobResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(GetIdentityResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncJobsClient:
+class AsyncIdentityClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def get(
-        self, id: str, type: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> JobResponseEnvelope:
+    async def get(self, *, request_options: typing.Optional[RequestOptions] = None) -> GetIdentityResponseEnvelope:
         """
         Parameters:
-            - id: str.
-
-            - type: str.
-
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.jobs.get(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            type="createmodel",
-        )
+        await client.identity.get()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/jobs/{jsonable_encoder(type)}/{jsonable_encoder(id)}"
-            ),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/me"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -123,15 +103,17 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(JobResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(GetIdentityResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `polytomic-0.1.2/src/polytomic/resources/model_sync/resources/executions/client.py` & `polytomic-0.2.0/src/polytomic/resources/users/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,112 +1,65 @@
 # This file was auto-generated from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from .....core.api_error import ApiError
-from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
-from .....core.jsonable_encoder import jsonable_encoder
-from .....core.remove_none_from_dict import remove_none_from_dict
-from .....core.request_options import RequestOptions
-from .....errors.unauthorized_error import UnauthorizedError
-from .....types.execution_logs_response_envelope import ExecutionLogsResponseEnvelope
-from .....types.get_execution_response_envelope import GetExecutionResponseEnvelope
-from .....types.list_execution_response_envelope import ListExecutionResponseEnvelope
-from .....types.rest_err_response import RestErrResponse
+from ...core.api_error import ApiError as core_api_error_ApiError
+from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from ...core.jsonable_encoder import jsonable_encoder
+from ...core.remove_none_from_dict import remove_none_from_dict
+from ...core.request_options import RequestOptions
+from ...errors.internal_server_error import InternalServerError
+from ...errors.not_found_error import NotFoundError
+from ...errors.unauthorized_error import UnauthorizedError
+from ...errors.unprocessable_entity_error import UnprocessableEntityError
+from ...types.api_error import ApiError as types_api_error_ApiError
+from ...types.api_key_response_envelope import ApiKeyResponseEnvelope
+from ...types.list_users_envelope import ListUsersEnvelope
+from ...types.rest_err_response import RestErrResponse
+from ...types.user_envelope import UserEnvelope
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
+# this is used as the default value for optional parameters
+OMIT = typing.cast(typing.Any, ...)
 
-class ExecutionsClient:
+
+class UsersClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def list(
-        self, sync_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> ListExecutionResponseEnvelope:
+    def list(self, org_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> ListUsersEnvelope:
         """
-        Parameters:
-            - sync_id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.model_sync.executions.list(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/syncs/{jsonable_encoder(sync_id)}/executions"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ListExecutionResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
 
-    def get(
-        self, sync_id: str, id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> GetExecutionResponseEnvelope:
-        """
         Parameters:
-            - sync_id: str.
-
-            - id: str.
+            - org_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.model_sync.executions.get(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        client.users.list(
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}",
+                f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{jsonable_encoder(org_id)}/users"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -118,112 +71,75 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetExecutionResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ListUsersEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_error_log_ur_ls(
-        self, sync_id: str, id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> ExecutionLogsResponseEnvelope:
-        """
-        Parameters:
-            - sync_id: str.
-
-            - id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import Polytomic
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-        client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.model_sync.executions.get_error_log_ur_ls(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
+    def create(
+        self,
+        org_id: str,
+        *,
+        email: str,
+        role: typing.Optional[str] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> UserEnvelope:
         """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/errors",
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ExecutionLogsResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
 
-    def get_error_logs(
-        self, sync_id: str, id: str, filename: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> None:
-        """
         Parameters:
-            - sync_id: str.
+            - org_id: str.
 
-            - id: str.
+            - email: str.
 
-            - filename: str.
+            - role: typing.Optional[str].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.model_sync.executions.get_error_logs(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            filename="path/to/file.json",
+        client.users.create(
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            email="mail@example.com",
+            role="admin",
         )
         """
+        _request: typing.Dict[str, typing.Any] = {"email": email}
+        if role is not OMIT:
+            _request["role"] = role
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
+            "POST",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/errors/{jsonable_encoder(filename)}",
+                f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{jsonable_encoder(org_id)}/users"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -231,108 +147,57 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_insert_log_ur_ls(
-        self, sync_id: str, id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> ExecutionLogsResponseEnvelope:
-        """
-        Parameters:
-            - sync_id: str.
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-            - id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.model_sync.executions.get_insert_log_ur_ls(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
+    def get(self, id: str, org_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> UserEnvelope:
         """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/inserts",
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ExecutionLogsResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
 
-    def get_insert_logs(
-        self, sync_id: str, id: str, filename: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> None:
-        """
         Parameters:
-            - sync_id: str.
-
             - id: str.
 
-            - filename: str.
+            - org_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.model_sync.executions.get_insert_logs(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        client.users.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            filename="path/to/file.json",
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
-                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/inserts/{jsonable_encoder(filename)}",
+                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -344,167 +209,82 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_record_log_ur_ls(
-        self, sync_id: str, id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> ExecutionLogsResponseEnvelope:
+    def update(
+        self,
+        id: str,
+        org_id: str,
+        *,
+        email: str,
+        role: typing.Optional[str] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> UserEnvelope:
         """
-        Parameters:
-            - sync_id: str.
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
 
-            - id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.model_sync.executions.get_record_log_ur_ls(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/records",
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ExecutionLogsResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_record_logs(
-        self, sync_id: str, id: str, filename: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> None:
-        """
         Parameters:
-            - sync_id: str.
-
             - id: str.
 
-            - filename: str.
+            - org_id: str.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import Polytomic
+            - email: str.
 
-        client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.model_sync.executions.get_record_logs(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            filename="path/to/file.json",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/records/{jsonable_encoder(filename)}",
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_update_log_ur_ls(
-        self, sync_id: str, id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> ExecutionLogsResponseEnvelope:
-        """
-        Parameters:
-            - sync_id: str.
-
-            - id: str.
+            - role: typing.Optional[str].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.model_sync.executions.get_update_log_ur_ls(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        client.users.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            email="mail@example.com",
+            role="admin",
         )
         """
+        _request: typing.Dict[str, typing.Any] = {"email": email}
+        if role is not OMIT:
+            _request["role"] = role
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
+            "PUT",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
-                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/updates",
+                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -512,53 +292,57 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ExecutionLogsResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_update_logs(
-        self, sync_id: str, id: str, filename: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> None:
+    def remove(self, id: str, org_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> UserEnvelope:
         """
-        Parameters:
-            - sync_id: str.
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
 
+        Parameters:
             - id: str.
 
-            - filename: str.
+            - org_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.model_sync.executions.get_update_logs(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        client.users.remove(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            filename="path/to/file.json",
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
+            "DELETE",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
-                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/updates/{jsonable_encoder(filename)}",
+                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -570,112 +354,81 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_warning_log_ur_ls(
-        self, sync_id: str, id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> ExecutionLogsResponseEnvelope:
+    def create_api_key(
+        self,
+        org_id: str,
+        id: str,
+        *,
+        force: typing.Optional[bool] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> ApiKeyResponseEnvelope:
         """
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+
         Parameters:
-            - sync_id: str.
+            - org_id: str.
 
             - id: str.
 
+            - force: typing.Optional[bool].
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.model_sync.executions.get_warning_log_ur_ls(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        client.users.create_api_key(
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            force=True,
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
+            "POST",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
-                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/warnings",
+                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}/keys",
             ),
             params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                        "force": force,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
                     }
                 )
             ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ExecutionLogsResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_warning_logs(
-        self, sync_id: str, id: str, filename: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> None:
-        """
-        Parameters:
-            - sync_id: str.
-
-            - id: str.
-
-            - filename: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.model_sync.executions.get_warning_logs(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            filename="path/to/file.json",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/warnings/{jsonable_encoder(filename)}",
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -683,106 +436,56 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic.parse_obj_as(ApiKeyResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncExecutionsClient:
+class AsyncUsersClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def list(
-        self, sync_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> ListExecutionResponseEnvelope:
+    async def list(self, org_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> ListUsersEnvelope:
         """
-        Parameters:
-            - sync_id: str.
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.model_sync.executions.list(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/syncs/{jsonable_encoder(sync_id)}/executions"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ListExecutionResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get(
-        self, sync_id: str, id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> GetExecutionResponseEnvelope:
-        """
         Parameters:
-            - sync_id: str.
-
-            - id: str.
+            - org_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.model_sync.executions.get(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        await client.users.list(
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}",
+                f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{jsonable_encoder(org_id)}/users"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -794,112 +497,75 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetExecutionResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ListUsersEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_error_log_ur_ls(
-        self, sync_id: str, id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> ExecutionLogsResponseEnvelope:
+    async def create(
+        self,
+        org_id: str,
+        *,
+        email: str,
+        role: typing.Optional[str] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> UserEnvelope:
         """
-        Parameters:
-            - sync_id: str.
-
-            - id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import AsyncPolytomic
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
 
-        client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.model_sync.executions.get_error_log_ur_ls(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/errors",
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ExecutionLogsResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get_error_logs(
-        self, sync_id: str, id: str, filename: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> None:
-        """
         Parameters:
-            - sync_id: str.
+            - org_id: str.
 
-            - id: str.
+            - email: str.
 
-            - filename: str.
+            - role: typing.Optional[str].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.model_sync.executions.get_error_logs(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            filename="path/to/file.json",
+        await client.users.create(
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            email="mail@example.com",
+            role="admin",
         )
         """
+        _request: typing.Dict[str, typing.Any] = {"email": email}
+        if role is not OMIT:
+            _request["role"] = role
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
+            "POST",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/errors/{jsonable_encoder(filename)}",
+                f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{jsonable_encoder(org_id)}/users"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -907,108 +573,59 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_insert_log_ur_ls(
-        self, sync_id: str, id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> ExecutionLogsResponseEnvelope:
-        """
-        Parameters:
-            - sync_id: str.
-
-            - id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.model_sync.executions.get_insert_log_ur_ls(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
+    async def get(
+        self, id: str, org_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> UserEnvelope:
         """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/inserts",
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ExecutionLogsResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
 
-    async def get_insert_logs(
-        self, sync_id: str, id: str, filename: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> None:
-        """
         Parameters:
-            - sync_id: str.
-
             - id: str.
 
-            - filename: str.
+            - org_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.model_sync.executions.get_insert_logs(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        await client.users.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            filename="path/to/file.json",
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
-                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/inserts/{jsonable_encoder(filename)}",
+                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -1020,167 +637,82 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_record_log_ur_ls(
-        self, sync_id: str, id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> ExecutionLogsResponseEnvelope:
+    async def update(
+        self,
+        id: str,
+        org_id: str,
+        *,
+        email: str,
+        role: typing.Optional[str] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> UserEnvelope:
         """
-        Parameters:
-            - sync_id: str.
-
-            - id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.model_sync.executions.get_record_log_ur_ls(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/records",
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ExecutionLogsResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
 
-    async def get_record_logs(
-        self, sync_id: str, id: str, filename: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> None:
-        """
         Parameters:
-            - sync_id: str.
-
             - id: str.
 
-            - filename: str.
+            - org_id: str.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import AsyncPolytomic
+            - email: str.
 
-        client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.model_sync.executions.get_record_logs(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            filename="path/to/file.json",
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/records/{jsonable_encoder(filename)}",
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get_update_log_ur_ls(
-        self, sync_id: str, id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> ExecutionLogsResponseEnvelope:
-        """
-        Parameters:
-            - sync_id: str.
-
-            - id: str.
+            - role: typing.Optional[str].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.model_sync.executions.get_update_log_ur_ls(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        await client.users.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            email="mail@example.com",
+            role="admin",
         )
         """
+        _request: typing.Dict[str, typing.Any] = {"email": email}
+        if role is not OMIT:
+            _request["role"] = role
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
+            "PUT",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
-                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/updates",
+                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -1188,53 +720,59 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ExecutionLogsResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_update_logs(
-        self, sync_id: str, id: str, filename: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> None:
+    async def remove(
+        self, id: str, org_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> UserEnvelope:
         """
-        Parameters:
-            - sync_id: str.
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
 
+        Parameters:
             - id: str.
 
-            - filename: str.
+            - org_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.model_sync.executions.get_update_logs(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        await client.users.remove(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            filename="path/to/file.json",
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
+            "DELETE",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
-                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/updates/{jsonable_encoder(filename)}",
+                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -1246,112 +784,81 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_warning_log_ur_ls(
-        self, sync_id: str, id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> ExecutionLogsResponseEnvelope:
+    async def create_api_key(
+        self,
+        org_id: str,
+        id: str,
+        *,
+        force: typing.Optional[bool] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> ApiKeyResponseEnvelope:
         """
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+
         Parameters:
-            - sync_id: str.
+            - org_id: str.
 
             - id: str.
 
+            - force: typing.Optional[bool].
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.model_sync.executions.get_warning_log_ur_ls(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        await client.users.create_api_key(
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            force=True,
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
+            "POST",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
-                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/warnings",
+                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}/keys",
             ),
             params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                        "force": force,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
                     }
                 )
             ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ExecutionLogsResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get_warning_logs(
-        self, sync_id: str, id: str, filename: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> None:
-        """
-        Parameters:
-            - sync_id: str.
-
-            - id: str.
-
-            - filename: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.model_sync.executions.get_warning_logs(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            filename="path/to/file.json",
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/syncs/{jsonable_encoder(sync_id)}/executions/{jsonable_encoder(id)}/warnings/{jsonable_encoder(filename)}",
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -1359,15 +866,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic.parse_obj_as(ApiKeyResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `polytomic-0.1.2/src/polytomic/resources/models/client.py` & `polytomic-0.2.0/src/polytomic/resources/models/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 # This file was auto-generated from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from ...core.api_error import ApiError
+from ...core.api_error import ApiError as core_api_error_ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ...core.request_options import RequestOptions
+from ...errors.bad_request_error import BadRequestError
+from ...errors.forbidden_error import ForbiddenError
+from ...errors.internal_server_error import InternalServerError
+from ...errors.not_found_error import NotFoundError
 from ...errors.unauthorized_error import UnauthorizedError
+from ...types.api_error import ApiError as types_api_error_ApiError
 from ...types.model_list_response_envelope import ModelListResponseEnvelope
 from ...types.model_model_field_request import ModelModelFieldRequest
 from ...types.model_relation import ModelRelation
 from ...types.model_response_envelope import ModelResponseEnvelope
 from ...types.rest_err_response import RestErrResponse
 
 try:
@@ -33,15 +38,14 @@
         """
         Parameters:
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         client.models.list()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/models"),
@@ -62,19 +66,21 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ModelListResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
         self,
         *,
         async_: typing.Optional[bool] = None,
         additional_fields: typing.Optional[typing.Sequence[ModelModelFieldRequest]] = OMIT,
         configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
@@ -116,15 +122,14 @@
             - tracking_columns: typing.Optional[typing.Sequence[str]].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         client.models.create(
             connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
             identifier="id",
             name="Users",
         )
@@ -181,33 +186,38 @@
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ModelResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> ModelResponseEnvelope:
         """
         Parameters:
             - id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         client.models.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
@@ -230,66 +240,23 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ModelResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def remove(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
-        """
-        Parameters:
-            - id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.models.remove(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/models/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def update(
         self,
         id: str,
         *,
         async_: typing.Optional[bool] = None,
         additional_fields: typing.Optional[typing.Sequence[ModelModelFieldRequest]] = OMIT,
@@ -334,15 +301,14 @@
             - tracking_columns: typing.Optional[typing.Sequence[str]].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         client.models.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             async_=False,
             connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
             identifier="id",
@@ -365,15 +331,15 @@
         if policies is not OMIT:
             _request["policies"] = policies
         if relations is not OMIT:
             _request["relations"] = relations
         if tracking_columns is not OMIT:
             _request["tracking_columns"] = tracking_columns
         _response = self._client_wrapper.httpx_client.request(
-            "PATCH",
+            "PUT",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/models/{jsonable_encoder(id)}"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "async": async_,
                         **(
                             request_options.get("additional_query_parameters", {})
@@ -401,36 +367,93 @@
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ModelResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 401:
+            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
+
+    def remove(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
+        """
+        Parameters:
+            - id: str.
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from polytomic.client import Polytomic
+
+        client = Polytomic(
+            token="YOUR_TOKEN",
+        )
+        client.models.remove(
+            id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        )
+        """
+        _response = self._client_wrapper.httpx_client.request(
+            "DELETE",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/models/{jsonable_encoder(id)}"),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncModelsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> ModelListResponseEnvelope:
         """
         Parameters:
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         await client.models.list()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/models"),
@@ -451,19 +474,21 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ModelListResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
         self,
         *,
         async_: typing.Optional[bool] = None,
         additional_fields: typing.Optional[typing.Sequence[ModelModelFieldRequest]] = OMIT,
         configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
@@ -505,15 +530,14 @@
             - tracking_columns: typing.Optional[typing.Sequence[str]].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         await client.models.create(
             connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
             identifier="id",
             name="Users",
         )
@@ -570,33 +594,38 @@
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ModelResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> ModelResponseEnvelope:
         """
         Parameters:
             - id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         await client.models.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
@@ -619,66 +648,23 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ModelResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def remove(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
-        """
-        Parameters:
-            - id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.models.remove(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/models/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update(
         self,
         id: str,
         *,
         async_: typing.Optional[bool] = None,
         additional_fields: typing.Optional[typing.Sequence[ModelModelFieldRequest]] = OMIT,
@@ -723,15 +709,14 @@
             - tracking_columns: typing.Optional[typing.Sequence[str]].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         await client.models.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             async_=False,
             connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
             identifier="id",
@@ -754,15 +739,15 @@
         if policies is not OMIT:
             _request["policies"] = policies
         if relations is not OMIT:
             _request["relations"] = relations
         if tracking_columns is not OMIT:
             _request["tracking_columns"] = tracking_columns
         _response = await self._client_wrapper.httpx_client.request(
-            "PATCH",
+            "PUT",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/models/{jsonable_encoder(id)}"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "async": async_,
                         **(
                             request_options.get("additional_query_parameters", {})
@@ -790,14 +775,72 @@
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ModelResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 401:
+            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def remove(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
+        """
+        Parameters:
+            - id: str.
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from polytomic.client import AsyncPolytomic
+
+        client = AsyncPolytomic(
+            token="YOUR_TOKEN",
+        )
+        await client.models.remove(
+            id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        )
+        """
+        _response = await self._client_wrapper.httpx_client.request(
+            "DELETE",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/models/{jsonable_encoder(id)}"),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `polytomic-0.1.2/src/polytomic/resources/organization/client.py` & `polytomic-0.2.0/src/polytomic/resources/organization/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # This file was auto-generated from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from ...core.api_error import ApiError
+from ...core.api_error import ApiError as core_api_error_ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ...core.request_options import RequestOptions
+from ...errors.internal_server_error import InternalServerError
+from ...errors.not_found_error import NotFoundError
 from ...errors.unauthorized_error import UnauthorizedError
+from ...errors.unprocessable_entity_error import UnprocessableEntityError
+from ...types.api_error import ApiError as types_api_error_ApiError
 from ...types.organization_envelope import OrganizationEnvelope
 from ...types.organizations_envelope import OrganizationsEnvelope
 from ...types.rest_err_response import RestErrResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
@@ -35,15 +39,14 @@
 
         Parameters:
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         client.organization.list()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/organizations"),
@@ -64,19 +67,21 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(OrganizationsEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
         self,
         *,
         client_id: typing.Optional[str] = OMIT,
         client_secret: typing.Optional[str] = OMIT,
         issuer: typing.Optional[str] = OMIT,
@@ -104,15 +109,14 @@
             - sso_org_id: typing.Optional[str].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         client.organization.create(
             client_id="client_id",
             client_secret="client_secret",
             issuer="https://example.com",
             name="My Organization",
@@ -157,19 +161,25 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(OrganizationEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> OrganizationEnvelope:
         """
         > 🚧 Requires partner key
         >
         > Organization endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
 
@@ -177,15 +187,14 @@
             - id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         client.organization.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
@@ -210,72 +219,21 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(OrganizationEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def remove(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
-        """
-        > 🚧 Requires partner key
-        >
-        > Organization endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
-
-        Parameters:
-            - id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.organization.remove(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{jsonable_encoder(id)}"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def update(
         self,
         id: str,
         *,
         client_id: typing.Optional[str] = OMIT,
         client_secret: typing.Optional[str] = OMIT,
@@ -306,15 +264,14 @@
             - sso_org_id: typing.Optional[str].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         client.organization.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             client_id="client_id",
             client_secret="client_secret",
             issuer="https://example.com",
@@ -331,15 +288,15 @@
         if issuer is not OMIT:
             _request["issuer"] = issuer
         if sso_domain is not OMIT:
             _request["sso_domain"] = sso_domain
         if sso_org_id is not OMIT:
             _request["sso_org_id"] = sso_org_id
         _response = self._client_wrapper.httpx_client.request(
-            "PATCH",
+            "PUT",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{jsonable_encoder(id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
@@ -362,19 +319,81 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(OrganizationEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
+
+    def remove(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
+        """
+        > 🚧 Requires partner key
+        >
+        > Organization endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+
+        Parameters:
+            - id: str.
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from polytomic.client import Polytomic
+
+        client = Polytomic(
+            token="YOUR_TOKEN",
+        )
+        client.organization.remove(
+            id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        )
+        """
+        _response = self._client_wrapper.httpx_client.request(
+            "DELETE",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{jsonable_encoder(id)}"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return
+        if _response.status_code == 401:
+            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncOrganizationClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> OrganizationsEnvelope:
@@ -385,15 +404,14 @@
 
         Parameters:
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         await client.organization.list()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/organizations"),
@@ -414,19 +432,21 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(OrganizationsEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
         self,
         *,
         client_id: typing.Optional[str] = OMIT,
         client_secret: typing.Optional[str] = OMIT,
         issuer: typing.Optional[str] = OMIT,
@@ -454,15 +474,14 @@
             - sso_org_id: typing.Optional[str].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         await client.organization.create(
             client_id="client_id",
             client_secret="client_secret",
             issuer="https://example.com",
             name="My Organization",
@@ -507,19 +526,25 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(OrganizationEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> OrganizationEnvelope:
         """
         > 🚧 Requires partner key
         >
         > Organization endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
 
@@ -527,15 +552,14 @@
             - id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         await client.organization.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
@@ -560,72 +584,21 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(OrganizationEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def remove(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
-        """
-        > 🚧 Requires partner key
-        >
-        > Organization endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
-
-        Parameters:
-            - id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.organization.remove(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{jsonable_encoder(id)}"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update(
         self,
         id: str,
         *,
         client_id: typing.Optional[str] = OMIT,
         client_secret: typing.Optional[str] = OMIT,
@@ -656,15 +629,14 @@
             - sso_org_id: typing.Optional[str].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
         await client.organization.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
             client_id="client_id",
             client_secret="client_secret",
             issuer="https://example.com",
@@ -681,15 +653,15 @@
         if issuer is not OMIT:
             _request["issuer"] = issuer
         if sso_domain is not OMIT:
             _request["sso_domain"] = sso_domain
         if sso_org_id is not OMIT:
             _request["sso_org_id"] = sso_org_id
         _response = await self._client_wrapper.httpx_client.request(
-            "PATCH",
+            "PUT",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{jsonable_encoder(id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
@@ -712,12 +684,74 @@
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(OrganizationEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def remove(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
+        """
+        > 🚧 Requires partner key
+        >
+        > Organization endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+
+        Parameters:
+            - id: str.
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from polytomic.client import AsyncPolytomic
+
+        client = AsyncPolytomic(
+            token="YOUR_TOKEN",
+        )
+        await client.organization.remove(
+            id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        )
+        """
+        _response = await self._client_wrapper.httpx_client.request(
+            "DELETE",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{jsonable_encoder(id)}"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return
+        if _response.status_code == 401:
+            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `polytomic-0.1.2/src/polytomic/resources/permissions/client.py` & `polytomic-0.2.0/src/polytomic/resources/permissions/client.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/resources/permissions/resources/policies/client.py` & `polytomic-0.2.0/src/polytomic/resources/webhooks/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,61 @@
 # This file was auto-generated from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from .....core.api_error import ApiError
-from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
-from .....core.jsonable_encoder import jsonable_encoder
-from .....core.remove_none_from_dict import remove_none_from_dict
-from .....core.request_options import RequestOptions
-from .....errors.unauthorized_error import UnauthorizedError
-from .....types.list_policies_response_envelope import ListPoliciesResponseEnvelope
-from .....types.policy_action import PolicyAction
-from .....types.policy_response_envelope import PolicyResponseEnvelope
-from .....types.rest_err_response import RestErrResponse
+from ...core.api_error import ApiError as core_api_error_ApiError
+from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from ...core.jsonable_encoder import jsonable_encoder
+from ...core.remove_none_from_dict import remove_none_from_dict
+from ...core.request_options import RequestOptions
+from ...errors.internal_server_error import InternalServerError
+from ...errors.not_found_error import NotFoundError
+from ...errors.unauthorized_error import UnauthorizedError
+from ...errors.unprocessable_entity_error import UnprocessableEntityError
+from ...types.api_error import ApiError as types_api_error_ApiError
+from ...types.rest_err_response import RestErrResponse
+from ...types.webhook_envelope import WebhookEnvelope
+from ...types.webhook_list_envelope import WebhookListEnvelope
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class PoliciesClient:
+class WebhooksClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> ListPoliciesResponseEnvelope:
+    def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> WebhookListEnvelope:
         """
+        Webooks can be set up using the webhook API endpoints. Currently, only one
+        webhook may be created per organization. The webhook will be called for events
+        in that organization.
+
+        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
+
         Parameters:
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.permissions.policies.list()
+        client.webhooks.list()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/permissions/policies"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/webhooks"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -58,66 +66,65 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ListPoliciesResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(WebhookListEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
         self,
         *,
-        name: str,
+        endpoint: str,
         organization_id: typing.Optional[str] = OMIT,
-        policy_actions: typing.Optional[typing.Sequence[PolicyAction]] = OMIT,
+        secret: str,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> PolicyResponseEnvelope:
+    ) -> WebhookEnvelope:
         """
+        Webooks can be set up using the webhook API endpoints. Currently, only one
+        webhook may be created per organization. The webhook will be called for events
+        in that organization.
+
+        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
+
         Parameters:
-            - name: str.
+            - endpoint: str.
 
             - organization_id: typing.Optional[str].
 
-            - policy_actions: typing.Optional[typing.Sequence[PolicyAction]].
+            - secret: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from polytomic import PolicyAction
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.permissions.policies.create(
-            name="Custom",
-            policy_actions=[
-                PolicyAction(
-                    action="read",
-                    role_ids=["248df4b7-aa70-47b8-a036-33ac447e668d"],
-                )
-            ],
+        client.webhooks.create(
+            endpoint="https://example.com/webhook",
+            secret="secret",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"name": name}
+        _request: typing.Dict[str, typing.Any] = {"endpoint": endpoint, "secret": secret}
         if organization_id is not OMIT:
             _request["organization_id"] = organization_id
-        if policy_actions is not OMIT:
-            _request["policy_actions"] = policy_actions
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/permissions/policies"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/webhooks"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -134,45 +141,54 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PolicyResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(WebhookEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> PolicyResponseEnvelope:
+    def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> WebhookEnvelope:
         """
+        Webooks can be set up using the webhook API endpoints. Currently, only one
+        webhook may be created per organization. The webhook will be called for events
+        in that organization.
+
+        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
+
         Parameters:
             - id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.permissions.policies.get(
+        client.webhooks.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/permissions/policies/{jsonable_encoder(id)}"
-            ),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/webhooks/{jsonable_encoder(id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -183,48 +199,78 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PolicyResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(WebhookEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    def delete(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
+    def update(
+        self,
+        id: str,
+        *,
+        endpoint: str,
+        organization_id: typing.Optional[str] = OMIT,
+        secret: str,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> WebhookEnvelope:
         """
+        Webooks can be set up using the webhook API endpoints. Currently, only one
+        webhook may be created per organization. The webhook will be called for events
+        in that organization.
+
+        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
+
         Parameters:
             - id: str.
 
+            - endpoint: str.
+
+            - organization_id: typing.Optional[str].
+
+            - secret: str.
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.permissions.policies.delete(
+        client.webhooks.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            endpoint="https://example.com/webhook",
+            secret="secret",
         )
         """
+        _request: typing.Dict[str, typing.Any] = {"endpoint": endpoint, "secret": secret}
+        if organization_id is not OMIT:
+            _request["organization_id"] = organization_id
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/permissions/policies/{jsonable_encoder(id)}"
-            ),
+            "PUT",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/webhooks/{jsonable_encoder(id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -232,81 +278,51 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic.parse_obj_as(WebhookEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update(
-        self,
-        id: str,
-        *,
-        name: str,
-        organization_id: typing.Optional[str] = OMIT,
-        policy_actions: typing.Optional[typing.Sequence[PolicyAction]] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> PolicyResponseEnvelope:
+    def remove(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
         Parameters:
             - id: str.
 
-            - name: str.
-
-            - organization_id: typing.Optional[str].
-
-            - policy_actions: typing.Optional[typing.Sequence[PolicyAction]].
-
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from polytomic import PolicyAction
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.permissions.policies.update(
+        client.webhooks.remove(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            name="Custom",
-            policy_actions=[
-                PolicyAction(
-                    action="read",
-                    role_ids=["248df4b7-aa70-47b8-a036-33ac447e668d"],
-                )
-            ],
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"name": name}
-        if organization_id is not OMIT:
-            _request["organization_id"] = organization_id
-        if policy_actions is not OMIT:
-            _request["policy_actions"] = policy_actions
         _response = self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/permissions/policies/{jsonable_encoder(id)}"
-            ),
+            "DELETE",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/webhooks/{jsonable_encoder(id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -314,44 +330,53 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PolicyResponseEnvelope, _response.json())  # type: ignore
+            return
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncPoliciesClient:
+class AsyncWebhooksClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> ListPoliciesResponseEnvelope:
+    async def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> WebhookListEnvelope:
         """
+        Webooks can be set up using the webhook API endpoints. Currently, only one
+        webhook may be created per organization. The webhook will be called for events
+        in that organization.
+
+        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
+
         Parameters:
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.permissions.policies.list()
+        await client.webhooks.list()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/permissions/policies"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/webhooks"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -362,66 +387,65 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ListPoliciesResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(WebhookListEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
         self,
         *,
-        name: str,
+        endpoint: str,
         organization_id: typing.Optional[str] = OMIT,
-        policy_actions: typing.Optional[typing.Sequence[PolicyAction]] = OMIT,
+        secret: str,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> PolicyResponseEnvelope:
+    ) -> WebhookEnvelope:
         """
+        Webooks can be set up using the webhook API endpoints. Currently, only one
+        webhook may be created per organization. The webhook will be called for events
+        in that organization.
+
+        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
+
         Parameters:
-            - name: str.
+            - endpoint: str.
 
             - organization_id: typing.Optional[str].
 
-            - policy_actions: typing.Optional[typing.Sequence[PolicyAction]].
+            - secret: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from polytomic import PolicyAction
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.permissions.policies.create(
-            name="Custom",
-            policy_actions=[
-                PolicyAction(
-                    action="read",
-                    role_ids=["248df4b7-aa70-47b8-a036-33ac447e668d"],
-                )
-            ],
+        await client.webhooks.create(
+            endpoint="https://example.com/webhook",
+            secret="secret",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"name": name}
+        _request: typing.Dict[str, typing.Any] = {"endpoint": endpoint, "secret": secret}
         if organization_id is not OMIT:
             _request["organization_id"] = organization_id
-        if policy_actions is not OMIT:
-            _request["policy_actions"] = policy_actions
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/permissions/policies"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/webhooks"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -438,45 +462,54 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PolicyResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(WebhookEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> PolicyResponseEnvelope:
+    async def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> WebhookEnvelope:
         """
+        Webooks can be set up using the webhook API endpoints. Currently, only one
+        webhook may be created per organization. The webhook will be called for events
+        in that organization.
+
+        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
+
         Parameters:
             - id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.permissions.policies.get(
+        await client.webhooks.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/permissions/policies/{jsonable_encoder(id)}"
-            ),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/webhooks/{jsonable_encoder(id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -487,48 +520,78 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PolicyResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(WebhookEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def delete(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
+    async def update(
+        self,
+        id: str,
+        *,
+        endpoint: str,
+        organization_id: typing.Optional[str] = OMIT,
+        secret: str,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> WebhookEnvelope:
         """
+        Webooks can be set up using the webhook API endpoints. Currently, only one
+        webhook may be created per organization. The webhook will be called for events
+        in that organization.
+
+        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
+
         Parameters:
             - id: str.
 
+            - endpoint: str.
+
+            - organization_id: typing.Optional[str].
+
+            - secret: str.
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.permissions.policies.delete(
+        await client.webhooks.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            endpoint="https://example.com/webhook",
+            secret="secret",
         )
         """
+        _request: typing.Dict[str, typing.Any] = {"endpoint": endpoint, "secret": secret}
+        if organization_id is not OMIT:
+            _request["organization_id"] = organization_id
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/permissions/policies/{jsonable_encoder(id)}"
-            ),
+            "PUT",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/webhooks/{jsonable_encoder(id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -536,81 +599,51 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic.parse_obj_as(WebhookEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update(
-        self,
-        id: str,
-        *,
-        name: str,
-        organization_id: typing.Optional[str] = OMIT,
-        policy_actions: typing.Optional[typing.Sequence[PolicyAction]] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> PolicyResponseEnvelope:
+    async def remove(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
         Parameters:
             - id: str.
 
-            - name: str.
-
-            - organization_id: typing.Optional[str].
-
-            - policy_actions: typing.Optional[typing.Sequence[PolicyAction]].
-
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from polytomic import PolicyAction
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.permissions.policies.update(
+        await client.webhooks.remove(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            name="Custom",
-            policy_actions=[
-                PolicyAction(
-                    action="read",
-                    role_ids=["248df4b7-aa70-47b8-a036-33ac447e668d"],
-                )
-            ],
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"name": name}
-        if organization_id is not OMIT:
-            _request["organization_id"] = organization_id
-        if policy_actions is not OMIT:
-            _request["policy_actions"] = policy_actions
         _response = await self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/permissions/policies/{jsonable_encoder(id)}"
-            ),
+            "DELETE",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/webhooks/{jsonable_encoder(id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -618,15 +651,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PolicyResponseEnvelope, _response.json())  # type: ignore
+            return
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `polytomic-0.1.2/src/polytomic/resources/permissions/resources/roles/client.py` & `polytomic-0.2.0/src/polytomic/resources/bulk_sync/resources/schemas/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,82 @@
 # This file was auto-generated from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from .....core.api_error import ApiError
+from .....core.api_error import ApiError as core_api_error_ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .....core.jsonable_encoder import jsonable_encoder
 from .....core.remove_none_from_dict import remove_none_from_dict
 from .....core.request_options import RequestOptions
+from .....errors.forbidden_error import ForbiddenError
+from .....errors.internal_server_error import InternalServerError
+from .....errors.not_found_error import NotFoundError
 from .....errors.unauthorized_error import UnauthorizedError
+from .....types.api_error import ApiError as types_api_error_ApiError
+from .....types.bulk_field import BulkField
+from .....types.bulk_schema import BulkSchema
+from .....types.bulk_schema_envelope import BulkSchemaEnvelope
+from .....types.list_bulk_schema import ListBulkSchema
 from .....types.rest_err_response import RestErrResponse
-from .....types.role_list_response_envelope import RoleListResponseEnvelope
-from .....types.role_response_envelope import RoleResponseEnvelope
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class RolesClient:
+class SchemasClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> RoleListResponseEnvelope:
+    def list(
+        self,
+        id: str,
+        *,
+        filters: typing.Optional[typing.Dict[str, typing.Optional[str]]] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> ListBulkSchema:
         """
         Parameters:
+            - id: str.
+
+            - filters: typing.Optional[typing.Dict[str, typing.Optional[str]]].
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.permissions.roles.list()
+        client.bulk_sync.schemas.list(
+            id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/permissions/roles"),
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}/schemas"
+            ),
             params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+                remove_none_from_dict(
+                    {
+                        "filters": jsonable_encoder(filters),
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -57,54 +85,57 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RoleListResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ListBulkSchema, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create(
+    def patch(
         self,
+        id: str,
         *,
-        name: str,
-        organization_id: typing.Optional[str] = OMIT,
+        schemas: typing.Optional[typing.Sequence[BulkSchema]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> RoleResponseEnvelope:
+    ) -> ListBulkSchema:
         """
         Parameters:
-            - name: str.
+            - id: str.
 
-            - organization_id: typing.Optional[str].
+            - schemas: typing.Optional[typing.Sequence[BulkSchema]].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.permissions.roles.create(
-            name="Custom",
+        client.bulk_sync.schemas.patch(
+            id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"name": name}
-        if organization_id is not OMIT:
-            _request["organization_id"] = organization_id
+        _request: typing.Dict[str, typing.Any] = {}
+        if schemas is not OMIT:
+            _request["schemas"] = schemas
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/permissions/roles"),
+            "PATCH",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}/schemas"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -121,93 +152,55 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RoleResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ListBulkSchema, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> RoleResponseEnvelope:
+    def get(
+        self, id: str, schema_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> BulkSchemaEnvelope:
         """
         Parameters:
             - id: str.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.permissions.roles.get(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/permissions/roles/{jsonable_encoder(id)}"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RoleResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def delete(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
-        """
-        Parameters:
-            - id: str.
+            - schema_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.permissions.roles.delete(
+        client.bulk_sync.schemas.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            schema_id="Contact",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
+            "GET",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/permissions/roles/{jsonable_encoder(id)}"
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/bulk/syncs/{jsonable_encoder(id)}/schemas/{jsonable_encoder(schema_id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -219,59 +212,73 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic.parse_obj_as(BulkSchemaEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def update(
         self,
         id: str,
+        schema_id: str,
         *,
-        name: str,
-        organization_id: typing.Optional[str] = OMIT,
+        enabled: typing.Optional[bool] = OMIT,
+        fields: typing.Optional[typing.Sequence[BulkField]] = OMIT,
+        partition_key: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> RoleResponseEnvelope:
+    ) -> BulkSchemaEnvelope:
         """
         Parameters:
             - id: str.
 
-            - name: str.
+            - schema_id: str.
+
+            - enabled: typing.Optional[bool].
 
-            - organization_id: typing.Optional[str].
+            - fields: typing.Optional[typing.Sequence[BulkField]].
+
+            - partition_key: typing.Optional[str].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.permissions.roles.update(
+        client.bulk_sync.schemas.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            name="Custom",
+            schema_id="contact",
+            enabled=True,
+            partition_key="email",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"name": name}
-        if organization_id is not OMIT:
-            _request["organization_id"] = organization_id
+        _request: typing.Dict[str, typing.Any] = {}
+        if enabled is not OMIT:
+            _request["enabled"] = enabled
+        if fields is not OMIT:
+            _request["fields"] = fields
+        if partition_key is not OMIT:
+            _request["partition_key"] = partition_key
         _response = self._client_wrapper.httpx_client.request(
-            "PATCH",
+            "PUT",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/permissions/roles/{jsonable_encoder(id)}"
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/bulk/syncs/{jsonable_encoder(id)}/schemas/{jsonable_encoder(schema_id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
@@ -289,46 +296,74 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RoleResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(BulkSchemaEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncRolesClient:
+class AsyncSchemasClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> RoleListResponseEnvelope:
+    async def list(
+        self,
+        id: str,
+        *,
+        filters: typing.Optional[typing.Dict[str, typing.Optional[str]]] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> ListBulkSchema:
         """
         Parameters:
+            - id: str.
+
+            - filters: typing.Optional[typing.Dict[str, typing.Optional[str]]].
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.permissions.roles.list()
+        await client.bulk_sync.schemas.list(
+            id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/permissions/roles"),
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}/schemas"
+            ),
             params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+                remove_none_from_dict(
+                    {
+                        "filters": jsonable_encoder(filters),
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -337,54 +372,57 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RoleListResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ListBulkSchema, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create(
+    async def patch(
         self,
+        id: str,
         *,
-        name: str,
-        organization_id: typing.Optional[str] = OMIT,
+        schemas: typing.Optional[typing.Sequence[BulkSchema]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> RoleResponseEnvelope:
+    ) -> ListBulkSchema:
         """
         Parameters:
-            - name: str.
+            - id: str.
 
-            - organization_id: typing.Optional[str].
+            - schemas: typing.Optional[typing.Sequence[BulkSchema]].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.permissions.roles.create(
-            name="Custom",
+        await client.bulk_sync.schemas.patch(
+            id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"name": name}
-        if organization_id is not OMIT:
-            _request["organization_id"] = organization_id
+        _request: typing.Dict[str, typing.Any] = {}
+        if schemas is not OMIT:
+            _request["schemas"] = schemas
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/permissions/roles"),
+            "PATCH",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}/schemas"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -401,93 +439,55 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RoleResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ListBulkSchema, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> RoleResponseEnvelope:
+    async def get(
+        self, id: str, schema_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> BulkSchemaEnvelope:
         """
         Parameters:
             - id: str.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.permissions.roles.get(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/permissions/roles/{jsonable_encoder(id)}"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RoleResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def delete(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
-        """
-        Parameters:
-            - id: str.
+            - schema_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.permissions.roles.delete(
+        await client.bulk_sync.schemas.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            schema_id="Contact",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
+            "GET",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/permissions/roles/{jsonable_encoder(id)}"
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/bulk/syncs/{jsonable_encoder(id)}/schemas/{jsonable_encoder(schema_id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -499,59 +499,73 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic.parse_obj_as(BulkSchemaEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update(
         self,
         id: str,
+        schema_id: str,
         *,
-        name: str,
-        organization_id: typing.Optional[str] = OMIT,
+        enabled: typing.Optional[bool] = OMIT,
+        fields: typing.Optional[typing.Sequence[BulkField]] = OMIT,
+        partition_key: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> RoleResponseEnvelope:
+    ) -> BulkSchemaEnvelope:
         """
         Parameters:
             - id: str.
 
-            - name: str.
+            - schema_id: str.
+
+            - enabled: typing.Optional[bool].
 
-            - organization_id: typing.Optional[str].
+            - fields: typing.Optional[typing.Sequence[BulkField]].
+
+            - partition_key: typing.Optional[str].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.permissions.roles.update(
+        await client.bulk_sync.schemas.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            name="Custom",
+            schema_id="contact",
+            enabled=True,
+            partition_key="email",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"name": name}
-        if organization_id is not OMIT:
-            _request["organization_id"] = organization_id
+        _request: typing.Dict[str, typing.Any] = {}
+        if enabled is not OMIT:
+            _request["enabled"] = enabled
+        if fields is not OMIT:
+            _request["fields"] = fields
+        if partition_key is not OMIT:
+            _request["partition_key"] = partition_key
         _response = await self._client_wrapper.httpx_client.request(
-            "PATCH",
+            "PUT",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/permissions/roles/{jsonable_encoder(id)}"
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/bulk/syncs/{jsonable_encoder(id)}/schemas/{jsonable_encoder(schema_id)}",
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
@@ -569,15 +583,21 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RoleResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(BulkSchemaEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `polytomic-0.1.2/src/polytomic/resources/schemas/client.py` & `polytomic-0.2.0/src/polytomic/resources/jobs/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 # This file was auto-generated from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from ...core.api_error import ApiError
+from ...core.api_error import ApiError as core_api_error_ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ...core.request_options import RequestOptions
+from ...errors.bad_request_error import BadRequestError
+from ...errors.internal_server_error import InternalServerError
+from ...errors.not_found_error import NotFoundError
 from ...errors.unauthorized_error import UnauthorizedError
+from ...types.api_error import ApiError as types_api_error_ApiError
+from ...types.job_response_envelope import JobResponseEnvelope
 from ...types.rest_err_response import RestErrResponse
-from ...types.schema_records_response_envelope import SchemaRecordsResponseEnvelope
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class SchemasClient:
+class JobsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def get_records(
-        self, connection_id: str, schema_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> SchemaRecordsResponseEnvelope:
+    def get(
+        self, id: str, type: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> JobResponseEnvelope:
         """
         Parameters:
-            - connection_id: str.
+            - id: str.
 
-            - schema_id: str.
+            - type: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.schemas.get_records(
-            connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            schema_id="contact",
+        client.jobs.get(
+            id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            type="createmodel",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/connections/{jsonable_encoder(connection_id)}/{jsonable_encoder(schema_id)}/records",
+                f"{self._client_wrapper.get_base_url()}/", f"api/jobs/{jsonable_encoder(type)}/{jsonable_encoder(id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -65,55 +67,59 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(SchemaRecordsResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(JobResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncSchemasClient:
+class AsyncJobsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def get_records(
-        self, connection_id: str, schema_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> SchemaRecordsResponseEnvelope:
+    async def get(
+        self, id: str, type: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> JobResponseEnvelope:
         """
         Parameters:
-            - connection_id: str.
+            - id: str.
 
-            - schema_id: str.
+            - type: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.schemas.get_records(
-            connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            schema_id="contact",
+        await client.jobs.get(
+            id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            type="createmodel",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/connections/{jsonable_encoder(connection_id)}/{jsonable_encoder(schema_id)}/records",
+                f"{self._client_wrapper.get_base_url()}/", f"api/jobs/{jsonable_encoder(type)}/{jsonable_encoder(id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -125,15 +131,21 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(SchemaRecordsResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(JobResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `polytomic-0.1.2/src/polytomic/resources/users/client.py` & `polytomic-0.2.0/src/polytomic/resources/permissions/resources/policies/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,57 @@
 # This file was auto-generated from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from ...core.api_error import ApiError
-from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
-from ...core.jsonable_encoder import jsonable_encoder
-from ...core.remove_none_from_dict import remove_none_from_dict
-from ...core.request_options import RequestOptions
-from ...errors.unauthorized_error import UnauthorizedError
-from ...types.api_key_response_envelope import ApiKeyResponseEnvelope
-from ...types.list_users_envelope import ListUsersEnvelope
-from ...types.rest_err_response import RestErrResponse
-from ...types.user_envelope import UserEnvelope
+from .....core.api_error import ApiError as core_api_error_ApiError
+from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.jsonable_encoder import jsonable_encoder
+from .....core.remove_none_from_dict import remove_none_from_dict
+from .....core.request_options import RequestOptions
+from .....errors.bad_request_error import BadRequestError
+from .....errors.forbidden_error import ForbiddenError
+from .....errors.internal_server_error import InternalServerError
+from .....errors.not_found_error import NotFoundError
+from .....errors.unauthorized_error import UnauthorizedError
+from .....types.api_error import ApiError as types_api_error_ApiError
+from .....types.list_policies_response_envelope import ListPoliciesResponseEnvelope
+from .....types.policy_action import PolicyAction
+from .....types.policy_response_envelope import PolicyResponseEnvelope
+from .....types.rest_err_response import RestErrResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class UsersClient:
+class PoliciesClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def list(self, org_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> ListUsersEnvelope:
+    def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> ListPoliciesResponseEnvelope:
         """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
-
         Parameters:
-            - org_id: str.
-
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.users.list(
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
+        client.permissions.policies.list()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{jsonable_encoder(org_id)}/users"
-            ),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/permissions/policies"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -68,65 +62,67 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ListUsersEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ListPoliciesResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
         self,
-        org_id: str,
         *,
-        email: str,
-        role: typing.Optional[str] = OMIT,
+        name: str,
+        organization_id: typing.Optional[str] = OMIT,
+        policy_actions: typing.Optional[typing.Sequence[PolicyAction]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> UserEnvelope:
+    ) -> PolicyResponseEnvelope:
         """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
-
         Parameters:
-            - org_id: str.
+            - name: str.
 
-            - email: str.
+            - organization_id: typing.Optional[str].
 
-            - role: typing.Optional[str].
+            - policy_actions: typing.Optional[typing.Sequence[PolicyAction]].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
+        from polytomic import PolicyAction
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.users.create(
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            email="mail@example.com",
-            role="admin",
+        client.permissions.policies.create(
+            name="Custom",
+            policy_actions=[
+                PolicyAction(
+                    action="read",
+                    role_ids=["248df4b7-aa70-47b8-a036-33ac447e668d"],
+                )
+            ],
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"email": email}
-        if role is not OMIT:
-            _request["role"] = role
+        _request: typing.Dict[str, typing.Any] = {"name": name}
+        if organization_id is not OMIT:
+            _request["organization_id"] = organization_id
+        if policy_actions is not OMIT:
+            _request["policy_actions"] = policy_actions
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{jsonable_encoder(org_id)}/users"
-            ),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/permissions/policies"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -143,52 +139,51 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PolicyResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, id: str, org_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> UserEnvelope:
+    def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> PolicyResponseEnvelope:
         """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
-
         Parameters:
             - id: str.
 
-            - org_id: str.
-
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.users.get(
+        client.permissions.policies.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}",
+                f"{self._client_wrapper.get_base_url()}/", f"api/permissions/policies/{jsonable_encoder(id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -200,126 +195,74 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PolicyResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def remove(self, id: str, org_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> UserEnvelope:
-        """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
-
-        Parameters:
-            - id: str.
-
-            - org_id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.users.remove(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}",
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     def update(
         self,
         id: str,
-        org_id: str,
         *,
-        email: str,
-        role: typing.Optional[str] = OMIT,
+        name: str,
+        organization_id: typing.Optional[str] = OMIT,
+        policy_actions: typing.Optional[typing.Sequence[PolicyAction]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> UserEnvelope:
+    ) -> PolicyResponseEnvelope:
         """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
-
         Parameters:
             - id: str.
 
-            - org_id: str.
+            - name: str.
 
-            - email: str.
+            - organization_id: typing.Optional[str].
 
-            - role: typing.Optional[str].
+            - policy_actions: typing.Optional[typing.Sequence[PolicyAction]].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
+        from polytomic import PolicyAction
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.users.update(
+        client.permissions.policies.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            email="mail@example.com",
-            role="admin",
+            name="Custom",
+            policy_actions=[
+                PolicyAction(
+                    action="read",
+                    role_ids=["248df4b7-aa70-47b8-a036-33ac447e668d"],
+                )
+            ],
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"email": email}
-        if role is not OMIT:
-            _request["role"] = role
+        _request: typing.Dict[str, typing.Any] = {"name": name}
+        if organization_id is not OMIT:
+            _request["organization_id"] = organization_id
+        if policy_actions is not OMIT:
+            _request["policy_actions"] = policy_actions
         _response = self._client_wrapper.httpx_client.request(
-            "PATCH",
+            "PUT",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}",
+                f"{self._client_wrapper.get_base_url()}/", f"api/permissions/policies/{jsonable_encoder(id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
@@ -337,78 +280,55 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PolicyResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create_api_key(
-        self,
-        org_id: str,
-        id: str,
-        *,
-        force: typing.Optional[bool] = None,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> ApiKeyResponseEnvelope:
+    def remove(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
-
         Parameters:
-            - org_id: str.
-
             - id: str.
 
-            - force: typing.Optional[bool].
-
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.users.create_api_key(
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        client.permissions.policies.remove(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            force=True,
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
+            "DELETE",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}/keys",
+                f"{self._client_wrapper.get_base_url()}/", f"api/permissions/policies/{jsonable_encoder(id)}"
             ),
             params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "force": force,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
-                )
+                request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
-            if request_options is not None
-            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -416,54 +336,49 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ApiKeyResponseEnvelope, _response.json())  # type: ignore
+            return
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncUsersClient:
+class AsyncPoliciesClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def list(self, org_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> ListUsersEnvelope:
+    async def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> ListPoliciesResponseEnvelope:
         """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
-
         Parameters:
-            - org_id: str.
-
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.users.list(
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
+        await client.permissions.policies.list()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{jsonable_encoder(org_id)}/users"
-            ),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/permissions/policies"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -474,65 +389,67 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ListUsersEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ListPoliciesResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
         self,
-        org_id: str,
         *,
-        email: str,
-        role: typing.Optional[str] = OMIT,
+        name: str,
+        organization_id: typing.Optional[str] = OMIT,
+        policy_actions: typing.Optional[typing.Sequence[PolicyAction]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> UserEnvelope:
+    ) -> PolicyResponseEnvelope:
         """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
-
         Parameters:
-            - org_id: str.
+            - name: str.
 
-            - email: str.
+            - organization_id: typing.Optional[str].
 
-            - role: typing.Optional[str].
+            - policy_actions: typing.Optional[typing.Sequence[PolicyAction]].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
+        from polytomic import PolicyAction
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.users.create(
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            email="mail@example.com",
-            role="admin",
+        await client.permissions.policies.create(
+            name="Custom",
+            policy_actions=[
+                PolicyAction(
+                    action="read",
+                    role_ids=["248df4b7-aa70-47b8-a036-33ac447e668d"],
+                )
+            ],
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"email": email}
-        if role is not OMIT:
-            _request["role"] = role
+        _request: typing.Dict[str, typing.Any] = {"name": name}
+        if organization_id is not OMIT:
+            _request["organization_id"] = organization_id
+        if policy_actions is not OMIT:
+            _request["policy_actions"] = policy_actions
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{jsonable_encoder(org_id)}/users"
-            ),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/permissions/policies"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -549,113 +466,51 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PolicyResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get(
-        self, id: str, org_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> UserEnvelope:
-        """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-        Parameters:
-            - id: str.
-
-            - org_id: str.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.users.get(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
+    async def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> PolicyResponseEnvelope:
         """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}",
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def remove(
-        self, id: str, org_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> UserEnvelope:
-        """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
-
         Parameters:
             - id: str.
 
-            - org_id: str.
-
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.users.remove(
+        await client.permissions.policies.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
+            "GET",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}",
+                f"{self._client_wrapper.get_base_url()}/", f"api/permissions/policies/{jsonable_encoder(id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -667,69 +522,74 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PolicyResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update(
         self,
         id: str,
-        org_id: str,
         *,
-        email: str,
-        role: typing.Optional[str] = OMIT,
+        name: str,
+        organization_id: typing.Optional[str] = OMIT,
+        policy_actions: typing.Optional[typing.Sequence[PolicyAction]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> UserEnvelope:
+    ) -> PolicyResponseEnvelope:
         """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
-
         Parameters:
             - id: str.
 
-            - org_id: str.
+            - name: str.
 
-            - email: str.
+            - organization_id: typing.Optional[str].
 
-            - role: typing.Optional[str].
+            - policy_actions: typing.Optional[typing.Sequence[PolicyAction]].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
+        from polytomic import PolicyAction
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.users.update(
+        await client.permissions.policies.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            email="mail@example.com",
-            role="admin",
+            name="Custom",
+            policy_actions=[
+                PolicyAction(
+                    action="read",
+                    role_ids=["248df4b7-aa70-47b8-a036-33ac447e668d"],
+                )
+            ],
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"email": email}
-        if role is not OMIT:
-            _request["role"] = role
+        _request: typing.Dict[str, typing.Any] = {"name": name}
+        if organization_id is not OMIT:
+            _request["organization_id"] = organization_id
+        if policy_actions is not OMIT:
+            _request["policy_actions"] = policy_actions
         _response = await self._client_wrapper.httpx_client.request(
-            "PATCH",
+            "PUT",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}",
+                f"{self._client_wrapper.get_base_url()}/", f"api/permissions/policies/{jsonable_encoder(id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
@@ -747,78 +607,55 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PolicyResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create_api_key(
-        self,
-        org_id: str,
-        id: str,
-        *,
-        force: typing.Optional[bool] = None,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> ApiKeyResponseEnvelope:
+    async def remove(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
-
         Parameters:
-            - org_id: str.
-
             - id: str.
 
-            - force: typing.Optional[bool].
-
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.users.create_api_key(
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        await client.permissions.policies.remove(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            force=True,
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
+            "DELETE",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}/keys",
+                f"{self._client_wrapper.get_base_url()}/", f"api/permissions/policies/{jsonable_encoder(id)}"
             ),
             params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "force": force,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
-                )
+                request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
-            if request_options is not None
-            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -826,15 +663,21 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ApiKeyResponseEnvelope, _response.json())  # type: ignore
+            return
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `polytomic-0.1.2/src/polytomic/resources/webhooks/client.py` & `polytomic-0.2.0/src/polytomic/resources/schemas/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,135 +1,66 @@
 # This file was auto-generated from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from ...core.api_error import ApiError
+from ...core.api_error import ApiError as core_api_error_ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ...core.request_options import RequestOptions
+from ...errors.bad_request_error import BadRequestError
+from ...errors.forbidden_error import ForbiddenError
+from ...errors.internal_server_error import InternalServerError
+from ...errors.not_found_error import NotFoundError
 from ...errors.unauthorized_error import UnauthorizedError
+from ...types.api_error import ApiError as types_api_error_ApiError
+from ...types.bulk_sync_source_schema_envelope import BulkSyncSourceSchemaEnvelope
+from ...types.bulk_sync_source_status_envelope import BulkSyncSourceStatusEnvelope
 from ...types.rest_err_response import RestErrResponse
-from ...types.webhook_envelope import WebhookEnvelope
-from ...types.webhook_list_envelope import WebhookListEnvelope
+from ...types.schema_records_response_envelope import SchemaRecordsResponseEnvelope
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
-# this is used as the default value for optional parameters
-OMIT = typing.cast(typing.Any, ...)
 
-
-class WebhooksClient:
+class SchemasClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> WebhookListEnvelope:
+    def refresh(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
-        Webooks can be set up using the webhook API endpoints. Currently, only one
-        webhook may be created per organization. The webhook will be called for events
-        in that organization.
-
-        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
-
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.webhooks.list()
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/webhooks"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(WebhookListEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def create(
-        self,
-        *,
-        endpoint: str,
-        organization_id: typing.Optional[str] = OMIT,
-        secret: str,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> WebhookEnvelope:
-        """
-        Webooks can be set up using the webhook API endpoints. Currently, only one
-        webhook may be created per organization. The webhook will be called for events
-        in that organization.
-
-        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
-
         Parameters:
-            - endpoint: str.
-
-            - organization_id: typing.Optional[str].
-
-            - secret: str.
+            - id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.webhooks.create(
-            endpoint="https://example.com/webhook",
-            secret="secret",
+        client.schemas.refresh(
+            id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"endpoint": endpoint, "secret": secret}
-        if organization_id is not OMIT:
-            _request["organization_id"] = organization_id
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/webhooks"),
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}/schemas/refresh"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -137,49 +68,52 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(WebhookEnvelope, _response.json())  # type: ignore
+            return
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> WebhookEnvelope:
+    def get_status(
+        self, id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> BulkSyncSourceStatusEnvelope:
         """
-        Webooks can be set up using the webhook API endpoints. Currently, only one
-        webhook may be created per organization. The webhook will be called for events
-        in that organization.
-
-        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
-
         Parameters:
             - id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.webhooks.get(
+        client.schemas.get_status(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/webhooks/{jsonable_encoder(id)}"),
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}/schemas/status"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -190,43 +124,56 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(WebhookEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(BulkSyncSourceStatusEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    def delete(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
+    def get(
+        self, id: str, schema_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> BulkSyncSourceSchemaEnvelope:
         """
         Parameters:
             - id: str.
 
+            - schema_id: str.
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.webhooks.delete(
+        client.schemas.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            schema_id="public.users",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/webhooks/{jsonable_encoder(id)}"),
+            "GET",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/connections/{jsonable_encoder(id)}/schemas/{jsonable_encoder(schema_id)}",
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -237,77 +184,59 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic.parse_obj_as(BulkSyncSourceSchemaEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def update(
-        self,
-        id: str,
-        *,
-        endpoint: str,
-        organization_id: typing.Optional[str] = OMIT,
-        secret: str,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> WebhookEnvelope:
-        """
-        Webooks can be set up using the webhook API endpoints. Currently, only one
-        webhook may be created per organization. The webhook will be called for events
-        in that organization.
-
-        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
+    def get_records(
+        self, id: str, schema_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> SchemaRecordsResponseEnvelope:
+        """
         Parameters:
             - id: str.
 
-            - endpoint: str.
-
-            - organization_id: typing.Optional[str].
-
-            - secret: str.
+            - schema_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.webhooks.update(
+        client.schemas.get_records(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            endpoint="https://example.com/webhook",
-            secret="secret",
+            schema_id="public.users",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"endpoint": endpoint, "secret": secret}
-        if organization_id is not OMIT:
-            _request["organization_id"] = organization_id
         _response = self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/webhooks/{jsonable_encoder(id)}"),
+            "GET",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/connections/{jsonable_encoder(id)}/schemas/{jsonable_encoder(schema_id)}/records",
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -315,127 +244,63 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(WebhookEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(SchemaRecordsResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncWebhooksClient:
+class AsyncSchemasClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> WebhookListEnvelope:
+    async def refresh(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
-        Webooks can be set up using the webhook API endpoints. Currently, only one
-        webhook may be created per organization. The webhook will be called for events
-        in that organization.
-
-        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
-
         Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.webhooks.list()
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/webhooks"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(WebhookListEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def create(
-        self,
-        *,
-        endpoint: str,
-        organization_id: typing.Optional[str] = OMIT,
-        secret: str,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> WebhookEnvelope:
-        """
-        Webooks can be set up using the webhook API endpoints. Currently, only one
-        webhook may be created per organization. The webhook will be called for events
-        in that organization.
-
-        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
-
-        Parameters:
-            - endpoint: str.
-
-            - organization_id: typing.Optional[str].
-
-            - secret: str.
+            - id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.webhooks.create(
-            endpoint="https://example.com/webhook",
-            secret="secret",
+        await client.schemas.refresh(
+            id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"endpoint": endpoint, "secret": secret}
-        if organization_id is not OMIT:
-            _request["organization_id"] = organization_id
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/webhooks"),
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}/schemas/refresh"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -443,49 +308,52 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(WebhookEnvelope, _response.json())  # type: ignore
+            return
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> WebhookEnvelope:
+    async def get_status(
+        self, id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> BulkSyncSourceStatusEnvelope:
         """
-        Webooks can be set up using the webhook API endpoints. Currently, only one
-        webhook may be created per organization. The webhook will be called for events
-        in that organization.
-
-        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
-
         Parameters:
             - id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.webhooks.get(
+        await client.schemas.get_status(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/webhooks/{jsonable_encoder(id)}"),
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/connections/{jsonable_encoder(id)}/schemas/status"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -496,43 +364,56 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(WebhookEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(BulkSyncSourceStatusEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def delete(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
+    async def get(
+        self, id: str, schema_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> BulkSyncSourceSchemaEnvelope:
         """
         Parameters:
             - id: str.
 
+            - schema_id: str.
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.webhooks.delete(
+        await client.schemas.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            schema_id="public.users",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/webhooks/{jsonable_encoder(id)}"),
+            "GET",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/connections/{jsonable_encoder(id)}/schemas/{jsonable_encoder(schema_id)}",
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -543,77 +424,59 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic.parse_obj_as(BulkSyncSourceSchemaEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def update(
-        self,
-        id: str,
-        *,
-        endpoint: str,
-        organization_id: typing.Optional[str] = OMIT,
-        secret: str,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> WebhookEnvelope:
-        """
-        Webooks can be set up using the webhook API endpoints. Currently, only one
-        webhook may be created per organization. The webhook will be called for events
-        in that organization.
-
-        Consult the [Events documentation](https://docs.polytomic.com/reference/events) for more information.
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
+    async def get_records(
+        self, id: str, schema_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> SchemaRecordsResponseEnvelope:
+        """
         Parameters:
             - id: str.
 
-            - endpoint: str.
-
-            - organization_id: typing.Optional[str].
-
-            - secret: str.
+            - schema_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.webhooks.update(
+        await client.schemas.get_records(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            endpoint="https://example.com/webhook",
-            secret="secret",
+            schema_id="public.users",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"endpoint": endpoint, "secret": secret}
-        if organization_id is not OMIT:
-            _request["organization_id"] = organization_id
         _response = await self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/webhooks/{jsonable_encoder(id)}"),
+            "GET",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/connections/{jsonable_encoder(id)}/schemas/{jsonable_encoder(schema_id)}/records",
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -621,15 +484,23 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(WebhookEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(SchemaRecordsResponseEnvelope, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `polytomic-0.1.2/src/polytomic/types/__init__.py` & `polytomic-0.2.0/src/polytomic/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .activate_sync_envelope import ActivateSyncEnvelope
 from .activate_sync_input import ActivateSyncInput
 from .activate_sync_output import ActivateSyncOutput
+from .api_error import ApiError
 from .api_key_response import ApiKeyResponse
 from .api_key_response_envelope import ApiKeyResponseEnvelope
 from .bulk_discover import BulkDiscover
 from .bulk_execution_status import BulkExecutionStatus
 from .bulk_field import BulkField
 from .bulk_itemized_schedule import BulkItemizedSchedule
 from .bulk_multi_schedule_configuration import BulkMultiScheduleConfiguration
@@ -55,14 +56,15 @@
 from .execution_status import ExecutionStatus
 from .filter import Filter
 from .get_connection_meta_envelope import GetConnectionMetaEnvelope
 from .get_execution_response_envelope import GetExecutionResponseEnvelope
 from .get_execution_response_schema import GetExecutionResponseSchema
 from .get_identity_response_envelope import GetIdentityResponseEnvelope
 from .get_identity_response_schema import GetIdentityResponseSchema
+from .get_model_sync_source_meta_envelope import GetModelSyncSourceMetaEnvelope
 from .identity import Identity
 from .identity_function import IdentityFunction
 from .job_response import JobResponse
 from .job_response_envelope import JobResponseEnvelope
 from .jsonschema_form import JsonschemaForm
 from .label_label import LabelLabel
 from .list_bulk_schema import ListBulkSchema
@@ -79,14 +81,15 @@
 from .model_relation import ModelRelation
 from .model_relation_to import ModelRelationTo
 from .model_response import ModelResponse
 from .model_response_envelope import ModelResponseEnvelope
 from .model_sync_field import ModelSyncField
 from .model_sync_response import ModelSyncResponse
 from .model_sync_response_envelope import ModelSyncResponseEnvelope
+from .model_sync_source_meta_response import ModelSyncSourceMetaResponse
 from .organization import Organization
 from .organization_envelope import OrganizationEnvelope
 from .organizations_envelope import OrganizationsEnvelope
 from .override import Override
 from .pick_value import PickValue
 from .policy_action import PolicyAction
 from .policy_response import PolicyResponse
@@ -104,14 +107,15 @@
 from .schedule_option_response_envelope import ScheduleOptionResponseEnvelope
 from .schedule_schedule_option import ScheduleScheduleOption
 from .schema import Schema
 from .schema_association import SchemaAssociation
 from .schema_field import SchemaField
 from .schema_records_response_envelope import SchemaRecordsResponseEnvelope
 from .source import Source
+from .source_meta import SourceMeta
 from .start_model_sync_response_envelope import StartModelSyncResponseEnvelope
 from .start_model_sync_response_schema import StartModelSyncResponseSchema
 from .supported_mode import SupportedMode
 from .sync_destination_properties import SyncDestinationProperties
 from .sync_status_envelope import SyncStatusEnvelope
 from .sync_status_response import SyncStatusResponse
 from .target import Target
@@ -125,14 +129,15 @@
 from .webhook_list_envelope import WebhookListEnvelope
 from .work_task_status import WorkTaskStatus
 
 __all__ = [
     "ActivateSyncEnvelope",
     "ActivateSyncInput",
     "ActivateSyncOutput",
+    "ApiError",
     "ApiKeyResponse",
     "ApiKeyResponseEnvelope",
     "BulkDiscover",
     "BulkExecutionStatus",
     "BulkField",
     "BulkItemizedSchedule",
     "BulkMultiScheduleConfiguration",
@@ -181,14 +186,15 @@
     "ExecutionStatus",
     "Filter",
     "GetConnectionMetaEnvelope",
     "GetExecutionResponseEnvelope",
     "GetExecutionResponseSchema",
     "GetIdentityResponseEnvelope",
     "GetIdentityResponseSchema",
+    "GetModelSyncSourceMetaEnvelope",
     "Identity",
     "IdentityFunction",
     "JobResponse",
     "JobResponseEnvelope",
     "JsonschemaForm",
     "LabelLabel",
     "ListBulkSchema",
@@ -205,14 +211,15 @@
     "ModelRelation",
     "ModelRelationTo",
     "ModelResponse",
     "ModelResponseEnvelope",
     "ModelSyncField",
     "ModelSyncResponse",
     "ModelSyncResponseEnvelope",
+    "ModelSyncSourceMetaResponse",
     "Organization",
     "OrganizationEnvelope",
     "OrganizationsEnvelope",
     "Override",
     "PickValue",
     "PolicyAction",
     "PolicyResponse",
@@ -230,14 +237,15 @@
     "ScheduleOptionResponseEnvelope",
     "ScheduleScheduleOption",
     "Schema",
     "SchemaAssociation",
     "SchemaField",
     "SchemaRecordsResponseEnvelope",
     "Source",
+    "SourceMeta",
     "StartModelSyncResponseEnvelope",
     "StartModelSyncResponseSchema",
     "SupportedMode",
     "SyncDestinationProperties",
     "SyncStatusEnvelope",
     "SyncStatusResponse",
     "Target",
```

### Comparing `polytomic-0.1.2/src/polytomic/types/activate_sync_envelope.py` & `polytomic-0.2.0/src/polytomic/types/activate_sync_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/activate_sync_input.py` & `polytomic-0.2.0/src/polytomic/types/activate_sync_input.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/activate_sync_output.py` & `polytomic-0.2.0/src/polytomic/types/activate_sync_output.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/api_key_response.py` & `polytomic-0.2.0/src/polytomic/types/api_key_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/api_key_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/api_key_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_discover.py` & `polytomic-0.2.0/src/polytomic/types/bulk_discover.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_execution_status.py` & `polytomic-0.2.0/src/polytomic/types/bulk_execution_status.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_field.py` & `polytomic-0.2.0/src/polytomic/types/bulk_field.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_itemized_schedule.py` & `polytomic-0.2.0/src/polytomic/types/bulk_itemized_schedule.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_multi_schedule_configuration.py` & `polytomic-0.2.0/src/polytomic/types/bulk_multi_schedule_configuration.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_schedule.py` & `polytomic-0.2.0/src/polytomic/types/bulk_schedule.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_schema.py` & `polytomic-0.2.0/src/polytomic/types/bulk_schema.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_schema_envelope.py` & `polytomic-0.2.0/src/polytomic/types/bulk_schema_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_schema_execution_status.py` & `polytomic-0.2.0/src/polytomic/types/bulk_schema_execution_status.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_selective_mode.py` & `polytomic-0.2.0/src/polytomic/types/bulk_selective_mode.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_sync_dest.py` & `polytomic-0.2.0/src/polytomic/types/bulk_sync_dest.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_sync_dest_envelope.py` & `polytomic-0.2.0/src/polytomic/types/bulk_sync_dest_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_sync_execution.py` & `polytomic-0.2.0/src/polytomic/types/bulk_sync_execution.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_sync_execution_envelope.py` & `polytomic-0.2.0/src/polytomic/types/bulk_sync_execution_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_sync_list_envelope.py` & `polytomic-0.2.0/src/polytomic/types/bulk_sync_list_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_sync_response.py` & `polytomic-0.2.0/src/polytomic/types/bulk_sync_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_sync_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/bulk_sync_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_sync_schema_execution.py` & `polytomic-0.2.0/src/polytomic/types/bulk_sync_schema_execution.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_sync_source.py` & `polytomic-0.2.0/src/polytomic/types/bulk_sync_source.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_sync_source_envelope.py` & `polytomic-0.2.0/src/polytomic/types/bulk_sync_source_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_sync_source_schema_envelope.py` & `polytomic-0.2.0/src/polytomic/types/bulk_sync_source_schema_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_sync_source_status.py` & `polytomic-0.2.0/src/polytomic/types/bulk_sync_source_status.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_sync_source_status_envelope.py` & `polytomic-0.2.0/src/polytomic/types/bulk_sync_source_status_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_sync_status_envelope.py` & `polytomic-0.2.0/src/polytomic/types/bulk_sync_status_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/bulk_sync_status_response.py` & `polytomic-0.2.0/src/polytomic/types/bulk_sync_status_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/configuration_value.py` & `polytomic-0.2.0/src/polytomic/types/configuration_value.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/connect_card_response.py` & `polytomic-0.2.0/src/polytomic/types/connect_card_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/connect_card_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/connect_card_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/connection_list_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/connection_list_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/connection_meta.py` & `polytomic-0.2.0/src/polytomic/types/connection_meta.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/connection_meta_response.py` & `polytomic-0.2.0/src/polytomic/types/connection_meta_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/connection_parameter_value.py` & `polytomic-0.2.0/src/polytomic/types/connection_parameter_value.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/connection_parameter_values_resp.py` & `polytomic-0.2.0/src/polytomic/types/connection_parameter_values_resp.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/connection_parameter_values_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/connection_parameter_values_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/connection_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/connection_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/connection_response_schema.py` & `polytomic-0.2.0/src/polytomic/types/connection_response_schema.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/connection_type.py` & `polytomic-0.2.0/src/polytomic/types/connection_type.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/connection_type_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/connection_type_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/connection_type_schema.py` & `polytomic-0.2.0/src/polytomic/types/connection_type_schema.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/create_connection_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/create_connection_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/create_connection_response_schema.py` & `polytomic-0.2.0/src/polytomic/types/create_connection_response_schema.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/event.py` & `polytomic-0.2.0/src/polytomic/types/event.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/event_types_envelope.py` & `polytomic-0.2.0/src/polytomic/types/event_types_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/events_envelope.py` & `polytomic-0.2.0/src/polytomic/types/events_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/execution_counts.py` & `polytomic-0.2.0/src/polytomic/types/execution_counts.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/execution_log_response.py` & `polytomic-0.2.0/src/polytomic/types/execution_log_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/execution_logs_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/execution_logs_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/execution_status.py` & `polytomic-0.2.0/src/polytomic/types/execution_status.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/filter.py` & `polytomic-0.2.0/src/polytomic/types/filter.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/get_connection_meta_envelope.py` & `polytomic-0.2.0/src/polytomic/types/get_connection_meta_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/get_execution_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/get_execution_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/get_execution_response_schema.py` & `polytomic-0.2.0/src/polytomic/types/get_execution_response_schema.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/get_identity_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/get_identity_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/get_identity_response_schema.py` & `polytomic-0.2.0/src/polytomic/types/get_identity_response_schema.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/identity.py` & `polytomic-0.2.0/src/polytomic/types/identity.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/identity_function.py` & `polytomic-0.2.0/src/polytomic/types/identity_function.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/job_response.py` & `polytomic-0.2.0/src/polytomic/types/job_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/job_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/job_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/list_bulk_schema.py` & `polytomic-0.2.0/src/polytomic/types/list_bulk_schema.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/list_bulk_sync_executions_envelope.py` & `polytomic-0.2.0/src/polytomic/types/list_bulk_sync_executions_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/list_execution_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/list_execution_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/list_model_sync_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/list_model_sync_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/list_policies_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/list_policies_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/list_users_envelope.py` & `polytomic-0.2.0/src/polytomic/types/list_users_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/mode.py` & `polytomic-0.2.0/src/polytomic/types/mode.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/model_field.py` & `polytomic-0.2.0/src/polytomic/types/model_field.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/model_field_response.py` & `polytomic-0.2.0/src/polytomic/types/model_field_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/model_list_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/model_list_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/model_model_field_request.py` & `polytomic-0.2.0/src/polytomic/types/model_model_field_request.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/model_relation.py` & `polytomic-0.2.0/src/polytomic/types/model_relation.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/model_relation_to.py` & `polytomic-0.2.0/src/polytomic/types/model_relation_to.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/model_response.py` & `polytomic-0.2.0/src/polytomic/types/model_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/model_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/model_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/model_sync_field.py` & `polytomic-0.2.0/src/polytomic/types/model_sync_field.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/model_sync_response.py` & `polytomic-0.2.0/src/polytomic/types/model_sync_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/model_sync_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/model_sync_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/organization.py` & `polytomic-0.2.0/src/polytomic/types/organization.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/organization_envelope.py` & `polytomic-0.2.0/src/polytomic/types/organization_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/organizations_envelope.py` & `polytomic-0.2.0/src/polytomic/types/organizations_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/override.py` & `polytomic-0.2.0/src/polytomic/types/override.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/pick_value.py` & `polytomic-0.2.0/src/polytomic/types/pick_value.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/policy_action.py` & `polytomic-0.2.0/src/polytomic/types/policy_action.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/policy_response.py` & `polytomic-0.2.0/src/polytomic/types/policy_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/policy_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/policy_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/relation.py` & `polytomic-0.2.0/src/polytomic/types/relation.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/relation_to.py` & `polytomic-0.2.0/src/polytomic/types/relation_to.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/rest_err_response.py` & `polytomic-0.2.0/src/polytomic/types/rest_err_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/role_list_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/role_list_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/role_response.py` & `polytomic-0.2.0/src/polytomic/types/role_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/role_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/role_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/run_after.py` & `polytomic-0.2.0/src/polytomic/types/run_after.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/schedule.py` & `polytomic-0.2.0/src/polytomic/types/schedule.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/schedule_frequency.py` & `polytomic-0.2.0/src/polytomic/types/schedule_frequency.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/schedule_option_response.py` & `polytomic-0.2.0/src/polytomic/types/schedule_option_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/schedule_option_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/schedule_option_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/schedule_schedule_option.py` & `polytomic-0.2.0/src/polytomic/types/schedule_schedule_option.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/schema.py` & `polytomic-0.2.0/src/polytomic/types/schema.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/schema_association.py` & `polytomic-0.2.0/src/polytomic/types/schema_association.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/schema_field.py` & `polytomic-0.2.0/src/polytomic/types/schema_field.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/schema_records_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/schema_records_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/source.py` & `polytomic-0.2.0/src/polytomic/types/source.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/start_model_sync_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/start_model_sync_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/start_model_sync_response_schema.py` & `polytomic-0.2.0/src/polytomic/types/start_model_sync_response_schema.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/supported_mode.py` & `polytomic-0.2.0/src/polytomic/types/supported_mode.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/sync_destination_properties.py` & `polytomic-0.2.0/src/polytomic/types/sync_destination_properties.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/sync_status_envelope.py` & `polytomic-0.2.0/src/polytomic/types/sync_status_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/sync_status_response.py` & `polytomic-0.2.0/src/polytomic/types/sync_status_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/target.py` & `polytomic-0.2.0/src/polytomic/types/target.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/target_field.py` & `polytomic-0.2.0/src/polytomic/types/target_field.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/target_response.py` & `polytomic-0.2.0/src/polytomic/types/target_response.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/target_response_envelope.py` & `polytomic-0.2.0/src/polytomic/types/target_response_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/user.py` & `polytomic-0.2.0/src/polytomic/types/user.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/user_envelope.py` & `polytomic-0.2.0/src/polytomic/types/user_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/webhook.py` & `polytomic-0.2.0/src/polytomic/types/webhook.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/webhook_envelope.py` & `polytomic-0.2.0/src/polytomic/types/webhook_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/webhook_list_envelope.py` & `polytomic-0.2.0/src/polytomic/types/webhook_list_envelope.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/src/polytomic/types/work_task_status.py` & `polytomic-0.2.0/src/polytomic/types/work_task_status.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.2/PKG-INFO` & `polytomic-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polytomic
-Version: 0.1.2
+Version: 0.2.0
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -32,28 +32,26 @@
 <!-- Begin Usage, generated by Fern  -->
 # Usage
 
 ```python
 from polytomic.client import Polytomic
 
 client = Polytomic(
-    x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
     token="YOUR_TOKEN",
 )
 ```
 <!-- End Usage  -->
 
 <!-- Begin Async Usage, generated by Fern  -->
 # Async Client
 
 ```python
 from polytomic.client import AsyncPolytomic
 
 client = AsyncPolytomic(
-    x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
     token="YOUR_TOKEN",
 )
 ```
 <!-- End Async Usage  -->
 
 <!-- Begin Status, generated by Fern  -->
 # Beta Status
```

