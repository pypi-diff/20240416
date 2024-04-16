# Comparing `tmp/plopp-24.2.0.tar.gz` & `tmp/plopp-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plopp-24.2.0.tar", last modified: Mon Feb 19 10:31:25 2024, max compression
+gzip compressed data, was "plopp-24.4.0.tar", last modified: Tue Apr 16 14:08:48 2024, max compression
```

## Comparing `plopp-24.2.0.tar` & `plopp-24.4.0.tar`

### file list

```diff
@@ -1,261 +1,277 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.990068 plopp-24.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-19 10:31:14.000000 plopp-24.2.0/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.954068 plopp-24.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-02-19 10:31:14.000000 plopp-24.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.954068 plopp-24.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-02-19 10:31:14.000000 plopp-24.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-02-19 10:31:14.000000 plopp-24.2.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-02-19 10:31:14.000000 plopp-24.2.0/.github/workflows/nightly_at_main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-02-19 10:31:14.000000 plopp-24.2.0/.github/workflows/nightly_at_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-19 10:31:14.000000 plopp-24.2.0/.github/workflows/python-version-ci
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-02-19 10:31:14.000000 plopp-24.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-02-19 10:31:14.000000 plopp-24.2.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-02-19 10:31:14.000000 plopp-24.2.0/.github/workflows/unpinned.yml
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-02-19 10:31:14.000000 plopp-24.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-19 10:31:14.000000 plopp-24.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-02-19 10:31:14.000000 plopp-24.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-02-19 10:31:14.000000 plopp-24.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-02-19 10:31:14.000000 plopp-24.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-19 10:31:14.000000 plopp-24.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-02-19 10:31:25.990068 plopp-24.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-19 10:31:14.000000 plopp-24.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.954068 plopp-24.2.0/conda/
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-02-19 10:31:14.000000 plopp-24.2.0/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.958068 plopp-24.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.958068 plopp-24.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_static/anaconda-icon.js
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_static/circle-exclamation.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.958068 plopp-24.2.0/docs/_static/customization/
--rw-r--r--   0 runner    (1001) docker     (127)   114427 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_static/customization/custom-interfaces.png
--rw-r--r--   0 runner    (1001) docker     (127)    44133 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_static/customization/graph-node-tips.png
--rw-r--r--   0 runner    (1001) docker     (127)    54880 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_static/customization/subplots.png
--rw-r--r--   0 runner    (1001) docker     (127)    19228 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_static/customization/tweaking-figures.png
--rw-r--r--   0 runner    (1001) docker     (127)   137750 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.958068 plopp-24.2.0/docs/_static/gallery/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_static/gallery/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)   211913 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_static/gallery/peeling-layers-thumbnail.png
--rw-r--r--   0 runner    (1001) docker     (127)    18766 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_static/gallery/scatter3d-with-slider-thumbnail.png
--rw-r--r--   0 runner    (1001) docker     (127)    66718 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_static/gallery/scatter3d-with-threshold-thumbnail.png
--rw-r--r--   0 runner    (1001) docker     (127)    76311 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_static/logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    76253 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.962068 plopp-24.2.0/docs/_static/plot-types/
--rw-r--r--   0 runner    (1001) docker     (127)    37065 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_static/plot-types/image-plot.png
--rw-r--r--   0 runner    (1001) docker     (127)    47635 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_static/plot-types/inspector-plot.png
--rw-r--r--   0 runner    (1001) docker     (127)    15510 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_static/plot-types/line-plot.png
--rw-r--r--   0 runner    (1001) docker     (127)   186659 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_static/plot-types/scatter3d-plot.png
--rw-r--r--   0 runner    (1001) docker     (127)    55181 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_static/plot-types/slicer-plot.png
--rw-r--r--   0 runner    (1001) docker     (127)    50020 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_static/plot-types/super-plot.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.962068 plopp-24.2.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_templates/class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_templates/doc_version.html
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_templates/module-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_templates/scipp-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_templates/scipp-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/_typehints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.962068 plopp-24.2.0/docs/about/
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/about/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.962068 plopp-24.2.0/docs/api-reference/
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/api-reference/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/api-reference/matplotlib.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/api-reference/plotly.md
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/api-reference/pythreejs.md
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.962068 plopp-24.2.0/docs/developer/
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/developer/coding-conventions.md
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/developer/dependency-management.md
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/developer/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/developer/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.966068 plopp-24.2.0/docs/gallery/
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/gallery/index.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/gallery/interactive-masking.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/gallery/masking-a-range.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/gallery/nyc-taxi.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/gallery/peeling-layers.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/gallery/polar-plots.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/gallery/rectangle-selection.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/gallery/scatter3d-with-slider.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/gallery/scatter3d-with-threshold.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/gallery/tiled-random-samples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.966068 plopp-24.2.0/docs/user-guide/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.966068 plopp-24.2.0/docs/user-guide/customization/
--rw-r--r--   0 runner    (1001) docker     (127)    17726 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/user-guide/customization/custom-interfaces.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/user-guide/customization/graph-node-tips.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7970 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/user-guide/customization/subplots.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/user-guide/customization/tweaking-figures.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.966068 plopp-24.2.0/docs/user-guide/getting-started/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/user-guide/getting-started/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/user-guide/getting-started/numpy-pandas-xarray.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8674 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/user-guide/getting-started/overview.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/user-guide/getting-started/saving-figures.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/user-guide/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.966068 plopp-24.2.0/docs/user-guide/plot-types/
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/user-guide/plot-types/image-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/user-guide/plot-types/inspector-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10137 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/user-guide/plot-types/line-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/user-guide/plot-types/scatter3d-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/user-guide/plot-types/slicer-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-02-19 10:31:14.000000 plopp-24.2.0/docs/user-guide/plot-types/super-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-02-19 10:31:14.000000 plopp-24.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.970068 plopp-24.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/basetest.in
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/basetest.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/constraints.in
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/make_base.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/mini.in
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/mini.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/mypy.in
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/mypy.txt
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/nightly.in
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/nightly.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/noplotly.in
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/noplotly.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/optional.in
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/optional.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-02-19 10:31:14.000000 plopp-24.2.0/requirements/wheels.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.970068 plopp-24.2.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    53363 2024-02-19 10:31:14.000000 plopp-24.2.0/resources/logo-plopp-2022.svg
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-19 10:31:25.990068 plopp-24.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.950068 plopp-24.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.974068 plopp-24.2.0/src/plopp/
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.974068 plopp-24.2.0/src/plopp/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/backends/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/backends/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.974068 plopp-24.2.0/src/plopp/backends/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/backends/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16231 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/backends/matplotlib/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/backends/matplotlib/figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/backends/matplotlib/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/backends/matplotlib/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/backends/matplotlib/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/backends/matplotlib/static.py
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/backends/matplotlib/tiled.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/backends/matplotlib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.974068 plopp-24.2.0/src/plopp/backends/plotly/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/backends/plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10934 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/backends/plotly/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/backends/plotly/figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/backends/plotly/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/backends/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.978068 plopp-24.2.0/src/plopp/backends/pythreejs/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/backends/pythreejs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8550 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/backends/pythreejs/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/backends/pythreejs/figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/backends/pythreejs/outline.py
--rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/backends/pythreejs/point_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.978068 plopp-24.2.0/src/plopp/core/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/core/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/core/limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/core/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/core/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/core/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.978068 plopp-24.2.0/src/plopp/data/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/data/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/data/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/data/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.982068 plopp-24.2.0/src/plopp/graphics/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/graphics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/graphics/basefig.py
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/graphics/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/graphics/colormapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/graphics/figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/graphics/imageview.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/graphics/lineview.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/graphics/scatter3dview.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/graphics/tiled.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.982068 plopp-24.2.0/src/plopp/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/plotting/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/plotting/inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/plotting/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/plotting/scatter3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/plotting/slicer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/plotting/superplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/plotting/xyplot.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.982068 plopp-24.2.0/src/plopp/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/widgets/checkboxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11211 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/widgets/cut3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/widgets/drawing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/widgets/slice.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/widgets/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/widgets/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-02-19 10:31:14.000000 plopp-24.2.0/src/plopp/widgets/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.990068 plopp-24.2.0/src/plopp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-02-19 10:31:25.000000 plopp-24.2.0/src/plopp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-02-19 10:31:25.000000 plopp-24.2.0/src/plopp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 10:31:25.000000 plopp-24.2.0/src/plopp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-19 10:31:25.000000 plopp-24.2.0/src/plopp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-19 10:31:25.000000 plopp-24.2.0/src/plopp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.982068 plopp-24.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.950068 plopp-24.2.0/tests/backends/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.986068 plopp-24.2.0/tests/backends/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/backends/matplotlib/mpl_canvas_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/backends/matplotlib/mpl_figure_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/backends/matplotlib/mpl_image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/backends/matplotlib/mpl_imageview_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/backends/matplotlib/mpl_interactive_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/backends/matplotlib/mpl_line_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/backends/matplotlib/mpl_lineview_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/backends/matplotlib/mpl_tiled_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/backends/matplotlib/mpl_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.986068 plopp-24.2.0/tests/backends/plotly/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/backends/plotly/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/backends/plotly/plotly_canvas_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/backends/plotly/plotly_figure_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/backends/plotly/plotly_line_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.986068 plopp-24.2.0/tests/backends/pythreejs/
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/backends/pythreejs/pythreejs_canvas_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/backends/pythreejs/pythreejs_figure_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/backends/pythreejs/pythreejs_point_cloud_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.986068 plopp-24.2.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/core/graph_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/core/limits_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/core/node_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/core/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.986068 plopp-24.2.0/tests/graphics/
--rw-r--r--   0 runner    (1001) docker     (127)     8472 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/graphics/colormapper_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/graphics/imageview_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/graphics/lineview_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/graphics/scatter3dview_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/high_level_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/minimal_plot_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/package_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.990068 plopp-24.2.0/tests/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/plotting/common_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/plotting/inspector_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/plotting/plot_1d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/plotting/plot_2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/plotting/scatter3d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/plotting/slicer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/plotting/superplot_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/plotting/xyplot_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:31:25.990068 plopp-24.2.0/tests/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/widgets/box_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/widgets/checkboxes_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/widgets/cut3d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-02-19 10:31:14.000000 plopp-24.2.0/tests/widgets/slice_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-02-19 10:31:14.000000 plopp-24.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.881412 plopp-24.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-16 14:08:37.000000 plopp-24.4.0/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.837412 plopp-24.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-16 14:08:37.000000 plopp-24.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.841412 plopp-24.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-16 14:08:37.000000 plopp-24.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-16 14:08:37.000000 plopp-24.4.0/.github/workflows/copier.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-16 14:08:37.000000 plopp-24.4.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-16 14:08:37.000000 plopp-24.4.0/.github/workflows/nightly_at_main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-16 14:08:37.000000 plopp-24.4.0/.github/workflows/nightly_at_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-16 14:08:37.000000 plopp-24.4.0/.github/workflows/python-version-ci
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-16 14:08:37.000000 plopp-24.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-16 14:08:37.000000 plopp-24.4.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-16 14:08:37.000000 plopp-24.4.0/.github/workflows/unpinned.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-16 14:08:37.000000 plopp-24.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-16 14:08:37.000000 plopp-24.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-16 14:08:37.000000 plopp-24.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-16 14:08:37.000000 plopp-24.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-16 14:08:37.000000 plopp-24.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-16 14:08:37.000000 plopp-24.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-16 14:08:48.881412 plopp-24.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-16 14:08:37.000000 plopp-24.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.841412 plopp-24.4.0/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-16 14:08:37.000000 plopp-24.4.0/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.841412 plopp-24.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.841412 plopp-24.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/anaconda-icon.js
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/circle-exclamation.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.841412 plopp-24.4.0/docs/_static/customization/
+-rw-r--r--   0 runner    (1001) docker     (127)   114427 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/customization/custom-interfaces.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44133 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/customization/graph-node-tips.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54880 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/customization/subplots.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19228 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/customization/tweaking-figures.png
+-rw-r--r--   0 runner    (1001) docker     (127)   137750 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.845412 plopp-24.4.0/docs/_static/gallery/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/gallery/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   211913 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/gallery/peeling-layers-thumbnail.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18766 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/gallery/scatter3d-with-slider-thumbnail.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66718 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/gallery/scatter3d-with-threshold-thumbnail.png
+-rw-r--r--   0 runner    (1001) docker     (127)    76311 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    76253 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.845412 plopp-24.4.0/docs/_static/plot-types/
+-rw-r--r--   0 runner    (1001) docker     (127)    37065 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/plot-types/image-plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47635 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/plot-types/inspector-plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15510 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/plot-types/line-plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    72368 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/plot-types/scatter-plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)   186659 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/plot-types/scatter3d-plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55181 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/plot-types/slicer-plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    50020 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_static/plot-types/super-plot.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.845412 plopp-24.4.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_templates/class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_templates/doc_version.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_templates/module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_templates/scipp-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/_templates/scipp-module-template.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.845412 plopp-24.4.0/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/about/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.849412 plopp-24.4.0/docs/api-reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/api-reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/api-reference/matplotlib.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/api-reference/plotly.md
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/api-reference/pythreejs.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7454 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.849412 plopp-24.4.0/docs/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/developer/coding-conventions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/developer/dependency-management.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/developer/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/developer/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.849412 plopp-24.4.0/docs/gallery/
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/gallery/index.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/gallery/interactive-masking.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/gallery/masking-a-range.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/gallery/nyc-taxi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/gallery/peeling-layers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/gallery/polar-plots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/gallery/rectangle-selection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/gallery/scatter3d-with-slider.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/gallery/scatter3d-with-threshold.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/gallery/tiled-random-samples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/gallery/updating-scatter.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.849412 plopp-24.4.0/docs/user-guide/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.849412 plopp-24.4.0/docs/user-guide/customization/
+-rw-r--r--   0 runner    (1001) docker     (127)    17726 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/customization/custom-interfaces.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/customization/graph-node-tips.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7970 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/customization/subplots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/customization/tweaking-figures.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.853412 plopp-24.4.0/docs/user-guide/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/getting-started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/getting-started/numpy-pandas-xarray.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8674 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/getting-started/overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/getting-started/saving-figures.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.853412 plopp-24.4.0/docs/user-guide/plot-types/
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/plot-types/image-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/plot-types/inspector-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/plot-types/line-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/plot-types/scatter-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/plot-types/scatter3d-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/plot-types/slicer-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-16 14:08:37.000000 plopp-24.4.0/docs/user-guide/plot-types/super-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-16 14:08:37.000000 plopp-24.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.857412 plopp-24.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/basetest.in
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/basetest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/constraints.in
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/make_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/mini.in
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/mini.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/mypy.in
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/mypy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/nightly.in
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/nightly.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/noplotly.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/noplotly.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/optional.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/optional.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-16 14:08:37.000000 plopp-24.4.0/requirements/wheels.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.857412 plopp-24.4.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    53363 2024-04-16 14:08:37.000000 plopp-24.4.0/resources/logo-plopp-2022.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-16 14:08:48.881412 plopp-24.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.833412 plopp-24.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.857412 plopp-24.4.0/src/plopp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.861412 plopp-24.4.0/src/plopp/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.861412 plopp-24.4.0/src/plopp/backends/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17975 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/matplotlib/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/matplotlib/figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/matplotlib/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/matplotlib/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/matplotlib/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/matplotlib/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/matplotlib/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/matplotlib/tiled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/matplotlib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.861412 plopp-24.4.0/src/plopp/backends/plotly/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11027 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/plotly/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/plotly/figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/plotly/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.865412 plopp-24.4.0/src/plopp/backends/pythreejs/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/pythreejs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/pythreejs/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/pythreejs/figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/pythreejs/outline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/backends/pythreejs/point_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.865412 plopp-24.4.0/src/plopp/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/core/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/core/limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/core/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/core/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.865412 plopp-24.4.0/src/plopp/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/data/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/data/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/data/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.869412 plopp-24.4.0/src/plopp/graphics/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/basefig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/colormapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/graphicalview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/imageview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/lineview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/scatter3dview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/scatterview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/graphics/tiled.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.869412 plopp-24.4.0/src/plopp/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/plotting/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/plotting/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/plotting/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/plotting/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/plotting/scatter3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/plotting/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/plotting/superplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/plotting/xyplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.873412 plopp-24.4.0/src/plopp/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/checkboxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13963 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/clip3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10244 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/cut3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/debounce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/linesave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-04-16 14:08:37.000000 plopp-24.4.0/src/plopp/widgets/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.881412 plopp-24.4.0/src/plopp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-16 14:08:48.000000 plopp-24.4.0/src/plopp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-04-16 14:08:48.000000 plopp-24.4.0/src/plopp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:08:48.000000 plopp-24.4.0/src/plopp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-16 14:08:48.000000 plopp-24.4.0/src/plopp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 14:08:48.000000 plopp-24.4.0/src/plopp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.873412 plopp-24.4.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.837412 plopp-24.4.0/tests/backends/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.873412 plopp-24.4.0/tests/backends/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/matplotlib/mpl_canvas_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/matplotlib/mpl_figure_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/matplotlib/mpl_image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/matplotlib/mpl_imageview_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/matplotlib/mpl_interactive_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/matplotlib/mpl_line_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/matplotlib/mpl_lineview_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/matplotlib/mpl_scatter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/matplotlib/mpl_tiled_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/matplotlib/mpl_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.873412 plopp-24.4.0/tests/backends/plotly/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/plotly/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/plotly/plotly_canvas_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/plotly/plotly_figure_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/plotly/plotly_line_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.877412 plopp-24.4.0/tests/backends/pythreejs/
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/pythreejs/pythreejs_canvas_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/pythreejs/pythreejs_figure_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/backends/pythreejs/pythreejs_point_cloud_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.877412 plopp-24.4.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/core/graph_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/core/limits_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/core/node_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/core/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.877412 plopp-24.4.0/tests/graphics/
+-rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/graphics/colormapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/graphics/imageview_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/graphics/lineview_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/graphics/scatter3dview_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/graphics/scatterview_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/high_level_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/minimal_plot_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/package_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.877412 plopp-24.4.0/tests/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/plotting/common_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/plotting/inspector_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/plotting/plot_1d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/plotting/plot_2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/plotting/scatter3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/plotting/scatter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/plotting/slicer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/plotting/superplot_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/plotting/xyplot_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:08:48.881412 plopp-24.4.0/tests/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/widgets/box_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/widgets/checkboxes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/widgets/clip3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/widgets/cut3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-16 14:08:37.000000 plopp-24.4.0/tests/widgets/slice_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-16 14:08:37.000000 plopp-24.4.0/tox.ini
```

### Comparing `plopp-24.2.0/.github/workflows/ci.yml` & `plopp-24.4.0/.github/workflows/nightly_at_release.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,40 @@
-# SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
-name: CI
+name: Nightly tests at latest release
 
 on:
-  push:
-    branches:
-      - main
-      - release
-  pull_request:
+  workflow_dispatch:
+  schedule:
+    - cron: '0 1 * * 1-5'
 
 jobs:
-  formatting:
-    name: Formatting and static analysis
+  setup:
+    name: Setup variables
     runs-on: 'ubuntu-22.04'
     outputs:
       min_python: ${{ steps.vars.outputs.min_python }}
-      min_tox_env: ${{ steps.vars.outputs.min_tox_env }}
+      release_tag: ${{ steps.release.outputs.release_tag }}
     steps:
       - uses: actions/checkout@v4
+        with:
+          fetch-depth: 0  # history required so we can determine latest release tag
+      - name: Get last release tag from git
+        id: release
+        run: echo "release_tag=$(git describe --tags --abbrev=0 --match '[0-9]*.[0-9]*.[0-9]*')" >> $GITHUB_OUTPUT
       - name: Get Python version for other CI jobs
         id: vars
-        run: |
-          echo "min_python=$(cat .github/workflows/python-version-ci)" >> $GITHUB_OUTPUT
-          echo "min_tox_env=py$(cat .github/workflows/python-version-ci | sed 's/\.//g')" >> $GITHUB_OUTPUT
-      - uses: actions/setup-python@v4
-        with:
-          python-version-file: '.github/workflows/python-version-ci'
-      - run: python -m pip install --upgrade pip
-      - run: python -m pip install -r requirements/ci.txt
-      - run: tox -e static
-      - uses: stefanzweifel/git-auto-commit-action@v5
-        with:
-          commit_message: Apply automatic formatting
+        run: echo "min_python=$(cat .github/workflows/python-version-ci)" >> $GITHUB_OUTPUT
 
   tests:
     name: Tests
-    needs: formatting
+    needs: setup
     strategy:
       matrix:
         os: ['ubuntu-22.04']
         python:
-          - version: '${{needs.formatting.outputs.min_python}}'
-            tox-env: '${{needs.formatting.outputs.min_tox_env}}'
+          - version: '${{needs.setup.outputs.min_python}}'
+            tox-env: 'nightly'
     uses: ./.github/workflows/test.yml
     with:
       os-variant: ${{ matrix.os }}
       python-version: ${{ matrix.python.version }}
       tox-env: ${{ matrix.python.tox-env }}
-
-  docs:
-    needs: tests
-    uses: ./.github/workflows/docs.yml
-    with:
-      publish: false
-      linkcheck: ${{ contains(matrix.variant.os, 'ubuntu') && github.ref == 'refs/heads/main' }}
-      branch: ${{ github.head_ref == '' && github.ref_name || github.head_ref }}
+      checkout_ref: ${{ needs.setup.outputs.release_tag }}
```

### Comparing `plopp-24.2.0/.github/workflows/docs.yml` & `plopp-24.4.0/.github/workflows/docs.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
 name: Docs
 
 on:
   workflow_dispatch:
     inputs:
       publish:
         default: false
@@ -43,33 +40,34 @@
 
 jobs:
   docs:
     name: Build documentation
     runs-on: 'ubuntu-22.04'
     steps:
       - run: sudo apt install --yes graphviz pandoc
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           ref: ${{ inputs.branch == '' && github.ref_name || inputs.branch }}
+          repository: ${{ github.event.pull_request.head.repo.full_name }}
           fetch-depth: 0  # history required so cmake can determine version
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version-file: '.github/workflows/python-version-ci'
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - run: tox -e releasedocs -- ${VERSION}
         if: ${{ inputs.version != '' }}
       - run: tox -e docs
         if: ${{ inputs.version == '' }}
       - run: tox -e linkcheck
         if: ${{ inputs.linkcheck }}
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
           name: docs_html
           path: html/
 
-      - uses: JamesIves/github-pages-deploy-action@v4.4.3
+      - uses: JamesIves/github-pages-deploy-action@v4.5.0
         if: ${{ inputs.publish }}
         with:
           branch: gh-pages
           folder: html
           single-commit: true
```

### Comparing `plopp-24.2.0/.github/workflows/nightly_at_main.yml` & `plopp-24.4.0/.github/workflows/nightly_at_main.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
 name: Nightly test at main branch
 
 on:
   workflow_dispatch:
   schedule:
     - cron: '30 1 * * 1-5'
```

### Comparing `plopp-24.2.0/.github/workflows/nightly_at_release.yml` & `plopp-24.4.0/.github/workflows/unpinned.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-# SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
-name: Nightly tests at latest release
+name: Unpinned tests at latest release
 
 on:
   workflow_dispatch:
   schedule:
-    - cron: '0 1 * * 1-5'
+    - cron: '0 2 * * 1'
 
 jobs:
   setup:
     name: Setup variables
     runs-on: 'ubuntu-22.04'
     outputs:
       min_python: ${{ steps.vars.outputs.min_python }}
@@ -30,14 +27,14 @@
     name: Tests
     needs: setup
     strategy:
       matrix:
         os: ['ubuntu-22.04']
         python:
           - version: '${{needs.setup.outputs.min_python}}'
-            tox-env: 'nightly'
+            tox-env: 'unpinned'
     uses: ./.github/workflows/test.yml
     with:
       os-variant: ${{ matrix.os }}
       python-version: ${{ matrix.python.version }}
       tox-env: ${{ matrix.python.tox-env }}
       checkout_ref: ${{ needs.setup.outputs.release_tag }}
```

### Comparing `plopp-24.2.0/.github/workflows/release.yml` & `plopp-24.4.0/.github/workflows/release.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
 name: Release
 
 on:
   release:
     types: [published]
   workflow_dispatch:
 
@@ -14,77 +11,77 @@
 
 jobs:
   build_conda:
     name: Conda build
     runs-on: 'ubuntu-22.04'
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           submodules: true
           fetch-depth: 0  # history required so setuptools_scm can determine version
 
       - uses: mamba-org/setup-micromamba@v1
         with:
           environment-name: build-env
           create-args: >-
             conda-build
             boa
       - run: conda mambabuild --channel conda-forge --channel scipp --no-anaconda-upload --override-channels --output-folder conda/package conda
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
           name: conda-package-noarch
           path: conda/package/noarch/*.tar.bz2
 
   build_wheels:
     name: Wheels
     runs-on: 'ubuntu-22.04'
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0  # history required so setuptools_scm can determine version
 
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version-file: '.github/workflows/python-version-ci'
 
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/wheels.txt
 
       - name: Build wheels
         run: python -m build
 
       - name: Upload wheels
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           name: dist
           path: dist
 
   upload_pypi:
     name: Deploy PyPI
     needs: [build_wheels, build_conda]
     runs-on: 'ubuntu-22.04'
     environment: release
     permissions:
       id-token: write
     if: github.event_name == 'release' && github.event.action == 'published'
     steps:
-      - uses: actions/download-artifact@v3
-      - uses: pypa/gh-action-pypi-publish@v1.8.10
+      - uses: actions/download-artifact@v4
+      - uses: pypa/gh-action-pypi-publish@v1.8.14
 
   upload_conda:
     name: Deploy Conda
     needs: [build_wheels, build_conda]
     runs-on: 'ubuntu-22.04'
     if: github.event_name == 'release' && github.event.action == 'published'
 
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
       - uses: mamba-org/setup-micromamba@v1
         with:
           environment-name: upload-env
           # frozen python due to breaking removal of 'imp' in 3.12
           create-args: >-
             anaconda-client
             python=3.11
@@ -100,15 +97,15 @@
   assets:
     name: Upload docs
     needs: docs
     runs-on: 'ubuntu-22.04'
     permissions:
       contents: write  # This is needed so that the action can upload the asset
     steps:
-    - uses: actions/download-artifact@v3
+    - uses: actions/download-artifact@v4
     - name: Zip documentation
       run: |
         mv docs_html documentation-${{ github.ref_name }}
         zip -r documentation-${{ github.ref_name }}.zip documentation-${{ github.ref_name }}
     - name: Upload release assets
       uses: svenstaro/upload-release-action@v2
       with:
```

### Comparing `plopp-24.2.0/.github/workflows/test.yml` & `plopp-24.4.0/.github/workflows/test.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
 name: Test
 
 on:
   workflow_dispatch:
     inputs:
       os-variant:
         default: 'ubuntu-22.04'
@@ -44,21 +41,21 @@
         type: string
 
 jobs:
   test:
     runs-on: ${{ inputs.os-variant }}
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           ref: ${{ inputs.checkout_ref }}
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ inputs.python-version }}
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r ${{ inputs.pip-recipe }}
       - run: tox -e ${{ inputs.tox-env }}
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         if: ${{ inputs.coverage-report }}
         with:
           name: CoverageReport
           path: coverage_html/
```

### Comparing `plopp-24.2.0/.pre-commit-config.yaml` & `plopp-24.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/CODE_OF_CONDUCT.md` & `plopp-24.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/CONTRIBUTING.md` & `plopp-24.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/LICENSE` & `plopp-24.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/PKG-INFO` & `plopp-24.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plopp
-Version: 24.2.0
+Version: 24.4.0
 Summary: Visualization library for Scipp
 Author: Scipp contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Scipp contributors (https://github.com/scipp)
         All rights reserved.
         
@@ -41,14 +41,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.5
 Provides-Extra: scipp
```

### Comparing `plopp-24.2.0/README.md` & `plopp-24.4.0/README.md`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/_static/anaconda-icon.js` & `plopp-24.4.0/docs/_static/anaconda-icon.js`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/_static/circle-exclamation.svg` & `plopp-24.4.0/docs/_static/circle-exclamation.svg`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/_static/customization/custom-interfaces.png` & `plopp-24.4.0/docs/_static/customization/custom-interfaces.png`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/_static/customization/graph-node-tips.png` & `plopp-24.4.0/docs/_static/customization/graph-node-tips.png`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/_static/customization/subplots.png` & `plopp-24.4.0/docs/_static/customization/subplots.png`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/_static/customization/tweaking-figures.png` & `plopp-24.4.0/docs/_static/customization/tweaking-figures.png`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/_static/favicon.ico` & `plopp-24.4.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/_static/gallery/peeling-layers-thumbnail.png` & `plopp-24.4.0/docs/_static/gallery/peeling-layers-thumbnail.png`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/_static/gallery/scatter3d-with-slider-thumbnail.png` & `plopp-24.4.0/docs/_static/gallery/scatter3d-with-slider-thumbnail.png`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/_static/gallery/scatter3d-with-threshold-thumbnail.png` & `plopp-24.4.0/docs/_static/gallery/scatter3d-with-threshold-thumbnail.png`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/_static/logo-dark.svg` & `plopp-24.4.0/docs/_static/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/_static/logo.svg` & `plopp-24.4.0/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/_static/plot-types/image-plot.png` & `plopp-24.4.0/docs/_static/plot-types/image-plot.png`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/_static/plot-types/inspector-plot.png` & `plopp-24.4.0/docs/_static/plot-types/inspector-plot.png`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/_static/plot-types/line-plot.png` & `plopp-24.4.0/docs/_static/plot-types/line-plot.png`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/_static/plot-types/scatter3d-plot.png` & `plopp-24.4.0/docs/_static/plot-types/scatter3d-plot.png`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/_static/plot-types/slicer-plot.png` & `plopp-24.4.0/docs/_static/plot-types/slicer-plot.png`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/_static/plot-types/super-plot.png` & `plopp-24.4.0/docs/_static/plot-types/super-plot.png`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/_templates/class-template.rst` & `plopp-24.4.0/docs/_templates/class-template.rst`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/_templates/module-template.rst` & `plopp-24.4.0/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/_templates/scipp-class-template.rst` & `plopp-24.4.0/docs/_templates/scipp-class-template.rst`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/_templates/scipp-module-template.rst` & `plopp-24.4.0/docs/_templates/scipp-module-template.rst`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/about/index.md` & `plopp-24.4.0/docs/about/index.md`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/api-reference/index.md` & `plopp-24.4.0/docs/api-reference/index.md`

 * *Files 27% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 .. autosummary::
    :toctree: ../generated
 
    plot
    slicer
    superplot
    inspector
+   scatter
    scatter3d
    xyplot
 ```
 
 ## Core
 
 ```{eval-rst}
@@ -36,16 +37,21 @@
    :toctree: ../generated
 
    graphics.Camera
    graphics.ColorMapper
    graphics.figure1d
    graphics.figure2d
    graphics.figure3d
+   graphics.imagefigure
    graphics.ImageView
+   graphics.linefigure
    graphics.LineView
+   graphics.scatterfigure
+   graphics.ScatterView
+   graphics.scatter3dfigure
    graphics.Scatter3dView
    graphics.tiled
 ```
 
 ## Widgets and tools
 
 ```{eval-rst}
@@ -71,14 +77,16 @@
    widgets.tools.PanZoomTool
    widgets.tools.SaveTool
    widgets.tools.ToggleTool
 
    widgets.drawing.DrawingTool
    widgets.drawing.PointsTool
 
+   widgets.clip3d.Clip3dTool
+   widgets.clip3d.ClippingPlanes
    widgets.cut3d.Cut3dTool
    widgets.cut3d.TriCutTool
 ```
 
 ## Backends
 
 ```{eval-rst}
```

### Comparing `plopp-24.2.0/docs/conf.py` & `plopp-24.4.0/docs/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import doctest
 import os
 import sys
-
-import plopp
+from importlib.metadata import version as get_version
 
 sys.path.insert(0, os.path.abspath('.'))
 
-from _typehints import typehints_formatter_for  # noqa: E402
-
 # General information about the project.
 project = u'Plopp'
 copyright = u'2024 Scipp contributors'
 author = u'Scipp contributors'
 
 html_show_sourcelink = True
 
@@ -22,22 +19,31 @@
     'sphinx.ext.autodoc',
     'sphinx.ext.autosummary',
     'sphinx.ext.doctest',
     'sphinx.ext.githubpages',
     'sphinx.ext.intersphinx',
     'sphinx.ext.mathjax',
     'sphinx.ext.napoleon',
+    'sphinx.ext.viewcode',
     'sphinx_autodoc_typehints',
     'sphinx_copybutton',
     'sphinx_design',
     'nbsphinx',
     'sphinx_gallery.load_style',
     'myst_parser',
 ]
 
+try:
+    import sciline.sphinxext.domain_types  # noqa: F401
+
+    extensions.append('sciline.sphinxext.domain_types')
+except ModuleNotFoundError:
+    pass
+
+
 myst_enable_extensions = [
     "amsmath",
     "colon_fence",
     "deflist",
     "dollarmath",
     "fieldlist",
     "html_admonition",
@@ -73,15 +79,26 @@
 napoleon_preprocess_types = True
 napoleon_type_aliases = {
     # objects without namespace: numpy
     "ndarray": "~numpy.ndarray",
 }
 typehints_defaults = 'comma'
 typehints_use_rtype = False
-typehints_formatter = typehints_formatter_for('plopp')
+
+
+sciline_domain_types_prefix = 'plopp'
+sciline_domain_types_aliases = {
+    'scipp._scipp.core.DataArray': 'scipp.DataArray',
+    'scipp._scipp.core.Dataset': 'scipp.Dataset',
+    'scipp._scipp.core.DType': 'scipp.DType',
+    'scipp._scipp.core.Unit': 'scipp.Unit',
+    'scipp._scipp.core.Variable': 'scipp.Variable',
+    'scipp.core.data_group.DataGroup': 'scipp.DataGroup',
+}
+
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
@@ -92,18 +109,16 @@
 master_doc = 'index'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 
-# The short X.Y version.
-version = plopp.__version__
-# The full version, including alpha/beta/rc tags.
-release = plopp.__version__
+release = get_version("plopp")
+version = ".".join(release.split('.')[:3])  # CalVer
 
 warning_is_error = True
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
@@ -228,14 +243,15 @@
     'rectangle-selection',
     'scatter3d-with-threshold',
     'scatter3d-with-slider',
     'interactive-masking',
     'peeling-layers',
     'tiled-random-samples',
     'polar-plots',
+    'updating-scatter',
 ]
 nbsphinx_thumbnails = {
     os.path.join(notebook_root, notebook): os.path.join(
         thumbnail_root, f'{notebook}-thumbnail.png'
     )
     for notebook in gallery_notebooks
 }
```

### Comparing `plopp-24.2.0/docs/developer/coding-conventions.md` & `plopp-24.4.0/docs/developer/coding-conventions.md`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/developer/dependency-management.md` & `plopp-24.4.0/docs/developer/dependency-management.md`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/developer/getting-started.md` & `plopp-24.4.0/docs/developer/getting-started.md`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/gallery/index.ipynb` & `plopp-24.4.0/docs/gallery/index.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978693181818181%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(8, '* [Polar plots](polar-plots.ipynb)\\n'), (9, '* "*

 * *            "[Updating scatter points](updating-scatter.ipynb)')], delete: [8]}}}"}*

```diff
@@ -31,15 +31,16 @@
                 "* [Masking a range](masking-a-range.ipynb)\n",
                 "* [Rectangle selection](rectangle-selection.ipynb)\n",
                 "* [3-D scatter plot with threshold](scatter3d-with-threshold.ipynb)\n",
                 "* [3-D scatter plot with slider](scatter3d-with-slider.ipynb)\n",
                 "* [Interactive masking](interactive-masking.ipynb)\n",
                 "* [Peeling off the layers](peeling-layers.ipynb)\n",
                 "* [Tiled random sample histograms](tiled-random-samples.ipynb)\n",
-                "* [Polar plots](polar-plots.ipynb)"
+                "* [Polar plots](polar-plots.ipynb)\n",
+                "* [Updating scatter points](updating-scatter.ipynb)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
```

### Comparing `plopp-24.2.0/docs/gallery/interactive-masking.ipynb` & `plopp-24.4.0/docs/gallery/interactive-masking.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/gallery/masking-a-range.ipynb` & `plopp-24.4.0/docs/gallery/masking-a-range.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/gallery/nyc-taxi.ipynb` & `plopp-24.4.0/docs/gallery/nyc-taxi.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/gallery/peeling-layers.ipynb` & `plopp-24.4.0/docs/gallery/peeling-layers.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999732905982906%*

 * *Differences: {"'cells'": "{5: {'source': {insert: [(8, 'clouds = list(p.artists.values())\\n')], delete: [8]}}}"}*

```diff
@@ -103,15 +103,15 @@
                 "a = da[da.data > sc.scalar(0.05)]\n",
                 "b = da[(da.data > sc.scalar(0.002)) & (da.data < sc.scalar(0.005))]\n",
                 "\n",
                 "# Display both on the same scatter plot\n",
                 "p = pp.scatter3d({'a': a, 'b': b}, pos='position', norm='log')\n",
                 "\n",
                 "# Extract the point clouds from the final plot and set a lower opacity on the second point cloud\n",
-                "clouds = list(p[0].artists.values())\n",
+                "clouds = list(p.artists.values())\n",
                 "clouds[1].opacity = 0.1\n",
                 "\n",
                 "p"
             ]
         }
     ],
     "metadata": {
```

### Comparing `plopp-24.2.0/docs/gallery/polar-plots.ipynb` & `plopp-24.4.0/docs/gallery/polar-plots.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/gallery/rectangle-selection.ipynb` & `plopp-24.4.0/docs/gallery/rectangle-selection.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/gallery/scatter3d-with-slider.ipynb` & `plopp-24.4.0/docs/gallery/scatter3d-with-slider.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/gallery/scatter3d-with-threshold.ipynb` & `plopp-24.4.0/docs/gallery/scatter3d-with-threshold.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/gallery/tiled-random-samples.ipynb` & `plopp-24.4.0/docs/gallery/tiled-random-samples.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955357142857143%*

 * *Differences: {"'metadata'": "{'language_info': {delete: ['version']}}"}*

```diff
@@ -157,14 +157,13 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.9.18"
+            "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `plopp-24.2.0/docs/index.md` & `plopp-24.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/user-guide/customization/custom-interfaces.ipynb` & `plopp-24.4.0/docs/user-guide/customization/custom-interfaces.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/user-guide/customization/graph-node-tips.ipynb` & `plopp-24.4.0/docs/user-guide/customization/graph-node-tips.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/user-guide/customization/subplots.ipynb` & `plopp-24.4.0/docs/user-guide/customization/subplots.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/user-guide/customization/tweaking-figures.ipynb` & `plopp-24.4.0/docs/user-guide/customization/tweaking-figures.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/user-guide/getting-started/installation.md` & `plopp-24.4.0/docs/user-guide/getting-started/installation.md`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/user-guide/getting-started/numpy-pandas-xarray.ipynb` & `plopp-24.4.0/docs/user-guide/getting-started/numpy-pandas-xarray.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/user-guide/getting-started/overview.ipynb` & `plopp-24.4.0/docs/user-guide/getting-started/overview.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/user-guide/getting-started/saving-figures.ipynb` & `plopp-24.4.0/docs/user-guide/getting-started/saving-figures.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994212962962963%*

 * *Differences: {"'cells'": '{7: {\'source\': {insert: [(2, "f3d.save(\'fig3d.html\')")], delete: [2]}}}'}*

```diff
@@ -95,15 +95,15 @@
             "execution_count": null,
             "id": "7445224e-bedd-4002-b0e7-091aad715e2c",
             "metadata": {},
             "outputs": [],
             "source": [
                 "f3d = pp.scatter3d(pp.data.scatter(), pos='position')\n",
                 "# Need index 0, as `scatter3d` returns a Box with the figure and cut3d tool\n",
-                "f3d[0].save('fig3d.html')"
+                "f3d.save('fig3d.html')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "618fe7bf-c9ae-4372-af42-e214b16ae980",
             "metadata": {},
             "source": [
```

### Comparing `plopp-24.2.0/docs/user-guide/index.md` & `plopp-24.4.0/docs/user-guide/index.md`

 * *Files 8% similar despite different names*

```diff
@@ -53,36 +53,46 @@
 
 :::{grid-item-card} Image plot
 :link: plot-types/image-plot.ipynb
 :img-bottom: ../_static/plot-types/image-plot.png
 
 :::
 
-::::{grid-item-card} Slicer plot
-:link: plot-types/slicer-plot.ipynb
-:img-bottom: ../_static/plot-types/slicer-plot.png
+::::{grid-item-card} Scatter plot
+:link: plot-types/scatter-plot.ipynb
+:img-bottom: ../_static/plot-types/scatter-plot.png
 
 :::
 
 ::::
 
 ::::{grid} 3
 
+:::{grid-item-card} Slicer plot
+:link: plot-types/slicer-plot.ipynb
+:img-bottom: ../_static/plot-types/slicer-plot.png
+
+:::
+
 :::{grid-item-card} Inspector plot
 :link: plot-types/inspector-plot.ipynb
 :img-bottom: ../_static/plot-types/inspector-plot.png
 
 :::
 
 :::{grid-item-card} Super-plot
 :link: plot-types/super-plot.ipynb
 :img-bottom: ../_static/plot-types/super-plot.png
 
 :::
 
+::::
+
+::::{grid} 3
+
 :::{grid-item-card} Scatter 3D plot
 :link: plot-types/scatter3d-plot.ipynb
 :img-bottom: ../_static/plot-types/scatter3d-plot.png
 
 :::
 
 ::::
@@ -93,14 +103,15 @@
 ---
 
 plot-types/line-plot
 plot-types/image-plot
 plot-types/slicer-plot
 plot-types/inspector-plot
 plot-types/super-plot
+plot-types/scatter-plot
 plot-types/scatter3d-plot
 ```
 
 ## Custom figures
 
 ::::{grid} 3
```

### Comparing `plopp-24.2.0/docs/user-guide/plot-types/image-plot.ipynb` & `plopp-24.4.0/docs/user-guide/plot-types/image-plot.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996603260869565%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'As with one-dimensional data, plotting two-dimensional "*

 * *            "data is done using the [plot](../../generated/plopp.plot.rst) function.')], delete: "*

 * *            '[2]}}}'}*

```diff
@@ -22,15 +22,15 @@
         {
             "cell_type": "markdown",
             "id": "8487626a-2461-40c2-b0cd-42c6f82c9fab",
             "metadata": {},
             "source": [
                 "## Basic image plot\n",
                 "\n",
-                "As with one-dimensional data, plotting two-dimensional data is done using the [plot](../../reference/generated/plopp.plot.rst) function."
+                "As with one-dimensional data, plotting two-dimensional data is done using the [plot](../../generated/plopp.plot.rst) function."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "5af375f3-655c-4466-ba56-00312dafc524",
             "metadata": {},
```

### Comparing `plopp-24.2.0/docs/user-guide/plot-types/inspector-plot.ipynb` & `plopp-24.4.0/docs/user-guide/plot-types/inspector-plot.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/docs/user-guide/plot-types/line-plot.ipynb` & `plopp-24.4.0/docs/user-guide/plot-types/line-plot.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998592342342343%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'The most common way to plot data with Plopp is to use "*

 * *            "the [plot](../../generated/plopp.plot.rst) function.\\n')], delete: [2]}}}"}*

```diff
@@ -22,15 +22,15 @@
         {
             "cell_type": "markdown",
             "id": "8487626a-2461-40c2-b0cd-42c6f82c9fab",
             "metadata": {},
             "source": [
                 "## Basic line plot\n",
                 "\n",
-                "The most common way to plot data with Plopp is to use the [plot](../../reference/generated/plopp.plot.rst) function.\n",
+                "The most common way to plot data with Plopp is to use the [plot](../../generated/plopp.plot.rst) function.\n",
                 "This can either be done using the `plopp.plot()` free function,\n",
                 "or calling the `.plot()` method on a Scipp data object (both are equivalent)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `plopp-24.2.0/docs/user-guide/plot-types/scatter3d-plot.ipynb` & `plopp-24.4.0/docs/user-guide/plot-types/scatter3d-plot.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9940600198412699%*

 * *Differences: {"'cells'": '{5: {\'source\': ["pp.scatter3d(da, pos=\'position\')"]}, 7: {\'source\': {insert: '*

 * *            '[(13, "pp.scatter3d(da, x=\'x\', y=\'y\', z=\'time\', pixel_size=0.2)")], delete: '*

 * *            '[13]}}}',*

 * * "'metadata'": "{'language_info': {delete: ['version']}}"}*

```diff
@@ -75,15 +75,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "edb1a9e2-5a86-4652-b2d6-62dbf716a02c",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pp.scatter3d(da, pos='position', figsize=(550, 400))"
+                "pp.scatter3d(da, pos='position')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "951c725d-c03f-4bee-b752-b7a5700aec2a",
             "metadata": {},
             "source": [
@@ -108,15 +108,15 @@
                 "    coords={\n",
                 "        'x': sc.array(dims=['row'], unit='m', values=x),\n",
                 "        'y': sc.array(dims=['row'], unit='m', values=y),\n",
                 "        'time': sc.array(dims=['row'], unit='s', values=time),\n",
                 "    },\n",
                 ")\n",
                 "\n",
-                "pp.scatter3d(da, x='x', y='y', z='time', figsize=(550, 400), pixel_size=0.2)"
+                "pp.scatter3d(da, x='x', y='y', z='time', pixel_size=0.2)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -127,14 +127,13 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `plopp-24.2.0/docs/user-guide/plot-types/slicer-plot.ipynb` & `plopp-24.4.0/docs/user-guide/plot-types/slicer-plot.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955357142857143%*

 * *Differences: {"'metadata'": "{'language_info': {delete: ['version']}}"}*

```diff
@@ -74,14 +74,13 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `plopp-24.2.0/docs/user-guide/plot-types/super-plot.ipynb` & `plopp-24.4.0/docs/user-guide/plot-types/super-plot.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9945436507936508%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(2, 'tool = p.right_bar[0]\\n'), (3, 'b = tool.button\\n'), "*

 * *            '(4, "sl = p.bottom_bar[0].controls[\'y\'][\'slider\']\\n"), (9, \'p.children = '*

 * *            "[\\n'), (10, '    p.top_bar,\\n'), (11, '    HBox([p.left_bar, p.canvas.to_image(), "*

 * *            "p.right_bar]),\\n'), (12, '    p.bottom_bar,\\n')], delete: [12, 11, 10, 9, 8, 3, "*

 * *            '2]}}}',*

 * * "'metadata'": "{'language_info': {delete: ['version']}}"}*

```diff
@@ -53,25 +53,25 @@
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "outputs": [],
             "source": [
                 "from ipywidgets import HBox\n",
                 "\n",
-                "b = p.children[0].children[1].children[0]\n",
-                "sl = p.children[1].controls['y']['slider']\n",
+                "tool = p.right_bar[0]\n",
+                "b = tool.button\n",
+                "sl = p.bottom_bar[0].controls['y']['slider']\n",
                 "b.click()\n",
                 "sl.value = 20\n",
                 "b.click()\n",
                 "sl.value = 30\n",
-                "f = p.children[0].children[0]\n",
-                "f.children = [\n",
-                "    f.top_bar,\n",
-                "    HBox([f.left_bar, f.canvas.to_image(), f.right_bar]),\n",
-                "    f.bottom_bar,\n",
+                "p.children = [\n",
+                "    p.top_bar,\n",
+                "    HBox([p.left_bar, p.canvas.to_image(), p.right_bar]),\n",
+                "    p.bottom_bar,\n",
                 "]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "00b5ac9c-364c-4403-ba2b-7895cbc61d36",
@@ -105,14 +105,13 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.9.15"
+            "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `plopp-24.2.0/pyproject.toml` & `plopp-24.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Typing :: Typed",
 ]
 requires-python = ">=3.9"
 
 # IMPORTANT:
 # Run 'tox -e deps' after making changes here. This will update requirement files.
@@ -58,14 +59,16 @@
 testpaths = "tests"
 filterwarnings = [
   "error",
   'ignore:\n            Sentinel is not a public part of the traitlets API:DeprecationWarning',
   'ignore:Passing unrecognized arguments to super:DeprecationWarning',
   'ignore:Jupyter is migrating its paths:DeprecationWarning',
   'ignore:setDaemon\(\) is deprecated, set the daemon attribute instead:DeprecationWarning',
+  'ignore:TriCutTool is deprecated::',
+  'ignore:Cut3dTool is deprecated::',
 ]
 
 [tool.bandit]
 # Excluding tests because bandit doesn't like `assert`.
 exclude_dirs = ["docs/conf.py", "tests"]
 
 [tool.black]
```

### Comparing `plopp-24.2.0/requirements/base.txt` & `plopp-24.4.0/requirements/base.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,11 +24,11 @@
     # via matplotlib
 pillow==10.2.0
     # via matplotlib
 pyparsing==3.1.1
     # via matplotlib
 python-dateutil==2.8.2
     # via matplotlib
-scipp==23.12.0
+scipp==24.2.0
     # via -r base.in
 six==1.16.0
     # via python-dateutil
```

### Comparing `plopp-24.2.0/requirements/ci.txt` & `plopp-24.4.0/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/requirements/constraints.txt` & `plopp-24.4.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/requirements/dev.txt` & `plopp-24.4.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/requirements/docs.txt` & `plopp-24.4.0/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/requirements/make_base.py` & `plopp-24.4.0/requirements/make_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
 import sys
 from argparse import ArgumentParser
 from pathlib import Path
 from typing import List
 
 import tomli
 
@@ -39,15 +36,15 @@
         f.write("\n".join(dependencies))
         f.write("\n")
 
 
 with open("../pyproject.toml", "rb") as toml_file:
     pyproject = tomli.load(toml_file)
     dependencies = pyproject["project"].get("dependencies")
-    if not dependencies:
+    if dependencies is None:
         raise RuntimeError("No dependencies found in pyproject.toml")
     dependencies = [dep.strip().strip('"') for dep in dependencies]
 
 write_dependencies("base", dependencies)
 
 
 def as_nightly(repo: str) -> str:
```

### Comparing `plopp-24.2.0/requirements/noplotly.txt` & `plopp-24.4.0/requirements/noplotly.txt`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/requirements/optional.txt` & `plopp-24.4.0/requirements/optional.txt`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/requirements/static.txt` & `plopp-24.4.0/requirements/static.txt`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/resources/logo-plopp-2022.svg` & `plopp-24.4.0/resources/logo-plopp-2022.svg`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/__init__.py` & `plopp-24.4.0/src/plopp/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,16 +12,26 @@
 
 from .backends.manager import BackendManager
 
 backends = BackendManager()
 
 from . import data
 from .core import Node, View, node, show_graph, widget_node
-from .graphics import Camera, figure1d, figure2d, figure3d, tiled
-from .plotting import inspector, plot, scatter3d, slicer, superplot, xyplot
+from .graphics import (
+    Camera,
+    figure1d,
+    figure2d,
+    figure3d,
+    imagefigure,
+    linefigure,
+    scatter3dfigure,
+    scatterfigure,
+    tiled,
+)
+from .plotting import inspector, plot, scatter, scatter3d, slicer, superplot, xyplot
 
 del importlib
 
 
 def show():
     """
     A function to display all the currently opened figures (note that this only applies
@@ -39,18 +49,23 @@
     'Node',
     'View',
     'backends',
     'data',
     'figure1d',
     'figure2d',
     'figure3d',
+    'imagefigure',
     'inspector',
+    'linefigure',
     'node',
     'plot',
+    'scatter',
+    'scatterfigure',
     'scatter3d',
+    'scatter3dfigure',
     'show',
     'show_graph',
     'slicer',
     'superplot',
     'tiled',
     'widget_node',
     'xyplot',
```

### Comparing `plopp-24.2.0/src/plopp/backends/common.py` & `plopp-24.4.0/src/plopp/backends/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     ymin: Optional[float] = None
     ymax: Optional[float] = None
 
     def union(self, other: BoundingBox) -> BoundingBox:
         """
         Return the union of this bounding box with another one.
         """
+
         return BoundingBox(
             xmin=_none_min(self.xmin, other.xmin),
             xmax=_none_max(self.xmax, other.xmax),
             ymin=_none_min(self.ymin, other.ymin),
             ymax=_none_max(self.ymax, other.ymax),
         )
 
@@ -86,31 +87,28 @@
     dim:
         The dimension along which to extract values.
     """
     x = data.coords[dim]
     y = data.data
     hist = len(x) != len(y)
     error = None
-    mask = {'x': x.values, 'y': np.full(y.shape, np.nan), 'visible': False}
+    xvalues = np.asarray(x.values)
+    yvalues = np.asarray(y.values)
+    values = {'x': xvalues, 'y': yvalues}
+    mask = {'x': xvalues, 'y': np.full(y.shape, np.nan), 'visible': False}
     if data.variances is not None:
         error = {
-            'x': sc.midpoints(x).values if hist else x.values,
-            'y': y.values,
-            'e': sc.stddevs(y).values,
+            'x': np.asarray(sc.midpoints(x).values) if hist else xvalues,
+            'y': yvalues,
+            'e': np.asarray(sc.stddevs(y).values),
         }
     if len(data.masks):
-        one_mask = merge_masks(data.masks).values
+        one_mask = np.asarray(merge_masks(data.masks).values)
         mask = {
-            'x': x.values,
-            'y': np.where(one_mask, y.values, np.nan),
+            'x': xvalues,
+            'y': np.where(one_mask, yvalues, np.nan),
             'visible': True,
         }
     if hist:
-        y = sc.concat([y[0:1], y], dim=dim)
-        if mask is not None:
-            mask['y'] = np.concatenate([mask['y'][0:1], mask['y']])
-    return {
-        'values': {'x': x.values, 'y': y.values},
-        'stddevs': error,
-        'mask': mask,
-        'hist': hist,
-    }
+        for array in (values, mask):
+            array['y'] = np.concatenate([array['y'][0:1], array['y']])
+    return {'values': values, 'stddevs': error, 'mask': mask, 'hist': hist}
```

### Comparing `plopp-24.2.0/src/plopp/backends/manager.py` & `plopp-24.4.0/src/plopp/backends/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,21 @@
     def image(self, *args, **kwargs):
         try:
             _image = self._backends['2d'].image
         except AttributeError:
             raise ValueError(f'Unsupported backend \'{self["2d"]}\' for image (2D).')
         return _image(*args, **kwargs)
 
+    def scatter(self, *args, **kwargs):
+        try:
+            _scatter = self._backends['2d'].scatter
+        except AttributeError:
+            raise ValueError(f'Unsupported backend \'{self["2d"]}\' for scatter.')
+        return _scatter(*args, **kwargs)
+
     def point_cloud(self, *args, **kwargs):
         try:
             _point_cloud = self._backends['3d'].point_cloud
         except AttributeError:
             raise ValueError(
                 f'Unsupported backend \'{self["3d"]}\' for point_cloud (3D).'
             )
```

### Comparing `plopp-24.2.0/src/plopp/backends/matplotlib/__init__.py` & `plopp-24.4.0/src/plopp/backends/matplotlib/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,22 @@
         """
         See :class:`line.Line` for details.
         """
         from .line import Line as LineMpl
 
         return LineMpl(*args, **kwargs)
 
+    def scatter(self, *args, **kwargs):
+        """
+        See :class:`scatter.Scatter` for details.
+        """
+        from .scatter import Scatter as ScatterMpl
+
+        return ScatterMpl(*args, **kwargs)
+
     def image(self, *args, **kwargs):
         """
         See :class:`image.Image` for details.
         """
         from .image import Image as ImageMpl
 
         return ImageMpl(*args, **kwargs)
```

### Comparing `plopp-24.2.0/src/plopp/backends/matplotlib/canvas.py` & `plopp-24.4.0/src/plopp/backends/matplotlib/canvas.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,28 +2,52 @@
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 from typing import Literal, Optional, Tuple, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import scipp as sc
+from matplotlib import dates as mdates
 from matplotlib.collections import QuadMesh
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
 from ...core.utils import maybe_variable_to_number, scalar_to_string
 from ..common import BoundingBox, axis_bounds
 from .utils import fig_to_bytes, is_sphinx_build, make_figure
 
 
+def _to_floats(x: np.ndarray) -> np.ndarray:
+    return mdates.date2num(x) if np.issubdtype(x.dtype, np.datetime64) else x
+
+
 def _none_if_not_finite(x: Union[float, int, None]) -> Union[float, int, None]:
     if x is None:
         return None
     return x if np.isfinite(x) else None
 
 
+def _cursor_value_to_variable(
+    x: Union[float, int], dtype: sc.DType, unit: str
+) -> sc.Variable:
+    if dtype == sc.DType.datetime64:
+        # Annoying chain of conversion but matplotlib has its own way of converting
+        # dates to numbers (number of days since epoch), and num2date returns a python
+        # datetime object, while scipp expects a numpy datetime64.
+        return sc.scalar(np.datetime64(mdates.num2date(x).replace(tzinfo=None))).to(
+            unit=unit
+        )
+    return sc.scalar(x, unit=unit)
+
+
+def _cursor_formatter(x: Union[float, int], dtype: sc.DType, unit: str) -> str:
+    if dtype == sc.DType.datetime64:
+        return mdates.num2date(x).replace(tzinfo=None).isoformat()
+    return scalar_to_string(sc.scalar(x, unit=unit))
+
+
 class Canvas:
     """
     Matplotlib-based canvas used to render 2D graphics.
     It provides a figure and some axes, as well as functions for controlling the zoom,
     panning, and the scale of the axes.
 
     Parameters
@@ -131,31 +155,41 @@
         Convert the underlying Matplotlib figure to an image widget from ``ipywidgets``.
         """
         from ipywidgets import Image
 
         return Image(value=fig_to_bytes(self.fig), format='png')
 
     def to_widget(self):
+        from ipywidgets import Layout, VBox
+
         if self.is_widget() and not is_sphinx_build():
-            return self.fig.canvas
+            # The Matplotlib canvas tries to fill the entire width of the output cell,
+            # which can add unnecessary whitespace between it and other widgets. To
+            # prevent this, we wrap the canvas in a VBox, which seems to help.
+            widget = VBox([self.fig.canvas])
         else:
-            return self.to_image()
+            widget = self.to_image()
+        # The max_width is set to prevent overflow, see gh-169
+        widget.layout = Layout(max_width='80%', overflow='auto')
+        return widget
 
     def autoscale(self):
         """
         Find the limits of the artists on the canvas and adjust the axes ranges.
         Add some padding in the case of 1d lines.
         """
         bbox = BoundingBox()
         lines = [line for line in self.ax.lines if hasattr(line, '_plopp_mask')]
         for line in lines:
             line_mask = sc.array(dims=['x'], values=line._plopp_mask)
-            line_x = sc.DataArray(data=sc.array(dims=['x'], values=line.get_xdata()))
+            line_x = sc.DataArray(
+                data=sc.array(dims=['x'], values=_to_floats(line.get_xdata()))
+            )
             line_y = sc.DataArray(
-                data=sc.array(dims=['x'], values=line.get_ydata()),
+                data=sc.array(dims=['x'], values=_to_floats(line.get_ydata())),
                 masks={'mask': line_mask},
             )
             line_bbox = BoundingBox(
                 **{**axis_bounds(('xmin', 'xmax'), line_x, self.xscale, pad=True)},
                 **{**axis_bounds(('ymin', 'ymax'), line_y, self.yscale, pad=True)},
             )
             bbox = bbox.union(line_bbox)
@@ -235,29 +269,30 @@
 
     def show(self):
         """
         Make a call to Matplotlib's underlying ``show`` function.
         """
         self.fig.show()
 
-    def set_axes(self, dims, units):
+    def set_axes(self, dims, units, dtypes):
         """
         Set the axes dimensions and units.
 
         Parameters
         ----------
         dims:
             The dimensions of the data.
         units:
             The units of the data.
+        dtypes:
+            The data types of the data.
         """
         self.units = units
         self.dims = dims
-        self._cursor_x_placeholder = sc.scalar(0.0, unit=self.units['x'])
-        self._cursor_y_placeholder = sc.scalar(0.0, unit=self.units['y'])
+        self.dtypes = dtypes
         self._cursor_x_prefix = ''
         self._cursor_y_prefix = ''
         if 'y' in self.dims:
             self._cursor_x_prefix = self.dims['x'] + '='
             self._cursor_y_prefix = self.dims['y'] + '='
         self.ax.format_coord = self.format_coord
 
@@ -275,21 +310,32 @@
         Parameters
         ----------
         x:
             The x coordinate of the mouse pointer.
         y:
             The y coordinate of the mouse pointer.
         """
-        self._cursor_x_placeholder.value = x
-        self._cursor_y_placeholder.value = y
-        out = (
-            f"({self._cursor_x_prefix}{scalar_to_string(self._cursor_x_placeholder)}, "
-            f"{self._cursor_y_prefix}{scalar_to_string(self._cursor_y_placeholder)})"
+        xstr = _cursor_formatter(x, self.dtypes['x'], self.units['x'])
+        ystr = _cursor_formatter(y, self.dtypes['y'], self.units['y'])
+        out = f"({self._cursor_x_prefix}{xstr}, {self._cursor_y_prefix}{ystr})"
+        if not self._coord_formatters:
+            return out
+        xpos = (
+            self.dims['x'],
+            _cursor_value_to_variable(x, self.dtypes['x'], self.units['x']),
+        )
+        ypos = (
+            (
+                self.dims['y'],
+                _cursor_value_to_variable(y, self.dtypes['y'], self.units['y']),
+            )
+            if 'y' in self.dims
+            else None
         )
-        extra = [formatter(x, y) for formatter in self._coord_formatters]
+        extra = [formatter(xpos, ypos) for formatter in self._coord_formatters]
         extra = [e for e in extra if e is not None]
         if extra:
             out += ": {" + ", ".join(extra) + "}"
         return out
 
     @property
     def empty(self) -> bool:
```

### Comparing `plopp-24.2.0/src/plopp/backends/matplotlib/figure.py` & `plopp-24.4.0/src/plopp/backends/pythreejs/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,34 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-from ...graphics import BaseFig
 
-
-class Figure(BaseFig):
-    """
-    Mixin class for Matplotlib figures
-    """
-
-    def __init_figure__(self, View, *args, **kwargs):
-        self._view = View(*args, **kwargs)
-        self._args = args
-        self._kwargs = kwargs
-
-    @property
-    def fig(self):
+class PythreejsBackend:
+    def is_interactive(self):
         """
-        Get the underlying Matplotlib figure.
+        Returns ``True`` if the backend currently in use allows for interactive figures.
         """
-        return self._view.canvas.fig
+        return True
 
-    @property
-    def ax(self):
+    def canvas3d(self, *args, **kwargs):
         """
-        Get the underlying Matplotlib axes.
+        See :class:`canvas.Canvas` for details.
         """
-        return self._view.canvas.ax
+        from .canvas import Canvas as CanvasP3js
+
+        return CanvasP3js(*args, **kwargs)
 
-    @property
-    def cax(self):
+    def point_cloud(self, *args, **kwargs):
         """
-        Get the underlying Matplotlib colorbar axes.
+        See :class:`point_cloud.PointCloud` for details.
         """
-        return self._view.canvas.cax
+        from .point_cloud import PointCloud as PointCloudP3js
 
-    def __add__(self, other):
-        from .tiled import hstack
+        return PointCloudP3js(*args, **kwargs)
 
-        return hstack(self, other)
-
-    def __truediv__(self, other):
-        from .tiled import vstack
+    def figure3d(self, *args, **kwargs):
+        """
+        See :class:`figure.Figure` for details.
+        """
+        from .figure import Figure as FigP3js
 
-        return vstack(self, other)
+        return FigP3js(*args, **kwargs)
```

### Comparing `plopp-24.2.0/src/plopp/backends/matplotlib/image.py` & `plopp-24.4.0/src/plopp/backends/matplotlib/image.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import uuid
+from typing import Tuple
 
 import numpy as np
 import scipp as sc
 
 from ...core.utils import coord_as_bin_edges, merge_masks, repeat, scalar_to_string
 from .canvas import Canvas
 
@@ -128,37 +129,14 @@
         for xy, var in string_labels.items():
             getattr(self._ax, f'set_{xy}ticks')(np.arange(float(var.shape[0])))
             getattr(self._ax, f'set_{xy}ticklabels')(var.values)
 
         if need_grid:
             self._ax.grid(True)
 
-        # Cache slicing order for hover values
-        if self._dim_1d is not None:
-            # If there is a 2d coord, we first slice the 1d coord, and then the
-            # dimension that is left should also be 1d, making value-based slicing
-            # possible.
-            self._hover_slicing = {
-                'dir': (self._dim_1d[0], self._dim_2d[0]),
-                'dim': (self._dim_1d[1], self._dim_2d[1]),
-                'unit': (
-                    self._data.coords[self._dim_1d[1]].unit,
-                    self._data.coords[self._dim_2d[1]].unit,
-                ),
-            }
-        else:
-            self._hover_slicing = {
-                'dir': ('y', 'x'),
-                'dim': (self._data.dims[0], self._data.dims[1]),
-                'unit': (
-                    self._data.coords[self._data.dims[0]].unit,
-                    self._data.coords[self._data.dims[1]].unit,
-                ),
-            }
-
         self._canvas.register_format_coord(self.format_coord)
 
     @property
     def data(self):
         """
         Get the Mesh's data in a form that may have been tweaked, compared to the
         original data, in the case of a two-dimensional coordinate.
@@ -200,41 +178,29 @@
         ----------
         new_values:
             New data to update the mesh values from.
         """
         self._data = new_values
         self._data_with_bin_edges.data = new_values.data
 
-    def format_coord(self, x: float, y: float) -> str:
+    def format_coord(
+        self, xslice: Tuple[str, sc.Variable], yslice: Tuple[str, sc.Variable]
+    ) -> str:
         """
         Format the coordinates of the mouse pointer to show the value of the
         data at that point.
 
         Parameters
         ----------
-        x:
-            The x coordinate of the mouse pointer.
-        y:
-            The y coordinate of the mouse pointer.
+        xslice:
+            Dimension and x coordinate of the mouse pointer, as slice parameters.
+        yslice:
+            Dimension and y coordinate of the mouse pointer, as slice parameters.
         """
-        xy = {'x': x, 'y': y}
         try:
-            val = self._data_with_bin_edges[
-                self._hover_slicing['dim'][0],
-                sc.scalar(
-                    xy[self._hover_slicing['dir'][0]],
-                    unit=self._hover_slicing['unit'][0],
-                ),
-            ]
-            val = val[
-                self._hover_slicing['dim'][1],
-                sc.scalar(
-                    xy[self._hover_slicing['dir'][1]],
-                    unit=self._hover_slicing['unit'][1],
-                ),
-            ]
+            val = self._data_with_bin_edges[yslice][xslice]
             prefix = self._data.name
             if prefix:
                 prefix += ': '
             return prefix + scalar_to_string(val)
         except IndexError:
             return None
```

### Comparing `plopp-24.2.0/src/plopp/backends/matplotlib/interactive.py` & `plopp-24.4.0/src/plopp/backends/matplotlib/interactive.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/backends/matplotlib/line.py` & `plopp-24.4.0/src/plopp/backends/matplotlib/line.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,30 +2,25 @@
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import uuid
 from typing import Dict
 
 import numpy as np
 import scipp as sc
+from matplotlib.dates import date2num
 from matplotlib.lines import Line2D
 from numpy.typing import ArrayLike
 
 from ..common import make_line_data
 from .canvas import Canvas
+from .utils import make_legend, parse_dicts_in_kwargs
 
 
-def _parse_dicts_in_kwargs(kwargs, name):
-    out = {}
-    for key, value in kwargs.items():
-        if isinstance(value, dict):
-            if name in value:
-                out[key] = value[name]
-        else:
-            out[key] = value
-    return out
+def _to_float(x):
+    return date2num(x) if np.issubdtype(x.dtype, np.datetime64) else x
 
 
 class Line:
     """
     Artist to represent one-dimensional data.
     If the coordinate is bin centers, the line is (by default) a set of markers.
     If the coordinate is bin edges, the line is a step function.
@@ -45,15 +40,15 @@
         self._canvas = canvas
         self._ax = self._canvas.ax
         self._data = data
         # Because all keyword arguments from the figure are forwarded to both the canvas
         # and the line, we need to remove the arguments that belong to the canvas.
         kwargs.pop('ax', None)
 
-        args = _parse_dicts_in_kwargs(kwargs, name=data.name)
+        args = parse_dicts_in_kwargs(kwargs, name=data.name)
 
         self._line = None
         self._mask = None
         self._error = None
         self._unit = None
         self.label = data.name
         self._dim = self._data.dim
@@ -164,23 +159,15 @@
                 zorder=10,
                 fmt="none",
             )
             # Set the selection mask on the line collection that makes the segments
             self._error[2][0]._plopp_mask = line_mask[1:] if data["hist"] else line_mask
 
         if self.label and self._canvas._legend:
-            leg_args = {}
-            if isinstance(self._canvas._legend, (list, tuple)):
-                leg_args = {'loc': self._canvas._legend}
-            elif not isinstance(self._canvas._legend, bool):
-                raise TypeError(
-                    "Legend must be a bool, tuple, or a list, "
-                    f"not {type(self._canvas._legend)}"
-                )
-            self._ax.legend(**leg_args)
+            self._ax.legend(**make_legend(self._canvas._legend))
 
     def update(self, new_values: sc.DataArray):
         """
         Update the x and y positions of the data points from new data.
 
         Parameters
         ----------
@@ -194,17 +181,17 @@
         self._mask.set_data(new_values['mask']['x'], new_values['mask']['y'])
         self._mask.set_visible(new_values['mask']['visible'])
 
         if (self._error is not None) and (new_values['stddevs'] is not None):
             coll = self._error.get_children()[0]
             coll.set_segments(
                 self._change_segments_y(
-                    new_values['stddevs']['x'],
-                    new_values['stddevs']['y'],
-                    new_values['stddevs']['e'],
+                    _to_float(new_values['stddevs']['x']),
+                    _to_float(new_values['stddevs']['y']),
+                    _to_float(new_values['stddevs']['e']),
                 )
             )
 
     def _change_segments_y(self, x: ArrayLike, y: ArrayLike, e: ArrayLike) -> ArrayLike:
         """
         Update the positions of the errorbars when `update_data` is called.
         """
```

### Comparing `plopp-24.2.0/src/plopp/backends/matplotlib/static.py` & `plopp-24.4.0/src/plopp/backends/matplotlib/static.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/backends/matplotlib/tiled.py` & `plopp-24.4.0/src/plopp/backends/matplotlib/tiled.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/backends/matplotlib/utils.py` & `plopp-24.4.0/src/plopp/backends/matplotlib/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 from io import BytesIO
-from typing import Literal
+from typing import Literal, Tuple, Union
 
 import matplotlib as mpl
 from matplotlib.pyplot import Figure, _get_backend_mod
 
 from ..protocols import FigureLike
 
 
@@ -52,14 +52,26 @@
     if not is_interactive_backend():
         return Figure(*args, **kwargs)
     backend = _get_backend_mod()
     manager = backend.new_figure_manager(1, *args, FigureClass=Figure, **kwargs)
     return manager.canvas.figure
 
 
+def make_legend(leg: Union[bool, Tuple[float, float]]):
+    """
+    Create a dict of arguments to be used in the legend creation.
+    """
+    leg_args = {}
+    if isinstance(leg, (list, tuple)):
+        leg_args = {'loc': leg}
+    elif not isinstance(leg, bool):
+        raise TypeError(f"Legend must be a bool, tuple, or a list, not {type(leg)}")
+    return leg_args
+
+
 def require_interactive_backend(func: str):
     """
     Raise an error if the current backend in use is non-interactive.
     """
     if not is_interactive_backend():
         raise RuntimeError(
             f"The {func} can only be used with the interactive widget "
@@ -106,7 +118,18 @@
         fig._view.__class__,
         *fig._args,
         **{**fig._kwargs, **kwargs},
     )
     for prop in ('xrange', 'yrange', 'xscale', 'yscale', 'title', 'grid'):
         setattr(out.canvas, prop, getattr(fig.canvas, prop))
     return out
+
+
+def parse_dicts_in_kwargs(kwargs, name):
+    out = {}
+    for key, value in kwargs.items():
+        if isinstance(value, dict):
+            if name in value:
+                out[key] = value[name]
+        else:
+            out[key] = value
+    return out
```

### Comparing `plopp-24.2.0/src/plopp/backends/plotly/__init__.py` & `plopp-24.4.0/src/plopp/backends/plotly/__init__.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/backends/plotly/canvas.py` & `plopp-24.4.0/src/plopp/backends/plotly/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,27 +147,30 @@
         """
         ext = filename.split('.')[-1]
         if ext == 'html':
             self.fig.write_html(filename)
         else:
             self.fig.write_image(filename)
 
-    def set_axes(self, dims, units):
+    def set_axes(self, dims, units, dtypes):
         """
         Set the axes dimensions and units.
 
         Parameters
         ----------
         dims:
             The dimensions of the data.
         units:
             The units of the data.
+        dtypes:
+            The data types of the data.
         """
-        self.units = units
         self.dims = dims
+        self.units = units
+        self.dtypes = dtypes
 
     @property
     def empty(self) -> bool:
         """
         Check if the canvas is empty.
         """
         return not self.dims
```

### Comparing `plopp-24.2.0/src/plopp/backends/plotly/figure.py` & `plopp-24.4.0/src/plopp/backends/plotly/figure.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/backends/plotly/line.py` & `plopp-24.4.0/src/plopp/backends/plotly/line.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/backends/protocols.py` & `plopp-24.4.0/src/plopp/backends/protocols.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/backends/pythreejs/canvas.py` & `plopp-24.4.0/src/plopp/backends/pythreejs/canvas.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,29 +60,34 @@
             scene=self.scene,
             controls=[self.controls],
             width=width,
             height=height,
         )
 
     def to_widget(self):
+        # The max_width is set to prevent overflow, see gh-169
+        self.renderer.layout = ipw.Layout(max_width='80%', overflow='auto')
         return self.renderer
 
-    def set_axes(self, dims, units):
+    def set_axes(self, dims, units, dtypes):
         """
         Set the axes dimensions and units.
 
         Parameters
         ----------
         dims:
             The dimensions of the data.
         units:
             The units of the data.
+        dtypes:
+            The data types of the data.
         """
         self.units = units
         self.dims = dims
+        self.dtypes = dtypes
 
     def make_outline(self, limits: Tuple[sc.Variable, sc.Variable, sc.Variable]):
         """
         Create an outline box with ticklabels, given a range in the XYZ directions.
         """
         from .outline import Outline
```

### Comparing `plopp-24.2.0/src/plopp/backends/pythreejs/outline.py` & `plopp-24.4.0/src/plopp/backends/pythreejs/outline.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/backends/pythreejs/point_cloud.py` & `plopp-24.4.0/src/plopp/backends/pythreejs/point_cloud.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/core/graph.py` & `plopp-24.4.0/src/plopp/core/graph.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/core/helpers.py` & `plopp-24.4.0/src/plopp/core/helpers.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/core/limits.py` & `plopp-24.4.0/src/plopp/core/limits.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/core/node.py` & `plopp-24.4.0/src/plopp/core/node.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/core/typing.py` & `plopp-24.4.0/src/plopp/core/typing.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/core/utils.py` & `plopp-24.4.0/src/plopp/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,17 +167,18 @@
     Parameters
     ----------
     var:
         The input scalar.
     precision:
         The number of decimal places to use for the string output.
     """
-    return value_to_string(var.value, precision=precision) + (
-        f" {var.unit}" if var.unit not in (None, "") else ""
-    )
+    out = value_to_string(var.value, precision=precision)
+    if (var.unit not in (None, "")) and var.dtype != sc.DType.datetime64:
+        out += f" {var.unit}"
+    return out
 
 
 def merge_masks(masks: Dict[str, sc.Variable]) -> sc.Variable:
     """
     Combine all masks into a single one using the OR operation.
 
     Parameters
```

### Comparing `plopp-24.2.0/src/plopp/data/examples.py` & `plopp-24.4.0/src/plopp/data/examples.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/data/factory.py` & `plopp-24.4.0/src/plopp/data/factory.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/graphics/basefig.py` & `plopp-24.4.0/src/plopp/backends/matplotlib/figure.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
+from ...graphics import BaseFig
 
-from ..core import View
 
-
-class BaseFig:
+class Figure(BaseFig):
     """
-    A Mixin class which is the base for all figures.
+    Mixin class for Matplotlib figures
     """
 
-    _view: View
-
-    @property
-    def canvas(self):
-        return self._view.canvas
+    def __init_figure__(self, View, *args, **kwargs):
+        self._view = View(*args, **kwargs)
+        self._args = args
+        self._kwargs = kwargs
 
     @property
-    def artists(self):
-        return self._view.artists
+    def fig(self):
+        """
+        Get the underlying Matplotlib figure.
+        """
+        return self._view.canvas.fig
 
     @property
-    def graph_nodes(self):
-        return self._view.graph_nodes
+    def ax(self):
+        """
+        Get the underlying Matplotlib axes.
+        """
+        return self._view.canvas.ax
 
     @property
-    def id(self):
-        return self._view.id
+    def cax(self):
+        """
+        Get the underlying Matplotlib colorbar axes.
+        """
+        return self._view.canvas.cax
 
     def save(self, filename, **kwargs):
         """
         Save the figure to file.
         The default directory for writing the file is the same as the
         directory where the script or notebook is running.
 
@@ -38,12 +45,16 @@
         ----------
         filename:
             Name of the output file. Possible file extensions are ``.jpg``, ``.png``,
             ``.svg``, and ``.pdf``.
         """
         return self._view.canvas.save(filename, **kwargs)
 
-    def update(self, *args, **kwargs):
-        return self._view.update(*args, **kwargs)
+    def __add__(self, other):
+        from .tiled import hstack
+
+        return hstack(self, other)
+
+    def __truediv__(self, other):
+        from .tiled import vstack
 
-    def notify_view(self, *args, **kwargs):
-        return self._view.notify_view(*args, **kwargs)
+        return vstack(self, other)
```

### Comparing `plopp-24.2.0/src/plopp/graphics/camera.py` & `plopp-24.4.0/src/plopp/graphics/camera.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/graphics/colormapper.py` & `plopp-24.4.0/src/plopp/graphics/colormapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import scipp as sc
 from matplotlib.colorbar import ColorbarBase
 from matplotlib.colors import Colormap, LinearSegmentedColormap, LogNorm, Normalize
 
 from ..backends.matplotlib.utils import fig_to_bytes
 from ..core.limits import find_limits, fix_empty_range
 from ..core.utils import maybe_variable_to_number, merge_masks
+from .common import args_to_update
 
 
 def _get_cmap(name: str, nan_color: str = None) -> Colormap:
     """
     Get a colormap object from a colormap name.
 
     Parameters
@@ -223,54 +224,50 @@
         if self.vmin >= self.normalizer.vmax:
             self.normalizer.vmax = self.vmax
             self.normalizer.vmin = self.vmin
         else:
             self.normalizer.vmin = self.vmin
             self.normalizer.vmax = self.vmax
 
-    def update(self, key: str, data: sc.DataArray):
+    def update(self, *args, **kwargs):
         """
-        Update the colorscale bounds taking into account new values.
+        Update the colorscale bounds taking into account new values,
+        by either supplying a dictionary of new data or by keyword arguments.
         We also update the colorbar widget if it exists.
-
-        Parameters
-        ----------
-        data:
-            The data array to use to update the colorscale range.
-        key:
-            The id of the node that provided this data.
-        """
-        if self.name is None:
-            self.name = data.name
-            # If name is None, this is the first time update is called
-            if self.user_vmin is not None:
-                self.user_vmin = maybe_variable_to_number(
-                    self.user_vmin, unit=self.unit
-                )
-            if self.user_vmax is not None:
-                self.user_vmax = maybe_variable_to_number(
-                    self.user_vmax, unit=self.unit
-                )
-        elif data.name != self.name:
-            self.name = ''
-        if self.cax is not None:
-            text = self.name
-            if self.unit is not None:
-                text += f'{" " if self.name else ""}[{self.unit}]'
-            self.cax.set_ylabel(text)
-        old_bounds = np.array([self.vmin, self.vmax])
-        self.autoscale()
-        self._set_normalizer_limits()
-
-        if not np.allclose(old_bounds, np.array([self.vmin, self.vmax])):
-            self._update_colorbar_widget()
-            keys = self.artists.keys()
-        else:
-            keys = [key]
-        self._set_artists_colors(keys)
+        """
+        new = args_to_update(*args, **kwargs)
+        for key, data in new.items():
+            if self.name is None:
+                self.name = data.name
+                # If name is None, this is the first time update is called
+                if self.user_vmin is not None:
+                    self.user_vmin = maybe_variable_to_number(
+                        self.user_vmin, unit=self.unit
+                    )
+                if self.user_vmax is not None:
+                    self.user_vmax = maybe_variable_to_number(
+                        self.user_vmax, unit=self.unit
+                    )
+            elif data.name != self.name:
+                self.name = ''
+            if self.cax is not None:
+                text = self.name
+                if self.unit is not None:
+                    text += f'{" " if self.name else ""}[{self.unit}]'
+                self.cax.set_ylabel(text)
+            old_bounds = np.array([self.vmin, self.vmax])
+            self.autoscale()
+            self._set_normalizer_limits()
+
+            if not np.allclose(old_bounds, np.array([self.vmin, self.vmax])):
+                self._update_colorbar_widget()
+                keys = self.artists.keys()
+            else:
+                keys = [key]
+            self._set_artists_colors(keys)
 
     def toggle_norm(self):
         """
         Toggle the norm flag, between `linear` and `log`.
         """
         self.norm = "log" if self.norm == 'linear' else 'linear'
         self.normalizer = _get_normalizer(self.norm)
```

### Comparing `plopp-24.2.0/src/plopp/graphics/figure.py` & `plopp-24.4.0/src/plopp/graphics/figure.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 from typing import Literal
 
 from .. import backends
+from ..utils import deprecated
 
 
+@deprecated('Use ``linefigure`` instead.')
 def figure1d(*args, style: Literal['line'] = 'line', **kwargs):
     """
     Create a figure to represent one-dimensional data from one or more graph node(s).
     By default, this will return a figure built from :class:`LineView` (see the
     documentation of this class for a list of available customization arguments).
 
+    .. deprecated:: v24.04.0
+
     Parameters
     ----------
     style:
         The type of figure to create.
 
     Examples
     --------
@@ -44,20 +48,23 @@
         from .lineview import LineView
 
         return backends.figure1d(LineView, *args, **kwargs)
 
     raise ValueError(f'Unsupported style={style} for figure1d.')
 
 
+@deprecated('Use ``imagefigure`` instead.')
 def figure2d(*args, style: Literal['image'] = 'image', **kwargs):
     """
     Create a figure to represent two-dimensional data from a graph node.
     By default, this will return a figure built from :class:`ImageView` (see the
     documentation of this class for a list of available customization arguments).
 
+    .. deprecated:: v24.04.0
+
     Parameters
     ----------
     style:
         The type of figure to create.
 
     Examples
     --------
@@ -78,20 +85,23 @@
         from .imageview import ImageView
 
         return backends.figure2d(ImageView, *args, **kwargs)
 
     raise ValueError(f'Unsupported style={style} for figure2d.')
 
 
+@deprecated('Use ``scatter3dfigure`` instead.')
 def figure3d(*args, style: Literal['scatter'] = 'scatter', **kwargs):
     """
     Create a figure to represent three-dimensional data from a graph node.
     By default, this will return a figure built from :class:`FigScatter3d` (see the
     documentation of this class for a list of available customization arguments).
 
+    .. deprecated:: v24.04.0
+
     Parameters
     ----------
     style:
         The type of figure to create.
 
     Examples
     --------
```

### Comparing `plopp-24.2.0/src/plopp/graphics/scatter3dview.py` & `plopp-24.4.0/src/plopp/graphics/scatter3dview.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 from typing import Literal, Optional, Tuple, Union
 
 import scipp as sc
 
 from .. import backends
 from ..core import View
 from ..core.utils import make_compatible
-from ..graphics import Camera
+from .camera import Camera
 from .colormapper import ColorMapper
+from .common import args_to_update
 
 
 class Scatter3dView(View):
     """
     View that makes a visual representation of three-dimensional scatter data.
     It has a :class:`Canvas`, a :class:`ColorMapper` and a specialized ``update``
     function that generates :class:`PointCloud` artists.
@@ -86,53 +87,54 @@
             nan_color="#f0f0f0",
             figsize=self.canvas.figsize,
         )
 
         self._original_artists = [n.id for n in nodes]
         self.render()
 
-    def update(self, new_values: sc.DataArray, key: str):
+    def update(self, *args, **kwargs):
         """
-        Add new point cloud or update point cloud array with new values.
-
-        Parameters
-        ----------
-        new_values:
-            New data to create or update a :class:`PointCloud` object from.
-        key:
-            The id of the node that sent the new data.
+        Update the view with new point clouds by either supplying a dictionary of
+        new data or by keyword arguments.
         """
+        new = args_to_update(*args, **kwargs)
         mapping = {'x': self._x, 'y': self._y, 'z': self._z}
-        if self.canvas.empty:
-            self.canvas.set_axes(
-                dims=mapping,
-                units={x: new_values.coords[dim].unit for x, dim in mapping.items()},
-            )
-            self.colormapper.unit = new_values.unit
-        else:
-            new_values.data = make_compatible(
-                new_values.data, unit=self.colormapper.unit
-            )
-            for xyz, dim in mapping.items():
-                new_values.coords[dim] = new_values.coords[dim].to(
-                    unit=self.canvas.units[xyz], copy=False
+        for key, new_values in new.items():
+            if self.canvas.empty:
+                self.canvas.set_axes(
+                    dims=mapping,
+                    units={
+                        x: new_values.coords[dim].unit for x, dim in mapping.items()
+                    },
+                    dtypes={
+                        x: new_values.coords[dim].dtype for x, dim in mapping.items()
+                    },
                 )
+                self.colormapper.unit = new_values.unit
+            else:
+                new_values.data = make_compatible(
+                    new_values.data, unit=self.colormapper.unit
+                )
+                for xyz, dim in mapping.items():
+                    new_values.coords[dim] = new_values.coords[dim].to(
+                        unit=self.canvas.units[xyz], copy=False
+                    )
+
+            if key not in self.artists:
+                pts = backends.point_cloud(
+                    data=new_values, x=self._x, y=self._y, z=self._z, **self._kwargs
+                )
+                self.artists[key] = pts
+                self.colormapper[key] = pts
+                self.canvas.add(pts.points)
+                if key in self._original_artists:
+                    self.canvas.make_outline(limits=self.get_limits())
 
-        if key not in self.artists:
-            pts = backends.point_cloud(
-                data=new_values, x=self._x, y=self._y, z=self._z, **self._kwargs
-            )
-            self.artists[key] = pts
-            self.colormapper[key] = pts
-            self.canvas.add(pts.points)
-            if key in self._original_artists:
-                self.canvas.make_outline(limits=self.get_limits())
-
-        self.artists[key].update(new_values=new_values)
-        self.colormapper.update(key=key, data=new_values)
+            self.artists[key].update(new_values=new_values)
+        self.colormapper.update(**new)
 
     def get_limits(self) -> Tuple[sc.Variable, sc.Variable, sc.Variable]:
         """
         Get global limits for all the point clouds in the scene.
         """
         xmin = None
         xmax = None
@@ -179,7 +181,31 @@
         Parameters
         ----------
         key:
             The id of the object to be removed.
         """
         self.canvas.remove(self.artists[key].points)
         del self.artists[key]
+
+
+def scatter3dfigure(*args, **kwargs):
+    """
+    Create a figure to represent three-dimensional data from one or more graph node(s).
+
+    .. versionadded:: 24.04.0
+
+    Examples
+    --------
+    Create an input node and attach a ``scatter3dfigure`` as a view:
+
+      >>> da = pp.data.scatter()
+      >>> in_node = pp.Node(da)
+      >>> fig = pp.scatter3dfigure(in_node)
+
+    With a customization argument to make the color scale logarithmic:
+
+      >>> da = pp.data.scatter()
+      >>> in_node = pp.Node(da)
+      >>> fig = pp.scatter3dfigure(in_node, norm='log')
+    """
+
+    return backends.figure3d(Scatter3dView, *args, **kwargs)
```

### Comparing `plopp-24.2.0/src/plopp/graphics/tiled.py` & `plopp-24.4.0/src/plopp/graphics/tiled.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/plotting/common.py` & `plopp-24.4.0/src/plopp/plotting/common.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/plotting/inspector.py` & `plopp-24.4.0/src/plopp/plotting/inspector.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Dict, Literal
 
 import scipp as sc
 
 from ..core import Node
 from ..core.typing import Plottable
 from ..core.utils import coord_as_bin_edges
-from ..graphics import figure1d, figure2d
+from ..graphics import imagefigure, linefigure
 from .common import preprocess, require_interactive_backend
 
 
 def _to_bin_edges(da: sc.DataArray, dim: str) -> sc.DataArray:
     """
     Convert dimension coords to bin edges.
     """
@@ -88,16 +88,16 @@
             'The inspector plot currently only works with '
             f'three-dimensional data, found {data.ndim} dims.'
         )
     if dim is None:
         dim = data.dims[-1]
     bin_edges_node = Node(_to_bin_edges, in_node, dim=dim)
     op_node = Node(_apply_op, da=bin_edges_node, op=operation, dim=dim)
-    f2d = figure2d(op_node, **kwargs)
-    f1d = figure1d()
+    f2d = imagefigure(op_node, **kwargs)
+    f1d = linefigure()
 
     from ..widgets import Box, PointsTool
 
     pts = PointsTool(
         figure=f2d,
         input_node=bin_edges_node,
         func=_slice_xy,
```

### Comparing `plopp-24.2.0/src/plopp/plotting/plot.py` & `plopp-24.4.0/src/plopp/plotting/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from functools import partial
 from typing import Dict, List, Literal, Optional, Tuple, Union
 
 from scipp import Variable
 
 from ..core.typing import PlottableMulti
-from ..graphics import figure1d, figure2d
+from ..graphics import imagefigure, linefigure
 from .common import input_to_nodes, preprocess, raise_multiple_inputs_for_2d_plot_error
 
 
 def plot(
     obj: PlottableMulti,
     *,
     aspect: Literal['auto', 'equal'] = 'auto',
@@ -111,25 +111,25 @@
     if len(ndims) > 1:
         raise ValueError(
             'All items given to the plot function must have the same '
             f'number of dimensions. Found dimensions {ndims}.'
         )
     ndim = ndims.pop()
     if ndim == 1:
-        return figure1d(
+        return linefigure(
             *nodes,
             errorbars=errorbars,
             mask_color=mask_color,
             legend=legend,
             **common_args,
         )
     elif ndim == 2:
         if len(nodes) > 1:
             raise_multiple_inputs_for_2d_plot_error(origin='plot')
-        return figure2d(
+        return imagefigure(
             *nodes,
             aspect=aspect,
             cbar=cbar,
             **common_args,
         )
     else:
         raise ValueError(
```

### Comparing `plopp-24.2.0/src/plopp/plotting/scatter3d.py` & `plopp-24.4.0/src/plopp/plotting/scatter3d.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,36 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import uuid
 from functools import partial
-from typing import Dict, Literal, Optional, Tuple, Union
+from typing import Literal, Optional, Tuple, Union
 
 import scipp as sc
 
 from ..core.typing import PlottableMulti
 from ..graphics import Camera
 from .common import check_not_binned, from_compatible_lib, input_to_nodes
 
 
-def _to_variable(
-    var: Union[str, sc.Variable], coords: Dict[str, sc.Variable]
-) -> sc.Variable:
-    return coords[var] if isinstance(var, str) else var
-
-
 def _preprocess_scatter(
     obj: PlottableMulti,
-    x: Union[str, sc.Variable],
-    y: Union[str, sc.Variable],
-    z: Union[str, sc.Variable],
-    pos: Union[str, sc.Variable],
+    x: str,
+    y: str,
+    z: str,
+    pos: Optional[str],
     name: Optional[str] = None,
 ) -> sc.DataArray:
     da = from_compatible_lib(obj)
     check_not_binned(da)
 
     if pos is not None:
-        pos = _to_variable(pos, coords=da.coords)
-        coords = {
-            x: pos.fields.x,
-            y: pos.fields.y,
-            z: pos.fields.z,
-        }
+        coords = {k: getattr(da.coords[pos].fields, k) for k in (x, y, z)}
     else:
-        coords = {k: _to_variable(k, coords=da.coords) for k in (x, y, z)}
+        coords = {k: da.coords[k] for k in (x, y, z)}
 
     out = sc.DataArray(data=da.data, masks=da.masks, coords=coords)
     if out.ndim != 1:
         out = out.flatten(to=uuid.uuid4().hex)
     if name is not None:
         out.name = name
     return out
@@ -102,42 +91,43 @@
         Initial camera configuration (position, target).
 
     Returns
     -------
     :
         A three-dimensional interactive scatter plot.
     """
-    from ..graphics import figure3d
-    from ..widgets import Box, ToggleTool, TriCutTool
+    from ..graphics import scatter3dfigure
+    from ..widgets import ClippingPlanes, ToggleTool
 
     if 'ax' in kwargs:
         raise ValueError(
             'Keyword "ax" detected. Embedding 3D scatter plots inside Matplotlib axes '
             'is not supported. See '
             'https://scipp.github.io/plopp/customization/subplots.html#FAQ:-subplots-with-3D-scatter-plots'  # noqa: E501
         )
 
     nodes = input_to_nodes(
         obj, processor=partial(_preprocess_scatter, x=x, y=y, z=z, pos=pos)
     )
 
-    fig = figure3d(
+    fig = scatter3dfigure(
         *nodes,
         x=x,
         y=y,
         z=z,
         figsize=figsize,
         norm=norm,
         title=title,
         vmin=vmin,
         vmax=vmax,
         cmap=cmap,
         camera=camera,
         **kwargs,
     )
-    tri_cutter = TriCutTool(fig)
+    clip_planes = ClippingPlanes(fig)
     fig.toolbar['cut3d'] = ToggleTool(
-        callback=tri_cutter.toggle_visibility,
-        icon='cube',
+        callback=clip_planes.toggle_visibility,
+        icon='layer-group',
         tooltip='Hide/show spatial cutting tool',
     )
-    return Box([fig, tri_cutter])
+    fig.bottom_bar.add(clip_planes)
+    return fig
```

### Comparing `plopp-24.2.0/src/plopp/plotting/slicer.py` & `plopp-24.4.0/src/plopp/plotting/slicer.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from itertools import groupby
 from typing import List, Literal, Optional, Union
 
 from scipp.typing import VariableLike
 
 from ..core import widget_node
 from ..core.typing import PlottableMulti
-from ..graphics import figure1d, figure2d
+from ..graphics import imagefigure, linefigure
 from .common import (
     input_to_nodes,
     preprocess,
     raise_multiple_inputs_for_2d_plot_error,
     require_interactive_backend,
 )
 
@@ -121,31 +121,29 @@
             nodes[0](), dims=[dim for dim in dims if dim not in keep]
         )
         self.slider_node = widget_node(self.slider)
         self.slice_nodes = [slice_dims(node, self.slider_node) for node in nodes]
 
         ndims = len(keep)
         if ndims == 1:
-            make_figure = figure1d
+            make_figure = linefigure
         elif ndims == 2:
             if len(self.slice_nodes) > 1:
                 raise_multiple_inputs_for_2d_plot_error(origin='slicer')
-            make_figure = figure2d
+            make_figure = imagefigure
         else:
             raise ValueError(
                 f'Slicer plot: the number of dims to be kept must be 1 or 2, '
                 f'but {ndims} were requested.'
             )
+
         self.figure = make_figure(
-            *self.slice_nodes,
-            autoscale=autoscale,
-            vmin=vmin,
-            vmax=vmax,
-            **kwargs,
+            *self.slice_nodes, autoscale=autoscale, vmin=vmin, vmax=vmax, **kwargs
         )
+        self.figure.bottom_bar.add(self.slider)
 
 
 def slicer(
     obj: PlottableMulti,
     *,
     keep: List[str] = None,
     autoscale: Literal['auto', 'grow', 'fixed'] = 'auto',
@@ -177,26 +175,18 @@
         If supplied, use these coords instead of the input's dimension coordinates.
     vmin:
         The minimum value of the y-axis (1d plots) or color range (2d plots).
     vmax:
         The maximum value of the y-axis (1d plots) or color range (2d plots).
     **kwargs:
         See :py:func:`plopp.plot` for the full list of figure customization arguments.
-
-    Returns
-    -------
-    :
-        A :class:`Box` which will contain a :class:`Figure` and slider widgets.
     """
     require_interactive_backend('slicer')
-    sl = Slicer(
+    return Slicer(
         obj,
         keep=keep,
         autoscale=autoscale,
         vmin=vmin,
         vmax=vmax,
         coords=coords,
         **kwargs,
-    )
-    from ..widgets import Box
-
-    return Box([sl.figure, sl.slider])
+    ).figure
```

### Comparing `plopp-24.2.0/src/plopp/plotting/xyplot.py` & `plopp-24.4.0/src/plopp/plotting/xyplot.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from typing import Union
 
 import scipp as sc
 from numpy import ndarray
 
 from ..core import Node
-from ..graphics import figure1d
+from ..graphics import linefigure
 from .common import to_variable
 
 
 def _make_data_array(x: sc.Variable, y: sc.Variable) -> sc.DataArray:
     """
     Make a data array from the supplied variables, using ``x`` as the coordinate and
     ``y`` as the data.
@@ -47,8 +47,8 @@
         See :py:func:`plopp.plot`.
     """
     x = Node(to_variable, x)
     y = Node(to_variable, y)
     dim = x().dim
     if dim != y().dim:
         raise sc.DimensionError("Dimensions of x and y must match")
-    return figure1d(Node(_make_data_array, x=x, y=y), **kwargs)
+    return linefigure(Node(_make_data_array, x=x, y=y), **kwargs)
```

### Comparing `plopp-24.2.0/src/plopp/widgets/box.py` & `plopp-24.4.0/src/plopp/widgets/box.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/widgets/checkboxes.py` & `plopp-24.4.0/src/plopp/widgets/checkboxes.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/widgets/cut3d.py` & `plopp-24.4.0/src/plopp/widgets/cut3d.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,83 +1,38 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-import asyncio
+
 from functools import partial
-from typing import Any, Callable, Dict, Literal, Tuple
+from typing import Any, Dict, Literal, Tuple
 
 import ipywidgets as ipw
 import numpy as np
 import scipp as sc
 
 from ..core import View, node
+from ..utils import deprecated
+from .debounce import debounce
 from .style import BUTTON_LAYOUT
 from .tools import PlusMinusTool
 
 
-class Timer:
-    """
-    From:
-    https://ipywidgets.readthedocs.io/en/8.0.2/examples/Widget%20Events.html#Debouncing
-    """
-
-    def __init__(self, timeout: float, callback: Callable):
-        self._timeout = timeout
-        self._callback = callback
-
-    async def _job(self):
-        await asyncio.sleep(self._timeout)
-        self._callback()
-
-    def start(self):
-        self._task = asyncio.ensure_future(self._job())
-
-    def cancel(self):
-        self._task.cancel()
-
-
-def debounce(wait: float):
-    """
-    Decorator that will postpone a function's
-    execution until after `wait` seconds
-    have elapsed since the last time it was invoked.
-
-    From:
-    https://ipywidgets.readthedocs.io/en/8.0.2/examples/Widget%20Events.html#Debouncing
-    """
-
-    def decorator(fn: Callable):
-        timer = None
-
-        def debounced(*args, **kwargs):
-            nonlocal timer
-
-            def call_it():
-                fn(*args, **kwargs)
-
-            if timer is not None:
-                timer.cancel()
-            timer = Timer(wait, call_it)
-            timer.start()
-
-        return debounced
-
-    return decorator
-
-
+@deprecated("Use ``Clip3dTool`` instead.")
 class Cut3dTool(ipw.HBox):
     """
     A tool that provides a slider to extract a plane of points in a three-dimensional
     scatter plot, and add it to the scene as an opaque cut. The slider controls the
     position of the slice. When the slider is dragged, the red outline of the cut is
     moved at the same time, while the actual point cloud gets updated less frequently
     using a debounce mechanism.
 
     The tool also has two buttons +/- to increase/decrease the thickness of the cut.
 
+    .. deprecated:: v24.04.0
+
     Parameters
     ----------
     view:
         The 3d figure that contains the point clouds to be cut.
     limits:
         The spatial extent of the points in the 3d figure in the XYZ directions.
     direction:
@@ -217,16 +172,15 @@
             )
             pos = sc.scalar(self.slider.value, unit=self._unit)
             selection = sc.abs(da.coords[self._dim] - pos) < delta
             if selection.sum().value > 0:
                 self.select_nodes[n.id] = node(partial(select, s=selection))(da=n)
                 self.select_nodes[n.id].add_view(self._view)
                 self._view.update(
-                    self.select_nodes[n.id].request_data(),
-                    key=self.select_nodes[n.id].id,
+                    {self.select_nodes[n.id].id: self.select_nodes[n.id].request_data()}
                 )
 
     def _remove_cut(self):
         """
         Remove a cut point the scene.
         """
         for n in self.select_nodes.values():
@@ -264,19 +218,22 @@
         Decrease the thickness of the cut.
         """
         self.thickness = max(self.thickness - self._thickness_step, 0)
         self._remove_cut()
         self._add_cut()
 
 
+@deprecated("Use ``ClippingPlanes`` instead.")
 class TriCutTool(ipw.HBox):
     """
     A collection of :class:`Cut3dTool` to make spatial cuts in the X, Y, and Z
     directions on a three-dimensional scatter plot.
 
+    .. deprecated:: v24.04.0
+
     Parameters
     ----------
     fig:
         The 3d figure that contains the point clouds to be cut.
     """
 
     def __init__(self, fig: View):
```

### Comparing `plopp-24.2.0/src/plopp/widgets/drawing.py` & `plopp-24.4.0/src/plopp/widgets/drawing.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         self._draw_nodes[nodeid] = draw_node
         artist.nodeid = nodeid
         output_node = node(self._func)(self._input_node, draw_node)
         output_node.name = f'Output node {len(self._output_nodes)}'
         self._output_nodes[nodeid] = output_node
         if self._destination_is_fig:
             output_node.add_view(self._destination._view)
-            self._destination.update(new_values=output_node(), key=output_node.id)
+            self._destination.update({output_node.id: output_node()})
             self._destination.artists[output_node.id].color = (
                 artist.color if hasattr(artist, 'color') else artist.edgecolor
             )
         elif isinstance(self._destination, Node):
             self._destination.add_parents(output_node)
             self._destination.notify_children(artist)
```

### Comparing `plopp-24.2.0/src/plopp/widgets/slice.py` & `plopp-24.4.0/src/plopp/widgets/slice.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/widgets/toolbar.py` & `plopp-24.4.0/src/plopp/widgets/toolbar.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/src/plopp/widgets/tools.py` & `plopp-24.4.0/src/plopp/widgets/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,22 +166,22 @@
 SaveTool = partial(ButtonTool, icon='save', tooltip='Save figure')
 """Save figure to png tool."""
 
 CameraTool = partial(ButtonTool, icon='camera', tooltip='Autoscale view')
 """Tool for changing the position of the camera in a 3d scene."""
 
 OutlineTool = partial(
-    ToggleTool, value=True, icon='codepen', tooltip='Toggle outline visibility'
+    ToggleTool, value=True, icon='cube', tooltip='Toggle outline visibility'
 )
 """Toggle outline visibility tool"""
 
 AxesTool = partial(
     ToggleTool,
     value=True,
-    description='\u27C0',
+    icon='ruler-combined',
     style={'font_weight': 'bold'},
     tooltip='Toggle visibility of XYZ axes',
 )
 """Toggle RGB axes helper visibility tool"""
 
 
 class PanZoomTool(MultiToggleTool):
```

### Comparing `plopp-24.2.0/src/plopp.egg-info/PKG-INFO` & `plopp-24.4.0/src/plopp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plopp
-Version: 24.2.0
+Version: 24.4.0
 Summary: Visualization library for Scipp
 Author: Scipp contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Scipp contributors (https://github.com/scipp)
         All rights reserved.
         
@@ -41,14 +41,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.5
 Provides-Extra: scipp
```

### Comparing `plopp-24.2.0/src/plopp.egg-info/SOURCES.txt` & `plopp-24.4.0/src/plopp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 tox.ini
 .github/dependabot.yml
 .github/workflows/ci.yml
+.github/workflows/copier.yml
 .github/workflows/docs.yml
 .github/workflows/nightly_at_main.yml
 .github/workflows/nightly_at_release.yml
 .github/workflows/python-version-ci
 .github/workflows/release.yml
 .github/workflows/test.yml
 .github/workflows/unpinned.yml
 conda/meta.yaml
-docs/_typehints.py
 docs/conf.py
 docs/index.md
 docs/_static/anaconda-icon.js
 docs/_static/circle-exclamation.svg
 docs/_static/favicon.ico
 docs/_static/logo-dark.svg
 docs/_static/logo.svg
@@ -34,14 +34,15 @@
 docs/_static/gallery/README.txt
 docs/_static/gallery/peeling-layers-thumbnail.png
 docs/_static/gallery/scatter3d-with-slider-thumbnail.png
 docs/_static/gallery/scatter3d-with-threshold-thumbnail.png
 docs/_static/plot-types/image-plot.png
 docs/_static/plot-types/inspector-plot.png
 docs/_static/plot-types/line-plot.png
+docs/_static/plot-types/scatter-plot.png
 docs/_static/plot-types/scatter3d-plot.png
 docs/_static/plot-types/slicer-plot.png
 docs/_static/plot-types/super-plot.png
 docs/_templates/class-template.rst
 docs/_templates/doc_version.html
 docs/_templates/module-template.rst
 docs/_templates/scipp-class-template.rst
@@ -61,26 +62,28 @@
 docs/gallery/nyc-taxi.ipynb
 docs/gallery/peeling-layers.ipynb
 docs/gallery/polar-plots.ipynb
 docs/gallery/rectangle-selection.ipynb
 docs/gallery/scatter3d-with-slider.ipynb
 docs/gallery/scatter3d-with-threshold.ipynb
 docs/gallery/tiled-random-samples.ipynb
+docs/gallery/updating-scatter.ipynb
 docs/user-guide/index.md
 docs/user-guide/customization/custom-interfaces.ipynb
 docs/user-guide/customization/graph-node-tips.ipynb
 docs/user-guide/customization/subplots.ipynb
 docs/user-guide/customization/tweaking-figures.ipynb
 docs/user-guide/getting-started/installation.md
 docs/user-guide/getting-started/numpy-pandas-xarray.ipynb
 docs/user-guide/getting-started/overview.ipynb
 docs/user-guide/getting-started/saving-figures.ipynb
 docs/user-guide/plot-types/image-plot.ipynb
 docs/user-guide/plot-types/inspector-plot.ipynb
 docs/user-guide/plot-types/line-plot.ipynb
+docs/user-guide/plot-types/scatter-plot.ipynb
 docs/user-guide/plot-types/scatter3d-plot.ipynb
 docs/user-guide/plot-types/slicer-plot.ipynb
 docs/user-guide/plot-types/super-plot.ipynb
 requirements/base.in
 requirements/base.txt
 requirements/basetest.in
 requirements/basetest.txt
@@ -108,14 +111,15 @@
 requirements/test.in
 requirements/test.txt
 requirements/wheels.in
 requirements/wheels.txt
 resources/logo-plopp-2022.svg
 src/plopp/__init__.py
 src/plopp/py.typed
+src/plopp/utils.py
 src/plopp.egg-info/PKG-INFO
 src/plopp.egg-info/SOURCES.txt
 src/plopp.egg-info/dependency_links.txt
 src/plopp.egg-info/requires.txt
 src/plopp.egg-info/top_level.txt
 src/plopp/backends/__init__.py
 src/plopp/backends/common.py
@@ -123,14 +127,15 @@
 src/plopp/backends/protocols.py
 src/plopp/backends/matplotlib/__init__.py
 src/plopp/backends/matplotlib/canvas.py
 src/plopp/backends/matplotlib/figure.py
 src/plopp/backends/matplotlib/image.py
 src/plopp/backends/matplotlib/interactive.py
 src/plopp/backends/matplotlib/line.py
+src/plopp/backends/matplotlib/scatter.py
 src/plopp/backends/matplotlib/static.py
 src/plopp/backends/matplotlib/tiled.py
 src/plopp/backends/matplotlib/utils.py
 src/plopp/backends/plotly/__init__.py
 src/plopp/backends/plotly/canvas.py
 src/plopp/backends/plotly/figure.py
 src/plopp/backends/plotly/line.py
@@ -151,32 +156,39 @@
 src/plopp/data/examples.py
 src/plopp/data/factory.py
 src/plopp/data/testing.py
 src/plopp/graphics/__init__.py
 src/plopp/graphics/basefig.py
 src/plopp/graphics/camera.py
 src/plopp/graphics/colormapper.py
+src/plopp/graphics/common.py
 src/plopp/graphics/figure.py
+src/plopp/graphics/graphicalview.py
 src/plopp/graphics/imageview.py
 src/plopp/graphics/lineview.py
 src/plopp/graphics/scatter3dview.py
+src/plopp/graphics/scatterview.py
 src/plopp/graphics/tiled.py
 src/plopp/plotting/__init__.py
 src/plopp/plotting/common.py
 src/plopp/plotting/inspector.py
 src/plopp/plotting/plot.py
+src/plopp/plotting/scatter.py
 src/plopp/plotting/scatter3d.py
 src/plopp/plotting/slicer.py
 src/plopp/plotting/superplot.py
 src/plopp/plotting/xyplot.py
 src/plopp/widgets/__init__.py
 src/plopp/widgets/box.py
 src/plopp/widgets/checkboxes.py
+src/plopp/widgets/clip3d.py
 src/plopp/widgets/cut3d.py
+src/plopp/widgets/debounce.py
 src/plopp/widgets/drawing.py
+src/plopp/widgets/linesave.py
 src/plopp/widgets/slice.py
 src/plopp/widgets/style.py
 src/plopp/widgets/toolbar.py
 src/plopp/widgets/tools.py
 tests/conftest.py
 tests/high_level_test.py
 tests/minimal_plot_test.py
@@ -184,14 +196,15 @@
 tests/backends/matplotlib/mpl_canvas_test.py
 tests/backends/matplotlib/mpl_figure_test.py
 tests/backends/matplotlib/mpl_image_test.py
 tests/backends/matplotlib/mpl_imageview_test.py
 tests/backends/matplotlib/mpl_interactive_test.py
 tests/backends/matplotlib/mpl_line_test.py
 tests/backends/matplotlib/mpl_lineview_test.py
+tests/backends/matplotlib/mpl_scatter_test.py
 tests/backends/matplotlib/mpl_tiled_test.py
 tests/backends/matplotlib/mpl_utils_test.py
 tests/backends/plotly/conftest.py
 tests/backends/plotly/plotly_canvas_test.py
 tests/backends/plotly/plotly_figure_test.py
 tests/backends/plotly/plotly_line_test.py
 tests/backends/pythreejs/pythreejs_canvas_test.py
@@ -201,19 +214,22 @@
 tests/core/limits_test.py
 tests/core/node_test.py
 tests/core/utils_test.py
 tests/graphics/colormapper_test.py
 tests/graphics/imageview_test.py
 tests/graphics/lineview_test.py
 tests/graphics/scatter3dview_test.py
+tests/graphics/scatterview_test.py
 tests/plotting/common_test.py
 tests/plotting/inspector_test.py
 tests/plotting/plot_1d_test.py
 tests/plotting/plot_2d_test.py
 tests/plotting/scatter3d_test.py
+tests/plotting/scatter_test.py
 tests/plotting/slicer_test.py
 tests/plotting/superplot_test.py
 tests/plotting/xyplot_test.py
 tests/widgets/box_test.py
 tests/widgets/checkboxes_test.py
+tests/widgets/clip3d_test.py
 tests/widgets/cut3d_test.py
 tests/widgets/slice_test.py
```

### Comparing `plopp-24.2.0/tests/backends/matplotlib/mpl_canvas_test.py` & `plopp-24.4.0/tests/backends/matplotlib/mpl_canvas_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/backends/matplotlib/mpl_image_test.py` & `plopp-24.4.0/tests/backends/matplotlib/mpl_image_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/backends/matplotlib/mpl_imageview_test.py` & `plopp-24.4.0/tests/backends/matplotlib/mpl_imageview_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/backends/matplotlib/mpl_interactive_test.py` & `plopp-24.4.0/tests/backends/matplotlib/mpl_interactive_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/backends/matplotlib/mpl_line_test.py` & `plopp-24.4.0/tests/backends/matplotlib/mpl_line_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/backends/matplotlib/mpl_lineview_test.py` & `plopp-24.4.0/tests/backends/matplotlib/mpl_lineview_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,12 +40,12 @@
 def test_grid():
     da = data_array(ndim=1)
     fig = LineView(Node(da), grid=True)
     assert fig.canvas.ax.xaxis.get_gridlines()[0].get_visible()
 
 
 def test_ax():
-    fig, ax = plt.subplots()
+    _, ax = plt.subplots()
     assert len(ax.lines) == 0
     da = data_array(ndim=1)
     _ = LineView(Node(da), ax=ax)
     assert len(ax.lines) > 0
```

### Comparing `plopp-24.2.0/tests/backends/matplotlib/mpl_tiled_test.py` & `plopp-24.4.0/tests/backends/matplotlib/mpl_tiled_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/backends/matplotlib/mpl_utils_test.py` & `plopp-24.4.0/tests/backends/matplotlib/mpl_utils_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/backends/plotly/plotly_canvas_test.py` & `plopp-24.4.0/tests/backends/plotly/plotly_canvas_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/backends/plotly/plotly_figure_test.py` & `plopp-24.4.0/tests/backends/plotly/plotly_figure_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/backends/plotly/plotly_line_test.py` & `plopp-24.4.0/tests/backends/plotly/plotly_line_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/backends/pythreejs/pythreejs_canvas_test.py` & `plopp-24.4.0/tests/backends/pythreejs/pythreejs_canvas_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,12 +247,12 @@
     assert not canvas.outline.visible
     canvas.toggle_outline()
     assert canvas.outline.visible
 
 
 def test_creation_with_title():
     text = 'My title'
-    canvas = Canvas(figsize=(700, 450), title=text)
+    canvas = Canvas(title=text)
     assert canvas.title == text
     html = '<i>My</i> <b>title</b>'
-    canvas = Canvas(figsize=(700, 450), title=html)
+    canvas = Canvas(title=html)
     assert canvas.title == html
```

### Comparing `plopp-24.2.0/tests/backends/pythreejs/pythreejs_figure_test.py` & `plopp-24.4.0/tests/backends/pythreejs/pythreejs_figure_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/backends/pythreejs/pythreejs_point_cloud_test.py` & `plopp-24.4.0/tests/backends/pythreejs/pythreejs_point_cloud_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/conftest.py` & `plopp-24.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/core/graph_test.py` & `plopp-24.4.0/tests/core/graph_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/core/limits_test.py` & `plopp-24.4.0/tests/core/limits_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/core/node_test.py` & `plopp-24.4.0/tests/core/node_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/core/utils_test.py` & `plopp-24.4.0/tests/core/utils_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/graphics/colormapper_test.py` & `plopp-24.4.0/tests/graphics/colormapper_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,65 +49,65 @@
 
 def test_autoscale():
     da = data_array(ndim=2, unit='K')
     mapper = ColorMapper()
     artist = DummyChild(da)
     mapper['data'] = artist
 
-    mapper.update(key='data', data=da)
+    mapper.update(data=da)
     assert mapper.vmin == da.min().value
     assert mapper.vmax == da.max().value
 
     const = 2.3
     artist.update(da * const)
-    mapper.update(key='data', data=da * const)
+    mapper.update(data=da * const)
     assert mapper.vmin == (da.min() * const).value
     assert mapper.vmax == (da.max() * const).value
 
 
 def test_auto_rescale_limits_can_shrink():
     da = data_array(ndim=2, unit='K')
     mapper = ColorMapper(autoscale='auto')
     artist = DummyChild(da)
     mapper['data'] = artist
 
-    mapper.update(key='data', data=da)
+    mapper.update(data=da)
     assert mapper.vmin == da.min().value
     assert mapper.vmax == da.max().value
 
     const = 0.5
     artist.update(da * const)
-    mapper.update(key='data', data=da * const)
+    mapper.update(data=da * const)
     assert mapper.vmin == da.min().value * const
     assert mapper.vmax == da.max().value * const
 
 
 def test_grow_rescale_limits_do_not_shrink():
     da = data_array(ndim=2, unit='K')
     mapper = ColorMapper(autoscale='grow')
     artist = DummyChild(da)
     mapper['data'] = artist
 
-    mapper.update(key='data', data=da)
+    mapper.update(data=da)
     assert mapper.vmin == da.min().value
     assert mapper.vmax == da.max().value
 
     const = 0.5
     artist.update(da * const)
-    mapper.update(key='data', data=da * const)
+    mapper.update(data=da * const)
     assert mapper.vmin == da.min().value
     assert mapper.vmax == da.max().value
 
 
 def test_correct_normalizer_limits():
     da = sc.DataArray(data=sc.array(dims=['y', 'x'], values=[[1, 2], [3, 4]]))
     mapper = ColorMapper()
     artist = DummyChild(da)
     mapper['data'] = artist
-    mapper.update(key='data', data=da)
+    mapper.update(data=da)
     assert mapper.vmin == da.min().value
     assert mapper.vmax == da.max().value
     # The normalizer initially has limits [0, 1].
     # In Matplotlib, if we set the normalizer vmin value (1) equal to the current vmax,
     # it will silently set it to something smaller, e.g. 0.9.
     # Our implementation needs to work around this.
     assert mapper.normalizer.vmin == da.min().value
@@ -117,40 +117,40 @@
 def test_vmin_vmax():
     da = data_array(ndim=2, unit='K') * 100.0
     vmin = sc.scalar(-0.1, unit='K')
     vmax = sc.scalar(3.5, unit='K')
     mapper = ColorMapper(vmin=vmin, vmax=vmax)
     artist = DummyChild(da)
     mapper['data'] = artist
-    mapper.update(key='data', data=da)
+    mapper.update(data=da)
     assert mapper.user_vmin == vmin.value
     assert mapper.user_vmax == vmax.value
     assert mapper.vmin == vmin.value
     assert mapper.vmax == vmax.value
 
 
 def test_vmin_vmax_no_variable():
     da = data_array(ndim=2, unit='K') * 100.0
     vmin = -0.1
     vmax = 3.5
     mapper = ColorMapper(vmin=vmin, vmax=vmax)
     artist = DummyChild(da)
     mapper['data'] = artist
-    mapper.update(key='data', data=da)
+    mapper.update(data=da)
     assert mapper.user_vmin == vmin
     assert mapper.user_vmax == vmax
     assert mapper.vmin == vmin
     assert mapper.vmax == vmax
 
 
 def test_toggle_norm():
     mapper = ColorMapper()
     da = data_array(ndim=2, unit='K')
     mapper['child1'] = DummyChild(da)
-    mapper.update(key='child1', data=da)
+    mapper.update(child1=da)
     assert mapper.norm == 'linear'
     assert isinstance(mapper.normalizer, Normalize)
     assert mapper.vmin == da.min().value
     assert mapper.vmax == da.max().value
 
     mapper.toggle_norm()
     assert mapper.norm == 'log'
@@ -161,21 +161,21 @@
 
 def test_update_changes_limits():
     da = data_array(ndim=2, unit='K')
     mapper = ColorMapper()
     artist = DummyChild(da)
     mapper['data'] = artist
 
-    mapper.update(data=da, key=None)
+    mapper.update(data=da)
     assert mapper.normalizer.vmin == da.min().value
     assert mapper.normalizer.vmax == da.max().value
 
     const = 2.3
     artist.update(da * const)
-    mapper.update(data=da * const, key=None)
+    mapper.update(data=da * const)
     assert mapper.normalizer.vmin == (da.min() * const).value
     assert mapper.normalizer.vmax == (da.max() * const).value
 
 
 def test_rgba():
     da = data_array(ndim=2, unit='K')
     mapper = ColorMapper()
@@ -193,58 +193,58 @@
 def test_colorbar_updated_on_rescale():
     da = data_array(ndim=2, unit='K')
     mapper = ColorMapper()
     artist = DummyChild(da)
     key = 'data'
     mapper[key] = artist
 
-    mapper.update(data=da, key=key)
+    mapper.update(data=da)
     _ = mapper.to_widget()
     old_image = mapper.widget.value
     old_image_array = old_image
 
     # Update with the same values should not make a new colorbar image
     artist.update(da)
-    mapper.update(data=da, key=key)
+    mapper.update(data=da)
     assert old_image is mapper.widget.value
 
     # Update with new values should make a new colorbar image
     const = 2.3
     artist.update(da * const)
-    mapper.update(data=da * const, key=key)
+    mapper.update(data=da * const)
     assert old_image_array != mapper.widget.value
 
 
 def test_colorbar_does_not_update_on_rescale_if_limits_can_only_grow():
     da = data_array(ndim=2, unit='K')
     mapper = ColorMapper(autoscale='grow')
     artist = DummyChild(da)
     key = 'data'
     mapper[key] = artist
 
-    mapper.update(data=da, key=key)
+    mapper.update(data=da)
     _ = mapper.to_widget()
     old_image = mapper.widget.value
     old_image_array = old_image
 
     # Update with the same values should not make a new colorbar image
     artist.update(da)
-    mapper.update(data=da, key=key)
+    mapper.update(data=da)
     assert old_image is mapper.widget.value
 
     # Update with a smaller range should not make a new colorbar image
     const = 0.8
     artist.update(da * const)
-    mapper.update(data=da * const, key=key)
+    mapper.update(data=da * const)
     assert old_image is mapper.widget.value
 
     # Update with new values should make a new colorbar image
     const = 2.3
     artist.update(da * const)
-    mapper.update(data=da * const, key=key)
+    mapper.update(data=da * const)
     assert old_image_array != mapper.widget.value
 
 
 def test_colorbar_is_not_created_if_cbar_false():
     mapper = ColorMapper(cbar=False)
     assert mapper.colorbar is None
     assert mapper.cax is None
@@ -261,29 +261,29 @@
 
 def test_autoscale_auto_vmin_set():
     da = data_array(ndim=2, unit='K')
     mapper = ColorMapper(autoscale='auto', vmin=-0.5)
     artist = DummyChild(da)
     key = 'data'
     mapper[key] = artist
-    mapper.update(data=da, key=key)
+    mapper.update(data=da)
     assert mapper.vmin == -0.5
     assert mapper.vmax == da.max().value
     # Make sure it handles when da.max() is greater than vmin
-    mapper.update(data=da - sc.scalar(5.0, unit='K'), key=key)
+    mapper.update(data=da - sc.scalar(5.0, unit='K'))
     assert mapper.vmin == -0.5
     assert mapper.vmin < mapper.vmax
 
 
 def test_autoscale_auto_vmax_set():
     da = data_array(ndim=2, unit='K')
     mapper = ColorMapper(autoscale='auto', vmax=0.5)
     artist = DummyChild(da)
     key = 'data'
     mapper[key] = artist
-    mapper.update(data=da, key=key)
+    mapper.update(data=da)
     assert mapper.vmax == 0.5
     assert mapper.vmin == da.min().value
     # Make sure it handles when da.min() is greater than vmax
-    mapper.update(data=da + sc.scalar(5.0, unit='K'), key=key)
+    mapper.update(data=da + sc.scalar(5.0, unit='K'))
     assert mapper.vmax == 0.5
     assert mapper.vmin < mapper.vmax
```

### Comparing `plopp-24.2.0/tests/graphics/imageview_test.py` & `plopp-24.4.0/tests/graphics/imageview_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,28 +15,24 @@
 
 
 def test_update():
     fig = ImageView()
     assert len(fig.artists) == 0
     da = data_array(ndim=2)
     key = 'data2d'
-    fig.update(da, key=key)
+    fig.update({key: da})
     assert sc.identical(fig.artists[key]._data, da)
 
 
 def test_update_not_2d_raises():
     fig = ImageView()
-    with pytest.raises(
-        ValueError, match="ImageView can only be used to plot 2-D data."
-    ):
-        fig.update(data_array(ndim=1), key='data1d')
-    with pytest.raises(
-        ValueError, match="ImageView can only be used to plot 2-D data."
-    ):
-        fig.update(data_array(ndim=3), key='data3d')
+    with pytest.raises(ValueError, match="Expected 2 dimension"):
+        fig.update(data1d=data_array(ndim=1))
+    with pytest.raises(ValueError, match="Expected 2 dimension"):
+        fig.update(data3d=data_array(ndim=3))
 
 
 def test_create_with_node():
     da = data_array(ndim=2)
     fig = ImageView(Node(da))
     assert len(fig.artists) == 1
     assert sc.identical(list(fig.artists.values())[0]._data, da)
@@ -61,15 +57,15 @@
     fig = ImageView(norm='log')
     assert fig.colormapper.norm == 'log'
 
 
 def test_raises_for_new_data_with_incompatible_dimension():
     a = data_array(ndim=2)
     b = a.rename(xx='zz')
-    with pytest.raises(sc.DimensionError):
+    with pytest.raises(KeyError):
         ImageView(Node(a), Node(b))
 
 
 def test_raises_for_new_data_with_incompatible_unit():
     a = data_array(ndim=2)
     b = a * a
     with pytest.raises(sc.UnitError):
```

### Comparing `plopp-24.2.0/tests/graphics/lineview_test.py` & `plopp-24.4.0/tests/graphics/lineview_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,25 +15,24 @@
     assert len(fig.artists) == 0
 
 
 def test_update():
     fig = LineView()
     assert len(fig.artists) == 0
     da = data_array(ndim=1)
-    key = 'data1d'
-    fig.update(da, key=key)
-    assert sc.identical(fig.artists[key]._data, da)
+    fig.update(data1d=da)
+    assert sc.identical(fig.artists['data1d']._data, da)
 
 
 def test_update_not_1d_raises():
     fig = LineView()
-    with pytest.raises(ValueError, match="LineView can only be used to plot 1-D data."):
-        fig.update(data_array(ndim=2), key='data2d')
-    with pytest.raises(ValueError, match="LineView can only be used to plot 1-D data."):
-        fig.update(data_array(ndim=3), key='data3d')
+    with pytest.raises(ValueError, match="Expected 1 dimension"):
+        fig.update(data2d=data_array(ndim=2))
+    with pytest.raises(ValueError, match="Expected 1 dimension"):
+        fig.update(data3d=data_array(ndim=3))
 
 
 def test_create_with_node():
     da = data_array(ndim=1)
     fig = LineView(Node(da))
     assert len(fig.artists) == 1
     line = list(fig.artists.values())[0]
@@ -71,38 +70,38 @@
 
 
 def test_update_grows_limits():
     da = data_array(ndim=1)
     fig = LineView(Node(da))
     old_lims = fig.canvas.yrange
     key = list(fig.artists.keys())[0]
-    fig.update(da * 2.5, key=key)
+    fig.update({key: da * 2.5})
     new_lims = fig.canvas.yrange
     assert new_lims[0] < old_lims[0]
     assert new_lims[1] > old_lims[1]
 
 
 def test_update_does_shrink_limits_if_auto_mode():
     da = data_array(ndim=1)
     fig = LineView(Node(da), autoscale='auto')
     old_lims = fig.canvas.yrange
     key = list(fig.artists.keys())[0]
     const = 0.5
-    fig.update(da * const, key=key)
+    fig.update({key: da * const})
     new_lims = fig.canvas.yrange
     assert new_lims[0] == old_lims[0] * const
     assert new_lims[1] == old_lims[1] * const
 
 
 def test_update_does_not_shrink_limits_if_grow_mode():
     da = data_array(ndim=1)
     fig = LineView(Node(da), autoscale='grow')
     old_lims = fig.canvas.yrange
     key = list(fig.artists.keys())[0]
-    fig.update(da * 0.5, key=key)
+    fig.update({key: da * 0.5})
     new_lims = fig.canvas.yrange
     assert new_lims[0] == old_lims[0]
     assert new_lims[1] == old_lims[1]
 
 
 def test_vmin():
     da = data_array(ndim=1)
@@ -137,15 +136,15 @@
     fig = LineView(Node(da), vmin=-0.5, vmax=0.68)
     assert np.allclose(fig.canvas.yrange, [-0.5, 0.68])
 
 
 def test_raises_for_new_data_with_incompatible_dimension():
     x = data_array(ndim=1)
     y = x.rename(xx='yy')
-    with pytest.raises(sc.DimensionError):
+    with pytest.raises(KeyError):
         LineView(Node(x), Node(y))
 
 
 def test_raises_for_new_data_with_incompatible_unit():
     a = data_array(ndim=1)
     b = a * a
     with pytest.raises(sc.UnitError):
```

### Comparing `plopp-24.2.0/tests/graphics/scatter3dview_test.py` & `plopp-24.4.0/tests/graphics/scatterview_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,82 +1,76 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+# Copyright (c) 2024 Scipp contributors (https://github.com/scipp)
 
 import pytest
 import scipp as sc
 
 from plopp import Node
-from plopp.data.testing import scatter
-from plopp.graphics.scatter3dview import Scatter3dView
+from plopp.data.testing import scatter as scatter_data
+from plopp.graphics.scatterview import ScatterView
 
 
 def test_creation():
-    da = scatter()
-    fig = Scatter3dView(Node(da), x='x', y='y', z='z')
+    da = scatter_data()
+    fig = ScatterView(Node(da), x='x', y='y')
     assert len(fig.artists) == 1
     key = list(fig.artists.keys())[0]
     assert sc.identical(fig.artists[key]._data, da)
 
 
 def test_update():
-    da = scatter()
-    fig = Scatter3dView(Node(da), x='x', y='y', z='z')
+    da = scatter_data()
+    fig = ScatterView(Node(da), x='x', y='y')
     assert len(fig.artists) == 1
     key = list(fig.artists.keys())[0]
-    fig.update(da * 3.3, key=key)
+    fig.update({key: da * 3.3})
     assert sc.identical(fig.artists[key]._data, da * 3.3)
 
 
-def test_log_norm():
-    da = scatter()
-    fig = Scatter3dView(Node(da), x='x', y='y', z='z', norm='log')
-    assert fig.colormapper.norm == 'log'
-
-
 def test_raises_for_new_data_with_incompatible_coordinate():
-    a = scatter()
-    b = scatter()
+    a = scatter_data()
+    b = scatter_data()
     b.coords['t'] = b.coords.pop('x')
     with pytest.raises(KeyError):
-        Scatter3dView(Node(a), Node(b), x='x', y='y', z='z')
+        ScatterView(Node(a), Node(b), x='x', y='y')
 
 
 def test_raises_for_new_data_with_incompatible_unit():
-    a = scatter()
+    a = scatter_data()
     b = a * a
     with pytest.raises(sc.UnitError):
-        Scatter3dView(Node(a), Node(b), x='x', y='y', z='z')
+        ScatterView(Node(a), Node(b), x='x', y='y', cbar=True)
 
 
 def test_raises_for_new_data_with_incompatible_coord_unit():
-    a = scatter()
+    a = scatter_data()
     b = a.copy()
     b.coords['x'] = a.coords['x'] * a.coords['x']
     with pytest.raises(sc.UnitError):
-        Scatter3dView(Node(a), Node(b), x='x', y='y', z='z')
+        ScatterView(Node(a), Node(b), x='x', y='y')
 
 
 def test_converts_new_data_units():
-    a = scatter()
+    a = scatter_data()
     a.unit = 'm'
-    b = scatter()
+    b = scatter_data()
     b.unit = 'cm'
     anode = Node(a)
     bnode = Node(b)
-    fig = Scatter3dView(anode, bnode, x='x', y='y', z='z')
+    fig = ScatterView(anode, bnode, x='x', y='y', cbar=True)
     assert sc.identical(fig.artists[anode.id]._data, a)
     assert sc.identical(fig.artists[bnode.id]._data, b.to(unit='m'))
 
 
 def test_converts_new_data_coordinate_units():
-    a = scatter()
-    b = scatter()
+    a = scatter_data()
+    b = scatter_data()
     xcoord = b.coords['x'].copy()
     xcoord.unit = 'cm'
     b.coords['x'] = xcoord
     anode = Node(a)
     bnode = Node(b)
-    fig = Scatter3dView(anode, bnode, x='x', y='y', z='z')
+    fig = ScatterView(anode, bnode, x='x', y='y')
     assert sc.identical(fig.artists[anode.id]._data, a)
     c = b.copy()
     c.coords['x'] = c.coords['x'].to(unit='m')
     assert sc.identical(fig.artists[bnode.id]._data, c)
```

### Comparing `plopp-24.2.0/tests/high_level_test.py` & `plopp-24.4.0/tests/high_level_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import ipywidgets as ipw
 import scipp as sc
 
-from plopp import Node, figure1d, figure2d, node, widget_node
+from plopp import Node, imagefigure, linefigure, node, widget_node
 from plopp.data.testing import data_array, dataset
 from plopp.widgets import Box, Checkboxes, SliceWidget, slice_dims
 
 
 @node
 def hide_masks(data_array, masks):
     out = data_array.copy(deep=False)
@@ -17,55 +17,55 @@
             del out.masks[name]
     return out
 
 
 def test_single_1d_line():
     da = data_array(ndim=1)
     n = Node(da)
-    _ = figure1d(n)
+    _ = linefigure(n)
 
 
 def test_two_1d_lines():
     ds = dataset(ndim=1)
     a = Node(ds['a'])
     b = Node(ds['b'])
-    _ = figure1d(a, b)
+    _ = linefigure(a, b)
 
 
 def test_difference_of_two_1d_lines():
     ds = dataset(ndim=1)
     a = Node(ds['a'])
     b = Node(ds['b'])
 
     @node
     def diff(x, y):
         return x - y
 
     c = diff(a, b)
-    _ = figure1d(a, b, c)
+    _ = linefigure(a, b, c)
 
 
 def test_2d_image():
     da = data_array(ndim=2)
     a = Node(da)
-    _ = figure2d(a)
+    _ = imagefigure(a)
 
 
 def test_2d_image_smoothing_slider():
     da = data_array(ndim=2)
     a = Node(da)
 
     sl = ipw.IntSlider(min=1, max=10)
     sigma_node = widget_node(sl)
 
     from scipp.scipy.ndimage import gaussian_filter
 
     smooth_node = Node(gaussian_filter, a, sigma=sigma_node)
 
-    fig = figure2d(smooth_node)
+    fig = imagefigure(smooth_node)
     Box([fig.to_widget(), sl])
     sl.value = 5
 
 
 def test_2d_image_with_masks():
     da = data_array(ndim=2)
     da.masks['m1'] = da.data < sc.scalar(0.0, unit='m/s')
@@ -73,15 +73,15 @@
 
     a = Node(da)
 
     widget = Checkboxes(da.masks.keys())
     w = widget_node(widget)
 
     masks_node = hide_masks(a, w)
-    fig = figure2d(masks_node)
+    fig = imagefigure(masks_node)
     Box([fig.to_widget(), widget])
     widget.toggle_all_button.value = False
 
 
 def test_two_1d_lines_with_masks():
     ds = dataset()
     ds['a'].masks['m1'] = ds['a'].coords['xx'] > sc.scalar(40.0, unit='m')
@@ -92,51 +92,51 @@
     b = Node(ds['b'])
 
     widget = Checkboxes(list(ds['a'].masks.keys()) + list(ds['b'].masks.keys()))
     w = widget_node(widget)
 
     node_masks_a = hide_masks(a, w)
     node_masks_b = hide_masks(b, w)
-    fig = figure1d(node_masks_a, node_masks_b)
+    fig = linefigure(node_masks_a, node_masks_b)
     Box([fig.to_widget(), widget])
     widget.toggle_all_button.value = False
 
 
 def test_node_sum_data_along_y():
     da = data_array(ndim=2, binedges=True)
     a = Node(da)
     s = Node(sc.sum, a, dim='yy')
 
-    fig1 = figure2d(a)
-    fig2 = figure1d(s)
+    fig1 = imagefigure(a)
+    fig2 = linefigure(s)
     Box([[fig1.to_widget(), fig2.to_widget()]])
 
 
 def test_slice_3d_cube():
     da = data_array(ndim=3)
     a = Node(da)
     sl = SliceWidget(da, dims=['zz'])
     w = widget_node(sl)
 
     slice_node = slice_dims(a, w)
 
-    fig = figure2d(slice_node)
+    fig = imagefigure(slice_node)
     Box([fig.to_widget(), sl])
     sl.controls["zz"]["slider"].value = 10
 
 
 def test_3d_image_slicer_with_connected_side_histograms():
     da = data_array(ndim=3)
     a = Node(da)
     sl = SliceWidget(da, dims=['zz'])
     w = widget_node(sl)
 
     sliced = slice_dims(a, w)
-    fig = figure2d(sliced)
+    fig = imagefigure(sliced)
 
     histx = Node(sc.sum, sliced, dim='xx')
     histy = Node(sc.sum, sliced, dim='yy')
 
-    fx = figure1d(histx)
-    fy = figure1d(histy)
+    fx = linefigure(histx)
+    fy = linefigure(histy)
     Box([[fx.to_widget(), fy.to_widget()], fig.to_widget(), sl])
     sl.controls["zz"]["slider"].value = 10
```

### Comparing `plopp-24.2.0/tests/plotting/common_test.py` & `plopp-24.4.0/tests/plotting/common_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/plotting/inspector_test.py` & `plopp-24.4.0/tests/plotting/inspector_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/plotting/plot_1d_test.py` & `plopp-24.4.0/tests/plotting/plot_1d_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/plotting/plot_2d_test.py` & `plopp-24.4.0/tests/plotting/plot_2d_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/plotting/scatter3d_test.py` & `plopp-24.4.0/tests/plotting/scatter3d_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,31 +30,31 @@
     x = sc.linspace(dim='x', start=-10.0, stop=10.0, num=nx, unit='m')
     y = sc.linspace(dim='y', start=-10.0, stop=10.0, num=ny, unit='m')
     da = sc.DataArray(
         data=sc.array(dims=['x', 'y'], values=np.random.rand(nx, ny)),
         coords={'position': sc.spatial.as_vectors(x, y, 0.0 * sc.units.m)},
     )
     p = pp.scatter3d(da, pos="position")
-    assert list(p[0].artists.values())[0].data.ndim == 1
+    assert list(p.artists.values())[0].data.ndim == 1
     nz = 12
     z = sc.linspace(dim='z', start=-10.0, stop=10.0, num=nz, unit='m')
     da = sc.DataArray(
         data=sc.array(dims=['x', 'y', 'z'], values=np.random.rand(nx, ny, nz)),
         coords={'position': sc.spatial.as_vectors(x, y, z)},
     )
     p = pp.scatter3d(da, pos="position")
-    assert list(p[0].artists.values())[0].data.ndim == 1
+    assert list(p.artists.values())[0].data.ndim == 1
 
 
 def test_scatter3d_can_plot_scalar_data():
     da = sc.DataArray(
         data=sc.scalar(1.2), coords={'position': sc.vector(value=[1, 2, 3])}
     )
     p = pp.scatter3d(da, pos='position')
-    assert list(p.children[0].artists.values())[0].data.ndim == 1
+    assert list(p.artists.values())[0].data.ndim == 1
 
 
 def test_raises_ValueError_when_given_binned_data():
     nx = 10
     da = sc.data.table_xyz(100).bin(x=nx)
     x = sc.linspace(dim='x', start=-10.0, stop=10.0, num=nx, unit='m')
     da.coords['position'] = sc.spatial.as_vectors(x, x, x)
@@ -85,15 +85,15 @@
 
 
 def test_scatter3d_dict_of_inputs():
     da1 = scatter()
     da2 = scatter()
     da2.coords['x'] += sc.scalar(100, unit='m')
     fig = pp.scatter3d({'a': da1, 'b': da2})
-    assert len(fig[0].artists) == 2
+    assert len(fig.artists) == 2
 
 
 def test_scatter3d_from_node():
     pp.scatter3d(pp.Node(scatter()))
 
 
 def test_scatter3d_from_multiple_nodes():
```

### Comparing `plopp-24.2.0/tests/plotting/slicer_test.py` & `plopp-24.4.0/tests/plotting/slicer_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,146 +5,146 @@
 import scipp as sc
 
 from plopp import Node
 from plopp.data.testing import data_array, dataset
 from plopp.plotting.slicer import Slicer
 
 
-def test_creation_keep_two_dims():
+def test_creation_keep_two_dims(use_ipympl):
     da = data_array(ndim=3)
     sl = Slicer(da, keep=['xx', 'yy'])
     assert sl.slider.value == {'zz': 0}
     assert sl.slider.controls['zz']['slider'].max == da.sizes['zz'] - 1
     assert sc.identical(sl.slice_nodes[0].request_data(), da['zz', 0])
 
 
-def test_creation_keep_one_dim():
+def test_creation_keep_one_dim(use_ipympl):
     da = data_array(ndim=3)
     sl = Slicer(da, keep=['xx'])
     assert sl.slider.value == {'zz': 0, 'yy': 0}
     assert sl.slider.controls['yy']['slider'].max == da.sizes['yy'] - 1
     assert sl.slider.controls['zz']['slider'].max == da.sizes['zz'] - 1
     assert sc.identical(sl.slice_nodes[0].request_data(), da['yy', 0]['zz', 0])
 
 
-def test_update_keep_two_dims():
+def test_update_keep_two_dims(use_ipympl):
     da = data_array(ndim=3)
     sl = Slicer(da, keep=['xx', 'yy'])
     assert sl.slider.value == {'zz': 0}
     assert sc.identical(sl.slice_nodes[0].request_data(), da['zz', 0])
     sl.slider.controls['zz']['slider'].value = 5
     assert sl.slider.value == {'zz': 5}
     assert sc.identical(sl.slice_nodes[0].request_data(), da['zz', 5])
 
 
-def test_update_keep_one_dim():
+def test_update_keep_one_dim(use_ipympl):
     da = data_array(ndim=3)
     sl = Slicer(da, keep=['xx'])
     assert sl.slider.value == {'zz': 0, 'yy': 0}
     assert sc.identical(sl.slice_nodes[0].request_data(), da['yy', 0]['zz', 0])
     sl.slider.controls['yy']['slider'].value = 5
     assert sl.slider.value == {'zz': 0, 'yy': 5}
     assert sc.identical(sl.slice_nodes[0].request_data(), da['yy', 5]['zz', 0])
     sl.slider.controls['zz']['slider'].value = 8
     assert sl.slider.value == {'zz': 8, 'yy': 5}
     assert sc.identical(sl.slice_nodes[0].request_data(), da['yy', 5]['zz', 8])
 
 
-def test_with_dataset():
+def test_with_dataset(use_ipympl):
     ds = dataset(ndim=2)
     sl = Slicer(ds, keep=['xx'])
     nodes = list(sl.figure.graph_nodes.values())
     sl.slider.controls['yy']['slider'].value = 5
     assert sc.identical(nodes[0].request_data(), ds['a']['yy', 5])
     assert sc.identical(nodes[1].request_data(), ds['b']['yy', 5])
 
 
-def test_with_data_group():
+def test_with_data_group(use_ipympl):
     da = data_array(ndim=2)
     dg = sc.DataGroup(a=da, b=da * 2.5)
     sl = Slicer(dg, keep=['xx'])
     nodes = list(sl.figure.graph_nodes.values())
     sl.slider.controls['yy']['slider'].value = 5
     assert sc.identical(nodes[0].request_data(), dg['a']['yy', 5])
     assert sc.identical(nodes[1].request_data(), dg['b']['yy', 5])
 
 
-def test_with_dict_of_data_arrays():
+def test_with_dict_of_data_arrays(use_ipympl):
     a = data_array(ndim=2)
     b = data_array(ndim=2) * 2.5
     sl = Slicer({'a': a, 'b': b}, keep=['xx'])
     nodes = list(sl.figure.graph_nodes.values())
     sl.slider.controls['yy']['slider'].value = 5
     assert sc.identical(nodes[0].request_data(), a['yy', 5])
     assert sc.identical(nodes[1].request_data(), b['yy', 5])
 
 
-def test_with_data_arrays_same_shape_different_coord():
+def test_with_data_arrays_same_shape_different_coord(use_ipympl):
     a = data_array(ndim=2)
     b = data_array(ndim=2) * 2.5
     b.coords['xx'] *= 1.5
     Slicer({'a': a, 'b': b}, keep=['xx'])
 
 
-def test_with_data_arrays_different_shape_along_keep_dim():
+def test_with_data_arrays_different_shape_along_keep_dim(use_ipympl):
     a = data_array(ndim=2)
     b = data_array(ndim=2) * 2.5
     Slicer({'a': a, 'b': b['xx', :10]}, keep=['xx'])
 
 
-def test_with_data_arrays_different_shape_along_non_keep_dim_raises():
+def test_with_data_arrays_different_shape_along_non_keep_dim_raises(use_ipympl):
     a = data_array(ndim=2)
     b = data_array(ndim=2) * 2.5
     with pytest.raises(
         ValueError, match='Slicer plot: all inputs must have the same sizes'
     ):
         Slicer({'a': a, 'b': b['yy', :10]}, keep=['xx'])
 
 
-def test_raises_ValueError_when_given_binned_data():
+def test_raises_ValueError_when_given_binned_data(use_ipympl):
     da = sc.data.table_xyz(100).bin(x=10, y=20)
     with pytest.raises(ValueError, match='Cannot plot binned data'):
         Slicer(da, keep=['xx'])
 
 
 @pytest.mark.parametrize('ndim', [2, 3])
-def test_from_node(ndim):
+def test_from_node(use_ipympl, ndim):
     da = data_array(ndim=ndim)
     Slicer(Node(da))
 
 
-def test_mixing_raw_data_and_nodes():
+def test_mixing_raw_data_and_nodes(use_ipympl):
     a = data_array(ndim=2)
     b = 6.7 * a
     Slicer({'a': Node(a), 'b': Node(b)})
     Slicer({'a': a, 'b': Node(b)})
     Slicer({'a': Node(a), 'b': b})
 
 
-def test_raises_when_requested_keep_dims_do_not_exist():
+def test_raises_when_requested_keep_dims_do_not_exist(use_ipympl):
     da = data_array(ndim=3)
     with pytest.raises(
         ValueError, match='Slicer plot: one or more of the requested dims to be kept'
     ):
         Slicer(da, keep=['time'])
 
 
-def test_raises_when_number_of_keep_dims_requested_is_bad():
+def test_raises_when_number_of_keep_dims_requested_is_bad(use_ipympl):
     da = data_array(ndim=4)
     with pytest.raises(
         ValueError, match='Slicer plot: the number of dims to be kept must be 1 or 2'
     ):
         Slicer(da, keep=['xx', 'yy', 'zz'])
     with pytest.raises(
         ValueError, match='Slicer plot: the list of dims to be kept cannot be empty'
     ):
         Slicer(da, keep=[])
 
 
-def test_autoscale_fixed():
+def test_autoscale_fixed(use_ipympl):
     da = sc.DataArray(
         data=sc.arange('x', 5 * 10 * 20).fold(dim='x', sizes={'z': 20, 'y': 10, 'x': 5})
     )
     sl = Slicer(da, keep=['y', 'x'], autoscale='fixed')
     assert sl.figure._view.colormapper.vmin == 0
     assert sl.figure._view.colormapper.vmax == 5 * 10 * 20 - 1
     sl.slider.controls['z']['slider'].value = 5
```

### Comparing `plopp-24.2.0/tests/plotting/superplot_test.py` & `plopp-24.4.0/tests/plotting/superplot_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 import pytest
 import scipp as sc
 
 from plopp import Node
 from plopp.data.testing import data_array
-from plopp.plotting.superplot import Superplot
+from plopp.plotting.superplot import superplot
 
 
-def test_creation():
+def test_creation(use_ipympl):
     da = data_array(ndim=2)
-    sp = Superplot(da, keep='xx')
-    assert len(sp.linesavetool._lines) == 0
+    sp = superplot(da, keep='xx')
+    assert len(sp.right_bar[0]._lines) == 0
 
 
-def test_from_node():
+def test_from_node(use_ipympl):
     da = data_array(ndim=2)
-    Superplot(Node(da))
+    superplot(Node(da))
 
 
-def test_save_line():
+def test_save_line(use_ipympl):
     da = data_array(ndim=2)
-    sp = Superplot(da, keep='xx')
-    tool = sp.linesavetool
+    sp = superplot(da, keep='xx')
+    tool = sp.right_bar[0]
     assert len(tool._lines) == 0
     tool.save_line()
     assert len(tool._lines) == 1
     line = list(tool._lines.values())[-1]
     assert sc.identical(line['line']._data, da['yy', 0])
     assert len(tool.container.children) == 1
 
-    sp.slider.controls['yy']['slider'].value = 5
+    slider = sp.bottom_bar[0]
+    slider.controls['yy']['slider'].value = 5
     tool.save_line()
     assert len(tool._lines) == 2
     line = list(tool._lines.values())[-1]
     assert sc.identical(line['line']._data, da['yy', 5])
     assert len(tool.container.children) == 2
 
 
-def test_remove_line():
+def test_remove_line(use_ipympl):
     da = data_array(ndim=2)
-    sp = Superplot(da, keep='xx')
-    tool = sp.linesavetool
+    sp = superplot(da, keep='xx')
+    tool = sp.right_bar[0]
     assert len(tool._lines) == 0
     tool.save_line()
-    sp.slider.controls['yy']['slider'].value = 5
+    slider = sp.bottom_bar[0]
+    slider.controls['yy']['slider'].value = 5
     tool.save_line()
-    sp.slider.controls['yy']['slider'].value = 15
+    slider.controls['yy']['slider'].value = 15
     tool.save_line()
     assert len(tool._lines) == 3
     assert len(tool.container.children) == 3
 
     keys = list(tool._lines.keys())
     first_line = keys[0]
     last_line = keys[2]
@@ -60,21 +62,21 @@
     assert len(tool.container.children) == 2
 
     tool.remove_line(change=None, line_id=last_line)
     assert last_line not in tool._lines
     assert len(tool.container.children) == 1
 
 
-def test_change_line_color():
+def test_change_line_color(use_ipympl):
     da = data_array(ndim=2)
-    sp = Superplot(da, keep='xx')
-    tool = sp.linesavetool
+    sp = superplot(da, keep='xx')
+    tool = sp.right_bar[0]
     tool.save_line()
     line_id = list(tool._lines.keys())[-1]
     tool.change_line_color(change={'new': '#000000'}, line_id=line_id)
     assert tool._lines[line_id]['line'].color == '#000000'
 
 
-def test_raises_ValueError_when_given_binned_data():
+def test_raises_ValueError_when_given_binned_data(use_ipympl):
     da = sc.data.table_xyz(100).bin(x=10, y=20)
     with pytest.raises(ValueError, match='Cannot plot binned data'):
-        Superplot(da, keep='x')
+        superplot(da, keep='x')
```

### Comparing `plopp-24.2.0/tests/plotting/xyplot_test.py` & `plopp-24.4.0/tests/plotting/xyplot_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/widgets/box_test.py` & `plopp-24.4.0/tests/widgets/box_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/widgets/checkboxes_test.py` & `plopp-24.4.0/tests/widgets/checkboxes_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/widgets/cut3d_test.py` & `plopp-24.4.0/tests/widgets/cut3d_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tests/widgets/slice_test.py` & `plopp-24.4.0/tests/widgets/slice_test.py`

 * *Files identical despite different names*

### Comparing `plopp-24.2.0/tox.ini` & `plopp-24.4.0/tox.ini`

 * *Files identical despite different names*

