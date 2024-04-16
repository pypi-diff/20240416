# Comparing `tmp/meltano-3.4.0a2.tar.gz` & `tmp/meltano-3.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meltano-3.4.0a2.tar", max compression
+gzip compressed data, was "meltano-3.4.0b1.tar", max compression
```

## Comparing `meltano-3.4.0a2.tar` & `meltano-3.4.0b1.tar`

### file list

```diff
@@ -1,298 +1,298 @@
--rw-r--r--   0        0        0     1048 2024-04-12 21:49:27.862604 meltano-3.4.0a2/LICENSE
--rw-r--r--   0        0        0     5237 2024-04-12 21:49:27.862604 meltano-3.4.0a2/README.md
--rw-r--r--   0        0        0    19419 2024-04-12 21:49:27.998604 meltano-3.4.0a2/pyproject.toml
--rw-r--r--   0        0        0      100 2024-04-12 21:49:27.998604 meltano-3.4.0a2/src/meltano/__init__.py
--rw-r--r--   0        0        0     3631 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/__init__.py
--rw-r--r--   0        0        0       73 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/__main__.py
--rw-r--r--   0        0        0     6770 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/add.py
--rw-r--r--   0        0        0     6006 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/cli.py
--rw-r--r--   0        0        0     3806 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/compile.py
--rw-r--r--   0        0        0    14489 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/config.py
--rw-r--r--   0        0        0      406 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/docs.py
--rw-r--r--   0        0        0      507 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/dragon.py
--rw-r--r--   0        0        0    17244 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/elt.py
--rw-r--r--   0        0        0     2548 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/environment.py
--rw-r--r--   0        0        0     1671 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/hub.py
--rw-r--r--   0        0        0     2221 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/initialize.py
--rw-r--r--   0        0        0     4100 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/install.py
--rw-r--r--   0        0        0      181 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/interactive/__init__.py
--rw-r--r--   0        0        0    16395 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/interactive/config.py
--rw-r--r--   0        0        0      241 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/interactive/utils.py
--rw-r--r--   0        0        0     6275 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/invoke.py
--rw-r--r--   0        0        0    10060 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/job.py
--rw-r--r--   0        0        0     3804 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/lock.py
--rw-r--r--   0        0        0     2242 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/params.py
--rw-r--r--   0        0        0     2789 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/remove.py
--rw-r--r--   0        0        0     7299 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/run.py
--rw-r--r--   0        0        0    12993 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/schedule.py
--rw-r--r--   0        0        0      770 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/schema.py
--rw-r--r--   0        0        0     4446 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/select.py
--rw-r--r--   0        0        0    10590 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/state.py
--rw-r--r--   0        0        0     4344 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/upgrade.py
--rw-r--r--   0        0        0    23965 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/utils.py
--rw-r--r--   0        0        0     4185 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/validate.py
--rw-r--r--   0        0        0        0 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/__init__.py
--rw-r--r--   0        0        0       64 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/behavior/__init__.py
--rw-r--r--   0        0        0    13060 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/behavior/canonical.py
--rw-r--r--   0        0        0     3962 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/behavior/hookable.py
--rw-r--r--   0        0        0      192 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/behavior/name_eq.py
--rw-r--r--   0        0        0     1187 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/behavior/versioned.py
--rw-r--r--   0        0        0      406 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/behavior/visitor.py
--rw-r--r--   0        0        0      117 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/block/__init__.py
--rw-r--r--   0        0        0     1582 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/block/blockset.py
--rw-r--r--   0        0        0    29706 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/block/extract_load.py
--rw-r--r--   0        0        0     2705 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/block/future_utils.py
--rw-r--r--   0        0        0     3946 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/block/ioblock.py
--rw-r--r--   0        0        0    11236 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/block/parser.py
--rw-r--r--   0        0        0     5745 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/block/plugin_command.py
--rw-r--r--   0        0        0    12176 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/block/singer.py
--rw-r--r--   0        0        0      128 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/bundle/__init__.py
--rw-r--r--   0        0        0      460 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/bundle/initialize.yml
--rw-r--r--   0        0        0     2773 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/bundle/settings.yml
--rw-r--r--   0        0        0    10326 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/cli_messages.py
--rw-r--r--   0        0        0     3094 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/config_service.py
--rw-r--r--   0        0        0       81 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/container/__init__.py
--rw-r--r--   0        0        0     2130 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/container/container_service.py
--rw-r--r--   0        0        0     2997 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/container/container_spec.py
--rw-r--r--   0        0        0     7391 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/db.py
--rw-r--r--   0        0        0    14930 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/elt_context.py
--rw-r--r--   0        0        0     6924 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/environment.py
--rw-r--r--   0        0        0     2797 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/environment_service.py
--rw-r--r--   0        0        0     3747 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/error.py
--rw-r--r--   0        0        0      181 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/hub/__init__.py
--rw-r--r--   0        0        0    11085 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/hub/client.py
--rw-r--r--   0        0        0      896 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/hub/schema.py
--rw-r--r--   0        0        0      103 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/job/__init__.py
--rw-r--r--   0        0        0     5940 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/job/finder.py
--rw-r--r--   0        0        0    11544 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/job/job.py
--rw-r--r--   0        0        0     1036 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/job/stale_job_failer.py
--rw-r--r--   0        0        0     6015 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/job_state.py
--rw-r--r--   0        0        0     2974 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/locked_definition_service.py
--rw-r--r--   0        0        0      699 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/logging/__init__.py
--rw-r--r--   0        0        0     4530 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/logging/formatters.py
--rw-r--r--   0        0        0     5573 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/logging/job_logging_service.py
--rw-r--r--   0        0        0     7367 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/logging/output_logger.py
--rw-r--r--   0        0        0     7084 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/logging/utils.py
--rw-r--r--   0        0        0     3453 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/manifest/__init__.py
--rw-r--r--   0        0        0      365 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/manifest/cache.py
--rw-r--r--   0        0        0     4835 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/manifest/contexts.py
--rw-r--r--   0        0        0     4867 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/manifest/jsonschema.py
--rw-r--r--   0        0        0    18190 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/manifest/manifest.py
--rw-r--r--   0        0        0     5137 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/meltano_file.py
--rw-r--r--   0        0        0     2679 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/meltano_invoker.py
--rw-r--r--   0        0        0     3665 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/migration_service.py
--rw-r--r--   0        0        0      481 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/models.py
--rw-r--r--   0        0        0      188 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/__init__.py
--rw-r--r--   0        0        0     5707 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/airflow.py
--rw-r--r--   0        0        0    27344 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/base.py
--rw-r--r--   0        0        0     3638 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/command.py
--rw-r--r--   0        0        0     1422 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/config_service.py
--rw-r--r--   0        0        0      139 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/dbt/__init__.py
--rw-r--r--   0        0        0     4072 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/dbt/base.py
--rw-r--r--   0        0        0     2703 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/error.py
--rw-r--r--   0        0        0     1849 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/factory.py
--rw-r--r--   0        0        0     9890 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/file.py
--rw-r--r--   0        0        0     2708 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/meltano_file.py
--rw-r--r--   0        0        0    14822 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/project_plugin.py
--rw-r--r--   0        0        0     1135 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/requirements.py
--rw-r--r--   0        0        0     7651 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/settings_service.py
--rw-r--r--   0        0        0      282 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/singer/__init__.py
--rw-r--r--   0        0        0     2552 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/singer/base.py
--rw-r--r--   0        0        0    19585 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/singer/catalog.py
--rw-r--r--   0        0        0     2362 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/singer/mapper.py
--rw-r--r--   0        0        0    23896 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/singer/tap.py
--rw-r--r--   0        0        0     5573 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/singer/target.py
--rw-r--r--   0        0        0     5850 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/superset.py
--rw-r--r--   0        0        0      269 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/utility.py
--rw-r--r--   0        0        0    17407 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin_install_service.py
--rw-r--r--   0        0        0    17248 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin_invoker.py
--rw-r--r--   0        0        0     6473 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin_location_remove.py
--rw-r--r--   0        0        0     3931 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin_lock_service.py
--rw-r--r--   0        0        0     2817 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin_remove_service.py
--rw-r--r--   0        0        0     2180 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin_repository.py
--rw-r--r--   0        0        0     3289 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin_test_service.py
--rw-r--r--   0        0        0    20306 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/project.py
--rw-r--r--   0        0        0     3999 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/project_add_service.py
--rw-r--r--   0        0        0    14180 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/project_files.py
--rw-r--r--   0        0        0     6581 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/project_init_service.py
--rw-r--r--   0        0        0    18330 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/project_plugins_service.py
--rw-r--r--   0        0        0     5118 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/project_settings_service.py
--rw-r--r--   0        0        0      262 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/runner/__init__.py
--rw-r--r--   0        0        0     2149 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/runner/dbt.py
--rw-r--r--   0        0        0    10141 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/runner/singer.py
--rw-r--r--   0        0        0     3769 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/schedule.py
--rw-r--r--   0        0        0    10918 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/schedule_service.py
--rw-r--r--   0        0        0     3384 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/select_service.py
--rw-r--r--   0        0        0      926 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/setting.py
--rw-r--r--   0        0        0    15081 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/setting_definition.py
--rw-r--r--   0        0        0    21245 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/settings_service.py
--rw-r--r--   0        0        0    46397 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/settings_store.py
--rw-r--r--   0        0        0     2573 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/sqlalchemy.py
--rw-r--r--   0        0        0     7282 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/state_service.py
--rw-r--r--   0        0        0     3728 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/state_store/__init__.py
--rw-r--r--   0        0        0     5482 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/state_store/azure.py
--rw-r--r--   0        0        0     2134 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/state_store/base.py
--rw-r--r--   0        0        0     3831 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/state_store/db.py
--rw-r--r--   0        0        0    17948 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/state_store/filesystem.py
--rw-r--r--   0        0        0     4170 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/state_store/google.py
--rw-r--r--   0        0        0     4860 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/state_store/s3.py
--rw-r--r--   0        0        0     4461 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/task_sets.py
--rw-r--r--   0        0        0     3993 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/task_sets_service.py
--rw-r--r--   0        0        0        0 2024-04-12 21:49:47.498551 meltano-3.4.0a2/src/meltano/core/tracking/.release_marker
--rw-r--r--   0        0        0     3614 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/README.md
--rw-r--r--   0        0        0      125 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/__init__.py
--rw-r--r--   0        0        0      470 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/contexts/__init__.py
--rw-r--r--   0        0        0     2515 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/contexts/cli.py
--rw-r--r--   0        0        0     6044 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/contexts/environment.py
--rw-r--r--   0        0        0     3790 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/contexts/exception.py
--rw-r--r--   0        0        0     4948 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/contexts/plugins.py
--rw-r--r--   0        0        0     4128 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/contexts/project.py
--rw-r--r--   0        0        0      918 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/block_event/jsonschema/1-0-0
--rw-r--r--   0        0        0     1051 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     1194 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-1-0
--rw-r--r--   0        0        0      720 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-0
--rw-r--r--   0        0        0      748 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-1
--rw-r--r--   0        0        0     6002 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     6501 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-1-0
--rw-r--r--   0        0        0     6963 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-2-0
--rw-r--r--   0        0        0     7408 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-3-0
--rw-r--r--   0        0        0     4449 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exception_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     1403 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-0
--rw-r--r--   0        0        0     1462 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-1
--rw-r--r--   0        0        0     3920 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/plugins_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     2109 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     2812 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-1-0
--rw-r--r--   0        0        0     1202 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/telemetry_state_change_event/jsonschema/1-0-0
--rw-r--r--   0        0        0      404 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu.json
--rw-r--r--   0        0        0     9688 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/micro.conf
--rw-r--r--   0        0        0     1112 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/schemas.py
--rw-r--r--   0        0        0    18604 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/tracker.py
--rw-r--r--   0        0        0     3562 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/transform_add_service.py
--rw-r--r--   0        0        0     7708 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/upgrade_service.py
--rw-r--r--   0        0        0    25155 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/utils/__init__.py
--rw-r--r--   0        0        0     1451 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/utils/pidfile.py
--rw-r--r--   0        0        0     4105 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/validation_service.py
--rw-r--r--   0        0        0    23806 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/venv_service.py
--rw-r--r--   0        0        0     1521 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/yaml.py
--rw-r--r--   0        0        0      508 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/__init__.py
--rw-r--r--   0        0        0       12 2024-04-12 21:49:47.406551 meltano-3.4.0a2/src/meltano/migrations/db.lock
--rw-r--r--   0        0        0     1490 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/env.py
--rw-r--r--   0        0        0      495 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/script.py.mako
--rw-r--r--   0        0        0       67 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/utils/__init__.py
--rw-r--r--   0        0        0     1261 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/utils/dialect_typing.py
--rw-r--r--   0        0        0     1814 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/13e8639c6d2b_add_state_edit_to_job_state_enum.py
--rw-r--r--   0        0        0      972 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/23ea52e6d784_add_resource_type_to_embed_token.py
--rw-r--r--   0        0        0      674 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/367228df6a43_add_trigger_to_job.py
--rw-r--r--   0        0        0      802 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/53e97221d99f_add_run_id_to_job.py
--rw-r--r--   0        0        0      563 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/5b43800443d1_rename_job_to_job_run_and_job_id_to_job_.py
--rw-r--r--   0        0        0    11827 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/6828cc5b1a4f_create_dedicated_state_table.py
--rw-r--r--   0        0        0     2877 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/6ef30ab7b8e5_.py
--rw-r--r--   0        0        0     1095 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/87d9638f6ac6_add_subscription.py
--rw-r--r--   0        0        0      643 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/990c0665f3ce_ensure_user_login_count_default_value.py
--rw-r--r--   0        0        0      786 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/a3e2b0a4937d_add_login_audit_columns.py
--rw-r--r--   0        0        0     2026 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/b4c05e463b53_.py
--rw-r--r--   0        0        0      972 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/ceb00d7ff3bd_create_the_embedtoken_table.py
--rw-r--r--   0        0        0      699 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/d135f52a6f49_add_last_heartbeat_at_column_to_job.py
--rw-r--r--   0        0        0      679 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/e4fbabc3fed6_add_last_activity_at_column.py
--rw-r--r--   0        0        0      486 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/f4c225a9492f_create_dedicated_job_state_table.py
--rw-r--r--   0        0        0    37569 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/schemas/meltano.schema.json
--rw-r--r--   0        0        0      438 2024-04-12 21:49:28.010604 meltano-3.4.0a2/tests/asserts.py
--rw-r--r--   0        0        0     7479 2024-04-12 21:49:28.010604 meltano-3.4.0a2/tests/conftest.py
--rw-r--r--   0        0        0     2174 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/cli.py
--rw-r--r--   0        0        0   125876 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/core.py
--rw-r--r--   0        0        0     2829 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/db/__init__.py
--rw-r--r--   0        0        0     2510 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/db/mssql.py
--rw-r--r--   0        0        0     1227 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/db/postgresql.py
--rw-r--r--   0        0        0     1222 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/db/postgresql_psycopg3.py
--rw-r--r--   0        0        0      328 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/db/sqlite.py
--rw-r--r--   0        0        0      752 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/docker/__init__.py
--rw-r--r--   0        0        0      276 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/docker/docker-compose.yml
--rw-r--r--   0        0        0     4132 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/docker/snowplow.py
--rw-r--r--   0        0        0     1535 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/fs.py
--rw-r--r--   0        0        0     3135 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/large_config_project/meltano.yml
--rw-r--r--   0        0        0    30013 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/large_config_project/schedule.yml
--rw-r--r--   0        0        0     1086 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/multifile_project/meltano.yml
--rw-r--r--   0        0        0      469 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/multifile_project/subconfig_2.yml
--rw-r--r--   0        0        0      394 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/multifile_project/subfolder/subconfig_1.yml
--rw-r--r--   0        0        0      631 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/plugins/extractors/tap-custom/test.yml
--rw-r--r--   0        0        0     1136 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/utils.py
--rw-r--r--   0        0        0    31067 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_add.py
--rw-r--r--   0        0        0    15154 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_cli.py
--rw-r--r--   0        0        0     5174 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_compile.py
--rw-r--r--   0        0        0     8595 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_config.py
--rw-r--r--   0        0        0    42025 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_elt.py
--rw-r--r--   0        0        0     1585 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_hub.py
--rw-r--r--   0        0        0     3577 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_initialize.py
--rw-r--r--   0        0        0    12665 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_install.py
--rw-r--r--   0        0        0     9285 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_invoke.py
--rw-r--r--   0        0        0     6777 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_job_cmd.py
--rw-r--r--   0        0        0     3771 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_lock.py
--rw-r--r--   0        0        0     1864 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_remove.py
--rw-r--r--   0        0        0    47456 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_run.py
--rw-r--r--   0        0        0     8502 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_schedule.py
--rw-r--r--   0        0        0     1140 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_select.py
--rw-r--r--   0        0        0    11532 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_state.py
--rw-r--r--   0        0        0     8268 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_upgrade.py
--rw-r--r--   0        0        0     5381 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/behavior/test_canonical.py
--rw-r--r--   0        0        0     2155 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/behavior/test_hookable.py
--rw-r--r--   0        0        0    21766 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/block/test_extract_load.py
--rw-r--r--   0        0        0      241 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/block/test_parser.py
--rw-r--r--   0        0        0      933 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/block/test_plugin_command.py
--rw-r--r--   0        0        0     7736 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/block/test_singer.py
--rw-r--r--   0        0        0     2302 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/container/test_container_spec.py
--rw-r--r--   0        0        0     6783 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/hub/test_meltano_hub_service.py
--rw-r--r--   0        0        0     2076 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/job/test_finder.py
--rw-r--r--   0        0        0     6240 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/job/test_job.py
--rw-r--r--   0        0        0     2579 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/job/test_stale_job_failer.py
--rw-r--r--   0        0        0     3357 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/logging/test_formatters.py
--rw-r--r--   0        0        0      806 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/logging/test_logging_utils.py
--rw-r--r--   0        0        0     7398 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/logging/test_output_logger.py
--rw-r--r--   0        0        0    32051 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/plugin/singer/test_catalog.py
--rw-r--r--   0        0        0      562 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/plugin/singer/test_mapper.py
--rw-r--r--   0        0        0    37590 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/plugin/singer/test_tap.py
--rw-r--r--   0        0        0     3690 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/plugin/singer/test_target.py
--rw-r--r--   0        0        0     3921 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/plugin/test_airflow.py
--rw-r--r--   0        0        0     2396 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/plugin/test_command.py
--rw-r--r--   0        0        0    22146 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/plugin/test_plugin.py
--rw-r--r--   0        0        0      174 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/plugin/test_plugin_config_service.py
--rw-r--r--   0        0        0    35208 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/plugin/test_plugin_settings.py
--rw-r--r--   0        0        0     5963 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/plugin/test_superset.py
--rw-r--r--   0        0        0     7999 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/runner/test_runner.py
--rw-r--r--   0        0        0     2807 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/state_store/test_db.py
--rw-r--r--   0        0        0    21574 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/state_store/test_filesystem.py
--rw-r--r--   0        0        0     6765 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/state_store/test_state_store.py
--rw-r--r--   0        0        0     1558 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_db_compat.py
--rw-r--r--   0        0        0     1813 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_db_connection.py
--rw-r--r--   0        0        0     5217 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_elt_context.py
--rw-r--r--   0        0        0     2610 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_environment_service.py
--rw-r--r--   0        0        0    13772 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_environment_variables.py
--rw-r--r--   0        0        0     2274 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_locked_definition_service.py
--rw-r--r--   0        0        0     2108 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_meltano_file.py
--rw-r--r--   0        0        0     3128 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_meltano_invoker.py
--rw-r--r--   0        0        0     4094 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_plugin_install_service.py
--rw-r--r--   0        0        0     6101 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_plugin_invoker.py
--rw-r--r--   0        0        0     3127 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_plugin_lock_service.py
--rw-r--r--   0        0        0     5749 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_plugin_remove_service.py
--rw-r--r--   0        0        0     5776 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_plugin_test_service.py
--rw-r--r--   0        0        0     4319 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_project.py
--rw-r--r--   0        0        0     8892 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_project_add_service.py
--rw-r--r--   0        0        0    16326 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_project_files.py
--rw-r--r--   0        0        0     3281 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_project_init_service.py
--rw-r--r--   0        0        0     8071 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_project_plugins_service.py
--rw-r--r--   0        0        0     7238 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_project_settings_service.py
--rw-r--r--   0        0        0     9759 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_schedule_service.py
--rw-r--r--   0        0        0     2766 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_setting_definition.py
--rw-r--r--   0        0        0    22226 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_settings_store.py
--rw-r--r--   0        0        0     3665 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_state_service.py
--rw-r--r--   0        0        0     2430 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_task_sets.py
--rw-r--r--   0        0        0     2645 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_task_sets_service.py
--rw-r--r--   0        0        0     7126 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_utils.py
--rw-r--r--   0        0        0     1813 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_validation_service.py
--rw-r--r--   0        0        0    12409 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_venv_service.py
--rw-r--r--   0        0        0     1980 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/tracking/test_environment_context.py
--rw-r--r--   0        0        0     5708 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/tracking/test_exception.py
--rw-r--r--   0        0        0     3061 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/tracking/test_plugins.py
--rw-r--r--   0        0        0     1271 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/tracking/test_project_context.py
--rw-r--r--   0        0        0      684 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/tracking/test_schemas.py
--rw-r--r--   0        0        0    19704 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/tracking/test_tracker.py
--rw-r--r--   0        0        0     9032 1970-01-01 00:00:00.000000 meltano-3.4.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1048 2024-04-16 15:52:52.147721 meltano-3.4.0b1/LICENSE
+-rw-r--r--   0        0        0     5237 2024-04-16 15:52:52.147721 meltano-3.4.0b1/README.md
+-rw-r--r--   0        0        0    19419 2024-04-16 15:52:52.275722 meltano-3.4.0b1/pyproject.toml
+-rw-r--r--   0        0        0      100 2024-04-16 15:52:52.275722 meltano-3.4.0b1/src/meltano/__init__.py
+-rw-r--r--   0        0        0     3631 2024-04-16 15:52:52.275722 meltano-3.4.0b1/src/meltano/cli/__init__.py
+-rw-r--r--   0        0        0       73 2024-04-16 15:52:52.275722 meltano-3.4.0b1/src/meltano/cli/__main__.py
+-rw-r--r--   0        0        0     6770 2024-04-16 15:52:52.275722 meltano-3.4.0b1/src/meltano/cli/add.py
+-rw-r--r--   0        0        0     6006 2024-04-16 15:52:52.275722 meltano-3.4.0b1/src/meltano/cli/cli.py
+-rw-r--r--   0        0        0     3806 2024-04-16 15:52:52.275722 meltano-3.4.0b1/src/meltano/cli/compile.py
+-rw-r--r--   0        0        0    14489 2024-04-16 15:52:52.275722 meltano-3.4.0b1/src/meltano/cli/config.py
+-rw-r--r--   0        0        0      406 2024-04-16 15:52:52.275722 meltano-3.4.0b1/src/meltano/cli/docs.py
+-rw-r--r--   0        0        0      507 2024-04-16 15:52:52.275722 meltano-3.4.0b1/src/meltano/cli/dragon.py
+-rw-r--r--   0        0        0    17244 2024-04-16 15:52:52.275722 meltano-3.4.0b1/src/meltano/cli/elt.py
+-rw-r--r--   0        0        0     2548 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/environment.py
+-rw-r--r--   0        0        0     1671 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/hub.py
+-rw-r--r--   0        0        0     2221 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/initialize.py
+-rw-r--r--   0        0        0     4100 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/install.py
+-rw-r--r--   0        0        0      181 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/interactive/__init__.py
+-rw-r--r--   0        0        0    16395 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/interactive/config.py
+-rw-r--r--   0        0        0      241 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/interactive/utils.py
+-rw-r--r--   0        0        0     6275 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/invoke.py
+-rw-r--r--   0        0        0    10060 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/job.py
+-rw-r--r--   0        0        0     3804 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/lock.py
+-rw-r--r--   0        0        0     2242 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/params.py
+-rw-r--r--   0        0        0     2789 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/remove.py
+-rw-r--r--   0        0        0     7299 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/run.py
+-rw-r--r--   0        0        0    12993 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/schedule.py
+-rw-r--r--   0        0        0      770 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/schema.py
+-rw-r--r--   0        0        0     4446 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/select.py
+-rw-r--r--   0        0        0    10590 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/state.py
+-rw-r--r--   0        0        0     4344 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/upgrade.py
+-rw-r--r--   0        0        0    23965 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/utils.py
+-rw-r--r--   0        0        0     4185 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/cli/validate.py
+-rw-r--r--   0        0        0        0 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/__init__.py
+-rw-r--r--   0        0        0       64 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/behavior/__init__.py
+-rw-r--r--   0        0        0    13060 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/behavior/canonical.py
+-rw-r--r--   0        0        0     3962 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/behavior/hookable.py
+-rw-r--r--   0        0        0      192 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/behavior/name_eq.py
+-rw-r--r--   0        0        0     1187 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/behavior/versioned.py
+-rw-r--r--   0        0        0      406 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/behavior/visitor.py
+-rw-r--r--   0        0        0      117 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/block/__init__.py
+-rw-r--r--   0        0        0     1582 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/block/blockset.py
+-rw-r--r--   0        0        0    29706 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/block/extract_load.py
+-rw-r--r--   0        0        0     2705 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/block/future_utils.py
+-rw-r--r--   0        0        0     3946 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/block/ioblock.py
+-rw-r--r--   0        0        0    11236 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/block/parser.py
+-rw-r--r--   0        0        0     5745 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/block/plugin_command.py
+-rw-r--r--   0        0        0    12176 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/block/singer.py
+-rw-r--r--   0        0        0      128 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/bundle/__init__.py
+-rw-r--r--   0        0        0      460 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/bundle/initialize.yml
+-rw-r--r--   0        0        0     2773 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/bundle/settings.yml
+-rw-r--r--   0        0        0    10326 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/cli_messages.py
+-rw-r--r--   0        0        0     3094 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/config_service.py
+-rw-r--r--   0        0        0       81 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/container/__init__.py
+-rw-r--r--   0        0        0     2130 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/container/container_service.py
+-rw-r--r--   0        0        0     2997 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/container/container_spec.py
+-rw-r--r--   0        0        0     7391 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/db.py
+-rw-r--r--   0        0        0    14930 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/elt_context.py
+-rw-r--r--   0        0        0     6924 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/environment.py
+-rw-r--r--   0        0        0     2797 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/environment_service.py
+-rw-r--r--   0        0        0     3747 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/error.py
+-rw-r--r--   0        0        0      181 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/hub/__init__.py
+-rw-r--r--   0        0        0    11085 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/hub/client.py
+-rw-r--r--   0        0        0      896 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/hub/schema.py
+-rw-r--r--   0        0        0      103 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/job/__init__.py
+-rw-r--r--   0        0        0     5940 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/job/finder.py
+-rw-r--r--   0        0        0    11544 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/job/job.py
+-rw-r--r--   0        0        0     1036 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/job/stale_job_failer.py
+-rw-r--r--   0        0        0     6015 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/job_state.py
+-rw-r--r--   0        0        0     2974 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/locked_definition_service.py
+-rw-r--r--   0        0        0      699 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/logging/__init__.py
+-rw-r--r--   0        0        0     4530 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/logging/formatters.py
+-rw-r--r--   0        0        0     5573 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/logging/job_logging_service.py
+-rw-r--r--   0        0        0     7367 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/logging/output_logger.py
+-rw-r--r--   0        0        0     7084 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/logging/utils.py
+-rw-r--r--   0        0        0     3453 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/manifest/__init__.py
+-rw-r--r--   0        0        0      365 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/manifest/cache.py
+-rw-r--r--   0        0        0     4835 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/manifest/contexts.py
+-rw-r--r--   0        0        0     4867 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/manifest/jsonschema.py
+-rw-r--r--   0        0        0    18190 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/manifest/manifest.py
+-rw-r--r--   0        0        0     5137 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/meltano_file.py
+-rw-r--r--   0        0        0     2679 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/meltano_invoker.py
+-rw-r--r--   0        0        0     3665 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/migration_service.py
+-rw-r--r--   0        0        0      481 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/models.py
+-rw-r--r--   0        0        0      188 2024-04-16 15:52:52.279723 meltano-3.4.0b1/src/meltano/core/plugin/__init__.py
+-rw-r--r--   0        0        0     5707 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/airflow.py
+-rw-r--r--   0        0        0    27344 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/base.py
+-rw-r--r--   0        0        0     3638 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/command.py
+-rw-r--r--   0        0        0     1422 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/config_service.py
+-rw-r--r--   0        0        0      139 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/dbt/__init__.py
+-rw-r--r--   0        0        0     4072 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/dbt/base.py
+-rw-r--r--   0        0        0     2703 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/error.py
+-rw-r--r--   0        0        0     1849 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/factory.py
+-rw-r--r--   0        0        0     9890 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/file.py
+-rw-r--r--   0        0        0     2708 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/meltano_file.py
+-rw-r--r--   0        0        0    14822 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/project_plugin.py
+-rw-r--r--   0        0        0     1135 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/requirements.py
+-rw-r--r--   0        0        0     7651 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/settings_service.py
+-rw-r--r--   0        0        0      282 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/singer/__init__.py
+-rw-r--r--   0        0        0     2552 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/singer/base.py
+-rw-r--r--   0        0        0    19585 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/singer/catalog.py
+-rw-r--r--   0        0        0     2362 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/singer/mapper.py
+-rw-r--r--   0        0        0    23896 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/singer/tap.py
+-rw-r--r--   0        0        0     5573 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/singer/target.py
+-rw-r--r--   0        0        0     5850 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/superset.py
+-rw-r--r--   0        0        0      269 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin/utility.py
+-rw-r--r--   0        0        0    17350 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin_install_service.py
+-rw-r--r--   0        0        0    17248 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin_invoker.py
+-rw-r--r--   0        0        0     6473 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin_location_remove.py
+-rw-r--r--   0        0        0     3931 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin_lock_service.py
+-rw-r--r--   0        0        0     2817 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin_remove_service.py
+-rw-r--r--   0        0        0     2180 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin_repository.py
+-rw-r--r--   0        0        0     3289 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/plugin_test_service.py
+-rw-r--r--   0        0        0    20306 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/project.py
+-rw-r--r--   0        0        0     3999 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/project_add_service.py
+-rw-r--r--   0        0        0    14180 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/project_files.py
+-rw-r--r--   0        0        0     6581 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/project_init_service.py
+-rw-r--r--   0        0        0    18330 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/project_plugins_service.py
+-rw-r--r--   0        0        0     5118 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/project_settings_service.py
+-rw-r--r--   0        0        0      262 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/runner/__init__.py
+-rw-r--r--   0        0        0     2149 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/runner/dbt.py
+-rw-r--r--   0        0        0    10141 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/runner/singer.py
+-rw-r--r--   0        0        0     3769 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/schedule.py
+-rw-r--r--   0        0        0    10918 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/schedule_service.py
+-rw-r--r--   0        0        0     3384 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/select_service.py
+-rw-r--r--   0        0        0      926 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/setting.py
+-rw-r--r--   0        0        0    15809 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/setting_definition.py
+-rw-r--r--   0        0        0    21245 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/settings_service.py
+-rw-r--r--   0        0        0    46397 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/settings_store.py
+-rw-r--r--   0        0        0     2573 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/sqlalchemy.py
+-rw-r--r--   0        0        0     7282 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/state_service.py
+-rw-r--r--   0        0        0     3728 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/state_store/__init__.py
+-rw-r--r--   0        0        0     5482 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/state_store/azure.py
+-rw-r--r--   0        0        0     2134 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/state_store/base.py
+-rw-r--r--   0        0        0     3831 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/state_store/db.py
+-rw-r--r--   0        0        0    17948 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/state_store/filesystem.py
+-rw-r--r--   0        0        0     4170 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/state_store/google.py
+-rw-r--r--   0        0        0     4860 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/state_store/s3.py
+-rw-r--r--   0        0        0     4461 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/task_sets.py
+-rw-r--r--   0        0        0     3993 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/task_sets_service.py
+-rw-r--r--   0        0        0        0 2024-04-16 15:53:10.131913 meltano-3.4.0b1/src/meltano/core/tracking/.release_marker
+-rw-r--r--   0        0        0     3614 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/tracking/README.md
+-rw-r--r--   0        0        0      125 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/tracking/__init__.py
+-rw-r--r--   0        0        0      470 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/tracking/contexts/__init__.py
+-rw-r--r--   0        0        0     2515 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/tracking/contexts/cli.py
+-rw-r--r--   0        0        0     6044 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/tracking/contexts/environment.py
+-rw-r--r--   0        0        0     3790 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/tracking/contexts/exception.py
+-rw-r--r--   0        0        0     4948 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/tracking/contexts/plugins.py
+-rw-r--r--   0        0        0     4128 2024-04-16 15:52:52.283722 meltano-3.4.0b1/src/meltano/core/tracking/contexts/project.py
+-rw-r--r--   0        0        0      918 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/block_event/jsonschema/1-0-0
+-rw-r--r--   0        0        0     1051 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     1194 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-1-0
+-rw-r--r--   0        0        0      720 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-0
+-rw-r--r--   0        0        0      748 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-1
+-rw-r--r--   0        0        0     6002 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     6501 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-1-0
+-rw-r--r--   0        0        0     6963 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-2-0
+-rw-r--r--   0        0        0     7408 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-3-0
+-rw-r--r--   0        0        0     4449 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exception_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     1403 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-0
+-rw-r--r--   0        0        0     1462 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-1
+-rw-r--r--   0        0        0     3920 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/plugins_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     2109 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     2812 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-1-0
+-rw-r--r--   0        0        0     1202 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/telemetry_state_change_event/jsonschema/1-0-0
+-rw-r--r--   0        0        0      404 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/iglu.json
+-rw-r--r--   0        0        0     9688 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/micro.conf
+-rw-r--r--   0        0        0     1112 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/schemas.py
+-rw-r--r--   0        0        0    18604 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/tracking/tracker.py
+-rw-r--r--   0        0        0     3562 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/transform_add_service.py
+-rw-r--r--   0        0        0     7708 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/upgrade_service.py
+-rw-r--r--   0        0        0    25155 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/utils/__init__.py
+-rw-r--r--   0        0        0     1451 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/utils/pidfile.py
+-rw-r--r--   0        0        0     4105 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/validation_service.py
+-rw-r--r--   0        0        0    23733 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/venv_service.py
+-rw-r--r--   0        0        0     1521 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/core/yaml.py
+-rw-r--r--   0        0        0      508 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/__init__.py
+-rw-r--r--   0        0        0       12 2024-04-16 15:53:10.055912 meltano-3.4.0b1/src/meltano/migrations/db.lock
+-rw-r--r--   0        0        0     1490 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/env.py
+-rw-r--r--   0        0        0      495 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/script.py.mako
+-rw-r--r--   0        0        0       67 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/utils/__init__.py
+-rw-r--r--   0        0        0     1261 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/utils/dialect_typing.py
+-rw-r--r--   0        0        0     1814 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/13e8639c6d2b_add_state_edit_to_job_state_enum.py
+-rw-r--r--   0        0        0      972 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/23ea52e6d784_add_resource_type_to_embed_token.py
+-rw-r--r--   0        0        0      674 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/367228df6a43_add_trigger_to_job.py
+-rw-r--r--   0        0        0      802 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/53e97221d99f_add_run_id_to_job.py
+-rw-r--r--   0        0        0      563 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/5b43800443d1_rename_job_to_job_run_and_job_id_to_job_.py
+-rw-r--r--   0        0        0    11827 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/6828cc5b1a4f_create_dedicated_state_table.py
+-rw-r--r--   0        0        0     2877 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/6ef30ab7b8e5_.py
+-rw-r--r--   0        0        0     1095 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/87d9638f6ac6_add_subscription.py
+-rw-r--r--   0        0        0      643 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/990c0665f3ce_ensure_user_login_count_default_value.py
+-rw-r--r--   0        0        0      786 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/a3e2b0a4937d_add_login_audit_columns.py
+-rw-r--r--   0        0        0     2026 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/b4c05e463b53_.py
+-rw-r--r--   0        0        0      972 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/ceb00d7ff3bd_create_the_embedtoken_table.py
+-rw-r--r--   0        0        0      699 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/d135f52a6f49_add_last_heartbeat_at_column_to_job.py
+-rw-r--r--   0        0        0      679 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/e4fbabc3fed6_add_last_activity_at_column.py
+-rw-r--r--   0        0        0      486 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/migrations/versions/f4c225a9492f_create_dedicated_job_state_table.py
+-rw-r--r--   0        0        0    37569 2024-04-16 15:52:52.287722 meltano-3.4.0b1/src/meltano/schemas/meltano.schema.json
+-rw-r--r--   0        0        0      438 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/asserts.py
+-rw-r--r--   0        0        0     7479 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/conftest.py
+-rw-r--r--   0        0        0     2174 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/fixtures/cli.py
+-rw-r--r--   0        0        0   125876 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/fixtures/core.py
+-rw-r--r--   0        0        0     2829 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/fixtures/db/__init__.py
+-rw-r--r--   0        0        0     2510 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/fixtures/db/mssql.py
+-rw-r--r--   0        0        0     1227 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/fixtures/db/postgresql.py
+-rw-r--r--   0        0        0     1222 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/fixtures/db/postgresql_psycopg3.py
+-rw-r--r--   0        0        0      328 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/fixtures/db/sqlite.py
+-rw-r--r--   0        0        0      752 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/fixtures/docker/__init__.py
+-rw-r--r--   0        0        0      276 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/fixtures/docker/docker-compose.yml
+-rw-r--r--   0        0        0     4132 2024-04-16 15:52:52.287722 meltano-3.4.0b1/tests/fixtures/docker/snowplow.py
+-rw-r--r--   0        0        0     1535 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/fixtures/fs.py
+-rw-r--r--   0        0        0     3135 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/fixtures/large_config_project/meltano.yml
+-rw-r--r--   0        0        0    30013 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/fixtures/large_config_project/schedule.yml
+-rw-r--r--   0        0        0     1086 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/fixtures/multifile_project/meltano.yml
+-rw-r--r--   0        0        0      469 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/fixtures/multifile_project/subconfig_2.yml
+-rw-r--r--   0        0        0      394 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/fixtures/multifile_project/subfolder/subconfig_1.yml
+-rw-r--r--   0        0        0      631 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/fixtures/plugins/extractors/tap-custom/test.yml
+-rw-r--r--   0        0        0     1136 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/fixtures/utils.py
+-rw-r--r--   0        0        0    31067 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_add.py
+-rw-r--r--   0        0        0    15154 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_cli.py
+-rw-r--r--   0        0        0     5174 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_compile.py
+-rw-r--r--   0        0        0     8595 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_config.py
+-rw-r--r--   0        0        0    42025 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_elt.py
+-rw-r--r--   0        0        0     1585 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_hub.py
+-rw-r--r--   0        0        0     3577 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_initialize.py
+-rw-r--r--   0        0        0    12665 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_install.py
+-rw-r--r--   0        0        0     9285 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_invoke.py
+-rw-r--r--   0        0        0     6777 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_job_cmd.py
+-rw-r--r--   0        0        0     3771 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_lock.py
+-rw-r--r--   0        0        0     1864 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_remove.py
+-rw-r--r--   0        0        0    47456 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_run.py
+-rw-r--r--   0        0        0     8502 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_schedule.py
+-rw-r--r--   0        0        0     1140 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_select.py
+-rw-r--r--   0        0        0    11532 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_state.py
+-rw-r--r--   0        0        0     8268 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/cli/test_upgrade.py
+-rw-r--r--   0        0        0     5381 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/behavior/test_canonical.py
+-rw-r--r--   0        0        0     2155 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/behavior/test_hookable.py
+-rw-r--r--   0        0        0    21766 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/block/test_extract_load.py
+-rw-r--r--   0        0        0      241 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/block/test_parser.py
+-rw-r--r--   0        0        0      933 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/block/test_plugin_command.py
+-rw-r--r--   0        0        0     7736 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/block/test_singer.py
+-rw-r--r--   0        0        0     2302 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/container/test_container_spec.py
+-rw-r--r--   0        0        0     6783 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/hub/test_meltano_hub_service.py
+-rw-r--r--   0        0        0     2076 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/job/test_finder.py
+-rw-r--r--   0        0        0     6240 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/job/test_job.py
+-rw-r--r--   0        0        0     2579 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/job/test_stale_job_failer.py
+-rw-r--r--   0        0        0     3357 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/logging/test_formatters.py
+-rw-r--r--   0        0        0      806 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/logging/test_logging_utils.py
+-rw-r--r--   0        0        0     7398 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/logging/test_output_logger.py
+-rw-r--r--   0        0        0    32051 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/plugin/singer/test_catalog.py
+-rw-r--r--   0        0        0      562 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/plugin/singer/test_mapper.py
+-rw-r--r--   0        0        0    37590 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/plugin/singer/test_tap.py
+-rw-r--r--   0        0        0     3690 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/plugin/singer/test_target.py
+-rw-r--r--   0        0        0     3921 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/plugin/test_airflow.py
+-rw-r--r--   0        0        0     2396 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/plugin/test_command.py
+-rw-r--r--   0        0        0    22146 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/plugin/test_plugin.py
+-rw-r--r--   0        0        0      174 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/plugin/test_plugin_config_service.py
+-rw-r--r--   0        0        0    35208 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/plugin/test_plugin_settings.py
+-rw-r--r--   0        0        0     5963 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/plugin/test_superset.py
+-rw-r--r--   0        0        0     7999 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/runner/test_runner.py
+-rw-r--r--   0        0        0     2807 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/state_store/test_db.py
+-rw-r--r--   0        0        0    21574 2024-04-16 15:52:52.291723 meltano-3.4.0b1/tests/meltano/core/state_store/test_filesystem.py
+-rw-r--r--   0        0        0     6765 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/state_store/test_state_store.py
+-rw-r--r--   0        0        0     1558 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_db_compat.py
+-rw-r--r--   0        0        0     1813 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_db_connection.py
+-rw-r--r--   0        0        0     5217 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_elt_context.py
+-rw-r--r--   0        0        0     2610 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_environment_service.py
+-rw-r--r--   0        0        0    13772 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_environment_variables.py
+-rw-r--r--   0        0        0     2274 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_locked_definition_service.py
+-rw-r--r--   0        0        0     2108 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_meltano_file.py
+-rw-r--r--   0        0        0     3128 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_meltano_invoker.py
+-rw-r--r--   0        0        0     4094 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_plugin_install_service.py
+-rw-r--r--   0        0        0     6101 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_plugin_invoker.py
+-rw-r--r--   0        0        0     3127 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_plugin_lock_service.py
+-rw-r--r--   0        0        0     5749 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_plugin_remove_service.py
+-rw-r--r--   0        0        0     5776 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_plugin_test_service.py
+-rw-r--r--   0        0        0     4319 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_project.py
+-rw-r--r--   0        0        0     8892 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_project_add_service.py
+-rw-r--r--   0        0        0    16326 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_project_files.py
+-rw-r--r--   0        0        0     3281 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_project_init_service.py
+-rw-r--r--   0        0        0     8071 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_project_plugins_service.py
+-rw-r--r--   0        0        0     7238 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_project_settings_service.py
+-rw-r--r--   0        0        0     9759 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_schedule_service.py
+-rw-r--r--   0        0        0     5865 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_setting_definition.py
+-rw-r--r--   0        0        0    22226 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_settings_store.py
+-rw-r--r--   0        0        0     3665 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_state_service.py
+-rw-r--r--   0        0        0     2430 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_task_sets.py
+-rw-r--r--   0        0        0     2645 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_task_sets_service.py
+-rw-r--r--   0        0        0     7126 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_utils.py
+-rw-r--r--   0        0        0     1813 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_validation_service.py
+-rw-r--r--   0        0        0    12257 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/test_venv_service.py
+-rw-r--r--   0        0        0     1980 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/tracking/test_environment_context.py
+-rw-r--r--   0        0        0     5708 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/tracking/test_exception.py
+-rw-r--r--   0        0        0     3061 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/tracking/test_plugins.py
+-rw-r--r--   0        0        0     1271 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/tracking/test_project_context.py
+-rw-r--r--   0        0        0      684 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/tracking/test_schemas.py
+-rw-r--r--   0        0        0    19704 2024-04-16 15:52:52.295723 meltano-3.4.0b1/tests/meltano/core/tracking/test_tracker.py
+-rw-r--r--   0        0        0     9032 1970-01-01 00:00:00.000000 meltano-3.4.0b1/PKG-INFO
```

### Comparing `meltano-3.4.0a2/LICENSE` & `meltano-3.4.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/README.md` & `meltano-3.4.0b1/README.md`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/pyproject.toml` & `meltano-3.4.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meltano"
-version = "3.4.0a2"
+version = "3.4.0b1"
 description = "Meltano is your CLI for ELT+: Open Source, Flexible, and Scalable. Move, transform, and test your data with confidence using a streamlined data engineering workflow you’ll love."
 authors = ["Meltano <hello@meltano.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/meltano/meltano"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
@@ -41,18 +41,18 @@
 
 [tool.poetry.dependencies]
 aiodocker = "^0.21.0"
 alembic = "^1.13.1"
 atomicwrites = "^1.2.1"
 azure-common = {version = "^1.1.28", optional = true}
 azure-core = {version = "^1.30.1", optional = true}
-azure-identity = {version = "^1.15.0", optional = true}
+azure-identity = {version = "^1.16.0", optional = true}
 azure-storage-blob = {version = "^12.19.1", optional = true}
-boto3 = {version = "^1.34.79", optional = true}
-check-jsonschema = "^0.28.1"
+boto3 = {version = "^1.34.84", optional = true}
+check-jsonschema = "^0.28.2"
 click = "^8.1"
 click-default-group = "^1.2.4"
 click-didyoumean = "^0.3.1"
 croniter = "^2.0.3"
 fasteners = "^0.19"
 flatten-dict = "^0"
 google-cloud-storage = {version = ">=1.31.0", optional = true}
@@ -72,15 +72,15 @@
 python-slugify = "^8.0.4"
 python-ulid = "^1.1.0"
 pyyaml = "^6.0.1"
 questionary = "^2.0.1"
 requests = "^2.31.0"
 rich = "^13.7.1"
 "ruamel.yaml" = "^0.18.6"
-setuptools = {version = "^69.2.0", python = ">=3.12"}
+setuptools = {version = "^69.5.1", python = ">=3.12"}
 smart-open = "^7.0.4"
 snowplow-tracker = "^1.0.2"
 sqlalchemy = "^2.0.29"
 structlog = "^24.1.0"
 tabulate = "^0.9.0"
 typing-extensions = "^4.11.0"
 tzlocal = "^5.2"
@@ -97,21 +97,21 @@
 postgres = ["psycopg"]
 psycopg2 = ["psycopg2-binary"]
 s3 = ["boto3"]
 uv = ["uv"]
 
 [tool.poetry.group.dev.dependencies]
 backoff = "^2.1.2"
-black = "^24.3.0"
-boto3-stubs = {extras = ["essential"], version = "1.34.79"}
+black = "^24.4.0"
+boto3-stubs = {extras = ["essential"], version = "1.34.84"}
 bumpversion = "^0.6.0"
 colorama = "^0.4.4"
 coverage = {extras = ["toml"], version = ">=7.3.2,!=7.3.3"}
 freezegun = "^1.4.0"
-hypothesis = "^6.100.0"
+hypothesis = "^6.100.1"
 mock = "^5.0.2"
 moto = "^5.0.5"
 mypy = "^1.9.0"
 pre-commit = "^3.5.0"
 pytest = "^8.1.1"
 pytest-asyncio = "^0.23.6"
 pytest-cov = "^5.0.0"
@@ -470,15 +470,15 @@
 skip_covered = true
 
 [tool.commitizen]
 name = "cz_version_bump"
 prerelease_offset = 1
 tag_format = "v$major.$minor.$patch$prerelease"
 changelog_merge_prerelease = true
-version = "3.4.0a2"
+version = "3.4.0b1"
 version_files = [
   "pyproject.toml:^version =",
   "src/meltano/__init__.py:^__version__ =",
   'docs/package.json:^  "version":',
 ]
 
 [tool.mypy]
```

### Comparing `meltano-3.4.0a2/src/meltano/cli/__init__.py` & `meltano-3.4.0b1/src/meltano/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/cli/add.py` & `meltano-3.4.0b1/src/meltano/cli/add.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/cli/cli.py` & `meltano-3.4.0b1/src/meltano/cli/cli.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/cli/compile.py` & `meltano-3.4.0b1/src/meltano/cli/compile.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/cli/config.py` & `meltano-3.4.0b1/src/meltano/cli/config.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/cli/elt.py` & `meltano-3.4.0b1/src/meltano/cli/elt.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/cli/environment.py` & `meltano-3.4.0b1/src/meltano/cli/environment.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/cli/hub.py` & `meltano-3.4.0b1/src/meltano/cli/hub.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/cli/initialize.py` & `meltano-3.4.0b1/src/meltano/cli/initialize.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/cli/install.py` & `meltano-3.4.0b1/src/meltano/cli/install.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/cli/interactive/config.py` & `meltano-3.4.0b1/src/meltano/cli/interactive/config.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/cli/invoke.py` & `meltano-3.4.0b1/src/meltano/cli/invoke.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/cli/job.py` & `meltano-3.4.0b1/src/meltano/cli/job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/cli/lock.py` & `meltano-3.4.0b1/src/meltano/cli/lock.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/cli/params.py` & `meltano-3.4.0b1/src/meltano/cli/params.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/cli/remove.py` & `meltano-3.4.0b1/src/meltano/cli/remove.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/cli/run.py` & `meltano-3.4.0b1/src/meltano/cli/run.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/cli/schedule.py` & `meltano-3.4.0b1/src/meltano/cli/schedule.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/cli/schema.py` & `meltano-3.4.0b1/src/meltano/cli/schema.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/cli/select.py` & `meltano-3.4.0b1/src/meltano/cli/select.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/cli/state.py` & `meltano-3.4.0b1/src/meltano/cli/state.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/cli/upgrade.py` & `meltano-3.4.0b1/src/meltano/cli/upgrade.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/cli/utils.py` & `meltano-3.4.0b1/src/meltano/cli/utils.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/cli/validate.py` & `meltano-3.4.0b1/src/meltano/cli/validate.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/behavior/canonical.py` & `meltano-3.4.0b1/src/meltano/core/behavior/canonical.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/behavior/hookable.py` & `meltano-3.4.0b1/src/meltano/core/behavior/hookable.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/behavior/versioned.py` & `meltano-3.4.0b1/src/meltano/core/behavior/versioned.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/block/blockset.py` & `meltano-3.4.0b1/src/meltano/core/block/blockset.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/block/extract_load.py` & `meltano-3.4.0b1/src/meltano/core/block/extract_load.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/block/future_utils.py` & `meltano-3.4.0b1/src/meltano/core/block/future_utils.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/block/ioblock.py` & `meltano-3.4.0b1/src/meltano/core/block/ioblock.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/block/parser.py` & `meltano-3.4.0b1/src/meltano/core/block/parser.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/block/plugin_command.py` & `meltano-3.4.0b1/src/meltano/core/block/plugin_command.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/block/singer.py` & `meltano-3.4.0b1/src/meltano/core/block/singer.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/bundle/settings.yml` & `meltano-3.4.0b1/src/meltano/core/bundle/settings.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/cli_messages.py` & `meltano-3.4.0b1/src/meltano/core/cli_messages.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/config_service.py` & `meltano-3.4.0b1/src/meltano/core/config_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/container/container_service.py` & `meltano-3.4.0b1/src/meltano/core/container/container_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/container/container_spec.py` & `meltano-3.4.0b1/src/meltano/core/container/container_spec.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/db.py` & `meltano-3.4.0b1/src/meltano/core/db.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/elt_context.py` & `meltano-3.4.0b1/src/meltano/core/elt_context.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/environment.py` & `meltano-3.4.0b1/src/meltano/core/environment.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/environment_service.py` & `meltano-3.4.0b1/src/meltano/core/environment_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/error.py` & `meltano-3.4.0b1/src/meltano/core/error.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/hub/client.py` & `meltano-3.4.0b1/src/meltano/core/hub/client.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/hub/schema.py` & `meltano-3.4.0b1/src/meltano/core/hub/schema.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/job/finder.py` & `meltano-3.4.0b1/src/meltano/core/job/finder.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/job/job.py` & `meltano-3.4.0b1/src/meltano/core/job/job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/job/stale_job_failer.py` & `meltano-3.4.0b1/src/meltano/core/job/stale_job_failer.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/job_state.py` & `meltano-3.4.0b1/src/meltano/core/job_state.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/locked_definition_service.py` & `meltano-3.4.0b1/src/meltano/core/locked_definition_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/logging/__init__.py` & `meltano-3.4.0b1/src/meltano/core/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/logging/formatters.py` & `meltano-3.4.0b1/src/meltano/core/logging/formatters.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/logging/job_logging_service.py` & `meltano-3.4.0b1/src/meltano/core/logging/job_logging_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/logging/output_logger.py` & `meltano-3.4.0b1/src/meltano/core/logging/output_logger.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/logging/utils.py` & `meltano-3.4.0b1/src/meltano/core/logging/utils.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/manifest/__init__.py` & `meltano-3.4.0b1/src/meltano/core/manifest/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/manifest/contexts.py` & `meltano-3.4.0b1/src/meltano/core/manifest/contexts.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/manifest/jsonschema.py` & `meltano-3.4.0b1/src/meltano/core/manifest/jsonschema.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/manifest/manifest.py` & `meltano-3.4.0b1/src/meltano/core/manifest/manifest.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/meltano_file.py` & `meltano-3.4.0b1/src/meltano/core/meltano_file.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/meltano_invoker.py` & `meltano-3.4.0b1/src/meltano/core/meltano_invoker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/migration_service.py` & `meltano-3.4.0b1/src/meltano/core/migration_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin/airflow.py` & `meltano-3.4.0b1/src/meltano/core/plugin/airflow.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin/base.py` & `meltano-3.4.0b1/src/meltano/core/plugin/base.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin/command.py` & `meltano-3.4.0b1/src/meltano/core/plugin/command.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin/config_service.py` & `meltano-3.4.0b1/src/meltano/core/plugin/config_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin/dbt/base.py` & `meltano-3.4.0b1/src/meltano/core/plugin/dbt/base.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin/error.py` & `meltano-3.4.0b1/src/meltano/core/plugin/error.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin/factory.py` & `meltano-3.4.0b1/src/meltano/core/plugin/factory.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin/file.py` & `meltano-3.4.0b1/src/meltano/core/plugin/file.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin/meltano_file.py` & `meltano-3.4.0b1/src/meltano/core/plugin/meltano_file.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin/project_plugin.py` & `meltano-3.4.0b1/src/meltano/core/plugin/project_plugin.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin/requirements.py` & `meltano-3.4.0b1/src/meltano/core/plugin/requirements.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin/settings_service.py` & `meltano-3.4.0b1/src/meltano/core/plugin/settings_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin/singer/base.py` & `meltano-3.4.0b1/src/meltano/core/plugin/singer/base.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin/singer/catalog.py` & `meltano-3.4.0b1/src/meltano/core/plugin/singer/catalog.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin/singer/mapper.py` & `meltano-3.4.0b1/src/meltano/core/plugin/singer/mapper.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin/singer/tap.py` & `meltano-3.4.0b1/src/meltano/core/plugin/singer/tap.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin/singer/target.py` & `meltano-3.4.0b1/src/meltano/core/plugin/singer/target.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin/superset.py` & `meltano-3.4.0b1/src/meltano/core/plugin/superset.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin_install_service.py` & `meltano-3.4.0b1/src/meltano/core/plugin_install_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -532,15 +532,14 @@
         service = VenvService(
             project=project,
             python=plugin.python,
             namespace=plugin.type,
             name=plugin.venv_name,
         )
     elif backend == "uv":  # pragma: no cover
-        logger.warning("The uv backend is experimental")
         service = UvVenvService(
             project=project,
             python=plugin.python,
             namespace=plugin.type,
             name=plugin.venv_name,
         )
     else:  # pragma: no cover
```

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin_invoker.py` & `meltano-3.4.0b1/src/meltano/core/plugin_invoker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin_location_remove.py` & `meltano-3.4.0b1/src/meltano/core/plugin_location_remove.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin_lock_service.py` & `meltano-3.4.0b1/src/meltano/core/plugin_lock_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin_remove_service.py` & `meltano-3.4.0b1/src/meltano/core/plugin_remove_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin_repository.py` & `meltano-3.4.0b1/src/meltano/core/plugin_repository.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/plugin_test_service.py` & `meltano-3.4.0b1/src/meltano/core/plugin_test_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/project.py` & `meltano-3.4.0b1/src/meltano/core/project.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/project_add_service.py` & `meltano-3.4.0b1/src/meltano/core/project_add_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/project_files.py` & `meltano-3.4.0b1/src/meltano/core/project_files.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/project_init_service.py` & `meltano-3.4.0b1/src/meltano/core/project_init_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/project_plugins_service.py` & `meltano-3.4.0b1/src/meltano/core/project_plugins_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/project_settings_service.py` & `meltano-3.4.0b1/src/meltano/core/project_settings_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/runner/dbt.py` & `meltano-3.4.0b1/src/meltano/core/runner/dbt.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/runner/singer.py` & `meltano-3.4.0b1/src/meltano/core/runner/singer.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/schedule.py` & `meltano-3.4.0b1/src/meltano/core/schedule.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/schedule_service.py` & `meltano-3.4.0b1/src/meltano/core/schedule_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/select_service.py` & `meltano-3.4.0b1/src/meltano/core/select_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/setting.py` & `meltano-3.4.0b1/src/meltano/core/setting.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/setting_definition.py` & `meltano-3.4.0b1/src/meltano/core/setting_definition.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 
 from meltano.core import utils
 from meltano.core.behavior import NameEq
 from meltano.core.behavior.canonical import Canonical
 from meltano.core.error import Error
 
 if t.TYPE_CHECKING:
-    from ruamel.yaml import Representer
+    from ruamel.yaml import Node, Representer, ScalarNode
 
 VALUE_PROCESSORS = {
     "nest_object": utils.nest_object,
     "upcase_string": lambda vlu: vlu.upper(),
     "stringify": lambda vlu: vlu if isinstance(vlu, str) else json.dumps(vlu),
 }
 
 
 class EnvVar:
     """Environment Variable class."""
 
-    def __init__(self, definition: str):
+    def __init__(self, definition: str) -> None:
         """Instantiate new EnvVar.
 
         Args:
             definition: Env var definition.
         """
         key = definition
         negated = False
@@ -66,27 +66,27 @@
         value = env[self.key]
         return str(not utils.truthy(value)) if self.negated else value
 
 
 class SettingMissingError(Error):
     """A setting is missing."""
 
-    def __init__(self, name: str):
+    def __init__(self, name: str) -> None:
         """Instantiate SettingMissingError.
 
         Args:
             name: Name of missing setting.
         """
         super().__init__(f"Cannot find setting {name}")
 
 
 class YAMLEnum(str, Enum):
     """Serializable Enum class."""
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Return as string.
 
         Returns:
             This enum in string form.
         """
         return self.value
 
@@ -100,15 +100,15 @@
 
         Returns:
             Object in yaml string form.
         """
         return dumper.represent_scalar("tag:yaml.org,2002:str", str(obj))
 
     @classmethod
-    def to_yaml(cls, representer: Representer, node: t.Any):
+    def to_yaml(cls, representer: Representer, node: t.Any) -> ScalarNode:
         """Represent as yaml.
 
         Args:
             representer: YAML representer.
             node: Object to dump.
 
         Returns:
@@ -116,16 +116,16 @@
         """
         return representer.represent_scalar("tag:yaml.org,2002:str", str(node))
 
     @classmethod
     def from_yaml(
         cls,
         constructor,  # noqa: ARG003
-        node,
-    ):
+        node: Node,
+    ) -> YAMLEnum:
         """Construct from yaml.
 
         Args:
             constructor: Class constructor.
             node: YAML node.
 
         Returns:
@@ -147,15 +147,15 @@
     OPTIONS = "options"
     FILE = "file"
     ARRAY = "array"
     OBJECT = "object"
     HIDDEN = "hidden"
 
     @cached_property
-    def is_sensitive(self):
+    def is_sensitive(self) -> bool:
         """Return whether the setting kind is sensitive.
 
         Returns:
             True if the setting kind is sensitive.
         """
         return self in {
             SettingKind.PASSWORD,
@@ -165,14 +165,20 @@
 
 ParseValueExpectedType = t.TypeVar("ParseValueExpectedType")
 
 
 class SettingDefinition(NameEq, Canonical):
     """Meltano SettingDefinition class."""
 
+    name: str
+    kind: SettingKind | None
+    hidden: bool
+    sensitive: bool
+    _custom: bool
+
     def __init__(
         self,
         name: str | None = None,
         aliases: list[str] | None = None,
         env: str | None = None,
         env_aliases: list[str] | None = None,
         kind: str | None = None,
@@ -221,16 +227,32 @@
         """
         aliases = aliases or []
         env_aliases = env_aliases or []
         options = options or []
         oauth = oauth or {}
 
         kind = SettingKind(kind) if kind else None
-        hidden = hidden or kind is SettingKind.HIDDEN or None
-        sensitive = sensitive or kind and kind.is_sensitive or None
+
+        # Handle deprecated SettingKind.HIDDEN
+        if kind is SettingKind.HIDDEN:
+            # Override kind if hidden flag is set
+            if hidden:
+                kind = SettingKind.STRING
+
+            # Prioritize kind over flag otherwise
+            hidden = True
+
+        # Handle deprecated SettingKind.PASSWORD and SettingKind.OAUTH
+        if kind and kind.is_sensitive:
+            # Override kind if sensitive flag is set
+            if sensitive:
+                kind = SettingKind.STRING
+
+            # Prioritize kind over flag otherwise
+            sensitive = True
 
         super().__init__(
             # Attributes will be listed in meltano.yml in this order:
             name=name,
             aliases=aliases,
             env=env,
             env_aliases=env_aliases,
@@ -259,15 +281,20 @@
 
         Returns:
             String representation of this setting.
         """
         return f"<SettingDefinition {self.name} ({self.kind})>"
 
     @classmethod
-    def from_missing(cls, defs: t.Iterable[SettingDefinition], config: dict, **kwargs):
+    def from_missing(
+        cls,
+        defs: t.Iterable[SettingDefinition],
+        config: dict,
+        **kwargs,
+    ) -> list[SettingDefinition]:
         """Create SettingDefinition instances for missing settings.
 
         Args:
             defs: Know setting definitions.
             config: Config dict.
             kwargs: Keyword arguments to pass to new SettingDefinition instances.
 
@@ -288,15 +315,15 @@
     @classmethod
     def from_key_value(
         cls,
         key: str,
         value: t.Any,
         custom: bool = True,
         default: t.Any | bool = False,
-    ):
+    ) -> SettingDefinition:
         """Create SettingDefinition instance from key-value pair.
 
         Args:
             key: Key.
             value: Value.
             custom: Custom setting flag.
             default: Default setting value.
```

### Comparing `meltano-3.4.0a2/src/meltano/core/settings_service.py` & `meltano-3.4.0b1/src/meltano/core/settings_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/settings_store.py` & `meltano-3.4.0b1/src/meltano/core/settings_store.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/sqlalchemy.py` & `meltano-3.4.0b1/src/meltano/core/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/state_service.py` & `meltano-3.4.0b1/src/meltano/core/state_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/state_store/__init__.py` & `meltano-3.4.0b1/src/meltano/core/state_store/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/state_store/azure.py` & `meltano-3.4.0b1/src/meltano/core/state_store/azure.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/state_store/base.py` & `meltano-3.4.0b1/src/meltano/core/state_store/base.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/state_store/db.py` & `meltano-3.4.0b1/src/meltano/core/state_store/db.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/state_store/filesystem.py` & `meltano-3.4.0b1/src/meltano/core/state_store/filesystem.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/state_store/google.py` & `meltano-3.4.0b1/src/meltano/core/state_store/google.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/state_store/s3.py` & `meltano-3.4.0b1/src/meltano/core/state_store/s3.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/task_sets.py` & `meltano-3.4.0b1/src/meltano/core/task_sets.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/task_sets_service.py` & `meltano-3.4.0b1/src/meltano/core/task_sets_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/README.md` & `meltano-3.4.0b1/src/meltano/core/tracking/README.md`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/contexts/cli.py` & `meltano-3.4.0b1/src/meltano/core/tracking/contexts/cli.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/contexts/environment.py` & `meltano-3.4.0b1/src/meltano/core/tracking/contexts/environment.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/contexts/exception.py` & `meltano-3.4.0b1/src/meltano/core/tracking/contexts/exception.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/contexts/plugins.py` & `meltano-3.4.0b1/src/meltano/core/tracking/contexts/plugins.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/contexts/project.py` & `meltano-3.4.0b1/src/meltano/core/tracking/contexts/project.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/block_event/jsonschema/1-0-0` & `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/block_event/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-0-0` & `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-1-0` & `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-1-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-0` & `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-1` & `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-1`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-0-0` & `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-1-0` & `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-1-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-2-0` & `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-2-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-3-0` & `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-3-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exception_context/jsonschema/1-0-0` & `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exception_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-0` & `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-1` & `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-1`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/plugins_context/jsonschema/1-0-0` & `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/plugins_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-0-0` & `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-1-0` & `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-1-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/telemetry_state_change_event/jsonschema/1-0-0` & `meltano-3.4.0b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/telemetry_state_change_event/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/micro.conf` & `meltano-3.4.0b1/src/meltano/core/tracking/micro.conf`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/schemas.py` & `meltano-3.4.0b1/src/meltano/core/tracking/schemas.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/tracking/tracker.py` & `meltano-3.4.0b1/src/meltano/core/tracking/tracker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/transform_add_service.py` & `meltano-3.4.0b1/src/meltano/core/transform_add_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/upgrade_service.py` & `meltano-3.4.0b1/src/meltano/core/upgrade_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/utils/__init__.py` & `meltano-3.4.0b1/src/meltano/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/utils/pidfile.py` & `meltano-3.4.0b1/src/meltano/core/utils/pidfile.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/validation_service.py` & `meltano-3.4.0b1/src/meltano/core/validation_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/core/venv_service.py` & `meltano-3.4.0b1/src/meltano/core/venv_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import platform
 import shlex
 import shutil
 import subprocess
 import sys
 import typing as t
 from asyncio.subprocess import Process
-from functools import cached_property
+from functools import cached_property, lru_cache
 from numbers import Number
 from pathlib import Path
 
 from meltano.core.error import AsyncSubprocessError, MeltanoError
 
 if t.TYPE_CHECKING:
     from collections.abc import Iterable
@@ -37,14 +37,62 @@
 
 
 logger = logging.getLogger(__name__)
 
 StdErrExtractor: TypeAlias = t.Callable[[Process], t.Awaitable[t.Union[str, None]]]
 
 
+@lru_cache(maxsize=None)
+def find_uv() -> str:
+    """Find the `uv` executable.
+
+    Tries to import the `uv` package and use its `find_uv_bin` function to find the
+    `uv` executable. If that fails, falls back to using the `uv` executable on the
+    system PATH. If it can't be found on the PATH, returns `"uv"`.
+
+    Adapted from https://github.com/wntrblm/nox/blob/55c7eaf2eb03feb4a4b79e74966c542b75d61401/nox/virtualenv.py#L42-L54.
+
+    Copyright 2016 Alethea Katherine Flowers
+
+    Licensed under the Apache License, Version 2.0 (the "License");
+    you may not use this file except in compliance with the License.
+    You may obtain a copy of the License at
+
+        http://www.apache.org/licenses/LICENSE-2.0
+
+    Unless required by applicable law or agreed to in writing, software
+    distributed under the License is distributed on an "AS IS" BASIS,
+    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+    See the License for the specific language governing permissions and
+    limitations under the License.
+
+    Returns:
+        A string representing the path to the `uv` executable.
+
+    Raises:
+        MeltanoError: The `uv` executable could not be found.
+    """
+    logger.warning("The uv backend is experimental")
+
+    with contextlib.suppress(ImportError, FileNotFoundError):
+        from uv import find_uv_bin
+
+        return find_uv_bin()
+
+    # Fall back to PATH.
+    uv = shutil.which("uv")
+
+    if not uv:
+        error = "Could not find the 'uv' executable"
+        instruction = "Please install 'meltano[uv]' or install 'uv' globally."
+        raise MeltanoError(error, instruction)
+
+    return uv
+
+
 class VirtualEnv:
     """Info about a single virtual environment."""
 
     _SUPPORTED_PLATFORMS = {
         "Linux",
         "Darwin",
         "Windows",
@@ -567,68 +615,23 @@
         except AsyncSubprocessError as err:  # noqa: WPS329
             raise await self.handle_installation_error(err) from err
 
 
 class UvVenvService(VenvService):
     """Manages virtual environments using `uv`."""
 
-    @staticmethod
-    def _find_uv() -> str:  # noqa: WPS605
-        """Find the `uv` executable.
-
-        Tries to import the `uv` package and use its `find_uv_bin` function to find the
-        `uv` executable. If that fails, falls back to using the `uv` executable on the
-        system PATH. If it can't be found on the PATH, returns `"uv"`.
-
-        Adapted from https://github.com/wntrblm/nox/blob/55c7eaf2eb03feb4a4b79e74966c542b75d61401/nox/virtualenv.py#L42-L54.
-
-        Copyright 2016 Alethea Katherine Flowers
-
-        Licensed under the Apache License, Version 2.0 (the "License");
-        you may not use this file except in compliance with the License.
-        You may obtain a copy of the License at
-
-           http://www.apache.org/licenses/LICENSE-2.0
-
-        Unless required by applicable law or agreed to in writing, software
-        distributed under the License is distributed on an "AS IS" BASIS,
-        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-        See the License for the specific language governing permissions and
-        limitations under the License.
-
-        Returns:
-            A string representing the path to the `uv` executable.
-
-        Raises:
-            MeltanoError: The `uv` executable could not be found.
-        """
-        with contextlib.suppress(ImportError, FileNotFoundError):
-            from uv import find_uv_bin
-
-            return find_uv_bin()
-
-        # Fall back to PATH.
-        uv = shutil.which("uv")
-
-        if not uv:
-            error = "Could not find the 'uv' executable"
-            instruction = "Please install 'meltano[uv]' or install 'uv' globally."
-            raise MeltanoError(error, instruction)
-
-        return uv
-
     def __init__(self, *args: t.Any, **kwargs: t.Any):
         """Initialize the `UvVenvService`.
 
         Args:
             args: Positional arguments for the VenvService.
             kwargs: Keyword arguments for the VenvService.
         """
         super().__init__(*args, **kwargs)
-        self.uv = self._find_uv()
+        self.uv = find_uv()
         logger.debug("Using uv executable at %s", self.uv)
 
     @override
     async def upgrade_installer(
         self,
         *,
         env: dict[str, str | None] | None = None,
```

### Comparing `meltano-3.4.0a2/src/meltano/core/yaml.py` & `meltano-3.4.0b1/src/meltano/core/yaml.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/migrations/env.py` & `meltano-3.4.0b1/src/meltano/migrations/env.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/migrations/utils/dialect_typing.py` & `meltano-3.4.0b1/src/meltano/migrations/utils/dialect_typing.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/migrations/versions/13e8639c6d2b_add_state_edit_to_job_state_enum.py` & `meltano-3.4.0b1/src/meltano/migrations/versions/13e8639c6d2b_add_state_edit_to_job_state_enum.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/migrations/versions/23ea52e6d784_add_resource_type_to_embed_token.py` & `meltano-3.4.0b1/src/meltano/migrations/versions/23ea52e6d784_add_resource_type_to_embed_token.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/migrations/versions/367228df6a43_add_trigger_to_job.py` & `meltano-3.4.0b1/src/meltano/migrations/versions/367228df6a43_add_trigger_to_job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/migrations/versions/53e97221d99f_add_run_id_to_job.py` & `meltano-3.4.0b1/src/meltano/migrations/versions/53e97221d99f_add_run_id_to_job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/migrations/versions/5b43800443d1_rename_job_to_job_run_and_job_id_to_job_.py` & `meltano-3.4.0b1/src/meltano/migrations/versions/5b43800443d1_rename_job_to_job_run_and_job_id_to_job_.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/migrations/versions/6828cc5b1a4f_create_dedicated_state_table.py` & `meltano-3.4.0b1/src/meltano/migrations/versions/6828cc5b1a4f_create_dedicated_state_table.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/migrations/versions/6ef30ab7b8e5_.py` & `meltano-3.4.0b1/src/meltano/migrations/versions/6ef30ab7b8e5_.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/migrations/versions/87d9638f6ac6_add_subscription.py` & `meltano-3.4.0b1/src/meltano/migrations/versions/87d9638f6ac6_add_subscription.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/migrations/versions/990c0665f3ce_ensure_user_login_count_default_value.py` & `meltano-3.4.0b1/src/meltano/migrations/versions/990c0665f3ce_ensure_user_login_count_default_value.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/migrations/versions/a3e2b0a4937d_add_login_audit_columns.py` & `meltano-3.4.0b1/src/meltano/migrations/versions/a3e2b0a4937d_add_login_audit_columns.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/migrations/versions/b4c05e463b53_.py` & `meltano-3.4.0b1/src/meltano/migrations/versions/b4c05e463b53_.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/migrations/versions/ceb00d7ff3bd_create_the_embedtoken_table.py` & `meltano-3.4.0b1/src/meltano/migrations/versions/ceb00d7ff3bd_create_the_embedtoken_table.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/migrations/versions/d135f52a6f49_add_last_heartbeat_at_column_to_job.py` & `meltano-3.4.0b1/src/meltano/migrations/versions/d135f52a6f49_add_last_heartbeat_at_column_to_job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/migrations/versions/e4fbabc3fed6_add_last_activity_at_column.py` & `meltano-3.4.0b1/src/meltano/migrations/versions/e4fbabc3fed6_add_last_activity_at_column.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/src/meltano/schemas/meltano.schema.json` & `meltano-3.4.0b1/src/meltano/schemas/meltano.schema.json`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/conftest.py` & `meltano-3.4.0b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/fixtures/cli.py` & `meltano-3.4.0b1/tests/fixtures/cli.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/fixtures/core.py` & `meltano-3.4.0b1/tests/fixtures/core.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/fixtures/db/__init__.py` & `meltano-3.4.0b1/tests/fixtures/db/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/fixtures/db/mssql.py` & `meltano-3.4.0b1/tests/fixtures/db/mssql.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/fixtures/db/postgresql.py` & `meltano-3.4.0b1/tests/fixtures/db/postgresql.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/fixtures/db/postgresql_psycopg3.py` & `meltano-3.4.0b1/tests/fixtures/db/postgresql_psycopg3.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/fixtures/docker/__init__.py` & `meltano-3.4.0b1/tests/fixtures/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/fixtures/docker/snowplow.py` & `meltano-3.4.0b1/tests/fixtures/docker/snowplow.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/fixtures/fs.py` & `meltano-3.4.0b1/tests/fixtures/fs.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/fixtures/large_config_project/meltano.yml` & `meltano-3.4.0b1/tests/fixtures/large_config_project/meltano.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/fixtures/large_config_project/schedule.yml` & `meltano-3.4.0b1/tests/fixtures/large_config_project/schedule.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/fixtures/multifile_project/meltano.yml` & `meltano-3.4.0b1/tests/fixtures/multifile_project/meltano.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/fixtures/plugins/extractors/tap-custom/test.yml` & `meltano-3.4.0b1/tests/fixtures/plugins/extractors/tap-custom/test.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/fixtures/utils.py` & `meltano-3.4.0b1/tests/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/cli/test_add.py` & `meltano-3.4.0b1/tests/meltano/cli/test_add.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/cli/test_cli.py` & `meltano-3.4.0b1/tests/meltano/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/cli/test_compile.py` & `meltano-3.4.0b1/tests/meltano/cli/test_compile.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/cli/test_config.py` & `meltano-3.4.0b1/tests/meltano/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/cli/test_elt.py` & `meltano-3.4.0b1/tests/meltano/cli/test_elt.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/cli/test_hub.py` & `meltano-3.4.0b1/tests/meltano/cli/test_hub.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/cli/test_initialize.py` & `meltano-3.4.0b1/tests/meltano/cli/test_initialize.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/cli/test_install.py` & `meltano-3.4.0b1/tests/meltano/cli/test_install.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/cli/test_invoke.py` & `meltano-3.4.0b1/tests/meltano/cli/test_invoke.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/cli/test_job_cmd.py` & `meltano-3.4.0b1/tests/meltano/cli/test_job_cmd.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/cli/test_lock.py` & `meltano-3.4.0b1/tests/meltano/cli/test_lock.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/cli/test_remove.py` & `meltano-3.4.0b1/tests/meltano/cli/test_remove.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/cli/test_run.py` & `meltano-3.4.0b1/tests/meltano/cli/test_run.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/cli/test_schedule.py` & `meltano-3.4.0b1/tests/meltano/cli/test_schedule.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/cli/test_select.py` & `meltano-3.4.0b1/tests/meltano/cli/test_select.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/cli/test_state.py` & `meltano-3.4.0b1/tests/meltano/cli/test_state.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/cli/test_upgrade.py` & `meltano-3.4.0b1/tests/meltano/cli/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/behavior/test_canonical.py` & `meltano-3.4.0b1/tests/meltano/core/behavior/test_canonical.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/behavior/test_hookable.py` & `meltano-3.4.0b1/tests/meltano/core/behavior/test_hookable.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/block/test_extract_load.py` & `meltano-3.4.0b1/tests/meltano/core/block/test_extract_load.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/block/test_plugin_command.py` & `meltano-3.4.0b1/tests/meltano/core/block/test_plugin_command.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/block/test_singer.py` & `meltano-3.4.0b1/tests/meltano/core/block/test_singer.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/container/test_container_spec.py` & `meltano-3.4.0b1/tests/meltano/core/container/test_container_spec.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/hub/test_meltano_hub_service.py` & `meltano-3.4.0b1/tests/meltano/core/hub/test_meltano_hub_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/job/test_finder.py` & `meltano-3.4.0b1/tests/meltano/core/job/test_finder.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/job/test_job.py` & `meltano-3.4.0b1/tests/meltano/core/job/test_job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/job/test_stale_job_failer.py` & `meltano-3.4.0b1/tests/meltano/core/job/test_stale_job_failer.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/logging/test_formatters.py` & `meltano-3.4.0b1/tests/meltano/core/logging/test_formatters.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/logging/test_logging_utils.py` & `meltano-3.4.0b1/tests/meltano/core/logging/test_logging_utils.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/logging/test_output_logger.py` & `meltano-3.4.0b1/tests/meltano/core/logging/test_output_logger.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/plugin/singer/test_catalog.py` & `meltano-3.4.0b1/tests/meltano/core/plugin/singer/test_catalog.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/plugin/singer/test_mapper.py` & `meltano-3.4.0b1/tests/meltano/core/plugin/singer/test_mapper.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/plugin/singer/test_tap.py` & `meltano-3.4.0b1/tests/meltano/core/plugin/singer/test_tap.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/plugin/singer/test_target.py` & `meltano-3.4.0b1/tests/meltano/core/plugin/singer/test_target.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/plugin/test_airflow.py` & `meltano-3.4.0b1/tests/meltano/core/plugin/test_airflow.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/plugin/test_command.py` & `meltano-3.4.0b1/tests/meltano/core/plugin/test_command.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/plugin/test_plugin.py` & `meltano-3.4.0b1/tests/meltano/core/plugin/test_plugin.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/plugin/test_plugin_settings.py` & `meltano-3.4.0b1/tests/meltano/core/plugin/test_plugin_settings.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/plugin/test_superset.py` & `meltano-3.4.0b1/tests/meltano/core/plugin/test_superset.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/runner/test_runner.py` & `meltano-3.4.0b1/tests/meltano/core/runner/test_runner.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/state_store/test_db.py` & `meltano-3.4.0b1/tests/meltano/core/state_store/test_db.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/state_store/test_filesystem.py` & `meltano-3.4.0b1/tests/meltano/core/state_store/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/state_store/test_state_store.py` & `meltano-3.4.0b1/tests/meltano/core/state_store/test_state_store.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_db_compat.py` & `meltano-3.4.0b1/tests/meltano/core/test_db_compat.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_db_connection.py` & `meltano-3.4.0b1/tests/meltano/core/test_db_connection.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_elt_context.py` & `meltano-3.4.0b1/tests/meltano/core/test_elt_context.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_environment_service.py` & `meltano-3.4.0b1/tests/meltano/core/test_environment_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_environment_variables.py` & `meltano-3.4.0b1/tests/meltano/core/test_environment_variables.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_locked_definition_service.py` & `meltano-3.4.0b1/tests/meltano/core/test_locked_definition_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_meltano_file.py` & `meltano-3.4.0b1/tests/meltano/core/test_meltano_file.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_meltano_invoker.py` & `meltano-3.4.0b1/tests/meltano/core/test_meltano_invoker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_plugin_install_service.py` & `meltano-3.4.0b1/tests/meltano/core/test_plugin_install_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_plugin_invoker.py` & `meltano-3.4.0b1/tests/meltano/core/test_plugin_invoker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_plugin_lock_service.py` & `meltano-3.4.0b1/tests/meltano/core/test_plugin_lock_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_plugin_remove_service.py` & `meltano-3.4.0b1/tests/meltano/core/test_plugin_remove_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_plugin_test_service.py` & `meltano-3.4.0b1/tests/meltano/core/test_plugin_test_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_project.py` & `meltano-3.4.0b1/tests/meltano/core/test_project.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_project_add_service.py` & `meltano-3.4.0b1/tests/meltano/core/test_project_add_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_project_files.py` & `meltano-3.4.0b1/tests/meltano/core/test_project_files.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_project_init_service.py` & `meltano-3.4.0b1/tests/meltano/core/test_project_init_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_project_plugins_service.py` & `meltano-3.4.0b1/tests/meltano/core/test_project_plugins_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_project_settings_service.py` & `meltano-3.4.0b1/tests/meltano/core/test_project_settings_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_schedule_service.py` & `meltano-3.4.0b1/tests/meltano/core/test_schedule_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_settings_store.py` & `meltano-3.4.0b1/tests/meltano/core/test_settings_store.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_state_service.py` & `meltano-3.4.0b1/tests/meltano/core/test_state_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_task_sets.py` & `meltano-3.4.0b1/tests/meltano/core/test_task_sets.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_task_sets_service.py` & `meltano-3.4.0b1/tests/meltano/core/test_task_sets_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_utils.py` & `meltano-3.4.0b1/tests/meltano/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_validation_service.py` & `meltano-3.4.0b1/tests/meltano/core/test_validation_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/test_venv_service.py` & `meltano-3.4.0b1/tests/meltano/core/test_venv_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import mock
 import pytest
 
 from meltano.core.error import AsyncSubprocessError, MeltanoError
 from meltano.core.plugin import PluginType
 from meltano.core.plugin.project_plugin import ProjectPlugin
 from meltano.core.plugin_install_service import install_pip_plugin
-from meltano.core.venv_service import UvVenvService, VenvService, VirtualEnv
+from meltano.core.venv_service import UvVenvService, VenvService, VirtualEnv, find_uv
 
 if t.TYPE_CHECKING:
     from meltano.core.project import Project
 
 
 def _check_venv_created_with_python(project: Project, python: str | None):
     with mock.patch(
@@ -277,40 +277,44 @@
         ):
             VirtualEnv(root, python="test-python-executable")
 
 
 class TestUvVenvService:
     @pytest.fixture()
     def subject(self, project):
+        find_uv.cache_clear()
         return UvVenvService(project=project, namespace="namespace", name="name")
 
-    def test_find_uv_builtin(self, project: Project, monkeypatch: pytest.MonkeyPatch):
+    def test_find_uv_builtin(self, monkeypatch: pytest.MonkeyPatch):
+        find_uv.cache_clear()
         monkeypatch.setattr("uv.find_uv_bin", lambda: "/usr/bin/uv")
-        service = UvVenvService(project=project, namespace="namespace", name="name")
-        assert service.uv == "/usr/bin/uv"
+        assert find_uv() == "/usr/bin/uv"
+
+    def test_find_uv_global(self, monkeypatch: pytest.MonkeyPatch):
+        find_uv.cache_clear()
 
-    def test_find_uv_global(self, project: Project, monkeypatch: pytest.MonkeyPatch):
         def raise_import_error():
             raise ImportError
 
         monkeypatch.setattr("uv.find_uv_bin", raise_import_error)
         monkeypatch.setattr("shutil.which", lambda _: "/usr/bin/uv")
 
-        service = UvVenvService(project=project, namespace="namespace", name="name")
-        assert service.uv == "/usr/bin/uv"
+        assert find_uv() == "/usr/bin/uv"
+
+    def test_find_uv_not_found(self, monkeypatch: pytest.MonkeyPatch):
+        find_uv.cache_clear()
 
-    def test_find_uv_not_found(self, project: Project, monkeypatch: pytest.MonkeyPatch):
         def raise_import_error():
             raise ImportError
 
         monkeypatch.setattr("uv.find_uv_bin", raise_import_error)
         monkeypatch.setattr("shutil.which", lambda _: None)
 
         with pytest.raises(MeltanoError, match="Could not find the 'uv' executable"):
-            UvVenvService(project=project, namespace="namespace", name="name")
+            find_uv()
 
     @pytest.mark.asyncio()
     @pytest.mark.usefixtures("project")
     async def test_install(self, subject: UvVenvService):
         # Make sure the venv exists already
         await subject.install(["cowsay"], clean=True)
```

### Comparing `meltano-3.4.0a2/tests/meltano/core/tracking/test_environment_context.py` & `meltano-3.4.0b1/tests/meltano/core/tracking/test_environment_context.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/tracking/test_exception.py` & `meltano-3.4.0b1/tests/meltano/core/tracking/test_exception.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/tracking/test_plugins.py` & `meltano-3.4.0b1/tests/meltano/core/tracking/test_plugins.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/tracking/test_project_context.py` & `meltano-3.4.0b1/tests/meltano/core/tracking/test_project_context.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/tracking/test_schemas.py` & `meltano-3.4.0b1/tests/meltano/core/tracking/test_schemas.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/tests/meltano/core/tracking/test_tracker.py` & `meltano-3.4.0b1/tests/meltano/core/tracking/test_tracker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a2/PKG-INFO` & `meltano-3.4.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meltano
-Version: 3.4.0a2
+Version: 3.4.0b1
 Summary: Meltano is your CLI for ELT+: Open Source, Flexible, and Scalable. Move, transform, and test your data with confidence using a streamlined data engineering workflow you’ll love.
 Home-page: https://meltano.com
 License: MIT
 Keywords: Meltano,ELT,Data integration,singer-io,dbt
 Author: Meltano
 Author-email: hello@meltano.com
 Requires-Python: >=3.8,<3.13
@@ -26,18 +26,18 @@
 Provides-Extra: s3
 Provides-Extra: uv
 Requires-Dist: aiodocker (>=0.21.0,<0.22.0)
 Requires-Dist: alembic (>=1.13.1,<2.0.0)
 Requires-Dist: atomicwrites (>=1.2.1,<2.0.0)
 Requires-Dist: azure-common (>=1.1.28,<2.0.0) ; extra == "azure"
 Requires-Dist: azure-core (>=1.30.1,<2.0.0) ; extra == "azure"
-Requires-Dist: azure-identity (>=1.15.0,<2.0.0) ; extra == "azure"
+Requires-Dist: azure-identity (>=1.16.0,<2.0.0) ; extra == "azure"
 Requires-Dist: azure-storage-blob (>=12.19.1,<13.0.0) ; extra == "azure"
-Requires-Dist: boto3 (>=1.34.79,<2.0.0) ; extra == "s3"
-Requires-Dist: check-jsonschema (>=0.28.1,<0.29.0)
+Requires-Dist: boto3 (>=1.34.84,<2.0.0) ; extra == "s3"
+Requires-Dist: check-jsonschema (>=0.28.2,<0.29.0)
 Requires-Dist: click (>=8.1,<9.0)
 Requires-Dist: click-default-group (>=1.2.4,<2.0.0)
 Requires-Dist: click-didyoumean (>=0.3.1,<0.4.0)
 Requires-Dist: croniter (>=2.0.3,<3.0.0)
 Requires-Dist: fasteners (>=0.19,<0.20)
 Requires-Dist: flatten-dict (>=0,<1)
 Requires-Dist: google-cloud-storage (>=1.31.0) ; extra == "gcs"
@@ -56,15 +56,15 @@
 Requires-Dist: python-slugify (>=8.0.4,<9.0.0)
 Requires-Dist: python-ulid (>=1.1.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: questionary (>=2.0.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: ruamel.yaml (>=0.18.6,<0.19.0)
-Requires-Dist: setuptools (>=69.2.0,<70.0.0) ; python_version >= "3.12"
+Requires-Dist: setuptools (>=69.5.1,<70.0.0) ; python_version >= "3.12"
 Requires-Dist: smart-open (>=7.0.4,<8.0.0)
 Requires-Dist: snowplow-tracker (>=1.0.2,<2.0.0)
 Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
 Requires-Dist: structlog (>=24.1.0,<25.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
 Requires-Dist: tzlocal (>=5.2,<6.0)
```

