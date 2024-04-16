# Comparing `tmp/fixpoint_sdk-0.6.0.tar.gz` & `tmp/fixpoint_sdk-0.8.0rc0.tar.gz`

## Comparing `fixpoint_sdk-0.6.0.tar` & `fixpoint_sdk-0.8.0rc0.tar`

### file list

```diff
@@ -1,179 +1,52 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/.editorconfig
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/.lintstagedrc.json
--rw-r--r--   0        0        0    21691 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/.pylintrc
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/mypy.ini
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/pytest.ini
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/requirements.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/test-requirements.txt
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/.github/workflows/pypi-release-prod.yml
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/.github/workflows/pypi-release-test.yml
--rwxr-xr-x   0        0        0      646 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/bin/pip-freeze
--rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/bin/pip-install
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/examples/__init__.py
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/examples/main.py
--rw-r--r--   0        0        0     4673 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/examples/router.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/examples/streaming.py
--rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/githooks/pre-commit
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/__init__.py
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/client.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/compat.py
--rw-r--r--   0        0        0    12109 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/completions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/lib/__init__.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/lib/debugging.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/lib/env.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/lib/exc.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/lib/iterwrapper.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/lib/logging.py
--rw-r--r--   0        0        0     7348 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/lib/requests.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/exceptions.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/.gitignore
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/.gitlab-ci.yml
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/.openapi-generator-ignore
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/.travis.yml
--rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/README.md
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/git_push.sh
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/pyproject.toml
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/requirements.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/setup.cfg
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/setup.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/test-requirements.txt
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/tox.ini
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/.github/workflows/python.yml
--rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/.openapi-generator/FILES
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/.openapi-generator/VERSION
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/AppLogLevelType.md
--rw-r--r--   0        0        0    44192 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyApi.md
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyCreateOpenAIChatInputLogRequest.md
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyCreateOpenAIChatOutputLogRequest.md
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyPostDatasetLogsRequest.md
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyUpdateSpendingTotalsRequest.md
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/OpenAIChatOutputLogChoice.md
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/OpenAIChatOutputLogUsage.md
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/ProtobufAny.md
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/ProtobufNullValue.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/RpcStatus.md
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ApiSecret.md
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ApiSecretProvider.md
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1AppLog.md
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1AttributeFilters.md
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateApiSecretRequest.md
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateAppLogsRequest.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateAppLogsResponse.md
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateDatasetRequest.md
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateDatasetResponse.md
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLikesRequest.md
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLikesResponse.md
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLogAttributeRequest.md
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLogAttributeResponse.md
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateRoutingConfigRequest.md
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1Dataset.md
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1DatasetFilters.md
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1DeleteLogAttributeResponse.md
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1FallbackStrategy.md
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1Like.md
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1LikeFilter.md
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1LikeIngest.md
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ListApiSecretsResponse.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ListAppLogsResponse.md
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ListDatasetsResponse.md
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ListLikesResponse.md
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ListLogAttributesResponse.md
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ListOpenAIChatLogsResponse.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ListRoutingConfigsResponse.md
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1LogAttribute.md
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1Message.md
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1Mode.md
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1Model.md
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatInputLog.md
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatLog.md
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatLogsFilters.md
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatOutputLog.md
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1OriginType.md
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1PostDatasetLogsResponse.md
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1RelativeDateTimeFilters.md
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ResetInterval.md
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1RoutingConfig.md
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1SpendCap.md
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1TerminalState.md
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1ThumbsReaction.md
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/docs/V1UsageTotals.md
--rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/__init__.py
--rw-r--r--   0        0        0    25750 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/api_client.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/api_response.py
--rw-r--r--   0        0        0    14511 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/configuration.py
--rw-r--r--   0        0        0     6009 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/py.typed
--rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/rest.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/api/__init__.py
--rw-r--r--   0        0        0   198013 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/api/llm_proxy_api.py
--rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/__init__.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/app_log_level_type.py
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_create_open_ai_chat_input_log_request.py
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_create_open_ai_chat_output_log_request.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_post_dataset_logs_request.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_update_spending_totals_request.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/open_ai_chat_output_log_choice.py
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/open_ai_chat_output_log_usage.py
--rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/protobuf_any.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/protobuf_null_value.py
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/rpc_status.py
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_api_secret.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_api_secret_provider.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_app_log.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_attribute_filters.py
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_api_secret_request.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_app_logs_request.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_app_logs_response.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_dataset_request.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_dataset_response.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_likes_request.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_likes_response.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_log_attribute_request.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_log_attribute_response.py
--rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_routing_config_request.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_dataset.py
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_dataset_filters.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_delete_log_attribute_response.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_fallback_strategy.py
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_like.py
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_like_filter.py
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_like_ingest.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_api_secrets_response.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_app_logs_response.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_datasets_response.py
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_likes_response.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_log_attributes_response.py
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_open_ai_chat_logs_response.py
--rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_routing_configs_response.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_log_attribute.py
--rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_message.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_mode.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_model.py
--rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_input_log.py
--rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_log.py
--rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_logs_filters.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_output_log.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_origin_type.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_post_dataset_logs_response.py
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_relative_date_time_filters.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_reset_interval.py
--rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_routing_config.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_spend_cap.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_terminal_state.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_thumbs_reaction.py
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_usage_totals.py
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/src/fixpoint_sdk/types/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0    15061 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/tests/mock_completions.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/tests/test_completions.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/tests/test_types.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/tests/lib/test_iterwrapper.py
--rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/tests/lib/test_requests.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/.gitignore
--rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/LICENSE
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/README.md
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 fixpoint_sdk-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/.editorconfig
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/.lintstagedrc.json
+-rw-r--r--   0        0        0    21726 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/.pylintrc
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/mypy.ini
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/pytest.ini
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/requirements.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/test-requirements.txt
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/.github/workflows/pypi-release-prod.yml
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/.github/workflows/pypi-release-test.yml
+-rwxr-xr-x   0        0        0      646 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/bin/pip-freeze
+-rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/bin/pip-install
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/examples/__init__.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/examples/direct_logging.py
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/examples/function_calling.py
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/examples/main.py
+-rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/examples/router.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/examples/streaming.py
+-rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/githooks/pre-commit
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/__init__.py
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/_logging_api.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/_mock_completions.py
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/client.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/compat.py
+-rw-r--r--   0        0        0    12815 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/completions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/__init__.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/_mock_requests.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/debugging.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/env.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/exc.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/iterwrapper.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/logging.py
+-rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/requests.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/openapi/__init__.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/openapi/exceptions.py
+-rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/types/__init__.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/types/_utils.py
+-rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/types/openai.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/tests/__init__.py
+-rw-r--r--   0        0        0    15061 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/tests/mock_completions.py
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/tests/test_client.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/tests/test_completions.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/tests/test_types.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/tests/lib/test_iterwrapper.py
+-rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/tests/lib/test_requests.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/tests/types/test_openai.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/.gitignore
+-rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/LICENSE
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/README.md
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.0rc0/PKG-INFO
```

### Comparing `fixpoint_sdk-0.6.0/.pylintrc` & `fixpoint_sdk-0.8.0rc0/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -431,14 +431,15 @@
         too-few-public-methods,
         use-symbolic-message-instead,
         use-implicit-booleaness-not-comparison-to-string,
         use-implicit-booleaness-not-comparison-to-zero,
         similarities,
         too-many-arguments,
         too-many-instance-attributes,
+        too-many-return-statements
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
```

### Comparing `fixpoint_sdk-0.6.0/mypy.ini` & `fixpoint_sdk-0.8.0rc0/mypy.ini`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [mypy]
-exclude = (venv/|src/fixpoint_sdk/openapi/gen)
+exclude = (venv/)
 # Start off with these
 warn_unused_configs = True
 warn_redundant_casts = True
 warn_unused_ignores = True
 
 # Getting these passing should be easy
 strict_equality = True
```

### Comparing `fixpoint_sdk-0.6.0/requirements.txt` & `fixpoint_sdk-0.8.0rc0/requirements.txt`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.6.0/.github/workflows/ci.yml` & `fixpoint_sdk-0.8.0rc0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.6.0/.github/workflows/pypi-release-prod.yml` & `fixpoint_sdk-0.8.0rc0/.github/workflows/pypi-release-prod.yml`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.6.0/.github/workflows/pypi-release-test.yml` & `fixpoint_sdk-0.8.0rc0/.github/workflows/pypi-release-test.yml`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.6.0/bin/pip-freeze` & `fixpoint_sdk-0.8.0rc0/bin/pip-freeze`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.6.0/examples/main.py` & `fixpoint_sdk-0.8.0rc0/examples/main.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.6.0/examples/router.py` & `fixpoint_sdk-0.8.0rc0/examples/router.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,43 +48,43 @@
     2. After that, it will try to use gpt-3.5-turbo-0301, until spending $0.0001.
     3. After that, it rejects requests.
     """
     routing_config_req = openapi_client.V1CreateRoutingConfigRequest(
         fallback_strategy=openapi_client.V1FallbackStrategy.FALLBACK_STRATEGY_NEXT,
         terminal_state=openapi_client.V1TerminalState.TERMINAL_STATE_ERROR,
         models=[
-            openapi_client.V1Model(
+            openapi_client.Fixpointv1Model(
                 provider="openai",
                 name="gpt-3.5-turbo-0125",
                 spend_cap=openapi_client.V1SpendCap(
                     amount="0.0001",
                     currency="USD",
                     reset_interval=openapi_client.V1ResetInterval.RESET_INTERVAL_MONTHLY,
                 ),
             ),
-            openapi_client.V1Model(
+            openapi_client.Fixpointv1Model(
                 provider="openai",
                 name="gpt-3.5-turbo-0301",
                 spend_cap=openapi_client.V1SpendCap(
                     amount="0.0001",
                     currency="USD",
                     reset_interval=openapi_client.V1ResetInterval.RESET_INTERVAL_MONTHLY,
                 ),
             ),
         ],
         description="This is a test routing config.",
     )
 
     try:
-        routing_config = client.fixpoint.proxy_client.llm_proxy_create_routing_config(
+        routing_config = client.fixpoint.proxy_client.fixpoint_create_routing_config(
             routing_config_req
         )
     except ApiException as e:
         print(
-            f"Exception when calling LLMProxyApi->llm_proxy_create_routing_config: {e}\n"
+            f"Exception when calling FixpointApi->fixpoint_create_routing_config: {e}\n"
         )
         raise
     print(f"Routing config created. ID = {routing_config.id}")
 
 
 def create_routing_config_last_uncapped(client: ChatRouterClient) -> None:
     """Create a routing config where the last model is uncapped.
@@ -94,37 +94,38 @@
     1. Tries to use gpt-3.5-turbo-0125 until it has spent $0.0001.
     2. After that, it will use gpt-3.5-turbo-0301, without a spending cap.
     """
     routing_config_req = openapi_client.V1CreateRoutingConfigRequest(
         fallback_strategy=openapi_client.V1FallbackStrategy.FALLBACK_STRATEGY_NEXT,
         terminal_state=openapi_client.V1TerminalState.TERMINAL_STATE_IGNORE_CAP,
         models=[
-            openapi_client.V1Model(
+            openapi_client.Fixpointv1Model(
                 provider="openai",
                 name="gpt-3.5-turbo-0125",
                 spend_cap=openapi_client.V1SpendCap(
                     amount="0.0001",
                     currency="USD",
                     reset_interval=openapi_client.V1ResetInterval.RESET_INTERVAL_MONTHLY,
                 ),
             ),
-            openapi_client.V1Model(
+            openapi_client.Fixpointv1Model(
                 provider="openai",
                 name="gpt-3.5-turbo-0301",
             ),
         ],
         description="This is a test routing config.",
     )
 
     try:
-        routing_config = client.fixpoint.proxy_client.llm_proxy_create_routing_config(
+        routing_config = client.fixpoint.proxy_client.fixpoint_create_routing_config(
             routing_config_req
         )
         print(f"Routing config created. ID = {routing_config.id}")
     except ApiException as e:
         print(
-            f"Exception when calling LLMProxyApi->llm_proxy_create_routing_config: {e}\n"
+            f"Exception when calling FixpointApi->fixpoint_create_routing_config: {e}\n"
         )
+        raise
 
 
 if __name__ == "__main__":
     main(os.environ.get("SKIP_CREATING_CONFIG", "false").lower() == "true")
```

### Comparing `fixpoint_sdk-0.6.0/examples/streaming.py` & `fixpoint_sdk-0.8.0rc0/examples/streaming.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.6.0/src/fixpoint_sdk/__init__.py` & `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """The Fixpoint SDK provides a Python client for the Fixpoint API."""
 
+import fixpoint_openapi as openapi_client
+
 from .client import FixpointClient, ChatRouterClient
 from .completions import FixpointChatCompletion, FixpointChatCompletionStream
-from .openapi.gen import openapi_client
 from . import types
 from .types import ThumbsReaction, ModeType
 from . import compat
 from .lib.logging import logger, LOGGER_NAME
 
 from .lib.exc import FixpointException, InitException, ApiException
```

### Comparing `fixpoint_sdk-0.6.0/src/fixpoint_sdk/client.py` & `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,49 @@
 """Defines the Fixpoint client, which is the main interface for the SDK."""
 
+from dataclasses import dataclass
 import typing
 
 from openai import OpenAI
 
-from .openapi.gen.openapi_client.configuration import Configuration
-from .openapi.gen.openapi_client.api_client import ApiClient
-from .openapi.gen.openapi_client.api.llm_proxy_api import LLMProxyApi
+from fixpoint_openapi.configuration import Configuration
+from fixpoint_openapi.api_client import ApiClient
+from fixpoint_openapi.api.fixpoint_api import FixpointApi
 
 from .lib.env import get_fixpoint_api_key, get_api_base_url
 from .lib.requests import Requester
 from . import types
-from .completions import Chat, ChatWithRouter
+from .completions import Chat, ChatWithRouter, _ChatDeps
+from ._logging_api import LLMLogging
+
+
+@dataclass
+class _FixpointClientDeps:
+    chat: typing.Optional[_ChatDeps] = None
+    requester: typing.Optional[Requester] = None
 
 
 class _FixpointClientBase:
     def __init__(
         self,
         *,
         fixpoint_api_key: typing.Optional[str] = None,
         openai_api_key: typing.Optional[str] = None,
         api_base_url: typing.Optional[str] = None,
+        _deps: typing.Optional[_FixpointClientDeps] = None,
         **kwargs: typing.Any,
     ):
         # Check that the environment variable FIXPOINT_API_KEY is set
         _api_key = get_fixpoint_api_key(fixpoint_api_key)
 
         self._api_key = _api_key
-        self._requester = Requester(self._api_key, get_api_base_url(api_base_url))
+        if _deps and _deps.requester:
+            self._requester = _deps.requester
+        else:
+            self._requester = Requester(self._api_key, get_api_base_url(api_base_url))
         if openai_api_key:
             kwargs = dict(kwargs, api_key=openai_api_key)
         self.fixpoint = _Fixpoint(self._requester)
 
 
 class ChatRouterClient(_FixpointClientBase):
     """The ChatRouterClient lets you interact with the Fixpoint API and the OpenAI API."""
@@ -46,54 +58,64 @@
     ):
         super().__init__(
             fixpoint_api_key=fixpoint_api_key,
             openai_api_key=openai_api_key,
             api_base_url=api_base_url,
             **kwargs,
         )
-        client = OpenAI(**kwargs)
+        client = OpenAI(api_key=openai_api_key, **kwargs)
         self.chat = ChatWithRouter(self._requester, client)
 
 
 class FixpointClient(_FixpointClientBase):
     """The FixpointClient lets you interact with the Fixpoint API."""
 
     def __init__(
         self,
         *,
         fixpoint_api_key: typing.Optional[str] = None,
         openai_api_key: typing.Optional[str] = None,
         api_base_url: typing.Optional[str] = None,
+        _deps: typing.Optional[_FixpointClientDeps] = None,
         **kwargs: typing.Any,
     ):
         super().__init__(
             fixpoint_api_key=fixpoint_api_key,
             openai_api_key=openai_api_key,
             api_base_url=api_base_url,
+            _deps=_deps,
             **kwargs,
         )
-        client = OpenAI(**kwargs)
-        self.chat = Chat(self._requester, client)
+        client = OpenAI(api_key=openai_api_key, **kwargs)
+        chat_deps = None
+        if _deps:
+            chat_deps = _deps.chat
+        self.chat = Chat(self._requester, client, _deps=chat_deps)
 
 
 class _Fixpoint:
     def __init__(self, requester: Requester):
         self.user_feedback = self._UserFeedback(requester)
         self.attributes = self._Attributes(requester)
+        self.logging = self._Logging(LLMLogging(requester))
 
         configuration = Configuration(
-            host=get_api_base_url(requester.base_url),
+            host=get_api_base_url(requester.base_url()),
         )
 
         api_client = ApiClient(
             configuration,
             header_name="Authorization",
-            header_value=f"Bearer {requester.api_key}",
+            header_value=f"Bearer {requester.api_key()}",
         )
-        self.proxy_client = LLMProxyApi(api_client)
+        self.proxy_client = FixpointApi(api_client)
+
+    class _Logging:
+        def __init__(self, llm: LLMLogging):
+            self.llm = llm
 
     class _UserFeedback:
         def __init__(self, requester: Requester):
             self._requester = requester
 
         def create(
             self, request: types.CreateUserFeedbackRequest
```

### Comparing `fixpoint_sdk-0.6.0/src/fixpoint_sdk/compat.py` & `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/compat.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.6.0/src/fixpoint_sdk/lib/debugging.py` & `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/debugging.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.6.0/src/fixpoint_sdk/lib/env.py` & `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/env.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.6.0/src/fixpoint_sdk/lib/exc.py` & `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/exc.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.6.0/src/fixpoint_sdk/lib/iterwrapper.py` & `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/iterwrapper.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.6.0/src/fixpoint_sdk/lib/requests.py` & `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/lib/requests.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,48 +13,57 @@
 
 ApiCallback = typing.Callable[[str, typing.Any, typing.Any], None]
 
 
 class Requester:
     """Makes requests to the Fixpoint API."""
 
-    api_key: str
-    base_url: str
+    _api_key: str
+    _base_url: str
     timeout_s: int
     _on_api_call: typing.Optional[ApiCallback]
 
     def __init__(
         self,
         api_key: str,
         base_url: str,
         timeout_s: int = DEFAULT_TIMEOUT_S,
         _on_api_call: typing.Optional[ApiCallback] = None,
     ):
-        self.api_key = api_key
-        self.base_url = base_url
+        self._api_key = api_key
+        self._base_url = base_url
         self.timeout_s = timeout_s
 
-        if self.base_url[-1] == "/":
-            self.base_url = self.base_url[:-1]
+        if self._base_url[-1] == "/":
+            self._base_url = self._base_url[:-1]
 
         self._on_api_call = _on_api_call
 
+    def base_url(self) -> str:
+        """Get the base URL."""
+        return self._base_url
+
+    def api_key(self) -> str:
+        """Get the API key."""
+        return self._api_key
+
     @debug_log_function_io
     def create_openai_routed_log(
         self,
-        request: types.OpenAILLMInputLog,
+        request: types.openai.RoutedCreateChatCompletionRequest,
         trace_id: typing.Optional[str] = None,
         mode: types.ModeType = types.ModeType.MODE_UNSPECIFIED,
     ) -> types.ChatCompletion:
         """Create routed input log for an LLM inference request."""
-        url = f"{self.base_url}/v1/router"
+        url = f"{self._base_url}/v1/router"
+        req_dict = request.to_dict()
         input_log_req = types.CreateLLMRoutingRequest(
-            messages=request["messages"],
-            user_id=request.get("user", None),
-            temperature=request.get("temperature", None),
+            messages=request.messages,
+            user_id=req_dict.get("user", None),
+            temperature=req_dict.get("temperature", None),
             trace_id=trace_id,
             mode=mode,
         )
 
         return typing.cast(
             types.ChatCompletion,
             self._post_to_fixpoint(url, input_log_req.to_dict()).json(),
@@ -65,15 +74,15 @@
         self,
         model_name: str,
         request: types.OpenAILLMInputLog,
         trace_id: typing.Optional[str] = None,
         mode: types.ModeType = types.ModeType.MODE_UNSPECIFIED,
     ) -> types.InputLog:
         """Create an input log for an LLM inference request."""
-        url = f"{self.base_url}/v1/openai_chats/{model_name}/input_logs"
+        url = f"{self._base_url}/v1/openai_chats/{model_name}/input_logs"
         input_log_req = types.CreateLLMInputLogRequest(
             model_name=model_name,
             messages=request["messages"],
             user_id=request.get("user", None),
             temperature=request.get("temperature", None),
             trace_id=trace_id,
             mode=mode,
@@ -88,15 +97,15 @@
         model_name: str,
         input_log_results: types.InputLog,
         open_ai_response: ChatCompletion,
         trace_id: typing.Optional[str] = None,
         mode: types.ModeType = types.ModeType.MODE_UNSPECIFIED,
     ) -> types.OutputLog:
         """Create an output log for an LLM inference response."""
-        url = f"{self.base_url}/v1/openai_chats/{model_name}/output_logs"
+        url = f"{self._base_url}/v1/openai_chats/{model_name}/output_logs"
 
         # If input_log_results doesn't have id then error
         if "name" not in input_log_results:
             raise ValueError("input_log_results must have a name")
 
         # If open_ai_response doesn't have id then error
         if not open_ai_response.id:
@@ -132,15 +141,15 @@
         )
 
     @debug_log_function_io
     def create_user_feedback(
         self, request: types.CreateUserFeedbackRequest
     ) -> types.CreateUserFeedbackResponse:
         """Create user feedback on an LLM log."""
-        url = f"{self.base_url}/v1/likes"
+        url = f"{self._base_url}/v1/likes"
 
         if "likes" not in request:
             raise ValueError("request must have a likes")
 
         if not isinstance(request["likes"], list):
             raise ValueError("request.likes must be a list")
 
@@ -170,15 +179,15 @@
         return typing.cast(types.CreateUserFeedbackResponse, resp.json())
 
     @debug_log_function_io
     def create_attribute(
         self, request: types.CreateLogAttributeRequest
     ) -> types.LogAttribute:
         """Create a LLM log attribute and attach it to that LLM log."""
-        url = f"{self.base_url}/v1/attributes"
+        url = f"{self._base_url}/v1/attributes"
 
         if "log_attribute" not in request:
             raise ValueError("request must have a log_attribute")
 
         log_attribute = request["log_attribute"]
 
         if "key" not in log_attribute:
@@ -198,15 +207,15 @@
 
     @debug_log_function_io
     def _post_to_fixpoint(
         self, url: str, req_or_resp_obj: typing.Dict[str, typing.Any]
     ) -> requests.Response:
         headers = {
             "Accept": "application/json",
-            "Authorization": f"Bearer {self.api_key}",
+            "Authorization": f"Bearer {self.api_key()}",
         }
         resp = requests.post(
             url, headers=headers, json=req_or_resp_obj, timeout=self.timeout_s
         )
         try:
             resp.raise_for_status()
         except requests.HTTPError as e:
```

### Comparing `fixpoint_sdk-0.6.0/src/fixpoint_sdk/types/__init__.py` & `fixpoint_sdk-0.8.0rc0/src/fixpoint_sdk/types/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """Type definitions for the Fixpoint SDK."""
 
 from dataclasses import dataclass, asdict
 import enum
 from typing import Any, Dict, List, Literal, Optional, TypedDict, Union
 from openai.types.chat import ChatCompletionMessageParam
 
+from . import openai
+from ._utils import to_dict_without_not_given, is_not_given, get_value_or_none
+
+__all__ = ["openai", "is_not_given", "get_value_or_none"]
+
 
 class ThumbsReaction(enum.Enum):
     """The specific user feedback reaction."""
 
     THUMBS_UNSPECIFIED = 0
     THUMBS_UP = 1
     THUMBS_DOWN = 2
@@ -48,19 +53,22 @@
     Literal[0],
     Literal[1],
     Literal[2],
     Literal[3],
 ]
 
 
-def parse_mode_type(mode: Optional[Union[str, int, object]] = None) -> ModeType:
+def parse_mode_type(
+    mode: Optional[Union[str, int, object, ModeType]] = None
+) -> ModeType:
     """Parse a mode type from a string."""
     if mode is None:
         return ModeType.MODE_UNSPECIFIED
-
+    if isinstance(mode, ModeType):
+        return mode
     if isinstance(mode, int):
         return ModeType(mode)
 
     if isinstance(mode, str):
         if mode == "unspecified":
             return ModeType.MODE_UNSPECIFIED
         if mode == "test":
@@ -80,15 +88,15 @@
     temperature: Optional[float] = None
     user_id: Optional[str] = None
     trace_id: Optional[str] = None
     mode: Optional[ModeType] = ModeType.MODE_UNSPECIFIED
 
     def to_dict(self) -> Dict[str, Any]:
         """Convert this request to a dictionary."""
-        d = asdict(self)
+        d = to_dict_without_not_given(self)
         if self.mode is not None:
             d["mode"] = self.mode.value
         return d
 
 
 @dataclass
 class CreateLLMInputLogRequest:
@@ -99,23 +107,23 @@
     user_id: Optional[str] = None
     temperature: Optional[float] = None
     trace_id: Optional[str] = None
     mode: Optional[ModeType] = ModeType.MODE_UNSPECIFIED
 
     def to_dict(self) -> Dict[str, Any]:
         """Convert this request to a dictionary."""
-        d = asdict(self)
+        d = to_dict_without_not_given(self)
         # convert this to a JSON-serializable type
         if self.mode is not None:
             d["mode"] = self.mode.value
         return d
 
 
 class OpenAILLMInputLog(TypedDict, total=False):
-    """An input log with attributes from OpenAI response.
+    """An input log with attributes from OpenAI request.
 
     This input log has some attributes that come directly from an OpenAI
     response. Some of the field names are slightly off from what our Fixpoint
     API expects, so we need to transform this to a `CreateLLMInputLogRequest`.
     """
 
     model: str
```

### Comparing `fixpoint_sdk-0.6.0/tests/mock_completions.py` & `fixpoint_sdk-0.8.0rc0/tests/mock_completions.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.6.0/tests/test_completions.py` & `fixpoint_sdk-0.8.0rc0/tests/test_completions.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.6.0/tests/test_types.py` & `fixpoint_sdk-0.8.0rc0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.6.0/tests/lib/test_iterwrapper.py` & `fixpoint_sdk-0.8.0rc0/tests/lib/test_iterwrapper.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.6.0/tests/lib/test_requests.py` & `fixpoint_sdk-0.8.0rc0/tests/lib/test_requests.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.6.0/LICENSE` & `fixpoint_sdk-0.8.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.6.0/README.md` & `fixpoint_sdk-0.8.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.6.0/pyproject.toml` & `fixpoint_sdk-0.8.0rc0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fixpoint_sdk"
-version = "0.6.0"
+version = "0.8.0-rc00"
 
 authors = [
 { name="Jakub Cichon", email="jakub@fixpoint.co" },
 { name="Dylan Mikus", email="dylan@fixpoint.co" },
 ]
 description = "Python SDK for Fixpoint - Auto-improvement to make your LLM apps smarter"
 readme = "README.md"
@@ -20,15 +20,16 @@
 ]
 
 dependencies = [
   "openai>=1.6.1",
   "requests==2.31.0",
   "python-dateutil>=2.8.2",
   "pydantic>=2",
-  "typing-extensions>=4.7.1"
+  "typing-extensions>=4.7.1",
+  "fixpoint-openapi>=0.1.0"
 ]
 
 [project.optional-dependencies]
 dev = [
   "black>=24",
   "build>=1.1.1",
   "ipdb>=0.13.13",
```

### Comparing `fixpoint_sdk-0.6.0/PKG-INFO` & `fixpoint_sdk-0.8.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.3
 Name: fixpoint_sdk
-Version: 0.6.0
+Version: 0.8.0rc0
 Summary: Python SDK for Fixpoint - Auto-improvement to make your LLM apps smarter
 Project-URL: Homepage, https://github.com/gofixpoint/python-sdk
 Project-URL: Issues, https://github.com/gofixpoint/python-sdk/issues
 Author-email: Jakub Cichon <jakub@fixpoint.co>, Dylan Mikus <dylan@fixpoint.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: fixpoint-openapi>=0.1.0
 Requires-Dist: openai>=1.6.1
 Requires-Dist: pydantic>=2
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: requests==2.31.0
 Requires-Dist: typing-extensions>=4.7.1
 Provides-Extra: dev
 Requires-Dist: black>=24; extra == 'dev'
```

