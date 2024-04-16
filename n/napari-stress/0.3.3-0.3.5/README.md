# Comparing `tmp/napari_stress-0.3.3.tar.gz` & `tmp/napari_stress-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_stress-0.3.3.tar", last modified: Sun Feb  4 12:30:12 2024, max compression
+gzip compressed data, was "napari_stress-0.3.5.tar", last modified: Tue Apr 16 12:57:17 2024, max compression
```

## Comparing `napari_stress-0.3.3.tar` & `napari_stress-0.3.5.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 12:30:12.283556 napari_stress-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-02-04 12:29:52.000000 napari_stress-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-04 12:29:52.000000 napari_stress-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-02-04 12:30:12.283556 napari_stress-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-02-04 12:29:52.000000 napari_stress-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-04 12:29:53.000000 napari_stress-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-02-04 12:30:12.283556 napari_stress-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-04 12:29:53.000000 napari_stress-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 12:30:12.263556 napari_stress-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 12:30:12.267556 napari_stress-0.3.3/src/napari_stress/
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 12:30:12.271556 napari_stress-0.3.3/src/napari_stress/_approximation/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_approximation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_approximation/expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_approximation/expansion_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_approximation/fit_ellipsoid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 12:30:12.271556 napari_stress-0.3.3/src/napari_stress/_measurements/
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_measurements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18703 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_measurements/curvature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_measurements/deviation_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    13684 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_measurements/geodesics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8368 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_measurements/intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_measurements/measurements.py
--rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_measurements/stresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_measurements/temporal_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)    27530 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_measurements/toolbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_measurements/toolbox.ui
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_napari_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 12:30:12.271556 napari_stress-0.3.3/src/napari_stress/_plotting/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11794 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_plotting/create_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 12:30:12.275556 napari_stress-0.3.3/src/napari_stress/_reconstruction/
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_reconstruction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_reconstruction/fit_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18144 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_reconstruction/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_reconstruction/reconstruct_surface.py
--rw-r--r--   0 runner    (1001) docker     (127)    11023 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_reconstruction/refine_surfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    14529 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_reconstruction/toolbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    15661 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_reconstruction/toolbox.ui
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 12:30:12.279556 napari_stress-0.3.3/src/napari_stress/_sample_data/
--rw-r--r--   0 runner    (1001) docker     (127)   354896 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_sample_data/ExampleTifSequence.tif
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_sample_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    66687 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_sample_data/dropplet_point_cloud.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1808756 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_sample_data/dropplet_point_cloud_4d.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_sample_data/sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 12:30:12.279556 napari_stress-0.3.3/src/napari_stress/_spherical_harmonics/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_spherical_harmonics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_spherical_harmonics/fit_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13386 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_spherical_harmonics/spherical_harmonics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_spherical_harmonics/spherical_harmonics_napari.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 12:30:12.279556 napari_stress-0.3.3/src/napari_stress/_stress/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_stress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_stress/charts_SPB.py
--rw-r--r--   0 runner    (1001) docker     (127)    82885 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_stress/euclidian_k_form_SPB.py
--rw-r--r--   0 runner    (1001) docker     (127)    26226 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_stress/lebedev_info_SPB.py
--rw-r--r--   0 runner    (1001) docker     (127)   145005 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_stress/lebedev_write_SPB.py
--rw-r--r--   0 runner    (1001) docker     (127)    72897 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_stress/manifold_SPB.py
--rw-r--r--   0 runner    (1001) docker     (127)    23955 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_stress/sph_func_SPB.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_surface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 12:30:12.283556 napari_stress-0.3.3/src/napari_stress/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_tests/test_approximation.py
--rw-r--r--   0 runner    (1001) docker     (127)    23387 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_tests/test_measurements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_tests/test_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_tests/test_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_tests/test_spherical_harmonic_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_tests/test_surface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_tests/test_vectors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 12:30:12.283556 napari_stress-0.3.3/src/napari_stress/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17285 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_utils/_aggregate_measurements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_utils/coordinate_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    23143 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_utils/frame_by_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_utils/import_export_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-02-04 12:29:53.000000 napari_stress-0.3.3/src/napari_stress/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 12:30:12.283556 napari_stress-0.3.3/src/napari_stress.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-02-04 12:30:12.000000 napari_stress-0.3.3/src/napari_stress.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-02-04 12:30:12.000000 napari_stress-0.3.3/src/napari_stress.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-04 12:30:12.000000 napari_stress-0.3.3/src/napari_stress.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-04 12:30:12.000000 napari_stress-0.3.3/src/napari_stress.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-04 12:30:12.000000 napari_stress-0.3.3/src/napari_stress.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-04 12:30:12.000000 napari_stress-0.3.3/src/napari_stress.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:57:17.019221 napari_stress-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-16 12:57:03.000000 napari_stress-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-16 12:57:03.000000 napari_stress-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-16 12:57:17.019221 napari_stress-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-16 12:57:03.000000 napari_stress-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-16 12:57:04.000000 napari_stress-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-16 12:57:17.019221 napari_stress-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-16 12:57:04.000000 napari_stress-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:57:17.003220 napari_stress-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:57:17.007221 napari_stress-0.3.5/src/napari_stress/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:57:17.007221 napari_stress-0.3.5/src/napari_stress/_approximation/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_approximation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_approximation/expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_approximation/expansion_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_approximation/fit_ellipsoid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:57:17.011221 napari_stress-0.3.5/src/napari_stress/_measurements/
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_measurements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18703 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_measurements/curvature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_measurements/deviation_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13684 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_measurements/geodesics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8368 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_measurements/intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_measurements/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_measurements/stresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_measurements/temporal_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27902 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_measurements/toolbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_measurements/toolbox.ui
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_napari_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:57:17.011221 napari_stress-0.3.5/src/napari_stress/_plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11794 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_plotting/create_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:57:17.011221 napari_stress-0.3.5/src/napari_stress/_reconstruction/
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_reconstruction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_reconstruction/fit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18144 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_reconstruction/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_reconstruction/reconstruct_surface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11023 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_reconstruction/refine_surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14844 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_reconstruction/toolbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15752 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_reconstruction/toolbox.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:57:17.015220 napari_stress-0.3.5/src/napari_stress/_sample_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   354896 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_sample_data/ExampleTifSequence.tif
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_sample_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66687 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_sample_data/dropplet_point_cloud.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1808756 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_sample_data/dropplet_point_cloud_4d.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_sample_data/sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:57:17.015220 napari_stress-0.3.5/src/napari_stress/_spherical_harmonics/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_spherical_harmonics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_spherical_harmonics/fit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13386 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_spherical_harmonics/spherical_harmonics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_spherical_harmonics/spherical_harmonics_napari.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:57:17.015220 napari_stress-0.3.5/src/napari_stress/_stress/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_stress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_stress/charts_SPB.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82885 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_stress/euclidian_k_form_SPB.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26226 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_stress/lebedev_info_SPB.py
+-rw-r--r--   0 runner    (1001) docker     (127)   145005 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_stress/lebedev_write_SPB.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72897 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_stress/manifold_SPB.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23955 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_stress/sph_func_SPB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_surface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:57:17.019221 napari_stress-0.3.5/src/napari_stress/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_tests/test_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23305 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_tests/test_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_tests/test_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_tests/test_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_tests/test_spherical_harmonic_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_tests/test_surface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_tests/test_vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:57:17.019221 napari_stress-0.3.5/src/napari_stress/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17285 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_utils/_aggregate_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_utils/coordinate_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23271 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_utils/frame_by_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_utils/import_export_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-16 12:57:04.000000 napari_stress-0.3.5/src/napari_stress/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:57:17.019221 napari_stress-0.3.5/src/napari_stress.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-16 12:57:16.000000 napari_stress-0.3.5/src/napari_stress.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-16 12:57:16.000000 napari_stress-0.3.5/src/napari_stress.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 12:57:16.000000 napari_stress-0.3.5/src/napari_stress.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-16 12:57:16.000000 napari_stress-0.3.5/src/napari_stress.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-16 12:57:16.000000 napari_stress-0.3.5/src/napari_stress.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 12:57:16.000000 napari_stress-0.3.5/src/napari_stress.egg-info/top_level.txt
```

### Comparing `napari_stress-0.3.3/LICENSE` & `napari_stress-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/PKG-INFO` & `napari_stress-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_stress
-Version: 0.3.3
+Version: 0.3.5
 Summary: Interactive surface analysis in napari for measuring mechanical stresses in biological tissues
 Author: Johannes Soltwedel, Ben J. Gross, Elijah Shelton, Carlos Gomez, Otger Campas
 Author-email: johannes_richard.mueller@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/campaslab/napari-stress/issues
 Project-URL: Documentation, https://campaslab.github.io/napari-stress
 Project-URL: Source Code, https://github.com/campaslab/napari-stress
@@ -36,22 +36,23 @@
 Requires-Dist: napari-tools-menu>=0.1.15
 Requires-Dist: numpy<1.24.0
 Requires-Dist: pandas
 Requires-Dist: pygeodesic
 Requires-Dist: pyocclient
 Requires-Dist: pyshtools<=4.10.0
 Requires-Dist: scikit-image
-Requires-Dist: scipy
+Requires-Dist: scipy>=1.9.0
 Requires-Dist: seaborn
 Requires-Dist: tqdm
 Requires-Dist: vedo>=2023.5.0
 Requires-Dist: vispy
 Requires-Dist: deprecation
+Requires-Dist: bokeh>=3.1.0
 
-[![License](https://img.shields.io/pypi/l/napari-stress.svg?color=green)](https://github.com/campaslab/napari-stress/raw/master/LICENSE)
+[![License](https://img.shields.io/pypi/l/napari-stress.svg?color=green)](https://github.com/campaslab/napari-stress/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-stress.svg?color=green)](https://pypi.org/project/napari-stress)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-stress.svg?color=green)](https://python.org)
 [![tests](https://github.com/campaslab/napari-stress/actions/workflows/test_and_deploy.yml/badge.svg)](https://github.com/campaslab/napari-stress/actions/workflows/test_and_deploy.yml)
 [![codecov](https://codecov.io/gh/campaslab/napari-stress/branch/main/graph/badge.svg?token=ZXQGREJAT9)](https://codecov.io/gh/campaslab/napari-stress)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/napari-stress.svg)](https://pypistats.org/packages/napari-stress)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-stress)](https://www.napari-hub.org/plugins/napari-stress)
```

### Comparing `napari_stress-0.3.3/README.md` & `napari_stress-0.3.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![License](https://img.shields.io/pypi/l/napari-stress.svg?color=green)](https://github.com/campaslab/napari-stress/raw/master/LICENSE)
+[![License](https://img.shields.io/pypi/l/napari-stress.svg?color=green)](https://github.com/campaslab/napari-stress/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-stress.svg?color=green)](https://pypi.org/project/napari-stress)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-stress.svg?color=green)](https://python.org)
 [![tests](https://github.com/campaslab/napari-stress/actions/workflows/test_and_deploy.yml/badge.svg)](https://github.com/campaslab/napari-stress/actions/workflows/test_and_deploy.yml)
 [![codecov](https://codecov.io/gh/campaslab/napari-stress/branch/main/graph/badge.svg?token=ZXQGREJAT9)](https://codecov.io/gh/campaslab/napari-stress)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/napari-stress.svg)](https://pypistats.org/packages/napari-stress)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-stress)](https://www.napari-hub.org/plugins/napari-stress)
```

### Comparing `napari_stress-0.3.3/setup.cfg` & `napari_stress-0.3.5/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -42,20 +42,21 @@
 	napari-tools-menu>=0.1.15
 	numpy<1.24.0
 	pandas
 	pygeodesic
 	pyocclient
 	pyshtools<=4.10.0
 	scikit-image
-	scipy
+	scipy>=1.9.0
 	seaborn
 	tqdm
 	vedo>=2023.5.0
 	vispy
 	deprecation
+	bokeh >= 3.1.0
 python_requires = >=3.7
 include_package_data = True
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
```

### Comparing `napari_stress-0.3.3/src/napari_stress/__init__.py` & `napari_stress-0.3.5/src/napari_stress/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.3.3"
+__version__ = "0.3.5"
 
 from . import _measurements as measurements
 from . import _approximation as approximation
 from . import _reconstruction as reconstruction
 from . import _sample_data as sample_data
 from . import _plotting as plotting
 from . import _utils as utils
```

### Comparing `napari_stress-0.3.3/src/napari_stress/_approximation/expansion.py` & `napari_stress-0.3.5/src/napari_stress/_approximation/expansion.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
     Parameters
     ----------
     points : napari.types.PointsData
         The points to expand.
     """
 
-    def __init__(self, get_measurements: bool = False):
-        super().__init__(get_measurements)
+    def __init__(self):
+        super().__init__()
 
     def _fit(self, points: "napari.types.PointsData") -> "napari.types.VectorsData":
         """
         Fit a 3D ellipsoid to given points using least squares fitting.
 
         The ellipsoid equation is: Ax^2 + By^2 + Cz^2 + Dxy + Exz + Fyz + Gx + Hy + Iz = 1
 
@@ -68,28 +68,28 @@
         )
 
         U, V = cartesian_to_elliptical(self.coefficients_, points, invert=True)
         expanded_points = elliptical_to_cartesian(U, V, self.coefficients_, invert=True)
 
         return expanded_points
 
-    def _measure_properties(self, input_points, output_points):
+    def _calculate_properties(self, input_points, output_points):
         """
         Measure properties of the expansion.
 
         Parameters
         ----------
         input_points : napari.types.PointsData
             The points before expansion.
         output_points : napari.types.PointsData
             The points after expansion.
         """
 
         distance = np.linalg.norm(input_points - output_points, axis=1)
-        self.properties["euclidian_distance"] = distance
+        self.properties["residuals"] = distance
 
     def _fit_ellipsoid_to_points(
         self,
         points: "napari.types.PointsData",
     ) -> np.ndarray:
         """
         Fit an ellipsoid to a set of points.
```

### Comparing `napari_stress-0.3.3/src/napari_stress/_approximation/expansion_base.py` & `napari_stress-0.3.5/src/napari_stress/_approximation/expansion_base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import numpy as np
-import pandas as pd
+from abc import ABC, abstractmethod
 
 
-class Expander:
-    def __init__(self, get_measurements: bool = False):
+class Expander(ABC):
+    def __init__(self):
         self.coefficients_ = None
-        self.properties = pd.DataFrame()
-        self._get_measurements = get_measurements
+        self.properties = {}
 
-    def fit(self, points: np.ndarray):
-        self._data = points
+    def fit(self, points: "napari.types.PointsData"):
         self.coefficients_ = self._fit(points)
         return self
 
     def expand(self, points: "napari.types.PointsData"):
         expanded_points = self._expand(points)
-        if self._get_measurements:
-            self._measure_properties(points, expanded_points)
+        self._calculate_properties(points, expanded_points)
         return expanded_points
 
     def fit_expand(self, points: "napari.types.PointsData"):
         self.fit(points)
         return self.expand(points)
 
+    @abstractmethod
     def _fit(self, points: "napari.types.PointsData"):
         raise NotImplementedError
 
+    @abstractmethod
     def _expand(self, points: "napari.types.PointsData"):
         raise NotImplementedError
 
-    def _measure_properties(self, input_points, output_points):
+    @abstractmethod
+    def _calculate_properties(self, input_points, output_points):
         raise NotImplementedError
```

### Comparing `napari_stress-0.3.3/src/napari_stress/_approximation/fit_ellipsoid.py` & `napari_stress-0.3.5/src/napari_stress/_approximation/fit_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_measurements/__init__.py` & `napari_stress-0.3.5/src/napari_stress/_measurements/__init__.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_measurements/curvature.py` & `napari_stress-0.3.5/src/napari_stress/_measurements/curvature.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_measurements/deviation_analysis.py` & `napari_stress-0.3.5/src/napari_stress/_measurements/deviation_analysis.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_measurements/geodesics.py` & `napari_stress-0.3.5/src/napari_stress/_measurements/geodesics.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_measurements/intensity.py` & `napari_stress-0.3.5/src/napari_stress/_measurements/intensity.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_measurements/measurements.py` & `napari_stress-0.3.5/src/napari_stress/_measurements/measurements.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_measurements/stresses.py` & `napari_stress-0.3.5/src/napari_stress/_measurements/stresses.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_measurements/temporal_correlation.py` & `napari_stress-0.3.5/src/napari_stress/_measurements/temporal_correlation.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_measurements/toolbox.py` & `napari_stress-0.3.5/src/napari_stress/_measurements/toolbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,17 +118,23 @@
         if event.type() == QEvent.ParentChange:
             self.layer_select.parent_changed.emit(self.parent())
 
         return super().eventFilter(obj, event)
 
     def _check_minimal_point_number(self) -> None:
         """Check if number of quadrature point complies with max_degree."""
-        minimal_point_number = lebedev_info_SPB.pts_of_lbdv_lookup[
-            self.spinBox_max_degree.value()
-        ]
+        # lebedev_info_SPB.pts_of_lbdv_lookup is a dictionary of the form
+        # {degree: number of quadrature points}
+        # if no value for the given key exists, pick the next higher value.
+        max_degree = self.spinBox_max_degree.value()
+        lookup = lebedev_info_SPB.pts_of_lbdv_lookup
+        for degree in range(max_degree, list(lookup.keys())[-1] + 1):
+            if degree in lookup.keys():
+                minimal_point_number = lookup.get(degree)
+                break
 
         if self.comboBox_quadpoints.currentData() < minimal_point_number:
             index = self.comboBox_quadpoints.findData(minimal_point_number)
             self.comboBox_quadpoints.setCurrentIndex(index)
 
         return None
```

### Comparing `napari_stress-0.3.3/src/napari_stress/_measurements/toolbox.ui` & `napari_stress-0.3.5/src/napari_stress/_measurements/toolbox.ui`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_plotting/create_plots.py` & `napari_stress-0.3.5/src/napari_stress/_plotting/create_plots.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_preprocess.py` & `napari_stress-0.3.5/src/napari_stress/_preprocess.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_reconstruction/__init__.py` & `napari_stress-0.3.5/src/napari_stress/_reconstruction/__init__.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_reconstruction/fit_utils.py` & `napari_stress-0.3.5/src/napari_stress/_reconstruction/fit_utils.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_reconstruction/patches.py` & `napari_stress-0.3.5/src/napari_stress/_reconstruction/patches.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_reconstruction/reconstruct_surface.py` & `napari_stress-0.3.5/src/napari_stress/_reconstruction/reconstruct_surface.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_reconstruction/refine_surfaces.py` & `napari_stress-0.3.5/src/napari_stress/_reconstruction/refine_surfaces.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_reconstruction/toolbox.py` & `napari_stress-0.3.5/src/napari_stress/_reconstruction/toolbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,16 @@
         self.image_layer_select = create_widget(annotation=Image, label="Image_layer")
         self.layout().addWidget(self.image_layer_select.native, 0, 1)
         self.installEventFilter(self)
 
         # populate comboboxes with allowed values
         self.comboBox_fittype.addItems(["fancy", "quick"])
         self.comboBox_fluorescence_type.addItems(["interior", "surface"])
-        self.comboBox_interpolation_method.addItems(["linear", "cubic"])
+        self.comboBox_interpolation_method.addItems(["cubic", "linear"])
+        self.comboBox_interpolation_method.setCurrentText("linear")
 
         # calculate density/point number
         self.spinBox_n_vertices.setValue(256)
         self.pushButton_run.clicked.connect(self._run)
         self.image_layer_select.changed.connect(self._set_scales)
         self.pushButton_export.clicked.connect(self._export_settings)
         self.pushButton_import.clicked.connect(self._import_settings)
@@ -55,14 +56,18 @@
         """Get scales from loaded data."""
         try:
             scales = self.image_layer_select.value.scale
             scales = scales[-3:]  # scales may be 4D
             self.doubleSpinBox_voxelsize_x.setValue(scales[2])
             self.doubleSpinBox_voxelsize_y.setValue(scales[1])
             self.doubleSpinBox_voxelsize_z.setValue(scales[0])
+
+            # set target voxel size to mean of scales as default
+            mean_scale = np.mean([scales[0], scales[2]])
+            self.doubleSpinBox_target_voxelsize.setValue(mean_scale)
         except Exception:
             pass
 
     def _export_settings(self, file_name: str = None):
         """
         Export reconstruction parameters to YAML file.
         """
@@ -258,14 +263,15 @@
             - points first guess: points sampled on fibonacci grid
             - traced points: points after tracing
             - trace vectors: vectors along which intensity was measured
             - droplet center: center of droplet
 
     """
     import copy
+    import vedo
     import napari_process_points_and_surfaces as nppas
     import napari_segment_blobs_and_things_with_membranes as nsbatwm
     from napari_stress import reconstruction
     from skimage import filters, transform
     from .refine_surfaces import resample_pointcloud
     from .patches import iterative_curvature_adaptive_patch_fitting
 
@@ -279,19 +285,20 @@
 
     # convert to surface
     label_image = nsbatwm.connected_component_labeling(binarized_image)
     surface = nppas.largest_label_to_surface(label_image)
     surface = nppas.remove_duplicate_vertices(surface)
 
     # Smooth and decimate
-    surface = nppas.smooth_surface(
-        surface, n_smoothing_iterations, feature_angle=120, edge_angle=90
+    mesh = (
+        vedo.Mesh(surface)
+        .smooth(niter=n_smoothing_iterations, feature_angle=120, edge_angle=90)
+        .decimate(n=n_points)
     )
-    surface = nppas.decimate_quadric(surface, number_of_vertices=n_points)
-    points_first_guess = surface[0]
+    points_first_guess = mesh.vertices
     points = copy.deepcopy(points_first_guess)
 
     # repeat tracing `n_tracing_iterations` times
     for i in range(n_tracing_iterations):
         resampled_points = resample_pointcloud(
             points, sampling_length=resampling_length
         )
@@ -321,25 +328,26 @@
     properties = {"name": "surface_first_guess"}
     layer_first_guess = (
         (surface[0] * target_voxelsize, surface[1]),
         properties,
         "surface",
     )
 
-    properties = {"name": "points_patch_fitted", "size": 0.5}
+    properties = {"name": "Droplet pointcloud (smoothed)", "size": 0.5}
     layer_patch_fitted = (
         points * target_voxelsize,
         properties,
         "points",
     )
 
     properties = {"name": "Label image", "scale": [target_voxelsize] * 3}
     layer_label_image = (label_image, properties, "labels")
 
     traced_points = list(traced_points)
+    traced_points[1]["name"] = "Droplet pointcloud (traced)"
     traced_points[0] *= target_voxelsize
 
     trace_vectors = list(trace_vectors)
     trace_vectors[0] *= target_voxelsize
 
     properties = {"name": "Center", "symbol": "ring", "face_color": "yellow", "size": 3}
     droplet_center = (traced_points[0].mean(axis=0)[None, :], properties, "points")
```

### Comparing `napari_stress-0.3.3/src/napari_stress/_reconstruction/toolbox.ui` & `napari_stress-0.3.5/src/napari_stress/_reconstruction/toolbox.ui`

 * *Files 0% similar despite different names*

#### Comparing `napari_stress-0.3.3/src/napari_stress/_reconstruction/toolbox.ui` & `napari_stress-0.3.5/src/napari_stress/_reconstruction/toolbox.ui`

```diff
@@ -66,23 +66,23 @@
             </item>
           </layout>
         </widget>
       </item>
       <item row="1" column="0" colspan="2">
         <widget class="QToolBox" name="toolBox">
           <property name="currentIndex">
-            <number>2</number>
+            <number>0</number>
           </property>
           <widget class="QWidget" name="page_3">
             <property name="geometry">
               <rect>
                 <x>0</x>
                 <y>0</y>
-                <width>125</width>
-                <height>118</height>
+                <width>855</width>
+                <height>253</height>
               </rect>
             </property>
             <attribute name="label">
               <string>1. Rescaling</string>
             </attribute>
             <layout class="QGridLayout" name="gridLayout_7">
               <item row="0" column="1">
@@ -169,16 +169,16 @@
             </layout>
           </widget>
           <widget class="QWidget" name="page">
             <property name="geometry">
               <rect>
                 <x>0</x>
                 <y>0</y>
-                <width>147</width>
-                <height>93</height>
+                <width>855</width>
+                <height>253</height>
               </rect>
             </property>
             <attribute name="label">
               <string>2. Initial reconstruction</string>
             </attribute>
             <layout class="QGridLayout" name="gridLayout_3">
               <item row="0" column="3">
@@ -233,15 +233,15 @@
                     </size>
                   </property>
                 </spacer>
               </item>
               <item row="2" column="3">
                 <widget class="QSpinBox" name="spinBox_n_smoothing">
                   <property name="value">
-                    <number>10</number>
+                    <number>15</number>
                   </property>
                 </widget>
               </item>
               <item row="1" column="1" colspan="2">
                 <widget class="QLabel" name="label">
                   <property name="text">
                     <string>Initial number of points</string>
@@ -250,17 +250,17 @@
               </item>
             </layout>
           </widget>
           <widget class="QWidget" name="page_2">
             <property name="geometry">
               <rect>
                 <x>0</x>
-                <y>0</y>
+                <y>-29</y>
                 <width>838</width>
-                <height>318</height>
+                <height>341</height>
               </rect>
             </property>
             <attribute name="label">
               <string>3. Surface tracing</string>
             </attribute>
             <layout class="QGridLayout" name="gridLayout_2">
               <item row="2" column="0" colspan="2">
@@ -340,15 +340,15 @@
                         <property name="minimum">
                           <double>0.500000000000000</double>
                         </property>
                         <property name="singleStep">
                           <double>1.000000000000000</double>
                         </property>
                         <property name="value">
-                          <double>2.500000000000000</double>
+                          <double>5.000000000000000</double>
                         </property>
                       </widget>
                     </item>
                   </layout>
                 </widget>
               </item>
               <item row="1" column="0" colspan="2">
@@ -396,15 +396,15 @@
                         <property name="maximum">
                           <double>10.000000000000000</double>
                         </property>
                         <property name="singleStep">
                           <double>0.250000000000000</double>
                         </property>
                         <property name="value">
-                          <double>0.500000000000000</double>
+                          <double>1.000000000000000</double>
                         </property>
                       </widget>
                     </item>
                     <item row="3" column="0">
                       <widget class="QLabel" name="label_8">
                         <property name="text">
                           <string>Sampling distance</string>
@@ -416,15 +416,15 @@
                         <property name="decimals">
                           <number>1</number>
                         </property>
                         <property name="minimum">
                           <double>2.000000000000000</double>
                         </property>
                         <property name="value">
-                          <double>10.000000000000000</double>
+                          <double>20.000000000000000</double>
                         </property>
                       </widget>
                     </item>
                     <item row="4" column="0">
                       <widget class="QLabel" name="label_10">
                         <property name="text">
                           <string>Image intensity interpolation</string>
@@ -457,22 +457,25 @@
             </layout>
           </widget>
         </widget>
       </item>
       <item row="6" column="0">
         <widget class="QCheckBox" name="checkBox_use_dask">
           <property name="text">
-            <string>Parallelize with dask</string>
+            <string>Parallelize with dask (only timelapse)</string>
           </property>
         </widget>
       </item>
       <item row="7" column="0">
         <widget class="QCheckBox" name="checkBox_return_intermediate">
           <property name="text">
-            <string>Return intermediate resultss (may require a lot of memory)</string>
+            <string>Return intermediate results (may require a lot of memory)</string>
+          </property>
+          <property name="checked">
+            <bool>true</bool>
           </property>
         </widget>
       </item>
     </layout>
   </widget>
   <tabstops>
     <tabstop>doubleSpinBox_voxelsize_x</tabstop>
```

### Comparing `napari_stress-0.3.3/src/napari_stress/_sample_data/ExampleTifSequence.tif` & `napari_stress-0.3.5/src/napari_stress/_sample_data/ExampleTifSequence.tif`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_sample_data/dropplet_point_cloud.csv` & `napari_stress-0.3.5/src/napari_stress/_sample_data/dropplet_point_cloud.csv`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_sample_data/dropplet_point_cloud_4d.csv` & `napari_stress-0.3.5/src/napari_stress/_sample_data/dropplet_point_cloud_4d.csv`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_sample_data/sample_data.py` & `napari_stress-0.3.5/src/napari_stress/_sample_data/sample_data.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_spherical_harmonics/fit_utils.py` & `napari_stress-0.3.5/src/napari_stress/_spherical_harmonics/fit_utils.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_spherical_harmonics/spherical_harmonics.py` & `napari_stress-0.3.5/src/napari_stress/_spherical_harmonics/spherical_harmonics.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_spherical_harmonics/spherical_harmonics_napari.py` & `napari_stress-0.3.5/src/napari_stress/_spherical_harmonics/spherical_harmonics_napari.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_stress/charts_SPB.py` & `napari_stress-0.3.5/src/napari_stress/_stress/charts_SPB.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_stress/euclidian_k_form_SPB.py` & `napari_stress-0.3.5/src/napari_stress/_stress/euclidian_k_form_SPB.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_stress/lebedev_info_SPB.py` & `napari_stress-0.3.5/src/napari_stress/_stress/lebedev_info_SPB.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_stress/lebedev_write_SPB.py` & `napari_stress-0.3.5/src/napari_stress/_stress/lebedev_write_SPB.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_stress/manifold_SPB.py` & `napari_stress-0.3.5/src/napari_stress/_stress/manifold_SPB.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_stress/sph_func_SPB.py` & `napari_stress-0.3.5/src/napari_stress/_stress/sph_func_SPB.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_surface.py` & `napari_stress-0.3.5/src/napari_stress/_surface.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_tests/test_approximation.py` & `napari_stress-0.3.5/src/napari_stress/_tests/test_approximation.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,19 +48,19 @@
         expander.fit(points)
 
         expanded_points = expander.expand(points)
         center = expander.center_
         axes_lengths = np.sort(expander.axes_)
 
         assert np.allclose(center, x0)
-        assert np.allclose(a2, axes_lengths[2] * 2)
-        assert np.allclose(a1, axes_lengths[1] * 2)
-        assert np.allclose(a0, axes_lengths[0] * 2)
+        assert np.allclose(a2, axes_lengths[2])
+        assert np.allclose(a1, axes_lengths[1])
+        assert np.allclose(a0, axes_lengths[0])
 
-        assert np.allclose(expander.properties.mean(), 0, atol=0.01)
+        assert np.allclose(expander.properties["residuals"].mean(), 0, atol=0.01)
         assert len(expanded_points) == len(points)
 
 
 def test_lsq_ellipsoid():
     from napari_stress import approximation, get_droplet_point_cloud
 
     pointcloud = get_droplet_point_cloud()[0][0][:, 1:]
```

### Comparing `napari_stress-0.3.3/src/napari_stress/_tests/test_measurements.py` & `napari_stress-0.3.5/src/napari_stress/_tests/test_measurements.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,29 +15,26 @@
     features = result[1]["metadata"]["features"]
 
     assert "mean_curvature" in features.keys()
     assert np.allclose(features["mean_curvature"].mean(), 1.0, atol=0.1)
 
 
 def test_intensity_measurement_on_normals():
-    from napari_stress import vectors, measurements, sample_data, frame_by_frame
+    from napari_stress import vectors, measurements, sample_data
     import napari_segment_blobs_and_things_with_membranes as nsbatwm
     import napari_process_points_and_surfaces as nppas
+    import vedo
 
-    droplet = sample_data.get_droplet_4d()[0][0]
-    droplet_rescaled = frame_by_frame(nsbatwm.rescale)(
-        droplet, scale_x=1, scale_y=1, scale_z=2
-    )
-    droplet_binary = frame_by_frame(nsbatwm.threshold_otsu)(droplet_rescaled)
-
-    surface = frame_by_frame(nppas.label_to_surface)(droplet_binary, 1)
-    surface_smooth = frame_by_frame(nppas.smooth_surface)(surface)
-    surface_decimated = frame_by_frame(nppas.decimate_quadric)(
-        surface_smooth, number_of_vertices=1000
-    )
+    droplet = sample_data.get_droplet_4d()[0][0][0]
+    droplet_rescaled = nsbatwm.rescale(droplet, scale_x=1, scale_y=1, scale_z=2)
+    droplet_binary = nsbatwm.threshold_otsu(droplet_rescaled)
+
+    surface = nppas.label_to_surface(droplet_binary)
+    mesh = vedo.Mesh(surface).smooth().decimate(n=1000)
+    surface_decimated = (mesh.vertices, np.asarray(mesh.cells))
 
     # measure intensity on normal vectors
     normals = vectors.normal_vectors_on_surface(
         surface_decimated, length_multiplier=5, center=True
     )
     vectors_LDtuple = measurements.intensity._sample_intensity_along_vector(
         normals, droplet_rescaled
@@ -46,15 +43,15 @@
     assert "intensity_mean" in vectors_LDtuple[1]["features"].keys()
 
     # measure intensity directly on surface
     intensities = measurements.intensity._measure_intensity_on_surface(
         surface_decimated, droplet_rescaled
     )
     assert len(intensities[0][2]) == len(surface_decimated[0])
-    assert "intensity_mean" in intensities[1]["metadata"]["features"][0].keys()
+    assert "intensity_mean" in intensities[1]["metadata"]["features"].keys()
 
 
 def test_mean_curvature_on_ellipsoid():
     """Test that the mean curvature is computed correctly."""
     from napari_stress import reconstruction, sample_data, measurements
 
     size = 128
@@ -379,15 +376,16 @@
 def test_comprehensive_stress_toolbox_4d(make_napari_viewer):
     from napari_stress import get_droplet_point_cloud_4d
     import napari_stress
     import os
 
     viewer = make_napari_viewer()
     pointcloud = get_droplet_point_cloud_4d()[0]
-    viewer.add_points(pointcloud[0], **pointcloud[1])
+    pointcloud_2tp = pointcloud[0][pointcloud[0][:, 0] <= 1, :]
+    viewer.add_points(pointcloud_2tp)
 
     widget = napari_stress._measurements.toolbox.stress_analysis_toolbox(viewer)
     viewer.window.add_dock_widget(widget)
 
     widget._run()
     widget.checkBox_export.setChecked(False)
     widget.checkBox_export.setChecked(True)
```

### Comparing `napari_stress-0.3.3/src/napari_stress/_tests/test_processing.py` & `napari_stress-0.3.5/src/napari_stress/_tests/test_processing.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_tests/test_reconstruction.py` & `napari_stress-0.3.5/src/napari_stress/_tests/test_reconstruction.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_tests/test_sample_data.py` & `napari_stress-0.3.5/src/napari_stress/_tests/test_sample_data.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_tests/test_spherical_harmonic_fit.py` & `napari_stress-0.3.5/src/napari_stress/_tests/test_spherical_harmonic_fit.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_tests/test_surface.py` & `napari_stress-0.3.5/src/napari_stress/_tests/test_surface.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_tests/test_types.py` & `napari_stress-0.3.5/src/napari_stress/_tests/test_types.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_tests/test_utils.py` & `napari_stress-0.3.5/src/napari_stress/_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_tests/test_vectors.py` & `napari_stress-0.3.5/src/napari_stress/_tests/test_vectors.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_utils/_aggregate_measurements.py` & `napari_stress-0.3.5/src/napari_stress/_utils/_aggregate_measurements.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_utils/coordinate_conversion.py` & `napari_stress-0.3.5/src/napari_stress/_utils/coordinate_conversion.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_utils/frame_by_frame.py` & `napari_stress-0.3.5/src/napari_stress/_utils/frame_by_frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,17 +345,19 @@
 
         # If data was only 3D
         _properties = {}
         if len(data) == 1:
             if "features" in properties[0].keys():
                 _properties["features"] = data[0][1]["features"]
                 _properties["features"]["frame"] = np.zeros(len(data[0][0]), dtype=int)
+                [frame.pop("features") for frame in properties]
             if "metadata" in properties[0].keys():
                 _properties["metadata"] = data[0][1]["metadata"]
                 _properties["metadata"]["frame"] = [0]
+                [frame.pop("metadata") for frame in properties]
         else:
             # Stack features
             if "features" in properties[0].keys():
                 # concatenate features and add time column
                 features = self._list_of_dataframes_to_dataframe(
                     [pd.DataFrame(frame["features"]) for frame in properties]
                 )
```

### Comparing `napari_stress-0.3.3/src/napari_stress/_utils/import_export_settings.py` & `napari_stress-0.3.5/src/napari_stress/_utils/import_export_settings.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/_vectors.py` & `napari_stress-0.3.5/src/napari_stress/_vectors.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/napari.yaml` & `napari_stress-0.3.5/src/napari_stress/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress/types.py` & `napari_stress-0.3.5/src/napari_stress/types.py`

 * *Files identical despite different names*

### Comparing `napari_stress-0.3.3/src/napari_stress.egg-info/PKG-INFO` & `napari_stress-0.3.5/src/napari_stress.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_stress
-Version: 0.3.3
+Version: 0.3.5
 Summary: Interactive surface analysis in napari for measuring mechanical stresses in biological tissues
 Author: Johannes Soltwedel, Ben J. Gross, Elijah Shelton, Carlos Gomez, Otger Campas
 Author-email: johannes_richard.mueller@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/campaslab/napari-stress/issues
 Project-URL: Documentation, https://campaslab.github.io/napari-stress
 Project-URL: Source Code, https://github.com/campaslab/napari-stress
@@ -36,22 +36,23 @@
 Requires-Dist: napari-tools-menu>=0.1.15
 Requires-Dist: numpy<1.24.0
 Requires-Dist: pandas
 Requires-Dist: pygeodesic
 Requires-Dist: pyocclient
 Requires-Dist: pyshtools<=4.10.0
 Requires-Dist: scikit-image
-Requires-Dist: scipy
+Requires-Dist: scipy>=1.9.0
 Requires-Dist: seaborn
 Requires-Dist: tqdm
 Requires-Dist: vedo>=2023.5.0
 Requires-Dist: vispy
 Requires-Dist: deprecation
+Requires-Dist: bokeh>=3.1.0
 
-[![License](https://img.shields.io/pypi/l/napari-stress.svg?color=green)](https://github.com/campaslab/napari-stress/raw/master/LICENSE)
+[![License](https://img.shields.io/pypi/l/napari-stress.svg?color=green)](https://github.com/campaslab/napari-stress/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-stress.svg?color=green)](https://pypi.org/project/napari-stress)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-stress.svg?color=green)](https://python.org)
 [![tests](https://github.com/campaslab/napari-stress/actions/workflows/test_and_deploy.yml/badge.svg)](https://github.com/campaslab/napari-stress/actions/workflows/test_and_deploy.yml)
 [![codecov](https://codecov.io/gh/campaslab/napari-stress/branch/main/graph/badge.svg?token=ZXQGREJAT9)](https://codecov.io/gh/campaslab/napari-stress)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/napari-stress.svg)](https://pypistats.org/packages/napari-stress)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-stress)](https://www.napari-hub.org/plugins/napari-stress)
```

### Comparing `napari_stress-0.3.3/src/napari_stress.egg-info/SOURCES.txt` & `napari_stress-0.3.5/src/napari_stress.egg-info/SOURCES.txt`

 * *Files identical despite different names*

