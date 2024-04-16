# Comparing `tmp/pinjected-0.2.32.tar.gz` & `tmp/pinjected-0.2.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinjected-0.2.32.tar", max compression
+gzip compressed data, was "pinjected-0.2.33.tar", max compression
```

## Comparing `pinjected-0.2.32.tar` & `pinjected-0.2.33.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.32/LICENSE
--rw-r--r--   0        0        0      457 2024-01-10 03:58:40.481212 pinjected-0.2.32/pinjected/__init__.py
--rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.32/pinjected/__main__.py
--rw-r--r--   0        0        0      994 2024-04-16 04:30:55.994066 pinjected-0.2.32/pinjected/decoration.py
--rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.32/pinjected/demo.py
--rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.32/pinjected/di/__init__.py
--rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.32/pinjected/di/app_designed.py
--rw-r--r--   0        0        0     5664 2024-04-02 03:27:58.890219 pinjected-0.2.32/pinjected/di/app_injected.py
--rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.32/pinjected/di/applicative.py
--rw-r--r--   0        0        0     7340 2024-03-26 02:52:38.836702 pinjected-0.2.32/pinjected/di/ast.py
--rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.32/pinjected/di/async_injected.py
--rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.32/pinjected/di/bindings.py
--rw-r--r--   0        0        0     9753 2024-03-26 02:52:38.838842 pinjected-0.2.32/pinjected/di/decorators.py
--rw-r--r--   0        0        0    13317 2024-03-26 02:52:38.839976 pinjected-0.2.32/pinjected/di/design.py
--rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.32/pinjected/di/design_bind_contextx.py
--rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.32/pinjected/di/designed.py
--rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.32/pinjected/di/dynamic_proxy.py
--rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.32/pinjected/di/graph.py
--rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.32/pinjected/di/implicit_globals.py
--rw-r--r--   0        0        0    54209 2024-04-16 06:03:24.715277 pinjected-0.2.32/pinjected/di/injected.py
--rw-r--r--   0        0        0     1892 2023-11-06 06:59:52.887127 pinjected-0.2.32/pinjected/di/injected_analysis.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.32/pinjected/di/metadata/__init__.py
--rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.32/pinjected/di/metadata/bind_metadata.py
--rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.32/pinjected/di/metadata/location_data.py
--rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.32/pinjected/di/modular_injected.py
--rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.32/pinjected/di/monadic.py
--rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.32/pinjected/di/overload_experimental.py
--rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.32/pinjected/di/playground.py
--rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.32/pinjected/di/provider.py
--rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.32/pinjected/di/proxiable.py
--rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.32/pinjected/di/session.py
--rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.32/pinjected/di/sessioned.py
--rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.32/pinjected/di/static_proxy.py
--rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.32/pinjected/di/test_ast.py
--rw-r--r--   0        0        0      997 2024-03-26 02:52:38.844108 pinjected-0.2.32/pinjected/di/test_dynamic_proxy.py
--rw-r--r--   0        0        0     1500 2024-03-20 13:37:29.443496 pinjected-0.2.32/pinjected/di/test_graph.py
--rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.32/pinjected/di/test_injected.py
--rw-r--r--   0        0        0      452 2024-03-26 02:52:38.845073 pinjected-0.2.32/pinjected/di/test_proxiable.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.32/pinjected/di/tools/__init__.py
--rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.32/pinjected/di/tools/add_overload.py
--rw-r--r--   0        0        0    15106 2024-03-26 02:52:38.846281 pinjected-0.2.32/pinjected/di/util.py
--rw-r--r--   0        0        0     1071 2023-08-25 06:23:59.157878 pinjected-0.2.32/pinjected/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.32/pinjected/exporter/__init__.py
--rw-r--r--   0        0        0      409 2024-04-16 06:03:24.715733 pinjected-0.2.32/pinjected/exporter/llm_export_v2.py
--rw-r--r--   0        0        0    30474 2024-04-16 09:19:20.392540 pinjected-0.2.32/pinjected/exporter/llm_exporter.py
--rw-r--r--   0        0        0     2216 2024-04-16 09:23:13.383068 pinjected-0.2.32/pinjected/exporter/optimize_import_stmts.py
--rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.32/pinjected/global_configs.py
--rw-r--r--   0        0        0     2927 2024-03-26 02:52:38.847411 pinjected-0.2.32/pinjected/graph_inspection.py
--rw-r--r--   0        0        0     2886 2024-04-15 04:38:55.875181 pinjected-0.2.32/pinjected/helper_structure.py
--rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.32/pinjected/helpers.py
--rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.32/pinjected/ide_supports/__init__.py
--rw-r--r--   0        0        0     9050 2024-01-10 03:58:40.484651 pinjected-0.2.32/pinjected/ide_supports/console_run_helper.py
--rw-r--r--   0        0        0     7287 2024-04-16 09:18:34.207695 pinjected-0.2.32/pinjected/ide_supports/create_configs.py
--rw-r--r--   0        0        0     1304 2024-04-16 09:21:04.827442 pinjected-0.2.32/pinjected/ide_supports/default_design.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.32/pinjected/llm_support/__init__.py
--rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.32/pinjected/llm_support/inspect_module.py
--rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.32/pinjected/llm_support/inspect_module_prompts.py
--rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.32/pinjected/logging_helper.py
--rw-r--r--   0        0        0     4121 2024-04-08 10:32:08.774921 pinjected-0.2.32/pinjected/main_impl.py
--rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.32/pinjected/maybe_patch.py
--rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.32/pinjected/meta_main.py
--rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.32/pinjected/module_helper.py
--rw-r--r--   0        0        0     2453 2024-04-15 03:39:25.763167 pinjected-0.2.32/pinjected/module_inspector.py
--rw-r--r--   0        0        0     4862 2024-04-16 09:26:56.419338 pinjected-0.2.32/pinjected/module_var_path.py
--rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.32/pinjected/notification.py
--rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.32/pinjected/nx_graph_util.py
--rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.32/pinjected/providable.py
--rw-r--r--   0        0        0    21320 2024-04-16 09:02:24.191362 pinjected-0.2.32/pinjected/run_config_utils.py
--rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.32/pinjected/run_config_utils_v2.py
--rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.32/pinjected/run_helpers/__init__.py
--rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.32/pinjected/run_helpers/config.py
--rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.32/pinjected/run_helpers/pinjected_environments.py
--rw-r--r--   0        0        0     9360 2024-04-15 05:43:18.485943 pinjected-0.2.32/pinjected/run_helpers/run_injected.py
--rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.32/pinjected/runnables.py
--rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.32/pinjected/test_package/__init__.py
--rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.32/pinjected/test_package/child/__init__.py
--rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.32/pinjected/test_package/child/module1.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.32/pinjected/v2/__init__.py
--rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.32/pinjected/v2/ainjected.py
--rw-r--r--   0        0        0     6128 2024-03-26 02:52:38.850654 pinjected-0.2.32/pinjected/v2/binds.py
--rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.32/pinjected/v2/di.py
--rw-r--r--   0        0        0      358 2024-03-26 02:52:38.851474 pinjected-0.2.32/pinjected/v2/keys.py
--rw-r--r--   0        0        0      478 2024-03-26 02:52:38.851836 pinjected-0.2.32/pinjected/v2/provide_context.py
--rw-r--r--   0        0        0     5647 2024-03-29 04:40:41.000002 pinjected-0.2.32/pinjected/v2/resolver.py
--rw-r--r--   0        0        0    19384 2024-03-26 02:52:38.852889 pinjected-0.2.32/pinjected/visualize_di.py
--rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.32/pinjected/viz/__init__.py
--rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.32/pinjected/viz/graph.py
--rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.32/pinjected/with_context.py
--rw-r--r--   0        0        0      759 2024-04-16 09:26:57.440750 pinjected-0.2.32/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 pinjected-0.2.32/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.33/LICENSE
+-rw-r--r--   0        0        0      457 2024-01-10 03:58:40.481212 pinjected-0.2.33/pinjected/__init__.py
+-rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.33/pinjected/__main__.py
+-rw-r--r--   0        0        0      994 2024-04-16 04:30:55.994066 pinjected-0.2.33/pinjected/decoration.py
+-rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.33/pinjected/demo.py
+-rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.33/pinjected/di/__init__.py
+-rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.33/pinjected/di/app_designed.py
+-rw-r--r--   0        0        0     5664 2024-04-02 03:27:58.890219 pinjected-0.2.33/pinjected/di/app_injected.py
+-rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.33/pinjected/di/applicative.py
+-rw-r--r--   0        0        0     7340 2024-03-26 02:52:38.836702 pinjected-0.2.33/pinjected/di/ast.py
+-rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.33/pinjected/di/async_injected.py
+-rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.33/pinjected/di/bindings.py
+-rw-r--r--   0        0        0     9753 2024-03-26 02:52:38.838842 pinjected-0.2.33/pinjected/di/decorators.py
+-rw-r--r--   0        0        0    13317 2024-03-26 02:52:38.839976 pinjected-0.2.33/pinjected/di/design.py
+-rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.33/pinjected/di/design_bind_contextx.py
+-rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.33/pinjected/di/designed.py
+-rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.33/pinjected/di/dynamic_proxy.py
+-rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.33/pinjected/di/graph.py
+-rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.33/pinjected/di/implicit_globals.py
+-rw-r--r--   0        0        0    54209 2024-04-16 06:03:24.715277 pinjected-0.2.33/pinjected/di/injected.py
+-rw-r--r--   0        0        0     1892 2023-11-06 06:59:52.887127 pinjected-0.2.33/pinjected/di/injected_analysis.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.33/pinjected/di/metadata/__init__.py
+-rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.33/pinjected/di/metadata/bind_metadata.py
+-rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.33/pinjected/di/metadata/location_data.py
+-rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.33/pinjected/di/modular_injected.py
+-rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.33/pinjected/di/monadic.py
+-rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.33/pinjected/di/overload_experimental.py
+-rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.33/pinjected/di/playground.py
+-rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.33/pinjected/di/provider.py
+-rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.33/pinjected/di/proxiable.py
+-rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.33/pinjected/di/session.py
+-rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.33/pinjected/di/sessioned.py
+-rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.33/pinjected/di/static_proxy.py
+-rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.33/pinjected/di/test_ast.py
+-rw-r--r--   0        0        0      997 2024-03-26 02:52:38.844108 pinjected-0.2.33/pinjected/di/test_dynamic_proxy.py
+-rw-r--r--   0        0        0     1500 2024-03-20 13:37:29.443496 pinjected-0.2.33/pinjected/di/test_graph.py
+-rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.33/pinjected/di/test_injected.py
+-rw-r--r--   0        0        0      452 2024-03-26 02:52:38.845073 pinjected-0.2.33/pinjected/di/test_proxiable.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.33/pinjected/di/tools/__init__.py
+-rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.33/pinjected/di/tools/add_overload.py
+-rw-r--r--   0        0        0    15106 2024-03-26 02:52:38.846281 pinjected-0.2.33/pinjected/di/util.py
+-rw-r--r--   0        0        0     1071 2023-08-25 06:23:59.157878 pinjected-0.2.33/pinjected/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.33/pinjected/exporter/__init__.py
+-rw-r--r--   0        0        0      409 2024-04-16 06:03:24.715733 pinjected-0.2.33/pinjected/exporter/llm_export_v2.py
+-rw-r--r--   0        0        0    31397 2024-04-16 10:24:12.376157 pinjected-0.2.33/pinjected/exporter/llm_exporter.py
+-rw-r--r--   0        0        0     2216 2024-04-16 09:23:13.383068 pinjected-0.2.33/pinjected/exporter/optimize_import_stmts.py
+-rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.33/pinjected/global_configs.py
+-rw-r--r--   0        0        0     2927 2024-03-26 02:52:38.847411 pinjected-0.2.33/pinjected/graph_inspection.py
+-rw-r--r--   0        0        0     2886 2024-04-15 04:38:55.875181 pinjected-0.2.33/pinjected/helper_structure.py
+-rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.33/pinjected/helpers.py
+-rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.33/pinjected/ide_supports/__init__.py
+-rw-r--r--   0        0        0     9050 2024-01-10 03:58:40.484651 pinjected-0.2.33/pinjected/ide_supports/console_run_helper.py
+-rw-r--r--   0        0        0     7287 2024-04-16 09:18:34.207695 pinjected-0.2.33/pinjected/ide_supports/create_configs.py
+-rw-r--r--   0        0        0     1304 2024-04-16 09:21:04.827442 pinjected-0.2.33/pinjected/ide_supports/default_design.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.33/pinjected/llm_support/__init__.py
+-rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.33/pinjected/llm_support/inspect_module.py
+-rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.33/pinjected/llm_support/inspect_module_prompts.py
+-rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.33/pinjected/logging_helper.py
+-rw-r--r--   0        0        0     4121 2024-04-08 10:32:08.774921 pinjected-0.2.33/pinjected/main_impl.py
+-rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.33/pinjected/maybe_patch.py
+-rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.33/pinjected/meta_main.py
+-rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.33/pinjected/module_helper.py
+-rw-r--r--   0        0        0     2453 2024-04-15 03:39:25.763167 pinjected-0.2.33/pinjected/module_inspector.py
+-rw-r--r--   0        0        0     4862 2024-04-16 09:26:56.419338 pinjected-0.2.33/pinjected/module_var_path.py
+-rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.33/pinjected/notification.py
+-rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.33/pinjected/nx_graph_util.py
+-rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.33/pinjected/providable.py
+-rw-r--r--   0        0        0    21320 2024-04-16 09:02:24.191362 pinjected-0.2.33/pinjected/run_config_utils.py
+-rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.33/pinjected/run_config_utils_v2.py
+-rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.33/pinjected/run_helpers/__init__.py
+-rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.33/pinjected/run_helpers/config.py
+-rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.33/pinjected/run_helpers/pinjected_environments.py
+-rw-r--r--   0        0        0     9360 2024-04-15 05:43:18.485943 pinjected-0.2.33/pinjected/run_helpers/run_injected.py
+-rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.33/pinjected/runnables.py
+-rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.33/pinjected/test_package/__init__.py
+-rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.33/pinjected/test_package/child/__init__.py
+-rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.33/pinjected/test_package/child/module1.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.33/pinjected/v2/__init__.py
+-rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.33/pinjected/v2/ainjected.py
+-rw-r--r--   0        0        0     6128 2024-03-26 02:52:38.850654 pinjected-0.2.33/pinjected/v2/binds.py
+-rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.33/pinjected/v2/di.py
+-rw-r--r--   0        0        0      358 2024-03-26 02:52:38.851474 pinjected-0.2.33/pinjected/v2/keys.py
+-rw-r--r--   0        0        0      478 2024-03-26 02:52:38.851836 pinjected-0.2.33/pinjected/v2/provide_context.py
+-rw-r--r--   0        0        0     5647 2024-03-29 04:40:41.000002 pinjected-0.2.33/pinjected/v2/resolver.py
+-rw-r--r--   0        0        0    19384 2024-03-26 02:52:38.852889 pinjected-0.2.33/pinjected/visualize_di.py
+-rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.33/pinjected/viz/__init__.py
+-rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.33/pinjected/viz/graph.py
+-rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.33/pinjected/with_context.py
+-rw-r--r--   0        0        0      759 2024-04-16 10:24:14.877900 pinjected-0.2.33/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 pinjected-0.2.33/PKG-INFO
```

### Comparing `pinjected-0.2.32/LICENSE` & `pinjected-0.2.33/LICENSE`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/decoration.py` & `pinjected-0.2.33/pinjected/decoration.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/demo.py` & `pinjected-0.2.33/pinjected/demo.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/di/app_designed.py` & `pinjected-0.2.33/pinjected/di/app_designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/di/app_injected.py` & `pinjected-0.2.33/pinjected/di/app_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/di/applicative.py` & `pinjected-0.2.33/pinjected/di/applicative.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/di/ast.py` & `pinjected-0.2.33/pinjected/di/ast.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/di/decorators.py` & `pinjected-0.2.33/pinjected/di/decorators.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/di/design.py` & `pinjected-0.2.33/pinjected/di/design.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/di/designed.py` & `pinjected-0.2.33/pinjected/di/designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/di/dynamic_proxy.py` & `pinjected-0.2.33/pinjected/di/dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/di/graph.py` & `pinjected-0.2.33/pinjected/di/graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/di/injected.py` & `pinjected-0.2.33/pinjected/di/injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/di/injected_analysis.py` & `pinjected-0.2.33/pinjected/di/injected_analysis.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/di/modular_injected.py` & `pinjected-0.2.33/pinjected/di/modular_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/di/overload_experimental.py` & `pinjected-0.2.33/pinjected/di/overload_experimental.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/di/proxiable.py` & `pinjected-0.2.33/pinjected/di/proxiable.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/di/session.py` & `pinjected-0.2.33/pinjected/di/session.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/di/sessioned.py` & `pinjected-0.2.33/pinjected/di/sessioned.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/di/static_proxy.py` & `pinjected-0.2.33/pinjected/di/static_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/di/test_dynamic_proxy.py` & `pinjected-0.2.33/pinjected/di/test_dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/di/test_graph.py` & `pinjected-0.2.33/pinjected/di/test_graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/di/test_injected.py` & `pinjected-0.2.33/pinjected/di/test_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/di/tools/add_overload.py` & `pinjected-0.2.33/pinjected/di/tools/add_overload.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/di/util.py` & `pinjected-0.2.33/pinjected/di/util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/exceptions.py` & `pinjected-0.2.33/pinjected/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/exporter/llm_exporter.py` & `pinjected-0.2.33/pinjected/exporter/llm_exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,26 +86,38 @@
             # the variable is defined at non-module script so let's read the file
             source = Path(frm.f_globals['__file__']).read_text()
             imports = get_required_imports(source, module_name="__main__")
         else:
             module = sys.modules[mod_name]
             imports = get_required_imports(module)
 
-        if callable(tgt.value):
-            src = inspect.getsource(tgt.value)
-            logger.info(f"trying to en_source a callable:{src}")
-            src = await self.extract_lambda(tgt.value)
-        else:
-            src = tgt.value
+        match tgt.value:
+            case str():
+                code = f'{assign_target} = """{tgt.value}"""'
+            case int() | float():
+                code = f'{assign_target} = {tgt.value}'
+            case list() | dict():
+                code = f'{assign_target} = {tgt.value}'
+            case f if callable(f):
+                src = inspect.getsource(tgt.value)
+                logger.info(f"trying to en_source a callable:{src}")
+                src = await self.extract_lambda(tgt.value)
+                code = f'{assign_target} = {src}'
+            case Path():
+                code = f"{assign_target} = Path('{tgt.value}')"
+            case None:
+                code = f"{assign_target} = None"
+            case _:
+                raise ValueError(f"Unsupported type {tgt.value}")
 
         # assert isinstance(tgt.value, (str, int, float,list,dict,NoneType)), f"tgt.value must be a simple value, got {tgt.value}"
 
         return CodeBlock(
             target=assign_target,
-            code=f"{assign_target} = {src}",
+            code=code,
             imports=imports
         )
 
     async def extract_lambda(self, f):
         from loguru import logger
         logger.info(f"extracting lambda from {f.__name__}")
         src = inspect.getsource(f)
@@ -118,14 +130,16 @@
     lambda ...: ...
     """
         logger.info(f"prompt:\n{prompt}")
         return await self.a_llm(prompt)
 
     async def get_source_func(self, assign_target, f):
         from loguru import logger
+        if f.__module__ == 'builtins':
+            return f"{assign_target} = {f.__name__}"
         if hasattr(f, "__original_code__"):
             # logger.info(f"retrieving source from __original_code__")
             src = f.__original_code__
             # logger.debug(f"original source from __original_code__:\n{src}")
             modified = add_async_to_function_source(src)
             if modified is not None:
                 src = modified
@@ -212,16 +226,18 @@
             match e:
                 case BiOp(sym, left, right):
                     return f"{await to_src(left)} {sym} {await to_src(right)}"
                 case Call(f, args, kwargs):
                     args_str = ""
                     if args:
                         args_str = ','.join([await to_src(a) for a in args])
+                    if args and kwargs:
+                        args_str += ','
                     if kwargs:
-                        args_str += ',' + ','.join([f'{k}={await to_src(v)}' for k, v in kwargs.items()])
+                        args_str += ','.join([f'{k}={await to_src(v)}' for k, v in kwargs.items()])
                     return f"{await to_src(f)}({args_str})"
                 case Attr(src, attr):
                     return f"{await to_src(src)}.{attr}"
                 case GetItem(src, key):
                     return f"{await to_src(src)}[{await to_src(key)}]"
                 case UnaryOp("await", tgt):
                     return f"(await {await to_src(tgt)})"
@@ -246,15 +262,15 @@
                         predef_blocks += await self.to_source(sym, data, visited)
                     return sym
                 case Object(str() as literal):
                     return f'"{literal}"'
                 case Object(float() | int() as num):
                     return str(num)
                 case Object(Path() as p):
-                    return f"Path({p})"
+                    return f"Path('{p}')"
                 case Object(unknown):
                     raise ValueError(f"Unsupported object:{unknown},{type(unknown)}")
                 case _:
                     raise ValueError(f"Unsupported type {e}, {type(e)}")
 
         src = await to_src(expr)
 
@@ -483,15 +499,15 @@
         org_func = f.original_function
         module = inspect.getmodule(org_func)
         # assert module is not None,f"module is None for {org_func},\n{inspect.getsource(org_func)}"
         if module is not None:
             imports = get_required_imports(module)
         else:
             imports = Imports()
-        func_name = f"provide_if__{assign_target}"
+        func_name = f"__{assign_target}"
         last_code = await self.get_source_func(func_name, f.target_function)
         # you need to actually call the func.
         pairs = [f"{k}={v}" for k, v in key_to_symbol.items()]
         if call:
             last_code += f"\n{assign_target} = {func_name}({','.join(pairs)})\n"
         else:
             last_code += f"\n{assign_target} = {func_name}"
@@ -544,15 +560,15 @@
             )
         ]
 
         block_asts = [ast.parse(b.code) for b in blocks]
         code = wrap_in_async_main(block_asts)
 
         # recreate the code
-        #code = "\n".join([b.code for b in blocks])
+        # code = "\n".join([b.code for b in blocks])
 
         import_lines = ""
         for name, full in imports.items():
             # logger.info(f"importing {name} from {full}")
             mod_paths = full.split('.')
             if len(mod_paths) <= 1:
                 import_lines += f"import {name}\n"
@@ -560,14 +576,15 @@
                 mod_name = ".".join(mod_paths[:-1])
                 import_lines += f"from {mod_name} import {name}\n"
 
         src = import_lines + "\n" + code
         src = fix_imports(src)
         return src
 
+
 def wrap_in_async_main(nodes):
     # Create the 'async main' function
     async_main_func = ast.AsyncFunctionDef(
         name='main',
         args=ast.arguments(
             args=[],
             vararg=None,
@@ -632,20 +649,23 @@
         ))
     return blocks
 
 
 @injected
 async def _export_injected(logger, a_llm, /, tgt: str):
     tgt = ModuleVarPath(tgt)
+    from loguru import logger
     mc: MetaContext = MetaContext.gather_from_path(tgt.module_file_path)
+    logger.info(f"loaded meta context for {tgt.module_file_path}")
+    logger.info(f"using meta context:{mc}")
     fd = await mc.a_final_design
     # hmm, the design must contain the tgt.var_name, so we add it here
     fd += providers(**{tgt.var_name: tgt.load()})
     exporter = PinjectedCodeExporter(fd, a_llm)
-    src = await exporter.export(tgt.var_name,tgt.module_name.split('.')[0])
+    src = await exporter.export(tgt.var_name, tgt.module_name.split('.')[0])
     logger.info(f"script:\n{src}")
     original_path = Path(tgt.module_file_path)
     dst = original_path.parent / (original_path.stem + f"__{tgt.var_name}.py")
     dst.write_text(src)
 
 
 export_injected: Injected = _export_injected(injected("export_target"))
@@ -728,14 +748,16 @@
 
 def get_required_imports(module_or_source, module_name=None) -> Imports:
     if isinstance(module_or_source, str):
         source = module_or_source
         if module_name is None:
             module_name = "."
     else:
+        if module_or_source.__name__ == 'builtins':
+            return Imports()
         source = ast.unparse(ast.parse(ast.unparse(ast.parse(inspect.getsource(module_or_source)))))
         module_name = module_or_source.__name__
 
     tree = ast.parse(source)
     module_info = {}
     classes = {}
     for node in ast.walk(tree):
@@ -778,9 +800,9 @@
 
 __meta_design__ = instances(
     default_design_paths=["pinjected.exporter.llm_exporter.default_design"],
     overrides=instances(
 
     ),
 ) + providers(
-    #custom_idea_config_creator=add_export_config,
+    # custom_idea_config_creator=add_export_config,
 )
```

### Comparing `pinjected-0.2.32/pinjected/exporter/optimize_import_stmts.py` & `pinjected-0.2.33/pinjected/exporter/optimize_import_stmts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/graph_inspection.py` & `pinjected-0.2.33/pinjected/graph_inspection.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/helper_structure.py` & `pinjected-0.2.33/pinjected/helper_structure.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/helpers.py` & `pinjected-0.2.33/pinjected/helpers.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/ide_supports/console_run_helper.py` & `pinjected-0.2.33/pinjected/ide_supports/console_run_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/ide_supports/create_configs.py` & `pinjected-0.2.33/pinjected/ide_supports/create_configs.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/ide_supports/default_design.py` & `pinjected-0.2.33/pinjected/ide_supports/default_design.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/llm_support/inspect_module.py` & `pinjected-0.2.33/pinjected/llm_support/inspect_module.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/llm_support/inspect_module_prompts.py` & `pinjected-0.2.33/pinjected/llm_support/inspect_module_prompts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/main_impl.py` & `pinjected-0.2.33/pinjected/main_impl.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/maybe_patch.py` & `pinjected-0.2.33/pinjected/maybe_patch.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/module_helper.py` & `pinjected-0.2.33/pinjected/module_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/module_inspector.py` & `pinjected-0.2.33/pinjected/module_inspector.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/module_var_path.py` & `pinjected-0.2.33/pinjected/module_var_path.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/notification.py` & `pinjected-0.2.33/pinjected/notification.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/nx_graph_util.py` & `pinjected-0.2.33/pinjected/nx_graph_util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/run_config_utils.py` & `pinjected-0.2.33/pinjected/run_config_utils.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/run_config_utils_v2.py` & `pinjected-0.2.33/pinjected/run_config_utils_v2.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/run_helpers/config.py` & `pinjected-0.2.33/pinjected/run_helpers/config.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/run_helpers/run_injected.py` & `pinjected-0.2.33/pinjected/run_helpers/run_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/runnables.py` & `pinjected-0.2.33/pinjected/runnables.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/test_package/__init__.py` & `pinjected-0.2.33/pinjected/test_package/__init__.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/test_package/child/module1.py` & `pinjected-0.2.33/pinjected/test_package/child/module1.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/v2/ainjected.py` & `pinjected-0.2.33/pinjected/v2/ainjected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/v2/binds.py` & `pinjected-0.2.33/pinjected/v2/binds.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/v2/di.py` & `pinjected-0.2.33/pinjected/v2/di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/v2/resolver.py` & `pinjected-0.2.33/pinjected/v2/resolver.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pinjected/visualize_di.py` & `pinjected-0.2.33/pinjected/visualize_di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.32/pyproject.toml` & `pinjected-0.2.33/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pinjected"
-version = "0.2.32"
+version = "0.2.33"
 description = "Immutable Dependency Injection for Python."
 authors = [ "proboscis <nameissoap@gmail.com>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 returns = "^0.21.0"
```

### Comparing `pinjected-0.2.32/PKG-INFO` & `pinjected-0.2.33/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinjected
-Version: 0.2.32
+Version: 0.2.33
 Summary: Immutable Dependency Injection for Python.
 License: MIT
 Author: proboscis
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

