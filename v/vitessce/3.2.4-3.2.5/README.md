# Comparing `tmp/vitessce-3.2.4.tar.gz` & `tmp/vitessce-3.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vitessce-3.2.4.tar", last modified: Mon Apr 15 16:14:25 2024, max compression
+gzip compressed data, was "vitessce-3.2.5.tar", last modified: Tue Apr 16 20:21:46 2024, max compression
```

## Comparing `vitessce-3.2.4.tar` & `vitessce-3.2.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:14:25.962208 vitessce-3.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-15 16:12:24.000000 vitessce-3.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-15 16:12:24.000000 vitessce-3.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-04-15 16:14:25.962208 vitessce-3.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-04-15 16:12:24.000000 vitessce-3.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-15 16:12:24.000000 vitessce-3.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-15 16:14:25.962208 vitessce-3.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 16:12:24.000000 vitessce-3.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:14:25.954208 vitessce-3.2.4/vitessce/
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    75366 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14681 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/config_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14976 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:14:25.958208 vitessce-3.2.4/vitessce/data_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/data_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10297 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/data_utils/anndata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/data_utils/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/data_utils/multivec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/data_utils/ome.py
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20435 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    53910 2024-04-15 16:12:25.000000 vitessce-3.2.4/vitessce/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:14:25.958208 vitessce-3.2.4/vitessce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-04-15 16:14:25.000000 vitessce-3.2.4/vitessce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-15 16:14:25.000000 vitessce-3.2.4/vitessce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:14:25.000000 vitessce-3.2.4/vitessce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-15 16:14:25.000000 vitessce-3.2.4/vitessce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 16:14:25.000000 vitessce-3.2.4/vitessce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:21:46.086568 vitessce-3.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-16 20:19:36.000000 vitessce-3.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-16 20:19:36.000000 vitessce-3.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-04-16 20:21:46.086568 vitessce-3.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-04-16 20:19:36.000000 vitessce-3.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-16 20:19:36.000000 vitessce-3.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-16 20:21:46.086568 vitessce-3.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 20:19:36.000000 vitessce-3.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:21:46.078568 vitessce-3.2.5/vitessce/
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75366 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14681 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/config_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14976 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:21:46.082568 vitessce-3.2.5/vitessce/data_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/data_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10297 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/data_utils/anndata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/data_utils/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/data_utils/multivec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/data_utils/ome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20435 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53910 2024-04-16 20:19:36.000000 vitessce-3.2.5/vitessce/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:21:46.082568 vitessce-3.2.5/vitessce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-04-16 20:21:46.000000 vitessce-3.2.5/vitessce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-16 20:21:46.000000 vitessce-3.2.5/vitessce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:21:46.000000 vitessce-3.2.5/vitessce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-16 20:21:46.000000 vitessce-3.2.5/vitessce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 20:21:46.000000 vitessce-3.2.5/vitessce.egg-info/top_level.txt
```

### Comparing `vitessce-3.2.4/LICENSE` & `vitessce-3.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.4/PKG-INFO` & `vitessce-3.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitessce
-Version: 3.2.4
+Version: 3.2.5
 Summary: Jupyter widget facilitating interactive visualization of spatial single-cell data with Vitessce
 Author-email: Mark Keller <mark_keller@hms.harvard.edu>
 License: MIT License
         
         Copyright (c) 2020 Gehlenborg Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `vitessce-3.2.4/README.md` & `vitessce-3.2.5/README.md`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.4/pyproject.toml` & `vitessce-3.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0", "wheel>=0.38.4"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vitessce"
-version = "3.2.4"
+version = "3.2.5"
 authors = [
   { name="Mark Keller", email="mark_keller@hms.harvard.edu" },
 ]
 description = "Jupyter widget facilitating interactive visualization of spatial single-cell data with Vitessce"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
```

### Comparing `vitessce-3.2.4/setup.cfg` & `vitessce-3.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.4/vitessce/__init__.py` & `vitessce-3.2.5/vitessce/__init__.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.4/vitessce/config.py` & `vitessce-3.2.5/vitessce/config.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.4/vitessce/config_converter.py` & `vitessce-3.2.5/vitessce/config_converter.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.4/vitessce/constants.py` & `vitessce-3.2.5/vitessce/constants.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.4/vitessce/data_utils/anndata.py` & `vitessce-3.2.5/vitessce/data_utils/anndata.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.4/vitessce/data_utils/entities.py` & `vitessce-3.2.5/vitessce/data_utils/entities.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.4/vitessce/data_utils/multivec.py` & `vitessce-3.2.5/vitessce/data_utils/multivec.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.4/vitessce/data_utils/ome.py` & `vitessce-3.2.5/vitessce/data_utils/ome.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.4/vitessce/export.py` & `vitessce-3.2.5/vitessce/export.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.4/vitessce/repr.py` & `vitessce-3.2.5/vitessce/repr.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.4/vitessce/routes.py` & `vitessce-3.2.5/vitessce/routes.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.4/vitessce/utils.py` & `vitessce-3.2.5/vitessce/utils.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.4/vitessce/widget.py` & `vitessce-3.2.5/vitessce/widget.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.4/vitessce/wrappers.py` & `vitessce-3.2.5/vitessce/wrappers.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.4/vitessce.egg-info/PKG-INFO` & `vitessce-3.2.5/vitessce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitessce
-Version: 3.2.4
+Version: 3.2.5
 Summary: Jupyter widget facilitating interactive visualization of spatial single-cell data with Vitessce
 Author-email: Mark Keller <mark_keller@hms.harvard.edu>
 License: MIT License
         
         Copyright (c) 2020 Gehlenborg Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `vitessce-3.2.4/vitessce.egg-info/SOURCES.txt` & `vitessce-3.2.5/vitessce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vitessce-3.2.4/vitessce.egg-info/requires.txt` & `vitessce-3.2.5/vitessce.egg-info/requires.txt`

 * *Files identical despite different names*

