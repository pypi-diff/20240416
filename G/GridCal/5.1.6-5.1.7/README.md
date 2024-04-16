# Comparing `tmp/GridCal-5.1.6.tar.gz` & `tmp/GridCal-5.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GridCal-5.1.6.tar", last modified: Sat Apr 13 14:14:26 2024, max compression
+gzip compressed data, was "GridCal-5.1.7.tar", last modified: Tue Apr 16 20:42:31 2024, max compression
```

## Comparing `GridCal-5.1.6.tar` & `GridCal-5.1.7.tar`

### file list

```diff
@@ -1,227 +1,227 @@
--rw-rw-r--   0 santi     (1000) santi     (1000)     2808 2024-04-12 12:41:14.151810 GridCal-5.1.6/GridCal/__version__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      654 2023-11-16 09:36:26.514645 GridCal-5.1.6/GridCal/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1545 2024-03-11 19:28:12.151075 GridCal-5.1.6/GridCal/ExecuteGridCal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11713 2024-03-11 19:28:12.175075 GridCal-5.1.6/GridCal/LICENSE.txt
--rw-rw-r--   0 santi     (1000) santi     (1000)     2965 2024-01-05 08:44:35.533288 GridCal-5.1.6/GridCal/update.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5188 2024-03-11 19:28:12.175075 GridCal-5.1.6/GridCal/templates.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8747 2024-03-28 10:16:48.968877 GridCal-5.1.6/GridCal/Session/results_model.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4257 2024-03-14 19:48:07.680505 GridCal-5.1.6/GridCal/Session/export_results_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21120 2024-03-14 19:48:07.680505 GridCal-5.1.6/GridCal/Session/session.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13285 2024-03-14 19:48:07.680505 GridCal-5.1.6/GridCal/Session/synchronization_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-14 19:48:07.680505 GridCal-5.1.6/GridCal/Session/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7043 2024-04-08 13:34:15.971164 GridCal-5.1.6/GridCal/Session/file_handler.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    33193 2022-08-17 15:43:33.049797 GridCal-5.1.6/GridCal/data/cables.csv
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2022-08-17 15:43:33.033797 GridCal-5.1.6/GridCal/data/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      388 2024-04-11 15:31:05.578472 GridCal-5.1.6/GridCal/data/sequence_lines.csv
--rw-rw-r--   0 santi     (1000) santi     (1000)    55648 2023-11-16 09:36:26.518645 GridCal-5.1.6/GridCal/data/transformers.csv
--rw-rw-r--   0 santi     (1000) santi     (1000)     5013 2022-08-17 15:43:33.045797 GridCal-5.1.6/GridCal/data/wires.csv
--rw-rw-r--   0 santi     (1000) santi     (1000)    25703 2024-03-14 19:48:07.672505 GridCal-5.1.6/GridCal/Gui/GeneralDialogues.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1634 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/update_gui_all.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.6/GridCal/Gui/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2551 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/messages.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2969 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/themes.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3978 2024-02-13 14:28:28.563734 GridCal-5.1.6/GridCal/Gui/ConsoleWidget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    85249 2024-04-12 16:08:47.131984 GridCal-5.1.6/GridCal/Gui/GuiFunctions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1986 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/plot_config.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3740 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/update_gui_common.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.6/GridCal/Gui/Widgets/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7365 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/Widgets/matplotlibwidget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    45061 2023-11-16 09:36:26.514645 GridCal-5.1.6/GridCal/Gui/Widgets/custom_qrangeslider.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.6/GridCal/Gui/ContingencyPlanner/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.086158 GridCal-5.1.6/GridCal/Gui/ContingencyPlanner/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15460 2023-11-16 09:36:26.482645 GridCal-5.1.6/GridCal/Gui/ContingencyPlanner/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5241 2024-03-11 19:28:12.159075 GridCal-5.1.6/GridCal/Gui/ContingencyPlanner/contingency_planner_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11953 2023-11-16 09:36:26.482645 GridCal-5.1.6/GridCal/Gui/ContingencyPlanner/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.6/GridCal/Gui/CoordinatesInput/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.086158 GridCal-5.1.6/GridCal/Gui/CoordinatesInput/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    39352 2023-11-16 09:36:26.482645 GridCal-5.1.6/GridCal/Gui/CoordinatesInput/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9471 2023-11-16 09:36:26.482645 GridCal-5.1.6/GridCal/Gui/CoordinatesInput/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15110 2024-03-11 19:28:12.159075 GridCal-5.1.6/GridCal/Gui/CoordinatesInput/coordinates_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.6/GridCal/Gui/TowerBuilder/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.102158 GridCal-5.1.6/GridCal/Gui/TowerBuilder/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11704 2024-03-11 19:28:12.175075 GridCal-5.1.6/GridCal/Gui/TowerBuilder/table_models.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4789 2023-11-16 09:36:26.506645 GridCal-5.1.6/GridCal/Gui/TowerBuilder/test_.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21426 2024-03-14 19:48:07.680505 GridCal-5.1.6/GridCal/Gui/TowerBuilder/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16061 2024-03-14 19:48:07.680505 GridCal-5.1.6/GridCal/Gui/TowerBuilder/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11180 2024-03-11 19:28:12.171075 GridCal-5.1.6/GridCal/Gui/TowerBuilder/LineBuilderDialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6333 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/graphics_manager.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.832547 GridCal-5.1.6/GridCal/Gui/Diagrams/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2695 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/diagrams_model.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      792 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   198492 2024-04-12 14:20:56.563894 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/diagram_editor_widget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7195 2024-04-12 14:37:07.823907 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/generic_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7801 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/matplotlibwidget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13045 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/terminal_item.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6408 2024-04-08 13:34:15.955164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_turbine_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6090 2024-04-08 13:34:15.955164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_pump_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6253 2024-04-12 14:15:42.503889 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_path_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6079 2024-04-08 13:34:15.955164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_p2x_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17195 2024-04-12 14:15:42.515889 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_node_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4879 2024-04-08 13:34:15.955164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/winding_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13617 2024-04-12 14:15:42.539889 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4338 2024-04-08 13:34:15.955164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/switch_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4321 2024-04-12 14:20:56.579894 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/series_reactance_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12367 2024-04-12 14:15:42.579889 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/dc_line_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4961 2024-04-12 14:15:42.475889 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/hvdc_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4480 2024-04-12 14:15:42.547889 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/upfc_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9547 2024-04-12 14:15:42.571889 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer2w_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9485 2024-04-11 15:31:05.570472 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_editor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4792 2024-04-12 14:15:42.555889 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/vsc_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13960 2024-04-12 14:04:34.963880 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer3w_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10044 2024-04-08 13:34:15.955164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer_editor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    32985 2024-04-12 14:15:42.563889 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics_template.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6403 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/static_generator_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6422 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/current_injection_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5938 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/injections_template_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5983 2024-04-08 13:34:15.955164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/battery_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6495 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/shunt_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6426 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/external_grid_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6416 2024-04-08 13:34:15.955164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/controllable_shunt_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5635 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/load_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    19276 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/generator_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.959164 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    30364 2024-04-12 14:04:34.939880 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/busbar_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21549 2024-04-12 14:04:34.795880 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/cn_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    30526 2024-04-12 14:15:42.495889 GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/bus_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   160182 2024-04-11 18:07:34.874291 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/map_widget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5067 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/node_widget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2418 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/map_events.py
--rw-rw-r--   0 santi     (1000) santi     (1000)       36 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/logger.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21089 2024-04-12 14:39:32.843909 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/grid_map_widget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3360 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/tile_worker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13730 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6101 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/base_tiles.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2766 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles_cache.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2974 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/pycacheback.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    30307 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/default_tile_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4966 2024-04-11 18:07:34.870291 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Schema/Nodes.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2090 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Schema/Connector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Schema/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2159 2024-04-11 18:07:34.870291 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Schema/SchemaManager.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4975 2024-04-11 18:07:34.870291 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Schema/Substations.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1917 2024-04-11 18:07:34.870291 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Schema/Line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      121 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/layer_types.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3646 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/point_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3920 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/image_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      282 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/place.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3651 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/polyline_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3900 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/text_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3757 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/polygon_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2942 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/open_street_map.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2349 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapbox.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2904 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/cartodb.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2513 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapquest.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2601 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_transport.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2419 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_watercolor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2391 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/blue_marble.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2408 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_toner.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4274 2024-04-03 10:10:53.828547 GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/gmt_local.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7262 2024-03-11 19:28:12.151075 GridCal-5.1.6/GridCal/Gui/AboutDialogue/about_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.082158 GridCal-5.1.6/GridCal/Gui/AboutDialogue/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.082158 GridCal-5.1.6/GridCal/Gui/AboutDialogue/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14879 2024-02-29 08:22:37.932355 GridCal-5.1.6/GridCal/Gui/AboutDialogue/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11275 2024-03-11 19:28:12.151075 GridCal-5.1.6/GridCal/Gui/AboutDialogue/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1217 2023-11-16 09:36:26.498645 GridCal-5.1.6/GridCal/Gui/ProfilesInput/excel_dialog.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      243 2023-11-16 09:36:26.498645 GridCal-5.1.6/GridCal/Gui/ProfilesInput/profiles_from_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.498645 GridCal-5.1.6/GridCal/Gui/ProfilesInput/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16317 2023-11-16 09:36:26.498645 GridCal-5.1.6/GridCal/Gui/ProfilesInput/profiles_from_data_gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      353 2023-06-09 13:30:46.098158 GridCal-5.1.6/GridCal/Gui/ProfilesInput/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11691 2024-03-11 19:28:12.171075 GridCal-5.1.6/GridCal/Gui/ProfilesInput/models_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    45917 2023-11-16 09:36:26.498645 GridCal-5.1.6/GridCal/Gui/ProfilesInput/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    24295 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/ProfilesInput/profile_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5707 2023-11-16 09:36:26.502645 GridCal-5.1.6/GridCal/Gui/ProfilesInput/profiles_from_models_gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2420 2023-11-16 09:36:26.498645 GridCal-5.1.6/GridCal/Gui/ProfilesInput/excel_sheet_selection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.482645 GridCal-5.1.6/GridCal/Gui/Analysis/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      485 2023-11-16 09:36:26.482645 GridCal-5.1.6/GridCal/Gui/Analysis/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21495 2023-11-16 09:36:26.482645 GridCal-5.1.6/GridCal/Gui/Analysis/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3871 2024-03-11 19:28:12.151075 GridCal-5.1.6/GridCal/Gui/Analysis/AnalysisDialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18860 2023-11-16 09:36:26.482645 GridCal-5.1.6/GridCal/Gui/Analysis/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    48733 2024-04-01 07:29:23.256927 GridCal-5.1.6/GridCal/Gui/Analysis/object_plot_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5003 2024-03-11 19:28:12.159075 GridCal-5.1.6/GridCal/Gui/CascadingSteps/cascading_steps.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.482645 GridCal-5.1.6/GridCal/Gui/CascadingSteps/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      281 2023-11-16 09:36:26.482645 GridCal-5.1.6/GridCal/Gui/CascadingSteps/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5684 2023-11-16 09:36:26.482645 GridCal-5.1.6/GridCal/Gui/CascadingSteps/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1464 2024-02-13 14:28:28.563734 GridCal-5.1.6/GridCal/Gui/Main/ConsoleLogController.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4843 2024-03-28 10:16:48.956877 GridCal-5.1.6/GridCal/Gui/Main/GridCalMain.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   276874 2024-04-12 06:51:51.955518 GridCal-5.1.6/GridCal/Gui/Main/MainWindow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.6/GridCal/Gui/Main/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      591 2023-11-16 09:36:26.498645 GridCal-5.1.6/GridCal/Gui/Main/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5157 2024-04-12 06:51:51.955518 GridCal-5.1.6/GridCal/Gui/Main/ConsoleLog.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   807433 2024-04-12 06:51:51.959518 GridCal-5.1.6/GridCal/Gui/Main/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2195 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/Main/object_select_window.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      359 2023-11-16 09:36:26.490645 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/README.txt
--rw-rw-r--   0 santi     (1000) santi     (1000)   110018 2024-04-08 13:34:15.963164 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/simulations.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    33887 2024-04-11 18:07:34.874291 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/io.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    31266 2024-04-08 13:34:15.963164 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/base_gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3784 2024-02-13 14:28:28.567734 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Scripting/python_highlighter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Scripting/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5813 2024-04-01 07:49:22.774443 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Scripting/scripting.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Settings/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17930 2024-04-11 18:07:34.874291 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Settings/configuration.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    45640 2024-04-11 18:07:34.874291 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Model/objects.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21114 2024-04-11 18:07:34.874291 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Model/time_events.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Model/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    72028 2024-04-12 10:06:43.207681 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Model/diagrams.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5891 2024-03-11 19:28:12.163075 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Model/compiled_arrays.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Results/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12771 2024-03-14 19:48:07.676505 GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Results/results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.6/GridCal/Gui/Visualization/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2838 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/Visualization/visualization.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11934 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/Visualization/palettes.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.6/GridCal/Gui/SyncDialogue/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.102158 GridCal-5.1.6/GridCal/Gui/SyncDialogue/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14939 2023-11-16 09:36:26.506645 GridCal-5.1.6/GridCal/Gui/SyncDialogue/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3233 2024-03-14 19:48:07.680505 GridCal-5.1.6/GridCal/Gui/SyncDialogue/sync_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4684 2023-11-16 09:36:26.506645 GridCal-5.1.6/GridCal/Gui/SyncDialogue/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6556 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/SolarPowerWizard/solar_power_wizzard.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.506645 GridCal-5.1.6/GridCal/Gui/SolarPowerWizard/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-11-16 09:36:26.506645 GridCal-5.1.6/GridCal/Gui/SolarPowerWizard/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18492 2023-11-16 09:36:26.506645 GridCal-5.1.6/GridCal/Gui/SolarPowerWizard/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7914 2023-11-16 09:36:26.506645 GridCal-5.1.6/GridCal/Gui/SolarPowerWizard/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    24893 2023-11-16 09:36:26.502645 GridCal-5.1.6/GridCal/Gui/RosetaExplorer/MainWindow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.502645 GridCal-5.1.6/GridCal/Gui/RosetaExplorer/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      574 2023-11-16 09:36:26.502645 GridCal-5.1.6/GridCal/Gui/RosetaExplorer/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18469 2024-03-11 19:28:12.171075 GridCal-5.1.6/GridCal/Gui/RosetaExplorer/RosetaExplorer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1976 2023-11-16 09:36:26.502645 GridCal-5.1.6/GridCal/Gui/RosetaExplorer/ConsoleWidget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   225320 2023-11-16 09:36:26.502645 GridCal-5.1.6/GridCal/Gui/RosetaExplorer/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.486645 GridCal-5.1.6/GridCal/Gui/LoadDesigner/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      316 2024-03-17 11:12:27.689061 GridCal-5.1.6/GridCal/Gui/LoadDesigner/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5615 2024-03-17 11:12:27.689061 GridCal-5.1.6/GridCal/Gui/LoadDesigner/load_designer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    37622 2024-03-17 11:12:27.689061 GridCal-5.1.6/GridCal/Gui/LoadDesigner/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13073 2024-03-17 11:12:27.689061 GridCal-5.1.6/GridCal/Gui/LoadDesigner/load_designer_ui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3692 2024-02-13 14:28:28.571734 GridCal-5.1.6/GridCal/Gui/WindPowerWizard/wind_power_wizzard.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.6/GridCal/Gui/WindPowerWizard/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-11-16 09:36:26.514645 GridCal-5.1.6/GridCal/Gui/WindPowerWizard/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9724 2023-11-16 09:36:26.514645 GridCal-5.1.6/GridCal/Gui/WindPowerWizard/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7869 2023-11-16 09:36:26.514645 GridCal-5.1.6/GridCal/Gui/WindPowerWizard/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-17 11:12:27.693060 GridCal-5.1.6/GridCal/Gui/SystemScaler/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      316 2024-03-17 11:12:27.693060 GridCal-5.1.6/GridCal/Gui/SystemScaler/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9718 2024-03-28 10:16:48.968877 GridCal-5.1.6/GridCal/Gui/SystemScaler/system_scaler.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    37622 2024-03-17 11:12:27.693060 GridCal-5.1.6/GridCal/Gui/SystemScaler/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4357 2024-03-17 11:12:27.693060 GridCal-5.1.6/GridCal/Gui/SystemScaler/system_scaler_ui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4262 2023-11-16 09:36:26.506645 GridCal-5.1.6/GridCal/Gui/TreeModelViewer/MainWindow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.506645 GridCal-5.1.6/GridCal/Gui/TreeModelViewer/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      574 2023-11-16 09:36:26.514645 GridCal-5.1.6/GridCal/Gui/TreeModelViewer/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   224984 2023-11-16 09:36:26.514645 GridCal-5.1.6/GridCal/Gui/TreeModelViewer/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8686 2024-03-11 19:28:12.175075 GridCal-5.1.6/GridCal/Gui/TreeModelViewer/TreeModelViewer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.502645 GridCal-5.1.6/GridCal/Gui/SigmaAnalysis/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.102158 GridCal-5.1.6/GridCal/Gui/SigmaAnalysis/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    41704 2023-11-16 09:36:26.502645 GridCal-5.1.6/GridCal/Gui/SigmaAnalysis/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4758 2023-11-16 09:36:26.502645 GridCal-5.1.6/GridCal/Gui/SigmaAnalysis/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4018 2024-03-14 19:48:07.680505 GridCal-5.1.6/GridCal/Gui/SigmaAnalysis/sigma_analysis_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.6/GridCal/Gui/GridGenerator/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.090158 GridCal-5.1.6/GridCal/Gui/GridGenerator/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5329 2024-03-11 19:28:12.159075 GridCal-5.1.6/GridCal/Gui/GridGenerator/grid_generator_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15613 2023-11-16 09:36:26.486645 GridCal-5.1.6/GridCal/Gui/GridGenerator/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15239 2023-11-16 09:36:26.486645 GridCal-5.1.6/GridCal/Gui/GridGenerator/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4923 2024-04-11 18:07:34.878291 GridCal-5.1.6/setup.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1043 2024-04-13 14:14:26.922700 GridCal-5.1.6/PKG-INFO
--rw-rw-r--   0 santi     (1000) santi     (1000)       37 2024-04-13 14:14:26.922700 GridCal-5.1.6/setup.cfg
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2808 2024-04-16 11:07:46.030900 GridCal-5.1.7/GridCal/__version__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      654 2023-11-16 09:36:26.514645 GridCal-5.1.7/GridCal/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1545 2024-03-11 19:28:12.151075 GridCal-5.1.7/GridCal/ExecuteGridCal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11713 2024-03-11 19:28:12.175075 GridCal-5.1.7/GridCal/LICENSE.txt
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2965 2024-01-05 08:44:35.533288 GridCal-5.1.7/GridCal/update.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5188 2024-03-11 19:28:12.175075 GridCal-5.1.7/GridCal/templates.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8747 2024-03-28 10:16:48.968877 GridCal-5.1.7/GridCal/Session/results_model.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4257 2024-03-14 19:48:07.680505 GridCal-5.1.7/GridCal/Session/export_results_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    24280 2024-04-16 15:44:22.535429 GridCal-5.1.7/GridCal/Session/session.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13285 2024-03-14 19:48:07.680505 GridCal-5.1.7/GridCal/Session/synchronization_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-14 19:48:07.680505 GridCal-5.1.7/GridCal/Session/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7043 2024-04-08 13:34:15.971164 GridCal-5.1.7/GridCal/Session/file_handler.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    33193 2022-08-17 15:43:33.049797 GridCal-5.1.7/GridCal/data/cables.csv
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2022-08-17 15:43:33.033797 GridCal-5.1.7/GridCal/data/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      388 2024-04-16 11:07:46.030900 GridCal-5.1.7/GridCal/data/sequence_lines.csv
+-rw-rw-r--   0 santi     (1000) santi     (1000)    55648 2023-11-16 09:36:26.518645 GridCal-5.1.7/GridCal/data/transformers.csv
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5013 2022-08-17 15:43:33.045797 GridCal-5.1.7/GridCal/data/wires.csv
+-rw-rw-r--   0 santi     (1000) santi     (1000)    25703 2024-03-14 19:48:07.672505 GridCal-5.1.7/GridCal/Gui/GeneralDialogues.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1634 2024-02-13 14:28:28.571734 GridCal-5.1.7/GridCal/Gui/update_gui_all.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.7/GridCal/Gui/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2551 2024-02-13 14:28:28.571734 GridCal-5.1.7/GridCal/Gui/messages.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2969 2024-02-13 14:28:28.571734 GridCal-5.1.7/GridCal/Gui/themes.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3978 2024-02-13 14:28:28.563734 GridCal-5.1.7/GridCal/Gui/ConsoleWidget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    85249 2024-04-16 11:07:46.022900 GridCal-5.1.7/GridCal/Gui/GuiFunctions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1986 2024-02-13 14:28:28.571734 GridCal-5.1.7/GridCal/Gui/plot_config.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3740 2024-02-13 14:28:28.571734 GridCal-5.1.7/GridCal/Gui/update_gui_common.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.7/GridCal/Gui/Widgets/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7365 2024-02-13 14:28:28.571734 GridCal-5.1.7/GridCal/Gui/Widgets/matplotlibwidget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    45061 2023-11-16 09:36:26.514645 GridCal-5.1.7/GridCal/Gui/Widgets/custom_qrangeslider.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.7/GridCal/Gui/ContingencyPlanner/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.086158 GridCal-5.1.7/GridCal/Gui/ContingencyPlanner/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15460 2023-11-16 09:36:26.482645 GridCal-5.1.7/GridCal/Gui/ContingencyPlanner/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5241 2024-03-11 19:28:12.159075 GridCal-5.1.7/GridCal/Gui/ContingencyPlanner/contingency_planner_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11953 2023-11-16 09:36:26.482645 GridCal-5.1.7/GridCal/Gui/ContingencyPlanner/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.7/GridCal/Gui/CoordinatesInput/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.086158 GridCal-5.1.7/GridCal/Gui/CoordinatesInput/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    39352 2023-11-16 09:36:26.482645 GridCal-5.1.7/GridCal/Gui/CoordinatesInput/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9471 2023-11-16 09:36:26.482645 GridCal-5.1.7/GridCal/Gui/CoordinatesInput/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15110 2024-03-11 19:28:12.159075 GridCal-5.1.7/GridCal/Gui/CoordinatesInput/coordinates_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.7/GridCal/Gui/TowerBuilder/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.102158 GridCal-5.1.7/GridCal/Gui/TowerBuilder/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11704 2024-03-11 19:28:12.175075 GridCal-5.1.7/GridCal/Gui/TowerBuilder/table_models.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4789 2023-11-16 09:36:26.506645 GridCal-5.1.7/GridCal/Gui/TowerBuilder/test_.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21426 2024-03-14 19:48:07.680505 GridCal-5.1.7/GridCal/Gui/TowerBuilder/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16061 2024-03-14 19:48:07.680505 GridCal-5.1.7/GridCal/Gui/TowerBuilder/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11180 2024-03-11 19:28:12.171075 GridCal-5.1.7/GridCal/Gui/TowerBuilder/LineBuilderDialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6333 2024-04-08 13:34:15.959164 GridCal-5.1.7/GridCal/Gui/Diagrams/graphics_manager.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.832547 GridCal-5.1.7/GridCal/Gui/Diagrams/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2695 2024-04-08 13:34:15.959164 GridCal-5.1.7/GridCal/Gui/Diagrams/diagrams_model.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      792 2024-04-08 13:34:15.959164 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   198560 2024-04-16 11:07:46.018900 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/diagram_editor_widget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7195 2024-04-16 11:07:46.018900 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/generic_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7801 2024-04-08 13:34:15.959164 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/matplotlibwidget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13045 2024-04-08 13:34:15.959164 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/terminal_item.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6408 2024-04-08 13:34:15.955164 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_turbine_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6090 2024-04-08 13:34:15.955164 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_pump_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6253 2024-04-16 11:07:46.018900 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_path_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6079 2024-04-08 13:34:15.955164 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_p2x_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17195 2024-04-16 11:07:46.018900 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_node_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4879 2024-04-08 13:34:15.955164 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/winding_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13617 2024-04-16 11:07:46.018900 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4338 2024-04-08 13:34:15.955164 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/switch_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4321 2024-04-16 11:07:46.018900 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/series_reactance_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12367 2024-04-16 11:07:46.018900 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/dc_line_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4961 2024-04-16 11:07:46.018900 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/hvdc_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4480 2024-04-16 11:07:46.018900 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/upfc_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9547 2024-04-16 11:07:46.018900 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer2w_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9485 2024-04-16 11:07:46.018900 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_editor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4792 2024-04-16 11:07:46.018900 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/vsc_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13960 2024-04-12 14:04:34.963880 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer3w_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10044 2024-04-08 13:34:15.955164 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer_editor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    32985 2024-04-16 11:07:46.018900 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics_template.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6403 2024-04-08 13:34:15.959164 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/static_generator_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6422 2024-04-08 13:34:15.959164 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/current_injection_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5938 2024-04-08 13:34:15.959164 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/injections_template_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5983 2024-04-08 13:34:15.955164 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/battery_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6495 2024-04-08 13:34:15.959164 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/shunt_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6426 2024-04-08 13:34:15.959164 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/external_grid_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6416 2024-04-08 13:34:15.955164 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/controllable_shunt_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5635 2024-04-08 13:34:15.959164 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/load_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    19276 2024-04-08 13:34:15.959164 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/generator_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.959164 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    30364 2024-04-16 11:07:46.018900 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/busbar_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21549 2024-04-16 11:07:46.018900 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/cn_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    30526 2024-04-16 11:07:46.018900 GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/bus_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   160182 2024-04-16 11:07:46.022900 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/map_widget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5067 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/node_widget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2418 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/map_events.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)       36 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/logger.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21089 2024-04-16 11:07:46.022900 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/grid_map_widget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3360 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Tiles/tile_worker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13730 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Tiles/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6101 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Tiles/base_tiles.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2766 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles_cache.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2974 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Tiles/pycacheback.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    30307 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Tiles/default_tile_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4966 2024-04-16 11:07:46.022900 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Schema/Nodes.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2090 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Schema/Connector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Schema/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2159 2024-04-16 11:07:46.022900 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Schema/SchemaManager.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4975 2024-04-16 11:07:46.022900 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Schema/Substations.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1917 2024-04-16 11:07:46.018900 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Schema/Line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      121 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Layers/layer_types.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3646 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Layers/point_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3920 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Layers/image_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Layers/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      282 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Layers/place.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3651 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Layers/polyline_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3900 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Layers/text_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3757 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Layers/polygon_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2942 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/TileProviders/open_street_map.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2349 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapbox.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2904 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/TileProviders/cartodb.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2513 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapquest.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2601 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_transport.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/TileProviders/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2419 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_watercolor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2391 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/TileProviders/blue_marble.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2408 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_toner.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4274 2024-04-03 10:10:53.828547 GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/TileProviders/gmt_local.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7262 2024-03-11 19:28:12.151075 GridCal-5.1.7/GridCal/Gui/AboutDialogue/about_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.082158 GridCal-5.1.7/GridCal/Gui/AboutDialogue/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.082158 GridCal-5.1.7/GridCal/Gui/AboutDialogue/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14879 2024-02-29 08:22:37.932355 GridCal-5.1.7/GridCal/Gui/AboutDialogue/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11275 2024-03-11 19:28:12.151075 GridCal-5.1.7/GridCal/Gui/AboutDialogue/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1217 2023-11-16 09:36:26.498645 GridCal-5.1.7/GridCal/Gui/ProfilesInput/excel_dialog.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      243 2023-11-16 09:36:26.498645 GridCal-5.1.7/GridCal/Gui/ProfilesInput/profiles_from_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.498645 GridCal-5.1.7/GridCal/Gui/ProfilesInput/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16317 2023-11-16 09:36:26.498645 GridCal-5.1.7/GridCal/Gui/ProfilesInput/profiles_from_data_gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      353 2023-06-09 13:30:46.098158 GridCal-5.1.7/GridCal/Gui/ProfilesInput/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11691 2024-03-11 19:28:12.171075 GridCal-5.1.7/GridCal/Gui/ProfilesInput/models_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    45917 2023-11-16 09:36:26.498645 GridCal-5.1.7/GridCal/Gui/ProfilesInput/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    24295 2024-02-13 14:28:28.571734 GridCal-5.1.7/GridCal/Gui/ProfilesInput/profile_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5707 2023-11-16 09:36:26.502645 GridCal-5.1.7/GridCal/Gui/ProfilesInput/profiles_from_models_gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2420 2023-11-16 09:36:26.498645 GridCal-5.1.7/GridCal/Gui/ProfilesInput/excel_sheet_selection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.482645 GridCal-5.1.7/GridCal/Gui/Analysis/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      485 2023-11-16 09:36:26.482645 GridCal-5.1.7/GridCal/Gui/Analysis/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21495 2023-11-16 09:36:26.482645 GridCal-5.1.7/GridCal/Gui/Analysis/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3871 2024-03-11 19:28:12.151075 GridCal-5.1.7/GridCal/Gui/Analysis/AnalysisDialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18860 2023-11-16 09:36:26.482645 GridCal-5.1.7/GridCal/Gui/Analysis/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    48733 2024-04-01 07:29:23.256927 GridCal-5.1.7/GridCal/Gui/Analysis/object_plot_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5027 2024-04-16 13:44:36.655200 GridCal-5.1.7/GridCal/Gui/CascadingSteps/cascading_steps.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.482645 GridCal-5.1.7/GridCal/Gui/CascadingSteps/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      281 2023-11-16 09:36:26.482645 GridCal-5.1.7/GridCal/Gui/CascadingSteps/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5684 2023-11-16 09:36:26.482645 GridCal-5.1.7/GridCal/Gui/CascadingSteps/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1464 2024-02-13 14:28:28.563734 GridCal-5.1.7/GridCal/Gui/Main/ConsoleLogController.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4843 2024-03-28 10:16:48.956877 GridCal-5.1.7/GridCal/Gui/Main/GridCalMain.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   276874 2024-04-16 11:07:46.022900 GridCal-5.1.7/GridCal/Gui/Main/MainWindow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.7/GridCal/Gui/Main/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      591 2023-11-16 09:36:26.498645 GridCal-5.1.7/GridCal/Gui/Main/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5157 2024-04-12 06:51:51.955518 GridCal-5.1.7/GridCal/Gui/Main/ConsoleLog.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   807433 2024-04-16 11:07:46.030900 GridCal-5.1.7/GridCal/Gui/Main/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2195 2024-02-13 14:28:28.571734 GridCal-5.1.7/GridCal/Gui/Main/object_select_window.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.7/GridCal/Gui/Main/SubClasses/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      359 2023-11-16 09:36:26.490645 GridCal-5.1.7/GridCal/Gui/Main/SubClasses/README.txt
+-rw-rw-r--   0 santi     (1000) santi     (1000)   108399 2024-04-16 15:44:22.499429 GridCal-5.1.7/GridCal/Gui/Main/SubClasses/simulations.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    34480 2024-04-16 15:44:22.559429 GridCal-5.1.7/GridCal/Gui/Main/SubClasses/io.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    31217 2024-04-16 13:44:36.655200 GridCal-5.1.7/GridCal/Gui/Main/SubClasses/base_gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3784 2024-02-13 14:28:28.567734 GridCal-5.1.7/GridCal/Gui/Main/SubClasses/Scripting/python_highlighter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.7/GridCal/Gui/Main/SubClasses/Scripting/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5813 2024-04-01 07:49:22.774443 GridCal-5.1.7/GridCal/Gui/Main/SubClasses/Scripting/scripting.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.7/GridCal/Gui/Main/SubClasses/Settings/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18004 2024-04-16 15:45:38.743431 GridCal-5.1.7/GridCal/Gui/Main/SubClasses/Settings/configuration.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    45640 2024-04-16 11:07:46.026900 GridCal-5.1.7/GridCal/Gui/Main/SubClasses/Model/objects.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21114 2024-04-16 11:07:46.026900 GridCal-5.1.7/GridCal/Gui/Main/SubClasses/Model/time_events.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.7/GridCal/Gui/Main/SubClasses/Model/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    72034 2024-04-16 12:18:07.015034 GridCal-5.1.7/GridCal/Gui/Main/SubClasses/Model/diagrams.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5891 2024-03-11 19:28:12.163075 GridCal-5.1.7/GridCal/Gui/Main/SubClasses/Model/compiled_arrays.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.7/GridCal/Gui/Main/SubClasses/Results/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12730 2024-04-16 15:44:22.543429 GridCal-5.1.7/GridCal/Gui/Main/SubClasses/Results/results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.7/GridCal/Gui/Visualization/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2838 2024-02-13 14:28:28.571734 GridCal-5.1.7/GridCal/Gui/Visualization/visualization.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11934 2024-02-13 14:28:28.571734 GridCal-5.1.7/GridCal/Gui/Visualization/palettes.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.7/GridCal/Gui/SyncDialogue/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.102158 GridCal-5.1.7/GridCal/Gui/SyncDialogue/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14939 2023-11-16 09:36:26.506645 GridCal-5.1.7/GridCal/Gui/SyncDialogue/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3233 2024-03-14 19:48:07.680505 GridCal-5.1.7/GridCal/Gui/SyncDialogue/sync_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4684 2023-11-16 09:36:26.506645 GridCal-5.1.7/GridCal/Gui/SyncDialogue/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6556 2024-02-13 14:28:28.571734 GridCal-5.1.7/GridCal/Gui/SolarPowerWizard/solar_power_wizzard.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.506645 GridCal-5.1.7/GridCal/Gui/SolarPowerWizard/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-11-16 09:36:26.506645 GridCal-5.1.7/GridCal/Gui/SolarPowerWizard/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18492 2023-11-16 09:36:26.506645 GridCal-5.1.7/GridCal/Gui/SolarPowerWizard/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7914 2023-11-16 09:36:26.506645 GridCal-5.1.7/GridCal/Gui/SolarPowerWizard/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    24893 2023-11-16 09:36:26.502645 GridCal-5.1.7/GridCal/Gui/RosetaExplorer/MainWindow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.502645 GridCal-5.1.7/GridCal/Gui/RosetaExplorer/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      574 2023-11-16 09:36:26.502645 GridCal-5.1.7/GridCal/Gui/RosetaExplorer/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18469 2024-03-11 19:28:12.171075 GridCal-5.1.7/GridCal/Gui/RosetaExplorer/RosetaExplorer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1976 2023-11-16 09:36:26.502645 GridCal-5.1.7/GridCal/Gui/RosetaExplorer/ConsoleWidget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   225320 2023-11-16 09:36:26.502645 GridCal-5.1.7/GridCal/Gui/RosetaExplorer/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.486645 GridCal-5.1.7/GridCal/Gui/LoadDesigner/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      316 2024-03-17 11:12:27.689061 GridCal-5.1.7/GridCal/Gui/LoadDesigner/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5615 2024-03-17 11:12:27.689061 GridCal-5.1.7/GridCal/Gui/LoadDesigner/load_designer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    37622 2024-03-17 11:12:27.689061 GridCal-5.1.7/GridCal/Gui/LoadDesigner/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13073 2024-03-17 11:12:27.689061 GridCal-5.1.7/GridCal/Gui/LoadDesigner/load_designer_ui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3692 2024-02-13 14:28:28.571734 GridCal-5.1.7/GridCal/Gui/WindPowerWizard/wind_power_wizzard.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.7/GridCal/Gui/WindPowerWizard/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-11-16 09:36:26.514645 GridCal-5.1.7/GridCal/Gui/WindPowerWizard/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9724 2023-11-16 09:36:26.514645 GridCal-5.1.7/GridCal/Gui/WindPowerWizard/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7869 2023-11-16 09:36:26.514645 GridCal-5.1.7/GridCal/Gui/WindPowerWizard/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-17 11:12:27.693060 GridCal-5.1.7/GridCal/Gui/SystemScaler/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      316 2024-03-17 11:12:27.693060 GridCal-5.1.7/GridCal/Gui/SystemScaler/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9718 2024-03-28 10:16:48.968877 GridCal-5.1.7/GridCal/Gui/SystemScaler/system_scaler.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    37622 2024-03-17 11:12:27.693060 GridCal-5.1.7/GridCal/Gui/SystemScaler/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4357 2024-03-17 11:12:27.693060 GridCal-5.1.7/GridCal/Gui/SystemScaler/system_scaler_ui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4262 2023-11-16 09:36:26.506645 GridCal-5.1.7/GridCal/Gui/TreeModelViewer/MainWindow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.506645 GridCal-5.1.7/GridCal/Gui/TreeModelViewer/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      574 2023-11-16 09:36:26.514645 GridCal-5.1.7/GridCal/Gui/TreeModelViewer/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   224984 2023-11-16 09:36:26.514645 GridCal-5.1.7/GridCal/Gui/TreeModelViewer/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8686 2024-03-11 19:28:12.175075 GridCal-5.1.7/GridCal/Gui/TreeModelViewer/TreeModelViewer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.502645 GridCal-5.1.7/GridCal/Gui/SigmaAnalysis/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.102158 GridCal-5.1.7/GridCal/Gui/SigmaAnalysis/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    41704 2023-11-16 09:36:26.502645 GridCal-5.1.7/GridCal/Gui/SigmaAnalysis/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4758 2023-11-16 09:36:26.502645 GridCal-5.1.7/GridCal/Gui/SigmaAnalysis/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4018 2024-03-14 19:48:07.680505 GridCal-5.1.7/GridCal/Gui/SigmaAnalysis/sigma_analysis_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.7/GridCal/Gui/GridGenerator/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.090158 GridCal-5.1.7/GridCal/Gui/GridGenerator/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5329 2024-03-11 19:28:12.159075 GridCal-5.1.7/GridCal/Gui/GridGenerator/grid_generator_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15613 2023-11-16 09:36:26.486645 GridCal-5.1.7/GridCal/Gui/GridGenerator/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15239 2023-11-16 09:36:26.486645 GridCal-5.1.7/GridCal/Gui/GridGenerator/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4923 2024-04-16 11:07:46.030900 GridCal-5.1.7/setup.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1043 2024-04-16 20:42:31.774153 GridCal-5.1.7/PKG-INFO
+-rw-rw-r--   0 santi     (1000) santi     (1000)       37 2024-04-16 20:42:31.774153 GridCal-5.1.7/setup.cfg
```

### Comparing `GridCal-5.1.6/GridCal/__version__.py` & `GridCal-5.1.7/GridCal/__version__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with GridCal.  If not, see <http://www.gnu.org/licenses/>.
 import datetime
 _current_year_ = datetime.datetime.now().year
 
 # do not forget to keep a three-number version!!!
-__GridCal_VERSION__ = "5.1.6"
+__GridCal_VERSION__ = "5.1.7"
 
 url = 'https://github.com/SanPen/GridCal'
 
 about_msg = "GridCal v" + str(__GridCal_VERSION__) + '\n\n'
 
 about_msg += """
 GridCal has been carefully crafted since 2015 to
```

### Comparing `GridCal-5.1.6/GridCal/__init__.py` & `GridCal-5.1.7/GridCal/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/ExecuteGridCal.py` & `GridCal-5.1.7/GridCal/ExecuteGridCal.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/LICENSE.txt` & `GridCal-5.1.7/GridCal/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/update.py` & `GridCal-5.1.7/GridCal/update.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/templates.py` & `GridCal-5.1.7/GridCal/templates.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Session/results_model.py` & `GridCal-5.1.7/GridCal/Session/results_model.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Session/export_results_driver.py` & `GridCal-5.1.7/GridCal/Session/export_results_driver.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Session/synchronization_driver.py` & `GridCal-5.1.7/GridCal/Session/synchronization_driver.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Session/file_handler.py` & `GridCal-5.1.7/GridCal/Session/file_handler.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/data/cables.csv` & `GridCal-5.1.7/GridCal/data/cables.csv`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/data/transformers.csv` & `GridCal-5.1.7/GridCal/data/transformers.csv`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/data/wires.csv` & `GridCal-5.1.7/GridCal/data/wires.csv`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/GeneralDialogues.py` & `GridCal-5.1.7/GridCal/Gui/GeneralDialogues.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/update_gui_all.py` & `GridCal-5.1.7/GridCal/Gui/update_gui_all.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/messages.py` & `GridCal-5.1.7/GridCal/Gui/messages.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/themes.py` & `GridCal-5.1.7/GridCal/Gui/themes.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/ConsoleWidget.py` & `GridCal-5.1.7/GridCal/Gui/ConsoleWidget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/GuiFunctions.py` & `GridCal-5.1.7/GridCal/Gui/GuiFunctions.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/plot_config.py` & `GridCal-5.1.7/GridCal/Gui/plot_config.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/update_gui_common.py` & `GridCal-5.1.7/GridCal/Gui/update_gui_common.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Widgets/matplotlibwidget.py` & `GridCal-5.1.7/GridCal/Gui/Widgets/matplotlibwidget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Widgets/custom_qrangeslider.py` & `GridCal-5.1.7/GridCal/Gui/Widgets/custom_qrangeslider.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/ContingencyPlanner/icons_rc.py` & `GridCal-5.1.7/GridCal/Gui/ContingencyPlanner/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/ContingencyPlanner/contingency_planner_dialogue.py` & `GridCal-5.1.7/GridCal/Gui/ContingencyPlanner/contingency_planner_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/ContingencyPlanner/gui.py` & `GridCal-5.1.7/GridCal/Gui/ContingencyPlanner/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/CoordinatesInput/icons_rc.py` & `GridCal-5.1.7/GridCal/Gui/CoordinatesInput/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/CoordinatesInput/gui.py` & `GridCal-5.1.7/GridCal/Gui/CoordinatesInput/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/CoordinatesInput/coordinates_dialogue.py` & `GridCal-5.1.7/GridCal/Gui/CoordinatesInput/coordinates_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/TowerBuilder/table_models.py` & `GridCal-5.1.7/GridCal/Gui/TowerBuilder/table_models.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/TowerBuilder/test_.py` & `GridCal-5.1.7/GridCal/Gui/TowerBuilder/test_.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/TowerBuilder/icons_rc.py` & `GridCal-5.1.7/GridCal/Gui/TowerBuilder/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/TowerBuilder/gui.py` & `GridCal-5.1.7/GridCal/Gui/TowerBuilder/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/TowerBuilder/LineBuilderDialogue.py` & `GridCal-5.1.7/GridCal/Gui/TowerBuilder/LineBuilderDialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/graphics_manager.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/graphics_manager.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/diagrams_model.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/diagrams_model.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/__init__.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/diagram_editor_widget.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/diagram_editor_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -933,15 +933,16 @@
 
                         graphic_object.change_size(h=location.h,
                                                    w=location.w)
 
                         # add fluid node reference for later
                         # fluid_node_dict[idtag] = graphic_object
                         self.graphics_manager.add_device(elm=location.api_object, graphic=graphic_object)
-                        self.graphics_manager.add_device(elm=location.api_object.bus, graphic=graphic_object)
+                        if location.api_object.bus is not None:
+                            self.graphics_manager.add_device(elm=location.api_object.bus, graphic=graphic_object)
 
                         # map the internal bus
                         # if location.api_object.bus is not None:
                         #     bus_dict[location.api_object.bus.idtag] = graphic_object
 
             else:
                 # pass for now...
```

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/generic_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/generic_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/matplotlibwidget.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/matplotlibwidget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/terminal_item.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/terminal_item.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_turbine_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_turbine_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_pump_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_pump_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_path_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_path_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_p2x_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_p2x_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_node_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_node_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/winding_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/winding_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/switch_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/switch_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/series_reactance_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/series_reactance_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/dc_line_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/dc_line_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/hvdc_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/hvdc_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/upfc_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/upfc_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer2w_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer2w_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_editor.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_editor.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/vsc_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/vsc_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer3w_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer3w_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer_editor.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer_editor.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics_template.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics_template.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/static_generator_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/static_generator_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/current_injection_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/current_injection_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/injections_template_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/injections_template_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/battery_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/battery_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/shunt_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/shunt_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/external_grid_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/external_grid_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/controllable_shunt_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/controllable_shunt_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/load_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/load_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/generator_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/generator_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/busbar_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/busbar_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/cn_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/cn_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/bus_graphics.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/bus_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/map_widget.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/map_widget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/node_widget.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/node_widget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/map_events.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/map_events.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/grid_map_widget.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/grid_map_widget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/tile_worker.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Tiles/tile_worker.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/base_tiles.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Tiles/base_tiles.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles_cache.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles_cache.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/pycacheback.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Tiles/pycacheback.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Tiles/default_tile_data.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Tiles/default_tile_data.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Schema/Nodes.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Schema/Nodes.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Schema/Connector.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Schema/Connector.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Schema/SchemaManager.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Schema/SchemaManager.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Schema/Substations.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Schema/Substations.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Schema/Line.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Schema/Line.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/point_layer.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Layers/point_layer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/image_layer.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Layers/image_layer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/polyline_layer.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Layers/polyline_layer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/text_layer.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Layers/text_layer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/Layers/polygon_layer.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/Layers/polygon_layer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/open_street_map.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/TileProviders/open_street_map.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapbox.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapbox.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/cartodb.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/TileProviders/cartodb.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapquest.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapquest.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_transport.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_transport.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_watercolor.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_watercolor.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/blue_marble.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/TileProviders/blue_marble.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_toner.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_toner.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Diagrams/MapWidget/TileProviders/gmt_local.py` & `GridCal-5.1.7/GridCal/Gui/Diagrams/MapWidget/TileProviders/gmt_local.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/AboutDialogue/about_dialogue.py` & `GridCal-5.1.7/GridCal/Gui/AboutDialogue/about_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/AboutDialogue/icons_rc.py` & `GridCal-5.1.7/GridCal/Gui/AboutDialogue/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/AboutDialogue/gui.py` & `GridCal-5.1.7/GridCal/Gui/AboutDialogue/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/ProfilesInput/excel_dialog.py` & `GridCal-5.1.7/GridCal/Gui/ProfilesInput/excel_dialog.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/ProfilesInput/profiles_from_data_gui.py` & `GridCal-5.1.7/GridCal/Gui/ProfilesInput/profiles_from_data_gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/ProfilesInput/models_dialogue.py` & `GridCal-5.1.7/GridCal/Gui/ProfilesInput/models_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/ProfilesInput/icons_rc.py` & `GridCal-5.1.7/GridCal/Gui/ProfilesInput/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/ProfilesInput/profile_dialogue.py` & `GridCal-5.1.7/GridCal/Gui/ProfilesInput/profile_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/ProfilesInput/profiles_from_models_gui.py` & `GridCal-5.1.7/GridCal/Gui/ProfilesInput/profiles_from_models_gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/ProfilesInput/excel_sheet_selection.py` & `GridCal-5.1.7/GridCal/Gui/ProfilesInput/excel_sheet_selection.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Analysis/icons_rc.py` & `GridCal-5.1.7/GridCal/Gui/Analysis/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Analysis/AnalysisDialogue.py` & `GridCal-5.1.7/GridCal/Gui/Analysis/AnalysisDialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Analysis/gui.py` & `GridCal-5.1.7/GridCal/Gui/Analysis/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Analysis/object_plot_analysis.py` & `GridCal-5.1.7/GridCal/Gui/Analysis/object_plot_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/CascadingSteps/cascading_steps.py` & `GridCal-5.1.7/GridCal/Gui/CascadingSteps/cascading_steps.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         if len(self.gridcal_main.circuit.get_buses()) > 0:
 
             self.gridcal_main.LOCK()
             if self.gridcal_main.session.exists(sim.SimulationTypes.Cascade_run):
                 options = self.gridcal_main.get_selected_power_flow_options()
                 options.solver_type = SolverType.LM
                 max_isl = self.gridcal_main.ui.cascading_islands_spinBox.value()
-                drv = sim.Cascading(self.gridcal_main.circuit.copy(), options, max_additional_islands=max_isl)
+                drv = sim.CascadingDriver(self.gridcal_main.circuit.copy(), options, max_additional_islands=max_isl)
 
                 self.gridcal_main.session.run(drv,
                                               post_func=self.gridcal_main.post_cascade,
                                               prog_func=self.gridcal_main.ui.progressBar.setValue,
                                               text_func=self.gridcal_main.ui.progress_label.setText)
 
             self.gridcal_main.cascade.perform_step_run()
@@ -97,17 +97,17 @@
 
                 options = self.gridcal_main.get_selected_power_flow_options()
                 options.solver_type = SolverType.LM
 
                 max_isl = self.gridcal_main.ui.cascading_islands_spinBox.value()
                 n_lsh_samples = self.gridcal_main.ui.max_iterations_stochastic_spinBox.value()
 
-                drv = sim.Cascading(self.gridcal_main.circuit.copy(), options,
-                                    max_additional_islands=max_isl,
-                                    n_lhs_samples_=n_lsh_samples)
+                drv = sim.CascadingDriver(self.gridcal_main.circuit.copy(), options,
+                                          max_additional_islands=max_isl,
+                                          n_lhs_samples_=n_lsh_samples)
 
                 self.gridcal_main.session.run(drv,
                                               post_func=self.gridcal_main.post_cascade,
                                               prog_func=self.gridcal_main.ui.progressBar.setValue,
                                               text_func=self.gridcal_main.ui.progress_label.setText)
 
                 # run
```

### Comparing `GridCal-5.1.6/GridCal/Gui/CascadingSteps/gui.py` & `GridCal-5.1.7/GridCal/Gui/CascadingSteps/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Main/ConsoleLogController.py` & `GridCal-5.1.7/GridCal/Gui/Main/ConsoleLogController.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Main/GridCalMain.py` & `GridCal-5.1.7/GridCal/Gui/Main/GridCalMain.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Main/MainWindow.py` & `GridCal-5.1.7/GridCal/Gui/Main/MainWindow.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Main/update_gui_file.py` & `GridCal-5.1.7/GridCal/Gui/Main/update_gui_file.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Main/ConsoleLog.py` & `GridCal-5.1.7/GridCal/Gui/Main/ConsoleLog.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Main/icons_rc.py` & `GridCal-5.1.7/GridCal/Gui/Main/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Main/object_select_window.py` & `GridCal-5.1.7/GridCal/Gui/Main/object_select_window.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Main/SubClasses/simulations.py` & `GridCal-5.1.7/GridCal/Gui/Main/SubClasses/simulations.py`

 * *Files 6% similar despite different names*

```diff
@@ -626,15 +626,15 @@
         """
         Get the current OPF time series results
         :param use_opf: use the OPF?
         :return:
         """
         if use_opf:
 
-            drv, opf_time_series_results = self.session.get_driver_results(SimulationTypes.OPFTimeSeries_run)
+            opf_time_series_results = self.session.optimal_power_flow_ts
 
             if opf_time_series_results is None:
                 if use_opf:
                     info_msg('There are no OPF time series, '
                              'therefore this operation will not use OPF information.')
                     self.ui.actionOpf_to_Power_flow.setChecked(False)
 
@@ -761,24 +761,20 @@
         """
         Action performed after the power flow.
         Returns:
 
         """
         # update the results in the circuit structures
 
-        drv, results = self.session.get_driver_results(sim.SimulationTypes.PowerFlow_run)
+        results = self.session.power_flow
 
         if results is not None:
             self.ui.progress_label.setText('Colouring power flow results in the grid...')
-            # QtGui.QGuiApplication.processEvents()
-
             self.remove_simulation(sim.SimulationTypes.PowerFlow_run)
-
             self.update_available_results()
-
             self.colour_diagrams()
 
         else:
             warning_msg('There are no power flow results.\nIs there any slack bus or generator?', 'Power flow')
 
         if not self.session.is_anything_running():
             self.UNLOCK()
@@ -789,15 +785,15 @@
         The short circuit simulation must be performed after a power flow simulation
         without any load or topology change
         :return:
         """
         if len(self.circuit.buses) > 0:
             if not self.session.is_this_running(sim.SimulationTypes.ShortCircuit_run):
 
-                pf_drv, pf_results = self.session.get_driver_results(sim.SimulationTypes.PowerFlow_run)
+                pf_results = self.session.power_flow
 
                 if pf_results is not None:
 
                     # Since we must run this study in the same conditions as
                     # the last power flow, no compilation is needed
 
                     # get the short circuit selected buses
@@ -857,23 +853,21 @@
     def post_short_circuit(self):
         """
         Action performed after the short circuit.
         Returns:
 
         """
         # update the results in the circuit structures
-        drv, results = self.session.get_driver_results(sim.SimulationTypes.ShortCircuit_run)
-        self.remove_simulation(sim.SimulationTypes.ShortCircuit_run)
+        results = self.session.short_circuit
+
         if results is not None:
 
             self.ui.progress_label.setText('Colouring short circuit results in the grid...')
-            QtGui.QGuiApplication.processEvents()
-
+            self.remove_simulation(sim.SimulationTypes.ShortCircuit_run)
             self.update_available_results()
-
             self.colour_diagrams()
 
         else:
             error_msg('Something went wrong, There are no power short circuit results.')
 
         if not self.session.is_anything_running():
             self.UNLOCK()
@@ -923,20 +917,18 @@
 
     def post_linear_analysis(self):
         """
         Action performed after the short circuit.
         Returns:
 
         """
-        drv, results = self.session.get_driver_results(sim.SimulationTypes.LinearAnalysis_run)
-
         self.remove_simulation(sim.SimulationTypes.LinearAnalysis_run)
 
         # update the results in the circuit structures
-        # if not drv.__cancel__:
+        results = self.session.linear_power_flow
         if results is not None:
 
             self.ui.progress_label.setText('Colouring PTDF results in the grid...')
             QtGui.QGuiApplication.processEvents()
 
             self.update_available_results()
             self.colour_diagrams()
@@ -978,18 +970,18 @@
 
     def post_linear_analysis_ts(self):
         """
         Action performed after the short circuit.
         Returns:
 
         """
-        drv, results = self.session.get_driver_results(sim.SimulationTypes.LinearAnalysis_TS_run)
         self.remove_simulation(sim.SimulationTypes.LinearAnalysis_TS_run)
 
         # update the results in the circuit structures
+        results = self.session.linear_power_flow_ts
         if results is not None:
 
             # expand the clusters
             results.expand_clustered_results()
 
             self.ui.progress_label.setText('Colouring PTDF results in the grid...')
             QtGui.QGuiApplication.processEvents()
@@ -1067,19 +1059,18 @@
 
     def post_contingency_analysis(self):
         """
         Action performed after the short circuit.
         Returns:
 
         """
-        drv, results = self.session.get_driver_results(sim.SimulationTypes.ContingencyAnalysis_run)
         self.remove_simulation(sim.SimulationTypes.ContingencyAnalysis_run)
 
         # update the results in the circuit structures
-        # if not drv.__cancel__:
+        results = self.session.contingency
         if results is not None:
 
             self.ui.progress_label.setText('Colouring contingency analysis results in the grid...')
             QtGui.QGuiApplication.processEvents()
 
             self.update_available_results()
 
@@ -1102,19 +1093,19 @@
                 if self.valid_time_series():
                     if not self.session.is_this_running(sim.SimulationTypes.ContingencyAnalysisTS_run):
 
                         self.add_simulation(sim.SimulationTypes.ContingencyAnalysisTS_run)
 
                         self.LOCK()
 
-                        drv = sim.ContingencyAnalysisTimeSeries(grid=self.circuit,
-                                                                options=self.get_contingency_options(),
-                                                                time_indices=self.get_time_indices(),
-                                                                clustering_results=self.get_clustering_results(),
-                                                                engine=self.get_preferred_engine())
+                        drv = sim.ContingencyAnalysisTimeSeriesDriver(grid=self.circuit,
+                                                                      options=self.get_contingency_options(),
+                                                                      time_indices=self.get_time_indices(),
+                                                                      clustering_results=self.get_clustering_results(),
+                                                                      engine=self.get_preferred_engine())
 
                         self.session.run(drv,
                                          post_func=self.post_contingency_analysis_ts,
                                          prog_func=self.ui.progressBar.setValue,
                                          text_func=self.ui.progress_label.setText)
                     else:
                         warning_msg('Another LODF is being executed now...')
@@ -1129,19 +1120,18 @@
 
     def post_contingency_analysis_ts(self) -> None:
         """
         Action performed after the short circuit.
         Returns:
 
         """
-        drv, results = self.session.get_driver_results(sim.SimulationTypes.ContingencyAnalysisTS_run)
         self.remove_simulation(sim.SimulationTypes.ContingencyAnalysisTS_run)
 
         # update the results in the circuit structures
-        # if not drv.__cancel__:
+        results = self.session.contingency_ts
         if results is not None:
 
             # expand the clusters
             results.expand_clustered_results()
 
             self.ui.progress_label.setText('Colouring results in the grid...')
             QtGui.QGuiApplication.processEvents()
@@ -1180,15 +1170,15 @@
                 sense_br = np.array([sense for i, bus, sense in lst_br])
 
                 # HVDC
                 idx_hvdc_br = np.array([i for i, bus, sense in lst_hvdc_br])
                 sense_hvdc_br = np.array([sense for i, bus, sense in lst_hvdc_br])
 
                 if self.ui.usePfValuesForAtcCheckBox.isChecked():
-                    pf_drv, pf_results = self.session.get_driver_results(sim.SimulationTypes.PowerFlow_run)
+                    pf_results = self.session.power_flow
                     if pf_results is not None:
                         Pf = pf_results.Sf.real
                         Pf_hvdc = pf_results.hvdc_Pf.real
                         use_provided_flows = True
                     else:
                         warning_msg('There were no power flow values available. Linear flows will be used.')
                         use_provided_flows = False
@@ -1246,19 +1236,18 @@
 
     def post_available_transfer_capacity(self):
         """
         Action performed after the short circuit.
         Returns:
 
         """
-        drv, results = self.session.get_driver_results(sim.SimulationTypes.NetTransferCapacity_run)
         self.remove_simulation(sim.SimulationTypes.NetTransferCapacity_run)
+        results = self.session.net_transfer_capacity
 
         # update the results in the circuit structures
-        # if not drv.__cancel__:
         if results is not None:
 
             self.ui.progress_label.setText('Colouring ATC results in the grid...')
             QtGui.QGuiApplication.processEvents()
 
             self.update_available_results()
             self.colour_diagrams()
@@ -1297,15 +1286,15 @@
                     sense_br = np.array([sense for i, bus, sense in lst_br])
 
                     # HVDC
                     idx_hvdc_br = np.array([i for i, bus, sense in lst_hvdc_br])
                     sense_hvdc_br = np.array([sense for i, bus, sense in lst_hvdc_br])
 
                     if self.ui.usePfValuesForAtcCheckBox.isChecked():
-                        pf_drv, pf_results = self.session.get_driver_results(sim.SimulationTypes.TimeSeries_run)
+                        pf_results = self.session.power_flow_ts
                         if pf_results is not None:
                             Pf = pf_results.Sf.real
                             Pf_hvdc = pf_results.hvdc_Pf.real
                             use_provided_flows = True
                         else:
                             warning_msg('There were no power flow values available. Linear flows will be used.')
                             use_provided_flows = False
@@ -1368,19 +1357,18 @@
 
     def post_available_transfer_capacity_ts(self):
         """
         Action performed after the short circuit.
         Returns:
 
         """
-        drv, results = self.session.get_driver_results(sim.SimulationTypes.NetTransferCapacityTS_run)
         self.remove_simulation(sim.SimulationTypes.NetTransferCapacityTS_run)
 
         # update the results in the circuit structures
-        # if not drv.__cancel__:
+        results = self.session.net_transfer_capacity_ts
         if results is not None:
 
             # expand the clusters
             results.expand_clustered_results()
 
             self.ui.progress_label.setText('Colouring ATC time series results in the grid...')
             QtGui.QGuiApplication.processEvents()
@@ -1397,15 +1385,15 @@
         """
         Run voltage stability (voltage collapse) in a separated thread
         :return:
         """
 
         if len(self.circuit.buses) > 0:
 
-            pf_drv, pf_results = self.session.get_driver_results(sim.SimulationTypes.PowerFlow_run)
+            pf_drv, pf_results = self.session.power_flow_driver_and_results
 
             if pf_results is not None:
 
                 if not self.session.is_this_running(sim.SimulationTypes.ContinuationPowerFlow_run):
 
                     # get the selected UI options
                     use_alpha = self.ui.start_vs_from_default_radioButton.isChecked()
@@ -1499,15 +1487,15 @@
                                                                    Vbase=pf_results.voltage,
                                                                    Starget=Sbase * alpha,
                                                                    base_overload_number=base_overload_number)
 
                         pf_options = self.get_selected_power_flow_options()
 
                         # create object
-                        drv = sim.ContinuationPowerFlowDriver(circuit=self.circuit,
+                        drv = sim.ContinuationPowerFlowDriver(grid=self.circuit,
                                                               options=vc_options,
                                                               inputs=vc_inputs,
                                                               pf_options=pf_options)
                         self.session.run(drv,
                                          post_func=self.post_continuation_power_flow,
                                          prog_func=self.ui.progressBar.setValue,
                                          text_func=self.ui.progress_label.setText)
@@ -1517,26 +1505,26 @@
                         Here the start and finish power states are taken from the profiles
                         '''
                         if start_idx > -1 and end_idx > -1:
 
                             # lock the UI
                             self.LOCK()
 
-                            pf_drv.run_at(start_idx)
+                            pf_drv.run_at(start_idx)  # TODO: inspect this
 
                             # get the power Injections array to get the initial and end points
                             Sprof = self.circuit.get_Sbus_prof()
                             vc_inputs = sim.ContinuationPowerFlowInput(Sbase=Sprof[start_idx, :],
                                                                        Vbase=pf_results.voltage,
                                                                        Starget=Sprof[end_idx, :])
 
                             pf_options = self.get_selected_power_flow_options()
 
                             # create object
-                            drv = sim.ContinuationPowerFlowDriver(circuit=self.circuit,
+                            drv = sim.ContinuationPowerFlowDriver(grid=self.circuit,
                                                                   options=vc_options,
                                                                   inputs=vc_inputs,
                                                                   pf_options=pf_options)
                             self.session.run(drv,
                                              post_func=self.post_continuation_power_flow,
                                              prog_func=self.ui.progressBar.setValue,
                                              text_func=self.ui.progress_label.setText)
@@ -1551,15 +1539,15 @@
             pass
 
     def post_continuation_power_flow(self):
         """
         Actions performed after the voltage stability. Launched by the thread after its execution
         :return:
         """
-        drv, results = self.session.get_driver_results(sim.SimulationTypes.ContinuationPowerFlow_run)
+        results = self.session.continuation_power_flow
 
         if results is not None:
 
             self.remove_simulation(sim.SimulationTypes.ContinuationPowerFlow_run)
 
             if results.voltages is not None:
                 if results.voltages.shape[0] > 0:
@@ -1616,15 +1604,15 @@
 
     def post_power_flow_time_series(self):
         """
         Events to do when the time series simulation has finished
         @return:
         """
 
-        drv, results = self.session.get_driver_results(sim.SimulationTypes.TimeSeries_run)
+        results = self.session.power_flow_ts
 
         if results is not None:
 
             # expand the clusters
             results.expand_clustered_results()
 
             self.remove_simulation(sim.SimulationTypes.TimeSeries_run)
@@ -1686,15 +1674,15 @@
 
     def post_stochastic(self):
         """
         Actions to perform after the Monte Carlo simulation is finished
         @return:
         """
 
-        drv, results = self.session.get_driver_results(sim.SimulationTypes.StochasticPowerFlow)
+        results = self.session.stochastic_power_flow
 
         if results is not None:
 
             self.remove_simulation(sim.SimulationTypes.StochasticPowerFlow)
 
             self.update_available_results()
 
@@ -1708,18 +1696,17 @@
 
     def post_cascade(self, idx=None):
         """
         Actions to perform after the cascade simulation is finished
         """
 
         # update the results in the circuit structures
-        drv, results = self.session.get_driver_results(sim.SimulationTypes.Cascade_run)
-
         self.remove_simulation(sim.SimulationTypes.Cascade_run)
 
+        results = self.session.cascade
         n = len(results.events)
 
         if n > 0:
 
             # display the last event, if none is selected
             if idx is None:
                 idx = n - 1
@@ -1798,15 +1785,15 @@
             areas_to = None
 
         ips_method = self.ips_solvers_dict[self.ui.ips_method_comboBox.currentText()]
         ips_tolerance = 1.0 / (10.0 ** self.ui.ips_tolerance_spinBox.value())
         ips_iterations = self.ui.ips_iterations_spinBox.value()
         ips_trust_radius = self.ui.ips_trust_radius_doubleSpinBox.value()
         ips_init_with_pf = self.ui.ips_initialize_with_pf_checkBox.isChecked()
-        pf_results = self.session.get_driver_results(SimulationTypes.PowerFlow_run)
+        pf_results = self.session.power_flow
 
         options = sim.OptimalPowerFlowOptions(solver=solver,
                                               time_grouping=time_grouping,
                                               zonal_grouping=zonal_grouping,
                                               mip_solver=mip_solver,
                                               power_flow_options=pf_options,
                                               consider_contingencies=consider_contingencies,
@@ -1859,15 +1846,15 @@
         else:
             pass
 
     def post_opf(self):
         """
         Actions to run after the OPF simulation
         """
-        drv, results = self.session.get_driver_results(sim.SimulationTypes.OPF_run)
+        results = self.session.optimal_power_flow
 
         if results is not None:
 
             self.remove_simulation(sim.SimulationTypes.OPF_run)
 
             if not results.converged:
                 warning_msg('Some islands did not solve.\n'
@@ -1928,15 +1915,15 @@
             pass
 
     def post_opf_time_series(self):
         """
         Post OPF Time Series
         """
 
-        drv, results = self.session.get_driver_results(sim.SimulationTypes.OPFTimeSeries_run)
+        results = self.session.optimal_power_flow_ts
 
         if results is not None:
 
             # expand the clusters
             results.expand_clustered_results()
 
             # remove from the current simulations
@@ -1957,20 +1944,20 @@
         """
         Copy the OPF generation values to the Time series object and execute a time series simulation
         """
         if len(self.circuit.buses) > 0:
 
             if self.circuit.time_profile is not None:
 
-                drv, results = self.session.get_driver_results(sim.SimulationTypes.OPFTimeSeries_run)
+                results = self.session.optimal_power_flow_ts
 
                 if results is not None:
 
-                    quit_msg = "Are you sure that you want overwrite the time events " \
-                               "with the simulated by the OPF time series?"
+                    quit_msg = ("Are you sure that you want overwrite the time events "
+                                "with the simulated by the OPF time series?")
                     reply = QtWidgets.QMessageBox.question(self, 'Message', quit_msg,
                                                            QtWidgets.QMessageBox.StandardButton.Yes,
                                                            QtWidgets.QMessageBox.StandardButton.No)
 
                     if reply == QtWidgets.QMessageBox.StandardButton.Yes:
 
                         results.apply_lp_profiles(self.circuit)
@@ -2068,15 +2055,15 @@
         else:
             pass
 
     def post_opf_ntc(self):
         """
         Actions to run after the OPF simulation
         """
-        drv, results = self.session.get_driver_results(sim.SimulationTypes.OPF_NTC_run)
+        results = self.session.optimal_net_transfer_capacity
 
         if results is not None:
             self.remove_simulation(sim.SimulationTypes.OPF_NTC_run)
             self.update_available_results()
             self.colour_diagrams()
 
         if not self.session.is_anything_running():
@@ -2120,15 +2107,15 @@
             pass
 
     def post_opf_ntc_ts(self):
         """
         Actions to run after the optimal net transfer capacity time series simulation
         """
 
-        drv, results = self.session.get_driver_results(sim.SimulationTypes.OPF_NTC_TS_run)
+        results = self.session.optimal_net_transfer_capacity_ts
 
         if results is not None:
 
             # expand the clusters
             results.expand_clustered_results()
 
             # remove from the current simulations
@@ -2147,15 +2134,15 @@
 
     def run_find_node_groups(self):
         """
         Run the node groups algorithm
         """
         if self.ui.actionFind_node_groups.isChecked():
 
-            drv, ptdf_results = self.session.get_driver_results(sim.SimulationTypes.LinearAnalysis_run)
+            ptdf_results = self.session.linear_power_flow
 
             if ptdf_results is not None:
 
                 self.LOCK()
                 sigmas = self.ui.node_distances_sigma_doubleSpinBox.value()
                 min_group_size = self.ui.node_distances_elements_spinBox.value()
                 drv = sim.NodeGroupsDriver(grid=self.circuit,
@@ -2179,15 +2166,15 @@
         """
         Colour the grid after running the node grouping
         :return:
         """
         self.UNLOCK()
         print('\nGroups:')
 
-        drv, results = self.session.get_driver_results(sim.SimulationTypes.NodeGrouping_run)
+        drv, _ = self.session.node_groups_driver
 
         if drv is not None:
 
             for group in drv.groups_by_name:
                 print(group)
 
             colours = viz.get_n_colours(n=len(drv.groups_by_index))
@@ -2232,15 +2219,15 @@
             pass
 
     def post_inputs_analysis(self):
         """
 
         :return:
         """
-        drv, results = self.session.get_driver_results(sim.SimulationTypes.InputsAnalysis_run)
+        results = self.session.inputs_analysis
 
         if results is not None:
             self.remove_simulation(sim.SimulationTypes.InputsAnalysis_run)
             self.update_available_results()
             self.colour_diagrams()
 
         if not self.session.is_anything_running():
@@ -2251,15 +2238,15 @@
         Add storage markers to the schematic
         """
 
         if len(self.circuit.buses) > 0:
 
             if self.ui.actionStorage_location_suggestion.isChecked():
 
-                ts_drv, ts_results = self.session.get_driver_results(sim.SimulationTypes.TimeSeries_run)
+                ts_results = self.session.power_flow_ts
 
                 if ts_results is not None:
 
                     # perform a time series analysis
                     ts_analysis = grid_analysis.TimeSeriesResultsAnalysis(self.circuit, ts_results)
 
                     # get the indices of the buses selected for storage
@@ -2372,19 +2359,19 @@
         else:
             pass
 
     def post_run_investments_evaluation(self) -> None:
         """
         Post investments evaluation
         """
-        drv, results = self.session.get_driver_results(sim.SimulationTypes.InvestmestsEvaluation_run)
-        self.remove_simulation(sim.SimulationTypes.InvestmestsEvaluation_run)
+        results = self.session.investments_evaluation
 
         # update the results in the circuit structures
         if results is not None:
+            self.remove_simulation(sim.SimulationTypes.InvestmestsEvaluation_run)
 
             self.ui.progress_label.setText('Colouring investments evaluation results in the grid...')
             QtGui.QGuiApplication.processEvents()
 
             self.update_available_results()
             self.colour_diagrams()
         else:
@@ -2395,15 +2382,15 @@
 
     def get_clustering_results(self) -> Union[sim.ClusteringResults, None]:
         """
         Get the clustering results if available
         :return: ClusteringResults or None
         """
         if self.ui.actionUse_clustering.isChecked():
-            _, clustering_results = self.session.get_driver_results(sim.SimulationTypes.ClusteringAnalysis_run)
+            clustering_results = self.session.clustering
 
             if clustering_results is not None:
                 n = len(clustering_results.time_indices)
 
                 if n != self.ui.cluster_number_spinBox.value():
                     error_msg("The number of clusters in the stored results is different from the specified :(\n"
                               "Run another clustering analysis.")
@@ -2461,16 +2448,17 @@
     def post_clustering(self):
         """
         Action performed after the short circuit.
         Returns:
 
         """
         # update the results in the circuit structures
-        drv, results = self.session.get_driver_results(sim.SimulationTypes.ClusteringAnalysis_run)
         self.remove_simulation(sim.SimulationTypes.ClusteringAnalysis_run)
+
+        results = self.session.clustering
         if results is not None:
 
             self.update_available_results()
         else:
             error_msg('Something went wrong, There are no power short circuit results.')
 
         if not self.session.is_anything_running():
@@ -2532,15 +2520,15 @@
         """
         When activating the use of clustering, also activate time series
         :return:
         """
         if self.ui.actionUse_clustering.isChecked():
 
             # check if there are clustering results yet
-            _, clustering_results = self.session.get_driver_results(sim.SimulationTypes.ClusteringAnalysis_run)
+            clustering_results = self.session.clustering
 
             if clustering_results is not None:
                 n = len(clustering_results.time_indices)
 
                 if n != self.ui.cluster_number_spinBox.value():
                     error_msg("The number of clusters in the stored results is different from the specified :(\n"
                               "Run another clustering analysis.")
```

### Comparing `GridCal-5.1.6/GridCal/Gui/Main/SubClasses/io.py` & `GridCal-5.1.7/GridCal/Gui/Main/SubClasses/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from GridCal.Gui.RosetaExplorer.RosetaExplorer import RosetaExplorerGUI
 from GridCal.Gui.Main.SubClasses.Settings.configuration import ConfigurationMain
 
 from GridCalEngine.Compilers.circuit_to_newton_pa import NEWTON_PA_AVAILABLE
 from GridCalEngine.Compilers.circuit_to_pgm import PGM_AVAILABLE
 from GridCalEngine.IO.gridcal.contingency_parser import import_contingencies_from_json, export_contingencies_json_file
 from GridCalEngine.DataStructures.numerical_circuit import compile_numerical_circuit_at
+from GridCalEngine.enumerations import CGMESVersions
 
 
 class IoMain(ConfigurationMain):
     """
     Inputs-Outputs Main
     """
 
@@ -56,14 +57,17 @@
         self.rosetta_gui: Union[RosetaExplorerGUI, None] = None
 
         self.accepted_extensions = ['.gridcal', '.xlsx', '.xls', '.sqlite', '.gch5',
                                     '.dgs', '.m', '.raw', '.RAW', '.json',
                                     '.ejson2', '.ejson3',
                                     '.xml', '.rawx', '.zip', '.dpx', '.epc']
 
+        self.cgmes_version_dict = {x.value: x for x in [CGMESVersions.v2_4_15, CGMESVersions.v3_0_0]}
+        self.ui.cgmes_version_comboBox.setModel(gf.get_list_model(list(self.cgmes_version_dict.keys())))
+
         self.ui.actionNew_project.triggered.connect(self.new_project)
         self.ui.actionOpen_file.triggered.connect(self.open_file)
         self.ui.actionAdd_circuit.triggered.connect(self.add_circuit)
         self.ui.actionSave.triggered.connect(self.save_file)
         self.ui.actionSave_as.triggered.connect(self.save_file_as)
         self.ui.actionExport_all_the_device_s_profiles.triggered.connect(self.export_object_profiles)
         self.ui.actionExport_all_results.triggered.connect(self.export_all)
@@ -514,25 +518,28 @@
     def get_file_save_options(self) -> filedrv.FileSavingOptions:
         """
         Compose the file saving options
         :return: FileSavingOptions
         """
 
         if self.ui.saveResultsCheckBox.isChecked():
-            sessions = [self.session]
+            sessions_data = self.session.get_save_data()
         else:
-            sessions = list()
+            sessions_data = list()
 
         # get json files to store
         json_files = {"gui_config": self.get_gui_config_data()}
 
+        cgmes_version = self.cgmes_version_dict[self.ui.cgmes_version_comboBox.currentText()]
+
         options = filedrv.FileSavingOptions(cgmes_boundary_set=self.current_boundary_set,
                                             simulation_drivers=self.get_simulations(),
-                                            sessions=sessions,
-                                            dictionary_of_json_files=json_files)
+                                            sessions_data=sessions_data,
+                                            dictionary_of_json_files=json_files,
+                                            cgmes_version=cgmes_version)
 
         return options
 
     def save_file_now(self, filename):
         """
         Save the file right now, without questions
         :param filename: filename to save to
@@ -755,18 +762,20 @@
             item = tree_mdl.itemFromIndex(idx[0])
             path = gf.get_tree_item_path(item)
 
             if len(path) > 1:
                 session_name = path[0]
                 study_name = path[1]
                 if self.last_file_driver is not None:
-                    data_dict, json_files = self.last_file_driver.load_session_objects(session_name=session_name,
-                                                                                       study_name=study_name)
+                    data_dict = self.last_file_driver.load_session_objects(session_name=session_name,
+                                                                           study_name=study_name)
 
-                    self.session.register_driver_from_disk_data(self.circuit, study_name, data_dict)
+                    self.session.register_driver_from_disk_data(grid=self.circuit,
+                                                                study_name=study_name,
+                                                                data_dict=data_dict)
 
                     self.update_available_results()
                 else:
                     error_msg('No file driver declared :/')
             else:
                 info_msg('Select a driver inside a session', 'Driver load from disk')
```

### Comparing `GridCal-5.1.6/GridCal/Gui/Main/SubClasses/base_gui.py` & `GridCal-5.1.7/GridCal/Gui/Main/SubClasses/base_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -646,15 +646,15 @@
         """
         Rate the Branches that do not have rate
         """
 
         branches = self.circuit.get_branches()
 
         if len(branches) > 0:
-            pf_drv, pf_results = self.session.get_driver_results(sim.SimulationTypes.PowerFlow_run)
+            pf_results = self.session.power_flow()
 
             if pf_results is not None:
                 factor = self.ui.branch_rating_doubleSpinBox.value()
 
                 for i, branch in enumerate(branches):
 
                     S = pf_results.Sf[i]
```

### Comparing `GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Scripting/python_highlighter.py` & `GridCal-5.1.7/GridCal/Gui/Main/SubClasses/Scripting/python_highlighter.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Scripting/scripting.py` & `GridCal-5.1.7/GridCal/Gui/Main/SubClasses/Scripting/scripting.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Settings/configuration.py` & `GridCal-5.1.7/GridCal/Gui/Main/SubClasses/Settings/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,15 +289,16 @@
                 "srap_deadband": self.ui.srap_deadband_doubleSpinBox,
                 "contingency_deadband": self.ui.contingency_deadband_SpinBox,
                 "srap_revert_to_nominal_rating": self.ui.srap_revert_to_nominal_rating_checkBox,
                 "contingency_massive_report": self.ui.contingency_detailed_massive_report_checkBox
             },
             "file": {
                 "store_results_in_file": self.ui.saveResultsCheckBox,
-                "current_boundary_set": self.current_boundary_set
+                "current_boundary_set": self.current_boundary_set,
+                "cgmes_selected_version": self.ui.cgmes_version_comboBox
             }
         }
 
     def get_gui_config_data(self) -> Dict[str, Dict[str, Union[float, int, str, bool]]]:
         """
         Get a dictionary with the GUI configuration data
         :return:
```

### Comparing `GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Model/objects.py` & `GridCal-5.1.7/GridCal/Gui/Main/SubClasses/Model/objects.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Model/time_events.py` & `GridCal-5.1.7/GridCal/Gui/Main/SubClasses/Model/time_events.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Model/diagrams.py` & `GridCal-5.1.7/GridCal/Gui/Main/SubClasses/Model/diagrams.py`

 * *Files 0% similar despite different names*

```diff
@@ -645,15 +645,15 @@
                                      max_branch_width=max_branch_width,
                                      min_bus_width=min_bus_width,
                                      max_bus_width=max_bus_width,
                                      cmap=cmap)
             else:
                 info_msg(f"{current_study} only has values for the snapshot")
 
-        elif current_study == sim.ContingencyAnalysisTimeSeries.tpe.value:
+        elif current_study == sim.ContingencyAnalysisTimeSeriesDriver.tpe.value:
             if t_idx is not None:
                 results: sim.ContingencyAnalysisTimeSeriesResults = self.session.get_results(
                     sim.SimulationTypes.ContingencyAnalysisTS_run)
                 bus_active = [bus.active_prof[t_idx] for bus in self.circuit.buses]
                 br_active = [br.active_prof[t_idx] for br in self.circuit.get_branches_wo_hvdc()]
                 hvdc_active = [hvdc.active_prof[t_idx] for hvdc in self.circuit.hvdc_lines]
```

### Comparing `GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Model/compiled_arrays.py` & `GridCal-5.1.7/GridCal/Gui/Main/SubClasses/Model/compiled_arrays.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Main/SubClasses/Results/results.py` & `GridCal-5.1.7/GridCal/Gui/Main/SubClasses/Results/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,15 +293,15 @@
                     self.session.delete_driver_by_name(study_name)
                     self.update_available_results()
 
     def copy_opf_to_profiles(self):
         """
         Copy the results from the OPF time series to the profiles
         """
-        drv, results = self.session.get_driver_results(sim.SimulationTypes.OPFTimeSeries_run)
+        results = self.session.optimal_power_flow_ts
 
         if results is not None:
 
             reply = QtWidgets.QMessageBox.question(self, 'Message',
                                                    'Are you sure that you want to overwrite '
                                                    'the generation profiles with the OPF results?',
                                                    QtWidgets.QMessageBox.StandardButton.Yes,
```

### Comparing `GridCal-5.1.6/GridCal/Gui/Visualization/visualization.py` & `GridCal-5.1.7/GridCal/Gui/Visualization/visualization.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/Visualization/palettes.py` & `GridCal-5.1.7/GridCal/Gui/Visualization/palettes.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/SyncDialogue/icons_rc.py` & `GridCal-5.1.7/GridCal/Gui/SyncDialogue/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/SyncDialogue/sync_dialogue.py` & `GridCal-5.1.7/GridCal/Gui/SyncDialogue/sync_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/SyncDialogue/gui.py` & `GridCal-5.1.7/GridCal/Gui/SyncDialogue/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/SolarPowerWizard/solar_power_wizzard.py` & `GridCal-5.1.7/GridCal/Gui/SolarPowerWizard/solar_power_wizzard.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/SolarPowerWizard/icons_rc.py` & `GridCal-5.1.7/GridCal/Gui/SolarPowerWizard/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/SolarPowerWizard/gui.py` & `GridCal-5.1.7/GridCal/Gui/SolarPowerWizard/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/RosetaExplorer/MainWindow.py` & `GridCal-5.1.7/GridCal/Gui/RosetaExplorer/MainWindow.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/RosetaExplorer/update_gui_file.py` & `GridCal-5.1.7/GridCal/Gui/RosetaExplorer/update_gui_file.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/RosetaExplorer/RosetaExplorer.py` & `GridCal-5.1.7/GridCal/Gui/RosetaExplorer/RosetaExplorer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/RosetaExplorer/ConsoleWidget.py` & `GridCal-5.1.7/GridCal/Gui/RosetaExplorer/ConsoleWidget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/RosetaExplorer/icons_rc.py` & `GridCal-5.1.7/GridCal/Gui/RosetaExplorer/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/LoadDesigner/load_designer.py` & `GridCal-5.1.7/GridCal/Gui/LoadDesigner/load_designer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/LoadDesigner/icons_rc.py` & `GridCal-5.1.7/GridCal/Gui/LoadDesigner/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/LoadDesigner/load_designer_ui.py` & `GridCal-5.1.7/GridCal/Gui/LoadDesigner/load_designer_ui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/WindPowerWizard/wind_power_wizzard.py` & `GridCal-5.1.7/GridCal/Gui/WindPowerWizard/wind_power_wizzard.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/WindPowerWizard/icons_rc.py` & `GridCal-5.1.7/GridCal/Gui/WindPowerWizard/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/WindPowerWizard/gui.py` & `GridCal-5.1.7/GridCal/Gui/WindPowerWizard/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/SystemScaler/system_scaler.py` & `GridCal-5.1.7/GridCal/Gui/SystemScaler/system_scaler.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/SystemScaler/icons_rc.py` & `GridCal-5.1.7/GridCal/Gui/SystemScaler/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/SystemScaler/system_scaler_ui.py` & `GridCal-5.1.7/GridCal/Gui/SystemScaler/system_scaler_ui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/TreeModelViewer/MainWindow.py` & `GridCal-5.1.7/GridCal/Gui/TreeModelViewer/MainWindow.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/TreeModelViewer/update_gui_file.py` & `GridCal-5.1.7/GridCal/Gui/TreeModelViewer/update_gui_file.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/TreeModelViewer/icons_rc.py` & `GridCal-5.1.7/GridCal/Gui/TreeModelViewer/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/TreeModelViewer/TreeModelViewer.py` & `GridCal-5.1.7/GridCal/Gui/TreeModelViewer/TreeModelViewer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/SigmaAnalysis/icons_rc.py` & `GridCal-5.1.7/GridCal/Gui/SigmaAnalysis/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/SigmaAnalysis/gui.py` & `GridCal-5.1.7/GridCal/Gui/SigmaAnalysis/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/SigmaAnalysis/sigma_analysis_dialogue.py` & `GridCal-5.1.7/GridCal/Gui/SigmaAnalysis/sigma_analysis_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/GridGenerator/grid_generator_dialogue.py` & `GridCal-5.1.7/GridCal/Gui/GridGenerator/grid_generator_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/GridGenerator/icons_rc.py` & `GridCal-5.1.7/GridCal/Gui/GridGenerator/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/GridCal/Gui/GridGenerator/gui.py` & `GridCal-5.1.7/GridCal/Gui/GridGenerator/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/setup.py` & `GridCal-5.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.6/PKG-INFO` & `GridCal-5.1.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GridCal
-Version: 5.1.6
+Version: 5.1.7
 Summary: GridCal is a Power Systems simulation program intended for professional use and research
 Home-page: https://github.com/SanPen/GridCal
 Author: Santiago Peñate Vera et. Al.
 Author-email: santiago@gridcal.org
 License: LGPL
 Keywords: power systems planning
 Classifier:  License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
```

