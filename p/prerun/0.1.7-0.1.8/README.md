# Comparing `tmp/prerun-0.1.7.tar.gz` & `tmp/prerun-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prerun-0.1.7.tar", last modified: Mon Apr 15 00:44:58 2024, max compression
+gzip compressed data, was "prerun-0.1.8.tar", last modified: Tue Apr 16 04:23:13 2024, max compression
```

## Comparing `prerun-0.1.7.tar` & `prerun-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:44:58.758834 prerun-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-15 00:44:51.000000 prerun-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-15 00:44:58.758834 prerun-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 00:44:51.000000 prerun-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-15 00:44:51.000000 prerun-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 00:44:58.758834 prerun-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:44:58.758834 prerun-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:44:58.758834 prerun-0.1.7/src/prerun/
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-04-15 00:44:51.000000 prerun-0.1.7/src/prerun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 00:44:51.000000 prerun-0.1.7/src/prerun/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:44:58.758834 prerun-0.1.7/src/prerun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-15 00:44:58.000000 prerun-0.1.7/src/prerun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-15 00:44:58.000000 prerun-0.1.7/src/prerun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 00:44:58.000000 prerun-0.1.7/src/prerun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 00:44:58.000000 prerun-0.1.7/src/prerun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 00:44:58.000000 prerun-0.1.7/src/prerun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 00:44:58.000000 prerun-0.1.7/src/prerun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:23:13.143890 prerun-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-16 04:23:06.000000 prerun-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-16 04:23:13.143890 prerun-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 04:23:06.000000 prerun-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-16 04:23:06.000000 prerun-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 04:23:13.143890 prerun-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:23:13.139890 prerun-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:23:13.143890 prerun-0.1.8/src/prerun/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-16 04:23:06.000000 prerun-0.1.8/src/prerun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 04:23:06.000000 prerun-0.1.8/src/prerun/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-16 04:23:06.000000 prerun-0.1.8/src/prerun/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-16 04:23:06.000000 prerun-0.1.8/src/prerun/recv_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-16 04:23:06.000000 prerun-0.1.8/src/prerun/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-16 04:23:06.000000 prerun-0.1.8/src/prerun/sigint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:23:13.143890 prerun-0.1.8/src/prerun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-16 04:23:13.000000 prerun-0.1.8/src/prerun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-16 04:23:13.000000 prerun-0.1.8/src/prerun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 04:23:13.000000 prerun-0.1.8/src/prerun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-16 04:23:13.000000 prerun-0.1.8/src/prerun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 04:23:13.000000 prerun-0.1.8/src/prerun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 04:23:13.000000 prerun-0.1.8/src/prerun.egg-info/top_level.txt
```

### Comparing `prerun-0.1.7/LICENSE` & `prerun-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `prerun-0.1.7/PKG-INFO` & `prerun-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prerun
-Version: 0.1.7
+Version: 0.1.8
 Summary: Prerun
 License: Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `prerun-0.1.7/src/prerun.egg-info/PKG-INFO` & `prerun-0.1.8/src/prerun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prerun
-Version: 0.1.7
+Version: 0.1.8
 Summary: Prerun
 License: Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

