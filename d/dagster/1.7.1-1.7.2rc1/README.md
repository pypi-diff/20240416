# Comparing `tmp/dagster-1.7.1.tar.gz` & `tmp/dagster-1.7.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-1.7.1.tar", last modified: Thu Apr 11 18:04:47 2024, max compression
+gzip compressed data, was "dagster-1.7.2rc1.tar", last modified: Tue Apr 16 17:50:58 2024, max compression
```

## Comparing `dagster-1.7.1.tar` & `dagster-1.7.2rc1.tar`

### file list

```diff
@@ -1,692 +1,693 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.426220 dagster-1.7.1/
--rw-r--r--   0 root         (0) root         (0)      553 2024-04-11 18:04:20.000000 dagster-1.7.1/COPYING
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-11 18:04:20.000000 dagster-1.7.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      533 2024-04-11 18:04:20.000000 dagster-1.7.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8928 2024-04-11 18:04:47.426220 dagster-1.7.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7214 2024-04-11 18:04:20.000000 dagster-1.7.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.310219 dagster-1.7.1/dagster/
--rw-r--r--   0 root         (0) root         (0)    29822 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/__main__.py
--rw-r--r--   0 root         (0) root         (0)    20744 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.314219 dagster-1.7.1/dagster/_api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      731 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_api/get_server_id.py
--rw-r--r--   0 root         (0) root         (0)     2147 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_api/list_repositories.py
--rw-r--r--   0 root         (0) root         (0)      531 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_api/notebook_data.py
--rw-r--r--   0 root         (0) root         (0)     3224 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_api/snapshot_execution_plan.py
--rw-r--r--   0 root         (0) root         (0)     1964 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_api/snapshot_job.py
--rw-r--r--   0 root         (0) root         (0)     5483 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_api/snapshot_partition.py
--rw-r--r--   0 root         (0) root         (0)     1670 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_api/snapshot_repository.py
--rw-r--r--   0 root         (0) root         (0)     3021 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_api/snapshot_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3370 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_api/snapshot_sensor.py
--rw-r--r--   0 root         (0) root         (0)      478 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_builtins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.314219 dagster-1.7.1/dagster/_check/
--rw-r--r--   0 root         (0) root         (0)     1352 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_check/README.md
--rw-r--r--   0 root         (0) root         (0)    52040 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_check/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.314219 dagster-1.7.1/dagster/_cli/
--rw-r--r--   0 root         (0) root         (0)     1182 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26898 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/api.py
--rw-r--r--   0 root         (0) root         (0)     8030 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/asset.py
--rw-r--r--   0 root         (0) root         (0)     8302 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/code_server.py
--rw-r--r--   0 root         (0) root         (0)     2374 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/config_scaffolder.py
--rw-r--r--   0 root         (0) root         (0)     3513 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/debug.py
--rw-r--r--   0 root         (0) root         (0)     8134 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/dev.py
--rw-r--r--   0 root         (0) root         (0)     6651 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/instance.py
--rw-r--r--   0 root         (0) root         (0)    30542 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/job.py
--rw-r--r--   0 root         (0) root         (0)     1695 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/load_handle.py
--rw-r--r--   0 root         (0) root         (0)     9114 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/project.py
--rw-r--r--   0 root         (0) root         (0)     5120 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/run.py
--rw-r--r--   0 root         (0) root         (0)    19351 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/schedule.py
--rw-r--r--   0 root         (0) root         (0)    15461 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/sensor.py
--rw-r--r--   0 root         (0) root         (0)     4259 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.314219 dagster-1.7.1/dagster/_cli/workspace/
--rw-r--r--   0 root         (0) root         (0)      180 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27910 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/workspace/cli_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.318220 dagster-1.7.1/dagster/_config/
--rw-r--r--   0 root         (0) root         (0)     3186 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3403 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    15830 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/config_type.py
--rw-r--r--   0 root         (0) root         (0)    18787 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/errors.py
--rw-r--r--   0 root         (0) root         (0)     1783 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/evaluate_value_result.py
--rw-r--r--   0 root         (0) root         (0)    14918 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/field.py
--rw-r--r--   0 root         (0) root         (0)    19728 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/field_utils.py
--rw-r--r--   0 root         (0) root         (0)     9536 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/post_process.py
--rw-r--r--   0 root         (0) root         (0)      855 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/primitive_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.322219 dagster-1.7.1/dagster/_config/pythonic_config/
--rw-r--r--   0 root         (0) root         (0)     1394 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/pythonic_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/pythonic_config/attach_other_object_to_context.py
--rw-r--r--   0 root         (0) root         (0)    18042 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/pythonic_config/config.py
--rw-r--r--   0 root         (0) root         (0)    11496 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/pythonic_config/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    11583 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/pythonic_config/io_manager.py
--rw-r--r--   0 root         (0) root         (0)     4022 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/pythonic_config/pydantic_compat_layer.py
--rw-r--r--   0 root         (0) root         (0)    41251 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/pythonic_config/resource.py
--rw-r--r--   0 root         (0) root         (0)     1996 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/pythonic_config/type_check_utils.py
--rw-r--r--   0 root         (0) root         (0)     8375 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/pythonic_config/typing_utils.py
--rw-r--r--   0 root         (0) root         (0)    12532 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/snap.py
--rw-r--r--   0 root         (0) root         (0)     3087 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/source.py
--rw-r--r--   0 root         (0) root         (0)     3528 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/stack.py
--rw-r--r--   0 root         (0) root         (0)     7772 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/traversal_context.py
--rw-r--r--   0 root         (0) root         (0)     4167 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/type_printer.py
--rw-r--r--   0 root         (0) root         (0)    17137 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.326219 dagster-1.7.1/dagster/_core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.326219 dagster-1.7.1/dagster/_core/asset_graph_view/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/asset_graph_view/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21047 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/asset_graph_view/asset_graph_view.py
--rw-r--r--   0 root         (0) root         (0)      994 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/assets.py
--rw-r--r--   0 root         (0) root         (0)    13427 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/code_pointer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.326219 dagster-1.7.1/dagster/_core/container_context/
--rw-r--r--   0 root         (0) root         (0)      184 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/container_context/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1278 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/container_context/config.py
--rw-r--r--   0 root         (0) root         (0)     2310 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/debug.py
--rw-r--r--   0 root         (0) root         (0)     9665 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/decorator_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.338220 dagster-1.7.1/dagster/_core/definitions/
--rw-r--r--   0 root         (0) root         (0)     7827 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4506 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_check_evaluation.py
--rw-r--r--   0 root         (0) root         (0)     7409 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_check_result.py
--rw-r--r--   0 root         (0) root         (0)     5416 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_check_spec.py
--rw-r--r--   0 root         (0) root         (0)     6073 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.338220 dagster-1.7.1/dagster/_core/definitions/asset_condition/
--rw-r--r--   0 root         (0) root         (0)       62 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_condition/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21008 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_condition/asset_condition.py
--rw-r--r--   0 root         (0) root         (0)    16484 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_condition/asset_condition_evaluation_context.py
--rw-r--r--   0 root         (0) root         (0)    26160 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_daemon_context.py
--rw-r--r--   0 root         (0) root         (0)    10572 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)     4628 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_dep.py
--rw-r--r--   0 root         (0) root         (0)    10251 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)     7621 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_graph_differ.py
--rw-r--r--   0 root         (0) root         (0)    16483 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_graph_subset.py
--rw-r--r--   0 root         (0) root         (0)     3644 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_in.py
--rw-r--r--   0 root         (0) root         (0)    29917 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_job.py
--rw-r--r--   0 root         (0) root         (0)     6060 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_key.py
--rw-r--r--   0 root         (0) root         (0)    30355 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_layer.py
--rw-r--r--   0 root         (0) root         (0)     6945 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_out.py
--rw-r--r--   0 root         (0) root         (0)    39535 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_selection.py
--rw-r--r--   0 root         (0) root         (0)     7444 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)     6764 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_spec.py
--rw-r--r--   0 root         (0) root         (0)     9802 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_subset.py
--rw-r--r--   0 root         (0) root         (0)    79547 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/assets.py
--rw-r--r--   0 root         (0) root         (0)    13880 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    54395 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/auto_materialize_rule.py
--rw-r--r--   0 root         (0) root         (0)    21660 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/auto_materialize_rule_evaluation.py
--rw-r--r--   0 root         (0) root         (0)     2768 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/auto_materialize_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)     2939 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/backfill_policy.py
--rw-r--r--   0 root         (0) root         (0)    34626 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/base_asset_graph.py
--rw-r--r--   0 root         (0) root         (0)    16772 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/cacheable_assets.py
--rw-r--r--   0 root         (0) root         (0)    40623 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/composition.py
--rw-r--r--   0 root         (0) root         (0)     4278 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/config.py
--rw-r--r--   0 root         (0) root         (0)    14811 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/configurable.py
--rw-r--r--   0 root         (0) root         (0)    22990 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/data_time.py
--rw-r--r--   0 root         (0) root         (0)    30060 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/data_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.342220 dagster-1.7.1/dagster/_core/definitions/decorators/
--rw-r--r--   0 root         (0) root         (0)      620 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16572 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/asset_check_decorator.py
--rw-r--r--   0 root         (0) root         (0)    69203 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4907 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/config_mapping_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9077 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/graph_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9353 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/hook_decorator.py
--rw-r--r--   0 root         (0) root         (0)    10815 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/job_decorator.py
--rw-r--r--   0 root         (0) root         (0)    19011 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/op_decorator.py
--rw-r--r--   0 root         (0) root         (0)    15668 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/repository_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8718 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/schedule_decorator.py
--rw-r--r--   0 root         (0) root         (0)    12463 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/sensor_decorator.py
--rw-r--r--   0 root         (0) root         (0)    12664 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/source_asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     5267 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/definition_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    23545 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/definitions_class.py
--rw-r--r--   0 root         (0) root         (0)    42247 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/dependency.py
--rw-r--r--   0 root         (0) root         (0)    26888 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/events.py
--rw-r--r--   0 root         (0) root         (0)    21182 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/executor_definition.py
--rw-r--r--   0 root         (0) root         (0)     9379 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/external_asset.py
--rw-r--r--   0 root         (0) root         (0)     9750 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/freshness_based_auto_materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.342220 dagster-1.7.1/dagster/_core/definitions/freshness_checks/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/freshness_checks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5838 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/freshness_checks/last_update.py
--rw-r--r--   0 root         (0) root         (0)     7677 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/freshness_checks/sensor.py
--rw-r--r--   0 root         (0) root         (0)     7938 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/freshness_checks/shared_builder.py
--rw-r--r--   0 root         (0) root         (0)     4669 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/freshness_checks/time_partition.py
--rw-r--r--   0 root         (0) root         (0)    10573 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/freshness_checks/utils.py
--rw-r--r--   0 root         (0) root         (0)     8801 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    16401 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/freshness_policy_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    47569 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/graph_definition.py
--rw-r--r--   0 root         (0) root         (0)     6546 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/hook_definition.py
--rw-r--r--   0 root         (0) root         (0)     1524 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/hook_invocation.py
--rw-r--r--   0 root         (0) root         (0)     3537 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/inference.py
--rw-r--r--   0 root         (0) root         (0)    21027 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/input.py
--rw-r--r--   0 root         (0) root         (0)     6410 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/instigation_logger.py
--rw-r--r--   0 root         (0) root         (0)     2991 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/job_base.py
--rw-r--r--   0 root         (0) root         (0)    53689 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/job_definition.py
--rw-r--r--   0 root         (0) root         (0)     5693 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/load_asset_checks_from_modules.py
--rw-r--r--   0 root         (0) root         (0)    22306 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/load_assets_from_modules.py
--rw-r--r--   0 root         (0) root         (0)     7171 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/logger_definition.py
--rw-r--r--   0 root         (0) root         (0)      636 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/logger_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8959 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.342220 dagster-1.7.1/dagster/_core/definitions/metadata/
--rw-r--r--   0 root         (0) root         (0)    42305 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10371 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/metadata/table.py
--rw-r--r--   0 root         (0) root         (0)    57203 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/multi_asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    22029 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/multi_dimensional_partitions.py
--rw-r--r--   0 root         (0) root         (0)      197 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/no_step_launcher.py
--rw-r--r--   0 root         (0) root         (0)    11892 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/node_container.py
--rw-r--r--   0 root         (0) root         (0)     8016 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/node_definition.py
--rw-r--r--   0 root         (0) root         (0)     2892 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/observe.py
--rw-r--r--   0 root         (0) root         (0)    23078 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/op_definition.py
--rw-r--r--   0 root         (0) root         (0)    22439 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/op_invocation.py
--rw-r--r--   0 root         (0) root         (0)     7551 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/op_selection.py
--rw-r--r--   0 root         (0) root         (0)    19237 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/output.py
--rw-r--r--   0 root         (0) root         (0)    50520 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/partition.py
--rw-r--r--   0 root         (0) root         (0)      630 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/partition_key_range.py
--rw-r--r--   0 root         (0) root         (0)    47665 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)    11087 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/partitioned_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3779 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/policy.py
--rw-r--r--   0 root         (0) root         (0)    27737 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/reconstruct.py
--rw-r--r--   0 root         (0) root         (0)    21602 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/remote_asset_graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.342220 dagster-1.7.1/dagster/_core/definitions/repository_definition/
--rw-r--r--   0 root         (0) root         (0)      654 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/repository_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6024 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/repository_definition/caching_index.py
--rw-r--r--   0 root         (0) root         (0)    21698 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/repository_definition/repository_data.py
--rw-r--r--   0 root         (0) root         (0)    20892 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/repository_definition/repository_data_builder.py
--rw-r--r--   0 root         (0) root         (0)    20432 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/repository_definition/repository_definition.py
--rw-r--r--   0 root         (0) root         (0)     1479 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/repository_definition/valid_definitions.py
--rw-r--r--   0 root         (0) root         (0)     8858 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/resolved_asset_deps.py
--rw-r--r--   0 root         (0) root         (0)     1465 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/resource_annotation.py
--rw-r--r--   0 root         (0) root         (0)    17900 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/resource_definition.py
--rw-r--r--   0 root         (0) root         (0)     5382 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/resource_invocation.py
--rw-r--r--   0 root         (0) root         (0)    10320 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/resource_requirement.py
--rw-r--r--   0 root         (0) root         (0)     3383 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/result.py
--rw-r--r--   0 root         (0) root         (0)    23076 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/run_config.py
--rw-r--r--   0 root         (0) root         (0)     1445 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    19555 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/run_request.py
--rw-r--r--   0 root         (0) root         (0)    44126 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/run_status_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    39363 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     6225 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/schema_change_checks.py
--rw-r--r--   0 root         (0) root         (0)     5134 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/scoped_resources_builder.py
--rw-r--r--   0 root         (0) root         (0)    14134 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/selector.py
--rw-r--r--   0 root         (0) root         (0)    53797 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    19244 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/source_asset.py
--rw-r--r--   0 root         (0) root         (0)     2481 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/step_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1530 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/target.py
--rw-r--r--   0 root         (0) root         (0)    21859 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/time_window_partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)   102142 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/time_window_partitions.py
--rw-r--r--   0 root         (0) root         (0)    15160 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/unresolved_asset_job_definition.py
--rw-r--r--   0 root         (0) root         (0)    11017 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/utils.py
--rw-r--r--   0 root         (0) root         (0)     3982 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/version_strategy.py
--rw-r--r--   0 root         (0) root         (0)    26986 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/errors.py
--rw-r--r--   0 root         (0) root         (0)    18062 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/event_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.342220 dagster-1.7.1/dagster/_core/events/
--rw-r--r--   0 root         (0) root         (0)    71913 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7635 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/events/log.py
--rw-r--r--   0 root         (0) root         (0)     1614 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/events/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.350220 dagster-1.7.1/dagster/_core/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38363 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/api.py
--rw-r--r--   0 root         (0) root         (0)    64654 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/asset_backfill.py
--rw-r--r--   0 root         (0) root         (0)    17100 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     6296 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/build_resources.py
--rw-r--r--   0 root         (0) root         (0)      224 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/bulk_actions.py
--rw-r--r--   0 root         (0) root         (0)     5587 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/compute_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.354220 dagster-1.7.1/dagster/_core/execution/context/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/context/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79687 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/context/compute.py
--rw-r--r--   0 root         (0) root         (0)    17598 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/context/hook.py
--rw-r--r--   0 root         (0) root         (0)     9613 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/context/init.py
--rw-r--r--   0 root         (0) root         (0)    29167 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/context/input.py
--rw-r--r--   0 root         (0) root         (0)    40124 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/context/invocation.py
--rw-r--r--   0 root         (0) root         (0)     3164 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/context/logger.py
--rw-r--r--   0 root         (0) root         (0)    37256 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/context/output.py
--rw-r--r--   0 root         (0) root         (0)    56002 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/context/system.py
--rw-r--r--   0 root         (0) root         (0)    18837 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/context_creation_job.py
--rw-r--r--   0 root         (0) root         (0)     5135 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/execute_in_process.py
--rw-r--r--   0 root         (0) root         (0)     5897 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/execute_in_process_result.py
--rw-r--r--   0 root         (0) root         (0)     9633 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/execution_result.py
--rw-r--r--   0 root         (0) root         (0)     8602 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/host_mode.py
--rw-r--r--   0 root         (0) root         (0)    14247 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/job_backfill.py
--rw-r--r--   0 root         (0) root         (0)     6723 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/job_execution_result.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/memoization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.358220 dagster-1.7.1/dagster/_core/execution/plan/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26460 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/active.py
--rw-r--r--   0 root         (0) root         (0)     9850 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/compute.py
--rw-r--r--   0 root         (0) root         (0)    16535 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/compute_generator.py
--rw-r--r--   0 root         (0) root         (0)    16974 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/execute_plan.py
--rw-r--r--   0 root         (0) root         (0)    40549 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/execute_step.py
--rw-r--r--   0 root         (0) root         (0)    11036 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/external_step.py
--rw-r--r--   0 root         (0) root         (0)     3664 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/handle.py
--rw-r--r--   0 root         (0) root         (0)    39260 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/inputs.py
--rw-r--r--   0 root         (0) root         (0)     6251 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/instance_concurrency_context.py
--rw-r--r--   0 root         (0) root         (0)     1197 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/local_external_step_main.py
--rw-r--r--   0 root         (0) root         (0)     5706 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/objects.py
--rw-r--r--   0 root         (0) root         (0)     7326 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/outputs.py
--rw-r--r--   0 root         (0) root         (0)    61075 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/plan.py
--rw-r--r--   0 root         (0) root         (0)      114 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/resume_retry.py
--rw-r--r--   0 root         (0) root         (0)    17174 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/state.py
--rw-r--r--   0 root         (0) root         (0)    15985 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/step.py
--rw-r--r--   0 root         (0) root         (0)     3796 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/utils.py
--rw-r--r--   0 root         (0) root         (0)     1762 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/poll_compute_logs.py
--rw-r--r--   0 root         (0) root         (0)     8230 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/resolve_versions.py
--rw-r--r--   0 root         (0) root         (0)    19141 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/resources_init.py
--rw-r--r--   0 root         (0) root         (0)     2100 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/retries.py
--rw-r--r--   0 root         (0) root         (0)     1564 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/run_cancellation_thread.py
--rw-r--r--   0 root         (0) root         (0)     9950 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/stats.py
--rw-r--r--   0 root         (0) root         (0)    14043 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/submit_asset_runs.py
--rw-r--r--   0 root         (0) root         (0)     1125 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/tags.py
--rw-r--r--   0 root         (0) root         (0)     1172 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/validate_run_config.py
--rw-r--r--   0 root         (0) root         (0)     1282 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/watch_orphans.py
--rw-r--r--   0 root         (0) root         (0)     4311 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/with_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.358220 dagster-1.7.1/dagster/_core/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/executor/base.py
--rw-r--r--   0 root         (0) root         (0)     5989 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/executor/child_process_executor.py
--rw-r--r--   0 root         (0) root         (0)     3366 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/executor/in_process.py
--rw-r--r--   0 root         (0) root         (0)     1509 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/executor/init.py
--rw-r--r--   0 root         (0) root         (0)    15497 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/executor/multiprocess.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.358220 dagster-1.7.1/dagster/_core/executor/step_delegating/
--rw-r--r--   0 root         (0) root         (0)      247 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/executor/step_delegating/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16894 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/executor/step_delegating/step_delegating_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.358220 dagster-1.7.1/dagster/_core/executor/step_delegating/step_handler/
--rw-r--r--   0 root         (0) root         (0)      152 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/executor/step_delegating/step_handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3078 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/executor/step_delegating/step_handler/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.362220 dagster-1.7.1/dagster/_core/instance/
--rw-r--r--   0 root         (0) root         (0)   131945 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/instance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15788 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/instance/config.py
--rw-r--r--   0 root         (0) root         (0)    24141 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/instance/ref.py
--rw-r--r--   0 root         (0) root         (0)     3899 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/instance_for_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.362220 dagster-1.7.1/dagster/_core/launcher/
--rw-r--r--   0 root         (0) root         (0)      297 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3819 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/launcher/base.py
--rw-r--r--   0 root         (0) root         (0)     6645 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/launcher/default_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1566 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/launcher/sync_in_memory_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)      473 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/libraries.py
--rw-r--r--   0 root         (0) root         (0)    18041 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1029 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/nux.py
--rw-r--r--   0 root         (0) root         (0)     5736 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/op_concurrency_limits_counter.py
--rw-r--r--   0 root         (0) root         (0)     3691 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.362220 dagster-1.7.1/dagster/_core/pipes/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/pipes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8974 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/pipes/client.py
--rw-r--r--   0 root         (0) root         (0)    18318 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/pipes/context.py
--rw-r--r--   0 root         (0) root         (0)     5648 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/pipes/subprocess.py
--rw-r--r--   0 root         (0) root         (0)    25661 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/pipes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.366220 dagster-1.7.1/dagster/_core/remote_representation/
--rw-r--r--   0 root         (0) root         (0)     2793 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36695 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/code_location.py
--rw-r--r--   0 root         (0) root         (0)    37482 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/external.py
--rw-r--r--   0 root         (0) root         (0)    83392 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/external_data.py
--rw-r--r--   0 root         (0) root         (0)     1450 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/feature_flags.py
--rw-r--r--   0 root         (0) root         (0)    12429 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/grpc_server_registry.py
--rw-r--r--   0 root         (0) root         (0)     1487 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/grpc_server_state_subscriber.py
--rw-r--r--   0 root         (0) root         (0)     4356 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/handle.py
--rw-r--r--   0 root         (0) root         (0)     1581 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/historical.py
--rw-r--r--   0 root         (0) root         (0)     4850 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/job_index.py
--rw-r--r--   0 root         (0) root         (0)    19669 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/origin.py
--rw-r--r--   0 root         (0) root         (0)     3602 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/represented.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.366220 dagster-1.7.1/dagster/_core/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      267 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2005 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/run_coordinator/base.py
--rw-r--r--   0 root         (0) root         (0)     1922 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/run_coordinator/default_run_coordinator.py
--rw-r--r--   0 root         (0) root         (0)    13364 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/run_coordinator/queued_run_coordinator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.366220 dagster-1.7.1/dagster/_core/scheduler/
--rw-r--r--   0 root         (0) root         (0)      534 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1241 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/scheduler/execution.py
--rw-r--r--   0 root         (0) root         (0)    28809 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/scheduler/instigation.py
--rw-r--r--   0 root         (0) root         (0)    10931 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.366220 dagster-1.7.1/dagster/_core/secrets/
--rw-r--r--   0 root         (0) root         (0)       51 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1801 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/secrets/env_file.py
--rw-r--r--   0 root         (0) root         (0)      388 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.366220 dagster-1.7.1/dagster/_core/selector/
--rw-r--r--   0 root         (0) root         (0)      295 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/selector/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18109 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/selector/subset_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.370220 dagster-1.7.1/dagster/_core/snap/
--rw-r--r--   0 root         (0) root         (0)     2842 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/snap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      494 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/snap/config_types.py
--rw-r--r--   0 root         (0) root         (0)     3999 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/snap/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     9302 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/snap/dep_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    12155 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/snap/execution_plan_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    16934 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/snap/job_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4561 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/snap/mode.py
--rw-r--r--   0 root         (0) root         (0)    14185 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/snap/node.py
--rw-r--r--   0 root         (0) root         (0)     3183 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/snap/snap_to_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.374220 dagster-1.7.1/dagster/_core/storage/
--rw-r--r--   0 root         (0) root         (0)     3058 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/DEVELOPING.md
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.374220 dagster-1.7.1/dagster/_core/storage/alembic/
--rw-r--r--   0 root         (0) root         (0)     6686 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/README.md
--rw-r--r--   0 root         (0) root         (0)      687 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      494 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.390220 dagster-1.7.1/dagster/_core/storage/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     3150 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/001_initial_1.py
--rw-r--r--   0 root         (0) root         (0)      312 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/001_initial_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1486 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
--rw-r--r--   0 root         (0) root         (0)      599 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     2729 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
--rw-r--r--   0 root         (0) root         (0)      953 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      953 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      956 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      956 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1171 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1171 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1125 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      432 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      432 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     3927 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
--rw-r--r--   0 root         (0) root         (0)     3927 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      325 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/017_initial_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      531 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      635 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1893 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
--rw-r--r--   0 root         (0) root         (0)      958 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
--rw-r--r--   0 root         (0) root         (0)      499 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
--rw-r--r--   0 root         (0) root         (0)     1951 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
--rw-r--r--   0 root         (0) root         (0)      428 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
--rw-r--r--   0 root         (0) root         (0)      427 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
--rw-r--r--   0 root         (0) root         (0)     1537 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
--rw-r--r--   0 root         (0) root         (0)     2481 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
--rw-r--r--   0 root         (0) root         (0)     1177 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
--rw-r--r--   0 root         (0) root         (0)     2062 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
--rw-r--r--   0 root         (0) root         (0)     2359 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
--rw-r--r--   0 root         (0) root         (0)     2898 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py
--rw-r--r--   0 root         (0) root         (0)     1322 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3887 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/asset_check_execution_record.py
--rw-r--r--   0 root         (0) root         (0)     7301 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/asset_value_loader.py
--rw-r--r--   0 root         (0) root         (0)     1227 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/base_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.390220 dagster-1.7.1/dagster/_core/storage/branching/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/branching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5579 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/branching/branching_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8725 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/captured_log_manager.py
--rw-r--r--   0 root         (0) root         (0)    16223 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/cloud_storage_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     9557 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1863 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/config.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)    25656 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/dagster_run.py
--rw-r--r--   0 root         (0) root         (0)    11187 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/db_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.394220 dagster-1.7.1/dagster/_core/storage/event_log/
--rw-r--r--   0 root         (0) root         (0)      742 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18330 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/event_log/base.py
--rw-r--r--   0 root         (0) root         (0)     3801 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/event_log/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     7289 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/event_log/migration.py
--rw-r--r--   0 root         (0) root         (0)     7911 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/event_log/polling_event_watcher.py
--rw-r--r--   0 root         (0) root         (0)     9250 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/event_log/schema.py
--rw-r--r--   0 root         (0) root         (0)   122582 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/event_log/sql_event_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.394220 dagster-1.7.1/dagster/_core/storage/event_log/sqlite/
--rw-r--r--   0 root         (0) root         (0)      200 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/event_log/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.394220 dagster-1.7.1/dagster/_core/storage/event_log/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     7508 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    22497 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    10983 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/file_manager.py
--rw-r--r--   0 root         (0) root         (0)    13492 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/fs_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8819 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/input_manager.py
--rw-r--r--   0 root         (0) root         (0)    10882 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    32629 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/legacy_storage.py
--rw-r--r--   0 root         (0) root         (0)    17558 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/local_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1167 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/mem_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     4355 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/memoizable_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.394220 dagster-1.7.1/dagster/_core/storage/migration/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5964 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/migration/bigint_migration.py
--rw-r--r--   0 root         (0) root         (0)    15491 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/migration/utils.py
--rw-r--r--   0 root         (0) root         (0)     3270 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/noop_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     2361 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/output_manager.py
--rw-r--r--   0 root         (0) root         (0)    17131 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/partition_status_cache.py
--rw-r--r--   0 root         (0) root         (0)     2121 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/root.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.394220 dagster-1.7.1/dagster/_core/storage/runs/
--rw-r--r--   0 root         (0) root         (0)      386 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13903 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/runs/base.py
--rw-r--r--   0 root         (0) root         (0)     2452 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/runs/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     8716 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/runs/migration.py
--rw-r--r--   0 root         (0) root         (0)     6391 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/runs/schema.py
--rw-r--r--   0 root         (0) root         (0)    37454 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/runs/sql_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.394220 dagster-1.7.1/dagster/_core/storage/runs/sqlite/
--rw-r--r--   0 root         (0) root         (0)       69 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/runs/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.394220 dagster-1.7.1/dagster/_core/storage/runs/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     6310 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.394220 dagster-1.7.1/dagster/_core/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)      272 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7236 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/schedules/base.py
--rw-r--r--   0 root         (0) root         (0)     4133 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/schedules/migration.py
--rw-r--r--   0 root         (0) root         (0)     4086 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/schedules/schema.py
--rw-r--r--   0 root         (0) root         (0)    25146 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/schedules/sql_schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.398220 dagster-1.7.1/dagster/_core/storage/schedules/sqlite/
--rw-r--r--   0 root         (0) root         (0)       84 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/schedules/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.398220 dagster-1.7.1/dagster/_core/storage/schedules/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     3684 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     7691 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/sql.py
--rw-r--r--   0 root         (0) root         (0)     1391 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/sqlalchemy_compat.py
--rw-r--r--   0 root         (0) root         (0)      926 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/sqlite.py
--rw-r--r--   0 root         (0) root         (0)     4875 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     3546 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/tags.py
--rw-r--r--   0 root         (0) root         (0)     1186 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/temp_file_manager.py
--rw-r--r--   0 root         (0) root         (0)    19355 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/upath_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.398220 dagster-1.7.1/dagster/_core/system_config/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/system_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13962 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/system_config/composite_descent.py
--rw-r--r--   0 root         (0) root         (0)    15178 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/system_config/objects.py
--rw-r--r--   0 root         (0) root         (0)    29921 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     4824 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/telemetry_upload.py
--rw-r--r--   0 root         (0) root         (0)    22361 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.398220 dagster-1.7.1/dagster/_core/types/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3084 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/types/builtin_config_schemas.py
--rw-r--r--   0 root         (0) root         (0)     7042 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/types/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    36504 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/types/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     3571 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/types/decorator.py
--rw-r--r--   0 root         (0) root         (0)     1846 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/types/loadable_target_origin.py
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/types/primitive_mapping.py
--rw-r--r--   0 root         (0) root         (0)     4764 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/types/python_dict.py
--rw-r--r--   0 root         (0) root         (0)     2769 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/types/python_set.py
--rw-r--r--   0 root         (0) root         (0)     3620 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/types/python_tuple.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/types/transform_typing.py
--rw-r--r--   0 root         (0) root         (0)     1441 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/utility_ops.py
--rw-r--r--   0 root         (0) root         (0)     6652 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.402220 dagster-1.7.1/dagster/_core/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4457 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/workspace/autodiscovery.py
--rw-r--r--   0 root         (0) root         (0)     3422 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/workspace/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    28842 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/workspace/context.py
--rw-r--r--   0 root         (0) root         (0)    11852 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/workspace/load.py
--rw-r--r--   0 root         (0) root         (0)     4721 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/workspace/load_target.py
--rw-r--r--   0 root         (0) root         (0)     4311 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/workspace/permissions.py
--rw-r--r--   0 root         (0) root         (0)     3463 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/workspace/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.406220 dagster-1.7.1/dagster/_daemon/
--rw-r--r--   0 root         (0) root         (0)     1971 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)       30 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/__main__.py
--rw-r--r--   0 root         (0) root         (0)    41787 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/asset_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.406220 dagster-1.7.1/dagster/_daemon/auto_run_reexecution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/auto_run_reexecution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7402 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
--rw-r--r--   0 root         (0) root         (0)     9036 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
--rw-r--r--   0 root         (0) root         (0)     2665 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/backfill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.406220 dagster-1.7.1/dagster/_daemon/cli/
--rw-r--r--   0 root         (0) root         (0)     5118 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19590 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/controller.py
--rw-r--r--   0 root         (0) root         (0)    12112 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.406220 dagster-1.7.1/dagster/_daemon/monitoring/
--rw-r--r--   0 root         (0) root         (0)      320 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1792 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/monitoring/concurrency.py
--rw-r--r--   0 root         (0) root         (0)     9904 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/monitoring/run_monitoring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.406220 dagster-1.7.1/dagster/_daemon/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      100 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18369 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
--rw-r--r--   0 root         (0) root         (0)    39110 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/sensor.py
--rw-r--r--   0 root         (0) root         (0)     2860 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/types.py
--rw-r--r--   0 root         (0) root         (0)      678 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/utils.py
--rw-r--r--   0 root         (0) root         (0)     4114 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.410220 dagster-1.7.1/dagster/_experimental/
--rw-r--r--   0 root         (0) root         (0)      300 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.410220 dagster-1.7.1/dagster/_generate/
--rw-r--r--   0 root         (0) root         (0)      253 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2997 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/download.py
--rw-r--r--   0 root         (0) root         (0)     4805 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.306219 dagster-1.7.1/dagster/_generate/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.410220 dagster-1.7.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.410220 dagster-1.7.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)      175 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.410220 dagster-1.7.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)      137 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      297 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.410220 dagster-1.7.1/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)     1753 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.410220 dagster-1.7.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.410220 dagster-1.7.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
--rw-r--r--   0 root         (0) root         (0)      164 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.414220 dagster-1.7.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)       80 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       34 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      279 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.414220 dagster-1.7.1/dagster/_grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.414220 dagster-1.7.1/dagster/_grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      178 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13462 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/__generated__/api_pb2.py
--rw-r--r--   0 root         (0) root         (0)    27262 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/__generated__/api_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    43164 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/__generated__/api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2060 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       89 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/__main__.py
--rw-r--r--   0 root         (0) root         (0)    22739 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     3584 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/compile.py
--rw-r--r--   0 root         (0) root         (0)    23173 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.414220 dagster-1.7.1/dagster/_grpc/protos/
--rw-r--r--   0 root         (0) root         (0)     5993 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/protos/api.proto
--rw-r--r--   0 root         (0) root         (0)    13431 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/proxy_server.py
--rw-r--r--   0 root         (0) root         (0)    60914 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/server.py
--rw-r--r--   0 root         (0) root         (0)     5297 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/server_watcher.py
--rw-r--r--   0 root         (0) root         (0)    29291 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/types.py
--rw-r--r--   0 root         (0) root         (0)     3693 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.414220 dagster-1.7.1/dagster/_legacy/
--rw-r--r--   0 root         (0) root         (0)      180 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_legacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.414220 dagster-1.7.1/dagster/_loggers/
--rw-r--r--   0 root         (0) root         (0)     3781 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_loggers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.414220 dagster-1.7.1/dagster/_model/
--rw-r--r--   0 root         (0) root         (0)      919 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3269 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_module_alias_map.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.418220 dagster-1.7.1/dagster/_scheduler/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41378 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_scheduler/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1262 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_scheduler/stale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.418220 dagster-1.7.1/dagster/_serdes/
--rw-r--r--   0 root         (0) root         (0)      701 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_serdes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8916 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_serdes/config_class.py
--rw-r--r--   0 root         (0) root         (0)      142 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_serdes/errors.py
--rw-r--r--   0 root         (0) root         (0)     7292 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_serdes/ipc.py
--rw-r--r--   0 root         (0) root         (0)    42415 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_serdes/serdes.py
--rw-r--r--   0 root         (0) root         (0)      674 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_serdes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.418220 dagster-1.7.1/dagster/_seven/
--rw-r--r--   0 root         (0) root         (0)     5455 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_seven/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_seven/abc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.418220 dagster-1.7.1/dagster/_seven/compat/
--rw-r--r--   0 root         (0) root         (0)      105 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_seven/compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3967 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_seven/compat/pendulum.py
--rw-r--r--   0 root         (0) root         (0)      383 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_seven/json.py
--rw-r--r--   0 root         (0) root         (0)      354 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_seven/temp_dir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.422220 dagster-1.7.1/dagster/_utils/
--rw-r--r--   0 root         (0) root         (0)    24377 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9314 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/alert.py
--rw-r--r--   0 root         (0) root         (0)     2250 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/backoff.py
--rw-r--r--   0 root         (0) root         (0)     5404 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/cached_method.py
--rw-r--r--   0 root         (0) root         (0)    42589 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/caching_instance_queryer.py
--rw-r--r--   0 root         (0) root         (0)     5865 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/concurrency.py
--rw-r--r--   0 root         (0) root         (0)    12887 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/container.py
--rw-r--r--   0 root         (0) root         (0)     2412 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)      799 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/env.py
--rw-r--r--   0 root         (0) root         (0)     5477 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/error.py
--rw-r--r--   0 root         (0) root         (0)     1255 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/external.py
--rw-r--r--   0 root         (0) root         (0)      891 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/forked_pdb.py
--rw-r--r--   0 root         (0) root         (0)     1870 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/hosted_user_process.py
--rw-r--r--   0 root         (0) root         (0)     2796 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/indenting_printer.py
--rw-r--r--   0 root         (0) root         (0)      745 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/internal_init.py
--rw-r--r--   0 root         (0) root         (0)     3227 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/interrupts.py
--rw-r--r--   0 root         (0) root         (0)    11214 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/log.py
--rw-r--r--   0 root         (0) root         (0)     2313 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/merger.py
--rw-r--r--   0 root         (0) root         (0)     1507 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/net.py
--rw-r--r--   0 root         (0) root         (0)      208 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/partitions.py
--rw-r--r--   0 root         (0) root         (0)    33171 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/schedules.py
--rw-r--r--   0 root         (0) root         (0)      477 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/security.py
--rw-r--r--   0 root         (0) root         (0)     3289 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     1820 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/temp_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.422220 dagster-1.7.1/dagster/_utils/test/
--rw-r--r--   0 root         (0) root         (0)    13678 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7622 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/test/data_versions.py
--rw-r--r--   0 root         (0) root         (0)      119 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/test/hello_world_defs.py
--rw-r--r--   0 root         (0) root         (0)      214 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/test/hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8622 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/test/mysql_instance.py
--rw-r--r--   0 root         (0) root         (0)      256 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/test/named_hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8959 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/test/postgres_instance.py
--rw-r--r--   0 root         (0) root         (0)    35720 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/test/schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.426220 dagster-1.7.1/dagster/_utils/test/toys/
--rw-r--r--   0 root         (0) root         (0)       83 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/test/toys/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/test/toys/single_repository.py
--rw-r--r--   0 root         (0) root         (0)     2004 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/timing.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/typed_dict.py
--rw-r--r--   0 root         (0) root         (0)      170 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/types.py
--rw-r--r--   0 root         (0) root         (0)     3334 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/typing_api.py
--rw-r--r--   0 root         (0) root         (0)     4740 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/warnings.py
--rw-r--r--   0 root         (0) root         (0)     4902 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/yaml_utils.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/py.typed
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.310219 dagster-1.7.1/dagster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8928 2024-04-11 18:04:47.000000 dagster-1.7.1/dagster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    27988 2024-04-11 18:04:47.000000 dagster-1.7.1/dagster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:04:47.000000 dagster-1.7.1/dagster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2024-04-11 18:04:47.000000 dagster-1.7.1/dagster.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1458 2024-04-11 18:04:47.000000 dagster-1.7.1/dagster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-11 18:04:47.000000 dagster-1.7.1/dagster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      154 2024-04-11 18:04:47.426220 dagster-1.7.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6827 2024-04-11 18:04:20.000000 dagster-1.7.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.243156 dagster-1.7.2rc1/
+-rw-r--r--   0 root         (0) root         (0)      553 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/COPYING
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      533 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9870 2024-04-16 17:50:58.243156 dagster-1.7.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8153 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.135156 dagster-1.7.2rc1/dagster/
+-rw-r--r--   0 root         (0) root         (0)    29906 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    20744 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.135156 dagster-1.7.2rc1/dagster/_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      731 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_api/get_server_id.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_api/list_repositories.py
+-rw-r--r--   0 root         (0) root         (0)      531 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_api/notebook_data.py
+-rw-r--r--   0 root         (0) root         (0)     3224 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_api/snapshot_execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_api/snapshot_job.py
+-rw-r--r--   0 root         (0) root         (0)     5483 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_api/snapshot_partition.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_api/snapshot_repository.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_api/snapshot_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3370 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_api/snapshot_sensor.py
+-rw-r--r--   0 root         (0) root         (0)      478 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_builtins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.139155 dagster-1.7.2rc1/dagster/_check/
+-rw-r--r--   0 root         (0) root         (0)     1352 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_check/README.md
+-rw-r--r--   0 root         (0) root         (0)    52040 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_check/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.139155 dagster-1.7.2rc1/dagster/_cli/
+-rw-r--r--   0 root         (0) root         (0)     1182 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26898 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_cli/api.py
+-rw-r--r--   0 root         (0) root         (0)     8030 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_cli/asset.py
+-rw-r--r--   0 root         (0) root         (0)     8302 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_cli/code_server.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_cli/config_scaffolder.py
+-rw-r--r--   0 root         (0) root         (0)     3513 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_cli/debug.py
+-rw-r--r--   0 root         (0) root         (0)     8134 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_cli/dev.py
+-rw-r--r--   0 root         (0) root         (0)     6651 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_cli/instance.py
+-rw-r--r--   0 root         (0) root         (0)    30542 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_cli/job.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_cli/load_handle.py
+-rw-r--r--   0 root         (0) root         (0)     9114 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_cli/project.py
+-rw-r--r--   0 root         (0) root         (0)     5120 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_cli/run.py
+-rw-r--r--   0 root         (0) root         (0)    19351 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_cli/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    15461 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_cli/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     4259 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.139155 dagster-1.7.2rc1/dagster/_cli/workspace/
+-rw-r--r--   0 root         (0) root         (0)      180 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_cli/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27910 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_cli/workspace/cli_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.143155 dagster-1.7.2rc1/dagster/_config/
+-rw-r--r--   0 root         (0) root         (0)     3186 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15830 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/config_type.py
+-rw-r--r--   0 root         (0) root         (0)    18787 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/evaluate_value_result.py
+-rw-r--r--   0 root         (0) root         (0)    14918 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/field.py
+-rw-r--r--   0 root         (0) root         (0)    19728 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/field_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9536 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/post_process.py
+-rw-r--r--   0 root         (0) root         (0)      855 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/primitive_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.147155 dagster-1.7.2rc1/dagster/_config/pythonic_config/
+-rw-r--r--   0 root         (0) root         (0)     1394 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/pythonic_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/pythonic_config/attach_other_object_to_context.py
+-rw-r--r--   0 root         (0) root         (0)    18042 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/pythonic_config/config.py
+-rw-r--r--   0 root         (0) root         (0)    11496 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/pythonic_config/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    11583 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/pythonic_config/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4022 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/pythonic_config/pydantic_compat_layer.py
+-rw-r--r--   0 root         (0) root         (0)    41251 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/pythonic_config/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/pythonic_config/type_check_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8375 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/pythonic_config/typing_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12532 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/snap.py
+-rw-r--r--   0 root         (0) root         (0)     3087 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/source.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/stack.py
+-rw-r--r--   0 root         (0) root         (0)     7772 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/traversal_context.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/type_printer.py
+-rw-r--r--   0 root         (0) root         (0)    17137 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_config/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.151156 dagster-1.7.2rc1/dagster/_core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.151156 dagster-1.7.2rc1/dagster/_core/asset_graph_view/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/asset_graph_view/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21047 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/asset_graph_view/asset_graph_view.py
+-rw-r--r--   0 root         (0) root         (0)      994 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13427 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/code_pointer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.151156 dagster-1.7.2rc1/dagster/_core/container_context/
+-rw-r--r--   0 root         (0) root         (0)      184 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/container_context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/container_context/config.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/debug.py
+-rw-r--r--   0 root         (0) root         (0)     9665 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/decorator_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.171156 dagster-1.7.2rc1/dagster/_core/definitions/
+-rw-r--r--   0 root         (0) root         (0)     7827 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4506 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/asset_check_evaluation.py
+-rw-r--r--   0 root         (0) root         (0)     7052 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/asset_check_result.py
+-rw-r--r--   0 root         (0) root         (0)     5416 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/asset_check_spec.py
+-rw-r--r--   0 root         (0) root         (0)     6073 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/asset_checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.175155 dagster-1.7.2rc1/dagster/_core/definitions/asset_condition/
+-rw-r--r--   0 root         (0) root         (0)       62 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/asset_condition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21141 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/asset_condition/asset_condition.py
+-rw-r--r--   0 root         (0) root         (0)    16508 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/asset_condition/asset_condition_evaluation_context.py
+-rw-r--r--   0 root         (0) root         (0)    26314 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/asset_daemon_context.py
+-rw-r--r--   0 root         (0) root         (0)    10648 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/asset_daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)     4628 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/asset_dep.py
+-rw-r--r--   0 root         (0) root         (0)    10133 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)     7700 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/asset_graph_differ.py
+-rw-r--r--   0 root         (0) root         (0)    16636 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/asset_graph_subset.py
+-rw-r--r--   0 root         (0) root         (0)     3644 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/asset_in.py
+-rw-r--r--   0 root         (0) root         (0)    29917 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/asset_job.py
+-rw-r--r--   0 root         (0) root         (0)     6060 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)    30355 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/asset_layer.py
+-rw-r--r--   0 root         (0) root         (0)     6945 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/asset_out.py
+-rw-r--r--   0 root         (0) root         (0)    39535 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/asset_selection.py
+-rw-r--r--   0 root         (0) root         (0)     7444 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6764 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/asset_spec.py
+-rw-r--r--   0 root         (0) root         (0)    10466 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/asset_subset.py
+-rw-r--r--   0 root         (0) root         (0)    79909 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13905 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    54478 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/auto_materialize_rule.py
+-rw-r--r--   0 root         (0) root         (0)    21726 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/auto_materialize_rule_evaluation.py
+-rw-r--r--   0 root         (0) root         (0)     2768 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/auto_materialize_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/backfill_policy.py
+-rw-r--r--   0 root         (0) root         (0)    34666 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/base_asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)    16772 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/cacheable_assets.py
+-rw-r--r--   0 root         (0) root         (0)    40623 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/composition.py
+-rw-r--r--   0 root         (0) root         (0)     4278 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/config.py
+-rw-r--r--   0 root         (0) root         (0)    14811 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/configurable.py
+-rw-r--r--   0 root         (0) root         (0)    22990 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/data_time.py
+-rw-r--r--   0 root         (0) root         (0)    30060 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/data_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.175155 dagster-1.7.2rc1/dagster/_core/definitions/decorators/
+-rw-r--r--   0 root         (0) root         (0)      620 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16572 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/decorators/asset_check_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    69203 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/decorators/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4907 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/decorators/config_mapping_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9077 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/decorators/graph_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9353 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/decorators/hook_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    10815 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/decorators/job_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    19011 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/decorators/op_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    15668 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/decorators/repository_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8718 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/decorators/schedule_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    12463 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/decorators/sensor_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    12664 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/decorators/source_asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     5267 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/definition_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    23545 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/definitions_class.py
+-rw-r--r--   0 root         (0) root         (0)    42247 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/dependency.py
+-rw-r--r--   0 root         (0) root         (0)    26888 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/events.py
+-rw-r--r--   0 root         (0) root         (0)    21182 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/executor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9379 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/external_asset.py
+-rw-r--r--   0 root         (0) root         (0)     9766 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/freshness_based_auto_materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.179155 dagster-1.7.2rc1/dagster/_core/definitions/freshness_checks/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/freshness_checks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5838 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/freshness_checks/last_update.py
+-rw-r--r--   0 root         (0) root         (0)     7677 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/freshness_checks/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     7938 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/freshness_checks/shared_builder.py
+-rw-r--r--   0 root         (0) root         (0)     4669 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/freshness_checks/time_partition.py
+-rw-r--r--   0 root         (0) root         (0)    10573 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/freshness_checks/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8801 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16401 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/freshness_policy_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    47569 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/graph_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6546 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/hook_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1524 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/hook_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3537 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/inference.py
+-rw-r--r--   0 root         (0) root         (0)    21027 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/input.py
+-rw-r--r--   0 root         (0) root         (0)     6410 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/instigation_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/job_base.py
+-rw-r--r--   0 root         (0) root         (0)    53689 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/job_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5693 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/load_asset_checks_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)    22306 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/load_assets_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)     7171 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/logger_definition.py
+-rw-r--r--   0 root         (0) root         (0)      636 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/logger_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     8959 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.179155 dagster-1.7.2rc1/dagster/_core/definitions/metadata/
+-rw-r--r--   0 root         (0) root         (0)    42305 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12410 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/metadata/table.py
+-rw-r--r--   0 root         (0) root         (0)    57203 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/multi_asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    22029 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/multi_dimensional_partitions.py
+-rw-r--r--   0 root         (0) root         (0)      197 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/no_step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11892 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/node_container.py
+-rw-r--r--   0 root         (0) root         (0)     8016 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/node_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/observe.py
+-rw-r--r--   0 root         (0) root         (0)    23078 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    23141 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/op_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7551 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/op_selection.py
+-rw-r--r--   0 root         (0) root         (0)    19237 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/output.py
+-rw-r--r--   0 root         (0) root         (0)    50520 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/partition.py
+-rw-r--r--   0 root         (0) root         (0)      630 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/partition_key_range.py
+-rw-r--r--   0 root         (0) root         (0)    47665 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    11087 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/partitioned_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/policy.py
+-rw-r--r--   0 root         (0) root         (0)    27737 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/reconstruct.py
+-rw-r--r--   0 root         (0) root         (0)    21602 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/remote_asset_graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.179155 dagster-1.7.2rc1/dagster/_core/definitions/repository_definition/
+-rw-r--r--   0 root         (0) root         (0)      654 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/repository_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6024 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/repository_definition/caching_index.py
+-rw-r--r--   0 root         (0) root         (0)    21698 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/repository_definition/repository_data.py
+-rw-r--r--   0 root         (0) root         (0)    20892 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/repository_definition/repository_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)    20432 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/repository_definition/repository_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/repository_definition/valid_definitions.py
+-rw-r--r--   0 root         (0) root         (0)     8858 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/resolved_asset_deps.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/resource_annotation.py
+-rw-r--r--   0 root         (0) root         (0)    17900 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/resource_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/resource_invocation.py
+-rw-r--r--   0 root         (0) root         (0)    10320 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/resource_requirement.py
+-rw-r--r--   0 root         (0) root         (0)     3383 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/result.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    19555 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/run_request.py
+-rw-r--r--   0 root         (0) root         (0)    44126 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/run_status_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    39363 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6225 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/schema_change_checks.py
+-rw-r--r--   0 root         (0) root         (0)     5134 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/scoped_resources_builder.py
+-rw-r--r--   0 root         (0) root         (0)    14134 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/selector.py
+-rw-r--r--   0 root         (0) root         (0)    53797 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    19244 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/source_asset.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/target.py
+-rw-r--r--   0 root         (0) root         (0)    21859 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/time_window_partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)   102142 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/time_window_partitions.py
+-rw-r--r--   0 root         (0) root         (0)    15160 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/unresolved_asset_job_definition.py
+-rw-r--r--   0 root         (0) root         (0)    11017 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3982 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/definitions/version_strategy.py
+-rw-r--r--   0 root         (0) root         (0)    27136 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    18062 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/event_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.179155 dagster-1.7.2rc1/dagster/_core/events/
+-rw-r--r--   0 root         (0) root         (0)    71913 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7635 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/events/log.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/events/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.183156 dagster-1.7.2rc1/dagster/_core/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38363 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/api.py
+-rw-r--r--   0 root         (0) root         (0)    64654 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/asset_backfill.py
+-rw-r--r--   0 root         (0) root         (0)    17100 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6296 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/build_resources.py
+-rw-r--r--   0 root         (0) root         (0)      224 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/bulk_actions.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/compute_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.187156 dagster-1.7.2rc1/dagster/_core/execution/context/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79687 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/context/compute.py
+-rw-r--r--   0 root         (0) root         (0)    17598 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/context/hook.py
+-rw-r--r--   0 root         (0) root         (0)     9613 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/context/init.py
+-rw-r--r--   0 root         (0) root         (0)    29167 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/context/input.py
+-rw-r--r--   0 root         (0) root         (0)    40124 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/context/invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/context/logger.py
+-rw-r--r--   0 root         (0) root         (0)    37256 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/context/output.py
+-rw-r--r--   0 root         (0) root         (0)    56002 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/context/system.py
+-rw-r--r--   0 root         (0) root         (0)    18837 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/context_creation_job.py
+-rw-r--r--   0 root         (0) root         (0)     5135 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/execute_in_process.py
+-rw-r--r--   0 root         (0) root         (0)     5897 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/execute_in_process_result.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/execution_result.py
+-rw-r--r--   0 root         (0) root         (0)     8602 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/host_mode.py
+-rw-r--r--   0 root         (0) root         (0)    14247 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/job_backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6723 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/job_execution_result.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/memoization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.191156 dagster-1.7.2rc1/dagster/_core/execution/plan/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/plan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26460 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/plan/active.py
+-rw-r--r--   0 root         (0) root         (0)     9850 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/plan/compute.py
+-rw-r--r--   0 root         (0) root         (0)    17019 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/plan/compute_generator.py
+-rw-r--r--   0 root         (0) root         (0)    16974 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/plan/execute_plan.py
+-rw-r--r--   0 root         (0) root         (0)    40549 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/plan/execute_step.py
+-rw-r--r--   0 root         (0) root         (0)    11036 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/plan/external_step.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/plan/handle.py
+-rw-r--r--   0 root         (0) root         (0)    39260 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/plan/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     6251 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/plan/instance_concurrency_context.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/plan/local_external_step_main.py
+-rw-r--r--   0 root         (0) root         (0)     5706 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/plan/objects.py
+-rw-r--r--   0 root         (0) root         (0)     7326 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/plan/outputs.py
+-rw-r--r--   0 root         (0) root         (0)    61075 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/plan/plan.py
+-rw-r--r--   0 root         (0) root         (0)      114 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/plan/resume_retry.py
+-rw-r--r--   0 root         (0) root         (0)    17174 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/plan/state.py
+-rw-r--r--   0 root         (0) root         (0)    15985 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/plan/step.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/plan/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/poll_compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)     8230 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/resolve_versions.py
+-rw-r--r--   0 root         (0) root         (0)    19141 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/resources_init.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/retries.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/run_cancellation_thread.py
+-rw-r--r--   0 root         (0) root         (0)     9950 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/stats.py
+-rw-r--r--   0 root         (0) root         (0)    14043 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/submit_asset_runs.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/validate_run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/watch_orphans.py
+-rw-r--r--   0 root         (0) root         (0)     4311 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/execution/with_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.191156 dagster-1.7.2rc1/dagster/_core/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/executor/base.py
+-rw-r--r--   0 root         (0) root         (0)     5989 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/executor/child_process_executor.py
+-rw-r--r--   0 root         (0) root         (0)     3366 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/executor/in_process.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/executor/init.py
+-rw-r--r--   0 root         (0) root         (0)    15497 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/executor/multiprocess.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.191156 dagster-1.7.2rc1/dagster/_core/executor/step_delegating/
+-rw-r--r--   0 root         (0) root         (0)      247 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/executor/step_delegating/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16894 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/executor/step_delegating/step_delegating_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.191156 dagster-1.7.2rc1/dagster/_core/executor/step_delegating/step_handler/
+-rw-r--r--   0 root         (0) root         (0)      152 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/executor/step_delegating/step_handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/executor/step_delegating/step_handler/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.191156 dagster-1.7.2rc1/dagster/_core/instance/
+-rw-r--r--   0 root         (0) root         (0)   132749 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/instance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16700 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/instance/config.py
+-rw-r--r--   0 root         (0) root         (0)    24178 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/instance/ref.py
+-rw-r--r--   0 root         (0) root         (0)     3899 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/instance_for_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.195155 dagster-1.7.2rc1/dagster/_core/launcher/
+-rw-r--r--   0 root         (0) root         (0)      297 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3819 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/launcher/base.py
+-rw-r--r--   0 root         (0) root         (0)     6645 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/launcher/default_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/launcher/sync_in_memory_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)      473 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/libraries.py
+-rw-r--r--   0 root         (0) root         (0)    18041 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/nux.py
+-rw-r--r--   0 root         (0) root         (0)     5736 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/op_concurrency_limits_counter.py
+-rw-r--r--   0 root         (0) root         (0)     3691 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.195155 dagster-1.7.2rc1/dagster/_core/pipes/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/pipes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8974 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/pipes/client.py
+-rw-r--r--   0 root         (0) root         (0)    18318 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/pipes/context.py
+-rw-r--r--   0 root         (0) root         (0)     5648 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/pipes/subprocess.py
+-rw-r--r--   0 root         (0) root         (0)    25661 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/pipes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.195155 dagster-1.7.2rc1/dagster/_core/remote_representation/
+-rw-r--r--   0 root         (0) root         (0)     2793 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/remote_representation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36695 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/remote_representation/code_location.py
+-rw-r--r--   0 root         (0) root         (0)    37482 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/remote_representation/external.py
+-rw-r--r--   0 root         (0) root         (0)    83392 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/remote_representation/external_data.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/remote_representation/feature_flags.py
+-rw-r--r--   0 root         (0) root         (0)    12429 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/remote_representation/grpc_server_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/remote_representation/grpc_server_state_subscriber.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/remote_representation/handle.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/remote_representation/historical.py
+-rw-r--r--   0 root         (0) root         (0)     4850 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/remote_representation/job_index.py
+-rw-r--r--   0 root         (0) root         (0)    19669 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/remote_representation/origin.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/remote_representation/represented.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.195155 dagster-1.7.2rc1/dagster/_core/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      267 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/run_coordinator/base.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/run_coordinator/default_run_coordinator.py
+-rw-r--r--   0 root         (0) root         (0)    13364 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/run_coordinator/queued_run_coordinator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.199156 dagster-1.7.2rc1/dagster/_core/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      534 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/scheduler/execution.py
+-rw-r--r--   0 root         (0) root         (0)    28809 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/scheduler/instigation.py
+-rw-r--r--   0 root         (0) root         (0)    10931 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/scheduler/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.199156 dagster-1.7.2rc1/dagster/_core/secrets/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/secrets/env_file.py
+-rw-r--r--   0 root         (0) root         (0)      388 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.199156 dagster-1.7.2rc1/dagster/_core/selector/
+-rw-r--r--   0 root         (0) root         (0)      295 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/selector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18109 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/selector/subset_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.199156 dagster-1.7.2rc1/dagster/_core/snap/
+-rw-r--r--   0 root         (0) root         (0)     2842 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/snap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/snap/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/snap/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     9302 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/snap/dep_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    12155 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/snap/execution_plan_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    16934 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/snap/job_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4561 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/snap/mode.py
+-rw-r--r--   0 root         (0) root         (0)    14185 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/snap/node.py
+-rw-r--r--   0 root         (0) root         (0)     3183 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/snap/snap_to_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.203156 dagster-1.7.2rc1/dagster/_core/storage/
+-rw-r--r--   0 root         (0) root         (0)     3058 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/DEVELOPING.md
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.203156 dagster-1.7.2rc1/dagster/_core/storage/alembic/
+-rw-r--r--   0 root         (0) root         (0)     6686 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/README.md
+-rw-r--r--   0 root         (0) root         (0)      687 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.215156 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     3150 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/001_initial_1.py
+-rw-r--r--   0 root         (0) root         (0)      312 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/001_initial_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      599 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      953 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      953 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      956 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      956 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      325 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/017_initial_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      531 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      635 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
+-rw-r--r--   0 root         (0) root         (0)      958 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
+-rw-r--r--   0 root         (0) root         (0)      499 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1951 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
+-rw-r--r--   0 root         (0) root         (0)      428 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
+-rw-r--r--   0 root         (0) root         (0)      427 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3887 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/asset_check_execution_record.py
+-rw-r--r--   0 root         (0) root         (0)     7301 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/asset_value_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/base_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.215156 dagster-1.7.2rc1/dagster/_core/storage/branching/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/branching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/branching/branching_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8725 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/captured_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16223 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/cloud_storage_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9557 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/config.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)    25656 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/dagster_run.py
+-rw-r--r--   0 root         (0) root         (0)    11187 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/db_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.215156 dagster-1.7.2rc1/dagster/_core/storage/event_log/
+-rw-r--r--   0 root         (0) root         (0)      742 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18869 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/event_log/base.py
+-rw-r--r--   0 root         (0) root         (0)     3801 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/event_log/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     7289 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/event_log/migration.py
+-rw-r--r--   0 root         (0) root         (0)     7911 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/event_log/polling_event_watcher.py
+-rw-r--r--   0 root         (0) root         (0)     9250 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/event_log/schema.py
+-rw-r--r--   0 root         (0) root         (0)   122582 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/event_log/sql_event_log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.215156 dagster-1.7.2rc1/dagster/_core/storage/event_log/sqlite/
+-rw-r--r--   0 root         (0) root         (0)      200 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/event_log/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.215156 dagster-1.7.2rc1/dagster/_core/storage/event_log/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     7508 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    22497 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    10983 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    13492 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/fs_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8819 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/input_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10882 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    32629 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/legacy_storage.py
+-rw-r--r--   0 root         (0) root         (0)    17558 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/local_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/mem_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4355 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/memoizable_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.215156 dagster-1.7.2rc1/dagster/_core/storage/migration/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5964 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/migration/bigint_migration.py
+-rw-r--r--   0 root         (0) root         (0)    15491 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/migration/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/noop_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/output_manager.py
+-rw-r--r--   0 root         (0) root         (0)    17131 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/partition_status_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/root.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.223156 dagster-1.7.2rc1/dagster/_core/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)      386 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13903 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/runs/base.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/runs/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     8716 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/runs/migration.py
+-rw-r--r--   0 root         (0) root         (0)     6391 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/runs/schema.py
+-rw-r--r--   0 root         (0) root         (0)    37454 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/runs/sql_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.223156 dagster-1.7.2rc1/dagster/_core/storage/runs/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/runs/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.223156 dagster-1.7.2rc1/dagster/_core/storage/runs/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     6310 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.223156 dagster-1.7.2rc1/dagster/_core/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)      272 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7236 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/schedules/base.py
+-rw-r--r--   0 root         (0) root         (0)     4133 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/schedules/migration.py
+-rw-r--r--   0 root         (0) root         (0)     4086 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/schedules/schema.py
+-rw-r--r--   0 root         (0) root         (0)    25146 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/schedules/sql_schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.223156 dagster-1.7.2rc1/dagster/_core/storage/schedules/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       84 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/schedules/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.223156 dagster-1.7.2rc1/dagster/_core/storage/schedules/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     3684 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     7691 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/sql.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/sqlalchemy_compat.py
+-rw-r--r--   0 root         (0) root         (0)      926 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     4875 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1186 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/temp_file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    19215 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/storage/upath_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.223156 dagster-1.7.2rc1/dagster/_core/system_config/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/system_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13962 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/system_config/composite_descent.py
+-rw-r--r--   0 root         (0) root         (0)    15178 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/system_config/objects.py
+-rw-r--r--   0 root         (0) root         (0)    29921 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/telemetry_upload.py
+-rw-r--r--   0 root         (0) root         (0)    22361 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.223156 dagster-1.7.2rc1/dagster/_core/types/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3084 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/types/builtin_config_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     7042 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/types/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    36504 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/types/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     3571 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/types/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/types/loadable_target_origin.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/types/primitive_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     4764 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/types/python_dict.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/types/python_set.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/types/python_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/types/transform_typing.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/utility_ops.py
+-rw-r--r--   0 root         (0) root         (0)     6652 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.223156 dagster-1.7.2rc1/dagster/_core/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4457 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/workspace/autodiscovery.py
+-rw-r--r--   0 root         (0) root         (0)     2679 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/workspace/batch_asset_record_loader.py
+-rw-r--r--   0 root         (0) root         (0)     3422 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/workspace/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    29210 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/workspace/context.py
+-rw-r--r--   0 root         (0) root         (0)    11852 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/workspace/load.py
+-rw-r--r--   0 root         (0) root         (0)     4721 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/workspace/load_target.py
+-rw-r--r--   0 root         (0) root         (0)     4311 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/workspace/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     3463 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_core/workspace/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.223156 dagster-1.7.2rc1/dagster/_daemon/
+-rw-r--r--   0 root         (0) root         (0)     1971 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_daemon/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    41795 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_daemon/asset_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.223156 dagster-1.7.2rc1/dagster/_daemon/auto_run_reexecution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_daemon/auto_run_reexecution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7402 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
+-rw-r--r--   0 root         (0) root         (0)     9036 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
+-rw-r--r--   0 root         (0) root         (0)     2665 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_daemon/backfill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.223156 dagster-1.7.2rc1/dagster/_daemon/cli/
+-rw-r--r--   0 root         (0) root         (0)     5118 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_daemon/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19590 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_daemon/controller.py
+-rw-r--r--   0 root         (0) root         (0)    12112 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_daemon/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.227156 dagster-1.7.2rc1/dagster/_daemon/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      320 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_daemon/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_daemon/monitoring/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)     9904 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_daemon/monitoring/run_monitoring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.227156 dagster-1.7.2rc1/dagster/_daemon/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      100 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_daemon/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18369 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    39110 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_daemon/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_daemon/types.py
+-rw-r--r--   0 root         (0) root         (0)      678 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_daemon/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4114 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_daemon/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.227156 dagster-1.7.2rc1/dagster/_experimental/
+-rw-r--r--   0 root         (0) root         (0)      300 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_experimental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.227156 dagster-1.7.2rc1/dagster/_generate/
+-rw-r--r--   0 root         (0) root         (0)      253 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_generate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_generate/download.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_generate/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.127155 dagster-1.7.2rc1/dagster/_generate/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.227156 dagster-1.7.2rc1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.227156 dagster-1.7.2rc1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)      175 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.227156 dagster-1.7.2rc1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)      137 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      297 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.227156 dagster-1.7.2rc1/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)     1753 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.227156 dagster-1.7.2rc1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.227156 dagster-1.7.2rc1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
+-rw-r--r--   0 root         (0) root         (0)      164 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.227156 dagster-1.7.2rc1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       34 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      279 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.231156 dagster-1.7.2rc1/dagster/_grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.231156 dagster-1.7.2rc1/dagster/_grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      178 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13462 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_grpc/__generated__/api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    27262 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_grpc/__generated__/api_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    43164 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_grpc/__generated__/api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       89 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_grpc/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    22739 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     3584 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_grpc/compile.py
+-rw-r--r--   0 root         (0) root         (0)    23173 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_grpc/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.231156 dagster-1.7.2rc1/dagster/_grpc/protos/
+-rw-r--r--   0 root         (0) root         (0)     5993 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_grpc/protos/api.proto
+-rw-r--r--   0 root         (0) root         (0)    13431 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_grpc/proxy_server.py
+-rw-r--r--   0 root         (0) root         (0)    60914 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_grpc/server.py
+-rw-r--r--   0 root         (0) root         (0)     5297 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_grpc/server_watcher.py
+-rw-r--r--   0 root         (0) root         (0)    29291 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_grpc/types.py
+-rw-r--r--   0 root         (0) root         (0)     3693 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_grpc/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.231156 dagster-1.7.2rc1/dagster/_legacy/
+-rw-r--r--   0 root         (0) root         (0)      180 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_legacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.231156 dagster-1.7.2rc1/dagster/_loggers/
+-rw-r--r--   0 root         (0) root         (0)     3781 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_loggers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.231156 dagster-1.7.2rc1/dagster/_model/
+-rw-r--r--   0 root         (0) root         (0)      919 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_module_alias_map.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.231156 dagster-1.7.2rc1/dagster/_scheduler/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41378 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_scheduler/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1262 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_scheduler/stale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.231156 dagster-1.7.2rc1/dagster/_serdes/
+-rw-r--r--   0 root         (0) root         (0)      701 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_serdes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9680 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_serdes/config_class.py
+-rw-r--r--   0 root         (0) root         (0)      142 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_serdes/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7292 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_serdes/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    42415 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_serdes/serdes.py
+-rw-r--r--   0 root         (0) root         (0)      674 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_serdes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.231156 dagster-1.7.2rc1/dagster/_seven/
+-rw-r--r--   0 root         (0) root         (0)     5455 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_seven/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_seven/abc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.231156 dagster-1.7.2rc1/dagster/_seven/compat/
+-rw-r--r--   0 root         (0) root         (0)      105 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_seven/compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_seven/compat/pendulum.py
+-rw-r--r--   0 root         (0) root         (0)      383 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_seven/json.py
+-rw-r--r--   0 root         (0) root         (0)      354 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_seven/temp_dir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.235156 dagster-1.7.2rc1/dagster/_utils/
+-rw-r--r--   0 root         (0) root         (0)    24377 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9314 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/alert.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/backoff.py
+-rw-r--r--   0 root         (0) root         (0)     5404 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/cached_method.py
+-rw-r--r--   0 root         (0) root         (0)    42615 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/caching_instance_queryer.py
+-rw-r--r--   0 root         (0) root         (0)     5865 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)    12887 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/container.py
+-rw-r--r--   0 root         (0) root         (0)     2412 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)      799 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/env.py
+-rw-r--r--   0 root         (0) root         (0)     5477 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/error.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/external.py
+-rw-r--r--   0 root         (0) root         (0)      891 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/forked_pdb.py
+-rw-r--r--   0 root         (0) root         (0)     1870 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/hosted_user_process.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/indenting_printer.py
+-rw-r--r--   0 root         (0) root         (0)      745 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/internal_init.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/interrupts.py
+-rw-r--r--   0 root         (0) root         (0)    11214 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/log.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/merger.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/net.py
+-rw-r--r--   0 root         (0) root         (0)      208 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/partitions.py
+-rw-r--r--   0 root         (0) root         (0)    33171 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/schedules.py
+-rw-r--r--   0 root         (0) root         (0)      477 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/security.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/temp_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.243156 dagster-1.7.2rc1/dagster/_utils/test/
+-rw-r--r--   0 root         (0) root         (0)    13678 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7622 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/test/data_versions.py
+-rw-r--r--   0 root         (0) root         (0)      119 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/test/hello_world_defs.py
+-rw-r--r--   0 root         (0) root         (0)      214 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/test/hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/test/mysql_instance.py
+-rw-r--r--   0 root         (0) root         (0)      256 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/test/named_hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8959 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/test/postgres_instance.py
+-rw-r--r--   0 root         (0) root         (0)    36138 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/test/schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.243156 dagster-1.7.2rc1/dagster/_utils/test/toys/
+-rw-r--r--   0 root         (0) root         (0)       83 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/test/toys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/test/toys/single_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/timing.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/typed_dict.py
+-rw-r--r--   0 root         (0) root         (0)      170 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/types.py
+-rw-r--r--   0 root         (0) root         (0)     3334 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/typing_api.py
+-rw-r--r--   0 root         (0) root         (0)     4740 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/warnings.py
+-rw-r--r--   0 root         (0) root         (0)     4902 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/_utils/yaml_utils.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/py.typed
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/dagster/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:50:58.135156 dagster-1.7.2rc1/dagster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9870 2024-04-16 17:50:57.000000 dagster-1.7.2rc1/dagster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    28041 2024-04-16 17:50:57.000000 dagster-1.7.2rc1/dagster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:50:57.000000 dagster-1.7.2rc1/dagster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2024-04-16 17:50:57.000000 dagster-1.7.2rc1/dagster.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1461 2024-04-16 17:50:57.000000 dagster-1.7.2rc1/dagster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 17:50:57.000000 dagster-1.7.2rc1/dagster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2024-04-16 17:50:58.251156 dagster-1.7.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6830 2024-04-16 17:50:34.000000 dagster-1.7.2rc1/setup.py
```

### Comparing `dagster-1.7.1/COPYING` & `dagster-1.7.2rc1/COPYING`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/LICENSE` & `dagster-1.7.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/MANIFEST.in` & `dagster-1.7.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/PKG-INFO` & `dagster-1.7.2rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.7.1
+Version: 1.7.2rc1
 Summary: Dagster is an orchestration platform for the development, production, and observation of data assets.
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Documentation, https://docs.dagster.io
@@ -102,14 +102,29 @@
 
 <p align="center">
   <img width="100%" alt="An example asset graph as rendered in the Dagster UI" src="https://raw.githubusercontent.com/dagster-io/dagster/master/.github/example-lineage.png">
 </p>
 
 Dagster is built to be used at every stage of the data development lifecycle - local development, unit tests, integration tests, staging environments, all the way up to production.
 
+## Special Event: Introducing Dagster+
+
+<p align="center">
+  <img width="100%" alt="Join us on April 17 (12PM ET) for a special event introducing Dagster+" src="https://i.imgur.com/1r7hOep.png">
+</p>
+
+Join us on April 17 (12PM ET) for a special event introducing Dagster+. [Register for our Dagster+ launch event here](https://dagster.io/events/dagster-plus-launch-event)
+
+In addition to the core open-source project, we are excited to announce Dagster+, the next generation of Dagster's cloud offering.
+
+- Find out how to weave data reliability and quality checks into the execution of your data pipelines.
+- See how diff-based branch deployments will accelerate your development cycle and cut extraneous compute costs.
+- Get a deep understanding of what is driving the cost of your data pipelines, then optimize to get the best cost/performance outcomes.
+- Enjoy the benefits of built-in data cataloging, and asset-level rich metadata.
+
 ## Quick Start:
 
 If you're new to Dagster, we recommend reading about its [core concepts](https://docs.dagster.io/concepts) or learning with the hands-on [tutorial](https://docs.dagster.io/tutorial).
 
 Dagster is available on PyPI and officially supports Python 3.8 through Python 3.12.
 
 ```bash
```

### Comparing `dagster-1.7.1/README.md` & `dagster-1.7.2rc1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -62,14 +62,29 @@
 
 <p align="center">
   <img width="100%" alt="An example asset graph as rendered in the Dagster UI" src="https://raw.githubusercontent.com/dagster-io/dagster/master/.github/example-lineage.png">
 </p>
 
 Dagster is built to be used at every stage of the data development lifecycle - local development, unit tests, integration tests, staging environments, all the way up to production.
 
+## Special Event: Introducing Dagster+
+
+<p align="center">
+  <img width="100%" alt="Join us on April 17 (12PM ET) for a special event introducing Dagster+" src="https://i.imgur.com/1r7hOep.png">
+</p>
+
+Join us on April 17 (12PM ET) for a special event introducing Dagster+. [Register for our Dagster+ launch event here](https://dagster.io/events/dagster-plus-launch-event)
+
+In addition to the core open-source project, we are excited to announce Dagster+, the next generation of Dagster's cloud offering.
+
+- Find out how to weave data reliability and quality checks into the execution of your data pipelines.
+- See how diff-based branch deployments will accelerate your development cycle and cut extraneous compute costs.
+- Get a deep understanding of what is driving the cost of your data pipelines, then optimize to get the best cost/performance outcomes.
+- Enjoy the benefits of built-in data cataloging, and asset-level rich metadata.
+
 ## Quick Start:
 
 If you're new to Dagster, we recommend reading about its [core concepts](https://docs.dagster.io/concepts) or learning with the hands-on [tutorial](https://docs.dagster.io/tutorial).
 
 Dagster is available on PyPI and officially supports Python 3.8 through Python 3.12.
 
 ```bash
```

### Comparing `dagster-1.7.1/dagster/__init__.py` & `dagster-1.7.2rc1/dagster/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,14 +277,16 @@
     TextMetadataValue as TextMetadataValue,
     TimestampMetadataValue as TimestampMetadataValue,
     UrlMetadataValue as UrlMetadataValue,
 )
 from dagster._core.definitions.metadata.table import (
     TableColumn as TableColumn,
     TableColumnConstraints as TableColumnConstraints,
+    TableColumnDep as TableColumnDep,
+    TableColumnLineage as TableColumnLineage,
     TableConstraints as TableConstraints,
     TableRecord as TableRecord,
     TableSchema as TableSchema,
 )
 from dagster._core.definitions.multi_asset_sensor_definition import (
     MultiAssetSensorDefinition as MultiAssetSensorDefinition,
     MultiAssetSensorEvaluationContext as MultiAssetSensorEvaluationContext,
```

### Comparing `dagster-1.7.1/dagster/_annotations.py` & `dagster-1.7.2rc1/dagster/_annotations.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_api/get_server_id.py` & `dagster-1.7.2rc1/dagster/_api/get_server_id.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_api/list_repositories.py` & `dagster-1.7.2rc1/dagster/_api/list_repositories.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_api/notebook_data.py` & `dagster-1.7.2rc1/dagster/_api/notebook_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_api/snapshot_execution_plan.py` & `dagster-1.7.2rc1/dagster/_api/snapshot_execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_api/snapshot_job.py` & `dagster-1.7.2rc1/dagster/_api/snapshot_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_api/snapshot_partition.py` & `dagster-1.7.2rc1/dagster/_api/snapshot_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_api/snapshot_repository.py` & `dagster-1.7.2rc1/dagster/_api/snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_api/snapshot_schedule.py` & `dagster-1.7.2rc1/dagster/_api/snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_api/snapshot_sensor.py` & `dagster-1.7.2rc1/dagster/_api/snapshot_sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_check/README.md` & `dagster-1.7.2rc1/dagster/_check/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_check/__init__.py` & `dagster-1.7.2rc1/dagster/_check/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_cli/__init__.py` & `dagster-1.7.2rc1/dagster/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_cli/api.py` & `dagster-1.7.2rc1/dagster/_cli/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_cli/asset.py` & `dagster-1.7.2rc1/dagster/_cli/asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_cli/code_server.py` & `dagster-1.7.2rc1/dagster/_cli/code_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_cli/config_scaffolder.py` & `dagster-1.7.2rc1/dagster/_cli/config_scaffolder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_cli/debug.py` & `dagster-1.7.2rc1/dagster/_cli/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_cli/dev.py` & `dagster-1.7.2rc1/dagster/_cli/dev.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_cli/instance.py` & `dagster-1.7.2rc1/dagster/_cli/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_cli/job.py` & `dagster-1.7.2rc1/dagster/_cli/job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_cli/load_handle.py` & `dagster-1.7.2rc1/dagster/_cli/load_handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_cli/project.py` & `dagster-1.7.2rc1/dagster/_cli/project.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_cli/run.py` & `dagster-1.7.2rc1/dagster/_cli/run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_cli/schedule.py` & `dagster-1.7.2rc1/dagster/_cli/schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_cli/sensor.py` & `dagster-1.7.2rc1/dagster/_cli/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_cli/utils.py` & `dagster-1.7.2rc1/dagster/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_cli/workspace/cli_target.py` & `dagster-1.7.2rc1/dagster/_cli/workspace/cli_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/__init__.py` & `dagster-1.7.2rc1/dagster/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/config_schema.py` & `dagster-1.7.2rc1/dagster/_config/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/config_type.py` & `dagster-1.7.2rc1/dagster/_config/config_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/errors.py` & `dagster-1.7.2rc1/dagster/_config/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/evaluate_value_result.py` & `dagster-1.7.2rc1/dagster/_config/evaluate_value_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/field.py` & `dagster-1.7.2rc1/dagster/_config/field.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/field_utils.py` & `dagster-1.7.2rc1/dagster/_config/field_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/post_process.py` & `dagster-1.7.2rc1/dagster/_config/post_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/primitive_mapping.py` & `dagster-1.7.2rc1/dagster/_config/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/pythonic_config/__init__.py` & `dagster-1.7.2rc1/dagster/_config/pythonic_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/pythonic_config/attach_other_object_to_context.py` & `dagster-1.7.2rc1/dagster/_config/pythonic_config/attach_other_object_to_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/pythonic_config/config.py` & `dagster-1.7.2rc1/dagster/_config/pythonic_config/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/pythonic_config/conversion_utils.py` & `dagster-1.7.2rc1/dagster/_config/pythonic_config/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/pythonic_config/io_manager.py` & `dagster-1.7.2rc1/dagster/_config/pythonic_config/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/pythonic_config/pydantic_compat_layer.py` & `dagster-1.7.2rc1/dagster/_config/pythonic_config/pydantic_compat_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/pythonic_config/resource.py` & `dagster-1.7.2rc1/dagster/_config/pythonic_config/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/pythonic_config/type_check_utils.py` & `dagster-1.7.2rc1/dagster/_config/pythonic_config/type_check_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/pythonic_config/typing_utils.py` & `dagster-1.7.2rc1/dagster/_config/pythonic_config/typing_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/snap.py` & `dagster-1.7.2rc1/dagster/_config/snap.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/source.py` & `dagster-1.7.2rc1/dagster/_config/source.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/stack.py` & `dagster-1.7.2rc1/dagster/_config/stack.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/traversal_context.py` & `dagster-1.7.2rc1/dagster/_config/traversal_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/type_printer.py` & `dagster-1.7.2rc1/dagster/_config/type_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_config/validate.py` & `dagster-1.7.2rc1/dagster/_config/validate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/asset_graph_view/asset_graph_view.py` & `dagster-1.7.2rc1/dagster/_core/asset_graph_view/asset_graph_view.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/assets.py` & `dagster-1.7.2rc1/dagster/_core/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/code_pointer.py` & `dagster-1.7.2rc1/dagster/_core/code_pointer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/container_context/config.py` & `dagster-1.7.2rc1/dagster/_core/container_context/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/debug.py` & `dagster-1.7.2rc1/dagster/_core/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/decorator_utils.py` & `dagster-1.7.2rc1/dagster/_core/decorator_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/__init__.py` & `dagster-1.7.2rc1/dagster/_core/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/asset_check_evaluation.py` & `dagster-1.7.2rc1/dagster/_core/definitions/asset_check_evaluation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/asset_check_result.py` & `dagster-1.7.2rc1/dagster/_core/definitions/asset_check_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-from typing import TYPE_CHECKING, Mapping, NamedTuple, Optional
+from typing import TYPE_CHECKING, AbstractSet, Mapping, NamedTuple, Optional
 
 import dagster._check as check
 from dagster._annotations import PublicAttr
 from dagster._core.definitions.asset_check_evaluation import (
     AssetCheckEvaluation,
     AssetCheckEvaluationTargetMaterializationData,
 )
-from dagster._core.definitions.asset_check_spec import AssetCheckSeverity
+from dagster._core.definitions.asset_check_spec import (
+    AssetCheckKey,
+    AssetCheckSeverity,
+)
 from dagster._core.definitions.events import (
     AssetKey,
     CoercibleToAssetKey,
     MetadataValue,
     RawMetadataValue,
     normalize_metadata,
 )
@@ -71,54 +74,48 @@
             check_name=check.opt_str_param(check_name, "check_name"),
             passed=check.bool_param(passed, "passed"),
             metadata=normalized_metadata,
             severity=check.inst_param(severity, "severity", AssetCheckSeverity),
             description=check.opt_str_param(description, "description"),
         )
 
-    def to_asset_check_evaluation(
-        self, step_context: "StepExecutionContext"
-    ) -> AssetCheckEvaluation:
-        spec_check_names_by_asset_key = (
-            step_context.job_def.asset_layer.check_names_by_asset_key_by_node_handle.get(
-                step_context.node_handle.root
-            )
-        )
-
-        if not spec_check_names_by_asset_key:
+    def resolve_target_check_key(
+        self, check_names_by_asset_key: Optional[Mapping[AssetKey, AbstractSet[str]]]
+    ) -> AssetCheckKey:
+        if not check_names_by_asset_key:
             raise DagsterInvariantViolationError(
                 "Received unexpected AssetCheckResult. No AssetCheckSpecs were found for this step."
                 "You may need to set `check_specs` on the asset decorator, or you may be emitting an "
                 "AssetCheckResult that isn't in the subset passed in `context.selected_asset_check_keys`."
             )
 
-        asset_keys_with_specs = spec_check_names_by_asset_key.keys()
+        asset_keys_with_specs = check_names_by_asset_key.keys()
 
         if self.asset_key is not None:
             if self.asset_key not in asset_keys_with_specs:
                 raise DagsterInvariantViolationError(
                     "Received unexpected AssetCheckResult. It targets asset"
                     f" '{self.asset_key.to_user_string()}' which is not targeted by any of the"
                     " checks currently being evaluated. Targeted assets:"
                     f" {[asset_key.to_user_string() for asset_key in asset_keys_with_specs]}."
                 )
 
             resolved_asset_key = self.asset_key
 
         else:
-            if len(spec_check_names_by_asset_key) > 1:
+            if len(check_names_by_asset_key) > 1:
                 raise DagsterInvariantViolationError(
                     "AssetCheckResult didn't specify an asset key, but there are multiple assets"
                     " to choose from:"
-                    f" {[asset_key.to_user_string() for asset_key in spec_check_names_by_asset_key.keys()]}"
+                    f" {[asset_key.to_user_string() for asset_key in check_names_by_asset_key.keys()]}"
                 )
 
             resolved_asset_key = next(iter(asset_keys_with_specs))
 
-        check_names_with_specs = spec_check_names_by_asset_key[resolved_asset_key]
+        check_names_with_specs = check_names_by_asset_key[resolved_asset_key]
         if self.check_name is not None:
             if self.check_name not in check_names_with_specs:
                 raise DagsterInvariantViolationError(
                     "Received unexpected AssetCheckResult. No checks currently being evaluated"
                     f" target asset '{resolved_asset_key.to_user_string()}' and have name"
                     f" '{self.check_name}'. Checks being evaluated for this asset:"
                     f" {check_names_with_specs}"
@@ -131,15 +128,28 @@
                     "AssetCheckResult result didn't specify a check name, but there are multiple"
                     " checks to choose from for the this asset key:"
                     f" {check_names_with_specs}"
                 )
 
             resolved_check_name = next(iter(check_names_with_specs))
 
-        input_asset_info = step_context.get_input_asset_version_info(resolved_asset_key)
+        return AssetCheckKey(asset_key=resolved_asset_key, name=resolved_check_name)
+
+    def to_asset_check_evaluation(
+        self, step_context: "StepExecutionContext"
+    ) -> AssetCheckEvaluation:
+        check_names_by_asset_key = (
+            step_context.job_def.asset_layer.check_names_by_asset_key_by_node_handle.get(
+                step_context.node_handle.root
+            )
+        )
+
+        check_key = self.resolve_target_check_key(check_names_by_asset_key)
+
+        input_asset_info = step_context.get_input_asset_version_info(check_key.asset_key)
         from dagster._core.events import DagsterEventType
 
         if (
             input_asset_info is not None
             and input_asset_info.event_type == DagsterEventType.ASSET_MATERIALIZATION
         ):
             target_materialization_data = AssetCheckEvaluationTargetMaterializationData(
@@ -147,27 +157,15 @@
                 storage_id=input_asset_info.storage_id,
                 timestamp=input_asset_info.timestamp,
             )
         else:
             target_materialization_data = None
 
         return AssetCheckEvaluation(
-            check_name=resolved_check_name,
-            asset_key=resolved_asset_key,
+            check_name=check_key.name,
+            asset_key=check_key.asset_key,
             passed=self.passed,
             metadata=self.metadata,
             target_materialization_data=target_materialization_data,
             severity=self.severity,
             description=self.description,
         )
-
-    def get_spec_python_identifier(
-        self, *, asset_key: Optional[AssetKey] = None, check_name: Optional[str] = None
-    ) -> str:
-        """Returns a string uniquely identifying the asset check spec associated with this result.
-        This is used for the output name associated with an `AssetCheckResult`.
-        """
-        asset_key = asset_key or self.asset_key
-        check_name = check_name or self.check_name
-        assert asset_key is not None, "Asset key must be provided if not set on spec"
-        assert asset_key is not None, "Asset key must be provided if not set on spec"
-        return f"{asset_key.to_python_identifier()}_{self.check_name}"
```

### Comparing `dagster-1.7.1/dagster/_core/definitions/asset_check_spec.py` & `dagster-1.7.2rc1/dagster/_core/definitions/asset_check_spec.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/asset_checks.py` & `dagster-1.7.2rc1/dagster/_core/definitions/asset_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/asset_condition/asset_condition.py` & `dagster-1.7.2rc1/dagster/_core/definitions/asset_condition/asset_condition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 import functools
 import hashlib
-from abc import ABC, abstractmethod, abstractproperty
+from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Dict,
     FrozenSet,
     List,
     Mapping,
-    NamedTuple,
     Optional,
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
 import pendulum
 
 from dagster._annotations import experimental
 from dagster._core.definitions.events import AssetKey
 from dagster._core.definitions.metadata import MetadataMapping, MetadataValue
 from dagster._core.definitions.partition import AllPartitionsSubset
+from dagster._model import DagsterModel
 from dagster._serdes.serdes import PackableValue, whitelist_for_serdes
 
 from ..asset_subset import AssetSubset, ValidAssetSubset
+from ..auto_materialize_rule import AutoMaterializeRule
 
 if TYPE_CHECKING:
-    from ..auto_materialize_rule import AutoMaterializeRule
     from .asset_condition_evaluation_context import AssetConditionEvaluationContext
 
 
 T = TypeVar("T")
 
 
 @whitelist_for_serdes
-class HistoricalAllPartitionsSubsetSentinel(NamedTuple):
+class HistoricalAllPartitionsSubsetSentinel(DagsterModel):
     """Serializable indicator that this value was an AllPartitionsSubset at serialization time, but
     the partitions may have changed since that time.
     """
 
 
 @whitelist_for_serdes
-class AssetConditionSnapshot(NamedTuple):
+class AssetConditionSnapshot(DagsterModel):
     """A serializable snapshot of a node in the AutomationCondition tree."""
 
     class_name: str
     description: str
     unique_id: str
 
 
 @whitelist_for_serdes
-class AssetSubsetWithMetadata(NamedTuple):
+class AssetSubsetWithMetadata(DagsterModel):
     """An asset subset with metadata that corresponds to it."""
 
     subset: AssetSubset
     metadata: MetadataMapping
 
     @property
     def frozen_metadata(self) -> FrozenSet[Tuple[str, MetadataValue]]:
@@ -71,66 +71,16 @@
     if isinstance(candidate_subset, AssetSubset) and isinstance(
         candidate_subset.value, AllPartitionsSubset
     ):
         return HistoricalAllPartitionsSubsetSentinel()
     return candidate_subset
 
 
-class AssetConditionResult(NamedTuple):
-    condition: "AssetCondition"
-    start_timestamp: float
-    end_timestamp: float
-
-    true_subset: AssetSubset
-    candidate_subset: AssetSubset
-    subsets_with_metadata: Sequence[AssetSubsetWithMetadata]
-    extra_state: PackableValue
-
-    child_results: Sequence["AssetConditionResult"]
-
-    @staticmethod
-    def create_from_children(
-        context: "AssetConditionEvaluationContext",
-        true_subset: AssetSubset,
-        child_results: Sequence["AssetConditionResult"],
-    ) -> "AssetConditionResult":
-        """Returns a new AssetConditionEvaluation from the given child results."""
-        return AssetConditionResult(
-            condition=context.condition,
-            start_timestamp=context.start_timestamp,
-            end_timestamp=pendulum.now("UTC").timestamp(),
-            true_subset=true_subset,
-            candidate_subset=context.candidate_subset,
-            subsets_with_metadata=[],
-            child_results=child_results,
-            extra_state=None,
-        )
-
-    @staticmethod
-    def create(
-        context: "AssetConditionEvaluationContext",
-        true_subset: AssetSubset,
-        subsets_with_metadata: Sequence[AssetSubsetWithMetadata] = [],
-        extra_state: PackableValue = None,
-    ) -> "AssetConditionResult":
-        """Returns a new AssetConditionEvaluation from the given parameters."""
-        return AssetConditionResult(
-            condition=context.condition,
-            start_timestamp=context.start_timestamp,
-            end_timestamp=pendulum.now("UTC").timestamp(),
-            true_subset=true_subset,
-            candidate_subset=context.candidate_subset,
-            subsets_with_metadata=subsets_with_metadata,
-            child_results=[],
-            extra_state=extra_state,
-        )
-
-
 @whitelist_for_serdes
-class AssetConditionEvaluation(NamedTuple):
+class AssetConditionEvaluation(DagsterModel):
     """Serializable representation of the results of evaluating a node in the evaluation tree."""
 
     condition_snapshot: AssetConditionSnapshot
     start_timestamp: Optional[float]
     end_timestamp: Optional[float]
 
     true_subset: AssetSubset
@@ -140,15 +90,15 @@
     child_evaluations: Sequence["AssetConditionEvaluation"]
 
     @property
     def asset_key(self) -> AssetKey:
         return self.true_subset.asset_key
 
     @staticmethod
-    def from_result(result: AssetConditionResult) -> "AssetConditionEvaluation":
+    def from_result(result: "AssetConditionResult") -> "AssetConditionEvaluation":
         return AssetConditionEvaluation(
             condition_snapshot=result.condition.snapshot,
             start_timestamp=result.start_timestamp,
             end_timestamp=result.end_timestamp,
             true_subset=result.true_subset,
             candidate_subset=get_serializable_candidate_subset(result.candidate_subset),
             subsets_with_metadata=result.subsets_with_metadata,
@@ -193,15 +143,18 @@
     def get_requested_or_discarded_subset(self) -> AssetSubset:
         discarded_subset = self.discarded_subset()
         if discarded_subset is None:
             return self.true_subset
         else:
             # the true_subset and discarded_subset were created on the same tick, so they are
             # guaranteed to be compatible with each other
-            return ValidAssetSubset(*self.true_subset) | discarded_subset
+            return (
+                ValidAssetSubset(asset_key=self.asset_key, value=self.true_subset.value)
+                | discarded_subset
+            )
 
     def for_child(self, child_condition: "AssetCondition") -> Optional["AssetConditionEvaluation"]:
         """Returns the evaluation of a given child condition by finding the child evaluation that
         has an identical hash to the given condition.
         """
         child_unique_id = child_condition.snapshot.unique_id
         for child_evaluation in self.child_evaluations:
@@ -225,15 +178,16 @@
         discarded_subset = self.discarded_subset()
         if discarded_subset is None:
             return 0
         return discarded_subset.size
 
 
 @whitelist_for_serdes
-class AssetConditionEvaluationState(NamedTuple):
+@dataclass(frozen=True)
+class AssetConditionEvaluationState:
     """Incremental state calculated during the evaluation of an AssetCondition. This may be used
     on the subsequent evaluation to make the computation more efficient.
 
     Attributes:
         previous_evaluation: The computed AssetConditionEvaluation.
         previous_tick_evaluation_timestamp: The evaluation_timestamp at which the evaluation was performed.
         max_storage_id: The maximum storage ID over all events used in this computation.
@@ -253,22 +207,24 @@
 
     @property
     def true_subset(self) -> AssetSubset:
         return self.previous_evaluation.true_subset
 
     @staticmethod
     def create(
-        context: "AssetConditionEvaluationContext", root_result: AssetConditionResult
+        context: "AssetConditionEvaluationContext", root_result: "AssetConditionResult"
     ) -> "AssetConditionEvaluationState":
         """Convenience constructor to generate an AssetConditionEvaluationState from the root result
         and the context in which it was evaluated.
         """
 
         # flatten the extra state into a single dict
-        def _flatten_extra_state(r: AssetConditionResult) -> Mapping[str, PackableValue]:
+        def _flatten_extra_state(
+            r: AssetConditionResult,
+        ) -> Mapping[str, PackableValue]:
             extra_state: Dict[str, PackableValue] = (
                 {r.condition.unique_id: r.extra_state} if r.extra_state else {}
             )
             for child in r.child_results:
                 extra_state.update(_flatten_extra_state(child))
             return extra_state
 
@@ -286,15 +242,15 @@
         extra_state = self.extra_state_by_unique_id.get(condition.unique_id)
         if isinstance(extra_state, as_type):
             return extra_state
         return None
 
 
 @whitelist_for_serdes
-class AssetConditionEvaluationWithRunIds(NamedTuple):
+class AssetConditionEvaluationWithRunIds(DagsterModel):
     """A union of an AssetConditionEvaluation and the set of run IDs that have been launched in
     response to it.
     """
 
     evaluation: AssetConditionEvaluation
     run_ids: FrozenSet[str]
 
@@ -303,16 +259,15 @@
         return self.evaluation.asset_key
 
     @property
     def num_requested(self) -> int:
         return self.evaluation.true_subset.size
 
 
-@experimental
-class AssetCondition(ABC):
+class AssetCondition(ABC, DagsterModel):
     """An AssetCondition represents some state of the world that can influence if an asset
     partition should be materialized or not. AssetConditions can be combined to create
     new conditions using the `&` (and), `|` (or), and `~` (not) operators.
 
     Examples:
         .. code-block:: python
 
@@ -320,27 +275,31 @@
 
             # At least one parent is newer and no parent is missing.
             my_policy = AutoMaterializePolicy(
                 asset_condition = AssetCondition.parent_newer() & ~AssetCondition.parent_missing()
             )
     """
 
+    class Config:
+        keep_untouched = (functools.cached_property,)
+
     @property
     def unique_id(self) -> str:
         parts = [
             self.__class__.__name__,
             *[child.unique_id for child in self.children],
         ]
         return hashlib.md5("".join(parts).encode()).hexdigest()
 
     @abstractmethod
-    def evaluate(self, context: "AssetConditionEvaluationContext") -> AssetConditionResult:
+    def evaluate(self, context: "AssetConditionEvaluationContext") -> "AssetConditionResult":
         raise NotImplementedError()
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def description(self) -> str:
         raise NotImplementedError()
 
     def __and__(self, other: "AssetCondition") -> "AssetCondition":
         # group AndAssetConditions together
         if isinstance(self, AndAssetCondition):
             return AndAssetCondition(operands=[*self.operands, other])
@@ -395,160 +354,207 @@
         )
 
     @staticmethod
     def parent_newer() -> "AssetCondition":
         """Returns an AssetCondition that is true for an asset partition when at least one parent
         asset partition is newer than it.
         """
-        from ..auto_materialize_rule import AutoMaterializeRule
-
-        return RuleCondition(AutoMaterializeRule.materialize_on_parent_updated())
+        return RuleCondition(rule=AutoMaterializeRule.materialize_on_parent_updated())
 
     @staticmethod
     def missing() -> "AssetCondition":
         """Returns an AssetCondition that is true for an asset partition when it has never been
         materialized.
         """
         from ..auto_materialize_rule import AutoMaterializeRule
 
-        return RuleCondition(AutoMaterializeRule.materialize_on_missing())
+        return RuleCondition(rule=AutoMaterializeRule.materialize_on_missing())
 
     @staticmethod
     def parent_missing() -> "AssetCondition":
         """Returns an AssetCondition that is true for an asset partition when at least one parent
         asset partition has never been materialized or observed.
         """
         from ..auto_materialize_rule import AutoMaterializeRule
 
-        return RuleCondition(AutoMaterializeRule.skip_on_parent_missing())
+        return RuleCondition(rule=AutoMaterializeRule.skip_on_parent_missing())
 
     @staticmethod
     def updated_since_cron(cron_schedule: str, timezone: str = "UTC") -> "AssetCondition":
         """Returns an AssetCondition that is true for an asset partition when it has been updated
         since the latest tick of the given cron schedule. For partitioned assets with a time
         component, this can only be true for the the most recent partition.
         """
         from ..auto_materialize_rule import AutoMaterializeRule
 
-        return ~RuleCondition(AutoMaterializeRule.materialize_on_cron(cron_schedule, timezone))
+        return ~RuleCondition(rule=AutoMaterializeRule.materialize_on_cron(cron_schedule, timezone))
 
     @staticmethod
     def parents_updated_since_cron(cron_schedule: str, timezone: str = "UTC") -> "AssetCondition":
         """Returns an AssetCondition that is true for an asset partition when all parent asset
         partitions have been updated more recently than the latest tick of the given cron schedule.
         """
         from ..auto_materialize_rule import AutoMaterializeRule
 
         return ~RuleCondition(
-            AutoMaterializeRule.skip_on_not_all_parents_updated_since_cron(cron_schedule, timezone)
+            rule=AutoMaterializeRule.skip_on_not_all_parents_updated_since_cron(
+                cron_schedule, timezone
+            )
         )
 
 
 @experimental
 @whitelist_for_serdes
-@dataclass(frozen=True)
 class RuleCondition(AssetCondition):
     """This class represents the condition that a particular AutoMaterializeRule is satisfied."""
 
-    rule: "AutoMaterializeRule"
+    rule: AutoMaterializeRule
 
     @property
     def unique_id(self) -> str:
         parts = [self.rule.__class__.__name__, self.description]
         return hashlib.md5("".join(parts).encode()).hexdigest()
 
     @property
     def description(self) -> str:
         return self.rule.description
 
-    def evaluate(self, context: "AssetConditionEvaluationContext") -> AssetConditionResult:
+    def evaluate(self, context: "AssetConditionEvaluationContext") -> "AssetConditionResult":
         context.root_context.daemon_context.logger.debug(
             f"Evaluating rule: {self.rule.to_snapshot()}"
         )
         evaluation_result = self.rule.evaluate_for_asset(context)
         context.root_context.daemon_context.logger.debug(
             f"Rule returned {evaluation_result.true_subset.size} partitions "
             f"({evaluation_result.end_timestamp - evaluation_result.start_timestamp:.2f} seconds)"
         )
         return evaluation_result
 
 
 @experimental
 @whitelist_for_serdes
-@dataclass(frozen=True)
 class AndAssetCondition(AssetCondition):
     """This class represents the condition that all of its children evaluate to true."""
 
     operands: Sequence[AssetCondition]
 
     @property
     def children(self) -> Sequence[AssetCondition]:
         return self.operands
 
     @property
     def description(self) -> str:
         return "All of"
 
-    def evaluate(self, context: "AssetConditionEvaluationContext") -> AssetConditionResult:
+    def evaluate(self, context: "AssetConditionEvaluationContext") -> "AssetConditionResult":
         child_results: List[AssetConditionResult] = []
         true_subset = context.candidate_subset
         for child in self.children:
             child_context = context.for_child(condition=child, candidate_subset=true_subset)
             child_result = child.evaluate(child_context)
             child_results.append(child_result)
             true_subset &= child_result.true_subset
         return AssetConditionResult.create_from_children(context, true_subset, child_results)
 
 
 @experimental
 @whitelist_for_serdes
-@dataclass(frozen=True)
 class OrAssetCondition(AssetCondition):
     """This class represents the condition that any of its children evaluate to true."""
 
     operands: Sequence[AssetCondition]
 
     @property
     def children(self) -> Sequence[AssetCondition]:
         return self.operands
 
     @property
     def description(self) -> str:
         return "Any of"
 
-    def evaluate(self, context: "AssetConditionEvaluationContext") -> AssetConditionResult:
+    def evaluate(self, context: "AssetConditionEvaluationContext") -> "AssetConditionResult":
         child_results: List[AssetConditionResult] = []
         true_subset = context.empty_subset()
         for child in self.children:
             child_context = context.for_child(
                 condition=child, candidate_subset=context.candidate_subset
             )
             child_result = child.evaluate(child_context)
             child_results.append(child_result)
             true_subset |= child_result.true_subset
         return AssetConditionResult.create_from_children(context, true_subset, child_results)
 
 
 @experimental
 @whitelist_for_serdes
-@dataclass(frozen=True)
 class NotAssetCondition(AssetCondition):
     """This class represents the condition that none of its children evaluate to true."""
 
     operand: AssetCondition
 
     @property
     def description(self) -> str:
         return "Not"
 
     @property
     def children(self) -> Sequence[AssetCondition]:
         return [self.operand]
 
-    def evaluate(self, context: "AssetConditionEvaluationContext") -> AssetConditionResult:
+    def evaluate(self, context: "AssetConditionEvaluationContext") -> "AssetConditionResult":
         child_context = context.for_child(
             condition=self.operand, candidate_subset=context.candidate_subset
         )
         child_result = self.operand.evaluate(child_context)
         true_subset = context.candidate_subset - child_result.true_subset
 
         return AssetConditionResult.create_from_children(context, true_subset, [child_result])
+
+
+@dataclass(frozen=True)
+class AssetConditionResult:
+    condition: AssetCondition
+    start_timestamp: float
+    end_timestamp: float
+
+    true_subset: AssetSubset
+    candidate_subset: AssetSubset
+    subsets_with_metadata: Sequence[AssetSubsetWithMetadata]
+
+    extra_state: PackableValue
+    child_results: Sequence["AssetConditionResult"]
+
+    @staticmethod
+    def create_from_children(
+        context: "AssetConditionEvaluationContext",
+        true_subset: AssetSubset,
+        child_results: Sequence["AssetConditionResult"],
+    ) -> "AssetConditionResult":
+        """Returns a new AssetConditionEvaluation from the given child results."""
+        return AssetConditionResult(
+            condition=context.condition,
+            start_timestamp=context.start_timestamp,
+            end_timestamp=pendulum.now("UTC").timestamp(),
+            true_subset=true_subset,
+            candidate_subset=context.candidate_subset,
+            subsets_with_metadata=[],
+            child_results=child_results,
+            extra_state=None,
+        )
+
+    @staticmethod
+    def create(
+        context: "AssetConditionEvaluationContext",
+        true_subset: AssetSubset,
+        subsets_with_metadata: Sequence[AssetSubsetWithMetadata] = [],
+        extra_state: PackableValue = None,
+    ) -> "AssetConditionResult":
+        """Returns a new AssetConditionEvaluation from the given parameters."""
+        return AssetConditionResult(
+            condition=context.condition,
+            start_timestamp=context.start_timestamp,
+            end_timestamp=pendulum.now("UTC").timestamp(),
+            true_subset=true_subset,
+            candidate_subset=context.candidate_subset,
+            subsets_with_metadata=subsets_with_metadata,
+            child_results=[],
+            extra_state=extra_state,
+        )
```

### Comparing `dagster-1.7.1/dagster/_core/definitions/asset_condition/asset_condition_evaluation_context.py` & `dagster-1.7.2rc1/dagster/_core/definitions/asset_condition/asset_condition_evaluation_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
         for parent_key in self.asset_graph.get(self.asset_key).parent_keys:
             if not self.materializable_in_same_run(self.asset_key, parent_key):
                 continue
             parent_info = self.evaluation_state_by_key.get(parent_key)
             if not parent_info:
                 continue
             parent_subset = parent_info.true_subset.as_valid(self.partitions_def)
-            subset |= parent_subset._replace(asset_key=self.asset_key)
+            subset |= parent_subset.copy(update={"asset_key": self.asset_key})
         return subset
 
     @functools.cached_property
     @root_property
     def materialized_since_previous_tick_subset(self) -> ValidAssetSubset:
         """Returns the set of asset partitions that were materialized since the previous tick."""
         return AssetSubset.from_asset_partitions_set(
@@ -389,14 +389,14 @@
         true_subset = self.empty_subset()
         for subset in mapping.values():
             true_subset |= subset
 
         return (
             self.candidate_subset & true_subset,
             [
-                AssetSubsetWithMetadata(subset, dict(metadata))
+                AssetSubsetWithMetadata(subset=subset, metadata=dict(metadata))
                 for metadata, subset in mapping.items()
             ],
         )
 
     def empty_subset(self) -> ValidAssetSubset:
         return AssetSubset.empty(self.asset_key, self.partitions_def)
```

### Comparing `dagster-1.7.1/dagster/_core/definitions/asset_daemon_context.py` & `dagster-1.7.2rc1/dagster/_core/definitions/asset_daemon_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import dataclasses
 import datetime
 import logging
 import time
 from collections import defaultdict
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
@@ -273,20 +274,23 @@
 
                     # make sure that the true_subset of the neighbor is accurate -- when it was
                     # evaluated it may have had a different requested AssetSubset. however, because
                     # all these neighbors must be executed as a unit, we need to union together
                     # the subset of all required neighbors
                     if neighbor_key in evaluation_state_by_key:
                         neighbor_evaluation_state = evaluation_state_by_key[neighbor_key]
-                        evaluation_state_by_key[neighbor_key] = neighbor_evaluation_state._replace(
-                            previous_evaluation=neighbor_evaluation_state.previous_evaluation._replace(
-                                true_subset=neighbor_evaluation_state.true_subset._replace(
-                                    asset_key=neighbor_key
-                                )
-                            )
+                        evaluation_state_by_key[neighbor_key] = dataclasses.replace(
+                            neighbor_evaluation_state,
+                            previous_evaluation=neighbor_evaluation_state.previous_evaluation.copy(
+                                update={
+                                    "true_subset": neighbor_evaluation_state.true_subset.copy(
+                                        update={"asset_key": neighbor_key}
+                                    )
+                                }
+                            ),
                         )
                     to_request |= {
                         ap._replace(asset_key=neighbor_key)
                         for ap in evaluation_state.true_subset.asset_partitions
                     }
 
         return (list(evaluation_state_by_key.values()), to_request)
```

### Comparing `dagster-1.7.1/dagster/_core/definitions/asset_daemon_cursor.py` & `dagster-1.7.2rc1/dagster/_core/definitions/asset_daemon_cursor.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 
     return AssetConditionEvaluationState(
         previous_evaluation=latest_evaluation,
         previous_tick_evaluation_timestamp=latest_timestamp,
         max_storage_id=latest_storage_id,
         # the only information we need to preserve from the previous cursor is the handled subset
         extra_state_by_unique_id={
-            RuleCondition(MaterializeOnMissingRule()).unique_id: handled_root_subset,
+            RuleCondition(rule=MaterializeOnMissingRule()).unique_id: handled_root_subset,
         }
         if handled_root_subset and handled_root_subset.size > 0
         else {},
     )
 
 
 def backcompat_deserialize_asset_daemon_cursor_str(
@@ -237,15 +237,17 @@
     )
     for asset_key in cursor_keys:
         latest_evaluation_result = latest_evaluation_by_asset_key.get(asset_key)
         # create a placeholder evaluation result if we don't have one
         if not latest_evaluation_result:
             partitions_def = asset_graph.get(asset_key).partitions_def if asset_graph else None
             latest_evaluation_result = AssetConditionEvaluation(
-                condition_snapshot=AssetConditionSnapshot("", "", ""),
+                condition_snapshot=AssetConditionSnapshot(
+                    class_name="", description="", unique_id=""
+                ),
                 true_subset=AssetSubset.empty(asset_key, partitions_def),
                 candidate_subset=AssetSubset.empty(asset_key, partitions_def),
                 start_timestamp=None,
                 end_timestamp=None,
                 subsets_with_metadata=[],
                 child_evaluations=[],
             )
```

### Comparing `dagster-1.7.1/dagster/_core/definitions/asset_dep.py` & `dagster-1.7.2rc1/dagster/_core/definitions/asset_dep.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/asset_graph.py` & `dagster-1.7.2rc1/dagster/_core/definitions/asset_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,20 +124,18 @@
             {self.key}
             if len(self.assets_def.keys) <= 1 or self.assets_def.can_subset
             else self.assets_def.keys
         )
 
     @property
     def execution_set_asset_and_check_keys(self) -> AbstractSet[AssetKeyOrCheckKey]:
-        if self.assets_def.can_subset or (
-            len(self.assets_def.keys) <= 1 and not len(self.assets_def.check_keys) > 0
-        ):
+        if self.assets_def.can_subset:
             return {self.key}
         else:
-            return {*self.assets_def.keys, *self.assets_def.check_keys}
+            return self.assets_def.asset_and_check_keys
 
     ##### ASSET GRAPH SPECIFIC INTERFACE
 
     @property
     def execution_type(self) -> AssetExecutionType:
         return self.assets_def.execution_type
```

### Comparing `dagster-1.7.1/dagster/_core/definitions/asset_graph_differ.py` & `dagster-1.7.2rc1/dagster/_core/definitions/asset_graph_differ.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 
 class ChangeReason(Enum):
     NEW = "NEW"
     CODE_VERSION = "CODE_VERSION"
     DEPENDENCIES = "DEPENDENCIES"
     PARTITIONS_DEFINITION = "PARTITIONS_DEFINITION"
+    TAGS = "TAGS"
+    METADATA = "METADATA"
 
 
 def _get_external_repo_from_context(
     context: BaseWorkspaceRequestContext, code_location_name: str, repository_name: str
 ) -> Optional[ExternalRepository]:
     """Returns the ExternalRepository specified by the code location name and repository name
     for the provided workspace context. If the repository doesn't exist, return None.
@@ -115,42 +117,42 @@
             # if the base asset graph is None, it is because the the asset graph in the branch deployment
             # is new and doesn't exist in the base deployment. Thus all assets are new.
             return [ChangeReason.NEW]
 
         if asset_key not in self.base_asset_graph.all_asset_keys:
             return [ChangeReason.NEW]
 
+        branch_asset = self.branch_asset_graph.get(asset_key)
+        base_asset = self.base_asset_graph.get(asset_key)
+
         changes = []
-        if (
-            self.branch_asset_graph.get(asset_key).code_version
-            != self.base_asset_graph.get(asset_key).code_version
-        ):
+        if branch_asset.code_version != base_asset.code_version:
             changes.append(ChangeReason.CODE_VERSION)
 
-        if (
-            self.branch_asset_graph.get(asset_key).parent_keys
-            != self.base_asset_graph.get(asset_key).parent_keys
-        ):
+        if branch_asset.parent_keys != base_asset.parent_keys:
             changes.append(ChangeReason.DEPENDENCIES)
         else:
             # if the set of upstream dependencies is different, then we don't need to check if the partition mappings
             # for dependencies have changed since ChangeReason.DEPENDENCIES is already in the list of changes
-            for upstream_asset in self.branch_asset_graph.get(asset_key).parent_keys:
+            for upstream_asset in branch_asset.parent_keys:
                 if self.branch_asset_graph.get_partition_mapping(
                     asset_key, upstream_asset
                 ) != self.base_asset_graph.get_partition_mapping(asset_key, upstream_asset):
                     changes.append(ChangeReason.DEPENDENCIES)
                     break
 
-        if (
-            self.branch_asset_graph.get(asset_key).partitions_def
-            != self.base_asset_graph.get(asset_key).partitions_def
-        ):
+        if branch_asset.partitions_def != base_asset.partitions_def:
             changes.append(ChangeReason.PARTITIONS_DEFINITION)
 
+        if branch_asset.tags != base_asset.tags:
+            changes.append(ChangeReason.TAGS)
+
+        if branch_asset.metadata != base_asset.metadata:
+            changes.append(ChangeReason.METADATA)
+
         return changes
 
     def get_changes_for_asset(self, asset_key: "AssetKey") -> Sequence[ChangeReason]:
         """Returns list of ChangeReasons for asset_key as compared to the base deployment."""
         return self._compare_base_and_branch_assets(asset_key)
 
     @property
```

### Comparing `dagster-1.7.1/dagster/_core/definitions/asset_graph_subset.py` & `dagster-1.7.2rc1/dagster/_core/definitions/asset_graph_subset.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,16 +274,19 @@
 
         partitions_def_class_names_by_asset_key = serialized_dict.get(
             "partitions_def_class_names_by_asset_key", {}
         )
 
         for key, value in serialized_dict["partitions_subsets_by_asset_key"].items():
             asset_key = AssetKey.from_user_string(key)
-            partitions_def = asset_graph.get(asset_key).partitions_def
+            if not asset_graph.has(asset_key):
+                # Asset had a definition at storage time, but no longer does
+                return False
 
+            partitions_def = asset_graph.get(asset_key).partitions_def
             if partitions_def is None:
                 # Asset had a partitions definition at storage time, but no longer does
                 return False
 
             if not partitions_def.can_deserialize_subset(
                 value,
                 serialized_partitions_def_unique_id=serializable_partitions_ids.get(key),
```

### Comparing `dagster-1.7.1/dagster/_core/definitions/asset_in.py` & `dagster-1.7.2rc1/dagster/_core/definitions/asset_in.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/asset_job.py` & `dagster-1.7.2rc1/dagster/_core/definitions/asset_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/asset_key.py` & `dagster-1.7.2rc1/dagster/_core/definitions/asset_key.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/asset_layer.py` & `dagster-1.7.2rc1/dagster/_core/definitions/asset_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/asset_out.py` & `dagster-1.7.2rc1/dagster/_core/definitions/asset_out.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/asset_selection.py` & `dagster-1.7.2rc1/dagster/_core/definitions/asset_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/asset_sensor_definition.py` & `dagster-1.7.2rc1/dagster/_core/definitions/asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/asset_spec.py` & `dagster-1.7.2rc1/dagster/_core/definitions/asset_spec.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/asset_subset.py` & `dagster-1.7.2rc1/dagster/_core/definitions/asset_subset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import datetime
 import operator
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Any,
     Callable,
-    NamedTuple,
     Optional,
     Union,
     cast,
 )
 
 import dagster._check as check
 from dagster._core.definitions.events import AssetKey, AssetKeyPartitionKey
@@ -17,38 +16,39 @@
     AllPartitionsSubset,
     PartitionsDefinition,
     PartitionsSubset,
 )
 from dagster._core.definitions.time_window_partitions import (
     BaseTimeWindowPartitionsSubset,
 )
+from dagster._model import DagsterModel
 from dagster._serdes.serdes import (
-    NamedTupleSerializer,
+    PydanticModelSerializer,
     whitelist_for_serdes,
 )
 
 if TYPE_CHECKING:
     from dagster._core.instance import DynamicPartitionsStore
 
 
-class AssetSubsetSerializer(NamedTupleSerializer):
+class AssetSubsetSerializer(PydanticModelSerializer):
     """Ensures that the inner PartitionsSubset is converted to a serializable form if necessary."""
 
     def get_storage_name(self) -> str:
         # override this method so all ValidAssetSubsets are serialzied as AssetSubsets
         return "AssetSubset"
 
     def before_pack(self, value: "AssetSubset") -> "AssetSubset":
         if value.is_partitioned:
-            return value._replace(value=value.subset_value.to_serializable_subset())
+            return value.copy(update={"value": value.subset_value.to_serializable_subset()})
         return value
 
 
 @whitelist_for_serdes(serializer=AssetSubsetSerializer)
-class AssetSubset(NamedTuple):
+class AssetSubset(DagsterModel):
     """Represents a set of AssetKeyPartitionKeys for a given AssetKey. For partitioned assets, this
     class uses a PartitionsSubset to represent the set of partitions, enabling lazy evaluation of the
     underlying partition keys. For unpartitioned assets, this class uses a bool to represent whether
     the asset is present or not.
     """
 
     asset_key: AssetKey
@@ -105,15 +105,15 @@
             return self.is_partitioned == other.is_partitioned
 
     def as_valid(self, partitions_def: Optional[PartitionsDefinition]) -> "ValidAssetSubset":
         """Converts this AssetSubset to a ValidAssetSubset by returning a copy of this AssetSubset
         if it is compatible with the given PartitionsDefinition, otherwise returns an empty subset.
         """
         if self._is_compatible_with_partitions_def(partitions_def):
-            return ValidAssetSubset(*self)
+            return ValidAssetSubset(asset_key=self.asset_key, value=self.value)
         else:
             return ValidAssetSubset.empty(self.asset_key, partitions_def)
 
     @staticmethod
     def all(
         asset_key: AssetKey,
         partitions_def: Optional[PartitionsDefinition],
@@ -173,14 +173,21 @@
         if not self.is_partitioned:
             return (
                 item.asset_key == self.asset_key and item.partition_key is None and self.bool_value
             )
         else:
             return item.asset_key == self.asset_key and item.partition_key in self.subset_value
 
+    def dict(self, **kwargs) -> dict:
+        # Must be overridden as the Pydantic implementation errors when encountering NamedTuples
+        # which have different fields than their __new__ method, which TimeWindowPartitionsSubset
+        # unfortunately has.
+        # This can likely be removed once TimeWindowPartitionsSubset is converted into a DagsterModel
+        return {"asset_key": self.asset_key, "value": self.value}
+
 
 @whitelist_for_serdes(serializer=AssetSubsetSerializer)
 class ValidAssetSubset(AssetSubset):
     """Represents an AssetSubset which is known to be compatible with the current PartitionsDefinition
     of the asset represents.
 
     This class serializes to a regular AssetSubset, as it is unknown if this value will still be
@@ -195,34 +202,34 @@
         self,
         partitions_def: Optional[PartitionsDefinition],
         current_time: Optional[datetime.datetime] = None,
         dynamic_partitions_store: Optional["DynamicPartitionsStore"] = None,
     ) -> "ValidAssetSubset":
         """Returns the AssetSubset containing all asset partitions which are not in this AssetSubset."""
         if partitions_def is None:
-            return self._replace(value=not self.bool_value)
+            return self.copy(update={"value": not self.bool_value})
         else:
             value = partitions_def.subset_with_partition_keys(
                 self.subset_value.get_partition_keys_not_in_subset(
                     partitions_def,
                     current_time=current_time,
                     dynamic_partitions_store=dynamic_partitions_store,
                 )
             )
-            return self._replace(value=value)
+            return self.copy(update={"value": value})
 
     def _oper(self, other: "ValidAssetSubset", oper: Callable[..., Any]) -> "ValidAssetSubset":
         value = oper(self.value, other.value)
-        return self._replace(value=value)
+        return self.copy(update={"value": value})
 
     def __sub__(self, other: AssetSubset) -> "ValidAssetSubset":
         """Returns an AssetSubset representing self.asset_partitions - other.asset_partitions."""
         valid_other = self.get_valid(other)
         if not self.is_partitioned:
-            return self._replace(value=self.bool_value and not valid_other.bool_value)
+            return self.copy(update={"value": self.bool_value and not valid_other.bool_value})
         return self._oper(valid_other, operator.sub)
 
     def __and__(self, other: AssetSubset) -> "ValidAssetSubset":
         """Returns an AssetSubset representing self.asset_partitions & other.asset_partitions."""
         return self._oper(self.get_valid(other), operator.and_)
 
     def __or__(self, other: AssetSubset) -> "ValidAssetSubset":
@@ -230,14 +237,18 @@
         return self._oper(self.get_valid(other), operator.or_)
 
     def get_valid(self, other: AssetSubset) -> "ValidAssetSubset":
         """Creates a ValidAssetSubset from the given AssetSubset by returning a copy of the given
         AssetSubset if it is compatible with this AssetSubset, otherwise returns an empty subset.
         """
         if self._is_compatible_with_subset(other):
-            return ValidAssetSubset(*other)
+            return ValidAssetSubset(asset_key=other.asset_key, value=other.value)
         else:
-            return self._replace(
+            return self.copy(
                 # unfortunately, this is the best way to get an empty partitions subset of an unknown
                 # type if you don't have access to the partitions definition
-                value=(self.subset_value - self.subset_value) if self.is_partitioned else False
+                update={
+                    "value": (self.subset_value - self.subset_value)
+                    if self.is_partitioned
+                    else False
+                }
             )
```

### Comparing `dagster-1.7.1/dagster/_core/definitions/assets.py` & `dagster-1.7.2rc1/dagster/_core/definitions/assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1112,14 +1112,23 @@
             if key == asset_key:
                 return output_name
 
         raise DagsterInvariantViolationError(
             f"Asset key {key.to_user_string()} not found in AssetsDefinition"
         )
 
+    def get_output_name_for_asset_check_key(self, key: AssetCheckKey) -> str:
+        for output_name, spec in self._check_specs_by_output_name.items():
+            if key == spec.key:
+                return output_name
+
+        raise DagsterInvariantViolationError(
+            f"Asset check key {key.to_user_string()} not found in AssetsDefinition"
+        )
+
     def get_op_def_for_asset_key(self, key: AssetKey) -> OpDefinition:
         """If this is an op-backed asset, returns the op def. If it's a graph-backed asset,
         returns the op def within the graph that produces the given asset key.
         """
         output_name = self.get_output_name_for_asset_key(key)
         return self.node_def.resolve_output_to_origin_op_def(output_name)
```

### Comparing `dagster-1.7.1/dagster/_core/definitions/auto_materialize_policy.py` & `dagster-1.7.2rc1/dagster/_core/definitions/auto_materialize_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,17 +307,17 @@
             operands=[
                 rule.to_asset_condition()
                 for rule in sorted(self.skip_rules, key=lambda rule: rule.description)
             ]
         )
         children = [
             materialize_condition,
-            NotAssetCondition(skip_condition),
+            NotAssetCondition(operand=skip_condition),
         ]
         if self.max_materializations_per_minute:
             discard_condition = DiscardOnMaxMaterializationsExceededRule(
                 self.max_materializations_per_minute
             ).to_asset_condition()
-            children.append(NotAssetCondition(discard_condition))
+            children.append(NotAssetCondition(operand=discard_condition))
 
         # results in an expression of the form (m1 | m2 | ... | mn) & ~(s1 | s2 | ... | sn) & ~d
-        return AndAssetCondition(children)
+        return AndAssetCondition(operands=children)
```

### Comparing `dagster-1.7.1/dagster/_core/definitions/auto_materialize_rule.py` & `dagster-1.7.2rc1/dagster/_core/definitions/auto_materialize_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,23 +42,24 @@
 )
 from dagster._utils.schedules import (
     cron_string_iterator,
     is_valid_cron_string,
     reverse_cron_string_iterator,
 )
 
-from .asset_condition.asset_condition_evaluation_context import AssetConditionEvaluationContext
 from .base_asset_graph import sort_key_for_asset_partition
 
 if TYPE_CHECKING:
     from dagster._core.definitions.asset_condition.asset_condition import (
         AssetCondition,
         AssetConditionResult,
     )
 
+    from .asset_condition.asset_condition_evaluation_context import AssetConditionEvaluationContext
+
 
 class AutoMaterializeRule(ABC):
     """An AutoMaterializeRule defines a bit of logic which helps determine if a materialization
     should be kicked off for a given asset partition.
 
     Each rule can have one of two decision types, `MATERIALIZE` (indicating that an asset partition
     should be materialized) or `SKIP` (indicating that the asset partition should not be
@@ -84,15 +85,15 @@
         """Converts this AutoMaterializeRule into an AssetCondition."""
         from .asset_condition.asset_condition import RuleCondition
 
         return RuleCondition(rule=self)
 
     @abstractmethod
     def evaluate_for_asset(
-        self, context: AssetConditionEvaluationContext
+        self, context: "AssetConditionEvaluationContext"
     ) -> "AssetConditionResult":
         """The core evaluation function for the rule. This function takes in a context object and
         returns a mapping from evaluated rules to the set of asset partitions that the rule applies
         to.
         """
         ...
 
@@ -271,15 +272,15 @@
         return AutoMaterializeDecisionType.MATERIALIZE
 
     @property
     def description(self) -> str:
         return "required to meet this or downstream asset's freshness policy"
 
     def evaluate_for_asset(
-        self, context: AssetConditionEvaluationContext
+        self, context: "AssetConditionEvaluationContext"
     ) -> "AssetConditionResult":
         from .asset_condition.asset_condition import AssetConditionResult
 
         true_subset, subsets_with_metadata = freshness_evaluation_results_for_asset_key(
             context.root_context
         )
         return AssetConditionResult.create(context, true_subset, subsets_with_metadata)
@@ -298,15 +299,15 @@
         return AutoMaterializeDecisionType.MATERIALIZE
 
     @property
     def description(self) -> str:
         return f"not materialized since last cron schedule tick of '{self.cron_schedule}' (timezone: {self.timezone})"
 
     def missed_cron_ticks(
-        self, context: AssetConditionEvaluationContext
+        self, context: "AssetConditionEvaluationContext"
     ) -> Sequence[datetime.datetime]:
         """Returns the cron ticks which have been missed since the previous cursor was generated."""
         # if it's the first time evaluating this rule, then just count the latest tick as missed
         if not context.previous_evaluation or not context.previous_evaluation_timestamp:
             previous_dt = next(
                 reverse_cron_string_iterator(
                     end_timestamp=context.evaluation_time.timestamp(),
@@ -323,15 +324,15 @@
         ):
             if dt > context.evaluation_time:
                 break
             missed_ticks.append(dt)
         return missed_ticks
 
     def get_new_candidate_asset_partitions(
-        self, context: AssetConditionEvaluationContext, missed_ticks: Sequence[datetime.datetime]
+        self, context: "AssetConditionEvaluationContext", missed_ticks: Sequence[datetime.datetime]
     ) -> AbstractSet[AssetKeyPartitionKey]:
         if not missed_ticks:
             return set()
 
         partitions_def = context.partitions_def
         if partitions_def is None:
             return {AssetKeyPartitionKey(context.asset_key)}
@@ -384,15 +385,15 @@
         else:
             return {
                 AssetKeyPartitionKey(context.asset_key, time_partition_key)
                 for time_partition_key in missed_time_partition_keys
             }
 
     def evaluate_for_asset(
-        self, context: AssetConditionEvaluationContext
+        self, context: "AssetConditionEvaluationContext"
     ) -> "AssetConditionResult":
         from .asset_condition.asset_condition import AssetConditionResult
 
         missed_ticks = self.missed_cron_ticks(context)
         new_asset_partitions = self.get_new_candidate_asset_partitions(context, missed_ticks)
 
         # if it's the first time evaluating this rule, must query for the actual subset that has
@@ -433,15 +434,15 @@
 
     @property
     def description(self) -> str:
         return f"latest run includes required tags: {self.latest_run_required_tags}"
 
     def passes(
         self,
-        context: AssetConditionEvaluationContext,
+        context: "AssetConditionEvaluationContext",
         asset_partitions: Iterable[AssetKeyPartitionKey],
     ) -> Iterable[AssetKeyPartitionKey]:
         if self.latest_run_required_tags is None:
             return asset_partitions
 
         will_update_asset_partitions: Set[AssetKeyPartitionKey] = set()
 
@@ -513,15 +514,15 @@
         base = "upstream data has changed since latest materialization"
         if self.updated_parent_filter is not None:
             return f"{base} and matches filter '{self.updated_parent_filter.description}'"
         else:
             return base
 
     def evaluate_for_asset(
-        self, context: AssetConditionEvaluationContext
+        self, context: "AssetConditionEvaluationContext"
     ) -> "AssetConditionResult":
         """Evaluates the set of asset partitions of this asset whose parents have been updated,
         or will update on this tick.
         """
         from .asset_condition.asset_condition import AssetConditionResult
 
         asset_partitions_by_updated_parents: Mapping[
@@ -617,15 +618,15 @@
     def decision_type(self) -> AutoMaterializeDecisionType:
         return AutoMaterializeDecisionType.MATERIALIZE
 
     @property
     def description(self) -> str:
         return "materialization is missing"
 
-    def get_handled_subset(self, context: AssetConditionEvaluationContext) -> AssetSubset:
+    def get_handled_subset(self, context: "AssetConditionEvaluationContext") -> AssetSubset:
         """Returns the AssetSubset which has been handled (materialized, requested, or discarded).
         Accounts for cases in which the partitions definition may have changed between ticks.
         """
         previous_handled_subset = (
             context.previous_evaluation_state.get_extra_state(context.condition, AssetSubset)
             if context.previous_evaluation_state
             else None
@@ -634,15 +635,15 @@
         return (
             context.materialized_since_previous_tick_subset
             | context.previous_tick_requested_subset
             | previous_handled_subset
         )
 
     def evaluate_for_asset(
-        self, context: AssetConditionEvaluationContext
+        self, context: "AssetConditionEvaluationContext"
     ) -> "AssetConditionResult":
         """Evaluates the set of asset partitions for this asset which are missing and were not
         previously discarded.
         """
         from .asset_condition.asset_condition import AssetConditionResult
 
         if context.asset_key in context.asset_graph.root_executable_asset_keys:
@@ -710,15 +711,15 @@
         return AutoMaterializeDecisionType.SKIP
 
     @property
     def description(self) -> str:
         return "waiting on upstream data to be up to date"
 
     def evaluate_for_asset(
-        self, context: AssetConditionEvaluationContext
+        self, context: "AssetConditionEvaluationContext"
     ) -> "AssetConditionResult":
         from .asset_condition.asset_condition import AssetConditionResult
 
         asset_partitions_by_evaluation_data = defaultdict(set)
 
         # only need to evaluate net-new candidates and candidates whose parents have changed
         subset_to_evaluate = (
@@ -757,15 +758,15 @@
 
     @property
     def description(self) -> str:
         return "waiting on upstream data to be present"
 
     def evaluate_for_asset(
         self,
-        context: AssetConditionEvaluationContext,
+        context: "AssetConditionEvaluationContext",
     ) -> "AssetConditionResult":
         from .asset_condition.asset_condition import AssetConditionResult
 
         asset_partitions_by_evaluation_data = defaultdict(set)
 
         # only need to evaluate net-new candidates and candidates whose parents have changed
         subset_to_evaluate = (
@@ -829,15 +830,15 @@
         if self.require_update_for_all_parent_partitions is False:
             return "waiting on upstream data to be updated"
         else:
             return "waiting until all upstream partitions are updated"
 
     def evaluate_for_asset(
         self,
-        context: AssetConditionEvaluationContext,
+        context: "AssetConditionEvaluationContext",
     ) -> "AssetConditionResult":
         from .asset_condition.asset_condition import AssetConditionResult
 
         asset_partitions_by_evaluation_data = defaultdict(set)
 
         # only need to evaluate net-new candidates and candidates whose parents have changed
         subset_to_evaluate = (
@@ -902,15 +903,15 @@
     def decision_type(self) -> AutoMaterializeDecisionType:
         return AutoMaterializeDecisionType.SKIP
 
     @property
     def description(self) -> str:
         return f"waiting until all upstream assets have updated since the last cron schedule tick of '{self.cron_schedule}' (timezone: {self.timezone})"
 
-    def passed_time_window(self, context: AssetConditionEvaluationContext) -> TimeWindow:
+    def passed_time_window(self, context: "AssetConditionEvaluationContext") -> TimeWindow:
         """Returns the window of time that has passed between the previous two cron ticks. All
         parent assets must contain all data from this time window in order for this asset to be
         materialized.
         """
         previous_ticks = reverse_cron_string_iterator(
             end_timestamp=context.evaluation_time.timestamp(),
             cron_string=self.cron_schedule,
@@ -919,15 +920,15 @@
         end_time = next(previous_ticks)
         start_time = next(previous_ticks)
 
         return TimeWindow(start=start_time, end=end_time)
 
     def get_parent_subset_updated_since_cron(
         self,
-        context: AssetConditionEvaluationContext,
+        context: "AssetConditionEvaluationContext",
         parent_asset_key: AssetKey,
         passed_time_window: TimeWindow,
     ) -> ValidAssetSubset:
         """Returns the AssetSubset of a given parent asset that has been updated since the end of
         the previous cron tick. If a value for this parent asset was computed on the previous
         evaluation, and that evaluation happened within the same cron tick as the current evaluation,
         then this value will be calculated incrementally from the previous value to avoid expensive
@@ -964,15 +965,15 @@
             # the set of asset partitions that have been updated since the previous evaluation
             new_parent_subset = context.instance_queryer.get_asset_subset_updated_after_cursor(
                 asset_key=parent_asset_key, after_cursor=context.previous_max_storage_id
             )
             return new_parent_subset | previous_parent_subset
 
     def get_parent_subsets_updated_since_cron_by_key(
-        self, context: AssetConditionEvaluationContext, passed_time_window: TimeWindow
+        self, context: "AssetConditionEvaluationContext", passed_time_window: TimeWindow
     ) -> Mapping[AssetKey, ValidAssetSubset]:
         """Returns a mapping of parent asset keys to the AssetSubset of each parent that has been
         updated since the end of the previous cron tick. Does not compute this value for time-window
         partitioned parents, as their partitions encode the time windows they have processed.
         """
         updated_subsets_by_key = {}
         for parent_asset_key in context.asset_graph.get(context.asset_key).parent_keys:
@@ -986,15 +987,15 @@
             updated_subsets_by_key[parent_asset_key] = self.get_parent_subset_updated_since_cron(
                 context, parent_asset_key, passed_time_window
             )
         return updated_subsets_by_key
 
     def parent_updated_since_cron(
         self,
-        context: AssetConditionEvaluationContext,
+        context: "AssetConditionEvaluationContext",
         passed_time_window: TimeWindow,
         parent_asset_key: AssetKey,
         child_asset_partition: AssetKeyPartitionKey,
         updated_parent_subset: ValidAssetSubset,
     ) -> bool:
         """Returns if, for a given child asset partition, the given parent asset been updated with
         information from the required time window.
@@ -1029,24 +1030,25 @@
                     parent_asset_key,
                     child_asset_partition.asset_key,
                     context.instance_queryer,
                     context.evaluation_time,
                 ).partitions_subset
 
                 non_updated_parent_asset_partitions = (
-                    ValidAssetSubset(parent_asset_key, parent_subset) - updated_parent_subset
+                    ValidAssetSubset(asset_key=parent_asset_key, value=parent_subset)
+                    - updated_parent_subset
                 ).asset_partitions
 
             return not any(
                 not context.will_update_asset_partition(p)
                 for p in non_updated_parent_asset_partitions
             )
 
     def evaluate_for_asset(
-        self, context: AssetConditionEvaluationContext
+        self, context: "AssetConditionEvaluationContext"
     ) -> "AssetConditionResult":
         from .asset_condition.asset_condition import AssetConditionResult
 
         passed_time_window = self.passed_time_window(context)
         has_new_passed_time_window = passed_time_window.end.timestamp() > (
             context.previous_evaluation_timestamp or 0
         )
@@ -1108,15 +1110,15 @@
         return AutoMaterializeDecisionType.SKIP
 
     @property
     def description(self) -> str:
         return "required parent partitions do not exist"
 
     def evaluate_for_asset(
-        self, context: AssetConditionEvaluationContext
+        self, context: "AssetConditionEvaluationContext"
     ) -> "AssetConditionResult":
         from .asset_condition.asset_condition import AssetConditionResult
 
         asset_partitions_by_evaluation_data = defaultdict(set)
 
         subset_to_evaluate = (
             context.candidates_not_evaluated_on_previous_tick_subset
@@ -1157,15 +1159,15 @@
     def description(self) -> str:
         if self.all_partitions:
             return "part of an asset targeted by an in-progress backfill"
         else:
             return "targeted by an in-progress backfill"
 
     def evaluate_for_asset(
-        self, context: AssetConditionEvaluationContext
+        self, context: "AssetConditionEvaluationContext"
     ) -> "AssetConditionResult":
         from .asset_condition.asset_condition import AssetConditionResult
 
         backfilling_subset = (
             # this backfilling subset is aware of the current partitions definitions, and so will
             # be valid
             (context.instance_queryer.get_active_backfill_target_asset_graph_subset())
@@ -1192,15 +1194,15 @@
         return AutoMaterializeDecisionType.DISCARD
 
     @property
     def description(self) -> str:
         return f"exceeds {self.limit} materialization(s) per minute"
 
     def evaluate_for_asset(
-        self, context: AssetConditionEvaluationContext
+        self, context: "AssetConditionEvaluationContext"
     ) -> "AssetConditionResult":
         from .asset_condition.asset_condition import AssetConditionResult
 
         # the set of asset partitions which exceed the limit
         rate_limited_asset_partitions = set(
             sorted(
                 context.candidate_subset.asset_partitions,
@@ -1223,15 +1225,15 @@
         return AutoMaterializeDecisionType.SKIP
 
     @property
     def description(self) -> str:
         return "in-progress run for asset"
 
     def evaluate_for_asset(
-        self, context: AssetConditionEvaluationContext
+        self, context: "AssetConditionEvaluationContext"
     ) -> "AssetConditionResult":
         from .asset_condition.asset_condition import AssetConditionResult
 
         if context.partitions_def is not None:
             raise DagsterInvariantViolationError(
                 "SkipOnRunInProgressRule is currently only support for non-partitioned assets."
             )
```

### Comparing `dagster-1.7.1/dagster/_core/definitions/auto_materialize_rule_evaluation.py` & `dagster-1.7.2rc1/dagster/_core/definitions/auto_materialize_rule_evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from dagster._core.definitions.asset_subset import AssetSubset
 from dagster._core.definitions.events import AssetKey
 from dagster._core.definitions.metadata import MetadataMapping, MetadataValue
 from dagster._serdes.serdes import (
     _WHITELIST_MAP,
     NamedTupleSerializer,
     PackableValue,
+    PydanticModelSerializer,
     UnpackContext,
     UnpackedValue,
     WhitelistMap,
     deserialize_value,
     whitelist_for_serdes,
 )
 from dagster._utils.security import non_secure_md5_hash_str
@@ -178,18 +179,18 @@
     asset_key: AssetKey,
     partitions_def: Optional[PartitionsDefinition],
 ) -> AssetSubset:
     if partitions_def is None or not serialized.can_deserialize(partitions_def):
         # partitions def has changed since storage time
         return AssetSubset.empty(asset_key, partitions_def)
 
-    return AssetSubset(asset_key, value=serialized.deserialize(partitions_def))
+    return AssetSubset(asset_key=asset_key, value=serialized.deserialize(partitions_def))
 
 
-class BackcompatAutoMaterializeAssetEvaluationSerializer(NamedTupleSerializer):
+class BackcompatAutoMaterializeAssetEvaluationSerializer(PydanticModelSerializer):
     """This handles backcompat for the old AutoMaterializeAssetEvaluation objects, turning them into
     AssetConditionEvaluationWithRunIds objects.
     """
 
     @property
     def partitions_def(self) -> Optional[PartitionsDefinition]:
         """This property gets overridden by subclasses at runtime, once the partitions_def for the
@@ -201,15 +202,15 @@
         self,
         asset_key: AssetKey,
         serialized: Union[None, SerializedPartitionsSubset],
     ) -> AssetSubset:
         if serialized is None:
             # Confusingly, we used `None` to indicate "all of an unpartitioned asset" in the old
             # serialization scheme
-            return AssetSubset(asset_key, True)
+            return AssetSubset(asset_key=asset_key, value=True)
         return deserialize_serialized_partitions_subset_to_asset_subset(
             serialized, asset_key, self.partitions_def
         )
 
     def _asset_condition_snapshot_from_rule_snapshot(
         self, rule_snapshot: AutoMaterializeRuleSnapshot
     ) -> "AssetConditionSnapshot":
@@ -344,16 +345,16 @@
 
         if is_partitioned:
             # In reality, we'd like to invert the inner true_subset here, but this is an
             # expensive operation, and error-prone as the set of all partitions may have changed
             # since the evaluation was stored. Instead, we just use an empty subset.
             true_subset = AssetSubset.empty(asset_key, self.partitions_def)
         else:
-            true_subset = evaluation.true_subset._replace(
-                value=not evaluation.true_subset.bool_value
+            true_subset = evaluation.true_subset.copy(
+                update={"value": not evaluation.true_subset.bool_value}
             )
         return AssetConditionEvaluation(
             condition_snapshot=AssetConditionSnapshot(
                 class_name=NotAssetCondition.__name__, description="Not", unique_id=unique_id
             ),
             true_subset=true_subset,
             candidate_subset=HistoricalAllPartitionsSubsetSentinel()
```

### Comparing `dagster-1.7.1/dagster/_core/definitions/auto_materialize_sensor_definition.py` & `dagster-1.7.2rc1/dagster/_core/definitions/auto_materialize_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/backfill_policy.py` & `dagster-1.7.2rc1/dagster/_core/definitions/backfill_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/base_asset_graph.py` & `dagster-1.7.2rc1/dagster/_core/definitions/base_asset_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,28 +347,28 @@
         relevant PartitionMapping.
         """
         child_asset_key = child_asset_subset.asset_key
         child_partitions_def = self.get(child_asset_key).partitions_def
         parent_partitions_def = self.get(parent_asset_key).partitions_def
 
         if parent_partitions_def is None:
-            return ValidAssetSubset(parent_asset_key, value=child_asset_subset.size > 0)
+            return ValidAssetSubset(asset_key=parent_asset_key, value=child_asset_subset.size > 0)
 
         partition_mapping = self.get_partition_mapping(child_asset_key, parent_asset_key)
         parent_partitions_subset = (
             partition_mapping.get_upstream_mapped_partitions_result_for_partitions(
                 child_asset_subset.subset_value if child_partitions_def is not None else None,
                 downstream_partitions_def=child_partitions_def,
                 upstream_partitions_def=parent_partitions_def,
                 dynamic_partitions_store=dynamic_partitions_store,
                 current_time=current_time,
             )
         ).partitions_subset
 
-        return ValidAssetSubset(parent_asset_key, value=parent_partitions_subset)
+        return ValidAssetSubset(asset_key=parent_asset_key, value=parent_partitions_subset)
 
     def get_child_asset_subset(
         self,
         parent_asset_subset: ValidAssetSubset,
         child_asset_key: AssetKey,
         dynamic_partitions_store: DynamicPartitionsStore,
         current_time: datetime,
@@ -385,25 +385,25 @@
                 return ValidAssetSubset.all(
                     child_asset_key, child_partitions_def, dynamic_partitions_store, current_time
                 )
             else:
                 return ValidAssetSubset.empty(child_asset_key, child_partitions_def)
 
         if child_partitions_def is None:
-            return ValidAssetSubset(child_asset_key, value=parent_asset_subset.size > 0)
+            return ValidAssetSubset(asset_key=child_asset_key, value=parent_asset_subset.size > 0)
         else:
             partition_mapping = self.get_partition_mapping(child_asset_key, parent_asset_key)
             child_partitions_subset = partition_mapping.get_downstream_partitions_for_partitions(
                 parent_asset_subset.subset_value,
                 parent_partitions_def,
                 downstream_partitions_def=child_partitions_def,
                 dynamic_partitions_store=dynamic_partitions_store,
                 current_time=current_time,
             )
-            return ValidAssetSubset(child_asset_key, value=child_partitions_subset)
+            return ValidAssetSubset(asset_key=child_asset_key, value=child_partitions_subset)
 
     def get_children_partitions(
         self,
         dynamic_partitions_store: DynamicPartitionsStore,
         current_time: datetime,
         asset_key: AssetKey,
         partition_key: Optional[str] = None,
```

### Comparing `dagster-1.7.1/dagster/_core/definitions/cacheable_assets.py` & `dagster-1.7.2rc1/dagster/_core/definitions/cacheable_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/composition.py` & `dagster-1.7.2rc1/dagster/_core/definitions/composition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/config.py` & `dagster-1.7.2rc1/dagster/_core/definitions/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/configurable.py` & `dagster-1.7.2rc1/dagster/_core/definitions/configurable.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/data_time.py` & `dagster-1.7.2rc1/dagster/_core/definitions/data_time.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/data_version.py` & `dagster-1.7.2rc1/dagster/_core/definitions/data_version.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/decorators/__init__.py` & `dagster-1.7.2rc1/dagster/_core/definitions/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/decorators/asset_check_decorator.py` & `dagster-1.7.2rc1/dagster/_core/definitions/decorators/asset_check_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/decorators/asset_decorator.py` & `dagster-1.7.2rc1/dagster/_core/definitions/decorators/asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/decorators/config_mapping_decorator.py` & `dagster-1.7.2rc1/dagster/_core/definitions/decorators/config_mapping_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/decorators/graph_decorator.py` & `dagster-1.7.2rc1/dagster/_core/definitions/decorators/graph_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/decorators/hook_decorator.py` & `dagster-1.7.2rc1/dagster/_core/definitions/decorators/hook_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/decorators/job_decorator.py` & `dagster-1.7.2rc1/dagster/_core/definitions/decorators/job_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/decorators/op_decorator.py` & `dagster-1.7.2rc1/dagster/_core/definitions/decorators/op_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/decorators/repository_decorator.py` & `dagster-1.7.2rc1/dagster/_core/definitions/decorators/repository_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/decorators/schedule_decorator.py` & `dagster-1.7.2rc1/dagster/_core/definitions/decorators/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/decorators/sensor_decorator.py` & `dagster-1.7.2rc1/dagster/_core/definitions/decorators/sensor_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/decorators/source_asset_decorator.py` & `dagster-1.7.2rc1/dagster/_core/definitions/decorators/source_asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/definition_config_schema.py` & `dagster-1.7.2rc1/dagster/_core/definitions/definition_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/definitions_class.py` & `dagster-1.7.2rc1/dagster/_core/definitions/definitions_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/dependency.py` & `dagster-1.7.2rc1/dagster/_core/definitions/dependency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/events.py` & `dagster-1.7.2rc1/dagster/_core/definitions/events.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/executor_definition.py` & `dagster-1.7.2rc1/dagster/_core/definitions/executor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/external_asset.py` & `dagster-1.7.2rc1/dagster/_core/definitions/external_asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/freshness_based_auto_materialize.py` & `dagster-1.7.2rc1/dagster/_core/definitions/freshness_based_auto_materialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,11 +222,11 @@
         # if this is False, then executing it would still leave the asset overdue
         and expected_data_time >= execution_period.start
         and evaluation_data is not None
     ):
         all_subset = AssetSubset.all(asset_key, None)
         return (
             AssetSubset.all(asset_key, None),
-            [AssetSubsetWithMetadata(all_subset, evaluation_data.metadata)],
+            [AssetSubsetWithMetadata(subset=all_subset, metadata=evaluation_data.metadata)],
         )
     else:
         return context.empty_subset(), []
```

### Comparing `dagster-1.7.1/dagster/_core/definitions/freshness_checks/last_update.py` & `dagster-1.7.2rc1/dagster/_core/definitions/freshness_checks/last_update.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/freshness_checks/sensor.py` & `dagster-1.7.2rc1/dagster/_core/definitions/freshness_checks/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/freshness_checks/shared_builder.py` & `dagster-1.7.2rc1/dagster/_core/definitions/freshness_checks/shared_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/freshness_checks/time_partition.py` & `dagster-1.7.2rc1/dagster/_core/definitions/freshness_checks/time_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/freshness_checks/utils.py` & `dagster-1.7.2rc1/dagster/_core/definitions/freshness_checks/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/freshness_policy.py` & `dagster-1.7.2rc1/dagster/_core/definitions/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/freshness_policy_sensor_definition.py` & `dagster-1.7.2rc1/dagster/_core/definitions/freshness_policy_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/graph_definition.py` & `dagster-1.7.2rc1/dagster/_core/definitions/graph_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/hook_definition.py` & `dagster-1.7.2rc1/dagster/_core/definitions/hook_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/hook_invocation.py` & `dagster-1.7.2rc1/dagster/_core/definitions/hook_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/inference.py` & `dagster-1.7.2rc1/dagster/_core/definitions/inference.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/input.py` & `dagster-1.7.2rc1/dagster/_core/definitions/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/instigation_logger.py` & `dagster-1.7.2rc1/dagster/_core/definitions/instigation_logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/job_base.py` & `dagster-1.7.2rc1/dagster/_core/definitions/job_base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/job_definition.py` & `dagster-1.7.2rc1/dagster/_core/definitions/job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/load_asset_checks_from_modules.py` & `dagster-1.7.2rc1/dagster/_core/definitions/load_asset_checks_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/load_assets_from_modules.py` & `dagster-1.7.2rc1/dagster/_core/definitions/load_assets_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/logger_definition.py` & `dagster-1.7.2rc1/dagster/_core/definitions/logger_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/logger_invocation.py` & `dagster-1.7.2rc1/dagster/_core/definitions/logger_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/materialize.py` & `dagster-1.7.2rc1/dagster/_core/definitions/materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/metadata/__init__.py` & `dagster-1.7.2rc1/dagster/_core/definitions/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/metadata/table.py` & `dagster-1.7.2rc1/dagster/_core/definitions/metadata/table.py`

 * *Files 24% similar despite different names*

```diff
@@ -297,15 +297,64 @@
     NamedTuple(
         "_TableSpec",
         [
             ("deps_by_column", PublicAttr[Mapping[str, Sequence[TableColumnDep]]]),
         ],
     )
 ):
-    """Represents the lineage of column outputs to column inputs for a tabular asset."""
+    """Represents the lineage of column outputs to column inputs for a tabular asset.
+
+    Args:
+        deps_by_column (Mapping[str, Sequence[TableColumnDep]]): A mapping from column names to
+            the columns that the column depends on.
+
+    Examples:
+        Defining column lineage at materialization time, where the resulting asset has two columns,
+        ``new_column_foo`` and ``new_column_qux``. The first column, ``new_column_foo``, depends on
+        ``column_bar`` in ``source_bar`` and ``column_baz`` in ``source_baz``. The second column,
+        ``new_column_qux``, depends on ``column_quuz`` in ``source_bar``.
+
+        .. code-block:: python
+
+            from dagster import (
+                AssetKey,
+                MaterializeResult,
+                TableColumnDep,
+                TableColumnLineage,
+                asset,
+            )
+
+
+            @asset(deps=[AssetKey("source_bar"), AssetKey("source_baz")])
+            def my_asset():
+                yield MaterializeResult(
+                    metadata={
+                        "dagster/column_lineage": TableColumnLineage(
+                            deps_by_column={
+                                "new_column_foo": [
+                                    TableColumnDep(
+                                        asset_key=AssetKey("source_bar"),
+                                        column_name="column_bar",
+                                    ),
+                                    TableColumnDep(
+                                        asset_key=AssetKey("source_baz"),
+                                        column_name="column_baz",
+                                    ),
+                                ],
+                                "new_column_qux": [
+                                    TableColumnDep(
+                                        asset_key=AssetKey("source_bar"),
+                                        column_name="column_quuz",
+                                    ),
+                                ],
+                            }
+                        )
+                    }
+                )
+    """
 
     def __new__(cls, deps_by_column: Mapping[str, Sequence[TableColumnDep]]):
         deps_by_column = check.mapping_param(
             deps_by_column, "deps_by_column", key_type=str, value_type=list
         )
 
         sorted_deps_by_column = {}
```

### Comparing `dagster-1.7.1/dagster/_core/definitions/multi_asset_sensor_definition.py` & `dagster-1.7.2rc1/dagster/_core/definitions/multi_asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/multi_dimensional_partitions.py` & `dagster-1.7.2rc1/dagster/_core/definitions/multi_dimensional_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/node_container.py` & `dagster-1.7.2rc1/dagster/_core/definitions/node_container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/node_definition.py` & `dagster-1.7.2rc1/dagster/_core/definitions/node_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/observe.py` & `dagster-1.7.2rc1/dagster/_core/definitions/observe.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/op_definition.py` & `dagster-1.7.2rc1/dagster/_core/definitions/op_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/op_invocation.py` & `dagster-1.7.2rc1/dagster/_core/definitions/op_invocation.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     TypeVar,
     Union,
     cast,
 )
 
 import dagster._check as check
 from dagster._core.decorator_utils import get_function_params
+from dagster._core.definitions.asset_check_result import AssetCheckResult
 from dagster._core.errors import (
     DagsterInvalidInvocationError,
     DagsterInvariantViolationError,
     DagsterTypeCheckDidNotPass,
 )
 
 from .events import (
@@ -361,38 +362,50 @@
     raise DagsterInvariantViolationError(
         f"{result.__class__.__name__} did not include asset_key and it can not be inferred. Specify which"
         f" asset_key, options are: {context.per_invocation_properties.assets_def.keys}"
     )
 
 
 def _output_name_for_result_obj(
-    event: AssetResult,
+    event: Union[AssetResult, AssetCheckResult],
     context: "BaseDirectExecutionContext",
 ):
     if not context.per_invocation_properties.assets_def:
         raise DagsterInvariantViolationError(
             f"Op {context.per_invocation_properties.alias} does not have an assets definition."
         )
-    asset_key = _key_for_result(event, context)
-    return context.per_invocation_properties.assets_def.get_output_name_for_asset_key(asset_key)
+
+    if isinstance(event, AssetResult):
+        asset_key = _key_for_result(event, context)
+        return context.per_invocation_properties.assets_def.get_output_name_for_asset_key(asset_key)
+    elif isinstance(event, AssetCheckResult):
+        check_names_by_asset_key = {}
+        for spec in context.per_invocation_properties.assets_def.check_specs:
+            if spec.asset_key not in check_names_by_asset_key:
+                check_names_by_asset_key[spec.asset_key] = []
+            check_names_by_asset_key[spec.asset_key].append(spec.name)
+
+        return context.per_invocation_properties.assets_def.get_output_name_for_asset_check_key(
+            event.resolve_target_check_key(check_names_by_asset_key)
+        )
 
 
 def _handle_gen_event(
     event: T,
     op_def: "OpDefinition",
     context: "BaseDirectExecutionContext",
     output_defs: Mapping[str, OutputDefinition],
     outputs_seen: Set[str],
 ) -> T:
     if isinstance(
         event,
         (AssetMaterialization, AssetObservation, ExpectationResult),
     ):
         return event
-    elif isinstance(event, AssetResult):
+    elif isinstance(event, (AssetResult, AssetCheckResult)):
         output_name = _output_name_for_result_obj(event, context)
         outputs_seen.add(output_name)
         return event
     else:
         if not isinstance(event, (Output, DynamicOutput)):
             raise DagsterInvariantViolationError(
                 f"When yielding outputs from a {op_def.node_type_str} generator,"
```

### Comparing `dagster-1.7.1/dagster/_core/definitions/op_selection.py` & `dagster-1.7.2rc1/dagster/_core/definitions/op_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/output.py` & `dagster-1.7.2rc1/dagster/_core/definitions/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/partition.py` & `dagster-1.7.2rc1/dagster/_core/definitions/partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/partition_key_range.py` & `dagster-1.7.2rc1/dagster/_core/definitions/partition_key_range.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/partition_mapping.py` & `dagster-1.7.2rc1/dagster/_core/definitions/partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/partitioned_schedule.py` & `dagster-1.7.2rc1/dagster/_core/definitions/partitioned_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/policy.py` & `dagster-1.7.2rc1/dagster/_core/definitions/policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/reconstruct.py` & `dagster-1.7.2rc1/dagster/_core/definitions/reconstruct.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/remote_asset_graph.py` & `dagster-1.7.2rc1/dagster/_core/definitions/remote_asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/repository_definition/__init__.py` & `dagster-1.7.2rc1/dagster/_core/definitions/repository_definition/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/repository_definition/caching_index.py` & `dagster-1.7.2rc1/dagster/_core/definitions/repository_definition/caching_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/repository_definition/repository_data.py` & `dagster-1.7.2rc1/dagster/_core/definitions/repository_definition/repository_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/repository_definition/repository_data_builder.py` & `dagster-1.7.2rc1/dagster/_core/definitions/repository_definition/repository_data_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/repository_definition/repository_definition.py` & `dagster-1.7.2rc1/dagster/_core/definitions/repository_definition/repository_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/repository_definition/valid_definitions.py` & `dagster-1.7.2rc1/dagster/_core/definitions/repository_definition/valid_definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/resolved_asset_deps.py` & `dagster-1.7.2rc1/dagster/_core/definitions/resolved_asset_deps.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/resource_annotation.py` & `dagster-1.7.2rc1/dagster/_core/definitions/resource_annotation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/resource_definition.py` & `dagster-1.7.2rc1/dagster/_core/definitions/resource_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/resource_invocation.py` & `dagster-1.7.2rc1/dagster/_core/definitions/resource_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/resource_requirement.py` & `dagster-1.7.2rc1/dagster/_core/definitions/resource_requirement.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/result.py` & `dagster-1.7.2rc1/dagster/_core/definitions/result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/run_config.py` & `dagster-1.7.2rc1/dagster/_core/definitions/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/run_config_schema.py` & `dagster-1.7.2rc1/dagster/_core/definitions/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/run_request.py` & `dagster-1.7.2rc1/dagster/_core/definitions/run_request.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/run_status_sensor_definition.py` & `dagster-1.7.2rc1/dagster/_core/definitions/run_status_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/schedule_definition.py` & `dagster-1.7.2rc1/dagster/_core/definitions/schedule_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/schema_change_checks.py` & `dagster-1.7.2rc1/dagster/_core/definitions/schema_change_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/scoped_resources_builder.py` & `dagster-1.7.2rc1/dagster/_core/definitions/scoped_resources_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/selector.py` & `dagster-1.7.2rc1/dagster/_core/definitions/selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/sensor_definition.py` & `dagster-1.7.2rc1/dagster/_core/definitions/sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/source_asset.py` & `dagster-1.7.2rc1/dagster/_core/definitions/source_asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/step_launcher.py` & `dagster-1.7.2rc1/dagster/_core/definitions/step_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/target.py` & `dagster-1.7.2rc1/dagster/_core/definitions/target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/time_window_partition_mapping.py` & `dagster-1.7.2rc1/dagster/_core/definitions/time_window_partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/time_window_partitions.py` & `dagster-1.7.2rc1/dagster/_core/definitions/time_window_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/unresolved_asset_job_definition.py` & `dagster-1.7.2rc1/dagster/_core/definitions/unresolved_asset_job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/utils.py` & `dagster-1.7.2rc1/dagster/_core/definitions/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/definitions/version_strategy.py` & `dagster-1.7.2rc1/dagster/_core/definitions/version_strategy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/errors.py` & `dagster-1.7.2rc1/dagster/_core/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -682,7 +682,11 @@
     """Indicates that a stored value can't be deserialized because the definition needed to interpret
     it has changed.
     """
 
 
 class DagsterPipesExecutionError(DagsterError):
     """Indicates that an error occurred during the execution of an external process."""
+
+
+class DagsterImportClassFromCodePointerError(DagsterError):
+    """Indicates that an error occurred while importing a class from a code pointer."""
```

### Comparing `dagster-1.7.1/dagster/_core/event_api.py` & `dagster-1.7.2rc1/dagster/_core/event_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/events/__init__.py` & `dagster-1.7.2rc1/dagster/_core/events/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/events/log.py` & `dagster-1.7.2rc1/dagster/_core/events/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/events/utils.py` & `dagster-1.7.2rc1/dagster/_core/events/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/api.py` & `dagster-1.7.2rc1/dagster/_core/execution/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/asset_backfill.py` & `dagster-1.7.2rc1/dagster/_core/execution/asset_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/backfill.py` & `dagster-1.7.2rc1/dagster/_core/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/build_resources.py` & `dagster-1.7.2rc1/dagster/_core/execution/build_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/compute_logs.py` & `dagster-1.7.2rc1/dagster/_core/execution/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/context/compute.py` & `dagster-1.7.2rc1/dagster/_core/execution/context/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/context/hook.py` & `dagster-1.7.2rc1/dagster/_core/execution/context/hook.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/context/init.py` & `dagster-1.7.2rc1/dagster/_core/execution/context/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/context/input.py` & `dagster-1.7.2rc1/dagster/_core/execution/context/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/context/invocation.py` & `dagster-1.7.2rc1/dagster/_core/execution/context/invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/context/logger.py` & `dagster-1.7.2rc1/dagster/_core/execution/context/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/context/output.py` & `dagster-1.7.2rc1/dagster/_core/execution/context/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/context/system.py` & `dagster-1.7.2rc1/dagster/_core/execution/context/system.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/context_creation_job.py` & `dagster-1.7.2rc1/dagster/_core/execution/context_creation_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/execute_in_process.py` & `dagster-1.7.2rc1/dagster/_core/execution/execute_in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/execute_in_process_result.py` & `dagster-1.7.2rc1/dagster/_core/execution/execute_in_process_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/execution_result.py` & `dagster-1.7.2rc1/dagster/_core/execution/execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/host_mode.py` & `dagster-1.7.2rc1/dagster/_core/execution/host_mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/job_backfill.py` & `dagster-1.7.2rc1/dagster/_core/execution/job_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/job_execution_result.py` & `dagster-1.7.2rc1/dagster/_core/execution/job_execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/memoization.py` & `dagster-1.7.2rc1/dagster/_core/execution/memoization.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/plan/active.py` & `dagster-1.7.2rc1/dagster/_core/execution/plan/active.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/plan/compute.py` & `dagster-1.7.2rc1/dagster/_core/execution/plan/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/plan/compute_generator.py` & `dagster-1.7.2rc1/dagster/_core/execution/plan/compute_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -175,21 +175,33 @@
 def _filter_expected_output_defs(
     result: Any, context: ExecutionContextTypes, output_defs: Sequence[OutputDefinition]
 ) -> Sequence[OutputDefinition]:
     result_tuple = (
         (result,) if not isinstance(result, tuple) or is_named_tuple_instance(result) else result
     )
     asset_results = [x for x in result_tuple if isinstance(x, AssetResult)]
-    remove_outputs = [
-        r.get_spec_python_identifier(
-            asset_key=x.asset_key or context.op_execution_context.asset_key
-        )
-        for x in asset_results
-        for r in x.check_results or []
-    ]
+
+    if not asset_results:
+        return output_defs
+
+    check_names_by_asset_key = {}
+    for spec in context.op_execution_context.assets_def.check_specs:
+        if spec.asset_key not in check_names_by_asset_key:
+            check_names_by_asset_key[spec.asset_key] = []
+        check_names_by_asset_key[spec.asset_key].append(spec.name)
+
+    remove_outputs = []
+    for asset_result in asset_results:
+        for check_result in asset_result.check_results:
+            remove_outputs.append(
+                context.op_execution_context.assets_def.get_output_name_for_asset_check_key(
+                    check_result.resolve_target_check_key(check_names_by_asset_key)
+                )
+            )
+
     return [out for out in output_defs if out.name not in remove_outputs]
 
 
 def _validate_multi_return(
     context: ExecutionContextTypes,
     result: Any,
     output_defs: Sequence[OutputDefinition],
```

### Comparing `dagster-1.7.1/dagster/_core/execution/plan/execute_plan.py` & `dagster-1.7.2rc1/dagster/_core/execution/plan/execute_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/plan/execute_step.py` & `dagster-1.7.2rc1/dagster/_core/execution/plan/execute_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/plan/external_step.py` & `dagster-1.7.2rc1/dagster/_core/execution/plan/external_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/plan/handle.py` & `dagster-1.7.2rc1/dagster/_core/execution/plan/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/plan/inputs.py` & `dagster-1.7.2rc1/dagster/_core/execution/plan/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/plan/instance_concurrency_context.py` & `dagster-1.7.2rc1/dagster/_core/execution/plan/instance_concurrency_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/plan/local_external_step_main.py` & `dagster-1.7.2rc1/dagster/_core/execution/plan/local_external_step_main.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/plan/objects.py` & `dagster-1.7.2rc1/dagster/_core/execution/plan/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/plan/outputs.py` & `dagster-1.7.2rc1/dagster/_core/execution/plan/outputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/plan/plan.py` & `dagster-1.7.2rc1/dagster/_core/execution/plan/plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/plan/state.py` & `dagster-1.7.2rc1/dagster/_core/execution/plan/state.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/plan/step.py` & `dagster-1.7.2rc1/dagster/_core/execution/plan/step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/plan/utils.py` & `dagster-1.7.2rc1/dagster/_core/execution/plan/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/poll_compute_logs.py` & `dagster-1.7.2rc1/dagster/_core/execution/poll_compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/resolve_versions.py` & `dagster-1.7.2rc1/dagster/_core/execution/resolve_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/resources_init.py` & `dagster-1.7.2rc1/dagster/_core/execution/resources_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/retries.py` & `dagster-1.7.2rc1/dagster/_core/execution/retries.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/run_cancellation_thread.py` & `dagster-1.7.2rc1/dagster/_core/execution/run_cancellation_thread.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/stats.py` & `dagster-1.7.2rc1/dagster/_core/execution/stats.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/submit_asset_runs.py` & `dagster-1.7.2rc1/dagster/_core/execution/submit_asset_runs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/tags.py` & `dagster-1.7.2rc1/dagster/_core/execution/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/validate_run_config.py` & `dagster-1.7.2rc1/dagster/_core/execution/validate_run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/watch_orphans.py` & `dagster-1.7.2rc1/dagster/_core/execution/watch_orphans.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/execution/with_resources.py` & `dagster-1.7.2rc1/dagster/_core/execution/with_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/executor/base.py` & `dagster-1.7.2rc1/dagster/_core/executor/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/executor/child_process_executor.py` & `dagster-1.7.2rc1/dagster/_core/executor/child_process_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/executor/in_process.py` & `dagster-1.7.2rc1/dagster/_core/executor/in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/executor/init.py` & `dagster-1.7.2rc1/dagster/_core/executor/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/executor/multiprocess.py` & `dagster-1.7.2rc1/dagster/_core/executor/multiprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/executor/step_delegating/step_delegating_executor.py` & `dagster-1.7.2rc1/dagster/_core/executor/step_delegating/step_delegating_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/executor/step_delegating/step_handler/base.py` & `dagster-1.7.2rc1/dagster/_core/executor/step_delegating/step_handler/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/instance/__init__.py` & `dagster-1.7.2rc1/dagster/_core/instance/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     PARENT_RUN_ID_TAG,
     PARTITION_NAME_TAG,
     RESUME_RETRY_TAG,
     ROOT_RUN_ID_TAG,
     RUN_FAILURE_REASON_TAG,
 )
 from dagster._serdes import ConfigurableClass
+from dagster._serdes.config_class import ConfigurableClassData
 from dagster._seven import get_current_datetime_in_utc
 from dagster._utils import PrintFn, is_uuid, traced
 from dagster._utils.error import serializable_error_info_from_exc_info
 from dagster._utils.merger import merge_dicts
 from dagster._utils.warnings import (
     deprecation_warning,
     experimental_warning,
@@ -474,14 +475,26 @@
 
         self._secrets_loader = check.opt_inst_param(secrets_loader, "secrets_loader", SecretsLoader)
 
         if self._secrets_loader:
             self._secrets_loader.register_instance(self)
 
         self._ref = check.opt_inst_param(ref, "ref", InstanceRef)
+        # Fetch backcompat version of instance ref that points to the dagster_cloud
+        # module to ensure compatibility with older versions of agent/user code.
+        if ref and ref.custom_instance_class_data:
+            module_elems = ref.custom_instance_class_data.module_name.split(".")
+            if "dagster_plus" == module_elems[0]:
+                self._ref = ref._replace(
+                    custom_instance_class_data=ConfigurableClassData(
+                        module_name=".".join(["dagster_cloud", *module_elems[1:]]),
+                        class_name=ref.custom_instance_class_data.class_name,
+                        config_yaml=ref.custom_instance_class_data.config_yaml,
+                    )
+                )
 
         self._subscribers: Dict[str, List[Callable]] = defaultdict(list)
 
         run_monitoring_enabled = self.run_monitoring_settings.get("enabled", False)
         self._run_monitoring_enabled = run_monitoring_enabled
         if self.run_monitoring_enabled and self.run_monitoring_max_resume_run_attempts:
             check.invariant(
```

### Comparing `dagster-1.7.1/dagster/_core/instance/config.py` & `dagster-1.7.2rc1/dagster/_core/instance/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Permissive,
     ScalarUnion,
     Selector,
     StringSource,
     validate_config,
 )
 from dagster._config.source import BoolSource
-from dagster._core.errors import DagsterInvalidConfigError
+from dagster._core.errors import DagsterImportClassFromCodePointerError, DagsterInvalidConfigError
 from dagster._core.storage.config import mysql_config, pg_config
 from dagster._serdes import class_from_code_pointer
 from dagster._utils.concurrency import get_max_concurrency_limit_value
 from dagster._utils.merger import merge_dicts
 from dagster._utils.yaml_utils import load_yaml_from_globs
 
 if TYPE_CHECKING:
@@ -32,14 +32,41 @@
 DAGSTER_CONFIG_YAML_FILENAME = "dagster.yaml"
 
 
 def is_dagster_home_set() -> bool:
     return bool(os.getenv("DAGSTER_HOME"))
 
 
+def dagster_instance_class_from_code_pointer(
+    module_name: str, class_name: str
+) -> Type["DagsterInstance"]:
+    try:
+        return cast(
+            Type["DagsterInstance"],
+            class_from_code_pointer(module_name, class_name),
+        )
+    except DagsterImportClassFromCodePointerError as e:
+        module_elems = module_name.split(".")
+        if "dagster_cloud" == module_elems[0]:
+            try:
+                return cast(
+                    Type["DagsterInstance"],
+                    class_from_code_pointer(
+                        ".".join(["dagster_plus", *module_elems[1:]]),
+                        class_name,
+                    ),
+                )
+            except Exception:
+                logger = logging.getLogger("dagster")
+                logger.exception("Error importing DagsterInstance class from dagster_plus module")
+                raise e
+        else:
+            raise e
+
+
 def dagster_instance_config(
     base_dir: str,
     config_filename: str = DAGSTER_CONFIG_YAML_FILENAME,
     overrides: Optional[Mapping[str, object]] = None,
 ) -> Tuple[Mapping[str, Any], Optional[Type["DagsterInstance"]]]:
     check.str_param(base_dir, "base_dir")
     check.invariant(os.path.isdir(base_dir), "base_dir should be a directory")
@@ -66,19 +93,16 @@
         if not validate_custom_config.success:
             raise DagsterInvalidConfigError(
                 f"Errors whilst loading dagster custom class config at {config_filename}",
                 validate_custom_config.errors,
                 custom_instance_class_data,
             )
 
-        custom_instance_class = cast(
-            Type["DagsterInstance"],
-            class_from_code_pointer(
-                custom_instance_class_data["module"], custom_instance_class_data["class"]
-            ),
+        custom_instance_class = dagster_instance_class_from_code_pointer(
+            custom_instance_class_data["module"], custom_instance_class_data["class"]
         )
 
         schema: Mapping[str, Field]
         if hasattr(custom_instance_class, "config_schema"):
             schema = merge_dicts(
                 dagster_instance_config_schema(),
                 custom_instance_class.config_schema(),  # type: ignore
```

### Comparing `dagster-1.7.1/dagster/_core/instance/ref.py` & `dagster-1.7.2rc1/dagster/_core/instance/ref.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 import os
 from typing import TYPE_CHECKING, Any, Mapping, NamedTuple, Optional, Sequence, Type
 
 import yaml
 
 import dagster._check as check
-from dagster._serdes import ConfigurableClassData, class_from_code_pointer, whitelist_for_serdes
-
-from .config import DAGSTER_CONFIG_YAML_FILENAME, dagster_instance_config
+from dagster._serdes import (
+    ConfigurableClassData,
+    whitelist_for_serdes,
+)
+
+from .config import (
+    DAGSTER_CONFIG_YAML_FILENAME,
+    dagster_instance_class_from_code_pointer,
+    dagster_instance_config,
+)
 
 if TYPE_CHECKING:
     from dagster._core.instance import DagsterInstance, DagsterInstanceOverrides
     from dagster._core.launcher.base import RunLauncher
     from dagster._core.run_coordinator.base import RunCoordinator
     from dagster._core.scheduler.scheduler import Scheduler
     from dagster._core.secrets.loader import SecretsLoader
@@ -569,22 +576,22 @@
             self.secrets_loader_data.rehydrate(as_type=SecretsLoader)
             if self.secrets_loader_data
             else None
         )
 
     @property
     def custom_instance_class(self) -> Type["DagsterInstance"]:
-        return (  # type: ignore  # (ambiguous return type)
-            class_from_code_pointer(
+        return (
+            dagster_instance_class_from_code_pointer(
                 self.custom_instance_class_data.module_name,
                 self.custom_instance_class_data.class_name,
             )
             if self.custom_instance_class_data
             else None
-        )
+        )  # type: ignore
 
     @property
     def custom_instance_class_config(self) -> Mapping[str, Any]:
         return (
             self.custom_instance_class_data.config_dict if self.custom_instance_class_data else {}
         )
```

### Comparing `dagster-1.7.1/dagster/_core/instance_for_test.py` & `dagster-1.7.2rc1/dagster/_core/instance_for_test.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/launcher/base.py` & `dagster-1.7.2rc1/dagster/_core/launcher/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/launcher/default_run_launcher.py` & `dagster-1.7.2rc1/dagster/_core/launcher/default_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/launcher/sync_in_memory_run_launcher.py` & `dagster-1.7.2rc1/dagster/_core/launcher/sync_in_memory_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/log_manager.py` & `dagster-1.7.2rc1/dagster/_core/log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/nux.py` & `dagster-1.7.2rc1/dagster/_core/nux.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/op_concurrency_limits_counter.py` & `dagster-1.7.2rc1/dagster/_core/op_concurrency_limits_counter.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/origin.py` & `dagster-1.7.2rc1/dagster/_core/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/pipes/client.py` & `dagster-1.7.2rc1/dagster/_core/pipes/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/pipes/context.py` & `dagster-1.7.2rc1/dagster/_core/pipes/context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/pipes/subprocess.py` & `dagster-1.7.2rc1/dagster/_core/pipes/subprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/pipes/utils.py` & `dagster-1.7.2rc1/dagster/_core/pipes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/remote_representation/__init__.py` & `dagster-1.7.2rc1/dagster/_core/remote_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/remote_representation/code_location.py` & `dagster-1.7.2rc1/dagster/_core/remote_representation/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/remote_representation/external.py` & `dagster-1.7.2rc1/dagster/_core/remote_representation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/remote_representation/external_data.py` & `dagster-1.7.2rc1/dagster/_core/remote_representation/external_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/remote_representation/feature_flags.py` & `dagster-1.7.2rc1/dagster/_core/remote_representation/feature_flags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/remote_representation/grpc_server_registry.py` & `dagster-1.7.2rc1/dagster/_core/remote_representation/grpc_server_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/remote_representation/grpc_server_state_subscriber.py` & `dagster-1.7.2rc1/dagster/_core/remote_representation/grpc_server_state_subscriber.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/remote_representation/handle.py` & `dagster-1.7.2rc1/dagster/_core/remote_representation/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/remote_representation/historical.py` & `dagster-1.7.2rc1/dagster/_core/remote_representation/historical.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/remote_representation/job_index.py` & `dagster-1.7.2rc1/dagster/_core/remote_representation/job_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/remote_representation/origin.py` & `dagster-1.7.2rc1/dagster/_core/remote_representation/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/remote_representation/represented.py` & `dagster-1.7.2rc1/dagster/_core/remote_representation/represented.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/run_coordinator/base.py` & `dagster-1.7.2rc1/dagster/_core/run_coordinator/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/run_coordinator/default_run_coordinator.py` & `dagster-1.7.2rc1/dagster/_core/run_coordinator/default_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/run_coordinator/queued_run_coordinator.py` & `dagster-1.7.2rc1/dagster/_core/run_coordinator/queued_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/scheduler/__init__.py` & `dagster-1.7.2rc1/dagster/_core/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/scheduler/execution.py` & `dagster-1.7.2rc1/dagster/_core/scheduler/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/scheduler/instigation.py` & `dagster-1.7.2rc1/dagster/_core/scheduler/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/scheduler/scheduler.py` & `dagster-1.7.2rc1/dagster/_core/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/secrets/env_file.py` & `dagster-1.7.2rc1/dagster/_core/secrets/env_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/selector/subset_selector.py` & `dagster-1.7.2rc1/dagster/_core/selector/subset_selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/snap/__init__.py` & `dagster-1.7.2rc1/dagster/_core/snap/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/snap/dagster_types.py` & `dagster-1.7.2rc1/dagster/_core/snap/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/snap/dep_snapshot.py` & `dagster-1.7.2rc1/dagster/_core/snap/dep_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/snap/execution_plan_snapshot.py` & `dagster-1.7.2rc1/dagster/_core/snap/execution_plan_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/snap/job_snapshot.py` & `dagster-1.7.2rc1/dagster/_core/snap/job_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/snap/mode.py` & `dagster-1.7.2rc1/dagster/_core/snap/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/snap/node.py` & `dagster-1.7.2rc1/dagster/_core/snap/node.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/snap/snap_to_yaml.py` & `dagster-1.7.2rc1/dagster/_core/snap/snap_to_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/DEVELOPING.md` & `dagster-1.7.2rc1/dagster/_core/storage/DEVELOPING.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/README.md` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/env.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/001_initial_1.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/001_initial_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/031_add_kvs_table.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/031_add_kvs_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py` & `dagster-1.7.2rc1/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/asset_check_execution_record.py` & `dagster-1.7.2rc1/dagster/_core/storage/asset_check_execution_record.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/asset_value_loader.py` & `dagster-1.7.2rc1/dagster/_core/storage/asset_value_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/base_storage.py` & `dagster-1.7.2rc1/dagster/_core/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/branching/branching_io_manager.py` & `dagster-1.7.2rc1/dagster/_core/storage/branching/branching_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/captured_log_manager.py` & `dagster-1.7.2rc1/dagster/_core/storage/captured_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/cloud_storage_compute_log_manager.py` & `dagster-1.7.2rc1/dagster/_core/storage/cloud_storage_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/compute_log_manager.py` & `dagster-1.7.2rc1/dagster/_core/storage/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/config.py` & `dagster-1.7.2rc1/dagster/_core/storage/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/dagster_run.py` & `dagster-1.7.2rc1/dagster/_core/storage/dagster_run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/db_io_manager.py` & `dagster-1.7.2rc1/dagster/_core/storage/db_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/event_log/__init__.py` & `dagster-1.7.2rc1/dagster/_core/storage/event_log/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/event_log/base.py` & `dagster-1.7.2rc1/dagster/_core/storage/event_log/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,38 +53,45 @@
         "_AssetEntry",
         [
             ("asset_key", AssetKey),
             ("last_materialization_record", Optional[EventLogRecord]),
             ("last_run_id", Optional[str]),
             ("asset_details", Optional[AssetDetails]),
             ("cached_status", Optional["AssetStatusCacheValue"]),
+            # This is an optional field which can be used for more performant last observation
+            # queries if the underlying storage supports it
+            ("last_observation_record", Optional[EventLogRecord]),
         ],
     )
 ):
     def __new__(
         cls,
         asset_key: AssetKey,
         last_materialization_record: Optional[EventLogRecord] = None,
         last_run_id: Optional[str] = None,
         asset_details: Optional[AssetDetails] = None,
         cached_status: Optional["AssetStatusCacheValue"] = None,
+        last_observation_record: Optional[EventLogRecord] = None,
     ):
         from dagster._core.storage.partition_status_cache import AssetStatusCacheValue
 
         return super(AssetEntry, cls).__new__(
             cls,
             asset_key=check.inst_param(asset_key, "asset_key", AssetKey),
             last_materialization_record=check.opt_inst_param(
                 last_materialization_record, "last_materialization_record", EventLogRecord
             ),
             last_run_id=check.opt_str_param(last_run_id, "last_run_id"),
             asset_details=check.opt_inst_param(asset_details, "asset_details", AssetDetails),
             cached_status=check.opt_inst_param(
                 cached_status, "cached_status", AssetStatusCacheValue
             ),
+            last_observation_record=check.opt_inst_param(
+                last_observation_record, "last_observation_record", EventLogRecord
+            ),
         )
 
     @property
     def last_materialization(self) -> Optional["EventLogEntry"]:
         if self.last_materialization_record is None:
             return None
         return self.last_materialization_record.event_log_entry
@@ -411,14 +418,18 @@
         return False
 
     @property
     def supports_global_concurrency_limits(self) -> bool:
         """Indicates that the EventLogStorage supports global concurrency limits."""
         return False
 
+    @property
+    def asset_records_have_last_observation(self) -> bool:
+        return False
+
     @abstractmethod
     def initialize_concurrency_limit_to_default(self, concurrency_key: str) -> bool:
         """Initialize a concurrency limit to the instance default value.  Is a no-op for concurrency
         keys that are already configured with a limit.
         """
         raise NotImplementedError()
```

### Comparing `dagster-1.7.1/dagster/_core/storage/event_log/in_memory.py` & `dagster-1.7.2rc1/dagster/_core/storage/event_log/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/event_log/migration.py` & `dagster-1.7.2rc1/dagster/_core/storage/event_log/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/event_log/polling_event_watcher.py` & `dagster-1.7.2rc1/dagster/_core/storage/event_log/polling_event_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/event_log/schema.py` & `dagster-1.7.2rc1/dagster/_core/storage/event_log/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/event_log/sql_event_log.py` & `dagster-1.7.2rc1/dagster/_core/storage/event_log/sql_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini` & `dagster-1.7.2rc1/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py` & `dagster-1.7.2rc1/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py` & `dagster-1.7.2rc1/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/file_manager.py` & `dagster-1.7.2rc1/dagster/_core/storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/fs_io_manager.py` & `dagster-1.7.2rc1/dagster/_core/storage/fs_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/input_manager.py` & `dagster-1.7.2rc1/dagster/_core/storage/input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/io_manager.py` & `dagster-1.7.2rc1/dagster/_core/storage/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/legacy_storage.py` & `dagster-1.7.2rc1/dagster/_core/storage/legacy_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/local_compute_log_manager.py` & `dagster-1.7.2rc1/dagster/_core/storage/local_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/mem_io_manager.py` & `dagster-1.7.2rc1/dagster/_core/storage/mem_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/memoizable_io_manager.py` & `dagster-1.7.2rc1/dagster/_core/storage/memoizable_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/migration/bigint_migration.py` & `dagster-1.7.2rc1/dagster/_core/storage/migration/bigint_migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/migration/utils.py` & `dagster-1.7.2rc1/dagster/_core/storage/migration/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/noop_compute_log_manager.py` & `dagster-1.7.2rc1/dagster/_core/storage/noop_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/output_manager.py` & `dagster-1.7.2rc1/dagster/_core/storage/output_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/partition_status_cache.py` & `dagster-1.7.2rc1/dagster/_core/storage/partition_status_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/root.py` & `dagster-1.7.2rc1/dagster/_core/storage/root.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/runs/base.py` & `dagster-1.7.2rc1/dagster/_core/storage/runs/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/runs/in_memory.py` & `dagster-1.7.2rc1/dagster/_core/storage/runs/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/runs/migration.py` & `dagster-1.7.2rc1/dagster/_core/storage/runs/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/runs/schema.py` & `dagster-1.7.2rc1/dagster/_core/storage/runs/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/runs/sql_run_storage.py` & `dagster-1.7.2rc1/dagster/_core/storage/runs/sql_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/runs/sqlite/alembic/alembic.ini` & `dagster-1.7.2rc1/dagster/_core/storage/runs/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py` & `dagster-1.7.2rc1/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/schedules/base.py` & `dagster-1.7.2rc1/dagster/_core/storage/schedules/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/schedules/migration.py` & `dagster-1.7.2rc1/dagster/_core/storage/schedules/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/schedules/schema.py` & `dagster-1.7.2rc1/dagster/_core/storage/schedules/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/schedules/sql_schedule_storage.py` & `dagster-1.7.2rc1/dagster/_core/storage/schedules/sql_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini` & `dagster-1.7.2rc1/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py` & `dagster-1.7.2rc1/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/sql.py` & `dagster-1.7.2rc1/dagster/_core/storage/sql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/sqlalchemy_compat.py` & `dagster-1.7.2rc1/dagster/_core/storage/sqlalchemy_compat.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/sqlite.py` & `dagster-1.7.2rc1/dagster/_core/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/sqlite_storage.py` & `dagster-1.7.2rc1/dagster/_core/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/tags.py` & `dagster-1.7.2rc1/dagster/_core/storage/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/temp_file_manager.py` & `dagster-1.7.2rc1/dagster/_core/storage/temp_file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/storage/upath_io_manager.py` & `dagster-1.7.2rc1/dagster/_core/storage/upath_io_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,50 @@
     def dump_to_path(self, context: OutputContext, obj: Any, path: "UPath"):
         """Child classes should override this method to write the object to the filesystem."""
 
     @abstractmethod
     def load_from_path(self, context: InputContext, path: "UPath") -> Any:
         """Child classes should override this method to load the object from the filesystem."""
 
+    def load_partitions(self, context: InputContext):
+        """This method is responsible for loading partitions.
+        The default implementation assumes that different partitions are stored as independent files.
+        When loading a single partition, it will call `load_from_path` on it.
+        When loading multiple partitions, it will invoke `load_from_path` multiple times over paths produced by
+        `get_path_for_partition` method, and store the results in a dictionary with formatted partitions as keys.
+        Sometimes, this is not desired. If the serialization format natively supports loading multiple partitions at once, this method should be overridden together with `get_path_for_partition`.
+        hint: context.asset_partition_keys can be used to access the partitions to load.
+        """
+        paths = self._get_paths_for_partitions(context)  # paths for normal partitions
+        backcompat_paths = self._get_multipartition_backcompat_paths(
+            context
+        )  # paths for multipartitions
+
+        context.log.debug(f"Loading {len(context.asset_partition_keys)} partitions...")
+
+        if len(context.asset_partition_keys) == 1:
+            partition_key = context.asset_partition_keys[0]
+            return self._load_partition_from_path(
+                context, partition_key, paths[partition_key], backcompat_paths.get(partition_key)
+            )
+        else:
+            objs = {}
+
+            for partition_key in context.asset_partition_keys:
+                obj = self._load_partition_from_path(
+                    context,
+                    partition_key,
+                    paths[partition_key],
+                    backcompat_paths.get(partition_key),
+                )
+                if obj is not None:  # in case some partitions were skipped
+                    objs[partition_key] = obj
+
+            return objs
+
     @property
     def fs(self) -> AbstractFileSystem:
         """Utility function to get the IOManager filesystem.
 
         Returns:
             AbstractFileSystem: fsspec filesystem.
 
@@ -168,15 +204,15 @@
         """Override this method if you want to use a different partitioning scheme
         (for example, if the saving function handles partitioning instead).
         The extension will be added later.
 
         Args:
             context (Union[InputContext, OutputContext]): The context for the I/O operation.
             path (UPath): The path to the file or object.
-            partition (str): Formatted partition/multipartition key
+            partition (str): slash-formatted partition/multipartition key
 
         Returns:
             UPath: The path to the file with the partition key appended.
         """
         return path / partition
 
     def _get_paths_for_partitions(
@@ -227,39 +263,22 @@
         asset_path = self._get_path_without_extension(context)
         return {
             partition_key: self._with_extension(asset_path / partition_key)
             for partition_key in partition_keys
             if isinstance(partition_key, MultiPartitionKey)
         }
 
-    def _load_single_input(
-        self, path: "UPath", context: InputContext, backcompat_path: Optional["UPath"] = None
-    ) -> Any:
+    def _load_single_input(self, path: "UPath", context: InputContext) -> Any:
         context.log.debug(self.get_loading_input_log_message(path))
-        try:
-            obj = self.load_from_path(context=context, path=path)
-            if asyncio.iscoroutine(obj):
-                obj = asyncio.run(obj)
-        except FileNotFoundError as e:
-            if backcompat_path is not None:
-                try:
-                    obj = self.load_from_path(context=context, path=backcompat_path)
-                    if asyncio.iscoroutine(obj):
-                        obj = asyncio.run(obj)
-
-                    context.log.debug(
-                        f"File not found at {path}. Loaded instead from backcompat path:"
-                        f" {backcompat_path}"
-                    )
-                except FileNotFoundError:
-                    raise e
-            else:
-                raise e
+        obj = self.load_from_path(context=context, path=path)
+        if asyncio.iscoroutine(obj):
+            obj = asyncio.run(obj)
 
         context.add_input_metadata({"path": MetadataValue.path(str(path))})
+
         return obj
 
     def _load_partition_from_path(
         self,
         context: InputContext,
         partition_key: str,
         path: "UPath",
@@ -270,15 +289,15 @@
         3. If allow_missing_partitions metadata is True, skip the partition if it was not found in any of the paths.
         Otherwise, raise an error.
 
         Args:
             context (InputContext): IOManager Input context
             partition_key (str): the partition key corresponding to the partition being loaded
             path (UPath): The path to the partition.
-            backcompat_path (Optional[UPath]): The path to the partition in the backcompat location.
+            backcompat_path (Optional[UPath]): The path to the partition in the backcompat location. These paths can be present in assets produced by very old Dagster versions (TODO: specify concrete version).
 
         Returns:
             Any: The object loaded from the partition.
         """
         allow_missing_partitions = (
             context.definition_metadata.get("allow_missing_partitions", False)
             if context.definition_metadata is not None
@@ -288,151 +307,123 @@
         try:
             context.log.debug(self.get_loading_input_partition_log_message(path, partition_key))
             obj = self.load_from_path(context=context, path=path)
             return obj
         except FileNotFoundError as e:
             if backcompat_path is not None:
                 try:
-                    obj = self.load_from_path(context=context, path=path)
+                    obj = self.load_from_path(context=context, path=backcompat_path)
                     context.log.debug(
                         f"File not found at {path}. Loaded instead from backcompat path:"
                         f" {backcompat_path}"
                     )
                     return obj
-                except FileNotFoundError as e:
+                except FileNotFoundError:
                     if allow_missing_partitions:
                         context.log.warning(self.get_missing_partition_log_message(partition_key))
                         return None
                     else:
                         raise e
             if allow_missing_partitions:
                 context.log.warning(self.get_missing_partition_log_message(partition_key))
                 return None
             else:
                 raise e
 
-    def _load_multiple_inputs(self, context: InputContext) -> Dict[str, Any]:
-        # load multiple partitions
+    def load_partitions_async(self, context: InputContext):
+        """Same as `load_partitions`, but for async."""
         paths = self._get_paths_for_partitions(context)  # paths for normal partitions
         backcompat_paths = self._get_multipartition_backcompat_paths(
             context
         )  # paths for multipartitions
 
-        context.log.debug(f"Loading {len(paths)} partitions...")
+        async def collect():
+            loop = asyncio.get_running_loop()
 
-        objs = {}
+            tasks = []
 
-        if not inspect.iscoroutinefunction(self.load_from_path):
             for partition_key in context.asset_partition_keys:
-                obj = self._load_partition_from_path(
-                    context,
-                    partition_key,
-                    paths[partition_key],
-                    backcompat_paths.get(partition_key),
-                )
-                if obj is not None:  # in case some partitions were skipped
-                    objs[partition_key] = obj
-            return objs
-        else:
-            # load_from_path returns a coroutine, so we need to await the results
-
-            async def collect():
-                loop = asyncio.get_running_loop()
-
-                tasks = []
-
-                for partition_key in context.asset_partition_keys:
-                    tasks.append(
-                        loop.create_task(
-                            self._load_partition_from_path(
-                                context,
-                                partition_key,
-                                paths[partition_key],
-                                backcompat_paths.get(partition_key),
-                            )
+                tasks.append(
+                    loop.create_task(
+                        self._load_partition_from_path(
+                            context,
+                            partition_key,
+                            paths[partition_key],
+                            backcompat_paths.get(partition_key),
                         )
                     )
+                )
 
-                results = await asyncio.gather(*tasks, return_exceptions=True)
+            results = await asyncio.gather(*tasks, return_exceptions=True)
 
-                # need to handle missing partitions here because exceptions don't get propagated from async calls
-                allow_missing_partitions = (
-                    context.definition_metadata.get("allow_missing_partitions", False)
-                    if context.definition_metadata is not None
-                    else False
-                )
+            # need to handle missing partitions here because exceptions don't get propagated from async calls
+            allow_missing_partitions = (
+                context.definition_metadata.get("allow_missing_partitions", False)
+                if context.definition_metadata is not None
+                else False
+            )
 
-                results_without_errors = []
-                found_errors = False
-                for partition_key, result in zip(context.asset_partition_keys, results):
-                    if isinstance(result, FileNotFoundError):
-                        if allow_missing_partitions:
-                            context.log.warning(
-                                self.get_missing_partition_log_message(partition_key)
-                            )
-                        else:
-                            context.log.error(str(result))
-                            found_errors = True
-                    elif isinstance(result, Exception):
+            results_without_errors = []
+            found_errors = False
+            for partition_key, result in zip(context.asset_partition_keys, results):
+                if isinstance(result, FileNotFoundError):
+                    if allow_missing_partitions:
+                        context.log.warning(self.get_missing_partition_log_message(partition_key))
+                    else:
                         context.log.error(str(result))
                         found_errors = True
-                    else:
-                        results_without_errors.append(result)
+                elif isinstance(result, Exception):
+                    context.log.error(str(result))
+                    found_errors = True
+                else:
+                    results_without_errors.append(result)
 
                 if found_errors:
                     raise RuntimeError(
                         f"{len(paths) - len(results_without_errors)} partitions could not be loaded"
                     )
 
-                return results_without_errors
+            return results_without_errors
 
-            awaited_objects = asyncio.get_event_loop().run_until_complete(collect())
+        awaited_objects = asyncio.get_event_loop().run_until_complete(collect())
 
-            return {
-                partition_key: awaited_object
-                for partition_key, awaited_object in zip(
-                    context.asset_partition_keys, awaited_objects
-                )
-                if awaited_object is not None
-            }
+        return {
+            partition_key: awaited_object
+            for partition_key, awaited_object in zip(context.asset_partition_keys, awaited_objects)
+            if awaited_object is not None
+        }
+
+    def _load_partitions(self, context: InputContext) -> Dict[str, Any]:
+        # load multiple partitions
+        if not inspect.iscoroutinefunction(self.load_from_path):
+            return self.load_partitions(context)
+        else:
+            # load_from_path returns a coroutine, so we need to await the results
+            return self.load_partitions_async(context)
 
     def load_input(self, context: InputContext) -> Union[Any, Dict[str, Any]]:
         # If no asset key, we are dealing with an op output which is always non-partitioned
         if not context.has_asset_key or not context.has_asset_partitions:
             path = self._get_path(context)
             return self._load_single_input(path, context)
         else:
+            # we are loading asset partitions
             asset_partition_keys = context.asset_partition_keys
             if len(asset_partition_keys) == 0:
                 return None
-            elif len(asset_partition_keys) == 1:
-                paths = self._get_paths_for_partitions(context)
-                check.invariant(len(paths) == 1, f"Expected 1 path, but got {len(paths)}")
-                path = next(iter(paths.values()))
-                backcompat_paths = self._get_multipartition_backcompat_paths(context)
-                backcompat_path = (
-                    None if not backcompat_paths else next(iter(backcompat_paths.values()))
-                )
-
-                return self._load_single_input(path, context, backcompat_path)
-            else:  # we are dealing with multiple partitions of an asset
-                type_annotation = context.dagster_type.typing_type
-                if type_annotation != Any and not is_dict_type(type_annotation):
-                    check.failed(
-                        "Loading an input that corresponds to multiple partitions, but the"
-                        " type annotation on the op input is not a dict, Dict, Mapping, or"
-                        f" Any: is '{type_annotation}'."
-                    )
-
-                return self._load_multiple_inputs(context)
+            else:
+                return self._load_partitions(context)
 
     def _handle_transition_to_partitioned_asset(self, context: OutputContext, path: "UPath"):
         # if the asset was previously non-partitioned, path will be a file, when it should
         # be a directory for the partitioned asset. Delete the file, so that it can be made
         # into a directory
+
+        # TODO: this might not be the case if the serialization format is already operating with directories
+        # e.g. DeltaLake, zarr
         if path.exists() and path.is_file():
             context.log.warn(
                 f"Found file at {path} believed to correspond with previously non-partitioned version"
                 f" of {context.asset_key}. Removing {path} and replacing with directory for partitioned data files."
             )
             path.unlink(missing_ok=True)
```

### Comparing `dagster-1.7.1/dagster/_core/system_config/composite_descent.py` & `dagster-1.7.2rc1/dagster/_core/system_config/composite_descent.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/system_config/objects.py` & `dagster-1.7.2rc1/dagster/_core/system_config/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/telemetry.py` & `dagster-1.7.2rc1/dagster/_core/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/telemetry_upload.py` & `dagster-1.7.2rc1/dagster/_core/telemetry_upload.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/test_utils.py` & `dagster-1.7.2rc1/dagster/_core/test_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/types/builtin_config_schemas.py` & `dagster-1.7.2rc1/dagster/_core/types/builtin_config_schemas.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/types/config_schema.py` & `dagster-1.7.2rc1/dagster/_core/types/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/types/dagster_type.py` & `dagster-1.7.2rc1/dagster/_core/types/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/types/decorator.py` & `dagster-1.7.2rc1/dagster/_core/types/decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/types/loadable_target_origin.py` & `dagster-1.7.2rc1/dagster/_core/types/loadable_target_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/types/primitive_mapping.py` & `dagster-1.7.2rc1/dagster/_core/types/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/types/python_dict.py` & `dagster-1.7.2rc1/dagster/_core/types/python_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/types/python_set.py` & `dagster-1.7.2rc1/dagster/_core/types/python_set.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/types/python_tuple.py` & `dagster-1.7.2rc1/dagster/_core/types/python_tuple.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/types/transform_typing.py` & `dagster-1.7.2rc1/dagster/_core/types/transform_typing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/utility_ops.py` & `dagster-1.7.2rc1/dagster/_core/utility_ops.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/utils.py` & `dagster-1.7.2rc1/dagster/_core/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/workspace/autodiscovery.py` & `dagster-1.7.2rc1/dagster/_core/workspace/autodiscovery.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/workspace/config_schema.py` & `dagster-1.7.2rc1/dagster/_core/workspace/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/workspace/context.py` & `dagster-1.7.2rc1/dagster/_core/workspace/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 )
 from dagster._core.remote_representation.origin import (
     GrpcServerCodeLocationOrigin,
     ManagedGrpcPythonEnvCodeLocationOrigin,
 )
 from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
 
+from .batch_asset_record_loader import BatchAssetRecordLoader
 from .load_target import WorkspaceLoadTarget
 from .permissions import (
     PermissionResult,
     get_location_scoped_user_permissions,
     get_user_permissions,
 )
 from .workspace import (
@@ -307,14 +308,19 @@
         check.str_param(notebook_path, "notebook_path")
         code_location = self.get_code_location(code_location_name)
         return code_location.get_external_notebook_data(notebook_path=notebook_path)
 
     def get_base_deployment_context(self) -> Optional["BaseWorkspaceRequestContext"]:
         return None
 
+    @property
+    @abstractmethod
+    def asset_record_loader(self) -> BatchAssetRecordLoader:
+        pass
+
 
 class WorkspaceRequestContext(BaseWorkspaceRequestContext):
     def __init__(
         self,
         instance: DagsterInstance,
         workspace_snapshot: Mapping[str, CodeLocationEntry],
         process_context: "IWorkspaceProcessContext",
@@ -330,14 +336,20 @@
         self._source = source
         self._read_only = read_only
         self._read_only_locations = check.opt_mapping_param(
             read_only_locations, "read_only_locations"
         )
         self._checked_permissions: Set[str] = set()
 
+        self._asset_record_loader = BatchAssetRecordLoader(self._instance, {})
+
+    @property
+    def asset_record_loader(self) -> BatchAssetRecordLoader:
+        return self._asset_record_loader
+
     @property
     def instance(self) -> DagsterInstance:
         return self._instance
 
     def get_workspace_snapshot(self) -> Mapping[str, CodeLocationEntry]:
         return self._workspace_snapshot
```

### Comparing `dagster-1.7.1/dagster/_core/workspace/load.py` & `dagster-1.7.2rc1/dagster/_core/workspace/load.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/workspace/load_target.py` & `dagster-1.7.2rc1/dagster/_core/workspace/load_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/workspace/permissions.py` & `dagster-1.7.2rc1/dagster/_core/workspace/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_core/workspace/workspace.py` & `dagster-1.7.2rc1/dagster/_core/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_daemon/__init__.py` & `dagster-1.7.2rc1/dagster/_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_daemon/asset_daemon.py` & `dagster-1.7.2rc1/dagster/_daemon/asset_daemon.py`

 * *Files 0% similar despite different names*

```diff
@@ -979,16 +979,16 @@
             tick_context.add_run_info(run_id=submitted_run.run_id)
 
             # write the submitted run ID to any evaluations
             for asset_key in asset_keys:
                 # asset keys for observation runs don't have evaluations
                 if asset_key in evaluations_by_asset_key:
                     evaluation = evaluations_by_asset_key[asset_key]
-                    evaluations_by_asset_key[asset_key] = evaluation._replace(
-                        run_ids=evaluation.run_ids | {submitted_run.run_id}
+                    evaluations_by_asset_key[asset_key] = evaluation.copy(
+                        update={"run_ids": evaluation.run_ids | {submitted_run.run_id}}
                     )
                     updated_evaluation_asset_keys.add(asset_key)
 
         evaluations_to_update = [
             evaluations_by_asset_key[asset_key] for asset_key in updated_evaluation_asset_keys
         ]
         if evaluations_to_update:
```

### Comparing `dagster-1.7.1/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py` & `dagster-1.7.2rc1/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_daemon/auto_run_reexecution/event_log_consumer.py` & `dagster-1.7.2rc1/dagster/_daemon/auto_run_reexecution/event_log_consumer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_daemon/backfill.py` & `dagster-1.7.2rc1/dagster/_daemon/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_daemon/cli/__init__.py` & `dagster-1.7.2rc1/dagster/_daemon/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_daemon/controller.py` & `dagster-1.7.2rc1/dagster/_daemon/controller.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_daemon/daemon.py` & `dagster-1.7.2rc1/dagster/_daemon/daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_daemon/monitoring/concurrency.py` & `dagster-1.7.2rc1/dagster/_daemon/monitoring/concurrency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_daemon/monitoring/run_monitoring.py` & `dagster-1.7.2rc1/dagster/_daemon/monitoring/run_monitoring.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py` & `dagster-1.7.2rc1/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_daemon/sensor.py` & `dagster-1.7.2rc1/dagster/_daemon/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_daemon/types.py` & `dagster-1.7.2rc1/dagster/_daemon/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_daemon/utils.py` & `dagster-1.7.2rc1/dagster/_daemon/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_daemon/workspace.py` & `dagster-1.7.2rc1/dagster/_daemon/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_generate/download.py` & `dagster-1.7.2rc1/dagster/_generate/download.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_generate/generate.py` & `dagster-1.7.2rc1/dagster/_generate/generate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md` & `dagster-1.7.2rc1/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_grpc/__generated__/api_pb2.py` & `dagster-1.7.2rc1/dagster/_grpc/__generated__/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_grpc/__generated__/api_pb2.pyi` & `dagster-1.7.2rc1/dagster/_grpc/__generated__/api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_grpc/__generated__/api_pb2_grpc.py` & `dagster-1.7.2rc1/dagster/_grpc/__generated__/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_grpc/__init__.py` & `dagster-1.7.2rc1/dagster/_grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_grpc/client.py` & `dagster-1.7.2rc1/dagster/_grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_grpc/compile.py` & `dagster-1.7.2rc1/dagster/_grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_grpc/impl.py` & `dagster-1.7.2rc1/dagster/_grpc/impl.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_grpc/protos/api.proto` & `dagster-1.7.2rc1/dagster/_grpc/protos/api.proto`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_grpc/proxy_server.py` & `dagster-1.7.2rc1/dagster/_grpc/proxy_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_grpc/server.py` & `dagster-1.7.2rc1/dagster/_grpc/server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_grpc/server_watcher.py` & `dagster-1.7.2rc1/dagster/_grpc/server_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_grpc/types.py` & `dagster-1.7.2rc1/dagster/_grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_grpc/utils.py` & `dagster-1.7.2rc1/dagster/_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_loggers/__init__.py` & `dagster-1.7.2rc1/dagster/_loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_model/__init__.py` & `dagster-1.7.2rc1/dagster/_model/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_module_alias_map.py` & `dagster-1.7.2rc1/dagster/_module_alias_map.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_scheduler/scheduler.py` & `dagster-1.7.2rc1/dagster/_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_scheduler/stale.py` & `dagster-1.7.2rc1/dagster/_scheduler/stale.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_serdes/__init__.py` & `dagster-1.7.2rc1/dagster/_serdes/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_serdes/config_class.py` & `dagster-1.7.2rc1/dagster/_serdes/config_class.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     cast,
     overload,
 )
 
 from typing_extensions import Self
 
 import dagster._check as check
+from dagster._core.errors import DagsterImportClassFromCodePointerError
 from dagster._utils import convert_dagster_submodule_name
 from dagster._utils.yaml_utils import load_run_config_yaml
 
 from .serdes import (
     NamedTupleSerializer,
     whitelist_for_serdes,
 )
@@ -91,27 +92,37 @@
     ) -> Union["ConfigurableClass", T_ConfigurableClass]:
         from dagster._config import process_config, resolve_to_config_type
         from dagster._core.errors import DagsterInvalidConfigError
 
         try:
             module = importlib.import_module(self.module_name)
         except ModuleNotFoundError:
-            check.failed(
-                f"Couldn't import module {self.module_name} when attempting to load the "
-                f"configurable class {self.module_name}.{self.class_name}"
-            )
+            module_elems = self.module_name.split(".")
+            if "dagster_cloud" == module_elems[0]:
+                try:
+                    module = importlib.import_module(".".join(["dagster_plus", *module_elems[1:]]))
+                except Exception:
+                    raise DagsterImportClassFromCodePointerError(
+                        f"Couldn't import module {self.module_name} when attempting to load the "
+                        f"configurable class {self.module_name}.{self.class_name}"
+                    )
+            else:
+                raise DagsterImportClassFromCodePointerError(
+                    f"Couldn't import module {self.module_name} when attempting to load the "
+                    f"configurable class {self.module_name}.{self.class_name}"
+                )
         try:
             # All rehydrated classes are expected to implement the ConfigurableClass interface and
             # will error when we call `klass.from_config_value` and `klass.config_type` below if
             # they do not. However, not all rehydrated classes actually have `ConfigurableClass` as
             # an ancestor due to some subtleties around multiple abstract classes that cause an
             # error when `ConfigurableClass` is added as an ancestor to storage classes.
             klass = cast(Type[ConfigurableClass], getattr(module, self.class_name))
         except AttributeError:
-            check.failed(
+            raise DagsterImportClassFromCodePointerError(
                 f"Couldn't find class {self.class_name} in module when attempting to load the "
                 f"configurable class {self.module_name}.{self.class_name}"
             )
 
         if not issubclass(klass, as_type or ConfigurableClass):
             raise check.CheckError(
                 klass,
@@ -214,23 +225,23 @@
         """
 
 
 def class_from_code_pointer(module_name: str, class_name: str) -> Type[object]:
     try:
         module = importlib.import_module(module_name)
     except ModuleNotFoundError:
-        check.failed(
+        raise DagsterImportClassFromCodePointerError(
             "Couldn't import module {module_name} when attempting to load the class {klass}".format(
                 module_name=module_name,
                 klass=module_name + "." + class_name,
             )
         )
     try:
         return getattr(module, class_name)
     except AttributeError:
-        check.failed(
+        raise DagsterImportClassFromCodePointerError(
             "Couldn't find class {class_name} in module when attempting to load the "
             "class {klass}".format(
                 class_name=class_name,
                 klass=module_name + "." + class_name,
             )
         )
```

### Comparing `dagster-1.7.1/dagster/_serdes/ipc.py` & `dagster-1.7.2rc1/dagster/_serdes/ipc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_serdes/serdes.py` & `dagster-1.7.2rc1/dagster/_serdes/serdes.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_serdes/utils.py` & `dagster-1.7.2rc1/dagster/_serdes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_seven/__init__.py` & `dagster-1.7.2rc1/dagster/_seven/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_seven/abc.py` & `dagster-1.7.2rc1/dagster/_seven/abc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_seven/compat/pendulum.py` & `dagster-1.7.2rc1/dagster/_seven/compat/pendulum.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/__init__.py` & `dagster-1.7.2rc1/dagster/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/alert.py` & `dagster-1.7.2rc1/dagster/_utils/alert.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/backoff.py` & `dagster-1.7.2rc1/dagster/_utils/backoff.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/cached_method.py` & `dagster-1.7.2rc1/dagster/_utils/cached_method.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/caching_instance_queryer.py` & `dagster-1.7.2rc1/dagster/_utils/caching_instance_queryer.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
                 value = partitions_def.empty_subset()
             else:
                 value = cache_value.deserialize_materialized_partition_subsets(partitions_def)
         else:
             value = self.asset_partition_has_materialization_or_observation(
                 AssetKeyPartitionKey(asset_key)
             )
-        return AssetSubset(asset_key, value)
+        return AssetSubset(asset_key=asset_key, value=value)
 
     ####################
     # ASSET RECORDS / STORAGE IDS
     ####################
 
     def has_cached_asset_record(self, asset_key: AssetKey) -> bool:
         return asset_key in self._asset_record_cache
@@ -821,15 +821,15 @@
     def get_asset_subset_updated_after_cursor(
         self, *, asset_key: AssetKey, after_cursor: Optional[int]
     ) -> ValidAssetSubset:
         """Returns the AssetSubset of the given asset that has been updated after the given cursor."""
         partitions_def = self.asset_graph.get(asset_key).partitions_def
         if partitions_def is None:
             return ValidAssetSubset(
-                asset_key,
+                asset_key=asset_key,
                 value=self.asset_partition_has_materialization_or_observation(
                     AssetKeyPartitionKey(asset_key), after_cursor=after_cursor
                 ),
             )
         else:
             new_asset_partitions = {
                 ap
```

### Comparing `dagster-1.7.1/dagster/_utils/concurrency.py` & `dagster-1.7.2rc1/dagster/_utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/container.py` & `dagster-1.7.2rc1/dagster/_utils/container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/dagster_type.py` & `dagster-1.7.2rc1/dagster/_utils/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/env.py` & `dagster-1.7.2rc1/dagster/_utils/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/error.py` & `dagster-1.7.2rc1/dagster/_utils/error.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/external.py` & `dagster-1.7.2rc1/dagster/_utils/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/forked_pdb.py` & `dagster-1.7.2rc1/dagster/_utils/forked_pdb.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/hosted_user_process.py` & `dagster-1.7.2rc1/dagster/_utils/hosted_user_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/indenting_printer.py` & `dagster-1.7.2rc1/dagster/_utils/indenting_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/internal_init.py` & `dagster-1.7.2rc1/dagster/_utils/internal_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/interrupts.py` & `dagster-1.7.2rc1/dagster/_utils/interrupts.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/log.py` & `dagster-1.7.2rc1/dagster/_utils/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/merger.py` & `dagster-1.7.2rc1/dagster/_utils/merger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/net.py` & `dagster-1.7.2rc1/dagster/_utils/net.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/schedules.py` & `dagster-1.7.2rc1/dagster/_utils/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/tags.py` & `dagster-1.7.2rc1/dagster/_utils/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/temp_file.py` & `dagster-1.7.2rc1/dagster/_utils/temp_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/test/__init__.py` & `dagster-1.7.2rc1/dagster/_utils/test/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/test/data_versions.py` & `dagster-1.7.2rc1/dagster/_utils/test/data_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/test/mysql_instance.py` & `dagster-1.7.2rc1/dagster/_utils/test/mysql_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/test/postgres_instance.py` & `dagster-1.7.2rc1/dagster/_utils/test/postgres_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/test/schedule_storage.py` & `dagster-1.7.2rc1/dagster/_utils/test/schedule_storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -728,15 +728,17 @@
         assert ticks_by_origin["sensor_one"][0].tick_id == b.tick_id
         assert ticks_by_origin["sensor_two"][0].tick_id == d.tick_id
 
     def test_auto_materialize_asset_evaluations(self, storage) -> None:
         if not self.can_store_auto_materialize_asset_evaluations():
             pytest.skip("Storage cannot store auto materialize asset evaluations")
 
-        condition_snapshot = AssetConditionSnapshot("foo", "bar", "")
+        condition_snapshot = AssetConditionSnapshot(
+            class_name="foo", description="bar", unique_id=""
+        )
 
         for _ in range(2):  # test idempotency
             storage.add_auto_materialize_asset_evaluations(
                 evaluation_id=10,
                 asset_evaluations=[
                     AssetConditionEvaluation(
                         condition_snapshot=condition_snapshot,
@@ -751,16 +753,16 @@
                         condition_snapshot=condition_snapshot,
                         true_subset=AssetSubset(asset_key=AssetKey("asset_two"), value=True),
                         candidate_subset=AssetSubset(asset_key=AssetKey("asset_two"), value=True),
                         start_timestamp=0,
                         end_timestamp=1,
                         subsets_with_metadata=[
                             AssetSubsetWithMetadata(
-                                AssetSubset(asset_key=AssetKey("asset_two"), value=True),
-                                {"foo": MetadataValue.text("bar")},
+                                subset=AssetSubset(asset_key=AssetKey("asset_two"), value=True),
+                                metadata={"foo": MetadataValue.text("bar")},
                             )
                         ],
                         child_evaluations=[],
                     ).with_run_ids(set()),
                 ],
             )
 
@@ -832,25 +834,29 @@
         )
         assert len(res) == 1
         assert res[0].evaluation_id == 10
 
         # add a mix of keys - one that already is using the unique index and one that is not
 
         eval_one = AssetConditionEvaluation(
-            condition_snapshot=AssetConditionSnapshot("foo", "bar", ""),
+            condition_snapshot=AssetConditionSnapshot(
+                class_name="foo", description="bar", unique_id=""
+            ),
             start_timestamp=0,
             end_timestamp=1,
             true_subset=AssetSubset(asset_key=AssetKey("asset_one"), value=True),
             candidate_subset=AssetSubset(asset_key=AssetKey("asset_one"), value=True),
             subsets_with_metadata=[],
             child_evaluations=[],
         ).with_run_ids(set())
 
         eval_asset_three = AssetConditionEvaluation(
-            condition_snapshot=AssetConditionSnapshot("foo", "bar", ""),
+            condition_snapshot=AssetConditionSnapshot(
+                class_name="foo", description="bar", unique_id=""
+            ),
             start_timestamp=0,
             end_timestamp=1,
             true_subset=AssetSubset(asset_key=AssetKey("asset_three"), value=True),
             candidate_subset=AssetSubset(asset_key=AssetKey("asset_three"), value=True),
             subsets_with_metadata=[],
             child_evaluations=[],
         ).with_run_ids(set())
@@ -882,23 +888,28 @@
         if not self.can_store_auto_materialize_asset_evaluations():
             pytest.skip("Storage cannot store auto materialize asset evaluations")
 
         partitions_def = StaticPartitionsDefinition(["a", "b"])
         subset = partitions_def.empty_subset().with_partition_keys(["a"])
         asset_subset = AssetSubset(asset_key=AssetKey("asset_two"), value=subset)
         asset_subset_with_metadata = AssetSubsetWithMetadata(
-            asset_subset,
-            {"foo": MetadataValue.text("bar"), "baz": MetadataValue.asset(AssetKey("asset_one"))},
+            subset=asset_subset,
+            metadata={
+                "foo": MetadataValue.text("bar"),
+                "baz": MetadataValue.asset(AssetKey("asset_one")),
+            },
         )
 
         storage.add_auto_materialize_asset_evaluations(
             evaluation_id=10,
             asset_evaluations=[
                 AssetConditionEvaluation(
-                    condition_snapshot=AssetConditionSnapshot("foo", "bar", ""),
+                    condition_snapshot=AssetConditionSnapshot(
+                        class_name="foo", description="bar", unique_id=""
+                    ),
                     start_timestamp=0,
                     end_timestamp=1,
                     true_subset=asset_subset,
                     candidate_subset=asset_subset,
                     subsets_with_metadata=[asset_subset_with_metadata],
                     child_evaluations=[],
                 ).with_run_ids(set()),
@@ -924,15 +935,17 @@
         if not self.can_purge():
             pytest.skip("Storage cannot purge")
 
         storage.add_auto_materialize_asset_evaluations(
             evaluation_id=11,
             asset_evaluations=[
                 AssetConditionEvaluation(
-                    condition_snapshot=AssetConditionSnapshot("foo", "bar", ""),
+                    condition_snapshot=AssetConditionSnapshot(
+                        class_name="foo", description="bar", unique_id=""
+                    ),
                     start_timestamp=0,
                     end_timestamp=1,
                     true_subset=AssetSubset(asset_key=AssetKey("asset_one"), value=True),
                     candidate_subset=AssetSubset(asset_key=AssetKey("asset_one"), value=True),
                     subsets_with_metadata=[],
                     child_evaluations=[],
                 ).with_run_ids(set()),
```

### Comparing `dagster-1.7.1/dagster/_utils/timing.py` & `dagster-1.7.2rc1/dagster/_utils/timing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/typed_dict.py` & `dagster-1.7.2rc1/dagster/_utils/typed_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/typing_api.py` & `dagster-1.7.2rc1/dagster/_utils/typing_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/warnings.py` & `dagster-1.7.2rc1/dagster/_utils/warnings.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster/_utils/yaml_utils.py` & `dagster-1.7.2rc1/dagster/_utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.1/dagster.egg-info/PKG-INFO` & `dagster-1.7.2rc1/dagster.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.7.1
+Version: 1.7.2rc1
 Summary: Dagster is an orchestration platform for the development, production, and observation of data assets.
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Documentation, https://docs.dagster.io
@@ -102,14 +102,29 @@
 
 <p align="center">
   <img width="100%" alt="An example asset graph as rendered in the Dagster UI" src="https://raw.githubusercontent.com/dagster-io/dagster/master/.github/example-lineage.png">
 </p>
 
 Dagster is built to be used at every stage of the data development lifecycle - local development, unit tests, integration tests, staging environments, all the way up to production.
 
+## Special Event: Introducing Dagster+
+
+<p align="center">
+  <img width="100%" alt="Join us on April 17 (12PM ET) for a special event introducing Dagster+" src="https://i.imgur.com/1r7hOep.png">
+</p>
+
+Join us on April 17 (12PM ET) for a special event introducing Dagster+. [Register for our Dagster+ launch event here](https://dagster.io/events/dagster-plus-launch-event)
+
+In addition to the core open-source project, we are excited to announce Dagster+, the next generation of Dagster's cloud offering.
+
+- Find out how to weave data reliability and quality checks into the execution of your data pipelines.
+- See how diff-based branch deployments will accelerate your development cycle and cut extraneous compute costs.
+- Get a deep understanding of what is driving the cost of your data pipelines, then optimize to get the best cost/performance outcomes.
+- Enjoy the benefits of built-in data cataloging, and asset-level rich metadata.
+
 ## Quick Start:
 
 If you're new to Dagster, we recommend reading about its [core concepts](https://docs.dagster.io/concepts) or learning with the hands-on [tutorial](https://docs.dagster.io/tutorial).
 
 Dagster is available on PyPI and officially supports Python 3.8 through Python 3.12.
 
 ```bash
```

### Comparing `dagster-1.7.1/dagster.egg-info/SOURCES.txt` & `dagster-1.7.2rc1/dagster.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -488,14 +488,15 @@
 dagster/_core/types/primitive_mapping.py
 dagster/_core/types/python_dict.py
 dagster/_core/types/python_set.py
 dagster/_core/types/python_tuple.py
 dagster/_core/types/transform_typing.py
 dagster/_core/workspace/__init__.py
 dagster/_core/workspace/autodiscovery.py
+dagster/_core/workspace/batch_asset_record_loader.py
 dagster/_core/workspace/config_schema.py
 dagster/_core/workspace/context.py
 dagster/_core/workspace/load.py
 dagster/_core/workspace/load_target.py
 dagster/_core/workspace/permissions.py
 dagster/_core/workspace/workspace.py
 dagster/_daemon/__init__.py
```

### Comparing `dagster-1.7.1/dagster.egg-info/requires.txt` & `dagster-1.7.2rc1/dagster.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 structlog
 sqlalchemy<3,>=1.0
 toposort>=1.0
 watchdog>=0.8.3
 docstring-parser
 pydantic!=1.10.7,<3,>1.10.0
 rich
-dagster-pipes==1.7.1
+dagster-pipes==1.7.2rc1
 
 [:platform_system == "Windows"]
 psutil>=1.0
 pywin32!=226
 
 [:python_version < "3.11"]
 protobuf<5,>=3.20.0
```

### Comparing `dagster-1.7.1/setup.py` & `dagster-1.7.2rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         'pywin32!=226; platform_system=="Windows"',
         "docstring-parser",
         "universal_pathlib; python_version<'3.12'",
         "universal_pathlib>=0.2.0; python_version>='3.12'",
         # https://github.com/pydantic/pydantic/issues/5821
         "pydantic>1.10.0,!= 1.10.7,<3",
         "rich",
-        "dagster-pipes==1.7.1",
+        "dagster-pipes==1.7.2rc1",
     ],
     extras_require={
         "docker": ["docker"],
         "test": [
             "buildkite-test-collector",
             "docker",
             f"grpcio-tools>={GRPC_VERSION_FLOOR}",
```

