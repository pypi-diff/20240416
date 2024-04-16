# Comparing `tmp/odp_sdk_python_ingest-0.4.8.tar.gz` & `tmp/odp_sdk_python_ingest-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odp_sdk_python_ingest-0.4.8.tar", max compression
+gzip compressed data, was "odp_sdk_python_ingest-0.4.9.tar", max compression
```

## Comparing `odp_sdk_python_ingest-0.4.8.tar` & `odp_sdk_python_ingest-0.4.9.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0      842 2023-08-16 09:22:41.871117 odp_sdk_python_ingest-0.4.8/README.md
--rw-r--r--   0        0        0        0 2023-08-16 09:22:41.871117 odp_sdk_python_ingest-0.4.8/odp/__init__.py
--rw-r--r--   0        0        0        0 2023-08-16 09:22:41.871117 odp_sdk_python_ingest-0.4.8/odp/auth/__init__.py
--rw-r--r--   0        0        0        0 2023-08-16 09:22:41.871117 odp_sdk_python_ingest-0.4.8/odp/auth/cdf/__init__.py
--rw-r--r--   0        0        0     3258 2023-08-16 09:22:41.871117 odp_sdk_python_ingest-0.4.8/odp/auth/cdf/cdf_token_handler.py
--rw-r--r--   0        0        0     1764 2023-08-16 09:22:41.871117 odp_sdk_python_ingest-0.4.8/odp/auth/cdf/federated_cognite_client.py
--rw-r--r--   0        0        0      163 2023-08-16 09:22:41.871117 odp_sdk_python_ingest-0.4.8/odp/auth/odp/__init__.py
--rw-r--r--   0        0        0     3306 2023-08-16 09:22:41.871117 odp_sdk_python_ingest-0.4.8/odp/auth/odp/interactive_login_token_handler.py
--rw-r--r--   0        0        0     1813 2023-08-16 09:22:41.871117 odp_sdk_python_ingest-0.4.8/odp/auth/odp/ropc_token_handler.py
--rw-r--r--   0        0        0     1358 2023-08-16 09:22:41.871117 odp_sdk_python_ingest-0.4.8/odp/auth/odp/token_handler.py
--rw-r--r--   0        0        0       49 2023-08-16 09:22:41.871117 odp_sdk_python_ingest-0.4.8/odp/auth/prefect/__init__.py
--rw-r--r--   0        0        0     3877 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/auth/prefect/prefect_b2c_client.py
--rw-r--r--   0        0        0        0 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/__init__.py
--rw-r--r--   0        0        0        0 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/blocks/__init__.py
--rw-r--r--   0        0        0     2490 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/blocks/aad_client_credentials.py
--rw-r--r--   0        0        0     1562 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/blocks/azure_key_vault.py
--rw-r--r--   0        0        0     6042 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/blocks/azure_storage.py
--rw-r--r--   0        0        0     2879 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/blocks/cdf_storage.py
--rw-r--r--   0        0        0      579 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/blocks/db_engine.py
--rw-r--r--   0        0        0      354 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/blocks/odcat.py
--rw-r--r--   0        0        0     2378 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/blocks/postgres.py
--rw-r--r--   0        0        0        0 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/cli/__init__.py
--rw-r--r--   0        0        0      479 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/cli/__main__.py
--rw-r--r--   0        0        0      435 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/cli/authenticate.py
--rw-r--r--   0        0        0     2610 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/cli/block.py
--rw-r--r--   0        0        0     5041 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/cli/context.py
--rw-r--r--   0        0        0     7296 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/cli/deploy.py
--rw-r--r--   0        0        0     2741 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/cli/parameters.py
--rw-r--r--   0        0        0       43 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/cli/params/__init__.py
--rw-r--r--   0        0        0      515 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/cli/params/type_param_type.py
--rw-r--r--   0        0        0     3421 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/cli/run.py
--rw-r--r--   0        0        0     1019 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/cli/schema.py
--rw-r--r--   0        0        0        0 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/config/__init__.py
--rw-r--r--   0        0        0      708 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/config/cdf_config.py
--rw-r--r--   0        0        0      816 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/config/dask_config.py
--rw-r--r--   0        0        0      125 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/deploy/__init__.py
--rw-r--r--   0        0        0      216 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/deploy/abstract_deployment_block.py
--rw-r--r--   0        0        0       40 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/deploy/block/__init__.py
--rw-r--r--   0        0        0      501 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/deploy/block/generic_block.py
--rw-r--r--   0        0        0     1591 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/deploy/deployment_block_factory.py
--rw-r--r--   0        0        0      190 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/deploy/runtime/__init__.py
--rw-r--r--   0        0        0      481 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/deploy/runtime/abstract_runtime.py
--rw-r--r--   0        0        0     3463 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/deploy/runtime/kubernetes.py
--rw-r--r--   0        0        0     4567 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/deploy/runtime/kubernetes_dask.py
--rw-r--r--   0        0        0     1718 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/deploy/runtime/kubernetes_tiered_resource.py
--rw-r--r--   0        0        0       88 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/deploy/schedule/__init__.py
--rw-r--r--   0        0        0      417 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/deploy/schedule/abstract_schedule.py
--rw-r--r--   0        0        0      471 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/deploy/schedule/cron_schedule.py
--rw-r--r--   0        0        0     1030 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/deploy/schedule/interval_schedule.py
--rw-r--r--   0        0        0       73 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/deploy/storage/__init__.py
--rw-r--r--   0        0        0      938 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/deploy/storage/abstract_storage.py
--rw-r--r--   0        0        0    10993 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/deploy/storage/docker.py
--rw-r--r--   0        0        0        0 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/deploy/storage/prefect_healthcheck.py
--rw-r--r--   0        0        0        0 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/flow_state/__init__.py
--rw-r--r--   0        0        0     4679 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/flow_state/stateful_value_impl.py
--rw-r--r--   0        0        0        0 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/flow_state/store/__init__.py
--rw-r--r--   0        0        0     1060 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/flow_state/store/watermark_file_store.py
--rw-r--r--   0        0        0      639 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/flow_state/store/watermark_inmemory_store.py
--rw-r--r--   0        0        0      728 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/flow_state/store/watermark_redis_store.py
--rw-r--r--   0        0        0     5488 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/secrets.py
--rw-r--r--   0        0        0        0 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/state_handlers/__init__.py
--rw-r--r--   0        0        0     2005 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/state_handlers/metrics_pusher.py
--rw-r--r--   0        0        0        0 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/tasks/__init__.py
--rw-r--r--   0        0        0        0 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/tasks/cdf/__init__.py
--rw-r--r--   0        0        0     3217 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/tasks/cdf/cdf_credentials.py
--rw-r--r--   0        0        0     1438 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/tasks/concurrency_limit.py
--rw-r--r--   0        0        0      705 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/tasks/measured_task.py
--rw-r--r--   0        0        0     1580 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/compute/tasks/tasks.py
--rw-r--r--   0        0        0        0 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/metrics/__init__.py
--rw-r--r--   0        0        0     4758 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/metrics/abstract_metrics.py
--rw-r--r--   0        0        0     2303 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/metrics/metric_client.py
--rw-r--r--   0        0        0        0 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/metrics/mock/__init__.py
--rw-r--r--   0        0        0     2523 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/metrics/mock/metric_client.py
--rw-r--r--   0        0        0     3271 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/metrics/mock/metrics.py
--rw-r--r--   0        0        0        0 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/metrics/prometheus/__init__.py
--rw-r--r--   0        0        0     2613 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/metrics/prometheus/metric_client.py
--rw-r--r--   0        0        0     3686 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/metrics/prometheus/metrics.py
--rw-r--r--   0        0        0        0 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/types/__init__.py
--rw-r--r--   0        0        0      361 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/types/file_info.py
--rw-r--r--   0        0        0      248 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/utils/__init__.py
--rw-r--r--   0        0        0     2887 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/utils/args.py
--rw-r--r--   0        0        0     1128 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/utils/deploy_helpers.py
--rw-r--r--   0        0        0     4913 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/utils/import_helpers.py
--rw-r--r--   0        0        0      607 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/utils/naming.py
--rw-r--r--   0        0        0     5715 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/utils/retry.py
--rw-r--r--   0        0        0      317 2023-08-16 09:22:41.875117 odp_sdk_python_ingest-0.4.8/odp/utils/timers.py
--rw-r--r--   0        0        0     1945 2023-08-16 09:23:48.265568 odp_sdk_python_ingest-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     2544 1970-01-01 00:00:00.000000 odp_sdk_python_ingest-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0      842 2023-08-18 14:13:08.549165 odp_sdk_python_ingest-0.4.9/README.md
+-rw-r--r--   0        0        0        0 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/auth/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/auth/cdf/__init__.py
+-rw-r--r--   0        0        0     3258 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/auth/cdf/cdf_token_handler.py
+-rw-r--r--   0        0        0     1764 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/auth/cdf/federated_cognite_client.py
+-rw-r--r--   0        0        0      163 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/auth/odp/__init__.py
+-rw-r--r--   0        0        0     3306 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/auth/odp/interactive_login_token_handler.py
+-rw-r--r--   0        0        0     1813 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/auth/odp/ropc_token_handler.py
+-rw-r--r--   0        0        0     1358 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/auth/odp/token_handler.py
+-rw-r--r--   0        0        0       49 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/auth/prefect/__init__.py
+-rw-r--r--   0        0        0     3877 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/auth/prefect/prefect_b2c_client.py
+-rw-r--r--   0        0        0        0 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/blocks/__init__.py
+-rw-r--r--   0        0        0     2490 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/blocks/aad_client_credentials.py
+-rw-r--r--   0        0        0     1620 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/blocks/azure_key_vault.py
+-rw-r--r--   0        0        0     6042 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/blocks/azure_storage.py
+-rw-r--r--   0        0        0     2879 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/blocks/cdf_storage.py
+-rw-r--r--   0        0        0      579 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/blocks/db_engine.py
+-rw-r--r--   0        0        0      354 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/blocks/odcat.py
+-rw-r--r--   0        0        0     2378 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/blocks/postgres.py
+-rw-r--r--   0        0        0        0 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/cli/__init__.py
+-rw-r--r--   0        0        0      479 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/cli/__main__.py
+-rw-r--r--   0        0        0      435 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/cli/authenticate.py
+-rw-r--r--   0        0        0     2610 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/cli/block.py
+-rw-r--r--   0        0        0     5041 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/cli/context.py
+-rw-r--r--   0        0        0     7296 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/cli/deploy.py
+-rw-r--r--   0        0        0     2741 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/cli/parameters.py
+-rw-r--r--   0        0        0       43 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/cli/params/__init__.py
+-rw-r--r--   0        0        0      515 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/cli/params/type_param_type.py
+-rw-r--r--   0        0        0     3421 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/cli/run.py
+-rw-r--r--   0        0        0     1019 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/cli/schema.py
+-rw-r--r--   0        0        0        0 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/config/__init__.py
+-rw-r--r--   0        0        0      708 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/config/cdf_config.py
+-rw-r--r--   0        0        0      816 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/config/dask_config.py
+-rw-r--r--   0        0        0      125 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/deploy/__init__.py
+-rw-r--r--   0        0        0      216 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/deploy/abstract_deployment_block.py
+-rw-r--r--   0        0        0       40 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/deploy/block/__init__.py
+-rw-r--r--   0        0        0      501 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/deploy/block/generic_block.py
+-rw-r--r--   0        0        0     1591 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/deploy/deployment_block_factory.py
+-rw-r--r--   0        0        0      190 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/deploy/runtime/__init__.py
+-rw-r--r--   0        0        0      481 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/deploy/runtime/abstract_runtime.py
+-rw-r--r--   0        0        0     3463 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/deploy/runtime/kubernetes.py
+-rw-r--r--   0        0        0     4567 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/deploy/runtime/kubernetes_dask.py
+-rw-r--r--   0        0        0     1718 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/deploy/runtime/kubernetes_tiered_resource.py
+-rw-r--r--   0        0        0       88 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/deploy/schedule/__init__.py
+-rw-r--r--   0        0        0      417 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/deploy/schedule/abstract_schedule.py
+-rw-r--r--   0        0        0      471 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/deploy/schedule/cron_schedule.py
+-rw-r--r--   0        0        0     1030 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/deploy/schedule/interval_schedule.py
+-rw-r--r--   0        0        0       73 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/deploy/storage/__init__.py
+-rw-r--r--   0        0        0      938 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/deploy/storage/abstract_storage.py
+-rw-r--r--   0        0        0    10993 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/deploy/storage/docker.py
+-rw-r--r--   0        0        0        0 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/deploy/storage/prefect_healthcheck.py
+-rw-r--r--   0        0        0        0 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/flow_state/__init__.py
+-rw-r--r--   0        0        0     4679 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/flow_state/stateful_value_impl.py
+-rw-r--r--   0        0        0        0 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/flow_state/store/__init__.py
+-rw-r--r--   0        0        0     1060 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/flow_state/store/watermark_file_store.py
+-rw-r--r--   0        0        0      639 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/flow_state/store/watermark_inmemory_store.py
+-rw-r--r--   0        0        0      728 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/flow_state/store/watermark_redis_store.py
+-rw-r--r--   0        0        0     5488 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/secrets.py
+-rw-r--r--   0        0        0        0 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/state_handlers/__init__.py
+-rw-r--r--   0        0        0     2005 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/state_handlers/metrics_pusher.py
+-rw-r--r--   0        0        0        0 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/tasks/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/tasks/cdf/__init__.py
+-rw-r--r--   0        0        0     3217 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/tasks/cdf/cdf_credentials.py
+-rw-r--r--   0        0        0     1438 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/tasks/concurrency_limit.py
+-rw-r--r--   0        0        0      705 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/tasks/measured_task.py
+-rw-r--r--   0        0        0     1580 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/compute/tasks/tasks.py
+-rw-r--r--   0        0        0        0 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/metrics/__init__.py
+-rw-r--r--   0        0        0     4758 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/metrics/abstract_metrics.py
+-rw-r--r--   0        0        0     2303 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/metrics/metric_client.py
+-rw-r--r--   0        0        0        0 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/metrics/mock/__init__.py
+-rw-r--r--   0        0        0     2523 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/metrics/mock/metric_client.py
+-rw-r--r--   0        0        0     3271 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/metrics/mock/metrics.py
+-rw-r--r--   0        0        0        0 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/metrics/prometheus/__init__.py
+-rw-r--r--   0        0        0     2613 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/metrics/prometheus/metric_client.py
+-rw-r--r--   0        0        0     3686 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/metrics/prometheus/metrics.py
+-rw-r--r--   0        0        0        0 2023-08-18 14:13:08.553165 odp_sdk_python_ingest-0.4.9/odp/types/__init__.py
+-rw-r--r--   0        0        0      361 2023-08-18 14:13:08.557165 odp_sdk_python_ingest-0.4.9/odp/types/file_info.py
+-rw-r--r--   0        0        0      248 2023-08-18 14:13:08.557165 odp_sdk_python_ingest-0.4.9/odp/utils/__init__.py
+-rw-r--r--   0        0        0     2887 2023-08-18 14:13:08.557165 odp_sdk_python_ingest-0.4.9/odp/utils/args.py
+-rw-r--r--   0        0        0     1128 2023-08-18 14:13:08.557165 odp_sdk_python_ingest-0.4.9/odp/utils/deploy_helpers.py
+-rw-r--r--   0        0        0     4913 2023-08-18 14:13:08.557165 odp_sdk_python_ingest-0.4.9/odp/utils/import_helpers.py
+-rw-r--r--   0        0        0      607 2023-08-18 14:13:08.557165 odp_sdk_python_ingest-0.4.9/odp/utils/naming.py
+-rw-r--r--   0        0        0     5715 2023-08-18 14:13:08.557165 odp_sdk_python_ingest-0.4.9/odp/utils/retry.py
+-rw-r--r--   0        0        0      317 2023-08-18 14:13:08.557165 odp_sdk_python_ingest-0.4.9/odp/utils/timers.py
+-rw-r--r--   0        0        0     1945 2023-08-18 14:14:30.750458 odp_sdk_python_ingest-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     2544 1970-01-01 00:00:00.000000 odp_sdk_python_ingest-0.4.9/PKG-INFO
```

### Comparing `odp_sdk_python_ingest-0.4.8/README.md` & `odp_sdk_python_ingest-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/auth/cdf/cdf_token_handler.py` & `odp_sdk_python_ingest-0.4.9/odp/auth/cdf/cdf_token_handler.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/auth/cdf/federated_cognite_client.py` & `odp_sdk_python_ingest-0.4.9/odp/auth/cdf/federated_cognite_client.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/auth/odp/interactive_login_token_handler.py` & `odp_sdk_python_ingest-0.4.9/odp/auth/odp/interactive_login_token_handler.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/auth/odp/ropc_token_handler.py` & `odp_sdk_python_ingest-0.4.9/odp/auth/odp/ropc_token_handler.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/auth/odp/token_handler.py` & `odp_sdk_python_ingest-0.4.9/odp/auth/odp/token_handler.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/auth/prefect/prefect_b2c_client.py` & `odp_sdk_python_ingest-0.4.9/odp/auth/prefect/prefect_b2c_client.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/blocks/aad_client_credentials.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/blocks/aad_client_credentials.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/blocks/azure_key_vault.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/blocks/azure_key_vault.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,17 @@
     _block_type_name = "Azure Key Vault"
     _logo_url = "https://stprododpcmscdnendpoint.azureedge.net/assets/icons/azure-storage.png"  # type: ignore
 
     aad_client_credentials: AadClientCredentials
     key_vault_url: AnyHttpUrl
     client: Optional[KeyClient]
 
+    class Config:
+        arbitrary_types_allowed = True
+
     def block_initialization(self) -> None:
         """Validate the block setup and create an authenticated client for the key vault."""
 
         try:
             tenant_id = re.search(
                 "https://login.microsoftonline.com/(.+?)/oauth2/v2.0/token", self.aad_client_credentials.token_url
             ).group(1)
```

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/blocks/azure_storage.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/blocks/azure_storage.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/blocks/cdf_storage.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/blocks/cdf_storage.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/blocks/db_engine.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/blocks/db_engine.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/blocks/postgres.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/blocks/postgres.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/cli/block.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/cli/block.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/cli/context.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/cli/context.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/cli/deploy.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/cli/parameters.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/cli/parameters.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/cli/params/type_param_type.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/cli/params/type_param_type.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/cli/run.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/cli/run.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/cli/schema.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/cli/schema.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/config/cdf_config.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/config/cdf_config.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/config/dask_config.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/config/dask_config.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/deploy/deployment_block_factory.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/deploy/deployment_block_factory.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/deploy/runtime/kubernetes.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/deploy/runtime/kubernetes.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/deploy/runtime/kubernetes_dask.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/deploy/runtime/kubernetes_dask.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/deploy/runtime/kubernetes_tiered_resource.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/deploy/runtime/kubernetes_tiered_resource.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/deploy/schedule/interval_schedule.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/deploy/schedule/interval_schedule.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/deploy/storage/abstract_storage.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/deploy/storage/abstract_storage.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/deploy/storage/docker.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/deploy/storage/docker.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/flow_state/stateful_value_impl.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/flow_state/stateful_value_impl.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/flow_state/store/watermark_file_store.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/flow_state/store/watermark_file_store.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/flow_state/store/watermark_inmemory_store.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/flow_state/store/watermark_inmemory_store.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/flow_state/store/watermark_redis_store.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/flow_state/store/watermark_redis_store.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/secrets.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/secrets.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/state_handlers/metrics_pusher.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/state_handlers/metrics_pusher.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/tasks/cdf/cdf_credentials.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/tasks/cdf/cdf_credentials.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/tasks/concurrency_limit.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/tasks/concurrency_limit.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/tasks/measured_task.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/tasks/measured_task.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/compute/tasks/tasks.py` & `odp_sdk_python_ingest-0.4.9/odp/compute/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/metrics/abstract_metrics.py` & `odp_sdk_python_ingest-0.4.9/odp/metrics/abstract_metrics.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/metrics/metric_client.py` & `odp_sdk_python_ingest-0.4.9/odp/metrics/metric_client.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/metrics/mock/metric_client.py` & `odp_sdk_python_ingest-0.4.9/odp/metrics/mock/metric_client.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/metrics/mock/metrics.py` & `odp_sdk_python_ingest-0.4.9/odp/metrics/mock/metrics.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/metrics/prometheus/metric_client.py` & `odp_sdk_python_ingest-0.4.9/odp/metrics/prometheus/metric_client.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/metrics/prometheus/metrics.py` & `odp_sdk_python_ingest-0.4.9/odp/metrics/prometheus/metrics.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/utils/args.py` & `odp_sdk_python_ingest-0.4.9/odp/utils/args.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/utils/deploy_helpers.py` & `odp_sdk_python_ingest-0.4.9/odp/utils/deploy_helpers.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/utils/import_helpers.py` & `odp_sdk_python_ingest-0.4.9/odp/utils/import_helpers.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/utils/naming.py` & `odp_sdk_python_ingest-0.4.9/odp/utils/naming.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/odp/utils/retry.py` & `odp_sdk_python_ingest-0.4.9/odp/utils/retry.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.8/pyproject.toml` & `odp_sdk_python_ingest-0.4.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odp-sdk-python-ingest"
-version = "0.4.8"
+version = "0.4.9"
 description = "ODP ingest SDK"
 authors = ["Thomas Li Fredriksen <thomas.fredriksen@oceandata.earth>"]
 readme = "README.md"
 packages = [
     {include="odp"}
 ]
```

### Comparing `odp_sdk_python_ingest-0.4.8/PKG-INFO` & `odp_sdk_python_ingest-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odp-sdk-python-ingest
-Version: 0.4.8
+Version: 0.4.9
 Summary: ODP ingest SDK
 Author: Thomas Li Fredriksen
 Author-email: thomas.fredriksen@oceandata.earth
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: odp-sdk-python-ingest Version: 0.4.8 Summary: ODP
+Metadata-Version: 2.1 Name: odp-sdk-python-ingest Version: 0.4.9 Summary: ODP
 ingest SDK Author: Thomas Li Fredriksen Author-email:
 thomas.fredriksen@oceandata.earth Requires-Python: >=3.10,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist:
 azure-common (>=1.1.28,<2.0.0) Requires-Dist: azure-identity (>=1.11.0,<2.0.0)
 Requires-Dist: azure-keyvault (>=4.2.0,<5.0.0) Requires-Dist: azure-keyvault-
 secrets (>=4.6.0,<5.0.0) Requires-Dist: azure-storage-blob (>=12.13.1,<13.0.0)
```

