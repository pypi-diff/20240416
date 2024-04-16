# Comparing `tmp/pyflowline-0.3.4.tar.gz` & `tmp/pyflowline-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflowline-0.3.4.tar", last modified: Mon Nov  6 20:22:15 2023, max compression
+gzip compressed data, was "pyflowline-0.3.5.tar", last modified: Tue Apr 16 15:38:05 2024, max compression
```

## Comparing `pyflowline-0.3.4.tar` & `pyflowline-0.3.5.tar`

### file list

```diff
@@ -1,176 +1,175 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.337170 pyflowline-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-11-06 20:22:00.000000 pyflowline-0.3.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2023-11-06 20:22:00.000000 pyflowline-0.3.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-11-06 20:22:00.000000 pyflowline-0.3.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2023-11-06 20:22:00.000000 pyflowline-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2023-11-06 20:22:00.000000 pyflowline-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2023-11-06 20:22:15.337170 pyflowline-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5674 2023-11-06 20:22:00.000000 pyflowline-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.297170 pyflowline-0.3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6813 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.309170 pyflowline-0.3.4/docs/figures/
--rw-r--r--   0 runner    (1001) docker     (127)    67244 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/figures/after_loop.png
--rw-r--r--   0 runner    (1001) docker     (127)    64320 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/figures/after_merge.png
--rw-r--r--   0 runner    (1001) docker     (127)    68901 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/figures/basic_element.png
--rw-r--r--   0 runner    (1001) docker     (127)    76858 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/figures/before_loop.png
--rw-r--r--   0 runner    (1001) docker     (127)    68959 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/figures/before_merge.png
--rw-r--r--   0 runner    (1001) docker     (127)    16482 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/figures/disconnect_flowline.png
--rw-r--r--   0 runner    (1001) docker     (127)   146717 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/figures/find_vertex.png
--rw-r--r--   0 runner    (1001) docker     (127)    15195 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/figures/flow_direction.png
--rw-r--r--   0 runner    (1001) docker     (127)   252712 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/figures/flow_direction_matrix.png
--rw-r--r--   0 runner    (1001) docker     (127)   525380 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/figures/hexagon.png
--rw-r--r--   0 runner    (1001) docker     (127)   628942 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/figures/hexagon_intersect.png
--rw-r--r--   0 runner    (1001) docker     (127)   524174 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/figures/lat_lon.png
--rw-r--r--   0 runner    (1001) docker     (127)   734342 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/figures/lat_lon_intersect.png
--rw-r--r--   0 runner    (1001) docker     (127)    45168 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/figures/merge_flowline.png
--rw-r--r--   0 runner    (1001) docker     (127)  1191889 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/figures/meshes.png
--rw-r--r--   0 runner    (1001) docker     (127)    47724 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/figures/remove_loop.png
--rw-r--r--   0 runner    (1001) docker     (127)   596253 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/figures/remove_loop_matrix.png
--rw-r--r--   0 runner    (1001) docker     (127)    93563 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/figures/simplification01.png
--rw-r--r--   0 runner    (1001) docker     (127)    21317 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/figures/small_river.png
--rw-r--r--   0 runner    (1001) docker     (127)   148387 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/figures/sqaure_intersect.png
--rw-r--r--   0 runner    (1001) docker     (127)    61180 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/figures/square.png
--rw-r--r--   0 runner    (1001) docker     (127)    46783 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/figures/structure_pyflowline.png
--rw-r--r--   0 runner    (1001) docker     (127)   160993 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/figures/workflow.png
--rw-r--r--   0 runner    (1001) docker     (127)     6708 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.313170 pyflowline-0.3.4/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.313170 pyflowline-0.3.4/docs/source/algorithm/
--rw-r--r--   0 runner    (1001) docker     (127)     7897 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/source/algorithm/algorithm.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.313170 pyflowline-0.3.4/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/source/api/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.313170 pyflowline-0.3.4/docs/source/application/
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/source/application/application.rst
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/source/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/source/contribution.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.313170 pyflowline-0.3.4/docs/source/data/
--rw-r--r--   0 runner    (1001) docker     (127)    29867 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/source/data/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/source/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/source/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      725 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.313170 pyflowline-0.3.4/docs/source/installation/
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/source/installation/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/source/references.rst
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/source/support.rst
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-11-06 20:22:01.000000 pyflowline-0.3.4/docs/source/visualization.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.313170 pyflowline-0.3.4/examples/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:01.000000 pyflowline-0.3.4/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2023-11-06 20:22:01.000000 pyflowline-0.3.4/examples/create_model_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.317170 pyflowline-0.3.4/pyflowline/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.317170 pyflowline-0.3.4/pyflowline/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.317170 pyflowline-0.3.4/pyflowline/algorithms/auxiliary/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/auxiliary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16301 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/auxiliary/calculate_area_of_difference.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/auxiliary/check_head_water.py
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/auxiliary/find_index_in_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/auxiliary/find_vertex_in_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/auxiliary/longlat_to_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.317170 pyflowline-0.3.4/pyflowline/algorithms/connection/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/connection/connect_disconnect_flowline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.317170 pyflowline-0.3.4/pyflowline/algorithms/cython/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/cython/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.317170 pyflowline-0.3.4/pyflowline/algorithms/direction/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/direction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/direction/correct_flowline_direction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.321170 pyflowline-0.3.4/pyflowline/algorithms/index/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7566 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/index/define_stream_order.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/index/define_stream_segment_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/index/define_stream_topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.321170 pyflowline-0.3.4/pyflowline/algorithms/intersect/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/intersect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/intersect/intersect_flowline_with_flowline.py
--rw-r--r--   0 runner    (1001) docker     (127)    15924 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/intersect/intersect_flowline_with_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/intersect/intersect_flowline_with_vertex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.321170 pyflowline-0.3.4/pyflowline/algorithms/loop/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/loop/remove_flowline_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.321170 pyflowline-0.3.4/pyflowline/algorithms/merge/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/merge/merge_flowline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.321170 pyflowline-0.3.4/pyflowline/algorithms/simplification/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/simplification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/simplification/remove_duplicate_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/simplification/remove_duplicate_flowline.py
--rw-r--r--   0 runner    (1001) docker     (127)     9151 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/simplification/remove_returning_flowline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/simplification/remove_small_river.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.325170 pyflowline-0.3.4/pyflowline/algorithms/split/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/split/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/split/find_flowline_confluence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/split/find_flowline_vertex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/split/split_by_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/split/split_flowline.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/algorithms/split/split_flowline_to_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/change_json_key_value.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.329170 pyflowline-0.3.4/pyflowline/classes/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/classes/_hpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/classes/_visual.py
--rw-r--r--   0 runner    (1001) docker     (127)    19639 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/classes/_visual_basin.py
--rw-r--r--   0 runner    (1001) docker     (127)    59508 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/classes/basin.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/classes/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/classes/confluence.py
--rw-r--r--   0 runner    (1001) docker     (127)     6760 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/classes/dggrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8963 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/classes/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     9669 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/classes/flowline.py
--rw-r--r--   0 runner    (1001) docker     (127)     7024 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/classes/hexagon.py
--rw-r--r--   0 runner    (1001) docker     (127)     6823 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/classes/latlon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/classes/link.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/classes/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/classes/mpas.py
--rw-r--r--   0 runner    (1001) docker     (127)    57219 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/classes/pycase.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/classes/square.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/classes/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/classes/tin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7224 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/classes/vertex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.333170 pyflowline-0.3.4/pyflowline/formats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/formats/convert_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8005 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/formats/convert_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/formats/convert_flowline_to_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     8731 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/formats/export_flowline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/formats/export_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/formats/export_vertex.py
--rw-r--r--   0 runner    (1001) docker     (127)     9810 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/formats/read_flowline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/formats/read_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     6937 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/formats/read_nhdplus_flowline_shapefile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.333170 pyflowline-0.3.4/pyflowline/mesh/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/mesh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.333170 pyflowline-0.3.4/pyflowline/mesh/dggrid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/mesh/dggrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12456 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/mesh/dggrid/create_dggrid_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.333170 pyflowline-0.3.4/pyflowline/mesh/hexagon/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/mesh/hexagon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28663 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/mesh/hexagon/create_hexagon_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.337170 pyflowline-0.3.4/pyflowline/mesh/latlon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/mesh/latlon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9140 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/mesh/latlon/create_latlon_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.337170 pyflowline-0.3.4/pyflowline/mesh/mpas/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/mesh/mpas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23255 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/mesh/mpas/create_mpas_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.337170 pyflowline-0.3.4/pyflowline/mesh/square/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/mesh/square/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15375 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/mesh/square/create_square_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.337170 pyflowline-0.3.4/pyflowline/mesh/tin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/mesh/tin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6165 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/mesh/tin/create_tin_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/pyflowline_create_template_configuration_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyflowline/pyflowline_read_model_configuration_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.317170 pyflowline-0.3.4/pyflowline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2023-11-06 20:22:15.000000 pyflowline-0.3.4/pyflowline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2023-11-06 20:22:15.000000 pyflowline-0.3.4/pyflowline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-06 20:22:15.000000 pyflowline-0.3.4/pyflowline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-11-06 20:22:15.000000 pyflowline-0.3.4/pyflowline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-06 20:22:15.000000 pyflowline-0.3.4/pyflowline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-11-06 20:22:01.000000 pyflowline-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      382 2023-11-06 20:22:15.341170 pyflowline-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2023-11-06 20:22:01.000000 pyflowline-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 20:22:15.337170 pyflowline-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2023-11-06 20:22:01.000000 pyflowline-0.3.4/tests/test_installation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.549494 pyflowline-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-16 15:37:59.000000 pyflowline-0.3.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-16 15:37:59.000000 pyflowline-0.3.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-16 15:37:59.000000 pyflowline-0.3.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-16 15:37:59.000000 pyflowline-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-16 15:37:59.000000 pyflowline-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-16 15:38:05.549494 pyflowline-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-16 15:37:59.000000 pyflowline-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.517494 pyflowline-0.3.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.529494 pyflowline-0.3.5/docs/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)    67244 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/after_loop.png
+-rw-r--r--   0 runner    (1001) docker     (127)    64320 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/after_merge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68901 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/basic_element.png
+-rw-r--r--   0 runner    (1001) docker     (127)    76858 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/before_loop.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68959 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/before_merge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16482 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/disconnect_flowline.png
+-rw-r--r--   0 runner    (1001) docker     (127)   146717 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/find_vertex.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15195 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/flow_direction.png
+-rw-r--r--   0 runner    (1001) docker     (127)   252712 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/flow_direction_matrix.png
+-rw-r--r--   0 runner    (1001) docker     (127)   525380 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/hexagon.png
+-rw-r--r--   0 runner    (1001) docker     (127)   628942 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/hexagon_intersect.png
+-rw-r--r--   0 runner    (1001) docker     (127)   524174 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/lat_lon.png
+-rw-r--r--   0 runner    (1001) docker     (127)   734342 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/lat_lon_intersect.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45168 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/merge_flowline.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1191889 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/meshes.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47724 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/remove_loop.png
+-rw-r--r--   0 runner    (1001) docker     (127)   596253 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/remove_loop_matrix.png
+-rw-r--r--   0 runner    (1001) docker     (127)    93563 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/simplification01.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21317 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/small_river.png
+-rw-r--r--   0 runner    (1001) docker     (127)   148387 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/sqaure_intersect.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61180 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/square.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46783 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/structure_pyflowline.png
+-rw-r--r--   0 runner    (1001) docker     (127)   160993 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.533494 pyflowline-0.3.5/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.533494 pyflowline-0.3.5/docs/source/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (127)     7897 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/algorithm/algorithm.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.533494 pyflowline-0.3.5/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/api/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.533494 pyflowline-0.3.5/docs/source/application/
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/application/application.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/contribution.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.533494 pyflowline-0.3.5/docs/source/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    29917 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/data/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.533494 pyflowline-0.3.5/docs/source/installation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/installation/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/references.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/support.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/visualization.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.533494 pyflowline-0.3.5/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-16 15:37:59.000000 pyflowline-0.3.5/examples/create_model_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.533494 pyflowline-0.3.5/pyflowline/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.533494 pyflowline-0.3.5/pyflowline/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.533494 pyflowline-0.3.5/pyflowline/algorithms/auxiliary/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/auxiliary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16198 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/auxiliary/calculate_area_of_difference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/auxiliary/check_head_water.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/auxiliary/find_index_in_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/auxiliary/find_vertex_in_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.537494 pyflowline-0.3.5/pyflowline/algorithms/connection/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/connection/connect_disconnect_flowline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.537494 pyflowline-0.3.5/pyflowline/algorithms/cython/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/cython/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.537494 pyflowline-0.3.5/pyflowline/algorithms/direction/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/direction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/direction/correct_flowline_direction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.537494 pyflowline-0.3.5/pyflowline/algorithms/index/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/index/define_stream_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/index/define_stream_segment_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/index/define_stream_topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.537494 pyflowline-0.3.5/pyflowline/algorithms/intersect/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/intersect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/intersect/intersect_flowline_with_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15785 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/intersect/intersect_flowline_with_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/intersect/intersect_flowline_with_vertex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.537494 pyflowline-0.3.5/pyflowline/algorithms/loop/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/loop/remove_flowline_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.537494 pyflowline-0.3.5/pyflowline/algorithms/merge/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/merge/merge_flowline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.537494 pyflowline-0.3.5/pyflowline/algorithms/simplification/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/simplification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/simplification/remove_duplicate_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/simplification/remove_duplicate_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/simplification/remove_returning_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/simplification/remove_small_river.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.541494 pyflowline-0.3.5/pyflowline/algorithms/split/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/split/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/split/find_flowline_confluence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/split/find_flowline_vertex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/split/split_by_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/split/split_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/split/split_flowline_to_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/change_json_key_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.545494 pyflowline-0.3.5/pyflowline/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/_hpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/_visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24307 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/_visual_basin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62019 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/basin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/confluence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/dggrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/flowline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/hexagon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/latlon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/mpas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59119 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/pycase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/square.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/tin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/vertex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.545494 pyflowline-0.3.5/pyflowline/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/formats/convert_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/formats/convert_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/formats/convert_flowline_to_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/formats/export_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/formats/export_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/formats/export_vertex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11769 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/formats/read_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/formats/read_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/formats/read_nhdplus_flowline_shapefile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.545494 pyflowline-0.3.5/pyflowline/mesh/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.545494 pyflowline-0.3.5/pyflowline/mesh/dggrid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/dggrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/dggrid/create_dggrid_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.545494 pyflowline-0.3.5/pyflowline/mesh/hexagon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/hexagon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28451 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/hexagon/create_hexagon_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.545494 pyflowline-0.3.5/pyflowline/mesh/latlon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/latlon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/latlon/create_latlon_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.545494 pyflowline-0.3.5/pyflowline/mesh/mpas/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/mpas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23224 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/mpas/create_mpas_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.545494 pyflowline-0.3.5/pyflowline/mesh/square/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/square/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15367 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/square/create_square_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.545494 pyflowline-0.3.5/pyflowline/mesh/tin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/tin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/tin/create_tin_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/pyflowline_create_template_configuration_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/pyflowline_read_model_configuration_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.549494 pyflowline-0.3.5/pyflowline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-16 15:38:05.000000 pyflowline-0.3.5/pyflowline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-16 15:38:05.000000 pyflowline-0.3.5/pyflowline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:38:05.000000 pyflowline-0.3.5/pyflowline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-16 15:38:05.000000 pyflowline-0.3.5/pyflowline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 15:38:05.000000 pyflowline-0.3.5/pyflowline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-16 15:38:05.549494 pyflowline-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-16 15:37:59.000000 pyflowline-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.549494 pyflowline-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-16 15:37:59.000000 pyflowline-0.3.5/tests/test_installation.py
```

### Comparing `pyflowline-0.3.4/CONTRIBUTING.rst` & `pyflowline-0.3.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/LICENSE` & `pyflowline-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/PKG-INFO` & `pyflowline-0.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflowline
-Version: 0.3.4
+Version: 0.3.5
 Summary: A mesh-independent river network generator for hydrologic models
 Home-page: https://github.com/changliao1025/pyflowline
 Author: Chang Liao
 Author-email: chang.liao@pnnl.gov
 License: custom
 Keywords: Earth Science
 Classifier: Development Status :: 4 - Beta
@@ -28,14 +28,15 @@
 Requires-Dist: matplotlib; extra == "visualization"
 Requires-Dist: cartopy>=0.21.0; extra == "visualization"
 Requires-Dist: simplekml; extra == "visualization"
 
 
 ### PyFlowline
 
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05446/status.svg)](https://doi.org/10.21105/joss.05446)
 [![DOI](https://zenodo.org/badge/368338554.svg)](https://zenodo.org/badge/latestdoi/368338554)
 [![Downloads](https://static.pepy.tech/badge/pyflowline)](https://pepy.tech/project/pyflowline)
 
 PyFlowline: a mesh-independent river network generator for hydrologic models.  
 
 ### Quickstart
 
@@ -106,11 +107,13 @@
 
 2. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL BATTELLE OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 ### References
 
 Several publications describe the algorithms used in `PyFlowline` in detail. If you make use of `PyFlowline` in your work, please consider including a reference to the following:
 
+* Liao et al., (2023). pyflowline: a mesh-independent river network generator for hydrologic models. Journal of Open Source Software, 8(91), 5446, https://doi.org/10.21105/joss.05446
+
 * Liao. C. Cooper, M (2022) Pyflowline: a mesh-independent river network generator for hydrologic models. Zenodo.
 https://doi.org/10.5281/zenodo.6407298
 
 * Liao, C., Zhou, T., Xu, D., Cooper, M. G., Engwirda, D., Li, H.-Y., & Leung, L. R. (2023). Topological relationship-based flow direction modeling: Mesh-independent river networks representation. Journal of Advances in Modeling Earth Systems, 15, e2022MS003089. https://doi.org/10.1029/2022MS003089
```

### Comparing `pyflowline-0.3.4/README.md` & `pyflowline-0.3.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ### PyFlowline
 
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05446/status.svg)](https://doi.org/10.21105/joss.05446)
 [![DOI](https://zenodo.org/badge/368338554.svg)](https://zenodo.org/badge/latestdoi/368338554)
 [![Downloads](https://static.pepy.tech/badge/pyflowline)](https://pepy.tech/project/pyflowline)
 
 PyFlowline: a mesh-independent river network generator for hydrologic models.  
 
 ### Quickstart
 
@@ -74,11 +75,13 @@
 
 2. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL BATTELLE OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 ### References
 
 Several publications describe the algorithms used in `PyFlowline` in detail. If you make use of `PyFlowline` in your work, please consider including a reference to the following:
 
+* Liao et al., (2023). pyflowline: a mesh-independent river network generator for hydrologic models. Journal of Open Source Software, 8(91), 5446, https://doi.org/10.21105/joss.05446
+
 * Liao. C. Cooper, M (2022) Pyflowline: a mesh-independent river network generator for hydrologic models. Zenodo.
 https://doi.org/10.5281/zenodo.6407298
 
 * Liao, C., Zhou, T., Xu, D., Cooper, M. G., Engwirda, D., Li, H.-Y., & Leung, L. R. (2023). Topological relationship-based flow direction modeling: Mesh-independent river networks representation. Journal of Advances in Modeling Earth Systems, 15, e2022MS003089. https://doi.org/10.1029/2022MS003089
```

### Comparing `pyflowline-0.3.4/docs/Makefile` & `pyflowline-0.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/figures/after_loop.png` & `pyflowline-0.3.5/docs/figures/after_loop.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/figures/after_merge.png` & `pyflowline-0.3.5/docs/figures/after_merge.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/figures/basic_element.png` & `pyflowline-0.3.5/docs/figures/basic_element.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/figures/before_loop.png` & `pyflowline-0.3.5/docs/figures/before_loop.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/figures/before_merge.png` & `pyflowline-0.3.5/docs/figures/before_merge.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/figures/disconnect_flowline.png` & `pyflowline-0.3.5/docs/figures/disconnect_flowline.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/figures/find_vertex.png` & `pyflowline-0.3.5/docs/figures/find_vertex.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/figures/flow_direction.png` & `pyflowline-0.3.5/docs/figures/flow_direction.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/figures/flow_direction_matrix.png` & `pyflowline-0.3.5/docs/figures/flow_direction_matrix.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/figures/hexagon.png` & `pyflowline-0.3.5/docs/figures/hexagon.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/figures/hexagon_intersect.png` & `pyflowline-0.3.5/docs/figures/hexagon_intersect.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/figures/lat_lon.png` & `pyflowline-0.3.5/docs/figures/lat_lon.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/figures/lat_lon_intersect.png` & `pyflowline-0.3.5/docs/figures/lat_lon_intersect.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/figures/merge_flowline.png` & `pyflowline-0.3.5/docs/figures/merge_flowline.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/figures/meshes.png` & `pyflowline-0.3.5/docs/figures/meshes.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/figures/remove_loop.png` & `pyflowline-0.3.5/docs/figures/remove_loop.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/figures/remove_loop_matrix.png` & `pyflowline-0.3.5/docs/figures/remove_loop_matrix.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/figures/simplification01.png` & `pyflowline-0.3.5/docs/figures/simplification01.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/figures/small_river.png` & `pyflowline-0.3.5/docs/figures/small_river.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/figures/sqaure_intersect.png` & `pyflowline-0.3.5/docs/figures/sqaure_intersect.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/figures/square.png` & `pyflowline-0.3.5/docs/figures/square.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/figures/structure_pyflowline.png` & `pyflowline-0.3.5/docs/figures/structure_pyflowline.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/figures/workflow.png` & `pyflowline-0.3.5/docs/figures/workflow.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/make.bat` & `pyflowline-0.3.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/source/algorithm/algorithm.rst` & `pyflowline-0.3.5/docs/source/algorithm/algorithm.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/source/api/api.rst` & `pyflowline-0.3.5/docs/source/api/api.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/source/application/application.rst` & `pyflowline-0.3.5/docs/source/application/application.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/source/conf.py` & `pyflowline-0.3.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/source/data/data.rst` & `pyflowline-0.3.5/docs/source/data/data.rst`

 * *Files 2% similar despite different names*

```diff
@@ -226,23 +226,24 @@
 ==============================
 Inputs
 ==============================
 
 The following recommended workspace structure and example input files are provided to run a PyFlowline simulation. Although the repo includes example configuration files in the examples/ directory, they can be placed wherever the user prefers, as long as the paths within them point to the correct locations for input (and output) data.
 
 ::
-	data
-	└── <domain_name>
-		├── input
-		│   ├── boundary_wgs.geojson
-		│   ├── flowline.geojson
-		│   ├── pyflowline_<domain_name>_<meshtype>.json
-		│   └── pyflowline_<domain_name>_basins.json 
-		└── output 
-			└── ...
+
+    data
+    └── <domain_name>
+        ├── input
+        │   ├── boundary_wgs.geojson
+        │   ├── flowline.geojson
+        │   ├── pyflowline_<domain_name>_<meshtype>.json
+        │   └── pyflowline_<domain_name>_basins.json
+        └── output
+            └── ...
 
 ==============================
 Outputs
 ==============================
 
 After running the PyFlowline simulation, the output workspace will be structured as follows:
```

### Comparing `pyflowline-0.3.4/docs/source/faq.rst` & `pyflowline-0.3.5/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/source/glossary.rst` & `pyflowline-0.3.5/docs/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/source/index.rst` & `pyflowline-0.3.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/source/installation/installation.rst` & `pyflowline-0.3.5/docs/source/installation/installation.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/source/quickstart.rst` & `pyflowline-0.3.5/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/docs/source/readme.rst` & `pyflowline-0.3.5/docs/source/readme.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/examples/create_model_configuration.py` & `pyflowline-0.3.5/examples/create_model_configuration.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/pyflowline/algorithms/auxiliary/calculate_area_of_difference.py` & `pyflowline-0.3.5/pyflowline/algorithms/auxiliary/calculate_area_of_difference.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import numpy as np
 from osgeo import ogr, osr
-import importlib
+import importlib.util
 
 from pyflowline.algorithms.auxiliary.find_index_in_list import find_list_in_list 
-from pyflowline.external.pyearth.gis.gdal.gdal_functions import calculate_angle_betwen_vertex_normal
-from pyflowline.external.pyearth.gis.gdal.gdal_functions import calculate_polygon_area
+
+from pyearth.gis.geometry.calculate_polygon_area import calculate_polygon_area
 
 iFlag_cython = importlib.util.find_spec("cython") 
 if iFlag_cython is not None:
     from pyflowline.algorithms.cython.kernel import find_vertex_in_list
 else:
     from pyflowline.algorithms.auxiliary.find_vertex_in_list import find_vertex_in_list
```

### Comparing `pyflowline-0.3.4/pyflowline/algorithms/auxiliary/find_index_in_list.py` & `pyflowline-0.3.5/pyflowline/algorithms/auxiliary/find_index_in_list.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import copy
 import numpy as np
-
-
-import importlib
+import importlib.util
 iFlag_cython = importlib.util.find_spec("cython") 
 if iFlag_cython is not None:
     from pyflowline.algorithms.cython.kernel import find_vertex_in_list
     from pyflowline.external.tinyr.tinyr.tinyr import RTree
     iFlag_use_rtree = 1
 else:
     iFlag_use_rtree =0
@@ -23,18 +21,18 @@
     if nVertex > 0 :
         if iFlag_use_rtree == 1:
             index_vertex = RTree(max_cap=5, min_cap=2)
             for i in range(nVertex):
                 lID = i 
                 x = aVertex_in[i].dLongitude_degree
                 y = aVertex_in[i].dLatitude_degree   
-                left= x - 1E-5
-                right= x + 1E-5
-                bottom= y-1E-5
-                top=    y+1E-5
+                left =   x - 1E-5
+                right =  x + 1E-5
+                bottom = y - 1E-5
+                top =    y + 1E-5
                 pBound= (left, bottom, right, top)
                 index_vertex.insert(lID, pBound)  # 
                 pass
             #now the new vertex
             pVertex_start = pEdge_in.pVertex_start
             pVertex_end = pEdge_in.pVertex_end
             x1=pVertex_start.dLongitude_degree
@@ -107,21 +105,15 @@
     if nEdge > 0 :
         for i in np.arange( nEdge):
             pEdge = aEdge_in[i]
             if pEdge == pEdge_in:
                 iFlag_exist = 1      
                 lIndex = i 
                 break                
-            else:
-                pass
-
-        pass        
-        
-    else:
-        pass
+            
     
     return iFlag_exist, lIndex
 
 
 def find_flowline_in_list(aFlowline_in, pFlowline_in):
     """[find the index of a flowline in a list]
 
@@ -138,22 +130,15 @@
 
     if nFlowline > 0 :
         for i in np.arange( nFlowline):
             pFlowline = aFlowline_in[i]
             if pFlowline == pFlowline_in:
                 iFlag_exist = 1      
                 lIndex = i 
-                break                
-            else:
-                pass
-
-        pass        
-        
-    else:
-        pass
+                break                        
     
     return iFlag_exist, lIndex
 
 def find_hexagon_through_edge(aHexagon_in, pEdge_in):
     """find the hexagons which contain an edge
 
     Args:
@@ -165,36 +150,33 @@
     """
 
     nHexagon = len(aHexagon_in)
     aHexagon_out = list()
     for i in range(nHexagon):
         pHexagon = aHexagon_in[i]
         if pHexagon.has_this_edge(pEdge_in) ==1:
-            aHexagon_out.append(pHexagon)
-            pass
-        else:
-            pass
+            aHexagon_out.append(pHexagon)            
 
     return aHexagon_out
 
 def check_if_duplicates(aList_in):
     """[Check if given list contains any duplicates]
 
     Returns:
         [type]: [description]
     """
-    iFlag_unique = 1
-    for elem in aList_in:
-        if aList_in.count(elem) > 1:
-            iFlag_unique = 0
-            break
-        else:
-            pass
-    
-    return iFlag_unique
+    #iFlag_unique = 1
+    #for elem in aList_in:
+    #    if aList_in.count(elem) > 1:
+    #        iFlag_unique = 0
+    #        break
+    #    else:
+    #        pass    
+    #return iFlag_unique
+    return int(len(aList_in) == len(set(aList_in)))
 
 
 def add_unique_vertex(aVertex_in, pVertex_in, dThreshold_in = 1.0E-6):
     """[add a vertex to a list if it is not already included]
 
     Args:
         aVertex_in ([type]): [description]
```

### Comparing `pyflowline-0.3.4/pyflowline/algorithms/auxiliary/find_vertex_in_list.py` & `pyflowline-0.3.5/pyflowline/algorithms/auxiliary/find_vertex_in_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-import importlib
+import importlib.util
 import numpy as np
 iFlag_cython = importlib.util.find_spec("cython") 
 if iFlag_cython is not None:
     from pyflowline.external.tinyr.tinyr.tinyr import RTree
     iFlag_use_rtree = 1
 else:
     iFlag_use_rtree =0
@@ -19,17 +19,15 @@
     Returns:
         [type]: [description]
     """
 
     iFlag_exist = 0
     lIndex= -1
     nVertex= len(aVertex_in)
-
     if iFlag_use_rtree == 1:
-
         #can we use rtree here?
         #index_vertex = rtree.index.Index()
         index_vertex = RTree(max_cap=5, min_cap=2)
         for i in range(nVertex):
             lID = i 
             x=aVertex_in[i].dLongitude_degree
             y=aVertex_in[i].dLatitude_degree
```

### Comparing `pyflowline-0.3.4/pyflowline/algorithms/connection/connect_disconnect_flowline.py` & `pyflowline-0.3.5/pyflowline/algorithms/connection/connect_disconnect_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/pyflowline/algorithms/index/define_stream_order.py` & `pyflowline-0.3.5/pyflowline/algorithms/index/define_stream_order.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 
 import numpy as np 
-import importlib
+import importlib.util
 from pyflowline.algorithms.auxiliary.check_head_water import check_head_water #this function should not be used since stream order of headwater is available 
 iFlag_cython = importlib.util.find_spec("cython") 
 if iFlag_cython is not None:
     from pyflowline.external.tinyr.tinyr.tinyr import RTree
     iFlag_use_rtree = 1
 else:
     iFlag_use_rtree =0
     pass
 
 def update_head_water_stream_order(aFlowline_in):
-    nFlowline = len(aFlowline_in)
-    aFlowline_out = list()
-    for i in range(nFlowline):
-        pFlowline = aFlowline_in[i]          
-        pVertex_start = pFlowline.pVertex_start  
-        if check_head_water(aFlowline_in, pVertex_start)==1:
-            pFlowline.iStream_order = 1
-            pass
-        else:
-            pFlowline.iStream_order = -1
-        
-        aFlowline_out.append(pFlowline)
+    start_vertices = {flowline.pVertex_start for flowline in aFlowline_in}
+    end_vertices = {flowline.pVertex_end for flowline in aFlowline_in}
 
-    return aFlowline_out
+    for flowline in aFlowline_in:
+        pVertex_start = flowline.pVertex_start
+        is_headwater = pVertex_start in start_vertices and pVertex_start not in end_vertices
+        flowline.iStream_order = 1 if is_headwater else -1
+
+    return aFlowline_in
+
+    #nFlowline = len(aFlowline_in)
+    #aFlowline_out = list()
+    #for i in range(nFlowline):
+    #    pFlowline = aFlowline_in[i]          
+    #    pVertex_start = pFlowline.pVertex_start  
+    #    if check_head_water(aFlowline_in, pVertex_start)==1:
+    #        pFlowline.iStream_order = 1
+    #    else:
+    #        pFlowline.iStream_order = -1
+    #    
+    #    aFlowline_out.append(pFlowline)
+    #return aFlowline_out
 
 
 def define_stream_order(aFlowline_in, aConfluence_in):
     """define the stream order, but do we need to keep the confluence information?
 
     Args:
         aFlowline_in (_type_): _description_
@@ -50,93 +58,87 @@
         print ('data incomplete')
     else:       
         aStream_order = np.full(nFlowline, 0, dtype=int)  
         if iMethod == 1: #the new method
             nConfleunce = len(aConfluence_in)
             aFlag_confluence_treated = np.full(nConfleunce, 0, dtype=int)
             #build rtree for confluence
-            index_confluence = RTree( max_cap=5, min_cap=2)
-            for i in range(nConfleunce):
-                lID = i 
-                pVertex_confluence = aConfluence_in[i].pVertex_confluence 
-                x = pVertex_confluence.dLongitude_degree
-                y = pVertex_confluence.dLatitude_degree   
-                left =   x - 1E-5
-                right =  x + 1E-5
-                bottom = y - 1E-5
-                top =    y + 1E-5
-                pBound= (left, bottom, right, top)                
-                index_confluence.insert(lID, pBound)  #
+            index_confluence = RTree( max_cap=5, min_cap=2)          
+            for i, confluence in enumerate(aConfluence_in):
+                pVertex_confluence = confluence.pVertex_confluence 
+                x, y = pVertex_confluence.dLongitude_degree, pVertex_confluence.dLatitude_degree
+                pBound = (x - 1E-5, y - 1E-5, x + 1E-5, y + 1E-5)
+                index_confluence.insert(i, pBound)
 
           
             while aFlowline_in[0].iStream_order < 0:
                 for i in range(nConfleunce):
                     if aFlag_confluence_treated[i] == 1:
                         continue
 
                     pConfluence = aConfluence_in[i]
                     aFlowline_upstream = pConfluence.aFlowline_upstream 
                     pFlowline_downstream = pConfluence.pFlowline_downstream
                     iStream_segment = pFlowline_downstream.iStream_segment
-                    iFlag_upstream_done = 1
-                    nUpstream = len(aFlowline_upstream)
-                    aStrord = list()
-                    for j in range(nUpstream):
-                        pFlowline_upstream = aFlowline_upstream[j]
-                        iStream_order_upstream = pFlowline_upstream.iStream_order
-                        if iStream_order_upstream < 1:
-                            iFlag_upstream_done = 0
-                            break
-                        else:
-                            aStrord.append( iStream_order_upstream  )
-                        pass
+                    #iFlag_upstream_done = 1
+                    #nUpstream = len(aFlowline_upstream)
+                    aStrord = [upstream.iStream_order for upstream in aFlowline_upstream if upstream.iStream_order >= 1]
+      
+                    #aStrord = list()
+                    #for j in range(nUpstream):
+                    #    pFlowline_upstream = aFlowline_upstream[j]
+                    #    iStream_order_upstream = pFlowline_upstream.iStream_order
+                    #    if iStream_order_upstream < 1:
+                    #        iFlag_upstream_done = 0
+                    #        break
+                    #    else:
+                    #        aStrord.append( iStream_order_upstream  )               
 
-                    if iFlag_upstream_done == 1:
+                    #if iFlag_upstream_done == 1:
+                    if len(aStrord) == len(aFlowline_upstream):
                         aFlag_confluence_treated[i] = 1
                         #now we can process the downstream
                         #get unique value
-                        dummy = np.array(aStrord)
-                        dummy1 = np.unique(dummy)
-                        if len(dummy1) == 1: #all upstreams have the same order
-                            iStream_order = aStrord[0] + 1
-                        else:
-                            iStream_order = np.max(dummy)  
-                        pass
-                        
+                        iStream_order = max(aStrord) if len(set(aStrord)) > 1 else aStrord[0] + 1                        
+                                              
                         #update
                         pFlowline_downstream.iStream_order = iStream_order
                         aFlowline_in[nSegment-iStream_segment].iStream_order = iStream_order
                         #update confluence
-                        x = pFlowline_downstream.pVertex_end.dLongitude_degree
-                        y = pFlowline_downstream.pVertex_end.dLatitude_degree   
-                        left =   x - 1E-5
-                        right =  x + 1E-5
-                        bottom = y - 1E-5
-                        top =    y + 1E-5
-                        pBound= (left, bottom, right, top)  
+                        #x = pFlowline_downstream.pVertex_end.dLongitude_degree
+                        #y = pFlowline_downstream.pVertex_end.dLatitude_degree   
+                        #left =   x - 1E-5
+                        #right =  x + 1E-5
+                        #bottom = y - 1E-5
+                        #top =    y + 1E-5
+                        #pBound= (left, bottom, right, top)  
+                        #aIntersect = list(index_confluence.search(pBound))
+
+                        #update confluence
+                        x, y = pFlowline_downstream.pVertex_end.dLongitude_degree, pFlowline_downstream.pVertex_end.dLatitude_degree
+                        pBound = (x - 1E-5, y - 1E-5, x + 1E-5, y + 1E-5)
                         aIntersect = list(index_confluence.search(pBound))
+
                         for k in aIntersect:
                             pConfluence2 = aConfluence_in[k]
                             if pConfluence2.pVertex_confluence == pFlowline_downstream.pVertex_end:
                                 for pFlowline_upstream2 in pConfluence2.aFlowline_upstream:
                                     if pFlowline_upstream2.iStream_segment == iStream_segment:
                                         pFlowline_upstream2.iStream_order = iStream_order
                                         break
                             pass
 
                                              
-            for i in range(nFlowline):
-                pFlowline = aFlowline_in[i]      
-                pFlowline.iStream_order =    aFlowline_in[i].iStream_order   
-                aFlowline_out.append(pFlowline)
-                aStream_order[i] = pFlowline.iStream_order
+            
+            for i, flowline in enumerate(aFlowline_in):                
+                aFlowline_out.append(flowline)
+                aStream_order[i] = flowline.iStream_order
                 
-            pass
-        else: #the old method, not computationally efficient enough
-              
+      
+        else: #the old method, not computationally efficient enough              
             for i in range(nFlowline):
                 pFlowline = aFlowline_in[i]
                 pVertex_start=pFlowline.pVertex_start
                 if check_head_water(aFlowline_in, pVertex_start)==1:     
                     aStream_order[i] = 1
                     pass
```

### Comparing `pyflowline-0.3.4/pyflowline/algorithms/index/define_stream_segment_index.py` & `pyflowline-0.3.5/pyflowline/algorithms/index/define_stream_segment_index.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,33 @@
-from pyflowline.algorithms.auxiliary.check_head_water import check_head_water
+
 def define_stream_segment_index(aFlowline_in):
     """build stream segment index, because they are ordered from outlet to headwater, so the index is from 1 to n
 
     Args:
         aFlowline_in (_type_): _description_
 
     Returns:
         _type_: _description_
     """
     nFlowline = len(aFlowline_in)
-    aFlowline_out = list()
-    aStream_segment = list()
+    #aFlowline_out = list()
+    #aStream_segment = list()
+    #if nFlowline == 0 :
+    #    print ('data incomplete')
+    #else:  
+    #    for i in range(nFlowline):
+    #        pFlowline = aFlowline_in[i]
+    #        pFlowline.iStream_segment = nFlowline - i              
+    #        aStream_segment.append(pFlowline.iStream_segment)
+    #        aFlowline_out.append(pFlowline)
+    #    pass
+
     if nFlowline == 0 :
         print ('data incomplete')
-    else:  
-        for i in range(nFlowline):
-            pFlowline = aFlowline_in[i]
-            pFlowline.iStream_segment = nFlowline - i              
-            aStream_segment.append(pFlowline.iStream_segment)
-            aFlowline_out.append(pFlowline)
+        return [], []
+    
+    for i, pFlowline in enumerate(aFlowline_in, start=1):
+        pFlowline.iStream_segment = nFlowline - i + 1
 
-        pass
-    return aFlowline_out, aStream_segment
+    aStream_segment = [pFlowline.iStream_segment for pFlowline in aFlowline_in]
+    #return aFlowline_out, aStream_segment
+    return aFlowline_in, aStream_segment
```

### Comparing `pyflowline-0.3.4/pyflowline/algorithms/intersect/intersect_flowline_with_flowline.py` & `pyflowline-0.3.5/pyflowline/algorithms/intersect/intersect_flowline_with_flowline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import numpy as np
 from osgeo import ogr, osr
 #from shapely.wkt import loads
 from pyflowline.classes.vertex import pyvertex
 
-import importlib
+import importlib.util
 iFlag_cython = importlib.util.find_spec("cython") 
 if iFlag_cython is not None:
     from pyflowline.algorithms.cython.kernel import find_vertex_in_list
 else:
     from pyflowline.algorithms.auxiliary.find_vertex_in_list import find_vertex_in_list
 
 def intersect_flowline_with_flowline( sFilename_flowline_a_in, sFilename_flowline_b_in, sFilename_output_in):
@@ -78,26 +78,23 @@
         if (pGeometry_flowline_a.IsValid()):
             pass
         else:
             print('Geometry issue')
 
         #convert geometry to edge
         pGeometrytype_flowline_a = pGeometry_flowline_a.GetGeometryName()
-        if(pGeometrytype_flowline_a == 'LINESTRING'):            
-            
-                     
-            aFlowline_intersect = list()
+        if(pGeometrytype_flowline_a == 'LINESTRING'):                                                     
             iFlag_intersected = 0 
             for j in range (nfeature_flowline_b):
             #for pFeature_flowline in pLayer_flowline:
                 pFeature_flowline_b = pLayer_flowline_b.GetFeature(j)
                 pGeometry_flowline_b = pFeature_flowline_b.GetGeometryRef()
 
                 if iFlag_id ==1:
-                    lFlowlineID = pFeature_flowline_b.GetField("id")
+                    lFlowlineID = pFeature_flowline_b.GetField("lineid")
                 else:
                     lFlowlineID = -1
 
                 if (pGeometry_flowline_b.IsValid()):
                     pass
                 else:
                     print('Geometry issue')
```

### Comparing `pyflowline-0.3.4/pyflowline/algorithms/intersect/intersect_flowline_with_mesh.py` & `pyflowline-0.3.5/pyflowline/algorithms/intersect/intersect_flowline_with_mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
 import os
-import importlib
+import importlib.util
 import numpy as np
 from osgeo import ogr, osr
 #from shapely.wkt import loads
 
 from pyflowline.formats.convert_coordinates import convert_gcs_coordinates_to_cell
 from pyflowline.formats.convert_coordinates import convert_gcs_coordinates_to_flowline
-from pyflowline.external.pyearth.gis.gdal.gdal_functions import get_geometry_coords
+from pyearth.gis.location.get_geometry_coordinates import get_geometry_coordinates
 
 iFlag_cython = importlib.util.find_spec("cython") 
 if iFlag_cython is not None:
     from pyflowline.external.tinyr.tinyr.tinyr import RTree
     iFlag_use_rtree = 1
 else:
     iFlag_use_rtree =0
@@ -74,15 +74,15 @@
             pBound= (left, bottom, right, top)
             index_flowline.insert(lID, pBound)  #  
 
         #now intersect using rtree
         for j in range (nfeature_mesh):
             pFeature_mesh = pLayer_mesh.GetFeature(j)
             pGeometry_mesh = pFeature_mesh.GetGeometryRef()
-            aCoords_gcs = get_geometry_coords(pGeometry_mesh)
+            aCoords_gcs = get_geometry_coordinates(pGeometry_mesh)
             lCellID = pFeature_mesh.GetField("cellid")
             dLon = pFeature_mesh.GetField("longitude")
             dLat = pFeature_mesh.GetField("latitude")        
             dArea = pFeature_mesh.GetField("area")
             if (pGeometry_mesh.IsValid()):
                 pass
             else:
@@ -183,19 +183,16 @@
                 else:
                     pCell.iFlag_intersected = 0   
                     aCell.append(pCell)
                     pass
     else:        
           
         for pFeature_mesh in pLayer_mesh:       
-            pGeometry_mesh = pFeature_mesh.GetGeometryRef()        
-            #dummy0 = loads( pGeometry_mesh.ExportToWkt() )
-            #aCoords_gcs = dummy0.exterior.coords
-            #aCoords_gcs= np.array(aCoords_gcs)       
-            aCoords_gcs = get_geometry_coords(pGeometry_mesh)
+            pGeometry_mesh = pFeature_mesh.GetGeometryRef()                    
+            aCoords_gcs = get_geometry_coordinates(pGeometry_mesh)
 
             lCellID = pFeature_mesh.GetField("cellid")
             dLon = pFeature_mesh.GetField("longitude")
             dLat = pFeature_mesh.GetField("latitude")        
             dArea = pFeature_mesh.GetField("area")
             if (iFlag_transform ==1): 
                 pGeometry_mesh.Transform(transform)
```

### Comparing `pyflowline-0.3.4/pyflowline/algorithms/intersect/intersect_flowline_with_vertex.py` & `pyflowline-0.3.5/pyflowline/algorithms/intersect/intersect_flowline_with_vertex.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/pyflowline/algorithms/merge/merge_flowline.py` & `pyflowline-0.3.5/pyflowline/algorithms/merge/merge_flowline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 
 import numpy as np
-
-
-import importlib
+import importlib.util
 iFlag_cython = importlib.util.find_spec("cython") 
 if iFlag_cython is not None:
     from pyflowline.algorithms.cython.kernel import find_vertex_in_list
 else:
     from pyflowline.algorithms.auxiliary.find_vertex_in_list import find_vertex_in_list
 
 lID = 0
@@ -27,109 +25,114 @@
         aIndex_middle_in (_type_): _description_
         aIndex_confluence_in (_type_): _description_
 
     Returns:
         List: The flowline are strictly ordered from outlet to headwater
     """
 
-    nVertex=len(aVertex_in)
+    #nVertex=len(aVertex_in)
     nFlowline = len(aFlowline_in)
     aFlowline_out=list()               
     aVertex = np.array(aVertex_in)
     aIndex_headwater = np.array(aIndex_headwater_in)
     aIndex_middle = np.array(aIndex_middle_in)
     aIndex_confluence = np.array(aIndex_confluence_in)
     if aIndex_middle.size == 0:
-        return aFlowline_in
-    
-    aVertex_headwater=aVertex[aIndex_headwater]    
-    aVertex_middle=aVertex[aIndex_middle]   
+        return aFlowline_in 
+
+    #convert to set
+    aVertex_headwater_set = set(aVertex[aIndex_headwater])  
+    aVertex_middle_set = set(aVertex[aIndex_middle])  
+
     if aIndex_confluence.size > 0:        
-        iFlag_confluence = 1
-        aVertex_confluence=aVertex[aIndex_confluence]    
+        iFlag_confluence = 1  
+        aVertex_confluence_set = set(aVertex[aIndex_confluence])  
     else:
         iFlag_confluence = 0
-        pass
     
-    def merge_flowline_reach(lIndex_in, pVertex_start_in, pVertex_end_in):
+    # Build the dictionary
+    vertex_to_flowline = {flowline.pVertex_end: flowline for flowline in aFlowline_in}  
+
+    def merge_flowline_reach(lIndex_in, pVertex_start_in):
         global lID
         pFlowline = aFlowline_in[lIndex_in]
         iSegment = pFlowline.iStream_segment
         pVertex_current = pVertex_start_in
         
-        while (find_vertex_in_list(aVertex_middle.tolist(), pVertex_current)[0] ==1):            
-            for j in range(0, nFlowline):      
-                pFlowline2 = aFlowline_in[j]                
-                pVertex_start = pFlowline2.pVertex_start
-                pVertex_end = pFlowline2.pVertex_end
-                if pVertex_end == pVertex_current:
-                    pFlowline = pFlowline.merge_upstream(pFlowline2)
-                    pVertex_current = pVertex_start                    
-                    break
-                else:
-                    pass
-
+        #while (find_vertex_in_list(aVertex_middle.tolist(), pVertex_current)[0] ==1):            
+        while (pVertex_current in aVertex_middle_set): 
+            if pVertex_current in vertex_to_flowline:
+                pFlowline2 = vertex_to_flowline[pVertex_current]
+                pFlowline = pFlowline.merge_upstream(pFlowline2)
+                pVertex_current = pFlowline2.pVertex_start
+
+            #old method    
+            #for j in range(0, nFlowline):      
+            #    pFlowline2 = aFlowline_in[j]                
+            #    pVertex_start = pFlowline2.pVertex_start
+            #    pVertex_end = pFlowline2.pVertex_end
+            #    if pVertex_end == pVertex_current:
+            #        pFlowline = pFlowline.merge_upstream(pFlowline2)
+            #        pVertex_current = pVertex_start                    
+            #        break                
                
         #go to next 
-        if find_vertex_in_list(aVertex_headwater.tolist(), pVertex_current)[0] ==1: 
+        #if find_vertex_in_list(aVertex_headwater.tolist(), pVertex_current)[0] ==1: 
+        if pVertex_current in aVertex_headwater_set:
             pFlowline.iStream_segment = iSegment      
             pFlowline.iStream_order = 1           
             pFlowline.lFlowlineIndex = lID
             aFlowline_out.append(pFlowline)        
             lID = lID + 1 
             return
         else:
             pFlowline.iStream_segment = iSegment              
             pFlowline.lFlowlineIndex = lID
             aFlowline_out.append(pFlowline)        
             lID = lID + 1 
             #confluence
-            if find_vertex_in_list(aVertex_confluence.tolist(), pVertex_current)[0] ==1: 
+            #if find_vertex_in_list(aVertex_confluence.tolist(), pVertex_current)[0] ==1: 
+            if pVertex_current in aVertex_confluence_set:
                 for k in range(0, nFlowline):                      
                     pFlowline3 = aFlowline_in[k]                
                     pVertex_start = pFlowline3.pVertex_start
                     pVertex_end = pFlowline3.pVertex_end
                     if pVertex_end == pVertex_current:
-                        merge_flowline_reach(k, pVertex_start, pVertex_end)
-                                
-    
+                        merge_flowline_reach(k, pVertex_start)
+                               
+        
     #find outlet
-    iFlag_first=1
+    dDiatance_min = float('inf')
     for i in range(nFlowline):        
         pFlowline = aFlowline_in[i]                
-        pVertex_start = pFlowline.pVertex_start
         pVertex_end = pFlowline.pVertex_end
-        dDiatance = pVertex_end.calculate_distance( pVertex_outlet_in)
-        if iFlag_first ==1:
-            dDiatance_min = dDiatance                
-            lIndex_outlet = i            
-            iFlag_first=0    
-        else:            
-            if  dDiatance < dDiatance_min:
-                dDiatance_min = dDiatance           
-                lIndex_outlet = i                
-                pass    
-            else:
-                pass
+        dDiatance = pVertex_end.calculate_distance(pVertex_outlet_in)
+        if dDiatance < dDiatance_min:
+            dDiatance_min = dDiatance
+            lIndex_outlet = i
             
     pFlowline = aFlowline_in[lIndex_outlet]            
     pVertex_start = pFlowline.pVertex_start
     pVertex_end = pFlowline.pVertex_end   
 
+    
+
     #now start from outlet
     if iFlag_confluence == 1:
         #check whether outlet is a confluence
-        if  (find_vertex_in_list(aVertex_confluence.tolist(), pVertex_end)[0] ==1):
+        #if  (find_vertex_in_list(aVertex_confluence.tolist(), pVertex_end)[0] ==1):
+        if pVertex_end in aVertex_confluence_set:
+            #if pVertex_end in end_vertex_to_flowline:
+            #    merge_flowline_reach(end_vertex_to_flowline[pVertex_end], pVertex_start_dummy)      
             for i in range(nFlowline):
                 pFlowline = aFlowline_in[i]  
                 pVertex_start_dummy = pFlowline.pVertex_start
                 pVertex_end_dummy = pFlowline.pVertex_end
-
                 if pVertex_end == pVertex_end_dummy:
                     #this is 
-                    merge_flowline_reach(i, pVertex_start_dummy, pVertex_end_dummy)  
-            pass
+                    merge_flowline_reach(i, pVertex_start_dummy)  
+            
         else:
-            merge_flowline_reach(lIndex_outlet, pVertex_start, pVertex_end)   
+            merge_flowline_reach(lIndex_outlet, pVertex_start)   
     else:
-        merge_flowline_reach(lIndex_outlet, pVertex_start, pVertex_end)   
+        merge_flowline_reach(lIndex_outlet, pVertex_start)   
     return aFlowline_out
```

### Comparing `pyflowline-0.3.4/pyflowline/algorithms/simplification/remove_returning_flowline.py` & `pyflowline-0.3.5/pyflowline/algorithms/simplification/remove_returning_flowline.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,106 +1,94 @@
 import copy
 import numpy as np
 from pyflowline.formats.convert_coordinates import convert_gcs_coordinates_to_flowline
-from pyflowline.algorithms.auxiliary.find_index_in_list import check_if_duplicates
 
 def remove_returning_flowline(iMesh_type_in, aCell_intersect_in, pVertex_outlet_in):    
     aFlowline_out=list()    
     nCell =  len(aCell_intersect_in)
+    #lCellID_to_cell = {cell.lCellID: cell for cell in aCell_intersect_in}
     def simplify_list(aCell_flowline_in):
         aCell_flowline_out = copy.deepcopy(aCell_flowline_in)
         nCell2 = len(aCell_flowline_out)          
-        iFlag_unique = check_if_duplicates(aCell_flowline_out)
-        if iFlag_unique == 1:
+        #iFlag_unique = check_if_duplicates(aCell_flowline_out)
+        if int(len(aCell_flowline_out) == len(set(aCell_flowline_out))) :
             return aCell_flowline_out
         else:
             for i in range(nCell2):
                 elem=aCell_flowline_out[i]
                 if aCell_flowline_out.count(elem) > 1:
                     dummy = [i for i, x in enumerate(aCell_flowline_out) if x == elem]                    
                     start = dummy[0]
                     end = dummy[-1]
                     del aCell_flowline_out[start: end]                     
-                    break                    
-                else:
-                    pass
-
-                pass             
+                    break                                              
             
             aCell_flowline_out = simplify_list(aCell_flowline_out)
         return   aCell_flowline_out
-
+      
     def retrieve_flowline_intersect_index(iSegment_in, iStream_order_in, pVertex_end_in):
+        lCellID =-1       
         iFlag_found = 1
         pVertex_end_current = pVertex_end_in
         aCell_flowline=list()  
         aSegment_upstream = list()
         aVertex_end_upstream = list()
         aStream_order = list()
         iFlag_skip = 0
         iFlag_previous_overlap=0
         while iFlag_found == 1:
-            iFlag_found = 0             
+            iFlag_found = 0                       
             for j in range(nCell):
                 pCell = aCell_intersect_in[j]
-                lCellID = pCell.lCellID
+                lCellID = pCell.lCellID               
                 aFlowline= pCell.aFlowline
                 nFlowline = len(aFlowline)
                 for i in range(nFlowline):
                     pFlowline = aFlowline[i]
                     pVertex_start = pFlowline.pVertex_start
                     pVertex_end = pFlowline.pVertex_end
                     iStream_segment = pFlowline.iStream_segment
                     iStream_order = pFlowline.iStream_order
                     if pVertex_end == pVertex_end_current: #be careful because this function is strict
                         if iStream_segment == iSegment_in:                            
                             dLength = pFlowline.dLength
                             iFlag_found2, dummy2 = pCell.which_edge_cross_this_vertex(pVertex_start)
                             iFlag_found3, dummy3 = pCell.which_edge_cross_this_vertex(pVertex_end)
-
                             if iFlag_found2 == 1 and iFlag_found3 == 1: #on the edge
                                 #same edge
                                 if dummy2.is_overlap(dummy3) ==1:                                    
                                     pVertex_end_current = pVertex_start    
-                                    aCell_flowline.append(lCellID)
-                                    #print(lCellID)
+                                    aCell_flowline.append(lCellID)                                    
                                     iFlag_found = 1                
                                     iFlag_previous_overlap =1
                                     
                                     pass
                                 else:
                                     if dLength < (0.1*pCell.dLength) : #because it taks a short cut                                        
                                         pVertex_end_current = pVertex_start   
                                         iFlag_found = 1                                          
                                         if iFlag_previous_overlap ==1: 
-                                            aCell_flowline.append(lCellID)              
-                                            #print(lCellID)
+                                            aCell_flowline.append(lCellID)  
                                             iFlag_previous_overlap=0
                                             pass
                                         else:
                                             iFlag_previous_overlap=1
                                             pass                                             
                                         pass
                                     else:
                                         pVertex_end_current = pVertex_start    
                                         aCell_flowline.append(lCellID)
-                                        #print(lCellID)
-                                        iFlag_found = 1                                      
-                                        pass
-
-                                    pass                                
-
-                                pass
+                                        iFlag_found = 1                                     
+                                      
 
                             else:
                                 pVertex_end_current = pVertex_start    
                                 aCell_flowline.append(lCellID)                                
                                 iFlag_found = 1
-                                iFlag_previous_overlap=0
-                                pass                            
+                                iFlag_previous_overlap=0                                                       
                                 
                             break
                             
                         else:
                             iFlag_found2, dummy2 = pCell.which_edge_cross_this_vertex(pVertex_start)
                             iFlag_found3, dummy3 = pCell.which_edge_cross_this_vertex(pVertex_end)
                             if pVertex_end == pVertex_end_in: 
@@ -119,76 +107,60 @@
 
                 if iFlag_found == 1:
                     break
         
         #should have finished search
         if iFlag_found == 0:
             #reverse 
-            aCell_flowline = aCell_flowline[::-1]
+            aCell_flowline = aCell_flowline[::-1]          
             #simplify list         
             aCell_simple = simplify_list(aCell_flowline)
             #save the output
             nCell3 = len(aCell_simple)
             aCoordinates = list()            
             if nCell3 >1:
                 for i in range(nCell3):
                     lCellID = aCell_simple[i]
                     for j in range( nCell):
                         if aCell_intersect_in[j].lCellID == lCellID:    
                             x = aCell_intersect_in[j].dLongitude_center_degree
                             y = aCell_intersect_in[j].dLatitude_center_degree                
                             aCoordinates.append([x,y])
-                    pass
+                 
                 pFlowline = convert_gcs_coordinates_to_flowline(aCoordinates)
                 pFlowline.iStream_segment = iSegment_in
                 pFlowline.iStream_order=iStream_order_in
                 aFlowline_out.append(pFlowline)
 
             sort_index = np.argsort(aStream_order)            
-            sort_index = sort_index[::-1]
-            nUpstream = len(aSegment_upstream)
+            #sort_index = sort_index[::-1] #can we process low order first?
+            #nUpstream = len(aSegment_upstream)
             for i in sort_index:
                 retrieve_flowline_intersect_index(aSegment_upstream[i], aStream_order[i], aVertex_end_upstream[i])
                 pass
             pass
 
         return 
-
-    #starting from the outlet
-    dDiatance_min=0.0
-    iFlag_first=1
-    for j in range(nCell):
-        pCell = aCell_intersect_in[j]
-        aFlowline= pCell.aFlowline
-        nFlowline = len(aFlowline)
-        for i in range(nFlowline):
-            pFlowline = aFlowline[i]
-            pVertex_start = pFlowline.pVertex_start
-            pVertex_end = pFlowline.pVertex_end
-            dDiatance = pVertex_end.calculate_distance( pVertex_outlet_in)
-            if iFlag_first ==1:
-                dDiatance_min = dDiatance               
-                lCellID_outlet = pCell.lCellID               
+    
+    dDiatance_min = float('inf')
+    lCellID_outlet = lCellID_outlet2 = lCellID_outlet3 = None    
+    for j, pCell in enumerate(aCell_intersect_in):
+        for i, pFlowline in enumerate(pCell.aFlowline):
+            dDiatance = pFlowline.pVertex_end.calculate_distance(pVertex_outlet_in)
+            if dDiatance < dDiatance_min:
+                dDiatance_min = dDiatance
+                lCellID_outlet = pCell.lCellID
                 lCellID_outlet2 = j
                 lCellID_outlet3 = i
-                iFlag_first=0
-            else:
-                if  dDiatance < dDiatance_min:
-                    dDiatance_min = dDiatance                
-                    lCellID_outlet = pCell.lCellID                
-                    lCellID_outlet2 = j
-                    lCellID_outlet3 = i
-                    pass    
-                else:
-                    pass
-
-            pass     
 
     #loop through       
     pFlowline = aCell_intersect_in[lCellID_outlet2].aFlowline[lCellID_outlet3]
     iStream_segment =pFlowline.iStream_segment
     iStream_order=pFlowline.iStream_order
     pVertex_outlet=pFlowline.pVertex_end
         
     retrieve_flowline_intersect_index(iStream_segment, iStream_order, pVertex_outlet)
 
+    #update outlet location since the conceptual flowline use center
+    pVertex_outlet =  aFlowline_out[0].pVertex_end
+
     return aFlowline_out, lCellID_outlet, pVertex_outlet
```

### Comparing `pyflowline-0.3.4/pyflowline/algorithms/simplification/remove_small_river.py` & `pyflowline-0.3.5/pyflowline/algorithms/simplification/remove_small_river.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,55 @@
-from pyflowline.algorithms.auxiliary.check_head_water import check_head_water
 def remove_small_river(aFlowline_in, dThreshold_in):
     """Remove small river that meet the threshold and headwater requirement, also dam flowline are reserved
 
     Args:
         aFlowline_in (_type_): _description_
         dThreshold_in (_type_): _description_
 
     Returns:
         List: Theortically, the flowline should be ordered from outlet to headwater
-    """
-    nFlowline = len(aFlowline_in)
-    aFlowline_out=list()        
-    if nFlowline == 1:
-        aFlowline_out.append(aFlowline_in[0])
+    """  
+         
+    if len(aFlowline_in) == 1:
+        return [aFlowline_in[0]]
     else:
+        aFlowline_out=list()   
         lID = 0        
-        for i in range(nFlowline):
-            pFlowline = aFlowline_in[i]      
-            iFlag_dam = pFlowline.iFlag_dam
-            pVertex_start = pFlowline.pVertex_start
-            pVertex_end = pFlowline.pVertex_end
+        for pFlowline in aFlowline_in:            
+            iFlag_dam = pFlowline.iFlag_dam           
             dLength = pFlowline.calculate_length()
-            if iFlag_dam ==1:
+            if iFlag_dam == 1 or pFlowline.iStream_order != 1 or dLength > dThreshold_in:
                 pFlowline.lFlowlineIndex = lID
                 aFlowline_out.append(pFlowline)
-                lID = lID +1       
-            else:
-                if pFlowline.iStream_order == 1:
-                    if dLength > dThreshold_in :
-                        pFlowline.lFlowlineIndex = lID
-                        aFlowline_out.append(pFlowline)
-                        lID = lID + 1 
-                        pass
-                    else:
-                        pass
-                    pass
-                else: #this one might be not used     
-                    pFlowline.lFlowlineIndex = lID
-                    aFlowline_out.append(pFlowline)
-                    lID = lID +1       
-                    pass        
+                lID += 1
+            #if iFlag_dam ==1:
+            #    pFlowline.lFlowlineIndex = lID
+            #    aFlowline_out.append(pFlowline)
+            #    lID = lID +1       
+            #else:
+            #    if pFlowline.iStream_order == 1:
+            #        if dLength > dThreshold_in :
+            #            pFlowline.lFlowlineIndex = lID
+            #            aFlowline_out.append(pFlowline)
+            #            lID = lID + 1                        
+            #    else: #this one might be not used     
+            #        pFlowline.lFlowlineIndex = lID
+            #        aFlowline_out.append(pFlowline)
+            #        lID = lID +1       
+            #        pass        
                     #if check_head_water(aFlowline_in, pVertex_start)==1:
                     #    if dLength > dThreshold_in :
                     #        pFlowline.lIndex = lID
                     #        aFlowline_out.append(pFlowline)
                     #        lID = lID + 1 
                     #        pass
                     #    else:
                     #        pass
                     #else:        
                     #    pFlowline.lIndex = lID
                     #    aFlowline_out.append(pFlowline)
                     #    lID = lID +1       
                     #    pass            
             
-            pass    
+           
 
     return aFlowline_out
```

### Comparing `pyflowline-0.3.4/pyflowline/algorithms/split/find_flowline_confluence.py` & `pyflowline-0.3.5/pyflowline/algorithms/split/find_flowline_confluence.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 
 import numpy as np
-
-#from pyflowline.algorithms.auxiliary.check_head_water import check_head_water
-
-
-import importlib
+import importlib.util
 iFlag_cython = importlib.util.find_spec("cython") 
 
 from pyflowline.algorithms.split.find_flowline_vertex import find_flowline_vertex
 if iFlag_cython is not None:
     from pyflowline.algorithms.cython.kernel import add_unique_vertex
     from pyflowline.algorithms.cython.kernel import find_vertex_in_list
 else:
@@ -21,106 +17,118 @@
     Args:
         aFlowline_in (_type_): _description_
         pVertex_outlet_in (_type_): _description_
 
     Returns:
         List: _description_
     """
-
-    nFlowline = len(aFlowline_in) 
     aVertex=list()
     aIndex_headwater=list()
     aIndex_confluence=list()
     aIndex_middle =list()
     lIndex_outlet = -1
+    aVertex = find_flowline_vertex(aFlowline_in)
+    vertex_to_index = {vertex: index for index, vertex in enumerate(aVertex)}
+    nVertex=len(aVertex)
+    aConnectivity  = np.full(  nVertex , 0, dtype=int )
+    #iFlag_first=1
+    #for i in range(nVertex):        
+    #    pVertex = aVertex[i]
+    #    dDiatance = pVertex.calculate_distance( pVertex_outlet_in) 
+    #    if iFlag_first ==1:
+    #        dDiatance_min = dDiatance                
+    #        lIndex_outlet = i            
+    #        pVertex_outlet_out =  pVertex
+    #        iFlag_first=0
+    #    else:
+    #        if  dDiatance < dDiatance_min:
+    #            dDiatance_min = dDiatance
+    #            #found it
+    #            lIndex_outlet = i       
+    #            pVertex_outlet_out =  pVertex
+    #            pass    
+    #        else:
+    #            pass
+
+    distances = [vertex.calculate_distance(pVertex_outlet_in) for vertex in aVertex]
+    lIndex_outlet = np.argmin(distances)
+    pVertex_outlet_out = aVertex[lIndex_outlet]
+    #a outlet can be a confluence, so we won't set it     
+    aConnectivity[lIndex_outlet] =0 
 
-    #add all the flowline start and end vertex into a host list
-    #because the flowlines are order from outlet to headwater, there is no order in vertex list
     #for i in range(0, nFlowline):      
     #    pFlowline = aFlowline_in[i]
     #    pVertex_start = pFlowline.pVertex_start
     #    pVertex_end = pFlowline.pVertex_end
-    #    aVertex, dummy = add_unique_vertex(aVertex, pVertex_start)
-    #    aVertex, dummy = add_unique_vertex(aVertex, pVertex_end)
-    #    pass
-
-    aVertex = find_flowline_vertex(aFlowline_in)
-
-    nVertex=len(aVertex)
-    aConnectivity  = np.full(  nVertex , 0, dtype=int )
-    iFlag_first=1
-    for i in range(nVertex):        
-        pVertex = aVertex[i]
-        dDiatance = pVertex.calculate_distance( pVertex_outlet_in) 
-        if iFlag_first ==1:
-            dDiatance_min = dDiatance                
-            lIndex_outlet = i            
-            pVertex_outlet_out =  pVertex
-            iFlag_first=0
-        else:
-            if  dDiatance < dDiatance_min:
-                dDiatance_min = dDiatance
-                #found it
-                lIndex_outlet = i       
-                pVertex_outlet_out =  pVertex
-                pass    
-            else:
-                pass
-
-    #a outlet can be a confluence, so we won't set it     
-    #aConnectivity[lIndex_outlet] =0 
-    for i in range(0, nFlowline):      
-        pFlowline = aFlowline_in[i]
+    #    
+    #    iFlag_exist, lIndex =  find_vertex_in_list(aVertex, pVertex_end)  
+    #    if lIndex != lIndex_outlet:
+    #        #if check_head_water(aFlowline_in, pVertex_start)==1:
+    #        if pFlowline.iStream_order == 1:
+    #            iFlag_exist, lIndex =  find_vertex_in_list(aVertex, pVertex_start)            
+    #            aConnectivity[lIndex] = 1
+    #            iFlag_exist, lIndex =  find_vertex_in_list(aVertex, pVertex_end)            
+    #            aConnectivity[lIndex] = aConnectivity[lIndex] + 1        
+    #        else:
+    #            #middle point, or confluence
+    #            iFlag_exist, lIndex =  find_vertex_in_list(aVertex, pVertex_start)
+    #            if iFlag_exist ==1:
+    #                aConnectivity[lIndex] = aConnectivity[lIndex] + 1
+#
+    #            iFlag_exist, lIndex =  find_vertex_in_list(aVertex, pVertex_end)
+    #            if iFlag_exist ==1:
+    #                aConnectivity[lIndex] = aConnectivity[lIndex] + 1
+    #    else:
+    #        #it is outlet, but an outlet can be a confluence as well
+    #        iFlag_exist, lIndex =  find_vertex_in_list(aVertex, pVertex_start)
+    #        if iFlag_exist ==1:
+    #            aConnectivity[lIndex] = aConnectivity[lIndex] + 1
+    #        iFlag_exist, lIndex =  find_vertex_in_list(aVertex, pVertex_end)
+    #        if iFlag_exist ==1:
+    #            aConnectivity[lIndex] = aConnectivity[lIndex] + 1
+    #        pass
+    for pFlowline in aFlowline_in:
         pVertex_start = pFlowline.pVertex_start
         pVertex_end = pFlowline.pVertex_end
-        
-        iFlag_exist, lIndex =  find_vertex_in_list(aVertex, pVertex_end)  
-        if lIndex != lIndex_outlet:
-
-            #if check_head_water(aFlowline_in, pVertex_start)==1:
+        lIndex_end = vertex_to_index.get(pVertex_end)
+        if lIndex_end != lIndex_outlet:
             if pFlowline.iStream_order == 1:
-                iFlag_exist, lIndex =  find_vertex_in_list(aVertex, pVertex_start)            
-                aConnectivity[lIndex] = 1
-                iFlag_exist, lIndex =  find_vertex_in_list(aVertex, pVertex_end)            
-                aConnectivity[lIndex] = aConnectivity[lIndex] + 1        
+                lIndex_start = vertex_to_index.get(pVertex_start)
+                aConnectivity[lIndex_start] = 1
+                aConnectivity[lIndex_end] += 1
             else:
-                #middle point, or confluence
-                iFlag_exist, lIndex =  find_vertex_in_list(aVertex, pVertex_start)
-                if iFlag_exist ==1:
-                    aConnectivity[lIndex] = aConnectivity[lIndex] + 1
-
-                iFlag_exist, lIndex =  find_vertex_in_list(aVertex, pVertex_end)
-                if iFlag_exist ==1:
-                    aConnectivity[lIndex] = aConnectivity[lIndex] + 1
+                lIndex_start = vertex_to_index.get(pVertex_start)
+                if lIndex_start is not None:
+                    aConnectivity[lIndex_start] += 1
+                if lIndex_end is not None:
+                    aConnectivity[lIndex_end] += 1
         else:
-            #it is outlet, but an outlet can be a confluence as well
-            iFlag_exist, lIndex =  find_vertex_in_list(aVertex, pVertex_start)
-            if iFlag_exist ==1:
-                aConnectivity[lIndex] = aConnectivity[lIndex] + 1
-            iFlag_exist, lIndex =  find_vertex_in_list(aVertex, pVertex_end)
-            if iFlag_exist ==1:
-                aConnectivity[lIndex] = aConnectivity[lIndex] + 1
-            pass
-
+            lIndex_start = vertex_to_index.get(pVertex_start)
+            if lIndex_start is not None:
+                aConnectivity[lIndex_start] += 1
+            if lIndex_end is not None:
+                aConnectivity[lIndex_end] += 1
     #reset outlet
-    #aConnectivity[lIndex_outlet] = 0
-    for i in range(0, nVertex): 
-        if i == lIndex_outlet:
-            if (aConnectivity[i] >1):
-                aIndex_confluence.append(i)
-                pass
-            pass
-        else:
-            if (aConnectivity[i] >=3):
-                aIndex_confluence.append(i)
-            else:
-                if (aConnectivity[i] ==1):
-                    aIndex_headwater.append(i)
-                else:
-                    if (aConnectivity[i] ==2):  
-                        aIndex_middle.append(i)
-                    else:
-                        #this is outlet
-                        pass
-
-
+    #for i in range(0, nVertex): 
+    #    if i == lIndex_outlet:
+    #        if (aConnectivity[i] >1):
+    #            aIndex_confluence.append(i)
+    #            pass
+    #        pass
+    #    else:
+    #        if (aConnectivity[i] >=3):
+    #            aIndex_confluence.append(i)
+    #        else:
+    #            if (aConnectivity[i] ==1):
+    #                aIndex_headwater.append(i)
+    #            else:
+    #                if (aConnectivity[i] ==2):  
+    #                    aIndex_middle.append(i)
+    #                else:
+    #                    #this is outlet
+    #                    pass
+
+    aIndex_headwater = [i for i, x in enumerate(aConnectivity) if x == 1 and i != lIndex_outlet]
+    aIndex_middle = [i for i, x in enumerate(aConnectivity) if x == 2 and i != lIndex_outlet]
+    aIndex_confluence = [i for i, x in enumerate(aConnectivity) if x >= 3 or (i == lIndex_outlet and x > 1)]
+                    
     return aVertex, lIndex_outlet, aIndex_headwater, aIndex_middle, aIndex_confluence, aConnectivity, pVertex_outlet_out
```

### Comparing `pyflowline-0.3.4/pyflowline/algorithms/split/find_flowline_vertex.py` & `pyflowline-0.3.5/pyflowline/algorithms/split/find_flowline_vertex.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-
-
-import importlib
+import importlib.util
 iFlag_cython = importlib.util.find_spec("cython") 
 if iFlag_cython is not None:
     from pyflowline.algorithms.cython.kernel import add_unique_vertex
 else:
     from pyflowline.algorithms.auxiliary.find_index_in_list import add_unique_vertex
 
 def find_flowline_vertex(aFlowline_in, dThreshold_in=1.0E-6): 
@@ -14,38 +12,29 @@
         aFlowline_in (_type_): _description_
         dThreshold_in (_type_, optional): _description_. Defaults to 1.0E-6.
 
     Returns:
         _type_: _description_
     """
     aVertex = set()
-    nFlowline = len(aFlowline_in) 
+    #nFlowline = len(aFlowline_in) 
     #set up index and id first
     lVertexID = 1
     
-    for i in range(0, nFlowline):
-        pFlowline = aFlowline_in[i]        
-        #update the start and end vertex
+    for pFlowline in aFlowline_in:
         pFlowline.pVertex_start.lVertexID = lVertexID
-        lVertexID = lVertexID + 1
+        pFlowline.pVertex_start.lFlowlineID = pFlowline.lFlowlineID
+        lVertexID += 1
         pFlowline.pVertex_end.lVertexID = lVertexID
-        lVertexID = lVertexID + 1
-        aVertex.add(pFlowline.pVertex_start) 
-        aVertex.add(pFlowline.pVertex_end)         
-        pass
+        pFlowline.pVertex_end.lFlowlineID = pFlowline.lFlowlineID
+        lVertexID += 1
+        aVertex.update([pFlowline.pVertex_start, pFlowline.pVertex_end])
 
     #conver the set back to list
-    aVertex=list(aVertex)
-    #for i in range(0, nFlowline):      
-    #    pFlowline = aFlowline_in[i]
-    #    pVertex_start = pFlowline.pVertex_start
-    #    pVertex_end = pFlowline.pVertex_end        
-    #    aVertex, dummy = add_unique_vertex(aVertex, pVertex_start,dThreshold_in)
-    #    aVertex, dummy = add_unique_vertex(aVertex, pVertex_end, dThreshold_in)
-    #    pass
+    aVertex=list(aVertex)  
 
     return aVertex
 
 def find_flowline_vertex_old(aFlowline_in, dThreshold_in=1.0E-6): 
     aVertex = list()
     nFlowline = len(aFlowline_in)    
     aVertex=list(aVertex)
```

### Comparing `pyflowline-0.3.4/pyflowline/algorithms/split/split_by_length.py` & `pyflowline-0.3.5/pyflowline/algorithms/split/split_by_length.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/pyflowline/algorithms/split/split_flowline.py` & `pyflowline-0.3.5/pyflowline/algorithms/split/split_flowline.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 import numpy as np
 from pyflowline.classes.edge import pyedge
 from pyflowline.classes.flowline import pyflowline
 
-import importlib
+import importlib.util
 iFlag_cython = importlib.util.find_spec("cython") 
 if iFlag_cython is not None:
     from pyflowline.algorithms.cython.kernel import find_vertex_on_edge
     from pyflowline.algorithms.cython.kernel import find_vertex_in_list
   
 else:
     from pyflowline.algorithms.auxiliary.find_index_in_list import find_vertex_on_edge    
@@ -23,122 +23,134 @@
         iFlag_intersect: 1: a vertex maybe on a line, but it is not a vertex of the line
         iFlag_use_id: 1: 
     Output:
         aFlowline_out: list of flowline
     """
     aFlowline_out = list()
     nFlowline = len(aFlowline_in)
-    
+    aVertex_in_set = set(aVertex_in)     
+
     for i in range(nFlowline):
         pFlowline = aFlowline_in[i]
         iStream_order = pFlowline.iStream_order
-        iStream_segment = pFlowline.iStream_segment
-        lFlowlineID = pFlowline.lFlowlineID        
+        #iStream_segment = pFlowline.iStream_segment          
         iFlag_dam = pFlowline.iFlag_dam
-        nVertex = pFlowline.nVertex
+        #nVertex = pFlowline.nVertex
         nEdge= pFlowline.nEdge
         iPart = 0        
         aVertex  = list() #the actual vertex of ROI
         aVertex_all = list() #include vertex that is not ROI, but we need them to subset 
         for j in range(nEdge):
             pEdge=pFlowline.aEdge[j]
             pVertex = pEdge.pVertex_start
             aVertex_all.append(pVertex)
             #get the start first
-            iFlag_exist, lIndex = find_vertex_in_list( aVertex_in,  pVertex)
-            if iFlag_exist == 1:                
-                iPart = iPart + 1
-                aVertex.append(pVertex)   
-                pass
+            #iFlag_exist, lIndex = find_vertex_in_list( aVertex_in,  pVertex)
+            #if iFlag_exist == 1:                
+            #    iPart = iPart + 1
+            #    aVertex.append(pVertex)   
+            #    pass
+
+            if pVertex in aVertex_in_set:                
+                iPart += 1
+                aVertex.append(pVertex)
 
             if iFlag_intersect is not None:
                 if iFlag_use_id is not None:
                     aDistance = list()
                     iFlag_exist=0
                     aVertex_dummy=list()
                     aIndex=list()
                     npoint =0
                     for k in range(len(aVertex_in)):
                         pVertex = aVertex_in[k]
-                        if pVertex.lFlowlineID == lFlowlineID:
+                        if pVertex.lFlowlineID == pFlowline.lFlowlineID:
                             iFlag_exist =1
                             iPart = iPart + 1                            
                             distance  = pEdge.pVertex_start.calculate_distance(pVertex)
                             aDistance.append(distance)
                             aVertex_dummy.append(pVertex)
                             aIndex.append(k) 
                             npoint= npoint+ 1
                             
                     #sort needed
-                    if iFlag_exist == 1 :
-                        x = np.array(aDistance)
-                        b = np.argsort(x)
-                        c = np.array(aIndex)
-                        d= c[b]
-                        aIndex_order = list(d)
-                        #then push back
-                        for k in range(npoint):
-                            pVertex_dummy = aVertex_in[ aIndex_order[k]  ] 
+                    #if iFlag_exist == 1 :
+                    #    x = np.array(aDistance)
+                    #    b = np.argsort(x)
+                    #    c = np.array(aIndex)
+                    #    d= c[b]
+                    #    aIndex_order = list(d)
+                    #    #then push back
+                    #    for k in range(npoint):
+                    #        pVertex_dummy = aVertex_in[ aIndex_order[k]  ] 
+                    #        aVertex.append(pVertex_dummy)
+                    #        aVertex_all.append(pVertex_dummy)
+                    #        pass
+                    if aDistance:
+                        aIndex_order = np.argsort(aDistance)
+                        for k in aIndex_order:
+                            pVertex_dummy = aVertex_in[k] 
                             aVertex.append(pVertex_dummy)
                             aVertex_all.append(pVertex_dummy)
-                            pass
 
                 else:
                     iFlag_exist, npoint, aIndex = find_vertex_on_edge( aVertex_in, pEdge)
                     #they must be ordered
                     if iFlag_exist==1:
                         for m in range(npoint):
                             pVertex_dummy = aVertex_in[aIndex[m]]
                             iPart = iPart + 1
                             aVertex.append(pVertex_dummy)
                             aVertex_all.append(pVertex_dummy)
-                            pass
-                        pass
+                          
 
         #the last ending vertex
         pVertex = pFlowline.pVertex_end
         aVertex_all.append(pVertex)
-        iFlag_exist, lIndex = find_vertex_in_list( aVertex_in,  pVertex)
-        if iFlag_exist == 1:
+        #iFlag_exist, lIndex = find_vertex_in_list( aVertex_in,  pVertex)
+        #if iFlag_exist == 1:
+        if pVertex in aVertex_in_set:
             iPart = iPart + 1
-            aVertex.append(pVertex)
-            pass
+            aVertex.append(pVertex)            
         if iPart == 0 :
-            print('Something is wrong')
-            pass
+            print('Something is wrong')            
         else:
             if iPart ==1:
                 #print('This flowline does not form any loop')
                 if iFlag_use_id is not None:
                     pass
                 pass
             else:
                 if iPart >=2:
                     nLine = iPart-1
                     #rebuild index
-                    aVertex_index =list()
-                    for m in range(iPart):
-                        pVertex= aVertex[m]
-                        iFlag_exist, lIndex = find_vertex_in_list( aVertex_all,  pVertex)
-                        if iFlag_exist ==1:
-                            aVertex_index.append(lIndex)
-                            pass
+                    #aVertex_index =list()
+                    #for m in range(iPart):
+                    #    pVertex= aVertex[m]
+                    #    iFlag_exist, lIndex = find_vertex_in_list( aVertex_all,  pVertex)
+                    #    if iFlag_exist ==1:
+                    #        aVertex_index.append(lIndex)
+                    #        pass
+                    
+                    aVertex_index = [aVertex_all.index(pVertex) for pVertex in aVertex if pVertex in aVertex_all]
+          
 
                     #find duplicate
                     for k in range(nLine):
                         t = aVertex_index[k]
                         s = aVertex_index[k+1]
                         if s!=t:
-                            aEdge=list()
-                            for l in range(t,s):
-                                pVertex0 = aVertex_all[l]  
-                                pVertex1 = aVertex_all[l+1]  
-                                pEdge = pyedge(pVertex0, pVertex1)
-                                aEdge.append(pEdge)
-                                pass
+                            #aEdge=list()
+                            #for l in range(t,s):
+                            #    pVertex0 = aVertex_all[l]  
+                            #    pVertex1 = aVertex_all[l+1]  
+                            #    pEdge = pyedge(pVertex0, pVertex1)
+                            #    aEdge.append(pEdge)
+                            #    pass
+                            aEdge=[pyedge(aVertex_all[l], aVertex_all[l+1]) for l in range(t,s)]
 
                             pFlowline1 = pyflowline(aEdge)
                             pFlowline1.iStream_order = iStream_order
                             pFlowline1.iFlag_dam = iFlag_dam
                             aFlowline_out.append(pFlowline1)
                         pass                    
                     pass
```

### Comparing `pyflowline-0.3.4/pyflowline/algorithms/split/split_flowline_to_edge.py` & `pyflowline-0.3.5/pyflowline/algorithms/split/split_flowline_to_edge.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from pyflowline.classes.flowline import pyflowline
 def split_flowline_to_edge(aFlowline_in):
     aFlowline_out = list()
     aEdge_out=list()
-    nFlowline = len(aFlowline_in)
-    for i in range(nFlowline):
-        pFlowline = aFlowline_in[i]
-        iStream_order = pFlowline.iStream_order
-        nVertex = pFlowline.nVertex
-        nEdge = pFlowline.nEdge
-        iPart = 0        
-        for j in range(nEdge):
-            pEdge = pFlowline.aEdge[j]
-            aEdge = list()
-            aEdge.append(pEdge)
-            aEdge_out.append(pEdge)            
-            pFlowline1 = pyflowline(aEdge)      
-            aFlowline_out.append(pFlowline1)    
-            pass
-        pass   
+    #nFlowline = len(aFlowline_in)
+    #for i in range(nFlowline):
+    #    pFlowline = aFlowline_in[i]     
+    #    nEdge = pFlowline.nEdge     
+    #    for j in range(nEdge):
+    #        pEdge = pFlowline.aEdge[j]
+    #        aEdge = list()
+    #        aEdge.append(pEdge)
+    #        aEdge_out.append(pEdge)            
+    #        pFlowline1 = pyflowline(aEdge)      
+    #        aFlowline_out.append(pFlowline1)    
+    #        pass
+    #    pass   
+    for pFlowline in aFlowline_in:
+        for pEdge in pFlowline.aEdge:
+            aEdge_out.append(pEdge)
+            aFlowline_out.append(pyflowline([pEdge]))
+            
     return aFlowline_out, aEdge_out
```

### Comparing `pyflowline-0.3.4/pyflowline/classes/_hpc.py` & `pyflowline-0.3.5/pyflowline/classes/_hpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,66 @@
-import os, stat
+import os
+import stat
 from pathlib import Path
+
+
 def _pyflowline_create_hpc_job(self, sSlurm_in=None):
     """create a HPC job for this simulation
     """
     os.chdir(self.sWorkspace_output)
-    
-    #part 1 python script         
-    
-    sFilename_pyflowline = os.path.join(str(Path(self.sWorkspace_output)) , "run_pyflowline.py" )
+
+    # part 1 python script
+
+    sFilename_pyflowline = os.path.join(
+        str(Path(self.sWorkspace_output)), "run_pyflowline.py")
     ofs_pyflowline = open(sFilename_pyflowline, 'w')
-       
-    sLine = '#!/qfs/people/liao313/.conda/envs/pyflowline/bin/' + 'python3' + '\n' 
-    ofs_pyflowline.write(sLine) 
+
+    sLine = '#!/qfs/people/liao313/.conda/envs/pyflowline/bin/' + 'python3' + '\n'
+    ofs_pyflowline.write(sLine)
     sLine = 'from pyflowline.pyflowline_read_model_configuration_file import pyflowline_read_model_configuration_file' + '\n'
-    ofs_pyflowline.write(sLine)         
-    sLine = 'sFilename_configuration_in = ' + '"' + self.sFilename_model_configuration + '"\n'
     ofs_pyflowline.write(sLine)
-    sLine = 'oPyflowline = pyflowline_read_model_configuration_file(sFilename_configuration_in,'  \
-        + 'iCase_index_in='+ str(self.iCase_index) + ',' \
-        + 'dResolution_meter_in=' + "{:0f}".format(self.dResolution_meter)+ ',' \
-        +  'sDate_in="'+ str(self.sDate) + '",' \
-        +  'sMesh_type_in="'+ str(self.sMesh_type) +'"' \
-        + ')'  +   '\n'   
-    ofs_pyflowline.write(sLine)
-         
-    sLine = 'oPyflowline.setup()' + '\n'   
-    ofs_pyflowline.write(sLine)
-    
-    if self.iFlag_flowline ==1:                        
-        sLine = 'oPyflowline.flowline_simplification()' + '\n'   
-        ofs_pyflowline.write(sLine)     
+    sLine = 'sFilename_configuration_in = ' + '"' + \
+        self.sFilename_model_configuration + '"\n'
+    ofs_pyflowline.write(sLine)
+    sLine = 'oPyflowline = pyflowline_read_model_configuration_file(sFilename_configuration_in,'\
+        + 'iCase_index_in=' + str(self.iCase_index) + ','\
+        + 'iResolution_index_in=' + str(self.iResolution_index) + ','\
+        + 'dResolution_meter_in=' + "{:0f}".format(self.dResolution_meter) + ','\
+        + 'sDggrid_type_in="'+ str(self.sDggrid_type) + '",' \
+        + 'sDate_in="' + str(self.sDate) + '",'\
+        + 'sMesh_type_in="' + str(self.sMesh_type) + '"' + ')' + '\n'
+    ofs_pyflowline.write(sLine)
+
+    sLine = 'oPyflowline.pyflowline_setup()' + '\n'
+    ofs_pyflowline.write(sLine)
+
+    if self.iFlag_flowline == 1:
+        sLine = 'oPyflowline.pyflowline_flowline_simplification()' + '\n'
+        ofs_pyflowline.write(sLine)
     else:
-        pass    
-    sLine = 'oPyflowline.mesh_generation()' + '\n'   
-    ofs_pyflowline.write(sLine)      
-    sLine = 'oPyflowline.reconstruct_topological_relationship()' + '\n'   
-    ofs_pyflowline.write(sLine)   
-
-    sLine = 'oPyflowline.analyze()' + '\n'   
-    ofs_pyflowline.write(sLine)      
-    
-    #sLine = 'oPyflowline.evaluate()' + '\n'   
-    #ofs_pyflowline.write(sLine) 
-    
-    sLine = 'oPyflowline.export()' + '\n'   
+        pass
+    sLine = 'oPyflowline.pyflowline_mesh_generation()' + '\n'
+    ofs_pyflowline.write(sLine)
+    sLine = 'oPyflowline.pyflowline_reconstruct_topological_relationship()' + '\n'
+    ofs_pyflowline.write(sLine)
+
+    sLine = 'oPyflowline.pyflowline_analyze()' + '\n'
+    ofs_pyflowline.write(sLine)
+
+    # sLine = 'oPyflowline.pyflowline_evaluate()' + '\n'
+    # ofs_pyflowline.write(sLine)
+
+    sLine = 'oPyflowline.pyflowline_export()' + '\n'
     ofs_pyflowline.write(sLine)
     ofs_pyflowline.close()
-    os.chmod(sFilename_pyflowline, stat.S_IREAD | stat.S_IWRITE | stat.S_IXUSR)          
-    
-    #part 2 bash script    
-    sFilename_job = os.path.join(str(Path(self.sWorkspace_output)  ) ,  "submit.job" )
+    os.chmod(sFilename_pyflowline, stat.S_IREAD | stat.S_IWRITE | stat.S_IXUSR)
+
+    # part 2 bash script
+    sFilename_job = os.path.join(
+        str(Path(self.sWorkspace_output)),  "submit.job")
     ofs = open(sFilename_job, 'w')
     sLine = '#!/bin/bash\n'
     ofs.write(sLine)
     sLine = '#SBATCH -A ESMD\n'
     ofs.write(sLine)
     sLine = '#SBATCH --job-name=' + self.sCase + '\n'
     ofs.write(sLine)
@@ -63,40 +70,40 @@
     ofs.write(sLine)
     sLine = '#SBATCH --ntasks-per-node=1' + '\n'
     ofs.write(sLine)
     if sSlurm_in is not None:
         sSlurm = sSlurm_in
     else:
         sSlurm = 'slurm'
-    sLine = '#SBATCH --partition='+ sSlurm + '\n'
+    sLine = '#SBATCH --partition=' + sSlurm + '\n'
     ofs.write(sLine)
     sLine = '#SBATCH -o stdout.out\n'
     ofs.write(sLine)
     sLine = '#SBATCH -e stderr.err\n'
-    ofs.write(sLine)    
+    ofs.write(sLine)
     sLine = 'module purge\n'
     ofs.write(sLine)
     sLine = 'module load gcc/8.1.0' + '\n'
     ofs.write(sLine)
-    
-    if self.iFlag_dggrid ==1:
+
+    if self.iFlag_dggrid == 1:
         sLine = 'module load gdal/2.3.1' + '\n'
         ofs.write(sLine)
 
-    sLine = 'module load anaconda3/2019.03' + '\n'
+    sLine = 'module load python/miniconda4.12.0 ' + '\n'
+    ofs.write(sLine)
+    sLine = 'source /share/apps/python/miniconda4.12.0/etc/profile.d/conda.sh' + '\n'
     ofs.write(sLine)
-    sLine = 'source /share/apps/anaconda3/2019.03/etc/profile.d/conda.sh' + '\n'
-    ofs.write(sLine)    
     sLine = 'conda activate hexwatershed' + '\n'
     ofs.write(sLine)
     sLine = 'cd $SLURM_SUBMIT_DIR\n'
     ofs.write(sLine)
-    sLine = 'JOB_DIRECTORY='+ self.sWorkspace_output +  '\n'
+    sLine = 'JOB_DIRECTORY=' + self.sWorkspace_output + '\n'
     ofs.write(sLine)
-    sLine = 'cd $JOB_DIRECTORY' +  '\n'
+    sLine = 'cd $JOB_DIRECTORY' + '\n'
     ofs.write(sLine)
-    sLine = 'python3 run_pyflowline.py' +  '\n'
+    sLine = 'python3 run_pyflowline.py' + '\n'
     ofs.write(sLine)
     sLine = 'conda deactivate' + '\n'
     ofs.write(sLine)
     ofs.close()
-    return
+    return
```

### Comparing `pyflowline-0.3.4/pyflowline/classes/_visual.py` & `pyflowline-0.3.5/pyflowline/classes/_visual.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
-from pathlib import Path
+
 #dependency packages
-from pyflowline.external.pyearth.visual.map.map_vector_polygon_data import map_vector_polygon_data
-from pyflowline.external.pyearth.visual.map.map_vector_polyline_data import map_vector_polyline_data
-from pyflowline.external.pyearth.visual.map.map_multiple_vector_data import map_multiple_vector_data
+from pyearth.visual.map.vector.map_vector_polygon_data import map_vector_polygon_data
+from pyearth.visual.map.vector.map_vector_polyline_data import map_vector_polyline_data
+from pyearth.visual.map.vector.map_multiple_vector_data import map_multiple_vector_data
 
 #plot function
 
 def plot(self,
          iFlag_type_in = None,
          iFlag_title_in = None,
          sFilename_output_in = None,
```

### Comparing `pyflowline-0.3.4/pyflowline/classes/_visual_basin.py` & `pyflowline-0.3.5/pyflowline/classes/_visual_basin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
-from pathlib import Path
+
 #dependency packages
-from pyflowline.external.pyearth.visual.map.map_vector_polygon_data import map_vector_polygon_data
-from pyflowline.external.pyearth.visual.map.map_vector_polyline_data import map_vector_polyline_data
-from pyflowline.external.pyearth.visual.map.map_multiple_vector_data import map_multiple_vector_data
+from pyearth.visual.map.vector.map_vector_polygon_data import map_vector_polygon_data
+from pyearth.visual.map.vector.map_vector_polyline_data import map_vector_polyline_data
+from pyearth.visual.map.vector.map_multiple_vector_data import map_multiple_vector_data
 
 def replace_last_occurrence(sFilename_path_in, sSubstring_in, sSubstring_out):
     last_occurrence_index = sFilename_path_in.rfind(sSubstring_in)
     if last_occurrence_index == -1:
         # Substring not found, return the original string
         return sFilename_path_in
     else:
@@ -18,15 +18,15 @@
 def basin_plot(self,
                iFlag_type_in,               
                sMesh_type,
                sFilename_output_in=None,
                sFilename_mesh_in = None,
                iFont_size_in = None,
                iFlag_title_in=None,
-               iFlag_colorbar_in=None,
+               iFlag_colorbar_in=None,               
                iFlag_scientific_notation_colorbar_in=None,
                iFlag_openstreetmap_in = None,
                dData_min_in = None,
                dData_max_in = None,
                sVariable_in=None,
                aExtent_in = None,
                 aLegend_in = None,
@@ -63,15 +63,15 @@
             pass
         else:
             if iFlag_type_in == 3:#polygon based
 
                 self._plot_polygon_variable( sVariable_in,                 
                                             iFlag_title_in= iFlag_title_in,
                                             iFont_size_in=iFont_size_in,
-                                            iFlag_colorbar_in=iFlag_colorbar_in,
+                                            iFlag_colorbar_in=iFlag_colorbar_in,                                            
                                             iFlag_scientific_notation_colorbar_in=iFlag_scientific_notation_colorbar_in,
                                             dData_min_in = dData_min_in,
                                             dData_max_in = dData_max_in,
                                                sFilename_output_in=sFilename_output_in,
                                                aExtent_in = aExtent_in,
                                                 aLegend_in = aLegend_in,
                                                pProjection_map_in = pProjection_map_in)
@@ -81,18 +81,20 @@
                 if iFlag_type_in == 4:#mixed
                     if sVariable_in == "flow_direction_with_mesh":
                         sFilename = self.sFilename_flow_direction #this can be either domain wide or subbasin level
                         aFiletype_in = [3, 2]
                         aFilename_in = [sFilename_mesh, sFilename]
                         map_multiple_vector_data(aFiletype_in,
                                              aFilename_in,
+                                             aFlag_thickness_in=[0, 1],
+                                             aVariable_in=['', 'drainage_area'],
                                              sFilename_output_in=sFilename_output_in,
                                              sTitle_in= 'Mesh with flowline',
                                              aFlag_color_in=[0, 0],
-                                             aFlag_fill_in = [0,0])
+                                             aFlag_fill_in = [0, 0])
                     else:
                         if sVariable_in == "flow_direction_with_observation":
                             sFilename0 = self.sFilename_flow_direction #this can be either domain wide or subbasin level
                             #should use the pyflowline simplified flowline
                             sFilename_dummy = self.sFilename_flowline_simplified
                             #now replace the folder string 
                             sFilename1 = replace_last_occurrence(sFilename_dummy, 'hexwatershed', 'pyflowline')
@@ -110,18 +112,42 @@
                                              sFilename_output_in=sFilename_output_in,
                                              sTitle_in= 'Flow direction with observation',
                                              aFlag_thickness_in=  [1, 0, 0],
                                              aVariable_in= ['drainage_area', '', 'stream_segment'],
                                              aLegend_in = aLegend_in,
                                              aFlag_color_in = [0, 0, 1],
                                              aFlag_fill_in  = [0, 0, 0],
+                                             aFlag_discrete_in = [0, 0, 1],
+                                             aExtent_in = aExtent_in,
+                                             pProjection_map_in = pProjection_map_in)
+                        else:
+                            if sVariable_in == "hillslope_with_flow_direction":
+                                sFilename0 = self.sFilename_hillslope_parquet
+                                sFilename1 = self.sFilename_flow_direction
+                                aFiletype_in = [3, 2]
+                                aFilename_in = [sFilename0, sFilename1]
+                                map_multiple_vector_data(aFiletype_in,
+                                             aFilename_in,  
+                                             iFlag_title_in=iFlag_title_in,                         
+                                             iFont_size_in=iFont_size_in,          
+                                             iFlag_openstreetmap_in=iFlag_openstreetmap_in,                                                    
+                                             sFilename_output_in=sFilename_output_in,
+                                             sTitle_in= 'Flow direction with hillslope',
+                                             aData_min_in=[1, 1],
+                                             aFlag_thickness_in=  [0, 1],
+                                             aFlag_discrete_in = [1,0], 
+                                             aVariable_in= ['hillslope', 'drainage_area'],
+                                             aLegend_in = aLegend_in,
+                                             aFlag_color_in = [1, 0],
+                                             aFlag_fill_in  = [1, 0],
                                                 aExtent_in = aExtent_in,
                                                pProjection_map_in = pProjection_map_in)
-                        else:
-                            print('Unsupported variable: ', sVariable_in, ' in basin_plot.')
+                            
+                            else:
+                                print('Unsupported variable: ', sVariable_in, ' in basin_plot.')
                             return                    
                     
                     pass
                 else:
                     #unsupported
                     pass   
 
@@ -214,15 +240,15 @@
         else:
             pass
     else:        
         sTitle=''
         pass
                
     
-    map_vector_polyline_data(sFilename_json,
+    map_vector_polyline_data(1, sFilename_json,
                              sFilename_output_in= sFilename_output_in,                             
                              iFlag_thickness_in= iFlag_thickness  ,
                              sTitle_in=sTitle,
                              iFlag_color_in= iFlag_color,
                              iFlag_label_in=iFlag_label,
                               iFont_size_in=iFont_size_in,
                              sField_thickness_in = sField_thickness,
@@ -231,14 +257,15 @@
                              pProjection_map_in = pProjection_map_in)
     
 def _plot_polygon_variable(self,
                              sVariable_in,
                              iFigwidth_in=None,
                              iFigheight_in=None,
                              iFlag_colorbar_in=None,
+                             iFlag_discrete_in= None,
                             iFlag_title_in=None,
                             iFont_size_in=None,
                             iFlag_scientific_notation_colorbar_in = None,
                              dData_min_in = None,
                              dData_max_in = None,
                              sFilename_output_in=None,
                               aExtent_in = None,
@@ -254,115 +281,168 @@
         aExtent_in (_type_, optional): _description_. Defaults to None.
         pProjection_map_in (_type_, optional): _description_. Defaults to None.
         dData_min_in (_type_, optional): _description_. Defaults to None.
         dData_max_in (_type_, optional): _description_. Defaults to None.
     """
     
     sMesh_type = self.sMesh_type
+    iFiletype = 1 #most file are geojson, but some are parquet
+    iFlag_integer_in = 0 #most variable are real, if not, it will be set to 1
    
     if sMesh_type == 'mpas':
-        if sVariable_in == 'elevation':
-            sVariable='elevation' #Elevation_profile'
-            sTitle = 'Surface elevation'
-            sUnit = 'Unit: m'
-            sColormap ='terrain'
-            dData_min = dData_min_in
+        #start with integer
+        if sVariable_in == 'subbasin':
+            iFlag_integer_in = 1
+            iFiletype = 3
+            sVariable='subbasin'
+            sTitle = 'Subbasin'
+            sUnit = 'ID'
+            sColormap='Spectral_r'
+            dData_min = 1
             dData_max = dData_max_in
-            sFilename = self.sFilename_elevation
-            sFilename = self.sFilename_variable_polygon
+            sFilename = self.sFilename_subbasin_parquet
         else:
-            if sVariable_in == 'drainage_area':
-                sVariable='drainage_area'
-                sTitle = 'Drainage area'
-                sUnit = r'Units: $m^{2}$'
-                dData_min = dData_min_in
+            if sVariable_in == 'hillslope':
+                sVariable='hillslope'
+                iFlag_integer_in = 1
+                iFiletype = 3
+                sTitle = 'Hillslope'
+                sUnit = 'ID'
+                sColormap='Spectral_r'
+                dData_min = 1
                 dData_max = dData_max_in
-                sColormap ='Spectral_r'
-                sFilename = self.sFilename_variable_polygon
+                sFilename = self.sFilename_hillslope_parquet
             else:
-                if sVariable_in == 'travel_distance':
-                    sVariable='travel_distance'
-                    sTitle = 'Distance to outlet'
-                    sUnit = r'Unit: m'
-                    dData_min = 0.0
-                    dData_max = dData_max_in
-                    sColormap ='Spectral_r'
+                #then with real
+                if sVariable_in == 'elevation':
+                    sVariable='elevation' #Elevation_profile'
+                    sTitle = 'Surface elevation'
+                    sUnit = 'Unit: m'
+                    sColormap ='terrain'
+                    dData_min = dData_min_in
+                    dData_max = dData_max_in            
                     sFilename = self.sFilename_variable_polygon
                 else:
-                    sVariable='slope'
-                    sTitle = 'Surface slope'
-                    sUnit = 'Unit: percent'
-                    sColormap='Spectral_r'
-                    dData_min = 0.0
-                    dData_max = dData_max_in
-                    sFilename = self.sFilename_variable_polygon
+                    if sVariable_in == 'drainage_area':
+                        sVariable='drainage_area'
+                        sTitle = 'Drainage area'
+                        sUnit = r'Units: $m^{2}$'
+                        dData_min = dData_min_in
+                        dData_max = dData_max_in
+                        sColormap ='Spectral_r'
+                        sFilename = self.sFilename_variable_polygon
+                    else:
+                        if sVariable_in == 'travel_distance':
+                            sVariable='travel_distance'
+                            sTitle = 'Distance to outlet'
+                            sUnit = r'Unit: m'
+                            dData_min = 0.0
+                            dData_max = dData_max_in
+                            sColormap ='Spectral_r'
+                            sFilename = self.sFilename_variable_polygon
+                        else:
+                            if sVariable=='slope':
+                                sTitle = 'Surface slope'
+                                sUnit = 'Unit: percent'
+                                sColormap='Spectral_r'
+                                dData_min = 0.0
+                                dData_max = dData_max_in
+                                sFilename = self.sFilename_variable_polygon
+                            else:
+                                pass
+
         
     else:
-        if sVariable_in == 'area':
-            sVariable='area'
-            sTitle = 'Area'
-            sUnit = r'Units: $m^{2}$'
-            sColormap ='terrain'
-            dData_min = dData_min_in
+        if sVariable_in == 'subbasin':
+            iFlag_integer_in = 1
+            iFiletype = 3
+            sVariable='subbasin'
+            sTitle = 'Subbasin'
+            sUnit = 'ID'
+            sColormap='Spectral_r'
+            dData_min = 1
             dData_max = dData_max_in
-            sFilename = self.sFilename_variable_polygon
-            pass
+            sFilename = self.sFilename_subbasin_parquet
         else:
-            if sVariable_in == 'elevation':
-                sVariable='elevation'
-                sTitle = 'Surface elevation'
-                sUnit = r'Unit: m'
-                sColormap ='terrain'
-                dData_min = dData_min_in
+            if sVariable_in == 'hillslope':
+                sVariable='hillslope'
+                iFlag_integer_in = 1
+                iFiletype = 3
+                sTitle = 'Hillslope'
+                sUnit = 'ID'
+                sColormap='Spectral_r'
+                dData_min = 1
                 dData_max = dData_max_in
-                sFilename = self.sFilename_variable_polygon
+                sFilename = self.sFilename_hillslope_parquet
             else:
-                if sVariable_in == 'drainage_area':
-                    sVariable='drainage_area'
-                    sTitle = 'Drainage area'
+                if sVariable_in == 'area':
+                    sVariable='area'
+                    sTitle = 'Area'
                     sUnit = r'Units: $m^{2}$'
+                    sColormap ='terrain'
                     dData_min = dData_min_in
                     dData_max = dData_max_in
-                    sColormap ='Spectral_r'
                     sFilename = self.sFilename_variable_polygon
-
+                    pass
                 else:
-                    if sVariable_in == 'travel_distance':
-                        sVariable='travel_distance'
-                        sTitle = 'Travel distance'
+                    if sVariable_in == 'elevation':
+                        sVariable='elevation'
+                        sTitle = 'Surface elevation'
                         sUnit = r'Unit: m'
-                        dData_min = 0.0
-                        dData_max = dData_max_in
-                        sColormap ='Spectral_r'
-                        iFlag_subbasin = 1
-                        sFilename = self.sFilename_variable_polygon
-                    else:
-                        sVariable='slope'
-                        sTitle = 'Surface slope'
-                        sUnit = r'Unit: percent'
-                        sColormap='Spectral_r'
+                        sColormap ='terrain'
                         dData_min = dData_min_in
                         dData_max = dData_max_in
                         sFilename = self.sFilename_variable_polygon
-            pass
+                    else:
+                        if sVariable_in == 'drainage_area':
+                            sVariable='drainage_area'
+                            sTitle = 'Drainage area'
+                            sUnit = r'Units: $m^{2}$'
+                            dData_min = dData_min_in
+                            dData_max = dData_max_in
+                            sColormap ='Spectral_r'
+                            sFilename = self.sFilename_variable_polygon
+
+                        else:
+                            if sVariable_in == 'travel_distance':
+                                sVariable='travel_distance'
+                                sTitle = 'Travel distance'
+                                sUnit = r'Unit: m'
+                                dData_min = 0.0
+                                dData_max = dData_max_in
+                                sColormap ='Spectral_r'                                
+                                sFilename = self.sFilename_variable_polygon
+                            else:
+                                if sVariable_in=='slope':
+                                    sVariable  = 'slope'
+                                    sTitle = 'Surface slope'
+                                    sUnit = r'Unit: percent'
+                                    sColormap='Spectral_r'
+                                    dData_min = dData_min_in
+                                    dData_max = dData_max_in
+                                    sFilename = self.sFilename_variable_polygon
+                                else:
+                                    pass
+                    pass
     
     if iFlag_title_in is not None:        
         if iFlag_title_in == 0:
             sTitle=''
         else:
             pass
     else:        
         sTitle=''
         pass
 
-    map_vector_polygon_data(sFilename,
+    map_vector_polygon_data(iFiletype, sFilename,
                             iFlag_color_in = 1,
                              iFlag_colorbar_in = iFlag_colorbar_in,
                              iFont_size_in = iFont_size_in,
                              iFlag_scientific_notation_colorbar_in = iFlag_scientific_notation_colorbar_in,
+                             iFlag_discrete_in = iFlag_integer_in, 
                              dData_max_in = dData_max,
                              dData_min_in = dData_min,
                              sFilename_output_in=sFilename_output_in,
                              sVariable_in= sVariable,
                              sTitle_in= sTitle,
                              sUnit_in= sUnit,
                              sColormap_in = sColormap,
```

### Comparing `pyflowline-0.3.4/pyflowline/classes/basin.py` & `pyflowline-0.3.5/pyflowline/classes/basin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 import os, sys
 from pathlib import Path
 import json
 from json import JSONEncoder
-import importlib
+import importlib.util
 import numpy as np
 
 from pyflowline.classes.timer import pytimer
 from pyflowline.classes.vertex import pyvertex
 from pyflowline.classes.edge import pyedge
 from pyflowline.classes.flowline import pyflowline
 from pyflowline.classes.confluence import pyconfluence
 from pyflowline.formats.read_flowline import read_flowline_geojson
 from pyflowline.formats.read_nhdplus_flowline_shapefile import  read_nhdplus_flowline_geojson_attribute
 from pyflowline.formats.read_nhdplus_flowline_shapefile import extract_nhdplus_flowline_shapefile_by_attribute
 from pyflowline.formats.read_nhdplus_flowline_shapefile import track_nhdplus_flowline
 from pyflowline.formats.convert_flowline_to_geojson import convert_flowline_to_geojson
 from pyflowline.formats.export_flowline import export_flowline_to_geojson
 from pyflowline.formats.export_vertex import export_vertex_to_geojson
-from pyflowline.external.pyearth.toolbox.reader.text_reader_string import text_reader_string
-iFlag_cython = importlib.util.find_spec("cython") 
-if iFlag_cython is not None:
-    from pyflowline.external.tinyr.tinyr.tinyr import RTree
-    iFlag_use_rtree = 1
-else:
-    iFlag_use_rtree =0
-    pass
+from pyearth.toolbox.reader.text_reader_string import text_reader_string
 
 from pyflowline.algorithms.split.find_flowline_vertex import find_flowline_vertex
 from pyflowline.algorithms.split.find_flowline_confluence import find_flowline_confluence
 from pyflowline.algorithms.split.split_flowline import split_flowline
 from pyflowline.algorithms.split.split_flowline_to_edge import split_flowline_to_edge
 from pyflowline.algorithms.split.split_by_length import split_flowline_by_length
 from pyflowline.algorithms.merge.merge_flowline import merge_flowline
@@ -40,26 +33,33 @@
 from pyflowline.algorithms.index.define_stream_segment_index import define_stream_segment_index
 from pyflowline.algorithms.index.define_stream_topology import define_stream_topology
 from pyflowline.algorithms.index.define_stream_order import define_stream_order, update_head_water_stream_order
 from pyflowline.algorithms.intersect.intersect_flowline_with_mesh import intersect_flowline_with_mesh
 from pyflowline.algorithms.intersect.intersect_flowline_with_flowline import intersect_flowline_with_flowline
 from pyflowline.algorithms.auxiliary.calculate_area_of_difference import calculate_area_of_difference_simplified
 
-iFlag_cython = importlib.util.find_spec("cython") 
+#cython for performance improvement
+iFlag_cython = importlib.util.find_spec("cython")
 if iFlag_cython is not None:
+
     from pyflowline.algorithms.cython.kernel import find_vertex_in_list
+    from pyflowline.external.tinyr.tinyr.tinyr import RTree
+    iFlag_use_rtree = 1
 else:
     from pyflowline.algorithms.auxiliary.find_vertex_in_list import find_vertex_in_list
+    iFlag_use_rtree = 0
 
-iFlag_kml = importlib.util.find_spec("simplekml") 
+#kml support for google earth visualization
+iFlag_kml = importlib.util.find_spec("simplekml")
 if iFlag_kml is not None:
-    from pyflowline.external.pyearth.gis.kml.convert_geojson_to_kml import convert_geojson_to_kml
-else:
+    #from pyearth.gis.kml.convert_geojson_to_kml import convert_geojson_to_kml
     pass
-sys.setrecursionlimit(10000)
+
+#change the default recursive call limit
+sys.setrecursionlimit(100000)
 
 class BasinClassEncoder(JSONEncoder):
     """Basin class encoder
 
     Args:
         JSONEncoder (_type_): _description_
     """
@@ -67,76 +67,78 @@
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.float32):
             return float(obj)
         if isinstance(obj, np.ndarray):
             return obj.tolist()
         if isinstance(obj, list):
-            pass  
+            pass
         if isinstance(obj, pyvertex):
-            return json.loads(obj.tojson()) 
+            return json.loads(obj.tojson())
         if isinstance(obj, pyedge):
-            return obj.lEdgeID        
+            return obj.lEdgeID
         if isinstance(obj, pyflowline):
             return obj.lFlowlineID
         if isinstance(obj, pyconfluence):
             return obj.dAngle_upstream
-       
+
         return JSONEncoder.default(self, obj)
 
 class pybasin(object):
     """Basin class
 
     Args:
         (object): None
 
     Returns:
         None: A basin object
     """
-    lBasinID =1 
+    lBasinID =1
     sBasinID=''
     lCellID_outlet=-1
     iFlag_debug = 0
+    iFlag_simplification_done = 0
     iFlag_disconnected =0
     iFlag_remove_small_river = 0
     iFlag_remove_low_order_river = 0
+    iFlag_correct_flowline_direction = 0
     iFlag_dam=0
 
     iFlag_break_by_distance = 0
     dLongitude_outlet_degree = -9999.
     dLatitude_outlet_degree = -9999.
     dAccumulation_threshold= 100000.0
     dThreshold_small_river = 10000
     dLength_flowline_filtered = 0.0
     dLength_flowline_simplified = 0.0
     dLength_flowline_conceptual = 0.0
 
     dArea_of_difference=0.0
     dDistance_displace = 0.0
-    dThreshold_break_by_distance = 5000.0 
+    dThreshold_break_by_distance = 5000.0
     sWorkspace_output_basin=''
-    sFilename_flowline_raw=''    
+    sFilename_flowline_raw=''
     sFilename_flowline_filter=''
     sFilename_flowline_filter_geojson=''
     sFilename_dam=''
     sFilename_flowline_topo=''
     #before intersect
     sFilename_flowline_simplified=''
     sFilename_flowline_segment_index_before_intersect=''
     sFilename_flowline_conceptual=''
     sFilename_flowline_edge=''
     sFilename_basin_info=''
     sFilename_flowline_simplified_info=''
     sFilename_flowline_conceptual_info=''
     sFilename_confluence_simplified_info=''
-    sFilename_confluence_conceptual_info=''    
+    sFilename_confluence_conceptual_info=''
 
     aFlowline_basin_filtered=None
     aFlowline_basin_simplified=None
-    aFlowline_basin_conceptual=None    
+    aFlowline_basin_conceptual=None
     aFlowline_basin_edge = None
     pVertex_outlet=None
     aConfluence_basin_simplified= None
     aConfluence_basin_conceptual= None
 
 
     #
@@ -144,118 +146,136 @@
     iMesh_type = 0
     sMesh_type = ''
     #json
     sFilename_watershed_json=''
     sFilename_stream_edge_json =''
 
     #geojson for hexwatershed compatibility
+    #parquet for integer
+    sFilename_subbasin_parquet=''
+    sFilename_hillslope_parquet=''
+
+    #real data type
     sFilename_elevation=''
     sFilename_slope=''
     sFilename_drainage_area=''
-    sFilename_flow_direction ='' 
+    sFilename_flow_direction =''
     sFilename_distance_to_outlet = ''
     sFilename_stream_segment=''
     sFilename_stream_edge=''
 
+    
+
     sFilename_variable_polygon=''
     sFilename_variable_polyline=''
 
+    #txt for characteristics
+    sFilename_watershed_characteristics_txt = ''
+    sFilename_segment_characteristics_txt = ''
+    sFilename_subbasin_characteristics_txt = ''
+    sFilename_hillslope_characteristics_txt = ''
+
     pRTree_flowline = None
     pRTree_edge = None
 
-    
-    iFlag_visual = importlib.util.find_spec("cartopy") 
+
+    iFlag_visual = importlib.util.find_spec("cartopy")
     if iFlag_visual is not None:
         from ._visual_basin import basin_plot
         from ._visual_basin import _plot_polyline_variable
         from ._visual_basin import _plot_polygon_variable
 
-        from ._visual_basin import _plot_area_of_difference 
+        from ._visual_basin import _plot_area_of_difference
     else:
         pass
 
     def __init__(self, aParameter):
         """
         Initialize the basin class object
 
         Args:
             aParameter (dict): Dictionary for parameters
         """
 
-        if 'lBasinID' in aParameter:            
+        if 'lBasinID' in aParameter:
             self.lBasinID             = int(aParameter['lBasinID'])
         else:
             self.lBasinID   = 1
-        
-        
-        if 'lCellID_outlet' in aParameter:            
+
+
+        if 'lCellID_outlet' in aParameter:
             self.lCellID_outlet             = int(aParameter['lCellID_outlet'])
         else:
             self.lCellID_outlet   = -1
 
-        if 'iFlag_disconnected' in aParameter:            
+        if 'iFlag_disconnected' in aParameter:
             self.iFlag_disconnected             = int(aParameter['iFlag_disconnected'])
         else:
             self.iFlag_disconnected   = 0
 
-        if 'iFlag_remove_small_river' in aParameter:            
+        if 'iFlag_remove_small_river' in aParameter:
             self.iFlag_remove_small_river             = int(aParameter['iFlag_remove_small_river'])
         else:
             self.iFlag_remove_small_river   = 0
 
         if 'iFlag_remove_low_order_river' in aParameter:
             self.iFlag_remove_low_order_river = int(aParameter['iFlag_remove_low_order_river'])
         else:
             self.iFlag_remove_low_order_river = 0
-        
-        if 'iFlag_dam' in aParameter:            
+
+        if 'iFlag_correct_flowline_direction' in aParameter:
+            self.iFlag_correct_flowline_direction             = int(aParameter['iFlag_correct_flowline_direction'])
+        else:
+            self.iFlag_correct_flowline_direction   = 0
+
+        if 'iFlag_dam' in aParameter:
             self.iFlag_dam             = int(aParameter['iFlag_dam'])
         else:
             self.iFlag_dam   = 0
-        
-        if 'iFlag_debug' in aParameter:            
+
+        if 'iFlag_debug' in aParameter:
             self.iFlag_debug             = int(aParameter['iFlag_debug'])
         else:
             self.iFlag_debug   = 0
-        
-        if 'dLongitude_outlet_degree' in aParameter:            
+
+        if 'dLongitude_outlet_degree' in aParameter:
             self.dLongitude_outlet_degree             = float(aParameter['dLongitude_outlet_degree'])
         else:
             self.dLongitude_outlet_degree   = -9999.
-        
-        if 'dLatitude_outlet_degree' in aParameter:            
+
+        if 'dLatitude_outlet_degree' in aParameter:
             self.dLatitude_outlet_degree             = float(aParameter['dLatitude_outlet_degree'])
         else:
             self.dLatitude_outlet_degree   = -9999.
-        
-        if 'dThreshold_small_river' in aParameter:            
+
+        if 'dThreshold_small_river' in aParameter:
             self.dThreshold_small_river             = float(aParameter['dThreshold_small_river'])
         else:
             self.dThreshold_small_river   = 10000.0
 
-        if 'dAccumulation_threshold' in aParameter:            
+        if 'dAccumulation_threshold' in aParameter:
             self.dAccumulation_threshold             = float(aParameter['dAccumulation_threshold'])
         else:
-            self.dAccumulation_threshold = 100000.0   
+            self.dAccumulation_threshold = 100000.0
 
         if 'sFilename_flowline_raw' in aParameter:
             self.sFilename_flowline_raw = aParameter['sFilename_flowline_raw']
         else:
             self.sFilename_flowline_raw   = ''
-       
+
         if 'sFilename_flowline_filter' in aParameter:
             self.sFilename_flowline_filter = aParameter['sFilename_flowline_filter']
         else:
             self.sFilename_flowline_filter = ''
 
         if 'sWorkspace_output_basin' in aParameter:
             self.sWorkspace_output_basin = aParameter['sWorkspace_output_basin']
         else:
             self.sWorkspace_output_basin = '.'
-            
+
         Path(self.sWorkspace_output_basin).mkdir(parents=True, exist_ok=True)
 
         self.sFilename_flowline_filter_geojson = os.path.join(str(self.sWorkspace_output_basin ), "flowline_filter.geojson"  )
 
         if 'sFilename_dam' in aParameter:
             self.sFilename_dam = aParameter['sFilename_dam']
         else:
@@ -310,57 +330,69 @@
         self.sFilename_watershed_json = os.path.join(str(self.sWorkspace_output_basin ), "watershed.json" )
         self.sFilename_stream_edge_json = os.path.join(str(self.sWorkspace_output_basin ), 'stream_edge.json')
         self.sFilename_basin_info = os.path.join(str(self.sWorkspace_output_basin ), 'basin_info.json')
         self.sFilename_flowline_conceptual_info = os.path.join(str(self.sWorkspace_output_basin ), 'flowline_conceptual_info.json')
         self.sFilename_flowline_simplified_info = os.path.join(str(self.sWorkspace_output_basin ), 'flowline_simplified_info.json')
         self.sFilename_confluence_conceptual_info = os.path.join(str(self.sWorkspace_output_basin ),'confluence_conceptual_info.json')
         self.sFilename_confluence_simplified_info = os.path.join(str(self.sWorkspace_output_basin ),'confluence_simplified_info.json')
-        
+
         #geojson, full path of the file
-        #full paths are required for the following files
-        #for hexwatershed compatibility, the geojson files will be generated by the pyhexwatershed front end
+        #full paths are required for the following files        
         self.sFilename_flowline_segment_index_before_intersect = os.path.join(str(self.sWorkspace_output_basin ),'flowline_segment_index_before_intersect.geojson')
         self.sFilename_flowline_simplified = os.path.join(str(self.sWorkspace_output_basin ),'flowline_simplified.geojson')
         self.sFilename_flowline_split = os.path.join(str(self.sWorkspace_output_basin ),'flowline_split.geojson')
         self.sFilename_flowline_intersect  = os.path.join(str(self.sWorkspace_output_basin ),'flowline_intersect_mesh.geojson')
         self.sFilename_flowline_conceptual = os.path.join(str(self.sWorkspace_output_basin ),'flowline_conceptual.geojson')
         self.sFilename_flowline_edge = os.path.join(str(self.sWorkspace_output_basin ),'flowline_edge.geojson')
         self.sFilename_area_of_difference = os.path.join(str(self.sWorkspace_output_basin ),'area_of_difference.geojson')
-         
+
+        #for hexwatershed compatibility, the geojson files will be generated by the pyhexwatershed front end
+        #parquet is often converted from geojson instead of directly generated
+        self.sFilename_subbasin_parquet = os.path.join(str(self.sWorkspace_output_basin ), "subbasin.parquet" )
+        self.sFilename_hillslope_parquet = os.path.join(str(self.sWorkspace_output_basin ), "hillslope.parquet" )
+
+        #geojson, some of these can also to convert to parquet for speed up
         self.sFilename_elevation = os.path.join(str(self.sWorkspace_output_basin ), "elevation.geojson" )
         self.sFilename_slope = os.path.join(str(self.sWorkspace_output_basin ), "slope.geojson" )
         self.sFilename_drainage_area =  os.path.join(str(self.sWorkspace_output_basin ), "drainage_area.geojson" )
         self.sFilename_flow_direction = os.path.join(str(self.sWorkspace_output_basin ), "flow_direction.geojson" )
         self.sFilename_distance_to_outlet = os.path.join(str(self.sWorkspace_output_basin ), "distance_to_outlet.geojson" )
         self.sFilename_stream_edge = os.path.join(str(self.sWorkspace_output_basin ), "stream_edge.geojson" )
         self.sFilename_stream_segment = os.path.join(str(self.sWorkspace_output_basin ), "stream_segment.geojson" )
         self.sFilename_variable_polygon = os.path.join(str(self.sWorkspace_output_basin ), "variable_polygon.geojson" )
         self.sFilename_variable_polyline = os.path.join(str(self.sWorkspace_output_basin ), "variable_polyline.geojson" )
-        
+
+        #txt
+        self.sFilename_watershed_characteristics_txt = os.path.join(str(self.sWorkspace_output_basin ), "watershed.txt" )
+        self.sFilename_segment_characteristics_txt = os.path.join(str(self.sWorkspace_output_basin ), "segment.txt" )
+        self.sFilename_subbasin_characteristics_txt = os.path.join(str(self.sWorkspace_output_basin ), "subbasin.txt" )
+        self.sFilename_hillslope_characteristics_txt = os.path.join(str(self.sWorkspace_output_basin ), "hillslope.txt" )
+
         #kml
         self.sFilename_flowline_conceptual_kml = os.path.join(str(self.sWorkspace_output_basin ),'flowline_conceptual.kml')
         return
-        
+
     def basin_flowline_simplification(self):
         """
         Run the basin flowline simplification
 
         Returns:
             list [pyflowline]: A list of simplified flowline
         """
         print('Start flowline simplification:',  self.sBasinID)
         sWorkspace_output_basin = self.sWorkspace_output_basin
-        
+
         ptimer = pytimer()
-        
-        if self.iFlag_dam == 1: 
-            sFilename_flowline_filter = self.sFilename_flowline_filter
-            aFlowline_basin_filtered_raw, pSpatial_reference = read_flowline_geojson( sFilename_flowline_filter )   
+
+        if self.iFlag_dam == 1:
+            #sFilename_flowline_filter = self.sFilename_flowline_filter
+            sFilename_flowline_filter = self.sFilename_flowline_filter_geojson
+            aFlowline_basin_filtered_raw, pSpatial_reference = read_flowline_geojson( sFilename_flowline_filter )
             aVertex_filtered = find_flowline_vertex(aFlowline_basin_filtered_raw)
-            
+
             ptimer.start()
             nFlowline_before = len(aFlowline_basin_filtered_raw)
             sFilename_dam = self.sFilename_dam
             #obtain dam lookup table C
             aData_dam = text_reader_string(sFilename_dam, iSkipline_in =1,cDelimiter_in=',' )
             sFilename_flowline_topo = self.sFilename_flowline_topo
             #obtain whole topology B
@@ -369,36 +401,36 @@
             aToFlowline = aData_flowline_topo[:,2].astype(int).ravel()
             sFilename_flowline_raw = self.sFilename_flowline_raw
             #find A lookup table
             aNHDPlusID_filter = read_nhdplus_flowline_geojson_attribute(sFilename_flowline_filter)
             ndam = len(aData_dam)
             aNHDPlusID_dams_headwater = list()
             aFlowline_dams_nonheadwater = list()
-            aVertex_dams_nonheadwater=list()
+            aVertex_dams_nonheadwater = list()
             n=0
             for j in range(0, ndam):
                 dLon = float(aData_dam[j][1])
                 dLat = float(aData_dam[j][0])
-                sDam = aData_dam[j][4]            
+                sDam = aData_dam[j][4]
                 #individual ID
                 lNHDPlusID = int(aData_dam[j][5])
                 #if lNHDPlusID in aNHDPlusID_filter:
                 if lNHDPlusID in aNHDPlusID_filter: #this is already included in A
                     #change flag by id
                     for k in range(len(aFlowline_basin_filtered_raw)):
                         #remove this flowline by ID
                         if aFlowline_basin_filtered_raw[k].lNHDPlusID == lNHDPlusID:
                             aFlowline_basin_filtered_raw[k].iFlag_dam =1
                             break
                     pass
-                else:                      
+                else:
                     aNHDPlusID_dams_headwater.append(lNHDPlusID)
-                    #not in A, so we need to trace it down    
-                          
-                    aNHDPlusID_dam_nonheadwater = track_nhdplus_flowline(aNHDPlusID_filter, aFromFlowline, aToFlowline, lNHDPlusID)                   
+                    #not in A, so we need to trace it down
+
+                    aNHDPlusID_dam_nonheadwater = track_nhdplus_flowline(aNHDPlusID_filter, aFromFlowline, aToFlowline, lNHDPlusID)
                     aFlowline_dam_nonheadwater = extract_nhdplus_flowline_shapefile_by_attribute(sFilename_flowline_raw, aNHDPlusID_dam_nonheadwater )
                     #clean up
                     aVertex_dam_nonheadwater = find_flowline_vertex(aFlowline_dam_nonheadwater)
                     dThreshold = 1.0
                     iFlag_found=0
                     n=n+len(aFlowline_dam_nonheadwater)
                     #print(j,n)
@@ -406,573 +438,617 @@
                         if iFlag_found ==1:
                             break
 
                         for i in range( len(aVertex_dam_nonheadwater) ):
                             pVertex_dam = aVertex_dam_nonheadwater[i]
                             dDistance = pVertex.calculate_distance(pVertex_dam)
                             if  dDistance<= dThreshold:
-                                aVertex_dam_nonheadwater[i] = pVertex 
+                                aVertex_dam_nonheadwater[i] = pVertex
                                 for k in range(len(aFlowline_dam_nonheadwater)):
-                                    if aFlowline_dam_nonheadwater[k].pVertex_end == pVertex_dam:  
-                                        #update 
+                                    if aFlowline_dam_nonheadwater[k].pVertex_end == pVertex_dam:
+                                        #update
                                         aEdge = aFlowline_dam_nonheadwater[k].aEdge
                                         aEdge[-1] = pyedge( aEdge[-1].pVertex_start, pVertex)
-                                        aFlowline_dam_nonheadwater[k] = pyflowline(aEdge)    
+                                        aFlowline_dam_nonheadwater[k] = pyflowline(aEdge)
 
-                                iFlag_found = 1    
+                                iFlag_found = 1
                                 break
                             else:
-                                #print(dDistance)          
-                                pass                    
+                                #print(dDistance)
+                                pass
 
                     aVertex_dams_nonheadwater.append(aVertex_dam_nonheadwater)
-                    
+
                     aFlowline_dams_nonheadwater.append(aFlowline_dam_nonheadwater)
 
 
             aFlowline_dams_headwater = extract_nhdplus_flowline_shapefile_by_attribute(sFilename_flowline_raw, aNHDPlusID_dams_headwater )
             for i in range(len(aFlowline_dams_headwater)):
                 aFlowline_dams_headwater[i].iFlag_dam = 1
-            
+
             aFlowline_dams_nonheadwater_all = [item for sublist in aFlowline_dams_nonheadwater for item in sublist]
             aVertex_dam_nonheadwater_all = [item for sublist in aVertex_dams_nonheadwater for item in sublist]
-            
-            aFlowline_basin_filtered = aFlowline_basin_filtered_raw + aFlowline_dams_headwater + aFlowline_dams_nonheadwater_all                       
+
+            aFlowline_basin_filtered = aFlowline_basin_filtered_raw + aFlowline_dams_headwater + aFlowline_dams_nonheadwater_all
             aVertex_dam = find_flowline_vertex(aFlowline_dams_headwater)
-            
+
             if self.iFlag_debug ==1:
                 sFilename_out = 'flowline_vertex_filtered.geojson'
                 sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
                 export_vertex_to_geojson( aVertex_filtered, sFilename_out)
                 sFilename_out = 'flowline_vertex_dam.geojson'
                 sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
                 export_vertex_to_geojson( aVertex_dam, sFilename_out)
                 sFilename_out = 'flowline_vertex_dam_nonheadwater.geojson'
                 sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
-                export_vertex_to_geojson( aVertex_dam_nonheadwater_all, sFilename_out)         
+                export_vertex_to_geojson( aVertex_dam_nonheadwater_all, sFilename_out)
 
             nFlowline_after = len(aFlowline_basin_filtered)
             print('Basin ',  self.sBasinID, ' has dam', nFlowline_before, nFlowline_after)
             ptimer.stop()
         else:
-            print('Basin ',  self.sBasinID, ' has no dam')
-            sFilename_flowline_filter = self.sFilename_flowline_filter
-            aFlowline_basin_filtered, pSpatial_reference = read_flowline_geojson( sFilename_flowline_filter ) 
-            #aVertex_filtered = find_flowline_vertex(aFlowline_basin_filtered)  
-    
+            print('Basin ',  self.sBasinID, ' has no dam')            
+            sFilename_flowline_filter = self.sFilename_flowline_filter_geojson #sFilename_flowline_filter = self.sFilename_flowline_filter
+            aFlowline_basin_filtered, pSpatial_reference = read_flowline_geojson( sFilename_flowline_filter )
+            #aVertex_filtered = find_flowline_vertex(aFlowline_basin_filtered)
+
             pass
         sys.stdout.flush()
         if self.iFlag_disconnected == 1:
-            #not used anymore                
+            #not used anymore
             #aThreshold = np.full(2, 300.0, dtype=float)
             #aFlowline_basin_filtered = connect_disconnect_flowline(aFlowline_basin_filtered, aVertex, aThreshold)
             #sFilename_out = 'flowline_connect.geojson'
-            #sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)    
+            #sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
             #export_flowline_to_geojson(iFlag_projected, aFlowline_basin_filtered,pSpatial_reference_gcs, sFilename_out)
             pass
-        
-            
+
+
         if self.iFlag_debug ==1:
             sFilename_out = 'flowline_before_intersect.geojson'
-            sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)            
+            sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
             self.basin_export_flowline(aFlowline_basin_filtered, sFilename_out)
         #calculate length
         self.aFlowline_basin_filtered = aFlowline_basin_filtered
         self.dLength_flowline_filtered = self.basin_calculate_flowline_length(aFlowline_basin_filtered)
 
         #assign vertex id
-        
+
 
         #simplification started
         print('Basin ',  self.sBasinID, 'find flowline vertex')
+        sys.stdout.flush()
         ptimer.start()
         aVertex = find_flowline_vertex(aFlowline_basin_filtered)
         ptimer.stop()
         if self.iFlag_debug ==1:
             sFilename_out = 'flowline_vertex_without_confluence_before_intersect.geojson'
             sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
             export_vertex_to_geojson( aVertex, sFilename_out)
-        
+
         try:
             print('Basin ', self.sBasinID, 'split flowline')
-            ptimer.start()
             sys.stdout.flush()
+            ptimer.start()
+       
             nFlowline_before = len(aFlowline_basin_filtered)
             aFlowline_basin_simplified = split_flowline(aFlowline_basin_filtered, aVertex)
             nFlowline_after = len(aFlowline_basin_simplified)
             ptimer.stop()
         except:
             print(nFlowline_before)
-        
-        
+
+
         if self.iFlag_debug ==1:
             sFilename_out = 'flowline_split_by_point_before_intersect.geojson'
             sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
             export_flowline_to_geojson(aFlowline_basin_simplified, sFilename_out)
-        
+
         #use location to find outlet
-        point= dict()   
+        point= dict()
         point['dLongitude_degree'] = self.dLongitude_outlet_degree
         point['dLatitude_degree'] = self.dLatitude_outlet_degree
         pVertex_outlet=pyvertex(point)
 
-        
         try:
             print('Basin ',  self.sBasinID, 'started correction flow direction')
+            sys.stdout.flush()
             ptimer.start()
-            nFlowline_before = len(aFlowline_basin_simplified)  
-            #this flowline is ordered from downstream to upstream      
+            nFlowline_before = len(aFlowline_basin_simplified)
+            #this flowline is ordered from downstream to upstream
             aFlowline_basin_simplified = correct_flowline_direction(aFlowline_basin_simplified,  pVertex_outlet )
             nFlowline_after = len(aFlowline_basin_simplified)
             ptimer.stop()
-            sys.stdout.flush()
+            #update outlet
             pVertex_outlet = aFlowline_basin_simplified[0].pVertex_end
+            print(pVertex_outlet.dLongitude_degree, pVertex_outlet.dLatitude_degree)
             self.pVertex_outlet = pVertex_outlet
             if self.iFlag_debug ==1:
                 sFilename_out = 'flowline_direction_before_intersect.geojson'
                 sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
                 export_flowline_to_geojson( aFlowline_basin_simplified,  sFilename_out)
         except:
             print('Error in flow direction correction')
-            
-        
-        
+
         #step 4: remove loops
         try:
             print('Basin ',  self.sBasinID, 'started loop removal')
-            ptimer.start()
-            aFlowline_basin_simplified = remove_flowline_loop(aFlowline_basin_simplified)   
-            ptimer.stop() 
             sys.stdout.flush()
+            ptimer.start()
+            aFlowline_basin_simplified = remove_flowline_loop(aFlowline_basin_simplified)
+            ptimer.stop()
+
             if self.iFlag_debug ==1:
                 sFilename_out = 'flowline_loop_before_intersect.geojson'
                 sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
                 export_flowline_to_geojson( aFlowline_basin_simplified, sFilename_out)
         except:
             print('Error in loop removal')
-        
-        
+
+
         #at this stage, the stream order information is not available, but could be easily rebuild for speed up the small river removal algorithm
         print('Basin ',  self.sBasinID, 'started update stream order initial')
+        sys.stdout.flush()
         ptimer.start()
         aFlowline_basin_simplified = update_head_water_stream_order(aFlowline_basin_simplified )
         ptimer.stop()
 
         #using loop to remove small river, here we use 3 steps
         if self.iFlag_remove_small_river ==1:
             for i in np.arange(0, 3, 1):
                 sStep = "{:02d}".format(i+1)
-                
-                dThreshold = self.dThreshold_small_river           
+
+                dThreshold = self.dThreshold_small_river
                 print('Basin ',  self.sBasinID, 'started small river removal', sStep, dThreshold)
-                ptimer.start()
                 sys.stdout.flush()
+                ptimer.start()
+
                 aFlowline_basin_simplified = remove_small_river(aFlowline_basin_simplified, dThreshold )
                 if self.iFlag_debug ==1:
                     sFilename_out = 'flowline_large_'+ sStep +'_before_intersect.geojson'
                     sFilename_out =os.path.join(sWorkspace_output_basin, sFilename_out)
                     export_flowline_to_geojson( aFlowline_basin_simplified,  sFilename_out)
                     #print(len(aFlowline_basin_simplified))
 
-                #update stream order    
+                #update stream order
                 aFlowline_basin_simplified = update_head_water_stream_order(aFlowline_basin_simplified )
 
                 aVertex, lIndex_outlet, aIndex_headwater,aIndex_middle, aIndex_confluence, aConnectivity, pVertex_outlet = find_flowline_confluence(aFlowline_basin_simplified,  pVertex_outlet)
                 if self.iFlag_debug ==1:
                     sFilename_out = 'flowline_vertex_with_confluence_'+ sStep +'_before_intersect.geojson'
                     sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
                     export_vertex_to_geojson( aVertex,  sFilename_out, aAttribute_data=aConnectivity)
 
-                aFlowline_basin_simplified = merge_flowline( aFlowline_basin_simplified, aVertex, pVertex_outlet, aIndex_headwater,aIndex_middle, aIndex_confluence  )  
+                aFlowline_basin_simplified = merge_flowline( aFlowline_basin_simplified, aVertex, pVertex_outlet, aIndex_headwater,aIndex_middle, aIndex_confluence  )
                 if self.iFlag_debug ==1:
                     sFilename_out = 'flowline_merge_'+ sStep +'_before_intersect.geojson'
                     sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
                     export_flowline_to_geojson( aFlowline_basin_simplified,  sFilename_out)
 
                 aFlowline_basin_simplified = update_head_water_stream_order(aFlowline_basin_simplified )
-                    
+
                 ptimer.stop()
                 if len(aFlowline_basin_simplified) == 1:
-                    break               
-                
+                    break
+
             sys.stdout.flush()
         else: #if we dont remove small river, we still need to merge the flowline
             aVertex, lIndex_outlet, aIndex_headwater,aIndex_middle, aIndex_confluence, aConnectivity, pVertex_outlet = find_flowline_confluence(aFlowline_basin_simplified,  pVertex_outlet)
             if self.iFlag_debug ==1:
                 sFilename_out = 'flowline_vertex_with_confluence_before_intersect.geojson'
                 sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
                 export_vertex_to_geojson( aVertex,  sFilename_out, aAttribute_data=aConnectivity)
-            aFlowline_basin_simplified = merge_flowline( aFlowline_basin_simplified, aVertex, pVertex_outlet, aIndex_headwater,aIndex_middle, aIndex_confluence  )  
+            aFlowline_basin_simplified = merge_flowline( aFlowline_basin_simplified, aVertex, pVertex_outlet, aIndex_headwater,aIndex_middle, aIndex_confluence  )
             if self.iFlag_debug ==1:
                 sFilename_out = 'flowline_merge_before_intersect.geojson'
                 sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
                 export_flowline_to_geojson( aFlowline_basin_simplified,  sFilename_out)
             aFlowline_basin_simplified = update_head_water_stream_order(aFlowline_basin_simplified )
             pass
-        
+
         #the final vertex info
-        print('Basin ',  self.sBasinID, 'find flowline confluence')
+        print('Basin ', self.sBasinID, 'find flowline confluence')
+        sys.stdout.flush()
         ptimer.start()
         aVertex, lIndex_outlet, aIndex_headwater,aIndex_middle, aIndex_confluence, aConnectivity, pVertex_outlet = find_flowline_confluence(aFlowline_basin_simplified,  pVertex_outlet)
         ptimer.stop()
         sFilename_out = 'vertex_simplified.geojson'
         sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
         export_vertex_to_geojson( aVertex,  sFilename_out, aAttribute_data=aConnectivity)
-        
+
         #starting here, the self object can be updated because no more edit (add/remove) will be made to the flowline
         #but attributes will be updated
-        
+
         #build segment index, they are reversed
         print('Basin ',  self.sBasinID, 'started stream segment definition')
+        sys.stdout.flush()
         ptimer.start()
         aFlowline_basin_simplified, aStream_segment = define_stream_segment_index(aFlowline_basin_simplified)
         ptimer.stop()
         if self.iFlag_debug ==1:
-            sFilename_out = self.sFilename_flowline_segment_index_before_intersect            
-            export_flowline_to_geojson(aFlowline_basin_simplified, 
-                                       sFilename_out, 
-                aAttribute_data=[aStream_segment], 
-                aAttribute_field=['stream_segment'], 
+            sFilename_out = self.sFilename_flowline_segment_index_before_intersect
+            export_flowline_to_geojson(aFlowline_basin_simplified,
+                                       sFilename_out,
+                aAttribute_data=[aStream_segment],
+                aAttribute_field=['stream_segment'],
                 aAttribute_dtype=['int'])
 
         aVertex = np.array(aVertex)
         aIndex_confluence = np.array(aIndex_confluence)
-        if aIndex_confluence.size > 0:        
+        if aIndex_confluence.size > 0:
             print('Basin ',  self.sBasinID, 'started confluence definition')
             ptimer.start()
             aVertex_confluence = aVertex[aIndex_confluence]
-            aConfluence_basin_simplified = self.basin_build_confluence(aFlowline_basin_simplified, aVertex_confluence) 
+            aConfluence_basin_simplified = self.basin_build_confluence(aFlowline_basin_simplified, aVertex_confluence)
             ptimer.stop()
 
         #change added a new function to build stream topology
         print('Basin ',  self.sBasinID, 'started stream topology definition')
         ptimer.start()
         aFlowline_basin_simplified = define_stream_topology(aFlowline_basin_simplified, aConfluence_basin_simplified)
         ptimer.stop()
-            
-        #build stream order 
+
+        #build stream order
         print('Basin ',  self.sBasinID, 'started stream order definition')
         ptimer.start()
         aFlowline_basin_simplified, aStream_order = define_stream_order(aFlowline_basin_simplified, aConfluence_basin_simplified)
         ptimer.stop()
-        sFilename_out = self.sFilename_flowline_simplified        
-        export_flowline_to_geojson(aFlowline_basin_simplified, 
-                                   sFilename_out, 
-                aAttribute_data=[aStream_segment, aStream_order], 
-                aAttribute_field=['stream_segment','stream_order'], 
+        sFilename_out = self.sFilename_flowline_simplified
+        export_flowline_to_geojson(aFlowline_basin_simplified,
+                                   sFilename_out,
+                aAttribute_data=[aStream_segment, aStream_order],
+                aAttribute_field=['stream_segment','stream_order'],
                 aAttribute_dtype=['int','int'])
-        
+
         if self.iFlag_break_by_distance==1:
             print('Basin ',  self.sBasinID, 'started flowline split by length')
             ptimer.start()
             aFlowline_basin_simplified_split = split_flowline_by_length(aFlowline_basin_simplified, self.dThreshold_break_by_distance)
             ptimer.stop()
-          
+
             sFilename_out = self.sFilename_flowline_split
             export_flowline_to_geojson(  aFlowline_basin_simplified_split, sFilename_out  )
 
         self.aConfluence_basin_simplified = aConfluence_basin_simplified
         self.aFlowline_basin_simplified= aFlowline_basin_simplified
         print('Finish flowline simplification:',  self.sBasinID)
         sys.stdout.flush()
+
+        self.iFlag_simplification_done = 1
         return aFlowline_basin_simplified
 
     def basin_reconstruct_topological_relationship(self, iMesh_type, sFilename_mesh):
         """
         Run the basin topologic relationship reconstruction
 
         Args:
             iMesh_type (int): Mesh type
             sFilename_mesh (str): Filename of the geojson mesh
 
         Returns:
             list [pyflowline]: A list of intersected cells
         """
-        print('Basin ',  self.sBasinID, 'Start topology reconstruction')
-        
+        print('Basin ',  self.sBasinID, 'Start topology reconstruction')        
         ptimer = pytimer()
-        
         sWorkspace_output_basin = self.sWorkspace_output_basin
         sFilename_flowline_in = self.sFilename_flowline_simplified
         sFilename_flowline_intersect_out = self.sFilename_flowline_intersect
 
         try:
             print('Basin ',  self.sBasinID, 'Start flowline and mesh intersection')
+            sys.stdout.flush()
             ptimer.start()
             aCell, aCell_intersect_basin, aFlowline_intersect_all = intersect_flowline_with_mesh(iMesh_type, sFilename_mesh, \
                 sFilename_flowline_in, sFilename_flowline_intersect_out)
             ptimer.stop()
-            sys.stdout.flush()
+            
             if self.iFlag_debug ==1:
                 sFilename_out = 'flowline_intersect_flowline_with_mesh.geojson'
-                sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)  
+                sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
                 export_flowline_to_geojson(aFlowline_intersect_all,  sFilename_out)
         except:
             print('Error in flowline and mesh intersection.')
-        
-        
-        point= dict()
-        point['dLongitude_degree'] = self.dLongitude_outlet_degree
-        point['dLatitude_degree'] = self.dLatitude_outlet_degree
-        pVertex_outlet_initial=pyvertex(point)
+
+        #not an ideal setup, but it could be improved
+        if self.iFlag_simplification_done ==1:
+            pVertex_outlet_initial = self.pVertex_outlet
+        else:    
+            point= dict()
+            point['dLongitude_degree'] = self.dLongitude_outlet_degree
+            point['dLatitude_degree'] = self.dLatitude_outlet_degree
+            pVertex_outlet_initial=pyvertex(point)
 
         #from this point, aFlowline_basin is conceptual
         #segment based
         try:
-            print('Basin ',  self.sBasinID, 'Start return flowline removal')
+            print('Basin ', self.sBasinID, 'Start return flowline removal')
+            sys.stdout.flush()
             ptimer.start()
             aFlowline_basin_conceptual, lCellID_outlet, pVertex_outlet = remove_returning_flowline(iMesh_type, aCell_intersect_basin, pVertex_outlet_initial)
-            ptimer.stop()
-            sys.stdout.flush()
+            print('Outlet ID', lCellID_outlet)
+            #this outlet is the one intersect outlet cell, not cell center
+            print('Outlet location', pVertex_outlet.dLongitude_degree, pVertex_outlet.dLatitude_degree)
+            ptimer.stop()           
             if self.iFlag_debug ==1:
                 sFilename_out = 'flowline_simplified_after_intersect.geojson'
-                sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)  
-                export_flowline_to_geojson(aFlowline_basin_conceptual,  sFilename_out)    
+                sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
+                export_flowline_to_geojson(aFlowline_basin_conceptual, sFilename_out)
         except:
             print('Error in remove_returning_flowline.')
-        
+
 
         #edge based
         try:
-            print('Basin ',  self.sBasinID, 'Start split flowline to edge')          
+            print('Basin ',  self.sBasinID, 'Start split flowline to edge')
+            sys.stdout.flush()
             ptimer.start()
             aFlowline_basin_conceptual, aEdge = split_flowline_to_edge(aFlowline_basin_conceptual)
             ptimer.stop()
-            sys.stdout.flush()
             if self.iFlag_debug ==1:
                 sFilename_out = 'flowline_edge_split_flowline_to_edge.geojson'
                 sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
                 export_flowline_to_geojson( aFlowline_basin_conceptual,  sFilename_out)
         except:
             print('Error in split_flowline_to_edge.')
 
         try:
-            print('Basin ',  self.sBasinID, 'Start remove duplicate flowline')          
+            print('Basin ',  self.sBasinID, 'Start remove duplicate flowline')
+            sys.stdout.flush()
             ptimer.start()
             aFlowline_basin_conceptual = remove_duplicate_flowline(aFlowline_basin_conceptual)
-            ptimer.stop()
-            sys.stdout.flush()
+            ptimer.stop()            
             if self.iFlag_debug ==1:
                 sFilename_out = 'flowline_edge_remove_duplicate_flowline.geojson'
                 sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
                 export_flowline_to_geojson( aFlowline_basin_conceptual,  sFilename_out)
         except:
             print('Error in remove_duplicate_flowline.')
 
         try:
-            print('Basin ',  self.sBasinID, 'Start flowline direction correction')          
+            print('Basin ',  self.sBasinID, 'Start flowline direction correction')
+            sys.stdout.flush()
             ptimer.start()
-            aFlowline_basin_conceptual = correct_flowline_direction(aFlowline_basin_conceptual,  pVertex_outlet )
+            aFlowline_basin_conceptual = correct_flowline_direction(aFlowline_basin_conceptual, pVertex_outlet)
             ptimer.stop()
-            sys.stdout.flush()
             if self.iFlag_debug ==1:
                 sFilename_out = 'flowline_edge_correct_flowline_direction.geojson'
                 sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
                 export_flowline_to_geojson( aFlowline_basin_conceptual,  sFilename_out)
         except:
             print('Error in correct_flowline_direction.')
 
         try:
-            print('Basin ',  self.sBasinID, 'Start flowline direction correction')          
+            print('Basin ',  self.sBasinID, 'Start flowline loop removal')
+            sys.stdout.flush()
             ptimer.start()
-            aFlowline_basin_conceptual = remove_flowline_loop(aFlowline_basin_conceptual )  
+            aFlowline_basin_conceptual = remove_flowline_loop(aFlowline_basin_conceptual )
             ptimer.stop()
-            sys.stdout.flush()
             if self.iFlag_debug ==1:
                 sFilename_out = 'flowline_edge_remove_flowline_loop.geojson'
                 sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
                 export_flowline_to_geojson( aFlowline_basin_conceptual,  sFilename_out)
         except:
             print('Error in remove_flowline_loop.')
-            
-        aFlowline_basin_conceptual = update_head_water_stream_order(aFlowline_basin_conceptual )
-  
+
+        try:
+            aFlowline_basin_conceptual = update_head_water_stream_order(aFlowline_basin_conceptual )
+        except:
+            print('Error in update_head_water_stream_order.')
+
         try:
-            print('Basin ',  self.sBasinID, 'Start find flowline confluence')          
+            print('Basin ',  self.sBasinID, 'Start find flowline confluence')
+            sys.stdout.flush()
             ptimer.start()
             aVertex, lIndex_outlet, aIndex_headwater,aIndex_middle, aIndex_confluence, aConnectivity, pVertex_outlet\
                 = find_flowline_confluence(aFlowline_basin_conceptual,  pVertex_outlet)
             ptimer.stop()
-            sys.stdout.flush()
             if self.iFlag_debug ==1:
                 sFilename_out = 'flowline_vertex_with_confluence_after_intersect.geojson'
                 sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
                 export_vertex_to_geojson( aVertex,  sFilename_out, aAttribute_data=aConnectivity)
         except:
             print('Error in find_flowline_confluence.')
-        
+
         #segment based
         try:
-            print('Basin ',  self.sBasinID, 'Start merge flowline')          
+            print('Basin ',  self.sBasinID, 'Start merge flowline')
+            sys.stdout.flush()
             ptimer.start()
-            aFlowline_basin_conceptual = merge_flowline( aFlowline_basin_conceptual,aVertex, pVertex_outlet, aIndex_headwater,aIndex_middle, aIndex_confluence  )     
+            aFlowline_basin_conceptual = merge_flowline( aFlowline_basin_conceptual, aVertex, pVertex_outlet, aIndex_headwater,aIndex_middle, aIndex_confluence  )
             ptimer.stop()
-            sys.stdout.flush()
         except:
             print('Error in merge_flowline.')
 
-        aFlowline_basin_conceptual = update_head_water_stream_order(aFlowline_basin_conceptual )            
+        aFlowline_basin_conceptual = update_head_water_stream_order(aFlowline_basin_conceptual )
 
         try:
-            print('Basin ',  self.sBasinID, 'Start find flowline confluence')          
+            print('Basin ',  self.sBasinID, 'Start find flowline confluence')
+            sys.stdout.flush()
             ptimer.start()
             aVertex, lIndex_outlet, aIndex_headwater,aIndex_middle, aIndex_confluence, aConnectivity, pVertex_outlet\
-                = find_flowline_confluence(aFlowline_basin_conceptual,  pVertex_outlet)   
+                = find_flowline_confluence(aFlowline_basin_conceptual,  pVertex_outlet)
             ptimer.stop()
-            sys.stdout.flush()
         except:
             print('Error in find_flowline_confluence.')
-             
+
         aFlowline_basin_conceptual, aStream_segment = define_stream_segment_index(aFlowline_basin_conceptual)
 
         #save confluence
         aVertex = np.array(aVertex)
         aIndex_confluence = np.array(aIndex_confluence)
-        if aIndex_confluence.size > 0:        
-            aVertex_confluence = aVertex[aIndex_confluence] 
-            aConfluence_basin_conceptual = self.basin_build_confluence(aFlowline_basin_conceptual, aVertex_confluence) 
+        if aIndex_confluence.size > 0:
+            aVertex_confluence = aVertex[aIndex_confluence]
+            aConfluence_basin_conceptual = self.basin_build_confluence(aFlowline_basin_conceptual, aVertex_confluence)
         else:
             #there is no confluence
             pass
 
         #change added a new function to build stream topology
         print('Basin ',  self.sBasinID, 'started stream topology definition')
+        sys.stdout.flush()
         ptimer.start()
         aFlowline_basin_conceptual = define_stream_topology(aFlowline_basin_conceptual, aConfluence_basin_conceptual)
         ptimer.stop()
-        sys.stdout.flush()
 
         aFlowline_basin_conceptual, aStream_order = define_stream_order(aFlowline_basin_conceptual, aConfluence_basin_conceptual)
 
         #edge based
         aFlowline_basin_edge, aEdge = split_flowline_to_edge(aFlowline_basin_conceptual)
-        sFilename_out = self.sFilename_flowline_edge    
+        sFilename_out = self.sFilename_flowline_edge
         export_flowline_to_geojson( aFlowline_basin_edge, sFilename_out)
-      
+
         sFilename_out = self.sFilename_flowline_conceptual
-        export_flowline_to_geojson( aFlowline_basin_conceptual, 
-                                   sFilename_out, 
-            aAttribute_data=[aStream_segment, aStream_order], 
-            aAttribute_field=['stream_segment','stream_order'], 
+        export_flowline_to_geojson( aFlowline_basin_conceptual,
+                                   sFilename_out,
+            aAttribute_data=[aStream_segment, aStream_order],
+            aAttribute_field=['stream_segment','stream_order'],
             aAttribute_dtype=['int','int'])
 
         self.aConfluence_basin_conceptual = aConfluence_basin_conceptual
-        self.aFlowline_basin_conceptual = aFlowline_basin_conceptual     
+        self.aFlowline_basin_conceptual = aFlowline_basin_conceptual
         self.aFlowline_basin_edge = aFlowline_basin_edge
-        
+
+        #check whether they are changed or not
+        self.pVertex_outlet = pVertex_outlet
         self.lCellID_outlet = lCellID_outlet
         self.dLongitude_outlet_degree = pVertex_outlet.dLongitude_degree
         self.dLatitude_outlet_degree = pVertex_outlet.dLatitude_degree
-        
+        print('Outlet ID', lCellID_outlet)
+        print('Outlet location', pVertex_outlet.dLongitude_degree, pVertex_outlet.dLatitude_degree)
+
         print('Finish topology reconstruction:',  self.sBasinID)
         sys.stdout.flush()
         if iFlag_use_rtree ==1:
             interleaved = True
             self.pRTree_flowline = RTree(interleaved=interleaved, max_cap=5, min_cap=2)
-            for lFlowlineIndex in range(len(self.aFlowline_basin_conceptual)):                
-                pBound = self.aFlowline_basin_conceptual[lFlowlineIndex].pBound                                    
+            for lFlowlineIndex in range(len(self.aFlowline_basin_conceptual)):
+                pBound = self.aFlowline_basin_conceptual[lFlowlineIndex].pBound
                 self.pRTree_flowline.insert(lFlowlineIndex, pBound)
 
             self.pRTree_edge = RTree(interleaved=interleaved, max_cap=5, min_cap=2)
-            for lEdgeIndex in range(len(self.aFlowline_basin_edge)):                
-                pBound = self.aFlowline_basin_edge[lEdgeIndex].pBound                                    
+            for lEdgeIndex in range(len(self.aFlowline_basin_edge)):
+                pBound = self.aFlowline_basin_edge[lEdgeIndex].pBound
                 self.pRTree_edge.insert(lEdgeIndex, pBound)
             pass
         return aCell_intersect_basin
 
-    def basin_build_confluence(self, aFlowline_basin_in, aVertex_confluence_in):    
+    def basin_build_confluence(self, aFlowline_basin_in, aVertex_confluence_in):
         """
         Build the conflence
 
         Args:
             aFlowline_basin_in (list [pyflowline]): A list of flowlines in this basin
             aVertex_confluence_in (list [pyconfluence]): A list of vertices in this basin
 
         Returns:
             list [pyconfluence]: A list of confluences in this basin
         """
         #this can only be calculated for confluence
-        aConfluence_basin=list()
-        for pVertex in aVertex_confluence_in:   
-            aFlowline_upstream =list()
-            for pFlowline in aFlowline_basin_in:
-                pVertex_start = pFlowline.pVertex_start
-                pVertex_end = pFlowline.pVertex_end
-                if pVertex_end == pVertex:                 
-                    aFlowline_upstream.append(pFlowline)
-                    pass
-                if pVertex_start == pVertex:
-                    pFlowline_downstream=pFlowline
-
+        # Create a dictionary to map each vertex to its upstream and downstream flowlines
+        vertex_to_flowlines = {}
+        for pFlowline in aFlowline_basin_in:
+            pVertex_start = pFlowline.pVertex_start
+            pVertex_end = pFlowline.pVertex_end
+
+            if pVertex_end not in vertex_to_flowlines:
+                vertex_to_flowlines[pVertex_end] = {'upstream': [], 'downstream': None}
+            vertex_to_flowlines[pVertex_end]['upstream'].append(pFlowline)
+
+            if pVertex_start not in vertex_to_flowlines:
+                vertex_to_flowlines[pVertex_start] = {'upstream': [], 'downstream': None}
+            vertex_to_flowlines[pVertex_start]['downstream'] = pFlowline
+
+        # Build the confluence for each vertex
+        aConfluence_basin = []
+        for pVertex in aVertex_confluence_in:
+            aFlowline_upstream = vertex_to_flowlines[pVertex]['upstream']
+            pFlowline_downstream = vertex_to_flowlines[pVertex]['downstream']
             pConfluence = pyconfluence(pVertex, aFlowline_upstream, pFlowline_downstream)
-            aConfluence_basin.append(pConfluence)   
+            aConfluence_basin.append(pConfluence)
+
+        #aConfluence_basin=list()
+        #for pVertex in aVertex_confluence_in:
+        #    aFlowline_upstream =list()
+        #    for pFlowline in aFlowline_basin_in:
+        #        pVertex_start = pFlowline.pVertex_start
+        #        pVertex_end = pFlowline.pVertex_end
+        #        if pVertex_end == pVertex:
+        #            aFlowline_upstream.append(pFlowline)
+        #            pass
+        #        if pVertex_start == pVertex:
+        #            pFlowline_downstream=pFlowline
+        #    pConfluence = pyconfluence(pVertex, aFlowline_upstream, pFlowline_downstream)
+        #    aConfluence_basin.append(pConfluence)
+
         return aConfluence_basin
 
     def basin_analyze(self):
         """
         Analyze the basin results including length, sinuosity, and breaching angle
         """
-           
+
         if self.aFlowline_basin_filtered is None:
             sFilename_flowline_filter = self.sFilename_flowline_filter
             sFilename_flowline_filter_geojson = self.sFilename_flowline_filter_geojson
-            self.aFlowline_basin_filtered, pSpatial_reference = read_flowline_geojson( sFilename_flowline_filter_geojson )   
-            self.dLength_flowline_filtered = self.calculate_flowline_length(self.aFlowline_basin_filtered)
-        
+            self.aFlowline_basin_filtered, pSpatial_reference = read_flowline_geojson( sFilename_flowline_filter_geojson )
+            self.dLength_flowline_filtered = self.basin_calculate_flowline_length(self.aFlowline_basin_filtered)
+
+        #maybe we should use the exisitng result
         point= dict()
         point['dLongitude_degree'] = self.dLongitude_outlet_degree
         point['dLatitude_degree'] = self.dLatitude_outlet_degree
         pVertex_outlet_initial=pyvertex(point)
-        if self.aFlowline_basin_simplified is None:            
+
+        if self.aFlowline_basin_simplified is None:
             sFilename_flowline_in = self.sFilename_flowline_simplified
-            aFlowline_simplified,pSpatial_reference = read_flowline_geojson( sFilename_flowline_in )   
-        
+            aFlowline_simplified,pSpatial_reference = read_flowline_geojson( sFilename_flowline_in )
+
             self.aFlowline_basin_simplified = aFlowline_simplified
             aVertex, lIndex_outlet, aIndex_headwater,aIndex_middle, aIndex_confluence, aConnectivity, pVertex_outlet\
-            = find_flowline_confluence(self.aFlowline_basin_simplified,  pVertex_outlet_initial)  
+            = find_flowline_confluence(self.aFlowline_basin_simplified,  pVertex_outlet_initial)
             aVertex = np.array(aVertex)
             aIndex_confluence = np.array(aIndex_confluence)
-            if aIndex_confluence.size > 0:        
-                aVertex_confluence = aVertex[aIndex_confluence] 
+            if aIndex_confluence.size > 0:
+                aVertex_confluence = aVertex[aIndex_confluence]
                 self.aConfluence_basin_simplified = self.build_confluence(self.aFlowline_basin_simplified, aVertex_confluence)
 
-        self.dLength_flowline_simplified = self.calculate_flowline_length(self.aFlowline_basin_simplified)
+        self.dLength_flowline_simplified = self.basin_calculate_flowline_length(self.aFlowline_basin_simplified)
 
         if self.aFlowline_basin_conceptual is None:
             sFilename_flowline_in = self.sFilename_flowline_conceptual
-            aFlowline_conceptual, pSpatial_reference = read_flowline_geojson( sFilename_flowline_in )   
+            aFlowline_conceptual, pSpatial_reference = read_flowline_geojson( sFilename_flowline_in )
             self.aFlowline_basin_conceptual = aFlowline_conceptual
-            
+
             aVertex, lIndex_outlet, aIndex_headwater,aIndex_middle, aIndex_confluence, aConnectivity, pVertex_outlet\
-            = find_flowline_confluence(self.aFlowline_basin_conceptual,  pVertex_outlet_initial)  
+            = find_flowline_confluence(self.aFlowline_basin_conceptual,  pVertex_outlet_initial)
             aVertex = np.array(aVertex)
             aIndex_confluence = np.array(aIndex_confluence)
-            if aIndex_confluence.size > 0:        
-                aVertex_confluence = aVertex[aIndex_confluence] 
+            if aIndex_confluence.size > 0:
+                aVertex_confluence = aVertex[aIndex_confluence]
                 self.aConfluence_basin_conceptual = self.build_confluence(self.aFlowline_basin_conceptual, aVertex_confluence)
 
-        self.dLength_flowline_conceptual = self.calculate_flowline_length(self.aFlowline_basin_conceptual)
-        self.calculate_river_sinuosity()
-        self.calculate_confluence_branching_angle()
-        return    
-    
+        self.dLength_flowline_conceptual = self.basin_calculate_flowline_length(self.aFlowline_basin_conceptual)
+        self.basin_calculate_river_sinuosity()
+        self.basin_calculate_confluence_branching_angle()
+        return
+
     def basin_export(self):
         """
         Export the basin outputs in json format
         """
         self.basin_export_basin_info_to_json()
         self.basin_export_flowline_info_to_json()
-        self.basin_export_confluence_info_to_json()   
+        self.basin_export_confluence_info_to_json()
 
         if iFlag_kml is not None:
             #only convert final conceptual flowline to kml
             sFilename_conceptual = self.sFilename_flowline_conceptual
             sFilename_conceptual_kml = self.sFilename_flowline_conceptual_kml
-            
-            convert_geojson_to_kml(sFilename_conceptual, sFilename_conceptual_kml)
+
+            #convert_geojson_to_kml(sFilename_conceptual, sFilename_conceptual_kml)
 
 
         return
 
     def basin_export_flowline(self, aFlowline_in, sFilename_json_in,iFlag_projected_in = None,  pSpatial_reference_in = None):
         """
         Export the basin flowline to geojson
@@ -980,17 +1056,17 @@
         Args:
             aFlowline_in (list [pyflowline]): A list of flowlines
             sFilename_json_in (str): The output json filename
             iFlag_projected_in (int, optional): Flag if re-projection is needed. Defaults to None.
             pSpatial_reference_in (object, optional): The spatial reference if re-projection is needed. Defaults to None.
         """
         export_flowline_to_geojson(aFlowline_in, sFilename_json_in,
-            iFlag_projected_in= iFlag_projected_in, 
+            iFlag_projected_in= iFlag_projected_in,
             pSpatial_reference_in = pSpatial_reference_in)
-            
+
         return
 
     def basin_export_basin_info_to_json(self):
         """
         Export the basin basin object to json
         """
         sFilename_json = self.sFilename_basin_info
@@ -1004,87 +1080,87 @@
             pass
 
         with open(sFilename_json, 'w', encoding='utf-8') as f:
             sJson = json.dumps(obj, default=lambda o: o.__dict__,\
             sort_keys=True, \
                 indent = 4, \
                     ensure_ascii=True, \
-                        cls=BasinClassEncoder)      
-            f.write(sJson)    
+                        cls=BasinClassEncoder)
+            f.write(sJson)
             f.close()
         return
 
     def basin_export_flowline_info_to_json(self):
         """
         Export the flowline object to json
         """
         iFlag_export_simplified=0
         if iFlag_export_simplified==1:
-            sFilename_json = self.sFilename_flowline_simplified_info            
+            sFilename_json = self.sFilename_flowline_simplified_info
             with open(sFilename_json, 'w', encoding='utf-8') as f:
-                sJson = json.dumps([json.loads(ob.tojson()) for ob in self.aFlowline_basin_simplified], indent = 4)        
-                f.write(sJson)    
+                sJson = json.dumps([json.loads(ob.tojson()) for ob in self.aFlowline_basin_simplified], indent = 4)
+                f.write(sJson)
                 f.close()
 
         sFilename_json = self.sFilename_flowline_conceptual_info
-     
+
         with open(sFilename_json, 'w', encoding='utf-8') as f:
-            sJson = json.dumps([json.loads(ob.tojson()) for ob in self.aFlowline_basin_conceptual], indent = 4)        
-            f.write(sJson)    
+            sJson = json.dumps([json.loads(ob.tojson()) for ob in self.aFlowline_basin_conceptual], indent = 4)
+            f.write(sJson)
             f.close()
         return
 
     def basin_export_confluence_info_to_json(self):
         """
         Export the confluence object to json
         """
         #iFlag_export_confluence =0
         if self.aConfluence_basin_simplified is not None:
             sFilename_json = self.sFilename_confluence_simplified_info
-  
+
             with open(sFilename_json, 'w', encoding='utf-8') as f:
-                sJson = json.dumps([json.loads(ob.tojson()) for ob in self.aConfluence_basin_simplified], indent = 4)        
-                f.write(sJson)    
+                sJson = json.dumps([json.loads(ob.tojson()) for ob in self.aConfluence_basin_simplified], indent = 4)
+                f.write(sJson)
                 f.close()
 
         if self.aConfluence_basin_conceptual is not None:
             sFilename_json = self.sFilename_confluence_conceptual_info
-   
+
 
             with open(sFilename_json, 'w', encoding='utf-8') as f:
-                sJson = json.dumps([json.loads(ob.tojson()) for ob in self.aConfluence_basin_conceptual], indent = 4)        
-                f.write(sJson)    
+                sJson = json.dumps([json.loads(ob.tojson()) for ob in self.aConfluence_basin_conceptual], indent = 4)
+                f.write(sJson)
                 f.close()
-                
-        return   
+
+        return
 
     def tojson(self):
         """
         Export the basin object to json
 
         Returns:
             json str: A json string
         """
         aSkip = ['aFlowline_basin_filtered', \
                 'aFlowline_basin_simplified','aFlowline_basin_conceptual','aConfluence_basin_simplified',
-                'aConfluence_basin_conceptual','pRTree_flowline', 'pRTree_edge']
+                'aConfluence_basin_conceptual','pRTree_flowline', 'pRTree_edge','aFlowline_basin_edge']
 
         obj = self.__dict__.copy()
         for sKey in aSkip:
             obj.pop(sKey, None)
             pass
- 
-    
-        sJson = json.dumps(obj, 
-            sort_keys=True, 
-                indent = 4, 
-                    ensure_ascii=True, 
+
+
+        sJson = json.dumps(obj,
+            sort_keys=True,
+                indent = 4,
+                    ensure_ascii=True,
                         cls=BasinClassEncoder)
         return sJson
-    
+
     def basin_export_config_to_json(self, sFilename_output_in = None):
         """
         Export the basin object to json using the encoder
 
         Args:
             sFilename_output_in (str, optional): The json filename. Defaults to None.
         """
@@ -1092,75 +1168,76 @@
         if sFilename_output_in is not None:
             sFilename_output = sFilename_output_in
         else:
             sFilename_output = os.path.join(self.sWorkspace_output_basin, 'configuration_basin.json' )
 
         aSkip = ['aFlowline_basin_filtered', \
                 'aFlowline_basin_simplified','aFlowline_basin_conceptual','aConfluence_basin_simplified',
-                'aConfluence_basin_conceptual']
+                'aConfluence_basin_conceptual','aFlowline_basin_edge']
         obj = self.__dict__.copy()
         for sKey in aSkip:
             obj.pop(sKey, None)
         with open(sFilename_output, 'w', encoding='utf-8') as f:
             json.dump(obj, f,sort_keys=True, \
                 ensure_ascii=False, \
                 indent=4, \
                 cls=BasinClassEncoder)
         return
 
     def basin_convert_flowline_to_geojson(self):
         """
         Convert the flowline to geojson
         """
-        sFilename_raw = self.sFilename_flowline_filter            
+        sFilename_raw = self.sFilename_flowline_filter
         sFilename_out = self.sFilename_flowline_filter_geojson
         print('Basin '+ self.sBasinID + ': initial flowline:', sFilename_raw )
         convert_flowline_to_geojson(1, sFilename_raw, sFilename_out)
-        return 
-        
+        return
+
     def basin_calculate_flowline_length(self, aFlowline_in):
         """
         Calculate the length of flowlines
 
         Args:
             aFlowline_in (list [pyflowline]): A list of flowlines
 
         Returns:
             float: The total length of all flowlines
         """
-        dLength = 0.0
-        nflowline = len(aFlowline_in)
-        for i in range(nflowline):
-            pFlowline= aFlowline_in[i]
-            pFlowline.calculate_length()
-            dLength = dLength + pFlowline.dLength        
-        return dLength
+        #dLength = 0.0
+        #nflowline = len(aFlowline_in)
+        #for i in range(nflowline):
+        #    pFlowline= aFlowline_in[i]
+        #    pFlowline.calculate_length()
+        #    dLength = dLength + pFlowline.dLength
+        #return dLength
+        return sum(pFlowline.dLength for pFlowline in aFlowline_in)
 
     def basin_calculate_river_sinuosity(self):
         """
         Calcualte the the river sinuosity
         """
         for pFlowline in self.aFlowline_basin_simplified:
-            pFlowline.calculate_flowline_sinuosity() 
+            pFlowline.calculate_flowline_sinuosity()
 
         for pFlowline in self.aFlowline_basin_conceptual:
-            pFlowline.calculate_flowline_sinuosity()    
+            pFlowline.calculate_flowline_sinuosity()
 
         return
 
     def basin_calculate_confluence_branching_angle(self):
         """
         Calcualte the the river confluence branching angle
         """
         for pConfluence in self.aConfluence_basin_simplified:
             pConfluence.calculate_branching_angle()
         for pConfluence in self.aConfluence_basin_conceptual:
-            pConfluence.calculate_branching_angle()    
+            pConfluence.calculate_branching_angle()
         return
-    
+
     def basin_evaluate(self, iMesh_type, sMesh_type):
         """
         Evaluate the model performance
 
         Args:
             iMesh_type (int): The mesh type
             sMesh_type (str): The mesh type
@@ -1174,107 +1251,106 @@
         Evaluate the model performance using area of difference
 
         Args:
             iMesh_type (int): The mesh type
             sMesh_type (str): The mesh type
         """
 
-        
+
         sFilename_simplified = self.sFilename_flowline_simplified
 
-        
+
         sFilename_flowline_edge = self.sFilename_flowline_edge
 
         #intersect first
         sFilename_output= os.path.join(self.sWorkspace_output_basin, 'flowline_intersect_flowline.json')
         aVertex_intersect = intersect_flowline_with_flowline(sFilename_simplified, sFilename_flowline_edge, sFilename_output)
 
         #get confluence simple
-        point= dict()   
+        point= dict()
         point['dLongitude_degree'] = self.dLongitude_outlet_degree
         point['dLatitude_degree'] = self.dLatitude_outlet_degree
         pVertex_outlet=pyvertex(point)
 
-        aFlowline_simplified,pSpatial_reference = read_flowline_geojson( sFilename_simplified )   
+        aFlowline_simplified,pSpatial_reference = read_flowline_geojson( sFilename_simplified )
         aVertex_simplified, lIndex_outlet_simplified, \
             aIndex_headwater_simplified, aIndex_middle, \
                 aIndex_confluence_simplified, aConnectivity, pVertex_outlet\
                 = find_flowline_confluence(aFlowline_simplified,  pVertex_outlet)
 
-        
-        aFlowline_conceptual,pSpatial_reference = read_flowline_geojson( sFilename_flowline_edge ) 
+
+        aFlowline_conceptual,pSpatial_reference = read_flowline_geojson( sFilename_flowline_edge )
         aVertex_conceptual, lIndex_outlet_conceptual, \
             aIndex_headwater_conceptual, aIndex_middle_conceptual, \
             aIndex_confluence_conceptual,  aConnectivity, pVertex_outlet \
                 = find_flowline_confluence(aFlowline_conceptual,  pVertex_outlet)
 
         #merge intersect with confluence
         a=np.array(aIndex_confluence_simplified)
         b=np.array(aIndex_confluence_conceptual)
         c=np.array(aIndex_middle_conceptual)
         d = list(np.array(aVertex_simplified)[a] )
         e = list(np.array(aVertex_conceptual)[b] )
         f = list(np.array(aVertex_conceptual)[c] )
 
         g = aVertex_intersect  + d + e + f
-        
+
         aVertex_all =list()
         for i in g:
             iFlag_exist, lIndex = find_vertex_in_list( aVertex_all,  i)
             if iFlag_exist ==1:
                 pass
             else:
                 aVertex_all.append(i)
 
-        h = aVertex_intersect  + d         
+        h = aVertex_intersect  + d
         aVertex_all_simplified =list()
         for i in h:
             iFlag_exist, lIndex = find_vertex_in_list( aVertex_all_simplified,  i)
             if iFlag_exist ==1:
                 pass
             else:
                 aVertex_all_simplified.append(i)
 
-        j = aVertex_intersect  + e + f       
+        j = aVertex_intersect  + e + f
         aVertex_all_conceptual =list()
         for i in j:
             iFlag_exist, lIndex = find_vertex_in_list( aVertex_all_conceptual,  i)
             if iFlag_exist ==1:
                 pass
             else:
                 aVertex_all_conceptual.append(i)
-        
-        #export 
+
+        #export
         self.iFlag_debug =1
         if self.iFlag_debug ==1:
             sFilename_output= os.path.join(self.sWorkspace_output_basin, 'vertex_split_all.json')
             export_vertex_to_geojson( aVertex_all, sFilename_output)
-        
-        #split 
+
+        #split
         aFlowline_simplified_split = split_flowline(aFlowline_simplified, aVertex_all_simplified,iFlag_intersect =1)
         self.iFlag_debug =1
         if self.iFlag_debug ==1:
             sFilename_out = 'flowline_split_simplified.json'
             sFilename_out = os.path.join(self.sWorkspace_output_basin, sFilename_out)
-            export_flowline_to_geojson(aFlowline_simplified_split, sFilename_out)     
-        
+            export_flowline_to_geojson(aFlowline_simplified_split, sFilename_out)
+
         aFlowline_conceptual_split = split_flowline(aFlowline_conceptual, aVertex_all_conceptual,\
             iFlag_intersect =1, iFlag_use_id=1)
         self.iFlag_debug =1
         if self.iFlag_debug ==1:
             sFilename_out = 'flowline_split_conceptual.json'
-            sFilename_out = os.path.join(self.sWorkspace_output_basin, sFilename_out)  
+            sFilename_out = os.path.join(self.sWorkspace_output_basin, sFilename_out)
             export_flowline_to_geojson(aFlowline_conceptual_split, sFilename_out)
             #aFlowline_conceptual_split, dummy = read_flowline_geojson(sFilename_out)
 
         aFlowline_all = aFlowline_simplified_split + aFlowline_conceptual_split
 
         sFilename_output = self.sFilename_area_of_difference
         #remove headwater not needed here
 
         aPolygon_out, dArea = calculate_area_of_difference_simplified(aFlowline_all, aVertex_all, sFilename_output)
         print('Area of difference: ', dArea)
         self.dArea_of_difference = dArea
-        self.dDistance_displace = dArea / self.dLength_flowline_simplified       
+        self.dDistance_displace = dArea / self.dLength_flowline_simplified
 
         return
-
```

### Comparing `pyflowline-0.3.4/pyflowline/classes/confluence.py` & `pyflowline-0.3.5/pyflowline/classes/confluence.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import importlib
+import importlib.util
 import json
 from json import JSONEncoder
 import numpy as np
 from pyflowline.classes.vertex import pyvertex
 from pyflowline.classes.flowline import pyflowline
 
 iFlag_cython = importlib.util.find_spec("cython") 
 if iFlag_cython is not None:
     from pyflowline.algorithms.cython.kernel import calculate_angle_betwen_vertex
 else:
-    from pyflowline.external.pyearth.gis.gdal.gdal_functions import  calculate_angle_betwen_vertex
+    from pyearth.gis.geometry.calculate_angle_betwen_vertex import  calculate_angle_betwen_vertex
 
 class ConfluenceClassEncoder(JSONEncoder):
     """Confluence Class Encoder
 
     Args:
         JSONEncoder (_type_): _description_
     """
```

### Comparing `pyflowline-0.3.4/pyflowline/classes/dggrid.py` & `pyflowline-0.3.5/pyflowline/classes/dggrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from json import JSONEncoder
 import numpy as np
 from pyflowline.classes.vertex import pyvertex
 from pyflowline.classes.edge import pyedge
 from pyflowline.classes.cell import pycell
 from pyflowline.classes.flowline import pyflowline
-from pyflowline.external.pyearth.gis.gdal.gdal_functions import calculate_polygon_area
+from pyearth.gis.geometry.calculate_polygon_area import calculate_polygon_area
 
 class DggridClassEncoder(JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.float32):
             return float(obj)
```

### Comparing `pyflowline-0.3.4/pyflowline/classes/edge.py` & `pyflowline-0.3.5/pyflowline/classes/edge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 
 import json
 from json import JSONEncoder
-import importlib
+import importlib.util
 import numpy as np
 from pyflowline.classes.vertex import pyvertex
 from pyflowline.algorithms.split.split_by_length import split_edge_by_length
 
 iFlag_cython = importlib.util.find_spec("cython") 
 if iFlag_cython is not None:
     from pyflowline.algorithms.cython.kernel import calculate_angle_betwen_vertex
     from pyflowline.algorithms.cython.kernel import calculate_distance_to_plane
 else:
-    from pyflowline.external.pyearth.gis.gdal.gdal_functions import  calculate_angle_betwen_vertex
-    from pyflowline.external.pyearth.gis.gdal.gdal_functions import calculate_distance_to_plane
+    from pyearth.gis.geometry.calculate_angle_betwen_vertex import  calculate_angle_betwen_vertex
+    from pyearth.gis.geometry.calculate_distance_to_plane import calculate_distance_to_plane
+
 
 class EdgeClassEncoder(JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.float32):
             return float(obj)
@@ -258,20 +259,20 @@
     
     def __eq__(self, other):
         """
         Check if two edges are equivalent
 
         Args:
             other (pyedge): The other edge
+            how about direction?
 
         Returns:
             int: 1 if equivalent; 0 if not
         """
-        iFlag_overlap = self.is_overlap(other)  
-        return iFlag_overlap
+        return int( self.pVertex_start == other.pVertex_start and self.pVertex_end == other.pVertex_end )
 
     def __ne__(self, other):
         """
         Check if two edges are equivalent
 
         Args:
             other (pyedge): The other edge
```

### Comparing `pyflowline-0.3.4/pyflowline/classes/flowline.py` & `pyflowline-0.3.5/pyflowline/classes/flowline.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         """
         Initilize a flowline object
 
         Args:
             aEdge (list [pyedge]): A list of edge objects
         """
         self.aEdge = aEdge
-        nEdge  = len(aEdge)
+        nEdge = len(aEdge)
         self.nEdge = nEdge
         self.pVertex_start = aEdge[0].pVertex_start
         self.pVertex_end =  aEdge[ nEdge-1  ].pVertex_end
         nVertex = nEdge +1
         self.aVertex=list()
         for i in range(nEdge):
             self.aVertex.append( aEdge[i].pVertex_start )
@@ -93,33 +93,38 @@
         self.aFlowlineID_start_end = list()
         self.aFlowlineID_end_start = list()
         self.aFlowlineID_end_end = list()
 
         self.calculate_flowline_bound()
      
         return
-
+    
+    def __hash__(self):
+        return hash((self.pVertex_start, self.pVertex_end))
+    
     def calculate_length(self):
         """
         Calcualte the length
 
         Returns:
             float: The length of the flowline
         """
-        dLength =0.0
+        #dLength =0.0
         #loop though
-        for i in range(self.nEdge):
+        #for i in range(self.nEdge):
         #for edge in self.aEdge:
-            self.aEdge[i].calculate_length()
-            dLength = dLength + self.aEdge[i].dLength
+        #    self.aEdge[i].calculate_length()
+        #    dLength = dLength + self.aEdge[i].dLength
 
         #assing
-        self.dLength= dLength
+        #self.dLength= dLength
 
-        return dLength
+   
+        self.dLength = sum(edge.dLength for edge in self.aEdge)
+        return self.dLength
     
     def calculate_flowline_bound(self):
         dLat_min = 90
         dLat_max = -90
         dLon_min = 180
         dLon_max = -180
         for i in range(self.nVertex):
@@ -266,15 +271,15 @@
 
         Returns:
             pyflowline: The updated flowline
         """
         aEdge=list()
         pFlowline_out=None
         for edge in self.aEdge:
-            edge.calculate_length()
+            #edge.calculate_length()
             if edge.dLength > dDistance:
                 #break it
                 aEdge0=edge.split_by_length(dDistance)
                 for edge0 in aEdge0:
                     aEdge.append(edge0)
                 pass
             else:
@@ -292,38 +297,25 @@
         dDistance = pVertex_start.calculate_distance(pVertex_end)
         self.dSinuosity = self.dLength / dDistance
         return
 
     def __eq__(self, other):
         """
         Check whether two flowline are equivalent
-
+    
         Args:
             other (pyflowline): The other flowline
-
+    
         Returns:
             int: 1 if equivalent, 0 if not
         """
-        iFlag_overlap = 0 
-        nEdge1 = self.nEdge
-        nEdge2 = other.nEdge
-        if nEdge1 == nEdge2:
-            for i in np.arange( nEdge1):
-                pEdge1 = self.aEdge[i]
-                pEdge2 = other.aEdge[i]
-                if pEdge1 == pEdge2:
-                    iFlag_overlap =1 
-                else:
-                    iFlag_overlap =0 
-                    break                
-            
-        else:
-            iFlag_overlap = 0
-
-        return iFlag_overlap
+        if len(self.aEdge) != len(other.aEdge):
+            return 0
+    
+        return int(all(edge1 == edge2 for edge1, edge2 in zip(self.aEdge, other.aEdge)))
 
     def __ne__(self, other):
         """
         Check whether two flowline are equivalent
 
         Args:
             other (pyflowline): The other flowline
```

### Comparing `pyflowline-0.3.4/pyflowline/classes/hexagon.py` & `pyflowline-0.3.5/pyflowline/classes/hexagon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from json import JSONEncoder
 import numpy as np
 from pyflowline.classes.vertex import pyvertex
 from pyflowline.classes.edge import pyedge
 from pyflowline.classes.cell import pycell
 from pyflowline.classes.flowline import pyflowline
-from pyflowline.external.pyearth.gis.gdal.gdal_functions import calculate_polygon_area
+from pyearth.gis.geometry.calculate_polygon_area import calculate_polygon_area
 
 class HexagonClassEncoder(JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.float32):
             return float(obj)
```

### Comparing `pyflowline-0.3.4/pyflowline/classes/latlon.py` & `pyflowline-0.3.5/pyflowline/classes/latlon.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 from json import JSONEncoder
 import numpy as np
 from pyflowline.classes.vertex import pyvertex
 from pyflowline.classes.edge import pyedge
 from pyflowline.classes.cell import pycell
 from pyflowline.classes.flowline import pyflowline
-from pyflowline.external.pyearth.gis.gdal.gdal_functions import calculate_polygon_area
+from pyearth.gis.geometry.calculate_polygon_area import calculate_polygon_area
 
 class LatlonClassEncoder(JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.float32):
             return float(obj)
```

### Comparing `pyflowline-0.3.4/pyflowline/classes/link.py` & `pyflowline-0.3.5/pyflowline/classes/link.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/pyflowline/classes/mpas.py` & `pyflowline-0.3.5/pyflowline/classes/mpas.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 from json import JSONEncoder
 import numpy as np
 from pyflowline.classes.vertex import pyvertex
 from pyflowline.classes.edge import pyedge
 from pyflowline.classes.cell import pycell
 from pyflowline.classes.flowline import pyflowline
-from pyflowline.external.pyearth.gis.gdal.gdal_functions import calculate_polygon_area
+from pyearth.gis.geometry.calculate_polygon_area import calculate_polygon_area
 
 class MpasClassEncoder(JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.float32):
             return float(obj)
```

### Comparing `pyflowline-0.3.4/pyflowline/classes/pycase.py` & `pyflowline-0.3.5/pyflowline/classes/pycase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import os
 import stat
 from pathlib import Path
 import json
 from json import JSONEncoder
 import datetime
-import importlib
+import importlib.util
 from shutil import copy2
 import numpy as np
 from osgeo import ogr, osr, gdal
 
-from pyflowline.external.pyearth.system.define_global_variables import *
+from pyearth.system.define_global_variables import *
 from pyflowline.classes.timer import pytimer
 from pyflowline.classes.mpas import pympas
 from pyflowline.classes.hexagon import pyhexagon
 from pyflowline.classes.latlon import pylatlon
 from pyflowline.classes.square import pysquare
 from pyflowline.classes.dggrid import pydggrid
 from pyflowline.classes.vertex import pyvertex
 from pyflowline.classes.basin import pybasin
 from pyflowline.classes.flowline import pyflowline
 from pyflowline.classes.edge import pyedge
 from pyflowline.formats.read_mesh import read_mesh_json, read_mesh_json_w_topology
-from pyflowline.external.pyearth.gis.gdal.gdal_functions import reproject_coordinates
-from pyflowline.external.pyearth.gis.gdal.gdal_functions  import degree_to_meter
-from pyflowline.external.pyearth.gis.gdal.gdal_functions  import meter_to_degree
-from pyflowline.external.pyearth.gis.gdal.gdal_functions import retrieve_geotiff_metadata
-from pyflowline.external.pyearth.gis.gdal.gdal_functions import read_mesh_boundary
-from pyflowline.external.pyearth.gis.gdal.gdal_functions import get_utm_spatial_reference
+
+
+from pyearth.gis.spatialref.reproject_coodinates import reproject_coordinates
+from pyearth.gis.spatialref.conversion_between_degree_and_meter  import degree_to_meter
+from pyearth.gis.spatialref.conversion_between_degree_and_meter  import meter_to_degree
+from pyearth.gis.gdal.read.raster.gdal_read_geotiff_file import gdal_read_geotiff_file
+from pyearth.gis.gdal.read.vector.gdal_read_geojson_boundary import gdal_read_geojson_boundary
+from pyearth.gis.spatialref.get_utm_spatial_reference import get_utm_spatial_reference
+from pyearth.toolbox.data.geoparquet.convert_geojson_to_geoparquet import convert_geojson_to_geoparquet
 
 iFlag_kml = importlib.util.find_spec("simplekml") 
-if iFlag_kml is not None:
-    from pyflowline.external.pyearth.gis.kml.convert_geojson_to_kml import convert_geojson_to_kml
-else:
-    pass
+
 
 iFlag_cython = importlib.util.find_spec("cython") 
 if iFlag_cython is not None:
     from pyflowline.external.tinyr.tinyr.tinyr import RTree
     iFlag_use_rtree = 1
 else:
     iFlag_use_rtree =0
@@ -309,15 +309,15 @@
 
         if 'sFilename_mesh_boundary' in aConfig_in:
             self.sFilename_mesh_boundary    = aConfig_in[ 'sFilename_mesh_boundary']
 
             if self.iFlag_mesh_boundary==1:
                 if not os.path.isfile(self.sFilename_mesh_boundary ):
                     print("The mesh boundary file does not exist, you should update this parameter before running the model!")
-                    exit()
+                    #exit()
                 pass
 
         if 'sFilename_spatial_reference' in aConfig_in:
             self.sFilename_spatial_reference = aConfig_in['sFilename_spatial_reference']
 
 
         if 'sFilename_dem' in aConfig_in:
@@ -418,16 +418,16 @@
 
         if self.iMesh_type == 4:
             if not os.path.isfile(self.sFilename_mesh_netcdf ):
                 print("The MPAS mesh file does not exist!")
                 exit()
         else:
             if not os.path.isfile(self.sFilename_dem ): #why DEM is required?
-                print("The DEM file does not exist!")
-                exit()
+                print("The DEM file does not exist in pyflowline!")
+                #exit()
 
         self.aBasin = list()
 
         if self.iFlag_flowline==1:
             if 'sFilename_basins' in aConfig_in:
                 self.sFilename_basins = aConfig_in['sFilename_basins']
                 if os.path.isfile(self.sFilename_basins):
@@ -507,148 +507,170 @@
             iFlag_mesh_boundary = self.iFlag_mesh_boundary
             dResolution_degree = self.dResolution_degree
             dResolution_meter = self.dResolution_meter
             sFilename_dem = self.sFilename_dem
             sFilename_spatial_reference = self.sFilename_spatial_reference
             sFilename_mesh = self.sFilename_mesh 
 
-            if iFlag_mesh_boundary ==1:
-                #create a polygon based on real boundary
-                pBoundary_wkt, aExtent = read_mesh_boundary(self.sFilename_mesh_boundary)           
-
-                if iMesh_type != 4: #not mpas
-                    spatial_reference_target = osr.SpatialReference()
-                    spatial_reference_target.ImportFromEPSG(4326)
-
-                    #check whether DEM exists
-                    if os.path.isfile(sFilename_dem):
-                        dPixelWidth, pPixelHeight, dOriginX, dOriginY, nrow, ncolumn, pSpatialRef_dem, pProjection, pGeotransform\
-                            = retrieve_geotiff_metadata(sFilename_dem)
-
-                        #lower left
-                        dX_lowerleft  = dOriginX
-                        dY_lowerleft = dOriginY - (nrow+1) * dPixelWidth
-                        dLongitude_left0,  dLatitude_bot0= reproject_coordinates(dX_lowerleft, dY_lowerleft,pSpatialRef_dem,    spatial_reference_target)
-
-                        #upper right
-                        dX_upperright = dOriginX + (ncolumn +1) * dPixelWidth
-                        dY_upperright = dOriginY
-                        dLongitude_right0, dLatitude_top0= reproject_coordinates(dX_upperright, dY_upperright,pSpatialRef_dem,  spatial_reference_target)
-
-                        #lower right
-                        dX_lowerright = dOriginX + (ncolumn +1) * dPixelWidth
-                        dY_lowerright = dOriginY - (nrow+1) * dPixelWidth
-
-                        dLongitude_right1,  dLatitude_bot1= reproject_coordinates(dX_lowerright, dY_lowerright,pSpatialRef_dem,    spatial_reference_target)
-
-                        #uppler left
-                        dX_upperleft   = dOriginX
-                        dY_upperleft   =  dOriginY
-                        dLongitude_left1, dLatitude_top1= reproject_coordinates(dX_upperleft, dY_upperleft, pSpatialRef_dem,  spatial_reference_target)
-
-                        dLatitude_top = np.max([dLatitude_top0, dLatitude_top1])
-                        dLatitude_bot = np.min([dLatitude_bot0, dLatitude_bot1])
+            if iFlag_global ==1: #a global mesh does not require boundary
+                pass
+            else:
 
-                        dLongitude_left = np.min([dLongitude_left0, dLongitude_left1])
-                        dLongitude_right = np.max([dLongitude_right0, dLongitude_right1])
+                if iFlag_mesh_boundary ==1:
+                    #create a polygon based on real boundary
+                    pBoundary_wkt, aExtent = gdal_read_geojson_boundary(self.sFilename_mesh_boundary)           
 
-                        dLatitude_mean = 0.5 * (dLatitude_top + dLatitude_bot)
-                        #pass
+                    if iMesh_type != 4: #not mpas
+                        spatial_reference_target = osr.SpatialReference()
+                        spatial_reference_target.ImportFromEPSG(4326)
+
+                        #check whether DEM exists
+                        if os.path.isfile(sFilename_dem):
+                            #dPixelWidth, pPixelHeight, dOriginX, dOriginY, nrow, ncolumn, pSpatialRef_dem, pProjection, pGeotransform\
+                            #    = retrieve_geotiff_metadata(sFilename_dem)
+                            dummy = gdal_read_geotiff_file(sFilename_dem, iFlag_metadata_only= 1)
+                            dPixelWidth = dummy['pixelWidth']                        
+                            pPixelHeight = dummy['pixelHeight']
+                            dOriginX = dummy['originX']
+                            dOriginY = dummy['originY']
+                            nrow = dummy['nrow']
+                            ncolumn = dummy['ncolumn']
+                            pSpatialRef_dem = dummy['spatialReference']
+                            #pProjection= dummy['projection']
+                            #pGeotransform = dummy['geotransform']
+
+                            #lower left
+                            dX_lowerleft  = dOriginX
+                            dY_lowerleft = dOriginY + (nrow+1) * pPixelHeight
+                            dLongitude_left0,  dLatitude_bot0= reproject_coordinates(dX_lowerleft, dY_lowerleft,pSpatialRef_dem,    spatial_reference_target)
+
+                            #upper right
+                            dX_upperright = dOriginX + (ncolumn +1) * dPixelWidth
+                            dY_upperright = dOriginY
+                            dLongitude_right0, dLatitude_top0= reproject_coordinates(dX_upperright, dY_upperright,pSpatialRef_dem,  spatial_reference_target)
+
+                            #lower right
+                            dX_lowerright = dOriginX + (ncolumn +1) * dPixelWidth
+                            dY_lowerright = dOriginY - (nrow+1) * dPixelWidth
+
+                            dLongitude_right1,  dLatitude_bot1= reproject_coordinates(dX_lowerright, dY_lowerright,pSpatialRef_dem,    spatial_reference_target)
+
+                            #uppler left
+                            dX_upperleft   = dOriginX
+                            dY_upperleft   =  dOriginY
+                            dLongitude_left1, dLatitude_top1= reproject_coordinates(dX_upperleft, dY_upperleft, pSpatialRef_dem,  spatial_reference_target)
 
-                        if dResolution_meter is None:
-                            #not used
-                            pass
-                        else:
-                            dResolution_degree = meter_to_degree(dResolution_meter, dLatitude_mean)
+                            dLatitude_top = np.max([dLatitude_top0, dLatitude_top1])
+                            dLatitude_bot = np.min([dLatitude_bot0, dLatitude_bot1])
 
-                        dX_lowerleft = dOriginX
-                        dY_upperleft = dOriginY
-                    else: #use the spatial extent and utm zone to obatin the mesh boundary
-                        dLongitude_left, dLongitude_right,dLatitude_bot,  dLatitude_top = aExtent
-                        dLatitude_mean = 0.5 * (dLatitude_top + dLatitude_bot)
-                        dLongitude_mean = 0.5 * (dLongitude_left + dLongitude_right)
+                            dLongitude_left = np.min([dLongitude_left0, dLongitude_left1])
+                            dLongitude_right = np.max([dLongitude_right0, dLongitude_right1])
 
-                        if iMesh_type == 3: #latlon
+                            dLatitude_mean = 0.5 * (dLatitude_top + dLatitude_bot)
+                            #pass
 
-                            pass
-                        else:
                             if dResolution_meter is None:
                                 #not used
                                 pass
                             else:
                                 dResolution_degree = meter_to_degree(dResolution_meter, dLatitude_mean)
-                            pass
 
-                        pUTM = get_utm_spatial_reference(dLongitude_mean)
-                        
-                        #calculate the lower left and upper right in utm projection
-                        dX_lowerleft, dY_lowerleft = reproject_coordinates(dLongitude_left, dLatitude_bot, spatial_reference_target,  pUTM)
-                        
-                        dX_lowerright, dY_lowerright = reproject_coordinates(dLongitude_right, dLatitude_bot, spatial_reference_target,  pUTM)
+                            dX_lowerleft = dOriginX
+                            dY_upperleft = dOriginY
+                        else: #use the spatial extent and utm zone to obatin the mesh boundary
+                            dLongitude_left, dLongitude_right,dLatitude_bot,  dLatitude_top = aExtent
+                            dLatitude_mean = 0.5 * (dLatitude_top + dLatitude_bot)
+                            dLongitude_mean = 0.5 * (dLongitude_left + dLongitude_right)
 
-                        dX_upperright, dY_upperright = reproject_coordinates(dLongitude_right, dLatitude_top, spatial_reference_target,  pUTM)
+                            if iMesh_type == 3: #latlon
 
-                        dX_upperleft, dY_upperright = reproject_coordinates(dLongitude_left, dLatitude_top, spatial_reference_target,  pUTM)
-                        
-                else:
+                                pass
+                            else:
+                                if dResolution_meter is None:
+                                    #not used
+                                    pass
+                                else:
+                                    dResolution_degree = meter_to_degree(dResolution_meter, dLatitude_mean)
+                                pass
 
-                    pass
-            else:
-                #if the boundary is not specified, a DEM file is required
-                if iMesh_type != 4: #mpas
-                    spatial_reference_target = osr.SpatialReference()
-                    spatial_reference_target.ImportFromEPSG(4326)
-
-                    #check whether DEM exists
-                    if os.path.isfile(sFilename_dem):
-                        dPixelWidth, dOriginX, dOriginY, nrow, ncolumn, pSpatialRef_dem, pProjection, pGeotransform\
-                            = retrieve_geotiff_metadata(sFilename_dem)
-
-                        #lower left
-                        dX_lowerleft  = dOriginX
-                        dY_lowerleft = dOriginY - (nrow+1) * dPixelWidth
-                        dLongitude_left0,  dLatitude_bot0= reproject_coordinates(dX_lowerleft, dY_lowerleft,pSpatialRef_dem,    spatial_reference_target)
-
-                        #upper right
-                        dX_upperright = dOriginX + (ncolumn +1) * dPixelWidth
-                        dY_upperright = dOriginY
-                        dLongitude_right0, dLatitude_top0= reproject_coordinates(dX_upperright, dY_upperright,pSpatialRef_dem,  spatial_reference_target)
-
-                        #lower right
-                        dX_lowerright = dOriginX + (ncolumn +1) * dPixelWidth
-                        dY_lowerright = dOriginY - (nrow+1) * dPixelWidth
-
-                        dLongitude_right1,  dLatitude_bot1= reproject_coordinates(dX_lowerright, dY_lowerright,pSpatialRef_dem,    spatial_reference_target)
-
-                        #uppler left
-                        dX_upperleft   = dOriginX
-                        dY_upperleft   =  dOriginY
-                        dLongitude_left1, dLatitude_top1= reproject_coordinates(dX_upperleft, dY_upperleft, pSpatialRef_dem,  spatial_reference_target)
-
-                        dLatitude_top = np.max([dLatitude_top0, dLatitude_top1])
-                        dLatitude_bot = np.min([dLatitude_bot0, dLatitude_bot1])
+                            pUTM = get_utm_spatial_reference(dLongitude_mean)
 
-                        dLongitude_left = np.min([dLongitude_left0, dLongitude_left1])
-                        dLongitude_right = np.max([dLongitude_right0, dLongitude_right1])
+                            #calculate the lower left and upper right in utm projection
+                            dX_lowerleft, dY_lowerleft = reproject_coordinates(dLongitude_left, dLatitude_bot, spatial_reference_target,  pUTM)
 
-                        dLatitude_mean = 0.5 * (dLatitude_top + dLatitude_bot)
-                        #pass
+                            dX_lowerright, dY_lowerright = reproject_coordinates(dLongitude_right, dLatitude_bot, spatial_reference_target,  pUTM)
 
-                        if dResolution_meter < 0:
-                            #not used
-                            pass
-                        else:
-                            dResolution_degree = meter_to_degree(dResolution_meter, dLatitude_mean)
+                            dX_upperright, dY_upperright = reproject_coordinates(dLongitude_right, dLatitude_top, spatial_reference_target,  pUTM)
+
+                            dX_upperleft, dY_upperright = reproject_coordinates(dLongitude_left, dLatitude_top, spatial_reference_target,  pUTM)
 
-                        dX_lowerleft = dOriginX
-                        dY_upperleft = dOriginY
                     else:
-                        print("Error: DEM file does not exist: " + sFilename_dem)
-                        return
-                pass
+
+                        pass
+                else:
+                    #if the boundary is not specified, a DEM file is required
+                    if iMesh_type != 4: #mpas
+                        spatial_reference_target = osr.SpatialReference()
+                        spatial_reference_target.ImportFromEPSG(4326)
+
+                        #check whether DEM exists
+                        if os.path.isfile(sFilename_dem):
+                            dummy = gdal_read_geotiff_file(sFilename_dem, iFlag_metadata_only= 1)
+                            dPixelWidth = dummy['pixelWidth']                        
+                            pPixelHeight = dummy['pixelHeight']
+                            dOriginX = dummy['originX']
+                            dOriginY = dummy['originY']
+                            nrow = dummy['nrow']
+                            ncolumn = dummy['ncolumn']
+                            pSpatialRef_dem = dummy['spatialReference']
+                            pProjection= dummy['projection']
+                            pGeotransform = dummy['geotransform']
+
+                            #lower left
+                            dX_lowerleft  = dOriginX
+                            dY_lowerleft = dOriginY - (nrow+1) * dPixelWidth
+                            dLongitude_left0,  dLatitude_bot0= reproject_coordinates(dX_lowerleft, dY_lowerleft,pSpatialRef_dem,    spatial_reference_target)
+
+                            #upper right
+                            dX_upperright = dOriginX + (ncolumn +1) * dPixelWidth
+                            dY_upperright = dOriginY
+                            dLongitude_right0, dLatitude_top0= reproject_coordinates(dX_upperright, dY_upperright,pSpatialRef_dem,  spatial_reference_target)
+
+                            #lower right
+                            dX_lowerright = dOriginX + (ncolumn +1) * dPixelWidth
+                            dY_lowerright = dOriginY - (nrow+1) * dPixelWidth
+
+                            dLongitude_right1,  dLatitude_bot1= reproject_coordinates(dX_lowerright, dY_lowerright,pSpatialRef_dem,    spatial_reference_target)
+
+                            #uppler left
+                            dX_upperleft   = dOriginX
+                            dY_upperleft   =  dOriginY
+                            dLongitude_left1, dLatitude_top1= reproject_coordinates(dX_upperleft, dY_upperleft, pSpatialRef_dem,  spatial_reference_target)
+
+                            dLatitude_top = np.max([dLatitude_top0, dLatitude_top1])
+                            dLatitude_bot = np.min([dLatitude_bot0, dLatitude_bot1])
+
+                            dLongitude_left = np.min([dLongitude_left0, dLongitude_left1])
+                            dLongitude_right = np.max([dLongitude_right0, dLongitude_right1])
+
+                            dLatitude_mean = 0.5 * (dLatitude_top + dLatitude_bot)
+                            #pass
+
+                            if dResolution_meter < 0:
+                                #not used
+                                pass
+                            else:
+                                dResolution_degree = meter_to_degree(dResolution_meter, dLatitude_mean)
+
+                            dX_lowerleft = dOriginX
+                            dY_upperleft = dOriginY
+                        else:
+                            print("Error: DEM file does not exist: " + sFilename_dem)
+                            return
+                    pass
 
             if iMesh_type ==1: #hexagon
                 #hexagon edge
                 dResolution_meter = degree_to_meter(dLatitude_mean, dResolution_degree )
                 dArea = np.power(dResolution_meter,2.0)
                 dLength_edge = np.sqrt(  2.0 * dArea / (3.0* np.sqrt(3.0))  )
                 if iFlag_rotation ==0:
@@ -660,15 +682,15 @@
                     dX_spacing = dLength_edge * 1.5
                     dY_spacing = dLength_edge * np.sqrt(3.0)
                     ncolumn= int( (dX_lowerright - dX_lowerleft) / dX_spacing )+1
                     nrow= int( (dY_upperleft - dY_lowerleft) / dY_spacing )
 
                 if iFlag_mesh_boundary ==1:
                     #create a polygon based on real boundary
-                    pBoundary_wkt, aExtent = read_mesh_boundary(self.sFilename_mesh_boundary)
+                    pBoundary_wkt, aExtent = gdal_read_geojson_boundary(self.sFilename_mesh_boundary)
 
                     aHexagon = create_hexagon_mesh(iFlag_rotation, dX_lowerleft, dY_lowerleft, dResolution_meter, ncolumn, nrow, 
                                                    sFilename_mesh, sFilename_spatial_reference, pBoundary_wkt)
                     pass
                 else:
                     pRing = ogr.Geometry(ogr.wkbLinearRing)
                     pRing.AddPoint(dLongitude_left, dLatitude_top)
@@ -678,24 +700,28 @@
                     pRing.AddPoint(dLongitude_left, dLatitude_top)
                     pBoundary = ogr.Geometry(ogr.wkbPolygon)
                     pBoundary.AddGeometry(pRing)
                     pBoundary_wkt = pBoundary.ExportToWkt() #wkt format
 
                     aHexagon = create_hexagon_mesh(iFlag_rotation, dX_lowerleft, dY_lowerleft, dResolution_meter, ncolumn, nrow,
                                                    sFilename_mesh, sFilename_spatial_reference, pBoundary_wkt)
+                    
+                    
                     pass
 
+                
+
                 self.aCell = aHexagon
             else:
                 if iMesh_type ==2: #sqaure
                     ncolumn= int( (dX_lowerright - dX_lowerleft) / dResolution_meter )
                     nrow= int( (dY_upperleft - dY_lowerleft) / dResolution_meter )
                     if iFlag_mesh_boundary ==1:
                         #create a polygon based on real boundary
-                        pBoundary_wkt, aExtent= read_mesh_boundary(self.sFilename_mesh_boundary)
+                        pBoundary_wkt, aExtent= gdal_read_geojson_boundary(self.sFilename_mesh_boundary)
 
                         aSquare = create_square_mesh(dX_lowerleft, dY_lowerleft, dResolution_meter, ncolumn, nrow, 
                                                      sFilename_mesh, sFilename_spatial_reference, pBoundary_wkt)
                         pass
                     else:
                         pRing = ogr.Geometry(ogr.wkbLinearRing)
                         pRing.AddPoint(dLongitude_left, dLatitude_top)
@@ -717,15 +743,15 @@
                         dArea = np.power(dResolution_meter,2.0)
                         ncolumn= int( (dLongitude_right - dLongitude_left) / dResolution_degree )
                         nrow= int( (dLatitude_top - dLatitude_bot) / dResolution_degree )
 
                         if iFlag_mesh_boundary ==1:
                             #create a polygon based on real boundary
                             #already produced
-                            pBoundary_wkt , aExtent= read_mesh_boundary(self.sFilename_mesh_boundary)
+                            pBoundary_wkt , aExtent= gdal_read_geojson_boundary(self.sFilename_mesh_boundary)
                             aLatlon = create_latlon_mesh(dLongitude_left, dLatitude_bot, dResolution_degree, ncolumn, nrow, 
                                                          sFilename_mesh, pBoundary_wkt)
                             pass
                         else:
                             pRing = ogr.Geometry(ogr.wkbLinearRing)
                             pRing.AddPoint(dLongitude_left, dLatitude_top)
                             pRing.AddPoint(dLongitude_right, dLatitude_top)
@@ -739,15 +765,14 @@
                                                          sFilename_mesh, pBoundary_wkt)
 
                             pass
                     
                         self.aCell = aLatlon
 
                         
-
                     else:
                         if iMesh_type == 4: #mpas
                             iFlag_use_mesh_dem = self.iFlag_use_mesh_dem
                             sFilename_mesh_netcdf = self.sFilename_mesh_netcdf
                             dLatitude_top    = self.dLatitude_top
                             dLatitude_bot    = self.dLatitude_bot
                             dLongitude_left  = self.dLongitude_left
@@ -758,15 +783,15 @@
                                                          sFilename_mesh_netcdf, sFilename_mesh, iFlag_antarctic_in=iFlag_antarctic_in )
                                 pass
                             else:
 
                                 if iFlag_mesh_boundary ==1:
                                     #create a polygon based on
                                     #read boundary
-                                    pBoundary_wkt, aExtent = read_mesh_boundary(self.sFilename_mesh_boundary)
+                                    pBoundary_wkt, aExtent = gdal_read_geojson_boundary(self.sFilename_mesh_boundary)
 
                                     aMpas = create_mpas_mesh(iFlag_global, iFlag_use_mesh_dem, iFlag_save_mesh,
                                                              sFilename_mesh_netcdf,  sFilename_mesh, iFlag_antarctic_in=iFlag_antarctic_in, pBoundary_in = pBoundary_wkt)
                                     pass
                                 else:
                                     pRing = ogr.Geometry(ogr.wkbLinearRing)
                                     pRing.AddPoint(dLongitude_left, dLatitude_top)
@@ -801,16 +826,15 @@
                                     sWorkspace_output = os.path.abspath(sWorkspace_output)
                                     pass
 
                                 if not os.path.exists(sWorkspace_output):
                                     os.makedirs(sWorkspace_output)
                                 
                                 if iFlag_mesh_boundary ==1:
-                                        #create a polygon based on
-                                    
+                                        #create a polygon based on                                   
 
                                     aDggrid = create_dggrid_mesh(iFlag_global,
                                                                      iFlag_save_mesh,
                                                                      sFilename_mesh,
                                                                      sWorkspace_output,
                                                                      iResolution_index_in= self.iResolution_index,
                                                                      iFlag_antarctic_in=iFlag_antarctic_in,
@@ -818,16 +842,15 @@
                                                                      sFilename_boundary_in = self.sFilename_mesh_boundary)
                                     
                                     
                                                                      
                                     pass
                                 else:                                       
                                     aDggrid = create_dggrid_mesh(iFlag_global,
-                                                                     iFlag_save_mesh,
-                                                                     dResolution_meter,
+                                                                     iFlag_save_mesh,                                                                   
                                                                      sFilename_mesh,
                                                                      sWorkspace_output,
                                                                       iResolution_index_in= self.iResolution_index,
                                                                           sDggrid_type_in = self.sDggrid_type)
                                     
                                     pass
 
@@ -848,14 +871,17 @@
                                     nrow= int( (dY_upperleft - dY_lowerleft) / dY_spacing )
                                     aTin = create_tin_mesh(dX_lowerleft, dY_lowerleft, dResolution_meter, ncolumn, nrow, sFilename_mesh, sFilename_spatial_reference)
                                     self.aCell = aTin
                                 else:
 
                                     print('Unsupported mesh type?')
                                 return
+
+            #no matter what type of mash, we will convert it to geoparquet for easy visualization
+            convert_geojson_to_geoparquet(sFilename_mesh, sFilename_mesh.replace('.geojson','.parquet'))    
         else:            
             pass
 
         #build rtree
         if iFlag_use_rtree == 1:
             interleaved = True
             self.pRTree_mesh = RTree(interleaved=interleaved, max_cap=5, min_cap=2)
@@ -883,24 +909,22 @@
             iMesh_type = self.iMesh_type 
             sFilename_mesh=self.sFilename_mesh         
             aFlowline_conceptual = list()   #store all the flowline
             aCellID_outlet = list()
             aBasin = list()
             aCell_intersect=list()
             ncell=len(self.aCell)
-            #there is a one-to-one match between cell id and cell center because each cell has only one center         
-            
+            #there is a one-to-one match between cell id and cell center because each cell has only one center                  
             
             for pBasin in self.aBasin:
                 aCell_intersect_basin = pBasin.basin_reconstruct_topological_relationship(iMesh_type,sFilename_mesh)
                 aFlowline_conceptual = aFlowline_conceptual + pBasin.aFlowline_basin_conceptual
                 aBasin.append(pBasin)
                 aCellID_outlet.append(pBasin.lCellID_outlet)
                 aCell_intersect = aCell_intersect + aCell_intersect_basin
-
                 if iFlag_use_rtree == 1:
                     #use rtree to update topology and length
                     for pFlowline in pBasin.aFlowline_basin_conceptual:                    
                         iStream_segment = pFlowline.iStream_segment
                         iStream_order = pFlowline.iStream_order                    
                         for pEdge in pFlowline.aEdge:
                             pVertex_start = pEdge.pVertex_start
@@ -1011,15 +1035,16 @@
 
     def pyflowline_analyze(self):
         """
         Analyze the domain results for every watershed
         """
         if self.iFlag_flowline == 1:
             for pBasin in self.aBasin:
-                pBasin.analyze()
+                #pBasin.basin_analyze()
+                pass
         return
 
     def pyflowline_setup(self):
         """
         Set up the flowlinecase
         """
         if self.iFlag_flowline == 1:
@@ -1121,22 +1146,23 @@
             pBasin.evaluate(self.iMesh_type, self.sMesh_type)
         return
 
     def pyflowline_export(self):
         """
         Export the model outputs
         """
-        print('Started export elevation')
+        print('PyFlowline started export results')
         ptimer = pytimer()
         ptimer.start()
         self.pyflowline_export_mesh_info_to_json()
         #convert the mesh into the kml format so it can be visualized in google earth and google map
         #shoule move this to the export function
         if iFlag_kml is not None:
-            convert_geojson_to_kml(self.sFilename_mesh, self.sFilename_mesh_kml)
+            #convert_geojson_to_kml(self.sFilename_mesh, self.sFilename_mesh_kml)
+            pass
 
         if self.iFlag_flowline ==1:
             for pBasin in self.aBasin:
                 pBasin.basin_export()
 
         self.tojson()
         ptimer.stop()
```

### Comparing `pyflowline-0.3.4/pyflowline/classes/square.py` & `pyflowline-0.3.5/pyflowline/classes/square.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from json import JSONEncoder
 import numpy as np
 from pyflowline.classes.vertex import pyvertex
 from pyflowline.classes.edge import pyedge
 from pyflowline.classes.cell import pycell
 from pyflowline.classes.flowline import pyflowline
-from pyflowline.external.pyearth.gis.gdal.gdal_functions import calculate_polygon_area
+from pyearth.gis.geometry.calculate_polygon_area import calculate_polygon_area
 
 class SquareClassEncoder(JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.float32):
             return float(obj)
```

### Comparing `pyflowline-0.3.4/pyflowline/classes/timer.py` & `pyflowline-0.3.5/pyflowline/classes/timer.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/pyflowline/classes/tin.py` & `pyflowline-0.3.5/pyflowline/classes/tin.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/pyflowline/classes/vertex.py` & `pyflowline-0.3.5/pyflowline/classes/vertex.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 
 import json
 from json import JSONEncoder
-import importlib
+import importlib.util
 import numpy as np
 
 iFlag_cython = importlib.util.find_spec("cython") 
 if iFlag_cython is not None:
-    from pyflowline.algorithms.cython.kernel import calculate_distance_based_on_lon_lat
+    from pyflowline.algorithms.cython.kernel import calculate_distance_based_on_longitude_latitude
 else:
-    from pyflowline.external.pyearth.gis.gdal.gdal_functions import calculate_distance_based_on_lon_lat
+    from pyearth.gis.geometry.calculate_distance_based_on_longitude_latitude import calculate_distance_based_on_longitude_latitude
+
+iPrecision_default = 8 #used for comparison
 
 class VertexClassEncoder(JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.ndarray):
             return obj.tolist()        
@@ -96,15 +98,15 @@
         point =dict()
         point['x'] = x
         point['y'] = y
         point['z'] = z
         pNvector = pynvector(point)
         return pNvector
     
-    def __hash__(self, precision=6):
+    def __hash__(self, precision=iPrecision_default):
 
         #design a hash function that uses both dLongitude and dLatitude
 
         # Scale the dLatitude and dLongitude to a suitable range
         dLongitude = self.dLongitude_degree
         dLatitude = self.dLatitude_degree
 
@@ -125,28 +127,27 @@
         Args:
             other (pyvertex): The other vertex
 
         Returns:
             int: 1 if equivalent, 0 if not
         """
         iFlag = False
-        #dThreshold_in = 1.0E-6        
-        if isinstance(other, pyvertex):
-            #c = self.calculate_distance(other)
-            #if( c <= dThreshold_in ): #be careful
-            #    #print(self.dLongitude_degree ,self.dLatitude_degree , 
-            #    #other.dLongitude_degree, other.dLatitude_degree)
-            #    iFlag = True
-            #else:
-            #    iFlag = False    
+        dThreshold_in = 10 ** (-1 * iPrecision_default)     
+        if isinstance(other, pyvertex):              
             if (self.dLongitude_degree == other.dLongitude_degree) and \
                 (self.dLatitude_degree == other.dLatitude_degree):
                 iFlag = True
-            else:
-                iFlag = False
+            else:                
+                #use absolute difference to check whether two vertices are the same
+                if (abs(self.dLongitude_degree - other.dLongitude_degree) < dThreshold_in) and \
+                    (abs(self.dLatitude_degree - other.dLatitude_degree) < dThreshold_in):                  
+                    iFlag = True
+                else:
+                    iFlag = False  
+              
         else:
             iFlag = False 
 
         return iFlag
 
     def __ne__(self, other):
         """
@@ -171,15 +172,15 @@
             float: The great circle distance
         """
         dDistance = 0.0
         lon1 = self.dLongitude_degree
         lat1 = self.dLatitude_degree    
         lon2 = other.dLongitude_degree
         lat2 = other.dLatitude_degree
-        dDistance = calculate_distance_based_on_lon_lat(lon1, lat1, lon2, lat2)        
+        dDistance = calculate_distance_based_on_longitude_latitude(lon1, lat1, lon2, lat2)        
         return dDistance
     
     def tojson(self):
         """
         Convert a vecter object to a json string
 
         Returns:
```

### Comparing `pyflowline-0.3.4/pyflowline/formats/convert_attributes.py` & `pyflowline-0.3.5/pyflowline/formats/convert_attributes.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/pyflowline/formats/convert_coordinates.py` & `pyflowline-0.3.5/pyflowline/formats/convert_coordinates.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import importlib
+import importlib.util
 from pyflowline.classes.vertex import pyvertex
 from pyflowline.classes.edge import pyedge
 from pyflowline.classes.flowline import pyflowline
 
 from pyflowline.classes.hexagon import pyhexagon
 from pyflowline.classes.square import pysquare
 from pyflowline.classes.latlon import pylatlon
 from pyflowline.classes.mpas import pympas
 from pyflowline.classes.tin import pytin
 from pyflowline.classes.dggrid import pydggrid
 
-from pyflowline.external.pyearth.gis.gdal.gdal_functions import reproject_coordinates
+from pyearth.gis.spatialref.reproject_coodinates import reproject_coordinates
 iFlag_cython = importlib.util.find_spec("cython") 
 if iFlag_cython is not None:
     from pyflowline.algorithms.cython.kernel import calculate_angle_betwen_vertex
     from pyflowline.algorithms.cython.kernel import calculate_distance_to_plane
-else:
-    from pyflowline.external.pyearth.gis.gdal.gdal_functions import  calculate_angle_betwen_vertex
-    from pyflowline.external.pyearth.gis.gdal.gdal_functions import calculate_distance_to_plane
+else:   
+    from pyearth.gis.geometry.calculate_angle_betwen_vertex import calculate_angle_betwen_vertex
+    from pyearth.gis.geometry.calculate_distance_to_plane import calculate_distance_to_plane
 
 def convert_gcs_coordinates_to_cell(iMesh_type_in,     
                                     dLongitude_center_in,     
                                     dLatitude_center_in,         
                                     aCoordinates_gcs_in,        
                                     iFlag_simplify_in=None):
     
@@ -185,35 +185,45 @@
 
     Returns:
         _type_: _description_
     """
     
     npoint = len(aCoordinates_in)
     
-    aVertex=list()
-    for i in range(npoint):
-        x = aCoordinates_in[i][0]
-        y = aCoordinates_in[i][1]
-        dummy = dict()
-        dummy['dLongitude_degree'] = x
-        dummy['dLatitude_degree'] = y
-        pVertex = pyvertex(dummy)
-        aVertex.append(pVertex)
+    #aVertex=list()
+    #for i in range(npoint):
+    #    x = aCoordinates_in[i][0]
+    #    y = aCoordinates_in[i][1]
+    #    dummy = dict()
+    #    dummy['dLongitude_degree'] = x
+    #    dummy['dLatitude_degree'] = y
+    #    pVertex = pyvertex(dummy)
+    #    aVertex.append(pVertex)
+
+    #simplified using a list comprehension.
+
+    aVertex = [pyvertex({'dLongitude_degree': x, 'dLatitude_degree': y}) for x, y in aCoordinates_in]
+    
         
-    aEdge=list()
-    for j in range(npoint-1):
-        if aVertex[j] == aVertex[j+1]:
-            print('Two vertices are the same')
-            pass
-        else:
-            pEdge = pyedge( aVertex[j], aVertex[j+1] )
-            aEdge.append(pEdge)
+    #aEdge=list()
+    #for j in range(npoint-1):
+    #    if aVertex[j] == aVertex[j+1]:
+    #        print('Two vertices are the same')
+    #        pass
+    #    else:
+    #        pEdge = pyedge( aVertex[j], aVertex[j+1] )
+    #        aEdge.append(pEdge)
+
+    aEdge = [pyedge(aVertex[j], aVertex[j+1]) for j in range(npoint - 1) if aVertex[j] != aVertex[j+1]]
+    
+    if len(aEdge) == 0:
+        print('No edge is created')
+        return None
     
-    pFlowline = pyflowline( aEdge)    
-    return pFlowline
+    return pyflowline(aEdge)
 
 def convert_pcs_coordinates_to_flowline(aCoordinates_in, pSpatial_reference_in):
     npoint = len(aCoordinates_in)
     
     aVertex=list()
     for i in range(npoint):
         x = aCoordinates_in[i][0]
```

### Comparing `pyflowline-0.3.4/pyflowline/formats/convert_flowline_to_geojson.py` & `pyflowline-0.3.5/pyflowline/formats/convert_flowline_to_geojson.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,23 +18,23 @@
         iReturn_code = 0
         return iReturn_code
 
     if iFlag_type_in ==0:
         pass
     else:
         if iFlag_type_in == 1:
-            
-            aFlowline_basin, pSpatial_reference = read_flowline_geojson( sFilename_geojson_in )   
+            sFilename_dummy = sFilename_geojson_out
+            sFilename_out = sFilename_dummy.replace('.geojson', '_withID.geojson')            
+            aFlowline_basin, pSpatial_reference = read_flowline_geojson( sFilename_geojson_in , sFilename_out = sFilename_out)   
+            #get lineid
+            aFlowlineID = [pFlowline.lFlowlineID for pFlowline in aFlowline_basin]          
             #convert it
-
-            iFlag_projected = 0
-            #pSpatial_reference_gcs = osr.SpatialReference()
-            #pSpatial_reference_gcs.ImportFromEPSG(4326)
-            #pSpatial_reference_gcs.SetAxisMappingStrategy(osr.OAMS_TRADITIONAL_GIS_ORDER)
-            export_flowline_to_geojson(aFlowline_basin, sFilename_geojson_out)
+            iFlag_projected = 0       
+            export_flowline_to_geojson(aFlowline_basin, sFilename_geojson_out, aAttribute_field=['lineid'],
+                                       aAttribute_dtype=['int'], aAttribute_data=[aFlowlineID])
         else:
             if iFlag_type_in == 2:
                 #polygon
                 pass
 
 
     return
@@ -56,15 +56,14 @@
         return iReturn_code
 
     if iFlag_type_in == 0:
         pass
     else:
         if iFlag_type_in == 1:
             aFlowline_basin, pSpatial_reference = read_flowline_shapefile( sFilename_shapefile_in )    
-            #aFlowline_basin, pSpatial_reference = read_flowline_geojson( sFilename_shapefile_in )   
             #convert it
 
             iFlag_projected = 0
             pSpatial_reference_gcs = osr.SpatialReference()
             pSpatial_reference_gcs.ImportFromEPSG(4326)
             pSpatial_reference_gcs.SetAxisMappingStrategy(osr.OAMS_TRADITIONAL_GIS_ORDER)
             export_flowline_to_geojson(aFlowline_basin, sFilename_geojson_in)
```

### Comparing `pyflowline-0.3.4/pyflowline/formats/export_flowline.py` & `pyflowline-0.3.5/pyflowline/formats/export_flowline.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,111 +11,129 @@
     pSpatial_reference_in=None, 
     aAttribute_field=None,
     aAttribute_data=None,
     aAttribute_dtype=None):
     
     
     """
-    convert a shpefile to json format.
+    convert a flowlist object list to json format.
     This function should be used for stream flowline only.
     """
 
     if os.path.exists(sFilename_json_in): 
         os.remove(sFilename_json_in)
-        pass
 
     nFlowline = len(aFlowline_in)
     if iFlag_projected_in is None:
         iFlag_projected_in = 0
     else:
         iFlag_projected_in = 1
 
     if  pSpatial_reference_in is None:        
         pSpatial_reference_in = osr.SpatialReference()  
         pSpatial_reference_in.ImportFromEPSG(4326)    # WGS84 lat/lon
     else:
         pass
 
-    if aAttribute_field is not None and aAttribute_data is not None and aAttribute_dtype is not None:
-        iFlag_attribute = 1
+    iFlag_attribute = int(all([aAttribute_field, aAttribute_data, aAttribute_dtype]))
+
 
-        nAttribute1 = len(aAttribute_field)
-        nAttribute2 = len(aAttribute_data)
-        nAttribute3 = len(aAttribute_dtype)
-        nAttribute4 = len(aAttribute_data[0])
-        if nAttribute3 != nAttribute1 or nAttribute1 != nAttribute2 or nFlowline!= nAttribute4:
+    #if aAttribute_field is not None and aAttribute_data is not None and aAttribute_dtype is not None:
+    #    iFlag_attribute = 1
+    #    nAttribute1 = len(aAttribute_field)
+    #    nAttribute2 = len(aAttribute_data)
+    #    nAttribute3 = len(aAttribute_dtype)
+    #    nAttribute4 = len(aAttribute_data[0])
+    #    if nAttribute3 != nAttribute1 or nAttribute1 != nAttribute2 or nFlowline!= nAttribute4:
+    #        print('The attribute is not correct, please check!')
+    #        return
+    #    else:
+    #        iFlag_attribute = 1
+    #else:
+    #    iFlag_attribute=0
+    #    pass
+
+    if iFlag_attribute:
+        nAttribute1, nAttribute2, nAttribute3 = map(len, [aAttribute_field, aAttribute_data, aAttribute_dtype])
+        if not nAttribute1 == nAttribute2 == nAttribute3 and nFlowline != len(aAttribute_data[0]):
             print('The attribute is not correct, please check!')
             return
-        else:
-            iFlag_attribute = 1
-    else:
-        iFlag_attribute=0
-        pass
 
 
-    pDriver_json = ogr.GetDriverByName('GeoJSON')
-    
-    pDataset_json = pDriver_json.CreateDataSource(sFilename_json_in)  
-    
-
+    pDriver_json = ogr.GetDriverByName('GeoJSON')    
+    pDataset_json = pDriver_json.CreateDataSource(sFilename_json_in)     
     pLayer_json = pDataset_json.CreateLayer('flowline', pSpatial_reference_in, ogr.wkbLineString)
     # Add one attribute
     pLayer_json.CreateField(ogr.FieldDefn('lineid', ogr.OFTInteger64)) #long type for high resolution
 
     #add the other fields
-    if iFlag_attribute ==1:
-        for i in range(nAttribute1):
-            sField = aAttribute_field[i]
-            dtype = aAttribute_dtype[i]
-            if dtype == 'int':
-                pLayer_json.CreateField(ogr.FieldDefn(sField, ogr.OFTInteger64))
-                pass
-            else:
-                pLayer_json.CreateField(ogr.FieldDefn(sField, ogr.OFTReal))
-                pass
+    #if iFlag_attribute ==1:
+    #    for i in range(nAttribute1):
+    #        sField = aAttribute_field[i]
+    #        dtype = aAttribute_dtype[i]
+    #        if dtype == 'int':
+    #            pLayer_json.CreateField(ogr.FieldDefn(sField, ogr.OFTInteger64))
+    #            pass
+    #        else:
+    #            pLayer_json.CreateField(ogr.FieldDefn(sField, ogr.OFTReal))
+    #            pass
+    
+    dtype_to_ogr = {'int': ogr.OFTInteger64, 'float': ogr.OFTReal}
+    if iFlag_attribute:
+        for field, dtype in zip(aAttribute_field, aAttribute_dtype):
+            pLayer_json.CreateField(ogr.FieldDefn(field, dtype_to_ogr[dtype]))
         
     
     pLayerDefn = pLayer_json.GetLayerDefn()
     pFeature_out = ogr.Feature(pLayerDefn)
 
-    lID = 0
-    for i in range(nFlowline):
-        pFlowline = aFlowline_in[i]
-        dummy =pFlowline.aVertex
+    #lID = 0
+    flag_to_attr = {1: ('dx', 'dy'), 0: ('dLongitude_degree', 'dLatitude_degree')}
+    for lID in range(nFlowline):
+        pFlowline = aFlowline_in[lID]
+        #dummy =pFlowline.aVertex
         #replace shapely with gdal function
         #aPoint=list()
         pLine = ogr.Geometry(ogr.wkbLineString)
-        for j in dummy:
-            if iFlag_projected_in ==1:
-                #aPoint.append( Point( j.dx, j.dy ) )                
-                pLine.AddPoint(j.dx, j.dy)
-                pass
-            else:
-                #aPoint.append( Point( j.dLongitude_degree, j.dLatitude_degree ) )
-                pLine.AddPoint(j.dLongitude_degree, j.dLatitude_degree)
-                pass
+        #for j in dummy:
+        #    if iFlag_projected_in ==1:
+        #        #aPoint.append( Point( j.dx, j.dy ) )                
+        #        pLine.AddPoint(j.dx, j.dy)
+        #        pass
+        #    else:
+        #        #aPoint.append( Point( j.dLongitude_degree, j.dLatitude_degree ) )
+        #        pLine.AddPoint(j.dLongitude_degree, j.dLatitude_degree)
+        #        pass
+
+        for vertex in pFlowline.aVertex:
+            pLine.AddPoint(*(getattr(vertex, attr) for attr in flag_to_attr[iFlag_projected_in]))
+
 
         #dummy1= LineString( aPoint )
         pGeometry_out = ogr.CreateGeometryFromWkb(pLine.ExportToWkb())
-        pFeature_out.SetGeometry(pGeometry_out)
-   
+        pFeature_out.SetGeometry(pGeometry_out)   
         pFeature_out.SetField("lineid", lID)
+
+        #if iFlag_attribute == 1:
+        #    for k in range(nAttribute1):
+        #        sField = aAttribute_field[k]
+        #        dtype = aAttribute_dtype[k]
+        #        dummy = aAttribute_data[k]
+        #        if dtype == 'int':
+        #            pFeature_out.SetField(sField, int(dummy[lID]))
+        #        else:
+        #            pFeature_out.SetField(sField, float(dummy[lID]))
+                
         if iFlag_attribute == 1:
-            for k in range(nAttribute1):
-                sField = aAttribute_field[k]
-                dtype = aAttribute_dtype[k]
-                dummy = aAttribute_data[k]
-                if dtype == 'int':
-                    pFeature_out.SetField(sField, int(dummy[i]))
-                else:
-                    pFeature_out.SetField(sField, float(dummy[i]))
+            for sField, dtype, dummy in zip(aAttribute_field, aAttribute_dtype, aAttribute_data):
+                pFeature_out.SetField(sField, int(dummy[lID]) if dtype == 'int' else float(dummy[lID]))
         
         # Add new pFeature_shapefile to output Layer
         pLayer_json.CreateFeature(pFeature_out)        
-        lID =  lID + 1
+      
         pass
         
     pDataset_json.FlushCache()
     pDataset_json = pLayer_json = pFeature_out  = None    
 
     return
```

### Comparing `pyflowline-0.3.4/pyflowline/formats/export_mesh.py` & `pyflowline-0.3.5/pyflowline/formats/export_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/pyflowline/formats/export_vertex.py` & `pyflowline-0.3.5/pyflowline/formats/export_vertex.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from osgeo import ogr, osr
-#from shapely.geometry import Point
+
 
 def export_vertex_to_geojson(aVertex_in, 
         sFilename_json_in,
         iFlag_projected_in=None,
         pSpatial_reference_in=None, 
         aAttribute_data=None):
     """
@@ -18,68 +18,72 @@
         pSpatial_reference_in (_type_, optional): _description_. Defaults to None.
         aAttribute_data (_type_, optional): _description_. Defaults to None.
     """
     
 
     if os.path.exists(sFilename_json_in): 
         os.remove(sFilename_json_in)
-        pass
-    
-    if iFlag_projected_in is None:
-        iFlag_projected_in = 0
-    else:
-        iFlag_projected_in = 1
+
+    iFlag_projected_in = 0 if iFlag_projected_in is None else 1
 
     if  pSpatial_reference_in is None:        
         pSpatial_reference_in = osr.SpatialReference()  
         pSpatial_reference_in.ImportFromEPSG(4326)    # WGS84 lat/lon
-    else:
-        pass
 
-    if aAttribute_data is not None:
-        aAttribute= aAttribute_data
-        iFlag_attribute =1
-    else:
-        iFlag_attribute=0
 
-    nVertex = len(aVertex_in)
+    iFlag_attribute = 1 if aAttribute_data is not None else 0
+    aAttribute = aAttribute_data if aAttribute_data is not None else []
+
+    #nVertex = len(aVertex_in)
     pDriver = ogr.GetDriverByName('GeoJSON')        
     pDataset_json = pDriver.CreateDataSource(sFilename_json_in)
     pLayer_json = pDataset_json.CreateLayer('vertex', pSpatial_reference_in, ogr.wkbPoint)
     # Add one attribute
     pLayer_json.CreateField(ogr.FieldDefn('pointid', ogr.OFTInteger64)) #long type for high resolution
     if iFlag_attribute ==1:        
         pLayer_json.CreateField(ogr.FieldDefn('connectivity', ogr.OFTInteger64)) #long type for high resolution
         pass
 
     pLayerDefn = pLayer_json.GetLayerDefn()
     pFeature_out = ogr.Feature(pLayerDefn)
-    lID = 0
-    for i in range(nVertex):       
-        pVertex = aVertex_in[i]
+    #lID = 0
+    #for i in range(nVertex):       
+    #    pVertex = aVertex_in[i]
+    #    pPoint = ogr.Geometry(ogr.wkbPoint)
+    #    if iFlag_projected_in ==1:           
+    #        pPoint.AddPoint(pVertex.dx, pVertex.dy)
+    #        pass
+    #    else:
+    #        pPoint.AddPoint(pVertex.dLongitude_degree, pVertex.dLatitude_degree)
+    #        pass
+    #    pGeometry_out = ogr.CreateGeometryFromWkb(pPoint.ExportToWkb())
+    #    pFeature_out.SetGeometry(pGeometry_out)   
+    #    pFeature_out.SetField("pointid", lID)
+    #    if iFlag_attribute ==1:
+    #        pFeature_out.SetField("connectivity", int(aAttribute[i]) )
+    #            
+    #    pLayer_json.CreateFeature(pFeature_out)        
+    #    lID =  lID + 1
+    #    pass
+
+    for lID, pVertex in enumerate(aVertex_in):
         pPoint = ogr.Geometry(ogr.wkbPoint)
-        if iFlag_projected_in ==1:
-            #dummy1= Point( pVertex.dx, pVertex.dy )
+        if iFlag_projected_in == 1:
             pPoint.AddPoint(pVertex.dx, pVertex.dy)
-            pass
         else:
-            #dummy1= Point( pVertex.dLongitude_degree, pVertex.dLatitude_degree ) 
             pPoint.AddPoint(pVertex.dLongitude_degree, pVertex.dLatitude_degree)
-            pass
-
 
         pGeometry_out = ogr.CreateGeometryFromWkb(pPoint.ExportToWkb())
         pFeature_out.SetGeometry(pGeometry_out)   
         pFeature_out.SetField("pointid", lID)
-        if iFlag_attribute ==1:
-            pFeature_out.SetField("connectivity", int(aAttribute[i]) )
-                
-        pLayer_json.CreateFeature(pFeature_out)        
-        lID =  lID + 1
-        pass
+
+        if iFlag_attribute == 1:
+            pFeature_out.SetField("connectivity", int(aAttribute[lID]))
+
+        pLayer_json.CreateFeature(pFeature_out)    
         
     pDataset_json.FlushCache()
     pDataset_json = pLayer_json = pFeature_out  = None    
 
     return
```

### Comparing `pyflowline-0.3.4/pyflowline/formats/read_flowline.py` & `pyflowline-0.3.5/pyflowline/formats/read_flowline.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import json
 import numpy as np
 from osgeo import ogr, osr, gdal
 from pyflowline.formats.convert_coordinates import convert_gcs_coordinates_to_flowline
 
 def read_flowline_shapefile(sFilename_shapefile_in):
     """
     convert a shpefile to json format.
@@ -143,33 +144,72 @@
                 print(sGeometry_type)
                 pass
     
 
     return aFlowline, pSpatialRef_shapefile
 
 
-def read_flowline_geojson(sFilename_geojson_in):
+def read_flowline_geojson(sFilename_geojson_in, sFilename_out = None):
     """
     read a geojson flowline
     This function should be used for stream flowline only.
     """
-
     aFlowline=list()
     pDriver_geojson = ogr.GetDriverByName('GeoJSON')   
     if os.path.isfile(sFilename_geojson_in):
         #print(sFilename_geojson_in)
         pass
     else:
         print('This geojson file does not exist: ', sFilename_geojson_in )
         exit()
+
+    if sFilename_out is not None:
+        # Open the GeoJSON file        
+        dataSource = pDriver_geojson.Open(sFilename_geojson_in, 1)  # 1 means writable
+        # Get the layer
+        layer = dataSource.GetLayer()
+        if os.path.exists(sFilename_out):
+            os.remove(sFilename_out)
+
+        # Create a new GeoJSON file
+        new_dataSource = pDriver_geojson.CreateDataSource(sFilename_out)
+
+        # Create a new layer with the same definition as the original layer
+        new_layer = new_dataSource.CreateLayer(layer.GetName(), layer.GetSpatialRef(), ogr.wkbMultiLineString)
+
+        # Add fields to the new layer
+        layer_defn = layer.GetLayerDefn()
+        for i in range(layer_defn.GetFieldCount()):
+            new_layer.CreateField(layer_defn.GetFieldDefn(i))
+
+        # Check if the field exists
+        field_names = [field.name for field in new_layer.schema]
+
+        if "lineid" not in field_names:
+            # Add a new field
+            new_field = ogr.FieldDefn("lineid", ogr.OFTInteger)
+            new_layer.CreateField(new_field)
+
+        # Copy features from the original layer to the new layer and assign an ID to each feature
+        for i, feature in enumerate(layer):
+            new_feature = ogr.Feature(new_layer.GetLayerDefn())
+            new_feature.SetFrom(feature)
+            new_feature.SetField("lineid", i + 1)
+            new_layer.CreateFeature(new_feature)
+
+        # Save and close the data sources
+        dataSource = None
+        new_dataSource = None
+        sFilename_geojson_in = sFilename_out #use this dataset because it has lineid
+            
     pDataset_geojson = pDriver_geojson.Open(sFilename_geojson_in, gdal.GA_ReadOnly)
     pLayer_geojson = pDataset_geojson.GetLayer(0)
     pSpatialRef_geojson = pLayer_geojson.GetSpatialRef()
     ldefn = pLayer_geojson.GetLayerDefn()
-    schema =list()
+    schema = list()
     for n in range(ldefn.GetFieldCount()):
         fdefn = ldefn.GetFieldDefn(n)
         schema.append(fdefn.name)
     if 'stream_segment' in schema:
         iFlag_segment = 1
     else:
         iFlag_segment = 0    
@@ -186,16 +226,19 @@
     else:
         iFlag_NHDPlusID = 0
     
 
     lFlowlineIndex = 0
     lFlowlineID = 1
     lVertexID = 1
-    for pFeature_geojson in pLayer_geojson:
-        #pGeometry_geojson = pFeature_geojson.GetGeometryRef()
+    nFeature = pLayer_geojson.GetFeatureCount()
+    #for pFeature_geojson in pLayer_geojson:
+    #pGeometry_geojson = pFeature_geojson.GetGeometryRef()
+    for iFeature in range(nFeature):
+        pFeature_geojson = pLayer_geojson.GetFeature(iFeature)
         pGeometry_in = pFeature_geojson.GetGeometryRef()
         sGeometry_type = pGeometry_in.GetGeometryName()
         if iFlag_segment ==1:
             iStream_segment = pFeature_geojson.GetField("stream_segment")
         else:
             iStream_segment = -1
 
@@ -203,55 +246,54 @@
             iStream_order = pFeature_geojson.GetField("stream_order")
         else:
             iStream_order = -1
         
         if iFlag_id ==1:
             lFlowlineID = pFeature_geojson.GetField("lineid")
         else:
-            lFlowlineID = -1
+            lFlowlineID=-1
+            pass
 
         if iFlag_NHDPlusID ==1:
             lNHDPlusID = pFeature_geojson.GetField("NHDPlusID")
         else:
             lNHDPlusID = -1
         
         if(sGeometry_type == 'MULTILINESTRING'):
             nLine = pGeometry_in.GetGeometryCount()
             for i in range(nLine):
-                Line = pGeometry_in.GetGeometryRef(i)       
-                aCoords = list()
-                for i in range(0,  Line.GetPointCount()):                   
-                    pt = Line.GetPoint(i)
-                    aCoords.append( [ pt[0], pt[1]]) 
-                    pass
-
-                dummy1= np.array(aCoords)
-                pFlowline = convert_gcs_coordinates_to_flowline(dummy1)
-                pFlowline.lFlowlineIndex = lFlowlineIndex
-                pFlowline.lFlowlineID = lFlowlineID
-                pFlowline.lNHDPlusID= lNHDPlusID
-                aFlowline.append(pFlowline)
-                lFlowlineIndex = lFlowlineIndex + 1
+                Line = pGeometry_in.GetGeometryRef(i)                    
+                aCoords = [[pt[0], pt[1]] for pt in Line.GetPoints()]
+                pFlowline = convert_gcs_coordinates_to_flowline(np.array(aCoords))
+                if pFlowline is not None:
+                    pFlowline.lFlowlineIndex = lFlowlineIndex
+                    pFlowline.lFlowlineID = lFlowlineID
+                    pFlowline.lNHDPlusID= lNHDPlusID
+                    aFlowline.append(pFlowline)
+                    lFlowlineIndex = lFlowlineIndex + 1
+                    if iFlag_id !=1:
+                        lFlowlineID = lFlowlineID + 1 #careful
+                else:
+                    print('Error in reading multi flowline: ', iFeature, i, aCoords) 
         
         else:
-            if sGeometry_type =='LINESTRING':                  
-                aCoords = list()
-                for i in range(0, pGeometry_in.GetPointCount()):                   
-                    pt = pGeometry_in.GetPoint(i)
-                    aCoords.append( [ pt[0], pt[1]])
-                    pass      
-
-                dummy1= np.array(aCoords)
-                pFlowline = convert_gcs_coordinates_to_flowline(dummy1)
-                pFlowline.lFlowlineIndex = lFlowlineIndex
-                pFlowline.iStream_segment = iStream_segment
-                pFlowline.iStream_order = iStream_order
-                pFlowline.lFlowlineID = lFlowlineID
-                pFlowline.lNHDPlusID = lNHDPlusID
-                aFlowline.append(pFlowline)
-                lFlowlineIndex = lFlowlineIndex + 1            
+            if sGeometry_type =='LINESTRING':         
+                aCoords = [[pt[0], pt[1]] for pt in pGeometry_in.GetPoints()]
+                pFlowline = convert_gcs_coordinates_to_flowline(np.array(aCoords))
+                if pFlowline is not None:
+                    pFlowline.lFlowlineIndex = lFlowlineIndex
+                    pFlowline.iStream_segment = iStream_segment
+                    pFlowline.iStream_order = iStream_order
+                    pFlowline.lFlowlineID = lFlowlineID
+                    pFlowline.lNHDPlusID = lNHDPlusID
+                    aFlowline.append(pFlowline)
+                    lFlowlineIndex = lFlowlineIndex + 1   
+                    if iFlag_id !=1:
+                        lFlowlineID = lFlowlineID + 1  #careful   
+                else:
+                    print('Error in reading single flowline: ', iFeature)     
             else:
                 print(sGeometry_type)
                 pass        
 
 
-    return aFlowline, pSpatialRef_geojson
+    return aFlowline, pSpatialRef_geojson
```

### Comparing `pyflowline-0.3.4/pyflowline/formats/read_mesh.py` & `pyflowline-0.3.5/pyflowline/formats/read_mesh.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import numpy as np
 from osgeo import ogr, gdal
 #from shapely.wkt import loads
 from pyflowline.formats.convert_coordinates import convert_gcs_coordinates_to_cell
-from pyflowline.external.pyearth.gis.gdal.gdal_functions import get_geometry_coords
+from pyearth.gis.location.get_geometry_coordinates import get_geometry_coordinates
 def read_mesh_json(iMesh_type_in, sFilename_mesh_in):
     """
     convert a shpefile to json format.
     This function should be used for stream flowline only.
     """
     iReturn_code = 1
     if os.path.isfile(sFilename_mesh_in):
@@ -34,15 +34,15 @@
 
     #we also need to spatial reference
     for pFeature_mesh in pLayer_mesh:
         pGeometry_mesh = pFeature_mesh.GetGeometryRef()        
         #dummy0 = loads( pGeometry_mesh.ExportToWkt() )
         #aCoords_gcs = dummy0.exterior.coords
         #aCoords_gcs= np.array(aCoords_gcs)
-        aCoords_gcs = get_geometry_coords(pGeometry_mesh)       
+        aCoords_gcs = get_geometry_coordinates(pGeometry_mesh)       
         lCellID = pFeature_mesh.GetField("cellid")
         dLon = pFeature_mesh.GetField("longitude")
         dLat = pFeature_mesh.GetField("latitude")        
         dArea = pFeature_mesh.GetField("area")
         if iMesh_type_in == 4:
             dElevation_mean = pFeature_mesh.GetField("elevation_mean")
             dElevation_profile0 = pFeature_mesh.GetField("elevation_profile0")
@@ -92,15 +92,15 @@
 
     #we also need to spatial reference
     for pFeature_mesh in pLayer_mesh:
         pGeometry_mesh = pFeature_mesh.GetGeometryRef()        
         #dummy0 = loads( pGeometry_mesh.ExportToWkt() )
         #aCoords_gcs = dummy0.exterior.coords
         #aCoords_gcs= np.array(aCoords_gcs)      
-        aCoords_gcs = get_geometry_coords(pGeometry_mesh)    
+        aCoords_gcs = get_geometry_coordinates(pGeometry_mesh)    
         lCellID = pFeature_mesh.GetField("cellid")
         dLon = pFeature_mesh.GetField("longitude")
         dLat = pFeature_mesh.GetField("latitude")        
         dArea = pFeature_mesh.GetField("area")
         if iMesh_type_in == 4:
             dElevation_mean = pFeature_mesh.GetField("elevation_mean")
             dElevation_profile0 = pFeature_mesh.GetField("elevation_profile0")
```

### Comparing `pyflowline-0.3.4/pyflowline/formats/read_nhdplus_flowline_shapefile.py` & `pyflowline-0.3.5/pyflowline/formats/read_nhdplus_flowline_shapefile.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/pyflowline/mesh/dggrid/create_dggrid_mesh.py` & `pyflowline-0.3.5/pyflowline/mesh/dggrid/create_dggrid_mesh.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 import os, stat
 import numpy as np
 from pathlib import Path
 import subprocess
 import datetime
 from shutil import copy2
 from osgeo import osr, ogr, gdal
-#from shapely.wkt import loads
-from pyflowline.formats.convert_coordinates import convert_gcs_coordinates_to_cell
 
-from pyflowline.external.pyearth.system.define_global_variables import *
+from pyflowline.formats.convert_coordinates import convert_gcs_coordinates_to_cell
 from pyflowline.formats.convert_attributes import convert_gcs_attributes_to_cell
-from pyflowline.external.pyearth.gis.gdal.gdal_functions import get_geometry_coords
+from pyearth.system.define_global_variables import *
+from pyearth.gis.location.get_geometry_coordinates import get_geometry_coordinates
 
 pDate = datetime.datetime.today()
 sDate_default = "{:04d}".format(pDate.year) + "{:02d}".format(pDate.month) + "{:02d}".format(pDate.day)
 
 #setup common resolution
 aISEA3H = [4320.490,
            2539.690,
@@ -126,33 +125,38 @@
         if sDggrid_type == 'ISEA4H':
             dResolution = aISEA4H[iResolution_index-1 ] * 1000
             pass
         pass
 
     return dResolution
 
-def convert_dggrid_mesh_to_pyflowline_mesh(sFilename_dggrid_mesh, sFilename_mesh_pyflowline):
+def convert_dggrid_mesh_to_pyflowline_mesh(sFilename_dggrid_mesh, sFilename_mesh_pyflowline,
+                                            iFlag_global_in = None):
     
     iReturn_code = 1
     if os.path.isfile(sFilename_dggrid_mesh):
         print(sFilename_dggrid_mesh)
         pass
     else:
         print('This mesh file does not exist: ', sFilename_dggrid_mesh )
         iReturn_code = 0
         return iReturn_code
     
+    if iFlag_global_in is not None:
+        iFlag_global = iFlag_global_in
+    else:
+        iFlag_global = 0
+    
     if os.path.isfile(sFilename_mesh_pyflowline):
         print('This mesh file already exists: ', sFilename_mesh_pyflowline )
         os.remove(sFilename_mesh_pyflowline)
 
     aDggrid=list()
     aDggrid_dict = dict()
     lCellIndex = 0
-
     pDriver_geojson = ogr.GetDriverByName('GeoJSON')    
     pDataset_mesh = pDriver_geojson.Open(sFilename_dggrid_mesh, gdal.GA_ReadOnly)
     pLayer_mesh = pDataset_mesh.GetLayer(0)
     pSpatial_reference_out = pLayer_mesh.GetSpatialRef()
     ldefn = pLayer_mesh.GetLayerDefn()
 
     pSpatial_reference_gcs = osr.SpatialReference()  
@@ -168,29 +172,24 @@
     pArea_field.SetPrecision(2)
     pLayer.CreateField(pArea_field)
     pLayerDefn = pLayer.GetLayerDefn()
     pFeature = ogr.Feature(pLayerDefn)   
     
     #we also need to spatial reference
     for pFeature_mesh in pLayer_mesh:
-        pGeometry_mesh = pFeature_mesh.GetGeometryRef()        
-        #dummy0 = loads( pGeometry_mesh.ExportToWkt() )
-        #aCoords_gcs = dummy0.exterior.coords
-        #aCoords_gcs= np.array(aCoords_gcs)  
-        aCoords_gcs = get_geometry_coords(pGeometry_mesh)   
+        pGeometry_mesh = pFeature_mesh.GetGeometryRef()              
+        aCoords_gcs = get_geometry_coordinates(pGeometry_mesh)   
         dLongitude_center = np.mean(aCoords_gcs[:-1,0])
         dLatitude_center = np.mean(aCoords_gcs[:-1,1])   
-
         lCellID = int(pFeature_mesh.GetField("name") )
         pdggrid = convert_gcs_coordinates_to_cell(5, dLongitude_center, dLatitude_center, aCoords_gcs)  
         dArea = pdggrid.calculate_cell_area()
         pdggrid.calculate_edge_length()
         pdggrid.dLength_flowline = pdggrid.dLength #Default
         pdggrid.lCellID = lCellID      
-
         aNeighbor = pFeature_mesh.GetField("neighbors")   
         pdggrid.nNeighbor = len(aNeighbor)
         pdggrid.aNeighbor = list()
         for i in range(len(aNeighbor)):
             pdggrid.aNeighbor.append( int(aNeighbor[i]) )       
 
         aDggrid.append(pdggrid)
@@ -214,45 +213,45 @@
         pFeature.SetField("longitude", dLongitude_center )
         pFeature.SetField("latitude", dLatitude_center )
         pFeature.SetField("area", dArea )
       
         pLayer.CreateFeature(pFeature)
 
     #rebuild neighbor list    
-    aDggrid_out = list()
-    
-    ncell = len(aDggrid)
-    aCellID  = list()
- 
+    aDggrid_middle = list()      
     for pCell in aDggrid:           
         aNeighbor = pCell.aNeighbor       
         aNeighbor_new = list()       
         for lNeighbor in aNeighbor:            
             if lNeighbor in aDggrid_dict:                
                 aNeighbor_new.append(lNeighbor)
         
         pCell.aNeighbor = aNeighbor_new
         pCell.nNeighbor = len(aNeighbor_new)
         pCell.nNeighbor_land= len(aNeighbor_new)
         pCell.aNeighbor_land = aNeighbor_new
         pCell.nNeighbor_ocean = pCell.nVertex - pCell.nNeighbor_land
-        aDggrid_out.append(pCell)
+        aDggrid_middle.append(pCell)
 
     #calculate neighbor distance
-    for pDggrid in aDggrid_out:
+    for pDggrid in aDggrid_middle:
         aNeighbor = pDggrid.aNeighbor
         pDggrid.aNeighbor_distance=list()
         for lCellID1 in aNeighbor:
             lIndex = aDggrid_dict[lCellID1]
-            pDggrid1 = aDggrid_out[lIndex]  
+            pDggrid1 = aDggrid_middle[lIndex]  
             dDistance = pDggrid.pVertex_center.calculate_distance( pDggrid1.pVertex_center )
             pDggrid.aNeighbor_distance.append(dDistance)
      
     pDataset = pLayer = pFeature  = None  
-    return aDggrid_out
+
+    #currently we do not fill the holes in dggrid, it is recommended to modify the input data directly.
+
+    
+    return aDggrid_middle
 
 def create_dggrid_mesh(iFlag_global,
                          iFlag_save_mesh,
                          sFilename_mesh,
                          sWorkspace_output, #for dggrid
                          iResolution_index_in = None,
                          sDggrid_type_in= None,
@@ -275,18 +274,21 @@
     dResolution= dggrid_find_resolution_by_index(sDggrid_type, iResolution_index)  
     print('Resolution is: ', dResolution)
     #  
     sResolution = "{:0d}".format( iResolution_index )
 
     if sFilename_boundary_in is not None:
         if os.path.isfile(sFilename_boundary_in):
-            iFlag_crop =1
+            iFlag_crop = 1
+            iFlag_global = 0
             sFilename_crop_geojson = sFilename_boundary_in
         else:
             iFlag_crop = 0
+            iFlag_global = 1
+
     else:
         iFlag_crop = 0   
 
     iFlag_mode = 1 
 
     if iFlag_mode == 1: #call the binary directly    
         #write configuration
@@ -328,15 +330,16 @@
         sCommand = "./run_dggrid.sh"
         print(sCommand)
         p = subprocess.Popen(sCommand, shell= True)
         p.wait()
 
         #convert the pyflowline mesh format
              
-        aDggrid = convert_dggrid_mesh_to_pyflowline_mesh(sFilename_cell, sFilename_mesh)
+        aDggrid = convert_dggrid_mesh_to_pyflowline_mesh(sFilename_cell, sFilename_mesh,
+                                                          iFlag_global_in = iFlag_global)
         
     return aDggrid
 
 if __name__ == '__main__':
 
 
     sRegion = 'conus'
```

### Comparing `pyflowline-0.3.4/pyflowline/mesh/hexagon/create_hexagon_mesh.py` & `pyflowline-0.3.5/pyflowline/mesh/hexagon/create_hexagon_mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #because it is mesh, it represent the edge instead of center
 #we will use gdal api for most operations
 import os
 import numpy as np
 from osgeo import ogr, osr
 from pyflowline.formats.convert_coordinates import convert_gcs_coordinates_to_cell
 from pyflowline.algorithms.auxiliary.find_index_in_list import check_if_duplicates
-from pyflowline.external.pyearth.gis.gdal.gdal_functions import reproject_coordinates_batch
+from pyearth.gis.spatialref.reproject_coodinates import reproject_coordinates_batch
 
 def index_to_row_col(index, num_columns):
     index -= 1  # Adjust for 1-based indexing
     row = index // num_columns + 1
     col = index % num_columns + 1
     return row, col
 
@@ -152,18 +152,15 @@
                     aNeighbor.append(lCellID5)
                    
         if iColumn > 1:#6
             iRow_dummy = iRow 
             iColumn_dummy = iColumn - 1
             lCellID6 = (iRow_dummy-1) * ncolumn_in + iColumn_dummy
             aNeighbor.append(lCellID6)
-
-        if check_if_duplicates(aNeighbor) == 0:
-            print('error')  
-
+      
         pHexagon.aNeighbor = aNeighbor
         pHexagon.nNeighbor = len(aNeighbor)
         pHexagon.aNeighbor_land= aNeighbor
         pHexagon.nNeighbor_land= pHexagon.nNeighbor
         aList.append(pHexagon)  
         return aList, dArea
 
@@ -231,19 +228,15 @@
                 lCellID5 = (iRow_dummy-1) * ncolumn_in + iColumn_dummy
                 aNeighbor.append(lCellID5)
                 if iRow!=1:
                     iRow_dummy = iRow - 1 
                     iColumn_dummy = iColumn - 1
                     lCellID6 = (iRow_dummy-1) * ncolumn_in + iColumn_dummy
                     aNeighbor.append(lCellID6)
-        
-        
-        if check_if_duplicates(aNeighbor) == 0:
-            print('error')  
-
+         
         pHexagon.aNeighbor = aNeighbor
         pHexagon.nNeighbor = len(aNeighbor)
         pHexagon.aNeighbor_land= aNeighbor
         pHexagon.nNeighbor_land= pHexagon.nNeighbor
         aList.append(pHexagon)
         return aList, dArea
 
@@ -433,20 +426,18 @@
                     pass
        
         
     #maybe rebuild topology?
     iFlag_fill_hole = 0    
     aHexagon_out = list()
 
-    if iFlag_fill_hole ==1:
-       
+    if iFlag_fill_hole ==1:       
         #find the virtual neighbors
         for pCell in aHexagon:            
             aNeighbor_land = pCell.aNeighbor_land   #including both holes and maps land cutoff by boundary
-            nNeighbor_land = pCell.nNeighbor
             aNeighbor_land_update = list()
             aNeighbor_land_virtual = list()
             nNeighbor_land_update = 0 
             for lNeighbor in aNeighbor_land: #loop all land neighbors               
                 if lNeighbor in aHexagon_dict:
                     nNeighbor_land_update = nNeighbor_land_update + 1 
                     aNeighbor_land_update.append(lNeighbor)
```

### Comparing `pyflowline-0.3.4/pyflowline/mesh/latlon/create_latlon_mesh.py` & `pyflowline-0.3.5/pyflowline/mesh/latlon/create_latlon_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/pyflowline/mesh/mpas/create_mpas_mesh.py` & `pyflowline-0.3.5/pyflowline/mesh/mpas/create_mpas_mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 import math
-import importlib
+import importlib.util
 import numpy as np
 from osgeo import ogr, osr, gdal
 from pyflowline.formats.convert_attributes import convert_gcs_attributes_to_cell
 gdal.UseExceptions()  
 iFlag_cython = importlib.util.find_spec("cython") 
 if iFlag_cython is not None:
     from pyflowline.algorithms.cython.kernel import convert_360_to_180
 else:
-    from pyflowline.external.pyearth.gis.gdal.gdal_functions import convert_360_to_180
+    from pyearth.gis.geometry.convert_longitude_range import convert_360_to_180
 
 def create_mpas_mesh(iFlag_global_in, 
     iFlag_use_mesh_dem, 
     iFlag_save_mesh_in,     
     sFilename_mesh_netcdf_in, 
     sFilename_output_in,
     iFlag_antarctic_in=None,
@@ -324,17 +324,15 @@
                         pFeature.SetField("elevation_mean", dElevation_mean )
                         pFeature.SetField("elevation_profile0", dElevation_profile0 )
 
                     pLayer.CreateFeature(pFeature)
             
     else:
         iFlag_remove_ice = 1
-        for i in range(ncell):
-            #center
-                  
+        for i in range(ncell):           
             #vertex
             aVertexOnCellIndex = np.array(aVertexOnCell[i,:])
             dummy0 = np.where(aVertexOnCellIndex > 0)
             aVertexIndex = aVertexOnCellIndex[dummy0]
             aLonVertex = aLongitudeVertex[aVertexIndex-1]
             aLatVertex = aLatitudeVertex[aVertexIndex-1]
             nVertex = len(aLonVertex)
@@ -417,16 +415,15 @@
     if iFlag_global_in == 1:
         aMpas_out = aMpas
     else:
         iFlag_fill_hole = 0        
         aMpas_out = list()
         ncell = len(aMpas)
         #generate the list of cell ID that are already certain        
-        if iFlag_fill_hole == 1:  
-            
+        if iFlag_fill_hole == 1:              
             #first update neighbor information because some cell should have vitual land neighbor (not present in the mesh)
             #this operation does not increase the number of cells, but it update the neighbor information
             #specifically, it divided the land neighbor into two parts: land and virtual land         
             for pCell in aMpas:               
                 aNeighbor_land = pCell.aNeighbor_land   #including both holes and maps land cutoff by boundary
                 aNeighbor_land_update = list()
                 aNeighbor_land_virtual = list()
```

### Comparing `pyflowline-0.3.4/pyflowline/mesh/square/create_square_mesh.py` & `pyflowline-0.3.5/pyflowline/mesh/square/create_square_mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #longitude left and latitude bottom and nrow and ncolumn and resolution is used to define the rectangle
 #because it is mesh, it represent the edge instead of center
 #we will use gdal api for most operations
 import os
 from osgeo import ogr, osr
 import numpy as np
 from pyflowline.formats.convert_coordinates import convert_gcs_coordinates_to_cell
-from pyflowline.external.pyearth.gis.gdal.gdal_functions import  reproject_coordinates_batch
+from pyearth.gis.spatialref.reproject_coodinates import  reproject_coordinates_batch
 
 def index_to_row_col(index, num_columns):
     index -= 1  # Adjust for 1-based indexing
     row = index // num_columns + 1
     col = index % num_columns + 1
     return row, col
```

### Comparing `pyflowline-0.3.4/pyflowline/mesh/tin/create_tin_mesh.py` & `pyflowline-0.3.5/pyflowline/mesh/tin/create_tin_mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import numpy as np
 from osgeo import ogr, osr
 from pyflowline.formats.convert_coordinates import convert_gcs_coordinates_to_cell
-from pyflowline.external.pyearth.gis.gdal.gdal_functions import reproject_coordinates_batch
+from pyearth.gis.spatialref.reproject_coodinates import reproject_coordinates_batch
 
 def create_tin_mesh(dX_left_in, dY_bot_in, 
                     dResolution_meter_in, 
                     ncolumn_in, nrow_in, 
 sFilename_output_in, 
 sFilename_spatial_reference_in, 
 pBoundary_in):
```

### Comparing `pyflowline-0.3.4/pyflowline/pyflowline_create_template_configuration_file.py` & `pyflowline-0.3.5/pyflowline/pyflowline_create_template_configuration_file.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.4/pyflowline/pyflowline_read_model_configuration_file.py` & `pyflowline-0.3.5/pyflowline/pyflowline_read_model_configuration_file.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-import os 
+import os
 from pathlib import Path
 import datetime
 import json
 from pyflowline.classes.pycase import flowlinecase
 pDate = datetime.datetime.today()
-sDate_default = "{:04d}".format(pDate.year) + "{:02d}".format(pDate.month) + "{:02d}".format(pDate.day)
+sDate_default = "{:04d}".format(
+    pDate.year) + "{:02d}".format(pDate.month) + "{:02d}".format(pDate.day)
 
-def pyflowline_read_model_configuration_file(sFilename_configuration_in,   
-    iFlag_standalone_in= None, 
-        iFlag_use_mesh_dem_in=None, 
-        iCase_index_in=None,   
-            dResolution_degree_in = None,  
-            dResolution_meter_in = None,  
-                sMesh_type_in = None,  
-                sModel_in = None, 
-                    sDate_in = None,
-                    sWorkspace_output_in = None):
+
+def pyflowline_read_model_configuration_file(sFilename_configuration_in,
+                                             iFlag_standalone_in=None,
+                                             iFlag_use_mesh_dem_in=None,
+                                             iCase_index_in=None,
+                                             iResolution_index_in = None,
+                                             dResolution_degree_in=None,
+                                             dResolution_meter_in=None,
+                                             sMesh_type_in=None,
+                                             sModel_in=None,
+                                             sDate_in=None,
+                                              sDggrid_type_in = None,
+                                             sWorkspace_output_in=None):
     """read a model configuration
 
     Args:
         sFilename_configuration_in (str): _description_
         iFlag_standalone_in (int, optional): _description_. Defaults to None.
         iFlag_use_mesh_dem_in (int, optional): _description_. Defaults to None.
         iCase_index_in (int, optional): _description_. Defaults to None.
@@ -33,40 +37,58 @@
     Returns:
         _type_: _description_
     """
 
     if not os.path.isfile(sFilename_configuration_in):
         print(sFilename_configuration_in + ' does not exist')
         return
-    
+
     # Opening JSON file
     with open(sFilename_configuration_in) as json_file:
-        aConfig = json.load(json_file)   
-    
-    if iCase_index_in is not None:        
+        aConfig = json.load(json_file)
+
+    if iCase_index_in is not None:
         iCase_index = iCase_index_in
-    else:       
-        iCase_index = int( aConfig['iCase_index'])
+    else:
+        iCase_index = int(aConfig['iCase_index'])
     
-    if iFlag_standalone_in is not None:        
+    if iResolution_index_in is not None:    
+        iResolution_index = iResolution_index_in
+    else:
+        if "iResolution_index" in aConfig:            
+            iResolution_index =  int( aConfig['iResolution_index'])
+        else:
+            iResolution_index = 10
+      
+        pass
+
+    if iFlag_standalone_in is not None:
         iFlag_standalone = iFlag_standalone_in
-    else:       
-        iFlag_standalone = int( aConfig['iFlag_standalone'])
+    else:
+        iFlag_standalone = int(aConfig['iFlag_standalone'])
 
-    if iFlag_use_mesh_dem_in is not None:        
+    if iFlag_use_mesh_dem_in is not None:
         iFlag_use_mesh_dem = iFlag_use_mesh_dem_in
-    else:       
+    else:
         iFlag_use_mesh_dem = int(aConfig['iFlag_use_mesh_dem'])
 
     if sMesh_type_in is not None:
         sMesh_type = sMesh_type_in
     else:
         sMesh_type = aConfig['sMesh_type']
         pass
-        
+
+    if sDggrid_type_in is not None:
+        sDggrid_type = sDggrid_type_in
+    else:
+        if "sDggrid_type" in aConfig:            
+            sDggrid_type = aConfig["sDggrid_type"]
+        else:
+            sDggrid_type = 'ISEA3H'
+
     if sModel_in is not None:
         sModel = sModel_in
     else:
         sModel = aConfig['sModel']
         pass
 
     if sDate_in is not None:
@@ -87,47 +109,42 @@
         dResolution_meter = aConfig['dResolution_meter']
         pass
 
     if sWorkspace_output_in is not None:
         sWorkspace_output = sWorkspace_output_in
     else:
         sWorkspace_output = aConfig['sWorkspace_output']
-        #try to create this output folder first using 
-    
+        # try to create this output folder first using
+
     try:
         print(sWorkspace_output)
         Path(sWorkspace_output).mkdir(parents=True, exist_ok=True)
     except ValueError:
         print("The specified output workspace cannot be created!")
         exit
-    
 
-    
     aConfig['iCase_index'] = iCase_index
     aConfig['iFlag_standalone'] = iFlag_standalone
     aConfig['iFlag_use_mesh_dem'] = iFlag_use_mesh_dem
+    aConfig["iResolution_index"] = iResolution_index
     aConfig['dResolution_degree'] = dResolution_degree
     aConfig['dResolution_meter'] = dResolution_meter
 
     aConfig['sDate'] = sDate
     aConfig['sModel'] = sModel
     aConfig['sMesh_type'] = sMesh_type
+    aConfig["sDggrid_type"] = sDggrid_type
     aConfig['sWorkspace_output'] = sWorkspace_output
 
     aConfig["sFilename_model_configuration"] = sFilename_configuration_in
-   
-    
 
-    #based on global variable, a few variables are calculate once
-    #calculate the modflow simulation period
-    #https://docs.python.org/3/library/datetime.html#datetime-objects
-   
-   
-    
-    #aConfig
-    
-    #simulation
-    
+    # based on global variable, a few variables are calculate once
+    # calculate the modflow simulation period
+    # https://docs.python.org/3/library/datetime.html#datetime-objects
+
+    # aConfig
+
+    # simulation
+
     oPyflowline = flowlinecase(aConfig)
-   
-    
-    return oPyflowline
+
+    return oPyflowline
```

### Comparing `pyflowline-0.3.4/pyflowline.egg-info/PKG-INFO` & `pyflowline-0.3.5/pyflowline.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflowline
-Version: 0.3.4
+Version: 0.3.5
 Summary: A mesh-independent river network generator for hydrologic models
 Home-page: https://github.com/changliao1025/pyflowline
 Author: Chang Liao
 Author-email: chang.liao@pnnl.gov
 License: custom
 Keywords: Earth Science
 Classifier: Development Status :: 4 - Beta
@@ -28,14 +28,15 @@
 Requires-Dist: matplotlib; extra == "visualization"
 Requires-Dist: cartopy>=0.21.0; extra == "visualization"
 Requires-Dist: simplekml; extra == "visualization"
 
 
 ### PyFlowline
 
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05446/status.svg)](https://doi.org/10.21105/joss.05446)
 [![DOI](https://zenodo.org/badge/368338554.svg)](https://zenodo.org/badge/latestdoi/368338554)
 [![Downloads](https://static.pepy.tech/badge/pyflowline)](https://pepy.tech/project/pyflowline)
 
 PyFlowline: a mesh-independent river network generator for hydrologic models.  
 
 ### Quickstart
 
@@ -106,11 +107,13 @@
 
 2. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL BATTELLE OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 ### References
 
 Several publications describe the algorithms used in `PyFlowline` in detail. If you make use of `PyFlowline` in your work, please consider including a reference to the following:
 
+* Liao et al., (2023). pyflowline: a mesh-independent river network generator for hydrologic models. Journal of Open Source Software, 8(91), 5446, https://doi.org/10.21105/joss.05446
+
 * Liao. C. Cooper, M (2022) Pyflowline: a mesh-independent river network generator for hydrologic models. Zenodo.
 https://doi.org/10.5281/zenodo.6407298
 
 * Liao, C., Zhou, T., Xu, D., Cooper, M. G., Engwirda, D., Li, H.-Y., & Leung, L. R. (2023). Topological relationship-based flow direction modeling: Mesh-independent river networks representation. Journal of Advances in Modeling Earth Systems, 15, e2022MS003089. https://doi.org/10.1029/2022MS003089
```

### Comparing `pyflowline-0.3.4/pyflowline.egg-info/SOURCES.txt` & `pyflowline-0.3.5/pyflowline.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,14 @@
 pyflowline.egg-info/top_level.txt
 pyflowline/algorithms/__init__.py
 pyflowline/algorithms/auxiliary/__init__.py
 pyflowline/algorithms/auxiliary/calculate_area_of_difference.py
 pyflowline/algorithms/auxiliary/check_head_water.py
 pyflowline/algorithms/auxiliary/find_index_in_list.py
 pyflowline/algorithms/auxiliary/find_vertex_in_list.py
-pyflowline/algorithms/auxiliary/longlat_to_3d.py
 pyflowline/algorithms/connection/__init__.py
 pyflowline/algorithms/connection/connect_disconnect_flowline.py
 pyflowline/algorithms/cython/__init__.py
 pyflowline/algorithms/cython/setup.py
 pyflowline/algorithms/direction/__init__.py
 pyflowline/algorithms/direction/correct_flowline_direction.py
 pyflowline/algorithms/index/__init__.py
```

### Comparing `pyflowline-0.3.4/setup.py` & `pyflowline-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 NAME = "pyflowline"
 DESCRIPTION = \
     "A mesh-independent river network generator for hydrologic models"
 AUTHOR = "Chang Liao"
 AUTHOR_EMAIL = "chang.liao@pnnl.gov"
 URL = "https://github.com/changliao1025/pyflowline"
-VERSION = "0.3.4"
+VERSION = "0.3.5"
 REQUIRES_PYTHON = ">=3.8.0"
 KEYWORDS = "Earth Science"
 
 REQUIRED = [
     "numpy", 
     "gdal",
     "netCDF4"
```

