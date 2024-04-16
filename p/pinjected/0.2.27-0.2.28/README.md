# Comparing `tmp/pinjected-0.2.27.tar.gz` & `tmp/pinjected-0.2.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinjected-0.2.27.tar", max compression
+gzip compressed data, was "pinjected-0.2.28.tar", max compression
```

## Comparing `pinjected-0.2.27.tar` & `pinjected-0.2.28.tar`

### file list

```diff
@@ -1,87 +1,89 @@
--rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.27/LICENSE
--rw-r--r--   0        0        0      457 2024-01-10 03:58:40.481212 pinjected-0.2.27/pinjected/__init__.py
--rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.27/pinjected/__main__.py
--rw-r--r--   0        0        0      994 2024-03-26 02:52:38.834501 pinjected-0.2.27/pinjected/decoration.py
--rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.27/pinjected/demo.py
--rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.27/pinjected/di/__init__.py
--rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.27/pinjected/di/app_designed.py
--rw-r--r--   0        0        0     5664 2024-04-02 03:27:58.890219 pinjected-0.2.27/pinjected/di/app_injected.py
--rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.27/pinjected/di/applicative.py
--rw-r--r--   0        0        0     7340 2024-03-26 02:52:38.836702 pinjected-0.2.27/pinjected/di/ast.py
--rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.27/pinjected/di/async_injected.py
--rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.27/pinjected/di/bindings.py
--rw-r--r--   0        0        0     9753 2024-03-26 02:52:38.838842 pinjected-0.2.27/pinjected/di/decorators.py
--rw-r--r--   0        0        0    13317 2024-03-26 02:52:38.839976 pinjected-0.2.27/pinjected/di/design.py
--rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.27/pinjected/di/design_bind_contextx.py
--rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.27/pinjected/di/designed.py
--rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.27/pinjected/di/dynamic_proxy.py
--rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.27/pinjected/di/graph.py
--rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.27/pinjected/di/implicit_globals.py
--rw-r--r--   0        0        0    52174 2024-03-26 02:52:38.842342 pinjected-0.2.27/pinjected/di/injected.py
--rw-r--r--   0        0        0     1892 2023-11-06 06:59:52.887127 pinjected-0.2.27/pinjected/di/injected_analysis.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.27/pinjected/di/metadata/__init__.py
--rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.27/pinjected/di/metadata/bind_metadata.py
--rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.27/pinjected/di/metadata/location_data.py
--rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.27/pinjected/di/modular_injected.py
--rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.27/pinjected/di/monadic.py
--rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.27/pinjected/di/overload_experimental.py
--rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.27/pinjected/di/playground.py
--rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.27/pinjected/di/provider.py
--rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.27/pinjected/di/proxiable.py
--rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.27/pinjected/di/session.py
--rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.27/pinjected/di/sessioned.py
--rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.27/pinjected/di/static_proxy.py
--rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.27/pinjected/di/test_ast.py
--rw-r--r--   0        0        0      997 2024-03-26 02:52:38.844108 pinjected-0.2.27/pinjected/di/test_dynamic_proxy.py
--rw-r--r--   0        0        0     1500 2024-03-20 13:37:29.443496 pinjected-0.2.27/pinjected/di/test_graph.py
--rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.27/pinjected/di/test_injected.py
--rw-r--r--   0        0        0      452 2024-03-26 02:52:38.845073 pinjected-0.2.27/pinjected/di/test_proxiable.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.27/pinjected/di/tools/__init__.py
--rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.27/pinjected/di/tools/add_overload.py
--rw-r--r--   0        0        0    15106 2024-03-26 02:52:38.846281 pinjected-0.2.27/pinjected/di/util.py
--rw-r--r--   0        0        0     1071 2023-08-25 06:23:59.157878 pinjected-0.2.27/pinjected/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.27/pinjected/exporter/__init__.py
--rw-r--r--   0        0        0    10630 2024-03-26 02:52:38.846870 pinjected-0.2.27/pinjected/exporter/llm_exporter.py
--rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.27/pinjected/global_configs.py
--rw-r--r--   0        0        0     2927 2024-03-26 02:52:38.847411 pinjected-0.2.27/pinjected/graph_inspection.py
--rw-r--r--   0        0        0     2440 2024-01-10 03:58:40.484318 pinjected-0.2.27/pinjected/helper_structure.py
--rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.27/pinjected/helpers.py
--rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.27/pinjected/ide_supports/__init__.py
--rw-r--r--   0        0        0     9050 2024-01-10 03:58:40.484651 pinjected-0.2.27/pinjected/ide_supports/console_run_helper.py
--rw-r--r--   0        0        0     8329 2024-03-26 02:52:38.848041 pinjected-0.2.27/pinjected/ide_supports/create_configs.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.27/pinjected/llm_support/__init__.py
--rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.27/pinjected/llm_support/inspect_module.py
--rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.27/pinjected/llm_support/inspect_module_prompts.py
--rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.27/pinjected/logging_helper.py
--rw-r--r--   0        0        0     4121 2024-04-08 10:32:08.774921 pinjected-0.2.27/pinjected/main_impl.py
--rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.27/pinjected/maybe_patch.py
--rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.27/pinjected/meta_main.py
--rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.27/pinjected/module_helper.py
--rw-r--r--   0        0        0     2285 2023-07-11 12:13:24.404168 pinjected-0.2.27/pinjected/module_inspector.py
--rw-r--r--   0        0        0     4701 2024-03-26 02:52:38.848756 pinjected-0.2.27/pinjected/module_var_path.py
--rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.27/pinjected/notification.py
--rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.27/pinjected/nx_graph_util.py
--rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.27/pinjected/providable.py
--rw-r--r--   0        0        0    20629 2024-01-29 15:55:46.347150 pinjected-0.2.27/pinjected/run_config_utils.py
--rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.27/pinjected/run_config_utils_v2.py
--rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.27/pinjected/run_helpers/__init__.py
--rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.27/pinjected/run_helpers/config.py
--rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.27/pinjected/run_helpers/pinjected_environments.py
--rw-r--r--   0        0        0     9360 2024-03-26 02:52:38.849412 pinjected-0.2.27/pinjected/run_helpers/run_injected.py
--rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.27/pinjected/runnables.py
--rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.27/pinjected/test_package/__init__.py
--rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.27/pinjected/test_package/child/__init__.py
--rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.27/pinjected/test_package/child/module1.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.27/pinjected/v2/__init__.py
--rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.27/pinjected/v2/ainjected.py
--rw-r--r--   0        0        0     6128 2024-03-26 02:52:38.850654 pinjected-0.2.27/pinjected/v2/binds.py
--rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.27/pinjected/v2/di.py
--rw-r--r--   0        0        0      358 2024-03-26 02:52:38.851474 pinjected-0.2.27/pinjected/v2/keys.py
--rw-r--r--   0        0        0      478 2024-03-26 02:52:38.851836 pinjected-0.2.27/pinjected/v2/provide_context.py
--rw-r--r--   0        0        0     5647 2024-03-29 04:40:41.000002 pinjected-0.2.27/pinjected/v2/resolver.py
--rw-r--r--   0        0        0    19384 2024-03-26 02:52:38.852889 pinjected-0.2.27/pinjected/visualize_di.py
--rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.27/pinjected/viz/__init__.py
--rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.27/pinjected/viz/graph.py
--rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.27/pinjected/with_context.py
--rw-r--r--   0        0        0      733 2024-04-08 10:34:08.946880 pinjected-0.2.27/pyproject.toml
--rw-r--r--   0        0        0     1027 1970-01-01 00:00:00.000000 pinjected-0.2.27/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.28/LICENSE
+-rw-r--r--   0        0        0      457 2024-01-10 03:58:40.481212 pinjected-0.2.28/pinjected/__init__.py
+-rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.28/pinjected/__main__.py
+-rw-r--r--   0        0        0      994 2024-04-16 04:30:55.994066 pinjected-0.2.28/pinjected/decoration.py
+-rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.28/pinjected/demo.py
+-rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.28/pinjected/di/__init__.py
+-rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.28/pinjected/di/app_designed.py
+-rw-r--r--   0        0        0     5664 2024-04-02 03:27:58.890219 pinjected-0.2.28/pinjected/di/app_injected.py
+-rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.28/pinjected/di/applicative.py
+-rw-r--r--   0        0        0     7340 2024-03-26 02:52:38.836702 pinjected-0.2.28/pinjected/di/ast.py
+-rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.28/pinjected/di/async_injected.py
+-rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.28/pinjected/di/bindings.py
+-rw-r--r--   0        0        0     9753 2024-03-26 02:52:38.838842 pinjected-0.2.28/pinjected/di/decorators.py
+-rw-r--r--   0        0        0    13317 2024-03-26 02:52:38.839976 pinjected-0.2.28/pinjected/di/design.py
+-rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.28/pinjected/di/design_bind_contextx.py
+-rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.28/pinjected/di/designed.py
+-rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.28/pinjected/di/dynamic_proxy.py
+-rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.28/pinjected/di/graph.py
+-rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.28/pinjected/di/implicit_globals.py
+-rw-r--r--   0        0        0    54209 2024-04-16 03:40:34.742175 pinjected-0.2.28/pinjected/di/injected.py
+-rw-r--r--   0        0        0     1892 2023-11-06 06:59:52.887127 pinjected-0.2.28/pinjected/di/injected_analysis.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.28/pinjected/di/metadata/__init__.py
+-rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.28/pinjected/di/metadata/bind_metadata.py
+-rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.28/pinjected/di/metadata/location_data.py
+-rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.28/pinjected/di/modular_injected.py
+-rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.28/pinjected/di/monadic.py
+-rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.28/pinjected/di/overload_experimental.py
+-rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.28/pinjected/di/playground.py
+-rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.28/pinjected/di/provider.py
+-rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.28/pinjected/di/proxiable.py
+-rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.28/pinjected/di/session.py
+-rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.28/pinjected/di/sessioned.py
+-rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.28/pinjected/di/static_proxy.py
+-rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.28/pinjected/di/test_ast.py
+-rw-r--r--   0        0        0      997 2024-03-26 02:52:38.844108 pinjected-0.2.28/pinjected/di/test_dynamic_proxy.py
+-rw-r--r--   0        0        0     1500 2024-03-20 13:37:29.443496 pinjected-0.2.28/pinjected/di/test_graph.py
+-rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.28/pinjected/di/test_injected.py
+-rw-r--r--   0        0        0      452 2024-03-26 02:52:38.845073 pinjected-0.2.28/pinjected/di/test_proxiable.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.28/pinjected/di/tools/__init__.py
+-rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.28/pinjected/di/tools/add_overload.py
+-rw-r--r--   0        0        0    15106 2024-03-26 02:52:38.846281 pinjected-0.2.28/pinjected/di/util.py
+-rw-r--r--   0        0        0     1071 2023-08-25 06:23:59.157878 pinjected-0.2.28/pinjected/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.28/pinjected/exporter/__init__.py
+-rw-r--r--   0        0        0      409 2024-04-15 12:03:47.624714 pinjected-0.2.28/pinjected/exporter/llm_export_v2.py
+-rw-r--r--   0        0        0    30638 2024-04-16 06:01:09.784205 pinjected-0.2.28/pinjected/exporter/llm_exporter.py
+-rw-r--r--   0        0        0     2643 2024-04-16 05:12:14.788477 pinjected-0.2.28/pinjected/exporter/optimize_import_stmts.py
+-rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.28/pinjected/global_configs.py
+-rw-r--r--   0        0        0     2927 2024-03-26 02:52:38.847411 pinjected-0.2.28/pinjected/graph_inspection.py
+-rw-r--r--   0        0        0     2886 2024-04-15 04:38:55.875181 pinjected-0.2.28/pinjected/helper_structure.py
+-rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.28/pinjected/helpers.py
+-rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.28/pinjected/ide_supports/__init__.py
+-rw-r--r--   0        0        0     9050 2024-01-10 03:58:40.484651 pinjected-0.2.28/pinjected/ide_supports/console_run_helper.py
+-rw-r--r--   0        0        0     8329 2024-03-26 02:52:38.848041 pinjected-0.2.28/pinjected/ide_supports/create_configs.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.28/pinjected/llm_support/__init__.py
+-rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.28/pinjected/llm_support/inspect_module.py
+-rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.28/pinjected/llm_support/inspect_module_prompts.py
+-rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.28/pinjected/logging_helper.py
+-rw-r--r--   0        0        0     4121 2024-04-08 10:32:08.774921 pinjected-0.2.28/pinjected/main_impl.py
+-rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.28/pinjected/maybe_patch.py
+-rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.28/pinjected/meta_main.py
+-rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.28/pinjected/module_helper.py
+-rw-r--r--   0        0        0     2453 2024-04-15 03:39:25.763167 pinjected-0.2.28/pinjected/module_inspector.py
+-rw-r--r--   0        0        0     4701 2024-03-26 02:52:38.848756 pinjected-0.2.28/pinjected/module_var_path.py
+-rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.28/pinjected/notification.py
+-rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.28/pinjected/nx_graph_util.py
+-rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.28/pinjected/providable.py
+-rw-r--r--   0        0        0    20629 2024-01-29 15:55:46.347150 pinjected-0.2.28/pinjected/run_config_utils.py
+-rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.28/pinjected/run_config_utils_v2.py
+-rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.28/pinjected/run_helpers/__init__.py
+-rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.28/pinjected/run_helpers/config.py
+-rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.28/pinjected/run_helpers/pinjected_environments.py
+-rw-r--r--   0        0        0     9360 2024-04-15 05:43:18.485943 pinjected-0.2.28/pinjected/run_helpers/run_injected.py
+-rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.28/pinjected/runnables.py
+-rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.28/pinjected/test_package/__init__.py
+-rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.28/pinjected/test_package/child/__init__.py
+-rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.28/pinjected/test_package/child/module1.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.28/pinjected/v2/__init__.py
+-rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.28/pinjected/v2/ainjected.py
+-rw-r--r--   0        0        0     6128 2024-03-26 02:52:38.850654 pinjected-0.2.28/pinjected/v2/binds.py
+-rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.28/pinjected/v2/di.py
+-rw-r--r--   0        0        0      358 2024-03-26 02:52:38.851474 pinjected-0.2.28/pinjected/v2/keys.py
+-rw-r--r--   0        0        0      478 2024-03-26 02:52:38.851836 pinjected-0.2.28/pinjected/v2/provide_context.py
+-rw-r--r--   0        0        0     5647 2024-03-29 04:40:41.000002 pinjected-0.2.28/pinjected/v2/resolver.py
+-rw-r--r--   0        0        0    19384 2024-03-26 02:52:38.852889 pinjected-0.2.28/pinjected/visualize_di.py
+-rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.28/pinjected/viz/__init__.py
+-rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.28/pinjected/viz/graph.py
+-rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.28/pinjected/with_context.py
+-rw-r--r--   0        0        0      759 2024-04-16 06:02:54.675698 pinjected-0.2.28/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 pinjected-0.2.28/PKG-INFO
```

### Comparing `pinjected-0.2.27/LICENSE` & `pinjected-0.2.28/LICENSE`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/decoration.py` & `pinjected-0.2.28/pinjected/decoration.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/demo.py` & `pinjected-0.2.28/pinjected/demo.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/di/app_designed.py` & `pinjected-0.2.28/pinjected/di/app_designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/di/app_injected.py` & `pinjected-0.2.28/pinjected/di/app_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/di/applicative.py` & `pinjected-0.2.28/pinjected/di/applicative.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/di/ast.py` & `pinjected-0.2.28/pinjected/di/ast.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/di/decorators.py` & `pinjected-0.2.28/pinjected/di/decorators.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/di/design.py` & `pinjected-0.2.28/pinjected/di/design.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/di/designed.py` & `pinjected-0.2.28/pinjected/di/designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/di/dynamic_proxy.py` & `pinjected-0.2.28/pinjected/di/dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/di/graph.py` & `pinjected-0.2.28/pinjected/di/graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/di/injected.py` & `pinjected-0.2.28/pinjected/di/injected.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 import asyncio
 import functools
 import hashlib
 import inspect
 import sys
 from copy import copy
 from dataclasses import dataclass, field
+from inspect import Traceback
 from typing import List, Generic, Union, Callable, TypeVar, Tuple, Set, Dict, Any, Awaitable
 
 from frozendict import frozendict
 from loguru import logger
 from makefun import create_function
 from returns.result import safe
 
 from pinjected.di.injected_analysis import get_instance_origin
 from pinjected.di.proxiable import DelegatedVar
-from pinjected.v2.ainjected import MappedAInjected
 
 T, U = TypeVar("T"), TypeVar("U")
 
 A = TypeVar("A")
 B = TypeVar("B")
 
 INJECTED_CONTEXT = frozendict()
@@ -39,24 +39,28 @@
 Okey, so let's implement this and be aware that the map function will erase it.
 So the use needs to be careful to add context at the very end, for running purposes.
 """
 
 
 @dataclass
 class FrameInfo:
+    original_frame: object
+    trc: Traceback
     filename: str
     line_number: int
     function_name: str
     sources: List[str]
     line_idx_in_sources: int
 
 
 def get_frame_info(stack_idx) -> Union[None, FrameInfo]:
     try:
-        return FrameInfo(*inspect.getframeinfo(inspect.stack(0)[stack_idx][0]))
+        original_trc = inspect.stack(0)[stack_idx][0]
+        trc: Traceback = inspect.getframeinfo(original_trc)
+        return FrameInfo(original_trc, trc, *trc)
     except Exception as e:
         return None
 
 
 def partialclass(name, cls, *args, **kwds):
     """
     copied from https://stackoverflow.com/questions/38911146/python-equivalent-of-functools-partial-for-a-class-constructor
@@ -336,15 +340,15 @@
             __skeleton__ = f"""async def {new_func_sig}:
     \"\"\"
     {__doc__}
     \"\"\"
 """
             new_func.__skeleton__ = __skeleton__
 
-            #logger.info(f"result of makefun_impl:{new_func}")
+            # logger.info(f"result of makefun_impl:{new_func}")
 
             return new_func
 
         makefun_impl.__name__ = original_function.__name__
         makefun_impl.__module__ = original_function.__module__
         makefun_impl.__original__ = original_function
 
@@ -355,21 +359,22 @@
             makefun_impl.__original_code__ = inspect.getsource(original_function.__func__)
             makefun_impl.__original_file__ = inspect.getfile(original_function.__func__)
         else:
             makefun_impl.__original_code__ = safe(inspect.getsource)(original_function).value_or("not available")
             makefun_impl.__original_file__ = safe(inspect.getfile)(original_function).value_or("not available")
 
         makefun_impl.__doc__ = original_function.__doc__
-        #logger.info(f"injection_targets:{injection_targets}")
+        # logger.info(f"injection_targets:{injection_targets}")
         injected_kwargs = Injected.dict(**injection_targets)
-        #logger.info(f"injected_kwargs:{injected_kwargs}")
+        # logger.info(f"injected_kwargs:{injected_kwargs}")
         # hmm?
         # Ah, so upon calling instance.method(), we need to manually check if __self__ is present?
         bound_func = Injected.bind(makefun_impl, injected_kwargs=injected_kwargs)
         bound_func.__is_async_function__ = inspect.iscoroutinefunction(original_function)
+        bound_func.__is_partial__ = True # this is to indicate that the bound_func is supposed to be used with PartialInjectedFunction.
         injected_factory = PartialInjectedFunction(src=bound_func)
         # the inner will be called upon calling the injection result.
         # This involves many internal Injecte instances. can I make it simler?
         # it takes *by_name, mzip, and map.
         injected_factory.__is_async_function__ = bound_func.__is_async_function__
         injected_factory.__runnable_metadata__ = {
             "kind": "callable"
@@ -399,20 +404,24 @@
 
             async def _a_target_function(*args, **kwargs):
                 return _target_function_(*args, **kwargs)
 
             _a_target_function.__signature__ = inspect.signature(_target_function_)
 
             async_target_function = _a_target_function
+            async_target_function.__original_code__ = safe(inspect.getsource)(_target_function_).value_or(
+                "not available")
         else:
             async_target_function = _target_function_
-        return InjectedFunction(
+        res = InjectedFunction(
+            original_function=_target_function_,
             target_function=async_target_function,
             kwargs_mapping=kwargs_mapping
         )
+        return res
 
     @staticmethod
     def direct(_target_function, **kwargs) -> "Injected":
         """
         uses Injected.pure by default unless the parameter is an instance of Injected.
         :param _target_function:
         :param kwargs:
@@ -481,22 +490,26 @@
 
             async def async_f(*args, **kwargs):
                 return f(*args, **kwargs)
 
             new_f = async_f
         else:
             new_f = f
-        return MappedInjected(self, new_f)
+        return MappedInjected(self, new_f, original_mapper=f)
 
     def from_impl(impl: Callable, dependencies: Set[str]):
         return GeneratedInjected(impl, dependencies)
 
     @staticmethod
     def pure(value):
-        return InjectedPure(value)
+        res = InjectedPure(value)
+        # I need to set the file that called this function.
+        res.__definition_frame__ = get_frame_info(2)
+        res.__original_file__ = get_frame_info(2).filename
+        return res
 
     @staticmethod
     def by_name(name: str):
         return InjectedByName(name, )
 
     def zip(self, other: "Injected[U]") -> "Injected[Tuple[T,U]]":
         assert isinstance(self, Injected)
@@ -553,17 +566,18 @@
         return self.zip(other).map(
             lambda t: lambda *args, **kwargs: t[1](t[0](*args, **kwargs))
         )
 
     @staticmethod
     def dict(**kwargs: "Injected") -> "Injected[Dict]":
         # raise RuntimeError("disabled")
-        keys = list(kwargs.keys())
+        #keys = list(kwargs.keys())
 
-        return Injected.mzip(*[kwargs[k] for k in keys]).map(lambda t: {k: v for k, v in zip(keys, t)})
+        #return Injected.mzip(*[kwargs[k] for k in keys]).map(lambda t: {k: v for k, v in zip(keys, t)})
+        return DictInjected(**kwargs)
 
     @property
     def proxy(self) -> DelegatedVar:
         """use this to modify injected variables freely without map.
         call eval() at the end to finish modification
         # it seems this thing is preventing from pickling?
         """
@@ -919,19 +933,20 @@
     def dynamic_dependencies(self) -> Set[str]:
         return self.src.dynamic_dependencies() | self._dynamic_dependencies
 
 
 class MappedInjected(Injected):
     __match_args__ = ("src", "f")
 
-    def __init__(self, src: Injected[T], f: Callable[[T], Awaitable[U]]):
+    def __init__(self, src: Injected[T], f: Callable[[T], Awaitable[U]], original_mapper):
         super(MappedInjected, self).__init__()
         assert inspect.iscoroutinefunction(f), f"{f} is not a coroutine function"
         self.src = src
         self.f: Callable[[T], Awaitable[U]] = f
+        self.original_mapper = original_mapper
 
     def dependencies(self) -> Set[str]:
         return self.src.dependencies()
 
     def get_provider(self):
         async def impl(**kwargs):
             assert self.dependencies() == set(
@@ -1017,19 +1032,21 @@
 
 
 class InjectedFunction(Injected[T]):
     # since the behavior differs in classes extending Generic[T]
     __match_args__ = ("target_function", "kwargs_mapping")
 
     def __init__(self,
+                 original_function,
                  target_function: Callable,
                  kwargs_mapping: Dict[str, Union[str, type, Callable, Injected, DelegatedVar]]
                  ):
         # I think we need to know where this class is instantiated outside of pinjected_package
         self.origin_frame = get_instance_origin("pinjected")
+        self.original_function = original_function
         super().__init__()
         assert not isinstance(target_function, (Injected, DelegatedVar))
         assert callable(target_function)
         self.target_function = target_function
         assert inspect.iscoroutinefunction(self.target_function), f"{self.target_function} is not a coroutine function"
         self.kwargs_mapping = copy(kwargs_mapping)
         for k, v in self.kwargs_mapping.items():
@@ -1214,14 +1231,48 @@
     def dynamic_dependencies(self) -> Set[str]:
         res = set()
         for s in self.srcs:
             res |= s.dynamic_dependencies()
 
         return res
 
+class DictInjected(Injected):
+    __match_args__ = ("srcs",)
+
+    def __init__(self, **srcs: Injected):
+        super().__init__()
+        self.srcs = {k: Injected.ensure_injected(v) for k, v in srcs.items()}
+        assert all(isinstance(s, Injected) for s in self.srcs.values()), self.srcs
+
+    def dependencies(self) -> Set[str]:
+        res = set()
+        for s in self.srcs.values():
+            res |= s.dependencies()
+
+        return res
+
+    def get_provider(self):
+        async def impl(**kwargs):  # can we pickle this though?
+            res = {}
+            for k, s in self.srcs.items():
+                r = s.get_provider()(**{k: kwargs[k] for k in s.dependencies()})
+                if not inspect.iscoroutinefunction(s.get_provider()):
+                    raise RuntimeError(f"provider is not a corountine function:{s}")
+                res[k] = await r
+            return res
+
+        signature = self.get_signature()
+        return create_function(func_signature=signature, func_impl=impl)
+
+    def dynamic_dependencies(self) -> Set[str]:
+        res = set()
+        for s in self.srcs.values():
+            res |= s.dynamic_dependencies()
+
+        return res
 
 def _injected_factory(**targets: Injected):
     def _impl(f):
         return Injected.partial(f, **targets)
 
     return _impl
```

### Comparing `pinjected-0.2.27/pinjected/di/injected_analysis.py` & `pinjected-0.2.28/pinjected/di/injected_analysis.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/di/modular_injected.py` & `pinjected-0.2.28/pinjected/di/modular_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/di/overload_experimental.py` & `pinjected-0.2.28/pinjected/di/overload_experimental.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/di/proxiable.py` & `pinjected-0.2.28/pinjected/di/proxiable.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/di/session.py` & `pinjected-0.2.28/pinjected/di/session.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/di/sessioned.py` & `pinjected-0.2.28/pinjected/di/sessioned.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/di/static_proxy.py` & `pinjected-0.2.28/pinjected/di/static_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/di/test_dynamic_proxy.py` & `pinjected-0.2.28/pinjected/di/test_dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/di/test_graph.py` & `pinjected-0.2.28/pinjected/di/test_graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/di/test_injected.py` & `pinjected-0.2.28/pinjected/di/test_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/di/tools/add_overload.py` & `pinjected-0.2.28/pinjected/di/tools/add_overload.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/di/util.py` & `pinjected-0.2.28/pinjected/di/util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/exceptions.py` & `pinjected-0.2.28/pinjected/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/exporter/llm_exporter.py` & `pinjected-0.2.28/pinjected/ide_supports/console_run_helper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,248 +1,248 @@
 import ast
-import inspect
-import uuid
-from dataclasses import dataclass
+import json
+from contextlib import contextmanager
 from pathlib import Path
-from typing import Callable, Awaitable
+from pprint import pformat
 
-import astor
+import click
 
-from pinjected import Design, Injected
-from pinjected.di.app_injected import EvaledInjected
-from pinjected.di.ast import Expr, BiOp, Call, Attr, GetItem, Object
-from pinjected.di.injected import InjectedPure, InjectedFunction, PartialInjectedFunction, ZippedInjected, \
-    MappedInjected, InjectedByName
-from pinjected.di.proxiable import DelegatedVar
-
-
-@dataclass
-class PinjectedCodeExporter:
-    src: Design
-    a_llm: Callable[[str], Awaitable[str]]
-
-    def __post_init__(self):
-        digraph = self.src.to_vis_graph()
-        self.mappings = {**digraph.explicit_mappings}
-
-    @staticmethod
-    async def to_source__instance(assign_target, tgt: InjectedPure):
-        # wait, tgt.value must be recoverable from the value. but it should always be.
-        return f"{assign_target} = {tgt.value}"
-
-    async def extract_lambda(self, f):
-        from loguru import logger
-        logger.info(f"extracting lambda from {f.__name__}")
-        src = inspect.getsource(f)
-        prompt = f"""
-    Please extract the lambda expression in question from function:{f.__name__} below.
-    ```
-    {src}
-    ```
-    The answer must be a valid python expression without comments, in the form of 
-    lambda ...: ...
-    """
-        return await self.a_llm(prompt)
-
-    async def get_source_func(self, assign_target, f):
-        from loguru import logger
-        if hasattr(f, "__original_code__"):
-            # logger.info(f"retrieving source from __original_code__")
-            src = f.__original_code__
-        else:
-            src = inspect.getsource(f)
-        """
-        @injected
-        def g(f,/,x):
-            return f(x=x,y=1)
-        
-        I need to remove @injected and positional only arguments. from this source, using AST.
-        """
-        # logger.info(f"getting source:{f.__name__}->\n{src}")
-        if f.__name__.endswith('<lambda>'):
-            src = await self.extract_lambda(f)
-            return f"{assign_target} = {src}\n"
-        else:
-            tree = ast.parse(src)
-            PinjectedCodeExporter.un_pinjected(assign_target, tree)
-            unparsed = ast.unparse(tree)
-            logger.debug(f"un_pinjected->\n{unparsed}")
-            return unparsed
-            # return astor.to_source(tree)
-
-    # Function to remove the @injected decorator and positional-only argument marker
-    @staticmethod
-    def un_pinjected(assignment, tree):
-        deletion_targets = {"injected", "instance"}
-        for node in ast.walk(tree):
-            # Check if the node is a function definition
-            if isinstance(node, ast.FunctionDef) or isinstance(node, ast.AsyncFunctionDef):
-                # Remove @injected decorator if present
-                is_instance = bool([decorator for decorator in node.decorator_list if
-                                    hasattr(decorator, 'id') and decorator.id == 'instance'])
-                node.decorator_list = [decorator for decorator in node.decorator_list if
-                                       not (hasattr(decorator, 'id') and decorator.id in deletion_targets)]
-                node.name = assignment
-
-                # Check for positional only arguments (Python 3.8+)
-                if node.args.posonlyargs:
-                    # Remove the positional-only argument marker
-                    node.args.posonlyargs = []
-
-                if is_instance:
-                    # Remove all args if it's @instance
-                    node.args.args = []
-
-    @staticmethod
-    def new_symbol():
-        return str(uuid.uuid4())[:3]
-
-    @staticmethod
-    def tmp_symbol():
-        return "tmp_" + PinjectedCodeExporter.new_symbol()
-
-    def find_matching_mapping(self, data: Injected):
-        from loguru import logger
-        logger.info(f"finding matching mapping for {data}")
-        match data:
-            case InjectedFunction(f, kwargs_mapping):
-                for k, v in self.mappings.items():
-                    match v:
-                        case PartialInjectedFunction(InjectedFunction(_f)) if f == _f:
-                            return k
-        return None
-
-    async def expr_to_source(self, assign_target: str, expr: Expr, visited):
-        from loguru import logger
-        predef_buffer = ""
-
-        async def to_src(e: Expr):
-            nonlocal predef_buffer
-            match e:
-                case BiOp(sym, left, right):
-                    return f"{await to_src(left)} {sym} {await to_src(right)}"
-                case Call(f, args, kwargs):
-                    args_str = ""
-                    if args:
-                        args_str = ','.join([await to_src(a) for a in args])
-                    if kwargs:
-                        args_str += ',' + ','.join([f'{k}={await to_src(v)}' for k, v in kwargs.items()])
-                    return f"{await to_src(f)}({args_str})"
-                case Attr(src, attr):
-                    return f"{await to_src(src)}.{attr}"
-                case GetItem(src, key):
-                    return f"{await to_src(src)}[{await to_src(key)}]"
-                case Object(InjectedByName(name)):
-                    return name
-                case Object(Injected() | DelegatedVar() as data):
-                    # we don't know if the data is from design or not, so the full function is constructed.
-                    # we need to look at a table...
-                    vid_to_key = {id(v): k for k, v in self.mappings.items()}
-                    sym = self.find_matching_mapping(data)
-                    if sym is None:
-                        if id(data) in vid_to_key:
-                            sym = vid_to_key[id(data)]
-                            logger.info(f"using symbol:{sym}")
-                        else:
-                            sym = "tmp__" + self.new_symbol()
-                        # here, we are seeing InjectedFunction
-                        # We need to handle InjectedByName
-                        logger.info(f"creating new symbol:{sym}, for {data}")
-                    if sym not in visited:
-                        predef_buffer += f"{await self.to_source(sym, data, visited)}\n"
-                    return sym
-                case Object(str() as literal):
-                    return f'"{literal}"'
-                case Object(float() | int() as num):
-                    return str(num)
-                case Object(Path() as p):
-                    return f"Path({p})"
-                case Object(unknown):
-                    raise ValueError(f"Unsupported object:{unknown},{type(unknown)}")
-                case _:
-                    raise ValueError(f"Unsupported type {e}, {type(e)}")
-
-        src = await to_src(expr)
-        code = f"{predef_buffer}\n{assign_target} = {src}"
-        if predef_buffer.strip():
-            prompt = f"""
-Please simplify the following python script to remove tmp functions and variables, as much as possible.
-The variables/functions to simplify have 'tmp' as their prefix.
-The script's purpose is to calculate {assign_target}.
-```
-{code}
-```
-The answer should not contain any explanation or triple ticks.
-Functions not in scope does not need to be defined.
-Beware that {assign_target} name must be preserved.
-    """
-            logger.debug(f"prompt:\n{prompt}")
-            simplified = await self.a_llm(prompt)
-            simplified = simplified.replace('```', "")
-            logger.debug(f"simplified:\n{simplified}")
-            return simplified
-        return code
-
-    async def to_source(self, assign_target: str, src: Injected, visited: set = None):
-        if visited is None:
-            visited = set()
-        code = ""
-        if isinstance(src, str):
-            src = Injected.by_name(src)
-        src = Injected.ensure_injected(src)
-        from loguru import logger
-        logger.info(f"visiting {assign_target}")
-        for dep in src.complete_dependencies:
-            if dep not in visited:
-                if dep not in self.mappings:
-                    logger.error(f"{dep} not in mappings! for {src}")
-                visited |= {dep}
-                code += await self.to_source(dep, self.mappings[dep], visited)
-
-        match src:
-            case InjectedPure() as p:
-                last_code = await self.to_source__instance(assign_target, p)
-            case InjectedFunction(tgt_func, _km) as f:
-                last_code = await self.get_source_func(assign_target, tgt_func)
-            case PartialInjectedFunction(InjectedFunction(func)) as pif:
-                last_code = await self.get_source_func(assign_target, func)
-            case EvaledInjected(value, tree):
-                from loguru import logger
-                logger.info(tree)
-                logger.info(value)
-                last_code = await self.expr_to_source(assign_target, tree, visited)
-            case ZippedInjected(a, b):
-                left, right = self.tmp_symbol() + "left", self.tmp_symbol() + "right"
-                prep = (await self.to_source(left, a, visited)
-                        + "\n"
-                        + await self.to_source(right, b, visited)
-                        + "\n")
-                last_code = prep + "\n" + f"{assign_target} = ({left},{right})\n"
-            case MappedInjected(src, f):
-                map_f = self.tmp_symbol()
-                map_src = self.tmp_symbol()
-                prep = await self.get_source_func(map_f, f) + "\n"
-                prep += await self.to_source(map_src, src, visited) + "\n"
-                last_code = prep + f"{assign_target} = {map_f}({map_src})\n"
-            case InjectedByName(name):
-                last_code = await self.to_source(name, self.mappings[name], visited=visited)
-            case _:
-                raise ValueError(f"Unsupported type {src}")
-        code += last_code + "\n"
-        return code
-
-    async def simplify_code(self, target_name, code):
-        prompt = f"""
-    Please convert the following python into simplified python script?
-    This script is for calculating result variable "{target_name}".
-    ```
-    {code}
-    ```
-    Simplification should involve removing placeholder function into an expression.
-    The answer should keep properly named variables and functions.
-    Variable assignments for tmp variables should be simplified as much as possible.
-    If tmp variables cannot be simplified, it should be renamed to proper variable names.
+from pinjected import injected, Injected
+
+
+@click.group()
+def main():
+    pass
+
+
+@main.command()
+@click.argument('script_path', type=click.Path(exists=True))
+@click.argument('func_name')
+def extract_func_source_and_imports(script_path: str, func_name: str):
+    func_and_imports = extract_func_source_and_imports_dict(func_name, script_path)
+
+    # Prepare the data containing the requested function source and imports
+    data = {
+        'code': func_and_imports['functions'].get(func_name, f"Function {func_name} not found."),
+        'imports': list(set(func_and_imports['imports']))
+    }
+    # Convert the data to JSON format and print it
+    text = json.dumps(data, indent=4)
+    # Ensure that the output does not contain "<pinjected>" to prevent code injection
+    assert "<pinjected>" not in text
+    text = "<pinjected>\n" + text + "\n</pinjected>"
+    print(text)
+
+
+def extract_func_source_and_imports_dict(script_path):
+    # Read the content of the script file
+    file_content = Path(script_path).read_text()
+    # Parse the file content into an AST node tree
+    node_tree = ast.parse(file_content)
+
+    # Function to get the source code of decorators with "@"
+    def get_decorators_source(decorators):
+        return ["@" + ast.get_source_segment(file_content, decorator).strip() for decorator in decorators]
+
+    # Initialize a dictionary to store functions and imports
+    func_and_imports = {'functions': {}, 'imports': []}
+    # Walk through the AST nodes
+    for node in ast.walk(node_tree):
+        # Check if the node is a function
+        if isinstance(node, ast.FunctionDef):
+            # Get decorators source code with "@"
+            decorators_source = get_decorators_source(node.decorator_list)
+            # Get the source code of the function definition
+            func_source_lines = file_content.splitlines()[node.lineno - 1:node.end_lineno]
+            func_source = "\n".join(decorators_source + func_source_lines)
+            # Store the function source code in the dictionary
+            func_and_imports['functions'][node.name] = func_source
+        # Check if the node is an import or import from statement
+        elif isinstance(node, (ast.Import, ast.ImportFrom)):
+            # Get the source code of the import
+            import_source = ast.get_source_segment(file_content, node)
+            # Store the import source code in the list
+            func_and_imports['imports'].append(import_source)
+    return func_and_imports
+
+
+def create_run_design(script_path: str):
+    """
+    This command should load the __meta_design__ and return the final design.
+    :param script_path:
+    :return:
+    """
+    from pinjected.helper_structure import MetaContext
+    __design__ = MetaContext.gather_from_path(Path(script_path)).accumulated
+    __graph__ = __design__.to_graph().auto_sync()
+    # mc:MetaContext = MetaContext.gather_from_path(Path(script_path))
+    # return mc.accumulated
+
+
+class WithBlockVisitor(ast.NodeVisitor):
+    def __init__(self):
+        self.result = {}
+
+    def visit_With(self, node):
+        # In Python 3.9 and above, 'with' statements use 'items' which is a list of 'withitem' objects.
+        # In earlier versions, the context expression was directly available as 'context_expr'.
+        # We'll check for both to ensure compatibility.
+        with_items = getattr(node, 'items', None) or [node]
+
+        for item in with_items:
+            context_expr = getattr(item, 'context_expr', None) or item
+
+            # Check if the with statement contains a call to reload
+            if isinstance(context_expr, ast.Call) and getattr(context_expr.func, 'id', None) == 'reload':
+                # Get the list of reload targets
+                reload_targets = [arg.s for arg in context_expr.args]
+                # Process each item in the with block
+                for body_item in node.body:
+                    if isinstance(body_item, ast.AnnAssign) and isinstance(body_item.target, ast.Name):
+                        variable_name = body_item.target.id
+                        # Assign reload targets to the variable in the result dict
+                        self.result[variable_name] = {
+                            'reload_targets': reload_targets
+                        }
+
+
+def extract_with_block_structure(source_code):
+    # Parse the source code into an AST
+    parsed_ast = ast.parse(source_code)
+    # Create a visitor instance
+    visitor = WithBlockVisitor()
+    # Visit the parsed AST
+    visitor.visit(parsed_ast)
+    # Return the collected results
+    return visitor.result
+
+
+def extrract_assignments(source_code):
+    """
+    Extract assignment statements from the given Python source code.
+    Returns a dictionary with variable names as keys and the source code of the assigned value as values.
+    This updated version handles type annotations.
     """
-        return await self.a_llm(prompt)
 
-    async def export(self, target):
-        return await self.to_source(target, self.mappings[target])
+    class AssignmentVisitor(ast.NodeVisitor):
+        def __init__(self):
+            self.assignments = {}
+
+        def visit_AnnAssign(self, node):
+            # Handle assignments with annotations
+            if isinstance(node.target, ast.Name):
+                var_name = node.target.id
+                value_code = ast.get_source_segment(source_code, node.value)
+                self.assignments[var_name] = value_code
+
+        def visit_Assign(self, node):
+            # Handle normal assignments
+            for target in node.targets:
+                if isinstance(target, ast.Name):
+                    var_name = target.id
+                    value_code = ast.get_source_segment(source_code, node.value)
+                    self.assignments[var_name] = value_code
+                # Handle tuple assignments
+                elif isinstance(target, ast.Tuple):
+                    for elt in target.elts:
+                        if isinstance(elt, ast.Name):
+                            var_name = elt.id
+                            value_code = ast.get_source_segment(source_code, node.value)
+                            self.assignments[var_name] = value_code
+
+    # Parse the source code into an AST
+    parsed_ast = ast.parse(source_code)
+    # Create a visitor instance
+    visitor = AssignmentVisitor()
+    # Visit the parsed AST
+    visitor.visit(parsed_ast)
+    # Return the collected assignments
+    return visitor.assignments
+
+@main.command()
+@click.argument('script_path', type=click.Path(exists=True))
+@click.argument('target_name')
+def generate_code_with_reload(
+        script_path: str,
+        target_name: str,
+):
+    """
+    1. find all function names using extract_func_source_and_imports
+    2. check the reload target of target_name
+    3. concat all sources and return it as a pinjected json
+    :param script_path:
+    :param target_name:
+    :return:
+    """
+    from loguru import logger
+    source = Path(script_path).read_text()
+    func_table = extract_func_source_and_imports_dict(script_path)
+    logger.info(f"func_table:{pformat(func_table)}")
+    reload_table = extract_with_block_structure(source)
+    if target_name not in reload_table:
+        reload_targets = []
+    else:
+        reload_targets = reload_table[target_name]['reload_targets']
+    funcs_to_reload = [func_table['functions'][func_name] for func_name in reload_targets]
+    imports = func_table['imports']
+    imports = '\n'.join(imports)
+    func_defs = '\n'.join(funcs_to_reload)
+    assignments: dict[str, str] = extrract_assignments(source)
+    # logger.info(pformat(assignments))
+
+    """
+    How can I add the child session?
+    """
+    code = f"""
+if '__graph__' not in globals():
+    from pinjected.helper_structure import MetaContext
+    from pathlib import Path
+    exec(Path("{script_path}").read_text())
+    __meta_context__ = MetaContext.gather_from_path(Path("{script_path}"))
+    __design__ = __meta_context__.final_design
+    __graph__ = __design__.to_graph().auto_sync()
+{imports}
+{func_defs}
+{target_name} = {assignments[target_name]}
+__graph__[{target_name}]
+"""
+    # oops, target_name is not in the scope
+    logger.debug(f"generated code:{code}")
+    data = "<pinjected>\n" + json.dumps({'code': code}) + "\n</pinjected>"
+    print(data)
+
+
+@injected
+def test_target_function():
+    print(f"hello")
+
+
+@contextmanager
+def reload(*targets):
+    # this is just a placeholder for the AST visitor
+    yield
+
+
+with reload('test_target_function'):
+    x = 0
+    run_test: Injected = test_target_function
+
+
+def is_pydevd():
+    import os
+    return 'PYDEVD_LOAD_VALUES_ASYNC' in os.environ
+
+
+if __name__ == '__main__' and not is_pydevd():
+    """
+    this code generation works, 
+    now the remaining task is, 
+    how to get the script path and its var name,
+    
+    Options:
+    1. use the gutter icon
+    2. action: run current thing? nah. 
+    so,, what is the way to rerun the current thing? quickly?
+    I think, placing a cursor on the target and then running the command is the best way.
+    so, let's make an action. 
+    """
+    main()
```

### Comparing `pinjected-0.2.27/pinjected/graph_inspection.py` & `pinjected-0.2.28/pinjected/graph_inspection.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/helper_structure.py` & `pinjected-0.2.28/pinjected/helper_structure.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,20 +48,30 @@
             overrides=overrides
         )
 
         return MetaContext(
             trace=designs,
             accumulated=res
         )
+
     @property
     def final_design(self):
         acc = self.accumulated
         design = load_variable_by_module_path(acc.provide('default_design_paths')[0])
         return design + acc.provide('overrides')
 
+    @property
+    async def a_final_design(self):
+        from pinjected.run_helpers.run_injected import load_user_default_design, load_user_overrides_design
+        acc = self.accumulated
+        g = acc.to_resolver()
+        module_path = (await g['default_design_paths'])[0]
+        design = load_variable_by_module_path(module_path)
+        return load_user_default_design() + design + (await g['overrides']) + load_user_overrides_design()
+
 
 @dataclass
 class RunnablePair:
     target: Injected
     design: Design
 
     def run(self):
```

### Comparing `pinjected-0.2.27/pinjected/helpers.py` & `pinjected-0.2.28/pinjected/helpers.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/ide_supports/create_configs.py` & `pinjected-0.2.28/pinjected/ide_supports/create_configs.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/llm_support/inspect_module.py` & `pinjected-0.2.28/pinjected/llm_support/inspect_module.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/llm_support/inspect_module_prompts.py` & `pinjected-0.2.28/pinjected/llm_support/inspect_module_prompts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/main_impl.py` & `pinjected-0.2.28/pinjected/main_impl.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/maybe_patch.py` & `pinjected-0.2.28/pinjected/maybe_patch.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/module_helper.py` & `pinjected-0.2.28/pinjected/module_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/module_inspector.py` & `pinjected-0.2.28/pinjected/module_inspector.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 
 
 @dataclass
 class ModuleVarSpec(Generic[T]):
     var: T
     var_path: str
 
+    @property
+    def module_file_path(self):
+        from pinjected.module_var_path import ModuleVarPath
+        return ModuleVarPath(self.var_path).module_file_path
+
 
 @memoize
 def get_project_root(start_path: str) -> str:
     from loguru import logger
     current_path = os.path.dirname(os.path.abspath(start_path))
     logger.debug(f"current_path:{current_path}")
     while os.path.exists(os.path.join(current_path, "__init__.py")):
```

### Comparing `pinjected-0.2.27/pinjected/module_var_path.py` & `pinjected-0.2.28/pinjected/module_var_path.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/notification.py` & `pinjected-0.2.28/pinjected/notification.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/nx_graph_util.py` & `pinjected-0.2.28/pinjected/nx_graph_util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/run_config_utils.py` & `pinjected-0.2.28/pinjected/run_config_utils.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/run_config_utils_v2.py` & `pinjected-0.2.28/pinjected/run_config_utils_v2.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/run_helpers/config.py` & `pinjected-0.2.28/pinjected/run_helpers/config.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/run_helpers/run_injected.py` & `pinjected-0.2.28/pinjected/run_helpers/run_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/runnables.py` & `pinjected-0.2.28/pinjected/runnables.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/test_package/__init__.py` & `pinjected-0.2.28/pinjected/test_package/__init__.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/test_package/child/module1.py` & `pinjected-0.2.28/pinjected/test_package/child/module1.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/v2/ainjected.py` & `pinjected-0.2.28/pinjected/v2/ainjected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/v2/binds.py` & `pinjected-0.2.28/pinjected/v2/binds.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/v2/di.py` & `pinjected-0.2.28/pinjected/v2/di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/v2/resolver.py` & `pinjected-0.2.28/pinjected/v2/resolver.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pinjected/visualize_di.py` & `pinjected-0.2.28/pinjected/visualize_di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.27/pyproject.toml` & `pinjected-0.2.28/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pinjected"
-version = "0.2.27"
+version = "0.2.28"
 description = "Immutable Dependency Injection for Python."
 authors = [ "proboscis <nameissoap@gmail.com>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 returns = "^0.21.0"
@@ -23,13 +23,14 @@
 pyvis = "^0.3.2"
 makefun = "^1.15.1"
 loguru = "^0.7.0"
 rich = "^13.7.0"
 snoop = "^0.4.3"
 pydantic = "^2.6.2"
 astor = "^0.8.1"
+injected-utils = "^0.1.7"
 
 [tool.poetry.scripts]
 pinjected = "pinjected.main_impl:main"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
```

### Comparing `pinjected-0.2.27/PKG-INFO` & `pinjected-0.2.28/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinjected
-Version: 0.2.27
+Version: 0.2.28
 Summary: Immutable Dependency Injection for Python.
 License: MIT
 Author: proboscis
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: astor (>=0.8.1,<0.9.0)
 Requires-Dist: cloudpickle (>=2.2.1,<3.0.0)
 Requires-Dist: cytoolz (>=0.12.2,<0.13.0)
 Requires-Dist: expression (>=4.2.4,<5.0.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: frozendict (>=2.3.8,<3.0.0)
+Requires-Dist: injected-utils (>=0.1.7,<0.2.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: makefun (>=1.15.1,<2.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: pydantic (>=2.6.2,<3.0.0)
 Requires-Dist: pyvis (>=0.3.2,<0.4.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: returns (>=0.21.0,<0.22.0)
```

