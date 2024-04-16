# Comparing `tmp/dagster-plus-0.0.1.tar.gz` & `tmp/dagster-plus-1.7.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-plus-0.0.1.tar", last modified: Wed Mar 27 17:06:57 2024, max compression
+gzip compressed data, was "dagster-plus-1.7.2rc1.tar", last modified: Tue Apr 16 18:02:11 2024, max compression
```

## Comparing `dagster-plus-0.0.1.tar` & `dagster-plus-1.7.2rc1.tar`

### file list

```diff
@@ -1,14 +1,140 @@
-drwxr-xr-x   0 shalabh    (501) staff       (20)        0 2024-03-27 17:06:57.082453 dagster-plus-0.0.1/
--rw-r--r--   0 shalabh    (501) staff       (20)       90 2024-03-27 14:54:57.000000 dagster-plus-0.0.1/LICENSE.md
--rw-r--r--   0 shalabh    (501) staff       (20)      444 2024-03-27 17:06:57.082226 dagster-plus-0.0.1/PKG-INFO
--rw-r--r--   0 shalabh    (501) staff       (20)       53 2024-03-27 15:03:02.000000 dagster-plus-0.0.1/README.md
-drwxr-xr-x   0 shalabh    (501) staff       (20)        0 2024-03-27 17:06:57.081027 dagster-plus-0.0.1/dagster_plus/
--rw-r--r--   0 shalabh    (501) staff       (20)        0 2024-03-27 14:54:40.000000 dagster-plus-0.0.1/dagster_plus/__init__.py
-drwxr-xr-x   0 shalabh    (501) staff       (20)        0 2024-03-27 17:06:57.082004 dagster-plus-0.0.1/dagster_plus.egg-info/
--rw-r--r--   0 shalabh    (501) staff       (20)      444 2024-03-27 17:06:57.000000 dagster-plus-0.0.1/dagster_plus.egg-info/PKG-INFO
--rw-r--r--   0 shalabh    (501) staff       (20)      239 2024-03-27 17:06:57.000000 dagster-plus-0.0.1/dagster_plus.egg-info/SOURCES.txt
--rw-r--r--   0 shalabh    (501) staff       (20)        1 2024-03-27 17:06:57.000000 dagster-plus-0.0.1/dagster_plus.egg-info/dependency_links.txt
--rw-r--r--   0 shalabh    (501) staff       (20)       14 2024-03-27 17:06:57.000000 dagster-plus-0.0.1/dagster_plus.egg-info/requires.txt
--rw-r--r--   0 shalabh    (501) staff       (20)       13 2024-03-27 17:06:57.000000 dagster-plus-0.0.1/dagster_plus.egg-info/top_level.txt
--rw-r--r--   0 shalabh    (501) staff       (20)      398 2024-03-27 15:02:56.000000 dagster-plus-0.0.1/pyproject.toml
--rw-r--r--   0 shalabh    (501) staff       (20)       38 2024-03-27 17:06:57.082490 dagster-plus-0.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.472538 dagster-plus-1.7.2rc1/
+-rw-r--r--   0 root         (0) root         (0)     4558 2024-04-16 18:02:11.472538 dagster-plus-1.7.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3056 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.408537 dagster-plus-1.7.2rc1/dagster_plus/
+-rw-r--r--   0 root         (0) root         (0)      160 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.408537 dagster-plus-1.7.2rc1/dagster_plus/agent/
+-rw-r--r--   0 root         (0) root         (0)      796 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.408537 dagster-plus-1.7.2rc1/dagster_plus/agent/cli/
+-rw-r--r--   0 root         (0) root         (0)     7581 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/agent/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45462 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/agent/dagster_cloud_agent.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/agent/queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.416538 dagster-plus-1.7.2rc1/dagster_plus/anomaly_detection/
+-rw-r--r--   0 root         (0) root         (0)      279 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/anomaly_detection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9294 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/anomaly_detection/defs.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/anomaly_detection/mutation.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/anomaly_detection/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.416538 dagster-plus-1.7.2rc1/dagster_plus/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19247 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/api/dagster_cloud_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.416538 dagster-plus-1.7.2rc1/dagster_plus/artifacts/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/artifacts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.416538 dagster-plus-1.7.2rc1/dagster_plus/auth/
+-rw-r--r--   0 root         (0) root         (0)      247 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/auth/constants.py
+-rw-r--r--   0 root         (0) root         (0)      455 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.416538 dagster-plus-1.7.2rc1/dagster_plus/dagster_insights/
+-rw-r--r--   0 root         (0) root         (0)     1873 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/dagster_insights/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.416538 dagster-plus-1.7.2rc1/dagster_plus/dagster_insights/bigquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/dagster_insights/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      816 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/dagster_insights/bigquery/bigquery_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7964 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/dagster_insights/bigquery/dbt_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     3233 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/dagster_insights/bigquery/insights_bigquery_resource.py
+-rw-r--r--   0 root         (0) root         (0)      138 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/dagster_insights/errors.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/dagster_insights/insights_utils.py
+-rw-r--r--   0 root         (0) root         (0)    10832 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/dagster_insights/metrics_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1403 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/dagster_insights/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.416538 dagster-plus-1.7.2rc1/dagster_plus/dagster_insights/snowflake/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/dagster_insights/snowflake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5611 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/dagster_insights/snowflake/dagster_snowflake_insights.py
+-rw-r--r--   0 root         (0) root         (0)     5185 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/dagster_insights/snowflake/dbt_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     7064 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/dagster_insights/snowflake/definitions.py
+-rw-r--r--   0 root         (0) root         (0)     9357 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/dagster_insights/snowflake/insights_snowflake_resource.py
+-rw-r--r--   0 root         (0) root         (0)     3807 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/dagster_insights/snowflake/snowflake_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.428538 dagster-plus-1.7.2rc1/dagster_plus/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.428538 dagster-plus-1.7.2rc1/dagster_plus/execution/cloud_run_launcher/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/execution/cloud_run_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/execution/cloud_run_launcher/k8s.py
+-rw-r--r--   0 root         (0) root         (0)     3096 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/execution/cloud_run_launcher/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.428538 dagster-plus-1.7.2rc1/dagster_plus/execution/monitoring/
+-rw-r--r--   0 root         (0) root         (0)    17254 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/execution/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.428538 dagster-plus-1.7.2rc1/dagster_plus/execution/utils/
+-rw-r--r--   0 root         (0) root         (0)      254 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/execution/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/execution/utils/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.428538 dagster-plus-1.7.2rc1/dagster_plus/instance/
+-rw-r--r--   0 root         (0) root         (0)    23058 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/instance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.428538 dagster-plus-1.7.2rc1/dagster_plus/metrics/
+-rw-r--r--   0 root         (0) root         (0)    10090 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/metrics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.428538 dagster-plus-1.7.2rc1/dagster_plus/pex/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/pex/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.428538 dagster-plus-1.7.2rc1/dagster_plus/pex/grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.444538 dagster-plus-1.7.2rc1/dagster_plus/pex/grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      285 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/pex/grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3907 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/pex/grpc/__generated__/multi_pex_api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9301 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      327 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/pex/grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5251 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/pex/grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     3790 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/pex/grpc/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.444538 dagster-plus-1.7.2rc1/dagster_plus/pex/grpc/server/
+-rw-r--r--   0 root         (0) root         (0)      119 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/pex/grpc/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.444538 dagster-plus-1.7.2rc1/dagster_plus/pex/grpc/server/cli/
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/pex/grpc/server/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17842 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/pex/grpc/server/manager.py
+-rw-r--r--   0 root         (0) root         (0)    12796 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/pex/grpc/server/registry.py
+-rw-r--r--   0 root         (0) root         (0)    15703 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/pex/grpc/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     3321 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/pex/grpc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.444538 dagster-plus-1.7.2rc1/dagster_plus/secrets/
+-rw-r--r--   0 root         (0) root         (0)       75 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.444538 dagster-plus-1.7.2rc1/dagster_plus/serverless/
+-rw-r--r--   0 root         (0) root         (0)       71 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/serverless/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4247 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/serverless/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.456538 dagster-plus-1.7.2rc1/dagster_plus/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1618 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/storage/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.456538 dagster-plus-1.7.2rc1/dagster_plus/storage/compute_logs/
+-rw-r--r--   0 root         (0) root         (0)       82 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/storage/compute_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4750 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/storage/compute_logs/compute_log_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.456538 dagster-plus-1.7.2rc1/dagster_plus/storage/event_logs/
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/storage/event_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16297 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/storage/event_logs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    46228 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/storage/event_logs/storage.py
+-rw-r--r--   0 root         (0) root         (0)      658 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/storage/event_logs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.464538 dagster-plus-1.7.2rc1/dagster_plus/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6446 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/storage/runs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    18838 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/storage/runs/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.464538 dagster-plus-1.7.2rc1/dagster_plus/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/storage/schedules/queries.py
+-rw-r--r--   0 root         (0) root         (0)     7574 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/storage/schedules/storage.py
+-rw-r--r--   0 root         (0) root         (0)      502 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/storage/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.464538 dagster-plus-1.7.2rc1/dagster_plus/util/
+-rw-r--r--   0 root         (0) root         (0)     2778 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/util/container_resources.py
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.464538 dagster-plus-1.7.2rc1/dagster_plus/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/workspace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.464538 dagster-plus-1.7.2rc1/dagster_plus/workspace/config_schema/
+-rw-r--r--   0 root         (0) root         (0)    10918 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/workspace/config_schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      967 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/workspace/config_schema/docker.py
+-rw-r--r--   0 root         (0) root         (0)     6575 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/workspace/config_schema/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     5319 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/workspace/config_schema/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.464538 dagster-plus-1.7.2rc1/dagster_plus/workspace/docker/
+-rw-r--r--   0 root         (0) root         (0)    12974 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/workspace/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      352 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/workspace/docker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.472538 dagster-plus-1.7.2rc1/dagster_plus/workspace/ecs/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/workspace/ecs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28817 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/workspace/ecs/client.py
+-rw-r--r--   0 root         (0) root         (0)    28613 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/workspace/ecs/launcher.py
+-rw-r--r--   0 root         (0) root         (0)      533 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/workspace/ecs/run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     4126 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/workspace/ecs/service.py
+-rw-r--r--   0 root         (0) root         (0)     2746 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/workspace/ecs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.472538 dagster-plus-1.7.2rc1/dagster_plus/workspace/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/workspace/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26243 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/workspace/kubernetes/launcher.py
+-rw-r--r--   0 root         (0) root         (0)     9824 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/workspace/kubernetes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.472538 dagster-plus-1.7.2rc1/dagster_plus/workspace/user_code_launcher/
+-rw-r--r--   0 root         (0) root         (0)      745 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/workspace/user_code_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14244 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/workspace/user_code_launcher/process.py
+-rw-r--r--   0 root         (0) root         (0)    83988 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/workspace/user_code_launcher/user_code_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/dagster_plus/workspace/user_code_launcher/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:11.408537 dagster-plus-1.7.2rc1/dagster_plus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4558 2024-04-16 18:02:11.000000 dagster-plus-1.7.2rc1/dagster_plus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4175 2024-04-16 18:02:11.000000 dagster-plus-1.7.2rc1/dagster_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 18:02:11.000000 dagster-plus-1.7.2rc1/dagster_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      529 2024-04-16 18:02:11.000000 dagster-plus-1.7.2rc1/dagster_plus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-16 18:02:11.000000 dagster-plus-1.7.2rc1/dagster_plus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 18:02:11.472538 dagster-plus-1.7.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3095 2024-04-16 17:50:53.000000 dagster-plus-1.7.2rc1/setup.py
```

