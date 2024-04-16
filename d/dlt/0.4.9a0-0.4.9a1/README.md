# Comparing `tmp/dlt-0.4.9a0.tar.gz` & `tmp/dlt-0.4.9a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt-0.4.9a0.tar", max compression
+gzip compressed data, was "dlt-0.4.9a1.tar", max compression
```

## Comparing `dlt-0.4.9a0.tar` & `dlt-0.4.9a1.tar`

### file list

```diff
@@ -1,347 +1,348 @@
--rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.4.9a0/LICENSE.txt
--rw-r--r--   0        0        0     5298 2024-04-14 11:41:16.421673 dlt-0.4.9a0/README.md
--rw-r--r--   0        0        0     2229 2024-04-07 14:59:43.705656 dlt-0.4.9a0/dlt/__init__.py
--rw-r--r--   0        0        0       69 2024-03-08 19:36:32.659855 dlt-0.4.9a0/dlt/__main__.py
--rw-r--r--   0        0        0        0 2023-11-18 17:38:04.257189 dlt-0.4.9a0/dlt/cli/__init__.py
--rw-r--r--   0        0        0    21512 2024-04-14 11:41:16.421673 dlt-0.4.9a0/dlt/cli/_dlt.py
--rw-r--r--   0        0        0     4187 2024-04-14 11:41:16.421673 dlt-0.4.9a0/dlt/cli/config_toml_writer.py
--rw-r--r--   0        0        0    18229 2024-01-24 17:23:08.476518 dlt-0.4.9a0/dlt/cli/deploy_command.py
--rw-r--r--   0        0        0    16912 2024-04-13 11:38:43.050742 dlt-0.4.9a0/dlt/cli/deploy_command_helpers.py
--rw-r--r--   0        0        0     1944 2024-01-25 20:07:33.363195 dlt-0.4.9a0/dlt/cli/echo.py
--rw-r--r--   0        0        0      435 2023-11-18 17:38:04.257189 dlt-0.4.9a0/dlt/cli/exceptions.py
--rw-r--r--   0        0        0    21105 2024-04-13 11:38:33.320742 dlt-0.4.9a0/dlt/cli/init_command.py
--rw-r--r--   0        0        0    14157 2024-04-14 11:41:16.421673 dlt-0.4.9a0/dlt/cli/pipeline_command.py
--rw-r--r--   0        0        0    10152 2024-04-13 11:38:50.650742 dlt-0.4.9a0/dlt/cli/pipeline_files.py
--rw-r--r--   0        0        0     2524 2024-01-24 17:23:08.476518 dlt-0.4.9a0/dlt/cli/requirements.py
--rw-r--r--   0        0        0     4895 2024-01-24 17:23:08.476518 dlt-0.4.9a0/dlt/cli/source_detection.py
--rw-r--r--   0        0        0     1912 2024-01-24 17:23:08.476518 dlt-0.4.9a0/dlt/cli/telemetry_command.py
--rw-r--r--   0        0        0     1999 2024-04-14 11:41:16.421673 dlt-0.4.9a0/dlt/cli/utils.py
--rw-r--r--   0        0        0      292 2024-04-09 13:29:46.170457 dlt-0.4.9a0/dlt/common/__init__.py
--rw-r--r--   0        0        0     1311 2024-01-24 17:23:08.476518 dlt-0.4.9a0/dlt/common/arithmetics.py
--rw-r--r--   0        0        0      808 2024-04-07 14:59:43.705656 dlt-0.4.9a0/dlt/common/configuration/__init__.py
--rw-r--r--   0        0        0     5144 2024-01-24 17:23:08.476518 dlt-0.4.9a0/dlt/common/configuration/accessors.py
--rw-r--r--   0        0        0     7410 2024-04-07 14:59:43.705656 dlt-0.4.9a0/dlt/common/configuration/container.py
--rw-r--r--   0        0        0     8457 2024-01-24 17:23:08.486518 dlt-0.4.9a0/dlt/common/configuration/exceptions.py
--rw-r--r--   0        0        0    11848 2024-04-13 11:29:48.720735 dlt-0.4.9a0/dlt/common/configuration/inject.py
--rw-r--r--   0        0        0     1777 2024-01-25 20:07:33.363195 dlt-0.4.9a0/dlt/common/configuration/paths.py
--rw-r--r--   0        0        0      682 2024-01-24 17:23:08.486518 dlt-0.4.9a0/dlt/common/configuration/providers/__init__.py
--rw-r--r--   0        0        0      805 2024-03-05 18:21:35.930419 dlt-0.4.9a0/dlt/common/configuration/providers/airflow.py
--rw-r--r--   0        0        0     1129 2024-01-24 17:23:08.486518 dlt-0.4.9a0/dlt/common/configuration/providers/context.py
--rw-r--r--   0        0        0     1346 2024-01-24 17:23:08.486518 dlt-0.4.9a0/dlt/common/configuration/providers/dictionary.py
--rw-r--r--   0        0        0     1995 2024-01-24 17:23:08.486518 dlt-0.4.9a0/dlt/common/configuration/providers/environ.py
--rw-r--r--   0        0        0     5141 2024-04-14 11:41:16.421673 dlt-0.4.9a0/dlt/common/configuration/providers/google_secrets.py
--rw-r--r--   0        0        0     1319 2024-01-24 17:23:08.486518 dlt-0.4.9a0/dlt/common/configuration/providers/provider.py
--rw-r--r--   0        0        0    13416 2024-04-14 11:41:16.421673 dlt-0.4.9a0/dlt/common/configuration/providers/toml.py
--rw-r--r--   0        0        0    20983 2024-04-09 13:29:46.170457 dlt-0.4.9a0/dlt/common/configuration/resolve.py
--rw-r--r--   0        0        0     1742 2024-01-24 17:23:08.486518 dlt-0.4.9a0/dlt/common/configuration/specs/__init__.py
--rw-r--r--   0        0        0     1836 2024-04-09 13:29:46.170457 dlt-0.4.9a0/dlt/common/configuration/specs/api_credentials.py
--rw-r--r--   0        0        0     5263 2024-04-09 13:29:46.170457 dlt-0.4.9a0/dlt/common/configuration/specs/aws_credentials.py
--rw-r--r--   0        0        0     2591 2024-04-14 11:41:16.421673 dlt-0.4.9a0/dlt/common/configuration/specs/azure_credentials.py
--rw-r--r--   0        0        0    18147 2024-04-11 11:44:50.568746 dlt-0.4.9a0/dlt/common/configuration/specs/base_configuration.py
--rw-r--r--   0        0        0     6498 2024-04-09 13:29:46.170457 dlt-0.4.9a0/dlt/common/configuration/specs/config_providers_context.py
--rw-r--r--   0        0        0     3456 2024-04-09 13:29:46.170457 dlt-0.4.9a0/dlt/common/configuration/specs/config_section_context.py
--rw-r--r--   0        0        0     2339 2024-04-09 13:29:46.170457 dlt-0.4.9a0/dlt/common/configuration/specs/connection_string_credentials.py
--rw-r--r--   0        0        0     2667 2024-01-24 17:23:08.486518 dlt-0.4.9a0/dlt/common/configuration/specs/exceptions.py
--rw-r--r--   0        0        0    13349 2024-04-14 11:41:16.421673 dlt-0.4.9a0/dlt/common/configuration/specs/gcp_credentials.py
--rw-r--r--   0        0        0      874 2024-04-09 13:29:46.170457 dlt-0.4.9a0/dlt/common/configuration/specs/known_sections.py
--rw-r--r--   0        0        0     2856 2024-04-09 13:29:46.170457 dlt-0.4.9a0/dlt/common/configuration/specs/run_configuration.py
--rw-r--r--   0        0        0     6650 2024-04-14 11:41:16.421673 dlt-0.4.9a0/dlt/common/configuration/utils.py
--rw-r--r--   0        0        0      220 2024-01-24 17:23:08.486518 dlt-0.4.9a0/dlt/common/data_types/__init__.py
--rw-r--r--   0        0        0     6832 2024-04-14 11:41:16.421673 dlt-0.4.9a0/dlt/common/data_types/type_helpers.py
--rw-r--r--   0        0        0      269 2024-01-24 17:23:08.486518 dlt-0.4.9a0/dlt/common/data_types/typing.py
--rw-r--r--   0        0        0      592 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/common/data_writers/__init__.py
--rw-r--r--   0        0        0    10821 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/common/data_writers/buffered.py
--rw-r--r--   0        0        0     5665 2024-04-14 11:41:16.421673 dlt-0.4.9a0/dlt/common/data_writers/escape.py
--rw-r--r--   0        0        0     1757 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/common/data_writers/exceptions.py
--rw-r--r--   0        0        0    23095 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/data_writers/writers.py
--rw-r--r--   0        0        0      423 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/destination/__init__.py
--rw-r--r--   0        0        0     3651 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/common/destination/capabilities.py
--rw-r--r--   0        0        0     5132 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/common/destination/exceptions.py
--rw-r--r--   0        0        0    25485 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/destination/reference.py
--rw-r--r--   0        0        0     6274 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/common/exceptions.py
--rw-r--r--   0        0        0     5149 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/git.py
--rw-r--r--   0        0        0     7099 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/json/__init__.py
--rw-r--r--   0        0        0     1814 2024-02-16 18:38:47.332466 dlt-0.4.9a0/dlt/common/json/_orjson.py
--rw-r--r--   0        0        0     2948 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/json/_simplejson.py
--rw-r--r--   0        0        0     1562 2023-11-18 17:38:04.257189 dlt-0.4.9a0/dlt/common/jsonpath.py
--rw-r--r--   0        0        0        0 2023-11-18 17:38:04.257189 dlt-0.4.9a0/dlt/common/libs/__init__.py
--rw-r--r--   0        0        0      181 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/libs/numpy.py
--rw-r--r--   0        0        0      436 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/libs/pandas.py
--rw-r--r--   0        0        0      217 2024-04-07 14:59:43.715656 dlt-0.4.9a0/dlt/common/libs/pandas_sql.py
--rw-r--r--   0        0        0    14934 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/libs/pyarrow.py
--rw-r--r--   0        0        0    15624 2024-02-27 21:03:24.137544 dlt-0.4.9a0/dlt/common/libs/pydantic.py
--rw-r--r--   0        0        0    15486 2024-03-08 19:36:32.669855 dlt-0.4.9a0/dlt/common/libs/sql_alchemy.py
--rw-r--r--   0        0        0     3652 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/common/logger.py
--rw-r--r--   0        0        0      854 2024-03-01 09:52:05.856761 dlt-0.4.9a0/dlt/common/managed_thread_pool.py
--rw-r--r--   0        0        0      384 2024-03-18 14:01:48.098768 dlt-0.4.9a0/dlt/common/normalizers/__init__.py
--rw-r--r--   0        0        0     1408 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/common/normalizers/configuration.py
--rw-r--r--   0        0        0      510 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/normalizers/exceptions.py
--rw-r--r--   0        0        0     1905 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/normalizers/json/__init__.py
--rw-r--r--   0        0        0    16970 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/normalizers/json/relational.py
--rw-r--r--   0        0        0      123 2024-03-18 14:01:48.098768 dlt-0.4.9a0/dlt/common/normalizers/naming/__init__.py
--rw-r--r--   0        0        0      810 2024-02-27 21:03:24.137544 dlt-0.4.9a0/dlt/common/normalizers/naming/direct.py
--rw-r--r--   0        0        0      798 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/normalizers/naming/duck_case.py
--rw-r--r--   0        0        0      830 2024-03-18 14:01:48.098768 dlt-0.4.9a0/dlt/common/normalizers/naming/exceptions.py
--rw-r--r--   0        0        0     4570 2024-03-18 14:01:48.098768 dlt-0.4.9a0/dlt/common/normalizers/naming/naming.py
--rw-r--r--   0        0        0     2967 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/normalizers/naming/snake_case.py
--rw-r--r--   0        0        0      359 2024-03-18 14:01:48.108768 dlt-0.4.9a0/dlt/common/normalizers/typing.py
--rw-r--r--   0        0        0     3426 2024-04-07 14:59:43.715656 dlt-0.4.9a0/dlt/common/normalizers/utils.py
--rw-r--r--   0        0        0      461 2024-02-27 21:03:24.137544 dlt-0.4.9a0/dlt/common/pendulum.py
--rw-r--r--   0        0        0    31127 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/pipeline.py
--rw-r--r--   0        0        0        0 2023-11-18 17:38:04.267189 dlt-0.4.9a0/dlt/common/reflection/__init__.py
--rw-r--r--   0        0        0      375 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/reflection/function_visitor.py
--rw-r--r--   0        0        0     6119 2024-04-07 14:59:43.715656 dlt-0.4.9a0/dlt/common/reflection/spec.py
--rw-r--r--   0        0        0     5103 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/reflection/utils.py
--rw-r--r--   0        0        0      329 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/runners/__init__.py
--rw-r--r--   0        0        0      665 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/common/runners/configuration.py
--rw-r--r--   0        0        0     3678 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/runners/pool_runner.py
--rw-r--r--   0        0        0     4132 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/runners/runnable.py
--rw-r--r--   0        0        0     3162 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/runners/stdout.py
--rw-r--r--   0        0        0     2137 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/runners/synth_pickle.py
--rw-r--r--   0        0        0      105 2023-11-18 17:38:04.267189 dlt-0.4.9a0/dlt/common/runners/typing.py
--rw-r--r--   0        0        0     5583 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/runners/venv.py
--rw-r--r--   0        0        0       71 2023-11-18 17:38:04.267189 dlt-0.4.9a0/dlt/common/runtime/__init__.py
--rw-r--r--   0        0        0    14599 2024-04-13 11:30:10.760740 dlt-0.4.9a0/dlt/common/runtime/collector.py
--rw-r--r--   0        0        0     5461 2024-01-25 20:07:33.363195 dlt-0.4.9a0/dlt/common/runtime/exec_info.py
--rw-r--r--   0        0        0     1067 2024-04-13 11:30:15.860741 dlt-0.4.9a0/dlt/common/runtime/init.py
--rw-r--r--   0        0        0     6616 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/runtime/json_logging.py
--rw-r--r--   0        0        0     2044 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/runtime/prometheus.py
--rw-r--r--   0        0        0     6702 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/runtime/segment.py
--rw-r--r--   0        0        0     2784 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/runtime/sentry.py
--rw-r--r--   0        0        0     1938 2024-04-13 11:30:29.100742 dlt-0.4.9a0/dlt/common/runtime/signals.py
--rw-r--r--   0        0        0      613 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/runtime/slack.py
--rw-r--r--   0        0        0     2960 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/runtime/telemetry.py
--rw-r--r--   0        0        0      579 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/runtime/typing.py
--rw-r--r--   0        0        0      805 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/schema/__init__.py
--rw-r--r--   0        0        0     2454 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/schema/detections.py
--rw-r--r--   0        0        0     5308 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/schema/exceptions.py
--rw-r--r--   0        0        0     5269 2024-03-18 14:01:48.108768 dlt-0.4.9a0/dlt/common/schema/migrations.py
--rw-r--r--   0        0        0    42497 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/schema/schema.py
--rw-r--r--   0        0        0     5865 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/schema/typing.py
--rw-r--r--   0        0        0    28875 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/schema/utils.py
--rw-r--r--   0        0        0     1672 2024-02-10 23:59:00.181729 dlt-0.4.9a0/dlt/common/source.py
--rw-r--r--   0        0        0     1224 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/storages/__init__.py
--rw-r--r--   0        0        0     4869 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/common/storages/configuration.py
--rw-r--r--   0        0        0     4230 2024-04-13 11:30:55.040743 dlt-0.4.9a0/dlt/common/storages/data_item_storage.py
--rw-r--r--   0        0        0     4184 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/common/storages/exceptions.py
--rw-r--r--   0        0        0    14242 2024-01-24 17:23:08.506518 dlt-0.4.9a0/dlt/common/storages/file_storage.py
--rw-r--r--   0        0        0    11065 2024-04-14 11:41:16.441673 dlt-0.4.9a0/dlt/common/storages/fsspec_filesystem.py
--rw-r--r--   0        0        0        0 2024-02-26 22:08:47.270507 dlt-0.4.9a0/dlt/common/storages/fsspecs/__init__.py
--rw-r--r--   0        0        0    20479 2024-04-14 11:41:16.441673 dlt-0.4.9a0/dlt/common/storages/fsspecs/google_drive.py
--rw-r--r--   0        0        0     3513 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/common/storages/live_schema_storage.py
--rw-r--r--   0        0        0    26784 2024-04-14 11:41:16.441673 dlt-0.4.9a0/dlt/common/storages/load_package.py
--rw-r--r--   0        0        0    10771 2024-04-14 11:41:16.441673 dlt-0.4.9a0/dlt/common/storages/load_storage.py
--rw-r--r--   0        0        0     3197 2024-04-07 14:59:43.715656 dlt-0.4.9a0/dlt/common/storages/normalize_storage.py
--rw-r--r--   0        0        0     9551 2024-04-14 11:41:16.441673 dlt-0.4.9a0/dlt/common/storages/schema_storage.py
--rw-r--r--   0        0        0     9065 2024-01-24 17:23:08.506518 dlt-0.4.9a0/dlt/common/storages/transactional_file.py
--rw-r--r--   0        0        0     2867 2024-01-24 17:23:08.506518 dlt-0.4.9a0/dlt/common/storages/versioned_storage.py
--rw-r--r--   0        0        0     7604 2024-04-14 11:41:16.441673 dlt-0.4.9a0/dlt/common/time.py
--rw-r--r--   0        0        0     8878 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/common/typing.py
--rw-r--r--   0        0        0    19596 2024-04-14 11:41:16.441673 dlt-0.4.9a0/dlt/common/utils.py
--rw-r--r--   0        0        0     7978 2024-04-07 14:59:43.715656 dlt-0.4.9a0/dlt/common/validation.py
--rw-r--r--   0        0        0     2369 2024-04-14 11:41:16.441673 dlt-0.4.9a0/dlt/common/versioned_state.py
--rw-r--r--   0        0        0     5528 2024-01-24 17:23:08.506518 dlt-0.4.9a0/dlt/common/warnings.py
--rw-r--r--   0        0        0     1219 2024-01-24 17:23:08.506518 dlt-0.4.9a0/dlt/common/wei.py
--rw-r--r--   0        0        0     1217 2024-04-11 11:44:50.568746 dlt-0.4.9a0/dlt/destinations/__init__.py
--rw-r--r--   0        0        0      404 2024-02-27 21:03:24.137544 dlt-0.4.9a0/dlt/destinations/adapters.py
--rw-r--r--   0        0        0     4856 2024-04-14 11:41:16.441673 dlt-0.4.9a0/dlt/destinations/decorators.py
--rw-r--r--   0        0        0     4918 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/destinations/exceptions.py
--rw-r--r--   0        0        0        0 2024-01-24 17:23:08.506518 dlt-0.4.9a0/dlt/destinations/impl/__init__.py
--rw-r--r--   0        0        0     1311 2024-03-18 14:01:48.108768 dlt-0.4.9a0/dlt/destinations/impl/athena/__init__.py
--rw-r--r--   0        0        0    18693 2024-04-13 11:31:25.760744 dlt-0.4.9a0/dlt/destinations/impl/athena/athena.py
--rw-r--r--   0        0        0     1054 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/destinations/impl/athena/configuration.py
--rw-r--r--   0        0        0     2169 2024-01-24 17:23:08.506518 dlt-0.4.9a0/dlt/destinations/impl/athena/factory.py
--rw-r--r--   0        0        0      439 2024-02-27 21:03:24.137544 dlt-0.4.9a0/dlt/destinations/impl/bigquery/README.md
--rw-r--r--   0        0        0     1118 2024-03-18 14:01:48.108768 dlt-0.4.9a0/dlt/destinations/impl/bigquery/__init__.py
--rw-r--r--   0        0        0    21073 2024-04-14 11:41:16.441673 dlt-0.4.9a0/dlt/destinations/impl/bigquery/bigquery.py
--rw-r--r--   0        0        0     8397 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/bigquery/bigquery_adapter.py
--rw-r--r--   0        0        0     1740 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/bigquery/configuration.py
--rw-r--r--   0        0        0     1309 2024-02-07 18:59:43.276965 dlt-0.4.9a0/dlt/destinations/impl/bigquery/factory.py
--rw-r--r--   0        0        0    10772 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/bigquery/sql_client.py
--rw-r--r--   0        0        0     1430 2024-03-18 14:01:48.118769 dlt-0.4.9a0/dlt/destinations/impl/databricks/__init__.py
--rw-r--r--   0        0        0     2043 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/destinations/impl/databricks/configuration.py
--rw-r--r--   0        0        0    13640 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/databricks/databricks.py
--rw-r--r--   0        0        0     1741 2024-02-07 18:59:43.276965 dlt-0.4.9a0/dlt/destinations/impl/databricks/factory.py
--rw-r--r--   0        0        0     6074 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/destinations/impl/databricks/sql_client.py
--rw-r--r--   0        0        0      673 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/destination/__init__.py
--rw-r--r--   0        0        0     1047 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/destination/configuration.py
--rw-r--r--   0        0        0     3675 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/destination/destination.py
--rw-r--r--   0        0        0     5626 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/destinations/impl/destination/factory.py
--rw-r--r--   0        0        0     1243 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/dremio/__init__.py
--rw-r--r--   0        0        0     1617 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/dremio/configuration.py
--rw-r--r--   0        0        0     8692 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/dremio/dremio.py
--rw-r--r--   0        0        0     1787 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/dremio/factory.py
--rw-r--r--   0        0        0     9314 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/dremio/pydremio.py
--rw-r--r--   0        0        0     5934 2024-04-13 11:31:52.880745 dlt-0.4.9a0/dlt/destinations/impl/dremio/sql_client.py
--rw-r--r--   0        0        0     1236 2024-03-18 14:01:48.118769 dlt-0.4.9a0/dlt/destinations/impl/duckdb/__init__.py
--rw-r--r--   0        0        0     9013 2024-04-13 11:31:56.870745 dlt-0.4.9a0/dlt/destinations/impl/duckdb/configuration.py
--rw-r--r--   0        0        0     7022 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/duckdb/duck.py
--rw-r--r--   0        0        0     1969 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/duckdb/factory.py
--rw-r--r--   0        0        0     6828 2024-04-05 22:42:00.549456 dlt-0.4.9a0/dlt/destinations/impl/duckdb/sql_client.py
--rw-r--r--   0        0        0     1485 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/dummy/__init__.py
--rw-r--r--   0        0        0     1027 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/destinations/impl/dummy/configuration.py
--rw-r--r--   0        0        0     6713 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/destinations/impl/dummy/dummy.py
--rw-r--r--   0        0        0     1111 2024-02-23 11:16:27.641941 dlt-0.4.9a0/dlt/destinations/impl/dummy/factory.py
--rw-r--r--   0        0        0      194 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/filesystem/__init__.py
--rw-r--r--   0        0        0      889 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/destinations/impl/filesystem/configuration.py
--rw-r--r--   0        0        0     2411 2024-03-24 19:55:58.511453 dlt-0.4.9a0/dlt/destinations/impl/filesystem/factory.py
--rw-r--r--   0        0        0     9542 2024-04-13 11:32:01.360745 dlt-0.4.9a0/dlt/destinations/impl/filesystem/filesystem.py
--rw-r--r--   0        0        0     1134 2024-03-18 14:01:48.118769 dlt-0.4.9a0/dlt/destinations/impl/motherduck/__init__.py
--rw-r--r--   0        0        0     3111 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/motherduck/configuration.py
--rw-r--r--   0        0        0     1966 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/motherduck/factory.py
--rw-r--r--   0        0        0      911 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/motherduck/motherduck.py
--rw-r--r--   0        0        0     1515 2024-03-18 14:01:48.118769 dlt-0.4.9a0/dlt/destinations/impl/motherduck/sql_client.py
--rw-r--r--   0        0        0      253 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/mssql/README.md
--rw-r--r--   0        0        0     1385 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/mssql/__init__.py
--rw-r--r--   0        0        0     3971 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/destinations/impl/mssql/configuration.py
--rw-r--r--   0        0        0     1764 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/mssql/factory.py
--rw-r--r--   0        0        0     7537 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/mssql/mssql.py
--rw-r--r--   0        0        0     6629 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/mssql/sql_client.py
--rw-r--r--   0        0        0      251 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/postgres/README.md
--rw-r--r--   0        0        0     1356 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/postgres/__init__.py
--rw-r--r--   0        0        0     1794 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/destinations/impl/postgres/configuration.py
--rw-r--r--   0        0        0     1840 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/postgres/factory.py
--rw-r--r--   0        0        0     6940 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/postgres/postgres.py
--rw-r--r--   0        0        0     5678 2024-03-31 18:13:49.090176 dlt-0.4.9a0/dlt/destinations/impl/postgres/sql_client.py
--rw-r--r--   0        0        0      677 2024-03-18 14:01:48.118769 dlt-0.4.9a0/dlt/destinations/impl/qdrant/__init__.py
--rw-r--r--   0        0        0     3044 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/destinations/impl/qdrant/configuration.py
--rw-r--r--   0        0        0     1146 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/qdrant/factory.py
--rw-r--r--   0        0        0     1831 2024-02-07 18:59:43.276965 dlt-0.4.9a0/dlt/destinations/impl/qdrant/qdrant_adapter.py
--rw-r--r--   0        0        0    17960 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/destinations/impl/qdrant/qdrant_client.py
--rw-r--r--   0        0        0     1159 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/redshift/README.md
--rw-r--r--   0        0        0     1181 2024-03-18 14:01:48.118769 dlt-0.4.9a0/dlt/destinations/impl/redshift/__init__.py
--rw-r--r--   0        0        0     1005 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/destinations/impl/redshift/configuration.py
--rw-r--r--   0        0        0     2006 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/redshift/factory.py
--rw-r--r--   0        0        0    10832 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/redshift/redshift.py
--rw-r--r--   0        0        0     1218 2024-03-18 14:01:48.118769 dlt-0.4.9a0/dlt/destinations/impl/snowflake/__init__.py
--rw-r--r--   0        0        0     5449 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/destinations/impl/snowflake/configuration.py
--rw-r--r--   0        0        0     2008 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/snowflake/factory.py
--rw-r--r--   0        0        0    11468 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/snowflake/snowflake.py
--rw-r--r--   0        0        0     6885 2024-03-18 14:01:48.118769 dlt-0.4.9a0/dlt/destinations/impl/snowflake/sql_client.py
--rw-r--r--   0        0        0     2851 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/synapse/__init__.py
--rw-r--r--   0        0        0     2746 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/destinations/impl/synapse/configuration.py
--rw-r--r--   0        0        0     2640 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/destinations/impl/synapse/factory.py
--rw-r--r--   0        0        0     1179 2024-02-07 18:59:43.276965 dlt-0.4.9a0/dlt/destinations/impl/synapse/sql_client.py
--rw-r--r--   0        0        0    13201 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/synapse/synapse.py
--rw-r--r--   0        0        0     2231 2024-03-08 19:36:32.679855 dlt-0.4.9a0/dlt/destinations/impl/synapse/synapse_adapter.py
--rw-r--r--   0        0        0      526 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/weaviate/README.md
--rw-r--r--   0        0        0      752 2024-03-18 14:01:48.118769 dlt-0.4.9a0/dlt/destinations/impl/weaviate/__init__.py
--rw-r--r--   0        0        0      280 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/weaviate/ci_naming.py
--rw-r--r--   0        0        0     2009 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/destinations/impl/weaviate/configuration.py
--rw-r--r--   0        0        0      666 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/destinations/impl/weaviate/exceptions.py
--rw-r--r--   0        0        0     1935 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/weaviate/factory.py
--rw-r--r--   0        0        0     3259 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/weaviate/naming.py
--rw-r--r--   0        0        0     3914 2024-02-07 18:59:43.276965 dlt-0.4.9a0/dlt/destinations/impl/weaviate/weaviate_adapter.py
--rw-r--r--   0        0        0    26468 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/destinations/impl/weaviate/weaviate_client.py
--rw-r--r--   0        0        0     6149 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/insert_job_client.py
--rw-r--r--   0        0        0    23940 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/destinations/job_client_impl.py
--rw-r--r--   0        0        0     6300 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/destinations/job_impl.py
--rw-r--r--   0        0        0     3075 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/destinations/path_utils.py
--rw-r--r--   0        0        0     9279 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/sql_client.py
--rw-r--r--   0        0        0    26428 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/destinations/sql_jobs.py
--rw-r--r--   0        0        0     4895 2024-02-27 21:03:24.137544 dlt-0.4.9a0/dlt/destinations/type_mapping.py
--rw-r--r--   0        0        0     1877 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/typing.py
--rw-r--r--   0        0        0      506 2024-04-11 11:44:50.568746 dlt-0.4.9a0/dlt/destinations/utils.py
--rw-r--r--   0        0        0      639 2024-04-07 14:59:43.715656 dlt-0.4.9a0/dlt/extract/__init__.py
--rw-r--r--   0        0        0     8539 2024-03-08 19:36:32.679855 dlt-0.4.9a0/dlt/extract/concurrency.py
--rw-r--r--   0        0        0    35950 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/extract/decorators.py
--rw-r--r--   0        0        0    16480 2024-03-08 19:36:32.679855 dlt-0.4.9a0/dlt/extract/exceptions.py
--rw-r--r--   0        0        0    17697 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/extract/extract.py
--rw-r--r--   0        0        0    15690 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/extract/extractors.py
--rw-r--r--   0        0        0    21382 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/extract/hints.py
--rw-r--r--   0        0        0    29587 2024-04-14 11:41:16.461673 dlt-0.4.9a0/dlt/extract/incremental/__init__.py
--rw-r--r--   0        0        0     1142 2024-01-24 17:23:08.526518 dlt-0.4.9a0/dlt/extract/incremental/exceptions.py
--rw-r--r--   0        0        0    14951 2024-04-14 11:41:16.461673 dlt-0.4.9a0/dlt/extract/incremental/transform.py
--rw-r--r--   0        0        0      322 2024-01-24 17:23:08.526518 dlt-0.4.9a0/dlt/extract/incremental/typing.py
--rw-r--r--   0        0        0     6786 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/extract/items.py
--rw-r--r--   0        0        0    16368 2024-03-08 19:36:32.679855 dlt-0.4.9a0/dlt/extract/pipe.py
--rw-r--r--   0        0        0    16344 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/extract/pipe_iterator.py
--rw-r--r--   0        0        0    26683 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/extract/resource.py
--rw-r--r--   0        0        0    19990 2024-03-18 14:01:48.118769 dlt-0.4.9a0/dlt/extract/source.py
--rw-r--r--   0        0        0     4650 2024-04-14 11:41:16.461673 dlt-0.4.9a0/dlt/extract/storage.py
--rw-r--r--   0        0        0    10122 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/extract/utils.py
--rw-r--r--   0        0        0     3500 2024-03-08 19:36:32.679855 dlt-0.4.9a0/dlt/extract/validation.py
--rw-r--r--   0        0        0      832 2024-04-07 14:59:43.715656 dlt-0.4.9a0/dlt/extract/wrappers.py
--rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.4.9a0/dlt/helpers/__init__.py
--rw-r--r--   0        0        0    23547 2024-04-14 11:41:16.461673 dlt-0.4.9a0/dlt/helpers/airflow_helper.py
--rw-r--r--   0        0        0     3701 2024-01-24 17:23:08.526518 dlt-0.4.9a0/dlt/helpers/dbt/__init__.py
--rw-r--r--   0        0        0     1241 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/helpers/dbt/configuration.py
--rw-r--r--   0        0        0     6848 2024-04-14 11:41:16.461673 dlt-0.4.9a0/dlt/helpers/dbt/dbt_utils.py
--rw-r--r--   0        0        0      772 2024-01-24 17:23:08.526518 dlt-0.4.9a0/dlt/helpers/dbt/exceptions.py
--rw-r--r--   0        0        0     7163 2024-02-07 18:59:43.286965 dlt-0.4.9a0/dlt/helpers/dbt/profiles.yml
--rw-r--r--   0        0        0    15742 2024-04-13 11:33:15.710743 dlt-0.4.9a0/dlt/helpers/dbt/runner.py
--rw-r--r--   0        0        0     4881 2023-11-18 17:38:04.277189 dlt-0.4.9a0/dlt/helpers/dbt_cloud/__init__.py
--rw-r--r--   0        0        0     4926 2024-01-24 17:23:08.526518 dlt-0.4.9a0/dlt/helpers/dbt_cloud/client.py
--rw-r--r--   0        0        0      623 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/helpers/dbt_cloud/configuration.py
--rw-r--r--   0        0        0      349 2024-04-14 11:41:16.461673 dlt-0.4.9a0/dlt/helpers/streamlit_app/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 14:59:43.715656 dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/__init__.py
--rw-r--r--   0        0        0     1239 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/load_info.py
--rw-r--r--   0        0        0      483 2024-04-07 14:59:43.715656 dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/menu.py
--rw-r--r--   0        0        0     2451 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/query.py
--rw-r--r--   0        0        0     1139 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/resource_state.py
--rw-r--r--   0        0        0      618 2024-04-07 14:59:43.715656 dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/show_data.py
--rw-r--r--   0        0        0     2842 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/table_hints.py
--rw-r--r--   0        0        0      150 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/index.py
--rw-r--r--   0        0        0        0 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/pages/__init__.py
--rw-r--r--   0        0        0     1668 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/pages/dashboard.py
--rw-r--r--   0        0        0     4446 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/pages/load_info.py
--rw-r--r--   0        0        0      757 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/theme.py
--rw-r--r--   0        0        0     2361 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/helpers/streamlit_app/utils.py
--rw-r--r--   0        0        0      386 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/__init__.py
--rw-r--r--   0        0        0      901 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/color_mode_selector.py
--rw-r--r--   0        0        0     1004 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/logo.py
--rw-r--r--   0        0        0      613 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/schema.py
--rw-r--r--   0        0        0     1542 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/stats.py
--rw-r--r--   0        0        0      805 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/summary.py
--rw-r--r--   0        0        0     1189 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/tags.py
--rw-r--r--   0        0        0       51 2023-11-18 17:38:04.277189 dlt-0.4.9a0/dlt/load/__init__.py
--rw-r--r--   0        0        0      807 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/load/configuration.py
--rw-r--r--   0        0        0     2061 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/load/exceptions.py
--rw-r--r--   0        0        0    25029 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/load/load.py
--rw-r--r--   0        0        0     8096 2024-04-13 11:33:36.000744 dlt-0.4.9a0/dlt/load/utils.py
--rw-r--r--   0        0        0       58 2024-01-24 17:23:08.526518 dlt-0.4.9a0/dlt/normalize/__init__.py
--rw-r--r--   0        0        0     1525 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/normalize/configuration.py
--rw-r--r--   0        0        0      644 2024-04-09 20:42:07.320460 dlt-0.4.9a0/dlt/normalize/exceptions.py
--rw-r--r--   0        0        0    18280 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/normalize/items_normalizers.py
--rw-r--r--   0        0        0    22419 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/normalize/normalize.py
--rw-r--r--   0        0        0    15006 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/pipeline/__init__.py
--rw-r--r--   0        0        0     2097 2024-04-09 20:42:07.320460 dlt-0.4.9a0/dlt/pipeline/configuration.py
--rw-r--r--   0        0        0      709 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/pipeline/current.py
--rw-r--r--   0        0        0     4950 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/pipeline/dbt.py
--rw-r--r--   0        0        0     4599 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/pipeline/exceptions.py
--rw-r--r--   0        0        0     9785 2024-04-09 20:42:07.320460 dlt-0.4.9a0/dlt/pipeline/helpers.py
--rw-r--r--   0        0        0      212 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/pipeline/mark.py
--rw-r--r--   0        0        0    74019 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/pipeline/pipeline.py
--rw-r--r--   0        0        0     3864 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/pipeline/platform.py
--rw-r--r--   0        0        0     1007 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/pipeline/progress.py
--rw-r--r--   0        0        0     4856 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/pipeline/state_sync.py
--rw-r--r--   0        0        0    13259 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/pipeline/trace.py
--rw-r--r--   0        0        0     5610 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/pipeline/track.py
--rw-r--r--   0        0        0       92 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/pipeline/typing.py
--rw-r--r--   0        0        0      796 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/pipeline/warnings.py
--rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.4.9a0/dlt/py.typed
--rw-r--r--   0        0        0        0 2023-11-18 17:38:04.277189 dlt-0.4.9a0/dlt/reflection/__init__.py
--rw-r--r--   0        0        0      565 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/reflection/names.py
--rw-r--r--   0        0        0     5818 2024-04-13 11:34:58.380741 dlt-0.4.9a0/dlt/reflection/script_inspector.py
--rw-r--r--   0        0        0     6278 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/reflection/script_visitor.py
--rw-r--r--   0        0        0      417 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/sources/__init__.py
--rw-r--r--   0        0        0      110 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/sources/config.py
--rw-r--r--   0        0        0      790 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/sources/credentials.py
--rw-r--r--   0        0        0      200 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/sources/filesystem.py
--rw-r--r--   0        0        0        0 2023-11-18 17:38:04.277189 dlt-0.4.9a0/dlt/sources/helpers/__init__.py
--rw-r--r--   0        0        0     1291 2024-04-09 20:42:07.320460 dlt-0.4.9a0/dlt/sources/helpers/requests/__init__.py
--rw-r--r--   0        0        0    10965 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/sources/helpers/requests/retry.py
--rw-r--r--   0        0        0     1969 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/sources/helpers/requests/session.py
--rw-r--r--   0        0        0      234 2023-11-18 17:38:04.277189 dlt-0.4.9a0/dlt/sources/helpers/requests/typing.py
--rw-r--r--   0        0        0     1210 2024-04-13 11:26:19.690742 dlt-0.4.9a0/dlt/sources/helpers/rest_client/__init__.py
--rw-r--r--   0        0        0     7190 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/sources/helpers/rest_client/auth.py
--rw-r--r--   0        0        0     9181 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/sources/helpers/rest_client/client.py
--rw-r--r--   0        0        0     4456 2024-04-13 22:20:19.334997 dlt-0.4.9a0/dlt/sources/helpers/rest_client/detector.py
--rw-r--r--   0        0        0      103 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/sources/helpers/rest_client/exceptions.py
--rw-r--r--   0        0        0     6001 2024-04-13 22:20:19.334997 dlt-0.4.9a0/dlt/sources/helpers/rest_client/paginators.py
--rw-r--r--   0        0        0      426 2024-04-13 22:20:19.334997 dlt-0.4.9a0/dlt/sources/helpers/rest_client/typing.py
--rw-r--r--   0        0        0      406 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/sources/helpers/rest_client/utils.py
--rw-r--r--   0        0        0     4860 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/sources/helpers/transform.py
--rw-r--r--   0        0        0     1130 2024-04-14 11:41:16.481673 dlt-0.4.9a0/dlt/version.py
--rw-r--r--   0        0        0     6985 2024-04-14 11:41:36.261674 dlt-0.4.9a0/pyproject.toml
--rw-r--r--   0        0        0     9936 1970-01-01 00:00:00.000000 dlt-0.4.9a0/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.4.9a1/LICENSE.txt
+-rw-r--r--   0        0        0     5298 2024-04-15 15:36:23.382155 dlt-0.4.9a1/README.md
+-rw-r--r--   0        0        0     2229 2024-04-07 14:59:43.705656 dlt-0.4.9a1/dlt/__init__.py
+-rw-r--r--   0        0        0       69 2024-03-08 19:36:32.659855 dlt-0.4.9a1/dlt/__main__.py
+-rw-r--r--   0        0        0        0 2023-11-18 17:38:04.257189 dlt-0.4.9a1/dlt/cli/__init__.py
+-rw-r--r--   0        0        0    21512 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/cli/_dlt.py
+-rw-r--r--   0        0        0     4187 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/cli/config_toml_writer.py
+-rw-r--r--   0        0        0    18229 2024-01-24 17:23:08.476518 dlt-0.4.9a1/dlt/cli/deploy_command.py
+-rw-r--r--   0        0        0    16912 2024-04-13 11:38:43.050742 dlt-0.4.9a1/dlt/cli/deploy_command_helpers.py
+-rw-r--r--   0        0        0     1944 2024-01-25 20:07:33.363195 dlt-0.4.9a1/dlt/cli/echo.py
+-rw-r--r--   0        0        0      435 2023-11-18 17:38:04.257189 dlt-0.4.9a1/dlt/cli/exceptions.py
+-rw-r--r--   0        0        0    21105 2024-04-13 11:38:33.320742 dlt-0.4.9a1/dlt/cli/init_command.py
+-rw-r--r--   0        0        0    14157 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/cli/pipeline_command.py
+-rw-r--r--   0        0        0    10152 2024-04-13 11:38:50.650742 dlt-0.4.9a1/dlt/cli/pipeline_files.py
+-rw-r--r--   0        0        0     2524 2024-01-24 17:23:08.476518 dlt-0.4.9a1/dlt/cli/requirements.py
+-rw-r--r--   0        0        0     4895 2024-01-24 17:23:08.476518 dlt-0.4.9a1/dlt/cli/source_detection.py
+-rw-r--r--   0        0        0     1912 2024-01-24 17:23:08.476518 dlt-0.4.9a1/dlt/cli/telemetry_command.py
+-rw-r--r--   0        0        0     1999 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/cli/utils.py
+-rw-r--r--   0        0        0      292 2024-04-09 13:29:46.170457 dlt-0.4.9a1/dlt/common/__init__.py
+-rw-r--r--   0        0        0     1311 2024-01-24 17:23:08.476518 dlt-0.4.9a1/dlt/common/arithmetics.py
+-rw-r--r--   0        0        0      808 2024-04-07 14:59:43.705656 dlt-0.4.9a1/dlt/common/configuration/__init__.py
+-rw-r--r--   0        0        0     5144 2024-01-24 17:23:08.476518 dlt-0.4.9a1/dlt/common/configuration/accessors.py
+-rw-r--r--   0        0        0     7410 2024-04-07 14:59:43.705656 dlt-0.4.9a1/dlt/common/configuration/container.py
+-rw-r--r--   0        0        0     8457 2024-01-24 17:23:08.486518 dlt-0.4.9a1/dlt/common/configuration/exceptions.py
+-rw-r--r--   0        0        0    11848 2024-04-13 11:29:48.720735 dlt-0.4.9a1/dlt/common/configuration/inject.py
+-rw-r--r--   0        0        0     1777 2024-01-25 20:07:33.363195 dlt-0.4.9a1/dlt/common/configuration/paths.py
+-rw-r--r--   0        0        0      682 2024-01-24 17:23:08.486518 dlt-0.4.9a1/dlt/common/configuration/providers/__init__.py
+-rw-r--r--   0        0        0      805 2024-03-05 18:21:35.930419 dlt-0.4.9a1/dlt/common/configuration/providers/airflow.py
+-rw-r--r--   0        0        0     1129 2024-01-24 17:23:08.486518 dlt-0.4.9a1/dlt/common/configuration/providers/context.py
+-rw-r--r--   0        0        0     1346 2024-01-24 17:23:08.486518 dlt-0.4.9a1/dlt/common/configuration/providers/dictionary.py
+-rw-r--r--   0        0        0     1995 2024-01-24 17:23:08.486518 dlt-0.4.9a1/dlt/common/configuration/providers/environ.py
+-rw-r--r--   0        0        0     5141 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/configuration/providers/google_secrets.py
+-rw-r--r--   0        0        0     1319 2024-01-24 17:23:08.486518 dlt-0.4.9a1/dlt/common/configuration/providers/provider.py
+-rw-r--r--   0        0        0    13416 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/configuration/providers/toml.py
+-rw-r--r--   0        0        0    20983 2024-04-09 13:29:46.170457 dlt-0.4.9a1/dlt/common/configuration/resolve.py
+-rw-r--r--   0        0        0     1742 2024-01-24 17:23:08.486518 dlt-0.4.9a1/dlt/common/configuration/specs/__init__.py
+-rw-r--r--   0        0        0     1836 2024-04-09 13:29:46.170457 dlt-0.4.9a1/dlt/common/configuration/specs/api_credentials.py
+-rw-r--r--   0        0        0     5263 2024-04-09 13:29:46.170457 dlt-0.4.9a1/dlt/common/configuration/specs/aws_credentials.py
+-rw-r--r--   0        0        0     2591 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/configuration/specs/azure_credentials.py
+-rw-r--r--   0        0        0    18147 2024-04-11 11:44:50.568746 dlt-0.4.9a1/dlt/common/configuration/specs/base_configuration.py
+-rw-r--r--   0        0        0     6498 2024-04-09 13:29:46.170457 dlt-0.4.9a1/dlt/common/configuration/specs/config_providers_context.py
+-rw-r--r--   0        0        0     3456 2024-04-09 13:29:46.170457 dlt-0.4.9a1/dlt/common/configuration/specs/config_section_context.py
+-rw-r--r--   0        0        0     2339 2024-04-09 13:29:46.170457 dlt-0.4.9a1/dlt/common/configuration/specs/connection_string_credentials.py
+-rw-r--r--   0        0        0     2667 2024-01-24 17:23:08.486518 dlt-0.4.9a1/dlt/common/configuration/specs/exceptions.py
+-rw-r--r--   0        0        0    13349 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/configuration/specs/gcp_credentials.py
+-rw-r--r--   0        0        0      874 2024-04-09 13:29:46.170457 dlt-0.4.9a1/dlt/common/configuration/specs/known_sections.py
+-rw-r--r--   0        0        0     2856 2024-04-09 13:29:46.170457 dlt-0.4.9a1/dlt/common/configuration/specs/run_configuration.py
+-rw-r--r--   0        0        0     6650 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/configuration/utils.py
+-rw-r--r--   0        0        0      220 2024-01-24 17:23:08.486518 dlt-0.4.9a1/dlt/common/data_types/__init__.py
+-rw-r--r--   0        0        0     6832 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/data_types/type_helpers.py
+-rw-r--r--   0        0        0      269 2024-01-24 17:23:08.486518 dlt-0.4.9a1/dlt/common/data_types/typing.py
+-rw-r--r--   0        0        0      754 2024-04-16 09:06:12.375886 dlt-0.4.9a1/dlt/common/data_writers/__init__.py
+-rw-r--r--   0        0        0    10766 2024-04-16 09:06:12.375886 dlt-0.4.9a1/dlt/common/data_writers/buffered.py
+-rw-r--r--   0        0        0     5665 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/data_writers/escape.py
+-rw-r--r--   0        0        0     2894 2024-04-16 09:06:12.375886 dlt-0.4.9a1/dlt/common/data_writers/exceptions.py
+-rw-r--r--   0        0        0    27064 2024-04-16 09:06:12.375886 dlt-0.4.9a1/dlt/common/data_writers/writers.py
+-rw-r--r--   0        0        0      483 2024-04-16 09:06:12.375886 dlt-0.4.9a1/dlt/common/destination/__init__.py
+-rw-r--r--   0        0        0     5375 2024-04-16 09:06:12.375886 dlt-0.4.9a1/dlt/common/destination/capabilities.py
+-rw-r--r--   0        0        0     5132 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/common/destination/exceptions.py
+-rw-r--r--   0        0        0    25485 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/destination/reference.py
+-rw-r--r--   0        0        0     6274 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/common/exceptions.py
+-rw-r--r--   0        0        0     5149 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/git.py
+-rw-r--r--   0        0        0     7099 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/json/__init__.py
+-rw-r--r--   0        0        0     1814 2024-02-16 18:38:47.332466 dlt-0.4.9a1/dlt/common/json/_orjson.py
+-rw-r--r--   0        0        0     2948 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/json/_simplejson.py
+-rw-r--r--   0        0        0     1562 2023-11-18 17:38:04.257189 dlt-0.4.9a1/dlt/common/jsonpath.py
+-rw-r--r--   0        0        0        0 2023-11-18 17:38:04.257189 dlt-0.4.9a1/dlt/common/libs/__init__.py
+-rw-r--r--   0        0        0      181 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/libs/numpy.py
+-rw-r--r--   0        0        0      436 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/libs/pandas.py
+-rw-r--r--   0        0        0      217 2024-04-07 14:59:43.715656 dlt-0.4.9a1/dlt/common/libs/pandas_sql.py
+-rw-r--r--   0        0        0    14934 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/libs/pyarrow.py
+-rw-r--r--   0        0        0    15624 2024-02-27 21:03:24.137544 dlt-0.4.9a1/dlt/common/libs/pydantic.py
+-rw-r--r--   0        0        0    15486 2024-03-08 19:36:32.669855 dlt-0.4.9a1/dlt/common/libs/sql_alchemy.py
+-rw-r--r--   0        0        0     3652 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/common/logger.py
+-rw-r--r--   0        0        0      854 2024-03-01 09:52:05.856761 dlt-0.4.9a1/dlt/common/managed_thread_pool.py
+-rw-r--r--   0        0        0      384 2024-03-18 14:01:48.098768 dlt-0.4.9a1/dlt/common/normalizers/__init__.py
+-rw-r--r--   0        0        0     1408 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/common/normalizers/configuration.py
+-rw-r--r--   0        0        0      510 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/normalizers/exceptions.py
+-rw-r--r--   0        0        0     1905 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/normalizers/json/__init__.py
+-rw-r--r--   0        0        0    16970 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/normalizers/json/relational.py
+-rw-r--r--   0        0        0      123 2024-03-18 14:01:48.098768 dlt-0.4.9a1/dlt/common/normalizers/naming/__init__.py
+-rw-r--r--   0        0        0      810 2024-02-27 21:03:24.137544 dlt-0.4.9a1/dlt/common/normalizers/naming/direct.py
+-rw-r--r--   0        0        0      798 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/normalizers/naming/duck_case.py
+-rw-r--r--   0        0        0      830 2024-03-18 14:01:48.098768 dlt-0.4.9a1/dlt/common/normalizers/naming/exceptions.py
+-rw-r--r--   0        0        0     4570 2024-03-18 14:01:48.098768 dlt-0.4.9a1/dlt/common/normalizers/naming/naming.py
+-rw-r--r--   0        0        0     2967 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/normalizers/naming/snake_case.py
+-rw-r--r--   0        0        0      359 2024-03-18 14:01:48.108768 dlt-0.4.9a1/dlt/common/normalizers/typing.py
+-rw-r--r--   0        0        0     3426 2024-04-07 14:59:43.715656 dlt-0.4.9a1/dlt/common/normalizers/utils.py
+-rw-r--r--   0        0        0      461 2024-02-27 21:03:24.137544 dlt-0.4.9a1/dlt/common/pendulum.py
+-rw-r--r--   0        0        0    31127 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/pipeline.py
+-rw-r--r--   0        0        0        0 2023-11-18 17:38:04.267189 dlt-0.4.9a1/dlt/common/reflection/__init__.py
+-rw-r--r--   0        0        0      375 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/reflection/function_visitor.py
+-rw-r--r--   0        0        0     6119 2024-04-07 14:59:43.715656 dlt-0.4.9a1/dlt/common/reflection/spec.py
+-rw-r--r--   0        0        0     5103 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/reflection/utils.py
+-rw-r--r--   0        0        0      329 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/runners/__init__.py
+-rw-r--r--   0        0        0      665 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/common/runners/configuration.py
+-rw-r--r--   0        0        0     3678 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/runners/pool_runner.py
+-rw-r--r--   0        0        0     4132 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/runners/runnable.py
+-rw-r--r--   0        0        0     3162 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/runners/stdout.py
+-rw-r--r--   0        0        0     2137 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/runners/synth_pickle.py
+-rw-r--r--   0        0        0      105 2023-11-18 17:38:04.267189 dlt-0.4.9a1/dlt/common/runners/typing.py
+-rw-r--r--   0        0        0     5583 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/runners/venv.py
+-rw-r--r--   0        0        0       71 2023-11-18 17:38:04.267189 dlt-0.4.9a1/dlt/common/runtime/__init__.py
+-rw-r--r--   0        0        0    14599 2024-04-13 11:30:10.760740 dlt-0.4.9a1/dlt/common/runtime/collector.py
+-rw-r--r--   0        0        0     5461 2024-01-25 20:07:33.363195 dlt-0.4.9a1/dlt/common/runtime/exec_info.py
+-rw-r--r--   0        0        0     1067 2024-04-13 11:30:15.860741 dlt-0.4.9a1/dlt/common/runtime/init.py
+-rw-r--r--   0        0        0     6616 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/runtime/json_logging.py
+-rw-r--r--   0        0        0     2044 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/runtime/prometheus.py
+-rw-r--r--   0        0        0     6702 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/runtime/segment.py
+-rw-r--r--   0        0        0     2784 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/runtime/sentry.py
+-rw-r--r--   0        0        0     1938 2024-04-13 11:30:29.100742 dlt-0.4.9a1/dlt/common/runtime/signals.py
+-rw-r--r--   0        0        0      613 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/runtime/slack.py
+-rw-r--r--   0        0        0     2960 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/runtime/telemetry.py
+-rw-r--r--   0        0        0      579 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/runtime/typing.py
+-rw-r--r--   0        0        0      805 2024-01-24 17:23:08.496518 dlt-0.4.9a1/dlt/common/schema/__init__.py
+-rw-r--r--   0        0        0     2454 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/schema/detections.py
+-rw-r--r--   0        0        0     5308 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/schema/exceptions.py
+-rw-r--r--   0        0        0     5269 2024-03-18 14:01:48.108768 dlt-0.4.9a1/dlt/common/schema/migrations.py
+-rw-r--r--   0        0        0    42497 2024-04-15 15:36:23.382155 dlt-0.4.9a1/dlt/common/schema/schema.py
+-rw-r--r--   0        0        0     5865 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/common/schema/typing.py
+-rw-r--r--   0        0        0    28875 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/common/schema/utils.py
+-rw-r--r--   0        0        0     1672 2024-02-10 23:59:00.181729 dlt-0.4.9a1/dlt/common/source.py
+-rw-r--r--   0        0        0     1224 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/common/storages/__init__.py
+-rw-r--r--   0        0        0     4869 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/common/storages/configuration.py
+-rw-r--r--   0        0        0     4175 2024-04-16 09:06:12.375886 dlt-0.4.9a1/dlt/common/storages/data_item_storage.py
+-rw-r--r--   0        0        0     4184 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/common/storages/exceptions.py
+-rw-r--r--   0        0        0    14242 2024-01-24 17:23:08.506518 dlt-0.4.9a1/dlt/common/storages/file_storage.py
+-rw-r--r--   0        0        0    11065 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/common/storages/fsspec_filesystem.py
+-rw-r--r--   0        0        0        0 2024-02-26 22:08:47.270507 dlt-0.4.9a1/dlt/common/storages/fsspecs/__init__.py
+-rw-r--r--   0        0        0    20479 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/common/storages/fsspecs/google_drive.py
+-rw-r--r--   0        0        0     3513 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/common/storages/live_schema_storage.py
+-rw-r--r--   0        0        0    26784 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/common/storages/load_package.py
+-rw-r--r--   0        0        0     9920 2024-04-16 09:06:12.375886 dlt-0.4.9a1/dlt/common/storages/load_storage.py
+-rw-r--r--   0        0        0     3197 2024-04-07 14:59:43.715656 dlt-0.4.9a1/dlt/common/storages/normalize_storage.py
+-rw-r--r--   0        0        0     9551 2024-04-15 17:18:10.812104 dlt-0.4.9a1/dlt/common/storages/schema_storage.py
+-rw-r--r--   0        0        0     9065 2024-01-24 17:23:08.506518 dlt-0.4.9a1/dlt/common/storages/transactional_file.py
+-rw-r--r--   0        0        0     2867 2024-01-24 17:23:08.506518 dlt-0.4.9a1/dlt/common/storages/versioned_storage.py
+-rw-r--r--   0        0        0     7604 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/common/time.py
+-rw-r--r--   0        0        0     8878 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/common/typing.py
+-rw-r--r--   0        0        0    19596 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/common/utils.py
+-rw-r--r--   0        0        0     7978 2024-04-07 14:59:43.715656 dlt-0.4.9a1/dlt/common/validation.py
+-rw-r--r--   0        0        0     2369 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/common/versioned_state.py
+-rw-r--r--   0        0        0     5528 2024-01-24 17:23:08.506518 dlt-0.4.9a1/dlt/common/warnings.py
+-rw-r--r--   0        0        0     1219 2024-01-24 17:23:08.506518 dlt-0.4.9a1/dlt/common/wei.py
+-rw-r--r--   0        0        0     1217 2024-04-11 11:44:50.568746 dlt-0.4.9a1/dlt/destinations/__init__.py
+-rw-r--r--   0        0        0      404 2024-02-27 21:03:24.137544 dlt-0.4.9a1/dlt/destinations/adapters.py
+-rw-r--r--   0        0        0     4856 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/destinations/decorators.py
+-rw-r--r--   0        0        0     6070 2024-04-16 09:06:12.375886 dlt-0.4.9a1/dlt/destinations/exceptions.py
+-rw-r--r--   0        0        0        0 2024-01-24 17:23:08.506518 dlt-0.4.9a1/dlt/destinations/impl/__init__.py
+-rw-r--r--   0        0        0     1311 2024-03-18 14:01:48.108768 dlt-0.4.9a1/dlt/destinations/impl/athena/__init__.py
+-rw-r--r--   0        0        0    18693 2024-04-13 11:31:25.760744 dlt-0.4.9a1/dlt/destinations/impl/athena/athena.py
+-rw-r--r--   0        0        0     1054 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/destinations/impl/athena/configuration.py
+-rw-r--r--   0        0        0     2169 2024-01-24 17:23:08.506518 dlt-0.4.9a1/dlt/destinations/impl/athena/factory.py
+-rw-r--r--   0        0        0      439 2024-02-27 21:03:24.137544 dlt-0.4.9a1/dlt/destinations/impl/bigquery/README.md
+-rw-r--r--   0        0        0     1118 2024-03-18 14:01:48.108768 dlt-0.4.9a1/dlt/destinations/impl/bigquery/__init__.py
+-rw-r--r--   0        0        0    21073 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/destinations/impl/bigquery/bigquery.py
+-rw-r--r--   0        0        0     8397 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/bigquery/bigquery_adapter.py
+-rw-r--r--   0        0        0     1740 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/bigquery/configuration.py
+-rw-r--r--   0        0        0     1309 2024-02-07 18:59:43.276965 dlt-0.4.9a1/dlt/destinations/impl/bigquery/factory.py
+-rw-r--r--   0        0        0    10772 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/bigquery/sql_client.py
+-rw-r--r--   0        0        0     1430 2024-03-18 14:01:48.118769 dlt-0.4.9a1/dlt/destinations/impl/databricks/__init__.py
+-rw-r--r--   0        0        0     2043 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/destinations/impl/databricks/configuration.py
+-rw-r--r--   0        0        0    13640 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/databricks/databricks.py
+-rw-r--r--   0        0        0     1741 2024-02-07 18:59:43.276965 dlt-0.4.9a1/dlt/destinations/impl/databricks/factory.py
+-rw-r--r--   0        0        0     6074 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/destinations/impl/databricks/sql_client.py
+-rw-r--r--   0        0        0      673 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/destination/__init__.py
+-rw-r--r--   0        0        0     1047 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/destination/configuration.py
+-rw-r--r--   0        0        0     3675 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/destination/destination.py
+-rw-r--r--   0        0        0     5626 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/destinations/impl/destination/factory.py
+-rw-r--r--   0        0        0     1243 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/dremio/__init__.py
+-rw-r--r--   0        0        0     1617 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/dremio/configuration.py
+-rw-r--r--   0        0        0     8692 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/dremio/dremio.py
+-rw-r--r--   0        0        0     1787 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/dremio/factory.py
+-rw-r--r--   0        0        0     9314 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/dremio/pydremio.py
+-rw-r--r--   0        0        0     5934 2024-04-13 11:31:52.880745 dlt-0.4.9a1/dlt/destinations/impl/dremio/sql_client.py
+-rw-r--r--   0        0        0     1236 2024-03-18 14:01:48.118769 dlt-0.4.9a1/dlt/destinations/impl/duckdb/__init__.py
+-rw-r--r--   0        0        0     9013 2024-04-13 11:31:56.870745 dlt-0.4.9a1/dlt/destinations/impl/duckdb/configuration.py
+-rw-r--r--   0        0        0     7022 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/duckdb/duck.py
+-rw-r--r--   0        0        0     1969 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/duckdb/factory.py
+-rw-r--r--   0        0        0     6828 2024-04-05 22:42:00.549456 dlt-0.4.9a1/dlt/destinations/impl/duckdb/sql_client.py
+-rw-r--r--   0        0        0     1485 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/dummy/__init__.py
+-rw-r--r--   0        0        0     1027 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/destinations/impl/dummy/configuration.py
+-rw-r--r--   0        0        0     6693 2024-04-16 09:06:12.375886 dlt-0.4.9a1/dlt/destinations/impl/dummy/dummy.py
+-rw-r--r--   0        0        0     1111 2024-02-23 11:16:27.641941 dlt-0.4.9a1/dlt/destinations/impl/dummy/factory.py
+-rw-r--r--   0        0        0      194 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/filesystem/__init__.py
+-rw-r--r--   0        0        0     1712 2024-04-16 09:06:12.375886 dlt-0.4.9a1/dlt/destinations/impl/filesystem/configuration.py
+-rw-r--r--   0        0        0     2411 2024-03-24 19:55:58.511453 dlt-0.4.9a1/dlt/destinations/impl/filesystem/factory.py
+-rw-r--r--   0        0        0     9541 2024-04-16 09:06:12.385886 dlt-0.4.9a1/dlt/destinations/impl/filesystem/filesystem.py
+-rw-r--r--   0        0        0      790 2024-04-16 09:06:12.385886 dlt-0.4.9a1/dlt/destinations/impl/filesystem/typing.py
+-rw-r--r--   0        0        0     1134 2024-03-18 14:01:48.118769 dlt-0.4.9a1/dlt/destinations/impl/motherduck/__init__.py
+-rw-r--r--   0        0        0     3111 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/motherduck/configuration.py
+-rw-r--r--   0        0        0     1966 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/motherduck/factory.py
+-rw-r--r--   0        0        0      911 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/motherduck/motherduck.py
+-rw-r--r--   0        0        0     1515 2024-03-18 14:01:48.118769 dlt-0.4.9a1/dlt/destinations/impl/motherduck/sql_client.py
+-rw-r--r--   0        0        0      253 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/mssql/README.md
+-rw-r--r--   0        0        0     1385 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/mssql/__init__.py
+-rw-r--r--   0        0        0     3971 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/destinations/impl/mssql/configuration.py
+-rw-r--r--   0        0        0     1764 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/mssql/factory.py
+-rw-r--r--   0        0        0     7537 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/mssql/mssql.py
+-rw-r--r--   0        0        0     6629 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/mssql/sql_client.py
+-rw-r--r--   0        0        0      251 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/postgres/README.md
+-rw-r--r--   0        0        0     1356 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/postgres/__init__.py
+-rw-r--r--   0        0        0     1794 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/destinations/impl/postgres/configuration.py
+-rw-r--r--   0        0        0     1840 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/postgres/factory.py
+-rw-r--r--   0        0        0     6940 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/postgres/postgres.py
+-rw-r--r--   0        0        0     5678 2024-03-31 18:13:49.090176 dlt-0.4.9a1/dlt/destinations/impl/postgres/sql_client.py
+-rw-r--r--   0        0        0      677 2024-03-18 14:01:48.118769 dlt-0.4.9a1/dlt/destinations/impl/qdrant/__init__.py
+-rw-r--r--   0        0        0     3044 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/destinations/impl/qdrant/configuration.py
+-rw-r--r--   0        0        0     1146 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/qdrant/factory.py
+-rw-r--r--   0        0        0     1831 2024-02-07 18:59:43.276965 dlt-0.4.9a1/dlt/destinations/impl/qdrant/qdrant_adapter.py
+-rw-r--r--   0        0        0    17960 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/destinations/impl/qdrant/qdrant_client.py
+-rw-r--r--   0        0        0     1159 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/redshift/README.md
+-rw-r--r--   0        0        0     1181 2024-03-18 14:01:48.118769 dlt-0.4.9a1/dlt/destinations/impl/redshift/__init__.py
+-rw-r--r--   0        0        0     1005 2024-04-09 13:29:46.180457 dlt-0.4.9a1/dlt/destinations/impl/redshift/configuration.py
+-rw-r--r--   0        0        0     2006 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/redshift/factory.py
+-rw-r--r--   0        0        0    10832 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/redshift/redshift.py
+-rw-r--r--   0        0        0     1218 2024-03-18 14:01:48.118769 dlt-0.4.9a1/dlt/destinations/impl/snowflake/__init__.py
+-rw-r--r--   0        0        0     5449 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/destinations/impl/snowflake/configuration.py
+-rw-r--r--   0        0        0     2008 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/snowflake/factory.py
+-rw-r--r--   0        0        0    11468 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/snowflake/snowflake.py
+-rw-r--r--   0        0        0     6885 2024-03-18 14:01:48.118769 dlt-0.4.9a1/dlt/destinations/impl/snowflake/sql_client.py
+-rw-r--r--   0        0        0     2851 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/synapse/__init__.py
+-rw-r--r--   0        0        0     2746 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/destinations/impl/synapse/configuration.py
+-rw-r--r--   0        0        0     2640 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/destinations/impl/synapse/factory.py
+-rw-r--r--   0        0        0     1179 2024-02-07 18:59:43.276965 dlt-0.4.9a1/dlt/destinations/impl/synapse/sql_client.py
+-rw-r--r--   0        0        0    13201 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/impl/synapse/synapse.py
+-rw-r--r--   0        0        0     2231 2024-03-08 19:36:32.679855 dlt-0.4.9a1/dlt/destinations/impl/synapse/synapse_adapter.py
+-rw-r--r--   0        0        0      526 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/weaviate/README.md
+-rw-r--r--   0        0        0      752 2024-03-18 14:01:48.118769 dlt-0.4.9a1/dlt/destinations/impl/weaviate/__init__.py
+-rw-r--r--   0        0        0      280 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/weaviate/ci_naming.py
+-rw-r--r--   0        0        0     2009 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/destinations/impl/weaviate/configuration.py
+-rw-r--r--   0        0        0      666 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/destinations/impl/weaviate/exceptions.py
+-rw-r--r--   0        0        0     1935 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/weaviate/factory.py
+-rw-r--r--   0        0        0     3259 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/impl/weaviate/naming.py
+-rw-r--r--   0        0        0     3914 2024-02-07 18:59:43.276965 dlt-0.4.9a1/dlt/destinations/impl/weaviate/weaviate_adapter.py
+-rw-r--r--   0        0        0    26468 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/destinations/impl/weaviate/weaviate_client.py
+-rw-r--r--   0        0        0     6149 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/insert_job_client.py
+-rw-r--r--   0        0        0    23940 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/destinations/job_client_impl.py
+-rw-r--r--   0        0        0     6300 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/destinations/job_impl.py
+-rw-r--r--   0        0        0     8366 2024-04-16 09:06:12.385886 dlt-0.4.9a1/dlt/destinations/path_utils.py
+-rw-r--r--   0        0        0     9279 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/destinations/sql_client.py
+-rw-r--r--   0        0        0    26428 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/destinations/sql_jobs.py
+-rw-r--r--   0        0        0     4895 2024-02-27 21:03:24.137544 dlt-0.4.9a1/dlt/destinations/type_mapping.py
+-rw-r--r--   0        0        0     1877 2024-01-24 17:23:08.516518 dlt-0.4.9a1/dlt/destinations/typing.py
+-rw-r--r--   0        0        0      506 2024-04-11 11:44:50.568746 dlt-0.4.9a1/dlt/destinations/utils.py
+-rw-r--r--   0        0        0      639 2024-04-07 14:59:43.715656 dlt-0.4.9a1/dlt/extract/__init__.py
+-rw-r--r--   0        0        0     8539 2024-03-08 19:36:32.679855 dlt-0.4.9a1/dlt/extract/concurrency.py
+-rw-r--r--   0        0        0    35950 2024-04-15 15:36:23.392155 dlt-0.4.9a1/dlt/extract/decorators.py
+-rw-r--r--   0        0        0    16480 2024-03-08 19:36:32.679855 dlt-0.4.9a1/dlt/extract/exceptions.py
+-rw-r--r--   0        0        0    17697 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/extract/extract.py
+-rw-r--r--   0        0        0    15690 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/extract/extractors.py
+-rw-r--r--   0        0        0    21382 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/extract/hints.py
+-rw-r--r--   0        0        0    29587 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/extract/incremental/__init__.py
+-rw-r--r--   0        0        0     1142 2024-01-24 17:23:08.526518 dlt-0.4.9a1/dlt/extract/incremental/exceptions.py
+-rw-r--r--   0        0        0    14951 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/extract/incremental/transform.py
+-rw-r--r--   0        0        0      322 2024-01-24 17:23:08.526518 dlt-0.4.9a1/dlt/extract/incremental/typing.py
+-rw-r--r--   0        0        0     6786 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/extract/items.py
+-rw-r--r--   0        0        0    16368 2024-03-08 19:36:32.679855 dlt-0.4.9a1/dlt/extract/pipe.py
+-rw-r--r--   0        0        0    16344 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/extract/pipe_iterator.py
+-rw-r--r--   0        0        0    26683 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/extract/resource.py
+-rw-r--r--   0        0        0    19990 2024-03-18 14:01:48.118769 dlt-0.4.9a1/dlt/extract/source.py
+-rw-r--r--   0        0        0     4650 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/extract/storage.py
+-rw-r--r--   0        0        0    10122 2024-04-09 20:42:07.310460 dlt-0.4.9a1/dlt/extract/utils.py
+-rw-r--r--   0        0        0     3500 2024-03-08 19:36:32.679855 dlt-0.4.9a1/dlt/extract/validation.py
+-rw-r--r--   0        0        0      832 2024-04-07 14:59:43.715656 dlt-0.4.9a1/dlt/extract/wrappers.py
+-rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.4.9a1/dlt/helpers/__init__.py
+-rw-r--r--   0        0        0    23547 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/helpers/airflow_helper.py
+-rw-r--r--   0        0        0     3701 2024-01-24 17:23:08.526518 dlt-0.4.9a1/dlt/helpers/dbt/__init__.py
+-rw-r--r--   0        0        0     1241 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/helpers/dbt/configuration.py
+-rw-r--r--   0        0        0     6848 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/helpers/dbt/dbt_utils.py
+-rw-r--r--   0        0        0      772 2024-01-24 17:23:08.526518 dlt-0.4.9a1/dlt/helpers/dbt/exceptions.py
+-rw-r--r--   0        0        0     7163 2024-02-07 18:59:43.286965 dlt-0.4.9a1/dlt/helpers/dbt/profiles.yml
+-rw-r--r--   0        0        0    15742 2024-04-13 11:33:15.710743 dlt-0.4.9a1/dlt/helpers/dbt/runner.py
+-rw-r--r--   0        0        0     4881 2023-11-18 17:38:04.277189 dlt-0.4.9a1/dlt/helpers/dbt_cloud/__init__.py
+-rw-r--r--   0        0        0     4926 2024-01-24 17:23:08.526518 dlt-0.4.9a1/dlt/helpers/dbt_cloud/client.py
+-rw-r--r--   0        0        0      623 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/helpers/dbt_cloud/configuration.py
+-rw-r--r--   0        0        0      349 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/helpers/streamlit_app/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 14:59:43.715656 dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/__init__.py
+-rw-r--r--   0        0        0     1239 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/load_info.py
+-rw-r--r--   0        0        0      483 2024-04-07 14:59:43.715656 dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/menu.py
+-rw-r--r--   0        0        0     2451 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/query.py
+-rw-r--r--   0        0        0     1139 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/resource_state.py
+-rw-r--r--   0        0        0      618 2024-04-07 14:59:43.715656 dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/show_data.py
+-rw-r--r--   0        0        0     2842 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/table_hints.py
+-rw-r--r--   0        0        0      150 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/index.py
+-rw-r--r--   0        0        0        0 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/pages/__init__.py
+-rw-r--r--   0        0        0     1668 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/pages/dashboard.py
+-rw-r--r--   0        0        0     4446 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/pages/load_info.py
+-rw-r--r--   0        0        0      757 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/theme.py
+-rw-r--r--   0        0        0     2361 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/helpers/streamlit_app/utils.py
+-rw-r--r--   0        0        0      386 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/__init__.py
+-rw-r--r--   0        0        0      901 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/color_mode_selector.py
+-rw-r--r--   0        0        0     1004 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/logo.py
+-rw-r--r--   0        0        0      613 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/schema.py
+-rw-r--r--   0        0        0     1542 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/stats.py
+-rw-r--r--   0        0        0      805 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/summary.py
+-rw-r--r--   0        0        0     1189 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/tags.py
+-rw-r--r--   0        0        0       51 2023-11-18 17:38:04.277189 dlt-0.4.9a1/dlt/load/__init__.py
+-rw-r--r--   0        0        0      807 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/load/configuration.py
+-rw-r--r--   0        0        0     2061 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/load/exceptions.py
+-rw-r--r--   0        0        0    25029 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/load/load.py
+-rw-r--r--   0        0        0     8096 2024-04-13 11:33:36.000744 dlt-0.4.9a1/dlt/load/utils.py
+-rw-r--r--   0        0        0       58 2024-01-24 17:23:08.526518 dlt-0.4.9a1/dlt/normalize/__init__.py
+-rw-r--r--   0        0        0     1598 2024-04-16 09:06:12.385886 dlt-0.4.9a1/dlt/normalize/configuration.py
+-rw-r--r--   0        0        0      644 2024-04-09 20:42:07.320460 dlt-0.4.9a1/dlt/normalize/exceptions.py
+-rw-r--r--   0        0        0    18280 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/normalize/items_normalizers.py
+-rw-r--r--   0        0        0    23745 2024-04-16 09:06:12.385886 dlt-0.4.9a1/dlt/normalize/normalize.py
+-rw-r--r--   0        0        0    15006 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/pipeline/__init__.py
+-rw-r--r--   0        0        0     2097 2024-04-09 20:42:07.320460 dlt-0.4.9a1/dlt/pipeline/configuration.py
+-rw-r--r--   0        0        0      709 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/pipeline/current.py
+-rw-r--r--   0        0        0     4950 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/pipeline/dbt.py
+-rw-r--r--   0        0        0     4599 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/pipeline/exceptions.py
+-rw-r--r--   0        0        0     9785 2024-04-09 20:42:07.320460 dlt-0.4.9a1/dlt/pipeline/helpers.py
+-rw-r--r--   0        0        0      212 2024-04-07 14:59:43.725656 dlt-0.4.9a1/dlt/pipeline/mark.py
+-rw-r--r--   0        0        0    72369 2024-04-16 09:06:12.385886 dlt-0.4.9a1/dlt/pipeline/pipeline.py
+-rw-r--r--   0        0        0     3864 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/pipeline/platform.py
+-rw-r--r--   0        0        0     1007 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/pipeline/progress.py
+-rw-r--r--   0        0        0     4856 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/pipeline/state_sync.py
+-rw-r--r--   0        0        0    13259 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/pipeline/trace.py
+-rw-r--r--   0        0        0     5610 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/pipeline/track.py
+-rw-r--r--   0        0        0       92 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/pipeline/typing.py
+-rw-r--r--   0        0        0      796 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/pipeline/warnings.py
+-rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.4.9a1/dlt/py.typed
+-rw-r--r--   0        0        0        0 2023-11-18 17:38:04.277189 dlt-0.4.9a1/dlt/reflection/__init__.py
+-rw-r--r--   0        0        0      565 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/reflection/names.py
+-rw-r--r--   0        0        0     5818 2024-04-13 11:34:58.380741 dlt-0.4.9a1/dlt/reflection/script_inspector.py
+-rw-r--r--   0        0        0     6278 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/reflection/script_visitor.py
+-rw-r--r--   0        0        0      417 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/sources/__init__.py
+-rw-r--r--   0        0        0      110 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/sources/config.py
+-rw-r--r--   0        0        0      790 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/sources/credentials.py
+-rw-r--r--   0        0        0      200 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/sources/filesystem.py
+-rw-r--r--   0        0        0        0 2023-11-18 17:38:04.277189 dlt-0.4.9a1/dlt/sources/helpers/__init__.py
+-rw-r--r--   0        0        0     1291 2024-04-09 20:42:07.320460 dlt-0.4.9a1/dlt/sources/helpers/requests/__init__.py
+-rw-r--r--   0        0        0    10965 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/sources/helpers/requests/retry.py
+-rw-r--r--   0        0        0     1969 2024-01-24 17:23:08.536518 dlt-0.4.9a1/dlt/sources/helpers/requests/session.py
+-rw-r--r--   0        0        0      234 2023-11-18 17:38:04.277189 dlt-0.4.9a1/dlt/sources/helpers/requests/typing.py
+-rw-r--r--   0        0        0     1210 2024-04-13 11:26:19.690742 dlt-0.4.9a1/dlt/sources/helpers/rest_client/__init__.py
+-rw-r--r--   0        0        0     7190 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/sources/helpers/rest_client/auth.py
+-rw-r--r--   0        0        0     9181 2024-04-15 15:36:23.402155 dlt-0.4.9a1/dlt/sources/helpers/rest_client/client.py
+-rw-r--r--   0        0        0     4456 2024-04-13 22:20:19.334997 dlt-0.4.9a1/dlt/sources/helpers/rest_client/detector.py
+-rw-r--r--   0        0        0      103 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/sources/helpers/rest_client/exceptions.py
+-rw-r--r--   0        0        0     6001 2024-04-13 22:20:19.334997 dlt-0.4.9a1/dlt/sources/helpers/rest_client/paginators.py
+-rw-r--r--   0        0        0      426 2024-04-13 22:20:19.334997 dlt-0.4.9a1/dlt/sources/helpers/rest_client/typing.py
+-rw-r--r--   0        0        0      406 2024-04-09 13:29:46.190457 dlt-0.4.9a1/dlt/sources/helpers/rest_client/utils.py
+-rw-r--r--   0        0        0     4860 2024-04-15 15:36:23.412155 dlt-0.4.9a1/dlt/sources/helpers/transform.py
+-rw-r--r--   0        0        0     1130 2024-04-15 15:36:23.412155 dlt-0.4.9a1/dlt/version.py
+-rw-r--r--   0        0        0     7009 2024-04-16 09:07:01.515887 dlt-0.4.9a1/pyproject.toml
+-rw-r--r--   0        0        0     9936 1970-01-01 00:00:00.000000 dlt-0.4.9a1/PKG-INFO
```

### Comparing `dlt-0.4.9a0/LICENSE.txt` & `dlt-0.4.9a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/README.md` & `dlt-0.4.9a1/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/__init__.py` & `dlt-0.4.9a1/dlt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/cli/_dlt.py` & `dlt-0.4.9a1/dlt/cli/_dlt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/cli/config_toml_writer.py` & `dlt-0.4.9a1/dlt/cli/config_toml_writer.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/cli/deploy_command.py` & `dlt-0.4.9a1/dlt/cli/deploy_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/cli/deploy_command_helpers.py` & `dlt-0.4.9a1/dlt/cli/deploy_command_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/cli/echo.py` & `dlt-0.4.9a1/dlt/cli/echo.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/cli/init_command.py` & `dlt-0.4.9a1/dlt/cli/init_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/cli/pipeline_command.py` & `dlt-0.4.9a1/dlt/cli/pipeline_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/cli/pipeline_files.py` & `dlt-0.4.9a1/dlt/cli/pipeline_files.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/cli/requirements.py` & `dlt-0.4.9a1/dlt/cli/requirements.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/cli/source_detection.py` & `dlt-0.4.9a1/dlt/cli/source_detection.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/cli/telemetry_command.py` & `dlt-0.4.9a1/dlt/cli/telemetry_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/cli/utils.py` & `dlt-0.4.9a1/dlt/cli/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/arithmetics.py` & `dlt-0.4.9a1/dlt/common/arithmetics.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/__init__.py` & `dlt-0.4.9a1/dlt/common/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/accessors.py` & `dlt-0.4.9a1/dlt/common/configuration/accessors.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/container.py` & `dlt-0.4.9a1/dlt/common/configuration/container.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/exceptions.py` & `dlt-0.4.9a1/dlt/common/configuration/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/inject.py` & `dlt-0.4.9a1/dlt/common/configuration/inject.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/paths.py` & `dlt-0.4.9a1/dlt/common/configuration/paths.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/providers/__init__.py` & `dlt-0.4.9a1/dlt/common/configuration/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/providers/airflow.py` & `dlt-0.4.9a1/dlt/common/configuration/providers/airflow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/providers/context.py` & `dlt-0.4.9a1/dlt/common/configuration/providers/context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/providers/dictionary.py` & `dlt-0.4.9a1/dlt/common/configuration/providers/dictionary.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/providers/environ.py` & `dlt-0.4.9a1/dlt/common/configuration/providers/environ.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/providers/google_secrets.py` & `dlt-0.4.9a1/dlt/common/configuration/providers/google_secrets.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/providers/provider.py` & `dlt-0.4.9a1/dlt/common/configuration/providers/provider.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/providers/toml.py` & `dlt-0.4.9a1/dlt/common/configuration/providers/toml.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/resolve.py` & `dlt-0.4.9a1/dlt/common/configuration/resolve.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/specs/__init__.py` & `dlt-0.4.9a1/dlt/common/configuration/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/specs/api_credentials.py` & `dlt-0.4.9a1/dlt/common/configuration/specs/api_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/specs/aws_credentials.py` & `dlt-0.4.9a1/dlt/common/configuration/specs/aws_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/specs/azure_credentials.py` & `dlt-0.4.9a1/dlt/common/configuration/specs/azure_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/specs/base_configuration.py` & `dlt-0.4.9a1/dlt/common/configuration/specs/base_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/specs/config_providers_context.py` & `dlt-0.4.9a1/dlt/common/configuration/specs/config_providers_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/specs/config_section_context.py` & `dlt-0.4.9a1/dlt/common/configuration/specs/config_section_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/specs/connection_string_credentials.py` & `dlt-0.4.9a1/dlt/common/configuration/specs/connection_string_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/specs/exceptions.py` & `dlt-0.4.9a1/dlt/common/configuration/specs/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/specs/gcp_credentials.py` & `dlt-0.4.9a1/dlt/common/configuration/specs/gcp_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/specs/known_sections.py` & `dlt-0.4.9a1/dlt/common/configuration/specs/known_sections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/specs/run_configuration.py` & `dlt-0.4.9a1/dlt/common/configuration/specs/run_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/configuration/utils.py` & `dlt-0.4.9a1/dlt/common/configuration/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/data_types/type_helpers.py` & `dlt-0.4.9a1/dlt/common/data_types/type_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/data_writers/__init__.py` & `dlt-0.4.9a1/dlt/common/data_writers/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 from dlt.common.data_writers.writers import (
     DataWriter,
     DataWriterMetrics,
     TDataItemFormat,
     FileWriterSpec,
+    resolve_best_writer_spec,
+    get_best_writer_spec,
+    is_native_writer,
 )
 from dlt.common.data_writers.buffered import BufferedDataWriter, new_file_id
 from dlt.common.data_writers.escape import (
     escape_redshift_literal,
     escape_redshift_identifier,
     escape_bigquery_identifier,
 )
 
 __all__ = [
     "DataWriter",
     "FileWriterSpec",
+    "resolve_best_writer_spec",
+    "get_best_writer_spec",
+    "is_native_writer",
     "DataWriterMetrics",
     "TDataItemFormat",
     "BufferedDataWriter",
     "new_file_id",
     "escape_redshift_literal",
     "escape_redshift_identifier",
     "escape_bigquery_identifier",
```

### Comparing `dlt-0.4.9a0/dlt/common/data_writers/buffered.py` & `dlt-0.4.9a1/dlt/common/data_writers/buffered.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,15 @@
         file_max_bytes: int = None,
         disable_compression: bool = False,
         _caps: DestinationCapabilitiesContext = None
     ):
         self.writer_spec = writer_spec
         if self.writer_spec.requires_destination_capabilities and not _caps:
             raise DestinationCapabilitiesRequired(self.writer_spec.file_format)
-        self.writer_cls = DataWriter.class_factory(
-            writer_spec.file_format, writer_spec.data_item_format
-        )
+        self.writer_cls = DataWriter.writer_class_from_spec(writer_spec)
         self._supports_schema_changes = self.writer_spec.supports_schema_changes
         self._caps = _caps
         # validate if template has correct placeholders
         self.file_name_template = file_name_template
         self.closed_files: List[DataWriterMetrics] = []  # all fully processed files
         # buffered items must be less than max items in file
         self.buffer_max_items = min(buffer_max_items, file_max_items or buffer_max_items)
```

### Comparing `dlt-0.4.9a0/dlt/common/data_writers/escape.py` & `dlt-0.4.9a1/dlt/common/data_writers/escape.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/data_writers/writers.py` & `dlt-0.4.9a1/dlt/common/data_writers/writers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import abc
 import csv
-from dataclasses import dataclass
 from typing import (
     IO,
     TYPE_CHECKING,
     Any,
     ClassVar,
     Dict,
     List,
@@ -16,29 +15,34 @@
     NamedTuple,
     TypeVar,
 )
 
 from dlt.common.json import json
 from dlt.common.configuration import configspec, known_sections, with_config
 from dlt.common.configuration.specs import BaseConfiguration
-from dlt.common.data_writers.exceptions import DataWriterNotFound, InvalidDataItem
+from dlt.common.data_writers.exceptions import (
+    SpecLookupFailed,
+    DataWriterNotFound,
+    FileFormatForItemFormatNotFound,
+    FileSpecNotFound,
+    InvalidDataItem,
+)
 from dlt.common.destination import DestinationCapabilitiesContext, TLoaderFileFormat
 from dlt.common.schema.typing import TTableSchemaColumns
 from dlt.common.typing import StrAny
 
 if TYPE_CHECKING:
     from dlt.common.libs.pyarrow import pyarrow as pa
 
 
 TDataItemFormat = Literal["arrow", "object"]
 TWriter = TypeVar("TWriter", bound="DataWriter")
 
 
-@dataclass
-class FileWriterSpec:
+class FileWriterSpec(NamedTuple):
     file_format: TLoaderFileFormat
     """format of the output file"""
     data_item_format: TDataItemFormat
     """format of the input data"""
     file_extension: str
     is_binary_format: bool
     supports_schema_changes: Literal["True", "Buffer", "False"]
@@ -101,41 +105,50 @@
     def from_file_format(
         cls,
         file_format: TLoaderFileFormat,
         data_item_format: TDataItemFormat,
         f: IO[Any],
         caps: DestinationCapabilitiesContext = None,
     ) -> "DataWriter":
-        return cls.class_factory(file_format, data_item_format)(f, caps)
+        return cls.class_factory(file_format, data_item_format, ALL_WRITERS)(f, caps)
 
     @classmethod
     def writer_spec_from_file_format(
         cls, file_format: TLoaderFileFormat, data_item_format: TDataItemFormat
     ) -> FileWriterSpec:
-        return cls.class_factory(file_format, data_item_format).writer_spec()
+        return cls.class_factory(file_format, data_item_format, ALL_WRITERS).writer_spec()
 
     @classmethod
     def item_format_from_file_extension(cls, extension: str) -> TDataItemFormat:
         """Simple heuristic to get data item format from file extension"""
         if extension == "typed-jsonl":
             return "object"
         elif extension == "parquet":
             return "arrow"
         else:
             raise ValueError(f"Cannot figure out data item format for extension {extension}")
 
     @staticmethod
+    def writer_class_from_spec(spec: FileWriterSpec) -> Type["DataWriter"]:
+        try:
+            return WRITER_SPECS[spec]
+        except KeyError:
+            raise FileSpecNotFound(spec.file_format, spec.data_item_format, spec)
+
+    @staticmethod
     def class_factory(
-        file_format: TLoaderFileFormat, data_item_format: TDataItemFormat
+        file_format: TLoaderFileFormat,
+        data_item_format: TDataItemFormat,
+        writers: Sequence[Type["DataWriter"]],
     ) -> Type["DataWriter"]:
-        for writer in ALL_WRITERS:
+        for writer in writers:
             spec = writer.writer_spec()
             if spec.file_format == file_format and spec.data_item_format == data_item_format:
                 return writer
-        raise DataWriterNotFound(file_format, data_item_format)
+        raise FileFormatForItemFormatNotFound(file_format, data_item_format)
 
 
 class JsonlWriter(DataWriter):
     def write_data(self, rows: Sequence[Any]) -> None:
         super().write_data(rows)
         for row in rows:
             json.dump(row, self._f)
@@ -597,16 +610,15 @@
         for batch in rows:
             # convert to object data item format
             super().write_data(batch.to_pylist())  # type: ignore[misc]
 
     @staticmethod
     def convert_spec(base: Type[DataWriter]) -> FileWriterSpec:
         spec = base.writer_spec()
-        spec.data_item_format = "arrow"
-        return spec
+        return spec._replace(data_item_format="arrow")
 
 
 class ArrowToInsertValuesWriter(ArrowToObjectAdapter, InsertValuesWriter):
     @classmethod
     def writer_spec(cls) -> FileWriterSpec:
         return cls.convert_spec(InsertValuesWriter)
 
@@ -619,20 +631,111 @@
 
 class ArrowToTypedJsonlListWriter(ArrowToObjectAdapter, TypedJsonlListWriter):
     @classmethod
     def writer_spec(cls) -> FileWriterSpec:
         return cls.convert_spec(TypedJsonlListWriter)
 
 
-# ArrowToCsvWriter
+def is_native_writer(writer_type: Type[DataWriter]) -> bool:
+    """Checks if writer has adapter mixin. Writers with adapters are not native and typically
+    decrease the performance.
+    """
+    # we only have arrow adapters now
+    return not issubclass(writer_type, ArrowToObjectAdapter)
+
+
 ALL_WRITERS: List[Type[DataWriter]] = [
     JsonlWriter,
     TypedJsonlListWriter,
     InsertValuesWriter,
     ParquetDataWriter,
     CsvWriter,
     ArrowToParquetWriter,
     ArrowToInsertValuesWriter,
     ArrowToJsonlWriter,
     ArrowToTypedJsonlListWriter,
     ArrowToCsvWriter,
 ]
+
+WRITER_SPECS: Dict[FileWriterSpec, Type[DataWriter]] = {
+    writer.writer_spec(): writer for writer in ALL_WRITERS
+}
+
+NATIVE_FORMAT_WRITERS: Dict[TDataItemFormat, Tuple[Type[DataWriter], ...]] = {
+    # all "object" writers are native object writers (no adapters yet)
+    "object": tuple(
+        writer
+        for writer in ALL_WRITERS
+        if writer.writer_spec().data_item_format == "object" and is_native_writer(writer)
+    ),
+    # exclude arrow adapters
+    "arrow": tuple(
+        writer
+        for writer in ALL_WRITERS
+        if writer.writer_spec().data_item_format == "arrow" and is_native_writer(writer)
+    ),
+}
+
+
+def resolve_best_writer_spec(
+    item_format: TDataItemFormat,
+    possible_file_formats: Sequence[TLoaderFileFormat],
+    preferred_format: TLoaderFileFormat = None,
+) -> FileWriterSpec:
+    """Finds best writer for `item_format` out of `possible_file_formats`. Tries `preferred_format` first.
+    Best possible writer is a native writer for `item_format` writing files in `preferred_format`.
+    If not found, any native writer for `possible_file_formats` is picked.
+    Native writer supports `item_format` directly without a need to convert to other item formats.
+    """
+    native_writers = NATIVE_FORMAT_WRITERS[item_format]
+    # check if preferred format has native item_format writer
+    if preferred_format:
+        if preferred_format not in possible_file_formats:
+            raise ValueError(
+                f"Preferred format {preferred_format} not possible in {possible_file_formats}"
+            )
+        try:
+            return DataWriter.class_factory(
+                preferred_format, item_format, native_writers
+            ).writer_spec()
+        except DataWriterNotFound:
+            pass
+    # if not found, use scan native file formats for item format
+    for supported_format in possible_file_formats:
+        if supported_format != preferred_format:
+            try:
+                return DataWriter.class_factory(
+                    supported_format, item_format, native_writers
+                ).writer_spec()
+            except DataWriterNotFound:
+                pass
+
+    # search all writers
+    if preferred_format:
+        try:
+            return DataWriter.class_factory(
+                preferred_format, item_format, ALL_WRITERS
+            ).writer_spec()
+        except DataWriterNotFound:
+            pass
+
+    for supported_format in possible_file_formats:
+        if supported_format != preferred_format:
+            try:
+                return DataWriter.class_factory(
+                    supported_format, item_format, ALL_WRITERS
+                ).writer_spec()
+            except DataWriterNotFound:
+                pass
+
+    raise SpecLookupFailed(item_format, possible_file_formats, preferred_format)
+
+
+def get_best_writer_spec(
+    item_format: TDataItemFormat, file_format: TLoaderFileFormat
+) -> FileWriterSpec:
+    """Gets writer for `item_format` writing files in {file_format}. Looks for native writer first"""
+    native_writers = NATIVE_FORMAT_WRITERS[item_format]
+    try:
+        return DataWriter.class_factory(file_format, item_format, native_writers).writer_spec()
+    except DataWriterNotFound:
+        return DataWriter.class_factory(file_format, item_format, ALL_WRITERS).writer_spec()
```

### Comparing `dlt-0.4.9a0/dlt/common/destination/exceptions.py` & `dlt-0.4.9a1/dlt/common/destination/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/destination/reference.py` & `dlt-0.4.9a1/dlt/common/destination/reference.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/exceptions.py` & `dlt-0.4.9a1/dlt/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/git.py` & `dlt-0.4.9a1/dlt/common/git.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/json/__init__.py` & `dlt-0.4.9a1/dlt/common/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/json/_orjson.py` & `dlt-0.4.9a1/dlt/common/json/_orjson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/json/_simplejson.py` & `dlt-0.4.9a1/dlt/common/json/_simplejson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/jsonpath.py` & `dlt-0.4.9a1/dlt/common/jsonpath.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/libs/pyarrow.py` & `dlt-0.4.9a1/dlt/common/libs/pyarrow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/libs/pydantic.py` & `dlt-0.4.9a1/dlt/common/libs/pydantic.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/libs/sql_alchemy.py` & `dlt-0.4.9a1/dlt/common/libs/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/logger.py` & `dlt-0.4.9a1/dlt/common/logger.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/managed_thread_pool.py` & `dlt-0.4.9a1/dlt/common/managed_thread_pool.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/normalizers/configuration.py` & `dlt-0.4.9a1/dlt/common/normalizers/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/normalizers/json/__init__.py` & `dlt-0.4.9a1/dlt/common/normalizers/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/normalizers/json/relational.py` & `dlt-0.4.9a1/dlt/common/normalizers/json/relational.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/normalizers/naming/direct.py` & `dlt-0.4.9a1/dlt/common/normalizers/naming/direct.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/normalizers/naming/duck_case.py` & `dlt-0.4.9a1/dlt/common/normalizers/naming/duck_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/normalizers/naming/exceptions.py` & `dlt-0.4.9a1/dlt/common/normalizers/naming/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/normalizers/naming/naming.py` & `dlt-0.4.9a1/dlt/common/normalizers/naming/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/normalizers/naming/snake_case.py` & `dlt-0.4.9a1/dlt/common/normalizers/naming/snake_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/normalizers/utils.py` & `dlt-0.4.9a1/dlt/common/normalizers/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/pipeline.py` & `dlt-0.4.9a1/dlt/common/pipeline.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/reflection/spec.py` & `dlt-0.4.9a1/dlt/common/reflection/spec.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/reflection/utils.py` & `dlt-0.4.9a1/dlt/common/reflection/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/runners/configuration.py` & `dlt-0.4.9a1/dlt/common/runners/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/runners/pool_runner.py` & `dlt-0.4.9a1/dlt/common/runners/pool_runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/runners/runnable.py` & `dlt-0.4.9a1/dlt/common/runners/runnable.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/runners/stdout.py` & `dlt-0.4.9a1/dlt/common/runners/stdout.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/runners/synth_pickle.py` & `dlt-0.4.9a1/dlt/common/runners/synth_pickle.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/runners/venv.py` & `dlt-0.4.9a1/dlt/common/runners/venv.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/runtime/collector.py` & `dlt-0.4.9a1/dlt/common/runtime/collector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/runtime/exec_info.py` & `dlt-0.4.9a1/dlt/common/runtime/exec_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/runtime/init.py` & `dlt-0.4.9a1/dlt/common/runtime/init.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/runtime/json_logging.py` & `dlt-0.4.9a1/dlt/common/runtime/json_logging.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/runtime/prometheus.py` & `dlt-0.4.9a1/dlt/common/runtime/prometheus.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/runtime/segment.py` & `dlt-0.4.9a1/dlt/common/runtime/segment.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/runtime/sentry.py` & `dlt-0.4.9a1/dlt/common/runtime/sentry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/runtime/signals.py` & `dlt-0.4.9a1/dlt/common/runtime/signals.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/runtime/slack.py` & `dlt-0.4.9a1/dlt/common/runtime/slack.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/runtime/telemetry.py` & `dlt-0.4.9a1/dlt/common/runtime/telemetry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/runtime/typing.py` & `dlt-0.4.9a1/dlt/common/runtime/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/schema/__init__.py` & `dlt-0.4.9a1/dlt/common/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/schema/detections.py` & `dlt-0.4.9a1/dlt/common/schema/detections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/schema/exceptions.py` & `dlt-0.4.9a1/dlt/common/schema/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/schema/migrations.py` & `dlt-0.4.9a1/dlt/common/schema/migrations.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/schema/schema.py` & `dlt-0.4.9a1/dlt/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/schema/typing.py` & `dlt-0.4.9a1/dlt/common/schema/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/schema/utils.py` & `dlt-0.4.9a1/dlt/common/schema/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/source.py` & `dlt-0.4.9a1/dlt/common/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/storages/__init__.py` & `dlt-0.4.9a1/dlt/common/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/storages/configuration.py` & `dlt-0.4.9a1/dlt/common/storages/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/storages/data_item_storage.py` & `dlt-0.4.9a1/dlt/common/storages/data_item_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,15 @@
     FileWriterSpec,
 )
 
 
 class DataItemStorage(ABC):
     def __init__(self, writer_spec: FileWriterSpec, *args: Any) -> None:
         self.writer_spec = writer_spec
-        self.writer_cls = DataWriter.class_factory(
-            writer_spec.file_format, writer_spec.data_item_format
-        )
+        self.writer_cls = DataWriter.writer_class_from_spec(writer_spec)
         self.buffered_writers: Dict[str, BufferedDataWriter[DataWriter]] = {}
         super().__init__(*args)
 
     def _get_writer(
         self, load_id: str, schema_name: str, table_name: str
     ) -> BufferedDataWriter[DataWriter]:
         # unique writer id
```

### Comparing `dlt-0.4.9a0/dlt/common/storages/exceptions.py` & `dlt-0.4.9a1/dlt/common/storages/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/storages/file_storage.py` & `dlt-0.4.9a1/dlt/common/storages/file_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/storages/fsspec_filesystem.py` & `dlt-0.4.9a1/dlt/common/storages/fsspec_filesystem.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/storages/fsspecs/google_drive.py` & `dlt-0.4.9a1/dlt/common/storages/fsspecs/google_drive.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/storages/live_schema_storage.py` & `dlt-0.4.9a1/dlt/common/storages/live_schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/storages/load_package.py` & `dlt-0.4.9a1/dlt/common/storages/load_package.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/storages/load_storage.py` & `dlt-0.4.9a1/dlt/common/storages/load_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,36 +78,16 @@
         )
 
     def initialize_storage(self) -> None:
         self.storage.create_folder(LoadStorage.NEW_PACKAGES_FOLDER, exists_ok=True)
         self.storage.create_folder(LoadStorage.NORMALIZED_FOLDER, exists_ok=True)
         self.storage.create_folder(LoadStorage.LOADED_FOLDER, exists_ok=True)
 
-    def create_item_storage(
-        self, preferred_format: TLoaderFileFormat, item_format: TDataItemFormat
-    ) -> DataItemStorage:
-        """Creates item storage for preferred_format + item_format combination. If not found, it
-        tries the remaining file formats in supported formats.
-        """
-        try:
-            return LoadItemStorage(
-                self.new_packages,
-                DataWriter.writer_spec_from_file_format(preferred_format, item_format),
-            )
-        except DataWriterNotFound:
-            for supported_format in self.supported_loader_file_formats:
-                if supported_format != preferred_format:
-                    try:
-                        return LoadItemStorage(
-                            self.new_packages,
-                            DataWriter.writer_spec_from_file_format(supported_format, item_format),
-                        )
-                    except DataWriterNotFound:
-                        pass
-            raise
+    def create_item_storage(self, writer_spec: FileWriterSpec) -> DataItemStorage:
+        return LoadItemStorage(self.new_packages, writer_spec)
 
     def import_extracted_package(
         self, load_id: str, extract_package_storage: PackageStorage
     ) -> None:
         # pass the original state
         self.new_packages.create_package(
             load_id, extract_package_storage.get_load_package_state(load_id)
```

### Comparing `dlt-0.4.9a0/dlt/common/storages/normalize_storage.py` & `dlt-0.4.9a1/dlt/common/storages/normalize_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/storages/schema_storage.py` & `dlt-0.4.9a1/dlt/common/storages/schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/storages/transactional_file.py` & `dlt-0.4.9a1/dlt/common/storages/transactional_file.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/storages/versioned_storage.py` & `dlt-0.4.9a1/dlt/common/storages/versioned_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/time.py` & `dlt-0.4.9a1/dlt/common/time.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/typing.py` & `dlt-0.4.9a1/dlt/common/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/utils.py` & `dlt-0.4.9a1/dlt/common/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/validation.py` & `dlt-0.4.9a1/dlt/common/validation.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/versioned_state.py` & `dlt-0.4.9a1/dlt/common/versioned_state.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/warnings.py` & `dlt-0.4.9a1/dlt/common/warnings.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/common/wei.py` & `dlt-0.4.9a1/dlt/common/wei.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/__init__.py` & `dlt-0.4.9a1/dlt/destinations/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/decorators.py` & `dlt-0.4.9a1/dlt/destinations/decorators.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/exceptions.py` & `dlt-0.4.9a1/dlt/destinations/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -108,17 +108,50 @@
             " to write your own materialization. The reason is:\n"
         )
         msg += reason
         super().__init__(msg)
 
 
 class InvalidFilesystemLayout(DestinationTerminalException):
-    def __init__(self, invalid_placeholders: Sequence[str]) -> None:
+    def __init__(
+        self,
+        layout: str,
+        expected_placeholders: Sequence[str],
+        extra_placeholders: Sequence[str],
+        invalid_placeholders: Sequence[str],
+        unused_placeholders: Sequence[str],
+    ) -> None:
         self.invalid_placeholders = invalid_placeholders
-        super().__init__(f"Invalid placeholders found in filesystem layout: {invalid_placeholders}")
+        self.extra_placeholders = extra_placeholders
+        self.expected_placeholders = expected_placeholders
+        self.unused_placeholders = unused_placeholders
+        self.layout = layout
+
+        message = (
+            f"Layout '{layout}' expected {', '.join(expected_placeholders)} placeholders."
+            f"Missing placeholders: {', '.join(invalid_placeholders)}."
+        )
+
+        if extra_placeholders:
+            message += f"Extra placeholders specified: {', '.join(extra_placeholders)}."
+
+        if unused_placeholders:
+            message += f"Unused placeholders: {', '.join(unused_placeholders)}."
+
+        super().__init__(message)
+
+
+class InvalidPlaceholderCallback(DestinationTransientException):
+    def __init__(self, callback_name: str) -> None:
+        self.callback_name = callback_name
+        super().__init__(
+            f"Invalid placeholder callback: {callback_name}, please make sure it can"
+            " accept parameters the following `schema name`, `table name`,"
+            " `load_id`, `file_id` and an `extension`",
+        )
 
 
 class CantExtractTablePrefix(DestinationTerminalException):
     def __init__(self, layout: str, details: str) -> None:
         msg = f"Cannot extract unique table prefix in layout '{layout}'. "
         msg += details
         msg += "An example of valid layout: {table_name}/{load_id}.{file_id}.{ext}"
```

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/athena/__init__.py` & `dlt-0.4.9a1/dlt/destinations/impl/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/athena/athena.py` & `dlt-0.4.9a1/dlt/destinations/impl/athena/athena.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/athena/configuration.py` & `dlt-0.4.9a1/dlt/destinations/impl/athena/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/athena/factory.py` & `dlt-0.4.9a1/dlt/destinations/impl/athena/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/bigquery/__init__.py` & `dlt-0.4.9a1/dlt/destinations/impl/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/bigquery/bigquery.py` & `dlt-0.4.9a1/dlt/destinations/impl/bigquery/bigquery.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/bigquery/bigquery_adapter.py` & `dlt-0.4.9a1/dlt/destinations/impl/bigquery/bigquery_adapter.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/bigquery/configuration.py` & `dlt-0.4.9a1/dlt/destinations/impl/bigquery/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/bigquery/factory.py` & `dlt-0.4.9a1/dlt/destinations/impl/bigquery/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/bigquery/sql_client.py` & `dlt-0.4.9a1/dlt/destinations/impl/bigquery/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/databricks/__init__.py` & `dlt-0.4.9a1/dlt/destinations/impl/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/databricks/configuration.py` & `dlt-0.4.9a1/dlt/destinations/impl/databricks/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/databricks/databricks.py` & `dlt-0.4.9a1/dlt/destinations/impl/databricks/databricks.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/databricks/factory.py` & `dlt-0.4.9a1/dlt/destinations/impl/databricks/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/databricks/sql_client.py` & `dlt-0.4.9a1/dlt/destinations/impl/databricks/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/destination/__init__.py` & `dlt-0.4.9a1/dlt/destinations/impl/destination/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/destination/configuration.py` & `dlt-0.4.9a1/dlt/destinations/impl/destination/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/destination/destination.py` & `dlt-0.4.9a1/dlt/destinations/impl/destination/destination.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/destination/factory.py` & `dlt-0.4.9a1/dlt/destinations/impl/destination/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/dremio/__init__.py` & `dlt-0.4.9a1/dlt/destinations/impl/dremio/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/dremio/configuration.py` & `dlt-0.4.9a1/dlt/destinations/impl/dremio/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/dremio/dremio.py` & `dlt-0.4.9a1/dlt/destinations/impl/dremio/dremio.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/dremio/factory.py` & `dlt-0.4.9a1/dlt/destinations/impl/dremio/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/dremio/pydremio.py` & `dlt-0.4.9a1/dlt/destinations/impl/dremio/pydremio.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/dremio/sql_client.py` & `dlt-0.4.9a1/dlt/destinations/impl/dremio/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/duckdb/__init__.py` & `dlt-0.4.9a1/dlt/destinations/impl/duckdb/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/duckdb/configuration.py` & `dlt-0.4.9a1/dlt/destinations/impl/duckdb/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/duckdb/duck.py` & `dlt-0.4.9a1/dlt/destinations/impl/duckdb/duck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/duckdb/factory.py` & `dlt-0.4.9a1/dlt/destinations/impl/duckdb/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/duckdb/sql_client.py` & `dlt-0.4.9a1/dlt/destinations/impl/duckdb/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/dummy/__init__.py` & `dlt-0.4.9a1/dlt/destinations/impl/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/dummy/configuration.py` & `dlt-0.4.9a1/dlt/destinations/impl/dummy/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/dummy/dummy.py` & `dlt-0.4.9a1/dlt/destinations/impl/dummy/dummy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from contextlib import contextmanager
 import random
+from contextlib import contextmanager
 from copy import copy
 from types import TracebackType
 from typing import (
     ClassVar,
-    ContextManager,
     Dict,
     Iterator,
     Optional,
     Sequence,
     Type,
     Iterable,
     List,
```

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/dummy/factory.py` & `dlt-0.4.9a1/dlt/destinations/impl/dummy/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/filesystem/factory.py` & `dlt-0.4.9a1/dlt/destinations/impl/filesystem/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/filesystem/filesystem.py` & `dlt-0.4.9a1/dlt/destinations/impl/filesystem/filesystem.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import posixpath
 import os
 from types import TracebackType
 from typing import ClassVar, List, Type, Iterable, Set, Iterator
 from fsspec import AbstractFileSystem
 from contextlib import contextmanager
 
+import dlt
 from dlt.common import logger
 from dlt.common.schema import Schema, TSchemaTables, TTableSchema
-from dlt.common.storages import FileStorage, ParsedLoadJobFileName, fsspec_from_config
+from dlt.common.storages import FileStorage, fsspec_from_config
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.destination.reference import (
     NewLoadJob,
     TLoadJobState,
     LoadJob,
     JobClientBase,
     FollowupJob,
@@ -34,40 +35,38 @@
         config: FilesystemDestinationClientConfiguration,
         schema_name: str,
         load_id: str,
     ) -> None:
         file_name = FileStorage.get_file_name_from_file_path(local_path)
         self.config = config
         self.dataset_path = dataset_path
-        self.destination_file_name = LoadFilesystemJob.make_destination_filename(
-            config.layout, file_name, schema_name, load_id
+        self.destination_file_name = path_utils.create_path(
+            config.layout,
+            file_name,
+            schema_name,
+            load_id,
+            current_datetime=config.current_datetime,
+            load_package_timestamp=dlt.current.load_package()["state"]["created_at"],  # type: ignore
+            extra_placeholders=config.extra_placeholders,
         )
 
         super().__init__(file_name)
         fs_client, _ = fsspec_from_config(config)
-        self.destination_file_name = LoadFilesystemJob.make_destination_filename(
-            config.layout, file_name, schema_name, load_id
+        self.destination_file_name = path_utils.create_path(
+            config.layout,
+            file_name,
+            schema_name,
+            load_id,
+            current_datetime=config.current_datetime,
+            load_package_timestamp=dlt.current.load_package()["state"]["created_at"],  # type: ignore
+            extra_placeholders=config.extra_placeholders,
         )
         item = self.make_remote_path()
         fs_client.put_file(local_path, item)
 
-    @staticmethod
-    def make_destination_filename(
-        layout: str, file_name: str, schema_name: str, load_id: str
-    ) -> str:
-        job_info = ParsedLoadJobFileName.parse(file_name)
-        return path_utils.create_path(
-            layout,
-            schema_name=schema_name,
-            table_name=job_info.table_name,
-            load_id=load_id,
-            file_id=job_info.file_id,
-            ext=job_info.file_format,
-        )
-
     def make_remote_path(self) -> str:
         return (
             f"{self.config.protocol}://{posixpath.join(self.dataset_path, self.destination_file_name)}"
         )
 
     def state(self) -> TLoadJobState:
         return "completed"
```

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/motherduck/__init__.py` & `dlt-0.4.9a1/dlt/destinations/impl/motherduck/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/motherduck/configuration.py` & `dlt-0.4.9a1/dlt/destinations/impl/motherduck/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/motherduck/factory.py` & `dlt-0.4.9a1/dlt/destinations/impl/motherduck/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/motherduck/motherduck.py` & `dlt-0.4.9a1/dlt/destinations/impl/motherduck/motherduck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/motherduck/sql_client.py` & `dlt-0.4.9a1/dlt/destinations/impl/motherduck/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/mssql/__init__.py` & `dlt-0.4.9a1/dlt/destinations/impl/mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/mssql/configuration.py` & `dlt-0.4.9a1/dlt/destinations/impl/mssql/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/mssql/factory.py` & `dlt-0.4.9a1/dlt/destinations/impl/mssql/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/mssql/mssql.py` & `dlt-0.4.9a1/dlt/destinations/impl/mssql/mssql.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/mssql/sql_client.py` & `dlt-0.4.9a1/dlt/destinations/impl/mssql/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/postgres/__init__.py` & `dlt-0.4.9a1/dlt/destinations/impl/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/postgres/configuration.py` & `dlt-0.4.9a1/dlt/destinations/impl/postgres/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/postgres/factory.py` & `dlt-0.4.9a1/dlt/destinations/impl/postgres/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/postgres/postgres.py` & `dlt-0.4.9a1/dlt/destinations/impl/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/postgres/sql_client.py` & `dlt-0.4.9a1/dlt/destinations/impl/postgres/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/qdrant/__init__.py` & `dlt-0.4.9a1/dlt/destinations/impl/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/qdrant/configuration.py` & `dlt-0.4.9a1/dlt/destinations/impl/qdrant/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/qdrant/factory.py` & `dlt-0.4.9a1/dlt/destinations/impl/qdrant/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/qdrant/qdrant_adapter.py` & `dlt-0.4.9a1/dlt/destinations/impl/qdrant/qdrant_adapter.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/qdrant/qdrant_client.py` & `dlt-0.4.9a1/dlt/destinations/impl/qdrant/qdrant_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/redshift/README.md` & `dlt-0.4.9a1/dlt/destinations/impl/redshift/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/redshift/__init__.py` & `dlt-0.4.9a1/dlt/destinations/impl/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/redshift/configuration.py` & `dlt-0.4.9a1/dlt/destinations/impl/redshift/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/redshift/factory.py` & `dlt-0.4.9a1/dlt/destinations/impl/redshift/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/redshift/redshift.py` & `dlt-0.4.9a1/dlt/destinations/impl/redshift/redshift.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/snowflake/__init__.py` & `dlt-0.4.9a1/dlt/destinations/impl/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/snowflake/configuration.py` & `dlt-0.4.9a1/dlt/destinations/impl/snowflake/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/snowflake/factory.py` & `dlt-0.4.9a1/dlt/destinations/impl/snowflake/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/snowflake/snowflake.py` & `dlt-0.4.9a1/dlt/destinations/impl/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/snowflake/sql_client.py` & `dlt-0.4.9a1/dlt/destinations/impl/snowflake/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/synapse/__init__.py` & `dlt-0.4.9a1/dlt/destinations/impl/synapse/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/synapse/configuration.py` & `dlt-0.4.9a1/dlt/destinations/impl/synapse/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/synapse/factory.py` & `dlt-0.4.9a1/dlt/destinations/impl/synapse/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/synapse/sql_client.py` & `dlt-0.4.9a1/dlt/destinations/impl/synapse/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/synapse/synapse.py` & `dlt-0.4.9a1/dlt/destinations/impl/synapse/synapse.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/synapse/synapse_adapter.py` & `dlt-0.4.9a1/dlt/destinations/impl/synapse/synapse_adapter.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/weaviate/README.md` & `dlt-0.4.9a1/dlt/destinations/impl/weaviate/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/weaviate/__init__.py` & `dlt-0.4.9a1/dlt/destinations/impl/weaviate/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/weaviate/configuration.py` & `dlt-0.4.9a1/dlt/destinations/impl/weaviate/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/weaviate/exceptions.py` & `dlt-0.4.9a1/dlt/destinations/impl/weaviate/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/weaviate/factory.py` & `dlt-0.4.9a1/dlt/destinations/impl/weaviate/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/weaviate/naming.py` & `dlt-0.4.9a1/dlt/destinations/impl/weaviate/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/weaviate/weaviate_adapter.py` & `dlt-0.4.9a1/dlt/destinations/impl/weaviate/weaviate_adapter.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/impl/weaviate/weaviate_client.py` & `dlt-0.4.9a1/dlt/destinations/impl/weaviate/weaviate_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/insert_job_client.py` & `dlt-0.4.9a1/dlt/destinations/insert_job_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/job_client_impl.py` & `dlt-0.4.9a1/dlt/destinations/job_client_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/job_impl.py` & `dlt-0.4.9a1/dlt/destinations/job_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/sql_client.py` & `dlt-0.4.9a1/dlt/destinations/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/sql_jobs.py` & `dlt-0.4.9a1/dlt/destinations/sql_jobs.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/type_mapping.py` & `dlt-0.4.9a1/dlt/destinations/type_mapping.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/destinations/typing.py` & `dlt-0.4.9a1/dlt/destinations/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/extract/__init__.py` & `dlt-0.4.9a1/dlt/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/extract/concurrency.py` & `dlt-0.4.9a1/dlt/extract/concurrency.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/extract/decorators.py` & `dlt-0.4.9a1/dlt/extract/decorators.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/extract/exceptions.py` & `dlt-0.4.9a1/dlt/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/extract/extract.py` & `dlt-0.4.9a1/dlt/extract/extract.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/extract/extractors.py` & `dlt-0.4.9a1/dlt/extract/extractors.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/extract/hints.py` & `dlt-0.4.9a1/dlt/extract/hints.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/extract/incremental/__init__.py` & `dlt-0.4.9a1/dlt/extract/incremental/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/extract/incremental/exceptions.py` & `dlt-0.4.9a1/dlt/extract/incremental/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/extract/incremental/transform.py` & `dlt-0.4.9a1/dlt/extract/incremental/transform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/extract/items.py` & `dlt-0.4.9a1/dlt/extract/items.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/extract/pipe.py` & `dlt-0.4.9a1/dlt/extract/pipe.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/extract/pipe_iterator.py` & `dlt-0.4.9a1/dlt/extract/pipe_iterator.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/extract/resource.py` & `dlt-0.4.9a1/dlt/extract/resource.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/extract/source.py` & `dlt-0.4.9a1/dlt/extract/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/extract/storage.py` & `dlt-0.4.9a1/dlt/extract/storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/extract/utils.py` & `dlt-0.4.9a1/dlt/extract/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/extract/validation.py` & `dlt-0.4.9a1/dlt/extract/validation.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/extract/wrappers.py` & `dlt-0.4.9a1/dlt/extract/wrappers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/airflow_helper.py` & `dlt-0.4.9a1/dlt/helpers/airflow_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/dbt/__init__.py` & `dlt-0.4.9a1/dlt/helpers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/dbt/configuration.py` & `dlt-0.4.9a1/dlt/helpers/dbt/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/dbt/dbt_utils.py` & `dlt-0.4.9a1/dlt/helpers/dbt/dbt_utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/dbt/exceptions.py` & `dlt-0.4.9a1/dlt/helpers/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/dbt/profiles.yml` & `dlt-0.4.9a1/dlt/helpers/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/dbt/runner.py` & `dlt-0.4.9a1/dlt/helpers/dbt/runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/dbt_cloud/__init__.py` & `dlt-0.4.9a1/dlt/helpers/dbt_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/dbt_cloud/client.py` & `dlt-0.4.9a1/dlt/helpers/dbt_cloud/client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/dbt_cloud/configuration.py` & `dlt-0.4.9a1/dlt/helpers/dbt_cloud/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/load_info.py` & `dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/load_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/query.py` & `dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/query.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/resource_state.py` & `dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/resource_state.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/show_data.py` & `dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/show_data.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/table_hints.py` & `dlt-0.4.9a1/dlt/helpers/streamlit_app/blocks/table_hints.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/streamlit_app/pages/dashboard.py` & `dlt-0.4.9a1/dlt/helpers/streamlit_app/pages/dashboard.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/streamlit_app/pages/load_info.py` & `dlt-0.4.9a1/dlt/helpers/streamlit_app/pages/load_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/streamlit_app/theme.py` & `dlt-0.4.9a1/dlt/helpers/streamlit_app/theme.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/streamlit_app/utils.py` & `dlt-0.4.9a1/dlt/helpers/streamlit_app/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/color_mode_selector.py` & `dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/color_mode_selector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/logo.py` & `dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/logo.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/schema.py` & `dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/stats.py` & `dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/stats.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/summary.py` & `dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/summary.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/tags.py` & `dlt-0.4.9a1/dlt/helpers/streamlit_app/widgets/tags.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/load/configuration.py` & `dlt-0.4.9a1/dlt/load/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/load/exceptions.py` & `dlt-0.4.9a1/dlt/load/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/load/load.py` & `dlt-0.4.9a1/dlt/load/load.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/load/utils.py` & `dlt-0.4.9a1/dlt/load/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/normalize/configuration.py` & `dlt-0.4.9a1/dlt/normalize/configuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from typing import TYPE_CHECKING
+from typing import Optional
 
 from dlt.common.configuration import configspec
 from dlt.common.configuration.specs import BaseConfiguration
-from dlt.common.destination import DestinationCapabilitiesContext
+from dlt.common.destination import DestinationCapabilitiesContext, TLoaderFileFormat
 from dlt.common.runners.configuration import PoolRunnerConfiguration, TPoolType
 from dlt.common.storages import (
     LoadStorageConfiguration,
     NormalizeStorageConfiguration,
     SchemaStorageConfiguration,
 )
 
@@ -19,14 +19,15 @@
     """When true, items to be normalized will have `_dlt_load_id` column added with the current load ID."""
 
 
 @configspec
 class NormalizeConfiguration(PoolRunnerConfiguration):
     pool_type: TPoolType = "process"
     destination_capabilities: DestinationCapabilitiesContext = None  # injectable
+    loader_file_format: Optional[TLoaderFileFormat] = None
     _schema_storage_config: SchemaStorageConfiguration = None
     _normalize_storage_config: NormalizeStorageConfiguration = None
     _load_storage_config: LoadStorageConfiguration = None
 
     json_normalizer: ItemsNormalizerConfiguration = ItemsNormalizerConfiguration(
         add_dlt_id=True, add_dlt_load_id=True
     )
```

### Comparing `dlt-0.4.9a0/dlt/normalize/exceptions.py` & `dlt-0.4.9a1/dlt/normalize/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/normalize/items_normalizers.py` & `dlt-0.4.9a1/dlt/normalize/items_normalizers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/normalize/normalize.py` & `dlt-0.4.9a1/dlt/normalize/normalize.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,22 @@
 from concurrent.futures import Future, Executor
 
 from dlt.common import logger
 from dlt.common.runtime.signals import sleep
 from dlt.common.configuration import with_config, known_sections
 from dlt.common.configuration.accessors import config
 from dlt.common.configuration.container import Container
-from dlt.common.data_writers import DataWriter, DataWriterMetrics, TDataItemFormat
+from dlt.common.data_writers import (
+    DataWriter,
+    DataWriterMetrics,
+    TDataItemFormat,
+    resolve_best_writer_spec,
+    get_best_writer_spec,
+    is_native_writer,
+)
 from dlt.common.data_writers.writers import EMPTY_DATA_WRITER_METRICS
 from dlt.common.runners import TRunMetrics, Runnable, NullExecutor
 from dlt.common.runtime import signals
 from dlt.common.runtime.collector import Collector, NULL_COLLECTOR
 from dlt.common.schema.typing import TStoredSchema
 from dlt.common.schema.utils import merge_schema_updates
 from dlt.common.storages import (
@@ -117,20 +124,38 @@
             schema = Schema.from_stored_schema(stored_schema)
             normalize_storage = NormalizeStorage(False, normalize_storage_config)
             load_storage = LoadStorage(False, supported_formats, loader_storage_config)
 
             def _get_items_normalizer(item_format: TDataItemFormat) -> ItemsNormalizer:
                 if item_format in item_normalizers:
                     return item_normalizers[item_format]
-                item_storage = load_storage.create_item_storage(preferred_file_format, item_format)
-                if item_storage.writer_spec.file_format != preferred_file_format:
+                # force file format
+                if config.loader_file_format:
+                    # TODO: pass supported_formats, when used in pipeline we already checked that
+                    # but if normalize is used standalone `supported_loader_file_formats` may be unresolved
+                    best_writer_spec = get_best_writer_spec(item_format, config.loader_file_format)
+                else:
+                    # find best spec among possible formats taking into account destination preference
+                    best_writer_spec = resolve_best_writer_spec(
+                        item_format, supported_formats, preferred_file_format
+                    )
+                    # if best_writer_spec.file_format != preferred_file_format:
+                    #     logger.warning(
+                    #         f"For data items yielded as {item_format} jobs in file format"
+                    #         f" {preferred_file_format} cannot be created."
+                    #         f" {best_writer_spec.file_format} jobs will be used instead."
+                    #         " This may decrease the performance."
+                    #     )
+                item_storage = load_storage.create_item_storage(best_writer_spec)
+                if not is_native_writer(item_storage.writer_cls):
                     logger.warning(
-                        f"For data items yielded as {item_format} job files in format"
-                        f" {preferred_file_format} cannot be created."
-                        f" {item_storage.writer_spec.file_format} jobs will be used instead."
+                        f"For data items yielded as {item_format} and job file format"
+                        f" {best_writer_spec.file_format} native writer could not be found. A"
+                        f" {item_storage.writer_cls.__name__} writer is used that internally"
+                        f" converts {item_format}. This will degrade performance."
                     )
                 cls = ArrowItemsNormalizer if item_format == "arrow" else JsonLItemsNormalizer
                 logger.info(
                     f"Created items normalizer {cls.__name__} with writer"
                     f" {item_storage.writer_cls.__name__} for item format {item_format} and file"
                     f" format {item_storage.writer_spec.file_format}"
                 )
```

### Comparing `dlt-0.4.9a0/dlt/pipeline/__init__.py` & `dlt-0.4.9a1/dlt/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/pipeline/configuration.py` & `dlt-0.4.9a1/dlt/pipeline/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/pipeline/current.py` & `dlt-0.4.9a1/dlt/pipeline/current.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/pipeline/dbt.py` & `dlt-0.4.9a1/dlt/pipeline/dbt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/pipeline/exceptions.py` & `dlt-0.4.9a1/dlt/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/pipeline/helpers.py` & `dlt-0.4.9a1/dlt/pipeline/helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/pipeline/pipeline.py` & `dlt-0.4.9a1/dlt/pipeline/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,19 +28,17 @@
 from dlt.common.configuration.exceptions import (
     ConfigFieldMissingException,
     ContextDefaultCannotBeCreated,
 )
 from dlt.common.configuration.specs.config_section_context import ConfigSectionContext
 from dlt.common.configuration.resolve import initialize_credentials
 from dlt.common.destination.exceptions import (
-    DestinationLoadingViaStagingNotSupported,
-    DestinationLoadingWithoutStagingNotSupported,
+    DestinationIncompatibleLoaderFileFormatException,
     DestinationNoStagingMode,
     DestinationUndefinedEntity,
-    DestinationIncompatibleLoaderFileFormatException,
 )
 from dlt.common.exceptions import MissingDependencyException
 from dlt.common.normalizers import explicit_normalizers, import_normalizers
 from dlt.common.runtime import signals, initialize_runtime
 from dlt.common.schema.typing import (
     TColumnNames,
     TSchemaTables,
@@ -63,14 +61,15 @@
     LoadStorageConfiguration,
     PackageStorage,
     LoadJobInfo,
     LoadPackageInfo,
 )
 from dlt.common.destination import (
     DestinationCapabilitiesContext,
+    merge_caps_file_formats,
     TDestination,
     ALL_SUPPORTED_FILE_FORMATS,
     TLoaderFileFormat,
 )
 from dlt.common.destination.reference import (
     DestinationClientDwhConfiguration,
     WithStateSync,
@@ -466,20 +465,28 @@
 
         # make sure destination capabilities are available
         self._get_destination_capabilities()
 
         # create default normalize config
         normalize_config = NormalizeConfiguration(
             workers=workers,
+            loader_file_format=loader_file_format,
             _schema_storage_config=self._schema_storage_config,
             _normalize_storage_config=self._normalize_storage_config(),
             _load_storage_config=self._load_storage_config(),
         )
         # run with destination context
-        with self._maybe_destination_capabilities(loader_file_format=loader_file_format):
+        with self._maybe_destination_capabilities() as caps:
+            if loader_file_format and loader_file_format not in caps.supported_loader_file_formats:
+                raise DestinationIncompatibleLoaderFileFormatException(
+                    self.destination.destination_name,
+                    (self.staging.destination_name if self.staging else None),
+                    loader_file_format,
+                    set(caps.supported_loader_file_formats),
+                )
             # shares schema storage with the pipeline so we do not need to install
             normalize_step: Normalize = Normalize(
                 collector=self.collector,
                 config=normalize_config,
                 schema_storage=self._schema_storage,
             )
             try:
@@ -755,16 +762,16 @@
                             # and storage is not initialized
                             should_wipe = not job_client.is_storage_initialized()
                     if should_wipe:
                         # reset pipeline
                         self._wipe_working_folder()
                         state = self._get_state()
                         self._configure(
-                            self._schema_storage_config.export_schema_path,
                             self._schema_storage_config.import_schema_path,
+                            self._schema_storage_config.export_schema_path,
                             False,
                         )
 
             # write the state back
             self._props_to_state(state)
             bump_pipeline_state_version_if_modified(state)
             self._save_state(state)
@@ -1258,81 +1265,38 @@
 
         with self._maybe_destination_capabilities():
             # default normalizers must match the destination
             self._set_default_normalizers()
 
     @contextmanager
     def _maybe_destination_capabilities(
-        self, loader_file_format: TLoaderFileFormat = None
+        self,
     ) -> Iterator[DestinationCapabilitiesContext]:
         try:
             caps: DestinationCapabilitiesContext = None
             injected_caps: ContextManager[DestinationCapabilitiesContext] = None
             if self.destination:
                 destination_caps = self._get_destination_capabilities()
                 stage_caps = self._get_staging_capabilities()
                 injected_caps = self._container.injectable_context(destination_caps)
                 caps = injected_caps.__enter__()
 
-                caps.preferred_loader_file_format = self._resolve_loader_file_format(
-                    self.destination.destination_name,
-                    (
-                        # DestinationReference.to_name(self.destination),
-                        self.staging.destination_name
-                        if self.staging
-                        else None
-                    ),
-                    # DestinationReference.to_name(self.staging) if self.staging else None,
-                    destination_caps,
-                    stage_caps,
-                    loader_file_format,
+                caps.preferred_loader_file_format, caps.supported_loader_file_formats = (
+                    merge_caps_file_formats(
+                        self.destination.destination_name,
+                        (self.staging.destination_name if self.staging else None),
+                        destination_caps,
+                        stage_caps,
+                    )
                 )
-                caps.supported_loader_file_formats = (
-                    destination_caps.supported_staging_file_formats if stage_caps else None
-                ) or destination_caps.supported_loader_file_formats
             yield caps
         finally:
             if injected_caps:
                 injected_caps.__exit__(None, None, None)
 
-    @staticmethod
-    def _resolve_loader_file_format(
-        destination: str,
-        staging: str,
-        dest_caps: DestinationCapabilitiesContext,
-        stage_caps: DestinationCapabilitiesContext,
-        file_format: TLoaderFileFormat,
-    ) -> TLoaderFileFormat:
-        possible_file_formats = dest_caps.supported_loader_file_formats
-        if stage_caps:
-            if not dest_caps.supported_staging_file_formats:
-                raise DestinationLoadingViaStagingNotSupported(destination)
-            possible_file_formats = [
-                f
-                for f in dest_caps.supported_staging_file_formats
-                if f in stage_caps.supported_loader_file_formats
-            ]
-        if not file_format:
-            if not stage_caps:
-                if not dest_caps.preferred_loader_file_format:
-                    raise DestinationLoadingWithoutStagingNotSupported(destination)
-                file_format = dest_caps.preferred_loader_file_format
-            elif stage_caps and dest_caps.preferred_staging_file_format in possible_file_formats:
-                file_format = dest_caps.preferred_staging_file_format
-            else:
-                file_format = possible_file_formats[0] if len(possible_file_formats) > 0 else None
-        if file_format not in possible_file_formats:
-            raise DestinationIncompatibleLoaderFileFormatException(
-                destination,
-                staging,
-                file_format,
-                set(possible_file_formats),
-            )
-        return file_format
-
     def _set_default_normalizers(self) -> None:
         _, self._default_naming, _ = import_normalizers(explicit_normalizers())
 
     def _set_dataset_name(self, new_dataset_name: str) -> None:
         if not new_dataset_name and not self.dataset_name:
             # dataset name is required but not provided - generate the default now
             destination_needs_dataset = False
```

### Comparing `dlt-0.4.9a0/dlt/pipeline/platform.py` & `dlt-0.4.9a1/dlt/pipeline/platform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/pipeline/progress.py` & `dlt-0.4.9a1/dlt/pipeline/progress.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/pipeline/state_sync.py` & `dlt-0.4.9a1/dlt/pipeline/state_sync.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/pipeline/trace.py` & `dlt-0.4.9a1/dlt/pipeline/trace.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/pipeline/track.py` & `dlt-0.4.9a1/dlt/pipeline/track.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/pipeline/warnings.py` & `dlt-0.4.9a1/dlt/pipeline/warnings.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/reflection/names.py` & `dlt-0.4.9a1/dlt/reflection/names.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/reflection/script_inspector.py` & `dlt-0.4.9a1/dlt/reflection/script_inspector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/reflection/script_visitor.py` & `dlt-0.4.9a1/dlt/reflection/script_visitor.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/sources/credentials.py` & `dlt-0.4.9a1/dlt/sources/credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/sources/helpers/requests/__init__.py` & `dlt-0.4.9a1/dlt/sources/helpers/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/sources/helpers/requests/retry.py` & `dlt-0.4.9a1/dlt/sources/helpers/requests/retry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/sources/helpers/requests/session.py` & `dlt-0.4.9a1/dlt/sources/helpers/requests/session.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/sources/helpers/rest_client/__init__.py` & `dlt-0.4.9a1/dlt/sources/helpers/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/sources/helpers/rest_client/auth.py` & `dlt-0.4.9a1/dlt/sources/helpers/rest_client/auth.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/sources/helpers/rest_client/client.py` & `dlt-0.4.9a1/dlt/sources/helpers/rest_client/client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/sources/helpers/rest_client/detector.py` & `dlt-0.4.9a1/dlt/sources/helpers/rest_client/detector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/sources/helpers/rest_client/paginators.py` & `dlt-0.4.9a1/dlt/sources/helpers/rest_client/paginators.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/sources/helpers/transform.py` & `dlt-0.4.9a1/dlt/sources/helpers/transform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/dlt/version.py` & `dlt-0.4.9a1/dlt/version.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.9a0/pyproject.toml` & `dlt-0.4.9a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt"
-version = "0.4.9a0"
+version = "0.4.9a1"
 description = "dlt is an open-source python-first scalable data loading library that does not require any backend to run."
 authors = ["dltHub Inc. <services@dlthub.com>"]
 maintainers = [ "Marcin Rudolf <marcin@dlthub.com>", "Adrian Brudaru <adrian@dlthub.com>", "Ty Dunn <ty@dlthub.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/dlt-hub"
 repository = "https://github.com/dlt-hub/dlt"
@@ -144,14 +144,15 @@
 cryptography = "^41.0.7"
 google-api-python-client = ">=1.7.11"
 pytest-asyncio = "^0.23.5"
 types-sqlalchemy = "^1.4.53.38"
 types-pytz = ">=2024.1.0.20240203"
 ruff = "^0.3.2"
 pyjwt = "^2.8.0"
+pytest-mock = "^3.14.0"
 
 [tool.poetry.group.pipeline]
 optional=true
 
 [tool.poetry.group.pipeline.dependencies]
 google-auth-oauthlib = "^1.0.0"
 tqdm = "^4.65.0"
```

### Comparing `dlt-0.4.9a0/PKG-INFO` & `dlt-0.4.9a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt
-Version: 0.4.9a0
+Version: 0.4.9a1
 Summary: dlt is an open-source python-first scalable data loading library that does not require any backend to run.
 Home-page: https://github.com/dlt-hub
 License: Apache-2.0
 Keywords: etl
 Author: dltHub Inc.
 Author-email: services@dlthub.com
 Maintainer: Marcin Rudolf
```

