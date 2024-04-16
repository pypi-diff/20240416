# Comparing `tmp/ecoscope-1.6.3.tar.gz` & `tmp/ecoscope-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoscope-1.6.3.tar", last modified: Tue Apr  9 07:54:46 2024, max compression
+gzip compressed data, was "ecoscope-1.7.0.tar", last modified: Tue Apr 16 09:39:52 2024, max compression
```

## Comparing `ecoscope-1.6.3.tar` & `ecoscope-1.7.0.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-09 07:54:46.256116 ecoscope-1.6.3/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1553 2024-04-09 07:51:27.000000 ecoscope-1.6.3/LICENSE
--rw-r--r--   0 gitonga   (1000) gitonga   (1000)     4430 2024-04-09 07:54:46.256116 ecoscope-1.6.3/PKG-INFO
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2946 2024-04-09 07:51:27.000000 ecoscope-1.6.3/README.rst
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-09 07:54:46.240115 ecoscope-1.6.3/ecoscope/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3762 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/__init__.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-09 07:54:46.244115 ecoscope-1.6.3/ecoscope/analysis/
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-09 07:54:46.244115 ecoscope-1.6.3/ecoscope/analysis/UD/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      105 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/analysis/UD/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7011 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/analysis/UD/etd_range.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      375 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/analysis/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1027 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/analysis/astronomy.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    15978 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/analysis/ecograph.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3849 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/analysis/geofence.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2955 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/analysis/immobility.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3208 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/analysis/percentile.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2147 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/analysis/proximity.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     4852 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/analysis/seasons.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2725 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/analysis/speed.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-09 07:54:46.248115 ecoscope-1.6.3/ecoscope/base/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      602 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/base/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1776 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/base/_dataclasses.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    25126 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/base/base.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7698 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/base/utils.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-09 07:54:46.248115 ecoscope-1.6.3/ecoscope/contrib/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       61 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/contrib/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    10988 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/contrib/basemaps.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)   123902 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/contrib/foliumap.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5197 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/contrib/geemap.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2359 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/contrib/legend.txt
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-09 07:54:46.248115 ecoscope-1.6.3/ecoscope/io/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      272 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/io/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    37546 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/io/earthranger.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    15218 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/io/eetools.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6616 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/io/raster.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1630 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/io/utils.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-09 07:54:46.248115 ecoscope-1.6.3/ecoscope/mapping/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      324 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/mapping/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    32305 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/mapping/map.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-09 07:54:46.252115 ecoscope-1.6.3/ecoscope/plotting/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      268 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/plotting/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7390 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/plotting/plot.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       22 2024-04-09 07:51:27.000000 ecoscope-1.6.3/ecoscope/version.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-09 07:54:46.256116 ecoscope-1.6.3/ecoscope.egg-info/
--rw-r--r--   0 gitonga   (1000) gitonga   (1000)     4430 2024-04-09 07:54:46.000000 ecoscope-1.6.3/ecoscope.egg-info/PKG-INFO
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1349 2024-04-09 07:54:46.000000 ecoscope-1.6.3/ecoscope.egg-info/SOURCES.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2024-04-09 07:54:46.000000 ecoscope-1.6.3/ecoscope.egg-info/dependency_links.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2024-04-09 07:54:45.000000 ecoscope-1.6.3/ecoscope.egg-info/not-zip-safe
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      277 2024-04-09 07:54:46.000000 ecoscope-1.6.3/ecoscope.egg-info/requires.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        9 2024-04-09 07:54:46.000000 ecoscope-1.6.3/ecoscope.egg-info/top_level.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      591 2024-04-09 07:51:27.000000 ecoscope-1.6.3/pyproject.toml
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       38 2024-04-09 07:54:46.256116 ecoscope-1.6.3/setup.cfg
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1969 2024-04-09 07:51:27.000000 ecoscope-1.6.3/setup.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-09 07:54:46.252115 ecoscope-1.6.3/tests/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7044 2024-04-09 07:51:27.000000 ecoscope-1.6.3/tests/test_base.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6694 2024-04-09 07:51:27.000000 ecoscope-1.6.3/tests/test_earthranger_io.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     4840 2024-04-09 07:51:27.000000 ecoscope-1.6.3/tests/test_ecodataframe.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5198 2024-04-09 07:51:27.000000 ecoscope-1.6.3/tests/test_ecograph.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6126 2024-04-09 07:51:27.000000 ecoscope-1.6.3/tests/test_ecomap.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5933 2024-04-09 07:51:27.000000 ecoscope-1.6.3/tests/test_eetools.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1876 2024-04-09 07:51:27.000000 ecoscope-1.6.3/tests/test_geofence.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      790 2024-04-09 07:51:27.000000 ecoscope-1.6.3/tests/test_immobility.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      962 2024-04-09 07:51:27.000000 ecoscope-1.6.3/tests/test_seasons.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      306 2024-04-09 07:51:27.000000 ecoscope-1.6.3/tests/test_speed.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2091 2024-04-09 07:51:27.000000 ecoscope-1.6.3/tests/test_ud.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      443 2024-04-09 07:51:27.000000 ecoscope-1.6.3/tests/test_utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-16 09:39:52.831373 ecoscope-1.7.0/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1553 2024-04-16 09:37:39.000000 ecoscope-1.7.0/LICENSE
+-rw-r--r--   0 gitonga   (1000) gitonga   (1000)     4430 2024-04-16 09:39:52.831373 ecoscope-1.7.0/PKG-INFO
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2946 2024-04-16 09:37:39.000000 ecoscope-1.7.0/README.rst
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-16 09:39:52.819373 ecoscope-1.7.0/ecoscope/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3762 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/__init__.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-16 09:39:52.823373 ecoscope-1.7.0/ecoscope/analysis/
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-16 09:39:52.823373 ecoscope-1.7.0/ecoscope/analysis/UD/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      105 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/analysis/UD/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7011 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/analysis/UD/etd_range.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      375 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/analysis/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1027 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/analysis/astronomy.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    15978 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/analysis/ecograph.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3849 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/analysis/geofence.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2955 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/analysis/immobility.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3208 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/analysis/percentile.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2147 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/analysis/proximity.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     4852 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/analysis/seasons.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2725 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/analysis/speed.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-16 09:39:52.823373 ecoscope-1.7.0/ecoscope/base/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      602 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/base/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1776 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/base/_dataclasses.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    25126 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/base/base.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7698 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/base/utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-16 09:39:52.827373 ecoscope-1.7.0/ecoscope/contrib/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       61 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/contrib/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    10988 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/contrib/basemaps.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)   123902 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/contrib/foliumap.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5197 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/contrib/geemap.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2359 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/contrib/legend.txt
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-16 09:39:52.827373 ecoscope-1.7.0/ecoscope/io/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      272 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/io/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    37546 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/io/earthranger.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    15218 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/io/eetools.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6616 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/io/raster.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2652 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/io/utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-16 09:39:52.827373 ecoscope-1.7.0/ecoscope/mapping/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      324 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/mapping/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    32305 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/mapping/map.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-16 09:39:52.827373 ecoscope-1.7.0/ecoscope/plotting/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      268 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/plotting/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7390 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/plotting/plot.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       22 2024-04-16 09:37:39.000000 ecoscope-1.7.0/ecoscope/version.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-16 09:39:52.831373 ecoscope-1.7.0/ecoscope.egg-info/
+-rw-r--r--   0 gitonga   (1000) gitonga   (1000)     4430 2024-04-16 09:39:52.000000 ecoscope-1.7.0/ecoscope.egg-info/PKG-INFO
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1372 2024-04-16 09:39:52.000000 ecoscope-1.7.0/ecoscope.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2024-04-16 09:39:52.000000 ecoscope-1.7.0/ecoscope.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2024-04-16 09:39:52.000000 ecoscope-1.7.0/ecoscope.egg-info/not-zip-safe
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      277 2024-04-16 09:39:52.000000 ecoscope-1.7.0/ecoscope.egg-info/requires.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        9 2024-04-16 09:39:52.000000 ecoscope-1.7.0/ecoscope.egg-info/top_level.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      591 2024-04-16 09:37:39.000000 ecoscope-1.7.0/pyproject.toml
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       38 2024-04-16 09:39:52.831373 ecoscope-1.7.0/setup.cfg
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1969 2024-04-16 09:37:39.000000 ecoscope-1.7.0/setup.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2024-04-16 09:39:52.831373 ecoscope-1.7.0/tests/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7044 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_base.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6694 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_earthranger_io.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     4840 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_ecodataframe.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5198 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_ecograph.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6126 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_ecomap.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5933 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_eetools.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1876 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_geofence.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      790 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_immobility.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2492 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_io_utils.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      962 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_seasons.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      306 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_speed.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2091 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_ud.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      443 2024-04-16 09:37:39.000000 ecoscope-1.7.0/tests/test_utils.py
```

### Comparing `ecoscope-1.6.3/LICENSE` & `ecoscope-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/PKG-INFO` & `ecoscope-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoscope
-Version: 1.6.3
+Version: 1.7.0
 Summary: Standard Analytical Reporting Framework for Conservation
 Home-page: http://github.com/wildlife-dynamics/ecoscope
 Author: Jake Wall
 Author-email: walljcg@gmail.com
 License: MIT
 Platform: Posix; MacOS X; Windows
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `ecoscope-1.6.3/README.rst` & `ecoscope-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope/__init__.py` & `ecoscope-1.7.0/ecoscope/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope/analysis/UD/etd_range.py` & `ecoscope-1.7.0/ecoscope/analysis/UD/etd_range.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope/analysis/astronomy.py` & `ecoscope-1.7.0/ecoscope/analysis/astronomy.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope/analysis/ecograph.py` & `ecoscope-1.7.0/ecoscope/analysis/ecograph.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope/analysis/geofence.py` & `ecoscope-1.7.0/ecoscope/analysis/geofence.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope/analysis/immobility.py` & `ecoscope-1.7.0/ecoscope/analysis/immobility.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope/analysis/percentile.py` & `ecoscope-1.7.0/ecoscope/analysis/percentile.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope/analysis/proximity.py` & `ecoscope-1.7.0/ecoscope/analysis/proximity.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope/analysis/seasons.py` & `ecoscope-1.7.0/ecoscope/analysis/seasons.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope/analysis/speed.py` & `ecoscope-1.7.0/ecoscope/analysis/speed.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope/base/__init__.py` & `ecoscope-1.7.0/ecoscope/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope/base/_dataclasses.py` & `ecoscope-1.7.0/ecoscope/base/_dataclasses.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope/base/base.py` & `ecoscope-1.7.0/ecoscope/base/base.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope/base/utils.py` & `ecoscope-1.7.0/ecoscope/base/utils.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope/contrib/basemaps.py` & `ecoscope-1.7.0/ecoscope/contrib/basemaps.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope/contrib/foliumap.py` & `ecoscope-1.7.0/ecoscope/contrib/foliumap.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope/contrib/geemap.py` & `ecoscope-1.7.0/ecoscope/contrib/geemap.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope/contrib/legend.txt` & `ecoscope-1.7.0/ecoscope/contrib/legend.txt`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope/io/earthranger.py` & `ecoscope-1.7.0/ecoscope/io/earthranger.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope/io/eetools.py` & `ecoscope-1.7.0/ecoscope/io/eetools.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope/io/raster.py` & `ecoscope-1.7.0/ecoscope/io/raster.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope/mapping/map.py` & `ecoscope-1.7.0/ecoscope/mapping/map.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope/plotting/plot.py` & `ecoscope-1.7.0/ecoscope/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/ecoscope.egg-info/PKG-INFO` & `ecoscope-1.7.0/ecoscope.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoscope
-Version: 1.6.3
+Version: 1.7.0
 Summary: Standard Analytical Reporting Framework for Conservation
 Home-page: http://github.com/wildlife-dynamics/ecoscope
 Author: Jake Wall
 Author-email: walljcg@gmail.com
 License: MIT
 Platform: Posix; MacOS X; Windows
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `ecoscope-1.6.3/ecoscope.egg-info/SOURCES.txt` & `ecoscope-1.7.0/ecoscope.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,11 +43,12 @@
 tests/test_earthranger_io.py
 tests/test_ecodataframe.py
 tests/test_ecograph.py
 tests/test_ecomap.py
 tests/test_eetools.py
 tests/test_geofence.py
 tests/test_immobility.py
+tests/test_io_utils.py
 tests/test_seasons.py
 tests/test_speed.py
 tests/test_ud.py
 tests/test_utils.py
```

### Comparing `ecoscope-1.6.3/pyproject.toml` & `ecoscope-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/setup.py` & `ecoscope-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/tests/test_base.py` & `ecoscope-1.7.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/tests/test_earthranger_io.py` & `ecoscope-1.7.0/tests/test_earthranger_io.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/tests/test_ecodataframe.py` & `ecoscope-1.7.0/tests/test_ecodataframe.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/tests/test_ecograph.py` & `ecoscope-1.7.0/tests/test_ecograph.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/tests/test_ecomap.py` & `ecoscope-1.7.0/tests/test_ecomap.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/tests/test_eetools.py` & `ecoscope-1.7.0/tests/test_eetools.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/tests/test_geofence.py` & `ecoscope-1.7.0/tests/test_geofence.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/tests/test_immobility.py` & `ecoscope-1.7.0/tests/test_immobility.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/tests/test_seasons.py` & `ecoscope-1.7.0/tests/test_seasons.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.6.3/tests/test_ud.py` & `ecoscope-1.7.0/tests/test_ud.py`

 * *Files identical despite different names*

