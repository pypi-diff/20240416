# Comparing `tmp/ansys-api-additive-1.6.8.tar.gz` & `tmp/ansys_api_additive-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-api-additive-1.6.8.tar", last modified: Fri Mar 15 17:54:09 2024, max compression
+gzip compressed data, was "ansys_api_additive-1.7.0.tar", last modified: Tue Apr 16 20:53:40 2024, max compression
```

## Comparing `ansys-api-additive-1.6.8.tar` & `ansys_api_additive-1.7.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:54:09.107071 ansys-api-additive-1.6.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-15 17:54:00.000000 ansys-api-additive-1.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-03-15 17:54:09.107071 ansys-api-additive-1.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-03-15 17:54:00.000000 ansys-api-additive-1.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:54:09.099071 ansys-api-additive-1.6.8/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:54:09.099071 ansys-api-additive-1.6.8/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:54:09.103071 ansys-api-additive-1.6.8/ansys/api/additive/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-15 17:54:00.000000 ansys-api-additive-1.6.8/ansys/api/additive/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-15 17:54:00.000000 ansys-api-additive-1.6.8/ansys/api/additive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 17:54:00.000000 ansys-api-additive-1.6.8/ansys/api/additive/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:54:09.103071 ansys-api-additive-1.6.8/ansys/api/additive/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-15 17:54:00.000000 ansys-api-additive-1.6.8/ansys/api/additive/v0/about.proto
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-03-15 17:54:00.000000 ansys-api-additive-1.6.8/ansys/api/additive/v0/additive_domain.proto
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-03-15 17:54:00.000000 ansys-api-additive-1.6.8/ansys/api/additive/v0/additive_materials.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-03-15 17:54:00.000000 ansys-api-additive-1.6.8/ansys/api/additive/v0/additive_simulation.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:54:09.103071 ansys-api-additive-1.6.8/ansys_api_additive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-03-15 17:54:09.000000 ansys-api-additive-1.6.8/ansys_api_additive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-15 17:54:09.000000 ansys-api-additive-1.6.8/ansys_api_additive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 17:54:09.000000 ansys-api-additive-1.6.8/ansys_api_additive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-15 17:54:09.000000 ansys-api-additive-1.6.8/ansys_api_additive.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-15 17:54:09.000000 ansys-api-additive-1.6.8/ansys_api_additive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-15 17:54:09.000000 ansys-api-additive-1.6.8/ansys_api_additive.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:54:09.103071 ansys-api-additive-1.6.8/google/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:54:09.103071 ansys-api-additive-1.6.8/google/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-15 17:54:00.000000 ansys-api-additive-1.6.8/google/api/annotations.proto
--rw-r--r--   0 runner    (1001) docker     (127)    15144 2024-03-15 17:54:00.000000 ansys-api-additive-1.6.8/google/api/http.proto
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-15 17:54:00.000000 ansys-api-additive-1.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 17:54:09.107071 ansys-api-additive-1.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-03-15 17:54:00.000000 ansys-api-additive-1.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:53:40.222701 ansys_api_additive-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-16 20:53:32.000000 ansys_api_additive-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-04-16 20:53:40.222701 ansys_api_additive-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-16 20:53:32.000000 ansys_api_additive-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:53:40.218701 ansys_api_additive-1.7.0/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:53:40.218701 ansys_api_additive-1.7.0/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:53:40.218701 ansys_api_additive-1.7.0/ansys/api/additive/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 20:53:32.000000 ansys_api_additive-1.7.0/ansys/api/additive/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-16 20:53:32.000000 ansys_api_additive-1.7.0/ansys/api/additive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:53:32.000000 ansys_api_additive-1.7.0/ansys/api/additive/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:53:40.218701 ansys_api_additive-1.7.0/ansys/api/additive/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-16 20:53:32.000000 ansys_api_additive-1.7.0/ansys/api/additive/v0/about.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-04-16 20:53:32.000000 ansys_api_additive-1.7.0/ansys/api/additive/v0/additive_domain.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-16 20:53:32.000000 ansys_api_additive-1.7.0/ansys/api/additive/v0/additive_materials.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-16 20:53:32.000000 ansys_api_additive-1.7.0/ansys/api/additive/v0/additive_simulation.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:53:40.222701 ansys_api_additive-1.7.0/ansys_api_additive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-04-16 20:53:40.000000 ansys_api_additive-1.7.0/ansys_api_additive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-16 20:53:40.000000 ansys_api_additive-1.7.0/ansys_api_additive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:53:40.000000 ansys_api_additive-1.7.0/ansys_api_additive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-16 20:53:40.000000 ansys_api_additive-1.7.0/ansys_api_additive.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-16 20:53:40.000000 ansys_api_additive-1.7.0/ansys_api_additive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 20:53:40.000000 ansys_api_additive-1.7.0/ansys_api_additive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:53:40.218701 ansys_api_additive-1.7.0/google/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:53:40.222701 ansys_api_additive-1.7.0/google/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-16 20:53:32.000000 ansys_api_additive-1.7.0/google/api/annotations.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    15144 2024-04-16 20:53:32.000000 ansys_api_additive-1.7.0/google/api/http.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-16 20:53:32.000000 ansys_api_additive-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 20:53:40.222701 ansys_api_additive-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-16 20:53:32.000000 ansys_api_additive-1.7.0/setup.py
```

### Comparing `ansys-api-additive-1.6.8/LICENSE` & `ansys_api_additive-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-api-additive-1.6.8/PKG-INFO` & `ansys_api_additive-1.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-additive
-Version: 1.6.8
-Summary: Autogenerated python gRPC interface package for ansys-api-additive, built on 17:54:09 on 15 March 2024
+Version: 1.7.0
+Summary: Autogenerated python gRPC interface package for ansys-api-additive, built on 20:53:40 on 16 April 2024
 Home-page: https://github.com/ansys/ansys-api-additive
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 License: MIT
 Project-URL: Documentation, https://github.com/ansys/ansys-api-additive/#readme
```

### Comparing `ansys-api-additive-1.6.8/README.md` & `ansys_api_additive-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ansys-api-additive-1.6.8/ansys/api/additive/v0/additive_domain.proto` & `ansys_api_additive-1.7.0/ansys/api/additive/v0/additive_domain.proto`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     double reference_width = 5;
     double depth = 6;
     double reference_depth = 7;
 }
 
 message MeltPool {
     repeated MeltPoolTimeStep time_steps = 1;
+    repeated bytes thermal_history_vtk = 2;
 }
 
 message AdditiveMaterial {
     double hardening_factor = 1;
     double strain_scaling_factor = 2;
     double support_yield_strength_ratio = 3;
     double poisson_ratio = 4;
```

### Comparing `ansys-api-additive-1.6.8/ansys/api/additive/v0/additive_materials.proto` & `ansys_api_additive-1.7.0/ansys/api/additive/v0/additive_materials.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-additive-1.6.8/ansys/api/additive/v0/additive_simulation.proto` & `ansys_api_additive-1.7.0/ansys/api/additive/v0/additive_simulation.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-additive-1.6.8/ansys_api_additive.egg-info/PKG-INFO` & `ansys_api_additive-1.7.0/ansys_api_additive.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-additive
-Version: 1.6.8
-Summary: Autogenerated python gRPC interface package for ansys-api-additive, built on 17:54:09 on 15 March 2024
+Version: 1.7.0
+Summary: Autogenerated python gRPC interface package for ansys-api-additive, built on 20:53:40 on 16 April 2024
 Home-page: https://github.com/ansys/ansys-api-additive
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 License: MIT
 Project-URL: Documentation, https://github.com/ansys/ansys-api-additive/#readme
```

### Comparing `ansys-api-additive-1.6.8/ansys_api_additive.egg-info/SOURCES.txt` & `ansys_api_additive-1.7.0/ansys_api_additive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansys-api-additive-1.6.8/google/api/annotations.proto` & `ansys_api_additive-1.7.0/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-additive-1.6.8/google/api/http.proto` & `ansys_api_additive-1.7.0/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-additive-1.6.8/setup.py` & `ansys_api_additive-1.7.0/setup.py`

 * *Files identical despite different names*

