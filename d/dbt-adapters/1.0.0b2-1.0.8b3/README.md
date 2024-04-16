# Comparing `tmp/dbt_adapters-1.0.0b2.tar.gz` & `tmp/dbt_adapters-1.0.8b3.tar.gz`

## Comparing `dbt_adapters-1.0.0b2.tar` & `dbt_adapters-1.0.8b3.tar`

### file list

```diff
@@ -1,154 +1,154 @@
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/__about__.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/__init__.py
--rw-r--r--   0        0        0    20084 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/cache.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/capability.py
--rw-r--r--   0        0        0     9021 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/factory.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/protocol.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/py.typed
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/reference_keys.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/utils.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/base/README.md
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/base/__init__.py
--rw-r--r--   0        0        0     5450 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/base/column.py
--rw-r--r--   0        0        0    16921 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/base/connections.py
--rw-r--r--   0        0        0    64403 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/base/impl.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/base/meta.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/base/plugin.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/base/query_headers.py
--rw-r--r--   0        0        0    15642 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/base/relation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/clients/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/clients/jinja.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/contracts/__init__.py
--rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/contracts/connection.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/contracts/macros.py
--rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/contracts/relation.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/events/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/events/__init__.py
--rw-r--r--   0        0        0     9484 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/events/adapter_types.proto
--rw-r--r--   0        0        0    26048 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/events/adapter_types_pb2.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/events/base_types.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/events/logging.py
--rw-r--r--   0        0        0    11726 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/events/types.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/exceptions/__init__.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/exceptions/alias.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/exceptions/cache.py
--rw-r--r--   0        0        0     8586 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/exceptions/compilation.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/exceptions/connection.py
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/exceptions/database.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/relation_configs/README.md
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/relation_configs/__init__.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/relation_configs/config_base.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/relation_configs/config_change.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/relation_configs/config_validation.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/sql/__init__.py
--rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/sql/connections.py
--rw-r--r--   0        0        0    10722 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/sql/impl.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/py.typed
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/__init__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/dbt_project.yml
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/docs/overview.md
--rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/apply_grants.sql
--rw-r--r--   0        0        0     5438 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/columns.sql
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/freshness.sql
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/indexes.sql
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/metadata.sql
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/persist_docs.sql
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/relation.sql
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/schema.sql
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/show.sql
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/timestamps.sql
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/validate_sql.sql
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/etc/datetime.sql
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/etc/statement.sql
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/generic_test_sql/not_null.sql
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/generic_test_sql/relationships.sql
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/generic_test_sql/unique.sql
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/configs.sql
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/hooks.sql
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/materialized_view.sql
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/table.sql
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/view.sql
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/clone/can_clone_table.sql
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/clone/clone.sql
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/clone/create_or_replace_clone.sql
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/seeds/helpers.sql
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/seeds/seed.sql
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/tests/helpers.sql
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/tests/test.sql
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/tests/unit.sql
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/python_model/python.sql
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/create.sql
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/create_backup.sql
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/create_intermediate.sql
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/drop.sql
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/drop_backup.sql
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/rename.sql
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/rename_intermediate.sql
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/replace.sql
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/schema.sql
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/column/columns_spec_ddl.sql
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/materialized_view/alter.sql
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/materialized_view/create.sql
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/materialized_view/drop.sql
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/materialized_view/refresh.sql
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/materialized_view/rename.sql
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/materialized_view/replace.sql
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/table/create.sql
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/table/drop.sql
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/table/rename.sql
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/table/replace.sql
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/view/create.sql
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/view/drop.sql
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/view/rename.sql
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/view/replace.sql
--rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/unit_test_sql/get_fixture_sql.sql
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/any_value.sql
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/array_append.sql
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/array_concat.sql
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/array_construct.sql
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/bool_or.sql
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/cast.sql
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/concat.sql
--rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/data_types.sql
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/date_spine.sql
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/date_trunc.sql
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/dateadd.sql
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/datediff.sql
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/escape_single_quotes.sql
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/except.sql
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/generate_series.sql
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/hash.sql
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/intersect.sql
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/last_day.sql
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/length.sql
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/listagg.sql
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/literal.sql
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/position.sql
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/replace.sql
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/right.sql
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/safe_cast.sql
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/split_part.sql
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/tests/generic/builtin.sql
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/.gitignore
--rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/LICENSE
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/README.md
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/pyproject.toml
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/__about__.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/__init__.py
+-rw-r--r--   0        0        0    20084 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/cache.py
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/capability.py
+-rw-r--r--   0        0        0     9423 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/factory.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/protocol.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/py.typed
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/reference_keys.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/utils.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/base/README.md
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/base/__init__.py
+-rw-r--r--   0        0        0     5450 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/base/column.py
+-rw-r--r--   0        0        0    16921 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/base/connections.py
+-rw-r--r--   0        0        0    68316 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/base/impl.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/base/meta.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/base/plugin.py
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/base/query_headers.py
+-rw-r--r--   0        0        0    15642 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/base/relation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/clients/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/clients/jinja.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/contracts/__init__.py
+-rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/contracts/connection.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/contracts/macros.py
+-rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/contracts/relation.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/events/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/events/__init__.py
+-rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/events/adapter_types.proto
+-rw-r--r--   0        0        0    26480 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/events/adapter_types_pb2.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/events/base_types.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/events/logging.py
+-rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/events/types.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/exceptions/__init__.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/exceptions/alias.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/exceptions/cache.py
+-rw-r--r--   0        0        0     8586 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/exceptions/compilation.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/exceptions/connection.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/exceptions/database.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/relation_configs/README.md
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/relation_configs/__init__.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/relation_configs/config_base.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/relation_configs/config_change.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/relation_configs/config_validation.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/sql/__init__.py
+-rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/sql/connections.py
+-rw-r--r--   0        0        0    10722 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/adapters/sql/impl.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/py.typed
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/__init__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/dbt_project.yml
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/docs/overview.md
+-rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/adapters/apply_grants.sql
+-rw-r--r--   0        0        0     5438 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/adapters/columns.sql
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/adapters/freshness.sql
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/adapters/indexes.sql
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/adapters/metadata.sql
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/adapters/persist_docs.sql
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/adapters/relation.sql
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/adapters/schema.sql
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/adapters/show.sql
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/adapters/timestamps.sql
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/adapters/validate_sql.sql
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/etc/datetime.sql
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/etc/statement.sql
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/generic_test_sql/not_null.sql
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/generic_test_sql/relationships.sql
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/generic_test_sql/unique.sql
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/configs.sql
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/hooks.sql
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/models/materialized_view.sql
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/models/table.sql
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/models/view.sql
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/models/clone/can_clone_table.sql
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/models/clone/clone.sql
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/models/clone/create_or_replace_clone.sql
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/seeds/seed.sql
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/tests/helpers.sql
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/tests/test.sql
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/tests/unit.sql
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/python_model/python.sql
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/create.sql
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/create_backup.sql
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/create_intermediate.sql
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/drop.sql
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/drop_backup.sql
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/rename.sql
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/rename_intermediate.sql
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/replace.sql
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/schema.sql
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/column/columns_spec_ddl.sql
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/materialized_view/alter.sql
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/materialized_view/create.sql
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/materialized_view/drop.sql
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/materialized_view/refresh.sql
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/materialized_view/rename.sql
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/materialized_view/replace.sql
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/table/create.sql
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/table/drop.sql
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/table/rename.sql
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/table/replace.sql
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/view/create.sql
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/view/drop.sql
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/view/rename.sql
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/view/replace.sql
+-rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/unit_test_sql/get_fixture_sql.sql
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/any_value.sql
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/array_append.sql
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/array_concat.sql
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/array_construct.sql
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/bool_or.sql
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/cast.sql
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/concat.sql
+-rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/data_types.sql
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/date_spine.sql
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/date_trunc.sql
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/dateadd.sql
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/datediff.sql
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/except.sql
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/generate_series.sql
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/hash.sql
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/intersect.sql
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/last_day.sql
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/length.sql
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/listagg.sql
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/literal.sql
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/position.sql
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/replace.sql
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/right.sql
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/safe_cast.sql
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/split_part.sql
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/dbt/include/global_project/tests/generic/builtin.sql
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/.gitignore
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/LICENSE
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/README.md
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/pyproject.toml
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 dbt_adapters-1.0.8b3/PKG-INFO
```

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/cache.py` & `dbt_adapters-1.0.8b3/dbt/adapters/cache.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/capability.py` & `dbt_adapters-1.0.8b3/dbt/adapters/capability.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,17 @@
     SchemaMetadataByRelations = "SchemaMetadataByRelations"
     """Indicates efficient support for retrieving schema metadata for a list of relations, rather than always retrieving
     all the relations in a schema."""
 
     TableLastModifiedMetadata = "TableLastModifiedMetadata"
     """Indicates support for determining the time of the last table modification by querying database metadata."""
 
+    TableLastModifiedMetadataBatch = "TableLastModifiedMetadataBatch"
+    """Indicates support for performantly determining the time of the last table modification by querying database metadata in batch."""
+
 
 class Support(str, Enum):
     Unknown = "Unknown"
     """The adapter has not declared whether this capability is a feature of the underlying DBMS."""
 
     Unsupported = "Unsupported"
     """This capability is not possible with the underlying DBMS, so the adapter does not implement related macros."""
```

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/factory.py` & `dbt_adapters-1.0.8b3/dbt/adapters/factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from multiprocessing.context import SpawnContext
 from pathlib import Path
 import threading
 import traceback
 from typing import Any, Dict, List, Optional, Set, Type
 
 from dbt_common.events.functions import fire_event
+from dbt_common.events.base_types import EventLevel
 from dbt_common.exceptions import DbtInternalError, DbtRuntimeError
 from dbt_common.semver import VersionSpecifier
 
 from dbt.adapters.base.plugin import AdapterPlugin
 from dbt.adapters.contracts.connection import AdapterRequiredConfig, Credentials
 from dbt.adapters.events.types import (
     AdapterImportError,
@@ -92,19 +93,30 @@
         self.packages[plugin.project_name] = Path(plugin.include_path)
 
         for dep in plugin.dependencies:
             self.load_plugin(dep)
 
         return plugin.credentials
 
-    def register_adapter(self, config: AdapterRequiredConfig, mp_context: SpawnContext) -> None:
+    def register_adapter(
+        self,
+        config: AdapterRequiredConfig,
+        mp_context: SpawnContext,
+        adapter_registered_log_level: Optional[EventLevel] = EventLevel.INFO
+    ) -> None:
         adapter_name = config.credentials.type
         adapter_type = self.get_adapter_class_by_name(adapter_name)
         adapter_version = self._adapter_version(adapter_name)
-        fire_event(AdapterRegistered(adapter_name=adapter_name, adapter_version=adapter_version))
+        fire_event(
+            AdapterRegistered(
+                adapter_name=adapter_name,
+                adapter_version=adapter_version
+            ),
+            level=adapter_registered_log_level
+        )
         with self.lock:
             if adapter_name in self.adapters:
                 # this shouldn't really happen...
                 return
 
             adapter: Adapter = adapter_type(config, mp_context)  # type: ignore
             self.adapters[adapter_name] = adapter
@@ -182,16 +194,20 @@
     def get_adapter_constraint_support(self, name: Optional[str]) -> List[str]:
         return self.lookup_adapter(name).CONSTRAINT_SUPPORT  # type: ignore
 
 
 FACTORY: AdapterContainer = AdapterContainer()
 
 
-def register_adapter(config: AdapterRequiredConfig, mp_context: SpawnContext) -> None:
-    FACTORY.register_adapter(config, mp_context)
+def register_adapter(
+        config: AdapterRequiredConfig,
+        mp_context: SpawnContext,
+        adapter_registered_log_level: Optional[EventLevel] = EventLevel.INFO
+) -> None:
+    FACTORY.register_adapter(config, mp_context, adapter_registered_log_level)
 
 
 def get_adapter(config: AdapterRequiredConfig):
     return FACTORY.lookup_adapter(config.credentials.type)
 
 
 def get_adapter_by_type(adapter_type):
```

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/protocol.py` & `dbt_adapters-1.0.8b3/dbt/adapters/protocol.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/reference_keys.py` & `dbt_adapters-1.0.8b3/dbt/adapters/reference_keys.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/utils.py` & `dbt_adapters-1.0.8b3/dbt/adapters/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/base/README.md` & `dbt_adapters-1.0.8b3/dbt/adapters/base/README.md`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/base/column.py` & `dbt_adapters-1.0.8b3/dbt/adapters/base/column.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/base/connections.py` & `dbt_adapters-1.0.8b3/dbt/adapters/base/connections.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/base/impl.py` & `dbt_adapters-1.0.8b3/dbt/adapters/base/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1058,26 +1058,31 @@
     def execute_macro(
         self,
         macro_name: str,
         macro_resolver: Optional[MacroResolverProtocol] = None,
         project: Optional[str] = None,
         context_override: Optional[Dict[str, Any]] = None,
         kwargs: Optional[Dict[str, Any]] = None,
+        needs_conn: bool = False,
     ) -> AttrDict:
         """Look macro_name up in the manifest and execute its results.
 
         :param macro_name: The name of the macro to execute.
         :param manifest: The manifest to use for generating the base macro
             execution context. If none is provided, use the internal manifest.
         :param project: The name of the project to search in, or None for the
             first match.
         :param context_override: An optional dict to update() the macro
             execution context.
         :param kwargs: An optional dict of keyword args used to pass to the
             macro.
+        : param needs_conn: A boolean that indicates whether the specified macro
+            requires an open connection to execute. If needs_conn is True, a
+            connection is expected and opened if necessary. Otherwise (and by default),
+            no connection is expected prior to executing the macro.
         """
 
         if kwargs is None:
             kwargs = {}
         if context_override is None:
             context_override = {}
 
@@ -1102,14 +1107,18 @@
             )
 
         macro_context = self._macro_context_generator(macro, self.config, resolver, project)
         macro_context.update(context_override)
 
         macro_function = CallableMacroGenerator(macro, macro_context)
 
+        if needs_conn:
+            connection = self.connections.get_thread_connection()
+            self.connections.open(connection)
+
         with self.connections.exception_handler(f"macro {macro_name}"):
             result = macro_function(**kwargs)
         return result
 
     @classmethod
     def _catalog_filter_table(
         cls, table: "agate.Table", used_schemas: FrozenSet[Tuple[str, str]]
@@ -1293,56 +1302,118 @@
         freshness: FreshnessResponse = {
             "max_loaded_at": max_loaded_at,
             "snapshotted_at": snapshotted_at,
             "age": age,
         }
         return adapter_response, freshness
 
+    def calculate_freshness_from_metadata_batch(
+        self,
+        sources: List[BaseRelation],
+        macro_resolver: Optional[MacroResolverProtocol] = None,
+    ) -> Tuple[List[Optional[AdapterResponse]], Dict[BaseRelation, FreshnessResponse]]:
+        """
+        Given a list of sources (BaseRelations), calculate the metadata-based freshness in batch.
+        This method should _not_ execute a warehouse query per source, but rather batch up
+        the sources into as few requests as possible to minimize the number of roundtrips required
+        to compute metadata-based freshness for each input source.
+
+        :param sources: The list of sources to calculate metadata-based freshness for
+        :param macro_resolver: An optional macro_resolver to use for get_relation_last_modified
+        :return: a tuple where:
+            * the first element is a list of optional AdapterResponses indicating the response
+              for each request the method made to compute the freshness for the provided sources.
+            * the second element is a dictionary mapping an input source BaseRelation to a FreshnessResponse,
+              if it was possible to calculate a FreshnessResponse for the source.
+        """
+        # Track schema, identifiers of sources for lookup from batch query
+        schema_identifier_to_source = {
+            (
+                source.path.get_lowered_part(ComponentName.Schema),
+                source.path.get_lowered_part(ComponentName.Identifier),
+            ): source
+            for source in sources
+        }
+
+        # Group metadata sources by information schema -- one query per information schema will be necessary
+        sources_by_info_schema: Dict[InformationSchema, List[BaseRelation]] = self._get_catalog_relations_by_info_schema(sources)
+
+        freshness_responses: Dict[BaseRelation, FreshnessResponse] = {}
+        adapter_responses: List[Optional[AdapterResponse]] = []
+        for (
+            information_schema,
+            sources_for_information_schema,
+        ) in sources_by_info_schema.items():
+            result = self.execute_macro(
+                GET_RELATION_LAST_MODIFIED_MACRO_NAME,
+                kwargs={
+                    "information_schema": information_schema,
+                    "relations": sources_for_information_schema,
+                },
+                macro_resolver=macro_resolver,
+                needs_conn=True,
+            )
+            adapter_response, table = result.response, result.table  # type: ignore[attr-defined]
+            adapter_responses.append(adapter_response)
+
+            for row in table:
+                raw_relation, freshness_response = self._parse_freshness_row(row, table)
+                source_relation_for_result = schema_identifier_to_source[raw_relation]
+                freshness_responses[source_relation_for_result] = freshness_response
+
+        return adapter_responses, freshness_responses
+
     def calculate_freshness_from_metadata(
         self,
         source: BaseRelation,
         macro_resolver: Optional[MacroResolverProtocol] = None,
     ) -> Tuple[Optional[AdapterResponse], FreshnessResponse]:
-        kwargs: Dict[str, Any] = {
-            "information_schema": source.information_schema_only(),
-            "relations": [source],
-        }
-        result = self.execute_macro(
-            GET_RELATION_LAST_MODIFIED_MACRO_NAME,
-            kwargs=kwargs,
+        adapter_responses, freshness_responses = self.calculate_freshness_from_metadata_batch(
+            sources=[source],
             macro_resolver=macro_resolver,
         )
-        adapter_response, table = result.response, result.table  # type: ignore[attr-defined]
-
-        try:
-            from dbt_common.clients.agate_helper import get_column_value_uncased
+        adapter_response = adapter_responses[0] if adapter_responses else None
+        return adapter_response, freshness_responses[source]
 
-            row = table[0]
-            last_modified_val = get_column_value_uncased("last_modified", row)
-            snapshotted_at_val = get_column_value_uncased("snapshotted_at", row)
-        except Exception:
-            raise MacroResultError(GET_RELATION_LAST_MODIFIED_MACRO_NAME, table)
-
-        if last_modified_val is None:
+    def _create_freshness_response(
+        self, last_modified: Optional[datetime], snapshotted_at: Optional[datetime]
+    ) -> FreshnessResponse:
+        if last_modified is None:
             # Interpret missing value as "infinitely long ago"
             max_loaded_at = datetime(1, 1, 1, 0, 0, 0, tzinfo=pytz.UTC)
         else:
-            max_loaded_at = _utc(last_modified_val, None, "last_modified")
-
-        snapshotted_at = _utc(snapshotted_at_val, None, "snapshotted_at")
+            max_loaded_at = _utc(last_modified, None, "last_modified")
 
+        snapshotted_at = _utc(snapshotted_at, None, "snapshotted_at")
         age = (snapshotted_at - max_loaded_at).total_seconds()
-
         freshness: FreshnessResponse = {
             "max_loaded_at": max_loaded_at,
             "snapshotted_at": snapshotted_at,
             "age": age,
         }
 
-        return adapter_response, freshness
+        return freshness
+
+    def _parse_freshness_row(self, row: "agate.Row", table: "agate.Table") -> Tuple[Any, FreshnessResponse]:
+        from dbt_common.clients.agate_helper import get_column_value_uncased
+
+        try:
+            last_modified_val = get_column_value_uncased("last_modified", row)
+            snapshotted_at_val = get_column_value_uncased("snapshotted_at", row)
+            identifier = get_column_value_uncased("identifier", row)
+            schema = get_column_value_uncased("schema", row)
+        except Exception:
+            raise MacroResultError(GET_RELATION_LAST_MODIFIED_MACRO_NAME, table)
+
+        freshness_response = self._create_freshness_response(
+            last_modified_val,
+            snapshotted_at_val
+        )
+        raw_relation = schema.lower().strip(), identifier.lower().strip()
+        return raw_relation, freshness_response
 
     def pre_model_hook(self, config: Mapping[str, Any]) -> Any:
         """A hook for running some operation before the model materialization
         runs. The hook can assume it has a connection available.
 
         The only parameter is a configuration dictionary (the same one
         available in the materialization context). It should be considered
```

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/base/meta.py` & `dbt_adapters-1.0.8b3/dbt/adapters/base/meta.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/base/plugin.py` & `dbt_adapters-1.0.8b3/dbt/adapters/base/plugin.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/base/query_headers.py` & `dbt_adapters-1.0.8b3/dbt/adapters/base/query_headers.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/base/relation.py` & `dbt_adapters-1.0.8b3/dbt/adapters/base/relation.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/clients/jinja.py` & `dbt_adapters-1.0.8b3/dbt/adapters/clients/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/contracts/connection.py` & `dbt_adapters-1.0.8b3/dbt/adapters/contracts/connection.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/contracts/relation.py` & `dbt_adapters-1.0.8b3/dbt/adapters/contracts/relation.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/events/README.md` & `dbt_adapters-1.0.8b3/dbt/adapters/events/README.md`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/events/adapter_types.proto` & `dbt_adapters-1.0.8b3/dbt/adapters/events/adapter_types.proto`

 * *Files 1% similar despite different names*

```diff
@@ -511,7 +511,17 @@
     string adapter = 2;
 }
 
 message ConstraintNotSupportedMsg {
     AdapterCommonEventInfo info = 1;
     ConstraintNotSupported data = 2;
 }
+
+// E050
+message TypeCodeNotFound {
+    int32 type_code = 1;
+}
+
+message TypeCodeNotFoundMsg {
+    AdapterCommonEventInfo info = 1;
+    TypeCodeNotFound data = 2;
+}
```

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/events/adapter_types_pb2.py` & `dbt_adapters-1.0.8b3/dbt/adapters/events/adapter_types_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: adapter_types.proto
-# Protobuf Python Version: 4.25.2
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13\x61\x64\x61pter_types.proto\x12\x0bproto_types\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"\xab\x02\n\x16\x41\x64\x61pterCommonEventInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0b\n\x03msg\x18\x03 \x01(\t\x12\r\n\x05level\x18\x04 \x01(\t\x12\x15\n\rinvocation_id\x18\x05 \x01(\t\x12\x0b\n\x03pid\x18\x06 \x01(\x05\x12\x0e\n\x06thread\x18\x07 \x01(\t\x12&\n\x02ts\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12=\n\x05\x65xtra\x18\t \x03(\x0b\x32..proto_types.AdapterCommonEventInfo.ExtraEntry\x12\x10\n\x08\x63\x61tegory\x18\n \x01(\t\x1a,\n\nExtraEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"]\n\x13\x41\x64\x61pterNodeRelation\x12\x10\n\x08\x64\x61tabase\x18\n \x01(\t\x12\x0e\n\x06schema\x18\x0b \x01(\t\x12\r\n\x05\x61lias\x18\x0c \x01(\t\x12\x15\n\rrelation_name\x18\r \x01(\t\"\x9f\x02\n\x0f\x41\x64\x61pterNodeInfo\x12\x11\n\tnode_path\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x11\n\tunique_id\x18\x03 \x01(\t\x12\x15\n\rresource_type\x18\x04 \x01(\t\x12\x14\n\x0cmaterialized\x18\x05 \x01(\t\x12\x13\n\x0bnode_status\x18\x06 \x01(\t\x12\x17\n\x0fnode_started_at\x18\x07 \x01(\t\x12\x18\n\x10node_finished_at\x18\x08 \x01(\t\x12%\n\x04meta\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x37\n\rnode_relation\x18\n \x01(\x0b\x32 .proto_types.AdapterNodeRelation\"G\n\x0fReferenceKeyMsg\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\"?\n\x19\x41\x64\x61pterDeprecationWarning\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"\x87\x01\n\x1c\x41\x64\x61pterDeprecationWarningMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.AdapterDeprecationWarning\"!\n\x1f\x43ollectFreshnessReturnSignature\"\x93\x01\n\"CollectFreshnessReturnSignatureMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.CollectFreshnessReturnSignature\"\x8e\x01\n\x11\x41\x64\x61pterEventDebug\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"w\n\x14\x41\x64\x61pterEventDebugMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.AdapterEventDebug\"\x8d\x01\n\x10\x41\x64\x61pterEventInfo\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"u\n\x13\x41\x64\x61pterEventInfoMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.AdapterEventInfo\"\x90\x01\n\x13\x41\x64\x61pterEventWarning\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"{\n\x16\x41\x64\x61pterEventWarningMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.AdapterEventWarning\"\xa0\x01\n\x11\x41\x64\x61pterEventError\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x10\n\x08\x65xc_info\x18\x05 \x01(\t\"w\n\x14\x41\x64\x61pterEventErrorMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.AdapterEventError\"f\n\rNewConnection\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x11\n\tconn_type\x18\x02 \x01(\t\x12\x11\n\tconn_name\x18\x03 \x01(\t\"o\n\x10NewConnectionMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NewConnection\"=\n\x10\x43onnectionReused\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x16\n\x0eorig_conn_name\x18\x02 \x01(\t\"u\n\x13\x43onnectionReusedMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConnectionReused\"0\n\x1b\x43onnectionLeftOpenInCleanup\x12\x11\n\tconn_name\x18\x01 \x01(\t\"\x8b\x01\n\x1e\x43onnectionLeftOpenInCleanupMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConnectionLeftOpenInCleanup\".\n\x19\x43onnectionClosedInCleanup\x12\x11\n\tconn_name\x18\x01 \x01(\t\"\x87\x01\n\x1c\x43onnectionClosedInCleanupMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConnectionClosedInCleanup\"f\n\x0eRollbackFailed\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"q\n\x11RollbackFailedMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RollbackFailed\"V\n\x10\x43onnectionClosed\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"u\n\x13\x43onnectionClosedMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConnectionClosed\"X\n\x12\x43onnectionLeftOpen\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"y\n\x15\x43onnectionLeftOpenMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ConnectionLeftOpen\"N\n\x08Rollback\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"e\n\x0bRollbackMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.Rollback\"@\n\tCacheMiss\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\"g\n\x0c\x43\x61\x63heMissMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.CacheMiss\"b\n\rListRelations\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12/\n\trelations\x18\x03 \x03(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"o\n\x10ListRelationsMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.ListRelations\"g\n\x0e\x43onnectionUsed\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x11\n\tconn_type\x18\x02 \x01(\t\x12\x11\n\tconn_name\x18\x03 \x01(\t\"q\n\x11\x43onnectionUsedMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ConnectionUsed\"[\n\x08SQLQuery\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\x12\x0b\n\x03sql\x18\x03 \x01(\t\"e\n\x0bSQLQueryMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.SQLQuery\"b\n\x0eSQLQueryStatus\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x0f\n\x07\x65lapsed\x18\x03 \x01(\x02\"q\n\x11SQLQueryStatusMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.SQLQueryStatus\"O\n\tSQLCommit\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"g\n\x0cSQLCommitMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.SQLCommit\"a\n\rColTypeChange\x12\x11\n\torig_type\x18\x01 \x01(\t\x12\x10\n\x08new_type\x18\x02 \x01(\t\x12+\n\x05table\x18\x03 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"o\n\x10\x43olTypeChangeMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.ColTypeChange\"@\n\x0eSchemaCreation\x12.\n\x08relation\x18\x01 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"q\n\x11SchemaCreationMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.SchemaCreation\"<\n\nSchemaDrop\x12.\n\x08relation\x18\x01 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"i\n\rSchemaDropMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SchemaDrop\"\xde\x01\n\x0b\x43\x61\x63heAction\x12\x0e\n\x06\x61\x63tion\x18\x01 \x01(\t\x12-\n\x07ref_key\x18\x02 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12/\n\tref_key_2\x18\x03 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12/\n\tref_key_3\x18\x04 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12.\n\x08ref_list\x18\x05 \x03(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"k\n\x0e\x43\x61\x63heActionMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.CacheAction\"\x98\x01\n\x0e\x43\x61\x63heDumpGraph\x12\x33\n\x04\x64ump\x18\x01 \x03(\x0b\x32%.proto_types.CacheDumpGraph.DumpEntry\x12\x14\n\x0c\x62\x65\x66ore_after\x18\x02 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x1a+\n\tDumpEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"q\n\x11\x43\x61\x63heDumpGraphMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CacheDumpGraph\"B\n\x11\x41\x64\x61pterRegistered\x12\x14\n\x0c\x61\x64\x61pter_name\x18\x01 \x01(\t\x12\x17\n\x0f\x61\x64\x61pter_version\x18\x02 \x01(\t\"w\n\x14\x41\x64\x61pterRegisteredMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.AdapterRegistered\"!\n\x12\x41\x64\x61pterImportError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"y\n\x15\x41\x64\x61pterImportErrorMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.AdapterImportError\"#\n\x0fPluginLoadError\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"s\n\x12PluginLoadErrorMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.PluginLoadError\"a\n\x14NewConnectionOpening\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x18\n\x10\x63onnection_state\x18\x02 \x01(\t\"}\n\x17NewConnectionOpeningMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NewConnectionOpening\"8\n\rCodeExecution\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x14\n\x0c\x63ode_content\x18\x02 \x01(\t\"o\n\x10\x43odeExecutionMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.CodeExecution\"6\n\x13\x43odeExecutionStatus\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07\x65lapsed\x18\x02 \x01(\x02\"{\n\x16\x43odeExecutionStatusMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.CodeExecutionStatus\"%\n\x16\x43\x61talogGenerationError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"\x81\x01\n\x19\x43\x61talogGenerationErrorMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.CatalogGenerationError\"-\n\x13WriteCatalogFailure\x12\x16\n\x0enum_exceptions\x18\x01 \x01(\x05\"{\n\x16WriteCatalogFailureMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.WriteCatalogFailure\"\x1e\n\x0e\x43\x61talogWritten\x12\x0c\n\x04path\x18\x01 \x01(\t\"q\n\x11\x43\x61talogWrittenMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CatalogWritten\"\x14\n\x12\x43\x61nnotGenerateDocs\"y\n\x15\x43\x61nnotGenerateDocsMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.CannotGenerateDocs\"\x11\n\x0f\x42uildingCatalog\"s\n\x12\x42uildingCatalogMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.BuildingCatalog\"-\n\x18\x44\x61tabaseErrorRunningHook\x12\x11\n\thook_type\x18\x01 \x01(\t\"\x85\x01\n\x1b\x44\x61tabaseErrorRunningHookMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DatabaseErrorRunningHook\"4\n\x0cHooksRunning\x12\x11\n\tnum_hooks\x18\x01 \x01(\x05\x12\x11\n\thook_type\x18\x02 \x01(\t\"m\n\x0fHooksRunningMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.HooksRunning\"T\n\x14\x46inishedRunningStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\x12\x11\n\texecution\x18\x02 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x03 \x01(\x02\"}\n\x17\x46inishedRunningStatsMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.FinishedRunningStats\"<\n\x15\x43onstraintNotEnforced\x12\x12\n\nconstraint\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x61pter\x18\x02 \x01(\t\"\x7f\n\x18\x43onstraintNotEnforcedMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConstraintNotEnforced\"=\n\x16\x43onstraintNotSupported\x12\x12\n\nconstraint\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x61pter\x18\x02 \x01(\t\"\x81\x01\n\x19\x43onstraintNotSupportedMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.ConstraintNotSupportedb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13\x61\x64\x61pter_types.proto\x12\x0bproto_types\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"\xab\x02\n\x16\x41\x64\x61pterCommonEventInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0b\n\x03msg\x18\x03 \x01(\t\x12\r\n\x05level\x18\x04 \x01(\t\x12\x15\n\rinvocation_id\x18\x05 \x01(\t\x12\x0b\n\x03pid\x18\x06 \x01(\x05\x12\x0e\n\x06thread\x18\x07 \x01(\t\x12&\n\x02ts\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12=\n\x05\x65xtra\x18\t \x03(\x0b\x32..proto_types.AdapterCommonEventInfo.ExtraEntry\x12\x10\n\x08\x63\x61tegory\x18\n \x01(\t\x1a,\n\nExtraEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"]\n\x13\x41\x64\x61pterNodeRelation\x12\x10\n\x08\x64\x61tabase\x18\n \x01(\t\x12\x0e\n\x06schema\x18\x0b \x01(\t\x12\r\n\x05\x61lias\x18\x0c \x01(\t\x12\x15\n\rrelation_name\x18\r \x01(\t\"\x9f\x02\n\x0f\x41\x64\x61pterNodeInfo\x12\x11\n\tnode_path\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x11\n\tunique_id\x18\x03 \x01(\t\x12\x15\n\rresource_type\x18\x04 \x01(\t\x12\x14\n\x0cmaterialized\x18\x05 \x01(\t\x12\x13\n\x0bnode_status\x18\x06 \x01(\t\x12\x17\n\x0fnode_started_at\x18\x07 \x01(\t\x12\x18\n\x10node_finished_at\x18\x08 \x01(\t\x12%\n\x04meta\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x37\n\rnode_relation\x18\n \x01(\x0b\x32 .proto_types.AdapterNodeRelation\"G\n\x0fReferenceKeyMsg\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\"?\n\x19\x41\x64\x61pterDeprecationWarning\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"\x87\x01\n\x1c\x41\x64\x61pterDeprecationWarningMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.AdapterDeprecationWarning\"!\n\x1f\x43ollectFreshnessReturnSignature\"\x93\x01\n\"CollectFreshnessReturnSignatureMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.CollectFreshnessReturnSignature\"\x8e\x01\n\x11\x41\x64\x61pterEventDebug\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"w\n\x14\x41\x64\x61pterEventDebugMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.AdapterEventDebug\"\x8d\x01\n\x10\x41\x64\x61pterEventInfo\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"u\n\x13\x41\x64\x61pterEventInfoMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.AdapterEventInfo\"\x90\x01\n\x13\x41\x64\x61pterEventWarning\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"{\n\x16\x41\x64\x61pterEventWarningMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.AdapterEventWarning\"\xa0\x01\n\x11\x41\x64\x61pterEventError\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x10\n\x08\x65xc_info\x18\x05 \x01(\t\"w\n\x14\x41\x64\x61pterEventErrorMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.AdapterEventError\"f\n\rNewConnection\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x11\n\tconn_type\x18\x02 \x01(\t\x12\x11\n\tconn_name\x18\x03 \x01(\t\"o\n\x10NewConnectionMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NewConnection\"=\n\x10\x43onnectionReused\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x16\n\x0eorig_conn_name\x18\x02 \x01(\t\"u\n\x13\x43onnectionReusedMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConnectionReused\"0\n\x1b\x43onnectionLeftOpenInCleanup\x12\x11\n\tconn_name\x18\x01 \x01(\t\"\x8b\x01\n\x1e\x43onnectionLeftOpenInCleanupMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConnectionLeftOpenInCleanup\".\n\x19\x43onnectionClosedInCleanup\x12\x11\n\tconn_name\x18\x01 \x01(\t\"\x87\x01\n\x1c\x43onnectionClosedInCleanupMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConnectionClosedInCleanup\"f\n\x0eRollbackFailed\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"q\n\x11RollbackFailedMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RollbackFailed\"V\n\x10\x43onnectionClosed\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"u\n\x13\x43onnectionClosedMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConnectionClosed\"X\n\x12\x43onnectionLeftOpen\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"y\n\x15\x43onnectionLeftOpenMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ConnectionLeftOpen\"N\n\x08Rollback\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"e\n\x0bRollbackMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.Rollback\"@\n\tCacheMiss\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\"g\n\x0c\x43\x61\x63heMissMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.CacheMiss\"b\n\rListRelations\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12/\n\trelations\x18\x03 \x03(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"o\n\x10ListRelationsMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.ListRelations\"g\n\x0e\x43onnectionUsed\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x11\n\tconn_type\x18\x02 \x01(\t\x12\x11\n\tconn_name\x18\x03 \x01(\t\"q\n\x11\x43onnectionUsedMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ConnectionUsed\"[\n\x08SQLQuery\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\x12\x0b\n\x03sql\x18\x03 \x01(\t\"e\n\x0bSQLQueryMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.SQLQuery\"b\n\x0eSQLQueryStatus\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x0f\n\x07\x65lapsed\x18\x03 \x01(\x02\"q\n\x11SQLQueryStatusMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.SQLQueryStatus\"O\n\tSQLCommit\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"g\n\x0cSQLCommitMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.SQLCommit\"a\n\rColTypeChange\x12\x11\n\torig_type\x18\x01 \x01(\t\x12\x10\n\x08new_type\x18\x02 \x01(\t\x12+\n\x05table\x18\x03 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"o\n\x10\x43olTypeChangeMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.ColTypeChange\"@\n\x0eSchemaCreation\x12.\n\x08relation\x18\x01 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"q\n\x11SchemaCreationMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.SchemaCreation\"<\n\nSchemaDrop\x12.\n\x08relation\x18\x01 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"i\n\rSchemaDropMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SchemaDrop\"\xde\x01\n\x0b\x43\x61\x63heAction\x12\x0e\n\x06\x61\x63tion\x18\x01 \x01(\t\x12-\n\x07ref_key\x18\x02 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12/\n\tref_key_2\x18\x03 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12/\n\tref_key_3\x18\x04 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12.\n\x08ref_list\x18\x05 \x03(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"k\n\x0e\x43\x61\x63heActionMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.CacheAction\"\x98\x01\n\x0e\x43\x61\x63heDumpGraph\x12\x33\n\x04\x64ump\x18\x01 \x03(\x0b\x32%.proto_types.CacheDumpGraph.DumpEntry\x12\x14\n\x0c\x62\x65\x66ore_after\x18\x02 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x1a+\n\tDumpEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"q\n\x11\x43\x61\x63heDumpGraphMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CacheDumpGraph\"B\n\x11\x41\x64\x61pterRegistered\x12\x14\n\x0c\x61\x64\x61pter_name\x18\x01 \x01(\t\x12\x17\n\x0f\x61\x64\x61pter_version\x18\x02 \x01(\t\"w\n\x14\x41\x64\x61pterRegisteredMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.AdapterRegistered\"!\n\x12\x41\x64\x61pterImportError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"y\n\x15\x41\x64\x61pterImportErrorMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.AdapterImportError\"#\n\x0fPluginLoadError\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"s\n\x12PluginLoadErrorMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.PluginLoadError\"a\n\x14NewConnectionOpening\x12/\n\tnode_info\x18\x01 \x01(\x0b\x32\x1c.proto_types.AdapterNodeInfo\x12\x18\n\x10\x63onnection_state\x18\x02 \x01(\t\"}\n\x17NewConnectionOpeningMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NewConnectionOpening\"8\n\rCodeExecution\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x14\n\x0c\x63ode_content\x18\x02 \x01(\t\"o\n\x10\x43odeExecutionMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.CodeExecution\"6\n\x13\x43odeExecutionStatus\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07\x65lapsed\x18\x02 \x01(\x02\"{\n\x16\x43odeExecutionStatusMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.CodeExecutionStatus\"%\n\x16\x43\x61talogGenerationError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"\x81\x01\n\x19\x43\x61talogGenerationErrorMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.CatalogGenerationError\"-\n\x13WriteCatalogFailure\x12\x16\n\x0enum_exceptions\x18\x01 \x01(\x05\"{\n\x16WriteCatalogFailureMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.WriteCatalogFailure\"\x1e\n\x0e\x43\x61talogWritten\x12\x0c\n\x04path\x18\x01 \x01(\t\"q\n\x11\x43\x61talogWrittenMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CatalogWritten\"\x14\n\x12\x43\x61nnotGenerateDocs\"y\n\x15\x43\x61nnotGenerateDocsMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.CannotGenerateDocs\"\x11\n\x0f\x42uildingCatalog\"s\n\x12\x42uildingCatalogMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.BuildingCatalog\"-\n\x18\x44\x61tabaseErrorRunningHook\x12\x11\n\thook_type\x18\x01 \x01(\t\"\x85\x01\n\x1b\x44\x61tabaseErrorRunningHookMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DatabaseErrorRunningHook\"4\n\x0cHooksRunning\x12\x11\n\tnum_hooks\x18\x01 \x01(\x05\x12\x11\n\thook_type\x18\x02 \x01(\t\"m\n\x0fHooksRunningMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.HooksRunning\"T\n\x14\x46inishedRunningStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\x12\x11\n\texecution\x18\x02 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x03 \x01(\x02\"}\n\x17\x46inishedRunningStatsMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.FinishedRunningStats\"<\n\x15\x43onstraintNotEnforced\x12\x12\n\nconstraint\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x61pter\x18\x02 \x01(\t\"\x7f\n\x18\x43onstraintNotEnforcedMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConstraintNotEnforced\"=\n\x16\x43onstraintNotSupported\x12\x12\n\nconstraint\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x61pter\x18\x02 \x01(\t\"\x81\x01\n\x19\x43onstraintNotSupportedMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.ConstraintNotSupported\"%\n\x10TypeCodeNotFound\x12\x11\n\ttype_code\x18\x01 \x01(\x05\"u\n\x13TypeCodeNotFoundMsg\x12\x31\n\x04info\x18\x01 \x01(\x0b\x32#.proto_types.AdapterCommonEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.TypeCodeNotFoundb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'adapter_types_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_ADAPTERCOMMONEVENTINFO_EXTRAENTRY']._options = None
@@ -199,8 +198,12 @@
   _globals['_CONSTRAINTNOTENFORCED']._serialized_end=8769
   _globals['_CONSTRAINTNOTENFORCEDMSG']._serialized_start=8771
   _globals['_CONSTRAINTNOTENFORCEDMSG']._serialized_end=8898
   _globals['_CONSTRAINTNOTSUPPORTED']._serialized_start=8900
   _globals['_CONSTRAINTNOTSUPPORTED']._serialized_end=8961
   _globals['_CONSTRAINTNOTSUPPORTEDMSG']._serialized_start=8964
   _globals['_CONSTRAINTNOTSUPPORTEDMSG']._serialized_end=9093
+  _globals['_TYPECODENOTFOUND']._serialized_start=9095
+  _globals['_TYPECODENOTFOUND']._serialized_end=9132
+  _globals['_TYPECODENOTFOUNDMSG']._serialized_start=9134
+  _globals['_TYPECODENOTFOUNDMSG']._serialized_end=9251
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/events/base_types.py` & `dbt_adapters-1.0.8b3/dbt/adapters/events/base_types.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/events/logging.py` & `dbt_adapters-1.0.8b3/dbt/adapters/events/logging.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/events/types.py` & `dbt_adapters-1.0.8b3/dbt/adapters/events/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dbt_common.ui import line_wrap_message, warning_tag
 
 from dbt.adapters.events.base_types import (
     DebugLevel,
+    DynamicLevel,
     ErrorLevel,
     InfoLevel,
     WarnLevel,
 )
 
 
 def format_adapter_message(name, base_msg, args) -> str:
@@ -277,15 +278,15 @@
     def message(self) -> str:
         return f"dump {self.before_after} {self.action} : {self.dump}"
 
 
 # Skipping E032, E033, E034
 
 
-class AdapterRegistered(InfoLevel):
+class AdapterRegistered(DynamicLevel):
     def code(self) -> str:
         return "E034"
 
     def message(self) -> str:
         return f"Registered adapter: {self.adapter_name}{self.adapter_version}"
 
 
@@ -417,7 +418,20 @@
 
     def message(self) -> str:
         msg = (
             f"The constraint type {self.constraint} is not supported by {self.adapter}, and will "
             "be ignored. Set 'warn_unsupported: false' on this constraint to ignore this warning."
         )
         return line_wrap_message(warning_tag(msg))
+
+
+class TypeCodeNotFound(DebugLevel):
+    def code(self) -> str:
+        return "E050"
+
+    def message(self) -> str:
+        msg = (
+            f"The `type_code` {self.type_code} was not recognized, which may affect error "
+            "messages for enforced contracts that fail as well as `Column.data_type` values "
+            "returned by `get_column_schema_from_query`"
+        )
+        return line_wrap_message(warning_tag(msg))
```

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/exceptions/__init__.py` & `dbt_adapters-1.0.8b3/dbt/adapters/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/exceptions/alias.py` & `dbt_adapters-1.0.8b3/dbt/adapters/exceptions/alias.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/exceptions/cache.py` & `dbt_adapters-1.0.8b3/dbt/adapters/exceptions/cache.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/exceptions/compilation.py` & `dbt_adapters-1.0.8b3/dbt/adapters/exceptions/compilation.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/exceptions/database.py` & `dbt_adapters-1.0.8b3/dbt/adapters/exceptions/database.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/relation_configs/README.md` & `dbt_adapters-1.0.8b3/dbt/adapters/relation_configs/README.md`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/relation_configs/config_base.py` & `dbt_adapters-1.0.8b3/dbt/adapters/relation_configs/config_base.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/relation_configs/config_change.py` & `dbt_adapters-1.0.8b3/dbt/adapters/relation_configs/config_change.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/relation_configs/config_validation.py` & `dbt_adapters-1.0.8b3/dbt/adapters/relation_configs/config_validation.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/sql/connections.py` & `dbt_adapters-1.0.8b3/dbt/adapters/sql/connections.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/adapters/sql/impl.py` & `dbt_adapters-1.0.8b3/dbt/adapters/sql/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/docs/overview.md` & `dbt_adapters-1.0.8b3/dbt/include/global_project/docs/overview.md`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/apply_grants.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/columns.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/freshness.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/adapters/freshness.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/indexes.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/metadata.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/persist_docs.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/relation.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/schema.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/show.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/adapters/show.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/timestamps.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/adapters/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/etc/datetime.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/etc/datetime.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/etc/statement.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/etc/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/configs.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/configs.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/hooks.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/hooks.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/materialized_view.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/models/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/table.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/models/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/view.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/models/view.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/clone/clone.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/models/clone/clone.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/incremental/merge.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/seeds/helpers.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/seeds/seed.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/seeds/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/snapshots/helpers.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/snapshots/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/snapshots/strategies.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/snapshots/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/tests/helpers.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/tests/test.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/tests/test.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/tests/unit.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/materializations/tests/unit.sql`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 {%- materialization unit, default -%}
 
   {% set relations = [] %}
 
   {% set expected_rows = config.get('expected_rows') %}
+  {% set expected_sql = config.get('expected_sql') %}
   {% set tested_expected_column_names = expected_rows[0].keys() if (expected_rows | length ) > 0 else get_columns_in_query(sql) %} %}
 
   {%- set target_relation = this.incorporate(type='table') -%}
   {%- set temp_relation = make_temp_relation(target_relation)-%}
   {% do run_query(get_create_table_as_sql(True, temp_relation, get_empty_subquery_sql(sql))) %}
   {%- set columns_in_relation = adapter.get_columns_in_relation(temp_relation) -%}
   {%- set column_name_to_data_types = {} -%}
   {%- for column in columns_in_relation -%}
-  {%- do column_name_to_data_types.update({column.name|lower: column.data_type}) -%}
+  {%-   do column_name_to_data_types.update({column.name|lower: column.data_type}) -%}
   {%- endfor -%}
 
-  {% set unit_test_sql = get_unit_test_sql(sql, get_expected_sql(expected_rows, column_name_to_data_types), tested_expected_column_names) %}
+  {% if not expected_sql %}
+  {%   set expected_sql = get_expected_sql(expected_rows, column_name_to_data_types) %}
+  {% endif %}
+  {% set unit_test_sql = get_unit_test_sql(sql, expected_sql, tested_expected_column_names) %}
 
   {% call statement('main', fetch_result=True) -%}
 
     {{ unit_test_sql }}
 
   {%- endcall %}
```

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/python_model/python.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/python_model/python.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/create.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/create.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/create_backup.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/create_backup.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/create_intermediate.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/create_intermediate.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/drop.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/drop.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/rename.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/rename.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/replace.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/column/columns_spec_ddl.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/column/columns_spec_ddl.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/materialized_view/alter.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/materialized_view/alter.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/materialized_view/drop.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/materialized_view/drop.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/table/create.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/table/create.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/view/create.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/view/create.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/view/replace.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/relations/view/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/unit_test_sql/get_fixture_sql.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/unit_test_sql/get_fixture_sql.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/data_types.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/data_types.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/date_spine.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/date_spine.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/generate_series.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/generate_series.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/listagg.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/split_part.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/dbt/include/global_project/tests/generic/builtin.sql` & `dbt_adapters-1.0.8b3/dbt/include/global_project/tests/generic/builtin.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/.gitignore` & `dbt_adapters-1.0.8b3/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/LICENSE` & `dbt_adapters-1.0.8b3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/README.md` & `dbt_adapters-1.0.8b3/README.md`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b2/pyproject.toml` & `dbt_adapters-1.0.8b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 dependencies = [
     "dbt_common @ git+https://github.com/dbt-labs/dbt-common.git",
 ]
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
-    "black",
+    "black>=24.3",
     "flake8",
     "Flake8-pyproject",
 ]
 [tool.hatch.envs.lint.scripts]
 all = [
     "- black-only",
     "- flake8-only",
```

### Comparing `dbt_adapters-1.0.0b2/PKG-INFO` & `dbt_adapters-1.0.8b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dbt-adapters
-Version: 1.0.0b2
+Version: 1.0.8b3
 Summary: The set of adapter protocols and base functionality that supports integration with dbt-core
 Project-URL: Homepage, https://github.com/dbt-labs/dbt-adapters
 Project-URL: Documentation, https://docs.getdbt.com
 Project-URL: Repository, https://github.com/dbt-labs/dbt-adapters.git
 Project-URL: Issues, https://github.com/dbt-labs/dbt-adapters/issues
 Project-URL: Changelog, https://github.com/dbt-labs/dbt-adapters/blob/main/CHANGELOG.md
 Author-email: dbt Labs <info@dbtlabs.com>
```

