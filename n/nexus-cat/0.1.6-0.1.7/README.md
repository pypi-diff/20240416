# Comparing `tmp/nexus-cat-0.1.6.tar.gz` & `tmp/nexus-cat-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus-cat-0.1.6.tar", last modified: Sun Apr  7 21:27:55 2024, max compression
+gzip compressed data, was "nexus-cat-0.1.7.tar", last modified: Tue Apr 16 14:25:50 2024, max compression
```

## Comparing `nexus-cat-0.1.6.tar` & `nexus-cat-0.1.7.tar`

### file list

```diff
@@ -1,44 +1,76 @@
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-07 21:27:55.231419 nexus-cat-0.1.6/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     1076 2024-04-06 13:06:16.000000 nexus-cat-0.1.6/LICENSE
--rw-r--r--   0 perraju   (1000) perraju   (1000)      646 2024-04-07 21:27:55.231419 nexus-cat-0.1.6/PKG-INFO
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     1620 2024-04-06 22:29:20.000000 nexus-cat-0.1.6/README.md
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-07 21:27:55.231419 nexus-cat-0.1.6/nexus/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      175 2024-04-07 21:27:44.000000 nexus-cat-0.1.6/nexus/__init__.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-07 21:27:55.231419 nexus-cat-0.1.6/nexus/core/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      145 2024-04-06 20:39:23.000000 nexus-cat-0.1.6/nexus/core/__init__.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     8816 2024-04-06 21:10:52.000000 nexus-cat-0.1.6/nexus/core/atom.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     2616 2024-03-31 10:20:59.000000 nexus-cat-0.1.6/nexus/core/box.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)    17034 2024-04-07 19:13:18.000000 nexus-cat-0.1.6/nexus/core/cluster.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     2141 2024-03-31 11:54:45.000000 nexus-cat-0.1.6/nexus/core/cutoff.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)    31548 2024-04-07 20:01:19.000000 nexus-cat-0.1.6/nexus/core/system.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-07 21:27:55.231419 nexus-cat-0.1.6/nexus/data/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     7530 2024-03-31 11:07:05.000000 nexus-cat-0.1.6/nexus/data/__init__.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-07 21:27:55.231419 nexus-cat-0.1.6/nexus/extensions/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     2021 2024-04-06 20:41:19.000000 nexus-cat-0.1.6/nexus/extensions/Na.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)    14848 2024-04-07 21:27:44.000000 nexus-cat-0.1.6/nexus/extensions/SiOz.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)       35 2024-04-06 21:21:46.000000 nexus-cat-0.1.6/nexus/extensions/__init__.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-07 21:27:55.231419 nexus-cat-0.1.6/nexus/io/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      612 2024-04-06 20:42:58.000000 nexus-cat-0.1.6/nexus/io/__init__.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      707 2024-04-05 12:20:44.000000 nexus-cat-0.1.6/nexus/io/make_lines_unique.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     4938 2024-04-07 19:13:18.000000 nexus-cat-0.1.6/nexus/io/read_and_create_system.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     1032 2024-03-31 11:09:48.000000 nexus-cat-0.1.6/nexus/io/read_lattices_properties.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      662 2024-03-31 11:10:34.000000 nexus-cat-0.1.6/nexus/io/read_number_of_configurations.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)    28785 2024-04-07 13:55:57.000000 nexus-cat-0.1.6/nexus/io/result.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      722 2024-04-05 17:39:46.000000 nexus-cat-0.1.6/nexus/io/write_list_of_files.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)    13820 2024-04-07 19:13:18.000000 nexus-cat-0.1.6/nexus/main.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-07 21:27:55.231419 nexus-cat-0.1.6/nexus/settings/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)       30 2024-04-06 20:43:10.000000 nexus-cat-0.1.6/nexus/settings/__init__.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     5787 2024-04-05 17:06:57.000000 nexus-cat-0.1.6/nexus/settings/parameter.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     9113 2024-04-06 21:49:55.000000 nexus-cat-0.1.6/nexus/settings/settings.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-07 21:27:55.231419 nexus-cat-0.1.6/nexus/utils/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)       97 2024-04-06 20:43:29.000000 nexus-cat-0.1.6/nexus/utils/__init__.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     1150 2024-03-31 12:26:32.000000 nexus-cat-0.1.6/nexus/utils/generate_color_gradient.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      927 2024-04-06 22:08:51.000000 nexus-cat-0.1.6/nexus/utils/print_title.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-07 21:27:55.231419 nexus-cat-0.1.6/nexus_cat.egg-info/
--rw-r--r--   0 perraju   (1000) perraju   (1000)      646 2024-04-07 21:27:55.000000 nexus-cat-0.1.6/nexus_cat.egg-info/PKG-INFO
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      834 2024-04-07 21:27:55.000000 nexus-cat-0.1.6/nexus_cat.egg-info/SOURCES.txt
--rw-rw-r--   0 perraju   (1000) perraju   (1000)        1 2024-04-07 21:27:55.000000 nexus-cat-0.1.6/nexus_cat.egg-info/dependency_links.txt
--rw-rw-r--   0 perraju   (1000) perraju   (1000)       25 2024-04-07 21:27:55.000000 nexus-cat-0.1.6/nexus_cat.egg-info/requires.txt
--rw-rw-r--   0 perraju   (1000) perraju   (1000)        6 2024-04-07 21:27:55.000000 nexus-cat-0.1.6/nexus_cat.egg-info/top_level.txt
--rw-rw-r--   0 perraju   (1000) perraju   (1000)       38 2024-04-07 21:27:55.231419 nexus-cat-0.1.6/setup.cfg
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      801 2024-04-07 21:27:44.000000 nexus-cat-0.1.6/setup.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-16 14:25:50.439286 nexus-cat-0.1.7/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     1076 2024-04-07 16:27:59.000000 nexus-cat-0.1.7/LICENSE
+-rw-r--r--   0 perraju   (1000) perraju   (1000)      646 2024-04-16 14:25:50.439286 nexus-cat-0.1.7/PKG-INFO
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     3674 2024-04-13 09:44:51.000000 nexus-cat-0.1.7/README.md
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-16 14:25:50.431287 nexus-cat-0.1.7/nexus/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      175 2024-04-16 14:25:01.000000 nexus-cat-0.1.7/nexus/__init__.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-16 14:25:50.431287 nexus-cat-0.1.7/nexus/core/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      145 2024-04-07 16:27:59.000000 nexus-cat-0.1.7/nexus/core/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     8816 2024-04-07 16:27:59.000000 nexus-cat-0.1.7/nexus/core/atom.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     2616 2024-04-07 16:27:59.000000 nexus-cat-0.1.7/nexus/core/box.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    17127 2024-04-16 14:25:01.000000 nexus-cat-0.1.7/nexus/core/cluster.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     2141 2024-04-07 16:27:59.000000 nexus-cat-0.1.7/nexus/core/cutoff.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    32716 2024-04-16 14:25:01.000000 nexus-cat-0.1.7/nexus/core/system.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-16 14:25:50.431287 nexus-cat-0.1.7/nexus/data/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     7530 2024-04-07 16:27:59.000000 nexus-cat-0.1.7/nexus/data/__init__.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-16 14:25:50.431287 nexus-cat-0.1.7/nexus/extensions/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     2021 2024-04-07 16:27:59.000000 nexus-cat-0.1.7/nexus/extensions/Na.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    24149 2024-04-16 14:25:01.000000 nexus-cat-0.1.7/nexus/extensions/SiOz.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       35 2024-04-07 16:27:59.000000 nexus-cat-0.1.7/nexus/extensions/__init__.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-16 14:25:50.431287 nexus-cat-0.1.7/nexus/io/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      612 2024-04-07 16:27:59.000000 nexus-cat-0.1.7/nexus/io/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      707 2024-04-07 16:27:59.000000 nexus-cat-0.1.7/nexus/io/make_lines_unique.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     4938 2024-04-07 17:30:39.000000 nexus-cat-0.1.7/nexus/io/read_and_create_system.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     1032 2024-04-07 16:27:59.000000 nexus-cat-0.1.7/nexus/io/read_lattices_properties.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      662 2024-04-07 16:27:59.000000 nexus-cat-0.1.7/nexus/io/read_number_of_configurations.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    31367 2024-04-16 14:25:01.000000 nexus-cat-0.1.7/nexus/io/result.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      722 2024-04-07 16:27:59.000000 nexus-cat-0.1.7/nexus/io/write_list_of_files.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    14408 2024-04-16 14:25:01.000000 nexus-cat-0.1.7/nexus/main.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-16 14:25:50.431287 nexus-cat-0.1.7/nexus/settings/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       30 2024-04-07 16:27:59.000000 nexus-cat-0.1.7/nexus/settings/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     5787 2024-04-07 16:27:59.000000 nexus-cat-0.1.7/nexus/settings/parameter.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     9113 2024-04-07 16:27:59.000000 nexus-cat-0.1.7/nexus/settings/settings.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-16 14:25:50.435287 nexus-cat-0.1.7/nexus/utils/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       97 2024-04-07 16:27:59.000000 nexus-cat-0.1.7/nexus/utils/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     1150 2024-04-07 16:27:59.000000 nexus-cat-0.1.7/nexus/utils/generate_color_gradient.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      927 2024-04-07 16:27:59.000000 nexus-cat-0.1.7/nexus/utils/print_title.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-16 14:25:50.435287 nexus-cat-0.1.7/nexus_cat.egg-info/
+-rw-r--r--   0 perraju   (1000) perraju   (1000)      646 2024-04-16 14:25:50.000000 nexus-cat-0.1.7/nexus_cat.egg-info/PKG-INFO
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     1603 2024-04-16 14:25:50.000000 nexus-cat-0.1.7/nexus_cat.egg-info/SOURCES.txt
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)        1 2024-04-16 14:25:50.000000 nexus-cat-0.1.7/nexus_cat.egg-info/dependency_links.txt
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       25 2024-04-16 14:25:50.000000 nexus-cat-0.1.7/nexus_cat.egg-info/requires.txt
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       17 2024-04-16 14:25:50.000000 nexus-cat-0.1.7/nexus_cat.egg-info/top_level.txt
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-16 14:25:50.435287 nexus-cat-0.1.7/nexus_test/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      175 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/__init__.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-16 14:25:50.435287 nexus-cat-0.1.7/nexus_test/core/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      145 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/core/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     8816 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/core/atom.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     2616 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/core/box.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    17034 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/core/cluster.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     2141 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/core/cutoff.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    31548 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/core/system.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-16 14:25:50.435287 nexus-cat-0.1.7/nexus_test/data/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     7530 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/data/__init__.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-16 14:25:50.435287 nexus-cat-0.1.7/nexus_test/extensions/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     2021 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/extensions/Na.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    14848 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/extensions/SiOz.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       35 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/extensions/__init__.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-16 14:25:50.439286 nexus-cat-0.1.7/nexus_test/io/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      612 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/io/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      707 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/io/make_lines_unique.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     4938 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/io/read_and_create_system.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     1032 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/io/read_lattices_properties.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      662 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/io/read_number_of_configurations.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    28785 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/io/result.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      722 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/io/write_list_of_files.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    13820 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/main.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-16 14:25:50.439286 nexus-cat-0.1.7/nexus_test/settings/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       30 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/settings/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     5787 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/settings/parameter.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     9113 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/settings/settings.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-16 14:25:50.439286 nexus-cat-0.1.7/nexus_test/utils/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       97 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/utils/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     1150 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/utils/generate_color_gradient.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      927 2024-04-07 21:17:38.000000 nexus-cat-0.1.7/nexus_test/utils/print_title.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       38 2024-04-16 14:25:50.439286 nexus-cat-0.1.7/setup.cfg
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      801 2024-04-16 14:25:47.000000 nexus-cat-0.1.7/setup.py
```

### Comparing `nexus-cat-0.1.6/LICENSE` & `nexus-cat-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.6/PKG-INFO` & `nexus-cat-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-cat
-Version: 0.1.6
+Version: 0.1.7
 Summary: Nexus is a Cluster Analysing Toolkit package for atomic systems.
 Home-page: https://github.com/JulienPerradin/nexus
 Author: Julien Perradin
 Author-email: julien.perradin@umontpellier.fr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nexus-cat-0.1.6/nexus/core/atom.py` & `nexus-cat-0.1.7/nexus/core/atom.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.6/nexus/core/box.py` & `nexus-cat-0.1.7/nexus/core/box.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.6/nexus/core/cluster.py` & `nexus-cat-0.1.7/nexus_test/core/cluster.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.6/nexus/core/cutoff.py` & `nexus-cat-0.1.7/nexus/core/cutoff.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.6/nexus/core/system.py` & `nexus-cat-0.1.7/nexus_test/core/system.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.6/nexus/data/__init__.py` & `nexus-cat-0.1.7/nexus/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.6/nexus/extensions/Na.py` & `nexus-cat-0.1.7/nexus/extensions/Na.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.6/nexus/extensions/SiOz.py` & `nexus-cat-0.1.7/nexus_test/extensions/SiOz.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.6/nexus/io/__init__.py` & `nexus-cat-0.1.7/nexus/io/__init__.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.6/nexus/io/make_lines_unique.py` & `nexus-cat-0.1.7/nexus/io/make_lines_unique.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.6/nexus/io/read_and_create_system.py` & `nexus-cat-0.1.7/nexus/io/read_and_create_system.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.6/nexus/io/read_lattices_properties.py` & `nexus-cat-0.1.7/nexus/io/read_lattices_properties.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.6/nexus/io/read_number_of_configurations.py` & `nexus-cat-0.1.7/nexus/io/read_number_of_configurations.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.6/nexus/io/result.py` & `nexus-cat-0.1.7/nexus_test/io/result.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.6/nexus/io/write_list_of_files.py` & `nexus-cat-0.1.7/nexus/io/write_list_of_files.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.6/nexus/main.py` & `nexus-cat-0.1.7/nexus_test/main.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.6/nexus/settings/parameter.py` & `nexus-cat-0.1.7/nexus/settings/parameter.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.6/nexus/settings/settings.py` & `nexus-cat-0.1.7/nexus/settings/settings.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.6/nexus/utils/generate_color_gradient.py` & `nexus-cat-0.1.7/nexus/utils/generate_color_gradient.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.6/nexus/utils/print_title.py` & `nexus-cat-0.1.7/nexus/utils/print_title.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.6/nexus_cat.egg-info/PKG-INFO` & `nexus-cat-0.1.7/nexus_cat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-cat
-Version: 0.1.6
+Version: 0.1.7
 Summary: Nexus is a Cluster Analysing Toolkit package for atomic systems.
 Home-page: https://github.com/JulienPerradin/nexus
 Author: Julien Perradin
 Author-email: julien.perradin@umontpellier.fr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nexus-cat-0.1.6/setup.py` & `nexus-cat-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nexus-cat',
-    version='0.1.6',
+    version='0.1.7',
     description='Nexus is a Cluster Analysing Toolkit package for atomic systems.',
     author='Julien Perradin',
     author_email='julien.perradin@umontpellier.fr',
     url='https://github.com/JulienPerradin/nexus',
     packages=find_packages(),
     install_requires=[
         'numpy',
```

