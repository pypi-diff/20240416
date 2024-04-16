# Comparing `tmp/rwmapeditor_exgcdwu-1.2.0.tar.gz` & `tmp/rwmapeditor_exgcdwu-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwmapeditor_exgcdwu-1.2.0.tar", last modified: Sat Apr 13 10:38:07 2024, max compression
+gzip compressed data, was "rwmapeditor_exgcdwu-1.2.1.tar", last modified: Tue Apr 16 17:15:44 2024, max compression
```

## Comparing `rwmapeditor_exgcdwu-1.2.0.tar` & `rwmapeditor_exgcdwu-1.2.1.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:38:07.132845 rwmapeditor_exgcdwu-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-13 10:38:07.132845 rwmapeditor_exgcdwu-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:38:07.128845 rwmapeditor_exgcdwu-1.2.0/rwmap/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:38:07.128845 rwmapeditor_exgcdwu-1.2.0/rwmap/_case/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_case/_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_case/_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_case/_objectgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_case/_tileset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:38:07.128845 rwmapeditor_exgcdwu-1.2.0/rwmap/_frame/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_frame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_frame/_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_frame/_element_ori.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_frame/_element_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:38:07.128845 rwmapeditor_exgcdwu-1.2.0/rwmap/_object/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_object/_object_ori.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_object/_object_tile_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:38:07.128845 rwmapeditor_exgcdwu-1.2.0/rwmap/_tile/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_tile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_tile/_tile_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:38:07.132845 rwmapeditor_exgcdwu-1.2.0/rwmap/_util/
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_util/_class_rel.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_util/_dict_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_util/_etElement_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_util/_list_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_util/_png_rel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/_util/_str_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:38:07.132845 rwmapeditor_exgcdwu-1.2.0/rwmap/data/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/data/default_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:38:07.132845 rwmapeditor_exgcdwu-1.2.0/rwmap/data/tile_group_grid/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/data/tile_group_grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/data/tile_group_grid/_tile_group_addlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/data/tile_group_grid/_tile_group_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/data/tile_group_grid/tile_group_one.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:38:07.132845 rwmapeditor_exgcdwu-1.2.0/rwmap/data/tobject_group_COP/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/rwmap/data/tobject_group_COP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:38:07.132845 rwmapeditor_exgcdwu-1.2.0/rwmapeditor_exgcdwu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-13 10:38:07.000000 rwmapeditor_exgcdwu-1.2.0/rwmapeditor_exgcdwu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-13 10:38:07.000000 rwmapeditor_exgcdwu-1.2.0/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 10:38:07.000000 rwmapeditor_exgcdwu-1.2.0/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-13 10:38:07.000000 rwmapeditor_exgcdwu-1.2.0/rwmapeditor_exgcdwu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-13 10:38:07.132845 rwmapeditor_exgcdwu-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-13 10:37:50.000000 rwmapeditor_exgcdwu-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:15:44.772176 rwmapeditor_exgcdwu-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-16 17:15:44.772176 rwmapeditor_exgcdwu-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:15:44.768175 rwmapeditor_exgcdwu-1.2.1/rwmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:15:44.768175 rwmapeditor_exgcdwu-1.2.1/rwmap/_case/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/_case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/_case/_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/_case/_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/_case/_objectgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/_case/_tileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:15:44.768175 rwmapeditor_exgcdwu-1.2.1/rwmap/_frame/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/_frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/_frame/_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/_frame/_element_ori.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/_frame/_element_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:15:44.768175 rwmapeditor_exgcdwu-1.2.1/rwmap/_object/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/_object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/_object/_object_ori.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/_object/_object_tile_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:15:44.768175 rwmapeditor_exgcdwu-1.2.1/rwmap/_tile/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/_tile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/_tile/_tile_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:15:44.772176 rwmapeditor_exgcdwu-1.2.1/rwmap/_util/
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/_util/_class_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/_util/_dict_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/_util/_etElement_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/_util/_list_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/_util/_png_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/_util/_str_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:15:44.772176 rwmapeditor_exgcdwu-1.2.1/rwmap/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/data/default_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:15:44.772176 rwmapeditor_exgcdwu-1.2.1/rwmap/data/tile_group_grid/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/data/tile_group_grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/data/tile_group_grid/_tile_group_addlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/data/tile_group_grid/_tile_group_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/data/tile_group_grid/tile_group_one.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:15:44.772176 rwmapeditor_exgcdwu-1.2.1/rwmap/data/tobject_group_COP/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/rwmap/data/tobject_group_COP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:15:44.772176 rwmapeditor_exgcdwu-1.2.1/rwmapeditor_exgcdwu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-16 17:15:44.000000 rwmapeditor_exgcdwu-1.2.1/rwmapeditor_exgcdwu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-16 17:15:44.000000 rwmapeditor_exgcdwu-1.2.1/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:15:44.000000 rwmapeditor_exgcdwu-1.2.1/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 17:15:44.000000 rwmapeditor_exgcdwu-1.2.1/rwmapeditor_exgcdwu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 17:15:44.000000 rwmapeditor_exgcdwu-1.2.1/rwmapeditor_exgcdwu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-16 17:15:44.776176 rwmapeditor_exgcdwu-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-16 17:15:38.000000 rwmapeditor_exgcdwu-1.2.1/setup.py
```

### Comparing `rwmapeditor_exgcdwu-1.2.0/LICENSE` & `rwmapeditor_exgcdwu-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.0/PKG-INFO` & `rwmapeditor_exgcdwu-1.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: rwmapeditor_exgcdwu
-Version: 1.2.0
+Version: 1.2.1
 Home-page: https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-
 Author: exgcdwu
 Author-email: 1006605318@qq.com
+License: GPL-3.0
 Requires-Python: >=3.0.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
 
 # rwmapeditor-exgcdwu
 ___一个铁锈战争 (Rusted Warfare) 地图编辑 python 库___
 
 ![released version](https://img.shields.io/pypi/v/rwmapeditor-exgcdwu.svg)
 
 ## 目标
@@ -43,18 +45,19 @@
 
 ## 简易使用例子
 
 ```python
 # coding: utf-8
 import rwmap as rw
 
-map_dir = 'D:/Game/steam/steamapps/common/Rusted Warfare/mods/maps/'
+rwmap_dir = 'D:/Game/steam/steamapps/common/Rusted Warfare/mods/maps/'
+youmap_dir = 'D:/Game/steam/steamapps/common/Rusted Warfare/mods/maps/'
 map_name = '[p2]example_skirmish_(2p).tmx'
 map_name_out = '[p2]example_skirmish_(2p)(1).tmx'
-mygraph:rw.RWmap = rw.RWmap.init_mapfile(map_dir + map_name, map_dir)
+mygraph:rw.RWmap = rw.RWmap.init_mapfile(youmap_dir + map_name, rwmap_dir)
 print(mygraph)
 
 mygraph.addObject(
     "Triggers", 
     {"id": "100", "name": "刷兵实验", "type": "unitAdd", "x": "1500", "y":"1000", "width": "20", "height": "20"}, 
     {"resetActivationAfter":"5s", "spawnUnits": "heavyTank*10", "team" :"0", "warmup":"5s"})
 
@@ -62,13 +65,13 @@
 mygraph.addTile("Ground", rw.Coordinate(2, 0), "Long Grass", rw.Coordinate(0, 0))
 mygraph.addTile("Ground", rw.Coordinate(0, 1), "Long Grass", rw.Coordinate(0, 0))
 
 mygraph.addTile_square("Ground", rw.Rectangle(rw.Coordinate(5, 5), rw.Coordinate(10, 10)), "Deep Water", rw.Coordinate(0, 0))
 
 mygraph.addTile_group(rw.Coordinate(5, 20), rw.data.tile_group_grid.fill_tile_group_one_ground_water_28_24)
 
-mygraph.write_file(map_dir + map_name_out)
+mygraph.write_file(youmap_dir + map_name_out)
 
 ```
```

### Comparing `rwmapeditor_exgcdwu-1.2.0/README.md` & `rwmapeditor_exgcdwu-1.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -33,18 +33,19 @@
 
 ## 简易使用例子
 
 ```python
 # coding: utf-8
 import rwmap as rw
 
-map_dir = 'D:/Game/steam/steamapps/common/Rusted Warfare/mods/maps/'
+rwmap_dir = 'D:/Game/steam/steamapps/common/Rusted Warfare/mods/maps/'
+youmap_dir = 'D:/Game/steam/steamapps/common/Rusted Warfare/mods/maps/'
 map_name = '[p2]example_skirmish_(2p).tmx'
 map_name_out = '[p2]example_skirmish_(2p)(1).tmx'
-mygraph:rw.RWmap = rw.RWmap.init_mapfile(map_dir + map_name, map_dir)
+mygraph:rw.RWmap = rw.RWmap.init_mapfile(youmap_dir + map_name, rwmap_dir)
 print(mygraph)
 
 mygraph.addObject(
     "Triggers", 
     {"id": "100", "name": "刷兵实验", "type": "unitAdd", "x": "1500", "y":"1000", "width": "20", "height": "20"}, 
     {"resetActivationAfter":"5s", "spawnUnits": "heavyTank*10", "team" :"0", "warmup":"5s"})
 
@@ -52,13 +53,13 @@
 mygraph.addTile("Ground", rw.Coordinate(2, 0), "Long Grass", rw.Coordinate(0, 0))
 mygraph.addTile("Ground", rw.Coordinate(0, 1), "Long Grass", rw.Coordinate(0, 0))
 
 mygraph.addTile_square("Ground", rw.Rectangle(rw.Coordinate(5, 5), rw.Coordinate(10, 10)), "Deep Water", rw.Coordinate(0, 0))
 
 mygraph.addTile_group(rw.Coordinate(5, 20), rw.data.tile_group_grid.fill_tile_group_one_ground_water_28_24)
 
-mygraph.write_file(map_dir + map_name_out)
+mygraph.write_file(youmap_dir + map_name_out)
 
 ```
```

### Comparing `rwmapeditor_exgcdwu-1.2.0/rwmap/_case/_layer.py` & `rwmapeditor_exgcdwu-1.2.1/rwmap/_case/_layer.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.0/rwmap/_case/_object.py` & `rwmapeditor_exgcdwu-1.2.1/rwmap/_case/_object.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.0/rwmap/_case/_objectgroup.py` & `rwmapeditor_exgcdwu-1.2.1/rwmap/_case/_objectgroup.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.0/rwmap/_case/_tileset.py` & `rwmapeditor_exgcdwu-1.2.1/rwmap/_case/_tileset.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.0/rwmap/_core.py` & `rwmapeditor_exgcdwu-1.2.1/rwmap/_core.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.0/rwmap/_frame/_coordinate.py` & `rwmapeditor_exgcdwu-1.2.1/rwmap/_frame/_coordinate.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.0/rwmap/_frame/_element_property.py` & `rwmapeditor_exgcdwu-1.2.1/rwmap/_frame/_element_property.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.0/rwmap/_tile/_tile_group.py` & `rwmapeditor_exgcdwu-1.2.1/rwmap/_tile/_tile_group.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.0/rwmap/_util/__init__.py` & `rwmapeditor_exgcdwu-1.2.1/rwmap/_util/__init__.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.0/rwmap/_util/_etElement_process.py` & `rwmapeditor_exgcdwu-1.2.1/rwmap/_util/_etElement_process.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.0/rwmap/_util/_str_util.py` & `rwmapeditor_exgcdwu-1.2.1/rwmap/_util/_str_util.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.0/rwmapeditor_exgcdwu.egg-info/PKG-INFO` & `rwmapeditor_exgcdwu-1.2.1/rwmapeditor_exgcdwu.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: rwmapeditor_exgcdwu
-Version: 1.2.0
+Version: 1.2.1
 Home-page: https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-
 Author: exgcdwu
 Author-email: 1006605318@qq.com
+License: GPL-3.0
 Requires-Python: >=3.0.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
 
 # rwmapeditor-exgcdwu
 ___一个铁锈战争 (Rusted Warfare) 地图编辑 python 库___
 
 ![released version](https://img.shields.io/pypi/v/rwmapeditor-exgcdwu.svg)
 
 ## 目标
@@ -43,18 +45,19 @@
 
 ## 简易使用例子
 
 ```python
 # coding: utf-8
 import rwmap as rw
 
-map_dir = 'D:/Game/steam/steamapps/common/Rusted Warfare/mods/maps/'
+rwmap_dir = 'D:/Game/steam/steamapps/common/Rusted Warfare/mods/maps/'
+youmap_dir = 'D:/Game/steam/steamapps/common/Rusted Warfare/mods/maps/'
 map_name = '[p2]example_skirmish_(2p).tmx'
 map_name_out = '[p2]example_skirmish_(2p)(1).tmx'
-mygraph:rw.RWmap = rw.RWmap.init_mapfile(map_dir + map_name, map_dir)
+mygraph:rw.RWmap = rw.RWmap.init_mapfile(youmap_dir + map_name, rwmap_dir)
 print(mygraph)
 
 mygraph.addObject(
     "Triggers", 
     {"id": "100", "name": "刷兵实验", "type": "unitAdd", "x": "1500", "y":"1000", "width": "20", "height": "20"}, 
     {"resetActivationAfter":"5s", "spawnUnits": "heavyTank*10", "team" :"0", "warmup":"5s"})
 
@@ -62,13 +65,13 @@
 mygraph.addTile("Ground", rw.Coordinate(2, 0), "Long Grass", rw.Coordinate(0, 0))
 mygraph.addTile("Ground", rw.Coordinate(0, 1), "Long Grass", rw.Coordinate(0, 0))
 
 mygraph.addTile_square("Ground", rw.Rectangle(rw.Coordinate(5, 5), rw.Coordinate(10, 10)), "Deep Water", rw.Coordinate(0, 0))
 
 mygraph.addTile_group(rw.Coordinate(5, 20), rw.data.tile_group_grid.fill_tile_group_one_ground_water_28_24)
 
-mygraph.write_file(map_dir + map_name_out)
+mygraph.write_file(youmap_dir + map_name_out)
 
 ```
```

### Comparing `rwmapeditor_exgcdwu-1.2.0/rwmapeditor_exgcdwu.egg-info/SOURCES.txt` & `rwmapeditor_exgcdwu-1.2.1/rwmapeditor_exgcdwu.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -32,8 +32,9 @@
 rwmap/data/tile_group_grid/_tile_group_addlayer.py
 rwmap/data/tile_group_grid/_tile_group_matrix.py
 rwmap/data/tile_group_grid/tile_group_one.py
 rwmap/data/tobject_group_COP/__init__.py
 rwmapeditor_exgcdwu.egg-info/PKG-INFO
 rwmapeditor_exgcdwu.egg-info/SOURCES.txt
 rwmapeditor_exgcdwu.egg-info/dependency_links.txt
+rwmapeditor_exgcdwu.egg-info/requires.txt
 rwmapeditor_exgcdwu.egg-info/top_level.txt
```

### Comparing `rwmapeditor_exgcdwu-1.2.0/setup.py` & `rwmapeditor_exgcdwu-1.2.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # setup.py
 
-#import os
+import os
 from setuptools import setup, find_packages
 
-__version__ = '1.2.0'
-#current_dir = os.path.dirname(__file__)
-#requirements = open(current_dir + '/requirements.txt').readlines()
+__version__ = '1.2.1'
+current_dir = os.path.dirname(__file__)
+
 
 def readme():
     with open('README.md') as file:
         return file.read()
 
-strreadme = readme()
+def requirements():
+    with open('requirements.txt') as file:
+        return file.readlines()
 
 setup(
     name = 'rwmapeditor_exgcdwu',
     version = __version__,
     author = 'exgcdwu',
     author_email = '1006605318@qq.com',
+    license = 'GPL-3.0',
     url = "https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-",
-    long_description = strreadme,
+    long_description = readme(),
     long_description_content_type = "text/markdown",
     packages = find_packages(exclude=["tests"]),
-    python_requires = '>=3.0.0'
-    #,install_requires = requirements
-)
+    #package_data = {current_dir: [f'{current_dir}/*.txt']},
+    python_requires = '>=3.0.0',
+    install_requires = ['numpy']#requirements()
+)
```

