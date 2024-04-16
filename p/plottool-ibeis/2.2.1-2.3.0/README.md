# Comparing `tmp/plottool_ibeis-2.2.1.tar.gz` & `tmp/plottool_ibeis-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plottool_ibeis-2.2.1.tar", last modified: Sat Jan 28 23:34:08 2023, max compression
+gzip compressed data, was "plottool_ibeis-2.3.0.tar", last modified: Tue Apr 16 01:31:34 2024, max compression
```

## Comparing `plottool_ibeis-2.2.1.tar` & `plottool_ibeis-2.3.0.tar`

### file list

```diff
@@ -1,51 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 23:34:08.296633 plottool_ibeis-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-01-28 23:34:08.296633 plottool_ibeis-2.2.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2178 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 23:34:08.292633 plottool_ibeis-2.2.1/plottool_ibeis/
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/__MPL_INIT__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16238 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/_cv2_impaint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/_oldimpaint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18523 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/abstract_interaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23668 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/color_funcs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4522 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/custom_constants.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18612 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/custom_figure.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   158769 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/draw_func2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8568 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/draw_sv.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8747 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/fig_presenter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    52125 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/interact_annotations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2907 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/interact_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/interact_impaint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8544 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/interact_keypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    13488 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/interact_matches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13391 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/interact_multi_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/interactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14111 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/mpl_keypoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10666 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/mpl_sift.py
--rw-r--r--   0 runner    (1001) docker     (123)    65721 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/nx_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1951 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/other.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4341 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/plot_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    91033 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/plots.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11856 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/screeninfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/test_colorsys.py
--rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/test_vtk_poly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 23:34:08.296633 plottool_ibeis-2.2.1/plottool_ibeis/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      586 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/tests/test_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/tests/test_interact_multi_image.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1735 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/tests/test_viz_image2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1757 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/tests/test_viz_images.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8010 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/viz_featrow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1861 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/viz_image2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4201 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/plottool_ibeis/viz_keypoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 23:34:08.292633 plottool_ibeis-2.2.1/plottool_ibeis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-01-28 23:34:08.000000 plottool_ibeis-2.2.1/plottool_ibeis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-01-28 23:34:08.000000 plottool_ibeis-2.2.1/plottool_ibeis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-28 23:34:08.000000 plottool_ibeis-2.2.1/plottool_ibeis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-01-28 23:34:08.000000 plottool_ibeis-2.2.1/plottool_ibeis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-28 23:34:08.000000 plottool_ibeis-2.2.1/plottool_ibeis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-28 23:34:08.296633 plottool_ibeis-2.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     9307 2023-01-28 23:34:02.000000 plottool_ibeis-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:31:34.592270 plottool_ibeis-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    32867 2024-04-16 01:31:34.592270 plottool_ibeis-2.3.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2178 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:31:34.540270 plottool_ibeis-2.3.0/plottool_ibeis/
+-rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/__MPL_INIT__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/__MPL_INIT__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16238 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/__main__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/_cv2_impaint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/_cv2_impaint.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/_oldimpaint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/_oldimpaint.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18459 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/abstract_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/abstract_interaction.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    23284 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/color_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/color_funcs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/custom_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/custom_constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18631 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/custom_figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/custom_figure.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   159913 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/draw_func2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21084 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/draw_func2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/draw_sv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/draw_sv.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8682 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/fig_presenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/fig_presenter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    52569 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/interact_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/interact_annotations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/interact_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/interact_helpers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/interact_impaint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/interact_impaint.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/interact_keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/interact_keypoints.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13169 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/interact_matches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/interact_matches.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/interact_multi_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/interact_multi_image.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11319 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/interactions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13936 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/mpl_keypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/mpl_keypoint.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/mpl_sift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/mpl_sift.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    65669 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/nx_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/nx_helpers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/other.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/other.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/plot_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/plot_helpers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    90840 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/plots.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11808 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/screeninfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/screeninfo.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/test_colorsys.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/test_colorsys.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12691 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/test_vtk_poly.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/test_vtk_poly.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:31:34.544270 plottool_ibeis-2.3.0/plottool_ibeis/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      521 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/tests/test_helpers.pyi
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1428 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/tests/test_interact_multi_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/tests/test_interact_multi_image.pyi
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1670 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/tests/test_viz_image2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/tests/test_viz_image2.pyi
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1692 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/tests/test_viz_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/tests/test_viz_images.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/viz_featrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/viz_featrow.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/viz_image2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/viz_image2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/viz_keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/plottool_ibeis/viz_keypoints.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:31:34.544270 plottool_ibeis-2.3.0/plottool_ibeis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    32867 2024-04-16 01:31:34.000000 plottool_ibeis-2.3.0/plottool_ibeis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-16 01:31:34.000000 plottool_ibeis-2.3.0/plottool_ibeis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 01:31:34.000000 plottool_ibeis-2.3.0/plottool_ibeis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14472 2024-04-16 01:31:34.000000 plottool_ibeis-2.3.0/plottool_ibeis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 01:31:34.000000 plottool_ibeis-2.3.0/plottool_ibeis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 01:31:34.592270 plottool_ibeis-2.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9900 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:31:34.544270 plottool_ibeis-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-16 01:30:32.000000 plottool_ibeis-2.3.0/tests/test_import.py
```

### Comparing `plottool_ibeis-2.2.1/LICENSE` & `plottool_ibeis-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plottool_ibeis-2.2.1/README.rst` & `plottool_ibeis-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/__MPL_INIT__.py` & `plottool_ibeis-2.3.0/plottool_ibeis/__MPL_INIT__.py`

 * *Files identical despite different names*

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/__init__.py` & `plottool_ibeis-2.3.0/plottool_ibeis/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # flake8: noqa
 """
 Wrappers around matplotlib
 """
-__version__ = '2.2.1'
+__version__ = '2.3.0'
 
 import utool as ut
 ut.noinject(__name__, '[plottool_ibeis.__init__]')
 
 
 # Hopefully this was imported sooner. TODO remove dependency
 #from guitool_ibeis import __PYQT__
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/_cv2_impaint.py` & `plottool_ibeis-2.3.0/plottool_ibeis/_cv2_impaint.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
             else:
                 cv2.circle(img, (x, y), 5, (0, 0, 255), -1)
 
     img = np.zeros((512, 512, 3), np.uint8)
     cv2.namedWindow('image')
     cv2.setMouseCallback('image', draw_circle)
 
-    while(1):
+    while True:
         cv2.imshow('image', img)
         keycode = cv2.waitKey(1) & 0xFF
         if keycode == ord('m'):
             globals_['mode'] = not globals_['mode']
         elif keycode == 27:
             break
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/_oldimpaint.py` & `plottool_ibeis-2.3.0/plottool_ibeis/_oldimpaint.py`

 * *Files identical despite different names*

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/abstract_interaction.py` & `plottool_ibeis-2.3.0/plottool_ibeis/abstract_interaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-# -*- coding: utf-8 -*-
 """
 Known Interactions that use AbstractInteraction:
     pt.MatchInteraction2
     pt.MultiImageInteraction
     ibeis.NameInteraction
 """
-from __future__ import absolute_import, division, print_function
+import ubelt as ub
 import six
 import re
 import utool as ut
 import matplotlib as mpl
 ut.noinject(__name__, '[abstract_iteract]')
 import plottool_ibeis.draw_func2 as df2  # NOQA
 from plottool_ibeis import fig_presenter  # NOQA
@@ -194,15 +193,15 @@
         #fig_presenter.update()
         self.fig.canvas.update()
         self.fig.canvas.flush_events()
 
     def on_scroll(self, event):
         if self.debug:
             print('[pt.a] on_scroll')
-            print(ut.repr3(event.__dict__))
+            print(ub.urepr(event.__dict__, nl=1))
         pass
 
     def close(self):
         assert isinstance(self.fig, mpl.figure.Figure)
         fig_presenter.close_figure(self.fig)
 
     def on_close(self, event=None):
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/color_funcs.py` & `plottool_ibeis-2.3.0/plottool_ibeis/color_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-from __future__ import absolute_import, division, print_function
-from six.moves import range, zip, map  # NOQA
-from plottool_ibeis import custom_constants  # NOQA
 import six
+import ubelt as ub
 from matplotlib import colors as mcolors
 import colorsys
 import numpy as np  # NOQA
 import utool as ut
 #from plottool_ibeis import colormaps as cmaps2
 #(print, print_, printDBG, rrr, profile) = utool.inject(__name__, '[colorfuncs]', DEBUG=False)
 ut.noinject(__name__)
@@ -18,15 +16,14 @@
         'is_01': all([c >= 0.0 and c <= 1.0 for c in channels]),
     }
     return tests01
 
 
 def _test_base255(channels):
     tests255 = {
-        #'is_int': all([ut.is_int(c) for c in channels]),
         'is_255': all([c >= 0.0 and c <= 255.0 for c in channels]),
     }
     return tests255
 
 
 def is_base01(channels):
     """ check if a color is in base 01 """
@@ -220,17 +217,18 @@
         >>> import plottool_ibeis as pt
         >>> pt.show_if_requested()
     """
     import plottool_ibeis as pt
     import vtool_ibeis as vt
     block = np.zeros((5, 5, 3))
     block_list = [block + color[0:3] for color in rgb_list]
-    #print(ut.repr2(block_list))
-    #print(ut.repr2(rgb_list))
-    chunks = ut.ichunks(block_list, 10)
+    #print(ub.urepr(block_list))
+    #print(ub.urepr(rgb_list))
+
+    chunks = ub.chunks(block_list, chunksize=10)
     stacked_chunk = []
     for chunk in chunks:
         stacked_chunk.append(vt.stack_image_list(chunk, vert=False))
     stacked_block = vt.stack_image_list(stacked_chunk, vert=True)
     # convert to bgr
     stacked_block = stacked_block[:, :, ::-1]
     uint8_img = (255 * stacked_block).astype(np.uint8)
@@ -252,15 +250,15 @@
         >>> rgb = (255.0 / 255.0, 100 / 255.0, 0 / 255.0)
         >>> amount = .5
         >>> new_rgb = desaturate_rgb(rgb, amount)
         >>> # xdoctest: +REQUIRES(--show)
         >>> color_list = [rgb, new_rgb, desaturate_rgb(rgb, .7)]
         >>> testshow_colors(color_list)
         >>> # verify results
-        >>> result = ut.repr2(new_rgb)
+        >>> result = ub.urepr(new_rgb, nl=0)
         >>> print(result)
         (1.0, 0.696078431372549, 0.5)
 
         (1.0, 0.41599384851980004, 0.039215686274509776)
     """
     hue_adjust = 0.0
     sat_adjust = -amount
@@ -292,15 +290,15 @@
         >>> # execute function
         >>> new_rgb = lighten_rgb(rgb, amount)
         >>> import plottool_ibeis as pt
         >>> if pt.show_was_requested():
         >>>     color_list = [rgb, new_rgb, lighten_rgb(rgb, .5)]
         >>>     testshow_colors(color_list)
         >>> # verify results
-        >>> result = ut.repr2(new_rgb, with_dtype=False)
+        >>> result = ub.urepr(new_rgb, with_dtype=False)
         >>> print(result)
     """
     hue_adjust = 0.0
     sat_adjust = -amount
     val_adjust = amount
     new_rgb = adjust_hsv_of_rgb(rgb, hue_adjust, sat_adjust, val_adjust)
     return new_rgb
@@ -634,26 +632,26 @@
     type_ =  ut.get_argval('--type', str, default=None)
     if type_ is None:
         maps = [m for m in pylab.cm.datad if not m.endswith("_r")]
         #maps += cmaps2.__all__
         maps.sort()
     else:
         maps = CMAP_DICT[type_]
-        print('CMAP_DICT = %s' % (ut.repr3(CMAP_DICT),))
+        print('CMAP_DICT = %s' % (ub.urepr(CMAP_DICT),))
 
     cmap_ = ut.get_argval('--cmap', default=None)
     if cmap_ is not None:
         maps = [getattr(plt.cm, cmap_)]
 
-    l = len(maps) + 1
+    ell = len(maps) + 1
     for i, m in enumerate(maps):
         if TRANSPOSE:
-            pylab.subplot(l, 1, i + 1)
+            pylab.subplot(ell, 1, i + 1)
         else:
-            pylab.subplot(1, l, i + 1)
+            pylab.subplot(1, ell, i + 1)
 
         #pylab.axis("off")
         ax = plt.gca()
         ax.set_xticks([])
         ax.set_yticks([])
         #try:
         cmap = pylab.get_cmap(m)
@@ -668,15 +666,11 @@
             pylab.title(m, rotation=90, fontsize=10)
     #pylab.savefig("colormaps.png", dpi=100, facecolor='gray')
 
 
 if __name__ == '__main__':
     """
     CommandLine:
-        python -m plottool_ibeis.color_funcs
-        python -m plottool_ibeis.color_funcs --allexamples
-        python -m plottool_ibeis.color_funcs --allexamples --noface --nosrc
-    """
-    import multiprocessing
-    multiprocessing.freeze_support()  # for win32
-    import utool as ut  # NOQA
-    ut.doctest_funcs()
+        python -m plottool_ibeis.color_funcs all
+    """
+    import xdoctest
+    xdoctest.doctest_module(__file__)
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/custom_constants.py` & `plottool_ibeis-2.3.0/plottool_ibeis/custom_constants.py`

 * *Files identical despite different names*

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/custom_figure.py` & `plottool_ibeis-2.3.0/plottool_ibeis/custom_figure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from os.path import exists, splitext, join, split
 import utool as ut
+import ubelt as ub
 import matplotlib as mpl
 import warnings
 import functools
 from plottool_ibeis import custom_constants
 import matplotlib.gridspec as gridspec  # NOQA
 ut.noinject(__name__, '[customfig]')
 
@@ -368,27 +369,27 @@
         extent = saveax.get_window_extent().transformed(fig.dpi_scale_trans.inverted())
         if verbose == 2:
             print('[pt.save_figure] bbox ar = %.2f' % np.abs((extent.width / extent.height,)))
         #extent = saveax.get_window_extent().transformed(fig.transFigure.inverted())
         #print('[df2] bbox ar = %.2f' % np.abs((extent.width / extent.height,)))
         savekw['bbox_inches'] = extent.expanded(1.0, 1.0)
         if verbose == 2:
-            print('[pt.save_figure] savekw = ' + ut.repr2(savekw))
+            print('[pt.save_figure] savekw = ' + ub.urepr(savekw))
 
     with warnings.catch_warnings():
         warnings.filterwarnings('ignore', category=DeprecationWarning)
         if overwrite or not exists(fpath_clean):
             if verbose == 2:
                 print('[pt.save_figure] save_figure() full=%r' % (fpath_clean,))
             elif verbose == 1:
                 fpathndir = ut.path_ndir_split(fpath_clean, 5)
                 print('[pt.save_figure] save_figure() ndir=%r' % (fpathndir))
             if verbose > 1 or ut.VERBOSE:
                 print(']pt.save_figure] fpath_clean = %s' % (fpath_clean, ))
-                print('[pt.save_figure] savekw = ' + ut.repr2(savekw))
+                print('[pt.save_figure] savekw = ' + ub.urepr(savekw))
             if fpath_clean.endswith('.png'):
                 savekw['transparent'] = True
                 savekw['edgecolor'] = 'none'
                 #savekw['axes.edgecolor'] = 'none'
             fig.savefig(fpath_clean, **savekw)
         else:
             if verbose > 0:
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/draw_func2.py` & `plottool_ibeis-2.3.0/plottool_ibeis/draw_func2.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,23 +284,24 @@
         coords (tuple): (default = (0, 0))
         coord_type (str): (default = 'axes')
         bbox_alignment (tuple): (default = (0, 0))
         max_dsize (None): (default = None)
 
     CommandLine:
         python -m plottool_ibeis.draw_func2 --exec-overlay_icon --show --icon zebra.png
-        python -m plottool_ibeis.draw_func2 --exec-overlay_icon --show --icon astro.png
-        python -m plottool_ibeis.draw_func2 --exec-overlay_icon --show --icon astro.png --artist
+        python -m plottool_ibeis.draw_func2 --exec-overlay_icon --show --icon astro
+        python -m plottool_ibeis.draw_func2 --exec-overlay_icon --show --icon astro --artist
 
     Example:
         >>> # DISABLE_DOCTEST
         >>> from plottool_ibeis.draw_func2 import *  # NOQA
         >>> import plottool_ibeis as pt
         >>> pt.plot2(np.arange(100), np.arange(100))
-        >>> icon = ut.get_argval('--icon', type_=str, default='astro.png')
+        >>> icon = ut.get_argval('--icon', type_=str, default='astro')
+        >>> icon = ut.grab_test_imgpath(icon)
         >>> coords = (0, 0)
         >>> coord_type = 'axes'
         >>> bbox_alignment = (0, 0)
         >>> max_dsize = None  # (128, None)
         >>> max_asize = (60, 40)
         >>> as_artist = not ub.argflag('--noartist')
         >>> result = overlay_icon(icon, coords, coord_type, bbox_alignment,
@@ -587,15 +588,15 @@
         groupid_list = []
         for axs in atomic_axes:
             for ax in axs:
                 groupid = ax.colNum
             groupid_list.append(groupid)
 
         groupxs = ut.group_indices(groupid_list)[1]
-        new_groups = ut.lmap(ut.flatten, ut.apply_grouping(atomic_axes, groupxs))
+        new_groups = [list(ub.flatten(g)) for g in ut.apply_grouping(atomic_axes, groupxs)]
         atomic_axes = new_groups
         #[[(ax.rowNum, ax.colNum) for ax in axs] for axs in atomic_axes]
         # save all rows of each column
 
     dpi_scale_trans_inv = fig.dpi_scale_trans.inverted()
     axes_bboxes_ = [axes_extent(axs, pad) for axs in atomic_axes]
     axes_extents_ = [extent.transformed(dpi_scale_trans_inv) for extent in axes_bboxes_]
@@ -829,15 +830,15 @@
                 groupid_list = []
                 for axs in atomic_axes:
                     for ax in axs:
                         groupid = ax.colNum
                     groupid_list.append(groupid)
 
                 groups = ub.group_items(atomic_axes, groupid_list)
-                new_groups = ut.emap(ut.flatten, groups.values())
+                new_groups = [list(ub.flatten(g)) for g in groups.values()]
                 atomic_axes = new_groups
                 #[[(ax.rowNum, ax.colNum) for ax in axs] for axs in atomic_axes]
                 # save all rows of each column
 
             subpath_list = save_parts(fig=fig, fpath=fpath_strict,
                                       grouped_axes=atomic_axes, dpi=dpi)
             absfpath_ = subpath_list[-1]
@@ -2192,21 +2193,40 @@
     if ax is None:
         ax = gca()
     ax.set_yticks(np.arange(nTicks) * spacing)
     small_yticks(ax)
 
 
 def small_xticks(ax=None):
+    """
+    Example:
+        >>> # ENABLE_DOCTEST
+        >>> from plottool_ibeis.draw_func2 import *  # NOQA
+        >>> import plottool_ibeis as pt
+        >>> fig = pt.figure()
+        >>> ax = fig.gca()
+        >>> small_xticks(ax)
+    """
     for tick in ax.xaxis.get_major_ticks():
-        tick.label.set_fontsize(8)
+        # Replaced for matplotlib 3.8
+        # https://matplotlib.org/stable/api/prev_api_changes/api_changes_3.8.0.html#unused-methods-in-axis-tick-xaxis-and-yaxis
+        try:
+            tick.label.set_fontsize(8)
+        except AttributeError:
+            tick.label1.set_fontsize(8)
 
 
 def small_yticks(ax=None):
     for tick in ax.yaxis.get_major_ticks():
-        tick.label.set_fontsize(8)
+        # Replaced for matplotlib 3.8
+        # https://matplotlib.org/stable/api/prev_api_changes/api_changes_3.8.0.html#unused-methods-in-axis-tick-xaxis-and-yaxis
+        try:
+            tick.label.set_fontsize(8)
+        except AttributeError:
+            tick.label1.set_fontsize(8)
 
 
 def plot_bars(y_data, nColorSplits=1):
     width = 1
     nDims = len(y_data)
     nGroup = nDims // nColorSplits
     ori_colors = distinct_colors(nColorSplits)
@@ -2563,21 +2583,27 @@
 
 
 def ensure_divider(ax):
     """ Returns previously constructed divider or creates one """
     from plottool_ibeis import plot_helpers as ph
     divider = ph.get_plotdat(ax, DF2_DIVIDER_KEY, None)
     if divider is None:
-        divider = make_axes_locatable(ax)
+        divider = make_axes_locatable(ax)  # type: mpl_toolkits.axes_grid1.axes_divider.AxesDivider
         ph.set_plotdat(ax, DF2_DIVIDER_KEY, divider)
         orig_append_axes = divider.append_axes
         def df2_append_axes(divider, position, size, pad=None, add_to_figure=True, **kwargs):
             """ override divider add axes to register the divided axes """
             div_axes = ph.get_plotdat(ax, 'df2_div_axes', [])
-            new_ax = orig_append_axes(position, size, pad=pad, add_to_figure=add_to_figure, **kwargs)
+            # https://matplotlib.org/stable/api/prev_api_changes/api_changes_3.7.0.html
+            try:
+                new_ax = orig_append_axes(position, size, pad=pad, add_to_figure=add_to_figure, **kwargs)
+            except Exception:
+                new_ax = orig_append_axes(position, size, pad=pad, **kwargs)
+            if add_to_figure:
+                divider._fig.add_axes(ax)
             div_axes.append(new_ax)
             ph.set_plotdat(ax, 'df2_div_axes', div_axes)
             return new_ax
         ut.inject_func_as_method(divider, df2_append_axes, 'append_axes', allow_override=True)
     return divider
 
 
@@ -3279,15 +3305,15 @@
     CommandLine:
         python -m plottool_ibeis.draw_func2 --test-draw_keypoint_patch --show
 
     Example:
         >>> # DISABLE_DOCTEST
         >>> from plottool_ibeis.draw_func2 import *  # NOQA
         >>> import vtool_ibeis as vt
-        >>> rchip = vt.imread(ut.grab_test_imgpath('astro.png'))
+        >>> rchip = vt.imread(ut.grab_test_imgpath('astro'))
         >>> kp = [100, 100, 20, 0, 20, 0]
         >>> sift = None
         >>> warped = True
         >>> patch_dict = {}
         >>> ax = draw_keypoint_patch(rchip, kp, sift, warped, patch_dict)
         >>> result = ('ax = %s' % (str(ax),))
         >>> print(result)
@@ -3362,15 +3388,15 @@
     CommandLine:
         python -m plottool_ibeis.draw_func2 --exec-imshow --show
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> from plottool_ibeis.draw_func2 import *  # NOQA
         >>> import vtool_ibeis as vt
-        >>> img_fpath = ut.grab_test_imgpath('carl.jpg')
+        >>> img_fpath = ut.grab_test_imgpath('carl')
         >>> img = vt.imread(img_fpath)
         >>> (fig, ax) = imshow(img)
         >>> result = ('(fig, ax) = %s' % (str((fig, ax)),))
         >>> print(result)
         >>> import plottool_ibeis as pt
         >>> pt.show_if_requested()
     """
@@ -3617,16 +3643,16 @@
         python -m plottool_ibeis.draw_func2 show_chipmatch2 --show
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> from plottool_ibeis.draw_func2 import *  # NOQA
         >>> import plottool_ibeis as pt
         >>> import vtool_ibeis as vt
-        >>> rchip1 = vt.imread(ut.grab_test_imgpath('easy1.png'))
-        >>> rchip2 = vt.imread(ut.grab_test_imgpath('easy2.png'))
+        >>> rchip1 = vt.imread(ut.grab_test_imgpath('tsukuba_r'))
+        >>> rchip2 = vt.imread(ut.grab_test_imgpath('tsukuba_l'))
         >>> kpts1 = np.array([
         >>>     [10,  10,   30,   0,    30,    0.  ],
         >>>     [ 355.89,  142.95,   10.46,   -0.63,    8.59,    0.  ],
         >>>     [ 356.35,  147.  ,    8.38,    1.08,   11.68,    0.  ],
         >>>     [ 361.4 ,  150.64,    7.44,    3.45,   13.63,    0.  ]
         >>> ], dtype=np.float64)
         >>> kpts2 = np.array([
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/draw_sv.py` & `plottool_ibeis-2.3.0/plottool_ibeis/draw_sv.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     import vtool_ibeis as vt
     wh2 = vt.get_size(chip2)
     chip1_Mt = vt.warpHomog(chip1, M, wh2)
     chip2_blendM = vt.blend_images(chip1_Mt, chip2)
     return chip2_blendM
 
 
-#@ut.indent_func
 def show_sv(chip1, chip2, kpts1, kpts2, fm, homog_tup=None, aff_tup=None,
             mx=None, show_assign=True, show_lines=True, show_kpts=True,
             show_aff=None, fnum=1, refine_method=None, **kwargs):
     """ Visualizes spatial verification
 
     CommandLine:
         python -m vtool_ibeis.spatial_verification --test-spatially_verify_kpts --show
@@ -194,14 +193,11 @@
     pt.plot_fmatch(xywh1, xywh2, kpts1, kpts2, fm_outliers, colors=color2,
                    scale_factor1=sf1, scale_factor2=sf2, **fmatch_kw)
 
 
 if __name__ == '__main__':
     """
     CommandLine:
-        python -m plottool_ibeis.draw_sv
-        python -m plottool_ibeis.draw_sv --allexamples
-        python -m plottool_ibeis.draw_sv --allexamples --noface --nosrc
+        python -m plottool_ibeis.draw_sv all
     """
-    import multiprocessing
-    multiprocessing.freeze_support()  # for win32
-    ut.doctest_funcs()
+    import xdoctest
+    xdoctest.doctest_module(__file__)
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/fig_presenter.py` & `plottool_ibeis-2.3.0/plottool_ibeis/fig_presenter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from __future__ import absolute_import, division, print_function
 import sys
 import time
 import utool as ut
 import matplotlib as mpl
 from plottool_ibeis import custom_figure
 
 #from .custom_constants import golden_wh
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/interact_annotations.py` & `plottool_ibeis-2.3.0/plottool_ibeis/interact_annotations.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,33 @@
 
 References:
     Adapted from matplotlib/examples/event_handling/poly_editor.py
     Jan 9 2014: taken from: https://gist.github.com/tonysyu/3090704
 
 CommandLine:
     python -m plottool_ibeis.interact_annotations --test-test_interact_annots --show
+
+
+To Liberate:
+
+    import liberator
+    lib = liberator.Liberator()
+    lib.add_dynamic(AnnotationInteraction)
+    # lib.expand(['vtool', 'plottool', 'utool', 'plottool_ibeis'])
+    lib.expand(['plottool_ibeis'])
+    text = lib.current_sourcecode()
+
+    import kwplot
+    fpath = ub.Path(kwplot.__file__).parent / 'box_annotator.py'
+    fpath.write_text(text)
+
 """
 import six
 import re
+import ubelt as ub
 import numpy as np
 try:
     import vtool_ibeis as vt
 except ImportError:
     pass
 import utool as ut
 import itertools as it
@@ -117,15 +133,15 @@
             species,
             bbox={'facecolor': 'white', 'alpha': .8},
             verticalalignment='top',
         )
         poly.metadata_tag = ax.text(
             0, 0,
             #tagpos[0] + 5, tagpos[1] + 80,
-            ut.repr3(metadata_, nobr=True),
+            ub.urepr(metadata_, nobr=True, nl=True),
             bbox={'facecolor': 'white', 'alpha': .7},
             verticalalignment='top',
         )
         # ???
         poly.species_tag.remove()  # eliminate "leftover" copies
         poly.metadata_tag.remove()
         #
@@ -234,15 +250,18 @@
             # Add selected color
             sel_color = df2.ORANGE if poly.is_orig else df2.LIGHT_BLUE
             poly.lines.set_color(sel_color)
         else:
             line = poly.lines
             line_color = line.get_color()
             desel_color = df2.WHITE if poly.is_orig else df2.LIGHTGRAY
-            if np.any(line_color != np.array(desel_color)):
+            try:
+                if np.any(line_color != np.array(desel_color)):
+                    line.set_color(np.array(desel_color))
+            except Exception:
                 line.set_color(np.array(desel_color))
 
     def update_lines(poly):
         poly.lines.set_data(list(zip(*poly.xy)))
         poly.handle.set_data(list(zip(*poly.calc_handle_display_coords())))
 
     def set_species(poly, text):
@@ -358,15 +377,14 @@
         return is_within_distance_from_line(xy_pt, line, max_dist)
 
     @property
     def size(poly):
         return vt.bbox_from_verts(poly.xy)[2:4]
 
 
-@six.add_metaclass(ut.ReloadingMetaclass)
 class AnnotationInteraction(abstract_interaction.AbstractInteraction):
     """
     An interactive polygon editor.
 
     SeeAlso:
         ibeis.viz.interact.interact_annotations2
         (ensure that any updates here are propogated there)
@@ -463,15 +481,14 @@
         self.add_action_buttons()
         self.update_callbacks(next_callback, prev_callback)
 
     def reinitialize_figure(self, fnum=None):
         self.fig.clear()
         self.fig.clf()
         #self.fig.cla()
-        #ut.qflag()
         self.fnum = fnum
         #print(self.fnum)
         ax = df2.gca()
         #self.fig.ax = ax
         self.ax = ax
         df2.remove_patches(self.ax)
         df2.imshow(self.img, fnum=fnum)
@@ -489,15 +506,15 @@
             'Add Annotation\n' + pretty_hotkey_map(ADD_RECTANGLE_HOTKEY),
             rect=[0.18, 0.015, self.but_width, self.but_height],
             callback=self.add_new_poly
         )
         # self.append_button(
         #     'Add Full Annotation\n' + pretty_hotkey_map(ADD_RECTANGLE_FULL_HOTKEY),
         #     rect=[0.34, 0.015, self.but_width, self.but_height],
-        #     callback=ut.partial(self.add_new_poly, full=True)
+        #     callback=partial(self.add_new_poly, full=True)
         # )
         self.append_button(
             'Delete Annotation\n' + pretty_hotkey_map(DEL_RECTANGLE_HOTKEY),
             rect=[0.50, 0.015, self.but_width, self.but_height],
             callback=self.delete_current_poly
         )
         self.append_button(
@@ -618,22 +635,22 @@
         """
         get the index of the vertex under cursor if within max_dist tolerance
         """
         # Remove any deleted polygons
         poly_dict = {k: v for k, v in self.editable_polys.items() if v is not None}
         if len(poly_dict) > 0:
             poly_inds = list(poly_dict.keys())
-            poly_list = ut.take(poly_dict, poly_inds)
+            poly_list = list(ub.take(poly_dict, poly_inds))
             # Put polygon coords into figure space
             poly_pts = [poly.get_transform().transform(np.asarray(poly.xy))
                         for poly in poly_list]
             # Find the nearest vertex from the annotations
             ind_dist_list = [vt.nearest_point(x, y, polypts)
                              for polypts in poly_pts]
-            dist_lists = ut.take_column(ind_dist_list, 1)
+            dist_lists = [r[1] for r in ind_dist_list]
             min_idx = np.argmin(dist_lists)
             sel_polyind = poly_inds[min_idx]
             sel_vertx, sel_dist = ind_dist_list[min_idx]
             # Ensure nearest distance is within threshold
             if sel_dist >= self.max_dist ** 2:
                 sel_polyind, sel_vertx = (None, None)
         else:
@@ -893,15 +910,15 @@
         self.draw_artists()
 
     def _show_poly_context_menu(self, event):
         def _make_options():
             metadata = self._selected_poly.metadata
             options = []
             options += [
-                #('Foo: ',  ut.partial(print, 'bar')),
+                #('Foo: ',  partial(print, 'bar')),
                 #('Move to back ',  self._selected_poly.move_to_back),
                 ('PolyInfo: ',  self._selected_poly.print_info),
             ]
             if isinstance(metadata, ut.LazyDict):
                 options += metadata.nocache_eval('annot_context_options')
             return options
         options = _make_options()
@@ -1335,15 +1352,15 @@
         xy_pt[1] = ylim[0] - margin
     return True
 
 
 def test_interact_annots():
     r"""
     CommandLine:
-        python -m plottool_ibeis.interact_annotations --test-test_interact_annots --show
+        xdoctest -m plottool_ibeis.interact_annotations test_interact_annots --show
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> from plottool_ibeis.interact_annotations import *  # NOQA
         >>> import plottool_ibeis as pt
         >>> # build test data
         >>> # execute function
@@ -1356,15 +1373,15 @@
     verts_list = [
         ((0, 400), (400, 400), (400, 0), (0, 0), (0, 400)),
         ((400, 700), (700, 700), (700, 400), (400, 400), (400, 700))
     ]
     #if img is None:
     try:
         img_url = 'http://i.imgur.com/Vq9CLok.jpg'
-        img_fpath = ut.grab_file_url(img_url)
+        img_fpath = ub.grabdata(img_url, appname='plottool')
         img = vt.imread(img_fpath)
     except Exception as ex:
         print('[interact_annot] cant read zebra: %r' % ex)
         img = np.random.uniform(0, 255, size=(100, 100))
     valid_species = ['species1', 'species2']
     metadata_list = [{'name': 'foo'}, None]
     self = AnnotationInteraction(img, verts_list=verts_list,
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/interact_helpers.py` & `plottool_ibeis-2.3.0/plottool_ibeis/interact_helpers.py`

 * *Files identical despite different names*

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/interact_impaint.py` & `plottool_ibeis-2.3.0/plottool_ibeis/interact_impaint.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     http://stackoverflow.com/questions/22232812/drawing-on-image-with-matplotlib-and-opencv-update-image
     http://stackoverflow.com/questions/34933254/force-matplotlib-to-block-in-a-pyqt-thread-process
     http://matplotlib.org/examples/user_interfaces/embedding_in_qt4.html
     http://stackoverflow.com/questions/22410663/block-qmainwindow-while-child-widget-is-alive-pyqt
     http://stackoverflow.com/questions/20289939/pause-execution-until-button-press
 """
 import utool as ut
+import ubelt as ub
 import numpy as np
 try:
     import vtool_ibeis as vt
 except ImportError:
     pass
 from plottool_ibeis import abstract_interaction
 import math
@@ -37,20 +38,20 @@
             mask = np.full(img.shape, 255, dtype=np.uint8)
         else:
             mask = init_mask
         self.mask = mask
         self.img = img
         self.brush_size = 75
         import plottool_ibeis as pt
-        self.valid_colors1 = ut.odict([
+        self.valid_colors1 = ub.odict([
             #('background', (255 * pt.BLACK).tolist()),
             ('scenery', (255 * pt.BLACK).tolist()),
             ('photobomb', (255 * pt.RED).tolist()),
         ])
-        self.valid_colors2 = ut.odict([
+        self.valid_colors2 = ub.odict([
             ('foreground', (255 * pt.WHITE).tolist()),
         ])
         self.color1_idx = 0
         self.color1 = self.valid_colors1['scenery']
         self.color2 = self.valid_colors2['foreground']
         self.background = None
         self.last_stroke = None
@@ -73,15 +74,18 @@
         pt.imshow(self.mask, ax=self.ax, interpolation='nearest', alpha=0.6)
         self.update_title()
         self.ax.grid(False)
 
     def update_image(self):
         import plottool_ibeis as pt
         #print('update_image')
+
+        # FIXME: this is no longer available. How do we update?
         self.ax.images.pop()
+
         #self.ax.imshow(self.mask, interpolation='nearest', alpha=0.6)
         pt.imshow(self.mask, ax=self.ax, interpolation='nearest', alpha=0.6)
         self.draw()
         #self.do_blit()
         #self.update()
         #self.ax.imshow(vt.blend_images_multiply(self.img, self.mask))
         #self.ax.grid(False)
@@ -122,17 +126,17 @@
                 line_thickness = int(self.brush_size)
                 cv2.line(self.mask, center, old_center, color_bgr, line_thickness)
         self.last_stroke = (color, (x, y))
 
     def on_click_inside(self, event, ax):
         x = int(math.floor(event.xdata))
         y = int(math.floor(event.ydata))
-        if(event.button == self.LEFT_BUTTON):
+        if event.button == self.LEFT_BUTTON:
             self.apply_stroke(x, y, self.color1)
-        if(event.button == self.RIGHT_BUTTON):
+        if event.button == self.RIGHT_BUTTON:
             self.apply_stroke(x, y, self.color2)
         self.update_image()
         #self.draw()
         #self.print_status()
 
     def on_scroll(self, event):
         self.brush_size = max(self.brush_size + event.step, 1)
@@ -152,17 +156,17 @@
     def on_drag_stop(self, event):
         self.last_stroke = None
 
     def on_drag_inside(self, event):
         #self.print_status()
         x = int(math.floor(event.xdata))
         y = int(math.floor(event.ydata))
-        if(event.button == self.LEFT_BUTTON):
+        if  event.button == self.LEFT_BUTTON:
             self.apply_stroke(x, y, self.color1)
-        elif(event.button == self.RIGHT_BUTTON):
+        elif  event.button == self.RIGHT_BUTTON:
             self.apply_stroke(x, y, self.color2)
         self.update_image()
         #self.do_blit()
         #self.draw()
 
 
 def impaint_mask2(img, init_mask=None):
@@ -197,15 +201,15 @@
         >>> from plottool_ibeis.interact_impaint import *  # NOQA
         >>> result = draw_demo()
         >>> print(result)
         >>> import plottool_ibeis as pt
         >>> pt.show_if_requested()
     """
     import matplotlib.pyplot as plt
-    fpath = ut.grab_test_imgpath('zebra.png')
+    fpath = ut.grab_test_imgpath('astro')
     img = vt.imread(fpath)
     mask = impaint_mask2(img)
     print('mask = %r' % (mask,))
     print('mask.sum() = %r' % (mask.sum(),))
     if False:
         plt.imshow(vt.blend_images_multiply(img, mask))
         ax = plt.gca()
@@ -213,15 +217,11 @@
         ax.set_xticks([])
         ax.set_yticks([])
 
 
 if __name__ == '__main__':
     """
     CommandLine:
-        python -m plottool_ibeis.interact_impaint
-        python -m plottool_ibeis.interact_impaint --allexamples
-        python -m plottool_ibeis.interact_impaint --allexamples --noface --nosrc
-    """
-    import multiprocessing
-    multiprocessing.freeze_support()  # for win32
-    import utool as ut  # NOQA
-    ut.doctest_funcs()
+        python -m plottool_ibeis.interact_impaint all
+    """
+    import xdoctest
+    xdoctest.doctest_module(__file__)
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/interact_keypoints.py` & `plottool_ibeis-2.3.0/plottool_ibeis/interact_keypoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from plottool_ibeis import abstract_interaction
 (print, rrr, profile) = ut.inject2(__name__)
 
 
 class KeypointInteraction(abstract_interaction.AbstractInteraction):
     r"""
     CommandLine:
-        python -m plottool_ibeis.interact_keypoints --exec-KeypointInteraction --show
-        python -m plottool_ibeis.interact_keypoints --exec-KeypointInteraction --show --fname=lena.png
+        xdoctest -m plottool_ibeis.interact_keypoints KeypointInteraction --show
+        xdoctest -m plottool_ibeis.interact_keypoints KeypointInteraction --show --fname=astro.png
 
     Example:
         >>> # DISABLE_DOCTEST
         >>> from plottool_ibeis.interact_keypoints import *  # NOQA
         >>> import numpy as np
         >>> import plottool_ibeis as pt
         >>> import utool as ut
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/interact_matches.py` & `plottool_ibeis-2.3.0/plottool_ibeis/interact_matches.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """
 Unfinished non-ibeis dependent version of interact matches
 """
 import utool as ut
-import six
+import ubelt as ub
 import numpy as np
 from plottool_ibeis import abstract_interaction
 
 BASE_CLASS = abstract_interaction.AbstractInteraction
 
 
-# TODO: move to plottool_ibeis and decouple with IBEIS
-# TODO: abstract interaction
-@six.add_metaclass(ut.ReloadingMetaclass)
 class MatchInteraction2(BASE_CLASS):
     """
     TODO: replace functional version with this class
 
     Plots a chip result and sets up callbacks for interaction.
 
     SeeAlso:
@@ -130,15 +127,15 @@
 
         if verbose:
             print('self.warp_homog = %r' % (self.warp_homog,))
         if self.warp_homog:
             show_matches_kw['H1'] = self.H1
             show_matches_kw['H2'] = self.H2
         if verbose:
-            print('show_matches_kw = %s' % (ut.repr2(show_matches_kw, truncate=True)))
+            print('show_matches_kw = %s' % (ub.urepr(show_matches_kw)[0:10]))
 
         #tup = show_matches(fm, fs, **show_matches_kw)
         ax, xywh1, xywh2 = pt.show_chipmatch2(
             self.rchip1, self.rchip2,
             self.kpts1, self.kpts2,
             fm=self.fm, fs=self.fs,
             pnum=pnum, **show_matches_kw)
@@ -168,15 +165,15 @@
         rchip2     = self.rchip2
         self.mx    = mx
         print('+--- SELECT --- ')
         print('... selecting mx-th=%r feature match' % mx)
         fsv = self.fsv
         fs  = self.fs
         print('score stats:')
-        print(ut.repr2(ut.get_stats(fsv, axis=0), nl=1))
+        print(ub.urepr(ut.get_stats(fsv, axis=0), nl=1))
         print('fsv[mx] = %r' % (fsv[mx],))
         print('fs[mx] = %r' % (fs[mx],))
         #----------------------
         # Get info for the select_ith_match plot
         self.mode = 1
         # Get the mx-th feature match
         fx1, fx2 = self.fm[mx]
@@ -337,15 +334,11 @@
                                             mode='vec', fnum=fnum, pnum=pnum)
     #pt.set_title('Gradient orientation\n %s, fx=%d' % (get_aidstrs(aid), fx))
 
 
 if __name__ == '__main__':
     """
     CommandLine:
-        python -m plottool_ibeis.interact_matches
-        python -m plottool_ibeis.interact_matches --allexamples
-        python -m plottool_ibeis.interact_matches --allexamples --noface --nosrc
+        python ~/code/plottool_ibeis/plottool_ibeis/interact_matches.py all
     """
-    import multiprocessing
-    multiprocessing.freeze_support()  # for win32
-    import utool as ut  # NOQA
-    ut.doctest_funcs()
+    import xdoctest
+    xdoctest.doctest_module(__file__)
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/interact_multi_image.py` & `plottool_ibeis-2.3.0/plottool_ibeis/interact_multi_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,24 +8,22 @@
 from matplotlib.widgets import Button  # NOQA
 import matplotlib as mpl  # NOQA
 import six
 try:
     import vtool_ibeis as vt
 except ImportError:
     pass
-#import utool
 import utool as ut
 ut.noinject(__name__, '[pt.interact_multiimage]')
 
 
 BASE_CLASS = abstract_interaction.AbstractInteraction
 #BASE_CLASS = object
 
 
-@ut.reloadable_class
 class MultiImageInteraction(BASE_CLASS):
     """
 
     CommandLine:
         python -m plottool_ibeis.interact_multi_image --exec-MultiImageInteraction --show
 
     Example:
@@ -88,22 +86,23 @@
         super(MultiImageInteraction, self).__init__(fnum=fnum, **kwargs)
         #self.start()
 
     def dump_to_disk(self, dpath, num=None, prefix='temp_img'):
         import matplotlib.pyplot as plt  # NOQA
         import numpy as np
         import plottool_ibeis as pt
-        dpath = ut.ensurepath(dpath)
+        import ubelt as ub
+        dpath = ub.ensuredir(dpath)
         num_zeros = np.ceil(np.log10(len(self.gpath_list)))
         total = len(self.gpath_list)
         if num is None:
             num = total
         fmtstr = prefix + '_%0' + str(num_zeros) + 'd.jpg'
         fig = pt.figure(fnum=self.fnum)
-        for index in ut.ProgIter(range(num), lbl='dumping images to disk'):
+        for index in ub.ProgIter(range(num), desc='dumping images to disk'):
             fig = pt.figure(fnum=self.fnum)
             fig.clf()
             ax = self._plot_index(index, {'fnum': self.fnum})
             fig = ax.figure
             axes_extents = pt.extract_axes_extents(fig)
             assert len(axes_extents) == 1, 'more than one axes'
             extent = axes_extents[0]
@@ -166,15 +165,15 @@
         for px, index in enumerate(range(start_index, stop_index)):
             self.plot_image(index)
         self.make_hud()
         self.draw()
 
     def _plot_index(self, index, _vizkw):
         gpath      = self.gpath_list[index]
-        if ut.is_funclike(gpath):
+        if hasattr(gpath, '__call__'):
             showfunc = gpath
             # HACK
             # override of plot image function
             showfunc(**_vizkw)
             import plottool_ibeis as pt
             ax = pt.gca()
         else:
@@ -247,15 +246,15 @@
                 if self.context_option_funcs is not None:
                     #if event.button == 3:
                     options = self.context_option_funcs[index]()
                     self.show_popup_menu(options, event)
             elif self.MOUSE_BUTTONS[event.button] == 'left':
                 #bbox_list  = ph.get_plotdat(ax, 'bbox_list')
                 gpath = self.gpath_list[index]
-                if ut.is_funclike(gpath):
+                if hasattr(gpath, '__call__'):
                     print('gpath_isfunklike')
                     print('gpath = %r' % (gpath,))
                     import plottool_ibeis as pt
                     fnum = pt.next_fnum()
                     gpath(fnum=fnum)
                     df2.update()
                 else:
@@ -329,15 +328,11 @@
     #    self.prev_but.on_clicked(self.display_prev_page)
     #    # Connect the callback whenever the figure is clicked
 
 
 if __name__ == '__main__':
     """
     CommandLine:
-        python -m plottool_ibeis.interact_multi_image
-        python -m plottool_ibeis.interact_multi_image --allexamples
-        python -m plottool_ibeis.interact_multi_image --allexamples --noface --nosrc
+        python -m plottool_ibeis.interact_multi_image all
     """
-    import multiprocessing
-    multiprocessing.freeze_support()  # for win32
-    import utool as ut  # NOQA
-    ut.doctest_funcs()
+    import xdoctest
+    xdoctest.doctest_module(__file__)
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/interactions.py` & `plottool_ibeis-2.3.0/plottool_ibeis/interactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,18 +42,19 @@
         python -m plottool_ibeis.interactions --exec-ExpandableInteraction --show
 
     Example:
         >>> # DISABLE_DOCTEST
         >>> from plottool_ibeis.interactions import *  # NOQA
         >>> import numpy as np
         >>> import plottool_ibeis as pt
+        >>> from functools import partial
         >>> inter = pt.interactions.ExpandableInteraction()
-        >>> inter.append_plot(ut.partial(pt.plot_func, np.sin, stop=np.pi * 2))
-        >>> inter.append_plot(ut.partial(pt.plot_func, np.cos, stop=np.pi * 2))
-        >>> inter.append_plot(ut.partial(pt.plot_func, np.tan, stop=np.pi * 2))
+        >>> inter.append_plot(partial(pt.plot_func, np.sin, stop=np.pi * 2))
+        >>> inter.append_plot(partial(pt.plot_func, np.cos, stop=np.pi * 2))
+        >>> inter.append_plot(partial(pt.plot_func, np.tan, stop=np.pi * 2))
         >>> inter.start()
         >>> pt.show_if_requested()
     """
     def __init__(self, fnum=None, _pnumiter=None, interactive=None, **kwargs):
         self.nRows = kwargs.get('nRows', None)
         self.nCols = kwargs.get('nCols', None)
         self._pnumiter = _pnumiter
@@ -319,14 +320,11 @@
         ax.figure.canvas.draw()
         ax.figure.canvas.flush_events()
 
 
 if __name__ == '__main__':
     r"""
     CommandLine:
-        python -m plottool_ibeis.interactions
-        python -m plottool_ibeis.interactions --allexamples
+        python -m plottool_ibeis.interactions all
     """
-    import multiprocessing
-    multiprocessing.freeze_support()  # for win32
-    import utool as ut  # NOQA
-    ut.doctest_funcs()
+    import xdoctest
+    xdoctest.doctest_module(__file__)
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/mpl_keypoint.py` & `plottool_ibeis-2.3.0/plottool_ibeis/mpl_keypoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         kpts[:, 0:2] = kpts_
         kpts[:, 2] = 1
         kpts[:, 4] = 1
         kpts_ = kpts
 
     if scale_factor is None:
         scale_factor = 1.0
-    #print('[mpl_keypoint.draw_keypoints] kwargs = ' + ut.repr2(kwargs))
+    #print('[mpl_keypoint.draw_keypoints] kwargs = ' + ub.urepr(kwargs))
     # ellipse and point properties
     pts_size       = kwargs.get('pts_size', 2)
     pts_alpha      = kwargs.get('pts_alpha', 1.0)
     ell_alpha      = kwargs.get('ell_alpha', 1.0)
     ell_linewidth  = kwargs.get('ell_linewidth', 2)
     ell_color      = kwargs.get('ell_color', None)
     if ell_color is None:
@@ -172,15 +172,15 @@
 
 def _draw_pts(ax, _xs, _ys, pts_size, pts_color, pts_alpha=None):
     ptskw = dict(c=pts_color, s=(2 * pts_size), marker='o', edgecolor='none')
     OLD_WAY = False
     #if pts_alpha is not None:
     #    ptskw['alpha'] = pts_alpha
     if OLD_WAY:
-        #print(ut.repr2(ptskw))
+        #print(ub.urepr(ptskw))
         ax.scatter(_xs, _ys, **ptskw)
         # FIXME: THIS MIGHT CAUSE ISSUES: UNEXPECTED CALL
         #ax.autoscale(enable=False)
     else:
         pts_patches = [mpl.patches.Circle((x, y), radius=(pts_size / 2), fill=True)
                        for x, y in zip(_xs, _ys)]
         #print(pts_color)
@@ -228,15 +228,15 @@
     Returns matplotlib keypoint transformations (circle -> ellipse)
 
     Example:
         >>> # Test CV2 ellipse vs mine using MSER
         >>> import vtool_ibeis as vt
         >>> import cv2
         >>> import plottool_ibeis as pt
-        >>> img_fpath = ut.grab_test_imgpath(ut.get_argval('--fname', default='zebra.png'))
+        >>> img_fpath = ut.grab_test_imgpath(ut.get_argval('--fname', default='astro'))
         >>> imgBGR = vt.imread(img_fpath)
         >>> imgGray = cv2.cvtColor(imgBGR, cv2.COLOR_BGR2GRAY)
         >>> mser = cv2.MSER_create()
         >>> regions, bboxs = mser.detectRegions(imgGray)
         >>> region = regions[0]
         >>> bbox = bboxs[0]
         >>> vis = imgBGR.copy()
@@ -257,14 +257,15 @@
         >>> #R = np.eye(3)
         >>> invVR = T.dot(R).dot(S)
         >>> kpts = vt.flatten_invV_mats_to_kpts(np.array([invVR]))
         >>> pt.imshow(vis)
         >>> # MINE IS MUCH LARGER (by factor of 2)) WHY?
         >>> # we start out with a unit circle not a half circle
         >>> pt.draw_keypoints(pt.gca(), kpts, pts=True, ori=True, eig=True, rect=True)
+        >>> ut.show_if_requested()
     """
     import vtool_ibeis.keypoint as ktool
     #invVR_mats = ktool.get_invV_mats(kpts, with_trans=True, with_ori=True)
     invVR_mats = ktool.get_invVR_mats3x3(kpts)
     if H is None:
         invVR_aff2Ds = [mpl.transforms.Affine2D(invVR)
                         for invVR in invVR_mats]
@@ -360,15 +361,11 @@
 
     return ori_actors
 
 
 if __name__ == '__main__':
     """
     CommandLine:
-        python -m plottool_ibeis.mpl_keypoint
-        python -m plottool_ibeis.mpl_keypoint --allexamples
-        python -m plottool_ibeis.mpl_keypoint --allexamples --noface --nosrc
+        python -m plottool_ibeis.mpl_keypoint all
     """
-    import multiprocessing
-    multiprocessing.freeze_support()  # for win32
-    import utool as ut  # NOQA
-    ut.doctest_funcs()
+    import xdoctest
+    xdoctest.doctest_module(__file__)
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/mpl_sift.py` & `plottool_ibeis-2.3.0/plottool_ibeis/mpl_sift.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import itertools as it
 import numpy as np
 import matplotlib as mpl
 import utool as ut
+import ubelt as ub
 from plottool_ibeis import color_funcs as color_fns
 ut.noinject(__name__, '[pt.mpl_sift]')
 
 
 TAU = 2 * np.pi  # References: tauday.com
 BLACK  = np.array((0.0, 0.0, 0.0, 1.0))
 RED    = np.array((1.0, 0.0, 0.0, 1.0))
@@ -208,15 +209,15 @@
         path_effects.append(patheffects.Normal())
 
     if MULTI_COLORED_ARMS:
         # Hack in same colorscheme for arms as the sift bars
         ori_colors = color_fns.distinct_colors(16)
         arm_collections = [
             mpl.collections.PatchCollection(patches)
-            for patches in ut.ichunks(arm_patches, 8)
+            for patches in ub.chunks(arm_patches, chunksize=8)
         ]
         for col, color in zip(arm_collections, ori_colors):
             col.set_color(color)
     else:
         # Just use a single color for all the arms
         arm1_coll = mpl.collections.PatchCollection(arm_patches)
         arm1_coll.set_color(arm1_color)
@@ -301,15 +302,11 @@
     rendered = render.image
     return rendered
 
 
 if __name__ == '__main__':
     """
     CommandLine:
-        python -m plottool_ibeis.mpl_sift
-        python -m plottool_ibeis.mpl_sift --allexamples
-        python -m plottool_ibeis.mpl_sift --allexamples --noface --nosrc
+        python -m plottool_ibeis.mpl_sift all
     """
-    import multiprocessing
-    multiprocessing.freeze_support()  # for win32
-    import utool as ut  # NOQA
-    ut.doctest_funcs()
+    import xdoctest
+    xdoctest.doctest_module(__file__)
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/nx_helpers.py` & `plottool_ibeis-2.3.0/plottool_ibeis/nx_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,23 +15,24 @@
     sudo apt-get install libgraphviz-dev
     pip install pygraphviz
     sudo pip3 install pygraphviz \
         --install-option="--include-path=/usr/include/graphviz" \
         --install-option="--library-path=/usr/lib/graphviz/"
     python -c "import pygraphviz; print(pygraphviz.__file__)"
     python3 -c "import pygraphviz; print(pygraphviz.__file__)"
-
 """
 try:
     import dtool as dt
 except ImportError:
     pass
 import numpy as np
 import utool as ut
+import ubelt as ub
 from functools import reduce
+from collections import defaultdict
 (print, rrr, profile) = ut.inject2(__name__)
 
 __docstubs__ = """
 from typing import Union
 """
 
 
@@ -95,16 +96,16 @@
         >>> # xdoctest: +REQUIRES(module:pygraphviz)
         >>> from plottool_ibeis.nx_helpers import *  # NOQA
         >>> import networkx as nx
         >>> graph = nx.DiGraph()
         >>> graph.add_nodes_from(['a', 'b', 'c', 'd'])
         >>> graph.add_edges_from({'a': 'b', 'b': 'c', 'b': 'd', 'c': 'd'}.items())
         >>> nx.set_node_attributes(graph, name='shape', values='rect')
-        >>> nx.set_node_attributes(graph, name='image', values={'a': ut.grab_test_imgpath('carl.jpg')})
-        >>> nx.set_node_attributes(graph, name='image', values={'d': ut.grab_test_imgpath('astro.png')})
+        >>> nx.set_node_attributes(graph, name='image', values={'a': ut.grab_test_imgpath('carl')})
+        >>> nx.set_node_attributes(graph, name='image', values={'d': ut.grab_test_imgpath('astro')})
         >>> #nx.set_node_attributes(graph, name='height', values=100)
         >>> with_labels = True
         >>> fnum = None
         >>> pnum = None
         >>> e = show_nx(graph, with_labels, fnum, pnum, layout='agraph')
         >>> import plottool_ibeis as pt
         >>> pt.show_if_requested()
@@ -147,17 +148,17 @@
         ax.autoscale()
         ax.autoscale_view(True, True, True)
     #axes.facecolor
 
     node_size = layout_info['node'].get('size')
     node_pos = layout_info['node'].get('pos')
     if node_size is not None:
-        size_arr = np.array(ut.take(node_size, graph.nodes()))
+        size_arr = np.array(list(ub.take(node_size, graph.nodes())))
         half_size_arr = size_arr / 2.
-        pos_arr = np.array(ut.take(node_pos, graph.nodes()))
+        pos_arr = np.array(list(ub.take(node_pos, graph.nodes())))
         # autoscale does not seem to work
         #ul_pos = pos_arr - half_size_arr
         #br_pos = pos_arr + half_size_arr
         # hack because edges are cut off.
         # need to take into account extent of edges as well
         ul_pos = pos_arr - half_size_arr * 1.5
         br_pos = pos_arr + half_size_arr * 1.5
@@ -769,17 +770,17 @@
         >>>     pt.show_nx(graph2, layout='custom', pnum=(2, 2, 2), fnum=1)
         >>>     pt.show_nx(graph3, layout='custom', pnum=(2, 2, 3), fnum=1)
         >>>     pt.show_nx(graph4, layout='custom', pnum=(2, 2, 4), fnum=1)
         >>>     pt.show_if_requested()
         >>> data1 = dict(graph1.nodes(data=True))
         >>> data2 = dict(graph4.nodes(data=True))
         >>> dataP = dict(pinned_graph.nodes(data=True))
-        >>> print('data1 = {}'.format(ub.repr2(data1, nl=1)))
-        >>> print('data2 = {}'.format(ub.repr2(data2, nl=1)))
-        >>> print('dataP = {}'.format(ub.repr2(dataP, nl=1)))
+        >>> print('data1 = {}'.format(ub.urepr(data1, nl=1)))
+        >>> print('data2 = {}'.format(ub.urepr(data2, nl=1)))
+        >>> print('dataP = {}'.format(ub.urepr(dataP, nl=1)))
         >>> g1pos = nx.get_node_attributes(graph1, 'pos')['1']
         >>> g4pos = nx.get_node_attributes(graph4, 'pos')['1']
         >>> g2pos = nx.get_node_attributes(graph2, 'pos')['1']
         >>> g3pos = nx.get_node_attributes(graph3, 'pos')['1']
         >>> print('g1pos = {!r}'.format(g1pos))
         >>> print('g4pos = {!r}'.format(g4pos))
         >>> print('g2pos = {!r}'.format(g2pos))
@@ -896,16 +897,16 @@
         test_fpath = ut.truepath('~/test_graphviz_draw.png')
         agraph.draw(test_fpath)
         ut.startfile(test_fpath)
     if verbose > 3:
         print('AFTER LAYOUT\n' + str(agraph))
 
     # TODO: just replace with a single dict of attributes
-    node_layout_attrs = ut.ddict(dict)
-    edge_layout_attrs = ut.ddict(dict)
+    node_layout_attrs = defaultdict(dict)
+    edge_layout_attrs = defaultdict(dict)
 
     #for node in agraph.nodes():
     for node in graph_.nodes():
         anode = pygraphviz.Node(agraph, node)
         node_attrs = parse_anode_layout_attrs(anode)
         for key, val in node_attrs.items():
             node_layout_attrs[key][node] = val
@@ -1156,18 +1157,18 @@
     # edge_startpoints = layout_info['edge']['start_pt']
 
     if as_directed is None:
         as_directed = graph.is_directed()
 
     # Draw nodes
     large_graph = len(graph) > LARGE_GRAPH
-    #for edge, pts in ut.ProgIter(edge_pos.items(), length=len(edge_pos), enabled=large_graph, lbl='drawing edges'):
+    #for edge, pts in ub.ProgIter(edge_pos.items(), total=len(edge_pos), enabled=large_graph, desc='drawing edges'):
 
-    for node, nattrs in ut.ProgIter(graph.nodes(data=True), length=len(graph),
-                                    lbl='drawing nodes', enabled=large_graph):
+    for node, nattrs in ub.ProgIter(graph.nodes(data=True), total=len(graph),
+                                    desc='drawing nodes', enabled=large_graph):
         # shape = nattrs.get('shape', 'circle')
         if nattrs is None:
             nattrs = {}
         label = nattrs.get('label', None)
         alpha = nattrs.get('alpha', 1.0)
         node_color = nattrs.get('color', pt.NEUTRAL_BLUE)
         if node_color is None:
@@ -1321,16 +1322,16 @@
 
     ###
     # Draw Edges
     # NEW WAY OF DRAWING EDGEES
     edge_pos = layout_info['edge'].get('ctrl_pts', None)
     n_invis_edge = 0
     if edge_pos is not None:
-        for edge, pts in ut.ProgIter(edge_pos.items(), length=len(edge_pos),
-                                     enabled=large_graph, lbl='drawing edges'):
+        for edge, pts in ub.ProgIter(edge_pos.items(), total=len(edge_pos),
+                                     enabled=large_graph, desc='drawing edges'):
             data = get_default_edge_data(graph, edge)
 
             if data.get('style', None) == 'invis':
                 n_invis_edge += 1
                 continue
 
             alpha = data.get('alpha', None)
@@ -1399,16 +1400,16 @@
             else:
                 width = .5
                 lw = 1.0
                 try:
                     import vtool_ibeis as vt
                     # Compute arrow width using estimated graph size
                     if node_size is not None and node_pos is not None:
-                        xys = np.array(ut.take(node_pos, node_pos.keys())).T
-                        whs = np.array(ut.take(node_size, node_pos.keys())).T
+                        xys = np.array(list(ub.take(node_pos, node_pos.keys()))).T
+                        whs = np.array(list(ub.take(node_size, node_pos.keys()))).T
                         bboxes = vt.bbox_from_xywh(xys, whs, [.5, .5])
                         extents = vt.extent_from_bbox(bboxes)
                         tl_pts = np.array([extents[0], extents[2]]).T
                         br_pts = np.array([extents[1], extents[3]]).T
                         pts = np.vstack([tl_pts, br_pts])
                         extent = vt.get_pointset_extents(pts)
                         graph_w, graph_h = vt.bbox_from_extent(extent)[2:4]
@@ -1647,16 +1648,13 @@
 #             yarrow = ax.annotate(ylabel, xy[::-1], xycoords=xycoords[::-1],
 #                                  xytext=xytext[::-1], textcoords=textcoords[::-1],
 #                                  ha='center', va=va, arrowprops=arrowprops)
 #     return xarrow, yarrow
 
 
 if __name__ == '__main__':
-    r"""
+    """
     CommandLine:
-        python -m plottool_ibeis.nx_helpers
-        python -m plottool_ibeis.nx_helpers --allexamples
+        python -m plottool_ibeis.nx_helpers all
     """
-    import multiprocessing
-    multiprocessing.freeze_support()  # for win32
-    import utool as ut  # NOQA
-    ut.doctest_funcs()
+    import xdoctest
+    xdoctest.doctest_module(__file__)
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/other.py` & `plottool_ibeis-2.3.0/plottool_ibeis/other.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # I'm not quite sure how to organize these functions yet
-from __future__ import absolute_import, division, print_function
 import numpy as np
 import vtool_ibeis.histogram as htool
 import utool as ut
 ut.noinject(__name__, '[pt.other]')
 
 
 def color_orimag(gori, gmag):
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/plot_helpers.py` & `plottool_ibeis-2.3.0/plottool_ibeis/plot_helpers.py`

 * *Files identical despite different names*

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/plots.py` & `plottool_ibeis-2.3.0/plottool_ibeis/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from functools import reduce
 from plottool_ibeis import draw_func2 as df2
 import ubelt as ub
 import scipy.stats
 import matplotlib as mpl
 import utool as ut  # NOQA
 import numpy as np
+from functools import partial
 print, rrr, profile = ut.inject2(__name__)
 
 
 __docstubs__ = """
 from typing import Union
 """
 
@@ -94,15 +95,15 @@
             # Special-er case where xdata is specified in ydata
             xkey = xdata
             ykeys = ut.setdiff(ydata_list.keys(), [xkey])
             xdata = ydata_list[xkey]
         else:
             ykeys = list(ydata_list.keys())
         # Normalize input
-        ydata_list = ut.take(ydata_list, ykeys)
+        ydata_list = list(ub.take(ydata_list, ykeys))
         kwargs['label_list'] = kwargs.get('label_list', ykeys)
 
     def is_listlike(data):
         flag = isinstance(data, (list, np.ndarray, tuple))
         flag &= hasattr(data, '__getitem__') and hasattr(data, '__len__')
         return flag
 
@@ -568,15 +569,15 @@
         >>> pt.present()
         >>> import plottool_ibeis as pt
         >>> pt.show_if_requested()
     """
     import matplotlib.font_manager
     avail_fonts = matplotlib.font_manager.findSystemFonts(fontpaths=None, fontext='ttf')
     names = [matplotlib.font_manager.FontProperties(fname=fname).get_name() for fname in avail_fonts]
-    print('avail_fonts = %s' % ut.repr4(sorted(set(names))))
+    print('avail_fonts = %s' % ub.urepr(sorted(set(names))))
 
     xdata = [1, 2, 3, 4, 5]
     ydata_list = [[1, 2, 3, 4, 5], [3, 3, 3, 3, 3], [5, 4, np.nan, 2, 1], [4, 3, np.nan, 1, 0]]
     kwargs = {'label_list': ['spamΣ', 'eggs', 'jamµ', 'pram'],  'linestyle': '-'}
     f = ['DejaVu Sans', 'Bitstream Vera Sans', 'Lucida Grande', 'Verdana', 'Geneva',
          'Lucid', 'Arial', 'Helvetica', 'Avant Garde', 'sans-serif']
     f = ['DejaVu Sans', 'Verdana', 'Arial']
@@ -961,15 +962,15 @@
         >>> plot_rank_cumhist(cdf_list, label_list, edges=edges, xmin=.9, num_xticks=numranks, fnum=fnum, pnum=(2, 1, 1), kind='plot', ymin=0, ymax=100)
         >>> ax1 = pt.gca()
         >>> plot_rank_cumhist(cdf_list.T[0:top].T, label_list, edges=edges[0:top + 1], xmin=.9, num_xticks=top, fnum=fnum, pnum=(2, 1, 2), kind='plot', ymin=0, ymax=100)
         >>> ax2 = pt.gca()
         >>> xmin = 1
         >>> xmax = top
         >>> (c1, c2, bbox_patch1, bbox_patch2, p) = zoom_effect01(ax1, ax2, xmin, xmax)
-        >>> result = ('(c1, c2, bbox_patch1, bbox_patch2, p) = %s' % (ut.repr2((c1, c2, bbox_patch1, bbox_patch2, p)),))
+        >>> result = ('(c1, c2, bbox_patch1, bbox_patch2, p) = %s' % (ub.urepr((c1, c2, bbox_patch1, bbox_patch2, p)),))
         >>> print(result)
         >>> ut.quit_if_noshow()
         >>> import plottool_ibeis as pt
         >>> pt.show_if_requested()
 
     """
     from matplotlib.transforms import (
@@ -1297,16 +1298,14 @@
             #     #    _p.set_edgecolor(None)
             _n_min = min(_n_min, _n.min())
             _n_max = max(_n_max, _n.max())
             _bin_max = max(_bin_max, max(_bins))
         except Exception as ex:
             ut.printex(ex, 'probably gave negative scores', keys=[
                 'bins', 'data', 'total_min'])
-            import utool
-            utool.embed()
             raise
 
             if ut.SUPER_STRICT:
                 raise
 
     if True:
         # TODO:
@@ -1336,15 +1335,15 @@
         if symlogkw.get('basey', 10) > 0:
             print('YSCALE')
             ax.set_yscale('symlog', **symlogkw)
         # ax.set_xscale('symlog', nonposx='clip')
         # ax.set_yscale('symlog', nonposy='clip')
         # ax.set_xscale('log', nonposx='clip')
         # ax.set_yscale('log', nonposy='clip')
-        # set_logyscale_from_data(sorted(ut.flatten(scores_list)))
+        # set_logyscale_from_data(sorted(ub.flatten(scores_list)))
 
     if overlay_score_domain is not None:
         ax  = df2.gca()
         p_max = max([prob.max() for prob in overlay_prob_given_list])
         scale_factor = _n_max / p_max
         for lblx in list(range(len(scores_list))):
             color = score_colors[lblx]
@@ -2075,16 +2074,16 @@
         colors[-1] = pt.GRAY
     #xints = np.arange(len(bin_labels))
 
     pt.figure(fnum=fnum, pnum=pnum)
     mask = freq > 0
     masked_freq   = freq.compress(mask, axis=0)
     size = masked_freq.sum()
-    masked_lbls   = ut.compress(bin_labels, mask)
-    masked_colors = ut.compress(colors, mask)
+    masked_lbls   = list(ub.compress(bin_labels, mask))
+    masked_colors = list(ub.compress(colors, mask))
     explode = [0] * len(masked_freq)
     masked_percent = (masked_freq * 100 / size)
     plt.pie(masked_percent, explode=explode, autopct='%1.1f%%',
                labels=masked_lbls, colors=masked_colors)
     #ax = pt.gca()
     pt.set_xlabel(label + '\nsize=%d' % (size,))
     pt.gca().set_aspect('equal')
@@ -2111,19 +2110,19 @@
         >>> #text_list = [x.strip() for x in ut.lorium_ipsum().split()]
         >>> result = word_histogram2(text_list, weight_list)
         >>> import plottool_ibeis as pt
         >>> pt.show_if_requested()
     """
     import matplotlib.pyplot as plt
     import plottool_ibeis as pt
-    text_hist = ut.dict_hist(text_list, weight_list=weight_list)
+    text_hist = ub.dict_hist(text_list, weights=weight_list)
     text_vals = list(text_hist.values())
     sortx = ut.list_argsort(text_vals)[::-1]
-    bin_labels = ut.take(list(text_hist.keys()), sortx)
-    freq = np.array(ut.take(text_vals, sortx))
+    bin_labels = list(ub.take(list(text_hist.keys()), sortx))
+    freq = np.array(list(ub.take(text_vals, sortx)))
     xints = np.arange(len(bin_labels))
 
     width = .95
     ymax = freq.max() if len(freq) > 0 else 0
 
     if len(freq) == 0:
         freq_max = 1
@@ -2256,16 +2255,16 @@
             # bw_low = day
             # bw_high = (maxtime - mintime) / 10
             grid_params = {
                 # 'bandwidth': np.logspace(np.log(bw_low), np.log(bw_high), 30)
                 # 'bandwidth': np.linspace(bw_low, bw_high, 30)
                 'bandwidth': np.linspace(day, day * 14, 14)
             }
-            # searcher = ut.partial(GridSearchCV, n_jobs=7)
-            searcher = ut.partial(RandomizedSearchCV, n_iter=5, n_jobs=8)
+            # searcher = partial(GridSearchCV, n_jobs=7)
+            searcher = partial(RandomizedSearchCV, n_iter=5, n_jobs=8)
             print('Searching for best bandwidth')
             grid = searcher(KernelDensity(kernel='gaussian'),
                                 grid_params, cv=2, verbose=0)
             grid.fit(unixtimes[:, None])
             bw = grid.best_params_['bandwidth']
             # print('bw = %r' % (bw,))
         # else:
@@ -2399,15 +2398,11 @@
         pt.imshow_null('NO WORDCLOUD DATA', ax=ax)
     ax.axis('off')
 
 
 if __name__ == '__main__':
     """
     CommandLine:
-        python -m plottool_ibeis.plots
-        python -m plottool_ibeis.plots --allexamples
-        python -m plottool_ibeis.plots --allexamples --noface --nosrc
-    """
-    import multiprocessing
-    multiprocessing.freeze_support()  # for win32
-    import utool as ut  # NOQA
-    ut.doctest_funcs()
+        python -m plottool_ibeis.plots all
+    """
+    import xdoctest
+    xdoctest.doctest_module(__file__)
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/screeninfo.py` & `plottool_ibeis-2.3.0/plottool_ibeis/screeninfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import six
 import sys
 import utool as ut
+import ubelt as ub
 import numpy as np
+from collections import OrderedDict
 try:
     import guitool_ibeis as gt
     from guitool_ibeis.__PYQT__ import QtWidgets
     from guitool_ibeis.__PYQT__ import QtCore
 except ImportError:
     try:
         from PyQt4 import QtGui as QtWidgets
@@ -82,15 +84,15 @@
         sympy.Eq(inches_diag, (inches_w ** 2 + inches_h ** 2) ** .5),
         sympy.Eq(res_w / res_h, inches_w / inches_h),
     ]
     print('Possible solutions:')
     query_vars = [inches_w, inches_h]
     for solution in sympy.solve(equations, query_vars):
         print('Solution:')
-        reprstr = ut.repr3(ut.odict(zip(query_vars, solution)), explicit=True, nobr=1, with_comma=False)
+        reprstr = ub.urepr(OrderedDict(zip(query_vars, solution)), explicit=True, nobr=1, with_comma=False, nl=True)
         print(ut.indent(ut.autopep8_format(reprstr)))
     #(inches_diag*res_w/sqrt(res_h**2 + res_w**2), inches_diag*res_h/sqrt(res_h**2 + res_w**2))
 
 
 def get_resolution_info(monitor_num=0):
     r"""
     Args:
@@ -106,15 +108,15 @@
 
     Example:
         >>> # DISABLE_DOCTEST
         >>> from plottool_ibeis.screeninfo import *  # NOQA
         >>> monitor_num = 1
         >>> for monitor_num in range(get_number_of_monitors()):
         >>>     info = get_resolution_info(monitor_num)
-        >>>     print('monitor(%d).info = %s' % (monitor_num, ut.repr3(info, precision=3)))
+        >>>     print('monitor(%d).info = %s' % (monitor_num, ub.urepr(info, nl=True, precision=3)))
     """
     import guitool_ibeis as gt
     app = gt.ensure_qtapp()[0]  # NOQA
     # screen_resolution = app.desktop().screenGeometry()
     # width, height = screen_resolution.width(), screen_resolution.height()
     # print('height = %r' % (height,))
     # print('width = %r' % (width,))
@@ -204,15 +206,15 @@
     mm_w = inches_w * ut.MM_PER_INCH
     mm_h = inches_h * ut.MM_PER_INCH
     mm_diag = inches_diag * ut.MM_PER_INCH
 
     ratio = min(mm_w, mm_h) / max(mm_w, mm_h)
 
     #pixel_density = dpi_x / ppi_x
-    info = ut.odict([
+    info = OrderedDict([
         ('monitor_num', monitor_num),
         ('off_x', off_x),
         ('off_y', off_y),
         ('ratio', ratio),
         ('ppi_x', ppi_x),
         ('ppi_y', ppi_y),
         ('dpi_x', dpi_x),
@@ -252,15 +254,15 @@
         python -m plottool_ibeis.screeninfo get_monitor_geom --show
 
     Example:
         >>> # DISABLE_DOCTEST
         >>> from plottool_ibeis.screeninfo import *  # NOQA
         >>> monitor_num = 0
         >>> geom = get_monitor_geom(monitor_num)
-        >>> result = ('geom = %s' % (ut.repr2(geom),))
+        >>> result = ('geom = %s' % (ub.urepr(geom),))
         >>> print(result)
     """
     gt.ensure_qtapp()
     desktop = QtWidgets.QDesktopWidget()
     rect = desktop.availableGeometry(screen=monitor_num)
     geom = (rect.x(), rect.y(), rect.width(), rect.height())
     return geom
@@ -362,14 +364,11 @@
     valid_positions = [get_position_ix(ix) for ix in range(num_wins)]
     return valid_positions
 
 
 if __name__ == '__main__':
     r"""
     CommandLine:
-        python -m plottool_ibeis.screeninfo
-        python -m plottool_ibeis.screeninfo --allexamples
+        python -m plottool_ibeis.screeninfo all
     """
-    import multiprocessing
-    multiprocessing.freeze_support()  # for win32
-    import utool as ut  # NOQA
-    ut.doctest_funcs()
+    import xdoctest
+    xdoctest.doctest_module(__file__)
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/test_colorsys.py` & `plottool_ibeis-2.3.0/plottool_ibeis/test_colorsys.py`

 * *Files identical despite different names*

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/test_vtk_poly.py` & `plottool_ibeis-2.3.0/plottool_ibeis/test_vtk_poly.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,19 @@
     hu = .5  # half unit
     d = np.sqrt((fu ** 2) / 2)  # diag
     hh = hu + d  # half height
 
     # left view faces us
 
     import utool as ut
+    import ubelt as ub
     import six
     import itertools
-    counter = ut.partial(six.next, itertools.count(0))
+    from functools import partial
+    counter = partial(six.next, itertools.count(0))
 
     vertex_locations = vtk.vtkPoints()
     vertex_locations.SetNumberOfPoints(24)
 
     p1, p2, p3 = np.array([
         (-hu, -hu, hh),
         ( hu, -hu, hh),
@@ -40,30 +42,30 @@
     # VERTEXES
     # left, up, back
     vplist = ['L', 'U', 'B', 'R', 'D', 'F']
     vpdict = {}
     print('perms = %r' % (perms,))
     for x in range(3):
         vp = vplist[x]
-        p = np.vstack(ut.take(plist, perms[x])).T
+        p = np.vstack(list(ub.take(plist, perms[x]))).T
         counts = [counter() for z in range(4)]
         vpdict[vp] = counts
         vertex_array.extend(p.tolist())
         vertex_locations.SetPoint(counts[0], p[0])
         vertex_locations.SetPoint(counts[1], p[1])
         vertex_locations.SetPoint(counts[2], p[2])
         vertex_locations.SetPoint(counts[3], p[3])
 
     # three more of the six main faces
     perms = [(0, 1, 2), (0, 2, 1), (2, 0, 1)]
     plist[-1] = -plist[-1]
     # right, down, front
     print('perms = %r' % (perms,))
     for x in range(3):
-        p = np.vstack(ut.take(plist, perms[x])).T
+        p = np.vstack(list(ub.take(plist, perms[x]))).T
         counts = [counter() for z in range(4)]
         vp = vplist[x + 3]
         vpdict[vp] = counts
         vertex_array.extend(p.tolist())
         vertex_locations.SetPoint(counts[0], p[0])
         vertex_locations.SetPoint(counts[1], p[1])
         vertex_locations.SetPoint(counts[2], p[2])
@@ -146,19 +148,17 @@
     mapper.SetInput(ug)
 
     actor = vtk.vtkActor()
     actor.SetMapper(mapper)
 
     if 1:
         # Read the image data from a file
-        import utool as ut
-
         textureCoords = vtk.vtkFloatArray()
         textureCoords.SetNumberOfComponents(3)
-        #coords = ut.take(vertex_array, face_dict['L'])
+        #coords = list(ub.take(vertex_array, face_dict['L']))
         #for coord in coords:
         #    textureCoords.InsertNextTuple(tuple(coord))
         textureCoords.InsertNextTuple((0, 0, 0))
         textureCoords.InsertNextTuple((1, 0, 0))
         textureCoords.InsertNextTuple((1, 1, 0))
         textureCoords.InsertNextTuple((0, 1, 0))
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/tests/test_helpers.py` & `plottool_ibeis-2.3.0/plottool_ibeis/tests/test_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from __future__ import absolute_import, division, print_function
 
 
 def dummy_bbox(img, shiftxy=(0.0, 0.0), scale=.25):
     """Default to rectangle that has a quarter-width/height border."""
     (gh, gw) = img.shape[0:2]
     half_w = gw / 2
     half_h = gh / 2
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/tests/test_interact_multi_image.py` & `plottool_ibeis-2.3.0/plottool_ibeis/tests/test_interact_multi_image.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python
 
 # DUPLICATE CODE, DELETE
-from __future__ import absolute_import, division, print_function
 from plottool_ibeis import interact_multi_image
 from plottool_ibeis import draw_func2 as df2
 import utool
 #import ibeis
 
 
 def run_test_interact_multimage(imgpaths):
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/tests/test_viz_image2.py` & `plottool_ibeis-2.3.0/plottool_ibeis/tests/test_viz_image2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-from __future__ import absolute_import, division, print_function
 from plottool_ibeis import viz_image2
 from plottool_ibeis import draw_func2 as df2
 import cv2
 import utool
 import numpy as np
 from plottool_ibeis.tests.test_helpers import dummy_bbox
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/tests/test_viz_images.py` & `plottool_ibeis-2.3.0/plottool_ibeis/tests/test_viz_images.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-from __future__ import absolute_import, division, print_function
 from plottool_ibeis import viz_image2
 from plottool_ibeis import draw_func2 as df2
 from plottool_ibeis import plot_helpers as ph
 import utool
 import numpy as np
 from plottool_ibeis.tests.test_helpers import dummy_bbox, imread_many
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/viz_featrow.py` & `plottool_ibeis-2.3.0/plottool_ibeis/viz_featrow.py`

 * *Files 4% similar despite different names*

```diff
@@ -190,15 +190,11 @@
         custom_figure.set_xlabel(dist_str)
     return px + nCols
 
 
 if __name__ == '__main__':
     """
     CommandLine:
-        python -m plottool_ibeis.viz_featrow
-        python -m plottool_ibeis.viz_featrow --allexamples
-        python -m plottool_ibeis.viz_featrow --allexamples --noface --nosrc
+        python -m plottool_ibeis.viz_featrow all
     """
-    import multiprocessing
-    multiprocessing.freeze_support()  # for win32
-    import utool as ut  # NOQA
-    ut.doctest_funcs()
+    import xdoctest
+    xdoctest.doctest_module(__file__)
```

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/viz_image2.py` & `plottool_ibeis-2.3.0/plottool_ibeis/viz_image2.py`

 * *Files identical despite different names*

### Comparing `plottool_ibeis-2.2.1/plottool_ibeis/viz_keypoints.py` & `plottool_ibeis-2.3.0/plottool_ibeis/viz_keypoints.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import utool
 import plottool_ibeis.draw_func2 as df2
 import numpy as np
 from plottool_ibeis import plot_helpers as ph
-#(print, print_, printDBG, rrr, profile) = utool.inject(__name__, '[viz_keypoints]', DEBUG=False)
 utool.noinject(__name__, '[viz_keypoints]')
 
 
 def testdata_kpts():
     import utool as ut
     import vtool_ibeis as vt
     import pyhesaff
@@ -37,56 +36,61 @@
         >>> from plottool_ibeis.viz_keypoints import *  # NOQA
         >>> import vtool_ibeis as vt
         >>> kpts, vecs, chip = testdata_kpts()
         >>> fnum = 0
         >>> pnum = None
         >>> result = show_keypoints(chip, kpts, fnum, pnum)
         >>> print(result)
+        >>> import utool as ut
+        >>> ut.show_if_requested()
     """
     #printDBG('[df2.show_kpts] %r' % (kwargs.keys(),))
     fig, ax = df2.imshow(chip, fnum=fnum, pnum=pnum, **kwargs)
     _annotate_kpts(kpts, **kwargs)
     ph.set_plotdat(ax, 'viztype', 'keypoints')
     ph.set_plotdat(ax, 'kpts', kpts)
     if kwargs.get('ddd', False):
         ph.draw()
 
 
-#@utool.indent_func
 def _annotate_kpts(kpts_, sel_fx=None, **kwargs):
     r"""
     Args:
         kpts_ (ndarray): keypoints
         sel_fx (None | Any):
 
     Keywords:
         color:  3/4-tuple, ndarray, or str
 
     Example:
-        >>> from plottool_ibeis.viz_keypoints import *  # NOQA
+        >>> from plottool_ibeis.viz_keypoints import _annotate_kpts
         >>> sel_fx = None
         >>> kpts = np.array([[  92.9246,   17.5453,    7.8103,   -3.4594,   10.8566,    0.    ],
         ...                  [  76.8585,   24.7918,   11.4412,   -3.2634,    9.6287,    0.    ],
         ...                  [ 140.6303,   24.9027,   10.4051,  -10.9452, 10.5991,    0.    ],])
+        >>> _annotate_kpts(kpts)
+        >>> import utool as ut
+        >>> ut.show_if_requested()
 
     """
     if len(kpts_) == 0:
         print('len(kpts_) == 0...')
         return
     #color = kwargs.get('color', 'distinct' if sel_fx is None else df2.ORANGE)
     color = kwargs.get('color', 'scale' if sel_fx is None else df2.ORANGE)
-    if color == 'distinct':
-        # hack for distinct colors
-        color = df2.distinct_colors(len(kpts_))  # , randomize=True)
-    elif color == 'scale':
-        # hack for distinct colors
-        import vtool_ibeis as vt
-        #color = df2.scores_to_color(vt.get_scales(kpts_), cmap_='inferno', score_range=(0, 50))
-        color = df2.scores_to_color(vt.get_scales(kpts_), cmap_='viridis', score_range=(5, 30), cmap_range=None)
-        #df2.distinct_colors(len(kpts_))  # , randomize=True)
+    if isinstance(color, str):
+        if color == 'distinct':
+            # hack for distinct colors
+            color = df2.distinct_colors(len(kpts_))  # , randomize=True)
+        elif color == 'scale':
+            # hack for distinct colors
+            import vtool_ibeis as vt
+            #color = df2.scores_to_color(vt.get_scales(kpts_), cmap_='inferno', score_range=(0, 50))
+            color = df2.scores_to_color(vt.get_scales(kpts_), cmap_='viridis', score_range=(5, 30), cmap_range=None)
+            #df2.distinct_colors(len(kpts_))  # , randomize=True)
     # Keypoint drawing kwargs
     drawkpts_kw = {
         'ell': True,
         'pts': False,
         'ell_alpha': .4,
         'ell_linewidth': 2,
         'ell_color': color,
@@ -97,16 +101,16 @@
     if sel_fx is None:
         df2.draw_kpts2(kpts_, **drawkpts_kw)
     else:
         # dont draw the selected keypoint in this batch
         nonsel_kpts_ = np.vstack((kpts_[0:sel_fx], kpts_[sel_fx + 1:]))
         # Draw selected keypoint
         sel_kpts = kpts_[sel_fx:sel_fx + 1]
-        import utool as ut
-        if ut.isiterable(color) and ut.isiterable(color[0]):
+        import ubelt as ub
+        if ub.iterable(color) and ub.iterable(color[0]):
             # hack for distinct colors
             drawkpts_kw['ell_color'] = color[0:sel_fx] + color[sel_fx + 1:]
         drawkpts_kw
         drawkpts_kw2 = drawkpts_kw.copy()
         drawkpts_kw2.update({
             'ell_color': df2.BLUE,
             'eig':  True,
```

### Comparing `plottool_ibeis-2.2.1/pyproject.toml` & `plottool_ibeis-2.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -9,29 +9,35 @@
 rel_mod_parent_dpath = "."
 tags = [ "erotemic", "purepy", "github", "cv2"]
 mod_name = "plottool_ibeis"
 repo_name = "plottool_ibeis"
 os = [ "win", "linux", "osx",]
 ci_pypy_versions = []
 # ci_cpython_versions = ["3.7", "3.8", "3.9", "3.10"]
-supported_python_versions = ["3.7", "3.8", "3.9", "3.10"]
-description = "Plottool - tools matplotlib computer vision plots"
+# supported_python_versions = ["3.8", "3.9", "3.10", "3.11", "3.12"]
+description = "Plottool - tools for matplotlib computer vision plots"
 url="https://github.com/Erotemic/plottool_ibeis"
 author="Jon Crall"
 author_email="erotemic@gmail.com"
-min_python = 3.7
+min_python = 3.8
 version = "{mod_dpath}/__init__.py::__version__"
 license = "Apache 2"
 dev_status = "beta"
 autostage = true
 
 [tool.pytest.ini_options]
-addopts = "-p no:doctest --xdoctest --xdoctest-style=google --ignore-glob=setup.py"
-norecursedirs = ".git ignore build __pycache__ dev _skbuild"
-filterwarnings = [ "default", "ignore:.*No cfgstr given in Cacher constructor or call.*:Warning", "ignore:.*Define the __nice__ method for.*:Warning", "ignore:.*private pytest class or function.*:Warning",]
+addopts = "-p no:doctest --xdoctest --xdoctest-style=google --ignore-glob=setup.py --ignore-glob=docs"
+norecursedirs = ".git ignore build __pycache__ dev _skbuild docs"
+filterwarnings = [
+    "default",
+    "ignore:.*No cfgstr given in Cacher constructor or call.*:Warning",
+    "ignore:.*Define the __nice__ method for.*:Warning",
+    "ignore:.*private pytest class or function.*:Warning",
+]
+
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 exclude_lines = [ "pragma: no cover", ".*  # pragma: no cover", ".*  # nocover", "def __repr__", "raise AssertionError", "raise NotImplementedError", "if 0:", "if trace is not None", "verbose = .*", "^ *raise", "^ *pass *$", "if _debug:", "if __name__ == .__main__.:", ".*if six.PY2:",]
 omit = [ "plottool_ibeis/__main__.py", "*/setup.py",]
```

### Comparing `plottool_ibeis-2.2.1/setup.py` & `plottool_ibeis-2.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # Generated by ~/code/xcookie/xcookie/builders/setup.py
 # based on part ~/code/xcookie/xcookie/rc/setup.py.in
 import sys
-from os.path import exists
+import re
+from os.path import exists, dirname, join
 from setuptools import find_packages
 from setuptools import setup
 
 
 def parse_version(fpath):
     """
     Statically parse the version number from a python file
@@ -49,16 +50,14 @@
     """
     Parse the description in the README file
 
     CommandLine:
         pandoc --from=markdown --to=rst --output=README.rst README.md
         python -c "import setup; print(setup.parse_description())"
     """
-    from os.path import dirname, join, exists
-
     readme_fpath = join(dirname(__file__), "README.rst")
     # This breaks on pip install, so check that it exists.
     if exists(readme_fpath):
         with open(readme_fpath, "r") as f:
             text = f.read()
         return text
     return ""
@@ -73,18 +72,18 @@
         fname (str): path to requirements file
         versions (bool | str, default=False):
             If true include version specs.
             If strict, then pin to the minimum version.
 
     Returns:
         List[str]: list of requirements items
-    """
-    from os.path import exists, dirname, join
-    import re
 
+    CommandLine:
+        python -c "import setup, ubelt; print(ubelt.urepr(setup.parse_requirements()))"
+    """
     require_fpath = fname
 
     def parse_line(line, dpath=""):
         """
         Parse information from a line in a requirements text file
 
         line = 'git+https://a.com/somedep@sometag#egg=SomeDep'
@@ -194,60 +193,69 @@
 #             raise KeyError(versions)
 #     requirements = [r.replace(' ', '') for r in requirements]
 #     return requirements
 
 
 NAME = "plottool_ibeis"
 INIT_PATH = "plottool_ibeis/__init__.py"
-VERSION = parse_version("plottool_ibeis/__init__.py")
+VERSION = parse_version(INIT_PATH)
 
 if __name__ == "__main__":
     setupkw = {}
 
-    setupkw["install_requires"] = parse_requirements("requirements/runtime.txt")
+    setupkw["install_requires"] = parse_requirements(
+        "requirements/runtime.txt", versions="loose"
+    )
     setupkw["extras_require"] = {
-        "all": parse_requirements("requirements.txt"),
-        "tests": parse_requirements("requirements/tests.txt"),
-        "optional": parse_requirements("requirements/optional.txt"),
-        "headless": parse_requirements("requirements/headless.txt"),
-        "graphics": parse_requirements("requirements/graphics.txt"),
-        # Strict versions
+        "all": parse_requirements("requirements.txt", versions="loose"),
+        "headless": parse_requirements("requirements/headless.txt", versions="loose"),
+        "graphics": parse_requirements("requirements/graphics.txt", versions="loose"),
+        "docs": parse_requirements("requirements/docs.txt", versions="loose"),
+        "optional": parse_requirements("requirements/optional.txt", versions="loose"),
+        "problematic": parse_requirements(
+            "requirements/problematic.txt", versions="loose"
+        ),
+        "runtime": parse_requirements("requirements/runtime.txt", versions="loose"),
+        "tests": parse_requirements("requirements/tests.txt", versions="loose"),
+        "all-strict": parse_requirements("requirements.txt", versions="strict"),
         "headless-strict": parse_requirements(
             "requirements/headless.txt", versions="strict"
         ),
         "graphics-strict": parse_requirements(
             "requirements/graphics.txt", versions="strict"
         ),
-        "all-strict": parse_requirements("requirements.txt", versions="strict"),
+        "docs-strict": parse_requirements("requirements/docs.txt", versions="strict"),
+        "optional-strict": parse_requirements(
+            "requirements/optional.txt", versions="strict"
+        ),
+        "problematic-strict": parse_requirements(
+            "requirements/problematic.txt", versions="strict"
+        ),
         "runtime-strict": parse_requirements(
             "requirements/runtime.txt", versions="strict"
         ),
         "tests-strict": parse_requirements("requirements/tests.txt", versions="strict"),
-        "optional-strict": parse_requirements(
-            "requirements/optional.txt", versions="strict"
-        ),
     }
-
     setupkw["name"] = NAME
     setupkw["version"] = VERSION
     setupkw["author"] = "Jon Crall"
     setupkw["author_email"] = "erotemic@gmail.com"
     setupkw["url"] = "https://github.com/Erotemic/plottool_ibeis"
-    setupkw["description"] = "Plottool - tools matplotlib computer vision plots"
+    setupkw["description"] = "Plottool - tools for matplotlib computer vision plots"
     setupkw["long_description"] = parse_description()
     setupkw["long_description_content_type"] = "text/x-rst"
     setupkw["license"] = "Apache 2"
     setupkw["packages"] = find_packages(".")
-    setupkw["python_requires"] = ">=3.7"
+    setupkw["python_requires"] = ">=3.8"
     setupkw["classifiers"] = [
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Utilities",
         "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ]
     setup(**setupkw)
```

