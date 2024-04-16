# Comparing `tmp/dagster-graphql-1.7.1.tar.gz` & `tmp/dagster-graphql-1.7.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-graphql-1.7.1.tar", last modified: Thu Apr 11 18:05:40 2024, max compression
+gzip compressed data, was "dagster-graphql-1.7.2rc1.tar", last modified: Tue Apr 16 17:51:26 2024, max compression
```

## Comparing `dagster-graphql-1.7.1.tar` & `dagster-graphql-1.7.2rc1.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:05:40.438583 dagster-graphql-1.7.1/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       49 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      691 2024-04-11 18:05:40.438583 dagster-graphql-1.7.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:05:40.414583 dagster-graphql-1.7.1/dagster_graphql/
--rw-r--r--   0 root         (0) root         (0)      641 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7401 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:05:40.418583 dagster-graphql-1.7.1/dagster_graphql/client/
--rw-r--r--   0 root         (0) root         (0)      482 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18338 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/client/client.py
--rw-r--r--   0 root         (0) root         (0)     2917 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/client/client_queries.py
--rw-r--r--   0 root         (0) root         (0)     6966 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/client/query.py
--rw-r--r--   0 root         (0) root         (0)     2917 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:05:40.422583 dagster-graphql-1.7.1/dagster_graphql/implementation/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12826 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/asset_checks_loader.py
--rw-r--r--   0 root         (0) root         (0)    20532 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:05:40.422583 dagster-graphql-1.7.1/dagster_graphql/implementation/execution/
--rw-r--r--   0 root         (0) root         (0)    14499 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12314 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     3727 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/execution/dynamic_partitions.py
--rw-r--r--   0 root         (0) root         (0)     4819 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/execution/launch_execution.py
--rw-r--r--   0 root         (0) root         (0)     4895 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/execution/run_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     7310 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/external.py
--rw-r--r--   0 root         (0) root         (0)     4251 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_asset_checks.py
--rw-r--r--   0 root         (0) root         (0)     4926 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_asset_condition_evaluations.py
--rw-r--r--   0 root         (0) root         (0)    28943 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_assets.py
--rw-r--r--   0 root         (0) root         (0)     3658 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
--rw-r--r--   0 root         (0) root         (0)     1237 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_backfills.py
--rw-r--r--   0 root         (0) root         (0)     1179 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_env_vars.py
--rw-r--r--   0 root         (0) root         (0)     3009 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_instigators.py
--rw-r--r--   0 root         (0) root         (0)      951 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_logs.py
--rw-r--r--   0 root         (0) root         (0)    12681 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_partition_sets.py
--rw-r--r--   0 root         (0) root         (0)     3726 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     2438 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_resources.py
--rw-r--r--   0 root         (0) root         (0)    15006 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_runs.py
--rw-r--r--   0 root         (0) root         (0)     9069 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_schedules.py
--rw-r--r--   0 root         (0) root         (0)    10352 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_sensors.py
--rw-r--r--   0 root         (0) root         (0)     2912 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_solids.py
--rw-r--r--   0 root         (0) root         (0)     2345 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_ticks.py
--rw-r--r--   0 root         (0) root         (0)    15798 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/loader.py
--rw-r--r--   0 root         (0) root         (0)     3097 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)      930 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     9774 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/implementation/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:05:40.430584 dagster-graphql-1.7.1/dagster_graphql/schema/
--rw-r--r--   0 root         (0) root         (0)     2877 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8533 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/asset_checks.py
--rw-r--r--   0 root         (0) root         (0)    11979 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/asset_condition_evaluations.py
--rw-r--r--   0 root         (0) root         (0)    54797 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)      385 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/asset_key.py
--rw-r--r--   0 root         (0) root         (0)     1606 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/asset_selections.py
--rw-r--r--   0 root         (0) root         (0)    10990 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/auto_materialize_asset_evaluations.py
--rw-r--r--   0 root         (0) root         (0)     2586 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    20849 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/backfill.py
--rw-r--r--   0 root         (0) root         (0)      627 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/config_type_or_error.py
--rw-r--r--   0 root         (0) root         (0)    15855 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/config_types.py
--rw-r--r--   0 root         (0) root         (0)     4823 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     1743 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/env_vars.py
--rw-r--r--   0 root         (0) root         (0)    17941 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/errors.py
--rw-r--r--   0 root         (0) root         (0)     5491 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/execution.py
--rw-r--r--   0 root         (0) root         (0)    18785 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/external.py
--rw-r--r--   0 root         (0) root         (0)     1769 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    13742 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/inputs.py
--rw-r--r--   0 root         (0) root         (0)    11731 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/instance.py
--rw-r--r--   0 root         (0) root         (0)    28766 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/instigation.py
--rw-r--r--   0 root         (0) root         (0)      232 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/instigators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:05:40.430584 dagster-graphql-1.7.1/dagster_graphql/schema/logs/
--rw-r--r--   0 root         (0) root         (0)     3632 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2868 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/logs/compute_logs.py
--rw-r--r--   0 root         (0) root         (0)    21701 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/logs/events.py
--rw-r--r--   0 root         (0) root         (0)      816 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/logs/log_level.py
--rw-r--r--   0 root         (0) root         (0)     5440 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/metadata.py
--rw-r--r--   0 root         (0) root         (0)      111 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/paging.py
--rw-r--r--   0 root         (0) root         (0)      529 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/partition_mappings.py
--rw-r--r--   0 root         (0) root         (0)    17797 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/partition_sets.py
--rw-r--r--   0 root         (0) root         (0)      748 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:05:40.434584 dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/
--rw-r--r--   0 root         (0) root         (0)     3263 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11060 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/config.py
--rw-r--r--   0 root         (0) root         (0)      582 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/config_result.py
--rw-r--r--   0 root         (0) root         (0)     1369 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/logger.py
--rw-r--r--   0 root         (0) root         (0)     1768 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/mode.py
--rw-r--r--   0 root         (0) root         (0)    40100 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/pipeline.py
--rw-r--r--   0 root         (0) root         (0)      855 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/pipeline_ref.py
--rw-r--r--   0 root         (0) root         (0)     2213 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/pipeline_run_stats.py
--rw-r--r--   0 root         (0) root         (0)     1496 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/resource.py
--rw-r--r--   0 root         (0) root         (0)     1263 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     1621 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/status.py
--rw-r--r--   0 root         (0) root         (0)      993 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/subscription.py
--rw-r--r--   0 root         (0) root         (0)     1654 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/repository_origin.py
--rw-r--r--   0 root         (0) root         (0)     9025 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:05:40.434584 dagster-graphql-1.7.1/dagster_graphql/schema/roots/
--rw-r--r--   0 root         (0) root         (0)     2094 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/roots/__init__.py
--rw-r--r--   0 root         (0) root         (0)      620 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/roots/assets.py
--rw-r--r--   0 root         (0) root         (0)      564 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/roots/execution_plan.py
--rw-r--r--   0 root         (0) root         (0)    32162 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/roots/mutation.py
--rw-r--r--   0 root         (0) root         (0)      723 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/roots/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    46505 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/roots/query.py
--rw-r--r--   0 root         (0) root         (0)     2905 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/roots/subscription.py
--rw-r--r--   0 root         (0) root         (0)     5092 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/run_config.py
--rw-r--r--   0 root         (0) root         (0)     6523 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/runs.py
--rw-r--r--   0 root         (0) root         (0)     1438 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/schedule_dry_run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:05:40.438583 dagster-graphql-1.7.1/dagster_graphql/schema/schedules/
--rw-r--r--   0 root         (0) root         (0)     4945 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9135 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/schedules/schedules.py
--rw-r--r--   0 root         (0) root         (0)     1833 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/schedules/ticks.py
--rw-r--r--   0 root         (0) root         (0)     1312 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/sensor_dry_run.py
--rw-r--r--   0 root         (0) root         (0)    10196 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/sensors.py
--rw-r--r--   0 root         (0) root         (0)    30059 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/solids.py
--rw-r--r--   0 root         (0) root         (0)     2390 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/table.py
--rw-r--r--   0 root         (0) root         (0)     1421 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/tags.py
--rw-r--r--   0 root         (0) root         (0)      574 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/test.py
--rw-r--r--   0 root         (0) root         (0)      744 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/used_solid.py
--rw-r--r--   0 root         (0) root         (0)      950 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/schema/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:05:40.438583 dagster-graphql-1.7.1/dagster_graphql/test/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7078 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/test/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/dagster_graphql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:05:40.414583 dagster-graphql-1.7.1/dagster_graphql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      691 2024-04-11 18:05:40.000000 dagster-graphql-1.7.1/dagster_graphql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4726 2024-04-11 18:05:40.000000 dagster-graphql-1.7.1/dagster_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:05:40.000000 dagster-graphql-1.7.1/dagster_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2024-04-11 18:05:40.000000 dagster-graphql-1.7.1/dagster_graphql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2024-04-11 18:05:40.000000 dagster-graphql-1.7.1/dagster_graphql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-11 18:05:40.000000 dagster-graphql-1.7.1/dagster_graphql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      180 2024-04-11 18:05:40.438583 dagster-graphql-1.7.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1531 2024-04-11 18:04:19.000000 dagster-graphql-1.7.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.807215 dagster-graphql-1.7.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       49 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      694 2024-04-16 17:51:26.807215 dagster-graphql-1.7.2rc1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.795215 dagster-graphql-1.7.2rc1/dagster_graphql/
+-rw-r--r--   0 root         (0) root         (0)      641 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7401 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.799214 dagster-graphql-1.7.2rc1/dagster_graphql/client/
+-rw-r--r--   0 root         (0) root         (0)      482 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18338 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/client/client_queries.py
+-rw-r--r--   0 root         (0) root         (0)     6966 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/client/query.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.799214 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12826 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/asset_checks_loader.py
+-rw-r--r--   0 root         (0) root         (0)    20532 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.799214 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/execution/
+-rw-r--r--   0 root         (0) root         (0)    14499 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12314 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/execution/dynamic_partitions.py
+-rw-r--r--   0 root         (0) root         (0)     4819 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/execution/launch_execution.py
+-rw-r--r--   0 root         (0) root         (0)     4895 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/execution/run_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     7310 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/external.py
+-rw-r--r--   0 root         (0) root         (0)     4251 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_asset_checks.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_asset_condition_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)    29108 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_assets.py
+-rw-r--r--   0 root         (0) root         (0)     3658 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_backfills.py
+-rw-r--r--   0 root         (0) root         (0)     1179 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_env_vars.py
+-rw-r--r--   0 root         (0) root         (0)     3009 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_instigators.py
+-rw-r--r--   0 root         (0) root         (0)      951 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_logs.py
+-rw-r--r--   0 root         (0) root         (0)    12681 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_resources.py
+-rw-r--r--   0 root         (0) root         (0)    15163 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_runs.py
+-rw-r--r--   0 root         (0) root         (0)     9069 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_schedules.py
+-rw-r--r--   0 root         (0) root         (0)    10352 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_sensors.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_solids.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_ticks.py
+-rw-r--r--   0 root         (0) root         (0)    14555 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/loader.py
+-rw-r--r--   0 root         (0) root         (0)     3097 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)      930 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     9774 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/implementation/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.807215 dagster-graphql-1.7.2rc1/dagster_graphql/schema/
+-rw-r--r--   0 root         (0) root         (0)     2877 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8533 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/asset_checks.py
+-rw-r--r--   0 root         (0) root         (0)    11979 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/asset_condition_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)    55049 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)      385 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/asset_selections.py
+-rw-r--r--   0 root         (0) root         (0)    10990 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)     2586 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    20849 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/backfill.py
+-rw-r--r--   0 root         (0) root         (0)      627 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/config_type_or_error.py
+-rw-r--r--   0 root         (0) root         (0)    15855 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     4823 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/env_vars.py
+-rw-r--r--   0 root         (0) root         (0)    17941 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5491 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/execution.py
+-rw-r--r--   0 root         (0) root         (0)    18785 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/external.py
+-rw-r--r--   0 root         (0) root         (0)     1769 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    13742 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/inputs.py
+-rw-r--r--   0 root         (0) root         (0)    11731 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/instance.py
+-rw-r--r--   0 root         (0) root         (0)    28766 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/instigation.py
+-rw-r--r--   0 root         (0) root         (0)      232 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/instigators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.807215 dagster-graphql-1.7.2rc1/dagster_graphql/schema/logs/
+-rw-r--r--   0 root         (0) root         (0)     3632 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/logs/compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)    21701 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/logs/events.py
+-rw-r--r--   0 root         (0) root         (0)      816 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/logs/log_level.py
+-rw-r--r--   0 root         (0) root         (0)     5440 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/metadata.py
+-rw-r--r--   0 root         (0) root         (0)      111 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/paging.py
+-rw-r--r--   0 root         (0) root         (0)      529 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/partition_mappings.py
+-rw-r--r--   0 root         (0) root         (0)    17797 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)      748 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.807215 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     3263 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11060 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/config.py
+-rw-r--r--   0 root         (0) root         (0)      582 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/config_result.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/mode.py
+-rw-r--r--   0 root         (0) root         (0)    40100 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      855 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/pipeline_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/pipeline_run_stats.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1263 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/status.py
+-rw-r--r--   0 root         (0) root         (0)      993 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/repository_origin.py
+-rw-r--r--   0 root         (0) root         (0)     9025 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.807215 dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/
+-rw-r--r--   0 root         (0) root         (0)     2094 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      620 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/assets.py
+-rw-r--r--   0 root         (0) root         (0)      564 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)    32162 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/mutation.py
+-rw-r--r--   0 root         (0) root         (0)      723 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    46584 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/query.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     5092 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     6523 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/runs.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/schedule_dry_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.807215 dagster-graphql-1.7.2rc1/dagster_graphql/schema/schedules/
+-rw-r--r--   0 root         (0) root         (0)     4945 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9135 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/schedules/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/schedules/ticks.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/sensor_dry_run.py
+-rw-r--r--   0 root         (0) root         (0)    10196 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/sensors.py
+-rw-r--r--   0 root         (0) root         (0)    30059 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/solids.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/table.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/tags.py
+-rw-r--r--   0 root         (0) root         (0)      574 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/test.py
+-rw-r--r--   0 root         (0) root         (0)      744 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/used_solid.py
+-rw-r--r--   0 root         (0) root         (0)      950 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/schema/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.807215 dagster-graphql-1.7.2rc1/dagster_graphql/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7078 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/test/utils.py
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/dagster_graphql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:51:26.799214 dagster-graphql-1.7.2rc1/dagster_graphql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      694 2024-04-16 17:51:26.000000 dagster-graphql-1.7.2rc1/dagster_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4726 2024-04-16 17:51:26.000000 dagster-graphql-1.7.2rc1/dagster_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:51:26.000000 dagster-graphql-1.7.2rc1/dagster_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2024-04-16 17:51:26.000000 dagster-graphql-1.7.2rc1/dagster_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2024-04-16 17:51:26.000000 dagster-graphql-1.7.2rc1/dagster_graphql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-16 17:51:26.000000 dagster-graphql-1.7.2rc1/dagster_graphql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2024-04-16 17:51:26.811215 dagster-graphql-1.7.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1534 2024-04-16 17:50:34.000000 dagster-graphql-1.7.2rc1/setup.py
```

### Comparing `dagster-graphql-1.7.1/LICENSE` & `dagster-graphql-1.7.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/PKG-INFO` & `dagster-graphql-1.7.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.7.1
+Version: 1.7.2rc1
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-graphql-1.7.1/dagster_graphql/__init__.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/cli.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/cli.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/client/client.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/client/client.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/client/client_queries.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/client/client_queries.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/client/query.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/client/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/client/utils.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/client/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/asset_checks_loader.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/asset_checks_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/events.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/execution/__init__.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/execution/backfill.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/execution/dynamic_partitions.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/execution/dynamic_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/execution/launch_execution.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/execution/launch_execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/execution/run_lifecycle.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/execution/run_lifecycle.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/external.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_asset_checks.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_asset_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_asset_condition_evaluations.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_asset_condition_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_assets.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from dagster._core.event_api import AssetRecordsFilter
 from dagster._core.events import ASSET_EVENTS
 from dagster._core.events.log import EventLogEntry
 from dagster._core.instance import DynamicPartitionsStore
 from dagster._core.remote_representation.code_location import CodeLocation
 from dagster._core.remote_representation.external import ExternalRepository
 from dagster._core.remote_representation.external_data import ExternalAssetNode
+from dagster._core.storage.event_log.base import AssetRecord
 from dagster._core.storage.event_log.sql_event_log import get_max_event_records_limit
 from dagster._core.storage.partition_status_cache import (
     build_failed_and_in_progress_partition_subset,
     get_and_update_asset_status_cache_value,
     get_materialized_multipartitions,
     get_validated_partition_keys,
     is_cacheable_partition_type,
@@ -412,27 +413,32 @@
     )
 
 
 def get_partition_subsets(
     instance: DagsterInstance,
     asset_key: AssetKey,
     dynamic_partitions_loader: DynamicPartitionsStore,
+    asset_record: Optional[AssetRecord],
     partitions_def: Optional[PartitionsDefinition] = None,
 ) -> Tuple[Optional[PartitionsSubset], Optional[PartitionsSubset], Optional[PartitionsSubset]]:
     """Returns a tuple of PartitionSubset objects: the first is the materialized partitions,
     the second is the failed partitions, and the third are in progress.
     """
     if not partitions_def:
         return None, None, None
 
     if instance.can_cache_asset_status_data() and is_cacheable_partition_type(partitions_def):
         # When the "cached_status_data" column exists in storage, update the column to contain
         # the latest partition status values
         updated_cache_value = get_and_update_asset_status_cache_value(
-            instance, asset_key, partitions_def, dynamic_partitions_loader
+            instance,
+            asset_key,
+            partitions_def,
+            dynamic_partitions_loader,
+            asset_record,
         )
         materialized_subset = (
             updated_cache_value.deserialize_materialized_partition_subsets(partitions_def)
             if updated_cache_value
             else partitions_def.empty_subset()
         )
         failed_subset = (
```

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_backfills.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_backfills.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_env_vars.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_instigators.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_instigators.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_logs.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_partition_sets.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_pipelines.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_pipelines.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_resources.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_runs.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_runs.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 from dagster._core.execution.stats import RunStepKeyStatsSnapshot, StepEventStatus
 from dagster._core.storage.dagster_run import DagsterRunStatus, RunRecord, RunsFilter
 from dagster._core.storage.tags import TagType, get_tag_type
 
 from .external import ensure_valid_config, get_external_job_or_raise
 
 if TYPE_CHECKING:
+    from dagster._core.workspace.batch_asset_record_loader import BatchAssetRecordLoader
+
     from ..schema.asset_graph import GrapheneAssetLatestInfo
     from ..schema.errors import GrapheneRunNotFoundError
     from ..schema.execution import GrapheneExecutionPlan
     from ..schema.logs.events import GrapheneRunStepStats
     from ..schema.pipelines.config import GraphenePipelineConfigValidationValid
     from ..schema.pipelines.pipeline import GrapheneEventConnection, GrapheneRun
     from ..schema.pipelines.pipeline_run_stats import GrapheneRunStatsSnapshot
@@ -154,15 +156,17 @@
 IN_PROGRESS_STATUSES = [
     DagsterRunStatus.STARTED,
     DagsterRunStatus.CANCELING,
 ]
 
 
 def get_assets_latest_info(
-    graphene_info: "ResolveInfo", step_keys_by_asset: Mapping[AssetKey, Sequence[str]]
+    graphene_info: "ResolveInfo",
+    step_keys_by_asset: Mapping[AssetKey, Sequence[str]],
+    asset_record_loader: "BatchAssetRecordLoader",
 ) -> Sequence["GrapheneAssetLatestInfo"]:
     from dagster_graphql.implementation.fetch_assets import get_asset_nodes_by_asset_key
 
     from ..schema.asset_graph import GrapheneAssetLatestInfo
     from ..schema.logs.events import GrapheneMaterializationEvent
     from ..schema.pipelines.pipeline import GrapheneRun
 
@@ -171,15 +175,15 @@
     asset_keys = list(step_keys_by_asset.keys())
 
     if not asset_keys:
         return []
 
     asset_nodes = get_asset_nodes_by_asset_key(graphene_info, asset_keys)
 
-    asset_records = instance.get_asset_records(asset_keys)
+    asset_records = asset_record_loader.get_asset_records(asset_keys)
 
     latest_materialization_by_asset = {
         asset_record.asset_entry.asset_key: (
             GrapheneMaterializationEvent(event=asset_record.asset_entry.last_materialization)
             if asset_record.asset_entry.last_materialization
             and asset_record.asset_entry.asset_key in step_keys_by_asset
             else None
```

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_schedules.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_sensors.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_solids.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/fetch_ticks.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/fetch_ticks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/loader.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from collections import defaultdict
 from enum import Enum
 from functools import lru_cache
-from typing import Any, Dict, Iterable, List, Mapping, Optional, Sequence, Set, Tuple
+from typing import Any, Dict, Iterable, List, Optional, Sequence, Set, Tuple
 
 from dagster import (
     DagsterInstance,
     _check as check,
 )
 from dagster._core.definitions.asset_spec import AssetExecutionType
 from dagster._core.definitions.data_version import CachingStaleStatusResolver
 from dagster._core.definitions.events import AssetKey
-from dagster._core.events.log import EventLogEntry
 from dagster._core.remote_representation import ExternalRepository
 from dagster._core.remote_representation.external_data import (
     ExternalAssetDependedBy,
     ExternalAssetDependency,
     ExternalAssetNode,
 )
 from dagster._core.scheduler.instigation import InstigatorState, InstigatorType
@@ -176,46 +175,14 @@
 
     def _fetch(self) -> None:
         records = self._instance.get_run_records(RunsFilter(run_ids=list(self._run_ids)))
         for record in records:
             self._records[record.dagster_run.run_id] = record
 
 
-class BatchMaterializationLoader:
-    """A batch loader that fetches materializations for asset keys.  This loader is expected to be
-    instantiated with a set of asset keys.
-    """
-
-    def __init__(self, instance: DagsterInstance, asset_keys: Iterable[AssetKey]):
-        self._instance = instance
-        self._asset_keys: List[AssetKey] = list(asset_keys)
-        self._fetched = False
-        self._materializations: Mapping[AssetKey, Optional[EventLogEntry]] = {}
-
-    def get_latest_materialization_for_asset_key(
-        self, asset_key: AssetKey
-    ) -> Optional[EventLogEntry]:
-        if asset_key not in self._asset_keys:
-            check.failed(
-                f"Asset key {asset_key} not recognized for this loader.  Expected one of:"
-                f" {self._asset_keys}"
-            )
-
-        if not self._fetched:
-            self._fetch()
-        return self._materializations.get(asset_key)
-
-    def _fetch(self) -> None:
-        self._fetched = True
-        self._materializations = {
-            record.asset_entry.asset_key: record.asset_entry.last_materialization
-            for record in self._instance.get_asset_records(self._asset_keys)
-        }
-
-
 class CrossRepoAssetDependedByLoader:
     """A batch loader that computes cross-repository asset dependencies. Locates source assets
     within all workspace repositories, and determines if they are derived (defined) assets in
     other repositories.
 
     For each asset that contains cross-repo dependencies (every asset that is defined as a source
     asset in another repository) a sink asset is any asset immediately downstream of the source
```

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/run_config_schema.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/telemetry.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/implementation/utils.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/implementation/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/__init__.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/asset_checks.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/asset_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/asset_condition_evaluations.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/asset_condition_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/asset_graph.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/asset_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     ExternalMultiPartitionsDefinitionData,
     ExternalPartitionsDefinitionData,
     ExternalStaticPartitionsDefinitionData,
     ExternalTimeWindowPartitionsDefinitionData,
 )
 from dagster._core.snap.node import GraphDefSnap, OpDefSnap
 from dagster._core.utils import is_valid_email
+from dagster._core.workspace.batch_asset_record_loader import BatchAssetRecordLoader
 from dagster._core.workspace.permissions import Permissions
 from dagster._utils.caching_instance_queryer import CachingInstanceQueryer
 
 from dagster_graphql.implementation.asset_checks_loader import AssetChecksLoader
 from dagster_graphql.implementation.events import iterate_metadata_entries
 from dagster_graphql.implementation.fetch_asset_checks import has_asset_checks
 from dagster_graphql.implementation.fetch_assets import (
@@ -65,15 +66,14 @@
 
 from ..implementation.fetch_assets import (
     build_partition_statuses,
     get_freshness_info,
     get_partition_subsets,
 )
 from ..implementation.loader import (
-    BatchMaterializationLoader,
     CrossRepoAssetDependedByLoader,
     StaleStatusLoader,
 )
 from ..schema.asset_checks import (
     AssetChecksOrErrorUnion,
     GrapheneAssetChecksOrError,
 )
@@ -160,30 +160,30 @@
     def __init__(
         self,
         repository_location: CodeLocation,
         external_repository: ExternalRepository,
         input_name: Optional[str],
         asset_key: AssetKey,
         asset_checks_loader: AssetChecksLoader,
-        materialization_loader: Optional[BatchMaterializationLoader] = None,
+        asset_record_loader: Optional[BatchAssetRecordLoader] = None,
         depended_by_loader: Optional[CrossRepoAssetDependedByLoader] = None,
         partition_mapping: Optional[PartitionMapping] = None,
     ):
         self._repository_location = check.inst_param(
             repository_location, "repository_location", CodeLocation
         )
         self._external_repository = check.inst_param(
             external_repository, "external_repository", ExternalRepository
         )
         self._asset_key = check.inst_param(asset_key, "asset_key", AssetKey)
         self._asset_checks_loader = check.inst_param(
             asset_checks_loader, "asset_checks_loader", AssetChecksLoader
         )
-        self._latest_materialization_loader = check.opt_inst_param(
-            materialization_loader, "materialization_loader", BatchMaterializationLoader
+        self._asset_record_loader = check.opt_inst_param(
+            asset_record_loader, "asset_record_loader", BatchAssetRecordLoader
         )
         self._depended_by_loader = check.opt_inst_param(
             depended_by_loader, "depended_by_loader", CrossRepoAssetDependedByLoader
         )
         self._partition_mapping = check.opt_inst_param(
             partition_mapping, "partition_mapping", PartitionMapping
         )
@@ -196,15 +196,15 @@
             asset_node = self._depended_by_loader.get_sink_asset(self._asset_key)
         asset_node = check.not_none(asset_node)
         return GrapheneAssetNode(
             self._repository_location,
             self._external_repository,
             asset_node,
             asset_checks_loader=self._asset_checks_loader,
-            materialization_loader=self._latest_materialization_loader,
+            asset_record_loader=self._asset_record_loader,
         )
 
     def resolve_partitionMapping(
         self, _graphene_info: ResolveInfo
     ) -> Optional[GraphenePartitionMapping]:
         if self._partition_mapping:
             return GraphenePartitionMapping(self._partition_mapping)
@@ -242,15 +242,15 @@
 
 class GrapheneAssetNode(graphene.ObjectType):
     _depended_by_loader: Optional[CrossRepoAssetDependedByLoader]
     _external_asset_node: ExternalAssetNode
     _node_definition_snap: Optional[Union[GraphDefSnap, OpDefSnap]]
     _external_job: Optional[ExternalJob]
     _external_repository: ExternalRepository
-    _latest_materialization_loader: Optional[BatchMaterializationLoader]
+    _asset_record_loader: Optional[BatchAssetRecordLoader]
     _stale_status_loader: Optional[StaleStatusLoader]
     _asset_checks_loader: AssetChecksLoader
     _asset_graph_differ: Optional[AssetGraphDiffer]
 
     # NOTE: properties/resolvers are listed alphabetically
     assetKey = graphene.NonNull(GrapheneAssetKey)
     assetMaterializations = graphene.Field(
@@ -348,15 +348,15 @@
 
     def __init__(
         self,
         repository_location: CodeLocation,
         external_repository: ExternalRepository,
         external_asset_node: ExternalAssetNode,
         asset_checks_loader: AssetChecksLoader,
-        materialization_loader: Optional[BatchMaterializationLoader] = None,
+        asset_record_loader: Optional[BatchAssetRecordLoader] = None,
         depended_by_loader: Optional[CrossRepoAssetDependedByLoader] = None,
         stale_status_loader: Optional[StaleStatusLoader] = None,
         dynamic_partitions_loader: Optional[CachingDynamicPartitionsLoader] = None,
         asset_graph_differ: Optional[AssetGraphDiffer] = None,
     ):
         from ..implementation.fetch_assets import get_unique_asset_id
 
@@ -367,16 +367,16 @@
         )
         self._external_repository = check.inst_param(
             external_repository, "external_repository", ExternalRepository
         )
         self._external_asset_node = check.inst_param(
             external_asset_node, "external_asset_node", ExternalAssetNode
         )
-        self._latest_materialization_loader = check.opt_inst_param(
-            materialization_loader, "materialization_loader", BatchMaterializationLoader
+        self._asset_record_loader = check.opt_inst_param(
+            asset_record_loader, "asset_record_loader", BatchAssetRecordLoader
         )
         self._depended_by_loader = check.opt_inst_param(
             depended_by_loader, "depended_by_loader", CrossRepoAssetDependedByLoader
         )
         self._stale_status_loader = check.opt_inst_param(
             stale_status_loader,
             "stale_status_loader",
@@ -616,22 +616,17 @@
         try:
             before_timestamp = (
                 int(beforeTimestampMillis) / 1000.0 if beforeTimestampMillis else None
             )
         except ValueError:
             before_timestamp = None
 
-        if (
-            self._latest_materialization_loader
-            and limit == 1
-            and not partitions
-            and not before_timestamp
-        ):
+        if self._asset_record_loader and limit == 1 and not partitions and not before_timestamp:
             latest_materialization_event = (
-                self._latest_materialization_loader.get_latest_materialization_for_asset_key(
+                self._asset_record_loader.get_latest_materialization_for_asset_key(
                     self._external_asset_node.asset_key
                 )
             )
 
             if not latest_materialization_event:
                 return []
 
@@ -802,15 +797,15 @@
             ),
             *self._external_asset_node.depended_by,
         ]
 
         if not depended_by_asset_nodes:
             return []
 
-        materialization_loader = BatchMaterializationLoader(
+        asset_record_loader = BatchAssetRecordLoader(
             instance=graphene_info.context.instance,
             asset_keys=[dep.downstream_asset_key for dep in depended_by_asset_nodes],
         )
         asset_checks_loader = AssetChecksLoader(
             context=graphene_info.context,
             asset_keys=[dep.downstream_asset_key for dep in depended_by_asset_nodes],
         )
@@ -818,15 +813,15 @@
         return [
             GrapheneAssetDependency(
                 repository_location=self._repository_location,
                 external_repository=self._external_repository,
                 input_name=dep.input_name,
                 asset_key=dep.downstream_asset_key,
                 asset_checks_loader=asset_checks_loader,
-                materialization_loader=materialization_loader,
+                asset_record_loader=asset_record_loader,
                 depended_by_loader=_depended_by_loader,
             )
             for dep in depended_by_asset_nodes
         ]
 
     def resolve_dependedByKeys(self, _graphene_info: ResolveInfo) -> Sequence[GrapheneAssetKey]:
         # CrossRepoAssetDependedByLoader class loads all cross-repo asset dependencies workspace-wide.
@@ -856,29 +851,29 @@
             for dep in self._external_asset_node.dependencies
         ]
 
     def resolve_dependencies(self, graphene_info: ResolveInfo) -> Sequence[GrapheneAssetDependency]:
         if not self._external_asset_node.dependencies:
             return []
 
-        materialization_loader = BatchMaterializationLoader(
+        asset_record_loader = BatchAssetRecordLoader(
             instance=graphene_info.context.instance,
             asset_keys=[dep.upstream_asset_key for dep in self._external_asset_node.dependencies],
         )
         asset_checks_loader = AssetChecksLoader(
             context=graphene_info.context,
             asset_keys=[dep.upstream_asset_key for dep in self._external_asset_node.dependencies],
         )
         return [
             GrapheneAssetDependency(
                 repository_location=self._repository_location,
                 external_repository=self._external_repository,
                 input_name=dep.input_name,
                 asset_key=dep.upstream_asset_key,
-                materialization_loader=materialization_loader,
+                asset_record_loader=asset_record_loader,
                 asset_checks_loader=asset_checks_loader,
                 partition_mapping=dep.partition_mapping,
             )
             for dep in self._external_asset_node.dependencies
         ]
 
     def resolve_freshnessInfo(
@@ -1117,14 +1112,19 @@
             materialized_partition_subset,
             failed_partition_subset,
             in_progress_subset,
         ) = get_partition_subsets(
             graphene_info.context.instance,
             asset_key,
             self._dynamic_partitions_loader,
+            (
+                self._asset_record_loader.get_asset_record(asset_key)
+                if self._asset_record_loader
+                else None
+            ),
             partitions_def,
         )
 
         return build_partition_statuses(
             self._dynamic_partitions_loader,
             materialized_partition_subset,
             failed_partition_subset,
@@ -1147,14 +1147,19 @@
                 failed_partition_subset,
                 in_progress_subset,
             ) = get_partition_subsets(
                 graphene_info.context.instance,
                 asset_key,
                 self._dynamic_partitions_loader,
                 (
+                    self._asset_record_loader.get_asset_record(self._external_asset_node.asset_key)
+                    if self._asset_record_loader
+                    else None
+                ),
+                (
                     self._external_asset_node.partitions_def_data.get_partitions_definition()
                     if self._external_asset_node.partitions_def_data
                     else None
                 ),
             )
 
             if (
```

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/asset_selections.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/asset_selections.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/auto_materialize_asset_evaluations.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/auto_materialize_asset_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/auto_materialize_policy.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/backfill.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/config_type_or_error.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/config_type_or_error.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/config_types.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/config_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/dagster_types.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/env_vars.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/errors.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/execution.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/external.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/freshness_policy.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/inputs.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/instance.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/instigation.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/logs/__init__.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/logs/compute_logs.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/logs/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/logs/events.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/logs/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/logs/log_level.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/logs/log_level.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/metadata.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/metadata.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/partition_mappings.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/partition_mappings.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/partition_sets.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/permissions.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/__init__.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/config.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/config_result.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/config_result.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/logger.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/mode.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/pipeline.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/pipeline_ref.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/pipeline_ref.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/pipeline_run_stats.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/pipeline_run_stats.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/resource.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/snapshot.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/status.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/status.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/pipelines/subscription.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/pipelines/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/repository_origin.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/repository_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/resources.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/roots/__init__.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/roots/assets.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/roots/execution_plan.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/roots/mutation.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/mutation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/roots/pipeline.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/roots/query.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,14 @@
     get_scheduler_or_error,
     get_schedules_or_error,
 )
 from ...implementation.fetch_sensors import get_sensor_or_error, get_sensors_or_error
 from ...implementation.fetch_solids import get_graph_or_error
 from ...implementation.fetch_ticks import get_instigation_ticks
 from ...implementation.loader import (
-    BatchMaterializationLoader,
     CrossRepoAssetDependedByLoader,
     StaleStatusLoader,
 )
 from ...implementation.run_config_schema import resolve_run_config_schema_or_error
 from ...implementation.utils import (
     capture_error,
     graph_selector_from_graphql,
@@ -935,18 +934,16 @@
             for node in results
             if use_all_asset_keys or node.assetKey in check.not_none(resolved_asset_keys)
         ]
 
         if not results:
             return []
 
-        materialization_loader = BatchMaterializationLoader(
-            instance=graphene_info.context.instance,
-            asset_keys=[node.assetKey for node in results],
-        )
+        asset_record_loader = graphene_info.context.asset_record_loader
+        asset_record_loader.add_asset_keys([node.assetKey for node in results])
         asset_checks_loader = AssetChecksLoader(
             context=graphene_info.context,
             asset_keys=[node.assetKey for node in results],
         )
 
         depended_by_loader = CrossRepoAssetDependedByLoader(context=graphene_info.context)
 
@@ -965,15 +962,15 @@
 
         nodes = [
             GrapheneAssetNode(
                 node.repository_location,
                 node.external_repository,
                 node.external_asset_node,
                 asset_checks_loader=asset_checks_loader,
-                materialization_loader=materialization_loader,
+                asset_record_loader=asset_record_loader,
                 depended_by_loader=depended_by_loader,
                 stale_status_loader=stale_status_loader,
                 dynamic_partitions_loader=dynamic_partitions_loader,
                 # base_deployment_context will be None if we are not in a branch deployment
                 asset_graph_differ=AssetGraphDiffer.from_external_repositories(
                     code_location_name=node.repository_location.name,
                     repository_name=node.external_repository.name,
@@ -1071,15 +1068,18 @@
         # Build mapping of asset key to the step keys required to generate the asset
         step_keys_by_asset: Dict[AssetKey, Sequence[str]] = {
             node.external_asset_node.asset_key: node.external_asset_node.op_names
             for node in results
             if node.assetKey in asset_keys
         }
 
-        return get_assets_latest_info(graphene_info, step_keys_by_asset)
+        asset_record_loader = graphene_info.context.asset_record_loader
+        asset_record_loader.add_asset_keys(asset_keys)
+
+        return get_assets_latest_info(graphene_info, step_keys_by_asset, asset_record_loader)
 
     @capture_error
     def resolve_logsForRun(
         self,
         graphene_info: ResolveInfo,
         runId: str,
         afterCursor: Optional[str] = None,
```

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/roots/subscription.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/roots/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/run_config.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/runs.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/schedule_dry_run.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/schedule_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/schedules/__init__.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/schedules/schedules.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/schedules/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/schedules/ticks.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/schedules/ticks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/sensor_dry_run.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/sensor_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/sensors.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/solids.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/table.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/table.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/tags.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/test.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/test.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/used_solid.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/used_solid.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/schema/util.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/schema/util.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql/test/utils.py` & `dagster-graphql-1.7.2rc1/dagster_graphql/test/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/dagster_graphql.egg-info/PKG-INFO` & `dagster-graphql-1.7.2rc1/dagster_graphql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.7.1
+Version: 1.7.2rc1
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-graphql-1.7.1/dagster_graphql.egg-info/SOURCES.txt` & `dagster-graphql-1.7.2rc1/dagster_graphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.1/setup.py` & `dagster-graphql-1.7.2rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_graphql_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.1",
+        "dagster==1.7.2rc1",
         "graphene>=3,<4",
         "gql[requests]>=3,<4",
         "requests",
         "starlette",  # used for run_in_threadpool utility fn
     ],
     entry_points={"console_scripts": ["dagster-graphql = dagster_graphql.cli:main"]},
 )
```

