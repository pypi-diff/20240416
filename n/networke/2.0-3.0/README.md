# Comparing `tmp/networke-2.0.tar.gz` & `tmp/networke-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networke-2.0.tar", last modified: Thu Apr 11 16:48:07 2024, max compression
+gzip compressed data, was "networke-3.0.tar", last modified: Tue Apr 16 16:21:37 2024, max compression
```

## Comparing `networke-2.0.tar` & `networke-3.0.tar`

### file list

```diff
@@ -1,24 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 16:48:07.499426 networke-2.0/
--rw-rw-rw-   0        0        0        0 2024-04-09 15:52:45.000000 networke-2.0/LICENSE.txt
--rw-rw-rw-   0        0        0       80 2024-04-11 16:48:07.499426 networke-2.0/PKG-INFO
--rw-rw-rw-   0        0        0        3 2024-04-09 15:52:26.000000 networke-2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 16:48:07.421306 networke-2.0/network/
--rw-rw-rw-   0        0        0       28 2024-04-09 15:55:03.000000 networke-2.0/network/__init__.py
--rw-rw-rw-   0        0        0     1720 2024-04-11 15:30:17.000000 networke-2.0/network/bst.py
--rw-rw-rw-   0        0        0      197 2024-04-11 13:17:01.000000 networke-2.0/network/comp_sum.py
--rw-rw-rw-   0        0        0      248 2024-04-11 13:23:15.000000 networke-2.0/network/hanoi.py
--rw-rw-rw-   0        0        0     3028 2024-04-11 16:21:42.000000 networke-2.0/network/krus.py
--rw-rw-rw-   0        0        0       82 2024-04-09 15:54:50.000000 networke-2.0/network/main.py
--rw-rw-rw-   0        0        0      971 2024-04-11 13:41:30.000000 networke-2.0/network/merge_sort.py
--rw-rw-rw-   0        0        0     5710 2024-04-11 16:32:14.000000 networke-2.0/network/poley.py
--rw-rw-rw-   0        0        0      236 2024-04-11 13:19:31.000000 networke-2.0/network/pow.py
--rw-rw-rw-   0        0        0     2805 2024-04-11 14:23:00.000000 networke-2.0/network/qu.py
--rw-rw-rw-   0        0        0      418 2024-04-11 13:29:15.000000 networke-2.0/network/seat.py
--rw-rw-rw-   0        0        0     1516 2024-04-11 13:55:51.000000 networke-2.0/network/stackey.py
-drwxrwxrwx   0        0        0        0 2024-04-11 16:48:07.499426 networke-2.0/networke.egg-info/
--rw-rw-rw-   0        0        0       80 2024-04-11 16:48:06.000000 networke-2.0/networke.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2024-04-11 16:48:07.000000 networke-2.0/networke.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 16:48:06.000000 networke-2.0/networke.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-11 16:48:06.000000 networke-2.0/networke.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 16:48:07.515049 networke-2.0/setup.cfg
--rw-rw-rw-   0        0        0      197 2024-04-11 16:47:47.000000 networke-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 16:21:37.090091 networke-3.0/
+-rw-rw-rw-   0        0        0        0 2024-04-09 15:52:45.000000 networke-3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       80 2024-04-16 16:21:37.086096 networke-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0        3 2024-04-09 15:52:26.000000 networke-3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 16:21:37.033124 networke-3.0/network/
+-rw-rw-rw-   0        0        0       28 2024-04-09 15:55:03.000000 networke-3.0/network/__init__.py
+-rw-rw-rw-   0        0        0     1720 2024-04-11 15:30:17.000000 networke-3.0/network/bst.py
+-rw-rw-rw-   0        0        0      197 2024-04-11 13:17:01.000000 networke-3.0/network/comp_sum.py
+-rw-rw-rw-   0        0        0     6873 2024-03-10 04:18:36.000000 networke-3.0/network/doublelinky.py
+-rw-rw-rw-   0        0        0      248 2024-04-11 13:23:15.000000 networke-3.0/network/hanoi.py
+-rw-rw-rw-   0        0        0     3028 2024-04-11 16:21:42.000000 networke-3.0/network/krus.py
+-rw-rw-rw-   0        0        0     4619 2024-02-23 14:09:39.000000 networke-3.0/network/linked_list.py
+-rw-rw-rw-   0        0        0       82 2024-04-09 15:54:50.000000 networke-3.0/network/main.py
+-rw-rw-rw-   0        0        0      971 2024-04-11 13:41:30.000000 networke-3.0/network/merge_sort.py
+-rw-rw-rw-   0        0        0     5710 2024-04-11 16:32:14.000000 networke-3.0/network/poley.py
+-rw-rw-rw-   0        0        0      236 2024-04-11 13:19:31.000000 networke-3.0/network/pow.py
+-rw-rw-rw-   0        0        0      232 2024-04-09 09:55:10.000000 networke-3.0/network/progarm_factorial.py
+-rw-rw-rw-   0        0        0      254 2024-04-07 07:46:58.000000 networke-3.0/network/program_5_fibonacci.py
+-rw-rw-rw-   0        0        0     2919 2024-04-09 10:58:58.000000 networke-3.0/network/program_array.py
+-rw-rw-rw-   0        0        0      222 2024-04-09 09:42:53.000000 networke-3.0/network/program_asc_Desc.py
+-rw-rw-rw-   0        0        0     2173 2024-04-09 12:33:55.000000 networke-3.0/network/program_dfs.py
+-rw-rw-rw-   0        0        0     3463 2024-04-09 13:52:44.000000 networke-3.0/network/program_heap.py
+-rw-rw-rw-   0        0        0     2205 2024-04-09 13:23:53.000000 networke-3.0/network/program_prims.py
+-rw-rw-rw-   0        0        0     1056 2024-04-09 11:30:12.000000 networke-3.0/network/program_quicksort.py
+-rw-rw-rw-   0        0        0     2320 2024-04-16 16:04:47.000000 networke-3.0/network/program_stack_expr.py
+-rw-rw-rw-   0        0        0     2805 2024-04-11 14:23:00.000000 networke-3.0/network/qu.py
+-rw-rw-rw-   0        0        0      418 2024-04-11 13:29:15.000000 networke-3.0/network/seat.py
+-rw-rw-rw-   0        0        0     1516 2024-04-11 13:55:51.000000 networke-3.0/network/stackey.py
+drwxrwxrwx   0        0        0        0 2024-04-16 16:21:37.080131 networke-3.0/networke.egg-info/
+-rw-rw-rw-   0        0        0       80 2024-04-16 16:21:36.000000 networke-3.0/networke.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      655 2024-04-16 16:21:36.000000 networke-3.0/networke.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 16:21:36.000000 networke-3.0/networke.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-16 16:21:36.000000 networke-3.0/networke.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 16:21:37.091089 networke-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      197 2024-04-16 16:00:55.000000 networke-3.0/setup.py
```

### Comparing `networke-2.0/network/bst.py` & `networke-3.0/network/bst.py`

 * *Files identical despite different names*

### Comparing `networke-2.0/network/krus.py` & `networke-3.0/network/krus.py`

 * *Files identical despite different names*

### Comparing `networke-2.0/network/merge_sort.py` & `networke-3.0/network/merge_sort.py`

 * *Files identical despite different names*

### Comparing `networke-2.0/network/poley.py` & `networke-3.0/network/poley.py`

 * *Files identical despite different names*

### Comparing `networke-2.0/network/qu.py` & `networke-3.0/network/qu.py`

 * *Files identical despite different names*

### Comparing `networke-2.0/network/stackey.py` & `networke-3.0/network/stackey.py`

 * *Files identical despite different names*

