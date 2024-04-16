# Comparing `tmp/pinjected-0.2.34.tar.gz` & `tmp/pinjected-0.2.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinjected-0.2.34.tar", max compression
+gzip compressed data, was "pinjected-0.2.35.tar", max compression
```

## Comparing `pinjected-0.2.34.tar` & `pinjected-0.2.35.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.34/LICENSE
--rw-r--r--   0        0        0      457 2024-01-10 03:58:40.481212 pinjected-0.2.34/pinjected/__init__.py
--rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.34/pinjected/__main__.py
--rw-r--r--   0        0        0      994 2024-04-16 04:30:55.994066 pinjected-0.2.34/pinjected/decoration.py
--rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.34/pinjected/demo.py
--rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.34/pinjected/di/__init__.py
--rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.34/pinjected/di/app_designed.py
--rw-r--r--   0        0        0     5664 2024-04-02 03:27:58.890219 pinjected-0.2.34/pinjected/di/app_injected.py
--rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.34/pinjected/di/applicative.py
--rw-r--r--   0        0        0     7340 2024-03-26 02:52:38.836702 pinjected-0.2.34/pinjected/di/ast.py
--rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.34/pinjected/di/async_injected.py
--rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.34/pinjected/di/bindings.py
--rw-r--r--   0        0        0     9753 2024-03-26 02:52:38.838842 pinjected-0.2.34/pinjected/di/decorators.py
--rw-r--r--   0        0        0    13317 2024-03-26 02:52:38.839976 pinjected-0.2.34/pinjected/di/design.py
--rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.34/pinjected/di/design_bind_contextx.py
--rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.34/pinjected/di/designed.py
--rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.34/pinjected/di/dynamic_proxy.py
--rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.34/pinjected/di/graph.py
--rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.34/pinjected/di/implicit_globals.py
--rw-r--r--   0        0        0    54209 2024-04-16 06:03:24.715277 pinjected-0.2.34/pinjected/di/injected.py
--rw-r--r--   0        0        0     1892 2023-11-06 06:59:52.887127 pinjected-0.2.34/pinjected/di/injected_analysis.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.34/pinjected/di/metadata/__init__.py
--rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.34/pinjected/di/metadata/bind_metadata.py
--rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.34/pinjected/di/metadata/location_data.py
--rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.34/pinjected/di/modular_injected.py
--rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.34/pinjected/di/monadic.py
--rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.34/pinjected/di/overload_experimental.py
--rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.34/pinjected/di/playground.py
--rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.34/pinjected/di/provider.py
--rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.34/pinjected/di/proxiable.py
--rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.34/pinjected/di/session.py
--rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.34/pinjected/di/sessioned.py
--rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.34/pinjected/di/static_proxy.py
--rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.34/pinjected/di/test_ast.py
--rw-r--r--   0        0        0      997 2024-03-26 02:52:38.844108 pinjected-0.2.34/pinjected/di/test_dynamic_proxy.py
--rw-r--r--   0        0        0     1500 2024-03-20 13:37:29.443496 pinjected-0.2.34/pinjected/di/test_graph.py
--rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.34/pinjected/di/test_injected.py
--rw-r--r--   0        0        0      452 2024-03-26 02:52:38.845073 pinjected-0.2.34/pinjected/di/test_proxiable.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.34/pinjected/di/tools/__init__.py
--rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.34/pinjected/di/tools/add_overload.py
--rw-r--r--   0        0        0    15106 2024-03-26 02:52:38.846281 pinjected-0.2.34/pinjected/di/util.py
--rw-r--r--   0        0        0     1071 2023-08-25 06:23:59.157878 pinjected-0.2.34/pinjected/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.34/pinjected/exporter/__init__.py
--rw-r--r--   0        0        0      409 2024-04-16 06:03:24.715733 pinjected-0.2.34/pinjected/exporter/llm_export_v2.py
--rw-r--r--   0        0        0    31457 2024-04-16 12:00:54.455268 pinjected-0.2.34/pinjected/exporter/llm_exporter.py
--rw-r--r--   0        0        0     2216 2024-04-16 09:23:13.383068 pinjected-0.2.34/pinjected/exporter/optimize_import_stmts.py
--rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.34/pinjected/global_configs.py
--rw-r--r--   0        0        0     2927 2024-03-26 02:52:38.847411 pinjected-0.2.34/pinjected/graph_inspection.py
--rw-r--r--   0        0        0     2886 2024-04-15 04:38:55.875181 pinjected-0.2.34/pinjected/helper_structure.py
--rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.34/pinjected/helpers.py
--rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.34/pinjected/ide_supports/__init__.py
--rw-r--r--   0        0        0     9050 2024-01-10 03:58:40.484651 pinjected-0.2.34/pinjected/ide_supports/console_run_helper.py
--rw-r--r--   0        0        0     7287 2024-04-16 09:18:34.207695 pinjected-0.2.34/pinjected/ide_supports/create_configs.py
--rw-r--r--   0        0        0     1304 2024-04-16 09:21:04.827442 pinjected-0.2.34/pinjected/ide_supports/default_design.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.34/pinjected/llm_support/__init__.py
--rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.34/pinjected/llm_support/inspect_module.py
--rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.34/pinjected/llm_support/inspect_module_prompts.py
--rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.34/pinjected/logging_helper.py
--rw-r--r--   0        0        0     4121 2024-04-08 10:32:08.774921 pinjected-0.2.34/pinjected/main_impl.py
--rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.34/pinjected/maybe_patch.py
--rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.34/pinjected/meta_main.py
--rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.34/pinjected/module_helper.py
--rw-r--r--   0        0        0     2453 2024-04-15 03:39:25.763167 pinjected-0.2.34/pinjected/module_inspector.py
--rw-r--r--   0        0        0     4862 2024-04-16 09:26:56.419338 pinjected-0.2.34/pinjected/module_var_path.py
--rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.34/pinjected/notification.py
--rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.34/pinjected/nx_graph_util.py
--rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.34/pinjected/providable.py
--rw-r--r--   0        0        0    21320 2024-04-16 09:02:24.191362 pinjected-0.2.34/pinjected/run_config_utils.py
--rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.34/pinjected/run_config_utils_v2.py
--rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.34/pinjected/run_helpers/__init__.py
--rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.34/pinjected/run_helpers/config.py
--rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.34/pinjected/run_helpers/pinjected_environments.py
--rw-r--r--   0        0        0     9360 2024-04-15 05:43:18.485943 pinjected-0.2.34/pinjected/run_helpers/run_injected.py
--rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.34/pinjected/runnables.py
--rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.34/pinjected/test_package/__init__.py
--rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.34/pinjected/test_package/child/__init__.py
--rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.34/pinjected/test_package/child/module1.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.34/pinjected/v2/__init__.py
--rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.34/pinjected/v2/ainjected.py
--rw-r--r--   0        0        0     6128 2024-03-26 02:52:38.850654 pinjected-0.2.34/pinjected/v2/binds.py
--rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.34/pinjected/v2/di.py
--rw-r--r--   0        0        0      358 2024-03-26 02:52:38.851474 pinjected-0.2.34/pinjected/v2/keys.py
--rw-r--r--   0        0        0      478 2024-03-26 02:52:38.851836 pinjected-0.2.34/pinjected/v2/provide_context.py
--rw-r--r--   0        0        0     5647 2024-03-29 04:40:41.000002 pinjected-0.2.34/pinjected/v2/resolver.py
--rw-r--r--   0        0        0    19384 2024-03-26 02:52:38.852889 pinjected-0.2.34/pinjected/visualize_di.py
--rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.34/pinjected/viz/__init__.py
--rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.34/pinjected/viz/graph.py
--rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.34/pinjected/with_context.py
--rw-r--r--   0        0        0      759 2024-04-16 12:00:58.208838 pinjected-0.2.34/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 pinjected-0.2.34/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.35/LICENSE
+-rw-r--r--   0        0        0      457 2024-01-10 03:58:40.481212 pinjected-0.2.35/pinjected/__init__.py
+-rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.35/pinjected/__main__.py
+-rw-r--r--   0        0        0      994 2024-04-16 04:30:55.994066 pinjected-0.2.35/pinjected/decoration.py
+-rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.35/pinjected/demo.py
+-rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.35/pinjected/di/__init__.py
+-rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.35/pinjected/di/app_designed.py
+-rw-r--r--   0        0        0     5664 2024-04-02 03:27:58.890219 pinjected-0.2.35/pinjected/di/app_injected.py
+-rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.35/pinjected/di/applicative.py
+-rw-r--r--   0        0        0     7340 2024-03-26 02:52:38.836702 pinjected-0.2.35/pinjected/di/ast.py
+-rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.35/pinjected/di/async_injected.py
+-rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.35/pinjected/di/bindings.py
+-rw-r--r--   0        0        0     9753 2024-03-26 02:52:38.838842 pinjected-0.2.35/pinjected/di/decorators.py
+-rw-r--r--   0        0        0    13317 2024-03-26 02:52:38.839976 pinjected-0.2.35/pinjected/di/design.py
+-rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.35/pinjected/di/design_bind_contextx.py
+-rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.35/pinjected/di/designed.py
+-rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.35/pinjected/di/dynamic_proxy.py
+-rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.35/pinjected/di/graph.py
+-rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.35/pinjected/di/implicit_globals.py
+-rw-r--r--   0        0        0    54209 2024-04-16 06:03:24.715277 pinjected-0.2.35/pinjected/di/injected.py
+-rw-r--r--   0        0        0     1892 2023-11-06 06:59:52.887127 pinjected-0.2.35/pinjected/di/injected_analysis.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.35/pinjected/di/metadata/__init__.py
+-rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.35/pinjected/di/metadata/bind_metadata.py
+-rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.35/pinjected/di/metadata/location_data.py
+-rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.35/pinjected/di/modular_injected.py
+-rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.35/pinjected/di/monadic.py
+-rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.35/pinjected/di/overload_experimental.py
+-rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.35/pinjected/di/playground.py
+-rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.35/pinjected/di/provider.py
+-rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.35/pinjected/di/proxiable.py
+-rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.35/pinjected/di/session.py
+-rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.35/pinjected/di/sessioned.py
+-rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.35/pinjected/di/static_proxy.py
+-rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.35/pinjected/di/test_ast.py
+-rw-r--r--   0        0        0      997 2024-03-26 02:52:38.844108 pinjected-0.2.35/pinjected/di/test_dynamic_proxy.py
+-rw-r--r--   0        0        0     1500 2024-03-20 13:37:29.443496 pinjected-0.2.35/pinjected/di/test_graph.py
+-rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.35/pinjected/di/test_injected.py
+-rw-r--r--   0        0        0      452 2024-03-26 02:52:38.845073 pinjected-0.2.35/pinjected/di/test_proxiable.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.35/pinjected/di/tools/__init__.py
+-rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.35/pinjected/di/tools/add_overload.py
+-rw-r--r--   0        0        0    15106 2024-03-26 02:52:38.846281 pinjected-0.2.35/pinjected/di/util.py
+-rw-r--r--   0        0        0     1071 2023-08-25 06:23:59.157878 pinjected-0.2.35/pinjected/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.35/pinjected/exporter/__init__.py
+-rw-r--r--   0        0        0      409 2024-04-16 06:03:24.715733 pinjected-0.2.35/pinjected/exporter/llm_export_v2.py
+-rw-r--r--   0        0        0    31538 2024-04-16 12:25:07.860805 pinjected-0.2.35/pinjected/exporter/llm_exporter.py
+-rw-r--r--   0        0        0     2216 2024-04-16 09:23:13.383068 pinjected-0.2.35/pinjected/exporter/optimize_import_stmts.py
+-rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.35/pinjected/global_configs.py
+-rw-r--r--   0        0        0     2927 2024-03-26 02:52:38.847411 pinjected-0.2.35/pinjected/graph_inspection.py
+-rw-r--r--   0        0        0     3763 2024-04-16 12:18:24.324205 pinjected-0.2.35/pinjected/helper_structure.py
+-rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.35/pinjected/helpers.py
+-rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.35/pinjected/ide_supports/__init__.py
+-rw-r--r--   0        0        0     9050 2024-01-10 03:58:40.484651 pinjected-0.2.35/pinjected/ide_supports/console_run_helper.py
+-rw-r--r--   0        0        0     7287 2024-04-16 09:18:34.207695 pinjected-0.2.35/pinjected/ide_supports/create_configs.py
+-rw-r--r--   0        0        0     1304 2024-04-16 09:21:04.827442 pinjected-0.2.35/pinjected/ide_supports/default_design.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.35/pinjected/llm_support/__init__.py
+-rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.35/pinjected/llm_support/inspect_module.py
+-rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.35/pinjected/llm_support/inspect_module_prompts.py
+-rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.35/pinjected/logging_helper.py
+-rw-r--r--   0        0        0     4121 2024-04-08 10:32:08.774921 pinjected-0.2.35/pinjected/main_impl.py
+-rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.35/pinjected/maybe_patch.py
+-rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.35/pinjected/meta_main.py
+-rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.35/pinjected/module_helper.py
+-rw-r--r--   0        0        0     2453 2024-04-15 03:39:25.763167 pinjected-0.2.35/pinjected/module_inspector.py
+-rw-r--r--   0        0        0     4862 2024-04-16 09:26:56.419338 pinjected-0.2.35/pinjected/module_var_path.py
+-rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.35/pinjected/notification.py
+-rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.35/pinjected/nx_graph_util.py
+-rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.35/pinjected/providable.py
+-rw-r--r--   0        0        0    21320 2024-04-16 09:02:24.191362 pinjected-0.2.35/pinjected/run_config_utils.py
+-rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.35/pinjected/run_config_utils_v2.py
+-rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.35/pinjected/run_helpers/__init__.py
+-rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.35/pinjected/run_helpers/config.py
+-rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.35/pinjected/run_helpers/pinjected_environments.py
+-rw-r--r--   0        0        0     9360 2024-04-15 05:43:18.485943 pinjected-0.2.35/pinjected/run_helpers/run_injected.py
+-rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.35/pinjected/runnables.py
+-rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.35/pinjected/test_package/__init__.py
+-rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.35/pinjected/test_package/child/__init__.py
+-rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.35/pinjected/test_package/child/module1.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.35/pinjected/v2/__init__.py
+-rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.35/pinjected/v2/ainjected.py
+-rw-r--r--   0        0        0     6128 2024-03-26 02:52:38.850654 pinjected-0.2.35/pinjected/v2/binds.py
+-rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.35/pinjected/v2/di.py
+-rw-r--r--   0        0        0      358 2024-03-26 02:52:38.851474 pinjected-0.2.35/pinjected/v2/keys.py
+-rw-r--r--   0        0        0      478 2024-03-26 02:52:38.851836 pinjected-0.2.35/pinjected/v2/provide_context.py
+-rw-r--r--   0        0        0     5647 2024-03-29 04:40:41.000002 pinjected-0.2.35/pinjected/v2/resolver.py
+-rw-r--r--   0        0        0    19384 2024-03-26 02:52:38.852889 pinjected-0.2.35/pinjected/visualize_di.py
+-rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.35/pinjected/viz/__init__.py
+-rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.35/pinjected/viz/graph.py
+-rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.35/pinjected/with_context.py
+-rw-r--r--   0        0        0      759 2024-04-16 12:26:53.486024 pinjected-0.2.35/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 pinjected-0.2.35/PKG-INFO
```

### Comparing `pinjected-0.2.34/LICENSE` & `pinjected-0.2.35/LICENSE`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/decoration.py` & `pinjected-0.2.35/pinjected/decoration.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/demo.py` & `pinjected-0.2.35/pinjected/demo.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/di/app_designed.py` & `pinjected-0.2.35/pinjected/di/app_designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/di/app_injected.py` & `pinjected-0.2.35/pinjected/di/app_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/di/applicative.py` & `pinjected-0.2.35/pinjected/di/applicative.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/di/ast.py` & `pinjected-0.2.35/pinjected/di/ast.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/di/decorators.py` & `pinjected-0.2.35/pinjected/di/decorators.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/di/design.py` & `pinjected-0.2.35/pinjected/di/design.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/di/designed.py` & `pinjected-0.2.35/pinjected/di/designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/di/dynamic_proxy.py` & `pinjected-0.2.35/pinjected/di/dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/di/graph.py` & `pinjected-0.2.35/pinjected/di/graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/di/injected.py` & `pinjected-0.2.35/pinjected/di/injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/di/injected_analysis.py` & `pinjected-0.2.35/pinjected/di/injected_analysis.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/di/modular_injected.py` & `pinjected-0.2.35/pinjected/di/modular_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/di/overload_experimental.py` & `pinjected-0.2.35/pinjected/di/overload_experimental.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/di/proxiable.py` & `pinjected-0.2.35/pinjected/di/proxiable.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/di/session.py` & `pinjected-0.2.35/pinjected/di/session.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/di/sessioned.py` & `pinjected-0.2.35/pinjected/di/sessioned.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/di/static_proxy.py` & `pinjected-0.2.35/pinjected/di/static_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/di/test_dynamic_proxy.py` & `pinjected-0.2.35/pinjected/di/test_dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/di/test_graph.py` & `pinjected-0.2.35/pinjected/di/test_graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/di/test_injected.py` & `pinjected-0.2.35/pinjected/di/test_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/di/tools/add_overload.py` & `pinjected-0.2.35/pinjected/di/tools/add_overload.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/di/util.py` & `pinjected-0.2.35/pinjected/di/util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/exceptions.py` & `pinjected-0.2.35/pinjected/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/exporter/llm_exporter.py` & `pinjected-0.2.35/pinjected/exporter/llm_exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,15 +313,15 @@
         if visited is None:
             visited = set()
         blocks = []
         if isinstance(src, str):
             src = Injected.by_name(src)
         src = Injected.ensure_injected(src)
         from loguru import logger
-        logger.info(f"visiting {assign_target}")
+        # logger.info(f"visiting {assign_target}")
         for dep in src.complete_dependencies:
             if dep not in visited:
                 if dep not in self.mappings:
                     logger.error(f"{dep} not in mappings! for {src}")
                 visited |= {dep}
                 if dep not in self.mappings:
                     logger.warning(f"mappings:{self.mappings}")
@@ -330,15 +330,15 @@
                 for b in blks:
                     assert isinstance(b, CodeBlock), f"block is not CodeBlock:{b},{type(b)},src:{src}\n{pformat(blks)}"
                 blocks += blks
                 for b in blocks:
                     assert isinstance(b,
                                       CodeBlock), f"block is not CodeBlock:{b},{type(b)},src:{src}\n{pformat(blocks)}"
 
-        logger.info(f"getting source for {assign_target},type:{type(src)}")
+        # logger.info(f"getting source for {assign_target},type:{type(src)}")
         match src:
             case InjectedPure() as p:
                 blocks += [await self.to_source__instance(assign_target, p)]
             case InjectedFunction(tgt_func, {'injected_kwargs': DictInjected(kwargs_mapping)}) as f if hasattr(f,
                                                                                                                '__is_partial__'):
                 assign_blocks = await self.get_blocks_for_func_call(
                     assign_target,
@@ -346,15 +346,15 @@
                     kwargs_mapping,
                     visited=visited,
                     call=False
                 )
                 blocks += assign_blocks
             case InjectedFunction(func_called, {'injected_kwargs': DictInjected(kwargs_mapping)}) as _if:
                 # aha, we need to solve the keyword mappings and add it as code blocks
-                logger.warning(f"kwargs_mapping for injected_function:{kwargs_mapping}")
+                # logger.warning(f"kwargs_mapping for injected_function:{kwargs_mapping}")
                 assign_blocks = await self.get_blocks_for_func_call(
                     assign_target,
                     _if,
                     kwargs_mapping,
                     visited,
                     call=True
                 )
@@ -536,35 +536,37 @@
     async def export(self, target, package_to_export: str):
         blocks: list[CodeBlock] = await self.to_source(target, self.mappings[target])
         imports = cytoolz.merge([b.imports.imports for b in blocks])
         classdefs = cytoolz.merge([b.imports.classes for b in blocks])
         classdefs = {k: v for k, v in classdefs.items() if imports[k].startswith(package_to_export)}
         # remove classdefs from imports
         from loguru import logger
-        logger.info(f"classdefs:{pformat(classdefs)}")
+        # logger.info(f"classdefs:{pformat(classdefs)}")
         imports = {k: v for k, v in imports.items() if k not in classdefs}
 
         tmp_code = "\n".join([b.code for b in blocks])
 
         used_names = extract_variable_names(tmp_code)
         # add classes used
-        logger.info(f"used_names:{used_names}")
+        # logger.info(f"used_names:{used_names}")
         used_classdefs = {k: v for k, v in classdefs.items() if k in used_names}
         class_blocks = class_defs_to_blocks(used_classdefs)
         logger.info(f'class_blocks:\n{pformat(class_blocks)}')
-        blocks = class_blocks + blocks
         blocks += [
             CodeBlock(
                 target="",
                 code=f"return {blocks[-1].target}",
                 imports=Imports()
             )
         ]
 
         block_asts = [ast.parse(b.code) for b in blocks]
+
+        class_codes = "\n".join([b.code for b in class_blocks])
+
         code = wrap_in_async_main(block_asts)
 
         # recreate the code
         # code = "\n".join([b.code for b in blocks])
 
         import_lines = ""
         for name, full in imports.items():
@@ -572,15 +574,15 @@
             mod_paths = full.split('.')
             if len(mod_paths) <= 1:
                 import_lines += f"import {name}\n"
             else:
                 mod_name = ".".join(mod_paths[:-1])
                 import_lines += f"from {mod_name} import {name}\n"
 
-        src = import_lines + "\n" + code
+        src = import_lines + "\n" + class_codes + "\n" + code
         src = fix_imports(src)
         return src
 
 
 def wrap_in_async_main(nodes):
     # Create the 'async main' function
     async_main_func = ast.AsyncFunctionDef(
@@ -650,19 +652,19 @@
     return blocks
 
 
 @injected
 async def _export_injected(logger, a_llm, /, tgt: str):
     tgt = ModuleVarPath(tgt)
     from loguru import logger
-    mc: MetaContext = MetaContext.gather_from_path(tgt.module_file_path)
-    logger.info(f"loaded meta context for {tgt.module_file_path}")
-    logger.info(f"using meta context:{mc}")
+    mc: MetaContext = await MetaContext.a_gather_from_path(tgt.module_file_path)
+    # logger.info(f"loaded meta context for {tgt.module_file_path}")
+    # logger.info(f"using meta context:{mc}")
     fd = await mc.a_final_design
-    logger.info(f"meta context final design:{fd.bindings}")
+    # logger.info(f"meta context final design:{pformat(fd.bindings)}")
     # hmm, the design must contain the tgt.var_name, so we add it here
     fd += providers(**{tgt.var_name: tgt.load()})
     exporter = PinjectedCodeExporter(fd, a_llm)
     src = await exporter.export(tgt.var_name, tgt.module_name.split('.')[0])
     logger.info(f"script:\n{src}")
     original_path = Path(tgt.module_file_path)
     dst = original_path.parent / (original_path.stem + f"__{tgt.var_name}.py")
```

### Comparing `pinjected-0.2.34/pinjected/exporter/optimize_import_stmts.py` & `pinjected-0.2.35/pinjected/exporter/optimize_import_stmts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/graph_inspection.py` & `pinjected-0.2.35/pinjected/graph_inspection.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/helper_structure.py` & `pinjected-0.2.35/pinjected/helper_structure.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,14 +25,40 @@
 
 @dataclass
 class MetaContext:
     trace: List[ModuleVarSpec[Design]]
     accumulated: Design
 
     @staticmethod
+    async def a_gather_from_path(file_path: Path, meta_design_name: str = "__meta_design__"):
+        if not isinstance(file_path, Path):
+            file_path = Path(file_path)
+        designs = list(walk_module_attr(file_path, meta_design_name))
+        designs.reverse()
+        res = Design()
+        overrides = Design()
+        for item in designs:
+            logger.debug(f"{meta_design_name} at :{item.var_path}")
+            res = res + item.var
+            try:
+
+                overrides += await item.var.to_resolver()["overrides"]
+            except Exception as e:
+                logger.debug(f"{item.var_path} does not contain overrides")
+        from pinjected import instances
+        res += instances(
+            overrides=overrides
+        )
+
+        return MetaContext(
+            trace=designs,
+            accumulated=res
+        )
+
+    @staticmethod
     def gather_from_path(file_path: Path, meta_design_name: str = "__meta_design__"):
         if not isinstance(file_path, Path):
             file_path = Path(file_path)
         designs = list(walk_module_attr(file_path, meta_design_name))
         designs.reverse()
         res = Design()
         overrides = Design()
```

### Comparing `pinjected-0.2.34/pinjected/helpers.py` & `pinjected-0.2.35/pinjected/helpers.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/ide_supports/console_run_helper.py` & `pinjected-0.2.35/pinjected/ide_supports/console_run_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/ide_supports/create_configs.py` & `pinjected-0.2.35/pinjected/ide_supports/create_configs.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/ide_supports/default_design.py` & `pinjected-0.2.35/pinjected/ide_supports/default_design.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/llm_support/inspect_module.py` & `pinjected-0.2.35/pinjected/llm_support/inspect_module.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/llm_support/inspect_module_prompts.py` & `pinjected-0.2.35/pinjected/llm_support/inspect_module_prompts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/main_impl.py` & `pinjected-0.2.35/pinjected/main_impl.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/maybe_patch.py` & `pinjected-0.2.35/pinjected/maybe_patch.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/module_helper.py` & `pinjected-0.2.35/pinjected/module_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/module_inspector.py` & `pinjected-0.2.35/pinjected/module_inspector.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/module_var_path.py` & `pinjected-0.2.35/pinjected/module_var_path.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/notification.py` & `pinjected-0.2.35/pinjected/notification.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/nx_graph_util.py` & `pinjected-0.2.35/pinjected/nx_graph_util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/run_config_utils.py` & `pinjected-0.2.35/pinjected/run_config_utils.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/run_config_utils_v2.py` & `pinjected-0.2.35/pinjected/run_config_utils_v2.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/run_helpers/config.py` & `pinjected-0.2.35/pinjected/run_helpers/config.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/run_helpers/run_injected.py` & `pinjected-0.2.35/pinjected/run_helpers/run_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/runnables.py` & `pinjected-0.2.35/pinjected/runnables.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/test_package/__init__.py` & `pinjected-0.2.35/pinjected/test_package/__init__.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/test_package/child/module1.py` & `pinjected-0.2.35/pinjected/test_package/child/module1.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/v2/ainjected.py` & `pinjected-0.2.35/pinjected/v2/ainjected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/v2/binds.py` & `pinjected-0.2.35/pinjected/v2/binds.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/v2/di.py` & `pinjected-0.2.35/pinjected/v2/di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/v2/resolver.py` & `pinjected-0.2.35/pinjected/v2/resolver.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pinjected/visualize_di.py` & `pinjected-0.2.35/pinjected/visualize_di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.34/pyproject.toml` & `pinjected-0.2.35/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pinjected"
-version = "0.2.34"
+version = "0.2.35"
 description = "Immutable Dependency Injection for Python."
 authors = [ "proboscis <nameissoap@gmail.com>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 returns = "^0.21.0"
```

### Comparing `pinjected-0.2.34/PKG-INFO` & `pinjected-0.2.35/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinjected
-Version: 0.2.34
+Version: 0.2.35
 Summary: Immutable Dependency Injection for Python.
 License: MIT
 Author: proboscis
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

