# Comparing `tmp/superblockify-1.0.0rc4.tar.gz` & `tmp/superblockify-1.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superblockify-1.0.0rc4.tar", last modified: Tue Apr  9 15:06:39 2024, max compression
+gzip compressed data, was "superblockify-1.0.0rc5.tar", last modified: Tue Apr 16 10:15:03 2024, max compression
```

## Comparing `superblockify-1.0.0rc4.tar` & `superblockify-1.0.0rc5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 15:06:39.879050 superblockify-1.0.0rc4/
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    34523 2024-03-25 08:40:49.000000 superblockify-1.0.0rc4/LICENSE
--rw-r--r--   0 carlsonb  (1000) carlsonb  (1000)     5430 2024-04-09 15:06:39.879050 superblockify-1.0.0rc4/PKG-INFO
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     3154 2024-04-09 10:03:29.000000 superblockify-1.0.0rc4/README.md
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     4595 2024-04-09 15:02:00.000000 superblockify-1.0.0rc4/pyproject.toml
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)       38 2024-04-09 15:06:39.879050 superblockify-1.0.0rc4/setup.cfg
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 15:06:39.875050 superblockify-1.0.0rc4/superblockify/
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      443 2024-04-08 20:10:55.000000 superblockify-1.0.0rc4/superblockify/__init__.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1153 2023-06-27 21:08:28.000000 superblockify-1.0.0rc4/superblockify/_api.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)       63 2024-04-09 15:05:39.000000 superblockify-1.0.0rc4/superblockify/_version.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     9072 2023-06-23 06:47:12.000000 superblockify-1.0.0rc4/superblockify/attribute.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     6298 2024-04-09 13:42:49.000000 superblockify-1.0.0rc4/superblockify/config.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     4592 2024-04-08 20:10:55.000000 superblockify-1.0.0rc4/superblockify/graph_stats.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      785 2024-03-25 08:40:43.000000 superblockify-1.0.0rc4/superblockify/logging.cfg
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 15:06:39.875050 superblockify-1.0.0rc4/superblockify/metrics/
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      272 2023-04-21 06:51:36.000000 superblockify-1.0.0rc4/superblockify/metrics/__init__.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    27220 2024-04-08 21:02:38.000000 superblockify-1.0.0rc4/superblockify/metrics/distances.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    29000 2024-03-25 08:40:43.000000 superblockify-1.0.0rc4/superblockify/metrics/measures.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    21147 2024-04-08 20:10:55.000000 superblockify-1.0.0rc4/superblockify/metrics/metric.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    16173 2024-03-25 08:40:43.000000 superblockify-1.0.0rc4/superblockify/metrics/plot.py
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 15:06:39.875050 superblockify-1.0.0rc4/superblockify/partitioning/
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      893 2024-03-25 08:40:43.000000 superblockify-1.0.0rc4/superblockify/partitioning/__init__.py
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 15:06:39.879050 superblockify-1.0.0rc4/superblockify/partitioning/approaches/
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      279 2024-03-25 08:40:43.000000 superblockify-1.0.0rc4/superblockify/partitioning/approaches/__init__.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     2672 2024-03-25 08:40:43.000000 superblockify-1.0.0rc4/superblockify/partitioning/approaches/attribute.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    30020 2024-04-08 20:10:55.000000 superblockify-1.0.0rc4/superblockify/partitioning/approaches/bearing.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     3988 2024-03-25 08:40:43.000000 superblockify-1.0.0rc4/superblockify/partitioning/approaches/betweenness.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1826 2024-03-25 08:40:43.000000 superblockify-1.0.0rc4/superblockify/partitioning/approaches/dummy.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     8957 2024-03-25 08:40:43.000000 superblockify-1.0.0rc4/superblockify/partitioning/approaches/steiner_tree.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1445 2023-05-22 07:49:38.000000 superblockify-1.0.0rc4/superblockify/partitioning/approaches/streettype.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    40980 2024-04-08 20:11:26.000000 superblockify-1.0.0rc4/superblockify/partitioning/base.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    10319 2024-04-08 20:10:55.000000 superblockify-1.0.0rc4/superblockify/partitioning/checks.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    11867 2024-04-08 20:10:55.000000 superblockify-1.0.0rc4/superblockify/partitioning/plot.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     2502 2024-03-25 08:40:43.000000 superblockify-1.0.0rc4/superblockify/partitioning/representative.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1914 2024-04-08 20:10:55.000000 superblockify-1.0.0rc4/superblockify/partitioning/speed.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    25005 2024-03-25 08:40:43.000000 superblockify-1.0.0rc4/superblockify/partitioning/utils.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    21795 2024-04-08 13:58:15.000000 superblockify-1.0.0rc4/superblockify/plot.py
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 15:06:39.879050 superblockify-1.0.0rc4/superblockify/population/
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      276 2024-03-25 08:40:43.000000 superblockify-1.0.0rc4/superblockify/population/__init__.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    12827 2024-03-25 08:40:43.000000 superblockify-1.0.0rc4/superblockify/population/approximation.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    10670 2024-04-08 20:10:55.000000 superblockify-1.0.0rc4/superblockify/population/ghsl.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    10445 2024-03-25 08:40:43.000000 superblockify-1.0.0rc4/superblockify/population/tessellation.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    14351 2024-04-08 20:10:55.000000 superblockify-1.0.0rc4/superblockify/utils.py
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 15:06:39.879050 superblockify-1.0.0rc4/superblockify.egg-info/
--rw-r--r--   0 carlsonb  (1000) carlsonb  (1000)     5430 2024-04-09 15:06:39.000000 superblockify-1.0.0rc4/superblockify.egg-info/PKG-INFO
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1467 2024-04-09 15:06:39.000000 superblockify-1.0.0rc4/superblockify.egg-info/SOURCES.txt
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)        1 2024-04-09 15:06:39.000000 superblockify-1.0.0rc4/superblockify.egg-info/dependency_links.txt
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      264 2024-04-09 15:06:39.000000 superblockify-1.0.0rc4/superblockify.egg-info/requires.txt
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)       14 2024-04-09 15:06:39.000000 superblockify-1.0.0rc4/superblockify.egg-info/top_level.txt
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 15:06:39.879050 superblockify-1.0.0rc4/tests/
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     7641 2024-03-25 08:40:43.000000 superblockify-1.0.0rc4/tests/test_attribute.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     3345 2024-03-25 08:40:43.000000 superblockify-1.0.0rc4/tests/test_graph_stats.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     6980 2024-04-08 20:10:55.000000 superblockify-1.0.0rc4/tests/test_plot.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    11491 2024-04-08 20:10:55.000000 superblockify-1.0.0rc4/tests/test_utils.py
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-16 10:15:03.441954 superblockify-1.0.0rc5/
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    34523 2024-03-25 08:40:49.000000 superblockify-1.0.0rc5/LICENSE
+-rw-r--r--   0 carlsonb  (1000) carlsonb  (1000)     5984 2024-04-16 10:15:03.441954 superblockify-1.0.0rc5/PKG-INFO
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     3551 2024-04-16 10:06:49.000000 superblockify-1.0.0rc5/README.md
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     4733 2024-04-16 10:14:04.000000 superblockify-1.0.0rc5/pyproject.toml
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)       38 2024-04-16 10:15:03.441954 superblockify-1.0.0rc5/setup.cfg
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-16 10:15:03.197953 superblockify-1.0.0rc5/superblockify/
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      443 2024-04-08 20:10:55.000000 superblockify-1.0.0rc5/superblockify/__init__.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1153 2023-06-27 21:08:28.000000 superblockify-1.0.0rc5/superblockify/_api.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)       63 2024-04-16 10:10:49.000000 superblockify-1.0.0rc5/superblockify/_version.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     9072 2023-06-23 06:47:12.000000 superblockify-1.0.0rc5/superblockify/attribute.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     6240 2024-04-16 10:11:16.000000 superblockify-1.0.0rc5/superblockify/config.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     4592 2024-04-08 20:10:55.000000 superblockify-1.0.0rc5/superblockify/graph_stats.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      782 2024-04-16 09:34:18.000000 superblockify-1.0.0rc5/superblockify/logging.cfg
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-16 10:15:03.265953 superblockify-1.0.0rc5/superblockify/metrics/
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      272 2023-04-21 06:51:36.000000 superblockify-1.0.0rc5/superblockify/metrics/__init__.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    27220 2024-04-08 21:02:38.000000 superblockify-1.0.0rc5/superblockify/metrics/distances.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    29000 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/metrics/measures.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    21147 2024-04-08 20:10:55.000000 superblockify-1.0.0rc5/superblockify/metrics/metric.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    16173 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/metrics/plot.py
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-16 10:15:03.333953 superblockify-1.0.0rc5/superblockify/partitioning/
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      893 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/partitioning/__init__.py
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-16 10:15:03.333953 superblockify-1.0.0rc5/superblockify/partitioning/approaches/
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      279 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/partitioning/approaches/__init__.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     2672 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/partitioning/approaches/attribute.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    30020 2024-04-08 20:10:55.000000 superblockify-1.0.0rc5/superblockify/partitioning/approaches/bearing.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     3988 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/partitioning/approaches/betweenness.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1826 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/partitioning/approaches/dummy.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     8957 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/partitioning/approaches/steiner_tree.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1445 2023-05-22 07:49:38.000000 superblockify-1.0.0rc5/superblockify/partitioning/approaches/streettype.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    40014 2024-04-16 09:32:16.000000 superblockify-1.0.0rc5/superblockify/partitioning/base.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    10319 2024-04-08 20:10:55.000000 superblockify-1.0.0rc5/superblockify/partitioning/checks.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    11867 2024-04-08 20:10:55.000000 superblockify-1.0.0rc5/superblockify/partitioning/plot.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     2502 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/partitioning/representative.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1914 2024-04-08 20:10:55.000000 superblockify-1.0.0rc5/superblockify/partitioning/speed.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    25005 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/partitioning/utils.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    21795 2024-04-08 13:58:15.000000 superblockify-1.0.0rc5/superblockify/plot.py
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-16 10:15:03.389954 superblockify-1.0.0rc5/superblockify/population/
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      276 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/population/__init__.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    12827 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/population/approximation.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    10670 2024-04-08 20:10:55.000000 superblockify-1.0.0rc5/superblockify/population/ghsl.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    10445 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/superblockify/population/tessellation.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    14351 2024-04-08 20:10:55.000000 superblockify-1.0.0rc5/superblockify/utils.py
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-16 10:15:03.441954 superblockify-1.0.0rc5/superblockify.egg-info/
+-rw-r--r--   0 carlsonb  (1000) carlsonb  (1000)     5984 2024-04-16 10:15:03.000000 superblockify-1.0.0rc5/superblockify.egg-info/PKG-INFO
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1467 2024-04-16 10:15:03.000000 superblockify-1.0.0rc5/superblockify.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)        1 2024-04-16 10:15:03.000000 superblockify-1.0.0rc5/superblockify.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      282 2024-04-16 10:15:03.000000 superblockify-1.0.0rc5/superblockify.egg-info/requires.txt
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)       14 2024-04-16 10:15:03.000000 superblockify-1.0.0rc5/superblockify.egg-info/top_level.txt
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-16 10:15:03.429954 superblockify-1.0.0rc5/tests/
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     7641 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/tests/test_attribute.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     3345 2024-03-25 08:40:43.000000 superblockify-1.0.0rc5/tests/test_graph_stats.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     6980 2024-04-08 20:10:55.000000 superblockify-1.0.0rc5/tests/test_plot.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    11491 2024-04-08 20:10:55.000000 superblockify-1.0.0rc5/tests/test_utils.py
```

### Comparing `superblockify-1.0.0rc4/LICENSE` & `superblockify-1.0.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/PKG-INFO` & `superblockify-1.0.0rc5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: superblockify
-Version: 1.0.0rc4
+Version: 1.0.0rc5
 Summary: Automated Generation, Visualization, and Analysis of potential Superblocks in Cities
 Author-email: Carlson Büth <carlson@cbueth.de>
 Maintainer: superblockify contributors
-License: APGL-3.0
+License: APGL-3.0-or-later
 Project-URL: Documentation, https://NERDSITU.github.io/superblockify
 Project-URL: Repository, https://github.com/NERDSITU/superblockify
 Project-URL: Changelog, https://NERDSITU.github.io/superblockify/changelog/
 Keywords: Low Traffic Neighborhoods,GIS,Networks,OpenStreetMap,Urban Planning,Urban Mobility,Urban Data
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -33,14 +35,15 @@
 Requires-Dist: numba
 Requires-Dist: tqdm
 Requires-Dist: contextily
 Requires-Dist: ruamel.yaml
 Requires-Dist: pyarrow
 Requires-Dist: seaborn
 Requires-Dist: psutil
+Requires-Dist: typing-extensions
 Provides-Extra: lint
 Requires-Dist: blackd; extra == "lint"
 Requires-Dist: isort; extra == "lint"
 Requires-Dist: pylint; extra == "lint"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
@@ -51,53 +54,57 @@
 Requires-Dist: myst-nb; extra == "doc"
 Requires-Dist: sphinx-book-theme; extra == "doc"
 Requires-Dist: rasterstats; extra == "doc"
 Requires-Dist: momepy; extra == "doc"
 Provides-Extra: all
 Requires-Dist: superblockify[doc,lint,test]; extra == "all"
 
-# `superblockify`
+# superblockify
 
 [![Dev](https://img.shields.io/badge/docs-dev-blue.svg)](https://NERDSITU.github.io/superblockify/)
-[![codecov](https://codecov.io/gh/NERDSITU/superblockify/branch/main/graph/badge.svg?token=AS72IFT2Q4)](https://codecov.io/gh/NERDSITU/superblockify)
+[![PyPI Version](https://badge.fury.io/py/superblockify.svg)](https://pypi.org/project/superblockify/)
+[![Python Version](https://img.shields.io/pypi/pyversions/superblockify)](https://pypi.org/project/superblockify/)
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PyPI License](https://img.shields.io/pypi/l/superblockify)](https://pypi.org/project/superblockify/)
 
 [![Docs](https://github.com/NERDSITU/superblockify/actions/workflows/docs.yml/badge.svg)](https://github.com/NERDSITU/superblockify/actions/workflows/docs.yml)
 [![Lint](https://github.com/NERDSITU/superblockify/actions/workflows/lint.yml/badge.svg)](https://github.com/NERDSITU/superblockify/actions/workflows/lint.yml)
 [![Test](https://github.com/NERDSITU/superblockify/actions/workflows/test.yml/badge.svg)](https://github.com/NERDSITU/superblockify/actions/workflows/test.yml)
+[![codecov](https://codecov.io/gh/NERDSITU/superblockify/branch/main/graph/badge.svg?token=AS72IFT2Q4)](https://codecov.io/gh/NERDSITU/superblockify)
 
 Source code for blockifying existing street networks.
 
 ---
 
 ## Installation
 
-Create a new environment with `conda` or `mamba` and install the package from the
-`conda-forge` channel.
+We recommend using `micromamba` to create a virtual
+environment and installing the package in editable mode.
+Alternatively, one can use `conda` or `mamba` to create the environment
+(they can be used interchangeably).
+After cloning the repository, navigate to the root folder and
+create the environment with the wished python version and the development dependencies.
 
 ```bash
-conda create -n sb_env -c conda-forge superblockify
-conda activate sb_env
+micromamba create -n sb_env -c conda-forge python=3.12 osmnx
+micromamba activate sb_env
+pip install superblockify
 ```
 
 This installs the package and its dependencies,
 ready for use when activating the environment.
 Learn more about `superblockify` by reading
 the [documentation](https://NERDSITU.github.io/superblockify/)
 or
 the [minimal working example](https://github.com/NERDSITU/superblockify/blob/main/scripts/examples/mwe.py).
 
 ## Development Setup
 
-For development, we recommend using `micromamba` to create a virtual
-environment and installing the package in editable mode.
-Alternatively, one can use `conda` or `mamba` to create the environment
-(they can be used interchangeably).
-After cloning the repository, navigate to the root folder and
+For development, clone the repository, navigate to the root folder and
 create the environment with the wished python version and the development dependencies.
 
 ```bash
 micromamba create -n sb_env -c conda-forge python=3.12 --file=environment.yml
 micromamba activate sb_env
 ```
```

### Comparing `superblockify-1.0.0rc4/README.md` & `superblockify-1.0.0rc5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,50 @@
-# `superblockify`
+# superblockify
 
 [![Dev](https://img.shields.io/badge/docs-dev-blue.svg)](https://NERDSITU.github.io/superblockify/)
-[![codecov](https://codecov.io/gh/NERDSITU/superblockify/branch/main/graph/badge.svg?token=AS72IFT2Q4)](https://codecov.io/gh/NERDSITU/superblockify)
+[![PyPI Version](https://badge.fury.io/py/superblockify.svg)](https://pypi.org/project/superblockify/)
+[![Python Version](https://img.shields.io/pypi/pyversions/superblockify)](https://pypi.org/project/superblockify/)
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PyPI License](https://img.shields.io/pypi/l/superblockify)](https://pypi.org/project/superblockify/)
 
 [![Docs](https://github.com/NERDSITU/superblockify/actions/workflows/docs.yml/badge.svg)](https://github.com/NERDSITU/superblockify/actions/workflows/docs.yml)
 [![Lint](https://github.com/NERDSITU/superblockify/actions/workflows/lint.yml/badge.svg)](https://github.com/NERDSITU/superblockify/actions/workflows/lint.yml)
 [![Test](https://github.com/NERDSITU/superblockify/actions/workflows/test.yml/badge.svg)](https://github.com/NERDSITU/superblockify/actions/workflows/test.yml)
+[![codecov](https://codecov.io/gh/NERDSITU/superblockify/branch/main/graph/badge.svg?token=AS72IFT2Q4)](https://codecov.io/gh/NERDSITU/superblockify)
 
 Source code for blockifying existing street networks.
 
 ---
 
 ## Installation
 
-Create a new environment with `conda` or `mamba` and install the package from the
-`conda-forge` channel.
+We recommend using `micromamba` to create a virtual
+environment and installing the package in editable mode.
+Alternatively, one can use `conda` or `mamba` to create the environment
+(they can be used interchangeably).
+After cloning the repository, navigate to the root folder and
+create the environment with the wished python version and the development dependencies.
 
 ```bash
-conda create -n sb_env -c conda-forge superblockify
-conda activate sb_env
+micromamba create -n sb_env -c conda-forge python=3.12 osmnx
+micromamba activate sb_env
+pip install superblockify
 ```
 
 This installs the package and its dependencies,
 ready for use when activating the environment.
 Learn more about `superblockify` by reading
 the [documentation](https://NERDSITU.github.io/superblockify/)
 or
 the [minimal working example](https://github.com/NERDSITU/superblockify/blob/main/scripts/examples/mwe.py).
 
 ## Development Setup
 
-For development, we recommend using `micromamba` to create a virtual
-environment and installing the package in editable mode.
-Alternatively, one can use `conda` or `mamba` to create the environment
-(they can be used interchangeably).
-After cloning the repository, navigate to the root folder and
+For development, clone the repository, navigate to the root folder and
 create the environment with the wished python version and the development dependencies.
 
 ```bash
 micromamba create -n sb_env -c conda-forge python=3.12 --file=environment.yml
 micromamba activate sb_env
 ```
```

### Comparing `superblockify-1.0.0rc4/pyproject.toml` & `superblockify-1.0.0rc5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "superblockify"
 authors = [{ name = "Carlson Büth", email = "carlson@cbueth.de" }]
 maintainers = [{ name = "superblockify contributors" }]
-license = { text = "APGL-3.0" }
+license = { text = "APGL-3.0-or-later" }
 readme = "README.md"
 description = "Automated Generation, Visualization, and Analysis of potential Superblocks in Cities"
 keywords = ["Low Traffic Neighborhoods", "GIS", "Networks", "OpenStreetMap", "Urban Planning", "Urban Mobility", "Urban Data"]
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Natural Language :: English",
     "Topic :: Scientific/Engineering :: GIS",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: Scientific/Engineering :: Physics",
 ]
 dynamic = ["version"]
@@ -36,14 +38,15 @@
     "numba",
     "tqdm",
     "contextily",
     "ruamel.yaml",
     "pyarrow",
     "seaborn",
     "psutil",
+    "typing-extensions",
 ]
 
 [project.urls]
 Documentation = "https://NERDSITU.github.io/superblockify"
 Repository = "https://github.com/NERDSITU/superblockify"
 Changelog = "https://NERDSITU.github.io/superblockify/changelog/"
 
@@ -145,8 +148,8 @@
 [tool.handlers.RotatingFileHandler]
 class = "logging.handlers.RotatingFileHandler"
 level = "DEBUG"
 formatter = "simpleFormatter"
 args = "('superblockify.log', 'w+', 1e6, 3)"
 
 [tool.formatters.simpleFormatter]
-format = "%(asctime)s | %(levelname)8s | %(filename)s:%(lineno)d | %(message)s"
+format = "%(asctime)s | %(levelname)8s | %(filename)s:%(lineno)d | %(message)s"
```

### Comparing `superblockify-1.0.0rc4/superblockify/_api.py` & `superblockify-1.0.0rc5/superblockify/_api.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify/attribute.py` & `superblockify-1.0.0rc5/superblockify/attribute.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify/config.py` & `superblockify-1.0.0rc5/superblockify/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,17 @@
     )
 
     # Metrics
     CLUSTERING_PERCENTILE = 90
     NUM_BINS = 36
 
     # Population data (GHSL)
-    FULL_RASTER = join(GHSL_DIR, "GHS_POP_E2025_GLOBE_R2023A_54009_100_V1_0.tif")
+    FULL_RASTER = (
+        None  # join(GHSL_DIR, "GHS_POP_E2025_GLOBE_R2023A_54009_100_V1_0.tif")
+    )
     DOWNLOAD_TIMEOUT = 60
 
     # Tests
     TEST_DATA_PATH = join(dirname(__file__), "..", "tests", "test_data")
     HIDE_PLOTS = True
 
     # Places
@@ -149,14 +151,13 @@
             ]
             PLACES_SMALL = [
                 (name, data["query"])
                 for name, data in places["place_lists"]["test_small"]["cities"].items()
             ]
             PLACES_100_CITIES = places["place_lists"]["100_cities_boeing"]["cities"]
             PLACES_GERMANY = places["place_lists"]["germany_by_pop"]["cities"]
-            PLACES_JUST_STREETS = places["place_lists"]["just_streets"]["cities"]
 
     # Plot format
     PLOT_SUFFIX = "pdf"
 
     # Reduce graph
     MAX_NODES = 20000
```

### Comparing `superblockify-1.0.0rc4/superblockify/graph_stats.py` & `superblockify-1.0.0rc5/superblockify/graph_stats.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify/logging.cfg` & `superblockify-1.0.0rc5/superblockify/logging.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 [handlers]
 keys = consoleHandler,RotatingFileHandler
 
 [formatters]
 keys = simpleFormatter
 
 [logger_root]
-level = DEBUG
+level = INFO
 handlers = consoleHandler
 
 [logger_superblockify]
-level = DEBUG
+level = INFO
 handlers = consoleHandler,RotatingFileHandler
 qualname = superblockify
 propagate = 1
 
 [handler_consoleHandler]
 class = StreamHandler
-level = DEBUG
+level = INFO
 formatter = simpleFormatter
 args = (sys.stdout,)
 
 [handler_tqdmHandler]
 class = StreamHandler
 level = INFO
 formatter = simpleFormatter
```

### Comparing `superblockify-1.0.0rc4/superblockify/metrics/distances.py` & `superblockify-1.0.0rc5/superblockify/metrics/distances.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify/metrics/measures.py` & `superblockify-1.0.0rc5/superblockify/metrics/measures.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify/metrics/metric.py` & `superblockify-1.0.0rc5/superblockify/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify/metrics/plot.py` & `superblockify-1.0.0rc5/superblockify/metrics/plot.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify/partitioning/__init__.py` & `superblockify-1.0.0rc5/superblockify/partitioning/__init__.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify/partitioning/approaches/attribute.py` & `superblockify-1.0.0rc5/superblockify/partitioning/approaches/attribute.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify/partitioning/approaches/bearing.py` & `superblockify-1.0.0rc5/superblockify/partitioning/approaches/bearing.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify/partitioning/approaches/betweenness.py` & `superblockify-1.0.0rc5/superblockify/partitioning/approaches/betweenness.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify/partitioning/approaches/dummy.py` & `superblockify-1.0.0rc5/superblockify/partitioning/approaches/dummy.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify/partitioning/approaches/steiner_tree.py` & `superblockify-1.0.0rc5/superblockify/partitioning/approaches/steiner_tree.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify/partitioning/approaches/streettype.py` & `superblockify-1.0.0rc5/superblockify/partitioning/approaches/streettype.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify/partitioning/base.py` & `superblockify-1.0.0rc5/superblockify/partitioning/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 from .utils import (
     show_highway_stats,
     show_graph_stats,
     remove_dead_ends_directed,
     split_up_isolated_edges_directed,
     get_key_figures,
     reduce_graph,
-    save_to_gpkg,
 )
 from .. import attribute
 from ..config import logger, Config
 from ..graph_stats import calculate_component_metrics
 from ..metrics.metric import Metric
 from ..plot import save_plot
 from ..population.tessellation import add_edge_cells
@@ -1031,35 +1030,7 @@
                     )
         # Convert self.sparsified to subgraph of self.graph.
         if partitioner.sparsified is not None:
             partitioner.sparsified = partitioner.graph.edge_subgraph(
                 partitioner.sparsified.edges
             )
         return partitioner
-
-    def export_ltns(
-        self,
-        save_path=None,
-        ltn_boundary=False,
-    ):
-        """Export to geopackage.
-
-        The name of the components (/partitions) is saved into a "classification" edge
-        attribute. The sparse graph is saved with the value "SPARSE" into the
-        "classification" edge attribute.
-
-        Parameters
-        ----------
-        save_path : str, optional
-            The path to save the geodatapackage to. If None, it will be saved to the
-            partitioners folder at (part.results_dir, part.name + ".gpkg")
-        ltn_boundary : bool, optional
-            If True, the boundary of the LTNs will be saved as a polygon into the `cell`
-            attribute of the LTNs layer.
-            For this, the tessellation needs to be calculated.
-
-        See Also
-        --------
-        :func:`superblockify.utils.save_to_gpkg`
-        """
-
-        save_to_gpkg(self, save_path, ltn_boundary)
```

### Comparing `superblockify-1.0.0rc4/superblockify/partitioning/checks.py` & `superblockify-1.0.0rc5/superblockify/partitioning/checks.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify/partitioning/plot.py` & `superblockify-1.0.0rc5/superblockify/partitioning/plot.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify/partitioning/representative.py` & `superblockify-1.0.0rc5/superblockify/partitioning/representative.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify/partitioning/speed.py` & `superblockify-1.0.0rc5/superblockify/partitioning/speed.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify/partitioning/utils.py` & `superblockify-1.0.0rc5/superblockify/partitioning/utils.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify/plot.py` & `superblockify-1.0.0rc5/superblockify/plot.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify/population/approximation.py` & `superblockify-1.0.0rc5/superblockify/population/approximation.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify/population/ghsl.py` & `superblockify-1.0.0rc5/superblockify/population/ghsl.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify/population/tessellation.py` & `superblockify-1.0.0rc5/superblockify/population/tessellation.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify/utils.py` & `superblockify-1.0.0rc5/superblockify/utils.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/superblockify.egg-info/PKG-INFO` & `superblockify-1.0.0rc5/superblockify.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: superblockify
-Version: 1.0.0rc4
+Version: 1.0.0rc5
 Summary: Automated Generation, Visualization, and Analysis of potential Superblocks in Cities
 Author-email: Carlson Büth <carlson@cbueth.de>
 Maintainer: superblockify contributors
-License: APGL-3.0
+License: APGL-3.0-or-later
 Project-URL: Documentation, https://NERDSITU.github.io/superblockify
 Project-URL: Repository, https://github.com/NERDSITU/superblockify
 Project-URL: Changelog, https://NERDSITU.github.io/superblockify/changelog/
 Keywords: Low Traffic Neighborhoods,GIS,Networks,OpenStreetMap,Urban Planning,Urban Mobility,Urban Data
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -33,14 +35,15 @@
 Requires-Dist: numba
 Requires-Dist: tqdm
 Requires-Dist: contextily
 Requires-Dist: ruamel.yaml
 Requires-Dist: pyarrow
 Requires-Dist: seaborn
 Requires-Dist: psutil
+Requires-Dist: typing-extensions
 Provides-Extra: lint
 Requires-Dist: blackd; extra == "lint"
 Requires-Dist: isort; extra == "lint"
 Requires-Dist: pylint; extra == "lint"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
@@ -51,53 +54,57 @@
 Requires-Dist: myst-nb; extra == "doc"
 Requires-Dist: sphinx-book-theme; extra == "doc"
 Requires-Dist: rasterstats; extra == "doc"
 Requires-Dist: momepy; extra == "doc"
 Provides-Extra: all
 Requires-Dist: superblockify[doc,lint,test]; extra == "all"
 
-# `superblockify`
+# superblockify
 
 [![Dev](https://img.shields.io/badge/docs-dev-blue.svg)](https://NERDSITU.github.io/superblockify/)
-[![codecov](https://codecov.io/gh/NERDSITU/superblockify/branch/main/graph/badge.svg?token=AS72IFT2Q4)](https://codecov.io/gh/NERDSITU/superblockify)
+[![PyPI Version](https://badge.fury.io/py/superblockify.svg)](https://pypi.org/project/superblockify/)
+[![Python Version](https://img.shields.io/pypi/pyversions/superblockify)](https://pypi.org/project/superblockify/)
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PyPI License](https://img.shields.io/pypi/l/superblockify)](https://pypi.org/project/superblockify/)
 
 [![Docs](https://github.com/NERDSITU/superblockify/actions/workflows/docs.yml/badge.svg)](https://github.com/NERDSITU/superblockify/actions/workflows/docs.yml)
 [![Lint](https://github.com/NERDSITU/superblockify/actions/workflows/lint.yml/badge.svg)](https://github.com/NERDSITU/superblockify/actions/workflows/lint.yml)
 [![Test](https://github.com/NERDSITU/superblockify/actions/workflows/test.yml/badge.svg)](https://github.com/NERDSITU/superblockify/actions/workflows/test.yml)
+[![codecov](https://codecov.io/gh/NERDSITU/superblockify/branch/main/graph/badge.svg?token=AS72IFT2Q4)](https://codecov.io/gh/NERDSITU/superblockify)
 
 Source code for blockifying existing street networks.
 
 ---
 
 ## Installation
 
-Create a new environment with `conda` or `mamba` and install the package from the
-`conda-forge` channel.
+We recommend using `micromamba` to create a virtual
+environment and installing the package in editable mode.
+Alternatively, one can use `conda` or `mamba` to create the environment
+(they can be used interchangeably).
+After cloning the repository, navigate to the root folder and
+create the environment with the wished python version and the development dependencies.
 
 ```bash
-conda create -n sb_env -c conda-forge superblockify
-conda activate sb_env
+micromamba create -n sb_env -c conda-forge python=3.12 osmnx
+micromamba activate sb_env
+pip install superblockify
 ```
 
 This installs the package and its dependencies,
 ready for use when activating the environment.
 Learn more about `superblockify` by reading
 the [documentation](https://NERDSITU.github.io/superblockify/)
 or
 the [minimal working example](https://github.com/NERDSITU/superblockify/blob/main/scripts/examples/mwe.py).
 
 ## Development Setup
 
-For development, we recommend using `micromamba` to create a virtual
-environment and installing the package in editable mode.
-Alternatively, one can use `conda` or `mamba` to create the environment
-(they can be used interchangeably).
-After cloning the repository, navigate to the root folder and
+For development, clone the repository, navigate to the root folder and
 create the environment with the wished python version and the development dependencies.
 
 ```bash
 micromamba create -n sb_env -c conda-forge python=3.12 --file=environment.yml
 micromamba activate sb_env
 ```
```

### Comparing `superblockify-1.0.0rc4/superblockify.egg-info/SOURCES.txt` & `superblockify-1.0.0rc5/superblockify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/tests/test_attribute.py` & `superblockify-1.0.0rc5/tests/test_attribute.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/tests/test_graph_stats.py` & `superblockify-1.0.0rc5/tests/test_graph_stats.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/tests/test_plot.py` & `superblockify-1.0.0rc5/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc4/tests/test_utils.py` & `superblockify-1.0.0rc5/tests/test_utils.py`

 * *Files identical despite different names*

