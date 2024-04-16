# Comparing `tmp/countess-0.0.58.tar.gz` & `tmp/countess-0.0.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "countess-0.0.58.tar", last modified: Tue Apr  9 05:48:04 2024, max compression
+gzip compressed data, was "countess-0.0.59.tar", last modified: Tue Apr 16 05:18:19 2024, max compression
```

## Comparing `countess-0.0.58.tar` & `countess-0.0.59.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-09 05:48:04.286211 countess-0.0.58/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1470 2023-10-25 21:13:29.000000 countess-0.0.58/LICENSE.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       59 2024-04-03 00:27:43.000000 countess-0.0.58/MANIFEST.in
--rw-r--r--   0 nick      (1000) nick      (1000)     2050 2024-04-09 05:48:04.286211 countess-0.0.58/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      723 2024-04-09 05:47:38.000000 countess-0.0.58/README.md
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-09 05:48:04.278211 countess-0.0.58/countess/
--rw-rw-r--   0 nick      (1000) nick      (1000)       43 2024-04-09 05:47:38.000000 countess-0.0.58/countess/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-09 05:48:04.282211 countess-0.0.58/countess/core/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.58/countess/core/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      466 2024-04-03 00:27:43.000000 countess-0.0.58/countess/core/cmd.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4764 2024-04-05 06:49:16.000000 countess-0.0.58/countess/core/config.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2799 2023-11-09 02:30:05.000000 countess-0.0.58/countess/core/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    19404 2024-04-09 05:40:26.000000 countess-0.0.58/countess/core/parameters.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    13908 2024-04-09 05:44:13.000000 countess-0.0.58/countess/core/pipeline.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    25925 2024-04-09 05:44:13.000000 countess-0.0.58/countess/core/plugins.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-09 05:48:04.282211 countess-0.0.58/countess/gui/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.58/countess/gui/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    18505 2024-04-09 05:44:13.000000 countess-0.0.58/countess/gui/config.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-09 05:48:04.282211 countess-0.0.58/countess/gui/icons/
--rw-rw-r--   0 nick      (1000) nick      (1000)       90 2024-04-03 00:27:43.000000 countess-0.0.58/countess/gui/icons/add.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-04-03 00:27:43.000000 countess-0.0.58/countess/gui/icons/check.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)    20442 2024-04-09 05:41:27.000000 countess-0.0.58/countess/gui/icons/countess.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-04-03 00:27:43.000000 countess-0.0.58/countess/gui/icons/del.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       62 2024-04-05 05:13:40.000000 countess-0.0.58/countess/gui/icons/hbar.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-04-03 00:27:43.000000 countess-0.0.58/countess/gui/icons/info.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-04-05 05:13:40.000000 countess-0.0.58/countess/gui/icons/redbar.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-04-05 05:13:40.000000 countess-0.0.58/countess/gui/icons/sort_dn.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       86 2024-04-05 05:13:40.000000 countess-0.0.58/countess/gui/icons/sort_un.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-04-05 05:13:40.000000 countess-0.0.58/countess/gui/icons/sort_up.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-04-03 00:27:43.000000 countess-0.0.58/countess/gui/icons/uncheck.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-04-05 05:13:40.000000 countess-0.0.58/countess/gui/icons/vbar.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)     5105 2024-04-03 00:27:43.000000 countess-0.0.58/countess/gui/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    20633 2024-04-09 05:44:13.000000 countess-0.0.58/countess/gui/main.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1730 2024-04-05 05:13:40.000000 countess-0.0.58/countess/gui/mini_browser.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    15188 2024-04-05 05:13:40.000000 countess-0.0.58/countess/gui/tabular.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    23070 2024-04-05 06:49:16.000000 countess-0.0.58/countess/gui/tree.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3565 2024-04-05 05:13:40.000000 countess-0.0.58/countess/gui/widgets.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-09 05:48:04.286211 countess-0.0.58/countess/plugins/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.58/countess/plugins/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2402 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/collate.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2116 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/column.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2245 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/correlation.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     7274 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/csv.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3844 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/data_table.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1842 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/expression.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2938 2024-04-05 05:13:40.000000 countess-0.0.58/countess/plugins/fastq.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4735 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/group_by.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3339 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/hgvs_parser.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4541 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/join.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3348 2023-11-28 03:30:23.000000 countess-0.0.58/countess/plugins/mutagenize.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3854 2024-04-08 01:06:06.000000 countess-0.0.58/countess/plugins/pivot.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2977 2024-04-03 00:27:43.000000 countess-0.0.58/countess/plugins/python.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     6758 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/regex.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1902 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/sequence.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3524 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/variant.py
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:39:01.000000 countess-0.0.58/countess/py.typed
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-09 05:48:04.286211 countess-0.0.58/countess/utils/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.58/countess/utils/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2768 2024-03-14 02:50:26.000000 countess-0.0.58/countess/utils/pandas.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2996 2024-04-03 00:27:43.000000 countess-0.0.58/countess/utils/parallel.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    18172 2024-04-09 05:40:45.000000 countess-0.0.58/countess/utils/variant.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-09 05:48:04.286211 countess-0.0.58/countess.egg-info/
--rw-r--r--   0 nick      (1000) nick      (1000)     2050 2024-04-09 05:48:04.000000 countess-0.0.58/countess.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     1651 2024-04-09 05:48:04.000000 countess-0.0.58/countess.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2024-04-09 05:48:04.000000 countess-0.0.58/countess.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     1056 2024-04-09 05:48:04.000000 countess-0.0.58/countess.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      310 2024-04-09 05:48:04.000000 countess-0.0.58/countess.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        9 2024-04-09 05:48:04.000000 countess-0.0.58/countess.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     3236 2024-04-05 06:49:16.000000 countess-0.0.58/pyproject.toml
--rw-rw-r--   0 nick      (1000) nick      (1000)       38 2024-04-09 05:48:04.286211 countess-0.0.58/setup.cfg
--rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-25 01:44:18.000000 countess-0.0.58/setup.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-09 05:48:04.286211 countess-0.0.58/tests/
--rw-rw-r--   0 nick      (1000) nick      (1000)      476 2024-04-05 05:13:41.000000 countess-0.0.58/tests/test_cmd.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      498 2024-04-05 05:13:41.000000 countess-0.0.58/tests/test_gui.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1060 2023-11-09 02:44:32.000000 countess-0.0.58/tests/test_plugins.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-16 05:18:19.841561 countess-0.0.59/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1470 2023-10-25 21:13:29.000000 countess-0.0.59/LICENSE.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       59 2024-04-03 00:27:43.000000 countess-0.0.59/MANIFEST.in
+-rw-r--r--   0 nick      (1000) nick      (1000)     2050 2024-04-16 05:18:19.841561 countess-0.0.59/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      723 2024-04-16 05:16:27.000000 countess-0.0.59/README.md
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-16 05:18:19.833561 countess-0.0.59/countess/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       43 2024-04-16 05:16:27.000000 countess-0.0.59/countess/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-16 05:18:19.837561 countess-0.0.59/countess/core/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.59/countess/core/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      466 2024-04-03 00:27:43.000000 countess-0.0.59/countess/core/cmd.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4764 2024-04-05 06:49:16.000000 countess-0.0.59/countess/core/config.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2799 2023-11-09 02:30:05.000000 countess-0.0.59/countess/core/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    19404 2024-04-12 03:37:47.000000 countess-0.0.59/countess/core/parameters.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    13908 2024-04-16 04:58:09.000000 countess-0.0.59/countess/core/pipeline.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    25925 2024-04-16 04:58:09.000000 countess-0.0.59/countess/core/plugins.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-16 05:18:19.837561 countess-0.0.59/countess/gui/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.59/countess/gui/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    18396 2024-04-16 04:58:09.000000 countess-0.0.59/countess/gui/config.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-16 05:18:19.837561 countess-0.0.59/countess/gui/icons/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       90 2024-04-03 00:27:43.000000 countess-0.0.59/countess/gui/icons/add.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-04-03 00:27:43.000000 countess-0.0.59/countess/gui/icons/check.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)    20442 2024-04-12 03:37:47.000000 countess-0.0.59/countess/gui/icons/countess.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-04-03 00:27:43.000000 countess-0.0.59/countess/gui/icons/del.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       62 2024-04-05 05:13:40.000000 countess-0.0.59/countess/gui/icons/hbar.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-04-03 00:27:43.000000 countess-0.0.59/countess/gui/icons/info.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-04-05 05:13:40.000000 countess-0.0.59/countess/gui/icons/redbar.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-04-05 05:13:40.000000 countess-0.0.59/countess/gui/icons/sort_dn.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       86 2024-04-05 05:13:40.000000 countess-0.0.59/countess/gui/icons/sort_un.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-04-05 05:13:40.000000 countess-0.0.59/countess/gui/icons/sort_up.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-04-03 00:27:43.000000 countess-0.0.59/countess/gui/icons/uncheck.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-04-05 05:13:40.000000 countess-0.0.59/countess/gui/icons/vbar.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5104 2024-04-15 03:16:30.000000 countess-0.0.59/countess/gui/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    20505 2024-04-16 04:58:09.000000 countess-0.0.59/countess/gui/main.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1730 2024-04-05 05:13:40.000000 countess-0.0.59/countess/gui/mini_browser.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    14479 2024-04-16 04:58:09.000000 countess-0.0.59/countess/gui/tabular.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    23070 2024-04-05 06:49:16.000000 countess-0.0.59/countess/gui/tree.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     9359 2024-04-15 09:54:50.000000 countess-0.0.59/countess/gui/widgets.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-16 05:18:19.841561 countess-0.0.59/countess/plugins/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.59/countess/plugins/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2402 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/collate.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2116 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/column.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2245 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/correlation.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     7274 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/csv.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3844 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/data_table.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1842 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/expression.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2938 2024-04-05 05:13:40.000000 countess-0.0.59/countess/plugins/fastq.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4735 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/group_by.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3339 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/hgvs_parser.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4541 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/join.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3348 2023-11-28 03:30:23.000000 countess-0.0.59/countess/plugins/mutagenize.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3854 2024-04-08 01:06:06.000000 countess-0.0.59/countess/plugins/pivot.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2977 2024-04-03 00:27:43.000000 countess-0.0.59/countess/plugins/python.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     6758 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/regex.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1902 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/sequence.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3524 2024-04-16 04:58:09.000000 countess-0.0.59/countess/plugins/variant.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:39:01.000000 countess-0.0.59/countess/py.typed
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-16 05:18:19.841561 countess-0.0.59/countess/utils/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.59/countess/utils/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2768 2024-03-14 02:50:26.000000 countess-0.0.59/countess/utils/pandas.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2996 2024-04-03 00:27:43.000000 countess-0.0.59/countess/utils/parallel.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    18172 2024-04-12 03:37:47.000000 countess-0.0.59/countess/utils/variant.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-16 05:18:19.841561 countess-0.0.59/countess.egg-info/
+-rw-r--r--   0 nick      (1000) nick      (1000)     2050 2024-04-16 05:18:19.000000 countess-0.0.59/countess.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1651 2024-04-16 05:18:19.000000 countess-0.0.59/countess.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2024-04-16 05:18:19.000000 countess-0.0.59/countess.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1056 2024-04-16 05:18:19.000000 countess-0.0.59/countess.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      310 2024-04-16 05:18:19.000000 countess-0.0.59/countess.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        9 2024-04-16 05:18:19.000000 countess-0.0.59/countess.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3236 2024-04-05 06:49:16.000000 countess-0.0.59/pyproject.toml
+-rw-rw-r--   0 nick      (1000) nick      (1000)       38 2024-04-16 05:18:19.841561 countess-0.0.59/setup.cfg
+-rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-25 01:44:18.000000 countess-0.0.59/setup.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-16 05:18:19.841561 countess-0.0.59/tests/
+-rw-rw-r--   0 nick      (1000) nick      (1000)      476 2024-04-05 05:13:41.000000 countess-0.0.59/tests/test_cmd.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      498 2024-04-05 05:13:41.000000 countess-0.0.59/tests/test_gui.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1060 2023-11-09 02:44:32.000000 countess-0.0.59/tests/test_plugins.py
```

### Comparing `countess-0.0.58/LICENSE.txt` & `countess-0.0.59/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/PKG-INFO` & `countess-0.0.59/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.58
+Version: 0.0.59
 Summary: CountESS
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -30,15 +30,15 @@
 Requires-Dist: pylint~=2.17; extra == "dev"
 Requires-Dist: types-psutil~=5.9.5; extra == "dev"
 Requires-Dist: types-ttkthemes~=3.2; extra == "dev"
 Requires-Dist: twine==4.0.2; extra == "dev"
 Requires-Dist: pandas-stubs~=2.1.0; extra == "dev"
 Requires-Dist: pytest~=7.2; extra == "dev"
 
-# CountESS 0.0.58
+# CountESS 0.0.59
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.58/README.md` & `countess-0.0.59/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CountESS 0.0.58
+# CountESS 0.0.59
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.58/countess/core/config.py` & `countess-0.0.59/countess/core/config.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/core/logger.py` & `countess-0.0.59/countess/core/logger.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/core/parameters.py` & `countess-0.0.59/countess/core/parameters.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/core/pipeline.py` & `countess-0.0.59/countess/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/core/plugins.py` & `countess-0.0.59/countess/core/plugins.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/gui/config.py` & `countess-0.0.59/countess/gui/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -421,26 +421,22 @@
     output_text = None
     preview = None
 
     def __init__(self, tk_parent: tk.Widget, plugin: BasePlugin, change_callback=None):
         self.plugin = plugin
         self.change_callback = change_callback
 
-        self.frame = tk.Frame(tk_parent)
-        self.frame.columnconfigure(0, weight=1)
+        self.frame = tk.Frame(tk_parent, highlightcolor="purple", highlightthickness=3)
+        self.frame.columnconfigure(0, weight=0)
+        self.frame.columnconfigure(1, weight=0)
+        self.frame.columnconfigure(2, weight=1)
         self.frame.grid(sticky=tk.NSEW)
 
         self.wrapper_cache: MutableMapping[str, ParameterWrapper] = {}
 
-        self.subframe = tk.Frame(self.frame)
-        self.subframe.columnconfigure(0, weight=0)
-        self.subframe.columnconfigure(1, weight=0)
-        self.subframe.columnconfigure(2, weight=1)
-        self.subframe.grid(row=1, sticky=tk.NSEW)
-
         self.update()
 
     def change_parameter(self, parameter):
         """Called whenever a parameter gets changed"""
         # if self.plugin.update():
         #    self.update()
         if self.change_callback:
@@ -452,15 +448,15 @@
 
         # Create any new parameter wrappers needed & update existing ones
         for n, (key, parameter) in enumerate(self.plugin.parameters.items()):
             if key in self.wrapper_cache:
                 self.wrapper_cache[key].update()
             else:
                 self.wrapper_cache[key] = ParameterWrapper(
-                    self.subframe, parameter, self.change_parameter, level=top_level
+                    self.frame, parameter, self.change_parameter, level=top_level
                 )
             self.wrapper_cache[key].set_row(n + 1)
 
         # Remove any parameter wrappers no longer needed
         for key, wrapper in list(self.wrapper_cache.items()):
             if key not in self.plugin.parameters:
                 wrapper.destroy()
```

### Comparing `countess-0.0.58/countess/gui/icons/countess.gif` & `countess-0.0.59/countess/gui/icons/countess.gif`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/gui/logger.py` & `countess-0.0.59/countess/gui/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         kwargs["style"] = self.style_name
         super().__init__(master, *args, **kwargs)
 
     def update_label(self, s):
         self.style.configure(self.style_name, text=s)
 
 
-class LoggerFrame(ttk.Frame):
+class LoggerFrame(tk.Frame):
     def __init__(self, tk_parent, *a, **k):
         super().__init__(tk_parent, *a, **k)
         self.columnconfigure(0, weight=1)
         self.rowconfigure(0, weight=1)
 
         self.treeview = LoggerTreeview(self)
         self.treeview.grid(row=0, column=0, sticky=tk.NSEW)
```

### Comparing `countess-0.0.58/countess/gui/main.py` & `countess-0.0.59/countess/gui/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from countess.core.pipeline import PipelineGraph
 from countess.core.plugins import get_plugin_classes
 from countess.gui.config import PluginConfigurator
 from countess.gui.logger import LoggerFrame
 from countess.gui.mini_browser import MiniBrowserFrame
 from countess.gui.tabular import TabularDataFrame
 from countess.gui.tree import FlippyCanvas, GraphWrapper
-from countess.gui.widgets import ask_open_filename, ask_saveas_filename, get_icon, info_button
+from countess.gui.widgets import ResizingFrame, ask_open_filename, ask_saveas_filename, get_icon, info_button
 from countess.utils.pandas import concat_dataframes
 
 # import faulthandler
 # faulthandler.enable(all_threads=True)
 
 
 plugin_classes = sorted(get_plugin_classes(), key=lambda x: x.name)
@@ -63,82 +63,79 @@
     preview_subframe = None
     config_change_task = None
     notes_widget = None
     node_update_thread = None
     info_toplevel = None
     info_frame = None
 
-    def __init__(self, frame, node, change_callback):
-        self.frame = frame
+    def __init__(self, tk_parent, node, logger, change_callback):
         self.node = node
+        self.logger = logger
         self.change_callback = change_callback
 
-        self.name_var = tk.StringVar(self.frame, value=node.name)
-        tk.Entry(self.frame, textvariable=self.name_var, font=("TkHeadingFont", 14, "bold")).grid(
+        self.frame = ResizingFrame(tk_parent, orientation=ResizingFrame.Orientation.VERTICAL, bg="darkgrey")
+        self.subframe = self.frame.add_frame()
+        self.subframe.columnconfigure(0, weight=1)
+        self.subframe.rowconfigure(3, weight=1)
+
+        self.name_var = tk.StringVar(self.subframe, value=node.name)
+        tk.Entry(self.subframe, textvariable=self.name_var, font=("TkHeadingFont", 14, "bold")).grid(
             row=0, columnspan=2, sticky=tk.EW, padx=10, pady=5
         )
         self.name_var.trace("w", self.name_changed_callback)
 
-        self.label = tk.Label(self.frame, justify=tk.LEFT, wraplength=500)
+        self.label = tk.Label(self.subframe, justify=tk.LEFT, wraplength=500)
         self.label.grid(sticky=tk.EW, row=1, padx=10, pady=5)
         self.label.bind("<Configure>", self.on_label_configure)
 
         self.show_config_subframe()
 
         if self.node.plugin:
             if self.node.is_dirty:
                 self.config_change_callback()
             else:
                 self.show_preview_subframe()
 
     def show_config_subframe(self):
         if self.config_canvas:
             self.config_canvas.destroy()
-        self.config_canvas = tk.Canvas(self.frame)
-        self.config_scrollbar = ttk.Scrollbar(self.frame, orient=tk.VERTICAL, command=self.config_canvas.yview)
+        self.config_canvas = tk.Canvas(self.subframe)
+        self.config_scrollbar = ttk.Scrollbar(self.subframe, orient=tk.VERTICAL, command=self.config_canvas.yview)
         self.config_canvas.configure(yscrollcommand=self.config_scrollbar.set, bd=0)
         self.config_canvas.grid(row=3, column=0, sticky=tk.NSEW)
         self.config_scrollbar.grid(row=3, column=1, sticky=tk.NS)
 
-        self.logger_subframe = LoggerFrame(self.frame)
-        self.logger = self.logger_subframe.get_logger(self.node.name)
-
         if self.node.plugin:
+            self.node.load_config(self.logger)
             if self.node.notes:
                 self.show_notes_widget(self.node.notes)
             else:
-                self.notes_widget = tk.Button(self.frame, text="add notes", command=self.on_add_notes)
+                self.notes_widget = tk.Button(self.subframe, text="add notes", command=self.on_add_notes)
                 self.notes_widget.grid(row=2, columnspan=2, padx=10, pady=5)
 
             descr = re.sub(r"\s+", " ", self.node.plugin.description)
             if self.node.plugin.additional:
                 descr += "\n" + re.sub(r"\s+", " ", self.node.plugin.additional)
 
             self.label["text"] = "%s %s — %s" % (
                 self.node.plugin.name,
                 self.node.plugin.version,
                 descr,
             )
             if self.node.plugin.link:
                 info_button(self.frame, command=self.on_info_button_press).place(anchor=tk.NE, relx=1, y=50)
-            # self.node.prepare(self.logger)
-            # self.node.plugin.update()
             self.configurator = PluginConfigurator(self.config_canvas, self.node.plugin, self.config_change_callback)
             self.config_subframe = self.configurator.frame
-            self.frame.rowconfigure(3, weight=1, minsize=self.frame.winfo_height() / 3)
 
         else:
             has_parents = len(self.node.parent_nodes) > 0
             has_children = len(self.node.child_nodes) > 0
             self.config_subframe = PluginChooserFrame(
                 self.config_canvas, "Choose Plugin", self.choose_plugin, has_parents, has_children
             )
-            self.config_subframe.grid(sticky=tk.NSEW)
-            self.frame.rowconfigure(3, weight=1)
-            self.frame.rowconfigure(4, weight=0)
 
         self.config_subframe_id = self.config_canvas.create_window((0, 0), window=self.config_subframe, anchor=tk.NW)
         self.config_subframe.bind(
             "<Configure>",
             lambda e: self.config_canvas.configure(scrollregion=self.config_canvas.bbox("all")),
         )
         self.config_canvas.bind("<Configure>", self.on_config_canvas_configure)
@@ -163,54 +160,53 @@
         self.info_toplevel = None
 
     def on_add_notes(self, *_):
         self.notes_widget.destroy()
         self.show_notes_widget()
 
     def show_notes_widget(self, notes=""):
-        self.notes_widget = tk.Text(self.frame, height=5)
+        self.notes_widget = tk.Text(self.subframe, height=5)
         self.notes_widget.insert("1.0", notes)
         self.notes_widget.bind("<<Modified>>", self.notes_modified_callback)
         self.notes_widget.grid(row=2, columnspan=2, sticky=tk.EW, padx=10, pady=5)
 
     def show_preview_subframe(self):
         if self.preview_subframe:
-            self.preview_subframe.destroy()
+            self.frame.remove_child(self.preview_subframe).destroy()
 
         if not self.node.plugin.show_preview:
-            self.frame.rowconfigure(4, weight=0)
             return
         elif not self.node.result:
             self.preview_subframe = tk.Frame(self.frame)
             self.preview_subframe.columnconfigure(0, weight=1)
             tk.Label(self.preview_subframe, text="no result").grid(sticky=tk.EW)
         elif all(isinstance(r, (str, bytes)) for r in self.node.result):
             text_result = "".join(self.node.result)
-            self.preview_subframe = tk.Frame(self.frame, highlightbackground="black", highlightthickness=3)
+            self.preview_subframe = tk.Frame(self.frame)
             self.preview_subframe.columnconfigure(0, weight=1)
             self.preview_subframe.rowconfigure(1, weight=1)
             n_lines = len(text_result.splitlines())
             tk.Label(self.preview_subframe, text=f"Text Preview {n_lines} Lines").grid(sticky=tk.NSEW)
             text = tk.Text(self.preview_subframe)
             text.insert("1.0", text_result)
             text["state"] = "disabled"
             text.grid(sticky=tk.NSEW)
         else:
             try:
                 df = concat_dataframes(self.node.result)
-                self.preview_subframe = TabularDataFrame(self.frame, highlightbackground="black", highlightthickness=3)
+                self.preview_subframe = TabularDataFrame(self.frame)
                 self.preview_subframe.set_dataframe(df)
                 self.preview_subframe.set_sort_order(self.node.sort_column or 0, self.node.sort_descending)
                 self.preview_subframe.set_callback(self.preview_changed_callback)
             except (TypeError, ValueError):
                 self.preview_subframe = tk.Frame(self.frame)
                 self.preview_subframe.columnconfigure(0, weight=1)
                 tk.Label(self.preview_subframe, text="no result").grid(sticky=tk.EW)
 
-        self.preview_subframe.grid(row=4, columnspan=2, sticky=tk.NSEW)
+        self.frame.add_child(self.preview_subframe)
 
     def preview_changed_callback(self, offset: int, sort_col: int, sort_desc: bool) -> None:
         self.node.sort_column = sort_col
         self.node.sort_descending = sort_desc
 
     def name_changed_callback(self, *_):
         name = self.name_var.get()
@@ -229,59 +225,48 @@
 
     def config_change_task_callback(self):
         self.config_change_task = None
 
         self.node_update_thread = threading.Thread(target=self.node.prerun, args=(self.logger,))
         self.node_update_thread.start()
 
-        self.logger_subframe.clear()
-        self.logger_subframe.grid(row=5, columnspan=2, sticky=tk.NSEW)
-        self.logger_subframe.after(100, self.config_change_task_callback_2)
-        self.change_callback(self.node)
+        self.config_change_task_callback_2()
 
     def config_change_task_callback_2(self):
         self.logger.poll()
 
         if self.node_update_thread.is_alive():
-            self.logger_subframe.after(100, self.config_change_task_callback_2)
+            self.frame.after(100, self.config_change_task_callback_2)
             return
 
         self.node_update_thread.join()
 
         # XXX stop the form scrolling away when it is refreshed, by putting
         # it back where it belongs.
         pos1, pos2 = self.config_scrollbar.get()
         self.show_preview_subframe()
         self.configurator.update()
         self.frame.update()
         self.config_canvas.yview_moveto(pos1)
         self.config_scrollbar.set(pos1, pos2)
 
-        if self.logger_subframe.count == 0:
-            self.logger_subframe.grid_forget()
-
-    #        else:
-    #            self.logger_subframe.progress_hide()
-
     def choose_plugin(self, plugin_class):
         self.node.plugin = plugin_class()
         self.node.prerun(self.logger)
         self.node.is_dirty = True
         self.show_config_subframe()
         self.change_callback(self.node)
 
     def destroy(self):
         if self.config_change_task:
             self.frame.after_cancel(self.config_change_task)
         if self.config_subframe:
             self.config_subframe.destroy()
         if self.preview_subframe:
             self.preview_subframe.destroy()
-        if self.logger_subframe:
-            self.logger_subframe.destroy()
 
 
 class ButtonMenu:  # pylint: disable=R0903
     def __init__(self, tk_parent, buttons):
         self.frame = tk.Frame(tk_parent)
         for button_number, (button_label, button_command) in enumerate(buttons):
             tk.Button(self.frame, text=button_label, command=button_command).grid(
@@ -367,146 +352,151 @@
                 ("Export Config", self.config_export),
                 ("Tidy Graph", self.graph_tidy),
                 ("Run", self.program_run),
                 ("Exit", self.program_exit),
             ],
         )
 
-        self.frame = tk.Frame(tk_parent)
-        self.frame.grid(sticky=tk.NSEW)
-
-        # The left (or top) pane, which contains the pipeline graph
-        self.canvas = FlippyCanvas(self.frame, bg="skyblue")
+        # +--------------------------------------------+
+        # | ButtonMenu                                 |
+        # +--------------+-----------------------------+
+        # | tree_canvas  | config_wrapper.subframe     |
+        # |              |                             |
+        # |              +-----------------------------+
+        # |              | configw_wrapper.preview     |
+        # |              |                             |
+        # +--------------+-----------------------------+
+        # | logger_subframe                            |
+        # +--------------------------------------------+
 
-        # The right (or bottom) pane, which contains everything else.
-        # 0: The node label
-        # 1: The plugin description
-        # 2: Node notes / add notes button
-        # 3: Configuration
-        # 4: Preview pane
-        # 5: Log output
+        # top level is a vertical layout with logs along the bottom
+        self.frame = ResizingFrame(tk_parent, orientation=ResizingFrame.Orientation.VERTICAL, bg="darkgrey")
+        self.frame.grid(sticky=tk.NSEW)
 
-        self.subframe = tk.Frame(self.frame)
-        self.subframe.columnconfigure(0, weight=1)
-        self.subframe.columnconfigure(1, weight=0)
-        self.subframe.rowconfigure(0, weight=0)
-        self.subframe.rowconfigure(1, weight=0)
-        self.subframe.rowconfigure(2, weight=0)
-        self.subframe.rowconfigure(3, weight=1)
-        self.subframe.rowconfigure(4, weight=1)
-        self.subframe.rowconfigure(5, weight=0)
+        # next is a division between the tree view and the configuration
+        self.main_subframe = ResizingFrame(self.frame, orientation=ResizingFrame.Orientation.AUTOMATIC, bg="darkgrey")
+        self.frame.add_child(self.main_subframe, weight=4)
 
-        self.frame.bind("<Configure>", self.on_frame_configure, add=True)
+        self.logger_subframe = LoggerFrame(self.frame)
+        self.logger = self.logger_subframe.get_logger("")
+        self.logger_subframe_show_task()
 
-        self.logger_subframe = LoggerFrame(self.subframe)
-        self.logger_subframe.grid(row=5, columnspan=2, sticky=tk.NSEW)
+        self.tree_canvas = FlippyCanvas(self.main_subframe, bg="skyblue")
+        self.main_subframe.add_child(self.tree_canvas)
 
         if config_filename:
             self.config_load(config_filename)
         else:
             self.config_new()
 
+    def logger_subframe_show_task(self):
+        if self.logger_subframe.count > 0:
+            self.frame.add_child(self.logger_subframe)
+            self.frame.after(100, self.logger_subframe_hide_task)
+        else:
+            self.frame.after(100, self.logger_subframe_show_task)
+
+    def logger_subframe_hide_task(self):
+        if self.logger_subframe.count == 0:
+            self.frame.remove_child(self.logger_subframe)
+            self.frame.after(100, self.logger_subframe_show_task)
+        else:
+            self.frame.after(100, self.logger_subframe_hide_task)
+
     def config_new(self):
         if self.config_changed:
             if not messagebox.askokcancel("Clear Config", "Clear unsaved config?"):
                 return
         self.config_changed = False
         self.config_filename = None
         if self.graph_wrapper:
             self.graph_wrapper.destroy()
         self.graph = PipelineGraph()
-        self.graph_wrapper = GraphWrapper(self.canvas, self.graph, self.node_select)
+        self.graph_wrapper = GraphWrapper(self.tree_canvas, self.graph, self.node_select)
         self.graph_wrapper.add_new_node()
 
     def config_load(self, filename=None):
         if not filename:
             filename = ask_open_filename(file_types=[(".INI Config File", "*.ini")])
         if not filename:
             return
         self.config_filename = filename
         if self.graph_wrapper:
             self.graph_wrapper.destroy()
         self.graph = read_config(filename)
-        self.graph_wrapper = GraphWrapper(self.canvas, self.graph, self.node_select)
+        self.graph_wrapper = GraphWrapper(self.tree_canvas, self.graph, self.node_select)
         self.node_select(None)
 
     def config_save(self, filename=None):
         if not filename:
             filename = ask_saveas_filename(
                 initial_file=self.config_filename,
                 file_types=[(".INI Config File", "*.ini")],
             )
         if not filename:
             return
         write_config(self.graph, filename)
         self.config_changed = False
-        # XXX there should be a self.graph_wrapper.refresh()
-        # Names may have changed on save
+        # Names may have changed on save so redraw the tree
         self.graph_wrapper.destroy()
-        self.graph_wrapper = GraphWrapper(self.canvas, self.graph, self.node_select)
+        self.graph_wrapper = GraphWrapper(self.tree_canvas, self.graph, self.node_select)
 
     def config_export(self, filename=None):
         if not filename:
             if self.config_filename:
                 initialfile = self.config_filename.removesuffix(".ini") + ".dot"
             else:
                 initialfile = None
             filename = ask_saveas_filename(initial_file=initialfile, file_types=[("Graphviz File", "*.dot")])
         if not filename:
             return
         export_config_graphviz(self.graph, filename)
 
     def graph_tidy(self):
         self.graph.tidy()
-        # XXX there should be a self.graph_wrapper.refresh()
         self.graph_wrapper.destroy()
-        self.graph_wrapper = GraphWrapper(self.canvas, self.graph, self.node_select)
+        self.graph_wrapper = GraphWrapper(self.tree_canvas, self.graph, self.node_select)
 
     def program_run(self):
         RunWindow(self.graph)
 
     def program_exit(self):
         if not self.config_changed or messagebox.askokcancel("Exit", "Exit CountESS without saving config?"):
             self.tk_parent.quit()
 
     def node_select(self, node):
-        for widget in self.subframe.winfo_children():
-            widget.destroy()
         if node:
+            new_config_wrapper = ConfiguratorWrapper(self.main_subframe, node, self.logger, self.node_changed)
             if self.config_wrapper:
-                self.config_wrapper.destroy()
-            self.config_wrapper = ConfiguratorWrapper(self.subframe, node, self.node_changed)
+                self.main_subframe.replace_child(self.config_wrapper.frame, new_config_wrapper.frame)
+            else:
+                self.main_subframe.add_child(new_config_wrapper.frame, weight=4)
+
+            self.config_wrapper = new_config_wrapper
+
+        elif self.config_wrapper:
+            self.main_subframe.remove_child(self.config_wrapper.frame).destroy()
+            self.config_wrapper = None
 
     def node_changed(self, node):
         self.config_changed = True
         self.graph_wrapper.node_changed(node)
 
-    def on_frame_configure(self, event):
-        """Swaps layout around when the window goes from landscape to portrait"""
-        if event.width > event.height:
-            x = event.width // 4
-            self.canvas.place(x=0, y=0, w=x, h=event.height)
-            self.subframe.place(x=x, y=0, w=event.width - x, h=event.height)
-        else:
-            y = event.height // 4
-            self.canvas.place(x=0, y=0, w=event.width, h=y)
-            self.subframe.place(x=0, y=y, w=event.width, h=event.height - y)
-
 
 class SplashScreen:
     def __init__(self, tk_root):
         bg = "skyblue"
         self.splash = tk.Toplevel(tk_root, bg=bg)
         self.splash.attributes("-type", "dialog")
 
         font = ("TkHeadingFont", 16, "bold")
         tk.Label(self.splash, text=f"CountESS {VERSION}", font=font, bg=bg).grid(padx=10, pady=10)
         tk.Label(self.splash, image=get_icon(tk_root, "countess"), bg=bg).grid(padx=10)
 
-        self.splash.after(3500, self.destroy)
+        self.splash.after(2500, self.destroy)
 
     def destroy(self):
         self.splash.destroy()
 
 
 def make_root():
     try:
```

### Comparing `countess-0.0.58/countess/gui/mini_browser.py` & `countess-0.0.59/countess/gui/mini_browser.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/gui/tabular.py` & `countess-0.0.59/countess/gui/tabular.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from math import ceil, floor, isinf, isnan
 from tkinter import ttk
 from typing import Callable, Optional, Union
 
 import pandas as pd
 from pandas.api.types import is_integer_dtype, is_numeric_dtype
 
-from countess.gui.widgets import copy_to_clipboard, get_icon
+from countess.gui.widgets import ResizingFrame, copy_to_clipboard, get_icon
 
 # XXX columns should automatically resize based on information
 # from _column_xscrollcommand which can tell if they're
 # overflowing.  Or maybe use
 #    df['seq'].str.len().max() to get max length of a string column
 # etc etc.
 
@@ -85,32 +85,40 @@
     column_formats: list[str] = []
     scrollbar = None
     index_cols = 0
     sort_by_col = None
     sort_ascending = True
     callback: Optional[Callable[[int, int, bool], None]] = None
 
-    def reset(self):
-        if self.subframe:
-            self.subframe.destroy()
-        self.rowconfigure(0, weight=1)
+    def __init__(self, *a, **k):
+        super().__init__(*a, **k)
+        self.rowconfigure(0, weight=0)
+        self.rowconfigure(1, weight=0)
+        self.rowconfigure(2, weight=1)
         self.columnconfigure(0, weight=1)
-        self.subframe = tk.Frame(self)
-        self.subframe.rowconfigure(0, weight=0)
-        self.subframe.rowconfigure(1, weight=0)
-        self.subframe.rowconfigure(2, weight=1)
-        self.subframe.grid(sticky=tk.NSEW)
+        self.columnconfigure(1, weight=0)
 
-    def set_dataframe(self, dataframe: pd.DataFrame, offset: Optional[int] = 0):
-        self.reset()
-        assert self.subframe
+        self.label = tk.Label(self, text="Dataframe Preview")
+        self.label.pack(fill="x")
+
+        self.label_frame = tk.Frame(self, height=60)
+        self.label_frame.pack(fill="x")
+
+        self.scrollbar = ttk.Scrollbar(self, orient=tk.VERTICAL)
+        self.scrollbar.pack(side="right", fill="y")
+        self.scrollbar["command"] = self._scrollbar_command
+
+        self.bind("<Configure>", self._configure)
 
+    def set_dataframe(self, dataframe: pd.DataFrame, offset: Optional[int] = 0):
         self.dataframe = dataframe
         self.length = len(dataframe)
 
+        # clean up column names
+
         if hasattr(self.dataframe.index, "names") and hasattr(self.dataframe.index, "dtypes"):
             # MultiIndex case
             column_names = list(self.dataframe.index.names) + list(self.dataframe.columns)
             column_dtypes = list(self.dataframe.index.dtypes) + list(self.dataframe.dtypes)
             index_frame = self.dataframe.index.to_frame()
             self.column_formats = [column_format_for(index_frame[name]) for name in dataframe.index.names] + [
                 column_format_for(dataframe[name]) for name in dataframe.columns
@@ -128,75 +136,68 @@
             # if it doesn't have a name, don't bother displaying it
             # XXX it's probably just a RangeIndex, should we display it anyway?
             column_names = list(self.dataframe.columns)
             column_dtypes = list(self.dataframe.dtypes)
             self.column_formats = [column_format_for(dataframe[name]) for name in dataframe.columns]
             self.index_cols = 0
 
-        if len(column_names) == 0:
-            label = tk.Label(self.subframe, text="Dataframe Preview\n\nno data")
-            label.grid(row=0, column=0, sticky=tk.NSEW)
+        n_columns = len(column_names)
+        if n_columns == 0:
+            self.label["text"] = "Dataframe Preview\n\nno data"
             return
 
-        title = tk.Label(self.subframe, text=f"Dataframe Preview {len(self.dataframe)} rows")
-        title.grid(row=0, column=0, columnspan=len(column_names) * 2 + 1, sticky=tk.NSEW, pady=5)
-
+        # make labels for all the columns
         ### XXX add in proper handling for MultiIndexes here
 
-        # Even-numbered columns are the data columns
+        for label in self.labels:
+            label.destroy()
 
         self.labels = []
         for num, (name, dtype) in enumerate(zip(column_names, column_dtypes)):
             if type(name) is tuple:
                 name = "\n".join([str(n) for n in name])
             else:
                 name = str(name)
             is_index = " (index)" if num < self.index_cols else ""
-            label = tk.Label(
-                self.subframe,
+            column_label = tk.Label(
+                self.label_frame,
                 text=f"{name}\n{dtype}{is_index}",
                 image=get_icon(self, "sort_un"),
                 compound=tk.RIGHT,
             )
-            label.grid(row=1, column=num * 2, sticky=tk.EW)
-            label.bind("<Button-1>", partial(self._label_button_1, num))
-            self.subframe.columnconfigure(num * 2, minsize=10, weight=1)
-            self.labels.append(label)
-
-        # Between them are blank columns which provide a handle for adjusting the column
-        # widths left and right
-
-        for num in range(0, len(column_names) - 1):
-            adjuster = tk.Frame(self.subframe, width=3, cursor="sb_h_double_arrow")
-            adjuster.grid(row=1, rowspan=2, column=num * 2 + 1, sticky=tk.NSEW)
-            adjuster.bind("<B1-Motion>", partial(self._column_adjust, num))
-
-        if len(self.dataframe) == 0:
-            label = tk.Label(self.subframe, text="no data")
-            label.grid(row=2, column=0, columnspan=len(column_names), sticky=tk.NSEW)
-            return
+            column_label.bind("<Button-1>", partial(self._label_button_1, num))
+            self.labels.append(column_label)
 
-        self.columns = [tk.Text(self.subframe) for _ in column_names]
-        for num, column in enumerate(self.columns):
-            column.grid(sticky=tk.NSEW, row=2, column=num * 2)
-            column["wrap"] = tk.NONE
-            column["xscrollcommand"] = partial(self._column_xscrollcommand, num)
-            column["yscrollcommand"] = self._column_yscrollcommand
-            column.bind("<Button-4>", self._column_scroll)
-            column.bind("<Button-5>", self._column_scroll)
-            column.bind("<<Selection>>", partial(self._column_selection, num))
-            column.bind("<Control-C>", self._column_copy)
-            column.bind("<<Copy>>", self._column_copy)
-        if self.columns:
-            self.columns[0].bind("<Configure>", self._column_configure)
+        # make a subframe to hold the column texts
 
-        self.scrollbar = ttk.Scrollbar(self.subframe, orient=tk.VERTICAL)
-        self.scrollbar.grid(sticky=tk.NS, row=2, column=len(self.columns) * 2 - 1)
-        self.scrollbar["command"] = self._scrollbar_command
-        self.refresh(offset)
+        if self.subframe:
+            self.subframe.destroy()
+        self.subframe = ResizingFrame(self, orientation=ResizingFrame.Orientation.HORIZONTAL, bg="darkgrey")
+        self.subframe.pack(side="left", fill="both", expand=True)
+
+        self.label["text"] = f"Dataframe Preview {len(self.dataframe)} rows"
+
+        self.columns = []
+        for num, (name, dtype) in enumerate(zip(column_names, column_dtypes)):
+            column_text = tk.Text(self.subframe)
+            self.subframe.add_child(column_text)
+            column_text["wrap"] = tk.NONE
+            column_text["yscrollcommand"] = self._column_yscrollcommand
+            column_text.bind("<Button-4>", self._column_scroll)
+            column_text.bind("<Button-5>", self._column_scroll)
+            column_text.bind("<<Selection>>", partial(self._column_selection, num))
+            column_text.bind("<Control-C>", self._column_copy)
+            column_text.bind("<<Copy>>", self._column_copy)
+            column_text.bind("<Configure>", partial(self._column_configure, num))
+            self.columns.append(column_text)
+
+    def _column_configure(self, num, ev):
+        # when the column changes position, move the labels around
+        # to match
+        self.labels[num].place(x=ev.x, width=ev.width)
 
     def refresh(self, new_offset=0):
         # Refreshes the column widgets.
         # XXX should handle new_height as well, as this changes a fair bit
         # with some window managers. Needs refactoring.
 
         new_offset = max(0, min(self.length - self.height, int(new_offset)))
@@ -282,55 +283,47 @@
 
     def _label_button_1(self, num, event):
         """Click on column labels to set sort order"""
         self.set_sort_order(num)
         if self.callback:
             self.callback(self.offset, self.sort_by_col, not self.sort_ascending)
 
-    def _column_adjust(self, num, event):
-        """Adjust column widths left and right by dragging the dummy columns"""
-        w0 = self.labels[num].winfo_width()
-        w1 = self.labels[num + 1].winfo_width()
-        self.subframe.columnconfigure(num * 2, minsize=w0 + event.x)
-        self.subframe.columnconfigure(num * 2 + 2, minsize=w1 - event.x)
-
     def _scrollbar_command(self, command, *parameters):
         # Detect scrollbar movement and move self.offset
         # to compensate.
         if command == "moveto":
             self.refresh(float(parameters[0]) * (self.length - self.height))
         elif command == "scroll":
             self.refresh(self.offset + int(parameters[0]))
         else:
             self.refresh()
 
-    def _column_xscrollcommand(self, num, x1, x2):
-        # XXX this gets called as the table is displayed
-        # if x2 < 1.0 this column is partially hidden.
-        pass
-
     # XXX the following two functions are clever but not
     # very efficient!  There's got to be a nicer way of
     # detecting this surely?
 
     def _column_yscrollcommand(self, y1, y2):
         # All this actually does is to detect if there's
         # too many rows for the window, in which case it
         # trims them off.  Once there's the right number
         # of rows, this won't get called any more.
-        span = int((float(y2) - float(y1)) * self.height)
+        span = int((float(y2) - float(y1)) * self.height) + 1
         if span > 0 and span != self.height:
             self.height = span
             self.refresh()
 
-    def _column_configure(self, *_):
-        # If we've resized the window, start with a huge
-        # number of rows and let _cw_yscrollcommand trim
-        # it back down again.  Probably could be more
-        # sensible.
+    def _configure(self, *_):
+        # the delay lets the sub-elements configure
+        # themselves before we try to measure them.
+        self.after(10, self._reset_height)
+
+    def _reset_height(self):
+        # Start with a huge number of rows and let
+        # _cw_yscrollcommand trim it back down again.
+        # Probably could be more efficient.
         self.height = min(self.length, 1000)
         self.refresh()
 
     def _column_scroll(self, event):
         # Detect scrollwheel motion on any of the columns
         if event.num == 4:
             self.refresh(self.offset - 5)
```

### Comparing `countess-0.0.58/countess/gui/tree.py` & `countess-0.0.59/countess/gui/tree.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/plugins/collate.py` & `countess-0.0.59/countess/plugins/collate.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/plugins/column.py` & `countess-0.0.59/countess/plugins/column.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/plugins/correlation.py` & `countess-0.0.59/countess/plugins/correlation.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/plugins/csv.py` & `countess-0.0.59/countess/plugins/csv.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/plugins/data_table.py` & `countess-0.0.59/countess/plugins/data_table.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/plugins/expression.py` & `countess-0.0.59/countess/plugins/expression.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/plugins/fastq.py` & `countess-0.0.59/countess/plugins/fastq.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/plugins/group_by.py` & `countess-0.0.59/countess/plugins/group_by.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/plugins/hgvs_parser.py` & `countess-0.0.59/countess/plugins/hgvs_parser.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/plugins/join.py` & `countess-0.0.59/countess/plugins/join.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/plugins/mutagenize.py` & `countess-0.0.59/countess/plugins/mutagenize.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/plugins/pivot.py` & `countess-0.0.59/countess/plugins/pivot.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/plugins/python.py` & `countess-0.0.59/countess/plugins/python.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/plugins/regex.py` & `countess-0.0.59/countess/plugins/regex.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/plugins/sequence.py` & `countess-0.0.59/countess/plugins/sequence.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/plugins/variant.py` & `countess-0.0.59/countess/plugins/variant.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/utils/pandas.py` & `countess-0.0.59/countess/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/utils/parallel.py` & `countess-0.0.59/countess/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess/utils/variant.py` & `countess-0.0.59/countess/utils/variant.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess.egg-info/PKG-INFO` & `countess-0.0.59/countess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.58
+Version: 0.0.59
 Summary: CountESS
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -30,15 +30,15 @@
 Requires-Dist: pylint~=2.17; extra == "dev"
 Requires-Dist: types-psutil~=5.9.5; extra == "dev"
 Requires-Dist: types-ttkthemes~=3.2; extra == "dev"
 Requires-Dist: twine==4.0.2; extra == "dev"
 Requires-Dist: pandas-stubs~=2.1.0; extra == "dev"
 Requires-Dist: pytest~=7.2; extra == "dev"
 
-# CountESS 0.0.58
+# CountESS 0.0.59
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.58/countess.egg-info/SOURCES.txt` & `countess-0.0.59/countess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/countess.egg-info/entry_points.txt` & `countess-0.0.59/countess.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/pyproject.toml` & `countess-0.0.59/pyproject.toml`

 * *Files identical despite different names*

### Comparing `countess-0.0.58/tests/test_plugins.py` & `countess-0.0.59/tests/test_plugins.py`

 * *Files identical despite different names*

