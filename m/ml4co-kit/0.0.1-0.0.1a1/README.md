# Comparing `tmp/ml4co_kit-0.0.1.tar.gz` & `tmp/ml4co_kit-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml4co_kit-0.0.1.tar", last modified: Tue Apr 16 04:03:30 2024, max compression
+gzip compressed data, was "ml4co_kit-0.0.1a1.tar", last modified: Mon Apr 15 16:45:53 2024, max compression
```

## Comparing `ml4co_kit-0.0.1.tar` & `ml4co_kit-0.0.1a1.tar`

### file list

```diff
@@ -1,768 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.981783 ml4co_kit-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-04-16 04:03:30.981783 ml4co_kit-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.825784 ml4co_kit-0.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.845784 ml4co_kit-0.0.1/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/docs/assets/kroA150_problem.png
--rw-r--r--   0 runner    (1001) docker     (127)    34941 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/docs/assets/kroA150_solution.png
--rw-r--r--   0 runner    (1001) docker     (127)    87460 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/docs/assets/mis_problem.png
--rw-r--r--   0 runner    (1001) docker     (127)    87798 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/docs/assets/mis_solution.png
--rw-r--r--   0 runner    (1001) docker     (127)   180376 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/docs/assets/ml4co-kit-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)   171559 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/docs/assets/organization.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.845784 ml4co_kit-0.0.1/docs/project_example/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/docs/project_example/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/docs/project_example/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/docs/project_example/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/docs/project_example/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/docs/project_example/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.845784 ml4co_kit-0.0.1/ml4co_kit/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.845784 ml4co_kit-0.0.1/ml4co_kit/data/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.845784 ml4co_kit-0.0.1/ml4co_kit/data/mis/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/data/mis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/data/mis/satlib_original.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.845784 ml4co_kit-0.0.1/ml4co_kit/data/tsp/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/data/tsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/data/tsp/tsp_uniform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/data/tsp/tsplib_original.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.849784 ml4co_kit-0.0.1/ml4co_kit/draw/
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/draw/mis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/draw/tsp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/draw/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.849784 ml4co_kit-0.0.1/ml4co_kit/evaluate/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/evaluate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.849784 ml4co_kit-0.0.1/ml4co_kit/evaluate/mis/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/evaluate/mis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/evaluate/mis/satlib_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.849784 ml4co_kit-0.0.1/ml4co_kit/evaluate/tsp/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/evaluate/tsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/evaluate/tsp/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/evaluate/tsp/tsplib_original_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/evaluate/tsp/uniform_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.849784 ml4co_kit-0.0.1/ml4co_kit/generator/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/generator/mis_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14195 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/generator/tsp_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.849784 ml4co_kit-0.0.1/ml4co_kit/learning/
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/learning/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/learning/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/learning/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/learning/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.849784 ml4co_kit-0.0.1/ml4co_kit/solver/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.849784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10540 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/gurobi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.853784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/
--rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)   101393 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.853784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/app/
--rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/app/configuration_mis.h
--rw-r--r--   0 runner    (1001) docker     (127)    10626 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/app/graphchecker.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/app/online_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/app/parse_parameters.h
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/app/parse_parameters_omis.h
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/app/reduction_evomis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/app/sort_adjacencies.cpp
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/compile_withcmake.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.833784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.829784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.853784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/app/
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/app/balance_configuration.h
--rw-r--r--   0 runner    (1001) docker     (127)    18484 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/app/configuration.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.853784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/interface/
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/interface/SConscript
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/interface/SConstruct
--rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/interface/kaHIP_interface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/interface/kaHIP_interface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.853784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.857784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)    16717 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/cycle_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/cycle_search.h
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/push_relabel.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/push_relabel.h
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/strongly_connected_components.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/strongly_connected_components.h
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/topological_sort.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/topological_sort.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.857784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/flow_graph.h
--rw-r--r--   0 runner    (1001) docker     (127)    15362 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_access.h
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_hierarchy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_hierarchy.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.857784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/matrix/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/matrix/matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/matrix/normal_matrix.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.857784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/bucket_pq.h
--rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/union_find.h
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/definitions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.857784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/io/
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/io/graph_io.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/io/graph_io.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.857784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/diversifyer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.861784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/exchange/
--rw-r--r--   0 runner    (1001) docker     (127)     9984 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/exchange/exchanger.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/exchange/exchanger.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.861784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.h
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.h
--rw-r--r--   0 runner    (1001) docker     (127)    12929 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/parallel_mh_async.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/parallel_mh_async.h
--rw-r--r--   0 runner    (1001) docker     (127)    16545 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/population.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/population.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.861784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.861784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.861784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.h
--rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.h
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening.h
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening_configurator.h
--rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/contraction.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/contraction.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.861784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/edge_rating/
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.865784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/compare_degrees.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.865784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/compare_rating.h
--rw-r--r--   0 runner    (1001) docker     (127)    14090 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.h
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.h
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.h
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/matching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/matching.h
--rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/random_matching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/random_matching.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.865784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/stop_rules/
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/stop_rules/stop_rules.h
--rw-r--r--   0 runner    (1001) docker     (127)    10512 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/graph_partitioner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/graph_partitioner.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.865784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/
--rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/bipartition.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/bipartition.h
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.h
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.h
--rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.865784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/partition_config.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.869784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.869784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.869784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/
--rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    30385 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.h
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.h
--rw-r--r--   0 runner    (1001) docker     (127)    24993 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    18912 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.h
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_definitions.h
--rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.h
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.873784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.h
--rw-r--r--   0 runner    (1001) docker     (127)     9915 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.h
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_stop_rule.h
--rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.873784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     7702 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.873784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.877784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/partition_accept_rule.h
--rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/queue_selection_strategie.h
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/search_stop_rule.h
--rw-r--r--   0 runner    (1001) docker     (127)    18924 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.h
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/vertex_moved_hashtable.h
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/boundary_lookup.h
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    25414 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.877784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.877784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/
--rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.877784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/
--rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.h
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.h
--rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.877784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.h
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.h
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.h
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/two_way_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.877784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/
--rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_bucket_queue.h
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_moves_queue.h
--rw-r--r--   0 runner    (1001) docker     (127)    11539 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.881784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/
--rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.h
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.881784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/w_cycles/
--rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.885784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_communication.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_communication.h
--rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_extractor.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_extractor.h
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_partition_assertions.h
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/macros_assertions.h
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/macros_common.h
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/misc.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/misc.h
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/mpi_tools.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/mpi_tools.h
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/partition_snapshooter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/partition_snapshooter.h
--rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/quality_metrics.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/quality_metrics.h
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/random_functions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/random_functions.h
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/timer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.885784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/Makefile.nmake
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   156123 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/argtable3.c
--rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/argtable3.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.885784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/Makefile.nmake
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/echo.c
--rw-r--r--   0 runner    (1001) docker     (127)    16761 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/ls.c
--rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/multisyntax.c
--rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/mv.c
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/myprog.c
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/myprog_C89.c
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/testargtable3.c
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/uname.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.889784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CuTest.c
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CuTest.h
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/Makefile.nmake
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testall.c
--rw-r--r--   0 runner    (1001) docker     (127)    15949 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargdate.c
--rw-r--r--   0 runner    (1001) docker     (127)    18636 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargdbl.c
--rw-r--r--   0 runner    (1001) docker     (127)    26632 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargfile.c
--rw-r--r--   0 runner    (1001) docker     (127)    81374 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargint.c
--rw-r--r--   0 runner    (1001) docker     (127)    21822 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testarglit.c
--rw-r--r--   0 runner    (1001) docker     (127)    13187 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargrex.c
--rw-r--r--   0 runner    (1001) docker     (127)    22381 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargstr.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.833784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.893784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/data_structure/
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/data_structure/array_set.h
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/data_structure/candidate_list.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/data_structure/candidate_list.h
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/data_structure/candidate_list_online.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/data_structure/candidate_list_online.h
--rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/data_structure/mis_permutation.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/data_structure/mis_permutation.h
--rw-r--r--   0 runner    (1001) docker     (127)    17497 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/data_structure/mis_permutation_online.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/data_structure/mis_permutation_online.h
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/data_structure/operation_log.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/data_structure/operation_log.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.893784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/data_structure/priority_queues/
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/data_structure/priority_queues/bucket_array.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/data_structure/priority_queues/bucket_array.h
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/data_structure/sparse_array_set.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.893784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.893784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.893784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/combine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/combine.h
--rw-r--r--   0 runner    (1001) docker     (127)    13072 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/cover_combine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/cover_combine.h
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/multiway_combine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/multiway_combine.h
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/separator_combine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/separator_combine.h
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/diversifier.h
--rw-r--r--   0 runner    (1001) docker     (127)    13116 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/population_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/population_mis.h
--rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/reduction_evolution.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/reduction_evolution.h
--rw-r--r--   0 runner    (1001) docker     (127)    16938 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/separator_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/separator_pool.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.893784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/hopcroft/
--rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/hopcroft/bipartite_vertex_cover.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/hopcroft/bipartite_vertex_cover.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.897784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/
--rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/ils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/ils.h
--rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/local_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/local_search.h
--rw-r--r--   0 runner    (1001) docker     (127)     9443 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/local_search_online.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/local_search_online.h
--rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/online_ils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/online_ils.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.897784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis.h
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis_online.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis_online.h
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_vertex.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_vertex.h
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/initial_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/initial_mis.h
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/random_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/random_mis.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.901784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.833784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.833784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.901784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/
--rw-r--r--   0 runner    (1001) docker     (127)    70067 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Graph.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Graph.h
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Utility.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Utility.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.833784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.833784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.833784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.901784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.901784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/
--rw-r--r--   0 runner    (1001) docker     (127)    15362 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/graph_access.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.901784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/priority_queues/
--rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/definitions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.901784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/io/
--rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/io/graph_io.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/io/graph_io.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.901784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/macros_assertions.h
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/macros_common.h
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/timer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.905784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/
--rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/ArraySet.h
--rw-r--r--   0 runner    (1001) docker     (127)    36218 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/MaximumMatching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/MaximumMatching.h
--rw-r--r--   0 runner    (1001) docker     (127)    12654 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/ProfilingHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/Reduction.h
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/SimpleSet.h
--rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/SparseArraySet.h
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/bucket_pq.h
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/configuration_mis.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.905784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/data_structures/
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/data_structures/array_set.h
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/fast_set.h
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/full_reductions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/full_reductions.h
--rw-r--r--   0 runner    (1001) docker     (127)    67592 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/parallel_reductions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/parallel_reductions.h
--rw-r--r--   0 runner    (1001) docker     (127)    67473 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/branch_and_reduce_algorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/branch_and_reduce_algorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/fast_set.h
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/modified.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/modified.h
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/mis/mis_config.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.905784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/tools/
--rw-r--r--   0 runner    (1001) docker     (127)    24348 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/tools/mis_log.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7978 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/lib/tools/mis_log.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.905784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/misc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.905784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/misc/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/misc/conversion/dimacs_to_metis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/misc/conversion/metis_to_dimacs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/misc/conversion/sort_metis.py
--rw-r--r--   0 runner    (1001) docker     (127)    16853 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/misc/cpp.vim
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.905784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/
--rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.905784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/app/
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/app/branch_reduce.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/app/configuration_mis.h
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/app/merge_graph_weights.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/app/parse_parameters.h
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/app/weighted_ls.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.841784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.905784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.909784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/interface/
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/interface/SConscript
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/interface/SConstruct
--rw-r--r--   0 runner    (1001) docker     (127)    11971 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/interface/kaHIP_interface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/interface/kaHIP_interface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.909784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.909784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)    16771 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/cycle_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/cycle_search.h
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/push_relabel.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/push_relabel.h
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/strongly_connected_components.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/strongly_connected_components.h
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/topological_sort.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/topological_sort.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.909784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/flow_graph.h
--rw-r--r--   0 runner    (1001) docker     (127)    15794 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_access.h
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_hierarchy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_hierarchy.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.909784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/normal_matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/online_distance_matrix.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.913784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/
--rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/bucket_pq.h
--rw-r--r--   0 runner    (1001) docker     (127)     9902 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/union_find.h
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/definitions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.913784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/io/
--rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/io/graph_io.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/io/graph_io.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.913784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/communication_graph_search_space.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/communication_graph_search_space.h
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_distance_matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_distance_matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_mapping.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_mapping.h
--rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/fast_construct_mapping.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/fast_construct_mapping.h
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space.h
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space_pruned.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space_pruned.h
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/local_search_mapping.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/local_search_mapping.h
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/mapping_algorithms.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/mapping_algorithms.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.917784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/diversifyer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.917784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/exchange/
--rw-r--r--   0 runner    (1001) docker     (127)    10946 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/exchange/exchanger.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/exchange/exchanger.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.917784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.h
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.h
--rw-r--r--   0 runner    (1001) docker     (127)    14215 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/parallel_mh_async.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/parallel_mh_async.h
--rw-r--r--   0 runner    (1001) docker     (127)    16784 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/population.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/population.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.917784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.917784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.917784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.h
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.h
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening.h
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening_configurator.h
--rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/contraction.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/contraction.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.917784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/edge_rating/
--rw-r--r--   0 runner    (1001) docker     (127)    14597 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.921784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/compare_degrees.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.921784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/compare_rating.h
--rw-r--r--   0 runner    (1001) docker     (127)    14144 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.h
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.h
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.h
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/matching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/matching.h
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/random_matching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/random_matching.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.921784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/stop_rules/
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/stop_rules/stop_rules.h
--rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/graph_partitioner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/graph_partitioner.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.925784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/
--rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/bipartition.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/bipartition.h
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_node_separator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_node_separator.h
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.h
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.h
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.925784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/partition_config.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.925784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.925784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.925784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/
--rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    30439 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.h
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.h
--rw-r--r--   0 runner    (1001) docker     (127)    25053 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.h
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_definitions.h
--rw-r--r--   0 runner    (1001) docker     (127)    10193 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.h
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.929784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.h
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.h
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_stop_rule.h
--rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.929784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     7756 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.929784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/
--rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/fm_ns_local_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8299 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/fm_ns_local_search.h
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/greedy_ns_local_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/greedy_ns_local_search.h
--rw-r--r--   0 runner    (1001) docker     (127)    13928 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/localized_fm_ns_local_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/localized_fm_ns_local_search.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.933784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.933784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/partition_accept_rule.h
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/queue_selection_strategie.h
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/search_stop_rule.h
--rw-r--r--   0 runner    (1001) docker     (127)    18978 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.h
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/vertex_moved_hashtable.h
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/boundary_lookup.h
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    25468 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.933784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.933784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/
--rw-r--r--   0 runner    (1001) docker     (127)    10337 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.933784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/
--rw-r--r--   0 runner    (1001) docker     (127)     8648 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.h
--rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.h
--rw-r--r--   0 runner    (1001) docker     (127)    13845 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.937784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.h
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.h
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.h
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/two_way_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.937784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_bucket_queue.h
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_moves_queue.h
--rw-r--r--   0 runner    (1001) docker     (127)    11593 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.937784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/area_bfs.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/area_bfs.h
--rw-r--r--   0 runner    (1001) docker     (127)    31427 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.h
--rw-r--r--   0 runner    (1001) docker     (127)    13781 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.937784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/w_cycles/
--rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.937784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/spac/
--rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/spac/spac.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/spac/spac.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.941784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_communication.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_communication.h
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_extractor.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_extractor.h
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_partition_assertions.h
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/macros_assertions.h
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/macros_common.h
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/misc.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/misc.h
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/mpi_tools.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/mpi_tools.h
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/partition_snapshooter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/partition_snapshooter.h
--rw-r--r--   0 runner    (1001) docker     (127)    13611 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/quality_metrics.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/quality_metrics.h
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/random_functions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/random_functions.h
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/timer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.941784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/Makefile.nmake
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   156123 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/argtable3.c
--rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/argtable3.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.945783 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/Makefile.nmake
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/echo.c
--rw-r--r--   0 runner    (1001) docker     (127)    16761 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/ls.c
--rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/multisyntax.c
--rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/mv.c
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/myprog.c
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/myprog_C89.c
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/testargtable3.c
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/uname.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.949784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CuTest.c
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CuTest.h
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/Makefile.nmake
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testall.c
--rw-r--r--   0 runner    (1001) docker     (127)    15949 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargdate.c
--rw-r--r--   0 runner    (1001) docker     (127)    18636 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargdbl.c
--rw-r--r--   0 runner    (1001) docker     (127)    26632 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargfile.c
--rw-r--r--   0 runner    (1001) docker     (127)    81374 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargint.c
--rw-r--r--   0 runner    (1001) docker     (127)    21822 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testarglit.c
--rw-r--r--   0 runner    (1001) docker     (127)    13187 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargrex.c
--rw-r--r--   0 runner    (1001) docker     (127)    22381 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargstr.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.841784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.949784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/array_set.h
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/candidate_list.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/candidate_list.h
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/dynamic_graph.h
--rw-r--r--   0 runner    (1001) docker     (127)    10625 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/mis_permutation.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/mis_permutation.h
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/operation_log.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/operation_log.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.949784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/priority_queues/
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/priority_queues/bucket_array.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/priority_queues/bucket_array.h
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/sized_vector.h
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/sparse_array_set.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.949784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.949784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/ils/
--rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/ils/ils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/ils/ils.h
--rw-r--r--   0 runner    (1001) docker     (127)    12974 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/ils/local_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/ils/local_search.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.953784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_mis.h
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_vertex.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_vertex.h
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/initial_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/initial_mis.h
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/random_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/random_mis.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.953784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)    25450 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/branch_and_reduce_algorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/branch_and_reduce_algorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/fast_set.h
--rw-r--r--   0 runner    (1001) docker     (127)    31140 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/reductions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10796 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/reductions.h
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/mis_config.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.953784 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/tools/mis_log.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis-source/wmis/lib/tools/mis_log.h
--rw-r--r--   0 runner    (1001) docker     (127)     9327 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.953784 ml4co_kit-0.0.1/ml4co_kit/solver/tsp/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/tsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14521 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/tsp/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/tsp/concorde.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/tsp/lkh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.953784 ml4co_kit-0.0.1/ml4co_kit/solver/tsp/lkh_solver/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/tsp/lkh_solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/tsp/lkh_solver/problems.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/tsp/lkh_solver/solve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.953784 ml4co_kit-0.0.1/ml4co_kit/solver/tsp/pyconcorde/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/tsp/pyconcorde/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.961784 ml4co_kit-0.0.1/ml4co_kit/solver/tsp/pyconcorde/concorde/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/tsp/pyconcorde/concorde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/tsp/pyconcorde/concorde/_concorde.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/tsp/pyconcorde/concorde/solve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.981783 ml4co_kit-0.0.1/ml4co_kit/solver/tsp/pyconcorde/data/
--rw-r--r--   0 runner    (1001) docker     (127)  7630518 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/tsp/pyconcorde/data/concorde.a
--rw-r--r--   0 runner    (1001) docker     (127)   248168 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/tsp/pyconcorde/data/concorde.h
--rw-r--r--   0 runner    (1001) docker     (127)   854866 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/tsp/pyconcorde/data/qsopt.a
--rw-r--r--   0 runner    (1001) docker     (127)    14871 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/tsp/pyconcorde/data/qsopt.h
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/solver/tsp/pyconcorde/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.981783 ml4co_kit-0.0.1/ml4co_kit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/ml4co_kit/utils/mis_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.981783 ml4co_kit-0.0.1/ml4co_kit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-04-16 04:03:30.000000 ml4co_kit-0.0.1/ml4co_kit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    55766 2024-04-16 04:03:30.000000 ml4co_kit-0.0.1/ml4co_kit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 04:03:30.000000 ml4co_kit-0.0.1/ml4co_kit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-16 04:03:30.000000 ml4co_kit-0.0.1/ml4co_kit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 04:03:30.000000 ml4co_kit-0.0.1/ml4co_kit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 04:03:30.981783 ml4co_kit-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:03:30.981783 ml4co_kit-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/tests/test_draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/tests/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/tests/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-16 04:03:24.000000 ml4co_kit-0.0.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:45:53.750479 ml4co_kit-0.0.1a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-15 16:45:53.750479 ml4co_kit-0.0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:45:53.742479 ml4co_kit-0.0.1a1/ml4co_kit/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:45:53.742479 ml4co_kit-0.0.1a1/ml4co_kit/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:45:53.742479 ml4co_kit-0.0.1a1/ml4co_kit/data/mis/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/data/mis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/data/mis/satlib_original.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:45:53.742479 ml4co_kit-0.0.1a1/ml4co_kit/data/tsp/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/data/tsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/data/tsp/tsp_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/data/tsp/tsplib_original.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:45:53.742479 ml4co_kit-0.0.1a1/ml4co_kit/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/evaluate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:45:53.742479 ml4co_kit-0.0.1a1/ml4co_kit/evaluate/mis/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/evaluate/mis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/evaluate/mis/satlib_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:45:53.746479 ml4co_kit-0.0.1a1/ml4co_kit/evaluate/tsp/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/evaluate/tsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/evaluate/tsp/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/evaluate/tsp/tsplib_original_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/evaluate/tsp/uniform_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:45:53.746479 ml4co_kit-0.0.1a1/ml4co_kit/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/generator/mis_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14195 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/generator/tsp_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:45:53.746479 ml4co_kit-0.0.1a1/ml4co_kit/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/solver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:45:53.746479 ml4co_kit-0.0.1a1/ml4co_kit/solver/mis/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/solver/mis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/solver/mis/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10540 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/solver/mis/gurobi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9327 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/solver/mis/kamis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:45:53.746479 ml4co_kit-0.0.1a1/ml4co_kit/solver/tsp/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/solver/tsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14521 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/solver/tsp/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/solver/tsp/concorde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/solver/tsp/lkh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:45:53.746479 ml4co_kit-0.0.1a1/ml4co_kit/solver/tsp/lkh_solver/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/solver/tsp/lkh_solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/solver/tsp/lkh_solver/problems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/solver/tsp/lkh_solver/solve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:45:53.746479 ml4co_kit-0.0.1a1/ml4co_kit/solver/tsp/pyconcorde/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/solver/tsp/pyconcorde/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:45:53.750479 ml4co_kit-0.0.1a1/ml4co_kit/solver/tsp/pyconcorde/concorde/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/solver/tsp/pyconcorde/concorde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/solver/tsp/pyconcorde/concorde/solve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/solver/tsp/pyconcorde/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:45:53.750479 ml4co_kit-0.0.1a1/ml4co_kit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/ml4co_kit/utils/mis_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:45:53.750479 ml4co_kit-0.0.1a1/ml4co_kit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-15 16:45:53.000000 ml4co_kit-0.0.1a1/ml4co_kit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-15 16:45:53.000000 ml4co_kit-0.0.1a1/ml4co_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:45:53.000000 ml4co_kit-0.0.1a1/ml4co_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-15 16:45:53.000000 ml4co_kit-0.0.1a1/ml4co_kit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 16:45:53.000000 ml4co_kit-0.0.1a1/ml4co_kit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 16:45:53.750479 ml4co_kit-0.0.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:45:53.750479 ml4co_kit-0.0.1a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/tests/test_draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/tests/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-15 16:45:43.000000 ml4co_kit-0.0.1a1/tests/test_utils.py
```

### Comparing `ml4co_kit-0.0.1/PKG-INFO` & `ml4co_kit-0.0.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml4co-kit
-Version: 0.0.1
+Version: 0.0.1a1
 Summary: ml4co-kit provides convenient dataset generators for the combinatorial optimization problem
 Home-page: https://github.com/Thinklab-SJTU/ML4CO-Kit
 Author: SJTU-ReThinkLab
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -30,19 +30,19 @@
 Requires-Dist: pandas>=2.0.0
 Requires-Dist: scipy>=1.10.1
 Requires-Dist: aiohttp>=3.9.3
 
 
 <img src="docs/assets/ml4co-kit-logo.png" alt="ML4CO-Kit" width="800"/>
 
-[![PyPi version](https://badgen.net/pypi/v/ml4co-kit/)](https://pypi.org/pypi/data4co/) [![PyPI pyversions](https://img.shields.io/badge/dynamic/json?color=blue&label=python&query=info.requires_python&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fdata4co%2Fjson)](https://pypi.python.org/pypi/ml4co-kit/) [![Downloads](https://static.pepy.tech/badge/ml4co-kit)](https://pepy.tech/project/ml4co-kit) [![GitHub stars](https://img.shields.io/github/stars/Thinklab-SJTU/ML4CO-Kit.svg?style=social&label=Star&maxAge=8640)](https://GitHub.com/Thinklab-SJTU/ML4CO-Kit/stargazers/)
+[![PyPi version](https://badgen.net/pypi/v/data4co/)](https://pypi.org/pypi/data4co/) [![PyPI pyversions](https://img.shields.io/badge/dynamic/json?color=blue&label=python&query=info.requires_python&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fdata4co%2Fjson)](https://pypi.python.org/pypi/data4co/) [![Downloads](https://static.pepy.tech/badge/data4co)](https://pepy.tech/project/data4co) [![GitHub stars](https://img.shields.io/github/stars/Thinklab-SJTU/ML4CO-Kit.svg?style=social&label=Star&maxAge=8640)](https://GitHub.com/Thinklab-SJTU/ML4CO-Kit/stargazers/) 
 
 `ML4CO-Kit` is a in-development toolkit for machine learning practices on combinatorial optimization problems, which is a by-product of our research for a unified modular framework that integrates existing ML4CO practices, minimizing disparities among methods and supporting the investigations via in-depth analysis and transparent ablation. 
 
-This reposity focuses on the supporting code for method development instead of implementing core technologies, which will be presented in the future in our full implementation and organization. `ML4CO-Kit` has the following features:
+This reposity focuses on the supporting code for method development instead of implementing core technologies, which will be presented in the future  in our full implementation and organization. `ML4CO-Kit` has the following features:
 
 * The skeleton of framework organization for ML4CO projects;
 * Implemented base classes that facilitate method development;
 * Mainstream traditional solver baselines and reference solution acquisition;
 * Data generation of various distributions;
 * Problem and solution visualization;
 * Evaluators for different problems.
@@ -92,15 +92,15 @@
 
 ```bash
 $ pip install matplotlib>=3.7.5
 ```
 
 ## Usage Examples
 
-### Solve with Traditional Solver Baselines
+### Solve with  Traditional Solver Baselines
 
 We provide base classes that offer a user-friendly approach for implementing traditional and learning-based solvers. Taking `TSPSolver` as an example, which includes functionalities for data input and output, as well as an evaluation function. The solver supports different data inputs, such as Numpy arrays and .txt and .tsp files. The outputs can be saved to corresponding types of files as needed. Additionally, the solver offers an evaluation function, by which users can quickly obtain the average tour length, average gap, and standard deviation of the test dataset. Traditional solvers are directly incorporated in our library inheriting `TSPSolver`.
 
 ```python
 >>> from ml4co_kit.solver import TSPLKHSolver
 
 # initialization
@@ -241,7 +241,8 @@
 <img src="docs/assets/mis_problem.png" width="35%" alt="" />
 <img src="docs/assets/mis_solution.png" width="35%" alt="" />
 </p>
 
 ### Develop ML4CO Algorithms
 
 Please refer to `ml4co_kit/learning` for the base classes that facilitate a quick establishment of a ML4CO project. You can easily build a project by inheriting the base classes and additionally implement task-specific and methodology-specific functions according to [ML4CO Organization](#ML4CO Organization:). We provide an minimalistic exmple of build a simple ML4TSP project in `docs/project_example`.
+
```

### Comparing `ml4co_kit-0.0.1/README.md` & `ml4co_kit-0.0.1a1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <img src="docs/assets/ml4co-kit-logo.png" alt="ML4CO-Kit" width="800"/>
 
-[![PyPi version](https://badgen.net/pypi/v/ml4co-kit/)](https://pypi.org/pypi/data4co/) [![PyPI pyversions](https://img.shields.io/badge/dynamic/json?color=blue&label=python&query=info.requires_python&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fdata4co%2Fjson)](https://pypi.python.org/pypi/ml4co-kit/) [![Downloads](https://static.pepy.tech/badge/ml4co-kit)](https://pepy.tech/project/ml4co-kit) [![GitHub stars](https://img.shields.io/github/stars/Thinklab-SJTU/ML4CO-Kit.svg?style=social&label=Star&maxAge=8640)](https://GitHub.com/Thinklab-SJTU/ML4CO-Kit/stargazers/)
+[![PyPi version](https://badgen.net/pypi/v/data4co/)](https://pypi.org/pypi/data4co/) [![PyPI pyversions](https://img.shields.io/badge/dynamic/json?color=blue&label=python&query=info.requires_python&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fdata4co%2Fjson)](https://pypi.python.org/pypi/data4co/) [![Downloads](https://static.pepy.tech/badge/data4co)](https://pepy.tech/project/data4co) [![GitHub stars](https://img.shields.io/github/stars/Thinklab-SJTU/ML4CO-Kit.svg?style=social&label=Star&maxAge=8640)](https://GitHub.com/Thinklab-SJTU/ML4CO-Kit/stargazers/) 
 
 `ML4CO-Kit` is a in-development toolkit for machine learning practices on combinatorial optimization problems, which is a by-product of our research for a unified modular framework that integrates existing ML4CO practices, minimizing disparities among methods and supporting the investigations via in-depth analysis and transparent ablation. 
 
-This reposity focuses on the supporting code for method development instead of implementing core technologies, which will be presented in the future in our full implementation and organization. `ML4CO-Kit` has the following features:
+This reposity focuses on the supporting code for method development instead of implementing core technologies, which will be presented in the future  in our full implementation and organization. `ML4CO-Kit` has the following features:
 
 * The skeleton of framework organization for ML4CO projects;
 * Implemented base classes that facilitate method development;
 * Mainstream traditional solver baselines and reference solution acquisition;
 * Data generation of various distributions;
 * Problem and solution visualization;
 * Evaluators for different problems.
@@ -58,15 +58,15 @@
 
 ```bash
 $ pip install matplotlib>=3.7.5
 ```
 
 ## Usage Examples
 
-### Solve with Traditional Solver Baselines
+### Solve with  Traditional Solver Baselines
 
 We provide base classes that offer a user-friendly approach for implementing traditional and learning-based solvers. Taking `TSPSolver` as an example, which includes functionalities for data input and output, as well as an evaluation function. The solver supports different data inputs, such as Numpy arrays and .txt and .tsp files. The outputs can be saved to corresponding types of files as needed. Additionally, the solver offers an evaluation function, by which users can quickly obtain the average tour length, average gap, and standard deviation of the test dataset. Traditional solvers are directly incorporated in our library inheriting `TSPSolver`.
 
 ```python
 >>> from ml4co_kit.solver import TSPLKHSolver
 
 # initialization
@@ -207,7 +207,8 @@
 <img src="docs/assets/mis_problem.png" width="35%" alt="" />
 <img src="docs/assets/mis_solution.png" width="35%" alt="" />
 </p>
 
 ### Develop ML4CO Algorithms
 
 Please refer to `ml4co_kit/learning` for the base classes that facilitate a quick establishment of a ML4CO project. You can easily build a project by inheriting the base classes and additionally implement task-specific and methodology-specific functions according to [ML4CO Organization](#ML4CO Organization:). We provide an minimalistic exmple of build a simple ML4TSP project in `docs/project_example`.
+
```

### Comparing `ml4co_kit-0.0.1/docs/project_example/solver.py` & `ml4co_kit-0.0.1a1/ml4co_kit/solver/tsp/lkh.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,121 +1,142 @@
 import time
 import numpy as np
+import tsplib95
+import pathlib
 from tqdm import tqdm
-from typing import Union, Any
-from pytorch_lightning.utilities import rank_zero_info
-from ml4co_kit.solver import TSPSolver
-from ml4co_kit.learning.model import BaseEncoder, ModelConfigurator
-from ml4co_kit.learning.search import SearchConfigurator
-from model import TSPGNN
-from search import tsp_greedy, tsp_2opt
-
-
-class TSPNARSolver(TSPSolver):
-    """
-    This is an TSP solver example to easily develop a solver class based on the learning models
-    by inheriting from the class ``solver.TSPSolver``.
-    """
+from multiprocessing import Pool
+from typing import Union
+from .base import TSPSolver
+from .lkh_solver import lkh_solve
 
-    def __init__(self):
-        super(TSPNARSolver, self).__init__()
 
-    def solve(
+class TSPLKHSolver(TSPSolver):
+    def __init__(
         self,
-        batch_size: int = 16,
-        encoder: Union[BaseEncoder, str] = "gnn",
-        encoder_kwargs: dict = {},
-        decoding_type: Union[Any, str] = "greedy",
-        decoding_kwargs: dict = {},
-        local_search_type: str = "2opt",
-        ls_kwargs: dict = {},
-        pretrained: bool = True,
-        device="cpu",
+        lkh_max_trials: int = 1000,
+        lkh_path: pathlib.Path = "LKH",
+        scale: int = 1e6,
+        lkh_runs: int = 10,
     ):
-        self.decoding_type = decoding_type
-        self.ls_type = local_search_type
-        self.model_config = ModelConfigurator(model_class={("tsp", "gnn"): TSPGNN})
-        self.search_config = SearchConfigurator(
-            decoding_class={("tsp", "greedy"): tsp_greedy},
-            local_search_class={("tsp", "2opt"): tsp_2opt},
+        """
+        TSPLKHSolver
+        Args:
+            lkh_max_trials (int, optional): The maximum number of trials for
+                the LKH solver. Defaults to 1000.
+            lkh_path (pathlib.Path, optional): The path to the LKH solver.
+                Defaults to "LKH".
+            scale (int, optional): The scale factor for coordinates in the
+                LKH solver. Defaults to 1e6.
+            lkh_runs (int, optional): The number of runs for the LKH solver.
+                Defaults to 10.
+        """
+        super(TSPLKHSolver, self).__init__(solver_type="lkh", scale=scale)
+        self.lkh_max_trials = lkh_max_trials
+        self.lkh_path = lkh_path
+        self.scale = scale
+        self.lkh_runs = lkh_runs
+
+    def _solve(self, nodes_coord: np.ndarray) -> list:
+        problem = tsplib95.models.StandardProblem()
+        problem.name = "TSP"
+        problem.type = "TSP"
+        problem.dimension = self.nodes_num
+        problem.edge_weight_type = self.norm
+        problem.node_coords = {
+            n + 1: nodes_coord[n] * self.scale for n in range(self.nodes_num)
+        }
+        solution = lkh_solve(
+            solver=self.lkh_path,
+            problem=problem,
+            max_trials=self.lkh_max_trials,
+            runs=self.lkh_runs,
         )
+        tour = [n - 1 for n in solution[0]]
+        return tour
 
-        # encoder & gain heatmap
-        if type(encoder) == str:
-            encoder_kwargs.update(
-                {
-                    "mode": "solve",
-                    "nodes_num": self.nodes_num,
-                }
-            )
-            self.encoder = self.model_config.get_model(task="tsp", model_name=encoder)(
-                **encoder_kwargs
-            )
-        else:
-            self.encoder = encoder
-        rank_zero_info(f"Begin encoding, Using {self.encoder}")
-        if pretrained:
-            rank_zero_info(f"Loading Weights from Pretrained CheckPoint")
-            pretrained_path = (
-                encoder_kwargs["pretrained_path"]
-                if "pretrained_path" in encoder_kwargs.keys()
-                else None
-            )
-            self.encoder.load_weights(pretrained_path)
-        self.encoder.to(device)
-
-        # model inference
-        solve_begin_time = time.time()
-        edge_index = None
-        points = self.points
-        heatmap = self.encoder.solve(points, edge_index, batch_size, device)
-        solve_end_time = time.time()
-        solve_time = solve_end_time - solve_begin_time
-        rank_zero_info(f"Model Inference, Using {solve_time}")
-
-        # decoding
-        if type(decoding_type) == str:
-            self.decoding_func = self.search_config.get_decoding_func(
-                task="tsp", name=decoding_type
-            )
+    def solve(
+        self,
+        points: Union[np.ndarray, list] = None,
+        norm: str = "EUC_2D",
+        normalize: bool = False,
+        num_threads: int = 1,
+        show_time: bool = False,
+    ) -> np.ndarray:
+        # prepare
+        self.from_data(points, norm, normalize)
+        start_time = time.time()
+
+        # solve
+        tours = list()
+        p_shape = self.points.shape
+        num_points = p_shape[0]
+        if num_threads == 1:
+            if show_time:
+                for idx in tqdm(range(num_points), desc="Solving TSP Using LKH"):
+                    tours.append(self._solve(self.points[idx]))
+            else:
+                for idx in range(num_points):
+                    tours.append(self._solve(self.points[idx]))
         else:
-            self.decoding_func = decoding_type
-        rank_zero_info(f"Decoding, Using {self.decoding_func.__name__}")
-        decoded_tours = list()
-        for idx in tqdm(range(self.points.shape[0]), desc="Decoding"):
-            adj_mat = np.expand_dims(heatmap[idx], axis=0)
-            tour = self.decoding_func(
-                adj_mat=adj_mat, 
-                np_points=self.points[idx], 
-                edge_index_np=None,
-                **decoding_kwargs
+            batch_points = self.points.reshape(
+                -1, num_threads, p_shape[-2], p_shape[-1]
             )
-            decoded_tours.append(tour[0])
-        decoded_tours = np.array(decoded_tours)
-
-        # local_search
-        ls_tours = None
-        self.local_search_func = self.search_config.get_local_search_func(
-            task="tsp", name=local_search_type
-        )
-        if self.local_search_func is not None:
-            rank_zero_info(f"Local Search, Using {self.local_search_func.__name__}")
-            ls_tours = list()
-            for idx in tqdm(range(self.points.shape[0]), desc="Local Search"):
-                adj_mat = heatmap[idx]
-                tour = self.local_search_func(
-                    np_points=self.points[idx],
-                    tours=decoded_tours[idx],
-                    adj_mat=adj_mat,
-                    device=device,
-                    **ls_kwargs,
-                )
-                ls_tours.append(tour)
-            ls_tours = np.array(ls_tours)
-
-        tours = decoded_tours if ls_tours is None else ls_tours
-        self.tours = tours
+            if show_time:
+                for idx in tqdm(
+                    range(num_points // num_threads), desc="Solving TSP Using LKH"
+                ):
+                    with Pool(num_threads) as p1:
+                        cur_tours = p1.map(
+                            self._solve,
+                            [
+                                batch_points[idx][inner_idx]
+                                for inner_idx in range(num_threads)
+                            ],
+                        )
+                    for tour in cur_tours:
+                        tours.append(tour)
+            else:
+                for idx in range(num_points // num_threads):
+                    with Pool(num_threads) as p1:
+                        cur_tours = p1.map(
+                            self._solve,
+                            [
+                                batch_points[idx][inner_idx]
+                                for inner_idx in range(num_threads)
+                            ],
+                        )
+                    for tour in cur_tours:
+                        tours.append(tour)
+
+        # format
+        tours = np.array(tours)
+        zeros = np.zeros((tours.shape[0], 1))
+        tours = np.append(tours, zeros, axis=1).astype(np.int32)
+        if tours.ndim == 2 and tours.shape[0] == 1:
+            tours = tours[0]
+        self.read_tours(tours)
+        end_time = time.time()
+        if show_time:
+            print(f"Use Time: {end_time - start_time}")
         return tours
 
-    def __repr__(self):
-        message = f"encoder={self.encoder}, decoding_type={self.decoding_type}, ls_type={self.ls_type}"
-        return f"{self.__class__.__name__}({message})"
+    def regret_solve(
+        self, points: np.ndarray, fixed_edges: tuple, norm: str = "EUC_2D"
+    ):
+        problem = tsplib95.models.StandardProblem()
+        problem.name = "TSP"
+        problem.type = "TSP"
+        problem.dimension = points.shape[0]
+        problem.edge_weight_type = norm
+        problem.node_coords = {
+            n + 1: self.scale * points[n] for n in range(points.shape[0])
+        }
+        problem.fixed_edges = [[n + 1 for n in fixed_edges]]
+        solution = lkh_solve(
+            solver=self.lkh_path,
+            problem=problem,
+            max_trials=self.lkh_max_trials,
+            runs=self.lkh_runs,
+        )
+        tour = [n - 1 for n in solution[0]] + [0]
+        np_tour = np.array(tour)
+        return np_tour
```

### Comparing `ml4co_kit-0.0.1/ml4co_kit/__init__.py` & `ml4co_kit-0.0.1a1/ml4co_kit/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 if found_matplotlib is not None:
     from .draw.tsp import draw_tsp_problem, draw_tsp_solution
     from .draw.mis import draw_mis_problem, draw_mis_solution
 else:
     print("matplotlib not installed")
 
 
-__version__ = "0.0.1"
+__version__ = "0.0.1a1"
 __author__ = "SJTU-ReThinkLab"
```

### Comparing `ml4co_kit-0.0.1/ml4co_kit/data/mis/satlib_original.py` & `ml4co_kit-0.0.1a1/ml4co_kit/data/mis/satlib_original.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/ml4co_kit/data/tsp/tsp_uniform.py` & `ml4co_kit-0.0.1a1/ml4co_kit/data/tsp/tsp_uniform.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/ml4co_kit/data/tsp/tsplib_original.py` & `ml4co_kit-0.0.1a1/ml4co_kit/data/tsp/tsplib_original.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/ml4co_kit/evaluate/mis/satlib_eval.py` & `ml4co_kit-0.0.1a1/ml4co_kit/evaluate/mis/satlib_eval.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/ml4co_kit/evaluate/tsp/base.py` & `ml4co_kit-0.0.1a1/ml4co_kit/evaluate/tsp/base.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/ml4co_kit/evaluate/tsp/tsplib_original_eval.py` & `ml4co_kit-0.0.1a1/ml4co_kit/evaluate/tsp/tsplib_original_eval.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/ml4co_kit/evaluate/tsp/uniform_eval.py` & `ml4co_kit-0.0.1a1/ml4co_kit/evaluate/tsp/uniform_eval.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/ml4co_kit/generator/mis_data.py` & `ml4co_kit-0.0.1a1/ml4co_kit/generator/mis_data.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/ml4co_kit/generator/tsp_data.py` & `ml4co_kit-0.0.1a1/ml4co_kit/generator/tsp_data.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/ml4co_kit/solver/mis/base.py` & `ml4co_kit-0.0.1a1/ml4co_kit/solver/mis/base.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/ml4co_kit/solver/mis/gurobi.py` & `ml4co_kit-0.0.1a1/ml4co_kit/solver/mis/gurobi.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/ml4co_kit/solver/mis/kamis.py` & `ml4co_kit-0.0.1a1/ml4co_kit/solver/mis/kamis.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/ml4co_kit/solver/tsp/base.py` & `ml4co_kit-0.0.1a1/ml4co_kit/solver/tsp/base.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/ml4co_kit/solver/tsp/concorde.py` & `ml4co_kit-0.0.1a1/ml4co_kit/solver/tsp/concorde.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/ml4co_kit/solver/tsp/lkh_solver/problems.py` & `ml4co_kit-0.0.1a1/ml4co_kit/solver/tsp/lkh_solver/problems.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/ml4co_kit/solver/tsp/lkh_solver/solve.py` & `ml4co_kit-0.0.1a1/ml4co_kit/solver/tsp/lkh_solver/solve.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/ml4co_kit/solver/tsp/pyconcorde/concorde/solve.py` & `ml4co_kit-0.0.1a1/ml4co_kit/solver/tsp/pyconcorde/concorde/solve.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/ml4co_kit/solver/tsp/pyconcorde/setup.py` & `ml4co_kit-0.0.1a1/ml4co_kit/solver/tsp/pyconcorde/setup.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/ml4co_kit/utils/file_utils.py` & `ml4co_kit-0.0.1a1/ml4co_kit/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/ml4co_kit/utils/mis_utils.py` & `ml4co_kit-0.0.1a1/ml4co_kit/utils/mis_utils.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/ml4co_kit.egg-info/PKG-INFO` & `ml4co_kit-0.0.1a1/ml4co_kit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml4co-kit
-Version: 0.0.1
+Version: 0.0.1a1
 Summary: ml4co-kit provides convenient dataset generators for the combinatorial optimization problem
 Home-page: https://github.com/Thinklab-SJTU/ML4CO-Kit
 Author: SJTU-ReThinkLab
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -30,19 +30,19 @@
 Requires-Dist: pandas>=2.0.0
 Requires-Dist: scipy>=1.10.1
 Requires-Dist: aiohttp>=3.9.3
 
 
 <img src="docs/assets/ml4co-kit-logo.png" alt="ML4CO-Kit" width="800"/>
 
-[![PyPi version](https://badgen.net/pypi/v/ml4co-kit/)](https://pypi.org/pypi/data4co/) [![PyPI pyversions](https://img.shields.io/badge/dynamic/json?color=blue&label=python&query=info.requires_python&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fdata4co%2Fjson)](https://pypi.python.org/pypi/ml4co-kit/) [![Downloads](https://static.pepy.tech/badge/ml4co-kit)](https://pepy.tech/project/ml4co-kit) [![GitHub stars](https://img.shields.io/github/stars/Thinklab-SJTU/ML4CO-Kit.svg?style=social&label=Star&maxAge=8640)](https://GitHub.com/Thinklab-SJTU/ML4CO-Kit/stargazers/)
+[![PyPi version](https://badgen.net/pypi/v/data4co/)](https://pypi.org/pypi/data4co/) [![PyPI pyversions](https://img.shields.io/badge/dynamic/json?color=blue&label=python&query=info.requires_python&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fdata4co%2Fjson)](https://pypi.python.org/pypi/data4co/) [![Downloads](https://static.pepy.tech/badge/data4co)](https://pepy.tech/project/data4co) [![GitHub stars](https://img.shields.io/github/stars/Thinklab-SJTU/ML4CO-Kit.svg?style=social&label=Star&maxAge=8640)](https://GitHub.com/Thinklab-SJTU/ML4CO-Kit/stargazers/) 
 
 `ML4CO-Kit` is a in-development toolkit for machine learning practices on combinatorial optimization problems, which is a by-product of our research for a unified modular framework that integrates existing ML4CO practices, minimizing disparities among methods and supporting the investigations via in-depth analysis and transparent ablation. 
 
-This reposity focuses on the supporting code for method development instead of implementing core technologies, which will be presented in the future in our full implementation and organization. `ML4CO-Kit` has the following features:
+This reposity focuses on the supporting code for method development instead of implementing core technologies, which will be presented in the future  in our full implementation and organization. `ML4CO-Kit` has the following features:
 
 * The skeleton of framework organization for ML4CO projects;
 * Implemented base classes that facilitate method development;
 * Mainstream traditional solver baselines and reference solution acquisition;
 * Data generation of various distributions;
 * Problem and solution visualization;
 * Evaluators for different problems.
@@ -92,15 +92,15 @@
 
 ```bash
 $ pip install matplotlib>=3.7.5
 ```
 
 ## Usage Examples
 
-### Solve with Traditional Solver Baselines
+### Solve with  Traditional Solver Baselines
 
 We provide base classes that offer a user-friendly approach for implementing traditional and learning-based solvers. Taking `TSPSolver` as an example, which includes functionalities for data input and output, as well as an evaluation function. The solver supports different data inputs, such as Numpy arrays and .txt and .tsp files. The outputs can be saved to corresponding types of files as needed. Additionally, the solver offers an evaluation function, by which users can quickly obtain the average tour length, average gap, and standard deviation of the test dataset. Traditional solvers are directly incorporated in our library inheriting `TSPSolver`.
 
 ```python
 >>> from ml4co_kit.solver import TSPLKHSolver
 
 # initialization
@@ -241,7 +241,8 @@
 <img src="docs/assets/mis_problem.png" width="35%" alt="" />
 <img src="docs/assets/mis_solution.png" width="35%" alt="" />
 </p>
 
 ### Develop ML4CO Algorithms
 
 Please refer to `ml4co_kit/learning` for the base classes that facilitate a quick establishment of a ML4CO project. You can easily build a project by inheriting the base classes and additionally implement task-specific and methodology-specific functions according to [ML4CO Organization](#ML4CO Organization:). We provide an minimalistic exmple of build a simple ML4TSP project in `docs/project_example`.
+
```

### Comparing `ml4co_kit-0.0.1/setup.py` & `ml4co_kit-0.0.1a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,16 +92,16 @@
     name=NAME,
     version=about["__version__"],
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author=AUTHOR,
     url=URL,
-    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*", "docs/**"]),
-    package_data={PACKAGE_NAME: ["**"], NAME: ["**"], "docs": ["**"]},
+    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
+    package_data={NAME: ["**"], "docs": ["**"]},
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
     license="Mulan PSL v2",
     python_requires=">=3.8",
     classifiers=[
         "License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)",
```

### Comparing `ml4co_kit-0.0.1/tests/test_draw.py` & `ml4co_kit-0.0.1a1/tests/test_draw.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/tests/test_evaluate.py` & `ml4co_kit-0.0.1a1/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/tests/test_generator.py` & `ml4co_kit-0.0.1a1/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/tests/test_solver.py` & `ml4co_kit-0.0.1a1/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.1/tests/test_utils.py` & `ml4co_kit-0.0.1a1/tests/test_utils.py`

 * *Files identical despite different names*

