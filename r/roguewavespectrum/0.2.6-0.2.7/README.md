# Comparing `tmp/roguewavespectrum-0.2.6.tar.gz` & `tmp/roguewavespectrum-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roguewavespectrum-0.2.6.tar", last modified: Wed Mar 27 00:03:35 2024, max compression
+gzip compressed data, was "roguewavespectrum-0.2.7.tar", last modified: Mon Apr 15 22:38:01 2024, max compression
```

## Comparing `roguewavespectrum-0.2.6.tar` & `roguewavespectrum-0.2.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-03-27 00:03:35.025546 roguewavespectrum-0.2.6/
--rw-r--r--   0 pietersmit   (502) staff       (20)    11357 2023-08-20 18:47:38.000000 roguewavespectrum-0.2.6/LICENSE
--rw-r--r--   0 pietersmit   (502) staff       (20)      947 2024-03-27 00:03:35.025254 roguewavespectrum-0.2.6/PKG-INFO
--rw-r--r--   0 pietersmit   (502) staff       (20)      288 2023-11-25 03:33:55.000000 roguewavespectrum-0.2.6/README.md
--rw-r--r--   0 pietersmit   (502) staff       (20)       38 2024-03-27 00:03:35.025639 roguewavespectrum-0.2.6/setup.cfg
--rw-r--r--   0 pietersmit   (502) staff       (20)     1350 2024-03-27 00:03:17.000000 roguewavespectrum-0.2.6/setup.py
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-03-27 00:03:35.009017 roguewavespectrum-0.2.6/src/
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-03-27 00:03:35.016540 roguewavespectrum-0.2.6/src/roguewavespectrum/
--rw-r--r--   0 pietersmit   (502) staff       (20)    17787 2024-01-20 00:31:35.000000 roguewavespectrum-0.2.6/src/roguewavespectrum/__init__.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     4306 2023-10-21 02:34:11.000000 roguewavespectrum-0.2.6/src/roguewavespectrum/_directions.py
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-03-27 00:03:35.019517 roguewavespectrum-0.2.6/src/roguewavespectrum/_estimators/
--rw-r--r--   0 pietersmit   (502) staff       (20)      658 2023-10-21 02:24:56.000000 roguewavespectrum-0.2.6/src/roguewavespectrum/_estimators/__init__.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     4697 2023-10-21 01:52:04.000000 roguewavespectrum-0.2.6/src/roguewavespectrum/_estimators/estimate.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     3862 2023-10-21 01:52:04.000000 roguewavespectrum-0.2.6/src/roguewavespectrum/_estimators/mem.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    28728 2023-11-27 00:48:14.000000 roguewavespectrum-0.2.6/src/roguewavespectrum/_estimators/mem2.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    16427 2023-12-22 18:30:38.000000 roguewavespectrum-0.2.6/src/roguewavespectrum/_factory_methods.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     1432 2024-01-23 21:48:48.000000 roguewavespectrum-0.2.6/src/roguewavespectrum/_geospatial.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     3275 2024-01-20 00:31:35.000000 roguewavespectrum-0.2.6/src/roguewavespectrum/_operations.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    16190 2023-11-25 03:33:55.000000 roguewavespectrum-0.2.6/src/roguewavespectrum/_partitioning.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     3902 2023-10-21 01:52:04.000000 roguewavespectrum-0.2.6/src/roguewavespectrum/_physical_constants.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    79503 2024-03-26 23:59:44.000000 roguewavespectrum-0.2.6/src/roguewavespectrum/_spectrum.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    21216 2023-11-27 00:51:17.000000 roguewavespectrum-0.2.6/src/roguewavespectrum/_spline_interpolation.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     3514 2023-10-21 01:52:04.000000 roguewavespectrum-0.2.6/src/roguewavespectrum/_time.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     2922 2023-11-25 03:33:55.000000 roguewavespectrum-0.2.6/src/roguewavespectrum/_timeseries.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    16274 2023-11-27 00:51:17.000000 roguewavespectrum-0.2.6/src/roguewavespectrum/_variable_names.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    27327 2023-11-25 03:33:55.000000 roguewavespectrum-0.2.6/src/roguewavespectrum/parametric.py
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-03-27 00:03:35.022105 roguewavespectrum-0.2.6/src/roguewavespectrum/spotter/
--rw-r--r--   0 pietersmit   (502) staff       (20)     5066 2024-01-20 00:31:35.000000 roguewavespectrum-0.2.6/src/roguewavespectrum/spotter/__init__.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     9651 2024-01-20 00:31:35.000000 roguewavespectrum-0.2.6/src/roguewavespectrum/spotter/_spotter_extrapolate_tail.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     3802 2024-01-20 00:31:35.000000 roguewavespectrum-0.2.6/src/roguewavespectrum/spotter/_spotter_post_processing.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     2762 2024-01-20 00:31:35.000000 roguewavespectrum-0.2.6/src/roguewavespectrum/spotter/_spotter_sdcard_data.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    12122 2024-01-20 00:31:36.000000 roguewavespectrum-0.2.6/src/roguewavespectrum/spotter/_spotter_time_integration.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    16780 2024-01-23 21:48:48.000000 roguewavespectrum-0.2.6/src/roguewavespectrum/spotter/_spotter_wavefleet_api.py
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-03-27 00:03:35.017916 roguewavespectrum-0.2.6/src/roguewavespectrum.egg-info/
--rw-r--r--   0 pietersmit   (502) staff       (20)      947 2024-03-27 00:03:34.000000 roguewavespectrum-0.2.6/src/roguewavespectrum.egg-info/PKG-INFO
--rw-r--r--   0 pietersmit   (502) staff       (20)     1398 2024-03-27 00:03:34.000000 roguewavespectrum-0.2.6/src/roguewavespectrum.egg-info/SOURCES.txt
--rw-r--r--   0 pietersmit   (502) staff       (20)        1 2024-03-27 00:03:34.000000 roguewavespectrum-0.2.6/src/roguewavespectrum.egg-info/dependency_links.txt
--rw-r--r--   0 pietersmit   (502) staff       (20)      129 2024-03-27 00:03:34.000000 roguewavespectrum-0.2.6/src/roguewavespectrum.egg-info/requires.txt
--rw-r--r--   0 pietersmit   (502) staff       (20)       18 2024-03-27 00:03:34.000000 roguewavespectrum-0.2.6/src/roguewavespectrum.egg-info/top_level.txt
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-03-27 00:03:35.024652 roguewavespectrum-0.2.6/test/
--rw-r--r--   0 pietersmit   (502) staff       (20)     1776 2023-10-27 21:23:45.000000 roguewavespectrum-0.2.6/test/test_directions.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     8227 2023-11-25 03:33:55.000000 roguewavespectrum-0.2.6/test/test_factory_methods.py
--rw-r--r--   0 pietersmit   (502) staff       (20)      876 2024-02-28 21:55:38.000000 roguewavespectrum-0.2.6/test/test_geospatial.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     2188 2023-10-21 21:15:35.000000 roguewavespectrum-0.2.6/test/test_parametric.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    19854 2024-03-27 00:02:22.000000 roguewavespectrum-0.2.6/test/test_spectrum.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     3820 2023-10-21 01:52:04.000000 roguewavespectrum-0.2.6/test/test_timeseries.py
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-04-15 22:38:01.088642 roguewavespectrum-0.2.7/
+-rw-r--r--   0 pietersmit   (502) staff       (20)    11357 2023-08-20 18:47:38.000000 roguewavespectrum-0.2.7/LICENSE
+-rw-r--r--   0 pietersmit   (502) staff       (20)      947 2024-04-15 22:38:01.088504 roguewavespectrum-0.2.7/PKG-INFO
+-rw-r--r--   0 pietersmit   (502) staff       (20)      288 2023-11-25 03:33:55.000000 roguewavespectrum-0.2.7/README.md
+-rw-r--r--   0 pietersmit   (502) staff       (20)       38 2024-04-15 22:38:01.088682 roguewavespectrum-0.2.7/setup.cfg
+-rw-r--r--   0 pietersmit   (502) staff       (20)     1350 2024-04-15 22:37:35.000000 roguewavespectrum-0.2.7/setup.py
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-04-15 22:38:01.077732 roguewavespectrum-0.2.7/src/
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-04-15 22:38:01.082438 roguewavespectrum-0.2.7/src/roguewavespectrum/
+-rw-r--r--   0 pietersmit   (502) staff       (20)    17787 2024-01-20 00:31:35.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/__init__.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     4306 2023-10-21 02:34:11.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_directions.py
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-04-15 22:38:01.084590 roguewavespectrum-0.2.7/src/roguewavespectrum/_estimators/
+-rw-r--r--   0 pietersmit   (502) staff       (20)      658 2023-10-21 02:24:56.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_estimators/__init__.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     4697 2023-10-21 01:52:04.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_estimators/estimate.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     3862 2023-10-21 01:52:04.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_estimators/mem.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    28728 2023-11-27 00:48:14.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_estimators/mem2.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    16922 2024-04-15 22:37:17.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_factory_methods.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     1432 2024-01-23 21:48:48.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_geospatial.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     3275 2024-01-20 00:31:35.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_operations.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    16190 2023-11-25 03:33:55.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_partitioning.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     3902 2023-10-21 01:52:04.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_physical_constants.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    79503 2024-03-26 23:59:44.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_spectrum.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    21216 2023-11-27 00:51:17.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_spline_interpolation.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     3514 2023-10-21 01:52:04.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_time.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     2922 2023-11-25 03:33:55.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_timeseries.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    16274 2023-11-27 00:51:17.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/_variable_names.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    27327 2023-11-25 03:33:55.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/parametric.py
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-04-15 22:38:01.086314 roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/
+-rw-r--r--   0 pietersmit   (502) staff       (20)     5066 2024-01-20 00:31:35.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/__init__.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     9651 2024-01-20 00:31:35.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/_spotter_extrapolate_tail.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     3802 2024-01-20 00:31:35.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/_spotter_post_processing.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     2762 2024-01-20 00:31:35.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/_spotter_sdcard_data.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    12122 2024-01-20 00:31:36.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/_spotter_time_integration.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    16780 2024-01-23 21:48:48.000000 roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/_spotter_wavefleet_api.py
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-04-15 22:38:01.083519 roguewavespectrum-0.2.7/src/roguewavespectrum.egg-info/
+-rw-r--r--   0 pietersmit   (502) staff       (20)      947 2024-04-15 22:38:01.000000 roguewavespectrum-0.2.7/src/roguewavespectrum.egg-info/PKG-INFO
+-rw-r--r--   0 pietersmit   (502) staff       (20)     1398 2024-04-15 22:38:01.000000 roguewavespectrum-0.2.7/src/roguewavespectrum.egg-info/SOURCES.txt
+-rw-r--r--   0 pietersmit   (502) staff       (20)        1 2024-04-15 22:38:01.000000 roguewavespectrum-0.2.7/src/roguewavespectrum.egg-info/dependency_links.txt
+-rw-r--r--   0 pietersmit   (502) staff       (20)      129 2024-04-15 22:38:01.000000 roguewavespectrum-0.2.7/src/roguewavespectrum.egg-info/requires.txt
+-rw-r--r--   0 pietersmit   (502) staff       (20)       18 2024-04-15 22:38:01.000000 roguewavespectrum-0.2.7/src/roguewavespectrum.egg-info/top_level.txt
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2024-04-15 22:38:01.088194 roguewavespectrum-0.2.7/test/
+-rw-r--r--   0 pietersmit   (502) staff       (20)     1776 2023-10-27 21:23:45.000000 roguewavespectrum-0.2.7/test/test_directions.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     8227 2023-11-25 03:33:55.000000 roguewavespectrum-0.2.7/test/test_factory_methods.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)      876 2024-02-28 21:55:38.000000 roguewavespectrum-0.2.7/test/test_geospatial.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     2188 2023-10-21 21:15:35.000000 roguewavespectrum-0.2.7/test/test_parametric.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    19854 2024-03-27 00:02:22.000000 roguewavespectrum-0.2.7/test/test_spectrum.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     3820 2023-10-21 01:52:04.000000 roguewavespectrum-0.2.7/test/test_timeseries.py
```

### Comparing `roguewavespectrum-0.2.6/LICENSE` & `roguewavespectrum-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/PKG-INFO` & `roguewavespectrum-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roguewavespectrum
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python package that implements a spectral object for ocean surface gravity waves
 Home-page: https://github.com/sofarocean/oceanwavespectrum.git
 Author: Pieter Bart Smit
 Author-email: sofaroceangithubbot@gmail.com
 License: Apache 2 License
 Project-URL: Sofar Ocean Site, https://www.sofarocean.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `roguewavespectrum-0.2.6/setup.py` & `roguewavespectrum-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     readme_contents = file.read()
 
 setuptools.setup(
     name="roguewavespectrum",
-    version="0.2.6",
+    version="0.2.7",
     license="Apache 2 License",
     install_requires=[
         "numpy",
         "numba",
         "linearwavetheory",
         "xarray",
         "scipy",
```

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum/__init__.py` & `roguewavespectrum-0.2.7/src/roguewavespectrum/__init__.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum/_directions.py` & `roguewavespectrum-0.2.7/src/roguewavespectrum/_directions.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum/_estimators/__init__.py` & `roguewavespectrum-0.2.7/src/roguewavespectrum/_estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum/_estimators/estimate.py` & `roguewavespectrum-0.2.7/src/roguewavespectrum/_estimators/estimate.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum/_estimators/mem.py` & `roguewavespectrum-0.2.7/src/roguewavespectrum/_estimators/mem.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum/_estimators/mem2.py` & `roguewavespectrum-0.2.7/src/roguewavespectrum/_estimators/mem2.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum/_factory_methods.py` & `roguewavespectrum-0.2.7/src/roguewavespectrum/_factory_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,33 +13,33 @@
     NAME_E,
     NAME_D,
     NAME_DEPTH,
 )
 
 import numpy as np
 from xarray import Dataset
-from typing import Union, Sequence, Literal
+from typing import Union, Sequence, Literal, Optional
 from roguewavespectrum.parametric import (
     create_dir_shape,
     create_freq_shape,
     parametric_directional_spectrum,
     parametric_spectrum,
 )
 from roguewavespectrum._operations import concatenate_spectra
 
 
 def create_spectrum1d(
     coordinates: Union[
         np.ndarray, tuple[str, np.ndarray], Sequence[tuple[str, np.ndarray]]
     ],
     variance_density: np.ndarray,
-    a1: np.ndarray,
-    b1: np.ndarray,
-    a2: np.ndarray,
-    b2: np.ndarray,
+    a1: Optional[np.ndarray] = None,
+    b1: Optional[np.ndarray] = None,
+    a2: Optional[np.ndarray] = None,
+    b2: Optional[np.ndarray] = None,
     **kwargs,
 ) -> Spectrum:
     """
     Create a roguewavespectrum.Spectrum1D object for a given 1D spectrum with a1/b1/a2/b2.
 
     :param coordinates:  A list of coordinates naming the dimension and giving the coordinate values. For a 1D spectrum
     that has dimensions [dim1,...,dimN,frequency] The list should take the form:
@@ -73,31 +73,40 @@
         coordinates = [coordinates]
 
     elif not isinstance(coordinates, Sequence):
         raise ValueError(
             "coordinates should be a numpy array or a sequence of tuples describing the coordinates"
         )
 
-    if not (a1.shape == b1.shape == a2.shape == b2.shape == variance_density.shape):
-        raise ValueError("a1,b1,a2,b2 and variance_density should have the same shape")
-
     if not coordinates[-1][0] == "frequency":
         raise ValueError("The last coordinate should be frequency")
 
     if len(coordinates) < variance_density.ndim:
         if len(coordinates) == 1:
             coordinates = [
                 (f"dim_{ndim}", np.arange(variance_density.shape[ndim]))
                 for ndim in range(variance_density.ndim - 1)
             ] + coordinates
         else:
             raise ValueError(
                 "The number of coordinates should match the number of dimensions of the variance_density"
             )
 
+    if (a1 is None) or (b1 is None) or (a2 is None) or (b2 is None):
+        if not ((a1 is None) and (b1 is None) and (a2 is None) and (b2 is None)):
+            raise ValueError("a1,b1,a2,b2 should all be None or all be numpy arrays")
+
+        a1 = np.ones_like(variance_density)
+        b1 = np.zeros_like(variance_density)
+        a2 = np.ones_like(variance_density)
+        b2 = np.zeros_like(variance_density)
+
+    if not (a1.shape == b1.shape == a2.shape == b2.shape == variance_density.shape):
+        raise ValueError("a1,b1,a2,b2 and variance_density should have the same shape")
+
     dims = [x[0] for x in coordinates]
     coords = {x[0]: x[1] for x in coordinates}
 
     if len(dims) != variance_density.ndim:
         raise ValueError(
             "The number of coordinates should match the number of dimensions of the variance_density"
         )
```

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum/_geospatial.py` & `roguewavespectrum-0.2.7/src/roguewavespectrum/_geospatial.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum/_operations.py` & `roguewavespectrum-0.2.7/src/roguewavespectrum/_operations.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum/_partitioning.py` & `roguewavespectrum-0.2.7/src/roguewavespectrum/_partitioning.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum/_physical_constants.py` & `roguewavespectrum-0.2.7/src/roguewavespectrum/_physical_constants.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum/_spectrum.py` & `roguewavespectrum-0.2.7/src/roguewavespectrum/_spectrum.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum/_spline_interpolation.py` & `roguewavespectrum-0.2.7/src/roguewavespectrum/_spline_interpolation.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum/_time.py` & `roguewavespectrum-0.2.7/src/roguewavespectrum/_time.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum/_timeseries.py` & `roguewavespectrum-0.2.7/src/roguewavespectrum/_timeseries.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum/_variable_names.py` & `roguewavespectrum-0.2.7/src/roguewavespectrum/_variable_names.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum/parametric.py` & `roguewavespectrum-0.2.7/src/roguewavespectrum/parametric.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum/spotter/__init__.py` & `roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/__init__.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum/spotter/_spotter_extrapolate_tail.py` & `roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/_spotter_extrapolate_tail.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum/spotter/_spotter_post_processing.py` & `roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/_spotter_post_processing.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum/spotter/_spotter_sdcard_data.py` & `roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/_spotter_sdcard_data.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum/spotter/_spotter_time_integration.py` & `roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/_spotter_time_integration.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum/spotter/_spotter_wavefleet_api.py` & `roguewavespectrum-0.2.7/src/roguewavespectrum/spotter/_spotter_wavefleet_api.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum.egg-info/PKG-INFO` & `roguewavespectrum-0.2.7/src/roguewavespectrum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roguewavespectrum
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python package that implements a spectral object for ocean surface gravity waves
 Home-page: https://github.com/sofarocean/oceanwavespectrum.git
 Author: Pieter Bart Smit
 Author-email: sofaroceangithubbot@gmail.com
 License: Apache 2 License
 Project-URL: Sofar Ocean Site, https://www.sofarocean.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `roguewavespectrum-0.2.6/src/roguewavespectrum.egg-info/SOURCES.txt` & `roguewavespectrum-0.2.7/src/roguewavespectrum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/test/test_directions.py` & `roguewavespectrum-0.2.7/test/test_directions.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/test/test_factory_methods.py` & `roguewavespectrum-0.2.7/test/test_factory_methods.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/test/test_geospatial.py` & `roguewavespectrum-0.2.7/test/test_geospatial.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/test/test_parametric.py` & `roguewavespectrum-0.2.7/test/test_parametric.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/test/test_spectrum.py` & `roguewavespectrum-0.2.7/test/test_spectrum.py`

 * *Files identical despite different names*

### Comparing `roguewavespectrum-0.2.6/test/test_timeseries.py` & `roguewavespectrum-0.2.7/test/test_timeseries.py`

 * *Files identical despite different names*

