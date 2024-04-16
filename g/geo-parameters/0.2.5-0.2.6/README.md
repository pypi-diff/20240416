# Comparing `tmp/geo_parameters-0.2.5.tar.gz` & `tmp/geo_parameters-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_parameters-0.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "geo_parameters-0.2.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `geo_parameters-0.2.5.tar` & `geo_parameters-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1776 2024-04-12 09:20:09.678411 geo_parameters-0.2.5/.github/workflows/tests.yml
--rw-r--r--   0        0        0     3140 2024-04-12 09:20:09.678411 geo_parameters-0.2.5/.gitignore
--rw-r--r--   0        0        0     1079 2024-04-12 09:20:09.678411 geo_parameters-0.2.5/LICENSE
--rw-r--r--   0        0        0     3386 2024-04-12 09:20:09.678411 geo_parameters-0.2.5/README.md
--rw-r--r--   0        0        0       91 2024-04-12 09:20:09.678411 geo_parameters-0.2.5/environment.yml
--rw-r--r--   0        0        0       90 2024-04-12 09:20:09.678411 geo_parameters-0.2.5/geo_parameters/__init__.py
--rw-r--r--   0        0        0      847 2024-04-12 09:20:09.678411 geo_parameters-0.2.5/geo_parameters/grid.py
--rw-r--r--   0        0        0     1967 2024-04-12 09:20:09.678411 geo_parameters-0.2.5/geo_parameters/metaparameter.py
--rw-r--r--   0        0        0     1298 2024-04-12 09:20:09.678411 geo_parameters-0.2.5/geo_parameters/ocean.py
--rw-r--r--   0        0        0     1124 2024-04-12 09:20:09.678411 geo_parameters-0.2.5/geo_parameters/parameter_funcs.py
--rw-r--r--   0        0        0    18443 2024-04-12 09:20:09.678411 geo_parameters-0.2.5/geo_parameters/wave.py
--rw-r--r--   0        0        0     1719 2024-04-12 09:20:09.678411 geo_parameters-0.2.5/geo_parameters/wind.py
--rw-r--r--   0        0        0      450 2024-04-12 09:20:09.678411 geo_parameters-0.2.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-12 09:20:09.678411 geo_parameters-0.2.5/tests/__init__.py
--rw-r--r--   0        0        0     1810 2024-04-12 09:20:09.678411 geo_parameters-0.2.5/tests/test_doc.py
--rw-r--r--   0        0        0     1020 2024-04-12 09:20:09.678411 geo_parameters-0.2.5/tests/test_funcs.py
--rw-r--r--   0        0        0      808 2024-04-12 09:20:09.678411 geo_parameters-0.2.5/tests/test_names.py
--rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 geo_parameters-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1776 2024-04-15 17:19:39.734180 geo_parameters-0.2.6/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     3140 2024-04-15 17:19:39.738180 geo_parameters-0.2.6/.gitignore
+-rw-r--r--   0        0        0     1079 2024-04-15 17:19:39.738180 geo_parameters-0.2.6/LICENSE
+-rw-r--r--   0        0        0     3386 2024-04-15 17:19:39.738180 geo_parameters-0.2.6/README.md
+-rw-r--r--   0        0        0       91 2024-04-15 17:19:39.738180 geo_parameters-0.2.6/environment.yml
+-rw-r--r--   0        0        0      135 2024-04-15 17:19:39.738180 geo_parameters-0.2.6/geo_parameters/__init__.py
+-rw-r--r--   0        0        0      830 2024-04-15 17:19:39.738180 geo_parameters-0.2.6/geo_parameters/grid.py
+-rw-r--r--   0        0        0     1967 2024-04-15 17:19:39.738180 geo_parameters-0.2.6/geo_parameters/metaparameter.py
+-rw-r--r--   0        0        0     1280 2024-04-15 17:19:39.738180 geo_parameters-0.2.6/geo_parameters/ocean.py
+-rw-r--r--   0        0        0     1124 2024-04-15 17:19:39.738180 geo_parameters-0.2.6/geo_parameters/parameter_funcs.py
+-rw-r--r--   0        0        0       68 2024-04-15 17:19:39.738180 geo_parameters-0.2.6/geo_parameters/ureg.py
+-rw-r--r--   0        0        0    18426 2024-04-15 17:19:39.738180 geo_parameters-0.2.6/geo_parameters/wave.py
+-rw-r--r--   0        0        0     1702 2024-04-15 17:19:39.738180 geo_parameters-0.2.6/geo_parameters/wind.py
+-rw-r--r--   0        0        0      450 2024-04-15 17:19:39.738180 geo_parameters-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 17:19:39.738180 geo_parameters-0.2.6/tests/__init__.py
+-rw-r--r--   0        0        0     1810 2024-04-15 17:19:39.738180 geo_parameters-0.2.6/tests/test_doc.py
+-rw-r--r--   0        0        0     1020 2024-04-15 17:19:39.738180 geo_parameters-0.2.6/tests/test_funcs.py
+-rw-r--r--   0        0        0      808 2024-04-15 17:19:39.738180 geo_parameters-0.2.6/tests/test_names.py
+-rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 geo_parameters-0.2.6/PKG-INFO
```

### Comparing `geo_parameters-0.2.5/.github/workflows/tests.yml` & `geo_parameters-0.2.6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.5/.gitignore` & `geo_parameters-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.5/LICENSE` & `geo_parameters-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.5/README.md` & `geo_parameters-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.5/geo_parameters/grid.py` & `geo_parameters-0.2.6/geo_parameters/grid.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-from .metaparameter import MetaParameter
-import pint
-
-ureg = pint.UnitRegistry()
-
-ureg.default_format = "~C"
+from geo_parameters.metaparameter import MetaParameter
+from geo_parameters.ureg import ureg
 
 
 class Lon(MetaParameter):
     name = "lon"
     _long_name = "longitude"
     _standard_name = "longitude"
     _unit = "degrees_east"
```

### Comparing `geo_parameters-0.2.5/geo_parameters/metaparameter.py` & `geo_parameters-0.2.6/geo_parameters/metaparameter.py`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.5/geo_parameters/ocean.py` & `geo_parameters-0.2.6/geo_parameters/ocean.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,9 @@
-from .metaparameter import MetaParameter
-import pint
-
-ureg = pint.UnitRegistry()
-
-ureg.default_format = "~C"
-
+from geo_parameters.metaparameter import MetaParameter
+from geo_parameters.ureg import ureg
 
 class WaterDepth(MetaParameter):
     name = "depth"
     _long_name = "water_depth"
     _standard_name = "sea_floor_depth_below_sea_surface"
     _unit = ureg.m
```

### Comparing `geo_parameters-0.2.5/geo_parameters/parameter_funcs.py` & `geo_parameters-0.2.6/geo_parameters/parameter_funcs.py`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.5/geo_parameters/wave.py` & `geo_parameters-0.2.6/geo_parameters/wave.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-from .metaparameter import MetaParameter
-import pint
-
-ureg = pint.UnitRegistry()
-ureg.default_format = "~C"
-
+from geo_parameters.metaparameter import MetaParameter
+from geo_parameters.ureg import ureg
 
 ## Wave heights
 class Hs(MetaParameter):
     name = "hs"
     _long_name = "significant_wave_height"
     _standard_name = [
         "sea_surface_wave_significant_height",
```

### Comparing `geo_parameters-0.2.5/geo_parameters/wind.py` & `geo_parameters-0.2.6/geo_parameters/wind.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-from .metaparameter import MetaParameter
-import pint
-
-ureg = pint.UnitRegistry()
-ureg.default_format = "~C"
-
+from geo_parameters.metaparameter import MetaParameter
+from geo_parameters.ureg import ureg
 
 class XWind(MetaParameter):
     name = "x_wind"
     _long_name = "x_wind_component"
     _standard_name = [
         "x_wind",
         "grid_eastward_wind",
```

### Comparing `geo_parameters-0.2.5/tests/test_doc.py` & `geo_parameters-0.2.6/tests/test_doc.py`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.5/tests/test_funcs.py` & `geo_parameters-0.2.6/tests/test_funcs.py`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.5/tests/test_names.py` & `geo_parameters-0.2.6/tests/test_names.py`

 * *Files identical despite different names*

