# Comparing `tmp/ssb_sgis-0.3.9.tar.gz` & `tmp/ssb_sgis-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_sgis-0.3.9.tar", max compression
+gzip compressed data, was "ssb_sgis-1.0.0.tar", max compression
```

## Comparing `ssb_sgis-0.3.9.tar` & `ssb_sgis-1.0.0.tar`

### file list

```diff
@@ -1,59 +1,63 @@
--rw-r--r--   0        0        0     1074 2023-12-15 08:19:01.042202 ssb_sgis-0.3.9/LICENSE
--rw-r--r--   0        0        0     7557 2023-12-15 08:19:01.042202 ssb_sgis-0.3.9/README.md
--rw-r--r--   0        0        0     2665 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     3601 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/__init__.py
--rw-r--r--   0        0        0      576 2023-12-15 08:19:01.070202 ssb_sgis-0.3.9/src/sgis/exceptions.py
--rw-r--r--   0        0        0        0 2023-12-15 08:19:01.070202 ssb_sgis-0.3.9/src/sgis/geopandas_tools/__init__.py
--rw-r--r--   0        0        0    17616 2023-12-15 08:19:01.070202 ssb_sgis-0.3.9/src/sgis/geopandas_tools/bounds.py
--rw-r--r--   0        0        0    12166 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/geopandas_tools/buffer_dissolve_explode.py
--rw-r--r--   0        0        0    14142 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/geopandas_tools/centerlines.py
--rw-r--r--   0        0        0    11548 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/geopandas_tools/cleaning.py
--rw-r--r--   0        0        0    17242 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/geopandas_tools/conversion.py
--rw-r--r--   0        0        0    10422 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/geopandas_tools/duplicates.py
--rw-r--r--   0        0        0    18649 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/geopandas_tools/general.py
--rw-r--r--   0        0        0      691 2023-12-15 08:19:01.070202 ssb_sgis-0.3.9/src/sgis/geopandas_tools/geocoding.py
--rw-r--r--   0        0        0     7147 2023-12-15 08:19:01.070202 ssb_sgis-0.3.9/src/sgis/geopandas_tools/geometry_types.py
--rw-r--r--   0        0        0    15047 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/geopandas_tools/neighbors.py
--rw-r--r--   0        0        0    14693 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/geopandas_tools/overlay.py
--rw-r--r--   0        0        0     6897 2023-12-15 08:19:01.070202 ssb_sgis-0.3.9/src/sgis/geopandas_tools/point_operations.py
--rw-r--r--   0        0        0    35737 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/geopandas_tools/polygon_operations.py
--rw-r--r--   0        0        0    10276 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/geopandas_tools/polygons_as_rings.py
--rw-r--r--   0        0        0     8513 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/geopandas_tools/sfilter.py
--rw-r--r--   0        0        0     6066 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/helpers.py
--rw-r--r--   0        0        0      459 2023-12-15 08:19:01.070202 ssb_sgis-0.3.9/src/sgis/io/_is_dapla.py
--rw-r--r--   0        0        0     7622 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/io/dapla_functions.py
--rw-r--r--   0        0        0      538 2023-12-15 08:19:01.070202 ssb_sgis-0.3.9/src/sgis/io/opener.py
--rw-r--r--   0        0        0     3774 2023-12-15 08:19:01.070202 ssb_sgis-0.3.9/src/sgis/io/read_parquet.py
--rw-r--r--   0        0        0     6457 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/io/write_municipality_data.py
--rw-r--r--   0        0        0        0 2023-12-15 08:19:01.070202 ssb_sgis-0.3.9/src/sgis/maps/__init__.py
--rw-r--r--   0        0        0     8073 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/maps/examine.py
--rw-r--r--   0        0        0    27857 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/maps/explore.py
--rw-r--r--   0        0        0     1902 2023-12-15 08:19:01.070202 ssb_sgis-0.3.9/src/sgis/maps/httpserver.py
--rw-r--r--   0        0        0    20680 2023-12-15 08:19:01.070202 ssb_sgis-0.3.9/src/sgis/maps/legend.py
--rw-r--r--   0        0        0    22806 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/maps/map.py
--rw-r--r--   0        0        0    18197 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/maps/maps.py
--rw-r--r--   0        0        0    14132 2023-12-15 08:19:01.070202 ssb_sgis-0.3.9/src/sgis/maps/thematicmap.py
--rw-r--r--   0        0        0     2733 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/maps/tilesources.py
--rw-r--r--   0        0        0        0 2023-12-15 08:19:01.070202 ssb_sgis-0.3.9/src/sgis/networkanalysis/__init__.py
--rw-r--r--   0        0        0     6308 2023-12-15 08:19:01.070202 ssb_sgis-0.3.9/src/sgis/networkanalysis/_get_route.py
--rw-r--r--   0        0        0     2151 2023-12-15 08:19:01.070202 ssb_sgis-0.3.9/src/sgis/networkanalysis/_od_cost_matrix.py
--rw-r--r--   0        0        0     4206 2023-12-15 08:19:01.070202 ssb_sgis-0.3.9/src/sgis/networkanalysis/_points.py
--rw-r--r--   0        0        0     5336 2023-12-15 08:19:01.070202 ssb_sgis-0.3.9/src/sgis/networkanalysis/_service_area.py
--rw-r--r--   0        0        0    13329 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/networkanalysis/closing_network_holes.py
--rw-r--r--   0        0        0    14267 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/networkanalysis/cutting_lines.py
--rw-r--r--   0        0        0    11217 2023-12-15 08:19:01.070202 ssb_sgis-0.3.9/src/sgis/networkanalysis/directednetwork.py
--rw-r--r--   0        0        0     3370 2023-12-15 08:19:01.070202 ssb_sgis-0.3.9/src/sgis/networkanalysis/finding_isolated_networks.py
--rw-r--r--   0        0        0     7686 2023-12-15 08:19:01.074202 ssb_sgis-0.3.9/src/sgis/networkanalysis/network.py
--rw-r--r--   0        0        0    67276 2023-12-15 08:19:01.074202 ssb_sgis-0.3.9/src/sgis/networkanalysis/networkanalysis.py
--rw-r--r--   0        0        0    12607 2023-12-15 08:19:01.074202 ssb_sgis-0.3.9/src/sgis/networkanalysis/networkanalysisrules.py
--rw-r--r--   0        0        0     6844 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/networkanalysis/nodes.py
--rw-r--r--   0        0        0     5558 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/networkanalysis/traveling_salesman.py
--rw-r--r--   0        0        0    16050 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/parallel/parallel.py
--rw-r--r--   0        0        0        0 2023-12-15 08:19:01.074202 ssb_sgis-0.3.9/src/sgis/py.typed
--rw-r--r--   0        0        0        0 2023-12-15 08:19:01.074202 ssb_sgis-0.3.9/src/sgis/raster/__init__.py
--rw-r--r--   0        0        0     5385 2023-12-15 08:19:01.074202 ssb_sgis-0.3.9/src/sgis/raster/base.py
--rw-r--r--   0        0        0     2867 2023-12-15 08:19:01.074202 ssb_sgis-0.3.9/src/sgis/raster/elevationraster.py
--rw-r--r--   0        0        0    40862 2023-12-15 08:19:14.914248 ssb_sgis-0.3.9/src/sgis/raster/raster.py
--rw-r--r--   0        0        0     1025 2023-12-15 08:19:01.074202 ssb_sgis-0.3.9/src/sgis/raster/sentinel.py
--rw-r--r--   0        0        0     3249 2023-12-15 08:19:01.074202 ssb_sgis-0.3.9/src/sgis/raster/zonal.py
--rw-r--r--   0        0        0     9163 1970-01-01 00:00:00.000000 ssb_sgis-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-16 13:15:56.799067 ssb_sgis-1.0.0/LICENSE
+-rw-r--r--   0        0        0     7557 2024-04-16 13:15:56.799067 ssb_sgis-1.0.0/README.md
+-rw-r--r--   0        0        0     2734 2024-04-16 13:16:08.895226 ssb_sgis-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4018 2024-04-16 13:16:08.895226 ssb_sgis-1.0.0/src/sgis/__init__.py
+-rw-r--r--   0        0        0      576 2024-04-16 13:15:56.827067 ssb_sgis-1.0.0/src/sgis/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-16 13:15:56.827067 ssb_sgis-1.0.0/src/sgis/geopandas_tools/__init__.py
+-rw-r--r--   0        0        0    22565 2024-04-16 13:16:08.895226 ssb_sgis-1.0.0/src/sgis/geopandas_tools/bounds.py
+-rw-r--r--   0        0        0    17930 2024-04-16 13:16:08.895226 ssb_sgis-1.0.0/src/sgis/geopandas_tools/buffer_dissolve_explode.py
+-rw-r--r--   0        0        0    14142 2024-04-16 13:15:56.827067 ssb_sgis-1.0.0/src/sgis/geopandas_tools/centerlines.py
+-rw-r--r--   0        0        0    23889 2024-04-16 13:16:08.895226 ssb_sgis-1.0.0/src/sgis/geopandas_tools/cleaning.py
+-rw-r--r--   0        0        0    21903 2024-04-16 13:16:08.895226 ssb_sgis-1.0.0/src/sgis/geopandas_tools/conversion.py
+-rw-r--r--   0        0        0    13124 2024-04-16 13:16:08.895226 ssb_sgis-1.0.0/src/sgis/geopandas_tools/duplicates.py
+-rw-r--r--   0        0        0    24999 2024-04-16 13:16:08.895226 ssb_sgis-1.0.0/src/sgis/geopandas_tools/general.py
+-rw-r--r--   0        0        0      691 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/geopandas_tools/geocoding.py
+-rw-r--r--   0        0        0     7167 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/geopandas_tools/geometry_types.py
+-rw-r--r--   0        0        0    15895 2024-04-16 13:16:08.895226 ssb_sgis-1.0.0/src/sgis/geopandas_tools/neighbors.py
+-rw-r--r--   0        0        0    23426 2024-04-16 13:16:08.899226 ssb_sgis-1.0.0/src/sgis/geopandas_tools/overlay.py
+-rw-r--r--   0        0        0     6897 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/geopandas_tools/point_operations.py
+-rw-r--r--   0        0        0    36718 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/geopandas_tools/polygon_operations.py
+-rw-r--r--   0        0        0    11184 2024-04-16 13:16:08.899226 ssb_sgis-1.0.0/src/sgis/geopandas_tools/polygons_as_rings.py
+-rw-r--r--   0        0        0     8531 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/geopandas_tools/sfilter.py
+-rw-r--r--   0        0        0     6190 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/helpers.py
+-rw-r--r--   0        0        0      431 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/io/_is_dapla.py
+-rw-r--r--   0        0        0     7987 2024-04-16 13:16:08.899226 ssb_sgis-1.0.0/src/sgis/io/dapla_functions.py
+-rw-r--r--   0        0        0      610 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/io/opener.py
+-rw-r--r--   0        0        0     3774 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/io/read_parquet.py
+-rw-r--r--   0        0        0        0 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/maps/__init__.py
+-rw-r--r--   0        0        0     8110 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/maps/examine.py
+-rw-r--r--   0        0        0    30785 2024-04-16 13:16:08.899226 ssb_sgis-1.0.0/src/sgis/maps/explore.py
+-rw-r--r--   0        0        0     1902 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/maps/httpserver.py
+-rw-r--r--   0        0        0    20680 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/maps/legend.py
+-rw-r--r--   0        0        0    23688 2024-04-16 13:16:08.899226 ssb_sgis-1.0.0/src/sgis/maps/map.py
+-rw-r--r--   0        0        0    20331 2024-04-16 13:16:08.899226 ssb_sgis-1.0.0/src/sgis/maps/maps.py
+-rw-r--r--   0        0        0    14132 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/maps/thematicmap.py
+-rw-r--r--   0        0        0     2733 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/maps/tilesources.py
+-rw-r--r--   0        0        0        0 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/networkanalysis/__init__.py
+-rw-r--r--   0        0        0     6308 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/networkanalysis/_get_route.py
+-rw-r--r--   0        0        0     2151 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/networkanalysis/_od_cost_matrix.py
+-rw-r--r--   0        0        0     4206 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/networkanalysis/_points.py
+-rw-r--r--   0        0        0     5336 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/networkanalysis/_service_area.py
+-rw-r--r--   0        0        0    13329 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/networkanalysis/closing_network_holes.py
+-rw-r--r--   0        0        0    14267 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/networkanalysis/cutting_lines.py
+-rw-r--r--   0        0        0    11217 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/networkanalysis/directednetwork.py
+-rw-r--r--   0        0        0     3370 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/networkanalysis/finding_isolated_networks.py
+-rw-r--r--   0        0        0     7686 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/networkanalysis/network.py
+-rw-r--r--   0        0        0    67276 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/networkanalysis/networkanalysis.py
+-rw-r--r--   0        0        0    12607 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/networkanalysis/networkanalysisrules.py
+-rw-r--r--   0        0        0     6844 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/networkanalysis/nodes.py
+-rw-r--r--   0        0        0     5558 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/networkanalysis/traveling_salesman.py
+-rw-r--r--   0        0        0    26997 2024-04-16 13:16:08.899226 ssb_sgis-1.0.0/src/sgis/parallel/parallel.py
+-rw-r--r--   0        0        0        0 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/py.typed
+-rw-r--r--   0        0        0        0 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/raster/__init__.py
+-rw-r--r--   0        0        0     1015 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/raster/bands.py
+-rw-r--r--   0        0        0      942 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/raster/base.py
+-rw-r--r--   0        0        0    34854 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/raster/cube.py
+-rw-r--r--   0        0        0      735 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/raster/cubebase.py
+-rw-r--r--   0        0        0     2352 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/raster/gradient.py
+-rw-r--r--   0        0        0     2782 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/raster/indices.py
+-rw-r--r--   0        0        0     2789 2024-04-16 13:15:56.831068 ssb_sgis-1.0.0/src/sgis/raster/methods_as_functions.py
+-rw-r--r--   0        0        0    45375 2024-04-16 13:15:56.835068 ssb_sgis-1.0.0/src/sgis/raster/raster.py
+-rw-r--r--   0        0        0     3898 2024-04-16 13:16:08.899226 ssb_sgis-1.0.0/src/sgis/raster/torchgeo.py
+-rw-r--r--   0        0        0     3259 2024-04-16 13:15:56.835068 ssb_sgis-1.0.0/src/sgis/raster/zonal.py
+-rw-r--r--   0        0        0     9068 1970-01-01 00:00:00.000000 ssb_sgis-1.0.0/PKG-INFO
```

### Comparing `ssb_sgis-0.3.9/LICENSE` & `ssb_sgis-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/README.md` & `ssb_sgis-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/pyproject.toml` & `ssb_sgis-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "ssb-sgis"
-version = "0.3.9"
+version = "1.0.0"
 description = "GIS functions used at Statistics Norway."
 authors = ["Statistics Norway <ort@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "sgis", from = "src"}]
 homepage = "https://github.com/statisticsnorway/ssb-sgis"
 repository = "https://github.com/statisticsnorway/ssb-sgis"
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 5 - Production/Stable",
     "Topic :: Scientific/Engineering :: GIS",
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/statisticsnorway/ssb-sgis/releases"
 
 [tool.poetry.dependencies]
@@ -22,35 +22,36 @@
 folium = ">=0.14.0"
 geopandas = "0.14.0"
 igraph = "0.11.2"
 mapclassify = ">=2.5.0"
 matplotlib = ">=3.7.0"
 networkx = ">=3.0"
 numpy = ">=1.24.2"
-pandas = ">=1.5.3"
+pandas = "2.0.3"
 pyarrow = ">=11.0.0"
 requests = ">=2.28.2"
 scikit-learn = ">=1.2.1"
 shapely = ">=2.0.1"
 xyzservices = ">=2023.2.0"
 jenkspy = ">=0.3.2"
 ipython = ">=8.13.2"
-rtree = "^1.0.1"
-geocoder = "^1.38.1"
-rasterio = "^1.3.8"
-xarray = "2023.8.0"
-rioxarray = "^0.14.1"
-numba = "^0.57.1"
+rtree = ">=1.0.1"
+geocoder = ">=1.38.1"
+rasterio = ">=1.3.8"
 pip = "23.2.1"
+dask = ">=2024.1.1"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["d", "jupyter"], version = ">=23.1.0"}
 coverage = {extras = ["toml"], version = ">=7.2.1"}
 darglint = ">=1.8.1"
 deptry = ">=0.8.0"
+numba = "^0.57.1"
+xarray = "2023.8.0"
+rioxarray = "^0.14.1"
 flake8 = ">=6.0.0"
 flake8-bandit = ">=4.1.1"
 flake8-bugbear = ">=23.2.13"
 flake8-docstrings = ">=1.7.0"
 flake8-rst-docstrings = ">=0.3.0"
 furo = ">=2023.3.27"
 isort = ">=5.12.0"
@@ -65,14 +66,16 @@
 pytest = ">=7.2.1"
 pytest-cov = ">=4.0.0"
 pytest-mock = ">=3.10.0"
 pyupgrade = ">=3.3.1"
 sphinx = ">=6.1.3"
 sphinx-autobuild = ">=2021.3.14"
 sphinx-autodoc-typehints = ">=1.22"
+torch = ">=2.2.2"
+torchgeo = ">=0.5.2"
 xdoctest = {extras = ["colors"], version = ">=1.1.1"}
 
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
@@ -93,14 +96,14 @@
 
 [tool.jupytext]
 formats = "ipynb,auto:percent"
 notebook_metadata_filter = "jupytext.text_representation,-jupytext.text_representation.jupytext_version,-widgets,-varInspector,-kernelspec"
 cell_metadata_filter = "-all"
 
 [tool.pytest.ini_options]
-  pythonpath = [
-   "src"
+pythonpath = [
+  "src"
 ]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ssb_sgis-0.3.9/src/sgis/__init__.py` & `ssb_sgis-1.0.0/src/sgis/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,49 @@
+config = {
+    "n_jobs": 1,
+}
+
+import sgis.raster.bands as bands
+import sgis.raster.indices as indices
+from sgis.raster.raster import Raster, get_shape_from_bounds, get_transform_from_bounds
+
 from .geopandas_tools.bounds import (
+    Gridlooper,
     bounds_to_points,
     bounds_to_polygon,
     get_total_bounds,
     gridloop,
     make_grid,
     make_grid_from_bbox,
     make_ssb_grid,
     points_in_bounds,
-    to_bbox,
 )
 from .geopandas_tools.buffer_dissolve_explode import (
     buff,
     buffdiss,
     buffdissexp,
     buffdissexp_by_cluster,
+    diss,
+    diss_by_cluster,
     dissexp,
     dissexp_by_cluster,
 )
 from .geopandas_tools.centerlines import get_rough_centerlines
-from .geopandas_tools.cleaning import coverage_clean, remove_spikes
+from .geopandas_tools.cleaning import (
+    coverage_clean,
+    remove_interior_slivers,
+    remove_spikes,
+    split_and_eliminate_by_longest,
+    split_by_neighbors,
+)
 from .geopandas_tools.conversion import (
     coordinate_array,
-    get_lonlat,
-    get_utm33,
+    from_4326,
+    to_4326,
+    to_bbox,
     to_gdf,
     to_geoseries,
     to_shapely,
 )
 from .geopandas_tools.duplicates import (  # drop_duplicate_geometries,
     get_intersections,
     update_geometries,
@@ -34,17 +51,20 @@
 from .geopandas_tools.general import (
     clean_clip,
     clean_geoms,
     drop_inactive_geometry_columns,
     get_common_crs,
     get_grouped_centroids,
     random_points,
+    random_points_in_polygons,
     rename_geometry_if,
     sort_large_first,
     sort_long_first,
+    sort_short_first,
+    sort_small_first,
     to_lines,
 )
 from .geopandas_tools.geocoding import address_to_coords, address_to_gdf
 from .geopandas_tools.geometry_types import (
     get_geom_type,
     is_single_geom_type,
     make_all_singlepart,
@@ -52,24 +72,27 @@
 )
 from .geopandas_tools.neighbors import (
     get_all_distances,
     get_k_nearest_neighbors,
     get_neighbor_dfs,
     get_neighbor_indices,
     k_nearest_neighbors,
+    sjoin_within_distance,
 )
 from .geopandas_tools.overlay import clean_overlay
 from .geopandas_tools.point_operations import snap_all, snap_within_distance
 from .geopandas_tools.polygon_operations import (
     PolygonsAsRings,
     close_all_holes,
     close_small_holes,
+    close_thin_holes,
     eliminate_by_largest,
     eliminate_by_longest,
     eliminate_by_smallest,
+    get_cluster_mapper,
     get_gaps,
     get_holes,
     get_polygon_clusters,
 )
 from .geopandas_tools.polygons_as_rings import PolygonsAsRings
 from .geopandas_tools.sfilter import sfilter, sfilter_inverse, sfilter_split
 from .helpers import get_object_name, sort_nans_last
@@ -105,18 +128,21 @@
 from .networkanalysis.networkanalysisrules import NetworkAnalysisRules
 from .networkanalysis.nodes import (
     make_edge_coords_cols,
     make_edge_wkt_cols,
     make_node_ids,
 )
 from .networkanalysis.traveling_salesman import traveling_salesman_problem
-from .parallel.parallel import Parallel
-from .raster.elevationraster import ElevationRaster
-from .raster.raster import Raster
-from .raster.sentinel import Sentinel2
+from .parallel.parallel import Parallel, parallel_overlay
+from .raster.cube import DataCube
+
+
+try:
+    import sgis.raster.torchgeo as torchgeo
+except ImportError:
+    pass
 
 
 try:
-    from .io.dapla_functions import check_files, exists, read_geopandas, write_geopandas
-    from .io.write_municipality_data import write_municipality_data
+    from .io.dapla_functions import check_files, read_geopandas, write_geopandas
 except ImportError:
     pass
```

### Comparing `ssb_sgis-0.3.9/src/sgis/exceptions.py` & `ssb_sgis-1.0.0/src/sgis/exceptions.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/src/sgis/geopandas_tools/bounds.py` & `ssb_sgis-1.0.0/src/sgis/geopandas_tools/bounds.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,185 @@
+import functools
 import numbers
-from typing import Any
 from collections.abc import Callable, Collection, Mapping
+from dataclasses import dataclass
+from typing import Any
 
 import geopandas as gpd
 import numpy as np
+import pandas as pd
 from geopandas import GeoDataFrame, GeoSeries
 from pandas.api.types import is_dict_like
 from shapely import Geometry, box, extract_unique_points
 from shapely.geometry import Polygon
 
-from .conversion import to_gdf
+from ..parallel.parallel import Parallel
+from .conversion import to_bbox, to_gdf
 from .general import clean_clip, is_bbox_like
 
 
+@dataclass
+class Gridlooper:
+    """Run functions in a loop cellwise based on a grid.
+
+    Args:
+        gridsize: Size of the grid cells in units of the crs (meters, degrees).
+        mask: Geometry object to create a grid around.
+        gridbuffer: Units to buffer each gridcell by. For edge cases.
+            Defaults to 0.
+        clip: If True (default) geometries are clipped by the grid cells.
+            If False, all geometries that intersect will be selected in each iteration.
+        verbose: Whether to print progress. Defaults to False.
+        keep_geom_type: Whether to keep only the input geometry types after clipping.
+            Defaults to True.
+
+    Examples
+    --------
+
+    Get some points and some polygons.
+
+    >>> import sgis as sg
+    >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
+    >>> points["idx"] = points.index
+    >>> buffered = sg.buff(points, 100)
+    >>> buffered
+        idx                                           geometry
+    0      0  POLYGON ((263222.700 6651184.900, 263222.651 6...
+    1      1  POLYGON ((272556.100 6653369.500, 272556.051 6...
+    2      2  POLYGON ((270182.300 6653032.700, 270182.251 6...
+    3      3  POLYGON ((259904.800 6650339.700, 259904.751 6...
+    4      4  POLYGON ((272976.200 6652889.100, 272976.151 6...
+    ..   ...                                                ...
+    995  995  POLYGON ((266901.700 6647844.500, 266901.651 6...
+    996  996  POLYGON ((261374.000 6653593.400, 261373.951 6...
+    997  997  POLYGON ((263642.900 6645427.000, 263642.851 6...
+    998  998  POLYGON ((269326.700 6650628.000, 269326.651 6...
+    999  999  POLYGON ((264670.300 6644239.500, 264670.251 6...
+
+    [1000 rows x 2 columns]
+
+    Instantiate a gridlooper.
+
+    >>> looper = sg.Gridlooper(gridsize=200, mask=buffered, concat=True, parallelizer=sg.Parallel(1, backend="multiprocessing"))
+
+    Run the function clean_overlay in a gridloop.
+
+    >>> results = looper.run(
+    ...     sg.clean_overlay,
+    ...     points,
+    ...     buffered,
+    ... )
+    >>> results
+        idx_1 idx_2                        geometry
+    0      220   220  POINT (254575.200 6661631.500)
+    1      735   735  POINT (256337.400 6649931.700)
+    2      575   575  POINT (256369.200 6650413.300)
+    3       39    39  POINT (256142.300 6650526.300)
+    4      235   235  POINT (256231.300 6650720.200)
+    ...    ...   ...                             ...
+    1481   711   795  POINT (272845.500 6655048.800)
+    1482   711   711  POINT (272845.500 6655048.800)
+    1483   757   757  POINT (273507.600 6652806.600)
+    1484   457   457  POINT (273524.400 6652979.900)
+    1485   284   284  POINT (273650.800 6653000.500)
+
+    [1486 rows x 3 columns]
+
+    """
+
+    gridsize: int
+    mask: GeoDataFrame | GeoSeries | Geometry
+    gridbuffer: int = 0
+    parallelizer: Parallel | None = None
+    concat: bool = False
+    clip: bool = True
+    keep_geom_type: bool = True
+    verbose: bool = False
+
+    def __post_init__(self):
+        if not isinstance(self.mask, GeoDataFrame):
+            self.mask = to_gdf(self.mask)
+
+    def run(self, func: Callable, *args, **kwargs):
+        def intersects_mask(df):
+            return df.index.isin(df.sjoin(self.mask).index)
+
+        grid: GeoSeries = (
+            make_grid(self.mask, gridsize=self.gridsize).loc[intersects_mask].geometry
+        )
+
+        n = len(grid)
+
+        buffered_grid = grid.buffer(self.gridbuffer, resolution=1, join_style=2)
+
+        if self.parallelizer is not None:
+            func_with_clip = functools.partial(
+                _clip_and_run_func,
+                func=func,
+                args=args,
+                kwargs=kwargs,
+                keep_geom_type=self.keep_geom_type,
+                clip=self.clip,
+            )
+            results = self.parallelizer.map(func_with_clip, buffered_grid)
+            if not self.gridbuffer or not self.clip:
+                return (
+                    results
+                    if not self.concat
+                    else pd.concat(results, ignore_index=True)
+                )
+            out = []
+            for cell_res, unbuffered in zip(results, grid, strict=True):
+                out.append(
+                    _clip_back_to_unbuffered_grid(
+                        cell_res, unbuffered, self.keep_geom_type
+                    )
+                )
+            return out if not self.concat else pd.concat(out, ignore_index=True)
+
+        results = []
+        for i, (unbuffered, buffered) in enumerate(zip(grid, buffered_grid)):
+            cell_kwargs = {
+                key: _clip_if_isinstance(
+                    value, buffered, self.keep_geom_type, self.clip
+                )
+                for key, value in kwargs.items()
+            }
+            cell_args = tuple(
+                _clip_if_isinstance(value, buffered, self.keep_geom_type, self.clip)
+                for value in args
+            )
+
+            cell_res = func(*cell_args, **cell_kwargs)
+
+            # clip back to original
+            if self.gridbuffer and self.clip:
+                cell_res = _clip_back_to_unbuffered_grid(
+                    cell_res, unbuffered, self.keep_geom_type
+                )
+
+            results.append(cell_res)
+
+            if self.verbose:
+                print(f"Done with {i+1} of {n} grid cells", end="\r")
+
+        return results if not self.concat else pd.concat(results, ignore_index=True)
+
+
 def gridloop(
     func: Callable,
-    mask: GeoDataFrame | GeoSeries | Geometry,
     gridsize: int,
+    mask: GeoDataFrame | GeoSeries | Geometry,
     gridbuffer: int = 0,
     clip: bool = True,
     keep_geom_type: bool = True,
     verbose: bool = False,
     args: tuple | None = None,
     kwargs: dict | None = None,
+    parallelizer: Parallel | None = None,
 ) -> list[Any]:
     """Runs a function in a loop cellwise based on a grid.
 
     Creates grid from a mask, and runs the function for each cell
     with all GeoDataFrame keyword arguments clipped to the cell
     extent.
 
@@ -104,79 +257,129 @@
     1483   757   757  POINT (273507.600 6652806.600)
     1484   457   457  POINT (273524.400 6652979.900)
     1485   284   284  POINT (273650.800 6653000.500)
 
     [1486 rows x 3 columns]
 
     """
-    if not isinstance(mask, GeoDataFrame):
-        mask = to_gdf(mask)
-
     if kwargs is None:
         kwargs = {}
     elif not isinstance(kwargs, dict):
         raise TypeError("kwargs should be a dict")
 
     if args is None:
         args = ()
     elif not isinstance(args, tuple):
         raise TypeError("args should be a tuple")
 
+    if not isinstance(mask, GeoDataFrame):
+        mask = to_gdf(mask)
+
     intersects_mask = lambda df: df.index.isin(df.sjoin(mask).index)
     grid: GeoSeries = make_grid(mask, gridsize=gridsize).loc[intersects_mask].geometry
 
-    if verbose:
-        n = len(grid)
-
-    def clip_if_isinstance(value, cell, keep_geom_type):
-        if not isinstance(value, (gpd.GeoDataFrame, gpd.GeoSeries, Geometry)):
-            return value
-
-        if isinstance(value, (gpd.GeoDataFrame, gpd.GeoSeries)):
-            if clip:
-                return clean_clip(value, cell, keep_geom_type=keep_geom_type)
-            return value.loc[value.intersects(cell)]
+    n = len(grid)
 
-        return value.intersection(cell).make_valid()
+    buffered_grid = grid.buffer(gridbuffer, resolution=1, join_style=2)
 
-    buffered = grid.buffer(gridbuffer, resolution=1, join_style=2)
+    if parallelizer is not None:
+        func_with_clip = functools.partial(
+            _clip_and_run_func,
+            func=func,
+            args=args,
+            kwargs=kwargs,
+            keep_geom_type=keep_geom_type,
+            clip=clip,
+        )
+        results = parallelizer.map(func_with_clip, buffered_grid)
+        if not gridbuffer or not clip:
+            return results
+        out = []
+        for cell_res, unbuffered in zip(results, grid, strict=True):
+            out.append(
+                _clip_back_to_unbuffered_grid(cell_res, unbuffered, keep_geom_type)
+            )
+        return out
 
     results = []
-    for i, (cell, buffered) in enumerate(zip(grid, buffered)):
-        cell_kwargs = {}
-        for key, value in kwargs.items():
-            value = clip_if_isinstance(value, buffered, keep_geom_type)
-            cell_kwargs[key] = value
-
-        cell_args = ()
-        for arg in args:
-            arg = clip_if_isinstance(arg, buffered, keep_geom_type)
-            cell_args = cell_args + (arg,)
+    for i, (unbuffered, buffered) in enumerate(zip(grid, buffered_grid)):
+        cell_kwargs = {
+            key: _clip_if_isinstance(value, buffered, keep_geom_type, clip)
+            for key, value in kwargs.items()
+        }
+        cell_args = tuple(
+            _clip_if_isinstance(value, buffered, keep_geom_type, clip) for value in args
+        )
 
         cell_res = func(*cell_args, **cell_kwargs)
 
         # clip back to original
         if gridbuffer and clip:
-            if isinstance(cell_res, (gpd.GeoDataFrame, gpd.GeoSeries, Geometry)):
-                cell_res = clip_if_isinstance(cell_res, cell, keep_geom_type)
-            else:
-                try:
-                    for res in cell_res:
-                        res = clip_if_isinstance(res, cell, keep_geom_type)
-                except TypeError:
-                    pass
+            cell_res = _clip_back_to_unbuffered_grid(
+                cell_res, unbuffered, keep_geom_type
+            )
 
         results.append(cell_res)
 
         if verbose:
             print(f"Done with {i+1} of {n} grid cells", end="\r")
 
     return results
 
 
+def _clip_and_run_func(
+    grid_cell: Polygon,
+    func: Callable,
+    args: tuple,
+    kwargs: dict,
+    keep_geom_type: bool,
+    clip: bool,
+):
+    cell_args = tuple(
+        _clip_if_isinstance(value, grid_cell, keep_geom_type, clip) for value in args
+    )
+    cell_kwargs = {
+        key: _clip_if_isinstance(value, grid_cell, keep_geom_type, clip)
+        for key, value in kwargs.items()
+    }
+
+    return func(*cell_args, **cell_kwargs)
+
+
+def _clip_if_isinstance(value, cell, keep_geom_type, clip: bool):
+    if not isinstance(value, (gpd.GeoDataFrame, gpd.GeoSeries, Geometry)):
+        return value
+
+    if isinstance(value, (gpd.GeoDataFrame, gpd.GeoSeries)):
+        if clip:
+            return clean_clip(value, cell, keep_geom_type=keep_geom_type)
+        return value.loc[value.intersects(cell)]
+
+    return value.intersection(cell).make_valid()
+
+
+def _clip_back_to_unbuffered_grid(results, mask, keep_geom_type):
+    if isinstance(results, (gpd.GeoDataFrame, gpd.GeoSeries, Geometry)):
+        return _clip_if_isinstance(results, mask, keep_geom_type, clip=True)
+    elif isinstance(results, (pd.DataFrame, pd.Series, np.ndarray)):
+        return results
+    try:
+        for key, value in results.items():
+            results[key] = _clip_if_isinstance(value, mask, keep_geom_type, clip=True)
+    except AttributeError:
+        try:
+            return [
+                _clip_if_isinstance(res, mask, keep_geom_type, clip=True)
+                for res in results
+            ]
+        except TypeError:
+            pass
+    return results
+
+
 def make_grid_from_bbox(
     minx: int | float,
     miny: int | float,
     maxx: int | float,
     maxy: int | float,
     *_,
     gridsize: int | float,
@@ -435,82 +638,23 @@
     as_bounds = bounds_to_polygon(gdf, copy=copy)
     if isinstance(gdf, GeoSeries):
         return GeoSeries(extract_unique_points(as_bounds), index=gdf.index)
     gdf.geometry = extract_unique_points(as_bounds.geometry)
     return gdf
 
 
-def to_bbox(
-    obj: GeoDataFrame | GeoSeries | Geometry | Collection | Mapping,
-) -> tuple[float, float, float, float]:
-    """Returns 4-length tuple of bounds if possible, else raises ValueError.
-
-    Args:
-        obj: Object to be converted to bounding box. Can be geopandas or shapely
-            objects, iterables of exactly four numbers or dictionary like/class
-            with a the keys/attributes "minx", "miny", "maxx", "maxy" or
-            "xmin", "ymin", "xmax", "ymax".
-    """
-    if isinstance(obj, (GeoDataFrame, GeoSeries)):
-        return tuple(obj.total_bounds)
-    if isinstance(obj, Geometry):
-        return tuple(obj.bounds)
-    if (
-        hasattr(obj, "__iter__")
-        and len(obj) == 4
-        and all(isinstance(x, numbers.Number) for x in obj)
-    ):
-        return tuple(obj)
-
-    if is_dict_like(obj) and all(x in obj for x in ["minx", "miny", "maxx", "maxy"]):
-        try:
-            minx = np.min(obj["minx"])
-            miny = np.min(obj["miny"])
-            maxx = np.max(obj["maxx"])
-            maxy = np.max(obj["maxy"])
-        except TypeError:
-            minx = np.min(obj.minx)
-            miny = np.min(obj.miny)
-            maxx = np.max(obj.maxx)
-            maxy = np.max(obj.maxy)
-        return minx, miny, maxx, maxy
-    if is_dict_like(obj) and all(x in obj for x in ["xmin", "ymin", "xmax", "ymax"]):
-        try:
-            xmin = np.min(obj["xmin"])
-            ymin = np.min(obj["ymin"])
-            xmax = np.max(obj["xmax"])
-            ymax = np.max(obj["ymax"])
-        except TypeError:
-            xmin = np.min(obj.xmin)
-            ymin = np.min(obj.ymin)
-            xmax = np.max(obj.xmax)
-            ymax = np.max(obj.ymax)
-        return xmin, ymin, xmax, ymax
-    if is_dict_like(obj) and hasattr(obj, "geometry"):
-        try:
-            return tuple(GeoSeries(obj["geometry"]).total_bounds)
-        except Exception:
-            return tuple(GeoSeries(obj.geometry).total_bounds)
-    try:
-        of_length = f" of length {len(obj)}"
-    except TypeError:
-        of_length = ""
-    raise TypeError(f"Cannot convert type {obj.__class__.__name__}{of_length} to bbox")
-
-
 def get_total_bounds(
     *geometries: GeoDataFrame | GeoSeries | Geometry,
 ) -> tuple[float, float, float, float]:
     """Get a combined total bounds of multiple geometry objects."""
     xs, ys = [], []
     for obj in geometries:
         minx, miny, maxx, maxy = to_bbox(obj)
         xs += [minx, maxx]
         ys += [miny, maxy]
-
     return min(xs), min(ys), max(xs), max(ys)
 
 
 def points_in_bounds(gdf: GeoDataFrame | GeoSeries, n2: int):
     if not isinstance(gdf, (GeoDataFrame, GeoSeries)) and is_bbox_like(gdf):
         minx, miny, maxx, maxy = gdf
     else:
```

### Comparing `ssb_sgis-0.3.9/src/sgis/geopandas_tools/buffer_dissolve_explode.py` & `ssb_sgis-1.0.0/src/sgis/geopandas_tools/buffer_dissolve_explode.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 - If 'by' is not specified, the index will be labeled 0, 1, …, n - 1 after exploded, instead of 0, 0, …, 0 as it will with the geopandas defaults.
 
 - index_parts is set to False, which will be the default in a future version of geopandas.
 
 - The buff function returns a GeoDataFrame, the geopandas method returns a GeoSeries.
 """
 
+from typing import Callable
+
+import numpy as np
+import pandas as pd
 from geopandas import GeoDataFrame, GeoSeries
 
-from .general import _push_geom_col
+from .general import merge_geometries, parallel_unary_union
 from .geometry_types import make_all_singlepart
-from .polygon_operations import (
-    get_cluster_mapper,
-    get_grouped_centroids,
-    get_polygon_clusters,
-)
+from .polygon_operations import get_cluster_mapper, get_grouped_centroids
 
 
 def _decide_ignore_index(kwargs: dict) -> tuple[dict, bool]:
     if "ignore_index" in kwargs:
         ignore_index = kwargs.pop("ignore_index")
         return kwargs, ignore_index
 
@@ -42,14 +42,16 @@
 def buffdissexp(
     gdf: GeoDataFrame,
     distance: int | float,
     *,
     resolution: int = 50,
     index_parts: bool = False,
     copy: bool = True,
+    grid_size: float | int | None = None,
+    n_jobs: int = 1,
     **dissolve_kwargs,
 ) -> GeoDataFrame:
     """Buffers and dissolves overlapping geometries.
 
     It takes a GeoDataFrame and buffer, fixes, dissolves, fixes and explodes geometries.
     If the 'by' parameter is not specified, the index will labeled 0, 1, …, n - 1,
     instead of 0, 0, …, 0. If 'by' is speficied, this will be the index.
@@ -71,27 +73,30 @@
     dissolve_kwargs, ignore_index = _decide_ignore_index(dissolve_kwargs)
 
     dissolved = buffdiss(
         gdf,
         distance,
         resolution=resolution,
         copy=copy,
+        grid_size=grid_size,
+        n_jobs=n_jobs,
         **dissolve_kwargs,
     )
 
     return make_all_singlepart(
         dissolved, ignore_index=ignore_index, index_parts=index_parts
     )
 
 
 def buffdiss(
     gdf: GeoDataFrame,
     distance: int | float,
     resolution: int = 50,
     copy: bool = True,
+    n_jobs: int = 1,
     **dissolve_kwargs,
 ) -> GeoDataFrame:
     """Buffers and dissolves geometries.
 
     It takes a GeoDataFrame and buffer, fixes, dissolves and fixes geometries.
     If the 'by' parameter is not specified, the index will labeled 0, 1, …, n - 1,
     instead of 0, 0, …, 0. If 'by' is speficied, this will be the index.
@@ -155,27 +160,148 @@
       group                                           geometry    number
     0     a  MULTIPOLYGON (((258866.258 6648220.031, 258865...  0.323948
     1     b  MULTIPOLYGON (((258404.858 6647830.931, 258404...  0.687635
     2     d  MULTIPOLYGON (((258180.258 6647935.731, 258179...  0.580157
     """
     buffered = buff(gdf, distance, resolution=resolution, copy=copy)
 
-    dissolved = buffered.dissolve(**dissolve_kwargs)
+    return _dissolve(buffered, n_jobs=n_jobs, **dissolve_kwargs)
+
+
+def _dissolve(gdf, aggfunc="first", grid_size=None, n_jobs=1, **dissolve_kwargs):
+
+    if not len(gdf):
+        return gdf
+
+    geom_col = gdf._geometry_column_name
+
+    by = dissolve_kwargs.pop("by", None)
+
+    by_was_none = not bool(by)
+
+    if by is None and dissolve_kwargs.get("level") is None:
+        by = np.zeros(len(gdf), dtype="int64")
+        other_cols = list(gdf.columns.difference({geom_col}))
+    else:
+        if isinstance(by, str):
+            by = [by]
+        other_cols = list(gdf.columns.difference({geom_col} | set(by or {})))
+
+    try:
+        is_one_hit = gdf.groupby(by, **dissolve_kwargs).transform("size") == 1
+    except IndexError:
+        # if no rows when dropna=True
+        original_by = [x for x in by]
+        query = gdf[by.pop(0)].notna()
+        for col in gdf[by]:
+            query &= gdf[col].notna()
+        gdf = gdf.loc[query]
+        assert not len(gdf), gdf
+        if not by_was_none and dissolve_kwargs.get("as_index", True):
+            try:
+                gdf = gdf.set_index(original_by)
+            except Exception as e:
+                print(gdf)
+                print(original_by)
+                raise e
+        return gdf
+
+    if not by_was_none and dissolve_kwargs.get("as_index", True):
+        one_hit = gdf[is_one_hit].set_index(by)
+    else:
+        one_hit = gdf[is_one_hit]
+    many_hits = gdf[~is_one_hit]
+
+    if not len(many_hits):
+        return GeoDataFrame(one_hit, geometry=geom_col, crs=gdf.crs)
+
+    dissolved = many_hits.groupby(by, **dissolve_kwargs)[other_cols].agg(aggfunc)
+
+    # dissolved = gdf.groupby(by, **dissolve_kwargs)[other_cols].agg(aggfunc)
+
+    if n_jobs > 1:
+        try:
+            agged = parallel_unary_union(
+                many_hits, n_jobs=n_jobs, by=by, grid_size=grid_size, **dissolve_kwargs
+            )
+            dissolved[geom_col] = agged
+            return GeoDataFrame(dissolved, geometry=geom_col, crs=gdf.crs)
+        except Exception as e:
+            print(e, dissolved, agged, many_hits)
+            raise e
+
+    geoms_agged = many_hits.groupby(by, **dissolve_kwargs)[geom_col].agg(
+        lambda x: merge_geometries(x, grid_size=grid_size)
+    )
 
-    dissolved[gdf._geometry_column_name] = dissolved.make_valid()
+    if not dissolve_kwargs.get("as_index"):
+        try:
+            geoms_agged = geoms_agged[geom_col]
+        except KeyError:
+            pass
 
-    return dissolved
+    dissolved[geom_col] = geoms_agged
+
+    return GeoDataFrame(
+        pd.concat([dissolved, one_hit]).sort_index(), geometry=geom_col, crs=gdf.crs
+    )
+
+
+def diss(
+    gdf: GeoDataFrame,
+    by=None,
+    aggfunc="first",
+    as_index: bool = True,
+    grid_size: float | int | None = None,
+    n_jobs: int = 1,
+    **dissolve_kwargs,
+):
+    """Dissolves geometries.
+
+    It takes a GeoDataFrame and dissolves and fixes geometries.
+
+    Args:
+        gdf: the GeoDataFrame that will be dissolved and exploded.
+        by: Columns to dissolve by.
+        aggfunc: How to aggregate the non-geometry colums not in "by".
+        as_index: Whether the 'by' columns should be returned as index. Defaults to
+            True to be consistent with geopandas.
+        **dissolve_kwargs: additional keyword arguments passed to geopandas' dissolve.
+
+    Returns:
+        A GeoDataFrame with dissolved geometries.
+    """
+    if not len(gdf):
+        if as_index:
+            try:
+                return gdf.set_index(by)
+            except Exception:
+                return gdf
+        else:
+            return gdf
+
+    return _dissolve(
+        gdf,
+        by=by,
+        aggfunc=aggfunc,
+        grid_size=grid_size,
+        n_jobs=n_jobs,
+        as_index=as_index,
+        **dissolve_kwargs,
+    )
 
 
 def dissexp(
     gdf: GeoDataFrame,
     by=None,
     aggfunc="first",
     as_index: bool = True,
     index_parts: bool = False,
+    grid_size: float | int | None = None,
+    n_jobs: int = 1,
     **dissolve_kwargs,
 ):
     """Dissolves overlapping geometries.
 
     It takes a GeoDataFrame and dissolves, fixes and explodes geometries.
 
     Args:
@@ -187,34 +313,87 @@
         index_parts: If False (default), the index after dissolve is respected. If
             True, an integer index level is added during explode.
         **dissolve_kwargs: additional keyword arguments passed to geopandas' dissolve.
 
     Returns:
         A GeoDataFrame where overlapping geometries are dissolved.
     """
-    geom_col = gdf._geometry_column_name
-
     dissolve_kwargs = dissolve_kwargs | {
         "by": by,
-        "aggfunc": aggfunc,
         "as_index": as_index,
     }
 
     dissolve_kwargs, ignore_index = _decide_ignore_index(dissolve_kwargs)
 
-    dissolved = gdf.dissolve(**dissolve_kwargs)
-
-    dissolved[geom_col] = dissolved.make_valid()
+    dissolved = diss(
+        gdf, aggfunc=aggfunc, grid_size=grid_size, n_jobs=n_jobs, **dissolve_kwargs
+    )
 
     return make_all_singlepart(
         dissolved, ignore_index=ignore_index, index_parts=index_parts
     )
 
 
-def dissexp_by_cluster(gdf: GeoDataFrame, **dissolve_kwargs) -> GeoDataFrame:
+def dissexp_by_cluster(
+    gdf: GeoDataFrame, predicate=None, n_jobs: int = 1, **dissolve_kwargs
+) -> GeoDataFrame:
+    """Dissolves overlapping geometries through clustering with sjoin and networkx.
+
+    Works exactly like dissexp, but, before dissolving, the geometries are divided
+    into clusters based on overlap (uses the function sgis.get_polygon_clusters).
+    The geometries are then dissolved based on this column (and optionally other
+    columns).
+
+    This might be many times faster than a regular dissexp, if there are many
+    non-overlapping geometries.
+
+    Args:
+        gdf: the GeoDataFrame that will be dissolved and exploded.
+        **dissolve_kwargs: Keyword arguments passed to geopandas' dissolve.
+
+    Returns:
+        A GeoDataFrame where overlapping geometries are dissolved.
+    """
+    return _run_func_by_cluster(
+        dissexp, gdf, predicate=predicate, n_jobs=n_jobs, **dissolve_kwargs
+    )
+
+
+def diss_by_cluster(
+    gdf: GeoDataFrame, predicate=None, n_jobs: int = 1, **dissolve_kwargs
+) -> GeoDataFrame:
+    """Dissolves overlapping geometries through clustering with sjoin and networkx.
+
+    Works exactly like dissexp, but, before dissolving, the geometries are divided
+    into clusters based on overlap (uses the function sgis.get_polygon_clusters).
+    The geometries are then dissolved based on this column (and optionally other
+    columns).
+
+    This might be many times faster than a regular dissexp, if there are many
+    non-overlapping geometries.
+
+    Args:
+        gdf: the GeoDataFrame that will be dissolved and exploded.
+        **dissolve_kwargs: Keyword arguments passed to geopandas' dissolve.
+
+    Returns:
+        A GeoDataFrame where overlapping geometries are dissolved.
+    """
+    return _run_func_by_cluster(
+        diss, gdf, predicate=predicate, n_jobs=n_jobs, **dissolve_kwargs
+    )
+
+
+def _run_func_by_cluster(
+    func: Callable,
+    gdf: GeoDataFrame,
+    predicate=None,
+    n_jobs: int = 1,
+    **dissolve_kwargs,
+) -> GeoDataFrame:
     """Dissolves overlapping geometries through clustering with sjoin and networkx.
 
     Works exactly like dissexp, but, before dissolving, the geometries are divided
     into clusters based on overlap (uses the function sgis.get_polygon_clusters).
     The geometries are then dissolved based on this column (and optionally other
     columns).
 
@@ -233,33 +412,35 @@
     by = dissolve_kwargs.pop("by", [])
     if isinstance(by, str):
         by = [by]
     elif by:
         by = list(by)
 
     if not len(gdf):
-        return dissexp(gdf, by=by, **dissolve_kwargs)
+        return func(gdf, by=by, **dissolve_kwargs)
 
     def get_group_clusters(group: GeoDataFrame):
         """Adds cluster column. Applied to each group because much faster."""
         group = group.reset_index(drop=True)
-        group["_cluster"] = get_cluster_mapper(group)  # component_mapper
+        group["_cluster"] = get_cluster_mapper(
+            group, predicate=predicate
+        )  # component_mapper
         group["_cluster"] = get_grouped_centroids(group, groupby="_cluster")
         return group
 
     if by:
         dissolved = (
             make_all_singlepart(gdf)
             .groupby(by, group_keys=True, dropna=False, as_index=False)
             .apply(get_group_clusters)
-            .pipe(dissexp, by=["_cluster"] + by, **dissolve_kwargs)
+            .pipe(func, by=["_cluster"] + by, n_jobs=n_jobs, **dissolve_kwargs)
         )
     else:
         dissolved = get_group_clusters(make_all_singlepart(gdf)).pipe(
-            dissexp, by="_cluster", **dissolve_kwargs
+            func, by="_cluster", n_jobs=n_jobs, **dissolve_kwargs
         )
 
     if not by:
         dissolved = dissolved.reset_index(drop=True)
 
     elif dissolve_kwargs.get("as_index", True):
         dissolved.index = dissolved.index.droplevel(0)
@@ -272,14 +453,15 @@
 
 def buffdissexp_by_cluster(
     gdf: GeoDataFrame,
     distance: int | float,
     *,
     resolution: int = 50,
     copy: bool = True,
+    n_jobs: int = 1,
     **dissolve_kwargs,
 ) -> GeoDataFrame:
     """Buffers and dissolves overlapping geometries.
 
     Works exactly like buffdissexp, but, before dissolving, the geometries are divided
     into clusters based on overlap (uses the function sgis.get_polygon_clusters).
     The geometries are then dissolved based on this column (and optionally other
@@ -297,15 +479,15 @@
         copy: Whether to copy the GeoDataFrame before buffering. Defaults to True.
         **dissolve_kwargs: additional keyword arguments passed to geopandas' dissolve.
 
     Returns:
         A buffered GeoDataFrame where overlapping geometries are dissolved.
     """
     buffered = buff(gdf, distance, resolution=resolution, copy=copy)
-    return dissexp_by_cluster(buffered, **dissolve_kwargs)
+    return dissexp_by_cluster(buffered, n_jobs=n_jobs, **dissolve_kwargs)
 
 
 def buff(
     gdf: GeoDataFrame | GeoSeries,
     distance: int | float,
     resolution: int = 50,
     copy: bool = True,
```

### Comparing `ssb_sgis-0.3.9/src/sgis/geopandas_tools/centerlines.py` & `ssb_sgis-1.0.0/src/sgis/geopandas_tools/centerlines.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/src/sgis/geopandas_tools/conversion.py` & `ssb_sgis-1.0.0/src/sgis/geopandas_tools/conversion.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,50 @@
 import numbers
-from collections.abc import Iterator, Sized
+import re
+from collections.abc import Collection, Iterator, Mapping, Sized
 from typing import Any
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import pyproj
+import rasterio
 import shapely
+from affine import Affine
 from geopandas import GeoDataFrame, GeoSeries
 from pandas.api.types import is_array_like, is_dict_like, is_list_like
+from pyproj import CRS
+from rasterio import features
 from shapely import Geometry, box, wkb, wkt
-from shapely.geometry import Point
+from shapely.errors import GEOSException
+from shapely.geometry import Point, shape
 from shapely.ops import unary_union
 
 
+try:
+    from torchgeo.datasets.geo import RasterDataset
+except ImportError:
+
+    class RasterDataset:
+        """Placeholder"""
+
+
+@staticmethod
+def crs_to_string(crs):
+    if crs is None:
+        return "None"
+    crs = pyproj.CRS(crs)
+    crs_str = str(crs.to_json_dict()["name"])
+    pattern = r"\d{4,5}"
+    try:
+        return re.search(pattern, crs_str).group()
+    except AttributeError:
+        return crs_str
+
+
 def to_geoseries(obj: Any, crs: Any | None = None) -> GeoSeries:
     if crs is None:
         try:
             crs = obj.crs
         except AttributeError:
             pass
 
@@ -49,31 +76,83 @@
 def to_shapely(obj) -> Geometry:
     if isinstance(obj, Geometry):
         return obj
     if not hasattr(obj, "__iter__"):
         raise TypeError(type(obj))
     if hasattr(obj, "unary_union"):
         return obj.unary_union
-    if is_bbox_like(obj):
-        return box(*obj)
+    # if is_bbox_like(obj):
+    #     return box(*obj)
     try:
         return Point(*obj)
-    except TypeError as e:
-        raise TypeError(obj) from e
+    except TypeError:
+        return box(*to_bbox(obj))
+
+
+def to_bbox(
+    obj: GeoDataFrame | GeoSeries | Geometry | Collection | Mapping,
+) -> tuple[float, float, float, float]:
+    """Returns 4-length tuple of bounds if possible, else raises ValueError.
+
+    Args:
+        obj: Object to be converted to bounding box. Can be geopandas or shapely
+            objects, iterables of exactly four numbers or dictionary like/class
+            with a the keys/attributes "minx", "miny", "maxx", "maxy" or
+            "xmin", "ymin", "xmax", "ymax".
+    """
+    if isinstance(obj, (GeoDataFrame, GeoSeries)):
+        return tuple(obj.total_bounds)
+    if isinstance(obj, Geometry):
+        return tuple(obj.bounds)
+
+    try:
+        minx = int(np.min(obj["minx"]))
+        miny = int(np.min(obj["miny"]))
+        maxx = int(np.max(obj["maxx"]))
+        maxy = int(np.max(obj["maxy"]))
+        return minx, miny, maxx, maxy
+    except Exception:
+        try:
+            minx = int(np.min(obj.minx))
+            miny = int(np.min(obj.miny))
+            maxx = int(np.max(obj.maxx))
+            maxy = int(np.max(obj.maxy))
+            return minx, miny, maxx, maxy
+        except Exception:
+            pass
+
+    if hasattr(obj, "geometry"):
+        try:
+            return tuple(GeoSeries(obj["geometry"]).total_bounds)
+        except Exception:
+            return tuple(GeoSeries(obj.geometry).total_bounds)
+
+    if (
+        hasattr(obj, "__len__")
+        and len(obj) == 4
+        and all(isinstance(x, numbers.Number) for x in obj)
+    ):
+        return tuple(obj)
 
+    try:
+        of_length = f" of length {len(obj)}"
+    except TypeError:
+        of_length = ""
+    raise TypeError(f"Cannot convert type {obj.__class__.__name__}{of_length} to bbox")
 
-def get_utm33(lon: float, lat: float, crs=25833):
+
+def from_4326(lon: float, lat: float, crs=25833):
     """Get utm 33 N coordinates from lonlat (4326)."""
     transformer = pyproj.Transformer.from_crs(
         "EPSG:4326", f"EPSG:{crs}", always_xy=True
     )
     return transformer.transform(lon, lat)
 
 
-def get_lonlat(lon: float, lat: float, crs=25833):
+def to_4326(lon: float, lat: float, crs=25833):
     """Get degree coordinates  33 N coordinates from lonlat (4326)."""
     transformer = pyproj.Transformer.from_crs(
         f"EPSG:{crs}", "EPSG:4326", always_xy=True
     )
     return transformer.transform(lon, lat)
 
 
@@ -119,24 +198,26 @@
         return np.array([(geom.x, geom.y) for geom in gdf])
     return np.array(
         [(geom.x, geom.y) if hasattr(geom, "x") else (None, None) for geom in gdf]
     )
 
 
 def to_gdf(
-    obj: Geometry
-    | str
-    | bytes
-    | list
-    | tuple
-    | dict
-    | GeoSeries
-    | pd.Series
-    | pd.DataFrame
-    | Iterator,
+    obj: (
+        Geometry
+        | str
+        | bytes
+        | list
+        | tuple
+        | dict
+        | GeoSeries
+        | pd.Series
+        | pd.DataFrame
+        | Iterator
+    ),
     crs: str | tuple[str] | None = None,
     geometry: str | tuple[str] | int | None = None,
     **kwargs,
 ) -> GeoDataFrame:
     """Converts geometry-like objects to a GeoDataFrame.
 
     Constructs a GeoDataFrame from any geometry-like object (coordinates, wkt, wkb),
@@ -246,14 +327,45 @@
     if obj is None:
         raise TypeError("Cannot convert NoneType to GeoDataFrame.")
 
     if isinstance(obj, GeoSeries):
         geom_col = geometry or "geometry"
         return _geoseries_to_gdf(obj, geom_col, crs, **kwargs)
 
+    if crs is None:
+        try:
+            crs = obj.crs
+        except AttributeError:
+            try:
+                matches = re.search(r"SRID=(\d+);", obj)
+            except TypeError:
+                try:
+                    matches = re.search(r"SRID=(\d+);", obj[0])
+                except Exception:
+                    pass
+            try:
+                crs = CRS(int("".join(x for x in matches.group(0) if x.isnumeric())))
+            except Exception:
+                pass
+
+    if isinstance(obj, RasterDataset):
+        # read the entire dataset
+        obj = obj[obj.bounds]
+        crs = obj["crs"]
+        array = np.array(obj["image"])
+        transform = get_transform_from_bounds(obj["bbox"], shape=array.shape)
+        return gpd.GeoDataFrame(
+            pd.DataFrame(
+                _array_to_geojson(array, transform),
+                columns=["value", "geometry"],
+            ),
+            geometry="geometry",
+            crs=crs,
+        )
+
     if is_array_like(geometry) and len(geometry) == len(obj):
         geometry = GeoSeries(
             _make_one_shapely_geom(g) for g in geometry if g is not None
         )
         return GeoDataFrame(obj, geometry=geometry, crs=crs, **kwargs)
 
     geom_col: str = find_geometry_column(obj, geometry)
@@ -271,14 +383,17 @@
 
     crs = crs or get_crs_from_dict(obj)
 
     if not is_dict_like(obj):
         if is_bbox_like(obj):
             obj = GeoSeries(shapely.box(*obj), index=index)
             return GeoDataFrame({geom_col: obj}, geometry=geom_col, crs=crs, **kwargs)
+        elif all(hasattr(obj, attr) for attr in ["minx", "miny", "maxx", "maxy"]):
+            obj = GeoSeries(shapely.box(*to_bbox(obj)), index=index)
+            return GeoDataFrame({geom_col: obj}, geometry=geom_col, crs=crs, **kwargs)
         if is_nested_geojson(obj):
             # crs = crs or get_crs_from_dict(obj)
             obj = pd.concat(
                 (GeoSeries(_from_json(g)) for g in obj if g is not None),
                 ignore_index=True,
             )
             if index is not None:
@@ -352,14 +467,41 @@
     try:
         geoseries = _series_like_to_geoseries(obj, index=index)
     except ValueError:
         geoseries = _series_like_to_geoseries(obj.dropna(), index=obj.dropna().index)
     return GeoDataFrame(geometry=geoseries, crs=crs, **kwargs)
 
 
+def _array_to_geojson(array: np.ndarray, transform: Affine):
+    try:
+        return [
+            (value, shape(geom))
+            for geom, value in features.shapes(array, transform=transform)
+        ]
+    except ValueError:
+        array = array.astype(np.float32)
+        return [
+            (value, shape(geom))
+            for geom, value in features.shapes(array, transform=transform)
+        ]
+
+
+def get_transform_from_bounds(
+    obj: GeoDataFrame | GeoSeries | Geometry | tuple, shape: tuple[float, ...]
+) -> Affine:
+    minx, miny, maxx, maxy = to_bbox(obj)
+    if len(shape) == 2:
+        width, height = shape
+    elif len(shape) == 3:
+        _, width, height = shape
+    else:
+        raise ValueError
+    return rasterio.transform.from_bounds(minx, miny, maxx, maxy, width, height)
+
+
 def make_shapely_geoms(obj):
     if _is_one_geometry(obj):
         return _make_one_shapely_geom(obj)
     if isinstance(obj, dict) and "coordinates" in obj:
         return _from_json(obj)
     return (_make_one_shapely_geom(g) for g in obj)
 
@@ -376,16 +518,17 @@
         return True
 
     return False"""
 
 
 def is_bbox_like(obj) -> bool:
     if (
-        hasattr(obj, "__iter__")
+        hasattr(obj, "__len__")
         and len(obj) == 4
+        and hasattr(obj, "__iter__")
         and all(isinstance(x, numbers.Number) for x in obj)
     ):
         return True
     return False
 
 
 def is_nested_geojson(obj) -> bool:
@@ -509,15 +652,22 @@
 
 def _make_one_shapely_geom(obj):
     """Create shapely geometry from wkt, wkb or coordinate tuple.
 
     Works recursively if the object is a nested iterable.
     """
     if isinstance(obj, str):
-        return wkt.loads(obj)
+        try:
+            return wkt.loads(obj)
+        except GEOSException:
+            if obj.startswith("geography"):
+                matches = re.search(r"SRID=(\d+);", obj)
+                srid = matches.group(0)
+                _, _wkt = obj.split(srid)
+                return wkt.loads(_wkt)
 
     if isinstance(obj, bytes):
         return wkb.loads(obj)
 
     if isinstance(obj, Geometry):
         return obj
```

### Comparing `ssb_sgis-0.3.9/src/sgis/geopandas_tools/duplicates.py` & `ssb_sgis-1.0.0/src/sgis/geopandas_tools/duplicates.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 from collections.abc import Iterable
 
 import networkx as nx
 import pandas as pd
 from geopandas import GeoDataFrame, GeoSeries
-from shapely import STRtree, difference, intersection, make_valid, unary_union, union
+from shapely import STRtree, difference, make_valid, simplify, unary_union
 from shapely.errors import GEOSException
-from shapely.geometry import Polygon
 
-from .general import _push_geom_col, clean_geoms
+from .general import (
+    _determine_geom_type_args,
+    _push_geom_col,
+    clean_geoms,
+    parallel_unary_union_geoseries,
+)
 from .geometry_types import get_geom_type, make_all_singlepart, to_single_geom_type
-from .overlay import clean_overlay
+from .overlay import _run_overlay_dask, clean_overlay, make_valid_and_keep_geom_type
+from .sfilter import sfilter_inverse, sfilter_split
+
+
+PRECISION = 1e-3
 
 
 def update_geometries(
     gdf: GeoDataFrame,
     geom_type: str | None = None,
-    keep_geom_type: bool = True,
+    keep_geom_type: bool | None = None,
     grid_size: int | None = None,
+    n_jobs: int = 1,
+    predicate: str | None = "intersects",
 ) -> GeoDataFrame:
     """Puts geometries on top of each other rowwise.
 
     Since this operation is done rowwise, it's important to
     first sort the GeoDataFrame approriately. See example below.
 
     Args:
@@ -76,58 +86,104 @@
         idx                                           geometry
     0    1  POLYGON ((0.03141 0.99951, 0.06279 0.99803, 0....
 
     """
     if len(gdf) <= 1:
         return gdf
 
-    if geom_type:
-        gdf = to_single_geom_type(gdf, geom_type)
-        keep_geom_type = True
-    elif keep_geom_type:
-        geom_type = get_geom_type(gdf)
-        if geom_type == "mixed":
-            raise ValueError("Cannot have mixed geometries when keep_geom_type is True")
-
-    geom_col = gdf._geometry_column_name
-    index_mapper = {i: idx for i, idx in enumerate(gdf.index)}
-    gdf = gdf.reset_index(drop=True)
+    copied = make_all_singlepart(clean_geoms(gdf))
+
+    copied, geom_type, keep_geom_type = _determine_geom_type_args(
+        copied, geom_type, keep_geom_type
+    )
 
-    tree = STRtree(gdf.geometry.values)
-    left, right = tree.query(gdf.geometry.values, predicate="intersects")
+    geom_col = copied._geometry_column_name
+    index_mapper = {i: idx for i, idx in enumerate(copied.index)}
+    copied = copied.reset_index(drop=True)
+
+    tree = STRtree(copied.geometry.values)
+    left, right = tree.query(copied.geometry.values, predicate=predicate)
     indices = pd.Series(right, index=left).loc[lambda x: x.index > x.values]
 
     # select geometries from 'right', index from 'left', dissolve by 'left'
-    erasers = (
-        pd.Series(gdf.geometry.loc[indices.values].values, index=indices.index)
-        .groupby(level=0)
-        .agg(unary_union)
-    )
+    erasers = pd.Series(copied.geometry.loc[indices.values].values, index=indices.index)
+    if n_jobs > 1:
+        erasers = parallel_unary_union_geoseries(
+            erasers,
+            level=0,
+            n_jobs=n_jobs,
+            grid_size=grid_size,
+        )
+        erasers = pd.Series(erasers, index=indices.index.unique())
+    else:
+        only_one = erasers.groupby(level=0).transform("size") == 1
+        one_hit = erasers[only_one]
+        many_hits = (
+            erasers[~only_one]
+            .groupby(level=0)
+            .agg(lambda x: make_valid(unary_union(x, grid_size=grid_size)))
+        )
+        erasers = pd.concat([one_hit, many_hits]).sort_index()
 
     # match up the aggregated erasers by index
-    erased = difference(
-        gdf.geometry.loc[erasers.index],
-        erasers,
-        grid_size=grid_size,
-    )
+    if n_jobs > 1:
+        arr1 = copied.geometry.loc[erasers.index].to_numpy()
+        arr2 = erasers.to_numpy()
+        try:
+            erased = _run_overlay_dask(
+                arr1, arr2, func=difference, n_jobs=n_jobs, grid_size=grid_size
+            )
+        except GEOSException:
+            arr1 = make_valid_and_keep_geom_type(
+                arr1, geom_type=geom_type, n_jobs=n_jobs
+            )
+            arr2 = make_valid_and_keep_geom_type(
+                arr2, geom_type=geom_type, n_jobs=n_jobs
+            )
+            erased = _run_overlay_dask(
+                arr1, arr2, func=difference, n_jobs=n_jobs, grid_size=grid_size
+            )
+        erased = GeoSeries(erased, index=erasers.index)
+    else:
+        erased = make_valid(
+            difference(
+                copied.geometry.loc[erasers.index],
+                erasers,
+                grid_size=grid_size,
+            )
+        )
+
+    copied.loc[erased.index, geom_col] = erased
+
+    copied = copied.loc[~copied.is_empty]
 
-    gdf.loc[erased.index, geom_col] = erased
+    copied.index = copied.index.map(index_mapper)
 
-    gdf = gdf.loc[~gdf.is_empty]
+    # TODO check why polygons dissappear in rare cases. For now, just add back the missing
+    dissapeared = sfilter_inverse(gdf, copied.buffer(-PRECISION))
+    copied = pd.concat([copied, dissapeared])
 
-    gdf.index = gdf.index.map(index_mapper)
+    # TODO fix dupliates again with dissolve?
+    # dups = get_intersections(copied, geom_type="polygon")
+    # dups["_cluster"] = get_cluster_mapper(dups.geometry.values)
+    # no_dups = dissexp(dups, by="_cluster").drop(columns="_cluster")
+    # copied = clean_overlay(copied, no_dups, how="update", geom_type="polygon")
 
     if keep_geom_type:
-        gdf = to_single_geom_type(gdf, geom_type)
+        copied = to_single_geom_type(copied, geom_type)
 
-    return gdf
+    return copied
 
 
 def get_intersections(
-    gdf: GeoDataFrame, geom_type: str | None = None, keep_geom_type: bool = True
+    gdf: GeoDataFrame,
+    geom_type: str | None = None,
+    keep_geom_type: bool | None = None,
+    predicate: str | None = "intersects",
+    n_jobs: int = 1,
 ) -> GeoDataFrame:
     """Find geometries that intersect in a GeoDataFrame.
 
     Does an intersection with itself and keeps only the geometries that appear
     more than once.
 
     Note that the returned GeoDataFrame in most cases contain two rows per
@@ -199,30 +255,40 @@
     """
     if isinstance(gdf, GeoSeries):
         gdf = GeoDataFrame({"geometry": gdf}, crs=gdf.crs)
         was_geoseries = True
     else:
         was_geoseries = False
 
+    gdf, geom_type, keep_geom_type = _determine_geom_type_args(
+        gdf, geom_type, keep_geom_type
+    )
+
     idx_name = gdf.index.name
     gdf = gdf.assign(orig_idx=gdf.index).reset_index(drop=True)
 
     duplicated_geoms = _get_intersecting_geometries(
-        gdf, geom_type, keep_geom_type
+        gdf,
+        geom_type,
+        keep_geom_type,
+        n_jobs=n_jobs,
+        predicate=predicate,
     ).pipe(clean_geoms)
 
     duplicated_geoms.index = duplicated_geoms["orig_idx"].values
     duplicated_geoms.index.name = idx_name
+
     if was_geoseries:
         return duplicated_geoms.geometry
+
     return duplicated_geoms.drop(columns="orig_idx")
 
 
 def _get_intersecting_geometries(
-    gdf: GeoDataFrame, geom_type, keep_geom_type
+    gdf: GeoDataFrame, geom_type, keep_geom_type, n_jobs, predicate
 ) -> GeoDataFrame:
     right = gdf[[gdf._geometry_column_name]]
     right["idx_right"] = right.index
 
     left = (
         gdf
         if not any("index_" in str(col) for col in gdf)
@@ -234,34 +300,50 @@
         return df["idx_left"] != df["idx_right"]
 
     if geom_type or get_geom_type(gdf) != "mixed":
         intersected = clean_overlay(
             left,
             right,
             how="intersection",
+            predicate=predicate,
             geom_type=geom_type,
             keep_geom_type=keep_geom_type,
+            n_jobs=n_jobs,
         ).loc[are_not_identical]
     else:
         if keep_geom_type:
             raise ValueError(
                 "Cannot set keep_geom_type=True when the geom_type is mixed."
             )
         gdf = make_all_singlepart(gdf)
         intersected = []
         for geom_type in ["polygon", "line", "point"]:
             if not len(to_single_geom_type(gdf, geom_type)):
                 continue
             intersected += [
-                clean_overlay(left, right, how="intersection", geom_type=geom_type)
+                clean_overlay(
+                    left,
+                    right,
+                    how="intersection",
+                    predicate=predicate,
+                    geom_type=geom_type,
+                    n_jobs=n_jobs,
+                )
             ]
         intersected = pd.concat(intersected, ignore_index=True).loc[are_not_identical]
 
     # make sure it's correct by sjoining a point inside the polygons
-    points_joined = intersected.representative_point().to_frame().sjoin(intersected)
+    points_joined = (
+        # large and very detailed geometries can dissappear with small negative buffer
+        simplify(intersected.geometry, 1e-3)
+        .buffer(-1e-3)
+        .representative_point()
+        .to_frame()
+        .sjoin(intersected)
+    )
 
     duplicated_points = points_joined.loc[points_joined.index.duplicated(keep=False)]
 
     return intersected.loc[intersected.index.isin(duplicated_points.index)].drop(
         columns=["idx_left", "idx_right"]
     )
```

### Comparing `ssb_sgis-0.3.9/src/sgis/geopandas_tools/general.py` & `ssb_sgis-1.0.0/src/sgis/geopandas_tools/general.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numbers
 import warnings
 from collections.abc import Hashable, Iterable
 from typing import Any
 
+import joblib
 import numpy as np
 import pandas as pd
 import pyproj
 from geopandas import GeoDataFrame, GeoSeries
 from geopandas.array import GeometryArray, GeometryDtype
 from numpy.typing import NDArray
 from shapely import (
@@ -15,16 +16,17 @@
     get_exterior_ring,
     get_interior_ring,
     get_num_interior_rings,
     get_parts,
     linestrings,
     make_valid,
 )
+from shapely import points as shapely_points
+from shapely import unary_union
 from shapely.geometry import LineString, Point
-from shapely.ops import unary_union
 
 from .geometry_types import get_geom_type, make_all_singlepart, to_single_geom_type
 
 
 def split_geom_types(gdf: GeoDataFrame | GeoSeries) -> tuple[GeoDataFrame | GeoSeries]:
     return tuple(
         gdf.loc[gdf.geom_type == geom_type] for geom_type in gdf.geom_type.unique()
@@ -293,32 +295,75 @@
     # using enumerate, then iloc on the sorted dict keys.
     # to avoid creating a temporary area column (which doesn't work for GeoSeries).
     area_mapper = dict(enumerate(gdf.area.values))
     sorted_areas = dict(reversed(sorted(area_mapper.items(), key=lambda item: item[1])))
     return gdf.iloc[list(sorted_areas)]
 
 
+def sort_df(
+    df: pd.DataFrame | GeoDataFrame, sort_col: pd.Series
+) -> pd.DataFrame | GeoDataFrame:
+    value_mapper: dict[int, Any] = dict(enumerate(sort_col.values))
+    sorted_indices = dict(
+        reversed(sorted(value_mapper.items(), key=lambda item: item[1]))
+    )
+    return df.iloc[list(sorted_indices)]
+
+
 def sort_long_first(gdf: GeoDataFrame | GeoSeries) -> GeoDataFrame | GeoSeries:
     """Sort GeoDataFrame by length in decending order.
 
     Args:
         gdf: A GeoDataFrame or GeoSeries.
 
     Returns:
-        A GeoDataFrame or GeoSeries sorted from large to small in length.
+        A GeoDataFrame or GeoSeries sorted from long to short in length.
     """
     # using enumerate, then iloc on the sorted dict keys.
     # to avoid creating a temporary area column (which doesn't work for GeoSeries).
     length_mapper = dict(enumerate(gdf.length.values))
     sorted_lengths = dict(
         reversed(sorted(length_mapper.items(), key=lambda item: item[1]))
     )
     return gdf.iloc[list(sorted_lengths)]
 
 
+def sort_short_first(gdf: GeoDataFrame | GeoSeries) -> GeoDataFrame | GeoSeries:
+    """Sort GeoDataFrame by length in ascending order.
+
+    Args:
+        gdf: A GeoDataFrame or GeoSeries.
+
+    Returns:
+        A GeoDataFrame or GeoSeries sorted from short to long in length.
+    """
+    # using enumerate, then iloc on the sorted dict keys.
+    # to avoid creating a temporary area column (which doesn't work for GeoSeries).
+    length_mapper = dict(enumerate(gdf.length.values))
+    sorted_lengths = dict(sorted(length_mapper.items(), key=lambda item: item[1]))
+    return gdf.iloc[list(sorted_lengths)]
+
+
+def sort_small_first(gdf: GeoDataFrame | GeoSeries) -> GeoDataFrame | GeoSeries:
+    """Sort GeoDataFrame by area in ascending order.
+
+    Args:
+        gdf: A GeoDataFrame or GeoSeries.
+
+    Returns:
+        A GeoDataFrame or GeoSeries sorted from small to large in area.
+
+    """
+    # using enumerate, then iloc on the sorted dict keys.
+    # to avoid creating a temporary area column (which doesn't work for GeoSeries).
+    area_mapper = dict(enumerate(gdf.area.values))
+    sorted_areas = dict(sorted(area_mapper.items(), key=lambda item: item[1]))
+    return gdf.iloc[list(sorted_areas)]
+
+
 def make_lines_between_points(
     arr1: NDArray[Point] | GeometryArray | GeoSeries,
     arr2: NDArray[Point] | GeometryArray | GeoSeries,
 ) -> NDArray[LineString]:
     """Creates an array of linestrings from two arrays of points.
 
     The operation is done rowwise.
@@ -401,14 +446,36 @@
     y = np.random.rand(n) * float(loc) * 2
 
     return GeoDataFrame(
         (Point(x, y) for x, y in zip(x, y, strict=True)), columns=["geometry"]
     )
 
 
+def random_points_in_polygons(gdf: GeoDataFrame, n: int, seed=None) -> GeoDataFrame:
+    all_points = []
+
+    rng = np.random.default_rng(seed)
+
+    for i, geom in enumerate(gdf.geometry):
+        minx, miny, maxx, maxy = geom.bounds
+
+        xs = rng.uniform(minx, maxx, size=n * 500)
+        ys = rng.uniform(miny, maxy, size=n * 500)
+
+        points = GeoSeries(shapely_points(xs, y=ys), index=[i] * len(xs))
+        all_points.append(points)
+
+    return (
+        pd.concat(all_points)
+        .loc[lambda x: x.intersects(gdf.geometry)]
+        .groupby(level=0)
+        .head(n)
+    )
+
+
 def to_lines(*gdfs: GeoDataFrame, copy: bool = True) -> GeoDataFrame:
     """Makes lines out of one or more GeoDataFrames and splits them at intersections.
 
     The GeoDataFrames' geometries are converted to LineStrings, then unioned together
     and made to singlepart. The lines are split at the intersections. Mimics
     'feature to line' in ArcGIS.
 
@@ -523,53 +590,192 @@
 
     return make_all_singlepart(unioned, ignore_index=True)
 
 
 def clean_clip(
     gdf: GeoDataFrame | GeoSeries,
     mask: GeoDataFrame | GeoSeries | Geometry,
-    keep_geom_type: bool = True,
+    keep_geom_type: bool | None = None,
     geom_type: str | None = None,
     **kwargs,
 ) -> GeoDataFrame | GeoSeries:
     """Clips and clean geometries.
 
     Geopandas.clip does a "fast and dirty clipping, with no guarantee for valid
     outputs". Here, the clipped geometries are made valid, and empty and NaN
     geometries are removed.
 
     Args:
         gdf: GeoDataFrame or GeoSeries to be clipped
         mask: the geometry to clip gdf
+        geom_type: Optionally specify what geometry type to keep.,
+            if there are mixed geometry types. Must be either "polygon",
+            "line" or "point".
+        keep_geom_type: Defaults to None, meaning True if 'geom_type' is given
+            and True if the geometries are single-typed and False if the geometries
+            are mixed.
         **kwargs: Keyword arguments passed to geopandas.GeoDataFrame.clip
 
     Returns:
         The cleanly clipped GeoDataFrame.
 
     Raises:
         TypeError: If gdf is not of type GeoDataFrame or GeoSeries.
     """
     if not isinstance(gdf, (GeoDataFrame, GeoSeries)):
         raise TypeError(f"'gdf' should be GeoDataFrame or GeoSeries, got {type(gdf)}")
 
-    if geom_type is None and keep_geom_type:
-        geom_type = get_geom_type(gdf)
-        if geom_type == "mixed":
-            raise ValueError(
-                "Mixed geometry types is not allowed when keep_geom_type is True."
-            )
+    gdf, geom_type, keep_geom_type = _determine_geom_type_args(
+        gdf, geom_type, keep_geom_type
+    )
 
     try:
         gdf = gdf.clip(mask, **kwargs).pipe(clean_geoms)
     except Exception:
         gdf = clean_geoms(gdf)
         try:
             mask = clean_geoms(mask)
         except TypeError:
             mask = make_valid(mask)
 
         return gdf.clip(mask, **kwargs).pipe(clean_geoms)
 
-    if geom_type is not None or keep_geom_type:
+    if keep_geom_type:
         gdf = to_single_geom_type(gdf, geom_type)
 
     return gdf
+
+
+def _determine_geom_type_args(
+    gdf: GeoDataFrame, geom_type: str | None, keep_geom_type: bool | None
+) -> tuple[GeoDataFrame, str, bool]:
+    if geom_type:
+        gdf = to_single_geom_type(gdf, geom_type)
+        keep_geom_type = True
+    elif keep_geom_type is None:
+        geom_type = get_geom_type(gdf)
+        if geom_type == "mixed":
+            keep_geom_type = False
+        else:
+            keep_geom_type = True
+    elif keep_geom_type:
+        geom_type = get_geom_type(gdf)
+        if geom_type == "mixed":
+            raise ValueError("Cannot set keep_geom_type=True with mixed geometries")
+    return gdf, geom_type, keep_geom_type
+
+
+def merge_geometries(geoms: GeoSeries, grid_size=None) -> Geometry:
+    return make_valid(unary_union(geoms, grid_size=grid_size))
+
+
+def parallel_unary_union(
+    gdf: GeoDataFrame, n_jobs: int = 1, by=None, grid_size=None, **kwargs
+) -> list[Geometry]:
+    try:
+        geom_col = gdf._geometry_column_name
+    except AttributeError:
+        geom_col = "geometry"
+
+    if by is not None and not isinstance(by, str):
+        gdf = gdf.copy()
+        try:
+            gdf["_by"] = gdf[by].astype(str).agg("-".join, axis=1)
+        except KeyError:
+            gdf["_by"] = by
+        by = "_by"
+
+    if gdf.crs is None:
+        gdf.crs = 25833
+        _was_none = True
+    else:
+        _was_none = False
+
+    if isinstance(gdf.index, pd.MultiIndex):
+        gdf = gdf.reset_index(drop=True)
+
+    dissolved = (
+        dask_geopandas.from_geopandas(gdf, npartitions=n_jobs).dissolve(by).compute()
+    )
+    if _was_none:
+        dissolved.crs = None
+
+    return dissolved.geometry
+
+
+def parallel_unary_union_geoseries(
+    ser: GeoSeries, n_jobs: int = 1, grid_size=None, **kwargs
+) -> list[Geometry]:
+    if ser.crs is None:
+        ser.crs = 25833
+        _was_none = True
+    else:
+        _was_none = False
+
+    if isinstance(ser.index, pd.MultiIndex):
+        ser = ser.reset_index(drop=True)
+
+    dissolved = (
+        dask_geopandas.from_geopandas(ser.to_frame("geometry"), npartitions=n_jobs)
+        .dissolve(**kwargs)
+        .compute()
+    )
+    if _was_none:
+        dissolved.crs = None
+
+    return dissolved.geometry
+
+
+def parallel_unary_union(
+    gdf: GeoDataFrame, n_jobs: int = 1, by=None, grid_size=None, **kwargs
+) -> list[Geometry]:
+    try:
+        geom_col = gdf._geometry_column_name
+    except AttributeError:
+        geom_col = "geometry"
+
+    with joblib.Parallel(n_jobs=n_jobs, backend="threading") as parallel:
+        delayed_operations = []
+        for _, geoms in gdf.groupby(by, **kwargs)[geom_col]:
+            delayed_operations.append(
+                joblib.delayed(merge_geometries)(geoms, grid_size=grid_size)
+            )
+
+        return parallel(delayed_operations)
+
+
+def parallel_unary_union_geoseries(
+    ser: GeoSeries, n_jobs: int = 1, grid_size=None, **kwargs
+) -> list[Geometry]:
+
+    is_one_hit = ser.groupby(**kwargs).transform("size") == 1
+
+    one_hit = ser.loc[is_one_hit]
+    many_hits = ser.loc[~is_one_hit]
+
+    with joblib.Parallel(n_jobs=n_jobs, backend="threading") as parallel:
+        delayed_operations = []
+        for _, geoms in many_hits.groupby(**kwargs):
+            delayed_operations.append(
+                joblib.delayed(merge_geometries)(geoms, grid_size=grid_size)
+            )
+
+        dissolved = pd.Series(
+            parallel(delayed_operations),
+            index=is_one_hit[lambda x: x == False].index.unique(),
+        )
+
+    return pd.concat([dissolved, one_hit]).sort_index().values
+
+
+def parallel_unary_union_geoseries(
+    ser: GeoSeries, n_jobs: int = 1, grid_size=None, **kwargs
+) -> list[Geometry]:
+
+    with joblib.Parallel(n_jobs=n_jobs, backend="threading") as parallel:
+        delayed_operations = []
+        for _, geoms in ser.groupby(**kwargs):
+            delayed_operations.append(
+                joblib.delayed(merge_geometries)(geoms, grid_size=grid_size)
+            )
+
+        return parallel(delayed_operations)
```

### Comparing `ssb_sgis-0.3.9/src/sgis/geopandas_tools/geocoding.py` & `ssb_sgis-1.0.0/src/sgis/geopandas_tools/geocoding.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/src/sgis/geopandas_tools/geometry_types.py` & `ssb_sgis-1.0.0/src/sgis/geopandas_tools/geometry_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from shapely import Geometry
 
 
 def make_all_singlepart(
     gdf: GeoDataFrame | GeoSeries, index_parts: bool = False, ignore_index: bool = False
 ) -> GeoDataFrame | GeoSeries:
     # only explode if nessecary
-    if index_parts or ignore_index and not gdf.index.equals(pd.Index(range(len(gdf)))):
+    if (
+        index_parts or ignore_index
+    ):  # and not gdf.index.equals(pd.Index(range(len(gdf)))):
         gdf = gdf.explode(index_parts=index_parts, ignore_index=ignore_index)
 
     while not gdf.geom_type.isin(
         ["Polygon", "Point", "LineString", "LinearRing"]
     ).all():
         gdf = gdf.explode(index_parts=index_parts, ignore_index=ignore_index)
```

### Comparing `ssb_sgis-0.3.9/src/sgis/geopandas_tools/neighbors.py` & `ssb_sgis-1.0.0/src/sgis/geopandas_tools/neighbors.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 The functions rely on the pandas index as identifiers for the geometries and their
 neighbors. This makes it easy to join or aggregate the results onto the input
 GeoDataFrames.
 
 The results of all functions will be identical with GeoDataFrame and GeoSeries as input
 types.
 """
+
 import numpy as np
+import shapely
 from geopandas import GeoDataFrame, GeoSeries
-from pandas import DataFrame, Series
+from pandas import DataFrame, Series, concat
+from shapely import STRtree
 from sklearn.neighbors import NearestNeighbors
 
 from .conversion import coordinate_array
 from .geometry_types import get_geom_type
 
 
 def get_neighbor_indices(
@@ -233,14 +236,41 @@
     return get_k_nearest_neighbors(
         gdf=gdf,
         neighbors=neighbors,
         k=len(neighbors),
     )
 
 
+def sjoin_within_distance(
+    gdf: GeoDataFrame | GeoSeries,
+    neighbors: GeoDataFrame | GeoSeries,
+    distance: int | float,
+    distance_col: str = "distance",
+    **kwargs,
+) -> GeoDataFrame:
+    """Sjoin with a buffer on the right GeoDataFrame and adds a distance column."""
+
+    new_neighbor_cols = {"__left_range_idx": range(len(neighbors))}
+    if distance:
+        new_neighbor_cols[neighbors._geometry_column_name] = lambda x: x.buffer(
+            distance
+        )
+
+    # using assign to get a copy
+    neighbors = neighbors.assign(**new_neighbor_cols)
+
+    out = gdf.sjoin(neighbors, **kwargs)
+
+    out[distance_col] = shapely.distance(
+        out.geometry.values, neighbors.geometry.iloc[out["__left_range_idx"]].values
+    )
+
+    return out.drop(columns="__left_range_idx")
+
+
 def get_k_nearest_neighbors(
     gdf: GeoDataFrame | GeoSeries,
     neighbors: GeoDataFrame | GeoSeries,
     k: int,
     *,
     strict: bool = False,
 ) -> DataFrame:
```

### Comparing `ssb_sgis-0.3.9/src/sgis/geopandas_tools/point_operations.py` & `ssb_sgis-1.0.0/src/sgis/geopandas_tools/point_operations.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/src/sgis/geopandas_tools/polygon_operations.py` & `ssb_sgis-1.0.0/src/sgis/geopandas_tools/polygon_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Functions for polygon geometries."""
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 import shapely
 from geopandas import GeoDataFrame, GeoSeries
+from geopandas.array import GeometryArray
 from shapely import (
     STRtree,
     area,
     box,
     buffer,
     difference,
     get_exterior_ring,
@@ -19,18 +20,25 @@
     make_valid,
     polygons,
     unary_union,
 )
 from shapely.errors import GEOSException
 
 from .duplicates import get_intersections
-from .general import _push_geom_col, clean_geoms, get_grouped_centroids, to_lines
+from .general import (
+    _push_geom_col,
+    clean_geoms,
+    get_grouped_centroids,
+    parallel_unary_union,
+    parallel_unary_union_geoseries,
+    to_lines,
+)
 from .geometry_types import get_geom_type, make_all_singlepart, to_single_geom_type
 from .neighbors import get_neighbor_indices
-from .overlay import clean_overlay
+from .overlay import _try_difference, clean_overlay
 from .polygons_as_rings import PolygonsAsRings
 from .sfilter import sfilter, sfilter_inverse
 
 
 def get_polygon_clusters(
     *gdfs: GeoDataFrame | GeoSeries,
     cluster_col: str = "cluster",
@@ -199,14 +207,16 @@
     gdf: GeoDataFrame | list[GeoDataFrame],
     to_eliminate: GeoDataFrame,
     *,
     remove_isolated: bool = False,
     fix_double: bool = True,
     ignore_index: bool = False,
     aggfunc: str | dict | list | None = None,
+    grid_size=None,
+    n_jobs: int = 1,
     **kwargs,
 ) -> GeoDataFrame | tuple[GeoDataFrame]:
     """Dissolves selected polygons with the longest bordering neighbor polygon.
 
     Eliminates selected geometries by dissolving them with the neighboring
     polygon with the longest shared border. The index and column values of the
     large polygons will be kept, unless else is specified.
@@ -232,15 +242,45 @@
             polygons might get values from the polygons to be eliminated
             (if aggfunc="first").
         kwargs: Keyword arguments passed to the dissolve method.
 
     Returns:
         The GeoDataFrame (gdf) with the geometries of 'to_eliminate' dissolved in.
         If multiple GeoDataFrame are passed as 'gdf', they are returned as a tuple.
+
+    Examples
+    --------
+
+    Create two polygons with a sliver in between:
+
+    >>> sliver = sg.to_gdf(Polygon([(0, 0), (0.1, 1), (0, 2), (-0.1, 1)]))
+    >>> small_poly = sg.to_gdf(
+    ...     Polygon([(0, 0), (-0.1, 1), (0, 2), (-1, 2), (-2, 2), (-1, 1)])
+    ... )
+    >>> large_poly = sg.to_gdf(
+    ...     Polygon([(0, 0), (0.1, 1), (1, 2), (2, 2), (3, 2), (3, 0)])
+    ... )
+
+    Using multiple GeoDataFrame as input, the sliver is eliminated into the small
+    polygon (because it has the longest border with sliver).
+
+    >>> small_poly_eliminated, large_poly_eliminated = sg.eliminate_by_longest(
+    ...     [small_poly, large_poly], sliver
+    ... )
+
+    With only one input GeoDataFrame:
+
+    >>> polys = pd.concat([small_poly, large_poly])
+    >>> eliminated = sg.eliminate_by_longest(polys, sliver)
+
+
     """
+    if not len(to_eliminate):
+        return gdf
+
     if isinstance(gdf, (list, tuple)):
         # concat, then break up the dataframes in the end
         was_multiple_gdfs = True
         original_cols = [df.columns for df in gdf]
         gdf = pd.concat(df.assign(**{"_df_idx": i}) for i, df in enumerate(gdf))
     else:
         was_multiple_gdfs = False
@@ -256,19 +296,21 @@
 
     gdf["_dissolve_idx"] = gdf.index
     to_eliminate = to_eliminate.assign(_eliminate_idx=lambda x: range(len(x)))
 
     # convert to lines to get the borders
     lines_eliminate = to_lines(to_eliminate[["_eliminate_idx", "geometry"]])
 
-    borders = (
-        gdf[["_dissolve_idx", "geometry"]]
-        .overlay(lines_eliminate, keep_geom_type=False)
-        .loc[lambda x: x["_eliminate_idx"].notna()]
-    )
+    borders = clean_overlay(
+        gdf[["_dissolve_idx", "geometry"]],
+        lines_eliminate,
+        keep_geom_type=False,
+        grid_size=grid_size,
+        n_jobs=n_jobs,
+    ).loc[lambda x: x["_eliminate_idx"].notna()]
 
     borders["_length"] = borders.length
 
     # as DataFrame because GeoDataFrame constructor is expensive
     borders = pd.DataFrame(borders)
 
     longest_border = borders.sort_values("_length", ascending=False).drop_duplicates(
@@ -293,14 +335,16 @@
 
     eliminated = _eliminate(
         pd.DataFrame(gdf),
         pd.concat([actually_eliminate, containing_eliminators]),
         aggfunc,
         crs,
         fix_double,
+        grid_size=grid_size,
+        n_jobs=n_jobs,
         **kwargs,
     )
 
     if not ignore_index:
         eliminated.index = eliminated.index.map(idx_mapper)
         eliminated.index.name = idx_name
 
@@ -337,14 +381,16 @@
     *,
     max_distance: int | float | None = None,
     remove_isolated: bool = False,
     fix_double: bool = False,
     ignore_index: bool = False,
     aggfunc: str | dict | list | None = None,
     predicate: str = "intersects",
+    grid_size=None,
+    n_jobs: int = 1,
     **kwargs,
 ) -> GeoDataFrame | tuple[GeoDataFrame]:
     """Dissolves selected polygons with the largest neighbor polygon.
 
     Eliminates selected geometries by dissolving them with the neighboring
     polygon with the largest area. The index and column values of the
     large polygons will be kept, unless else is specified.
@@ -370,67 +416,102 @@
         predicate: Binary predicate passed to sjoin. Defaults to "intersects".
         kwargs: Keyword arguments passed to the dissolve method.
 
     Returns:
         The GeoDataFrame (gdf) with the geometries of 'to_eliminate' dissolved in.
         If multiple GeoDataFrame are passed as 'gdf', they are returned as a tuple.
 
+    Examples
+    --------
+
+    Create two polygons with a sliver in between:
+
+    >>> sliver = sg.to_gdf(Polygon([(0, 0), (0.1, 1), (0, 2), (-0.1, 1)]))
+    >>> small_poly = sg.to_gdf(
+    ...     Polygon([(0, 0), (-0.1, 1), (0, 2), (-1, 2), (-2, 2), (-1, 1)])
+    ... )
+    >>> large_poly = sg.to_gdf(
+    ...     Polygon([(0, 0), (0.1, 1), (1, 2), (2, 2), (3, 2), (3, 0)])
+    ... )
+
+    Using multiple GeoDataFrame as input, the sliver is eliminated into
+    the large polygon.
+
+    >>> small_poly_eliminated, large_poly_eliminated = sg.eliminate_by_largest(
+    ...     [small_poly, large_poly], sliver
+    ... )
+
+    With only one input GeoDataFrame:
+
+    >>> polys = pd.concat([small_poly, large_poly])
+    >>> eliminated = sg.eliminate_by_largest(polys, sliver)
+
     """
     return _eliminate_by_area(
         gdf,
         to_eliminate=to_eliminate,
         remove_isolated=remove_isolated,
         max_distance=max_distance,
         ignore_index=ignore_index,
         sort_ascending=False,
         aggfunc=aggfunc,
         predicate=predicate,
         fix_double=fix_double,
+        grid_size=grid_size,
+        n_jobs=n_jobs,
         **kwargs,
     )
 
 
 def eliminate_by_smallest(
     gdf: GeoDataFrame | list[GeoDataFrame],
     to_eliminate: GeoDataFrame,
     *,
     max_distance: int | float | None = None,
     remove_isolated: bool = False,
     ignore_index: bool = False,
     aggfunc: str | dict | list | None = None,
     predicate: str = "intersects",
     fix_double: bool = False,
+    grid_size=None,
+    n_jobs: int = 1,
     **kwargs,
 ) -> GeoDataFrame | tuple[GeoDataFrame]:
     return _eliminate_by_area(
         gdf,
         to_eliminate=to_eliminate,
         remove_isolated=remove_isolated,
         max_distance=max_distance,
         ignore_index=ignore_index,
         sort_ascending=True,
         aggfunc=aggfunc,
         predicate=predicate,
         fix_double=fix_double,
+        grid_size=grid_size,
+        n_jobs=n_jobs,
         **kwargs,
     )
 
 
 def _eliminate_by_area(
     gdf: GeoDataFrame,
     to_eliminate: GeoDataFrame,
     remove_isolated: bool,
     max_distance: int | float | None,
     sort_ascending: bool,
     ignore_index: bool = False,
     aggfunc: str | dict | list | None = None,
     predicate="intersects",
     fix_double: bool = False,
+    grid_size=None,
+    n_jobs: int = 1,
     **kwargs,
 ) -> GeoDataFrame:
+    if not len(to_eliminate):
+        return gdf
     if isinstance(gdf, (list, tuple)):
         was_multiple_gdfs = True
         original_cols = [df.columns for df in gdf]
         gdf = pd.concat(df.assign(**{"_df_idx": i}) for i, df in enumerate(gdf))
     else:
         was_multiple_gdfs = False
 
@@ -464,15 +545,24 @@
         .loc[lambda x: ~x.index.duplicated(keep="first")]
     )
 
     gdf = pd.DataFrame(gdf)
 
     notna = joined.loc[lambda x: x["_dissolve_idx"].notna()]
 
-    eliminated = _eliminate(gdf, notna, aggfunc, crs, fix_double=fix_double, **kwargs)
+    eliminated = _eliminate(
+        gdf,
+        notna,
+        aggfunc,
+        crs,
+        fix_double=fix_double,
+        grid_size=grid_size,
+        n_jobs=n_jobs,
+        **kwargs,
+    )
 
     if not ignore_index:
         eliminated.index = eliminated.index.map(idx_mapper)
         eliminated.index.name = idx_name
 
     if not remove_isolated:
         isolated = joined.loc[joined["_dissolve_idx"].isna()]
@@ -499,15 +589,17 @@
     for i, cols in enumerate(original_cols):
         df = out.loc[out["_df_idx"] == i, cols]
         gdfs += (df,)
 
     return gdfs
 
 
-def _eliminate(gdf, to_eliminate, aggfunc, crs, fix_double, **kwargs):
+def _eliminate(
+    gdf, to_eliminate, aggfunc, crs, fix_double, grid_size, n_jobs, **kwargs
+):
     if not len(to_eliminate):
         return gdf
 
     in_to_eliminate = gdf["_dissolve_idx"].isin(to_eliminate["_dissolve_idx"])
     to_dissolve = gdf.loc[in_to_eliminate]
     not_to_dissolve = gdf.loc[~in_to_eliminate].set_index("_dissolve_idx")
 
@@ -553,49 +645,14 @@
 
         # TODO kan dette fikses trygt med .duplicated og ~x.duplicated?
         eliminators: pd.Series = many_hits.loc[
             many_hits["_to_eliminate"] != 1, "geometry"
         ]
         to_be_eliminated = many_hits.loc[many_hits["_to_eliminate"] == 1]
 
-        if 0:
-            tree = STRtree(eliminators.values)
-            left, right = tree.query(
-                to_be_eliminated.geometry.values, predicate="intersects"
-            )
-            pairs = pd.Series(right, index=left).to_frame("right")
-            pairs["_dissolve_idx"] = pairs.index.map(
-                dict(enumerate(to_be_eliminated.index))
-            )
-
-            soon_erased = to_be_eliminated.iloc[pairs.index]
-            intersecting = eliminators.iloc[pairs["right"]]
-
-            intersecting.index = soon_erased.index
-            soon_erased = soon_erased.geometry.groupby(level=0).agg(unary_union)
-            intersecting = intersecting.groupby(level=0).agg(unary_union)
-
-            soon_erased.loc[:] = difference(
-                soon_erased.values,
-                intersecting.values,
-            )
-            intersecting.loc[:] = difference(
-                intersecting.values,
-                soon_erased.values,
-            )
-
-            eliminated["geometry"] = (
-                pd.concat([intersecting, soon_erased])
-                .groupby(level=0)
-                .agg(lambda x: make_valid(unary_union(x.dropna().values)))
-            )
-            from ..maps.maps import explore, explore_locals
-
-            explore_locals()
-
         # all_geoms: pd.Series = gdf.set_index("_dissolve_idx").geometry
         all_geoms: pd.Series = gdf.geometry
 
         tree = STRtree(all_geoms.values)
         left, right = tree.query(
             to_be_eliminated.geometry.values, predicate="intersects"
         )
@@ -617,78 +674,71 @@
             # (~to_be_eliminated.index.isin(soon_erased.index))
             # |
             (~to_be_eliminated["_row_idx"].isin(soon_erased["_row_idx"])),
             # | (~to_be_eliminated["_row_idx"].isin(soon_erased.index)),
             "geometry",
         ]
 
-        if 0:
-            from ..geopandas_tools.conversion import to_gdf
-            from ..maps.maps import explore, explore_locals
-
-            display(pairs)
-            display(soon_erased.index.unique())
-            display(soon_erased._row_idx.unique())
-            display(to_be_eliminated.index.unique())
-            display(to_be_eliminated._row_idx.unique())
-            display(missing.index.unique())
-
-            display(soon_erased)
-            display(to_be_eliminated)
-            display(missing)
-
-            explore(
-                to_gdf(soon_erased, 25833), intersecting=to_gdf(intersecting, 25833)
-            )
-            for j, ((i, g), (i2, g2)) in enumerate(
-                zip(intersecting.items(), soon_erased.geometry.items())
-            ):
-                explore(
-                    to_gdf(g, 25833).assign(ii=i, j=j),
-                    g2=to_gdf(g2, 25833).assign(ii=i2, j=j),
-                )
-
-        if 0:
-            explore(to_gdf(to_be_eliminated.iloc[[16]]))
-            explore(to_gdf(to_be_eliminated.iloc[[15]]))
-            explore(to_gdf(to_be_eliminated.iloc[[0]]))
-            print("hei")
-            explore(to_gdf(soon_erased.loc[soon_erased.index == 16]))
-            explore(to_gdf(soon_erased.loc[soon_erased.index == 36]))
-
-            explore(to_gdf(soon_erased.loc[soon_erased._row_idx == 16]))
-            explore(to_gdf(soon_erased.loc[soon_erased._row_idx == 36]))
-
         # allign and aggregate by dissolve index to not get duplicates in difference
         intersecting.index = soon_erased.index
-        soon_erased = soon_erased.geometry.groupby(level=0).agg(unary_union)
-        intersecting = intersecting.groupby(level=0).agg(unary_union)
+        soon_erased = soon_erased.geometry.groupby(level=0).agg(
+            lambda x: unary_union(x, grid_size=grid_size)
+        )
+        intersecting = intersecting.groupby(level=0).agg(
+            lambda x: unary_union(x, grid_size=grid_size)
+        )
 
         # from ..maps.maps import explore_locals
         # explore_locals()
 
-        soon_erased.loc[:] = difference(
-            soon_erased.values,
-            intersecting.values,
+        soon_erased.loc[:] = _try_difference(
+            soon_erased.to_numpy(),
+            intersecting.to_numpy(),
+            grid_size=grid_size,
+            n_jobs=n_jobs,
+            geom_type="polygon",
         )
 
-        eliminated["geometry"] = (
-            pd.concat([eliminators, soon_erased, missing])
-            .groupby(level=0)
-            .agg(lambda x: make_valid(unary_union(x.dropna().values)))
-        )
+        if n_jobs > 1:
+            eliminated["geometry"] = GeoSeries(
+                parallel_unary_union_geoseries(
+                    pd.concat([eliminators, soon_erased, missing]),
+                    level=0,
+                    grid_size=grid_size,
+                    n_jobs=n_jobs,
+                ),
+                index=eliminated.index,
+            )
+        else:
+            eliminated["geometry"] = (
+                pd.concat([eliminators, soon_erased, missing])
+                .groupby(level=0)
+                .agg(
+                    lambda x: make_valid(
+                        unary_union(x.dropna().values, grid_size=grid_size)
+                    )
+                )
+            )
 
     else:
-        eliminated["geometry"] = many_hits.groupby("_dissolve_idx")["geometry"].agg(
-            lambda x: make_valid(unary_union(x.values))
-        )
+        if n_jobs > 1:
+            eliminated["geometry"] = parallel_unary_union(
+                many_hits, by="_dissolve_idx", grid_size=grid_size, n_jobs=n_jobs
+            )
+        else:
+            eliminated["geometry"] = many_hits.groupby("_dissolve_idx")["geometry"].agg(
+                lambda x: make_valid(unary_union(x.values, grid_size=grid_size))
+            )
 
     # setting crs on the GeometryArrays to avoid warning in concat
     not_to_dissolve.geometry.values.crs = crs
-    eliminated.geometry.values.crs = crs
+    try:
+        eliminated.geometry.values.crs = crs
+    except AttributeError:
+        pass
     one_hit.geometry.values.crs = crs
 
     to_concat = [not_to_dissolve, eliminated, one_hit]
 
     assert all(df.index.name == "_dissolve_idx" for df in to_concat)
 
     return pd.concat(to_concat).sort_index().drop(columns="_to_eliminate")
@@ -701,14 +751,21 @@
 
     def to_none_if_thin(geoms):
         try:
             buffered_in = buffer(
                 difference(polygons(geoms), inside_holes), -(tolerance / 2)
             )
             return np.where(is_empty(buffered_in), None, geoms)
+        except GEOSException:
+            buffered_in = buffer(
+                difference(make_valid(polygons(make_valid(geoms))), inside_holes),
+                -(tolerance / 2),
+            )
+            return np.where(is_empty(buffered_in), None, geoms)
+
         except ValueError as e:
             if not len(geoms):
                 return geoms
             raise e
 
     if not (gdf.geom_type == "Polygon").all():
         raise ValueError(gdf.geom_type.value_counts())
@@ -969,15 +1026,19 @@
                 no_islands = make_valid(unary_union(hole.difference(all_geoms)))
 
             holes_closed.append(no_islands)
 
     return make_valid(unary_union(holes_closed))
 
 
-def get_gaps(gdf: GeoDataFrame, include_interiors: bool = False) -> GeoDataFrame:
+def get_gaps(
+    gdf: GeoDataFrame,
+    include_interiors: bool = False,
+    grid_size: float | int | None = None,
+) -> GeoDataFrame:
     """Get the gaps between polygons.
 
     Args:
         gdf: GeoDataFrame of polygons.
         include_interiors: If False (default), the holes inside individual polygons
             will not be included as gaps.
 
@@ -994,15 +1055,17 @@
         gdf = close_all_holes(gdf)
 
     bbox = GeoDataFrame(
         {"geometry": [box(*tuple(gdf.total_bounds)).buffer(1)]}, crs=gdf.crs
     )
 
     bbox_diff = make_all_singlepart(
-        clean_overlay(bbox, gdf, how="difference", geom_type="polygon")
+        clean_overlay(
+            bbox, gdf, how="difference", geom_type="polygon", grid_size=grid_size
+        )
     )
 
     # remove the outer "gap", i.e. the surrounding area
     bbox_ring = get_exterior_ring(bbox.geometry.values)
     without_outer_ring = sfilter_inverse(bbox_diff, bbox_ring)
     return without_outer_ring.reset_index(drop=True)
```

### Comparing `ssb_sgis-0.3.9/src/sgis/geopandas_tools/polygons_as_rings.py` & `ssb_sgis-1.0.0/src/sgis/geopandas_tools/polygons_as_rings.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     distance,
     extract_unique_points,
     get_coordinates,
     get_exterior_ring,
     get_interior_ring,
     get_num_interior_rings,
     get_parts,
-    get_rings,
     intersection,
     intersects,
     is_empty,
     is_ring,
     length,
     line_merge,
     linearrings,
@@ -56,23 +55,39 @@
 
 from .conversion import to_gdf, to_geoseries
 
 
 class PolygonsAsRings:
     """Convert polygons to linearrings, apply linestring functions, then convert back to polygons."""
 
-    def __init__(self, polys: GeoDataFrame | GeoSeries | GeometryArray, crs=None):
+    def __init__(
+        self,
+        polys: GeoDataFrame | GeoSeries | GeometryArray,
+        crs=None,
+        allow_multipart: bool = False,
+        gridsize: int | None = None,
+    ):
         if not isinstance(polys, (pd.DataFrame, pd.Series, GeometryArray)):
             raise TypeError(type(polys))
 
         self.polyclass = polys.__class__
 
         if not isinstance(polys, pd.DataFrame):
             polys = to_gdf(polys, crs)
 
+        if not allow_multipart and not (polys.geom_type == "Polygon").all():
+            raise ValueError(
+                "All geometries must be single-type Polygons. Set allow_multipart=True to allow MultiPolygons",
+                polys.geom_type.value_counts(),
+            )
+        if not polys.geom_type.isin(["Polygon", "MultiPolygon"]).all():
+            raise ValueError(
+                f"All geometries must be Polygons. Got {polys.geom_type.value_counts()}"
+            )
+
         self._index_mapper = dict(enumerate(polys.index))
         self.gdf = polys.reset_index(drop=True)
 
         if crs is not None:
             self.crs = crs
         elif hasattr(polys, "crs"):
             self.crs = polys.crs
@@ -109,14 +124,16 @@
         interiors = interiors.dropna()
 
         self.rings = pd.concat([exterior, interiors])
 
     def get_rings(self, agg: bool = False):
         gdf = self.gdf.copy()
         rings = self.rings.copy()
+        if not len(rings):
+            return GeoSeries()
         if agg:
             gdf.geometry = rings.groupby(level=1).agg(unary_union)
         else:
             rings.index = rings.index.get_level_values(1)
             rings.name = "geometry"
             gdf = gdf.drop(columns="geometry").join(rings)
 
@@ -144,15 +161,23 @@
     def apply_numpy_func(
         self, func: Callable, args: tuple | None = None, kwargs: dict | None = None
     ):
         """Run a function that takes an array of lines/rings and returns an array of lines/rings."""
         kwargs = kwargs or {}
         args = args or ()
 
-        self.rings.loc[:] = np.array(func(self.rings.values, *args, **kwargs))
+        results = np.array(func(self.rings.values, *args, **kwargs))
+
+        if len(results) != len(self.rings):
+            raise ValueError(
+                f"Different length of results. Got {len(results)} and {len(self.rings)} original rings"
+            )
+
+        self.rings.loc[:] = results
+
         return self
 
     def apply_geoseries_func(
         self, func: Callable, args: tuple | None = None, kwargs: dict | None = None
     ):
         """Run a function that takes a GeoSeries and returns a GeoSeries."""
         kwargs = kwargs or {}
@@ -306,15 +331,15 @@
     if interiors is None:
         return (
             pd.Series(
                 make_valid(polygons(exterior.values)),
                 index=exterior.index,
             )
             .groupby(level=0)
-            .agg(unary_union)
+            .agg(lambda x: make_valid(unary_union(x)))
         )
 
     interiors.index = interiors.index.get_level_values(1)
     new_interiors = []
     for col in interiors:
         new_interiors.append(get_linearring_series(interiors[col]))
 
@@ -331,9 +356,9 @@
 
     return (
         pd.Series(
             make_valid(polygons(exterior.values, out_interiors.values)),
             index=exterior.index,
         )
         .groupby(level=0)
-        .agg(unary_union)
+        .agg(lambda x: make_valid(unary_union(x)))
     )
```

### Comparing `ssb_sgis-0.3.9/src/sgis/geopandas_tools/sfilter.py` & `ssb_sgis-1.0.0/src/sgis/geopandas_tools/sfilter.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,67 +7,14 @@
 
 from .conversion import to_gdf
 
 
 gdf_type_error_message = "'gdf' should be of type GeoDataFrame or GeoSeries."
 
 
-def _get_sfilter_indices(
-    left: GeoDataFrame | GeoSeries,
-    right: GeoDataFrame | GeoSeries | Geometry,
-    predicate: str,
-) -> np.ndarray:
-    """Compute geometric comparisons and get matching indices.
-
-    Taken from:
-    geopandas.tools.sjoin._geom_predicate_query
-
-    Parameters
-    ----------
-    left : GeoDataFrame
-    right : GeoDataFrame
-    predicate : string
-        Binary predicate to query.
-
-    Returns
-    -------
-    DataFrame
-        DataFrame with matching indices in
-        columns named `_key_left` and `_key_right`.
-    """
-    original_predicate = predicate
-
-    with warnings.catch_warnings():
-        # We don't need to show our own warning here
-        # TODO remove this once the deprecation has been enforced
-        warnings.filterwarnings(
-            "ignore", "Generated spatial index is empty", FutureWarning
-        )
-
-        if predicate == "within":
-            # within is implemented as the inverse of contains
-            # contains is a faster predicate
-            # see discussion at https://github.com/geopandas/geopandas/pull/1421
-            predicate = "contains"
-            sindex = left.sindex
-            input_geoms = right.geometry if isinstance(right, GeoDataFrame) else right
-        else:
-            # all other predicates are symmetric
-            # keep them the same
-            sindex = right.sindex
-            input_geoms = left.geometry if isinstance(left, GeoDataFrame) else left
-
-    l_idx, r_idx = sindex.query(input_geoms, predicate=predicate, sort=False)
-
-    if original_predicate == "within":
-        return np.unique(r_idx)
-
-    return np.unique(l_idx)
-
-
 def sfilter(
     gdf: GeoDataFrame | GeoSeries,
     other: GeoDataFrame | GeoSeries | Geometry,
     predicate: str = "intersects",
 ) -> GeoDataFrame:
     """Filter a GeoDataFrame or GeoSeries by spatial predicate.
 
@@ -286,7 +233,60 @@
 
         try:
             other = other.set_crs(crs)
         except ValueError as e:
             raise ValueError("crs mismatch", crs, other.crs) from e
 
     return other
+
+
+def _get_sfilter_indices(
+    left: GeoDataFrame | GeoSeries,
+    right: GeoDataFrame | GeoSeries | Geometry,
+    predicate: str,
+) -> np.ndarray:
+    """Compute geometric comparisons and get matching indices.
+
+    Taken from:
+    geopandas.tools.sjoin._geom_predicate_query
+
+    Parameters
+    ----------
+    left : GeoDataFrame
+    right : GeoDataFrame
+    predicate : string
+        Binary predicate to query.
+
+    Returns
+    -------
+    DataFrame
+        DataFrame with matching indices in
+        columns named `_key_left` and `_key_right`.
+    """
+    original_predicate = predicate
+
+    with warnings.catch_warnings():
+        # We don't need to show our own warning here
+        # TODO remove this once the deprecation has been enforced
+        warnings.filterwarnings(
+            "ignore", "Generated spatial index is empty", FutureWarning
+        )
+
+        if predicate == "within":
+            # within is implemented as the inverse of contains
+            # contains is a faster predicate
+            # see discussion at https://github.com/geopandas/geopandas/pull/1421
+            predicate = "contains"
+            sindex = left.sindex
+            input_geoms = right.geometry if isinstance(right, GeoDataFrame) else right
+        else:
+            # all other predicates are symmetric
+            # keep them the same
+            sindex = right.sindex
+            input_geoms = left.geometry if isinstance(left, GeoDataFrame) else left
+
+    l_idx, r_idx = sindex.query(input_geoms, predicate=predicate, sort=False)
+
+    if original_predicate == "within":
+        return np.sort(np.unique(r_idx))
+
+    return np.sort(np.unique(l_idx))
```

### Comparing `ssb_sgis-0.3.9/src/sgis/helpers.py` & `ssb_sgis-1.0.0/src/sgis/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -215,14 +215,22 @@
     df["_idx"] = range(len(df))
 
     df = df.sort_values(["n_nan", "_idx"]).drop(columns=["n_nan", "_idx"])
 
     return df.reset_index(drop=True) if ignore_index else df
 
 
+def is_number(text) -> bool:
+    try:
+        float(text)
+        return True
+    except ValueError:
+        return False
+
+
 class LocalFunctionError(ValueError):
     def __init__(self, func: str):
         self.func = func.__name__
 
     def __str__(self):
         return (
             f"{self.func}. "
```

### Comparing `ssb_sgis-0.3.9/src/sgis/io/dapla_functions.py` & `ssb_sgis-1.0.0/src/sgis/io/dapla_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Functions for reading and writing GeoDataFrames in Statistics Norway's GCS Dapla.
 """
+
 from pathlib import Path
 from typing import Optional
 
 import dapla as dp
 import geopandas as gpd
 import pandas as pd
 from geopandas import GeoDataFrame
@@ -11,15 +12,15 @@
 from pandas import DataFrame
 from pyarrow import parquet
 
 
 def read_geopandas(
     gcs_path: str | Path,
     pandas_fallback: bool = False,
-    fs: Optional[dp.gcs.GCSFileSystem] = None,
+    file_system: Optional[dp.gcs.GCSFileSystem] = None,
     **kwargs,
 ) -> GeoDataFrame | DataFrame:
     """Reads geoparquet or other geodata from a file on GCS.
 
     If the file has 0 rows, the contents will be returned as a pandas.DataFrame,
     since geopandas does not read and write empty tables.
 
@@ -40,46 +41,51 @@
 
     if not isinstance(gcs_path, str):
         try:
             gcs_path = str(gcs_path)
         except TypeError:
             raise TypeError(f"Unexpected type {type(gcs_path)}.")
 
-    if fs is None:
-        fs = dp.FileClient.get_gcs_file_system()
+    if file_system is None:
+        file_system = dp.FileClient.get_gcs_file_system()
 
     if "parquet" in gcs_path or "prqt" in gcs_path:
-        with fs.open(gcs_path, mode="rb") as file:
+        with file_system.open(gcs_path, mode="rb") as file:
             try:
                 return gpd.read_parquet(file, **kwargs)
             except ValueError as e:
+                if "Missing geo metadata" not in str(e) and "geometry" not in str(e):
+                    raise e
                 df = dp.read_pandas(gcs_path, **kwargs)
 
                 if pandas_fallback or not len(df):
                     return df
                 else:
                     raise e
     else:
-        with fs.open(gcs_path, mode="rb") as file:
+        with file_system.open(gcs_path, mode="rb") as file:
             try:
                 return gpd.read_file(file, **kwargs)
             except ValueError as e:
+                if "Missing geo metadata" not in str(e) and "geometry" not in str(e):
+                    raise e
                 df = dp.read_pandas(gcs_path, **kwargs)
 
                 if pandas_fallback or not len(df):
                     return df
                 else:
                     raise e
 
 
 def write_geopandas(
     df: gpd.GeoDataFrame,
     gcs_path: str | Path,
     overwrite: bool = True,
-    fs: Optional[dp.gcs.GCSFileSystem] = None,
+    pandas_fallback: bool = False,
+    file_system: Optional[dp.gcs.GCSFileSystem] = None,
     **kwargs,
 ) -> None:
     """Writes a GeoDataFrame to the speficied format.
 
     Note:
         Does not currently write to shapelfile or filegeodatabase.
 
@@ -96,32 +102,30 @@
             gcs_path = str(gcs_path)
         except TypeError as e:
             raise TypeError(f"Unexpected type {type(gcs_path)}.") from e
 
     if not overwrite and exists(gcs_path):
         raise ValueError("File already exists.")
 
-    if fs is None:
-        fs = dp.FileClient.get_gcs_file_system()
+    if file_system is None:
+        file_system = dp.FileClient.get_gcs_file_system()
 
     pd.io.parquet.BaseImpl.validate_dataframe(df)
 
     if not len(df):
-        try:
-            dp.write_pandas(df, gcs_path, **kwargs)
-        except Exception:
-            dp.write_pandas(
-                df.drop(df._geometry_column_name, axis=1), gcs_path, **kwargs
-            )
+        if pandas_fallback:
+            df.geometry = df.geometry.astype(str)
+            df = pd.DataFrame(df)
+        dp.write_pandas(df, gcs_path, **kwargs)
         return
 
-    fs = dp.FileClient.get_gcs_file_system()
+    file_system = dp.FileClient.get_gcs_file_system()
 
     if ".parquet" in gcs_path or "prqt" in gcs_path:
-        with fs.open(gcs_path, mode="wb") as buffer:
+        with file_system.open(gcs_path, mode="wb") as buffer:
             table = _geopandas_to_arrow(df, index=df.index, schema_version=None)
             parquet.write_table(table, buffer, compression="snappy", **kwargs)
         return
 
     layer = kwargs.pop("layer", None)
     if ".gpkg" in gcs_path:
         driver = "GPKG"
@@ -131,30 +135,30 @@
     elif ".gml" in gcs_path:
         driver = "GML"
     elif ".shp" in gcs_path:
         driver = "ESRI Shapefile"
     else:
         driver = None
 
-    with fs.open(gcs_path, "wb") as file:
+    with file_system.open(gcs_path, "wb") as file:
         df.to_file(file, driver=driver, layer=layer)
 
 
 def exists(path: str | Path) -> bool:
     """Returns True if the path exists, and False if it doesn't.
 
     Args:
         path (str): The path to the file or directory.
 
     Returns:
         True if the path exists, False if not.
     """
 
-    fs = dp.FileClient.get_gcs_file_system()
-    return fs.exists(path)
+    file_system = dp.FileClient.get_gcs_file_system()
+    return file_system.exists(path)
 
 
 def check_files(
     folder: str,
     contains: str | None = None,
     within_minutes: int | None = None,
 ) -> pd.DataFrame:
@@ -162,18 +166,18 @@
 
     Args:
         folder: Google cloud storage folder.
         contains: Optional substring that must be in the file path.
         within_minutes: Optionally include only files that were updated in the
             last n minutes.
     """
-    fs = dp.FileClient.get_gcs_file_system()
+    file_system = dp.FileClient.get_gcs_file_system()
 
     # (recursive doesn't work, so doing recursive search below)
-    info = fs.ls(folder, detail=True, recursive=True)
+    info = file_system.ls(folder, detail=True, recursive=True)
 
     if not info:
         return pd.DataFrame(columns=["kb", "mb", "name", "child", "path"])
 
     fileinfo = [
         (x["name"], x["size"], x["updated"])
         for x in info
@@ -217,25 +221,25 @@
         return df[["kb", "mb", "name", "child", "path"]]
 
     the_time = pd.Timestamp.now() - pd.Timedelta(minutes=within_minutes)
     return df.loc[lambda x: x.index > the_time, ["kb", "mb", "name", "child", "path"]]
 
 
 def get_files_in_subfolders(folderinfo: list[dict]) -> list[dict]:
-    fs = dp.FileClient.get_gcs_file_system()
+    file_system = dp.FileClient.get_gcs_file_system()
 
     if isinstance(folderinfo, (str, Path)):
         folderinfo = [folderinfo]
 
     fileinfo = []
 
     while folderinfo:
         new_folderinfo = []
         for m in folderinfo:
-            more_info = fs.ls(m, detail=True, recursive=True)
+            more_info = file_system.ls(m, detail=True, recursive=True)
             if not more_info:
                 continue
 
             more_fileinfo = [
                 (x["name"], x["size"], x["updated"])
                 for x in more_info
                 if x["storageClass"] != "DIRECTORY"
```

### Comparing `ssb_sgis-0.3.9/src/sgis/io/opener.py` & `ssb_sgis-1.0.0/src/sgis/io/opener.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 except ImportError:
     pass
 
 from ._is_dapla import is_dapla
 
 
 @contextmanager
-def opener(path, mode="rb"):
+def opener(path, mode="rb", file_system=None):
     """Yields a gcs buffer if in Dapla, otherwise yields the path.
 
     Example
     -------
     >>> with opener(path) as file:
     >>>     with rasterio.open(file) as src:
     >>>         array = src.read()
     """
     if is_dapla():
-        fs = dp.FileClient.get_gcs_file_system()
-        yield fs.open(str(path), mode=mode)
+        if file_system is None:
+            file_system = dp.FileClient.get_gcs_file_system()
+        yield file_system.open(str(path), mode=mode)
     else:
         yield str(path)
```

### Comparing `ssb_sgis-0.3.9/src/sgis/io/read_parquet.py` & `ssb_sgis-1.0.0/src/sgis/io/read_parquet.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/src/sgis/maps/examine.py` & `ssb_sgis-1.0.0/src/sgis/maps/examine.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import geopandas as gpd
 import numpy as np
 
 from ..geopandas_tools.bounds import get_total_bounds
 from ..helpers import unit_is_degrees
+from .map import Map
 from .maps import clipmap, explore, samplemap
 
 
 class Examine:
     """Explore geometries one row at a time.
 
     It takes one or more GeoDataFrames and shows an interactive map
@@ -71,31 +72,34 @@
     def __init__(
         self,
         *gdfs: gpd.GeoDataFrame,
         column: str | None = None,
         mask_gdf: gpd.GeoDataFrame | None = None,
         sort_values: str | None = None,
         size: int | float = 1000,
-        only_show_mask: bool = False,
+        only_show_mask: bool = True,
         **kwargs,
     ):
-        if not all(isinstance(gdf, gpd.GeoDataFrame) or not len(gdf) for gdf in gdfs):
-            raise ValueError("gdfs must be of type GeoDataFrame.")
+        gdfs, column, kwargs = Map._separate_args(gdfs, column, kwargs)
 
-        self._gdfs = gdfs
         if mask_gdf is None:
             self.mask_gdf = gdfs[0]
         else:
             self.mask_gdf = mask_gdf
 
+        m = Map(*gdfs, column=column, **kwargs)
+        self._gdfs: dict[str, gpd.GeoDataFrame] = dict(zip(m.labels, m.gdfs))
+
         self.indices = list(range(len(self.mask_gdf)))
         self.i = 0
         self.column = column
         self.size = size
-        self.kwargs = kwargs
+        self.kwargs = {
+            key: value for key, value in kwargs.items() if key not in self._gdfs
+        }
 
         if not len(self.mask_gdf):
             return
 
         if unit_is_degrees(self.mask_gdf) and size > 360:
             raise ValueError(
                 "CRS unit is degrees. Use geopandas' "
@@ -109,22 +113,17 @@
                 or not isinstance(sort_values, str)
                 and "area" in sort_values
             ):
                 self.mask_gdf["area"] = self.mask_gdf.area
             self.mask_gdf = self.mask_gdf.sort_values(sort_values)
 
         if only_show_mask:
-            self.kwargs["show"] = [True] + [False] * len(self._gdfs[1:])
-        elif not kwargs.get("show"):
-            self.kwargs["show"] = [True] * len(self._gdfs)
-
-    def add_gdfs(self, *gdfs):
-        self._gdfs = self._gdfs + gdfs
-        self.kwargs["show"] += [True for _ in range(len(gdfs))]
-        return self
+            self.kwargs["show"] = [True] + [False] * (len(self._gdfs) - 1)
+        elif not kwargs.get("show", True):
+            self.kwargs["show"] = [False] * len(self._gdfs)
 
     def next(self, i: int | None = None, **kwargs):
         """Displays a map of geometries within the next row of the mask gdf.
 
         Args:
             i: Index to display.
             **kwargs: Additional keyword arguments passed to sgis.clipmap.
@@ -141,16 +140,16 @@
 
         if self.i >= len(self.mask_gdf):
             print("All rows are shown.")
             return
 
         print(f"i == {self.i} (of {len(self.mask_gdf)})")
         clipmap(
-            *self._gdfs,
             self.column,
+            **self._gdfs,
             mask=self.mask_gdf.iloc[[self.i]].buffer(self.size),
             **self.kwargs,
         )
         self.i += 1
 
     def sample(self, **kwargs):
         """Takes a sample index of the mask and displays a map of this area.
@@ -162,16 +161,16 @@
             kwargs = self._fix_kwargs(kwargs)
             self.kwargs = self.kwargs | kwargs
 
         i = np.random.randint(0, len(self.mask_gdf))
 
         print(f"Showing index {i}")
         clipmap(
-            *self._gdfs,
             self.column,
+            **self._gdfs,
             mask=self.mask_gdf.iloc[[i]].buffer(self.size),
             **self.kwargs,
         )
 
     def current(self, i: int | None = None, **kwargs):
         """Repeat the last shown map."""
         if kwargs:
@@ -181,73 +180,73 @@
         if i and i < 0:
             self.i -= i
         elif i:
             self.i = i
 
         print(f"{self.i + 1} of {len(self.mask_gdf)}")
         clipmap(
-            *self._gdfs,
             self.column,
+            **self._gdfs,
             mask=self.mask_gdf.iloc[[self.i]].buffer(self.size),
             **self.kwargs,
         )
 
     def explore(self, **kwargs):
         """Show all rows like the function explore."""
         if kwargs:
             kwargs = self._fix_kwargs(kwargs)
             self.kwargs = self.kwargs | kwargs
 
         explore(
-            *self._gdfs,
-            self.column,
+            **self._gdfs,
+            column=self.column,
             **self.kwargs,
         )
 
     def clipmap(self, **kwargs):
         """Show all rows like the function clipmap."""
         if kwargs:
             kwargs = self._fix_kwargs(kwargs)
             self.kwargs = self.kwargs | kwargs
 
         clipmap(
-            *self._gdfs,
-            self.column,
+            **self._gdfs,
+            column=self.column,
             **self.kwargs,
         )
 
     def samplemap(self, **kwargs):
         """Show all rows like the function samplemap."""
         if kwargs:
             kwargs = self._fix_kwargs(kwargs)
             self.kwargs = self.kwargs | kwargs
 
         samplemap(
-            *self._gdfs,
-            self.column,
+            **self._gdfs,
+            column=self.column,
             **self.kwargs,
         )
 
     @property
     def mask(self) -> gpd.GeoDataFrame:
         """Returns a GeoDataFrame of the last shown mask geometry."""
         return self.mask_gdf.iloc[[self.i]]
 
     @property
-    def gdfs(self) -> tuple[gpd.GeoDataFrame]:
+    def gdfs(self) -> dict[str, gpd.GeoDataFrame]:
         """Returns all GeoDataFrames in the area of the last shown mask geometry."""
         mask = self.mask_gdf.iloc[[self.i]]
-        gdfs = ()
-        for gdf in self._gdfs:
-            gdfs = gdfs + (gdf.clip(mask.buffer(self.size)),)
+        gdfs = {}
+        for label, gdf in self._gdfs.items():
+            gdfs[label] = gdf.clip(mask.buffer(self.size))
         return gdfs
 
     @property
     def bounds(self):
-        return get_total_bounds(*self.gdfs)
+        return get_total_bounds(*list(self.gdfs.values()))
 
     def _fix_kwargs(self, kwargs) -> dict:
         self.size = kwargs.pop("size", self.size)
         self.column = kwargs.pop("column", self.column)
         return kwargs
 
     def __repr__(self) -> str:
```

### Comparing `ssb_sgis-0.3.9/src/sgis/maps/explore.py` & `ssb_sgis-1.0.0/src/sgis/maps/explore.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,49 @@
 """Interactive map of one or more GeoDataFrames with layers that can be toggles on/off.
 
 This module holds the Explore class, which is the basis for the explore, samplemap and
 clipmap functions from the 'maps' module.
 """
+
 import os
 import warnings
 from collections.abc import Iterable
 from numbers import Number
 from statistics import mean
 
 import branca as bc
 import folium
 import matplotlib
 import numpy as np
 import pandas as pd
 import xyzservices
 from folium import plugins
-from geopandas import GeoDataFrame
+from geopandas import GeoDataFrame, GeoSeries
 from IPython.display import display
 from jinja2 import Template
 from pandas.api.types import is_datetime64_any_dtype
 from shapely import Geometry
 from shapely.geometry import LineString
 
-from ..geopandas_tools.conversion import to_gdf
+from ..geopandas_tools.conversion import from_4326, to_gdf
 from ..geopandas_tools.general import clean_geoms, make_all_singlepart
 from ..geopandas_tools.geometry_types import get_geom_type, to_single_geom_type
 from .httpserver import run_html_server
 from .map import Map
 from .tilesources import kartverket, xyz
 
 
+try:
+    from torchgeo.datasets.geo import RasterDataset
+except ImportError:
+
+    class RasterDataset:
+        """Placeholder"""
+
+
 # the geopandas._explore raises a deprication warning. Ignoring for now.
 warnings.filterwarnings(
     action="ignore", category=matplotlib.MatplotlibDeprecationWarning
 )
 pd.options.mode.chained_assignment = None
 
 
@@ -99,14 +108,15 @@
             "OpenStreetMap", min_zoom=0, max_zoom=max_zoom
         ),
         "grunnkart": kartverket.norges_grunnkart,
         "gråtone": kartverket.norges_grunnkart_gråtone,
         "norge_i_bilder": kartverket.norge_i_bilder,
         "dark": xyz.CartoDB.DarkMatter,
         "voyager": xyz.CartoDB.Voyager,
+        "strava": xyz.Strava.All,
     }
     try:
         name = tile["name"]
     except TypeError:
         name = tile
 
     if not isinstance(tile, str):
@@ -133,51 +143,69 @@
             attr = None
 
     return folium.TileLayer(provider, name=name, attr=attr, max_zoom=max_zoom)
 
 
 class Explore(Map):
     # class attribute that can be overridden locally
-    tiles = ("OpenStreetMap", "dark", "norge_i_bilder", "grunnkart")
+    tiles = (
+        "grunnkart",
+        "norge_i_bilder",
+        "dark",
+        "OpenStreetMap",
+    )
 
     def __init__(
         self,
         *gdfs,
+        mask=None,
         column: str | None = None,
         popup: bool = True,
-        max_zoom: int = 30,
+        max_zoom: int = 40,
         smooth_factor: float = 1.5,
         browser: bool = False,
         prefer_canvas: bool = True,
         measure_control: bool = True,
-        geocoder: bool = True,
+        geocoder: bool = False,
         save=None,
         show: bool | Iterable[bool] | None = None,
+        text: str | None = None,
+        decimals: int = 6,
         **kwargs,
     ):
         self.popup = popup
         self.max_zoom = max_zoom
         self.smooth_factor = smooth_factor
         self.prefer_canvas = prefer_canvas
         self.measure_control = measure_control
         self.geocoder = geocoder
         self.save = save
+        self.mask = mask
+        self.text = text
+        self.decimals = decimals
 
         self.browser = browser
         if not self.browser and "show_in_browser" in kwargs:
             self.browser = kwargs.pop("show_in_browser")
         if not self.browser and "in_browser" in kwargs:
             self.browser = kwargs.pop("in_browser")
 
         if show is None:
             show_was_none = True
             show = True
         else:
             show_was_none = False
 
+        self.raster_datasets = tuple(
+            raster_dataset_to_background_map(x)
+            for x in gdfs
+            if isinstance(x, RasterDataset)
+        )
+        self.tiles  # += self.raster_datasets
+
         super().__init__(*gdfs, column=column, show=show, **kwargs)
 
         if self.gdfs is None:
             return
 
         # stringify or remove columns not renerable by leaflet (list, geometry etc.)
         new_gdfs, show_new = [], []
@@ -228,25 +256,33 @@
                 self._cmap = "viridis"
             self.cmap_start = kwargs.pop("cmap_start", 0)
             self.cmap_stop = kwargs.pop("cmap_stop", 256)
 
         if self._gdf.crs is None:
             self.kwargs["crs"] = "Simple"
 
+        self.original_crs = self.gdf.crs
+
+    def __repr__(self):
+        return f"{self.__class__.__name__}()"
+
     def explore(
         self, column: str | None = None, center=None, size=None, **kwargs
     ) -> None:
-        if not any(len(gdf) for gdf in self._gdfs):
+        if not any(len(gdf) for gdf in self._gdfs) and not len(self.raster_datasets):
             warnings.warn("None of the GeoDataFrames have rows.")
             return
         if column:
             self._column = column
             self._update_column()
             kwargs.pop("column", None)
 
+        if self.mask is not None:
+            return self.clipmap(mask=self.mask, column=self._column, **kwargs)
+
         if center is None:
             self.to_show = self._gdfs
             self._explore(**kwargs)
             return
 
         size = size if size else 1000
 
@@ -510,14 +546,17 @@
         if "tooltip" in self.kwargs:
             tooltip = self.kwargs.pop("tooltip")
             return tooltip
         return [col for col in gdf.columns if col not in COLS_TO_DROP]
 
     @staticmethod
     def _prepare_gdf_for_map(gdf):
+        if isinstance(gdf, GeoSeries):
+            gdf = gdf.to_frame("geometry")
+
         # convert LinearRing to LineString
         rings_mask = gdf.geom_type == "LinearRing"
         if rings_mask.any():
             gdf.geometry[rings_mask] = gdf.geometry[rings_mask].apply(
                 lambda g: LineString(g)
             )
 
@@ -592,20 +631,24 @@
             **map_kwds,
         )
 
         self._add_tiles(m, more_tiles)
 
         if self.measure_control:
             MeasureControlFix(
-                primary_length_unit="meters",
+                primary_length_unit="m",
                 secondary_length_unit="kilometers",
                 primary_area_unit="sqmeters",
                 secondary_area_unit="sqkilometers",
                 position="bottomleft",
                 capture_z_index=False,
+                thousands_sep="",
+                units={
+                    "m": {"factor": 1, "display": "m", "decimals": self.decimals},
+                },
             ).add_to(m)
 
         plugins.Fullscreen(
             position="topleft",
             title="Expand me",
             title_cancel="Exit me",
             force_separate_button=True,
@@ -622,14 +665,20 @@
         if self.geocoder:
             plugins.Geocoder(position="topright").add_to(m)
 
         # fit bounds to get a proper zoom level
         if fit and "zoom_start" not in kwargs:
             m.fit_bounds([[bounds[1], bounds[0]], [bounds[3], bounds[2]]])
 
+        if self.text:
+            style = bc.element.MacroElement()
+            style._template = bc.element.Template(get_textbox(self.text))
+            m.get_root().add_child(style)
+            # folium.LayerControl(collapsed=False).add_to(m)
+
         return m
 
     def _make_geojson(
         self,
         df,
         show: bool,
         color=None,
@@ -789,14 +838,19 @@
     fields = list(map(str, fields))
     if type == "tooltip":
         return folium.GeoJsonTooltip(fields, **kwds)
     elif type == "popup":
         return folium.GeoJsonPopup(fields, **kwds)
 
 
+def raster_dataset_to_background_map(dataset: RasterDataset):
+    crs = dataset.crs
+    bbox = dataset.bounds
+
+
 def _categorical_legend(m, title, categories, colors):
     """
     Add categorical legend to a map
 
     The implementation is using the code originally written by Michel Metran
     (@michelmetran) and released on GitHub
     (https://github.com/michelmetran/package_folium) under MIT license.
@@ -903,7 +957,63 @@
         </div>
     </div>
     """
 
     # Add Body
     body = bc.element.Element(body, "legend")
     m.get_root().html.add_child(body)
+
+
+def get_textbox(text: str) -> str:
+    return f"""
+{{% macro html(this, kwargs) %}}
+<!doctype html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+    <meta name="viewport" content="width=device-width, initial-scale=1">
+    <title>Textbox Project</title>
+    <link rel="stylesheet" href="//code.jquery.com/ui/1.12.1/themes/base/jquery-ui.css">
+    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.2.1/css/all.min.css" integrity="sha512-MV7K8+y+gLIBoVD59lQIYicR65iaqukzvf/nwasF0nqhPay5w/9lJmVM2hMDcnK1OnMGCdVK+iQrJ7lzPJQd1w==" crossorigin="anonymous" referrerpolicy="no-referrer"/>
+    <script src="https://code.jquery.com/jquery-1.12.4.js"></script>
+    <script src="https://code.jquery.com/ui/1.12.1/jquery-ui.js"></script>
+
+    <script>
+      $( function() {{
+        $( "#textbox" ).draggable({{
+          start: function (event, ui) {{
+            $(this).css({{
+              right: "auto",
+              top: "auto",
+              bottom: "auto"
+            }});
+          }}
+        }});
+      }});
+    </script>
+  </head>
+
+  <body>
+    <div id="textbox" class="textbox">
+      <div class="textbox-content">
+        <p>{text}</p>
+      </div>
+    </div>
+
+</body>
+</html>
+
+<style type='text/css'>
+  .textbox {{
+    position: absolute;
+    z-index:9999;
+    border-radius:4px;
+    background: white;
+    padding: 1px;
+    font-size:11px;
+    left: 20px;
+    top: 50%;
+    color: black;
+  }}
+</style>
+{{% endmacro %}}
+"""
```

### Comparing `ssb_sgis-0.3.9/src/sgis/maps/httpserver.py` & `ssb_sgis-1.0.0/src/sgis/maps/httpserver.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/src/sgis/maps/legend.py` & `ssb_sgis-1.0.0/src/sgis/maps/legend.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/src/sgis/maps/map.py` & `ssb_sgis-1.0.0/src/sgis/maps/map.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Interactive or static map of one or more GeoDataFrames.
 
 This module holds the Map class, which is the basis for the Explore class.
 """
+
 import warnings
 
 import matplotlib
 import matplotlib.colors as colors
 import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame, GeoSeries
@@ -19,14 +20,22 @@
     drop_inactive_geometry_columns,
     get_common_crs,
     rename_geometry_if,
 )
 from ..helpers import get_object_name
 
 
+try:
+    from torchgeo.datasets.geo import RasterDataset
+except ImportError:
+
+    class RasterDataset:
+        """Placeholder"""
+
+
 # the geopandas._explore raises a deprication warning. Ignoring for now.
 warnings.filterwarnings(
     action="ignore", category=matplotlib.MatplotlibDeprecationWarning
 )
 pd.options.mode.chained_assignment = None
 
 
@@ -79,14 +88,15 @@
         k: int = 5,
         bins: tuple[float] | None = None,
         nan_label: str = "Missing",
         nan_color="#c2c2c2",
         scheme: str = DEFAULT_SCHEME,
         **kwargs,
     ):
+
         gdfs, column, kwargs = self._separate_args(gdfs, column, kwargs)
 
         self._column = column
         self.bins = bins
         self._k = k
         self.nan_label = nan_label
         self.nan_color = nan_color
@@ -111,57 +121,77 @@
         self.labels = labels
         if not self.labels:
             self._get_labels(gdfs)
 
         show = kwargs.pop("show", True)
         if isinstance(show, (int, bool)):
             show_temp = [bool(show) for _ in range(len(gdfs))]
-        elif not hasattr(show, "__iter__") or len(show) != len(gdfs):
+        elif not hasattr(show, "__iter__"):
             raise ValueError(
-                "'show' must be boolean or an iterable of boleans same length as gdfs"
+                "'show' must be boolean or an iterable of boleans same "
+                f"length as gdfs ({len(gdfs)}). Got len {len(show)}"
             )
         else:
             show_temp = show
 
+        show_args = show_temp[: len(gdfs)]
+        show_kwargs = show_temp[len(gdfs) :]
         self._gdfs = []
         new_labels = []
         self.show = []
-        for label, gdf, show in zip(self.labels, gdfs, show_temp, strict=True):
+        for label, gdf, show in zip(self.labels, gdfs, show_args):
             if not len(gdf):
                 continue
 
             gdf = clean_geoms(gdf).reset_index(drop=True)
             if not len(gdf):
                 continue
 
             self._gdfs.append(gdf)
             new_labels.append(label)
             self.show.append(show)
         self.labels = new_labels
 
-        if len(self._gdfs):
-            last_show = self.show[-1]
-        else:
-            last_show = show
+        # if len(self._gdfs):
+        #     last_show = self.show[-1]
+        # else:
+        #     last_show = show
 
         # pop all geometry-like items from kwargs into self._gdfs
         self.kwargs = {}
+        i = 0
         for key, value in kwargs.items():
-            if isinstance(value, GeoDataFrame):
-                self._gdfs.append(value)
-                self.labels.append(key)
-                self.show.append(last_show)
-                continue
+            # if isinstance(value, GeoDataFrame):
+            #     self._gdfs.append(value)
+            #     self.labels.append(key)
+            #     try:
+            #         show = show_kwargs[i]
+            #     except IndexError:
+            #         pass
+            #     self.show.append(show)
+            #     i += 1
+            #     continue
             try:
                 self._gdfs.append(to_gdf(value))
                 self.labels.append(key)
-                self.show.append(last_show)
+                try:
+                    show = show_kwargs[i]
+                    i += 1
+                except IndexError:
+                    pass
+                self.show.append(show)
             except Exception:
                 self.kwargs[key] = value
 
+        if hasattr(self.show, "__iter__") and len(self.show) != len(self._gdfs):
+            raise ValueError(
+                "'show' must be boolean or an iterable of boleans same "
+                f"length as gdfs ({len(gdfs)}). Got len {len(show)}"
+            )
+
         if not any(len(gdf) for gdf in self._gdfs):
             warnings.warn("None of the GeoDataFrames have rows.")
             self._gdfs = None
             self._is_categorical = True
             self._unique_values = []
             return
 
@@ -302,38 +332,40 @@
         def as_dict(obj):
             if hasattr(obj, "__dict__"):
                 return obj.__dict__
             elif isinstance(obj, dict):
                 return obj
             raise TypeError
 
-        gdfs: tuple[GeoDataFrame] = ()
+        allowed_types = (GeoDataFrame, GeoSeries, Geometry, RasterDataset)
+
+        gdfs: tuple[GeoDataFrame | GeoSeries | Geometry | RasterDataset] = ()
         for arg in args:
             if isinstance(arg, str):
                 if column is None:
                     column = arg
                 else:
                     raise ValueError(
                         "Can specify at most one string as a positional argument."
                     )
-            elif isinstance(arg, (GeoDataFrame, GeoSeries, Geometry)):
+            elif isinstance(arg, allowed_types):
                 gdfs = gdfs + (arg,)
             elif isinstance(arg, dict) or hasattr(arg, "__dict__"):
                 # add dicts or classes with GeoDataFrames to kwargs
                 more_gdfs = {}
                 for key, value in as_dict(arg).items():
-                    if isinstance(value, (GeoDataFrame, GeoSeries, Geometry)):
+                    if isinstance(value, allowed_types):
                         more_gdfs[key] = value
                     elif isinstance(value, dict) or hasattr(value, "__dict__"):
                         try:
                             # same as above, one level down
                             more_gdfs |= {
                                 k: v
                                 for k, v in value.items()
-                                if isinstance(v, (GeoDataFrame, GeoSeries, Geometry))
+                                if isinstance(v, allowed_types)
                             }
                         except Exception:
                             # no need to raise here
                             pass
 
                 kwargs |= more_gdfs
```

### Comparing `ssb_sgis-0.3.9/src/sgis/maps/maps.py` & `ssb_sgis-1.0.0/src/sgis/maps/maps.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,39 +4,52 @@
 interactive map with layers that can be toggled on and off. The 'samplemap' and
 'clipmap' functions do the same, but displays a random and chosen area respectfully.
 
 The 'qtm' function shows a simple static map of one or more GeoDataFrames.
 """
 
 import inspect
-import warnings
 from numbers import Number
 from typing import Any
 
 from geopandas import GeoDataFrame, GeoSeries
+from pyproj import CRS
 from shapely import Geometry
 
 from ..geopandas_tools.conversion import to_gdf as to_gdf_func
-from ..geopandas_tools.general import clean_clip, clean_geoms, is_wkt
+from ..geopandas_tools.general import clean_geoms, get_common_crs, is_wkt
 from ..geopandas_tools.geocoding import address_to_gdf
 from ..geopandas_tools.geometry_types import get_geom_type
-from ..helpers import make_namedict
 from .explore import Explore
 from .map import Map
 from .thematicmap import ThematicMap
 
 
+try:
+    from torchgeo.datasets.geo import RasterDataset
+except ImportError:
+
+    class RasterDataset:
+        """Placeholder"""
+
+
 def _get_location_mask(kwargs: dict, gdfs) -> tuple[GeoDataFrame | None, dict]:
     try:
-        crs = gdfs[0].crs
+        crs = get_common_crs(gdfs)
     except IndexError:
-        crs = [x for x in kwargs.values() if isinstance(x, GeoDataFrame)][0].crs
+        for x in kwargs.values():
+            try:
+                crs = CRS(x.crs) if hasattr(x, "crs") else CRS(x["crs"])
+                break
+            except Exception:
+                crs = None
 
     masks = {
         "bygdoy": (10.6976899, 59.9081695),
+        "akersveien": (10.7476367, 59.9222191),
         "kongsvinger": (12.0035242, 60.1875279),
         "stavanger": (5.6960601, 58.8946196),
         "volda": (6.0705987, 62.146643),
     }
 
     if "size" in kwargs and kwargs["size"] is not None:
         size = kwargs["size"]
@@ -55,16 +68,17 @@
     return None, kwargs
 
 
 def explore(
     *gdfs: GeoDataFrame | dict[str, GeoDataFrame],
     column: str | None = None,
     center: Any | None = None,
+    center_4326: Any | None = None,
     labels: tuple[str] | None = None,
-    max_zoom: int = 30,
+    max_zoom: int = 40,
     browser: bool = False,
     smooth_factor: int | float = 1.5,
     size: int | None = None,
     **kwargs,
 ) -> None:
     """Interactive map of GeoDataFrames with layers that can be toggled on/off.
 
@@ -102,27 +116,31 @@
     See also
     --------
     samplemap: same functionality, but shows only a random area of a given size.
     clipmap: same functionality, but shows only the areas clipped by a given mask.
 
     Examples
     --------
-    >>> from sgis import read_parquet_url, explore
-    >>> roads = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_eidskog_2022.parquet")
-    >>> points = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_eidskog.parquet")
+    >>> import sgis as sg
+    >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
+    >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
 
-    Simple explore of two GeoDataFrames.
+    Explore the area 500 meter around a given point. Coordinates are in UTM 33 format (25833).
 
-    >>> explore(roads, points)
+    >>> sg.explore(roads, points, center=(262274.6528, 6650143.176, 500))
+
+    Same as above, but with coordinates given as WGS84, same as the coordinates displayed in the corner of the map.
+
+    >>> sg.explore(roads, points, center_4326=(10.7463, 59.92, 500))
 
     With additional arguments.
 
     >>> roads["meters"] = roads.length
     >>> points["meters"] = points.length
-    >>> explore(roads, points, column="meters", cmap="plasma", max_zoom=60)
+    >>> sg.explore(roads, points, column="meters", cmap="plasma", max_zoom=60, center_4326=(10.7463, 59.92, 500))
     """
 
     gdfs, column, kwargs = Map._separate_args(gdfs, column, kwargs)
 
     loc_mask, kwargs = _get_location_mask(kwargs | {"size": size}, gdfs)
 
     kwargs.pop("size", None)
@@ -136,26 +154,45 @@
             mask=mask,
             labels=labels,
             browser=browser,
             max_zoom=max_zoom,
             **kwargs,
         )
 
+    try:
+        to_crs = gdfs[0].crs
+    except IndexError:
+        try:
+            to_crs = [x for x in kwargs.values() if hasattr(x, "crs")][0].crs
+        except IndexError:
+            to_crs = None
+
+    if center_4326 is not None:
+        from_crs = 4326
+        center = center_4326
+    elif "crs" in kwargs:
+        from_crs = kwargs.pop("crs")
+    else:
+        from_crs = to_crs
+
     if center is not None:
         size = size or 1000
         if isinstance(center, str) and not is_wkt(center):
-            mask = address_to_gdf(center, crs=gdfs[0].crs).buffer(size)
-        elif isinstance(center, GeoDataFrame):
+            mask = address_to_gdf(center, crs=from_crs)
+        elif isinstance(center, (GeoDataFrame, GeoSeries)):
             mask = center
         else:
-            try:
-                mask = to_gdf_func(center, crs=gdfs[0].crs)
-            except IndexError:
-                df = [x for x in kwargs.values() if hasattr(x, "crs")][0]
-                mask = to_gdf_func(center, crs=df.crs)
+            if isinstance(center, (tuple, list)) and len(center) == 3:
+                *center, size = center
+            mask = to_gdf_func(center, crs=from_crs)
+
+        try:
+            mask = mask.to_crs(to_crs)
+        except ValueError:
+            pass
 
         if get_geom_type(mask) in ["point", "line"]:
             mask = mask.buffer(size)
 
         return clipmap(
             *gdfs,
             column=column,
@@ -172,30 +209,30 @@
         labels=labels,
         browser=browser,
         max_zoom=max_zoom,
         smooth_factor=smooth_factor,
         **kwargs,
     )
 
-    if m.gdfs is None:
+    if m.gdfs is None and not len(m.raster_datasets):
         return
 
     if not kwargs.pop("explore", True):
         return qtm(m._gdf, column=m.column, cmap=m._cmap, k=m.k)
 
-    return m.explore()
+    m.explore()
 
 
 def samplemap(
     *gdfs: GeoDataFrame,
     column: str | None = None,
     size: int = 1000,
     sample_from_first: bool = True,
     labels: tuple[str] | None = None,
-    max_zoom: int = 30,
+    max_zoom: int = 40,
     smooth_factor: int = 1.5,
     explore: bool = True,
     browser: bool = False,
     **kwargs,
 ) -> None:
     """Shows an interactive map of a random area of GeoDataFrames.
 
@@ -268,15 +305,15 @@
             column=column,
             labels=labels,
             browser=browser,
             max_zoom=max_zoom,
             smooth_factor=smooth_factor,
             **kwargs,
         )
-        if m.gdfs is None:
+        if m.gdfs is None and not len(m.raster_datasets):
             return
         if mask is not None:
             m._gdfs = [gdf.clip(mask) for gdf in m._gdfs]
             m._gdf = m._gdf.clip(mask)
             m._nan_idx = m._gdf[m._column].isna()
             m._get_unique_values()
 
@@ -316,15 +353,15 @@
 
 def clipmap(
     *gdfs: GeoDataFrame,
     column: str | None = None,
     mask: GeoDataFrame | GeoSeries | Geometry = None,
     labels: tuple[str] | None = None,
     explore: bool = True,
-    max_zoom: int = 30,
+    max_zoom: int = 40,
     smooth_factor: int | float = 1.5,
     browser: bool = False,
     **kwargs,
 ) -> None:
     """Shows an interactive map of a of GeoDataFrames clipped to the mask extent.
 
     It takes all the GeoDataFrames specified, clips them to the extent of the mask,
@@ -377,15 +414,15 @@
             column=column,
             labels=labels,
             browser=browser,
             max_zoom=max_zoom,
             smooth_factor=smooth_factor,
             **kwargs,
         )
-        if m.gdfs is None:
+        if m.gdfs is None and not len(m.raster_datasets):
             return
 
         m._gdfs = [gdf.clip(mask) for gdf in m._gdfs]
         m._gdf = m._gdf.clip(mask)
         m._nan_idx = m._gdf[m._column].isna()
         m._get_unique_values()
         m.explore(center=center, size=size)
@@ -403,59 +440,82 @@
         m._gdf = m._gdf.clip(mask)
         m._nan_idx = m._gdf[m._column].isna()
         m._get_unique_values()
 
         qtm(m._gdf, column=m.column, cmap=m._cmap, k=m.k)
 
 
-def explore_locals(*gdfs, to_gdf: bool = True, **kwargs):
-    """Viser kart (explore) over alle lokale GeoDataFrames.
+def explore_locals(*gdfs, convert: bool = True, **kwargs):
+    """Displays all local variables with geometries (GeoDataFrame etc.).
 
-    Lokalt betyr enten inni funksjonen/metoden du er i, eller i notebooken
-    du jobber i.
+    Local means inside a function or file/notebook.
 
     Args:
-        *gdfs: Ekstra GeoDataFrames du vil legge til
-        **kwargs: keyword arguments som sendes til sg.explore.
+        *gdfs: Additional GeoDataFrames.
+        convert: If True (default), non-GeoDataFrames will be converted
+            to GeoDataFrames if possible.
+        **kwargs: keyword arguments passed to sg.explore.
     """
-    frame = inspect.currentframe()
 
+    def as_dict(obj):
+        if hasattr(obj, "__dict__"):
+            return obj.__dict__
+        elif isinstance(obj, dict):
+            return obj
+        raise TypeError
+
+    frame = inspect.currentframe().f_back
+
+    allowed_types = (GeoDataFrame, GeoSeries, Geometry, RasterDataset)
+
+    local_gdfs = {}
     while True:
-        local_gdfs = {}
         for name, value in frame.f_locals.items():
-            if isinstance(value, GeoDataFrame):
+            if isinstance(value, GeoDataFrame) and len(value):
                 local_gdfs[name] = value
                 continue
-            if not to_gdf:
-                continue
-            try:
-                if hasattr(value, "__len__") and not len(value):
-                    continue
-            except TypeError:
+            if not convert:
                 continue
 
+            if isinstance(value, dict) or hasattr(value, "__dict__"):
+                # add dicts or classes with GeoDataFrames to kwargs
+                for key, value in as_dict(value).items():
+                    if isinstance(value, allowed_types):
+                        gdf = clean_geoms(to_gdf_func(value))
+                        if len(gdf):
+                            local_gdfs[key] = gdf
+
+                    elif isinstance(value, dict) or hasattr(value, "__dict__"):
+                        try:
+                            for k, v in value.items():
+                                if isinstance(v, allowed_types):
+                                    gdf = clean_geoms(to_gdf_func(v))
+                                    if len(gdf):
+                                        local_gdfs[k] = gdf
+                        except Exception:
+                            # no need to raise here
+                            pass
+
+                continue
             try:
                 gdf = clean_geoms(to_gdf_func(value))
                 if len(gdf):
                     local_gdfs[name] = gdf
+                continue
             except Exception:
                 pass
 
         if local_gdfs:
             break
 
         frame = frame.f_back
 
         if not frame:
             break
 
-    mask = kwargs.pop("mask", None)
-    if mask is not None:
-        local_gdfs = {name: gdf.clip(mask) for name, gdf in local_gdfs.items()}
-
     explore(*gdfs, **local_gdfs, **kwargs)
 
 
 def qtm(
     *gdfs: GeoDataFrame,
     column: str | None = None,
     title: str | None = None,
```

### Comparing `ssb_sgis-0.3.9/src/sgis/maps/thematicmap.py` & `ssb_sgis-1.0.0/src/sgis/maps/thematicmap.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/src/sgis/maps/tilesources.py` & `ssb_sgis-1.0.0/src/sgis/maps/tilesources.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/src/sgis/networkanalysis/_get_route.py` & `ssb_sgis-1.0.0/src/sgis/networkanalysis/_get_route.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/src/sgis/networkanalysis/_od_cost_matrix.py` & `ssb_sgis-1.0.0/src/sgis/networkanalysis/_od_cost_matrix.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/src/sgis/networkanalysis/_points.py` & `ssb_sgis-1.0.0/src/sgis/networkanalysis/_points.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/src/sgis/networkanalysis/_service_area.py` & `ssb_sgis-1.0.0/src/sgis/networkanalysis/_service_area.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/src/sgis/networkanalysis/closing_network_holes.py` & `ssb_sgis-1.0.0/src/sgis/networkanalysis/closing_network_holes.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/src/sgis/networkanalysis/cutting_lines.py` & `ssb_sgis-1.0.0/src/sgis/networkanalysis/cutting_lines.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/src/sgis/networkanalysis/directednetwork.py` & `ssb_sgis-1.0.0/src/sgis/networkanalysis/directednetwork.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/src/sgis/networkanalysis/finding_isolated_networks.py` & `ssb_sgis-1.0.0/src/sgis/networkanalysis/finding_isolated_networks.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/src/sgis/networkanalysis/network.py` & `ssb_sgis-1.0.0/src/sgis/networkanalysis/network.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/src/sgis/networkanalysis/networkanalysis.py` & `ssb_sgis-1.0.0/src/sgis/networkanalysis/networkanalysis.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/src/sgis/networkanalysis/networkanalysisrules.py` & `ssb_sgis-1.0.0/src/sgis/networkanalysis/networkanalysisrules.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/src/sgis/networkanalysis/nodes.py` & `ssb_sgis-1.0.0/src/sgis/networkanalysis/nodes.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/src/sgis/networkanalysis/traveling_salesman.py` & `ssb_sgis-1.0.0/src/sgis/networkanalysis/traveling_salesman.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.3.9/src/sgis/raster/elevationraster.py` & `ssb_sgis-1.0.0/src/sgis/raster/gradient.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,88 +1,78 @@
 import numpy as np
 
-from .raster import Raster
 
+def get_gradient(raster, degrees: bool = False, copy: bool = False):
+    """Get the slope of an elevation raster.
 
-class ElevationRaster(Raster):
-    """For raster calculation on elevation images."""
+    Calculates the absolute slope between the grid cells
+    based on the image resolution.
 
-    def __init__(self, raster=None, **kwargs):
-        kwargs = {"band_index": 1} | kwargs
-        super().__init__(raster, **kwargs)
-
-    def gradient(self, degrees: bool = False, copy: bool = False):
-        """Get the slope of an elevation raster.
-
-        Calculates the absolute slope between the grid cells
-        based on the image resolution.
-
-        For multiband images, the calculation is done for each band.
-
-        Args:
-            degrees: If False (default), the returned values will be in ratios,
-                where a value of 1 means 1 meter up per 1 meter forward. If True,
-                the values will be in degrees from 0 to 90.
-            copy: Whether to copy or overwrite the original Raster.
-                Defaults to False to save memory.
-
-        Returns:
-            The class instance with new array values, or a copy if copy is True.
-
-        Examples
-        --------
-        Making an array where the gradient to the center is always 10.
-
-        >>> import sgis as sg
-        >>> import numpy as np
-        >>> arr = np.array(
-        ...         [
-        ...             [100, 100, 100, 100, 100],
-        ...             [100, 110, 110, 110, 100],
-        ...             [100, 110, 120, 110, 100],
-        ...             [100, 110, 110, 110, 100],
-        ...             [100, 100, 100, 100, 100],
-        ...         ]
-        ...     )
-
-        Now let's create an ElevationRaster from this array with a resolution of 10.
-
-        >>> r = sg.ElevationRaster.from_array(arr, crs=None, bounds=(0, 0, 50, 50))
-        >>> r.res
-        (10.0, 10.0)
-
-        The gradient will be 1 (1 meter up for every meter forward).
-        The calculation is by default done in place to save memory.
-
-        >>> r.gradient()
-        >>> r.array
-        array([[0., 1., 1., 1., 0.],
-            [1., 1., 1., 1., 1.],
-            [1., 1., 0., 1., 1.],
-            [1., 1., 1., 1., 1.],
-            [0., 1., 1., 1., 0.]])
-        """
-        if len(self.array.shape) == 2:
-            array = self._slope_2d(self.array, degrees=degrees)
-        else:
-            out_array = []
-            for array in self.array:
-                results = self._slope_2d(array, degrees=degrees)
-                out_array.append(results)
-            array = np.array(out_array)
-
-        return self._return_self_or_copy(array, copy)
-
-    def _slope_2d(self, array, degrees) -> np.ndarray:
-        gradient_x, gradient_y = np.gradient(array, self.res[0], self.res[1])
-
-        gradient = abs(gradient_x) + abs(gradient_y)
-
-        if not degrees:
-            return gradient
+    For multiband images, the calculation is done for each band.
 
-        radians = np.arctan(gradient)
-        degrees = np.degrees(radians)
+    Args:
+        degrees: If False (default), the returned values will be in ratios,
+            where a value of 1 means 1 meter up per 1 meter forward. If True,
+            the values will be in degrees from 0 to 90.
+        copy: Whether to copy or overwrite the original Raster.
+            Defaults to False to save memory.
+
+    Returns:
+        The class instance with new array values, or a copy if copy is True.
+
+    Examples
+    --------
+    Making an array where the gradient to the center is always 10.
+
+    >>> import sgis as sg
+    >>> import numpy as np
+    >>> arr = np.array(
+    ...         [
+    ...             [100, 100, 100, 100, 100],
+    ...             [100, 110, 110, 110, 100],
+    ...             [100, 110, 120, 110, 100],
+    ...             [100, 110, 110, 110, 100],
+    ...             [100, 100, 100, 100, 100],
+    ...         ]
+    ...     )
+
+    Now let's create a Raster from this array with a resolution of 10.
+
+    >>> r = sg.Raster.from_array(arr, crs=None, bounds=(0, 0, 50, 50), res=10)
+
+    The gradient will be 1 (1 meter up for every meter forward).
+    The calculation is by default done in place to save memory.
+
+    >>> r.gradient()
+    >>> r.array
+    array([[0., 1., 1., 1., 0.],
+        [1., 1., 1., 1., 1.],
+        [1., 1., 0., 1., 1.],
+        [1., 1., 1., 1., 1.],
+        [0., 1., 1., 1., 0.]])
+    """
+    if len(raster.array.shape) == 2:
+        array = _slope_2d(raster.array, raster.res, degrees=degrees)
+    else:
+        out_array = []
+        for array in raster.array:
+            results = _slope_2d(array, raster.res, degrees=degrees)
+            out_array.append(results)
+        array = np.array(out_array)
+
+    return raster._return_self_or_copy(array, copy)
+
+
+def _slope_2d(array, res, degrees) -> np.ndarray:
+    gradient_x, gradient_y = np.gradient(array, res, res)
+
+    gradient = abs(gradient_x) + abs(gradient_y)
+
+    if not degrees:
+        return gradient
 
-        assert np.max(degrees) <= 90
+    radians = np.arctan(gradient)
+    degrees = np.degrees(radians)
 
-        return degrees
+    assert np.max(degrees) <= 90
+
+    return degrees
```

### Comparing `ssb_sgis-0.3.9/src/sgis/raster/raster.py` & `ssb_sgis-1.0.0/src/sgis/raster/raster.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,71 @@
+import functools
 import numbers
 import re
-import uuid
 import warnings
-from collections.abc import Callable
+from collections.abc import Callable, Iterable
 from copy import copy, deepcopy
 from json import loads
 from pathlib import Path
 
 import geopandas as gpd
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import pyproj
 import rasterio
 import shapely
+from typing_extensions import Self  # TODO: imperter fra typing når python 3.11
 
 
 try:
     import xarray as xr
+    from xarray import DataArray
 except ImportError:
-    pass
+
+    class DataArray:
+        pass
+
+
 try:
     from rioxarray.rioxarray import _generate_spatial_coords
 except ImportError:
     pass
 from affine import Affine
 from geopandas import GeoDataFrame, GeoSeries
 from pandas.api.types import is_list_like
 from rasterio import features
 from rasterio.enums import MergeAlg
 from rasterio.io import DatasetReader
-from rasterio.mask import mask as rast_mask
 from rasterio.vrt import WarpedVRT
 from rasterio.warp import reproject
-from shapely import Geometry, box
+from shapely import Geometry
 from shapely.geometry import Point, Polygon, shape
 
-from ..geopandas_tools.bounds import to_bbox
-from ..geopandas_tools.conversion import to_gdf
+from ..geopandas_tools.conversion import to_bbox, to_gdf, to_shapely
 from ..geopandas_tools.general import is_bbox_like, is_wkt
-from ..helpers import get_non_numpy_func_name, get_numpy_func, is_property
+from ..helpers import is_property
 from ..io.opener import opener
-from .base import (
-    RasterBase,
-    RasterHasChangedError,
-    get_index_mapper,
-    memfile_from_array,
-)
+from .base import ALLOWED_KEYS, NESSECARY_META, get_index_mapper, memfile_from_array
+from .gradient import get_gradient
 from .zonal import (
     _aggregate,
     _no_overlap_df,
     make_geometry_iterrows,
     prepare_zonal,
     zonal_post,
 )
 
 
 numpy_func_message = (
-    "aggfunc must be functions or " "strings of numpy functions or methods."
+    "aggfunc must be functions or strings of numpy functions or methods."
 )
 
 
-class Raster(RasterBase):
+class Raster:
     """For reading, writing and working with rasters.
 
     Raster instances should be created with the methods 'from_path', 'from_array' or
     'from_gdf'.
 
 
     Examples
@@ -97,15 +97,15 @@
 
     >>> raster.write("path/to/file.tif")
 
     Convert to GeoDataFrame.
 
     >>> gdf = raster.to_gdf(column="elevation")
     >>> gdf
-           elevation                                           geometry  band_index
+           elevation                                           geometry  indexes
     0            1.9  POLYGON ((-25665.000 6676005.000, -25665.000 6...           1
     1           11.0  POLYGON ((-25655.000 6676005.000, -25655.000 6...           1
     2           18.1  POLYGON ((-25645.000 6676005.000, -25645.000 6...           1
     3           15.8  POLYGON ((-25635.000 6676005.000, -25635.000 6...           1
     4           11.6  POLYGON ((-25625.000 6676005.000, -25625.000 6...           1
     ...          ...                                                ...         ...
     25096       13.4  POLYGON ((-24935.000 6674005.000, -24935.000 6...           1
@@ -143,145 +143,111 @@
     25097   9.4   9.4  POLYGON ((-24925.000 6674005.000, -24925.000 6...
     25098   5.3   5.3  POLYGON ((-24915.000 6674005.000, -24915.000 6...
     25099   2.3   2.3  POLYGON ((-24905.000 6674005.000, -24905.000 6...
     25100   0.1   0.1  POLYGON ((-24895.000 6674005.000, -24895.000 6...
 
     """
 
+    # attributes conserning file path
+    filename_regex: str | None = None
+    date_format: str | None = None
+    contains: str | None = None
+    endswith: str = ".tif"
+
+    # attributes conserning rasterio metadata
+    _profile = {
+        "driver": "GTiff",
+        "compress": "LZW",
+        "nodata": None,
+        "dtype": None,
+        "crs": None,
+        "tiled": None,
+        "indexes": None,
+    }
+
+    # driver: str = "GTiff"
+    # compress: str = "LZW"
+    # _nodata: int | float | None = None
+    # _dtype: type | None = None
+
     def __init__(
         self,
         raster=None,
         *,
         path: str | None = None,
+        # indexes: int | list[int] | None = None,
         array: np.ndarray | None = None,
-        band_index: int | list[int] | None = None,
-        name: str | None = None,
-        name_regex: str | None = None,
-        date: str | None = None,
-        date_regex: str | None = None,
-        shortname: str | None = None,
-        dtype: type | None = None,
-        nodata: int | float | None = None,
+        file_system=None,
         **kwargs,
     ):
         if raster is not None:
             if not isinstance(raster, Raster):
                 raise TypeError(
-                    "Raster should be constructed with the from-classmethods."
+                    "Raster should be constructed with the classmethods (from_...)."
                 )
             for key, value in raster.__dict__.items():
-                self[key] = value
+                setattr(raster, key, value)
             return
 
-        self.path = path
-        self.array = array
+        if path is None and not any([kwargs.get("transform"), kwargs.get("bounds")]):
+            raise TypeError(
+                "Must specify either bounds or transform when constructing raster from array."
+            )
 
-        # hasattr check to allow class attributes in subclasses
-        if not hasattr(self, "shortname"):
-            self.shortname = shortname
-        if not hasattr(self, "name_regex"):
-            self.name_regex = name_regex
-        if not hasattr(self, "date_regex"):
-            self.date_regex = date_regex
-        if not hasattr(self, "_dtype") or dtype is not None:
-            self._dtype = dtype
-        if not hasattr(self, "nodata"):
-            self.nodata = nodata
-
-        if not hasattr(self, "driver"):
-            self.driver = kwargs.pop("driver", "GTiff")
-        if not hasattr(self, "compress"):
-            self.compress = kwargs.pop("compress", "LZW")
-
-        if not hasattr(self, "_band_index") or band_index is not None:
-            self._band_index = self._get_band_index(band_index)
-
-        # underscore to allow properties without setters in subclasses (e.g. Sentinel2)
-        if date:
-            self._date = date
-        if name:
-            self._name = name
+        # add class profile first to override with args and kwargs
+        self.update(**self._profile)
 
-        self.root = kwargs.pop("root", None)
+        self._crs = kwargs.pop("crs", self._crs if hasattr(self, "_crs") else None)
+        self._bounds = None
 
-        self._hash = uuid.uuid4()
+        self.path = path
+        self.array = array
+        self.file_system = file_system
+        self._indexes = self._get_indexes(kwargs.pop("indexes", self.indexes))
 
         # override the above with kwargs
         self.update(**kwargs)
 
-        if self.path is None and self.array is None:
-            return
-
-        if self.path is not None and self.array is not None:
-            raise ValueError("Cannot supply both 'path' and 'array'.")
-
-        # the important attributes must be of correct type
-        crs = kwargs.get("crs")
-        transform = kwargs.get("transform")
-        bounds = kwargs.get("bounds")
-        if bounds is not None:
-            bounds = to_bbox(bounds)
-
-        if not any([path, transform, bounds]):
-            raise TypeError(
-                "Must specify either bounds or transform when constructing raster from array."
-            )
-
-        self._crs = pyproj.CRS(crs) if crs else None
-        transform = Affine(*transform) if transform is not None else None
-
-        if transform and not bounds:
-            self._bounds = rasterio.transform.array_bounds(
-                self.height, self.width, transform
-            )
-        elif not path:
-            self._bounds = bounds
-
         attributes = set(self.__dict__.keys()).difference(set(self.properties))
 
-        if self.path is not None and not self.has_nessecary_attrs(attributes):
-            self.add_meta()
+        if self.path is not None and not self._has_nessecary_attrs(attributes):
+            self._add_meta()
             self._meta_added = True
 
-        if self.path is None:
-            if not isinstance(self.array, np.ndarray):
-                raise TypeError
-
-            if not hasattr(self, "crs"):
-                raise TypeError("Must specify crs when constructing raster from array.")
-
-            self._band_index = self._add_band_index_from_array(band_index)
-
         self._prev_crs = self._crs
 
     @classmethod
     def from_path(
         cls,
         path: str,
+        res: int | None = None,
+        file_system=None,
         **kwargs,
     ):
         """Construct Raster from file path.
 
         Args:
             path: Path to a raster image file.
 
         Returns:
             A Raster instance.
         """
         return cls(
             path=str(path),
+            file_system=file_system,
+            res=res,
             **kwargs,
         )
 
     @classmethod
     def from_array(
         cls,
         array: np.ndarray,
+        crs,
         *,
-        crs=None,
         transform: Affine | None = None,
         bounds: tuple | Geometry | None = None,
         copy: bool = True,
         **kwargs,
     ):
         """Construct Raster from numpy array.
 
@@ -301,29 +267,45 @@
 
         Returns:
             A Raster instance.
         """
         if array is None:
             raise TypeError("Must specify array.")
 
+        if not any([transform, bounds]):
+            raise TypeError(
+                "Must specify either bounds or transform when constructing raster from array."
+            )
+
         array = array.copy() if copy else array
 
-        return cls(
-            array=array,
-            crs=crs,
-            transform=transform,
-            bounds=bounds,
-            **kwargs,
-        )
+        if len(array.shape) == 2:
+            height, width = array.shape
+        elif len(array.shape) == 3:
+            height, width = array.shape[1:]
+        else:
+            raise ValueError("array must be 2 or 3 dimensional.")
+
+        transform = Affine(*transform) if transform is not None else None
+
+        if bounds is not None:
+            bounds = to_bbox(bounds)
+
+        if transform and not bounds:
+            bounds = rasterio.transform.array_bounds(height, width, transform)
+
+        crs = pyproj.CRS(crs) if crs else None
+
+        return cls(array=array, crs=crs, transform=transform, bounds=bounds, **kwargs)
 
     @classmethod
     def from_gdf(
         cls,
         gdf: GeoDataFrame,
-        columns: str | list[str],
+        columns: str | Iterable[str],
         res: int,
         fill=0,
         all_touched=False,
         merge_alg=MergeAlg.replace,
         default_value=1,
         dtype=None,
         **kwargs,
@@ -344,21 +326,21 @@
             raise TypeError("Unexpected argument 'transform'")
 
         kwargs["crs"] = gdf.crs or kwargs.get("crs")
 
         if kwargs["crs"] is None:
             raise TypeError("Must specify crs if the object doesn't have crs.")
 
-        shape = cls.get_shape_from_bounds(gdf.total_bounds, res=res)
-        transform = cls.get_transform_from_bounds(gdf.total_bounds, shape)
+        shape = get_shape_from_bounds(gdf.total_bounds, res=res)
+        transform = get_transform_from_bounds(gdf.total_bounds, shape)
         kwargs["transform"] = transform
 
         def _rasterize(gdf, col):
             return features.rasterize(
-                cls._to_geojson_geom_val(gdf, col),
+                cls._gdf_to_geojson_with_col(gdf, col),
                 out_shape=shape,
                 transform=transform,
                 fill=fill,
                 all_touched=all_touched,
                 merge_alg=merge_alg,
                 default_value=default_value,
                 dtype=dtype,
@@ -396,50 +378,73 @@
             dictionary: Dictionary with the nessecary and optional information
                 about the raster. This can be fetched from an existing raster with
                 the to_dict method.
 
         Returns:
             A Raster instance.
         """
-
-        cls.validate_dict(dictionary)
+        cls._validate_dict(dictionary)
 
         return cls(**dictionary)
 
-    def update(self, **kwargs):
+    def update(self, **kwargs) -> Self:
         for key, value in kwargs.items():
-            self.validate_key(key)
-            if key == "indexes":
-                self._band_index = value
+            self._validate_key(key)
             if is_property(self, key):
-                self["_" + key] = value
-            else:
-                self[key] = value
+                key = "_" + key
+            setattr(self, key, value)
         return self
 
-    def load(self, res: int | None = None, **kwargs):
+    def write(self, path: str, window=None, **kwargs) -> None:
+        """Write the raster as a single file.
+
+        Multiband arrays will result in a multiband image file.
+
+        Args:
+            path: File path to write to.
+            window: Optional window to clip the image to.
+        """
+
+        if self.array is None:
+            raise AttributeError("The image hasn't been loaded.")
+
+        profile = self.profile | kwargs
+
+        with opener(path, file_system=self.file_system) as file:
+            with rasterio.open(file, "w", **profile) as dst:
+                self._write(dst, window)
+
+        self.path = str(path)
+
+    def load(self, **kwargs) -> Self:
         """Load the entire image as an np.array.
 
         The array is stored in the 'array' attribute
         of the Raster.
 
         Args:
             **kwargs: Keyword arguments passed to the rasterio read
                 method.
         """
         if "mask" in kwargs:
             raise ValueError("Got an unexpected keyword argument 'mask'")
         if "window" in kwargs:
             raise ValueError("Got an unexpected keyword argument 'window'")
 
-        self._read_tif(res=res, **kwargs)
+        self._read_tif(**kwargs)
 
         return self
 
-    def clip(self, mask, boundless: bool = True, **kwargs):
+    def clip(
+        self,
+        mask,
+        masked: bool = False,
+        boundless: bool = True,
+        **kwargs,
+    ) -> Self:
         """Load the part of the image inside the mask.
 
         The returned array is stored in the 'array' attribute
         of the Raster.
 
         Args:
             mask: Geometry-like object or bounding box.
@@ -448,27 +453,35 @@
 
         Returns:
             Self, but with the array loaded.
         """
         if not isinstance(mask, GeoDataFrame):
             mask = self._return_gdf(mask)
 
-        if not self.crs.equals(pyproj.CRS(mask.crs)):
-            raise ValueError("crs mismatch.")
+        try:
+            mask = mask.to_crs(self.crs)
+        except ValueError:
+            mask = mask.set_crs(self.crs)
+
+        # if not self.crs.equals(pyproj.CRS(mask.crs)):
+        #     raise ValueError("crs mismatch.")
 
-        self._read_with_mask(mask=mask, boundless=boundless, **kwargs)
+        self._read_with_mask(mask=mask, masked=masked, boundless=boundless, **kwargs)
 
         return self
 
-    def sample(self, n=1, size=20, mask=None, copy=True, **kwargs):
+    def intersects(self, other) -> bool:
+        return self.unary_union.intersects(to_shapely(other))
+
+    def sample(self, n=1, size=20, mask=None, copy=True, **kwargs) -> Self:
         if mask is not None:
             points = GeoSeries(self.unary_union).clip(mask).sample_points(n)
         else:
             points = GeoSeries(self.unary_union).sample_points(n)
-        buffered = points.buffer(size / self.res[0])
+        buffered = points.buffer(size / self.res)
         boxes = to_gdf(
             [shapely.box(*arr) for arr in buffered.bounds.values], crs=self.crs
         )
         if copy:
             copy = self.copy()
             return copy.clip(boxes, **kwargs)
         return self.clip(boxes, **kwargs)
@@ -511,42 +524,77 @@
             aggregated,
             polygons=polygons,
             idx_mapper=idx_mapper,
             idx_name=idx_name,
             dropna=dropna,
         )
 
-    def write(self, path: str, window=None, **kwargs):
-        """Write the raster as a single file.
-
-        Multiband arrays will result in a multiband image file.
+    def gradient(self, degrees: bool = False, copy: bool = False) -> Self:
+        """Get the slope of an elevation raster.
 
-        Args:
-            path: File path to write to.
-            window: Optional window to clip the image to.
-        """
+        Calculates the absolute slope between the grid cells
+        based on the image resolution.
 
-        if self.array is None:
-            raise AttributeError("The image hasn't been loaded yet.")
+        For multiband images, the calculation is done for each band.
 
-        profile = self.profile | kwargs
+        Args:
+            degrees: If False (default), the returned values will be in ratios,
+                where a value of 1 means 1 meter up per 1 meter forward. If True,
+                the values will be in degrees from 0 to 90.
+            copy: Whether to copy or overwrite the original Raster.
+                Defaults to False to save memory.
 
-        with opener(path) as file:
-            with rasterio.open(file, "w", **profile) as dst:
-                self._write(dst, window)
+        Returns:
+            The class instance with new array values, or a copy if copy is True.
 
-        self.path = str(path)
+        Examples
+        --------
+        Making an array where the gradient to the center is always 10.
+
+        >>> import sgis as sg
+        >>> import numpy as np
+        >>> arr = np.array(
+        ...         [
+        ...             [100, 100, 100, 100, 100],
+        ...             [100, 110, 110, 110, 100],
+        ...             [100, 110, 120, 110, 100],
+        ...             [100, 110, 110, 110, 100],
+        ...             [100, 100, 100, 100, 100],
+        ...         ]
+        ...     )
+
+        Now let's create a Raster from this array with a resolution of 10.
+
+        >>> r = sg.Raster.from_array(arr, crs=None, bounds=(0, 0, 50, 50))
+
+        The gradient will be 1 (1 meter up for every meter forward).
+        The calculation is by default done in place to save memory.
+
+        >>> r.gradient()
+        >>> r.array
+        array([[0., 1., 1., 1., 0.],
+            [1., 1., 1., 1., 1.],
+            [1., 1., 0., 1., 1.],
+            [1., 1., 1., 1., 1.],
+            [0., 1., 1., 1., 0.]])
+        """
+        return get_gradient(self, degrees=degrees, copy=copy)
 
-    def to_xarray(self) -> xr.DataArray:
-        self.check_for_array()
+    def to_xarray(self) -> DataArray:
+        self._check_for_array()
+        self.name = self.name or self.__class__.__name__.lower()
         coords = _generate_spatial_coords(self.transform, self.width, self.height)
         if len(self.array.shape) == 2:
             dims = ["y", "x"]
+            # dims = ["band", "y", "x"]
+            # array = np.array([self.array])
+            # assert len(array.shape) == 3
         elif len(self.array.shape) == 3:
             dims = ["band", "y", "x"]
+            # array = self.array
         else:
             raise ValueError("Array must be 2 or 3 dimensional.")
         return xr.DataArray(
             self.array,
             coords=coords,
             dims=dims,
             name=self.name,
@@ -573,17 +621,17 @@
                 Can be a single string or an iterable with the same length as
                 the number of raster bands.
 
         Returns:
             A GeoDataFrame with a geometry column, a 'band' column and a
             one or more value columns.
         """
-        self.check_for_array()
+        self._check_for_array()
 
-        array_list = self._to_2d_array_list(self.array)
+        array_list = self.array_list()
 
         if is_list_like(column) and len(column) != len(array_list):
             raise ValueError(
                 "columns should be a string or a list of same length as "
                 f"layers in the array ({len(array_list)})."
             )
 
@@ -599,581 +647,569 @@
                 pd.DataFrame(
                     self._array_to_geojson(array, self.transform),
                     columns=[column, "geometry"],
                 ),
                 geometry="geometry",
                 crs=self.crs,
             )
-            gdf["band_index"] = i + 1
-
-            if hasattr(self, "_datadict"):
-                for name, value in self._datadict.items():
-                    try:
-                        gdf[name] = value
-                    except Exception:
-                        # in case of iterable columns (band_index...)
-                        # reset index in case of duplicate index
-                        index = gdf.index
-                        gdf = gdf.reset_index(drop=True)
-                        gdf[name] = pd.Series(
-                            [value for _ in range(len(gdf))], index=gdf.index
-                        )
-                        gdf.index = index
-
+            gdf["indexes"] = i + 1
             gdfs.append(gdf)
 
         return pd.concat(gdfs, ignore_index=True)
 
     def set_crs(
         self,
         crs,
         allow_override: bool = False,
-    ):
+    ) -> Self:
         """Set coordinate reference system."""
         if not allow_override and self.crs is not None:
             raise ValueError("Cannot overwrite crs when allow_override is False.")
 
         if self.array is None:
             raise ValueError("array must be loaded/clipped before set_crs")
 
         self._crs = pyproj.CRS(crs)
         return self
 
-    def to_crs(self, crs, **kwargs):
+    def to_crs(self, crs, **kwargs) -> Self:
         """Reproject the raster.
 
         Args:
             crs: The new coordinate reference system.
             **kwargs: Keyword arguments passed to the reproject function
                 from the rasterio.warp module.
         """
         if self.crs is None:
             raise ValueError("Raster has no crs. Use set_crs.")
 
-        if pyproj.CRS(crs).equals(pyproj.CRS(self.crs)):
-            return self
+        # if pyproj.CRS(crs).equals(pyproj.CRS(self._crs)) and pyproj.CRS(crs).equals(
+        #     pyproj.CRS(self._prev_crs)
+        # ):
+        #     return self
 
         if self.array is None:
             project = pyproj.Transformer.from_crs(
                 pyproj.CRS(self._prev_crs), pyproj.CRS(crs), always_xy=True
             ).transform
 
             old_box = shapely.box(*self.bounds)
             new_box = shapely.ops.transform(project, old_box)
             self._bounds = to_bbox(new_box)
 
-            # TODO: fix this
-            print("old/new:", shapely.area(old_box) / shapely.area(new_box))
-
-            """self._bounds = rasterio.warp.transform_bounds(
-                pyproj.CRS(self._prev_crs), pyproj.CRS(crs), *to_bbox(self._bounds)
-            )
-            transformer = pyproj.Transformer.from_crs(
-                pyproj.CRS(self._prev_crs), pyproj.CRS(crs), always_xy=True
-            )
-            minx, miny, maxx, maxy = self.bounds
-            xs, ys = transformer.transform(xx=[minx, maxx], yy=[miny, maxy])
+            # TODO: fix area changing... if possible
+            # print("old/new:", shapely.area(old_box) / shapely.area(new_box))
 
-            minx, maxx = xs
-            miny, maxy = ys
-            self._bounds = minx, miny, maxx, maxy"""
+            if pyproj.CRS(crs).equals(pyproj.CRS(self._crs)):
+                self._warped_crs = self._crs
+                return self
+
+            # self._bounds = rasterio.warp.transform_bounds(
+            #     pyproj.CRS(self._prev_crs), pyproj.CRS(crs), *to_bbox(self._bounds)
+            # )
+            # transformer = pyproj.Transformer.from_crs(
+            #     pyproj.CRS(self._prev_crs), pyproj.CRS(crs), always_xy=True
+            # )
+            # minx, miny, maxx, maxy = self.bounds
+            # xs, ys = transformer.transform(xx=[minx, maxx], yy=[miny, maxy])
+
+            # minx, maxx = xs
+            # miny, maxy = ys
+            # self._bounds = minx, miny, maxx, maxy
 
             # self._bounds = shapely.transform(old_box, project)
         else:
+            was_2d = len(self.shape) == 2
             self.array, transform = reproject(
                 source=self.array,
-                src_crs=self.crs,
+                src_crs=self._prev_crs,
                 src_transform=self.transform,
                 dst_crs=pyproj.CRS(crs),
                 **kwargs,
             )
+            if was_2d and len(self.array.shape) == 3:
+                assert self.array.shape[0] == 1
+                self.array = self.array[0]
 
             self._bounds = rasterio.transform.array_bounds(
                 self.height, self.width, transform
             )
 
         self._warped_crs = pyproj.CRS(crs)
         self._prev_crs = pyproj.CRS(crs)
 
         return self
 
     def plot(self, mask=None) -> None:
-        self.check_for_array()
+        self._check_for_array()
         """Plot the images. One image per band."""
-        if len(self.shape) == 3:
-            for arr in self.array:
-                self._plot_2d(arr)
+        if mask is not None:
+            raster = self.copy().clip(mask)
+        else:
+            raster = self
+
+        if len(raster.shape) == 2:
+            array = np.array([raster.array])
+        else:
+            array = raster.array
 
-    def astype(self, dtype: type):
+        for arr in array:
+            ax = plt.axes()
+            ax.imshow(arr)
+            ax.axis("off")
+            plt.show()
+            plt.close()
+
+    def astype(self, dtype: type) -> Self:
         if self.array is None:
             raise ValueError("Array is not loaded.")
         if not rasterio.dtypes.can_cast_dtype(self.array, dtype):
             min_dtype = rasterio.dtypes.get_minimum_dtype(self.array)
             raise ValueError(f"Cannot cast to dtype. Minimum dtype is {min_dtype}")
         self.array = self.array.astype(dtype)
         self._dtype = dtype
         return self
 
-    def as_minimum_dtype(self):
+    def as_minimum_dtype(self) -> Self:
         min_dtype = rasterio.dtypes.get_minimum_dtype(self.array)
         self.array = self.array.astype(min_dtype)
         return self
 
-    def add_meta(self):
+    def min(self) -> int | None:
+        if np.size(self.array):
+            return np.min(self.array)
+        return None
+
+    def max(self) -> int | None:
+        if np.size(self.array):
+            return np.max(self.array)
+        return None
+
+    def _add_meta(self) -> Self:
         mess = "Cannot add metadata after image has been "
         if hasattr(self, "_clipped"):
             raise ValueError(mess + "clipped.")
         if hasattr(self, "_warped_crs"):
             raise ValueError(mess + "reprojected.")
 
-        with opener(self.path) as file:
+        with opener(self.path, file_system=self.file_system) as file:
             with rasterio.open(file) as src:
                 self._add_meta_from_src(src)
 
         return self
 
-    def get_coords(self):
-        # TODO: droppe
-        self.check_for_array()
-        return _generate_spatial_coords(self.transform, self.width, self.height)
-
-    @property
-    def subfolder(self):
-        try:
-            folder = Path(Path(self.path).parent).name
-            if self.root:
-                return folder.difference(self.root)
-            else:
-                return folder
-        except TypeError:
-            return None
-
-    @property
-    def tile(self) -> str | None:
-        if self.bounds is None:
-            return None
-        return f"{int(self.bounds[0])}{int(self.bounds[1])}"
-
-    @property
-    def raster_id(self) -> str:
-        shortname = self.shortname if self.shortname else ""
-        date = self.date if self.date else ""
-        name = self.name if self.name else ""
-        return f"{shortname}_{self.tile}_{date}_{name}".replace("__", "_").strip("_")
+    def array_list(self) -> list[np.ndarray]:
+        self._check_for_array()
+        if len(self.array.shape) == 2:
+            return [self.array]
+        elif len(self.array.shape) == 3:
+            return list(self.array)
+        else:
+            raise ValueError
 
     @property
-    def band_index(self):
-        return self._band_index
+    def indexes(self) -> int | tuple[int] | None:
+        return self._indexes
 
     @property
     def name(self) -> str | None:
-        if hasattr(self, "_name"):
-            return self._name
-        if not self.name_regex and self.path:
-            return Path(self.path).stem
         try:
-            return re.search(self.name_regex, Path(self.path).name).group()
-        except (AttributeError, TypeError):
-            return None
+            return self._name
+        except AttributeError:
+            try:
+                return Path(self.path).name
+            except TypeError:
+                return None
 
     @name.setter
     def name(self, value):
         self._name = value
         return self._name
 
     @property
     def date(self):
-        if hasattr(self, "_date"):
-            return self._date
         try:
-            return re.search(self.date_regex, Path(self.path).name).group()
+            pattern = re.compile(self.filename_regex, re.VERBOSE)
+            return re.match(pattern, Path(self.path).name).group("date")
         except (AttributeError, TypeError):
             return None
 
-    @date.setter
-    def date(self, value):
-        self._date = value
-        return self._date
-
-    @property
-    def band_color(self):
-        """To be implemented in subclasses."""
-        pass
-
     @property
-    def is_mask(self):
-        """To be implemented in subclasses."""
-        pass
+    def band(self) -> str | None:
+        try:
+            pattern = re.compile(self.filename_regex, re.VERBOSE)
+            return re.match(pattern, Path(self.path).name).group("band")
+        except (AttributeError, TypeError):
+            return None
 
-    def array_list(self):
-        return self._to_2d_array_list(self.array)
+    # @property
+    # def band_color(self):
+    #     """To be implemented in subclasses."""
+    #     pass
 
     @property
     def dtype(self):
         try:
             return self.array.dtype
-        except Exception:
-            return getattr(self, "_dtype", None)
+        except AttributeError:
+            try:
+                return self._dtype
+            except AttributeError:
+                return None
 
     @dtype.setter
     def dtype(self, new_dtype):
         self.array = self.array.astype(new_dtype)
         return self.array.dtype
 
-    def read_kwargs(self, kwargs):
-        # if kwargs is None:
-        #   kwargs = {}
+    @property
+    def nodata(self) -> int | None:
+        try:
+            return self._nodata
+        except AttributeError:
+            return None
+
+    @property
+    def tile(self) -> str | None:
+        if self.bounds is None:
+            return None
+        return f"{int(self.bounds[0])}_{int(self.bounds[1])}"
+
+    @property
+    def meta(self) -> dict:
         return {
-            "indexes": self.band_index,
-            "masked": False,
-            "fill_value": self.nodata,
-        } | kwargs or {}
+            "path": self.path,
+            "type": self.__class__.__name__,
+            "bounds": self.bounds,
+            "indexes": self.indexes,
+            "crs": self.crs,
+        }
 
     @property
-    def profile(self):
+    def profile(self) -> dict:
         # TODO: .crs blir feil hvis warpa. Eller?
         return {
             "driver": self.driver,
+            "compress": self.compress,
             "dtype": self.dtype,
             "crs": self.crs,
             "transform": self.transform,
             "nodata": self.nodata,
             "count": self.count,
             "height": self.height,
             "width": self.width,
-            "compress": self.compress,
-            "indexes": self.band_index,
+            "indexes": self.indexes,
         }
 
     @property
-    def raster_type(self) -> str:
-        return self.__class__.__name__
-
-    @property
-    def area(self):
-        return shapely.area(self.unary_union)
-
-    @property
-    def length(self):
-        return shapely.length(self.unary_union)
-
-    @property
-    def crs(self):
-        try:
-            return self._warped_crs
-        except AttributeError:
-            try:
-                return self._crs
-            except AttributeError:
-                return None
-
-    @property
-    def unary_union(self) -> Polygon:
-        return shapely.box(*self.bounds)
-
-    @property
-    def centroid(self) -> Point:
-        x = (self.bounds[0] + self.bounds[2]) / 2
-        y = (self.bounds[1] + self.bounds[3]) / 2
-        return Point(x, y)
+    def read_kwargs(self) -> dict:
+        return {
+            "indexes": self.indexes,
+            "fill_value": self.nodata,
+            "masked": True,
+        }
 
     @property
-    def res(self) -> tuple[float, float]:
+    def res(self) -> float | None:
+        if hasattr(self, "_res") and self._res is not None:
+            return self._res
         if self.width is None:
             return None
         diffx = self.bounds[2] - self.bounds[0]
-        diffy = self.bounds[3] - self.bounds[1]
-        resx = diffx / self.width
-        resy = diffy / self.height
-        return resx, resy
+        return diffx / self.width
 
     @property
-    def height(self):
+    def height(self) -> int | None:
         if self.array is None:
             try:
                 return self._height
             except AttributeError:
                 return None
         i = 1 if len(self.array.shape) == 3 else 0
         return self.array.shape[i]
 
     @property
-    def width(self):
+    def width(self) -> int | None:
         if self.array is None:
             try:
                 return self._width
             except AttributeError:
-                return None
+                try:
+                    heigth, width = get_shape_from_bounds(self, self.res)  # .res[0])
+                    self._width = width
+                    self._heigth = heigth
+                    return self._width
+                except Exception:
+                    return None
         i = 2 if len(self.array.shape) == 3 else 1
         return self.array.shape[i]
 
     @property
-    def count(self):
+    def count(self) -> int:
         if self.array is not None:
             if len(self.array.shape) == 3:
                 return self.array.shape[0]
             if len(self.array.shape) == 2:
                 return 1
-        if not hasattr(self._band_index, "__iter__"):
+        if not hasattr(self._indexes, "__iter__"):
             return 1
-        return len(self._band_index)
+        return len(self._indexes)
 
     @property
-    def shape(self):
+    def shape(self) -> tuple[int]:
         """Shape that is consistent with the array, whether it is loaded or not."""
         if self.array is not None:
             return self.array.shape
-        if self._band_index is None or hasattr(self._band_index, "__iter__"):
+        if hasattr(self._indexes, "__iter__"):
             return self.count, self.width, self.height
         return self.width, self.height
 
     @property
-    def transform(self) -> Affine:
-        return rasterio.transform.from_bounds(*self.bounds, self.width, self.height)
+    def transform(self) -> Affine | None:
+        try:
+            return rasterio.transform.from_bounds(*self.bounds, self.width, self.height)
+        except (ZeroDivisionError, TypeError):
+            if not self.width or not self.height:
+                return None
 
     @property
     def bounds(self) -> tuple[float, float, float, float] | None:
-        if not hasattr(self, "_bounds"):
+        try:
+            return to_bbox(self._bounds)
+        except (AttributeError, TypeError):
             return None
-        return to_bbox(self._bounds)
 
     @property
-    def total_bounds(self) -> tuple[float, float, float, float]:
-        return self.bounds
-
-    @classmethod
-    def has_nessecary_attrs(cls, dict_like):
-        """Check if Raster init got enough kwargs to not need to read src."""
+    def crs(self):
         try:
-            cls.validate_dict(dict_like)
-            return True
+            return self._warped_crs
         except AttributeError:
-            return False
+            try:
+                return self._crs
+            except AttributeError:
+                return None
+
+    @property
+    def area(self) -> float:
+        return shapely.area(self.unary_union)
+
+    @property
+    def length(self) -> float:
+        return shapely.length(self.unary_union)
+
+    @property
+    def unary_union(self) -> Polygon:
+        return shapely.box(*self.bounds)
+
+    @property
+    def centroid(self) -> Point:
+        x = (self.bounds[0] + self.bounds[2]) / 2
+        y = (self.bounds[1] + self.bounds[3]) / 2
+        return Point(x, y)
+
+    @property
+    def properties(self) -> list[str]:
+        out = []
+        for attr in dir(self):
+            try:
+                if is_property(self, attr):
+                    out.append(attr)
+            except AttributeError:
+                pass
+        return out
 
-    def band_index_tuple(self) -> tuple[int, ...]:
+    def indexes_as_tuple(self) -> tuple[int, ...]:
         if len(self.shape) == 2:
             return (1,)
         return tuple(i + 1 for i in range(self.shape[0]))
 
-    def get(self, key, default=None):
-        try:
-            return self[key]
-        except (KeyError, ValueError, IndexError):
-            return default
-
     def copy(self, deep=True):
         """Returns a (deep) copy of the class instance.
 
         Args:
             deep: Whether to return a deep or shallow copy. Defaults to True.
         """
         if deep:
             return deepcopy(self)
         else:
             return copy(self)
 
     def equals(self, other) -> bool:
         if not isinstance(other, Raster):
             raise NotImplementedError("other must be of type Raster")
+        if type(other) != type(self):
+            return False
         if self.array is None and other.array is not None:
             return False
         if self.array is not None and other.array is None:
             return False
 
         for method in dir(self):
             if not is_property(self, method):
                 continue
-            if self[method] != other[method]:
+            if getattr(self, method) != getattr(other, method):
                 return False
 
         return np.array_equal(self.array, other.array)
 
-    @staticmethod
-    def _plot_2d(array, mask=None) -> None:
-        ax = plt.axes()
-        ax.imshow(array)
-        ax.axis("off")
-        plt.show()
-        plt.close()
-
-    def check_for_array(self, text=""):
-        mess = "Arrays are not loaded. " + text
-        if self.array is None:
-            raise ValueError(mess)
-
-    def _add_band_index_from_array(self, band_index):
-        if band_index is not None:
-            return band_index
-        elif len(self.array.shape) == 3:
-            return tuple(x + 1 for x in range(len(self.array)))
-        elif len(self.array.shape) == 2:
-            return 1
-        else:
-            raise ValueError
-
-    def _add_meta_from_src(self, src):
-        if not hasattr(self, "_bounds"):
-            self._bounds = tuple(src.bounds)
-        self._width = src.width
-        self._height = src.height
-
-        if not hasattr(self, "_band_index") or self._band_index is None:
-            self._band_index = src.indexes
-
-        if not hasattr(self, "nodata") or self.nodata is None:
-            self.nodata = src.nodata
-
+    def __repr__(self) -> str:
+        """The print representation."""
+        shape = self.shape
+        shp = ", ".join([str(x) for x in shape])
         try:
-            self._crs = pyproj.CRS(src.crs)
-        except pyproj.exceptions.CRSError:
-            self._crs = None
+            res = int(self.res)
+        except TypeError:
+            res = None
+        return f"{self.__class__.__name__}(shape=({shp}), res={res}, name={self.name}, path={self.path})"
 
-    def _load_warp_file(self) -> DatasetReader:
-        """(from Torchgeo). Load and warp a file to the correct CRS and resolution.
+    def __mul__(self, scalar):
+        self._check_for_array()
+        self.array = self.array * scalar
+        return self
 
-        Args:
-            filepath: file to load and warp
+    def __add__(self, scalar):
+        self._check_for_array()
+        self.array = self.array + scalar
+        return self
 
-        Returns:
-            file handle of warped VRT
-        """
-        with opener(self.path) as file:
-            src = rasterio.open(file)
+    def __sub__(self, scalar):
+        self._check_for_array()
+        self.array = self.array - scalar
+        return self
 
-        # Only warp if necessary
-        if src.crs != self.crs:
-            vrt = WarpedVRT(src, crs=self.crs)
-            src.close()
-            return vrt
-        return src
+    def __truediv__(self, scalar):
+        self._check_for_array()
+        self.array = self.array / scalar
+        return self
 
-    def _read_tif(self, **kwargs) -> None:
-        def _read(self, src):
-            self._add_meta_from_src(src)
-            out_shape = self.get_shape_from_res(kwargs.pop("res", None))
+    def __floordiv__(self, scalar):
+        self._check_for_array()
+        self.array = self.array // scalar
+        return self
 
-            if hasattr(self, "_warped_crs"):
-                src = WarpedVRT(src, crs=self.crs)
+    def __pow__(self, exponent):
+        self._check_for_array()
+        self.array = self.array**exponent
+        return self
 
-            self.array = src.read(
-                out_shape=out_shape,
-                **self.read_kwargs(kwargs),
+    def _has_nessecary_attrs(self, dict_like) -> bool:
+        """Check if Raster init got enough kwargs to not need to read src."""
+        try:
+            self._validate_dict(dict_like)
+            return all(
+                x is not None for x in [self.indexes, self.res, self.crs, self.bounds]
             )
-            if self._dtype:
-                self = self.astype(self._dtype)
-            else:
-                self = self.as_minimum_dtype()
-
-        with opener(self.path) as file:
-            with rasterio.open(file) as src:
-                _read(self, src)
-
-    def _read_with_mask(self, mask, boundless, **kwargs):
-        kwargs = {"mask": mask, "boundless": boundless} | kwargs
-
-        def _read(self, src, mask, boundless, **kwargs):
-            # to non-warped crs
-            # mask = mask.to_crs(self._crs)
-
-            self._add_meta_from_src(src)
-            transform = self.transform
-            window = rasterio.windows.from_bounds(*to_bbox(mask), transform=transform)
-            kwargs = {
-                "window": window,
-                "boundless": boundless,
-                **self.read_kwargs(kwargs),
-            }
-            if hasattr(self, "_warped_crs"):
-                src = WarpedVRT(src, crs=self.crs)
-                kwargs.pop("boundless")
-            self.array = src.read(**kwargs)
-
-            self._bounds = src.window_bounds(window=window)
-
-            if not np.size(self.array):
-                return
+        except AttributeError:
+            return False
 
-            if self._dtype:
-                self = self.astype(self._dtype)
-            else:
-                self = self.as_minimum_dtype()
+    def _return_self_or_copy(self, array, copy: bool):
+        if not copy:
+            self.array = array
+            return self
+        else:
+            copy = self.copy()
+            copy.array = array
+            return copy
 
-        if self.array is not None:
-            with memfile_from_array(self.array, **self.profile) as src:
-                _read(self, src, **kwargs)
-            return
+    @classmethod
+    def _validate_dict(cls, dict_like) -> None:
+        missing = []
+        for attr in NESSECARY_META:
+            if any(
+                [
+                    attr in dict_like,
+                    f"_{attr}" in dict_like,
+                    attr.lstrip("_") in dict_like,
+                ]
+            ):
+                continue
+            missing.append(attr)
+        if missing:
+            raise AttributeError(f"Missing nessecary key(s) {', '.join(missing)}")
 
-        with opener(self.path) as file:
-            with rasterio.open(file, **self.profile) as src:
-                _read(self, src, **kwargs)
+    @classmethod
+    def _validate_key(cls, key) -> None:
+        if key not in ALLOWED_KEYS:
+            raise ValueError(
+                f"Got an unexpected key {key!r}. Allowed keys are ",
+                ", ".join(ALLOWED_KEYS),
+            )
 
-    def get_shape_from_res(self, res):
+    def _get_shape_from_res(self, res) -> tuple[int] | None:
         if res is None:
             return None
         if hasattr(res, "__iter__") and len(res) == 2:
-            res, res = res
+            res = res[0]
         diffx = self.bounds[2] - self.bounds[0]
         diffy = self.bounds[3] - self.bounds[1]
         width = int(diffx / res)
         height = int(diffy / res)
-        if hasattr(self.band_index, "__iter__"):
-            return len(self.band_index), width, height
+        if hasattr(self.indexes, "__iter__"):
+            return len(self.indexes), width, height
         return width, height
 
     def _write(self, dst, window):
         if np.ma.is_masked(self.array):
             if len(self.array.shape) == 2:
                 return dst.write(
                     self.array.filled(self.nodata), indexes=1, window=window
                 )
 
-            for i in range(len(self.band_index_tuple())):
+            for i in range(len(self.indexes_as_tuple())):
                 dst.write(
                     self.array[i].filled(self.nodata),
                     indexes=i + 1,
                     window=window,
                 )
 
         else:
             if len(self.array.shape) == 2:
                 return dst.write(self.array, indexes=1, window=window)
 
-            for i, idx in enumerate(self.band_index_tuple()):
+            for i, idx in enumerate(self.indexes_as_tuple()):
                 dst.write(self.array[i], indexes=idx, window=window)
 
-    def _get_band_index(self, band_index):
-        if isinstance(band_index, numbers.Number):
-            return int(band_index)
-        if band_index is None:
-            return None
+    def _get_indexes(self, indexes):
+        if isinstance(indexes, numbers.Number):
+            return int(indexes)
+        if indexes is None:
+            if self.array is not None and len(self.array.shape) == 3:
+                return tuple(i + 1 for i in range(self.array.shape[0]))
+            elif self.array is not None and len(self.array.shape) == 2:
+                return 1
+            elif self.array is not None:
+                raise ValueError("Array must be 2 or 3 dimensional.")
+            else:
+                return None
         try:
-            return tuple(int(x) for x in band_index)
+            return tuple(int(x) for x in indexes)
         except Exception as e:
             raise TypeError(
-                "band_index should be an integer or an iterable of integers."
+                "indexes should be an integer or an iterable of integers."
+                f"Got {type(indexes)}: {indexes}"
             ) from e
 
     def _return_gdf(self, obj) -> GeoDataFrame:
         if isinstance(obj, str) and not is_wkt(obj):
             return self._read_tif(obj)
         elif isinstance(obj, Raster):
             return obj.to_gdf()
         elif is_bbox_like(obj):
             return to_gdf(shapely.box(*to_bbox(obj)), crs=self.crs)
         else:
             return to_gdf(obj, crs=self.crs)
 
     @staticmethod
-    def _to_geojson(gdf: GeoDataFrame) -> list[dict]:
+    def _gdf_to_geojson(gdf: GeoDataFrame) -> list[dict]:
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=UserWarning)
             return [x["geometry"] for x in loads(gdf.to_json())["features"]]
 
     @staticmethod
-    def _to_geojson_geom_val(gdf: GeoDataFrame, column: str) -> list[dict]:
+    def _gdf_to_geojson_with_col(gdf: GeoDataFrame, column: str) -> list[dict]:
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=UserWarning)
             return [
                 (feature["geometry"], val)
                 for val, feature in zip(gdf[column], loads(gdf.to_json())["features"])
             ]
 
@@ -1187,85 +1223,172 @@
         except ValueError:
             array = array.astype(np.float32)
             return [
                 (value, shape(geom))
                 for geom, value in features.shapes(array, transform=transform)
             ]
 
-    def min(self):
-        if np.size(self.array):
-            return np.min(self.array)
-        return None
+    def _add_indexes_from_array(self, indexes):
+        if indexes is not None:
+            return indexes
+        elif len(self.array.shape) == 3:
+            return tuple(x + 1 for x in range(len(self.array)))
+        elif len(self.array.shape) == 2:
+            return 1
+        else:
+            raise ValueError
 
-    def max(self):
-        if np.size(self.array):
-            return np.max(self.array)
-        return None
+    def _add_meta_from_src(self, src):
+        if not hasattr(self, "_bounds") or self._bounds is None:
+            self._bounds = tuple(src.bounds)
 
-    def __hash__(self):
-        return hash(self._hash)
+        try:
+            self._crs = pyproj.CRS(src.crs)
+        except pyproj.exceptions.CRSError:
+            self._crs = None
 
-    def __eq__(self, other):
-        if isinstance(other, Raster):
-            return np.all(np.array_equal(self.array, other.array))
-        return NotImplemented
+        self._width = src.width
+        self._height = src.height
 
-    def __repr__(self) -> str:
-        """The print representation."""
-        shape = self.shape
-        shp = ", ".join([str(x) for x in shape])
-        try:
-            res = int(self.res[0])
-        except TypeError:
-            res = None
-        crs = str(self.crs_to_string(self.crs))
-        raster_id = self.raster_id
-        path = self.path
-        return f"{self.__class__.__name__}(shape=({shp}), res={res}, raster_id={raster_id}, crs={crs}, path={path})"
+        # for attr in dir(self):
+        #     try:
+        #         if is_property(self, attr):
+        #             continue
+        #         if attr is None:
+        #             new_value = getattr(src, attr)
+        #             setattr(self, attr, new_value)
+        #     except AttributeError:
+        #         pass
+
+        for attr in ["_indexes", "_nodata"]:
+            if not hasattr(self, attr) or getattr(self, attr) is None:
+                new_value = getattr(src, attr.replace("_", ""))
+                setattr(self, attr, new_value)
 
-    def __setattr__(self, __name: str, __value) -> None:
-        return super().__setattr__(__name, __value)
+        # if not hasattr(self, "_indexes") or self._indexes is None:
+        #     self._indexes = src.indexes
 
-    def __setitem__(self, key, value):
-        setattr(self, key, value)
+        # if not hasattr(self, "_nodata") or self._nodata is None:
+        #     self._nodata = src.nodata
 
-    def __getitem__(self, key):
-        return getattr(self, key)
+    def _load_warp_file(self) -> DatasetReader:
+        """(from Torchgeo). Load and warp a file to the correct CRS and resolution.
 
-    def __mul__(self, scalar):
-        self.check_for_array()
-        self.array = self.array * scalar
-        return self
+        Args:
+            filepath: file to load and warp
 
-    def __add__(self, scalar):
-        self.check_for_array()
-        self.array = self.array + scalar
-        return self
+        Returns:
+            file handle of warped VRT
+        """
+        with opener(self.path, file_system=self.file_system) as file:
+            src = rasterio.open(file)
 
-    def __sub__(self, scalar):
-        self.check_for_array()
-        self.array = self.array - scalar
-        return self
+        # Only warp if necessary
+        if src.crs != self.crs:
+            vrt = WarpedVRT(src, crs=self.crs)
+            src.close()
+            return vrt
+        return src
 
-    def __truediv__(self, scalar):
-        self.check_for_array()
-        self.array = self.array / scalar
-        return self
+    def _read_tif(self, **kwargs) -> None:
+        return self._read(self.path, **kwargs)
 
-    def __floordiv__(self, scalar):
-        self.check_for_array()
-        self.array = self.array // scalar
-        return self
+    @functools.lru_cache(maxsize=128)
+    def _read(self, path, **kwargs):
+        with opener(path, file_system=self.file_system) as file:
+            with rasterio.open(file) as src:
+                self._add_meta_from_src(src)
+                out_shape = self._get_shape_from_res(self.res)
 
-    def __pow__(self, exponent):
-        self.check_for_array()
-        self.array = self.array**exponent
-        return self
+                if hasattr(self, "_warped_crs"):
+                    src = WarpedVRT(src, crs=self.crs)
 
-    def _return_self_or_copy(self, array, copy: bool):
-        if not copy:
-            self.array = array
-            return self
+                self.array = src.read(
+                    out_shape=out_shape,
+                    **(self.read_kwargs | kwargs),
+                )
+                if self._dtype:
+                    self = self.astype(self.dtype)
+                else:
+                    self = self.as_minimum_dtype()
+
+    def _read_with_mask(self, mask, masked, boundless, **kwargs):
+        kwargs["mask"] = mask
+
+        def _read(self, src, mask, **kwargs):
+            self._add_meta_from_src(src)
+            if self.bounds is None:
+                self._bounds = to_bbox(mask)
+
+            window = rasterio.windows.from_bounds(
+                *to_bbox(mask), transform=self.transform
+            )
+
+            out_shape = get_shape_from_bounds(mask, self.res)
+
+            kwargs = (
+                {"window": window, "boundless": boundless} | self.read_kwargs | kwargs
+            )
+
+            if hasattr(self, "_warped_crs"):
+                src = WarpedVRT(src, crs=self.crs)
+
+            self.array = src.read(out_shape=out_shape, **kwargs)
+
+            if not masked:
+                self.array[self.array.mask] = self.nodata
+                self.array = self.array.data
+
+            if boundless:
+                self._bounds = src.window_bounds(window=window)
+            else:
+                intersected = to_shapely(self.bounds).intersection(to_shapely(mask))
+                if intersected.is_empty:
+                    self._bounds = None
+                else:
+                    self._bounds = intersected.bounds
+
+            if not np.size(self.array):
+                return
+
+            if self._dtype:
+                self = self.astype(self._dtype)
+            else:
+                self = self.as_minimum_dtype()
+
+        if self.array is not None:
+            with memfile_from_array(self.array, **self.profile) as src:
+                _read(self, src, **kwargs)
         else:
-            copy = self.copy()
-            copy.array = array
-            return copy
+            with opener(self.path, file_system=self.file_system) as file:
+                with rasterio.open(file, **self.profile) as src:
+                    _read(self, src, **kwargs)
+
+    def _check_for_array(self, text=""):
+        if self.array is None:
+            raise ValueError("Arrays are not loaded. " + text)
+
+
+def get_transform_from_bounds(
+    obj: GeoDataFrame | GeoSeries | Geometry | tuple, shape: tuple[float, ...]
+) -> Affine:
+    minx, miny, maxx, maxy = to_bbox(obj)
+    if len(shape) == 2:
+        width, height = shape
+    elif len(shape) == 3:
+        _, width, height = shape
+    else:
+        raise ValueError
+    return rasterio.transform.from_bounds(minx, miny, maxx, maxy, width, height)
+
+
+def get_shape_from_bounds(
+    obj: GeoDataFrame | GeoSeries | Geometry | tuple, res: int
+) -> tuple[int, int]:
+    resx, resy = (res, res) if isinstance(res, numbers.Number) else res
+
+    minx, miny, maxx, maxy = to_bbox(obj)
+    diffx = maxx - minx
+    diffy = maxy - miny
+    width = int(diffx / resx)
+    heigth = int(diffy / resy)
+    return heigth, width
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ssb_sgis-0.3.9/src/sgis/raster/sentinel.py` & `ssb_sgis-1.0.0/src/sgis/raster/bands.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,34 @@
 import numpy as np
 
 from .raster import Raster
 
 
+SENTINEL2_FILENAME_REGEX = r"""
+    ^SENTINEL2X_
+    (?P<date>\d{8})
+    .*T(?P<tile>\d{2}[A-Z]{3})
+    .*(?:_(?P<resolution>{}m))?
+    .*(?P<band>B\d{1,2}A|B\d{1,2})
+    .*\..*$
+"""
+
+
 class Sentinel2(Raster):
+    filename_regex = SENTINEL2_FILENAME_REGEX
+    date_format: str = "%Y%m%d"
+
+    _profile = {
+        "driver": "GTiff",
+        "compress": "LZW",
+        "dtype": np.uint16,
+        "nodata": 0,
+        "indexes": 1,
+    }
+
     band_colors = {
         "B1": "coastal aerosol",
         "B2": "blue",
         "B3": "green",
         "B4": "red",
         "B5": "vegetation red edge",
         "B6": "vegetation red edge",
@@ -16,28 +37,12 @@
         "B8A": "narrow nir",
         "B9": "water vapour",
         "B10": "swir - cirrus",
         "B11": "swir",
         "B12": "swir",
     }
 
-    def __init__(self, raster=None, **kwargs):
-        kwargs = {
-            "nodata": 0,
-            "dtype": np.uint16,
-            "band_index": 1,
-            "name_regex": r"B\d{1,2}A|B\d{1,2}",
-            "date_regex": r"20\d{6}",
-            "shortname": "sentinel2",
-        } | kwargs
-
-        super().__init__(raster, **kwargs)
-
     @property
     def band_color(self):
-        if not self.name:
+        if not self.band:
             return None
-        return self.colors[self.name]
-
-    @property
-    def is_mask(self):
-        return "masks" in str(self.path).lower()
+        return self.band_colors[self.band]
```

### Comparing `ssb_sgis-0.3.9/src/sgis/raster/zonal.py` & `ssb_sgis-1.0.0/src/sgis/raster/zonal.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,32 +32,32 @@
     array_func: Callable,
     aggfunc,
     func_names,
     by_date,
 ) -> pd.DataFrame:
     cube = cube.copy()
     i, polygon = poly_iter
-    if not by_date or cube.df["date"].isna().all():
+    if not by_date or cube.date.isna().all():
         df = _clip_and_aggregate(
             cube, polygon, array_func, aggfunc, func_names, date=None, i=i
         )
         return df if by_date else df.drop(columns="date")
 
     out = []
 
-    na_date = cube.query("date.isna()")
+    na_date = cube[cube.date.isna()]
     df = _clip_and_aggregate(
         na_date, polygon, array_func, aggfunc, func_names, date=pd.NA, i=i
     )
     out.append(df)
 
-    cube.df = cube.df[lambda x: x["date"].notna()]
+    cube = cube[lambda x: x["date"].notna()]
 
-    for dt in cube.df["date"].unique():
-        cube_date = cube.query(f"date == {dt}")
+    for dt in cube.date.unique():
+        cube_date = cube[cube.date == dt]
         df = _clip_and_aggregate(
             cube_date, polygon, array_func, aggfunc, func_names, dt, i
         )
         out.append(df)
 
     return pd.concat(out)
 
@@ -69,15 +69,16 @@
     return df
 
 
 def _clip_and_aggregate(cube, polygon, array_func, aggfunc, func_names, date, i):
     if not len(cube):
         return _no_overlap_df(func_names, i, date)
     clipped = cube.clipmerge(polygon)
-    if not len(clipped) or clipped.arrays.isna().all():
+    print(list(clipped))
+    if not len(clipped) or [arr is None for arr in clipped.arrays]:
         return _no_overlap_df(func_names, i, date)
     assert len(clipped) == 1
     array = clipped[0].array
     df = _aggregate(array, array_func, aggfunc, func_names, date, i)
     return df
```

### Comparing `ssb_sgis-0.3.9/PKG-INFO` & `ssb_sgis-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 Metadata-Version: 2.1
 Name: ssb-sgis
-Version: 0.3.9
+Version: 1.0.0
 Summary: GIS functions used at Statistics Norway.
 Home-page: https://github.com/statisticsnorway/ssb-sgis
 License: MIT
 Author: Statistics Norway
 Author-email: ort@ssb.no
 Requires-Python: >=3.10,<4
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Dist: branca (>=0.6.0)
+Requires-Dist: dask (>=2024.1.1)
 Requires-Dist: folium (>=0.14.0)
-Requires-Dist: geocoder (>=1.38.1,<2.0.0)
+Requires-Dist: geocoder (>=1.38.1)
 Requires-Dist: geopandas (==0.14.0)
 Requires-Dist: igraph (==0.11.2)
 Requires-Dist: ipython (>=8.13.2)
 Requires-Dist: jenkspy (>=0.3.2)
 Requires-Dist: mapclassify (>=2.5.0)
 Requires-Dist: matplotlib (>=3.7.0)
 Requires-Dist: networkx (>=3.0)
-Requires-Dist: numba (>=0.57.1,<0.58.0)
 Requires-Dist: numpy (>=1.24.2)
-Requires-Dist: pandas (>=1.5.3)
+Requires-Dist: pandas (==2.0.3)
 Requires-Dist: pip (==23.2.1)
 Requires-Dist: pyarrow (>=11.0.0)
-Requires-Dist: rasterio (>=1.3.8,<2.0.0)
+Requires-Dist: rasterio (>=1.3.8)
 Requires-Dist: requests (>=2.28.2)
-Requires-Dist: rioxarray (>=0.14.1,<0.15.0)
-Requires-Dist: rtree (>=1.0.1,<2.0.0)
+Requires-Dist: rtree (>=1.0.1)
 Requires-Dist: scikit-learn (>=1.2.1)
 Requires-Dist: shapely (>=2.0.1)
-Requires-Dist: xarray (==2023.8.0)
 Requires-Dist: xyzservices (>=2023.2.0)
 Project-URL: Changelog, https://github.com/statisticsnorway/ssb-sgis/releases
 Project-URL: Repository, https://github.com/statisticsnorway/ssb-sgis
 Description-Content-Type: text/markdown
 
 # ssb-sgis
```

