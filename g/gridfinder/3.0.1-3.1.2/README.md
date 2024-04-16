# Comparing `tmp/gridfinder-3.0.1.tar.gz` & `tmp/gridfinder-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridfinder-3.0.1.tar", last modified: Tue Mar  5 08:44:39 2024, max compression
+gzip compressed data, was "gridfinder-3.1.2.tar", last modified: Tue Apr 16 17:12:47 2024, max compression
```

## Comparing `gridfinder-3.0.1.tar` & `gridfinder-3.1.2.tar`

### file list

```diff
@@ -1,27 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 08:44:39.866072 gridfinder-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-05 08:44:30.000000 gridfinder-3.0.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 08:44:39.862072 gridfinder-3.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 08:44:39.862072 gridfinder-3.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-05 08:44:30.000000 gridfinder-3.0.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-05 08:44:30.000000 gridfinder-3.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-05 08:44:30.000000 gridfinder-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-05 08:44:30.000000 gridfinder-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-05 08:44:30.000000 gridfinder-3.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-03-05 08:44:39.866072 gridfinder-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-03-05 08:44:30.000000 gridfinder-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 08:44:39.866072 gridfinder-3.0.1/gridfinder/
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-03-05 08:44:30.000000 gridfinder-3.0.1/gridfinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-03-05 08:44:30.000000 gridfinder-3.0.1/gridfinder/gridfinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-03-05 08:44:30.000000 gridfinder-3.0.1/gridfinder/post.py
--rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-03-05 08:44:30.000000 gridfinder-3.0.1/gridfinder/prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 08:44:30.000000 gridfinder-3.0.1/gridfinder/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-03-05 08:44:30.000000 gridfinder-3.0.1/gridfinder/util.py
--rw-r--r--   0 runner    (1001) docker     (127)   684229 2024-03-05 08:44:30.000000 gridfinder-3.0.1/gridfinder-animated.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 08:44:39.866072 gridfinder-3.0.1/gridfinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-03-05 08:44:39.000000 gridfinder-3.0.1/gridfinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-05 08:44:39.000000 gridfinder-3.0.1/gridfinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 08:44:39.000000 gridfinder-3.0.1/gridfinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-05 08:44:39.000000 gridfinder-3.0.1/gridfinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-05 08:44:39.000000 gridfinder-3.0.1/gridfinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-03-05 08:44:30.000000 gridfinder-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 08:44:39.866072 gridfinder-3.0.1/setup.cfg
+-rw-r--r--   0        0        0     1070 2024-04-16 17:12:44.782351 gridfinder-3.1.2/LICENSE
+-rw-r--r--   0        0        0     1866 2024-04-16 17:12:44.782351 gridfinder-3.1.2/README.md
+-rw-r--r--   0        0        0      821 2024-04-16 17:12:44.842350 gridfinder-3.1.2/gridfinder/__init__.py
+-rw-r--r--   0        0        0     4755 2024-04-16 17:12:44.842350 gridfinder-3.1.2/gridfinder/gridfinder.py
+-rw-r--r--   0        0        0     7768 2024-04-16 17:12:44.842350 gridfinder-3.1.2/gridfinder/post.py
+-rw-r--r--   0        0        0    10313 2024-04-16 17:12:44.842350 gridfinder-3.1.2/gridfinder/prepare.py
+-rw-r--r--   0        0        0        0 2024-04-16 17:12:44.842350 gridfinder-3.1.2/gridfinder/py.typed
+-rw-r--r--   0        0        0     2128 2024-04-16 17:12:44.842350 gridfinder-3.1.2/gridfinder/util.py
+-rw-r--r--   0        0        0     2200 2024-04-16 17:12:47.938325 gridfinder-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0      853 2024-04-16 17:12:44.842350 gridfinder-3.1.2/tests/conftest.py
+-rw-r--r--   0        0        0   334514 2024-04-16 17:12:44.842350 gridfinder-3.1.2/tests/data/aoi.geojson
+-rw-r--r--   0        0        0  1854698 2024-04-16 17:12:44.846350 gridfinder-3.1.2/tests/data/costs.tif
+-rw-r--r--   0        0        0  1854698 2024-04-16 17:12:44.858350 gridfinder-3.1.2/tests/data/dist.tif
+-rw-r--r--   0        0        0    30838 2024-04-16 17:12:44.858350 gridfinder-3.1.2/tests/data/grid.geojson
+-rw-r--r--   0        0        0  1854698 2024-04-16 17:12:44.858350 gridfinder-3.1.2/tests/data/guess.tif
+-rw-r--r--   0        0        0  1853139 2024-04-16 17:12:44.866350 gridfinder-3.1.2/tests/data/ntl.tif
+-rw-r--r--   0        0        0  3166410 2024-04-16 17:12:44.874350 gridfinder-3.1.2/tests/data/pop.tif
+-rw-r--r--   0        0        0 22881603 2024-04-16 17:12:44.954349 gridfinder-3.1.2/tests/data/roads.geojson
+-rw-r--r--   0        0        0  1854698 2024-04-16 17:12:44.958349 gridfinder-3.1.2/tests/data/targets.tif
+-rw-r--r--   0        0        0  1854698 2024-04-16 17:12:44.958349 gridfinder-3.1.2/tests/data/targets_clean.tif
+-rw-r--r--   0        0        0  1854698 2024-04-16 17:12:44.962349 gridfinder-3.1.2/tests/data/thin.tif
+-rw-r--r--   0        0        0      389 2024-04-16 17:12:44.962349 gridfinder-3.1.2/tests/test_gridfinder.py
+-rw-r--r--   0        0        0      622 2024-04-16 17:12:44.962349 gridfinder-3.1.2/tests/test_post.py
+-rw-r--r--   0        0        0     1128 2024-04-16 17:12:44.962349 gridfinder-3.1.2/tests/test_prepare.py
+-rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 gridfinder-3.1.2/PKG-INFO
```

### Comparing `gridfinder-3.0.1/LICENSE` & `gridfinder-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gridfinder-3.0.1/PKG-INFO` & `gridfinder-3.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: gridfinder
-Version: 3.0.1
+Version: 3.1.2
 Summary: Algorithm for guessing MV grid network based on night time lights
-Author-email: Chris Arderne <chris@rdrn.me>
-License: MIT License
-Project-URL: homepage, https://gridfinder.rdrn.me
-Project-URL: repository, https://github.com/carderne/gridfinder
 Keywords: ntl,electricity,grid
+Home-page: https://gridfinder.rdrn.me
+Author-Email: Chris Arderne <chris@rdrn.me>
+License: MIT License
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Project-URL: Homepage, https://gridfinder.rdrn.me
+Project-URL: Repository, https://github.com/carderne/gridfinder
 Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: affine~=2.4
 Requires-Dist: click~=8.0
 Requires-Dist: fiona~=1.9
 Requires-Dist: geopandas~=0.14
 Requires-Dist: numba~=0.58
 Requires-Dist: numpy~=1.26
 Requires-Dist: pandas~=2.2
@@ -29,21 +28,15 @@
 Requires-Dist: pyarrow~=15.0
 Requires-Dist: pyproj~=3.6
 Requires-Dist: rasterio~=1.3
 Requires-Dist: Rtree~=1.2
 Requires-Dist: scikit-image~=0.22
 Requires-Dist: scipy~=1.12
 Requires-Dist: Shapely~=2.0
-Provides-Extra: dev
-Requires-Dist: descartes~=1.1.0; extra == "dev"
-Requires-Dist: folium~=0.15; extra == "dev"
-Requires-Dist: matplotlib~=3.8; extra == "dev"
-Requires-Dist: pytest~=8.0; extra == "dev"
-Requires-Dist: ruff~=0.2; extra == "dev"
-Requires-Dist: seaborn~=0.13; extra == "dev"
+Description-Content-Type: text/markdown
 
 # gridfinder
 
 gridfinder uses night-time lights imagery to as an indicator of settlements/towns with grid electricity access. Then a minimum spanning tree is calculated for these connect points, using a many-to-many variant Dijkstra algorithm and using existing road networks as a cost function. Adapted from [this work from Facebook](https://github.com/facebookresearch/many-to-many-dijkstra). Currently gridfinder only uses road networks, but it would be trivial to add other cost parameters such as slope or terrain.
 
 The algorithm looks as follows in process, guessing the grid network for Uganda:
 
@@ -71,24 +64,17 @@
 ```
 
 ## Development
 Download or clone the repository and install the required packages (preferably in a virtual environment):
 ```bash
 git clone https://github.com/carderne/gridfinder.git
 cd gridfinder
-pip install -e '.[dev]'
-```
-
-### Linting
-```bash
-make lint
-```
-
-### Typecheck
-```bash
-make check
+rye sync
 ```
 
-### Testing
+Useful commands:
 ```bash
-make test
+rye fmt
+rye lint
+rye run check  # type check
+rye run test
 ```
```

### Comparing `gridfinder-3.0.1/README.md` & `gridfinder-3.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -28,24 +28,17 @@
 ```
 
 ## Development
 Download or clone the repository and install the required packages (preferably in a virtual environment):
 ```bash
 git clone https://github.com/carderne/gridfinder.git
 cd gridfinder
-pip install -e '.[dev]'
+rye sync
 ```
 
-### Linting
+Useful commands:
 ```bash
-make lint
-```
-
-### Typecheck
-```bash
-make check
-```
-
-### Testing
-```bash
-make test
+rye fmt
+rye lint
+rye run check  # type check
+rye run test
 ```
```

### Comparing `gridfinder-3.0.1/gridfinder/__init__.py` & `gridfinder-3.1.2/gridfinder/__init__.py`

 * *Files identical despite different names*

### Comparing `gridfinder-3.0.1/gridfinder/gridfinder.py` & `gridfinder-3.1.2/gridfinder/gridfinder.py`

 * *Files identical despite different names*

### Comparing `gridfinder-3.0.1/gridfinder/post.py` & `gridfinder-3.1.2/gridfinder/post.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,14 @@
 
 def thin_arr(guess: np.ndarray) -> np.ndarray:
     guess_skel = skeletonize(guess)
     guess_skel = guess_skel.astype("int32")
     return guess_skel
 
 
-
 def raster_to_lines(guess_skel_in: Pathy) -> gpd.GeoDataFrame:
     """
     Convert thinned raster to linestring geometry.
 
     Parameters
     ----------
     guess_skel_in : Output from thin().
```

### Comparing `gridfinder-3.0.1/gridfinder/prepare.py` & `gridfinder-3.1.2/gridfinder/prepare.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import json
 import os
 from math import sqrt
 from pathlib import Path
 
-import fiona
 import geopandas as gpd
 import numpy as np
 import rasterio as rs
 from geopandas.geodataframe import GeoDataFrame
 from rasterio import Affine
 from rasterio.features import rasterize
 from rasterio.io import MemoryFile
@@ -117,92 +116,77 @@
 
 
 def prepare_ntl(
     ntl_in: Pathy,
     aoi_in: Pathy,
     ntl_filter: np.ndarray | None = None,
     threshold: float = 0.1,
-    upsample_by: int = 2,
 ) -> tuple[np.ndarray, Affine]:
     """Convert the supplied NTL raster and output an array of electrified cells
     as targets for the algorithm.
 
     Parameters
     ----------
     ntl_in : Path to an NTL raster file.
     aoi_in : Path to a Fiona-readable AOI file.
     ntl_filter : The filter will be convolved over the raster.
     threshold : The threshold to apply after filtering, values above
         are considered electrified.
-    upsample_by : The factor by which to upsample the input raster, applied to both axes
-        (so a value of 2 results in a raster 4 times bigger). This is to
-        allow the roads detail to be captured in higher resolution.
 
     Returns
     -------
     ntl_thresh : Array of cells of value 0 (not electrified) or 1 (electrified).
     newaff : Affine raster transformation for the returned array.
     """
 
     if isinstance(aoi_in, gpd.GeoDataFrame):
         aoi = aoi_in
     else:
         aoi = gpd.read_file(aoi_in)
 
+    aoi_buff = aoi.buffer(0.1)
+    coords = [json.loads(aoi.to_json())["features"][0]["geometry"]]
+    coords_buff = [json.loads(aoi_buff.to_json())["features"][0]["geometry"]]
+
     if ntl_filter is None:
         ntl_filter = create_filter()
 
-    ntl_big = rs.open(ntl_in)
-
-    coords = [json.loads(aoi.to_json())["features"][0]["geometry"]]
-    ntl, affine = mask(dataset=ntl_big, shapes=coords, crop=True, nodata=0)
+    with rs.open(ntl_in) as ds:
+        ntl, affine = mask(dataset=ds, shapes=coords_buff, crop=True, nodata=0)
 
     if ntl.ndim == 3:
         ntl = ntl[0]
 
     ntl_convolved = signal.convolve2d(ntl, ntl_filter, mode="same")
     ntl_filtered = ntl - ntl_convolved
 
-    ntl_interp = np.empty(
-        shape=(
-            1,  # same number of bands
-            round(ntl.shape[0] * upsample_by),
-            round(ntl.shape[1] * upsample_by),
-        )
-    )
-
-    # adjust the new affine transform to the 150% smaller cell size
-    newaff = Affine(
-        affine.a / upsample_by,
-        affine.b,
-        affine.c,
-        affine.d,
-        affine.e / upsample_by,
-        affine.f,
-    )
-    with fiona.Env():
-        with rs.Env():
-            reproject(
-                ntl_filtered,
-                ntl_interp,
-                src_transform=affine,
-                dst_transform=newaff,
-                src_crs={"init": "epsg:4326"},
-                dst_crs={"init": "epsg:4326"},
-                resampling=Resampling.bilinear,
-            )
-
-    ntl_interp = ntl_interp[0]
-
-    ntl_thresh = np.empty_like(ntl_interp)
-    ntl_thresh[:] = ntl_interp[:]
+    ntl_thresh = np.empty_like(ntl_filtered)
+    ntl_thresh[:] = ntl_filtered[:]
     ntl_thresh[ntl_thresh < threshold] = 0
     ntl_thresh[ntl_thresh >= threshold] = 1
 
-    return ntl_thresh, newaff
+    with MemoryFile() as f:
+        with f.open(
+            transform=affine,
+            driver="GTiff",
+            height=ntl_thresh.shape[0],
+            width=ntl_thresh.shape[1],
+            count=1,
+            dtype=ntl_thresh.dtype,
+            crs=aoi.crs,
+            nodata=0,
+        ) as ds:
+            ds.write(ntl_thresh, 1)
+        with f.open() as ds:
+            clipped, affine = mask(dataset=ds, shapes=coords, crop=True, nodata=0)
+
+    if len(clipped.shape) >= 3:
+        clipped = clipped[0]
+
+    return clipped, affine
 
 
 def drop_zero_pop(
     targets_in: Pathy,
     pop_in: Pathy,
     aoi: GeoDataFrame,
 ) -> np.ndarray:
```

### Comparing `gridfinder-3.0.1/gridfinder/util.py` & `gridfinder-3.1.2/gridfinder/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,23 +73,20 @@
     Returns
     -------
     clipped : Contents of clipped raster.
     affine : The affine
     crs : form {'init': 'epsg:4326'}
     """
 
-    raster_ds = rs.open(raster)
-    raster_crs = raster_ds.crs
+    with rs.open(raster) as ds:
+        raster_crs = ds.crs
+        if not (boundary.crs == raster_crs or boundary.crs == raster_crs.data):
+            boundary = boundary.to_crs(crs=raster_crs)  # type: ignore
+        coords = [json.loads(boundary.to_json())["features"][0]["geometry"]]
 
-    if not (boundary.crs == raster_crs or boundary.crs == raster_crs.data):
-        boundary = boundary.to_crs(crs=raster_crs)  # type: ignore
-    coords = [json.loads(boundary.to_json())["features"][0]["geometry"]]
-
-    # mask/clip the raster using rasterio.mask
-    clipped, affine = mask(dataset=raster_ds, shapes=coords, crop=True)
+        # mask/clip the raster using rasterio.mask
+        clipped, affine = mask(dataset=ds, shapes=coords, crop=True)
 
     if len(clipped.shape) >= 3:
         clipped = clipped[0]
 
-    raster_ds.close()
-
     return clipped, affine, raster_crs
```

