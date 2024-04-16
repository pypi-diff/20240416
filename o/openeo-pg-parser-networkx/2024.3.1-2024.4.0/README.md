# Comparing `tmp/openeo_pg_parser_networkx-2024.3.1.tar.gz` & `tmp/openeo_pg_parser_networkx-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openeo_pg_parser_networkx-2024.3.1.tar", max compression
+gzip compressed data, was "openeo_pg_parser_networkx-2024.4.0.tar", max compression
```

## Comparing `openeo_pg_parser_networkx-2024.3.1.tar` & `openeo_pg_parser_networkx-2024.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    10765 2024-03-05 13:56:22.087912 openeo_pg_parser_networkx-2024.3.1/LICENSE
--rw-r--r--   0        0        0     5886 2024-03-05 13:56:22.087912 openeo_pg_parser_networkx-2024.3.1/README.md
--rw-r--r--   0        0        0      241 2024-03-05 13:56:22.091913 openeo_pg_parser_networkx-2024.3.1/openeo_pg_parser_networkx/__init__.py
--rw-r--r--   0        0        0    19598 2024-03-05 13:56:22.091913 openeo_pg_parser_networkx-2024.3.1/openeo_pg_parser_networkx/graph.py
--rw-r--r--   0        0        0    10036 2024-03-05 13:56:22.091913 openeo_pg_parser_networkx-2024.3.1/openeo_pg_parser_networkx/pg_schema.py
--rw-r--r--   0        0        0     5125 2024-03-05 13:56:22.091913 openeo_pg_parser_networkx-2024.3.1/openeo_pg_parser_networkx/process_registry.py
--rw-r--r--   0        0        0    11440 2024-03-05 13:56:22.091913 openeo_pg_parser_networkx-2024.3.1/openeo_pg_parser_networkx/resolving_utils.py
--rw-r--r--   0        0        0    10738 2024-03-05 13:56:22.091913 openeo_pg_parser_networkx-2024.3.1/openeo_pg_parser_networkx/utils.py
--rw-r--r--   0        0        0     1590 2024-03-05 13:56:22.091913 openeo_pg_parser_networkx-2024.3.1/pyproject.toml
--rw-r--r--   0        0        0     7170 1970-01-01 00:00:00.000000 openeo_pg_parser_networkx-2024.3.1/PKG-INFO
+-rw-r--r--   0        0        0    10765 2024-04-16 13:48:34.049644 openeo_pg_parser_networkx-2024.4.0/LICENSE
+-rw-r--r--   0        0        0     5886 2024-04-16 13:48:34.053644 openeo_pg_parser_networkx-2024.4.0/README.md
+-rw-r--r--   0        0        0      241 2024-04-16 13:48:34.053644 openeo_pg_parser_networkx-2024.4.0/openeo_pg_parser_networkx/__init__.py
+-rw-r--r--   0        0        0    19598 2024-04-16 13:48:34.053644 openeo_pg_parser_networkx-2024.4.0/openeo_pg_parser_networkx/graph.py
+-rw-r--r--   0        0        0    10036 2024-04-16 13:48:34.053644 openeo_pg_parser_networkx-2024.4.0/openeo_pg_parser_networkx/pg_schema.py
+-rw-r--r--   0        0        0     5125 2024-04-16 13:48:34.053644 openeo_pg_parser_networkx-2024.4.0/openeo_pg_parser_networkx/process_registry.py
+-rw-r--r--   0        0        0    11644 2024-04-16 13:48:34.053644 openeo_pg_parser_networkx-2024.4.0/openeo_pg_parser_networkx/resolving_utils.py
+-rw-r--r--   0        0        0    10738 2024-04-16 13:48:34.053644 openeo_pg_parser_networkx-2024.4.0/openeo_pg_parser_networkx/utils.py
+-rw-r--r--   0        0        0     1590 2024-04-16 13:48:34.057644 openeo_pg_parser_networkx-2024.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7170 1970-01-01 00:00:00.000000 openeo_pg_parser_networkx-2024.4.0/PKG-INFO
```

### Comparing `openeo_pg_parser_networkx-2024.3.1/LICENSE` & `openeo_pg_parser_networkx-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openeo_pg_parser_networkx-2024.3.1/README.md` & `openeo_pg_parser_networkx-2024.4.0/README.md`

 * *Files identical despite different names*

### Comparing `openeo_pg_parser_networkx-2024.3.1/openeo_pg_parser_networkx/graph.py` & `openeo_pg_parser_networkx-2024.4.0/openeo_pg_parser_networkx/graph.py`

 * *Files identical despite different names*

### Comparing `openeo_pg_parser_networkx-2024.3.1/openeo_pg_parser_networkx/pg_schema.py` & `openeo_pg_parser_networkx-2024.4.0/openeo_pg_parser_networkx/pg_schema.py`

 * *Files identical despite different names*

### Comparing `openeo_pg_parser_networkx-2024.3.1/openeo_pg_parser_networkx/process_registry.py` & `openeo_pg_parser_networkx-2024.4.0/openeo_pg_parser_networkx/process_registry.py`

 * *Files identical despite different names*

### Comparing `openeo_pg_parser_networkx-2024.3.1/openeo_pg_parser_networkx/resolving_utils.py` & `openeo_pg_parser_networkx-2024.4.0/openeo_pg_parser_networkx/resolving_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,18 +227,22 @@
     "Rewires" the from_parameter connections of filled in UDPs to be consistent with
     the parameters available from parent nodes.
     '''
     if len(arguments) > 0:
         for node_key, node in process_graph[process_replacement_id].items():
             for arg_key, from_param in node['arguments'].items():
                 # Find from_parameter value in arguments list and replace with arguments[from_parameter value] value
-                if "from_parameter" in from_param:
+                if isinstance(from_param, dict) and "from_parameter" in from_param:
                     process_graph[process_replacement_id][node_key]['arguments'][
                         arg_key
                     ] = arguments[from_param['from_parameter']]
+                else:
+                    process_graph[process_replacement_id][node_key]['arguments'][
+                        arg_key
+                    ] = from_param
 
 
 def _adjust_references(input_graph):
     '''
     "Rewires" the from_node connections of filled in UDPs to be consistent with
     the nodes available on the level of the parent nodes.
```

### Comparing `openeo_pg_parser_networkx-2024.3.1/openeo_pg_parser_networkx/utils.py` & `openeo_pg_parser_networkx-2024.4.0/openeo_pg_parser_networkx/utils.py`

 * *Files identical despite different names*

### Comparing `openeo_pg_parser_networkx-2024.3.1/pyproject.toml` & `openeo_pg_parser_networkx-2024.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openeo-pg-parser-networkx"
-version = "2024.3.1"
+version = "2024.4.0"
 
 description = "Parse OpenEO process graphs from JSON to traversible Python objects."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>", "Sean Hoyal <sean.hoyal@eodc.eu>", "Valentina Hutter <valentina.hutter@eodc.eu>", "Gerald Irsiegler <gerald.irsiegler@eodc.eu>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/Open-EO/openeo-pg-parser-networkx"
 classifiers = [
```

### Comparing `openeo_pg_parser_networkx-2024.3.1/PKG-INFO` & `openeo_pg_parser_networkx-2024.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openeo-pg-parser-networkx
-Version: 2024.3.1
+Version: 2024.4.0
 Summary: Parse OpenEO process graphs from JSON to traversible Python objects.
 Home-page: https://github.com/Open-EO/openeo-pg-parser-networkx
 License: Apache 2.0
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 4 - Beta
```

