# Comparing `tmp/sampy-abm-1.0.2.tar.gz` & `tmp/sampy_abm-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sampy-abm-1.0.2.tar", last modified: Thu Jun 22 17:10:02 2023, max compression
+gzip compressed data, was "sampy_abm-1.0.3.tar", last modified: Tue Apr 16 19:33:08 2024, max compression
```

## Comparing `sampy-abm-1.0.2.tar` & `sampy_abm-1.0.3.tar`

### file list

```diff
@@ -1,90 +1,96 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.535132 sampy-abm-1.0.2/
--rw-rw-rw-   0        0        0    35149 2023-06-07 19:00:29.000000 sampy-abm-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      823 2023-06-22 17:10:02.535132 sampy-abm-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      413 2023-06-22 17:08:16.000000 sampy-abm-1.0.2/README.md
--rw-rw-rw-   0        0        0      632 2023-06-22 17:08:14.000000 sampy-abm-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 17:10:02.536101 sampy-abm-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.393054 sampy-abm-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.412281 sampy-abm-1.0.2/src/sampy/
--rw-rw-rw-   0        0        0      106 2023-06-22 17:07:25.000000 sampy-abm-1.0.2/src/sampy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.414271 sampy-abm-1.0.2/src/sampy/addons/
-drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.423384 sampy-abm-1.0.2/src/sampy/addons/ORM_related_addons/
--rw-rw-rw-   0        0        0    32933 2023-06-22 17:07:26.000000 sampy-abm-1.0.2/src/sampy/addons/ORM_related_addons/ORM_like_agents.py
--rw-rw-rw-   0        0        0        0 2023-06-22 17:07:26.000000 sampy-abm-1.0.2/src/sampy/addons/ORM_related_addons/__init__.py
--rw-rw-rw-   0        0        0     7126 2023-06-22 17:07:27.000000 sampy-abm-1.0.2/src/sampy/addons/ORM_related_addons/graph_from_ORM_xml.py
--rw-rw-rw-   0        0        0    13398 2023-06-22 17:07:27.000000 sampy-abm-1.0.2/src/sampy/addons/ORM_related_addons/jit_compiled_function.py
--rw-rw-rw-   0        0        0        0 2023-06-22 17:07:26.000000 sampy-abm-1.0.2/src/sampy/addons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.440746 sampy-abm-1.0.2/src/sampy/agent/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:07:27.000000 sampy-abm-1.0.2/src/sampy/agent/__init__.py
--rw-rw-rw-   0        0        0    11730 2023-06-22 17:07:28.000000 sampy-abm-1.0.2/src/sampy/agent/base.py
--rw-rw-rw-   0        0        0     3860 2023-06-22 17:07:28.000000 sampy-abm-1.0.2/src/sampy/agent/builtin_agent.py
--rw-rw-rw-   0        0        0    24137 2023-06-22 17:07:28.000000 sampy-abm-1.0.2/src/sampy/agent/jit_compiled_functions.py
--rw-rw-rw-   0        0        0    16668 2023-06-22 17:07:29.000000 sampy-abm-1.0.2/src/sampy/agent/mortality.py
--rw-rw-rw-   0        0        0    20506 2023-06-22 17:07:29.000000 sampy-abm-1.0.2/src/sampy/agent/movement.py
--rw-rw-rw-   0        0        0    20600 2023-06-22 17:07:29.000000 sampy-abm-1.0.2/src/sampy/agent/random_walk.py
--rw-rw-rw-   0        0        0    24184 2023-06-22 17:07:30.000000 sampy-abm-1.0.2/src/sampy/agent/reproduction.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.445992 sampy-abm-1.0.2/src/sampy/data_processing/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:07:30.000000 sampy-abm-1.0.2/src/sampy/data_processing/__init__.py
--rw-rw-rw-   0        0        0     6627 2023-06-22 17:07:30.000000 sampy-abm-1.0.2/src/sampy/data_processing/csv_manager.py
--rw-rw-rw-   0        0        0     1138 2023-06-22 17:07:31.000000 sampy-abm-1.0.2/src/sampy/data_processing/write_file.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.447607 sampy-abm-1.0.2/src/sampy/disease/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:07:31.000000 sampy-abm-1.0.2/src/sampy/disease/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.457167 sampy-abm-1.0.2/src/sampy/disease/single_species/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:07:31.000000 sampy-abm-1.0.2/src/sampy/disease/single_species/__init__.py
--rw-rw-rw-   0        0        0     5485 2023-06-22 17:07:32.000000 sampy-abm-1.0.2/src/sampy/disease/single_species/base.py
--rw-rw-rw-   0        0        0     7773 2023-06-22 17:07:32.000000 sampy-abm-1.0.2/src/sampy/disease/single_species/builtin_disease.py
--rw-rw-rw-   0        0        0     3387 2023-06-22 17:07:32.000000 sampy-abm-1.0.2/src/sampy/disease/single_species/jit_compiled_functions.py
--rw-rw-rw-   0        0        0    21124 2023-06-22 17:07:33.000000 sampy-abm-1.0.2/src/sampy/disease/single_species/transition.py
--rw-rw-rw-   0        0        0     7973 2023-06-22 17:07:33.000000 sampy-abm-1.0.2/src/sampy/disease/single_species/transmission.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.465388 sampy-abm-1.0.2/src/sampy/disease/two_species/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:07:33.000000 sampy-abm-1.0.2/src/sampy/disease/two_species/__init__.py
--rw-rw-rw-   0        0        0     5375 2023-06-22 17:07:34.000000 sampy-abm-1.0.2/src/sampy/disease/two_species/base.py
--rw-rw-rw-   0        0        0    12561 2023-06-22 17:07:34.000000 sampy-abm-1.0.2/src/sampy/disease/two_species/builtin_disease.py
--rw-rw-rw-   0        0        0     7147 2023-06-22 17:07:34.000000 sampy-abm-1.0.2/src/sampy/disease/two_species/jit_compiled_functions.py
--rw-rw-rw-   0        0        0    12671 2023-06-22 17:07:35.000000 sampy-abm-1.0.2/src/sampy/disease/two_species/transition.py
--rw-rw-rw-   0        0        0    11929 2023-06-22 17:07:35.000000 sampy-abm-1.0.2/src/sampy/disease/two_species/transmission.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.479984 sampy-abm-1.0.2/src/sampy/graph/
--rw-rw-rw-   0        0        0       59 2023-06-22 17:07:35.000000 sampy-abm-1.0.2/src/sampy/graph/__init__.py
--rw-rw-rw-   0        0        0     4856 2023-06-22 17:07:36.000000 sampy-abm-1.0.2/src/sampy/graph/builtin_graph.py
--rw-rw-rw-   0        0        0     6844 2023-06-22 17:07:36.000000 sampy-abm-1.0.2/src/sampy/graph/from_files.py
--rw-rw-rw-   0        0        0     7166 2023-06-22 17:07:36.000000 sampy-abm-1.0.2/src/sampy/graph/jit_compiled_functions.py
--rw-rw-rw-   0        0        0    26225 2023-06-22 17:07:37.000000 sampy-abm-1.0.2/src/sampy/graph/misc.py
--rw-rw-rw-   0        0        0    10145 2023-06-22 17:07:37.000000 sampy-abm-1.0.2/src/sampy/graph/spatial_2d.py
--rw-rw-rw-   0        0        0     2869 2023-06-22 17:07:37.000000 sampy-abm-1.0.2/src/sampy/graph/spatial_functions.py
--rw-rw-rw-   0        0        0    12256 2023-06-22 17:07:38.000000 sampy-abm-1.0.2/src/sampy/graph/topology.py
--rw-rw-rw-   0        0        0     7263 2023-06-22 17:07:38.000000 sampy-abm-1.0.2/src/sampy/graph/vertex_attributes.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.489034 sampy-abm-1.0.2/src/sampy/intervention/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:07:38.000000 sampy-abm-1.0.2/src/sampy/intervention/__init__.py
--rw-rw-rw-   0        0        0      939 2023-06-22 17:07:39.000000 sampy-abm-1.0.2/src/sampy/intervention/built_in_interventions.py
--rw-rw-rw-   0        0        0     2543 2023-06-22 17:07:39.000000 sampy-abm-1.0.2/src/sampy/intervention/culling.py
--rw-rw-rw-   0        0        0     1813 2023-06-22 17:07:39.000000 sampy-abm-1.0.2/src/sampy/intervention/jit_compiled_functions.py
--rw-rw-rw-   0        0        0     2374 2023-06-22 17:07:40.000000 sampy-abm-1.0.2/src/sampy/intervention/sampling.py
--rw-rw-rw-   0        0        0     5007 2023-06-22 17:07:40.000000 sampy-abm-1.0.2/src/sampy/intervention/vaccination.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.493041 sampy-abm-1.0.2/src/sampy/pandas_xs/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:07:40.000000 sampy-abm-1.0.2/src/sampy/pandas_xs/__init__.py
--rw-rw-rw-   0        0        0      621 2023-06-22 17:07:41.000000 sampy-abm-1.0.2/src/sampy/pandas_xs/jit_compiled_functions.py
--rw-rw-rw-   0        0        0    21328 2023-06-22 17:07:41.000000 sampy-abm-1.0.2/src/sampy/pandas_xs/pandas_xs.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.502142 sampy-abm-1.0.2/src/sampy/spatial/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:07:41.000000 sampy-abm-1.0.2/src/sampy/spatial/__init__.py
--rw-rw-rw-   0        0        0      797 2023-06-22 17:07:42.000000 sampy-abm-1.0.2/src/sampy/spatial/base_graph_intersection.py
--rw-rw-rw-   0        0        0       21 2023-06-22 17:07:42.000000 sampy-abm-1.0.2/src/sampy/spatial/built_in_graph_intersections.py
--rw-rw-rw-   0        0        0        0 2023-06-22 17:07:42.000000 sampy-abm-1.0.2/src/sampy/spatial/builtin_proximity_classes.py
--rw-rw-rw-   0        0        0      800 2023-06-22 17:07:43.000000 sampy-abm-1.0.2/src/sampy/spatial/graph_intersection_geometry.py
--rw-rw-rw-   0        0        0     2381 2023-06-22 17:07:43.000000 sampy-abm-1.0.2/src/sampy/spatial/jit_compiled_functions.py
--rw-rw-rw-   0        0        0    11967 2023-06-22 17:07:43.000000 sampy-abm-1.0.2/src/sampy/spatial/proximity_3d.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.505982 sampy-abm-1.0.2/src/sampy/utils/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:07:44.000000 sampy-abm-1.0.2/src/sampy/utils/__init__.py
--rw-rw-rw-   0        0        0     1939 2023-06-22 17:07:44.000000 sampy-abm-1.0.2/src/sampy/utils/decorators.py
--rw-rw-rw-   0        0        0     2661 2023-06-22 17:07:44.000000 sampy-abm-1.0.2/src/sampy/utils/errors_shortcut.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.525078 sampy-abm-1.0.2/src/sampy_abm.egg-info/
--rw-rw-rw-   0        0        0      823 2023-06-22 17:10:02.000000 sampy-abm-1.0.2/src/sampy_abm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2622 2023-06-22 17:10:02.000000 sampy-abm-1.0.2/src/sampy_abm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 17:10:02.000000 sampy-abm-1.0.2/src/sampy_abm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-22 17:10:02.000000 sampy-abm-1.0.2/src/sampy_abm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-22 17:10:02.000000 sampy-abm-1.0.2/src/sampy_abm.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-22 17:10:02.532980 sampy-abm-1.0.2/tests/
--rw-rw-rw-   0        0        0    24727 2023-06-22 17:07:19.000000 sampy-abm-1.0.2/tests/test_agents.py
--rw-rw-rw-   0        0        0     3081 2023-06-22 17:07:19.000000 sampy-abm-1.0.2/tests/test_disease_single_species.py
--rw-rw-rw-   0        0        0      639 2023-06-22 17:07:20.000000 sampy-abm-1.0.2/tests/test_disease_two_species.py
--rw-rw-rw-   0        0        0     9469 2023-06-22 17:07:20.000000 sampy-abm-1.0.2/tests/test_graphs.py
--rw-rw-rw-   0        0        0    24740 2023-06-22 17:07:20.000000 sampy-abm-1.0.2/tests/test_pandas_xs.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:33:08.560460 sampy_abm-1.0.3/
+-rw-rw-rw-   0        0        0    35149 2023-06-07 19:00:29.000000 sampy_abm-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1113 2024-04-16 19:33:08.559516 sampy_abm-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2024-04-16 19:24:44.000000 sampy_abm-1.0.3/README.md
+-rw-rw-rw-   0        0        0      653 2024-04-16 19:16:23.000000 sampy_abm-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 19:33:08.560460 sampy_abm-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-16 19:33:08.179712 sampy_abm-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-16 19:33:08.195598 sampy_abm-1.0.3/src/sampy/
+-rw-rw-rw-   0        0        0      111 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:33:08.197156 sampy_abm-1.0.3/src/sampy/addons/
+drwxrwxrwx   0        0        0        0 2024-04-16 19:33:08.210129 sampy_abm-1.0.3/src/sampy/addons/GIS_interface/
+-rw-rw-rw-   0        0        0        0 2023-09-27 19:51:45.000000 sampy_abm-1.0.3/src/sampy/addons/GIS_interface/__init__.py
+-rw-rw-rw-   0        0        0    16769 2024-01-19 22:03:25.000000 sampy_abm-1.0.3/src/sampy/addons/GIS_interface/geographic_grid.py
+-rw-rw-rw-   0        0        0     1234 2024-01-19 18:45:58.000000 sampy_abm-1.0.3/src/sampy/addons/GIS_interface/jit_compiled_functions.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:33:08.230945 sampy_abm-1.0.3/src/sampy/addons/ORM_related_addons/
+-rw-rw-rw-   0        0        0    33431 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/addons/ORM_related_addons/ORM_like_agents.py
+-rw-rw-rw-   0        0        0        0 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/addons/ORM_related_addons/__init__.py
+-rw-rw-rw-   0        0        0     7269 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/addons/ORM_related_addons/graph_from_ORM_xml.py
+-rw-rw-rw-   0        0        0    13716 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/addons/ORM_related_addons/jit_compiled_function.py
+-rw-rw-rw-   0        0        0        0 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/addons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:33:08.290528 sampy_abm-1.0.3/src/sampy/agent/
+-rw-rw-rw-   0        0        0        0 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/agent/__init__.py
+-rw-rw-rw-   0        0        0    14344 2024-04-16 18:32:20.000000 sampy_abm-1.0.3/src/sampy/agent/base.py
+-rw-rw-rw-   0        0        0     5888 2024-02-20 15:57:34.000000 sampy_abm-1.0.3/src/sampy/agent/builtin_agent.py
+-rw-rw-rw-   0        0        0    31493 2023-12-12 23:07:41.000000 sampy_abm-1.0.3/src/sampy/agent/jit_compiled_functions.py
+-rw-rw-rw-   0        0        0    16936 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/agent/mortality.py
+-rw-rw-rw-   0        0        0    20847 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/agent/movement.py
+-rw-rw-rw-   0        0        0    24899 2024-02-20 19:59:11.000000 sampy_abm-1.0.3/src/sampy/agent/random_walk.py
+-rw-rw-rw-   0        0        0    46162 2024-02-20 15:57:32.000000 sampy_abm-1.0.3/src/sampy/agent/reproduction.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:33:08.308395 sampy_abm-1.0.3/src/sampy/data_processing/
+-rw-rw-rw-   0        0        0        0 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/data_processing/__init__.py
+-rw-rw-rw-   0        0        0     6786 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/data_processing/csv_manager.py
+-rw-rw-rw-   0        0        0     3563 2024-04-16 18:32:20.000000 sampy_abm-1.0.3/src/sampy/data_processing/extract_data_for_SCRW.py
+-rw-rw-rw-   0        0        0     1336 2023-11-29 17:30:15.000000 sampy_abm-1.0.3/src/sampy/data_processing/jit_compiled_functions.py
+-rw-rw-rw-   0        0        0     2397 2023-11-15 19:06:17.000000 sampy_abm-1.0.3/src/sampy/data_processing/write_file.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:33:08.310389 sampy_abm-1.0.3/src/sampy/disease/
+-rw-rw-rw-   0        0        0        0 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/disease/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:33:08.336641 sampy_abm-1.0.3/src/sampy/disease/single_species/
+-rw-rw-rw-   0        0        0        0 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/disease/single_species/__init__.py
+-rw-rw-rw-   0        0        0     5585 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/disease/single_species/base.py
+-rw-rw-rw-   0        0        0     7890 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/disease/single_species/builtin_disease.py
+-rw-rw-rw-   0        0        0     3491 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/disease/single_species/jit_compiled_functions.py
+-rw-rw-rw-   0        0        0    21476 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/disease/single_species/transition.py
+-rw-rw-rw-   0        0        0     8113 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/disease/single_species/transmission.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:33:08.371643 sampy_abm-1.0.3/src/sampy/disease/two_species/
+-rw-rw-rw-   0        0        0        0 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/disease/two_species/__init__.py
+-rw-rw-rw-   0        0        0     5480 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/disease/two_species/base.py
+-rw-rw-rw-   0        0        0    14295 2023-10-02 15:00:46.000000 sampy_abm-1.0.3/src/sampy/disease/two_species/builtin_disease.py
+-rw-rw-rw-   0        0        0     7321 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/disease/two_species/jit_compiled_functions.py
+-rw-rw-rw-   0        0        0    12893 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/disease/two_species/transition.py
+-rw-rw-rw-   0        0        0    12091 2023-09-27 15:09:08.000000 sampy_abm-1.0.3/src/sampy/disease/two_species/transmission.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:33:08.424800 sampy_abm-1.0.3/src/sampy/graph/
+-rw-rw-rw-   0        0        0       59 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/graph/__init__.py
+-rw-rw-rw-   0        0        0     5692 2023-10-03 18:01:06.000000 sampy_abm-1.0.3/src/sampy/graph/builtin_graph.py
+-rw-rw-rw-   0        0        0     7005 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/graph/from_files.py
+-rw-rw-rw-   0        0        0     8000 2023-09-19 19:26:32.000000 sampy_abm-1.0.3/src/sampy/graph/jit_compiled_functions.py
+-rw-rw-rw-   0        0        0    31198 2024-04-16 18:32:20.000000 sampy_abm-1.0.3/src/sampy/graph/misc.py
+-rw-rw-rw-   0        0        0    21223 2023-09-27 15:09:08.000000 sampy_abm-1.0.3/src/sampy/graph/spatial_2d.py
+-rw-rw-rw-   0        0        0     3022 2023-08-09 16:20:50.000000 sampy_abm-1.0.3/src/sampy/graph/spatial_functions.py
+-rw-rw-rw-   0        0        0    13955 2024-04-16 18:32:20.000000 sampy_abm-1.0.3/src/sampy/graph/topology.py
+-rw-rw-rw-   0        0        0     7403 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/graph/vertex_attributes.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:33:08.448483 sampy_abm-1.0.3/src/sampy/intervention/
+-rw-rw-rw-   0        0        0        0 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/intervention/__init__.py
+-rw-rw-rw-   0        0        0      965 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/intervention/built_in_interventions.py
+-rw-rw-rw-   0        0        0     2595 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/intervention/culling.py
+-rw-rw-rw-   0        0        0     1860 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/intervention/jit_compiled_functions.py
+-rw-rw-rw-   0        0        0     2424 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/intervention/sampling.py
+-rw-rw-rw-   0        0        0     5094 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/intervention/vaccination.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:33:08.461572 sampy_abm-1.0.3/src/sampy/pandas_xs/
+-rw-rw-rw-   0        0        0        0 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/pandas_xs/__init__.py
+-rw-rw-rw-   0        0        0      645 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/pandas_xs/jit_compiled_functions.py
+-rw-rw-rw-   0        0        0    24127 2024-04-16 18:32:20.000000 sampy_abm-1.0.3/src/sampy/pandas_xs/pandas_xs.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:33:08.495948 sampy_abm-1.0.3/src/sampy/spatial/
+-rw-rw-rw-   0        0        0        0 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/spatial/__init__.py
+-rw-rw-rw-   0        0        0     6213 2023-09-27 15:09:08.000000 sampy_abm-1.0.3/src/sampy/spatial/base_graph_intersection.py
+-rw-rw-rw-   0        0        0     2471 2023-11-17 19:11:12.000000 sampy_abm-1.0.3/src/sampy/spatial/built_in_graph_intersections.py
+-rw-rw-rw-   0        0        0     6073 2023-11-17 15:58:57.000000 sampy_abm-1.0.3/src/sampy/spatial/builtin_proximity_classes.py
+-rw-rw-rw-   0        0        0     9263 2023-09-27 15:09:08.000000 sampy_abm-1.0.3/src/sampy/spatial/graph_intersection_geometry.py
+-rw-rw-rw-   0        0        0     8837 2023-11-22 15:04:38.000000 sampy_abm-1.0.3/src/sampy/spatial/jit_compiled_functions.py
+-rw-rw-rw-   0        0        0    13973 2023-11-22 14:58:19.000000 sampy_abm-1.0.3/src/sampy/spatial/proximity_3d.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:33:08.502640 sampy_abm-1.0.3/src/sampy/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/utils/__init__.py
+-rw-rw-rw-   0        0        0     1999 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/utils/decorators.py
+-rw-rw-rw-   0        0        0     2708 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/src/sampy/utils/errors_shortcut.py
+drwxrwxrwx   0        0        0        0 2024-04-16 19:33:08.557499 sampy_abm-1.0.3/src/sampy_abm.egg-info/
+-rw-rw-rw-   0        0        0     1113 2024-04-16 19:33:08.000000 sampy_abm-1.0.3/src/sampy_abm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2875 2024-04-16 19:33:08.000000 sampy_abm-1.0.3/src/sampy_abm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 19:33:08.000000 sampy_abm-1.0.3/src/sampy_abm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-04-16 19:33:08.000000 sampy_abm-1.0.3/src/sampy_abm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-16 19:33:08.000000 sampy_abm-1.0.3/src/sampy_abm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 19:33:08.556463 sampy_abm-1.0.3/tests/
+-rw-rw-rw-   0        0        0    25169 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/tests/test_agents.py
+-rw-rw-rw-   0        0        0     3138 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/tests/test_disease_single_species.py
+-rw-rw-rw-   0        0        0      656 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/tests/test_disease_two_species.py
+-rw-rw-rw-   0        0        0    20605 2023-08-09 16:20:38.000000 sampy_abm-1.0.3/tests/test_graphs.py
+-rw-rw-rw-   0        0        0    25319 2023-07-26 15:27:11.000000 sampy_abm-1.0.3/tests/test_pandas_xs.py
```

### Comparing `sampy-abm-1.0.2/LICENSE` & `sampy_abm-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sampy-abm-1.0.2/src/sampy/addons/ORM_related_addons/ORM_like_agents.py` & `sampy_abm-1.0.3/src/sampy/addons/ORM_related_addons/ORM_like_agents.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,498 +1,498 @@
-from ...agent.base import BaseAgingAgent
-from ...agent.mortality import NaturalMortalityOrmMethodology, OffspringDependantOnParents
-from ...agent.reproduction import (OffspringCreationWithCustomProb,
-                                      FindMateMonogamous,
-                                      FindMatePolygamous)
-from ...agent.movement import TerritorialMovementWithoutResistance
-from ...utils.decorators import sampy_class
-
-from .jit_compiled_function import *
-from ...agent.jit_compiled_functions import movement_mov_around_territory_fill_bool_mov_using_condition
-
-import numpy as np
-
-
-class ComponentsFromORM:
-    """
-    This class contains basic methods extracted from ORM source code. Developed for the need of the Leighton Lab.
-    Add orm-like methods to the agents. That are:
-
-        - movement that take into account 'resistance' to the movement (i.e. each agent movement has a probability of
-          success that depends on the user's landscape;
-        - when an agent fails to move (for any reason), its displacement ends for the current timestep;
-        - add a form of discrete correlated random walk, using the hexagonal structure of ORM landscapes (see
-          dispersion);
-        - add a series of ways to modelize natural mortality, as found in ORM code;
-        - some methods make the assumption that each timestep represent a week, with 52 weeks in a year.
-
-    IMPORTANT: for some methods, the underlying graph is assumed to come from an ORM xml using the class
-               GraphFromORMxml
-    """
-    def __init__(self, **kwargs):
-        self.df_population['has_moved'] = False
-        self.dict_default_val['has_moved'] = False
-
-    def orm_dispersion(self, timestep, permissible_weeks, condition, arr_nb_steps, arr_prob_nb_steps,
-                       position_attribute='position', territory_attribute='territory', reflexion=False):
-        """
-        This method ignores resistance to movement.
-
-        In the ORM, agents' dispersion is dealt with on a yearly basis. That is, each year (52 timesteps each
-        representing a week) an agent will disperse once and only once. This method takes care of checking if an agent
-        already dispersed or not. When an agent disperse, it draws a number of steps and performs a discrete
-        correlated random walk on the hexagonal landscape. At first, the agent choses a random direction among the six
-        possible neighbours of its current cell (North, north-east, south-est, etc. See GraphORMXml description for
-        details). If there is no cell in that direction, dispersion stops (but it is still counted as if the agent
-        dispersed this year). If there is one, the agent jumps to this new cell, then a new direction is picked: with a
-        60% chance the direction remains unchanged, with 20% it turns left by one notch (if for instance the first
-        direction was North-east, then there is a 20% chance that the next direction will be North), with 20% it turns
-        right. We then repeat the process until the agent has made all its steps.
-
-        IMPORTANT: This method assumes agents are living on a GraphFromORMxml.
-        Warning: If reflexion is used, there might be a bias since we recycle an already used random value.
-
-        :param timestep: current timestep, number of week since simulation started (starts at 0).
-        :param permissible_weeks: array-like object of integer saying which week of the year the agents can disperse
-                                  (counted from 0 to 51).
-        :param condition: 1D array of bool of shape (nb_agents,) saying which agents are allowed to disperse.
-        :param arr_nb_steps: 1D array of non-negative integers, works in tandem with arr_prob_nb_steps.
-        :param arr_prob_nb_steps: 1D array of float, each between 0 and 1. arr_prob_nb_steps[i] is the probability for
-                                  a dispersing agent to do arr_nb_steps[i] steps. Note that this number of step can be
-                                  0. Effectively, this would lead to the agent "having dispersed this year" yet without
-                                  having moved.
-        :param position_attribute: optional, string, default 'position'. Name of the position attribute in the agents.
-        :param territory_attribute: optional, string, default 'territory'. Name of the territory attribute in the
-                                    agents.
-        :param reflexion: optionnal, boolean, default False.
-        """
-        if self.df_population.nb_rows == 0:
-            return
-
-        # we reinitialize the 'has_moved' status if first week of the year
-        if timestep % 52 == 0:
-            self.df_population['has_moved'] = False
-
-        if timestep % 52 not in permissible_weeks:
-            return
-
-        can_move = condition & ~self.df_population['has_moved']
-        will_move = np.random.uniform(0, 1, can_move.sum()) < \
-                    (permissible_weeks.index(timestep % 52) + 1) / len(permissible_weeks)
-        prob = arr_prob_nb_steps.astype('float64')
-        prob = prob / prob.sum()
-        rand_nb_steps = np.random.choice(arr_nb_steps, will_move.sum(), p=prob)
-        rand_directions = np.random.uniform(0, 1, rand_nb_steps.sum())
-
-        if reflexion:
-            orm_like_agent_dispersion_with_reflexion(can_move, will_move, rand_nb_steps, rand_directions,
-                                                     self.df_population[position_attribute],
-                                                     self.df_population[territory_attribute],
-                                                     self.df_population['has_moved'],
-                                                     self.graph.connections, self.graph.weights)
-        else:
-            orm_like_agent_orm_dispersion(can_move, will_move, rand_nb_steps, rand_directions,
-                                          self.df_population[position_attribute],
-                                          self.df_population[territory_attribute],
-                                          self.df_population['has_moved'],
-                                          self.graph.connections)
-
-    def orm_dispersion_with_resistance(self, timestep, permissible_weeks, condition, arr_nb_steps, arr_prob_nb_steps,
-                                       position_attribute='position', territory_attribute='territory'):
-        """
-        This method included resistance to movement.
-
-        In the ORM, agents' dispersion is dealt with on a yearly basis. That is, each year (52 timesteps each
-        representing a week) an agent will disperse once and only once. This method takes care of checking if an agent
-        already dispersed or not. When an agent disperse, it draws a number of steps and performs a discrete
-        correlated random walk on the hexagonal landscape. At first, the agent choses a random direction among the six
-        possible neighbours of its current cell (North, north-east, south-est, etc. See GraphORMXml description for
-        details). If there is no cell in that direction, dispersion stops (but it is still counted as if the agent
-        dispersed this year). If there is one, the agent jumps to this new cell, then a new direction is picked: with a
-        60% chance the direction remains unchanged, with 20% it turns left by one notch (if for instance the first
-        direction was North-east, then there is a 20% chance that the next direction will be North), with 20% it turns
-        right. We then repeat the process until the agent has made all its steps.
-
-        IMPORTANT: This method assumes agents are living on a GraphFromORMxml.
-        Warning: If reflexion is used, there might be a bias since we recycle an already used random value.
-
-        :param timestep: current timestep, number of week since simulation started (starts at 0).
-        :param permissible_weeks: array-like object of integer saying which week of the year the agents can disperse
-                                  (counted from 0 to 51).
-        :param condition: 1D array of bool of shape (nb_agents,) saying which agents are allowed to disperse.
-        :param arr_nb_steps: 1D array of non-negative integers, works in tandem with arr_prob_nb_steps.
-        :param arr_prob_nb_steps: 1D array of float, each between 0 and 1. arr_prob_nb_steps[i] is the probability for
-                                  a dispersing agent to do arr_nb_steps[i] steps. Note that this number of step can be
-                                  0. Effectively, this would lead to the agent "having dispersed this year" yet without
-                                  having moved.
-        :param position_attribute: optional, string, default 'position'. Name of the position attribute in the agents.
-        :param territory_attribute: optional, string, default 'territory'. Name of the territory attribute in the
-                                    agents.
-        """
-        if self.df_population.nb_rows == 0:
-            return
-
-        # we reinitialize the 'has_moved' status if first week of the year
-        if timestep % 52 == 0:
-            self.df_population['has_moved'] = False
-
-        if timestep % 52 not in permissible_weeks:
-            return
-
-        can_move = condition & ~self.df_population['has_moved']
-        will_move = np.random.uniform(0, 1, can_move.sum()) < \
-                    (permissible_weeks.index(timestep % 52) + 1) / len(permissible_weeks)
-        prob = arr_prob_nb_steps.astype('float64')
-        prob = prob / prob.sum()
-        rand_nb_steps = np.random.choice(arr_nb_steps, will_move.sum(), p=prob)
-        rand_directions = np.random.uniform(0, 1, rand_nb_steps.sum())
-        rand_res = np.random.uniform(0, 1, rand_nb_steps.sum())
-
-        orm_like_agent_orm_dispersion_with_resistance(can_move, will_move, rand_nb_steps, rand_directions,
-                                                      self.df_population[position_attribute],
-                                                      self.df_population[territory_attribute],
-                                                      self.df_population['has_moved'], self.graph.connections,
-                                                      self.graph.prob_successful_move,
-                                                      rand_res)
-
-    def mov_around_with_resistance(self,
-                                   proba_remain_on_territory,
-                                   condition=None,
-                                   territory_attribute='territory',
-                                   position_attribute='position'):
-        """
-        This method includes movement resistance. Update the average position of the agent around its territory during
-        the current time step.
-
-        :param proba_remain_on_territory: float, probability to stay on the territory
-        :param condition: optional, array of bool, default None. Array of boolean such that the i-th value is
-                          True if and only if the i-th agent (i.e. the agent at the line i of df_population) can
-                          move.
-        :param territory_attribute: optional, string, default 'territory'
-        :param position_attribute: optional, string, default 'position'
-        """
-        if self.df_population.nb_rows == 0:
-            return
-
-        if condition is not None:
-            pre_bool_mov = np.random.uniform(0, 1, condition.sum()) > proba_remain_on_territory
-            bool_mov = movement_mov_around_territory_fill_bool_mov_using_condition(pre_bool_mov, condition)
-        else:
-            bool_mov = np.random.uniform(0, 1, self.df_population.shape[0]) > proba_remain_on_territory
-
-        rand_direction = np.random.uniform(0, 1, bool_mov.sum())
-        rand_res = np.random.uniform(0, 1, bool_mov.sum())
-
-        orm_like_agents_mov_around_with_resistance(self.df_population[territory_attribute],
-                                                   self.df_population[position_attribute],
-                                                   self.graph.connections, self.graph.weights,
-                                                   self.graph.prob_successful_move, bool_mov, rand_direction,
-                                                   rand_res)
-
-    def _mortality_from_v08(self, arr_annual_mortality, condition_count, alpha_beta=None, condition=None,
-                            shuffle=True, age_attribute='age', position_attribute='position'):
-        """
-        (made by Francois Viard)
-
-        This is an adaptation of the mortality method found in ARM v08 (file cFox.cs). ARM is not a typo, it is the
-        'Arctic Rabies Model', which is a variation of ORM. I don't think it's been published or used in publication?
-
-        WARNING: There are no sources given in the ORM file for the origin of this method. As such, I cannot guarantee
-                 that I correctly understood what it is supposed to do and why. Therefore, this method is considered
-                 private and should be use with caution.
-
-        :param arr_annual_mortality: array of float between 0 and 1. arr_annual_mortality[i] is the target probability
-                                     for an agent to die at age i.
-        :param condition_count: 1D array of bool, tells which agent to count.
-        :param alpha_beta: Absolute mystery. In the formula used in ARM there is an Alpha and a Beta, but I could not
-                           figure out if those were actually modified or if the default values were always taken. I
-                           finally decided to postpone the inclusion of those option to a later date... However,
-                           every project finally moved away from this method and fell back to the usual ORM mortality.
-                           As it is, DO NOT USE THIS KWARGS.
-        :param condition: optional, 1D array of bool, default None. If not None, tells which agents can die.
-        :param shuffle: optional, bool, default True. If True, shuffle the population dataframe before applying method
-        :param age_attribute: optional, string, default 'age'. Name of the age attribute of the agents.
-        :param position_attribute: optional, string, default 'position'. Name of the position attribute of the agents.
-        """
-        if self.df_population.nb_rows == 0:
-            return
-
-        if shuffle:
-            permutation = self.df_population.scramble(return_permutation=True)
-            if condition is not None:
-                condition = condition[permutation]
-            condition_count = condition_count[permutation]
-
-        count_arr = self.count_pop_per_vertex(position_attribute=position_attribute, condition=condition_count)
-        if alpha_beta is None:
-            if condition is None:
-                rand = np.random.uniform(0, 1, self.df_population.nb_rows)
-                survive = orm_like_agents_mortality_from_v08_no_condition_no_alpha_beta(count_arr, condition_count,
-                                                                                        self.df_population[position_attribute],
-                                                                                        self.graph.df_attributes['K'],
-                                                                                        arr_annual_mortality,
-                                                                                        self.df_population[age_attribute],
-                                                                                        rand)
-            else:
-                rand = np.random.uniform(0, 1, self.df_population.nb_rows)
-                survive = orm_like_agents_mortality_from_v08_with_condition_no_alpha_beta(count_arr, condition_count,
-                                                                                          self.df_population[
-                                                                                            position_attribute],
-                                                                                          self.graph.df_attributes['K'],
-                                                                                          arr_annual_mortality,
-                                                                                          self.df_population[
-                                                                                            age_attribute],
-                                                                                          rand, condition)
-        self.df_population = self.df_population[survive]
-
-    def _mortality_from_v08_with_gender(self, arr_female_annual_mortality, arr_male_annual_mortality, condition_count,
-                                        alpha_beta=None, condition=None, shuffle=True, age_attribute='age',
-                                        position_attribute='position', gender_attribute='gender'):
-        """
-        (made by Francois Viard)
-
-        This is an adaptation of the mortality method found in ARM v08 (file cFox.cs). ARM is not a typo, it is the
-        'Arctic Rabies Model', which is a variation of ORM. I don't think it's been published or used in publication?
-
-        WARNING: There are no sources given in the ORM file for the origin of this method. As such, I cannot guarantee
-                 that I correctly understood what it is supposed to do and why. Therefore, this method is considered
-                 private and should be use with caution.
-
-        :param arr_female_annual_mortality: array of float between 0 and 1. arr_annual_mortality[i] is the target
-                                    probability for a female agent to die at age i.
-        :param arr_male_annual_mortality: array of float between 0 and 1. arr_annual_mortality[i] is the target
-                                    probability for a male agent to die at age i.
-        :param condition_count: 1D array of bool, tells which agent to count.
-        :param alpha_beta: Absolute mystery. In the formula used in ARM there is an Alpha and a Beta, but I could not
-                           figure out if those were actually modified or if the default values were always taken. I
-                           finally decided to postpone the inclusion of those option to a later date... However,
-                           every project finally moved away from this method and fell back to the usual ORM mortality.
-                           As it is, DO NOT USE THIS KWARGS.
-        :param condition: optional, 1D array of bool, default None. If not None, tells which agents can die.
-        :param shuffle: optional, bool, default True. If True, shuffle the population dataframe before applying method
-        :param age_attribute: optional, string, default 'age'. Name of the age attribute of the agents.
-        :param position_attribute: optional, string, default 'position'. Name of the position attribute of the agents.
-        :param gender_attribute: optional, string, default 'gender'. Name of the gender attribute of the agents.
-        """
-        if self.df_population.nb_rows == 0:
-            return
-
-        if shuffle:
-            permutation = self.df_population.scramble(return_permutation=True)
-            if condition is not None:
-                condition = condition[permutation]
-            condition_count = condition_count[permutation]
-
-        count_arr = self.count_pop_per_vertex(position_attribute=position_attribute, condition=condition_count)
-        if alpha_beta is None:
-            if condition is None:
-                rand = np.random.uniform(0, 1, self.df_population.nb_rows)
-                survive = orm_like_agents_mortality_from_v08_with_gender_no_condition_no_alpha_beta(count_arr,
-                                                                                condition_count,
-                                                                                self.df_population[position_attribute],
-                                                                                self.graph.df_attributes['K'],
-                                                                                self.df_population[gender_attribute],
-                                                                                arr_female_annual_mortality,
-                                                                                arr_male_annual_mortality,
-                                                                                self.df_population[age_attribute],
-                                                                                rand)
-            else:
-                rand = np.random.uniform(0, 1, (condition.sum(),))
-                survive = orm_like_agents_mortality_from_v08_with_gender_with_condition_no_alpha_beta(count_arr,
-                                                                                condition_count,
-                                                                                self.df_population[position_attribute],
-                                                                                self.graph.df_attributes['K'],
-                                                                                self.df_population[gender_attribute],
-                                                                                arr_female_annual_mortality,
-                                                                                arr_male_annual_mortality,
-                                                                                self.df_population[age_attribute],
-                                                                                rand,
-                                                                                condition)
-        self.df_population = self.df_population[survive]
-
-
-class ExperimentalDensityDependentMortality:
-    """
-    Some experiments that will be moved elsewhere soon.
-    """
-    def __init__(self, **kwargs):
-        self._corrected_beta_female = None
-        self._corrected_beta_male = None
-
-    def compute_and_save_beta_female(self, alpha, arr_female_weekly_mortality):
-        self._corrected_beta_female = 1. + (1. / alpha) * np.log((1. / arr_female_weekly_mortality) - 1.)
-
-    def compute_and_save_beta_male(self, alpha, arr_male_weekly_mortality):
-        self._corrected_beta_male = 1. + (1. / alpha) * np.log((1. / arr_male_weekly_mortality) - 1.)
-
-    def experimental_mortality_logistic_function(self, alpha, arr_female_weekly_mortality, arr_male_weekly_mortality,
-                                                 age_attribute='age', position_attribute='position', k_attribute='K',
-                                                 shuffle=True, gender_attribute='gender'):
-        if self._corrected_beta_female is None:
-            self.compute_and_save_beta_female(alpha, arr_female_weekly_mortality)
-        if self._corrected_beta_male is None:
-            self.compute_and_save_beta_male(alpha, arr_male_weekly_mortality)
-        if shuffle:
-            self.df_population.scramble()
-        count_arr = self.count_pop_per_vertex(position_attribute=position_attribute)
-        rand = np.random.uniform(0, 1, (self.df_population.nb_rows,))
-        survive = experimental_density_mortality(count_arr, self.df_population[position_attribute],
-                                                 self.df_population[age_attribute],
-                                                 self.graph.df_attributes[k_attribute],
-                                                 self.df_population[gender_attribute],
-                                                 self._corrected_beta_male, self._corrected_beta_female,
-                                                 alpha, rand)
-        self.df_population = self.df_population[survive]
-
-
-@sampy_class
-class ORMLikeAgent(BaseAgingAgent,
-                   NaturalMortalityOrmMethodology,
-                   OffspringDependantOnParents,
-                   FindMateMonogamous,
-                   OffspringCreationWithCustomProb,
-                   TerritorialMovementWithoutResistance,
-                   ComponentsFromORM):
-    """
-    Basic ORM like agents.
-
-    Includes main components from SamPy plus the building block 'ComponentsFromORM'.
-
-    :param graph: Mandatory kwargs, a graph object. Some methods expect this to be a "GraphFromORMXml' object.
-    """
-    def __init__(self, **kwargs):
-        pass
-
-
-@sampy_class
-class ORMMongooses(BaseAgingAgent,
-                   NaturalMortalityOrmMethodology,
-                   OffspringDependantOnParents,
-                   FindMatePolygamous,
-                   OffspringCreationWithCustomProb,
-                   TerritorialMovementWithoutResistance,
-                   ComponentsFromORM):
-    """
-    Mongooses from ORM with some updates for Caroline Sauve projects.
-    Includes main components from SamPy plus the building block 'ComponentsFromORM'.
-
-    :param graph: Mandatory kwargs, a graph object. Some methods expect this to be a GraphFromORMXml object.
-    :param pregnancy_duration: mandatory kwargs, an integer. Duration in weeks of pregnancy.
-    """
-    def __init__(self, pregnancy_duration=None, **kwargs):
-        if pregnancy_duration is None:
-            raise ValueError("A value for pregnancy duration should be given using kwarg 'pregnancy_duration'")
-        self.pregnancy_duration = pregnancy_duration
-        self.df_population['nb_weeks_being_pregnant'] = 0
-        self.dict_default_val['nb_weeks_being_pregnant'] = 0
-
-        self.df_population['week_next_potential_mating'] = -1
-        self.dict_default_val['week_next_potential_mating'] = -1
-
-    def increment_number_of_weeks_of_pregnancy(self):
-        """
-        Mongoose object keeps track of pregnancy duration with individual counters. This method increments those
-        counters. Should be called weekly.
-        """
-        self.df_population['nb_weeks_being_pregnant'] += self.df_population['is_pregnant']
-
-    def check_if_mother_free_of_dependent_young(self, age_independence, min_age_reproduction, mother_attribute='mom_id',
-                                                id_attribute='col_id', age_attribute='age'):
-        """
-        Checks which females old enough to reproduce do not have offsprings.
-
-        :param age_independence: integer, age at which offspring can live on their own.
-        :param min_age_reproduction: integer, age at which females can reproduce.
-        :param mother_attribute: optional, string, default 'mom_id'. Name of the attribute giving the id of the mother
-                                 of each agent.
-        :param id_attribute: optional, string, default 'col_id'. Name of the attribute containing the id of the agents.
-        :param age_attribute: optional, string, default 'age'. Name of the attribute containing the age of the agents.
-
-        :return: 1D array of bool, where return[i] is True if and only if the i-th agent is a Female available for
-                 reproduction.
-        """
-        offsprings = self.df_population[age_attribute] < age_independence
-        mom_id_offsprings = self.df_population[mother_attribute][offsprings]
-        potential_mothers = (self.df_population[age_attribute] >= min_age_reproduction) & self.get_females()
-        orm_mongooses_check_if_mother_free_of_juveniles(mom_id_offsprings, self.df_population[id_attribute],
-                                                        potential_mothers)
-        return potential_mothers
-
-    def give_birth_if_needed(self, arr_nb_children, arr_prob_nb_children, condition=None, prob_failure=None):
-        """
-        Make each female that reached the end of their pregnancy period give birth.
-
-        :param arr_nb_children: 1D array of integer, works in tandem with arr_prob_nb_children below.
-        :param arr_prob_nb_children: 1D array of float between 0 and 1. arr_prob_nb_children[i] is the probability for
-                                     a female giving birth to have arr_nb_children[i] offsprings.
-        :param condition: optional, 1D array of bool, default None. If not None, tells which female agents can give
-                          birth.
-        :param prob_failure: optional, float between 0 and 1, default one. If not None, gives the probability for the
-                             agent to fail giving birth. Note that this is equivalent with putting 0 as a possible value
-                             in arr_nb_children, and we recommend user to chose one solution or the other.
-        """
-        about_to_give_birth = (self.df_population['nb_weeks_being_pregnant'] >= self.pregnancy_duration)
-        if condition is None:
-            condition = about_to_give_birth
-        else:
-            condition = condition & about_to_give_birth
-        self.df_population['nb_weeks_being_pregnant'] *= ~condition
-        self.create_offsprings_custom_prob(arr_nb_children, arr_prob_nb_children, condition=condition,
-                                           prob_failure=prob_failure)
-
-    def children_follow_their_mom(self, min_age, max_age, age_attribute='age', mom_id_attribute='mom_id',
-                                  id_attribute='col_id', position_attribute='position',
-                                  territory_attribute='territory'):
-        youngs = (self.df_population[age_attribute] >= min_age) & (self.df_population[age_attribute] <= max_age)
-        id_moms = self.df_population[mom_id_attribute][youngs]
-        orm_mongooses_update_ter_pos_youngs(id_moms, youngs, self.df_population[territory_attribute],
-                                            self.df_population[position_attribute], self.df_population[id_attribute],
-                                            self.df_population[mom_id_attribute])
-
-    def weekly_mating_checks_and_update(self, current_week, mean_mate_weeks, var_mate_weeks, age_independence,
-                                        min_age_reproduction, gender_attribute='gender', mother_attribute='mom_id',
-                                        id_attribute='col_id', age_attribute='age', position_attribute='position',
-                                        pregnancy_attribute='is_pregnant', mate_attribute='current_mate'):
-        """
-        Method written in order to reproduce the multiple reproduction spikes that can be seen in Mongooses.
-
-        :param current_week: integer, value between 0 and 51 representing the current week of the year.
-        :param mean_mate_weeks:
-        :param var_mate_weeks:
-        :param age_independence:
-        :param min_age_reproduction:
-        :param gender_attribute:
-        :param mother_attribute:
-        :param id_attribute:
-        :param age_attribute:
-        :param position_attribute:
-        :param pregnancy_attribute:
-        :param mate_attribute:
-        """
-
-        # we begin with making the females ready to mate attempt to, well, mate
-        potentially_mating_females = self.df_population['week_next_potential_mating'] == current_week
-        if potentially_mating_females.sum() > 0:
-            female_available = self.check_if_mother_free_of_dependent_young(age_independence, min_age_reproduction,
-                                                                            gender_attribute=gender_attribute,
-                                                                            mother_attribute=mother_attribute,
-                                                                            id_attribute=id_attribute,
-                                                                            age_attribute=age_attribute)
-            female_available = female_available & ~self.df_population[pregnancy_attribute]
-            mating_females = potentially_mating_females & female_available
-            mating_males = self.get_males() & (self.df_population[age_attribute] >= min_age_reproduction)
-            self.find_random_mate_on_position(1., condition=(mating_females | mating_males), id_attribute=id_attribute,
-                                              position_attribute=position_attribute, gender_attribute=gender_attribute,
-                                              mate_attribute=mate_attribute, pregnancy_attribute=pregnancy_attribute)
-
-        # we now (re)-initialize the "week_next_potential_mating" attribute
-        init_next_week = potentially_mating_females | ((self.df_population['week_next_potential_mating'] == -1) &
-                                                       (self.df_population[age_attribute] >= min_age_reproduction))
-        nb_init_to_perform = init_next_week.sum()
-        if nb_init_to_perform > 0:
-            rand_gauss = np.random.normal(0, 1, (nb_init_to_perform,))
-            orm_mongooses_update_mating_week(current_week, mean_mate_weeks, var_mate_weeks,
-                                             self.df_population['week_next_potential_mating'],
-                                             init_next_week, rand_gauss)
-
-
-
+from ...agent.base import BaseAgingAgent
+from ...agent.mortality import NaturalMortalityOrmMethodology, OffspringDependantOnParents
+from ...agent.reproduction import (OffspringCreationWithCustomProb,
+                                      FindMateMonogamous,
+                                      FindMatePolygamous)
+from ...agent.movement import TerritorialMovementWithoutResistance
+from ...utils.decorators import sampy_class
+
+from .jit_compiled_function import *
+from ...agent.jit_compiled_functions import movement_mov_around_territory_fill_bool_mov_using_condition
+
+import numpy as np
+
+
+class ComponentsFromORM:
+    """
+    This class contains basic methods extracted from ORM source code. Developed for the need of the Leighton Lab.
+    Add orm-like methods to the agents. That are:
+
+        - movement that take into account 'resistance' to the movement (i.e. each agent movement has a probability of
+          success that depends on the user's landscape;
+        - when an agent fails to move (for any reason), its displacement ends for the current timestep;
+        - add a form of discrete correlated random walk, using the hexagonal structure of ORM landscapes (see
+          dispersion);
+        - add a series of ways to modelize natural mortality, as found in ORM code;
+        - some methods make the assumption that each timestep represent a week, with 52 weeks in a year.
+
+    IMPORTANT: for some methods, the underlying graph is assumed to come from an ORM xml using the class
+               GraphFromORMxml
+    """
+    def __init__(self, **kwargs):
+        self.df_population['has_moved'] = False
+        self.dict_default_val['has_moved'] = False
+
+    def orm_dispersion(self, timestep, permissible_weeks, condition, arr_nb_steps, arr_prob_nb_steps,
+                       position_attribute='position', territory_attribute='territory', reflexion=False):
+        """
+        This method ignores resistance to movement.
+
+        In the ORM, agents' dispersion is dealt with on a yearly basis. That is, each year (52 timesteps each
+        representing a week) an agent will disperse once and only once. This method takes care of checking if an agent
+        already dispersed or not. When an agent disperse, it draws a number of steps and performs a discrete
+        correlated random walk on the hexagonal landscape. At first, the agent choses a random direction among the six
+        possible neighbours of its current cell (North, north-east, south-est, etc. See GraphORMXml description for
+        details). If there is no cell in that direction, dispersion stops (but it is still counted as if the agent
+        dispersed this year). If there is one, the agent jumps to this new cell, then a new direction is picked: with a
+        60% chance the direction remains unchanged, with 20% it turns left by one notch (if for instance the first
+        direction was North-east, then there is a 20% chance that the next direction will be North), with 20% it turns
+        right. We then repeat the process until the agent has made all its steps.
+
+        IMPORTANT: This method assumes agents are living on a GraphFromORMxml.
+        Warning: If reflexion is used, there might be a bias since we recycle an already used random value.
+
+        :param timestep: current timestep, number of week since simulation started (starts at 0).
+        :param permissible_weeks: array-like object of integer saying which week of the year the agents can disperse
+                                  (counted from 0 to 51).
+        :param condition: 1D array of bool of shape (nb_agents,) saying which agents are allowed to disperse.
+        :param arr_nb_steps: 1D array of non-negative integers, works in tandem with arr_prob_nb_steps.
+        :param arr_prob_nb_steps: 1D array of float, each between 0 and 1. arr_prob_nb_steps[i] is the probability for
+                                  a dispersing agent to do arr_nb_steps[i] steps. Note that this number of step can be
+                                  0. Effectively, this would lead to the agent "having dispersed this year" yet without
+                                  having moved.
+        :param position_attribute: optional, string, default 'position'. Name of the position attribute in the agents.
+        :param territory_attribute: optional, string, default 'territory'. Name of the territory attribute in the
+                                    agents.
+        :param reflexion: optionnal, boolean, default False.
+        """
+        if self.df_population.nb_rows == 0:
+            return
+
+        # we reinitialize the 'has_moved' status if first week of the year
+        if timestep % 52 == 0:
+            self.df_population['has_moved'] = False
+
+        if timestep % 52 not in permissible_weeks:
+            return
+
+        can_move = condition & ~self.df_population['has_moved']
+        will_move = np.random.uniform(0, 1, can_move.sum()) < \
+                    (permissible_weeks.index(timestep % 52) + 1) / len(permissible_weeks)
+        prob = arr_prob_nb_steps.astype('float64')
+        prob = prob / prob.sum()
+        rand_nb_steps = np.random.choice(arr_nb_steps, will_move.sum(), p=prob)
+        rand_directions = np.random.uniform(0, 1, rand_nb_steps.sum())
+
+        if reflexion:
+            orm_like_agent_dispersion_with_reflexion(can_move, will_move, rand_nb_steps, rand_directions,
+                                                     self.df_population[position_attribute],
+                                                     self.df_population[territory_attribute],
+                                                     self.df_population['has_moved'],
+                                                     self.graph.connections, self.graph.weights)
+        else:
+            orm_like_agent_orm_dispersion(can_move, will_move, rand_nb_steps, rand_directions,
+                                          self.df_population[position_attribute],
+                                          self.df_population[territory_attribute],
+                                          self.df_population['has_moved'],
+                                          self.graph.connections)
+
+    def orm_dispersion_with_resistance(self, timestep, permissible_weeks, condition, arr_nb_steps, arr_prob_nb_steps,
+                                       position_attribute='position', territory_attribute='territory'):
+        """
+        This method included resistance to movement.
+
+        In the ORM, agents' dispersion is dealt with on a yearly basis. That is, each year (52 timesteps each
+        representing a week) an agent will disperse once and only once. This method takes care of checking if an agent
+        already dispersed or not. When an agent disperse, it draws a number of steps and performs a discrete
+        correlated random walk on the hexagonal landscape. At first, the agent choses a random direction among the six
+        possible neighbours of its current cell (North, north-east, south-est, etc. See GraphORMXml description for
+        details). If there is no cell in that direction, dispersion stops (but it is still counted as if the agent
+        dispersed this year). If there is one, the agent jumps to this new cell, then a new direction is picked: with a
+        60% chance the direction remains unchanged, with 20% it turns left by one notch (if for instance the first
+        direction was North-east, then there is a 20% chance that the next direction will be North), with 20% it turns
+        right. We then repeat the process until the agent has made all its steps.
+
+        IMPORTANT: This method assumes agents are living on a GraphFromORMxml.
+        Warning: If reflexion is used, there might be a bias since we recycle an already used random value.
+
+        :param timestep: current timestep, number of week since simulation started (starts at 0).
+        :param permissible_weeks: array-like object of integer saying which week of the year the agents can disperse
+                                  (counted from 0 to 51).
+        :param condition: 1D array of bool of shape (nb_agents,) saying which agents are allowed to disperse.
+        :param arr_nb_steps: 1D array of non-negative integers, works in tandem with arr_prob_nb_steps.
+        :param arr_prob_nb_steps: 1D array of float, each between 0 and 1. arr_prob_nb_steps[i] is the probability for
+                                  a dispersing agent to do arr_nb_steps[i] steps. Note that this number of step can be
+                                  0. Effectively, this would lead to the agent "having dispersed this year" yet without
+                                  having moved.
+        :param position_attribute: optional, string, default 'position'. Name of the position attribute in the agents.
+        :param territory_attribute: optional, string, default 'territory'. Name of the territory attribute in the
+                                    agents.
+        """
+        if self.df_population.nb_rows == 0:
+            return
+
+        # we reinitialize the 'has_moved' status if first week of the year
+        if timestep % 52 == 0:
+            self.df_population['has_moved'] = False
+
+        if timestep % 52 not in permissible_weeks:
+            return
+
+        can_move = condition & ~self.df_population['has_moved']
+        will_move = np.random.uniform(0, 1, can_move.sum()) < \
+                    (permissible_weeks.index(timestep % 52) + 1) / len(permissible_weeks)
+        prob = arr_prob_nb_steps.astype('float64')
+        prob = prob / prob.sum()
+        rand_nb_steps = np.random.choice(arr_nb_steps, will_move.sum(), p=prob)
+        rand_directions = np.random.uniform(0, 1, rand_nb_steps.sum())
+        rand_res = np.random.uniform(0, 1, rand_nb_steps.sum())
+
+        orm_like_agent_orm_dispersion_with_resistance(can_move, will_move, rand_nb_steps, rand_directions,
+                                                      self.df_population[position_attribute],
+                                                      self.df_population[territory_attribute],
+                                                      self.df_population['has_moved'], self.graph.connections,
+                                                      self.graph.prob_successful_move,
+                                                      rand_res)
+
+    def mov_around_with_resistance(self,
+                                   proba_remain_on_territory,
+                                   condition=None,
+                                   territory_attribute='territory',
+                                   position_attribute='position'):
+        """
+        This method includes movement resistance. Update the average position of the agent around its territory during
+        the current time step.
+
+        :param proba_remain_on_territory: float, probability to stay on the territory
+        :param condition: optional, array of bool, default None. Array of boolean such that the i-th value is
+                          True if and only if the i-th agent (i.e. the agent at the line i of df_population) can
+                          move.
+        :param territory_attribute: optional, string, default 'territory'
+        :param position_attribute: optional, string, default 'position'
+        """
+        if self.df_population.nb_rows == 0:
+            return
+
+        if condition is not None:
+            pre_bool_mov = np.random.uniform(0, 1, condition.sum()) > proba_remain_on_territory
+            bool_mov = movement_mov_around_territory_fill_bool_mov_using_condition(pre_bool_mov, condition)
+        else:
+            bool_mov = np.random.uniform(0, 1, self.df_population.shape[0]) > proba_remain_on_territory
+
+        rand_direction = np.random.uniform(0, 1, bool_mov.sum())
+        rand_res = np.random.uniform(0, 1, bool_mov.sum())
+
+        orm_like_agents_mov_around_with_resistance(self.df_population[territory_attribute],
+                                                   self.df_population[position_attribute],
+                                                   self.graph.connections, self.graph.weights,
+                                                   self.graph.prob_successful_move, bool_mov, rand_direction,
+                                                   rand_res)
+
+    def _mortality_from_v08(self, arr_annual_mortality, condition_count, alpha_beta=None, condition=None,
+                            shuffle=True, age_attribute='age', position_attribute='position'):
+        """
+        (made by Francois Viard)
+
+        This is an adaptation of the mortality method found in ARM v08 (file cFox.cs). ARM is not a typo, it is the
+        'Arctic Rabies Model', which is a variation of ORM. I don't think it's been published or used in publication?
+
+        WARNING: There are no sources given in the ORM file for the origin of this method. As such, I cannot guarantee
+                 that I correctly understood what it is supposed to do and why. Therefore, this method is considered
+                 private and should be use with caution.
+
+        :param arr_annual_mortality: array of float between 0 and 1. arr_annual_mortality[i] is the target probability
+                                     for an agent to die at age i.
+        :param condition_count: 1D array of bool, tells which agent to count.
+        :param alpha_beta: Absolute mystery. In the formula used in ARM there is an Alpha and a Beta, but I could not
+                           figure out if those were actually modified or if the default values were always taken. I
+                           finally decided to postpone the inclusion of those option to a later date... However,
+                           every project finally moved away from this method and fell back to the usual ORM mortality.
+                           As it is, DO NOT USE THIS KWARGS.
+        :param condition: optional, 1D array of bool, default None. If not None, tells which agents can die.
+        :param shuffle: optional, bool, default True. If True, shuffle the population dataframe before applying method
+        :param age_attribute: optional, string, default 'age'. Name of the age attribute of the agents.
+        :param position_attribute: optional, string, default 'position'. Name of the position attribute of the agents.
+        """
+        if self.df_population.nb_rows == 0:
+            return
+
+        if shuffle:
+            permutation = self.df_population.scramble(return_permutation=True)
+            if condition is not None:
+                condition = condition[permutation]
+            condition_count = condition_count[permutation]
+
+        count_arr = self.count_pop_per_vertex(position_attribute=position_attribute, condition=condition_count)
+        if alpha_beta is None:
+            if condition is None:
+                rand = np.random.uniform(0, 1, self.df_population.nb_rows)
+                survive = orm_like_agents_mortality_from_v08_no_condition_no_alpha_beta(count_arr, condition_count,
+                                                                                        self.df_population[position_attribute],
+                                                                                        self.graph.df_attributes['K'],
+                                                                                        arr_annual_mortality,
+                                                                                        self.df_population[age_attribute],
+                                                                                        rand)
+            else:
+                rand = np.random.uniform(0, 1, self.df_population.nb_rows)
+                survive = orm_like_agents_mortality_from_v08_with_condition_no_alpha_beta(count_arr, condition_count,
+                                                                                          self.df_population[
+                                                                                            position_attribute],
+                                                                                          self.graph.df_attributes['K'],
+                                                                                          arr_annual_mortality,
+                                                                                          self.df_population[
+                                                                                            age_attribute],
+                                                                                          rand, condition)
+        self.df_population = self.df_population[survive]
+
+    def _mortality_from_v08_with_gender(self, arr_female_annual_mortality, arr_male_annual_mortality, condition_count,
+                                        alpha_beta=None, condition=None, shuffle=True, age_attribute='age',
+                                        position_attribute='position', gender_attribute='gender'):
+        """
+        (made by Francois Viard)
+
+        This is an adaptation of the mortality method found in ARM v08 (file cFox.cs). ARM is not a typo, it is the
+        'Arctic Rabies Model', which is a variation of ORM. I don't think it's been published or used in publication?
+
+        WARNING: There are no sources given in the ORM file for the origin of this method. As such, I cannot guarantee
+                 that I correctly understood what it is supposed to do and why. Therefore, this method is considered
+                 private and should be use with caution.
+
+        :param arr_female_annual_mortality: array of float between 0 and 1. arr_annual_mortality[i] is the target
+                                    probability for a female agent to die at age i.
+        :param arr_male_annual_mortality: array of float between 0 and 1. arr_annual_mortality[i] is the target
+                                    probability for a male agent to die at age i.
+        :param condition_count: 1D array of bool, tells which agent to count.
+        :param alpha_beta: Absolute mystery. In the formula used in ARM there is an Alpha and a Beta, but I could not
+                           figure out if those were actually modified or if the default values were always taken. I
+                           finally decided to postpone the inclusion of those option to a later date... However,
+                           every project finally moved away from this method and fell back to the usual ORM mortality.
+                           As it is, DO NOT USE THIS KWARGS.
+        :param condition: optional, 1D array of bool, default None. If not None, tells which agents can die.
+        :param shuffle: optional, bool, default True. If True, shuffle the population dataframe before applying method
+        :param age_attribute: optional, string, default 'age'. Name of the age attribute of the agents.
+        :param position_attribute: optional, string, default 'position'. Name of the position attribute of the agents.
+        :param gender_attribute: optional, string, default 'gender'. Name of the gender attribute of the agents.
+        """
+        if self.df_population.nb_rows == 0:
+            return
+
+        if shuffle:
+            permutation = self.df_population.scramble(return_permutation=True)
+            if condition is not None:
+                condition = condition[permutation]
+            condition_count = condition_count[permutation]
+
+        count_arr = self.count_pop_per_vertex(position_attribute=position_attribute, condition=condition_count)
+        if alpha_beta is None:
+            if condition is None:
+                rand = np.random.uniform(0, 1, self.df_population.nb_rows)
+                survive = orm_like_agents_mortality_from_v08_with_gender_no_condition_no_alpha_beta(count_arr,
+                                                                                condition_count,
+                                                                                self.df_population[position_attribute],
+                                                                                self.graph.df_attributes['K'],
+                                                                                self.df_population[gender_attribute],
+                                                                                arr_female_annual_mortality,
+                                                                                arr_male_annual_mortality,
+                                                                                self.df_population[age_attribute],
+                                                                                rand)
+            else:
+                rand = np.random.uniform(0, 1, (condition.sum(),))
+                survive = orm_like_agents_mortality_from_v08_with_gender_with_condition_no_alpha_beta(count_arr,
+                                                                                condition_count,
+                                                                                self.df_population[position_attribute],
+                                                                                self.graph.df_attributes['K'],
+                                                                                self.df_population[gender_attribute],
+                                                                                arr_female_annual_mortality,
+                                                                                arr_male_annual_mortality,
+                                                                                self.df_population[age_attribute],
+                                                                                rand,
+                                                                                condition)
+        self.df_population = self.df_population[survive]
+
+
+class ExperimentalDensityDependentMortality:
+    """
+    Some experiments that will be moved elsewhere soon.
+    """
+    def __init__(self, **kwargs):
+        self._corrected_beta_female = None
+        self._corrected_beta_male = None
+
+    def compute_and_save_beta_female(self, alpha, arr_female_weekly_mortality):
+        self._corrected_beta_female = 1. + (1. / alpha) * np.log((1. / arr_female_weekly_mortality) - 1.)
+
+    def compute_and_save_beta_male(self, alpha, arr_male_weekly_mortality):
+        self._corrected_beta_male = 1. + (1. / alpha) * np.log((1. / arr_male_weekly_mortality) - 1.)
+
+    def experimental_mortality_logistic_function(self, alpha, arr_female_weekly_mortality, arr_male_weekly_mortality,
+                                                 age_attribute='age', position_attribute='position', k_attribute='K',
+                                                 shuffle=True, gender_attribute='gender'):
+        if self._corrected_beta_female is None:
+            self.compute_and_save_beta_female(alpha, arr_female_weekly_mortality)
+        if self._corrected_beta_male is None:
+            self.compute_and_save_beta_male(alpha, arr_male_weekly_mortality)
+        if shuffle:
+            self.df_population.scramble()
+        count_arr = self.count_pop_per_vertex(position_attribute=position_attribute)
+        rand = np.random.uniform(0, 1, (self.df_population.nb_rows,))
+        survive = experimental_density_mortality(count_arr, self.df_population[position_attribute],
+                                                 self.df_population[age_attribute],
+                                                 self.graph.df_attributes[k_attribute],
+                                                 self.df_population[gender_attribute],
+                                                 self._corrected_beta_male, self._corrected_beta_female,
+                                                 alpha, rand)
+        self.df_population = self.df_population[survive]
+
+
+@sampy_class
+class ORMLikeAgent(BaseAgingAgent,
+                   NaturalMortalityOrmMethodology,
+                   OffspringDependantOnParents,
+                   FindMateMonogamous,
+                   OffspringCreationWithCustomProb,
+                   TerritorialMovementWithoutResistance,
+                   ComponentsFromORM):
+    """
+    Basic ORM like agents.
+
+    Includes main components from SamPy plus the building block 'ComponentsFromORM'.
+
+    :param graph: Mandatory kwargs, a graph object. Some methods expect this to be a "GraphFromORMXml' object.
+    """
+    def __init__(self, **kwargs):
+        pass
+
+
+@sampy_class
+class ORMMongooses(BaseAgingAgent,
+                   NaturalMortalityOrmMethodology,
+                   OffspringDependantOnParents,
+                   FindMatePolygamous,
+                   OffspringCreationWithCustomProb,
+                   TerritorialMovementWithoutResistance,
+                   ComponentsFromORM):
+    """
+    Mongooses from ORM with some updates for Caroline Sauve projects.
+    Includes main components from SamPy plus the building block 'ComponentsFromORM'.
+
+    :param graph: Mandatory kwargs, a graph object. Some methods expect this to be a GraphFromORMXml object.
+    :param pregnancy_duration: mandatory kwargs, an integer. Duration in weeks of pregnancy.
+    """
+    def __init__(self, pregnancy_duration=None, **kwargs):
+        if pregnancy_duration is None:
+            raise ValueError("A value for pregnancy duration should be given using kwarg 'pregnancy_duration'")
+        self.pregnancy_duration = pregnancy_duration
+        self.df_population['nb_weeks_being_pregnant'] = 0
+        self.dict_default_val['nb_weeks_being_pregnant'] = 0
+
+        self.df_population['week_next_potential_mating'] = -1
+        self.dict_default_val['week_next_potential_mating'] = -1
+
+    def increment_number_of_weeks_of_pregnancy(self):
+        """
+        Mongoose object keeps track of pregnancy duration with individual counters. This method increments those
+        counters. Should be called weekly.
+        """
+        self.df_population['nb_weeks_being_pregnant'] += self.df_population['is_pregnant']
+
+    def check_if_mother_free_of_dependent_young(self, age_independence, min_age_reproduction, mother_attribute='mom_id',
+                                                id_attribute='col_id', age_attribute='age'):
+        """
+        Checks which females old enough to reproduce do not have offsprings.
+
+        :param age_independence: integer, age at which offspring can live on their own.
+        :param min_age_reproduction: integer, age at which females can reproduce.
+        :param mother_attribute: optional, string, default 'mom_id'. Name of the attribute giving the id of the mother
+                                 of each agent.
+        :param id_attribute: optional, string, default 'col_id'. Name of the attribute containing the id of the agents.
+        :param age_attribute: optional, string, default 'age'. Name of the attribute containing the age of the agents.
+
+        :return: 1D array of bool, where return[i] is True if and only if the i-th agent is a Female available for
+                 reproduction.
+        """
+        offsprings = self.df_population[age_attribute] < age_independence
+        mom_id_offsprings = self.df_population[mother_attribute][offsprings]
+        potential_mothers = (self.df_population[age_attribute] >= min_age_reproduction) & self.get_females()
+        orm_mongooses_check_if_mother_free_of_juveniles(mom_id_offsprings, self.df_population[id_attribute],
+                                                        potential_mothers)
+        return potential_mothers
+
+    def give_birth_if_needed(self, arr_nb_children, arr_prob_nb_children, condition=None, prob_failure=None):
+        """
+        Make each female that reached the end of their pregnancy period give birth.
+
+        :param arr_nb_children: 1D array of integer, works in tandem with arr_prob_nb_children below.
+        :param arr_prob_nb_children: 1D array of float between 0 and 1. arr_prob_nb_children[i] is the probability for
+                                     a female giving birth to have arr_nb_children[i] offsprings.
+        :param condition: optional, 1D array of bool, default None. If not None, tells which female agents can give
+                          birth.
+        :param prob_failure: optional, float between 0 and 1, default one. If not None, gives the probability for the
+                             agent to fail giving birth. Note that this is equivalent with putting 0 as a possible value
+                             in arr_nb_children, and we recommend user to chose one solution or the other.
+        """
+        about_to_give_birth = (self.df_population['nb_weeks_being_pregnant'] >= self.pregnancy_duration)
+        if condition is None:
+            condition = about_to_give_birth
+        else:
+            condition = condition & about_to_give_birth
+        self.df_population['nb_weeks_being_pregnant'] *= ~condition
+        self.create_offsprings_custom_prob(arr_nb_children, arr_prob_nb_children, condition=condition,
+                                           prob_failure=prob_failure)
+
+    def children_follow_their_mom(self, min_age, max_age, age_attribute='age', mom_id_attribute='mom_id',
+                                  id_attribute='col_id', position_attribute='position',
+                                  territory_attribute='territory'):
+        youngs = (self.df_population[age_attribute] >= min_age) & (self.df_population[age_attribute] <= max_age)
+        id_moms = self.df_population[mom_id_attribute][youngs]
+        orm_mongooses_update_ter_pos_youngs(id_moms, youngs, self.df_population[territory_attribute],
+                                            self.df_population[position_attribute], self.df_population[id_attribute],
+                                            self.df_population[mom_id_attribute])
+
+    def weekly_mating_checks_and_update(self, current_week, mean_mate_weeks, var_mate_weeks, age_independence,
+                                        min_age_reproduction, gender_attribute='gender', mother_attribute='mom_id',
+                                        id_attribute='col_id', age_attribute='age', position_attribute='position',
+                                        pregnancy_attribute='is_pregnant', mate_attribute='current_mate'):
+        """
+        Method written in order to reproduce the multiple reproduction spikes that can be seen in Mongooses.
+
+        :param current_week: integer, value between 0 and 51 representing the current week of the year.
+        :param mean_mate_weeks:
+        :param var_mate_weeks:
+        :param age_independence:
+        :param min_age_reproduction:
+        :param gender_attribute:
+        :param mother_attribute:
+        :param id_attribute:
+        :param age_attribute:
+        :param position_attribute:
+        :param pregnancy_attribute:
+        :param mate_attribute:
+        """
+
+        # we begin with making the females ready to mate attempt to, well, mate
+        potentially_mating_females = self.df_population['week_next_potential_mating'] == current_week
+        if potentially_mating_females.sum() > 0:
+            female_available = self.check_if_mother_free_of_dependent_young(age_independence, min_age_reproduction,
+                                                                            gender_attribute=gender_attribute,
+                                                                            mother_attribute=mother_attribute,
+                                                                            id_attribute=id_attribute,
+                                                                            age_attribute=age_attribute)
+            female_available = female_available & ~self.df_population[pregnancy_attribute]
+            mating_females = potentially_mating_females & female_available
+            mating_males = self.get_males() & (self.df_population[age_attribute] >= min_age_reproduction)
+            self.find_random_mate_on_position(1., condition=(mating_females | mating_males), id_attribute=id_attribute,
+                                              position_attribute=position_attribute, gender_attribute=gender_attribute,
+                                              mate_attribute=mate_attribute, pregnancy_attribute=pregnancy_attribute)
+
+        # we now (re)-initialize the "week_next_potential_mating" attribute
+        init_next_week = potentially_mating_females | ((self.df_population['week_next_potential_mating'] == -1) &
+                                                       (self.df_population[age_attribute] >= min_age_reproduction))
+        nb_init_to_perform = init_next_week.sum()
+        if nb_init_to_perform > 0:
+            rand_gauss = np.random.normal(0, 1, (nb_init_to_perform,))
+            orm_mongooses_update_mating_week(current_week, mean_mate_weeks, var_mate_weeks,
+                                             self.df_population['week_next_potential_mating'],
+                                             init_next_week, rand_gauss)
+
+
+
```

### Comparing `sampy-abm-1.0.2/src/sampy/addons/ORM_related_addons/graph_from_ORM_xml.py` & `sampy_abm-1.0.3/src/sampy/addons/ORM_related_addons/graph_from_ORM_xml.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-from ...graph.topology import BaseTopology
-from ...graph.vertex_attributes import BaseVertexAttributes, PeriodicAttributes
-from ...utils.decorators import sampy_class
-import xml.etree.ElementTree as ET
-import numpy as np
-
-
-@sampy_class
-class GraphFromORMxml(BaseTopology,
-                      BaseVertexAttributes,
-                      PeriodicAttributes):
-    """
-    Class developed for the need of the Leighton Lab. The graph structure is read from an XML, as generated by Badr
-    QGIS module.
-
-    The obtained graph has a hexagonal structure (i.e. each vertex represents a hexagonal cell), where each vertex has
-    an orientation. That is, a vertex has a north neighbour, a north-east one, a south-east one, etc... Vertices come
-    with several attributes : 'K' measuring the carrying capacity, 'in-res' measuring how hard it is to get into a cell,
-    'out-res' measuring how hard it is to leave a cell.
-
-    Those two last resistance values are compressed into a 2D array of same shape as connections called
-    prob_successful_move, that gives the probability for a movement along an edge to be successful.
-
-    Finally, each cell belongs to some category, called a "super-cell". You can access them via methods below.
-    """
-    def __init__(self, path_to_xml=None):
-        if path_to_xml is None:
-            raise ValueError("A path to an ORM XML should be provided.")
-
-        tree = ET.parse(path_to_xml)
-        root = tree.getroot()
-
-        # get super_cells info
-        self.dict_super_cell = {}
-        counter = 0
-        for super_cell in root.findall('SuperCells'):
-            temp_dict = {}
-            for info in super_cell:
-                temp_dict[info.tag] = info.text
-            self.dict_super_cell[temp_dict['ID']] = {'index': counter,
-                                                     'in_res': float(temp_dict['InResistance'])/100.,
-                                                     'out_res': float(temp_dict['OutResistance'])/100.}
-            counter += 1
-
-        # read the various parameters to create a sampy graph
-        counter = 0
-        for cell in root.findall('AllCellData'):
-            id_cell = cell.find('HEXID').text
-            if id_cell not in self.dict_cell_id_to_ind:
-                self.dict_cell_id_to_ind[id_cell] = counter
-                counter += 1
-            else:
-                raise ValueError("The cell " + id_cell + " is defined two times in the xml.")
-
-        self.connections = np.full((counter, 6), -1, dtype=np.int32)
-        self.weights = np.full((counter, 6), -1.)
-        self.prob_successful_move = np.full((counter, 6), -1.)
-        self.df_attributes['K'] = np.full((counter,), 0.)
-        self.df_attributes['in_res'] = np.full((counter,), 0.)
-        self.df_attributes['out_res'] = np.full((counter,), 0.)
-        self.df_attributes['super_cell'] = np.full((counter,), 0)
-        self.df_attributes['easting'] = np.full((counter,), 0.)
-        self.df_attributes['northing'] = np.full((counter,), 0.)
-        array_nb_neighbours = np.full((counter,), 0, dtype=np.int8)
-
-        for cell in root.findall('AllCellData'):
-            index_cell = self.dict_cell_id_to_ind[cell.find('HEXID').text]
-            for info in cell:
-
-                if info.tag == 'N':
-                    if info.text != 'b' and info.text in self.dict_cell_id_to_ind:
-                        self.connections[index_cell][0] = self.dict_cell_id_to_ind[info.text]
-                        array_nb_neighbours[index_cell] += 1
-                if info.tag == 'NE':
-                    if info.text != 'b' and info.text in self.dict_cell_id_to_ind:
-                        self.connections[index_cell][1] = self.dict_cell_id_to_ind[info.text]
-                        array_nb_neighbours[index_cell] += 1
-                if info.tag == 'SE':
-                    if info.text != 'b' and info.text in self.dict_cell_id_to_ind:
-                        self.connections[index_cell][2] = self.dict_cell_id_to_ind[info.text]
-                        array_nb_neighbours[index_cell] += 1
-                if info.tag == 'S':
-                    if info.text != 'b' and info.text in self.dict_cell_id_to_ind:
-                        self.connections[index_cell][3] = self.dict_cell_id_to_ind[info.text]
-                        array_nb_neighbours[index_cell] += 1
-                if info.tag == 'SW':
-                    if info.text != 'b' and info.text in self.dict_cell_id_to_ind:
-                        self.connections[index_cell][4] = self.dict_cell_id_to_ind[info.text]
-                        array_nb_neighbours[index_cell] += 1
-                if info.tag == 'NW':
-                    if info.text != 'b' and info.text in self.dict_cell_id_to_ind:
-                        self.connections[index_cell][5] = self.dict_cell_id_to_ind[info.text]
-                        array_nb_neighbours[index_cell] += 1
-
-                elif info.tag == 'K':
-                    self.df_attributes['K'][index_cell] = float(info.text)
-                elif info.tag == 'supercell':
-                    self.df_attributes['super_cell'][index_cell] = self.dict_super_cell[info.text]['index']
-                    self.df_attributes['in_res'][index_cell] = self.dict_super_cell[info.text]['in_res']
-                    self.df_attributes['out_res'][index_cell] = self.dict_super_cell[info.text]['out_res']
-                elif info.tag == 'easting':
-                    self.df_attributes['easting'][index_cell] = float(info.text)
-                elif info.tag == 'northing':
-                    self.df_attributes['northing'][index_cell] = float(info.text)
-
-        # we now populate the weights array
-        for i in range(self.connections.shape[0]):
-            nb_neighbours = array_nb_neighbours[i]
-            seen_neighb = 0
-            if nb_neighbours == 0:
-                continue
-            for j in range(6):
-                if self.connections[i][j] != -1:
-
-                    self.prob_successful_move[i][j] = (1. - self.df_attributes['out_res'][i]) * \
-                                                      (1. - self.df_attributes['in_res'][self.connections[i][j]])
-
-                    seen_neighb += 1
-                    if seen_neighb == nb_neighbours:
-                        self.weights[i][j] = 1.
-                        break
-                    else:
-                        self.weights[i][j] = float(seen_neighb)/float(nb_neighbours)
-
-    def get_super_cell(self, name_super_cell):
-        """
-        Get a 1D array of bool arr_cell, where arr_cell[i] is True if and only if the cell of index i is a super-cell
-        of the requested category.
-
-        :param name_super_cell: String, the kind of super-cell you want the list of.
-
-        :return: 1D array of bool
-        """
-        return self.df_attributes['super_cell'] == self.dict_super_cell[name_super_cell]['index']
-
-    @property
-    def list_super_cell_names(self):
-        """
-        Gives you the list of all the supercells present in your landscape.
-
-        :return: a list of string
-        """
-        return [super_cell_name for super_cell_name in self.dict_super_cell]
+from ...graph.topology import BaseTopology
+from ...graph.vertex_attributes import BaseVertexAttributes, PeriodicAttributes
+from ...utils.decorators import sampy_class
+import xml.etree.ElementTree as ET
+import numpy as np
+
+
+@sampy_class
+class GraphFromORMxml(BaseTopology,
+                      BaseVertexAttributes,
+                      PeriodicAttributes):
+    """
+    Class developed for the need of the Leighton Lab. The graph structure is read from an XML, as generated by Badr
+    QGIS module.
+
+    The obtained graph has a hexagonal structure (i.e. each vertex represents a hexagonal cell), where each vertex has
+    an orientation. That is, a vertex has a north neighbour, a north-east one, a south-east one, etc... Vertices come
+    with several attributes : 'K' measuring the carrying capacity, 'in-res' measuring how hard it is to get into a cell,
+    'out-res' measuring how hard it is to leave a cell.
+
+    Those two last resistance values are compressed into a 2D array of same shape as connections called
+    prob_successful_move, that gives the probability for a movement along an edge to be successful.
+
+    Finally, each cell belongs to some category, called a "super-cell". You can access them via methods below.
+    """
+    def __init__(self, path_to_xml=None):
+        if path_to_xml is None:
+            raise ValueError("A path to an ORM XML should be provided.")
+
+        tree = ET.parse(path_to_xml)
+        root = tree.getroot()
+
+        # get super_cells info
+        self.dict_super_cell = {}
+        counter = 0
+        for super_cell in root.findall('SuperCells'):
+            temp_dict = {}
+            for info in super_cell:
+                temp_dict[info.tag] = info.text
+            self.dict_super_cell[temp_dict['ID']] = {'index': counter,
+                                                     'in_res': float(temp_dict['InResistance'])/100.,
+                                                     'out_res': float(temp_dict['OutResistance'])/100.}
+            counter += 1
+
+        # read the various parameters to create a sampy graph
+        counter = 0
+        for cell in root.findall('AllCellData'):
+            id_cell = cell.find('HEXID').text
+            if id_cell not in self.dict_cell_id_to_ind:
+                self.dict_cell_id_to_ind[id_cell] = counter
+                counter += 1
+            else:
+                raise ValueError("The cell " + id_cell + " is defined two times in the xml.")
+
+        self.connections = np.full((counter, 6), -1, dtype=np.int32)
+        self.weights = np.full((counter, 6), -1.)
+        self.prob_successful_move = np.full((counter, 6), -1.)
+        self.df_attributes['K'] = np.full((counter,), 0.)
+        self.df_attributes['in_res'] = np.full((counter,), 0.)
+        self.df_attributes['out_res'] = np.full((counter,), 0.)
+        self.df_attributes['super_cell'] = np.full((counter,), 0)
+        self.df_attributes['easting'] = np.full((counter,), 0.)
+        self.df_attributes['northing'] = np.full((counter,), 0.)
+        array_nb_neighbours = np.full((counter,), 0, dtype=np.int8)
+
+        for cell in root.findall('AllCellData'):
+            index_cell = self.dict_cell_id_to_ind[cell.find('HEXID').text]
+            for info in cell:
+
+                if info.tag == 'N':
+                    if info.text != 'b' and info.text in self.dict_cell_id_to_ind:
+                        self.connections[index_cell][0] = self.dict_cell_id_to_ind[info.text]
+                        array_nb_neighbours[index_cell] += 1
+                if info.tag == 'NE':
+                    if info.text != 'b' and info.text in self.dict_cell_id_to_ind:
+                        self.connections[index_cell][1] = self.dict_cell_id_to_ind[info.text]
+                        array_nb_neighbours[index_cell] += 1
+                if info.tag == 'SE':
+                    if info.text != 'b' and info.text in self.dict_cell_id_to_ind:
+                        self.connections[index_cell][2] = self.dict_cell_id_to_ind[info.text]
+                        array_nb_neighbours[index_cell] += 1
+                if info.tag == 'S':
+                    if info.text != 'b' and info.text in self.dict_cell_id_to_ind:
+                        self.connections[index_cell][3] = self.dict_cell_id_to_ind[info.text]
+                        array_nb_neighbours[index_cell] += 1
+                if info.tag == 'SW':
+                    if info.text != 'b' and info.text in self.dict_cell_id_to_ind:
+                        self.connections[index_cell][4] = self.dict_cell_id_to_ind[info.text]
+                        array_nb_neighbours[index_cell] += 1
+                if info.tag == 'NW':
+                    if info.text != 'b' and info.text in self.dict_cell_id_to_ind:
+                        self.connections[index_cell][5] = self.dict_cell_id_to_ind[info.text]
+                        array_nb_neighbours[index_cell] += 1
+
+                elif info.tag == 'K':
+                    self.df_attributes['K'][index_cell] = float(info.text)
+                elif info.tag == 'supercell':
+                    self.df_attributes['super_cell'][index_cell] = self.dict_super_cell[info.text]['index']
+                    self.df_attributes['in_res'][index_cell] = self.dict_super_cell[info.text]['in_res']
+                    self.df_attributes['out_res'][index_cell] = self.dict_super_cell[info.text]['out_res']
+                elif info.tag == 'easting':
+                    self.df_attributes['easting'][index_cell] = float(info.text)
+                elif info.tag == 'northing':
+                    self.df_attributes['northing'][index_cell] = float(info.text)
+
+        # we now populate the weights array
+        for i in range(self.connections.shape[0]):
+            nb_neighbours = array_nb_neighbours[i]
+            seen_neighb = 0
+            if nb_neighbours == 0:
+                continue
+            for j in range(6):
+                if self.connections[i][j] != -1:
+
+                    self.prob_successful_move[i][j] = (1. - self.df_attributes['out_res'][i]) * \
+                                                      (1. - self.df_attributes['in_res'][self.connections[i][j]])
+
+                    seen_neighb += 1
+                    if seen_neighb == nb_neighbours:
+                        self.weights[i][j] = 1.
+                        break
+                    else:
+                        self.weights[i][j] = float(seen_neighb)/float(nb_neighbours)
+
+    def get_super_cell(self, name_super_cell):
+        """
+        Get a 1D array of bool arr_cell, where arr_cell[i] is True if and only if the cell of index i is a super-cell
+        of the requested category.
+
+        :param name_super_cell: String, the kind of super-cell you want the list of.
+
+        :return: 1D array of bool
+        """
+        return self.df_attributes['super_cell'] == self.dict_super_cell[name_super_cell]['index']
+
+    @property
+    def list_super_cell_names(self):
+        """
+        Gives you the list of all the supercells present in your landscape.
+
+        :return: a list of string
+        """
+        return [super_cell_name for super_cell_name in self.dict_super_cell]
```

### Comparing `sampy-abm-1.0.2/src/sampy/addons/ORM_related_addons/jit_compiled_function.py` & `sampy_abm-1.0.3/src/sampy/addons/ORM_related_addons/jit_compiled_function.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,318 +1,318 @@
-import numpy as np
-import numba as nb
-
-
-@nb.njit
-def orm_like_agent_orm_dispersion(arr_can_move, arr_will_move, arr_rand_nb_steps, arr_rand_direction,
-                                  col_position, col_territory, col_has_moved, connections):
-    counter_arr_will_move = 0
-    counter_arr_rand_nb_steps = 0
-    counter_arr_rand_direction = 0
-    for i in range(arr_can_move.shape[0]):
-        if arr_can_move[i]:
-
-            # first we determine if the agent is allowed to move. If not, we skip to the next agent
-            will_move = arr_will_move[counter_arr_will_move]
-            counter_arr_will_move += 1
-            if not will_move:
-                continue
-
-            # now we update the 'has moved' flag (in ORM, this is done even if the agent moves 0 cells)
-            col_has_moved[i] = True
-
-            nb_steps = arr_rand_nb_steps[counter_arr_rand_nb_steps]
-            counter_arr_rand_nb_steps += 1
-            if nb_steps == 0:
-                continue
-
-            for j in range(nb_steps):
-                rand_direction = arr_rand_direction[counter_arr_rand_direction]
-                counter_arr_rand_direction += 1
-
-                if j == 0:
-                    direction = int(np.floor(rand_direction * 6)) % 6
-                else:
-                    if rand_direction <= 0.2:
-                        direction = (direction - 1) % 6
-                    elif rand_direction >= 0.8:
-                        direction = (direction + 1) % 6
-
-                if connections[col_territory[i]][direction] == -1:
-                    break
-
-                col_position[i] = connections[col_territory[i]][direction]
-                col_territory[i] = connections[col_territory[i]][direction]
-
-
-@nb.njit
-def orm_like_agent_dispersion_with_reflexion(arr_can_move, arr_will_move, arr_rand_nb_steps, arr_rand_direction,
-                                             col_position, col_territory, col_has_moved, connections, weights):
-    counter_arr_will_move = 0
-    counter_arr_rand_nb_steps = 0
-    counter_arr_rand_direction = 0
-    for i in range(arr_can_move.shape[0]):
-        if arr_can_move[i]:
-
-            # first we determine if the agent is allowed to move. If not, we skip to the next agent
-            will_move = arr_will_move[counter_arr_will_move]
-            counter_arr_will_move += 1
-            if not will_move:
-                continue
-
-            # now we update the 'has moved' flag (in ORM, this is done even if the agent moves 0 cells)
-            col_has_moved[i] = True
-
-            nb_steps = arr_rand_nb_steps[counter_arr_rand_nb_steps]
-            counter_arr_rand_nb_steps += 1
-            if nb_steps == 0:
-                continue
-
-            for j in range(nb_steps):
-                rand_direction = arr_rand_direction[counter_arr_rand_direction]
-                counter_arr_rand_direction += 1
-
-                if j == 0:
-                    direction = int(np.floor(rand_direction * 6)) % 6
-                else:
-                    if rand_direction <= 0.2:
-                        direction = (direction - 1) % 6
-                    elif rand_direction >= 0.8:
-                        direction = (direction + 1) % 6
-
-                if connections[col_territory[i]][direction] == -1:
-                    for k in range(6):
-                        if rand_direction <= weights[col_territory[i]][k]:
-                            col_position[i] = connections[col_territory[i]][k]
-                            col_territory[i] = connections[col_territory[i]][k]
-                            break
-                else:
-                    col_position[i] = connections[col_territory[i]][direction]
-                    col_territory[i] = connections[col_territory[i]][direction]
-
-
-@nb.njit
-def orm_like_agent_orm_dispersion_with_resistance(arr_can_move, arr_will_move, arr_rand_nb_steps, arr_rand_direction,
-                                                  col_position, col_territory, col_has_moved, connections,
-                                                  prob_successful_mov, rand_res):
-    counter_arr_will_move = 0
-    counter_arr_rand_nb_steps = 0
-    counter_arr_rand_direction = 0
-    counter_rand_res = -1
-    for i in range(arr_can_move.shape[0]):
-        if arr_can_move[i]:
-
-            # first we determine if the agent is allowed to move. If not, we skip to the next agent
-            will_move = arr_will_move[counter_arr_will_move]
-            counter_arr_will_move += 1
-            if not will_move:
-                continue
-            # now we update the 'has moved' flag (in ORM, this is done even if the agent moves 0 cells)
-            col_has_moved[i] = True
-
-            nb_steps = arr_rand_nb_steps[counter_arr_rand_nb_steps]
-            counter_arr_rand_nb_steps += 1
-            if nb_steps == 0:
-                continue
-
-            for j in range(nb_steps):
-
-                rand_direction = arr_rand_direction[counter_arr_rand_direction]
-                counter_arr_rand_direction += 1
-
-                if j == 0:
-                    direction = int(np.floor(rand_direction * 6)) % 6
-                else:
-                    if rand_direction <= 0.2:
-                        direction = (direction - 1) % 6
-                    elif rand_direction >= 0.8:
-                        direction = (direction + 1) % 6
-
-                if connections[col_territory[i]][direction] == -1:
-                    break
-
-                counter_rand_res += 1
-                if rand_res[counter_rand_res] >= prob_successful_mov[col_territory[i]][direction]:
-                    break
-
-                col_position[i] = connections[col_territory[i]][direction]
-                col_territory[i] = connections[col_territory[i]][direction]
-
-
-@nb.njit
-def orm_like_agents_mov_around_with_resistance(territory, position, connections, weights, prob_successful_mov,
-                                               arr_bool_mov, rand_direction, rand_res):
-    counter = 0
-    for i in range(territory.shape[0]):
-        if arr_bool_mov[i]:
-            for j in range(6):
-                if rand_direction[counter] <= weights[territory[i]][j]:
-                    if rand_res[counter] <= prob_successful_mov[territory[i]][j]:
-                        position[i] = connections[territory[i]][j]
-                    counter += 1
-                    break
-
-
-@nb.njit
-def orm_like_agents_mortality_from_v08_no_condition_no_alpha_beta(arr_count, arr_condition_count, arr_position, arr_k,
-                                                                  arr_annual_mortality, arr_age, arr_rand):
-    rv = np.full(arr_age.shape, True, dtype=np.bool_)
-    for i in range(rv.shape[0]):
-        if arr_k[arr_position[i]] == 0.:
-            rv[i] = False
-            if arr_condition_count[i]:
-                arr_count[arr_position[i]] -= 1
-            continue
-
-        mort_adjust = float(arr_count[arr_position[i]]) / float(arr_k[arr_position[i]])
-        age_agent = arr_age[i] // 52
-        p0 = 1 - np.exp(-arr_annual_mortality[age_agent])
-        alpha = 4. * 1.5 / p0
-        if arr_rand[i] <= (p0 / (1 + np.exp(-(mort_adjust - 1.5) * alpha))):
-            rv[i] = False
-            if arr_condition_count[i]:
-                arr_count[arr_position[i]] -= 1
-    return rv
-
-
-@nb.njit
-def orm_like_agents_mortality_from_v08_with_gender_no_condition_no_alpha_beta(arr_count, arr_condition_count,
-                                                                              arr_position, arr_k, arr_gender,
-                                                                              arr_female_mortality, arr_male_mortality,
-                                                                              arr_age, arr_rand):
-    rv = np.full(arr_age.shape, True, dtype=np.bool_)
-    for i in range(rv.shape[0]):
-        if arr_k[arr_position[i]] == 0.:
-            rv[i] = False
-            if arr_condition_count[i]:
-                arr_count[arr_position[i]] -= 1
-            continue
-
-        mort_adjust = float(arr_count[arr_position[i]]) / float(arr_k[arr_position[i]])
-        age_agent = arr_age[i] // 52
-        if arr_gender[i] == 0:
-            p0 = 1 - np.exp(-arr_male_mortality[age_agent])
-        else:
-            p0 = 1 - np.exp(-arr_female_mortality[age_agent])
-        alpha = 4. * 1.5 / p0
-        if arr_rand[i] <= (p0 / (1 + np.exp(-(mort_adjust - 1.5) * alpha))):
-            rv[i] = False
-            if arr_condition_count[i]:
-                arr_count[arr_position[i]] -= 1
-    return rv
-
-
-def orm_like_agents_mortality_from_v08_with_gender_with_condition_no_alpha_beta(arr_count, arr_condition_count,
-                                                                                arr_position, arr_k, arr_gender,
-                                                                                arr_female_mortality, arr_male_mortality,
-                                                                                arr_age, arr_rand, condition):
-    rv = np.full(arr_age.shape, True, dtype=np.bool_)
-    counter = 0
-    for i in range(rv.shape[0]):
-        if condition[i]:
-            if arr_k[arr_position[i]] == 0.:
-                rv[i] = False
-                if arr_condition_count[i]:
-                    arr_count[arr_position[i]] -= 1
-                counter += 1
-                continue
-
-            mort_adjust = float(arr_count[arr_position[i]]) / float(arr_k[arr_position[i]])
-            age_agent = arr_age[i] // 52
-            if arr_gender[i] == 0:
-                p0 = 1 - np.exp(-arr_male_mortality[age_agent])
-            else:
-                p0 = 1 - np.exp(-arr_female_mortality[age_agent])
-            alpha = 4. * 1.5 / p0
-            if arr_rand[counter] <= (p0 / (1 + np.exp(-(mort_adjust - 1.5) * alpha))):
-                rv[i] = False
-                if arr_condition_count[i]:
-                    arr_count[arr_position[i]] -= 1
-            counter += 1
-    return rv
-
-
-@nb.njit
-def orm_like_agents_mortality_from_v08_with_condition_no_alpha_beta(arr_count, arr_condition_count, arr_position, arr_k,
-                                                                    arr_annual_mortality, arr_age, arr_rand,
-                                                                    condition):
-    rv = np.full(arr_age.shape, True, dtype=np.bool_)
-    for i in range(rv.shape[0]):
-        if condition[i]:
-            if arr_k[arr_position[i]] == 0.:
-                rv[i] = False
-                if arr_condition_count[i]:
-                    arr_count[arr_position[i]] -= 1
-                continue
-
-            mort_adjust = float(arr_count[arr_position[i]]) / float(arr_k[arr_position[i]])
-            age_agent = arr_age[i] // 52
-            p0 = 1 - np.exp(-arr_annual_mortality[age_agent])
-            alpha = 4. * 1.5 / p0
-            if arr_rand[i] <= (p0 / (1 + np.exp(-(mort_adjust - 1.5) * alpha))):
-                rv[i] = False
-                if arr_condition_count[i]:
-                    arr_count[arr_position[i]] -= 1
-    return rv
-
-
-@nb.njit
-def orm_mongooses_check_if_mother_free_of_juveniles(offsprings_mom_id, mother_id, potential_mother):
-    set_offsprings_mom_id = set(offsprings_mom_id)
-    for i in range(potential_mother.shape[0]):
-        if potential_mother[i]:
-            if mother_id[i] in set_offsprings_mom_id:
-                potential_mother[i] = False
-
-
-@nb.njit
-def orm_mongooses_update_ter_pos_youngs(mom_id, youngs, col_territory, col_position, col_id, col_mom_id):
-    set_mom_id = set(mom_id)
-    dict_mom_to_territory = dict()
-    for i in range(col_id.shape[0]):
-        if col_id[i] in set_mom_id:
-            dict_mom_to_territory[col_id[i]] = col_territory[i]
-    for i in range(youngs.shape[0]):
-        if youngs[i]:
-            col_territory[i] = dict_mom_to_territory[col_mom_id[i]]
-            col_position[i] = dict_mom_to_territory[col_mom_id[i]]
-
-
-@nb.njit
-def orm_mongooses_update_mating_week(current_week, mean_week, sd_week, arr_next_mating,
-                                     arr_init_to_perform, rand_gauss):
-    counter = 0
-    for i in range(arr_init_to_perform.shape[0]):
-        if arr_init_to_perform[i]:
-            potential_weeks = np.sort(np.rint(rand_gauss[counter] * sd_week + mean_week).astype('int32') % 52)
-            next_week_found = False
-            for j in range(potential_weeks.shape[0]):
-                if current_week < potential_weeks[j]:
-                    next_week_found = True
-                    arr_next_mating[i] = potential_weeks[j]
-                    break
-            if not next_week_found:
-                arr_next_mating[i] = potential_weeks[0]
-            counter += 1
-
-
-@nb.njit
-def experimental_density_mortality(arr_count, arr_position, arr_age, arr_k, arr_gender, beta_male, beta_female,
-                                   alpha, rand):
-    rv = np.full(arr_age.shape, True, dtype=np.bool_)
-    for i in range(rv.shape[0]):
-        if arr_k[arr_position[i]] == 0.:
-            rv[i] = False
-            arr_count[arr_position[i]] -= 1
-            continue
-
-        mort_adjust = float(arr_count[arr_position[i]]) / float(arr_k[arr_position[i]])
-        if arr_gender[i] == 0:
-            p = 1. / (1. + np.exp(-alpha * (mort_adjust - beta_male[arr_age[i]])))
-        else:
-            p = 1. / (1. + np.exp(-alpha * (mort_adjust - beta_female[arr_age[i]])))
-
-        if rand[i] <= p:
-            rv[i] = False
-            arr_count[arr_position[i]] -= 1
-    return rv
-
+import numpy as np
+import numba as nb
+
+
+@nb.njit
+def orm_like_agent_orm_dispersion(arr_can_move, arr_will_move, arr_rand_nb_steps, arr_rand_direction,
+                                  col_position, col_territory, col_has_moved, connections):
+    counter_arr_will_move = 0
+    counter_arr_rand_nb_steps = 0
+    counter_arr_rand_direction = 0
+    for i in range(arr_can_move.shape[0]):
+        if arr_can_move[i]:
+
+            # first we determine if the agent is allowed to move. If not, we skip to the next agent
+            will_move = arr_will_move[counter_arr_will_move]
+            counter_arr_will_move += 1
+            if not will_move:
+                continue
+
+            # now we update the 'has moved' flag (in ORM, this is done even if the agent moves 0 cells)
+            col_has_moved[i] = True
+
+            nb_steps = arr_rand_nb_steps[counter_arr_rand_nb_steps]
+            counter_arr_rand_nb_steps += 1
+            if nb_steps == 0:
+                continue
+
+            for j in range(nb_steps):
+                rand_direction = arr_rand_direction[counter_arr_rand_direction]
+                counter_arr_rand_direction += 1
+
+                if j == 0:
+                    direction = int(np.floor(rand_direction * 6)) % 6
+                else:
+                    if rand_direction <= 0.2:
+                        direction = (direction - 1) % 6
+                    elif rand_direction >= 0.8:
+                        direction = (direction + 1) % 6
+
+                if connections[col_territory[i]][direction] == -1:
+                    break
+
+                col_position[i] = connections[col_territory[i]][direction]
+                col_territory[i] = connections[col_territory[i]][direction]
+
+
+@nb.njit
+def orm_like_agent_dispersion_with_reflexion(arr_can_move, arr_will_move, arr_rand_nb_steps, arr_rand_direction,
+                                             col_position, col_territory, col_has_moved, connections, weights):
+    counter_arr_will_move = 0
+    counter_arr_rand_nb_steps = 0
+    counter_arr_rand_direction = 0
+    for i in range(arr_can_move.shape[0]):
+        if arr_can_move[i]:
+
+            # first we determine if the agent is allowed to move. If not, we skip to the next agent
+            will_move = arr_will_move[counter_arr_will_move]
+            counter_arr_will_move += 1
+            if not will_move:
+                continue
+
+            # now we update the 'has moved' flag (in ORM, this is done even if the agent moves 0 cells)
+            col_has_moved[i] = True
+
+            nb_steps = arr_rand_nb_steps[counter_arr_rand_nb_steps]
+            counter_arr_rand_nb_steps += 1
+            if nb_steps == 0:
+                continue
+
+            for j in range(nb_steps):
+                rand_direction = arr_rand_direction[counter_arr_rand_direction]
+                counter_arr_rand_direction += 1
+
+                if j == 0:
+                    direction = int(np.floor(rand_direction * 6)) % 6
+                else:
+                    if rand_direction <= 0.2:
+                        direction = (direction - 1) % 6
+                    elif rand_direction >= 0.8:
+                        direction = (direction + 1) % 6
+
+                if connections[col_territory[i]][direction] == -1:
+                    for k in range(6):
+                        if rand_direction <= weights[col_territory[i]][k]:
+                            col_position[i] = connections[col_territory[i]][k]
+                            col_territory[i] = connections[col_territory[i]][k]
+                            break
+                else:
+                    col_position[i] = connections[col_territory[i]][direction]
+                    col_territory[i] = connections[col_territory[i]][direction]
+
+
+@nb.njit
+def orm_like_agent_orm_dispersion_with_resistance(arr_can_move, arr_will_move, arr_rand_nb_steps, arr_rand_direction,
+                                                  col_position, col_territory, col_has_moved, connections,
+                                                  prob_successful_mov, rand_res):
+    counter_arr_will_move = 0
+    counter_arr_rand_nb_steps = 0
+    counter_arr_rand_direction = 0
+    counter_rand_res = -1
+    for i in range(arr_can_move.shape[0]):
+        if arr_can_move[i]:
+
+            # first we determine if the agent is allowed to move. If not, we skip to the next agent
+            will_move = arr_will_move[counter_arr_will_move]
+            counter_arr_will_move += 1
+            if not will_move:
+                continue
+            # now we update the 'has moved' flag (in ORM, this is done even if the agent moves 0 cells)
+            col_has_moved[i] = True
+
+            nb_steps = arr_rand_nb_steps[counter_arr_rand_nb_steps]
+            counter_arr_rand_nb_steps += 1
+            if nb_steps == 0:
+                continue
+
+            for j in range(nb_steps):
+
+                rand_direction = arr_rand_direction[counter_arr_rand_direction]
+                counter_arr_rand_direction += 1
+
+                if j == 0:
+                    direction = int(np.floor(rand_direction * 6)) % 6
+                else:
+                    if rand_direction <= 0.2:
+                        direction = (direction - 1) % 6
+                    elif rand_direction >= 0.8:
+                        direction = (direction + 1) % 6
+
+                if connections[col_territory[i]][direction] == -1:
+                    break
+
+                counter_rand_res += 1
+                if rand_res[counter_rand_res] >= prob_successful_mov[col_territory[i]][direction]:
+                    break
+
+                col_position[i] = connections[col_territory[i]][direction]
+                col_territory[i] = connections[col_territory[i]][direction]
+
+
+@nb.njit
+def orm_like_agents_mov_around_with_resistance(territory, position, connections, weights, prob_successful_mov,
+                                               arr_bool_mov, rand_direction, rand_res):
+    counter = 0
+    for i in range(territory.shape[0]):
+        if arr_bool_mov[i]:
+            for j in range(6):
+                if rand_direction[counter] <= weights[territory[i]][j]:
+                    if rand_res[counter] <= prob_successful_mov[territory[i]][j]:
+                        position[i] = connections[territory[i]][j]
+                    counter += 1
+                    break
+
+
+@nb.njit
+def orm_like_agents_mortality_from_v08_no_condition_no_alpha_beta(arr_count, arr_condition_count, arr_position, arr_k,
+                                                                  arr_annual_mortality, arr_age, arr_rand):
+    rv = np.full(arr_age.shape, True, dtype=np.bool_)
+    for i in range(rv.shape[0]):
+        if arr_k[arr_position[i]] == 0.:
+            rv[i] = False
+            if arr_condition_count[i]:
+                arr_count[arr_position[i]] -= 1
+            continue
+
+        mort_adjust = float(arr_count[arr_position[i]]) / float(arr_k[arr_position[i]])
+        age_agent = arr_age[i] // 52
+        p0 = 1 - np.exp(-arr_annual_mortality[age_agent])
+        alpha = 4. * 1.5 / p0
+        if arr_rand[i] <= (p0 / (1 + np.exp(-(mort_adjust - 1.5) * alpha))):
+            rv[i] = False
+            if arr_condition_count[i]:
+                arr_count[arr_position[i]] -= 1
+    return rv
+
+
+@nb.njit
+def orm_like_agents_mortality_from_v08_with_gender_no_condition_no_alpha_beta(arr_count, arr_condition_count,
+                                                                              arr_position, arr_k, arr_gender,
+                                                                              arr_female_mortality, arr_male_mortality,
+                                                                              arr_age, arr_rand):
+    rv = np.full(arr_age.shape, True, dtype=np.bool_)
+    for i in range(rv.shape[0]):
+        if arr_k[arr_position[i]] == 0.:
+            rv[i] = False
+            if arr_condition_count[i]:
+                arr_count[arr_position[i]] -= 1
+            continue
+
+        mort_adjust = float(arr_count[arr_position[i]]) / float(arr_k[arr_position[i]])
+        age_agent = arr_age[i] // 52
+        if arr_gender[i] == 0:
+            p0 = 1 - np.exp(-arr_male_mortality[age_agent])
+        else:
+            p0 = 1 - np.exp(-arr_female_mortality[age_agent])
+        alpha = 4. * 1.5 / p0
+        if arr_rand[i] <= (p0 / (1 + np.exp(-(mort_adjust - 1.5) * alpha))):
+            rv[i] = False
+            if arr_condition_count[i]:
+                arr_count[arr_position[i]] -= 1
+    return rv
+
+
+def orm_like_agents_mortality_from_v08_with_gender_with_condition_no_alpha_beta(arr_count, arr_condition_count,
+                                                                                arr_position, arr_k, arr_gender,
+                                                                                arr_female_mortality, arr_male_mortality,
+                                                                                arr_age, arr_rand, condition):
+    rv = np.full(arr_age.shape, True, dtype=np.bool_)
+    counter = 0
+    for i in range(rv.shape[0]):
+        if condition[i]:
+            if arr_k[arr_position[i]] == 0.:
+                rv[i] = False
+                if arr_condition_count[i]:
+                    arr_count[arr_position[i]] -= 1
+                counter += 1
+                continue
+
+            mort_adjust = float(arr_count[arr_position[i]]) / float(arr_k[arr_position[i]])
+            age_agent = arr_age[i] // 52
+            if arr_gender[i] == 0:
+                p0 = 1 - np.exp(-arr_male_mortality[age_agent])
+            else:
+                p0 = 1 - np.exp(-arr_female_mortality[age_agent])
+            alpha = 4. * 1.5 / p0
+            if arr_rand[counter] <= (p0 / (1 + np.exp(-(mort_adjust - 1.5) * alpha))):
+                rv[i] = False
+                if arr_condition_count[i]:
+                    arr_count[arr_position[i]] -= 1
+            counter += 1
+    return rv
+
+
+@nb.njit
+def orm_like_agents_mortality_from_v08_with_condition_no_alpha_beta(arr_count, arr_condition_count, arr_position, arr_k,
+                                                                    arr_annual_mortality, arr_age, arr_rand,
+                                                                    condition):
+    rv = np.full(arr_age.shape, True, dtype=np.bool_)
+    for i in range(rv.shape[0]):
+        if condition[i]:
+            if arr_k[arr_position[i]] == 0.:
+                rv[i] = False
+                if arr_condition_count[i]:
+                    arr_count[arr_position[i]] -= 1
+                continue
+
+            mort_adjust = float(arr_count[arr_position[i]]) / float(arr_k[arr_position[i]])
+            age_agent = arr_age[i] // 52
+            p0 = 1 - np.exp(-arr_annual_mortality[age_agent])
+            alpha = 4. * 1.5 / p0
+            if arr_rand[i] <= (p0 / (1 + np.exp(-(mort_adjust - 1.5) * alpha))):
+                rv[i] = False
+                if arr_condition_count[i]:
+                    arr_count[arr_position[i]] -= 1
+    return rv
+
+
+@nb.njit
+def orm_mongooses_check_if_mother_free_of_juveniles(offsprings_mom_id, mother_id, potential_mother):
+    set_offsprings_mom_id = set(offsprings_mom_id)
+    for i in range(potential_mother.shape[0]):
+        if potential_mother[i]:
+            if mother_id[i] in set_offsprings_mom_id:
+                potential_mother[i] = False
+
+
+@nb.njit
+def orm_mongooses_update_ter_pos_youngs(mom_id, youngs, col_territory, col_position, col_id, col_mom_id):
+    set_mom_id = set(mom_id)
+    dict_mom_to_territory = dict()
+    for i in range(col_id.shape[0]):
+        if col_id[i] in set_mom_id:
+            dict_mom_to_territory[col_id[i]] = col_territory[i]
+    for i in range(youngs.shape[0]):
+        if youngs[i]:
+            col_territory[i] = dict_mom_to_territory[col_mom_id[i]]
+            col_position[i] = dict_mom_to_territory[col_mom_id[i]]
+
+
+@nb.njit
+def orm_mongooses_update_mating_week(current_week, mean_week, sd_week, arr_next_mating,
+                                     arr_init_to_perform, rand_gauss):
+    counter = 0
+    for i in range(arr_init_to_perform.shape[0]):
+        if arr_init_to_perform[i]:
+            potential_weeks = np.sort(np.rint(rand_gauss[counter] * sd_week + mean_week).astype('int32') % 52)
+            next_week_found = False
+            for j in range(potential_weeks.shape[0]):
+                if current_week < potential_weeks[j]:
+                    next_week_found = True
+                    arr_next_mating[i] = potential_weeks[j]
+                    break
+            if not next_week_found:
+                arr_next_mating[i] = potential_weeks[0]
+            counter += 1
+
+
+@nb.njit
+def experimental_density_mortality(arr_count, arr_position, arr_age, arr_k, arr_gender, beta_male, beta_female,
+                                   alpha, rand):
+    rv = np.full(arr_age.shape, True, dtype=np.bool_)
+    for i in range(rv.shape[0]):
+        if arr_k[arr_position[i]] == 0.:
+            rv[i] = False
+            arr_count[arr_position[i]] -= 1
+            continue
+
+        mort_adjust = float(arr_count[arr_position[i]]) / float(arr_k[arr_position[i]])
+        if arr_gender[i] == 0:
+            p = 1. / (1. + np.exp(-alpha * (mort_adjust - beta_male[arr_age[i]])))
+        else:
+            p = 1. / (1. + np.exp(-alpha * (mort_adjust - beta_female[arr_age[i]])))
+
+        if rand[i] <= p:
+            rv[i] = False
+            arr_count[arr_position[i]] -= 1
+    return rv
+
```

### Comparing `sampy-abm-1.0.2/src/sampy/agent/base.py` & `sampy_abm-1.0.3/src/sampy/agent/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,245 +1,284 @@
-import pandas as pd
-import numpy as np
-from .jit_compiled_functions import (count_nb_agent_per_vertex,
-                                     conditional_count_nb_agent_per_vertex)
-from ..pandas_xs.pandas_xs import DataFrameXS
-
-
-class BaseAgingAgent:
-    """
-    Base class for aging agents, i.e. agents having an age attribute that is used in the simulation (for instance for
-    varying probabilities of dispersion or varying mortality rates).
-    """
-    def __init__(self, **kwargs):
-        try:
-            self.graph = kwargs['graph']
-        except KeyError:
-            raise ValueError("A graph object should be passed to the constructor, using the kwarg 'graph'.")
-
-        if not hasattr(self, 'df_population'):
-            self.df_population = DataFrameXS()
-
-        self.df_population['col_id'] = None
-        self.df_population['age'] = None
-
-        if hasattr(self, 'dict_default_val'):
-            self.dict_default_val['age'] = 0
-        else:
-            self.dict_default_val = {'age': 0}
-
-        self.counter_id = 0
-
-        self.on_ticker = ['increase_age']
-        self.type = 'agent'
-
-    def _sampy_debug_add_attribute(self, name_attr, def_value=np.nan):
-        if not isinstance(name_attr, str):
-            raise ValueError("An attribute name should be a string.")
-        if name_attr in self.df_population.dict_colname_to_index:
-            raise KeyError("An attribute with the name " + name_attr + " already exists.")
-        x = np.array([def_value])
-        if x.shape != (1,):
-            raise ValueError("A default value should be a single number, integer or np.nan.")
-        if str(x.dtype) not in self.df_population.ALLOWED_TYPE:
-            raise ValueError("The chosen default value results in arrays of dtype '" + str(x.dtype) + "', which is not"
-                             " supported by DataFrameXS object. Supported types are:" +
-                             str(self.df_population.LIST_ALLOWED_TYPE) + ".")
-
-    def add_attribute(self, name_attr, def_value=np.nan):
-        """
-        add a new column to the dataframe df_population, whose name is the parameter 'name_attr'
-
-        :param name_attr: name of the new column
-        :param def_value: default value for the created column, set the whole column to this value if df_population is
-            non empty, and save the default value for later calls.
-        """
-        self.df_population[name_attr] = def_value
-        self.dict_default_val[name_attr] = def_value
-
-    def _sampy_debug_set_default_val(self, dict_values, replace=False):
-        if not hasattr(dict_values, 'items') or not hasattr(getattr(dict_values, 'items'), '__call__'):
-            raise TypeError("Dict_value parameter should be a dictionary like object, with a method 'items' "
-                             "allowing to loop over keys and values of the object.")
-        for key, val in dict_values.items():
-            if not isinstance(key, str):
-                raise KeyError("Column names should be a string.")
-            if key not in self.df_population.dict_colname_to_index:
-                raise KeyError("Trying to set the default value of a non existing column (" + key + ")")
-            x = np.array([val])
-            if x.shape != (1,):
-                raise ValueError("A default value should be a single number, integer or np.nan.")
-            if str(x.dtype) not in self.df_population.ALLOWED_TYPE:
-                raise ValueError(
-                    "The chosen default value results in arrays of dtype '" + str(x.dtype) + "', which is not" +
-                    " supported by DataFrameXS object. Supported types are:" +
-                    str(self.df_population.LIST_ALLOWED_TYPE) + ".")
-
-    def set_default_val(self, dict_values, replace=False):
-        """
-        Change the defaults values in the attribute dict_default_val. If replace is True, then the attr dict_default_val
-        is replaced by the content of the argument dict_values. Otherwise, the content of dict_values is added to
-        dict_values, modifying it if needed.
-
-        :param dict_values: dictionary like object, with an items method
-        :param replace: optional, boolean, default False
-        """
-        if replace:
-            self.dict_default_val = {}
-        for name, val in dict_values.items():
-            self.dict_default_val[name] = val
-
-    def _sampy_debug_add_agents(self, dict_values):
-        if not hasattr(dict_values, 'items') or not hasattr(getattr(dict_values, 'items'), '__call__'):
-            raise TypeError("Dict_value parameter should be a dictionary like object, with a method 'items' "
-                             "allowing to loop over keys and values of the object.")
-        nb_rows_added = 0
-        found_non_cst_col = False
-        name_first_non_cst_column = None
-        for key, val in dict_values.items():
-            if not isinstance(key, str):
-                raise KeyError("Column names should be a string.")
-            if key not in self.df_population.dict_colname_to_index:
-                raise KeyError("The agents have an that is not a column of the population DataFrame (" + key + ").")
-            x = np.array(val)
-            if len(x.shape) > 1:
-                raise ValueError("The value for column " + key + " results in an array of dimension " +
-                                 str(x.shape) + " while add_agents expects one dimensional arrays or constants.")
-            if len(x.shape) == 1:
-                if found_non_cst_col:
-                    if x.shape[0] != nb_rows_added:
-                        raise ValueError("The value for column " + key + " results in creating " + str(x.shape[0]) +
-                                         " lines, while column " + name_first_non_cst_column + " value results in " +
-                                         "creating " + str(nb_rows_added) + '.')
-                else:
-                    nb_rows_added = x.shape[0]
-                    found_non_cst_col = True
-                    name_first_non_cst_column = key
-
-    def add_agents(self, dict_values):
-        """
-        add new rows to the dataframe df_population, which corresponds to new individuals. The recommanded use for this
-        method is to provide a dict_value of the form:
-
-            dict_value = {name_col1: list_of_values1, name_col2: list_of_values2, ...}
-
-        list of values can be replaced by np.array. Note that some of those lists can be replaced by constants if you
-        want some columns to be filled with a single value. If the user provides constant for all list_of_values, then a
-        single line is added. Finally, any non mentioned column will be filled with the associated default value.
-
-        Note that the user does not have the hand on the col_id column since it is considered internal, and the user
-        should add an extra column to identify some individuals.
-
-        :param dict_values: values of the attributes of the new individuals.
-        """
-
-        constant_cols = {}
-        array_cols = {}
-        for name, col in dict_values.items():
-            if col is None:
-                array_cols[name] = col
-            else:
-                arr_col = np.array(col)
-                if len(arr_col.shape) == 0:
-                    constant_cols[name] = col
-                else:
-                    array_cols[name] = arr_col
-
-        # create a DataFrameXS from the input values
-        df = DataFrameXS()
-
-        # populate the dataframe df. First considering the case where some lists have been provided.
-        if array_cols:
-            for name, col in array_cols.items():
-                df[name] = col
-            # then add the constant columns
-            for name, const in constant_cols.items():
-                df[name] = const
-
-        # now the case where only single values have been provided
-        else:
-            for name, const in dict_values.items():
-                if const is None or (len(np.array(const).shape) > 0 and np.array(const).shape[0] == 0) :
-                    df[name] = None
-                else:
-                    df[name] = [const]
-
-        # add the default values if needed.
-        for name, value in self.dict_default_val.items():
-            if name not in df.dict_colname_to_index:
-                df[name] = value
-
-        # create the col_id column
-        df['col_id'] = [self.counter_id + i for i in range(df.nb_rows)]
-        self.counter_id = df['col_id'][-1] + 1
-
-        # concatenate df to df_population
-        self.df_population.concat(df, inplace=True)
-
-    def increase_age(self):
-        """
-        increment by one the age of all the agents
-        """
-        self.df_population['age'] += 1
-
-    def tick(self):
-        """
-        execute in order all the methods whose name are in the list 'on_ticker'. Those methods should not accept
-        any arguments.
-        """
-        for method in self.on_ticker:
-            getattr(self, method)()
-
-    def save_population_to_csv(self, path, sep=';', **kwargs):
-        """
-        Save the dataframe df_population as csv
-
-        :param path: full path of the csv file
-        :param sep: optional. Separator used in csv. Default is ';'
-        """
-        self.df_population.to_csv(path, sep=sep, **kwargs)
-
-    def load_population_from_csv(self, path, sep=';', **kwargs):
-        """
-        load a csv film to create the dataframe. Override the existing dataframe df_population, if any.
-
-        :param path: full path of the csv file
-        :param sep: optional. Separator used in csv. Default is ';'
-        """
-        self.df_population = DataFrameXS.read_csv(path, sep=sep, **kwargs)
-
-    def _sampy_debug_count_pop_per_vertex(self, position_attribute='position', condition=None):
-        if condition is not None:
-            if (not isinstance(condition, np.ndarray)) or \
-                    (condition.shape != (self.df_population.nb_rows,)) or \
-                    (not str(condition.dtype).startswith('bool')):
-                raise ValueError("if used, condition argument should be a 1D array of bool of same length as the number"
-                                 " of individuals.")
-
-    def count_pop_per_vertex(self, position_attribute='position', condition=None):
-        """
-        Count the number of agent in each cell, and return the result as a 1D numpy array.
-
-        :param position_attribute: Optional, string, default 'position'. Name of the attribute corresponding to cell
-                                   index on which agent is.
-        :param condition: Optional, 1D array of bool, default None. If not None, count only the agent for which the
-                          condition is True.
-
-        :return: 1D array X such that X[i] is the number of agent in the cell whose index is i.
-        """
-        if condition is None:
-            return count_nb_agent_per_vertex(self.df_population[position_attribute],
-                                             self.graph.weights.shape[0])
-        else:
-            if (not isinstance(condition, np.ndarray)) or \
-               (len(condition.shape) != 1) or \
-               (condition.shape[0] != self.df_population.nb_rows) or \
-               (not str(condition.dtype).startswith('bool')):
-                raise ValueError("if used, condition argument should be a 1D array of bool of same length as the number"
-                                 " of individuals.")
-            return conditional_count_nb_agent_per_vertex(condition,
-                                                         self.df_population[position_attribute],
-                                                         self.graph.weights.shape[0])
-
-    @property
-    def number_agents(self):
-        return self.df_population.nb_rows
+import pandas as pd
+import numpy as np
+from .jit_compiled_functions import (count_nb_agent_per_vertex,
+                                     conditional_count_nb_agent_per_vertex)
+from ..pandas_xs.pandas_xs import DataFrameXS
+
+
+class BaseAgingAgent:
+    """
+    Base class for aging agents, i.e. agents having an age attribute that is used in the simulation (for instance for
+    varying probabilities of dispersion or varying mortality rates).
+    """
+    def __init__(self, **kwargs):
+        try:
+            self.graph = kwargs['graph']
+        except KeyError:
+            raise ValueError("A graph object should be passed to the constructor, using the kwarg 'graph'.")
+
+        if not hasattr(self, 'df_population'):
+            self.df_population = DataFrameXS()
+
+        self.df_population['col_id'] = None
+        self.df_population['age'] = None
+
+        if hasattr(self, 'dict_default_val'):
+            self.dict_default_val['age'] = 0
+        else:
+            self.dict_default_val = {'age': 0}
+
+        self.counter_id = 0
+
+        self.on_ticker = ['increase_age']
+        self.type = 'agent'
+
+    def _sampy_debug_add_attribute(self, name_attr, def_value=np.nan):
+        if not isinstance(name_attr, str):
+            raise ValueError("An attribute name should be a string.")
+        if name_attr in self.df_population.dict_colname_to_index:
+            raise KeyError("An attribute with the name " + name_attr + " already exists.")
+        x = np.array([def_value])
+        if x.shape != (1,):
+            raise ValueError("A default value should be a single number, integer or np.nan.")
+        if str(x.dtype) not in self.df_population.ALLOWED_TYPE:
+            raise ValueError("The chosen default value results in arrays of dtype '" + str(x.dtype) + "', which is not"
+                             " supported by DataFrameXS object. Supported types are:" +
+                             str(self.df_population.LIST_ALLOWED_TYPE) + ".")
+
+    def add_attribute(self, name_attr, def_value=np.nan):
+        """
+        add a new column to the dataframe df_population, whose name is the parameter 'name_attr'
+
+        :param name_attr: name of the new column
+        :param def_value: default value for the created column, set the whole column to this value if df_population is
+            non empty, and save the default value for later calls.
+        """
+        self.df_population[name_attr] = def_value
+        self.dict_default_val[name_attr] = def_value
+
+    def _sampy_debug_set_default_val(self, dict_values, replace=False):
+        if not hasattr(dict_values, 'items') or not hasattr(getattr(dict_values, 'items'), '__call__'):
+            raise TypeError("Dict_value parameter should be a dictionary like object, with a method 'items' "
+                             "allowing to loop over keys and values of the object.")
+        for key, val in dict_values.items():
+            if not isinstance(key, str):
+                raise KeyError("Column names should be a string.")
+            if key not in self.df_population.dict_colname_to_index:
+                raise KeyError("Trying to set the default value of a non existing column (" + key + ")")
+            x = np.array([val])
+            if x.shape != (1,):
+                raise ValueError("A default value should be a single number, integer or np.nan.")
+            if str(x.dtype) not in self.df_population.ALLOWED_TYPE:
+                raise ValueError(
+                    "The chosen default value results in arrays of dtype '" + str(x.dtype) + "', which is not" +
+                    " supported by DataFrameXS object. Supported types are:" +
+                    str(self.df_population.LIST_ALLOWED_TYPE) + ".")
+
+    def set_default_val(self, dict_values, replace=False):
+        """
+        Change the defaults values in the attribute dict_default_val. If replace is True, then the attr dict_default_val
+        is replaced by the content of the argument dict_values. Otherwise, the content of dict_values is added to
+        dict_values, modifying it if needed.
+
+        :param dict_values: dictionary like object, with an items method
+        :param replace: optional, boolean, default False
+        """
+        if replace:
+            self.dict_default_val = {}
+        for name, val in dict_values.items():
+            self.dict_default_val[name] = val
+
+    def _sampy_debug_add_agents(self, dict_values):
+        if not hasattr(dict_values, 'items') or not hasattr(getattr(dict_values, 'items'), '__call__'):
+            raise TypeError("Dict_value parameter should be a dictionary like object, with a method 'items' "
+                             "allowing to loop over keys and values of the object.")
+        nb_rows_added = 0
+        found_non_cst_col = False
+        name_first_non_cst_column = None
+        for key, val in dict_values.items():
+            if not isinstance(key, str):
+                raise KeyError("Column names should be a string.")
+            if key not in self.df_population.dict_colname_to_index:
+                raise KeyError("The agents have an attribute that is not a column of the population DataFrame (" + key + ").")
+            x = np.array(val)
+            if len(x.shape) > 1:
+                raise ValueError("The value for column " + key + " results in an array of dimension " +
+                                 str(x.shape) + " while add_agents expects one dimensional arrays or constants.")
+            if len(x.shape) == 1:
+                if found_non_cst_col:
+                    if x.shape[0] != nb_rows_added:
+                        raise ValueError("The value for column " + key + " results in creating " + str(x.shape[0]) +
+                                         " lines, while column " + name_first_non_cst_column + " value results in " +
+                                         "creating " + str(nb_rows_added) + '.')
+                else:
+                    nb_rows_added = x.shape[0]
+                    found_non_cst_col = True
+                    name_first_non_cst_column = key
+
+    def add_agents(self, dict_values):
+        """
+        add new rows to the dataframe df_population, which corresponds to new individuals. The recommanded use for this
+        method is to provide a dict_value of the form:
+
+            dict_value = {name_col1: list_of_values1, name_col2: list_of_values2, ...}
+
+        list of values can be replaced by np.array. Note that some of those lists can be replaced by constants if you
+        want some columns to be filled with a single value. If the user provides constant for all list_of_values, then a
+        single line is added. Finally, any non mentioned column will be filled with the associated default value.
+
+        Note that the user does not have the hand on the col_id column since it is considered internal, and you
+        should add an extra column if you want to identify individuals using your own conventions.
+
+        :param dict_values: values of the attributes of the new individuals.
+        """
+
+        constant_cols = {}
+        array_cols = {}
+        for name, col in dict_values.items():
+            if col is None:
+                array_cols[name] = col
+            else:
+                arr_col = np.array(col)
+                if len(arr_col.shape) == 0:
+                    constant_cols[name] = col
+                else:
+                    array_cols[name] = arr_col
+
+        # create a DataFrameXS from the input values
+        df = DataFrameXS()
+
+        # populate the dataframe df. First considering the case where some lists have been provided.
+        if array_cols:
+            for name, col in array_cols.items():
+                df[name] = col
+            # then add the constant columns
+            for name, const in constant_cols.items():
+                df[name] = const
+
+        # now the case where only single values have been provided
+        else:
+            for name, const in dict_values.items():
+                if const is None or (len(np.array(const).shape) > 0 and np.array(const).shape[0] == 0) :
+                    df[name] = None
+                else:
+                    df[name] = [const]
+
+        # add the default values if needed.
+        for name, value in self.dict_default_val.items():
+            if name not in df.dict_colname_to_index:
+                df[name] = value
+
+        # create the col_id column
+        df['col_id'] = [self.counter_id + i for i in range(df.nb_rows)]
+        self.counter_id = df['col_id'][-1] + 1
+
+        # concatenate df to df_population
+        self.df_population.concat(df, inplace=True)
+
+    def _sampy_debug_add_agents_from_dataframe(self, dataframe):
+        if not isinstance(dataframe, DataFrameXS):
+            raise ValueError("The dataframe should be a DataFrameXS object.")
+
+    def add_agents_from_dataframe(self, dataframe: DataFrameXS):
+        """
+        add new rows to the dataframe df_population, which corresponds to new individuals.
+        Those agents are given in the form of a DataFrameXS object where each row corresponds
+        to a new agent. 
+
+        WARNING: this method will modify the input DataFrame. For instance, if the input
+                 DataFrame contains a column col_id, it will be dropped and replaced by
+                 a new one with values consistant with the current ids. It is planned
+                 to add an option to allow this method to work with a copy of the input
+                 dataframe instead.
+
+        :param dataframe: A DataFrameXS object.
+        """
+        if dataframe.is_empty:
+            return
+        
+        # first, if the input DataFrame contains a column named "col_id", it should be dropped.
+        if 'col_id' in dataframe.dict_colname_to_index:
+            dataframe.drop_column('col_id')
+
+        # we now create a compatible id column for the new agents
+        dataframe['col_id'] = [self.counter_id + i for i in range(dataframe.nb_rows)]
+        self.counter_id = dataframe['col_id'][-1] + 1 # save new value for next agents
+
+        # we now check that the method has everything required to fill in the "potentially missing" values
+        for name in self.df_population.list_col_name:
+            if name not in self.dict_default_val:
+                if (name in dataframe.dict_colname_to_index) and (dataframe[name] is None):
+                    raise ValueError("The dataframe describing the new agents has an empty column named " + name + ", and there is no associated default value associated with this column.")
+                if (name not in dataframe.dict_colname_to_index):
+                    raise ValueError("The dataframe describing the new agents does not have a column named " + name + ", and there is no associated default value associated with this column.")
+        
+        self.df_population.concat(dataframe, inplace=True, dict_default_values=self.dict_default_val)
+
+    def increase_age(self):
+        """
+        increment by one the age of all the agents
+        """
+        self.df_population['age'] += 1
+
+    def tick(self):
+        """
+        execute in order all the methods whose name are in the list 'on_ticker'. Those methods should not accept
+        any arguments.
+        """
+        for method in self.on_ticker:
+            getattr(self, method)()
+
+    def save_population_to_csv(self, path, sep=';', **kwargs):
+        """
+        Save the dataframe df_population as csv
+
+        :param path: full path of the csv file
+        :param sep: optional. Separator used in csv. Default is ';'
+        """
+        self.df_population.to_csv(path, sep=sep, **kwargs)
+
+    def load_population_from_csv(self, path, sep=';', **kwargs):
+        """
+        load a csv film to create the dataframe. Override the existing dataframe df_population, if any.
+
+        :param path: full path of the csv file
+        :param sep: optional. Separator used in csv. Default is ';'
+        """
+        self.df_population = DataFrameXS.read_csv(path, sep=sep, **kwargs)
+
+    def _sampy_debug_count_pop_per_vertex(self, position_attribute='position', condition=None):
+        if condition is not None:
+            if (not isinstance(condition, np.ndarray)) or \
+                    (condition.shape != (self.df_population.nb_rows,)) or \
+                    (not str(condition.dtype).startswith('bool')):
+                raise ValueError("if used, condition argument should be a 1D array of bool of same length as the number"
+                                 " of individuals.")
+
+    def count_pop_per_vertex(self, position_attribute='position', condition=None):
+        """
+        Count the number of agent in each cell, and return the result as a 1D numpy array.
+
+        :param position_attribute: Optional, string, default 'position'. Name of the attribute corresponding to cell
+                                   index on which agent is.
+        :param condition: Optional, 1D array of bool, default None. If not None, count only the agent for which the
+                          condition is True.
+
+        :return: 1D array X such that X[i] is the number of agent in the cell whose index is i.
+        """
+        if condition is None:
+            return count_nb_agent_per_vertex(self.df_population[position_attribute],
+                                             self.graph.weights.shape[0])
+        else:
+            if (not isinstance(condition, np.ndarray)) or \
+               (len(condition.shape) != 1) or \
+               (condition.shape[0] != self.df_population.nb_rows) or \
+               (not str(condition.dtype).startswith('bool')):
+                raise ValueError("if used, condition argument should be a 1D array of bool of same length as the number"
+                                 " of individuals.")
+            return conditional_count_nb_agent_per_vertex(condition,
+                                                         self.df_population[position_attribute],
+                                                         self.graph.weights.shape[0])
+
+    @property
+    def number_agents(self):
+        return self.df_population.nb_rows
```

### Comparing `sampy-abm-1.0.2/src/sampy/agent/jit_compiled_functions.py` & `sampy_abm-1.0.3/src/sampy/agent/jit_compiled_functions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,577 +1,730 @@
-import numba as nb
-import numpy as np
-from numba.typed import List
-
-
-# ---------------------------------------------------------------------------------------------------------------------
-# base section
-
-
-@nb.njit
-def count_nb_agent_per_vertex(arr_pos, nb_vertex):
-    rv = np.zeros((nb_vertex,), dtype=np.int32)
-    for i in range(arr_pos.shape[0]):
-        rv[arr_pos[i]] += 1
-    return rv
-
-
-@nb.njit
-def conditional_count_nb_agent_per_vertex(arr_condition, arr_pos, nb_vertex):
-    rv = np.zeros((nb_vertex,), dtype=np.int32)
-    for i in range(arr_pos.shape[0]):
-        if arr_condition[i]:
-            rv[arr_pos[i]] += 1
-    return rv
-
-# ---------------------------------------------------------------------------------------------------------------------
-# mortality section
-
-
-@nb.njit
-def mortality_natural_death_orm_methodology(bias, rand, arr_prob_male, arr_prob_female, arr_count, pos, k, age, gender):
-    rv = np.full(rand.shape, True, dtype=np.bool_)
-    for i in range(rv.shape[0]):
-        if k[pos[i]] == 0:
-            p = 1.
-        else:
-            if gender[i] == 0:
-                p = arr_prob_male[age[i]] * ((float(arr_count[pos[i]]) / float(k[pos[i]])) + bias)
-            else:
-                p = arr_prob_female[age[i]] * ((float(arr_count[pos[i]]) / float(k[pos[i]])) + bias)
-        if rand[i] <= p:
-            rv[i] = False
-            arr_count[pos[i]] -= 1
-    return rv
-
-
-@nb.njit
-def mortality_natural_death_orm_methodology_condition_count(bias, rand, arr_prob_male, arr_prob_female,
-                                                            arr_count, arr_cond_count, pos, k, age, gender):
-    rv = np.full(rand.shape, True, dtype=np.bool_)
-    for i in range(rv.shape[0]):
-        if k[pos[i]] == 0:
-            p = 1.
-        else:
-            if gender[i] == 0:
-                p = arr_prob_male[age[i]] * ((float(arr_count[pos[i]]) / float(k[pos[i]])) + bias)
-            else:
-                p = arr_prob_female[age[i]] * ((float(arr_count[pos[i]]) / float(k[pos[i]])) + bias)
-        if rand[i] <= p:
-            rv[i] = False
-            if arr_cond_count[i]:
-                arr_count[pos[i]] -= 1
-    return rv
-
-
-@nb.njit
-def mortality_natural_death_orm_methodology_condition_death(bias, rand, arr_prob_male, arr_prob_female,
-                                                            arr_count, arr_cond_death, pos, k, age, gender):
-    rv = np.full(rand.shape, True, dtype=np.bool_)
-    for i in range(rv.shape[0]):
-        if arr_cond_death[i]:
-            if k[pos[i]] == 0:
-                p = 1.
-            else:
-                if gender[i] == 0:
-                    p = arr_prob_male[age[i]] * ((float(arr_count[pos[i]]) / float(k[pos[i]])) + bias)
-                else:
-                    p = arr_prob_female[age[i]] * ((float(arr_count[pos[i]]) / float(k[pos[i]])) + bias)
-            if rand[i] <= p:
-                rv[i] = False
-                arr_count[pos[i]] -= 1
-    return rv
-
-
-@nb.njit
-def mortality_natural_death_orm_methodology_both_cond(bias, rand, arr_prob_male, arr_prob_female,
-                                                      arr_count, arr_cond_death, arr_cond_count, pos, k, age, gender):
-    rv = np.full(rand.shape, True, dtype=np.bool_)
-    for i in range(rv.shape[0]):
-        if arr_cond_death[i]:
-            if k[pos[i]] == 0:
-                p = 1.
-            else:
-                if gender[i] == 0:
-                    p = arr_prob_male[age[i]] * ((float(arr_count[pos[i]]) / float(k[pos[i]])) + bias)
-                else:
-                    p = arr_prob_female[age[i]] * ((float(arr_count[pos[i]]) / float(k[pos[i]])) + bias)
-            if rand[i] <= p:
-                rv[i] = False
-                if arr_cond_count[i]:
-                    arr_count[pos[i]] -= 1
-    return rv
-
-# ---------------------------------------------------------------------------------------------------------------------
-# reproduction
-
-
-@nb.njit
-def reproduction_find_random_mate_on_position(col_mate, col_pregnancy, arr_id, position, gender, nb_vertex,
-                                              rand_preg, prob_pregnancy):
-    list_vert_id_male = List()
-    list_vert_index_male = List()
-    for i in range(nb_vertex):
-        male_on_pos_i = List()
-        male_on_pos_i.append(arr_id[0])
-        male_on_pos_i.pop()
-        list_vert_id_male.append(male_on_pos_i)
-
-        index_male_on_pos_i = List()
-        index_male_on_pos_i.append(0)
-        index_male_on_pos_i.pop()
-        list_vert_index_male.append(index_male_on_pos_i)
-
-    arr_nb_male_per_vertex = np.full((nb_vertex,), 0, dtype=np.int32)
-    for i in range(arr_id.shape[0]):
-        col_mate[i] = -1
-        col_pregnancy[i] = False
-        if gender[i] == 0:
-            arr_nb_male_per_vertex[position[i]] += 1
-            list_vert_id_male[position[i]].append(arr_id[i])
-            list_vert_index_male[position[i]].append(i)
-
-    arr_ind_vertex = np.full((nb_vertex,), 0, dtype=np.int32)
-    counter = 0
-    for i in range(arr_id.shape[0]):
-        if gender[i] == 1:
-            if arr_ind_vertex[position[i]] < arr_nb_male_per_vertex[position[i]]:
-                col_mate[i] = list_vert_id_male[position[i]][arr_ind_vertex[position[i]]]
-                col_mate[list_vert_index_male[position[i]][arr_ind_vertex[position[i]]]] = arr_id[i]
-                arr_ind_vertex[position[i]] += 1
-                if rand_preg[counter] <= prob_pregnancy:
-                    col_pregnancy[i] = True
-            counter += 1
-
-
-@nb.njit
-def reproduction_find_random_mate_on_position_condition(col_mate, col_pregnancy, arr_id, position, gender, nb_vertex,
-                                                        rand_preg, prob_pregnancy, condition):
-    list_vert_id_male = List()
-    list_vert_index_male = List()
-    for i in range(nb_vertex):
-        male_on_pos_i = List()
-        male_on_pos_i.append(arr_id[0])
-        male_on_pos_i.pop()
-        list_vert_id_male.append(male_on_pos_i)
-
-        index_male_on_pos_i = List()
-        index_male_on_pos_i.append(0)
-        index_male_on_pos_i.pop()
-        list_vert_index_male.append(index_male_on_pos_i)
-
-    arr_nb_male_per_vertex = np.full((nb_vertex,), 0, dtype=np.int32)
-    for i in range(arr_id.shape[0]):
-        if condition[i]:
-            col_mate[i] = -1
-            col_pregnancy[i] = False
-            if gender[i] == 0:
-                arr_nb_male_per_vertex[position[i]] += 1
-                list_vert_id_male[position[i]].append(arr_id[i])
-                list_vert_index_male[position[i]].append(i)
-
-    arr_ind_vertex = np.full((nb_vertex,), 0, dtype=np.int32)
-    counter = 0
-    for i in range(arr_id.shape[0]):
-        if gender[i] == 1 and condition[i]:
-            if arr_ind_vertex[position[i]] < arr_nb_male_per_vertex[position[i]]:
-                col_mate[i] = list_vert_id_male[position[i]][arr_ind_vertex[position[i]]]
-                col_mate[list_vert_index_male[position[i]][arr_ind_vertex[position[i]]]] = arr_id[i]
-                arr_ind_vertex[position[i]] += 1
-                if rand_preg[counter] <= prob_pregnancy:
-                    col_pregnancy[i] = True
-            counter += 1
-
-
-@nb.njit
-def reproduction_find_random_mate_on_position_polygamous(arr_id, position, gender, col_mate, col_pregnant,
-                                                         nb_vertex, rand_preg, rand_chose_mate, prob_pregnancy):
-    list_vert_id_male = List()
-    for i in range(nb_vertex):
-        male_on_pos_i = List()
-        male_on_pos_i.append(arr_id[0])
-        male_on_pos_i.pop()
-        list_vert_id_male.append(male_on_pos_i)
-
-    arr_nb_male_per_vertex = np.full((nb_vertex,), 0, dtype=np.int32)
-    for i in range(arr_id.shape[0]):
-        col_pregnant[i] = False
-        col_mate[i] = -1
-        if gender[i] == 0:
-            arr_nb_male_per_vertex[position[i]] += 1
-            list_vert_id_male[position[i]].append(arr_id[i])
-
-    counter = 0
-    for i in range(arr_id.shape[0]):
-        if gender[i] == 1:
-            if arr_nb_male_per_vertex[position[i]] > 0:
-                rand_index_male = int(np.floor(rand_chose_mate[counter] * arr_nb_male_per_vertex[position[i]])) % \
-                                  arr_nb_male_per_vertex[position[i]]
-                col_mate[i] = list_vert_id_male[position[i]][rand_index_male]
-                if rand_preg[counter] <= prob_pregnancy:
-                    col_pregnant[i] = True
-            counter += 1
-
-
-@nb.njit
-def reproduction_find_random_mate_on_position_polygamous_condition(arr_id, position, gender, col_mate, col_pregnant,
-                                                                   nb_vertex, rand_preg, rand_chose_mate,
-                                                                   prob_pregnancy, condition):
-    list_vert_id_male = List()
-    for i in range(nb_vertex):
-        male_on_pos_i = List()
-        male_on_pos_i.append(arr_id[0])
-        male_on_pos_i.pop()
-        list_vert_id_male.append(male_on_pos_i)
-
-    arr_nb_male_per_vertex = np.full((nb_vertex,), 0, dtype=np.int32)
-    for i in range(arr_id.shape[0]):
-        if condition[i]:
-            col_pregnant[i] = False
-            col_mate[i] = -1
-            if gender[i] == 0:
-                arr_nb_male_per_vertex[position[i]] += 1
-                list_vert_id_male[position[i]].append(arr_id[i])
-
-    counter = 0
-    for i in range(arr_id.shape[0]):
-        if gender[i] == 1 and condition[i]:
-            if arr_nb_male_per_vertex[position[i]] > 0:
-                rand_index_male = int(np.floor(rand_chose_mate[counter] * arr_nb_male_per_vertex[position[i]])) % \
-                                  arr_nb_male_per_vertex[position[i]]
-                col_mate[i] = list_vert_id_male[position[i]][rand_index_male]
-                if rand_preg[counter] <= prob_pregnancy:
-                    col_pregnant[i] = True
-            counter += 1
-
-# ---------------------------------------------------------------------------------------------------------------------
-# graph based movement section
-
-
-@nb.njit
-def movement_change_territory_and_position_condition(territory, position, condition, rand, connections, weights):
-    counter_rand = 0
-    for i in range(territory.shape[0]):
-        if condition[i]:
-            found = False
-            for j in range(weights.shape[1]):
-                if rand[counter_rand] <= weights[territory[i]][j]:
-                    found = True
-                    # very important to update position first
-                    position[i] = connections[territory[i]][j]
-                    territory[i] = connections[territory[i]][j]
-                    break
-            if not found:
-                position[i] = territory[i]
-            counter_rand += 1
-
-
-@nb.njit
-def movement_change_territory_and_position(territory, position, rand, connections, weights):
-    for i in range(territory.shape[0]):
-        found = False
-        for j in range(weights.shape[1]):
-            if rand[i] <= weights[territory[i]][j]:
-                found = True
-                position[i] = connections[territory[i]][j]
-                territory[i] = connections[territory[i]][j]
-                break
-        if not found:
-            position[i] = territory[i]
-
-
-@nb.njit
-def movement_mov_around_territory_fill_bool_mov_using_condition(pre_bool_mov, condition):
-    counter = 0
-    bool_mov = np.full(condition.shape, False, dtype=np.bool_)
-    for i in range(condition.shape[0]):
-        if condition[i]:
-            if pre_bool_mov[counter]:
-                bool_mov[i] = True
-            counter += 1
-    return bool_mov
-
-
-@nb.njit
-def movement_mov_around_territory(territory, position, bool_mov, rand, connections, weights):
-    counter_rand = 0
-    for i in range(territory.shape[0]):
-        if bool_mov[i]:
-            for j in range(weights.shape[1]):
-                if rand[counter_rand] <= weights[territory[i]][j] and connections[territory[i]][j] != -1:
-                    position[i] = connections[territory[i]][j]
-                    break
-            counter_rand += 1
-
-
-@nb.njit
-def movement_dispersion_with_varying_nb_of_steps_condition(territory, position, condition, rand, arr_nb_steps,
-                                                           connections, weights):
-    counter_rand = 0
-    counter_arr_steps = 0
-    for i in range(territory.shape[0]):
-        if condition[i]:
-            position[i] = territory[i]
-            for _ in range(arr_nb_steps[counter_arr_steps]):
-                for j in range(weights.shape[1]):
-                    if rand[counter_rand] <= weights[territory[i]][j]:
-                        position[i] = connections[territory[i]][j]
-                        territory[i] = connections[territory[i]][j]
-                        break
-                counter_rand += 1
-            counter_arr_steps += 1
-
-
-@nb.njit
-def movement_dispersion_with_varying_nb_of_steps(territory, position, rand, arr_nb_steps,
-                                                 connections, weights):
-    counter_rand = 0
-    counter_arr_steps = 0
-    for i in range(territory.shape[0]):
-        position[i] = territory[i]
-        for _ in range(arr_nb_steps[counter_arr_steps]):
-            for j in range(weights.shape[1]):
-                if rand[counter_rand] <= weights[territory[i]][j]:
-                    position[i] = connections[territory[i]][j]
-                    territory[i] = connections[territory[i]][j]
-                    break
-            counter_rand += 1
-        counter_arr_steps += 1
-
-# ---------------------------------------------------------------------------------------------------------------------
-# spherical random walk section
-
-
-@nb.njit
-def random_walk_on_sphere_set_position_based_on_graph(arr_selected_agents, arr_pos_agent,
-                                                      agent_coord_x, agent_coord_y, agent_coord_z,
-                                                      graph_coord_x, graph_coord_y, graph_coord_z):
-    for i in range(arr_selected_agents.shape[0]):
-        if arr_selected_agents[i]:
-            ind_vertex = arr_pos_agent[i]
-            agent_coord_x[i] = graph_coord_x[ind_vertex]
-            agent_coord_y[i] = graph_coord_y[ind_vertex]
-            agent_coord_z[i] = graph_coord_z[ind_vertex]
-
-
-@nb.njit
-def random_walk_on_sphere_start_random_walk_uniform_prob(arr_start_rw, arr_iorw):
-    for i in range(arr_start_rw.shape[0]):
-        if arr_start_rw[i]:
-            arr_iorw[i] = True
-
-
-@nb.njit
-def random_walk_on_sphere_start_random_walk_uniform_prob_return_new_walkers(arr_start_rw, arr_iorw):
-    arr_new_walkers = np.full(arr_iorw.shape, False, dtype=np.bool_)
-    for i in range(arr_start_rw.shape[0]):
-        if arr_start_rw[i]:
-            if not arr_iorw[i]:
-                arr_new_walkers[i] = True
-            arr_iorw[i] = True
-    return arr_new_walkers
-
-
-@nb.njit
-def conditional_random_walk_on_sphere_start_random_walk_uniform_prob(arr_start_rw, arr_iorw, condition):
-    counter_arr_start_rw = 0
-    for i in range(arr_start_rw.shape[0]):
-        if condition[i]:
-            if arr_start_rw[counter_arr_start_rw]:
-                arr_iorw[i] = True
-            counter_arr_start_rw += 1
-
-
-@nb.njit
-def conditional_random_walk_on_sphere_start_random_walk_uniform_prob_return_new_walkers(arr_start_rw, arr_iorw,
-                                                                                        condition):
-    arr_new_walkers = np.full(arr_iorw.shape, False, dtype=np.bool_)
-    counter_arr_start_rw = 0
-    for i in range(arr_start_rw.shape[0]):
-        if condition[i]:
-            if arr_start_rw[counter_arr_start_rw]:
-                if not arr_iorw[i]:
-                    arr_new_walkers[i] = True
-                arr_iorw[i] = True
-            counter_arr_start_rw += 1
-    return arr_new_walkers
-
-
-@nb.njit
-def random_walk_on_sphere_set_initial_dir_to_north(arr_selected_agents,
-                                                   pos_x, pos_y, pos_z,
-                                                   dir_x, dir_y, dir_z):
-    for i in range(arr_selected_agents.shape[0]):
-        if arr_selected_agents[i]:
-            if pos_x[i] == 0. and pos_y[i] == 0:
-                dir_x[i] = 1.
-                dir_y[i] = 0.
-                dir_z[i] = 0.
-            else:
-                norm_p = np.sqrt(pos_x[i]**2 + pos_y[i]**2 + pos_z[i]**2)
-                position = np.array([pos_x[i], pos_y[i], pos_z[i]])
-                position = position / norm_p
-                # the direction toward the north at position is given, up to normalization, by the following formula
-                # (0, 0, 1) - <(0, 0, 1), position> position
-                # which leads to the following line
-                direction = np.array([-position[2] * position[0],
-                                      -position[2] * position[1],
-                                      1. - position[2] ** 2])
-                dir_norm = np.sqrt((direction[0] ** 2 + direction[1] ** 2 + direction[2] ** 2))
-                dir_x[i] = direction[0] / dir_norm
-                dir_y[i] = direction[1] / dir_norm
-                dir_z[i] = direction[2] / dir_norm
-
-
-@nb.njit
-def random_walk_on_sphere_deviate_direction_from_angles(deviation_angle, arr_selected_agents, px, py, pz,
-                                                        dx, dy, dz):
-    counter_dev_angle = 0
-    for i in range(arr_selected_agents.shape[0]):
-        if arr_selected_agents[i]:
-            angle = deviation_angle[counter_dev_angle]
-            norm_pos = np.sqrt(px[i]**2 + py[i]**2 + pz[i]**2)
-            position = np.array([px[i], py[i], pz[i]])
-            position = position / norm_pos
-
-            # we rotate the direction by an angle of Theta with respect to the rotation axis given by the position.
-            # position and direction are assumed to be orthonormal. We use the Euler-Rodrigues Formula.
-            c = np.cos(angle)
-            s = np.sin(angle)
-            direction = np.array([c * dx[i] + s * (position[1] * dz[i] - position[2] * dy[i]),
-                                  c * dy[i] + s * (position[2] * dx[i] - position[0] * dz[i]),
-                                  c * dz[i] + s * (position[0] * dy[i] - position[1] * dx[i])])
-
-            # normalizing the result to avoid accumulation of approximation errors.
-            direction = direction - np.dot(position, direction) * position
-            norm_d = np.sqrt(direction[0]**2 + direction[1]**2 + direction[2]**2)
-            direction = direction / norm_d
-
-            # saving the results
-            dx[i] = direction[0]
-            dy[i] = direction[1]
-            dz[i] = direction[2]
-
-            # increment the counter
-            counter_dev_angle += 1
-
-
-@nb.njit
-def random_walk_on_sphere_propose_step_gamma_law(arr_selected_agents, gamma_sample, pos_x, pos_y, pos_z, dir_x, dir_y, dir_z,
-                                       radius):
-    r_pos_x = np.full(gamma_sample.shape, -1.)
-    r_pos_y = np.full(gamma_sample.shape, -1.)
-    r_pos_z = np.full(gamma_sample.shape, -1.)
-
-    r_dir_x = np.full(gamma_sample.shape, -1.)
-    r_dir_y = np.full(gamma_sample.shape, -1.)
-    r_dir_z = np.full(gamma_sample.shape, -1.)
-
-    counter = 0
-    for i in range(arr_selected_agents.shape[0]):
-        if arr_selected_agents[i]:
-            angle = gamma_sample[counter] / radius
-            nmz_pos = np.array([pos_x[i], pos_y[i], pos_z[i]]) / np.sqrt(pos_x[i]**2 + pos_y[i]**2 + pos_z[i]**2)
-            direction = np.array([dir_x[i], dir_y[i], dir_z[i]])
-
-            nmz_new_pos = np.cos(angle) * nmz_pos + np.sin(angle) * direction
-            nmz_new_pos = nmz_new_pos / np.sqrt(nmz_new_pos[0] ** 2 + nmz_new_pos[1]**2 + nmz_new_pos[2]**2)
-
-            direction = np.cos(angle) * direction - np.sin(angle) * nmz_pos
-            # this next line is just there to be absolutely sure we stay normal to the position
-            direction = direction - (direction[0] * nmz_new_pos[0] + direction[1] * nmz_new_pos[1] +
-                                     direction[2] * nmz_new_pos[2]) * nmz_new_pos
-            # extra normalization because this step will be repeated many time
-            direction = direction / np.sqrt(direction[0]**2 + direction[1]**2 + direction[2]**2)
-
-            r_pos_x[counter] = radius * nmz_new_pos[0]
-            r_pos_y[counter] = radius * nmz_new_pos[1]
-            r_pos_z[counter] = radius * nmz_new_pos[2]
-
-            r_dir_x[counter] = direction[0]
-            r_dir_y[counter] = direction[1]
-            r_dir_z[counter] = direction[2]
-
-            counter += 1
-
-    return r_pos_x, r_pos_y, r_pos_z, r_dir_x, r_dir_y, r_dir_z
-
-
-@nb.njit
-def random_walk_on_sphere_make_step_gamma_law(arr_selected_agents, gamma_sample, pos_x, pos_y, pos_z, dir_x, dir_y,
-                                              dir_z, radius):
-    counter = 0
-    for i in range(arr_selected_agents.shape[0]):
-        if arr_selected_agents[i]:
-            angle = gamma_sample[counter] / radius
-            nmz_pos = np.array([pos_x[i], pos_y[i], pos_z[i]]) / np.sqrt(pos_x[i]**2 + pos_y[i]**2 + pos_z[i]**2)
-            direction = np.array([dir_x[i], dir_y[i], dir_z[i]])
-
-            nmz_new_pos = np.cos(angle) * nmz_pos + np.sin(angle) * direction
-            nmz_new_pos = nmz_new_pos / np.sqrt(nmz_new_pos[0] ** 2 + nmz_new_pos[1]**2 + nmz_new_pos[2]**2)
-
-            direction = np.cos(angle) * direction - np.sin(angle) * nmz_pos
-            # this next line is just there to be absolutely sure we stay normal to the position
-            direction = direction - (direction[0] * nmz_new_pos[0] + direction[1] * nmz_new_pos[1] +
-                                     direction[2] * nmz_new_pos[2]) * nmz_new_pos
-            # extra normalization because this step will be repeated many time
-            direction = direction / np.sqrt(direction[0]**2 + direction[1]**2 + direction[2]**2)
-
-            pos_x[i] = radius * nmz_new_pos[0]
-            pos_y[i] = radius * nmz_new_pos[1]
-            pos_z[i] = radius * nmz_new_pos[2]
-
-            dir_x[i] = direction[0]
-            dir_y[i] = direction[1]
-            dir_z[i] = direction[2]
-
-            counter += 1
-
-
-@nb.njit
-def random_walk_on_sphere_validate_step(arr_selected_agent, arr_success, proposed_px, proposed_py, proposed_pz,
-                                        proposed_dx, proposed_dy, proposed_dz, px, py, pz, dx, dy, dz):
-    counter = 0
-    for i in range(arr_selected_agent.shape[0]):
-        if arr_selected_agent[i]:
-            if arr_success[counter]:
-                px[i] = proposed_px[counter]
-                py[i] = proposed_py[counter]
-                pz[i] = proposed_pz[counter]
-                dx[i] = proposed_dx[counter]
-                dy[i] = proposed_dy[counter]
-                dz[i] = proposed_dz[counter]
-            counter += 1
-
-
-@nb.njit
-def random_walk_on_sphere_validate_step_return_fail(arr_selected_agent, arr_success, proposed_px, proposed_py,
-                                                    proposed_pz, proposed_dx, proposed_dy, proposed_dz, px, py, pz,
-                                                    dx, dy, dz):
-    returned_arr = np.full(arr_selected_agent.shape, False)
-    counter = 0
-    for i in range(arr_selected_agent.shape[0]):
-        if arr_selected_agent[i]:
-            if arr_success[counter]:
-                px[i] = proposed_px[counter]
-                py[i] = proposed_py[counter]
-                pz[i] = proposed_pz[counter]
-                dx[i] = proposed_dx[counter]
-                dy[i] = proposed_dy[counter]
-                dz[i] = proposed_dz[counter]
-            else:
-                arr_selected_agent[i] = True
-            counter += 1
-    return returned_arr
-
-
-@nb.njit
-def _temp_random_walk_on_sphere_exit_random_walk_based_on_k(arr_selected_agents, rand, prob, alpha, arr_pos, arr_k,
-                                                            arr_pop):
-    rv = np.full(arr_selected_agents.shape, False, dtype=np.bool_)
-    counter = 0
-    for i in range(arr_selected_agents.shape[0]):
-        if arr_selected_agents[i]:
-            if rand[counter] <= prob * np.exp(-alpha * (arr_pop[arr_pos[i]] / arr_k[arr_pos[i]])):
-                rv[i] = True
-            counter += 1
-    return rv
+import numba as nb
+import numpy as np
+from numba.typed import List
+
+
+# ---------------------------------------------------------------------------------------------------------------------
+# base section
+
+
+@nb.njit
+def count_nb_agent_per_vertex(arr_pos, nb_vertex):
+    rv = np.zeros((nb_vertex,), dtype=np.int32)
+    for i in range(arr_pos.shape[0]):
+        rv[arr_pos[i]] += 1
+    return rv
+
+
+@nb.njit
+def conditional_count_nb_agent_per_vertex(arr_condition, arr_pos, nb_vertex):
+    rv = np.zeros((nb_vertex,), dtype=np.int32)
+    for i in range(arr_pos.shape[0]):
+        if arr_condition[i]:
+            rv[arr_pos[i]] += 1
+    return rv
+
+# ---------------------------------------------------------------------------------------------------------------------
+# mortality section
+
+
+@nb.njit
+def mortality_natural_death_orm_methodology(bias, rand, arr_prob_male, arr_prob_female, arr_count, pos, k, age, gender):
+    rv = np.full(rand.shape, True, dtype=np.bool_)
+    for i in range(rv.shape[0]):
+        if k[pos[i]] == 0:
+            p = 1.
+        else:
+            if gender[i] == 0:
+                p = arr_prob_male[age[i]] * ((float(arr_count[pos[i]]) / float(k[pos[i]])) + bias)
+            else:
+                p = arr_prob_female[age[i]] * ((float(arr_count[pos[i]]) / float(k[pos[i]])) + bias)
+        if rand[i] <= p:
+            rv[i] = False
+            arr_count[pos[i]] -= 1
+    return rv
+
+
+@nb.njit
+def mortality_natural_death_orm_methodology_condition_count(bias, rand, arr_prob_male, arr_prob_female,
+                                                            arr_count, arr_cond_count, pos, k, age, gender):
+    rv = np.full(rand.shape, True, dtype=np.bool_)
+    for i in range(rv.shape[0]):
+        if k[pos[i]] == 0:
+            p = 1.
+        else:
+            if gender[i] == 0:
+                p = arr_prob_male[age[i]] * ((float(arr_count[pos[i]]) / float(k[pos[i]])) + bias)
+            else:
+                p = arr_prob_female[age[i]] * ((float(arr_count[pos[i]]) / float(k[pos[i]])) + bias)
+        if rand[i] <= p:
+            rv[i] = False
+            if arr_cond_count[i]:
+                arr_count[pos[i]] -= 1
+    return rv
+
+
+@nb.njit
+def mortality_natural_death_orm_methodology_condition_death(bias, rand, arr_prob_male, arr_prob_female,
+                                                            arr_count, arr_cond_death, pos, k, age, gender):
+    rv = np.full(rand.shape, True, dtype=np.bool_)
+    for i in range(rv.shape[0]):
+        if arr_cond_death[i]:
+            if k[pos[i]] == 0:
+                p = 1.
+            else:
+                if gender[i] == 0:
+                    p = arr_prob_male[age[i]] * ((float(arr_count[pos[i]]) / float(k[pos[i]])) + bias)
+                else:
+                    p = arr_prob_female[age[i]] * ((float(arr_count[pos[i]]) / float(k[pos[i]])) + bias)
+            if rand[i] <= p:
+                rv[i] = False
+                arr_count[pos[i]] -= 1
+    return rv
+
+
+@nb.njit
+def mortality_natural_death_orm_methodology_both_cond(bias, rand, arr_prob_male, arr_prob_female,
+                                                      arr_count, arr_cond_death, arr_cond_count, pos, k, age, gender):
+    rv = np.full(rand.shape, True, dtype=np.bool_)
+    for i in range(rv.shape[0]):
+        if arr_cond_death[i]:
+            if k[pos[i]] == 0:
+                p = 1.
+            else:
+                if gender[i] == 0:
+                    p = arr_prob_male[age[i]] * ((float(arr_count[pos[i]]) / float(k[pos[i]])) + bias)
+                else:
+                    p = arr_prob_female[age[i]] * ((float(arr_count[pos[i]]) / float(k[pos[i]])) + bias)
+            if rand[i] <= p:
+                rv[i] = False
+                if arr_cond_count[i]:
+                    arr_count[pos[i]] -= 1
+    return rv
+
+# ---------------------------------------------------------------------------------------------------------------------
+# reproduction
+
+
+@nb.njit
+def reproduction_find_random_mate_on_position(col_mate, col_pregnancy, arr_id, position, gender, nb_vertex,
+                                              rand_preg, prob_pregnancy):
+    list_vert_id_male = List()
+    list_vert_index_male = List()
+    for i in range(nb_vertex):
+        male_on_pos_i = List()
+        male_on_pos_i.append(arr_id[0])
+        male_on_pos_i.pop()
+        list_vert_id_male.append(male_on_pos_i)
+
+        index_male_on_pos_i = List()
+        index_male_on_pos_i.append(0)
+        index_male_on_pos_i.pop()
+        list_vert_index_male.append(index_male_on_pos_i)
+
+    arr_nb_male_per_vertex = np.full((nb_vertex,), 0, dtype=np.int32)
+    for i in range(arr_id.shape[0]):
+        col_mate[i] = -1
+        col_pregnancy[i] = False
+        if gender[i] == 0:
+            arr_nb_male_per_vertex[position[i]] += 1
+            list_vert_id_male[position[i]].append(arr_id[i])
+            list_vert_index_male[position[i]].append(i)
+
+    arr_ind_vertex = np.full((nb_vertex,), 0, dtype=np.int32)
+    counter = 0
+    for i in range(arr_id.shape[0]):
+        if gender[i] == 1:
+            if arr_ind_vertex[position[i]] < arr_nb_male_per_vertex[position[i]]:
+                col_mate[i] = list_vert_id_male[position[i]][arr_ind_vertex[position[i]]]
+                col_mate[list_vert_index_male[position[i]][arr_ind_vertex[position[i]]]] = arr_id[i]
+                arr_ind_vertex[position[i]] += 1
+                if rand_preg[counter] <= prob_pregnancy:
+                    col_pregnancy[i] = True
+            counter += 1
+
+
+@nb.njit
+def reproduction_find_random_mate_on_position_condition(col_mate, col_pregnancy, arr_id, position, gender, nb_vertex,
+                                                        rand_preg, prob_pregnancy, condition):
+    list_vert_id_male = List()
+    list_vert_index_male = List()
+    for i in range(nb_vertex):
+        male_on_pos_i = List()
+        male_on_pos_i.append(arr_id[0])
+        male_on_pos_i.pop()
+        list_vert_id_male.append(male_on_pos_i)
+
+        index_male_on_pos_i = List()
+        index_male_on_pos_i.append(0)
+        index_male_on_pos_i.pop()
+        list_vert_index_male.append(index_male_on_pos_i)
+
+    arr_nb_male_per_vertex = np.full((nb_vertex,), 0, dtype=np.int32)
+    for i in range(arr_id.shape[0]):
+        if condition[i]:
+            col_mate[i] = -1
+            col_pregnancy[i] = False
+            if gender[i] == 0:
+                arr_nb_male_per_vertex[position[i]] += 1
+                list_vert_id_male[position[i]].append(arr_id[i])
+                list_vert_index_male[position[i]].append(i)
+
+    arr_ind_vertex = np.full((nb_vertex,), 0, dtype=np.int32)
+    counter = 0
+    for i in range(arr_id.shape[0]):
+        if gender[i] == 1 and condition[i]:
+            if arr_ind_vertex[position[i]] < arr_nb_male_per_vertex[position[i]]:
+                col_mate[i] = list_vert_id_male[position[i]][arr_ind_vertex[position[i]]]
+                col_mate[list_vert_index_male[position[i]][arr_ind_vertex[position[i]]]] = arr_id[i]
+                arr_ind_vertex[position[i]] += 1
+                if rand_preg[counter] <= prob_pregnancy:
+                    col_pregnancy[i] = True
+            counter += 1
+
+
+@nb.njit
+def reproduction_find_random_mate_on_position_polygamous(arr_id, position, gender, col_mate, col_pregnant,
+                                                         nb_vertex, rand_preg, rand_chose_mate, prob_pregnancy):
+    list_vert_id_male = List()
+    for i in range(nb_vertex):
+        male_on_pos_i = List()
+        male_on_pos_i.append(arr_id[0])
+        male_on_pos_i.pop()
+        list_vert_id_male.append(male_on_pos_i)
+
+    arr_nb_male_per_vertex = np.full((nb_vertex,), 0, dtype=np.int32)
+    for i in range(arr_id.shape[0]):
+        col_pregnant[i] = False
+        col_mate[i] = -1
+        if gender[i] == 0:
+            arr_nb_male_per_vertex[position[i]] += 1
+            list_vert_id_male[position[i]].append(arr_id[i])
+
+    counter = 0
+    for i in range(arr_id.shape[0]):
+        if gender[i] == 1:
+            if arr_nb_male_per_vertex[position[i]] > 0:
+                rand_index_male = int(np.floor(rand_chose_mate[counter] * arr_nb_male_per_vertex[position[i]])) % \
+                                  arr_nb_male_per_vertex[position[i]]
+                col_mate[i] = list_vert_id_male[position[i]][rand_index_male]
+                if rand_preg[counter] <= prob_pregnancy:
+                    col_pregnant[i] = True
+            counter += 1
+
+
+@nb.njit
+def reproduction_find_random_mate_on_position_polygamous_condition(arr_id, position, gender, col_mate, col_pregnant,
+                                                                   nb_vertex, rand_preg, rand_chose_mate,
+                                                                   prob_pregnancy, condition):
+    list_vert_id_male = List()
+    for i in range(nb_vertex):
+        male_on_pos_i = List()
+        male_on_pos_i.append(arr_id[0])
+        male_on_pos_i.pop()
+        list_vert_id_male.append(male_on_pos_i)
+
+    arr_nb_male_per_vertex = np.full((nb_vertex,), 0, dtype=np.int32)
+    for i in range(arr_id.shape[0]):
+        if condition[i]:
+            col_pregnant[i] = False
+            col_mate[i] = -1
+            if gender[i] == 0:
+                arr_nb_male_per_vertex[position[i]] += 1
+                list_vert_id_male[position[i]].append(arr_id[i])
+
+    counter = 0
+    for i in range(arr_id.shape[0]):
+        if gender[i] == 1 and condition[i]:
+            if arr_nb_male_per_vertex[position[i]] > 0:
+                rand_index_male = int(np.floor(rand_chose_mate[counter] * arr_nb_male_per_vertex[position[i]])) % \
+                                  arr_nb_male_per_vertex[position[i]]
+                col_mate[i] = list_vert_id_male[position[i]][rand_index_male]
+                if rand_preg[counter] <= prob_pregnancy:
+                    col_pregnant[i] = True
+            counter += 1
+
+# ---------------------------------------------------------------------------------------------------------------------
+# graph based movement section
+
+
+@nb.njit
+def movement_change_territory_and_position_condition(territory, position, condition, rand, connections, weights):
+    counter_rand = 0
+    for i in range(territory.shape[0]):
+        if condition[i]:
+            found = False
+            for j in range(weights.shape[1]):
+                if rand[counter_rand] <= weights[territory[i]][j]:
+                    found = True
+                    # very important to update position first
+                    position[i] = connections[territory[i]][j]
+                    territory[i] = connections[territory[i]][j]
+                    break
+            if not found:
+                position[i] = territory[i]
+            counter_rand += 1
+
+
+@nb.njit
+def movement_change_territory_and_position(territory, position, rand, connections, weights):
+    for i in range(territory.shape[0]):
+        found = False
+        for j in range(weights.shape[1]):
+            if rand[i] <= weights[territory[i]][j]:
+                found = True
+                position[i] = connections[territory[i]][j]
+                territory[i] = connections[territory[i]][j]
+                break
+        if not found:
+            position[i] = territory[i]
+
+
+@nb.njit
+def movement_mov_around_territory_fill_bool_mov_using_condition(pre_bool_mov, condition):
+    counter = 0
+    bool_mov = np.full(condition.shape, False, dtype=np.bool_)
+    for i in range(condition.shape[0]):
+        if condition[i]:
+            if pre_bool_mov[counter]:
+                bool_mov[i] = True
+            counter += 1
+    return bool_mov
+
+
+@nb.njit
+def movement_mov_around_territory(territory, position, bool_mov, rand, connections, weights):
+    counter_rand = 0
+    for i in range(territory.shape[0]):
+        if bool_mov[i]:
+            for j in range(weights.shape[1]):
+                if rand[counter_rand] <= weights[territory[i]][j] and connections[territory[i]][j] != -1:
+                    position[i] = connections[territory[i]][j]
+                    break
+            counter_rand += 1
+
+
+@nb.njit
+def movement_dispersion_with_varying_nb_of_steps_condition(territory, position, condition, rand, arr_nb_steps,
+                                                           connections, weights):
+    counter_rand = 0
+    counter_arr_steps = 0
+    for i in range(territory.shape[0]):
+        if condition[i]:
+            position[i] = territory[i]
+            for _ in range(arr_nb_steps[counter_arr_steps]):
+                for j in range(weights.shape[1]):
+                    if rand[counter_rand] <= weights[territory[i]][j]:
+                        position[i] = connections[territory[i]][j]
+                        territory[i] = connections[territory[i]][j]
+                        break
+                counter_rand += 1
+            counter_arr_steps += 1
+
+
+@nb.njit
+def movement_dispersion_with_varying_nb_of_steps(territory, position, rand, arr_nb_steps,
+                                                 connections, weights):
+    counter_rand = 0
+    counter_arr_steps = 0
+    for i in range(territory.shape[0]):
+        position[i] = territory[i]
+        for _ in range(arr_nb_steps[counter_arr_steps]):
+            for j in range(weights.shape[1]):
+                if rand[counter_rand] <= weights[territory[i]][j]:
+                    position[i] = connections[territory[i]][j]
+                    territory[i] = connections[territory[i]][j]
+                    break
+            counter_rand += 1
+        counter_arr_steps += 1
+
+# ---------------------------------------------------------------------------------------------------------------------
+# spherical random walk section
+
+
+@nb.njit
+def random_walk_on_sphere_set_position_based_on_graph(arr_selected_agents, arr_pos_agent,
+                                                      agent_coord_x, agent_coord_y, agent_coord_z,
+                                                      graph_coord_x, graph_coord_y, graph_coord_z):
+    for i in range(arr_selected_agents.shape[0]):
+        if arr_selected_agents[i]:
+            ind_vertex = arr_pos_agent[i]
+            agent_coord_x[i] = graph_coord_x[ind_vertex]
+            agent_coord_y[i] = graph_coord_y[ind_vertex]
+            agent_coord_z[i] = graph_coord_z[ind_vertex]
+
+
+@nb.njit
+def random_walk_on_sphere_start_random_walk_uniform_prob(arr_start_rw, arr_iorw):
+    for i in range(arr_start_rw.shape[0]):
+        if arr_start_rw[i]:
+            arr_iorw[i] = True
+
+
+@nb.njit
+def random_walk_on_sphere_start_random_walk_uniform_prob_return_new_walkers(arr_start_rw, arr_iorw):
+    arr_new_walkers = np.full(arr_iorw.shape, False, dtype=np.bool_)
+    for i in range(arr_start_rw.shape[0]):
+        if arr_start_rw[i]:
+            if not arr_iorw[i]:
+                arr_new_walkers[i] = True
+            arr_iorw[i] = True
+    return arr_new_walkers
+
+
+@nb.njit
+def conditional_random_walk_on_sphere_start_random_walk_uniform_prob(arr_start_rw, arr_iorw, condition):
+    counter_arr_start_rw = 0
+    for i in range(arr_start_rw.shape[0]):
+        if condition[i]:
+            if arr_start_rw[counter_arr_start_rw]:
+                arr_iorw[i] = True
+            counter_arr_start_rw += 1
+
+
+@nb.njit
+def conditional_random_walk_on_sphere_start_random_walk_uniform_prob_return_new_walkers(arr_start_rw, arr_iorw,
+                                                                                        condition):
+    arr_new_walkers = np.full(arr_iorw.shape, False, dtype=np.bool_)
+    counter_arr_start_rw = 0
+    for i in range(arr_start_rw.shape[0]):
+        if condition[i]:
+            if arr_start_rw[counter_arr_start_rw]:
+                if not arr_iorw[i]:
+                    arr_new_walkers[i] = True
+                arr_iorw[i] = True
+            counter_arr_start_rw += 1
+    return arr_new_walkers
+
+
+@nb.njit
+def random_walk_on_sphere_set_initial_dir_to_north(arr_selected_agents,
+                                                   pos_x, pos_y, pos_z,
+                                                   dir_x, dir_y, dir_z):
+    for i in range(arr_selected_agents.shape[0]):
+        if arr_selected_agents[i]:
+            if pos_x[i] == 0. and pos_y[i] == 0:
+                dir_x[i] = 1.
+                dir_y[i] = 0.
+                dir_z[i] = 0.
+            else:
+                norm_p = np.sqrt(pos_x[i]**2 + pos_y[i]**2 + pos_z[i]**2)
+                position = np.array([pos_x[i], pos_y[i], pos_z[i]])
+                position = position / norm_p
+                # the direction toward the north at position is given, up to normalization, by the following formula
+                # (0, 0, 1) - <(0, 0, 1), position> position
+                # which leads to the following line
+                direction = np.array([-position[2] * position[0],
+                                      -position[2] * position[1],
+                                      1. - position[2] ** 2])
+                dir_norm = np.sqrt((direction[0] ** 2 + direction[1] ** 2 + direction[2] ** 2))
+                dir_x[i] = direction[0] / dir_norm
+                dir_y[i] = direction[1] / dir_norm
+                dir_z[i] = direction[2] / dir_norm
+
+
+@nb.njit
+def random_walk_on_sphere_deviate_direction_from_angles(deviation_angle, arr_selected_agents, px, py, pz,
+                                                        dx, dy, dz):
+    counter_dev_angle = 0
+    for i in range(arr_selected_agents.shape[0]):
+        if arr_selected_agents[i]:
+            angle = deviation_angle[counter_dev_angle]
+            norm_pos = np.sqrt(px[i]**2 + py[i]**2 + pz[i]**2)
+            position = np.array([px[i], py[i], pz[i]])
+            position = position / norm_pos
+
+            # we rotate the direction by an angle of Theta with respect to the rotation axis given by the position.
+            # position and direction are assumed to be orthonormal. We use the Euler-Rodrigues Formula.
+            c = np.cos(angle)
+            s = np.sin(angle)
+            direction = np.array([c * dx[i] + s * (position[1] * dz[i] - position[2] * dy[i]),
+                                  c * dy[i] + s * (position[2] * dx[i] - position[0] * dz[i]),
+                                  c * dz[i] + s * (position[0] * dy[i] - position[1] * dx[i])])
+
+            # normalizing the result to avoid accumulation of approximation errors.
+            direction = direction - np.dot(position, direction) * position
+            norm_d = np.sqrt(direction[0]**2 + direction[1]**2 + direction[2]**2)
+            direction = direction / norm_d
+
+            # saving the results
+            dx[i] = direction[0]
+            dy[i] = direction[1]
+            dz[i] = direction[2]
+
+            # increment the counter
+            counter_dev_angle += 1
+
+
+@nb.njit
+def random_walk_on_sphere_propose_step_gamma_law(arr_selected_agents, gamma_sample, pos_x, pos_y, pos_z, dir_x, dir_y, 
+                                                dir_z, radius):
+    r_pos_x = np.full(gamma_sample.shape, -1.)
+    r_pos_y = np.full(gamma_sample.shape, -1.)
+    r_pos_z = np.full(gamma_sample.shape, -1.)
+
+    r_dir_x = np.full(gamma_sample.shape, -1.)
+    r_dir_y = np.full(gamma_sample.shape, -1.)
+    r_dir_z = np.full(gamma_sample.shape, -1.)
+
+    counter = 0
+    for i in range(arr_selected_agents.shape[0]):
+        if arr_selected_agents[i]:
+            angle = gamma_sample[counter] / radius
+            nmz_pos = np.array([pos_x[i], pos_y[i], pos_z[i]]) / np.sqrt(pos_x[i]**2 + pos_y[i]**2 + pos_z[i]**2)
+            direction = np.array([dir_x[i], dir_y[i], dir_z[i]])
+
+            nmz_new_pos = np.cos(angle) * nmz_pos + np.sin(angle) * direction
+            nmz_new_pos = nmz_new_pos / np.sqrt(nmz_new_pos[0] ** 2 + nmz_new_pos[1]**2 + nmz_new_pos[2]**2)
+
+            direction = np.cos(angle) * direction - np.sin(angle) * nmz_pos
+            # this next line is just there to be absolutely sure we stay normal to the position
+            direction = direction - (direction[0] * nmz_new_pos[0] + direction[1] * nmz_new_pos[1] +
+                                     direction[2] * nmz_new_pos[2]) * nmz_new_pos
+            # extra normalization because this step will be repeated many time
+            direction = direction / np.sqrt(direction[0]**2 + direction[1]**2 + direction[2]**2)
+
+            r_pos_x[counter] = radius * nmz_new_pos[0]
+            r_pos_y[counter] = radius * nmz_new_pos[1]
+            r_pos_z[counter] = radius * nmz_new_pos[2]
+
+            r_dir_x[counter] = direction[0]
+            r_dir_y[counter] = direction[1]
+            r_dir_z[counter] = direction[2]
+
+            counter += 1
+
+    return r_pos_x, r_pos_y, r_pos_z, r_dir_x, r_dir_y, r_dir_z
+
+
+@nb.njit
+def random_walk_on_sphere_make_step_gamma_law(arr_selected_agents, gamma_sample, pos_x, pos_y, 
+                                              pos_z, dir_x, dir_y, dir_z, radius):
+    counter = 0
+    for i in range(arr_selected_agents.shape[0]):
+        if arr_selected_agents[i]:
+            angle = gamma_sample[counter] / radius
+            nmz_pos = np.array([pos_x[i], pos_y[i], pos_z[i]]) / np.sqrt(pos_x[i]**2 + pos_y[i]**2 + pos_z[i]**2)
+            direction = np.array([dir_x[i], dir_y[i], dir_z[i]])
+
+            nmz_new_pos = np.cos(angle) * nmz_pos + np.sin(angle) * direction
+            nmz_new_pos = nmz_new_pos / np.sqrt(nmz_new_pos[0] ** 2 + nmz_new_pos[1]**2 + nmz_new_pos[2]**2)
+
+            direction = np.cos(angle) * direction - np.sin(angle) * nmz_pos
+            # this next line is just there to be absolutely sure we stay normal to the position
+            direction = direction - (direction[0] * nmz_new_pos[0] + direction[1] * nmz_new_pos[1] +
+                                     direction[2] * nmz_new_pos[2]) * nmz_new_pos
+            # extra normalization because this step will be repeated many time
+            direction = direction / np.sqrt(direction[0]**2 + direction[1]**2 + direction[2]**2)
+
+            pos_x[i] = radius * nmz_new_pos[0]
+            pos_y[i] = radius * nmz_new_pos[1]
+            pos_z[i] = radius * nmz_new_pos[2]
+
+            dir_x[i] = direction[0]
+            dir_y[i] = direction[1]
+            dir_z[i] = direction[2]
+
+            counter += 1
+
+
+@nb.njit
+def random_walk_on_sphere_validate_step(arr_selected_agent, arr_success, proposed_px, proposed_py, proposed_pz,
+                                        proposed_dx, proposed_dy, proposed_dz, px, py, pz, dx, dy, dz):
+    counter = 0
+    for i in range(arr_selected_agent.shape[0]):
+        if arr_selected_agent[i]:
+            if arr_success[counter]:
+                px[i] = proposed_px[counter]
+                py[i] = proposed_py[counter]
+                pz[i] = proposed_pz[counter]
+                dx[i] = proposed_dx[counter]
+                dy[i] = proposed_dy[counter]
+                dz[i] = proposed_dz[counter]
+            counter += 1
+
+
+@nb.njit
+def random_walk_on_sphere_validate_step_return_fail(arr_selected_agent, arr_success, proposed_px, proposed_py,
+                                                    proposed_pz, proposed_dx, proposed_dy, proposed_dz, px, py, pz,
+                                                    dx, dy, dz):
+    returned_arr = np.full(arr_selected_agent.shape, False, dtype=np.bool_)
+    counter = 0
+    for i in range(arr_selected_agent.shape[0]):
+        if arr_selected_agent[i]:
+            if arr_success[counter]:
+                px[i] = proposed_px[counter]
+                py[i] = proposed_py[counter]
+                pz[i] = proposed_pz[counter]
+                dx[i] = proposed_dx[counter]
+                dy[i] = proposed_dy[counter]
+                dz[i] = proposed_dz[counter]
+            else:
+                returned_arr[i] = True
+            counter += 1
+    return returned_arr
+
+
+@nb.njit
+def random_walk_on_sphere_exit_random_walk_according_to_proximity_class(arr_sucess, arr_position, arr_selected_agents,
+                                                                        arr_pos_attribute, arr_walk_status):
+    counter = 0
+    for i in range(arr_selected_agents.shape[0]):
+        if arr_selected_agents[i]:
+            if arr_sucess[counter]:
+                arr_pos_attribute[i] = arr_position[counter]
+                arr_walk_status[i] = False
+            counter += 1
+
+
+@nb.njit
+def random_walk_on_sphere_exit_random_walk_according_to_proximity_class_return_fail(arr_sucess, arr_position, 
+                                                    arr_selected_agents, arr_pos_attribute, arr_walk_status):
+    r_fail = np.full(arr_selected_agents.shape, False, dtype=nb.types.bool_)
+    counter = 0
+    for i in range(arr_selected_agents.shape[0]):
+        if arr_selected_agents[i]:
+            if arr_sucess[counter]:
+                arr_pos_attribute[i] = arr_position[counter]
+                arr_walk_status[i] = False
+            else:
+                r_fail[i] = True
+            counter += 1
+    return r_fail
+
+
+@nb.njit
+def random_walk_on_sphere_exit_random_walk_according_to_proximity_class_no_status_update(arr_sucess, arr_position, 
+                                                                                         arr_selected_agents,
+                                                                                         arr_pos_attribute):
+    counter = 0
+    for i in range(arr_selected_agents.shape[0]):
+        if arr_selected_agents[i]:
+            if arr_sucess[counter]:
+                arr_pos_attribute[i] = arr_position[counter]
+            counter += 1
+
+
+@nb.njit
+def _temp_random_walk_on_sphere_exit_random_walk_based_on_k(arr_selected_agents, rand, prob, alpha, arr_pos, arr_k,
+                                                            arr_pop):
+    rv = np.full(arr_selected_agents.shape, False, dtype=np.bool_)
+    counter = 0
+    for i in range(arr_selected_agents.shape[0]):
+        if arr_selected_agents[i]:
+            if rand[counter] <= prob * np.exp(-alpha * (arr_pop[arr_pos[i]] / arr_k[arr_pos[i]])):
+                rv[i] = True
+            counter += 1
+    return rv
+
+
+# ---------------------------------------------------------------------------------------------------------------------
+# reproduction with markers section
+
+@nb.njit
+def reproduction_with_marker_find_random_mate_on_position(col_mate, col_pregnancy, arr_id, 
+                                                          position, gender, nb_vertex,
+                                                          rand_preg, prob_pregnancy,
+                                                          arr_markers):
+    returned_dict = dict()
+
+    list_vert_id_male = List()
+    list_vert_index_male = List()
+    for i in range(nb_vertex):
+        male_on_pos_i = List()
+        male_on_pos_i.append(arr_id[0])
+        male_on_pos_i.pop()
+        list_vert_id_male.append(male_on_pos_i)
+
+        index_male_on_pos_i = List()
+        index_male_on_pos_i.append(0)
+        index_male_on_pos_i.pop()
+        list_vert_index_male.append(index_male_on_pos_i)
+
+    arr_nb_male_per_vertex = np.full((nb_vertex,), 0, dtype=np.int32)
+    for i in range(arr_id.shape[0]):
+        col_mate[i] = -1
+        col_pregnancy[i] = False
+        if gender[i] == 0:
+            arr_nb_male_per_vertex[position[i]] += 1
+            list_vert_id_male[position[i]].append(arr_id[i])
+            list_vert_index_male[position[i]].append(i)
+            returned_dict[arr_id[i]] = arr_markers[i, :]
+
+    arr_ind_vertex = np.full((nb_vertex,), 0, dtype=np.int32)
+    counter = 0
+    for i in range(arr_id.shape[0]):
+        if gender[i] == 1:
+            if arr_ind_vertex[position[i]] < arr_nb_male_per_vertex[position[i]]:
+                col_mate[i] = list_vert_id_male[position[i]][arr_ind_vertex[position[i]]]
+                col_mate[list_vert_index_male[position[i]][arr_ind_vertex[position[i]]]] = arr_id[i]
+                arr_ind_vertex[position[i]] += 1
+                if rand_preg[counter] <= prob_pregnancy:
+                    col_pregnancy[i] = True
+            counter += 1
+
+    return returned_dict
+
+
+@nb.njit
+def reproduction_with_markers_find_random_mate_on_position_condition(col_mate, col_pregnancy, 
+                                                                     arr_id, position, gender, 
+                                                                     nb_vertex, rand_preg, 
+                                                                     prob_pregnancy, condition,
+                                                                     arr_markers):
+    returned_dict = dict()
+
+    list_vert_id_male = List()
+    list_vert_index_male = List()
+    for i in range(nb_vertex):
+        male_on_pos_i = List()
+        male_on_pos_i.append(arr_id[0])
+        male_on_pos_i.pop()
+        list_vert_id_male.append(male_on_pos_i)
+
+        index_male_on_pos_i = List()
+        index_male_on_pos_i.append(0)
+        index_male_on_pos_i.pop()
+        list_vert_index_male.append(index_male_on_pos_i)
+
+    arr_nb_male_per_vertex = np.full((nb_vertex,), 0, dtype=np.int32)
+    for i in range(arr_id.shape[0]):
+        if condition[i]:
+            col_mate[i] = -1
+            col_pregnancy[i] = False
+            if gender[i] == 0:
+                arr_nb_male_per_vertex[position[i]] += 1
+                list_vert_id_male[position[i]].append(arr_id[i])
+                list_vert_index_male[position[i]].append(i)
+                returned_dict[arr_id[i]] = arr_markers[i, :]
+
+    arr_ind_vertex = np.full((nb_vertex,), 0, dtype=np.int32)
+    counter = 0
+    for i in range(arr_id.shape[0]):
+        if gender[i] == 1 and condition[i]:
+            if arr_ind_vertex[position[i]] < arr_nb_male_per_vertex[position[i]]:
+                col_mate[i] = list_vert_id_male[position[i]][arr_ind_vertex[position[i]]]
+                col_mate[list_vert_index_male[position[i]][arr_ind_vertex[position[i]]]] = arr_id[i]
+                arr_ind_vertex[position[i]] += 1
+                if rand_preg[counter] <= prob_pregnancy:
+                    col_pregnancy[i] = True
+            counter += 1
+
+    return returned_dict
+
+
+@nb.njit
+def reproduction_with_marker_extract_gene_from_dict(arr_father_id, dict_marker_of_fathers, arr_markers):
+    for i in range(arr_markers.shape[0]):
+        for j in range(arr_markers.shape[0]):
+            arr_markers[i, j] = dict_marker_of_fathers[arr_father_id[i]][j]
+
+
+@nb.njit
+def reproduction_with_marker_attribute_genes_to_offsprings(arr_offsprings_gene, 
+                                                           arr_father_genes, 
+                                                           arr_mother_genes,
+                                                           arr_random):
+    for i in range(arr_offsprings_gene.shape[0]):
+        for j in range(arr_offsprings_gene.shape[0] // 2):
+            arr_offsprings_gene[i, 2*j] = arr_mother_genes[i, 2*j + arr_random[i, 2*j]]
+            arr_offsprings_gene[i, 2*j + 1] = arr_father_genes[i, 2*j + arr_random[i, 2*j + 1]]
```

### Comparing `sampy-abm-1.0.2/src/sampy/agent/mortality.py` & `sampy_abm-1.0.3/src/sampy/agent/mortality.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,268 +1,268 @@
-import numpy as np
-from .jit_compiled_functions import *
-from ..pandas_xs.pandas_xs import DataFrameXS
-from ..utils.errors_shortcut import (check_col_exists_good_type,
-                                     check_input_array,
-                                     check_input_is_permutation,
-                                     check_if_gender_array)
-
-
-class NaturalMortalityOrmMethodology:
-    """
-    This class provides methods to modelize natural mortality.
-    See description of method 'natural_death_orm_methodology' for a precise description.
-    """
-    def __init__(self, **kwargs):
-        if not hasattr(self, 'df_population'):
-            self.df_population = DataFrameXS()
-
-    def _sampy_debug_natural_death_orm_methodology(self, array_death_proba_male, array_death_proba_female,
-                                                   shuffle=False,
-                                                   permutation_shuffle=None,
-                                                   condition=None,
-                                                   condition_count=None,
-                                                   gender_attribute='gender',
-                                                   age_attribute='age',
-                                                   position_attribute='position',
-                                                   k_factor_attribute='K'):
-        if self.df_population.nb_rows == 0:
-            return
-
-        check_col_exists_good_type(self.df_population, position_attribute, 'position_attribute', 'int',
-                                   reject_none=True)
-        check_col_exists_good_type(self.graph.df_attributes, k_factor_attribute, 'k_factor_attribute', 'float',
-                                   reject_none=True)
-
-        # we check that the 2 first arrays are 1D float array
-        check_input_array(array_death_proba_female, 'array_death_proba_female', 'float', nb_dim=1)
-        check_input_array(array_death_proba_male, 'array_death_proba_male', 'float', nb_dim=1)
-
-        # we need to check that there is no animal whose age is bigger than the size of the prob_arrays.
-        # in order to do so, we need to check that age_attribute and gender_attribute are properly used.
-        check_col_exists_good_type(self.df_population, age_attribute, 'age_attribute',
-                                   prefix_dtype='int', reject_none=True)
-
-        # now the gender attribute
-        check_col_exists_good_type(self.df_population, gender_attribute, 'gender_attribute',
-                                   prefix_dtype='int', reject_none=True)
-        check_if_gender_array(self.df_population[gender_attribute])
-
-        # now we check that there are no animal too old.
-        max_female = self.df_population[age_attribute][self.df_population[gender_attribute] == 1].max()
-        if max_female >= array_death_proba_female.shape[0]:
-            raise ValueError("There is a female agent of age " + str(max_female) + " while the array "
-                             "array_death_proba_female covers only ages until " +
-                             str(array_death_proba_female.shape[0] - 1) + ".")
-
-        max_male = self.df_population[age_attribute][self.df_population[gender_attribute] == 0].max()
-        if max_male >= array_death_proba_male.shape[0]:
-            raise ValueError("There is a male agent of age " + str(max_male) + " while the array "
-                             "array_death_proba_male covers only ages until " +
-                             str(array_death_proba_male.shape[0] - 1) + ".")
-
-        if permutation_shuffle is not None:
-            if not shuffle:
-                raise ValueError("A value for permutation_shuffle has been provided while shuffle is deactivated.")
-            check_input_is_permutation(permutation_shuffle, 'permutation_shuffle', length=self.df_population.nb_rows)
-
-        if condition is not None:
-            check_input_array(condition, 'condition', 'bool', shape=(self.df_population.nb_rows,))
-
-        if condition_count is not None:
-            check_input_array(condition_count, 'condition_count', 'bool', shape=(self.df_population.nb_rows,))
-
-    def natural_death_orm_methodology(self, array_death_proba_male, array_death_proba_female,
-                                      bias=0.,
-                                      shuffle=True,
-                                      permutation_shuffle=None,
-                                      condition=None,
-                                      condition_count=None,
-                                      gender_attribute='gender',
-                                      age_attribute='age',
-                                      position_attribute='position',
-                                      k_factor_attribute='K',
-                                      return_death_dataframe=False
-                                      ):
-        """
-        Kill agents using ORM methodology. I.E. the probability for a given agent to die is given by the formula:
-
-                            'prob_death * ( bias + (nb_agents_on_cell / K_cell) )'
-
-        Where prob_death is a parameter depending on the age of the agent, nb_agents_on_cell is the number of agent on
-        the cell of the tested agent (this number is updated along the process), and K is the K parameter of the current
-        cell. This method takes the gender into account.
-
-        The user can shuffle the dataframe before applying this function using the kwarg 'shuffle', and supply a
-        permutation to be used for the shuffling using the kwarg 'permutation_shuffle'. The user can also
-        specify two conditions as 1D boolean arrays:
-
-            - condition: array telling which agents are susceptible to be killed
-            - condition_count: array telling which agents are counted to determine the number of agents in each cell.
-                               This is useful if, for instance, the user wants to exclude juveniles from the
-                               nb_agents_on_cell used in the above formula.
-
-        WARNING: if shuffle is used, then any data previously extracted using the row position of the agents in the
-                 DataFrame df_population will be irrelevant.
-
-        :param array_death_proba_male: 1D array of float where array_death_proba_male[i] is the proba of death of a
-                                       male agent whose age is 'i'.
-        :param array_death_proba_female: 1D array of float where array_death_proba_female[i] is the proba of death of a
-                                         female agent whose age is 'i'.
-        :param bias: optional, float, default 0. Hyperparameter used to configure the mortality. Represents a 'base
-                     mortality'.
-        :param shuffle: optional, boolean, default True.
-        :param permutation_shuffle: optional, 1D array of int, default None. Permutation used for the shuffle. If
-                                    shuffle is activated and no permutation is provided, then one is generated using
-                                    numpy.random.permutation
-        :param condition: optional, 1D array of bool, default None. Array telling which agent are susceptible to die.
-        :param condition_count: optional, 1D array of bool, default None. Array telling which agent are to be counted.
-        :param gender_attribute: optional, string, default 'gender'. Name of the column containing gender info.
-        :param age_attribute: optional, string, default 'age'. Name of the column containing age info.
-        :param position_attribute: optional, string, default 'position'. Name of the column containing position info.
-        :param k_factor_attribute: optional, string, default 'K'. Name of the column containing K value in graph
-                                   df_attribute DataFrame.
-        :param return_death_dataframe: optional, boolean, default False. If True, returns a DataFrameXS containing all
-                                       the agents killed during this method call
-
-        :return: if return_death_dataframe is set to True, returns a DataFrameXS containing the agents killed during
-                 this method call.
-        """
-        if self.df_population.nb_rows == 0:
-            return
-        # shuffle the population dataframe if required
-        if shuffle:
-            used_permutation = self.df_population.scramble(permutation=permutation_shuffle, return_permutation=True)
-            if condition is not None:
-                condition = condition[used_permutation]
-            if condition_count is not None:
-                condition_count = condition_count[used_permutation]
-
-        # count agents per cell
-        count_arr = self.count_pop_per_vertex(position_attribute=position_attribute, condition=condition_count)
-        if condition is None:
-            if condition_count is None:
-                arr_survive = mortality_natural_death_orm_methodology(bias,
-                                                                      np.random.uniform(0, 1,
-                                                                                        self.df_population.nb_rows),
-                                                                      array_death_proba_male,
-                                                                      array_death_proba_female, count_arr,
-                                                                      self.df_population[position_attribute],
-                                                                      self.graph.df_attributes[k_factor_attribute],
-                                                                      self.df_population[age_attribute],
-                                                                      self.df_population[gender_attribute])
-            else:
-                arr_survive = mortality_natural_death_orm_methodology_condition_count(
-                                                                bias,
-                                                                np.random.uniform(0, 1, self.df_population.nb_rows),
-                                                                array_death_proba_male,
-                                                                array_death_proba_female, count_arr,
-                                                                condition_count,
-                                                                self.df_population[position_attribute],
-                                                                self.graph.df_attributes[k_factor_attribute],
-                                                                self.df_population[age_attribute],
-                                                                self.df_population[gender_attribute])
-        else:
-            if condition_count is None:
-                arr_survive = mortality_natural_death_orm_methodology_condition_death(
-                                                                bias,
-                                                                np.random.uniform(0, 1, self.df_population.nb_rows),
-                                                                array_death_proba_male,
-                                                                array_death_proba_female, count_arr,
-                                                                condition,
-                                                                self.df_population[position_attribute],
-                                                                self.graph.df_attributes[k_factor_attribute],
-                                                                self.df_population[age_attribute],
-                                                                self.df_population[gender_attribute])
-            else:
-                arr_survive = mortality_natural_death_orm_methodology_both_cond(
-                                                                bias,
-                                                                np.random.uniform(0, 1, self.df_population.nb_rows),
-                                                                array_death_proba_male,
-                                                                array_death_proba_female, count_arr,
-                                                                condition, condition_count,
-                                                                self.df_population[position_attribute],
-                                                                self.graph.df_attributes[k_factor_attribute],
-                                                                self.df_population[age_attribute],
-                                                                self.df_population[gender_attribute])
-
-        if return_death_dataframe:
-            death_df = self.df_population[~arr_survive]
-            self.df_population = self.df_population[arr_survive]
-            return death_df
-        else:
-            self.df_population = self.df_population[arr_survive]
-
-    def kill_too_old(self, limit_age, age_attribute='age'):
-        """
-        Kill agents whose age is greater or equal to the specified limit age.
-
-        :param limit_age: integer. Any agent older than this parameter will be killed.
-        :param age_attribute: optional, string, default 'age'. Name of the age attribute in the population dataframe.
-        """
-        self.df_population = self.df_population[self.df_population[age_attribute] < limit_age]
-
-
-class OffspringDependantOnParents:
-    """
-    This class add the possibility to kill the dependent offsprings whose mother is dead.
-    """
-    def __init__(self, **kwargs):
-        pass
-
-    def _sampy_debug_kill_children_whose_mother_is_dead(self, age_limit,
-                                                        id_attribute='col_id',
-                                                        age_attribute='age',
-                                                        mother_id_attribute='mom_id'):
-        if self.df_population.nb_rows == 0:
-            return
-        check_col_exists_good_type(self.df_population, age_attribute, 'age_attribute', prefix_dtype='int',
-                                   reject_none=True)
-        check_col_exists_good_type(self.df_population, mother_id_attribute, 'mother_id_attribute', prefix_dtype='int',
-                                   reject_none=True)
-
-    def kill_children_whose_mother_is_dead(self, age_limit,
-                                           id_attribute='col_id',
-                                           age_attribute='age',
-                                           mother_id_attribute='mom_id'):
-        """
-        Kill the agents that are not independent yet and whose mother is dead. Note that an agent whose age is precisely
-        age_limit is not considered independent.
-
-        :param age_limit: integer. Age of independence.
-        :param id_attribute: optional, string, default 'col_id'
-        :param age_attribute: optional, string, default 'age'
-        :param mother_id_attribute: optional, string, default 'mom_id'
-        """
-        if self.df_population.nb_rows == 0:
-            return
-        young = self.df_population[age_attribute] <= age_limit
-        has_mom = self.df_population.check_arr_in_col(self.df_population[mother_id_attribute], id_attribute,
-                                                      condition=young)
-        too_old = np.array(self.df_population[age_attribute] > age_limit)
-        self.df_population = self.df_population[has_mom | too_old]
-
-
-class KillPercentagePop:
-    """
-    This class adds the possibility to kill a given percentage of the population.
-    """
-    def __init__(self, **kwargs):
-        pass
-
-    def _sampy_debug_kill_proportion_of_population(self, proportion, condition=None):
-        if condition is not None:
-            check_input_array(condition, 'condition', 'bool', shape=(self.df_population.nb_rows,))
-
-    def kill_proportion_of_population(self, proportion, condition=None):
-        """
-        For each agent, a random uniform number between 0 and 1 is sampled, and each agent for which this number is
-        smaller than the argument 'proportion' is killed. Note that the user can use the kwarg 'condition' to
-        exclude some agents from this test.
-
-        :param proportion: float between 0 and 1.
-        :param condition: optional, 1D array of bool, default None.
-        """
-        rand = np.random.uniform(0, 1, (self.df_population.nb_rows,)) > proportion
-        if condition is not None:
-            rand = rand & condition
-        self.df_population = self.df_population[rand]
+import numpy as np
+from .jit_compiled_functions import *
+from ..pandas_xs.pandas_xs import DataFrameXS
+from ..utils.errors_shortcut import (check_col_exists_good_type,
+                                     check_input_array,
+                                     check_input_is_permutation,
+                                     check_if_gender_array)
+
+
+class NaturalMortalityOrmMethodology:
+    """
+    This class provides methods to modelize natural mortality.
+    See description of method 'natural_death_orm_methodology' for a precise description.
+    """
+    def __init__(self, **kwargs):
+        if not hasattr(self, 'df_population'):
+            self.df_population = DataFrameXS()
+
+    def _sampy_debug_natural_death_orm_methodology(self, array_death_proba_male, array_death_proba_female,
+                                                   shuffle=False,
+                                                   permutation_shuffle=None,
+                                                   condition=None,
+                                                   condition_count=None,
+                                                   gender_attribute='gender',
+                                                   age_attribute='age',
+                                                   position_attribute='position',
+                                                   k_factor_attribute='K'):
+        if self.df_population.nb_rows == 0:
+            return
+
+        check_col_exists_good_type(self.df_population, position_attribute, 'position_attribute', 'int',
+                                   reject_none=True)
+        check_col_exists_good_type(self.graph.df_attributes, k_factor_attribute, 'k_factor_attribute', 'float',
+                                   reject_none=True)
+
+        # we check that the 2 first arrays are 1D float array
+        check_input_array(array_death_proba_female, 'array_death_proba_female', 'float', nb_dim=1)
+        check_input_array(array_death_proba_male, 'array_death_proba_male', 'float', nb_dim=1)
+
+        # we need to check that there is no animal whose age is bigger than the size of the prob_arrays.
+        # in order to do so, we need to check that age_attribute and gender_attribute are properly used.
+        check_col_exists_good_type(self.df_population, age_attribute, 'age_attribute',
+                                   prefix_dtype='int', reject_none=True)
+
+        # now the gender attribute
+        check_col_exists_good_type(self.df_population, gender_attribute, 'gender_attribute',
+                                   prefix_dtype='int', reject_none=True)
+        check_if_gender_array(self.df_population[gender_attribute])
+
+        # now we check that there are no animal too old.
+        max_female = self.df_population[age_attribute][self.df_population[gender_attribute] == 1].max()
+        if max_female >= array_death_proba_female.shape[0]:
+            raise ValueError("There is a female agent of age " + str(max_female) + " while the array "
+                             "array_death_proba_female covers only ages until " +
+                             str(array_death_proba_female.shape[0] - 1) + ".")
+
+        max_male = self.df_population[age_attribute][self.df_population[gender_attribute] == 0].max()
+        if max_male >= array_death_proba_male.shape[0]:
+            raise ValueError("There is a male agent of age " + str(max_male) + " while the array "
+                             "array_death_proba_male covers only ages until " +
+                             str(array_death_proba_male.shape[0] - 1) + ".")
+
+        if permutation_shuffle is not None:
+            if not shuffle:
+                raise ValueError("A value for permutation_shuffle has been provided while shuffle is deactivated.")
+            check_input_is_permutation(permutation_shuffle, 'permutation_shuffle', length=self.df_population.nb_rows)
+
+        if condition is not None:
+            check_input_array(condition, 'condition', 'bool', shape=(self.df_population.nb_rows,))
+
+        if condition_count is not None:
+            check_input_array(condition_count, 'condition_count', 'bool', shape=(self.df_population.nb_rows,))
+
+    def natural_death_orm_methodology(self, array_death_proba_male, array_death_proba_female,
+                                      bias=0.,
+                                      shuffle=True,
+                                      permutation_shuffle=None,
+                                      condition=None,
+                                      condition_count=None,
+                                      gender_attribute='gender',
+                                      age_attribute='age',
+                                      position_attribute='position',
+                                      k_factor_attribute='K',
+                                      return_death_dataframe=False
+                                      ):
+        """
+        Kill agents using ORM methodology. I.E. the probability for a given agent to die is given by the formula:
+
+                            'prob_death * ( bias + (nb_agents_on_cell / K_cell) )'
+
+        Where prob_death is a parameter depending on the age of the agent, nb_agents_on_cell is the number of agent on
+        the cell of the tested agent (this number is updated along the process), and K is the K parameter of the current
+        cell. This method takes the gender into account.
+
+        The user can shuffle the dataframe before applying this function using the kwarg 'shuffle', and supply a
+        permutation to be used for the shuffling using the kwarg 'permutation_shuffle'. The user can also
+        specify two conditions as 1D boolean arrays:
+
+            - condition: array telling which agents are susceptible to be killed
+            - condition_count: array telling which agents are counted to determine the number of agents in each cell.
+                               This is useful if, for instance, the user wants to exclude juveniles from the
+                               nb_agents_on_cell used in the above formula.
+
+        WARNING: if shuffle is used, then any data previously extracted using the row position of the agents in the
+                 DataFrame df_population will be irrelevant.
+
+        :param array_death_proba_male: 1D array of float where array_death_proba_male[i] is the proba of death of a
+                                       male agent whose age is 'i'.
+        :param array_death_proba_female: 1D array of float where array_death_proba_female[i] is the proba of death of a
+                                         female agent whose age is 'i'.
+        :param bias: optional, float, default 0. Hyperparameter used to configure the mortality. Represents a 'base
+                     mortality'.
+        :param shuffle: optional, boolean, default True.
+        :param permutation_shuffle: optional, 1D array of int, default None. Permutation used for the shuffle. If
+                                    shuffle is activated and no permutation is provided, then one is generated using
+                                    numpy.random.permutation
+        :param condition: optional, 1D array of bool, default None. Array telling which agent are susceptible to die.
+        :param condition_count: optional, 1D array of bool, default None. Array telling which agent are to be counted.
+        :param gender_attribute: optional, string, default 'gender'. Name of the column containing gender info.
+        :param age_attribute: optional, string, default 'age'. Name of the column containing age info.
+        :param position_attribute: optional, string, default 'position'. Name of the column containing position info.
+        :param k_factor_attribute: optional, string, default 'K'. Name of the column containing K value in graph
+                                   df_attribute DataFrame.
+        :param return_death_dataframe: optional, boolean, default False. If True, returns a DataFrameXS containing all
+                                       the agents killed during this method call
+
+        :return: if return_death_dataframe is set to True, returns a DataFrameXS containing the agents killed during
+                 this method call.
+        """
+        if self.df_population.nb_rows == 0:
+            return
+        # shuffle the population dataframe if required
+        if shuffle:
+            used_permutation = self.df_population.scramble(permutation=permutation_shuffle, return_permutation=True)
+            if condition is not None:
+                condition = condition[used_permutation]
+            if condition_count is not None:
+                condition_count = condition_count[used_permutation]
+
+        # count agents per cell
+        count_arr = self.count_pop_per_vertex(position_attribute=position_attribute, condition=condition_count)
+        if condition is None:
+            if condition_count is None:
+                arr_survive = mortality_natural_death_orm_methodology(bias,
+                                                                      np.random.uniform(0, 1,
+                                                                                        self.df_population.nb_rows),
+                                                                      array_death_proba_male,
+                                                                      array_death_proba_female, count_arr,
+                                                                      self.df_population[position_attribute],
+                                                                      self.graph.df_attributes[k_factor_attribute],
+                                                                      self.df_population[age_attribute],
+                                                                      self.df_population[gender_attribute])
+            else:
+                arr_survive = mortality_natural_death_orm_methodology_condition_count(
+                                                                bias,
+                                                                np.random.uniform(0, 1, self.df_population.nb_rows),
+                                                                array_death_proba_male,
+                                                                array_death_proba_female, count_arr,
+                                                                condition_count,
+                                                                self.df_population[position_attribute],
+                                                                self.graph.df_attributes[k_factor_attribute],
+                                                                self.df_population[age_attribute],
+                                                                self.df_population[gender_attribute])
+        else:
+            if condition_count is None:
+                arr_survive = mortality_natural_death_orm_methodology_condition_death(
+                                                                bias,
+                                                                np.random.uniform(0, 1, self.df_population.nb_rows),
+                                                                array_death_proba_male,
+                                                                array_death_proba_female, count_arr,
+                                                                condition,
+                                                                self.df_population[position_attribute],
+                                                                self.graph.df_attributes[k_factor_attribute],
+                                                                self.df_population[age_attribute],
+                                                                self.df_population[gender_attribute])
+            else:
+                arr_survive = mortality_natural_death_orm_methodology_both_cond(
+                                                                bias,
+                                                                np.random.uniform(0, 1, self.df_population.nb_rows),
+                                                                array_death_proba_male,
+                                                                array_death_proba_female, count_arr,
+                                                                condition, condition_count,
+                                                                self.df_population[position_attribute],
+                                                                self.graph.df_attributes[k_factor_attribute],
+                                                                self.df_population[age_attribute],
+                                                                self.df_population[gender_attribute])
+
+        if return_death_dataframe:
+            death_df = self.df_population[~arr_survive]
+            self.df_population = self.df_population[arr_survive]
+            return death_df
+        else:
+            self.df_population = self.df_population[arr_survive]
+
+    def kill_too_old(self, limit_age, age_attribute='age'):
+        """
+        Kill agents whose age is greater or equal to the specified limit age.
+
+        :param limit_age: integer. Any agent older than this parameter will be killed.
+        :param age_attribute: optional, string, default 'age'. Name of the age attribute in the population dataframe.
+        """
+        self.df_population = self.df_population[self.df_population[age_attribute] < limit_age]
+
+
+class OffspringDependantOnParents:
+    """
+    This class add the possibility to kill the dependent offsprings whose mother is dead.
+    """
+    def __init__(self, **kwargs):
+        pass
+
+    def _sampy_debug_kill_children_whose_mother_is_dead(self, age_limit,
+                                                        id_attribute='col_id',
+                                                        age_attribute='age',
+                                                        mother_id_attribute='mom_id'):
+        if self.df_population.nb_rows == 0:
+            return
+        check_col_exists_good_type(self.df_population, age_attribute, 'age_attribute', prefix_dtype='int',
+                                   reject_none=True)
+        check_col_exists_good_type(self.df_population, mother_id_attribute, 'mother_id_attribute', prefix_dtype='int',
+                                   reject_none=True)
+
+    def kill_children_whose_mother_is_dead(self, age_limit,
+                                           id_attribute='col_id',
+                                           age_attribute='age',
+                                           mother_id_attribute='mom_id'):
+        """
+        Kill the agents that are not independent yet and whose mother is dead. Note that an agent whose age is precisely
+        age_limit is not considered independent.
+
+        :param age_limit: integer. Age of independence.
+        :param id_attribute: optional, string, default 'col_id'
+        :param age_attribute: optional, string, default 'age'
+        :param mother_id_attribute: optional, string, default 'mom_id'
+        """
+        if self.df_population.nb_rows == 0:
+            return
+        young = self.df_population[age_attribute] <= age_limit
+        has_mom = self.df_population.check_arr_in_col(self.df_population[mother_id_attribute], id_attribute,
+                                                      condition=young)
+        too_old = np.array(self.df_population[age_attribute] > age_limit)
+        self.df_population = self.df_population[has_mom | too_old]
+
+
+class KillPercentagePop:
+    """
+    This class adds the possibility to kill a given percentage of the population.
+    """
+    def __init__(self, **kwargs):
+        pass
+
+    def _sampy_debug_kill_proportion_of_population(self, proportion, condition=None):
+        if condition is not None:
+            check_input_array(condition, 'condition', 'bool', shape=(self.df_population.nb_rows,))
+
+    def kill_proportion_of_population(self, proportion, condition=None):
+        """
+        For each agent, a random uniform number between 0 and 1 is sampled, and each agent for which this number is
+        smaller than the argument 'proportion' is killed. Note that the user can use the kwarg 'condition' to
+        exclude some agents from this test.
+
+        :param proportion: float between 0 and 1.
+        :param condition: optional, 1D array of bool, default None.
+        """
+        rand = np.random.uniform(0, 1, (self.df_population.nb_rows,)) > proportion
+        if condition is not None:
+            rand = rand & condition
+        self.df_population = self.df_population[rand]
```

### Comparing `sampy-abm-1.0.2/src/sampy/agent/movement.py` & `sampy_abm-1.0.3/src/sampy/agent/movement.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,341 +1,341 @@
-import numpy as np
-from .jit_compiled_functions import *
-from ..pandas_xs.pandas_xs import DataFrameXS
-from ..utils.errors_shortcut import (check_col_exists_good_type,
-                                     check_input_array)
-
-
-class TerritorialMovementWithoutResistance:
-    """
-    Add graph based movements abilities to the agents. Agents have both a territory and a position, which can be
-    different. Generally, the position of an agent will be either its territory vertex, or a vertex neighbouring its
-    territory.
-
-    Note that both position and territory are stored as integers, i.e. using the vertices indices which generally
-    differ from their id. If needed, conversion should be performed by the user using the graph attribute
-    'dict_cell_id_to_ind'. Equivalently, the user may extract a table giving the correspondence between id and indexes
-    using the graph method 'save_table_id_of_vertices_to_indices'.
-    """
-    def __init__(self, **kwargs):
-        if not hasattr(self, 'df_population'):
-            self.df_population = DataFrameXS()
-
-        self.df_population['territory'] = None
-        self.df_population['position'] = None
-
-    def _sampy_debug_change_territory(self,
-                                      condition=None,
-                                      territory_attribute='territory',
-                                      position_attribute='position'):
-        if self.df_population.nb_rows == 0:
-            return
-        if condition is not None:
-            if (not isinstance(condition, np.ndarray)) or \
-                    (condition.shape != (self.df_population.nb_rows,)) or \
-                    (not str(condition.dtype).startswith('bool')):
-                raise ValueError("if used, condition argument should be a 1D array of bool of same length as the number"
-                                 " of individuals.")
-
-        check_col_exists_good_type(self.df_population, territory_attribute, prefix_dtype='int')
-        check_col_exists_good_type(self.df_population, position_attribute, prefix_dtype='int')
-
-    def change_territory(self,
-                         condition=None,
-                         territory_attribute='territory',
-                         position_attribute='position'):
-        """
-        Change the territory and the position of the agents. If an agent is on an isolated vertex (a vertex without
-        any neighbour), then the agent stays on the vertex.
-
-        :param condition: optional, array of bool, default None. If not None, array telling which
-        :param territory_attribute: optional, string, default 'territory'
-        :param position_attribute: optional, string, default 'position'
-        """
-        if self.df_population.nb_rows == 0:
-            return
-        if condition is not None:
-            rand = np.random.uniform(0, 1, (condition.sum(),))
-            movement_change_territory_and_position_condition(self.df_population[territory_attribute],
-                                                             self.df_population[position_attribute],
-                                                             condition, rand,
-                                                             self.graph.connections, self.graph.weights)
-        else:
-            rand = np.random.uniform(0, 1, (self.df_population.shape[0],))
-            movement_change_territory_and_position(self.df_population[territory_attribute],
-                                                   self.df_population[position_attribute],
-                                                   rand, self.graph.connections, self.graph.weights)
-
-    def _sampy_debug_mov_around_territory(self,
-                                          proba_remain_on_territory,
-                                          condition=None,
-                                          territory_attribute='territory',
-                                          position_attribute='position'):
-        if self.df_population.nb_rows == 0:
-            return
-        if condition is not None:
-            check_input_array(condition, 'condition', 'bool', shape=(self.df_population.nb_rows,))
-        check_col_exists_good_type(self.df_population, territory_attribute, 'territory_attribute', prefix_dtype='int',
-                                   reject_none=True)
-        check_col_exists_good_type(self.df_population, position_attribute, 'position_attribute', prefix_dtype='int',
-                                   reject_none=True)
-
-    def mov_around_territory(self,
-                             proba_remain_on_territory,
-                             condition=None,
-                             territory_attribute='territory',
-                             position_attribute='position'):
-        """
-        Update the average position of the agent around its territory during the current time step.
-
-        :param proba_remain_on_territory: float, probability to stay on the territory
-        :param condition: optional, array of bool, default None. Array of boolean such that the i-th value is
-                          True if and only if the i-th agent (i.e. the agent at the line i of df_population) can
-                          move.
-        :param territory_attribute: optional, string, default 'territory'
-        :param position_attribute: optional, string, default 'position'
-        """
-        if self.df_population.nb_rows == 0:
-            return
-        if condition is not None:
-            pre_bool_mov = np.random.uniform(0, 1, condition.sum()) > proba_remain_on_territory
-            bool_mov = movement_mov_around_territory_fill_bool_mov_using_condition(pre_bool_mov, condition)
-        else:
-            bool_mov = np.random.uniform(0, 1, self.df_population.shape[0]) > proba_remain_on_territory
-        rand = np.random.uniform(0, 1, bool_mov.sum())
-        movement_mov_around_territory(self.df_population[territory_attribute], self.df_population[position_attribute],
-                                      bool_mov, rand, self.graph.connections, self.graph.weights)
-
-    def _sampy_debug_dispersion_with_varying_nb_of_steps(self, arr_nb_steps, arr_prob,
-                                                         condition=None,
-                                                         territory_attribute='territory',
-                                                         position_attribute='position'
-                                                         ):
-        if self.df_population.nb_rows == 0:
-            return
-
-        check_input_array(arr_nb_steps, 'arr_nb_steps', 'int', nb_dim=1)
-        check_input_array(arr_prob, 'arr_prob', 'float', nb_dim=1)
-
-        if arr_prob.shape != arr_nb_steps.shape:
-            raise ValueError("Arguments 'arr_nb_steps' and 'arr_prob' have different shapes.")
-
-        if condition is not None:
-            check_input_array(condition, 'condition', 'bool', shape=(self.df_population.nb_rows,))
-
-        check_col_exists_good_type(self.df_population, territory_attribute, 'territory_attribute', prefix_dtype='int',
-                                   reject_none=True)
-        check_col_exists_good_type(self.df_population, position_attribute, 'position_attribute', prefix_dtype='int',
-                                   reject_none=True)
-
-    def dispersion_with_varying_nb_of_steps(self, arr_nb_steps, arr_prob,
-                                            condition=None,
-                                            territory_attribute='territory',
-                                            position_attribute='position'
-                                            ):
-        """
-        Used to modelize dispersion of agents. Each selected agent will perform a random number of discrete steps on
-        the graph. The number of steps is determined using the user inputs 'arr_nb_steps' and 'arr_prob'. Both
-        position and territory are updated.
-
-        :param arr_nb_steps: 1D array of int, giving the permissible number of steps.
-        :param arr_prob: 1D array of float, arr_prob[i] is the probability that a given agent will perform
-                         arr_nb_steps[i] steps.
-        :param condition: optional, array of bool, default None. Array of boolean such that the i-th value is
-                          True if and only if the i-th agent (i.e. the agent at the line i of df_population) can
-                          move. If left at None, all the agents move.
-        :param territory_attribute: optional, string, default 'territory'.
-        :param position_attribute: optional, string, default 'position'.
-        """
-        if self.df_population.nb_rows == 0:
-            return
-        prob = arr_prob.astype('float64')
-        prob = prob / prob.sum()
-        if condition is not None:
-            # get number of steps
-            arr_nb_steps = np.random.choice(arr_nb_steps, condition.sum(), p=prob)
-        else:
-            arr_nb_steps = np.random.choice(arr_nb_steps, self.df_population.nb_rows, p=prob)
-        rand = np.random.uniform(0, 1, arr_nb_steps.sum())
-        if condition is None:
-            movement_dispersion_with_varying_nb_of_steps(self.df_population[territory_attribute],
-                                                         self.df_population[position_attribute],
-                                                         rand, arr_nb_steps, self.graph.connections, self.graph.weights)
-        else:
-            movement_dispersion_with_varying_nb_of_steps_condition(self.df_population[territory_attribute],
-                                                                   self.df_population[position_attribute],
-                                                                   condition,
-                                                                   rand, arr_nb_steps, self.graph.connections,
-                                                                   self.graph.weights)
-
-
-class TerritorialMovementWithResistance:
-    """
-    Add graph based movements abilities to the agents. Agents have both a territory and a position, which can be
-    different. Generally, the position of an agent will be either its territory vertex, or a vertex neighbouring its
-    territory. Here each connection in the graph is assumed to come with probability saying how likely a movement on
-    that connection is to fail.
-
-    Note that both position and territory are stored as integers, i.e. using the vertices indices which generally
-    differ from their id. If needed, conversion should be performed by the user using the graph attribute
-    'dict_cell_id_to_ind'. Equivalently, the user may extract a table giving the correspondence between id and indexes
-    using the graph method 'save_table_id_of_vertices_to_indices'.
-    """
-    def __init__(self, **kwargs):
-        if not hasattr(self, 'df_population'):
-            self.df_population = DataFrameXS()
-
-        self.df_population['territory'] = None
-        self.df_population['position'] = None
-
-    def _sampy_debug_change_territory_with_resistance(self,
-                                                      resistance_array,
-                                                      condition=None,
-                                                      territory_attribute='territory',
-                                                      position_attribute='position'):
-        if self.df_population.nb_rows == 0:
-            return
-        if (not isinstance(resistance_array, np.ndarray) or \
-                resistance_array.shape != self.graph.connections.shape or \
-                (not str(resistance_array.dtype).startswith('float'))):
-            raise ValueError("The resistance array should be a 2 dimensional array of floats of shape " +
-                             str(resistance_array.shape))
-        if condition is not None:
-            if (not isinstance(condition, np.ndarray)) or \
-                    (condition.shape != (self.df_population.nb_rows,)) or \
-                    (not str(condition.dtype).startswith('bool')):
-                raise ValueError("if used, condition argument should be a 1D array of bool of same length as the number"
-                                 " of individuals.")
-
-        check_col_exists_good_type(self.df_population, territory_attribute, prefix_dtype='int')
-        check_col_exists_good_type(self.df_population, position_attribute, prefix_dtype='int')
-
-    def change_territory_with_resistance(self,
-                                         resistance_array,
-                                         condition=None,
-                                         territory_attribute='territory',
-                                         position_attribute='position'):
-        """
-        Change the territory and the position of the agents. If an agent is on an isolated vertex (a vertex without
-        any neighbour), then the agent stays on the vertex.
-
-        :param resistance_array: 2d array of float, array of same shape as the connections of the graph, gives the
-                                 'resistance to movement' of each connection
-        :param condition: optional, array of bool, default None. If not None, array telling which
-        :param territory_attribute: optional, string, default 'territory'
-        :param position_attribute: optional, string, default 'position'
-        """
-        if self.df_population.nb_rows == 0:
-            return
-        if condition is not None:
-            rand = np.random.uniform(0, 1, (condition.sum(),))
-            movement_change_territory_and_position_condition(self.df_population[territory_attribute],
-                                                             self.df_population[position_attribute],
-                                                             condition, rand,
-                                                             self.graph.connections, self.graph.weights)
-        else:
-            rand = np.random.uniform(0, 1, (self.df_population.shape[0],))
-            movement_change_territory_and_position(self.df_population[territory_attribute],
-                                                   self.df_population[position_attribute],
-                                                   rand, self.graph.connections, self.graph.weights)
-
-    def _sampy_debug_mov_around_territory(self,
-                                          proba_remain_on_territory,
-                                          condition=None,
-                                          territory_attribute='territory',
-                                          position_attribute='position'):
-        if self.df_population.nb_rows == 0:
-            return
-        if condition is not None:
-            check_input_array(condition, 'condition', 'bool', shape=(self.df_population.nb_rows,))
-        check_col_exists_good_type(self.df_population, territory_attribute, 'territory_attribute', prefix_dtype='int',
-                                   reject_none=True)
-        check_col_exists_good_type(self.df_population, position_attribute, 'position_attribute', prefix_dtype='int',
-                                   reject_none=True)
-
-    def mov_around_territory(self,
-                             proba_remain_on_territory,
-                             condition=None,
-                             territory_attribute='territory',
-                             position_attribute='position'):
-        """
-        Update the average position of the agent around its territory during the current time step.
-
-        :param proba_remain_on_territory: float, probability to stay on the territory
-        :param condition: optional, array of bool, default None. Array of boolean such that the i-th value is
-                          True if and only if the i-th agent (i.e. the agent at the line i of df_population) can
-                          move.
-        :param territory_attribute: optional, string, default 'territory'
-        :param position_attribute: optional, string, default 'position'
-        """
-        if self.df_population.nb_rows == 0:
-            return
-        if condition is not None:
-            pre_bool_mov = np.random.uniform(0, 1, condition.sum()) > proba_remain_on_territory
-            bool_mov = movement_mov_around_territory_fill_bool_mov_using_condition(pre_bool_mov, condition)
-        else:
-            bool_mov = np.random.uniform(0, 1, self.df_population.shape[0]) > proba_remain_on_territory
-        rand = np.random.uniform(0, 1, bool_mov.sum())
-        movement_mov_around_territory(self.df_population[territory_attribute], self.df_population[position_attribute],
-                                      bool_mov, rand, self.graph.connections, self.graph.weights)
-
-    def _sampy_debug_dispersion_with_varying_nb_of_steps(self, arr_nb_steps, arr_prob,
-                                                         condition=None,
-                                                         territory_attribute='territory',
-                                                         position_attribute='position'
-                                                         ):
-        if self.df_population.nb_rows == 0:
-            return
-
-        check_input_array(arr_nb_steps, 'arr_nb_steps', 'int', nb_dim=1)
-        check_input_array(arr_prob, 'arr_prob', 'float', nb_dim=1)
-
-        if arr_prob.shape != arr_nb_steps.shape:
-            raise ValueError("Arguments 'arr_nb_steps' and 'arr_prob' have different shapes.")
-
-        if condition is not None:
-            check_input_array(condition, 'condition', 'bool', shape=(self.df_population.nb_rows,))
-
-        check_col_exists_good_type(self.df_population, territory_attribute, 'territory_attribute', prefix_dtype='int',
-                                   reject_none=True)
-        check_col_exists_good_type(self.df_population, position_attribute, 'position_attribute', prefix_dtype='int',
-                                   reject_none=True)
-
-    def dispersion_with_varying_nb_of_steps(self, arr_nb_steps, arr_prob,
-                                            condition=None,
-                                            territory_attribute='territory',
-                                            position_attribute='position'
-                                            ):
-        """
-        Used to modelize dispersion of agents. Each selected agent will perform a random number of discrete steps on
-        the graph. The number of steps is determined using the user inputs 'arr_nb_steps' and 'arr_prob'. Both
-        position and territory are updated.
-
-        :param arr_nb_steps: 1D array of int, giving the permissible number of steps.
-        :param arr_prob: 1D array of float, arr_prob[i] is the probability that a given agent will perform
-                         arr_nb_steps[i] steps.
-        :param condition: optional, array of bool, default None. Array of boolean such that the i-th value is
-                          True if and only if the i-th agent (i.e. the agent at the line i of df_population) can
-                          move. If left at None, all the agents move.
-        :param territory_attribute: optional, string, default 'territory'.
-        :param position_attribute: optional, string, default 'position'.
-        """
-        if self.df_population.nb_rows == 0:
-            return
-        prob = arr_prob.astype('float64')
-        prob = prob / prob.sum()
-        if condition is not None:
-            # get number of steps
-            arr_nb_steps = np.random.choice(arr_nb_steps, condition.sum(), p=prob)
-        else:
-            arr_nb_steps = np.random.choice(arr_nb_steps, self.df_population.nb_rows, p=prob)
-        rand = np.random.uniform(0, 1, arr_nb_steps.sum())
-        if condition is None:
-            movement_dispersion_with_varying_nb_of_steps(self.df_population[territory_attribute],
-                                                         self.df_population[position_attribute],
-                                                         rand, arr_nb_steps, self.graph.connections, self.graph.weights)
-        else:
-            movement_dispersion_with_varying_nb_of_steps_condition(self.df_population[territory_attribute],
-                                                                   self.df_population[position_attribute],
-                                                                   condition,
-                                                                   rand, arr_nb_steps, self.graph.connections,
-                                                                   self.graph.weights)
+import numpy as np
+from .jit_compiled_functions import *
+from ..pandas_xs.pandas_xs import DataFrameXS
+from ..utils.errors_shortcut import (check_col_exists_good_type,
+                                     check_input_array)
+
+
+class TerritorialMovementWithoutResistance:
+    """
+    Add graph based movements abilities to the agents. Agents have both a territory and a position, which can be
+    different. Generally, the position of an agent will be either its territory vertex, or a vertex neighbouring its
+    territory.
+
+    Note that both position and territory are stored as integers, i.e. using the vertices indices which generally
+    differ from their id. If needed, conversion should be performed by the user using the graph attribute
+    'dict_cell_id_to_ind'. Equivalently, the user may extract a table giving the correspondence between id and indexes
+    using the graph method 'save_table_id_of_vertices_to_indices'.
+    """
+    def __init__(self, **kwargs):
+        if not hasattr(self, 'df_population'):
+            self.df_population = DataFrameXS()
+
+        self.df_population['territory'] = None
+        self.df_population['position'] = None
+
+    def _sampy_debug_change_territory(self,
+                                      condition=None,
+                                      territory_attribute='territory',
+                                      position_attribute='position'):
+        if self.df_population.nb_rows == 0:
+            return
+        if condition is not None:
+            if (not isinstance(condition, np.ndarray)) or \
+                    (condition.shape != (self.df_population.nb_rows,)) or \
+                    (not str(condition.dtype).startswith('bool')):
+                raise ValueError("if used, condition argument should be a 1D array of bool of same length as the number"
+                                 " of individuals.")
+
+        check_col_exists_good_type(self.df_population, territory_attribute, prefix_dtype='int')
+        check_col_exists_good_type(self.df_population, position_attribute, prefix_dtype='int')
+
+    def change_territory(self,
+                         condition=None,
+                         territory_attribute='territory',
+                         position_attribute='position'):
+        """
+        Change the territory and the position of the agents. If an agent is on an isolated vertex (a vertex without
+        any neighbour), then the agent stays on the vertex.
+
+        :param condition: optional, array of bool, default None. If not None, array telling which
+        :param territory_attribute: optional, string, default 'territory'
+        :param position_attribute: optional, string, default 'position'
+        """
+        if self.df_population.nb_rows == 0:
+            return
+        if condition is not None:
+            rand = np.random.uniform(0, 1, (condition.sum(),))
+            movement_change_territory_and_position_condition(self.df_population[territory_attribute],
+                                                             self.df_population[position_attribute],
+                                                             condition, rand,
+                                                             self.graph.connections, self.graph.weights)
+        else:
+            rand = np.random.uniform(0, 1, (self.df_population.shape[0],))
+            movement_change_territory_and_position(self.df_population[territory_attribute],
+                                                   self.df_population[position_attribute],
+                                                   rand, self.graph.connections, self.graph.weights)
+
+    def _sampy_debug_mov_around_territory(self,
+                                          proba_remain_on_territory,
+                                          condition=None,
+                                          territory_attribute='territory',
+                                          position_attribute='position'):
+        if self.df_population.nb_rows == 0:
+            return
+        if condition is not None:
+            check_input_array(condition, 'condition', 'bool', shape=(self.df_population.nb_rows,))
+        check_col_exists_good_type(self.df_population, territory_attribute, 'territory_attribute', prefix_dtype='int',
+                                   reject_none=True)
+        check_col_exists_good_type(self.df_population, position_attribute, 'position_attribute', prefix_dtype='int',
+                                   reject_none=True)
+
+    def mov_around_territory(self,
+                             proba_remain_on_territory,
+                             condition=None,
+                             territory_attribute='territory',
+                             position_attribute='position'):
+        """
+        Update the average position of the agent around its territory during the current time step.
+
+        :param proba_remain_on_territory: float, probability to stay on the territory
+        :param condition: optional, array of bool, default None. Array of boolean such that the i-th value is
+                          True if and only if the i-th agent (i.e. the agent at the line i of df_population) can
+                          move.
+        :param territory_attribute: optional, string, default 'territory'
+        :param position_attribute: optional, string, default 'position'
+        """
+        if self.df_population.nb_rows == 0:
+            return
+        if condition is not None:
+            pre_bool_mov = np.random.uniform(0, 1, condition.sum()) > proba_remain_on_territory
+            bool_mov = movement_mov_around_territory_fill_bool_mov_using_condition(pre_bool_mov, condition)
+        else:
+            bool_mov = np.random.uniform(0, 1, self.df_population.shape[0]) > proba_remain_on_territory
+        rand = np.random.uniform(0, 1, bool_mov.sum())
+        movement_mov_around_territory(self.df_population[territory_attribute], self.df_population[position_attribute],
+                                      bool_mov, rand, self.graph.connections, self.graph.weights)
+
+    def _sampy_debug_dispersion_with_varying_nb_of_steps(self, arr_nb_steps, arr_prob,
+                                                         condition=None,
+                                                         territory_attribute='territory',
+                                                         position_attribute='position'
+                                                         ):
+        if self.df_population.nb_rows == 0:
+            return
+
+        check_input_array(arr_nb_steps, 'arr_nb_steps', 'int', nb_dim=1)
+        check_input_array(arr_prob, 'arr_prob', 'float', nb_dim=1)
+
+        if arr_prob.shape != arr_nb_steps.shape:
+            raise ValueError("Arguments 'arr_nb_steps' and 'arr_prob' have different shapes.")
+
+        if condition is not None:
+            check_input_array(condition, 'condition', 'bool', shape=(self.df_population.nb_rows,))
+
+        check_col_exists_good_type(self.df_population, territory_attribute, 'territory_attribute', prefix_dtype='int',
+                                   reject_none=True)
+        check_col_exists_good_type(self.df_population, position_attribute, 'position_attribute', prefix_dtype='int',
+                                   reject_none=True)
+
+    def dispersion_with_varying_nb_of_steps(self, arr_nb_steps, arr_prob,
+                                            condition=None,
+                                            territory_attribute='territory',
+                                            position_attribute='position'
+                                            ):
+        """
+        Used to modelize dispersion of agents. Each selected agent will perform a random number of discrete steps on
+        the graph. The number of steps is determined using the user inputs 'arr_nb_steps' and 'arr_prob'. Both
+        position and territory are updated.
+
+        :param arr_nb_steps: 1D array of int, giving the permissible number of steps.
+        :param arr_prob: 1D array of float, arr_prob[i] is the probability that a given agent will perform
+                         arr_nb_steps[i] steps.
+        :param condition: optional, array of bool, default None. Array of boolean such that the i-th value is
+                          True if and only if the i-th agent (i.e. the agent at the line i of df_population) can
+                          move. If left at None, all the agents move.
+        :param territory_attribute: optional, string, default 'territory'.
+        :param position_attribute: optional, string, default 'position'.
+        """
+        if self.df_population.nb_rows == 0:
+            return
+        prob = arr_prob.astype('float64')
+        prob = prob / prob.sum()
+        if condition is not None:
+            # get number of steps
+            arr_nb_steps = np.random.choice(arr_nb_steps, condition.sum(), p=prob)
+        else:
+            arr_nb_steps = np.random.choice(arr_nb_steps, self.df_population.nb_rows, p=prob)
+        rand = np.random.uniform(0, 1, arr_nb_steps.sum())
+        if condition is None:
+            movement_dispersion_with_varying_nb_of_steps(self.df_population[territory_attribute],
+                                                         self.df_population[position_attribute],
+                                                         rand, arr_nb_steps, self.graph.connections, self.graph.weights)
+        else:
+            movement_dispersion_with_varying_nb_of_steps_condition(self.df_population[territory_attribute],
+                                                                   self.df_population[position_attribute],
+                                                                   condition,
+                                                                   rand, arr_nb_steps, self.graph.connections,
+                                                                   self.graph.weights)
+
+
+class TerritorialMovementWithResistance:
+    """
+    Add graph based movements abilities to the agents. Agents have both a territory and a position, which can be
+    different. Generally, the position of an agent will be either its territory vertex, or a vertex neighbouring its
+    territory. Here each connection in the graph is assumed to come with probability saying how likely a movement on
+    that connection is to fail.
+
+    Note that both position and territory are stored as integers, i.e. using the vertices indices which generally
+    differ from their id. If needed, conversion should be performed by the user using the graph attribute
+    'dict_cell_id_to_ind'. Equivalently, the user may extract a table giving the correspondence between id and indexes
+    using the graph method 'save_table_id_of_vertices_to_indices'.
+    """
+    def __init__(self, **kwargs):
+        if not hasattr(self, 'df_population'):
+            self.df_population = DataFrameXS()
+
+        self.df_population['territory'] = None
+        self.df_population['position'] = None
+
+    def _sampy_debug_change_territory_with_resistance(self,
+                                                      resistance_array,
+                                                      condition=None,
+                                                      territory_attribute='territory',
+                                                      position_attribute='position'):
+        if self.df_population.nb_rows == 0:
+            return
+        if (not isinstance(resistance_array, np.ndarray) or \
+                resistance_array.shape != self.graph.connections.shape or \
+                (not str(resistance_array.dtype).startswith('float'))):
+            raise ValueError("The resistance array should be a 2 dimensional array of floats of shape " +
+                             str(resistance_array.shape))
+        if condition is not None:
+            if (not isinstance(condition, np.ndarray)) or \
+                    (condition.shape != (self.df_population.nb_rows,)) or \
+                    (not str(condition.dtype).startswith('bool')):
+                raise ValueError("if used, condition argument should be a 1D array of bool of same length as the number"
+                                 " of individuals.")
+
+        check_col_exists_good_type(self.df_population, territory_attribute, prefix_dtype='int')
+        check_col_exists_good_type(self.df_population, position_attribute, prefix_dtype='int')
+
+    def change_territory_with_resistance(self,
+                                         resistance_array,
+                                         condition=None,
+                                         territory_attribute='territory',
+                                         position_attribute='position'):
+        """
+        Change the territory and the position of the agents. If an agent is on an isolated vertex (a vertex without
+        any neighbour), then the agent stays on the vertex.
+
+        :param resistance_array: 2d array of float, array of same shape as the connections of the graph, gives the
+                                 'resistance to movement' of each connection
+        :param condition: optional, array of bool, default None. If not None, array telling which
+        :param territory_attribute: optional, string, default 'territory'
+        :param position_attribute: optional, string, default 'position'
+        """
+        if self.df_population.nb_rows == 0:
+            return
+        if condition is not None:
+            rand = np.random.uniform(0, 1, (condition.sum(),))
+            movement_change_territory_and_position_condition(self.df_population[territory_attribute],
+                                                             self.df_population[position_attribute],
+                                                             condition, rand,
+                                                             self.graph.connections, self.graph.weights)
+        else:
+            rand = np.random.uniform(0, 1, (self.df_population.shape[0],))
+            movement_change_territory_and_position(self.df_population[territory_attribute],
+                                                   self.df_population[position_attribute],
+                                                   rand, self.graph.connections, self.graph.weights)
+
+    def _sampy_debug_mov_around_territory(self,
+                                          proba_remain_on_territory,
+                                          condition=None,
+                                          territory_attribute='territory',
+                                          position_attribute='position'):
+        if self.df_population.nb_rows == 0:
+            return
+        if condition is not None:
+            check_input_array(condition, 'condition', 'bool', shape=(self.df_population.nb_rows,))
+        check_col_exists_good_type(self.df_population, territory_attribute, 'territory_attribute', prefix_dtype='int',
+                                   reject_none=True)
+        check_col_exists_good_type(self.df_population, position_attribute, 'position_attribute', prefix_dtype='int',
+                                   reject_none=True)
+
+    def mov_around_territory(self,
+                             proba_remain_on_territory,
+                             condition=None,
+                             territory_attribute='territory',
+                             position_attribute='position'):
+        """
+        Update the average position of the agent around its territory during the current time step.
+
+        :param proba_remain_on_territory: float, probability to stay on the territory
+        :param condition: optional, array of bool, default None. Array of boolean such that the i-th value is
+                          True if and only if the i-th agent (i.e. the agent at the line i of df_population) can
+                          move.
+        :param territory_attribute: optional, string, default 'territory'
+        :param position_attribute: optional, string, default 'position'
+        """
+        if self.df_population.nb_rows == 0:
+            return
+        if condition is not None:
+            pre_bool_mov = np.random.uniform(0, 1, condition.sum()) > proba_remain_on_territory
+            bool_mov = movement_mov_around_territory_fill_bool_mov_using_condition(pre_bool_mov, condition)
+        else:
+            bool_mov = np.random.uniform(0, 1, self.df_population.shape[0]) > proba_remain_on_territory
+        rand = np.random.uniform(0, 1, bool_mov.sum())
+        movement_mov_around_territory(self.df_population[territory_attribute], self.df_population[position_attribute],
+                                      bool_mov, rand, self.graph.connections, self.graph.weights)
+
+    def _sampy_debug_dispersion_with_varying_nb_of_steps(self, arr_nb_steps, arr_prob,
+                                                         condition=None,
+                                                         territory_attribute='territory',
+                                                         position_attribute='position'
+                                                         ):
+        if self.df_population.nb_rows == 0:
+            return
+
+        check_input_array(arr_nb_steps, 'arr_nb_steps', 'int', nb_dim=1)
+        check_input_array(arr_prob, 'arr_prob', 'float', nb_dim=1)
+
+        if arr_prob.shape != arr_nb_steps.shape:
+            raise ValueError("Arguments 'arr_nb_steps' and 'arr_prob' have different shapes.")
+
+        if condition is not None:
+            check_input_array(condition, 'condition', 'bool', shape=(self.df_population.nb_rows,))
+
+        check_col_exists_good_type(self.df_population, territory_attribute, 'territory_attribute', prefix_dtype='int',
+                                   reject_none=True)
+        check_col_exists_good_type(self.df_population, position_attribute, 'position_attribute', prefix_dtype='int',
+                                   reject_none=True)
+
+    def dispersion_with_varying_nb_of_steps(self, arr_nb_steps, arr_prob,
+                                            condition=None,
+                                            territory_attribute='territory',
+                                            position_attribute='position'
+                                            ):
+        """
+        Used to modelize dispersion of agents. Each selected agent will perform a random number of discrete steps on
+        the graph. The number of steps is determined using the user inputs 'arr_nb_steps' and 'arr_prob'. Both
+        position and territory are updated.
+
+        :param arr_nb_steps: 1D array of int, giving the permissible number of steps.
+        :param arr_prob: 1D array of float, arr_prob[i] is the probability that a given agent will perform
+                         arr_nb_steps[i] steps.
+        :param condition: optional, array of bool, default None. Array of boolean such that the i-th value is
+                          True if and only if the i-th agent (i.e. the agent at the line i of df_population) can
+                          move. If left at None, all the agents move.
+        :param territory_attribute: optional, string, default 'territory'.
+        :param position_attribute: optional, string, default 'position'.
+        """
+        if self.df_population.nb_rows == 0:
+            return
+        prob = arr_prob.astype('float64')
+        prob = prob / prob.sum()
+        if condition is not None:
+            # get number of steps
+            arr_nb_steps = np.random.choice(arr_nb_steps, condition.sum(), p=prob)
+        else:
+            arr_nb_steps = np.random.choice(arr_nb_steps, self.df_population.nb_rows, p=prob)
+        rand = np.random.uniform(0, 1, arr_nb_steps.sum())
+        if condition is None:
+            movement_dispersion_with_varying_nb_of_steps(self.df_population[territory_attribute],
+                                                         self.df_population[position_attribute],
+                                                         rand, arr_nb_steps, self.graph.connections, self.graph.weights)
+        else:
+            movement_dispersion_with_varying_nb_of_steps_condition(self.df_population[territory_attribute],
+                                                                   self.df_population[position_attribute],
+                                                                   condition,
+                                                                   rand, arr_nb_steps, self.graph.connections,
+                                                                   self.graph.weights)
```

### Comparing `sampy-abm-1.0.2/src/sampy/agent/random_walk.py` & `sampy_abm-1.0.3/src/sampy/agent/random_walk.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,322 +1,380 @@
-import numpy as np
-import pandas as pd
-import time
-
-from .jit_compiled_functions import (random_walk_on_sphere_set_position_based_on_graph,
-                                     random_walk_on_sphere_start_random_walk_uniform_prob,
-                                     random_walk_on_sphere_start_random_walk_uniform_prob_return_new_walkers,
-                                     conditional_random_walk_on_sphere_start_random_walk_uniform_prob,
-                                     conditional_random_walk_on_sphere_start_random_walk_uniform_prob_return_new_walkers,
-                                     random_walk_on_sphere_set_initial_dir_to_north,
-                                     random_walk_on_sphere_deviate_direction_from_angles,
-                                     random_walk_on_sphere_propose_step_gamma_law,
-                                     random_walk_on_sphere_make_step_gamma_law,
-                                     random_walk_on_sphere_validate_step,
-                                     random_walk_on_sphere_validate_step_return_fail,
-                                     _temp_random_walk_on_sphere_exit_random_walk_based_on_k)
-
-
-class SphericalRandomWalk:
-    """
-    This class give the ability for the agent to perform random walks on a sphere. The directions are preserved between
-    consecutive steps by using parallel transport. The associated technical background can be found in the publication
-    {in-preparation} by F. Viard, A. Allibert and P. Leighton.
-    """
-    def __init__(self, px=0., py=0., pz=0., dx=0., dy=0., dz=0., **kwargs):
-        self.df_population['is_on_random_walk'] = False
-        self.df_population['px'] = px
-        self.df_population['py'] = py
-        self.df_population['pz'] = pz
-        self.df_population['dx'] = dx
-        self.df_population['dy'] = dy
-        self.df_population['dz'] = dz
-
-        self.dict_default_values['is_on_random_walk'] = False
-        self.dict_default_values['px'] = px
-        self.dict_default_values['py'] = py
-        self.dict_default_values['pz'] = pz
-        self.dict_default_values['dx'] = dx
-        self.dict_default_values['dy'] = dy
-        self.dict_default_values['dz'] = dz
-
-    def set_dtype_of_positions_and_directions(self, targeted_dtype='float64'):
-        """
-        The computations needed for spherical random walks, as they are now, are really sensitive to rounding errors.
-        Therefore, it may be needed to increase the precision of columns px, py, pz, dx, dy and dz to float64. This
-        method is a shortcut for doing it on all 6 columns. This method won't have any effect if there is no agents.
-
-        :param targeted_dtype: optional, string, default 'float64'. The new datatype for the position and direction
-                               columns.
-
-        :return: True if the columns were not empty and the assignement succeded, False otherwise.
-        """
-        if self.df_population.is_empty:
-            return False
-
-        self.df_population.change_type('px', targeted_dtype)
-        self.df_population.change_type('py', targeted_dtype)
-        self.df_population.change_type('pz', targeted_dtype)
-        self.df_population.change_type('dx', targeted_dtype)
-        self.df_population.change_type('dy', targeted_dtype)
-        self.df_population.change_type('dz', targeted_dtype)
-
-        return True
-
-    def set_position_based_on_graph(self, arr_selected_agent,
-                                    agent_position_attribute='position',
-                                    graph_coord_x_attribute='coord_x',
-                                    graph_coord_y_attribute='coord_y',
-                                    graph_coord_z_attribute='coord_z'):
-        """
-        Set the position of the selected agents using coordinates of the graph vertex the agent is currently on.
-
-        :param arr_selected_agent: 1D array of bool, saying which agents should have their coordinates updated according
-                                   to their position on the graph.
-        :param agent_position_attribute: optional, string, default 'position'. Name of the attribute position column in
-                                         the df_population dataframe in the agent class.
-        :param graph_coord_x_attribute: optional, string, default 'coord_x'. X coordinate of the graph vertices.
-        :param graph_coord_y_attribute: optional, string, default 'coord_y'. Y coordinate of the graph vertices.
-        :param graph_coord_z_attribute: optional, string, default 'coord_z'. Z coordinate of the graph vertices.
-        """
-        random_walk_on_sphere_set_position_based_on_graph(arr_selected_agent,
-                                                          self.df_population[agent_position_attribute],
-                                                          self.df_population['px'],
-                                                          self.df_population['py'],
-                                                          self.df_population['pz'],
-                                                          self.graph.df_attributes[graph_coord_x_attribute],
-                                                          self.graph.df_attributes[graph_coord_y_attribute],
-                                                          self.graph.df_attributes[graph_coord_z_attribute])
-
-    def start_random_walk_uniform_prob(self, prob, condition=None, return_arr_new_walker=True):
-        """
-        Perform a uniform test for each agent. Successful agents have their attribute 'is_on_random_walk' set to true.
-
-        :param prob: float, probability for all agent to start a random walk
-        :param condition: optional, 1D array of bool, default None.
-        :param return_arr_new_walker: optional, boolean, default True.
-
-        :return: None if return_arr_new_walker is False, a 1D array of bool otherwise.
-        """
-        if condition is None:
-            arr_start_rw = np.random.uniform(0, 1, (self.df_population.shape[0],)) <= prob
-            if return_arr_new_walker:
-                return random_walk_on_sphere_start_random_walk_uniform_prob_return_new_walkers(arr_start_rw,
-                                                                                self.df_population['is_on_random_walk'])
-            random_walk_on_sphere_start_random_walk_uniform_prob(arr_start_rw, self.df_population['is_on_random_walk'])
-        else:
-            arr_start_rw = np.random.uniform(0, 1, (condition.sum(),)) <= prob
-            if return_arr_new_walker:
-                return conditional_random_walk_on_sphere_start_random_walk_uniform_prob_return_new_walkers(arr_start_rw,
-                                                                                                           self.df_population['is_on_random_walk'],
-                                                                                                           condition)
-            conditional_random_walk_on_sphere_start_random_walk_uniform_prob(arr_start_rw,
-                                                                             self.df_population['is_on_random_walk'],
-                                                                             condition)
-
-    def set_direction_to_north(self, arr_selected_agents):
-        """
-        Set the directions of the selected agents in the direction of the north pole (coordinates X and Y are 0.).
-        Agents located at the north or south pole have their initial direction set to (1., 0., 0.). Note that the
-        direction is a vector of norm 1.
-
-        :param arr_selected_agents: 1D array of bool
-        """
-        random_walk_on_sphere_set_initial_dir_to_north(arr_selected_agents,
-                                                       self.df_population['px'],
-                                                       self.df_population['py'],
-                                                       self.df_population['pz'],
-                                                       self.df_population['dx'],
-                                                       self.df_population['dy'],
-                                                       self.df_population['dz'])
-
-    def set_direction_von_mises(self, arr_selected_agents, kappa):
-        """
-        Set the direction of the selected agents by deviating their current direction by an angle given by von mises
-        distribution.
-
-        :param arr_selected_agents: 1D array of bool saying which agent should have their direction changed
-        :param kappa: kappa parameter for the von mises distribution. The hiher the value of Kappa, the smaller the
-                      deviation.
-        """
-        deviation_angles = np.random.vonmises(0, kappa, (arr_selected_agents.sum(),))
-        random_walk_on_sphere_deviate_direction_from_angles(deviation_angles, arr_selected_agents,
-                                                            self.df_population['px'],
-                                                            self.df_population['py'],
-                                                            self.df_population['pz'],
-                                                            self.df_population['dx'],
-                                                            self.df_population['dy'],
-                                                            self.df_population['dz'])
-
-    def make_step_using_gamma_law(self, arr_selected_agents, k, theta, radius,
-                                  list_proximity_classes=None, mode_proximity_test='AND',
-                                  return_agents_failed_making_step=False):
-        """
-        The selected agents make a step, following their current direction with a step length given by a
-        Gamma distribution. The user can provide a list of proximity class to test if the step fails or succeed.
-
-        :param arr_selected_agents: 1D array of bool saying which agent should make a new step
-        :param k: shape parameter gamma law
-        :param theta: scale parameter gamma law
-        :param radius: float, radius of the sphere on which the agents live
-        :param list_proximity_classes: optional, list of proximity class, default None. If a list of proximity class is
-                                       provided, the method will check that each step is valid according to those
-                                       proximity class. If the list has more than one element, this test is done using
-                                       the methodology defined by the kwarg mode_proximity_test.
-        :param mode_proximity_test: optional, string, default 'AND'. Only two accepted values, that are 'AND' and 'OR'.
-                                    If 'AND', a step is valid if and only if all the proximity classes validate it.
-                                    IF 'OR', a step is valid if at least one of the proximity classes validate it.
-        :param return_agents_failed_making_step: optional, boolean, default False. If True, returns a 1D array of bool
-                                                 Saying which agent failed their step.
-                                                 WARNING: in the resulting array res, res[i] is True if and only if
-                                                          the agent at line i had the opportunity to make a step but
-                                                          failed to do so. If res[i] is False, then it means the agent
-                                                          at line i either was not selected to make a step, or succeded
-                                                          to do so.
-
-        :return: if return_agents_failed_making_step is True, 1D array of bool. None otherwise.
-        """
-        gamma_sample = np.random.gamma(k, theta, size=(arr_selected_agents.sum(),))
-
-        if list_proximity_classes is not None:
-
-            new_px, new_py, new_pz, new_dx, new_dy, new_dz = random_walk_on_sphere_propose_step_gamma_law(
-                                                                                  arr_selected_agents, gamma_sample,
-                                                                                  self.df_population['px'],
-                                                                                  self.df_population['py'],
-                                                                                  self.df_population['pz'],
-                                                                                  self.df_population['dx'],
-                                                                                  self.df_population['dy'],
-                                                                                  self.df_population['dz'],
-                                                                                  radius)
-
-            list_arr_successful_steps = []
-            for proximity_class in list_proximity_classes:
-                list_arr_successful_steps.append(proximity_class.is_pos_allowed(new_px, new_py, new_pz))
-            if mode_proximity_test.lower() == 'and':
-                for i, arr in enumerate(list_arr_successful_steps):
-                    if i == 0:
-                        continue
-                    list_arr_successful_steps[0] = list_arr_successful_steps[0] & arr
-            elif mode_proximity_test.lower() == 'or':
-                for i, arr in enumerate(list_arr_successful_steps):
-                    if i == 0:
-                        continue
-                    list_arr_successful_steps[0] = list_arr_successful_steps[0] | arr
-            else:
-                raise ValueError("The value for mode_proximity_test kwarg should either be 'AND' or 'OR'.")
-
-            if return_agents_failed_making_step:
-                return random_walk_on_sphere_validate_step_return_fail(arr_selected_agents,
-                                                                       list_arr_successful_steps[0],
-                                                                       new_px, new_py, new_pz, new_dx, new_dy, new_dz,
-                                                                       self.df_population['px'],
-                                                                       self.df_population['py'],
-                                                                       self.df_population['pz'],
-                                                                       self.df_population['dx'],
-                                                                       self.df_population['dy'],
-                                                                       self.df_population['dz'])
-
-            random_walk_on_sphere_validate_step(arr_selected_agents, list_arr_successful_steps[0],
-                                                new_px, new_py, new_pz, new_dx, new_dy, new_dz,
-                                                self.df_population['px'],
-                                                self.df_population['py'],
-                                                self.df_population['pz'],
-                                                self.df_population['dx'],
-                                                self.df_population['dy'],
-                                                self.df_population['dz'])
-
-        else:
-            random_walk_on_sphere_make_step_gamma_law(arr_selected_agents, gamma_sample,
-                                                      self.df_population['px'],
-                                                      self.df_population['py'],
-                                                      self.df_population['pz'],
-                                                      self.df_population['dx'],
-                                                      self.df_population['dy'],
-                                                      self.df_population['dz'],
-                                                      radius)
-
-
-# class RandomWalkOnSphere:
-#     """
-#     This class give the ability for the agent to perform random walks on a sphere. The directions are preserved between
-#     consecutive steps by using parallel transport.
-#     """
-#     def __init__(self):
-#         self.radius = 1.
-#         self.unit = 'km'
-#         if hasattr(self, 'df_population'):
-#             self.df_population['is_on_random_walk'] = False
-#             self.df_population['coord_x'] = np.nan
-#             self.df_population['coord_y'] = np.nan
-#             self.df_population['coord_z'] = np.nan
-#             self.df_population['direction_x'] = np.nan
-#             self.df_population['direction_y'] = np.nan
-#             self.df_population['direction_z'] = np.nan
-#         else:
-#             self.df_population = pd.DataFrame(columns=['is_on_random_walk', 'coord_x', 'coord_y', 'coord_z',
-#                                                        'direction_x', 'direction_y', 'direction_z'])
-#
-#         if hasattr(self, 'dict_default_values'):
-#             self.dict_default_values['is_on_random_walk'] = False
-#             self.dict_default_values['coord_x'] = np.nan
-#             self.dict_default_values['coord_y'] = np.nan
-#             self.dict_default_values['coord_z'] = np.nan
-#             self.dict_default_values['direction_x'] = np.nan
-#             self.dict_default_values['direction_y'] = np.nan
-#             self.dict_default_values['direction_z'] = np.nan
-#         else:
-#             self.dict_default_values = dict()
-#             self.dict_default_values['is_on_random_walk'] = False
-#             self.dict_default_values['coord_x'] = np.nan
-#             self.dict_default_values['coord_y'] = np.nan
-#             self.dict_default_values['coord_z'] = np.nan
-#             self.dict_default_values['direction_x'] = np.nan
-#             self.dict_default_values['direction_y'] = np.nan
-#             self.dict_default_values['direction_z'] = np.nan
-#         super().__init__()
-#
-#     def set_radius(self, radius, unit='km'):
-#         """
-#         Set the value of the radius of the sphere on which the agents walk.
-#         :param radius: float, value for the radius of the sphere.
-#         :param unit: optional, string, default 'km'. Unit used for distances. For the moment, this parameter is not
-#             used by any method.
-#         """
-#         self.radius = radius
-#         self.unit = unit
-#
-#     def _temp_exit_random_walk_based_on_k(self, arr_selected_agents, arr_pos_selected_agents, prob_settlement, alpha,
-#                                           arr_pop=None):
-#         """
-#         This method is considered private as it is a quick and dirty hack to have a 'kind of realistic' condition for
-#         exiting random walk state. This is not based on ANY literature, so be careful and use at your own risk.
-#         """
-#         arr_selected_agents = np.array(arr_selected_agents)
-#         # print('selected_agents', arr_selected_agents)
-#         arr_pos_selected_agents = np.array(arr_pos_selected_agents, dtype=np.int32)
-#         # print('pos_agents', arr_pos_selected_agents)
-#         # print(arr_pos_selected_agents)
-#         nb_agents = arr_selected_agents.sum()
-#         rand = np.random.uniform(0, 1, (nb_agents,))
-#         arr_k = np.array(self.graph.df_attributes['K'])
-#         if arr_pop is None:
-#             arr_pop = self.count_pop_per_vertex(position_attribute='territory')
-#         arr_pop = np.array(arr_pop, dtype=np.int32)
-#         arr_stop = _temp_random_walk_on_sphere_exit_random_walk_based_on_k(arr_selected_agents, rand, prob_settlement,
-#                                                                            alpha, arr_pos_selected_agents, arr_k,
-#                                                                            arr_pop)
-#         # print('stopping agents:', arr_stop)
-#         self.df_population['is_on_random_walk'] = self.df_population['is_on_random_walk'] & ~arr_stop
-#         # print(self.df_population[['territory', 'col_id']])
-#         # print(self.df_population['territory'])
-#         self.df_population['territory'] = self.df_population['territory'] + \
-#                                           arr_stop * (arr_pos_selected_agents - self.df_population['territory'])
-#         # print(' ')
-#         # print(self.df_population['territory'])
-#         # print('---------')
-#         # time.sleep(2.)
-#
-#         self.df_population['position'] = self.df_population['position'] + \
-#                                           arr_stop * (arr_pos_selected_agents - self.df_population['position'])
-#         return arr_stop
-
+import numpy as np
+import pandas as pd
+import time
+
+from .jit_compiled_functions import (random_walk_on_sphere_set_position_based_on_graph,
+                                     random_walk_on_sphere_start_random_walk_uniform_prob,
+                                     random_walk_on_sphere_start_random_walk_uniform_prob_return_new_walkers,
+                                     conditional_random_walk_on_sphere_start_random_walk_uniform_prob,
+                                     conditional_random_walk_on_sphere_start_random_walk_uniform_prob_return_new_walkers,
+                                     random_walk_on_sphere_set_initial_dir_to_north,
+                                     random_walk_on_sphere_deviate_direction_from_angles,
+                                     random_walk_on_sphere_propose_step_gamma_law,
+                                     random_walk_on_sphere_make_step_gamma_law,
+                                     random_walk_on_sphere_validate_step,
+                                     random_walk_on_sphere_validate_step_return_fail,
+                                     _temp_random_walk_on_sphere_exit_random_walk_based_on_k,
+                                     random_walk_on_sphere_exit_random_walk_according_to_proximity_class,
+                                     random_walk_on_sphere_exit_random_walk_according_to_proximity_class_no_status_update,
+                                     random_walk_on_sphere_exit_random_walk_according_to_proximity_class_return_fail)
+
+
+class SphericalRandomWalk:
+    """
+    This class give the ability for the agent to perform random walks on a sphere. The directions 
+    are preserved between consecutive steps by using parallel transport. The associated technical 
+    background can be found in the publication {in-preparation} by F. Viard, A. Allibert and 
+    P. Leighton.
+    """
+    def __init__(self, px=0., py=0., pz=0., dx=0., dy=0., dz=0., **kwargs):
+        self.df_population['is_on_random_walk'] = False
+        self.df_population['px'] = px
+        self.df_population['py'] = py
+        self.df_population['pz'] = pz
+        self.df_population['dx'] = dx
+        self.df_population['dy'] = dy
+        self.df_population['dz'] = dz
+
+        self.dict_default_val['is_on_random_walk'] = False
+        self.dict_default_val['px'] = px
+        self.dict_default_val['py'] = py
+        self.dict_default_val['pz'] = pz
+        self.dict_default_val['dx'] = dx
+        self.dict_default_val['dy'] = dy
+        self.dict_default_val['dz'] = dz
+
+    def set_dtype_of_positions_and_directions(self, targeted_dtype='float64'):
+        """
+        The computations needed for spherical random walks, as they are now, are really sensitive to
+        rounding errors. Therefore, it may be needed to increase the precision of columns px, py, 
+        pz, dx, dy and dz to float64. This method is a shortcut for doing it on all 6 columns. 
+        This method won't have any effect if there is no agents.
+
+        :param targeted_dtype: optional, string, default 'float64'. The new datatype for the 
+                               position and direction columns.
+
+        :return: True if the columns were not empty and the assignement succeded, False otherwise.
+        """
+        if self.df_population.is_empty:
+            return False
+
+        self.df_population.change_type('px', targeted_dtype)
+        self.df_population.change_type('py', targeted_dtype)
+        self.df_population.change_type('pz', targeted_dtype)
+        self.df_population.change_type('dx', targeted_dtype)
+        self.df_population.change_type('dy', targeted_dtype)
+        self.df_population.change_type('dz', targeted_dtype)
+
+        return True
+
+    def set_position_based_on_graph(self, arr_selected_agent,
+                                    agent_position_attribute='position',
+                                    graph_coord_x_attribute='coord_x',
+                                    graph_coord_y_attribute='coord_y',
+                                    graph_coord_z_attribute='coord_z'):
+        """
+        Set the position of the selected agents using coordinates of the graph vertex the agent is 
+        currently on.
+
+        :param arr_selected_agent: 1D array of bool, saying which agents should have their 
+                                   coordinates updated according to their position on the graph.
+        :param agent_position_attribute: optional, string, default 'position'. Name of the attribute 
+                                         position column in the df_population dataframe in the agent 
+                                         class.
+        :param graph_coord_x_attribute: optional, string, default 'coord_x'. X coordinate of the 
+                                        graph vertices.
+        :param graph_coord_y_attribute: optional, string, default 'coord_y'. Y coordinate of the 
+                                        graph vertices.
+        :param graph_coord_z_attribute: optional, string, default 'coord_z'. Z coordinate of the 
+                                        graph vertices.
+        """
+        random_walk_on_sphere_set_position_based_on_graph(arr_selected_agent,
+                                                          self.df_population[agent_position_attribute],
+                                                          self.df_population['px'],
+                                                          self.df_population['py'],
+                                                          self.df_population['pz'],
+                                                          self.graph.df_attributes[graph_coord_x_attribute],
+                                                          self.graph.df_attributes[graph_coord_y_attribute],
+                                                          self.graph.df_attributes[graph_coord_z_attribute])
+
+    def start_random_walk_uniform_prob(self, prob, condition=None, return_arr_new_walker=True):
+        """
+        Perform a uniform test for each agent. Successful agents have their attribute 
+        'is_on_random_walk' set to true.
+
+        :param prob: float, probability for all agent to start a random walk
+        :param condition: optional, 1D array of bool, default None.
+        :param return_arr_new_walker: optional, boolean, default True.
+
+        :return: None if return_arr_new_walker is False, a 1D array of bool otherwise.
+        """
+        if condition is None:
+            arr_start_rw = np.random.uniform(0, 1, (self.df_population.shape[0],)) <= prob
+            if return_arr_new_walker:
+                return random_walk_on_sphere_start_random_walk_uniform_prob_return_new_walkers(arr_start_rw,
+                                                                                self.df_population['is_on_random_walk'])
+            random_walk_on_sphere_start_random_walk_uniform_prob(arr_start_rw, self.df_population['is_on_random_walk'])
+        else:
+            arr_start_rw = np.random.uniform(0, 1, (condition.sum(),)) <= prob
+            if return_arr_new_walker:
+                return conditional_random_walk_on_sphere_start_random_walk_uniform_prob_return_new_walkers(arr_start_rw,
+                                                                                self.df_population['is_on_random_walk'],
+                                                                                condition)
+            conditional_random_walk_on_sphere_start_random_walk_uniform_prob(arr_start_rw,
+                                                                             self.df_population['is_on_random_walk'],
+                                                                             condition)
+
+    def set_direction_to_north(self, arr_selected_agents):
+        """
+        Set the directions of the selected agents in the direction of the north pole (coordinates X 
+        and Y are 0.). Agents located at the north or south pole have their initial direction set to
+        (1., 0., 0.). Note that the direction is always a vector of norm 1.
+
+        :param arr_selected_agents: 1D array of bool
+        """
+        random_walk_on_sphere_set_initial_dir_to_north(arr_selected_agents,
+                                                       self.df_population['px'],
+                                                       self.df_population['py'],
+                                                       self.df_population['pz'],
+                                                       self.df_population['dx'],
+                                                       self.df_population['dy'],
+                                                       self.df_population['dz'])
+
+    def set_direction_von_mises(self, arr_selected_agents, kappa, mean=0.):
+        """
+        Set the direction of the selected agents by deviating their current direction by an angle 
+        given by von mises distribution.
+
+        :param arr_selected_agents: 1D array of bool saying which agent should have their direction 
+                                    changed
+        :param kappa: kappa parameter for the von mises distribution. The hiher the value of Kappa, 
+                      the smaller the deviation.
+        :param mean: optionnal, float, default 0. . The mean of the von-mises distribution.
+        """
+        deviation_angles = np.random.vonmises(mean, kappa, (arr_selected_agents.sum(),))
+        random_walk_on_sphere_deviate_direction_from_angles(deviation_angles, arr_selected_agents,
+                                                            self.df_population['px'],
+                                                            self.df_population['py'],
+                                                            self.df_population['pz'],
+                                                            self.df_population['dx'],
+                                                            self.df_population['dy'],
+                                                            self.df_population['dz'])
+
+    def make_step_using_gamma_law(self, arr_selected_agents, k, theta, radius,
+                                  list_proximity_classes=None, mode_proximity_test='AND',
+                                  return_agents_failed_making_step=False):
+        """
+        The selected agents make a step, following their current direction with a step length given 
+        by a Gamma distribution. The user can provide a list of proximity class to test if the step 
+        fails or succeed.
+
+        :param arr_selected_agents: 1D array of bool saying which agent should make a new step
+        :param k: shape parameter gamma law
+        :param theta: scale parameter gamma law
+        :param radius: float, radius of the sphere on which the agents live
+        :param list_proximity_classes: optional, list of proximity class, default None. If a list of
+                                       proximity class is provided, the method will check that each 
+                                       step is valid according to those proximity class. If the list 
+                                       has more than one element, this test is done using the 
+                                       methodology defined by the kwarg mode_proximity_test.
+        :param mode_proximity_test: optional, string, default 'AND'. Only two accepted values, that 
+                                    are 'AND' and 'OR'. If 'AND', a step is valid if and only if all
+                                    the proximity classes validate it. IF 'OR', a step is valid if 
+                                    at least one of the proximity classes validate it.
+        :param return_agents_failed_making_step: optional, boolean, default False. If True, returns 
+                                                 a 1D array of bool Saying which agent failed their 
+                                                 step.
+                                                 WARNING: in the resulting array res, res[i] is True if and only if
+                                                          the agent at line i had the opportunity to make a step but
+                                                          failed to do so. If res[i] is False, then it means the agent
+                                                          at line i either was not selected to make a step, or succeded
+                                                          to do so.
+
+        :return: if return_agents_failed_making_step is True, 1D array of bool. None otherwise.
+        """
+        gamma_sample = np.random.gamma(k, theta, size=(arr_selected_agents.sum(),))
+
+        if list_proximity_classes is not None:
+
+            new_px, new_py, new_pz, new_dx, new_dy, new_dz = random_walk_on_sphere_propose_step_gamma_law(
+                                                                                  arr_selected_agents, gamma_sample,
+                                                                                  self.df_population['px'],
+                                                                                  self.df_population['py'],
+                                                                                  self.df_population['pz'],
+                                                                                  self.df_population['dx'],
+                                                                                  self.df_population['dy'],
+                                                                                  self.df_population['dz'],
+                                                                                  radius)
+
+            list_arr_successful_steps = []
+            for proximity_class in list_proximity_classes:
+                list_arr_successful_steps.append(proximity_class.is_pos_allowed(new_px, new_py, new_pz))
+            if mode_proximity_test.lower() == 'and':
+                for i, arr in enumerate(list_arr_successful_steps):
+                    if i == 0:
+                        continue
+                    list_arr_successful_steps[0] = list_arr_successful_steps[0] & arr
+            elif mode_proximity_test.lower() == 'or':
+                for i, arr in enumerate(list_arr_successful_steps):
+                    if i == 0:
+                        continue
+                    list_arr_successful_steps[0] = list_arr_successful_steps[0] | arr
+            else:
+                raise ValueError("The value for mode_proximity_test kwarg should either be 'AND' or 'OR'.")
+
+            if return_agents_failed_making_step:
+                return random_walk_on_sphere_validate_step_return_fail(arr_selected_agents,
+                                                                       list_arr_successful_steps[0],
+                                                                       new_px, new_py, new_pz, new_dx, new_dy, new_dz,
+                                                                       self.df_population['px'],
+                                                                       self.df_population['py'],
+                                                                       self.df_population['pz'],
+                                                                       self.df_population['dx'],
+                                                                       self.df_population['dy'],
+                                                                       self.df_population['dz'])
+
+            random_walk_on_sphere_validate_step(arr_selected_agents, list_arr_successful_steps[0],
+                                                new_px, new_py, new_pz, new_dx, new_dy, new_dz,
+                                                self.df_population['px'],
+                                                self.df_population['py'],
+                                                self.df_population['pz'],
+                                                self.df_population['dx'],
+                                                self.df_population['dy'],
+                                                self.df_population['dz'])
+
+        else:
+            random_walk_on_sphere_make_step_gamma_law(arr_selected_agents, gamma_sample,
+                                                      self.df_population['px'],
+                                                      self.df_population['py'],
+                                                      self.df_population['pz'],
+                                                      self.df_population['dx'],
+                                                      self.df_population['dy'],
+                                                      self.df_population['dz'],
+                                                      radius)
+
+    def exit_random_walk_according_to_proximity_class(self, arr_selected_agents, proximity_class_from_graph, 
+                                                      position_attribute='position', extra_position_attributes=None,
+                                                      return_agents_that_failed=False):
+        """
+        This method ends the movement of the selected agents with respect to a proximity class linked to a graph
+        object. 
+
+        :param arr_selected_agents: 1D array of bool telling which agent are trying to exit random walk.
+        :param proximity_class_from_graph: proximity class. Should be linked to the graph on which the agents
+                                           try to settle.
+        :param position_attribute: optional, string, default position. Position attribute to use.
+        :param extra_position_attributes: optional, list of string, default None. If needed, this argument can
+                                          be used to update extra position attributes.
+        :param return_agents_that_failed: optional, boolean, default False. If True, the method returns a 1D
+                                          array of bool telling which agents failed to end their walk.
+        """
+        coord_x = self.df_population['px'][arr_selected_agents]
+        coord_y = self.df_population['py'][arr_selected_agents]
+        coord_z = self.df_population['pz'][arr_selected_agents]
+
+        distances, indices = proximity_class_from_graph.get_closest_point(coord_x, coord_y, coord_z)
+        arr_success = proximity_class_from_graph.is_pos_allowed(coord_x, coord_y, coord_z,
+                                                                distances=distances, indices=indices)
+
+        if extra_position_attributes is not None:
+            for pos_attribute in extra_position_attributes:
+                random_walk_on_sphere_exit_random_walk_according_to_proximity_class_no_status_update(arr_success, indices,
+                                                                                arr_selected_agents, 
+                                                                                self.df_population[pos_attribute])
+
+        if return_agents_that_failed:
+            return random_walk_on_sphere_exit_random_walk_according_to_proximity_class_return_fail(arr_success, indices,
+                                                                                arr_selected_agents, 
+                                                                                self.df_population[position_attribute],
+                                                                                self.df_population['is_on_random_walk'])
+        else:
+            random_walk_on_sphere_exit_random_walk_according_to_proximity_class(arr_success, indices,
+                                                                                arr_selected_agents, 
+                                                                                self.df_population[position_attribute],
+                                                                                self.df_population['is_on_random_walk'])
+
+
+# class RandomWalkOnSphere:
+#     """
+#     This class give the ability for the agent to perform random walks on a sphere. The directions are preserved between
+#     consecutive steps by using parallel transport.
+#     """
+#     def __init__(self):
+#         self.radius = 1.
+#         self.unit = 'km'
+#         if hasattr(self, 'df_population'):
+#             self.df_population['is_on_random_walk'] = False
+#             self.df_population['coord_x'] = np.nan
+#             self.df_population['coord_y'] = np.nan
+#             self.df_population['coord_z'] = np.nan
+#             self.df_population['direction_x'] = np.nan
+#             self.df_population['direction_y'] = np.nan
+#             self.df_population['direction_z'] = np.nan
+#         else:
+#             self.df_population = pd.DataFrame(columns=['is_on_random_walk', 'coord_x', 'coord_y', 'coord_z',
+#                                                        'direction_x', 'direction_y', 'direction_z'])
+#
+#         if hasattr(self, 'dict_default_values'):
+#             self.dict_default_values['is_on_random_walk'] = False
+#             self.dict_default_values['coord_x'] = np.nan
+#             self.dict_default_values['coord_y'] = np.nan
+#             self.dict_default_values['coord_z'] = np.nan
+#             self.dict_default_values['direction_x'] = np.nan
+#             self.dict_default_values['direction_y'] = np.nan
+#             self.dict_default_values['direction_z'] = np.nan
+#         else:
+#             self.dict_default_values = dict()
+#             self.dict_default_values['is_on_random_walk'] = False
+#             self.dict_default_values['coord_x'] = np.nan
+#             self.dict_default_values['coord_y'] = np.nan
+#             self.dict_default_values['coord_z'] = np.nan
+#             self.dict_default_values['direction_x'] = np.nan
+#             self.dict_default_values['direction_y'] = np.nan
+#             self.dict_default_values['direction_z'] = np.nan
+#         super().__init__()
+#
+#     def set_radius(self, radius, unit='km'):
+#         """
+#         Set the value of the radius of the sphere on which the agents walk.
+#         :param radius: float, value for the radius of the sphere.
+#         :param unit: optional, string, default 'km'. Unit used for distances. For the moment, this parameter is not
+#             used by any method.
+#         """
+#         self.radius = radius
+#         self.unit = unit
+#
+#     def _temp_exit_random_walk_based_on_k(self, arr_selected_agents, arr_pos_selected_agents, prob_settlement, alpha,
+#                                           arr_pop=None):
+#         """
+#         This method is considered private as it is a quick and dirty hack to have a 'kind of realistic' condition for
+#         exiting random walk state. This is not based on ANY literature, so be careful and use at your own risk.
+#         """
+#         arr_selected_agents = np.array(arr_selected_agents)
+#         # print('selected_agents', arr_selected_agents)
+#         arr_pos_selected_agents = np.array(arr_pos_selected_agents, dtype=np.int32)
+#         # print('pos_agents', arr_pos_selected_agents)
+#         # print(arr_pos_selected_agents)
+#         nb_agents = arr_selected_agents.sum()
+#         rand = np.random.uniform(0, 1, (nb_agents,))
+#         arr_k = np.array(self.graph.df_attributes['K'])
+#         if arr_pop is None:
+#             arr_pop = self.count_pop_per_vertex(position_attribute='territory')
+#         arr_pop = np.array(arr_pop, dtype=np.int32)
+#         arr_stop = _temp_random_walk_on_sphere_exit_random_walk_based_on_k(arr_selected_agents, rand, prob_settlement,
+#                                                                            alpha, arr_pos_selected_agents, arr_k,
+#                                                                            arr_pop)
+#         # print('stopping agents:', arr_stop)
+#         self.df_population['is_on_random_walk'] = self.df_population['is_on_random_walk'] & ~arr_stop
+#         # print(self.df_population[['territory', 'col_id']])
+#         # print(self.df_population['territory'])
+#         self.df_population['territory'] = self.df_population['territory'] + \
+#                                           arr_stop * (arr_pos_selected_agents - self.df_population['territory'])
+#         # print(' ')
+#         # print(self.df_population['territory'])
+#         # print('---------')
+#         # time.sleep(2.)
+#
+#         self.df_population['position'] = self.df_population['position'] + \
+#                                           arr_stop * (arr_pos_selected_agents - self.df_population['position'])
+#         return arr_stop
+
```

### Comparing `sampy-abm-1.0.2/src/sampy/data_processing/csv_manager.py` & `sampy_abm-1.0.3/src/sampy/data_processing/csv_manager.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,159 +1,159 @@
-import numpy as np
-
-
-class ParamManager:
-    def __init__(self, names, values):
-        for name, value in zip(names, values):
-            setattr(self, name, value)
-
-
-class CsvManager:
-    """
-    Realistically, most of Sampy's run will be done during sensitivity analysis to assert that the model is a faithful
-    representation of the ecological system of interest. The current class is Sampy's solution for dealing with vast CSV
-    of parameters used to run large scale sensitivity analysis.
-
-    The expected CSV structure is as follows.
-
-        - Each row should correspond to the parameters used in a single run of the model.
-        - Each column corresponds either to a constant parameter, or to a single value within an array.
-        - the current class distinguishes parameters that should be stored in array based on their name in the header.
-          That is, if a column name is of the form arr_[some name]_[some_number], then the content of this column will
-          be considered as the [some_number]-th element of an array. The array's name will be [some_name].
-
-    Let show the use of CsvManager class on a small example. Assume we have a csv of parameter at the adress path_csv,
-    and that the two first line of the csv are:
-
-    const1;const2;arr_test_array_0;arr_test_array_1;arr_another_array_0
-    0;wonderful_string_of_chars;2.;3.;True
-
-    One can instantiates a CsvManager class the following way:
-
-    >>> csv_manager = CsvManager(path_csv, ';', dict_types={'const1': int, 'test_array': float, 'another_array': bool})
-
-    Then, by calling the method 'get_parameters', one gets a ParamManager object whose attributes are the parameters
-    stored in a line of the csv.
-
-    >>> param = csv_manager.get_parameters()
-    >>> print(param.test_array)
-    array([2., 3.])
-
-    If one calls get_parameters another time, it will return another ParamManager object corresponding to the next line
-    in the csv. Once the end of the csv is reached, get_parameters returns None.
-
-    The kwargs 'nb_cores' and 'id_process' are designed for large analysis using multiple cores. If used, the obtained
-    csv_manager will only return lines 'i' in the csv such that 'i % nb_cores == id_process'.
-
-    Finally, when working on very large csv one can use the kwarg buffer_size (default 1000) which says how many
-    lines of the csv are stored in memory (CsvManager does not try to open the file entirely in memory, and process it
-    by blocks of buffer_size lines).
-    """
-    def __init__(self, path_to_csv, sep, dict_types=None, buffer_size=1000, nb_cores=1, id_process=0):
-        self.path_to_csv = path_to_csv
-        self.sep = sep
-        if dict_types is None:
-            self.dict_types = {}
-        else:
-            self.dict_types = dict_types
-
-        self.buffer_size = buffer_size
-        self.nb_line_consumed = 0
-        self.buffer = []
-        self.counter_buffer = 0
-
-        self.nb_usable_lines_in_csv = 0
-
-        self.dict_arr = {}
-        self.dict_const = {}
-
-        self.nb_cores = nb_cores
-        self.id_process = id_process
-
-        with open(self.path_to_csv, 'r') as f_in:
-            for i, line in enumerate(f_in):
-                if i == 0:
-                    self.header = line.replace('\n', '')
-                    self.extract_info_header()
-                    continue
-                if i % self.nb_cores == self.id_process:
-                    self.nb_usable_lines_in_csv += 1
-
-    def extract_info_header(self):
-        list_header = self.header.split(self.sep)
-        dict_col_to_index = {col_name: ind for ind, col_name in enumerate(list_header)}
-        r_dict_const = {}
-        temp_dict_arr = {}
-        for col_name in list_header:
-            if col_name.split('_')[0] == 'arr':
-                name_param = '_'.join(col_name.split('_')[1:-1])
-                try:
-                    temp_dict_arr[name_param].append(col_name)
-                except KeyError:
-                    temp_dict_arr[name_param] = [col_name]
-            else:
-                r_dict_const[col_name] = dict_col_to_index[col_name]
-        r_dict_arr = {}
-        for name_arr, arr in temp_dict_arr.items():
-            sorted_arr = sorted(arr, key=lambda y: int(y.split('_')[-1]))
-            r_dict_arr[name_arr] = [dict_col_to_index[name_col] for name_col in sorted_arr]
-        self.dict_arr = r_dict_arr
-        self.dict_const = r_dict_const
-
-    def get_parameters(self):
-        try:
-            line = self.buffer[self.counter_buffer]
-            self.counter_buffer += 1
-            self.nb_line_consumed += 1
-        except IndexError:
-            if self.nb_line_consumed == self.nb_usable_lines_in_csv:
-                return
-            self.fill_buffer()
-            line = self.buffer[0]
-            self.counter_buffer = 1
-            self.nb_line_consumed += 1
-        return self.create_param_manager_from_line(line)
-
-    def fill_buffer(self):
-        self.buffer = []
-        size_current_buffer = 0
-        with open(self.path_to_csv) as f:
-            seen_lines = 0
-            for i, line in enumerate(f):
-                if i == 0:
-                    continue
-                if i % self.nb_cores == self.id_process:
-                    seen_lines += 1
-                    if seen_lines <= self.nb_line_consumed:
-                        continue
-                    self.buffer.append(line.replace('\n', ''))
-                    size_current_buffer += 1
-                    if size_current_buffer == self.buffer_size:
-                        break
-        return
-
-    def create_param_manager_from_line(self, line):
-        data = line.split(self.sep)
-        names = []
-        values = []
-        for name in self.dict_const:
-            names.append(name)
-            if name in self.dict_types:
-                if self.dict_types[name] == bool:
-                    values.append(data[self.dict_const[name]].lower() == 'true')
-                else:
-                    values.append(self.dict_types[name](data[self.dict_const[name]]))
-            else:
-                values.append(data[self.dict_const[name]])
-        for name in self.dict_arr:
-            names.append(name)
-            if name in self.dict_types:
-                if self.dict_types[name] == bool:
-                    values.append(np.array([data[u].lower() == 'true' for u in self.dict_arr[name]]))
-                else:
-                    values.append(np.array([self.dict_types[name](data[u]) for u in self.dict_arr[name]]))
-            else:
-                values.append(np.array([data[u] for u in self.dict_arr[name]]))
-        return ParamManager(names, values)
-
-
-
+import numpy as np
+
+
+class ParamManager:
+    def __init__(self, names, values):
+        for name, value in zip(names, values):
+            setattr(self, name, value)
+
+
+class CsvManager:
+    """
+    Realistically, most of Sampy's run will be done during sensitivity analysis to assert that the model is a faithful
+    representation of the ecological system of interest. The current class is Sampy's solution for dealing with vast CSV
+    of parameters used to run large scale sensitivity analysis.
+
+    The expected CSV structure is as follows.
+
+        - Each row should correspond to the parameters used in a single run of the model.
+        - Each column corresponds either to a constant parameter, or to a single value within an array.
+        - the current class distinguishes parameters that should be stored in array based on their name in the header.
+          That is, if a column name is of the form arr_[some name]_[some_number], then the content of this column will
+          be considered as the [some_number]-th element of an array. The array's name will be [some_name].
+
+    Let show the use of CsvManager class on a small example. Assume we have a csv of parameter at the adress path_csv,
+    and that the two first line of the csv are:
+
+    const1;const2;arr_test_array_0;arr_test_array_1;arr_another_array_0
+    0;wonderful_string_of_chars;2.;3.;True
+
+    One can instantiates a CsvManager class the following way:
+
+    >>> csv_manager = CsvManager(path_csv, ';', dict_types={'const1': int, 'test_array': float, 'another_array': bool})
+
+    Then, by calling the method 'get_parameters', one gets a ParamManager object whose attributes are the parameters
+    stored in a line of the csv.
+
+    >>> param = csv_manager.get_parameters()
+    >>> print(param.test_array)
+    array([2., 3.])
+
+    If one calls get_parameters another time, it will return another ParamManager object corresponding to the next line
+    in the csv. Once the end of the csv is reached, get_parameters returns None.
+
+    The kwargs 'nb_cores' and 'id_process' are designed for large analysis using multiple cores. If used, the obtained
+    csv_manager will only return lines 'i' in the csv such that 'i % nb_cores == id_process'.
+
+    Finally, when working on very large csv one can use the kwarg buffer_size (default 1000) which says how many
+    lines of the csv are stored in memory (CsvManager does not try to open the file entirely in memory, and process it
+    by blocks of buffer_size lines).
+    """
+    def __init__(self, path_to_csv, sep, dict_types=None, buffer_size=1000, nb_cores=1, id_process=0):
+        self.path_to_csv = path_to_csv
+        self.sep = sep
+        if dict_types is None:
+            self.dict_types = {}
+        else:
+            self.dict_types = dict_types
+
+        self.buffer_size = buffer_size
+        self.nb_line_consumed = 0
+        self.buffer = []
+        self.counter_buffer = 0
+
+        self.nb_usable_lines_in_csv = 0
+
+        self.dict_arr = {}
+        self.dict_const = {}
+
+        self.nb_cores = nb_cores
+        self.id_process = id_process
+
+        with open(self.path_to_csv, 'r') as f_in:
+            for i, line in enumerate(f_in):
+                if i == 0:
+                    self.header = line.replace('\n', '')
+                    self.extract_info_header()
+                    continue
+                if i % self.nb_cores == self.id_process:
+                    self.nb_usable_lines_in_csv += 1
+
+    def extract_info_header(self):
+        list_header = self.header.split(self.sep)
+        dict_col_to_index = {col_name: ind for ind, col_name in enumerate(list_header)}
+        r_dict_const = {}
+        temp_dict_arr = {}
+        for col_name in list_header:
+            if col_name.split('_')[0] == 'arr':
+                name_param = '_'.join(col_name.split('_')[1:-1])
+                try:
+                    temp_dict_arr[name_param].append(col_name)
+                except KeyError:
+                    temp_dict_arr[name_param] = [col_name]
+            else:
+                r_dict_const[col_name] = dict_col_to_index[col_name]
+        r_dict_arr = {}
+        for name_arr, arr in temp_dict_arr.items():
+            sorted_arr = sorted(arr, key=lambda y: int(y.split('_')[-1]))
+            r_dict_arr[name_arr] = [dict_col_to_index[name_col] for name_col in sorted_arr]
+        self.dict_arr = r_dict_arr
+        self.dict_const = r_dict_const
+
+    def get_parameters(self):
+        try:
+            line = self.buffer[self.counter_buffer]
+            self.counter_buffer += 1
+            self.nb_line_consumed += 1
+        except IndexError:
+            if self.nb_line_consumed == self.nb_usable_lines_in_csv:
+                return
+            self.fill_buffer()
+            line = self.buffer[0]
+            self.counter_buffer = 1
+            self.nb_line_consumed += 1
+        return self.create_param_manager_from_line(line)
+
+    def fill_buffer(self):
+        self.buffer = []
+        size_current_buffer = 0
+        with open(self.path_to_csv) as f:
+            seen_lines = 0
+            for i, line in enumerate(f):
+                if i == 0:
+                    continue
+                if i % self.nb_cores == self.id_process:
+                    seen_lines += 1
+                    if seen_lines <= self.nb_line_consumed:
+                        continue
+                    self.buffer.append(line.replace('\n', ''))
+                    size_current_buffer += 1
+                    if size_current_buffer == self.buffer_size:
+                        break
+        return
+
+    def create_param_manager_from_line(self, line):
+        data = line.split(self.sep)
+        names = []
+        values = []
+        for name in self.dict_const:
+            names.append(name)
+            if name in self.dict_types:
+                if self.dict_types[name] == bool:
+                    values.append(data[self.dict_const[name]].lower() == 'true')
+                else:
+                    values.append(self.dict_types[name](data[self.dict_const[name]]))
+            else:
+                values.append(data[self.dict_const[name]])
+        for name in self.dict_arr:
+            names.append(name)
+            if name in self.dict_types:
+                if self.dict_types[name] == bool:
+                    values.append(np.array([data[u].lower() == 'true' for u in self.dict_arr[name]]))
+                else:
+                    values.append(np.array([self.dict_types[name](data[u]) for u in self.dict_arr[name]]))
+            else:
+                values.append(np.array([data[u] for u in self.dict_arr[name]]))
+        return ParamManager(names, values)
+
+
+
```

### Comparing `sampy-abm-1.0.2/src/sampy/disease/single_species/base.py` & `sampy_abm-1.0.3/src/sampy/disease/single_species/base.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-import numpy as np
-from .jit_compiled_functions import *
-from ...utils.errors_shortcut import check_col_exists_good_type
-
-
-class BaseSingleSpeciesDisease:
-    def __init__(self, disease_name=None, host=None, **kwargs):
-        # check values have been given
-        if host is None:
-            raise ValueError("No host given for the disease. Use the kwarg 'host'.")
-        if disease_name is None:
-            raise ValueError("No name given to the disease. Use the kwarg 'disease_name'.")
-
-        self.host = host
-        self.disease_name = disease_name
-
-        self.host.df_population['inf_' + disease_name] = False
-        self.host.df_population['con_' + disease_name] = False
-        self.host.df_population['imm_' + disease_name] = False
-
-        if hasattr(host, 'dict_default_val'):
-            self.host.dict_default_val['inf_' + disease_name] = False
-            self.host.dict_default_val['con_' + disease_name] = False
-            self.host.dict_default_val['imm_' + disease_name] = False
-
-        if not hasattr(self, 'list_disease_status'):
-            self.set_disease_status = {'inf', 'con', 'imm'}
-        else:
-            self.set_disease_status.update(['inf', 'con', 'imm'])
-
-        self.on_ticker = []
-
-    def tick(self):
-        """
-        execute in order all the methods whose name are in the list 'on_ticker'. Those methods should not accept
-        any arguments.
-        """
-        for method in self.on_ticker:
-            getattr(self, method)()
-
-    def _sampy_debug_count_nb_status_per_vertex(self, target_status, position_attribute='position'):
-        if self.host.df_population.nb_rows == 0:
-            return
-        check_col_exists_good_type(self.host.df_population, position_attribute, 'attribute_position',
-                                   prefix_dtype='int', reject_none=True)
-        check_col_exists_good_type(self.host.df_population, target_status + '_' + self.disease_name,
-                                   'target_status', prefix_dtype='bool', reject_none=True)
-
-    def count_nb_status_per_vertex(self, target_status, position_attribute='position'):
-        """
-        Count the number of agent having the targeted status in each vertex. The status can either be 'inf', 'con' and
-        'imm', which respectively corresponds to infected, contagious and immunized agents.
-
-        :param target_status: string in ['inf', 'con', 'imm'].
-        :param position_attribute: optional, string.
-
-        :return: array counting the number of agent having the target status in each vertex
-        """
-        if self.host.df_population.nb_rows == 0:
-            return np.full((self.host.graph.number_vertices,), 0, dtype=np.int32)
-        return base_conditional_count_nb_agent_per_vertex(self.host.df_population[target_status + '_' +
-                                                                                  self.disease_name],
-                                                          self.host.df_population[position_attribute],
-                                                          self.host.graph.weights.shape[0])
-
-    def contaminate_vertices(self, list_vertices, level, return_arr_newly_contaminated=True,
-                             condition=None, position_attribute='position'):
-        """
-        Contaminate the vertices given in the list 'list_vertices' with the disease. Each agent on the vertex have a
-        probability of 'level' to be contaminated.
-
-        :param list_vertices: list of vertices ID to be contaminated.
-        :param level: float, probability for agent on the vertices to be contaminated
-        :param return_arr_newly_contaminated: optional, boolean, default True. If True, the method returns an array
-                                              telling which agents were contaminated.
-        :param condition: optional, array of bool, default None. If not None, say which agents are susceptible to be
-                          contaminated.
-        :param position_attribute: optional, string, default 'position'. Agent attribute to be used to define
-                                   their position.
-        :return: if return_arr_newly_contaminated is set to True, returns a 1D array of bool. Otherwise, returns
-                 None.
-        """
-        for i, vertex_id in enumerate(list_vertices):
-            if i == 0:
-                arr_new_infected = (self.host.df_population[position_attribute] ==
-                                    self.host.graph.dict_cell_id_to_ind[vertex_id])
-                continue
-            arr_new_infected = arr_new_infected | (self.host.df_population[position_attribute] ==
-                                                   self.host.graph.dict_cell_id_to_ind[vertex_id])
-        arr_new_infected = arr_new_infected & ~(self.host.df_population['inf_' + self.disease_name] |
-                                                self.host.df_population['con_' + self.disease_name] |
-                                                self.host.df_population['imm_' + self.disease_name])
-        if condition is not None:
-            arr_new_infected = arr_new_infected & condition
-        rand = np.random.uniform(0, 1, (arr_new_infected.sum(),))
-        base_contaminate_vertices(arr_new_infected, rand, level)
-        self.host.df_population['inf_' + self.disease_name] = \
-            self.host.df_population['inf_' + self.disease_name] | arr_new_infected
-        if return_arr_newly_contaminated:
-            return arr_new_infected
+import numpy as np
+from .jit_compiled_functions import *
+from ...utils.errors_shortcut import check_col_exists_good_type
+
+
+class BaseSingleSpeciesDisease:
+    def __init__(self, disease_name=None, host=None, **kwargs):
+        # check values have been given
+        if host is None:
+            raise ValueError("No host given for the disease. Use the kwarg 'host'.")
+        if disease_name is None:
+            raise ValueError("No name given to the disease. Use the kwarg 'disease_name'.")
+
+        self.host = host
+        self.disease_name = disease_name
+
+        self.host.df_population['inf_' + disease_name] = False
+        self.host.df_population['con_' + disease_name] = False
+        self.host.df_population['imm_' + disease_name] = False
+
+        if hasattr(host, 'dict_default_val'):
+            self.host.dict_default_val['inf_' + disease_name] = False
+            self.host.dict_default_val['con_' + disease_name] = False
+            self.host.dict_default_val['imm_' + disease_name] = False
+
+        if not hasattr(self, 'list_disease_status'):
+            self.set_disease_status = {'inf', 'con', 'imm'}
+        else:
+            self.set_disease_status.update(['inf', 'con', 'imm'])
+
+        self.on_ticker = []
+
+    def tick(self):
+        """
+        execute in order all the methods whose name are in the list 'on_ticker'. Those methods should not accept
+        any arguments.
+        """
+        for method in self.on_ticker:
+            getattr(self, method)()
+
+    def _sampy_debug_count_nb_status_per_vertex(self, target_status, position_attribute='position'):
+        if self.host.df_population.nb_rows == 0:
+            return
+        check_col_exists_good_type(self.host.df_population, position_attribute, 'attribute_position',
+                                   prefix_dtype='int', reject_none=True)
+        check_col_exists_good_type(self.host.df_population, target_status + '_' + self.disease_name,
+                                   'target_status', prefix_dtype='bool', reject_none=True)
+
+    def count_nb_status_per_vertex(self, target_status, position_attribute='position'):
+        """
+        Count the number of agent having the targeted status in each vertex. The status can either be 'inf', 'con' and
+        'imm', which respectively corresponds to infected, contagious and immunized agents.
+
+        :param target_status: string in ['inf', 'con', 'imm'].
+        :param position_attribute: optional, string.
+
+        :return: array counting the number of agent having the target status in each vertex
+        """
+        if self.host.df_population.nb_rows == 0:
+            return np.full((self.host.graph.number_vertices,), 0, dtype=np.int32)
+        return base_conditional_count_nb_agent_per_vertex(self.host.df_population[target_status + '_' +
+                                                                                  self.disease_name],
+                                                          self.host.df_population[position_attribute],
+                                                          self.host.graph.weights.shape[0])
+
+    def contaminate_vertices(self, list_vertices, level, return_arr_newly_contaminated=True,
+                             condition=None, position_attribute='position'):
+        """
+        Contaminate the vertices given in the list 'list_vertices' with the disease. Each agent on the vertex have a
+        probability of 'level' to be contaminated.
+
+        :param list_vertices: list of vertices ID to be contaminated.
+        :param level: float, probability for agent on the vertices to be contaminated
+        :param return_arr_newly_contaminated: optional, boolean, default True. If True, the method returns an array
+                                              telling which agents were contaminated.
+        :param condition: optional, array of bool, default None. If not None, say which agents are susceptible to be
+                          contaminated.
+        :param position_attribute: optional, string, default 'position'. Agent attribute to be used to define
+                                   their position.
+        :return: if return_arr_newly_contaminated is set to True, returns a 1D array of bool. Otherwise, returns
+                 None.
+        """
+        for i, vertex_id in enumerate(list_vertices):
+            if i == 0:
+                arr_new_infected = (self.host.df_population[position_attribute] ==
+                                    self.host.graph.dict_cell_id_to_ind[vertex_id])
+                continue
+            arr_new_infected = arr_new_infected | (self.host.df_population[position_attribute] ==
+                                                   self.host.graph.dict_cell_id_to_ind[vertex_id])
+        arr_new_infected = arr_new_infected & ~(self.host.df_population['inf_' + self.disease_name] |
+                                                self.host.df_population['con_' + self.disease_name] |
+                                                self.host.df_population['imm_' + self.disease_name])
+        if condition is not None:
+            arr_new_infected = arr_new_infected & condition
+        rand = np.random.uniform(0, 1, (arr_new_infected.sum(),))
+        base_contaminate_vertices(arr_new_infected, rand, level)
+        self.host.df_population['inf_' + self.disease_name] = \
+            self.host.df_population['inf_' + self.disease_name] | arr_new_infected
+        if return_arr_newly_contaminated:
+            return arr_new_infected
```

### Comparing `sampy-abm-1.0.2/src/sampy/disease/single_species/builtin_disease.py` & `sampy_abm-1.0.3/src/sampy/disease/single_species/builtin_disease.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-from .base import BaseSingleSpeciesDisease
-from .transition import (TransitionCustomProbPermanentImmunity)
-from .transmission import TransmissionByContact
-from ...utils.decorators import sampy_class
-
-
-# todo: the name of this class is way too long. We need to find a short and expressive name
-@sampy_class
-class ContactCustomProbTransitionPermanentImmunity(BaseSingleSpeciesDisease,
-                                                   TransitionCustomProbPermanentImmunity,
-                                                   TransmissionByContact):
-    """
-    Basic disease, transmission by direct contact (contagion only between agents on the same vertex), transition between
-    disease states encoded by user given arrays of probabilities, and permanent immunity.
-
-    IMPORTANT: We strongly recommend the user to use the "simplified" methods defined here instead of the usual
-               'contaminate_vertices', 'contact_contagion' and 'transition_between_states'. Indeed, the combination of
-               building blocks involved in this disease requires many actions to be performed in a precise order,
-               otherwise the model's behaviour cannot be guaranteed. See each simplified method description to learn
-               about each respective ordering.
-
-    :param disease_name: mandatory kwargs. String.
-    :param host: mandatory kwargs. Population object of the host.
-    """
-    def __init__(self, **kwargs):
-        pass
-
-    def simplified_contaminate_vertices(self, list_vertices, level, arr_timesteps, arr_prob_timesteps,
-                                        condition=None, position_attribute='position',
-                                        return_arr_newly_contaminated=False):
-        """
-        Contaminate a list of vertices.
-
-        Detailed explanation: each agent has a series of counter attached, telling how much time-steps they will spend
-                              in each disease status. Those counters have to be initialized when an individual is newly
-                              infected, and that's what this method does to the newly infected individuals.
-
-        :param list_vertices: list of vertices ID to be contaminated.
-        :param level: float, probability for agent on the vertices to be contaminated.
-        :param arr_timesteps: 1D array of integer. Works in tandem with 'arr_prob_timesteps'. See below.
-        :param arr_prob_timesteps: 1D array of float. arr_prob_timesteps[i] is the probability for an agent to stay
-                                   infected but not contagious for arr_timesteps[i] timesteps.
-        :param condition: optional, array of bool, default None. If not None, say which agents are susceptible to be
-                          contaminated.
-        :param position_attribute: optional, string, default 'position'. Agent attribute to be used to define
-                                   their position.
-        :param return_arr_newly_contaminated: optional, boolean, default True. If True, the method returns an array
-                                              telling which agents were contaminated.
-
-        :return: if return_arr_newly_contaminated is set to True, returns a 1D array of bool. Returns None ortherwise.
-        """
-        #
-        arr_new_contaminated = self.contaminate_vertices(list_vertices, level, return_arr_newly_contaminated=True,
-                                                         condition=condition, position_attribute=position_attribute)
-        self.initialize_counters_of_newly_infected(arr_new_contaminated, arr_timesteps, arr_prob_timesteps)
-        if return_arr_newly_contaminated:
-            return arr_new_contaminated
-
-    def simplified_contact_contagion(self, contact_rate, arr_timesteps, arr_prob_timesteps,
-                                     position_attribute='position', condition=None,
-                                     return_arr_newly_contaminated=False):
-        """
-        Propagate the disease by direct contact using the following methodology. For any vertex X of the graph, we
-        count the number of contagious agents N_c, then each non immuned agent on the vertex X has a probability of
-
-                            1 - (1 - contact_rate) ** N_c
-
-        to become infected.
-
-        Detailed Explanation: each agent has a series of counter attached, telling how much time-steps they will spend
-                              in each disease status. Those counters have to be initialized when an individual is newly
-                              infected, and that's what this method does to the newly infected individuals.
-
-        :param contact_rate:
-        :param arr_timesteps: 1D array of integer. Works in tandem with 'arr_prob_timesteps'. See below.
-        :param arr_prob_timesteps: 1D array of float. arr_prob_timesteps[i] is the probability for an agent to stay
-                                   infected but not contagious for arr_timesteps[i] timesteps.
-        :param condition: optional, array of bool, default None. If not None, say which agents are susceptible to be
-                          contaminated.
-        :param position_attribute: optional, string, default 'position'. Agent attribute to be used to define
-                                   their position.
-        :param return_arr_newly_contaminated: optional, boolean, default True. If True, the method returns an array
-                                              telling which agents were contaminated.
-
-        :return: if return_arr_newly_contaminated is set to True, returns a 1D array of bool. Returns None ortherwise.
-        """
-        arr_new_contaminated = self.contact_contagion(contact_rate, position_attribute=position_attribute,
-                                                      condition=condition, return_arr_new_infected=True)
-        self.initialize_counters_of_newly_infected(arr_new_contaminated, arr_timesteps, arr_prob_timesteps)
-        if return_arr_newly_contaminated:
-            return arr_new_contaminated
-
-    def simplified_transition_between_states(self, prob_death, arr_infectious_period, arr_prob_infectious_period):
-        """
-        Takes care of the transition between all the disease states. That is, agents that are at the end of their
-        infected period become contagious and agents at the end of their contagious period either die (with a
-        probability of 'prob_death') or become immuned.
-
-        Detailed Explanation: the method transition_between_states is coded in such a way that when using it for
-                              transitionning from con to imm, all the agents at the end of their contagious period at
-                              the time the method is called transition. Therefore, we have to make the transition
-                              'con' to 'death' first.
-
-        :param prob_death: float between 0 and 1, probability for an agent to die at the end of the contagious period
-        :param arr_infectious_period: 1d array of int, works in tandem with arr_prob_infectious_period. See Below.
-        :param arr_prob_infectious_period: 1d array of floats, sums to 1. Same shape as arr_infectious_period.
-                    When an agent transition from infected to contagious, then arr_prob_infectious_period[i] is the
-                    probability for this agent to stay arr_infectious_period[i] timesteps contagious.
-        """
-        self.transition_between_states('con', 'death', proba_death=prob_death)
-
-        if self.host.df_population.nb_rows == 0:
-            return
-
-        self.transition_between_states('con', 'imm')
-        self.transition_between_states('inf', 'con', arr_nb_timestep=arr_infectious_period,
-                                       arr_prob_nb_timestep=arr_prob_infectious_period)
+from .base import BaseSingleSpeciesDisease
+from .transition import (TransitionCustomProbPermanentImmunity)
+from .transmission import TransmissionByContact
+from ...utils.decorators import sampy_class
+
+
+# todo: the name of this class is way too long. We need to find a short and expressive name
+@sampy_class
+class ContactCustomProbTransitionPermanentImmunity(BaseSingleSpeciesDisease,
+                                                   TransitionCustomProbPermanentImmunity,
+                                                   TransmissionByContact):
+    """
+    Basic disease, transmission by direct contact (contagion only between agents on the same vertex), transition between
+    disease states encoded by user given arrays of probabilities, and permanent immunity.
+
+    IMPORTANT: We strongly recommend the user to use the "simplified" methods defined here instead of the usual
+               'contaminate_vertices', 'contact_contagion' and 'transition_between_states'. Indeed, the combination of
+               building blocks involved in this disease requires many actions to be performed in a precise order,
+               otherwise the model's behaviour cannot be guaranteed. See each simplified method description to learn
+               about each respective ordering.
+
+    :param disease_name: mandatory kwargs. String.
+    :param host: mandatory kwargs. Population object of the host.
+    """
+    def __init__(self, **kwargs):
+        pass
+
+    def simplified_contaminate_vertices(self, list_vertices, level, arr_timesteps, arr_prob_timesteps,
+                                        condition=None, position_attribute='position',
+                                        return_arr_newly_contaminated=False):
+        """
+        Contaminate a list of vertices.
+
+        Detailed explanation: each agent has a series of counter attached, telling how much time-steps they will spend
+                              in each disease status. Those counters have to be initialized when an individual is newly
+                              infected, and that's what this method does to the newly infected individuals.
+
+        :param list_vertices: list of vertices ID to be contaminated.
+        :param level: float, probability for agent on the vertices to be contaminated.
+        :param arr_timesteps: 1D array of integer. Works in tandem with 'arr_prob_timesteps'. See below.
+        :param arr_prob_timesteps: 1D array of float. arr_prob_timesteps[i] is the probability for an agent to stay
+                                   infected but not contagious for arr_timesteps[i] timesteps.
+        :param condition: optional, array of bool, default None. If not None, say which agents are susceptible to be
+                          contaminated.
+        :param position_attribute: optional, string, default 'position'. Agent attribute to be used to define
+                                   their position.
+        :param return_arr_newly_contaminated: optional, boolean, default True. If True, the method returns an array
+                                              telling which agents were contaminated.
+
+        :return: if return_arr_newly_contaminated is set to True, returns a 1D array of bool. Returns None ortherwise.
+        """
+        #
+        arr_new_contaminated = self.contaminate_vertices(list_vertices, level, return_arr_newly_contaminated=True,
+                                                         condition=condition, position_attribute=position_attribute)
+        self.initialize_counters_of_newly_infected(arr_new_contaminated, arr_timesteps, arr_prob_timesteps)
+        if return_arr_newly_contaminated:
+            return arr_new_contaminated
+
+    def simplified_contact_contagion(self, contact_rate, arr_timesteps, arr_prob_timesteps,
+                                     position_attribute='position', condition=None,
+                                     return_arr_newly_contaminated=False):
+        """
+        Propagate the disease by direct contact using the following methodology. For any vertex X of the graph, we
+        count the number of contagious agents N_c, then each non immuned agent on the vertex X has a probability of
+
+                            1 - (1 - contact_rate) ** N_c
+
+        to become infected.
+
+        Detailed Explanation: each agent has a series of counter attached, telling how much time-steps they will spend
+                              in each disease status. Those counters have to be initialized when an individual is newly
+                              infected, and that's what this method does to the newly infected individuals.
+
+        :param contact_rate:
+        :param arr_timesteps: 1D array of integer. Works in tandem with 'arr_prob_timesteps'. See below.
+        :param arr_prob_timesteps: 1D array of float. arr_prob_timesteps[i] is the probability for an agent to stay
+                                   infected but not contagious for arr_timesteps[i] timesteps.
+        :param condition: optional, array of bool, default None. If not None, say which agents are susceptible to be
+                          contaminated.
+        :param position_attribute: optional, string, default 'position'. Agent attribute to be used to define
+                                   their position.
+        :param return_arr_newly_contaminated: optional, boolean, default True. If True, the method returns an array
+                                              telling which agents were contaminated.
+
+        :return: if return_arr_newly_contaminated is set to True, returns a 1D array of bool. Returns None ortherwise.
+        """
+        arr_new_contaminated = self.contact_contagion(contact_rate, position_attribute=position_attribute,
+                                                      condition=condition, return_arr_new_infected=True)
+        self.initialize_counters_of_newly_infected(arr_new_contaminated, arr_timesteps, arr_prob_timesteps)
+        if return_arr_newly_contaminated:
+            return arr_new_contaminated
+
+    def simplified_transition_between_states(self, prob_death, arr_infectious_period, arr_prob_infectious_period):
+        """
+        Takes care of the transition between all the disease states. That is, agents that are at the end of their
+        infected period become contagious and agents at the end of their contagious period either die (with a
+        probability of 'prob_death') or become immuned.
+
+        Detailed Explanation: the method transition_between_states is coded in such a way that when using it for
+                              transitionning from con to imm, all the agents at the end of their contagious period at
+                              the time the method is called transition. Therefore, we have to make the transition
+                              'con' to 'death' first.
+
+        :param prob_death: float between 0 and 1, probability for an agent to die at the end of the contagious period
+        :param arr_infectious_period: 1d array of int, works in tandem with arr_prob_infectious_period. See Below.
+        :param arr_prob_infectious_period: 1d array of floats, sums to 1. Same shape as arr_infectious_period.
+                    When an agent transition from infected to contagious, then arr_prob_infectious_period[i] is the
+                    probability for this agent to stay arr_infectious_period[i] timesteps contagious.
+        """
+        self.transition_between_states('con', 'death', proba_death=prob_death)
+
+        if self.host.df_population.nb_rows == 0:
+            return
+
+        self.transition_between_states('con', 'imm')
+        self.transition_between_states('inf', 'con', arr_nb_timestep=arr_infectious_period,
+                                       arr_prob_nb_timestep=arr_prob_infectious_period)
```

### Comparing `sampy-abm-1.0.2/src/sampy/disease/single_species/jit_compiled_functions.py` & `sampy_abm-1.0.3/src/sampy/disease/single_species/jit_compiled_functions.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-import numba as nb
-import numpy as np
-from numba.typed import List
-
-
-# ----------------------------------------------------------------------------------------------------------------------
-# generic functions
-@nb.njit
-def conditional_count_return_full_array(nb_vertex, arr_pos, arr_cond):
-    pos_count = np.zeros((nb_vertex,), dtype=np.int32)
-    for i in range(arr_pos.shape[0]):
-        if arr_cond[i]:
-            pos_count[arr_pos[i]] += 1
-    rv = np.zeros((arr_pos.shape[0],), dtype=np.int32)
-    for i in range(arr_pos.shape[0]):
-        rv[i] = pos_count[arr_pos[i]]
-    return rv
-
-# ----------------------------------------------------------------------------------------------------------------------
-# base
-
-
-@nb.njit
-def base_conditional_count_nb_agent_per_vertex(arr_condition, arr_pos, nb_vertex):
-    rv = np.zeros((nb_vertex,), dtype=np.int32)
-    for i in range(arr_pos.shape[0]):
-        if arr_condition[i]:
-            rv[arr_pos[i]] += 1
-    return rv
-
-
-@nb.njit
-def base_contaminate_vertices(arr_new_infected, rand, level):
-    counter = 0
-    for i in range(arr_new_infected.shape[0]):
-        if arr_new_infected[i]:
-            if rand[counter] >= level:
-                arr_new_infected[i] = False
-            counter += 1
-
-# ----------------------------------------------------------------------------------------------------------------------
-# transition
-
-
-@nb.njit
-def transition_initialize_counters_of_newly_infected(arr_new_infected, arr_cnt, arr_new_cnt):
-    counter = 0
-    for i in range(arr_new_infected.shape[0]):
-        if arr_new_infected[i]:
-            arr_cnt[i] = arr_new_cnt[counter]
-            counter += 1
-
-
-@nb.njit
-def transition_conditional_count_nb_agent_per_vertex(arr_condition, arr_pos, nb_vertex):
-    rv = np.zeros((nb_vertex,), dtype=np.int32)
-    for i in range(arr_pos.shape[0]):
-        if arr_condition[i]:
-            rv[arr_pos[i]] += 1
-    return rv
-
-
-@nb.njit
-def transition_falsify_when_condition(arr_bool, condition):
-    for i in range(arr_bool.shape[0]):
-        if condition[i]:
-            arr_bool[i] = False
-
-
-# ----------------------------------------------------------------------------------------------------------------------
-# transmission
-
-
-@nb.njit
-def transmission_contact_contagion_contact_tracing(arr_id, arr_pos, arr_con, rand_con, arr_new_infected, nb_vertex):
-    nb_new_infected = arr_new_infected.sum()
-
-    list_vert_id_con = List()
-    for i in range(nb_vertex):
-        con_on_pos_i = List()
-        con_on_pos_i.append(arr_id[0])
-        con_on_pos_i.pop()
-        list_vert_id_con.append(con_on_pos_i)
-
-    arr_nb_con_per_vertex = np.full((nb_vertex,), 0, dtype=np.int32)
-    for i in range(arr_id.shape[0]):
-        if arr_con[i]:
-            arr_nb_con_per_vertex[arr_pos[i]] += 1
-            list_vert_id_con[arr_pos[i]].append(arr_id[i])
-
-    rv_id = np.full((nb_new_infected,), 0, dtype=np.int32)
-    rv_con = np.full((nb_new_infected,), 0, dtype=np.int32)
-    counter = 0
-    for i in range(arr_new_infected.shape[0]):
-        if arr_new_infected[i]:
-            rand_index_con = int(np.floor(rand_con[counter] * arr_nb_con_per_vertex[arr_pos[i]])) % \
-                             arr_nb_con_per_vertex[arr_pos[i]]
-            rv_id[counter] = arr_id[i]
-            rv_con[counter] = list_vert_id_con[arr_pos[i]][rand_index_con]
-            counter += 1
-
-    return rv_id, rv_con
-
-
+import numba as nb
+import numpy as np
+from numba.typed import List
+
+
+# ----------------------------------------------------------------------------------------------------------------------
+# generic functions
+@nb.njit
+def conditional_count_return_full_array(nb_vertex, arr_pos, arr_cond):
+    pos_count = np.zeros((nb_vertex,), dtype=np.int32)
+    for i in range(arr_pos.shape[0]):
+        if arr_cond[i]:
+            pos_count[arr_pos[i]] += 1
+    rv = np.zeros((arr_pos.shape[0],), dtype=np.int32)
+    for i in range(arr_pos.shape[0]):
+        rv[i] = pos_count[arr_pos[i]]
+    return rv
+
+# ----------------------------------------------------------------------------------------------------------------------
+# base
+
+
+@nb.njit
+def base_conditional_count_nb_agent_per_vertex(arr_condition, arr_pos, nb_vertex):
+    rv = np.zeros((nb_vertex,), dtype=np.int32)
+    for i in range(arr_pos.shape[0]):
+        if arr_condition[i]:
+            rv[arr_pos[i]] += 1
+    return rv
+
+
+@nb.njit
+def base_contaminate_vertices(arr_new_infected, rand, level):
+    counter = 0
+    for i in range(arr_new_infected.shape[0]):
+        if arr_new_infected[i]:
+            if rand[counter] >= level:
+                arr_new_infected[i] = False
+            counter += 1
+
+# ----------------------------------------------------------------------------------------------------------------------
+# transition
+
+
+@nb.njit
+def transition_initialize_counters_of_newly_infected(arr_new_infected, arr_cnt, arr_new_cnt):
+    counter = 0
+    for i in range(arr_new_infected.shape[0]):
+        if arr_new_infected[i]:
+            arr_cnt[i] = arr_new_cnt[counter]
+            counter += 1
+
+
+@nb.njit
+def transition_conditional_count_nb_agent_per_vertex(arr_condition, arr_pos, nb_vertex):
+    rv = np.zeros((nb_vertex,), dtype=np.int32)
+    for i in range(arr_pos.shape[0]):
+        if arr_condition[i]:
+            rv[arr_pos[i]] += 1
+    return rv
+
+
+@nb.njit
+def transition_falsify_when_condition(arr_bool, condition):
+    for i in range(arr_bool.shape[0]):
+        if condition[i]:
+            arr_bool[i] = False
+
+
+# ----------------------------------------------------------------------------------------------------------------------
+# transmission
+
+
+@nb.njit
+def transmission_contact_contagion_contact_tracing(arr_id, arr_pos, arr_con, rand_con, arr_new_infected, nb_vertex):
+    nb_new_infected = arr_new_infected.sum()
+
+    list_vert_id_con = List()
+    for i in range(nb_vertex):
+        con_on_pos_i = List()
+        con_on_pos_i.append(arr_id[0])
+        con_on_pos_i.pop()
+        list_vert_id_con.append(con_on_pos_i)
+
+    arr_nb_con_per_vertex = np.full((nb_vertex,), 0, dtype=np.int32)
+    for i in range(arr_id.shape[0]):
+        if arr_con[i]:
+            arr_nb_con_per_vertex[arr_pos[i]] += 1
+            list_vert_id_con[arr_pos[i]].append(arr_id[i])
+
+    rv_id = np.full((nb_new_infected,), 0, dtype=np.int32)
+    rv_con = np.full((nb_new_infected,), 0, dtype=np.int32)
+    counter = 0
+    for i in range(arr_new_infected.shape[0]):
+        if arr_new_infected[i]:
+            rand_index_con = int(np.floor(rand_con[counter] * arr_nb_con_per_vertex[arr_pos[i]])) % \
+                             arr_nb_con_per_vertex[arr_pos[i]]
+            rv_id[counter] = arr_id[i]
+            rv_con[counter] = list_vert_id_con[arr_pos[i]][rand_index_con]
+            counter += 1
+
+    return rv_id, rv_con
+
+
```

### Comparing `sampy-abm-1.0.2/src/sampy/disease/single_species/transition.py` & `sampy_abm-1.0.3/src/sampy/disease/single_species/transition.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,352 +1,352 @@
-import numpy as np
-from .jit_compiled_functions import *
-from ...utils.errors_shortcut import (check_input_array,
-                                      check_col_exists_good_type)
-
-
-class TransitionCustomProbPermanentImmunity:
-    """
-    This class introduce transitions between disease states based on probabilities given by the user.
-
-    WARNING: be aware that the time each agent spend in each status of the disease is kept in memory using counters.
-             Those counters HAVE TO be initialized for newly infected individuals throught the use of the method
-             'initialize_counters_of_newly_infected'. This problem is addressed by the 'simplified' methods in Sampy
-             built-in diseases.
-    """
-    def __init__(self, **kwargs):
-        self.host.df_population['cnt_inf_' + self.disease_name] = 0
-        self.host.dict_default_val['cnt_inf_' + self.disease_name] = 0
-
-        self.host.df_population['cnt_con_' + self.disease_name] = 0
-        self.host.dict_default_val['cnt_con_' + self.disease_name] = 0
-
-        self.on_ticker.append('decrement_counter')
-
-    def _sampy_debug_initialize_counters_of_newly_infected(self, arr_new_infected, arr_nb_timestep, arr_prob):
-        if self.host.df_population.nb_rows == 0:
-            return
-
-        check_input_array(arr_new_infected, 'arr_new_infected', 'bool',
-                          shape=(self.host.df_population.nb_rows,))
-        check_input_array(arr_nb_timestep, 'arr_nb_timestep', 'int', nb_dim=1)
-        check_input_array(arr_prob, 'arr_prob', 'float', nb_dim=1)
-
-        if arr_prob.shape != arr_nb_timestep.shape:
-            raise ValueError("Arguments 'arr_nb_timestep' and 'arr_prob' have different shapes.")
-
-    def initialize_counters_of_newly_infected(self, arr_new_infected, arr_nb_timestep, arr_prob):
-        """
-        Method that HAS TO be called each time new individuals get infected
-
-        :param arr_new_infected: 1d array of bool, saying which agent are newly infected and should have their
-                                 'infectious status counter' initialized.
-        :param arr_nb_timestep: 1d array of int. work in tandem with arr_prob, see below.
-        :param arr_prob: 1D array of float. arr_prob[i] is the probability for an agent to stay infected but not
-                         contagious for arr_nb_timestep[i] time-steps.
-
-        """
-        if self.host.df_population.nb_rows == 0:
-            return
-        prob = arr_prob.astype('float64')
-        prob = prob/prob.sum()
-        arr_cnt = np.random.choice(arr_nb_timestep, arr_new_infected.sum(), p=prob)
-
-        transition_initialize_counters_of_newly_infected(arr_new_infected,
-                                                         self.host.df_population['cnt_inf_' + self.disease_name],
-                                                         arr_cnt)
-
-    def decrement_counter(self):
-        """
-        Reduce by one the counters of the agents in a given disease state. Note that this method will only decrease
-        positive counters, so that if a negative counter was to appear, which shouldn't, this should be caused by
-        something else.
-        """
-        if self.host.df_population.nb_rows == 0:
-            return
-        self.host.df_population['cnt_inf_' + self.disease_name] -= self.host.df_population['inf_' + self.disease_name] & \
-                                                        (self.host.df_population['cnt_inf_' + self.disease_name] > 0)
-        self.host.df_population['cnt_con_' + self.disease_name] -= self.host.df_population['con_' + self.disease_name] & \
-                                                        (self.host.df_population['cnt_con_' + self.disease_name] > 0)
-
-    def _sampy_debug_transition_between_states(self, initial_state, target_state, condition=None, proba_death=1.,
-                                               arr_nb_timestep=None, arr_prob_nb_timestep=None,
-                                               return_transition_count=False, position_attribute='position'):
-        if self.host.df_population.nb_rows == 0:
-            return
-
-        if initial_state not in self.set_disease_status:
-            raise ValueError("Initial state is not in " + str(self.set_disease_status) + ".")
-        if target_state not in self.set_disease_status and target_state != 'death':
-            raise ValueError("Initial state is not in " + str(self.set_disease_status | {'death'}) + ".")
-
-        if condition is not None:
-            check_input_array(condition, 'condition', 'bool', shape=(self.host.df_population.nb_rows,))
-
-        if arr_nb_timestep is None and arr_prob_nb_timestep is not None:
-            raise ValueError("'arr_nb_timestep' is None while 'arr_prob_nb_timestep' is not.")
-
-        if arr_nb_timestep is not None and arr_prob_nb_timestep is None:
-            raise ValueError("'arr_prob_nb_timestep' is None while 'arr_nb_timestep' is not.")
-
-        if arr_nb_timestep is not None:
-            check_input_array(arr_nb_timestep, 'arr_nb_timestep', 'int', nb_dim=1)
-            check_input_array(arr_prob_nb_timestep, 'arr_prob_nb_timestep', 'float', nb_dim=1)
-            if arr_nb_timestep.shape != arr_prob_nb_timestep.shape:
-                raise ValueError("Arguments 'arr_nb_timestep' and 'arr_prob_nb_timestep' have different shapes.")
-
-        check_col_exists_good_type(self.host.df_population, position_attribute, 'position_attribute',
-                                   prefix_dtype='int', reject_none=True)
-
-    def transition_between_states(self, initial_state, target_state, condition=None, proba_death=1.,
-                                  arr_nb_timestep=None, arr_prob_nb_timestep=None, return_transition_count=False,
-                                  position_attribute='position'):
-        """
-        Performs the transition from an initial_state to a target_state of the disease, where 'death' is a possible
-        target_state. When performing the transition, each agent for which 'initial_state' is True and the associated
-        counter is 0 makes the transition (except if the target state is death proba_death is smaller than 1.).
-
-        WARNING: note that an agent can only be in a SINGLE state. That is, an agent cannot be simultaneously 'infected'
-                 and 'contagious'. So if the user wants, for instance, to count all agents carrying the disease, then
-                 both 'inf' and 'con' states have to be considered.
-
-        :param initial_state: string, in ['inf', 'con', 'imm']
-        :param target_state: string, in ['con', 'imm', 'death']
-        :param proba_death: optional, float, default 1.0. Probability of death if target_state=death.
-        :param arr_nb_timestep: optional, 1d array of int, default None.
-        :param arr_prob_nb_timestep: optional, 1d array of float, default None.
-        :param return_transition_count: optional, bool, default False. If True, returns a 1D array of integer counting
-                                        how many agents did the transition per cell.
-        :param position_attribute: optional, string, default 'position'. Name of the position attribute used for counting
-                                   if 'return_transition_count' is set to True.
-
-        :returns: if return_transition_count is True, returns a 1d array of int. Else, returns None.
-        """
-        if self.host.df_population.nb_rows == 0:
-            return
-
-        # bool array of all individuals that will make transition
-        susceptible = self.host.df_population['cnt_' + initial_state + '_' + self.disease_name] == 0
-        susceptible = susceptible & self.host.df_population[initial_state + '_' + self.disease_name]
-        if condition is not None:
-            susceptible = susceptible & condition
-
-        count_arr = None
-
-        # in case of death
-        if target_state == 'death':
-            # there might be a probability of dying of the disease, which is taken into account now
-            if proba_death < 1.:
-                susceptible = susceptible & \
-                              (np.random.uniform(0, 1, (self.host.df_population.shape[0],)) < proba_death)
-
-            if return_transition_count:
-                count_arr = transition_conditional_count_nb_agent_per_vertex(susceptible,
-                                                                             self.host.df_population[
-                                                                                 position_attribute],
-                                                                             self.host.graph.weights.shape[0])
-
-            # killing
-            self.host.df_population = self.host.df_population[~susceptible]
-
-        # all the rest corresponds to transition between stages of the disease
-        else:
-            if return_transition_count:
-                count_arr = transition_conditional_count_nb_agent_per_vertex(susceptible,
-                                                                             self.host.df_population[
-                                                                                 position_attribute],
-                                                                             self.host.graph.weights.shape[0])
-
-            self.host.df_population[target_state + '_' + self.disease_name] = susceptible | self.host.df_population[
-                                                                                target_state + '_' + self.disease_name]
-            if target_state == 'imm':
-                transition_falsify_when_condition(self.host.df_population['inf_' + self.disease_name], susceptible)
-                transition_falsify_when_condition(self.host.df_population['con_' + self.disease_name], susceptible)
-
-            else:
-                transition_falsify_when_condition(self.host.df_population[initial_state + '_' + self.disease_name],
-                                                  susceptible)
-
-                prob = arr_prob_nb_timestep.astype('float64')
-                prob = prob / prob.sum()
-                arr_cnt = np.random.choice(arr_nb_timestep, susceptible.sum(), p=prob)
-
-                transition_initialize_counters_of_newly_infected(susceptible,
-                                                                 self.host.df_population[
-                                                                     'cnt_' + target_state + '_' + self.disease_name],
-                                                                 arr_cnt)
-        return count_arr
-
-
-class TransitionCustomProbFiniteImmunity:
-    """
-    This class introduce transitions between disease states based on probabilities given by the user. Immunity is
-    not permanent.
-
-    WARNING: be aware that the time each agent spend in each status of the disease is kept in memory using counters.
-             Those counters HAVE TO be initialized for newly infected individuals throught the use of the method
-             'initialize_counters_of_newly_infected'. This is a current problem of Sampy that the user has to
-             explicitly call a method that should be automatically called in the background. This issue will be
-             adressed in the future once a satisfactory design solution has been found (here, satisfactory means
-             'that doesn't create too much special cases that developers working on Sampy have to keep in mind').
-    """
-    def __init__(self, **kwargs):
-        self.host.df_population['cnt_inf_' + self.disease_name] = 0
-        self.host.dict_default_val['cnt_inf_' + self.disease_name] = 0
-
-        self.host.df_population['cnt_con_' + self.disease_name] = 0
-        self.host.dict_default_val['cnt_con_' + self.disease_name] = 0
-
-        self.host.df_population['cnt_imm_' + self.disease_name] = 0
-        self.host.dict_default_val['cnt_imm_' + self.disease_name] = 0
-
-    def _sampy_debug_initialize_counters_of_newly_infected(self, arr_new_infected, arr_nb_timestep, arr_prob):
-        if self.host.df_population.nb_rows == 0:
-            return
-
-        check_input_array(arr_new_infected, 'arr_new_infected', 'bool',
-                          shape=(self.host.df_population.nb_rows,))
-        check_input_array(arr_nb_timestep, 'arr_nb_timestep', 'int', nb_dim=1)
-        check_input_array(arr_prob, 'arr_prob', 'float', nb_dim=1)
-
-        if arr_prob.shape != arr_nb_timestep:
-            raise ValueError("Arguments 'arr_nb_timestep' and 'arr_prob' have different shapes.")
-
-    def initialize_counters_of_newly_infected(self, arr_new_infected, arr_nb_timestep, arr_prob):
-        """
-        Method that HAS TO be called each time new individuals get infected
-
-        :param arr_new_infected: 1d array of bool, saying which agent are newly infected and should have their
-                                 'infectious status counter' initialized.
-        :param arr_nb_timestep: 1d array of int.
-        :param arr_prob: 1d array of non negative floats, will be normalized to sum to 1.
-
-        """
-        if self.host.df_population.nb_rows == 0:
-            return
-        prob = arr_prob.astype('float64')
-        prob = prob/prob.sum()
-        arr_cnt = np.random.choice(arr_nb_timestep, arr_new_infected.sum(), p=prob)
-
-        transition_initialize_counters_of_newly_infected(arr_new_infected,
-                                                         self.host.df_population['cnt_inf_' + self.disease_name],
-                                                         arr_cnt)
-
-    def decrement_counter(self):
-        """
-        Reduce by one the counters of the agents in a given disease state. Note that this method will only decrease
-        positive counters, so that if a negative counter was to appear, which shouldn't, this should be caused by
-        something else.
-        """
-        if self.host.df_population.nb_rows == 0:
-            return
-        self.host.df_population['cnt_inf_' + self.disease_name] -= self.host.df_population['inf_' + self.disease_name] & \
-                                                        (self.host.df_population['cnt_inf_' + self.disease_name] > 0)
-        self.host.df_population['cnt_con_' + self.disease_name] -= self.host.df_population['con_' + self.disease_name] & \
-                                                        (self.host.df_population['cnt_con_' + self.disease_name] > 0)
-        self.host.df_population['cnt_imm_' + self.disease_name] -= self.host.df_population['imm_' + self.disease_name] & \
-                                                                   (self.host.df_population[
-                                                                        'cnt_imm_' + self.disease_name] > 0)
-
-    def _sampy_debug_transition_between_states(self, initial_state, target_state, condition=None, proba_death=1.,
-                                               arr_nb_timestep=None, arr_prob_nb_timestep=None,
-                                               return_transition_count=False, position_attribute='position'):
-        if self.host.df_population.nb_rows == 0:
-            return
-
-        if initial_state not in self.set_disease_status:
-            raise ValueError("Initial state is not in " + str(self.set_disease_status) + ".")
-        if target_state not in self.set_disease_status and target_state != 'death':
-            raise ValueError("Initial state is not in " + str(self.set_disease_status | {'death'}) + ".")
-
-        if condition is not None:
-            check_input_array(condition, 'condition', 'bool', shape=(self.host.df_population.nb_rows,))
-
-        if arr_nb_timestep is None and arr_prob_nb_timestep is not None:
-            raise ValueError("'arr_nb_timestep' is None while 'arr_prob_nb_timestep' is not.")
-
-        if arr_nb_timestep is not None and arr_prob_nb_timestep is None:
-            raise ValueError("'arr_prob_nb_timestep' is None while 'arr_nb_timestep' is not.")
-
-        if arr_nb_timestep is not None:
-            check_input_array(arr_nb_timestep, 'arr_nb_timestep', 'int', nb_dim=1)
-            check_input_array(arr_prob_nb_timestep, 'arr_prob_nb_timestep', 'float', nb_dim=1)
-            if arr_nb_timestep.shape != arr_prob_nb_timestep.shape:
-                raise ValueError("Arguments 'arr_nb_timestep' and 'arr_prob_nb_timestep' have different shapes.")
-
-        check_col_exists_good_type(self.host.df_population, position_attribute, 'position_attribute',
-                                   prefix_dtype='int', reject_none=True)
-
-    def transition_between_states(self, initial_state, target_state, condition=None, proba_death=1.,
-                                  arr_nb_timestep=None, arr_prob_nb_timestep=None, return_transition_count=False,
-                                  position_attribute='position'):
-        """
-        Performs the transition from an initial_state to a target_state of the disease, where 'death' is a possible
-        target_state. When performing the transition, each agent for which 'initial_state' is True and the associated
-        counter is 0 makes the transition (except if the target state is death and proba_death is smaller than 1.).
-
-        WARNING: note that an agent can only be in a SINGLE state. That is, an agent cannot be simultaneously 'infected'
-                 and 'contagious'. So if the user wants, for instance, to count all agents carrying the disease, then
-                 both 'inf' and 'con' states have to be considered.
-
-        :param initial_state: string, in ['inf', 'con', 'imm']
-        :param target_state: string, in ['con', 'imm', 'death']
-        :param proba_death: optional, float, default 1.0. Probability of death if target_state=death.
-        :param arr_nb_timestep: optional, 1d array of int, default None.
-        :param arr_prob_nb_timestep: optional, 1d array of float, default None.
-        :param return_transition_count: optional, bool, default False. If True, returns a 1D array of integer counting
-                                        how many agents did the transition per cell.
-        :param position_attribute: optional, string, default 'position'. Name of the position attribute used for counting
-                                   if 'return_transition_count' is set to True.
-
-        :returns: if return_transition_count is True, returns a 1d array of int. Else, returns None.
-        """
-        if self.host.df_population.nb_rows == 0:
-            return
-
-        # bool array of all individuals that will make transition
-        susceptible = self.host.df_population['cnt_' + initial_state + '_' + self.disease_name] == 0
-        susceptible = susceptible & self.host.df_population[initial_state + '_' + self.disease_name]
-        if condition is not None:
-            susceptible = susceptible & condition
-
-        count_arr = None
-
-        # in case of death
-        if target_state == 'death':
-            # there might be a probability of dying of the disease, which is taken into account now
-            if proba_death < 1.:
-                susceptible = susceptible & \
-                              (np.random.uniform(0, 1, (self.host.df_population.shape[0],)) < proba_death)
-
-            if return_transition_count:
-                count_arr = transition_conditional_count_nb_agent_per_vertex(susceptible,
-                                                                             self.host.df_population[
-                                                                                 position_attribute],
-                                                                             self.host.graph.weights.shape[0])
-
-            # killing
-            self.host.df_population = self.host.df_population[~susceptible]
-
-        # all the rest corresponds to transition between stages of the disease
-        else:
-            if return_transition_count:
-                count_arr = transition_conditional_count_nb_agent_per_vertex(susceptible,
-                                                                             self.host.df_population[
-                                                                                 position_attribute],
-                                                                             self.host.graph.weights.shape[0])
-
-            self.host.df_population[target_state + '_' + self.disease_name] = susceptible | self.host.df_population[
-                                                                                target_state + '_' + self.disease_name]
-
-            transition_falsify_when_condition(self.host.df_population[initial_state + '_' + self.disease_name],
-                                              susceptible)
-
-            prob = arr_prob_nb_timestep.astype('float64')
-            prob = prob / prob.sum()
-            arr_cnt = np.random.choice(arr_nb_timestep, susceptible.sum(), p=prob)
-
-            transition_initialize_counters_of_newly_infected(susceptible,
-                                                             self.host.df_population[
-                                                                 'cnt_' + target_state + '_' + self.disease_name],
-                                                             arr_cnt)
-        return count_arr
+import numpy as np
+from .jit_compiled_functions import *
+from ...utils.errors_shortcut import (check_input_array,
+                                      check_col_exists_good_type)
+
+
+class TransitionCustomProbPermanentImmunity:
+    """
+    This class introduce transitions between disease states based on probabilities given by the user.
+
+    WARNING: be aware that the time each agent spend in each status of the disease is kept in memory using counters.
+             Those counters HAVE TO be initialized for newly infected individuals throught the use of the method
+             'initialize_counters_of_newly_infected'. This problem is addressed by the 'simplified' methods in Sampy
+             built-in diseases.
+    """
+    def __init__(self, **kwargs):
+        self.host.df_population['cnt_inf_' + self.disease_name] = 0
+        self.host.dict_default_val['cnt_inf_' + self.disease_name] = 0
+
+        self.host.df_population['cnt_con_' + self.disease_name] = 0
+        self.host.dict_default_val['cnt_con_' + self.disease_name] = 0
+
+        self.on_ticker.append('decrement_counter')
+
+    def _sampy_debug_initialize_counters_of_newly_infected(self, arr_new_infected, arr_nb_timestep, arr_prob):
+        if self.host.df_population.nb_rows == 0:
+            return
+
+        check_input_array(arr_new_infected, 'arr_new_infected', 'bool',
+                          shape=(self.host.df_population.nb_rows,))
+        check_input_array(arr_nb_timestep, 'arr_nb_timestep', 'int', nb_dim=1)
+        check_input_array(arr_prob, 'arr_prob', 'float', nb_dim=1)
+
+        if arr_prob.shape != arr_nb_timestep.shape:
+            raise ValueError("Arguments 'arr_nb_timestep' and 'arr_prob' have different shapes.")
+
+    def initialize_counters_of_newly_infected(self, arr_new_infected, arr_nb_timestep, arr_prob):
+        """
+        Method that HAS TO be called each time new individuals get infected
+
+        :param arr_new_infected: 1d array of bool, saying which agent are newly infected and should have their
+                                 'infectious status counter' initialized.
+        :param arr_nb_timestep: 1d array of int. work in tandem with arr_prob, see below.
+        :param arr_prob: 1D array of float. arr_prob[i] is the probability for an agent to stay infected but not
+                         contagious for arr_nb_timestep[i] time-steps.
+
+        """
+        if self.host.df_population.nb_rows == 0:
+            return
+        prob = arr_prob.astype('float64')
+        prob = prob/prob.sum()
+        arr_cnt = np.random.choice(arr_nb_timestep, arr_new_infected.sum(), p=prob)
+
+        transition_initialize_counters_of_newly_infected(arr_new_infected,
+                                                         self.host.df_population['cnt_inf_' + self.disease_name],
+                                                         arr_cnt)
+
+    def decrement_counter(self):
+        """
+        Reduce by one the counters of the agents in a given disease state. Note that this method will only decrease
+        positive counters, so that if a negative counter was to appear, which shouldn't, this should be caused by
+        something else.
+        """
+        if self.host.df_population.nb_rows == 0:
+            return
+        self.host.df_population['cnt_inf_' + self.disease_name] -= self.host.df_population['inf_' + self.disease_name] & \
+                                                        (self.host.df_population['cnt_inf_' + self.disease_name] > 0)
+        self.host.df_population['cnt_con_' + self.disease_name] -= self.host.df_population['con_' + self.disease_name] & \
+                                                        (self.host.df_population['cnt_con_' + self.disease_name] > 0)
+
+    def _sampy_debug_transition_between_states(self, initial_state, target_state, condition=None, proba_death=1.,
+                                               arr_nb_timestep=None, arr_prob_nb_timestep=None,
+                                               return_transition_count=False, position_attribute='position'):
+        if self.host.df_population.nb_rows == 0:
+            return
+
+        if initial_state not in self.set_disease_status:
+            raise ValueError("Initial state is not in " + str(self.set_disease_status) + ".")
+        if target_state not in self.set_disease_status and target_state != 'death':
+            raise ValueError("Initial state is not in " + str(self.set_disease_status | {'death'}) + ".")
+
+        if condition is not None:
+            check_input_array(condition, 'condition', 'bool', shape=(self.host.df_population.nb_rows,))
+
+        if arr_nb_timestep is None and arr_prob_nb_timestep is not None:
+            raise ValueError("'arr_nb_timestep' is None while 'arr_prob_nb_timestep' is not.")
+
+        if arr_nb_timestep is not None and arr_prob_nb_timestep is None:
+            raise ValueError("'arr_prob_nb_timestep' is None while 'arr_nb_timestep' is not.")
+
+        if arr_nb_timestep is not None:
+            check_input_array(arr_nb_timestep, 'arr_nb_timestep', 'int', nb_dim=1)
+            check_input_array(arr_prob_nb_timestep, 'arr_prob_nb_timestep', 'float', nb_dim=1)
+            if arr_nb_timestep.shape != arr_prob_nb_timestep.shape:
+                raise ValueError("Arguments 'arr_nb_timestep' and 'arr_prob_nb_timestep' have different shapes.")
+
+        check_col_exists_good_type(self.host.df_population, position_attribute, 'position_attribute',
+                                   prefix_dtype='int', reject_none=True)
+
+    def transition_between_states(self, initial_state, target_state, condition=None, proba_death=1.,
+                                  arr_nb_timestep=None, arr_prob_nb_timestep=None, return_transition_count=False,
+                                  position_attribute='position'):
+        """
+        Performs the transition from an initial_state to a target_state of the disease, where 'death' is a possible
+        target_state. When performing the transition, each agent for which 'initial_state' is True and the associated
+        counter is 0 makes the transition (except if the target state is death proba_death is smaller than 1.).
+
+        WARNING: note that an agent can only be in a SINGLE state. That is, an agent cannot be simultaneously 'infected'
+                 and 'contagious'. So if the user wants, for instance, to count all agents carrying the disease, then
+                 both 'inf' and 'con' states have to be considered.
+
+        :param initial_state: string, in ['inf', 'con', 'imm']
+        :param target_state: string, in ['con', 'imm', 'death']
+        :param proba_death: optional, float, default 1.0. Probability of death if target_state=death.
+        :param arr_nb_timestep: optional, 1d array of int, default None.
+        :param arr_prob_nb_timestep: optional, 1d array of float, default None.
+        :param return_transition_count: optional, bool, default False. If True, returns a 1D array of integer counting
+                                        how many agents did the transition per cell.
+        :param position_attribute: optional, string, default 'position'. Name of the position attribute used for counting
+                                   if 'return_transition_count' is set to True.
+
+        :returns: if return_transition_count is True, returns a 1d array of int. Else, returns None.
+        """
+        if self.host.df_population.nb_rows == 0:
+            return
+
+        # bool array of all individuals that will make transition
+        susceptible = self.host.df_population['cnt_' + initial_state + '_' + self.disease_name] == 0
+        susceptible = susceptible & self.host.df_population[initial_state + '_' + self.disease_name]
+        if condition is not None:
+            susceptible = susceptible & condition
+
+        count_arr = None
+
+        # in case of death
+        if target_state == 'death':
+            # there might be a probability of dying of the disease, which is taken into account now
+            if proba_death < 1.:
+                susceptible = susceptible & \
+                              (np.random.uniform(0, 1, (self.host.df_population.shape[0],)) < proba_death)
+
+            if return_transition_count:
+                count_arr = transition_conditional_count_nb_agent_per_vertex(susceptible,
+                                                                             self.host.df_population[
+                                                                                 position_attribute],
+                                                                             self.host.graph.weights.shape[0])
+
+            # killing
+            self.host.df_population = self.host.df_population[~susceptible]
+
+        # all the rest corresponds to transition between stages of the disease
+        else:
+            if return_transition_count:
+                count_arr = transition_conditional_count_nb_agent_per_vertex(susceptible,
+                                                                             self.host.df_population[
+                                                                                 position_attribute],
+                                                                             self.host.graph.weights.shape[0])
+
+            self.host.df_population[target_state + '_' + self.disease_name] = susceptible | self.host.df_population[
+                                                                                target_state + '_' + self.disease_name]
+            if target_state == 'imm':
+                transition_falsify_when_condition(self.host.df_population['inf_' + self.disease_name], susceptible)
+                transition_falsify_when_condition(self.host.df_population['con_' + self.disease_name], susceptible)
+
+            else:
+                transition_falsify_when_condition(self.host.df_population[initial_state + '_' + self.disease_name],
+                                                  susceptible)
+
+                prob = arr_prob_nb_timestep.astype('float64')
+                prob = prob / prob.sum()
+                arr_cnt = np.random.choice(arr_nb_timestep, susceptible.sum(), p=prob)
+
+                transition_initialize_counters_of_newly_infected(susceptible,
+                                                                 self.host.df_population[
+                                                                     'cnt_' + target_state + '_' + self.disease_name],
+                                                                 arr_cnt)
+        return count_arr
+
+
+class TransitionCustomProbFiniteImmunity:
+    """
+    This class introduce transitions between disease states based on probabilities given by the user. Immunity is
+    not permanent.
+
+    WARNING: be aware that the time each agent spend in each status of the disease is kept in memory using counters.
+             Those counters HAVE TO be initialized for newly infected individuals throught the use of the method
+             'initialize_counters_of_newly_infected'. This is a current problem of Sampy that the user has to
+             explicitly call a method that should be automatically called in the background. This issue will be
+             adressed in the future once a satisfactory design solution has been found (here, satisfactory means
+             'that doesn't create too much special cases that developers working on Sampy have to keep in mind').
+    """
+    def __init__(self, **kwargs):
+        self.host.df_population['cnt_inf_' + self.disease_name] = 0
+        self.host.dict_default_val['cnt_inf_' + self.disease_name] = 0
+
+        self.host.df_population['cnt_con_' + self.disease_name] = 0
+        self.host.dict_default_val['cnt_con_' + self.disease_name] = 0
+
+        self.host.df_population['cnt_imm_' + self.disease_name] = 0
+        self.host.dict_default_val['cnt_imm_' + self.disease_name] = 0
+
+    def _sampy_debug_initialize_counters_of_newly_infected(self, arr_new_infected, arr_nb_timestep, arr_prob):
+        if self.host.df_population.nb_rows == 0:
+            return
+
+        check_input_array(arr_new_infected, 'arr_new_infected', 'bool',
+                          shape=(self.host.df_population.nb_rows,))
+        check_input_array(arr_nb_timestep, 'arr_nb_timestep', 'int', nb_dim=1)
+        check_input_array(arr_prob, 'arr_prob', 'float', nb_dim=1)
+
+        if arr_prob.shape != arr_nb_timestep:
+            raise ValueError("Arguments 'arr_nb_timestep' and 'arr_prob' have different shapes.")
+
+    def initialize_counters_of_newly_infected(self, arr_new_infected, arr_nb_timestep, arr_prob):
+        """
+        Method that HAS TO be called each time new individuals get infected
+
+        :param arr_new_infected: 1d array of bool, saying which agent are newly infected and should have their
+                                 'infectious status counter' initialized.
+        :param arr_nb_timestep: 1d array of int.
+        :param arr_prob: 1d array of non negative floats, will be normalized to sum to 1.
+
+        """
+        if self.host.df_population.nb_rows == 0:
+            return
+        prob = arr_prob.astype('float64')
+        prob = prob/prob.sum()
+        arr_cnt = np.random.choice(arr_nb_timestep, arr_new_infected.sum(), p=prob)
+
+        transition_initialize_counters_of_newly_infected(arr_new_infected,
+                                                         self.host.df_population['cnt_inf_' + self.disease_name],
+                                                         arr_cnt)
+
+    def decrement_counter(self):
+        """
+        Reduce by one the counters of the agents in a given disease state. Note that this method will only decrease
+        positive counters, so that if a negative counter was to appear, which shouldn't, this should be caused by
+        something else.
+        """
+        if self.host.df_population.nb_rows == 0:
+            return
+        self.host.df_population['cnt_inf_' + self.disease_name] -= self.host.df_population['inf_' + self.disease_name] & \
+                                                        (self.host.df_population['cnt_inf_' + self.disease_name] > 0)
+        self.host.df_population['cnt_con_' + self.disease_name] -= self.host.df_population['con_' + self.disease_name] & \
+                                                        (self.host.df_population['cnt_con_' + self.disease_name] > 0)
+        self.host.df_population['cnt_imm_' + self.disease_name] -= self.host.df_population['imm_' + self.disease_name] & \
+                                                                   (self.host.df_population[
+                                                                        'cnt_imm_' + self.disease_name] > 0)
+
+    def _sampy_debug_transition_between_states(self, initial_state, target_state, condition=None, proba_death=1.,
+                                               arr_nb_timestep=None, arr_prob_nb_timestep=None,
+                                               return_transition_count=False, position_attribute='position'):
+        if self.host.df_population.nb_rows == 0:
+            return
+
+        if initial_state not in self.set_disease_status:
+            raise ValueError("Initial state is not in " + str(self.set_disease_status) + ".")
+        if target_state not in self.set_disease_status and target_state != 'death':
+            raise ValueError("Initial state is not in " + str(self.set_disease_status | {'death'}) + ".")
+
+        if condition is not None:
+            check_input_array(condition, 'condition', 'bool', shape=(self.host.df_population.nb_rows,))
+
+        if arr_nb_timestep is None and arr_prob_nb_timestep is not None:
+            raise ValueError("'arr_nb_timestep' is None while 'arr_prob_nb_timestep' is not.")
+
+        if arr_nb_timestep is not None and arr_prob_nb_timestep is None:
+            raise ValueError("'arr_prob_nb_timestep' is None while 'arr_nb_timestep' is not.")
+
+        if arr_nb_timestep is not None:
+            check_input_array(arr_nb_timestep, 'arr_nb_timestep', 'int', nb_dim=1)
+            check_input_array(arr_prob_nb_timestep, 'arr_prob_nb_timestep', 'float', nb_dim=1)
+            if arr_nb_timestep.shape != arr_prob_nb_timestep.shape:
+                raise ValueError("Arguments 'arr_nb_timestep' and 'arr_prob_nb_timestep' have different shapes.")
+
+        check_col_exists_good_type(self.host.df_population, position_attribute, 'position_attribute',
+                                   prefix_dtype='int', reject_none=True)
+
+    def transition_between_states(self, initial_state, target_state, condition=None, proba_death=1.,
+                                  arr_nb_timestep=None, arr_prob_nb_timestep=None, return_transition_count=False,
+                                  position_attribute='position'):
+        """
+        Performs the transition from an initial_state to a target_state of the disease, where 'death' is a possible
+        target_state. When performing the transition, each agent for which 'initial_state' is True and the associated
+        counter is 0 makes the transition (except if the target state is death and proba_death is smaller than 1.).
+
+        WARNING: note that an agent can only be in a SINGLE state. That is, an agent cannot be simultaneously 'infected'
+                 and 'contagious'. So if the user wants, for instance, to count all agents carrying the disease, then
+                 both 'inf' and 'con' states have to be considered.
+
+        :param initial_state: string, in ['inf', 'con', 'imm']
+        :param target_state: string, in ['con', 'imm', 'death']
+        :param proba_death: optional, float, default 1.0. Probability of death if target_state=death.
+        :param arr_nb_timestep: optional, 1d array of int, default None.
+        :param arr_prob_nb_timestep: optional, 1d array of float, default None.
+        :param return_transition_count: optional, bool, default False. If True, returns a 1D array of integer counting
+                                        how many agents did the transition per cell.
+        :param position_attribute: optional, string, default 'position'. Name of the position attribute used for counting
+                                   if 'return_transition_count' is set to True.
+
+        :returns: if return_transition_count is True, returns a 1d array of int. Else, returns None.
+        """
+        if self.host.df_population.nb_rows == 0:
+            return
+
+        # bool array of all individuals that will make transition
+        susceptible = self.host.df_population['cnt_' + initial_state + '_' + self.disease_name] == 0
+        susceptible = susceptible & self.host.df_population[initial_state + '_' + self.disease_name]
+        if condition is not None:
+            susceptible = susceptible & condition
+
+        count_arr = None
+
+        # in case of death
+        if target_state == 'death':
+            # there might be a probability of dying of the disease, which is taken into account now
+            if proba_death < 1.:
+                susceptible = susceptible & \
+                              (np.random.uniform(0, 1, (self.host.df_population.shape[0],)) < proba_death)
+
+            if return_transition_count:
+                count_arr = transition_conditional_count_nb_agent_per_vertex(susceptible,
+                                                                             self.host.df_population[
+                                                                                 position_attribute],
+                                                                             self.host.graph.weights.shape[0])
+
+            # killing
+            self.host.df_population = self.host.df_population[~susceptible]
+
+        # all the rest corresponds to transition between stages of the disease
+        else:
+            if return_transition_count:
+                count_arr = transition_conditional_count_nb_agent_per_vertex(susceptible,
+                                                                             self.host.df_population[
+                                                                                 position_attribute],
+                                                                             self.host.graph.weights.shape[0])
+
+            self.host.df_population[target_state + '_' + self.disease_name] = susceptible | self.host.df_population[
+                                                                                target_state + '_' + self.disease_name]
+
+            transition_falsify_when_condition(self.host.df_population[initial_state + '_' + self.disease_name],
+                                              susceptible)
+
+            prob = arr_prob_nb_timestep.astype('float64')
+            prob = prob / prob.sum()
+            arr_cnt = np.random.choice(arr_nb_timestep, susceptible.sum(), p=prob)
+
+            transition_initialize_counters_of_newly_infected(susceptible,
+                                                             self.host.df_population[
+                                                                 'cnt_' + target_state + '_' + self.disease_name],
+                                                             arr_cnt)
+        return count_arr
```

### Comparing `sampy-abm-1.0.2/src/sampy/disease/single_species/transmission.py` & `sampy_abm-1.0.3/src/sampy/disease/single_species/transmission.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-import numpy as np
-from .jit_compiled_functions import *
-from ...utils.errors_shortcut import (check_input_array,
-                                      check_col_exists_good_type)
-
-
-class TransmissionByContact:
-    def __init__(self, **kwargs):
-        pass
-
-    def _sampy_debug_contact_contagion(self, contact_rate, position_attribute='position', condition=None,
-                                       return_arr_new_infected=True):
-        if self.host.df_population.nb_rows == 0:
-            return
-
-        check_col_exists_good_type(self.host.df_population, position_attribute, 'position_attribute',
-                                   prefix_dtype='int', reject_none=True)
-        if condition is not None:
-            check_input_array(condition, 'condition', 'bool', shape=(self.host.df_population.nb_rows,))
-
-    def contact_contagion(self, contact_rate, position_attribute='position',
-                          condition=None,
-                          return_arr_new_infected=True):
-        """
-        Propagate the disease by direct contact using the following methodology. For any vertex X of the graph, we
-        count the number of contagious agents N_c, then each non immuned agent on the vertex X has a probability of
-
-                            1 - (1 - contact_rate) ** N_c
-
-        to become infected.
-
-        :param contact_rate: Float value. used to determine the probability of becoming infected
-        :param position_attribute: optional, string, default 'position'. Name of the agent attribute used as position.
-        :param condition: optional, array of bool, default None. Array of boolean such that the i-th value is
-                          True if and only if the i-th agent (i.e. the agent at the line i of df_population) can be
-                          infected and transmit disease. All the agent having their corresponding value to False are
-                          protected from infection and cannot transmit the disease.
-        :param return_arr_new_infected: optional, bool, default True
-        """
-        col_pos = self.host.df_population[position_attribute]
-        col_con = self.host.df_population['con_' + self.disease_name]
-        if condition is not None:
-            col_con = col_con & condition
-        nb_vertex = self.host.graph.connections.shape[0]
-
-        # return the array counting the number of contagious agents
-        count_con = conditional_count_return_full_array(nb_vertex, col_pos, col_con)
-
-        # make the array of newly infected individuals. Note that for the moment the computation is not optimized,
-        # and the random contamination is computed for EVERY agent, and then we exclude the not susceptible ones.
-        new_infected = np.random.uniform(0, 1, (count_con.shape[0],)) < 1 - (1 - contact_rate) ** count_con
-
-        # exclusion of the immuned and already infected agents
-        new_infected = new_infected & ~(self.host.df_population['inf_' + self.disease_name]) \
-                                    & ~(self.host.df_population['con_' + self.disease_name]) \
-                                    & ~(self.host.df_population['imm_' + self.disease_name])
-
-        if condition is not None:
-            new_infected = new_infected & condition
-
-        self.host.df_population['inf_' + self.disease_name] = self.host.df_population['inf_' + self.disease_name] | new_infected
-
-        if return_arr_new_infected:
-            return new_infected
-
-
-class TransmissionByContactWithContactTracing:
-    def __init__(self, **kwargs):
-        pass
-
-    def _sampy_debug_contact_contagion(self, contact_rate, position_attribute='position', condition=None,
-                                       return_arr_new_infected=True):
-        if self.host.df_population.nb_rows == 0:
-            return
-
-        check_col_exists_good_type(self.host.df_population, position_attribute, 'position_attribute',
-                                   prefix_dtype='int', reject_none=True)
-        if condition is not None:
-            check_input_array(condition, 'condition', 'bool', shape=(self.host.df_population.nb_rows,))
-
-    def contact_contagion(self, contact_rate, position_attribute='position', id_attribute='col_id',
-                          condition=None,
-                          return_arr_new_infected=True):
-        """
-        Propagate the disease by direct contact using the following methodology. For any vertex X of the graph, we
-        count the number of contagious agents N_c, then each non immuned agent on the cell X has a probability of
-
-                            1 - (1 - contact_rate) ** N_c
-
-        to become infected. This class will assign to each newly contaminated agent an individual who
-        contaminated it. This comes with an extra computational cost.
-
-        :param contact_rate: Float value. used to determine the probability of becoming infected
-        :param position_attribute: optional, string, default 'position'. Name of the agent attribute used as position.
-        :param id_attribute: optional, string, default 'col_id'.
-        :param condition: optional, array of bool, default None. Array of boolean such that the i-th value is
-                          True if and only if the i-th agent (i.e. the agent at the line i of df_population) can be
-                          infected. All the agent having their corresponding value to False are protected from
-                          infection.
-        :param return_arr_new_infected: optional, bool, default True
-        """
-        col_pos = self.host.df_population[position_attribute]
-        col_con = self.host.df_population['con_' + self.disease_name]
-        nb_vertex = self.host.graph.connections.shape[0]
-
-        # return the array counting the number of contagious agents
-        count_con = conditional_count_return_full_array(nb_vertex, col_pos, col_con)
-
-        # make the array of newly infected individuals. Note that for the moment the computation is not optimized,
-        # and the random contamination is computed for EVERY agent, and then we exclude the not susceptible ones.
-        new_infected = np.random.uniform(0, 1, (count_con.shape[0],)) < 1 - (1 - contact_rate) ** count_con
-
-        # exclusion of the immuned and already infected agents
-        new_infected = new_infected & ~(self.host.df_population['inf_' + self.disease_name]) \
-                                    & ~(self.host.df_population['con_' + self.disease_name]) \
-                                    & ~(self.host.df_population['imm_' + self.disease_name])
-
-        if condition is not None:
-            new_infected = new_infected & condition
-
-        self.host.df_population['inf_' + self.disease_name] = self.host.df_population['inf_' + self.disease_name] | new_infected
-
-        # here we assign to each newly infected agent a 'source of disease'
-        rand_con = np.random.uniform(0, 1, new_infected.sum())
-        col_id, col_contact = transmission_contact_contagion_contact_tracing(self.host.df_population[id_attribute],
-                                                                             col_pos,
-                                                                             col_con,
-                                                                             rand_con,
-                                                                             new_infected,
-                                                                             nb_vertex)
-
-        if return_arr_new_infected:
-            return new_infected, col_id, col_contact
-        else:
-            return col_id, col_contact
-
-    def create_csv_contact_list(self, list_arr_id, list_arr_contact, list_timestep=None):
-        list_non_zero_arr = [(len(arr.shape) > 0 and arr.shape[0] > 0) for arr in list_arr_id]
-        final_list_arr_id = [arr for i, arr in enumerate(list_arr_id) if list_non_zero_arr[i]]
-        final_list_arr_contact = [arr for i, arr in enumerate(list_arr_contact) if list_non_zero_arr[i]]
+import numpy as np
+from .jit_compiled_functions import *
+from ...utils.errors_shortcut import (check_input_array,
+                                      check_col_exists_good_type)
+
+
+class TransmissionByContact:
+    def __init__(self, **kwargs):
+        pass
+
+    def _sampy_debug_contact_contagion(self, contact_rate, position_attribute='position', condition=None,
+                                       return_arr_new_infected=True):
+        if self.host.df_population.nb_rows == 0:
+            return
+
+        check_col_exists_good_type(self.host.df_population, position_attribute, 'position_attribute',
+                                   prefix_dtype='int', reject_none=True)
+        if condition is not None:
+            check_input_array(condition, 'condition', 'bool', shape=(self.host.df_population.nb_rows,))
+
+    def contact_contagion(self, contact_rate, position_attribute='position',
+                          condition=None,
+                          return_arr_new_infected=True):
+        """
+        Propagate the disease by direct contact using the following methodology. For any vertex X of the graph, we
+        count the number of contagious agents N_c, then each non immuned agent on the vertex X has a probability of
+
+                            1 - (1 - contact_rate) ** N_c
+
+        to become infected.
+
+        :param contact_rate: Float value. used to determine the probability of becoming infected
+        :param position_attribute: optional, string, default 'position'. Name of the agent attribute used as position.
+        :param condition: optional, array of bool, default None. Array of boolean such that the i-th value is
+                          True if and only if the i-th agent (i.e. the agent at the line i of df_population) can be
+                          infected and transmit disease. All the agent having their corresponding value to False are
+                          protected from infection and cannot transmit the disease.
+        :param return_arr_new_infected: optional, bool, default True
+        """
+        col_pos = self.host.df_population[position_attribute]
+        col_con = self.host.df_population['con_' + self.disease_name]
+        if condition is not None:
+            col_con = col_con & condition
+        nb_vertex = self.host.graph.connections.shape[0]
+
+        # return the array counting the number of contagious agents
+        count_con = conditional_count_return_full_array(nb_vertex, col_pos, col_con)
+
+        # make the array of newly infected individuals. Note that for the moment the computation is not optimized,
+        # and the random contamination is computed for EVERY agent, and then we exclude the not susceptible ones.
+        new_infected = np.random.uniform(0, 1, (count_con.shape[0],)) < 1 - (1 - contact_rate) ** count_con
+
+        # exclusion of the immuned and already infected agents
+        new_infected = new_infected & ~(self.host.df_population['inf_' + self.disease_name]) \
+                                    & ~(self.host.df_population['con_' + self.disease_name]) \
+                                    & ~(self.host.df_population['imm_' + self.disease_name])
+
+        if condition is not None:
+            new_infected = new_infected & condition
+
+        self.host.df_population['inf_' + self.disease_name] = self.host.df_population['inf_' + self.disease_name] | new_infected
+
+        if return_arr_new_infected:
+            return new_infected
+
+
+class TransmissionByContactWithContactTracing:
+    def __init__(self, **kwargs):
+        pass
+
+    def _sampy_debug_contact_contagion(self, contact_rate, position_attribute='position', condition=None,
+                                       return_arr_new_infected=True):
+        if self.host.df_population.nb_rows == 0:
+            return
+
+        check_col_exists_good_type(self.host.df_population, position_attribute, 'position_attribute',
+                                   prefix_dtype='int', reject_none=True)
+        if condition is not None:
+            check_input_array(condition, 'condition', 'bool', shape=(self.host.df_population.nb_rows,))
+
+    def contact_contagion(self, contact_rate, position_attribute='position', id_attribute='col_id',
+                          condition=None,
+                          return_arr_new_infected=True):
+        """
+        Propagate the disease by direct contact using the following methodology. For any vertex X of the graph, we
+        count the number of contagious agents N_c, then each non immuned agent on the cell X has a probability of
+
+                            1 - (1 - contact_rate) ** N_c
+
+        to become infected. This class will assign to each newly contaminated agent an individual who
+        contaminated it. This comes with an extra computational cost.
+
+        :param contact_rate: Float value. used to determine the probability of becoming infected
+        :param position_attribute: optional, string, default 'position'. Name of the agent attribute used as position.
+        :param id_attribute: optional, string, default 'col_id'.
+        :param condition: optional, array of bool, default None. Array of boolean such that the i-th value is
+                          True if and only if the i-th agent (i.e. the agent at the line i of df_population) can be
+                          infected. All the agent having their corresponding value to False are protected from
+                          infection.
+        :param return_arr_new_infected: optional, bool, default True
+        """
+        col_pos = self.host.df_population[position_attribute]
+        col_con = self.host.df_population['con_' + self.disease_name]
+        nb_vertex = self.host.graph.connections.shape[0]
+
+        # return the array counting the number of contagious agents
+        count_con = conditional_count_return_full_array(nb_vertex, col_pos, col_con)
+
+        # make the array of newly infected individuals. Note that for the moment the computation is not optimized,
+        # and the random contamination is computed for EVERY agent, and then we exclude the not susceptible ones.
+        new_infected = np.random.uniform(0, 1, (count_con.shape[0],)) < 1 - (1 - contact_rate) ** count_con
+
+        # exclusion of the immuned and already infected agents
+        new_infected = new_infected & ~(self.host.df_population['inf_' + self.disease_name]) \
+                                    & ~(self.host.df_population['con_' + self.disease_name]) \
+                                    & ~(self.host.df_population['imm_' + self.disease_name])
+
+        if condition is not None:
+            new_infected = new_infected & condition
+
+        self.host.df_population['inf_' + self.disease_name] = self.host.df_population['inf_' + self.disease_name] | new_infected
+
+        # here we assign to each newly infected agent a 'source of disease'
+        rand_con = np.random.uniform(0, 1, new_infected.sum())
+        col_id, col_contact = transmission_contact_contagion_contact_tracing(self.host.df_population[id_attribute],
+                                                                             col_pos,
+                                                                             col_con,
+                                                                             rand_con,
+                                                                             new_infected,
+                                                                             nb_vertex)
+
+        if return_arr_new_infected:
+            return new_infected, col_id, col_contact
+        else:
+            return col_id, col_contact
+
+    def create_csv_contact_list(self, list_arr_id, list_arr_contact, list_timestep=None):
+        list_non_zero_arr = [(len(arr.shape) > 0 and arr.shape[0] > 0) for arr in list_arr_id]
+        final_list_arr_id = [arr for i, arr in enumerate(list_arr_id) if list_non_zero_arr[i]]
+        final_list_arr_contact = [arr for i, arr in enumerate(list_arr_contact) if list_non_zero_arr[i]]
```

### Comparing `sampy-abm-1.0.2/src/sampy/disease/two_species/base.py` & `sampy_abm-1.0.3/src/sampy/disease/two_species/base.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-import numpy as np
-from .jit_compiled_functions import base_contaminate_vertices
-
-
-class BaseTwoSpeciesDisease:
-    """Base class for two species disease. This building block expects the following kwargs:
-
-    :param disease_name: mandatory kwargs. String.
-    :param host1: mandatory kwargs. Population object of the first host.
-    :param host2: mandatory kwargs. Population object of the second host.
-    """
-    def __init__(self, disease_name='', host1=None, host2=None, **kwargs):
-        # check values have been given
-        if not host1:
-            raise ValueError('No first host given for the disease. Use Kwarg host1.')
-        if not host2:
-            raise ValueError('No second host given for the disease. Use Kwarg host2.')
-        if not disease_name:
-            raise ValueError('No name given to the disease. Use Kwarg disease_name.')
-
-        self.host1 = host1
-        self.host2 = host2
-
-        self.disease_name = disease_name
-
-        self.host1.df_population['inf_' + disease_name] = False
-        self.host1.df_population['con_' + disease_name] = False
-        self.host1.df_population['imm_' + disease_name] = False
-
-        if hasattr(host1, 'dict_default_val'):
-            self.host1.dict_default_val['inf_' + disease_name] = False
-            self.host1.dict_default_val['con_' + disease_name] = False
-            self.host1.dict_default_val['imm_' + disease_name] = False
-
-        self.host2.df_population['inf_' + disease_name] = False
-        self.host2.df_population['con_' + disease_name] = False
-        self.host2.df_population['imm_' + disease_name] = False
-
-        if hasattr(host2, 'dict_default_val'):
-            self.host2.dict_default_val['inf_' + disease_name] = False
-            self.host2.dict_default_val['con_' + disease_name] = False
-            self.host2.dict_default_val['imm_' + disease_name] = False
-
-        if not hasattr(self, 'set_disease_status'):
-            self.set_disease_status = {'inf', 'con', 'imm'}
-        else:
-            self.set_disease_status.update(['inf', 'con', 'imm'])
-
-        self.on_ticker = []
-
-    def tick(self):
-        """
-        execute in order all the methods whose name are in the list 'on_ticker'. Those methods should not accept
-        any arguments.
-        """
-        for method in self.on_ticker:
-            getattr(self, method)()
-
-    def contaminate_vertices(self, host, list_vertices, level, return_arr_newly_contaminated=True,
-                             condition=None, position_attribute='position'):
-        """
-        Contaminate the vertices given in the list 'list_vertices' with the disease. Each agent on the vertex have a
-        probability of 'level' to be contaminated.
-
-        :param host: string, either 'host1' or 'host2'. If host1 should be targeted, put 'host1', If host2 should be
-                     targeted, put 'host2'. Any other input will lead to an error.
-        :param list_vertices: list of vertices ID to be contaminated.
-        :param level: float, probability for agent on the vertices to be contaminated.
-        :param return_arr_newly_contaminated: optional, boolean, default True. If True, the method returns an array
-                                              telling which agents were contaminated.
-        :param condition: optional, array of bool, default None. If not None, say which agents are susceptible to be
-                          contaminated.
-        :param position_attribute: optional, string, default 'position'. Agent attribute to be used to define
-                                   their position.
-        :return: if return_arr_newly_contaminated is set to True, returns a 1D array of bool. Otherwise, returns
-                 None.
-        """
-        # here we check that the given object seems to be the one provided during construction.
-        if host == 'host1':
-            host = self.host1
-        elif host == 'host2':
-            host = self.host2
-        else:
-            raise ValueError('The "host" argument is not recognized. It should be either "host1" or "host2".')
-
-
-        # this is quite inefficient, but this function is not assumed to be called often.
-        for i, vertex_id in enumerate(list_vertices):
-            if i == 0:
-                arr_new_infected = (host.df_population[position_attribute] ==
-                                    host.graph.dict_cell_id_to_ind[vertex_id])
-                continue
-            arr_new_infected = arr_new_infected | (host.df_population[position_attribute] ==
-                                                   host.graph.dict_cell_id_to_ind[vertex_id])
-        arr_new_infected = arr_new_infected & ~(host.df_population['inf_' + self.disease_name] |
-                                                host.df_population['con_' + self.disease_name] |
-                                                host.df_population['imm_' + self.disease_name])
-        if condition is not None:
-            arr_new_infected = arr_new_infected & condition
-        rand = np.random.uniform(0, 1, (arr_new_infected.sum(),))
-        base_contaminate_vertices(arr_new_infected, rand, level)
-        host.df_population['inf_' + self.disease_name] = host.df_population['inf_' + self.disease_name] | \
-                                                         arr_new_infected
-        if return_arr_newly_contaminated:
-            return arr_new_infected
+import numpy as np
+from .jit_compiled_functions import base_contaminate_vertices
+
+
+class BaseTwoSpeciesDisease:
+    """Base class for two species disease. This building block expects the following kwargs:
+
+    :param disease_name: mandatory kwargs. String.
+    :param host1: mandatory kwargs. Population object of the first host.
+    :param host2: mandatory kwargs. Population object of the second host.
+    """
+    def __init__(self, disease_name='', host1=None, host2=None, **kwargs):
+        # check values have been given
+        if not host1:
+            raise ValueError('No first host given for the disease. Use Kwarg host1.')
+        if not host2:
+            raise ValueError('No second host given for the disease. Use Kwarg host2.')
+        if not disease_name:
+            raise ValueError('No name given to the disease. Use Kwarg disease_name.')
+
+        self.host1 = host1
+        self.host2 = host2
+
+        self.disease_name = disease_name
+
+        self.host1.df_population['inf_' + disease_name] = False
+        self.host1.df_population['con_' + disease_name] = False
+        self.host1.df_population['imm_' + disease_name] = False
+
+        if hasattr(host1, 'dict_default_val'):
+            self.host1.dict_default_val['inf_' + disease_name] = False
+            self.host1.dict_default_val['con_' + disease_name] = False
+            self.host1.dict_default_val['imm_' + disease_name] = False
+
+        self.host2.df_population['inf_' + disease_name] = False
+        self.host2.df_population['con_' + disease_name] = False
+        self.host2.df_population['imm_' + disease_name] = False
+
+        if hasattr(host2, 'dict_default_val'):
+            self.host2.dict_default_val['inf_' + disease_name] = False
+            self.host2.dict_default_val['con_' + disease_name] = False
+            self.host2.dict_default_val['imm_' + disease_name] = False
+
+        if not hasattr(self, 'set_disease_status'):
+            self.set_disease_status = {'inf', 'con', 'imm'}
+        else:
+            self.set_disease_status.update(['inf', 'con', 'imm'])
+
+        self.on_ticker = []
+
+    def tick(self):
+        """
+        execute in order all the methods whose name are in the list 'on_ticker'. Those methods should not accept
+        any arguments.
+        """
+        for method in self.on_ticker:
+            getattr(self, method)()
+
+    def contaminate_vertices(self, host, list_vertices, level, return_arr_newly_contaminated=True,
+                             condition=None, position_attribute='position'):
+        """
+        Contaminate the vertices given in the list 'list_vertices' with the disease. Each agent on the vertex have a
+        probability of 'level' to be contaminated.
+
+        :param host: string, either 'host1' or 'host2'. If host1 should be targeted, put 'host1', If host2 should be
+                     targeted, put 'host2'. Any other input will lead to an error.
+        :param list_vertices: list of vertices ID to be contaminated.
+        :param level: float, probability for agent on the vertices to be contaminated.
+        :param return_arr_newly_contaminated: optional, boolean, default True. If True, the method returns an array
+                                              telling which agents were contaminated.
+        :param condition: optional, array of bool, default None. If not None, say which agents are susceptible to be
+                          contaminated.
+        :param position_attribute: optional, string, default 'position'. Agent attribute to be used to define
+                                   their position.
+        :return: if return_arr_newly_contaminated is set to True, returns a 1D array of bool. Otherwise, returns
+                 None.
+        """
+        # here we check that the given object seems to be the one provided during construction.
+        if host == 'host1':
+            host = self.host1
+        elif host == 'host2':
+            host = self.host2
+        else:
+            raise ValueError('The "host" argument is not recognized. It should be either "host1" or "host2".')
+
+
+        # this is quite inefficient, but this function is not assumed to be called often.
+        for i, vertex_id in enumerate(list_vertices):
+            if i == 0:
+                arr_new_infected = (host.df_population[position_attribute] ==
+                                    host.graph.dict_cell_id_to_ind[vertex_id])
+                continue
+            arr_new_infected = arr_new_infected | (host.df_population[position_attribute] ==
+                                                   host.graph.dict_cell_id_to_ind[vertex_id])
+        arr_new_infected = arr_new_infected & ~(host.df_population['inf_' + self.disease_name] |
+                                                host.df_population['con_' + self.disease_name] |
+                                                host.df_population['imm_' + self.disease_name])
+        if condition is not None:
+            arr_new_infected = arr_new_infected & condition
+        rand = np.random.uniform(0, 1, (arr_new_infected.sum(),))
+        base_contaminate_vertices(arr_new_infected, rand, level)
+        host.df_population['inf_' + self.disease_name] = host.df_population['inf_' + self.disease_name] | \
+                                                         arr_new_infected
+        if return_arr_newly_contaminated:
+            return arr_new_infected
```

### Comparing `sampy-abm-1.0.2/src/sampy/disease/two_species/builtin_disease.py` & `sampy_abm-1.0.3/src/sampy/disease/two_species/builtin_disease.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,168 +1,190 @@
-from .base import BaseTwoSpeciesDisease
-from .transition import TransitionCustomProbPermanentImmunity
-from .transmission import ContactTransmissionSameGraph
-from ...utils.decorators import sampy_class
-
-
-@sampy_class
-class TwoSpeciesContactCustomProbTransitionPermanentImmunity(BaseTwoSpeciesDisease,
-                                                             TransitionCustomProbPermanentImmunity,
-                                                             ContactTransmissionSameGraph):
-    """
-    Basic disease, transmission by direct contact (contagion only between agents on the same vertex), transition between
-    disease states encoded by user given arrays of probabilities, and permanent immunity.
-
-    IMPORTANT: We strongly recommend the user to use the "simplified" methods defined here instead of the usual
-               'contaminate_vertices', 'contact_contagion' and 'transition_between_states'. Indeed, the combination of
-               building blocks involved in this disease requires many actions to be performed in a precise order,
-               otherwise the model's behaviour cannot be guaranteed. See each simplified method description to learn
-               about each respective ordering.
-
-    :param disease_name: mandatory kwargs. String.
-    :param host1: mandatory kwargs. Population object of the first host.
-    :param host2: mandatory kwargs. Population object of the second host.
-    """
-    def __init__(self, **kwargs):
-        pass
-
-    def simplified_contact_contagion(self, contact_rate_matrix, arr_timesteps_host1, arr_prob_timesteps_host1,
-                                     arr_timesteps_host2, arr_prob_timesteps_host2,
-                                     position_attribute_host1='position', position_attribute_host2='position',
-                                     condition_host1=None, condition_host2=None,
-                                     return_arr_new_infected=False, return_type_transmission=False):
-        """
-        Propagate the disease by direct contact using the following methodology. For any vertex X of the graph, we
-        count the number of contagious agents N_c_host_j, then each non immuned agent of host_k on the vertex X has a
-        probability of
-
-                            1 - (1 - contact_rate_matrix[j,k]) ** N_c_host_j
-
-        to become infected by a contact with an agent of host_j.
-
-        Detailed Explanation: each agent has a series of counter attached, telling how much time-steps they will spend
-                              in each disease status. Those counters have to be initialized when an individual is newly
-                              infected, and that's what this method does to the newly infected individuals.
-
-        :param contact_rate_matrix: 2D array of floats of shape (2, 2). Here, contact_rate_matrix[0][0] is the
-                                    probability of contact contagion from host1 to host1, contact_rate_matrix[0][1] is
-                                    the probability of contact contagion from host1 to host2, etc...
-        :param arr_timesteps_host1: 1d array of int. work in tandem with arr_prob_timesteps_host1, see below.
-        :param arr_prob_timesteps_host1: 1D array of float. arr_prob[i] is the probability for an agent to stay infected
-                                         but not contagious for arr_nb_timestep[i] time-steps.
-        :param arr_timesteps_host2: same but for host2.
-        :param arr_prob_timesteps_host2: same but for host2.
-        :param position_attribute_host1: optional, string, default 'position'. Name of the agent attribute used as
-                                         position for host1.
-        :param position_attribute_host2: optional, string, default 'position'. Name of the agent attribute used as
-                                         position for host2.
-        :param condition_host1: optional, array of bool, default None. Array of boolean such that the i-th value is
-                          True if and only if the i-th agent of host1 (i.e. the agent at the line i of df_population)
-                          can be infected and transmit disease. All the agent having their corresponding value to False
-                          are protected from infection and cannot transmit the disease.
-        :param condition_host2: optional, array of bool, default None. Array of boolean such that the i-th value is
-                          True if and only if the i-th agent of host2 (i.e. the agent at the line i of df_population)
-                          can be infected and transmit disease. All the agent having their corresponding value to False
-                          are protected from infection and cannot transmit the disease.
-        :param return_arr_new_infected: optional, boolean, default False. If True, the method returns two arrays telling
-                                        which agent got contaminated in each host species.
-        :param return_type_transmission: optional, boolean, default False.
-
-        :return: Depending on the values of the parameters 'return_arr_new_infected' and 'return_type_transmission',
-                 the return value will either be None (both are False) or a dictionnary whose key-values are:
-                    - 'arr_new_infected_host1', 'arr_new_infected_host2' if return_arr_new_infected is True, and the
-                      values are 1D arrays of bool telling which agents got infected for each host;
-                    - 'arr_type_transmission_host1', 'arr_type_transmission_host2' if return_type_transmission is True,
-                      and the values are 1D arrays of non-negative integers such that the integer at line i is 0 if the
-                      i-th agent has not been contaminated, 1 if it has been contaminated by a member of its own species
-                      2 if it has been contaminated by a member of the other species, 3 if it has been contaminated by
-                      agents from both its species and the other.
-        """
-        dict_contagion = self.contact_contagion(contact_rate_matrix, return_arr_new_infected=True,
-                                                return_type_transmission=return_type_transmission,
-                                                position_attribute_host1=position_attribute_host1,
-                                                position_attribute_host2=position_attribute_host2,
-                                                condition_host1=condition_host1, condition_host2=condition_host2)
-        self.initialize_counters_of_newly_infected('host1', dict_contagion['arr_new_infected_host1'],
-                                                   arr_timesteps_host1, arr_prob_timesteps_host1)
-        self.initialize_counters_of_newly_infected('host2', dict_contagion['arr_new_infected_host2'],
-                                                   arr_timesteps_host2, arr_prob_timesteps_host2)
-        if not return_type_transmission and not return_arr_new_infected:
-            return
-        if return_arr_new_infected:
-            return dict_contagion
-        else:  # no other case needed
-            del dict_contagion['arr_new_infected_host1']
-            del dict_contagion['arr_new_infected_host2']
-            return dict_contagion
-
-    def simplified_transition_between_states(self, prob_death_host1, prob_death_host2,
-                                             arr_infectious_period_host1, arr_prob_infectious_period_host1,
-                                             arr_infectious_period_host2, arr_prob_infectious_period_host2):
-        """
-        Takes care of the transition between all the disease states. That is, agents that are at the end of their
-        infected period become contagious and agents at the end of their contagious period either die (with a
-        probability of 'prob_death') or become immuned.
-
-        Detailed Explanation: the method transition_between_states is coded in such a way that when using it for
-                              transitionning from con to imm, all the agents at the end of their contagious period at
-                              the time the method is called transition. Therefore, we have to make the transition
-                              'con' to 'death' first.
-
-        :param prob_death_host1: float between 0 and 1, probability for an agent of host1 to die at the end of the
-                                 contagious period
-        :param prob_death_host2: float between 0 and 1, probability for an agent of host2 to die at the end of the
-                                 contagious period
-        :param arr_infectious_period_host1: 1d array of int, works in tandem with arr_prob_infectious_period_host1.
-                                            See Below.
-        :param arr_prob_infectious_period_host1: 1d array of floats, sums to 1. Same shape as
-                    arr_infectious_period_host1. When an agent transition from infected to contagious, then
-                    arr_prob_infectious_period_host1[i] is the probability for this agent to stay
-                    arr_infectious_period_host1[i] timesteps contagious.
-        :param arr_infectious_period_host2: same as host1
-        :param arr_prob_infectious_period_host2: same as host1
-        """
-        self.transition_between_states('host1', 'con', 'death', proba_death=prob_death_host1)
-        self.transition_between_states('host2', 'con', 'death', proba_death=prob_death_host2)
-
-        if self.host1.df_population.nb_rows != 0:
-            self.transition_between_states('host1', 'con', 'imm')
-            self.transition_between_states('host1', 'inf', 'con', arr_nb_timestep=arr_infectious_period_host1,
-                                           arr_prob_nb_timestep=arr_prob_infectious_period_host1)
-
-        if self.host2.df_population.nb_rows != 0:
-            self.transition_between_states('host2', 'con', 'imm')
-            self.transition_between_states('host2', 'inf', 'con', arr_nb_timestep=arr_infectious_period_host2,
-                                           arr_prob_nb_timestep=arr_prob_infectious_period_host2)
-
-    def simplified_contaminate_vertices(self, host, list_vertices, level, arr_timesteps, arr_prob_timesteps,
-                                        condition=None, position_attribute='position',
-                                        return_arr_newly_contaminated=True):
-        """
-        Contaminate a list of vertices.
-
-        Detailed explanation: each agent has a series of counter attached, telling how much time-steps they will spend
-                              in each disease status. Those counters have to be initialized when an individual is newly
-                              infected, and that's what this method does to the newly infected individuals.
-
-        :param host: string, either 'host1' or 'host2', tells which host to infect.
-        :param list_vertices: list of vertices ID to be contaminated.
-        :param level: float, probability for agent on the vertices to be contaminated.
-        :param arr_timesteps: 1D array of integer. Works in tandem with 'arr_prob_timesteps'. See below.
-        :param arr_prob_timesteps: 1D array of float. arr_prob_timesteps[i] is the probability for an agent to stay
-                                   infected but not contagious for arr_timesteps[i] timesteps.
-        :param condition: optional, array of bool, default None. If not None, say which agents are susceptible to be
-                          contaminated.
-        :param position_attribute: optional, string, default 'position'. Agent attribute to be used to define
-                                   their position.
-        :param return_arr_newly_contaminated: optional, boolean, default True. If True, the method returns an array
-                                              telling which agents were contaminated.
-
-        :return: if return_arr_newly_contaminated is set to True, returns a 1D array of bool telling which agents where
-                 contaminated. Returns None otherwise.
-        """
-        arr_new_contaminated = self.contaminate_vertices(host, list_vertices, level,
-                                                         condition=condition, position_attribute=position_attribute,
-                                                         return_arr_newly_contaminated=True)
-        self.initialize_counters_of_newly_infected(host, arr_new_contaminated, arr_timesteps, arr_prob_timesteps)
-        if return_arr_newly_contaminated:
-            return arr_new_contaminated
+from .base import BaseTwoSpeciesDisease
+from .transition import TransitionCustomProbPermanentImmunity
+from .transmission import ContactTransmissionSameGraph
+from ...utils.decorators import sampy_class
+
+
+@sampy_class
+class TwoSpeciesContactCustomProbTransitionPermanentImmunity(BaseTwoSpeciesDisease,
+                                                             TransitionCustomProbPermanentImmunity,
+                                                             ContactTransmissionSameGraph):
+    """
+    Basic disease, transmission by direct contact (contagion only between agents on the same vertex), transition between
+    disease states encoded by user given arrays of probabilities, and permanent immunity.
+
+    IMPORTANT: We strongly recommend the user to use the "simplified" methods defined here instead of the usual
+               'contaminate_vertices', 'contact_contagion' and 'transition_between_states'. Indeed, the combination of
+               building blocks involved in this disease requires many actions to be performed in a precise order,
+               otherwise the model's behaviour cannot be guaranteed. See each simplified method description to learn
+               about each respective ordering.
+
+    :param disease_name: mandatory kwargs. String.
+    :param host1: mandatory kwargs. Population object of the first host.
+    :param host2: mandatory kwargs. Population object of the second host.
+    """
+    def __init__(self, **kwargs):
+        pass
+
+    def simplified_contact_contagion(self, contact_rate_matrix, arr_timesteps_host1, arr_prob_timesteps_host1,
+                                     arr_timesteps_host2, arr_prob_timesteps_host2,
+                                     position_attribute_host1='position', position_attribute_host2='position',
+                                     condition_host1=None, condition_host2=None,
+                                     return_arr_new_infected=False, return_type_transmission=False):
+        """
+        Propagate the disease by direct contact using the following methodology. For any vertex X of the graph, we
+        count the number of contagious agents N_c_host_j, then each non immuned agent of host_k on the vertex X has a
+        probability of
+
+                            1 - (1 - contact_rate_matrix[j,k]) ** N_c_host_j
+
+        to become infected by a contact with an agent of host_j.
+
+        Detailed Explanation: each agent has a series of counter attached, telling how much time-steps they will spend
+                              in each disease status. Those counters have to be initialized when an individual is newly
+                              infected, and that's what this method does to the newly infected individuals.
+
+        :param contact_rate_matrix: 2D array of floats of shape (2, 2). Here, contact_rate_matrix[0][0] is the
+                                    probability of contact contagion from host1 to host1, contact_rate_matrix[0][1] is
+                                    the probability of contact contagion from host1 to host2, etc...
+        :param arr_timesteps_host1: 1d array of int. work in tandem with arr_prob_timesteps_host1, see below.
+        :param arr_prob_timesteps_host1: 1D array of float. arr_prob[i] is the probability for an agent to stay infected
+                                         but not contagious for arr_nb_timestep[i] time-steps.
+        :param arr_timesteps_host2: same but for host2.
+        :param arr_prob_timesteps_host2: same but for host2.
+        :param position_attribute_host1: optional, string, default 'position'. Name of the agent attribute used as
+                                         position for host1.
+        :param position_attribute_host2: optional, string, default 'position'. Name of the agent attribute used as
+                                         position for host2.
+        :param condition_host1: optional, array of bool, default None. Array of boolean such that the i-th value is
+                          True if and only if the i-th agent of host1 (i.e. the agent at the line i of df_population)
+                          can be infected and transmit disease. All the agent having their corresponding value to False
+                          are protected from infection and cannot transmit the disease.
+        :param condition_host2: optional, array of bool, default None. Array of boolean such that the i-th value is
+                          True if and only if the i-th agent of host2 (i.e. the agent at the line i of df_population)
+                          can be infected and transmit disease. All the agent having their corresponding value to False
+                          are protected from infection and cannot transmit the disease.
+        :param return_arr_new_infected: optional, boolean, default False. If True, the method returns two arrays telling
+                                        which agent got contaminated in each host species.
+        :param return_type_transmission: optional, boolean, default False.
+
+        :return: Depending on the values of the parameters 'return_arr_new_infected' and 'return_type_transmission',
+                 the return value will either be None (both are False) or a dictionnary whose key-values are:
+                    - 'arr_new_infected_host1', 'arr_new_infected_host2' if return_arr_new_infected is True, and the
+                      values are 1D arrays of bool telling which agents got infected for each host;
+                    - 'arr_type_transmission_host1', 'arr_type_transmission_host2' if return_type_transmission is True,
+                      and the values are 1D arrays of non-negative integers such that the integer at line i is 0 if the
+                      i-th agent has not been contaminated, 1 if it has been contaminated by a member of its own species
+                      2 if it has been contaminated by a member of the other species, 3 if it has been contaminated by
+                      agents from both its species and the other.
+        """
+        dict_contagion = self.contact_contagion(contact_rate_matrix, return_arr_new_infected=True,
+                                                return_type_transmission=return_type_transmission,
+                                                position_attribute_host1=position_attribute_host1,
+                                                position_attribute_host2=position_attribute_host2,
+                                                condition_host1=condition_host1, condition_host2=condition_host2)
+        self.initialize_counters_of_newly_infected('host1', dict_contagion['arr_new_infected_host1'],
+                                                   arr_timesteps_host1, arr_prob_timesteps_host1)
+        self.initialize_counters_of_newly_infected('host2', dict_contagion['arr_new_infected_host2'],
+                                                   arr_timesteps_host2, arr_prob_timesteps_host2)
+        if not return_type_transmission and not return_arr_new_infected:
+            return
+        if return_arr_new_infected:
+            return dict_contagion
+        else:  # no other case needed
+            del dict_contagion['arr_new_infected_host1']
+            del dict_contagion['arr_new_infected_host2']
+            return dict_contagion
+
+    def simplified_transition_between_states(self, prob_death_host1, prob_death_host2,
+                                             arr_infectious_period_host1, arr_prob_infectious_period_host1,
+                                             arr_infectious_period_host2, arr_prob_infectious_period_host2,
+                                             return_arr_death=False):
+        """
+        Takes care of the transition between all the disease states. That is, agents that are at the end of their
+        infected period become contagious and agents at the end of their contagious period either die (with a
+        probability of 'prob_death') or become immuned.
+
+        Detailed Explanation: the method transition_between_states is coded in such a way that when using it for
+                              transitionning from con to imm, all the agents at the end of their contagious period at
+                              the time the method is called transition. Therefore, we have to make the transition
+                              'con' to 'death' first.
+
+        :param prob_death_host1: float between 0 and 1, probability for an agent of host1 to die at the end of the
+                                 contagious period
+        :param prob_death_host2: float between 0 and 1, probability for an agent of host2 to die at the end of the
+                                 contagious period
+        :param arr_infectious_period_host1: 1d array of int, works in tandem with arr_prob_infectious_period_host1.
+                                            See Below.
+        :param arr_prob_infectious_period_host1: 1d array of floats, sums to 1. Same shape as
+                    arr_infectious_period_host1. When an agent transition from infected to contagious, then
+                    arr_prob_infectious_period_host1[i] is the probability for this agent to stay
+                    arr_infectious_period_host1[i] timesteps contagious.
+        :param arr_infectious_period_host2: same as host1
+        :param arr_prob_infectious_period_host2: same as host1
+        :param return_arr_death: optional, boolean, default False. If True, the method returns two 1D arrays of
+                                 integers giving the number of death per vertex.
+        
+        :return: Depending on the values of the parameter 'return_arr_death' the returned value will either be 
+                 None (both are False) or a dictionnary whose key-values are:
+                    - 'arr_death_disease_host1', 'arr_death_disease_host2' if return_arr_death is True, and the
+                      values are 1D arrays of integers telling how much agents died per vertex.
+        """
+        dict_transition = dict()
+
+        if return_arr_death:
+            dict_transition['arr_death_disease_host1'] = self.transition_between_states('host1', 'con', 'death', 
+                                                                                        proba_death=prob_death_host1,
+                                                                                        return_transition_count=True)
+            dict_transition['arr_death_disease_host2'] = self.transition_between_states('host2', 'con', 'death', 
+                                                                                        proba_death=prob_death_host2,
+                                                                                        return_transition_count=True)
+            
+        else:
+            self.transition_between_states('host1', 'con', 'death', proba_death=prob_death_host1)
+            self.transition_between_states('host2', 'con', 'death', proba_death=prob_death_host2)
+
+        if self.host1.df_population.nb_rows != 0:
+            self.transition_between_states('host1', 'con', 'imm')
+            self.transition_between_states('host1', 'inf', 'con', arr_nb_timestep=arr_infectious_period_host1,
+                                           arr_prob_nb_timestep=arr_prob_infectious_period_host1)
+
+        if self.host2.df_population.nb_rows != 0:
+            self.transition_between_states('host2', 'con', 'imm')
+            self.transition_between_states('host2', 'inf', 'con', arr_nb_timestep=arr_infectious_period_host2,
+                                           arr_prob_nb_timestep=arr_prob_infectious_period_host2)
+            
+        if return_arr_death:
+            return dict_transition
+
+    def simplified_contaminate_vertices(self, host, list_vertices, level, arr_timesteps, arr_prob_timesteps,
+                                        condition=None, position_attribute='position',
+                                        return_arr_newly_contaminated=True):
+        """
+        Contaminate a list of vertices.
+
+        Detailed explanation: each agent has a series of counter attached, telling how much time-steps they will spend
+                              in each disease status. Those counters have to be initialized when an individual is newly
+                              infected, and that's what this method does to the newly infected individuals.
+
+        :param host: string, either 'host1' or 'host2', tells which host to infect.
+        :param list_vertices: list of vertices ID to be contaminated.
+        :param level: float, probability for agent on the vertices to be contaminated.
+        :param arr_timesteps: 1D array of integer. Works in tandem with 'arr_prob_timesteps'. See below.
+        :param arr_prob_timesteps: 1D array of float. arr_prob_timesteps[i] is the probability for an agent to stay
+                                   infected but not contagious for arr_timesteps[i] timesteps.
+        :param condition: optional, array of bool, default None. If not None, say which agents are susceptible to be
+                          contaminated.
+        :param position_attribute: optional, string, default 'position'. Agent attribute to be used to define
+                                   their position.
+        :param return_arr_newly_contaminated: optional, boolean, default True. If True, the method returns an array
+                                              telling which agents were contaminated.
+
+        :return: if return_arr_newly_contaminated is set to True, returns a 1D array of bool telling which agents where
+                 contaminated. Returns None otherwise.
+        """
+        arr_new_contaminated = self.contaminate_vertices(host, list_vertices, level,
+                                                         condition=condition, position_attribute=position_attribute,
+                                                         return_arr_newly_contaminated=True)
+        self.initialize_counters_of_newly_infected(host, arr_new_contaminated, arr_timesteps, arr_prob_timesteps)
+        if return_arr_newly_contaminated:
+            return arr_new_contaminated
```

### Comparing `sampy-abm-1.0.2/src/sampy/disease/two_species/jit_compiled_functions.py` & `sampy_abm-1.0.3/src/sampy/disease/two_species/jit_compiled_functions.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-import numpy as np
-import numba as nb
-
-
-@nb.njit
-def base_contaminate_vertices(arr_new_infected, rand, level):
-    counter = 0
-    for i in range(arr_new_infected.shape[0]):
-        if arr_new_infected[i]:
-            if rand[counter] >= level:
-                arr_new_infected[i] = False
-            counter += 1
-
-
-@nb.njit
-def transition_initialize_counters_of_newly_infected(arr_new_infected, arr_cnt, arr_new_cnt):
-    counter = 0
-    for i in range(arr_new_infected.shape[0]):
-        if arr_new_infected[i]:
-            arr_cnt[i] = arr_new_cnt[counter]
-            counter += 1
-
-
-@nb.njit
-def transition_conditional_count_nb_agent_per_vertex(arr_condition, arr_pos, nb_vertex):
-    rv = np.zeros((nb_vertex,), dtype=np.int32)
-    for i in range(arr_pos.shape[0]):
-        if arr_condition[i]:
-            rv[arr_pos[i]] += 1
-    return rv
-
-
-@nb.njit
-def transition_falsify_when_condition(arr_bool, condition):
-    for i in range(arr_bool.shape[0]):
-        if condition[i]:
-            arr_bool[i] = False
-
-
-@nb.njit
-def transmission_conditional_count(nb_vertex, arr_pos, arr_cond):
-    pos_count = np.zeros((nb_vertex,), dtype=np.int32)
-    for i in range(arr_pos.shape[0]):
-        if arr_cond[i]:
-            pos_count[arr_pos[i]] += 1
-    return pos_count
-
-
-@nb.njit
-def transmission_count_needed_samples(susceptible, pos_susceptible, arr_count_con_host1, arr_count_con_host2):
-    needed_samples = 0
-    for i in range(susceptible.shape[0]):
-        if susceptible[i]:
-            needed_samples += (int(arr_count_con_host1[pos_susceptible[i]] > 0) +
-                               int(arr_count_con_host2[pos_susceptible[i]] > 0))
-    return needed_samples
-
-
-@nb.njit
-def transmission_disease_propagation(susceptible_host1, susceptible_host2, pos_host1, pos_host2, inf_status_host1,
-                                     inf_status_host2, count_con_host1, count_con_host2, random_numbers,
-                                     contact_rate_matrix):
-    counter = 0
-    for i in range(susceptible_host1.shape[0]):
-        if susceptible_host1[i]:
-            # host1 to host 1
-            if count_con_host1[pos_host1[i]] > 0:
-                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[0][0]) ** count_con_host1[pos_host1[i]]:
-                    inf_status_host1[i] = True
-                counter += 1
-
-            # host2 to host1
-            if count_con_host2[pos_host1[i]] > 0:
-                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[1][0]) ** count_con_host2[pos_host1[i]]:
-                    inf_status_host1[i] = True
-                counter += 1
-
-    for i in range(susceptible_host2.shape[0]):
-        if susceptible_host2[i]:
-            # host1 to host2
-            if count_con_host1[pos_host2[i]] > 0:
-                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[0][1]) ** count_con_host1[pos_host2[i]]:
-                    inf_status_host2[i] = True
-                counter += 1
-
-            # host2 to host2
-            if count_con_host2[pos_host2[i]] > 0:
-                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[1][1]) ** count_con_host2[pos_host2[i]]:
-                    inf_status_host2[i] = True
-                counter += 1
-
-
-@nb.njit
-def transmission_disease_propagation_return_new_inf(susceptible_host1, susceptible_host2, pos_host1, pos_host2,
-                                                    inf_status_host1, inf_status_host2, count_con_host1,
-                                                    count_con_host2, random_numbers, contact_rate_matrix):
-    counter = 0
-    new_infected_host1 = np.full(susceptible_host1.shape, False)
-    new_infected_host2 = np.full(susceptible_host2.shape, False)
-    for i in range(susceptible_host1.shape[0]):
-        if susceptible_host1[i]:
-            # host1 to host 1
-            if count_con_host1[pos_host1[i]] > 0:
-                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[0][0]) ** count_con_host1[pos_host1[i]]:
-                    inf_status_host1[i] = True
-                    new_infected_host1[i] = True
-                counter += 1
-
-            # host2 to host1
-            if count_con_host2[pos_host1[i]] > 0:
-                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[1][0]) ** count_con_host2[pos_host1[i]]:
-                    inf_status_host1[i] = True
-                    new_infected_host1[i] = True
-                counter += 1
-
-    for i in range(susceptible_host2.shape[0]):
-        if susceptible_host2[i]:
-            # host1 to host2
-            if count_con_host1[pos_host2[i]] > 0:
-                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[0][1]) ** count_con_host1[pos_host2[i]]:
-                    inf_status_host2[i] = True
-                    new_infected_host2[i] = True
-                counter += 1
-
-            # host2 to host2
-            if count_con_host2[pos_host2[i]] > 0:
-                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[1][1]) ** count_con_host2[pos_host2[i]]:
-                    inf_status_host2[i] = True
-                    new_infected_host2[i] = True
-                counter += 1
-
-    return new_infected_host1, new_infected_host2
-
-
-@nb.njit
-def transmission_disease_propagation_return_type_inf(susceptible_host1, susceptible_host2, pos_host1, pos_host2,
-                                                     inf_status_host1, inf_status_host2, count_con_host1,
-                                                     count_con_host2, random_numbers, contact_rate_matrix):
-    counter = 0
-    type_inf_host1 = np.full(susceptible_host1.shape, 0, dtype=int)
-    type_inf_host2 = np.full(susceptible_host2.shape, 0, dtype=int)
-    for i in range(susceptible_host1.shape[0]):
-        if susceptible_host1[i]:
-            # host1 to host 1
-            if count_con_host1[pos_host1[i]] > 0:
-                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[0][0]) ** count_con_host1[pos_host1[i]]:
-                    inf_status_host1[i] = True
-                    type_inf_host1[i] += 1
-                counter += 1
-
-            # host2 to host1
-            if count_con_host2[pos_host1[i]] > 0:
-                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[1][0]) ** count_con_host2[pos_host1[i]]:
-                    inf_status_host1[i] = True
-                    type_inf_host1[i] += 2
-                counter += 1
-
-    for i in range(susceptible_host2.shape[0]):
-        if susceptible_host2[i]:
-            # host1 to host2
-            if count_con_host1[pos_host2[i]] > 0:
-                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[0][1]) ** count_con_host1[pos_host2[i]]:
-                    inf_status_host2[i] = True
-                    type_inf_host2[i] += 1
-                counter += 1
-
-            # host2 to host2
-            if count_con_host2[pos_host2[i]] > 0:
-                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[1][1]) ** count_con_host2[pos_host2[i]]:
-                    inf_status_host2[i] = True
-                    type_inf_host2[i] += 2
-                counter += 1
-
-    return type_inf_host1, type_inf_host2
+import numpy as np
+import numba as nb
+
+
+@nb.njit
+def base_contaminate_vertices(arr_new_infected, rand, level):
+    counter = 0
+    for i in range(arr_new_infected.shape[0]):
+        if arr_new_infected[i]:
+            if rand[counter] >= level:
+                arr_new_infected[i] = False
+            counter += 1
+
+
+@nb.njit
+def transition_initialize_counters_of_newly_infected(arr_new_infected, arr_cnt, arr_new_cnt):
+    counter = 0
+    for i in range(arr_new_infected.shape[0]):
+        if arr_new_infected[i]:
+            arr_cnt[i] = arr_new_cnt[counter]
+            counter += 1
+
+
+@nb.njit
+def transition_conditional_count_nb_agent_per_vertex(arr_condition, arr_pos, nb_vertex):
+    rv = np.zeros((nb_vertex,), dtype=np.int32)
+    for i in range(arr_pos.shape[0]):
+        if arr_condition[i]:
+            rv[arr_pos[i]] += 1
+    return rv
+
+
+@nb.njit
+def transition_falsify_when_condition(arr_bool, condition):
+    for i in range(arr_bool.shape[0]):
+        if condition[i]:
+            arr_bool[i] = False
+
+
+@nb.njit
+def transmission_conditional_count(nb_vertex, arr_pos, arr_cond):
+    pos_count = np.zeros((nb_vertex,), dtype=np.int32)
+    for i in range(arr_pos.shape[0]):
+        if arr_cond[i]:
+            pos_count[arr_pos[i]] += 1
+    return pos_count
+
+
+@nb.njit
+def transmission_count_needed_samples(susceptible, pos_susceptible, arr_count_con_host1, arr_count_con_host2):
+    needed_samples = 0
+    for i in range(susceptible.shape[0]):
+        if susceptible[i]:
+            needed_samples += (int(arr_count_con_host1[pos_susceptible[i]] > 0) +
+                               int(arr_count_con_host2[pos_susceptible[i]] > 0))
+    return needed_samples
+
+
+@nb.njit
+def transmission_disease_propagation(susceptible_host1, susceptible_host2, pos_host1, pos_host2, inf_status_host1,
+                                     inf_status_host2, count_con_host1, count_con_host2, random_numbers,
+                                     contact_rate_matrix):
+    counter = 0
+    for i in range(susceptible_host1.shape[0]):
+        if susceptible_host1[i]:
+            # host1 to host 1
+            if count_con_host1[pos_host1[i]] > 0:
+                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[0][0]) ** count_con_host1[pos_host1[i]]:
+                    inf_status_host1[i] = True
+                counter += 1
+
+            # host2 to host1
+            if count_con_host2[pos_host1[i]] > 0:
+                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[1][0]) ** count_con_host2[pos_host1[i]]:
+                    inf_status_host1[i] = True
+                counter += 1
+
+    for i in range(susceptible_host2.shape[0]):
+        if susceptible_host2[i]:
+            # host1 to host2
+            if count_con_host1[pos_host2[i]] > 0:
+                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[0][1]) ** count_con_host1[pos_host2[i]]:
+                    inf_status_host2[i] = True
+                counter += 1
+
+            # host2 to host2
+            if count_con_host2[pos_host2[i]] > 0:
+                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[1][1]) ** count_con_host2[pos_host2[i]]:
+                    inf_status_host2[i] = True
+                counter += 1
+
+
+@nb.njit
+def transmission_disease_propagation_return_new_inf(susceptible_host1, susceptible_host2, pos_host1, pos_host2,
+                                                    inf_status_host1, inf_status_host2, count_con_host1,
+                                                    count_con_host2, random_numbers, contact_rate_matrix):
+    counter = 0
+    new_infected_host1 = np.full(susceptible_host1.shape, False)
+    new_infected_host2 = np.full(susceptible_host2.shape, False)
+    for i in range(susceptible_host1.shape[0]):
+        if susceptible_host1[i]:
+            # host1 to host 1
+            if count_con_host1[pos_host1[i]] > 0:
+                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[0][0]) ** count_con_host1[pos_host1[i]]:
+                    inf_status_host1[i] = True
+                    new_infected_host1[i] = True
+                counter += 1
+
+            # host2 to host1
+            if count_con_host2[pos_host1[i]] > 0:
+                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[1][0]) ** count_con_host2[pos_host1[i]]:
+                    inf_status_host1[i] = True
+                    new_infected_host1[i] = True
+                counter += 1
+
+    for i in range(susceptible_host2.shape[0]):
+        if susceptible_host2[i]:
+            # host1 to host2
+            if count_con_host1[pos_host2[i]] > 0:
+                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[0][1]) ** count_con_host1[pos_host2[i]]:
+                    inf_status_host2[i] = True
+                    new_infected_host2[i] = True
+                counter += 1
+
+            # host2 to host2
+            if count_con_host2[pos_host2[i]] > 0:
+                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[1][1]) ** count_con_host2[pos_host2[i]]:
+                    inf_status_host2[i] = True
+                    new_infected_host2[i] = True
+                counter += 1
+
+    return new_infected_host1, new_infected_host2
+
+
+@nb.njit
+def transmission_disease_propagation_return_type_inf(susceptible_host1, susceptible_host2, pos_host1, pos_host2,
+                                                     inf_status_host1, inf_status_host2, count_con_host1,
+                                                     count_con_host2, random_numbers, contact_rate_matrix):
+    counter = 0
+    type_inf_host1 = np.full(susceptible_host1.shape, 0, dtype=int)
+    type_inf_host2 = np.full(susceptible_host2.shape, 0, dtype=int)
+    for i in range(susceptible_host1.shape[0]):
+        if susceptible_host1[i]:
+            # host1 to host 1
+            if count_con_host1[pos_host1[i]] > 0:
+                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[0][0]) ** count_con_host1[pos_host1[i]]:
+                    inf_status_host1[i] = True
+                    type_inf_host1[i] += 1
+                counter += 1
+
+            # host2 to host1
+            if count_con_host2[pos_host1[i]] > 0:
+                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[1][0]) ** count_con_host2[pos_host1[i]]:
+                    inf_status_host1[i] = True
+                    type_inf_host1[i] += 2
+                counter += 1
+
+    for i in range(susceptible_host2.shape[0]):
+        if susceptible_host2[i]:
+            # host1 to host2
+            if count_con_host1[pos_host2[i]] > 0:
+                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[0][1]) ** count_con_host1[pos_host2[i]]:
+                    inf_status_host2[i] = True
+                    type_inf_host2[i] += 1
+                counter += 1
+
+            # host2 to host2
+            if count_con_host2[pos_host2[i]] > 0:
+                if random_numbers[counter] < 1 - (1 - contact_rate_matrix[1][1]) ** count_con_host2[pos_host2[i]]:
+                    inf_status_host2[i] = True
+                    type_inf_host2[i] += 2
+                counter += 1
+
+    return type_inf_host1, type_inf_host2
```

### Comparing `sampy-abm-1.0.2/src/sampy/disease/two_species/transition.py` & `sampy_abm-1.0.3/src/sampy/disease/two_species/transition.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,222 +1,222 @@
-import numpy as np
-from ...utils.errors_shortcut import (check_input_array,
-                                      check_col_exists_good_type)
-from .jit_compiled_functions import (transition_initialize_counters_of_newly_infected,
-                                     transition_conditional_count_nb_agent_per_vertex,
-                                     transition_falsify_when_condition)
-
-
-class TransitionCustomProbPermanentImmunity:
-    """
-    This class introduce transitions between disease states based on probabilities given by the user. This class assumes
-    that the disease have two hosts, stored as attributes 'host1' and 'host2'.
-
-    WARNING: be aware that the time each agent spend in each status of the disease is kept in memory using counters.
-             Those counters HAVE TO be initialized for newly infected individuals throught the use of the method
-             'initialize_counters_of_newly_infected'. This problem is addressed by the 'simplified' methods in Sampy
-             built-in diseases.
-    """
-    def __init__(self, **kwargs):
-        self.host1.df_population['cnt_inf_' + self.disease_name] = 0
-        self.host1.df_population['cnt_con_' + self.disease_name] = 0
-        if hasattr(self.host1, 'dict_default_val'):
-            self.host1.dict_default_val['cnt_inf_' + self.disease_name] = 0
-            self.host1.dict_default_val['cnt_con_' + self.disease_name] = 0
-
-        self.host2.df_population['cnt_inf_' + self.disease_name] = 0
-        self.host2.df_population['cnt_con_' + self.disease_name] = 0
-        if hasattr(self.host2, 'dict_default_val'):
-            self.host2.dict_default_val['cnt_inf_' + self.disease_name] = 0
-            self.host2.dict_default_val['cnt_con_' + self.disease_name] = 0
-
-        self.on_ticker.append('decrement_counter')
-
-    def _sampy_debug_initialize_counters_of_newly_infected(self, host, arr_new_infected, arr_nb_timestep, arr_prob):
-        if host == "host1":
-            host = self.host1
-        elif host == "host2":
-            host = self.host2
-        else:
-            raise ValueError('The "host" argument is not recognized. It should be either "host1" or "host2".')
-
-        if host.df_population.nb_rows == 0:
-            return
-
-        check_input_array(arr_new_infected, 'arr_new_infected', 'bool',
-                          shape=(host.df_population.nb_rows,))
-        check_input_array(arr_nb_timestep, 'arr_nb_timestep', 'int', nb_dim=1)
-        check_input_array(arr_prob, 'arr_prob', 'float', nb_dim=1)
-
-        if arr_prob.shape != arr_nb_timestep.shape:
-            raise ValueError("Arguments 'arr_nb_timestep' and 'arr_prob' have different shapes.")
-
-    def initialize_counters_of_newly_infected(self, host, arr_new_infected, arr_nb_timestep, arr_prob):
-        """
-        Method that HAS TO be called each time new individuals get infected
-
-        :param host: string, either 'host1' or 'host2'. If host1 should be targeted, put 'host1', If host2 should be
-                     targeted, put 'host2'. Any other input will lead to an error.
-        :param arr_new_infected: 1d array of bool, saying which agent are newly infected and should have their
-                                 'infectious status counter' initialized.
-        :param arr_nb_timestep: 1d array of int. work in tandem with arr_prob, see below.
-        :param arr_prob: 1D array of float. arr_prob[i] is the probability for an agent to stay infected but not
-                         contagious for arr_nb_timestep[i] time-steps.
-
-        """
-        if host == 'host1':
-            host = self.host1
-        elif host == 'host2':
-            host = self.host2
-        else:
-            raise ValueError('The "host" argument is not recognized. It should be either "host1" or "host2".')
-
-        if host.df_population.nb_rows == 0:
-            return
-        prob = arr_prob.astype('float64')
-        prob = prob/prob.sum()
-        arr_cnt = np.random.choice(arr_nb_timestep, arr_new_infected.sum(), p=prob)
-
-        transition_initialize_counters_of_newly_infected(arr_new_infected,
-                                                         host.df_population['cnt_inf_' + self.disease_name],
-                                                         arr_cnt)
-
-    def decrement_counter(self):
-        """
-        Reduce by one the counters of the agents in a given disease state. Note that this method will only decrease
-        positive counters, so that if a negative counter was to appear, which shouldn't, this should be caused by
-        something else.
-        """
-        if self.host1.df_population.nb_rows > 0:
-            self.host1.df_population['cnt_inf_' + self.disease_name] -= \
-                self.host1.df_population['inf_' + self.disease_name] & (self.host1.df_population['cnt_inf_' + self.disease_name] > 0)
-            self.host1.df_population['cnt_con_' + self.disease_name] -= \
-                self.host1.df_population['con_' + self.disease_name] & (self.host1.df_population['cnt_con_' + self.disease_name] > 0)
-
-        if self.host2.df_population.nb_rows > 0:
-            self.host2.df_population['cnt_inf_' + self.disease_name] -= \
-                self.host2.df_population['inf_' + self.disease_name] & (self.host2.df_population['cnt_inf_' + self.disease_name] > 0)
-            self.host2.df_population['cnt_con_' + self.disease_name] -= \
-                self.host2.df_population['con_' + self.disease_name] & (self.host2.df_population['cnt_con_' + self.disease_name] > 0)
-
-    def _sampy_debug_transition_between_states(self, host, initial_state, target_state, condition=None, proba_death=1.,
-                                               arr_nb_timestep=None, arr_prob_nb_timestep=None,
-                                               return_transition_count=False, position_attribute='position'):
-
-        if host == 'host1':
-            host = self.host1
-        elif host == 'host2':
-            host = self.host2
-        else:
-            raise ValueError('The "host" argument is not recognized. It should be either "host1" or "host2".')
-
-        if host.df_population.nb_rows == 0:
-            return
-
-        if initial_state not in self.set_disease_status:
-            raise ValueError("Initial state is not in " + str(self.set_disease_status) + ".")
-        if target_state not in self.set_disease_status and target_state != 'death':
-            raise ValueError("Initial state is not in " + str(self.set_disease_status | {'death'}) + ".")
-
-        if condition is not None:
-            check_input_array(condition, 'condition', 'bool', shape=(host.df_population.nb_rows,))
-
-        if arr_nb_timestep is None and arr_prob_nb_timestep is not None:
-            raise ValueError("'arr_nb_timestep' is None while 'arr_prob_nb_timestep' is not.")
-
-        if arr_nb_timestep is not None and arr_prob_nb_timestep is None:
-            raise ValueError("'arr_prob_nb_timestep' is None while 'arr_nb_timestep' is not.")
-
-        if arr_nb_timestep is not None:
-            check_input_array(arr_nb_timestep, 'arr_nb_timestep', 'int', nb_dim=1)
-            check_input_array(arr_prob_nb_timestep, 'arr_prob_nb_timestep', 'float', nb_dim=1)
-            if arr_nb_timestep.shape != arr_prob_nb_timestep.shape:
-                raise ValueError("Arguments 'arr_nb_timestep' and 'arr_prob_nb_timestep' have different shapes.")
-
-        check_col_exists_good_type(host.df_population, position_attribute, 'position_attribute',
-                                   prefix_dtype='int', reject_none=True)
-
-    def transition_between_states(self, host, initial_state, target_state, condition=None, proba_death=1.,
-                                  arr_nb_timestep=None, arr_prob_nb_timestep=None, return_transition_count=False,
-                                  position_attribute='position'):
-        """
-        Performs the transition from an initial_state to a target_state of the disease, where 'death' is a possible
-        target_state. When performing the transition, each agent for which 'initial_state' is True and the associated
-        counter is 0 makes the transition (except if the target state is death proba_death is smaller than 1.).
-
-        WARNING: note that an agent can only be in a SINGLE state. That is, an agent cannot be simultaneously 'infected'
-                 and 'contagious'. So if the user wants, for instance, to count all agents carrying the disease, then
-                 both 'inf' and 'con' states have to be considered.
-
-        :param host: string, either 'host1' or 'host2'. If host1 should be targeted, put 'host1', If host2 should be
-                     targeted, put 'host2'. Any other input will lead to an error.
-        :param initial_state: string, in ['inf', 'con', 'imm']
-        :param target_state: string, in ['con', 'imm', 'death']
-        :param proba_death: optional, float, default 1.0. Probability of death if target_state=death.
-        :param arr_nb_timestep: optional, 1d array of int, default None.
-        :param arr_prob_nb_timestep: optional, 1d array of float, default None.
-        :param return_transition_count: optional, bool, default False. If True, returns a 1D array of integer counting
-                                        how many agents did the transition per cell.
-        :param position_attribute: optional, string, default 'position'. Name of the position attribute used for counting
-                                   if 'return_transition_count' is set to True.
-
-        :returns: if return_transition_count is True, returns a 1d array of int. Else, returns None.
-        """
-        if host == 'host1':
-            host = self.host1
-        elif host == 'host2':
-            host = self.host2
-        else:
-            raise ValueError('The "host" argument is not recognized. It should be either "host1" or "host2".')
-
-        if host.df_population.nb_rows == 0:
-            return
-
-        # bool array of all individuals that will make transition
-        susceptible = host.df_population['cnt_' + initial_state + '_' + self.disease_name] == 0
-        susceptible = susceptible & host.df_population[initial_state + '_' + self.disease_name]
-        if condition is not None:
-            susceptible = susceptible & condition
-
-        count_arr = None
-
-        # in case of death
-        if target_state == 'death':
-            # there might be a probability of dying of the disease, which is taken into account now
-            if proba_death < 1.:
-                susceptible = susceptible & \
-                              (np.random.uniform(0, 1, (host.df_population.shape[0],)) < proba_death)
-
-            if return_transition_count:
-                count_arr = transition_conditional_count_nb_agent_per_vertex(susceptible,
-                                                                             host.df_population[position_attribute],
-                                                                             host.graph.connections.shape[0])
-
-            # killing
-            host.df_population = host.df_population[~susceptible]
-
-        # all the rest corresponds to transition between stages of the disease
-        else:
-            if return_transition_count:
-                count_arr = transition_conditional_count_nb_agent_per_vertex(susceptible,
-                                                                             host.df_population[position_attribute],
-                                                                             host.graph.connections.shape[0])
-
-            host.df_population[target_state + '_' + self.disease_name] = susceptible | host.df_population[
-                target_state + '_' + self.disease_name]
-            if target_state == 'imm':
-                transition_falsify_when_condition(host.df_population['inf_' + self.disease_name], susceptible)
-                transition_falsify_when_condition(host.df_population['con_' + self.disease_name], susceptible)
-
-            else:
-                transition_falsify_when_condition(host.df_population[initial_state + '_' + self.disease_name],
-                                                  susceptible)
-
-                prob = arr_prob_nb_timestep.astype('float64')
-                prob = prob / prob.sum()
-                arr_cnt = np.random.choice(arr_nb_timestep, susceptible.sum(), p=prob)
-
-                transition_initialize_counters_of_newly_infected(susceptible,
-                                                                 host.df_population[
-                                                                     'cnt_' + target_state + '_' + self.disease_name],
-                                                                 arr_cnt)
-        return count_arr
+import numpy as np
+from ...utils.errors_shortcut import (check_input_array,
+                                      check_col_exists_good_type)
+from .jit_compiled_functions import (transition_initialize_counters_of_newly_infected,
+                                     transition_conditional_count_nb_agent_per_vertex,
+                                     transition_falsify_when_condition)
+
+
+class TransitionCustomProbPermanentImmunity:
+    """
+    This class introduce transitions between disease states based on probabilities given by the user. This class assumes
+    that the disease have two hosts, stored as attributes 'host1' and 'host2'.
+
+    WARNING: be aware that the time each agent spend in each status of the disease is kept in memory using counters.
+             Those counters HAVE TO be initialized for newly infected individuals throught the use of the method
+             'initialize_counters_of_newly_infected'. This problem is addressed by the 'simplified' methods in Sampy
+             built-in diseases.
+    """
+    def __init__(self, **kwargs):
+        self.host1.df_population['cnt_inf_' + self.disease_name] = 0
+        self.host1.df_population['cnt_con_' + self.disease_name] = 0
+        if hasattr(self.host1, 'dict_default_val'):
+            self.host1.dict_default_val['cnt_inf_' + self.disease_name] = 0
+            self.host1.dict_default_val['cnt_con_' + self.disease_name] = 0
+
+        self.host2.df_population['cnt_inf_' + self.disease_name] = 0
+        self.host2.df_population['cnt_con_' + self.disease_name] = 0
+        if hasattr(self.host2, 'dict_default_val'):
+            self.host2.dict_default_val['cnt_inf_' + self.disease_name] = 0
+            self.host2.dict_default_val['cnt_con_' + self.disease_name] = 0
+
+        self.on_ticker.append('decrement_counter')
+
+    def _sampy_debug_initialize_counters_of_newly_infected(self, host, arr_new_infected, arr_nb_timestep, arr_prob):
+        if host == "host1":
+            host = self.host1
+        elif host == "host2":
+            host = self.host2
+        else:
+            raise ValueError('The "host" argument is not recognized. It should be either "host1" or "host2".')
+
+        if host.df_population.nb_rows == 0:
+            return
+
+        check_input_array(arr_new_infected, 'arr_new_infected', 'bool',
+                          shape=(host.df_population.nb_rows,))
+        check_input_array(arr_nb_timestep, 'arr_nb_timestep', 'int', nb_dim=1)
+        check_input_array(arr_prob, 'arr_prob', 'float', nb_dim=1)
+
+        if arr_prob.shape != arr_nb_timestep.shape:
+            raise ValueError("Arguments 'arr_nb_timestep' and 'arr_prob' have different shapes.")
+
+    def initialize_counters_of_newly_infected(self, host, arr_new_infected, arr_nb_timestep, arr_prob):
+        """
+        Method that HAS TO be called each time new individuals get infected
+
+        :param host: string, either 'host1' or 'host2'. If host1 should be targeted, put 'host1', If host2 should be
+                     targeted, put 'host2'. Any other input will lead to an error.
+        :param arr_new_infected: 1d array of bool, saying which agent are newly infected and should have their
+                                 'infectious status counter' initialized.
+        :param arr_nb_timestep: 1d array of int. work in tandem with arr_prob, see below.
+        :param arr_prob: 1D array of float. arr_prob[i] is the probability for an agent to stay infected but not
+                         contagious for arr_nb_timestep[i] time-steps.
+
+        """
+        if host == 'host1':
+            host = self.host1
+        elif host == 'host2':
+            host = self.host2
+        else:
+            raise ValueError('The "host" argument is not recognized. It should be either "host1" or "host2".')
+
+        if host.df_population.nb_rows == 0:
+            return
+        prob = arr_prob.astype('float64')
+        prob = prob/prob.sum()
+        arr_cnt = np.random.choice(arr_nb_timestep, arr_new_infected.sum(), p=prob)
+
+        transition_initialize_counters_of_newly_infected(arr_new_infected,
+                                                         host.df_population['cnt_inf_' + self.disease_name],
+                                                         arr_cnt)
+
+    def decrement_counter(self):
+        """
+        Reduce by one the counters of the agents in a given disease state. Note that this method will only decrease
+        positive counters, so that if a negative counter was to appear, which shouldn't, this should be caused by
+        something else.
+        """
+        if self.host1.df_population.nb_rows > 0:
+            self.host1.df_population['cnt_inf_' + self.disease_name] -= \
+                self.host1.df_population['inf_' + self.disease_name] & (self.host1.df_population['cnt_inf_' + self.disease_name] > 0)
+            self.host1.df_population['cnt_con_' + self.disease_name] -= \
+                self.host1.df_population['con_' + self.disease_name] & (self.host1.df_population['cnt_con_' + self.disease_name] > 0)
+
+        if self.host2.df_population.nb_rows > 0:
+            self.host2.df_population['cnt_inf_' + self.disease_name] -= \
+                self.host2.df_population['inf_' + self.disease_name] & (self.host2.df_population['cnt_inf_' + self.disease_name] > 0)
+            self.host2.df_population['cnt_con_' + self.disease_name] -= \
+                self.host2.df_population['con_' + self.disease_name] & (self.host2.df_population['cnt_con_' + self.disease_name] > 0)
+
+    def _sampy_debug_transition_between_states(self, host, initial_state, target_state, condition=None, proba_death=1.,
+                                               arr_nb_timestep=None, arr_prob_nb_timestep=None,
+                                               return_transition_count=False, position_attribute='position'):
+
+        if host == 'host1':
+            host = self.host1
+        elif host == 'host2':
+            host = self.host2
+        else:
+            raise ValueError('The "host" argument is not recognized. It should be either "host1" or "host2".')
+
+        if host.df_population.nb_rows == 0:
+            return
+
+        if initial_state not in self.set_disease_status:
+            raise ValueError("Initial state is not in " + str(self.set_disease_status) + ".")
+        if target_state not in self.set_disease_status and target_state != 'death':
+            raise ValueError("Initial state is not in " + str(self.set_disease_status | {'death'}) + ".")
+
+        if condition is not None:
+            check_input_array(condition, 'condition', 'bool', shape=(host.df_population.nb_rows,))
+
+        if arr_nb_timestep is None and arr_prob_nb_timestep is not None:
+            raise ValueError("'arr_nb_timestep' is None while 'arr_prob_nb_timestep' is not.")
+
+        if arr_nb_timestep is not None and arr_prob_nb_timestep is None:
+            raise ValueError("'arr_prob_nb_timestep' is None while 'arr_nb_timestep' is not.")
+
+        if arr_nb_timestep is not None:
+            check_input_array(arr_nb_timestep, 'arr_nb_timestep', 'int', nb_dim=1)
+            check_input_array(arr_prob_nb_timestep, 'arr_prob_nb_timestep', 'float', nb_dim=1)
+            if arr_nb_timestep.shape != arr_prob_nb_timestep.shape:
+                raise ValueError("Arguments 'arr_nb_timestep' and 'arr_prob_nb_timestep' have different shapes.")
+
+        check_col_exists_good_type(host.df_population, position_attribute, 'position_attribute',
+                                   prefix_dtype='int', reject_none=True)
+
+    def transition_between_states(self, host, initial_state, target_state, condition=None, proba_death=1.,
+                                  arr_nb_timestep=None, arr_prob_nb_timestep=None, return_transition_count=False,
+                                  position_attribute='position'):
+        """
+        Performs the transition from an initial_state to a target_state of the disease, where 'death' is a possible
+        target_state. When performing the transition, each agent for which 'initial_state' is True and the associated
+        counter is 0 makes the transition (except if the target state is death proba_death is smaller than 1.).
+
+        WARNING: note that an agent can only be in a SINGLE state. That is, an agent cannot be simultaneously 'infected'
+                 and 'contagious'. So if the user wants, for instance, to count all agents carrying the disease, then
+                 both 'inf' and 'con' states have to be considered.
+
+        :param host: string, either 'host1' or 'host2'. If host1 should be targeted, put 'host1', If host2 should be
+                     targeted, put 'host2'. Any other input will lead to an error.
+        :param initial_state: string, in ['inf', 'con', 'imm']
+        :param target_state: string, in ['con', 'imm', 'death']
+        :param proba_death: optional, float, default 1.0. Probability of death if target_state=death.
+        :param arr_nb_timestep: optional, 1d array of int, default None.
+        :param arr_prob_nb_timestep: optional, 1d array of float, default None.
+        :param return_transition_count: optional, bool, default False. If True, returns a 1D array of integer counting
+                                        how many agents did the transition per cell.
+        :param position_attribute: optional, string, default 'position'. Name of the position attribute used for counting
+                                   if 'return_transition_count' is set to True.
+
+        :returns: if return_transition_count is True, returns a 1d array of int. Else, returns None.
+        """
+        if host == 'host1':
+            host = self.host1
+        elif host == 'host2':
+            host = self.host2
+        else:
+            raise ValueError('The "host" argument is not recognized. It should be either "host1" or "host2".')
+
+        if host.df_population.nb_rows == 0:
+            return
+
+        # bool array of all individuals that will make transition
+        susceptible = host.df_population['cnt_' + initial_state + '_' + self.disease_name] == 0
+        susceptible = susceptible & host.df_population[initial_state + '_' + self.disease_name]
+        if condition is not None:
+            susceptible = susceptible & condition
+
+        count_arr = None
+
+        # in case of death
+        if target_state == 'death':
+            # there might be a probability of dying of the disease, which is taken into account now
+            if proba_death < 1.:
+                susceptible = susceptible & \
+                              (np.random.uniform(0, 1, (host.df_population.shape[0],)) < proba_death)
+
+            if return_transition_count:
+                count_arr = transition_conditional_count_nb_agent_per_vertex(susceptible,
+                                                                             host.df_population[position_attribute],
+                                                                             host.graph.connections.shape[0])
+
+            # killing
+            host.df_population = host.df_population[~susceptible]
+
+        # all the rest corresponds to transition between stages of the disease
+        else:
+            if return_transition_count:
+                count_arr = transition_conditional_count_nb_agent_per_vertex(susceptible,
+                                                                             host.df_population[position_attribute],
+                                                                             host.graph.connections.shape[0])
+
+            host.df_population[target_state + '_' + self.disease_name] = susceptible | host.df_population[
+                target_state + '_' + self.disease_name]
+            if target_state == 'imm':
+                transition_falsify_when_condition(host.df_population['inf_' + self.disease_name], susceptible)
+                transition_falsify_when_condition(host.df_population['con_' + self.disease_name], susceptible)
+
+            else:
+                transition_falsify_when_condition(host.df_population[initial_state + '_' + self.disease_name],
+                                                  susceptible)
+
+                prob = arr_prob_nb_timestep.astype('float64')
+                prob = prob / prob.sum()
+                arr_cnt = np.random.choice(arr_nb_timestep, susceptible.sum(), p=prob)
+
+                transition_initialize_counters_of_newly_infected(susceptible,
+                                                                 host.df_population[
+                                                                     'cnt_' + target_state + '_' + self.disease_name],
+                                                                 arr_cnt)
+        return count_arr
```

### Comparing `sampy-abm-1.0.2/src/sampy/disease/two_species/transmission.py` & `sampy_abm-1.0.3/src/sampy/disease/two_species/transmission.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-import numpy as np
-from .jit_compiled_functions import (transmission_conditional_count,
-                                     transmission_count_needed_samples,
-                                     transmission_disease_propagation,
-                                     transmission_disease_propagation_return_new_inf,
-                                     transmission_disease_propagation_return_type_inf)
-from ...utils.errors_shortcut import (check_input_array,
-                                      check_col_exists_good_type)
-
-
-class ContactTransmissionSameGraph:
-    """
-    The disease is spread by direct contact between the agents. Both populations are assumed to live on the same graph.
-    """
-    def __init__(self, **kwargs):
-        pass
-
-    def _sampy_debug_contact_contagion(self, contact_rate_matrix, position_attribute_host1='position',
-                                       position_attribute_host2='position', condition_host1=None, condition_host2=None,
-                                       return_arr_new_infected=False, return_type_transmission=False):
-        if not isinstance(contact_rate_matrix, np.ndarray):
-            raise ValueError("contact_rate_matrix argument should be a ndarray of shape (2, 2).")
-        if self.host1.df_population.nb_rows > 0:
-            check_col_exists_good_type(self.host1.df_population, position_attribute_host1, 'position_attribute_host1',
-                                       prefix_dtype='int', reject_none=True)
-            if condition_host1 is not None:
-                check_input_array(condition_host1, "condition_host1", "bool", shape=(self.host1.df_population.nb_rows,))
-        if self.host2.df_population.nb_rows > 0:
-            check_col_exists_good_type(self.host2.df_population, position_attribute_host2, 'position_attribute_host2',
-                                       prefix_dtype='int', reject_none=True)
-            if condition_host2 is not None:
-                check_input_array(condition_host2, "condition_host2", "bool", shape=(self.host2.df_population.nb_rows,))
-
-    def contact_contagion(self, contact_rate_matrix, position_attribute_host1='position',
-                          position_attribute_host2='position', condition_host1=None, condition_host2=None,
-                          return_arr_new_infected=False, return_type_transmission=False):
-        """
-        Propagate the disease by direct contact using the following methodology.
-
-        We denote by N_{v, host_i} the number of contagious agents of the species host_i on the vertex v of the graph.
-        Then, for any susceptible agent of the species host_j living on the vertex v, the probability for this agent to
-        be contaminated by an infected agent of the species host_i is given by:
-
-                            1 - (1 - contact_rate_{i,j}) ** N_{c, host_i}
-
-        In practice, for any susceptible agent, we perform two independent tests (one for each host species) and if any
-        of those test is a success, the agent is contaminated.
-
-        :param contact_rate_matrix: 2D array of floats of shape (2, 2). Here, contact_rate_matrix[0][0] is the
-                                    probability of contact contagion from host1 to host1, contact_rate_matrix[0][1] is
-                                    the probability of contact contagion from host1 to host2, etc...
-        :param position_attribute_host1: optional, string, default 'position'. Name of the agent attribute used as
-                                         position for host1.
-        :param position_attribute_host2: optional, string, default 'position'. Name of the agent attribute used as
-                                         position for host2.
-        :param condition_host1: optional, array of bool, default None. Array of boolean such that the i-th value is
-                          True if and only if the i-th agent of host1 (i.e. the agent at the line i of df_population)
-                          can be infected and transmit disease. All the agent having their corresponding value to False
-                          are protected from infection and cannot transmit the disease.
-        :param condition_host2: optional, array of bool, default None. Array of boolean such that the i-th value is
-                          True if and only if the i-th agent of host2 (i.e. the agent at the line i of df_population)
-                          can be infected and transmit disease. All the agent having their corresponding value to False
-                          are protected from infection and cannot transmit the disease.
-        :param return_arr_new_infected: optional, boolean, default False. If True, the method returns two arrays telling
-                                        which agent got contaminated in each host species.
-        :param return_type_transmission: optional, boolean, default False.
-
-        :return: Depending on the values of the parameters 'return_arr_new_infected' and 'return_type_transmission',
-                 the return value will either be None (both are False) or a dictionnary whose key-values are:
-                    - 'arr_new_infected_host1', 'arr_new_infected_host2' if return_arr_new_infected is True, and the
-                      values are 1D arrays of bool telling which agents got infected for each host;
-                    - 'arr_type_transmission_host1', 'arr_type_transmission_host2' if return_type_transmission is True,
-                      and the values are 1D arrays of non-negative integers such that the integer at line i is 0 if the
-                      i-th agent has not been contaminated, 1 if it has been contaminated by a member of its own species
-                      2 if it has been contaminated by a member of the other species, 3 if it has been contaminated by
-                      agents from both its species and the other.
-        """
-        if self.host1.df_population.nb_rows > 0:
-            pos_host1 = self.host1.df_population[position_attribute_host1]
-            contagious_host1 = self.host1.df_population['con_' + self.disease_name]
-            susceptible_host1 = ~(self.host1.df_population['inf_' + self.disease_name] |
-                                  self.host1.df_population['con_' + self.disease_name] |
-                                  self.host1.df_population['imm_' + self.disease_name])
-            if condition_host1 is not None:
-                contagious_host1 = contagious_host1 & condition_host1
-                susceptible_host1 = susceptible_host1 & condition_host1
-            count_con_host1 = transmission_conditional_count(self.host1.graph.number_vertices, pos_host1,
-                                                             contagious_host1)
-        else:
-            if self.host2.df_population.nb_rows == 0:
-                return
-            # not the best hack, but the case where one of the two species died off should not be very common,
-            # todo: change this for a properly optimized branch instead of this dirty hack
-            pos_host1 = np.array([0])
-            count_con_host1 = np.full((self.host1.graph.number_vertices,), 0, dtype=int)
-            susceptible_host1 = np.array([False])
-
-        if self.host2.df_population.nb_rows > 0:
-            pos_host2 = self.host2.df_population[position_attribute_host2]
-            contagious_host2 = self.host2.df_population['con_' + self.disease_name]
-            susceptible_host2 = ~(self.host2.df_population['inf_' + self.disease_name] |
-                                  self.host2.df_population['con_' + self.disease_name] |
-                                  self.host2.df_population['imm_' + self.disease_name])
-            if condition_host2 is not None:
-                contagious_host2 = contagious_host2 & condition_host2
-                susceptible_host1 = susceptible_host1 & condition_host1
-            count_con_host2 = transmission_conditional_count(self.host2.graph.number_vertices, pos_host2,
-                                                             contagious_host2)
-        else:
-            # the case of both species having died out has already been treated.
-            # todo: see above, same problem of dirty hack
-            pos_host2 = np.array([0])
-            count_con_host2 = np.full((self.host2.graph.number_vertices,), 0, dtype=int)
-            susceptible_host2 = np.array([False])
-
-        # we now take care of the contaminations
-        nb_samples_host1 = transmission_count_needed_samples(susceptible_host1, pos_host1, count_con_host1,
-                                                             count_con_host2)
-        nb_samples_host2 = transmission_count_needed_samples(susceptible_host2, pos_host2, count_con_host1,
-                                                             count_con_host2)
-        random_numbers = np.random.uniform(0, 1, (nb_samples_host1 + nb_samples_host2,))
-
-        rv = None
-        if return_arr_new_infected and not return_type_transmission:
-            rv = {}
-            new_inf_host1, new_inf_host2 = transmission_disease_propagation_return_new_inf(
-                                                                   susceptible_host1, susceptible_host2,
-                                                                   self.host1.df_population[position_attribute_host1],
-                                                                   self.host2.df_population[position_attribute_host2],
-                                                                   self.host1.df_population['inf_' + self.disease_name],
-                                                                   self.host2.df_population['inf_' + self.disease_name],
-                                                                   count_con_host1, count_con_host2,
-                                                                   random_numbers, contact_rate_matrix)
-            rv['arr_new_infected_host1'] = new_inf_host1
-            rv['arr_new_infected_host2'] = new_inf_host2
-            return rv
-        if return_type_transmission:
-            rv = {}
-            type_inf_host1, type_inf_host2 = transmission_disease_propagation_return_type_inf(
-                                                                   susceptible_host1, susceptible_host2,
-                                                                   self.host1.df_population[position_attribute_host1],
-                                                                   self.host2.df_population[position_attribute_host2],
-                                                                   self.host1.df_population['inf_' + self.disease_name],
-                                                                   self.host2.df_population['inf_' + self.disease_name],
-                                                                   count_con_host1, count_con_host2,
-                                                                   random_numbers, contact_rate_matrix)
-            rv['arr_type_transmission_host1'] = type_inf_host1
-            rv['arr_type_transmission_host2'] = type_inf_host2
-            if return_arr_new_infected:
-                rv['arr_new_infected_host1'] = type_inf_host1 > 0
-                rv['arr_new_infected_host2'] = type_inf_host2 > 0
-            return rv
-
-        # case where nothing is returned
-        transmission_disease_propagation(susceptible_host1, susceptible_host2,
-                                         self.host1.df_population[position_attribute_host1],
-                                         self.host2.df_population[position_attribute_host2],
-                                         self.host1.df_population['inf_' + self.disease_name],
-                                         self.host2.df_population['inf_' + self.disease_name],
-                                         count_con_host1, count_con_host2,
-                                         random_numbers, contact_rate_matrix)
-        return rv
+import numpy as np
+from .jit_compiled_functions import (transmission_conditional_count,
+                                     transmission_count_needed_samples,
+                                     transmission_disease_propagation,
+                                     transmission_disease_propagation_return_new_inf,
+                                     transmission_disease_propagation_return_type_inf)
+from ...utils.errors_shortcut import (check_input_array,
+                                      check_col_exists_good_type)
+
+
+class ContactTransmissionSameGraph:
+    """
+    The disease is spread by direct contact between the agents. Both populations are assumed to live on the same graph.
+    """
+    def __init__(self, **kwargs):
+        pass
+
+    def _sampy_debug_contact_contagion(self, contact_rate_matrix, position_attribute_host1='position',
+                                       position_attribute_host2='position', condition_host1=None, condition_host2=None,
+                                       return_arr_new_infected=False, return_type_transmission=False):
+        if not isinstance(contact_rate_matrix, np.ndarray):
+            raise ValueError("contact_rate_matrix argument should be a ndarray of shape (2, 2).")
+        if self.host1.df_population.nb_rows > 0:
+            check_col_exists_good_type(self.host1.df_population, position_attribute_host1, 'position_attribute_host1',
+                                       prefix_dtype='int', reject_none=True)
+            if condition_host1 is not None:
+                check_input_array(condition_host1, "condition_host1", "bool", shape=(self.host1.df_population.nb_rows,))
+        if self.host2.df_population.nb_rows > 0:
+            check_col_exists_good_type(self.host2.df_population, position_attribute_host2, 'position_attribute_host2',
+                                       prefix_dtype='int', reject_none=True)
+            if condition_host2 is not None:
+                check_input_array(condition_host2, "condition_host2", "bool", shape=(self.host2.df_population.nb_rows,))
+
+    def contact_contagion(self, contact_rate_matrix, position_attribute_host1='position',
+                          position_attribute_host2='position', condition_host1=None, condition_host2=None,
+                          return_arr_new_infected=False, return_type_transmission=False):
+        """
+        Propagate the disease by direct contact using the following methodology.
+
+        We denote by N_{v, host_i} the number of contagious agents of the species host_i on the vertex v of the graph.
+        Then, for any susceptible agent of the species host_j living on the vertex v, the probability for this agent to
+        be contaminated by an infected agent of the species host_i is given by:
+
+                            1 - (1 - contact_rate_{i,j}) ** N_{c, host_i}
+
+        In practice, for any susceptible agent, we perform two independent tests (one for each host species) and if any
+        of those test is a success, the agent is contaminated.
+
+        :param contact_rate_matrix: 2D array of floats of shape (2, 2). Here, contact_rate_matrix[0][0] is the
+                                    probability of contact contagion from host1 to host1, contact_rate_matrix[0][1] is
+                                    the probability of contact contagion from host1 to host2, etc...
+        :param position_attribute_host1: optional, string, default 'position'. Name of the agent attribute used as
+                                         position for host1.
+        :param position_attribute_host2: optional, string, default 'position'. Name of the agent attribute used as
+                                         position for host2.
+        :param condition_host1: optional, array of bool, default None. Array of boolean such that the i-th value is
+                          True if and only if the i-th agent of host1 (i.e. the agent at the line i of df_population)
+                          can be infected and transmit disease. All the agent having their corresponding value to False
+                          are protected from infection and cannot transmit the disease.
+        :param condition_host2: optional, array of bool, default None. Array of boolean such that the i-th value is
+                          True if and only if the i-th agent of host2 (i.e. the agent at the line i of df_population)
+                          can be infected and transmit disease. All the agent having their corresponding value to False
+                          are protected from infection and cannot transmit the disease.
+        :param return_arr_new_infected: optional, boolean, default False. If True, the method returns two arrays telling
+                                        which agent got contaminated in each host species.
+        :param return_type_transmission: optional, boolean, default False.
+
+        :return: Depending on the values of the parameters 'return_arr_new_infected' and 'return_type_transmission',
+                 the return value will either be None (both are False) or a dictionnary whose key-values are:
+                    - 'arr_new_infected_host1', 'arr_new_infected_host2' if return_arr_new_infected is True, and the
+                      values are 1D arrays of bool telling which agents got infected for each host;
+                    - 'arr_type_transmission_host1', 'arr_type_transmission_host2' if return_type_transmission is True,
+                      and the values are 1D arrays of non-negative integers such that the integer at line i is 0 if the
+                      i-th agent has not been contaminated, 1 if it has been contaminated by a member of its own species
+                      2 if it has been contaminated by a member of the other species, 3 if it has been contaminated by
+                      agents from both its species and the other.
+        """
+        if self.host1.df_population.nb_rows > 0:
+            pos_host1 = self.host1.df_population[position_attribute_host1]
+            contagious_host1 = self.host1.df_population['con_' + self.disease_name]
+            susceptible_host1 = ~(self.host1.df_population['inf_' + self.disease_name] |
+                                  self.host1.df_population['con_' + self.disease_name] |
+                                  self.host1.df_population['imm_' + self.disease_name])
+            if condition_host1 is not None:
+                contagious_host1 = contagious_host1 & condition_host1
+                susceptible_host1 = susceptible_host1 & condition_host1
+            count_con_host1 = transmission_conditional_count(self.host1.graph.number_vertices, pos_host1,
+                                                             contagious_host1)
+        else:
+            if self.host2.df_population.nb_rows == 0:
+                return
+            # not the best hack, but the case where one of the two species died off should not be very common,
+            # todo: change this for a properly optimized branch instead of this dirty hack
+            pos_host1 = np.array([0])
+            count_con_host1 = np.full((self.host1.graph.number_vertices,), 0, dtype=int)
+            susceptible_host1 = np.array([False])
+
+        if self.host2.df_population.nb_rows > 0:
+            pos_host2 = self.host2.df_population[position_attribute_host2]
+            contagious_host2 = self.host2.df_population['con_' + self.disease_name]
+            susceptible_host2 = ~(self.host2.df_population['inf_' + self.disease_name] |
+                                  self.host2.df_population['con_' + self.disease_name] |
+                                  self.host2.df_population['imm_' + self.disease_name])
+            if condition_host2 is not None:
+                contagious_host2 = contagious_host2 & condition_host2
+                susceptible_host2 = susceptible_host2 & condition_host2
+            count_con_host2 = transmission_conditional_count(self.host2.graph.number_vertices, pos_host2,
+                                                             contagious_host2)
+        else:
+            # the case of both species having died out has already been treated.
+            # todo: see above, same problem of dirty hack
+            pos_host2 = np.array([0])
+            count_con_host2 = np.full((self.host2.graph.number_vertices,), 0, dtype=int)
+            susceptible_host2 = np.array([False])
+
+        # we now take care of the contaminations
+        nb_samples_host1 = transmission_count_needed_samples(susceptible_host1, pos_host1, count_con_host1,
+                                                             count_con_host2)
+        nb_samples_host2 = transmission_count_needed_samples(susceptible_host2, pos_host2, count_con_host1,
+                                                             count_con_host2)
+        random_numbers = np.random.uniform(0, 1, (nb_samples_host1 + nb_samples_host2,))
+
+        rv = None
+        if return_arr_new_infected and not return_type_transmission:
+            rv = {}
+            new_inf_host1, new_inf_host2 = transmission_disease_propagation_return_new_inf(
+                                                                   susceptible_host1, susceptible_host2,
+                                                                   self.host1.df_population[position_attribute_host1],
+                                                                   self.host2.df_population[position_attribute_host2],
+                                                                   self.host1.df_population['inf_' + self.disease_name],
+                                                                   self.host2.df_population['inf_' + self.disease_name],
+                                                                   count_con_host1, count_con_host2,
+                                                                   random_numbers, contact_rate_matrix)
+            rv['arr_new_infected_host1'] = new_inf_host1
+            rv['arr_new_infected_host2'] = new_inf_host2
+            return rv
+        if return_type_transmission:
+            rv = {}
+            type_inf_host1, type_inf_host2 = transmission_disease_propagation_return_type_inf(
+                                                                   susceptible_host1, susceptible_host2,
+                                                                   self.host1.df_population[position_attribute_host1],
+                                                                   self.host2.df_population[position_attribute_host2],
+                                                                   self.host1.df_population['inf_' + self.disease_name],
+                                                                   self.host2.df_population['inf_' + self.disease_name],
+                                                                   count_con_host1, count_con_host2,
+                                                                   random_numbers, contact_rate_matrix)
+            rv['arr_type_transmission_host1'] = type_inf_host1
+            rv['arr_type_transmission_host2'] = type_inf_host2
+            if return_arr_new_infected:
+                rv['arr_new_infected_host1'] = type_inf_host1 > 0
+                rv['arr_new_infected_host2'] = type_inf_host2 > 0
+            return rv
+
+        # case where nothing is returned
+        transmission_disease_propagation(susceptible_host1, susceptible_host2,
+                                         self.host1.df_population[position_attribute_host1],
+                                         self.host2.df_population[position_attribute_host2],
+                                         self.host1.df_population['inf_' + self.disease_name],
+                                         self.host2.df_population['inf_' + self.disease_name],
+                                         count_con_host1, count_con_host2,
+                                         random_numbers, contact_rate_matrix)
+        return rv
```

### Comparing `sampy-abm-1.0.2/src/sampy/graph/from_files.py` & `sampy_abm-1.0.3/src/sampy/graph/from_files.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,161 +1,161 @@
-from ..pandas_xs.pandas_xs import DataFrameXS
-from .misc import convert_graph_structure_to_dictionary
-
-import numpy as np
-import os
-import shutil
-import json
-import glob
-
-
-class SaveAndLoadSquareGrids:
-    """
-    Add to the square grids graphs the possibility to save them using their own special format.
-
-    We also provide a Json
-    """
-    def __init__(self, **kwargs):
-        pass
-
-    def save(self, path_to_folder, erase_folder=True):
-        """
-        Save the graph structure in a folder using .npy files. The end result is not human readable.
-
-        :param path_to_folder: Path to the folder. If it does not exists, the folder will be created.
-        :param erase_folder: optional, boolean, default True. If True, any folder already existing at 'path_to_folder'
-                             will be deleted.
-        """
-        if os.path.exists(path_to_folder):
-            if not erase_folder:
-                raise OSError("Something already exists at " + path_to_folder + '.')
-            if not os.path.isdir(path_to_folder):
-                raise OSError("The object at " + path_to_folder + " is not a directory. In doubt, we prefer not to " +
-                              "delete it.")
-            shutil.rmtree(path_to_folder)
-        os.mkdir(path_to_folder)
-
-        np.save(path_to_folder + '/connections.npy', self.connections)
-        np.save(path_to_folder + '/weights.npy', self.weights)
-
-        attributes_that_are_none = []
-        for name in self.df_attributes.list_col_name:
-            if self.df_attributes[name] is not None:
-                np.save(path_to_folder + '/attr_' + name + '.npy', self.df_attributes[name])
-            else:
-                attributes_that_are_none.append(name)
-
-        metadata_json = {'shape_0': self.shape[0],
-                         'shape_1': self.shape[1],
-                         'type': self.type,
-                         'attributes_none': attributes_that_are_none}
-        metadata = open(path_to_folder + '/metadata_json.json', 'w')
-        metadata.write(json.dumps(metadata_json))
-        metadata.close()
-
-    @classmethod
-    def load(cls, path_to_folder):
-        """
-
-        :param path_to_folder:
-        :return:
-        """
-        if os.path.exists(path_to_folder):
-            if not os.path.isdir(path_to_folder):
-                raise OSError("The object at " + path_to_folder + " is not a directory.")
-        else:
-            raise OSError("Nothing at " + path_to_folder + '.')
-
-        metadata = json.load(open(path_to_folder + '/metadata_json.json'))
-        shape = (metadata['shape_0'], metadata['shape_1'])
-        graph_type = metadata['type']
-
-        graph = cls(shape=shape)
-        graph.type = graph_type
-        graph.shape = shape
-
-        graph.connections = np.load(path_to_folder + '/connections.npy')
-        graph.weights = np.load(path_to_folder + '/weights.npy')
-
-        for path in glob.glob(path_to_folder + '/*'):
-            if os.path.basename(path).startswith('attr_'):
-                name = os.path.basename(path).split('.')[0]
-                name = name[5:]
-                graph.df_attributes[name] = np.load(path)
-
-        for name in metadata['attributes_none']:
-            graph.df_attributes[name] = None
-
-        return graph
-
-    def save_as_json(self, path_to_json, erase_existing_file=False):
-        """
-        Save a SquareGrid graph as a JSON. This is not the recommended way of saving a
-
-        :param path_to_json:
-        :param erase_existing_file:
-        """
-        if os.path.exists(path_to_json):
-            if not erase_existing_file:
-                raise OSError("Something already exists at " + path_to_json + '.')
-            os.remove(path_to_json)
-
-        dict_graph_structure = convert_graph_structure_to_dictionary(self, save_vertices_index=True,
-                                                                     add_to_metadata={'is_SquareGrid': True,
-                                                                                      'shape_0': self.shape[0],
-                                                                                      'shape_1': self.shape[1]})
-
-        graph_json = open(path_to_json, 'w')
-        graph_json.write(json.dumps(dict_graph_structure))
-        graph_json.close()
-
-    @classmethod
-    def from_json(cls, path_to_json):
-        """
-        Load a SquareGrid graph from a JSON. Metadata section of the json should contain a flag 'is_SquareGrid" set to
-        True and vertices index should be provided.
-
-        :param path_to_json: string, path to a Json
-        :return: Square Grid graph object.
-        """
-        graph_as_dict = json.load(open(path_to_json, 'r'))
-        if 'is_SquareGrid' not in graph_as_dict['metadata'] or not graph_as_dict['metadata']['is_SquareGrid']:
-            raise TypeError("The file in " + path_to_json + " is not a SquareGrid Json.")
-        if not graph_as_dict['metadata']['vertices_index_provided']:
-            raise TypeError("The file in " + path_to_json + " is supposedly a SquareGrid Json, yet vertices index " +
-                            "are not provided.")
-        shape = (graph_as_dict['metadata']['shape_0'], graph_as_dict['metadata']['shape_1'])
-        graph = cls(shape=shape)
-        graph.dict_cell_id_to_ind = {}
-        for i in range(shape[0]):
-            for j in range(shape[1]):
-                graph.dict_cell_id_to_ind[(i, j)] = graph_as_dict['vertices'][str((i, j))]['index']
-
-        for name in graph_as_dict['metadata']['empty_attributes']:
-            graph.df_attributes[name] = None
-
-        tmp_dict_attribute = {}
-        for name in graph_as_dict['metadata']['non_empty_attributes']:
-            tmp_dict_attribute[name] = [None for _ in range(graph_as_dict['metadata']['nb_vertices'])]
-
-        for i in range(shape[0]):
-            for j in range(shape[1]):
-                index_vertex = graph.dict_cell_id_to_ind[(i, j)]
-                for name in tmp_dict_attribute:
-                    tmp_dict_attribute[name][index_vertex] = graph_as_dict['vertices'][str((i, j))][name]
-                for k in range(graph_as_dict['metadata']['max_degree_vertex']):
-                    if ('n' + str(k)) in graph_as_dict['vertices'][str((i, j))]:
-                        graph.connections[index_vertex][k] = graph_as_dict['vertices'][graph_as_dict['vertices'][str((i, j))][('n' + str(k))]]['index']
-                        graph.weights[index_vertex][k] = graph_as_dict['vertices'][str((i, j))][('w' + str(k))]
-                    else:
-                        graph.connections[index_vertex][k] = -1
-                        graph.weights[index_vertex][k] = -1.
-
-        for name in tmp_dict_attribute:
-            graph.df_attributes[name] = tmp_dict_attribute[name]
-
-        return graph
-
-
-class FromJson:
-    def __init__(self, **kwargs):
-        pass
+from ..pandas_xs.pandas_xs import DataFrameXS
+from .misc import convert_graph_structure_to_dictionary
+
+import numpy as np
+import os
+import shutil
+import json
+import glob
+
+
+class SaveAndLoadSquareGrids:
+    """
+    Add to the square grids graphs the possibility to save them using their own special format.
+
+    We also provide a Json
+    """
+    def __init__(self, **kwargs):
+        pass
+
+    def save(self, path_to_folder, erase_folder=True):
+        """
+        Save the graph structure in a folder using .npy files. The end result is not human readable.
+
+        :param path_to_folder: Path to the folder. If it does not exists, the folder will be created.
+        :param erase_folder: optional, boolean, default True. If True, any folder already existing at 'path_to_folder'
+                             will be deleted.
+        """
+        if os.path.exists(path_to_folder):
+            if not erase_folder:
+                raise OSError("Something already exists at " + path_to_folder + '.')
+            if not os.path.isdir(path_to_folder):
+                raise OSError("The object at " + path_to_folder + " is not a directory. In doubt, we prefer not to " +
+                              "delete it.")
+            shutil.rmtree(path_to_folder)
+        os.mkdir(path_to_folder)
+
+        np.save(path_to_folder + '/connections.npy', self.connections)
+        np.save(path_to_folder + '/weights.npy', self.weights)
+
+        attributes_that_are_none = []
+        for name in self.df_attributes.list_col_name:
+            if self.df_attributes[name] is not None:
+                np.save(path_to_folder + '/attr_' + name + '.npy', self.df_attributes[name])
+            else:
+                attributes_that_are_none.append(name)
+
+        metadata_json = {'shape_0': self.shape[0],
+                         'shape_1': self.shape[1],
+                         'type': self.type,
+                         'attributes_none': attributes_that_are_none}
+        metadata = open(path_to_folder + '/metadata_json.json', 'w')
+        metadata.write(json.dumps(metadata_json))
+        metadata.close()
+
+    @classmethod
+    def load(cls, path_to_folder):
+        """
+
+        :param path_to_folder:
+        :return:
+        """
+        if os.path.exists(path_to_folder):
+            if not os.path.isdir(path_to_folder):
+                raise OSError("The object at " + path_to_folder + " is not a directory.")
+        else:
+            raise OSError("Nothing at " + path_to_folder + '.')
+
+        metadata = json.load(open(path_to_folder + '/metadata_json.json'))
+        shape = (metadata['shape_0'], metadata['shape_1'])
+        graph_type = metadata['type']
+
+        graph = cls(shape=shape)
+        graph.type = graph_type
+        graph.shape = shape
+
+        graph.connections = np.load(path_to_folder + '/connections.npy')
+        graph.weights = np.load(path_to_folder + '/weights.npy')
+
+        for path in glob.glob(path_to_folder + '/*'):
+            if os.path.basename(path).startswith('attr_'):
+                name = os.path.basename(path).split('.')[0]
+                name = name[5:]
+                graph.df_attributes[name] = np.load(path)
+
+        for name in metadata['attributes_none']:
+            graph.df_attributes[name] = None
+
+        return graph
+
+    def save_as_json(self, path_to_json, erase_existing_file=False):
+        """
+        Save a SquareGrid graph as a JSON. This is not the recommended way of saving a
+
+        :param path_to_json:
+        :param erase_existing_file:
+        """
+        if os.path.exists(path_to_json):
+            if not erase_existing_file:
+                raise OSError("Something already exists at " + path_to_json + '.')
+            os.remove(path_to_json)
+
+        dict_graph_structure = convert_graph_structure_to_dictionary(self, save_vertices_index=True,
+                                                                     add_to_metadata={'is_SquareGrid': True,
+                                                                                      'shape_0': self.shape[0],
+                                                                                      'shape_1': self.shape[1]})
+
+        graph_json = open(path_to_json, 'w')
+        graph_json.write(json.dumps(dict_graph_structure))
+        graph_json.close()
+
+    @classmethod
+    def from_json(cls, path_to_json):
+        """
+        Load a SquareGrid graph from a JSON. Metadata section of the json should contain a flag 'is_SquareGrid" set to
+        True and vertices index should be provided.
+
+        :param path_to_json: string, path to a Json
+        :return: Square Grid graph object.
+        """
+        graph_as_dict = json.load(open(path_to_json, 'r'))
+        if 'is_SquareGrid' not in graph_as_dict['metadata'] or not graph_as_dict['metadata']['is_SquareGrid']:
+            raise TypeError("The file in " + path_to_json + " is not a SquareGrid Json.")
+        if not graph_as_dict['metadata']['vertices_index_provided']:
+            raise TypeError("The file in " + path_to_json + " is supposedly a SquareGrid Json, yet vertices index " +
+                            "are not provided.")
+        shape = (graph_as_dict['metadata']['shape_0'], graph_as_dict['metadata']['shape_1'])
+        graph = cls(shape=shape)
+        graph.dict_cell_id_to_ind = {}
+        for i in range(shape[0]):
+            for j in range(shape[1]):
+                graph.dict_cell_id_to_ind[(i, j)] = graph_as_dict['vertices'][str((i, j))]['index']
+
+        for name in graph_as_dict['metadata']['empty_attributes']:
+            graph.df_attributes[name] = None
+
+        tmp_dict_attribute = {}
+        for name in graph_as_dict['metadata']['non_empty_attributes']:
+            tmp_dict_attribute[name] = [None for _ in range(graph_as_dict['metadata']['nb_vertices'])]
+
+        for i in range(shape[0]):
+            for j in range(shape[1]):
+                index_vertex = graph.dict_cell_id_to_ind[(i, j)]
+                for name in tmp_dict_attribute:
+                    tmp_dict_attribute[name][index_vertex] = graph_as_dict['vertices'][str((i, j))][name]
+                for k in range(graph_as_dict['metadata']['max_degree_vertex']):
+                    if ('n' + str(k)) in graph_as_dict['vertices'][str((i, j))]:
+                        graph.connections[index_vertex][k] = graph_as_dict['vertices'][graph_as_dict['vertices'][str((i, j))][('n' + str(k))]]['index']
+                        graph.weights[index_vertex][k] = graph_as_dict['vertices'][str((i, j))][('w' + str(k))]
+                    else:
+                        graph.connections[index_vertex][k] = -1
+                        graph.weights[index_vertex][k] = -1.
+
+        for name in tmp_dict_attribute:
+            graph.df_attributes[name] = tmp_dict_attribute[name]
+
+        return graph
+
+
+class FromJson:
+    def __init__(self, **kwargs):
+        pass
```

### Comparing `sampy-abm-1.0.2/src/sampy/graph/jit_compiled_functions.py` & `sampy_abm-1.0.3/src/sampy/graph/jit_compiled_functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,169 +1,181 @@
-import numpy as np
-import math
-import numba as nb
-
-
-@nb.njit
-def topology_convert_1d_array_to_2d_array(arr_1d, arr_fast_squarify, shape_0, shape_1):
-    rv = np.full((shape_0, shape_1), arr_1d[0])
-    for i in range(arr_1d.shape[0]):
-        rv[arr_fast_squarify[i][0]][arr_fast_squarify[i][1]] = arr_1d[i]
-    return rv
-
-
-@nb.njit
-def topology_convert_2d_array_to_1d_array(arr_2d, arr_fast_flat):
-    n = arr_2d.shape[0] * arr_2d.shape[1]
-    rv = np.full((n, ), arr_2d[0][0])
-    for i in range(arr_2d.shape[0]):
-        for j in range(arr_2d.shape[1]):
-            rv[arr_fast_flat[i][j]] = arr_2d[i][j]
-    return rv
-
-
-@nb.njit
-def compute_sin_attr_with_condition(arr_attr, arr_cond, time, amplitude, period, phase, intercept):
-    for i in range(arr_cond.shape[0]):
-        if arr_cond[i]:
-            arr_attr[i] = amplitude*np.sin(2*math.pi*time/period + phase) + intercept
-
-
-@nb.njit
-def get_oriented_neighborhood_of_vertices(connections):
-    rv = np.full(connections.shape, -1, dtype=np.int32)
-    for ind_center in range(connections.shape[0]):
-        # we first create the set of neighbours
-        set_neighbours = set()
-        nb_neighbours = 0
-        for i in range(connections.shape[1]):
-            ind_neighb = connections[ind_center][i]
-            if ind_neighb == -1:
-                pass
-            else:
-                set_neighbours.add(ind_neighb)
-                nb_neighbours += 1
-        # we now fill the returned array
-        for j in range(nb_neighbours):
-            ind_neighbour = connections[ind_center][j]
-            if ind_neighbour == -1:
-                pass
-            else:
-                rv[ind_center][0] = ind_neighbour
-                break
-        for j in range(1, nb_neighbours):
-            ind_current_neigh = rv[ind_center][j-1]
-            for k in range(connections.shape[1]):
-                ind_neighbour = connections[ind_current_neigh][k]
-                if ind_neighbour == -1:
-                    pass
-                elif ind_neighbour in set_neighbours:
-                    if j != 1 and rv[ind_center][j-2] == ind_neighbour:
-                        pass
-                    else:
-                        rv[ind_center][j] = ind_neighbour
-                        break
-    return rv
-
-
-@nb.njit
-def get_surface_array(oriented_neighbourhood_array, x_coord, y_coord, z_coord, radius):
-    rv = np.full((oriented_neighbourhood_array.shape[0],), 0., dtype=np.float64)
-    for index_center in range(oriented_neighbourhood_array.shape[0]):
-        # get coordinates of the center
-        x_center = x_coord[index_center]
-        y_center = y_coord[index_center]
-        z_center = z_coord[index_center]
-
-        # quick loop to determine the number of vertices of the current polygon
-        nb_vertices = 0
-        for i in range(oriented_neighbourhood_array.shape[1]):
-            if oriented_neighbourhood_array[index_center][i] != -1:
-                nb_vertices += 1
-
-        # we first create the normal vectors of each hyperplane defining the spherical polygon. Those vectors are not
-        # normalized
-        oriented_normal_vect = np.full((nb_vertices, 3), -1.)
-        current_index = 0
-        for i in range(oriented_neighbourhood_array.shape[1]):
-            index_current_neighbour = oriented_neighbourhood_array[index_center][i]
-            if index_current_neighbour != -1:
-                oriented_normal_vect[current_index][0] = x_coord[index_current_neighbour] - x_center
-                oriented_normal_vect[current_index][1] = y_coord[index_current_neighbour] - y_center
-                oriented_normal_vect[current_index][2] = z_coord[index_current_neighbour] - z_center
-            current_index += 1
-
-        # we know compute the coordinates of the vertices of the spherical polygon using a cross product.
-        oriented_vertices_polygon = np.full((nb_vertices, 3), -1.)
-        for i in range(nb_vertices):
-            vertex = np.cross(oriented_normal_vect[i][:], oriented_normal_vect[(i+1) % nb_vertices][:])
-            if x_center * vertex[0] + y_center * vertex[1] + z_center * vertex[2] > 0:
-                oriented_vertices_polygon[i][:] = vertex / (np.sqrt((vertex ** 2).sum()))
-            else:
-                oriented_vertices_polygon[i][:] = - vertex / (np.sqrt((vertex ** 2).sum()))
-
-        area = 0.
-        first_point = oriented_vertices_polygon[0][:]
-        second_point = oriented_vertices_polygon[1][:]
-        for i in range(2, nb_vertices):
-            third_point = oriented_vertices_polygon[i][:]
-
-            vec1 = second_point - np.dot(second_point, first_point) * first_point
-            vec2 = third_point - np.dot(third_point, first_point) * first_point
-            area += np.arccos(np.dot(vec1, vec2) / (np.linalg.norm(vec1) * np.linalg.norm(vec2)))
-
-            vec1 = first_point - np.dot(first_point, second_point) * second_point
-            vec2 = third_point - np.dot(third_point, second_point) * second_point
-            area += np.arccos(np.dot(vec1, vec2) / (np.linalg.norm(vec1) * np.linalg.norm(vec2)))
-
-            vec1 = first_point - np.dot(first_point, third_point) * third_point
-            vec2 = second_point - np.dot(second_point, third_point) * third_point
-            area += np.arccos(np.dot(vec1, vec2) / (np.linalg.norm(vec1) * np.linalg.norm(vec2)))
-
-            area -= np.pi
-            second_point = oriented_vertices_polygon[i][:]
-        rv[index_center] = (radius**2)*area
-    return rv
-
-
-@nb.njit
-def icosphere_get_distance_matrix(dist_matrix, connections, lats, lons, radius):
-    for i in range(dist_matrix.shape[0]):
-        for j in range(dist_matrix.shape[1]):
-            if connections[i][j] != -1:
-                dist_matrix[i][j] = radius * np.arccos(np.sin(lats[i]) * np.sin(lats[connections[i][j]]) +
-                                                       np.cos(lats[i]) * np.cos(lats[connections[i][j]]) *
-                                                       np.cos(lons[i] - lons[connections[i][j]]))
-    return dist_matrix
-
-
-@nb.njit
-def keep_subgraph_from_array_of_bool_equi_weight(arr_keep, connections):
-    counter = 0
-    dict_old_to_new = dict()
-    for i in range(arr_keep.shape[0]):
-        if arr_keep[i]:
-            dict_old_to_new[i] = counter
-            counter += 1
-
-    arr_nb_connections = np.full((counter,), 0, dtype=np.int32)
-    new_arr_connections = np.full((counter, 6), -1, dtype=np.int32)
-    new_arr_weights = np.full((counter, 6), -1., dtype=np.float32)
-
-    counter = 0
-    for i in range(arr_keep.shape[0]):
-        if arr_keep[i]:
-            for j in range(connections.shape[1]):
-                if connections[i][j] in dict_old_to_new:
-                    new_arr_connections[counter][arr_nb_connections[counter]] = dict_old_to_new[connections[i][j]]
-                    arr_nb_connections[counter] += 1
-            counter += 1
-
-    for i in range(arr_nb_connections.shape[0]):
-        for j in range(arr_nb_connections[i]):
-            if j + 1 == arr_nb_connections[i]:
-                new_arr_weights[i][j] = 1.
-            else:
-                new_arr_weights[i][j] = (j + 1) / arr_nb_connections[i]
-
-    return new_arr_connections, new_arr_weights
-
+import numpy as np
+import math
+import numba as nb
+
+
+@nb.njit
+def topology_convert_1d_array_to_2d_array(arr_1d, arr_fast_squarify, shape_0, shape_1):
+    rv = np.full((shape_0, shape_1), arr_1d[0])
+    for i in range(arr_1d.shape[0]):
+        rv[arr_fast_squarify[i][0]][arr_fast_squarify[i][1]] = arr_1d[i]
+    return rv
+
+
+@nb.njit
+def topology_convert_2d_array_to_1d_array(arr_2d, arr_fast_flat):
+    n = arr_2d.shape[0] * arr_2d.shape[1]
+    rv = np.full((n, ), arr_2d[0][0])
+    for i in range(arr_2d.shape[0]):
+        for j in range(arr_2d.shape[1]):
+            rv[arr_fast_flat[i][j]] = arr_2d[i][j]
+    return rv
+
+
+@nb.njit
+def compute_sin_attr_with_condition(arr_attr, arr_cond, time, amplitude, period, phase, intercept):
+    for i in range(arr_cond.shape[0]):
+        if arr_cond[i]:
+            arr_attr[i] = amplitude*np.sin(2*math.pi*time/period + phase) + intercept
+
+
+@nb.njit
+def get_oriented_neighborhood_of_vertices(connections):
+    rv = np.full(connections.shape, -1, dtype=np.int32)
+    for ind_center in range(connections.shape[0]):
+        # we first create the set of neighbours
+        set_neighbours = set()
+        nb_neighbours = 0
+        for i in range(connections.shape[1]):
+            ind_neighb = connections[ind_center][i]
+            if ind_neighb == -1:
+                pass
+            else:
+                set_neighbours.add(ind_neighb)
+                nb_neighbours += 1
+        # we now fill the returned array
+        for j in range(nb_neighbours):
+            ind_neighbour = connections[ind_center][j]
+            if ind_neighbour == -1:
+                pass
+            else:
+                rv[ind_center][0] = ind_neighbour
+                break
+        for j in range(1, nb_neighbours):
+            ind_current_neigh = rv[ind_center][j-1]
+            for k in range(connections.shape[1]):
+                ind_neighbour = connections[ind_current_neigh][k]
+                if ind_neighbour == -1:
+                    pass
+                elif ind_neighbour in set_neighbours:
+                    if j != 1 and rv[ind_center][j-2] == ind_neighbour:
+                        pass
+                    else:
+                        rv[ind_center][j] = ind_neighbour
+                        break
+    return rv
+
+
+@nb.njit
+def get_surface_array(oriented_neighbourhood_array, x_coord, y_coord, z_coord, radius):
+    rv = np.full((oriented_neighbourhood_array.shape[0],), 0., dtype=np.float64)
+    for index_center in range(oriented_neighbourhood_array.shape[0]):
+        # get coordinates of the center
+        x_center = x_coord[index_center]
+        y_center = y_coord[index_center]
+        z_center = z_coord[index_center]
+
+        # quick loop to determine the number of vertices of the current polygon
+        nb_vertices = 0
+        for i in range(oriented_neighbourhood_array.shape[1]):
+            if oriented_neighbourhood_array[index_center][i] != -1:
+                nb_vertices += 1
+
+        # we first create the normal vectors of each hyperplane defining the spherical polygon. Those vectors are not
+        # normalized
+        oriented_normal_vect = np.full((nb_vertices, 3), -1.)
+        current_index = 0
+        for i in range(oriented_neighbourhood_array.shape[1]):
+            index_current_neighbour = oriented_neighbourhood_array[index_center][i]
+            if index_current_neighbour != -1:
+                oriented_normal_vect[current_index][0] = x_coord[index_current_neighbour] - x_center
+                oriented_normal_vect[current_index][1] = y_coord[index_current_neighbour] - y_center
+                oriented_normal_vect[current_index][2] = z_coord[index_current_neighbour] - z_center
+            current_index += 1
+
+        # we know compute the coordinates of the vertices of the spherical polygon using a cross product.
+        oriented_vertices_polygon = np.full((nb_vertices, 3), -1.)
+        for i in range(nb_vertices):
+            vertex = np.cross(oriented_normal_vect[i][:], oriented_normal_vect[(i+1) % nb_vertices][:])
+            if x_center * vertex[0] + y_center * vertex[1] + z_center * vertex[2] > 0:
+                oriented_vertices_polygon[i][:] = vertex / (np.sqrt((vertex ** 2).sum()))
+            else:
+                oriented_vertices_polygon[i][:] = - vertex / (np.sqrt((vertex ** 2).sum()))
+
+        area = 0.
+        first_point = oriented_vertices_polygon[0][:]
+        second_point = oriented_vertices_polygon[1][:]
+        for i in range(2, nb_vertices):
+            third_point = oriented_vertices_polygon[i][:]
+
+            vec1 = second_point - np.dot(second_point, first_point) * first_point
+            vec2 = third_point - np.dot(third_point, first_point) * first_point
+            area += np.arccos(np.dot(vec1, vec2) / (np.linalg.norm(vec1) * np.linalg.norm(vec2)))
+
+            vec1 = first_point - np.dot(first_point, second_point) * second_point
+            vec2 = third_point - np.dot(third_point, second_point) * second_point
+            area += np.arccos(np.dot(vec1, vec2) / (np.linalg.norm(vec1) * np.linalg.norm(vec2)))
+
+            vec1 = first_point - np.dot(first_point, third_point) * third_point
+            vec2 = second_point - np.dot(second_point, third_point) * third_point
+            area += np.arccos(np.dot(vec1, vec2) / (np.linalg.norm(vec1) * np.linalg.norm(vec2)))
+
+            area -= np.pi
+            second_point = oriented_vertices_polygon[i][:]
+        rv[index_center] = (radius**2)*area
+    return rv
+
+
+@nb.njit
+def icosphere_get_distance_matrix(dist_matrix, connections, lats, lons, radius):
+    for i in range(dist_matrix.shape[0]):
+        for j in range(dist_matrix.shape[1]):
+            if connections[i][j] != -1:
+                dist_matrix[i][j] = radius * np.arccos(np.sin(lats[i]) * np.sin(lats[connections[i][j]]) +
+                                                       np.cos(lats[i]) * np.cos(lats[connections[i][j]]) *
+                                                       np.cos(lons[i] - lons[connections[i][j]]))
+    return dist_matrix
+
+
+@nb.njit
+def keep_subgraph_from_array_of_bool_equi_weight(arr_keep, connections):
+    counter = 0
+    dict_old_to_new = dict()
+    for i in range(arr_keep.shape[0]):
+        if arr_keep[i]:
+            dict_old_to_new[i] = counter
+            counter += 1
+
+    arr_nb_connections = np.full((counter,), 0, dtype=np.int32)
+    new_arr_connections = np.full((counter, 6), -1, dtype=np.int32)
+    new_arr_weights = np.full((counter, 6), -1., dtype=np.float32)
+
+    counter = 0
+    for i in range(arr_keep.shape[0]):
+        if arr_keep[i]:
+            for j in range(connections.shape[1]):
+                if connections[i][j] in dict_old_to_new:
+                    new_arr_connections[counter][arr_nb_connections[counter]] = dict_old_to_new[connections[i][j]]
+                    arr_nb_connections[counter] += 1
+            counter += 1
+
+    for i in range(arr_nb_connections.shape[0]):
+        for j in range(arr_nb_connections[i]):
+            if j + 1 == arr_nb_connections[i]:
+                new_arr_weights[i][j] = 1.
+            else:
+                new_arr_weights[i][j] = (j + 1) / arr_nb_connections[i]
+
+    return new_arr_connections, new_arr_weights
+
+
+@nb.njit
+def compute_area_oriented_array_of_conv_polygons_same_nb_vert(array_vertices):
+    array_area = np.zeros((array_vertices.shape[0],), dtype=float)
+    for i in range(array_vertices.shape[0]):
+        for j in range(array_vertices.shape[1]): # that's where the assumption that the number
+                                                 # of vertices is the same accross all polyg
+            next_j = (j + 1) % array_vertices.shape[1]
+            array_area[i] += array_vertices[i, j, 0] * array_vertices[i, next_j, 1] - \
+                array_vertices[i, j, 1] * array_vertices[i, next_j, 0]
+        array_area[i] /= 2.
+    return array_area
```

### Comparing `sampy-abm-1.0.2/src/sampy/graph/spatial_functions.py` & `sampy_abm-1.0.3/src/sampy/graph/spatial_functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,53 @@
-import numpy as np
-
-
-def create_2d_coords_from_oriented_connection_matrix(connections, index_first_vertex, coord_first_vertex,
-                                                     list_vectors):
-    """
-    WARNING: The graph is assumed to be connected.
-
-    Create the coordinates (2D) of each vertex of the graph. The algorithm starts at the cell given by the
-        kwarg 'index_first_cell', which receives as coordinates the one given in 'coord_first_cell'. Then we loop
-        through each neighbours of the starting cell, giving coordinates to each one using the parameter 'list_vector'
-        (see description of 'list_vector' parameter below for a more detailed explanation). We then repeat the process
-        with a vertex that has coordinates, and so on until each vertex has coordinates. This algorithm works only if
-        the graph is connected.
-
-    :param connections: 2D array of integers. Connection matrix used in SamPy Graph objects to encode the edges between
-                        vertices. Here it is assumed to be oriented (that is each column correspond to a specific
-                        direction).
-    :param index_first_vertex: non-negative integer
-    :param coord_first_vertex: couple of floats
-    :param list_vectors: list containing connections.shape[1] arrays, each of shape (2,).
-
-    :return: a pair (coords_x, coords_y) of 1D arrays of floats giving the coordinates of each vertex.
-    """
-    # we now create the arrays that will contain the x and y coordinates
-    coord_x = np.full(connections.shape[0], 0., dtype=float)
-    coord_y = np.full(connections.shape[0], 0., dtype=float)
-
-    # we initialize the coordinates and create two data-structure that will allow us to recursively give coordinates
-    # to each vertex.
-    coord_x[index_first_vertex] = float(coord_first_vertex[0])
-    coord_y[index_first_vertex] = float(coord_first_vertex[1])
-    set_index_vert_with_coords = set([index_first_vertex])
-    list_index_vert_with_coords = [index_first_vertex]
-
-    # now we recursively give coordinates to every vertex
-    for i in range(connections.shape[0]):
-        try:
-            current_vertex = list_index_vert_with_coords[i]
-        except IndexError:
-            raise ValueError("Error encountered while creating vertices' coordinates. The most likely explanation"
-                             " is that the graph is not connected.")
-        for j in range(connections.shape[1]):
-            if connections[current_vertex, j] not in set_index_vert_with_coords:
-                coord_x[connections[i, j]] = coord_x[current_vertex] + list_vectors[j][0]
-                coord_y[connections[i, j]] = coord_y[current_vertex] + list_vectors[j][1]
-                list_index_vert_with_coords.append(connections[i, j])
-                set_index_vert_with_coords.add(connections[i, j])
-
-    return coord_x, coord_y
+import numpy as np
+
+
+def create_2d_coords_from_oriented_connection_matrix(connections, index_first_vertex, coord_first_vertex,
+                                                     list_vectors):
+    """
+    WARNING: The graph is assumed to be connected.
+
+    Create the coordinates (2D) of each vertex of the graph. The algorithm starts at the cell given by the
+        kwarg 'index_first_cell', which receives as coordinates the one given in 'coord_first_cell'. Then we loop
+        through each neighbours of the starting cell, giving coordinates to each one using the parameter 'list_vector'
+        (see description of 'list_vector' parameter below for a more detailed explanation). We then repeat the process
+        with a vertex that has coordinates, and so on until each vertex has coordinates. This algorithm works only if
+        the graph is connected.
+
+    :param connections: 2D array of integers. Connection matrix used in SamPy Graph objects to encode the edges between
+                        vertices. Here it is assumed to be oriented (that is each column correspond to a specific
+                        direction).
+    :param index_first_vertex: non-negative integer
+    :param coord_first_vertex: couple of floats
+    :param list_vectors: list containing connections.shape[1] arrays, each of shape (2,).
+
+    :return: a pair (coords_x, coords_y) of 1D arrays of floats giving the coordinates of each vertex.
+    """
+    # we now create the arrays that will contain the x and y coordinates
+    coord_x = np.full(connections.shape[0], 0., dtype=float)
+    coord_y = np.full(connections.shape[0], 0., dtype=float)
+
+    # we initialize the coordinates and create two data-structure that will allow us to recursively give coordinates
+    # to each vertex.
+    coord_x[index_first_vertex] = float(coord_first_vertex[0])
+    coord_y[index_first_vertex] = float(coord_first_vertex[1])
+    set_index_vert_with_coords = set([index_first_vertex])
+    list_index_vert_with_coords = [index_first_vertex]
+
+    # now we recursively give coordinates to every vertex
+    for i in range(connections.shape[0]):
+        try:
+            current_vertex = list_index_vert_with_coords[i]
+        except IndexError:
+            raise ValueError("Error encountered while creating vertices' coordinates. The most likely explanation"
+                             " is that the graph is not connected.")
+        for j in range(connections.shape[1]):
+            if (connections[current_vertex, j] not in set_index_vert_with_coords) and (connections[current_vertex, j] != -1):
+                coord_x[connections[current_vertex, j]] = coord_x[current_vertex] + list_vectors[j][0]
+                coord_y[connections[current_vertex, j]] = coord_y[current_vertex] + list_vectors[j][1]
+                list_index_vert_with_coords.append(connections[current_vertex, j])
+                set_index_vert_with_coords.add(connections[current_vertex, j])
+
+    return coord_x, coord_y
+
+
+
```

### Comparing `sampy-abm-1.0.2/src/sampy/graph/topology.py` & `sampy_abm-1.0.3/src/sampy/graph/topology.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,273 +1,296 @@
-from .misc import (create_grid_hexagonal_cells,
-                   create_grid_square_cells,
-                   create_grid_square_with_diagonals,
-                   SubdividedIcosahedron)
-from .jit_compiled_functions import (get_oriented_neighborhood_of_vertices,
-                                     get_surface_array,
-                                     topology_convert_1d_array_to_2d_array,
-                                     topology_convert_2d_array_to_1d_array,
-                                     icosphere_get_distance_matrix)
-
-
-import numpy as np
-from math import sqrt, pi
-import pandas as pd
-
-import os
-
-
-class BaseTopology:
-    def __init__(self, **kwargs):
-        self.connections = None
-        self.weights = None
-        self.type = None
-        self.dict_cell_id_to_ind = {}
-        self.time = 0
-
-        self.on_ticker = ['increment_time']
-
-    def increment_time(self):
-        self.time += 1
-
-    def tick(self):
-        """
-        execute the methods whose names are stored in the attribute on_ticker, in order.
-        """
-        for method in self.on_ticker:
-            getattr(self, method)()
-
-    def save_table_id_of_vertices_to_indices(self, path_to_csv, sep, erase_existing_file=True):
-        """
-        Create and save a two column csv allowing to match vertices id's with vertices indexes.
-
-        :param path_to_csv: string, path to the output csv
-        :param sep: string, separator to use in the csv.
-        :param erase_existing_file: optional, boolean, default True. If True, the method will check if there is already
-                                    a file at path_to_csv and delete it if it exists.
-        """
-        if erase_existing_file:
-            if os.path.exists(path_to_csv):
-                os.remove(path_to_csv)
-        with open(path_to_csv, 'a') as f_out:
-            f_out.write("id_vertex" + sep + "index_vertex" + "\n")
-            for id_vertex, index in self.dict_cell_id_to_ind.items():
-                f_out.write(str(id_vertex) + sep + str(index) + '\n')
-        return
-
-    @property
-    def number_vertices(self):
-        return self.connections.shape[0]
-
-
-class SquareGridWithDiagTopology(BaseTopology):
-    def __init__(self, shape=None, **kwargs):
-        if shape is None:
-            raise ValueError("Kwarg 'shape' is missing while initializing the graph topology. 'shape' should be a "
-                             "tuple like object of the form (a, b), where a and b are integers bigger than 1.")
-        len_side_a = shape[0]
-        len_side_b = shape[1]
-        self.create_square_with_diag_grid(len_side_a, len_side_b)
-        self.shape = (len_side_a, len_side_b)
-        self.type = 'SquareGridWithDiag'
-
-    def create_square_with_diag_grid(self, len_side_a, len_side_b):
-        """
-        Create a square grid with diagonals, where each vertex X[i][j] is linked to X[i-1][j-1], X[i][j-1], X[i+1][j-1],
-        X[i+1][j], X[i+1][j+1], x[i][j+1], x[i-1][j+1] and x[i-1][j] if they exist. Note that the weights on the
-        'diagonal connections' is reduced to take into account the fact that the vertices on the diagonal are 'further
-        away' (i.e. using sqrt(2) as a distance instead of 1 in the weight computation).
-
-        :param len_side_a: integer, x coordinate
-        :param len_side_b: integer, y coordinate
-        """
-        if (len_side_a < 2) or (len_side_b < 2):
-            raise ValueError('side length attributes for HexagonalCells should be at least 2.')
-
-        self.connections, self.weights = create_grid_square_with_diagonals(len_side_a, len_side_b)
-
-        # populate the dictionary from cell coordinates to cell indexes in arrays connection and weights
-        for i in range(len_side_a):
-            for j in range(len_side_b):
-                self.dict_cell_id_to_ind[(i, j)] = j + i*len_side_b
-
-
-class SquareGridTopology(BaseTopology):
-    def __init__(self, shape=None, **kwargs):
-        if shape is None:
-            raise ValueError("Kwarg 'shape' is missing while initializing the graph topology. 'shape' should be a "
-                             "tuple like object of the form (a, b), where a and b are integers bigger than 1.")
-        len_side_a = shape[0]
-        len_side_b = shape[1]
-        self.create_square_grid(len_side_a, len_side_b)
-        self.shape = (len_side_a, len_side_b)
-        self.type = 'SquareGrid'
-
-    def create_square_grid(self, len_side_a, len_side_b):
-        """
-        Create a square grid, where each vertex X[i][j] is linked to X[i-1][j], X[i][j-1], X[i+1][j], X[i][j+1] if they
-        exist.
-
-        :param len_side_a: integer, x coordinate
-        :param len_side_b: integer, y coordinate
-        """
-        if (len_side_a < 2) or (len_side_b < 2):
-            raise ValueError('side length attributes for HexagonalCells should be at least 2.')
-
-        self.connections, self.weights = create_grid_square_cells(len_side_a, len_side_b)
-        self.shape = (len_side_a, len_side_b)
-
-        # populate the dictionary from cell coordinates to cell indexes in arrays connection and weights
-        for i in range(len_side_a):
-            for j in range(len_side_b):
-                self.dict_cell_id_to_ind[(i, j)] = j + i*len_side_b
-
-
-class SquareGridsConvertBetween1DArrayAnd2DArrays:
-    def __init__(self, **kwargs):
-        self._array_optimized_squarification = None
-        self._array_optimized_flat = None
-
-    def _sampy_debug_convert_1d_array_to_2d_array(self, input_arr):
-        if not type(input_arr) is np.ndarray:
-            raise ValueError("Input variable is not a numpy array.")
-        if input_arr.shape != (self.number_vertices,):
-            raise ValueError("Input array of invalid shape.")
-
-    def convert_1d_array_to_2d_array(self, input_arr):
-        """
-        Takes a 1D array of shape (nb_vertices,) and convert it into a 2D array of shape self.shape.
-
-        :param input_arr: 1D array.
-        :return: 2D array
-        """
-        if self._array_optimized_squarification is None:
-            self._array_optimized_squarification = np.full((self.number_vertices, 2), 0)
-            for key, val in self.dict_cell_id_to_ind.items():
-                self._array_optimized_squarification[val][0] = key[0]
-                self._array_optimized_squarification[val][1] = key[1]
-        return topology_convert_1d_array_to_2d_array(input_arr, self._array_optimized_squarification,
-                                                     self.shape[0], self.shape[1])
-
-    def _sampy_debug_convert_2d_array_to_1d_array(self, input_arr):
-        if not type(input_arr) is np.ndarray:
-            raise ValueError("Input variable is not a numpy array.")
-        if input_arr.shape != self.shape:
-            raise ValueError("Input array of invalid shape.")
-
-    def convert_2d_array_to_1d_array(self, input_array):
-        """
-
-        :param input_array:
-        :return:
-        """
-        if self._array_optimized_flat is None:
-            self._array_optimized_flat = np.full(self.shape, 0)
-            for key, val in self.dict_cell_id_to_ind.items():
-                self._array_optimized_flat[key[0], key[1]] = val
-        return topology_convert_2d_array_to_1d_array(input_array, self._array_optimized_flat)
-
-
-class IcosphereTopology(BaseTopology):
-    def __init__(self, nb_sub=None, radius=1., **kwargs):
-        if nb_sub is None:
-            raise ValueError("kwarg nb_sub missing")
-        self.nb_sub = nb_sub
-        self.radius = float(radius)
-
-        icosahedron = SubdividedIcosahedron(nb_sub)
-        self.connections = np.copy(icosahedron.connections)
-        self.weights = np.copy(icosahedron.weights)
-        self.arr_coord = np.copy(icosahedron.arr_coord)
-        del icosahedron
-
-        self.type = 'IcoSphere'
-        self.three_d_coord_created = False
-
-    def create_3d_coord(self):
-        self.df_attributes['coord_x'] = self.arr_coord[:, 0].astype(np.float64)
-        self.df_attributes['coord_y'] = self.arr_coord[:, 1].astype(np.float64)
-        self.df_attributes['coord_z'] = self.arr_coord[:, 2].astype(np.float64)
-
-        norm = np.sqrt(self.df_attributes['coord_x']**2 +
-                       self.df_attributes['coord_y']**2 +
-                       self.df_attributes['coord_z']**2)
-
-        self.df_attributes['coord_x_normalized'] = self.df_attributes['coord_x'] / norm
-        self.df_attributes['coord_x'] = self.radius * self.df_attributes['coord_x_normalized']
-
-        self.df_attributes['coord_y_normalized'] = self.df_attributes['coord_y'] / norm
-        self.df_attributes['coord_y'] = self.radius * self.df_attributes['coord_y_normalized']
-
-        self.df_attributes['coord_z_normalized'] = self.df_attributes['coord_z'] / norm
-        self.df_attributes['coord_z'] = self.radius * self.df_attributes['coord_z_normalized']
-
-        self.three_d_coord_created = True
-
-    def create_pseudo_epsg4326_coordinates(self):
-        """
-        This method approximate the shape of the earth using a sphere, which creates deformations.
-        """
-        if not self.three_d_coord_created:
-            self.create_3d_coord()
-
-        self.df_attributes['lat'] = (180*(pi/2 - np.arccos(self.df_attributes['coord_z_normalized']))/pi).astype(np.float64)
-        self.df_attributes['lon'] = (180*np.arctan2(self.df_attributes['coord_y_normalized'],
-                                                   self.df_attributes['coord_x_normalized'])/pi).astype(np.float64)
-
-    def compute_distance_matrix_on_sphere(self):
-        """
-        This method compute a distance matrix that gives the distance between each pair of connected vertex of the
-        graph. The distance is the geodesic distance on a sphere (i.e. the distance
-
-        :return: Array of floats with the same shape as the array 'connections'
-        """
-        dist_matrix = np.full(self.connections.shape, -1., dtype=np.float64)
-        lats_rad = (np.pi * self.df_attributes['lat'] / 180).astype(np.float64)
-        lons_rad = (np.pi * self.df_attributes['lon'] / 180).astype(np.float64)
-
-        dist_matrix = icosphere_get_distance_matrix(dist_matrix, self.connections, lats_rad, lons_rad, self.radius)
-
-        return dist_matrix
-
-    def create_and_save_radius_cells_as_attribute(self, radius_attribute='radius_each_cell'):
-        """
-        Save radius of each cell. The radius of a cell centered on a vertex v is defined as the maximum distance between
-        v and its neighbours. The radius is saved within df_attributes.
-
-        :param radius_attribute: optional, string, default 'radius_each_cell'. Name of the attribute corresponding to
-                                 the radius of each cell.
-        """
-        dist_matrix = self.compute_distance_matrix_on_sphere()
-        max_distance = np.amax(dist_matrix, axis=1).astype(np.float64)
-        self.df_attributes[radius_attribute] = max_distance
-
-    def compute_surface_array(self):
-        """
-        Return an array giving the surface of each cell of the icosphere
-        :return: array of floats shape (nb_vertex,)
-        """
-        # note that this orientation is not necessarily clockwise, and can be anti-clockwise for some vertices.
-        # But this is not important for our purpose of computing the area of each cell of the icosphere.
-        oriented_neigh_vert = get_oriented_neighborhood_of_vertices(self.connections)
-
-        return get_surface_array(oriented_neigh_vert,
-                                 self.df_attributes['coord_x_normalized'],
-                                 self.df_attributes['coord_y_normalized'],
-                                 self.df_attributes['coord_z_normalized'],
-                                 self.radius).astype(np.float64)
-
-    def create_and_save_surface_array_as_attribute(self):
-        arr_surface = self.compute_surface_array()
-        self.df_attributes['surface_cell'] = arr_surface
-
-
-class OrientedHexagonalGrid(BaseTopology):
-    """
-    Create an hexagonal lattice on a square. Each
-    """
-    def __init__(self, nb_hex_x_axis=None, nb_hex_y_axis=None, **kwargs):
-        """
-        :param nb_hex_x_axis: mandatory kwargs. Integer, number of hexagons on the horizontal axis.
-        :param nb_hex_y_axis: mandatory kwargs. Integer, number of hexagons on the vertical axis.
-        """
-        pass
+from .misc import (create_grid_hexagonal_cells,
+                   create_grid_square_cells,
+                   create_grid_square_with_diagonals,
+                   SubdividedIcosahedron)
+from .jit_compiled_functions import (get_oriented_neighborhood_of_vertices,
+                                     get_surface_array,
+                                     topology_convert_1d_array_to_2d_array,
+                                     topology_convert_2d_array_to_1d_array,
+                                     icosphere_get_distance_matrix)
+
+
+import numpy as np
+from math import sqrt, pi
+import pandas as pd
+
+import os
+
+
+class BaseTopology:
+    def __init__(self, **kwargs):
+        self.connections = None
+        self.weights = None
+        self.type = None
+        self.dict_cell_id_to_ind = {}
+        self.time = 0
+
+        self.on_ticker = ['increment_time']
+
+    def increment_time(self):
+        self.time += 1
+
+    def tick(self):
+        """
+        execute the methods whose names are stored in the attribute on_ticker, in order.
+        """
+        for method in self.on_ticker:
+            getattr(self, method)()
+
+    def save_table_id_of_vertices_to_indices(self, path_to_csv, sep, erase_existing_file=True):
+        """
+        Create and save a two column csv allowing to match vertices id's with vertices indexes.
+
+        :param path_to_csv: string, path to the output csv
+        :param sep: string, separator to use in the csv.
+        :param erase_existing_file: optional, boolean, default True. If True, the method will check if there is already
+                                    a file at path_to_csv and delete it if it exists.
+        """
+        if erase_existing_file:
+            if os.path.exists(path_to_csv):
+                os.remove(path_to_csv)
+        with open(path_to_csv, 'a') as f_out:
+            f_out.write("id_vertex" + sep + "index_vertex" + "\n")
+            for id_vertex, index in self.dict_cell_id_to_ind.items():
+                f_out.write(str(id_vertex) + sep + str(index) + '\n')
+        return
+
+    @property
+    def number_vertices(self):
+        return self.connections.shape[0]
+
+
+class SquareGridWithDiagTopology(BaseTopology):
+    def __init__(self, shape=None, equi_prob=False, **kwargs):
+        if shape is None:
+            raise ValueError("Kwarg 'shape' is missing while initializing the graph topology. 'shape' should be a "
+                             "tuple like object of the form (a, b), where a and b are integers bigger than 1.")
+        len_side_a = shape[0]
+        len_side_b = shape[1]
+        self.create_square_with_diag_grid(len_side_a, len_side_b, equi_prob=equi_prob)
+        self.shape = (len_side_a, len_side_b)
+        self.type = 'SquareGridWithDiag'
+
+    def create_square_with_diag_grid(self, len_side_a, len_side_b, equi_prob=False):
+        """
+        Create a square grid with diagonals, where each vertex X[i][j] is linked to X[i-1][j-1], X[i][j-1], X[i+1][j-1],
+        X[i+1][j], X[i+1][j+1], x[i][j+1], x[i-1][j+1] and x[i-1][j] if they exist. Note that the weights on the
+        'diagonal connections' is reduced to take into account the fact that the vertices on the diagonal are 'further
+        away' (i.e. using sqrt(2) as a distance instead of 1 in the weight computation). If one wants all the weights
+        to be equal (so that an agent moving from a cell has the same probability to perform a diagonal step as to 
+        perform an horizontal/vertical step), set the kwarg equi_prob to True.
+
+        :param len_side_a: integer, x coordinate
+        :param len_side_b: integer, y coordinate
+        :param equi_prob: bool, optional, default False. If True, all the neighbouring cells have the same weight.
+        """
+        if (len_side_a < 2) or (len_side_b < 2):
+            raise ValueError('side length attributes for HexagonalCells should be at least 2.')
+
+        self.connections, self.weights = create_grid_square_with_diagonals(len_side_a, len_side_b, equi_prob)
+
+        # populate the dictionary from cell coordinates to cell indexes in arrays connection and weights
+        for i in range(len_side_a):
+            for j in range(len_side_b):
+                self.dict_cell_id_to_ind[(i, j)] = j + i*len_side_b
+
+
+class SquareGridTopology(BaseTopology):
+    def __init__(self, shape=None, **kwargs):
+        if shape is None:
+            raise ValueError("Kwarg 'shape' is missing while initializing the graph topology. 'shape' should be a "
+                             "tuple like object of the form (a, b), where a and b are integers bigger than 1.")
+        len_side_a = shape[0]
+        len_side_b = shape[1]
+        self.create_square_grid(len_side_a, len_side_b)
+        self.shape = (len_side_a, len_side_b)
+        self.type = 'SquareGrid'
+
+    def create_square_grid(self, len_side_a, len_side_b):
+        """
+        Create a square grid, where each vertex X[i][j] is linked to X[i-1][j], X[i][j-1], X[i+1][j], X[i][j+1] if they
+        exist.
+
+        :param len_side_a: integer, x coordinate
+        :param len_side_b: integer, y coordinate
+        """
+        if (len_side_a < 2) or (len_side_b < 2):
+            raise ValueError('side length attributes for HexagonalCells should be at least 2.')
+
+        self.connections, self.weights = create_grid_square_cells(len_side_a, len_side_b)
+        self.shape = (len_side_a, len_side_b)
+
+        # populate the dictionary from cell coordinates to cell indexes in arrays connection and weights
+        for i in range(len_side_a):
+            for j in range(len_side_b):
+                self.dict_cell_id_to_ind[(i, j)] = j + i*len_side_b
+
+
+class SquareGridsConvertBetween1DArrayAnd2DArrays:
+    def __init__(self, **kwargs):
+        self._array_optimized_squarification = None
+        self._array_optimized_flat = None
+
+    def _sampy_debug_convert_1d_array_to_2d_array(self, input_arr):
+        if not type(input_arr) is np.ndarray:
+            raise ValueError("Input variable is not a numpy array.")
+        if input_arr.shape != (self.number_vertices,):
+            raise ValueError("Input array of invalid shape.")
+
+    def convert_1d_array_to_2d_array(self, input_arr):
+        """
+        Takes a 1D array of shape (nb_vertices,) and convert it into a 2D array of shape self.shape.
+
+        :param input_arr: 1D array.
+        :return: 2D array
+        """
+        if self._array_optimized_squarification is None:
+            self._array_optimized_squarification = np.full((self.number_vertices, 2), 0)
+            for key, val in self.dict_cell_id_to_ind.items():
+                self._array_optimized_squarification[val][0] = key[0]
+                self._array_optimized_squarification[val][1] = key[1]
+        return topology_convert_1d_array_to_2d_array(input_arr, self._array_optimized_squarification,
+                                                     self.shape[0], self.shape[1])
+
+    def _sampy_debug_convert_2d_array_to_1d_array(self, input_arr):
+        if not type(input_arr) is np.ndarray:
+            raise ValueError("Input variable is not a numpy array.")
+        if input_arr.shape != self.shape:
+            raise ValueError("Input array of invalid shape.")
+
+    def convert_2d_array_to_1d_array(self, input_array):
+        """
+
+        :param input_array:
+        :return:
+        """
+        if self._array_optimized_flat is None:
+            self._array_optimized_flat = np.full(self.shape, 0)
+            for key, val in self.dict_cell_id_to_ind.items():
+                self._array_optimized_flat[key[0], key[1]] = val
+        return topology_convert_2d_array_to_1d_array(input_array, self._array_optimized_flat)
+
+
+class IcosphereTopology(BaseTopology):
+    def __init__(self, nb_sub=None, radius=1., **kwargs):
+        if nb_sub is None:
+            raise ValueError("kwarg nb_sub missing")
+        self.nb_sub = nb_sub
+        self.radius = float(radius)
+
+        icosahedron = SubdividedIcosahedron(nb_sub)
+        self.connections = np.copy(icosahedron.connections)
+        self.weights = np.copy(icosahedron.weights)
+        self.arr_coord = np.copy(icosahedron.arr_coord)
+        del icosahedron
+
+        # in the case of icoSphere Graph, vertices don't have a 'human readable' id (yet)
+        self.dict_cell_id_to_ind = {i:i for i in range(self.number_vertices)}
+
+        self.type = 'IcoSphere'
+        self.three_d_coord_created = False
+
+    def create_3d_coord(self):
+        self.df_attributes['coord_x'] = self.arr_coord[:, 0].astype(np.float64)
+        self.df_attributes['coord_y'] = self.arr_coord[:, 1].astype(np.float64)
+        self.df_attributes['coord_z'] = self.arr_coord[:, 2].astype(np.float64)
+
+        norm = np.sqrt(self.df_attributes['coord_x']**2 +
+                       self.df_attributes['coord_y']**2 +
+                       self.df_attributes['coord_z']**2)
+
+        self.df_attributes['coord_x_normalized'] = self.df_attributes['coord_x'] / norm
+        self.df_attributes['coord_x'] = self.radius * self.df_attributes['coord_x_normalized']
+
+        self.df_attributes['coord_y_normalized'] = self.df_attributes['coord_y'] / norm
+        self.df_attributes['coord_y'] = self.radius * self.df_attributes['coord_y_normalized']
+
+        self.df_attributes['coord_z_normalized'] = self.df_attributes['coord_z'] / norm
+        self.df_attributes['coord_z'] = self.radius * self.df_attributes['coord_z_normalized']
+
+        self.three_d_coord_created = True
+
+    def create_pseudo_epsg4326_coordinates(self):
+        """
+        This method approximate the shape of the earth using a sphere, which creates deformations.
+        """
+        if not self.three_d_coord_created:
+            self.create_3d_coord()
+
+        self.df_attributes['lat'] = (180*(pi/2 - np.arccos(self.df_attributes['coord_z_normalized']))/pi).astype(np.float64)
+        self.df_attributes['lon'] = (180*np.arctan2(self.df_attributes['coord_y_normalized'],
+                                                   self.df_attributes['coord_x_normalized'])/pi).astype(np.float64)
+
+    def compute_distance_matrix_on_sphere(self):
+        """
+        This method compute a distance matrix that gives the distance between each pair of connected vertex of the
+        graph. The distance is the geodesic distance on a sphere (i.e. the distance
+
+        :return: Array of floats with the same shape as the array 'connections'
+        """
+        dist_matrix = np.full(self.connections.shape, -1., dtype=np.float64)
+        lats_rad = (np.pi * self.df_attributes['lat'] / 180).astype(np.float64)
+        lons_rad = (np.pi * self.df_attributes['lon'] / 180).astype(np.float64)
+
+        dist_matrix = icosphere_get_distance_matrix(dist_matrix, self.connections, lats_rad, lons_rad, self.radius)
+
+        return dist_matrix
+
+    def create_and_save_radius_cells_as_attribute(self, radius_attribute='radius_each_cell'):
+        """
+        Save radius of each cell. The radius of a cell centered on a vertex v is defined as the maximum distance between
+        v and its neighbours. The radius is saved within df_attributes.
+
+        :param radius_attribute: optional, string, default 'radius_each_cell'. Name of the attribute corresponding to
+                                 the radius of each cell.
+        """
+        dist_matrix = self.compute_distance_matrix_on_sphere()
+        max_distance = np.amax(dist_matrix, axis=1).astype(np.float64)
+        self.df_attributes[radius_attribute] = max_distance
+
+    def compute_surface_array(self):
+        """
+        Return an array giving the surface of each cell of the icosphere
+        :return: array of floats shape (nb_vertex,)
+        """
+        # note that this orientation is not necessarily clockwise, and can be anti-clockwise for some vertices.
+        # But this is not important for our purpose of computing the area of each cell of the icosphere.
+        oriented_neigh_vert = get_oriented_neighborhood_of_vertices(self.connections)
+
+        return get_surface_array(oriented_neigh_vert,
+                                 self.df_attributes['coord_x_normalized'],
+                                 self.df_attributes['coord_y_normalized'],
+                                 self.df_attributes['coord_z_normalized'],
+                                 self.radius).astype(np.float64)
+
+    def create_and_save_surface_array_as_attribute(self):
+        arr_surface = self.compute_surface_array()
+        self.df_attributes['surface_cell'] = arr_surface
+
+
+class OrientedHexagonalGridOnSquare(BaseTopology):
+    """
+    Create an hexagonal grid on a square. The shape of the 5 x 3 grid is as follows:
+
+       *   *       *   *       *   *
+     *       *   *       *   *       *
+       *   *       *   *       *   *
+     *       *   *       *   *       *
+       *   *       *   *       *   *
+     *       *   *       *   *       *
+       *   *       *   *       *   *
+
+    """
+    def __init__(self, nb_hex_x_axis=None, nb_hex_y_axis=None, **kwargs):
+        """
+        :param nb_hex_x_axis: mandatory kwargs. Integer, number of hexagons on the horizontal axis.
+        :param nb_hex_y_axis: mandatory kwargs. Integer, number of hexagons on the vertical axis.
+        """
+        if (nb_hex_x_axis is None) or (nb_hex_y_axis is None):
+            raise ValueError("Mandatory kwargs missing: 'nb_hex_x_axis' and/or 'nb_hex_y_axis'." + 
+                             " Integers strictly bigger than Two are expected.")
+        self.connections, self.weights = create_grid_hexagonal_cells(nb_hex_x_axis, nb_hex_y_axis)
+        counter = 0
+        for i in range(nb_hex_x_axis):
+            for j in range(nb_hex_y_axis):
+                self.dict_cell_id_to_ind[(i, j)] = counter
+                counter += 1
```

### Comparing `sampy-abm-1.0.2/src/sampy/graph/vertex_attributes.py` & `sampy_abm-1.0.3/src/sampy/graph/vertex_attributes.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-import numpy as np
-from .jit_compiled_functions import compute_sin_attr_with_condition
-from ..pandas_xs.pandas_xs import DataFrameXS
-
-
-class BaseVertexAttributes:
-    def __init__(self, **kwargs):
-        if not hasattr(self, 'df_attributes'):
-            self.df_attributes = DataFrameXS()
-
-    def _sampy_debug_create_vertex_attribute(self, attr_name, value):
-        if not isinstance(attr_name, str):
-            raise TypeError("the name of a vertex attribute should be a string.")
-        arr = np.array(value)
-        if len(arr.shape) != 0:
-            if len(arr.shape) > 1:
-                raise ValueError('Shape of provided array for graph attribute ' + attr_name + ' is ' + str(arr.shape) +
-                                 ', while Sampy expects an array of shape (' + str(self.weights.shape[0]) +
-                                 ',).')
-            if arr.shape[0] != self.weights.shape[0]:
-                raise ValueError('Provided array for graph attribute ' + attr_name + ' has ' +
-                                 str(arr.shape[0]) + 'elements, while the graph has ' + str(self.weights.shape[0]) +
-                                 'vertices. Those numbers should be the same.')
-
-    def create_vertex_attribute(self, attr_name, value):
-        """
-        Creates a new vertex attribute and populates its values. Accepted input for 'value' are:
-                - None: in this case, the attribute column is set empty
-                - A single value, in which case all vertexes will have the same attribute value
-                - A 1D array, which will become the attribute column.
-
-        Note that if you use a 1D array, then you are implicitly working with the indexes of the vertices, that is that
-        the value at position 'i' in the array corresponds to the attribute value associated with the vertex whose index
-        is 'i'. If you want to work with vertexes id instead, use the method 'create_vertex_attribute_from_dict'.
-
-        :param attr_name: string, name of the attribute
-        :param value: either None, a single value, or a 1D array.
-        """
-        if self.df_attributes.nb_rows == 0 and len(np.array(value).shape) == 0:
-            self.df_attributes[attr_name] = [value for _ in range(self.weights.shape[0])]
-        else:
-            self.df_attributes[attr_name] = value
-
-    def _sampy_debug_create_vertex_attribute_from_dict(self, attr_name, dict_id_to_val, default_val=np.nan):
-        if (not hasattr(dict_id_to_val, 'items')) or (not hasattr(dict_id_to_val.items, '__call__')):
-            raise ValueError('the method create_vertex_attribute_from_dict expects a dictionnary-like object, ' +
-                             'which has a method \'items\'.')
-        if not isinstance(attr_name, str):
-            raise TypeError("the name of a vertex attribute should be a string.")
-        for key, _ in dict_id_to_val.items():
-            if key not in self.dict_cell_id_to_ind:
-                raise ValueError(str(key) + ' is not the id of any vertex in the graph.')
-
-    def create_vertex_attribute_from_dict(self, attr_name, dict_id_to_val, default_val):
-        """
-        Creates a new vertex attribute and populates its values using a dictionary-like object, whose keys are id of
-        vertices, and values the corresponding attribute values. Note that you can specify a default value for the
-        vertices not appearing in the dictionary.
-
-        IMPORTANT: first, the method creates an array filled with the default value, and then replace the values in the
-                   array using the dictionary. Therefore, the dtype of the attribute will be defined using the default
-                   value. Thus, the user should either chose a default value with appropriate dtype, or change the
-                   type of the attribute after creating the attribute.
-
-        :param attr_name: string, name of the attribute.
-        :param dict_id_to_val: Dictionary like object, whose keys are id of vertices, and values the corresponding
-                               attribute value.
-        :param default_val: Value used for the vertices for which an attribute value is not provided.
-        """
-        arr_attr = np.full((self.number_vertices,), default_val)
-        for key, val in dict_id_to_val.items():
-            arr_attr[self.dict_cell_id_to_ind[key]] = val
-        self.df_attributes[attr_name] = arr_attr
-
-    def change_type_attribute(self, attr_name, str_type):
-        """
-        Change the dtype of the selected attribute. Note that the type should be supported by DataFrameXS
-        :param attr_name: string, name of the attribute
-        :param str_type: string, target dtype of the attribute
-        """
-        self.df_attributes.change_type(attr_name, str_type)
-
-
-class PeriodicAttributes:
-    """
-    Class that adds methods to define periodically varying arguments.
-    """
-    def __init__(self, **kwargs):
-        if not hasattr(self, 'df_attributes'):
-            self.df_attributes = DataFrameXS()
-
-    def update_periodic_attribute(self, time, attr_name, amplitude, period, phase, intercept, condition=None):
-        """
-        Call this method to update the value of an attribute using the following formula.
-
-            amplitude * np.sin(2 * math.pi * time / period + phase) + intercept
-
-        Where time is either the value of the attribute 'time' of the graph, or if 'time' parameter is not None
-
-        :param time: float or int, used as time parameter in the update formula.
-        :param attr_name: string, name of the attribute
-        :param amplitude: float, see formula above
-        :param phase: float, see formula above
-        :param period: float, see formula above
-        :param intercept: float, see formula above
-        :param condition: optional, default None. Boolean Array saying for which cell to apply the sinusoidal variation.
-            If None, this method behave like an array of True has been provided.
-        """
-        arr_attr = self.df_attributes[attr_name]
-        if condition is None:
-            condition = np.full(arr_attr.shape, True, dtype=np.bool_)
-        if time is None:
-            time = self.time
-        compute_sin_attr_with_condition(arr_attr, condition, time, amplitude,
-                                        period, phase, intercept)
-
-
-class AttributesFrom2DArraysSquareGrids:
-    """
-    Allow the user to add attributes based on 2D arrays. Designed to work with 'SquareGrids' topologies.
-    """
-    def __init__(self, **kwargs):
-        pass
-
-    def create_attribute_from_2d_array(self, attr_name, array_2d):
-        """
-        Create or update an attribute based on a 2D array input.
-
-        :param attr_name: string, name of the attribute
-        :param array_2d: 2d array
-        """
-        if array_2d.shape != self.shape:
-            raise ValueError('Shapes do not match. Graph of shape ' + str(self.shape) +
-                             ' while array of shape ' + str(array_2d.shape) + '.')
-        arr_attr = np.full((self.number_vertices,), array_2d[0][0])
-        for i in range(array_2d.shape[0]):
-            for j in range(array_2d.shape[1]):
-                arr_attr[self.dict_cell_id_to_ind[(i, j)]] = array_2d[i][j]
-
-        self.df_attributes[attr_name] = arr_attr
+import numpy as np
+from .jit_compiled_functions import compute_sin_attr_with_condition
+from ..pandas_xs.pandas_xs import DataFrameXS
+
+
+class BaseVertexAttributes:
+    def __init__(self, **kwargs):
+        if not hasattr(self, 'df_attributes'):
+            self.df_attributes = DataFrameXS()
+
+    def _sampy_debug_create_vertex_attribute(self, attr_name, value):
+        if not isinstance(attr_name, str):
+            raise TypeError("the name of a vertex attribute should be a string.")
+        arr = np.array(value)
+        if len(arr.shape) != 0:
+            if len(arr.shape) > 1:
+                raise ValueError('Shape of provided array for graph attribute ' + attr_name + ' is ' + str(arr.shape) +
+                                 ', while Sampy expects an array of shape (' + str(self.weights.shape[0]) +
+                                 ',).')
+            if arr.shape[0] != self.weights.shape[0]:
+                raise ValueError('Provided array for graph attribute ' + attr_name + ' has ' +
+                                 str(arr.shape[0]) + 'elements, while the graph has ' + str(self.weights.shape[0]) +
+                                 'vertices. Those numbers should be the same.')
+
+    def create_vertex_attribute(self, attr_name, value):
+        """
+        Creates a new vertex attribute and populates its values. Accepted input for 'value' are:
+                - None: in this case, the attribute column is set empty
+                - A single value, in which case all vertexes will have the same attribute value
+                - A 1D array, which will become the attribute column.
+
+        Note that if you use a 1D array, then you are implicitly working with the indexes of the vertices, that is that
+        the value at position 'i' in the array corresponds to the attribute value associated with the vertex whose index
+        is 'i'. If you want to work with vertexes id instead, use the method 'create_vertex_attribute_from_dict'.
+
+        :param attr_name: string, name of the attribute
+        :param value: either None, a single value, or a 1D array.
+        """
+        if self.df_attributes.nb_rows == 0 and len(np.array(value).shape) == 0:
+            self.df_attributes[attr_name] = [value for _ in range(self.weights.shape[0])]
+        else:
+            self.df_attributes[attr_name] = value
+
+    def _sampy_debug_create_vertex_attribute_from_dict(self, attr_name, dict_id_to_val, default_val=np.nan):
+        if (not hasattr(dict_id_to_val, 'items')) or (not hasattr(dict_id_to_val.items, '__call__')):
+            raise ValueError('the method create_vertex_attribute_from_dict expects a dictionnary-like object, ' +
+                             'which has a method \'items\'.')
+        if not isinstance(attr_name, str):
+            raise TypeError("the name of a vertex attribute should be a string.")
+        for key, _ in dict_id_to_val.items():
+            if key not in self.dict_cell_id_to_ind:
+                raise ValueError(str(key) + ' is not the id of any vertex in the graph.')
+
+    def create_vertex_attribute_from_dict(self, attr_name, dict_id_to_val, default_val):
+        """
+        Creates a new vertex attribute and populates its values using a dictionary-like object, whose keys are id of
+        vertices, and values the corresponding attribute values. Note that you can specify a default value for the
+        vertices not appearing in the dictionary.
+
+        IMPORTANT: first, the method creates an array filled with the default value, and then replace the values in the
+                   array using the dictionary. Therefore, the dtype of the attribute will be defined using the default
+                   value. Thus, the user should either chose a default value with appropriate dtype, or change the
+                   type of the attribute after creating the attribute.
+
+        :param attr_name: string, name of the attribute.
+        :param dict_id_to_val: Dictionary like object, whose keys are id of vertices, and values the corresponding
+                               attribute value.
+        :param default_val: Value used for the vertices for which an attribute value is not provided.
+        """
+        arr_attr = np.full((self.number_vertices,), default_val)
+        for key, val in dict_id_to_val.items():
+            arr_attr[self.dict_cell_id_to_ind[key]] = val
+        self.df_attributes[attr_name] = arr_attr
+
+    def change_type_attribute(self, attr_name, str_type):
+        """
+        Change the dtype of the selected attribute. Note that the type should be supported by DataFrameXS
+        :param attr_name: string, name of the attribute
+        :param str_type: string, target dtype of the attribute
+        """
+        self.df_attributes.change_type(attr_name, str_type)
+
+
+class PeriodicAttributes:
+    """
+    Class that adds methods to define periodically varying arguments.
+    """
+    def __init__(self, **kwargs):
+        if not hasattr(self, 'df_attributes'):
+            self.df_attributes = DataFrameXS()
+
+    def update_periodic_attribute(self, time, attr_name, amplitude, period, phase, intercept, condition=None):
+        """
+        Call this method to update the value of an attribute using the following formula.
+
+            amplitude * np.sin(2 * math.pi * time / period + phase) + intercept
+
+        Where time is either the value of the attribute 'time' of the graph, or if 'time' parameter is not None
+
+        :param time: float or int, used as time parameter in the update formula.
+        :param attr_name: string, name of the attribute
+        :param amplitude: float, see formula above
+        :param phase: float, see formula above
+        :param period: float, see formula above
+        :param intercept: float, see formula above
+        :param condition: optional, default None. Boolean Array saying for which cell to apply the sinusoidal variation.
+            If None, this method behave like an array of True has been provided.
+        """
+        arr_attr = self.df_attributes[attr_name]
+        if condition is None:
+            condition = np.full(arr_attr.shape, True, dtype=np.bool_)
+        if time is None:
+            time = self.time
+        compute_sin_attr_with_condition(arr_attr, condition, time, amplitude,
+                                        period, phase, intercept)
+
+
+class AttributesFrom2DArraysSquareGrids:
+    """
+    Allow the user to add attributes based on 2D arrays. Designed to work with 'SquareGrids' topologies.
+    """
+    def __init__(self, **kwargs):
+        pass
+
+    def create_attribute_from_2d_array(self, attr_name, array_2d):
+        """
+        Create or update an attribute based on a 2D array input.
+
+        :param attr_name: string, name of the attribute
+        :param array_2d: 2d array
+        """
+        if array_2d.shape != self.shape:
+            raise ValueError('Shapes do not match. Graph of shape ' + str(self.shape) +
+                             ' while array of shape ' + str(array_2d.shape) + '.')
+        arr_attr = np.full((self.number_vertices,), array_2d[0][0])
+        for i in range(array_2d.shape[0]):
+            for j in range(array_2d.shape[1]):
+                arr_attr[self.dict_cell_id_to_ind[(i, j)]] = array_2d[i][j]
+
+        self.df_attributes[attr_name] = arr_attr
```

### Comparing `sampy-abm-1.0.2/src/sampy/intervention/built_in_interventions.py` & `sampy_abm-1.0.3/src/sampy/intervention/built_in_interventions.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from .vaccination import (BaseVaccinationSingleSpeciesDisease,
-                          VaccinationSingleSpeciesDiseaseFixedDuration)
-from .culling import (BaseCullingSingleSpecies,
-                      CullingSingleSpecies)
-from ..utils.decorators import sampy_class
-
-
-@sampy_class
-class BasicVaccination(BaseVaccinationSingleSpeciesDisease,
-                       VaccinationSingleSpeciesDiseaseFixedDuration):
-    """
-    Provide basic vaccination capacities. Vaccines have a fixed duration, always the same for every vaccinated agent.
-    When vaccinated, an agent is totally immuned to the disease.
-    """
-    def __init__(self, **kwargs):
-        pass
-
-
-@sampy_class
-class BasicCulling(BaseCullingSingleSpecies,
-                   CullingSingleSpecies):
-    """
-    Provide way to cull the agent population, notably by allowing to kill a given proportion of agents on cells.
-    """
-    def __init__(self, **kwargs):
-        pass
+from .vaccination import (BaseVaccinationSingleSpeciesDisease,
+                          VaccinationSingleSpeciesDiseaseFixedDuration)
+from .culling import (BaseCullingSingleSpecies,
+                      CullingSingleSpecies)
+from ..utils.decorators import sampy_class
+
+
+@sampy_class
+class BasicVaccination(BaseVaccinationSingleSpeciesDisease,
+                       VaccinationSingleSpeciesDiseaseFixedDuration):
+    """
+    Provide basic vaccination capacities. Vaccines have a fixed duration, always the same for every vaccinated agent.
+    When vaccinated, an agent is totally immuned to the disease.
+    """
+    def __init__(self, **kwargs):
+        pass
+
+
+@sampy_class
+class BasicCulling(BaseCullingSingleSpecies,
+                   CullingSingleSpecies):
+    """
+    Provide way to cull the agent population, notably by allowing to kill a given proportion of agents on cells.
+    """
+    def __init__(self, **kwargs):
+        pass
```

### Comparing `sampy-abm-1.0.2/src/sampy/intervention/culling.py` & `sampy_abm-1.0.3/src/sampy/intervention/culling.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import numpy as np
-from .jit_compiled_functions import culling_apply_culling_from_array_condition
-
-
-class BaseCullingSingleSpecies:
-    def __init__(self, species=None, **kwargs):
-        if species is None:
-            raise ValueError(
-                "No agent object provided for the culling. Should be provided using kwarg 'species'.")
-        self.species = species
-
-
-class CullingSingleSpecies:
-    def __init__(self, **kwargs):
-        pass
-
-    def apply_culling_from_array(self, array_culling_level, condition=None, position_attribute='position'):
-        """
-        Kill proportion of agents based on the 1D array 'array_culling_level'. array_culling_level[i] is the
-        probability for an agent on the vertex of index i to be killed.
-
-        By default, all agent can be killed. Use kwarg 'condition' to refine the culling.
-
-        :param array_culling_level: 1D array of float
-        :param condition: optional, 1D array of bool, default None.
-        :param position_attribute: optionnal, string, default 'position'
-        """
-        if condition is None:
-            condition = np.full((self.species.df_population.nb_rows,), True, dtype=np.bool_)
-
-        rand = np.random.uniform(0, 1, (condition.sum(),))
-
-        survive_culling = culling_apply_culling_from_array_condition(array_culling_level,
-                                                                     self.species.df_population[position_attribute],
-                                                                     rand, condition)
-
-        self.species.df_population = self.species.df_population[survive_culling]
-
-    def apply_culling_from_dict(self, graph, dict_vertex_id_to_level, condition=None, position_attribute='position'):
-        """
-        Same as apply_culling_from_array, but the 1D array is replaced by a dictionary whose keys are vertices ID and
-        values is the culling level on each cell.
-
-        :param graph: graph object on which the culling is applied
-        :param dict_vertex_id_to_level: dictionnary-like object with culling level
-        :param condition: optional, 1D array of bool, default None.
-        :param position_attribute: optional, string, default 'position'.
-        """
-        array_cul_level = np.full((graph.number_vertices,), 0., dtype=float)
-        for id_vertex, level in dict_vertex_id_to_level.items():
-            array_cul_level[graph.dict_cell_id_to_ind[id_vertex]] = level
-        self.apply_culling_from_array(array_cul_level, condition=condition, position_attribute=position_attribute)
+import numpy as np
+from .jit_compiled_functions import culling_apply_culling_from_array_condition
+
+
+class BaseCullingSingleSpecies:
+    def __init__(self, species=None, **kwargs):
+        if species is None:
+            raise ValueError(
+                "No agent object provided for the culling. Should be provided using kwarg 'species'.")
+        self.species = species
+
+
+class CullingSingleSpecies:
+    def __init__(self, **kwargs):
+        pass
+
+    def apply_culling_from_array(self, array_culling_level, condition=None, position_attribute='position'):
+        """
+        Kill proportion of agents based on the 1D array 'array_culling_level'. array_culling_level[i] is the
+        probability for an agent on the vertex of index i to be killed.
+
+        By default, all agent can be killed. Use kwarg 'condition' to refine the culling.
+
+        :param array_culling_level: 1D array of float
+        :param condition: optional, 1D array of bool, default None.
+        :param position_attribute: optionnal, string, default 'position'
+        """
+        if condition is None:
+            condition = np.full((self.species.df_population.nb_rows,), True, dtype=np.bool_)
+
+        rand = np.random.uniform(0, 1, (condition.sum(),))
+
+        survive_culling = culling_apply_culling_from_array_condition(array_culling_level,
+                                                                     self.species.df_population[position_attribute],
+                                                                     rand, condition)
+
+        self.species.df_population = self.species.df_population[survive_culling]
+
+    def apply_culling_from_dict(self, graph, dict_vertex_id_to_level, condition=None, position_attribute='position'):
+        """
+        Same as apply_culling_from_array, but the 1D array is replaced by a dictionary whose keys are vertices ID and
+        values is the culling level on each cell.
+
+        :param graph: graph object on which the culling is applied
+        :param dict_vertex_id_to_level: dictionnary-like object with culling level
+        :param condition: optional, 1D array of bool, default None.
+        :param position_attribute: optional, string, default 'position'.
+        """
+        array_cul_level = np.full((graph.number_vertices,), 0., dtype=float)
+        for id_vertex, level in dict_vertex_id_to_level.items():
+            array_cul_level[graph.dict_cell_id_to_ind[id_vertex]] = level
+        self.apply_culling_from_array(array_cul_level, condition=condition, position_attribute=position_attribute)
```

### Comparing `sampy-abm-1.0.2/src/sampy/intervention/jit_compiled_functions.py` & `sampy_abm-1.0.3/src/sampy/intervention/jit_compiled_functions.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import numba as nb
-import numpy as np
-
-
-@nb.njit
-def vaccination_apply_vaccine_from_array_condition(arr_vaccine_status, arr_cnt_vaccine_status, arr_immune_status,
-                                                   arr_vaccine_level, arr_position, rand, condition):
-    counter_rand = 0
-    newly_vaccinated = np.full(arr_vaccine_status.shape, False, dtype=np.bool_)
-    for i in range(arr_vaccine_status.shape[0]):
-        if condition[i]:
-            if rand[counter_rand] < arr_vaccine_level[arr_position[i]]:
-                arr_vaccine_status[i] = True
-                arr_cnt_vaccine_status[i] = 0
-                arr_immune_status[i] = True
-                newly_vaccinated[i] = True
-            counter_rand += 1
-    return newly_vaccinated
-
-
-@nb.njit
-def culling_apply_culling_from_array_condition(arr_culling_level, arr_position, rand, condition):
-    counter_rand = 0
-    survive = np.full(arr_position.shape, True, dtype=np.bool_)
-    for i in range(arr_position.shape[0]):
-        if condition[i]:
-            if rand[counter_rand] < arr_culling_level[arr_position[i]]:
-                survive[i] = False
-            counter_rand += 1
-    return survive
-
-
-def sampling_get_potential_targets(arr_position, arr_level_per_position):
-    set_allowed_pos = set([i for i, val in enumerate(arr_level_per_position) if val > 0.])
-    return np.array([u in set_allowed_pos for u in arr_position])
-
-
-@nb.njit
-def sampling_sample_from_array_condition(arr_sampling_level, arr_position, rand, condition):
-    sampled = np.full(arr_position.shape, False, dtype=np.bool_)
-    counter_rand = 0
-    for i in range(arr_position.shape[0]):
-        if condition[i]:
-            if rand[counter_rand] < arr_sampling_level[arr_position[i]]:
-                sampled[i] = True
-            counter_rand += 1
-    return sampled
+import numba as nb
+import numpy as np
+
+
+@nb.njit
+def vaccination_apply_vaccine_from_array_condition(arr_vaccine_status, arr_cnt_vaccine_status, arr_immune_status,
+                                                   arr_vaccine_level, arr_position, rand, condition):
+    counter_rand = 0
+    newly_vaccinated = np.full(arr_vaccine_status.shape, False, dtype=np.bool_)
+    for i in range(arr_vaccine_status.shape[0]):
+        if condition[i]:
+            if rand[counter_rand] < arr_vaccine_level[arr_position[i]]:
+                arr_vaccine_status[i] = True
+                arr_cnt_vaccine_status[i] = 0
+                arr_immune_status[i] = True
+                newly_vaccinated[i] = True
+            counter_rand += 1
+    return newly_vaccinated
+
+
+@nb.njit
+def culling_apply_culling_from_array_condition(arr_culling_level, arr_position, rand, condition):
+    counter_rand = 0
+    survive = np.full(arr_position.shape, True, dtype=np.bool_)
+    for i in range(arr_position.shape[0]):
+        if condition[i]:
+            if rand[counter_rand] < arr_culling_level[arr_position[i]]:
+                survive[i] = False
+            counter_rand += 1
+    return survive
+
+
+def sampling_get_potential_targets(arr_position, arr_level_per_position):
+    set_allowed_pos = set([i for i, val in enumerate(arr_level_per_position) if val > 0.])
+    return np.array([u in set_allowed_pos for u in arr_position])
+
+
+@nb.njit
+def sampling_sample_from_array_condition(arr_sampling_level, arr_position, rand, condition):
+    sampled = np.full(arr_position.shape, False, dtype=np.bool_)
+    counter_rand = 0
+    for i in range(arr_position.shape[0]):
+        if condition[i]:
+            if rand[counter_rand] < arr_sampling_level[arr_position[i]]:
+                sampled[i] = True
+            counter_rand += 1
+    return sampled
```

### Comparing `sampy-abm-1.0.2/src/sampy/intervention/sampling.py` & `sampy_abm-1.0.3/src/sampy/intervention/sampling.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-import numpy as np
-from .jit_compiled_functions import (sampling_get_potential_targets,
-                                     sampling_sample_from_array_condition)
-
-
-class BaseSamplingSingleSpecies:
-    """
-    Base Class for single species sampling.
-    """
-    def __init__(self, target_species=None, **kwargs):
-        if target_species is None:
-            raise ValueError("No agent object provided for the sampling. Should be provided using kwarg "
-                             "'target_species'.")
-        self.target_species = target_species
-
-
-class SamplingSingleSpecies:
-    """
-    Introduce the methods for sampling a single species
-    """
-    def __init__(self, **kwargs):
-        pass
-
-    def sample_proportion_from_array(self, array_proportion, condition=None, position_attribute='position',
-                                     return_as_pandas_df=False, eliminate_sampled_pop=False):
-        """
-        Take as input an array telling the proportion of agent to sample in each vertex.
-
-        :param array_proportion: 1D array of float. array_proportion[i] is the probability for an agent living in the
-                                 vertex of index i.
-        :param condition: optional, 1D array of bool, default None. If not None, tell which agent can be sampled.
-        :param position_attribute: optional, string, default 'position'. Tell which attribute of the agents should
-                                   be used as position.
-        :param return_as_pandas_df: optional, boolean, default False. Clear.
-        :param eliminate_sampled_pop: optional, boolean, default False. If True,
-
-        :return: a DataFrameXS if return_as_pandas_df is False, a pandas dataframe otherwise. The returned DF is
-                 the sample of the population taken from df_population
-        """
-        targets = sampling_get_potential_targets(self.target_species.df_population[position_attribute],
-                                                 array_proportion)
-        if condition is not None:
-            targets = targets & condition
-
-        rand = np.random.uniform(0, 1, (targets.sum(),))
-
-        sampled = sampling_sample_from_array_condition(array_proportion,
-                                                       self.target_species.df_population[position_attribute],
-                                                       rand, targets)
-
+import numpy as np
+from .jit_compiled_functions import (sampling_get_potential_targets,
+                                     sampling_sample_from_array_condition)
+
+
+class BaseSamplingSingleSpecies:
+    """
+    Base Class for single species sampling.
+    """
+    def __init__(self, target_species=None, **kwargs):
+        if target_species is None:
+            raise ValueError("No agent object provided for the sampling. Should be provided using kwarg "
+                             "'target_species'.")
+        self.target_species = target_species
+
+
+class SamplingSingleSpecies:
+    """
+    Introduce the methods for sampling a single species
+    """
+    def __init__(self, **kwargs):
+        pass
+
+    def sample_proportion_from_array(self, array_proportion, condition=None, position_attribute='position',
+                                     return_as_pandas_df=False, eliminate_sampled_pop=False):
+        """
+        Take as input an array telling the proportion of agent to sample in each vertex.
+
+        :param array_proportion: 1D array of float. array_proportion[i] is the probability for an agent living in the
+                                 vertex of index i.
+        :param condition: optional, 1D array of bool, default None. If not None, tell which agent can be sampled.
+        :param position_attribute: optional, string, default 'position'. Tell which attribute of the agents should
+                                   be used as position.
+        :param return_as_pandas_df: optional, boolean, default False. Clear.
+        :param eliminate_sampled_pop: optional, boolean, default False. If True,
+
+        :return: a DataFrameXS if return_as_pandas_df is False, a pandas dataframe otherwise. The returned DF is
+                 the sample of the population taken from df_population
+        """
+        targets = sampling_get_potential_targets(self.target_species.df_population[position_attribute],
+                                                 array_proportion)
+        if condition is not None:
+            targets = targets & condition
+
+        rand = np.random.uniform(0, 1, (targets.sum(),))
+
+        sampled = sampling_sample_from_array_condition(array_proportion,
+                                                       self.target_species.df_population[position_attribute],
+                                                       rand, targets)
+
```

### Comparing `sampy-abm-1.0.2/src/sampy/intervention/vaccination.py` & `sampy_abm-1.0.3/src/sampy/intervention/vaccination.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-import numpy as np
-from ..pandas_xs.pandas_xs import DataFrameXS
-from .jit_compiled_functions import vaccination_apply_vaccine_from_array_condition
-
-
-class BaseVaccinationSingleSpeciesDisease:
-    def __init__(self, disease=None, **kwargs):
-        if disease is None:
-            raise ValueError(
-                "No disease object provided for the vaccination. Should be provided using kwarg 'disease'.")
-        self.disease = disease
-        self.target_species = self.disease.host
-        self.target_species.df_population['vaccinated_' + self.disease.disease_name] = False
-        self.target_species.dict_default_val['vaccinated_' + self.disease.disease_name] = False
-
-
-class VaccinationSingleSpeciesDiseaseFixedDuration:
-    def __init__(self, duration_vaccine=None, **kwargs):
-        if duration_vaccine is None:
-            raise ValueError(
-                "No duration provided for the vaccination duration. Should be provided using kwarg 'duration_vaccine'.")
-        self.duration_vaccine = int(duration_vaccine)
-        self.target_species.df_population['cnt_vaccinated_' + self.disease.disease_name] = 0
-        self.target_species.dict_default_val['cnt_vaccinated_' + self.disease.disease_name] = 0
-
-    def update_vaccine_status(self):
-        """
-        Should be call at each time-step of the simulation. Update the attribute that count how many day each individual
-        has been vaccinated, and remove the vaccinated status of the individual which recieved their dose for more than
-        'duration_vaccine' time-steps.
-        """
-        self.target_species.df_population['cnt_vaccinated_' + self.disease.disease_name] += 1
-
-        arr_lose_vaccine = self.target_species.df_population['cnt_vaccinated_' + self.disease.disease_name] >= \
-                           self.duration_vaccine
-        not_arr_lose_vaccine = ~arr_lose_vaccine
-
-        self.target_species.df_population['cnt_vaccinated_' + self.disease.disease_name] = \
-            self.target_species.df_population['cnt_vaccinated_' + self.disease.disease_name] * not_arr_lose_vaccine
-        self.target_species.df_population['vaccinated_' + self.disease.disease_name] = \
-            self.target_species.df_population['vaccinated_' + self.disease.disease_name] * not_arr_lose_vaccine
-        self.target_species.df_population['imm_' + self.disease.disease_name] = \
-            self.target_species.df_population['imm_' + self.disease.disease_name] * not_arr_lose_vaccine
-
-    def apply_vaccine_from_array(self, array_vaccine_level, condition=None, position_attribute='position'):
-        """
-        Apply vaccine to the agents based on the 1D array 'array_vaccine_level'. array_vaccine_level[i] is the
-        probability for an agent on the vertex of index i to get vaccinated.
-
-        Note that, by default, infected and contagious agents can get vaccinated. They can be excluded using the
-        kwarg 'condition'
-
-        :param array_vaccine_level: 1D array of float. Floats between 0 and 1.
-        :param condition: optional, 1D array of bool, default None.
-        :param position_attribute: optional, string, default 'position'.
-        """
-        if condition is None:
-            condition = np.full((self.target_species.df_population.nb_rows,), True, dtype=np.bool_)
-
-        rand = np.random.uniform(0, 1, (condition.sum(),))
-
-        newly_vaccinated = \
-            vaccination_apply_vaccine_from_array_condition(
-                self.target_species.df_population['vaccinated_' + self.disease.disease_name],
-                self.target_species.df_population['cnt_vaccinated_' + self.disease.disease_name],
-                self.target_species.df_population['imm_' + self.disease.disease_name],
-                array_vaccine_level, self.target_species.df_population[position_attribute], rand, condition)
-
-        not_newly_vaccinated = ~newly_vaccinated
-        self.target_species.df_population['inf_' + self.disease.disease_name] *= not_newly_vaccinated
-        self.target_species.df_population['con_' + self.disease.disease_name] *= not_newly_vaccinated
-
-    def apply_vaccine_from_dict(self, graph, dict_vertex_id_to_level, condition=None, position_attribute='position'):
-        """
-        same as apply_vaccine_from_array, but the 1D array is replaced by a dictionary whose keys are vertices ID and
-        values is the vaccination level on each cell.
-
-        :param graph: graph object on which the vaccine is applied
-        :param dict_vertex_id_to_level: dictionnary-like object with vaccine level
-        :param condition: optional, 1D array of bool, default None.
-        :param position_attribute: optional, string, default 'position'.
-        """
-        array_vac_level = np.full((graph.number_vertices,), 0., dtype=float)
-        for id_vertex, level in dict_vertex_id_to_level.items():
-            array_vac_level[graph.dict_cell_id_to_ind[id_vertex]] = level
-
-        self.apply_vaccine_from_array(array_vac_level, condition=condition, position_attribute=position_attribute)
+import numpy as np
+from ..pandas_xs.pandas_xs import DataFrameXS
+from .jit_compiled_functions import vaccination_apply_vaccine_from_array_condition
+
+
+class BaseVaccinationSingleSpeciesDisease:
+    def __init__(self, disease=None, **kwargs):
+        if disease is None:
+            raise ValueError(
+                "No disease object provided for the vaccination. Should be provided using kwarg 'disease'.")
+        self.disease = disease
+        self.target_species = self.disease.host
+        self.target_species.df_population['vaccinated_' + self.disease.disease_name] = False
+        self.target_species.dict_default_val['vaccinated_' + self.disease.disease_name] = False
+
+
+class VaccinationSingleSpeciesDiseaseFixedDuration:
+    def __init__(self, duration_vaccine=None, **kwargs):
+        if duration_vaccine is None:
+            raise ValueError(
+                "No duration provided for the vaccination duration. Should be provided using kwarg 'duration_vaccine'.")
+        self.duration_vaccine = int(duration_vaccine)
+        self.target_species.df_population['cnt_vaccinated_' + self.disease.disease_name] = 0
+        self.target_species.dict_default_val['cnt_vaccinated_' + self.disease.disease_name] = 0
+
+    def update_vaccine_status(self):
+        """
+        Should be call at each time-step of the simulation. Update the attribute that count how many day each individual
+        has been vaccinated, and remove the vaccinated status of the individual which recieved their dose for more than
+        'duration_vaccine' time-steps.
+        """
+        self.target_species.df_population['cnt_vaccinated_' + self.disease.disease_name] += 1
+
+        arr_lose_vaccine = self.target_species.df_population['cnt_vaccinated_' + self.disease.disease_name] >= \
+                           self.duration_vaccine
+        not_arr_lose_vaccine = ~arr_lose_vaccine
+
+        self.target_species.df_population['cnt_vaccinated_' + self.disease.disease_name] = \
+            self.target_species.df_population['cnt_vaccinated_' + self.disease.disease_name] * not_arr_lose_vaccine
+        self.target_species.df_population['vaccinated_' + self.disease.disease_name] = \
+            self.target_species.df_population['vaccinated_' + self.disease.disease_name] * not_arr_lose_vaccine
+        self.target_species.df_population['imm_' + self.disease.disease_name] = \
+            self.target_species.df_population['imm_' + self.disease.disease_name] * not_arr_lose_vaccine
+
+    def apply_vaccine_from_array(self, array_vaccine_level, condition=None, position_attribute='position'):
+        """
+        Apply vaccine to the agents based on the 1D array 'array_vaccine_level'. array_vaccine_level[i] is the
+        probability for an agent on the vertex of index i to get vaccinated.
+
+        Note that, by default, infected and contagious agents can get vaccinated. They can be excluded using the
+        kwarg 'condition'
+
+        :param array_vaccine_level: 1D array of float. Floats between 0 and 1.
+        :param condition: optional, 1D array of bool, default None.
+        :param position_attribute: optional, string, default 'position'.
+        """
+        if condition is None:
+            condition = np.full((self.target_species.df_population.nb_rows,), True, dtype=np.bool_)
+
+        rand = np.random.uniform(0, 1, (condition.sum(),))
+
+        newly_vaccinated = \
+            vaccination_apply_vaccine_from_array_condition(
+                self.target_species.df_population['vaccinated_' + self.disease.disease_name],
+                self.target_species.df_population['cnt_vaccinated_' + self.disease.disease_name],
+                self.target_species.df_population['imm_' + self.disease.disease_name],
+                array_vaccine_level, self.target_species.df_population[position_attribute], rand, condition)
+
+        not_newly_vaccinated = ~newly_vaccinated
+        self.target_species.df_population['inf_' + self.disease.disease_name] *= not_newly_vaccinated
+        self.target_species.df_population['con_' + self.disease.disease_name] *= not_newly_vaccinated
+
+    def apply_vaccine_from_dict(self, graph, dict_vertex_id_to_level, condition=None, position_attribute='position'):
+        """
+        same as apply_vaccine_from_array, but the 1D array is replaced by a dictionary whose keys are vertices ID and
+        values is the vaccination level on each cell.
+
+        :param graph: graph object on which the vaccine is applied
+        :param dict_vertex_id_to_level: dictionnary-like object with vaccine level
+        :param condition: optional, 1D array of bool, default None.
+        :param position_attribute: optional, string, default 'position'.
+        """
+        array_vac_level = np.full((graph.number_vertices,), 0., dtype=float)
+        for id_vertex, level in dict_vertex_id_to_level.items():
+            array_vac_level[graph.dict_cell_id_to_ind[id_vertex]] = level
+
+        self.apply_vaccine_from_array(array_vac_level, condition=condition, position_attribute=position_attribute)
```

### Comparing `sampy-abm-1.0.2/src/sampy/pandas_xs/pandas_xs.py` & `sampy_abm-1.0.3/src/sampy/pandas_xs/pandas_xs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,482 +1,523 @@
-import numpy as np
-import copy
-from .jit_compiled_functions import dataframe_xs_check_arr_in_col, dataframe_xs_check_arr_in_col_conditional
-import pandas as pd
-
-
-class DataFrameXS:
-    """
-    Class that encodes a really simplified version of a dataframe, where each column is stored as a separated one
-    dimensional numpy array. Note that this class is made to be more rigid than Pandas Dataframe: the class won't try
-    to fill in blanks or fancy things like that. The idea being to maintain control on what is going on and avoid bugs
-    that goes unnoticed.
-
-    Indexing:
-    ---------
-    3 types of indexing are supported: indexing by a string, an array of bool or an array of int. Any other index will
-    raise a TypeError.
-        - Indexing by a string returns the corresponding column. Keep in mind that it is not a copy, and modifying it
-          will change the original column.
-        - Indexing by an array of bool returns a copy.
-        - Indexing by an array of int returns a copy.
-    """
-    LIST_ALLOWED_TYPE = ['bool', 'uint8', 'int8', 'uint16', 'int16', 'uint32', 'int32',
-                         'uint64', 'int64', 'float32', 'float64']
-    ALLOWED_TYPE = set(LIST_ALLOWED_TYPE)
-
-    def __init__(self):
-        self.list_col = []
-        self.list_col_name = []
-        self.dict_colname_to_index = dict()
-        self.nb_rows = 0
-        self.nb_cols = 0
-
-# ----------------------------------------------------------------------------------------------------------------------
-# class methods
-
-    @classmethod
-    def from_lists(cls, list_col_name, list_col):
-        """
-        Returns a DataFrameXS from a list of column names and a list of columns. If the lists are of different length,
-        or if some column names are repeated, an Exception will be raised.
-
-        :param list_col_name: list of strings
-        :param list_col: list of 1D numpy array, that will become columns of the dataframe.
-
-        :return: DataFrameXS object.
-        """
-        if len(list_col) != len(list_col_name):
-            raise ValueError("Inputs do not have the same length.")
-        if len(list_col_name) > len(set(list_col_name)):
-            raise ValueError("Several columns have the same name.")
-
-        r_df = cls()
-        for name, col in zip(list_col_name, list_col):
-            r_df[name] = col
-        return r_df
-
-    @classmethod
-    def from_dict(cls, dict_name_to_col):
-        """
-        Returns a DataFrameXS object from a dictionary whose keys are column names, and values are columns.
-
-        :param dict_name_to_col: dictionary, whose key are strings and values 1D numpy arrays or None.
-
-        :return: DataFrameXS object
-        """
-        r_df = cls()
-        for name, col in dict_name_to_col.items():
-            r_df[name] = col
-        return r_df
-
-    @classmethod
-    def read_csv(cls, path, sep=';', **kwargs):
-        """
-        Use pandas to read a csv, and then converts the pandas Dataframe into a DataFrameXS. Be careful that the type
-        of the columns are supported by DataFrameXS instances.
-
-        :param path: string, path to the csv
-        :param sep: optional, string, default ';'. Separator in the csv.
-
-        :return: DataFrameXS object
-        """
-        df = cls()
-        pd_df = pd.read_csv(path, sep=sep, **kwargs)
-        for name in pd_df:
-            df[name] = np.copy(np.array(pd_df[name]))
-        return df
-
-# ----------------------------------------------------------------------------------------------------------------------
-# __methods__
-
-    def __setitem__(self, key, value):
-        """
-        Allow the user to set a column values by using the syntax df[key] = value
-
-        :param key: string, name of the column
-        :param value: either a single value, in which case all the column will be set to this value, or an iterable that
-                      can be casted to a numpy array of supported type. If the Value is None, then the column
-                      is set empty.
-        """
-        # check if the user provided a string as a column name
-        if not isinstance(key, str):
-            raise ValueError("A column name should be a string in a dataframe_xs.")
-
-        # in case a column is set empty
-        if value is None:
-            self._add_empty_col(key)
-        else:
-            # cast the input as a numpy array
-            temp_value = np.array(value)
-
-            # check if the input is of allowed type
-            if str(temp_value.dtype) not in self.ALLOWED_TYPE:
-                raise ValueError("The proposed column is of an unsupported type. Supported types are " +
-                                 str(self.LIST_ALLOWED_TYPE))
-
-            # check if the user provided a single value
-            if len(temp_value.shape) == 0:
-                if self.nb_rows == 0:
-                    self._add_empty_col(key)
-                else:
-                    value = np.full((self.nb_rows,), value)
-                    self._add_col_without_nb_rows_check(key, value)
-
-            # if the user provided an input that results in an array of shape (0,)
-            elif temp_value.shape == (0,):
-                self._add_empty_col(key)
-
-            # Now the case of a real serie of values
-            else:
-                value = temp_value
-                # check that the the input is of dimension 1
-                if len(value.shape) > 1:
-                    raise ValueError("A column should be an array of dimension 1, and your input dim is " +
-                                     str(value.shape) + '.')
-
-                # in the case the dataframe is empty
-                if self.nb_rows == 0:
-                    self.nb_rows = value.shape[0]
-                    self._add_col_without_nb_rows_check(key, value)
-                else:
-                    if value.shape[0] != self.nb_rows:
-                        raise ValueError("Dataframe has " + str(self.nb_rows) + " rows while the input has " +
-                                         str(value.shape[0]) + '.')
-                    else:
-                        self._add_col_without_nb_rows_check(key, value)
-
-    def __getitem__(self, item):
-        """
-        Use the syntax df[item] to retrieve data. Three possible uses:
-            1) item is the name of a column: retrieve the corresponding column. Keep in mind that this is not a copy,
-               and modifying the obtained array will modify the column in the dataframe.
-            2) item is an array of bool of same length as the dataframe: retrieve a copy of the dataframe with only the
-               lines of position i such that item[i] == True.
-            3) item is an array of int: retrieve a copy of the dataframe
-
-        :param item: either a string, a 1D array of bool, or a 1D array of int.
-
-        :return: a column of the DataFrameXS if item is a string, a DataFrameXS object otherwise.
-        """
-        # if a string is provided, return the column as np.array
-        if isinstance(item, str):
-            if item not in self.dict_colname_to_index:
-                raise KeyError("No column named " + item + ".")
-            else:
-                return self.list_col[self.dict_colname_to_index[item]]
-
-        # if an array is provided
-        elif isinstance(item, np.ndarray):
-            # check if the array is empty
-            if len(item.shape) == 0 or item.shape == (0,):
-                raise IndexError("Cannot index using an empty array")
-
-            # check if the array is not of dim 1
-            if len(item.shape) != 1:
-                raise IndexError("Boolean array indexing requires the array of boolean indexes to be one dimensional.")
-
-            # case of an array of bool
-            elif str(item.dtype) == 'bool':
-                if item.shape[0] != self.nb_rows:
-                    raise IndexError("Boolean array indexing requires the array of boolean indexes to be of the same" +
-                                     "length as the dataframe.")
-                nb_rows = item.sum()
-                if nb_rows == 0:
-                    r_df = DataFrameXS()
-                    for name in self.list_col_name:
-                        r_df[name] = None
-                    return r_df
-                else:
-                    new_cols = []
-                    for col in self.list_col:
-                        if col is None:
-                            new_cols.append(None)
-                        else:
-                            new_cols.append(col[item])
-                    return self._create_df_without_check(self.list_col_name, new_cols, nb_rows, self.nb_cols)
-
-            # case of an array of int
-            elif str(item.dtype).startswith('int'):
-                new_cols = []
-                for name, col in zip(self.list_col_name, self.list_col):
-                    if col is None:
-                        new_cols.append(None)
-                    else:
-                        new_cols.append(col[item])
-                return self._create_df_without_check(self.list_col_name, new_cols, item.shape[0], self.nb_cols)
-            else:
-                raise TypeError("Indexing with an array is only allowed using Bool or Int arrays.")
-        else:
-            raise TypeError("A Dataframe XS only supports integer, array of int and array of bool indexing.")
-
-# ----------------------------------------------------------------------------------------------------------------------
-# private methods
-
-    def _add_empty_col(self, key):
-        if key in self.dict_colname_to_index:
-            self.list_col[self.dict_colname_to_index[key]] = None
-            if self.is_empty:
-                self.nb_rows = 0
-        else:
-            self.dict_colname_to_index[key] = self.nb_cols
-            self.nb_cols += 1
-            self.list_col_name.append(key)
-            self.list_col.append(None)
-
-    def _add_col_without_nb_rows_check(self, key, value):
-        if key in self.dict_colname_to_index:
-            self.list_col[self.dict_colname_to_index[key]] = value
-        else:
-            self.dict_colname_to_index[key] = self.nb_cols
-            self.nb_cols += 1
-            self.list_col_name.append(key)
-            self.list_col.append(value)
-
-    @classmethod
-    def _create_df_without_check(cls, list_col_name, list_col, nb_rows, nb_cols):
-        r_df = cls()
-        r_df.list_col_name = copy.deepcopy(list_col_name)
-        r_df.list_col = list_col
-        r_df.nb_rows = nb_rows
-        r_df.nb_cols = nb_cols
-        r_df.dict_colname_to_index = {name: index for index, name in enumerate(list_col_name)}
-        return r_df
-
-# ----------------------------------------------------------------------------------------------------------------------
-# properties
-
-    @property
-    def is_empty(self):
-        for value in self.list_col:
-            if value is not None:
-                return False
-        return True
-
-    @property
-    def shape(self):
-        return self.nb_rows, self.nb_cols
-
-# ----------------------------------------------------------------------------------------------------------------------
-# methods
-
-    def _sampy_debug_scramble(self, permutation=None, return_permutation=False):
-        if permutation is not None:
-            if not isinstance(permutation, np.ndarray):
-                raise TypeError("Permutation parameter should be an array.")
-            if not str(permutation.dtype).startswith('int'):
-                raise TypeError("Permutation parameter should be an array of integers.")
-            if not permutation.shape == (self.nb_rows,):
-                raise ValueError("Permutation parameter should be an array of integers of shape (nb_rows,).")
-            if not (np.sort(permutation) == np.arange(0, self.nb_rows)).all():
-                raise ValueError("Permutation parameter should be a permutation of the integers from 0 to nb_rows.")
-
-    def scramble(self, permutation=None, return_permutation=False):
-        """
-        Scramble the rows of the dataframe XS. The user can provide a permutation that will be used to scramble the
-        rows.
-
-        WARNING: if you use the keyword argument permutation, be sure you provide a permutation of the correct size.
-        Otherwise the result can be unpredictable.
-
-        :param permutation: optional, array of int, default None.
-        :param return_permutation: optional, boolean default False. If True, the function returns the permutation used
-                                   to shuffle the DataFrameXS (useful if some other objects have to be shuffled).
-        """
-        if permutation is None:
-            permutation = np.random.permutation(self.nb_rows)
-        for i, col in enumerate(self.list_col):
-            if col is not None:
-                self.list_col[i] = col[permutation]
-
-        if return_permutation:
-            return permutation
-
-    def _sampy_debug_get_copy(self, col_name):
-        if not isinstance(col_name, str):
-            raise TypeError("get_copy expects a string as argument.")
-        else:
-            if col_name not in self.dict_colname_to_index:
-                raise KeyError("no column with the name " + col_name + " in the dataframe.")
-
-    def get_copy(self, col_name):
-        """
-        Returns a copy of the selected column.
-        :param col_name: string, name of the column to copy.
-        """
-        col = self.list_col[self.dict_colname_to_index[col_name]]
-        if col is None:
-            return
-        else:
-            return np.copy(col)
-
-    def _sampy_debug_check_arr_in_col(self, input_arr, name_col, condition=None):
-        if condition is not None:
-            if not isinstance(condition, np.ndarray):
-                raise ValueError("condition should be an array.")
-            if str(condition.dtype) != 'bool':
-                raise ValueError("condition should be an array of bool.")
-            if input_arr.shape != condition.shape:
-                raise ValueError("condition and input_arr don't have the same shape.")
-
-        if not isinstance(input_arr, np.ndarray):
-            raise ValueError('Input array is not a numpy ndarray.')
-        if len(input_arr.shape) != 1:
-            raise ValueError('Input array is not one dimensional.')
-        if input_arr.shape[0] == 0:
-            raise ValueError('Input array is empty.')
-        if str(input_arr.dtype) != str(self[name_col].dtype):
-            raise ValueError("The input array (" + str(input_arr.dtype) + ") is not of the same type as the " +
-                             "selected column (" + str(self[name_col].dtype) + ").")
-
-    def check_arr_in_col(self, input_arr, name_col, condition=None):
-        """
-        Check which elements of the input array are in selected column.
-
-        :param input_arr: 1D numpy array.
-        :param name_col: string, name of the column
-        :param condition: optional, boolean array.
-
-        :return: 1D boolean array saying which elements of the input array are in the selected column.
-        """
-        if condition is None:
-            return dataframe_xs_check_arr_in_col(input_arr, self[name_col])
-        else:
-            return dataframe_xs_check_arr_in_col_conditional(input_arr, self[name_col], condition)
-
-    def _sampy_debug_change_type(self, col_name, str_type):
-        if not isinstance(str_type, str):
-            raise ValueError("str_type should be a string in the list: " + str(self.LIST_ALLOWED_TYPE) + ".")
-        if str_type not in self.ALLOWED_TYPE:
-            raise ValueError("The type " + str_type + "is not in " + str(self.LIST_ALLOWED_TYPE) + ".")
-
-    def change_type(self, col_name, str_type):
-        """
-        Change the type of a column. The selected type has to be in the allowed type list.
-        Do nothing if the selected column is empty.
-
-        :param col_name: string, name of the column whose type should be changed.
-        :param type: string, numpy identifier of the new type of the column.
-        """
-        if self[col_name] is not None:
-            self[col_name] = self[col_name].astype(str_type)
-
-    def copy(self):
-        """
-        Returns a copy of the dataframe
-        :return: a dataframeXS
-        """
-        new_list_col = []
-        for col in self.list_col:
-            new_list_col.append(np.copy(col))
-        return self._create_df_without_check(self.list_col_name, new_list_col, self.nb_rows, self.nb_cols)
-
-    def concat(self, df, inplace=True):
-        """
-        Append the input DataFrameXS to the current DataFrameXS. The column names of the current DataFrameXS have to be
-        column names of the input, or an Exception will be raised. Finally, note that the types of the columns of the
-        input will be casted to the types of the corresponding columns of the current DataFrameXS.
-
-        Extra columns in the input are ignored.
-
-        :param df: DataFrame XS
-        :param inplace: optional, boolean, default True. If True, the input is appended to the current DataFrame.
-                        Otherwise, a new DataFrameXS is returned.
-
-        :return: if inplace is False, return a DataFrameXS, otherwise returns None.
-        """
-        if not isinstance(df, DataFrameXS):
-            raise ValueError("Input is not a DataframeXS")
-
-        # case where the current DataFrameXS is empty, which can happen when initializing a simulation
-        if self.is_empty:
-
-            # if input is empty, the case is clear
-            if df.is_empty:
-                if inplace:
-                    return
-                else:
-                    return self.copy()
-
-            # if df is not empty, fill self columns with df columns
-            else:
-                new_col = []
-                for name in self.list_col_name:
-                    col = df[name]
-                    if col is None:
-                        new_col.append(None)
-                    else:
-                        new_col.append(np.copy(col))
-                if inplace:
-                    self.list_col = new_col
-                    self.nb_rows = df.nb_rows
-                else:
-                    return self._create_df_without_check(self.list_col_name, new_col, df.nb_rows, self.nb_cols)
-
-        # when both dataframes are not empty. Most important checks are done by __getitem__
-        elif not df.is_empty:
-            new_col = []
-            for name in self.list_col_name:
-                df_col = df[name]
-                self_col = self[name]
-                if self_col is not None:
-                    if df_col is not None:
-                        new_col.append(np.hstack([self_col, df_col]).astype(self_col.dtype))
-                    else:
-                        filled_col = np.full((df.nb_rows,), np.nan).astype(self_col.dtype)
-                        new_col.append(np.hstack([self_col, filled_col]).astype(self_col.dtype))
-                else:
-                    if df_col is not None:
-                        filled_col = np.full((self.nb_rows,), np.nan).astype(df_col.dtype)
-                        new_col.append(np.hstack([filled_col, df_col]).astype(df_col.dtype))
-                    else:
-                        new_col.append(None)
-            if inplace:
-                self.nb_rows += df.nb_rows
-                self.list_col = new_col
-            else:
-                return self._create_df_without_check(self.list_col_name, new_col, self.nb_rows + df.nb_rows,
-                                                     self.nb_cols)
-
-        # when current is not empty, and input is. No checks are done in this case.
-        else:
-            if inplace:
-                return
-            else:
-                return self.copy()
-
-    def add_rows_from_dict(self, dict_val, inplace=True):
-        """
-        Use "from_dict" class method to create a new DataFrameXS from the dict-like object in argument dict_val, and
-        then concatenate it to the current DataFrameXS. If inplace is True, this methods returns nothing and modify the
-        current DataFrameXS, otherwise it returns a new dataframe obtained by concatenation
-
-        :param dict_val: dictionary like object, used to create a new df that will be concatenated to self.
-        :param inplace: optional, boolean, default True. If true, current df is modified, otherwise returns a new df.
-
-        :return: if inplace is True, returns None, else returns a DataFrameXS
-        """
-        # creates a DataFrame from the inputs
-        df = DataFrameXS.from_dict(dict_val)
-
-        # concat method takes care of modifying and returning what's needed.
-        return self.concat(df, inplace=inplace)
-
-    def get_as_pandas_dataframe(self):
-        """
-        Copy the dataframe content into a panda DataFrame, which is returned
-        :return: Pandas DataFrame
-        """
-        pd_df = pd.DataFrame()
-        for name in self.dict_colname_to_index:
-            pd_df[name] = np.copy(self[name])
-        return pd_df
-
-    def to_csv(self, path, sep=';', **kwargs):
-        """
-        Save the DataFrame content into a CSV.
-
-        WARNING: as a 'quick and dirty solution', this method calls 'get_as_pandas_dataframe' and then use pandas
-        'to_csv' method. This is obviously inefficient, therefore this method should not be called regularly in a sim.
-        """
-        df = self.get_as_pandas_dataframe()
-        df.to_csv(path, sep=sep, index=False, **kwargs)
+import numpy as np
+import copy
+from .jit_compiled_functions import dataframe_xs_check_arr_in_col, dataframe_xs_check_arr_in_col_conditional
+import pandas as pd
+
+
+class DataFrameXS:
+    """
+    Class that encodes a really simplified version of a dataframe, where each column is stored as a separated one
+    dimensional numpy array. Note that this class is made to be more rigid than Pandas Dataframe: the class won't try
+    to fill in blanks or fancy things like that. The idea being to maintain control on what is going on and avoid bugs
+    that go unnoticed.
+
+    Indexing:
+    ---------
+    3 types of indexing are supported: indexing by a string, an array of bool or an array of int. Any other index will
+    raise a TypeError.
+        - Indexing by a string returns the corresponding column. Keep in mind that it is not a copy, and modifying it
+          will change the original column.
+        - Indexing by an array of bool returns a copy.
+        - Indexing by an array of int returns a copy.
+    """
+    LIST_ALLOWED_TYPE = ['bool', 'uint8', 'int8', 'uint16', 'int16', 'uint32', 'int32',
+                         'uint64', 'int64', 'float32', 'float64']
+    ALLOWED_TYPE = set(LIST_ALLOWED_TYPE)
+
+    def __init__(self):
+        self.list_col = []
+        self.list_col_name = []
+        self.dict_colname_to_index = dict()
+        self.nb_rows = 0
+        self.nb_cols = 0
+
+# ----------------------------------------------------------------------------------------------------------------------
+# class methods
+
+    @classmethod
+    def from_lists(cls, list_col_name, list_col):
+        """
+        Returns a DataFrameXS from a list of column names and a list of columns. If the lists are of different length,
+        or if some column names are repeated, an Exception will be raised.
+
+        :param list_col_name: list of strings
+        :param list_col: list of 1D numpy array, that will become columns of the dataframe.
+
+        :return: DataFrameXS object.
+        """
+        if len(list_col) != len(list_col_name):
+            raise ValueError("Inputs do not have the same length.")
+        if len(list_col_name) > len(set(list_col_name)):
+            raise ValueError("Several columns have the same name.")
+
+        r_df = cls()
+        for name, col in zip(list_col_name, list_col):
+            r_df[name] = col
+        return r_df
+
+    @classmethod
+    def from_dict(cls, dict_name_to_col):
+        """
+        Returns a DataFrameXS object from a dictionary whose keys are column names, and values are columns.
+
+        :param dict_name_to_col: dictionary, whose key are strings and values 1D numpy arrays or None.
+
+        :return: DataFrameXS object
+        """
+        r_df = cls()
+        for name, col in dict_name_to_col.items():
+            r_df[name] = col
+        return r_df
+
+    @classmethod
+    def read_csv(cls, path, sep=';', **kwargs):
+        """
+        Use pandas to read a csv, and then converts the pandas Dataframe into a DataFrameXS. Be careful that the type
+        of the columns are supported by DataFrameXS instances.
+
+        :param path: string, path to the csv
+        :param sep: optional, string, default ';'. Separator in the csv.
+
+        :return: DataFrameXS object
+        """
+        df = cls()
+        pd_df = pd.read_csv(path, sep=sep, **kwargs)
+        for name in pd_df:
+            df[name] = np.copy(np.array(pd_df[name]))
+        return df
+
+# ----------------------------------------------------------------------------------------------------------------------
+# __methods__
+
+    def __setitem__(self, key, value):
+        """
+        Allow the user to set a column values by using the syntax df[key] = value
+
+        :param key: string, name of the column
+        :param value: either a single value, in which case all the column will be set to this value, or an iterable that
+                      can be casted to a numpy array of supported type. If the Value is None, then the column
+                      is set empty.
+        """
+        # check if the user provided a string as a column name
+        if not isinstance(key, str):
+            raise ValueError("A column name should be a string in a dataframe_xs.")
+
+        # in case a column is set empty
+        if value is None:
+            self._add_empty_col(key)
+        else:
+            # cast the input as a numpy array
+            temp_value = np.array(value)
+
+            # check if the input is of allowed type
+            if str(temp_value.dtype) not in self.ALLOWED_TYPE:
+                raise ValueError("The proposed column is of an unsupported type. Supported types are " +
+                                 str(self.LIST_ALLOWED_TYPE))
+
+            # check if the user provided a single value
+            if len(temp_value.shape) == 0:
+                if self.nb_rows == 0:
+                    self._add_empty_col(key)
+                else:
+                    value = np.full((self.nb_rows,), value)
+                    self._add_col_without_nb_rows_check(key, value)
+
+            # if the user provided an input that results in an array of shape (0,)
+            elif temp_value.shape == (0,):
+                self._add_empty_col(key)
+
+            # Now the case of a real serie of values
+            else:
+                value = temp_value
+                # check that the the input is of dimension 1
+                if len(value.shape) > 1:
+                    raise ValueError("A column should be an array of dimension 1, and your input dim is " +
+                                     str(value.shape) + '.')
+
+                # in the case the dataframe is empty
+                if self.nb_rows == 0:
+                    self.nb_rows = value.shape[0]
+                    self._add_col_without_nb_rows_check(key, value)
+                else:
+                    if value.shape[0] != self.nb_rows:
+                        raise ValueError("Dataframe has " + str(self.nb_rows) + " rows while the input has " +
+                                         str(value.shape[0]) + '.')
+                    else:
+                        self._add_col_without_nb_rows_check(key, value)
+
+    def __getitem__(self, item):
+        """
+        Use the syntax df[item] to retrieve data. Three possible uses:
+            1) item is the name of a column: retrieve the corresponding column. Keep in mind that this is not a copy,
+               and modifying the obtained array will modify the column in the dataframe.
+            2) item is an array of bool of same length as the dataframe: retrieve a copy of the dataframe with only the
+               lines of position i such that item[i] == True.
+            3) item is an array of int: retrieve a copy of the dataframe
+
+        :param item: either a string, a 1D array of bool, or a 1D array of int.
+
+        :return: a column of the DataFrameXS if item is a string, a DataFrameXS object otherwise.
+        """
+        # if a string is provided, return the column as np.array
+        if isinstance(item, str):
+            if item not in self.dict_colname_to_index:
+                raise KeyError("No column named " + item + ".")
+            else:
+                return self.list_col[self.dict_colname_to_index[item]]
+
+        # if an array is provided
+        elif isinstance(item, np.ndarray):
+            # check if the array is empty
+            if len(item.shape) == 0 or item.shape == (0,):
+                raise IndexError("Cannot index using an empty array")
+
+            # check if the array is not of dim 1
+            if len(item.shape) != 1:
+                raise IndexError("Boolean array indexing requires the array of boolean indexes to be one dimensional.")
+
+            # case of an array of bool
+            elif str(item.dtype) == 'bool':
+                if item.shape[0] != self.nb_rows:
+                    raise IndexError("Boolean array indexing requires the array of boolean indexes to be of the same" +
+                                     "length as the dataframe.")
+                nb_rows = item.sum()
+                if nb_rows == 0:
+                    r_df = DataFrameXS()
+                    for name in self.list_col_name:
+                        r_df[name] = None
+                    return r_df
+                else:
+                    new_cols = []
+                    for col in self.list_col:
+                        if col is None:
+                            new_cols.append(None)
+                        else:
+                            new_cols.append(col[item])
+                    return self._create_df_without_check(self.list_col_name, new_cols, nb_rows, self.nb_cols)
+
+            # case of an array of int
+            elif str(item.dtype).startswith('int'):
+                new_cols = []
+                for name, col in zip(self.list_col_name, self.list_col):
+                    if col is None:
+                        new_cols.append(None)
+                    else:
+                        new_cols.append(col[item])
+                return self._create_df_without_check(self.list_col_name, new_cols, item.shape[0], self.nb_cols)
+            else:
+                raise TypeError("Indexing with an array is only allowed using Bool or Int arrays.")
+        else:
+            raise TypeError("A Dataframe XS only supports integer, array of int and array of bool indexing.")
+
+# ----------------------------------------------------------------------------------------------------------------------
+# private methods
+
+    def _add_empty_col(self, key):
+        if key in self.dict_colname_to_index:
+            self.list_col[self.dict_colname_to_index[key]] = None
+            if self.is_empty:
+                self.nb_rows = 0
+        else:
+            self.dict_colname_to_index[key] = self.nb_cols
+            self.nb_cols += 1
+            self.list_col_name.append(key)
+            self.list_col.append(None)
+
+    def _add_col_without_nb_rows_check(self, key, value):
+        if key in self.dict_colname_to_index:
+            self.list_col[self.dict_colname_to_index[key]] = value
+        else:
+            self.dict_colname_to_index[key] = self.nb_cols
+            self.nb_cols += 1
+            self.list_col_name.append(key)
+            self.list_col.append(value)
+
+    @classmethod
+    def _create_df_without_check(cls, list_col_name, list_col, nb_rows, nb_cols):
+        r_df = cls()
+        r_df.list_col_name = copy.deepcopy(list_col_name)
+        r_df.list_col = list_col
+        r_df.nb_rows = nb_rows
+        r_df.nb_cols = nb_cols
+        r_df.dict_colname_to_index = {name: index for index, name in enumerate(list_col_name)}
+        return r_df
+
+# ----------------------------------------------------------------------------------------------------------------------
+# properties
+
+    @property
+    def is_empty(self):
+        for value in self.list_col:
+            if value is not None:
+                return False
+        return True
+
+    @property
+    def shape(self):
+        return self.nb_rows, self.nb_cols
+
+# ----------------------------------------------------------------------------------------------------------------------
+# methods
+
+    def _sampy_debug_scramble(self, permutation=None, return_permutation=False):
+        if permutation is not None:
+            if not isinstance(permutation, np.ndarray):
+                raise TypeError("Permutation parameter should be an array.")
+            if not str(permutation.dtype).startswith('int'):
+                raise TypeError("Permutation parameter should be an array of integers.")
+            if not permutation.shape == (self.nb_rows,):
+                raise ValueError("Permutation parameter should be an array of integers of shape (nb_rows,).")
+            if not (np.sort(permutation) == np.arange(0, self.nb_rows)).all():
+                raise ValueError("Permutation parameter should be a permutation of the integers from 0 to nb_rows.")
+
+    def scramble(self, permutation=None, return_permutation=False):
+        """
+        Scramble the rows of the dataframe XS. The user can provide a permutation that will be used to scramble the
+        rows.
+
+        WARNING: if you use the keyword argument permutation, be sure you provide a permutation of the correct size.
+        Otherwise the result can be unpredictable.
+
+        :param permutation: optional, array of int, default None.
+        :param return_permutation: optional, boolean default False. If True, the function returns the permutation used
+                                   to shuffle the DataFrameXS (useful if some other objects have to be shuffled).
+        """
+        if permutation is None:
+            permutation = np.random.permutation(self.nb_rows)
+        for i, col in enumerate(self.list_col):
+            if col is not None:
+                self.list_col[i] = col[permutation]
+
+        if return_permutation:
+            return permutation
+
+    def _sampy_debug_get_copy(self, col_name):
+        if not isinstance(col_name, str):
+            raise TypeError("get_copy expects a string as argument.")
+        else:
+            if col_name not in self.dict_colname_to_index:
+                raise KeyError("no column with the name " + col_name + " in the dataframe.")
+
+    def get_copy(self, col_name):
+        """
+        Returns a copy of the selected column.
+        :param col_name: string, name of the column to copy.
+        """
+        col = self.list_col[self.dict_colname_to_index[col_name]]
+        if col is None:
+            return
+        else:
+            return np.copy(col)
+        
+    def drop_column(self, col_name):
+        """
+        Delete a column from the DataFrame.
+
+        :param col_name: string, name of the column to delete.
+        """
+        if not col_name in self.dict_colname_to_index:
+            raise ValueError(col_name + " is not the name of a column of the DataFrame.")
+        
+        # get the index of the column
+        index_column = self.dict_colname_to_index[col_name]
+
+        _ = self.list_col.pop(index_column)
+        self.list_col_name.remove(col_name)
+        del self.dict_colname_to_index[col_name]
+
+        # the indexes of the column appearing at the right of the deleted column should be shifted by 1
+        for name in self.dict_colname_to_index:
+            if self.dict_colname_to_index[name] >= index_column:
+                self.dict_colname_to_index[name] -= 1
+
+        self.nb_cols -= 1
+        if self.is_empty:
+            self.nb_rows = 0
+        
+
+    def _sampy_debug_check_arr_in_col(self, input_arr, name_col, condition=None):
+        if condition is not None:
+            if not isinstance(condition, np.ndarray):
+                raise ValueError("condition should be an array.")
+            if str(condition.dtype) != 'bool':
+                raise ValueError("condition should be an array of bool.")
+            if input_arr.shape != condition.shape:
+                raise ValueError("condition and input_arr don't have the same shape.")
+
+        if not isinstance(input_arr, np.ndarray):
+            raise ValueError('Input array is not a numpy ndarray.')
+        if len(input_arr.shape) != 1:
+            raise ValueError('Input array is not one dimensional.')
+        if input_arr.shape[0] == 0:
+            raise ValueError('Input array is empty.')
+        if str(input_arr.dtype) != str(self[name_col].dtype):
+            raise ValueError("The input array (" + str(input_arr.dtype) + ") is not of the same type as the " +
+                             "selected column (" + str(self[name_col].dtype) + ").")
+
+    def check_arr_in_col(self, input_arr, name_col, condition=None):
+        """
+        Check which elements of the input array are in selected column.
+
+        :param input_arr: 1D numpy array.
+        :param name_col: string, name of the column
+        :param condition: optional, boolean array.
+
+        :return: 1D boolean array saying which elements of the input array are in the selected column.
+        """
+        if condition is None:
+            return dataframe_xs_check_arr_in_col(input_arr, self[name_col])
+        else:
+            return dataframe_xs_check_arr_in_col_conditional(input_arr, self[name_col], condition)
+
+    def _sampy_debug_change_type(self, col_name, str_type):
+        if not isinstance(str_type, str):
+            raise ValueError("str_type should be a string in the list: " + str(self.LIST_ALLOWED_TYPE) + ".")
+        if str_type not in self.ALLOWED_TYPE:
+            raise ValueError("The type " + str_type + "is not in " + str(self.LIST_ALLOWED_TYPE) + ".")
+
+    def change_type(self, col_name, str_type):
+        """
+        Change the type of a column. The selected type has to be in the allowed type list.
+        Do nothing if the selected column is empty.
+
+        :param col_name: string, name of the column whose type should be changed.
+        :param type: string, numpy identifier of the new type of the column.
+        """
+        if self[col_name] is not None:
+            self[col_name] = self[col_name].astype(str_type)
+
+    def copy(self):
+        """
+        Returns a copy of the dataframe
+        :return: a dataframeXS
+        """
+        new_list_col = []
+        for col in self.list_col:
+            new_list_col.append(np.copy(col))
+        return self._create_df_without_check(self.list_col_name, new_list_col, self.nb_rows, self.nb_cols)
+
+    def concat(self, df, inplace=True, dict_default_values=None):
+        """
+        Append the input DataFrameXS to the current DataFrameXS. The column names of the current DataFrameXS have to be
+        column names of the input, or an Exception will be raised. Finally, note that the types of the columns of the
+        input will be casted to the types of the corresponding columns of the current DataFrameXS.
+
+        Extra columns in the input are ignored.
+
+        WARNING: if one column of one of the dataframes involved exists but is empty while the same column in the 
+                 other is not, this method tries to fill the missing values with np.NaN and then convert the obtained 
+                 column into the correct dtype. This results in unexpected behaviour when the column is supposed to be
+                 of type bool. Therefore, we recommand the user to provide default values to be used instead of NaN 
+                 using the kwarg 'dict_default_values'. 
+
+        :param df: DataFrame XS
+        :param inplace: optional, boolean, default True. If True, the input is appended to the current DataFrame.
+                        Otherwise, a new DataFrameXS is returned.
+        :param dict_default_values: optional, dictionary, default None. Dictionary of the form {name_col: default val, ...}.
+                                    Provides default values to be used if a column of one of the DF is empty while the same
+                                    column in the other is not.
+
+        :return: if inplace is False, return a DataFrameXS, otherwise returns None.
+        """
+        if not isinstance(df, DataFrameXS):
+            raise ValueError("Input is not a DataframeXS")
+
+        # case where the current DataFrameXS is empty, which can happen when initializing a simulation
+        if self.is_empty:
+
+            # if input is empty, the case is clear
+            if df.is_empty:
+                if inplace:
+                    return
+                else:
+                    return self.copy()
+
+            # if df is not empty, fill self columns with df columns
+            else:
+                new_col = []
+                for name in self.list_col_name:
+                    col = df[name]
+                    if col is None:
+                        new_col.append(None)
+                    else:
+                        new_col.append(np.copy(col))
+                if inplace:
+                    self.list_col = new_col
+                    self.nb_rows = df.nb_rows
+                else:
+                    return self._create_df_without_check(self.list_col_name, new_col, df.nb_rows, self.nb_cols)
+
+        # when both dataframes are not empty. Most important checks are done by __getitem__
+        elif not df.is_empty:
+            new_col = []
+            for name in self.list_col_name:
+                df_col = df[name]
+                self_col = self[name]
+                if self_col is not None:
+                    if df_col is not None:
+                        new_col.append(np.hstack([self_col, df_col]).astype(self_col.dtype))
+                    else:
+                        if dict_default_values is not None and name in dict_default_values:
+                            filled_col = np.full((df.nb_rows,), dict_default_values[name]).astype(self_col.dtype)
+                        else:
+                            filled_col = np.full((df.nb_rows,), np.nan).astype(self_col.dtype)
+                        new_col.append(np.hstack([self_col, filled_col]).astype(self_col.dtype))
+                else:
+                    if df_col is not None:
+                        if dict_default_values is not None and name in dict_default_values:
+                            filled_col = np.full((self.nb_rows,), dict_default_values[name]).astype(df_col.dtype)
+                        else:
+                            filled_col = np.full((self.nb_rows,), np.nan).astype(df_col.dtype)
+                        new_col.append(np.hstack([filled_col, df_col]).astype(df_col.dtype))
+                    else:
+                        new_col.append(None)
+            if inplace:
+                self.nb_rows += df.nb_rows
+                self.list_col = new_col
+            else:
+                return self._create_df_without_check(self.list_col_name, new_col, self.nb_rows + df.nb_rows,
+                                                     self.nb_cols)
+
+        # when current is not empty, and input is. No checks are done in this case.
+        else:
+            if inplace:
+                return
+            else:
+                return self.copy()
+
+    def add_rows_from_dict(self, dict_val, inplace=True):
+        """
+        Use "from_dict" class method to create a new DataFrameXS from the dict-like object in argument dict_val, and
+        then concatenate it to the current DataFrameXS. If inplace is True, this methods returns nothing and modify the
+        current DataFrameXS, otherwise it returns a new dataframe obtained by concatenation
+
+        :param dict_val: dictionary like object, used to create a new df that will be concatenated to self.
+        :param inplace: optional, boolean, default True. If true, current df is modified, otherwise returns a new df.
+
+        :return: if inplace is True, returns None, else returns a DataFrameXS
+        """
+        # creates a DataFrame from the inputs
+        df = DataFrameXS.from_dict(dict_val)
+
+        # concat method takes care of modifying and returning what's needed.
+        return self.concat(df, inplace=inplace)
+
+    def get_as_pandas_dataframe(self):
+        """
+        Copy the dataframe content into a panda DataFrame, which is returned
+        :return: Pandas DataFrame
+        """
+        pd_df = pd.DataFrame()
+        for name in self.dict_colname_to_index:
+            pd_df[name] = np.copy(self[name])
+        return pd_df
+
+    def to_csv(self, path, sep=';', **kwargs):
+        """
+        Save the DataFrame content into a CSV.
+
+        WARNING: as a 'quick and dirty solution', this method calls 'get_as_pandas_dataframe' and then use pandas
+        'to_csv' method. This is obviously inefficient, therefore this method should not be called regularly in a sim.
+        """
+        df = self.get_as_pandas_dataframe()
+        df.to_csv(path, sep=sep, index=False, **kwargs)
```

### Comparing `sampy-abm-1.0.2/src/sampy/spatial/proximity_3d.py` & `sampy_abm-1.0.3/src/sampy/spatial/proximity_3d.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,243 +1,281 @@
-import numpy as np
-
-from scipy.spatial import cKDTree
-# from netCDF4 import Dataset
-
-from .jit_compiled_functions import (conditional_proximity_is_step_allowed_return_infos,
-                                     proximity_is_step_allowed_return_infos,
-                                     conditional_proximity_is_pos_allowed,
-                                     proximity_is_pos_allowed)
-
-
-class BaseProximity3dFromArrays:
-    """
-    Base class for constructing 3d-proximity object from raw one dimensional arrays.
-
-    :param arr_radius_point: 1d array of float, giving the "radius" around each point of the proximity object.
-    :param coord_x: 1d array of floats, x coordinates of points
-    :param coord_y: 1d array of floats, y coordinates of points
-    :param coord_z: 1d array of floats, z coordinates of points
-    :param allowed_points: optional, 1D array of bool, default None.
-    """
-    def __init__(self, arr_radius_point=None, coord_x=None, coord_y=None, coord_z=None, allowed_points=None, **kwargs):
-        if arr_radius_point is None:
-            raise ValueError("No value for arr_radius_point kwarg has been given.")
-        if coord_x is None:
-            raise ValueError("No value for coord_x kwarg has been given.")
-        if coord_y is None:
-            raise ValueError("No value for coord_y kwarg has been given.")
-        if coord_z is None:
-            raise ValueError("No value for coord_z kwarg has been given.")
-
-        stacked_arr = np.column_stack([coord_x, coord_y, coord_z])
-        try:
-            radius = float(arr_radius_point)
-            self.arr_radius_point = np.full(coord_x.shape, radius)
-        except TypeError:
-            self.arr_radius_point = np.copy(arr_radius_point)
-
-        self.coord_x = np.copy(coord_x)
-        self.coord_y = np.copy(coord_y)
-        self.coord_z = np.copy(coord_z)
-        self.kdtree = cKDTree(stacked_arr)
-
-        self.allowed_points = allowed_points
-
-    def update_allowed_points(self, arr_new_allowed_point):
-        """
-        Update the array of allowed points.
-
-        :param arr_new_allowed_point: 1D array of bool, telling which point is allowed.
-        """
-        self.allowed_points = arr_new_allowed_point
-
-
-class BaseProximity3dFromLatLonGrid:
-    """
-    Base class for constructing 3d-proximity object from two 2d grids of lattitude and longitude.
-
-    :param grid_lats: 2D array of float, latitudes of the points.
-    :param grid_lons: 2D array of float, longitude of the points.
-    :param radius: float, radius of the sphere on which the points live
-    :param arr_radius_point: 1d array of float, giving the "radius" around each point of the proximity object.
-    :param allowed_points: optional, 2D array of bool, default None.
-    """
-    def __init__(self, grid_lats=None, grid_lons=None, radius=None, arr_radius_point=None, allowed_points=None,
-                 **kwargs):
-        if grid_lats is None:
-            raise ValueError("No value for grid_lats kwarg has been given.")
-        if grid_lons is None:
-            raise ValueError("No value for grid_lons kwarg has been given.")
-        if radius is None:
-            raise ValueError("No value for radius kwarg has been given.")
-
-        # start creating the proximity 3d thingy
-        grid_coord_x = radius * np.cos(np.radians(grid_lats)) * np.cos(np.radians(grid_lons))
-        grid_coord_y = radius * np.cos(np.radians(grid_lats)) * np.sin(np.radians(grid_lons))
-        grid_coord_z = radius * np.sin(np.radians(grid_lats))
-
-        if arr_radius_point is None:
-            arr_radius_point = np.full(grid_lats.shape, -1.)
-            for i in range(grid_lats.shape[0]):
-                for j in range(grid_lats.shape[1]):
-                    current_max_dist = 0.
-                    if i - 1 >= 0:
-                        d = (grid_coord_x[i - 1, j] - grid_coord_x[i, j]) ** 2 + \
-                            (grid_coord_y[i - 1, j] - grid_coord_y[i, j]) ** 2 + \
-                            (grid_coord_z[i - 1, j] - grid_coord_z[i, j]) ** 2
-                        d = np.sqrt(d)
-                        if d > current_max_dist:
-                            current_max_dist = d
-                    if j - 1 >= 0:
-                        d = (grid_coord_x[i, j - 1] - grid_coord_x[i, j]) ** 2 + \
-                            (grid_coord_y[i, j - 1] - grid_coord_y[i, j]) ** 2 + \
-                            (grid_coord_z[i, j - 1] - grid_coord_z[i, j]) ** 2
-                        d = np.sqrt(d)
-                        if d > current_max_dist:
-                            current_max_dist = d
-                    try:
-                        d = (grid_coord_x[i, j + 1] - grid_coord_x[i, j]) ** 2 + \
-                            (grid_coord_y[i, j + 1] - grid_coord_y[i, j]) ** 2 + \
-                            (grid_coord_z[i, j + 1] - grid_coord_z[i, j]) ** 2
-                        d = np.sqrt(d)
-                        if d > current_max_dist:
-                            current_max_dist = d
-                    except IndexError:
-                        pass
-                    try:
-                        d = (grid_coord_x[i + 1, j] - grid_coord_x[i, j]) ** 2 + \
-                            (grid_coord_y[i + 1, j] - grid_coord_y[i, j]) ** 2 + \
-                            (grid_coord_z[i + 1, j] - grid_coord_z[i, j]) ** 2
-                        d = np.sqrt(d)
-                        if d > current_max_dist:
-                            current_max_dist = d
-                    except IndexError:
-                        pass
-                    arr_radius_point[i, j] = current_max_dist
-
-        self.coord_x = grid_coord_x.flatten()
-        self.coord_y = grid_coord_y.flatten()
-        self.coord_z = grid_coord_z.flatten()
-        self.arr_radius_point = arr_radius_point.flatten()
-        self.kdtree = cKDTree(np.column_stack([self.coord_x, self.coord_y, self.coord_z]))
-        self.allowed_points = allowed_points
-
-    def update_allowed_points(self, arr_new_allowed_point):
-        """
-        Update the array of allowed points.
-
-        :param arr_new_allowed_point: 2D array of bool, telling which point of the grid is allowed.
-        """
-        self.allowed_points = arr_new_allowed_point.flatten()
-
-
-class Proximity3dBasicSpatialQueries:
-    def __init__(self, **kwargs):
-        pass
-
-    def get_closest_point(self, arr_target_x, arr_target_y, arr_target_z):
-        """
-        Given a series of target-point whose coordinates are given as three 1 dimensional arrays, this method gives the
-        index of the closest point (and the distance) in the proximity class to each of the target-points.
-
-        :param arr_target_x: 1d array of float, x coordinate of target point.
-        :param arr_target_y: 1d array of float, y coordinate of target point.
-        :param arr_target_z: 1d array of float, z coordinate of target point.
-
-        :return: couple of arrays (distance, indices), the second one giving the index of the closest point and the
-            first one the distance to this point
-        """
-        stacked_arr = np.column_stack([arr_target_x, arr_target_y, arr_target_z])
-        return self.kdtree.query(stacked_arr, k=1)
-
-    def is_pos_allowed(self, pos_x, pos_y, pos_z, distances=None, indices=None):
-        """
-        Given a series of position, whose coordinates are given as three 1 dimensional arrays, this method tells which
-        are allowed with respect to the current proximity class.
-
-        :param pos_x: 1d array of float, x coordinate of the positions.
-        :param pos_y: 1d array of float, y coordinate of the positions
-        :param pos_z: 1d array of float, z coordinate of the positions
-        :param distances: optional, 1d array of float, default None. If given, distances[i] should be the distance
-                          from the position i to its closest point in the proximity class.
-        :param indices: optional, 1d array of int, default None. If given, indices[i] should be the index of the point
-                        in the proximity class which is the closest to the position i.
-
-        :return: an array of bool, telling which positions are allowed.
-        """
-        if (indices is None) or (distances is None):
-            distances, indices = self.get_closest_point(pos_x, pos_y, pos_z)
-        if self.allowed_points is not None:
-            return conditional_proximity_is_pos_allowed(indices, distances, self.arr_radius_point, self.allowed_points)
-        else:
-            return proximity_is_pos_allowed(indices, distances, self.arr_radius_point)
-
-
-# class LegacyNetcdfThingy:
-#     def __init__(self, **kwargs):
-#         pass
-#
-#     @classmethod
-#     def from_netcdf(cls, path_to_netcdf, name_lats_attr, name_lons_attr, arr_radius_point=None, radius=1.):
-#         """
-#         todo
-#         :param path_to_netcdf:
-#         :param name_lats_attr:
-#         :param name_lons_attr:
-#         :param arr_radius_point:
-#         :param radius:
-#         :return:
-#         """
-#         data = Dataset(path_to_netcdf, mode='r')
-#         nf_lats = np.array(data.variables[name_lats_attr][:])
-#         nf_lons = np.array(data.variables[name_lons_attr][:])
-#         lats = nf_lats.flatten()
-#         lons = nf_lons.flatten()
-#         coord_x = radius * np.cos(np.radians(lats)) * np.cos(np.radians(lons))
-#         coord_y = radius * np.cos(np.radians(lats)) * np.sin(np.radians(lons))
-#         coord_z = radius * np.sin(np.radians(lats))
-#         if arr_radius_point is None:
-#             nf_coord_x = radius * np.cos(np.radians(nf_lats)) * np.cos(np.radians(nf_lons))
-#             nf_coord_y = radius * np.cos(np.radians(nf_lats)) * np.sin(np.radians(nf_lons))
-#             nf_coord_z = radius * np.sin(np.radians(nf_lats))
-#             arr_radius_point = np.full(nf_lats.shape, -1.)
-#             for i in range(nf_lats.shape[0]):
-#                 for j in range(nf_lats.shape[1]):
-#                     current_max_dist = 0.
-#                     if i-1 >= 0:
-#                         d = (nf_coord_x[i-1, j] - nf_coord_x[i, j])**2 + \
-#                             (nf_coord_y[i-1, j] - nf_coord_y[i, j])**2 + \
-#                             (nf_coord_z[i-1, j] - nf_coord_z[i, j]) ** 2
-#                         d = np.sqrt(d)
-#                         if d > current_max_dist:
-#                             current_max_dist = d
-#                     if j-1 >= 0:
-#                         d = (nf_coord_x[i, j-1] - nf_coord_x[i, j])**2 + \
-#                             (nf_coord_y[i, j-1] - nf_coord_y[i, j])**2 + \
-#                             (nf_coord_z[i, j-1] - nf_coord_z[i, j]) ** 2
-#                         d = np.sqrt(d)
-#                         if d > current_max_dist:
-#                             current_max_dist = d
-#                     try:
-#                         d = (nf_coord_x[i, j + 1] - nf_coord_x[i, j]) ** 2 + \
-#                             (nf_coord_y[i, j + 1] - nf_coord_y[i, j]) ** 2 + \
-#                             (nf_coord_z[i, j + 1] - nf_coord_z[i, j]) ** 2
-#                         d = np.sqrt(d)
-#                         if d > current_max_dist:
-#                             current_max_dist = d
-#                     except IndexError:
-#                         pass
-#                     try:
-#                         d = (nf_coord_x[i+1, j] - nf_coord_x[i, j]) ** 2 + \
-#                             (nf_coord_y[i+1, j] - nf_coord_y[i, j]) ** 2 + \
-#                             (nf_coord_z[i+1, j] - nf_coord_z[i, j]) ** 2
-#                         d = np.sqrt(d)
-#                         if d > current_max_dist:
-#                             current_max_dist = d
-#                     except IndexError:
-#                         pass
-#                     arr_radius_point[i, j] = current_max_dist
-#             arr_radius_point = arr_radius_point.flatten()
-#         r_cls = cls(arr_radius_point, coord_x, coord_y, coord_z)
-#         setattr(r_cls, 'netcdf', data)
-#         return r_cls
+import numpy as np
+
+from scipy.spatial import cKDTree
+
+from .jit_compiled_functions import (conditional_proximity_is_pos_allowed,
+                                     proximity_is_pos_allowed)
+
+
+class BaseProximity3dFromArrays:
+    """
+    Base class for constructing 3d-proximity object from raw one dimensional arrays.
+
+    :param arr_radius_point: 1d array of float, giving the "radius" around each point of the proximity object.
+    :param coord_x: 1d array of floats, x coordinates of points
+    :param coord_y: 1d array of floats, y coordinates of points
+    :param coord_z: 1d array of floats, z coordinates of points
+    :param allowed_points: optional, 1D array of bool, default None.
+    """
+    def __init__(self, arr_radius_point=None, coord_x=None, coord_y=None, coord_z=None, allowed_points=None, **kwargs):
+        if arr_radius_point is None:
+            raise ValueError("No value for arr_radius_point kwarg has been given.")
+        if coord_x is None:
+            raise ValueError("No value for coord_x kwarg has been given.")
+        if coord_y is None:
+            raise ValueError("No value for coord_y kwarg has been given.")
+        if coord_z is None:
+            raise ValueError("No value for coord_z kwarg has been given.")
+
+        stacked_arr = np.column_stack([coord_x, coord_y, coord_z])
+        try:
+            radius = float(arr_radius_point)
+            self.arr_radius_point = np.full(coord_x.shape, radius)
+        except TypeError:
+            self.arr_radius_point = np.copy(arr_radius_point)
+
+        self.coord_x = np.copy(coord_x)
+        self.coord_y = np.copy(coord_y)
+        self.coord_z = np.copy(coord_z)
+        self.kdtree = cKDTree(stacked_arr)
+
+        self.allowed_points = allowed_points
+
+    def update_allowed_points(self, arr_new_allowed_point):
+        """
+        Update the array of allowed points.
+
+        :param arr_new_allowed_point: 1D array of bool, telling which point is allowed.
+        """
+        self.allowed_points = arr_new_allowed_point
+
+
+class BaseProximity3dFromLatLonGrid:
+    """
+    Base class for constructing 3d-proximity object from two 2d grids of lattitude and longitude.
+
+    :param grid_lats: 2D array of float, latitudes of the points.
+    :param grid_lons: 2D array of float, longitude of the points.
+    :param sphere_radius: float, radius of the sphere on which the points live
+    :param arr_radius_point: 1d array of float, giving the "radius" around each point of the proximity object.
+    :param allowed_points: optional, 2D array of bool, default None.
+    """
+    def __init__(self, grid_lats=None, grid_lons=None, sphere_radius=None, arr_radius_point=None, allowed_points=None,
+                 **kwargs):
+        if grid_lats is None:
+            raise ValueError("No value for grid_lats kwarg has been given.")
+        if grid_lons is None:
+            raise ValueError("No value for grid_lons kwarg has been given.")
+        if sphere_radius is None:
+            raise ValueError("No value for radius kwarg has been given.")
+        
+        self.sphere_radius = sphere_radius
+
+        # start creating the proximity 3d thingy
+        grid_coord_x = sphere_radius * np.cos(np.radians(grid_lats)) * np.cos(np.radians(grid_lons))
+        grid_coord_y = sphere_radius * np.cos(np.radians(grid_lats)) * np.sin(np.radians(grid_lons))
+        grid_coord_z = sphere_radius * np.sin(np.radians(grid_lats))
+
+        if arr_radius_point is None:
+            arr_radius_point = np.full(grid_lats.shape, -1.)
+            for i in range(grid_lats.shape[0]):
+                for j in range(grid_lats.shape[1]):
+                    current_max_dist = 0.
+                    if i - 1 >= 0:
+                        d = (grid_coord_x[i - 1, j] - grid_coord_x[i, j]) ** 2 + \
+                            (grid_coord_y[i - 1, j] - grid_coord_y[i, j]) ** 2 + \
+                            (grid_coord_z[i - 1, j] - grid_coord_z[i, j]) ** 2
+                        d = np.sqrt(d)
+                        if d > current_max_dist:
+                            current_max_dist = d
+                    if j - 1 >= 0:
+                        d = (grid_coord_x[i, j - 1] - grid_coord_x[i, j]) ** 2 + \
+                            (grid_coord_y[i, j - 1] - grid_coord_y[i, j]) ** 2 + \
+                            (grid_coord_z[i, j - 1] - grid_coord_z[i, j]) ** 2
+                        d = np.sqrt(d)
+                        if d > current_max_dist:
+                            current_max_dist = d
+                    try:
+                        d = (grid_coord_x[i, j + 1] - grid_coord_x[i, j]) ** 2 + \
+                            (grid_coord_y[i, j + 1] - grid_coord_y[i, j]) ** 2 + \
+                            (grid_coord_z[i, j + 1] - grid_coord_z[i, j]) ** 2
+                        d = np.sqrt(d)
+                        if d > current_max_dist:
+                            current_max_dist = d
+                    except IndexError:
+                        pass
+                    try:
+                        d = (grid_coord_x[i + 1, j] - grid_coord_x[i, j]) ** 2 + \
+                            (grid_coord_y[i + 1, j] - grid_coord_y[i, j]) ** 2 + \
+                            (grid_coord_z[i + 1, j] - grid_coord_z[i, j]) ** 2
+                        d = np.sqrt(d)
+                        if d > current_max_dist:
+                            current_max_dist = d
+                    except IndexError:
+                        pass
+                    arr_radius_point[i, j] = current_max_dist
+
+        self.coord_x = grid_coord_x.flatten()
+        self.coord_y = grid_coord_y.flatten()
+        self.coord_z = grid_coord_z.flatten()
+        self.arr_radius_point = arr_radius_point.flatten()
+        self.kdtree = cKDTree(np.column_stack([self.coord_x, self.coord_y, self.coord_z]))
+        self.allowed_points = allowed_points
+
+    def update_allowed_points(self, arr_new_allowed_point):
+        """
+        Update the array of allowed points.
+
+        :param arr_new_allowed_point: 2D array of bool, telling which point of the grid is allowed.
+        """
+        self.allowed_points = arr_new_allowed_point.flatten()
+
+
+class BaseProximity3dFromGraph:
+    """
+    Base class for constructing 3d-proximity object from a graph. The graph is assumed to have its vertices
+    3D coordinates stored as attributes, as well as their radiuses. 
+
+    :param graph: mandatory kwarg, graph object.
+    :param radius_attribute: optional, string, default 'radius_each_cell'
+    :param coord_x_attribute: optional, string, default 'coord_x'
+    :param coord_y_attribute: optional, string, default 'coord_y'
+    :param coord_z_attribute: optional, string, default 'coord_z'
+    :param allowed_points: optional, 1D array of bool, default None.
+    """
+    def __init__(self, graph=None, radius_attribute='radius_each_cell', coord_x_attribute='coord_x', 
+                 coord_y_attribute='coord_y', coord_z_attribute='coord_z', allowed_points=None, **kwargs):
+        
+        if graph is None:
+            raise ValueError('Mandatory kwarg graph not provided for Proximity3D class from graph.')
+
+        self.arr_radius_point = np.copy(graph.df_attributes[radius_attribute])
+
+        self.coord_x = np.copy(graph.df_attributes[coord_x_attribute])
+        self.coord_y = np.copy(graph.df_attributes[coord_y_attribute])
+        self.coord_z = np.copy(graph.df_attributes[coord_z_attribute])
+
+        stacked_arr = np.column_stack([self.coord_x, self.coord_y, self.coord_z])
+        self.kdtree = cKDTree(stacked_arr)
+
+        self.allowed_points = allowed_points
+
+    def update_allowed_points(self, arr_new_allowed_point):
+        """
+        Update the array of allowed points.
+
+        :param arr_new_allowed_point: 1D array of bool, telling which point is allowed.
+        """
+        self.allowed_points = arr_new_allowed_point
+
+
+class Proximity3dBasicSpatialQueries:
+    def __init__(self, **kwargs):
+        pass
+
+    def get_closest_point(self, arr_target_x, arr_target_y, arr_target_z, nb_points=1):
+        """
+        Given a series of target-point whose coordinates are given as three 1 dimensional arrays, this method gives the
+        index of the closest point(s) (and the distance(s)) in the proximity class to each of the target-points.
+
+        :param arr_target_x: 1d array of float, x coordinate of target point.
+        :param arr_target_y: 1d array of float, y coordinate of target point.
+        :param arr_target_z: 1d array of float, z coordinate of target point.
+        :param nb_points: optional, integer, default 1. Number of point to retrieve for each target.
+
+        :return: couple of arrays (distance, indices), the second one giving the index of the closest point and the
+            first one the distance to this point
+        """
+        stacked_arr = np.column_stack([arr_target_x, arr_target_y, arr_target_z])
+        return self.kdtree.query(stacked_arr, k=nb_points)
+
+    def is_pos_allowed(self, pos_x, pos_y, pos_z, distances=None, indices=None):
+        """
+        Given a series of position, whose coordinates are given as three 1 dimensional arrays, this method tells which
+        are allowed with respect to the current proximity class.
+
+        :param pos_x: 1d array of float, x coordinate of the positions.
+        :param pos_y: 1d array of float, y coordinate of the positions
+        :param pos_z: 1d array of float, z coordinate of the positions
+        :param distances: optional, 1d array of float, default None. If given, distances[i] should be the distance
+                          from the position i to its closest point in the proximity class.
+        :param indices: optional, 1d array of int, default None. If given, indices[i] should be the index of the point
+                        in the proximity class which is the closest to the position i.
+
+        :return: an array of bool, telling which positions are allowed.
+        """
+        if (indices is None) or (distances is None):
+            distances, indices = self.get_closest_point(pos_x, pos_y, pos_z)
+        if self.allowed_points is not None:
+            return conditional_proximity_is_pos_allowed(indices, distances, self.arr_radius_point, self.allowed_points)
+        else:
+            return proximity_is_pos_allowed(indices, distances, self.arr_radius_point)
+
+
+# class LegacyNetcdfThingy:
+#     def __init__(self, **kwargs):
+#         pass
+#
+#     @classmethod
+#     def from_netcdf(cls, path_to_netcdf, name_lats_attr, name_lons_attr, arr_radius_point=None, radius=1.):
+#         """
+#         todo
+#         :param path_to_netcdf:
+#         :param name_lats_attr:
+#         :param name_lons_attr:
+#         :param arr_radius_point:
+#         :param radius:
+#         :return:
+#         """
+#         data = Dataset(path_to_netcdf, mode='r')
+#         nf_lats = np.array(data.variables[name_lats_attr][:])
+#         nf_lons = np.array(data.variables[name_lons_attr][:])
+#         lats = nf_lats.flatten()
+#         lons = nf_lons.flatten()
+#         coord_x = radius * np.cos(np.radians(lats)) * np.cos(np.radians(lons))
+#         coord_y = radius * np.cos(np.radians(lats)) * np.sin(np.radians(lons))
+#         coord_z = radius * np.sin(np.radians(lats))
+#         if arr_radius_point is None:
+#             nf_coord_x = radius * np.cos(np.radians(nf_lats)) * np.cos(np.radians(nf_lons))
+#             nf_coord_y = radius * np.cos(np.radians(nf_lats)) * np.sin(np.radians(nf_lons))
+#             nf_coord_z = radius * np.sin(np.radians(nf_lats))
+#             arr_radius_point = np.full(nf_lats.shape, -1.)
+#             for i in range(nf_lats.shape[0]):
+#                 for j in range(nf_lats.shape[1]):
+#                     current_max_dist = 0.
+#                     if i-1 >= 0:
+#                         d = (nf_coord_x[i-1, j] - nf_coord_x[i, j])**2 + \
+#                             (nf_coord_y[i-1, j] - nf_coord_y[i, j])**2 + \
+#                             (nf_coord_z[i-1, j] - nf_coord_z[i, j]) ** 2
+#                         d = np.sqrt(d)
+#                         if d > current_max_dist:
+#                             current_max_dist = d
+#                     if j-1 >= 0:
+#                         d = (nf_coord_x[i, j-1] - nf_coord_x[i, j])**2 + \
+#                             (nf_coord_y[i, j-1] - nf_coord_y[i, j])**2 + \
+#                             (nf_coord_z[i, j-1] - nf_coord_z[i, j]) ** 2
+#                         d = np.sqrt(d)
+#                         if d > current_max_dist:
+#                             current_max_dist = d
+#                     try:
+#                         d = (nf_coord_x[i, j + 1] - nf_coord_x[i, j]) ** 2 + \
+#                             (nf_coord_y[i, j + 1] - nf_coord_y[i, j]) ** 2 + \
+#                             (nf_coord_z[i, j + 1] - nf_coord_z[i, j]) ** 2
+#                         d = np.sqrt(d)
+#                         if d > current_max_dist:
+#                             current_max_dist = d
+#                     except IndexError:
+#                         pass
+#                     try:
+#                         d = (nf_coord_x[i+1, j] - nf_coord_x[i, j]) ** 2 + \
+#                             (nf_coord_y[i+1, j] - nf_coord_y[i, j]) ** 2 + \
+#                             (nf_coord_z[i+1, j] - nf_coord_z[i, j]) ** 2
+#                         d = np.sqrt(d)
+#                         if d > current_max_dist:
+#                             current_max_dist = d
+#                     except IndexError:
+#                         pass
+#                     arr_radius_point[i, j] = current_max_dist
+#             arr_radius_point = arr_radius_point.flatten()
+#         r_cls = cls(arr_radius_point, coord_x, coord_y, coord_z)
+#         setattr(r_cls, 'netcdf', data)
+#         return r_cls
```

### Comparing `sampy-abm-1.0.2/src/sampy/utils/decorators.py` & `sampy_abm-1.0.3/src/sampy/utils/decorators.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-from functools import wraps
-
-
-def sampy_class(cls):
-    """
-    A sampy class is obtained by composition of multiple building blocks using multiple inheritance. This decorator
-    removes the need for the user to deal with MRO himself, as well as calling the parents classes while defining new
-    sampy classes.
-
-    :param cls: class decorated.
-
-    :return: class with a modified init function.
-    """
-    def modify_init(init):
-
-        def sampy_init(self, **kwargs):
-
-            # call the init of all the inherited classes.
-            ordered_init_call = []
-            for i, sub_cls in enumerate(type(self).mro()):
-                if i == 0:
-                    continue
-                if sub_cls.__name__.startswith('Base'):
-                    ordered_init_call.append(sub_cls)
-            for i, sub_cls in enumerate(type(self).mro()):
-                if i == 0:
-                    continue
-                if not sub_cls.__name__.startswith('Base'):
-                    ordered_init_call.append(sub_cls)
-
-            for i, sub_cls in enumerate(ordered_init_call):
-                if sub_cls.__name__ == 'object':
-                    sub_cls.__init__(self)
-                else:
-                    sub_cls.__init__(self, **kwargs)
-
-            init(self, **kwargs)
-
-        return sampy_init
-
-    setattr(cls, '__init__', modify_init(cls.__init__))
-
-    return cls
-
-
-def debug_method(method):
-    @wraps(method)
-    def returned_function(self, *args, **kwargs):
-        # print(args, kwargs)
-        if hasattr(self, '_sampy_debug_' + method.__name__):
-            getattr(self, '_sampy_debug_' + method.__name__)(*args, **kwargs)
-        rv = method(self, *args, **kwargs)
-        return rv
-    return returned_function
-
-
-def use_debug_mode(cls):
-    for name in dir(cls):
-        if not name.startswith('_') and hasattr(getattr(cls, name), '__call__'):
-            setattr(cls, name, debug_method(getattr(cls, name)))
+from functools import wraps
+
+
+def sampy_class(cls):
+    """
+    A sampy class is obtained by composition of multiple building blocks using multiple inheritance. This decorator
+    removes the need for the user to deal with MRO himself, as well as calling the parents classes while defining new
+    sampy classes.
+
+    :param cls: class decorated.
+
+    :return: class with a modified init function.
+    """
+    def modify_init(init):
+
+        def sampy_init(self, **kwargs):
+
+            # call the init of all the inherited classes.
+            ordered_init_call = []
+            for i, sub_cls in enumerate(type(self).mro()):
+                if i == 0:
+                    continue
+                if sub_cls.__name__.startswith('Base'):
+                    ordered_init_call.append(sub_cls)
+            for i, sub_cls in enumerate(type(self).mro()):
+                if i == 0:
+                    continue
+                if not sub_cls.__name__.startswith('Base'):
+                    ordered_init_call.append(sub_cls)
+
+            for i, sub_cls in enumerate(ordered_init_call):
+                if sub_cls.__name__ == 'object':
+                    sub_cls.__init__(self)
+                else:
+                    sub_cls.__init__(self, **kwargs)
+
+            init(self, **kwargs)
+
+        return sampy_init
+
+    setattr(cls, '__init__', modify_init(cls.__init__))
+
+    return cls
+
+
+def debug_method(method):
+    @wraps(method)
+    def returned_function(self, *args, **kwargs):
+        # print(args, kwargs)
+        if hasattr(self, '_sampy_debug_' + method.__name__):
+            getattr(self, '_sampy_debug_' + method.__name__)(*args, **kwargs)
+        rv = method(self, *args, **kwargs)
+        return rv
+    return returned_function
+
+
+def use_debug_mode(cls):
+    for name in dir(cls):
+        if not name.startswith('_') and hasattr(getattr(cls, name), '__call__'):
+            setattr(cls, name, debug_method(getattr(cls, name)))
```

### Comparing `sampy-abm-1.0.2/src/sampy/utils/errors_shortcut.py` & `sampy_abm-1.0.3/src/sampy/utils/errors_shortcut.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import numpy as np
-
-
-def check_input_array(array, name_argument, prefix_dtype, nb_dim=None, shape=None):
-    if not isinstance(array, np.ndarray):
-        raise TypeError("The parameter " + name_argument + " should be an array.")
-    if not str(array.dtype).startswith(prefix_dtype):
-        raise TypeError("The parameter " + name_argument + " should be an array of type " + prefix_dtype + ".")
-    if nb_dim is not None:
-        if len(array.shape) != nb_dim:
-            raise ValueError("The parameter " + name_argument + " should be an array of dim " + str(nb_dim) +
-                             ", while the input is of dim " + str(len(array.shape)) + ".")
-    if shape is not None:
-        if array.shape != shape:
-            raise ValueError("The parameter " + name_argument + " should be an array of shape " + str(shape) +
-                             ", while the input is of shape " + str(array.shape) + ".")
-
-
-def check_input_is_permutation(array, name_argument, length):
-    if (not isinstance(array, np.ndarray)) or (not str(array.dtype).startswith('int')):
-        raise TypeError("The parameter " + name_argument + " should be an array of integers.")
-    if array.shape != (length,):
-        raise ValueError("The parameter " + name_argument + " should be an array of shape (nb_agents,).")
-    if not (np.sort(array) == np.arange(0, length).all()):
-        raise ValueError("The parameter " + name_argument + " should either be None, or a permutation of all "
-                         "the integers from 0 to " + str(length - 1) + ".")
-
-
-def check_col_exists_good_type(df, name_col, name_argument, prefix_dtype='', reject_none=False):
-    if not isinstance(name_col, str):
-        raise TypeError("A column name should be a string, which is not the case for provided " + name_argument + ".")
-    if name_col not in df.dict_colname_to_index:
-        raise KeyError("Provided " + name_argument + " does not match any column name in df_population.")
-    if reject_none:
-        if df[name_col] is None:
-            raise ValueError("The column " + name_col + " is empty while it should contain the age of the agents.")
-        if not str(df[name_col].dtype).startswith(prefix_dtype):
-            raise TypeError("The column " + name_col + " is not of the proper type. Expected " + prefix_dtype +
-                            ", got " + str(df[name_col].dtype) + ".")
-
-
-def check_if_gender_array(array):
-    arr_1 = array == 1
-    arr_0 = array == 0
-    if not (arr_1 | arr_0).all():
-        raise TypeError("The provided column for gender should only contains 0s and 1s, since it is the way gender "
-                        "is encoded in sampy.")
+import numpy as np
+
+
+def check_input_array(array, name_argument, prefix_dtype, nb_dim=None, shape=None):
+    if not isinstance(array, np.ndarray):
+        raise TypeError("The parameter " + name_argument + " should be an array.")
+    if not str(array.dtype).startswith(prefix_dtype):
+        raise TypeError("The parameter " + name_argument + " should be an array of type " + prefix_dtype + ".")
+    if nb_dim is not None:
+        if len(array.shape) != nb_dim:
+            raise ValueError("The parameter " + name_argument + " should be an array of dim " + str(nb_dim) +
+                             ", while the input is of dim " + str(len(array.shape)) + ".")
+    if shape is not None:
+        if array.shape != shape:
+            raise ValueError("The parameter " + name_argument + " should be an array of shape " + str(shape) +
+                             ", while the input is of shape " + str(array.shape) + ".")
+
+
+def check_input_is_permutation(array, name_argument, length):
+    if (not isinstance(array, np.ndarray)) or (not str(array.dtype).startswith('int')):
+        raise TypeError("The parameter " + name_argument + " should be an array of integers.")
+    if array.shape != (length,):
+        raise ValueError("The parameter " + name_argument + " should be an array of shape (nb_agents,).")
+    if not (np.sort(array) == np.arange(0, length).all()):
+        raise ValueError("The parameter " + name_argument + " should either be None, or a permutation of all "
+                         "the integers from 0 to " + str(length - 1) + ".")
+
+
+def check_col_exists_good_type(df, name_col, name_argument, prefix_dtype='', reject_none=False):
+    if not isinstance(name_col, str):
+        raise TypeError("A column name should be a string, which is not the case for provided " + name_argument + ".")
+    if name_col not in df.dict_colname_to_index:
+        raise KeyError("Provided " + name_argument + " does not match any column name in df_population.")
+    if reject_none:
+        if df[name_col] is None:
+            raise ValueError("The column " + name_col + " is empty while it should contain the age of the agents.")
+        if not str(df[name_col].dtype).startswith(prefix_dtype):
+            raise TypeError("The column " + name_col + " is not of the proper type. Expected " + prefix_dtype +
+                            ", got " + str(df[name_col].dtype) + ".")
+
+
+def check_if_gender_array(array):
+    arr_1 = array == 1
+    arr_0 = array == 0
+    if not (arr_1 | arr_0).all():
+        raise TypeError("The provided column for gender should only contains 0s and 1s, since it is the way gender "
+                        "is encoded in sampy.")
```

### Comparing `sampy-abm-1.0.2/src/sampy_abm.egg-info/SOURCES.txt` & `sampy_abm-1.0.3/src/sampy_abm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 LICENSE
 README.md
 pyproject.toml
 src/sampy/__init__.py
 src/sampy/addons/__init__.py
+src/sampy/addons/GIS_interface/__init__.py
+src/sampy/addons/GIS_interface/geographic_grid.py
+src/sampy/addons/GIS_interface/jit_compiled_functions.py
 src/sampy/addons/ORM_related_addons/ORM_like_agents.py
 src/sampy/addons/ORM_related_addons/__init__.py
 src/sampy/addons/ORM_related_addons/graph_from_ORM_xml.py
 src/sampy/addons/ORM_related_addons/jit_compiled_function.py
 src/sampy/agent/__init__.py
 src/sampy/agent/base.py
 src/sampy/agent/builtin_agent.py
 src/sampy/agent/jit_compiled_functions.py
 src/sampy/agent/mortality.py
 src/sampy/agent/movement.py
 src/sampy/agent/random_walk.py
 src/sampy/agent/reproduction.py
 src/sampy/data_processing/__init__.py
 src/sampy/data_processing/csv_manager.py
+src/sampy/data_processing/extract_data_for_SCRW.py
+src/sampy/data_processing/jit_compiled_functions.py
 src/sampy/data_processing/write_file.py
 src/sampy/disease/__init__.py
 src/sampy/disease/single_species/__init__.py
 src/sampy/disease/single_species/base.py
 src/sampy/disease/single_species/builtin_disease.py
 src/sampy/disease/single_species/jit_compiled_functions.py
 src/sampy/disease/single_species/transition.py
```

### Comparing `sampy-abm-1.0.2/tests/test_agents.py` & `sampy_abm-1.0.3/tests/test_agents.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,443 +1,443 @@
-from sampy.agent.base import BaseAgingAgent
-from sampy.agent.builtin_agent import BasicMammal
-from sampy.agent.jit_compiled_functions import (count_nb_agent_per_vertex,
-                                                conditional_count_nb_agent_per_vertex,
-                                                mortality_natural_death_orm_methodology,
-                                                mortality_natural_death_orm_methodology_condition_death,
-                                                mortality_natural_death_orm_methodology_condition_count,
-                                                mortality_natural_death_orm_methodology_both_cond,
-                                                reproduction_find_random_mate_on_position,
-                                                reproduction_find_random_mate_on_position_condition,
-                                                reproduction_find_random_mate_on_position_polygamous,
-                                                reproduction_find_random_mate_on_position_polygamous_condition,
-                                                movement_change_territory_and_position,
-                                                movement_change_territory_and_position_condition,
-                                                movement_mov_around_territory_fill_bool_mov_using_condition,
-                                                movement_mov_around_territory,
-                                                movement_dispersion_with_varying_nb_of_steps,
-                                                movement_dispersion_with_varying_nb_of_steps_condition)
-from sampy.pandas_xs.pandas_xs import DataFrameXS
-from sampy.utils.decorators import use_debug_mode
-import numpy as np
-import unittest
-
-use_debug_mode(DataFrameXS)
-use_debug_mode(BaseAgingAgent)
-
-
-class TestJitCompiledFuncAgent(unittest.TestCase):
-    def test_count_nb_agents_per_vertex(self):
-        pos = np.array([0, 0, 0, 1, 1, 3, 4, 3, 2, 0, 2])
-        nb_vertex = 6
-        x = count_nb_agent_per_vertex(pos, nb_vertex)
-        self.assertTrue((x == np.array([4, 2, 2, 2, 1, 0])).all())
-
-        pos = np.array([0 for _ in range(1000)])
-        nb_vertex = 3
-        x = count_nb_agent_per_vertex(pos, nb_vertex)
-        self.assertTrue((x == np.array([1000, 0, 0])).all())
-
-    def test_conditional_count_nb_agents_per_vertex(self):
-        pos = np.array([0, 0, 0, 1, 1, 3, 4, 3, 2, 0, 2])
-        condition = np.array([False, False, False, True, True, True, True, True, True, False, True])
-        nb_vertex = 6
-        x = conditional_count_nb_agent_per_vertex(condition, pos, nb_vertex)
-        self.assertTrue((x == np.array([0, 2, 2, 2, 1, 0])).all())
-
-        pos = np.array([0 for _ in range(1000)])
-        condition = np.array([True]*400 + [False]*600)
-        nb_vertex = 3
-        x = conditional_count_nb_agent_per_vertex(condition, pos, nb_vertex)
-        self.assertTrue((x == np.array([400, 0, 0])).all())
-
-    def test_mortality_natural_death_orm_methodology(self):
-        bias = 0.
-        rand = np.array([0.5 for _ in range(8)])
-        prob_male = np.array([0.2, 0.5, 0.8, 1.])
-        prob_female = np.array([0.2, 0.4, 0.8, 1.])
-        count = np.array([2, 2, 4])
-        pos = np.array([0, 1, 2, 2, 0, 1, 2, 2])
-        k = np.array([2, 2, 2])
-        age = np.array([1, 0, 1, 1, 2, 1, 3, 3])
-        gender = np.array([0, 0, 0, 1, 1, 1, 1, 0])
-        expected_death = [0.5 > float(prob_male[1]) * (float(count[0]) / float(k[0])),
-                          0.5 > float(prob_male[0]) * (float(count[1]) / float(k[1])),
-                          0.5 > float(prob_male[1]) * (float(count[2]) / float(k[2])),
-                          0.5 > float(prob_female[1]) * (float(count[2] - 1) / float(k[2])),
-                          0.5 > float(prob_female[2]) * (float(count[0] - 1) / float(k[2])),
-                          0.5 > float(prob_female[1]) * (float(count[1]) / float(k[1])),
-                          0.5 > float(prob_female[3]) * (float(count[2] - 2) / float(k[2])),
-                          0.5 > float(prob_male[3]) * (float(count[2] - 3) / float(k[2]))]
-        death = mortality_natural_death_orm_methodology(bias, rand, prob_male, prob_female, count, pos, k, age, gender)
-        expected_death = np.array(expected_death)
-        self.assertTrue((death == expected_death).all())
-
-    def test_mortality_natural_death_orm_methodology_condition_death(self):
-        bias = 0.
-        rand = np.array([0.5 for _ in range(8)])
-        prob_male = np.array([0.2, 0.5, 0.8, 1.])
-        prob_female = np.array([0.2, 0.4, 0.8, 1.])
-        count = np.array([2, 2, 4])
-        pos = np.array([0, 1, 2, 2, 0, 1, 2, 2])
-        k = np.array([2, 2, 2])
-        age = np.array([1, 0, 1, 1, 2, 1, 3, 3])
-        gender = np.array([0, 0, 0, 1, 1, 1, 1, 0])
-        cond_death = np.array([True, True, True, True, True, True, False, True])
-        expected_death = [0.5 > float(prob_male[1]) * (float(count[0]) / float(k[0])),
-                          0.5 > float(prob_male[0]) * (float(count[1]) / float(k[1])),
-                          0.5 > float(prob_male[1]) * (float(count[2]) / float(k[2])),
-                          0.5 > float(prob_female[1]) * (float(count[2] - 1) / float(k[2])),
-                          0.5 > float(prob_female[2]) * (float(count[0] - 1) / float(k[2])),
-                          0.5 > float(prob_female[1]) * (float(count[1]) / float(k[1])),
-                          True,
-                          0.5 > float(prob_male[3]) * (float(count[2] - 2) / float(k[2]))]
-        expected_death = np.array(expected_death, dtype=np.bool_)
-        death = mortality_natural_death_orm_methodology_condition_death(bias, rand, prob_male, prob_female, count,
-                                                                        cond_death, pos, k, age, gender)
-        self.assertTrue((death == expected_death).all())
-
-    def test_mortality_natural_death_orm_methodology_condition_count(self):
-        # note that with the values considered below, the 4th agent should die if the 7th agent was counted.
-        bias = 0.
-        rand = np.array([0.5 for _ in range(8)])
-        prob_male = np.array([0.2, 0.5, 0.8, 1.])
-        prob_female = np.array([0.2, 0.4, 0.8, 1.])
-        count = np.array([2, 2, 3])
-        pos = np.array([0, 1, 2, 2, 0, 1, 2, 2])
-        k = np.array([2, 2, 2])
-        age = np.array([1, 0, 1, 1, 2, 1, 3, 3])
-        gender = np.array([0, 0, 0, 1, 1, 1, 1, 0])
-        cond_count = np.array([True, True, True, True, True, True, False, True])
-        expected_death = [0.5 > float(prob_male[1]) * (float(count[0]) / float(k[0])),
-                          0.5 > float(prob_male[0]) * (float(count[1]) / float(k[1])),
-                          0.5 > float(prob_male[1]) * (float(count[2]) / float(k[2])),
-                          0.5 > float(prob_female[1]) * (float(count[2] - 1) / float(k[2])),
-                          0.5 > float(prob_female[2]) * (float(count[0] - 1) / float(k[0])),
-                          0.5 > float(prob_female[1]) * (float(count[1]) / float(k[1])),
-                          0.5 > float(prob_female[3]) * (float(count[2] - 2) / float(k[2])),
-                          0.5 > float(prob_male[3]) * (float(count[2] - 2) / float(k[2]))]
-        expected_death = np.array(expected_death, dtype=np.bool_)
-        death = mortality_natural_death_orm_methodology_condition_count(bias, rand, prob_male, prob_female, count,
-                                                                        cond_count, pos, k, age, gender)
-        self.assertTrue((death == expected_death).all())
-
-    def test_mortality_natural_death_orm_methodology_both_cond(self):
-        # note that with the values considered below, the 4th agent should die if the 7th agent was counted.
-        bias = 0.
-        rand = np.array([0.5 for _ in range(8)])
-        prob_male = np.array([0.2, 0.5, 0.8, 1.])
-        prob_female = np.array([0.2, 0.4, 0.8, 1.])
-        count = np.array([2, 2, 3])
-        pos = np.array([0, 1, 2, 2, 0, 1, 2, 2])
-        k = np.array([2, 2, 2])
-        age = np.array([1, 0, 1, 1, 2, 1, 3, 3])
-        gender = np.array([0, 0, 0, 1, 1, 1, 1, 0])
-        cond_count = np.array([True, True, True, True, True, True, False, True])
-        cond_death = np.array([True, True, True, True, True, True, True, False])
-        expected_death = [0.5 > float(prob_male[1]) * (float(count[0]) / float(k[0])),
-                          0.5 > float(prob_male[0]) * (float(count[1]) / float(k[1])),
-                          0.5 > float(prob_male[1]) * (float(count[2]) / float(k[2])),
-                          0.5 > float(prob_female[1]) * (float(count[2] - 1) / float(k[2])),
-                          0.5 > float(prob_female[2]) * (float(count[0] - 1) / float(k[0])),
-                          0.5 > float(prob_female[1]) * (float(count[1]) / float(k[1])),
-                          0.5 > float(prob_female[3]) * (float(count[2] - 2) / float(k[2])),
-                          True]
-        expected_death = np.array(expected_death, dtype=np.bool_)
-        death = mortality_natural_death_orm_methodology_both_cond(bias, rand, prob_male, prob_female, count, cond_death,
-                                                                  cond_count, pos, k, age, gender)
-        self.assertTrue((death == expected_death).all())
-
-    def test_reproduction_find_random_mate_on_position(self):
-        col_mate = np.array([i for i in range(10)])
-        col_pregnancy = np.array([True for _ in range(10)])
-        arr_id = np.array([i for i in range(10)])
-        position = np.array([0, 0, 1, 1, 1, 2, 3, 3, 3, 3])
-        gender = np.array([i % 2 for i in range(10)])
-        nb_vertex = 5
-        rand_preg = np.array([0.4, 0.3, 0.2, 0.1, 0.8])
-        prob_preg = 0.5
-        reproduction_find_random_mate_on_position(col_mate, col_pregnancy, arr_id, position, gender, nb_vertex,
-                                                  rand_preg, prob_preg)
-        self.assertTrue((col_mate == np.array([1, 0, 3, 2, -1, -1, 7, 6, 9, 8])).all())
-        self.assertTrue((col_pregnancy == np.array([False, True, False, True, False,
-                                                    False, False, True, False, False])).all())
-
-    def test_reproduction_find_random_mate_on_position_condition(self):
-        col_mate = np.array([-2 for _ in range(10)])
-        col_pregnancy = np.array([True for _ in range(10)])
-        arr_id = np.array([i for i in range(10)])
-        position = np.array([0, 0, 1, 1, 1, 2, 3, 3, 3, 3])
-        gender = np.array([i % 2 for i in range(10)])
-        nb_vertex = 5
-        rand_preg = np.array([0.4, 0.3, 0.2, 0.1, 0.8])
-        prob_preg = 0.5
-        condition = np.array([False] + [True for _ in range(9)])
-        reproduction_find_random_mate_on_position_condition(col_mate,col_pregnancy, arr_id, position, gender, nb_vertex,
-                                                            rand_preg, prob_preg, condition)
-        self.assertTrue((col_mate == np.array([-2, -1, 3, 2, -1, -1, 7, 6, 9, 8])).all())
-        self.assertTrue((col_pregnancy == np.array([True, False, False, True, False,
-                                                    False, False, True, False, False])).all())
-        # Yup, there is a pregnant male above. That's normal. It's to check that the function is not modifying anything
-        # when condition is set on False.
-
-    def test_reproduction_find_random_mate_on_position_polygamous(self):
-        col_mate = np.array([-2 for _ in range(10)])
-        col_pregnancy = np.array([False for _ in range(10)])
-        arr_id = np.array([i for i in range(10)])
-        position = np.array([0, 0, 1, 1, 1, 2, 3, 3, 3, 3])
-        gender = np.array([i % 2 for i in range(10)])
-        nb_vertex = 5
-        rand_preg = np.array([0.4, 0.3, 0.2, 0.1, 0.8])
-        rand_mate = np.array([0.98, 0.6, 0.1, 0.2, 0.49])
-        prob_preg = 0.5
-        reproduction_find_random_mate_on_position_polygamous(arr_id, position, gender, col_mate, col_pregnancy,
-                                                             nb_vertex, rand_preg, rand_mate, prob_preg)
-        self.assertTrue((col_mate == np.array([-1, 0, -1, 4, -1, -1, -1, 6, -1, 6])).all())
-        self.assertTrue((col_pregnancy == np.array([False, True, False, True, False,
-                                                    False, False, True, False, False])).all())
-
-    def test_reproduction_find_random_mate_on_position_polygamous_condition(self):
-        col_mate = np.array([-2 for _ in range(10)])
-        col_pregnancy = np.array([True for _ in range(10)])
-        arr_id = np.array([i for i in range(10)])
-        position = np.array([0, 0, 1, 1, 1, 2, 3, 3, 3, 3])
-        gender = np.array([i % 2 for i in range(10)])
-        nb_vertex = 5
-        rand_preg = np.array([0.4, 0.3, 0.2, 0.1, 0.8])
-        rand_mate = np.array([0.98, 0.6, 0.1, 0.2, 0.49])
-        prob_preg = 0.5
-        condition = np.array([False] + [True for _ in range(9)])
-        reproduction_find_random_mate_on_position_polygamous_condition(arr_id, position, gender, col_mate,
-                                                                       col_pregnancy, nb_vertex, rand_preg, rand_mate,
-                                                                       prob_preg, condition)
-        self.assertTrue((col_mate == np.array([-2, -1, -1, 4, -1, -1, -1, 6, -1, 6])).all())
-        self.assertTrue((col_pregnancy == np.array([True, False, False, True, False,
-                                                    False, False, True, False, False])).all())
-
-    def test_movement_change_territory_and_position(self):
-        territory = np.array([0, 0, 1, 1, 2, 2, 3, 3, 4, 4, 5, 5])
-        position = np.array([i % 5 for i in range(12)])
-        rand = np.array([0.5 for _ in range(12)])
-        connections = np.array([[-1, -1, -1],
-                                [2, -1, -1],
-                                [1, -1, -1],
-                                [4, 5, -1],
-                                [3, 5, -1],
-                                [3, -1, 4]])
-        weights = np.array([[-1., -1., -1.],
-                            [1., -1., -1.],
-                            [1., -1., -1.],
-                            [.6, 1., -1],
-                            [.4, 1., -1.],
-                            [.4, -1., 1.]])
-
-        movement_change_territory_and_position(territory, position, rand, connections, weights)
-
-        self.assertTrue((territory == position).all())
-        self.assertTrue((territory == np.array([0, 0, 2, 2, 1, 1, 4, 4, 5, 5, 4, 4])).all())
-
-    def test_movement_change_territory_and_position_condition(self):
-        condition = np.array([i % 2 == 1 for i in range(12)])
-        territory = np.array([0, 0, 1, 1, 2, 2, 3, 3, 4, 4, 5, 5])
-        position = np.array([i % 5 for i in range(12)])
-        rand = np.array([0.5 for _ in range(12)])
-        connections = np.array([[-1, -1, -1],
-                                [2, -1, -1],
-                                [1, -1, -1],
-                                [4, 5, -1],
-                                [3, 5, -1],
-                                [3, -1, 4]])
-        weights = np.array([[-1., -1., -1.],
-                            [1., -1., -1.],
-                            [1., -1., -1.],
-                            [.6, 1., -1],
-                            [.4, 1., -1.],
-                            [.4, -1., 1.]])
-
-        movement_change_territory_and_position_condition(territory, position, condition, rand, connections, weights)
-
-        self.assertTrue((position == np.array([0, 0, 2, 2, 4, 1, 1, 4, 3, 5, 0, 4])).all())
-        self.assertTrue((territory == np.array([0, 0, 1, 2, 2, 1, 3, 4, 4, 5, 5, 4])).all())
-
-    def test_movement_mov_around_territory_fill_bool_mov_using_condition(self):
-        condition = np.array([i % 2 == 0 for i in range(10)])
-        pre_bol_mov = np.array([True, True, False, False, True])
-        result = movement_mov_around_territory_fill_bool_mov_using_condition(pre_bol_mov, condition)
-
-        self.assertTrue((result == np.array([True, False, True, False, False, False, False, False, True, False])).all())
-
-    def test_movement_mov_around_territory(self):
-        territory = np.array([0, 0, 1, 1, 2, 2, 3, 3, 4, 4, 5, 5])
-        position = np.array([i % 5 for i in range(12)])
-        rand = np.array([0.5 for _ in range(6)])
-        connections = np.array([[-1, -1, -1],
-                                [2, -1, -1],
-                                [1, -1, -1],
-                                [4, 5, -1],
-                                [3, 5, -1],
-                                [3, -1, 4]])
-        weights = np.array([[-1., -1., -1.],
-                            [1., -1., -1.],
-                            [1., -1., -1.],
-                            [.6, 1., -1.],
-                            [.4, 1., -1.],
-                            [.4, -1., 1.]])
-        bool_mov = np.array([i % 2 == 0 for i in range(12)])
-        movement_mov_around_territory(territory, position, bool_mov, rand, connections, weights)
-        self.assertTrue((position == np.array([0, 1, 2, 3, 1, 0, 4, 2, 5, 4, 4, 1])).all())
-        self.assertTrue((territory == np.array([0, 0, 1, 1, 2, 2, 3, 3, 4, 4, 5, 5])).all())
-
-    def test_movement_dispersion_with_varying_nb_of_steps(self):
-        territory = np.array([0, 0, 1, 1, 2, 2, 3, 3, 4, 4, 5, 5])
-        position = np.array([i % 5 for i in range(12)])
-        nb_steps = np.array([0, 1, 1, 2, 1, 2, 1, 1, 0, 1, 0, 3])
-        rand = np.array([.5, .5, .5, .5, .5, .5, .5, .7, .5, .5, .3, .5, .5])
-        connections = np.array([[-1, -1, -1],
-                                [2, -1, -1],
-                                [1, -1, -1],
-                                [4, 5, -1],
-                                [3, 5, -1],
-                                [3, -1, 4]])
-        weights = np.array([[-1., -1., -1.],
-                            [1., -1., -1.],
-                            [1., -1., -1.],
-                            [.6, 1., -1.],
-                            [.4, 1., -1.],
-                            [.4, -1., 1.]])
-        movement_dispersion_with_varying_nb_of_steps(territory, position, rand, nb_steps, connections, weights)
-        self.assertTrue((position == territory).all())
-        self.assertTrue((position == np.array([0, 0, 2, 1, 1, 2, 5, 4, 4, 5, 5, 5])).all())
-
-    def test_movement_dispersion_with_varying_nb_of_steps_condition(self):
-        territory = np.array([0, 0, 1, 1, 2, 2, 3, 3, 4, 4, 5, 5])
-        position = np.array([i % 5 for i in range(12)])
-        condition = np.array([True, False] + [True for _ in range(10)])
-        nb_steps = np.array([0, 1, 2, 1, 2, 1, 1, 0, 1, 0, 3])
-        rand = np.array([.5, .5, .5, .5, .5, .5, .7, .5, .5, .3, .5, .5])
-        connections = np.array([[-1, -1, -1],
-                                [2, -1, -1],
-                                [1, -1, -1],
-                                [4, 5, -1],
-                                [3, 5, -1],
-                                [3, -1, 4]])
-        weights = np.array([[-1., -1., -1.],
-                            [1., -1., -1.],
-                            [1., -1., -1.],
-                            [.6, 1., -1.],
-                            [.4, 1., -1.],
-                            [.4, -1., 1.]])
-        movement_dispersion_with_varying_nb_of_steps_condition(territory, position, condition, rand, nb_steps,
-                                                               connections, weights)
-        self.assertTrue((position == np.array([0, 1, 2, 1, 1, 2, 5, 4, 4, 5, 5, 5])).all())
-        self.assertTrue((territory == np.array([0, 0, 2, 1, 1, 2, 5, 4, 4, 5, 5, 5])).all())
-
-
-class TestBaseAgingAgent(unittest.TestCase):
-
-    def test_error_when_missing_graph(self):
-        with self.assertRaises(ValueError):
-            x = BaseAgingAgent()
-
-    def test_creation_when_something_as_graph(self):
-        x = BaseAgingAgent(graph='test')
-        self.assertTrue(isinstance(x.df_population, DataFrameXS))
-        self.assertEqual(x.df_population.list_col_name, ['col_id', 'age'])
-        self.assertEqual(x.df_population.list_col, [None, None])
-        self.assertEqual(x.df_population.nb_rows, 0)
-        self.assertEqual(x.df_population.nb_cols, 2)
-        self.assertEqual(x.df_population.shape, (0, 2))
-        self.assertEqual(x.dict_default_val, {'age': 0})
-
-    def test_change_default_val(self):
-        x = BaseAgingAgent(graph='test')
-        with self.assertRaises(TypeError):
-            x.set_default_val([])
-        with self.assertRaises(KeyError):
-            x.set_default_val({'test': 10})
-
-        x.add_attribute('test', def_value=10)
-        self.assertEqual(x.dict_default_val, {'age': 0, 'test': 10})
-        x.set_default_val({'age': 2}, replace=True)
-        self.assertEqual(x.dict_default_val, {'age': 2})
-
-    def test_add_agents(self):
-        x = BaseAgingAgent(graph='test')
-        with self.assertRaises(ValueError):
-            x.add_agents({'age': ['test', 'test2']})
-        with self.assertRaises(KeyError):
-            x.add_agents({'wrong_col_name': [0, 0]})
-
-        x.add_agents({'age': [1, 2, 3, 4]})
-        self.assertTrue((x.df_population['age'] == np.array([1, 2, 3, 4])).all())
-        self.assertTrue((x.df_population['col_id'] == np.array([0, 1, 2, 3])).all())
-        self.assertEqual(x.df_population.shape, (4, 2))
-
-        x.add_attribute('test_attr', def_value=10)
-        x.add_agents({'age': 1})
-        self.assertTrue((x.df_population['age'] == np.array([1, 2, 3, 4, 1])).all())
-        self.assertTrue((x.df_population['col_id'] == np.array([0, 1, 2, 3, 4])).all())
-        self.assertTrue((x.df_population['test_attr'] == np.array([10, 10, 10, 10, 10])).all())
-        self.assertEqual(x.df_population.shape, (5, 3))
-
-        x.add_attribute('test_attr2')
-        x.add_agents({'age': 17})
-        self.assertTrue((x.df_population['age'] == np.array([1, 2, 3, 4, 1, 17])).all())
-        self.assertTrue((x.df_population['col_id'] == np.array([0, 1, 2, 3, 4, 5])).all())
-        self.assertTrue((x.df_population['test_attr'] == np.array([10, 10, 10, 10, 10, 10])).all())
-        self.assertTrue((np.nan_to_num(x.df_population['test_attr2'], 0.) == np.array([0., 0., 0., 0., 0., 0.])).all())
-        self.assertEqual(x.df_population.shape, (6, 4))
-
-        x.add_agents({'age': [3, 4], 'test_attr2': 3.})
-        self.assertTrue((x.df_population['age'] == np.array([1, 2, 3, 4, 1, 17, 3, 4])).all())
-        self.assertTrue((x.df_population['col_id'] == np.array([0, 1, 2, 3, 4, 5, 6, 7])).all())
-        self.assertTrue((x.df_population['test_attr'] == np.array([10, 10, 10, 10, 10, 10, 10, 10])).all())
-        self.assertTrue((np.nan_to_num(x.df_population['test_attr2'], 0.) == np.array([0., 0., 0., 0., 0., 0., 3., 3.])).all())
-        self.assertEqual(x.df_population.shape, (8, 4))
-
-        with self.assertRaises(ValueError):
-            x.add_agents({'age': [1, 2], 'test_attr': [4, 5, 6]})
-
-    def test_count_agents_per_vertex(self):
-        class FakeGraph:
-            weights = np.array([0, 0, 0, 0, 0])
-        x = BaseAgingAgent(graph=FakeGraph())
-        x.add_attribute('position', def_value=0)
-        x.add_agents({'age': 0, 'position': [0, 0, 0, 1, 1, 3, 4, 3, 2, 0, 2]})
-
-        count_all = x.count_pop_per_vertex()
-
-        self.assertEqual(count_all.sum(), 11)
-        self.assertTrue((count_all == np.array([4, 2, 2, 2, 1])).all())
-
-        with self.assertRaises(ValueError):
-            condition = np.array([True, False])
-            x.count_pop_per_vertex(condition=condition)
-
-        with self.assertRaises(ValueError):
-            condition = np.array([0, 0, 0, 1, 1, 3, 4, 3, 2, 0, 2])
-            x.count_pop_per_vertex(condition=condition)
-
-        with self.assertRaises(ValueError):
-            condition = np.array([[0, 0, 0, 1, 1, 3, 4, 3, 2, 0, 2]])
-            x.count_pop_per_vertex(condition=condition)
-
-        with self.assertRaises(ValueError):
-            condition = {}
-            x.count_pop_per_vertex(condition=condition)
-
-        condition = np.array([False, False, False, True, True, True, True, True, True, False, True])
-        count_cond = x.count_pop_per_vertex(condition=condition)
-
-        self.assertEqual(count_cond.sum(), 7)
-        self.assertTrue((count_cond == np.array([0, 2, 2, 2, 1])).all())
-
-
-class TestMovementTerritorialMovementWithoutResistance(unittest.TestCase):
-    pass
-
-
-class TestBuiltInAgentBasicMammal(unittest.TestCase):
-    def test_object_creation(self):
-        with self.assertRaises(ValueError):
-            x = BasicMammal()
+from sampy.agent.base import BaseAgingAgent
+from sampy.agent.builtin_agent import BasicMammal
+from sampy.agent.jit_compiled_functions import (count_nb_agent_per_vertex,
+                                                conditional_count_nb_agent_per_vertex,
+                                                mortality_natural_death_orm_methodology,
+                                                mortality_natural_death_orm_methodology_condition_death,
+                                                mortality_natural_death_orm_methodology_condition_count,
+                                                mortality_natural_death_orm_methodology_both_cond,
+                                                reproduction_find_random_mate_on_position,
+                                                reproduction_find_random_mate_on_position_condition,
+                                                reproduction_find_random_mate_on_position_polygamous,
+                                                reproduction_find_random_mate_on_position_polygamous_condition,
+                                                movement_change_territory_and_position,
+                                                movement_change_territory_and_position_condition,
+                                                movement_mov_around_territory_fill_bool_mov_using_condition,
+                                                movement_mov_around_territory,
+                                                movement_dispersion_with_varying_nb_of_steps,
+                                                movement_dispersion_with_varying_nb_of_steps_condition)
+from sampy.pandas_xs.pandas_xs import DataFrameXS
+from sampy.utils.decorators import use_debug_mode
+import numpy as np
+import unittest
+
+use_debug_mode(DataFrameXS)
+use_debug_mode(BaseAgingAgent)
+
+
+class TestJitCompiledFuncAgent(unittest.TestCase):
+    def test_count_nb_agents_per_vertex(self):
+        pos = np.array([0, 0, 0, 1, 1, 3, 4, 3, 2, 0, 2])
+        nb_vertex = 6
+        x = count_nb_agent_per_vertex(pos, nb_vertex)
+        self.assertTrue((x == np.array([4, 2, 2, 2, 1, 0])).all())
+
+        pos = np.array([0 for _ in range(1000)])
+        nb_vertex = 3
+        x = count_nb_agent_per_vertex(pos, nb_vertex)
+        self.assertTrue((x == np.array([1000, 0, 0])).all())
+
+    def test_conditional_count_nb_agents_per_vertex(self):
+        pos = np.array([0, 0, 0, 1, 1, 3, 4, 3, 2, 0, 2])
+        condition = np.array([False, False, False, True, True, True, True, True, True, False, True])
+        nb_vertex = 6
+        x = conditional_count_nb_agent_per_vertex(condition, pos, nb_vertex)
+        self.assertTrue((x == np.array([0, 2, 2, 2, 1, 0])).all())
+
+        pos = np.array([0 for _ in range(1000)])
+        condition = np.array([True]*400 + [False]*600)
+        nb_vertex = 3
+        x = conditional_count_nb_agent_per_vertex(condition, pos, nb_vertex)
+        self.assertTrue((x == np.array([400, 0, 0])).all())
+
+    def test_mortality_natural_death_orm_methodology(self):
+        bias = 0.
+        rand = np.array([0.5 for _ in range(8)])
+        prob_male = np.array([0.2, 0.5, 0.8, 1.])
+        prob_female = np.array([0.2, 0.4, 0.8, 1.])
+        count = np.array([2, 2, 4])
+        pos = np.array([0, 1, 2, 2, 0, 1, 2, 2])
+        k = np.array([2, 2, 2])
+        age = np.array([1, 0, 1, 1, 2, 1, 3, 3])
+        gender = np.array([0, 0, 0, 1, 1, 1, 1, 0])
+        expected_death = [0.5 > float(prob_male[1]) * (float(count[0]) / float(k[0])),
+                          0.5 > float(prob_male[0]) * (float(count[1]) / float(k[1])),
+                          0.5 > float(prob_male[1]) * (float(count[2]) / float(k[2])),
+                          0.5 > float(prob_female[1]) * (float(count[2] - 1) / float(k[2])),
+                          0.5 > float(prob_female[2]) * (float(count[0] - 1) / float(k[2])),
+                          0.5 > float(prob_female[1]) * (float(count[1]) / float(k[1])),
+                          0.5 > float(prob_female[3]) * (float(count[2] - 2) / float(k[2])),
+                          0.5 > float(prob_male[3]) * (float(count[2] - 3) / float(k[2]))]
+        death = mortality_natural_death_orm_methodology(bias, rand, prob_male, prob_female, count, pos, k, age, gender)
+        expected_death = np.array(expected_death)
+        self.assertTrue((death == expected_death).all())
+
+    def test_mortality_natural_death_orm_methodology_condition_death(self):
+        bias = 0.
+        rand = np.array([0.5 for _ in range(8)])
+        prob_male = np.array([0.2, 0.5, 0.8, 1.])
+        prob_female = np.array([0.2, 0.4, 0.8, 1.])
+        count = np.array([2, 2, 4])
+        pos = np.array([0, 1, 2, 2, 0, 1, 2, 2])
+        k = np.array([2, 2, 2])
+        age = np.array([1, 0, 1, 1, 2, 1, 3, 3])
+        gender = np.array([0, 0, 0, 1, 1, 1, 1, 0])
+        cond_death = np.array([True, True, True, True, True, True, False, True])
+        expected_death = [0.5 > float(prob_male[1]) * (float(count[0]) / float(k[0])),
+                          0.5 > float(prob_male[0]) * (float(count[1]) / float(k[1])),
+                          0.5 > float(prob_male[1]) * (float(count[2]) / float(k[2])),
+                          0.5 > float(prob_female[1]) * (float(count[2] - 1) / float(k[2])),
+                          0.5 > float(prob_female[2]) * (float(count[0] - 1) / float(k[2])),
+                          0.5 > float(prob_female[1]) * (float(count[1]) / float(k[1])),
+                          True,
+                          0.5 > float(prob_male[3]) * (float(count[2] - 2) / float(k[2]))]
+        expected_death = np.array(expected_death, dtype=np.bool_)
+        death = mortality_natural_death_orm_methodology_condition_death(bias, rand, prob_male, prob_female, count,
+                                                                        cond_death, pos, k, age, gender)
+        self.assertTrue((death == expected_death).all())
+
+    def test_mortality_natural_death_orm_methodology_condition_count(self):
+        # note that with the values considered below, the 4th agent should die if the 7th agent was counted.
+        bias = 0.
+        rand = np.array([0.5 for _ in range(8)])
+        prob_male = np.array([0.2, 0.5, 0.8, 1.])
+        prob_female = np.array([0.2, 0.4, 0.8, 1.])
+        count = np.array([2, 2, 3])
+        pos = np.array([0, 1, 2, 2, 0, 1, 2, 2])
+        k = np.array([2, 2, 2])
+        age = np.array([1, 0, 1, 1, 2, 1, 3, 3])
+        gender = np.array([0, 0, 0, 1, 1, 1, 1, 0])
+        cond_count = np.array([True, True, True, True, True, True, False, True])
+        expected_death = [0.5 > float(prob_male[1]) * (float(count[0]) / float(k[0])),
+                          0.5 > float(prob_male[0]) * (float(count[1]) / float(k[1])),
+                          0.5 > float(prob_male[1]) * (float(count[2]) / float(k[2])),
+                          0.5 > float(prob_female[1]) * (float(count[2] - 1) / float(k[2])),
+                          0.5 > float(prob_female[2]) * (float(count[0] - 1) / float(k[0])),
+                          0.5 > float(prob_female[1]) * (float(count[1]) / float(k[1])),
+                          0.5 > float(prob_female[3]) * (float(count[2] - 2) / float(k[2])),
+                          0.5 > float(prob_male[3]) * (float(count[2] - 2) / float(k[2]))]
+        expected_death = np.array(expected_death, dtype=np.bool_)
+        death = mortality_natural_death_orm_methodology_condition_count(bias, rand, prob_male, prob_female, count,
+                                                                        cond_count, pos, k, age, gender)
+        self.assertTrue((death == expected_death).all())
+
+    def test_mortality_natural_death_orm_methodology_both_cond(self):
+        # note that with the values considered below, the 4th agent should die if the 7th agent was counted.
+        bias = 0.
+        rand = np.array([0.5 for _ in range(8)])
+        prob_male = np.array([0.2, 0.5, 0.8, 1.])
+        prob_female = np.array([0.2, 0.4, 0.8, 1.])
+        count = np.array([2, 2, 3])
+        pos = np.array([0, 1, 2, 2, 0, 1, 2, 2])
+        k = np.array([2, 2, 2])
+        age = np.array([1, 0, 1, 1, 2, 1, 3, 3])
+        gender = np.array([0, 0, 0, 1, 1, 1, 1, 0])
+        cond_count = np.array([True, True, True, True, True, True, False, True])
+        cond_death = np.array([True, True, True, True, True, True, True, False])
+        expected_death = [0.5 > float(prob_male[1]) * (float(count[0]) / float(k[0])),
+                          0.5 > float(prob_male[0]) * (float(count[1]) / float(k[1])),
+                          0.5 > float(prob_male[1]) * (float(count[2]) / float(k[2])),
+                          0.5 > float(prob_female[1]) * (float(count[2] - 1) / float(k[2])),
+                          0.5 > float(prob_female[2]) * (float(count[0] - 1) / float(k[0])),
+                          0.5 > float(prob_female[1]) * (float(count[1]) / float(k[1])),
+                          0.5 > float(prob_female[3]) * (float(count[2] - 2) / float(k[2])),
+                          True]
+        expected_death = np.array(expected_death, dtype=np.bool_)
+        death = mortality_natural_death_orm_methodology_both_cond(bias, rand, prob_male, prob_female, count, cond_death,
+                                                                  cond_count, pos, k, age, gender)
+        self.assertTrue((death == expected_death).all())
+
+    def test_reproduction_find_random_mate_on_position(self):
+        col_mate = np.array([i for i in range(10)])
+        col_pregnancy = np.array([True for _ in range(10)])
+        arr_id = np.array([i for i in range(10)])
+        position = np.array([0, 0, 1, 1, 1, 2, 3, 3, 3, 3])
+        gender = np.array([i % 2 for i in range(10)])
+        nb_vertex = 5
+        rand_preg = np.array([0.4, 0.3, 0.2, 0.1, 0.8])
+        prob_preg = 0.5
+        reproduction_find_random_mate_on_position(col_mate, col_pregnancy, arr_id, position, gender, nb_vertex,
+                                                  rand_preg, prob_preg)
+        self.assertTrue((col_mate == np.array([1, 0, 3, 2, -1, -1, 7, 6, 9, 8])).all())
+        self.assertTrue((col_pregnancy == np.array([False, True, False, True, False,
+                                                    False, False, True, False, False])).all())
+
+    def test_reproduction_find_random_mate_on_position_condition(self):
+        col_mate = np.array([-2 for _ in range(10)])
+        col_pregnancy = np.array([True for _ in range(10)])
+        arr_id = np.array([i for i in range(10)])
+        position = np.array([0, 0, 1, 1, 1, 2, 3, 3, 3, 3])
+        gender = np.array([i % 2 for i in range(10)])
+        nb_vertex = 5
+        rand_preg = np.array([0.4, 0.3, 0.2, 0.1, 0.8])
+        prob_preg = 0.5
+        condition = np.array([False] + [True for _ in range(9)])
+        reproduction_find_random_mate_on_position_condition(col_mate,col_pregnancy, arr_id, position, gender, nb_vertex,
+                                                            rand_preg, prob_preg, condition)
+        self.assertTrue((col_mate == np.array([-2, -1, 3, 2, -1, -1, 7, 6, 9, 8])).all())
+        self.assertTrue((col_pregnancy == np.array([True, False, False, True, False,
+                                                    False, False, True, False, False])).all())
+        # Yup, there is a pregnant male above. That's normal. It's to check that the function is not modifying anything
+        # when condition is set on False.
+
+    def test_reproduction_find_random_mate_on_position_polygamous(self):
+        col_mate = np.array([-2 for _ in range(10)])
+        col_pregnancy = np.array([False for _ in range(10)])
+        arr_id = np.array([i for i in range(10)])
+        position = np.array([0, 0, 1, 1, 1, 2, 3, 3, 3, 3])
+        gender = np.array([i % 2 for i in range(10)])
+        nb_vertex = 5
+        rand_preg = np.array([0.4, 0.3, 0.2, 0.1, 0.8])
+        rand_mate = np.array([0.98, 0.6, 0.1, 0.2, 0.49])
+        prob_preg = 0.5
+        reproduction_find_random_mate_on_position_polygamous(arr_id, position, gender, col_mate, col_pregnancy,
+                                                             nb_vertex, rand_preg, rand_mate, prob_preg)
+        self.assertTrue((col_mate == np.array([-1, 0, -1, 4, -1, -1, -1, 6, -1, 6])).all())
+        self.assertTrue((col_pregnancy == np.array([False, True, False, True, False,
+                                                    False, False, True, False, False])).all())
+
+    def test_reproduction_find_random_mate_on_position_polygamous_condition(self):
+        col_mate = np.array([-2 for _ in range(10)])
+        col_pregnancy = np.array([True for _ in range(10)])
+        arr_id = np.array([i for i in range(10)])
+        position = np.array([0, 0, 1, 1, 1, 2, 3, 3, 3, 3])
+        gender = np.array([i % 2 for i in range(10)])
+        nb_vertex = 5
+        rand_preg = np.array([0.4, 0.3, 0.2, 0.1, 0.8])
+        rand_mate = np.array([0.98, 0.6, 0.1, 0.2, 0.49])
+        prob_preg = 0.5
+        condition = np.array([False] + [True for _ in range(9)])
+        reproduction_find_random_mate_on_position_polygamous_condition(arr_id, position, gender, col_mate,
+                                                                       col_pregnancy, nb_vertex, rand_preg, rand_mate,
+                                                                       prob_preg, condition)
+        self.assertTrue((col_mate == np.array([-2, -1, -1, 4, -1, -1, -1, 6, -1, 6])).all())
+        self.assertTrue((col_pregnancy == np.array([True, False, False, True, False,
+                                                    False, False, True, False, False])).all())
+
+    def test_movement_change_territory_and_position(self):
+        territory = np.array([0, 0, 1, 1, 2, 2, 3, 3, 4, 4, 5, 5])
+        position = np.array([i % 5 for i in range(12)])
+        rand = np.array([0.5 for _ in range(12)])
+        connections = np.array([[-1, -1, -1],
+                                [2, -1, -1],
+                                [1, -1, -1],
+                                [4, 5, -1],
+                                [3, 5, -1],
+                                [3, -1, 4]])
+        weights = np.array([[-1., -1., -1.],
+                            [1., -1., -1.],
+                            [1., -1., -1.],
+                            [.6, 1., -1],
+                            [.4, 1., -1.],
+                            [.4, -1., 1.]])
+
+        movement_change_territory_and_position(territory, position, rand, connections, weights)
+
+        self.assertTrue((territory == position).all())
+        self.assertTrue((territory == np.array([0, 0, 2, 2, 1, 1, 4, 4, 5, 5, 4, 4])).all())
+
+    def test_movement_change_territory_and_position_condition(self):
+        condition = np.array([i % 2 == 1 for i in range(12)])
+        territory = np.array([0, 0, 1, 1, 2, 2, 3, 3, 4, 4, 5, 5])
+        position = np.array([i % 5 for i in range(12)])
+        rand = np.array([0.5 for _ in range(12)])
+        connections = np.array([[-1, -1, -1],
+                                [2, -1, -1],
+                                [1, -1, -1],
+                                [4, 5, -1],
+                                [3, 5, -1],
+                                [3, -1, 4]])
+        weights = np.array([[-1., -1., -1.],
+                            [1., -1., -1.],
+                            [1., -1., -1.],
+                            [.6, 1., -1],
+                            [.4, 1., -1.],
+                            [.4, -1., 1.]])
+
+        movement_change_territory_and_position_condition(territory, position, condition, rand, connections, weights)
+
+        self.assertTrue((position == np.array([0, 0, 2, 2, 4, 1, 1, 4, 3, 5, 0, 4])).all())
+        self.assertTrue((territory == np.array([0, 0, 1, 2, 2, 1, 3, 4, 4, 5, 5, 4])).all())
+
+    def test_movement_mov_around_territory_fill_bool_mov_using_condition(self):
+        condition = np.array([i % 2 == 0 for i in range(10)])
+        pre_bol_mov = np.array([True, True, False, False, True])
+        result = movement_mov_around_territory_fill_bool_mov_using_condition(pre_bol_mov, condition)
+
+        self.assertTrue((result == np.array([True, False, True, False, False, False, False, False, True, False])).all())
+
+    def test_movement_mov_around_territory(self):
+        territory = np.array([0, 0, 1, 1, 2, 2, 3, 3, 4, 4, 5, 5])
+        position = np.array([i % 5 for i in range(12)])
+        rand = np.array([0.5 for _ in range(6)])
+        connections = np.array([[-1, -1, -1],
+                                [2, -1, -1],
+                                [1, -1, -1],
+                                [4, 5, -1],
+                                [3, 5, -1],
+                                [3, -1, 4]])
+        weights = np.array([[-1., -1., -1.],
+                            [1., -1., -1.],
+                            [1., -1., -1.],
+                            [.6, 1., -1.],
+                            [.4, 1., -1.],
+                            [.4, -1., 1.]])
+        bool_mov = np.array([i % 2 == 0 for i in range(12)])
+        movement_mov_around_territory(territory, position, bool_mov, rand, connections, weights)
+        self.assertTrue((position == np.array([0, 1, 2, 3, 1, 0, 4, 2, 5, 4, 4, 1])).all())
+        self.assertTrue((territory == np.array([0, 0, 1, 1, 2, 2, 3, 3, 4, 4, 5, 5])).all())
+
+    def test_movement_dispersion_with_varying_nb_of_steps(self):
+        territory = np.array([0, 0, 1, 1, 2, 2, 3, 3, 4, 4, 5, 5])
+        position = np.array([i % 5 for i in range(12)])
+        nb_steps = np.array([0, 1, 1, 2, 1, 2, 1, 1, 0, 1, 0, 3])
+        rand = np.array([.5, .5, .5, .5, .5, .5, .5, .7, .5, .5, .3, .5, .5])
+        connections = np.array([[-1, -1, -1],
+                                [2, -1, -1],
+                                [1, -1, -1],
+                                [4, 5, -1],
+                                [3, 5, -1],
+                                [3, -1, 4]])
+        weights = np.array([[-1., -1., -1.],
+                            [1., -1., -1.],
+                            [1., -1., -1.],
+                            [.6, 1., -1.],
+                            [.4, 1., -1.],
+                            [.4, -1., 1.]])
+        movement_dispersion_with_varying_nb_of_steps(territory, position, rand, nb_steps, connections, weights)
+        self.assertTrue((position == territory).all())
+        self.assertTrue((position == np.array([0, 0, 2, 1, 1, 2, 5, 4, 4, 5, 5, 5])).all())
+
+    def test_movement_dispersion_with_varying_nb_of_steps_condition(self):
+        territory = np.array([0, 0, 1, 1, 2, 2, 3, 3, 4, 4, 5, 5])
+        position = np.array([i % 5 for i in range(12)])
+        condition = np.array([True, False] + [True for _ in range(10)])
+        nb_steps = np.array([0, 1, 2, 1, 2, 1, 1, 0, 1, 0, 3])
+        rand = np.array([.5, .5, .5, .5, .5, .5, .7, .5, .5, .3, .5, .5])
+        connections = np.array([[-1, -1, -1],
+                                [2, -1, -1],
+                                [1, -1, -1],
+                                [4, 5, -1],
+                                [3, 5, -1],
+                                [3, -1, 4]])
+        weights = np.array([[-1., -1., -1.],
+                            [1., -1., -1.],
+                            [1., -1., -1.],
+                            [.6, 1., -1.],
+                            [.4, 1., -1.],
+                            [.4, -1., 1.]])
+        movement_dispersion_with_varying_nb_of_steps_condition(territory, position, condition, rand, nb_steps,
+                                                               connections, weights)
+        self.assertTrue((position == np.array([0, 1, 2, 1, 1, 2, 5, 4, 4, 5, 5, 5])).all())
+        self.assertTrue((territory == np.array([0, 0, 2, 1, 1, 2, 5, 4, 4, 5, 5, 5])).all())
+
+
+class TestBaseAgingAgent(unittest.TestCase):
+
+    def test_error_when_missing_graph(self):
+        with self.assertRaises(ValueError):
+            x = BaseAgingAgent()
+
+    def test_creation_when_something_as_graph(self):
+        x = BaseAgingAgent(graph='test')
+        self.assertTrue(isinstance(x.df_population, DataFrameXS))
+        self.assertEqual(x.df_population.list_col_name, ['col_id', 'age'])
+        self.assertEqual(x.df_population.list_col, [None, None])
+        self.assertEqual(x.df_population.nb_rows, 0)
+        self.assertEqual(x.df_population.nb_cols, 2)
+        self.assertEqual(x.df_population.shape, (0, 2))
+        self.assertEqual(x.dict_default_val, {'age': 0})
+
+    def test_change_default_val(self):
+        x = BaseAgingAgent(graph='test')
+        with self.assertRaises(TypeError):
+            x.set_default_val([])
+        with self.assertRaises(KeyError):
+            x.set_default_val({'test': 10})
+
+        x.add_attribute('test', def_value=10)
+        self.assertEqual(x.dict_default_val, {'age': 0, 'test': 10})
+        x.set_default_val({'age': 2}, replace=True)
+        self.assertEqual(x.dict_default_val, {'age': 2})
+
+    def test_add_agents(self):
+        x = BaseAgingAgent(graph='test')
+        with self.assertRaises(ValueError):
+            x.add_agents({'age': ['test', 'test2']})
+        with self.assertRaises(KeyError):
+            x.add_agents({'wrong_col_name': [0, 0]})
+
+        x.add_agents({'age': [1, 2, 3, 4]})
+        self.assertTrue((x.df_population['age'] == np.array([1, 2, 3, 4])).all())
+        self.assertTrue((x.df_population['col_id'] == np.array([0, 1, 2, 3])).all())
+        self.assertEqual(x.df_population.shape, (4, 2))
+
+        x.add_attribute('test_attr', def_value=10)
+        x.add_agents({'age': 1})
+        self.assertTrue((x.df_population['age'] == np.array([1, 2, 3, 4, 1])).all())
+        self.assertTrue((x.df_population['col_id'] == np.array([0, 1, 2, 3, 4])).all())
+        self.assertTrue((x.df_population['test_attr'] == np.array([10, 10, 10, 10, 10])).all())
+        self.assertEqual(x.df_population.shape, (5, 3))
+
+        x.add_attribute('test_attr2')
+        x.add_agents({'age': 17})
+        self.assertTrue((x.df_population['age'] == np.array([1, 2, 3, 4, 1, 17])).all())
+        self.assertTrue((x.df_population['col_id'] == np.array([0, 1, 2, 3, 4, 5])).all())
+        self.assertTrue((x.df_population['test_attr'] == np.array([10, 10, 10, 10, 10, 10])).all())
+        self.assertTrue((np.nan_to_num(x.df_population['test_attr2'], 0.) == np.array([0., 0., 0., 0., 0., 0.])).all())
+        self.assertEqual(x.df_population.shape, (6, 4))
+
+        x.add_agents({'age': [3, 4], 'test_attr2': 3.})
+        self.assertTrue((x.df_population['age'] == np.array([1, 2, 3, 4, 1, 17, 3, 4])).all())
+        self.assertTrue((x.df_population['col_id'] == np.array([0, 1, 2, 3, 4, 5, 6, 7])).all())
+        self.assertTrue((x.df_population['test_attr'] == np.array([10, 10, 10, 10, 10, 10, 10, 10])).all())
+        self.assertTrue((np.nan_to_num(x.df_population['test_attr2'], 0.) == np.array([0., 0., 0., 0., 0., 0., 3., 3.])).all())
+        self.assertEqual(x.df_population.shape, (8, 4))
+
+        with self.assertRaises(ValueError):
+            x.add_agents({'age': [1, 2], 'test_attr': [4, 5, 6]})
+
+    def test_count_agents_per_vertex(self):
+        class FakeGraph:
+            weights = np.array([0, 0, 0, 0, 0])
+        x = BaseAgingAgent(graph=FakeGraph())
+        x.add_attribute('position', def_value=0)
+        x.add_agents({'age': 0, 'position': [0, 0, 0, 1, 1, 3, 4, 3, 2, 0, 2]})
+
+        count_all = x.count_pop_per_vertex()
+
+        self.assertEqual(count_all.sum(), 11)
+        self.assertTrue((count_all == np.array([4, 2, 2, 2, 1])).all())
+
+        with self.assertRaises(ValueError):
+            condition = np.array([True, False])
+            x.count_pop_per_vertex(condition=condition)
+
+        with self.assertRaises(ValueError):
+            condition = np.array([0, 0, 0, 1, 1, 3, 4, 3, 2, 0, 2])
+            x.count_pop_per_vertex(condition=condition)
+
+        with self.assertRaises(ValueError):
+            condition = np.array([[0, 0, 0, 1, 1, 3, 4, 3, 2, 0, 2]])
+            x.count_pop_per_vertex(condition=condition)
+
+        with self.assertRaises(ValueError):
+            condition = {}
+            x.count_pop_per_vertex(condition=condition)
+
+        condition = np.array([False, False, False, True, True, True, True, True, True, False, True])
+        count_cond = x.count_pop_per_vertex(condition=condition)
+
+        self.assertEqual(count_cond.sum(), 7)
+        self.assertTrue((count_cond == np.array([0, 2, 2, 2, 1])).all())
+
+
+class TestMovementTerritorialMovementWithoutResistance(unittest.TestCase):
+    pass
+
+
+class TestBuiltInAgentBasicMammal(unittest.TestCase):
+    def test_object_creation(self):
+        with self.assertRaises(ValueError):
+            x = BasicMammal()
         list_expected_col = ['col_id', 'age', 'position', 'territory', 'gender', 'mom_id', 'dad_id', 'is_pregnant']
```

### Comparing `sampy-abm-1.0.2/tests/test_disease_single_species.py` & `sampy_abm-1.0.3/tests/test_disease_single_species.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-import numpy as np
-import unittest
-
-from sampy.pandas_xs.pandas_xs import DataFrameXS
-from sampy.utils.decorators import use_debug_mode
-from sampy.disease.single_species.jit_compiled_functions import (conditional_count_return_full_array,
-                                                                 base_conditional_count_nb_agent_per_vertex,
-                                                                 base_contaminate_vertices,
-                                                                 transition_initialize_counters_of_newly_infected,
-                                                                 transition_conditional_count_nb_agent_per_vertex,
-                                                                 transition_falsify_when_condition)
-
-
-use_debug_mode(DataFrameXS)
-
-
-class TestJitCompiledFuncSingleSpeciesDisease(unittest.TestCase):
-    def test_conditional_count_return_full_array(self):
-        nb_vertex = 5
-        arr_pos = np.array([1, 1, 2, 2, 3, 3, 3, 4, 4])
-        condition = np.array([False, False, True, True, True, False, True, False, True])
-        count = conditional_count_return_full_array(nb_vertex, arr_pos, condition)
-        self.assertTrue((count == np.array([0, 0, 2, 2, 2, 2, 2, 1, 1])).all())
-
-    def test_base_conditional_count_nb_agent_per_vertex(self):
-        nb_vertex = 5
-        arr_pos = np.array([1, 1, 2, 2, 3, 3, 3, 4, 4])
-        condition = np.array([False, False, True, True, True, False, True, False, True])
-        count = base_conditional_count_nb_agent_per_vertex(condition, arr_pos, nb_vertex)
-        self.assertTrue((count == np.array([0, 0, 2, 2, 1])).all())
-
-    def test_base_contaminate_vertices(self):
-        new_infected = np.array([True, True, False, False])
-        rand = np.array([0.1, 0.2, 0.05, 0.4])
-        level = 0.15
-        base_contaminate_vertices(new_infected, rand, level)
-        self.assertTrue((new_infected == np.array([True, False, False, False])).all())
-
-    def test_transition_initialize_counters_of_newly_infected(self):
-        new_infected = np.array([True, False, True, False])
-        counts = np.array([0, 17, 3, 14])
-        new_counts = np.array([4, 8])
-        transition_initialize_counters_of_newly_infected(new_infected, counts, new_counts)
-        self.assertTrue((counts == np.array([4, 17, 8, 14])).all())
-
-    def test_transition_conditional_count_nb_agent_per_vertex(self):
-        nb_vertex = 5
-        arr_pos = np.array([1, 1, 2, 2, 3, 3, 3, 4, 4])
-        condition = np.array([False, False, True, True, True, False, True, False, True])
-        count = transition_conditional_count_nb_agent_per_vertex(condition, arr_pos, nb_vertex)
-        self.assertTrue((count == np.array([0, 0, 2, 2, 1])).all())
-
-    def test_transition_falsify_when_condition(self):
-        to_falsify = np.array([True, True, False, False, True])
-        condition = np.array([True, False, True, False, False, False])
-        transition_falsify_when_condition(to_falsify, condition)
-        self.assertTrue((to_falsify == np.array([False, True, False, False, True])).all())
+import numpy as np
+import unittest
+
+from sampy.pandas_xs.pandas_xs import DataFrameXS
+from sampy.utils.decorators import use_debug_mode
+from sampy.disease.single_species.jit_compiled_functions import (conditional_count_return_full_array,
+                                                                 base_conditional_count_nb_agent_per_vertex,
+                                                                 base_contaminate_vertices,
+                                                                 transition_initialize_counters_of_newly_infected,
+                                                                 transition_conditional_count_nb_agent_per_vertex,
+                                                                 transition_falsify_when_condition)
+
+
+use_debug_mode(DataFrameXS)
+
+
+class TestJitCompiledFuncSingleSpeciesDisease(unittest.TestCase):
+    def test_conditional_count_return_full_array(self):
+        nb_vertex = 5
+        arr_pos = np.array([1, 1, 2, 2, 3, 3, 3, 4, 4])
+        condition = np.array([False, False, True, True, True, False, True, False, True])
+        count = conditional_count_return_full_array(nb_vertex, arr_pos, condition)
+        self.assertTrue((count == np.array([0, 0, 2, 2, 2, 2, 2, 1, 1])).all())
+
+    def test_base_conditional_count_nb_agent_per_vertex(self):
+        nb_vertex = 5
+        arr_pos = np.array([1, 1, 2, 2, 3, 3, 3, 4, 4])
+        condition = np.array([False, False, True, True, True, False, True, False, True])
+        count = base_conditional_count_nb_agent_per_vertex(condition, arr_pos, nb_vertex)
+        self.assertTrue((count == np.array([0, 0, 2, 2, 1])).all())
+
+    def test_base_contaminate_vertices(self):
+        new_infected = np.array([True, True, False, False])
+        rand = np.array([0.1, 0.2, 0.05, 0.4])
+        level = 0.15
+        base_contaminate_vertices(new_infected, rand, level)
+        self.assertTrue((new_infected == np.array([True, False, False, False])).all())
+
+    def test_transition_initialize_counters_of_newly_infected(self):
+        new_infected = np.array([True, False, True, False])
+        counts = np.array([0, 17, 3, 14])
+        new_counts = np.array([4, 8])
+        transition_initialize_counters_of_newly_infected(new_infected, counts, new_counts)
+        self.assertTrue((counts == np.array([4, 17, 8, 14])).all())
+
+    def test_transition_conditional_count_nb_agent_per_vertex(self):
+        nb_vertex = 5
+        arr_pos = np.array([1, 1, 2, 2, 3, 3, 3, 4, 4])
+        condition = np.array([False, False, True, True, True, False, True, False, True])
+        count = transition_conditional_count_nb_agent_per_vertex(condition, arr_pos, nb_vertex)
+        self.assertTrue((count == np.array([0, 0, 2, 2, 1])).all())
+
+    def test_transition_falsify_when_condition(self):
+        to_falsify = np.array([True, True, False, False, True])
+        condition = np.array([True, False, True, False, False, False])
+        transition_falsify_when_condition(to_falsify, condition)
+        self.assertTrue((to_falsify == np.array([False, True, False, False, True])).all())
```

### Comparing `sampy-abm-1.0.2/tests/test_disease_two_species.py` & `sampy_abm-1.0.3/tests/test_disease_two_species.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import numpy as np
-import unittest
-
-from sampy.pandas_xs.pandas_xs import DataFrameXS
-from sampy.utils.decorators import use_debug_mode
-from sampy.disease.two_species.jit_compiled_functions import base_contaminate_vertices
-
-use_debug_mode(DataFrameXS)
-
-
-class TestJitCompiledFuncTwoSpeciesDisease(unittest.TestCase):
-    def test_base_contaminate_vertices(self):
-        new_infected = np.array([True, True, False, False])
-        rand = np.array([0.1, 0.2, 0.05, 0.4])
-        level = 0.15
-        base_contaminate_vertices(new_infected, rand, level)
-        self.assertTrue((new_infected == np.array([True, False, False, False])).all())
+import numpy as np
+import unittest
+
+from sampy.pandas_xs.pandas_xs import DataFrameXS
+from sampy.utils.decorators import use_debug_mode
+from sampy.disease.two_species.jit_compiled_functions import base_contaminate_vertices
+
+use_debug_mode(DataFrameXS)
+
+
+class TestJitCompiledFuncTwoSpeciesDisease(unittest.TestCase):
+    def test_base_contaminate_vertices(self):
+        new_infected = np.array([True, True, False, False])
+        rand = np.array([0.1, 0.2, 0.05, 0.4])
+        level = 0.15
+        base_contaminate_vertices(new_infected, rand, level)
+        self.assertTrue((new_infected == np.array([True, False, False, False])).all())
```

### Comparing `sampy-abm-1.0.2/tests/test_pandas_xs.py` & `sampy_abm-1.0.3/tests/test_pandas_xs.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,579 +1,579 @@
-import sampy
-import numpy as np
-import unittest
-import warnings
-warnings.filterwarnings("ignore", message="numpy.dtype size changed")
-warnings.filterwarnings("ignore", message="numpy.ufunc size changed")
-
-sampy.use_debug_mode(sampy.DataFrameXS)
-
-
-class TestSetItemsPandasXS(unittest.TestCase):
-    def setUp(self):
-        self.df = sampy.DataFrameXS()
-
-    def test_key_empty(self):
-        with self.assertRaises(ValueError) as cm:
-            self.df[None] = None
-        self.assertEqual(str(cm.exception), "A column name should be a string in a dataframe_xs.")
-
-    def test_key_int(self):
-        with self.assertRaises(ValueError) as cm:
-            self.df[1] = None
-        self.assertEqual(str(cm.exception), "A column name should be a string in a dataframe_xs.")
-
-    def test_key_float(self):
-        with self.assertRaises(ValueError) as cm:
-            self.df[1.] = None
-        self.assertEqual(str(cm.exception), "A column name should be a string in a dataframe_xs.")
-
-    def test_key_list(self):
-        with self.assertRaises(ValueError) as cm:
-            self.df[[]] = None
-        self.assertEqual(str(cm.exception), "A column name should be a string in a dataframe_xs.")
-
-    def test_key_dict(self):
-        with self.assertRaises(ValueError) as cm:
-            self.df[{}] = None
-        self.assertEqual(str(cm.exception), "A column name should be a string in a dataframe_xs.")
-
-    def test_key_array_of_a_single_str(self):
-        with self.assertRaises(ValueError) as cm:
-            self.df[np.array('abc')] = None
-        self.assertEqual(str(cm.exception), "A column name should be a string in a dataframe_xs.")
-
-    def test_add_first_column_as_empty_list(self):
-        self.df['1'] = []
-        self.assertEqual(self.df.shape, (0, 1))
-        self.assertIsNone(self.df.list_col[0])
-
-    def test_add_first_column_as_list(self):
-        self.df['test'] = [1, 2, 3, 4]
-        with self.subTest():
-            self.assertEqual(len(self.df.list_col), 1)
-
-        with self.subTest():
-            self.assertEqual(self.df.nb_cols, 1)
-
-        with self.subTest():
-            self.assertEqual(self.df.nb_rows, 4)
-
-        with self.subTest():
-            self.assertTrue( 'test' in self.df.dict_colname_to_index )
-            self.assertEqual(self.df.dict_colname_to_index['test'], 0)
-            self.assertTrue((self.df.list_col[0] == np.array([1, 2, 3, 4])).all())
-
-        with self.subTest():
-            self.assertEqual(str(self.df.list_col[0].dtype), 'int32')
-
-    def test_add_first_column_as_array(self):
-        self.df['test'] = np.array([1, 2, 3, 4])
-
-        with self.subTest():
-            self.assertEqual(len(self.df.list_col), 1)
-
-        with self.subTest():
-            self.assertEqual(self.df.nb_cols, 1)
-
-        with self.subTest():
-            self.assertEqual(self.df.nb_rows, 4)
-
-        with self.subTest():
-            self.assertTrue( 'test' in self.df.dict_colname_to_index )
-            self.assertEqual(self.df.dict_colname_to_index['test'], 0)
-            self.assertTrue((self.df.list_col[0] == np.array([1, 2, 3, 4])).all())
-
-        with self.subTest():
-            self.assertEqual(str(self.df.list_col[0].dtype), 'int32')
-
-    def test_value_is_a_dict(self):
-        with self.assertRaises(ValueError) as cm:
-            self.df['test'] = {}
-        self.assertEqual(str(cm.exception), "The proposed column is of an unsupported type. Supported types are " +
-                         str(self.df.LIST_ALLOWED_TYPE))
-
-    def test_value_is_list_of_string(self):
-        with self.assertRaises(ValueError) as cm:
-            self.df['test'] = ['abc', 'def']
-        self.assertEqual(str(cm.exception), "The proposed column is of an unsupported type. Supported types are " +
-                         str(self.df.LIST_ALLOWED_TYPE))
-
-    def test_value_is_arr_complex(self):
-        with self.assertRaises(ValueError) as cm:
-            self.df['test'] = np.array([1, 2, 3, 4, 5], dtype=np.complex_)
-        self.assertEqual(str(cm.exception), "The proposed column is of an unsupported type. Supported types are " +
-                         str(self.df.LIST_ALLOWED_TYPE))
-
-    def test_add_wrong_col_on_non_empty_df(self):
-        self.df['1'] = [1, 2]
-        with self.subTest():
-            with self.assertRaises(ValueError) as cm:
-                self.df['test'] = ['abc', 'def']
-            self.assertEqual(str(cm.exception), "The proposed column is of an unsupported type. Supported types are " +
-                             str(self.df.LIST_ALLOWED_TYPE))
-        with self.subTest():
-            with self.assertRaises(ValueError) as cm:
-                self.df['test'] = np.array([1, 2], dtype=np.complex_)
-            self.assertEqual(str(cm.exception), "The proposed column is of an unsupported type. Supported types are " +
-                             str(self.df.LIST_ALLOWED_TYPE))
-        with self.subTest():
-            with self.assertRaises(ValueError) as cm:
-                self.df['test'] = {}
-            self.assertEqual(str(cm.exception), "The proposed column is of an unsupported type. Supported types are " +
-                             str(self.df.LIST_ALLOWED_TYPE))
-
-    def test_add_new_column_of_wrong_length(self):
-        self.df['1'] = [1, 2, 3, 4]
-        with self.subTest():
-            with self.assertRaises(ValueError) as cm:
-                self.df['2'] = [1, 2, 3]
-            self.assertEqual(str(cm.exception), "Dataframe has " + str(self.df.nb_rows) + " rows while the input has 3.")
-        with self.subTest():
-            with self.assertRaises(ValueError) as cm:
-                self.df['2'] = [1, 2, 3, 4, 5]
-            self.assertEqual(str(cm.exception),
-                             "Dataframe has " + str(self.df.nb_rows) + " rows while the input has 5.")
-
-    def test_add_empty_column(self):
-        self.df['1'] = [1, 2, 3, 4]
-        self.df['test'] = None
-        with self.subTest():
-            self.assertEqual(self.df.nb_rows, 4)
-        with self.subTest():
-            self.assertEqual(self.df.nb_cols, 2)
-        with self.subTest():
-            self.assertIn('test', self.df.dict_colname_to_index)
-            self.assertEqual(self.df.dict_colname_to_index['test'], 1)
-            self.assertIsNone(self.df.list_col[1])
-
-    def test_add_column_by_single_value(self):
-        self.df['1'] = [1, 2, 3, 4]
-        self.df['2'] = True
-        self.assertEqual(self.df.list_col[self.df.dict_colname_to_index['2']].shape, (4,))
-        self.assertEqual(str(self.df.list_col[self.df.dict_colname_to_index['2']].dtype), 'bool')
-        self.assertTrue(self.df.list_col[1].all())
-
-    def test_add_column_as_empty_list(self):
-        self.df['1'] = [1, 2, 3, 4]
-        self.df['2'] = []
-        self.assertEqual(self.df.shape, (4, 2))
-        self.assertIsNone(self.df.list_col[1])
-
-    def test_add_column_as_empty_tuple(self):
-        self.df['1'] = [1, 2, 3, 4]
-        self.df['2'] = tuple()
-        self.assertEqual(self.df.shape, (4, 2))
-        self.assertIsNone(self.df.list_col[1])
-
-    def test_add_column_as_list_of_int(self):
-        self.df['1'] = [1, 2, 3]
-        self.df['2'] = [4, 5, 6]
-        self.assertEqual(self.df.shape, (3, 2))
-        self.assertTrue((self.df.list_col[self.df.dict_colname_to_index['2']] == np.array([4, 5, 6])).all())
-
-    def test_is_empty(self):
-        self.assertTrue(self.df.is_empty)
-        self.df['1'] = None
-        self.assertTrue(self.df.is_empty)
-        self.df['2'] = [1, 2, 3]
-        self.assertFalse(self.df.is_empty)
-        self.df['2'] = None
-        self.assertTrue(self.df.is_empty)
-
-    def test_shape(self):
-        self.assertEqual(self.df.shape, (0, 0))
-        self.df['1'] = None
-        self.assertEqual(self.df.shape, (0, 1))
-        self.df['2'] = [1, 2, 3]
-        self.assertEqual(self.df.shape, (3, 2))
-        self.df['2'] = None
-        self.assertEqual(self.df.shape, (0, 2))
-
-
-class TestGetItemsPandasXS(unittest.TestCase):
-    def setUp(self):
-        self.df = sampy.DataFrameXS()
-        self.df['col1'] = [1, 2, 3, 4]
-        self.df['col2'] = [2., 3., 4., 5.]
-
-    def test_check_cols_are_retrieved_correctly(self):
-        self.assertTrue((self.df['col1'] == np.array([1, 2, 3, 4])).all())
-        self.assertTrue((self.df['col2'] == np.array([2., 3., 4., 5.])).all())
-        self.assertFalse((self.df['col1'] == self.df['col2']).all())
-        self.assertTrue(str(self.df['col1'].dtype).startswith('int'))
-
-    def test_getitems_returns_ref(self):
-        self.df['col1'][0] = 0
-        self.assertTrue((self.df['col1'] == np.array([0, 2, 3, 4])).all())
-
-    def test_bool_arr_indexing(self):
-        arr_bool = np.array([True, False, True, False])
-        df = self.df[arr_bool]
-        self.assertEqual(df.nb_rows, 2)
-        self.assertEqual(df.nb_cols, 2)
-        self.assertEqual(df.list_col_name, self.df.list_col_name)
-        self.assertTrue((df['col1'] == np.array([1, 3])).all())
-        self.assertTrue((df['col2'] == np.array([2., 4.])).all())
-
-    def test_int_arr_indexing(self):
-        arr_int = np.array([2, 0, 1, 3])
-        df = self.df[arr_int]
-        self.assertEqual(df.nb_rows, 4)
-        self.assertEqual(df.nb_cols, 2)
-        self.assertEqual(df.list_col_name, self.df.list_col_name)
-        self.assertTrue((df['col1'] == np.array([3, 1, 2, 4])).all())
-        self.assertTrue((df['col2'] == np.array([4., 2., 3., 5.])).all())
-        self.assertFalse((df['col1'] == df['col2']).all())
-        self.assertTrue(str(df['col1'].dtype).startswith('int'))
-
-    def test_wrong_indexing(self):
-        with self.subTest():
-            with self.assertRaises(TypeError) as cm:
-                self.df[{}]
-        with self.subTest():
-            with self.assertRaises(TypeError) as cm:
-                self.df[1]
-        with self.subTest():
-            with self.assertRaises(TypeError) as cm:
-                self.df[[True, True, False]]
-        with self.subTest():
-            with self.assertRaises(TypeError) as cm:
-                self.df[np.array([1., 2., 3., 4.])]
-        with self.subTest():
-            with self.assertRaises(KeyError) as cm:
-                self.df['wrong_col_name']
-        with self.subTest():
-            with self.assertRaises(IndexError) as cm:
-                self.df[np.array([True, True, False])]
-        with self.subTest():
-            with self.assertRaises(IndexError) as cm:
-                self.df[np.array([True, True, False, False, False])]
-        with self.subTest():
-            with self.assertRaises(IndexError) as cm:
-                self.df[np.array([0, 5])]
-
-
-class TestGenericMethodsPandasXS(unittest.TestCase):
-    def setUp(self):
-        self.df = sampy.DataFrameXS()
-        self.df['col1'] = [1, 2, 3, 4]
-        self.df['col2'] = [2., 3., 4., 5.]
-
-    def test_scramble(self):
-        with self.assertRaises(ValueError):
-            self.df.scramble(permutation=np.array([2, 0, 1]))
-        with self.assertRaises(TypeError):
-            self.df.scramble(permutation=[2, 0, 1, 3])
-        with self.assertRaises(ValueError):
-            self.df.scramble(permutation=np.array([2, 0, 1, 4]))
-        with self.assertRaises(ValueError):
-            self.df.scramble(permutation=np.array([[2, 0, 1, 4]]))
-        with self.assertRaises(TypeError):
-            self.df.scramble(permutation=np.array([]))
-        with self.assertRaises(ValueError):
-            self.df.scramble(permutation=np.array(0))
-        perm = np.array([2, 0, 1, 3])
-        self.df.scramble(permutation=perm)
-        self.assertEqual(self.df.nb_rows, 4)
-        self.assertEqual(self.df.nb_cols, 2)
-        self.assertEqual(self.df.list_col_name, ['col1', 'col2'])
-        self.assertTrue((self.df['col1'] == np.array([3, 1, 2, 4])).all())
-        self.assertTrue((self.df['col2'] == np.array([4., 2., 3., 5.])).all())
-        self.assertFalse((self.df['col1'] == self.df['col2']).all())
-        self.assertTrue(str(self.df['col1'].dtype).startswith('int'))
-
-    def test_get_copy(self):
-        with self.assertRaises(KeyError):
-            self.df.get_copy('wrong_col_name')
-
-        with self.assertRaises(TypeError):
-            self.df.get_copy([])
-
-        with self.assertRaises(TypeError):
-            self.df.get_copy(1)
-
-        u = self.df.get_copy('col1')
-        self.assertTrue((u == self.df['col1']).all())
-        u[0] = 0
-        self.assertFalse((u == self.df['col1']).all())
-
-    def test_check_arr_in_col(self):
-        with self.subTest():
-            with self.assertRaises(ValueError):
-                input_arr = np.array([1., 2., 3., 4.])
-                self.df.check_arr_in_col(input_arr, 'col1')
-        with self.subTest():
-            with self.assertRaises(ValueError):
-                input_arr = np.array([1, 2, 3, 4])
-                self.df.check_arr_in_col(input_arr, 'col2')
-        with self.subTest():
-            with self.assertRaises(ValueError):
-                input_arr = np.array([[1., 2.], [3., 4.]])
-                self.df.check_arr_in_col(input_arr, 'col2')
-        with self.subTest():
-            with self.assertRaises(ValueError):
-                input_arr = np.array(2.)
-                self.df.check_arr_in_col(input_arr, 'col2')
-        with self.subTest():
-            with self.assertRaises(ValueError):
-                input_arr = np.array(2.)
-                self.df.check_arr_in_col(input_arr, 'col2')
-        with self.subTest():
-            input_arr = np.array([3, 4, 8, 0, 10, 1])
-            input_arr = input_arr.astype('int8')
-            with self.assertRaises(ValueError):
-                result = self.df.check_arr_in_col(input_arr, 'col1')
-        with self.subTest():
-            input_arr = np.array([3, 4, 8, 0, 10, 1])
-            result = self.df.check_arr_in_col(input_arr, 'col1')
-            self.assertTrue((result == np.array([True, True, False, False, False, True])).all())
-
-    def test_check_arr_in_col_conditional(self):
-        with self.subTest():
-            with self.assertRaises(ValueError):
-                condition = np.array([True, True, False, False])
-                input_arr = np.array([1., 2., 3., 4.])
-                self.df.check_arr_in_col(input_arr, 'col1', condition=condition)
-        with self.subTest():
-            with self.assertRaises(ValueError):
-                condition = np.array([True, True, False, False])
-                input_arr = np.array([1, 2, 3, 4])
-                self.df.check_arr_in_col(input_arr, 'col2', condition=condition)
-        with self.subTest():
-            with self.assertRaises(ValueError):
-                condition = np.array([[True, True], [False, False]])
-                input_arr = np.array([[1., 2.], [3., 4.]])
-                self.df.check_arr_in_col(input_arr, 'col2', condition=condition)
-        with self.subTest():
-            with self.assertRaises(ValueError):
-                condition = np.array([True])
-                input_arr = np.array(2.)
-                self.df.check_arr_in_col(input_arr, 'col2', condition=condition)
-        with self.subTest():
-            with self.assertRaises(ValueError):
-                condition = np.array([True])
-                input_arr = np.array({})
-                self.df.check_arr_in_col(input_arr, 'col2', condition=condition)
-        with self.subTest():
-            condition = np.array([True, False, False, True, True, True])
-            input_arr = np.array([3, 4, 8, 0, 10, 1])
-            input_arr = input_arr.astype('int8')
-            with self.assertRaises(ValueError):
-                self.df.check_arr_in_col(input_arr, 'col1', condition=condition)
-        with self.subTest():
-            condition = np.array([True, False, False, True, True, True])
-            input_arr = np.array([3, 4, 8, 0, 10, 1])
-            result = self.df.check_arr_in_col(input_arr, 'col1', condition=condition)
-            self.assertTrue((result == np.array([True, False, False, False, False, True])).all())
-        with self.subTest():
-            condition = np.array([True, False, False, True, True])
-            input_arr = np.array([3, 4, 8, 0, 10, 1])
-            with self.assertRaises(ValueError):
-                self.df.check_arr_in_col(input_arr, 'col1', condition=condition)
-        with self.subTest():
-            condition = np.array([1, 0, 0, 1, 1, 1])
-            input_arr = np.array([3, 4, 8, 0, 10, 1])
-            with self.assertRaises(ValueError):
-                self.df.check_arr_in_col(input_arr, 'col1', condition=condition)
-        with self.subTest():
-            condition = {}
-            input_arr = np.array([3, 4, 8, 0, 10, 1])
-            with self.assertRaises(ValueError):
-                self.df.check_arr_in_col(input_arr, 'col1', condition=condition)
-        with self.subTest():
-            condition = np.array([[True, False], [False, True], [True, True]])
-            input_arr = np.array([3, 4, 8, 0, 10, 1])
-            with self.assertRaises(ValueError):
-                self.df.check_arr_in_col(input_arr, 'col1', condition=condition)
-
-    def test_concat_inplace_is_false(self):
-        with self.subTest():
-            df = sampy.DataFrameXS()
-            df['col1'] = [5, 6, 7, 8]
-            df['col2'] = [6., 7., 8., 9.]
-            c_df = self.df.concat(df, inplace=False)
-
-            # concats happened as expected
-            self.assertTrue((c_df['col1'] == np.array([1, 2, 3, 4, 5, 6, 7, 8])).all())
-            self.assertTrue((c_df['col2'] == np.array([2., 3., 4., 5., 6., 7., 8., 9.])).all())
-
-            # columns are new copied columns
-            c_df['col1'][0] = 0
-            self.assertFalse(c_df['col1'][0] == self.df['col1'][0])
-
-        with self.subTest():
-            # same test as the previous one, but there is an extra column
-            df = sampy.DataFrameXS()
-            df['col1'] = [5, 6, 7, 8]
-            df['col2'] = [6., 7., 8., 9.]
-            df['col3'] = [1, 2, 3, 4]
-            c_df = self.df.concat(df, inplace=False)
-
-            # check that there is no col3 in the dataframe
-            with self.assertRaises(KeyError):
-                c_df['col3']
-
-            # perform all the previous checks in this case.
-            # concat happened as expected
-            self.assertTrue((c_df['col1'] == np.array([1, 2, 3, 4, 5, 6, 7, 8])).all())
-            self.assertTrue((c_df['col2'] == np.array([2., 3., 4., 5., 6., 7., 8., 9.])).all())
-
-            # columns are new copied columns
-            c_df['col1'][0] = 0
-            self.assertFalse(c_df['col1'][0] == self.df['col1'][0])
-
-        # check that an error is raised when the df don't have the right col_names
-        with self.subTest():
-            df = sampy.DataFrameXS()
-            df['col1'] = [5, 6, 7, 8]
-            df['col3'] = [6., 7., 8., 9.]
-            with self.assertRaises(KeyError):
-                self.df.concat(df, inplace=False)
-
-        # check that appending with an empty dataframe returns a copy
-        with self.subTest():
-            df = sampy.DataFrameXS()
-            c_df = self.df.concat(df, inplace=False)
-            self.assertTrue((c_df['col1'] == self.df['col1']).all())
-            self.assertTrue((c_df['col2'] == self.df['col2']).all())
-
-            c_df['col1'][0] = 0
-            self.assertFalse(c_df['col1'][0] == self.df['col1'][0])
-
-        # check that having a null column in the input is correctly dealt with
-        with self.subTest():
-            df = sampy.DataFrameXS()
-            df['col1'] = [5, 6, 7, 8]
-            df['col2'] = None
-            c_df = self.df.concat(df, inplace=False)
-            self.assertTrue((c_df['col1'] == np.array([1, 2, 3, 4, 5, 6, 7, 8])).all())
-            self.assertTrue((np.nan_to_num(c_df['col2'], nan=0.) == np.array([2., 3., 4., 5., 0., 0., 0., 0.])).all())
-            self.assertEqual(str(c_df['col2'].dtype), str(self.df['col2'].dtype))
-
-        # same thing but in reverse
-        with self.subTest():
-            df_in = sampy.DataFrameXS()
-            df_in['col1'] = [1, 2, 3, 4]
-            df_in['col2'] = None
-
-            df = sampy.DataFrameXS()
-            df['col1'] = [5, 6, 7, 8]
-            df['col2'] = [6., 7., 8., 9.]
-            c_df = df_in.concat(df, inplace=False)
-            self.assertTrue((c_df['col1'] == np.array([1, 2, 3, 4, 5, 6, 7, 8])).all())
-            self.assertTrue((np.nan_to_num(c_df['col2'], 0.) == np.array([0., 0., 0., 0., 6., 7., 8., 9.])).all())
-            self.assertEqual(str(c_df['col2'].dtype), str(df['col2'].dtype))
-
-        # When the first df is empty
-        with self.subTest():
-            df_in = sampy.DataFrameXS()
-            df_in['col1'] = None
-            df_in['col2'] = None
-
-            df = sampy.DataFrameXS()
-            df['col1'] = [5, 6, 7, 8]
-            df['col2'] = [6., 7., 8., 9.]
-            c_df = df_in.concat(df, inplace=False)
-
-            self.assertTrue((c_df['col1'] == np.array([5, 6, 7, 8])).all())
-            self.assertEqual(str(c_df['col1'].dtype), str(df['col1'].dtype))
-            self.assertTrue((np.nan_to_num(c_df['col2'], nan=0.) == np.array([6., 7., 8., 9.])).all())
-            self.assertEqual(str(c_df['col2'].dtype), str(df['col2'].dtype))
-
-            # check that a copy is retrieved
-            c_df['col1'][0] = 0
-            self.assertFalse((c_df['col1'] == df['col1']).all())
-
-        # adding an empty column on an empty column
-        with self.subTest():
-            df_in = sampy.DataFrameXS()
-            df_in['col1'] = [1, 2, 3, 4]
-            df_in['col2'] = None
-
-            df = sampy.DataFrameXS()
-            df['col1'] = [5, 6, 7, 8]
-            df['col2'] = None
-
-            c_df = df_in.concat(df, inplace=False)
-
-            self.assertIsNone(c_df['col2'])
-            self.assertTrue((c_df['col1'] == np.array([1, 2, 3, 4, 5, 6, 7, 8])).all())
-            self.assertEqual(str(c_df['col1'].dtype), str(df['col1'].dtype))
-
-    def test_concat_inplace_is_true_basic(self):
-        df = sampy.DataFrameXS()
-        df['col1'] = [5, 6, 7, 8]
-        df['col2'] = [6., 7., 8., 9.]
-        self.df.concat(df, inplace=True)
-
-        # concats happened as expected
-        self.assertTrue((self.df['col1'] == np.array([1, 2, 3, 4, 5, 6, 7, 8])).all())
-        self.assertTrue((self.df['col2'] == np.array([2., 3., 4., 5., 6., 7., 8., 9.])).all())
-
-    def test_concat_inplace_is_true_extra_col(self):
-        df = sampy.DataFrameXS()
-        df['col1'] = [5, 6, 7, 8]
-        df['col2'] = [6., 7., 8., 9.]
-        df['col3'] = [1, 2, 3, 4]
-        self.df.concat(df, inplace=True)
-
-        # check that there is no col3 in the dataframe
-        with self.assertRaises(KeyError):
-            self.df['col3']
-
-        # perform all the previous checks in this case.
-        # concat happened as expected
-        self.assertTrue((self.df['col1'] == np.array([1, 2, 3, 4, 5, 6, 7, 8])).all())
-        self.assertTrue((self.df['col2'] == np.array([2., 3., 4., 5., 6., 7., 8., 9.])).all())
-        self.assertEqual(self.df.nb_rows, 8)
-
-    def test_concat_inplace_is_true_wrong_col_name(self):
-        df = sampy.DataFrameXS()
-        df['col1'] = [5, 6, 7, 8]
-        df['col3'] = [6., 7., 8., 9.]
-        with self.assertRaises(KeyError):
-            self.df.concat(df, inplace=True)
-
-    def test_concat_inplace_is_true_empty_col_on_empty_col(self):
-        self.df['col2'] = None
-
-        df = sampy.DataFrameXS()
-        df['col1'] = [5, 6, 7, 8]
-        df['col2'] = None
-
-        self.df.concat(df, inplace=True)
-
-        self.assertIsNone(self.df['col2'])
-        self.assertTrue((self.df['col1'] == np.array([1, 2, 3, 4, 5, 6, 7, 8])).all())
-        self.assertEqual(str(self.df['col1'].dtype), str(df['col1'].dtype))
-
-    def test_concat_inplace_is_true_empty_col_in_input(self):
-        df = sampy.DataFrameXS()
-        df['col1'] = [5, 6, 7, 8]
-        df['col2'] = None
-
-        self.df.concat(df, inplace=True)
-
-        self.assertTrue((np.nan_to_num(self.df['col2'], nan=0.) == np.array([2., 3., 4., 5., 0., 0., 0., 0.])).all())
-        self.assertTrue((self.df['col1'] == np.array([1, 2, 3, 4, 5, 6, 7, 8])).all())
-        self.assertEqual(str(self.df['col1'].dtype), str(df['col1'].dtype))
-
-    def test_concat_inplace_is_true_on_empty_df(self):
-        self.df['col1'] = None
-        self.df['col2'] = None
-
-        df = sampy.DataFrameXS()
-        df['col1'] = [5, 6, 7, 8]
-        df['col2'] = [6., 7., 8., 9.]
-        self.df.concat(df, inplace=True)
-
-        self.assertTrue((self.df['col1'] == np.array([5, 6, 7, 8])).all())
-        self.assertEqual(str(self.df['col1'].dtype), str(df['col1'].dtype))
-        self.assertTrue((np.nan_to_num(self.df['col2'], nan=0.) == np.array([6., 7., 8., 9.])).all())
-        self.assertEqual(str(self.df['col2'].dtype), str(df['col2'].dtype))
-
-        self.assertEqual(self.df.nb_rows, 4)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import sampy
+import numpy as np
+import unittest
+import warnings
+warnings.filterwarnings("ignore", message="numpy.dtype size changed")
+warnings.filterwarnings("ignore", message="numpy.ufunc size changed")
+
+sampy.use_debug_mode(sampy.DataFrameXS)
+
+
+class TestSetItemsPandasXS(unittest.TestCase):
+    def setUp(self):
+        self.df = sampy.DataFrameXS()
+
+    def test_key_empty(self):
+        with self.assertRaises(ValueError) as cm:
+            self.df[None] = None
+        self.assertEqual(str(cm.exception), "A column name should be a string in a dataframe_xs.")
+
+    def test_key_int(self):
+        with self.assertRaises(ValueError) as cm:
+            self.df[1] = None
+        self.assertEqual(str(cm.exception), "A column name should be a string in a dataframe_xs.")
+
+    def test_key_float(self):
+        with self.assertRaises(ValueError) as cm:
+            self.df[1.] = None
+        self.assertEqual(str(cm.exception), "A column name should be a string in a dataframe_xs.")
+
+    def test_key_list(self):
+        with self.assertRaises(ValueError) as cm:
+            self.df[[]] = None
+        self.assertEqual(str(cm.exception), "A column name should be a string in a dataframe_xs.")
+
+    def test_key_dict(self):
+        with self.assertRaises(ValueError) as cm:
+            self.df[{}] = None
+        self.assertEqual(str(cm.exception), "A column name should be a string in a dataframe_xs.")
+
+    def test_key_array_of_a_single_str(self):
+        with self.assertRaises(ValueError) as cm:
+            self.df[np.array('abc')] = None
+        self.assertEqual(str(cm.exception), "A column name should be a string in a dataframe_xs.")
+
+    def test_add_first_column_as_empty_list(self):
+        self.df['1'] = []
+        self.assertEqual(self.df.shape, (0, 1))
+        self.assertIsNone(self.df.list_col[0])
+
+    def test_add_first_column_as_list(self):
+        self.df['test'] = [1, 2, 3, 4]
+        with self.subTest():
+            self.assertEqual(len(self.df.list_col), 1)
+
+        with self.subTest():
+            self.assertEqual(self.df.nb_cols, 1)
+
+        with self.subTest():
+            self.assertEqual(self.df.nb_rows, 4)
+
+        with self.subTest():
+            self.assertTrue( 'test' in self.df.dict_colname_to_index )
+            self.assertEqual(self.df.dict_colname_to_index['test'], 0)
+            self.assertTrue((self.df.list_col[0] == np.array([1, 2, 3, 4])).all())
+
+        with self.subTest():
+            self.assertEqual(str(self.df.list_col[0].dtype), 'int32')
+
+    def test_add_first_column_as_array(self):
+        self.df['test'] = np.array([1, 2, 3, 4])
+
+        with self.subTest():
+            self.assertEqual(len(self.df.list_col), 1)
+
+        with self.subTest():
+            self.assertEqual(self.df.nb_cols, 1)
+
+        with self.subTest():
+            self.assertEqual(self.df.nb_rows, 4)
+
+        with self.subTest():
+            self.assertTrue( 'test' in self.df.dict_colname_to_index )
+            self.assertEqual(self.df.dict_colname_to_index['test'], 0)
+            self.assertTrue((self.df.list_col[0] == np.array([1, 2, 3, 4])).all())
+
+        with self.subTest():
+            self.assertEqual(str(self.df.list_col[0].dtype), 'int32')
+
+    def test_value_is_a_dict(self):
+        with self.assertRaises(ValueError) as cm:
+            self.df['test'] = {}
+        self.assertEqual(str(cm.exception), "The proposed column is of an unsupported type. Supported types are " +
+                         str(self.df.LIST_ALLOWED_TYPE))
+
+    def test_value_is_list_of_string(self):
+        with self.assertRaises(ValueError) as cm:
+            self.df['test'] = ['abc', 'def']
+        self.assertEqual(str(cm.exception), "The proposed column is of an unsupported type. Supported types are " +
+                         str(self.df.LIST_ALLOWED_TYPE))
+
+    def test_value_is_arr_complex(self):
+        with self.assertRaises(ValueError) as cm:
+            self.df['test'] = np.array([1, 2, 3, 4, 5], dtype=np.complex_)
+        self.assertEqual(str(cm.exception), "The proposed column is of an unsupported type. Supported types are " +
+                         str(self.df.LIST_ALLOWED_TYPE))
+
+    def test_add_wrong_col_on_non_empty_df(self):
+        self.df['1'] = [1, 2]
+        with self.subTest():
+            with self.assertRaises(ValueError) as cm:
+                self.df['test'] = ['abc', 'def']
+            self.assertEqual(str(cm.exception), "The proposed column is of an unsupported type. Supported types are " +
+                             str(self.df.LIST_ALLOWED_TYPE))
+        with self.subTest():
+            with self.assertRaises(ValueError) as cm:
+                self.df['test'] = np.array([1, 2], dtype=np.complex_)
+            self.assertEqual(str(cm.exception), "The proposed column is of an unsupported type. Supported types are " +
+                             str(self.df.LIST_ALLOWED_TYPE))
+        with self.subTest():
+            with self.assertRaises(ValueError) as cm:
+                self.df['test'] = {}
+            self.assertEqual(str(cm.exception), "The proposed column is of an unsupported type. Supported types are " +
+                             str(self.df.LIST_ALLOWED_TYPE))
+
+    def test_add_new_column_of_wrong_length(self):
+        self.df['1'] = [1, 2, 3, 4]
+        with self.subTest():
+            with self.assertRaises(ValueError) as cm:
+                self.df['2'] = [1, 2, 3]
+            self.assertEqual(str(cm.exception), "Dataframe has " + str(self.df.nb_rows) + " rows while the input has 3.")
+        with self.subTest():
+            with self.assertRaises(ValueError) as cm:
+                self.df['2'] = [1, 2, 3, 4, 5]
+            self.assertEqual(str(cm.exception),
+                             "Dataframe has " + str(self.df.nb_rows) + " rows while the input has 5.")
+
+    def test_add_empty_column(self):
+        self.df['1'] = [1, 2, 3, 4]
+        self.df['test'] = None
+        with self.subTest():
+            self.assertEqual(self.df.nb_rows, 4)
+        with self.subTest():
+            self.assertEqual(self.df.nb_cols, 2)
+        with self.subTest():
+            self.assertIn('test', self.df.dict_colname_to_index)
+            self.assertEqual(self.df.dict_colname_to_index['test'], 1)
+            self.assertIsNone(self.df.list_col[1])
+
+    def test_add_column_by_single_value(self):
+        self.df['1'] = [1, 2, 3, 4]
+        self.df['2'] = True
+        self.assertEqual(self.df.list_col[self.df.dict_colname_to_index['2']].shape, (4,))
+        self.assertEqual(str(self.df.list_col[self.df.dict_colname_to_index['2']].dtype), 'bool')
+        self.assertTrue(self.df.list_col[1].all())
+
+    def test_add_column_as_empty_list(self):
+        self.df['1'] = [1, 2, 3, 4]
+        self.df['2'] = []
+        self.assertEqual(self.df.shape, (4, 2))
+        self.assertIsNone(self.df.list_col[1])
+
+    def test_add_column_as_empty_tuple(self):
+        self.df['1'] = [1, 2, 3, 4]
+        self.df['2'] = tuple()
+        self.assertEqual(self.df.shape, (4, 2))
+        self.assertIsNone(self.df.list_col[1])
+
+    def test_add_column_as_list_of_int(self):
+        self.df['1'] = [1, 2, 3]
+        self.df['2'] = [4, 5, 6]
+        self.assertEqual(self.df.shape, (3, 2))
+        self.assertTrue((self.df.list_col[self.df.dict_colname_to_index['2']] == np.array([4, 5, 6])).all())
+
+    def test_is_empty(self):
+        self.assertTrue(self.df.is_empty)
+        self.df['1'] = None
+        self.assertTrue(self.df.is_empty)
+        self.df['2'] = [1, 2, 3]
+        self.assertFalse(self.df.is_empty)
+        self.df['2'] = None
+        self.assertTrue(self.df.is_empty)
+
+    def test_shape(self):
+        self.assertEqual(self.df.shape, (0, 0))
+        self.df['1'] = None
+        self.assertEqual(self.df.shape, (0, 1))
+        self.df['2'] = [1, 2, 3]
+        self.assertEqual(self.df.shape, (3, 2))
+        self.df['2'] = None
+        self.assertEqual(self.df.shape, (0, 2))
+
+
+class TestGetItemsPandasXS(unittest.TestCase):
+    def setUp(self):
+        self.df = sampy.DataFrameXS()
+        self.df['col1'] = [1, 2, 3, 4]
+        self.df['col2'] = [2., 3., 4., 5.]
+
+    def test_check_cols_are_retrieved_correctly(self):
+        self.assertTrue((self.df['col1'] == np.array([1, 2, 3, 4])).all())
+        self.assertTrue((self.df['col2'] == np.array([2., 3., 4., 5.])).all())
+        self.assertFalse((self.df['col1'] == self.df['col2']).all())
+        self.assertTrue(str(self.df['col1'].dtype).startswith('int'))
+
+    def test_getitems_returns_ref(self):
+        self.df['col1'][0] = 0
+        self.assertTrue((self.df['col1'] == np.array([0, 2, 3, 4])).all())
+
+    def test_bool_arr_indexing(self):
+        arr_bool = np.array([True, False, True, False])
+        df = self.df[arr_bool]
+        self.assertEqual(df.nb_rows, 2)
+        self.assertEqual(df.nb_cols, 2)
+        self.assertEqual(df.list_col_name, self.df.list_col_name)
+        self.assertTrue((df['col1'] == np.array([1, 3])).all())
+        self.assertTrue((df['col2'] == np.array([2., 4.])).all())
+
+    def test_int_arr_indexing(self):
+        arr_int = np.array([2, 0, 1, 3])
+        df = self.df[arr_int]
+        self.assertEqual(df.nb_rows, 4)
+        self.assertEqual(df.nb_cols, 2)
+        self.assertEqual(df.list_col_name, self.df.list_col_name)
+        self.assertTrue((df['col1'] == np.array([3, 1, 2, 4])).all())
+        self.assertTrue((df['col2'] == np.array([4., 2., 3., 5.])).all())
+        self.assertFalse((df['col1'] == df['col2']).all())
+        self.assertTrue(str(df['col1'].dtype).startswith('int'))
+
+    def test_wrong_indexing(self):
+        with self.subTest():
+            with self.assertRaises(TypeError) as cm:
+                self.df[{}]
+        with self.subTest():
+            with self.assertRaises(TypeError) as cm:
+                self.df[1]
+        with self.subTest():
+            with self.assertRaises(TypeError) as cm:
+                self.df[[True, True, False]]
+        with self.subTest():
+            with self.assertRaises(TypeError) as cm:
+                self.df[np.array([1., 2., 3., 4.])]
+        with self.subTest():
+            with self.assertRaises(KeyError) as cm:
+                self.df['wrong_col_name']
+        with self.subTest():
+            with self.assertRaises(IndexError) as cm:
+                self.df[np.array([True, True, False])]
+        with self.subTest():
+            with self.assertRaises(IndexError) as cm:
+                self.df[np.array([True, True, False, False, False])]
+        with self.subTest():
+            with self.assertRaises(IndexError) as cm:
+                self.df[np.array([0, 5])]
+
+
+class TestGenericMethodsPandasXS(unittest.TestCase):
+    def setUp(self):
+        self.df = sampy.DataFrameXS()
+        self.df['col1'] = [1, 2, 3, 4]
+        self.df['col2'] = [2., 3., 4., 5.]
+
+    def test_scramble(self):
+        with self.assertRaises(ValueError):
+            self.df.scramble(permutation=np.array([2, 0, 1]))
+        with self.assertRaises(TypeError):
+            self.df.scramble(permutation=[2, 0, 1, 3])
+        with self.assertRaises(ValueError):
+            self.df.scramble(permutation=np.array([2, 0, 1, 4]))
+        with self.assertRaises(ValueError):
+            self.df.scramble(permutation=np.array([[2, 0, 1, 4]]))
+        with self.assertRaises(TypeError):
+            self.df.scramble(permutation=np.array([]))
+        with self.assertRaises(ValueError):
+            self.df.scramble(permutation=np.array(0))
+        perm = np.array([2, 0, 1, 3])
+        self.df.scramble(permutation=perm)
+        self.assertEqual(self.df.nb_rows, 4)
+        self.assertEqual(self.df.nb_cols, 2)
+        self.assertEqual(self.df.list_col_name, ['col1', 'col2'])
+        self.assertTrue((self.df['col1'] == np.array([3, 1, 2, 4])).all())
+        self.assertTrue((self.df['col2'] == np.array([4., 2., 3., 5.])).all())
+        self.assertFalse((self.df['col1'] == self.df['col2']).all())
+        self.assertTrue(str(self.df['col1'].dtype).startswith('int'))
+
+    def test_get_copy(self):
+        with self.assertRaises(KeyError):
+            self.df.get_copy('wrong_col_name')
+
+        with self.assertRaises(TypeError):
+            self.df.get_copy([])
+
+        with self.assertRaises(TypeError):
+            self.df.get_copy(1)
+
+        u = self.df.get_copy('col1')
+        self.assertTrue((u == self.df['col1']).all())
+        u[0] = 0
+        self.assertFalse((u == self.df['col1']).all())
+
+    def test_check_arr_in_col(self):
+        with self.subTest():
+            with self.assertRaises(ValueError):
+                input_arr = np.array([1., 2., 3., 4.])
+                self.df.check_arr_in_col(input_arr, 'col1')
+        with self.subTest():
+            with self.assertRaises(ValueError):
+                input_arr = np.array([1, 2, 3, 4])
+                self.df.check_arr_in_col(input_arr, 'col2')
+        with self.subTest():
+            with self.assertRaises(ValueError):
+                input_arr = np.array([[1., 2.], [3., 4.]])
+                self.df.check_arr_in_col(input_arr, 'col2')
+        with self.subTest():
+            with self.assertRaises(ValueError):
+                input_arr = np.array(2.)
+                self.df.check_arr_in_col(input_arr, 'col2')
+        with self.subTest():
+            with self.assertRaises(ValueError):
+                input_arr = np.array(2.)
+                self.df.check_arr_in_col(input_arr, 'col2')
+        with self.subTest():
+            input_arr = np.array([3, 4, 8, 0, 10, 1])
+            input_arr = input_arr.astype('int8')
+            with self.assertRaises(ValueError):
+                result = self.df.check_arr_in_col(input_arr, 'col1')
+        with self.subTest():
+            input_arr = np.array([3, 4, 8, 0, 10, 1])
+            result = self.df.check_arr_in_col(input_arr, 'col1')
+            self.assertTrue((result == np.array([True, True, False, False, False, True])).all())
+
+    def test_check_arr_in_col_conditional(self):
+        with self.subTest():
+            with self.assertRaises(ValueError):
+                condition = np.array([True, True, False, False])
+                input_arr = np.array([1., 2., 3., 4.])
+                self.df.check_arr_in_col(input_arr, 'col1', condition=condition)
+        with self.subTest():
+            with self.assertRaises(ValueError):
+                condition = np.array([True, True, False, False])
+                input_arr = np.array([1, 2, 3, 4])
+                self.df.check_arr_in_col(input_arr, 'col2', condition=condition)
+        with self.subTest():
+            with self.assertRaises(ValueError):
+                condition = np.array([[True, True], [False, False]])
+                input_arr = np.array([[1., 2.], [3., 4.]])
+                self.df.check_arr_in_col(input_arr, 'col2', condition=condition)
+        with self.subTest():
+            with self.assertRaises(ValueError):
+                condition = np.array([True])
+                input_arr = np.array(2.)
+                self.df.check_arr_in_col(input_arr, 'col2', condition=condition)
+        with self.subTest():
+            with self.assertRaises(ValueError):
+                condition = np.array([True])
+                input_arr = np.array({})
+                self.df.check_arr_in_col(input_arr, 'col2', condition=condition)
+        with self.subTest():
+            condition = np.array([True, False, False, True, True, True])
+            input_arr = np.array([3, 4, 8, 0, 10, 1])
+            input_arr = input_arr.astype('int8')
+            with self.assertRaises(ValueError):
+                self.df.check_arr_in_col(input_arr, 'col1', condition=condition)
+        with self.subTest():
+            condition = np.array([True, False, False, True, True, True])
+            input_arr = np.array([3, 4, 8, 0, 10, 1])
+            result = self.df.check_arr_in_col(input_arr, 'col1', condition=condition)
+            self.assertTrue((result == np.array([True, False, False, False, False, True])).all())
+        with self.subTest():
+            condition = np.array([True, False, False, True, True])
+            input_arr = np.array([3, 4, 8, 0, 10, 1])
+            with self.assertRaises(ValueError):
+                self.df.check_arr_in_col(input_arr, 'col1', condition=condition)
+        with self.subTest():
+            condition = np.array([1, 0, 0, 1, 1, 1])
+            input_arr = np.array([3, 4, 8, 0, 10, 1])
+            with self.assertRaises(ValueError):
+                self.df.check_arr_in_col(input_arr, 'col1', condition=condition)
+        with self.subTest():
+            condition = {}
+            input_arr = np.array([3, 4, 8, 0, 10, 1])
+            with self.assertRaises(ValueError):
+                self.df.check_arr_in_col(input_arr, 'col1', condition=condition)
+        with self.subTest():
+            condition = np.array([[True, False], [False, True], [True, True]])
+            input_arr = np.array([3, 4, 8, 0, 10, 1])
+            with self.assertRaises(ValueError):
+                self.df.check_arr_in_col(input_arr, 'col1', condition=condition)
+
+    def test_concat_inplace_is_false(self):
+        with self.subTest():
+            df = sampy.DataFrameXS()
+            df['col1'] = [5, 6, 7, 8]
+            df['col2'] = [6., 7., 8., 9.]
+            c_df = self.df.concat(df, inplace=False)
+
+            # concats happened as expected
+            self.assertTrue((c_df['col1'] == np.array([1, 2, 3, 4, 5, 6, 7, 8])).all())
+            self.assertTrue((c_df['col2'] == np.array([2., 3., 4., 5., 6., 7., 8., 9.])).all())
+
+            # columns are new copied columns
+            c_df['col1'][0] = 0
+            self.assertFalse(c_df['col1'][0] == self.df['col1'][0])
+
+        with self.subTest():
+            # same test as the previous one, but there is an extra column
+            df = sampy.DataFrameXS()
+            df['col1'] = [5, 6, 7, 8]
+            df['col2'] = [6., 7., 8., 9.]
+            df['col3'] = [1, 2, 3, 4]
+            c_df = self.df.concat(df, inplace=False)
+
+            # check that there is no col3 in the dataframe
+            with self.assertRaises(KeyError):
+                c_df['col3']
+
+            # perform all the previous checks in this case.
+            # concat happened as expected
+            self.assertTrue((c_df['col1'] == np.array([1, 2, 3, 4, 5, 6, 7, 8])).all())
+            self.assertTrue((c_df['col2'] == np.array([2., 3., 4., 5., 6., 7., 8., 9.])).all())
+
+            # columns are new copied columns
+            c_df['col1'][0] = 0
+            self.assertFalse(c_df['col1'][0] == self.df['col1'][0])
+
+        # check that an error is raised when the df don't have the right col_names
+        with self.subTest():
+            df = sampy.DataFrameXS()
+            df['col1'] = [5, 6, 7, 8]
+            df['col3'] = [6., 7., 8., 9.]
+            with self.assertRaises(KeyError):
+                self.df.concat(df, inplace=False)
+
+        # check that appending with an empty dataframe returns a copy
+        with self.subTest():
+            df = sampy.DataFrameXS()
+            c_df = self.df.concat(df, inplace=False)
+            self.assertTrue((c_df['col1'] == self.df['col1']).all())
+            self.assertTrue((c_df['col2'] == self.df['col2']).all())
+
+            c_df['col1'][0] = 0
+            self.assertFalse(c_df['col1'][0] == self.df['col1'][0])
+
+        # check that having a null column in the input is correctly dealt with
+        with self.subTest():
+            df = sampy.DataFrameXS()
+            df['col1'] = [5, 6, 7, 8]
+            df['col2'] = None
+            c_df = self.df.concat(df, inplace=False)
+            self.assertTrue((c_df['col1'] == np.array([1, 2, 3, 4, 5, 6, 7, 8])).all())
+            self.assertTrue((np.nan_to_num(c_df['col2'], nan=0.) == np.array([2., 3., 4., 5., 0., 0., 0., 0.])).all())
+            self.assertEqual(str(c_df['col2'].dtype), str(self.df['col2'].dtype))
+
+        # same thing but in reverse
+        with self.subTest():
+            df_in = sampy.DataFrameXS()
+            df_in['col1'] = [1, 2, 3, 4]
+            df_in['col2'] = None
+
+            df = sampy.DataFrameXS()
+            df['col1'] = [5, 6, 7, 8]
+            df['col2'] = [6., 7., 8., 9.]
+            c_df = df_in.concat(df, inplace=False)
+            self.assertTrue((c_df['col1'] == np.array([1, 2, 3, 4, 5, 6, 7, 8])).all())
+            self.assertTrue((np.nan_to_num(c_df['col2'], 0.) == np.array([0., 0., 0., 0., 6., 7., 8., 9.])).all())
+            self.assertEqual(str(c_df['col2'].dtype), str(df['col2'].dtype))
+
+        # When the first df is empty
+        with self.subTest():
+            df_in = sampy.DataFrameXS()
+            df_in['col1'] = None
+            df_in['col2'] = None
+
+            df = sampy.DataFrameXS()
+            df['col1'] = [5, 6, 7, 8]
+            df['col2'] = [6., 7., 8., 9.]
+            c_df = df_in.concat(df, inplace=False)
+
+            self.assertTrue((c_df['col1'] == np.array([5, 6, 7, 8])).all())
+            self.assertEqual(str(c_df['col1'].dtype), str(df['col1'].dtype))
+            self.assertTrue((np.nan_to_num(c_df['col2'], nan=0.) == np.array([6., 7., 8., 9.])).all())
+            self.assertEqual(str(c_df['col2'].dtype), str(df['col2'].dtype))
+
+            # check that a copy is retrieved
+            c_df['col1'][0] = 0
+            self.assertFalse((c_df['col1'] == df['col1']).all())
+
+        # adding an empty column on an empty column
+        with self.subTest():
+            df_in = sampy.DataFrameXS()
+            df_in['col1'] = [1, 2, 3, 4]
+            df_in['col2'] = None
+
+            df = sampy.DataFrameXS()
+            df['col1'] = [5, 6, 7, 8]
+            df['col2'] = None
+
+            c_df = df_in.concat(df, inplace=False)
+
+            self.assertIsNone(c_df['col2'])
+            self.assertTrue((c_df['col1'] == np.array([1, 2, 3, 4, 5, 6, 7, 8])).all())
+            self.assertEqual(str(c_df['col1'].dtype), str(df['col1'].dtype))
+
+    def test_concat_inplace_is_true_basic(self):
+        df = sampy.DataFrameXS()
+        df['col1'] = [5, 6, 7, 8]
+        df['col2'] = [6., 7., 8., 9.]
+        self.df.concat(df, inplace=True)
+
+        # concats happened as expected
+        self.assertTrue((self.df['col1'] == np.array([1, 2, 3, 4, 5, 6, 7, 8])).all())
+        self.assertTrue((self.df['col2'] == np.array([2., 3., 4., 5., 6., 7., 8., 9.])).all())
+
+    def test_concat_inplace_is_true_extra_col(self):
+        df = sampy.DataFrameXS()
+        df['col1'] = [5, 6, 7, 8]
+        df['col2'] = [6., 7., 8., 9.]
+        df['col3'] = [1, 2, 3, 4]
+        self.df.concat(df, inplace=True)
+
+        # check that there is no col3 in the dataframe
+        with self.assertRaises(KeyError):
+            self.df['col3']
+
+        # perform all the previous checks in this case.
+        # concat happened as expected
+        self.assertTrue((self.df['col1'] == np.array([1, 2, 3, 4, 5, 6, 7, 8])).all())
+        self.assertTrue((self.df['col2'] == np.array([2., 3., 4., 5., 6., 7., 8., 9.])).all())
+        self.assertEqual(self.df.nb_rows, 8)
+
+    def test_concat_inplace_is_true_wrong_col_name(self):
+        df = sampy.DataFrameXS()
+        df['col1'] = [5, 6, 7, 8]
+        df['col3'] = [6., 7., 8., 9.]
+        with self.assertRaises(KeyError):
+            self.df.concat(df, inplace=True)
+
+    def test_concat_inplace_is_true_empty_col_on_empty_col(self):
+        self.df['col2'] = None
+
+        df = sampy.DataFrameXS()
+        df['col1'] = [5, 6, 7, 8]
+        df['col2'] = None
+
+        self.df.concat(df, inplace=True)
+
+        self.assertIsNone(self.df['col2'])
+        self.assertTrue((self.df['col1'] == np.array([1, 2, 3, 4, 5, 6, 7, 8])).all())
+        self.assertEqual(str(self.df['col1'].dtype), str(df['col1'].dtype))
+
+    def test_concat_inplace_is_true_empty_col_in_input(self):
+        df = sampy.DataFrameXS()
+        df['col1'] = [5, 6, 7, 8]
+        df['col2'] = None
+
+        self.df.concat(df, inplace=True)
+
+        self.assertTrue((np.nan_to_num(self.df['col2'], nan=0.) == np.array([2., 3., 4., 5., 0., 0., 0., 0.])).all())
+        self.assertTrue((self.df['col1'] == np.array([1, 2, 3, 4, 5, 6, 7, 8])).all())
+        self.assertEqual(str(self.df['col1'].dtype), str(df['col1'].dtype))
+
+    def test_concat_inplace_is_true_on_empty_df(self):
+        self.df['col1'] = None
+        self.df['col2'] = None
+
+        df = sampy.DataFrameXS()
+        df['col1'] = [5, 6, 7, 8]
+        df['col2'] = [6., 7., 8., 9.]
+        self.df.concat(df, inplace=True)
+
+        self.assertTrue((self.df['col1'] == np.array([5, 6, 7, 8])).all())
+        self.assertEqual(str(self.df['col1'].dtype), str(df['col1'].dtype))
+        self.assertTrue((np.nan_to_num(self.df['col2'], nan=0.) == np.array([6., 7., 8., 9.])).all())
+        self.assertEqual(str(self.df['col2'].dtype), str(df['col2'].dtype))
+
+        self.assertEqual(self.df.nb_rows, 4)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

