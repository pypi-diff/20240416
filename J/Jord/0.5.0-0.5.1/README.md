# Comparing `tmp/Jord-0.5.0.tar.gz` & `tmp/jord-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jord-0.5.0.tar", last modified: Fri Mar 22 09:56:07 2024, max compression
+gzip compressed data, was "jord-0.5.1.tar", last modified: Tue Apr 16 07:37:18 2024, max compression
```

## Comparing `Jord-0.5.0.tar` & `jord-0.5.1.tar`

### file list

```diff
@@ -1,159 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.273641 Jord-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.245641 Jord-0.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-03-22 09:55:59.000000 Jord-0.5.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-22 09:55:59.000000 Jord-0.5.0/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-22 09:55:59.000000 Jord-0.5.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 09:55:59.000000 Jord-0.5.0/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.265641 Jord-0.5.0/Jord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-03-22 09:56:07.000000 Jord-0.5.0/Jord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-03-22 09:56:07.000000 Jord-0.5.0/Jord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 09:56:07.000000 Jord-0.5.0/Jord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-22 09:56:07.000000 Jord-0.5.0/Jord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-22 09:56:07.000000 Jord-0.5.0/Jord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-22 09:55:59.000000 Jord-0.5.0/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-03-22 09:55:59.000000 Jord-0.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-22 09:55:59.000000 Jord-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-03-22 09:56:07.273641 Jord-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-03-22 09:55:59.000000 Jord-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-22 09:55:59.000000 Jord-0.5.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.245641 Jord-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-22 09:55:59.000000 Jord-0.5.0/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.245641 Jord-0.5.0/jord/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1484 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.245641 Jord-0.5.0/jord/fiona_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/fiona_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/fiona_utilities/deserialise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.249641 Jord-0.5.0/jord/gdal_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/gdal_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      672 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/gdal_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1087 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/gdal_utilities/cloning.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1077 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/gdal_utilities/context.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2228 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/gdal_utilities/conversion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      491 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/gdal_utilities/drivers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      404 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/gdal_utilities/enums.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      768 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/gdal_utilities/error_handling.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1231 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/gdal_utilities/importing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2750 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/gdal_utilities/persistence.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/gdal_utilities/spatial_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.249641 Jord-0.5.0/jord/geojson_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/geojson_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/geojson_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      704 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/geojson_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.249641 Jord-0.5.0/jord/geometric_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/geometric_analysis/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/geometric_analysis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5638 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/geometric_analysis/center_line.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      394 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/geometric_analysis/degrees_of_freedom.py
--rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/geometric_analysis/intersections.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/geometric_analysis/tracing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.249641 Jord-0.5.0/jord/geopandas_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/geopandas_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       82 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/geopandas_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      756 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/geopandas_utilities/geometry_filtering.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/geopandas_utilities/importing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.253641 Jord-0.5.0/jord/geopandas_utilities/serialisation/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/geopandas_utilities/serialisation/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      303 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/geopandas_utilities/serialisation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      673 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/geopandas_utilities/serialisation/well_known_binary.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1226 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/geopandas_utilities/serialisation/well_known_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.253641 Jord-0.5.0/jord/networkx_utilities/
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/networkx_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/networkx_utilities/construction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.253641 Jord-0.5.0/jord/pillow_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/pillow_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      455 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/pillow_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      280 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/pillow_utilities/exif.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      476 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/pillow_utilities/tiff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.257641 Jord-0.5.0/jord/qgis_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      937 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3350 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/categorisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.257641 Jord-0.5.0/jord/qgis_utilities/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/configuration/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      300 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/configuration/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1057 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/configuration/plugin_settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3233 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/configuration/project_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.257641 Jord-0.5.0/jord/qgis_utilities/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/conversion/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/conversion/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      128 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/conversion/parsing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14840 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/data_provider.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1296 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/geo_interface_serialisation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      915 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.257641 Jord-0.5.0/jord/qgis_utilities/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/helpers/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      454 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/helpers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2484 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/helpers/actions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1088 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/helpers/drawing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6589 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/helpers/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/helpers/groups.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1780 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/helpers/models.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3566 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/helpers/progress_bar.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1208 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/helpers/sessions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2077 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/helpers/signals.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1223 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/helpers/timestamp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      460 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/importing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13707 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/layer_creation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2128 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/layer_serialisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.261641 Jord-0.5.0/jord/qgis_utilities/numpy_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/numpy_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/numpy_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2676 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/numpy_utilities/conversion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4075 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/numpy_utilities/data_type.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2925 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      474 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/numpy_utilities/rasters.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      392 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/plugin_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/styles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1933 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qgis_utilities/styling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.261641 Jord-0.5.0/jord/qlive_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qlive_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qlive_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1862 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qlive_utilities/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.261641 Jord-0.5.0/jord/qlive_utilities/clients/
--rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qlive_utilities/clients/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      447 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qlive_utilities/clients/arguments.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2865 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qlive_utilities/clients/auto.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qlive_utilities/clients/batching.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qlive_utilities/clients/interfaced.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qlive_utilities/pandas_procedures.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20181 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qlive_utilities/procedures.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2544 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qlive_utilities/serialisation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qlive_utilities/uri_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.261641 Jord-0.5.0/jord/qt_utilities/
--rwxr-xr-x   0 runner    (1001) docker     (127)      240 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qt_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23854 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/qt_utilities/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.261641 Jord-0.5.0/jord/rasterio_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/rasterio_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/rasterio_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.265641 Jord-0.5.0/jord/shapely_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/shapely_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      558 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/shapely_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/shapely_utilities/base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8327 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/shapely_utilities/clamp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1907 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/shapely_utilities/geometry_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/shapely_utilities/grouping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27412 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/shapely_utilities/lines.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      918 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/shapely_utilities/mirroring.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9931 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/shapely_utilities/morphology.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4177 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/shapely_utilities/points.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12570 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/shapely_utilities/polygons.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5885 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/shapely_utilities/projection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2796 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/shapely_utilities/rings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      585 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/shapely_utilities/selection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2902 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/shapely_utilities/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.265641 Jord-0.5.0/jord/spatialite_utilities/
--rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/spatialite_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      241 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/spatialite_utilities/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.265641 Jord-0.5.0/jord/torch_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:00.000000 Jord-0.5.0/jord/torch_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-22 09:56:00.000000 Jord-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-22 09:56:00.000000 Jord-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-22 09:56:07.273641 Jord-0.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     9495 2024-03-22 09:56:00.000000 Jord-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.265641 Jord-0.5.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:56:07.265641 Jord-0.5.0/tests/qgis/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-22 09:56:00.000000 Jord-0.5.0/tests/qgis/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1997 2024-03-22 09:56:00.000000 Jord-0.5.0/tests/test_import.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      471 2024-03-22 09:56:00.000000 Jord-0.5.0/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.920349 jord-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.892350 jord-0.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-16 07:37:15.000000 jord-0.5.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-16 07:37:15.000000 jord-0.5.1/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-16 07:37:15.000000 jord-0.5.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:15.000000 jord-0.5.1/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.912349 jord-0.5.1/Jord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-16 07:37:18.000000 jord-0.5.1/Jord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-16 07:37:18.000000 jord-0.5.1/Jord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:37:18.000000 jord-0.5.1/Jord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-16 07:37:18.000000 jord-0.5.1/Jord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 07:37:18.000000 jord-0.5.1/Jord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-16 07:37:15.000000 jord-0.5.1/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-04-16 07:37:15.000000 jord-0.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-16 07:37:15.000000 jord-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-16 07:37:18.920349 jord-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-16 07:37:15.000000 jord-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-16 07:37:15.000000 jord-0.5.1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.892350 jord-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-16 07:37:15.000000 jord-0.5.1/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.892350 jord-0.5.1/jord/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 07:37:15.000000 jord-0.5.1/jord/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1484 2024-04-16 07:37:15.000000 jord-0.5.1/jord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.892350 jord-0.5.1/jord/fiona_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:15.000000 jord-0.5.1/jord/fiona_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-04-16 07:37:15.000000 jord-0.5.1/jord/fiona_utilities/deserialise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.896350 jord-0.5.1/jord/gdal_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 07:37:15.000000 jord-0.5.1/jord/gdal_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      672 2024-04-16 07:37:15.000000 jord-0.5.1/jord/gdal_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1087 2024-04-16 07:37:15.000000 jord-0.5.1/jord/gdal_utilities/cloning.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1077 2024-04-16 07:37:15.000000 jord-0.5.1/jord/gdal_utilities/context.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2228 2024-04-16 07:37:15.000000 jord-0.5.1/jord/gdal_utilities/conversion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      491 2024-04-16 07:37:15.000000 jord-0.5.1/jord/gdal_utilities/drivers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      404 2024-04-16 07:37:15.000000 jord-0.5.1/jord/gdal_utilities/enums.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      768 2024-04-16 07:37:15.000000 jord-0.5.1/jord/gdal_utilities/error_handling.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1231 2024-04-16 07:37:15.000000 jord-0.5.1/jord/gdal_utilities/importing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2750 2024-04-16 07:37:15.000000 jord-0.5.1/jord/gdal_utilities/persistence.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-16 07:37:15.000000 jord-0.5.1/jord/gdal_utilities/spatial_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.896350 jord-0.5.1/jord/geojson_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geojson_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geojson_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      704 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geojson_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.896350 jord-0.5.1/jord/geometric_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geometric_analysis/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geometric_analysis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5638 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geometric_analysis/center_line.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      394 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geometric_analysis/degrees_of_freedom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geometric_analysis/intersections.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geometric_analysis/tracing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.896350 jord-0.5.1/jord/geopandas_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geopandas_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       82 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geopandas_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      756 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geopandas_utilities/geometry_filtering.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geopandas_utilities/importing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.900349 jord-0.5.1/jord/geopandas_utilities/serialisation/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geopandas_utilities/serialisation/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      303 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geopandas_utilities/serialisation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      673 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geopandas_utilities/serialisation/well_known_binary.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1226 2024-04-16 07:37:15.000000 jord-0.5.1/jord/geopandas_utilities/serialisation/well_known_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.900349 jord-0.5.1/jord/networkx_utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-04-16 07:37:15.000000 jord-0.5.1/jord/networkx_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-16 07:37:15.000000 jord-0.5.1/jord/networkx_utilities/construction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.900349 jord-0.5.1/jord/pillow_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 07:37:15.000000 jord-0.5.1/jord/pillow_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      455 2024-04-16 07:37:15.000000 jord-0.5.1/jord/pillow_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      280 2024-04-16 07:37:15.000000 jord-0.5.1/jord/pillow_utilities/exif.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      476 2024-04-16 07:37:15.000000 jord-0.5.1/jord/pillow_utilities/tiff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.900349 jord-0.5.1/jord/qgis_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      937 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3476 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/categorisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.904349 jord-0.5.1/jord/qgis_utilities/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/configuration/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      300 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/configuration/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1057 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/configuration/plugin_settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3233 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/configuration/project_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.904349 jord-0.5.1/jord/qgis_utilities/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/conversion/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/conversion/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      128 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/conversion/parsing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14840 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/data_provider.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1296 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/geo_interface_serialisation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      915 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.904349 jord-0.5.1/jord/qgis_utilities/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      477 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2484 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/actions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1088 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/drawing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6589 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1780 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3566 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/progress_bar.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1208 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/sessions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2077 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/signals.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1223 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/helpers/timestamp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      460 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/importing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13965 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/layer_creation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2128 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/layer_serialisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.904349 jord-0.5.1/jord/qgis_utilities/numpy_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/numpy_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/numpy_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2676 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/numpy_utilities/conversion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4075 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/numpy_utilities/data_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2925 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      474 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/numpy_utilities/rasters.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      392 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/plugin_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/styles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1933 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qgis_utilities/styling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.908349 jord-0.5.1/jord/qlive_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1862 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.908349 jord-0.5.1/jord/qlive_utilities/clients/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/clients/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      447 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/clients/arguments.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2865 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/clients/auto.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/clients/batching.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/clients/interfaced.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/pandas_procedures.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20181 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/procedures.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2544 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/serialisation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qlive_utilities/uri_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.908349 jord-0.5.1/jord/qt_utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      240 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qt_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23854 2024-04-16 07:37:15.000000 jord-0.5.1/jord/qt_utilities/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.908349 jord-0.5.1/jord/rasterio_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 07:37:15.000000 jord-0.5.1/jord/rasterio_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-16 07:37:15.000000 jord-0.5.1/jord/rasterio_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.912349 jord-0.5.1/jord/shapely_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      558 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8327 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/clamp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1907 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/geometry_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/grouping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27412 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/lines.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      918 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/mirroring.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9931 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/morphology.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4177 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/points.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12570 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/polygons.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5885 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/projection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2796 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/rings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      585 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/selection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2902 2024-04-16 07:37:15.000000 jord-0.5.1/jord/shapely_utilities/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.912349 jord-0.5.1/jord/spatialite_utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-04-16 07:37:15.000000 jord-0.5.1/jord/spatialite_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      241 2024-04-16 07:37:15.000000 jord-0.5.1/jord/spatialite_utilities/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.912349 jord-0.5.1/jord/torch_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:15.000000 jord-0.5.1/jord/torch_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-16 07:37:15.000000 jord-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-16 07:37:15.000000 jord-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-16 07:37:18.920349 jord-0.5.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9495 2024-04-16 07:37:15.000000 jord-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.912349 jord-0.5.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:18.912349 jord-0.5.1/tests/qgis/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-16 07:37:15.000000 jord-0.5.1/tests/qgis/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1997 2024-04-16 07:37:15.000000 jord-0.5.1/tests/test_import.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      471 2024-04-16 07:37:15.000000 jord-0.5.1/tests/test_sanity.py
```

### Comparing `Jord-0.5.0/.github/CODE_OF_CONDUCT.md` & `jord-0.5.1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/.github/CONTRIBUTING.md` & `jord-0.5.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/Jord.egg-info/PKG-INFO` & `jord-0.5.1/Jord.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.5.0
+Version: 0.5.1
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Lindbjerg
 Author-email: chen@mapspeople.dk
 Maintainer: Christian Heider Lindbjerg
 Maintainer-email: chen@mapspeople.dk
 License: Apache License, Version 2.0
@@ -27,94 +27,94 @@
 Requires-Dist: draugr>=1.0.9
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: pyzmq
 Requires-Dist: sorcery
 Requires-Dist: sympy
 Requires-Dist: tqdm
 Requires-Dist: warg>=1.1.6
-Provides-Extra: samples
-Provides-Extra: gdal
 Provides-Extra: dev
-Requires-Dist: pytest>=4.3.0; extra == "dev"
-Requires-Dist: pyzmq; extra == "dev"
-Requires-Dist: pytest>=4.4.1; extra == "dev"
-Requires-Dist: apppath>=1.0.2; extra == "dev"
-Requires-Dist: twine>=1.13.0; extra == "dev"
-Requires-Dist: numpy>=1.20.0; extra == "dev"
-Requires-Dist: draugr>=1.0.9; extra == "dev"
-Requires-Dist: sorcery; extra == "dev"
-Requires-Dist: sphinx>=4.0.1; extra == "dev"
-Requires-Dist: sympy; extra == "dev"
-Requires-Dist: pre-commit>=2.17.0; extra == "dev"
 Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
+Requires-Dist: draugr>=1.0.9; extra == "dev"
+Requires-Dist: pytest>=4.4.1; extra == "dev"
+Requires-Dist: black[jupyter]>=21.5b0; extra == "dev"
 Requires-Dist: pip>=22.1.2; extra == "dev"
+Requires-Dist: sympy; extra == "dev"
+Requires-Dist: wheel>=0.33.0; extra == "dev"
+Requires-Dist: pyzmq; extra == "dev"
+Requires-Dist: sorcery; extra == "dev"
+Requires-Dist: furo; extra == "dev"
 Requires-Dist: mock; extra == "dev"
+Requires-Dist: sphinx>=4.0.1; extra == "dev"
+Requires-Dist: tqdm; extra == "dev"
+Requires-Dist: apppath>=1.0.2; extra == "dev"
+Requires-Dist: coveralls>=1.6.0; extra == "dev"
 Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
+Requires-Dist: pytest>=4.3.0; extra == "dev"
+Requires-Dist: numpy>=1.20.0; extra == "dev"
 Requires-Dist: warg>=1.1.6; extra == "dev"
-Requires-Dist: wheel>=0.33.0; extra == "dev"
-Requires-Dist: black[jupyter]>=21.5b0; extra == "dev"
-Requires-Dist: coveralls>=1.6.0; extra == "dev"
-Requires-Dist: tqdm; extra == "dev"
-Requires-Dist: furo; extra == "dev"
-Provides-Extra: q
-Requires-Dist: pyqt5-tools; extra == "q"
+Requires-Dist: pre-commit>=2.17.0; extra == "dev"
+Requires-Dist: twine>=1.13.0; extra == "dev"
+Provides-Extra: tests
+Requires-Dist: pytest>=4.4.1; extra == "tests"
+Requires-Dist: mock; extra == "tests"
+Provides-Extra: docs
+Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
+Requires-Dist: sphinx>=4.0.1; extra == "docs"
+Requires-Dist: furo; extra == "docs"
 Provides-Extra: shapely
-Requires-Dist: shapely; extra == "shapely"
 Requires-Dist: pyproj; extra == "shapely"
+Requires-Dist: shapely; extra == "shapely"
+Provides-Extra: q
+Requires-Dist: pyqt5-tools; extra == "q"
+Provides-Extra: setup
+Provides-Extra: network
+Requires-Dist: networkx; extra == "network"
 Provides-Extra: legacy
-Requires-Dist: importlib-resources; extra == "legacy"
 Requires-Dist: importlib-metadata; extra == "legacy"
+Requires-Dist: importlib-resources; extra == "legacy"
 Provides-Extra: pil
 Requires-Dist: Pillow; extra == "pil"
-Provides-Extra: extra
-Provides-Extra: network
-Requires-Dist: networkx; extra == "network"
-Provides-Extra: docs
-Requires-Dist: sphinx>=4.0.1; extra == "docs"
-Requires-Dist: furo; extra == "docs"
-Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
-Provides-Extra: setup
-Provides-Extra: geopandas
-Requires-Dist: geopandas; extra == "geopandas"
-Provides-Extra: tests
-Requires-Dist: pytest>=4.4.1; extra == "tests"
-Requires-Dist: mock; extra == "tests"
 Provides-Extra: fiona
 Requires-Dist: fiona; extra == "fiona"
+Provides-Extra: geopandas
+Requires-Dist: geopandas; extra == "geopandas"
+Provides-Extra: samples
+Provides-Extra: gdal
+Provides-Extra: extra
 Provides-Extra: all
-Requires-Dist: networkx; extra == "all"
-Requires-Dist: importlib-metadata; extra == "all"
-Requires-Dist: pytest>=4.3.0; extra == "all"
-Requires-Dist: pyzmq; extra == "all"
-Requires-Dist: pytest>=4.4.1; extra == "all"
-Requires-Dist: apppath>=1.0.2; extra == "all"
-Requires-Dist: twine>=1.13.0; extra == "all"
-Requires-Dist: numpy>=1.20.0; extra == "all"
+Requires-Dist: pytest-cov>=2.11.1; extra == "all"
+Requires-Dist: pre-commit>=2.17.0; extra == "all"
 Requires-Dist: draugr>=1.0.9; extra == "all"
-Requires-Dist: shapely; extra == "all"
-Requires-Dist: sorcery; extra == "all"
-Requires-Dist: sphinx>=4.0.1; extra == "all"
+Requires-Dist: pytest>=4.4.1; extra == "all"
+Requires-Dist: pyqt5-tools; extra == "all"
 Requires-Dist: fiona; extra == "all"
-Requires-Dist: sympy; extra == "all"
-Requires-Dist: pyproj; extra == "all"
-Requires-Dist: pre-commit>=2.17.0; extra == "all"
 Requires-Dist: Pillow; extra == "all"
-Requires-Dist: pytest-cov>=2.11.1; extra == "all"
+Requires-Dist: importlib-resources; extra == "all"
+Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
 Requires-Dist: pip>=22.1.2; extra == "all"
-Requires-Dist: geopandas; extra == "all"
+Requires-Dist: networkx; extra == "all"
+Requires-Dist: sympy; extra == "all"
+Requires-Dist: wheel>=0.33.0; extra == "all"
+Requires-Dist: pyzmq; extra == "all"
+Requires-Dist: sorcery; extra == "all"
+Requires-Dist: shapely; extra == "all"
+Requires-Dist: furo; extra == "all"
 Requires-Dist: mock; extra == "all"
+Requires-Dist: sphinx>=4.0.1; extra == "all"
+Requires-Dist: apppath>=1.0.2; extra == "all"
+Requires-Dist: geopandas; extra == "all"
+Requires-Dist: coveralls>=1.6.0; extra == "all"
 Requires-Dist: sphinxcontrib-programoutput; extra == "all"
+Requires-Dist: pytest>=4.3.0; extra == "all"
+Requires-Dist: importlib-metadata; extra == "all"
+Requires-Dist: numpy>=1.20.0; extra == "all"
 Requires-Dist: warg>=1.1.6; extra == "all"
-Requires-Dist: importlib-resources; extra == "all"
-Requires-Dist: wheel>=0.33.0; extra == "all"
-Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
-Requires-Dist: coveralls>=1.6.0; extra == "all"
-Requires-Dist: pyqt5-tools; extra == "all"
+Requires-Dist: pyproj; extra == "all"
 Requires-Dist: tqdm; extra == "all"
-Requires-Dist: furo; extra == "all"
+Requires-Dist: twine>=1.13.0; extra == "all"
 
 <!--![header](.github/images/header.png)-->
 
 <p align="center">
   <img src=".github/images/header.svg" alt='header' />
 </p>
```

### Comparing `Jord-0.5.0/Jord.egg-info/SOURCES.txt` & `jord-0.5.1/Jord.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 jord/qgis_utilities/conversion/parsing.py
 jord/qgis_utilities/helpers/README.md
 jord/qgis_utilities/helpers/__init__.py
 jord/qgis_utilities/helpers/actions.py
 jord/qgis_utilities/helpers/drawing.py
 jord/qgis_utilities/helpers/environment.py
 jord/qgis_utilities/helpers/groups.py
+jord/qgis_utilities/helpers/logging.py
 jord/qgis_utilities/helpers/models.py
 jord/qgis_utilities/helpers/progress_bar.py
 jord/qgis_utilities/helpers/sessions.py
 jord/qgis_utilities/helpers/signals.py
 jord/qgis_utilities/helpers/timestamp.py
 jord/qgis_utilities/numpy_utilities/README.md
 jord/qgis_utilities/numpy_utilities/__init__.py
```

### Comparing `Jord-0.5.0/Jord.egg-info/requires.txt` & `jord-0.5.1/Jord.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -4,86 +4,86 @@
 pyzmq
 sorcery
 sympy
 tqdm
 warg>=1.1.6
 
 [all]
-networkx
-importlib-metadata
-pytest>=4.3.0
-pyzmq
-pytest>=4.4.1
-apppath>=1.0.2
-twine>=1.13.0
-numpy>=1.20.0
+pytest-cov>=2.11.1
+pre-commit>=2.17.0
 draugr>=1.0.9
-shapely
-sorcery
-sphinx>=4.0.1
+pytest>=4.4.1
+pyqt5-tools
 fiona
-sympy
-pyproj
-pre-commit>=2.17.0
 Pillow
-pytest-cov>=2.11.1
+importlib-resources
+black[jupyter]>=21.5b0
 pip>=22.1.2
-geopandas
+networkx
+sympy
+wheel>=0.33.0
+pyzmq
+sorcery
+shapely
+furo
 mock
+sphinx>=4.0.1
+apppath>=1.0.2
+geopandas
+coveralls>=1.6.0
 sphinxcontrib-programoutput
+pytest>=4.3.0
+importlib-metadata
+numpy>=1.20.0
 warg>=1.1.6
-importlib-resources
-wheel>=0.33.0
-black[jupyter]>=21.5b0
-coveralls>=1.6.0
-pyqt5-tools
+pyproj
 tqdm
-furo
+twine>=1.13.0
 
 [dev]
-pytest>=4.3.0
-pyzmq
-pytest>=4.4.1
-apppath>=1.0.2
-twine>=1.13.0
-numpy>=1.20.0
-draugr>=1.0.9
-sorcery
-sphinx>=4.0.1
-sympy
-pre-commit>=2.17.0
 pytest-cov>=2.11.1
+draugr>=1.0.9
+pytest>=4.4.1
+black[jupyter]>=21.5b0
 pip>=22.1.2
+sympy
+wheel>=0.33.0
+pyzmq
+sorcery
+furo
 mock
+sphinx>=4.0.1
+tqdm
+apppath>=1.0.2
+coveralls>=1.6.0
 sphinxcontrib-programoutput
+pytest>=4.3.0
+numpy>=1.20.0
 warg>=1.1.6
-wheel>=0.33.0
-black[jupyter]>=21.5b0
-coveralls>=1.6.0
-tqdm
-furo
+pre-commit>=2.17.0
+twine>=1.13.0
 
 [docs]
+sphinxcontrib-programoutput
 sphinx>=4.0.1
 furo
-sphinxcontrib-programoutput
 
 [extra]
 
 [fiona]
 fiona
 
 [gdal]
 
 [geopandas]
 geopandas
 
 [legacy]
-importlib-resources
 importlib-metadata
+importlib-resources
 
 [network]
 networkx
 
 [pil]
 Pillow
 
@@ -91,13 +91,13 @@
 pyqt5-tools
 
 [samples]
 
 [setup]
 
 [shapely]
-shapely
 pyproj
+shapely
 
 [tests]
 pytest>=4.4.1
 mock
```

### Comparing `Jord-0.5.0/LICENSE.md` & `jord-0.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/PKG-INFO` & `jord-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.5.0
+Version: 0.5.1
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Lindbjerg
 Author-email: chen@mapspeople.dk
 Maintainer: Christian Heider Lindbjerg
 Maintainer-email: chen@mapspeople.dk
 License: Apache License, Version 2.0
@@ -27,94 +27,94 @@
 Requires-Dist: draugr>=1.0.9
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: pyzmq
 Requires-Dist: sorcery
 Requires-Dist: sympy
 Requires-Dist: tqdm
 Requires-Dist: warg>=1.1.6
-Provides-Extra: samples
-Provides-Extra: gdal
 Provides-Extra: dev
-Requires-Dist: pytest>=4.3.0; extra == "dev"
-Requires-Dist: pyzmq; extra == "dev"
-Requires-Dist: pytest>=4.4.1; extra == "dev"
-Requires-Dist: apppath>=1.0.2; extra == "dev"
-Requires-Dist: twine>=1.13.0; extra == "dev"
-Requires-Dist: numpy>=1.20.0; extra == "dev"
-Requires-Dist: draugr>=1.0.9; extra == "dev"
-Requires-Dist: sorcery; extra == "dev"
-Requires-Dist: sphinx>=4.0.1; extra == "dev"
-Requires-Dist: sympy; extra == "dev"
-Requires-Dist: pre-commit>=2.17.0; extra == "dev"
 Requires-Dist: pytest-cov>=2.11.1; extra == "dev"
+Requires-Dist: draugr>=1.0.9; extra == "dev"
+Requires-Dist: pytest>=4.4.1; extra == "dev"
+Requires-Dist: black[jupyter]>=21.5b0; extra == "dev"
 Requires-Dist: pip>=22.1.2; extra == "dev"
+Requires-Dist: sympy; extra == "dev"
+Requires-Dist: wheel>=0.33.0; extra == "dev"
+Requires-Dist: pyzmq; extra == "dev"
+Requires-Dist: sorcery; extra == "dev"
+Requires-Dist: furo; extra == "dev"
 Requires-Dist: mock; extra == "dev"
+Requires-Dist: sphinx>=4.0.1; extra == "dev"
+Requires-Dist: tqdm; extra == "dev"
+Requires-Dist: apppath>=1.0.2; extra == "dev"
+Requires-Dist: coveralls>=1.6.0; extra == "dev"
 Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
+Requires-Dist: pytest>=4.3.0; extra == "dev"
+Requires-Dist: numpy>=1.20.0; extra == "dev"
 Requires-Dist: warg>=1.1.6; extra == "dev"
-Requires-Dist: wheel>=0.33.0; extra == "dev"
-Requires-Dist: black[jupyter]>=21.5b0; extra == "dev"
-Requires-Dist: coveralls>=1.6.0; extra == "dev"
-Requires-Dist: tqdm; extra == "dev"
-Requires-Dist: furo; extra == "dev"
-Provides-Extra: q
-Requires-Dist: pyqt5-tools; extra == "q"
+Requires-Dist: pre-commit>=2.17.0; extra == "dev"
+Requires-Dist: twine>=1.13.0; extra == "dev"
+Provides-Extra: tests
+Requires-Dist: pytest>=4.4.1; extra == "tests"
+Requires-Dist: mock; extra == "tests"
+Provides-Extra: docs
+Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
+Requires-Dist: sphinx>=4.0.1; extra == "docs"
+Requires-Dist: furo; extra == "docs"
 Provides-Extra: shapely
-Requires-Dist: shapely; extra == "shapely"
 Requires-Dist: pyproj; extra == "shapely"
+Requires-Dist: shapely; extra == "shapely"
+Provides-Extra: q
+Requires-Dist: pyqt5-tools; extra == "q"
+Provides-Extra: setup
+Provides-Extra: network
+Requires-Dist: networkx; extra == "network"
 Provides-Extra: legacy
-Requires-Dist: importlib-resources; extra == "legacy"
 Requires-Dist: importlib-metadata; extra == "legacy"
+Requires-Dist: importlib-resources; extra == "legacy"
 Provides-Extra: pil
 Requires-Dist: Pillow; extra == "pil"
-Provides-Extra: extra
-Provides-Extra: network
-Requires-Dist: networkx; extra == "network"
-Provides-Extra: docs
-Requires-Dist: sphinx>=4.0.1; extra == "docs"
-Requires-Dist: furo; extra == "docs"
-Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
-Provides-Extra: setup
-Provides-Extra: geopandas
-Requires-Dist: geopandas; extra == "geopandas"
-Provides-Extra: tests
-Requires-Dist: pytest>=4.4.1; extra == "tests"
-Requires-Dist: mock; extra == "tests"
 Provides-Extra: fiona
 Requires-Dist: fiona; extra == "fiona"
+Provides-Extra: geopandas
+Requires-Dist: geopandas; extra == "geopandas"
+Provides-Extra: samples
+Provides-Extra: gdal
+Provides-Extra: extra
 Provides-Extra: all
-Requires-Dist: networkx; extra == "all"
-Requires-Dist: importlib-metadata; extra == "all"
-Requires-Dist: pytest>=4.3.0; extra == "all"
-Requires-Dist: pyzmq; extra == "all"
-Requires-Dist: pytest>=4.4.1; extra == "all"
-Requires-Dist: apppath>=1.0.2; extra == "all"
-Requires-Dist: twine>=1.13.0; extra == "all"
-Requires-Dist: numpy>=1.20.0; extra == "all"
+Requires-Dist: pytest-cov>=2.11.1; extra == "all"
+Requires-Dist: pre-commit>=2.17.0; extra == "all"
 Requires-Dist: draugr>=1.0.9; extra == "all"
-Requires-Dist: shapely; extra == "all"
-Requires-Dist: sorcery; extra == "all"
-Requires-Dist: sphinx>=4.0.1; extra == "all"
+Requires-Dist: pytest>=4.4.1; extra == "all"
+Requires-Dist: pyqt5-tools; extra == "all"
 Requires-Dist: fiona; extra == "all"
-Requires-Dist: sympy; extra == "all"
-Requires-Dist: pyproj; extra == "all"
-Requires-Dist: pre-commit>=2.17.0; extra == "all"
 Requires-Dist: Pillow; extra == "all"
-Requires-Dist: pytest-cov>=2.11.1; extra == "all"
+Requires-Dist: importlib-resources; extra == "all"
+Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
 Requires-Dist: pip>=22.1.2; extra == "all"
-Requires-Dist: geopandas; extra == "all"
+Requires-Dist: networkx; extra == "all"
+Requires-Dist: sympy; extra == "all"
+Requires-Dist: wheel>=0.33.0; extra == "all"
+Requires-Dist: pyzmq; extra == "all"
+Requires-Dist: sorcery; extra == "all"
+Requires-Dist: shapely; extra == "all"
+Requires-Dist: furo; extra == "all"
 Requires-Dist: mock; extra == "all"
+Requires-Dist: sphinx>=4.0.1; extra == "all"
+Requires-Dist: apppath>=1.0.2; extra == "all"
+Requires-Dist: geopandas; extra == "all"
+Requires-Dist: coveralls>=1.6.0; extra == "all"
 Requires-Dist: sphinxcontrib-programoutput; extra == "all"
+Requires-Dist: pytest>=4.3.0; extra == "all"
+Requires-Dist: importlib-metadata; extra == "all"
+Requires-Dist: numpy>=1.20.0; extra == "all"
 Requires-Dist: warg>=1.1.6; extra == "all"
-Requires-Dist: importlib-resources; extra == "all"
-Requires-Dist: wheel>=0.33.0; extra == "all"
-Requires-Dist: black[jupyter]>=21.5b0; extra == "all"
-Requires-Dist: coveralls>=1.6.0; extra == "all"
-Requires-Dist: pyqt5-tools; extra == "all"
+Requires-Dist: pyproj; extra == "all"
 Requires-Dist: tqdm; extra == "all"
-Requires-Dist: furo; extra == "all"
+Requires-Dist: twine>=1.13.0; extra == "all"
 
 <!--![header](.github/images/header.png)-->
 
 <p align="center">
   <img src=".github/images/header.svg" alt='header' />
 </p>
```

### Comparing `Jord-0.5.0/README.md` & `jord-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/SECURITY.md` & `jord-0.5.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/__init__.py` & `jord-0.5.1/jord/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     from importlib_metadata import PackageNotFoundError
     from importlib_resources import files
 
 from warg import package_is_editable, clean_string, get_version
 
 __project__ = "Jord"
 __author__ = "Christian Heider Lindbjerg"
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 __doc__ = r"""
 .. module:: jord
    :platform: Unix, Windows
    :synopsis: A set of general tools build for geo data.
 
 .. moduleauthor:: Christian Heider Lindbjerg <chen@mapspeople.dk>
```

### Comparing `Jord-0.5.0/jord/fiona_utilities/deserialise.py` & `jord-0.5.1/jord/fiona_utilities/deserialise.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/gdal_utilities/__init__.py` & `jord-0.5.1/jord/gdal_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/gdal_utilities/cloning.py` & `jord-0.5.1/jord/gdal_utilities/cloning.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/gdal_utilities/context.py` & `jord-0.5.1/jord/gdal_utilities/context.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/gdal_utilities/conversion.py` & `jord-0.5.1/jord/gdal_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/gdal_utilities/error_handling.py` & `jord-0.5.1/jord/gdal_utilities/error_handling.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/gdal_utilities/importing.py` & `jord-0.5.1/jord/gdal_utilities/importing.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/gdal_utilities/persistence.py` & `jord-0.5.1/jord/gdal_utilities/persistence.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/geojson_utilities/geometry_types.py` & `jord-0.5.1/jord/geojson_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/geometric_analysis/center_line.py` & `jord-0.5.1/jord/geometric_analysis/center_line.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/geometric_analysis/intersections.py` & `jord-0.5.1/jord/geometric_analysis/intersections.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/geopandas_utilities/geometry_filtering.py` & `jord-0.5.1/jord/geopandas_utilities/geometry_filtering.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/geopandas_utilities/serialisation/well_known_binary.py` & `jord-0.5.1/jord/geopandas_utilities/serialisation/well_known_binary.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/geopandas_utilities/serialisation/well_known_text.py` & `jord-0.5.1/jord/geopandas_utilities/serialisation/well_known_text.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/networkx_utilities/construction.py` & `jord-0.5.1/jord/networkx_utilities/construction.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qgis_utilities/__init__.py` & `jord-0.5.1/jord/qgis_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qgis_utilities/categorisation.py` & `jord-0.5.1/jord/qgis_utilities/categorisation.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,15 +68,19 @@
 
     if isinstance(iterable, Callable) and not isinstance(iterable, Generator):
         # noinspection PyCallingNonCallable
         iterable = iterable()  # Compat
 
     color_iter = iter(iterable)
 
-    assert field_name in layer.fields().names()
+    available_field_names = layer.fields().names()
+
+    assert (
+        field_name in available_field_names
+    ), f"Did not find {field_name=} in {available_field_names=}"
 
     render_categories = []
     for cat in layer.uniqueValues(layer.fields().indexFromName(field_name)):
         if cat:
             sym = QgsSymbol.defaultSymbol(layer.geometryType())
             col = next(color_iter)
```

### Comparing `Jord-0.5.0/jord/qgis_utilities/configuration/plugin_settings.py` & `jord-0.5.1/jord/qgis_utilities/configuration/plugin_settings.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qgis_utilities/configuration/project_settings.py` & `jord-0.5.1/jord/qgis_utilities/configuration/project_settings.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qgis_utilities/data_provider.py` & `jord-0.5.1/jord/qgis_utilities/data_provider.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qgis_utilities/enums.py` & `jord-0.5.1/jord/qgis_utilities/enums.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qgis_utilities/geo_interface_serialisation.py` & `jord-0.5.1/jord/qgis_utilities/geo_interface_serialisation.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qgis_utilities/geometry_types.py` & `jord-0.5.1/jord/qgis_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qgis_utilities/helpers/actions.py` & `jord-0.5.1/jord/qgis_utilities/helpers/actions.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qgis_utilities/helpers/drawing.py` & `jord-0.5.1/jord/qgis_utilities/helpers/drawing.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qgis_utilities/helpers/environment.py` & `jord-0.5.1/jord/qgis_utilities/helpers/environment.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qgis_utilities/helpers/groups.py` & `jord-0.5.1/jord/qgis_utilities/helpers/groups.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qgis_utilities/helpers/models.py` & `jord-0.5.1/jord/qgis_utilities/helpers/models.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qgis_utilities/helpers/progress_bar.py` & `jord-0.5.1/jord/qgis_utilities/helpers/progress_bar.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qgis_utilities/helpers/sessions.py` & `jord-0.5.1/jord/qgis_utilities/helpers/sessions.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qgis_utilities/helpers/signals.py` & `jord-0.5.1/jord/qgis_utilities/helpers/signals.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qgis_utilities/helpers/timestamp.py` & `jord-0.5.1/jord/qgis_utilities/helpers/timestamp.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qgis_utilities/layer_creation.py` & `jord-0.5.1/jord/qgis_utilities/layer_creation.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,21 @@
         fields = None
 
     if categorise_by_attribute and fields:
         assert (
             categorise_by_attribute in fields
         ), f"{categorise_by_attribute} was not found in {fields}"
 
+    if not isinstance(qgis_instance_handle, QgsProject):
+        qgis_project = qgis_instance_handle.qgis_project
+    elif qgis_instance_handle is None:
+        qgis_project = QgsProject.instance()
+    else:
+        qgis_project = qgis_instance_handle
+
     if geom_type == GeoJsonGeometryTypesEnum.geometry_collection.value.__name__:
         for g in geom.asGeometryCollection():  # TODO: Look into recursion?
             uri = json.loads(g.asJson())["type"]
             if uri is None:
                 raise Exception(f"Could not load {g.asJson()} as json")
             sub_type = uri  # TODO: URI MIGHT BE NONE?
 
@@ -146,24 +153,21 @@
             sub_layer.commitChanges()
             sub_layer.updateFields()
             sub_layer.updateExtents()
 
             return_collection.append(sub_layer)
 
             if group:
-                qgis_instance_handle.qgis_project.addMapLayer(sub_layer, False)
+
+                qgis_project.addMapLayer(sub_layer, False)
                 group.insertLayer(0, sub_layer)
             else:
-                qgis_instance_handle.qgis_project.addMapLayer(sub_layer)
+                qgis_project.addMapLayer(sub_layer)
 
-            layer_tree_handle = (
-                qgis_instance_handle.qgis_project.layerTreeRoot().findLayer(
-                    sub_layer.id()
-                )
-            )
+            layer_tree_handle = qgis_project.layerTreeRoot().findLayer(sub_layer.id())
             if layer_tree_handle:
                 layer_tree_handle.setItemVisibilityChecked(visible)
     else:
         uri += "?"
 
         if crs:
             uri += f"crs={crs}"
@@ -207,22 +211,20 @@
         layer.commitChanges()
         layer.updateFields()
         layer.updateExtents()
 
         return_collection.append(layer)
 
         if group:
-            qgis_instance_handle.qgis_project.addMapLayer(layer, False)
+            qgis_project.addMapLayer(layer, False)
             group.insertLayer(0, layer)
         else:
-            qgis_instance_handle.qgis_project.addMapLayer(layer)
+            qgis_project.addMapLayer(layer)
 
-        layer_tree_handle = qgis_instance_handle.qgis_project.layerTreeRoot().findLayer(
-            layer.id()
-        )
+        layer_tree_handle = qgis_project.layerTreeRoot().findLayer(layer.id())
         if layer_tree_handle:
             layer_tree_handle.setItemVisibilityChecked(visible)
 
     actions = qgis.utils.iface.layerTreeView().defaultActions()
     actions.showFeatureCount()
     actions.showFeatureCount()  # TODO: Duplicate?
 
@@ -282,19 +284,24 @@
     :param name:
     :param crs:
     :param columns:
     :param index:
     :return:
     """
 
-    # noinspection PyUnresolvedReferences
-    from qgis.core import QgsVectorLayer, QgsFeature
     from .categorisation import categorise_layer
 
     # noinspection PyUnresolvedReferences
+    from qgis.core import (
+        QgsFeature,
+        QgsVectorLayer,
+        QgsProject,
+    )
+
+    # noinspection PyUnresolvedReferences
     import qgis
 
     # uri = geom.type()
     # uri = geom.wkbType()
     # uri = geom.wktTypeStr()
 
     return_collection = []
@@ -418,23 +425,28 @@
     if categorise_by_attribute:
         categorise_layer(layer, categorise_by_attribute)
 
     layer.commitChanges()
     layer.updateFields()
     layer.updateExtents()
 
+    if not isinstance(qgis_instance_handle, QgsProject):
+        qgis_project = qgis_instance_handle.qgis_project
+    elif qgis_instance_handle is None:
+        qgis_project = QgsProject.instance()
+    else:
+        qgis_project = qgis_instance_handle
+
     if group:
-        qgis_instance_handle.qgis_project.addMapLayer(layer, False)
+        qgis_project.addMapLayer(layer, False)
         group.insertLayer(0, layer)
     else:
-        qgis_instance_handle.qgis_project.addMapLayer(layer)
+        qgis_project.addMapLayer(layer)
 
-    layer_tree_handle = qgis_instance_handle.qgis_project.layerTreeRoot().findLayer(
-        layer.id()
-    )
+    layer_tree_handle = qgis_project.layerTreeRoot().findLayer(layer.id())
     if layer_tree_handle:
         layer_tree_handle.setItemVisibilityChecked(visible)
 
     actions = qgis.utils.iface.layerTreeView().defaultActions()
     actions.showFeatureCount()  # TODO: Twice?
     actions.showFeatureCount()
```

### Comparing `Jord-0.5.0/jord/qgis_utilities/layer_serialisation.py` & `jord-0.5.1/jord/qgis_utilities/layer_serialisation.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qgis_utilities/numpy_utilities/conversion.py` & `jord-0.5.1/jord/qgis_utilities/numpy_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qgis_utilities/numpy_utilities/data_type.py` & `jord-0.5.1/jord/qgis_utilities/numpy_utilities/data_type.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py` & `jord-0.5.1/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qgis_utilities/styles.py` & `jord-0.5.1/jord/qgis_utilities/styles.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qgis_utilities/styling.py` & `jord-0.5.1/jord/qgis_utilities/styling.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qlive_utilities/client.py` & `jord-0.5.1/jord/qlive_utilities/client.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qlive_utilities/clients/auto.py` & `jord-0.5.1/jord/qlive_utilities/clients/auto.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qlive_utilities/procedures.py` & `jord-0.5.1/jord/qlive_utilities/procedures.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qlive_utilities/serialisation.py` & `jord-0.5.1/jord/qlive_utilities/serialisation.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qlive_utilities/uri_utilities.py` & `jord-0.5.1/jord/qlive_utilities/uri_utilities.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/qt_utilities/enums.py` & `jord-0.5.1/jord/qt_utilities/enums.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/shapely_utilities/__init__.py` & `jord-0.5.1/jord/shapely_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/shapely_utilities/base.py` & `jord-0.5.1/jord/shapely_utilities/base.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/shapely_utilities/clamp.py` & `jord-0.5.1/jord/shapely_utilities/clamp.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/shapely_utilities/geometry_types.py` & `jord-0.5.1/jord/shapely_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/shapely_utilities/grouping.py` & `jord-0.5.1/jord/shapely_utilities/grouping.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/shapely_utilities/lines.py` & `jord-0.5.1/jord/shapely_utilities/lines.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/shapely_utilities/mirroring.py` & `jord-0.5.1/jord/shapely_utilities/mirroring.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/shapely_utilities/morphology.py` & `jord-0.5.1/jord/shapely_utilities/morphology.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/shapely_utilities/points.py` & `jord-0.5.1/jord/shapely_utilities/points.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/shapely_utilities/polygons.py` & `jord-0.5.1/jord/shapely_utilities/polygons.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/shapely_utilities/projection.py` & `jord-0.5.1/jord/shapely_utilities/projection.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/shapely_utilities/rings.py` & `jord-0.5.1/jord/shapely_utilities/rings.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/shapely_utilities/selection.py` & `jord-0.5.1/jord/shapely_utilities/selection.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/jord/shapely_utilities/transformation.py` & `jord-0.5.1/jord/shapely_utilities/transformation.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/setup.py` & `jord-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `Jord-0.5.0/tests/test_import.py` & `jord-0.5.1/tests/test_import.py`

 * *Files identical despite different names*

