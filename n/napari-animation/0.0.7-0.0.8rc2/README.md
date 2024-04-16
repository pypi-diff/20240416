# Comparing `tmp/napari_animation-0.0.7.tar.gz` & `tmp/napari_animation-0.0.8rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_animation-0.0.7.tar", last modified: Thu May 25 14:47:35 2023, max compression
+gzip compressed data, was "napari_animation-0.0.8rc2.tar", last modified: Tue Apr 16 02:01:12 2024, max compression
```

## Comparing `napari_animation-0.0.7.tar` & `napari_animation-0.0.8rc2.tar`

### file list

```diff
@@ -1,67 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:35.666994 napari_animation-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:35.658994 napari_animation-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:35.658994 napari_animation-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-25 14:47:24.000000 napari_animation-0.0.7/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-25 14:47:24.000000 napari_animation-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-25 14:47:24.000000 napari_animation-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-25 14:47:24.000000 napari_animation-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-25 14:47:24.000000 napari_animation-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-25 14:47:35.666994 napari_animation-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-05-25 14:47:24.000000 napari_animation-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-25 14:47:24.000000 napari_animation-0.0.7/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:35.662994 napari_animation-0.0.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-25 14:47:24.000000 napari_animation-0.0.7/examples/animate2D.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-25 14:47:24.000000 napari_animation-0.0.7/examples/animate3D.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-25 14:47:24.000000 napari_animation-0.0.7/examples/animateMixed.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-25 14:47:24.000000 napari_animation-0.0.7/examples/ease_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-25 14:47:24.000000 napari_animation-0.0.7/examples/interactive_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-25 14:47:24.000000 napari_animation-0.0.7/examples/programmatic_notebook_example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:35.662994 napari_animation-0.0.7/napari_animation/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:35.662994 napari_animation-0.0.7/napari_animation/_qt/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_qt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:35.662994 napari_animation-0.0.7/napari_animation/_qt/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_qt/_tests/test_animation_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_qt/animation_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_qt/frame_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_qt/keyframelistcontrol_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_qt/keyframeslist_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_qt/savedialog_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:35.662994 napari_animation-0.0.7/napari_animation/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_tests/test_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_tests/test_easing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_tests/test_frame_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_tests/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/_tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-25 14:47:35.000000 napari_animation-0.0.7/napari_animation/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/easing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/frame_sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:35.666994 napari_animation-0.0.7/napari_animation/interpolation/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/interpolation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/interpolation/base_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/interpolation/interpolation_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/interpolation/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/interpolation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/interpolation/viewer_state_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/key_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-25 14:47:24.000000 napari_animation-0.0.7/napari_animation/viewer_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:35.662994 napari_animation-0.0.7/napari_animation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-25 14:47:35.000000 napari_animation-0.0.7/napari_animation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-25 14:47:35.000000 napari_animation-0.0.7/napari_animation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:47:35.000000 napari_animation-0.0.7/napari_animation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 14:47:35.000000 napari_animation-0.0.7/napari_animation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:47:35.000000 napari_animation-0.0.7/napari_animation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-25 14:47:35.000000 napari_animation-0.0.7/napari_animation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 14:47:35.000000 napari_animation-0.0.7/napari_animation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-25 14:47:24.000000 napari_animation-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-25 14:47:24.000000 napari_animation-0.0.7/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:47:35.666994 napari_animation-0.0.7/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   607232 2023-05-25 14:47:24.000000 napari_animation-0.0.7/resources/screenshot-animation-widget.png
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-25 14:47:35.666994 napari_animation-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-25 14:47:24.000000 napari_animation-0.0.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-25 14:47:24.000000 napari_animation-0.0.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:01:12.226538 napari_animation-0.0.8rc2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:01:12.206538 napari_animation-0.0.8rc2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:01:12.210538 napari_animation-0.0.8rc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/.github/workflows/deploy_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-04-16 02:01:12.226538 napari_animation-0.0.8rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:01:12.214538 napari_animation-0.0.8rc2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:01:12.214538 napari_animation-0.0.8rc2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:01:12.214538 napari_animation-0.0.8rc2/docs/_static/favicon/
+-rw-r--r--   0 runner    (1001) docker     (127)    36168 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/docs/_static/favicon/logo-noborder-180.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/docs/_static/favicon/logo-silhouette-192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/docs/_static/favicon/logo-silhouette-dark-light.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:01:12.214538 napari_animation-0.0.8rc2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/docs/_templates/navbar-project.html
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/docs/_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:01:12.214538 napari_animation-0.0.8rc2/docs/developers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/docs/developers/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/docs/gallery.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:01:12.214538 napari_animation-0.0.8rc2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   143476 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:01:12.214538 napari_animation-0.0.8rc2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/examples/animate2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/examples/animate3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/examples/animateMixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/examples/ease_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/examples/interactive_animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/examples/layer_planes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/examples/programmatic_notebook_example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:01:12.218538 napari_animation-0.0.8rc2/napari_animation/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:01:12.218538 napari_animation-0.0.8rc2/napari_animation/_qt/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/_qt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:01:12.218538 napari_animation-0.0.8rc2/napari_animation/_qt/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/_qt/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/_qt/_tests/test_animation_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/_qt/animation_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/_qt/frame_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/_qt/keyframelistcontrol_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/_qt/keyframeslist_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/_qt/savedialog_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:01:12.222538 napari_animation-0.0.8rc2/napari_animation/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/_tests/test_animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/_tests/test_easing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/_tests/test_frame_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/_tests/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/_tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-16 02:01:12.000000 napari_animation-0.0.8rc2/napari_animation/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/easing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/frame_sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:01:12.222538 napari_animation-0.0.8rc2/napari_animation/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/interpolation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/interpolation/base_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/interpolation/interpolation_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/interpolation/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/interpolation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/interpolation/viewer_state_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/key_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/napari_animation/viewer_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:01:12.222538 napari_animation-0.0.8rc2/napari_animation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-04-16 02:01:12.000000 napari_animation-0.0.8rc2/napari_animation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-16 02:01:12.000000 napari_animation-0.0.8rc2/napari_animation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 02:01:12.000000 napari_animation-0.0.8rc2/napari_animation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-16 02:01:12.000000 napari_animation-0.0.8rc2/napari_animation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 02:01:12.000000 napari_animation-0.0.8rc2/napari_animation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-16 02:01:12.000000 napari_animation-0.0.8rc2/napari_animation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-16 02:01:12.000000 napari_animation-0.0.8rc2/napari_animation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:01:12.222538 napari_animation-0.0.8rc2/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   607232 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/resources/screenshot-animation-widget.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-16 02:01:12.226538 napari_animation-0.0.8rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-16 02:01:03.000000 napari_animation-0.0.8rc2/tox.ini
```

### Comparing `napari_animation-0.0.7/.github/workflows/test_and_deploy.yml` & `napari_animation-0.0.8rc2/.github/workflows/test_and_deploy.yml`

 * *Files 7% similar despite different names*

```diff
@@ -10,47 +10,51 @@
     tags:
       - "v*" # Push events to matching v*, i.e. v1.0, v20.15.10
   pull_request:
     branches:
       - main
   workflow_dispatch:
 
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
+
 jobs:
   code:
     name: Code
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        task: [flake8, black, isort]
+        task: [black, ruff]
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v4
       - name: Set up Python 3.8
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: 3.8
       - name: Install dependencies
         run: |
           pip install --upgrade pip
           pip install tox
       - name: Run task
         run: tox -e ${{ matrix.task }}
   test:
     name: ${{ matrix.platform }} py${{ matrix.python-version }}
     runs-on: ${{ matrix.platform }}
     strategy:
       matrix:
         platform: [ ubuntu-latest, windows-latest, macos-latest ]
-        python-version: [ "3.8", "3.9", "3.10" ]
+        python-version: [ "3.8", "3.9", "3.10", "3.11" ]
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - uses: tlambert03/setup-qt-libs@v1
 
       # strategy borrowed from vispy for installing opengl libs on windows
       - name: Install Windows OpenGL
@@ -63,34 +67,34 @@
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install setuptools tox tox-gh-actions
 
       # this runs the platform-specific tests declared in tox.ini
       - name: Test with tox
-        uses: GabrielBB/xvfb-action@v1
+        uses: aganders3/headless-gui@v1
         with:
             run: tox
         env:
           PLATFORM: ${{ matrix.platform }}
 
       - name: Coverage
-        uses: codecov/codecov-action@v1
+        uses: codecov/codecov-action@v3
 
   deploy:
     # this will run when you have tagged a commit, starting with "v*"
     # and requires that you have put your twine API key in your 
     # github secrets (see readme for details)
     needs: [ test ]
     runs-on: ubuntu-latest
     if: contains(github.ref, 'tags')
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: "3.x"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -U setuptools setuptools_scm wheel twine
       - name: Build and publish
```

### Comparing `napari_animation-0.0.7/.gitignore` & `napari_animation-0.0.8rc2/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+*.swp
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
@@ -73,7 +74,17 @@
 .python-version
 
 # OS
 .DS_Store
 
 # written by setuptools_scm
 */_version.py
+
+# vscode
+.vscode
+
+# Autogenerated gallery
+docs/gallery
+docs/jupyter_execute
+docs/sg_execution_times.rst
+examples/*.mov
+examples/*.mp4
```

### Comparing `napari_animation-0.0.7/LICENSE` & `napari_animation-0.0.8rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.7/PKG-INFO` & `napari_animation-0.0.8rc2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,65 @@
-Metadata-Version: 2.1
-Name: napari_animation
-Version: 0.0.7
-Summary: A plugin for making animations in napari
-Home-page: https://github.com/napari/napari-animation
-Download-URL: https://github.com/napari/napari-animation
-Author: Nicholas Sofroniew, Alister Burt, Guillaume Witz, Faris Abouakil, Talley Lambert
-License: BSD 3-Clause
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Framework :: napari
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-Provides-Extra: dev
-License-File: LICENSE
-
 # napari-animation
 
 [![License](https://img.shields.io/pypi/l/napari-animation.svg?color=green)](https://github.com/napari/napari-animation/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-animation.svg?color=green)](https://pypi.org/project/napari-animation)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-animation.svg?color=green)](https://python.org)
 [![tests](https://github.com/napari/napari-animation/actions/workflows/test_and_deploy.yml/badge.svg)](https://github.com/napari/napari-animation/actions)
 [![codecov](https://codecov.io/gh/napari/napari-animation/branch/main/graph/badge.svg)](https://codecov.io/gh/napari/napari-animation)
 
-**napari-animation** is a plugin for making animations in [napari].
+**napari-animation** is a plugin for making animations in [napari](https://napari.org).
 
 <p align="center">
   <img width="500" src="https://user-images.githubusercontent.com/7307488/196110138-6c4663b1-67b2-4c79-97b7-57b706d1d49c.gif">
 </p>
 
 ----------------------------------
 
 [Merlin Lange](https://twitter.com/Merlin_Lange) used *napari-animation* to create one of [Nature's best science images for September 2022](https://www.nature.com/immersive/d41586-022-03051-6/index.html)
 
 ----------------------------------
 
-This plugin is built on [naparimovie](https://github.com/guiwitz/naparimovie) from @guiwitz. naparimovie was submitted to napari in [PR#851](https://github.com/napari/napari/pull/780) before napari plugin infrastructure existed.
+This plugin is built on [`naparimovie`](https://github.com/guiwitz/naparimovie) from [@guiwitz](https://github.com/guiwitz). `naparimovie` was submitted to napari in [PR#851](https://github.com/napari/napari/pull/780) before napari plugin infrastructure existed.
 
 ----------------------------------
+
 ## Overview
 
-**napari-animation** provides a framework for the creation of animations in napari, the plugin contains:
-- an easy to use GUI for creating animations interactively
-- a Python package for the programmatic creation of animations
+**napari-animation** provides a framework for the creation of animations in napari. The plugin contains:
+
+- an easy to use GUI for creating animations interactively;
+- a Python package for the programmatic creation of animations.
 
 This plugin remains under development and contributions are very welcome, please open an issue to discuss potential improvements.
 
+You can read the documentation at [https://napari.org/napari-animation](https://napari.org/napari-animation)
+
 ## Installation
 
 ### PyPI
 `napari-animation` is available through the Python package index and can be installed using `pip`.
 
 ```sh
 pip install napari-animation
 ```
 
+```{warning}
+`napari-animation` uses `ffmpeg` to export animations. If you are using a macOS arm64 computer (Apple Silicon e.g. M1, M2 processor)
+the PyPI package does not include the needed binary for your platform. You will need to install `ffmpeg` using
+`conda` from the [conda-forge channel](https://conda-forge.org/docs/#what-is-conda-forge) (`conda install -c conda-forge ffmpeg`)
+or using [`homebrew`](https://brew.sh) (`brew install ffmpeg`).
+```
+
+### Conda
+`napari-animation` is also available for install using `conda` through the [conda-forge channel](https://conda-forge.org/docs/#what-is-conda-forge).
+
+```sh
+conda install -c conda-forge napari-animation
+```
+
 ### Local
 You can clone this repository and install locally with
 
     pip install -e .
 
 ### Interactive use
 **napari-animation** can be used interactively.
@@ -80,16 +72,17 @@
 
 To activate the GUI, select **napari-animation: wizard** from the *plugins menu*
 
 <p align="center">
   <img width="200" src="https://user-images.githubusercontent.com/7307488/196114466-56cb5985-0d79-4cfa-96f1-38cf3ccfbc48.png">
 </p>
 
-### Headless
-**napari-animation** can also be run headless, allowing for reproducible, scripted creation of animations.
+### Scripting
+
+**napari-animation** can also be run programatically, allowing for reproducible, scripted creation of animations.
 
 ```python
 from napari_animation import Animation
 
 animation = Animation(viewer)
 
 viewer.dims.ndisplay = 3
@@ -104,44 +97,96 @@
 viewer.reset_view()
 viewer.camera.angles = (0.0, 0.0, 90.0)
 animation.capture_keyframe()
 animation.animate('demo.mov', canvas_only=False)
 ```
 
 ## Examples
-Examples can be found in our [examples](examples) folder. Simple examples for both interactive and headless 
+
+Examples can be found in our [Examples gallery](https://napari.org/napari-animation/gallery), generated from [our example scripts](https://github.com/napari/napari-animation/tree/main/examples). Simple examples for both interactive and headless
 use of the plugin follow.
 
 ## Contributing
 
-Contributions are very welcome and a detailed contributing guide is coming soon. 
+Contributions are very welcome and a detailed contributing guide is coming soon.
+In the meantime, clone this repository and install it in editable mode using `pip`:
+
+```
+pip install -e .
+```
+We recommend using a virtual environment, for example `conda`.
+
+
+```{important}
+Ensure you have a suitable Qt backend for napari! We recommend `PyQt5`.
+For more information, see the napari [Qt backend installation guide](https://napari.org/stable/tutorials/fundamentals/installation.html#choosing-a-different-qt-backend)
+```
+
+To set up your development installation, clone this repository, navigate to the clone folder, and install napari-animation in editable mode using `pip`.
+
+```sh
+conda create -n nap-anim python=3.10
+conda activate nap-anim
+pip install -e ".[dev]" PyQt5
+
+```
 
 Tests are run with `pytest`.
+You can make sure your `[dev]` installation is working properly by running
+`pytest .` from within the repository.
 
-We use [`pre-commit`](https://pre-commit.com) to sort imports with
-[`isort`](https://github.com/timothycrosley/isort), format code with
-[`black`](https://github.com/psf/black), and lint with
-[`flake8`](https://github.com/PyCQA/flake8) automatically prior to each commit.
+```{note}
+We use [`pre-commit`](https://pre-commit.com) to sort imports and lint with
+[`ruff`](https://github.com/astral-sh/ruff) and format code with
+[`black`](https://github.com/psf/black) automatically prior to each commit.
 To minmize test errors when submitting pull requests, please install `pre-commit`
 in your environment as follows:
 
+`pre-commit install`
+```
+
+## Documentation
+
+The documentation is available at [https://napari.org/napari-animation](https://napari.org/napari-animation)
+
+The documentation for napari-animation is built with [Sphinx](https://www.spinx-doc.org) and the [napari Sphinx Theme](https://github.com/napari/napari-sphinx-theme).
+
+### Building docs locally
+
+After installing the documentation dependencies with
+
 ```sh
-pre-commit install
+pip install ".[doc]"
 ```
 
+you can see a local version of the documentation by running
+
+```sh
+make docs
+```
+
+Open up the `docs/_build/index.html` file in your browser, and you'll see the home page of the docs being displayed.
+
+### Deploying docs
+
+The napari-animation documentation is automatically built and deployed to the website
+whenever the main branch is updated, or a new release is tagged.
+This is controlled by the [deploy_docs.yml](https://github.com/napari/napari-animation/blob/main/.github/workflows/deploy_docs.yml) github actions script.
+
+You can also manually trigger a documenation re-build and deployment [from the github actions tab](https://github.com/napari/napari-animation/actions/workflows/deploy_docs.yml).
+
 ## License
 
-Distributed under the terms of the [BSD-3] license,
-"napari-animation" is free and open source software
+Distributed under the terms of the [BSD-3 license](http://opensource.org/licenses/BSD-3-Clause),
+`napari-animation` is free and open source software.
 
 ## Issues
 
-If you encounter any problems, please [file an issue] along with a detailed description.
+If you encounter any problems, please [file an issue](https://github.com/napari/napari-animation/issues) along with a detailed description.
 
-[napari]: https://github.com/napari/napari
 [Cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
 [BSD-3]: http://opensource.org/licenses/BSD-3-Clause
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
 [file an issue]: https://github.com/sofroniewn/napari-animation/issues
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
```

### Comparing `napari_animation-0.0.7/examples/animate2D.py` & `napari_animation-0.0.8rc2/examples/animate2D.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 """
+Animate 2D
+==========
+
 Display a labels layer above of an image layer using the add_labels and
 add_image APIs
 """
 
 from skimage import data
 from scipy import ndimage as ndi
 from napari_animation import Animation
 import napari
 
 
 blobs = data.binary_blobs(length=128, volume_fraction=0.1, n_dim=3)
-viewer = napari.view_image(blobs.astype(float), name='blobs')
+viewer = napari.view_image(blobs.astype(float), name="blobs")
 labeled = ndi.label(blobs)[0]
-viewer.add_labels(labeled, name='blob ID')
+viewer.add_labels(labeled, name="blob ID")
 
 animation = Animation(viewer)
-viewer.update_console({'animation': animation})
+viewer.update_console({"animation": animation})
 
 animation.capture_keyframe()
 viewer.camera.zoom = 0.2
 animation.capture_keyframe()
 viewer.camera.zoom = 10.0
 viewer.camera.center = (0, 40.0, 10.0)
 animation.capture_keyframe()
 viewer.dims.current_step = (60, 0, 0)
 animation.capture_keyframe(steps=60)
 viewer.dims.current_step = (0, 0, 0)
 animation.capture_keyframe(steps=60)
 viewer.reset_view()
 animation.capture_keyframe()
-animation.animate('demo2D.mov', canvas_only=False)
-
+animation.animate("animate2D.mp4", canvas_only=False)
```

### Comparing `napari_animation-0.0.7/examples/animate3D.py` & `napari_animation-0.0.8rc2/examples/animateMixed.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,48 @@
 """
+Animate mixed
+=============
+
 Display a labels layer above of an image layer using the add_labels and
 add_image APIs
 """
 
 from skimage import data
 from scipy import ndimage as ndi
 from napari_animation import Animation
 import napari
 
 
 blobs = data.binary_blobs(length=128, volume_fraction=0.1, n_dim=3)
-viewer = napari.view_image(blobs.astype(float), name='blobs')
+viewer = napari.view_image(blobs.astype(float), name="blobs")
 labeled = ndi.label(blobs)[0]
-viewer.add_labels(labeled, name='blob ID')
+viewer.add_labels(labeled, name="blob ID")
 
 animation = Animation(viewer)
-viewer.update_console({'animation': animation})
+viewer.update_console({"animation": animation})
+
+animation.capture_keyframe()
+viewer.camera.zoom = 0.2
+animation.capture_keyframe()
+viewer.camera.zoom = 10.0
+viewer.camera.center = (0, 40.0, 10.0)
+animation.capture_keyframe()
+viewer.dims.current_step = (60, 0, 0)
+animation.capture_keyframe(steps=60)
+viewer.dims.current_step = (0, 0, 0)
+animation.capture_keyframe(steps=60)
+viewer.reset_view()
+animation.capture_keyframe()
 
 viewer.dims.ndisplay = 3
 viewer.camera.angles = (0.0, 0.0, 90.0)
 animation.capture_keyframe()
 viewer.camera.zoom = 2.4
 animation.capture_keyframe()
 viewer.camera.angles = (-7.0, 15.7, 62.4)
 animation.capture_keyframe(steps=60)
 viewer.camera.angles = (2.0, -24.4, -36.7)
 animation.capture_keyframe(steps=60)
 viewer.reset_view()
 viewer.camera.angles = (0.0, 0.0, 90.0)
 animation.capture_keyframe()
-animation.animate('demo3D.mov', canvas_only=False)
+animation.animate("animateMixed.mp4", canvas_only=False)
```

### Comparing `napari_animation-0.0.7/examples/programmatic_notebook_example.ipynb` & `napari_animation-0.0.8rc2/examples/programmatic_notebook_example.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Programmatic example'])]))]}"}*

```diff
@@ -1,10 +1,17 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Programmatic example"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import napari\n",
                 "from skimage import data\n",
```

### Comparing `napari_animation-0.0.7/napari_animation/_qt/_tests/test_animation_widget.py` & `napari_animation-0.0.8rc2/napari_animation/_qt/_tests/test_animation_widget.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.7/napari_animation/_qt/animation_widget.py` & `napari_animation-0.0.8rc2/napari_animation/_qt/animation_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
     QErrorMessage,
     QPushButton,
     QSlider,
     QVBoxLayout,
     QWidget,
 )
 
-from ..animation import Animation
+from napari_animation.animation import Animation
+
 from .frame_widget import FrameWidget
 from .keyframelistcontrol_widget import KeyFrameListControlWidget
 from .keyframeslist_widget import KeyFramesListWidget
 from .savedialog_widget import SaveDialogWidget
 
 
 class AnimationWidget(QWidget):
@@ -148,15 +149,14 @@
     def _on_slider_moved(self, event=None):
         frame_index = event
         if frame_index < len(self.animation._frames):
             with self.animation.key_frames.selection.events.active.blocker():
                 self.animation.set_movie_frame_index(frame_index)
 
     def _save_callback(self, event=None):
-
         saveDialogWidget = SaveDialogWidget(self)
         animation_kwargs = saveDialogWidget.getAnimationParameters(
             self, "Save animation", str(Path.home())
         )
 
         if animation_kwargs.get("filename", None) is not None:
             try:
```

### Comparing `napari_animation-0.0.7/napari_animation/_qt/frame_widget.py` & `napari_animation-0.0.8rc2/napari_animation/_qt/frame_widget.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.7/napari_animation/_qt/keyframelistcontrol_widget.py` & `napari_animation-0.0.8rc2/napari_animation/_qt/keyframelistcontrol_widget.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.7/napari_animation/_qt/keyframeslist_widget.py` & `napari_animation-0.0.8rc2/napari_animation/_qt/keyframeslist_widget.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.7/napari_animation/_qt/savedialog_widget.py` & `napari_animation-0.0.8rc2/napari_animation/_qt/savedialog_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,20 +31,20 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def getAnimationParameters(
         self,
         parent=None,
         caption="Select a file :",
-        dir=".",
+        directory=".",
         options=None,
     ):
         # Set dialog parameters
         self.setWindowTitle(caption)
-        self.setDirectory(dir)
+        self.setDirectory(directory)
         self.setNameFilter(self._qt_file_name_filters)
         self.setFileMode(QFileDialog.AnyFile)
         self.setAcceptMode(QFileDialog.AcceptSave)
 
         if options is not None:
             self.setOptions(options)
 
@@ -61,17 +61,18 @@
             animation_kwargs = {
                 "filename": self.get_file_path(),
                 "fps": self.optionsWidget.fpsSpinBox.value(),
                 "quality": int(self.optionsWidget.qualitySlider.value()),
                 "canvas_only": self.optionsWidget.canvasCheckBox.isChecked(),
                 "scale_factor": self.optionsWidget.scaleSpinBox.value(),
             }
-            return animation_kwargs
         else:
-            return ""
+            animation_kwargs = {}
+
+        return animation_kwargs
 
     def get_file_path(self) -> Path:
         provided_file_name = Path(list(self.selectedFiles())[0])
         if provided_file_name.suffix not in self._valid_file_extensions:
             extension_in_gui = self.qt_filter_to_extension(
                 self.selectedNameFilter()
             )
```

### Comparing `napari_animation-0.0.7/napari_animation/_tests/conftest.py` & `napari_animation-0.0.8rc2/napari_animation/_tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     viewer = make_napari_viewer()
     animation = Animation(viewer)
     return animation
 
 
 @pytest.fixture
 def animation_with_key_frames(empty_animation):
-    for i in range(2):
+    for _i in range(2):
         empty_animation.capture_keyframe()
         empty_animation.viewer.camera.zoom *= 2
     return empty_animation
 
 
 @pytest.fixture
 def viewer_state(empty_animation):
@@ -38,15 +38,15 @@
 def frame_sequence(animation_with_key_frames):
     return animation_with_key_frames._frames
 
 
 @pytest.fixture
 def image_animation(make_napari_viewer):
     viewer = make_napari_viewer()
-    viewer.add_image(np.random.random((28, 28)))
+    viewer.add_image(np.random.random((2, 28, 28)))
     return Animation(viewer)
 
 
 @pytest.fixture
 def layer_state(image_animation: Animation):
     image_animation.capture_keyframe()
     return image_animation.key_frames[0].viewer_state.layers
```

### Comparing `napari_animation-0.0.7/napari_animation/_tests/test_animation.py` & `napari_animation-0.0.8rc2/napari_animation/_tests/test_animation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 from unittest.mock import patch
 
 import numpy as np
 import pytest
+from napari._tests.utils import (
+    add_layer_by_type,
+    assert_layer_state_equal,
+    layer_test_data,
+)
 
 from napari_animation import Animation, ViewerState
 from napari_animation.utils import make_thumbnail
 
-CAPTURED_LAYER_ATTRIBUTES = [
+CAPTURED_IMAGE_LAYER_ATTRIBUTES = [
     "name",
     "scale",
     "translate",
     "rotate",
     "shear",
     "opacity",
     "blending",
     "visible",
 ]
 
+NOT_CAPTURED_LAYER_ATTRIBUTES = [
+    "metadata",
+    "data",
+]
+
 
 def test_animation(make_napari_viewer):
     """Test creation of an animation class."""
     viewer = make_napari_viewer()
     animation = Animation(viewer)
     assert animation is not None
 
@@ -65,15 +75,15 @@
     current_state = ViewerState.from_viewer(animation.viewer)
     viewer_state.apply(animation.viewer)
 
     animation_dims_state = animation.viewer.dims.dict()
     animation_camera_state = animation.viewer.camera.dict()
 
     assert animation_dims_state == current_state.dims
-    for key in ("center", "angles", "interactive"):
+    for key in ("center", "angles", "mouse_pan", "mouse_zoom"):
         assert animation_camera_state[key] == current_state.camera[key]
 
 
 def test_thumbnail_generation(empty_animation):
     """Test thumbnail generation"""
     animation = empty_animation
     shape = (32, 32, 4)
@@ -89,22 +99,22 @@
 
 @patch("napari_animation.animation.imsave")
 @patch("imageio.get_writer")
 @patch(
     "napari_animation.frame_sequence.FrameSequence.iter_frames",
     return_value=["frame"] * 30,
 )
-@pytest.mark.parametrize("ext", [".mp4", ".mov", ""])
+@pytest.mark.parametrize("ext", [".mp4", ".mov", ".gif", ""])
 def test_animate_filenames(
     frame_gen, get_writer, imsave, animation_with_key_frames, ext, tmp_path
 ):
     """Test that Animation.animate() produces files with correct filenames"""
     output_filename = tmp_path / f"test{ext}"
     animation_with_key_frames.animate(output_filename)
-    if ext in (".mp4", ".mov"):
+    if ext in (".mp4", ".mov", ".gif"):
         expected_filename = output_filename
         saved_filename = get_writer.call_args[0][0]
         assert saved_filename == expected_filename
     elif ext == "":
         expected = [output_filename / f"test_{i:06d}.png" for i in range(30)]
         saved_files = [call[0][0] for call in imsave.call_args_list]
         assert saved_files == expected
@@ -121,21 +131,69 @@
     # title="napari version 0.4.17 https://napari.org/"
     with open(output_filename, "rb") as f:
         content = f.read()
     assert b"napari version" in content
     assert b"https://napari.org" in content
 
 
-@pytest.mark.parametrize("attribute", CAPTURED_LAYER_ATTRIBUTES)
+@pytest.mark.parametrize("attribute", CAPTURED_IMAGE_LAYER_ATTRIBUTES)
 def test_layer_attribute_capture(layer_state, attribute):
     """Test that 'attribute' is captured in the layer state dictionary"""
     for layer_state_dict in layer_state.values():
-        assert attribute in layer_state_dict.keys()
+        assert attribute in layer_state_dict
 
 
 def test_end_state_reached(image_animation):
     """Check that animation ends in the same state as the final key-frame"""
     image_animation.capture_keyframe()
     image_animation.viewer.dims.current_step = (28, 0)
     image_animation.capture_keyframe(steps=2)
     last_state = image_animation._frames[-1]
     assert last_state == image_animation.key_frames[-1].viewer_state
+
+
+def test_ndisplay_interpolation(image_animation):
+    """Check that dims.ndisplay interpolation is boolean"""
+    image_animation.capture_keyframe()
+    image_animation.viewer.dims.ndisplay = 3
+    image_animation.capture_keyframe(steps=3)
+    assert image_animation._frames[0].dims["ndisplay"] == 2
+    assert image_animation._frames[1].dims["ndisplay"] == 3
+    assert image_animation._frames[-1].dims["ndisplay"] == 3
+
+
+@pytest.mark.parametrize("layer_class, data, ndim", layer_test_data)
+def test_attributes_for_all_layer_types(
+    make_napari_viewer, layer_class, data, ndim
+):
+    """Test that attributes are in the viewer_state for all napari layer types"""
+    viewer = make_napari_viewer()
+    add_layer_by_type(viewer, layer_class, data, visible=True)
+    layer_animation = Animation(viewer)
+    # get the state of the layer
+    layer_state = viewer.layers[0]._get_state()
+    # remove attributes that are not captured
+    for key in NOT_CAPTURED_LAYER_ATTRIBUTES:
+        layer_state.pop(key)
+
+    layer_animation.capture_keyframe()
+    # get the layer attributes captured to viewer_state
+    animation_state = layer_animation.key_frames[0].viewer_state.layers[
+        viewer.layers[0].name
+    ]
+
+    assert_layer_state_equal(animation_state, layer_state)
+
+
+@pytest.mark.parametrize("layer_class, data, ndim", layer_test_data)
+def test_animating_all_layer_types(
+    make_napari_viewer, layer_class, data, ndim
+):
+    """Test that all napari layer types can be animated"""
+    viewer = make_napari_viewer()
+    add_layer_by_type(viewer, layer_class, data, visible=True)
+    layer_animation = Animation(viewer)
+    layer_animation.capture_keyframe()
+    layer_animation.viewer.camera.zoom *= 2
+    layer_animation.capture_keyframe()
+    # advance the movie frame, simulating slider movement
+    layer_animation.set_movie_frame_index(1)
```

### Comparing `napari_animation-0.0.7/napari_animation/_tests/test_easing.py` & `napari_animation-0.0.8rc2/napari_animation/_tests/test_easing.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.7/napari_animation/_tests/test_frame_sequence.py` & `napari_animation-0.0.8rc2/napari_animation/_tests/test_frame_sequence.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.7/napari_animation/_tests/test_interpolation.py` & `napari_animation-0.0.8rc2/napari_animation/_tests/test_interpolation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import numbers
 from dataclasses import asdict
 from typing import NamedTuple
 
 import numpy as np
 import pytest
 
 from napari_animation.interpolation import interpolate_viewer_state
@@ -10,25 +11,37 @@
     interpolate_log,
     interpolate_num,
     interpolate_sequence,
 )
 from napari_animation.interpolation.utils import nested_assert_close
 
 
+def _expected_type(a, b):
+    if isinstance(a, numbers.Integral) and isinstance(b, numbers.Real):
+        return type(b)
+    return type(a)
+
+
 # Actual tests
-@pytest.mark.parametrize("a", [0.0, 0])
-@pytest.mark.parametrize("b", [100.0, 100])
+@pytest.mark.parametrize("a", [0.0, 0, np.float32(0)])
+@pytest.mark.parametrize("b", [100.0, 100, np.float32(100)])
 @pytest.mark.parametrize("fraction", [0, 0.0, 0.5, 1.0, 1])
 def test_interpolate_num(a, b, fraction):
     """Check that interpolation of numbers produces valid output"""
     result = interpolate_num(a, b, fraction)
-    assert isinstance(result, type(a))
+    assert isinstance(result, _expected_type(a, b))
     assert result == fraction * b
 
 
+@pytest.mark.parametrize("b", [1.0, np.float32(1)])
+def test_interpolate_proper_type(b):
+    result = interpolate_num(0, b, 0.5)
+    assert np.isclose(result, 0.5)
+
+
 @pytest.mark.parametrize("a,b", [([0.0, 0.0, 0.0], [1.0, 1.0, 1.0])])
 @pytest.mark.parametrize(
     "fraction,expected",
     [(0.0, [0.0, 0.0, 0.0]), (0.5, [0.5, 0.5, 0.5]), (1.0, [1.0, 1.0, 1.0])],
 )
 def test_interpolate_seq(a, b, fraction, expected):
     """Check that interpolation of sequences produces valid output"""
```

### Comparing `napari_animation-0.0.7/napari_animation/_tests/test_utils.py` & `napari_animation-0.0.8rc2/napari_animation/_tests/test_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import pytest
 
 from ..interpolation.utils import keys_to_list, nested_get
 
 input_dict = [{"a": 1, "b": {"c": "d"}}]
 keys = [["b", "c"]]
 expected = ["d"]
-test_set = [param for param in zip(input_dict, keys, expected)]
+test_set = list(zip(input_dict, keys, expected))
 
 
 @pytest.mark.parametrize("input_dict,keys,expected", test_set)
 def test_nested_get(input_dict, keys, expected):
     result = nested_get(input_dict, keys)
     assert result == expected
 
 
 input_dict = [{"a": 1, "b": {"c": "d"}, "e": {}}]
 expected = [[["a"], ["b", "c"], ["e"]]]
-test_set = [param for param in zip(input_dict, expected)]
+test_set = list(zip(input_dict, expected))
 
 
 @pytest.mark.parametrize("input_dict,expected", test_set)
 def test_keys_to_list(input_dict, expected):
-    result = [keys for keys in keys_to_list(input_dict)]
+    result = list(keys_to_list(input_dict))
     for keys in result:
         assert isinstance(keys, list)
     assert result == expected
```

### Comparing `napari_animation-0.0.7/napari_animation/animation.py` & `napari_animation-0.0.8rc2/napari_animation/animation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 import os
 from itertools import count
 from pathlib import Path
 from time import sleep
 
 import imageio
 import numpy as np
-from napari._version import __version__ as napari_version
 from napari.utils.io import imsave
 from tqdm import tqdm
 
 from napari_animation.easing import Easing
 
 from .frame_sequence import FrameSequence
 from .key_frame import KeyFrame, KeyFrameList
 
+try:
+    from importlib.metadata import version
+except ImportError:
+    try:
+        from importlib_metadata import version
+    except ImportError:
+
+        def version(_=None):
+            return "<0.4.15"
+
+
+napari_version = version("napari")
+
 
 class Animation:
     """Make animations using the napari viewer.
 
     Parameters
     ----------
     viewer : napari.Viewer
@@ -126,15 +138,15 @@
             return
 
     def animate(
         self,
         filename,
         fps=20,
         quality=5,
-        format=None,
+        file_format=None,
         canvas_only=True,
         scale_factor=None,
     ):
         """Create a movie based on key-frames
         Parameters
         -------
         filename : str
@@ -142,23 +154,23 @@
             should be one of .gif, .mp4, .mov, .avi, .mpg, .mpeg, .mkv, .wmv
             If no extension is provided, images are saved as a folder of PNGs
         fps : int
             frames per second
         quality: float
             number from 1 (lowest quality) to 9
             only applies to non-gif extensions
-        format: str
+        file_format: str
             The format to use to write the file. By default imageio selects the appropriate
             for you based on the filename.
         canvas_only : bool
             If True include just includes the canvas, otherwise include the full napari
             viewer.
         scale_factor : float
             Rescaling factor for the image size. Only used without
-            viewer (with_viewer = False).
+            viewer (canvas_only = True).
         """
         self._validate_animation()
 
         description = f"napari version {napari_version} https://napari.org/"
         output_params = ["-metadata", f'title="{description}"']
 
         # create path object
@@ -170,14 +182,15 @@
         save_as_folder = False
         if file_path.suffix == "":
             save_as_folder = True
 
         # try to create an ffmpeg writer. If not installed default to folder creation
         if save_as_folder is False:
             try:
+                duration = 1000 / fps
                 # create imageio writer. Handle separately imageio-ffmpeg extensions and
                 # gif extension which doesn't accept the quality parameter.
                 if file_path.suffix in [
                     ".mov",
                     ".avi",
                     ".mpg",
                     ".mpeg",
@@ -185,23 +198,22 @@
                     ".mkv",
                     ".wmv",
                 ]:
                     writer = imageio.get_writer(
                         filename,
                         fps=fps,
                         quality=quality,
-                        format=format,
+                        format=file_format,
                         output_params=output_params,
                     )
                 else:
                     writer = imageio.get_writer(
                         filename,
-                        fps=fps,
-                        format=format,
-                        output_params=output_params,
+                        duration=duration,
+                        format=file_format,
                     )
             except ValueError as err:
                 print(err)
                 print("Your file will be saved as a series of PNG files")
                 save_as_folder = True
 
         if save_as_folder:
@@ -253,11 +265,13 @@
         active_keyframe = event.value
         if active_keyframe:
             keyframe_index = self.key_frames.index(active_keyframe)
             self.set_key_frame_index(keyframe_index)
 
     def _repr_html_(self):
         if self._filename is None:
-            return 'Video animation not yet available (use the "animate" method to generate it).'
+            html = 'Video animation not yet available (use the "animate" method to generate it).'
+        elif str(self._filename).endswith(".gif"):
+            html = f'<img src="{self._filename}">'
         else:
             html = f'<video width="100%" height="100%" controls> <source src="{self._filename}"> </video>'
-            return html
+        return html
```

### Comparing `napari_animation-0.0.7/napari_animation/easing.py` & `napari_animation-0.0.8rc2/napari_animation/easing.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.7/napari_animation/frame_sequence.py` & `napari_animation-0.0.8rc2/napari_animation/frame_sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
         self.events = EmitterGroup(
             source=self, n_frames=None, _current_index=None
         )
 
         self.state_interpolation_map: InterpolationMap = {
             "camera.angles": Interpolation.SLERP,
             "camera.zoom": Interpolation.LOG,
+            "dims.ndisplay": Interpolation.BOOL,
         }
 
         # cache of interpolated viewer states
         self._cache: Dict[int, ViewerState] = LRUDict(cache_size=cache_size)
 
         # map of frame number -> (kf0, kf1, fraction)
         self._keyframe_index: Dict[int, Tuple[KeyFrame, KeyFrame, float]] = {}
@@ -121,18 +122,18 @@
         """Get the interpolated state at frame `key` in the animation."""
         if key < 0:
             key += len(self)
 
         if key not in self._cache:
             try:
                 kf0, kf1, frac = self._keyframe_index[key]
-            except KeyError:
+            except KeyError as err:
                 raise IndexError(
                     f"Frame index ({key}) out of range ({len(self)} frames)"
-                )
+                ) from err
             if frac == 0:
                 self._cache[key] = kf0.viewer_state
             else:
                 self._cache[key] = interpolate_viewer_state(
                     kf0.viewer_state,
                     kf1.viewer_state,
                     frac,
@@ -144,15 +145,15 @@
     def iter_frames(
         self,
         viewer: napari.viewer.Viewer,
         canvas_only: bool = True,
         scale_factor: float = None,
     ) -> Iterator[np.ndarray]:
         """Iterate over interpolated viewer states, and yield rendered frames."""
-        for i, state in enumerate(self):
+        for _i, state in enumerate(self):
             frame = state.render(viewer, canvas_only=canvas_only)
             if scale_factor not in (None, 1):
                 from scipy import ndimage as ndi
 
                 frame = ndi.zoom(frame, (scale_factor, scale_factor, 1))
                 frame = frame.astype(np.uint8)
             yield frame
```

### Comparing `napari_animation-0.0.7/napari_animation/interpolation/base_interpolation.py` & `napari_animation-0.0.8rc2/napari_animation/interpolation/base_interpolation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from numbers import Number
+from numbers import Integral, Number, Real
 from typing import Sequence, Tuple, TypeVar
 
 import numpy as np
 from scipy.spatial.transform import Rotation as R
 
 _T = TypeVar("_T")
 
@@ -81,14 +81,16 @@
 
     Returns
     ----------
         : numeric type
     Interpolated value between a and b at fraction.
     """
     number_cls = type(a)
+    if isinstance(b, Real) and isinstance(a, Integral):
+        number_cls = type(b)
     return number_cls(a + (b - a) * fraction)
 
 
 def interpolate_bool(a: bool, b: bool, fraction: float) -> bool:
     """Instantaneous transition from a to b.
 
     Parameters
```

### Comparing `napari_animation-0.0.7/napari_animation/interpolation/interpolation_constants.py` & `napari_animation-0.0.8rc2/napari_animation/interpolation/interpolation_constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from enum import Enum
 from functools import partial
 
 from .base_interpolation import default_interpolation as _default_interpolation
+from .base_interpolation import interpolate_bool as _interpolate_bool
 from .base_interpolation import interpolate_log as _interpolate_log
 from .base_interpolation import slerp as _slerp
 
 
 class Interpolation(Enum):
     """Interpolation: interpolation function to use for a transition.
 
     Selects a preset interpolation function
         * DEFAULT: linear interpolation between start and endpoint.
         * SLERP: spherical linear interpolation on Euler angles.
         * LOG: log interpolation between start and endpoint.
+        * BOOL: boolean interpolation between start and endpoint.
 
     """
 
     DEFAULT = partial(_default_interpolation)
     LOG = partial(_interpolate_log)
     SLERP = partial(_slerp)
+    BOOL = partial(_interpolate_bool)
 
     def __call__(self, *args):
         return self.value(*args)
```

### Comparing `napari_animation-0.0.7/napari_animation/interpolation/utils.py` & `napari_animation-0.0.8rc2/napari_animation/interpolation/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,16 +63,16 @@
                 yield [key] + sub_key
         else:
             yield [key]
 
 
 def nested_assert_close(a, b):
     """Assert close on nested dicts."""
-    a_keys = [key for key in keys_to_list(a)]
-    b_keys = [key for key in keys_to_list(b)]
+    a_keys = list(keys_to_list(a))
+    b_keys = list(keys_to_list(b))
 
     assert a_keys == b_keys
 
     for key in a_keys:
         a_1 = nested_get(a, key)
         b_1 = nested_get(b, key)
```

### Comparing `napari_animation-0.0.7/napari_animation/interpolation/viewer_state_interpolation.py` & `napari_animation-0.0.8rc2/napari_animation/interpolation/viewer_state_interpolation.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     initial_state = asdict(initial_state)
     final_state = asdict(final_state)
 
     for keys in keys_to_list(initial_state):
         v0 = nested_get(initial_state, keys)
         v1 = nested_get(final_state, keys)
 
-        all_keys_are_strings = all([isinstance(key, str) for key in keys])
+        all_keys_are_strings = all(isinstance(key, str) for key in keys)
         if interpolation_map is not None and all_keys_are_strings:
             attribute_name = ".".join(keys)
             interpolation_function = interpolation_map.get(
                 attribute_name, Interpolation.DEFAULT
             )
         else:
             interpolation_function = Interpolation.DEFAULT
```

### Comparing `napari_animation-0.0.7/napari_animation/key_frame.py` & `napari_animation-0.0.8rc2/napari_animation/key_frame.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.7/napari_animation/viewer_state.py` & `napari_animation-0.0.8rc2/napari_animation/viewer_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+import contextlib
 from dataclasses import dataclass
 
 import napari
 import numpy as np
 
+from napari_animation.utils import layer_attribute_changed
+
 
 @dataclass(frozen=True)
 class ViewerState:
     """The state of the viewer camera, dims, and layers.
 
     Parameters
     ----------
@@ -28,15 +31,15 @@
         """Create a ViewerState from a viewer instance."""
         layers = {
             layer.name: layer.as_layer_data_tuple()[1]
             for layer in viewer.layers
         }
         for layer_attributes in layers.values():
             layer_attributes.pop("metadata")
-            layer_attributes.pop("properties", None)
+
         return cls(
             camera=viewer.camera.dict(), dims=viewer.dims.dict(), layers=layers
         )
 
     def apply(self, viewer: napari.viewer.Viewer):
         """Update `viewer` to match this ViewerState.
 
@@ -50,17 +53,19 @@
         viewer.dims.update(self.dims)
 
         for layer_name, layer_state in self.layers.items():
             layer = viewer.layers[layer_name]
             layer_attributes = layer.as_layer_data_tuple()[1]
             for attribute_name, value in layer_state.items():
                 original_value = layer_attributes[attribute_name]
-                # Only set if value differs to avoid expensive redraws
-                if not np.array_equal(original_value, value):
-                    setattr(layer, attribute_name, value)
+                # Only setattr if value has changed to avoid expensive redraws
+                # dicts can hold arrays, e.g. `color`, requiring comparisons of key/value pairs
+                if layer_attribute_changed(value, original_value):
+                    with contextlib.suppress(AttributeError):
+                        setattr(layer, attribute_name, value)
 
     def render(
         self, viewer: napari.viewer.Viewer, canvas_only: bool = True
     ) -> np.ndarray:
         """Render this ViewerState to an image.
 
         Parameters
```

### Comparing `napari_animation-0.0.7/resources/screenshot-animation-widget.png` & `napari_animation-0.0.8rc2/resources/screenshot-animation-widget.png`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.7/setup.cfg` & `napari_animation-0.0.8rc2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-name = napari_animation
+name = napari-animation
 url = https://github.com/napari/napari-animation
 download_url = https://github.com/napari/napari-animation
 license = BSD 3-Clause
 license_file = LICENSE
 description = A plugin for making animations in napari
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -26,54 +26,54 @@
 zip_safe = False
 packages = find:
 python_requires = >=3.8
 include_package_data = True
 install_requires = 
 	imageio
 	imageio-ffmpeg
-	napari
+	napari>=0.4.19rc5
 	npe2
 	numpy
 	qtpy
 	scipy
 	tqdm>=4.56.0
 	superqt
 
 [options.extras_require]
 testing = 
 	pytest
+	pytest-cov
 	pytest-qt
+	lxml_html_clean
+doc = 
+	sphinx>6
+	sphinx-autobuild
+	sphinx-external-toc
+	sphinx-copybutton
+	sphinx-gallery
+	sphinx-favicon
+	sphinxcontrib-video
+	matplotlib
+	myst-nb
+	napari-sphinx-theme>=0.3.0
 dev = 
 	pre-commit
 	black
-	flake8
-	isort
+	ruff
 	check-manifest
-	PyQt5>=5.12.3,!=5.15.0
 	%(testing)s
+	%(doc)s
 
 [options.entry_points]
 napari.manifest = 
 	napari-animation = napari_animation:napari.yaml
 
 [options.package_data]
 napari-animation = napari.yaml
 
-[isort]
-profile = black
-line_length = 79
-skip_glob = examples/
-multi_line_output = 3
-
-[flake8]
-ignore = E203,W503,E501,C901
-max-line-length = 79
-max-complexity = 18
-exclude = __init__.py,examples
-
 [coverage:report]
 exclude_lines = 
 	pragma: no cover
 	if TYPE_CHECKING:
 	raise NotImplementedError()
 
 [tool:pytest]
```

### Comparing `napari_animation-0.0.7/tox.ini` & `napari_animation-0.0.8rc2/tox.ini`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # For more information about tox, see https://tox.readthedocs.io/en/latest/
 [tox]
-envlist = py{38,39,310}-{linux,macos,windows}-{pyqt,pyside}
+envlist = py{38,39,310,311}-{linux,macos,windows}-pyqt, py{38,39,310}-{linux,macos,windows}-pyside
 
 [gh-actions]
 python =
     3.8: py38
     3.9: py39
     3.10: py310
+    3.11: py311
     
 [gh-actions:env]
 PLATFORM =
     ubuntu-latest: linux
     macos-latest: macos
     windows-latest: windows
 
@@ -22,37 +23,34 @@
 passenv = 
     CI
     GITHUB_ACTIONS
     DISPLAY
     XAUTHORITY
     NUMPY_EXPERIMENTAL_ARRAY_FUNCTION
     PYVISTA_OFF_SCREEN
-conda_deps =
-    # use conda to install numcodecs on mac py3.9
-    py39-macos: numcodecs
-conda_channels =
-    conda-forge
 deps = 
     pytest  # https://docs.pytest.org/en/latest/contents.html
     pytest-cov  # https://pytest-cov.readthedocs.io/en/latest/
     pytest-qt  # https://pytest-qt.readthedocs.io/en/latest/intro.html
     pytest-xvfb ; sys_platform == 'linux'
-    pyqt: napari[pyqt5,testing]
-    pyside: napari[pyside2,testing]
 commands = pytest -v --color=yes --cov=napari_animation --cov-report=xml
 
-[testenv:isort]
-skip_install = True
-deps = pre-commit
-commands = pre-commit run isort --all-files
-
+[testenv:py{38,39,310,311}-{linux,macos,windows}-pyqt]
+deps =
+    napari[pyqt5,testing]
+    lxml_html_clean # should only be needed till napari 0.5.0
+
+[testenv:py{38,39,310}-{linux,macos,windows}-pyside]
+deps =
+    napari[pyside2,testing]
+    lxml_html_clean # should only be needed till napari 0.5.0
 
-[testenv:flake8]
+[testenv:ruff]
 skip_install = True
 deps = pre-commit
-commands = pre-commit run flake8 --all-files
+commands = pre-commit run ruff --all-files
 
 
 [testenv:black]
 skip_install = True
 deps = pre-commit
 commands = pre-commit run black --all-files
```

