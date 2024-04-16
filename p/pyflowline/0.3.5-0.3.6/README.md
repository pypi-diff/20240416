# Comparing `tmp/pyflowline-0.3.5.tar.gz` & `tmp/pyflowline-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflowline-0.3.5.tar", last modified: Tue Apr 16 15:38:05 2024, max compression
+gzip compressed data, was "pyflowline-0.3.6.tar", last modified: Tue Apr 16 16:04:36 2024, max compression
```

## Comparing `pyflowline-0.3.5.tar` & `pyflowline-0.3.6.tar`

### file list

```diff
@@ -1,175 +1,175 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.549494 pyflowline-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-16 15:37:59.000000 pyflowline-0.3.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-16 15:37:59.000000 pyflowline-0.3.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-16 15:37:59.000000 pyflowline-0.3.5/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-16 15:37:59.000000 pyflowline-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-16 15:37:59.000000 pyflowline-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-16 15:38:05.549494 pyflowline-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-16 15:37:59.000000 pyflowline-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.517494 pyflowline-0.3.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.529494 pyflowline-0.3.5/docs/figures/
--rw-r--r--   0 runner    (1001) docker     (127)    67244 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/after_loop.png
--rw-r--r--   0 runner    (1001) docker     (127)    64320 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/after_merge.png
--rw-r--r--   0 runner    (1001) docker     (127)    68901 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/basic_element.png
--rw-r--r--   0 runner    (1001) docker     (127)    76858 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/before_loop.png
--rw-r--r--   0 runner    (1001) docker     (127)    68959 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/before_merge.png
--rw-r--r--   0 runner    (1001) docker     (127)    16482 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/disconnect_flowline.png
--rw-r--r--   0 runner    (1001) docker     (127)   146717 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/find_vertex.png
--rw-r--r--   0 runner    (1001) docker     (127)    15195 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/flow_direction.png
--rw-r--r--   0 runner    (1001) docker     (127)   252712 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/flow_direction_matrix.png
--rw-r--r--   0 runner    (1001) docker     (127)   525380 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/hexagon.png
--rw-r--r--   0 runner    (1001) docker     (127)   628942 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/hexagon_intersect.png
--rw-r--r--   0 runner    (1001) docker     (127)   524174 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/lat_lon.png
--rw-r--r--   0 runner    (1001) docker     (127)   734342 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/lat_lon_intersect.png
--rw-r--r--   0 runner    (1001) docker     (127)    45168 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/merge_flowline.png
--rw-r--r--   0 runner    (1001) docker     (127)  1191889 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/meshes.png
--rw-r--r--   0 runner    (1001) docker     (127)    47724 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/remove_loop.png
--rw-r--r--   0 runner    (1001) docker     (127)   596253 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/remove_loop_matrix.png
--rw-r--r--   0 runner    (1001) docker     (127)    93563 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/simplification01.png
--rw-r--r--   0 runner    (1001) docker     (127)    21317 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/small_river.png
--rw-r--r--   0 runner    (1001) docker     (127)   148387 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/sqaure_intersect.png
--rw-r--r--   0 runner    (1001) docker     (127)    61180 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/square.png
--rw-r--r--   0 runner    (1001) docker     (127)    46783 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/structure_pyflowline.png
--rw-r--r--   0 runner    (1001) docker     (127)   160993 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/figures/workflow.png
--rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.533494 pyflowline-0.3.5/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.533494 pyflowline-0.3.5/docs/source/algorithm/
--rw-r--r--   0 runner    (1001) docker     (127)     7897 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/algorithm/algorithm.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.533494 pyflowline-0.3.5/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/api/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.533494 pyflowline-0.3.5/docs/source/application/
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/application/application.rst
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/contribution.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.533494 pyflowline-0.3.5/docs/source/data/
--rw-r--r--   0 runner    (1001) docker     (127)    29917 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/data/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.533494 pyflowline-0.3.5/docs/source/installation/
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/installation/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/references.rst
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/support.rst
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-16 15:37:59.000000 pyflowline-0.3.5/docs/source/visualization.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.533494 pyflowline-0.3.5/examples/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-16 15:37:59.000000 pyflowline-0.3.5/examples/create_model_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.533494 pyflowline-0.3.5/pyflowline/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.533494 pyflowline-0.3.5/pyflowline/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.533494 pyflowline-0.3.5/pyflowline/algorithms/auxiliary/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/auxiliary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16198 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/auxiliary/calculate_area_of_difference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/auxiliary/check_head_water.py
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/auxiliary/find_index_in_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/auxiliary/find_vertex_in_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.537494 pyflowline-0.3.5/pyflowline/algorithms/connection/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/connection/connect_disconnect_flowline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.537494 pyflowline-0.3.5/pyflowline/algorithms/cython/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/cython/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.537494 pyflowline-0.3.5/pyflowline/algorithms/direction/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/direction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/direction/correct_flowline_direction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.537494 pyflowline-0.3.5/pyflowline/algorithms/index/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/index/define_stream_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/index/define_stream_segment_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/index/define_stream_topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.537494 pyflowline-0.3.5/pyflowline/algorithms/intersect/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/intersect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/intersect/intersect_flowline_with_flowline.py
--rw-r--r--   0 runner    (1001) docker     (127)    15785 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/intersect/intersect_flowline_with_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/intersect/intersect_flowline_with_vertex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.537494 pyflowline-0.3.5/pyflowline/algorithms/loop/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/loop/remove_flowline_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.537494 pyflowline-0.3.5/pyflowline/algorithms/merge/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/merge/merge_flowline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.537494 pyflowline-0.3.5/pyflowline/algorithms/simplification/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/simplification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/simplification/remove_duplicate_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/simplification/remove_duplicate_flowline.py
--rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/simplification/remove_returning_flowline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/simplification/remove_small_river.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.541494 pyflowline-0.3.5/pyflowline/algorithms/split/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/split/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/split/find_flowline_confluence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/split/find_flowline_vertex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/split/split_by_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/split/split_flowline.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/algorithms/split/split_flowline_to_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/change_json_key_value.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.545494 pyflowline-0.3.5/pyflowline/classes/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/_hpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/_visual.py
--rw-r--r--   0 runner    (1001) docker     (127)    24307 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/_visual_basin.py
--rw-r--r--   0 runner    (1001) docker     (127)    62019 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/basin.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/confluence.py
--rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/dggrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/flowline.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/hexagon.py
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/latlon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/link.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/mpas.py
--rw-r--r--   0 runner    (1001) docker     (127)    59119 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/pycase.py
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/square.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/tin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/classes/vertex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.545494 pyflowline-0.3.5/pyflowline/formats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/formats/convert_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/formats/convert_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/formats/convert_flowline_to_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/formats/export_flowline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/formats/export_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/formats/export_vertex.py
--rw-r--r--   0 runner    (1001) docker     (127)    11769 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/formats/read_flowline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/formats/read_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/formats/read_nhdplus_flowline_shapefile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.545494 pyflowline-0.3.5/pyflowline/mesh/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.545494 pyflowline-0.3.5/pyflowline/mesh/dggrid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/dggrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/dggrid/create_dggrid_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.545494 pyflowline-0.3.5/pyflowline/mesh/hexagon/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/hexagon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28451 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/hexagon/create_hexagon_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.545494 pyflowline-0.3.5/pyflowline/mesh/latlon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/latlon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/latlon/create_latlon_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.545494 pyflowline-0.3.5/pyflowline/mesh/mpas/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/mpas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23224 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/mpas/create_mpas_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.545494 pyflowline-0.3.5/pyflowline/mesh/square/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/square/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15367 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/square/create_square_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.545494 pyflowline-0.3.5/pyflowline/mesh/tin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/tin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/mesh/tin/create_tin_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/pyflowline_create_template_configuration_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyflowline/pyflowline_read_model_configuration_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.549494 pyflowline-0.3.5/pyflowline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-16 15:38:05.000000 pyflowline-0.3.5/pyflowline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-16 15:38:05.000000 pyflowline-0.3.5/pyflowline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:38:05.000000 pyflowline-0.3.5/pyflowline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-16 15:38:05.000000 pyflowline-0.3.5/pyflowline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 15:38:05.000000 pyflowline-0.3.5/pyflowline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-16 15:37:59.000000 pyflowline-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-16 15:38:05.549494 pyflowline-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-16 15:37:59.000000 pyflowline-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:38:05.549494 pyflowline-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-16 15:37:59.000000 pyflowline-0.3.5/tests/test_installation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.499727 pyflowline-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-16 16:04:31.000000 pyflowline-0.3.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-16 16:04:31.000000 pyflowline-0.3.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-16 16:04:31.000000 pyflowline-0.3.6/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-16 16:04:31.000000 pyflowline-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-16 16:04:31.000000 pyflowline-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-16 16:04:36.499727 pyflowline-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-16 16:04:31.000000 pyflowline-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.471726 pyflowline-0.3.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.483726 pyflowline-0.3.6/docs/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)    67244 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/figures/after_loop.png
+-rw-r--r--   0 runner    (1001) docker     (127)    64320 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/figures/after_merge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68901 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/figures/basic_element.png
+-rw-r--r--   0 runner    (1001) docker     (127)    76858 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/figures/before_loop.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68959 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/figures/before_merge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16482 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/figures/disconnect_flowline.png
+-rw-r--r--   0 runner    (1001) docker     (127)   146717 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/figures/find_vertex.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15195 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/figures/flow_direction.png
+-rw-r--r--   0 runner    (1001) docker     (127)   252712 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/figures/flow_direction_matrix.png
+-rw-r--r--   0 runner    (1001) docker     (127)   525380 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/figures/hexagon.png
+-rw-r--r--   0 runner    (1001) docker     (127)   628942 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/figures/hexagon_intersect.png
+-rw-r--r--   0 runner    (1001) docker     (127)   524174 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/figures/lat_lon.png
+-rw-r--r--   0 runner    (1001) docker     (127)   734342 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/figures/lat_lon_intersect.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45168 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/figures/merge_flowline.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1191889 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/figures/meshes.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47724 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/figures/remove_loop.png
+-rw-r--r--   0 runner    (1001) docker     (127)   596253 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/figures/remove_loop_matrix.png
+-rw-r--r--   0 runner    (1001) docker     (127)    93563 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/figures/simplification01.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21317 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/figures/small_river.png
+-rw-r--r--   0 runner    (1001) docker     (127)   148387 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/figures/sqaure_intersect.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61180 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/figures/square.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46783 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/figures/structure_pyflowline.png
+-rw-r--r--   0 runner    (1001) docker     (127)   160993 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/figures/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.483726 pyflowline-0.3.6/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.483726 pyflowline-0.3.6/docs/source/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (127)     7897 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/source/algorithm/algorithm.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.483726 pyflowline-0.3.6/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/source/api/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.483726 pyflowline-0.3.6/docs/source/application/
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/source/application/application.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/source/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/source/contribution.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.483726 pyflowline-0.3.6/docs/source/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    29917 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/source/data/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/source/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/source/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.483726 pyflowline-0.3.6/docs/source/installation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/source/installation/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/source/references.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/source/support.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-16 16:04:31.000000 pyflowline-0.3.6/docs/source/visualization.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.483726 pyflowline-0.3.6/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:31.000000 pyflowline-0.3.6/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-16 16:04:31.000000 pyflowline-0.3.6/examples/create_model_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.487727 pyflowline-0.3.6/pyflowline/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.487727 pyflowline-0.3.6/pyflowline/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.487727 pyflowline-0.3.6/pyflowline/algorithms/auxiliary/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/auxiliary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16311 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/auxiliary/calculate_area_of_difference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/auxiliary/check_head_water.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/auxiliary/find_index_in_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/auxiliary/find_vertex_in_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.487727 pyflowline-0.3.6/pyflowline/algorithms/connection/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/connection/connect_disconnect_flowline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.487727 pyflowline-0.3.6/pyflowline/algorithms/cython/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/cython/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.487727 pyflowline-0.3.6/pyflowline/algorithms/direction/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/direction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/direction/correct_flowline_direction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.487727 pyflowline-0.3.6/pyflowline/algorithms/index/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/index/define_stream_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/index/define_stream_segment_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/index/define_stream_topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.491726 pyflowline-0.3.6/pyflowline/algorithms/intersect/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/intersect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/intersect/intersect_flowline_with_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15785 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/intersect/intersect_flowline_with_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/intersect/intersect_flowline_with_vertex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.491726 pyflowline-0.3.6/pyflowline/algorithms/loop/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/loop/remove_flowline_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.491726 pyflowline-0.3.6/pyflowline/algorithms/merge/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/merge/merge_flowline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.491726 pyflowline-0.3.6/pyflowline/algorithms/simplification/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/simplification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/simplification/remove_duplicate_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/simplification/remove_duplicate_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/simplification/remove_returning_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/simplification/remove_small_river.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.491726 pyflowline-0.3.6/pyflowline/algorithms/split/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/split/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/split/find_flowline_confluence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/split/find_flowline_vertex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/split/split_by_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/split/split_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/algorithms/split/split_flowline_to_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/change_json_key_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.495727 pyflowline-0.3.6/pyflowline/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/classes/_hpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/classes/_visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24307 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/classes/_visual_basin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62019 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/classes/basin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/classes/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/classes/confluence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/classes/dggrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/classes/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/classes/flowline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/classes/hexagon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/classes/latlon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/classes/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/classes/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/classes/mpas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59119 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/classes/pycase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/classes/square.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/classes/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/classes/tin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/classes/vertex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.495727 pyflowline-0.3.6/pyflowline/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/formats/convert_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/formats/convert_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/formats/convert_flowline_to_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/formats/export_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/formats/export_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/formats/export_vertex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11769 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/formats/read_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/formats/read_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/formats/read_nhdplus_flowline_shapefile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.495727 pyflowline-0.3.6/pyflowline/mesh/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/mesh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.495727 pyflowline-0.3.6/pyflowline/mesh/dggrid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/mesh/dggrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/mesh/dggrid/create_dggrid_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.499727 pyflowline-0.3.6/pyflowline/mesh/hexagon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/mesh/hexagon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28451 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/mesh/hexagon/create_hexagon_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.499727 pyflowline-0.3.6/pyflowline/mesh/latlon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/mesh/latlon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/mesh/latlon/create_latlon_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.499727 pyflowline-0.3.6/pyflowline/mesh/mpas/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/mesh/mpas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23224 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/mesh/mpas/create_mpas_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.499727 pyflowline-0.3.6/pyflowline/mesh/square/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/mesh/square/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15367 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/mesh/square/create_square_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.499727 pyflowline-0.3.6/pyflowline/mesh/tin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/mesh/tin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/mesh/tin/create_tin_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/pyflowline_create_template_configuration_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyflowline/pyflowline_read_model_configuration_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.499727 pyflowline-0.3.6/pyflowline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-16 16:04:36.000000 pyflowline-0.3.6/pyflowline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-16 16:04:36.000000 pyflowline-0.3.6/pyflowline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 16:04:36.000000 pyflowline-0.3.6/pyflowline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-16 16:04:36.000000 pyflowline-0.3.6/pyflowline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 16:04:36.000000 pyflowline-0.3.6/pyflowline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-16 16:04:31.000000 pyflowline-0.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-16 16:04:36.499727 pyflowline-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-16 16:04:31.000000 pyflowline-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:04:36.499727 pyflowline-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-16 16:04:31.000000 pyflowline-0.3.6/tests/test_installation.py
```

### Comparing `pyflowline-0.3.5/CONTRIBUTING.rst` & `pyflowline-0.3.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/LICENSE` & `pyflowline-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/PKG-INFO` & `pyflowline-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflowline
-Version: 0.3.5
+Version: 0.3.6
 Summary: A mesh-independent river network generator for hydrologic models
 Home-page: https://github.com/changliao1025/pyflowline
 Author: Chang Liao
 Author-email: chang.liao@pnnl.gov
 License: custom
 Keywords: Earth Science
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyflowline-0.3.5/README.md` & `pyflowline-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/Makefile` & `pyflowline-0.3.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/figures/after_loop.png` & `pyflowline-0.3.6/docs/figures/after_loop.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/figures/after_merge.png` & `pyflowline-0.3.6/docs/figures/after_merge.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/figures/basic_element.png` & `pyflowline-0.3.6/docs/figures/basic_element.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/figures/before_loop.png` & `pyflowline-0.3.6/docs/figures/before_loop.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/figures/before_merge.png` & `pyflowline-0.3.6/docs/figures/before_merge.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/figures/disconnect_flowline.png` & `pyflowline-0.3.6/docs/figures/disconnect_flowline.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/figures/find_vertex.png` & `pyflowline-0.3.6/docs/figures/find_vertex.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/figures/flow_direction.png` & `pyflowline-0.3.6/docs/figures/flow_direction.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/figures/flow_direction_matrix.png` & `pyflowline-0.3.6/docs/figures/flow_direction_matrix.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/figures/hexagon.png` & `pyflowline-0.3.6/docs/figures/hexagon.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/figures/hexagon_intersect.png` & `pyflowline-0.3.6/docs/figures/hexagon_intersect.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/figures/lat_lon.png` & `pyflowline-0.3.6/docs/figures/lat_lon.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/figures/lat_lon_intersect.png` & `pyflowline-0.3.6/docs/figures/lat_lon_intersect.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/figures/merge_flowline.png` & `pyflowline-0.3.6/docs/figures/merge_flowline.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/figures/meshes.png` & `pyflowline-0.3.6/docs/figures/meshes.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/figures/remove_loop.png` & `pyflowline-0.3.6/docs/figures/remove_loop.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/figures/remove_loop_matrix.png` & `pyflowline-0.3.6/docs/figures/remove_loop_matrix.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/figures/simplification01.png` & `pyflowline-0.3.6/docs/figures/simplification01.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/figures/small_river.png` & `pyflowline-0.3.6/docs/figures/small_river.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/figures/sqaure_intersect.png` & `pyflowline-0.3.6/docs/figures/sqaure_intersect.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/figures/square.png` & `pyflowline-0.3.6/docs/figures/square.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/figures/structure_pyflowline.png` & `pyflowline-0.3.6/docs/figures/structure_pyflowline.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/figures/workflow.png` & `pyflowline-0.3.6/docs/figures/workflow.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/make.bat` & `pyflowline-0.3.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/source/algorithm/algorithm.rst` & `pyflowline-0.3.6/docs/source/algorithm/algorithm.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/source/api/api.rst` & `pyflowline-0.3.6/docs/source/api/api.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/source/application/application.rst` & `pyflowline-0.3.6/docs/source/application/application.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/source/conf.py` & `pyflowline-0.3.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/source/data/data.rst` & `pyflowline-0.3.6/docs/source/data/data.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/source/faq.rst` & `pyflowline-0.3.6/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/source/glossary.rst` & `pyflowline-0.3.6/docs/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/source/index.rst` & `pyflowline-0.3.6/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/source/installation/installation.rst` & `pyflowline-0.3.6/docs/source/installation/installation.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/source/quickstart.rst` & `pyflowline-0.3.6/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/docs/source/readme.rst` & `pyflowline-0.3.6/docs/source/readme.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/examples/create_model_configuration.py` & `pyflowline-0.3.6/examples/create_model_configuration.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/algorithms/auxiliary/calculate_area_of_difference.py` & `pyflowline-0.3.6/pyflowline/algorithms/auxiliary/calculate_area_of_difference.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import numpy as np
 from osgeo import ogr, osr
 import importlib.util
 
 from pyflowline.algorithms.auxiliary.find_index_in_list import find_list_in_list 
 
 from pyearth.gis.geometry.calculate_polygon_area import calculate_polygon_area
+from pyearth.gis.geometry.calculate_angle_between_vertex_normal import calculate_angle_between_vertex_normal
 
 iFlag_cython = importlib.util.find_spec("cython") 
 if iFlag_cython is not None:
     from pyflowline.algorithms.cython.kernel import find_vertex_in_list
 else:
     from pyflowline.algorithms.auxiliary.find_vertex_in_list import find_vertex_in_list
 
@@ -103,15 +104,15 @@
                         nEdge2 = pFlowline_dummy.nEdge
                         pEdge2 = pFlowline_dummy.aEdge[nEdge2-1]
                         pVertex_dummy = pEdge2.pVertex_start
 
                     #calculate angle              
                     x3 = pVertex_dummy.dLongitude_degree
                     y3 = pVertex_dummy.dLatitude_degree
-                    angle_dummy = calculate_angle_betwen_vertex_normal( x1, y1, x2, y2, x3, y3  )                    
+                    angle_dummy = calculate_angle_between_vertex_normal( x1, y1, x2, y2, x3, y3  )                    
                     aAngle.append(angle_dummy)
                 for i in pFlowline_in.aFlowlineID_end_end:
                     pFlowline_dummy = aFlowline_in[i]
                     if (pFlowline_dummy.pVertex_start == pVertex_stop):
                         nEdge2 = pFlowline_dummy.nEdge
                         pEdge2 = pFlowline_dummy.aEdge[0]
                         pVertex_dummy = pEdge2.pVertex_end
@@ -119,15 +120,15 @@
                         nEdge2 = pFlowline_dummy.nEdge
                         pEdge2 = pFlowline_dummy.aEdge[nEdge2-1]
                         pVertex_dummy = pEdge2.pVertex_start
 
                     #calculate angle              
                     x3 = pVertex_dummy.dLongitude_degree
                     y3 = pVertex_dummy.dLatitude_degree
-                    angle_dummy = calculate_angle_betwen_vertex_normal( x1, y1, x2, y2, x3, y3  )                    
+                    angle_dummy = calculate_angle_between_vertex_normal( x1, y1, x2, y2, x3, y3  )                    
                     aAngle.append(angle_dummy)
                   
                 #mini
                 dummy = pFlowline_in.aFlowlineID_end_start + pFlowline_in.aFlowlineID_end_end
                 if iFlag_rightleft ==0 :
                     min_angle = min(aAngle)
                     iIndex_right = aAngle.index(min_angle)                   
@@ -177,30 +178,30 @@
                     else:
                         nEdge2 = pFlowline_dummy.nEdge
                         pEdge2 = pFlowline_dummy.aEdge[nEdge2-1]
                         pVertex_dummy = pEdge2.pVertex_start
 
                     x3 = pVertex_dummy.dLongitude_degree
                     y3 = pVertex_dummy.dLatitude_degree
-                    angle_dummy = calculate_angle_betwen_vertex_normal( x1, y1, x2, y2, x3, y3  )
+                    angle_dummy = calculate_angle_between_vertex_normal( x1, y1, x2, y2, x3, y3  )
                     aAngle.append(angle_dummy)
                 for i in pFlowline_in.aFlowlineID_start_end:
                     pFlowline_dummy = aFlowline_in[i]
                     if (pFlowline_dummy.pVertex_start == pVertex_stop):
                         nEdge2 = pFlowline_dummy.nEdge
                         pEdge2 = pFlowline_dummy.aEdge[0]
                         pVertex_dummy = pEdge2.pVertex_end
                     else:
                         nEdge2 = pFlowline_dummy.nEdge
                         pEdge2 = pFlowline_dummy.aEdge[nEdge2-1]
                         pVertex_dummy = pEdge2.pVertex_start
 
                     x3 = pVertex_dummy.dLongitude_degree
                     y3 = pVertex_dummy.dLatitude_degree
-                    angle_dummy = calculate_angle_betwen_vertex_normal( x1, y1, x2, y2, x3, y3  )
+                    angle_dummy = calculate_angle_between_vertex_normal( x1, y1, x2, y2, x3, y3  )
                     aAngle.append(angle_dummy)
                     
                 #mini
                 dummy = pFlowline_in.aFlowlineID_start_start + pFlowline_in.aFlowlineID_start_end
                 if iFlag_rightleft ==0 :
                     min_angle = min(aAngle)
                     iIndex_right = aAngle.index(min_angle)
```

### Comparing `pyflowline-0.3.5/pyflowline/algorithms/auxiliary/check_head_water.py` & `pyflowline-0.3.6/pyflowline/algorithms/auxiliary/check_head_water.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/algorithms/auxiliary/find_index_in_list.py` & `pyflowline-0.3.6/pyflowline/algorithms/auxiliary/find_index_in_list.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/algorithms/auxiliary/find_vertex_in_list.py` & `pyflowline-0.3.6/pyflowline/algorithms/auxiliary/find_vertex_in_list.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/algorithms/connection/connect_disconnect_flowline.py` & `pyflowline-0.3.6/pyflowline/algorithms/connection/connect_disconnect_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/algorithms/direction/correct_flowline_direction.py` & `pyflowline-0.3.6/pyflowline/algorithms/direction/correct_flowline_direction.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/algorithms/index/define_stream_order.py` & `pyflowline-0.3.6/pyflowline/algorithms/index/define_stream_order.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/algorithms/index/define_stream_segment_index.py` & `pyflowline-0.3.6/pyflowline/algorithms/index/define_stream_segment_index.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/algorithms/index/define_stream_topology.py` & `pyflowline-0.3.6/pyflowline/algorithms/index/define_stream_topology.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/algorithms/intersect/intersect_flowline_with_flowline.py` & `pyflowline-0.3.6/pyflowline/algorithms/intersect/intersect_flowline_with_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/algorithms/intersect/intersect_flowline_with_mesh.py` & `pyflowline-0.3.6/pyflowline/algorithms/intersect/intersect_flowline_with_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/algorithms/intersect/intersect_flowline_with_vertex.py` & `pyflowline-0.3.6/pyflowline/algorithms/intersect/intersect_flowline_with_vertex.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/algorithms/loop/remove_flowline_loop.py` & `pyflowline-0.3.6/pyflowline/algorithms/loop/remove_flowline_loop.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/algorithms/merge/merge_flowline.py` & `pyflowline-0.3.6/pyflowline/algorithms/merge/merge_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/algorithms/simplification/remove_returning_flowline.py` & `pyflowline-0.3.6/pyflowline/algorithms/simplification/remove_returning_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/algorithms/simplification/remove_small_river.py` & `pyflowline-0.3.6/pyflowline/algorithms/simplification/remove_small_river.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/algorithms/split/find_flowline_confluence.py` & `pyflowline-0.3.6/pyflowline/algorithms/split/find_flowline_confluence.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/algorithms/split/find_flowline_vertex.py` & `pyflowline-0.3.6/pyflowline/algorithms/split/find_flowline_vertex.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/algorithms/split/split_by_length.py` & `pyflowline-0.3.6/pyflowline/algorithms/split/split_by_length.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/algorithms/split/split_flowline.py` & `pyflowline-0.3.6/pyflowline/algorithms/split/split_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/algorithms/split/split_flowline_to_edge.py` & `pyflowline-0.3.6/pyflowline/algorithms/split/split_flowline_to_edge.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/classes/_hpc.py` & `pyflowline-0.3.6/pyflowline/classes/_hpc.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/classes/_visual.py` & `pyflowline-0.3.6/pyflowline/classes/_visual.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/classes/_visual_basin.py` & `pyflowline-0.3.6/pyflowline/classes/_visual_basin.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/classes/basin.py` & `pyflowline-0.3.6/pyflowline/classes/basin.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/classes/confluence.py` & `pyflowline-0.3.6/pyflowline/classes/confluence.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/classes/dggrid.py` & `pyflowline-0.3.6/pyflowline/classes/dggrid.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/classes/edge.py` & `pyflowline-0.3.6/pyflowline/classes/edge.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/classes/flowline.py` & `pyflowline-0.3.6/pyflowline/classes/flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/classes/hexagon.py` & `pyflowline-0.3.6/pyflowline/classes/hexagon.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/classes/latlon.py` & `pyflowline-0.3.6/pyflowline/classes/latlon.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/classes/link.py` & `pyflowline-0.3.6/pyflowline/classes/link.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/classes/mpas.py` & `pyflowline-0.3.6/pyflowline/classes/mpas.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/classes/pycase.py` & `pyflowline-0.3.6/pyflowline/classes/pycase.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/classes/square.py` & `pyflowline-0.3.6/pyflowline/classes/square.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/classes/timer.py` & `pyflowline-0.3.6/pyflowline/classes/timer.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/classes/tin.py` & `pyflowline-0.3.6/pyflowline/classes/tin.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/classes/vertex.py` & `pyflowline-0.3.6/pyflowline/classes/vertex.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/formats/convert_attributes.py` & `pyflowline-0.3.6/pyflowline/formats/convert_attributes.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/formats/convert_coordinates.py` & `pyflowline-0.3.6/pyflowline/formats/convert_coordinates.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/formats/convert_flowline_to_geojson.py` & `pyflowline-0.3.6/pyflowline/formats/convert_flowline_to_geojson.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/formats/export_flowline.py` & `pyflowline-0.3.6/pyflowline/formats/export_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/formats/export_mesh.py` & `pyflowline-0.3.6/pyflowline/formats/export_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/formats/export_vertex.py` & `pyflowline-0.3.6/pyflowline/formats/export_vertex.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/formats/read_flowline.py` & `pyflowline-0.3.6/pyflowline/formats/read_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/formats/read_mesh.py` & `pyflowline-0.3.6/pyflowline/formats/read_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/formats/read_nhdplus_flowline_shapefile.py` & `pyflowline-0.3.6/pyflowline/formats/read_nhdplus_flowline_shapefile.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/mesh/dggrid/create_dggrid_mesh.py` & `pyflowline-0.3.6/pyflowline/mesh/dggrid/create_dggrid_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/mesh/hexagon/create_hexagon_mesh.py` & `pyflowline-0.3.6/pyflowline/mesh/hexagon/create_hexagon_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/mesh/latlon/create_latlon_mesh.py` & `pyflowline-0.3.6/pyflowline/mesh/latlon/create_latlon_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/mesh/mpas/create_mpas_mesh.py` & `pyflowline-0.3.6/pyflowline/mesh/mpas/create_mpas_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/mesh/square/create_square_mesh.py` & `pyflowline-0.3.6/pyflowline/mesh/square/create_square_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/mesh/tin/create_tin_mesh.py` & `pyflowline-0.3.6/pyflowline/mesh/tin/create_tin_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/pyflowline_create_template_configuration_file.py` & `pyflowline-0.3.6/pyflowline/pyflowline_create_template_configuration_file.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline/pyflowline_read_model_configuration_file.py` & `pyflowline-0.3.6/pyflowline/pyflowline_read_model_configuration_file.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/pyflowline.egg-info/PKG-INFO` & `pyflowline-0.3.6/pyflowline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflowline
-Version: 0.3.5
+Version: 0.3.6
 Summary: A mesh-independent river network generator for hydrologic models
 Home-page: https://github.com/changliao1025/pyflowline
 Author: Chang Liao
 Author-email: chang.liao@pnnl.gov
 License: custom
 Keywords: Earth Science
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyflowline-0.3.5/pyflowline.egg-info/SOURCES.txt` & `pyflowline-0.3.6/pyflowline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.5/setup.py` & `pyflowline-0.3.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 NAME = "pyflowline"
 DESCRIPTION = \
     "A mesh-independent river network generator for hydrologic models"
 AUTHOR = "Chang Liao"
 AUTHOR_EMAIL = "chang.liao@pnnl.gov"
 URL = "https://github.com/changliao1025/pyflowline"
-VERSION = "0.3.5"
+VERSION = "0.3.6"
 REQUIRES_PYTHON = ">=3.8.0"
 KEYWORDS = "Earth Science"
 
 REQUIRED = [
     "numpy", 
     "gdal",
     "netCDF4"
```

