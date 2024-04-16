# Comparing `tmp/rio_ui-0.5.7.tar.gz` & `tmp/rio_ui-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rio_ui-0.5.7.tar", max compression
+gzip compressed data, was "rio_ui-0.5.8.tar", max compression
```

## Comparing `rio_ui-0.5.7.tar` & `rio_ui-0.5.8.tar`

### file list

```diff
@@ -1,216 +1,216 @@
--rw-r--r--   0        0        0    35149 2024-04-06 18:09:28.058340 rio_ui-0.5.7/LICENSE.txt
--rw-r--r--   0        0        0     7217 2024-04-14 14:22:40.210263 rio_ui-0.5.7/README.md
--rw-r--r--   0        0        0     2441 2024-04-14 19:53:24.034814 rio_ui-0.5.7/pyproject.toml
--rw-r--r--   0        0        0      676 2024-04-08 18:37:44.149116 rio_ui-0.5.7/rio/__init__.py
--rw-r--r--   0        0        0       91 2024-04-06 18:09:28.078340 rio_ui-0.5.7/rio/__main__.py
--rw-r--r--   0        0        0    19313 2024-04-09 19:38:54.555684 rio_ui-0.5.7/rio/app.py
--rw-r--r--   0        0        0    32065 2024-04-14 19:29:03.548737 rio_ui-0.5.7/rio/app_server.py
--rw-r--r--   0        0        0      233 2024-04-06 18:09:28.081673 rio_ui-0.5.7/rio/assets/hosted/README.md
--rw-r--r--   0        0        0   557380 2024-04-06 18:09:28.088340 rio_ui-0.5.7/rio/assets/hosted/fonts/Noto Sans/NotoSans-Bold.ttf
--rw-r--r--   0        0        0   401608 2024-04-06 18:09:28.091673 rio_ui-0.5.7/rio/assets/hosted/fonts/Noto Sans/NotoSans-BoldItalic.ttf
--rw-r--r--   0        0        0   403724 2024-04-06 18:09:28.095007 rio_ui-0.5.7/rio/assets/hosted/fonts/Noto Sans/NotoSans-Italic.ttf
--rw-r--r--   0        0        0   556216 2024-04-06 18:09:28.098340 rio_ui-0.5.7/rio/assets/hosted/fonts/Noto Sans/NotoSans-Regular.ttf
--rw-r--r--   0        0        0     4449 2024-04-06 18:09:28.098340 rio_ui-0.5.7/rio/assets/hosted/fonts/Noto Sans/OFL.txt
--rw-r--r--   0        0        0    11560 2024-04-06 18:09:28.101673 rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto/LICENSE.txt
--rw-r--r--   0        0        0   167336 2024-04-06 18:09:28.101673 rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   171508 2024-04-06 18:09:28.105007 rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   170504 2024-04-06 18:09:28.105007 rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   168260 2024-04-06 18:09:28.105007 rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0    11560 2024-04-06 18:09:28.098340 rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto Mono/LICENSE.txt
--rw-r--r--   0        0        0    87392 2024-04-06 18:09:28.098340 rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Bold.ttf
--rw-r--r--   0        0        0    94636 2024-04-06 18:09:28.101673 rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf
--rw-r--r--   0        0        0    94372 2024-04-06 18:09:28.101673 rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Italic.ttf
--rw-r--r--   0        0        0    87236 2024-04-06 18:09:28.101673 rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Regular.ttf
--rw-r--r--   0        0        0    54189 2024-04-08 17:00:05.405088 rio_ui-0.5.7/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png
--rw-r--r--   0        0        0    31665 2024-04-06 18:09:28.105007 rio_ui-0.5.7/rio/assets/hosted/rio-logos/rio-logo-square.png
--rw-r--r--   0        0        0  1081400 2024-04-07 20:27:02.369218 rio_ui-0.5.7/rio/assets/icon-sets/material.tar.xz
--rw-r--r--   0        0        0    14992 2024-04-14 09:27:29.097282 rio_ui-0.5.7/rio/assets/icon-sets/rio.tar.xz
--rw-r--r--   0        0        0     1096 2024-04-06 18:09:28.108340 rio_ui-0.5.7/rio/assets/icon-sets/styling.tar.xz
--rw-r--r--   0        0        0     8798 2024-04-12 12:19:28.613327 rio_ui-0.5.7/rio/assets.py
--rw-r--r--   0        0        0     3316 2024-04-06 18:09:28.108340 rio_ui-0.5.7/rio/byte_serving.py
--rw-r--r--   0        0        0     7389 2024-04-10 21:00:39.348528 rio_ui-0.5.7/rio/cli/__init__.py
--rw-r--r--   0        0        0     2392 2024-04-08 18:37:44.152450 rio_ui-0.5.7/rio/cli/cli_instance.py
--rw-r--r--   0        0        0     6642 2024-04-06 18:09:28.108340 rio_ui-0.5.7/rio/cli/nice_traceback.py
--rw-r--r--   0        0        0    13832 2024-04-12 10:18:09.239288 rio_ui-0.5.7/rio/cli/project.py
--rw-r--r--   0        0        0    12661 2024-04-12 12:19:28.613327 rio_ui-0.5.7/rio/cli/project_setup.py
--rw-r--r--   0        0        0     4172 2024-04-08 18:37:44.152450 rio_ui-0.5.7/rio/cli/rio_api.py
--rw-r--r--   0        0        0     2278 2024-04-08 18:37:44.152450 rio_ui-0.5.7/rio/cli/rioignore.py
--rw-r--r--   0        0        0       40 2024-04-14 14:22:40.220263 rio_ui-0.5.7/rio/cli/run_project/__init__.py
--rw-r--r--   0        0        0     5404 2024-04-08 16:50:31.798904 rio_ui-0.5.7/rio/cli/run_project/app_loading.py
--rw-r--r--   0        0        0    20827 2024-04-12 12:19:28.613327 rio_ui-0.5.7/rio/cli/run_project/arbiter.py
--rw-r--r--   0        0        0     1656 2024-04-06 18:09:28.108340 rio_ui-0.5.7/rio/cli/run_project/file_watcher_worker.py
--rw-r--r--   0        0        0      423 2024-04-06 18:09:28.108340 rio_ui-0.5.7/rio/cli/run_project/run_models.py
--rw-r--r--   0        0        0      476 2024-04-08 18:37:44.152450 rio_ui-0.5.7/rio/cli/run_project/run_utils.py
--rw-r--r--   0        0        0     3828 2024-04-12 10:18:09.239288 rio_ui-0.5.7/rio/cli/run_project/uvicorn_worker.py
--rw-r--r--   0        0        0     2229 2024-04-06 18:09:28.108340 rio_ui-0.5.7/rio/cli/run_project/webview_worker.py
--rw-r--r--   0        0        0     3982 2024-04-08 18:37:44.152450 rio_ui-0.5.7/rio/cli/tomlconfig.py
--rw-r--r--   0        0        0    19604 2024-04-09 19:38:54.559018 rio_ui-0.5.7/rio/color.py
--rw-r--r--   0        0        0     7924 2024-04-12 12:19:28.613327 rio_ui-0.5.7/rio/common.py
--rw-r--r--   0        0        0     1552 2024-04-10 18:34:30.899371 rio_ui-0.5.7/rio/components/__init__.py
--rw-r--r--   0        0        0     4469 2024-04-12 12:17:57.040111 rio_ui-0.5.7/rio/components/app_root.py
--rw-r--r--   0        0        0     4055 2024-04-08 18:37:44.152450 rio_ui-0.5.7/rio/components/auto_form.py
--rw-r--r--   0        0        0     4751 2024-04-09 19:38:54.559018 rio_ui-0.5.7/rio/components/banner.py
--rw-r--r--   0        0        0      889 2024-04-07 08:57:25.524848 rio_ui-0.5.7/rio/components/build_failed.py
--rw-r--r--   0        0        0    13570 2024-04-12 20:47:24.392283 rio_ui-0.5.7/rio/components/button.py
--rw-r--r--   0        0        0     5064 2024-04-09 19:38:54.559018 rio_ui-0.5.7/rio/components/card.py
--rw-r--r--   0        0        0     1025 2024-04-06 18:09:28.108340 rio_ui-0.5.7/rio/components/class_container.py
--rw-r--r--   0        0        0      352 2024-04-06 18:09:28.108340 rio_ui-0.5.7/rio/components/code_explorer.py
--rw-r--r--   0        0        0     3745 2024-04-09 19:38:54.559018 rio_ui-0.5.7/rio/components/color_picker.py
--rw-r--r--   0        0        0    26039 2024-04-12 12:19:28.613327 rio_ui-0.5.7/rio/components/component.py
--rw-r--r--   0        0        0     1029 2024-04-06 18:09:28.108340 rio_ui-0.5.7/rio/components/component_tree.py
--rw-r--r--   0        0        0     1225 2024-04-09 19:38:54.562351 rio_ui-0.5.7/rio/components/container.py
--rw-r--r--   0        0        0      215 2024-04-06 18:09:28.108340 rio_ui-0.5.7/rio/components/debugger_connector.py
--rw-r--r--   0        0        0     4067 2024-04-06 18:09:28.108340 rio_ui-0.5.7/rio/components/devel_component.py
--rw-r--r--   0        0        0     3889 2024-04-09 19:38:54.562351 rio_ui-0.5.7/rio/components/drawer.py
--rw-r--r--   0        0        0     6670 2024-04-09 19:38:54.562351 rio_ui-0.5.7/rio/components/dropdown.py
--rw-r--r--   0        0        0     2922 2024-04-09 19:38:54.562351 rio_ui-0.5.7/rio/components/flow_container.py
--rw-r--r--   0        0        0     5867 2024-04-10 17:00:38.844482 rio_ui-0.5.7/rio/components/fundamental_component.py
--rw-r--r--   0        0        0     7057 2024-04-09 19:38:54.562351 rio_ui-0.5.7/rio/components/grid.py
--rw-r--r--   0        0        0      604 2024-04-09 19:38:54.562351 rio_ui-0.5.7/rio/components/html.py
--rw-r--r--   0        0        0     7782 2024-04-09 19:38:54.562351 rio_ui-0.5.7/rio/components/icon.py
--rw-r--r--   0        0        0     3676 2024-04-09 19:38:54.562351 rio_ui-0.5.7/rio/components/image.py
--rw-r--r--   0        0        0    13127 2024-04-09 19:38:54.565684 rio_ui-0.5.7/rio/components/key_event_listener.py
--rw-r--r--   0        0        0     2981 2024-04-12 12:17:57.116777 rio_ui-0.5.7/rio/components/labeled_column.py
--rw-r--r--   0        0        0     8968 2024-04-09 19:38:54.585684 rio_ui-0.5.7/rio/components/linear_containers.py
--rw-r--r--   0        0        0     4478 2024-04-09 19:38:54.565684 rio_ui-0.5.7/rio/components/link.py
--rw-r--r--   0        0        0    10184 2024-04-12 12:17:57.146777 rio_ui-0.5.7/rio/components/list_items.py
--rw-r--r--   0        0        0     3527 2024-04-09 19:38:54.565684 rio_ui-0.5.7/rio/components/list_view.py
--rw-r--r--   0        0        0     1389 2024-04-09 19:38:54.565684 rio_ui-0.5.7/rio/components/markdown.py
--rw-r--r--   0        0        0     4917 2024-04-09 19:38:54.565684 rio_ui-0.5.7/rio/components/media_player.py
--rw-r--r--   0        0        0     6919 2024-04-09 19:38:54.565684 rio_ui-0.5.7/rio/components/mouse_event_listener.py
--rw-r--r--   0        0        0     5165 2024-04-09 19:38:54.569018 rio_ui-0.5.7/rio/components/multi_line_text_input.py
--rw-r--r--   0        0        0     1422 2024-04-09 19:38:54.569018 rio_ui-0.5.7/rio/components/node_input.py
--rw-r--r--   0        0        0     1426 2024-04-09 19:38:54.569018 rio_ui-0.5.7/rio/components/node_output.py
--rw-r--r--   0        0        0     8478 2024-04-09 19:38:54.569018 rio_ui-0.5.7/rio/components/number_input.py
--rw-r--r--   0        0        0     2190 2024-04-09 19:38:54.569018 rio_ui-0.5.7/rio/components/overlay.py
--rw-r--r--   0        0        0     5060 2024-04-09 19:38:54.569018 rio_ui-0.5.7/rio/components/page_view.py
--rw-r--r--   0        0        0     4959 2024-04-09 19:38:54.569018 rio_ui-0.5.7/rio/components/plot.py
--rw-r--r--   0        0        0     3280 2024-04-09 19:38:54.569018 rio_ui-0.5.7/rio/components/popup.py
--rw-r--r--   0        0        0      975 2024-04-09 19:38:54.569018 rio_ui-0.5.7/rio/components/progress_bar.py
--rw-r--r--   0        0        0     3560 2024-04-09 19:38:54.569018 rio_ui-0.5.7/rio/components/progress_circle.py
--rw-r--r--   0        0        0     4106 2024-04-09 19:38:54.569018 rio_ui-0.5.7/rio/components/rectangle.py
--rw-r--r--   0        0        0     3688 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/revealer.py
--rw-r--r--   0        0        0     1857 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/components/root_components.py
--rw-r--r--   0        0        0     1889 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/scroll_container.py
--rw-r--r--   0        0        0     1213 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/scroll_target.py
--rw-r--r--   0        0        0     1114 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/separator.py
--rw-r--r--   0        0        0     6120 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/slider.py
--rw-r--r--   0        0        0     3649 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/slideshow.py
--rw-r--r--   0        0        0     1442 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/spacer.py
--rw-r--r--   0        0        0     2762 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/stack.py
--rw-r--r--   0        0        0     3154 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/switch.py
--rw-r--r--   0        0        0      879 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/switcher.py
--rw-r--r--   0        0        0     9237 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/switcher_bar.py
--rw-r--r--   0        0        0     2305 2024-04-09 19:38:54.572351 rio_ui-0.5.7/rio/components/table.py
--rw-r--r--   0        0        0     2018 2024-04-09 19:38:54.575684 rio_ui-0.5.7/rio/components/text.py
--rw-r--r--   0        0        0     5380 2024-04-09 19:38:54.575684 rio_ui-0.5.7/rio/components/text_input.py
--rw-r--r--   0        0        0     1231 2024-04-09 19:38:54.575684 rio_ui-0.5.7/rio/components/theme_context_switcher.py
--rw-r--r--   0        0        0     2861 2024-04-09 19:38:54.575684 rio_ui-0.5.7/rio/components/tooltip.py
--rw-r--r--   0        0        0      633 2024-04-09 19:38:54.575684 rio_ui-0.5.7/rio/components/website.py
--rw-r--r--   0        0        0      123 2024-04-08 18:37:44.152450 rio_ui-0.5.7/rio/cursor_style.py
--rw-r--r--   0        0        0     5840 2024-04-08 18:37:44.152450 rio_ui-0.5.7/rio/dataclass.py
--rw-r--r--   0        0        0       53 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/debug/__init__.py
--rw-r--r--   0        0        0       63 2024-04-14 14:22:40.220263 rio_ui-0.5.7/rio/debug/client_side_debugger/__init__.py
--rw-r--r--   0        0        0    10452 2024-04-14 09:27:29.090615 rio_ui-0.5.7/rio/debug/client_side_debugger/component_details.py
--rw-r--r--   0        0        0     3729 2024-04-14 09:27:29.090615 rio_ui-0.5.7/rio/debug/client_side_debugger/debugger.py
--rw-r--r--   0        0        0      795 2024-04-12 12:17:57.210110 rio_ui-0.5.7/rio/debug/client_side_debugger/deploy_page.py
--rw-r--r--   0        0        0      782 2024-04-12 12:17:57.210110 rio_ui-0.5.7/rio/debug/client_side_debugger/docs_page.py
--rw-r--r--   0        0        0    12359 2024-04-12 12:17:57.423443 rio_ui-0.5.7/rio/debug/client_side_debugger/icons_page.py
--rw-r--r--   0        0        0     2379 2024-04-12 12:17:57.236777 rio_ui-0.5.7/rio/debug/client_side_debugger/project_page.py
--rw-r--r--   0        0        0     2265 2024-04-08 18:37:44.155783 rio_ui-0.5.7/rio/debug/client_side_debugger/sample_icons_grid.py
--rw-r--r--   0        0        0    16597 2024-04-12 12:17:57.400110 rio_ui-0.5.7/rio/debug/client_side_debugger/theme_picker_page.py
--rw-r--r--   0        0        0     1089 2024-04-10 18:34:30.899371 rio_ui-0.5.7/rio/debug/client_side_debugger/tree_page.py
--rw-r--r--   0        0        0     7224 2024-04-08 18:37:44.155783 rio_ui-0.5.7/rio/debug/monkeypatches.py
--rw-r--r--   0        0        0      567 2024-04-08 18:37:44.155783 rio_ui-0.5.7/rio/debug/typing_utils.py
--rw-r--r--   0        0        0    14210 2024-04-12 12:19:28.613327 rio_ui-0.5.7/rio/debug/validator.py
--rw-r--r--   0        0        0       53 2024-04-14 14:22:40.220263 rio_ui-0.5.7/rio/docs/__init__.py
--rw-r--r--   0        0        0     4867 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/docs/custom.py
--rw-r--r--   0        0        0     1124 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/docs/models.py
--rw-r--r--   0        0        0    14587 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/docs/parsers.py
--rw-r--r--   0        0        0      960 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/errors.py
--rw-r--r--   0        0        0     3173 2024-04-08 18:37:44.155783 rio_ui-0.5.7/rio/event.py
--rw-r--r--   0        0        0     6732 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/fills.py
--rw-r--r--   0        0        0   943434 2024-04-14 14:22:51.470276 rio_ui-0.5.7/rio/generated/index.html
--rw-r--r--   0        0        0      897 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/global_state.py
--rw-r--r--   0        0        0     9940 2024-04-07 11:32:34.208243 rio_ui-0.5.7/rio/icon_registry.py
--rw-r--r--   0        0        0     3500 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/inspection.py
--rw-r--r--   0        0        0     3625 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/maybes.py
--rw-r--r--   0        0        0     1577 2024-04-12 20:47:24.392283 rio_ui-0.5.7/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py
--rw-r--r--   0        0        0     1531 2024-04-12 20:47:24.392283 rio_ui-0.5.7/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py
--rw-r--r--   0        0        0      283 2024-04-13 19:40:36.493590 rio_ui-0.5.7/rio/patches_for_3rd_party_stuff/__init__.py
--rw-r--r--   0        0        0     7380 2024-04-09 19:38:54.575684 rio_ui-0.5.7/rio/routing.py
--rw-r--r--   0        0        0      417 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/self_serializing.py
--rw-r--r--   0        0        0     8463 2024-04-06 18:09:28.111674 rio_ui-0.5.7/rio/serialization.py
--rw-r--r--   0        0        0    76913 2024-04-12 20:47:24.392283 rio_ui-0.5.7/rio/session.py
--rw-r--r--   0        0        0     1395 2024-04-06 18:09:28.115007 rio_ui-0.5.7/rio/snippets/README.md
--rw-r--r--   0        0        0    12317 2024-04-14 11:20:42.330273 rio_ui-0.5.7/rio/snippets/__init__.py
--rw-r--r--   0        0        0     1318 2024-04-09 16:47:56.822558 rio_ui-0.5.7/rio/snippets/snippet-files/other-examples/simple_counter_app.py
--rw-r--r--   0        0        0      684 2024-04-06 18:08:52.814883 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/README.md
--rw-r--r--   0        0        0      863 2024-04-14 06:35:30.859117 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/__init__.py
--rw-r--r--   0        0        0      326 2024-04-14 14:22:40.220263 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/__init__.py
--rw-r--r--   0        0        0     1829 2024-04-13 20:00:32.294184 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py
--rw-r--r--   0        0        0     1196 2024-04-08 18:37:44.155783 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py
--rw-r--r--   0        0        0     3728 2024-04-08 18:37:44.155783 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py
--rw-r--r--   0        0        0      517 2024-04-08 18:37:44.159116 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py
--rw-r--r--   0        0        0     2227 2024-04-07 09:24:53.378316 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py
--rw-r--r--   0        0        0      184 2024-04-07 18:38:03.958535 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/meta.json
--rw-r--r--   0        0        0       44 2024-04-14 14:22:40.220263 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/pages/__init__.py
--rw-r--r--   0        0        0     5823 2024-04-10 17:01:52.457775 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py
--rw-r--r--   0        0        0     3344 2024-04-06 18:08:52.814883 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg
--rw-r--r--   0        0        0        0 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md
--rw-r--r--   0        0        0        0 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/__init__.py
--rw-r--r--   0        0        0     7595 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv
--rw-r--r--   0        0        0      156 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/__init__.py
--rw-r--r--   0        0        0     6866 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py
--rw-r--r--   0        0        0     4602 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py
--rw-r--r--   0        0        0     3359 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py
--rw-r--r--   0        0        0      628 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py
--rw-r--r--   0        0        0      226 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/meta.json
--rw-r--r--   0        0        0       59 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/__init__.py
--rw-r--r--   0        0        0     6789 2024-04-14 18:51:40.939394 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py
--rw-r--r--   0        0        0     3586 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg
--rw-r--r--   0        0        0        0 2024-04-06 18:09:28.115007 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Empty/README.md
--rw-r--r--   0        0        0        0 2024-04-07 08:44:19.156096 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Empty/__init__.py
--rw-r--r--   0        0        0       98 2024-04-07 08:04:03.043617 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Empty/meta.json
--rw-r--r--   0        0        0        0 2024-04-06 18:09:28.115007 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Empty/pages/__init__.py
--rw-r--r--   0        0        0      504 2024-04-12 10:18:09.242621 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py
--rw-r--r--   0        0        0     3344 2024-04-06 18:09:28.115007 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg
--rw-r--r--   0        0        0      714 2024-04-12 10:18:09.225955 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/README.md
--rw-r--r--   0        0        0        0 2024-04-10 16:49:08.284483 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/__init__.py
--rw-r--r--   0        0        0       94 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/components/__init__.py
--rw-r--r--   0        0        0     4821 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py
--rw-r--r--   0        0        0     4139 2024-04-12 10:18:09.225955 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py
--rw-r--r--   0        0        0     1685 2024-04-12 10:18:09.225955 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py
--rw-r--r--   0        0        0       55 2024-04-10 18:59:11.048460 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/meta.json
--rw-r--r--   0        0        0       44 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/pages/__init__.py
--rw-r--r--   0        0        0     6969 2024-04-14 09:27:29.083948 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py
--rw-r--r--   0        0        0     3586 2024-04-10 16:49:08.284483 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg
--rw-r--r--   0        0        0      490 2024-04-08 13:25:22.132597 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md
--rw-r--r--   0        0        0        0 2024-04-08 13:21:28.592126 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/__init__.py
--rw-r--r--   0        0        0       34 2024-04-12 12:20:05.616618 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/__init__.py
--rw-r--r--   0        0        0     2049 2024-04-12 12:19:28.609994 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py
--rw-r--r--   0        0        0       92 2024-04-08 13:26:20.426025 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/meta.json
--rw-r--r--   0        0        0       61 2024-04-14 14:22:40.220263 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/__init__.py
--rw-r--r--   0        0        0     4659 2024-04-12 12:19:28.593327 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0     3344 2024-04-08 13:24:10.679136 rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg
--rw-r--r--   0        0        0        0 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/components/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/__init__.py
--rw-r--r--   0        0        0      806 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/__init__.py
--rw-r--r--   0        0        0     1070 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py
--rw-r--r--   0        0        0        0 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/__init__.py
--rw-r--r--   0        0        0      875 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/__init__.py
--rw-r--r--   0        0        0     1070 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py
--rw-r--r--   0        0        0        0 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/__init__.py
--rw-r--r--   0        0        0     2216 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0       34 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/__init__.py
--rw-r--r--   0        0        0     1256 2024-04-12 20:47:24.408950 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py
--rw-r--r--   0        0        0        0 2024-04-12 20:47:24.412283 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/__init__.py
--rw-r--r--   0        0        0     4328 2024-04-12 20:47:24.412283 rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py
--rw-r--r--   0        0        0     8134 2024-04-08 18:37:44.159116 rio_ui-0.5.7/rio/state_properties.py
--rw-r--r--   0        0        0     3077 2024-04-06 18:09:28.115007 rio_ui-0.5.7/rio/text_style.py
--rw-r--r--   0        0        0    19432 2024-04-09 19:38:54.575684 rio_ui-0.5.7/rio/theme.py
--rw-r--r--   0        0        0     5167 2024-04-06 18:09:28.115007 rio_ui-0.5.7/rio/user_settings_module.py
--rw-r--r--   0        0        0     3890 2024-04-06 18:09:28.115007 rio_ui-0.5.7/rio/world_units.py
--rw-r--r--   0        0        0     9774 1970-01-01 00:00:00.000000 rio_ui-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-06 18:09:28.058340 rio_ui-0.5.8/LICENSE.txt
+-rw-r--r--   0        0        0     7536 2024-04-15 19:47:20.290142 rio_ui-0.5.8/README.md
+-rw-r--r--   0        0        0     2441 2024-04-16 20:42:01.961956 rio_ui-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0      731 2024-04-16 20:40:48.375159 rio_ui-0.5.8/rio/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-06 18:09:28.078340 rio_ui-0.5.8/rio/__main__.py
+-rw-r--r--   0        0        0    19313 2024-04-09 19:38:54.555684 rio_ui-0.5.8/rio/app.py
+-rw-r--r--   0        0        0    32193 2024-04-16 20:40:48.375159 rio_ui-0.5.8/rio/app_server.py
+-rw-r--r--   0        0        0      233 2024-04-06 18:09:28.081673 rio_ui-0.5.8/rio/assets/hosted/README.md
+-rw-r--r--   0        0        0   557380 2024-04-06 18:09:28.088340 rio_ui-0.5.8/rio/assets/hosted/fonts/Noto Sans/NotoSans-Bold.ttf
+-rw-r--r--   0        0        0   401608 2024-04-06 18:09:28.091673 rio_ui-0.5.8/rio/assets/hosted/fonts/Noto Sans/NotoSans-BoldItalic.ttf
+-rw-r--r--   0        0        0   403724 2024-04-06 18:09:28.095007 rio_ui-0.5.8/rio/assets/hosted/fonts/Noto Sans/NotoSans-Italic.ttf
+-rw-r--r--   0        0        0   556216 2024-04-06 18:09:28.098340 rio_ui-0.5.8/rio/assets/hosted/fonts/Noto Sans/NotoSans-Regular.ttf
+-rw-r--r--   0        0        0     4449 2024-04-06 18:09:28.098340 rio_ui-0.5.8/rio/assets/hosted/fonts/Noto Sans/OFL.txt
+-rw-r--r--   0        0        0    11560 2024-04-06 18:09:28.101673 rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0        0        0   167336 2024-04-06 18:09:28.101673 rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   171508 2024-04-06 18:09:28.105007 rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   170504 2024-04-06 18:09:28.105007 rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   168260 2024-04-06 18:09:28.105007 rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0    11560 2024-04-06 18:09:28.098340 rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto Mono/LICENSE.txt
+-rw-r--r--   0        0        0    87392 2024-04-06 18:09:28.098340 rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Bold.ttf
+-rw-r--r--   0        0        0    94636 2024-04-06 18:09:28.101673 rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf
+-rw-r--r--   0        0        0    94372 2024-04-06 18:09:28.101673 rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Italic.ttf
+-rw-r--r--   0        0        0    87236 2024-04-06 18:09:28.101673 rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Regular.ttf
+-rw-r--r--   0        0        0    54189 2024-04-08 17:00:05.405088 rio_ui-0.5.8/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png
+-rw-r--r--   0        0        0    31665 2024-04-06 18:09:28.105007 rio_ui-0.5.8/rio/assets/hosted/rio-logos/rio-logo-square.png
+-rw-r--r--   0        0        0  1081400 2024-04-07 20:27:02.369218 rio_ui-0.5.8/rio/assets/icon-sets/material.tar.xz
+-rw-r--r--   0        0        0    14992 2024-04-14 09:27:29.097282 rio_ui-0.5.8/rio/assets/icon-sets/rio.tar.xz
+-rw-r--r--   0        0        0     1096 2024-04-06 18:09:28.108340 rio_ui-0.5.8/rio/assets/icon-sets/styling.tar.xz
+-rw-r--r--   0        0        0     8798 2024-04-12 12:19:28.613327 rio_ui-0.5.8/rio/assets.py
+-rw-r--r--   0        0        0     3316 2024-04-06 18:09:28.108340 rio_ui-0.5.8/rio/byte_serving.py
+-rw-r--r--   0        0        0     7445 2024-04-16 20:40:48.375159 rio_ui-0.5.8/rio/cli/__init__.py
+-rw-r--r--   0        0        0     2392 2024-04-08 18:37:44.152450 rio_ui-0.5.8/rio/cli/cli_instance.py
+-rw-r--r--   0        0        0     6642 2024-04-06 18:09:28.108340 rio_ui-0.5.8/rio/cli/nice_traceback.py
+-rw-r--r--   0        0        0    13832 2024-04-12 10:18:09.239288 rio_ui-0.5.8/rio/cli/project.py
+-rw-r--r--   0        0        0    12661 2024-04-15 19:46:56.423852 rio_ui-0.5.8/rio/cli/project_setup.py
+-rw-r--r--   0        0        0     4172 2024-04-08 18:37:44.152450 rio_ui-0.5.8/rio/cli/rio_api.py
+-rw-r--r--   0        0        0     2278 2024-04-08 18:37:44.152450 rio_ui-0.5.8/rio/cli/rioignore.py
+-rw-r--r--   0        0        0       40 2024-04-14 14:22:40.220263 rio_ui-0.5.8/rio/cli/run_project/__init__.py
+-rw-r--r--   0        0        0     5404 2024-04-08 16:50:31.798904 rio_ui-0.5.8/rio/cli/run_project/app_loading.py
+-rw-r--r--   0        0        0    22196 2024-04-16 20:40:48.375159 rio_ui-0.5.8/rio/cli/run_project/arbiter.py
+-rw-r--r--   0        0        0     1656 2024-04-06 18:09:28.108340 rio_ui-0.5.8/rio/cli/run_project/file_watcher_worker.py
+-rw-r--r--   0        0        0      423 2024-04-06 18:09:28.108340 rio_ui-0.5.8/rio/cli/run_project/run_models.py
+-rw-r--r--   0        0        0      476 2024-04-08 18:37:44.152450 rio_ui-0.5.8/rio/cli/run_project/run_utils.py
+-rw-r--r--   0        0        0     4097 2024-04-16 20:40:48.375159 rio_ui-0.5.8/rio/cli/run_project/uvicorn_worker.py
+-rw-r--r--   0        0        0     2229 2024-04-06 18:09:28.108340 rio_ui-0.5.8/rio/cli/run_project/webview_worker.py
+-rw-r--r--   0        0        0     3982 2024-04-08 18:37:44.152450 rio_ui-0.5.8/rio/cli/tomlconfig.py
+-rw-r--r--   0        0        0    19604 2024-04-09 19:38:54.559018 rio_ui-0.5.8/rio/color.py
+-rw-r--r--   0        0        0     9824 2024-04-16 20:40:48.378492 rio_ui-0.5.8/rio/common.py
+-rw-r--r--   0        0        0     1552 2024-04-10 18:34:30.899371 rio_ui-0.5.8/rio/components/__init__.py
+-rw-r--r--   0        0        0     4469 2024-04-12 12:17:57.040111 rio_ui-0.5.8/rio/components/app_root.py
+-rw-r--r--   0        0        0     4055 2024-04-08 18:37:44.152450 rio_ui-0.5.8/rio/components/auto_form.py
+-rw-r--r--   0        0        0     4751 2024-04-09 19:38:54.559018 rio_ui-0.5.8/rio/components/banner.py
+-rw-r--r--   0        0        0      889 2024-04-07 08:57:25.524848 rio_ui-0.5.8/rio/components/build_failed.py
+-rw-r--r--   0        0        0    13570 2024-04-12 20:47:24.392283 rio_ui-0.5.8/rio/components/button.py
+-rw-r--r--   0        0        0     5064 2024-04-09 19:38:54.559018 rio_ui-0.5.8/rio/components/card.py
+-rw-r--r--   0        0        0     1025 2024-04-06 18:09:28.108340 rio_ui-0.5.8/rio/components/class_container.py
+-rw-r--r--   0        0        0      352 2024-04-06 18:09:28.108340 rio_ui-0.5.8/rio/components/code_explorer.py
+-rw-r--r--   0        0        0     3745 2024-04-09 19:38:54.559018 rio_ui-0.5.8/rio/components/color_picker.py
+-rw-r--r--   0        0        0    26039 2024-04-12 12:19:28.613327 rio_ui-0.5.8/rio/components/component.py
+-rw-r--r--   0        0        0     1029 2024-04-06 18:09:28.108340 rio_ui-0.5.8/rio/components/component_tree.py
+-rw-r--r--   0        0        0     1225 2024-04-09 19:38:54.562351 rio_ui-0.5.8/rio/components/container.py
+-rw-r--r--   0        0        0      215 2024-04-06 18:09:28.108340 rio_ui-0.5.8/rio/components/debugger_connector.py
+-rw-r--r--   0        0        0     4067 2024-04-06 18:09:28.108340 rio_ui-0.5.8/rio/components/devel_component.py
+-rw-r--r--   0        0        0     3889 2024-04-09 19:38:54.562351 rio_ui-0.5.8/rio/components/drawer.py
+-rw-r--r--   0        0        0     6670 2024-04-09 19:38:54.562351 rio_ui-0.5.8/rio/components/dropdown.py
+-rw-r--r--   0        0        0     2922 2024-04-09 19:38:54.562351 rio_ui-0.5.8/rio/components/flow_container.py
+-rw-r--r--   0        0        0     5867 2024-04-10 17:00:38.844482 rio_ui-0.5.8/rio/components/fundamental_component.py
+-rw-r--r--   0        0        0     7057 2024-04-09 19:38:54.562351 rio_ui-0.5.8/rio/components/grid.py
+-rw-r--r--   0        0        0      604 2024-04-09 19:38:54.562351 rio_ui-0.5.8/rio/components/html.py
+-rw-r--r--   0        0        0     7782 2024-04-09 19:38:54.562351 rio_ui-0.5.8/rio/components/icon.py
+-rw-r--r--   0        0        0     3676 2024-04-09 19:38:54.562351 rio_ui-0.5.8/rio/components/image.py
+-rw-r--r--   0        0        0    13127 2024-04-09 19:38:54.565684 rio_ui-0.5.8/rio/components/key_event_listener.py
+-rw-r--r--   0        0        0     2981 2024-04-12 12:17:57.116777 rio_ui-0.5.8/rio/components/labeled_column.py
+-rw-r--r--   0        0        0     8968 2024-04-09 19:38:54.585684 rio_ui-0.5.8/rio/components/linear_containers.py
+-rw-r--r--   0        0        0     4478 2024-04-09 19:38:54.565684 rio_ui-0.5.8/rio/components/link.py
+-rw-r--r--   0        0        0    10184 2024-04-12 12:17:57.146777 rio_ui-0.5.8/rio/components/list_items.py
+-rw-r--r--   0        0        0     3527 2024-04-09 19:38:54.565684 rio_ui-0.5.8/rio/components/list_view.py
+-rw-r--r--   0        0        0     1389 2024-04-09 19:38:54.565684 rio_ui-0.5.8/rio/components/markdown.py
+-rw-r--r--   0        0        0     4917 2024-04-09 19:38:54.565684 rio_ui-0.5.8/rio/components/media_player.py
+-rw-r--r--   0        0        0     6919 2024-04-09 19:38:54.565684 rio_ui-0.5.8/rio/components/mouse_event_listener.py
+-rw-r--r--   0        0        0     5165 2024-04-09 19:38:54.569018 rio_ui-0.5.8/rio/components/multi_line_text_input.py
+-rw-r--r--   0        0        0     1422 2024-04-09 19:38:54.569018 rio_ui-0.5.8/rio/components/node_input.py
+-rw-r--r--   0        0        0     1426 2024-04-09 19:38:54.569018 rio_ui-0.5.8/rio/components/node_output.py
+-rw-r--r--   0        0        0     8478 2024-04-09 19:38:54.569018 rio_ui-0.5.8/rio/components/number_input.py
+-rw-r--r--   0        0        0     2190 2024-04-09 19:38:54.569018 rio_ui-0.5.8/rio/components/overlay.py
+-rw-r--r--   0        0        0     5116 2024-04-16 20:40:48.378492 rio_ui-0.5.8/rio/components/page_view.py
+-rw-r--r--   0        0        0     4959 2024-04-09 19:38:54.569018 rio_ui-0.5.8/rio/components/plot.py
+-rw-r--r--   0        0        0     3280 2024-04-09 19:38:54.569018 rio_ui-0.5.8/rio/components/popup.py
+-rw-r--r--   0        0        0      975 2024-04-09 19:38:54.569018 rio_ui-0.5.8/rio/components/progress_bar.py
+-rw-r--r--   0        0        0     3560 2024-04-09 19:38:54.569018 rio_ui-0.5.8/rio/components/progress_circle.py
+-rw-r--r--   0        0        0     4106 2024-04-09 19:38:54.569018 rio_ui-0.5.8/rio/components/rectangle.py
+-rw-r--r--   0        0        0     3688 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/revealer.py
+-rw-r--r--   0        0        0     1914 2024-04-16 20:40:48.378492 rio_ui-0.5.8/rio/components/root_components.py
+-rw-r--r--   0        0        0     1889 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/scroll_container.py
+-rw-r--r--   0        0        0     1213 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/scroll_target.py
+-rw-r--r--   0        0        0     1114 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/separator.py
+-rw-r--r--   0        0        0     6120 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/slider.py
+-rw-r--r--   0        0        0     3649 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/slideshow.py
+-rw-r--r--   0        0        0     1442 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/spacer.py
+-rw-r--r--   0        0        0     2762 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/stack.py
+-rw-r--r--   0        0        0     3154 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/switch.py
+-rw-r--r--   0        0        0      879 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/switcher.py
+-rw-r--r--   0        0        0     9237 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/switcher_bar.py
+-rw-r--r--   0        0        0     2305 2024-04-09 19:38:54.572351 rio_ui-0.5.8/rio/components/table.py
+-rw-r--r--   0        0        0     2018 2024-04-09 19:38:54.575684 rio_ui-0.5.8/rio/components/text.py
+-rw-r--r--   0        0        0     5380 2024-04-09 19:38:54.575684 rio_ui-0.5.8/rio/components/text_input.py
+-rw-r--r--   0        0        0     1231 2024-04-09 19:38:54.575684 rio_ui-0.5.8/rio/components/theme_context_switcher.py
+-rw-r--r--   0        0        0     2861 2024-04-09 19:38:54.575684 rio_ui-0.5.8/rio/components/tooltip.py
+-rw-r--r--   0        0        0      633 2024-04-09 19:38:54.575684 rio_ui-0.5.8/rio/components/website.py
+-rw-r--r--   0        0        0      123 2024-04-08 18:37:44.152450 rio_ui-0.5.8/rio/cursor_style.py
+-rw-r--r--   0        0        0     5753 2024-04-15 19:47:20.290142 rio_ui-0.5.8/rio/dataclass.py
+-rw-r--r--   0        0        0       53 2024-04-06 18:09:28.111674 rio_ui-0.5.8/rio/debug/__init__.py
+-rw-r--r--   0        0        0       63 2024-04-14 14:22:40.220263 rio_ui-0.5.8/rio/debug/client_side_debugger/__init__.py
+-rw-r--r--   0        0        0    10723 2024-04-15 19:47:20.300142 rio_ui-0.5.8/rio/debug/client_side_debugger/component_details.py
+-rw-r--r--   0        0        0     3589 2024-04-15 19:47:20.300142 rio_ui-0.5.8/rio/debug/client_side_debugger/debugger.py
+-rw-r--r--   0        0        0      795 2024-04-12 12:17:57.210110 rio_ui-0.5.8/rio/debug/client_side_debugger/deploy_page.py
+-rw-r--r--   0        0        0      782 2024-04-12 12:17:57.210110 rio_ui-0.5.8/rio/debug/client_side_debugger/docs_page.py
+-rw-r--r--   0        0        0    12359 2024-04-12 12:17:57.423443 rio_ui-0.5.8/rio/debug/client_side_debugger/icons_page.py
+-rw-r--r--   0        0        0     1055 2024-04-15 19:47:20.300142 rio_ui-0.5.8/rio/debug/client_side_debugger/layout_preview.py
+-rw-r--r--   0        0        0     2379 2024-04-12 12:17:57.236777 rio_ui-0.5.8/rio/debug/client_side_debugger/project_page.py
+-rw-r--r--   0        0        0     2265 2024-04-08 18:37:44.155783 rio_ui-0.5.8/rio/debug/client_side_debugger/sample_icons_grid.py
+-rw-r--r--   0        0        0    16597 2024-04-12 12:17:57.400110 rio_ui-0.5.8/rio/debug/client_side_debugger/theme_picker_page.py
+-rw-r--r--   0        0        0     1089 2024-04-10 18:34:30.899371 rio_ui-0.5.8/rio/debug/client_side_debugger/tree_page.py
+-rw-r--r--   0        0        0     7224 2024-04-08 18:37:44.155783 rio_ui-0.5.8/rio/debug/monkeypatches.py
+-rw-r--r--   0        0        0      567 2024-04-08 18:37:44.155783 rio_ui-0.5.8/rio/debug/typing_utils.py
+-rw-r--r--   0        0        0    14210 2024-04-12 12:19:28.613327 rio_ui-0.5.8/rio/debug/validator.py
+-rw-r--r--   0        0        0       31 2024-04-16 20:40:48.378492 rio_ui-0.5.8/rio/docs/__init__.py
+-rw-r--r--   0        0        0     4884 2024-04-16 20:40:48.378492 rio_ui-0.5.8/rio/docs/custom.py
+-rw-r--r--   0        0        0      960 2024-04-06 18:09:28.111674 rio_ui-0.5.8/rio/errors.py
+-rw-r--r--   0        0        0     3173 2024-04-08 18:37:44.155783 rio_ui-0.5.8/rio/event.py
+-rw-r--r--   0        0        0     6732 2024-04-06 18:09:28.111674 rio_ui-0.5.8/rio/fills.py
+-rw-r--r--   0        0        0   529611 2024-04-16 20:44:03.208838 rio_ui-0.5.8/rio/generated/index.html
+-rw-r--r--   0        0        0      897 2024-04-06 18:09:28.111674 rio_ui-0.5.8/rio/global_state.py
+-rw-r--r--   0        0        0     9940 2024-04-07 11:32:34.208243 rio_ui-0.5.8/rio/icon_registry.py
+-rw-r--r--   0        0        0     3500 2024-04-06 18:09:28.111674 rio_ui-0.5.8/rio/inspection.py
+-rw-r--r--   0        0        0     3625 2024-04-06 18:09:28.111674 rio_ui-0.5.8/rio/maybes.py
+-rw-r--r--   0        0        0     1577 2024-04-12 20:47:24.392283 rio_ui-0.5.8/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py
+-rw-r--r--   0        0        0     1531 2024-04-12 20:47:24.392283 rio_ui-0.5.8/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py
+-rw-r--r--   0        0        0      757 2024-04-15 19:47:20.290142 rio_ui-0.5.8/rio/patches_for_3rd_party_stuff/_OverlappedFuture_cancel_overlapped.py
+-rw-r--r--   0        0        0      374 2024-04-15 19:47:20.290142 rio_ui-0.5.8/rio/patches_for_3rd_party_stuff/__init__.py
+-rw-r--r--   0        0        0     7380 2024-04-09 19:38:54.575684 rio_ui-0.5.8/rio/routing.py
+-rw-r--r--   0        0        0      417 2024-04-06 18:09:28.111674 rio_ui-0.5.8/rio/self_serializing.py
+-rw-r--r--   0        0        0     8463 2024-04-06 18:09:28.111674 rio_ui-0.5.8/rio/serialization.py
+-rw-r--r--   0        0        0    75851 2024-04-16 20:40:48.378492 rio_ui-0.5.8/rio/session.py
+-rw-r--r--   0        0        0     1395 2024-04-06 18:09:28.115007 rio_ui-0.5.8/rio/snippets/README.md
+-rw-r--r--   0        0        0    12479 2024-04-15 19:47:20.300142 rio_ui-0.5.8/rio/snippets/__init__.py
+-rw-r--r--   0        0        0     1318 2024-04-09 16:47:56.822558 rio_ui-0.5.8/rio/snippets/snippet-files/other-examples/simple_counter_app.py
+-rw-r--r--   0        0        0      684 2024-04-06 18:08:52.814883 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/README.md
+-rw-r--r--   0        0        0      326 2024-04-14 14:22:40.220263 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/components/__init__.py
+-rw-r--r--   0        0        0     1829 2024-04-13 20:00:32.294184 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py
+-rw-r--r--   0        0        0     1196 2024-04-08 18:37:44.155783 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py
+-rw-r--r--   0        0        0     3728 2024-04-08 18:37:44.155783 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py
+-rw-r--r--   0        0        0      517 2024-04-08 18:37:44.159116 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py
+-rw-r--r--   0        0        0     2227 2024-04-07 09:24:53.378316 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py
+-rw-r--r--   0        0        0      184 2024-04-07 18:38:03.958535 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/meta.json
+-rw-r--r--   0        0        0       44 2024-04-14 14:22:40.220263 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/pages/__init__.py
+-rw-r--r--   0        0        0     5823 2024-04-10 17:01:52.457775 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py
+-rw-r--r--   0        0        0      863 2024-04-15 19:47:20.300142 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py
+-rw-r--r--   0        0        0     3344 2024-04-06 18:08:52.814883 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg
+-rw-r--r--   0        0        0        0 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/README.md
+-rw-r--r--   0        0        0     7595 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv
+-rw-r--r--   0        0        0      156 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/__init__.py
+-rw-r--r--   0        0        0     6866 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py
+-rw-r--r--   0        0        0     4602 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py
+-rw-r--r--   0        0        0     3359 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py
+-rw-r--r--   0        0        0      628 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py
+-rw-r--r--   0        0        0      226 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/meta.json
+-rw-r--r--   0        0        0       59 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/__init__.py
+-rw-r--r--   0        0        0     6789 2024-04-15 19:47:20.300142 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:47:20.300142 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/root_init.py
+-rw-r--r--   0        0        0     3586 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg
+-rw-r--r--   0        0        0        0 2024-04-06 18:09:28.115007 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Empty/README.md
+-rw-r--r--   0        0        0       98 2024-04-07 08:04:03.043617 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Empty/meta.json
+-rw-r--r--   0        0        0        0 2024-04-06 18:09:28.115007 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Empty/pages/__init__.py
+-rw-r--r--   0        0        0      504 2024-04-12 10:18:09.242621 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Empty/pages/sample_page.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:47:20.300142 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Empty/root_init.py
+-rw-r--r--   0        0        0     3344 2024-04-06 18:09:28.115007 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg
+-rw-r--r--   0        0        0      714 2024-04-12 10:18:09.225955 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/README.md
+-rw-r--r--   0        0        0       94 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/components/__init__.py
+-rw-r--r--   0        0        0     4821 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py
+-rw-r--r--   0        0        0     4139 2024-04-12 10:18:09.225955 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py
+-rw-r--r--   0        0        0     1685 2024-04-12 10:18:09.225955 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py
+-rw-r--r--   0        0        0       55 2024-04-10 18:59:11.048460 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/meta.json
+-rw-r--r--   0        0        0       44 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/pages/__init__.py
+-rw-r--r--   0        0        0     6969 2024-04-14 09:27:29.083948 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:47:20.300142 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/root_init.py
+-rw-r--r--   0        0        0     3586 2024-04-10 16:49:08.284483 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg
+-rw-r--r--   0        0        0      490 2024-04-08 13:25:22.132597 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/README.md
+-rw-r--r--   0        0        0       34 2024-04-12 12:20:05.616618 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/__init__.py
+-rw-r--r--   0        0        0     2049 2024-04-12 12:19:28.609994 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py
+-rw-r--r--   0        0        0       92 2024-04-08 13:26:20.426025 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/meta.json
+-rw-r--r--   0        0        0       61 2024-04-14 14:22:40.220263 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/__init__.py
+-rw-r--r--   0        0        0     4659 2024-04-12 12:19:28.593327 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0        0 2024-04-15 19:47:20.300142 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/root_init.py
+-rw-r--r--   0        0        0     3344 2024-04-08 13:24:10.679136 rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg
+-rw-r--r--   0        0        0        0 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/components/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/__init__.py
+-rw-r--r--   0        0        0      806 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/__init__.py
+-rw-r--r--   0        0        0     1070 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py
+-rw-r--r--   0        0        0        0 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/__init__.py
+-rw-r--r--   0        0        0      875 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/__init__.py
+-rw-r--r--   0        0        0     1070 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py
+-rw-r--r--   0        0        0        0 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/__init__.py
+-rw-r--r--   0        0        0     2216 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0       34 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/__init__.py
+-rw-r--r--   0        0        0     1256 2024-04-12 20:47:24.408950 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py
+-rw-r--r--   0        0        0        0 2024-04-12 20:47:24.412283 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/__init__.py
+-rw-r--r--   0        0        0     4328 2024-04-12 20:47:24.412283 rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py
+-rw-r--r--   0        0        0     8134 2024-04-08 18:37:44.159116 rio_ui-0.5.8/rio/state_properties.py
+-rw-r--r--   0        0        0     3077 2024-04-06 18:09:28.115007 rio_ui-0.5.8/rio/text_style.py
+-rw-r--r--   0        0        0    19432 2024-04-09 19:38:54.575684 rio_ui-0.5.8/rio/theme.py
+-rw-r--r--   0        0        0     5167 2024-04-06 18:09:28.115007 rio_ui-0.5.8/rio/user_settings_module.py
+-rw-r--r--   0        0        0     3890 2024-04-06 18:09:28.115007 rio_ui-0.5.8/rio/world_units.py
+-rw-r--r--   0        0        0    10093 1970-01-01 00:00:00.000000 rio_ui-0.5.8/PKG-INFO
```

### Comparing `rio_ui-0.5.7/LICENSE.txt` & `rio_ui-0.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/README.md` & `rio_ui-0.5.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 ![Rio](https://img.shields.io/badge/Rio-outline.svg?color=%2311e8e3e&link=https%3A%2F%2Frio.dev&style=flat-square&logo=data:image/svg%2bxml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjxzdmcKICAgd2lkdGg9IjEwMDIuMTA1IgogICBoZWlnaHQ9IjE0OTkuODA1NyIKICAgdmlld0JveD0iMCAwIDI2NS4xNDAyOSAzOTYuODIzNTkiCiAgIHZlcnNpb249IjEuMSIKICAgaWQ9InN2Zzg5NiIKICAgeG1sOnNwYWNlPSJwcmVzZXJ2ZSIKICAgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIgogICB4bWxuczpzdmc9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIgogICB4bWxuczpyZGY9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkvMDIvMjItcmRmLXN5bnRheC1ucyMiCiAgIHhtbG5zOmNjPSJodHRwOi8vY3JlYXRpdmVjb21tb25zLm9yZy9ucyMiCiAgIHhtbG5zOmRjPSJodHRwOi8vcHVybC5vcmcvZGMvZWxlbWVudHMvMS4xLyI+PGRlZnMKICAgICBpZD0iZGVmczg5MCIgLz48bWV0YWRhdGEKICAgICBpZD0ibWV0YWRhdGE4OTMiPjxyZGY6UkRGPjxjYzpXb3JrCiAgICAgICAgIHJkZjphYm91dD0iIj48ZGM6Zm9ybWF0PmltYWdlL3N2Zyt4bWw8L2RjOmZvcm1hdD48ZGM6dHlwZQogICAgICAgICAgIHJkZjpyZXNvdXJjZT0iaHR0cDovL3B1cmwub3JnL2RjL2RjbWl0eXBlL1N0aWxsSW1hZ2UiIC8+PC9jYzpXb3JrPjwvcmRmOlJERj48L21ldGFkYXRhPjxnCiAgICAgaWQ9ImxheWVyMSIKICAgICB0cmFuc2Zvcm09InRyYW5zbGF0ZSgyNi40MTM4NDcsNTAuMjcxMzUpIj48cGF0aAogICAgICAgaWQ9InBhdGgxIgogICAgICAgc3R5bGU9ImZpbGw6I2ZmZmZmZjtmaWxsLW9wYWNpdHk6MTtzdHJva2Utd2lkdGg6MC4yNjQ1ODMiCiAgICAgICBkPSJtIC04LjgwMzA4MDMsLTUwLjI3MTM1IGMgLTE1LjI3NjU1OTcsMC44NjA1MjQgLTE4LjYzMTgzNDcsMTcuNTQ0NTEyIC0xNy4zNjc0MTU3LDI5Ljk2ODk1MiAwLjUxMzcyNywxNi4yNDQxNjYxIC0xLjIxMzE5NywzMi43MTkyOTcgMS4yNjg1MTcsNDguNzY2NzkzIDguMTQxMTg1LDE0LjcxMDAxMiAyNi4wNzc2NzYxLDE4Ljg0OTk3MiAzOS44Nzc0ODIsMjYuNzcwMTM0IDMwLjM3ODk2MiwxNS4wNjY1NSA2MC43NTc5MjUsMzAuMTMzMTAxIDkxLjEzNjg4Nyw0NS4xOTk2NTEgLTM0LjgyMjM5OCwxNy42MDY2OCAtNzAuMjI2MTE3LDM0LjE0NzgzIC0xMDQuNjYwNTA2OCw1Mi40NjUyOCAtMjAuMDM3Nzc1MiwxMS40ODE0NCAtMzQuNzc4MTg3MiwzNi45NjY5OCAtMjQuMTAxMTk2Miw1OS41OTIxMSAxMS4yOTkzMSwyNS42MDQ3IDM5Ljc0MjkxMSwzMy43MTY5NSA2Mi40NzIyMDgsNDUuOTY4MDIgNTguOTU5MTAzLDI5LjA5NDExIDExNy43MTA1MzUsNTguNjQ4NDIgMTc2Ljc4OTE1NSw4Ny40NzU2IDE0LjA2MTIxLDMuOTY4MzYgMjQuMDM2NzYsLTEyLjAyMzEgMjEuODAwNzksLTI0LjUzMjIgLTAuNTQyODUsLTE3LjgzMTU3IDEuMjU4MTYsLTM1LjkwMjkyIC0xLjI2ODM2LC01My41MzY0OCAtOC4xNDA2MywtMTQuNzEwNzEgLTI2LjA3NjkyLC0xOC44NTE5OCAtMzkuODc3MTksLTI2Ljc3MTcyIC0zMC4zNzYwNiwtMTUuMDcxMTUgLTYwLjgwMDczLC0zMC4xNDExNyAtOTEuMTQ2NDIsLTQ1LjIxMzA0IDM0LjUwODc5LC0xNy4zNzM3NyA2OS40NTU5NywtMzMuOTI1NjUgMTAzLjY3Mjk4LC01MS44NDY2MyAyMC4xOTUxMywtMTEuMDA2MjggMzUuMzg2NDQsLTM2LjMwMDA1IDI1LjYwMzM4LC01OC45ODA5NCBDIDIyNC43MDYyMyw1OC44NzI1MzQgMTk2LjA1MDY3LDUwLjQ4NjY0MSAxNzMuMTY3MjYsMzguMjM4MTkxIDE1MS4xOTIyNiwyNy4zNDkyOTUgMTI2LjI0NjM5LDE0LjkzOTYzOCAxMDYuMTIxMTcsNC45OTc2Mjc4IDcwLjA0MTcxOSwtMTIuODk5Mjk5IDMzLjk2MjI2OCwtMzAuNzk2MjI1IC0yLjExNzE4MzQsLTQ4LjY5MzE1MiBsIC0zLjM3MjY3NzcsLTEuMjE4NDkyIHoiIC8+PC9nPjwvc3ZnPgo=)
+![Version](https://img.shields.io/pypi/v/rio-ui?color=%2311e8e3e&style=flat-square)
 ![Discord](https://img.shields.io/discord/1213589765484576818?color=%2311e8e3e&label=discord&style=flat-square)
 ![Python Version](https://img.shields.io/pypi/pyversions/rio-ui?style=flat-square)
-![Version](https://img.shields.io/pypi/v/rio-ui?color=%2311e8e3e&style=flat-square)
 ![License](https://img.shields.io/pypi/l/rio-ui?color=%2311e8e3e&style=flat-square)
-
-<!-- TODO: Gitlab Stars -->
+![GitHub Stars](https://img.shields.io/github/stars/rio-labs/rio?style=flat-square)
 
 <!-- https://shields.io/badges -->
 
-<img src="https://gitlab.com/team-rio/rio/-/raw/dev/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png" alt="Rio Logo" style="width: 30rem" />
+<img src="https://github.com/rio-labs/rio/blob/dev/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png?raw=true" alt="Rio Logo" style="width: 16rem" />
 
 🌊 You've arrived at **Rio**, an easy to use framework for creating websites and
 apps.
 
 🐍 Rio is based **entirely on Python**. You **won't need a single line of HTML, CSS, or
 JavaScript** to create beautiful, modern apps.
 
-[Tutorial](https://rio.dev/get-started) - [Examples](https://rio.dev/examples) - [Discord](https://discord.gg/7ejXaPwhyH) - [Docs](https://rio.dev/docs) - [Source Code](https://gitlab.com/team-rio/rio)
+[Tutorial](https://rio.dev/get-started) - [Examples](https://rio.dev/examples) - [Discord](https://discord.gg/7ejXaPwhyH) - [Docs](https://rio.dev/docs) - [Source Code](https://github.com/rio-labs/rio)
 
 Rio brings React-style components to Python. Pull from a wealth of built-in
 components and combine them to create your own custom components. Then combine
 those into entire apps. Best of all, Rio apps can run both locally on your
 machine and on the web.
 
 ## Features 🧩
 
--   Modern, **declarative UI** framework
--   **100% Python** - Zero HTML, CSS, or JavaScript required
--   Over **50 Built-in components** for common UI elements, such as `rio.Switch`, `rio.Button`, and `rio.Text`, and many more
--   Integrates with **modern Python tooling**: Thanks to being **entirely Type Safe** editors can give you instant suggestions and highlight problems right away
--   Apps can run **both locally and on the web**
--   **Open Source & Free forever**
+- Modern, **declarative UI** framework
+- **100% Python** - Zero HTML, CSS, or JavaScript required
+- Over **50 Built-in components** for common UI elements, such as `rio.Switch`, `rio.Button`, and `rio.Text`, and many more
+- Integrates with **modern Python tooling**: Thanks to being **entirely Type Safe** editors can give you instant suggestions and highlight problems right away
+- Apps can run **both locally and on the web**
+- **Open Source & Free forever**
 
 ## Installation 🛠️
 
 Rio is available on PyPI, so you can install it using pip:
 
 ```bash
 pip install rio-ui
@@ -143,8 +142,18 @@
     pages=[
         rio.Page(
             page_url="",
             build=DallEPage,
         ),
     ],
 )
+
+## Status: In Development 🚧
+
+Rio is still in development. We're working hard to bring you the best possible
+experience. If you have any feedback, please let us know on our Discord server.
+
+## Contributing 🤝
+
+Write how someone can contribute to the project. :)
+
 ```
```

### Comparing `rio_ui-0.5.7/pyproject.toml` & `rio_ui-0.5.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 license = "LGPL-3.0" # TODO
 name = "rio-ui"
-version = "0.5.7"
+version = "0.5.8"
 description = "Build modern Websites and Apps just with Python"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>", "Paul Pinterits"]
 readme = "README.md"
 packages = [{ include = "rio" }]
 include = ["rio/generated/index.html"]
 keywords = [
     "web-development",
```

### Comparing `rio_ui-0.5.7/rio/__init__.py` & `rio_ui-0.5.8/rio/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+import logging
+
+_logger = logging.getLogger(__name__)
+
 # Re-export dataclass stuff for easy use.
 from dataclasses import KW_ONLY as KW_ONLY
 from dataclasses import field as field
 
 # URLs are used as an important datatype within rio. Re-export them for easy
 # use.
 from yarl import URL as URL
```

### Comparing `rio_ui-0.5.7/rio/app.py` & `rio_ui-0.5.8/rio/app.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/app_server.py` & `rio_ui-0.5.8/rio/app_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         full_url = base_url.with_path(relative_url.path)
 
         url = ET.SubElement(tree, "url")
         loc = ET.SubElement(url, "loc")
         loc.text = str(full_url)
 
     # Done
-    return ET.tostring(tree, encoding="unicode")
+    return ET.tostring(tree, encoding="unicode", xml_declaration=True)
 
 
 @functools.lru_cache(maxsize=None)
 def read_frontend_template(template_name: str) -> str:
     """
     Read a text file from the frontend directory and return its content. The
     results are cached to avoid repeated disk access.
@@ -198,21 +198,23 @@
         )
         self.add_api_route(
             "/rio/upload/{upload_token}", self._serve_file_upload, methods=["PUT"]
         )
         self.add_api_websocket_route("/rio/ws", self._serve_websocket)
 
         # Because this is a single page application, all other routes should
-        # serve the index page. The session will determine which components should
-        # be shown.
+        # serve the index page. The session will determine which components
+        # should be shown.
         self.add_api_route(
             "/{initial_route_str:path}", self._serve_index, methods=["GET"]
         )
 
     async def _call_on_app_start(self) -> None:
+        rio._logger.debug("Calling `on_app_start`")
+
         if self.app._on_app_start is None:
             return
 
         try:
             result = self.app._on_app_start(self.app)
 
             if inspect.isawaitable(result):
@@ -220,14 +222,16 @@
 
         # Display and discard exceptions
         except Exception:
             print("Exception in `on_app_start` event handler:")
             traceback.print_exc()
 
     async def _call_on_app_close(self) -> None:
+        rio._logger.debug("Calling `on_app_close`")
+
         if self.app._on_app_close is None:
             return
 
         try:
             result = self.app._on_app_close(self.app)
 
             if inspect.isawaitable(result):
```

### Comparing `rio_ui-0.5.7/rio/assets/hosted/fonts/Noto Sans/NotoSans-Bold.ttf` & `rio_ui-0.5.8/rio/assets/hosted/fonts/Noto Sans/NotoSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/assets/hosted/fonts/Noto Sans/NotoSans-BoldItalic.ttf` & `rio_ui-0.5.8/rio/assets/hosted/fonts/Noto Sans/NotoSans-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/assets/hosted/fonts/Noto Sans/NotoSans-Italic.ttf` & `rio_ui-0.5.8/rio/assets/hosted/fonts/Noto Sans/NotoSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/assets/hosted/fonts/Noto Sans/NotoSans-Regular.ttf` & `rio_ui-0.5.8/rio/assets/hosted/fonts/Noto Sans/NotoSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/assets/hosted/fonts/Noto Sans/OFL.txt` & `rio_ui-0.5.8/rio/assets/hosted/fonts/Noto Sans/OFL.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto/LICENSE.txt` & `rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto/Roboto-Bold.ttf` & `rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto/Roboto-BoldItalic.ttf` & `rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto/Roboto-Italic.ttf` & `rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto/Roboto-Regular.ttf` & `rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto Mono/LICENSE.txt` & `rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto Mono/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Bold.ttf` & `rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf` & `rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Italic.ttf` & `rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Regular.ttf` & `rio_ui-0.5.8/rio/assets/hosted/fonts/Roboto Mono/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png` & `rio_ui-0.5.8/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/assets/hosted/rio-logos/rio-logo-square.png` & `rio_ui-0.5.8/rio/assets/hosted/rio-logos/rio-logo-square.png`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/assets/icon-sets/material.tar.xz` & `rio_ui-0.5.8/rio/assets/icon-sets/material.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/assets/icon-sets/rio.tar.xz` & `rio_ui-0.5.8/rio/assets/icon-sets/rio.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/assets/icon-sets/styling.tar.xz` & `rio_ui-0.5.8/rio/assets/icon-sets/styling.tar.xz`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/assets.py` & `rio_ui-0.5.8/rio/assets.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/byte_serving.py` & `rio_ui-0.5.8/rio/byte_serving.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/cli/__init__.py` & `rio_ui-0.5.8/rio/cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+import logging
+
+_logger = logging.getLogger(__name__)
+
+
 from typing import Literal
 
 import imy.package_metadata
 import introspection
 import revel
 from revel import *  # type: ignore
```

### Comparing `rio_ui-0.5.7/rio/cli/cli_instance.py` & `rio_ui-0.5.8/rio/cli/cli_instance.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/cli/nice_traceback.py` & `rio_ui-0.5.8/rio/cli/nice_traceback.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/cli/project.py` & `rio_ui-0.5.8/rio/cli/project.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/cli/project_setup.py` & `rio_ui-0.5.8/rio/cli/project_setup.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/cli/rio_api.py` & `rio_ui-0.5.8/rio/cli/rio_api.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/cli/rioignore.py` & `rio_ui-0.5.8/rio/cli/rioignore.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/cli/run_project/app_loading.py` & `rio_ui-0.5.8/rio/cli/run_project/app_loading.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/cli/run_project/arbiter.py` & `rio_ui-0.5.8/rio/cli/run_project/arbiter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-import functools
 import json
 import logging
 import signal
 import socket
 import threading
 import time
 import webbrowser
@@ -124,14 +123,15 @@
         self._mainloop: asyncio.AbstractEventLoop | None = None
 
     def push_event(self, event: run_models.Event) -> None:
         """
         Pushes an event into the event queue. Threadsafe.
         """
         assert self._mainloop is not None, "Can't push events before asyncio is running"
+        rio.cli._logger.debug(f"Pushing arbiter event `{event}`")
         self._mainloop.call_soon_threadsafe(self._event_queue.put_nowait, event)
 
     @property
     def _host(self) -> str:
         return "0.0.0.0" if self.public else "127.0.0.1"
 
     @property
@@ -160,14 +160,16 @@
         Stops the app. This function can safely be called more than once, and at
         any point in time.
         """
         # Already shutting down? Then do nothing
         if not self._stopping_lock.acquire(blocking=False):
             return
 
+        rio.cli._logger.debug("Stopping the app")
+
         # Visualize KeyboardInterrupts
         if keyboard_interrupt:
             print()
             print("[yellow]Interrupted[/]")
         else:
             print("Stopping")
 
@@ -175,55 +177,58 @@
         self._stop_requested.set()
         self._server_is_ready.set()
 
         # Stop any running workers
         assert self._mainloop is not None, "Mainloop isn't running!?"
 
         def cancel_all_tasks() -> None:
+            rio.cli._logger.debug(
+                "Cancelling all arbiter tasks because the app is stopping"
+            )
+
             for task in self.running_tasks:
                 task.cancel()
 
         self._mainloop.call_soon_threadsafe(cancel_all_tasks)
 
         # Stop the webview
         if self._webview_worker is not None:
+            rio.cli._logger.debug("Stopping the webview because the app is stopping")
             self._webview_worker.request_stop()
 
     def try_load_app(self) -> tuple[rio.App, Exception | None]:
         """
         Tries to load the user's app. If it fails, a dummy app is created and
         returned, unless running in release mode.
 
         Returns the new app and the error that occurred, if any.
         """
+        rio.cli._logger.debug("Trying to load the app")
+
         try:
             app = app_loading.load_user_app(self.proj)
 
         except app_loading.AppLoadError as err:
             # If running in release mode, no further attempts to load the app
             # will be made. This error is fatal.
             if not self.debug_mode:
+                rio.cli._logger.critical(f"The app could not be loaded: {err}")
                 revel.fatal(f'The app could not be loaded: "{err}"')
 
             # Otherwise create a placeholder app which displays the error
             # message
             return (
                 app_loading.make_error_message_app(
                     err,
                     self.proj.project_directory,
                     self._app_theme,
                 ),
                 err,
             )
 
-        # If running in debug mode, catch exceptions thrown by the app's `build`
-        # function and display them in the GUI
-        if self.debug_mode:
-            app._build = functools.partial(self._try_build_app, app._build)
-
         # Remember the app's theme. If in the future a placeholder app is used,
         # this theme will be used for it.
         self._app_theme = app._theme
 
         return app, None
 
     def run(self) -> None:
@@ -241,35 +246,41 @@
                 self._run_async(),
             ),
             name="arbiter function of rio run",
         )
         asyncio_thread.start()
 
         # Wait for the http server to be ready
+        rio.cli._logger.debug("Waiting for the http server to be ready")
         self._server_is_ready.wait()
 
         # Make sure the startup was successful
         if self._stop_requested.is_set():
+            rio.cli._logger.debug(
+                "Stopping the arbiter because a stop was requested before the startup sequence has finished"
+            )
             asyncio_thread.join()
             return
 
         # The webview needs to be shown from the main thread. So, if running
         # inside of a window run the arbiter in a separate thread. Otherwise
         # just run it from this one.
         if self.run_in_window:
             self._webview_worker = webview_worker.WebViewWorker(
                 push_event=self.push_event,
                 debug_mode=self.debug_mode,
                 url=self.url,
             )
 
+            rio.cli._logger.debug("Starting the webview worker")
             self._webview_worker.run()
 
         # If not running in a webview, just wait
         else:
+            rio.cli._logger.debug("Opening the browser")
             webbrowser.open(self.url)
 
             # Event.wait() blocks the SIGINT handler, so we must periodically
             # return to python land to react to keyboard interrupts.
             #
             # We could pass a timeout to `_stop_requested.wait()`, but
             # `time.sleep()` reacts to keyboard interrupts immediately, which is
@@ -279,16 +290,19 @@
 
                 if self._stop_requested.is_set():
                     break
 
         # Make sure the main thread stays alive until the asyncio thread is
         # done. Otherwise we get weird errors like "Can't start thread during
         # interpreter shutdown" from asyncio.
+        rio.cli._logger.debug("The arbiter is waiting for the asyncio thread to finish")
         asyncio_thread.join()
 
+        rio.cli._logger.debug("Arbiter shutdown complete")
+
     async def _run_async(self) -> None:
         # Publish the task, so it can be cancelled
         self._arbiter_task = asyncio.current_task()
 
         # Make sure the webview module is available
         if self.run_in_window and webview is None:
             revel.fatal(
@@ -316,29 +330,35 @@
         # Anything else is an unintentional crash
         except Exception as err:
             revel.error("The arbiter has crashed.")
             revel.error("This is a bug in Rio - please report it")
             print()
             revel.print(nice_traceback.format_exception_revel(err))
 
+            rio.cli._logger.exception("The arbiter has crashed")
+
             self.stop(keyboard_interrupt=False)
 
         finally:
             # Wait until all the other tasks are done. If we return, then
             # `asyncio.run` will cancel anything that's still running.
+            rio.cli._logger.debug("Waiting for all arbiter tasks to finish")
+
             for task in self.running_tasks:
                 if task is self._arbiter_task:
                     continue
 
                 try:
                     await task
                 except asyncio.CancelledError:
                     pass
 
             # Then cancel all remaining tasks to ensure the program exits
+            rio.cli._logger.debug("Cancelling all remaining asyncio tasks")
+
             for task in asyncio.all_tasks():
                 if task is self._arbiter_task:
                     continue
 
                 task.cancel()
 
     async def _run_async_inner(self) -> None:
@@ -350,14 +370,16 @@
         print("Starting...")
 
         # Expose the mainloop
         self._mainloop = asyncio.get_running_loop()
 
         # Make sure the chosen port is available
         with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
+            rio.cli._logger.debug(f"Checking if port {self.port} is available")
+
             sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
 
             try:
                 sock.bind((self._host, self.port))
             except OSError:
                 revel.error(f"The port [bold]{self.port}[/] is already in use.")
                 revel.error(f"Each port can only be used by one app at a time.")
@@ -365,14 +387,15 @@
                     f"Try using another port, or let Rio choose one for you, by not specifying any port."
                 )
                 self.stop(keyboard_interrupt=False)
                 return
 
             # If running in debug mode, install safeguards
             if self.debug_mode:
+                rio.cli._logger.debug("Applying monkeypatches")
                 apply_monkeypatches()
 
             # Try to load the app
             app, _ = self.try_load_app()
 
             # Start the file watcher
             if self.debug_mode:
@@ -400,17 +423,19 @@
 
             self._uvicorn_task = asyncio.create_task(
                 self._uvicorn_worker.run(),
                 name="Uvicorn",
             )
 
             # Wait for the server to be ready or fails to start
+            rio.cli._logger.debug("Waiting for uvicorn to be ready or to fail")
             await uvicorn_is_ready_or_has_failed
 
             # Let everyone else know that the server is ready
+            rio.cli._logger.debug("App startup complete and ready for connections")
             self._server_is_ready.set()
 
             # The app has just successfully started. Inform the user
             if self.debug_mode:
                 revel.warning("Debug mode is enabled.")
                 revel.warning(
                     "Debug mode includes helpful tools for development, but is slower and disables some safety checks. Never use it in production!"
@@ -436,14 +461,15 @@
 
             # Keep track when the app was last reloaded
             last_reload_started_at = -1
 
             # Listen for events and react to them
             while True:
                 event = await self._event_queue.get()
+                rio.cli._logger.debug(f"Received arbiter event `{event}`")
 
                 # A file has changed
                 if isinstance(event, run_models.FileChanged):
                     # Ignore events that happened before the last reload started
                     if event.timestamp_nanoseconds < last_reload_started_at:
                         continue
 
@@ -456,14 +482,17 @@
 
                     # Update the timestamp
                     last_reload_started_at = time.monotonic_ns()
 
                     # If the `rio.toml` has changed, reload the entire project,
                     # not just the app
                     if event.path_to_file == self.proj.rio_toml_path:
+                        rio.cli._logger.info(
+                            "Reloading project configuration from `rio.toml`"
+                        )
                         print("Reloading project configuration from `rio.toml`")
                         self.proj.discard_changes_and_reload()
 
                     # Restart the app
                     await self._restart_app()
 
                 # Somebody requested that the app should stop
@@ -478,14 +507,16 @@
     def _spawn_traceback_popups(self, err: Union[str, BaseException]) -> None:
         """
         Displays a popup with the traceback in the rio UI.
         """
         assert self._uvicorn_worker is not None
         assert self._uvicorn_worker.app_server is not None
 
+        rio.cli._logger.debug("Spawning traceback popups")
+
         popup_html = app_loading.make_traceback_html(
             err=err,
             project_directory=self.proj.project_directory,
         )
 
         for session in self._uvicorn_worker.app_server._active_session_tokens.values():
             self._evaluate_javascript_in_session_if_connected(
@@ -499,14 +530,16 @@
 window.setConnectionLostPopupVisible(true);
 """,
             )
 
     async def _restart_app(self) -> None:
         assert self._uvicorn_worker is not None
 
+        rio.cli._logger.debug("Beginning app restart sequence")
+
         app_server = self._uvicorn_worker.app_server
         assert app_server is not None
 
         # Shut down the current app. This happens automatically when the app
         # server shuts down, but since we're just swapping out the app, we have
         # to call it manually.
         # TODO: Shouldn't we close all the active sessions first? It's odd that
@@ -533,14 +566,16 @@
 
         # The app has changed, but the uvicorn server is still the same. Because
         # of this, uvicorn won't call the `on_app_start` function - do it
         # manually.
         await app_server._call_on_app_start()
 
         # Tell all sessions to reconnect, and close old sessions
+        rio.cli._logger.debug("Reloading all sessions")
+
         for sess in list(app_server._active_session_tokens.values()):
             # Tell the session to reload
             #
             # TODO: Should there be some waiting period here, so that the
             # session has time to save settings first and shut down in general?
             self._evaluate_javascript_in_session_if_connected(
                 sess, "window.location.reload()"
@@ -571,15 +606,7 @@
         async def evaljs_as_coroutine() -> None:
             await session._evaluate_javascript(javascript_source)
 
         session.create_task(
             evaljs_as_coroutine(),
             name=f"Eval JS in session {session._session_token}",
         )
-
-    def _try_build_app(self, build: Callable[[], rio.Component]) -> rio.Component:
-        try:
-            return build()
-        except Exception as error:
-            return app_loading.make_error_message_component(
-                error, self.proj.project_directory
-            )
```

### Comparing `rio_ui-0.5.7/rio/cli/run_project/file_watcher_worker.py` & `rio_ui-0.5.8/rio/cli/run_project/file_watcher_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/cli/run_project/uvicorn_worker.py` & `rio_ui-0.5.8/rio/cli/run_project/uvicorn_worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import revel
 import uvicorn
 import uvicorn.lifespan.on
 
 import rio
 import rio.app_server
+import rio.cli
 
 from .. import nice_traceback
 from . import run_models
 
 
 class UvicornWorker:
     def __init__(
@@ -33,14 +34,16 @@
         self.run_in_window = run_in_window
         self.on_server_is_ready_or_failed = on_server_is_ready_or_failed
 
         # The app server used to host the app
         self.app_server: rio.app_server.AppServer | None = None
 
     async def run(self) -> None:
+        rio.cli._logger.debug("Uvicorn worker is starting")
+
         # Set up a uvicorn server, but don't start it yet
         app_server = self.app._as_fastapi(
             debug_mode=self.debug_mode,
             running_in_window=self.run_in_window,
             validator_factory=None,
             internal_on_app_start=lambda: self.on_server_is_ready_or_failed.set_result(
                 None
@@ -89,19 +92,23 @@
 
         # Run the server
         try:
             await serve_task
         except asyncio.CancelledError:
             pass
         except Exception as err:
+            rio.cli._logger.exception(f"Uvicorn has crashed")
+
             revel.error(f"Uvicorn has crashed:")
             print()
             revel.print(nice_traceback.format_exception_revel(err))
             self.push_event(run_models.StopRequested())
         finally:
+            rio.cli._logger.debug("Requesting uvicorn to exit")
+
             self._uvicorn_server.should_exit = True
 
             # Make sure not to return before the task has returned, but also
             # avoid receiving any exceptions _again_
             try:
                 await serve_task
             except:
@@ -109,8 +116,9 @@
 
     def replace_app(self, app: rio.App) -> None:
         """
         Replace the app currently running in the server with a new one. The
         worker must already be running for this to work.
         """
         assert self.app_server is not None
+        rio.cli._logger.debug("Replacing the app in the server")
         self.app_server.app = app
```

### Comparing `rio_ui-0.5.7/rio/cli/run_project/webview_worker.py` & `rio_ui-0.5.8/rio/cli/run_project/webview_worker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/cli/tomlconfig.py` & `rio_ui-0.5.8/rio/cli/tomlconfig.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/color.py` & `rio_ui-0.5.8/rio/color.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/__init__.py` & `rio_ui-0.5.8/rio/components/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/app_root.py` & `rio_ui-0.5.8/rio/components/app_root.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/auto_form.py` & `rio_ui-0.5.8/rio/components/auto_form.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/banner.py` & `rio_ui-0.5.8/rio/components/banner.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/build_failed.py` & `rio_ui-0.5.8/rio/components/build_failed.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/button.py` & `rio_ui-0.5.8/rio/components/button.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/card.py` & `rio_ui-0.5.8/rio/components/card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/class_container.py` & `rio_ui-0.5.8/rio/components/class_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/color_picker.py` & `rio_ui-0.5.8/rio/components/color_picker.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/component.py` & `rio_ui-0.5.8/rio/components/component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/component_tree.py` & `rio_ui-0.5.8/rio/components/component_tree.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/container.py` & `rio_ui-0.5.8/rio/components/container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/devel_component.py` & `rio_ui-0.5.8/rio/components/devel_component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/drawer.py` & `rio_ui-0.5.8/rio/components/drawer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/dropdown.py` & `rio_ui-0.5.8/rio/components/dropdown.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/flow_container.py` & `rio_ui-0.5.8/rio/components/flow_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/fundamental_component.py` & `rio_ui-0.5.8/rio/components/fundamental_component.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/grid.py` & `rio_ui-0.5.8/rio/components/grid.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/html.py` & `rio_ui-0.5.8/rio/components/html.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/icon.py` & `rio_ui-0.5.8/rio/components/icon.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/image.py` & `rio_ui-0.5.8/rio/components/image.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/key_event_listener.py` & `rio_ui-0.5.8/rio/components/key_event_listener.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/labeled_column.py` & `rio_ui-0.5.8/rio/components/labeled_column.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/linear_containers.py` & `rio_ui-0.5.8/rio/components/linear_containers.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/link.py` & `rio_ui-0.5.8/rio/components/link.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/list_items.py` & `rio_ui-0.5.8/rio/components/list_items.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/list_view.py` & `rio_ui-0.5.8/rio/components/list_view.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/markdown.py` & `rio_ui-0.5.8/rio/components/markdown.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/media_player.py` & `rio_ui-0.5.8/rio/components/media_player.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/mouse_event_listener.py` & `rio_ui-0.5.8/rio/components/mouse_event_listener.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/multi_line_text_input.py` & `rio_ui-0.5.8/rio/components/multi_line_text_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/node_input.py` & `rio_ui-0.5.8/rio/components/node_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/node_output.py` & `rio_ui-0.5.8/rio/components/node_output.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/number_input.py` & `rio_ui-0.5.8/rio/components/number_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/overlay.py` & `rio_ui-0.5.8/rio/components/overlay.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/page_view.py` & `rio_ui-0.5.8/rio/components/page_view.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from collections.abc import Callable
 from dataclasses import KW_ONLY, field
 from typing import *  # type: ignore
 
 import rio
 
+from .. import common
 from .component import Component
 
 __all__ = [
     "PageView",
 ]
 
 
@@ -158,14 +159,14 @@
         # component is mistaken of being internal to Rio. Take care to fix that.
         try:
             page = self.session._active_page_instances[self.level]
         except IndexError:
             if self.fallback_build is None:
                 result = default_fallback_build(self.session)
             else:
-                result = self.fallback_build()
+                result = common.safe_build(self.fallback_build)
                 result._rio_internal_ = False
         else:
-            result = page.build()
+            result = common.safe_build(page.build)
             result._rio_internal_ = False
 
         return result
```

### Comparing `rio_ui-0.5.7/rio/components/plot.py` & `rio_ui-0.5.8/rio/components/plot.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/popup.py` & `rio_ui-0.5.8/rio/components/popup.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/progress_bar.py` & `rio_ui-0.5.8/rio/components/progress_bar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/progress_circle.py` & `rio_ui-0.5.8/rio/components/progress_circle.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/rectangle.py` & `rio_ui-0.5.8/rio/components/rectangle.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/revealer.py` & `rio_ui-0.5.8/rio/components/revealer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/root_components.py` & `rio_ui-0.5.8/rio/components/root_components.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from collections.abc import Callable
 from typing import *  # type: ignore
 
+from .. import common
 from .component import Component
 from .fundamental_component import FundamentalComponent
 from .scroll_container import ScrollContainer
 
 __all__ = ["HighLevelRootComponent"]
 
 
@@ -30,19 +31,19 @@
 
             debugger = rio.debug.client_side_debugger.ClientSideDebugger()
         else:
             debugger = None
 
         # User content should automatically scroll if it grows too large, so we
         # wrap it in a ScrollContainer
-        user_content = ScrollContainer(self.build_function())
+        user_content = ScrollContainer(common.safe_build(self.build_function))
 
         return FundamentalRootComponent(
             user_content,
-            self.build_connection_lost_message_function(),
+            common.safe_build(self.build_connection_lost_message_function),
             debugger=debugger,
         )
 
 
 class FundamentalRootComponent(FundamentalComponent):
     content: Component
     connection_lost_component: Component
```

### Comparing `rio_ui-0.5.7/rio/components/scroll_container.py` & `rio_ui-0.5.8/rio/components/scroll_container.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/scroll_target.py` & `rio_ui-0.5.8/rio/components/scroll_target.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/separator.py` & `rio_ui-0.5.8/rio/components/separator.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/slider.py` & `rio_ui-0.5.8/rio/components/slider.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/slideshow.py` & `rio_ui-0.5.8/rio/components/slideshow.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/spacer.py` & `rio_ui-0.5.8/rio/components/spacer.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/stack.py` & `rio_ui-0.5.8/rio/components/stack.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/switch.py` & `rio_ui-0.5.8/rio/components/switch.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/switcher.py` & `rio_ui-0.5.8/rio/components/switcher.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/switcher_bar.py` & `rio_ui-0.5.8/rio/components/switcher_bar.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/table.py` & `rio_ui-0.5.8/rio/components/table.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/text.py` & `rio_ui-0.5.8/rio/components/text.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/text_input.py` & `rio_ui-0.5.8/rio/components/text_input.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/theme_context_switcher.py` & `rio_ui-0.5.8/rio/components/theme_context_switcher.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/tooltip.py` & `rio_ui-0.5.8/rio/components/tooltip.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/components/website.py` & `rio_ui-0.5.8/rio/components/website.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/dataclass.py` & `rio_ui-0.5.8/rio/dataclass.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
 import abc
+import copy
 import dataclasses
+import functools
 from collections.abc import Callable
 from typing import *  # type: ignore
 
 from typing_extensions import (
     Any,
     ClassVar,
     Self,
@@ -101,20 +103,15 @@
         serialize=serialize,
         init=init,
         repr=repr,
     )
 
 
 def _make_default_factory_for_value(value: T) -> Callable[[], T]:
-    def default_factory() -> T:
-        return value
-
-    default_factory.__name__ = default_factory.__qualname__ = f"return_{value!r}"
-
-    return default_factory
+    return functools.partial(copy.deepcopy, value)
 
 
 @dataclass_transform(
     eq_default=False,
     field_specifiers=(internal_field, dataclasses.field),
 )
 class RioDataclassMeta(abc.ABCMeta):
```

### Comparing `rio_ui-0.5.7/rio/debug/client_side_debugger/component_details.py` & `rio_ui-0.5.8/rio/debug/client_side_debugger/component_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,16 @@
                 style="dim",
                 justify="left",
             ),
             row_index,
             0,
             width=5,
         )
+
+        row_index_before_properties = row_index
         row_index += 1
 
         # Custom properties
         #
         # Make sure to skip any which already have custom tailored cells
         debug_details = target.get_debug_details()
         for prop_name, prop_value in debug_details.items():
@@ -332,10 +334,16 @@
         # the entire Grid, but that would ellipsize some long texts. Instead,
         # add a Spacer into a fifth column, which will take up any unused space.
         result.add(
             rio.Spacer(height=0),
             row_index - 1,
             4,
         )
+        # result.add(
+        #     layout_preview.LayoutPreview(component=target),
+        #     row_index_before_properties + 1,
+        #     4,
+        #     height=row_index - row_index_before_properties,
+        # )
 
         # Done
         return result
```

### Comparing `rio_ui-0.5.7/rio/debug/client_side_debugger/debugger.py` & `rio_ui-0.5.8/rio/debug/client_side_debugger/debugger.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,17 +43,15 @@
             return tree_page.TreePage(
                 width=WIDE_PAGE_WIDTH,
             )
 
         # Icons
         if self.selected_page == "icons":
             return icons_page.IconsPage(
-                # This page contains wide source code. Constant changes to the
-                # size would cause unsightly resizes.
-                width=REGULAR_PAGE_WIDTH + 15
+                width=WIDE_PAGE_WIDTH,
             )
 
         # Theme
         if self.selected_page == "theme":
             return theme_picker_page.ThemePickerPage(
                 width=WIDE_PAGE_WIDTH,
             )
```

### Comparing `rio_ui-0.5.7/rio/debug/client_side_debugger/deploy_page.py` & `rio_ui-0.5.8/rio/debug/client_side_debugger/deploy_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/debug/client_side_debugger/docs_page.py` & `rio_ui-0.5.8/rio/debug/client_side_debugger/docs_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/debug/client_side_debugger/icons_page.py` & `rio_ui-0.5.8/rio/debug/client_side_debugger/icons_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/debug/client_side_debugger/project_page.py` & `rio_ui-0.5.8/rio/debug/client_side_debugger/project_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/debug/client_side_debugger/sample_icons_grid.py` & `rio_ui-0.5.8/rio/debug/client_side_debugger/sample_icons_grid.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/debug/client_side_debugger/theme_picker_page.py` & `rio_ui-0.5.8/rio/debug/client_side_debugger/theme_picker_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/debug/client_side_debugger/tree_page.py` & `rio_ui-0.5.8/rio/debug/client_side_debugger/tree_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/debug/monkeypatches.py` & `rio_ui-0.5.8/rio/debug/monkeypatches.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/debug/typing_utils.py` & `rio_ui-0.5.8/rio/debug/typing_utils.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/debug/validator.py` & `rio_ui-0.5.8/rio/debug/validator.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/docs/custom.py` & `rio_ui-0.5.8/rio/docs/custom.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Contains processing specific to the RIO project.
 """
 
 from typing import *  # type: ignore
 
-import rio
+import imy.docstrings
 
-from . import models
+import rio
 
 
 def find_items_needing_documentation() -> Iterable[Type | Callable]:
     """
     Find all classes and functions in `Rio` that need to be documented.
     """
 
@@ -72,15 +72,15 @@
             continue
 
         # Internal
         if not cur.__name__.startswith("_"):
             yield cur
 
 
-def postprocess_class_docs(docs: models.ClassDocs) -> None:
+def postprocess_class_docs(docs: imy.docstrings.ClassDocs) -> None:
     """
     Perform RIO specific post-processing on the component, such as stripping out
     internal attributes and functions.
     """
 
     # Strip default docstrings created by dataclasses
     if docs.summary is not None and docs.summary.startswith(f"{docs.name}("):
@@ -162,10 +162,10 @@
         # Inject a short description for `__init__` if there is none.
         if func_docs.name == "__init__" and func_docs.summary is None:
             func_docs.summary = f"Creates a new `{docs.name}` instance."
 
     # TODO: Strip out anything `Session` inherits from `unicall`
 
 
-def postprocess_component_docs(docs: models.ClassDocs) -> None:
+def postprocess_component_docs(docs: imy.docstrings.ClassDocs) -> None:
     # Apply the standard class post-processing
     postprocess_class_docs(docs)
```

### Comparing `rio_ui-0.5.7/rio/errors.py` & `rio_ui-0.5.8/rio/errors.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/event.py` & `rio_ui-0.5.8/rio/event.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/fills.py` & `rio_ui-0.5.8/rio/fills.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/global_state.py` & `rio_ui-0.5.8/rio/global_state.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/icon_registry.py` & `rio_ui-0.5.8/rio/icon_registry.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/inspection.py` & `rio_ui-0.5.8/rio/inspection.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/maybes.py` & `rio_ui-0.5.8/rio/maybes.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py` & `rio_ui-0.5.8/rio/patches_for_3rd_party_stuff/IocpProactor_accept_locals_accept_coro.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py` & `rio_ui-0.5.8/rio/patches_for_3rd_party_stuff/ProactorBasePipeTransport_call_connection_lost.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/routing.py` & `rio_ui-0.5.8/rio/routing.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/serialization.py` & `rio_ui-0.5.8/rio/serialization.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/session.py` & `rio_ui-0.5.8/rio/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     inspection,
     routing,
     serialization,
     text_style,
     theme,
     user_settings_module,
 )
-from .components import build_failed, fundamental_component, root_components
+from .components import fundamental_component, root_components
 from .state_properties import StateBinding
 
 __all__ = ["Session"]
 
 
 T = typing.TypeVar("T")
 
@@ -717,41 +717,21 @@
                 # If the event handler made the component dirty again, undo it
                 self._dirty_components.discard(component)
 
             # Others need to be built
             global_state.currently_building_component = component
             global_state.currently_building_session = self
 
-            try:
-                build_result = component.build()
-            except Exception as err:
-                logging.exception(
-                    f"An exception occurred in the `build` method of {component!r}"
-                )
-                build_result = build_failed.BuildFailed(
-                    f"`{type(component).__name__}.build` has crashed",
-                    repr(err),
-                )
-            else:
-                # Sanity check
-                if not isinstance(build_result, rio.Component):  # type: ignore[unnecessary-isinstance]
-                    logging.error(
-                        f"The output of `build` methods must be instances of"
-                        f" `rio.Component`, but `{component}` returned `{build_result}`"
-                    )
-                    build_result = build_failed.BuildFailed(
-                        f"`{type(component).__name__}.build` has returned an invalid result",
-                        f"`build` must return instances of `rio.Component`, but the result was {build_result!r}",
-                    )
-            finally:
-                global_state.currently_building_component = None
-                global_state.currently_building_session = None
+            build_result = common.safe_build(component.build)
+
+            global_state.currently_building_component = None
+            global_state.currently_building_session = None
 
             if component in self._dirty_components:
-                logging.warning(
+                raise RuntimeError(
                     f"The `build()` method of the component `{component}`"
                     f" changed the component's state. Assignments to properties"
                     f" of the component aren't allowed in the `build()` method."
                 )
 
             # Has this component been built before?
             try:
```

### Comparing `rio_ui-0.5.7/rio/snippets/README.md` & `rio_ui-0.5.8/rio/snippets/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/__init__.py` & `rio_ui-0.5.8/rio/snippets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -326,22 +326,28 @@
             # Others are categorized by the directory they're in
             dir_name = snippet.file_path.parent.name
 
             if dir_name == "assets":
                 asset_snippets.append(snippet)
 
             elif dir_name == "components":
+                if snippet.name == "__init__.py":
+                    continue
+
                 assert snippet.is_text_snippet, snippet.file_path
                 component_snippets.append(snippet)
 
             elif dir_name == "pages":
+                if snippet.name == "__init__.py":
+                    continue
+
                 assert snippet.is_text_snippet, snippet.file_path
                 page_snippets.append(snippet)
 
-            elif snippet.file_path.name == "__init__.py":
+            elif snippet.file_path.name == "root_init.py":
                 assert root_init_snippet is None
                 assert snippet.is_text_snippet, snippet.file_path
                 root_init_snippet = snippet
 
             elif snippet.file_path.suffix == ".py":
                 other_python_files.append(snippet)
 
@@ -352,15 +358,15 @@
         assert readme_snippet is not None, f"`README.md` snippet not found for `{name}`"
         assert (
             thumbnail_snippet is not None
         ), f"`thumbnail.svg` snippet not found for {name}"
         assert metadata is not None, f"`meta.json` snippet not found for `{name}`"
         assert (
             root_init_snippet is not None
-        ), f"`__init__.py` snippet not found for `{name}`"
+        ), f"`root_init.py` snippet not found for `{name}`"
 
         return ProjectTemplate(
             name=name,
             level=metadata.level,
             summary=metadata.summary,
             description_markdown_source=readme_snippet.stripped_code(),
             thumbnail=thumbnail_snippet,
```

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/other-examples/simple_counter_app.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/other-examples/simple_counter_app.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/README.md` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/__init__.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/root_init.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_message.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/components/chat_suggestion_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/components/empty_chat_placeholder.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/components/generating_response_placeholder.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/conversation.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/pages/chat_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-AI Chatbot/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/assets/cryptos.csv`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/balance_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_card.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/components/crypto_chart.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/data_models.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/pages/dashboard_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,17 +39,17 @@
     fetches the data when the component is populated.
 
     The build method creates a grid layout for the dashboard, containing a balance component,
     three cryptocurrency components, and a cryptocurrency chart component. The layout is
     structured as follows:
 
     ###################################################
-    #            BalanceCard        | CryptoCard(BTC) #
-    #           Crypto Chart        | CryptoCard(LTC) #
-    #          (Crypto Chart)       | CryptoCard(ETH) #
+    #            BalanceCard        # CryptoCard(BTC) #
+    #           Crypto Chart        # CryptoCard(LTC) #
+    #          (Crypto Chart)       # CryptoCard(ETH) #
     ###################################################
 
     Attributes:
         coin_data: A pandas DataFrame that holds the historical data of three cryptocurrencies:
             Bitcoin, Litecoin, and Ethereum.
     """
```

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Crypto Dashboard/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Empty/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/README.md` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/README.md`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_editor.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/components/item_list.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/data_models.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/pages/crud_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Simple CRUD/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg` & `rio_ui-0.5.8/rio/snippets/snippet-files/project-template-Tic-Tac-Toe/thumbnail.svg`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-2/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-3/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-4/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/components/field.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py` & `rio_ui-0.5.8/rio/snippets/snippet-files/tutorial-tic-tac-toe-part-5/pages/tic_tac_toe_page.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/state_properties.py` & `rio_ui-0.5.8/rio/state_properties.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/text_style.py` & `rio_ui-0.5.8/rio/text_style.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/theme.py` & `rio_ui-0.5.8/rio/theme.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/user_settings_module.py` & `rio_ui-0.5.8/rio/user_settings_module.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/rio/world_units.py` & `rio_ui-0.5.8/rio/world_units.py`

 * *Files identical despite different names*

### Comparing `rio_ui-0.5.7/PKG-INFO` & `rio_ui-0.5.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rio-ui
-Version: 0.5.7
+Version: 0.5.8
 Summary: Build modern Websites and Apps just with Python
 Home-page: https://rio.dev
 License: LGPL-3.0
 Keywords: web-development,web-framework,framework,functional,type-safe,typing,typed,react,web,app,user-interface,web-app,local-app,modern,rio
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -49,46 +49,45 @@
 Requires-Dist: uvicorn[standard] (>=0.23.2,<0.24.0)
 Requires-Dist: watchfiles (>=0.21.0,<0.22.0)
 Requires-Dist: yarl (>=1.9.2,<2.0.0)
 Project-URL: Documentation, https://rio.dev/docs
 Description-Content-Type: text/markdown
 
 ![Rio](https://img.shields.io/badge/Rio-outline.svg?color=%2311e8e3e&link=https%3A%2F%2Frio.dev&style=flat-square&logo=data:image/svg%2bxml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjxzdmcKICAgd2lkdGg9IjEwMDIuMTA1IgogICBoZWlnaHQ9IjE0OTkuODA1NyIKICAgdmlld0JveD0iMCAwIDI2NS4xNDAyOSAzOTYuODIzNTkiCiAgIHZlcnNpb249IjEuMSIKICAgaWQ9InN2Zzg5NiIKICAgeG1sOnNwYWNlPSJwcmVzZXJ2ZSIKICAgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIgogICB4bWxuczpzdmc9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIgogICB4bWxuczpyZGY9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkvMDIvMjItcmRmLXN5bnRheC1ucyMiCiAgIHhtbG5zOmNjPSJodHRwOi8vY3JlYXRpdmVjb21tb25zLm9yZy9ucyMiCiAgIHhtbG5zOmRjPSJodHRwOi8vcHVybC5vcmcvZGMvZWxlbWVudHMvMS4xLyI+PGRlZnMKICAgICBpZD0iZGVmczg5MCIgLz48bWV0YWRhdGEKICAgICBpZD0ibWV0YWRhdGE4OTMiPjxyZGY6UkRGPjxjYzpXb3JrCiAgICAgICAgIHJkZjphYm91dD0iIj48ZGM6Zm9ybWF0PmltYWdlL3N2Zyt4bWw8L2RjOmZvcm1hdD48ZGM6dHlwZQogICAgICAgICAgIHJkZjpyZXNvdXJjZT0iaHR0cDovL3B1cmwub3JnL2RjL2RjbWl0eXBlL1N0aWxsSW1hZ2UiIC8+PC9jYzpXb3JrPjwvcmRmOlJERj48L21ldGFkYXRhPjxnCiAgICAgaWQ9ImxheWVyMSIKICAgICB0cmFuc2Zvcm09InRyYW5zbGF0ZSgyNi40MTM4NDcsNTAuMjcxMzUpIj48cGF0aAogICAgICAgaWQ9InBhdGgxIgogICAgICAgc3R5bGU9ImZpbGw6I2ZmZmZmZjtmaWxsLW9wYWNpdHk6MTtzdHJva2Utd2lkdGg6MC4yNjQ1ODMiCiAgICAgICBkPSJtIC04LjgwMzA4MDMsLTUwLjI3MTM1IGMgLTE1LjI3NjU1OTcsMC44NjA1MjQgLTE4LjYzMTgzNDcsMTcuNTQ0NTEyIC0xNy4zNjc0MTU3LDI5Ljk2ODk1MiAwLjUxMzcyNywxNi4yNDQxNjYxIC0xLjIxMzE5NywzMi43MTkyOTcgMS4yNjg1MTcsNDguNzY2NzkzIDguMTQxMTg1LDE0LjcxMDAxMiAyNi4wNzc2NzYxLDE4Ljg0OTk3MiAzOS44Nzc0ODIsMjYuNzcwMTM0IDMwLjM3ODk2MiwxNS4wNjY1NSA2MC43NTc5MjUsMzAuMTMzMTAxIDkxLjEzNjg4Nyw0NS4xOTk2NTEgLTM0LjgyMjM5OCwxNy42MDY2OCAtNzAuMjI2MTE3LDM0LjE0NzgzIC0xMDQuNjYwNTA2OCw1Mi40NjUyOCAtMjAuMDM3Nzc1MiwxMS40ODE0NCAtMzQuNzc4MTg3MiwzNi45NjY5OCAtMjQuMTAxMTk2Miw1OS41OTIxMSAxMS4yOTkzMSwyNS42MDQ3IDM5Ljc0MjkxMSwzMy43MTY5NSA2Mi40NzIyMDgsNDUuOTY4MDIgNTguOTU5MTAzLDI5LjA5NDExIDExNy43MTA1MzUsNTguNjQ4NDIgMTc2Ljc4OTE1NSw4Ny40NzU2IDE0LjA2MTIxLDMuOTY4MzYgMjQuMDM2NzYsLTEyLjAyMzEgMjEuODAwNzksLTI0LjUzMjIgLTAuNTQyODUsLTE3LjgzMTU3IDEuMjU4MTYsLTM1LjkwMjkyIC0xLjI2ODM2LC01My41MzY0OCAtOC4xNDA2MywtMTQuNzEwNzEgLTI2LjA3NjkyLC0xOC44NTE5OCAtMzkuODc3MTksLTI2Ljc3MTcyIC0zMC4zNzYwNiwtMTUuMDcxMTUgLTYwLjgwMDczLC0zMC4xNDExNyAtOTEuMTQ2NDIsLTQ1LjIxMzA0IDM0LjUwODc5LC0xNy4zNzM3NyA2OS40NTU5NywtMzMuOTI1NjUgMTAzLjY3Mjk4LC01MS44NDY2MyAyMC4xOTUxMywtMTEuMDA2MjggMzUuMzg2NDQsLTM2LjMwMDA1IDI1LjYwMzM4LC01OC45ODA5NCBDIDIyNC43MDYyMyw1OC44NzI1MzQgMTk2LjA1MDY3LDUwLjQ4NjY0MSAxNzMuMTY3MjYsMzguMjM4MTkxIDE1MS4xOTIyNiwyNy4zNDkyOTUgMTI2LjI0NjM5LDE0LjkzOTYzOCAxMDYuMTIxMTcsNC45OTc2Mjc4IDcwLjA0MTcxOSwtMTIuODk5Mjk5IDMzLjk2MjI2OCwtMzAuNzk2MjI1IC0yLjExNzE4MzQsLTQ4LjY5MzE1MiBsIC0zLjM3MjY3NzcsLTEuMjE4NDkyIHoiIC8+PC9nPjwvc3ZnPgo=)
+![Version](https://img.shields.io/pypi/v/rio-ui?color=%2311e8e3e&style=flat-square)
 ![Discord](https://img.shields.io/discord/1213589765484576818?color=%2311e8e3e&label=discord&style=flat-square)
 ![Python Version](https://img.shields.io/pypi/pyversions/rio-ui?style=flat-square)
-![Version](https://img.shields.io/pypi/v/rio-ui?color=%2311e8e3e&style=flat-square)
 ![License](https://img.shields.io/pypi/l/rio-ui?color=%2311e8e3e&style=flat-square)
-
-<!-- TODO: Gitlab Stars -->
+![GitHub Stars](https://img.shields.io/github/stars/rio-labs/rio?style=flat-square)
 
 <!-- https://shields.io/badges -->
 
-<img src="https://gitlab.com/team-rio/rio/-/raw/dev/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png" alt="Rio Logo" style="width: 30rem" />
+<img src="https://github.com/rio-labs/rio/blob/dev/rio/assets/hosted/rio-logos/logo-and-text-horizontal.png?raw=true" alt="Rio Logo" style="width: 16rem" />
 
 🌊 You've arrived at **Rio**, an easy to use framework for creating websites and
 apps.
 
 🐍 Rio is based **entirely on Python**. You **won't need a single line of HTML, CSS, or
 JavaScript** to create beautiful, modern apps.
 
-[Tutorial](https://rio.dev/get-started) - [Examples](https://rio.dev/examples) - [Discord](https://discord.gg/7ejXaPwhyH) - [Docs](https://rio.dev/docs) - [Source Code](https://gitlab.com/team-rio/rio)
+[Tutorial](https://rio.dev/get-started) - [Examples](https://rio.dev/examples) - [Discord](https://discord.gg/7ejXaPwhyH) - [Docs](https://rio.dev/docs) - [Source Code](https://github.com/rio-labs/rio)
 
 Rio brings React-style components to Python. Pull from a wealth of built-in
 components and combine them to create your own custom components. Then combine
 those into entire apps. Best of all, Rio apps can run both locally on your
 machine and on the web.
 
 ## Features 🧩
 
--   Modern, **declarative UI** framework
--   **100% Python** - Zero HTML, CSS, or JavaScript required
--   Over **50 Built-in components** for common UI elements, such as `rio.Switch`, `rio.Button`, and `rio.Text`, and many more
--   Integrates with **modern Python tooling**: Thanks to being **entirely Type Safe** editors can give you instant suggestions and highlight problems right away
--   Apps can run **both locally and on the web**
--   **Open Source & Free forever**
+- Modern, **declarative UI** framework
+- **100% Python** - Zero HTML, CSS, or JavaScript required
+- Over **50 Built-in components** for common UI elements, such as `rio.Switch`, `rio.Button`, and `rio.Text`, and many more
+- Integrates with **modern Python tooling**: Thanks to being **entirely Type Safe** editors can give you instant suggestions and highlight problems right away
+- Apps can run **both locally and on the web**
+- **Open Source & Free forever**
 
 ## Installation 🛠️
 
 Rio is available on PyPI, so you can install it using pip:
 
 ```bash
 pip install rio-ui
@@ -197,9 +196,19 @@
     pages=[
         rio.Page(
             page_url="",
             build=DallEPage,
         ),
     ],
 )
+
+## Status: In Development 🚧
+
+Rio is still in development. We're working hard to bring you the best possible
+experience. If you have any feedback, please let us know on our Discord server.
+
+## Contributing 🤝
+
+Write how someone can contribute to the project. :)
+
 ```
```

