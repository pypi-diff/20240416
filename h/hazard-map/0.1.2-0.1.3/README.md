# Comparing `tmp/hazard_map-0.1.2.tar.gz` & `tmp/hazard_map-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hazard_map-0.1.2.tar", max compression
+gzip compressed data, was "hazard_map-0.1.3.tar", max compression
```

## Comparing `hazard_map-0.1.2.tar` & `hazard_map-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      553 2024-04-15 15:19:20.736333 hazard_map-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1074 2024-04-15 14:10:28.660232 hazard_map-0.1.2/readme.md
--rw-r--r--   0        0        0     2031 2024-04-15 15:19:43.263377 hazard_map-0.1.2/src/hazard_map/__init__.py
--rw-r--r--   0        0        0     8809 2024-04-15 15:11:39.828436 hazard_map-0.1.2/src/hazard_map/hazard_map.py
--rw-r--r--   0        0        0     1826 1970-01-01 00:00:00.000000 hazard_map-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     9755 2024-04-16 15:59:57.751998 hazard_map-0.1.3/hazard_map/hazard_map.py
+-rw-r--r--   0        0        0     2061 2024-04-16 16:02:56.085637 hazard_map-0.1.3/hazard_map/main.py
+-rw-r--r--   0        0        0      587 2024-04-16 16:02:08.072015 hazard_map-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1654 2024-04-16 15:59:15.366899 hazard_map-0.1.3/readme.md
+-rw-r--r--   0        0        0     2382 1970-01-01 00:00:00.000000 hazard_map-0.1.3/PKG-INFO
```

### Comparing `hazard_map-0.1.2/pyproject.toml` & `hazard_map-0.1.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 [tool.poetry]
 name = "hazard-map"
-version = "0.1.2"
+version = "0.1.3"
 description = "Build and analyze a network model of hazards, causes, and controls"
 authors = ["Thom Cameron <thomcm@proton.me>"]
 readme = "readme.md"
 license = "license.txt"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-argparse = "^1.4.0"
-numpy = "^1.26.4"
-pandas = "^2.2.1"
-openpyxl = "^3.1.2"
+argparse = "^1.4"
+numpy = "^1.26"
+pandas = "^2.2"
+openpyxl = "^3.1"
 networkx = "^3.3"
-scipy = "^1.13.0"
-matplotlib = "^3.8.4"
+scipy = "^1.13"
+matplotlib = "^3.8"
+
+[tool.poetry.dev-dependencies]
+pytest = "^8.1.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-hazard-map = "hazard_map.__init__:main"
+hazard-map = "hazard_map.main:main"
```

### Comparing `hazard_map-0.1.2/src/hazard_map/__init__.py` & `hazard_map-0.1.3/hazard_map/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 import argparse
-# from hazard_map import HazardMap, Sheet
-from hazard_map.hazard_map import HazardMap, Sheet
 
-DEFAULT_OUTPUT_DIR = './hazard-log'
+from hazard_map.hazard_map import HazardMap, Sheet
 
 def main():
+    arguments = parse_arguments()
+
     print('Welcome to hazard-map!')
 
     print()
     
-    arguments = parse_arguments()
-
-    if arguments.output_directory:
-        if arguments.output_directory[-1] == '/': 
-            arguments.output_directory = arguments.output_directory[:-1]
-        output_directory = arguments.output_directory
-    else:
-        output_directory = DEFAULT_OUTPUT_DIR
+    if arguments.output_directory[-1] in ('/', '\\'): 
+        arguments.output_directory = arguments.output_directory[:-1]
     print(f'The ourputs of this script will be saved in the following directory:')
-    print(output_directory)
+    print(arguments.output_directory)
 
     print()
 
     hazard_log = HazardMap(arguments.input_workbook)
 
     graph = hazard_log.extract_sheet_mappings([
         Sheet('HazardCause Mapping', (0, 0), (1, 1), (2, 2), False),
         Sheet('CauseControl Mapping', (0, 0), (1, 1), (2, 2), False),
     ])
-    print('Mappings were successfully extracted from the workbook!')
+    print(f'Mappings were successfully extracted from the workbook "{arguments.input_workbook}"!')
 
     print()
 
-    hazard_log_output_file = hazard_log.write_to_file(output_directory)
-    print(f'Wrote the mappings in the hazard log format to "{hazard_log_output_file}"')
+    hazard_log_output_file = hazard_log.write_to_file(
+        arguments.output_directory, 
+        arguments.output_json,
+    )
 
     hazard_log.draw_graph()
-    plot_output_file = hazard_log.save_graph(output_directory, arguments.plot_dpi)
+    plot_output_file = hazard_log.save_graph(arguments.output_directory, arguments.plot_dpi)
     print(f'Saved a plot of the network to "{plot_output_file}"')
 
 def parse_arguments():
     parser = argparse.ArgumentParser(
         prog='hazard-map',
         description='Build and analyze a network model of hazards, causes, and controls',
     )
@@ -48,23 +44,31 @@
     parser.add_argument(
         'input_workbook',
         help='The hazard mapping excel file to evaluate',
     )
 
     parser.add_argument(
         '-o', '--output-directory',
-        help='Set a custom directory for the script to save its outputs to',
-        default=None,
+        help='Set a directory for the script to save its outputs to',
+        default='hazard-log',
         type=str,
     )
 
     parser.add_argument(
         '-d', '--plot-dpi',
         help='Set a custom DPI (quality) for the plot output',
         default=None,
         type=int,
     )
 
+    parser.add_argument(
+        '-j', '--output-json',
+        help='Save a json description of the mappings alongside the hazard log',
+        default=False,
+        type=bool,
+        action=argparse.BooleanOptionalAction,
+    )
+
     return parser.parse_args()
 
 if __name__ == '__main__':
     main()
```

### Comparing `hazard_map-0.1.2/src/hazard_map/hazard_map.py` & `hazard_map-0.1.3/hazard_map/hazard_map.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import io
 import os
 import re
 from enum import Enum
 from dataclasses import dataclass
 import functools
+import json
 
 import numpy as np
 import pandas as pd
 import networkx as nx
 from matplotlib import pyplot as plt
 
 
@@ -43,20 +44,19 @@
             int(match['number']),
         )
 
     def __lt__(self, other) -> bool:
         self.number < other.number
 
 
-DEFAULT_OUTPUT_DIR = './hazard-log'
 ZERO_PADDING_DIGITS = 2
 DEFAULT_RENDERING_DPI = 480
 
 NODE_MATCHER = re.compile(r'^(?P<kind>H|CA|CO)-?(?P<number>\d+)$')
-MAPPING_MATCHER = re.compile('^\s*[Y]\s*$', re.I)
+MAPPING_MATCHER = re.compile(r'^\s*[Y]\s*$', re.I)
 
 KIND_STR_DICT = {
     'H': Kind.HAZARD,
     'CA': Kind.CAUSE,
     'CO': Kind.CONTROL,
 }
 
@@ -92,15 +92,15 @@
 
             df.apply(self._extract_individual_mappings, axis=1)
 
     def _extract_clean_mappings(self, df: pd.DataFrame, sheet: Sheet) -> pd.DataFrame:
         # find out what size the mapping table is (i.e. how many pairs are in the table)
         def find_list_length(s: pd.Series) -> int:
             for i, item in enumerate(s): 
-                if item in [0, np.nan]: break
+                if item in [0, np.nan, '']: break
             return i
         table_dimensions = tuple([
             find_list_length(name_list)
             for name_list, axis in zip(
                 (
                     df.iloc[sheet.name_list_locations[1], sheet.mapping_table_location[0]:], 
                     df.iloc[sheet.mapping_table_location[1]:, sheet.name_list_locations[0]],
@@ -123,22 +123,18 @@
 
         row = row.dropna()
         mapped = row[row.str.match(MAPPING_MATCHER)].index.str.strip().to_list()
         mapped_typed = [Node.from_str(node_str) for node_str in mapped]
         
         for map_to in mapped_typed: self.graph.add_edge(map_from, map_to)
 
-    def write_to_file(self, custom_output_location: str=None) -> str:
-        output_directory = (
-            custom_output_location if custom_output_location 
-            else DEFAULT_OUTPUT_DIR
-        )
+    def write_to_file(self, output_directory: str, output_json: bool=False) -> str:
         if not os.path.exists(output_directory): os.system(f'mkdir {output_directory}')
-        output_file = f'{output_directory}/{self.WORKBOOK_NAME}-hazard_log_format.xlsx'
-        
+        output_file = f'{output_directory}/{self.WORKBOOK_NAME}-hazard_log.xlsx'
+
         with pd.ExcelWriter(output_file) as writer:
             for hazard in self.filter_node_set_for_kind(
                 self.graph.nodes, 
                 Kind.HAZARD,
             ):
                 cause_control_mappings = []
                 for cause in self.filter_node_set_for_kind(
@@ -146,25 +142,61 @@
                     Kind.CAUSE,
                 ):
                     for control in self.filter_node_set_for_kind(
                         self.graph[cause], 
                         Kind.CONTROL,
                     ):
                         cause_control_mappings.append((cause.to_str(), control.to_str()))
+
                 df = (
                     pd.DataFrame(
                         data=cause_control_mappings, 
                         columns=['cause', 'control'],
                     )
                     .set_index('cause', append=True)
                     .reorder_levels([1, 0])
-                    .to_excel(writer, sheet_name=hazard.to_str())
                 )
+                df.to_excel(writer, sheet_name=hazard.to_str())
+            print(
+                'Wrote the mappings in the hazard log format to '
+                f'\"{os.path.basename(output_file)}\"'
+            )
+
+        if output_json:
+            json_file = f'{output_directory}/{self.WORKBOOK_NAME}-mappings.json'
+            json_mappings = self._create_json_description()
+            with open(json_file, 'w') as f:
+                f.write(json_mappings)
+            print(
+                'Created a json description of the mappings in '
+                f'\"{os.path.basename(json_file)}\"'
+            )
 
-        return os.path.basename(output_file)
+    def _create_json_description(self) -> str:
+        mapping_dict = {}
+
+        for hazard in self.filter_node_set_for_kind(
+            self.graph.nodes, 
+            Kind.HAZARD,
+        ):
+            mapping_dict[hazard.to_str()] = {}
+
+            for cause in self.filter_node_set_for_kind(
+                self.graph[hazard], 
+                Kind.CAUSE,
+            ):
+                mapping_dict[hazard.to_str()][cause.to_str()] = []
+
+                for control in self.filter_node_set_for_kind(
+                    self.graph[cause], 
+                    Kind.CONTROL,
+                ):
+                    mapping_dict[hazard.to_str()][cause.to_str()].append(control.to_str())
+
+        return json.dumps(mapping_dict, indent=2)
 
     def filter_node_set_for_kind(self, node_set: set, kind: Kind) -> list[Node]:
         return sorted([node for node in node_set if node.kind == kind])
 
     def draw_graph(self, custom_dpi: int=None) -> (plt.Figure, plt.Axes):        
         self.fig, self.ax = plt.subplots(
             frameon=False,
@@ -203,22 +235,18 @@
             min([
                 size_limits[0] + add_size_per_connect*n_connections,
                 size_limits[1],
             ])
             for node, n_connections in degrees
         ]
 
-    def save_graph(self, custom_output_location: str=None, custom_dpi: int=None) -> str: 
+    def save_graph(self, output_directory: str, custom_dpi: int=None) -> str: 
         if not hasattr(self, 'fig'):
             self.draw_graph()
 
-        output_directory = (
-            custom_output_location if custom_output_location 
-            else DEFAULT_OUTPUT_DIR
-        )
         if not os.path.exists(output_directory): os.system(f'mkdir {output_directory}')
         output_file = f'{output_directory}/{self.WORKBOOK_NAME}-graph_rendering.png'
 
         plt.savefig(
             output_file, 
             transparent=True, 
             dpi=DEFAULT_RENDERING_DPI if not custom_dpi else custom_dpi,
```

