# Comparing `tmp/tui_dsmt-202404111315.tar.gz` & `tmp/tui_dsmt-202404160633.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui_dsmt-202404111315.tar", last modified: Thu Apr 11 13:15:46 2024, max compression
+gzip compressed data, was "tui_dsmt-202404160633.tar", last modified: Tue Apr 16 06:33:27 2024, max compression
```

## Comparing `tui_dsmt-202404111315.tar` & `tui_dsmt-202404160633.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:15:46.409528 tui_dsmt-202404111315/
--rw-r--r--   0 root         (0) root         (0)      761 2024-04-11 13:15:46.409528 tui_dsmt-202404111315/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 13:15:46.409528 tui_dsmt-202404111315/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1101 2024-04-10 09:51:41.000000 tui_dsmt-202404111315/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:15:46.385528 tui_dsmt-202404111315/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:15:46.385528 tui_dsmt-202404111315/src/tui_dsmt/
--rw-rw-rw-   0 root         (0) root         (0)      780 2024-04-11 12:11:46.000000 tui_dsmt-202404111315/src/tui_dsmt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:15:46.393528 tui_dsmt-202404111315/src/tui_dsmt/clustering/
--rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-10 09:51:41.000000 tui_dsmt-202404111315/src/tui_dsmt/clustering/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2691 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/clustering/animation.py
--rw-rw-rw-   0 root         (0) root         (0)    19108 2024-04-10 09:51:41.000000 tui_dsmt-202404111315/src/tui_dsmt/clustering/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/clustering/draw.py
--rw-rw-rw-   0 root         (0) root         (0)     1749 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/clustering/evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)     4488 2024-04-10 09:51:41.000000 tui_dsmt-202404111315/src/tui_dsmt/clustering/hierarchical.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/clustering/interactive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:15:46.397528 tui_dsmt-202404111315/src/tui_dsmt/fpm/
--rw-rw-rw-   0 root         (0) root         (0)    14098 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/fpm/BruteForceFI.py
--rw-rw-rw-   0 root         (0) root         (0)     4055 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/fpm/ConditionalFPTree.py
--rw-rw-rw-   0 root         (0) root         (0)     5522 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/fpm/ConditionalPatternBase.py
--rw-rw-rw-   0 root         (0) root         (0)    10145 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/fpm/FPTree.py
--rw-rw-rw-   0 root         (0) root         (0)    18908 2024-04-10 09:51:41.000000 tui_dsmt-202404111315/src/tui_dsmt/fpm/HashTree.py
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-04-10 09:51:41.000000 tui_dsmt-202404111315/src/tui_dsmt/fpm/Itemset.py
--rw-rw-rw-   0 root         (0) root         (0)     3036 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/fpm/ItemsetGrid.py
--rw-rw-rw-   0 root         (0) root         (0)     5942 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/fpm/ItemsetGridApriori.py
--rw-rw-rw-   0 root         (0) root         (0)     5865 2024-04-11 12:11:46.000000 tui_dsmt-202404111315/src/tui_dsmt/fpm/ItemsetGridECLAT.py
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/fpm/SequentialDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)     1129 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/fpm/SequentialItemset.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/fpm/TransactionDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)   112120 2024-04-11 12:11:46.000000 tui_dsmt-202404111315/src/tui_dsmt/fpm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:15:46.405528 tui_dsmt-202404111315/src/tui_dsmt/graph/
--rw-rw-rw-   0 root         (0) root         (0)     3894 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/graph/BFS.py
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/graph/BipartiteFlow.py
--rw-rw-rw-   0 root         (0) root         (0)     3478 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/graph/DFS.py
--rw-rw-rw-   0 root         (0) root         (0)     5843 2024-04-10 09:51:41.000000 tui_dsmt-202404111315/src/tui_dsmt/graph/Dijkstra.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/graph/EdmondsKarp.py
--rw-rw-rw-   0 root         (0) root         (0)     4747 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/graph/FordFulkerson.py
--rw-rw-rw-   0 root         (0) root         (0)     4461 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/graph/Hall.py
--rw-rw-rw-   0 root         (0) root         (0)     2095 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/graph/InteractiveGraph.py
--rw-rw-rw-   0 root         (0) root         (0)     3142 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/graph/Kruskal.py
--rw-rw-rw-   0 root         (0) root         (0)     4877 2024-04-11 12:11:46.000000 tui_dsmt-202404111315/src/tui_dsmt/graph/LabelPropagation.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-11 12:11:46.000000 tui_dsmt-202404111315/src/tui_dsmt/graph/MarkovClusterAlgorithm.py
--rw-rw-rw-   0 root         (0) root         (0)     2234 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/graph/MaximumFlow.py
--rw-rw-rw-   0 root         (0) root         (0)     2705 2024-04-11 12:11:46.000000 tui_dsmt-202404111315/src/tui_dsmt/graph/RandomWalk.py
--rw-rw-rw-   0 root         (0) root         (0)   420228 2024-04-11 12:11:46.000000 tui_dsmt-202404111315/src/tui_dsmt/graph/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5267 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/graph/game.py
--rw-rw-rw-   0 root         (0) root         (0)     5539 2024-04-11 12:11:46.000000 tui_dsmt-202404111315/src/tui_dsmt/graph/html.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/graph/representation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:15:46.405528 tui_dsmt-202404111315/src/tui_dsmt/jpanim/
--rw-rw-rw-   0 root         (0) root         (0)     2576 2024-04-11 12:11:46.000000 tui_dsmt-202404111315/src/tui_dsmt/jpanim/JupyterAnimation.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-03-08 12:22:54.000000 tui_dsmt-202404111315/src/tui_dsmt/jpanim/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:15:46.405528 tui_dsmt-202404111315/src/tui_dsmt/util/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-10 09:51:41.000000 tui_dsmt-202404111315/src/tui_dsmt/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:15:46.409528 tui_dsmt-202404111315/src/tui_dsmt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      761 2024-04-11 13:15:46.000000 tui_dsmt-202404111315/src/tui_dsmt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1582 2024-04-11 13:15:46.000000 tui_dsmt-202404111315/src/tui_dsmt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 13:15:46.000000 tui_dsmt-202404111315/src/tui_dsmt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      118 2024-04-11 13:15:46.000000 tui_dsmt-202404111315/src/tui_dsmt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-11 13:15:46.000000 tui_dsmt-202404111315/src/tui_dsmt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 06:33:27.272922 tui_dsmt-202404160633/
+-rw-r--r--   0 root         (0) root         (0)      761 2024-04-16 06:33:27.272922 tui_dsmt-202404160633/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 06:33:27.272922 tui_dsmt-202404160633/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1101 2024-04-10 09:51:41.000000 tui_dsmt-202404160633/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 06:33:27.260922 tui_dsmt-202404160633/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 06:33:27.260922 tui_dsmt-202404160633/src/tui_dsmt/
+-rw-rw-rw-   0 root         (0) root         (0)      780 2024-04-16 06:33:20.000000 tui_dsmt-202404160633/src/tui_dsmt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 06:33:27.264922 tui_dsmt-202404160633/src/tui_dsmt/clustering/
+-rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-10 09:51:41.000000 tui_dsmt-202404160633/src/tui_dsmt/clustering/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2691 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/clustering/animation.py
+-rw-rw-rw-   0 root         (0) root         (0)    19108 2024-04-10 09:51:41.000000 tui_dsmt-202404160633/src/tui_dsmt/clustering/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)      260 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/clustering/draw.py
+-rw-rw-rw-   0 root         (0) root         (0)     1749 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/clustering/evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4488 2024-04-10 09:51:41.000000 tui_dsmt-202404160633/src/tui_dsmt/clustering/hierarchical.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/clustering/interactive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 06:33:27.268922 tui_dsmt-202404160633/src/tui_dsmt/fpm/
+-rw-rw-rw-   0 root         (0) root         (0)    14098 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/fpm/BruteForceFI.py
+-rw-rw-rw-   0 root         (0) root         (0)     4055 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/fpm/ConditionalFPTree.py
+-rw-rw-rw-   0 root         (0) root         (0)     5522 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/fpm/ConditionalPatternBase.py
+-rw-rw-rw-   0 root         (0) root         (0)    10145 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/fpm/FPTree.py
+-rw-rw-rw-   0 root         (0) root         (0)    18908 2024-04-10 09:51:41.000000 tui_dsmt-202404160633/src/tui_dsmt/fpm/HashTree.py
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-04-10 09:51:41.000000 tui_dsmt-202404160633/src/tui_dsmt/fpm/Itemset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/fpm/ItemsetGrid.py
+-rw-rw-rw-   0 root         (0) root         (0)     5942 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/fpm/ItemsetGridApriori.py
+-rw-rw-rw-   0 root         (0) root         (0)     5865 2024-04-16 06:33:20.000000 tui_dsmt-202404160633/src/tui_dsmt/fpm/ItemsetGridECLAT.py
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/fpm/SequentialDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/fpm/SequentialItemset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/fpm/TransactionDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)   112120 2024-04-16 06:33:20.000000 tui_dsmt-202404160633/src/tui_dsmt/fpm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 06:33:27.272922 tui_dsmt-202404160633/src/tui_dsmt/graph/
+-rw-rw-rw-   0 root         (0) root         (0)     3894 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/graph/BFS.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/graph/BipartiteFlow.py
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/graph/DFS.py
+-rw-rw-rw-   0 root         (0) root         (0)     5843 2024-04-10 09:51:41.000000 tui_dsmt-202404160633/src/tui_dsmt/graph/Dijkstra.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/graph/EdmondsKarp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4747 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/graph/FordFulkerson.py
+-rw-rw-rw-   0 root         (0) root         (0)     4461 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/graph/Hall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/graph/InteractiveGraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     3142 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/graph/Kruskal.py
+-rw-rw-rw-   0 root         (0) root         (0)     4877 2024-04-16 06:33:20.000000 tui_dsmt-202404160633/src/tui_dsmt/graph/LabelPropagation.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-16 06:33:20.000000 tui_dsmt-202404160633/src/tui_dsmt/graph/MarkovClusterAlgorithm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/graph/MaximumFlow.py
+-rw-rw-rw-   0 root         (0) root         (0)     2705 2024-04-16 06:33:20.000000 tui_dsmt-202404160633/src/tui_dsmt/graph/RandomWalk.py
+-rw-rw-rw-   0 root         (0) root         (0)   420228 2024-04-16 06:33:20.000000 tui_dsmt-202404160633/src/tui_dsmt/graph/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5267 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/graph/game.py
+-rw-rw-rw-   0 root         (0) root         (0)     5539 2024-04-16 06:33:20.000000 tui_dsmt-202404160633/src/tui_dsmt/graph/html.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/graph/representation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 06:33:27.272922 tui_dsmt-202404160633/src/tui_dsmt/jpanim/
+-rw-rw-rw-   0 root         (0) root         (0)     2576 2024-04-16 06:33:20.000000 tui_dsmt-202404160633/src/tui_dsmt/jpanim/JupyterAnimation.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-03-08 12:22:54.000000 tui_dsmt-202404160633/src/tui_dsmt/jpanim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 06:33:27.272922 tui_dsmt-202404160633/src/tui_dsmt/util/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-10 09:51:41.000000 tui_dsmt-202404160633/src/tui_dsmt/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 06:33:27.272922 tui_dsmt-202404160633/src/tui_dsmt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      761 2024-04-16 06:33:27.000000 tui_dsmt-202404160633/src/tui_dsmt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1582 2024-04-16 06:33:27.000000 tui_dsmt-202404160633/src/tui_dsmt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 06:33:27.000000 tui_dsmt-202404160633/src/tui_dsmt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2024-04-16 06:33:27.000000 tui_dsmt-202404160633/src/tui_dsmt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-16 06:33:27.000000 tui_dsmt-202404160633/src/tui_dsmt.egg-info/top_level.txt
```

### Comparing `tui_dsmt-202404111315/PKG-INFO` & `tui_dsmt-202404160633/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsmt
-Version: 202404111315
+Version: 202404160633
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-methoden-und-techniken
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tui_dsmt-202404111315/setup.py` & `tui_dsmt-202404160633/setup.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/__init__.py` & `tui_dsmt-202404160633/src/tui_dsmt/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/clustering/animation.py` & `tui_dsmt-202404160633/src/tui_dsmt/clustering/animation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/clustering/datasets.py` & `tui_dsmt-202404160633/src/tui_dsmt/clustering/datasets.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/clustering/evaluation.py` & `tui_dsmt-202404160633/src/tui_dsmt/clustering/evaluation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/clustering/hierarchical.py` & `tui_dsmt-202404160633/src/tui_dsmt/clustering/hierarchical.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/clustering/interactive.py` & `tui_dsmt-202404160633/src/tui_dsmt/clustering/interactive.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/fpm/BruteForceFI.py` & `tui_dsmt-202404160633/src/tui_dsmt/fpm/BruteForceFI.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/fpm/ConditionalFPTree.py` & `tui_dsmt-202404160633/src/tui_dsmt/fpm/ConditionalFPTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/fpm/ConditionalPatternBase.py` & `tui_dsmt-202404160633/src/tui_dsmt/fpm/ConditionalPatternBase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/fpm/FPTree.py` & `tui_dsmt-202404160633/src/tui_dsmt/fpm/FPTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/fpm/HashTree.py` & `tui_dsmt-202404160633/src/tui_dsmt/fpm/HashTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/fpm/Itemset.py` & `tui_dsmt-202404160633/src/tui_dsmt/fpm/Itemset.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/fpm/ItemsetGrid.py` & `tui_dsmt-202404160633/src/tui_dsmt/fpm/ItemsetGrid.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/fpm/ItemsetGridApriori.py` & `tui_dsmt-202404160633/src/tui_dsmt/fpm/ItemsetGridApriori.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/fpm/ItemsetGridECLAT.py` & `tui_dsmt-202404160633/src/tui_dsmt/fpm/ItemsetGridECLAT.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/fpm/SequentialDatabase.py` & `tui_dsmt-202404160633/src/tui_dsmt/fpm/SequentialDatabase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/fpm/SequentialItemset.py` & `tui_dsmt-202404160633/src/tui_dsmt/fpm/SequentialItemset.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/fpm/TransactionDatabase.py` & `tui_dsmt-202404160633/src/tui_dsmt/fpm/TransactionDatabase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/fpm/__init__.py` & `tui_dsmt-202404160633/src/tui_dsmt/fpm/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/graph/BFS.py` & `tui_dsmt-202404160633/src/tui_dsmt/graph/BFS.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/graph/BipartiteFlow.py` & `tui_dsmt-202404160633/src/tui_dsmt/graph/BipartiteFlow.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/graph/DFS.py` & `tui_dsmt-202404160633/src/tui_dsmt/graph/DFS.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/graph/Dijkstra.py` & `tui_dsmt-202404160633/src/tui_dsmt/graph/Dijkstra.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/graph/FordFulkerson.py` & `tui_dsmt-202404160633/src/tui_dsmt/graph/FordFulkerson.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/graph/Hall.py` & `tui_dsmt-202404160633/src/tui_dsmt/graph/Hall.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/graph/InteractiveGraph.py` & `tui_dsmt-202404160633/src/tui_dsmt/graph/InteractiveGraph.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/graph/Kruskal.py` & `tui_dsmt-202404160633/src/tui_dsmt/graph/Kruskal.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/graph/LabelPropagation.py` & `tui_dsmt-202404160633/src/tui_dsmt/graph/LabelPropagation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/graph/MaximumFlow.py` & `tui_dsmt-202404160633/src/tui_dsmt/graph/MaximumFlow.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/graph/RandomWalk.py` & `tui_dsmt-202404160633/src/tui_dsmt/graph/RandomWalk.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/graph/__init__.py` & `tui_dsmt-202404160633/src/tui_dsmt/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/graph/game.py` & `tui_dsmt-202404160633/src/tui_dsmt/graph/game.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/graph/html.py` & `tui_dsmt-202404160633/src/tui_dsmt/graph/html.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/graph/representation.py` & `tui_dsmt-202404160633/src/tui_dsmt/graph/representation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt/jpanim/JupyterAnimation.py` & `tui_dsmt-202404160633/src/tui_dsmt/jpanim/JupyterAnimation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404111315/src/tui_dsmt.egg-info/PKG-INFO` & `tui_dsmt-202404160633/src/tui_dsmt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsmt
-Version: 202404111315
+Version: 202404160633
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-methoden-und-techniken
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tui_dsmt-202404111315/src/tui_dsmt.egg-info/SOURCES.txt` & `tui_dsmt-202404160633/src/tui_dsmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

