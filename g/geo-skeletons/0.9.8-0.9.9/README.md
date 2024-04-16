# Comparing `tmp/geo_skeletons-0.9.8.tar.gz` & `tmp/geo_skeletons-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_skeletons-0.9.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "geo_skeletons-0.9.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `geo_skeletons-0.9.8.tar` & `geo_skeletons-0.9.9.tar`

### file list

```diff
@@ -1,49 +1,51 @@
--rw-r--r--   0        0        0     1775 2023-09-20 13:05:43.141758 geo_skeletons-0.9.8/.github/workflows/tests.yml
--rw-r--r--   0        0        0     3140 2023-09-20 13:05:43.141758 geo_skeletons-0.9.8/.gitignore
--rw-r--r--   0        0        0      819 2023-09-20 13:05:43.141758 geo_skeletons-0.9.8/.readthedocs.yml
--rw-r--r--   0        0        0    18092 2023-09-20 13:05:43.141758 geo_skeletons-0.9.8/LICENSE
--rw-r--r--   0        0        0     2616 2023-09-20 13:05:43.141758 geo_skeletons-0.9.8/README.md
--rw-r--r--   0        0        0      638 2023-09-20 13:05:43.141758 geo_skeletons-0.9.8/docs/Makefile
--rw-r--r--   0        0        0     1967 2023-09-20 13:05:43.145758 geo_skeletons-0.9.8/docs/conf.py
--rw-r--r--   0        0        0    18586 2023-09-20 13:05:43.145758 geo_skeletons-0.9.8/docs/index.rst
--rw-r--r--   0        0        0       72 2023-09-20 13:05:43.145758 geo_skeletons-0.9.8/docs/requirements.txt
--rw-r--r--   0        0        0   183077 2023-09-20 13:05:43.145758 geo_skeletons-0.9.8/docs/simple_plot.png
--rw-r--r--   0        0        0      128 2023-09-20 13:05:43.145758 geo_skeletons-0.9.8/environment.yml
--rw-r--r--   0        0        0       88 2023-09-20 13:05:43.145758 geo_skeletons-0.9.8/geo_skeletons/__init__.py
--rw-r--r--   0        0        0      158 2023-09-20 13:05:43.145758 geo_skeletons-0.9.8/geo_skeletons/decorators/__init__.py
--rw-r--r--   0        0        0     6050 2023-09-20 13:05:43.145758 geo_skeletons-0.9.8/geo_skeletons/decorators/coordinate_factory.py
--rw-r--r--   0        0        0     2933 2023-09-20 13:05:43.145758 geo_skeletons-0.9.8/geo_skeletons/decorators/coordinate_manager.py
--rw-r--r--   0        0        0    13574 2023-09-20 13:05:43.145758 geo_skeletons-0.9.8/geo_skeletons/decorators/dataset_manager.py
--rw-r--r--   0        0        0     1767 2023-09-20 13:05:43.145758 geo_skeletons-0.9.8/geo_skeletons/decorators/datavar_factory.py
--rw-r--r--   0        0        0     3242 2023-09-20 13:05:43.145758 geo_skeletons-0.9.8/geo_skeletons/decorators/mask_factory.py
--rw-r--r--   0        0        0     1662 2023-09-20 13:05:43.145758 geo_skeletons-0.9.8/geo_skeletons/distance_functions.py
--rw-r--r--   0        0        0     7665 2023-09-20 13:05:43.145758 geo_skeletons-0.9.8/geo_skeletons/gridded_skeleton.py
--rw-r--r--   0        0        0     3762 2023-09-20 13:05:43.145758 geo_skeletons-0.9.8/geo_skeletons/point_skeleton.py
--rw-r--r--   0        0        0    32775 2023-09-20 13:05:43.145758 geo_skeletons-0.9.8/geo_skeletons/skeleton.py
--rw-r--r--   0        0        0      498 2023-09-20 13:05:43.145758 geo_skeletons-0.9.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-09-20 13:05:43.145758 geo_skeletons-0.9.8/tests/__init__.py
--rw-r--r--   0        0        0     2711 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_absorb_skeleton.py
--rw-r--r--   0        0        0     5308 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_add_coords_gridded.py
--rw-r--r--   0        0        0     5582 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_add_coords_point.py
--rw-r--r--   0        0        0     1320 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_add_datavar_gridded.py
--rw-r--r--   0        0        0     1002 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_add_datavar_point.py
--rw-r--r--   0        0        0     3611 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_add_mask_gridded.py
--rw-r--r--   0        0        0     3640 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_add_mask_point.py
--rw-r--r--   0        0        0      465 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_ds_manager.py
--rw-r--r--   0        0        0     2892 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_gridded_init_cartesian.py
--rw-r--r--   0        0        0     2798 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_gridded_init_spherical.py
--rw-r--r--   0        0        0     3492 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_gridded_init_strict_and_native.py
--rw-r--r--   0        0        0     3359 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_gridded_utm_conversions.py
--rw-r--r--   0        0        0     3792 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_point_init_cartesian.py
--rw-r--r--   0        0        0     3552 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_point_init_spherical.py
--rw-r--r--   0        0        0     3467 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_point_init_strict_and_native.py
--rw-r--r--   0        0        0     1980 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_point_utm_conversions.py
--rw-r--r--   0        0        0     5223 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_set_spacing.py
--rw-r--r--   0        0        0     1471 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_slicing_data.py
--rw-r--r--   0        0        0     3579 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_will_grid_be_spherical_or_cartesian_cartesian_input.py
--rw-r--r--   0        0        0     3633 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_will_grid_be_spherical_or_cartesian_spherical_input.py
--rw-r--r--   0        0        0     2195 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_yank_point_cartesian_gridded.py
--rw-r--r--   0        0        0     2182 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_yank_point_cartesian_point.py
--rw-r--r--   0        0        0     2610 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_yank_point_spherical_gridded.py
--rw-r--r--   0        0        0     2426 2023-09-20 13:05:43.149758 geo_skeletons-0.9.8/tests/test_yank_point_spherical_point.py
--rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 geo_skeletons-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1775 2023-11-23 15:06:20.259125 geo_skeletons-0.9.9/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     3140 2023-11-23 15:06:20.259125 geo_skeletons-0.9.9/.gitignore
+-rw-r--r--   0        0        0      819 2023-11-23 15:06:20.259125 geo_skeletons-0.9.9/.readthedocs.yml
+-rw-r--r--   0        0        0    18092 2023-11-23 15:06:20.259125 geo_skeletons-0.9.9/LICENSE
+-rw-r--r--   0        0        0     2616 2023-11-23 15:06:20.259125 geo_skeletons-0.9.9/README.md
+-rw-r--r--   0        0        0      638 2023-11-23 15:06:20.259125 geo_skeletons-0.9.9/docs/Makefile
+-rw-r--r--   0        0        0     1967 2023-11-23 15:06:20.259125 geo_skeletons-0.9.9/docs/conf.py
+-rw-r--r--   0        0        0    18586 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/docs/index.rst
+-rw-r--r--   0        0        0       72 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/docs/requirements.txt
+-rw-r--r--   0        0        0   183077 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/docs/simple_plot.png
+-rw-r--r--   0        0        0      128 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/environment.yml
+-rw-r--r--   0        0        0       88 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/geo_skeletons/__init__.py
+-rw-r--r--   0        0        0      158 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/geo_skeletons/decorators/__init__.py
+-rw-r--r--   0        0        0     6050 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/geo_skeletons/decorators/coordinate_factory.py
+-rw-r--r--   0        0        0     3129 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/geo_skeletons/decorators/coordinate_manager.py
+-rw-r--r--   0        0        0    12797 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/geo_skeletons/decorators/dataset_manager.py
+-rw-r--r--   0        0        0     1980 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/geo_skeletons/decorators/datavar_factory.py
+-rw-r--r--   0        0        0     3051 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/geo_skeletons/decorators/mask_factory.py
+-rw-r--r--   0        0        0     1662 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/geo_skeletons/distance_functions.py
+-rw-r--r--   0        0        0      739 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/geo_skeletons/errors.py
+-rw-r--r--   0        0        0     7983 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/geo_skeletons/gridded_skeleton.py
+-rw-r--r--   0        0        0     3519 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/geo_skeletons/point_skeleton.py
+-rw-r--r--   0        0        0    41828 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/geo_skeletons/skeleton.py
+-rw-r--r--   0        0        0      498 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/tests/__init__.py
+-rw-r--r--   0        0        0     4230 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/tests/test_absorb_skeleton.py
+-rw-r--r--   0        0        0     5308 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/tests/test_add_coords_gridded.py
+-rw-r--r--   0        0        0     5582 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/tests/test_add_coords_point.py
+-rw-r--r--   0        0        0     1320 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/tests/test_add_datavar_gridded.py
+-rw-r--r--   0        0        0     1002 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/tests/test_add_datavar_point.py
+-rw-r--r--   0        0        0     3611 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/tests/test_add_mask_gridded.py
+-rw-r--r--   0        0        0     3640 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/tests/test_add_mask_point.py
+-rw-r--r--   0        0        0      465 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/tests/test_ds_manager.py
+-rw-r--r--   0        0        0     3004 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/tests/test_from_ds.py
+-rw-r--r--   0        0        0     2892 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/tests/test_gridded_init_cartesian.py
+-rw-r--r--   0        0        0     2798 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/tests/test_gridded_init_spherical.py
+-rw-r--r--   0        0        0     3492 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/tests/test_gridded_init_strict_and_native.py
+-rw-r--r--   0        0        0     3359 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/tests/test_gridded_utm_conversions.py
+-rw-r--r--   0        0        0     3792 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/tests/test_point_init_cartesian.py
+-rw-r--r--   0        0        0     3552 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/tests/test_point_init_spherical.py
+-rw-r--r--   0        0        0     3467 2023-11-23 15:06:20.263125 geo_skeletons-0.9.9/tests/test_point_init_strict_and_native.py
+-rw-r--r--   0        0        0     1980 2023-11-23 15:06:20.267126 geo_skeletons-0.9.9/tests/test_point_utm_conversions.py
+-rw-r--r--   0        0        0     5223 2023-11-23 15:06:20.267126 geo_skeletons-0.9.9/tests/test_set_spacing.py
+-rw-r--r--   0        0        0     1471 2023-11-23 15:06:20.267126 geo_skeletons-0.9.9/tests/test_slicing_data.py
+-rw-r--r--   0        0        0     3278 2023-11-23 15:06:20.267126 geo_skeletons-0.9.9/tests/test_will_grid_be_spherical_or_cartesian_cartesian_input.py
+-rw-r--r--   0        0        0     3333 2023-11-23 15:06:20.267126 geo_skeletons-0.9.9/tests/test_will_grid_be_spherical_or_cartesian_spherical_input.py
+-rw-r--r--   0        0        0     2195 2023-11-23 15:06:20.267126 geo_skeletons-0.9.9/tests/test_yank_point_cartesian_gridded.py
+-rw-r--r--   0        0        0     2182 2023-11-23 15:06:20.267126 geo_skeletons-0.9.9/tests/test_yank_point_cartesian_point.py
+-rw-r--r--   0        0        0     2610 2023-11-23 15:06:20.267126 geo_skeletons-0.9.9/tests/test_yank_point_spherical_gridded.py
+-rw-r--r--   0        0        0     2426 2023-11-23 15:06:20.267126 geo_skeletons-0.9.9/tests/test_yank_point_spherical_point.py
+-rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 geo_skeletons-0.9.9/PKG-INFO
```

### Comparing `geo_skeletons-0.9.8/.github/workflows/tests.yml` & `geo_skeletons-0.9.9/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/.gitignore` & `geo_skeletons-0.9.9/.gitignore`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/.readthedocs.yml` & `geo_skeletons-0.9.9/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/LICENSE` & `geo_skeletons-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/README.md` & `geo_skeletons-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/docs/Makefile` & `geo_skeletons-0.9.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/docs/conf.py` & `geo_skeletons-0.9.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/docs/index.rst` & `geo_skeletons-0.9.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/docs/simple_plot.png` & `geo_skeletons-0.9.9/docs/simple_plot.png`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/geo_skeletons/decorators/coordinate_factory.py` & `geo_skeletons-0.9.9/geo_skeletons/decorators/coordinate_factory.py`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/geo_skeletons/decorators/coordinate_manager.py` & `geo_skeletons-0.9.9/geo_skeletons/decorators/coordinate_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,21 +11,25 @@
         self.vars = {}
         self.vars["added"] = {}
         self.vars["initial"] = {}
 
         self.masks = {}
         self.masks["added"] = {}
 
-    def add_var(self, name: str, coords: str) -> None:
+        self.default_values = {}
+
+    def add_var(self, name: str, coords: str, default_value: float) -> None:
         """Add a variable that the Skeleton will use."""
         self.vars["added"][name] = coords
+        self.default_values[name] = default_value
 
-    def add_mask(self, name: str, coords: str) -> None:
+    def add_mask(self, name: str, coords: str, default_value: int) -> None:
         """Add a mask that the Skeleton will use."""
-        self.masks["added"][name] = coords
+        self.masks["added"][f"{name}_mask"] = coords
+        self.default_values[f"{name}_mask"] = default_value
 
     def add_coord(self, name: str, grid_coord: bool) -> None:
         """Add a coordinate that the Skeleton will use.
 
         grid_coord = True means that the coordinate describes the outer
         dimensions (e.g. x, y)
```

### Comparing `geo_skeletons-0.9.8/geo_skeletons/decorators/dataset_manager.py` & `geo_skeletons-0.9.9/geo_skeletons/decorators/dataset_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import numpy as np
 import xarray as xr
 from .coordinate_manager import CoordinateManager
 
+from ..errors import DataWrongDimensionError, UnknownCoordinateError, CoordinateWrongLengthError, GridError
+
 
 def move_time_dim_to_front(coord_list) -> list[str]:
     if "time" not in coord_list:
         return coord_list
     coord_list.insert(0, coord_list.pop(coord_list.index("time")))
     return coord_list
 
@@ -39,81 +41,56 @@
             xy_set = "x" in ds_coords and "y" in ds_coords
             lonlat_set = "lon" in ds_coords and "lat" in ds_coords
             inds_set = "inds" in ds_coords
             if inds_set:
                 ind_len = len(coord_dict["inds"])
                 for key, value in var_dict.items():
                     if len(value[1]) != ind_len:
-                        raise ValueError(
-                            f"Variable {key} is {len(value[1])} long but the index variable is {ind_len} long!"
-                        )
+                        raise CoordinateWrongLengthError(variable=key, len_of_variable=len(value[1]), index_variable='inds', len_of_index_variable=ind_len)
             if not (xy_set or lonlat_set or inds_set):
-                raise ValueError(
-                    "A proper spatial grid is not set: Requires 'x' and 'y', 'lon' and 'lat' or 'inds'!"
-                )
+                raise GridError
             if sum([xy_set, lonlat_set, inds_set]) > 1:
-                raise ValueError(
-                    "A well defined spatial grid is not set: Requires 'x' and 'y', 'lon' and 'lat' or 'inds'!"
-                )
+                raise GridError
 
             # Check that all added coordinates are provided
             for coord in self.coord_manager.added_coords("all"):
                 if coord not in ds_coords:
                     if self.get(coord) is not None:
                         # Add in old coordinate if it is not provided now (can happen when using set_spacing)
                         coord_dict[coord] = self.ds().get(coord).values
                     else:
-                        raise ValueError(
-                            f"Coordinate '{coord}' has been added (by a decorator?) but it was not provided when the Dataset ({ds_coords}) was created!"
-                        )
+                        raise UnknownCoordinateError(f"Skeleton has coordinate '{coord}', but it was not provided on initialization: {ds_coords}!")
 
             # Check that all provided coordinates have been added
             for coord in set(ds_coords) - set(SPATIAL_COORDS):
                 if coord not in self.coord_manager.added_coords("all"):
-                    raise Warning(
-                        f"Coordinate '{coord}' has been provided, but has not been added ({self.coord_manager.added_coords('all')})! Missing a decorator?"
-                    )
+                    raise UnknownCoordinateError(f"Coordinate {coord} provided on initialization, but Skeleton doesn't have it: {self.coord_manager.added_coords('all')}! Missing a decorator?")
 
         def determine_coords() -> dict:
             """Creates dictonary of the coordinates"""
 
             coord_dict = {}
             if "y" in self.coord_manager.initial_coords():
                 coord_dict[y_str] = y
             if "x" in self.coord_manager.initial_coords():
                 coord_dict[x_str] = x
             if "inds" in self.coord_manager.initial_coords():
                 coord_dict["inds"] = np.arange(len(x))
 
             # Add in other possible coordinates that are set at initialization
-            for key in self.coord_manager.added_coords("grid"):
+            for key in self.coord_manager.added_coords():
                 value = kwargs.get(key)
 
                 if value is None:
                     value = self.get(key)
 
                 if value is None:
-                    raise KeyError(
-                        f"The variable {key} was not provided in the keyword list when the object was initialized!"
-                    )
-                value = np.array(value)
-                coord_dict[key] = value
-
-            for key in self.coord_manager.added_coords("gridpoint"):
-                value = kwargs.get(key)
-
-                if value is None:
-                    value = self.get(key)
-
-                if value is None:
-                    raise KeyError(
-                        f"The variable {key} was not provided in the keyword list when the object was initialized!"
-                    )
-                value = np.array(value)
-                coord_dict[key] = value
+                    raise UnknownCoordinateError(f"Skeleton has coordinate '{key}', but it was not provided on initialization {kwargs.keys()} nor is it already set {self.coords()}!")
+                
+                coord_dict[key] = np.array(value)
 
             coord_dict = {
                 c: coord_dict[c] for c in move_time_dim_to_front(list(coord_dict))
             }
 
             return coord_dict
 
@@ -141,15 +118,14 @@
             x, y, is_cartesian=(x_str == "x"), indexed=indexed
         )
 
         coord_dict = determine_coords()
         var_dict = determine_vars()
 
         check_consistency()
-
         self.set_new_ds(xr.Dataset(coords=coord_dict, data_vars=var_dict))
 
     def set_new_ds(self, ds: xr.Dataset) -> None:
         self.data = ds
 
     def ds(self):
         """Resturns the Dataset (None if doesn't exist)."""
@@ -158,29 +134,42 @@
         return self.data
 
     def set(self, data: np.ndarray, data_name: str, coord_type: str = "all") -> None:
         """Adds in new data to the Dataset.
 
         coord_type = 'all', 'spatial', 'grid' or 'gridpoint'
         """
+
         self._merge_in_ds(self.compile_to_ds(data, data_name, coord_type))
 
-    def get(self, data_name: str, default_data=None, **kwargs) -> xr.DataArray:
+    def get(self, name: str, default_data=None, empty: bool=False, **kwargs) -> xr.DataArray:
         """Gets data from Dataset.
 
         **kwargs can be used for slicing data.
 
         """
         ds = self.ds()
         if ds is None:
             return None
 
-        data = ds.get(data_name, default_data)
-        if isinstance(data, xr.DataArray):
-            data = self._slice_data(data, **kwargs)
+        if empty:
+            coords = self.coord_manager.added_vars().get(name)
+            if coords is None:
+                coords = self.coord_manager.added_masks().get(name)
+                
+            empty_data = np.full(self.coords_to_size(self.coords(coords)), self.coord_manager.default_values.get(name))
+            default_data = xr.DataArray(data=empty_data,coords=self.coords_dict(coords))
+
+        data = ds.get(name, default_data)
+        if not isinstance(data, xr.DataArray):
+            return data
+        
+        data = self._slice_data(data, **kwargs)
+        if empty:
+            data.values = np.full(data.shape, self.coord_manager.default_values.get(name))
 
         return data
 
     def set_attrs(self, attributes: dict, data_array_name: str = None) -> None:
         """Sets attributes to DataArray da_name.
 
         If data_array_name is not given, sets global attributes
@@ -196,15 +185,16 @@
         for key, value in kwargs.items():
             if key in list(data.coords):
                 coordinates[key] = value
             else:
                 keywords[key] = value
 
         for key, value in coordinates.items():
-            data = eval(f"data.sel({key}={value}, **keywords)")
+            #data = eval(f"data.sel({key}={value}, **keywords)")
+            data = data.sel({key: value}, **keywords)
 
         return data
 
     def _merge_in_ds(self, ds_list: list[xr.Dataset]) -> None:
         """Merge in Datasets with some data into the existing Dataset of the
         Skeleton.
         """
@@ -222,47 +212,31 @@
         coord_type determines over which coordinates to set the mask:
 
         'all': all coordinates in the Dataset
         'spatial': Dataset coordinates from the Skeleton (x, y, lon, lat, inds)
         'grid': coordinates for the grid (e.g. z, time)
         'gridpoint': coordinates for a grid point (e.g. frequency, direcion or time)
         """
-
-        def check_coord_consistency():
-            for i, item in enumerate(coords_dict.items()):
-                if i > len(data.shape) - 1:
-                    raise Exception(
-                        f"{item[0]} coordinate is {len(item[1])} long, but that dimension doesnt exist in the data!!!"
-                    )
-                if len(item[1]) != data.shape[i]:
-                    raise Exception(
-                        f"{item[0]} coordinate is {len(item[1])} long, but size of data in that dimension (dim {i}) is {data.shape[i]}!!!"
-                    )
-
-            if i < len(data.shape) - 1:
-                raise Exception(
-                    f"The data had {len(data.shape)} dimensions but only {i} dimensions have been defined. Missing a decorator?"
-                )
-
         coords_dict = self.coords_dict(coord_type)
-        check_coord_consistency()
 
-        # Data variables
-        vars_dict = {}
-        vars_dict[data_name] = (coords_dict.keys(), data)
+        coord_shape = tuple(len(x) for x in coords_dict.values())
+        if coord_shape != data.shape:
+            raise DataWrongDimensionError(data_shape = data.shape, coord_shape=coord_shape)
+
+        vars_dict = {data_name: (coords_dict.keys(), data)}
 
         ds = xr.Dataset(data_vars=vars_dict, coords=coords_dict)
         return ds
 
     def vars(self) -> list[str]:
         """Returns a list of the variables in the Dataset."""
-        if hasattr(self, "data"):
-            return list(self.data.keys())
-        return []
-
+        if self.ds() is None:
+            return []
+        return list(self.data.keys())
+        
     def vars_dict(self) -> list[str]:
         """Returns a dict of the variables in the Dataset."""
         return self.keys_to_dict(self.vars())
 
     def coords(self, coords: str = "all") -> list[str]:
         """Returns a list of the coordinates from the Dataset.
 
@@ -278,18 +252,18 @@
             for val in list1:
                 if val in list2:
                     list3.append(val)
             return list3
 
         if coords not in ["all", "spatial", "grid", "gridpoint"]:
             raise ValueError(
-                "Type needs to be 'all', 'spatial', 'grid' or 'gridpoint'."
+                f"Keyword 'coords' needs to be 'all' (default), 'spatial', 'grid' or 'gridpoint', not {coords}."
             )
 
-        if not hasattr(self, "data"):
+        if self.ds() is None:
             return []
 
         all_coords = list(self.ds().coords)
 
         if coords == "all":
             return move_time_dim_to_front(all_coords)
         if coords == "spatial":
```

### Comparing `geo_skeletons-0.9.8/geo_skeletons/decorators/datavar_factory.py` & `geo_skeletons-0.9.9/geo_skeletons/decorators/datavar_factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,41 +13,42 @@
     """stash_get = True means that the coordinate data can be accessed
     by method ._{name}() instead of .{name}()
 
     This allows for alternative definitions of the get-method elsewere."""
 
     def datavar_decorator(c):
         def get_var(
-            self, empty: bool = False, data_array: bool = False, **kwargs
+            self, empty: bool = False, data_array: bool = False, squeeze: bool=False, **kwargs
         ) -> np.ndarray:
             """Returns the data variable.
 
             Set empty=True to get an empty data variable (even if it doesn't exist).
 
             **kwargs can be used for slicing data.
             """
             if not self._structure_initialized():
                 return None
-            if empty:
-                return np.full(self.size(coords, **kwargs), default_value)
+            return self.get(name, empty=empty, data_array=data_array, squeeze=squeeze, **kwargs)
+            # if empty:
+            #     return np.full(self.size(coords, **kwargs), default_value)
+
+            # data = self._ds_manager.get(name, **kwargs)
+            # if data_array:
+            #     return data.copy()
+            # return data.values.copy()
 
-            data = self._ds_manager.get(name, **kwargs)
-            if data_array:
-                return data.copy()
-            return data.values.copy()
-
-        def set_var(self, data: Union[np.ndarray, int, float] = None) -> None:
+        def set_var(self, data: Union[np.ndarray, int, float] = None, allow_reshape: bool=False, coords: list[str]=None) -> None:
             if isinstance(data, int) or isinstance(data, float):
                 data = np.full(self._ds_manager.get(name).shape, data)
-            self._update_datavar(name, data)
+            self.set(name, data, allow_reshape=allow_reshape)
 
         if not hasattr(c, "_coord_manager"):
             c._coord_manager = CoordinateManager()
 
-        c._coord_manager.add_var(name, coords)
+        c._coord_manager.add_var(name, coords, default_value)
 
         if append:
             exec(f"c.{name} = partial(get_var, c)")
             exec(f"c.set_{name} = partial(set_var, c)")
         else:
             exec(f"c.{name} = get_var")
             exec(f"c.set_{name} = set_var")
```

### Comparing `geo_skeletons-0.9.8/geo_skeletons/decorators/mask_factory.py` & `geo_skeletons-0.9.9/geo_skeletons/decorators/mask_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,37 +4,32 @@
 CARTESIAN_STRINGS = ["x", "y", "xy"]
 SPHERICAL_STRINGS = ["lon", "lat", "lonlat"]
 
 
 def add_mask(
     name: str,
     default_value: int,
-    coords: str = "all",
+    coords: str = "grid",
     opposite_name: str = None,
 ):
     """coord_type = 'all', 'spatial', 'grid' or 'gridpoint'"""
 
     def mask_decorator(c):
         def get_mask(self, empty: bool = False, **kwargs) -> np.ndarray:
             """Returns bool array of the mask.
 
             Set boolean=False to get 0 for land and 1 for sea.
             Set empty=True to get an empty mask (even if it doesn't exist)
 
             **kwargs can be used for slicing data.
             """
 
-            if empty:
-                return np.full(self.size(coords, **kwargs), default_value).astype(bool)
-            mask = self._ds_manager.get(f"{name}_mask", **kwargs).values.copy()
+            mask = self.get(f"{name}_mask", boolean_mask=True, **kwargs)
 
-            if mask is None:
-                return None
-
-            return mask.astype(bool)
+            return mask
 
         def get_not_mask(self, **kwargs):
             mask = get_mask(self, **kwargs)
             if mask is None:
                 return None
             return np.logical_not(mask)
 
@@ -42,15 +37,15 @@
             self,
             type: str = "lonlat",
             native: bool = True,
             order_by: str = "lat",
             strict=False,
             **kwargs,
         ):
-            mask = self.get(f"{name}_mask", **kwargs).copy()
+            mask = get_mask(self, **kwargs)
 
             if type in CARTESIAN_STRINGS:
                 return self.xy(
                     mask=mask, native=native, order_by=order_by, strict=strict, **kwargs
                 )
             elif type in SPHERICAL_STRINGS:
                 return self.lonlat(
@@ -61,34 +56,34 @@
             self,
             type: str = "lonlat",
             native: bool = True,
             order_by: str = "lat",
             strict=False,
             **kwargs,
         ):
-            mask = np.logical_not(self.get(f"{name}_mask", **kwargs).copy())
+            mask = np.logical_not(get_mask(self, **kwargs))
 
             if type in CARTESIAN_STRINGS:
                 return self.xy(
                     mask=mask, native=native, order_by=order_by, strict=strict, **kwargs
                 )
             elif type in SPHERICAL_STRINGS:
                 return self.lonlat(
                     mask=mask, native=native, order_by=order_by, strict=strict, **kwargs
                 )
 
         def set_mask(self, data: np.ndarray = None) -> None:
-            self._update_mask(name, data)
+            self.set(f"{name}_mask", data.astype(bool))
 
         def set_opposite_mask(self, data: np.ndarray = None) -> None:
-            self._update_mask(name, np.logical_not(data))
+            self.set(f"{name}_mask", np.logical_not(data))
 
         if not hasattr(c, "_coord_manager"):
             c._coord_manager = CoordinateManager()
-        c._coord_manager.add_mask(name, coords)
+        c._coord_manager.add_mask(name, coords, default_value)
         exec(f"c.{name}_mask = get_mask")
         exec(f"c.{name}_points = get_masked_points")
         exec(f"c.set_{name}_mask = set_mask")
         if opposite_name is not None:
             exec(f"c.{opposite_name}_mask = get_not_mask")
             exec(f"c.{opposite_name}_points = get_not_points")
             exec(f"c.set_{opposite_name}_mask = set_opposite_mask")
```

### Comparing `geo_skeletons-0.9.8/geo_skeletons/distance_functions.py` & `geo_skeletons-0.9.9/geo_skeletons/distance_functions.py`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/geo_skeletons/gridded_skeleton.py` & `geo_skeletons-0.9.9/geo_skeletons/gridded_skeleton.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,43 @@
 import numpy as np
 from .skeleton import Skeleton
 from .point_skeleton import PointSkeleton
 from .distance_functions import lon_in_km, lat_in_km
-
+import xarray as xr
 
 class GriddedSkeleton(Skeleton):
     """Gives a gridded structure to the Skeleton.
 
     In practise this means that:
 
     1) Grid coordinates are defined as x,y / lon,lat.
     2) Methods x(), y() / lon(), lat() will return the vectors defining the grid.
     3) Methods xy() / lonlat() will return a list of all points of the grid
     (i.e. raveled meshgrid).
     """
 
+    @classmethod
+    def from_skeleton(
+        cls,
+        skeleton: Skeleton,
+        mask: np.ndarray = None,
+    ):
+        if not skeleton.is_gridded():
+            raise Exception("Can't create a GriddedSkeleton from a non-gridded data structure!")
+        
+        if mask is None:
+            mask = np.full(skeleton.size('spatial'), True)
+        lon, lat = skeleton.lon(strict=True, mask=mask), skeleton.lat(strict=True, mask=mask)
+        x, y = skeleton.x(strict=True, mask=mask), skeleton.y(strict=True, mask=mask)
+
+        new_skeleton = cls(lon=lon, lat=lat, x=x, y=y, name=skeleton.name)
+        new_skeleton.set_utm(skeleton.utm(), silent=True)
+
+        return new_skeleton
+
     def is_gridded(self) -> bool:
         return True
 
     def _initial_coords(self) -> list[str]:
         """Initial coordinates used with GriddedSkeletons. Additional coordinates
         can be added by decorators (e.g. @add_time).
         """
@@ -66,14 +85,15 @@
     def xy(
         self,
         mask: np.ndarray = None,
         order_by: str = "y",
         native: bool = False,
         strict: bool = False,
         normalize: bool = False,
+        utm: tuple[int, str] = None,
         **kwargs,
     ) -> tuple[np.ndarray, np.ndarray]:
         """Returns a tuple of x and y of all points.
         If strict=True, then None is returned if grid is sperical.
 
         mask is a boolean array (default True for all points)
         order_by = 'y' (default) or 'x'
@@ -82,30 +102,30 @@
         if not self.is_cartesian() and (strict or self.strict) and (not native):
             return None, None
 
         if mask is None:
             mask = np.full(super().size("spatial", **kwargs), True)
         mask = mask.ravel()
 
-        x, y = self._native_xy(**kwargs)
+        x, y = self._native_xy(utm=utm, **kwargs)
 
         if self.is_cartesian() or native:
             return x[mask], y[mask]
 
         # Only convert if skeleton is not Cartesian and native output is not requested
         points = PointSkeleton(lon=x, lat=y)
         points.set_utm(self.utm(), silent=True)
 
         return points.xy(mask=mask)
 
-    def _native_xy(self, **kwargs) -> tuple[np.ndarray, np.ndarray]:
+    def _native_xy(self, utm: tuple[int, str]=None, **kwargs) -> tuple[np.ndarray, np.ndarray]:
         """Returns a tuple of native x and y of all points."""
 
         x, y = np.meshgrid(
-            super().x(native=True, **kwargs), super().y(native=True, **kwargs)
+            super().x(native=True, utm=utm, **kwargs), super().y(native=True, utm=utm, **kwargs)
         )
 
         return x.ravel(), y.ravel()
 
     def set_spacing(
         self,
         dlon: float = 0.0,
@@ -136,65 +156,65 @@
 
         Set floating_edge=True to force exact dlon, dlat
         and instead possibly move lon_max, lat_max slightly
         to make it work (only compatibel with native coordinates).
 
         """
 
-        def determine_nx_ny(nx, ny, dx, dy, dm, dlon, dlat, dnmi):
-            x_end = self.edges("x", native=True)[1]
-            y_end = self.edges("y", native=True)[1]
+        def determine_nx(x_type: str, nx, dx, dm, dlon, dnmi):
+            if x_type == 'x':
+                lon_type = 'lon'
+            else:
+                lon_type = 'lat'
 
-            if nx and ny:
-                return int(nx), int(ny), x_end, y_end
+            x_end = self.edges(x_type, native=True)[1]
+
+            if nx:
+                return int(nx), x_end
 
             if dnmi:
                 if self.is_cartesian():
                     dm = dnmi * 1850
                 else:
                     dlat = dnmi / 60
                     x_km = lon_in_km(np.median(self.lat()))
                     y_km = lat_in_km(np.median(self.lat()))
-                    dlon = dlat * (y_km / x_km)
+                    if x_type == 'x':
+                        dlon = dlat * (y_km / x_km)
+                    else:
+                        dlon = dlat
 
-            if dlon and dlat:
-                nx = np.round((self.edges("lon")[1] - self.edges("lon")[0]) / dlon) + 1
-                ny = np.round((self.edges("lat")[1] - self.edges("lat")[0]) / dlat) + 1
+            if dlon:
+                nx = np.round((self.edges(lon_type)[1] - self.edges(lon_type)[0]) / dlon) + 1
                 if floating_edge:
                     if self.is_cartesian():
                         raise Exception(
                             "Grid is cartesian, so cant set exact dlon/dlat using floating_edge!"
                         )
-                    x_end = self.edges("lon")[0] + (nx - 1) * dlon
-                    y_end = self.edges("lat")[0] + (ny - 1) * dlat
-                return int(nx), int(ny), x_end, y_end
+                    x_end = self.edges(lon_type)[0] + (nx - 1) * dlon
+                return int(nx), x_end
 
             if dm:
                 dx = dm
-                dy = dm
 
-            if dx and dy:
-                nx = np.round((self.edges("x")[1] - self.edges("x")[0]) / dx) + 1
-                ny = np.round((self.edges("y")[1] - self.edges("y")[0]) / dy) + 1
+            if dx:
+                nx = np.round((self.edges(x_type)[1] - self.edges(x_type)[0]) / dx) + 1
                 if floating_edge:
                     if not self.is_cartesian():
                         raise Exception(
                             "Grid is spherical, so cant set exact dx/dy using floating_edge!"
                         )
-                    x_end = self.edges("x")[0] + (nx - 1) * dx
-                    y_end = self.edges("y")[0] + (ny - 1) * dy
-                return int(nx), int(ny), x_end, y_end
-
-            raise ValueError(
-                "Give a combination of nx/xy, dlon/dlat, dx/dy or dm or dmi"
-            )
+                    x_end = self.edges(x_type)[0] + (nx - 1) * dx
+                return int(nx), x_end
 
-        nx, ny, native_x_end, native_y_end = determine_nx_ny(
-            nx, ny, dx, dy, dm, dlon, dlat, dnmi
-        )
+            # Nothing given
+            return len(self.x()), x_end
+
+        nx, native_x_end = determine_nx('x', nx, dx, dm, dlon, dnmi)
+        ny, native_y_end = determine_nx('y', ny, dy, dm, dlat, dnmi)
 
         # Unique to not get [0,0,0] etc. arrays if nx=1
         x_native = np.unique(np.linspace(self.x(native=True)[0], native_x_end, nx))
         y_native = np.unique(np.linspace(self.y(native=True)[0], native_y_end, ny))
 
         if self.is_cartesian():
             x = x_native
@@ -205,19 +225,12 @@
             lon = x_native
             lat = y_native
             x = None
             y = None
         self._init_structure(x, y, lon, lat)
 
     def __repr__(self) -> str:
-        string = "grid = GriddedSkeleton"
-
-        x0, x1 = self.edges("x", native=True)
-        y0, y1 = self.edges("y", native=True)
-        string += f"({self.x_str}=({x0},{x1}), {self.y_str}=({y0},{y1}))\n"
-
-        string += f"grid.set_spacing(nx={self.nx()}, ny={self.ny()})\n"
-        if self.is_cartesian():
-            utm_number, utm_zone = self.utm()
-            string += f"grid.set_utm(({utm_number}, '{utm_zone}'))"
-
+        string = f"<{type(self).__name__} (GriddedSkeleton)>\n"
+        string += "-"*34 + " Containing " + "-"*34 + "\n"
+        string += self.ds().__repr__()
+        string += "\n" + "-"*80
         return string
```

### Comparing `geo_skeletons-0.9.8/geo_skeletons/point_skeleton.py` & `geo_skeletons-0.9.9/geo_skeletons/point_skeleton.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from .skeleton import Skeleton
-
+import xarray as xr
 
 class PointSkeleton(Skeleton):
     """Gives a unstructured structure to the Skeleton.
 
     In practise this means that:
 
     1) Grid coordinates are defined with and index (inds),
@@ -15,24 +15,26 @@
 
     @classmethod
     def from_skeleton(
         cls,
         skeleton: Skeleton,
         mask: np.ndarray = None,
     ):
+        
         if mask is None:
-            mask = np.full(skeleton.size(), True)
+            mask = np.full(skeleton.size('spatial'), True)
+
         lon, lat = skeleton.lonlat(strict=True, mask=mask)
         x, y = skeleton.xy(strict=True, mask=mask)
 
         new_skeleton = cls(lon=lon, lat=lat, x=x, y=y, name=skeleton.name)
         new_skeleton.set_utm(skeleton.utm(), silent=True)
 
         return new_skeleton
-
+    
     def is_gridded(self) -> bool:
         return False
 
     def _initial_coords(self) -> list[str]:
         """Initial coordinates used with PointSkeletons. Additional coordinates
         can be added by decorators (e.g. @add_time).
         """
@@ -69,57 +71,39 @@
         if lon is None:
             return None, None
         if mask is not None:
             return lon[mask], lat[mask]
         return lon, lat
 
     def xy(
-        self, mask: np.ndarray = None, strict=False, normalize: bool = False, **kwargs
+        self, mask: np.ndarray = None, strict=False, normalize: bool = False, utm: tuple[int, str]=None, **kwargs
     ) -> tuple[np.ndarray, np.ndarray]:
         """Returns a tuple of x- and y-coordinates of all points.
 
         If native=True, then lon-lat coordinatites are returned for spherical grids instead
         If strict=True, then (None, None) is returned if grid is spherical
 
         native=True overrides strict=True for spherical grids
 
         Identical to (.x(), .y()) (with no mask)
         mask is a boolean array (default True for all points)
         """
 
         # Transforms x-y to lon-lat if necessary
-        x, y = super().x(strict=strict, normalize=normalize, **kwargs), super().y(
-            strict=strict, normalize=normalize, **kwargs
+        x, y = super().x(strict=strict, normalize=normalize, utm=utm, **kwargs), super().y(
+            strict=strict, normalize=normalize, utm=utm, **kwargs
         )
 
         if x is None:
             return None, None
 
         if mask is not None:
             return x[mask], y[mask]
         return x, y
 
     def __repr__(self) -> str:
-        string = "points = PointSkeleton"
-
-        x, y = self.lonlat(native=True)
-
-        string += f"({self.x_str}=("
-
-        for xx in x:
-            string += f"{xx},"
-
-        string = string[:-1]
-        string += ")"
-
-        string += f", {self.y_str}=("
-
-        for yy in y:
-            string += f"{yy},"
-
-        string = string[:-1]
-        string += "))\n"
-        if self.is_cartesian():
-            utm_number, utm_zone = self.utm()
-            string += f"points.set_utm(({utm_number}, '{utm_zone}'))"
-
+        string = f"<{type(self).__name__} (PointSkeleton)>\n"
+        string += "-"*34 + " Containing " + "-"*34 + "\n"
+        string += self.ds().__repr__()
+        string += "\n" + "-"*80
         return string
+
```

### Comparing `geo_skeletons-0.9.8/geo_skeletons/skeleton.py` & `geo_skeletons-0.9.9/geo_skeletons/skeleton.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import numpy as np
 import xarray as xr
-import utm
+import utm as utm_module
 from copy import copy
 from .decorators.dataset_manager import DatasetManager
 from .decorators.coordinate_manager import CoordinateManager
 from typing import Iterable, Union
 from .distance_functions import min_distance, min_cartesian_distance
-
+from .errors import DataWrongDimensionError
+import itertools
+import pandas as pd
+from typing import Iterable
 DEFAULT_UTM = (33, "W")
 VALID_UTM_ZONES = [
     "C",
     "D",
     "E",
     "F",
     "G",
@@ -24,31 +27,135 @@
     "Q",
     "R",
     "S",
     "T",
     "U",
     "V",
     "W",
+    "X",
 ]
 
 VALID_UTM_NUMBERS = np.linspace(1, 60, 60).astype(int)
 
 
+class SkeletonIterator:
+    def __init__(self, dict_of_coords: dict, coords_to_iterate: list[str], skeleton) -> None:
+        self.coords_to_iterate = coords_to_iterate
+        self.dict_of_coords = dict_of_coords
+        self.skeleton = skeleton
+        self._compile_list()
+    
+    def __iter__(self):
+        return self
+    
+    def __next__(self):
+        self.ct += 1
+        if self.ct < len(self.list_of_skeletons):
+            return self.list_of_skeletons[self.ct]
+        raise StopIteration
+
+    def __call__(self, coords_to_iterate: list[str]):
+        self.coords_to_iterate = coords_to_iterate
+        self._compile_list()
+        return self
+
+    def _compile_list(self):
+        coord_dict = {}
+        for coord in self.coords_to_iterate:
+            
+            coord_value = self.dict_of_coords.get(coord)
+            
+            if coord_value is None:
+                print(f"Cannot iterate over coord {coord}, since it does not exist: {self.dict_of_coords.keys()}")
+            else:
+                coord_dict[coord] = coord_value
+        
+        coord_tuples = itertools.product(*[val.values for __, val in coord_dict.items()])
+        list_of_skeletons = []
+        for ctuple in coord_tuples:
+            arg_dict = {}
+            for n, val in enumerate(ctuple):
+                arg_dict[list(coord_dict.keys())[n]] = val
+            list_of_skeletons.append(self.skeleton.sel(arg_dict))
+
+        self.list_of_skeletons = list_of_skeletons
+        self.ct = -1
+
+
 class Skeleton:
     """Contains methods and data of the spatial x,y / lon, lat coordinates and
     makes possible conversions between them.
 
     Keeps track of the native structure of the grid (cartesian UTM / sperical).
     """
 
     def __init__(
         self, x=None, y=None, lon=None, lat=None, name: str = "LonelySkeleton", **kwargs
     ) -> None:
         self.name = name
         self._init_structure(x, y, lon, lat, **kwargs)
+            
+
+    @classmethod
+    def from_ds(cls, ds: xr.Dataset, **kwargs):
+        """Generats a PointSkeleton from an xarray Dataset. All coordinates must be present, but only matching data variables included."""
+        coords = list(ds.coords) + list(kwargs.keys())
+
+       
+        # Getting mandatory spatial variables
+        lon, lat = ds.get('lon'), ds.get('lat')
+        x, y = ds.get('x'), ds.get('y')
+       
+        if lon is not None:
+            lon = lon.values
+        if lat is not None:
+            lat = lat.values
+        if x is not None:
+            x = x.values
+        if y is not None:
+            y = y.values
+
+        if x is None and y is None and lon is None and lat is None:
+            raise ValueError("Can't find x/y lon/lat pair in Dataset!")
+
+        # Gather other coordinates
+        additional_coords = {}
+        for coord in [coord for coord in coords if coord not in ['inds', 'lon','lat', 'x','y']]:
+            ds_val = ds.get(coord)
+            if ds_val is not None:
+                ds_val = ds_val.values
+            provided_val =kwargs.get(coord)
+
+            val = provided_val
+            if val is None:
+                val = ds_val
+            #val = provided_val or ds_val
+            if val is None:
+                raise ValueError(f"Can't find required coordinate {coord} in Dataset or in kwargs!")
+            additional_coords[coord] = val
+
+
+        # Initialize Skeleton
+        points = cls(x=x, y=y, lon=lon, lat=lat, **additional_coords)
+
+        # Set data variables and masks that exist
+        for data_var in points.data_vars():
+            val = ds.get(data_var)
+            if val is not None:
+                points.set(data_var, val)
+
+        points.set_metadata(ds.attrs)
+
+        return points
+
+    def __iter__(self):
+        return SkeletonIterator(self._ds_manager.coords_dict('all'), self._ds_manager.coords_dict('grid').keys(), self)
+
+
+
 
     def _init_structure(self, x=None, y=None, lon=None, lat=None, **kwargs) -> None:
         """Determines grid type (Cartesian/Spherical), generates a DatasetManager
         and initializes the Xarray dataset within the DatasetManager.
 
         The initial coordinates and variables are read from the method of the
         subclass (e.g. PointSkeleton)
@@ -59,21 +166,21 @@
             self._coord_manager = CoordinateManager()
 
         # Initial values defined in subclass (e.g. GriddedSkeleton)
         self._coord_manager.set_initial_coords(self._initial_coords())
         self._coord_manager.set_initial_vars(self._initial_vars())
 
         x, y, lon, lat, kwargs = sanitize_input(
-            x, y, lon, lat, self.is_gridded(), self._structure_initialized(), **kwargs
+            x, y, lon, lat, self.is_gridded(), **kwargs
         )
 
         x_str, y_str, xvec, yvec = will_grid_be_spherical_or_cartesian(x, y, lon, lat)
 
-        if not self._structure_initialized() and self.is_gridded():
-            xvec, yvec = coord_len_to_max_two(xvec), coord_len_to_max_two(yvec)
+        # if not self._structure_initialized() and self.is_gridded():
+        #     xvec, yvec = coord_len_to_max_two(xvec), coord_len_to_max_two(yvec)
 
         self.x_str = x_str
         self.y_str = y_str
 
         # The manager contains the Xarray Dataset
         if not self._structure_initialized():
             self._ds_manager = DatasetManager(self._coord_manager)
@@ -87,82 +194,179 @@
         return hasattr(self, "_ds_manager")
 
     def _skeleton_empty(self) -> bool:
         if not self._structure_initialized():
             return True
         return len(self.ds()[self.x_str]) == 0 and len(self.ds()[self.y_str]) == 0
 
-    def _absorb_skeleton(self, skeleton_to_absorb, dimension: str) -> None:
+    def absorb(self, skeleton_to_absorb, dim: str) -> None:
         """Absorb another object of same type. This is used e.g. when pathcing
         cached data and joining different Boundary etc. over time.
         """
-        if not self.is_gridded():
+        if not self.is_gridded() and dim == 'inds':
             inds = skeleton_to_absorb.inds() + len(self.inds())
             skeleton_to_absorb.ds()["inds"] = inds
-        self._ds_manager.set_new_ds(
-            xr.concat(
-                [self.ds(), skeleton_to_absorb.ds()], dim=dimension, data_vars="minimal"
-            ).sortby(dimension)
-        )
+
+        new_skeleton = self.from_ds(xr.concat(
+                    [self.ds(), skeleton_to_absorb.ds()],  dim=dim, data_vars="minimal"
+                ).sortby(dim))
+        return new_skeleton
 
     def _reset_masks(self) -> None:
         """Resets the mask to default values."""
         for name in self._coord_manager.added_masks():
             # update-method sets empty mask when no is provided
-            self._update_mask(name)
+            self.set(name)
 
     def _reset_datavars(self) -> None:
         """Resets the data variables to default values."""
         for name in self._coord_manager.added_vars():
             # update-method sets empty mask when no is provided
-            self._update_datavar(name)
+            self.set(name)
+
+    def data_vars(self) -> None:
+        return list(self._coord_manager.added_vars().keys())
+
+    def sel(self, **kwargs):
+        return self.from_ds(self.ds().sel(**kwargs))
 
-    def _update_mask(self, name: str, updated_mask=None) -> None:
-        coords = self._coord_manager.added_masks().get(name)
-        if name is None:
+    def isel(self, **kwargs):
+        return self.from_ds(self.ds().isel(**kwargs))
+
+    def insert(self, name: str, data: np.ndarray, **kwargs) -> None:
+        """Inserts a slice of data into the Skeleton. 
+        
+        If data named 'geodata' has shape dimension ('time', 'inds', 'threshold') and shape (57, 10, 3), then 
+        data_slice having the threshold=0.4 and time='2023-11-08 12:00:00' having shape=(10,) can be inserted by using the values:
+        
+        .insert(name='geodata', data=data_slice, time='2023-11-08 12:00:00', threshold=0.4)"""
+        dims = self.ds().dims
+        index_kwargs = {}
+        for dim in dims:
+            val = kwargs.get(dim)
+            if val is not None:
+                index_kwargs[dim] = np.where(self.get(dim)==val)[0][0]
+        
+        self.ind_insert(name=name, data=data, **index_kwargs)
+
+    def ind_insert(self, name: str, data: np.ndarray, **kwargs) -> None:
+        """Inserts a slice of data into the Skeleton. 
+        
+        If data named 'geodata' has dimension ('time', 'inds', 'threshold') and shape (57, 10, 3), then 
+        data_slice having the first threshold and first time can be inserted by using the index values:
+        
+        .insert(name='geodata', data=data_slice, time=0, threshold=0)"""
+
+        dims = self.ds().dims
+        index_list = list(np.arange(len(dims)))
+        for n, dim in enumerate(dims):
+            var = self.get(dim)
+            if var is None:
+                raise KeyError(f"No coordinate {dim} exists!")
+            ind = kwargs.get(dim, slice(len(var)))
+            index_list[n] = ind
+
+        old_data = self.get(name)
+        N = len(old_data.shape)
+        data_str = 'old_data['
+        for n in range(N):
+            data_str += f"{index_list[n]},"
+        data_str = data_str[:-1]
+        data_str += '] = data'
+        exec(data_str)
+        self.set(name, old_data)
+        return
+            
+
+
+    def set(self, name: str, data=None, allow_reshape: bool=False, coords: list[str]=None, silent:bool=True) -> None:
+        var_coord_type = self._coord_manager.added_vars().get(name)
+        mask_coord_type = self._coord_manager.added_masks().get(name)
+
+        coord_type = var_coord_type or mask_coord_type
+        metadata = self.metadata()
+        if coord_type is None:
             raise ValueError(
-                f"A mask named {name} has not been defines ({list(self._coord_manager.added_masks().keys())})"
+                f"A data variable named {name} has not been defines ({list(self._coord_manager.added_vars().keys())}, {list(self._coord_manager.added_masks().keys())})"
             )
 
-        if updated_mask is None:
-            updated_mask = self.get(f"{name}_mask", empty=True)
+        if data is None:
+            data = self.get(name, empty=True)
 
-        self._ds_manager.set(
-            data=updated_mask.astype(int), data_name=f"{name}_mask", coord_type=coords
-        )
+        if mask_coord_type is not None:
+            data = data.astype(int)
 
-    def _update_datavar(self, name: str, updated_var=None) -> None:
-        coords = self._coord_manager.added_vars().get(name)
-        if name is None:
-            raise ValueError(
-                f"A data variable named {name} has not been defines ({list(self._coord_manager.added_vars().keys())})"
-            )
+        if isinstance(data, xr.DataArray):
+            coords = list(data.dims)
+            data = data.values
+
+        if coords is not None:
+            data_coordinates = list(self.get(name, data_array=True).dims)
+            if len(data_coordinates) != len(coords):
+                allow_reshape = True # We have some trivial dimension that needs to be expanded
+            shape_list = [coords.index(c) for c in data_coordinates if c in coords]
+            if shape_list != [n for n in range(len(shape_list))]: # Don't reshape trivially
+                if not silent:
+                    print(f'Reshaping data {data.shape} -> {np.transpose(data, tuple(shape_list)).shape}: {coords} -> {data_coordinates}')
+                data = np.transpose(data, tuple(shape_list))
+
+        try:
+            self._ds_manager.set(data=data, data_name=name, coord_type=coord_type)
+        except DataWrongDimensionError as data_error:
+            if allow_reshape:
+                if not silent:
+                    print(f'Size of {name} does not match size of {type(self).__name__}, trying to reshape...')
+                if len(data.shape) == 2 and len(self.size(coord_type)) ==2 and sum(data.shape) == sum(self.size(coord_type)):
+                    if not silent:
+                        print(f'Transposing data {data.shape} -> {data.T.shape}...')
+                    reshaped_data = data.T
+                elif len(data.shape) == 2 and len(self.size(coord_type, squeeze=True)) ==2 and sum(data.shape) == sum(self.size(coord_type, squeeze=True)) and data.shape != self.size(coord_type, squeeze=True):
+                    if not silent:
+                        print(f'Transposing and reshaping data {data.shape} -> {data.T.shape} -> {self.size(coord_type)}')
+                    reshaped_data = np.reshape(data.T, self.size(coord_type))
+                else:
+                    if len(data.shape) > len(self.size(coord_type)):   
+                        if not silent:
+                            print(f'Squeezing data {data.shape} -> {self.size(coord_type)}...')
+                    else:
+                        if not silent:
+                            print(f'Expanding data {data.shape} -> {self.size(coord_type)}...')
+                    reshaped_data = np.reshape(data, self.size(coord_type))
+                self._ds_manager.set(data=reshaped_data, data_name=name, coord_type=coord_type)
+            else:
+                raise data_error
 
-        if updated_var is None:
-            updated_var = self.get(name, empty=True)
-        self._ds_manager.set(data=updated_var, data_name=name, coord_type=coords)
+        self.set_metadata(metadata)
 
-    def get(self, name, empty=False):
+    def get(self, name, empty=False, data_array: bool=False, squeeze: bool=False, boolean_mask: bool=False, **kwargs):
         """Gets a mask or data variable.
 
         The ds_manager always gets what is in the Dataset (integers for masks).
         The Skeletons get-method gives boolen masks, and you can also
         request empty masks that will be return even if data doesn't exist."""
         if not self._structure_initialized():
             return None
 
-        if empty:
-            return eval(f"self.{name}(empty=True)")
+        data = self._ds_manager.get(name, empty=empty, **kwargs)
 
-        data = self._ds_manager.get(name)
-        if data is None:
+        if not isinstance(data, xr.DataArray):
             return None
 
-        data = eval(f"self.{name}()")
-        return data
+        data = data.copy()
+
+        if boolean_mask:
+            data.values = data.values.astype(bool)
+
+        if squeeze:
+            data = data.squeeze(drop=True)
+
+        if data_array:
+            return data
+        else:
+            return data.values
 
     def is_empty(self, name):
         """Checks if a Dataset variable is empty.
 
         Empty means all initial values OR all 0 values."""
         data = self.get(name)
         if data is None:
@@ -210,15 +414,15 @@
 
                 # *** ValueError: latitudes must all have the same sign
                 if len(lat[lat >= 0]) > len(lat[lat < 0]):
                     lat, lon = lat[lat >= 0], lon[lat >= 0]
                 else:
                     lat, lon = lat[lat < 0], lon[lat < 0]
 
-                __, __, zone_number, zone_letter = utm.from_latlon(lat, lon)
+                __, __, zone_number, zone_letter = utm_module.from_latlon(lat, lon)
         else:
             zone_number, zone_letter = utm_zone
 
         if isinstance(zone_number, int) or isinstance(zone_number, float):
             number = copy(int(zone_number))
         else:
             raise ValueError("zone_number needs to be an integer")
@@ -251,29 +455,34 @@
         return zone_number, zone_letter
 
     def ds(self):
         if not self._structure_initialized():
             return None
         return self._ds_manager.ds()
 
-    def size(self, coords: str = "all", **kwargs) -> tuple[int]:
+    def size(self, coords: str = "all", squeeze: bool = False, **kwargs) -> tuple[int]:
         """Returns the size of the Dataset.
 
         'all' [default]: size of entire Dataset
         'spatial': size over coordinates from the Skeleton (x, y, lon, lat, inds)
         'grid': size over coordinates for the grid (e.g. z, time)
         'gridpoint': size over coordinates for a grid point (e.g. frequency, direcion or time)
         """
 
         if not self._structure_initialized():
             return None
-        return self._ds_manager.coords_to_size(
+        
+        size = self._ds_manager.coords_to_size(
             self._ds_manager.coords(coords), **kwargs
         )
 
+        if squeeze:
+            size = tuple([s for s in size if s >1])
+        return size
+
     def inds(self, **kwargs) -> np.ndarray:
         if not self._structure_initialized():
             return None
         inds = self._ds_manager.get("inds", **kwargs)
         if inds is None:
             return None
         vals = inds.values.copy()
@@ -282,152 +491,171 @@
         return vals
 
     def x(
         self,
         native: bool = False,
         strict: bool = False,
         normalize: bool = False,
+        utm: tuple[int, str] = None,
         **kwargs,
     ) -> np.ndarray:
         """Returns the cartesian x-coordinate.
 
         If the grid is spherical, a conversion to UTM coordinates is made based on the medain latitude.
 
         If native=True, then longitudes are returned for spherical grids instead
         If strict=True, then None is returned if grid is sperical
 
         native=True overrides strict=True for spherical grids
+
+        Give utm to get cartesian coordinates in specific utm system. Otherwise defaults to the one set for the grid.
         """
 
         if not self._structure_initialized():
             return None
 
         if not self.is_cartesian() and native:
             return self.lon(**kwargs)
 
         if not self.is_cartesian() and (strict or self.strict):
             return None
 
-        if self.is_cartesian():
+        if self.is_cartesian() and (self.utm() == utm or utm is None):
             x = self._ds_manager.get("x", **kwargs).values.copy()
-        else:
+            if normalize:
+                x = x - min(x)
+            return x
+    
+        if utm is None:
             number, letter = self.utm()
-            if (
-                self.is_gridded()
-            ):  # This will rotate the grid, but is best estimate to keep it strucutred
-                lat = np.median(self.lat(**kwargs))
-                # print(
-                #    "Regridding spherical grid to cartesian coordinates. This will cause a rotation!"
-                # )
-                x, __, __, __ = utm.from_latlon(
-                    lat,
-                    self.lon(**kwargs),
+        else:
+            number, letter = utm
+            
+        if (
+            self.is_gridded()
+        ):  # This will rotate the grid, but is best estimate to keep it strucutred
+            lat = np.median(self.lat(**kwargs))
+            # print(
+            #    "Regridding spherical grid to cartesian coordinates. This will cause a rotation!"
+            # )
+            x, __, __, __ = utm_module.from_latlon(
+                lat,
+                self.lon(**kwargs),
+                force_zone_number=number,
+                force_zone_letter=letter,
+            )
+        else:
+            lat = self.lat(**kwargs)
+            lat = cap_lat_for_utm(lat)
+
+            posmask = lat >= 0
+            negmask = lat < 0
+            x = np.zeros(len(lat))
+            if np.any(posmask):
+                x[posmask], __, __, __ = utm_module.from_latlon(
+                    lat[posmask],
+                    self.lon(**kwargs)[posmask],
+                    force_zone_number=number,
+                    force_zone_letter=letter,
+                )
+            if np.any(negmask):
+                x[negmask], __, __, __ = utm_module.from_latlon(
+                    -lat[negmask],
+                    self.lon(**kwargs)[negmask],
                     force_zone_number=number,
                     force_zone_letter=letter,
                 )
-            else:
-                lat = self.lat(**kwargs)
-                lat = cap_lat_for_utm(lat)
-
-                posmask = lat >= 0
-                negmask = lat < 0
-                x = np.zeros(len(lat))
-                if np.any(posmask):
-                    x[posmask], __, __, __ = utm.from_latlon(
-                        lat[posmask],
-                        self.lon(**kwargs)[posmask],
-                        force_zone_number=number,
-                        force_zone_letter=letter,
-                    )
-                if np.any(negmask):
-                    x[negmask], __, __, __ = utm.from_latlon(
-                        -lat[negmask],
-                        self.lon(**kwargs)[negmask],
-                        force_zone_number=number,
-                        force_zone_letter=letter,
-                    )
 
         if normalize:
             x = x - min(x)
 
         return x
 
     def y(
         self,
         native: bool = False,
         strict: bool = False,
         normalize: bool = False,
+        utm: tuple[int, str] = None,
         **kwargs,
     ) -> np.ndarray:
         """Returns the cartesian y-coordinate.
 
         If the grid is spherical, a conversion to UTM coordinates is made based on the medain latitude.
 
         If native=True, then latitudes are returned for spherical grids instead
         If strict=True, then None is returned if grid is sperical
 
         native=True overrides strict=True for spherical grids
+
+        Give utm to get cartesian coordinates in specific utm system. Otherwise defaults to the one set for the grid.
         """
 
         if not self._structure_initialized():
             return None
 
         if not self.is_cartesian() and native:
             return self.lat(**kwargs)
 
         if not self.is_cartesian() and (strict or self.strict):
             return None
 
-        if self.is_cartesian():
+        if self.is_cartesian() and (self.utm() == utm or utm is None):
             y = self._ds_manager.get("y", **kwargs).values.copy()
-        else:
+            if normalize:
+                y = y - min(y)
+            return y
+
+        if utm is None:
             number, letter = self.utm()
-            posmask = self.lat(**kwargs) >= 0
-            negmask = self.lat(**kwargs) < 0
-            if (
-                self.is_gridded()
-            ):  # This will rotate the grid, but is best estimate to keep it strucutred
-                lon = np.median(self.lon(**kwargs))
-                # print(
-                #    "Regridding spherical grid to cartesian coordinates. This will cause a rotation!"
-                # )
-                y = np.zeros(len(self.lat(**kwargs)))
-                if np.any(posmask):
-                    _, y[posmask], __, __ = utm.from_latlon(
-                        self.lat(**kwargs)[posmask],
-                        lon,
-                        force_zone_number=number,
-                        force_zone_letter=letter,
-                    )
-                if np.any(negmask):
-                    _, y[negmask], __, __ = utm.from_latlon(
-                        -self.lat(**kwargs)[negmask],
-                        lon,
-                        force_zone_number=number,
-                        force_zone_letter=letter,
-                    )
-                    y[negmask] = -y[negmask]
-            else:
-                lat = cap_lat_for_utm(self.lat(**kwargs))
-                y = np.zeros(len(self.lat(**kwargs)))
-                if np.any(posmask):
-                    _, y[posmask], __, __ = utm.from_latlon(
-                        lat[posmask],
-                        self.lon(**kwargs)[posmask],
-                        force_zone_number=number,
-                        force_zone_letter=letter,
-                    )
-                if np.any(negmask):
-                    _, y[negmask], __, __ = utm.from_latlon(
-                        -lat[negmask],
-                        self.lon(**kwargs)[negmask],
-                        force_zone_number=number,
-                        force_zone_letter=letter,
-                    )
-                    y[negmask] = -y[negmask]
+        else:
+            number, letter = utm
+        posmask = self.lat(**kwargs) >= 0
+        negmask = self.lat(**kwargs) < 0
+        if (
+            self.is_gridded()
+        ):  # This will rotate the grid, but is best estimate to keep it strucutred
+            lon = np.median(self.lon(**kwargs))
+            # print(
+            #    "Regridding spherical grid to cartesian coordinates. This will cause a rotation!"
+            # )
+            y = np.zeros(len(self.lat(**kwargs)))
+            if np.any(posmask):
+                _, y[posmask], __, __ = utm_module.from_latlon(
+                    self.lat(**kwargs)[posmask],
+                    lon,
+                    force_zone_number=number,
+                    force_zone_letter=letter,
+                )
+            if np.any(negmask):
+                _, y[negmask], __, __ = utm_module.from_latlon(
+                    -self.lat(**kwargs)[negmask],
+                    lon,
+                    force_zone_number=number,
+                    force_zone_letter=letter,
+                )
+                y[negmask] = -y[negmask]
+        else:
+            lat = cap_lat_for_utm(self.lat(**kwargs))
+            y = np.zeros(len(self.lat(**kwargs)))
+            if np.any(posmask):
+                _, y[posmask], __, __ = utm_module.from_latlon(
+                    lat[posmask],
+                    self.lon(**kwargs)[posmask],
+                    force_zone_number=number,
+                    force_zone_letter=letter,
+                )
+            if np.any(negmask):
+                _, y[negmask], __, __ = utm_module.from_latlon(
+                    -lat[negmask],
+                    self.lon(**kwargs)[negmask],
+                    force_zone_number=number,
+                    force_zone_letter=letter,
+                )
+                y[negmask] = -y[negmask]
 
         if normalize:
             y = y - min(y)
 
         return y
 
     def lon(self, native: bool = False, strict=False, **kwargs) -> np.ndarray:
@@ -456,15 +684,15 @@
                 y = np.median(self.y(**kwargs))
                 # print(
                 #    "Regridding cartesian grid to spherical coordinates. This will cause a rotation!"
                 # )
             else:
                 y = self.y(**kwargs)
             number, letter = self.utm()
-            __, lon = utm.to_latlon(
+            __, lon = utm_module.to_latlon(
                 self.x(**kwargs),
                 np.mod(y, 10_000_000),
                 zone_number=number,
                 zone_letter=letter,
                 strict=False,
             )
 
@@ -497,15 +725,15 @@
                 x = np.median(self.x(**kwargs))
                 # print(
                 #    "Regridding cartesian grid to spherical coordinates. This will cause a rotation!"
                 # )
             else:
                 x = self.x(**kwargs)
             number, letter = self.utm()
-            lat, __ = utm.to_latlon(
+            lat, __ = utm_module.to_latlon(
                 x,
                 np.mod(self.y(**kwargs), 10_000_000),
                 zone_number=number,
                 zone_letter=letter,
                 strict=False,
             )
             return lat
@@ -631,36 +859,36 @@
         Set unique=True to remove any repeated points.
         Set fast=True to use UTM casrtesian search for low latitudes."""
 
         if self.is_cartesian():
             fast = True
 
         # If lon/lat is given, convert to cartesian and set grid UTM zone to match the query point
-        x = force_to_iterable(x, fmt="numpy")
-        y = force_to_iterable(y, fmt="numpy")
-        lon = force_to_iterable(lon, fmt="numpy")
-        lat = force_to_iterable(lat, fmt="numpy")
+        x = force_to_iterable(x)
+        y = force_to_iterable(y)
+        lon = force_to_iterable(lon)
+        lat = force_to_iterable(lat)
 
         if all([x is None for x in (x, y, lon, lat)]):
             raise ValueError("Give either x-y pair or lon-lat pair!")
 
         orig_zone = self.utm()
         if lon is not None and lat is not None:
             if self.is_cartesian():
-                x, y, __, __ = utm.from_latlon(
+                x, y, __, __ = utm_module.from_latlon(
                     lat,
                     lon,
                     force_zone_number=orig_zone[0],
                     force_zone_letter=orig_zone[1],
                 )
             else:
-                x, y, zone_number, zone_letter = utm.from_latlon(lat, lon)
+                x, y, zone_number, zone_letter = utm_module.from_latlon(lat, lon)
                 self.set_utm((zone_number, zone_letter), silent=True)
         else:
-            lat, lon = utm.to_latlon(
+            lat, lon = utm_module.to_latlon(
                 x,
                 y,
                 zone_number=orig_zone[0],
                 zone_letter=orig_zone[1],
                 strict=False,
             )
 
@@ -699,15 +927,15 @@
         else:
             return {"inds": np.array(inds), "dx": np.array(dx)}
 
     def metadata(self) -> dict:
         """Return metadata of the dataset:"""
         if not self._structure_initialized():
             return None
-        return self.ds().attrs
+        return self.ds().attrs.copy()
 
     def set_metadata(
         self, metadata: dict, append=False, data_array_name: str = None
     ) -> None:
         if not self._structure_initialized():
             return None
         if append:
@@ -783,25 +1011,23 @@
     @name.setter
     def name(self, new_name):
         if isinstance(new_name, str):
             self._name = new_name
         else:
             raise ValueError("name needs to be a string")
 
-
 def coord_len_to_max_two(xvec):
     if xvec is not None and len(xvec) > 2:
         xvec = np.array([min(xvec), max(xvec)])
     return xvec
 
 
-def sanitize_singe_variable(name: str, x, fmt: str = "numpy"):
+def sanitize_singe_variable(name: str, x):
     """Forces to nump array and checks dimensions etc"""
-
-    x = force_to_iterable(x, fmt=fmt)
+    x = force_to_iterable(x)
 
     # np.array([None, None]) -> None
     if x is None or all(v is None for v in x):
         x = None
 
     if x is not None and len(x.shape) > 1:
         raise Exception(
@@ -850,36 +1076,54 @@
     """Takes only edges of arrays, so [1,2,3] -> [1,3]"""
     for key, value in spatial.items():
         if value is not None:
             spatial[key] = coord_len_to_max_two(value)
 
     return spatial
 
+def check_that_variables_equal_length(x, y) -> bool:
+    if x is None and y is None:
+        return True
+    if x is None:
+        raise ValueError(f"x/lon variable None even though y/lat variable is not!")
+    if y is None:
+        raise ValueError(f"y/lat variable None even though x/lon variable is not!")
+    return len(x) == len(y)
+
 
-def sanitize_input(x, y, lon, lat, is_gridded_format, is_initialized, **kwargs):
+def sanitize_time_input(time):
+    if isinstance(time, str):
+        return pd.DatetimeIndex([time])
+    if not isinstance(time, Iterable):
+        return pd.DatetimeIndex([time])
+    return pd.DatetimeIndex(time)
+
+def sanitize_input(x, y, lon, lat, is_gridded_format, **kwargs):
     """Sanitizes input. After this all variables are either
     non-empty np.ndarrays with len >= 1 or None"""
 
     spatial = {"x": x, "y": y, "lon": lon, "lat": lat}
     for key, value in spatial.items():
         spatial[key] = sanitize_singe_variable(key, value)
 
     other = {}
     for key, value in kwargs.items():
         if key == "time":
             # other[key] = sanitize_singe_variable(key, value, fmt="datetime")
-            other[key] = value
+            other[key] = sanitize_time_input(value)
         else:
             other[key] = sanitize_singe_variable(key, value)
 
     if not is_gridded_format:
         spatial = sanitize_point_structure(spatial)
-    else:
-        if not is_initialized:
-            spatial = get_edges_of_arrays(spatial)
+
+        for x, y in [('x','y'), ('lon','lat')]:
+            length_ok = check_that_variables_equal_length(spatial[x], spatial[y])
+            if not length_ok:
+                raise Exception(f"{x} is length {len(spatial[x])} but {y} is length {len(spatial[y])}!")
 
     if np.all([a is None for a in spatial.values()]):
         raise Exception("x, y, lon, lat cannot ALL be None!")
 
     return spatial["x"], spatial["y"], spatial["lon"], spatial["lat"], other
 
 
@@ -946,33 +1190,22 @@
         print(
             f"Min latitude {min(lat)}<-80. These points well be capped to -80 deg in UTM conversion!"
         )
     return lat
 
 
 def force_to_iterable(x, fmt: str = None) -> Iterable:
-    """Returns original x if iterable, but tries to convert it to numpy array if it is e.g. integer of float.
-
-    fmt = 'numpy', 'list' or 'tuple' to force to certain format
+    """Returns an numpy array with at least one dimension and Nones removed
 
     Will return None if given None."""
     if x is None:
         return None
 
-    if not isinstance(x, Iterable):
-        x = [x]
-
-    x = [float(a) for a in x if a is not None]
-
-    if fmt == "numpy":
-        x = np.array(x)
-    elif fmt == "list":
-        x = list(x)
-    elif fmt == "tuple":
-        x = tuple(x)
+    x = np.atleast_1d(x)
+    x = np.array([a for a in x if a is not None])
 
     return x
 
 
 def valid_utm_zone(utm_zone: tuple[int, str]) -> bool:
     """Checks that a UTM zone, e.g. (33, 'V') is valid."""
```

### Comparing `geo_skeletons-0.9.8/tests/test_absorb_skeleton.py` & `geo_skeletons-0.9.9/tests/test_gridded_init_strict_and_native.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,100 @@
-from geo_skeletons.point_skeleton import PointSkeleton
 from geo_skeletons.gridded_skeleton import GriddedSkeleton
 import numpy as np
 
 
-def test_absorb_point_cartesian():
-    grid = PointSkeleton(x=(1, 2), y=(0, 3))
-    grid2 = PointSkeleton(x=(3, 4), y=(0, 3))
-    grid._absorb_skeleton(grid2, dimension="inds")
+def test_spherical_strict():
+    grid = GriddedSkeleton(lon=(1, 2), lat=(0, 3))
+
+    assert grid.x(strict=True) is None
+    assert grid.y(strict=True) is None
+
+    np.testing.assert_array_almost_equal(grid.lon(strict=True), np.array([1, 2]))
+    np.testing.assert_array_almost_equal(grid.lat(strict=True), np.array([0, 3]))
+
+    np.testing.assert_array_almost_equal(
+        grid.lonlat(strict=True), (np.array([1, 2, 1, 2]), np.array([0, 0, 3, 3]))
+    )
+
+    assert grid.xy(strict=True) == (None, None)
+
+
+def test_spherical_global_strict():
+    grid = GriddedSkeleton(lon=(1, 2), lat=(0, 3))
+    grid.strict = True
+
+    assert grid.x(strict=False) is None
+    assert grid.y(strict=False) is None
+
+    np.testing.assert_array_almost_equal(grid.lon(strict=True), np.array([1, 2]))
+    np.testing.assert_array_almost_equal(grid.lat(strict=True), np.array([0, 3]))
+
+    np.testing.assert_array_almost_equal(
+        grid.lonlat(strict=True), (np.array([1, 2, 1, 2]), np.array([0, 0, 3, 3]))
+    )
+
+    assert grid.xy(strict=False) == (None, None)
+
+
+def test_spherical_native():
+    grid = GriddedSkeleton(lon=(1, 2), lat=(0, 3))
+
+    np.testing.assert_array_almost_equal(grid.lon(native=True), np.array([1, 2]))
+    np.testing.assert_array_almost_equal(grid.lat(native=True), np.array([0, 3]))
+    np.testing.assert_array_almost_equal(grid.x(native=True), np.array([1, 2]))
+    np.testing.assert_array_almost_equal(grid.y(native=True), np.array([0, 3]))
 
-    np.testing.assert_array_almost_equal(grid.x(), np.array([1, 2, 3, 4]))
-    np.testing.assert_array_almost_equal(grid.x(normalize=True), np.array([0, 1, 2, 3]))
-    np.testing.assert_array_almost_equal(grid.y(), np.array([0, 3, 0, 3]))
-    np.testing.assert_array_almost_equal(grid.y(normalize=True), np.array([0, 3, 0, 3]))
-    np.testing.assert_array_almost_equal(grid.inds(), np.array([0, 1, 2, 3]))
     np.testing.assert_array_almost_equal(
-        grid.xy(), (np.array([1, 2, 3, 4]), np.array([0, 3, 0, 3]))
+        grid.lonlat(native=True), (np.array([1, 2, 1, 2]), np.array([0, 0, 3, 3]))
+    )
+    np.testing.assert_array_almost_equal(
+        grid.xy(native=True), (np.array([1, 2, 1, 2]), np.array([0, 0, 3, 3]))
     )
 
 
-def test_absorb_point_spherical():
-    grid = PointSkeleton(lon=(1, 2), lat=(0, 3))
-    grid2 = PointSkeleton(lon=(3, 4), lat=(0, 3))
-    grid._absorb_skeleton(grid2, dimension="inds")
+def test_cartesian_strict():
+    grid = GriddedSkeleton(x=(1, 2), y=(0, 3))
+
+    assert grid.lon(strict=True) is None
+    assert grid.lat(strict=True) is None
+
+    np.testing.assert_array_almost_equal(grid.x(strict=True), np.array([1, 2]))
+    np.testing.assert_array_almost_equal(grid.y(strict=True), np.array([0, 3]))
 
-    np.testing.assert_array_almost_equal(grid.lon(), np.array([1, 2, 3, 4]))
-    np.testing.assert_array_almost_equal(grid.lat(), np.array([0, 3, 0, 3]))
-    np.testing.assert_array_almost_equal(grid.inds(), np.array([0, 1, 2, 3]))
     np.testing.assert_array_almost_equal(
-        grid.lonlat(), (np.array([1, 2, 3, 4]), np.array([0, 3, 0, 3]))
+        grid.xy(strict=True), (np.array([1, 2, 1, 2]), np.array([0, 0, 3, 3]))
     )
 
+    assert grid.lonlat(strict=True) == (None, None)
 
-def test_absorb_gridded_cartesian():
+
+def test_cartesian_global_strict():
     grid = GriddedSkeleton(x=(1, 2), y=(0, 3))
-    grid.set_spacing(nx=2, ny=2)
-    grid2 = GriddedSkeleton(x=(3, 4), y=(0, 3))
-    grid2.set_spacing(nx=2, ny=2)
-    grid._absorb_skeleton(grid2, dimension="x")
-    assert grid.inds() is None
-    np.testing.assert_array_almost_equal(grid.x(), np.array([1, 2, 3, 4]))
-    np.testing.assert_array_almost_equal(grid.x(normalize=True), np.array([0, 1, 2, 3]))
-    np.testing.assert_array_almost_equal(grid.y(), np.array([0, 3]))
-    np.testing.assert_array_almost_equal(grid.y(normalize=True), np.array([0, 3]))
+    grid.strict = True
+
+    assert grid.lon(strict=False) is None
+    assert grid.lat(strict=False) is None
+
+    np.testing.assert_array_almost_equal(grid.x(strict=True), np.array([1, 2]))
+    np.testing.assert_array_almost_equal(grid.y(strict=True), np.array([0, 3]))
+
     np.testing.assert_array_almost_equal(
-        grid.xy(),
-        (np.array([1, 2, 3, 4, 1, 2, 3, 4]), np.array([0, 0, 0, 0, 3, 3, 3, 3])),
+        grid.xy(strict=True), (np.array([1, 2, 1, 2]), np.array([0, 0, 3, 3]))
     )
 
+    assert grid.lonlat(strict=False) == (None, None)
 
-def test_absorb_gridded_spherical():
-    grid = GriddedSkeleton(lon=(1, 2), lat=(0, 3))
-    grid.set_spacing(nx=2, ny=2)
-    grid2 = GriddedSkeleton(lon=(3, 4), lat=(0, 3))
-    grid2.set_spacing(nx=2, ny=2)
-    grid._absorb_skeleton(grid2, dimension="lon")
-    assert grid.inds() is None
-    np.testing.assert_array_almost_equal(grid.lon(), np.array([1, 2, 3, 4]))
-    np.testing.assert_array_almost_equal(grid.lat(), np.array([0, 3]))
+
+def test_cartesian_native():
+    grid = GriddedSkeleton(x=(1, 2), y=(0, 3))
+
+    np.testing.assert_array_almost_equal(grid.lon(native=True), np.array([1, 2]))
+    np.testing.assert_array_almost_equal(grid.lat(native=True), np.array([0, 3]))
+    np.testing.assert_array_almost_equal(grid.x(native=True), np.array([1, 2]))
+    np.testing.assert_array_almost_equal(grid.y(native=True), np.array([0, 3]))
+
+    np.testing.assert_array_almost_equal(
+        grid.lonlat(native=True), (np.array([1, 2, 1, 2]), np.array([0, 0, 3, 3]))
+    )
     np.testing.assert_array_almost_equal(
-        grid.lonlat(),
-        (np.array([1, 2, 3, 4, 1, 2, 3, 4]), np.array([0, 0, 0, 0, 3, 3, 3, 3])),
+        grid.xy(native=True), (np.array([1, 2, 1, 2]), np.array([0, 0, 3, 3]))
     )
```

### Comparing `geo_skeletons-0.9.8/tests/test_add_coords_gridded.py` & `geo_skeletons-0.9.9/tests/test_add_coords_gridded.py`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/tests/test_add_coords_point.py` & `geo_skeletons-0.9.9/tests/test_add_coords_point.py`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/tests/test_add_datavar_gridded.py` & `geo_skeletons-0.9.9/tests/test_add_datavar_gridded.py`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/tests/test_add_datavar_point.py` & `geo_skeletons-0.9.9/tests/test_add_datavar_point.py`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/tests/test_add_mask_gridded.py` & `geo_skeletons-0.9.9/tests/test_add_mask_gridded.py`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/tests/test_add_mask_point.py` & `geo_skeletons-0.9.9/tests/test_add_mask_point.py`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/tests/test_gridded_init_cartesian.py` & `geo_skeletons-0.9.9/tests/test_gridded_init_cartesian.py`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/tests/test_gridded_init_spherical.py` & `geo_skeletons-0.9.9/tests/test_gridded_init_spherical.py`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/tests/test_gridded_init_strict_and_native.py` & `geo_skeletons-0.9.9/tests/test_point_init_spherical.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,100 +1,92 @@
-from geo_skeletons.gridded_skeleton import GriddedSkeleton
+from geo_skeletons.point_skeleton import PointSkeleton
 import numpy as np
 
 
-def test_spherical_strict():
-    grid = GriddedSkeleton(lon=(1, 2), lat=(0, 3))
-
-    assert grid.x(strict=True) is None
-    assert grid.y(strict=True) is None
-
-    np.testing.assert_array_almost_equal(grid.lon(strict=True), np.array([1, 2]))
-    np.testing.assert_array_almost_equal(grid.lat(strict=True), np.array([0, 3]))
-
+def test_init_trivial():
+    grid = PointSkeleton(lon=(1, 2), lat=(0, 3))
+    repr = print(grid)
+    assert grid.nx() == 2
+    assert grid.ny() == 2
+    assert grid.size() == (2,)
+    np.testing.assert_array_almost_equal(grid.lon(), np.array([1, 2]))
+    np.testing.assert_array_almost_equal(grid.lat(), np.array([0, 3]))
+    np.testing.assert_array_almost_equal(grid.inds(), np.array([0, 1]))
     np.testing.assert_array_almost_equal(
-        grid.lonlat(strict=True), (np.array([1, 2, 1, 2]), np.array([0, 0, 3, 3]))
+        grid.lonlat(), (np.array([1, 2]), np.array([0, 3]))
     )
 
-    assert grid.xy(strict=True) == (None, None)
-
-
-def test_spherical_global_strict():
-    grid = GriddedSkeleton(lon=(1, 2), lat=(0, 3))
-    grid.strict = True
-
-    assert grid.x(strict=False) is None
-    assert grid.y(strict=False) is None
-
-    np.testing.assert_array_almost_equal(grid.lon(strict=True), np.array([1, 2]))
-    np.testing.assert_array_almost_equal(grid.lat(strict=True), np.array([0, 3]))
 
+def test_init_one_point_in_lat():
+    grid = PointSkeleton(lon=(3, 5), lat=(0, 0))
+    assert grid.nx() == 2
+    assert grid.ny() == 2
+    assert grid.size() == (2,)
+    np.testing.assert_array_almost_equal(grid.lon(), np.array([3, 5]))
+    np.testing.assert_array_almost_equal(grid.lat(), np.array([0, 0]))
+    np.testing.assert_array_almost_equal(grid.inds(), np.array([0, 1]))
     np.testing.assert_array_almost_equal(
-        grid.lonlat(strict=True), (np.array([1, 2, 1, 2]), np.array([0, 0, 3, 3]))
+        grid.lonlat(), (np.array([3, 5]), np.array([0, 0]))
     )
 
-    assert grid.xy(strict=False) == (None, None)
-
-
-def test_spherical_native():
-    grid = GriddedSkeleton(lon=(1, 2), lat=(0, 3))
 
-    np.testing.assert_array_almost_equal(grid.lon(native=True), np.array([1, 2]))
-    np.testing.assert_array_almost_equal(grid.lat(native=True), np.array([0, 3]))
-    np.testing.assert_array_almost_equal(grid.x(native=True), np.array([1, 2]))
-    np.testing.assert_array_almost_equal(grid.y(native=True), np.array([0, 3]))
-
-    np.testing.assert_array_almost_equal(
-        grid.lonlat(native=True), (np.array([1, 2, 1, 2]), np.array([0, 0, 3, 3]))
-    )
+def test_init_one_point_in_lat_constant():
+    grid = PointSkeleton(lon=(3, 5), lat=0)
+    assert grid.nx() == 2
+    assert grid.ny() == 2
+    assert grid.size() == (2,)
+    np.testing.assert_array_almost_equal(grid.lon(), np.array([3, 5]))
+    np.testing.assert_array_almost_equal(grid.lat(), np.array([0, 0]))
+    np.testing.assert_array_almost_equal(grid.inds(), np.array([0, 1]))
     np.testing.assert_array_almost_equal(
-        grid.xy(native=True), (np.array([1, 2, 1, 2]), np.array([0, 0, 3, 3]))
+        grid.lonlat(), (np.array([3, 5]), np.array([0, 0]))
     )
 
 
-def test_cartesian_strict():
-    grid = GriddedSkeleton(x=(1, 2), y=(0, 3))
-
-    assert grid.lon(strict=True) is None
-    assert grid.lat(strict=True) is None
-
-    np.testing.assert_array_almost_equal(grid.x(strict=True), np.array([1, 2]))
-    np.testing.assert_array_almost_equal(grid.y(strict=True), np.array([0, 3]))
-
+def test_init_one_point_in_lon():
+    grid = PointSkeleton(lon=(0, 0), lat=(3, 5))
+    assert grid.nx() == 2
+    assert grid.ny() == 2
+    assert grid.size() == (2,)
+    np.testing.assert_array_almost_equal(grid.lat(), np.array([3, 5]))
+    np.testing.assert_array_almost_equal(grid.lon(), np.array([0, 0]))
+    np.testing.assert_array_almost_equal(grid.inds(), np.array([0, 1]))
     np.testing.assert_array_almost_equal(
-        grid.xy(strict=True), (np.array([1, 2, 1, 2]), np.array([0, 0, 3, 3]))
+        grid.lonlat(), (np.array([0, 0]), np.array([3, 5]))
     )
 
-    assert grid.lonlat(strict=True) == (None, None)
-
-
-def test_cartesian_global_strict():
-    grid = GriddedSkeleton(x=(1, 2), y=(0, 3))
-    grid.strict = True
-
-    assert grid.lon(strict=False) is None
-    assert grid.lat(strict=False) is None
-
-    np.testing.assert_array_almost_equal(grid.x(strict=True), np.array([1, 2]))
-    np.testing.assert_array_almost_equal(grid.y(strict=True), np.array([0, 3]))
 
+def test_init_one_point_in_lon_constnat():
+    grid = PointSkeleton(lon=0, lat=(3, 5))
+    assert grid.nx() == 2
+    assert grid.ny() == 2
+    assert grid.size() == (2,)
+    np.testing.assert_array_almost_equal(grid.lat(), np.array([3, 5]))
+    np.testing.assert_array_almost_equal(grid.lon(), np.array([0, 0]))
+    np.testing.assert_array_almost_equal(grid.inds(), np.array([0, 1]))
     np.testing.assert_array_almost_equal(
-        grid.xy(strict=True), (np.array([1, 2, 1, 2]), np.array([0, 0, 3, 3]))
+        grid.lonlat(), (np.array([0, 0]), np.array([3, 5]))
     )
 
-    assert grid.lonlat(strict=False) == (None, None)
-
 
-def test_cartesian_native():
-    grid = GriddedSkeleton(x=(1, 2), y=(0, 3))
+def test_init_one_point():
+    grid = PointSkeleton(lon=0, lat=3)
+    assert grid.nx() == 1
+    assert grid.ny() == 1
+    assert grid.size() == (1,)
+    np.testing.assert_array_almost_equal(grid.lat(), np.array([3]))
+    np.testing.assert_array_almost_equal(grid.lon(), np.array([0]))
+    np.testing.assert_array_almost_equal(grid.inds(), np.array([0]))
+    np.testing.assert_array_almost_equal(grid.lonlat(), (np.array([0]), np.array([3])))
 
-    np.testing.assert_array_almost_equal(grid.lon(native=True), np.array([1, 2]))
-    np.testing.assert_array_almost_equal(grid.lat(native=True), np.array([0, 3]))
-    np.testing.assert_array_almost_equal(grid.x(native=True), np.array([1, 2]))
-    np.testing.assert_array_almost_equal(grid.y(native=True), np.array([0, 3]))
 
+def test_init_long():
+    grid = PointSkeleton(lon=[0, 2, 4, 5, 6, 6], lat=[3, 1, 2, 3, 4, 5])
+    assert grid.nx() == 6
+    assert grid.ny() == 6
+    assert grid.size() == (6,)
+    np.testing.assert_array_almost_equal(grid.lat(), np.array([3, 1, 2, 3, 4, 5]))
+    np.testing.assert_array_almost_equal(grid.lon(), np.array([0, 2, 4, 5, 6, 6]))
+    np.testing.assert_array_almost_equal(grid.inds(), np.array([0, 1, 2, 3, 4, 5]))
     np.testing.assert_array_almost_equal(
-        grid.lonlat(native=True), (np.array([1, 2, 1, 2]), np.array([0, 0, 3, 3]))
-    )
-    np.testing.assert_array_almost_equal(
-        grid.xy(native=True), (np.array([1, 2, 1, 2]), np.array([0, 0, 3, 3]))
+        grid.lonlat(), (np.array([0, 2, 4, 5, 6, 6]), np.array([3, 1, 2, 3, 4, 5]))
     )
```

### Comparing `geo_skeletons-0.9.8/tests/test_gridded_utm_conversions.py` & `geo_skeletons-0.9.9/tests/test_gridded_utm_conversions.py`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/tests/test_point_init_cartesian.py` & `geo_skeletons-0.9.9/tests/test_point_init_cartesian.py`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/tests/test_point_init_strict_and_native.py` & `geo_skeletons-0.9.9/tests/test_point_init_strict_and_native.py`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/tests/test_point_utm_conversions.py` & `geo_skeletons-0.9.9/tests/test_point_utm_conversions.py`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/tests/test_set_spacing.py` & `geo_skeletons-0.9.9/tests/test_set_spacing.py`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/tests/test_slicing_data.py` & `geo_skeletons-0.9.9/tests/test_slicing_data.py`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/tests/test_will_grid_be_spherical_or_cartesian_cartesian_input.py` & `geo_skeletons-0.9.9/tests/test_will_grid_be_spherical_or_cartesian_cartesian_input.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,107 +2,98 @@
 from geo_skeletons.skeleton import will_grid_be_spherical_or_cartesian as func
 import numpy as np
 
 
 def test_x_y_tuple():
     lon, lat = None, None
     x, y = (0.0, 1.0), (2.0, 3.0)
-    is_initialized = False
 
     for is_gridded in [True, False]:
-        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded, is_initialized)
+        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded)
 
         native_x, native_y, xvec, yvec = func(lon=lon, lat=lat, x=x, y=y)
         assert native_x == "x"
         assert native_y == "y"
         assert np.all(xvec == np.array([0.0, 1.0]))
         assert np.all(yvec == np.array([2.0, 3.0]))
 
 
 def test_x_y_tuple_none_tuple():
     lon, lat = (None, None), (None, None)
     x, y = (0.0, 1.0), (2.0, 3.0)
-    is_initialized = False
 
     for is_gridded in [True, False]:
-        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded, is_initialized)
+        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded)
 
         native_x, native_y, xvec, yvec = func(lon=lon, lat=lat, x=x, y=y)
         assert native_x == "x"
         assert native_y == "y"
         assert np.all(xvec == np.array([0.0, 1.0]))
         assert np.all(yvec == np.array([2.0, 3.0]))
 
 
 def test_x_y_int_tuple():
     lon, lat = None, None
     x, y = (0, 1), (2, 3)
-    is_initialized = False
-
     for is_gridded in [True, False]:
-        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded, is_initialized)
+        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded)
 
         native_x, native_y, xvec, yvec = func(lon=lon, lat=lat, x=x, y=y)
         assert native_x == "x"
         assert native_y == "y"
         assert np.all(xvec == np.array([0.0, 1.0]))
         assert np.all(yvec == np.array([2.0, 3.0]))
 
 
 def test_x_lat_single_tuple():
     lon, lat = None, None
     x, y = (0.0), (2.0)
-    is_initialized = False
 
     for is_gridded in [True, False]:
-        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded, is_initialized)
+        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded)
 
         native_x, native_y, xvec, yvec = func(lon=lon, lat=lat, x=x, y=y)
         assert native_x == "x"
         assert native_y == "y"
         assert np.all(xvec == np.array([0.0]))
         assert np.all(yvec == np.array([2.0]))
 
 
 def test_x_y_single_value():
     lon, lat = None, None
     x, y = 0.0, 2.0
-    is_initialized = False
 
     for is_gridded in [True, False]:
-        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded, is_initialized)
+        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded)
 
         native_x, native_y, xvec, yvec = func(lon=lon, lat=lat, x=x, y=y)
         assert native_x == "x"
         assert native_y == "y"
         assert np.all(xvec == np.array([0.0]))
         assert np.all(yvec == np.array([2.0]))
 
 
 def test_x_y_array():
     lon, lat = None, None
     x, y = np.array([0.0, 1.0, 2.0, 3.0]), np.array([2.0, 3.0, 4.0, 5.0])
-    is_initialized = True
 
     for is_gridded in [True, False]:
-        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded, is_initialized)
+        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded)
 
         native_x, native_y, xvec, yvec = func(lon=lon, lat=lat, x=x, y=y)
         assert native_x == "x"
         assert native_y == "y"
         assert np.all(xvec == np.array([0.0, 1.0, 2.0, 3.0]))
         assert np.all(yvec == np.array([2.0, 3.0, 4.0, 5.0]))
 
 
 def test_x_y_int_array():
     lon, lat = None, None
     x, y = np.array([0, 1, 2, 3]), np.array([2, 3, 4, 5])
-    is_initialized = True
-
     for is_gridded in [True, False]:
-        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded, is_initialized)
+        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded)
 
         native_x, native_y, xvec, yvec = func(lon=lon, lat=lat, x=x, y=y)
         assert native_x == "x"
         assert native_y == "y"
         assert np.all(xvec == np.array([0, 1, 2, 3]))
         assert np.all(yvec == np.array([2, 3, 4, 5]))
```

### Comparing `geo_skeletons-0.9.8/tests/test_will_grid_be_spherical_or_cartesian_spherical_input.py` & `geo_skeletons-0.9.9/tests/test_will_grid_be_spherical_or_cartesian_spherical_input.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,107 +2,99 @@
 from geo_skeletons.skeleton import will_grid_be_spherical_or_cartesian as func
 import numpy as np
 
 
 def test_lon_lat_tuple():
     x, y = None, None
     lon, lat = (0.0, 1.0), (2.0, 3.0)
-    is_initialized = False
 
     for is_gridded in [True, False]:
-        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded, is_initialized)
+        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded)
 
         native_x, native_y, xvec, yvec = func(lon=lon, lat=lat, x=x, y=y)
         assert native_x == "lon"
         assert native_y == "lat"
         assert np.all(xvec == np.array([0.0, 1.0]))
         assert np.all(yvec == np.array([2.0, 3.0]))
 
 
 def test_lon_lat_tuple_none_tuple():
     x, y = (None, None), (None, None)
     lon, lat = (0.0, 1.0), (2.0, 3.0)
-    is_initialized = False
-
     for is_gridded in [True, False]:
-        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded, is_initialized)
+        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded)
 
         native_x, native_y, xvec, yvec = func(lon=lon, lat=lat, x=x, y=y)
         assert native_x == "lon"
         assert native_y == "lat"
         assert np.all(xvec == np.array([0.0, 1.0]))
         assert np.all(yvec == np.array([2.0, 3.0]))
 
 
 def test_lon_lat_int_tuple():
     x, y = None, None
     lon, lat = (0, 1), (2, 3)
-    is_initialized = False
 
     for is_gridded in [True, False]:
-        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded, is_initialized)
+        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded)
 
         native_x, native_y, xvec, yvec = func(lon=lon, lat=lat, x=x, y=y)
         assert native_x == "lon"
         assert native_y == "lat"
         assert np.all(xvec == np.array([0.0, 1.0]))
         assert np.all(yvec == np.array([2.0, 3.0]))
 
 
 def test_lon_lat_single_tuple():
     x, y = None, None
     lon, lat = (0.0), (2.0)
-    is_initialized = False
 
     for is_gridded in [True, False]:
-        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded, is_initialized)
+        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded)
 
         native_x, native_y, xvec, yvec = func(lon=lon, lat=lat, x=x, y=y)
         assert native_x == "lon"
         assert native_y == "lat"
         assert np.all(xvec == np.array([0.0]))
         assert np.all(yvec == np.array([2.0]))
 
 
 def test_lon_lat_single_value():
     x, y = None, None
     lon, lat = 0.0, 2.0
-    is_initialized = False
 
     for is_gridded in [True, False]:
-        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded, is_initialized)
+        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded)
 
         native_x, native_y, xvec, yvec = func(lon=lon, lat=lat, x=x, y=y)
         assert native_x == "lon"
         assert native_y == "lat"
         assert np.all(xvec == np.array([0.0]))
         assert np.all(yvec == np.array([2.0]))
 
 
 def test_lon_lat_array():
     x, y = None, None
     lon, lat = np.array([0.0, 1.0, 2.0, 3.0]), np.array([2.0, 3.0, 4.0, 5.0])
-    is_initialized = True
 
     for is_gridded in [True, False]:
-        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded, is_initialized)
+        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded)
 
         native_x, native_y, xvec, yvec = func(lon=lon, lat=lat, x=x, y=y)
         assert native_x == "lon"
         assert native_y == "lat"
         assert np.all(xvec == np.array([0.0, 1.0, 2.0, 3.0]))
         assert np.all(yvec == np.array([2.0, 3.0, 4.0, 5.0]))
 
 
 def test_lon_lat_int_array():
     x, y = None, None
     lon, lat = np.array([0, 1, 2, 3]), np.array([2, 3, 4, 5])
-    is_initialized = True
 
     for is_gridded in [True, False]:
-        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded, is_initialized)
+        x, y, lon, lat, __ = sanitize_input(x, y, lon, lat, is_gridded)
 
         native_x, native_y, xvec, yvec = func(lon=lon, lat=lat, x=x, y=y)
         assert native_x == "lon"
         assert native_y == "lat"
         assert np.all(xvec == np.array([0, 1, 2, 3]))
         assert np.all(yvec == np.array([2, 3, 4, 5]))
```

### Comparing `geo_skeletons-0.9.8/tests/test_yank_point_cartesian_gridded.py` & `geo_skeletons-0.9.9/tests/test_yank_point_cartesian_gridded.py`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/tests/test_yank_point_cartesian_point.py` & `geo_skeletons-0.9.9/tests/test_yank_point_cartesian_point.py`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/tests/test_yank_point_spherical_gridded.py` & `geo_skeletons-0.9.9/tests/test_yank_point_spherical_gridded.py`

 * *Files identical despite different names*

### Comparing `geo_skeletons-0.9.8/tests/test_yank_point_spherical_point.py` & `geo_skeletons-0.9.9/tests/test_yank_point_spherical_point.py`

 * *Files identical despite different names*

