# Comparing `tmp/dbt-tests-adapter-1.7.9.tar.gz` & `tmp/dbt_tests_adapter-1.8.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-tests-adapter-1.7.9.tar", last modified: Wed Feb 28 21:50:47 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `dbt-tests-adapter-1.7.9.tar` & `dbt_tests_adapter-1.8.0b1.tar`

### file list

```diff
@@ -1,180 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.322361 dbt-tests-adapter-1.7.9/
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-02-28 21:50:47.322361 dbt-tests-adapter-1.7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.290361 dbt-tests-adapter-1.7.9/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.290361 dbt-tests-adapter-1.7.9/dbt/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.294361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.294361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/aliases/
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/aliases/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/aliases/test_aliases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.298361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/expected_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_adapter_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12481 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_docs_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_generic_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_incremental.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_singular_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_snapshot_check_cols.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_snapshot_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_table_materialization.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_validate_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.298361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/caching/
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/caching/test_caching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.298361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/column_types/
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/column_types/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/column_types/test_column_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.298361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/concurrency/
--rw-r--r--   0 runner    (1001) docker     (127)    14683 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/concurrency/test_concurrency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.298361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)    11044 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/constraints/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)    19051 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/constraints/test_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.298361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/dbt_clone/
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/dbt_clone/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/dbt_clone/test_dbt_clone.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.298361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/dbt_debug/
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/dbt_debug/test_dbt_debug.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.298361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/dbt_show/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/dbt_show/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/dbt_show/test_dbt_show.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.298361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/ephemeral/
--rw-r--r--   0 runner    (1001) docker     (127)    12015 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/ephemeral/test_ephemeral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.302361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/grants/
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/grants/base_grants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/grants/test_incremental_grants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/grants/test_invalid_grants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/grants/test_model_grants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/grants/test_seed_grants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/grants/test_snapshot_grants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.302361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)    10041 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/hooks/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)    15090 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/hooks/test_model_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/hooks/test_run_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.302361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/incremental/
--rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/incremental/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/incremental/test_incremental_predicates.py
--rw-r--r--   0 runner    (1001) docker     (127)    17492 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/incremental/test_incremental_unique_id.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.302361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/materialized_view/
--rw-r--r--   0 runner    (1001) docker     (127)     9075 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/materialized_view/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10585 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/materialized_view/changes.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/materialized_view/files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.302361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/persist_docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/persist_docs/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/persist_docs/test_persist_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.302361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/python_model/
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/python_model/test_python_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/python_model/test_spark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.306361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/query_comment/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/query_comment/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/query_comment/test_query_comment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.306361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/relations/
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/relations/test_changing_relation_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.306361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_copy/
--rw-r--r--   0 runner    (1001) docker     (127)    19865 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_copy/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_copy/test_copy_uppercase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_copy/test_simple_copy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.306361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_seed/
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_seed/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)   111485 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_seed/seeds.py
--rw-r--r--   0 runner    (1001) docker     (127)    14227 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_seed/test_seed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_seed/test_seed_type_override.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.306361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_snapshot/
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_snapshot/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_snapshot/seeds.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_snapshot/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_snapshot/test_snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.306361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/store_test_failures_tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/store_test_failures_tests/_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    13030 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/store_test_failures_tests/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/store_test_failures_tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.318361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/base_array_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/base_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.322361 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/data_types/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/data_types/base_data_type_macro.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/data_types/test_type_bigint.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/data_types/test_type_boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/data_types/test_type_float.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/data_types/test_type_int.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/data_types/test_type_numeric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/data_types/test_type_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/data_types/test_type_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_any_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_array_append.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_array_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_array_construct.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_bool_or.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_cast_bool_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_date_spine.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_date_trunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_dateadd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_datediff.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_equals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_escape_single_quotes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_except.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_generate_series.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_get_intervals_between.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_get_powers_of_two.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_intersect.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_last_day.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_listagg.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_null_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_position.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_replace.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_right.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_safe_cast.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_split_part.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_string_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_any_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_array_append.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_array_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_array_construct.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_bool_or.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_cast_bool_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_current_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_date_spine.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_date_trunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_dateadd.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_datediff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_equals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_escape_single_quotes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_except.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_generate_series.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_get_intervals_between.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_get_powers_of_two.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_intersect.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_last_day.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_length.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_listagg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_null_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_position.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_replace.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_right.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_safe_cast.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_split_part.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_string_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_timestamps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_validate_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:50:47.322361 dbt-tests-adapter-1.7.9/dbt_tests_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-02-28 21:50:47.000000 dbt-tests-adapter-1.7.9/dbt_tests_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-02-28 21:50:47.000000 dbt-tests-adapter-1.7.9/dbt_tests_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 21:50:47.000000 dbt-tests-adapter-1.7.9/dbt_tests_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 21:50:47.000000 dbt-tests-adapter-1.7.9/dbt_tests_adapter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-28 21:50:47.000000 dbt-tests-adapter-1.7.9/dbt_tests_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-28 21:50:47.000000 dbt-tests-adapter-1.7.9/dbt_tests_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 21:50:47.322361 dbt-tests-adapter-1.7.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-02-28 21:50:34.000000 dbt-tests-adapter-1.7.9/setup.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/__about__.py
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/aliases/fixtures.py
+-rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/aliases/test_aliases.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/__init__.py
+-rw-r--r--   0        0        0     7617 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/expected_catalog.py
+-rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/files.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_adapter_methods.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_base.py
+-rw-r--r--   0        0        0    12770 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_docs_generate.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_empty.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_ephemeral.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_generic_tests.py
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_incremental.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_singular_tests.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_snapshot_check_cols.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_snapshot_timestamp.py
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_table_materialization.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_validate_connection.py
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/caching/test_caching.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/catalog/files.py
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/catalog/relation_types.py
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/column_types/fixtures.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/column_types/test_column_types.py
+-rw-r--r--   0        0        0    14694 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/concurrency/test_concurrency.py
+-rw-r--r--   0        0        0    11094 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/constraints/fixtures.py
+-rw-r--r--   0        0        0    18494 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/constraints/test_constraints.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/dbt_clone/fixtures.py
+-rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/dbt_clone/test_dbt_clone.py
+-rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/dbt_debug/test_dbt_debug.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/dbt_show/fixtures.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/dbt_show/test_dbt_show.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/empty/test_empty.py
+-rw-r--r--   0        0        0    12159 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/ephemeral/test_ephemeral.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/base_grants.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/test_incremental_grants.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/test_invalid_grants.py
+-rw-r--r--   0        0        0     5581 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/test_model_grants.py
+-rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/test_seed_grants.py
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/test_snapshot_grants.py
+-rw-r--r--   0        0        0    10051 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/hooks/fixtures.py
+-rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/hooks/test_model_hooks.py
+-rw-r--r--   0        0        0     6645 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/hooks/test_run_hooks.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/hooks/data/seed_model.sql
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/hooks/data/seed_run.sql
+-rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/incremental/fixtures.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py
+-rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py
+-rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/incremental/test_incremental_predicates.py
+-rw-r--r--   0        0        0    17895 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/incremental/test_incremental_unique_id.py
+-rw-r--r--   0        0        0     9037 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/materialized_view/basic.py
+-rw-r--r--   0        0        0    10573 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/materialized_view/changes.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/materialized_view/files.py
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/persist_docs/fixtures.py
+-rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/persist_docs/test_persist_docs.py
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/python_model/test_python_model.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/python_model/test_spark.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/query_comment/fixtures.py
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/query_comment/test_query_comment.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/relations/test_changing_relation_type.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/relations/test_dropping_schema_named.py
+-rw-r--r--   0        0        0    19870 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_copy/fixtures.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_copy/test_copy_uppercase.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_copy/test_simple_copy.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_seed/fixtures.py
+-rw-r--r--   0        0        0    33348 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_seed/seed_bom.csv
+-rw-r--r--   0        0        0   111485 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_seed/seeds.py
+-rw-r--r--   0        0        0    14662 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_seed/test_seed.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_seed/test_seed_type_override.py
+-rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_snapshot/common.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_snapshot/seeds.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_snapshot/snapshots.py
+-rw-r--r--   0        0        0     8704 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_snapshot/test_snapshot.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/store_test_failures_tests/_files.py
+-rw-r--r--   0        0        0    13105 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/store_test_failures_tests/basic.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/store_test_failures_tests/fixtures.py
+-rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/unit_testing/test_case_insensitivity.py
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/unit_testing/test_invalid_input.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/unit_testing/test_types.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/base_array_utils.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/base_utils.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_any_value.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_array_append.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_array_concat.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_array_construct.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_bool_or.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_cast_bool_to_text.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_concat.py
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_date_spine.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_date_trunc.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_dateadd.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_datediff.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_equals.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_escape_single_quotes.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_except.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_generate_series.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_get_intervals_between.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_get_powers_of_two.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_hash.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_intersect.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_last_day.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_length.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_listagg.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_null_compare.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_position.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_replace.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_right.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_safe_cast.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_split_part.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_string_literal.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_any_value.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_array_append.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_array_concat.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_array_construct.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_bool_or.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_cast_bool_to_text.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_concat.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_current_timestamp.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_date_spine.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_date_trunc.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_dateadd.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_datediff.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_equals.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_escape_single_quotes.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_except.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_generate_series.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_get_intervals_between.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_get_powers_of_two.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_hash.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_intersect.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_last_day.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_length.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_listagg.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_null_compare.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_position.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_replace.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_right.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_safe_cast.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_split_part.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_string_literal.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_timestamps.py
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_validate_sql.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/base_data_type_macro.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_bigint.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_boolean.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_float.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_int.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_numeric.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_string.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_timestamp.py
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/.gitignore
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/README.md
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/pyproject.toml
+-rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0b1/PKG-INFO
```

### Comparing `dbt-tests-adapter-1.7.9/PKG-INFO` & `dbt_tests_adapter-1.8.0b1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 Metadata-Version: 2.1
 Name: dbt-tests-adapter
-Version: 1.7.9
-Summary: The dbt adapter tests for adapter plugins
-Home-page: https://github.com/dbt-labs/dbt-core/tree/main/tests/adapter
-Author: dbt Labs
-Author-email: info@dbtlabs.com
+Version: 1.8.0b1
+Summary: The set of reusable tests and test fixtures used to test common functionality
+Project-URL: Homepage, https://github.com/dbt-labs/dbt-adapters
+Project-URL: Documentation, https://docs.getdbt.com
+Project-URL: Repository, https://github.com/dbt-labs/dbt-adapters.git
+Project-URL: Issues, https://github.com/dbt-labs/dbt-adapters/issues
+Project-URL: Changelog, https://github.com/dbt-labs/dbt-adapters/blob/main/CHANGELOG.md
+Author-email: dbt Labs <info@dbtlabs.com>
+Maintainer-email: dbt Labs <info@dbtlabs.com>
+Keywords: adapter,adapters,database,dbt,dbt Cloud,dbt Core,dbt Labs,dbt-core,elt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.8.0
+Requires-Dist: dbt-adapters
+Requires-Dist: dbt-core<1.9.0,>=1.8.0a1
+Requires-Dist: pyyaml
+Provides-Extra: build
+Requires-Dist: check-wheel-contents; extra == 'build'
+Requires-Dist: twine; extra == 'build'
+Requires-Dist: wheel; extra == 'build'
 Description-Content-Type: text/markdown
-Requires-Dist: dbt-core==1.7.9
-Requires-Dist: pytest>=7.0.0
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/dbt-labs/dbt-core/fa1ea14ddfb1d5ae319d5141844910dd53ab2834/etc/dbt-core.svg" alt="dbt logo" width="750"/>
+  <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
 
 # dbt-tests-adapter
 
 For context and guidance on using this package, please read: ["Testing a new adapter"](https://docs.getdbt.com/docs/contributing/testing-a-new-adapter)
 
 ## What is it?
```

### Comparing `dbt-tests-adapter-1.7.9/README.md` & `dbt_tests_adapter-1.8.0b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-  <img src="https://raw.githubusercontent.com/dbt-labs/dbt-core/fa1ea14ddfb1d5ae319d5141844910dd53ab2834/etc/dbt-core.svg" alt="dbt logo" width="750"/>
+  <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
 
 # dbt-tests-adapter
 
 For context and guidance on using this package, please read: ["Testing a new adapter"](https://docs.getdbt.com/docs/contributing/testing-a-new-adapter)
 
 ## What is it?
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/aliases/fixtures.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/aliases/fixtures.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,30 +27,30 @@
 """
 
 # base aliases #
 MODELS__SCHEMA_YML = """
 version: 2
 models:
 - name: foo_alias
-  tests:
+  data_tests:
   - expect_value:
       field: tablename
       value: foo
 - name: ref_foo_alias
-  tests:
+  data_tests:
   - expect_value:
       field: tablename
       value: ref_foo_alias
 - name: alias_in_project
-  tests:
+  data_tests:
   - expect_value:
       field: tablename
       value: project_alias
 - name: alias_in_project_with_override
-  tests:
+  data_tests:
   - expect_value:
       field: tablename
       value: override_alias
 
 """
 
 MODELS__FOO_ALIAS_SQL = """
@@ -124,20 +124,20 @@
 """
 
 # dupe custom database #
 MODELS_DUPE_CUSTOM_DATABASE__SCHEMA_YML = """
 version: 2
 models:
 - name: model_a
-  tests:
+  data_tests:
   - expect_value:
       field: tablename
       value: duped_alias
 - name: model_b
-  tests:
+  data_tests:
   - expect_value:
       field: tablename
       value: duped_alias
 
 """
 
 MODELS_DUPE_CUSTOM_DATABASE__MODEL_A_SQL = """
@@ -157,25 +157,25 @@
 """
 
 # dupe custom schema #
 MODELS_DUPE_CUSTOM_SCHEMA__SCHEMA_YML = """
 version: 2
 models:
 - name: model_a
-  tests:
+  data_tests:
   - expect_value:
       field: tablename
       value: duped_alias
 - name: model_b
-  tests:
+  data_tests:
   - expect_value:
       field: tablename
       value: duped_alias
 - name: model_c
-  tests:
+  data_tests:
   - expect_value:
       field: tablename
       value: duped_alias
 
 """
 
 MODELS_DUPE_CUSTOM_SCHEMA__MODEL_A_SQL = """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/aliases/test_aliases.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/aliases/test_aliases.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,11 @@
 import pytest
+
+from dbt.tests.adapter.aliases import fixtures
 from dbt.tests.util import run_dbt
-from dbt.tests.adapter.aliases.fixtures import (
-    MACROS__CAST_SQL,
-    MACROS__EXPECT_VALUE_SQL,
-    MODELS__SCHEMA_YML,
-    MODELS__FOO_ALIAS_SQL,
-    MODELS__ALIAS_IN_PROJECT_SQL,
-    MODELS__ALIAS_IN_PROJECT_WITH_OVERRIDE_SQL,
-    MODELS__REF_FOO_ALIAS_SQL,
-    MODELS_DUPE__MODEL_A_SQL,
-    MODELS_DUPE__MODEL_B_SQL,
-    MODELS_DUPE_CUSTOM_SCHEMA__SCHEMA_YML,
-    MODELS_DUPE_CUSTOM_SCHEMA__MODEL_A_SQL,
-    MODELS_DUPE_CUSTOM_SCHEMA__MODEL_B_SQL,
-    MODELS_DUPE_CUSTOM_SCHEMA__MODEL_C_SQL,
-    MODELS_DUPE_CUSTOM_DATABASE__SCHEMA_YML,
-    MODELS_DUPE_CUSTOM_DATABASE__MODEL_A_SQL,
-    MODELS_DUPE_CUSTOM_DATABASE__MODEL_B_SQL,
-)
 
 
 class BaseAliases:
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "config-version": 2,
@@ -37,24 +21,27 @@
                 }
             },
         }
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "schema.yml": MODELS__SCHEMA_YML,
-            "foo_alias.sql": MODELS__FOO_ALIAS_SQL,
-            "alias_in_project.sql": MODELS__ALIAS_IN_PROJECT_SQL,
-            "alias_in_project_with_override.sql": MODELS__ALIAS_IN_PROJECT_WITH_OVERRIDE_SQL,
-            "ref_foo_alias.sql": MODELS__REF_FOO_ALIAS_SQL,
+            "schema.yml": fixtures.MODELS__SCHEMA_YML,
+            "foo_alias.sql": fixtures.MODELS__FOO_ALIAS_SQL,
+            "alias_in_project.sql": fixtures.MODELS__ALIAS_IN_PROJECT_SQL,
+            "alias_in_project_with_override.sql": fixtures.MODELS__ALIAS_IN_PROJECT_WITH_OVERRIDE_SQL,
+            "ref_foo_alias.sql": fixtures.MODELS__REF_FOO_ALIAS_SQL,
         }
 
     @pytest.fixture(scope="class")
     def macros(self):
-        return {"cast.sql": MACROS__CAST_SQL, "expect_value.sql": MACROS__EXPECT_VALUE_SQL}
+        return {
+            "cast.sql": fixtures.MACROS__CAST_SQL,
+            "expect_value.sql": fixtures.MACROS__EXPECT_VALUE_SQL,
+        }
 
     def test_alias_model_name(self, project):
         results = run_dbt(["run"])
         assert len(results) == 4
         run_dbt(["test"])
 
 
@@ -64,21 +51,24 @@
         return {
             "config-version": 2,
             "macro-paths": ["macros"],
         }
 
     @pytest.fixture(scope="class")
     def macros(self):
-        return {"cast.sql": MACROS__CAST_SQL, "expect_value.sql": MACROS__EXPECT_VALUE_SQL}
+        return {
+            "cast.sql": fixtures.MACROS__CAST_SQL,
+            "expect_value.sql": fixtures.MACROS__EXPECT_VALUE_SQL,
+        }
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "model_a.sql": MODELS_DUPE__MODEL_A_SQL,
-            "model_b.sql": MODELS_DUPE__MODEL_B_SQL,
+            "model_a.sql": fixtures.MODELS_DUPE__MODEL_A_SQL,
+            "model_b.sql": fixtures.MODELS_DUPE__MODEL_B_SQL,
         }
 
     def test_alias_dupe_thorews_exeption(self, project):
         message = ".*identical database representation.*"
         with pytest.raises(Exception) as exc:
             assert message in exc
             run_dbt(["run"])
@@ -90,23 +80,26 @@
         return {
             "config-version": 2,
             "macro-paths": ["macros"],
         }
 
     @pytest.fixture(scope="class")
     def macros(self):
-        return {"cast.sql": MACROS__CAST_SQL, "expect_value.sql": MACROS__EXPECT_VALUE_SQL}
+        return {
+            "cast.sql": fixtures.MACROS__CAST_SQL,
+            "expect_value.sql": fixtures.MACROS__EXPECT_VALUE_SQL,
+        }
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "schema.yml": MODELS_DUPE_CUSTOM_SCHEMA__SCHEMA_YML,
-            "model_a.sql": MODELS_DUPE_CUSTOM_SCHEMA__MODEL_A_SQL,
-            "model_b.sql": MODELS_DUPE_CUSTOM_SCHEMA__MODEL_B_SQL,
-            "model_c.sql": MODELS_DUPE_CUSTOM_SCHEMA__MODEL_C_SQL,
+            "schema.yml": fixtures.MODELS_DUPE_CUSTOM_SCHEMA__SCHEMA_YML,
+            "model_a.sql": fixtures.MODELS_DUPE_CUSTOM_SCHEMA__MODEL_A_SQL,
+            "model_b.sql": fixtures.MODELS_DUPE_CUSTOM_SCHEMA__MODEL_B_SQL,
+            "model_c.sql": fixtures.MODELS_DUPE_CUSTOM_SCHEMA__MODEL_C_SQL,
         }
 
     def test_same_alias_succeeds_in_different_schemas(self, project):
         results = run_dbt(["run"])
         assert len(results) == 3
         res = run_dbt(["test"])
         assert len(res) > 0
@@ -124,22 +117,25 @@
                     "model_b": {"schema": unique_schema + "_alt"},
                 },
             },
         }
 
     @pytest.fixture(scope="class")
     def macros(self):
-        return {"cast.sql": MACROS__CAST_SQL, "expect_value.sql": MACROS__EXPECT_VALUE_SQL}
+        return {
+            "cast.sql": fixtures.MACROS__CAST_SQL,
+            "expect_value.sql": fixtures.MACROS__EXPECT_VALUE_SQL,
+        }
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "schema.yml": MODELS_DUPE_CUSTOM_DATABASE__SCHEMA_YML,
-            "model_a.sql": MODELS_DUPE_CUSTOM_DATABASE__MODEL_A_SQL,
-            "model_b.sql": MODELS_DUPE_CUSTOM_DATABASE__MODEL_B_SQL,
+            "schema.yml": fixtures.MODELS_DUPE_CUSTOM_DATABASE__SCHEMA_YML,
+            "model_a.sql": fixtures.MODELS_DUPE_CUSTOM_DATABASE__MODEL_A_SQL,
+            "model_b.sql": fixtures.MODELS_DUPE_CUSTOM_DATABASE__MODEL_B_SQL,
         }
 
     def test_alias_model_name_diff_database(self, project):
         results = run_dbt(["run"])
         assert len(results) == 2
         res = run_dbt(["test"])
         assert len(res) > 0
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/expected_catalog.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/expected_catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     view_type,
     table_type,
     model_stats,
     seed_stats=None,
     case=None,
     case_columns=False,
 ):
-
     if case is None:
 
         def case(x):
             return x
 
     col_case = case if case_columns else lambda x: x
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/files.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,35 +55,35 @@
 
 generic_test_seed_yml = """
 version: 2
 models:
   - name: base
     columns:
      - name: id
-       tests:
+       data_tests:
          - not_null
 """
 
 generic_test_view_yml = """
 version: 2
 models:
   - name: view_model
     columns:
      - name: id
-       tests:
+       data_tests:
          - not_null
 """
 
 generic_test_table_yml = """
 version: 2
 models:
   - name: table_model
     columns:
      - name: id
-       tests:
+       data_tests:
          - not_null
 """
 
 test_passing_sql = """
 select * from (
     select 1 as id
 ) as my_subquery
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_adapter_methods.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_adapter_methods.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 
-from dbt.tests.util import run_dbt, check_relations_equal
 from dbt.tests.fixtures.project import write_project_files
+from dbt.tests.util import check_relations_equal, run_dbt
 
 
 tests__get_columns_in_relation_sql = """
 {% set columns = adapter.get_columns_in_relation(ref('model')) %}
 {% set limit_query = 0 %}
 {% if (columns | length) == 0 %}
     {% set limit_query = 1 %}
@@ -86,14 +86,25 @@
 
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "name": "adapter_methods",
         }
 
+    @pytest.fixture(autouse=True)
+    def clean_up(self, project):
+        yield
+        with project.adapter.connection_named("__test"):
+            relation = project.adapter.Relation.create(
+                database=project.database, schema=project.test_schema
+            )
+            project.adapter.drop_schema(relation)
+
+    pass
+
     # snowflake need all tables in CAP name
     @pytest.fixture(scope="class")
     def equal_tables(self):
         return ["model", "expected"]
 
     def test_adapter_methods(self, project, equal_tables):
         run_dbt(["compile"])  # trigger any compile-time issues
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_base.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 import pytest
+
+from dbt.tests.adapter.basic import files
 from dbt.tests.util import (
-    run_dbt,
-    check_result_nodes_by_name,
-    relation_from_name,
     check_relation_types,
     check_relations_equal,
-)
-from dbt.tests.adapter.basic.files import (
-    seeds_base_csv,
-    base_view_sql,
-    base_table_sql,
-    base_materialized_var_sql,
-    schema_base_yml,
+    check_result_nodes_by_name,
+    relation_from_name,
+    run_dbt,
 )
 
 
 class BaseSimpleMaterializations:
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "view_model.sql": base_view_sql,
-            "table_model.sql": base_table_sql,
-            "swappable.sql": base_materialized_var_sql,
-            "schema.yml": schema_base_yml,
+            "view_model.sql": files.base_view_sql,
+            "table_model.sql": files.base_table_sql,
+            "swappable.sql": files.base_materialized_var_sql,
+            "schema.yml": files.schema_base_yml,
         }
 
     @pytest.fixture(scope="class")
     def seeds(self):
         return {
-            "base.csv": seeds_base_csv,
+            "base.csv": files.seeds_base_csv,
         }
 
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "name": "base",
         }
 
-    def test_base(self, project):
+    @pytest.fixture(autouse=True)
+    def clean_up(self, project):
+        yield
+        with project.adapter.connection_named("__test"):
+            relation = project.adapter.Relation.create(
+                database=project.database, schema=project.test_schema
+            )
+            project.adapter.drop_schema(relation)
 
+    pass
+
+    def test_base(self, project):
         # seed command
         results = run_dbt(["seed"])
         # seed result length
         assert len(results) == 1
 
         # run command
         results = run_dbt()
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_docs_generate.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_docs_generate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,40 @@
-import pytest
 import os
 from datetime import datetime
-import dbt
 
-from dbt.tests.util import run_dbt, rm_file, get_artifact, check_datetime_between
+import pytest
+
+from dbt.tests.adapter.basic import expected_catalog
 from dbt.tests.fixtures.project import write_project_files
-from dbt.tests.adapter.basic.expected_catalog import (
-    base_expected_catalog,
-    no_stats,
-    expected_references_catalog,
-)
+from dbt.tests.util import run_dbt, rm_file, get_artifact, check_datetime_between
+
 
 models__schema_yml = """
 version: 2
 
 models:
   - name: model
     description: "The test model"
     docs:
       show: false
     columns:
       - name: id
         description: The user ID number
-        tests:
+        data_tests:
           - unique
           - not_null
       - name: first_name
         description: The user's first name
       - name: email
         description: The user's email
       - name: ip_address
         description: The user's IP address
       - name: updated_at
         description: The last time this user's email was updated
-    tests:
+    data_tests:
       - test.nothing
 
   - name: second_model
     description: "The second test model"
     docs:
       show: false
     columns:
@@ -333,16 +330,14 @@
                     found_node[node_key] == expected_node[node_key]
                 ), f"Key '{node_key}' in '{unique_id}' did not match"
 
 
 def verify_metadata(metadata, dbt_schema_version, start_time):
     assert "generated_at" in metadata
     check_datetime_between(metadata["generated_at"], start=start_time)
-    assert "dbt_version" in metadata
-    assert metadata["dbt_version"] == dbt.version.__version__
     assert "dbt_schema_version" in metadata
     assert metadata["dbt_schema_version"] == dbt_schema_version
     key = "env_key"
     if os.name == "nt":
         key = key.upper()
     assert metadata["env"] == {key: "env_value"}
 
@@ -413,25 +408,37 @@
             "second_model.sql": models__second_model_sql,
             "readme.md": models__readme_md,
             "model.sql": models__model_sql,
         }
 
     @pytest.fixture(scope="class")
     def expected_catalog(self, project, profile_user):
-        return base_expected_catalog(
+        return expected_catalog.base_expected_catalog(
             project,
             role=profile_user,
             id_type="integer",
             text_type="text",
             time_type="timestamp without time zone",
             view_type="VIEW",
             table_type="BASE TABLE",
-            model_stats=no_stats(),
+            model_stats=expected_catalog.no_stats(),
         )
 
+    @pytest.fixture(autouse=True)
+    def clean_up(self, project):
+        yield
+        with project.adapter.connection_named("__test"):
+            alternate_schema = f"{project.test_schema}_test"
+            relation = project.adapter.Relation.create(
+                database=project.database, schema=alternate_schema
+            )
+            project.adapter.drop_schema(relation)
+
+    pass
+
     # Test "--no-compile" flag works and produces no manifest.json
     def test_run_and_generate_no_compile(self, project, expected_catalog):
         start_time = run_and_generate(project, ["--no-compile"])
         assert not os.path.exists(os.path.join(project.project_root, "target", "manifest.json"))
         verify_catalog(project, expected_catalog, start_time)
 
     # Test generic "docs generate" command
@@ -459,24 +466,24 @@
             "ephemeral_summary.sql": ref_models__ephemeral_summary_sql,
             "ephemeral_copy.sql": ref_models__ephemeral_copy_sql,
             "docs.md": ref_models__docs_md,
         }
 
     @pytest.fixture(scope="class")
     def expected_catalog(self, project, profile_user):
-        return expected_references_catalog(
+        return expected_catalog.expected_references_catalog(
             project,
             role=profile_user,
             id_type="integer",
             text_type="text",
             time_type="timestamp without time zone",
             bigint_type="bigint",
             view_type="VIEW",
             table_type="BASE TABLE",
-            model_stats=no_stats(),
+            model_stats=expected_catalog.no_stats(),
         )
 
     def test_references(self, project, expected_catalog):
         start_time = run_and_generate(project)
         verify_catalog(project, expected_catalog, start_time)
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_empty.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_empty.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from dbt.tests.util import run_dbt
 import os
 
+from dbt.tests.util import run_dbt
+
 
 class BaseEmpty:
     def test_empty(self, project):
         # check seed
         results = run_dbt(["seed"])
         assert len(results) == 0
         run_results_path = os.path.join(project.project_root, "target", "run_results.json")
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_ephemeral.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_ephemeral.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,37 @@
-import pytest
 import os
+
+import pytest
+
+from dbt.tests.adapter.basic import files
 from dbt.tests.util import (
-    run_dbt,
-    get_manifest,
     check_relations_equal,
     check_result_nodes_by_name,
+    get_manifest,
     relation_from_name,
-)
-from dbt.tests.adapter.basic.files import (
-    seeds_base_csv,
-    base_ephemeral_sql,
-    ephemeral_view_sql,
-    ephemeral_table_sql,
-    schema_base_yml,
+    run_dbt,
 )
 
 
 class BaseEphemeral:
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {"name": "ephemeral"}
 
     @pytest.fixture(scope="class")
     def seeds(self):
-        return {"base.csv": seeds_base_csv}
+        return {"base.csv": files.seeds_base_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "ephemeral.sql": base_ephemeral_sql,
-            "view_model.sql": ephemeral_view_sql,
-            "table_model.sql": ephemeral_table_sql,
-            "schema.yml": schema_base_yml,
+            "ephemeral.sql": files.base_ephemeral_sql,
+            "view_model.sql": files.ephemeral_view_sql,
+            "table_model.sql": files.ephemeral_table_sql,
+            "schema.yml": files.schema_base_yml,
         }
 
     def test_ephemeral(self, project):
         # seed command
         results = run_dbt(["seed"])
         assert len(results) == 1
         check_result_nodes_by_name(results, ["base"])
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_generic_tests.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_generic_tests.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 import pytest
+
+from dbt.tests.adapter.basic import files
 from dbt.tests.util import run_dbt
-from dbt.tests.adapter.basic.files import (
-    seeds_base_csv,
-    generic_test_seed_yml,
-    base_view_sql,
-    base_table_sql,
-    schema_base_yml,
-    generic_test_view_yml,
-    generic_test_table_yml,
-)
 
 
 class BaseGenericTests:
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {"name": "generic_tests"}
 
     @pytest.fixture(scope="class")
     def seeds(self):
         return {
-            "base.csv": seeds_base_csv,
-            "schema.yml": generic_test_seed_yml,
+            "base.csv": files.seeds_base_csv,
+            "schema.yml": files.generic_test_seed_yml,
         }
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "view_model.sql": base_view_sql,
-            "table_model.sql": base_table_sql,
-            "schema.yml": schema_base_yml,
-            "schema_view.yml": generic_test_view_yml,
-            "schema_table.yml": generic_test_table_yml,
+            "view_model.sql": files.base_view_sql,
+            "table_model.sql": files.base_table_sql,
+            "schema.yml": files.schema_base_yml,
+            "schema_view.yml": files.generic_test_view_yml,
+            "schema_table.yml": files.generic_test_table_yml,
         }
 
+    @pytest.fixture(autouse=True)
+    def clean_up(self, project):
+        yield
+        with project.adapter.connection_named("__test"):
+            relation = project.adapter.Relation.create(
+                database=project.database, schema=project.test_schema
+            )
+            project.adapter.drop_schema(relation)
+
+    pass
+
     def test_generic_tests(self, project):
         # seed command
         results = run_dbt(["seed"])
 
         # test command selecting base model
         results = run_dbt(["test", "-m", "base"])
         assert len(results) == 1
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_incremental.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_incremental.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 import pytest
+
+# TODO: update to new dbt-artifacts once available
+from dbt.artifacts.schemas.results import RunStatus
+from dbt.tests.adapter.basic import files
 from dbt.tests.util import run_dbt, check_relations_equal, relation_from_name
-from dbt.contracts.results import RunStatus
-from dbt.tests.adapter.basic.files import (
-    seeds_base_csv,
-    seeds_added_csv,
-    schema_base_yml,
-    incremental_sql,
-    incremental_not_schema_change_sql,
-)
 
 
 class BaseIncremental:
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {"name": "incremental"}
 
     @pytest.fixture(scope="class")
     def models(self):
-        return {"incremental.sql": incremental_sql, "schema.yml": schema_base_yml}
+        return {"incremental.sql": files.incremental_sql, "schema.yml": files.schema_base_yml}
 
     @pytest.fixture(scope="class")
     def seeds(self):
-        return {"base.csv": seeds_base_csv, "added.csv": seeds_added_csv}
+        return {"base.csv": files.seeds_base_csv, "added.csv": files.seeds_added_csv}
+
+    @pytest.fixture(autouse=True)
+    def clean_up(self, project):
+        yield
+        with project.adapter.connection_named("__test"):
+            relation = project.adapter.Relation.create(
+                database=project.database, schema=project.test_schema
+            )
+            project.adapter.drop_schema(relation)
+
+    pass
 
     def test_incremental(self, project):
         # seed command
         results = run_dbt(["seed"])
         assert len(results) == 2
 
         # base table rowcount
@@ -63,15 +70,15 @@
 class BaseIncrementalNotSchemaChange:
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {"name": "incremental"}
 
     @pytest.fixture(scope="class")
     def models(self):
-        return {"incremental_not_schema_change.sql": incremental_not_schema_change_sql}
+        return {"incremental_not_schema_change.sql": files.incremental_not_schema_change_sql}
 
     def test_incremental_not_schema_change(self, project):
         # Schema change is not evaluated on first run, so two are needed
         run_dbt(["run", "--select", "incremental_not_schema_change"])
         run_result = (
             run_dbt(["run", "--select", "incremental_not_schema_change"]).results[0].status
         )
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_singular_tests.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/relations/test_dropping_schema_named.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 import pytest
-from dbt.tests.adapter.basic.files import (
-    test_passing_sql,
-    test_failing_sql,
-)
-from dbt.tests.util import check_result_nodes_by_name, run_dbt
 
+from dbt.tests.util import get_connection, run_dbt
 
-class BaseSingularTests:
+
+class BaseDropSchemaNamed:
     @pytest.fixture(scope="class")
-    def tests(self):
+    def models(self):
         return {
-            "passing.sql": test_passing_sql,
-            "failing.sql": test_failing_sql,
+            "model_a.sql": "select 1 as id",
         }
 
-    @pytest.fixture(scope="class")
-    def project_config_update(self):
-        return {"name": "singular_tests"}
+    def test_dropped_schema_named_drops_expected_schema(self, project):
+        results = run_dbt(["run"])
+        assert len(results) == 1
+
+        run_dbt(
+            [
+                "run-operation",
+                "drop_schema_named",
+                "--args",
+                f"{{schema_name: {project.test_schema} }}",
+            ]
+        )
+
+        adapter = project.adapter
+        with get_connection(adapter):
+            schemas = adapter.list_schemas(project.database)
 
-    def test_singular_tests(self, project):
-        # test command
-        results = run_dbt(["test"], expect_pass=False)
-        assert len(results) == 2
-
-        # We have the right result nodes
-        check_result_nodes_by_name(results, ["passing", "failing"])
-
-        # Check result status
-        for result in results:
-            if result.node.name == "passing":
-                assert result.status == "pass"
-            elif result.node.name == "failing":
-                assert result.status == "fail"
+        assert project.test_schema not in schemas
 
 
-class TestSingularTests(BaseSingularTests):
+class TestDropSchemaNamed(BaseDropSchemaNamed):
     pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 import pytest
 
-from dbt.tests.util import run_dbt, check_result_nodes_by_name
-from dbt.tests.adapter.basic.files import (
-    seeds_base_csv,
-    ephemeral_with_cte_sql,
-    test_ephemeral_passing_sql,
-    test_ephemeral_failing_sql,
-    schema_base_yml,
-)
+from dbt.tests.adapter.basic import files
+from dbt.tests.util import check_result_nodes_by_name, run_dbt
 
 
 class BaseSingularTestsEphemeral:
     @pytest.fixture(scope="class")
     def seeds(self):
         return {
-            "base.csv": seeds_base_csv,
+            "base.csv": files.seeds_base_csv,
         }
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "ephemeral.sql": ephemeral_with_cte_sql,
-            "passing_model.sql": test_ephemeral_passing_sql,
-            "failing_model.sql": test_ephemeral_failing_sql,
-            "schema.yml": schema_base_yml,
+            "ephemeral.sql": files.ephemeral_with_cte_sql,
+            "passing_model.sql": files.test_ephemeral_passing_sql,
+            "failing_model.sql": files.test_ephemeral_failing_sql,
+            "schema.yml": files.schema_base_yml,
         }
 
     @pytest.fixture(scope="class")
     def tests(self):
         return {
-            "passing.sql": test_ephemeral_passing_sql,
-            "failing.sql": test_ephemeral_failing_sql,
+            "passing.sql": files.test_ephemeral_passing_sql,
+            "failing.sql": files.test_ephemeral_failing_sql,
         }
 
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "name": "singular_tests_ephemeral",
         }
 
+    @pytest.fixture(autouse=True)
+    def clean_up(self, project):
+        yield
+        with project.adapter.connection_named("__test"):
+            relation = project.adapter.Relation.create(
+                database=project.database, schema=project.test_schema
+            )
+            project.adapter.drop_schema(relation)
+
+    pass
+
     def test_singular_tests_ephemeral(self, project):
         # check results from seed command
         results = run_dbt(["seed"])
         assert len(results) == 1
         check_result_nodes_by_name(results, ["base"])
 
         # Check results from test command
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_snapshot_check_cols.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_snapshot_check_cols.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 import pytest
-from dbt.tests.util import run_dbt, update_rows, relation_from_name
-from dbt.tests.adapter.basic.files import (
-    seeds_base_csv,
-    seeds_added_csv,
-    cc_all_snapshot_sql,
-    cc_date_snapshot_sql,
-    cc_name_snapshot_sql,
-)
+
+from dbt.tests.adapter.basic import files
+from dbt.tests.util import relation_from_name, run_dbt, update_rows
 
 
 def check_relation_rows(project, snapshot_name, count):
     relation = relation_from_name(project.adapter, snapshot_name)
     result = project.run_sql(f"select count(*) as num_rows from {relation}", fetch="one")
     assert result[0] == count
 
@@ -19,26 +14,37 @@
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {"name": "snapshot_strategy_check_cols"}
 
     @pytest.fixture(scope="class")
     def seeds(self):
         return {
-            "base.csv": seeds_base_csv,
-            "added.csv": seeds_added_csv,
+            "base.csv": files.seeds_base_csv,
+            "added.csv": files.seeds_added_csv,
         }
 
     @pytest.fixture(scope="class")
     def snapshots(self):
         return {
-            "cc_all_snapshot.sql": cc_all_snapshot_sql,
-            "cc_date_snapshot.sql": cc_date_snapshot_sql,
-            "cc_name_snapshot.sql": cc_name_snapshot_sql,
+            "cc_all_snapshot.sql": files.cc_all_snapshot_sql,
+            "cc_date_snapshot.sql": files.cc_date_snapshot_sql,
+            "cc_name_snapshot.sql": files.cc_name_snapshot_sql,
         }
 
+    @pytest.fixture(autouse=True)
+    def clean_up(self, project):
+        yield
+        with project.adapter.connection_named("__test"):
+            relation = project.adapter.Relation.create(
+                database=project.database, schema=project.test_schema
+            )
+            project.adapter.drop_schema(relation)
+
+    pass
+
     def test_snapshot_check_cols(self, project):
         # seed command
         results = run_dbt(["seed"])
         assert len(results) == 2
 
         # snapshot command
         results = run_dbt(["snapshot"])
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_snapshot_timestamp.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_snapshot_timestamp.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 import pytest
+
+from dbt.tests.adapter.basic import files
 from dbt.tests.util import run_dbt, relation_from_name, update_rows
-from dbt.tests.adapter.basic.files import (
-    seeds_base_csv,
-    seeds_newcolumns_csv,
-    seeds_added_csv,
-    ts_snapshot_sql,
-)
 
 
 def check_relation_rows(project, snapshot_name, count):
     relation = relation_from_name(project.adapter, snapshot_name)
     result = project.run_sql(f"select count(*) as num_rows from {relation}", fetch="one")
     assert result[0] == count
 
 
 class BaseSnapshotTimestamp:
     @pytest.fixture(scope="class")
     def seeds(self):
         return {
-            "base.csv": seeds_base_csv,
-            "newcolumns.csv": seeds_newcolumns_csv,
-            "added.csv": seeds_added_csv,
+            "base.csv": files.seeds_base_csv,
+            "newcolumns.csv": files.seeds_newcolumns_csv,
+            "added.csv": files.seeds_added_csv,
         }
 
     @pytest.fixture(scope="class")
     def snapshots(self):
         return {
-            "ts_snapshot.sql": ts_snapshot_sql,
+            "ts_snapshot.sql": files.ts_snapshot_sql,
         }
 
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {"name": "snapshot_strategy_timestamp"}
 
+    @pytest.fixture(autouse=True)
+    def clean_up(self, project):
+        yield
+        with project.adapter.connection_named("__test"):
+            relation = project.adapter.Relation.create(
+                database=project.database, schema=project.test_schema
+            )
+            project.adapter.drop_schema(relation)
+
+    pass
+
     def test_snapshot_timestamp(self, project):
         # seed command
         results = run_dbt(["seed"])
         assert len(results) == 3
 
         # snapshot command
         results = run_dbt(["snapshot"])
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/basic/test_table_materialization.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/basic/test_table_materialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from dbt.tests.util import run_dbt, check_relations_equal
+from dbt.tests.util import check_relations_equal, run_dbt
 
 
 seeds__seed_csv = """id,first_name,last_name,email,gender,ip_address
 1,Jack,Hunter,jhunter0@pbs.org,Male,59.80.20.168
 2,Kathryn,Walker,kwalker1@ezinearticles.com,Female,194.121.179.35
 3,Gerald,Ryan,gryan2@com.com,Male,11.3.212.243
 4,Bonnie,Spencer,bspencer3@ameblo.jp,Female,216.32.196.175
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/caching/test_caching.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/caching/test_caching.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pytest
 
 from dbt.tests.util import run_dbt
 
+
 model_sql = """
 {{
     config(
         materialized='table'
     )
 }}
 select 1 as id
@@ -87,15 +88,15 @@
 
     def test_cache(self, project):
         # this should only cache the schema containing the selected model
         run_args = ["--cache-selected-only", "run", "--select", "model"]
         self.run_and_inspect_cache(project, run_args)
 
 
-class TestNoPopulateCache(BaseCachingTest):
+class BaseNoPopulateCache(BaseCachingTest):
     @pytest.fixture(scope="class")
     def models(self):
         return {
             "model.sql": model_sql,
         }
 
     def test_cache(self, project):
@@ -111,7 +112,11 @@
 
 class TestCachingUppercaseModel(BaseCachingUppercaseModel):
     pass
 
 
 class TestCachingSelectedSchemaOnly(BaseCachingSelectedSchemaOnly):
     pass
+
+
+class TestNoPopulateCache(BaseNoPopulateCache):
+    pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/column_types/fixtures.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/column_types/fixtures.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     '8'::varchar(20) as varchar_col
 """
 
 schema_yml = """
 version: 2
 models:
   - name: model
-    tests:
+    data_tests:
       - is_type:
           column_map:
             smallint_col: ['integer', 'number']
             int_col: ['integer', 'number']
             bigint_col: ['integer', 'number']
             real_col: ['float', 'number']
             double_col: ['float', 'number']
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/column_types/test_column_types.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/column_types/test_column_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import pytest
+
+from dbt.tests.adapter.column_types import fixtures
 from dbt.tests.util import run_dbt
-from dbt.tests.adapter.column_types.fixtures import macro_test_is_type_sql, model_sql, schema_yml
 
 
 class BaseColumnTypes:
     @pytest.fixture(scope="class")
     def macros(self):
-        return {"test_is_type.sql": macro_test_is_type_sql}
+        return {"test_is_type.sql": fixtures.macro_test_is_type_sql}
 
     def run_and_test(self):
         results = run_dbt(["run"])
         assert len(results) == 1
         results = run_dbt(["test"])
         assert len(results) == 1
 
 
-class TestPostgresColumnTypes(BaseColumnTypes):
+class BasePostgresColumnTypes(BaseColumnTypes):
     @pytest.fixture(scope="class")
     def models(self):
-        return {"model.sql": model_sql, "schema.yml": schema_yml}
+        return {"model.sql": fixtures.model_sql, "schema.yml": fixtures.schema_yml}
 
     def test_run_and_test(self, project):
         self.run_and_test()
+
+
+class TestPostgresColumnTypes(BasePostgresColumnTypes):
+    pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/concurrency/test_concurrency.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/concurrency/test_concurrency.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from dbt.tests.util import (
     check_relations_equal,
     check_table_does_not_exist,
     rm_file,
     run_dbt,
     run_dbt_and_capture,
     write_file,
@@ -298,16 +299,14 @@
             "table_b.sql": models__table_b_sql,
             "view_model.sql": models__view_model_sql,
             "dep.sql": models__dep_sql,
             "view_with_conflicting_cascade.sql": models__view_with_conflicting_cascade_sql,
             "skip.sql": models__skip_sql,
         }
 
-
-class TestConcurenncy(BaseConcurrency):
     def test_concurrency(self, project):
         run_dbt(["seed", "--select", "seed"])
         results = run_dbt(["run"], expect_pass=False)
         assert len(results) == 7
         check_relations_equal(project.adapter, ["seed", "view_model"])
         check_relations_equal(project.adapter, ["seed", "dep"])
         check_relations_equal(project.adapter, ["seed", "table_a"])
@@ -324,7 +323,11 @@
         check_relations_equal(project.adapter, ["seed", "dep"])
         check_relations_equal(project.adapter, ["seed", "table_a"])
         check_relations_equal(project.adapter, ["seed", "table_b"])
         check_table_does_not_exist(project.adapter, "invalid")
         check_table_does_not_exist(project.adapter, "skip")
 
         assert "PASS=5 WARN=0 ERROR=1 SKIP=1 TOTAL=7" in output
+
+
+class TestConcurenncy(BaseConcurrency):
+    pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/constraints/fixtures.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/constraints/fixtures.py`

 * *Files 15% similar despite different names*

```diff
@@ -275,15 +275,15 @@
         constraints:
           - type: not_null
           - type: primary_key
           - type: check
             expression: (id > 0)
           - type: check
             expression: id >= 1
-        tests:
+        data_tests:
           - unique
       - name: color
         data_type: text
       - name: date_day
         data_type: text
   - name: my_model_error
     config:
@@ -294,15 +294,15 @@
         data_type: integer
         description: hello
         constraints:
           - type: not_null
           - type: primary_key
           - type: check
             expression: (id > 0)
-        tests:
+        data_tests:
           - unique
       - name: color
         data_type: text
       - name: date_day
         data_type: text
   - name: my_model_wrong_order
     config:
@@ -313,15 +313,15 @@
         data_type: integer
         description: hello
         constraints:
           - type: not_null
           - type: primary_key
           - type: check
             expression: (id > 0)
-        tests:
+        data_tests:
           - unique
       - name: color
         data_type: text
       - name: date_day
         data_type: text
   - name: my_model_wrong_name
     config:
@@ -332,15 +332,15 @@
         data_type: integer
         description: hello
         constraints:
           - type: not_null
           - type: primary_key
           - type: check
             expression: (id > 0)
-        tests:
+        data_tests:
           - unique
       - name: color
         data_type: text
       - name: date_day
         data_type: text
 """
 
@@ -361,15 +361,15 @@
           - type: check
             expression: (id > 0)
           - type: check
             expression: id >= 1
           - type: foreign_key
             expression: {schema}.foreign_key_model (id)
           - type: unique
-        tests:
+        data_tests:
           - unique
       - name: color
         data_type: text
       - name: date_day
         data_type: text
   - name: my_model_error
     config:
@@ -380,15 +380,15 @@
         data_type: integer
         description: hello
         constraints:
           - type: not_null
           - type: primary_key
           - type: check
             expression: (id > 0)
-        tests:
+        data_tests:
           - unique
       - name: color
         data_type: text
       - name: date_day
         data_type: text
   - name: my_model_wrong_order
     config:
@@ -399,15 +399,15 @@
         data_type: integer
         description: hello
         constraints:
           - type: not_null
           - type: primary_key
           - type: check
             expression: (id > 0)
-        tests:
+        data_tests:
           - unique
       - name: color
         data_type: text
       - name: date_day
         data_type: text
   - name: my_model_wrong_name
     config:
@@ -418,15 +418,15 @@
         data_type: integer
         description: hello
         constraints:
           - type: not_null
           - type: primary_key
           - type: check
             expression: (id > 0)
-        tests:
+        data_tests:
           - unique
       - name: color
         data_type: text
       - name: date_day
         data_type: text
   - name: foreign_key_model
     config:
@@ -462,15 +462,15 @@
         expression: {schema}.foreign_key_model (id)
     columns:
       - name: id
         data_type: integer
         description: hello
         constraints:
           - type: not_null
-        tests:
+        data_tests:
           - unique
       - name: color
         data_type: text
       - name: date_day
         data_type: text
   - name: foreign_key_model
     config:
@@ -513,15 +513,15 @@
         columns: [ '"from"' ]
     columns:
       - name: id
         data_type: integer
         description: hello
         constraints:
           - type: not_null
-        tests:
+        data_tests:
           - unique
       - name: from  # reserved word
         quote: true
         data_type: text
         constraints:
           - type: not_null
       - name: date_day
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/constraints/test_constraints.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/constraints/test_constraints.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,21 @@
-import pytest
 import re
 
+import pytest
+
+from dbt.tests.adapter.constraints import fixtures
 from dbt.tests.util import (
     run_dbt,
     get_manifest,
     run_dbt_and_capture,
     write_file,
     read_file,
     relation_from_name,
 )
 
-from dbt.tests.adapter.constraints.fixtures import (
-    my_model_sql,
-    my_incremental_model_sql,
-    my_model_wrong_order_sql,
-    my_model_wrong_name_sql,
-    my_model_data_type_sql,
-    model_data_type_schema_yml,
-    my_model_view_wrong_order_sql,
-    my_model_view_wrong_name_sql,
-    my_model_incremental_wrong_order_sql,
-    my_model_incremental_wrong_name_sql,
-    my_model_with_nulls_sql,
-    my_model_incremental_with_nulls_sql,
-    my_model_with_quoted_column_name_sql,
-    model_schema_yml,
-    model_fk_constraint_schema_yml,
-    constrained_model_schema_yml,
-    model_quoted_column_schema_yml,
-    foreign_key_model_sql,
-    my_model_wrong_order_depends_on_fk_sql,
-    my_model_incremental_wrong_order_depends_on_fk_sql,
-    my_model_contract_sql_header_sql,
-    my_model_incremental_contract_sql_header_sql,
-    model_contract_header_schema_yml,
-    create_table_macro_sql,
-    incremental_foreign_key_schema_yml,
-    incremental_foreign_key_model_raw_numbers_sql,
-    incremental_foreign_key_model_stg_numbers_sql,
-)
-
 
 class BaseConstraintsColumnsEqual:
     """
     dbt should catch these mismatches during its "preflight" checks.
     """
 
     @pytest.fixture
@@ -100,18 +72,18 @@
 
         expected = ["id", "error", "missing in definition", "missing in contract"]
         assert all([(exp in log_output or exp.upper() in log_output) for exp in expected])
 
     def test__constraints_wrong_column_data_types(
         self, project, string_type, int_type, schema_string_type, schema_int_type, data_types
     ):
-        for (sql_column_value, schema_data_type, error_data_type) in data_types:
+        for sql_column_value, schema_data_type, error_data_type in data_types:
             # Write parametrized data_type to sql file
             write_file(
-                my_model_data_type_sql.format(sql_value=sql_column_value),
+                fixtures.my_model_data_type_sql.format(sql_value=sql_column_value),
                 "models",
                 "my_model_data_type.sql",
             )
 
             # Write wrong data_type to corresponding schema file
             # Write integer type for all schema yaml values except when testing integer type itself
             wrong_schema_data_type = (
@@ -119,15 +91,15 @@
                 if schema_data_type.upper() != schema_int_type.upper()
                 else schema_string_type
             )
             wrong_schema_error_data_type = (
                 int_type if schema_data_type.upper() != schema_int_type.upper() else string_type
             )
             write_file(
-                model_data_type_schema_yml.format(data_type=wrong_schema_data_type),
+                fixtures.model_data_type_schema_yml.format(data_type=wrong_schema_data_type),
                 "models",
                 "constraints_schema.yml",
             )
 
             results, log_output = run_dbt_and_capture(
                 ["run", "-s", "my_model_data_type"], expect_pass=False
             )
@@ -142,24 +114,24 @@
                 error_data_type,
                 wrong_schema_error_data_type,
                 "data type mismatch",
             ]
             assert all([(exp in log_output or exp.upper() in log_output) for exp in expected])
 
     def test__constraints_correct_column_data_types(self, project, data_types):
-        for (sql_column_value, schema_data_type, _) in data_types:
+        for sql_column_value, schema_data_type, _ in data_types:
             # Write parametrized data_type to sql file
             write_file(
-                my_model_data_type_sql.format(sql_value=sql_column_value),
+                fixtures.my_model_data_type_sql.format(sql_value=sql_column_value),
                 "models",
                 "my_model_data_type.sql",
             )
             # Write correct data_type to corresponding schema file
             write_file(
-                model_data_type_schema_yml.format(data_type=schema_data_type),
+                fixtures.model_data_type_schema_yml.format(data_type=schema_data_type),
                 "models",
                 "constraints_schema.yml",
             )
 
             run_dbt(["run", "-s", "my_model_data_type"])
 
             manifest = get_manifest(project.project_root)
@@ -188,17 +160,17 @@
     passed into the DDL statement. If they don't match up with the underlying data,
     the data platform should raise an error at runtime.
     """
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "my_model.sql": my_model_wrong_order_depends_on_fk_sql,
-            "foreign_key_model.sql": foreign_key_model_sql,
-            "constraints_schema.yml": model_fk_constraint_schema_yml,
+            "my_model.sql": fixtures.my_model_wrong_order_depends_on_fk_sql,
+            "foreign_key_model.sql": fixtures.foreign_key_model_sql,
+            "constraints_schema.yml": fixtures.model_fk_constraint_schema_yml,
         }
 
     @pytest.fixture(scope="class")
     def expected_sql(self):
         return """
 create table <model_identifier> (
     id integer not null primary key check ((id > 0)) check (id >= 1) references <foreign_key_model_identifier> (id) unique,
@@ -250,21 +222,21 @@
         assert _normalize_whitespace(expected_sql) == _normalize_whitespace(generated_sql_generic)
 
 
 class BaseConstraintsRollback:
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "my_model.sql": my_model_sql,
-            "constraints_schema.yml": model_schema_yml,
+            "my_model.sql": fixtures.my_model_sql,
+            "constraints_schema.yml": fixtures.model_schema_yml,
         }
 
     @pytest.fixture(scope="class")
     def null_model_sql(self):
-        return my_model_with_nulls_sql
+        return fixtures.my_model_with_nulls_sql
 
     @pytest.fixture(scope="class")
     def expected_color(self):
         return "blue"
 
     @pytest.fixture(scope="class")
     def expected_error_messages(self):
@@ -304,61 +276,61 @@
         self.assert_expected_error_messages(failing_results[0].message, expected_error_messages)
 
 
 class BaseTableConstraintsColumnsEqual(BaseConstraintsColumnsEqual):
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "my_model_wrong_order.sql": my_model_wrong_order_sql,
-            "my_model_wrong_name.sql": my_model_wrong_name_sql,
-            "constraints_schema.yml": model_schema_yml,
+            "my_model_wrong_order.sql": fixtures.my_model_wrong_order_sql,
+            "my_model_wrong_name.sql": fixtures.my_model_wrong_name_sql,
+            "constraints_schema.yml": fixtures.model_schema_yml,
         }
 
 
 class BaseViewConstraintsColumnsEqual(BaseConstraintsColumnsEqual):
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "my_model_wrong_order.sql": my_model_view_wrong_order_sql,
-            "my_model_wrong_name.sql": my_model_view_wrong_name_sql,
-            "constraints_schema.yml": model_schema_yml,
+            "my_model_wrong_order.sql": fixtures.my_model_view_wrong_order_sql,
+            "my_model_wrong_name.sql": fixtures.my_model_view_wrong_name_sql,
+            "constraints_schema.yml": fixtures.model_schema_yml,
         }
 
 
 class BaseIncrementalConstraintsColumnsEqual(BaseConstraintsColumnsEqual):
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "my_model_wrong_order.sql": my_model_incremental_wrong_order_sql,
-            "my_model_wrong_name.sql": my_model_incremental_wrong_name_sql,
-            "constraints_schema.yml": model_schema_yml,
+            "my_model_wrong_order.sql": fixtures.my_model_incremental_wrong_order_sql,
+            "my_model_wrong_name.sql": fixtures.my_model_incremental_wrong_name_sql,
+            "constraints_schema.yml": fixtures.model_schema_yml,
         }
 
 
 class BaseIncrementalConstraintsRuntimeDdlEnforcement(BaseConstraintsRuntimeDdlEnforcement):
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "my_model.sql": my_model_incremental_wrong_order_depends_on_fk_sql,
-            "foreign_key_model.sql": foreign_key_model_sql,
-            "constraints_schema.yml": model_fk_constraint_schema_yml,
+            "my_model.sql": fixtures.my_model_incremental_wrong_order_depends_on_fk_sql,
+            "foreign_key_model.sql": fixtures.foreign_key_model_sql,
+            "constraints_schema.yml": fixtures.model_fk_constraint_schema_yml,
         }
 
 
 class BaseIncrementalConstraintsRollback(BaseConstraintsRollback):
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "my_model.sql": my_incremental_model_sql,
-            "constraints_schema.yml": model_schema_yml,
+            "my_model.sql": fixtures.my_incremental_model_sql,
+            "constraints_schema.yml": fixtures.model_schema_yml,
         }
 
     @pytest.fixture(scope="class")
     def null_model_sql(self):
-        return my_model_incremental_with_nulls_sql
+        return fixtures.my_model_incremental_with_nulls_sql
 
 
 class TestTableConstraintsColumnsEqual(BaseTableConstraintsColumnsEqual):
     pass
 
 
 class TestViewConstraintsColumnsEqual(BaseViewConstraintsColumnsEqual):
@@ -400,25 +372,25 @@
         assert model_config.contract.enforced
 
 
 class BaseTableContractSqlHeader(BaseContractSqlHeader):
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "my_model_contract_sql_header.sql": my_model_contract_sql_header_sql,
-            "constraints_schema.yml": model_contract_header_schema_yml,
+            "my_model_contract_sql_header.sql": fixtures.my_model_contract_sql_header_sql,
+            "constraints_schema.yml": fixtures.model_contract_header_schema_yml,
         }
 
 
 class BaseIncrementalContractSqlHeader(BaseContractSqlHeader):
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "my_model_contract_sql_header.sql": my_model_incremental_contract_sql_header_sql,
-            "constraints_schema.yml": model_contract_header_schema_yml,
+            "my_model_contract_sql_header.sql": fixtures.my_model_incremental_contract_sql_header_sql,
+            "constraints_schema.yml": fixtures.model_contract_header_schema_yml,
         }
 
 
 class TestTableContractSqlHeader(BaseTableContractSqlHeader):
     pass
 
 
@@ -432,17 +404,17 @@
     passed into the DDL statement. If they don't match up with the underlying data,
     the data platform should raise an error at runtime.
     """
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "my_model.sql": my_model_wrong_order_depends_on_fk_sql,
-            "foreign_key_model.sql": foreign_key_model_sql,
-            "constraints_schema.yml": constrained_model_schema_yml,
+            "my_model.sql": fixtures.my_model_wrong_order_depends_on_fk_sql,
+            "foreign_key_model.sql": fixtures.foreign_key_model_sql,
+            "constraints_schema.yml": fixtures.constrained_model_schema_yml,
         }
 
     @pytest.fixture(scope="class")
     def expected_sql(self):
         return """
 create table <model_identifier> (
     id integer not null,
@@ -500,16 +472,16 @@
     pass
 
 
 class BaseConstraintQuotedColumn(BaseConstraintsRuntimeDdlEnforcement):
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "my_model.sql": my_model_with_quoted_column_name_sql,
-            "constraints_schema.yml": model_quoted_column_schema_yml,
+            "my_model.sql": fixtures.my_model_with_quoted_column_name_sql,
+            "constraints_schema.yml": fixtures.model_quoted_column_schema_yml,
         }
 
     @pytest.fixture(scope="class")
     def expected_sql(self):
         return """
 create table <model_identifier> (
     id integer not null,
@@ -532,33 +504,37 @@
 """
 
 
 class TestConstraintQuotedColumn(BaseConstraintQuotedColumn):
     pass
 
 
-class TestIncrementalForeignKeyConstraint:
+class BaseIncrementalForeignKeyConstraint:
     @pytest.fixture(scope="class")
     def macros(self):
         return {
-            "create_table.sql": create_table_macro_sql,
+            "create_table.sql": fixtures.create_table_macro_sql,
         }
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "schema.yml": incremental_foreign_key_schema_yml,
-            "raw_numbers.sql": incremental_foreign_key_model_raw_numbers_sql,
-            "stg_numbers.sql": incremental_foreign_key_model_stg_numbers_sql,
+            "schema.yml": fixtures.incremental_foreign_key_schema_yml,
+            "raw_numbers.sql": fixtures.incremental_foreign_key_model_raw_numbers_sql,
+            "stg_numbers.sql": fixtures.incremental_foreign_key_model_stg_numbers_sql,
         }
 
     def test_incremental_foreign_key_constraint(self, project):
         unformatted_constraint_schema_yml = read_file("models", "schema.yml")
         write_file(
             unformatted_constraint_schema_yml.format(schema=project.test_schema),
             "models",
             "schema.yml",
         )
 
         run_dbt(["run", "--select", "raw_numbers"])
         run_dbt(["run", "--select", "stg_numbers"])
         run_dbt(["run", "--select", "stg_numbers"])
+
+
+class TestIncrementalForeignKeyConstraint(BaseIncrementalForeignKeyConstraint):
+    pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/dbt_clone/fixtures.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/dbt_clone/fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 schema_yml = """
 version: 2
 models:
   - name: view_model
     columns:
       - name: id
-        tests:
+        data_tests:
           - unique:
               severity: error
           - not_null
       - name: name
 """
 
 get_schema_name_sql = """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/dbt_clone/test_dbt_clone.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/dbt_clone/test_dbt_clone.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,60 +1,48 @@
-import os
-import shutil
 from collections import Counter
 from copy import deepcopy
+import os
+import shutil
 
+from dbt_common.exceptions import DbtRuntimeError
 import pytest
 
-from dbt.exceptions import DbtRuntimeError
-from dbt.tests.adapter.dbt_clone.fixtures import (
-    seed_csv,
-    table_model_sql,
-    view_model_sql,
-    ephemeral_model_sql,
-    exposures_yml,
-    schema_yml,
-    snapshot_sql,
-    get_schema_name_sql,
-    macros_sql,
-    infinite_macros_sql,
-    custom_can_clone_tables_false_macros_sql,
-)
+from dbt.tests.adapter.dbt_clone import fixtures
 from dbt.tests.util import run_dbt, run_dbt_and_capture
 
 
 class BaseClone:
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "table_model.sql": table_model_sql,
-            "view_model.sql": view_model_sql,
-            "ephemeral_model.sql": ephemeral_model_sql,
-            "schema.yml": schema_yml,
-            "exposures.yml": exposures_yml,
+            "table_model.sql": fixtures.table_model_sql,
+            "view_model.sql": fixtures.view_model_sql,
+            "ephemeral_model.sql": fixtures.ephemeral_model_sql,
+            "schema.yml": fixtures.schema_yml,
+            "exposures.yml": fixtures.exposures_yml,
         }
 
     @pytest.fixture(scope="class")
     def macros(self):
         return {
-            "macros.sql": macros_sql,
-            "infinite_macros.sql": infinite_macros_sql,
-            "get_schema_name.sql": get_schema_name_sql,
+            "macros.sql": fixtures.macros_sql,
+            "infinite_macros.sql": fixtures.infinite_macros_sql,
+            "get_schema_name.sql": fixtures.get_schema_name_sql,
         }
 
     @pytest.fixture(scope="class")
     def seeds(self):
         return {
-            "seed.csv": seed_csv,
+            "seed.csv": fixtures.seed_csv,
         }
 
     @pytest.fixture(scope="class")
     def snapshots(self):
         return {
-            "snapshot.sql": snapshot_sql,
+            "snapshot.sql": fixtures.snapshot_sql,
         }
 
     @pytest.fixture(scope="class")
     def other_schema(self, unique_schema):
         return unique_schema + "_other"
 
     @property
@@ -156,18 +144,18 @@
             run_dbt(clone_args)
 
 
 class BaseCloneNotPossible(BaseClone):
     @pytest.fixture(scope="class")
     def macros(self):
         return {
-            "macros.sql": macros_sql,
-            "my_can_clone_tables.sql": custom_can_clone_tables_false_macros_sql,
-            "infinite_macros.sql": infinite_macros_sql,
-            "get_schema_name.sql": get_schema_name_sql,
+            "macros.sql": fixtures.macros_sql,
+            "my_can_clone_tables.sql": fixtures.custom_can_clone_tables_false_macros_sql,
+            "infinite_macros.sql": fixtures.infinite_macros_sql,
+            "get_schema_name.sql": fixtures.get_schema_name_sql,
         }
 
     def test_can_clone_false(self, project, unique_schema, other_schema):
         project.create_test_schema(other_schema)
         self.run_and_save_state(project.project_root, with_snapshot=True)
 
         clone_args = [
@@ -215,20 +203,24 @@
                 database=project.database, schema=project.test_schema
             )
             project.adapter.drop_schema(relation)
 
     pass
 
 
-class TestCloneSameTargetAndState(BaseClone):
+class BaseCloneSameTargetAndState(BaseClone):
     def test_clone_same_target_and_state(self, project, unique_schema, other_schema):
         project.create_test_schema(other_schema)
         self.run_and_save_state(project.project_root)
 
         clone_args = [
             "clone",
             "--state",
             "target",
         ]
 
         results, output = run_dbt_and_capture(clone_args, expect_pass=False)
         assert "Warning: The state and target directories are the same: 'target'" in output
+
+
+class TestCloneSameTargetAndState(BaseCloneSameTargetAndState):
+    pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/dbt_debug/test_dbt_debug.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/dbt_debug/test_dbt_debug.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-import pytest
 import os
 import re
-import yaml
 
+# TODO: does this belong in dbt-tests-adapters?
 from dbt.cli.exceptions import DbtUsageException
+import pytest
+import yaml
+
 from dbt.tests.util import run_dbt, run_dbt_and_capture
 
+
 MODELS__MODEL_SQL = """
 seled 1 as id
 """
 
 
 class BaseDebug:
     @pytest.fixture(scope="class")
@@ -42,15 +45,15 @@
 
 class BaseDebugProfileVariable(BaseDebug):
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {"config-version": 2, "profile": '{{ "te" ~ "st" }}'}
 
 
-class TestDebugPostgres(BaseDebug):
+class BaseDebugPostgres(BaseDebug):
     def test_ok(self, project):
         run_dbt(["debug"])
         assert "ERROR" not in self.capsys.readouterr().out
 
     def test_connection_flag(self, project):
         """Testing that the --connection flag works as expected, including that output is not lost"""
         _, out = run_dbt_and_capture(["debug", "--connection"])
@@ -78,19 +81,19 @@
         self.assertGotValue(re.compile(r"\s+Connection test"), "ERROR")
 
     def test_empty_target(self, project):
         run_dbt(["debug", "--target", "none_target"], expect_pass=False)
         self.assertGotValue(re.compile(r"\s+output 'none_target'"), "misconfigured")
 
 
-class TestDebugProfileVariablePostgres(BaseDebugProfileVariable):
+class TestDebugPostgres(BaseDebugPostgres):
     pass
 
 
-class TestDebugInvalidProjectPostgres(BaseDebug):
+class BaseDebugInvalidProjectPostgres(BaseDebug):
     def test_empty_project(self, project):
         with open("dbt_project.yml", "w") as f:  # noqa: F841
             pass
 
         run_dbt(["debug", "--profile", "test"], expect_pass=False)
         splitout = self.capsys.readouterr().out.split("\n")
         self.check_project(splitout)
@@ -121,7 +124,11 @@
 
     def test_profile_not_found(self, project):
         _, out = run_dbt_and_capture(
             ["debug", "--connection", "--profile", "NONE"], expect_pass=False
         )
         assert "Profile loading failed for the following reason" in out
         assert "Could not find profile named 'NONE'" in out
+
+
+class TestDebugInvalidProjectPostgres(BaseDebugInvalidProjectPostgres):
+    pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/dbt_show/fixtures.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/dbt_show/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/dbt_show/test_dbt_show.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/dbt_show/test_dbt_show.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,50 @@
 import pytest
-from dbt.tests.util import run_dbt
 
-from dbt.tests.adapter.dbt_show.fixtures import (
-    models__sql_header,
-    models__ephemeral_model,
-    models__second_ephemeral_model,
-    models__sample_model,
-    seeds__sample_seed,
-)
+from dbt.tests.adapter.dbt_show import fixtures
+from dbt.tests.util import run_dbt
 
 
 # -- Below we define base classes for tests you import based on if your adapter supports dbt show or not --
 class BaseShowLimit:
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "sample_model.sql": models__sample_model,
-            "ephemeral_model.sql": models__ephemeral_model,
+            "sample_model.sql": fixtures.models__sample_model,
+            "ephemeral_model.sql": fixtures.models__ephemeral_model,
         }
 
     @pytest.fixture(scope="class")
     def seeds(self):
-        return {"sample_seed.csv": seeds__sample_seed}
+        return {"sample_seed.csv": fixtures.seeds__sample_seed}
 
     @pytest.mark.parametrize(
         "args,expected",
         [
             ([], 5),  # default limit
             (["--limit", 3], 3),  # fetch 3 rows
             (["--limit", -1], 7),  # fetch all rows
         ],
     )
     def test_limit(self, project, args, expected):
         run_dbt(["build"])
-        dbt_args = ["show", "--inline", models__second_ephemeral_model, *args]
+        dbt_args = ["show", "--inline", fixtures.models__second_ephemeral_model, *args]
         results = run_dbt(dbt_args)
         assert len(results.results[0].agate_table) == expected
         # ensure limit was injected in compiled_code when limit specified in command args
         limit = results.args.get("limit")
         if limit > 0:
             assert f"limit {limit}" in results.results[0].node.compiled_code
 
 
 class BaseShowSqlHeader:
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "sql_header.sql": models__sql_header,
+            "sql_header.sql": fixtures.models__sql_header,
         }
 
     def test_sql_header(self, project):
         run_dbt(["show", "--select", "sql_header", "--vars", "timezone: Asia/Kolkata"])
 
 
 class TestPostgresShowSqlHeader(BaseShowSqlHeader):
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/ephemeral/test_ephemeral.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/ephemeral/test_ephemeral.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-import pytest
-import re
 import os
-from dbt.tests.util import run_dbt, check_relations_equal
+import re
+
+import pytest
+
+from dbt.tests.util import check_relations_equal, run_dbt
 
 
 models__dependent_sql = """
 
 -- multiple ephemeral refs should share a cte
 select * from {{ref('base')}} where gender = 'Male'
 union all
@@ -242,16 +244,14 @@
             "base": {
                 "female_only.sql": models__base__female_only_sql,
                 "base.sql": models__base__base_sql,
                 "base_copy.sql": models__base__base_copy_sql,
             },
         }
 
-
-class TestEphemeralMulti(BaseEphemeralMulti):
     def test_ephemeral_multi(self, project):
         run_dbt(["seed"])
         results = run_dbt(["run"])
         assert len(results) == 3
 
         check_relations_equal(project.adapter, ["seed", "dependent"])
         check_relations_equal(project.adapter, ["seed", "double_dependent"])
@@ -275,15 +275,19 @@
             ");"
         )
         sql_file = "".join(sql_file.split())
         expected_sql = "".join(expected_sql.split())
         assert sql_file == expected_sql
 
 
-class TestEphemeralNested(BaseEphemeral):
+class TestEphemeralMulti(BaseEphemeralMulti):
+    pass
+
+
+class BaseEphemeralNested(BaseEphemeral):
     @pytest.fixture(scope="class")
     def models(self):
         return {
             "ephemeral_level_two.sql": models_n__ephemeral_level_two_sql,
             "root_view.sql": models_n__root_view_sql,
             "ephemeral.sql": models_n__ephemeral_sql,
             "source_table.sql": models_n__source_table_sql,
@@ -308,15 +312,19 @@
         )
 
         sql_file = "".join(sql_file.split())
         expected_sql = "".join(expected_sql.split())
         assert sql_file == expected_sql
 
 
-class TestEphemeralErrorHandling(BaseEphemeral):
+class TestEphemeralNested(BaseEphemeralNested):
+    pass
+
+
+class BaseEphemeralErrorHandling(BaseEphemeral):
     @pytest.fixture(scope="class")
     def models(self):
         return {
             "dependent.sql": ephemeral_errors__dependent_sql,
             "base": {
                 "base.sql": ephemeral_errors__base__base_sql,
                 "base_copy.sql": ephemeral_errors__base__base_copy_sql,
@@ -324,7 +332,11 @@
         }
 
     def test_ephemeral_error_handling(self, project):
         results = run_dbt(["run"], expect_pass=False)
         assert len(results) == 1
         assert results[0].status == "skipped"
         assert "Compilation Error" in results[0].message
+
+
+class TestEphemeralErrorHandling(BaseEphemeralErrorHandling):
+    pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/grants/base_grants.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/base_grants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-import pytest
 import os
-from dbt.tests.util import (
-    relation_from_name,
-    get_connection,
-)
+
+# TODO: does this belong in dbt-tests-adapter?
 from dbt.context.base import BaseContext  # diff_of_two_dicts only
+import pytest
+
+from dbt.tests.util import get_connection, relation_from_name
+
 
 TEST_USER_ENV_VARS = ["DBT_TEST_USER_1", "DBT_TEST_USER_2", "DBT_TEST_USER_3"]
 
 
 def replace_all(text, dic):
     for i, j in dic.items():
         text = text.replace(i, j)
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/grants/test_incremental_grants.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/test_incremental_grants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import pytest
+
+from dbt.tests.adapter.grants.base_grants import BaseGrants
 from dbt.tests.util import (
+    get_connection,
+    get_manifest,
+    relation_from_name,
     run_dbt,
     run_dbt_and_capture,
-    get_manifest,
     write_file,
-    relation_from_name,
-    get_connection,
 )
-from dbt.tests.adapter.grants.base_grants import BaseGrants
+
 
 my_incremental_model_sql = """
   select 1 as fun
 """
 
 incremental_model_schema_yml = """
 version: 2
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/grants/test_invalid_grants.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/test_invalid_grants.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import pytest
-from dbt.tests.util import (
-    run_dbt_and_capture,
-    write_file,
-)
+
 from dbt.tests.adapter.grants.base_grants import BaseGrants
+from dbt.tests.util import run_dbt_and_capture, write_file
+
 
 my_invalid_model_sql = """
   select 1 as fun
 """
 
 invalid_user_table_model_schema_yml = """
 version: 2
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/grants/test_model_grants.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/test_model_grants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import pytest
+
+from dbt.tests.adapter.grants.base_grants import BaseGrants
 from dbt.tests.util import (
-    run_dbt_and_capture,
     get_manifest,
+    run_dbt_and_capture,
     write_file,
 )
-from dbt.tests.adapter.grants.base_grants import BaseGrants
+
 
 my_model_sql = """
   select 1 as fun
 """
 
 model_schema_yml = """
 version: 2
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/grants/test_seed_grants.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/test_seed_grants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import pytest
+
+from dbt.tests.adapter.grants.base_grants import BaseGrants
 from dbt.tests.util import (
+    get_manifest,
     run_dbt,
     run_dbt_and_capture,
-    get_manifest,
     write_file,
 )
-from dbt.tests.adapter.grants.base_grants import BaseGrants
+
 
 seeds__my_seed_csv = """
 id,name,some_date
 1,Easton,1981-05-20T06:46:51
 2,Lillian,1978-09-03T18:10:33
 """.lstrip()
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/grants/test_snapshot_grants.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/grants/test_snapshot_grants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import pytest
+
+from dbt.tests.adapter.grants.base_grants import BaseGrants
 from dbt.tests.util import (
+    get_manifest,
     run_dbt,
     run_dbt_and_capture,
-    get_manifest,
     write_file,
 )
-from dbt.tests.adapter.grants.base_grants import BaseGrants
+
 
 my_snapshot_sql = """
 {% snapshot my_snapshot %}
     {{ config(
         check_cols='all', unique_key='id', strategy='check',
         target_database=database, target_schema=schema
     ) }}
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/hooks/fixtures.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/hooks/fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,25 +337,25 @@
 
 properties__seed_models = """
 version: 2
 seeds:
 - name: example_seed
   columns:
   - name: new_col
-    tests:
+    data_tests:
     - not_null
 """
 
 properties__test_snapshot_models = """
 version: 2
 snapshots:
 - name: example_snapshot
   columns:
   - name: new_col
-    tests:
+    data_tests:
     - not_null
 """
 
 seeds__example_seed_csv = """a,b,c
 1,2,3
 4,5,6
 7,8,9
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/hooks/test_model_hooks.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/hooks/test_model_hooks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,17 @@
-import pytest
-
 from pathlib import Path
 
-from dbt.exceptions import CompilationError, ParsingError
+from dbt_common.exceptions import CompilationError
+# TODO: does this belong in dbt-tests-adapter?
+from dbt.exceptions import ParsingError
+import pytest
+
+from dbt.tests.adapter.hooks import fixtures
+from dbt.tests.util import run_dbt, write_file
 
-from dbt.tests.util import (
-    run_dbt,
-    write_file,
-)
-
-from dbt.tests.adapter.hooks.fixtures import (
-    models__hooked,
-    models__hooks,
-    models__hooks_configured,
-    models__hooks_error,
-    models__hooks_kwargs,
-    models__post,
-    models__pre,
-    properties__seed_models,
-    properties__test_snapshot_models,
-    seeds__example_seed_csv,
-    snapshots__test_snapshot,
-)
 
 MODEL_PRE_HOOK = """
    insert into {{this.schema}}.on_model_hook (
         test_state,
         target_dbname,
         target_host,
         target_name,
@@ -80,15 +66,15 @@
     '{{ run_started_at }}',
     '{{ invocation_id }}',
     '{{ thread_id }}'
    )
 """
 
 
-class BaseTestPrePost(object):
+class BaseTestPrePost:
     @pytest.fixture(scope="class", autouse=True)
     def setUp(self, project):
         project.run_sql_file(project.test_data_dir / Path("seed_model.sql"))
 
     def get_ctx_vars(self, state, count, project):
         fields = [
             "test_state",
@@ -131,15 +117,15 @@
             ), "run_started_at was not set"
             assert (
                 ctx["invocation_id"] is not None and len(ctx["invocation_id"]) > 0
             ), "invocation_id was not set"
             assert ctx["thread_id"].startswith("Thread-")
 
 
-class TestPrePostModelHooks(BaseTestPrePost):
+class BasePrePostModelHooks(BaseTestPrePost):
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "models": {
                 "test": {
                     "pre-hook": [
                         # inside transaction (runs second)
@@ -155,23 +141,27 @@
                     ],
                 }
             }
         }
 
     @pytest.fixture(scope="class")
     def models(self):
-        return {"hooks.sql": models__hooks}
+        return {"hooks.sql": fixtures.models__hooks}
 
     def test_pre_and_post_run_hooks(self, project, dbt_profile_target):
         run_dbt()
         self.check_hooks("start", project, dbt_profile_target.get("host", None))
         self.check_hooks("end", project, dbt_profile_target.get("host", None))
 
 
-class TestPrePostModelHooksUnderscores(TestPrePostModelHooks):
+class TestPrePostModelHooks(BasePrePostModelHooks):
+    pass
+
+
+class TestPrePostModelHooksUnderscores(BasePrePostModelHooks):
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "models": {
                 "test": {
                     "pre_hook": [
                         # inside transaction (runs second)
@@ -186,15 +176,15 @@
                         MODEL_POST_HOOK,
                     ],
                 }
             }
         }
 
 
-class TestHookRefs(BaseTestPrePost):
+class BaseHookRefs(BaseTestPrePost):
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "models": {
                 "test": {
                     "hooked": {
                         "post-hook": [
@@ -217,30 +207,38 @@
                     }
                 },
             }
         }
 
     @pytest.fixture(scope="class")
     def models(self):
-        return {"hooked.sql": models__hooked, "post.sql": models__post, "pre.sql": models__pre}
+        return {
+            "hooked.sql": fixtures.models__hooked,
+            "post.sql": fixtures.models__post,
+            "pre.sql": fixtures.models__pre,
+        }
 
     def test_pre_post_model_hooks_refed(self, project, dbt_profile_target):
         run_dbt()
         self.check_hooks("start", project, dbt_profile_target.get("host", None))
         self.check_hooks("end", project, dbt_profile_target.get("host", None))
 
 
-class TestPrePostModelHooksOnSeeds(object):
+class TestHookRefs(BaseHookRefs):
+    pass
+
+
+class BasePrePostModelHooksOnSeeds:
     @pytest.fixture(scope="class")
     def seeds(self):
-        return {"example_seed.csv": seeds__example_seed_csv}
+        return {"example_seed.csv": fixtures.seeds__example_seed_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
-        return {"schema.yml": properties__seed_models}
+        return {"schema.yml": fixtures.properties__seed_models}
 
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "seed-paths": ["seeds"],
             "models": {},
             "seeds": {
@@ -257,27 +255,31 @@
     def test_hooks_on_seeds(self, project):
         res = run_dbt(["seed"])
         assert len(res) == 1, "Expected exactly one item"
         res = run_dbt(["test"])
         assert len(res) == 1, "Expected exactly one item"
 
 
-class TestHooksRefsOnSeeds:
+class TestPrePostModelHooksOnSeeds(BasePrePostModelHooksOnSeeds):
+    pass
+
+
+class BaseHooksRefsOnSeeds:
     """
     This should not succeed, and raise an explicit error
     https://github.com/dbt-labs/dbt-core/issues/6806
     """
 
     @pytest.fixture(scope="class")
     def seeds(self):
-        return {"example_seed.csv": seeds__example_seed_csv}
+        return {"example_seed.csv": fixtures.seeds__example_seed_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
-        return {"schema.yml": properties__seed_models, "post.sql": models__post}
+        return {"schema.yml": fixtures.properties__seed_models, "post.sql": fixtures.models__post}
 
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "seeds": {
                 "post-hook": [
                     "select * from {{ ref('post') }}",
@@ -287,15 +289,19 @@
 
     def test_hook_with_ref_on_seeds(self, project):
         with pytest.raises(ParsingError) as excinfo:
             run_dbt(["parse"])
         assert "Seeds cannot depend on other nodes" in str(excinfo.value)
 
 
-class TestPrePostModelHooksOnSeedsPlusPrefixed(TestPrePostModelHooksOnSeeds):
+class TestHooksRefsOnSeeds(BaseHooksRefsOnSeeds):
+    pass
+
+
+class BasePrePostModelHooksOnSeedsPlusPrefixed(BasePrePostModelHooksOnSeeds):
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "seed-paths": ["seeds"],
             "models": {},
             "seeds": {
                 "+post-hook": [
@@ -303,15 +309,19 @@
                     "update {{ this }} set new_col = 1",
                 ],
                 "quote_columns": False,
             },
         }
 
 
-class TestPrePostModelHooksOnSeedsPlusPrefixedWhitespace(TestPrePostModelHooksOnSeeds):
+class TestPrePostModelHooksOnSeedsPlusPrefixed(BasePrePostModelHooksOnSeedsPlusPrefixed):
+    pass
+
+
+class BasePrePostModelHooksOnSeedsPlusPrefixedWhitespace(BasePrePostModelHooksOnSeeds):
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "seed-paths": ["seeds"],
             "models": {},
             "seeds": {
                 "+post-hook": [
@@ -319,28 +329,34 @@
                     "update {{ this }} set new_col = 1",
                 ],
                 "quote_columns": False,
             },
         }
 
 
-class TestPrePostModelHooksOnSnapshots(object):
+class TestPrePostModelHooksOnSeedsPlusPrefixedWhitespace(
+    BasePrePostModelHooksOnSeedsPlusPrefixedWhitespace
+):
+    pass
+
+
+class BasePrePostModelHooksOnSnapshots:
     @pytest.fixture(scope="class", autouse=True)
     def setUp(self, project):
         path = Path(project.project_root) / "test-snapshots"
         Path.mkdir(path)
-        write_file(snapshots__test_snapshot, path, "snapshot.sql")
+        write_file(fixtures.snapshots__test_snapshot, path, "snapshot.sql")
 
     @pytest.fixture(scope="class")
     def models(self):
-        return {"schema.yml": properties__test_snapshot_models}
+        return {"schema.yml": fixtures.properties__test_snapshot_models}
 
     @pytest.fixture(scope="class")
     def seeds(self):
-        return {"example_seed.csv": seeds__example_seed_csv}
+        return {"example_seed.csv": fixtures.seeds__example_seed_csv}
 
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "seed-paths": ["seeds"],
             "snapshot-paths": ["test-snapshots"],
             "models": {},
@@ -360,35 +376,43 @@
         assert len(res) == 1, "Expected exactly one item"
         res = run_dbt(["snapshot"])
         assert len(res) == 1, "Expected exactly one item"
         res = run_dbt(["test"])
         assert len(res) == 1, "Expected exactly one item"
 
 
+class TestPrePostModelHooksOnSnapshots(BasePrePostModelHooksOnSnapshots):
+    pass
+
+
 class PrePostModelHooksInConfigSetup(BaseTestPrePost):
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "macro-paths": ["macros"],
         }
 
     @pytest.fixture(scope="class")
     def models(self):
-        return {"hooks.sql": models__hooks_configured}
+        return {"hooks.sql": fixtures.models__hooks_configured}
 
 
-class TestPrePostModelHooksInConfig(PrePostModelHooksInConfigSetup):
+class BasePrePostModelHooksInConfig(PrePostModelHooksInConfigSetup):
     def test_pre_and_post_model_hooks_model(self, project, dbt_profile_target):
         run_dbt()
 
         self.check_hooks("start", project, dbt_profile_target.get("host", None))
         self.check_hooks("end", project, dbt_profile_target.get("host", None))
 
 
-class TestPrePostModelHooksInConfigWithCount(PrePostModelHooksInConfigSetup):
+class TestPrePostModelHooksInConfig(BasePrePostModelHooksInConfig):
+    pass
+
+
+class BasePrePostModelHooksInConfigWithCount(PrePostModelHooksInConfigSetup):
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "models": {
                 "test": {
                     "pre-hook": [
                         # inside transaction (runs second)
@@ -409,26 +433,34 @@
     def test_pre_and_post_model_hooks_model_and_project(self, project, dbt_profile_target):
         run_dbt()
 
         self.check_hooks("start", project, dbt_profile_target.get("host", None), count=2)
         self.check_hooks("end", project, dbt_profile_target.get("host", None), count=2)
 
 
-class TestPrePostModelHooksInConfigKwargs(TestPrePostModelHooksInConfig):
+class TestPrePostModelHooksInConfigWithCount(BasePrePostModelHooksInConfigWithCount):
+    pass
+
+
+class BasePrePostModelHooksInConfigKwargs(BasePrePostModelHooksInConfig):
     @pytest.fixture(scope="class")
     def models(self):
-        return {"hooks.sql": models__hooks_kwargs}
+        return {"hooks.sql": fixtures.models__hooks_kwargs}
+
 
+class TestPrePostModelHooksInConfigKwargs(BasePrePostModelHooksInConfigKwargs):
+    pass
 
-class TestPrePostSnapshotHooksInConfigKwargs(TestPrePostModelHooksOnSnapshots):
+
+class BasePrePostSnapshotHooksInConfigKwargs(BasePrePostModelHooksOnSnapshots):
     @pytest.fixture(scope="class", autouse=True)
     def setUp(self, project):
         path = Path(project.project_root) / "test-kwargs-snapshots"
         Path.mkdir(path)
-        write_file(snapshots__test_snapshot, path, "snapshot.sql")
+        write_file(fixtures.snapshots__test_snapshot, path, "snapshot.sql")
 
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "seed-paths": ["seeds"],
             "snapshot-paths": ["test-kwargs-snapshots"],
             "models": {},
@@ -440,17 +472,25 @@
             },
             "seeds": {
                 "quote_columns": False,
             },
         }
 
 
-class TestDuplicateHooksInConfigs(object):
+class TestPrePostSnapshotHooksInConfigKwargs(BasePrePostSnapshotHooksInConfigKwargs):
+    pass
+
+
+class BaseDuplicateHooksInConfigs:
     @pytest.fixture(scope="class")
     def models(self):
-        return {"hooks.sql": models__hooks_error}
+        return {"hooks.sql": fixtures.models__hooks_error}
 
     def test_run_duplicate_hook_defs(self, project):
         with pytest.raises(CompilationError) as exc:
             run_dbt()
         assert "pre_hook" in str(exc.value)
         assert "pre-hook" in str(exc.value)
+
+
+class TestDuplicateHooksInConfigs(BaseDuplicateHooksInConfigs):
+    pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/hooks/test_run_hooks.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/hooks/test_run_hooks.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,38 @@
 import os
-import pytest
-
 from pathlib import Path
 
-from dbt.tests.adapter.hooks.fixtures import (
-    macros__hook,
-    macros__before_and_after,
-    models__hooks,
-    seeds__example_seed_csv,
-    macros_missing_column,
-    models__missing_column,
-)
-
-from dbt.tests.util import (
-    check_table_does_not_exist,
-    run_dbt,
-)
+import pytest
 
+from dbt.tests.adapter.hooks import fixtures
+from dbt.tests.util import check_table_does_not_exist, run_dbt
 
-class TestPrePostRunHooks(object):
+
+class BasePrePostRunHooks:
     @pytest.fixture(scope="function")
     def setUp(self, project):
         project.run_sql_file(project.test_data_dir / Path("seed_run.sql"))
         project.run_sql(f"drop table if exists { project.test_schema }.schemas")
         project.run_sql(f"drop table if exists { project.test_schema }.db_schemas")
         os.environ["TERM_TEST"] = "TESTING"
 
     @pytest.fixture(scope="class")
     def macros(self):
-        return {"hook.sql": macros__hook, "before-and-after.sql": macros__before_and_after}
+        return {
+            "hook.sql": fixtures.macros__hook,
+            "before-and-after.sql": fixtures.macros__before_and_after,
+        }
 
     @pytest.fixture(scope="class")
     def models(self):
-        return {"hooks.sql": models__hooks}
+        return {"hooks.sql": fixtures.models__hooks}
 
     @pytest.fixture(scope="class")
     def seeds(self):
-        return {"example_seed.csv": seeds__example_seed_csv}
+        return {"example_seed.csv": fixtures.seeds__example_seed_csv}
 
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             # The create and drop table statements here validate that these hooks run
             # in the same order that they are defined. Drop before create is an error.
             # Also check that the table does not exist below.
@@ -139,27 +131,35 @@
         self.check_hooks("end", project, dbt_profile_target.get("host", None))
 
         check_table_does_not_exist(project.adapter, "start_hook_order_test")
         check_table_does_not_exist(project.adapter, "end_hook_order_test")
         self.assert_used_schemas(project)
 
 
-class TestAfterRunHooks(object):
+class TestPrePostRunHooks(BasePrePostRunHooks):
+    pass
+
+
+class BaseAfterRunHooks:
     @pytest.fixture(scope="class")
     def macros(self):
-        return {"temp_macro.sql": macros_missing_column}
+        return {"temp_macro.sql": fixtures.macros_missing_column}
 
     @pytest.fixture(scope="class")
     def models(self):
-        return {"test_column.sql": models__missing_column}
+        return {"test_column.sql": fixtures.models__missing_column}
 
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             # The create and drop table statements here validate that these hooks run
             # in the same order that they are defined. Drop before create is an error.
             # Also check that the table does not exist below.
             "on-run-start": "- {{ export_table_check() }}"
         }
 
     def test_missing_column_pre_hook(self, project):
         run_dbt(["run"], expect_pass=False)
+
+
+class TestAfterRunHooks(BaseAfterRunHooks):
+    pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/incremental/fixtures.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/incremental/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-import pytest
-from dbt.tests.util import run_dbt, check_relations_equal
 from collections import namedtuple
 
+import pytest
+
+from dbt.tests.util import check_relations_equal, run_dbt
+
 
 models__merge_exclude_columns_sql = """
 {{ config(
     materialized = 'incremental',
     unique_key = 'id',
     incremental_strategy='merge',
     merge_exclude_columns=['msg']
@@ -61,15 +63,14 @@
 
     def update_incremental_model(self, incremental_model):
         """update incremental model after the seed table has been updated"""
         model_result_set = run_dbt(["run", "--select", incremental_model])
         return len(model_result_set)
 
     def get_test_fields(self, project, seed, incremental_model, update_sql_file):
-
         seed_count = len(run_dbt(["seed", "--select", seed, "--full-refresh"]))
 
         model_count = len(run_dbt(["run", "--select", incremental_model, "--full-refresh"]))
 
         relation = incremental_model
         # update seed in anticipation of incremental model update
         row_count_query = "select * from {}.{}".format(project.test_schema, seed)
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,32 @@
 import pytest
 
-from dbt.tests.util import (
-    check_relations_equal,
-    run_dbt,
-)
-
-from dbt.tests.adapter.incremental.fixtures import (
-    _MODELS__INCREMENTAL_SYNC_REMOVE_ONLY,
-    _MODELS__INCREMENTAL_IGNORE,
-    _MODELS__INCREMENTAL_SYNC_REMOVE_ONLY_TARGET,
-    _MODELS__INCREMENTAL_IGNORE_TARGET,
-    _MODELS__INCREMENTAL_FAIL,
-    _MODELS__INCREMENTAL_SYNC_ALL_COLUMNS,
-    _MODELS__INCREMENTAL_APPEND_NEW_COLUMNS_REMOVE_ONE,
-    _MODELS__A,
-    _MODELS__INCREMENTAL_APPEND_NEW_COLUMNS_TARGET,
-    _MODELS__INCREMENTAL_APPEND_NEW_COLUMNS,
-    _MODELS__INCREMENTAL_SYNC_ALL_COLUMNS_TARGET,
-    _MODELS__INCREMENTAL_APPEND_NEW_COLUMNS_REMOVE_ONE_TARGET,
-)
+from dbt.tests.adapter.incremental import fixtures
+from dbt.tests.util import check_relations_equal, run_dbt
 
 
 class BaseIncrementalOnSchemaChangeSetup:
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "incremental_sync_remove_only.sql": _MODELS__INCREMENTAL_SYNC_REMOVE_ONLY,
-            "incremental_ignore.sql": _MODELS__INCREMENTAL_IGNORE,
-            "incremental_sync_remove_only_target.sql": _MODELS__INCREMENTAL_SYNC_REMOVE_ONLY_TARGET,
-            "incremental_ignore_target.sql": _MODELS__INCREMENTAL_IGNORE_TARGET,
-            "incremental_fail.sql": _MODELS__INCREMENTAL_FAIL,
-            "incremental_sync_all_columns.sql": _MODELS__INCREMENTAL_SYNC_ALL_COLUMNS,
-            "incremental_append_new_columns_remove_one.sql": _MODELS__INCREMENTAL_APPEND_NEW_COLUMNS_REMOVE_ONE,
-            "model_a.sql": _MODELS__A,
-            "incremental_append_new_columns_target.sql": _MODELS__INCREMENTAL_APPEND_NEW_COLUMNS_TARGET,
-            "incremental_append_new_columns.sql": _MODELS__INCREMENTAL_APPEND_NEW_COLUMNS,
-            "incremental_sync_all_columns_target.sql": _MODELS__INCREMENTAL_SYNC_ALL_COLUMNS_TARGET,
-            "incremental_append_new_columns_remove_one_target.sql": _MODELS__INCREMENTAL_APPEND_NEW_COLUMNS_REMOVE_ONE_TARGET,
+            "incremental_sync_remove_only.sql": fixtures._MODELS__INCREMENTAL_SYNC_REMOVE_ONLY,
+            "incremental_ignore.sql": fixtures._MODELS__INCREMENTAL_IGNORE,
+            "incremental_sync_remove_only_target.sql": fixtures._MODELS__INCREMENTAL_SYNC_REMOVE_ONLY_TARGET,
+            "incremental_ignore_target.sql": fixtures._MODELS__INCREMENTAL_IGNORE_TARGET,
+            "incremental_fail.sql": fixtures._MODELS__INCREMENTAL_FAIL,
+            "incremental_sync_all_columns.sql": fixtures._MODELS__INCREMENTAL_SYNC_ALL_COLUMNS,
+            "incremental_append_new_columns_remove_one.sql": fixtures._MODELS__INCREMENTAL_APPEND_NEW_COLUMNS_REMOVE_ONE,
+            "model_a.sql": fixtures._MODELS__A,
+            "incremental_append_new_columns_target.sql": fixtures._MODELS__INCREMENTAL_APPEND_NEW_COLUMNS_TARGET,
+            "incremental_append_new_columns.sql": fixtures._MODELS__INCREMENTAL_APPEND_NEW_COLUMNS,
+            "incremental_sync_all_columns_target.sql": fixtures._MODELS__INCREMENTAL_SYNC_ALL_COLUMNS_TARGET,
+            "incremental_append_new_columns_remove_one_target.sql": fixtures._MODELS__INCREMENTAL_APPEND_NEW_COLUMNS_REMOVE_ONE_TARGET,
         }
 
     def run_twice_and_assert(self, include, compare_source, compare_target, project):
-
         # dbt run (twice)
         run_args = ["run"]
         if include:
             run_args.extend(("--select", include))
         results_one = run_dbt(run_args)
         assert len(results_one) == 3
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/incremental/test_incremental_predicates.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/incremental/test_incremental_predicates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-import pytest
-from dbt.tests.util import run_dbt, check_relations_equal
 from collections import namedtuple
 
+import pytest
+
+from dbt.tests.util import check_relations_equal, run_dbt
+
 
 models__delete_insert_incremental_predicates_sql = """
 {{ config(
     materialized = 'incremental',
     unique_key = 'id'
 ) }}
 
@@ -73,15 +75,14 @@
         """update incremental model after the seed table has been updated"""
         model_result_set = run_dbt(["run", "--select", incremental_model])
         return len(model_result_set)
 
     def get_test_fields(
         self, project, seed, incremental_model, update_sql_file, opt_model_count=None
     ):
-
         seed_count = len(run_dbt(["seed", "--select", seed, "--full-refresh"]))
 
         model_count = len(run_dbt(["run", "--select", incremental_model, "--full-refresh"]))
         # pass on kwarg
         relation = incremental_model
         # update seed in anticipation of incremental model update
         row_count_query = "select * from {}.{}".format(project.test_schema, seed)
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/incremental/test_incremental_unique_id.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/incremental/test_incremental_unique_id.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-import pytest
-from dbt.tests.util import run_dbt, check_relations_equal
-from dbt.contracts.results import RunStatus
 from collections import namedtuple
 from pathlib import Path
 
+# TODO: repoint to dbt-artifacts when it's available
+from dbt.artifacts.schemas.results import RunStatus
+import pytest
+
+from dbt.tests.util import check_relations_equal, run_dbt
+
+
 models__trinary_unique_key_list_sql = """
 -- a multi-argument unique key list should see overwriting on rows in the model
 --   where all unique key fields apply
 
 {{
     config(
         materialized='incremental',
@@ -340,14 +344,25 @@
     def seeds(self):
         return {
             "duplicate_insert.sql": seeds__duplicate_insert_sql,
             "seed.csv": seeds__seed_csv,
             "add_new_rows.sql": seeds__add_new_rows_sql,
         }
 
+    @pytest.fixture(autouse=True)
+    def clean_up(self, project):
+        yield
+        with project.adapter.connection_named("__test"):
+            relation = project.adapter.Relation.create(
+                database=project.database, schema=project.test_schema
+            )
+            project.adapter.drop_schema(relation)
+
+    pass
+
     def update_incremental_model(self, incremental_model):
         """update incremental model after the seed table has been updated"""
         model_result_set = run_dbt(["run", "--select", incremental_model])
         return len(model_result_set)
 
     def get_test_fields(
         self, project, seed, incremental_model, update_sql_file, opt_model_count=None
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/materialized_view/basic.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/materialized_view/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 from typing import Optional, Tuple
 
 import pytest
 
 from dbt.adapters.base.relation import BaseRelation
-from dbt.contracts.relation import RelationType
+from dbt.adapters.contracts.relation import RelationType
+
+from dbt.tests.adapter.materialized_view import files
 from dbt.tests.util import (
     assert_message_in_logs,
     get_model_file,
     run_dbt,
     run_dbt_and_capture,
     set_model_file,
 )
 
-from dbt.tests.adapter.materialized_view.files import (
-    MY_MATERIALIZED_VIEW,
-    MY_SEED,
-    MY_TABLE,
-    MY_VIEW,
-)
-
 
 class MaterializedViewBasic:
     """
     Tests basic functionality:
 
     - create
     - idempotent create
@@ -62,22 +57,22 @@
 
     """
     Configure these if needed
     """
 
     @pytest.fixture(scope="class", autouse=True)
     def seeds(self):
-        return {"my_seed.csv": MY_SEED}
+        return {"my_seed.csv": files.MY_SEED}
 
     @pytest.fixture(scope="class", autouse=True)
     def models(self):
         yield {
-            "my_table.sql": MY_TABLE,
-            "my_view.sql": MY_VIEW,
-            "my_materialized_view.sql": MY_MATERIALIZED_VIEW,
+            "my_table.sql": files.MY_TABLE,
+            "my_view.sql": files.MY_VIEW,
+            "my_materialized_view.sql": files.MY_MATERIALIZED_VIEW,
         }
 
     """
     Don't configure these unless absolutely necessary
     """
 
     @pytest.fixture(scope="class")
@@ -146,15 +141,14 @@
         new_model = initial_model.replace(
             "materialized='materialized_view'", "materialized='view'"
         )
         set_model_file(project, materialized_view, new_model)
 
     @pytest.fixture(scope="function", autouse=True)
     def setup(self, project, my_materialized_view):
-
         run_dbt(["seed"])
         run_dbt(["run", "--models", my_materialized_view.identifier, "--full-refresh"])
 
         # the tests touch these files, store their contents in memory
         initial_model = get_model_file(project, my_materialized_view)
 
         yield
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/materialized_view/changes.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/materialized_view/changes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from typing import Optional
 
+from dbt_common.contracts.config.materialization import OnConfigurationChangeOption
 import pytest
 
 from dbt.adapters.base.relation import BaseRelation
-from dbt.contracts.graph.model_config import OnConfigurationChangeOption
-from dbt.contracts.relation import RelationType
+from dbt.adapters.contracts.relation import RelationType
+
+from dbt.tests.adapter.materialized_view import files
 from dbt.tests.util import (
     assert_message_in_logs,
     get_model_file,
     run_dbt,
     run_dbt_and_capture,
     set_model_file,
 )
 
-from dbt.tests.adapter.materialized_view.files import (
-    MY_MATERIALIZED_VIEW,
-    MY_SEED,
-)
-
 
 class MaterializedViewChanges:
     """
     Tests change management functionality:
 
     - apply small changes via alter
     - apply large changes via replace
@@ -101,19 +98,19 @@
 
     """
     Configure these if needed
     """
 
     @pytest.fixture(scope="class", autouse=True)
     def seeds(self):
-        yield {"my_seed.csv": MY_SEED}
+        yield {"my_seed.csv": files.MY_SEED}
 
     @pytest.fixture(scope="class", autouse=True)
     def models(self):
-        yield {"my_materialized_view.sql": MY_MATERIALIZED_VIEW}
+        yield {"my_materialized_view.sql": files.MY_MATERIALIZED_VIEW}
 
     """
     Don't configure these unless absolutely necessary
     """
 
     @pytest.fixture(scope="class")
     def my_materialized_view(self, project) -> BaseRelation:
@@ -122,15 +119,14 @@
             schema=project.test_schema,
             database=project.database,
             type=RelationType.MaterializedView,
         )
 
     @pytest.fixture(scope="function", autouse=True)
     def setup(self, project, my_materialized_view):
-
         # make sure the model in the data reflects the files each time
         run_dbt(["seed"])
         run_dbt(["run", "--models", my_materialized_view.identifier, "--full-refresh"])
 
         # the tests touch these files, store their contents in memory
         initial_model = get_model_file(project, my_materialized_view)
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/persist_docs/fixtures.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/persist_docs/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/persist_docs/test_persist_docs.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/persist_docs/test_persist_docs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,38 @@
 import json
 import os
 import pytest
 
+from dbt.tests.adapter.persist_docs import fixtures
 from dbt.tests.util import run_dbt
 
-from dbt.tests.adapter.persist_docs.fixtures import (
-    _DOCS__MY_FUN_DOCS,
-    _MODELS__MISSING_COLUMN,
-    _MODELS__MODEL_USING_QUOTE_UTIL,
-    _MODELS__NO_DOCS_MODEL,
-    _MODELS__TABLE,
-    _MODELS__VIEW,
-    _PROPERTIES__QUOTE_MODEL,
-    _PROPERITES__SCHEMA_MISSING_COL,
-    _PROPERTIES__SCHEMA_YML,
-    _SEEDS__SEED,
-)
-
 
 class BasePersistDocsBase:
     @pytest.fixture(scope="class", autouse=True)
     def setUp(self, project):
         run_dbt(["seed"])
         run_dbt()
 
     @pytest.fixture(scope="class")
     def seeds(self):
-        return {"seed.csv": _SEEDS__SEED}
+        return {"seed.csv": fixtures._SEEDS__SEED}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "no_docs_model.sql": _MODELS__NO_DOCS_MODEL,
-            "table_model.sql": _MODELS__TABLE,
-            "view_model.sql": _MODELS__VIEW,
+            "no_docs_model.sql": fixtures._MODELS__NO_DOCS_MODEL,
+            "table_model.sql": fixtures._MODELS__TABLE,
+            "view_model.sql": fixtures._MODELS__VIEW,
         }
 
     @pytest.fixture(scope="class")
     def properties(self):
         return {
-            "my_fun_docs.md": _DOCS__MY_FUN_DOCS,
-            "schema.yml": _PROPERTIES__SCHEMA_YML,
+            "my_fun_docs.md": fixtures._DOCS__MY_FUN_DOCS,
+            "schema.yml": fixtures._PROPERTIES__SCHEMA_YML,
         }
 
     def _assert_common_comments(self, *comments):
         for comment in comments:
             assert '"with double quotes"' in comment
             assert """'''abc123'''""" in comment
             assert "\n" in comment
@@ -129,19 +117,19 @@
                     },
                 }
             }
         }
 
     @pytest.fixture(scope="class")
     def models(self):
-        return {"missing_column.sql": _MODELS__MISSING_COLUMN}
+        return {"missing_column.sql": fixtures._MODELS__MISSING_COLUMN}
 
     @pytest.fixture(scope="class")
     def properties(self):
-        return {"schema.yml": _PROPERITES__SCHEMA_MISSING_COL}
+        return {"schema.yml": fixtures._PROPERITES__SCHEMA_MISSING_COL}
 
     def test_missing_column(self, project):
         run_dbt(["docs", "generate"])
         with open("target/catalog.json") as fp:
             catalog_data = json.load(fp)
         assert "nodes" in catalog_data
 
@@ -152,19 +140,19 @@
 
 class BasePersistDocsCommentOnQuotedColumn:
     """Covers edge case where column with comment must be quoted.
     We set this using the `quote:` tag in the property file."""
 
     @pytest.fixture(scope="class")
     def models(self):
-        return {"quote_model.sql": _MODELS__MODEL_USING_QUOTE_UTIL}
+        return {"quote_model.sql": fixtures._MODELS__MODEL_USING_QUOTE_UTIL}
 
     @pytest.fixture(scope="class")
     def properties(self):
-        return {"properties.yml": _PROPERTIES__QUOTE_MODEL}
+        return {"properties.yml": fixtures._PROPERTIES__QUOTE_MODEL}
 
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "models": {
                 "test": {
                     "materialized": "table",
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/python_model/test_python_model.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/python_model/test_python_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-import pytest
 import os
+
+import pytest
 import yaml
+
 from dbt.tests.util import run_dbt
 
+
 basic_sql = """
 select 1 as id union all
 select 1 as id union all
 select 1 as id union all
 select 1 as id union all
 select 1 as id union all
 select 1 as id
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/python_model/test_spark.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/python_model/test_spark.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import pytest
+
 from dbt.tests.util import run_dbt
 
+
 PANDAS_MODEL = """
 import pandas as pd
 
 def model(dbt, session):
     dbt.config(
         materialized="table",
     )
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/query_comment/fixtures.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/query_comment/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/query_comment/test_query_comment.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/query_comment/test_query_comment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-import pytest
 import json
-from dbt.exceptions import DbtRuntimeError
-from dbt.version import __version__ as dbt_version
+from importlib import import_module
+
+import pytest
+from dbt_common.exceptions import DbtRuntimeError
+
+from dbt.tests.adapter.query_comment import fixtures
 from dbt.tests.util import run_dbt_and_capture
-from dbt.tests.adapter.query_comment.fixtures import MACROS__MACRO_SQL, MODELS__X_SQL
 
 
 class BaseDefaultQueryComments:
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "x.sql": MODELS__X_SQL,
+            "x.sql": fixtures.MODELS__X_SQL,
         }
 
     @pytest.fixture(scope="class")
     def macros(self):
         return {
-            "macro.sql": MACROS__MACRO_SQL,
+            "macro.sql": fixtures.MACROS__MACRO_SQL,
         }
 
     def run_get_json(self, expect_pass=True):
         res, raw_logs = run_dbt_and_capture(
             ["--debug", "--log-format=json", "run"], expect_pass=expect_pass
         )
 
@@ -31,39 +33,43 @@
 
 # Base setup to be inherited #
 class BaseQueryComments(BaseDefaultQueryComments):
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {"query-comment": "dbt\nrules!\n"}
 
-    def test_matches_comment(self, project) -> bool:
+    def test_matches_comment(self, project):
         logs = self.run_get_json()
         assert r"/* dbt\nrules! */\n" in logs
 
 
 class BaseMacroQueryComments(BaseDefaultQueryComments):
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {"query-comment": "{{ query_header_no_args() }}"}
 
-    def test_matches_comment(self, project) -> bool:
+    def test_matches_comment(self, project):
         logs = self.run_get_json()
         assert r"/* dbt macros\nare pretty cool */\n" in logs
 
 
 class BaseMacroArgsQueryComments(BaseDefaultQueryComments):
     @pytest.fixture(scope="class")
+    def get_package_version(self, project):
+        return import_module("." + project.adapter_type, "dbt.adapters").__version__.version
+
+    @pytest.fixture(scope="class")
     def project_config_update(self):
         return {"query-comment": "{{ return(ordered_to_json(query_header_args(target.name))) }}"}
 
-    def test_matches_comment(self, project) -> bool:
+    def test_matches_comment(self, project, get_package_version):
         logs = self.run_get_json()
         expected_dct = {
             "app": "dbt++",
-            "dbt_version": dbt_version,
+            "dbt_version": get_package_version,
             "macro_version": "0.1.0",
             "message": f"blah: {project.adapter.config.target_name}",
         }
         expected = r"/* {} */\n".format(json.dumps(expected_dct, sort_keys=True)).replace(
             '"', r"\""
         )
         assert expected in logs
@@ -80,25 +86,25 @@
 
 
 class BaseNullQueryComments(BaseDefaultQueryComments):
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {"query-comment": None}
 
-    def test_matches_comment(self, project) -> bool:
+    def test_matches_comment(self, project):
         logs = self.run_get_json()
         assert "/*" not in logs or "*/" not in logs
 
 
 class BaseEmptyQueryComments(BaseDefaultQueryComments):
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {"query-comment": ""}
 
-    def test_matches_comment(self, project) -> bool:
+    def test_matches_comment(self, project):
         logs = self.run_get_json()
         assert "/*" not in logs or "*/" not in logs
 
 
 # Tests #
 class TestQueryComments(BaseQueryComments):
     pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/relations/test_changing_relation_type.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/relations/test_changing_relation_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import List, Optional
+
 import pytest
 
 from dbt.tests.util import run_dbt
 
 
 _DEFAULT_CHANGE_RELATION_TYPE_MODEL = """
 {{ config(materialized=var('materialized')) }}
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_copy/fixtures.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_copy/fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 _PROPERTIES__SCHEMA_YML = """
 version: 2
 models:
 - name: disabled
   columns:
   - name: id
-    tests:
+    data_tests:
     - unique
 """
 
 
 _SEEDS__SEED_INITIAL = """
 id,first_name,last_name,email,gender,ip_address
 1,Jack,Hunter,jhunter0@pbs.org,Male,59.80.20.168
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_copy/test_copy_uppercase.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_copy/test_copy_uppercase.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,14 @@
 import pytest
-from dbt.tests.util import run_dbt, check_relations_equal
 
-from dbt.tests.adapter.simple_copy.fixtures import (
-    _PROPERTIES__SCHEMA_YML,
-    _SEEDS__SEED_INITIAL,
-    _MODELS__ADVANCED_INCREMENTAL,
-    _MODELS__COMPOUND_SORT,
-    _MODELS__DISABLED,
-    _MODELS__EMPTY,
-    _MODELS_GET_AND_REF_UPPERCASE,
-    _MODELS__INCREMENTAL,
-    _MODELS__INTERLEAVED_SORT,
-    _MODELS__MATERIALIZED,
-    _MODELS__VIEW_MODEL,
-)
+from dbt.tests.adapter.simple_copy import fixtures
+from dbt.tests.util import run_dbt, check_relations_equal
 
 
-class TestSimpleCopyUppercase:
+class BaseSimpleCopyUppercase:
     @pytest.fixture(scope="class")
     def dbt_profile_target(self):
         return {
             "type": "postgres",
             "threads": 4,
             "host": "localhost",
             "port": 5432,
@@ -28,41 +16,44 @@
             "pass": "password",
             "dbname": "dbtMixedCase",
         }
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "ADVANCED_INCREMENTAL.sql": _MODELS__ADVANCED_INCREMENTAL,
-            "COMPOUND_SORT.sql": _MODELS__COMPOUND_SORT,
-            "DISABLED.sql": _MODELS__DISABLED,
-            "EMPTY.sql": _MODELS__EMPTY,
-            "GET_AND_REF.sql": _MODELS_GET_AND_REF_UPPERCASE,
-            "INCREMENTAL.sql": _MODELS__INCREMENTAL,
-            "INTERLEAVED_SORT.sql": _MODELS__INTERLEAVED_SORT,
-            "MATERIALIZED.sql": _MODELS__MATERIALIZED,
-            "VIEW_MODEL.sql": _MODELS__VIEW_MODEL,
+            "ADVANCED_INCREMENTAL.sql": fixtures._MODELS__ADVANCED_INCREMENTAL,
+            "COMPOUND_SORT.sql": fixtures._MODELS__COMPOUND_SORT,
+            "DISABLED.sql": fixtures._MODELS__DISABLED,
+            "EMPTY.sql": fixtures._MODELS__EMPTY,
+            "GET_AND_REF.sql": fixtures._MODELS_GET_AND_REF_UPPERCASE,
+            "INCREMENTAL.sql": fixtures._MODELS__INCREMENTAL,
+            "INTERLEAVED_SORT.sql": fixtures._MODELS__INTERLEAVED_SORT,
+            "MATERIALIZED.sql": fixtures._MODELS__MATERIALIZED,
+            "VIEW_MODEL.sql": fixtures._MODELS__VIEW_MODEL,
         }
 
     @pytest.fixture(scope="class")
     def properties(self):
         return {
-            "schema.yml": _PROPERTIES__SCHEMA_YML,
+            "schema.yml": fixtures._PROPERTIES__SCHEMA_YML,
         }
 
     @pytest.fixture(scope="class")
     def seeds(self):
-        return {"seed.csv": _SEEDS__SEED_INITIAL}
+        return {"seed.csv": fixtures._SEEDS__SEED_INITIAL}
 
     def test_simple_copy_uppercase(self, project):
-
         # Load the seed file and check that it worked
         results = run_dbt(["seed"])
         assert len(results) == 1
 
         # Run the project and ensure that all the models loaded
         results = run_dbt()
         assert len(results) == 7
 
         check_relations_equal(
             project.adapter, ["seed", "VIEW_MODEL", "INCREMENTAL", "MATERIALIZED", "GET_AND_REF"]
         )
+
+
+class TestSimpleCopyUppercase(BaseSimpleCopyUppercase):
+    pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_seed/fixtures.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_seed/fixtures.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,50 +50,50 @@
 
 properties__schema_yml = """
 version: 2
 seeds:
 - name: seed_enabled
   columns:
   - name: birthday
-    tests:
+    data_tests:
     - column_type:
         type: date
   - name: seed_id
-    tests:
+    data_tests:
     - column_type:
         type: text
 
 - name: seed_tricky
   columns:
   - name: seed_id
-    tests:
+    data_tests:
     - column_type:
         type: integer
   - name: seed_id_str
-    tests:
+    data_tests:
     - column_type:
         type: text
   - name: a_bool
-    tests:
+    data_tests:
     - column_type:
         type: boolean
   - name: looks_like_a_bool
-    tests:
+    data_tests:
     - column_type:
         type: text
   - name: a_date
-    tests:
+    data_tests:
     - column_type:
         type: timestamp without time zone
   - name: looks_like_a_date
-    tests:
+    data_tests:
     - column_type:
         type: text
   - name: relative
-    tests:
+    data_tests:
     - column_type:
         type: text
   - name: weekday
-    tests:
+    data_tests:
     - column_type:
         type: text
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_seed/seeds.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_seed/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_seed/test_seed.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_seed/test_seed.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,23 @@
-import csv
-import pytest
-
 from codecs import BOM_UTF8
+import csv
 from pathlib import Path
 
+import pytest
+
+from dbt.tests.adapter.simple_seed import fixtures, seeds
 from dbt.tests.util import (
+    check_relations_equal,
+    check_table_does_exist,
+    check_table_does_not_exist,
     copy_file,
     mkdir,
+    read_file,
     rm_dir,
     run_dbt,
-    read_file,
-    check_relations_equal,
-    check_table_does_exist,
-    check_table_does_not_exist,
-)
-
-from dbt.tests.adapter.simple_seed.fixtures import (
-    models__downstream_from_seed_actual,
-    models__from_basic_seed,
-    models__downstream_from_seed_pipe_separated,
-)
-
-from dbt.tests.adapter.simple_seed.seeds import (
-    seed__actual_csv,
-    seeds__expected_sql,
-    seeds__enabled_in_config_csv,
-    seeds__disabled_in_config_csv,
-    seeds__tricky_csv,
-    seeds__wont_parse_csv,
-    seed__unicode_csv,
-    seed__with_dots_csv,
-    seeds__pipe_separated_csv,
 )
 
 
 class SeedConfigBase(object):
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
@@ -44,24 +27,24 @@
         }
 
 
 class SeedTestBase(SeedConfigBase):
     @pytest.fixture(scope="class", autouse=True)
     def setUp(self, project):
         """Create table for ensuring seeds and models used in tests build correctly"""
-        project.run_sql(seeds__expected_sql)
+        project.run_sql(seeds.seeds__expected_sql)
 
     @pytest.fixture(scope="class")
     def seeds(self, test_data_dir):
-        return {"seed_actual.csv": seed__actual_csv}
+        return {"seed_actual.csv": seeds.seed__actual_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "models__downstream_from_seed_actual.sql": models__downstream_from_seed_actual,
+            "models__downstream_from_seed_actual.sql": fixtures.models__downstream_from_seed_actual,
         }
 
     def _build_relations_for_test(self, project):
         """The testing environment needs seeds and models to interact with"""
         seed_result = run_dbt(["seed"])
         assert len(seed_result) == 1
         check_relations_equal(project.adapter, ["seed_expected", "seed_actual"])
@@ -77,43 +60,51 @@
         check_relations_equal(project.adapter, ["seed_actual", "seed_expected"])
         if exists:
             check_table_does_exist(project.adapter, "models__downstream_from_seed_actual")
         else:
             check_table_does_not_exist(project.adapter, "models__downstream_from_seed_actual")
 
 
-class TestBasicSeedTests(SeedTestBase):
+class BaseBasicSeedTests(SeedTestBase):
     def test_simple_seed(self, project):
         """Build models and observe that run truncates a seed and re-inserts rows"""
         self._build_relations_for_test(project)
         self._check_relation_end_state(run_result=run_dbt(["seed"]), project=project, exists=True)
 
     def test_simple_seed_full_refresh_flag(self, project):
         """Drop the seed_actual table and re-create. Verifies correct behavior by the absence of the
         model which depends on seed_actual."""
         self._build_relations_for_test(project)
         self._check_relation_end_state(
             run_result=run_dbt(["seed", "--full-refresh"]), project=project, exists=False
         )
 
 
-class TestSeedConfigFullRefreshOn(SeedTestBase):
+class TestBasicSeedTests(BaseBasicSeedTests):
+    pass
+
+
+class BaseSeedConfigFullRefreshOn(SeedTestBase):
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "seeds": {"quote_columns": False, "full_refresh": True},
         }
 
     def test_simple_seed_full_refresh_config(self, project):
         """config option should drop current model and cascade drop to downstream models"""
         self._build_relations_for_test(project)
         self._check_relation_end_state(run_result=run_dbt(["seed"]), project=project, exists=False)
 
 
-class TestSeedConfigFullRefreshOff(SeedTestBase):
+class TestSeedConfigFullRefreshOn(BaseSeedConfigFullRefreshOn):
+    pass
+
+
+class BaseSeedConfigFullRefreshOff(SeedTestBase):
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "seeds": {"quote_columns": False, "full_refresh": False},
         }
 
     def test_simple_seed_full_refresh_config(self, project):
@@ -121,19 +112,23 @@
         self._build_relations_for_test(project)
         self._check_relation_end_state(run_result=run_dbt(["seed"]), project=project, exists=True)
         self._check_relation_end_state(
             run_result=run_dbt(["seed", "--full-refresh"]), project=project, exists=True
         )
 
 
-class TestSeedCustomSchema(SeedTestBase):
+class TestSeedConfigFullRefreshOff(BaseSeedConfigFullRefreshOff):
+    pass
+
+
+class BaseSeedCustomSchema(SeedTestBase):
     @pytest.fixture(scope="class", autouse=True)
     def setUp(self, project):
         """Create table for ensuring seeds and models used in tests build correctly"""
-        project.run_sql(seeds__expected_sql)
+        project.run_sql(seeds.seeds__expected_sql)
 
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "seeds": {
                 "schema": "custom_schema",
                 "quote_columns": False,
@@ -161,34 +156,38 @@
         # this should drop the seed table, then re-create
         results = run_dbt(["seed", "--full-refresh"])
         assert len(results) == 1
         custom_schema = f"{project.test_schema}_custom_schema"
         check_relations_equal(project.adapter, [f"{custom_schema}.seed_actual", "seed_expected"])
 
 
+class TestSeedCustomSchema(BaseSeedCustomSchema):
+    pass
+
+
 class SeedUniqueDelimiterTestBase(SeedConfigBase):
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "seeds": {"quote_columns": False, "delimiter": "|"},
         }
 
     @pytest.fixture(scope="class", autouse=True)
     def setUp(self, project):
         """Create table for ensuring seeds and models used in tests build correctly"""
-        project.run_sql(seeds__expected_sql)
+        project.run_sql(seeds.seeds__expected_sql)
 
     @pytest.fixture(scope="class")
     def seeds(self, test_data_dir):
-        return {"seed_pipe_separated.csv": seeds__pipe_separated_csv}
+        return {"seed_pipe_separated.csv": seeds.seeds__pipe_separated_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "models__downstream_from_seed_pipe_separated.sql": models__downstream_from_seed_pipe_separated,
+            "models__downstream_from_seed_pipe_separated.sql": fixtures.models__downstream_from_seed_pipe_separated,
         }
 
     def _build_relations_for_test(self, project):
         """The testing environment needs seeds and models to interact with"""
         seed_result = run_dbt(["seed"])
         assert len(seed_result) == 1
         check_relations_equal(project.adapter, ["seed_expected", "seed_pipe_separated"])
@@ -206,54 +205,66 @@
             check_table_does_exist(project.adapter, "models__downstream_from_seed_pipe_separated")
         else:
             check_table_does_not_exist(
                 project.adapter, "models__downstream_from_seed_pipe_separated"
             )
 
 
-class TestSeedWithUniqueDelimiter(SeedUniqueDelimiterTestBase):
+class BaseSeedWithUniqueDelimiter(SeedUniqueDelimiterTestBase):
     def test_seed_with_unique_delimiter(self, project):
         """Testing correct run of seeds with a unique delimiter (pipe in this case)"""
         self._build_relations_for_test(project)
         self._check_relation_end_state(run_result=run_dbt(["seed"]), project=project, exists=True)
 
 
-class TestSeedWithWrongDelimiter(SeedUniqueDelimiterTestBase):
+class TestSeedWithUniqueDelimiter(BaseSeedWithUniqueDelimiter):
+    pass
+
+
+class BaseSeedWithWrongDelimiter(SeedUniqueDelimiterTestBase):
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "seeds": {"quote_columns": False, "delimiter": ";"},
         }
 
     def test_seed_with_wrong_delimiter(self, project):
         """Testing failure of running dbt seed with a wrongly configured delimiter"""
         seed_result = run_dbt(["seed"], expect_pass=False)
         assert "syntax error" in seed_result.results[0].message.lower()
 
 
-class TestSeedWithEmptyDelimiter(SeedUniqueDelimiterTestBase):
+class TestSeedWithWrongDelimiter(BaseSeedWithWrongDelimiter):
+    pass
+
+
+class BaseSeedWithEmptyDelimiter(SeedUniqueDelimiterTestBase):
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "seeds": {"quote_columns": False, "delimiter": ""},
         }
 
     def test_seed_with_empty_delimiter(self, project):
         """Testing failure of running dbt seed with an empty configured delimiter value"""
         seed_result = run_dbt(["seed"], expect_pass=False)
         assert "compilation error" in seed_result.results[0].message.lower()
 
 
-class TestSimpleSeedEnabledViaConfig(object):
+class TestSeedWithEmptyDelimiter(BaseSeedWithEmptyDelimiter):
+    pass
+
+
+class BaseSimpleSeedEnabledViaConfig:
     @pytest.fixture(scope="session")
     def seeds(self):
         return {
-            "seed_enabled.csv": seeds__enabled_in_config_csv,
-            "seed_disabled.csv": seeds__disabled_in_config_csv,
-            "seed_tricky.csv": seeds__tricky_csv,
+            "seed_enabled.csv": seeds.seeds__enabled_in_config_csv,
+            "seed_disabled.csv": seeds.seeds__disabled_in_config_csv,
+            "seed_tricky.csv": seeds.seeds__tricky_csv,
         }
 
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "seeds": {
                 "test": {"seed_enabled": {"enabled": True}, "seed_disabled": {"enabled": False}},
@@ -284,43 +295,51 @@
         results = run_dbt(["seed", "--exclude", "seed_enabled"])
         assert len(results) == 1
         check_table_does_not_exist(project.adapter, "seed_enabled")
         check_table_does_not_exist(project.adapter, "seed_disabled")
         check_table_does_exist(project.adapter, "seed_tricky")
 
 
-class TestSeedParsing(SeedConfigBase):
+class TestSimpleSeedEnabledViaConfig(BaseSimpleSeedEnabledViaConfig):
+    pass
+
+
+class BaseSeedParsing(SeedConfigBase):
     @pytest.fixture(scope="class", autouse=True)
     def setUp(self, project):
         """Create table for ensuring seeds and models used in tests build correctly"""
-        project.run_sql(seeds__expected_sql)
+        project.run_sql(seeds.seeds__expected_sql)
 
     @pytest.fixture(scope="class")
     def seeds(self):
-        return {"seed.csv": seeds__wont_parse_csv}
+        return {"seed.csv": seeds.seeds__wont_parse_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
-        return {"model.sql": models__from_basic_seed}
+        return {"model.sql": fixtures.models__from_basic_seed}
 
     def test_dbt_run_skips_seeds(self, project):
         # run does not try to parse the seed files
         assert len(run_dbt()) == 1
 
         # make sure 'dbt seed' fails, otherwise our test is invalid!
         run_dbt(["seed"], expect_pass=False)
 
 
-class TestSimpleSeedWithBOM(SeedConfigBase):
+class TestSeedParsing(BaseSeedParsing):
+    pass
+
+
+class BaseSimpleSeedWithBOM(SeedConfigBase):
     # Reference: BOM = byte order mark; see https://www.ibm.com/docs/en/netezza?topic=formats-byte-order-mark
     # Tests for hidden unicode character in csv
     @pytest.fixture(scope="class", autouse=True)
     def setUp(self, project):
         """Create table for ensuring seeds and models used in tests build correctly"""
-        project.run_sql(seeds__expected_sql)
+        project.run_sql(seeds.seeds__expected_sql)
         copy_file(
             project.test_dir,
             "seed_bom.csv",
             project.project_root / Path("seeds") / "seed_bom.csv",
             "",
         )
 
@@ -332,15 +351,19 @@
         with open(
             project.project_root / Path("seeds") / Path("seed_bom.csv"), encoding="utf-8"
         ) as fp:
             assert fp.read(1) == BOM_UTF8.decode("utf-8")
         check_relations_equal(project.adapter, ["seed_expected", "seed_bom"])
 
 
-class TestSeedSpecificFormats(SeedConfigBase):
+class TestSimpleSeedWithBOM(BaseSimpleSeedWithBOM):
+    pass
+
+
+class BaseSeedSpecificFormats(SeedConfigBase):
     """Expect all edge cases to build"""
 
     @staticmethod
     def _make_big_seed(test_data_dir):
         mkdir(test_data_dir)
         big_seed_path = test_data_dir / Path("tmp.csv")
         with open(big_seed_path, "w") as f:
@@ -353,24 +376,28 @@
     @pytest.fixture(scope="class")
     def seeds(self, test_data_dir):
         big_seed_path = self._make_big_seed(test_data_dir)
         big_seed = read_file(big_seed_path)
 
         yield {
             "big_seed.csv": big_seed,
-            "seed.with.dots.csv": seed__with_dots_csv,
-            "seed_unicode.csv": seed__unicode_csv,
+            "seed.with.dots.csv": seeds.seed__with_dots_csv,
+            "seed_unicode.csv": seeds.seed__unicode_csv,
         }
         rm_dir(test_data_dir)
 
     def test_simple_seed(self, project):
         results = run_dbt(["seed"])
         assert len(results) == 3
 
 
+class TestSeedSpecificFormats(BaseSeedSpecificFormats):
+    pass
+
+
 class BaseTestEmptySeed:
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "seeds": {
                 "quote_columns": False,
             },
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_seed/test_seed_type_override.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_seed/test_seed_type_override.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,31 @@
 import pytest
 
+from dbt.tests.adapter.simple_seed import fixtures, seeds
 from dbt.tests.util import run_dbt
 
-from dbt.tests.adapter.simple_seed.fixtures import (
-    macros__schema_test,
-    properties__schema_yml,
-)
-
-from dbt.tests.adapter.simple_seed.seeds import (
-    seeds__enabled_in_config_csv,
-    seeds__disabled_in_config_csv,
-    seeds__tricky_csv,
-)
-
 
 class BaseSimpleSeedColumnOverride:
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "schema.yml": properties__schema_yml,
+            "schema.yml": fixtures.properties__schema_yml,
         }
 
     @pytest.fixture(scope="class")
     def seeds(self):
         return {
-            "seed_enabled.csv": seeds__enabled_in_config_csv,
-            "seed_disabled.csv": seeds__disabled_in_config_csv,
-            "seed_tricky.csv": seeds__tricky_csv,
+            "seed_enabled.csv": seeds.seeds__enabled_in_config_csv,
+            "seed_disabled.csv": seeds.seeds__disabled_in_config_csv,
+            "seed_tricky.csv": seeds.seeds__tricky_csv,
         }
 
     @pytest.fixture(scope="class")
     def macros(self):
-        return {"schema_test.sql": macros__schema_test}
+        return {"schema_test.sql": fixtures.macros__schema_test}
 
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "seeds": {
                 "test": {
                     "enabled": False,
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_snapshot/common.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_snapshot/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import Dict, List
 
-from dbt.tests.util import relation_from_name
 from dbt.tests.fixtures.project import TestProjInfo
+from dbt.tests.util import relation_from_name
 
 
 def get_records(
-    project: TestProjInfo, table: str, select: str = None, where: str = None
+    project: TestProjInfo, table: str, select: str = None, where: str = None  # type: ignore
 ) -> List[tuple]:
     """
     Gets records from a single table in a dbt project
 
     Args:
-        project: the dbt project that contains the table
+        project: the dbt project that contains the table to get records from
         table: the name of the table without a schema
         select: the selection clause; defaults to all columns (*)
         where: the where clause to apply, if any; defaults to all records
 
     Returns:
         A list of records with each record as a tuple
     """
@@ -26,15 +26,17 @@
         select {select_clause}
         from {table_name}
         where {where_clause}
     """
     return [tuple(record) for record in project.run_sql(sql, fetch="all")]
 
 
-def update_records(project: TestProjInfo, table: str, updates: Dict[str, str], where: str = None):
+def update_records(
+    project: TestProjInfo, table: str, updates: Dict[str, str], where: str = None  # type: ignore
+):
     """
     Applies updates to a table in a dbt project
 
     Args:
         project: the dbt project that contains the table
         table: the name of the table without a schema
         updates: the updates to be applied in the form {'field_name': 'expression to be applied'}
@@ -50,15 +52,15 @@
         set {set_clause}
         where {where_clause}
     """
     project.run_sql(sql)
 
 
 def insert_records(
-    project: TestProjInfo, to_table: str, from_table: str, select: str, where: str = None
+    project: TestProjInfo, to_table: str, from_table: str, select: str, where: str = None  # type: ignore
 ):
     """
     Inserts records from one table into another table in a dbt project
 
     Args:
         project: the dbt project that contains the table
         to_table: the name of the table, without a schema, in which the records will be inserted
@@ -75,34 +77,34 @@
         select {select_clause}
         from {from_table_name}
         where {where_clause}
     """
     project.run_sql(sql)
 
 
-def delete_records(project: TestProjInfo, table: str, where: str = None):
+def delete_records(project: TestProjInfo, table: str, where: str = None):  # type: ignore
     """
     Deletes records from a table in a dbt project
 
     Args:
-        project: the dbt project that contains the table
+        project: the dbt project that contains the table and where to
         table: the name of the table without a schema
         where: the where clause to apply, if any; defaults to all records
     """
     table_name = relation_from_name(project.adapter, table)
     where_clause = where or "1 = 1"
     sql = f"""
         delete from {table_name}
         where {where_clause}
     """
     project.run_sql(sql)
 
 
 def clone_table(
-    project: TestProjInfo, to_table: str, from_table: str, select: str, where: str = None
+    project: TestProjInfo, to_table: str, from_table: str, select: str, where: str = None  # type: ignore
 ):
     """
     Creates a new table based on another table in a dbt project
 
     Args:
         project: the dbt project that contains the table
         to_table: the name of the table, without a schema, to be created
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_snapshot/seeds.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_snapshot/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_snapshot/snapshots.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_snapshot/snapshots.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/simple_snapshot/test_snapshot.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/simple_snapshot/test_snapshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+from typing import Dict, Iterable, List
+
 import pytest
 
-from typing import Dict, List, Iterable
+from dbt.tests.adapter.simple_snapshot import common, seeds, snapshots
 from dbt.tests.util import run_dbt
 
-from dbt.tests.adapter.simple_snapshot import common
-from dbt.tests.adapter.simple_snapshot import seeds, snapshots
 
 MODEL_FACT_SQL = """
 {{ config(materialized="table") }}
 select * from {{ ref('seed') }}
 where id between 1 and 20
 """
 
@@ -50,30 +50,32 @@
         self.project = project
         self.create_fact_from_seed("id between 1 and 20")
         run_dbt(["snapshot"])
         yield
         self.delete_snapshot_records()
         self.delete_fact_records()
 
-    def update_fact_records(self, updates: Dict[str, str], where: str = None):
+    def update_fact_records(self, updates: Dict[str, str], where: str = None):  # type: ignore
         common.update_records(self.project, "fact", updates, where)
 
-    def insert_fact_records(self, where: str = None):
+    def insert_fact_records(self, where: str = None):  # type: ignore
         common.insert_records(self.project, "fact", "seed", "*", where)
 
-    def delete_fact_records(self, where: str = None):
+    def delete_fact_records(self, where: str = None):  # type: ignore
         common.delete_records(self.project, "fact", where)
 
-    def add_fact_column(self, column: str = None, definition: str = None):
+    def add_fact_column(self, column: str = None, definition: str = None):  # type: ignore
         common.add_column(self.project, "fact", column, definition)
 
-    def create_fact_from_seed(self, where: str = None):
+    def create_fact_from_seed(self, where: str = None):  # type: ignore
         common.clone_table(self.project, "fact", "seed", "*", where)
 
-    def get_snapshot_records(self, select: str = None, where: str = None) -> List[tuple]:
+    def get_snapshot_records(
+        self, select: str = None, where: str = None  # type: ignore
+    ) -> List[tuple]:
         return common.get_records(self.project, "snapshot", select, where)
 
     def delete_snapshot_records(self):
         common.delete_records(self.project, "snapshot")
 
     def _assert_results(
         self,
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/store_test_failures_tests/_files.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/store_test_failures_tests/_files.py`

 * *Files 7% similar despite different names*

```diff
@@ -128,23 +128,23 @@
 SCHEMA_YML = """
 version: 2
 
 models:
   - name: chipmunks
     columns:
       - name: name
-        tests:
+        data_tests:
           - not_null:
               store_failures_as: view
           - accepted_values:
               store_failures: false
               store_failures_as: table
               values:
                 - alvin
                 - simon
                 - theodore
       - name: shirt
-        tests:
+        data_tests:
           - not_null:
               store_failures: true
               store_failures_as: view
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/store_test_failures_tests/basic.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/store_test_failures_tests/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from collections import namedtuple
 from typing import Set
 
+# TODO: repoint to dbt-artifacts when it's available
+from dbt.artifacts.schemas.results import TestStatus
 import pytest
 
-from dbt.contracts.results import TestStatus
-from dbt.tests.util import run_dbt, check_relation_types
-
 from dbt.tests.adapter.store_test_failures_tests import _files
+from dbt.tests.util import run_dbt, check_relation_types
 
 
 TestResult = namedtuple("TestResult", ["name", "status", "type"])
 
 
 class StoreTestFailuresAsBase:
     seed_table: str = "chipmunks_stage"
@@ -163,15 +163,15 @@
             "results_table.sql": _files.TEST__TABLE_UNSET,
             "results_ephemeral.sql": _files.TEST__EPHEMERAL_UNSET,
             "results_unset.sql": _files.TEST__UNSET_UNSET,
         }
 
     @pytest.fixture(scope="class")
     def project_config_update(self):
-        return {"tests": {"store_failures": False}}
+        return {"data_tests": {"store_failures": False}}
 
     def test_tests_run_successfully_and_are_stored_as_expected(self, project):
         expected_results = {
             TestResult("results_view", TestStatus.Fail, "view"),
             TestResult("results_table", TestStatus.Fail, "table"),
             TestResult("results_ephemeral", TestStatus.Fail, None),
             TestResult("results_unset", TestStatus.Fail, None),
@@ -200,15 +200,15 @@
             "results_true.sql": _files.TEST__VIEW_TRUE,
             "results_false.sql": _files.TEST__VIEW_FALSE,
             "results_unset.sql": _files.TEST__VIEW_UNSET,
         }
 
     @pytest.fixture(scope="class")
     def project_config_update(self):
-        return {"tests": {"store_failures_as": "view"}}
+        return {"data_tests": {"store_failures_as": "view"}}
 
     def test_tests_run_successfully_and_are_stored_as_expected(self, project):
         expected_results = {
             TestResult("results_true", TestStatus.Fail, "view"),
             TestResult("results_false", TestStatus.Fail, "view"),
             TestResult("results_unset", TestStatus.Fail, "view"),
         }
@@ -238,15 +238,15 @@
             "results_unset.sql": _files.TEST__UNSET_UNSET,
             "results_true.sql": _files.TEST__UNSET_TRUE,
             "results_view.sql": _files.TEST__VIEW_UNSET,
         }
 
     @pytest.fixture(scope="class")
     def project_config_update(self):
-        return {"tests": {"store_failures_as": "ephemeral", "store_failures": True}}
+        return {"data_tests": {"store_failures_as": "ephemeral", "store_failures": True}}
 
     def test_tests_run_successfully_and_are_stored_as_expected(self, project):
         expected_results = {
             TestResult("results_unset", TestStatus.Fail, None),
             TestResult("results_true", TestStatus.Fail, None),
             TestResult("results_view", TestStatus.Fail, "view"),
         }
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/store_test_failures_tests/fixtures.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/store_test_failures_tests/fixtures.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,27 +49,27 @@
 version: 2
 
 models:
 
   - name: fine_model
     columns:
       - name: id
-        tests:
+        data_tests:
           - unique
           - not_null
 
   - name: problematic_model
     columns:
       - name: id
-        tests:
+        data_tests:
           - unique:
               store_failures: true
           - not_null
       - name: first_name
-        tests:
+        data_tests:
           # test truncation of really long test name
           - accepted_values:
               values:
                 - Jack
                 - Kathryn
                 - Gerald
                 - Bonnie
@@ -79,15 +79,15 @@
                 - Craig
                 # - Gary
                 # - Rose
 
   - name: fine_model_but_with_a_no_good_very_long_name
     columns:
       - name: quite_long_column_name
-        tests:
+        data_tests:
           # test truncation of really long test name with builtin
           - unique
 """
 
 #
 # Models
 #
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,12 @@
 import pytest
 
-from dbt.tests.util import (
-    check_relations_equal,
-    run_dbt,
-)
-
-from dbt.tests.adapter.store_test_failures_tests.fixtures import (
-    seeds__people,
-    seeds__expected_accepted_values,
-    seeds__expected_failing_test,
-    seeds__expected_not_null_problematic_model_id,
-    seeds__expected_unique_problematic_model_id,
-    properties__schema_yml,
-    models__problematic_model,
-    models__fine_model,
-    models__file_model_but_with_a_no_good_very_long_name,
-    tests__failing_test,
-    tests__passing_test,
-)
+from dbt.tests.adapter.store_test_failures_tests import fixtures
+from dbt.tests.util import check_relations_equal, run_dbt
+
 
 # used to rename test audit schema to help test schema meet max char limit
 # the default is _dbt_test__audit but this runs over the postgres 63 schema name char limit
 # without which idempotency conditions will not hold (i.e. dbt can't drop the schema properly)
 TEST_AUDIT_SCHEMA_SUFFIX = "dbt_test__aud"
 
 
@@ -31,48 +16,48 @@
         self.test_audit_schema = f"{project.test_schema}_{TEST_AUDIT_SCHEMA_SUFFIX}"
         run_dbt(["seed"])
         run_dbt(["run"])
 
     @pytest.fixture(scope="class")
     def seeds(self):
         return {
-            "people.csv": seeds__people,
-            "expected_accepted_values.csv": seeds__expected_accepted_values,
-            "expected_failing_test.csv": seeds__expected_failing_test,
-            "expected_not_null_problematic_model_id.csv": seeds__expected_not_null_problematic_model_id,
-            "expected_unique_problematic_model_id.csv": seeds__expected_unique_problematic_model_id,
+            "people.csv": fixtures.seeds__people,
+            "expected_accepted_values.csv": fixtures.seeds__expected_accepted_values,
+            "expected_failing_test.csv": fixtures.seeds__expected_failing_test,
+            "expected_not_null_problematic_model_id.csv": fixtures.seeds__expected_not_null_problematic_model_id,
+            "expected_unique_problematic_model_id.csv": fixtures.seeds__expected_unique_problematic_model_id,
         }
 
     @pytest.fixture(scope="class")
     def tests(self):
         return {
-            "failing_test.sql": tests__failing_test,
-            "passing_test.sql": tests__passing_test,
+            "failing_test.sql": fixtures.tests__failing_test,
+            "passing_test.sql": fixtures.tests__passing_test,
         }
 
     @pytest.fixture(scope="class")
     def properties(self):
-        return {"schema.yml": properties__schema_yml}
+        return {"schema.yml": fixtures.properties__schema_yml}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "fine_model.sql": models__fine_model,
-            "fine_model_but_with_a_no_good_very_long_name.sql": models__file_model_but_with_a_no_good_very_long_name,
-            "problematic_model.sql": models__problematic_model,
+            "fine_model.sql": fixtures.models__fine_model,
+            "fine_model_but_with_a_no_good_very_long_name.sql": fixtures.models__file_model_but_with_a_no_good_very_long_name,
+            "problematic_model.sql": fixtures.models__problematic_model,
         }
 
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "seeds": {
                 "quote_columns": False,
                 "test": self.column_type_overrides(),
             },
-            "tests": {"+schema": TEST_AUDIT_SCHEMA_SUFFIX},
+            "data_tests": {"+schema": TEST_AUDIT_SCHEMA_SUFFIX},
         }
 
     def column_type_overrides(self):
         return {}
 
     def run_tests_store_one_failure(self, project):
         run_dbt(["test"], expect_pass=False)
@@ -129,15 +114,15 @@
                 f"{self.test_audit_schema}.accepted_values_problemat"
                 "ic_mo_c533ab4ca65c1a9dbf14f79ded49b628",
                 "expected_accepted_values",
             ],
         )
 
 
-class TestStoreTestFailures(StoreTestFailuresBase):
+class BaseStoreTestFailures(StoreTestFailuresBase):
     @pytest.fixture(scope="function")
     def clean_up(self, project):
         yield
         with project.adapter.connection_named("__test"):
             relation = project.adapter.Relation.create(
                 database=project.database, schema=self.test_audit_schema
             )
@@ -161,7 +146,11 @@
                 },
             },
         }
 
     def test__store_and_assert(self, project, clean_up):
         self.run_tests_store_one_failure(project)
         self.run_tests_store_failures_and_assert(project)
+
+
+class TestStoreTestFailures(BaseStoreTestFailures):
+    pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/base_array_utils.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/base_array_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 from dbt.tests.adapter.utils.base_utils import BaseUtils
-from dbt.tests.util import run_dbt, check_relations_equal, get_relation_columns
+from dbt.tests.util import (
+    check_relations_equal,
+    get_relation_columns,
+    run_dbt,
+)
 
 
 class BaseArrayUtils(BaseUtils):
     def assert_columns_equal(self, project, expected_cols, actual_cols):
         assert (
             expected_cols == actual_cols
         ), f"Type difference detected: {expected_cols} vs. {actual_cols}"
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/base_utils.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/base_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 from dbt.tests.util import run_dbt
 
+
 macros__equals_sql = """
 {% macro equals(expr1, expr2) -%}
 case when (({{ expr1 }} = {{ expr2 }}) or ({{ expr1 }} is null and {{ expr2 }} is null))
     then 0
     else 1
 end = 0
 {% endmacro %}
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/data_types/base_data_type_macro.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/base_data_type_macro.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-from dbt.tests.util import run_dbt, check_relations_equal, get_relation_columns
+from dbt.tests.util import (
+    check_relations_equal,
+    get_relation_columns,
+    run_dbt,
+)
 
 
 class BaseDataTypeMacro:
     # make it possible to dynamically update the macro call with a namespace
     # (e.g.) 'dateadd', 'dbt.dateadd', 'dbt_utils.dateadd'
     def macro_namespace(self):
         return ""
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/data_types/test_type_bigint.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_bigint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import pytest
+
 from dbt.tests.adapter.utils.data_types.base_data_type_macro import BaseDataTypeMacro
 
+
 models__expected_sql = """
 select 9223372036854775800 as bigint_col
 """.lstrip()
 
 models__actual_sql = """
 select cast('9223372036854775800' as {{ type_bigint() }}) as bigint_col
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/data_types/test_type_boolean.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_boolean.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import pytest
+
 from dbt.tests.adapter.utils.data_types.base_data_type_macro import BaseDataTypeMacro
 
+
 seeds__expected_csv = """boolean_col
 True
 """.lstrip()
 
 models__actual_sql = """
 select cast('True' as {{ type_boolean() }}) as boolean_col
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/data_types/test_type_float.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_float.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import pytest
+
 from dbt.tests.adapter.utils.data_types.base_data_type_macro import BaseDataTypeMacro
 
+
 seeds__expected_csv = """float_col
 1.2345
 """.lstrip()
 
 models__actual_sql = """
 select cast('1.2345' as {{ type_float() }}) as float_col
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/data_types/test_type_int.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_int.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import pytest
+
 from dbt.tests.adapter.utils.data_types.base_data_type_macro import BaseDataTypeMacro
 
+
 seeds__expected_csv = """int_col
 12345678
 """.lstrip()
 
 models__actual_sql = """
 select cast('12345678' as {{ type_int() }}) as int_col
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/data_types/test_type_numeric.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_numeric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import pytest
+
 from dbt.tests.adapter.utils.data_types.base_data_type_macro import BaseDataTypeMacro
 
+
 seeds__expected_csv = """numeric_col
 1.2345
 """.lstrip()
 
 # need to explicitly cast this to avoid it being a double/float
 seeds__expected_yml = """
 version: 2
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/data_types/test_type_string.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_string.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import pytest
+
 from dbt.tests.adapter.utils.data_types.base_data_type_macro import BaseDataTypeMacro
 
+
 seeds__expected_csv = """string_col
 "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."
 """.lstrip()
 
 models__actual_sql = """
 select cast('Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.'
 as {{ type_string() }}) as string_col
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/data_types/test_type_timestamp.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/data_types/test_type_timestamp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import pytest
+
 from dbt.tests.adapter.utils.data_types.base_data_type_macro import BaseDataTypeMacro
 
+
 seeds__expected_csv = """timestamp_col
 2021-01-01 01:01:01
 """.lstrip()
 
 # need to explicitly cast this to avoid it being a DATETIME on BigQuery
 # (but - should it actually be a DATETIME, for consistency with other dbs?)
 seeds__expected_yml = """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_any_value.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_any_value.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,12 +49,12 @@
 """
 
 
 models__test_any_value_yml = """
 version: 2
 models:
   - name: test_any_value
-    tests:
+    data_tests:
       - assert_equal:
           actual: actual
           expected: expected
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_array_concat.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_array_concat.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_bool_or.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_bool_or.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,12 +51,12 @@
 """
 
 
 models__test_bool_or_yml = """
 version: 2
 models:
   - name: test_bool_or
-    tests:
+    data_tests:
       - assert_equal:
           actual: actual
           expected: expected
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_concat.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_concat.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,12 +34,12 @@
 """
 
 
 models__test_concat_yml = """
 version: 2
 models:
   - name: test_concat
-    tests:
+    data_tests:
       - assert_equal:
           actual: actual
           expected: expected
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_date_spine.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_date_spine.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,12 +81,12 @@
 SELECT * from joined
 """
 
 models__test_date_spine_yml = """
 version: 2
 models:
   - name: test_date_spine
-    tests:
+    data_tests:
       - assert_equal:
           actual: date_day
           expected: expected
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_date_trunc.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_date_trunc.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,12 +29,12 @@
 """
 
 
 models__test_date_trunc_yml = """
 version: 2
 models:
   - name: test_date_trunc
-    tests:
+    data_tests:
       - assert_equal:
           actual: actual
           expected: expected
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_dateadd.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_dateadd.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,12 +29,12 @@
 from data
 """
 
 models__test_dateadd_yml = """
 version: 2
 models:
   - name: test_dateadd
-    tests:
+    data_tests:
       - assert_equal:
           actual: actual
           expected: expected
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_datediff.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_datediff.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,12 +54,12 @@
 """
 
 
 models__test_datediff_yml = """
 version: 2
 models:
   - name: test_datediff
-    tests:
+    data_tests:
       - assert_equal:
           actual: actual
           expected: expected
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_equals.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_equals.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_escape_single_quotes.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_escape_single_quotes.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 """
 
 
 models__test_escape_single_quotes_yml = """
 version: 2
 models:
   - name: test_escape_single_quotes
-    tests:
+    data_tests:
       - assert_equal:
           actual: actual
           expected: expected
       - assert_equal:
           actual: actual_length
           expected: expected_length
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_except.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_except.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_generate_series.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_generate_series.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,12 +34,12 @@
 SELECT * from joined
 """
 
 models__test_generate_series_yml = """
 version: 2
 models:
   - name: test_generate_series
-    tests:
+    data_tests:
       - assert_equal:
           actual: generated_number
           expected: expected
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_get_intervals_between.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_get_intervals_between.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 
 """
 
 models__test_get_intervals_between_yml = """
 version: 2
 models:
   - name: test_get_intervals_between
-    tests:
+    data_tests:
       - assert_equal:
           actual: intervals
           expected: expected
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_get_powers_of_two.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_get_powers_of_two.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,12 +28,12 @@
 select {{ get_powers_of_two(823543) }} as actual, 20 as expected
 """
 
 models__test_get_powers_of_two_yml = """
 version: 2
 models:
   - name: test_powers_of_two
-    tests:
+    data_tests:
       - assert_equal:
           actual: actual
           expected: expected
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_hash.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_hash.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,12 +33,12 @@
 """
 
 
 models__test_hash_yml = """
 version: 2
 models:
   - name: test_hash
-    tests:
+    data_tests:
       - assert_equal:
           actual: actual
           expected: expected
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_intersect.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_intersect.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_last_day.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_last_day.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,12 +28,12 @@
 """
 
 
 models__test_last_day_yml = """
 version: 2
 models:
   - name: test_last_day
-    tests:
+    data_tests:
       - assert_equal:
           actual: actual
           expected: expected
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_listagg.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_listagg.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,12 +99,12 @@
 """
 
 
 models__test_listagg_yml = """
 version: 2
 models:
   - name: test_listagg
-    tests:
+    data_tests:
       - assert_equal:
           actual: actual
           expected: expected
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_null_compare.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_position.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-MODELS__TEST_MIXED_NULL_COMPARE_SQL = """
-select
-    1 as actual,
-    null as expected
+# position
+
+seeds__data_position_csv = """substring_text,string_text,result
+def,abcdef,4
+land,earth,0
+town,fishtown,5
+ember,december,4
 """
 
 
-MODELS__TEST_MIXED_NULL_COMPARE_YML = """
-version: 2
-models:
-  - name: test_mixed_null_compare
-    tests:
-      - assert_equal:
-          actual: actual
-          expected: expected
-"""
+models__test_position_sql = """
+with data as (
+
+    select * from {{ ref('data_position') }}
 
+)
 
-MODELS__TEST_NULL_COMPARE_SQL = """
 select
-    null as actual,
-    null as expected
+
+    {{ position('substring_text', 'string_text') }} as actual,
+    result as expected
+
+from data
 """
 
 
-MODELS__TEST_NULL_COMPARE_YML = """
+models__test_position_yml = """
 version: 2
 models:
-  - name: test_null_compare
-    tests:
+  - name: test_position
+    data_tests:
       - assert_equal:
           actual: actual
           expected: expected
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_position.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_right.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# position
+# right
 
-seeds__data_position_csv = """substring_text,string_text,result
-def,abcdef,4
-land,earth,0
-town,fishtown,5
-ember,december,4
+seeds__data_right_csv = """string_text,length_expression,output
+abcdef,3,def
+fishtown,4,town
+december,5,ember
+december,0,
 """
 
 
-models__test_position_sql = """
+models__test_right_sql = """
 with data as (
 
-    select * from {{ ref('data_position') }}
+    select * from {{ ref('data_right') }}
 
 )
 
 select
 
-    {{ position('substring_text', 'string_text') }} as actual,
-    result as expected
+    {{ right('string_text', 'length_expression') }} as actual,
+    coalesce(output, '') as expected
 
 from data
 """
 
 
-models__test_position_yml = """
+models__test_right_yml = """
 version: 2
 models:
-  - name: test_position
-    tests:
+  - name: test_right
+    data_tests:
       - assert_equal:
           actual: actual
           expected: expected
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_replace.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_replace.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,12 +28,12 @@
 """
 
 
 models__test_replace_yml = """
 version: 2
 models:
   - name: test_replace
-    tests:
+    data_tests:
       - assert_equal:
           actual: actual
           expected: expected
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_split_part.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_split_part.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,12 +46,12 @@
 """
 
 
 models__test_split_part_yml = """
 version: 2
 models:
   - name: test_split_part
-    tests:
+    data_tests:
       - assert_equal:
           actual: actual
           expected: expected
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/fixture_string_literal.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/fixture_string_literal.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 """
 
 
 models__test_string_literal_yml = """
 version: 2
 models:
   - name: test_string_literal
-    tests:
+    data_tests:
       - assert_equal:
           actual: actual
           expected: expected
 """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_any_value.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_any_value.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 import pytest
-from dbt.tests.adapter.utils.base_utils import BaseUtils
-from dbt.tests.adapter.utils.fixture_any_value import (
-    seeds__data_any_value_csv,
-    seeds__data_any_value_expected_csv,
-    models__test_any_value_sql,
-    models__test_any_value_yml,
-)
 
+from dbt.tests.adapter.utils import base_utils, fixture_any_value
 
-class BaseAnyValue(BaseUtils):
+
+class BaseAnyValue(base_utils.BaseUtils):
     @pytest.fixture(scope="class")
     def seeds(self):
         return {
-            "data_any_value.csv": seeds__data_any_value_csv,
-            "data_any_value_expected.csv": seeds__data_any_value_expected_csv,
+            "data_any_value.csv": fixture_any_value.seeds__data_any_value_csv,
+            "data_any_value_expected.csv": fixture_any_value.seeds__data_any_value_expected_csv,
         }
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "test_any_value.yml": models__test_any_value_yml,
+            "test_any_value.yml": fixture_any_value.models__test_any_value_yml,
             "test_any_value.sql": self.interpolate_macro_namespace(
-                models__test_any_value_sql, "any_value"
+                fixture_any_value.models__test_any_value_sql, "any_value"
             ),
         }
 
 
 class TestAnyValue(BaseAnyValue):
     pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_bool_or.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_bool_or.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 import pytest
-from dbt.tests.adapter.utils.base_utils import BaseUtils
-from dbt.tests.adapter.utils.fixture_bool_or import (
-    seeds__data_bool_or_csv,
-    seeds__data_bool_or_expected_csv,
-    models__test_bool_or_sql,
-    models__test_bool_or_yml,
-)
 
+from dbt.tests.adapter.utils import base_utils, fixture_bool_or
 
-class BaseBoolOr(BaseUtils):
+
+class BaseBoolOr(base_utils.BaseUtils):
     @pytest.fixture(scope="class")
     def seeds(self):
         return {
-            "data_bool_or.csv": seeds__data_bool_or_csv,
-            "data_bool_or_expected.csv": seeds__data_bool_or_expected_csv,
+            "data_bool_or.csv": fixture_bool_or.seeds__data_bool_or_csv,
+            "data_bool_or_expected.csv": fixture_bool_or.seeds__data_bool_or_expected_csv,
         }
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "test_bool_or.yml": models__test_bool_or_yml,
+            "test_bool_or.yml": fixture_bool_or.models__test_bool_or_yml,
             "test_bool_or.sql": self.interpolate_macro_namespace(
-                models__test_bool_or_sql, "bool_or"
+                fixture_bool_or.models__test_bool_or_sql, "bool_or"
             ),
         }
 
 
 class TestBoolOr(BaseBoolOr):
     pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_cast_bool_to_text.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_cast_bool_to_text.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import pytest
-from dbt.tests.adapter.utils.base_utils import BaseUtils
-from dbt.tests.adapter.utils.fixture_cast_bool_to_text import (
-    models__test_cast_bool_to_text_sql,
-    models__test_cast_bool_to_text_yml,
-)
 
+from dbt.tests.adapter.utils import base_utils, fixture_cast_bool_to_text
 
-class BaseCastBoolToText(BaseUtils):
+
+class BaseCastBoolToText(base_utils.BaseUtils):
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "test_cast_bool_to_text.yml": models__test_cast_bool_to_text_yml,
+            "test_cast_bool_to_text.yml": fixture_cast_bool_to_text.models__test_cast_bool_to_text_yml,
             "test_cast_bool_to_text.sql": self.interpolate_macro_namespace(
-                models__test_cast_bool_to_text_sql, "cast_bool_to_text"
+                fixture_cast_bool_to_text.models__test_cast_bool_to_text_sql, "cast_bool_to_text"
             ),
         }
 
 
 class TestCastBoolToText(BaseCastBoolToText):
     pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_concat.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_length.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import pytest
-from dbt.tests.adapter.utils.base_utils import BaseUtils
-from dbt.tests.adapter.utils.fixture_concat import (
-    seeds__data_concat_csv,
-    models__test_concat_sql,
-    models__test_concat_yml,
-)
 
+from dbt.tests.adapter.utils import base_utils, fixture_length
 
-class BaseConcat(BaseUtils):
+
+class BaseLength(base_utils.BaseUtils):
     @pytest.fixture(scope="class")
     def seeds(self):
-        return {"data_concat.csv": seeds__data_concat_csv}
+        return {"data_length.csv": fixture_length.seeds__data_length_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "test_concat.yml": models__test_concat_yml,
-            "test_concat.sql": self.interpolate_macro_namespace(models__test_concat_sql, "concat"),
+            "test_length.yml": fixture_length.models__test_length_yml,
+            "test_length.sql": self.interpolate_macro_namespace(
+                fixture_length.models__test_length_sql, "length"
+            ),
         }
 
 
-class TestConcat(BaseConcat):
+class TestLength(BaseLength):
     pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_current_timestamp.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_current_timestamp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-import pytest
+from datetime import datetime, timedelta, timezone
 
-from datetime import datetime
-from datetime import timezone
-from datetime import timedelta
+import pytest
 
-from dbt.tests.util import run_dbt
-from dbt.tests.util import relation_from_name
+from dbt.tests.util import relation_from_name, run_dbt
 
 
 models__current_ts_sql = """
 select {{ dbt.current_timestamp() }} as current_ts_column
 """
 
 
@@ -36,15 +33,16 @@
         sql_timestamp = result[0] if result is not None else None
         return sql_timestamp
 
     def test_current_timestamp_matches_utc(self, current_timestamp):
         sql_timestamp = current_timestamp
         now_utc = self.utcnow_matching_type(sql_timestamp)
         # Plenty of wiggle room if clocks aren't perfectly sync'd, etc
-        tolerance = timedelta(minutes=1)
+        # The clock on the macos image appears to be a few minutes slow in GHA, causing false negatives
+        tolerance = timedelta(minutes=5)
         assert (sql_timestamp > (now_utc - tolerance)) and (
             sql_timestamp < (now_utc + tolerance)
         ), f"SQL timestamp {sql_timestamp.isoformat()} is not close enough to Python UTC {now_utc.isoformat()}"
 
     def utcnow_matching_type(self, dt: datetime) -> datetime:
         """
         Current UTC datetime with the same timezone-awareness (or naiveness) as the input.
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_date_trunc.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_date_trunc.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import pytest
-from dbt.tests.adapter.utils.base_utils import BaseUtils
-from dbt.tests.adapter.utils.fixture_date_trunc import (
-    seeds__data_date_trunc_csv,
-    models__test_date_trunc_sql,
-    models__test_date_trunc_yml,
-)
 
+from dbt.tests.adapter.utils import base_utils, fixture_date_trunc
 
-class BaseDateTrunc(BaseUtils):
+
+class BaseDateTrunc(base_utils.BaseUtils):
     @pytest.fixture(scope="class")
     def seeds(self):
-        return {"data_date_trunc.csv": seeds__data_date_trunc_csv}
+        return {"data_date_trunc.csv": fixture_date_trunc.seeds__data_date_trunc_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "test_date_trunc.yml": models__test_date_trunc_yml,
+            "test_date_trunc.yml": fixture_date_trunc.models__test_date_trunc_yml,
             "test_date_trunc.sql": self.interpolate_macro_namespace(
-                models__test_date_trunc_sql, "date_trunc"
+                fixture_date_trunc.models__test_date_trunc_sql, "date_trunc"
             ),
         }
 
 
 class TestDateTrunc(BaseDateTrunc):
     pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_dateadd.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_dateadd.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import pytest
-from dbt.tests.adapter.utils.base_utils import BaseUtils
-from dbt.tests.adapter.utils.fixture_dateadd import (
-    seeds__data_dateadd_csv,
-    models__test_dateadd_sql,
-    models__test_dateadd_yml,
-)
 
+from dbt.tests.adapter.utils import base_utils, fixture_dateadd
 
-class BaseDateAdd(BaseUtils):
+
+class BaseDateAdd(base_utils.BaseUtils):
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "name": "test",
             # this is only needed for BigQuery, right?
             # no harm having it here until/unless there's an adapter that doesn't support the 'timestamp' type
             "seeds": {
@@ -24,21 +20,21 @@
                     },
                 },
             },
         }
 
     @pytest.fixture(scope="class")
     def seeds(self):
-        return {"data_dateadd.csv": seeds__data_dateadd_csv}
+        return {"data_dateadd.csv": fixture_dateadd.seeds__data_dateadd_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "test_dateadd.yml": models__test_dateadd_yml,
+            "test_dateadd.yml": fixture_dateadd.models__test_dateadd_yml,
             "test_dateadd.sql": self.interpolate_macro_namespace(
-                models__test_dateadd_sql, "dateadd"
+                fixture_dateadd.models__test_dateadd_sql, "dateadd"
             ),
         }
 
 
 class TestDateAdd(BaseDateAdd):
     pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_datediff.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_datediff.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import pytest
-from dbt.tests.adapter.utils.base_utils import BaseUtils
-from dbt.tests.adapter.utils.fixture_datediff import (
-    seeds__data_datediff_csv,
-    models__test_datediff_sql,
-    models__test_datediff_yml,
-)
 
+from dbt.tests.adapter.utils import base_utils, fixture_datediff
 
-class BaseDateDiff(BaseUtils):
+
+class BaseDateDiff(base_utils.BaseUtils):
     @pytest.fixture(scope="class")
     def seeds(self):
-        return {"data_datediff.csv": seeds__data_datediff_csv}
+        return {"data_datediff.csv": fixture_datediff.seeds__data_datediff_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "test_datediff.yml": models__test_datediff_yml,
+            "test_datediff.yml": fixture_datediff.models__test_datediff_yml,
             "test_datediff.sql": self.interpolate_macro_namespace(
-                models__test_datediff_sql, "datediff"
+                fixture_datediff.models__test_datediff_sql, "datediff"
             ),
         }
 
 
 class TestDateDiff(BaseDateDiff):
     pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_equals.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_equals.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 import pytest
-from dbt.tests.adapter.utils.base_utils import macros__equals_sql
-from dbt.tests.adapter.utils.fixture_equals import (
-    SEEDS__DATA_EQUALS_CSV,
-    MODELS__EQUAL_VALUES_SQL,
-    MODELS__NOT_EQUAL_VALUES_SQL,
-)
-from dbt.tests.util import run_dbt, relation_from_name
+
+from dbt.tests.adapter.utils import base_utils, fixture_equals
+from dbt.tests.util import relation_from_name, run_dbt
 
 
 class BaseEquals:
     @pytest.fixture(scope="class")
     def macros(self):
         return {
-            "equals.sql": macros__equals_sql,
+            "equals.sql": base_utils.macros__equals_sql,
         }
 
     @pytest.fixture(scope="class")
     def seeds(self):
         return {
-            "data_equals.csv": SEEDS__DATA_EQUALS_CSV,
+            "data_equals.csv": fixture_equals.SEEDS__DATA_EQUALS_CSV,
         }
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "equal_values.sql": MODELS__EQUAL_VALUES_SQL,
-            "not_equal_values.sql": MODELS__NOT_EQUAL_VALUES_SQL,
+            "equal_values.sql": fixture_equals.MODELS__EQUAL_VALUES_SQL,
+            "not_equal_values.sql": fixture_equals.MODELS__NOT_EQUAL_VALUES_SQL,
         }
 
     def test_equal_values(self, project):
         run_dbt(["seed"])
         run_dbt(["run"])
 
         # There are 9 cases total; 3 are equal and 6 are not equal
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_escape_single_quotes.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_escape_single_quotes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 import pytest
-from dbt.tests.adapter.utils.base_utils import BaseUtils
-from dbt.tests.adapter.utils.fixture_escape_single_quotes import (
-    models__test_escape_single_quotes_quote_sql,
-    models__test_escape_single_quotes_backslash_sql,
-    models__test_escape_single_quotes_yml,
-)
 
+from dbt.tests.adapter.utils import base_utils, fixture_escape_single_quotes
 
-class BaseEscapeSingleQuotesQuote(BaseUtils):
+
+class BaseEscapeSingleQuotesQuote(base_utils.BaseUtils):
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "test_escape_single_quotes.yml": models__test_escape_single_quotes_yml,
+            "test_escape_single_quotes.yml": fixture_escape_single_quotes.models__test_escape_single_quotes_yml,
             "test_escape_single_quotes.sql": self.interpolate_macro_namespace(
-                models__test_escape_single_quotes_quote_sql, "escape_single_quotes"
+                fixture_escape_single_quotes.models__test_escape_single_quotes_quote_sql,
+                "escape_single_quotes",
             ),
         }
 
 
-class BaseEscapeSingleQuotesBackslash(BaseUtils):
+class BaseEscapeSingleQuotesBackslash(base_utils.BaseUtils):
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "test_escape_single_quotes.yml": models__test_escape_single_quotes_yml,
+            "test_escape_single_quotes.yml": fixture_escape_single_quotes.models__test_escape_single_quotes_yml,
             "test_escape_single_quotes.sql": self.interpolate_macro_namespace(
-                models__test_escape_single_quotes_backslash_sql, "escape_single_quotes"
+                fixture_escape_single_quotes.models__test_escape_single_quotes_backslash_sql,
+                "escape_single_quotes",
             ),
         }
 
 
 class TestEscapeSingleQuotes(BaseEscapeSingleQuotesQuote):
     pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_except.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_except.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,46 @@
 import pytest
-from dbt.tests.util import run_dbt, check_relations_equal
-from dbt.tests.adapter.utils.base_utils import BaseUtils
-from dbt.tests.adapter.utils.fixture_except import (
-    seeds__data_except_a_csv,
-    seeds__data_except_b_csv,
-    seeds__data_except_a_minus_b_csv,
-    seeds__data_except_b_minus_a_csv,
-    models__data_except_empty_sql,
-    models__test_except_a_minus_b_sql,
-    models__test_except_b_minus_a_sql,
-    models__test_except_a_minus_a_sql,
-    models__test_except_a_minus_empty_sql,
-    models__test_except_empty_minus_a_sql,
-    models__test_except_empty_minus_empty_sql,
-)
 
+from dbt.tests.adapter.utils import base_utils, fixture_except
+from dbt.tests.util import check_relations_equal, run_dbt
 
-class BaseExcept(BaseUtils):
+
+class BaseExcept(base_utils.BaseUtils):
     @pytest.fixture(scope="class")
     def seeds(self):
         return {
-            "data_except_a.csv": seeds__data_except_a_csv,
-            "data_except_b.csv": seeds__data_except_b_csv,
-            "data_except_a_minus_b.csv": seeds__data_except_a_minus_b_csv,
-            "data_except_b_minus_a.csv": seeds__data_except_b_minus_a_csv,
+            "data_except_a.csv": fixture_except.seeds__data_except_a_csv,
+            "data_except_b.csv": fixture_except.seeds__data_except_b_csv,
+            "data_except_a_minus_b.csv": fixture_except.seeds__data_except_a_minus_b_csv,
+            "data_except_b_minus_a.csv": fixture_except.seeds__data_except_b_minus_a_csv,
         }
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
             "data_except_empty.sql": self.interpolate_macro_namespace(
-                models__data_except_empty_sql, "except"
+                fixture_except.models__data_except_empty_sql, "except"
             ),
             "test_except_a_minus_b.sql": self.interpolate_macro_namespace(
-                models__test_except_a_minus_b_sql, "except"
+                fixture_except.models__test_except_a_minus_b_sql, "except"
             ),
             "test_except_b_minus_a.sql": self.interpolate_macro_namespace(
-                models__test_except_b_minus_a_sql, "except"
+                fixture_except.models__test_except_b_minus_a_sql, "except"
             ),
             "test_except_a_minus_a.sql": self.interpolate_macro_namespace(
-                models__test_except_a_minus_a_sql, "except"
+                fixture_except.models__test_except_a_minus_a_sql, "except"
             ),
             "test_except_a_minus_empty.sql": self.interpolate_macro_namespace(
-                models__test_except_a_minus_empty_sql, "except"
+                fixture_except.models__test_except_a_minus_empty_sql, "except"
             ),
             "test_except_empty_minus_a.sql": self.interpolate_macro_namespace(
-                models__test_except_empty_minus_a_sql, "except"
+                fixture_except.models__test_except_empty_minus_a_sql, "except"
             ),
             "test_except_empty_minus_empty.sql": self.interpolate_macro_namespace(
-                models__test_except_empty_minus_empty_sql, "except"
+                fixture_except.models__test_except_empty_minus_empty_sql, "except"
             ),
         }
 
     def test_build_assert_equal(self, project):
         run_dbt(["deps"])
         run_dbt(["build"])
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_generate_series.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_generate_series.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import pytest
-from dbt.tests.adapter.utils.base_utils import BaseUtils
-from dbt.tests.adapter.utils.fixture_generate_series import (
-    models__test_generate_series_sql,
-    models__test_generate_series_yml,
-)
 
+from dbt.tests.adapter.utils import base_utils, fixture_generate_series
 
-class BaseGenerateSeries(BaseUtils):
+
+class BaseGenerateSeries(base_utils.BaseUtils):
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "test_generate_series.yml": models__test_generate_series_yml,
+            "test_generate_series.yml": fixture_generate_series.models__test_generate_series_yml,
             "test_generate_series.sql": self.interpolate_macro_namespace(
-                models__test_generate_series_sql, "generate_series"
+                fixture_generate_series.models__test_generate_series_sql, "generate_series"
             ),
         }
 
 
 class TestGenerateSeries(BaseGenerateSeries):
     pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_get_intervals_between.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_get_intervals_between.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import pytest
-from dbt.tests.adapter.utils.base_utils import BaseUtils
-from dbt.tests.adapter.utils.fixture_get_intervals_between import (
-    models__test_get_intervals_between_sql,
-    models__test_get_intervals_between_yml,
-)
 
+from dbt.tests.adapter.utils import base_utils, fixture_get_intervals_between
 
-class BaseGetIntervalsBetween(BaseUtils):
+
+class BaseGetIntervalsBetween(base_utils.BaseUtils):
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "test_get_intervals_between.yml": models__test_get_intervals_between_yml,
+            "test_get_intervals_between.yml": fixture_get_intervals_between.models__test_get_intervals_between_yml,
             "test_get_intervals_between.sql": self.interpolate_macro_namespace(
-                models__test_get_intervals_between_sql, "get_intervals_between"
+                fixture_get_intervals_between.models__test_get_intervals_between_sql,
+                "get_intervals_between",
             ),
         }
 
 
 class TestGetIntervalsBetween(BaseGetIntervalsBetween):
     pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_get_powers_of_two.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_get_powers_of_two.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import pytest
-from dbt.tests.adapter.utils.base_utils import BaseUtils
-from dbt.tests.adapter.utils.fixture_get_powers_of_two import (
-    models__test_get_powers_of_two_sql,
-    models__test_get_powers_of_two_yml,
-)
 
+from dbt.tests.adapter.utils import base_utils, fixture_get_powers_of_two
 
-class BaseGetPowersOfTwo(BaseUtils):
+
+class BaseGetPowersOfTwo(base_utils.BaseUtils):
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "test_get_powers_of_two.yml": models__test_get_powers_of_two_yml,
+            "test_get_powers_of_two.yml": fixture_get_powers_of_two.models__test_get_powers_of_two_yml,
             "test_get_powers_of_two.sql": self.interpolate_macro_namespace(
-                models__test_get_powers_of_two_sql, "get_powers_of_two"
+                fixture_get_powers_of_two.models__test_get_powers_of_two_sql, "get_powers_of_two"
             ),
         }
 
 
 class TestGetPowersOfTwo(BaseGetPowersOfTwo):
     pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_hash.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_hash.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import pytest
-from dbt.tests.adapter.utils.base_utils import BaseUtils
-from dbt.tests.adapter.utils.fixture_hash import (
-    seeds__data_hash_csv,
-    models__test_hash_sql,
-    models__test_hash_yml,
-)
 
+from dbt.tests.adapter.utils import base_utils, fixture_hash
 
-class BaseHash(BaseUtils):
+
+class BaseHash(base_utils.BaseUtils):
     @pytest.fixture(scope="class")
     def seeds(self):
-        return {"data_hash.csv": seeds__data_hash_csv}
+        return {"data_hash.csv": fixture_hash.seeds__data_hash_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "test_hash.yml": models__test_hash_yml,
-            "test_hash.sql": self.interpolate_macro_namespace(models__test_hash_sql, "hash"),
+            "test_hash.yml": fixture_hash.models__test_hash_yml,
+            "test_hash.sql": self.interpolate_macro_namespace(
+                fixture_hash.models__test_hash_sql, "hash"
+            ),
         }
 
 
 class TestHash(BaseHash):
     pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_intersect.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_intersect.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,45 @@
 import pytest
-from dbt.tests.util import run_dbt, check_relations_equal
-from dbt.tests.adapter.utils.base_utils import BaseUtils
-from dbt.tests.adapter.utils.fixture_intersect import (
-    seeds__data_intersect_a_csv,
-    seeds__data_intersect_b_csv,
-    seeds__data_intersect_a_overlap_b_csv,
-    models__data_intersect_empty_sql,
-    models__test_intersect_a_overlap_b_sql,
-    models__test_intersect_b_overlap_a_sql,
-    models__test_intersect_a_overlap_a_sql,
-    models__test_intersect_a_overlap_empty_sql,
-    models__test_intersect_empty_overlap_a_sql,
-    models__test_intersect_empty_overlap_empty_sql,
-)
 
+from dbt.tests.adapter.utils import base_utils, fixture_intersect
+from dbt.tests.util import check_relations_equal, run_dbt
 
-class BaseIntersect(BaseUtils):
+
+class BaseIntersect(base_utils.BaseUtils):
     @pytest.fixture(scope="class")
     def seeds(self):
         return {
-            "data_intersect_a.csv": seeds__data_intersect_a_csv,
-            "data_intersect_b.csv": seeds__data_intersect_b_csv,
-            "data_intersect_a_overlap_b.csv": seeds__data_intersect_a_overlap_b_csv,
+            "data_intersect_a.csv": fixture_intersect.seeds__data_intersect_a_csv,
+            "data_intersect_b.csv": fixture_intersect.seeds__data_intersect_b_csv,
+            "data_intersect_a_overlap_b.csv": fixture_intersect.seeds__data_intersect_a_overlap_b_csv,
         }
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
             "data_intersect_empty.sql": self.interpolate_macro_namespace(
-                models__data_intersect_empty_sql, "intersect"
+                fixture_intersect.models__data_intersect_empty_sql, "intersect"
             ),
             "test_intersect_a_overlap_b.sql": self.interpolate_macro_namespace(
-                models__test_intersect_a_overlap_b_sql, "intersect"
+                fixture_intersect.models__test_intersect_a_overlap_b_sql, "intersect"
             ),
             "test_intersect_b_overlap_a.sql": self.interpolate_macro_namespace(
-                models__test_intersect_b_overlap_a_sql, "intersect"
+                fixture_intersect.models__test_intersect_b_overlap_a_sql, "intersect"
             ),
             "test_intersect_a_overlap_a.sql": self.interpolate_macro_namespace(
-                models__test_intersect_a_overlap_a_sql, "intersect"
+                fixture_intersect.models__test_intersect_a_overlap_a_sql, "intersect"
             ),
             "test_intersect_a_overlap_empty.sql": self.interpolate_macro_namespace(
-                models__test_intersect_a_overlap_empty_sql, "intersect"
+                fixture_intersect.models__test_intersect_a_overlap_empty_sql, "intersect"
             ),
             "test_intersect_empty_overlap_a.sql": self.interpolate_macro_namespace(
-                models__test_intersect_empty_overlap_a_sql, "intersect"
+                fixture_intersect.models__test_intersect_empty_overlap_a_sql, "intersect"
             ),
             "test_intersect_empty_overlap_empty.sql": self.interpolate_macro_namespace(
-                models__test_intersect_empty_overlap_empty_sql, "intersect"
+                fixture_intersect.models__test_intersect_empty_overlap_empty_sql, "intersect"
             ),
         }
 
     def test_build_assert_equal(self, project):
         run_dbt(["deps"])
         run_dbt(["build"])
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_last_day.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_last_day.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import pytest
-from dbt.tests.adapter.utils.base_utils import BaseUtils
-from dbt.tests.adapter.utils.fixture_last_day import (
-    seeds__data_last_day_csv,
-    models__test_last_day_sql,
-    models__test_last_day_yml,
-)
 
+from dbt.tests.adapter.utils import base_utils, fixture_last_day
 
-class BaseLastDay(BaseUtils):
+
+class BaseLastDay(base_utils.BaseUtils):
     @pytest.fixture(scope="class")
     def seeds(self):
-        return {"data_last_day.csv": seeds__data_last_day_csv}
+        return {"data_last_day.csv": fixture_last_day.seeds__data_last_day_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "test_last_day.yml": models__test_last_day_yml,
+            "test_last_day.yml": fixture_last_day.models__test_last_day_yml,
             "test_last_day.sql": self.interpolate_macro_namespace(
-                models__test_last_day_sql, "last_day"
+                fixture_last_day.models__test_last_day_sql, "last_day"
             ),
         }
 
 
 class TestLastDay(BaseLastDay):
     pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_length.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_position.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import pytest
-from dbt.tests.adapter.utils.base_utils import BaseUtils
-from dbt.tests.adapter.utils.fixture_length import (
-    seeds__data_length_csv,
-    models__test_length_sql,
-    models__test_length_yml,
-)
 
+from dbt.tests.adapter.utils import base_utils, fixture_position
 
-class BaseLength(BaseUtils):
+
+class BasePosition(base_utils.BaseUtils):
     @pytest.fixture(scope="class")
     def seeds(self):
-        return {"data_length.csv": seeds__data_length_csv}
+        return {"data_position.csv": fixture_position.seeds__data_position_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "test_length.yml": models__test_length_yml,
-            "test_length.sql": self.interpolate_macro_namespace(models__test_length_sql, "length"),
+            "test_position.yml": fixture_position.models__test_position_yml,
+            "test_position.sql": self.interpolate_macro_namespace(
+                fixture_position.models__test_position_sql, "position"
+            ),
         }
 
 
-class TestLength(BaseLength):
+class TestPosition(BasePosition):
     pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_listagg.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_listagg.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 import pytest
-from dbt.tests.adapter.utils.base_utils import BaseUtils
-from dbt.tests.adapter.utils.fixture_listagg import (
-    seeds__data_listagg_csv,
-    seeds__data_listagg_output_csv,
-    models__test_listagg_sql,
-    models__test_listagg_yml,
-)
 
+from dbt.tests.adapter.utils import base_utils, fixture_listagg
 
-class BaseListagg(BaseUtils):
+
+class BaseListagg(base_utils.BaseUtils):
     @pytest.fixture(scope="class")
     def seeds(self):
         return {
-            "data_listagg.csv": seeds__data_listagg_csv,
-            "data_listagg_output.csv": seeds__data_listagg_output_csv,
+            "data_listagg.csv": fixture_listagg.seeds__data_listagg_csv,
+            "data_listagg_output.csv": fixture_listagg.seeds__data_listagg_output_csv,
         }
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "test_listagg.yml": models__test_listagg_yml,
+            "test_listagg.yml": fixture_listagg.models__test_listagg_yml,
             "test_listagg.sql": self.interpolate_macro_namespace(
-                models__test_listagg_sql, "listagg"
+                fixture_listagg.models__test_listagg_sql, "listagg"
             ),
         }
 
 
 class TestListagg(BaseListagg):
     pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_safe_cast.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_safe_cast.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import pytest
-from dbt.tests.adapter.utils.base_utils import BaseUtils
-from dbt.tests.adapter.utils.fixture_safe_cast import (
-    seeds__data_safe_cast_csv,
-    models__test_safe_cast_sql,
-    models__test_safe_cast_yml,
-)
 
+from dbt.tests.adapter.utils import base_utils, fixture_safe_cast
 
-class BaseSafeCast(BaseUtils):
+
+class BaseSafeCast(base_utils.BaseUtils):
     @pytest.fixture(scope="class")
     def seeds(self):
-        return {"data_safe_cast.csv": seeds__data_safe_cast_csv}
+        return {"data_safe_cast.csv": fixture_safe_cast.seeds__data_safe_cast_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "test_safe_cast.yml": models__test_safe_cast_yml,
+            "test_safe_cast.yml": fixture_safe_cast.models__test_safe_cast_yml,
             "test_safe_cast.sql": self.interpolate_macro_namespace(
-                self.interpolate_macro_namespace(models__test_safe_cast_sql, "safe_cast"),
+                self.interpolate_macro_namespace(
+                    fixture_safe_cast.models__test_safe_cast_sql, "safe_cast"
+                ),
                 "type_string",
             ),
         }
 
 
 class TestSafeCast(BaseSafeCast):
     pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_split_part.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_split_part.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import pytest
-from dbt.tests.adapter.utils.base_utils import BaseUtils
-from dbt.tests.adapter.utils.fixture_split_part import (
-    seeds__data_split_part_csv,
-    models__test_split_part_sql,
-    models__test_split_part_yml,
-)
 
+from dbt.tests.adapter.utils import base_utils, fixture_split_part
 
-class BaseSplitPart(BaseUtils):
+
+class BaseSplitPart(base_utils.BaseUtils):
     @pytest.fixture(scope="class")
     def seeds(self):
-        return {"data_split_part.csv": seeds__data_split_part_csv}
+        return {"data_split_part.csv": fixture_split_part.seeds__data_split_part_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "test_split_part.yml": models__test_split_part_yml,
+            "test_split_part.yml": fixture_split_part.models__test_split_part_yml,
             "test_split_part.sql": self.interpolate_macro_namespace(
-                models__test_split_part_sql, "split_part"
+                fixture_split_part.models__test_split_part_sql, "split_part"
             ),
         }
 
 
 class TestSplitPart(BaseSplitPart):
     pass
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_timestamps.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_timestamps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-import pytest
 import re
+
+import pytest
+
 from dbt.tests.util import check_relation_has_expected_schema, run_dbt
 
+
 _MODEL_CURRENT_TIMESTAMP = """
 select {{ current_timestamp() }} as current_timestamp,
        {{ current_timestamp_in_utc_backcompat() }} as current_timestamp_in_utc_backcompat,
        {{ current_timestamp_backcompat() }} as current_timestamp_backcompat
 """
 
 _MODEL_EXPECTED_SQL = """
```

### Comparing `dbt-tests-adapter-1.7.9/dbt/tests/adapter/utils/test_validate_sql.py` & `dbt_tests_adapter-1.8.0b1/dbt/tests/adapter/utils/test_validate_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Type
 
+from dbt_common.exceptions import DbtRuntimeError
 import pytest
 
 from dbt.adapters.base.impl import BaseAdapter
-from dbt.exceptions import DbtRuntimeError, InvalidConnectionError
+from dbt.adapters.exceptions import InvalidConnectionError
 
 
 class BaseValidateSqlMethod:
     """Tests the behavior of the validate_sql method for the relevant adapters.
 
     The valid and invalid SQL should work with most engines by default, but
     both inputs can be overridden as needed for a given engine to get the correct
@@ -37,15 +38,15 @@
 
         return "Let's run some invalid SQL and see if we get an error!"
 
     @pytest.fixture(scope="class")
     def expected_exception(self) -> Type[Exception]:
         """Returns the Exception type thrown by a failed query.
 
-        Defaults to dbt.exceptions.DbtRuntimeError because that is the most common
+        Defaults to dbt_common.exceptions.DbtRuntimeError because that is the most common
         base exception for adapters to throw."""
         return DbtRuntimeError
 
     def test_validate_sql_success(self, adapter: BaseAdapter, valid_sql: str) -> None:
         """Executes validate_sql on valid SQL. No news is good news."""
         with adapter.connection_named("test_valid_sql_validation"):
             adapter.validate_sql(valid_sql)
```

