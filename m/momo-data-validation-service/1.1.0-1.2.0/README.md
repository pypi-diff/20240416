# Comparing `tmp/momo-data-validation-service-1.1.0.tar.gz` & `tmp/momo_data_validation_service-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momo-data-validation-service-1.1.0.tar", last modified: Thu Apr 11 01:04:47 2024, max compression
+gzip compressed data, was "momo_data_validation_service-1.2.0.tar", last modified: Tue Apr 16 09:28:25 2024, max compression
```

## Comparing `momo-data-validation-service-1.1.0.tar` & `momo_data_validation_service-1.2.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.021191 momo-data-validation-service-1.1.0/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    11358 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/LICENSE
--rw-r--r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    45975 2024-04-11 01:04:47.021191 momo-data-validation-service-1.1.0/PKG-INFO
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    44079 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/README.md
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.001188 momo-data-validation-service-1.1.0/data_validation/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      718 2024-04-11 00:51:14.000000 momo-data-validation-service-1.1.0/data_validation/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    26509 2024-04-09 07:00:39.000000 momo-data-validation-service-1.1.0/data_validation/__main__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1986 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/app.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    48902 2024-04-03 08:52:32.000000 momo-data-validation-service-1.1.0/data_validation/cli_tools.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      881 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/client_info.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    10055 2024-04-03 08:53:31.000000 momo-data-validation-service-1.1.0/data_validation/clients.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    14254 2024-04-05 09:03:48.000000 momo-data-validation-service-1.1.0/data_validation/combiner.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    40169 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/config_manager.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     5244 2024-04-11 00:51:19.000000 momo-data-validation-service-1.1.0/data_validation/consts.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    14688 2024-04-05 04:52:49.000000 momo-data-validation-service-1.1.0/data_validation/data_validation.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      687 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/exceptions.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1269 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/jellyfish_distance.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2521 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/metadata.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    16257 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/partition_builder.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.001188 momo-data-validation-service-1.1.0/data_validation/query_builder/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      575 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/query_builder/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2583 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/query_builder/partition_row_builder.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    19246 2024-04-05 09:03:17.000000 momo-data-validation-service-1.1.0/data_validation/query_builder/query_builder.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     3710 2024-03-27 04:01:18.000000 momo-data-validation-service-1.1.0/data_validation/query_builder/random_row_builder.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.001188 momo-data-validation-service-1.1.0/data_validation/result_handlers/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/result_handlers/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     3970 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/result_handlers/bigquery.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2526 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/result_handlers/text.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    14320 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/schema_validation.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1773 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/secret_manager.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    10173 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/state_manager.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    16109 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/validation_builder.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.021191 momo-data-validation-service-1.1.0/momo_data_validation_service.egg-info/
--rw-r--r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    45975 2024-04-11 01:04:46.000000 momo-data-validation-service-1.1.0/momo_data_validation_service.egg-info/PKG-INFO
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     3288 2024-04-11 01:04:46.000000 momo-data-validation-service-1.1.0/momo_data_validation_service.egg-info/SOURCES.txt
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        1 2024-04-11 01:04:46.000000 momo-data-validation-service-1.1.0/momo_data_validation_service.egg-info/dependency_links.txt
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)       66 2024-04-11 01:04:46.000000 momo-data-validation-service-1.1.0/momo_data_validation_service.egg-info/entry_points.txt
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      620 2024-04-11 01:04:46.000000 momo-data-validation-service-1.1.0/momo_data_validation_service.egg-info/requires.txt
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)       28 2024-04-11 01:04:46.000000 momo-data-validation-service-1.1.0/momo_data_validation_service.egg-info/top_level.txt
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)       67 2024-04-11 01:04:47.025191 momo-data-validation-service-1.1.0/setup.cfg
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     3036 2024-04-11 01:03:30.000000 momo-data-validation-service-1.1.0/setup.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:46.993187 momo-data-validation-service-1.1.0/third_party/
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:46.997187 momo-data-validation-service-1.1.0/third_party/ibis/
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.017190 momo-data-validation-service-1.1.0/third_party/ibis/ibis_addon/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_addon/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2515 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_addon/api.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    20735 2024-04-10 03:40:35.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_addon/operations.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.017190 momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     6916 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1378 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/api.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      934 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/client.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2748 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/compiler.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1517 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/datatypes.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2300 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/registry.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.017190 momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/tests/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        1 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/tests/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     4999 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1292 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.017190 momo-data-validation-service-1.1.0/third_party/ibis/ibis_db2/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2649 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_db2/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1264 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_db2/api.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1024 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_db2/compiler.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1492 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_db2/datatypes.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    15919 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_db2/registry.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.017190 momo-data-validation-service-1.1.0/third_party/ibis/ibis_impala/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_impala/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     7187 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_impala/api.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.017190 momo-data-validation-service-1.1.0/third_party/ibis/ibis_mssql/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2987 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_mssql/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1237 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_mssql/api.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1315 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_mssql/datatypes.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.017190 momo-data-validation-service-1.1.0/third_party/ibis/ibis_mysql/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_mysql/__init__.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.017190 momo-data-validation-service-1.1.0/third_party/ibis/ibis_mysql/base_sql_compiler/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_mysql/base_sql_compiler/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     4596 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_mysql/base_sql_compiler/select_builder.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1509 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_mysql/compiler.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.017190 momo-data-validation-service-1.1.0/third_party/ibis/ibis_oracle/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     3043 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_oracle/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1228 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_oracle/api.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1085 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_oracle/compiler.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     6593 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_oracle/datatypes.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    14411 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_oracle/registry.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.021191 momo-data-validation-service-1.1.0/third_party/ibis/ibis_postgres/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      101 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_postgres/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     4126 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_postgres/client.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      839 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_postgres/datatypes.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.021191 momo-data-validation-service-1.1.0/third_party/ibis/ibis_redshift/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     4053 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_redshift/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1170 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_redshift/api.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1543 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_redshift/compiler.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.021191 momo-data-validation-service-1.1.0/third_party/ibis/ibis_snowflake/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_snowflake/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1148 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_snowflake/api.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1986 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_snowflake/datatypes.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.021191 momo-data-validation-service-1.1.0/third_party/ibis/ibis_teradata/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     9164 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_teradata/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1210 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_teradata/api.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1810 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_teradata/compiler.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     7034 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_teradata/datatypes.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     8568 2024-03-27 04:03:19.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_teradata/registry.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.021191 momo-data-validation-service-1.1.0/third_party/ibis/ibis_trino/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)       92 2024-04-02 06:55:24.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_trino/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2288 2024-04-10 03:08:36.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_trino/compiler.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      891 2024-04-03 07:43:34.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_trino/datatypes.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-16 09:28:25.549204 momo_data_validation_service-1.2.0/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    11358 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/LICENSE
+-rw-r--r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    45975 2024-04-16 09:28:25.549204 momo_data_validation_service-1.2.0/PKG-INFO
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    44079 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/README.md
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-16 09:28:25.505204 momo_data_validation_service-1.2.0/data_validation/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      718 2024-04-11 00:51:14.000000 momo_data_validation_service-1.2.0/data_validation/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    26509 2024-04-09 07:00:39.000000 momo_data_validation_service-1.2.0/data_validation/__main__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1986 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/data_validation/app.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    48902 2024-04-03 08:52:32.000000 momo_data_validation_service-1.2.0/data_validation/cli_tools.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      881 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/data_validation/client_info.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    10055 2024-04-03 08:53:31.000000 momo_data_validation_service-1.2.0/data_validation/clients.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    14254 2024-04-05 09:03:48.000000 momo_data_validation_service-1.2.0/data_validation/combiner.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    40169 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/data_validation/config_manager.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     5244 2024-04-11 00:51:19.000000 momo_data_validation_service-1.2.0/data_validation/consts.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    14688 2024-04-16 07:30:23.000000 momo_data_validation_service-1.2.0/data_validation/data_validation.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      687 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/data_validation/exceptions.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1269 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/data_validation/jellyfish_distance.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2521 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/data_validation/metadata.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    16257 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/data_validation/partition_builder.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-16 09:28:25.509204 momo_data_validation_service-1.2.0/data_validation/query_builder/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      575 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/data_validation/query_builder/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2583 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/data_validation/query_builder/partition_row_builder.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    19246 2024-04-05 09:03:17.000000 momo_data_validation_service-1.2.0/data_validation/query_builder/query_builder.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     3710 2024-03-27 04:01:18.000000 momo_data_validation_service-1.2.0/data_validation/query_builder/random_row_builder.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-16 09:28:25.509204 momo_data_validation_service-1.2.0/data_validation/result_handlers/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/data_validation/result_handlers/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     3970 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/data_validation/result_handlers/bigquery.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2526 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/data_validation/result_handlers/text.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    14320 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/data_validation/schema_validation.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1773 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/data_validation/secret_manager.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    10173 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/data_validation/state_manager.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    16109 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/data_validation/validation_builder.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-16 09:28:25.545204 momo_data_validation_service-1.2.0/momo_data_validation_service.egg-info/
+-rw-r--r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    45975 2024-04-16 09:28:25.000000 momo_data_validation_service-1.2.0/momo_data_validation_service.egg-info/PKG-INFO
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     3288 2024-04-16 09:28:25.000000 momo_data_validation_service-1.2.0/momo_data_validation_service.egg-info/SOURCES.txt
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        1 2024-04-16 09:28:25.000000 momo_data_validation_service-1.2.0/momo_data_validation_service.egg-info/dependency_links.txt
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)       66 2024-04-16 09:28:25.000000 momo_data_validation_service-1.2.0/momo_data_validation_service.egg-info/entry_points.txt
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      620 2024-04-16 09:28:25.000000 momo_data_validation_service-1.2.0/momo_data_validation_service.egg-info/requires.txt
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)       28 2024-04-16 09:28:25.000000 momo_data_validation_service-1.2.0/momo_data_validation_service.egg-info/top_level.txt
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)       67 2024-04-16 09:28:25.569204 momo_data_validation_service-1.2.0/setup.cfg
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     3036 2024-04-16 09:26:57.000000 momo_data_validation_service-1.2.0/setup.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-16 09:28:25.497204 momo_data_validation_service-1.2.0/third_party/
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-16 09:28:25.497204 momo_data_validation_service-1.2.0/third_party/ibis/
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-16 09:28:25.541204 momo_data_validation_service-1.2.0/third_party/ibis/ibis_addon/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_addon/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2515 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_addon/api.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    21342 2024-04-16 06:57:03.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_addon/operations.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-16 09:28:25.541204 momo_data_validation_service-1.2.0/third_party/ibis/ibis_cloud_spanner/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     6916 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_cloud_spanner/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1378 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_cloud_spanner/api.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      934 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_cloud_spanner/client.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2748 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_cloud_spanner/compiler.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1517 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_cloud_spanner/datatypes.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2300 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_cloud_spanner/registry.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-16 09:28:25.541204 momo_data_validation_service-1.2.0/third_party/ibis/ibis_cloud_spanner/tests/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        1 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_cloud_spanner/tests/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     4999 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1292 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-16 09:28:25.541204 momo_data_validation_service-1.2.0/third_party/ibis/ibis_db2/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2649 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_db2/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1264 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_db2/api.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1024 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_db2/compiler.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1492 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_db2/datatypes.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    15919 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_db2/registry.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-16 09:28:25.541204 momo_data_validation_service-1.2.0/third_party/ibis/ibis_impala/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_impala/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     7187 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_impala/api.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-16 09:28:25.541204 momo_data_validation_service-1.2.0/third_party/ibis/ibis_mssql/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2987 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_mssql/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1237 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_mssql/api.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1315 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_mssql/datatypes.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-16 09:28:25.541204 momo_data_validation_service-1.2.0/third_party/ibis/ibis_mysql/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_mysql/__init__.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-16 09:28:25.545204 momo_data_validation_service-1.2.0/third_party/ibis/ibis_mysql/base_sql_compiler/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_mysql/base_sql_compiler/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     4596 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_mysql/base_sql_compiler/select_builder.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1509 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_mysql/compiler.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-16 09:28:25.545204 momo_data_validation_service-1.2.0/third_party/ibis/ibis_oracle/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     3043 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_oracle/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1228 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_oracle/api.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1085 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_oracle/compiler.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     6593 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_oracle/datatypes.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    14411 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_oracle/registry.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-16 09:28:25.545204 momo_data_validation_service-1.2.0/third_party/ibis/ibis_postgres/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      101 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_postgres/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     4126 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_postgres/client.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      839 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_postgres/datatypes.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-16 09:28:25.545204 momo_data_validation_service-1.2.0/third_party/ibis/ibis_redshift/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     4053 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_redshift/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1170 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_redshift/api.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1543 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_redshift/compiler.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-16 09:28:25.545204 momo_data_validation_service-1.2.0/third_party/ibis/ibis_snowflake/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_snowflake/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1148 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_snowflake/api.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1986 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_snowflake/datatypes.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-16 09:28:25.545204 momo_data_validation_service-1.2.0/third_party/ibis/ibis_teradata/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     9164 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_teradata/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1210 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_teradata/api.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1810 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_teradata/compiler.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     7034 2024-03-20 09:17:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_teradata/datatypes.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     8568 2024-03-27 04:03:19.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_teradata/registry.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-16 09:28:25.545204 momo_data_validation_service-1.2.0/third_party/ibis/ibis_trino/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)       97 2024-04-16 09:25:29.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_trino/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      936 2024-04-16 09:25:53.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_trino/datatypes.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      365 2024-04-16 08:03:30.000000 momo_data_validation_service-1.2.0/third_party/ibis/ibis_trino/registry.py
```

### Comparing `momo-data-validation-service-1.1.0/LICENSE` & `momo_data_validation_service-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/PKG-INFO` & `momo_data_validation_service-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momo-data-validation-service
-Version: 1.1.0
+Version: 1.2.0
 Summary: A package to enable easy data validation
 Home-page: https://glab.mservice.io/ai-data-platform/uncategorized-projects/professional-services-data-validator
 Author: Nguyen Thuy Dung
 Author-email: dung.nguyen24@mservice.com.vn
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs==23.1.0
-Requires-Dist: grpcio==1.53.0
+Requires-Dist: grpcio==1.62.1
 Requires-Dist: lazy-object-proxy==1.9.0
 Requires-Dist: marshmallow==3.19.0
 Requires-Dist: fsspec>=2022.8.2
 Requires-Dist: google-api-python-client==2.91.0
 Requires-Dist: ibis-framework==5.1.0
 Requires-Dist: impyla==0.18.0
 Requires-Dist: SQLAlchemy==1.4.49
```

### Comparing `momo-data-validation-service-1.1.0/README.md` & `momo_data_validation_service-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/__init__.py` & `momo_data_validation_service-1.2.0/data_validation/__init__.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/__main__.py` & `momo_data_validation_service-1.2.0/data_validation/__main__.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/app.py` & `momo_data_validation_service-1.2.0/data_validation/app.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/cli_tools.py` & `momo_data_validation_service-1.2.0/data_validation/cli_tools.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/client_info.py` & `momo_data_validation_service-1.2.0/data_validation/client_info.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/clients.py` & `momo_data_validation_service-1.2.0/data_validation/clients.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/combiner.py` & `momo_data_validation_service-1.2.0/data_validation/combiner.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/config_manager.py` & `momo_data_validation_service-1.2.0/data_validation/config_manager.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/consts.py` & `momo_data_validation_service-1.2.0/data_validation/consts.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/data_validation.py` & `momo_data_validation_service-1.2.0/data_validation/data_validation.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/exceptions.py` & `momo_data_validation_service-1.2.0/data_validation/exceptions.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/jellyfish_distance.py` & `momo_data_validation_service-1.2.0/data_validation/jellyfish_distance.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/metadata.py` & `momo_data_validation_service-1.2.0/data_validation/metadata.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/partition_builder.py` & `momo_data_validation_service-1.2.0/data_validation/partition_builder.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/query_builder/__init__.py` & `momo_data_validation_service-1.2.0/data_validation/query_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/query_builder/partition_row_builder.py` & `momo_data_validation_service-1.2.0/data_validation/query_builder/partition_row_builder.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/query_builder/query_builder.py` & `momo_data_validation_service-1.2.0/data_validation/query_builder/query_builder.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/query_builder/random_row_builder.py` & `momo_data_validation_service-1.2.0/data_validation/query_builder/random_row_builder.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/result_handlers/bigquery.py` & `momo_data_validation_service-1.2.0/data_validation/result_handlers/bigquery.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/result_handlers/text.py` & `momo_data_validation_service-1.2.0/data_validation/result_handlers/text.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/schema_validation.py` & `momo_data_validation_service-1.2.0/data_validation/schema_validation.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/secret_manager.py` & `momo_data_validation_service-1.2.0/data_validation/secret_manager.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/state_manager.py` & `momo_data_validation_service-1.2.0/data_validation/state_manager.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/data_validation/validation_builder.py` & `momo_data_validation_service-1.2.0/data_validation/validation_builder.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/momo_data_validation_service.egg-info/PKG-INFO` & `momo_data_validation_service-1.2.0/momo_data_validation_service.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momo-data-validation-service
-Version: 1.1.0
+Version: 1.2.0
 Summary: A package to enable easy data validation
 Home-page: https://glab.mservice.io/ai-data-platform/uncategorized-projects/professional-services-data-validator
 Author: Nguyen Thuy Dung
 Author-email: dung.nguyen24@mservice.com.vn
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs==23.1.0
-Requires-Dist: grpcio==1.53.0
+Requires-Dist: grpcio==1.62.1
 Requires-Dist: lazy-object-proxy==1.9.0
 Requires-Dist: marshmallow==3.19.0
 Requires-Dist: fsspec>=2022.8.2
 Requires-Dist: google-api-python-client==2.91.0
 Requires-Dist: ibis-framework==5.1.0
 Requires-Dist: impyla==0.18.0
 Requires-Dist: SQLAlchemy==1.4.49
```

### Comparing `momo-data-validation-service-1.1.0/momo_data_validation_service.egg-info/SOURCES.txt` & `momo_data_validation_service-1.2.0/momo_data_validation_service.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -75,9 +75,9 @@
 third_party/ibis/ibis_snowflake/datatypes.py
 third_party/ibis/ibis_teradata/__init__.py
 third_party/ibis/ibis_teradata/api.py
 third_party/ibis/ibis_teradata/compiler.py
 third_party/ibis/ibis_teradata/datatypes.py
 third_party/ibis/ibis_teradata/registry.py
 third_party/ibis/ibis_trino/__init__.py
-third_party/ibis/ibis_trino/compiler.py
-third_party/ibis/ibis_trino/datatypes.py
+third_party/ibis/ibis_trino/datatypes.py
+third_party/ibis/ibis_trino/registry.py
```

### Comparing `momo-data-validation-service-1.1.0/momo_data_validation_service.egg-info/requires.txt` & `momo_data_validation_service-1.2.0/momo_data_validation_service.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 attrs==23.1.0
-grpcio==1.53.0
+grpcio==1.62.1
 lazy-object-proxy==1.9.0
 marshmallow==3.19.0
 fsspec>=2022.8.2
 google-api-python-client==2.91.0
 ibis-framework==5.1.0
 impyla==0.18.0
 SQLAlchemy==1.4.49
```

### Comparing `momo-data-validation-service-1.1.0/setup.py` & `momo_data_validation_service-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 
 import os
 
 import setuptools
 
 name = "momo-data-validation-service"
 description = "A package to enable easy data validation"
-version = "1.1.0"
+version = "1.2.0"
 release_status = "Development Status :: 3 - Alpha"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 dependencies = [
     # Dependency corrections from our requirements
     "attrs==23.1.0",
-#     "grpcio==1.62.1",
-    "grpcio==1.53.0",
+    "grpcio==1.62.1",
+    # "grpcio==1.53.0",
     "lazy-object-proxy==1.9.0",
     "marshmallow==3.19.0",
     # Core dependencies
     "fsspec>=2022.8.2",
     "google-api-python-client==2.91.0",
     "ibis-framework==5.1.0",
     "impyla==0.18.0",
```

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_addon/api.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_addon/api.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_addon/operations.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_addon/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 from ibis.backends.impala.compiler import ImpalaExprTranslator
 from ibis.backends.mssql.compiler import MsSqlExprTranslator
 from ibis.backends.mysql.compiler import MySQLExprTranslator
 from ibis.backends.pandas.dispatch import execute_node
 from ibis.backends.pandas.execution.temporal import execute_epoch_seconds
 from ibis.backends.postgres.compiler import PostgreSQLExprTranslator
 from ibis.backends.trino.compiler import TrinoSQLExprTranslator
-# import third_party.ibis.ibis_trino.compiler
 from ibis.expr.operations import (
     Cast,
     Comparison,
     ExtractEpochSeconds,
     HashBytes,
     IfNull,
     RandomScalar,
@@ -146,14 +145,21 @@
 def format_hashbytes_trino(translator, op):
     arg = translator.translate(op.arg)
     if op.how == "sha256":
         return f"LOWER(TO_HEX(SHA256(TO_UTF8({arg})))) AS `hash__all`"
     else:
         raise ValueError(f"unexpected value for 'how': {op.how}")
 
+def sa_format_hashbytes_trino(translator, op):
+    arg = translator.translate(op.arg)
+    convert = sa.func.to_utf8(arg)
+    hash_func = sa.func.sha256(convert)
+    hex = sa.func.to_hex(hash_func)
+    return sa.func.lower(hex)
+
 
 def format_hashbytes_teradata(translator, op):
     arg = translator.translate(op.arg)
     if op.how == "sha256":
         return f"rtrim(hash_sha256({arg}))"
     elif op.how == "sha512":
         return f"rtrim(hash_sha512({arg}))"
@@ -191,14 +197,25 @@
     arg_type = arg.output_dtype
     fmt_string = translator.translate(format_string)
     if isinstance(arg_type, dt.Timestamp):
         fmt_string = "%Y-%m-%d %H:%i:%S"
     return sa.func.date_format(arg_formatted, fmt_string)
 
 
+def strftime_trino(translator, op):
+    arg = op.arg
+    format_string = op.format_str
+    arg_formatted = translator.translate(arg)
+    arg_type = arg.output_dtype
+    fmt_string = translator.translate(format_string)
+    if isinstance(arg_type, dt.Timestamp):
+        fmt_string = "%Y-%m-%d %H:%i:%S"
+    return sa.func.date_format(arg_formatted, fmt_string)
+
+
 def strftime_mssql(translator, op):
     """Use MS SQL CONVERT() in place of STRFTIME().
 
     This is pretty restrictive due to the limited styles offered by SQL Server,
     we've just covered off the generic formats used when casting date based columns
     to string in order to complete row data comparison."""
     arg, pattern = map(translator.translate, op.args)
@@ -506,18 +523,19 @@
 TemporalValue.to_char = compile_to_char
 
 BigQueryExprTranslator._registry[HashBytes] = format_hashbytes_bigquery
 BigQueryExprTranslator._registry[RawSQL] = format_raw_sql
 BigQueryExprTranslator._registry[Strftime] = strftime_bigquery
 BigQueryExprTranslator._registry[BinaryLength] = sa_format_binary_length
 
-TrinoSQLExprTranslator._registry[HashBytes] = format_hashbytes_trino
+TrinoSQLExprTranslator._registry[HashBytes] = sa_format_hashbytes_trino
 TrinoSQLExprTranslator._registry[RawSQL] = sa_format_raw_sql
 TrinoSQLExprTranslator._registry[ToChar] = sa_format_to_char
 TrinoSQLExprTranslator._registry[BinaryLength] = sa_format_binary_length
+TrinoSQLExprTranslator._registry[Strftime] = strftime_trino
 
 AlchemyExprTranslator._registry[RawSQL] = format_raw_sql
 AlchemyExprTranslator._registry[HashBytes] = format_hashbytes_alchemy
 ExprTranslator._registry[RawSQL] = format_raw_sql
 ExprTranslator._registry[HashBytes] = format_hashbytes_base
 
 ImpalaExprTranslator._registry[RawSQL] = format_raw_sql
```

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/__init__.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_cloud_spanner/__init__.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/api.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_cloud_spanner/api.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/client.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_cloud_spanner/client.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/compiler.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_cloud_spanner/compiler.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/datatypes.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_cloud_spanner/datatypes.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/registry.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_cloud_spanner/registry.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_db2/__init__.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_db2/__init__.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_db2/api.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_db2/api.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_db2/compiler.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_db2/compiler.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_db2/datatypes.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_db2/datatypes.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_db2/registry.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_db2/registry.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_impala/api.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_impala/api.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_mssql/__init__.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_mssql/api.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_mssql/api.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_mssql/datatypes.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_mssql/datatypes.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_mysql/base_sql_compiler/select_builder.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_mysql/base_sql_compiler/select_builder.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_mysql/compiler.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_mysql/compiler.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_oracle/__init__.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_oracle/api.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_oracle/api.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_oracle/compiler.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_oracle/compiler.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_oracle/datatypes.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_oracle/datatypes.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_oracle/registry.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_oracle/registry.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_postgres/client.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_postgres/client.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_postgres/datatypes.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_postgres/datatypes.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_redshift/__init__.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_redshift/api.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_redshift/api.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_redshift/compiler.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_redshift/compiler.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_snowflake/api.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_snowflake/api.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_snowflake/datatypes.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_snowflake/datatypes.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_teradata/__init__.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_teradata/__init__.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_teradata/api.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_teradata/api.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_teradata/compiler.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_teradata/compiler.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_teradata/datatypes.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_teradata/datatypes.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_teradata/registry.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_teradata/registry.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.1.0/third_party/ibis/ibis_trino/datatypes.py` & `momo_data_validation_service-1.2.0/third_party/ibis/ibis_trino/datatypes.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import ibis.expr.datatypes as dt
 from trino.sqlalchemy.dialect import TrinoDialect
 from trino.sqlalchemy.datatype import parse_sqltype
+import third_party.ibis.ibis_trino.registry
+
 
 VARBINARY=parse_sqltype("varbinary")
 
 @dt.dtype.register(TrinoDialect, type(VARBINARY))
 def sa_trino_varbinary(_, satype, nullable=True):
     return dt.binary(nullable=nullable)
```

