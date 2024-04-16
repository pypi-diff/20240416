# Comparing `tmp/exoplanet-0.5.3rc1.tar.gz` & `tmp/exoplanet-0.6.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exoplanet-0.5.3rc1.tar", last modified: Wed Oct 12 23:49:27 2022, max compression
+gzip compressed data, was "exoplanet-0.6.0rc2.tar", last modified: Tue Apr 16 15:36:52 2024, max compression
```

## Comparing `exoplanet-0.5.3rc1.tar` & `exoplanet-0.6.0rc2.tar`

### file list

```diff
@@ -1,112 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 23:49:27.300967 exoplanet-0.5.3rc1/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/.clang-format
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 23:49:27.292967 exoplanet-0.5.3rc1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 23:49:27.292967 exoplanet-0.5.3rc1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 23:49:27.292967 exoplanet-0.5.3rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/.github/workflows/joss.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2989 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      953 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1869 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (121)     3356 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     6169 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2991 2022-10-12 23:49:27.300967 exoplanet-0.5.3rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2198 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 23:49:27.292967 exoplanet-0.5.3rc1/binder/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/binder/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/binder/runtime.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 23:49:27.292967 exoplanet-0.5.3rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 23:49:27.296967 exoplanet-0.5.3rc1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)    33319 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/_static/big_logo.png
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/_static/exoplanet.css
--rw-r--r--   0 runner    (1001) docker     (121)     1845 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/_static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (121)    18175 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)    65535 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/_static/logo_shadow.png
--rw-r--r--   0 runner    (1001) docker     (121)    80605 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/_static/orbit3D.png
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1533 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3523 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 23:49:27.296967 exoplanet-0.5.3rc1/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (121)     1429 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/tutorials/about.md
--rw-r--r--   0 runner    (1001) docker     (121)     9810 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/tutorials/autodiff.md
--rw-r--r--   0 runner    (1001) docker     (121)     2317 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/tutorials/citation.md
--rw-r--r--   0 runner    (1001) docker     (121)    22446 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/tutorials/data-and-models.md
--rw-r--r--   0 runner    (1001) docker     (121)    17781 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/tutorials/intro-to-pymc3.md
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/tutorials/ipython_kernel_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3759 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/tutorials/light-delay.md
--rw-r--r--   0 runner    (1001) docker     (121)     2175 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/tutorials/reparameterization.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 23:49:27.296967 exoplanet-0.5.3rc1/docs/user/
--rw-r--r--   0 runner    (1001) docker     (121)     1412 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/user/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3978 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/user/dev.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/user/install.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1422 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/user/multiprocessing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2197 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/docs/user/theano.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 23:49:27.296967 exoplanet-0.5.3rc1/joss/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 23:49:27.296967 exoplanet-0.5.3rc1/joss/figures/
--rw-r--r--   0 runner    (1001) docker     (121)   183655 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/joss/figures/figure.png
--rw-r--r--   0 runner    (1001) docker     (121)    98285 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/joss/figures/joss-logo.png
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/joss/metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    41317 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/joss/paper.bib
--rw-r--r--   0 runner    (1001) docker     (121)    13547 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/joss/paper.md
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-12 23:49:27.300967 exoplanet-0.5.3rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2552 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 23:49:27.292967 exoplanet-0.5.3rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 23:49:27.296967 exoplanet-0.5.3rc1/src/exoplanet/
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/src/exoplanet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16266 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/src/exoplanet/citations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 23:49:27.300967 exoplanet-0.5.3rc1/src/exoplanet/distributions/
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/src/exoplanet/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5723 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/src/exoplanet/distributions/eccentricity.py
--rw-r--r--   0 runner    (1001) docker     (121)     3591 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/src/exoplanet/distributions/physical.py
--rw-r--r--   0 runner    (1001) docker     (121)     5158 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/src/exoplanet/distributions/transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)    12624 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/src/exoplanet/estimators.py
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-12 23:49:27.000000 exoplanet-0.5.3rc1/src/exoplanet/exoplanet_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     3416 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/src/exoplanet/interp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 23:49:27.300967 exoplanet-0.5.3rc1/src/exoplanet/light_curves/
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/src/exoplanet/light_curves/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4178 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/src/exoplanet/light_curves/interpolated.py
--rw-r--r--   0 runner    (1001) docker     (121)     9946 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/src/exoplanet/light_curves/limb_dark.py
--rw-r--r--   0 runner    (1001) docker     (121)     2034 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/src/exoplanet/light_curves/secondary_eclipse.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 23:49:27.300967 exoplanet-0.5.3rc1/src/exoplanet/orbits/
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/src/exoplanet/orbits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1034 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/src/exoplanet/orbits/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     3684 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/src/exoplanet/orbits/dur_to_ecc.py
--rw-r--r--   0 runner    (1001) docker     (121)    32557 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/src/exoplanet/orbits/keplerian.py
--rw-r--r--   0 runner    (1001) docker     (121)     3661 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/src/exoplanet/orbits/simple.py
--rw-r--r--   0 runner    (1001) docker     (121)     7817 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/src/exoplanet/orbits/ttv.py
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/src/exoplanet/units.py
--rw-r--r--   0 runner    (1001) docker     (121)     2034 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/src/exoplanet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 23:49:27.300967 exoplanet-0.5.3rc1/src/exoplanet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2991 2022-10-12 23:49:27.000000 exoplanet-0.5.3rc1/src/exoplanet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-10-12 23:49:27.000000 exoplanet-0.5.3rc1/src/exoplanet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-12 23:49:27.000000 exoplanet-0.5.3rc1/src/exoplanet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-12 23:49:26.000000 exoplanet-0.5.3rc1/src/exoplanet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-10-12 23:49:27.000000 exoplanet-0.5.3rc1/src/exoplanet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-12 23:49:27.000000 exoplanet-0.5.3rc1/src/exoplanet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 23:49:27.300967 exoplanet-0.5.3rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/tests/citations_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     7478 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/tests/distributions_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2385 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/tests/estimators_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/tests/interp_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     8642 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/tests/light_curves_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 23:49:27.300967 exoplanet-0.5.3rc1/tests/orbits/
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/tests/orbits/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    20329 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/tests/orbits/keplerian_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2333 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/tests/orbits/simple_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2719 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/tests/orbits/ttv_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      974 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/tests/units_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      734 2022-10-12 23:49:17.000000 exoplanet-0.5.3rc1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:36:52.484014 exoplanet-0.6.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:36:52.468014 exoplanet-0.6.0rc2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:36:52.468014 exoplanet-0.6.0rc2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:36:52.468014 exoplanet-0.6.0rc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/.github/workflows/joss.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-16 15:36:52.484014 exoplanet-0.6.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:36:52.468014 exoplanet-0.6.0rc2/binder/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/binder/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/binder/runtime.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:36:52.472014 exoplanet-0.6.0rc2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:36:52.472014 exoplanet-0.6.0rc2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    33319 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/_static/big_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/_static/exoplanet.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/_static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18175 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    65535 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/_static/logo_shadow.png
+-rw-r--r--   0 runner    (1001) docker     (127)    80605 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/_static/orbit3D.png
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:36:52.472014 exoplanet-0.6.0rc2/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/tutorials/about.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/tutorials/autodiff.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/tutorials/citation.md
+-rw-r--r--   0 runner    (1001) docker     (127)    22485 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/tutorials/data-and-models.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17459 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/tutorials/intro-to-pymc.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/tutorials/intro-to-pymc3.md
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/tutorials/ipython_kernel_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/tutorials/light-delay.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/tutorials/reparameterization.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:36:52.472014 exoplanet-0.6.0rc2/docs/user/
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/user/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/user/dev.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/user/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/docs/user/multiprocessing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:36:52.472014 exoplanet-0.6.0rc2/joss/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:36:52.476014 exoplanet-0.6.0rc2/joss/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)   183655 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/joss/figures/figure.png
+-rw-r--r--   0 runner    (1001) docker     (127)    98285 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/joss/figures/joss-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/joss/metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    41317 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/joss/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (127)    13547 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/joss/paper.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:36:52.484014 exoplanet-0.6.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:36:52.464014 exoplanet-0.6.0rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:36:52.476014 exoplanet-0.6.0rc2/src/exoplanet/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/src/exoplanet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16274 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/src/exoplanet/citations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/src/exoplanet/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:36:52.476014 exoplanet-0.6.0rc2/src/exoplanet/distributions/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/src/exoplanet/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/src/exoplanet/distributions/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8831 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/src/exoplanet/distributions/eccentricity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12599 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/src/exoplanet/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 15:36:52.000000 exoplanet-0.6.0rc2/src/exoplanet/exoplanet_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/src/exoplanet/interp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:36:52.476014 exoplanet-0.6.0rc2/src/exoplanet/light_curves/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/src/exoplanet/light_curves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/src/exoplanet/light_curves/interpolated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9865 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/src/exoplanet/light_curves/limb_dark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/src/exoplanet/light_curves/secondary_eclipse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:36:52.480014 exoplanet-0.6.0rc2/src/exoplanet/orbits/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/src/exoplanet/orbits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/src/exoplanet/orbits/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/src/exoplanet/orbits/dur_to_ecc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32554 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/src/exoplanet/orbits/keplerian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/src/exoplanet/orbits/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/src/exoplanet/orbits/ttv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/src/exoplanet/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/src/exoplanet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:36:52.480014 exoplanet-0.6.0rc2/src/exoplanet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-16 15:36:52.000000 exoplanet-0.6.0rc2/src/exoplanet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-16 15:36:52.000000 exoplanet-0.6.0rc2/src/exoplanet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:36:52.000000 exoplanet-0.6.0rc2/src/exoplanet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:36:52.000000 exoplanet-0.6.0rc2/src/exoplanet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-16 15:36:52.000000 exoplanet-0.6.0rc2/src/exoplanet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 15:36:52.000000 exoplanet-0.6.0rc2/src/exoplanet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:36:52.480014 exoplanet-0.6.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/tests/citations_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15507 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/tests/distributions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/tests/estimators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/tests/interp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8524 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/tests/light_curves_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:36:52.480014 exoplanet-0.6.0rc2/tests/orbits/
+-rw-r--r--   0 runner    (1001) docker     (127)    20666 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/tests/orbits/keplerian_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/tests/orbits/simple_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/tests/orbits/ttv_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/tests/units_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-16 15:36:40.000000 exoplanet-0.6.0rc2/tox.ini
```

### Comparing `exoplanet-0.5.3rc1/.github/ISSUE_TEMPLATE/bug_report.md` & `exoplanet-0.6.0rc2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `exoplanet-0.5.3rc1/.github/ISSUE_TEMPLATE/feature_request.md` & `exoplanet-0.6.0rc2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `exoplanet-0.5.3rc1/.github/workflows/joss.yml` & `exoplanet-0.6.0rc2/.github/workflows/joss.yml`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     paths:
       - "joss/**"
 
 jobs:
   joss:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Generate .tex
         uses: docker://openjournals/paperdraft:latest
         with:
           args: joss/paper.md --defaults=metadata.yaml --to=latex --output=paper.tex
@@ -28,20 +28,20 @@
         with:
           args: joss/paper.md --defaults=metadata.yaml
         env:
           GIT_SHA: $GITHUB_SHA
           JOURNAL: joss
 
       - name: Upload the generated files as an artifact
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           path: joss
           name: joss
 
       - name: Deploy
         if: ${{ github.event_name != 'pull_request' }}
-        uses: peaceiris/actions-gh-pages@v3.8.0
+        uses: peaceiris/actions-gh-pages@v4.0.0
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_dir: ./joss
           force_orphan: true
           publish_branch: joss-compiled
```

### Comparing `exoplanet-0.5.3rc1/.github/workflows/tests.yml` & `exoplanet-0.6.0rc2/.github/workflows/tests.yml`

 * *Files 16% similar despite different names*

```diff
@@ -2,124 +2,86 @@
 
 on:
   push:
     branches:
       - main
     tags:
       - "*"
-    paths-ignore:
-      - "joss/**"
-      - "docs/**"
   pull_request:
 
 jobs:
   tests:
-    runs-on: ubuntu-latest
+    runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.9", "3.10"]
-        pymc-version: ["3.11", "dev"]
+        python-version: ["3.10"]
+        os: ["ubuntu-latest"]
+        session: ["test_pymc3", "test_pymc"]
         include:
+          - python-version: "3.9"
+            os: "ubuntu-latest"
+            session: "test_pymc3"
+          - python-version: "3.11"
+            os: "ubuntu-latest"
+            session: "test_pymc"
           - python-version: "3.10"
-            pymc-version: "beta"
+            os: "ubuntu-latest"
+            session: "lint"
 
     steps:
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
-      - name: Setup Python
-        uses: actions/setup-python@v4
+      - uses: actions/setup-python@v4
+        name: Install Python
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
-          python -m pip install -U coveralls coverage[toml] tox tox-gh-actions
+          python -m pip install -U nox
 
       - name: Run tests
-        run: python -m tox
-        env:
-          PYMC_VERSION: ${{ matrix.pymc-version }}
-
-      - name: Combine and upload coverage
-        run: |
-          python -m coverage combine
-          python -m coverage xml -i
-          python -m coveralls --service=github
-        env:
-          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-          COVERALLS_PARALLEL: true
-          COVERALLS_FLAG_NAME: py${{ matrix.python-version }}-pymc${{ matrix.pymc-version }}
-
-  coverage:
-    needs: tests
-    runs-on: ubuntu-latest
-    steps:
-      - name: Setup Python
-        uses: actions/setup-python@v4
-        with:
-          python-version: "3.9"
-      - name: Finish coverage collection
         run: |
-          python -m pip install -U pip
-          python -m pip install -U coveralls
-          python -m coveralls --finish
-        env:
-          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-
-  lint:
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v3
-        with:
-          fetch-depth: 0
-
-      - name: Setup Python
-        uses: actions/setup-python@v4
-        with:
-          python-version: "3.9"
-
-      - name: Install dependencies
-        run: |
-          python -m pip install -U pip
-          python -m pip install tox
-
-      - name: Lint the code
-        run: python -m tox -e lint
+          python -m nox --non-interactive \
+            --error-on-missing-interpreter \
+            --python ${{ matrix.python-version }} \
+            --session ${{ matrix.session }}
 
   build:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         name: Install Python
         with:
           python-version: "3.9"
       - name: Build sdist and wheel
         run: |
           python -m pip install -U pip
           python -m pip install -U build
           python -m build .
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
           path: dist/*
 
-  upload_pypi:
-    needs: [tests, lint, build]
+  publish:
+    environment:
+      name: pypi
+      url: https://pypi.org/p/exoplanet
+    permissions:
+      id-token: write
+    needs: [tests, build]
     runs-on: ubuntu-latest
-    if: startsWith(github.ref, 'refs/tags/')
+    if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/')
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
         with:
           name: artifact
           path: dist
-
-      - uses: pypa/gh-action-pypi-publish@v1.5.0
-        with:
-          user: __token__
-          password: ${{ secrets.pypi_password }}
+      - uses: pypa/gh-action-pypi-publish@v1.8.14
```

### Comparing `exoplanet-0.5.3rc1/.pre-commit-config.yaml` & `exoplanet-0.6.0rc2/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.3.0
+  rev: v4.6.0
   hooks:
   - id: trailing-whitespace
     exclude: src/exoplanet/theano_ops/lib/vendor
     exclude: docs/tutorials
   - id: end-of-file-fixer
     exclude: src/exoplanet/theano_ops/lib/vendor
     exclude_types: [json]
     exclude: docs/tutorials
   - id: debug-statements
     exclude: src/exoplanet/theano_ops/lib/vendor
     exclude: docs/tutorials
 
 - repo: https://github.com/PyCQA/isort
-  rev: "5.10.1"
+  rev: "5.13.2"
   hooks:
   - id: isort
     args: []
     additional_dependencies: [toml]
     exclude: docs/tutorials
 
 - repo: https://github.com/psf/black
-  rev: "22.10.0"
+  rev: "24.3.0"
   hooks:
   - id: black
 
 - repo: https://github.com/dfm/black_nbconvert
   rev: v0.4.0
   hooks:
   - id: black_nbconvert
 
 - repo: https://github.com/mwouts/jupytext
-  rev: v1.14.1
+  rev: v1.15.2
   hooks:
   - id: jupytext
     files: |
       (?x)^(docs/tutorials/.*\.md)$
     args: [--pipe, black]
     additional_dependencies:
       - black
```

### Comparing `exoplanet-0.5.3rc1/CITATION.cff` & `exoplanet-0.6.0rc2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `exoplanet-0.5.3rc1/CODE_OF_CONDUCT.md` & `exoplanet-0.6.0rc2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `exoplanet-0.5.3rc1/CONTRIBUTING.md` & `exoplanet-0.6.0rc2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `exoplanet-0.5.3rc1/HISTORY.rst` & `exoplanet-0.6.0rc2/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `exoplanet-0.5.3rc1/LICENSE` & `exoplanet-0.6.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `exoplanet-0.5.3rc1/PKG-INFO` & `exoplanet-0.6.0rc2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: exoplanet
-Version: 0.5.3rc1
-Summary: Fast and scalable MCMC for all your exoplanet needs
-Home-page: https://docs.exoplanet.codes
-Author: Daniel Foreman-Mackey
-Author-email: foreman.mackey@gmail.com
-Maintainer: Daniel Foreman-Mackey
-Maintainer-email: foreman.mackey@gmail.com
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: extras
-Provides-Extra: test
-Provides-Extra: docs
-License-File: LICENSE
-
 <p align="center">
   <img width="240" src="https://raw.githubusercontent.com/exoplanet-dev/exoplanet/main/docs/_static/logo.png">
   <br><br>
   <a href="https://github.com/exoplanet-dev/exoplanet/actions/workflows/tests.yml">
     <img src="https://github.com/exoplanet-dev/exoplanet/actions/workflows/tests.yml/badge.svg" alt="Tests">
   </a>
   <a href="https://docs.exoplanet.codes">
@@ -37,27 +13,28 @@
 </p>
 
 # exoplanet
 
 Fast & scalable MCMC for all your exoplanet needs! _exoplanet_ is a toolkit for
 probabilistic modeling of time series data in astronomy with a focus on
 observations of [exoplanets](https://en.wikipedia.org/wiki/Exoplanet), using
-[PyMC3](https://docs.pymc.io). _PyMC3_ is a flexible and high-performance model
-building language and inference engine that scales well to problems with a large
-number of parameters. _exoplanet_ extends _PyMC3_'s language to support many of
-the custom functions and distributions required when fitting exoplanet datasets.
+[PyMC](https://www.pymc.io). _PyMC_ is a flexible and high-performance
+model-building language and inference engine that scales well to problems with a
+large number of parameters. _exoplanet_ extends _PyMC_'s language to support
+many of the custom functions and distributions required when fitting exoplanet
+datasets.
 
 Read the full documentation at [docs.exoplanet.codes](https://docs.exoplanet.codes).
 
 ## Installation
 
 The quickest way to get started is to use [pip](https://pip.pypa.io):
 
 ```bash
-python -m pip install exoplanet
+python -m pip install "exoplanet[pymc]"
 ```
 
 Note that you will need Python (>=3.6) installed for this to work, but then this
 will install all the required dependencies.
 
 Check out the [main installation documentation
 page](https://docs.exoplanet.codes/en/latest/user/install/) for more options.
@@ -67,11 +44,11 @@
 Check out the tutorials and API docs on [the docs
 page](https://docs.exoplanet.codes) for example usage and much more info. You
 can also find more in-depth examples on the [exoplanet case studies
 page](https://gallery.exoplanet.codes).
 
 ## Contributing
 
-_exoplanet_ is an open source project and we would love it if you wanted to
+_exoplanet_ is an open-source project, and we would love it if you wanted to
 contribute. Check out [the developer
 documentation](https://docs.exoplanet.codes/en/latest/user/dev/) for more info
 about getting started.
```

#### html2text {}

```diff
@@ -1,35 +1,24 @@
-Metadata-Version: 2.1 Name: exoplanet Version: 0.5.3rc1 Summary: Fast and
-scalable MCMC for all your exoplanet needs Home-page: https://
-docs.exoplanet.codes Author: Daniel Foreman-Mackey Author-email:
-foreman.mackey@gmail.com Maintainer: Daniel Foreman-Mackey Maintainer-email:
-foreman.mackey@gmail.com License: MIT Classifier: Development Status :: 4 -
-Beta Classifier: Intended Audience :: Developers Classifier: Intended Audience
-:: Science/Research Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python Classifier: Programming Language :: Python :: 3 Requires-Python:
->=3.6 Description-Content-Type: text/markdown Provides-Extra: extras Provides-
-Extra: test Provides-Extra: docs License-File: LICENSE
  [https://raw.githubusercontent.com/exoplanet-dev/exoplanet/main/docs/_static/
                                    logo.png]
 
                             _[_T_e_s_t_s_]_[_D_o_c_s_]_[_C_o_v_e_r_a_g_e_]
 # exoplanet Fast & scalable MCMC for all your exoplanet needs! _exoplanet_ is a
 toolkit for probabilistic modeling of time series data in astronomy with a
 focus on observations of [exoplanets](https://en.wikipedia.org/wiki/Exoplanet),
-using [PyMC3](https://docs.pymc.io). _PyMC3_ is a flexible and high-performance
-model building language and inference engine that scales well to problems with
-a large number of parameters. _exoplanet_ extends _PyMC3_'s language to support
+using [PyMC](https://www.pymc.io). _PyMC_ is a flexible and high-performance
+model-building language and inference engine that scales well to problems with
+a large number of parameters. _exoplanet_ extends _PyMC_'s language to support
 many of the custom functions and distributions required when fitting exoplanet
 datasets. Read the full documentation at [docs.exoplanet.codes](https://
 docs.exoplanet.codes). ## Installation The quickest way to get started is to
-use [pip](https://pip.pypa.io): ```bash python -m pip install exoplanet ```
-Note that you will need Python (>=3.6) installed for this to work, but then
+use [pip](https://pip.pypa.io): ```bash python -m pip install "exoplanet[pymc]"
+``` Note that you will need Python (>=3.6) installed for this to work, but then
 this will install all the required dependencies. Check out the [main
 installation documentation page](https://docs.exoplanet.codes/en/latest/user/
 install/) for more options. ## Usage Check out the tutorials and API docs on
 [the docs page](https://docs.exoplanet.codes) for example usage and much more
 info. You can also find more in-depth examples on the [exoplanet case studies
-page](https://gallery.exoplanet.codes). ## Contributing _exoplanet_ is an open
-source project and we would love it if you wanted to contribute. Check out [the
-developer documentation](https://docs.exoplanet.codes/en/latest/user/dev/) for
-more info about getting started.
+page](https://gallery.exoplanet.codes). ## Contributing _exoplanet_ is an open-
+source project, and we would love it if you wanted to contribute. Check out
+[the developer documentation](https://docs.exoplanet.codes/en/latest/user/dev/
+) for more info about getting started.
```

### Comparing `exoplanet-0.5.3rc1/docs/Makefile` & `exoplanet-0.6.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `exoplanet-0.5.3rc1/docs/_static/big_logo.png` & `exoplanet-0.6.0rc2/docs/_static/big_logo.png`

 * *Files identical despite different names*

### Comparing `exoplanet-0.5.3rc1/docs/_static/favicon.png` & `exoplanet-0.6.0rc2/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `exoplanet-0.5.3rc1/docs/_static/logo.png` & `exoplanet-0.6.0rc2/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `exoplanet-0.5.3rc1/docs/_static/logo_shadow.png` & `exoplanet-0.6.0rc2/docs/_static/logo_shadow.png`

 * *Files identical despite different names*

### Comparing `exoplanet-0.5.3rc1/docs/_static/orbit3D.png` & `exoplanet-0.6.0rc2/docs/_static/orbit3D.png`

 * *Files identical despite different names*

### Comparing `exoplanet-0.5.3rc1/docs/conf.py` & `exoplanet-0.6.0rc2/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # General stuff
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.mathjax",
     "myst_nb",
+    "IPython.sphinxext.ipython_console_highlighting",
 ]
 
 myst_enable_extensions = ["dollarmath", "colon_fence"]
 
 templates_path = ["_templates"]
 source_suffix = ".rst"
 master_doc = "index"
```

### Comparing `exoplanet-0.5.3rc1/docs/index.rst` & `exoplanet-0.6.0rc2/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 exoplanet
 =========
 
 *exoplanet* is a toolkit for probabilistic modeling of time series data in
 astronomy with a focus on observations of `exoplanets
-<https://en.wikipedia.org/wiki/Exoplanet>`_, using `PyMC3
-<https://docs.pymc.io>`_. *PyMC3* is a flexible and high-performance model
+<https://en.wikipedia.org/wiki/Exoplanet>`_, using `PyMC
+<https://www.pymc.io>`_. *PyMC* is a flexible and high-performance model
 building language and inference engine that scales well to problems with a large
-number of parameters. *exoplanet* extends *PyMC3*'s language to support many of
+number of parameters. *exoplanet* extends *PyMC*'s language to support many of
 the custom functions and distributions required when fitting exoplanet datasets.
 These features include:
 
 * A fast and robust solver for Kepler's equation.
 * Scalable Gaussian Processes using `celerite <https://celerite2.readthedocs.io>`_.
 * Fast and accurate limb darkened light curves using `starry
   <https://rodluger.github.io/starry>`_.
@@ -40,45 +40,44 @@
 
    🖥 For general installation and basic usage, continue scrolling to the table of
    contents below.
 
    🖼 For more in depth examples of *exoplanet* used for more realistic problems,
    go to the `Case studies page <https://gallery.exoplanet.codes>`_.
 
-   📈 For more information about scalable Gaussian Processes in PyMC3 (this was
+   📈 For more information about scalable Gaussian Processes in PyMC (this was
    previously implemented as part of *exoplanet*), see the `celerite2 documentation
    page <https://celerite2.readthedocs.io>`_.
 
-   👉 For helper functions and PyMC3 extras that used to be implemented as part of
-   *exoplanet*, see the `pymc3-ext project
-   <https://github.com/exoplanet-dev/pymc3-ext>`_.
+   👉 For helper functions and PyMC extras that used to be implemented as part of
+   *exoplanet*, see the `pymc-ext project
+   <https://github.com/exoplanet-dev/pymc-ext>`_.
 
 
 Contents
 --------
 
 .. toctree::
    :maxdepth: 1
    :caption: User Guide
 
    user/install
    tutorials/citation.md
-   user/theano
    user/multiprocessing
    user/api
    user/dev
    changes.rst
 
 .. toctree::
    :maxdepth: 1
    :caption: Tutorials
 
    tutorials/about.md
    tutorials/autodiff.md
-   tutorials/intro-to-pymc3.md
+   tutorials/intro-to-pymc.md
    tutorials/data-and-models.md
    tutorials/light-delay.md
    tutorials/reparameterization.md
    Case studies <https://gallery.exoplanet.codes>
    celerite2 <https://celerite2.readthedocs.io>
```

### Comparing `exoplanet-0.5.3rc1/docs/tutorials/about.md` & `exoplanet-0.6.0rc2/docs/tutorials/about.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 ---
 jupytext:
   text_representation:
     extension: .md
     format_name: myst
     format_version: 0.13
-    jupytext_version: 1.14.1
+    jupytext_version: 1.15.2
 kernelspec:
-  display_name: Python 3
+  display_name: Python 3 (ipykernel)
   language: python
   name: python3
 ---
 
 # About these tutorials
 
 +++
 
-This and the following tutorials are automatically executed with every change of the code to make sure that they are always up to date with the code.
-As a result, they are designed to require only a relatively small amount of computation time; when using `exoplanet` for research you will probably find that your runtimes are longer.
+This and the following tutorials are automatically executed with every change of the code to make sure that they are always up-to-date with the code.
+As a result, they are designed to require only a relatively small amount of computation time; when using `exoplanet` for research you will probably find that your run times are longer.
 For more in-depth tutorials with real-world applications and real data, check out the [Case Studies page](https://gallery.exoplanet.codes).
 
 At the top of each tutorial, you'll find a cell like the following that indicates the version of `exoplanet` that was used to generate the tutorial:
 
 ```{code-cell}
 import exoplanet
 
 exoplanet.utils.docs_setup()
 print(f"exoplanet.__version__ = '{exoplanet.__version__}'")
 ```
 
-That cell also includes a call to the `exoplanet.utils.docs_setup` function that will squash some warnings (these are generally caused by Theano/Aesara; see {ref}`theano` for more info) and set up our `matplotlib` style.
+That cell also includes a call to the `exoplanet.utils.docs_setup` function that will squash some warnings (these are generally caused by Theano/PyTensor) and set up our `matplotlib` style.
 
-To exectute a tutorial on your own, you can click on the buttons at the top right or this page to launch the notebook using [Binder](https://mybinder.org) or download the `.ipynb` file directly.
+To execute a tutorial on your own, you can click on the buttons at the top right or this page to launch the notebook using [Binder](https://mybinder.org) or download the `.ipynb` file directly.
 
 ```{code-cell}
 
 ```
```

### Comparing `exoplanet-0.5.3rc1/docs/tutorials/autodiff.md` & `exoplanet-0.6.0rc2/docs/tutorials/autodiff.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ---
 jupytext:
   text_representation:
     extension: .md
     format_name: myst
     format_version: 0.13
-    jupytext_version: 1.14.1
+    jupytext_version: 1.15.2
 kernelspec:
-  display_name: Python 3
+  display_name: Python 3 (ipykernel)
   language: python
   name: python3
 ---
 
 (autodiff)=
 
 # Automatic differentation & gradient-based inference
@@ -18,33 +18,33 @@
 ```{code-cell}
 import exoplanet
 
 exoplanet.utils.docs_setup()
 print(f"exoplanet.__version__ = '{exoplanet.__version__}'")
 ```
 
-The major selling point of `exoplanet` compared to other similar libraries is that it integrates with the `PyMC3` probabilistic modeling framework.
-`PyMC3` offers gradient-based inference algorithms (more on these below) that can be more computationally efficient (per effective sample) than other tools commonly used for probabilistic inference in astrophysics.
+The major selling point of `exoplanet` compared to other similar libraries is that it integrates with the `PyMC` probabilistic modeling framework.
+`PyMC` offers gradient-based inference algorithms (more on these below) that can be more computationally efficient (per effective sample) than other tools commonly used for probabilistic inference in astrophysics.
 When I am writing this, gradient-based inference methodology is not widely used in astro because it can be difficult to compute the relevant gradients (derivatives of your log probability function with respect to the parameters).
-`PyMC3` (and many other frameworks like it) handle this issue using [automatic differentiation (AD)](https://en.wikipedia.org/wiki/Automatic_differentiation), a method (or collection of methods) for automatically propagating derivatives through your code.
+`PyMC` (and many other frameworks like it) handle this issue using [automatic differentiation (AD)](https://en.wikipedia.org/wiki/Automatic_differentiation), a method (or collection of methods) for automatically propagating derivatives through your code.
 
 It's beyond the scope of this tutorial to go into too many details about AD and most users of `exoplanet` shouldn't need to interact with this too much, but this should at least give you a little taste of the kinds of things AD can do for you and demonstrate how this translates into efficient inference with probabilistic models.
-The main thing that I want to emphasize here is that AD is not the same as *symbolic differentiation* (it's not going to provide you with a mathematical expression for your gradients), but it's also not the same as numerical methods like [finite difference](https://en.wikipedia.org/wiki/Finite_difference).
+The main thing that I want to emphasize here is that AD is not the same as _symbolic differentiation_ (it's not going to provide you with a mathematical expression for your gradients), but it's also not the same as numerical methods like [finite difference](https://en.wikipedia.org/wiki/Finite_difference).
 Using AD to evaluate the gradients of your model will generally be faster, more efficient, and more numerically stable than alternatives, but there are always exceptions to any rule.
 There are times when providing your AD framework with a custom implementation and/or differentation rule for a particular function is beneficial in terms of cost and stability.
 `exoplanet` is designed to provide these custom implementations only where it is useful (e.g. solving Kepler's equation or evaluating limb-darkened light curves) and then rely on the existing AD toolkit elsewhere.
 
-## Automatic differentation in Theano/Aesara
+## Automatic differentiation in PyTensor
 
-Let's start by giving a quick taste for how AD works in the context of `PyMC3` and `exoplanet`.
-`PyMC3` is built on top of a library called `Aesara` (formerly `Theano`, see {ref}`theano`) that was designed for AD and fast linear algebra in the context of neural networks.
+Let's start by giving a quick taste for how AD works in the context of `PyMC` and `exoplanet`.
+`PyMC` is built on top of a library called `PyTensor`, a fork of the now unmaintained Theano library that was designed for AD and fast linear algebra in the context of neural networks.
 The learning curve can be steep because your code ends up looking a little different from the usual way you would write Python code.
-(If you're looking for something more "Pythonic", [JAX](https://github.com/google/jax) might be a good alternative, but for our purposes we'll stick with `Aesara`.)
-In `Aesara`, you start be defining the *relationships* between variables and then ask to evaluate a variable using this "graph".
-This might seem a little counterintuitive and you hopefully won't have to worry about this too much, but it can be a handy workflow because `Aesara` will compile and optimize your model in the background (generally making it faster).
+(If you're looking for something more "Pythonic", [JAX](https://github.com/google/jax) might be a good alternative, but for our purposes, we'll stick with `PyTensor`.)
+In `PyTensor`, you start by defining the _relationships_ between variables and then ask to evaluate a variable using this "graph".
+This might seem a little counterintuitive, and you hopefully won't have to worry about this too much, but it can be a handy workflow because `PyTensor` will compile and optimize your model in the background (generally making it faster).
 This structure allows us to evaluate the derivative of some variable with respect to another.
 
 Here's a simple example where we define a relationship between two variables `x` and `y`:
 
 $$
 y = \exp\left[\sin\left(\frac{2\,\pi\,x}{3}\right)\right]
 $$
@@ -55,28 +55,28 @@
 $$
 \frac{\mathrm{d}y}{\mathrm{d}x} = \frac{2\,\pi}{3}\,\exp\left[\sin\left(\frac{2\,\pi\,x}{3}\right)\right]\,\cos\left(\frac{2\,\pi\,x}{3}\right)
 $$
 
 ```{code-cell}
 import numpy as np
 import matplotlib.pyplot as plt
-from aesara_theano_fallback import aesara
-import aesara_theano_fallback.tensor as at
+import pytensor
+import pytensor.tensor as pt
 
 # Define the relationship between two variables x and y=f(x)
-x_ = at.vector("x")
-y_ = at.exp(at.sin(2 * np.pi * x_ / 3.0))
+x_ = pt.vector("x")
+y_ = pt.exp(pt.sin(2 * np.pi * x_ / 3.0))
 
-# Here aesara will compile a function to evaluate y
-func = aesara.function([x_], y_)
+# Here pytensor will compile a function to evaluate y
+func = pytensor.function([x_], y_)
 
 # Request the gradient of y with respect to x
 # Note the call to `sum`. This is a bit of a cheat since by
-# default Aesara only computes gradients of a *scalar* function
-grad = aesara.function([x_], aesara.grad(at.sum(y_), x_))
+# default pytensor only computes gradients of a *scalar* function
+grad = pytensor.function([x_], pytensor.grad(pt.sum(y_), x_))
 
 # Plot the function and its derivative
 x = np.linspace(-3, 3, 500)
 plt.plot(x, func(x), "k", lw=1, label="f(x)")
 plt.plot(x, grad(x), "C0", label="df(x)/dx; AD", lw=3)
 
 # Overplot the symbolic derivative for comparison
@@ -96,94 +96,95 @@
 
 This example is obviously pretty artificial, but I think that you can imagine how something like this would start to come in handy when your models get more complicated.
 In particular, I think that you'll probably pretty regularly find yourself experimenting with different choices of parameters and it would be a real pain to be required to re-write all your derivative code for every new choice of parameterization.
 
 ## Gradient-based inference
 
 Now that we have a way of easily evaluating the derivatives of scalar functions, we have a wide array of new inference algorithms at our disposal.
-For example, if we use Aesara to evaluate our log probability function, we could pass the value and gradient to [`scipy.optimize.minimize`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.minimize.html) in order to find the maximum likelihood or maximum a posteriori parameters.
-But, the point of `exoplanet` is that it integrates with `PyMC3` which provides implementations of various gradient-based Markov chain Monte Carlo (MCMC) methods like [Hamiltonian Monte Carlo](https://en.wikipedia.org/wiki/Hamiltonian_Monte_Carlo) and [No U-Turn Sampling](https://arxiv.org/abs/1111.4246).
-`PyMC3` also supports gradient-based methods for [variational inference](https://en.wikipedia.org/wiki/Variational_Bayesian_methods), but (so far) `exoplanet` had mostly been used for MCMC.
+For example, if we use PyTensor to evaluate our log probability function, we could pass the value and gradient to [`scipy.optimize.minimize`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.minimize.html) in order to find the maximum likelihood or maximum a posteriori parameters.
+But, the point of `exoplanet` is that it integrates with `PyMC` which provides implementations of various gradient-based Markov chain Monte Carlo (MCMC) methods like [Hamiltonian Monte Carlo](https://en.wikipedia.org/wiki/Hamiltonian_Monte_Carlo) and [No U-Turn Sampling](https://arxiv.org/abs/1111.4246).
+`PyMC` also supports gradient-based methods for [variational inference](https://en.wikipedia.org/wiki/Variational_Bayesian_methods), but (so far) `exoplanet` had mostly been used for MCMC.
 
-Take a look at {ref}`intro-to-pymc3` for some specific introductory examples of using `PyMC3` for MCMC, but the general motivation for using `PyMC3` (instead of [emcee](https://emcee.readthedocs.io) or [dynesty](https://dynesty.readthedocs.io), for example) is that it can be far more computationally efficient (per effective sample), especially when your model has more than a couple of parameters.
-We're not going to do a systematic study of the relative performance of different methods because that is fraught and can be problem specific, but let's look at another very artificial example where we compare the performance of sampling a 50-dimensional Gaussian using `PyMC3` and [`emcee`](https://emcee.readthedocs.io).
+Take a look at {ref}`intro-to-pymc` for some specific introductory examples of using `PyMC` for MCMC, but the general motivation for using `PyMC` (instead of [emcee](https://emcee.readthedocs.io) or [dynesty](https://dynesty.readthedocs.io), for example) is that it can be far more computationally efficient (per effective sample), especially when your model has more than a couple of parameters.
+We're not going to do a systematic study of the relative performance of different methods because that is fraught and can be problem specific, but let's look at another very artificial example where we compare the performance of sampling a 50-dimensional Gaussian using `PyMC` and [`emcee`](https://emcee.readthedocs.io).
 
 ```{code-cell}
 import time
 import emcee
 import logging
-import pymc3 as pm
+import pymc as pm
 import arviz as az
-import pymc3_ext as pmx
+import pymc_ext as pmx
 
-# Make PyMC3 less noisy just for this example!
-logger = logging.getLogger("pymc3")
+logger = logging.getLogger("pymc")
 logger.setLevel(logging.ERROR)
 
-# First define and sample the model using PyMC3
+# First define and sample the model using PyMC
 with pm.Model() as model:
     pm.Normal("x", shape=50)
 
     # Run a fake chain just to get everything to compile
     pm.sample(
         tune=1, draws=1, chains=1, return_inferencedata=True, progressbar=False
     )
 
     # Run and time the sampling
     start = time.time()
     pymc_trace = pm.sample(
         tune=1000,
-        draws=1000,
+        draws=5000,
         chains=2,
         cores=1,
         return_inferencedata=True,
         progressbar=False,
     )
     pymc_time = time.time() - start
 
     # Compute the cost per sample
     pymc_per_eff = pymc_time / np.mean(az.summary(pymc_trace)["ess_bulk"])
 
+
 # Then sample the same model using emcee
-func = pmx.get_theano_function_for_var(model.logpt, model=model)
+func = pmx.utils.Evaluator(model.logp(), model=model)
 
 
 def logp(theta):
-    return func(theta)
+    return func({"x": theta})
 
 
-init = np.random.randn(124, model.ndim)
+ndim = sum([v.size for v in model.initial_point().values()])
+init = np.random.randn(124, ndim)
 nwalkers, ndim = init.shape
 sampler = emcee.EnsembleSampler(nwalkers, ndim, logp)
 
 start = time.time()
 init = sampler.run_mcmc(init, 1000)
 sampler.reset()
-sampler.run_mcmc(init, 3000)
+sampler.run_mcmc(init, 5000)
 emcee_time = time.time() - start
 
 emcee_trace = az.from_emcee(sampler=sampler)
 emcee_per_eff = emcee_time / np.mean(az.summary(emcee_trace)["ess_bulk"])
 ```
 
 After running these chains, we can compare the relative performance (remember that this is a very artificial example so caveats, small print, yadda, etc.).
 To compare the performance of different MCMC samplers, the best metric is the computational cost per effective sample (for the parameter/function that you most care about).
-In this case, we'll look at the total runtime (including burn-in) divided by an estaimte of the the mean effective sample size across all 50 dimensions (lower is better):
+In this case, we'll look at the total runtime (including burn-in) divided by an estimate of the mean effective sample size across all 50 dimensions (lower is better):
 
 ```{code-cell}
 print(
-    f"For PyMC3, the runtime per effective sample is: {pymc_per_eff * 1e3:.2f} ms"
+    f"For PyMC, the runtime per effective sample is: {pymc_per_eff * 1e3:.2f} ms"
 )
 print(
     f"For emcee, the runtime per effective sample is: {emcee_per_eff * 1e3:.2f} ms"
 )
 ```
 
-So, in this case, PyMC3 is a few order of magnitude more efficient.
-As your models get more complex (in terms of computational cost, number of parameters, and the geometry of your parameter space), your mileage might vary, but my experience is that using `PyMC3` is almost always a good idea if you can!
+So, in this case, `PyMC` is a few order of magnitude more efficient.
+As your models get more complex (in terms of computational cost, number of parameters, and the geometry of your parameter space), your mileage might vary, but my experience is that using `PyMC` is almost always a good idea if you can!
 
 :::{tip}
 If you find that your model is not sampling well, this is almost always caused by **parameterization issues** and you'll probably get drastically better performance with some reparameterization.
 See {ref}`reparameterization` for some tips and tricks.
 :::
 
 ```{code-cell}
```

### Comparing `exoplanet-0.5.3rc1/docs/tutorials/citation.md` & `exoplanet-0.6.0rc2/docs/tutorials/citation.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,57 @@
 ---
 jupytext:
   text_representation:
     extension: .md
     format_name: myst
     format_version: 0.13
-    jupytext_version: 1.14.1
+    jupytext_version: 1.15.2
 kernelspec:
-  display_name: Python 3
+  display_name: Python 3 (ipykernel)
   language: python
   name: python3
 ---
 
 # Citing exoplanet & its dependencies
 
 +++
 
 The _exoplanet_ package is mostly just glue that connects many other ideas and software.
 In a situation like this, it can be easy to forget about the important infrastructure upon which our science is built.
-In order to make sure that you can easily give credit where credit is due, we have tried to make it as painless as possible to work out which citations are expected for a model fit using _exoplanet_ by including a {func}`exoplanet.citations.get_citations_for_model` function that introspects the current PyMC3 model and constructs a list of citations for the functions used in that model.
+In order to make sure that you can easily give credit where credit is due, we have tried to make it as painless as possible to work out which citations are expected for a model fit using _exoplanet_ by including a {func}`exoplanet.citations.get_citations_for_model` function that introspects the current PyMC model and constructs a list of citations for the functions used in that model.
 
 For example, you might compute a quadratically limb darkened light curve using `starry` (via the {class}`exoplanet.LimbDarkLightCurve` class):
 
 ```{code-cell}
-import pymc3 as pm
+import pymc as pm
 import exoplanet as xo
 
 with pm.Model() as model:
-    u = xo.distributions.QuadLimbDark("u")
+    u = xo.distributions.quad_limb_dark("u")
     orbit = xo.orbits.KeplerianOrbit(period=10.0)
     light_curve = xo.LimbDarkLightCurve(u[0], u[1])
     transit = light_curve.get_light_curve(r=0.1, orbit=orbit, t=[0.0, 0.1])
 
     txt, bib = xo.citations.get_citations_for_model()
 ```
 
-The {func}`exoplanet.citations.get_citations_for_model` function would generate an acknowledgement that cites:
+The {func}`exoplanet.citations.get_citations_for_model` function would generate an acknowledgment that cites:
 
-- [PyMC3](https://docs.pymc.io/#citing-pymc3): for the inference engine and modeling framework,
-- [Theano/Aesara](https://aesara.readthedocs.io/en/latest/citation.html): for the numerical infrastructure,
+- PyMC: for the inference engine and modeling framework,
 - [AstroPy](http://www.astropy.org/acknowledging.html): for units and constants,
 - [Kipping (2013)](https://arxiv.org/abs/1308.0009): for the reparameterization of the limb darkening parameters for a quadratic law, and
 - [Luger, et al. (2018)](https://arxiv.org/abs/1810.06559): for the light curve calculation.
 
-The first output from {func}`exoplanet.citations.get_citations_for_model` gives the acknowledgement text:
+The first output from {func}`exoplanet.citations.get_citations_for_model` gives the acknowledgment text:
 
 ```{code-cell}
 print(txt)
 ```
 
-And the second output is a string with BibTeX entries for each of the citations in the acknowledgement text:
+And the second output is a string with BibTeX entries for each of the citations in the acknowledgment text:
 
 ```{code-cell}
 print(bib.split("\n\n")[0] + "\n\n...")
 ```
 
 ```{code-cell}
```

### Comparing `exoplanet-0.5.3rc1/docs/tutorials/data-and-models.md` & `exoplanet-0.6.0rc2/docs/tutorials/data-and-models.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ---
 jupytext:
   text_representation:
     extension: .md
     format_name: myst
     format_version: 0.13
-    jupytext_version: 1.14.1
+    jupytext_version: 1.15.2
 kernelspec:
-  display_name: Python 3
+  display_name: Python 3 (ipykernel)
   language: python
   name: python3
 ---
 
 (data-and-models)=
 
 # Data & models
@@ -19,15 +19,15 @@
 import exoplanet
 
 exoplanet.utils.docs_setup()
 print(f"exoplanet.__version__ = '{exoplanet.__version__}'")
 ```
 
 This tutorial provides an overview of the kinds of datasets that `exoplanet` has been designed to model.
-It's worth noting that this is certainly not a comprehensive list and `exoplanet` is designed to be *low-level* library that can be built on top of to support new use cases.
+It's worth noting that this is certainly not a comprehensive list and `exoplanet` is designed to be _low-level_ library that can be built on top of to support new use cases.
 
 :::{tip}
 For real world use cases and examples, check out the [Case Studies](https://gallery.exoplanet.codes) page.
 :::
 
 +++
 
@@ -59,15 +59,15 @@
 # Get the position and velocity as a function of time
 t = np.linspace(0, 20, 5000)
 x, y, z = orbit.get_relative_position(t)
 vx, vy, vz = orbit.get_star_velocity(t)
 
 # Plot the coordinates
 # Note the use of `.eval()` throughout since the coordinates are all
-# Aesara/Theano objects
+# PyTensor objects
 fig, axes = plt.subplots(2, 1, figsize=(8, 8), sharex=True)
 ax = axes[0]
 ax.plot(t, x.eval(), label="x")
 ax.plot(t, y.eval(), label="y")
 ax.plot(t, z.eval(), label="z")
 ax.set_ylabel("position of orbiting body [$R_*$]")
 ax.legend(fontsize=10, loc=1)
@@ -78,20 +78,20 @@
 ax.plot(t, vz.eval(), label="$v_z$")
 ax.set_xlim(t.min(), t.max())
 ax.set_xlabel("time [days]")
 ax.set_ylabel("velocity of central [$R_*$/day]")
 _ = ax.legend(fontsize=10, loc=1)
 ```
 
-The key feture of `exoplanet` is that all of the parameters to a `KeplerianOrbit` can be `PyMC3` variables.
-This means that these elements are now something that you can *infer*.
-For example, if we want to fit for the orbital period, we can define a `PyMC3` model like the following:
+The key feature of `exoplanet` is that all of the parameters to a `KeplerianOrbit` can be `PyMC` variables.
+This means that these elements are now something that you can _infer_.
+For example, if we want to fit for the orbital period, we can define a `PyMC` model like the following:
 
 ```{code-cell}
-import pymc3 as pm
+import pymc as pm
 
 with pm.Model():
     log_period = pm.Normal("log_period", mu=np.log(10), sigma=2.0)
     orbit = xo.orbits.KeplerianOrbit(
         period=pm.math.exp(log_period),  # ...
     )
 
@@ -136,16 +136,16 @@
       Z\\
     \end{array}
   \right ].
 $$
 
 We choose to orient the $\hat{\boldsymbol{X}}$ unit vector in the north direction, $\hat{\boldsymbol{Y}}$ in the east direction, and $\hat{\boldsymbol{Z}}$ towards the observer. Under this convention, the inclination of an orbit is defined by the dot-product of the orbital angular momentum vector with $\hat{\boldsymbol{Z}}$, conforming to the common astrometric convention that a zero inclination ($i = 0$) orbit is face-on, with the test body orbiting in a counter-clockwise manner around the primary body.
 
-In the stellar and exoplanetary fields, there is less agreement on which  segment of the line of nodes is defined as the *ascending* node.
-We choose to define the ascending node as the point where the orbiting body crosses the plane of the sky moving *away* from the observer (i.e., crossing from $Z > 0$ to $Z< 0$).
+In the stellar and exoplanetary fields, there is less agreement on which segment of the line of nodes is defined as the _ascending_ node.
+We choose to define the ascending node as the point where the orbiting body crosses the plane of the sky moving _away_ from the observer (i.e., crossing from $Z > 0$ to $Z< 0$).
 This convention has historically been the choice of the visual binary field; the opposite convention occasionally appears in exoplanet and planetary studies.
 
 To implement the transformation from perifocal frame to observer frame, we consider the rotation matrices
 
 $$
   \boldsymbol{P}_x(\phi) = \left [
   \begin{array}{ccc}
@@ -160,15 +160,15 @@
   \begin{array}{ccc}
     \cos \phi & - \sin \phi & 0\\
     \sin \phi & \cos \phi & 0 \\
     0 & 0 & 1 \\
     \end{array}\right].
 $$
 
-which result in a *clockwise* rotation of the axes, as defined using the right hand rule.
+which result in a _clockwise_ rotation of the axes, as defined using the right hand rule.
 
 This means when we look down the $z$-axis, for a positive angle $\phi$, it would be as if the $x$ and $y$ axes rotated clockwise.
 In order to find out what defines counter-clockwise when considering the other rotations, we look to the right hand rule and cross products of the axes unit vectors.
 Since $\hat{\boldsymbol{x}} \times \hat{\boldsymbol{y}} = \hat{\boldsymbol{z}}$, when looking down the $z$ axis the direction of the $x$-axis towards the $y$-axis defines counter clockwise.
 Similarly, we have $\hat{\boldsymbol{y}} \times \hat{\boldsymbol{z}} = \hat{\boldsymbol{x}}$, and $\hat{\boldsymbol{z}} \times \hat{\boldsymbol{x}} = \hat{\boldsymbol{y}}$.
 
 To convert a position $\boldsymbol{r}$ in the perifocal frame to the observer frame $\boldsymbol{R}$ (referencing the figure above), three rotations are required:
@@ -203,19 +203,19 @@
 $$
 
 The central body is defined by any two of radius $R_\star$, mass $M_\star$, or density $\rho_\star$.
 The third physical parameter can always be computed using the other two so `exoplanet` will throw an error if three are given (even if they are numerically self-consistent).
 
 The orbits are then typically defined by (check out the docstring {class}`exoplanet.orbits.KeplerianOrbit` for all the options):
 
-* the period $P$ or semi-major axis $a$ of the orbit,
-* the time of conjunction $t_0$ or time of periastron passage $t_\mathrm{p}$,
-* the planet's radius $R_\mathrm{pl}$ and mass $M_\mathrm{pl}$,
-* the eccentricity $e$, argument of periastron $\omega$ and the longitude of ascending node $\Omega$, and
-* the inclination of the orbital plane $i$ or the impact parameter $b$.
+- the period $P$ or semi-major axis $a$ of the orbit,
+- the time of conjunction $t_0$ or time of periastron passage $t_\mathrm{p}$,
+- the planet's radius $R_\mathrm{pl}$ and mass $M_\mathrm{pl}$,
+- the eccentricity $e$, argument of periastron $\omega$ and the longitude of ascending node $\Omega$, and
+- the inclination of the orbital plane $i$ or the impact parameter $b$.
 
 A `KeplerianOrbit` object in `exoplanet` will always be fully specified.
 For example, if the orbit is defined using the period $P$, the semi-major axis $a$ will be computed using Kepler's third law.
 
 +++
 
 (data-and-models/rvs)=
@@ -223,95 +223,95 @@
 ## Radial velocities
 
 A {class}`exoplanet.orbits.KeplerianOrbit` can be used to compute the expected radial velocity time series for a given set of parameters.
 One typical parameterization for a radial velocity fit would look something like this:
 
 ```{code-cell}
 import arviz as az
-import pymc3_ext as pmx
-import aesara_theano_fallback.tensor as tt
+import pymc_ext as pmx
+import pytensor.tensor as pt
 
 # Create a dummy dataset
 random = np.random.default_rng(1234)
 t_plot = np.linspace(0, 50, 500)
 t = np.sort(random.uniform(0, 50, 20))
 rv_err = 0.5 + np.zeros_like(t)
 rv_obs = 5.0 * np.sin(2 * np.pi * t / 10.0) + np.sqrt(
     0.05**2 + rv_err**2
 ) * random.normal(size=len(t))
 
 with pm.Model():
-
     # Period, semi-amplitude, and eccentricity
     log_period = pm.Normal("log_period", mu=np.log(10.0), sigma=1.0)
-    period = pm.Deterministic("period", tt.exp(log_period))
-    log_semiamp = pm.Normal("log_semiamp", mu=np.log(5.0), sd=2.0)
-    semiamp = pm.Deterministic("semiamp", tt.exp(log_semiamp))
-    ecc = pm.Uniform("ecc", lower=0, upper=1)
+    period = pm.Deterministic("period", pt.exp(log_period))
+    log_semiamp = pm.Normal("log_semiamp", mu=np.log(5.0), sigma=2.0)
+    semiamp = pm.Deterministic("semiamp", pt.exp(log_semiamp))
+    ecc = pm.Uniform("ecc", lower=0, upper=0.5, initval=0.01)
 
     # At low eccentricity, omega and the phase of periastron (phi) are
     # correlated so it can be best to fit in (omega ± phi) / 2
-    plus = pmx.Angle("plus")
-    minus = pmx.Angle("minus")
+    plus = pmx.angle("plus")
+    minus = pmx.angle("minus")
     phi = pm.Deterministic("phi", plus + minus)
     omega = pm.Deterministic("omega", plus - minus)
 
     # For non-zero eccentricity, it can sometimes be better to use
     # sqrt(e)*sin(omega) and sqrt(e)*cos(omega) as your parameters:
     #
-    #     ecs = pmx.UnitDisk("ecs", testval=0.01 * np.ones(2))
-    #     ecc = pm.Deterministic("ecc", tt.sum(ecs ** 2, axis=0))
-    #     omega = pm.Deterministic("omega", tt.arctan2(ecs[1], ecs[0]))
-    #     phi = pmx.Angle("phi")
+    #     h, k = xo.unit_disk("h", "k")
+    #     ecc = pm.Deterministic("ecc", h**2 + k**2)
+    #     omega = pm.Deterministic("omega", pt.arctan2(h, k))
+    #     phi = xo.angle("phi")
 
     # Jitter & the system mean velocity offset
-    log_jitter = pm.Normal("log_jitter", mu=np.log(0.05), sd=5.0)
-    zero_point = pm.Normal("zero_point", mu=0, sd=10.0)
+    log_jitter = pm.Normal("log_jitter", mu=np.log(0.05), sigma=5.0)
+    zero_point = pm.Normal("zero_point", mu=0, sigma=10.0)
 
     # Then we define the orbit
     tperi = pm.Deterministic("tperi", period * phi / (2 * np.pi))
     orbit = xo.orbits.KeplerianOrbit(
         period=period, t_periastron=tperi, ecc=ecc, omega=omega
     )
 
     # And define the RV model
     rv_model = zero_point + orbit.get_radial_velocity(t, K=semiamp)
 
     # Finally add in the observation model
-    err = tt.sqrt(rv_err**2 + tt.exp(2 * log_jitter))
+    err = pt.sqrt(rv_err**2 + pt.exp(2 * log_jitter))
     pm.Normal("obs", mu=rv_model, sigma=rv_err, observed=rv_obs)
 
     # We'll also track the model just for plotting purposes
     pm.Deterministic(
-        "rv_plot", zero_point + orbit.get_radial_velocity(t_plot, K=semiamp)
+        "__rv_plot", zero_point + orbit.get_radial_velocity(t_plot, K=semiamp)
     )
 
-    soln = pmx.optimize(vars=[plus, minus, ecc])
+    soln = pmx.optimize(vars=[plus, minus])
     soln = pmx.optimize(soln)
-    trace = pmx.sample(
+    trace = pm.sample(
         tune=1000,
         draws=1000,
         cores=2,
         chains=2,
-        start=soln,
-        return_inferencedata=True,
+        initvals=soln,
+        target_accept=0.9,
+        init="adapt_full",
     )
 
 # Plot the results
-rv_plot = trace.posterior["rv_plot"].values
+rv_plot = trace.posterior["__rv_plot"].values
 q16, q50, q84 = np.percentile(rv_plot, [16, 50, 84], axis=(0, 1))
 plt.errorbar(t, rv_obs, yerr=rv_err, fmt="+k", label="data")
 plt.plot(t_plot, q50)
 plt.fill_between(t_plot, q16, q84, alpha=0.3, label="posterior")
 plt.xlim(0, 50)
 plt.legend(fontsize=12, loc=2)
 plt.xlabel("time [days]")
 plt.ylabel("radial velocity [m/s]")
 
-az.summary(trace, var_names=["^(?!rv_plot).*"], filter_vars="regex")
+az.summary(trace, var_names=["^(?!__).*"], filter_vars="regex")
 ```
 
 Instead of using `semiamp` as a parameter, we could have passed `m_planet` and `incl` as parameters to `KeplerianOrbit` and fit the physical orbit.
 Similarly, if we we doing a joint fit with a transit light curve (see {ref}`data-and-models/combining` below) we could have parameterized in terms of `t0` (the time of a reference transit) instead of the phase of periastron.
 
 As mentioned in the comments above and discussed in {ref}`reparameterization`, the performance of these fits can be problem specific and depend on the choice of parameters.
 Therefore it is often worthwhile experimenting with different parameterizations, but this can be a good place to start for radial velocity-only fits.
@@ -329,33 +329,32 @@
 random = np.random.default_rng(5678)
 t_plot = np.linspace(0, 22 * 365.25, 500)
 t = np.sort(random.uniform(0.0, 22 * 365.25, 45))
 rho_err = random.uniform(0.05, 0.1, len(t))
 theta_err = random.uniform(0.05, 0.1, len(t))
 
 with pm.Model():
-
     # Period, semi-major axis, eccentricity, and t0
     log_period = pm.Normal("log_period", mu=np.log(25.0 * 365.25), sigma=1.0)
-    period = pm.Deterministic("period", tt.exp(log_period))
-    log_a = pm.Normal("log_a", mu=np.log(0.3), sd=2.0)
-    a = pm.Deterministic("a", tt.exp(log_a))
+    period = pm.Deterministic("period", pt.exp(log_period))
+    log_a = pm.Normal("log_a", mu=np.log(0.3), sigma=2.0)
+    a = pm.Deterministic("a", pt.exp(log_a))
     ecc = pm.Uniform("ecc", lower=0, upper=1)
     tperi = pm.Normal("tperi", mu=3500.0, sigma=1000.0)
 
     # For astrometric orbits, a good choice of parameterization can be
     # (Omega ± omega) / 2
-    plus = pmx.Angle("plus")
-    minus = pmx.Angle("minus")
+    plus = pmx.angle("plus")
+    minus = pmx.angle("minus")
     Omega = pm.Deterministic("Omega", plus + minus)
     omega = pm.Deterministic("omega", plus - minus)
 
     # We'll use a uniform prior on cos(incl)
-    cos_incl = pm.Uniform("cos_incl", lower=-1.0, upper=1.0, testval=0.3)
-    incl = pm.Deterministic("incl", tt.arccos(cos_incl))
+    cos_incl = pm.Uniform("cos_incl", lower=-1.0, upper=1.0, initval=0.3)
+    incl = pm.Deterministic("incl", pt.arccos(cos_incl))
 
     # Then we define the orbit
     orbit = xo.orbits.KeplerianOrbit(
         a=a,
         t_periastron=tperi,
         period=period,
         incl=incl,
@@ -373,109 +372,113 @@
     # ================================================== #
     rho_obs, theta_obs = pmx.eval_in_model([rho_model, theta_model])
     rho_obs += rho_err * random.normal(size=len(t))
     theta_obs += theta_err * random.normal(size=len(t))
     # =============== end simulated data =============== #
 
     # Define the observation model this is simple for rho:
-    pm.Normal("rho_obs", mu=rho_model, sd=rho_err, observed=rho_obs)
+    pm.Normal("rho_obs", mu=rho_model, sigma=rho_err, observed=rho_obs)
 
     # But we want to be cognizant of the fact that theta wraps so the following
     # is equivalent to
     #
-    #   pm.Normal("obs_theta", mu=theta_model, observed=theta_obs, sd=theta_err)
+    #   pm.Normal("obs_theta", mu=theta_model, observed=theta_obs, sigma=theta_err)
     #
     # but takes into account the wrapping
-    theta_diff = tt.arctan2(
-        tt.sin(theta_model - theta_obs), tt.cos(theta_model - theta_obs)
+    theta_diff = pt.arctan2(
+        pt.sin(theta_model - theta_obs), pt.cos(theta_model - theta_obs)
+    )
+    pm.Normal(
+        "theta_obs",
+        mu=theta_diff,
+        sigma=theta_err,
+        observed=np.zeros_like(theta_obs),
     )
-    pm.Normal("theta_obs", mu=theta_diff, sd=theta_err, observed=0.0)
 
     # We'll also track the model just for plotting purposes
     rho_plot, theta_plot = orbit.get_relative_angles(t_plot)
-    pm.Deterministic("rho_plot", rho_plot)
-    pm.Deterministic("theta_plot", theta_plot)
+    pm.Deterministic("__rho_plot", rho_plot)
+    pm.Deterministic("__theta_plot", theta_plot)
 
-    trace = pmx.sample(
+    trace = pm.sample(
         tune=1000,
         draws=1000,
         cores=2,
         chains=2,
         target_accept=0.95,
-        return_inferencedata=True,
+        init="adapt_full",
     )
 
 # Plot the results
 fig, (ax1, ax2) = plt.subplots(2, 1, figsize=(8, 8), sharex=True)
 
 q16, q50, q84 = np.percentile(
-    trace.posterior["rho_plot"].values, [16, 50, 84], axis=(0, 1)
+    trace.posterior["__rho_plot"].values, [16, 50, 84], axis=(0, 1)
 )
 ax1.errorbar(t, rho_obs, yerr=rho_err, fmt="+k", label="data")
 ax1.plot(t_plot, q50)
 ax1.fill_between(t_plot, q16, q84, alpha=0.3, label="posterior")
 ax1.set_ylabel(r"$\rho$ [arcsec]")
 
 q16, q50, q84 = np.percentile(
-    trace.posterior["theta_plot"].values, [16, 50, 84], axis=(0, 1)
+    trace.posterior["__theta_plot"].values, [16, 50, 84], axis=(0, 1)
 )
 ax2.errorbar(t, theta_obs, yerr=rho_err, fmt="+k", label="data")
 ax2.plot(t_plot, q50)
 ax2.fill_between(t_plot, q16, q84, alpha=0.3, label="posterior")
 ax2.set_xlim(t_plot.min(), t_plot.max())
 ax2.legend(fontsize=12, loc=2)
 ax2.set_ylabel(r"$\theta$ [radians]")
 ax2.set_xlabel("time [days]")
 
 # Compute the convergence stats
-az.summary(trace, var_names=["^(?!.*_plot).*"], filter_vars="regex")
+az.summary(trace, var_names=["^(?!__).*"], filter_vars="regex")
 ```
 
 In this example, the units of `a` are arcseconds, but the {func}`exoplanet.orbits.KeplerianOrbit.get_relative_angles` function accepts a parallax argument if you have a constraint on the parallax of the system.
 If you provide parallax as an argument, `a` should be provided in the usual units of Solar radii.
 
 +++
 
 (data-and-models/transits)=
 
 ## Transits, occultations, and eclipses
 
 `exoplanet` has built in support for evaluating quadratically limb darkened light curve models using the algorithm from [Agol et al. (2020)](https://arxiv.org/abs/1908.03222).
-If you need flexible surface models or higher order limb darkening, check out the [`starry` package](https://starry.readthedocs.io) which also integrates with `PyMC3`.
+If you need flexible surface models or higher order limb darkening, check out the [`starry` package](https://starry.readthedocs.io) which also integrates with `PyMC` (3, but not 5 at the time of writing this).
 
 Transit and occultation modeling is one of the primary applications of `exoplanet` so there are quite a few options (including transit timing variations, detached eclipsing binary modeling, and much more) that are highlighted on the [Case Studies](https://gallery.exoplanet.codes) page.
 But, a bread-and-butter transit model implemented in `exoplanet` might look something like the following:
 
 ```{code-cell}
 random = np.random.default_rng(123)
 num_transits = 4
 t = np.arange(0, 35, 0.02)
 yerr = 5e-4
 
 with pm.Model():
-
     # The baseline flux
     mean = pm.Normal("mean", mu=0.0, sigma=1.0)
 
     # Often the best parameterization is actually in terms of the
     # times of two reference transits rather than t0 and period
     t0 = pm.Normal("t0", mu=4.35, sigma=1.0)
     t1 = pm.Normal("t1", mu=33.2, sigma=1.0)
     period = pm.Deterministic("period", (t1 - t0) / num_transits)
 
     # The Kipping (2013) parameterization for quadratic limb darkening
     # paramters
-    u = xo.distributions.QuadLimbDark("u", testval=np.array([0.3, 0.2]))
+    u = xo.distributions.quad_limb_dark("u", initval=np.array([0.3, 0.2]))
 
     # The radius ratio and impact parameter; these parameters can
     # introduce pretty serious covariances and are ripe for
     # reparameterization
     log_r = pm.Normal("log_r", mu=np.log(0.04), sigma=2.0)
-    r = pm.Deterministic("r", tt.exp(log_r))
-    b = xo.distributions.ImpactParameter("b", ror=r, testval=0.35)
+    r = pm.Deterministic("r", pt.exp(log_r))
+    b = xo.distributions.impact_parameter("b", r, initval=0.35)
 
     # Set up a Keplerian orbit for the planets
     orbit = xo.orbits.KeplerianOrbit(period=period, t0=t0, b=b)
 
     # Compute the model light curve; note that we index using `[:, 0]`
     # since `get_light_curve` returns an object with the shape
     # `(n_times, n_planets)`
@@ -484,68 +487,64 @@
             orbit=orbit, r=r, t=t
         )[:, 0]
         + mean
     )
 
     # Here we track the value of the model light curve for plotting
     # purposes
-    pm.Deterministic("light_curve", light_curve)
+    pm.Deterministic("__light_curve", light_curve)
 
     # ================================================== #
     # Simulate data from the model for testing           #
     # You should remove the following lines in your code #
     # ================================================== #
     y = pmx.eval_in_model(light_curve)
     y += yerr * random.normal(size=len(y))
     # =============== end simulated data =============== #
 
     # The likelihood function assuming known Gaussian uncertainty
-    pm.Normal("obs", mu=light_curve, sd=yerr, observed=y)
+    pm.Normal("obs", mu=light_curve, sigma=yerr, observed=y)
 
-    trace = pmx.sample(
-        tune=1000,
-        draws=1000,
-        cores=2,
-        chains=2,
-        return_inferencedata=True,
+    trace = pm.sample(
+        tune=1000, draws=1000, cores=2, chains=2, init="adapt_full"
     )
 
 # Plot the results
 q16, q50, q84 = np.percentile(
-    trace.posterior["light_curve"].values, [16, 50, 84], axis=(0, 1)
+    trace.posterior["__light_curve"].values, [16, 50, 84], axis=(0, 1)
 )
 plt.plot(t, y, ".k", ms=2, label="data")
 plt.plot(t, q50)
 plt.fill_between(t, q16, q84, alpha=0.3, label="posterior")
 plt.xlim(0.0, 35)
 plt.legend(fontsize=12, loc=3)
 plt.xlabel("time [days]")
 plt.ylabel("relative flux")
 
 # Compute the convergence stats
-az.summary(trace, var_names=["^(?!light_curve).*"], filter_vars="regex")
+az.summary(trace, var_names=["^(?!__).*"], filter_vars="regex")
 ```
 
 (data-and-models/combining)=
 
 ## Combining datasets
 
-Since `exoplanet` is built on top of `PyMC3`, it has the capacity to support essentially arbitrariliy complicated models.
+Since `exoplanet` is built on top of `PyMC`, it has the capacity to support essentially arbitrarily complicated models.
 This means that you can share parameters or fit multiple datasets however you want.
 We won't go into too many details about this here, but you can see some examples on the [Case Studies](https://gallery.exoplanet.codes) of joint transit/radial velocity fits, or inferences based on datasets from multiple instruments.
 
 The basic idea behind how to simultaneously fit multiple datasets is that you'll need to define the relationship between the datasets (perhaps share parameters or a shared `KeplerianOrbit`) and then you'll include the likelihood for each dataset in your model.
 In all of the above examples, we had a line like
 
 ```python
 pm.Normal("obs", mu=rv_model, sigma=rv_err, observed=rv_obs)
 ```
 
 in all of our models.
 This defines a Gaussian likelihood conditioned on the `observed` data.
-To combine datasets, you can simply add multiple lines like this (one for each dataset) and, behind the scenes, `PyMC3` will multiply these likelihoods (or actually add their logarithms) as it should.
+To combine datasets, you can simply add multiple lines like this (one for each dataset) and, behind the scenes, `PyMC` will multiply these likelihoods (or actually add their logarithms) as it should.
 
 For more concrete examples, check out the [Case Studies](https://gallery.exoplanet.codes) and (if that's not sufficient) feel free to start [a "discussion" on the GitHub repository](https://github.com/exoplanet-dev/exoplanet/discussions) asking for help.
 
 ```{code-cell}
 
 ```
```

### Comparing `exoplanet-0.5.3rc1/docs/tutorials/intro-to-pymc3.md` & `exoplanet-0.6.0rc2/docs/tutorials/intro-to-pymc.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 ---
 jupytext:
   encoding: '# -*- coding: utf-8 -*-'
   text_representation:
     extension: .md
     format_name: myst
     format_version: 0.13
-    jupytext_version: 1.14.1
+    jupytext_version: 1.15.2
 kernelspec:
-  display_name: Python 3
+  display_name: Python 3 (ipykernel)
   language: python
   name: python3
 ---
 
-(intro-to-pymc3)=
+(intro-to-pymc)=
 
-# A quick intro to PyMC3
+# A quick intro to PyMC
 
 ```{code-cell}
 import exoplanet
 
 exoplanet.utils.docs_setup()
 print(f"exoplanet.__version__ = '{exoplanet.__version__}'")
 ```
 
 Gradient-based inference methods (like [Hamiltonian Monte Carlo (HMC)](https://en.wikipedia.org/wiki/Hamiltonian_Monte_Carlo)) haven't been widely used in astrophysics, but they are the standard methods for probabilistic inference using Markov chain Monte Carlo (MCMC) in many other fields.
-*exoplanet* is designed to provide the building blocks for fitting many exoplanet datasets using this technology, and this tutorial presents some of the basic features of the [PyMC3](https://docs.pymc.io/) modeling language and inference engine.
-The [documentation for PyMC3](https://docs.pymc.io/) includes many other tutorials that you should check out to get more familiar with the features that are available.
+_exoplanet_ is designed to provide the building blocks for fitting many exoplanet datasets using this technology, and this tutorial presents some of the basic features of the [PyMC](https://docs.pymc.io/) modeling language and inference engine.
+The [documentation for PyMC](https://docs.pymc.io/) includes many other tutorials that you should check out to get more familiar with the features that are available.
 
-In this tutorial, we will go through two simple examples of fitting some data using PyMC3.
+In this tutorial, we will go through two simple examples of fitting some data using PyMC.
 The first is the classic fitting a line to data with unknown error bars, and the second is a more relevant example where we fit a radial velocity model to the public radial velocity observations of [51 Peg](https://en.wikipedia.org/wiki/51_Pegasi).
 You can read more about fitting lines to data [in the bible of line fitting](https://arxiv.org/abs/1008.4686) and you can see another example of fitting the 51 Peg data using HMC (this time using [Stan](http://mc-stan.org)) [here](https://dfm.io/posts/stan-c++/).
 
 ## Hello world (AKA fitting a line to data)
 
 My standard intro to a new modeling language or inference framework is to fit a line to data.
-So. Let's do that with PyMC3.
+So. Let's do that with PyMC.
 
 To start, we'll generate some fake data using a linear model.
 Feel free to change the random number seed to try out a different dataset.
 
 ```{code-cell}
 import numpy as np
 import matplotlib.pyplot as plt
@@ -93,64 +93,61 @@
 m &\sim& \mathrm{Uniform}(-5,\,5) \\
 b &\sim& \mathrm{Uniform}(-5,\,5) \\
 \log(\sigma) &\sim& \mathrm{Uniform}(-5,\,5) \\
 y_n &\sim& \mathrm{Normal}(m\,x_n+b,\,\sigma)
 \end{eqnarray}
 $$
 
-This is the way that a model like this is often defined in statistics and it will be useful when we implement out model in PyMC3 so take a moment to make sure that you understand the notation.
+This is the way that a model like this is often defined in statistics and it will be useful when we implement out model in PyMC so take a moment to make sure that you understand the notation.
 
-Now, let's implement this model in PyMC3.
-The documentation for the distributions available in PyMC3's modeling language can be [found here](https://docs.pymc.io/api/distributions/continuous.html) and these will come in handy as you go on to write your own models.
+Now, let's implement this model in PyMC.
+The documentation for the distributions available in PyMC's modeling language can be [found here](https://www.pymc.io/projects/docs/en/stable/api/distributions.html) and these will come in handy as you go on to write your own models.
 
 ```{code-cell}
-import pymc3 as pm
+import pymc as pm
 
 with pm.Model() as model:
-
     # Define the priors on each parameter:
     m = pm.Uniform("m", lower=-5, upper=5)
     b = pm.Uniform("b", lower=-5, upper=5)
     logs = pm.Uniform("logs", lower=-5, upper=5)
 
     # Define the likelihood. A few comments:
     #  1. For mathematical operations like "exp", you can't use
     #     numpy. Instead, use the mathematical operations defined
     #     in "pm.math".
     #  2. To condition on data, you use the "observed" keyword
     #     argument to any distribution. In this case, we want to
     #     use the "Normal" distribution (look up the docs for
     #     this).
-    pm.Normal("obs", mu=m * x + b, sd=pm.math.exp(logs), observed=y)
+    pm.Normal("obs", mu=m * x + b, sigma=pm.math.exp(logs), observed=y)
 
     # This is how you will sample the model. Take a look at the
     # docs to see that other parameters that are available.
-    trace = pm.sample(
-        draws=1000, tune=1000, chains=2, cores=2, return_inferencedata=True
-    )
+    trace = pm.sample(draws=1000, tune=1000, chains=2, cores=2)
 ```
 
 Now since we now have samples, let's make some diagnostic plots.
-The first plot to look at is the "traceplot" implemented in PyMC3.
+The first plot to look at is the "traceplot" implemented in PyMC.
 In this plot, you'll see the marginalized distribution for each parameter on the left and the trace plot (parameter value as a function of step number) on the right.
-In each panel, you should see two lines with different colors.
+In each panel, you should see two lines with different colors or linestyles.
 These are the results of different independent chains and if the results are substantially different in the different chains then there is probably something going wrong.
 
 ```{code-cell}
 import arviz as az
 
 _ = az.plot_trace(trace, var_names=["m", "b", "logs"])
 ```
 
 It's also good to quantify that "looking substantially different" argument.
-This is implemented in PyMC3 as the "summary" function.
-In this table, some of the key columns to look at are `n_eff` and `Rhat`.
+This is implemented in PyMC as the "summary" function.
+In this table, some of the key columns to look at are the columns starting with `ess_` and `Rhat`.
 
-1. `n_eff` shows an estimate of the number of effective (or independent) samples for that parameter. In this case, `n_eff` should probably be around 500 per chain (there should have been 2 chains run).
-2. `Rhat` shows the [Gelman–Rubin statistic](https://docs.pymc.io/api/diagnostics.html#pymc3.diagnostics.gelman_rubin) and it should be close to 1.
+1. The `ess_*` columns show an estimate of the number of effective (or independent) samples for that parameter. In this case, the `ess` should probably be around 500 per chain (there should have been 2 chains run).
+2. `Rhat` shows the Gelman–Rubin statistic, and it should be close to 1.
 
 ```{code-cell}
 az.summary(trace, var_names=["m", "b", "logs"])
 ```
 
 The last diagnostic plot that we'll make here is the [corner plot made using corner.py](https://corner.readthedocs.io).
 
@@ -159,36 +156,36 @@
 
 _ = corner.corner(
     trace,
     truths=dict(m=true_m, b=true_b, logs=true_logs),
 )
 ```
 
-**Extra credit:** Here are a few suggestions for things to try out while getting more familiar with PyMC3:
+**Extra credit:** Here are a few suggestions for things to try out while getting more familiar with PyMC:
 
-1. Try initializing the parameters using the `testval` argument to the distributions. Does this improve performance in this case? It will substantially improve performance in more complicated examples.
+1. Try initializing the parameters using the `initval` argument to the distributions. Does this improve performance in this case? It will substantially improve performance in more complicated examples.
 2. Try changing the priors on the parameters. For example, try the "uninformative" prior [recommended by Jake VanderPlas on his blog](http://jakevdp.github.io/blog/2014/06/14/frequentism-and-bayesianism-4-bayesian-in-python/#Prior-on-Slope-and-Intercept).
 3. What happens as you substantially increase or decrease the simulated noise? Does the performance change significantly? Why?
 
 ## A more realistic example: radial velocity exoplanets
 
-While the above example was cute, it doesn't really fully exploit the power of PyMC3 and it doesn't really show some of the real issues that you will face when you use PyMC3 as an astronomer.
-To get a better sense of how you might use PyMC3 in Real Life™, let's take a look at a more realistic example: fitting a Keplerian orbit to radial velocity observations.
+While the above example was cute, it doesn't really fully exploit the power of PyMC and it doesn't really show some of the real issues that you will face when you use PyMC as an astronomer.
+To get a better sense of how you might use PyMC in Real Life™, let's take a look at a more realistic example: fitting a Keplerian orbit to radial velocity observations.
 
-One of the key aspects of this problem that I want to highlight is the fact that PyMC3 (and the underlying model building framework [Theano (recently renamed to Aesara)](https://aesara.readthedocs.io/)) don't have out-of-the-box support for the root-finding that is required to solve Kepler's equation.
+One of the key aspects of this problem that I want to highlight is the fact that PyMC (and the underlying model-building framework [PyTensor](https://pytensor.readthedocs.io/)) don't have out-of-the-box support for the root-finding that is required to solve Kepler's equation.
 As part of the process of computing a Keplerian RV model, we must solve the equation:
 
 $$
 M = E - e\,\sin E
 $$
 
 for the eccentric anomaly $E$ given some mean anomaly $M$ and eccentricity $e$.
-There are commonly accepted methods of solving this equation using [Newton's method](https://en.wikipedia.org/wiki/Newton%27s_method), but if we want to expose that to PyMC3, we have to define a [custom Theano operation](https://aesara.readthedocs.io/en/latest/extending/index.html) with a custom gradient.
+There are commonly accepted methods of solving this equation using [Newton's method](https://en.wikipedia.org/wiki/Newton%27s_method), but if we want to expose that to PyMC, we have to define a [custom Pytensor operation](https://pytensor.readthedocs.io/en/latest/extending/index.html) with a custom gradient.
 I won't go into the details of the math (because [I blogged about it](https://dfm.io/posts/stan-c++/)) and I won't go into the details of the implementation.
-So, for this tutorial, we'll use the custom Kepler solver that is implemented as part of *exoplanet* and fit the publicly available radial velocity observations of the famous exoplanetary system 51 Peg using PyMC3.
+So, for this tutorial, we'll use the custom Kepler solver that is implemented as part of _exoplanet_ and fit the publicly available radial velocity observations of the famous exoplanetary system 51 Peg using PyMC.
 
 First, we need to download the data from the exoplanet archive:
 
 ```{code-cell}
 import requests
 import pandas as pd
 import matplotlib.pyplot as plt
@@ -227,101 +224,98 @@
     va="bottom",
     fontsize=12,
 )
 plt.ylabel("radial velocity [m/s]")
 _ = plt.xlabel("phase")
 ```
 
-Now, here's the implementation of a radial velocity model in PyMC3.
+Now, here's the implementation of a radial velocity model in PyMC.
 Some of this will look familiar after the Hello World example, but things are a bit more complicated now.
 Take a minute to take a look through this and see if you can follow it.
 There's a lot going on, so I want to point out a few things to pay attention to:
 
-1. All of the mathematical operations (for example `exp` and `sqrt`) are being performed using Theano/Aesara (see {ref}`theano`) instead of NumPy.
+1. All of the mathematical operations (for example `exp` and `sqrt`) are being performed using [PyTensor](https://pytensor.readthedocs.io) instead of NumPy.
 2. All of the parameters have initial guesses provided. This is an example where this makes a big difference because some of the parameters (like period) are very tightly constrained.
 3. Some of the lines are wrapped in `Deterministic` distributions. This can be useful because it allows us to track values as the chain progresses even if they're not parameters. For example, after sampling, we will have a sample for `bkg` (the background RV trend) for each step in the chain. This can be especially useful for making plots of the results.
 4. Similarly, at the end of the model definition, we compute the RV curve for a single orbit on a fine grid. This can be very useful for diagnosing fits gone wrong.
-5. For parameters that specify angles (like $\omega$, called `w` in the model below), it can be inefficient to sample in the angle directly because of the fact that the value wraps around at $2\pi$. Instead, it can be better to sample the unit vector specified by the angle or as a parameter in a unit disk, when combined with eccentricity. In practice, this can be achieved by sampling a 2-vector from an isotropic Gaussian and normalizing the components by the norm. These are implemented in the [pymc3-ext](https://github.com/exoplanet-dev/pymc3-ext) package.
+5. For parameters that specify angles (like $\omega$, called `w` in the model below), it can be inefficient to sample in the angle directly because of the fact that the value wraps around at $2\pi$. Instead, it can be better to sample the unit vector specified by the angle or as a parameter in a unit disk, when combined with eccentricity. There are some helper functions like {func}`exoplanet.distributions.angle` and {func}`exoplanet.distributions.unit_disk` to help with this.
 
 ```{code-cell}
-import pymc3_ext as pmx
-import aesara_theano_fallback.tensor as tt
-
+import pytensor.tensor as pt
 import exoplanet as xo
 
 with pm.Model() as model:
-
     # Parameters
     logK = pm.Uniform(
         "logK",
         lower=0,
         upper=np.log(200),
-        testval=np.log(0.5 * (np.max(rv) - np.min(rv))),
+        initval=np.log(0.5 * (np.max(rv) - np.min(rv))),
     )
     logP = pm.Uniform(
-        "logP", lower=0, upper=np.log(10), testval=np.log(lit_period)
+        "logP", lower=0, upper=np.log(10), initval=np.log(lit_period)
     )
-    phi = pm.Uniform("phi", lower=0, upper=2 * np.pi, testval=0.1)
+    phi = pm.Uniform("phi", lower=0, upper=2 * np.pi, initval=0.1)
 
     # Parameterize the eccentricity using:
     #  h = sqrt(e) * sin(w)
     #  k = sqrt(e) * cos(w)
-    hk = pmx.UnitDisk("hk", testval=np.array([0.01, 0.01]))
-    e = pm.Deterministic("e", hk[0] ** 2 + hk[1] ** 2)
-    w = pm.Deterministic("w", tt.arctan2(hk[1], hk[0]))
+    h, k = xo.unit_disk("h", "k", initval=np.array([0.01, 0.01]))
+    e = pm.Deterministic("e", h**2 + k**2)
+    w = pm.Deterministic("w", pt.arctan2(k, h))
 
-    rv0 = pm.Normal("rv0", mu=0.0, sd=10.0, testval=0.0)
-    rvtrend = pm.Normal("rvtrend", mu=0.0, sd=10.0, testval=0.0)
+    rv0 = pm.Normal("rv0", mu=0.0, sigma=10.0, initval=0.0)
+    rvtrend = pm.Normal("rvtrend", mu=0.0, sigma=10.0, initval=0.0)
 
     # Deterministic transformations
-    n = 2 * np.pi * tt.exp(-logP)
-    P = pm.Deterministic("P", tt.exp(logP))
-    K = pm.Deterministic("K", tt.exp(logK))
-    cosw = tt.cos(w)
-    sinw = tt.sin(w)
+    n = 2 * np.pi * pt.exp(-logP)
+    P = pm.Deterministic("P", pt.exp(logP))
+    K = pm.Deterministic("K", pt.exp(logK))
+    cosw = pt.cos(w)
+    sinw = pt.sin(w)
     t0 = (phi + w) / n
 
     # The RV model
     bkg = pm.Deterministic("bkg", rv0 + rvtrend * t / 365.25)
     M = n * t - (phi + w)
 
     # This is the line that uses the custom Kepler solver
-    f = xo.orbits.get_true_anomaly(M, e + tt.zeros_like(M))
+    f = xo.orbits.get_true_anomaly(M, e + pt.zeros_like(M))
     rvmodel = pm.Deterministic(
-        "rvmodel", bkg + K * (cosw * (tt.cos(f) + e) - sinw * tt.sin(f))
+        "rvmodel", bkg + K * (cosw * (pt.cos(f) + e) - sinw * pt.sin(f))
     )
 
     # Condition on the observations
-    pm.Normal("obs", mu=rvmodel, sd=rv_err, observed=rv)
+    pm.Normal("obs", mu=rvmodel, sigma=rv_err, observed=rv)
 
     # Compute the phased RV signal
     phase = np.linspace(0, 1, 500)
     M_pred = 2 * np.pi * phase - (phi + w)
-    f_pred = xo.orbits.get_true_anomaly(M_pred, e + tt.zeros_like(M_pred))
+    f_pred = xo.orbits.get_true_anomaly(M_pred, e + pt.zeros_like(M_pred))
     rvphase = pm.Deterministic(
-        "rvphase", K * (cosw * (tt.cos(f_pred) + e) - sinw * tt.sin(f_pred))
+        "rvphase", K * (cosw * (pt.cos(f_pred) + e) - sinw * pt.sin(f_pred))
     )
 ```
 
 In this case, I've found that it is useful to first optimize the parameters to find the "maximum a posteriori" (MAP) parameters and then start the sampler from there.
-This is useful here because MCMC is not designed to *find* the maximum of the posterior; it's just meant to sample the shape of the posterior.
-The performance of all MCMC methods can be really bad when the initialization isn't good (especially when some parameters are very well constrained).
-To find the maximum a posteriori parameters using PyMC3, you can use the `optimize` function from [pymc3-ext](https://github.com/exoplanet-dev/pymc3-ext):
+This is useful here because MCMC is not designed to _find_ the maximum of the posterior; it's just meant to sample the shape of the posterior.
+The performance of all MCMC methods can be really bad when the initialization isn't good (especially when some parameters are very well-constrained).
+To find the maximum a posteriori parameters using PyMC, you can use the [`find_MAP` function](https://www.pymc.io/projects/docs/en/stable/api/generated/pymc.find_MAP.html):
 
 ```{code-cell}
 with model:
-    map_params = pmx.optimize()
+    map_params = pm.find_MAP()
 ```
 
 Let's make a plot to check that this initialization looks reasonable.
 In the top plot, we're looking at the RV observations as a function of time with the initial guess for the long-term trend overplotted in blue.
 In the lower panel, we plot the "folded" curve where we have wrapped the observations onto the best-fit period and the prediction for a single overplotted in orange.
 If this doesn't look good, try adjusting the initial guesses for the parameters and see if you can get a better fit.
 
-**Exercise:** Try changing the initial guesses for the parameters (as specified by the `testval` argument) and see how sensitive the results are to these values. Are there some parameters that are less important? Why is this?
+**Exercise:** Try changing the initial guesses for the parameters (as specified by the `initval` argument) and see how sensitive the results are to these values. Are there some parameters that are less important? Why is this?
 
 ```{code-cell}
 fig, axes = plt.subplots(2, 1, figsize=(8, 8))
 
 period = map_params["P"]
 
 ax = axes[0]
@@ -337,26 +331,26 @@
 ax.set_ylim(-110, 110)
 ax.set_ylabel("radial velocity [m/s]")
 ax.set_xlabel("phase [days]")
 
 plt.tight_layout()
 ```
 
-Now let's sample the posterior starting from our MAP estimate (here we're using the sampling routine from [pymc3-ext](https://github.com/exoplanet-dev/pymc3-ext) which wraps the PyMC3 function with some better defaults).
+Now let's sample the posterior starting from our MAP estimate:
 
 ```{code-cell}
 with model:
-    trace = pmx.sample(
+    trace = pm.sample(
         draws=1000,
         tune=1000,
-        start=map_params,
+        initvals=map_params,
         chains=2,
         cores=2,
         target_accept=0.95,
-        return_inferencedata=True,
+        init="adapt_full",
     )
 ```
 
 As above, it's always a good idea to take a look at the summary statistics for the chain.
 If everything went as planned, there should be more than 1000 effective samples per chain and the Rhat values should be close to 1.
 (Not too bad for about 30 seconds of run time!)
 
@@ -403,7 +397,11 @@
     axes[1].plot(phase * period, rvphase[i], color="C1", lw=1, alpha=0.3)
 
 axes[0].set_ylim(-110, 110)
 axes[1].set_ylim(-110, 110)
 
 plt.tight_layout()
 ```
+
+```{code-cell}
+
+```
```

### Comparing `exoplanet-0.5.3rc1/docs/tutorials/light-delay.md` & `exoplanet-0.6.0rc2/docs/tutorials/light-delay.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ---
 jupytext:
   text_representation:
     extension: .md
     format_name: myst
     format_version: 0.13
-    jupytext_version: 1.14.1
+    jupytext_version: 1.15.2
 kernelspec:
-  display_name: Python 3
+  display_name: Python 3 (ipykernel)
   language: python
   name: python3
 ---
 
 # Light travel time delay
 
 ```{code-cell}
@@ -128,7 +128,11 @@
 plt.xlabel("time [days]")
 plt.ylabel("relative flux")
 plt.legend(fontsize=10, loc="lower right")
 _ = plt.title(
     "Light delay causes transits to occur 8.32 minutes early", fontsize=14
 )
 ```
+
+```{code-cell}
+
+```
```

### Comparing `exoplanet-0.5.3rc1/docs/tutorials/reparameterization.md` & `exoplanet-0.6.0rc2/docs/tutorials/reparameterization.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 ---
 jupytext:
   text_representation:
     extension: .md
     format_name: myst
     format_version: 0.13
-    jupytext_version: 1.14.1
+    jupytext_version: 1.15.2
 kernelspec:
-  display_name: Python 3
+  display_name: Python 3 (ipykernel)
   language: python
   name: python3
 ---
 
 (reparameterization)=
 
 # Reparameterization
 
 +++
 
-One thing that you'll often find when using `exoplanet` (and `PyMC3` or other libraries for gradient-based inference) is that performance of your inference can be quite sensitive to the parameterization of your problem.
-For example, you might see warnings from `PyMC3` telling you to consider reparameterizing your model (because of divergences) or (worse!) you might find that sampling is unreasonably slow or the number of effective samples is very small.
+One thing that you'll often find when using `exoplanet` (and `PyMC` or other libraries for gradient-based inference) is that performance of your inference can be quite sensitive to the parameterization of your problem.
+For example, you might see warnings from `PyMC` telling you to consider reparameterizing your model (because of divergences) or (worse!) you might find that sampling is unreasonably slow or the number of effective samples is very small.
 These issues can almost always be solved by investigating any sources of non-linear degeneracies between parameters in your model or heavy tails in the posterior density.
 
 [The Stan User's Guide](https://mc-stan.org/docs/2_27/stan-users-guide/reparameterization-section.html) includes some general advice about reparameterization that can be a useful place to start, but I've found that the best choices tend to be pretty problem specific.
 Throughout these tutorials and the [Case Studies](https://gallery.exoplanet.codes) we have tried to select sensible parameterizations (sometimes after many experiments) and comment wherever we've chosen something non-standard.
 
 Some of the trickiest parameters are things like orbital eccentricity, inclination, and other angles.
 In the case of eccentricity, you can sometimes reparameterize in terms of an observable (such as transit duration, see the "Quick fits for TESS light curves" case study).
```

### Comparing `exoplanet-0.5.3rc1/docs/user/api.rst` & `exoplanet-0.6.0rc2/docs/user/api.rst`

 * *Files 6% similar despite different names*

```diff
@@ -40,16 +40,18 @@
 
 Distributions
 -------------
 
 Physical distributions
 ~~~~~~~~~~~~~~~~~~~~~~
 
-.. autoclass:: exoplanet.distributions.QuadLimbDark
-.. autoclass:: exoplanet.distributions.ImpactParameter
+.. autofunction:: exoplanet.distributions.angle
+.. autofunction:: exoplanet.distributions.unit_disk
+.. autofunction:: exoplanet.distributions.quad_limb_dark
+.. autofunction:: exoplanet.distributions.impact_parameter
 
 Eccentricity distributions
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. autofunction:: exoplanet.distributions.eccentricity.kipping13
 .. autofunction:: exoplanet.distributions.eccentricity.vaneylen19
```

### Comparing `exoplanet-0.5.3rc1/docs/user/dev.rst` & `exoplanet-0.6.0rc2/docs/user/dev.rst`

 * *Files 5% similar despite different names*

```diff
@@ -80,19 +80,19 @@
 and try to follow roughly the same format.
 
 2. **Case studies**: These are more in depth tutorials that require more
 computational run time. These can be found in the `case studies
 <https://github.com/exoplanet-dev/case-studies>`_ repo and there is more
 information there about how to contribute.
 
-3. **Theano/Aesara ops**: ``exoplanet`` comes bundled with a set of custom ops
+3. **Theano/PyTensor ops**: ``exoplanet`` comes bundled with a set of custom ops
 that are implemented in the `exoplanet-core project
 <https://github.com/exoplanet-dev/exoplanet-core>`_. As a user, hopefully you'll
-rarely interact with these directly and we haven't put a lot of work into making
-them user friendly, but if you are interested in diving in, feel free to ask
+rarely interact with these directly, and we haven't put a lot of work into making
+them user-friendly, but if you are interested in diving in, feel free to ask
 questions on GitHub or via email.
 
 
 Testing your contribution
 +++++++++++++++++++++++++
 
 If you're contributing a change to the code (either a new feature or bug fix),
```

### Comparing `exoplanet-0.5.3rc1/docs/user/install.rst` & `exoplanet-0.6.0rc2/docs/user/install.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,57 @@
 .. _install:
 
 Installation
 ============
 
-.. note:: ``exoplanet`` requires Python 3.6 and later.
+.. note:: ``exoplanet`` requires Python 3.8 and later.
 
 Using pip
 ---------
 
 The recommended method of installing *exoplanet* is with `pip
 <https://pip.pypa.io>`_:
 
 .. code-block:: bash
 
-    python -m pip install -U exoplanet
+    python -m pip install -U "exoplanet[pymc]"
 
-If you want to install some recommended extras (`pymc3-ext
-<https://github.com/exoplanet-dev/pymc3-ext>`_ and `celerite2
+If you want to install some recommended extras (`pymc-ext
+<https://github.com/exoplanet-dev/pymc-ext>`_ and `celerite2
 <https://celerite2.readthedocs.io>`_), you can use the following, or just follow
 the instructions on the relevant documentation pages:
 
 .. code-block:: bash
 
     python -m pip install -U "exoplanet[extras]"
 
 Both of these installation methods will install the required dependencies:
 
 - `numpy <https://numpy.org>`_
 - `astropy <https://www.astropy.org>`_
-- `pymc3 <https://docs.pymc.io>`_
+- `pymc <https://www.pymc.io>`_
 - `exoplanet-core <https://github.com/exoplanet-dev/exoplanet-core>`_
-- `aesara-theano-fallback <https://github.com/exoplanet-dev/aesara-theano-fallback>`_
 
+Compatibility with PyMC3
+------------------------
+
+Although now updated to work with ``PyMC`` version 5, ``exoplanet`` is still
+backwards compatible with ``PyMC3``. To install the ``PyMC3`` compatible version
+of ``exoplanet``, use the following command:
+
+.. code-block:: bash
+
+    python -m pip install -U "exoplanet[pymc3]"
+
+or first install ``PyMC3`` (however you want) and then ``exoplanet`` without any
+extras:
+
+.. code-block:: bash
+
+    python -m pip install -U exoplanet
 
 Using conda
 -----------
 
 *exoplanet* can also be installed using `conda <https://docs.conda.io>`_ from
 ``conda-forge``:
```

### Comparing `exoplanet-0.5.3rc1/docs/user/multiprocessing.rst` & `exoplanet-0.6.0rc2/docs/user/multiprocessing.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 .. _multiprocessing:
 
 Multiprocessing
 ===============
 
-By default, when you sample with ``PyMC3``, it will try to run chains in
+By default, when you sample with ``PyMC``, it will try to run chains in
 parallel using Python's `multiprocessing` module. This is pretty much always
 what you want, but it can also cause some headaches (mostly on macOS or Windows)
 for the large and computationally expensive models tackled by ``exoplanet``. In
 particular, you might sometimes get hit by the "dreaded broken pipe" error where
 your sampler crashes for no obvious reason or (worse!) you might find you
 sampler hanging indefinitely before it even starts running. The official
-``PyMC3`` solution is to use the ``mp_ctx="forkserver"`` option when calling
+``PyMC`` solution is to use the ``mp_ctx="forkserver"`` option when calling
 ``pm.sample`` on macOS or Windows. Unfortunately, this (for reasons that I don't
 totally understand) will often cause a huge performance hit that can increase
 your runtime by orders of magnitude.
 
 Throughout these documentation pages and for the Case Studies, we have tried to
 design the example models such that you shouldn't run into issues with
 multiprocessing but, if you do, please `open an issue on GitHub
 <https://github.com/exoplanet-dev/exoplanet/issues>`_. For your own projects, if
 you run into multiprocessing issues, you can try adjusting the ``mp_ctx`` and
-``pickle_backend`` parameters (see the `PyMC3 docs
-<https://docs.pymc.io/api/inference.html#pymc3.sampling.sample>`_), or as a last
-resort, set ``cores=1`` to get serial sampling.
+``pickle_backend`` parameters (see the `PyMC docs
+<https://www.pymc.io/projects/docs/en/stable/api/generated/pymc.sample.html>`_),
+or as a last resort, set ``cores=1`` to get serial sampling.
```

### Comparing `exoplanet-0.5.3rc1/joss/figures/figure.png` & `exoplanet-0.6.0rc2/joss/figures/figure.png`

 * *Files identical despite different names*

### Comparing `exoplanet-0.5.3rc1/joss/figures/joss-logo.png` & `exoplanet-0.6.0rc2/joss/figures/joss-logo.png`

 * *Files identical despite different names*

### Comparing `exoplanet-0.5.3rc1/joss/metadata.yaml` & `exoplanet-0.6.0rc2/joss/metadata.yaml`

 * *Files identical despite different names*

### Comparing `exoplanet-0.5.3rc1/joss/paper.bib` & `exoplanet-0.6.0rc2/joss/paper.bib`

 * *Files identical despite different names*

### Comparing `exoplanet-0.5.3rc1/joss/paper.md` & `exoplanet-0.6.0rc2/joss/paper.md`

 * *Files identical despite different names*

### Comparing `exoplanet-0.5.3rc1/pyproject.toml` & `exoplanet-0.6.0rc2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 [tool.isort]
 skip_glob = ["docs/tutorials/*.py"]
 line_length = 79
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
-known_third_party = ["astropy", "corner", "jupytext", "matplotlib", "nbconvert", "nbformat", "numpy", "packaging", "pandas", "pkg_resources", "pymc3", "pytest", "requests", "scipy", "setuptools", "sphinx_typlog_theme", "theano"]
 
 [tool.coverage.run]
 parallel = true
 branch = true
 source = ["exoplanet"]
 omit = [
   "*_test.py",
@@ -33,9 +32,9 @@
 [tool.coverage.report]
 show_missing = true
 exclude_lines = [
   "raise NotImplementedError",
   "except ImportError",
   "pragma: no cover",
   "def R_op",
-  "if verbose"
+  "if verbose",
 ]
```

### Comparing `exoplanet-0.5.3rc1/setup.py` & `exoplanet-0.6.0rc2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,36 +19,40 @@
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
-INSTALL_REQUIRES = [
-    "exoplanet-core>=0.1,<0.2",
-    "pymc3>=3.9",
-    "aesara-theano-fallback>=0.0.2",
-    "astropy>=3.1",
-    "numpy<1.22",
-]
+INSTALL_REQUIRES = ["astropy>=3.1"]
 EXTRA_REQUIRE = {
-    "extras": ["pymc3-ext>=0.1.0", "celerite2>=0.2.0"],
-    "test": [
-        "scipy",
-        "pytest",
-        "coverage[toml]",
-        "pytest-env",
+    "pymc3": [
+        "pymc3>=3.9",
+        "numpy<1.22",
+        "aesara-theano-fallback>=0.0.2",
+        "xarray<2023.10.0",
+        "exoplanet-core>=0.2.0",
+    ],
+    "pymc": ["pymc>=5.0.0", "exoplanet-core>=0.3.0"],
+    "extras": ["pymc>=5.0.0", "pymc-ext>=1.0.1", "celerite2>=0.3.1"],
+    "extras-pymc3": [
+        "pymc3>=3.9",
+        "pymc3-ext>=0.1.0",
+        "celerite2>=0.2.0,<0.3.1",
     ],
+    "test": ["scipy", "pytest", "pytest-env"],
     "docs": [
+        "exoplanet-core>=0.3.0",
+        "pymc>=5.0.0",
+        "pymc-ext>=1.0.1",
         "sphinx-book-theme",
         "myst-nb",
+        "ipython",
         "matplotlib",
         "corner",
-        "lightkurve",
-        "pymc3-ext>=0.1.0",
         "emcee",
     ],
 }
 
 # END PROJECT SPECIFIC
```

### Comparing `exoplanet-0.5.3rc1/src/exoplanet/citations.py` & `exoplanet-0.6.0rc2/src/exoplanet/citations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-# -*- coding: utf-8 -*-
-
 __all__ = ["add_citations_to_model", "CITATIONS"]
 
 import logging
 import textwrap
 
-import pymc3 as pm
+from exoplanet.compat import USING_PYMC3, pm
 
 
 def add_citations_to_model(citations, model=None):
     try:
         model = pm.modelcontext(model)
         if not hasattr(model, "__citations__"):
             model.__citations__ = dict()
@@ -17,38 +15,35 @@
             model.__citations__[k] = CITATIONS[k]
 
     except TypeError:
         pass
 
 
 def get_citations_for_model(model=None, width=79):
-    """Get the citations for the components used an exoplanet PyMC3
+    """Get the citations for the components used an exoplanet PyMC model
 
     Returns: The acknowledgement text for exoplanet and its dependencies and a
     string containing the BibTeX entries for the citations in the
     acknowledgement.
 
     """
     model = pm.modelcontext(model)
     if not hasattr(model, "__citations__"):
         logging.warning("no citations registered with model")
         return "", ""
 
-    cite = (
-        list(CITATIONS["pymc3"][0])
-        + list(CITATIONS["theano"][0])
-        + list(CITATIONS["arviz"][0])
-    )
+    cite = list(CITATIONS["arviz"][0])
     bib = [
         CITATIONS["exoplanet"][1],
-        CITATIONS["pymc3"][1],
-        CITATIONS["theano"][1],
         CITATIONS["arviz"][1],
     ]
-    for k, v in model.__citations__.items():
+    if USING_PYMC3:
+        cite += list(CITATIONS["pymc3"][0]) + list(CITATIONS["theano"][0])
+        bib += [CITATIONS["pymc3"][1], CITATIONS["theano"][1]]
+    for _, v in model.__citations__.items():
         cite += list(v[0])
         bib.append(v[1])
 
     txt = (
         r"This research made use of \textsf{{exoplanet}} "
         r"\citep{{exoplanet:joss, exoplanet:zenodo}} and its dependencies "
         r"\citep{{{0}}}."
```

### Comparing `exoplanet-0.5.3rc1/src/exoplanet/estimators.py` & `exoplanet-0.6.0rc2/src/exoplanet/estimators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 __all__ = [
     "estimate_semi_amplitude",
     "estimate_minimum_mass",
     "find_peaks",
     "lomb_scargle_estimator",
     "autocorr_estimator",
     "bls_estimator",
```

### Comparing `exoplanet-0.5.3rc1/src/exoplanet/interp.py` & `exoplanet-0.6.0rc2/src/exoplanet/interp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-# -*- coding: utf-8 -*-
-
 __all__ = ["regular_grid_interp", "RegularGridInterpolator"]
 
 import itertools
 
-import aesara_theano_fallback.tensor as tt
-import numpy as np
-
-from .utils import as_tensor_variable
+from exoplanet.compat import tensor as pt
+from exoplanet.utils import as_tensor_variable
 
 
 def regular_grid_interp(points, values, coords, *, fill_value=None):
     """Perform a linear interpolation in N-dimensions w a regular grid
 
     The data must be defined on a filled regular grid, but the spacing may be
     uneven in any of the dimensions.
@@ -35,32 +31,32 @@
     ndim = len(points)
     values = as_tensor_variable(values)
     coords = as_tensor_variable(coords)
 
     # Find where the points should be inserted
     indices = []
     norm_distances = []
-    out_of_bounds = tt.zeros(coords.shape[:-1], dtype=bool)
+    out_of_bounds = pt.zeros(coords.shape[:-1], dtype=bool)
     for n, grid in enumerate(points):
         x = coords[..., n]
-        i = tt.extra_ops.searchsorted(grid, x) - 1
+        i = pt.extra_ops.searchsorted(grid, x) - 1
         out_of_bounds |= (i < 0) | (i >= grid.shape[0] - 1)
-        i = tt.clip(i, 0, grid.shape[0] - 2)
+        i = pt.clip(i, 0, grid.shape[0] - 2)
         indices.append(i)
         norm_distances.append((x - grid[i]) / (grid[i + 1] - grid[i]))
 
-    result = tt.zeros(tuple(coords.shape[:-1]) + tuple(values.shape[ndim:]))
+    result = pt.zeros(tuple(coords.shape[:-1]) + tuple(values.shape[ndim:]))
     for edge_indices in itertools.product(*((i, i + 1) for i in indices)):
-        weight = tt.ones(coords.shape[:-1])
+        weight = pt.ones(coords.shape[:-1])
         for ei, i, yi in zip(edge_indices, indices, norm_distances):
-            weight *= tt.where(tt.eq(ei, i), 1 - yi, yi)
+            weight *= pt.where(pt.eq(ei, i), 1 - yi, yi)
         result += values[edge_indices] * weight
 
     if fill_value is not None:
-        result = tt.switch(out_of_bounds, fill_value, result)
+        result = pt.switch(out_of_bounds, fill_value, result)
 
     return result
 
 
 class RegularGridInterpolator:
     """Linear interpolation on a regular grid in arbitrary dimensions
```

### Comparing `exoplanet-0.5.3rc1/src/exoplanet/light_curves/interpolated.py` & `exoplanet-0.6.0rc2/src/exoplanet/light_curves/interpolated.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-# -*- coding: utf-8 -*-
-
 __all__ = ["InterpolatedLightCurve"]
 
-import aesara_theano_fallback.tensor as tt
 import numpy as np
 
+from exoplanet.compat import tensor as pt
+
 
 def interp(n, x, xmin, xmax, dx, func):
     """One-dimensional regularly spaced cubic interpolation
 
     Args:
         n (int): The axis of the output that should be interpolated
         x (tensor): The x coordinates where the model should be evaluated
@@ -16,28 +15,28 @@
         xmax (scalar): The last coordinate in the grid
         dx (scalar): The grid spacing
         func (callable): The function that should be interpolated
 
     Returns:
         y: The function ``func`` interpolated to the coordinates ``x``
     """
-    xp = tt.arange(xmin - dx, xmax + 2.5 * dx, dx)
+    xp = pt.arange(xmin - dx, xmax + 2.5 * dx, dx)
     yp = func(xp)
 
     y0 = yp[:-3, n]
     y1 = yp[1:-2, n]
     y2 = yp[2:-1, n]
     y3 = yp[3:, n]
 
     a0 = y1
     a1 = -y0 / 3.0 - 0.5 * y1 + y2 - y3 / 6.0
     a2 = 0.5 * (y0 + y2) - y1
     a3 = 0.5 * ((y1 - y2) + (y3 - y0) / 3.0)
 
-    inds = tt.cast(tt.floor((x - xmin) / dx), "int64")
+    inds = pt.cast(pt.floor((x - xmin) / dx), "int64")
     x0 = (x - xp[inds + 1]) / dx
     return a0[inds] + a1[inds] * x0 + a2[inds] * x0**2 + a3[inds] * x0**3
 
 
 class InterpolatedLightCurve:
     """This light curve object is an EXPERIMENTAL and UNTESTED interface for
     pre-computing transit light curves on a grid and then interpolating this
@@ -87,15 +86,15 @@
                 use_in_transit=use_in_transit,
                 light_delay=light_delay,
             )
             mn = orbit.t0
             mx = orbit.t0 + orbit.period
             return interp(
                 0,
-                tt.mod(t - orbit.t0, orbit.period) + orbit.t0,
+                pt.mod(t - orbit.t0, orbit.period) + orbit.t0,
                 mn,
                 mx,
                 (mx - mn) / (self.num_phase + 1),
                 func,
             )[:, None]
 
         ys = []
@@ -111,23 +110,23 @@
                 light_delay=light_delay,
             )
             mn = orbit.t0[n]
             mx = orbit.t0[n] + orbit.period[n]
             ys.append(
                 interp(
                     n,
-                    tt.mod(t - orbit.t0[n], orbit.period[n]) + orbit.t0[n],
+                    pt.mod(t - orbit.t0[n], orbit.period[n]) + orbit.t0[n],
                     mn,
                     mx,
                     (mx - mn) / (self.num_phase + 1),
                     func,
                 )
             )
 
-        return tt.stack(ys, axis=-1)
+        return pt.stack(ys, axis=-1)
 
 
 class _wrapper:
     def __init__(self, base_light_curve, *args, **kwargs):
         self.base_light_curve = base_light_curve
         self.args = args
         self.kwargs = kwargs
```

### Comparing `exoplanet-0.5.3rc1/src/exoplanet/light_curves/limb_dark.py` & `exoplanet-0.6.0rc2/src/exoplanet/light_curves/limb_dark.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-# -*- coding: utf-8 -*-
-
 __all__ = ["LimbDarkLightCurve"]
 
-import aesara_theano_fallback.tensor as tt
 import numpy as np
-from aesara_theano_fallback import aesara as theano
-from exoplanet_core.pymc import ops
 
-from ..citations import add_citations_to_model
-from ..utils import as_tensor_variable, deprecation_warning
+from exoplanet.citations import add_citations_to_model
+from exoplanet.compat import Assert, ops
+from exoplanet.compat import tensor as pt
+from exoplanet.utils import as_tensor_variable, deprecation_warning
 
 
 def get_cl(u1, u2):
     u1 = as_tensor_variable(u1)
     u2 = as_tensor_variable(u2)
     c0 = 1 - u1 - 1.5 * u2
     c1 = u1 + 2 * u2
     c2 = -0.25 * u2
     norm = np.pi * (c0 + c1 / 1.5)
-    return tt.stack([c0, c1, c2]) / norm
+    return pt.stack([c0, c1, c2]) / norm
 
 
 def quad_limbdark_light_curve(c, b, r):
     b = as_tensor_variable(b)
     r = as_tensor_variable(r)
-    return tt.dot(ops.quad_solution_vector(b, r), c) - 1.0
+    return pt.dot(ops.quad_solution_vector(b, r), c) - 1.0
 
 
 class LimbDarkLightCurve:
     """A quadratically limb darkened light curve
 
     .. note:: Earlier versions of exoplanet supported higher (and lower) order
         limb darkening, but this support was removed in v0.5.0. For higher
@@ -51,20 +48,20 @@
 
             # If a vector is provided, we need to assert that it is 2D
             msg = (
                 "only quadratic limb darkening is supported; "
                 "use `starry` for more flexibility"
             )
             try:
-                assert_op = theano.assert_op.Assert(msg)
+                assert_op = Assert(msg)
             except AttributeError:
-                assert_op = tt.opt.Assert(msg)
+                assert_op = Assert(msg)
             u1 = as_tensor_variable(u1)
             u1 = assert_op(
-                u1, tt.and_(tt.eq(u1.ndim, 1), tt.eq(u1.shape[0], 2))
+                u1, pt.and_(pt.eq(u1.ndim, 1), pt.eq(u1.shape[0], 2))
             )
 
             self.u1 = u1[0]
             self.u2 = u1[1]
         else:
             self.u1 = as_tensor_variable(u1)
             self.u2 = as_tensor_variable(u2)
@@ -86,22 +83,22 @@
             ror: The radius ratio that approximately corresponds to the depth
             ``delta`` at impact parameter ``b``.
 
         """
         b = as_tensor_variable(b)
         delta = as_tensor_variable(delta)
         f0 = 1 - 2 * self.u1 / 6.0 - 2 * self.u2 / 12.0
-        arg = 1 - tt.sqrt(1 - b**2)
+        arg = 1 - pt.sqrt(1 - b**2)
         f = 1 - self.u1 * arg - self.u2 * arg**2
         factor = f0 / f
-        ror = tt.sqrt(delta * factor)
+        ror = pt.sqrt(delta * factor)
         if not jac:
-            return tt.reshape(ror, b.shape)
+            return pt.reshape(ror, b.shape)
         drorddelta = 0.5 * factor / ror
-        return tt.reshape(ror, b.shape), tt.reshape(drorddelta, b.shape)
+        return pt.reshape(ror, b.shape), pt.reshape(drorddelta, b.shape)
 
     def get_light_curve(
         self,
         orbit=None,
         r=None,
         t=None,
         texp=None,
@@ -156,31 +153,31 @@
             raise ValueError("missing required argument 't'")
 
         use_in_transit = (
             not light_delay if use_in_transit is None else use_in_transit
         )
 
         r = as_tensor_variable(r)
-        r = tt.reshape(r, (r.size,))
+        r = pt.reshape(r, (r.size,))
         t = as_tensor_variable(t)
 
         # If use_in_transit, we should only evaluate the model at times where
         # at least one planet is transiting
         if use_in_transit:
-            transit_model = tt.shape_padleft(
-                tt.zeros_like(r), t.ndim
-            ) + tt.shape_padright(tt.zeros_like(t), r.ndim)
+            transit_model = pt.shape_padleft(
+                pt.zeros_like(r), t.ndim
+            ) + pt.shape_padright(pt.zeros_like(t), r.ndim)
             inds = orbit.in_transit(t, r=r, texp=texp, light_delay=light_delay)
             t = t[inds]
 
         # Handle exposure time integration
         if texp is None:
             tgrid = t
-            rgrid = tt.shape_padleft(r, tgrid.ndim) + tt.shape_padright(
-                tt.zeros_like(tgrid), r.ndim
+            rgrid = pt.shape_padleft(r, tgrid.ndim) + pt.shape_padright(
+                pt.zeros_like(tgrid), r.ndim
             )
         else:
             texp = as_tensor_variable(texp)
 
             oversample = int(oversample)
             oversample += 1 - oversample % 2
             stencil = np.ones(oversample)
@@ -199,41 +196,41 @@
                 raise ValueError("order must be <= 2")
             stencil /= np.sum(stencil)
 
             if texp.ndim == 0:
                 dt = texp * dt
             else:
                 if use_in_transit:
-                    dt = tt.shape_padright(texp[inds]) * dt
+                    dt = pt.shape_padright(texp[inds]) * dt
                 else:
-                    dt = tt.shape_padright(texp) * dt
-            tgrid = tt.shape_padright(t) + dt
+                    dt = pt.shape_padright(texp) * dt
+            tgrid = pt.shape_padright(t) + dt
 
             # Madness to get the shapes to work out...
-            rgrid = tt.shape_padleft(r, tgrid.ndim) + tt.shape_padright(
-                tt.zeros_like(tgrid), 1
+            rgrid = pt.shape_padleft(r, tgrid.ndim) + pt.shape_padright(
+                pt.zeros_like(tgrid), 1
             )
 
         # Evalute the coordinates of the transiting body in the plane of the
         # sky
         coords = orbit.get_relative_position(tgrid, light_delay=light_delay)
-        b = tt.sqrt(coords[0] ** 2 + coords[1] ** 2)
-        b = tt.reshape(b, rgrid.shape)
-        los = tt.reshape(coords[2], rgrid.shape)
+        b = pt.sqrt(coords[0] ** 2 + coords[1] ** 2)
+        b = pt.reshape(b, rgrid.shape)
+        los = pt.reshape(coords[2], rgrid.shape)
 
         lc = self._compute_light_curve(
             b / orbit.r_star, rgrid / orbit.r_star, los / orbit.r_star
         )
 
         if texp is not None:
-            stencil = tt.shape_padright(tt.shape_padleft(stencil, t.ndim), 1)
-            lc = tt.sum(stencil * lc, axis=t.ndim)
+            stencil = pt.shape_padright(pt.shape_padleft(stencil, t.ndim), 1)
+            lc = pt.sum(stencil * lc, axis=t.ndim)
 
         if use_in_transit:
-            transit_model = tt.set_subtensor(transit_model[inds], lc)
+            transit_model = pt.set_subtensor(transit_model[inds], lc)
             return transit_model
         else:
             return lc
 
     def _compute_light_curve(self, b, r, los=None):
         """Compute the light curve for a set of impact parameters and radii
 
@@ -246,10 +243,10 @@
             los (Optional[tensor]): The coordinates of the body along the
                 line-of-sight. If ``los > 0`` the body is between the observer
                 and the source.
 
         """
         b = as_tensor_variable(b)
         if los is None:
-            los = tt.ones_like(b)
+            los = pt.ones_like(b)
         lc = quad_limbdark_light_curve(self.c, b, r)
-        return tt.switch(tt.gt(los, 0), lc, tt.zeros_like(lc))
+        return pt.switch(pt.gt(los, 0), lc, pt.zeros_like(lc))
```

### Comparing `exoplanet-0.5.3rc1/src/exoplanet/light_curves/secondary_eclipse.py` & `exoplanet-0.6.0rc2/src/exoplanet/light_curves/secondary_eclipse.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# -*- coding: utf-8 -*-
-
 __all__ = ["SecondaryEclipseLightCurve"]
 
-from ..utils import as_tensor_variable
-from .limb_dark import LimbDarkLightCurve
+from exoplanet.light_curves.limb_dark import LimbDarkLightCurve
+from exoplanet.utils import as_tensor_variable
 
 
 class SecondaryEclipseLightCurve:
     """The light curve for a secondary eclipse model computed using starry
 
     Args:
         u_primary (vector): A vector of limb darkening coefficients for the
```

### Comparing `exoplanet-0.5.3rc1/src/exoplanet/orbits/constants.py` & `exoplanet-0.6.0rc2/src/exoplanet/orbits/constants.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 __all__ = [
     "G_grav",
     "gcc_per_sun",
     "au_per_R_sun",
     "day_per_yr_over_2pi",
     "c_light",
 ]
@@ -18,19 +16,15 @@
     G_grav = c.G.to(u.R_sun**3 / u.M_sun / u.day**2).value
     gcc_per_sun = (u.M_sun / u.R_sun**3).to(u.g / u.cm**3)
     au_per_R_sun = u.R_sun.to(u.au)
     c_light = c.c.to(u.R_sun / u.day).value
 
     day_per_yr_over_2pi = (
         (1.0 * u.au) ** (3 / 2)
-        / (
-            np.sqrt(
-                c.G.to(u.au**3 / (u.M_sun * u.day**2)) * (1.0 * u.M_sun)
-            )
-        )
+        / (np.sqrt(c.G.to(u.au**3 / (u.M_sun * u.day**2)) * (1.0 * u.M_sun)))
     ).value
 
 except TypeError:
     warnings.warn(
         "Something went wrong when computing units. "
         "Check that AstroPy is working.",
         category=RuntimeWarning,
```

### Comparing `exoplanet-0.5.3rc1/src/exoplanet/orbits/dur_to_ecc.py` & `exoplanet-0.6.0rc2/src/exoplanet/orbits/dur_to_ecc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-# -*- coding: utf-8 -*-
-
 """This module has an EXPERIMENTAL and UNTESTED implementation of analytic
 marginalizion over eccentricity as a function of transit duration (since the
 mapping is not 1-to-1). The implementation as written probably DOES NOT WORK,
 but I've (DFM) left it here for my own future reference. Feel free to ping me
 if you're interested in what's going on here!"""
 
 __all__ = ["duration_to_eccentricity"]
 
 from itertools import product
 
-import aesara_theano_fallback.tensor as tt
 import numpy as np
-import pymc3 as pm
 
-from .keplerian import KeplerianOrbit, _get_consistent_inputs
+from exoplanet.compat import pm
+from exoplanet.compat import tensor as pt
+from exoplanet.orbits.keplerian import KeplerianOrbit, _get_consistent_inputs
 
 
 def duration_to_eccentricity(
     func, duration, ror, **kwargs
 ):  # pragma: no cover
     num_planets = kwargs.pop("num_planets", 1)
     orbit_type = kwargs.pop("orbit_type", KeplerianOrbit)
@@ -32,83 +30,81 @@
         kwargs.get("m_star", None),
         kwargs.get("rho_star_units", None),
         kwargs.get("m_planet", 0.0),
         kwargs.get("m_planet_units", None),
     )
     a, period, rho_star, r_star, m_star, m_planet = inputs
     b = kwargs.get("b", 0.0)
-    s = tt.sin(kwargs["omega"])
-    umax_inv = tt.switch(tt.lt(s, 0), tt.sqrt(1 - s**2), 1.0)
+    s = pt.sin(kwargs["omega"])
+    umax_inv = pt.switch(pt.lt(s, 0), pt.sqrt(1 - s**2), 1.0)
 
-    const = (
-        period * tt.shape_padright(r_star) * tt.sqrt((1 + ror) ** 2 - b**2)
-    )
+    const = period * pt.shape_padright(r_star) * pt.sqrt((1 + ror) ** 2 - b**2)
     const /= np.pi * a
 
     u = duration / const
 
     e1 = -s * u**2 / ((s * u) ** 2 + 1)
-    e2 = tt.sqrt((s**2 - 1) * u**2 + 1) / ((s * u) ** 2 + 1)
+    e2 = pt.sqrt((s**2 - 1) * u**2 + 1) / ((s * u) ** 2 + 1)
 
     models = []
     logjacs = []
     logprobs = []
     for args in product(*(zip("np", (-1, 1)) for _ in range(num_planets))):
         labels, signs = zip(*args)
 
         # Compute the eccentricity branch
-        ecc = tt.stack([e1[i] + signs[i] * e2[i] for i in range(num_planets)])
+        ecc = pt.stack([e1[i] + signs[i] * e2[i] for i in range(num_planets)])
 
         # Work out the Jacobian
-        valid_ecc = tt.and_(tt.lt(ecc, 1.0), tt.ge(ecc, 0.0))
-        logjac = tt.switch(
-            tt.all(valid_ecc),
-            tt.sum(
-                0.5 * tt.log(1 - ecc**2)
-                + 2 * tt.log(s * ecc + 1)
-                - tt.log(tt.abs_(s + ecc))
-                - tt.log(const)
+        valid_ecc = pt.and_(pt.lt(ecc, 1.0), pt.ge(ecc, 0.0))
+        logjac = pt.switch(
+            pt.all(valid_ecc),
+            pt.sum(
+                0.5 * pt.log(1 - ecc**2)
+                + 2 * pt.log(s * ecc + 1)
+                - pt.log(pt.abs(s + ecc))
+                - pt.log(const)
             ),
             -np.inf,
         )
-        ecc = tt.switch(valid_ecc, ecc, tt.zeros_like(ecc))
+        ecc = pt.switch(valid_ecc, ecc, pt.zeros_like(ecc))
 
         # Create a sub-model to capture this component
         with pm.Model(name="dur_ecc_" + "_".join(labels)) as model:
             pm.Deterministic("ecc", ecc)
             orbit = orbit_type(ecc=ecc, **kwargs)
-            logprob = tt.sum(func(orbit))
+            logprob = pt.sum(func(orbit))
 
         models.append(model)
         logjacs.append(logjac)
         logprobs.append(logprob)
 
     # Compute the marginalized likelihood
-    logjacs = tt.stack(logjacs)
-    logprobs = tt.stack(logprobs)
-    logprob = tt.switch(
-        tt.gt(1.0 / u, umax_inv),
-        tt.sum(pm.logsumexp(logprobs + logjacs)),
+    logjacs = pt.stack(logjacs)
+    logprobs = pt.stack(logprobs)
+    logprob = pt.switch(
+        pt.gt(1.0 / u, umax_inv),
+        pt.sum(pm.logsumexp(logprobs + logjacs)),
         -np.inf,
     )
     pm.Potential(name + "_logp", logprob)
     pm.Deterministic(name + "_logjacs", logjacs)
     pm.Deterministic(name + "_logprobs", logprobs)
 
     # Loop over models and compute the marginalized values for all the
     # parameters and deterministics
-    norm = tt.sum(pm.logsumexp(logjacs))
-    logw = tt.switch(
-        tt.gt(1.0 / u, umax_inv),
+    norm = pt.sum(pm.logsumexp(logjacs))
+    logw = pt.switch(
+        pt.gt(1.0 / u, umax_inv),
         logjacs - norm,
-        -np.inf + tt.zeros_like(logjacs),
+        -np.inf + pt.zeros_like(logjacs),
     )
     pm.Deterministic(name + "_logw", logw)
     for k in models[0].named_vars.keys():
         name = k[len(models[0].name) + 1 :]
         pm.Deterministic(
             name,
             sum(
-                tt.exp(logw[i]) * model.named_vars[model.name + "_" + name]
+                pt.exp(logw[i]) * model.named_vars[model.name + "_" + name]
                 for i, model in enumerate(models)
             ),
         )
```

### Comparing `exoplanet-0.5.3rc1/src/exoplanet/orbits/keplerian.py` & `exoplanet-0.6.0rc2/src/exoplanet/orbits/keplerian.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-# -*- coding: utf-8 -*-
-
 __all__ = [
     "KeplerianOrbit",
     "get_true_anomaly",
     "get_aor_from_transit_duration",
 ]
 
 import warnings
 from collections import defaultdict
 
-import aesara_theano_fallback.tensor as tt
 import numpy as np
-from aesara_theano_fallback import ifelse
 from astropy import units as u
-from exoplanet_core.pymc import ops
 
-from ..citations import add_citations_to_model
-from ..units import has_unit, to_unit, with_unit
-from ..utils import as_tensor_variable, deprecation_warning
-from .constants import G_grav, au_per_R_sun, c_light, gcc_per_sun
+from exoplanet.citations import add_citations_to_model
+from exoplanet.compat import ifelse, ops
+from exoplanet.compat import tensor as pt
+from exoplanet.orbits.constants import (
+    G_grav,
+    au_per_R_sun,
+    c_light,
+    gcc_per_sun,
+)
+from exoplanet.units import has_unit, to_unit, with_unit
+from exoplanet.utils import as_tensor_variable, deprecation_warning
 
 
 class KeplerianOrbit:
     """A system of bodies on Keplerian orbits around a common central
 
     Given the input parameters, the values of all other parameters will be
     computed so a ``KeplerianOrbit`` instance will always have attributes for
@@ -169,118 +171,118 @@
 
         self.K0 = self.n * self.a / self.m_total
 
         if Omega is None:
             self.Omega = None
         else:
             self.Omega = as_tensor_variable(Omega)
-            self.cos_Omega = tt.cos(self.Omega)
-            self.sin_Omega = tt.sin(self.Omega)
+            self.cos_Omega = pt.cos(self.Omega)
+            self.sin_Omega = pt.sin(self.Omega)
 
         # Eccentricity
         if ecc is None:
             self.ecc = None
-            self.M0 = 0.5 * np.pi + tt.zeros_like(self.n)
+            self.M0 = 0.5 * np.pi + pt.zeros_like(self.n)
             incl_factor = 1
         else:
             self.ecc = as_tensor_variable(ecc)
             if omega is not None:
                 if sin_omega is not None and cos_omega is not None:
                     raise ValueError(
                         "either 'omega' or 'sin_omega' and 'cos_omega' can be "
                         "provided"
                     )
                 self.omega = as_tensor_variable(omega)
-                self.cos_omega = tt.cos(self.omega)
-                self.sin_omega = tt.sin(self.omega)
+                self.cos_omega = pt.cos(self.omega)
+                self.sin_omega = pt.sin(self.omega)
             elif sin_omega is not None and cos_omega is not None:
                 self.cos_omega = as_tensor_variable(cos_omega)
                 self.sin_omega = as_tensor_variable(sin_omega)
-                self.omega = tt.arctan2(self.sin_omega, self.cos_omega)
+                self.omega = pt.arctan2(self.sin_omega, self.cos_omega)
 
             else:
                 raise ValueError("both e and omega must be provided")
 
             opsw = 1 + self.sin_omega
-            E0 = 2 * tt.arctan2(
-                tt.sqrt(1 - self.ecc) * self.cos_omega,
-                tt.sqrt(1 + self.ecc) * opsw,
+            E0 = 2 * pt.arctan2(
+                pt.sqrt(1 - self.ecc) * self.cos_omega,
+                pt.sqrt(1 + self.ecc) * opsw,
             )
-            self.M0 = E0 - self.ecc * tt.sin(E0)
+            self.M0 = E0 - self.ecc * pt.sin(E0)
 
             ome2 = 1 - self.ecc**2
-            self.K0 /= tt.sqrt(ome2)
+            self.K0 /= pt.sqrt(ome2)
             incl_factor = (1 + self.ecc * self.sin_omega) / ome2
 
         # The Jacobian for the transform cos(i) -> b
         self.dcosidb = self.jacobians["b"]["cos_incl"] = (
             incl_factor * self.r_star / self.a
         )
 
         if b is not None:
             if incl is not None or duration is not None:
                 raise ValueError(
                     "only one of 'incl', 'b', and 'duration' can be given"
                 )
             self.b = as_tensor_variable(b)
             self.cos_incl = self.dcosidb * self.b
-            self.incl = tt.arccos(self.cos_incl)
+            self.incl = pt.arccos(self.cos_incl)
         elif incl is not None:
             if duration is not None:
                 raise ValueError(
                     "only one of 'incl', 'b', and 'duration' can be given"
                 )
             self.incl = as_tensor_variable(incl)
-            self.cos_incl = tt.cos(self.incl)
+            self.cos_incl = pt.cos(self.incl)
             self.b = self.cos_incl / self.dcosidb
         elif duration is not None:
             # This assertion should never be hit because of the first
             # conditional in this method, but let's keep it here anyways
             assert self.ecc is not None
 
             self.duration = as_tensor_variable(to_unit(duration, u.day))
-            c = tt.sin(np.pi * self.duration * incl_factor / self.period)
+            c = pt.sin(np.pi * self.duration * incl_factor / self.period)
             c2 = c * c
             aor = self.a_planet / self.r_star
             esinw = self.ecc * self.sin_omega
-            self.b = tt.sqrt(
+            self.b = pt.sqrt(
                 (aor**2 * c2 - 1)
                 / (
                     c2 * esinw**2
                     + 2 * c2 * esinw
                     + c2
                     - self.ecc**4
                     + 2 * self.ecc**2
                     - 1
                 )
             )
             self.b *= 1 - self.ecc**2
             self.cos_incl = self.dcosidb * self.b
-            self.incl = tt.arccos(self.cos_incl)
+            self.incl = pt.arccos(self.cos_incl)
         else:
-            zla = tt.zeros_like(self.a)
+            zla = pt.zeros_like(self.a)
             self.incl = 0.5 * np.pi + zla
             self.cos_incl = zla
             self.b = zla
 
         if t0 is not None and t_periastron is not None:
             raise ValueError("you can't define both t0 and t_periastron")
         if t0 is None and t_periastron is None:
-            t0 = tt.zeros_like(self.period)
+            t0 = pt.zeros_like(self.period)
 
         if t0 is None:
             self.t_periastron = as_tensor_variable(t_periastron)
             self.t0 = self.t_periastron + self.M0 / self.n
         else:
             self.t0 = as_tensor_variable(t0)
             self.t_periastron = self.t0 - self.M0 / self.n
 
         self.tref = self.t_periastron - self.t0
 
-        self.sin_incl = tt.sin(self.incl)
+        self.sin_incl = pt.sin(self.incl)
 
     def _rotate_vector(self, x, y):
         """Apply the rotation matrices to go from orbit to observer frame
 
         In order,
         1. rotate about the z axis by an amount omega -> x1, y1, z1
         2. rotate about the x1 axis by an amount -incl -> x2, y2, z2
@@ -317,22 +319,22 @@
 
         X = self.cos_Omega * x2 - self.sin_Omega * y2
         Y = self.sin_Omega * x2 + self.cos_Omega * y2
         return X, Y, Z
 
     def _warp_times(self, t, _pad=True):
         if _pad:
-            return tt.shape_padright(t) - self.t0
+            return pt.shape_padright(t) - self.t0
         return t - self.t0
 
     def _get_true_anomaly(self, t, _pad=True):
         M = (self._warp_times(t, _pad=_pad) - self.tref) * self.n
         if self.ecc is None:
-            return tt.sin(M), tt.cos(M)
-        sinf, cosf = ops.kepler(M, self.ecc + tt.zeros_like(M))
+            return pt.sin(M), pt.cos(M)
+        sinf, cosf = ops.kepler(M, self.ecc + pt.zeros_like(M))
         return sinf, cosf
 
     def _get_position_and_velocity(self, t, parallax=None):
         sinf, cosf = self._get_true_anomaly(t)
 
         if self.ecc is None:
             r = 1.0
@@ -341,33 +343,33 @@
             r = (1.0 - self.ecc**2) / (1 + self.ecc * cosf)
             vx, vy, vz = self._rotate_vector(
                 -self.K0 * sinf, self.K0 * (cosf + self.ecc)
             )
 
         x, y, z = self._rotate_vector(r * cosf, r * sinf)
 
-        pos = tt.stack((x, y, z), axis=-1)
-        pos = tt.concatenate(
+        pos = pt.stack((x, y, z), axis=-1)
+        pos = pt.concatenate(
             (
-                tt.sum(
-                    tt.shape_padright(self.a_star) * pos, axis=0, keepdims=True
+                pt.sum(
+                    pt.shape_padright(self.a_star) * pos, axis=0, keepdims=True
                 ),
-                tt.shape_padright(self.a_planet) * pos,
+                pt.shape_padright(self.a_planet) * pos,
             ),
             axis=0,
         )
-        vel = tt.stack((vx, vy, vz), axis=-1)
-        vel = tt.concatenate(
+        vel = pt.stack((vx, vy, vz), axis=-1)
+        vel = pt.concatenate(
             (
-                tt.sum(
-                    tt.shape_padright(self.m_planet) * vel,
+                pt.sum(
+                    pt.shape_padright(self.m_planet) * vel,
                     axis=0,
                     keepdims=True,
                 ),
-                -tt.shape_padright(self.m_star) * vel,
+                -pt.shape_padright(self.m_star) * vel,
             ),
             axis=0,
         )
 
         if parallax is not None:
             # convert r into arcseconds
             pos = pos * (parallax * au_per_R_sun)
@@ -429,42 +431,42 @@
         angvel = 2 * np.pi / self.period
         if self.ecc is None:
             r = a
             vamp = angvel * a
             vz = vamp * self.sin_incl * cosf
         else:
             r = a * (1.0 - self.ecc**2) / (1 + self.ecc * cosf)
-            vamp = angvel * a / tt.sqrt(1 - self.ecc**2)
+            vamp = angvel * a / pt.sqrt(1 - self.ecc**2)
             cwf = self.cos_omega * cosf - self.sin_omega * sinf
             vz = vamp * self.sin_incl * (self.ecc * self.cos_omega + cwf)
 
         # True position of the body
         x, y, z = self._rotate_vector(r * cosf, r * sinf)
 
         # Component of the acceleration in the z direction
         az = -(angvel**2) * (a / r) ** 3 * z
 
         # Compute the time delay at the **retarded** position, accounting
         # for the instantaneous velocity and acceleration of the body.
         # See the derivation at https://github.com/rodluger/starry/issues/66
-        delay = tt.switch(
-            tt.lt(tt.abs_(az), 1.0e-10),
+        delay = pt.switch(
+            pt.lt(pt.abs(az), 1.0e-10),
             (z0 - z) / (c_light + vz),
             (c_light / az)
             * (
                 (1 + vz / c_light)
-                - tt.sqrt(
+                - pt.sqrt(
                     (1 + vz / c_light) * (1 + vz / c_light)
                     - 2 * az * (z0 - z) / c_light**2
                 )
             ),
         )
 
         if _pad:
-            new_t = tt.shape_padright(t) - delay
+            new_t = pt.shape_padright(t) - delay
         else:
             new_t = t - delay
 
         # Re-compute Kepler's equation, this time at the **retarded** position
         return self._get_position(a, new_t, parallax, _pad=False)
 
     def get_planet_position(self, t, parallax=None, light_delay=False):
@@ -477,15 +479,15 @@
 
         Returns:
             The components of the position vector at ``t`` in units of
             ``R_sun``.
 
         """
         return tuple(
-            tt.squeeze(x)
+            pt.squeeze(x)
             for x in self._get_position(
                 self.a_planet, t, parallax, light_delay=light_delay
             )
         )
 
     def get_star_position(self, t, parallax=None, light_delay=False):
         """The star's position in the barycentric frame
@@ -502,15 +504,15 @@
 
         Returns:
             The components of the position vector at ``t`` in units of
             ``R_sun``.
 
         """
         return tuple(
-            tt.squeeze(x)
+            pt.squeeze(x)
             for x in self._get_position(
                 self.a_star, t, parallax, light_delay=light_delay
             )
         )
 
     def get_relative_position(self, t, parallax=None, light_delay=False):
         """The planets' positions relative to the star in the X,Y,Z frame.
@@ -529,15 +531,15 @@
 
         Returns:
             The components of the position vector at ``t`` in units of
             ``R_sun``.
 
         """
         return tuple(
-            tt.squeeze(x)
+            pt.squeeze(x)
             for x in self._get_position(
                 -self.a, t, parallax, light_delay=light_delay
             )
         )
 
     def get_relative_angles(self, t, parallax=None, light_delay=False):
         """The planets' relative position to the star in the sky plane, in
@@ -558,16 +560,16 @@
 
         """
         X, Y, Z = self._get_position(
             -self.a, t, parallax, light_delay=light_delay
         )
 
         # calculate rho and theta
-        rho = tt.squeeze(tt.sqrt(X**2 + Y**2))  # arcsec
-        theta = tt.squeeze(tt.arctan2(Y, X))  # radians between [-pi, pi]
+        rho = pt.squeeze(pt.sqrt(X**2 + Y**2))  # arcsec
+        theta = pt.squeeze(pt.arctan2(Y, X))  # radians between [-pi, pi]
 
         return (rho, theta)
 
     def _get_velocity(self, m, t):
         """Get the velocity vector of a body in the observer frame"""
         sinf, cosf = self._get_true_anomaly(t)
         K = self.K0 * m
@@ -583,15 +585,15 @@
 
         Returns:
             The components of the velocity vector at ``t`` in units of
             ``M_sun/day``.
 
         """
         return tuple(
-            tt.squeeze(x) for x in self._get_velocity(-self.m_star, t)
+            pt.squeeze(x) for x in self._get_velocity(-self.m_star, t)
         )
 
     def get_star_velocity(self, t):
         """Get the star's velocity vector
 
         .. note:: For a system with multiple planets, this will return one
             column per planet with the contributions from each planet. The
@@ -602,15 +604,15 @@
 
         Returns:
             The components of the velocity vector at ``t`` in units of
             ``M_sun/day``.
 
         """
         return tuple(
-            tt.squeeze(x) for x in self._get_velocity(self.m_planet, t)
+            pt.squeeze(x) for x in self._get_velocity(self.m_planet, t)
         )
 
     def get_relative_velocity(self, t):
         """The planets' velocity relative to the star
 
         .. note:: This treats each planet independently and does not take the
             other planets into account when computing the position of the
@@ -621,15 +623,15 @@
 
         Returns:
             The components of the velocity vector at ``t`` in units of
             ``R_sun/day``.
 
         """
         return tuple(
-            tt.squeeze(x) for x in self._get_velocity(-self.m_total, t)
+            pt.squeeze(x) for x in self._get_velocity(-self.m_total, t)
         )
 
     def get_radial_velocity(self, t, K=None, output_units=None):
         """Get the radial velocity of the star
 
         .. note:: The convention in exoplanet is that positive `z` points
             *towards* the observer. However, for consistency with radial
@@ -652,17 +654,17 @@
 
         """
 
         # Special case for K given: m_planet, incl, etc. is ignored
         if K is not None:
             sinf, cosf = self._get_true_anomaly(t)
             if self.ecc is None:
-                return tt.squeeze(K * cosf)
+                return pt.squeeze(K * cosf)
             # cos(w + f) + e * cos(w) from Lovis & Fischer
-            return tt.squeeze(
+            return pt.squeeze(
                 K
                 * (
                     self.cos_omega * cosf
                     - self.sin_omega * sinf
                     + self.ecc * self.cos_omega
                 )
             )
@@ -683,27 +685,27 @@
             factor = (
                 K**2 * (self.ecc * cosf + 1) ** 2 / (a * (self.ecc**2 - 1))
             )
         return self._rotate_vector(factor * cosf, factor * sinf)
 
     def get_planet_acceleration(self, t):
         return tuple(
-            tt.squeeze(x)
+            pt.squeeze(x)
             for x in self._get_acceleration(self.a_planet, -self.m_star, t)
         )
 
     def get_star_acceleration(self, t):
         return tuple(
-            tt.squeeze(x)
+            pt.squeeze(x)
             for x in self._get_acceleration(self.a_star, self.m_planet, t)
         )
 
     def get_relative_acceleration(self, t):
         return tuple(
-            tt.squeeze(x)
+            pt.squeeze(x)
             for x in self._get_acceleration(-self.a, -self.m_total, t)
         )
 
     def in_transit(self, t, r=0.0, texp=None, light_delay=False):
         """Get a list of timestamps that are in transit
 
         Args:
@@ -716,28 +718,28 @@
 
         """
         if light_delay:
             raise NotImplementedError(
                 "Light travel time delay not yet implemented for `in_transit`"
             )
 
-        z = tt.zeros_like(self.a)
+        z = pt.zeros_like(self.a)
         r = as_tensor_variable(r) + z
         R = self.r_star + z
 
         # Wrap the times into time since transit
         hp = 0.5 * self.period
-        dt = tt.mod(self._warp_times(t) + hp, self.period) - hp
+        dt = pt.mod(self._warp_times(t) + hp, self.period) - hp
 
         if self.ecc is None:
             # Equation 14 from Winn (2010)
             k = r / R
-            arg = tt.square(1 + k) - tt.square(self.b)
+            arg = pt.square(1 + k) - pt.square(self.b)
             factor = R / (self.a * self.sin_incl)
-            hdur = hp * tt.arcsin(factor * tt.sqrt(arg)) / np.pi
+            hdur = hp * pt.arcsin(factor * pt.sqrt(arg)) / np.pi
             t_start = -hdur
             t_end = hdur
             flag = z
 
         else:
             M_contact = ops.contact_points(
                 self.a,
@@ -747,33 +749,33 @@
                 self.cos_incl + z,
                 self.sin_incl + z,
                 R + r,
             )
             flag = M_contact[2]
 
             t_start = (M_contact[0] - self.M0) / self.n
-            t_start = tt.mod(t_start + hp, self.period) - hp
+            t_start = pt.mod(t_start + hp, self.period) - hp
             t_end = (M_contact[1] - self.M0) / self.n
-            t_end = tt.mod(t_end + hp, self.period) - hp
+            t_end = pt.mod(t_end + hp, self.period) - hp
 
-            t_start = tt.switch(
-                tt.gt(t_start, 0.0), t_start - self.period, t_start
+            t_start = pt.switch(
+                pt.gt(t_start, 0.0), t_start - self.period, t_start
             )
-            t_end = tt.switch(tt.lt(t_end, 0.0), t_end + self.period, t_end)
+            t_end = pt.switch(pt.lt(t_end, 0.0), t_end + self.period, t_end)
 
         if texp is not None:
             t_start -= 0.5 * texp
             t_end += 0.5 * texp
 
-        mask = tt.any(tt.and_(dt >= t_start, dt <= t_end), axis=-1)
+        mask = pt.any(pt.and_(dt >= t_start, dt <= t_end), axis=-1)
 
         result = ifelse(
-            tt.all(tt.eq(flag, 0)),
-            tt.arange(t.shape[0])[mask],
-            tt.arange(t.shape[0]),
+            pt.all(pt.eq(flag, 0)),
+            pt.arange(t.shape[0])[mask],
+            pt.arange(t.shape[0]),
         )
 
         return result
 
     def _flip(self, r_planet, model=None):
         if self.ecc is None:
             orbit = type(self)(
@@ -810,15 +812,15 @@
         e: The eccentricity. This should have the same shape as ``M``.
 
     Returns:
         The true anomaly of the orbit.
 
     """
     sinf, cosf = ops.kepler(M, e)
-    return tt.arctan2(sinf, cosf)
+    return pt.arctan2(sinf, cosf)
 
 
 def get_aor_from_transit_duration(duration, period, b, ror=None):
     """Get the semimajor axis implied by a circular orbit and duration
 
     Args:
         duration: The transit duration
@@ -832,17 +834,17 @@
 
     """
     if ror is None:
         ror = as_tensor_variable(0.0)
     b2 = b**2
     opk2 = (1 + ror) ** 2
     phi = np.pi * duration / period
-    sinp = tt.sin(phi)
-    cosp = tt.cos(phi)
-    num = tt.sqrt(opk2 - b2 * cosp**2)
+    sinp = pt.sin(phi)
+    cosp = pt.cos(phi)
+    num = pt.sqrt(opk2 - b2 * cosp**2)
     aor = num / sinp
     grad = np.pi * cosp * (b2 - opk2) / (num * period * sinp**2)
     return aor, grad
 
 
 def _get_consistent_inputs(a, period, rho_star, r_star, m_star, m_planet):
     if a is None and period is None:
@@ -852,19 +854,19 @@
 
     if m_planet is not None:
         m_planet = as_tensor_variable(to_unit(m_planet, u.M_sun))
 
     if a is not None:
         a = as_tensor_variable(to_unit(a, u.R_sun))
         if m_planet is None:
-            m_planet = tt.zeros_like(a)
+            m_planet = pt.zeros_like(a)
     if period is not None:
         period = as_tensor_variable(to_unit(period, u.day))
         if m_planet is None:
-            m_planet = tt.zeros_like(period)
+            m_planet = pt.zeros_like(period)
 
     # Compute the implied density if a and period are given
     implied_rho_star = False
     if a is not None and period is not None:
         if rho_star is not None or m_star is not None:
             raise ValueError(
                 "if both a and period are given, you can't "
@@ -922,11 +924,11 @@
     # Work out the planet parameters
     if a is None:
         a = (
             G_grav * (m_star + m_planet) * period**2 / (4 * np.pi**2)
         ) ** (1.0 / 3)
     elif period is None:
         period = (
-            2 * np.pi * a ** (3 / 2) / (tt.sqrt(G_grav * (m_star + m_planet)))
+            2 * np.pi * a ** (3 / 2) / (pt.sqrt(G_grav * (m_star + m_planet)))
         )
 
     return a, period, rho_star * gcc_per_sun, r_star, m_star, m_planet
```

### Comparing `exoplanet-0.5.3rc1/src/exoplanet/orbits/simple.py` & `exoplanet-0.6.0rc2/src/exoplanet/orbits/simple.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-# -*- coding: utf-8 -*-
-
 __all__ = ["SimpleTransitOrbit"]
 
-import aesara_theano_fallback.tensor as tt
 import numpy as np
 
-from ..utils import as_tensor_variable
+from exoplanet.compat import tensor as pt
+from exoplanet.utils import as_tensor_variable
 
 
 class SimpleTransitOrbit:
     """An orbit representing a set of planets transiting a common central
 
     This orbit is parameterized by the observables of a transiting system,
     period, phase, duration, and impact parameter.
@@ -34,15 +32,15 @@
         x2 = r_star**2 * ((1 + ror) ** 2 - b**2)
         self.speed = 2 * np.sqrt(x2) / duration
 
         self._half_period = 0.5 * self.period
         self._ref_time = self.t0 - self._half_period
 
     def get_star_position(self, t, light_delay=False):
-        nothing = tt.zeros_like(as_tensor_variable(t))
+        nothing = pt.zeros_like(as_tensor_variable(t))
         return nothing, nothing, nothing
 
     def get_planet_position(self, t, light_delay=False):
         return self.get_relative_position(t, light_delay=False)
 
     def get_relative_position(self, t, light_delay=False):
         """The planets' positions relative to the star
@@ -55,20 +53,20 @@
             ``R_sun``.
 
         """
         if light_delay:
             raise NotImplementedError(
                 "Light travel time delay is not implemented for simple orbits"
             )
-        dt = tt.mod(tt.shape_padright(t) - self._ref_time, self.period)
+        dt = pt.mod(pt.shape_padright(t) - self._ref_time, self.period)
         dt -= self._half_period
-        x = tt.squeeze(self.speed * dt)
-        y = tt.squeeze(self._b_norm + tt.zeros_like(dt))
-        m = tt.abs_(dt) < 0.5 * self.duration
-        z = tt.squeeze(m * 1.0 - (~m) * 1.0)
+        x = pt.squeeze(self.speed * dt)
+        y = pt.squeeze(self._b_norm + pt.zeros_like(dt))
+        m = pt.abs(dt) < 0.5 * self.duration
+        z = pt.squeeze(m * 1.0 - (~m) * 1.0)
         return x, y, z
 
     def get_planet_velocity(self, t):
         raise NotImplementedError("a SimpleTransitOrbit has no velocity")
 
     def get_star_velocity(self, t):
         raise NotImplementedError("a SimpleTransitOrbit has no velocity")
@@ -88,18 +86,18 @@
             The indices of the timestamps that are in transit.
 
         """
         if light_delay:
             raise NotImplementedError(
                 "Light travel time delay is not implemented for simple orbits"
             )
-        dt = tt.mod(tt.shape_padright(t) - self._ref_time, self.period)
+        dt = pt.mod(pt.shape_padright(t) - self._ref_time, self.period)
         dt -= self._half_period
         if r is None:
             tol = 0.5 * self.duration
         else:
             x = (r + self.r_star) ** 2 - self._b_norm**2
-            tol = tt.sqrt(x) / self.speed
+            tol = pt.sqrt(x) / self.speed
         if texp is not None:
             tol += 0.5 * texp
-        mask = tt.any(tt.abs_(dt) < tol, axis=-1)
-        return tt.arange(t.size)[mask]
+        mask = pt.any(pt.abs(dt) < tol, axis=-1)
+        return pt.arange(t.size)[mask]
```

### Comparing `exoplanet-0.5.3rc1/src/exoplanet/orbits/ttv.py` & `exoplanet-0.6.0rc2/src/exoplanet/orbits/ttv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-# -*- coding: utf-8 -*-
-
 __all__ = ["TTVOrbit", "compute_expected_transit_times"]
 
-import aesara_theano_fallback.tensor as tt
 import numpy as np
 
-from ..utils import as_tensor_variable
-from .keplerian import KeplerianOrbit
+from exoplanet.compat import tensor as pt
+from exoplanet.orbits.keplerian import KeplerianOrbit
+from exoplanet.utils import as_tensor_variable
 
 
 def compute_expected_transit_times(min_time, max_time, period, t0):
     """Compute the expected transit times within a dataset
 
     Args:
         min_time (float): The start time of the dataset
@@ -78,68 +76,68 @@
             raise ValueError(
                 "one of 'ttvs' or 'transit_times' must be " "defined"
             )
         if ttvs is not None:
             self.ttvs = [as_tensor_variable(ttv, ndim=1) for ttv in ttvs]
             if transit_inds is None:
                 self.transit_inds = [
-                    tt.arange(ttv.shape[0]) for ttv in self.ttvs
+                    pt.arange(ttv.shape[0]) for ttv in self.ttvs
                 ]
             else:
                 self.transit_inds = [
-                    tt.cast(as_tensor_variable(inds, ndim=1), "int64")
+                    pt.cast(as_tensor_variable(inds, ndim=1), "int64")
                     for inds in transit_inds
                 ]
 
         else:
             # If transit times are given, compute the least squares period and
             # t0 based on these times.
             self.transit_times = []
             self.ttvs = []
             self.transit_inds = []
             period = []
             t0 = []
             for i, times in enumerate(transit_times):
                 times = as_tensor_variable(times, ndim=1)
                 if transit_inds is None:
-                    inds = tt.arange(times.shape[0])
+                    inds = pt.arange(times.shape[0])
                 else:
-                    inds = tt.cast(
+                    inds = pt.cast(
                         as_tensor_variable(transit_inds[i]), "int64"
                     )
                 self.transit_inds.append(inds)
 
                 # A convoluted version of linear regression; don't ask
                 N = times.shape[0]
-                sumx = tt.sum(inds)
-                sumx2 = tt.sum(inds**2)
-                sumy = tt.sum(times)
-                sumxy = tt.sum(inds * times)
+                sumx = pt.sum(inds)
+                sumx2 = pt.sum(inds**2)
+                sumy = pt.sum(times)
+                sumxy = pt.sum(inds * times)
                 denom = N * sumx2 - sumx**2
                 slope = (N * sumxy - sumx * sumy) / denom
                 intercept = (sumx2 * sumy - sumx * sumxy) / denom
                 expect = intercept + inds * slope
 
                 period.append(slope)
                 t0.append(intercept)
                 self.ttvs.append(times - expect)
                 self.transit_times.append(times)
 
-            kwargs["t0"] = tt.stack(t0)
+            kwargs["t0"] = pt.stack(t0)
 
             # We'll have two different periods: one that is the mean difference
             # between transit times and one that is a parameter that sets the
             # transit shape. If a "period" parameter is not given, these will
             # be the same. Users will probably want to put a prior relating the
             # two periods if they use separate values.
-            self.ttv_period = tt.stack(period)
+            self.ttv_period = pt.stack(period)
             if "period" not in kwargs:
                 if "delta_log_period" in kwargs:
-                    kwargs["period"] = tt.exp(
-                        tt.log(self.ttv_period)
+                    kwargs["period"] = pt.exp(
+                        pt.log(self.ttv_period)
                         + kwargs.pop("delta_log_period")
                     )
                 else:
                     kwargs["period"] = self.ttv_period
 
         super(TTVOrbit, self).__init__(*args, **kwargs)
 
@@ -149,41 +147,41 @@
                 self.t0[i] + self.period[i] * self.transit_inds[i] + ttv
                 for i, ttv in enumerate(self.ttvs)
             ]
 
         # Compute the full set of transit times
         self.all_transit_times = []
         for i, inds in enumerate(self.transit_inds):
-            expect = self.t0[i] + self.period[i] * tt.arange(inds.max() + 1)
+            expect = self.t0[i] + self.period[i] * pt.arange(inds.max() + 1)
             self.all_transit_times.append(
-                tt.set_subtensor(expect[inds], self.transit_times[i])
+                pt.set_subtensor(expect[inds], self.transit_times[i])
             )
 
         # Set up a histogram for identifying the transit offsets
         self._bin_edges = [
-            tt.concatenate(
+            pt.concatenate(
                 (
                     [tts[0] - 0.5 * self.ttv_period[i]],
                     0.5 * (tts[1:] + tts[:-1]),
                     [tts[-1] + 0.5 * self.ttv_period[i]],
                 )
             )
             for i, tts in enumerate(self.all_transit_times)
         ]
         self._bin_values = [
-            tt.concatenate(([tts[0]], tts, [tts[-1]]))
+            pt.concatenate(([tts[0]], tts, [tts[-1]]))
             for i, tts in enumerate(self.all_transit_times)
         ]
 
     def _get_model_dt(self, t):
         vals = []
         for i in range(len(self.ttvs)):
-            inds = tt.extra_ops.searchsorted(self._bin_edges[i], t)
+            inds = pt.extra_ops.searchsorted(self._bin_edges[i], t)
             vals.append(self._bin_values[i][inds])
-        return tt.stack(vals, -1)
+        return pt.stack(vals, -1)
 
     def _warp_times(self, t, _pad=True):
         # This is the key function that takes the TTVs into account by
         # stretching the time axis around each transit
         if _pad:
-            return tt.shape_padright(t) - self._get_model_dt(t)
+            return pt.shape_padright(t) - self._get_model_dt(t)
         return t - self._get_model_dt(t)
```

### Comparing `exoplanet-0.5.3rc1/src/exoplanet/units.py` & `exoplanet-0.6.0rc2/src/exoplanet/units.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-# -*- coding: utf-8 -*-
-
 __all__ = ["with_unit", "has_unit", "to_unit"]
 
-from .utils import as_tensor_variable
+from exoplanet.utils import as_tensor_variable
 
 UNIT_ATTR_NAME = "__exoplanet_unit__"
 
 
 def with_unit(obj, unit):
-    """Decorate a Theano tensor with Astropy units
+    """Decorate an PyTensor tensor with Astropy units
 
     Args:
-        obj: The Theano tensor
+        obj: The PyTensor tensor
         unit (astropy.Unit): The units for this object
 
     Raises:
         TypeError: If the tensor already has units
 
     """
     if hasattr(obj, UNIT_ATTR_NAME):
@@ -27,21 +25,21 @@
 
 def has_unit(obj):
     """Does an object have units as defined by exoplanet?"""
     return hasattr(obj, UNIT_ATTR_NAME)
 
 
 def to_unit(obj, target):
-    """Convert a Theano tensor with units to a target set of units
+    """Convert an PyTensor tensor with units to a target set of units
 
     Args:
-        obj: The Theano tensor
+        obj: The PyTensor tensor
         target (astropy.Unit): The target units
 
     Returns:
-        A Theano tensor in the right units
+        A PyTensor tensor in the right units
 
     """
     if not has_unit(obj):
         return obj
     base = getattr(obj, UNIT_ATTR_NAME)
     return obj * base.to(target)
```

### Comparing `exoplanet-0.5.3rc1/src/exoplanet/utils.py` & `exoplanet-0.6.0rc2/src/exoplanet/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-# -*- coding: utf-8 -*-
-
 __all__ = [
     "logger",
     "as_tensor_variable",
     "deprecation_warning",
     "deprecated",
     "docs_setup",
 ]
 
 import logging
 import warnings
 from functools import wraps
 
-from aesara_theano_fallback import aesara as theano
+from exoplanet.compat import tensor
 
 logger = logging.getLogger("exoplanet")
 
 
 def as_tensor_variable(x, dtype="float64", **kwargs):
-    t = theano.tensor.as_tensor_variable(x, **kwargs)
+    t = tensor.as_tensor_variable(x, **kwargs)
     if dtype is None:
         return t
     return t.astype(dtype)
 
 
 def deprecation_warning(msg):
     warnings.warn(msg, category=DeprecationWarning, stacklevel=2)
@@ -43,28 +41,24 @@
 
     return wrapper
 
 
 def docs_setup():
     """Set some environment variables and ignore some warnings for the docs"""
     import logging
-    import warnings
 
     import matplotlib.pyplot as plt
 
-    # Remove when Theano is updated
-    warnings.filterwarnings("ignore", category=DeprecationWarning)
-    warnings.filterwarnings("ignore", category=FutureWarning)
-
-    # Remove when arviz is updated
-    warnings.filterwarnings("ignore", category=UserWarning)
-
     logger = logging.getLogger("theano.gof.compilelock")
     logger.setLevel(logging.ERROR)
-    logger = logging.getLogger("theano.tensor.opt")
+    logger = logging.getLogger("pytensor.tensor.rewriting")
+    logger.setLevel(logging.ERROR)
+    logger = logging.getLogger("pytensor.tensor.blas")
+    logger.setLevel(logging.ERROR)
+    logger = logging.getLogger("matplotlib.font_manager")
     logger.setLevel(logging.ERROR)
     logger = logging.getLogger("exoplanet")
     logger.setLevel(logging.DEBUG)
 
     plt.style.use("default")
     plt.rcParams["savefig.dpi"] = 100
     plt.rcParams["figure.dpi"] = 100
```

### Comparing `exoplanet-0.5.3rc1/src/exoplanet.egg-info/SOURCES.txt` & `exoplanet-0.6.0rc2/src/exoplanet.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-.clang-format
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
+.readthedocs.yaml
 CITATION.cff
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.md
+noxfile.py
 pyproject.toml
 pytest.ini
 readthedocs.yml
 setup.py
 tox.ini
 .github/dependabot.yml
 .github/ISSUE_TEMPLATE/bug_report.md
@@ -21,71 +22,68 @@
 .github/workflows/tests.yml
 binder/requirements.txt
 binder/runtime.txt
 docs/.gitignore
 docs/Makefile
 docs/changes.rst
 docs/conf.py
-docs/environment.yml
 docs/index.rst
 docs/_static/big_logo.png
 docs/_static/exoplanet.css
 docs/_static/favicon.png
 docs/_static/logo.png
 docs/_static/logo_shadow.png
 docs/_static/orbit3D.png
 docs/tutorials/about.md
 docs/tutorials/autodiff.md
 docs/tutorials/citation.md
 docs/tutorials/data-and-models.md
+docs/tutorials/intro-to-pymc.md
 docs/tutorials/intro-to-pymc3.md
 docs/tutorials/ipython_kernel_config.py
 docs/tutorials/light-delay.md
 docs/tutorials/reparameterization.md
 docs/user/api.rst
 docs/user/dev.rst
 docs/user/install.rst
 docs/user/multiprocessing.rst
-docs/user/theano.rst
 joss/metadata.yaml
 joss/paper.bib
 joss/paper.md
 joss/figures/figure.png
 joss/figures/joss-logo.png
 src/exoplanet/__init__.py
 src/exoplanet/citations.py
+src/exoplanet/compat.py
 src/exoplanet/estimators.py
 src/exoplanet/exoplanet_version.py
 src/exoplanet/interp.py
 src/exoplanet/units.py
 src/exoplanet/utils.py
 src/exoplanet.egg-info/PKG-INFO
 src/exoplanet.egg-info/SOURCES.txt
 src/exoplanet.egg-info/dependency_links.txt
 src/exoplanet.egg-info/not-zip-safe
 src/exoplanet.egg-info/requires.txt
 src/exoplanet.egg-info/top_level.txt
 src/exoplanet/distributions/__init__.py
+src/exoplanet/distributions/distributions.py
 src/exoplanet/distributions/eccentricity.py
-src/exoplanet/distributions/physical.py
-src/exoplanet/distributions/transforms.py
 src/exoplanet/light_curves/__init__.py
 src/exoplanet/light_curves/interpolated.py
 src/exoplanet/light_curves/limb_dark.py
 src/exoplanet/light_curves/secondary_eclipse.py
 src/exoplanet/orbits/__init__.py
 src/exoplanet/orbits/constants.py
 src/exoplanet/orbits/dur_to_ecc.py
 src/exoplanet/orbits/keplerian.py
 src/exoplanet/orbits/simple.py
 src/exoplanet/orbits/ttv.py
 tests/citations_test.py
-tests/conftest.py
 tests/distributions_test.py
 tests/estimators_test.py
 tests/interp_test.py
 tests/light_curves_test.py
 tests/units_test.py
-tests/orbits/conftest.py
 tests/orbits/keplerian_test.py
 tests/orbits/simple_test.py
 tests/orbits/ttv_test.py
```

### Comparing `exoplanet-0.5.3rc1/tests/citations_test.py` & `exoplanet-0.6.0rc2/tests/citations_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-# -*- coding: utf-8 -*-
-
 __all__ = ["test_basic"]
 
-import pymc3 as pm
-
 from exoplanet.citations import CITATIONS, get_citations_for_model
+from exoplanet.compat import pm
 from exoplanet.light_curves import LimbDarkLightCurve
 
 
 def test_basic():
     with pm.Model() as model:
         txt, bib = get_citations_for_model()
     assert txt == ""
     assert bib == ""
 
     with pm.Model() as model:
         LimbDarkLightCurve(0.5, 0.2)
         txt, bib = get_citations_for_model()
-    for k in ["exoplanet", "theano", "pymc3", "starry"]:
+    for k in ["exoplanet", "starry"]:
         assert all(v in bib for v in CITATIONS[k][0])
         assert CITATIONS[k][1] in bib
 
     txt1, bib1 = get_citations_for_model(model=model)
     assert txt == txt1
     assert bib == bib1
```

### Comparing `exoplanet-0.5.3rc1/tests/estimators_test.py` & `exoplanet-0.6.0rc2/tests/estimators_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 import astropy.units as u
 import numpy as np
 
 from exoplanet.estimators import (
     autocorr_estimator,
     bls_estimator,
     estimate_minimum_mass,
```

### Comparing `exoplanet-0.5.3rc1/tests/interp_test.py` & `exoplanet-0.6.0rc2/tests/interp_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 import numpy as np
 from scipy.interpolate import (
     RegularGridInterpolator as SpRegularGridInterpolator,
 )
 
 from exoplanet.interp import RegularGridInterpolator
```

### Comparing `exoplanet-0.5.3rc1/tests/light_curves_test.py` & `exoplanet-0.6.0rc2/tests/light_curves_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-# -*- coding: utf-8 -*-
-
 import logging
 
-import aesara_theano_fallback.tensor as tt
 import numpy as np
 import pytest
-from aesara_theano_fallback import aesara as theano
-from packaging import version
 
+from exoplanet.compat import change_flags, function, grad
+from exoplanet.compat import tensor as pt
+from exoplanet.compat import verify_grad
 from exoplanet.light_curves import (
     LimbDarkLightCurve,
     SecondaryEclipseLightCurve,
 )
 from exoplanet.orbits import KeplerianOrbit
 
 try:
@@ -24,19 +22,20 @@
 def test_light_curve():
     u_val = np.array([0.2, 0.3])
     b_val = np.linspace(-1.5, 1.5, 100)
     r_val = 0.1 + np.zeros_like(b_val)
     lc = LimbDarkLightCurve(u_val[0], u_val[1])
     evaluated = lc._compute_light_curve(b_val, r_val).eval()
 
-    if version.parse(starry.__version__) < version.parse("0.9.9"):
-        m = starry.Map(lmax=len(u_val))
-        m[:] = u_val
-        expect = m.flux(xo=b_val, ro=r_val) - 1
-    else:
+    # Currently, if we're testing with starry theano _will_ be installed; no
+    # need for a compatibility layer
+    import theano
+
+    flags = theano.config.gcc__cxxflags
+    with change_flags(gcc__cxxflags=flags + " -fexceptions"):
         m = starry.Map(udeg=len(u_val))
         m[1:] = u_val
         expect = m.flux(xo=b_val, ro=r_val[0]).eval() - 1
 
     assert np.allclose(expect, evaluated)
 
 
@@ -45,40 +44,36 @@
     b_val = np.linspace(-1.5, 1.5, 20)
     r_val = 0.1 + np.zeros_like(b_val)
 
     lc = lambda u, b, r: LimbDarkLightCurve(  # NOQA
         u[0], u[1]
     )._compute_light_curve(b, r)
 
-    with theano.configparser.change_flags(compute_test_value="off"):
+    with change_flags(compute_test_value="off"):
         with caplog.at_level(logging.DEBUG, logger="theano.gof.cmodule"):
-            theano.gradient.verify_grad(
-                lc, [u_val, b_val, r_val], rng=np.random
-            )
+            verify_grad(lc, [u_val, b_val, r_val], rng=np.random)
 
 
 def test_vector_params():
-    u = tt.vector()
+    u = pt.vector()
     u.tag.test_value = u_val = np.array([0.3, 0.2])
     b = np.linspace(-1.5, 1.5, 20)
     r = 0.1 + np.zeros_like(b)
 
     with pytest.warns(DeprecationWarning, match=r"vector of limb darkening"):
-        lc1 = theano.function(
-            [u], LimbDarkLightCurve(u)._compute_light_curve(b, r)
-        )(u_val)
-    lc2 = theano.function(
+        lc1 = function([u], LimbDarkLightCurve(u)._compute_light_curve(b, r))(
+            u_val
+        )
+    lc2 = function(
         [u], LimbDarkLightCurve(u[0], u[1])._compute_light_curve(b, r)
     )(u_val)
     np.testing.assert_allclose(lc1, lc2)
 
     with pytest.raises(AssertionError):
-        theano.function(
-            [], LimbDarkLightCurve([0.3])._compute_light_curve(b, r)
-        )()
+        function([], LimbDarkLightCurve([0.3])._compute_light_curve(b, r))()
 
 
 def test_in_transit():
     t = np.linspace(-20, 20, 1000)
     m_planet = np.array([0.3, 0.5])
     m_star = 1.45
     orbit = KeplerianOrbit(
@@ -92,22 +87,22 @@
     )
     u = np.array([0.2, 0.3])
     r = np.array([0.1, 0.01])
 
     lc = LimbDarkLightCurve(u[0], u[1])
     model1 = lc.get_light_curve(r=r, orbit=orbit, t=t)
     model2 = lc.get_light_curve(r=r, orbit=orbit, t=t, use_in_transit=False)
-    vals = theano.function([], [model1, model2])()
+    vals = function([], [model1, model2])()
     assert np.allclose(*vals)
 
     model1 = lc.get_light_curve(r=r, orbit=orbit, t=t, texp=0.1)
     model2 = lc.get_light_curve(
         r=r, orbit=orbit, t=t, texp=0.1, use_in_transit=False
     )
-    vals = theano.function([], [model1, model2])()
+    vals = function([], [model1, model2])()
     assert np.allclose(*vals)
 
 
 def test_variable_texp():
     t = np.linspace(-20, 20, 1000)
     m_planet = np.array([0.3, 0.5])
     m_star = 1.45
@@ -131,26 +126,26 @@
     model2 = lc.get_light_curve(
         r=r,
         orbit=orbit,
         t=t,
         use_in_transit=False,
         texp=texp0 + np.zeros_like(t),
     )
-    vals = theano.function([], [model1, model2])()
+    vals = function([], [model1, model2])()
     assert np.allclose(*vals)
 
     model1 = lc.get_light_curve(r=r, orbit=orbit, t=t, texp=texp0)
     model2 = lc.get_light_curve(
         r=r,
         orbit=orbit,
         t=t,
         texp=texp0 + np.zeros_like(t),
         use_in_transit=False,
     )
-    vals = theano.function([], [model1, model2])()
+    vals = function([], [model1, model2])()
     assert np.allclose(*vals)
 
 
 def test_contact_bug():
     orbit = KeplerianOrbit(period=3.456, ecc=0.6, omega=-1.5)
     t = np.linspace(-0.1, 0.1, 1000)
     u = [0.3, 0.2]
@@ -199,15 +194,15 @@
     a = orbit.a.eval()
     incl = orbit.incl.eval()
 
     lc = LimbDarkLightCurve(u_star[0], u_star[1])
 
     model1 = lc.get_light_curve(r=r_pl, orbit=orbit, t=t)
     model2 = lc.get_light_curve(r=r_pl, orbit=orbit, t=t, use_in_transit=False)
-    vals = theano.function([], [model1, model2])()
+    vals = function([], [model1, model2])()
     assert np.allclose(*vals)
 
     params = TransitParams()
     params.t0 = t0
     params.per = period
     params.rp = r
     params.a = a / r_star
@@ -220,21 +215,21 @@
     model = TransitModel(params, t)
     flux = model.light_curve(params)
     assert np.allclose(vals[0][:, 0], flux - 1)
 
 
 def test_singular_points():
     u = np.array([0.2, 0.3])
-    b = tt.vector()
+    b = pt.vector()
     b.tag.test_value = np.array([0.5])
-    r = tt.vector()
+    r = pt.vector()
     r.tag.test_value = np.array([0.1])
     lc = LimbDarkLightCurve(u[0], u[1])
     f = lc._compute_light_curve(b, r)
-    func = theano.function([b, r], f)
+    func = function([b, r], f)
 
     def compare(b_val, r_val, b_eps, r_eps):
         """
         Compare the flux at a singular point
         to the flux at neighboring points.
 
         """
@@ -277,18 +272,18 @@
     lc = LimbDarkLightCurve(u[0], u[1])
 
     for b, delta in [
         (np.float64(0.5), np.float64(0.01)),
         (np.array([0.1, 0.9]), np.array([0.1, 0.5])),
         (np.array([0.1, 0.9, 0.3]), np.array([0.1, 0.5, 0.0234])),
     ]:
-        dv = tt.as_tensor_variable(delta)
+        dv = pt.as_tensor_variable(delta)
         ror, jac = lc.get_ror_from_approx_transit_depth(dv, b, jac=True)
         _check_quad(u, b, delta, ror.eval())
-        assert np.allclose(theano.grad(tt.sum(ror), dv).eval(), jac.eval())
+        assert np.allclose(grad(pt.sum(ror), dv).eval(), jac.eval())
 
 
 def test_secondary_eclipse():
     u1 = np.array([0.3, 0.2])
     lc1 = LimbDarkLightCurve(u1[0], u1[1])
 
     u2 = np.array([0.4, 0.1])
```

### Comparing `exoplanet-0.5.3rc1/tests/orbits/keplerian_test.py` & `exoplanet-0.6.0rc2/tests/orbits/keplerian_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-# -*- coding: utf-8 -*-
-
-import aesara_theano_fallback.tensor as tt
 import astropy.units as u
 import numpy as np
 import pytest
-from aesara_theano_fallback import aesara as theano
 from astropy.constants import c
 from scipy.optimize import minimize
 
+from exoplanet.compat import change_flags, function, grad
+from exoplanet.compat import tensor as pt
 from exoplanet.orbits.keplerian import (
     KeplerianOrbit,
     _get_consistent_inputs,
     get_aor_from_transit_duration,
 )
 from exoplanet.units import with_unit
 
@@ -40,15 +38,15 @@
         )
     m = r_batman < 100.0
     assert m.sum() > 0
 
     orbit = KeplerianOrbit(
         period=period, a=a, t0=t0, ecc=e, omega=omega, incl=incl
     )
-    func = theano.function([], orbit.get_relative_position(t))
+    func = function([], orbit.get_relative_position(t))
     x, y, z = func()
     r = np.sqrt(x**2 + y**2)
 
     # Make sure that the in-transit impact parameter matches batman
     assert np.allclose(r_batman[m], r[m], atol=2e-5)
 
     # In-transit should correspond to positive z in our parameterization
@@ -72,68 +70,69 @@
         ecc=np.array([0.1, 0.8]),
         omega=np.array([0.5, 1.3]),
         Omega=np.array([0.0, 1.0]),
         incl=np.array([0.25 * np.pi, 0.3 * np.pi]),
         m_planet=m_planet,
     )
 
-    planet_coords = theano.function([], orbit.get_planet_position(t))()
-    star_coords = theano.function([], orbit.get_star_position(t))()
+    planet_coords = function([], orbit.get_planet_position(t))()
+    star_coords = function([], orbit.get_star_position(t))()
 
     com = np.sum(
         (
             m_planet[None, :] * np.array(planet_coords)
             + m_star * np.array(star_coords)
         )
         / (m_star + m_planet)[None, :],
         axis=0,
     )
     assert np.allclose(com, 0.0)
 
 
 def test_velocity():
-    t_tensor = tt.dvector()
-    t = np.linspace(0, 100, 1000)
-    m_planet = 0.1
-    m_star = 1.3
-    orbit = KeplerianOrbit(
-        m_star=m_star,
-        r_star=1.0,
-        t0=0.5,
-        period=100.0,
-        ecc=0.1,
-        omega=0.5,
-        Omega=1.0,
-        incl=0.25 * np.pi,
-        m_planet=m_planet,
-    )
+    with change_flags(compute_test_value="off"):
+        t_tensor = pt.dvector()
+        t = np.linspace(0, 100, 1000)
+        m_planet = 0.1
+        m_star = 1.3
+        orbit = KeplerianOrbit(
+            m_star=m_star,
+            r_star=1.0,
+            t0=0.5,
+            period=100.0,
+            ecc=0.1,
+            omega=0.5,
+            Omega=1.0,
+            incl=0.25 * np.pi,
+            m_planet=m_planet,
+        )
 
-    star_pos = orbit.get_star_position(t_tensor)
-    star_vel = theano.function([], orbit.get_star_velocity(t))()
-    star_vel_expect = np.empty_like(star_vel)
-    for i in range(3):
-        g = theano.grad(tt.sum(star_pos[i]), t_tensor)
-        star_vel_expect[i] = theano.function([t_tensor], g)(t)
-    assert np.allclose(star_vel, star_vel_expect)
-
-    planet_pos = orbit.get_planet_position(t_tensor)
-    planet_vel = theano.function([], orbit.get_planet_velocity(t))()
-    planet_vel_expect = np.empty_like(planet_vel)
-    for i in range(3):
-        g = theano.grad(tt.sum(planet_pos[i]), t_tensor)
-        planet_vel_expect[i] = theano.function([t_tensor], g)(t)
-    assert np.allclose(planet_vel, planet_vel_expect)
-
-    pos = orbit.get_relative_position(t_tensor)
-    vel = np.array(theano.function([], orbit.get_relative_velocity(t))())
-    vel_expect = np.empty_like(vel)
-    for i in range(3):
-        g = theano.grad(tt.sum(pos[i]), t_tensor)
-        vel_expect[i] = theano.function([t_tensor], g)(t)
-    assert np.allclose(vel, vel_expect)
+        star_pos = orbit.get_star_position(t_tensor)
+        star_vel = function([], orbit.get_star_velocity(t))()
+        star_vel_expect = np.empty_like(star_vel)
+        for i in range(3):
+            g = grad(pt.sum(star_pos[i]), t_tensor)
+            star_vel_expect[i] = function([t_tensor], g)(t)
+        assert np.allclose(star_vel, star_vel_expect)
+
+        planet_pos = orbit.get_planet_position(t_tensor)
+        planet_vel = function([], orbit.get_planet_velocity(t))()
+        planet_vel_expect = np.empty_like(planet_vel)
+        for i in range(3):
+            g = grad(pt.sum(planet_pos[i]), t_tensor)
+            planet_vel_expect[i] = function([t_tensor], g)(t)
+        assert np.allclose(planet_vel, planet_vel_expect)
+
+        pos = orbit.get_relative_position(t_tensor)
+        vel = np.array(function([], orbit.get_relative_velocity(t))())
+        vel_expect = np.empty_like(vel)
+        for i in range(3):
+            g = grad(pt.sum(pos[i]), t_tensor)
+            vel_expect[i] = function([t_tensor], g)(t)
+        assert np.allclose(vel, vel_expect)
 
 
 def test_radial_velocity():
     t = np.linspace(0, 100, 1000)
     m_planet = 0.1
     m_star = 1.3
     orbit = KeplerianOrbit(
@@ -152,52 +151,53 @@
     rv2 = orbit.get_radial_velocity(
         t, K=orbit.K0 * orbit.m_planet * orbit.sin_incl
     ).eval()
     assert np.allclose(rv1, rv2)
 
 
 def test_acceleration():
-    t_tensor = tt.dvector()
-    t = np.linspace(0, 100, 1000)
-    m_planet = 0.1
-    m_star = 1.3
-    orbit = KeplerianOrbit(
-        m_star=m_star,
-        r_star=1.0,
-        t0=0.5,
-        period=100.0,
-        ecc=0.1,
-        omega=0.5,
-        incl=0.25 * np.pi,
-        m_planet=m_planet,
-    )
+    with change_flags(compute_test_value="off"):
+        t_tensor = pt.dvector()
+        t = np.linspace(0, 100, 1000)
+        m_planet = 0.1
+        m_star = 1.3
+        orbit = KeplerianOrbit(
+            m_star=m_star,
+            r_star=1.0,
+            t0=0.5,
+            period=100.0,
+            ecc=0.1,
+            omega=0.5,
+            incl=0.25 * np.pi,
+            m_planet=m_planet,
+        )
 
-    star_vel = orbit.get_star_velocity(t_tensor)
-    star_acc = theano.function([], orbit.get_star_acceleration(t))()
-    star_acc_expect = np.empty_like(star_acc)
-    for i in range(3):
-        g = theano.grad(tt.sum(star_vel[i]), t_tensor)
-        star_acc_expect[i] = theano.function([t_tensor], g)(t)
-    assert np.allclose(star_acc, star_acc_expect)
-
-    planet_vel = orbit.get_planet_velocity(t_tensor)
-    planet_acc = theano.function([], orbit.get_planet_acceleration(t))()
-    planet_acc_expect = np.empty_like(planet_acc)
-    for i in range(3):
-        g = theano.grad(tt.sum(planet_vel[i]), t_tensor)
-        planet_acc_expect[i] = theano.function([t_tensor], g)(t)
-    assert np.allclose(planet_acc, planet_acc_expect)
-
-    vel = orbit.get_relative_velocity(t_tensor)
-    acc = theano.function([], orbit.get_relative_acceleration(t))()
-    acc_expect = np.empty_like(acc)
-    for i in range(3):
-        g = theano.grad(tt.sum(vel[i]), t_tensor)
-        acc_expect[i] = theano.function([t_tensor], g)(t)
-    assert np.allclose(acc, acc_expect)
+        star_vel = orbit.get_star_velocity(t_tensor)
+        star_acc = function([], orbit.get_star_acceleration(t))()
+        star_acc_expect = np.empty_like(star_acc)
+        for i in range(3):
+            g = grad(pt.sum(star_vel[i]), t_tensor)
+            star_acc_expect[i] = function([t_tensor], g)(t)
+        assert np.allclose(star_acc, star_acc_expect)
+
+        planet_vel = orbit.get_planet_velocity(t_tensor)
+        planet_acc = function([], orbit.get_planet_acceleration(t))()
+        planet_acc_expect = np.empty_like(planet_acc)
+        for i in range(3):
+            g = grad(pt.sum(planet_vel[i]), t_tensor)
+            planet_acc_expect[i] = function([t_tensor], g)(t)
+        assert np.allclose(planet_acc, planet_acc_expect)
+
+        vel = orbit.get_relative_velocity(t_tensor)
+        acc = function([], orbit.get_relative_acceleration(t))()
+        acc_expect = np.empty_like(acc)
+        for i in range(3):
+            g = grad(pt.sum(vel[i]), t_tensor)
+            acc_expect[i] = function([t_tensor], g)(t)
+        assert np.allclose(acc, acc_expect)
 
 
 def test_flip():
     t = np.linspace(0, 100, 1000)
     m_planet = 0.1
     m_star = 1.3
     orbit1 = KeplerianOrbit(
@@ -209,22 +209,22 @@
         omega=0.5,
         Omega=1.0,
         incl=0.25 * np.pi,
         m_planet=m_planet,
     )
     orbit2 = orbit1._flip(0.7)
 
-    x1, y1, z1 = theano.function([], orbit1.get_star_position(t))()
-    x2, y2, z2 = theano.function([], orbit2.get_planet_position(t))()
+    x1, y1, z1 = function([], orbit1.get_star_position(t))()
+    x2, y2, z2 = function([], orbit2.get_planet_position(t))()
     assert np.allclose(x1, x2, atol=1e-5)
     assert np.allclose(y1, y2, atol=1e-5)
     assert np.allclose(z1, z2, atol=1e-5)
 
-    x1, y1, z1 = theano.function([], orbit1.get_planet_position(t))()
-    x2, y2, z2 = theano.function([], orbit2.get_star_position(t))()
+    x1, y1, z1 = function([], orbit1.get_planet_position(t))()
+    x2, y2, z2 = function([], orbit2.get_star_position(t))()
     assert np.allclose(x1, x2, atol=1e-5)
     assert np.allclose(y1, y2, atol=1e-5)
     assert np.allclose(z1, z2, atol=1e-5)
 
 
 def test_flip_circular():
     t = np.linspace(0, 100, 1000)
@@ -237,22 +237,22 @@
         period=100.0,
         Omega=1.0,
         incl=0.25 * np.pi,
         m_planet=m_planet,
     )
     orbit2 = orbit1._flip(0.7)
 
-    x1, y1, z1 = theano.function([], orbit1.get_star_position(t))()
-    x2, y2, z2 = theano.function([], orbit2.get_planet_position(t))()
+    x1, y1, z1 = function([], orbit1.get_star_position(t))()
+    x2, y2, z2 = function([], orbit2.get_planet_position(t))()
     assert np.allclose(x1, x2, atol=1e-5)
     assert np.allclose(y1, y2, atol=1e-5)
     assert np.allclose(z1, z2, atol=1e-5)
 
-    x1, y1, z1 = theano.function([], orbit1.get_planet_position(t))()
-    x2, y2, z2 = theano.function([], orbit2.get_star_position(t))()
+    x1, y1, z1 = function([], orbit1.get_planet_position(t))()
+    x2, y2, z2 = function([], orbit2.get_star_position(t))()
     assert np.allclose(x1, x2, atol=1e-5)
     assert np.allclose(y1, y2, atol=1e-5)
     assert np.allclose(z1, z2, atol=1e-5)
 
 
 def test_in_transit():
     t = np.linspace(-20, 20, 1000)
@@ -267,17 +267,17 @@
         ecc=np.array([0.1, 0.8]),
         omega=np.array([0.5, 1.3]),
         Omega=np.array([0.0, 1.0]),
         m_planet=m_planet,
     )
 
     r_pl = np.array([0.1, 0.03])
-    coords = theano.function([], orbit.get_relative_position(t))()
+    coords = function([], orbit.get_relative_position(t))()
     r2 = coords[0] ** 2 + coords[1] ** 2
-    inds = theano.function([], orbit.in_transit(t, r=r_pl))()
+    inds = function([], orbit.in_transit(t, r=r_pl))()
 
     m = np.isin(np.arange(len(t)), inds)
     in_ = r2[inds] <= ((r_star + r_pl) ** 2)[None, :]
     in_ &= coords[2][inds] > 0
     assert np.all(np.any(in_, axis=1))
 
     out = r2[~m] > ((r_star + r_pl) ** 2)[None, :]
@@ -304,16 +304,16 @@
         r_star=r_star,
         t0=np.array([0.5, 17.4]),
         period=np.array([10.0, 5.3]),
         m_planet=m_planet,
     )
 
     r_pl = np.array([0.1, 0.03])
-    inds = theano.function([], orbit.in_transit(t, r=r_pl))()
-    inds_circ = theano.function([], orbit_circ.in_transit(t, r=r_pl))()
+    inds = function([], orbit.in_transit(t, r=r_pl))()
+    inds_circ = function([], orbit_circ.in_transit(t, r=r_pl))()
     assert np.all(inds == inds_circ)
 
 
 def test_small_star():
     _rsky = pytest.importorskip("batman._rsky")
 
     m_star = 0.151
@@ -337,15 +337,15 @@
     a = orbit.a.eval()
     incl = orbit.incl.eval()
 
     r_batman = _rsky._rsky(t, t0, period, a, incl, ecc, omega, 1, 1)
     m = r_batman < 100.0
     assert m.sum() > 0
 
-    func = theano.function([], orbit.get_relative_position(t))
+    func = function([], orbit.get_relative_position(t))
     x, y, z = func()
     r = np.sqrt(x**2 + y**2)
 
     # Make sure that the in-transit impact parameter matches batman
     assert np.allclose(r_batman[m], r[m], atol=2e-5)
 
 
@@ -365,15 +365,15 @@
         t0=t0,
         b=b,
         ecc=ecc,
         omega=omega,
     )
     coords = orbit.get_relative_position(t0)
     assert np.allclose(
-        (tt.sqrt(coords[0] ** 2 + coords[1] ** 2) / r_star).eval(), b
+        (pt.sqrt(coords[0] ** 2 + coords[1] ** 2) / r_star).eval(), b
     )
     assert coords[2].eval() > 0
 
 
 def test_consistent_coords():
     import astropy.constants as c
     import astropy.units as u
@@ -498,75 +498,76 @@
         _get_consistent_inputs(a3, period3, None, r_star3, m_star3, None)
 
     with pytest.raises(ValueError):
         _get_consistent_inputs(a3, None, rho_star3, r_star3, m_star3, None)
 
 
 def test_light_delay():
-    # Instantiate the orbit
-    m_star = tt.scalar()
-    period = tt.scalar()
-    ecc = tt.scalar()
-    omega = tt.scalar()
-    Omega = tt.scalar()
-    incl = tt.scalar()
-    m_planet = tt.scalar()
-    t = tt.scalar()
-    orbit = KeplerianOrbit(
-        m_star=m_star,
-        r_star=1.0,
-        t0=0.0,
-        period=period,
-        ecc=ecc,
-        omega=omega,
-        Omega=Omega,
-        incl=incl,
-        m_planet=m_planet,
-    )
+    with change_flags(compute_test_value="off"):
+        # Instantiate the orbit
+        m_star = pt.scalar()
+        period = pt.scalar()
+        ecc = pt.scalar()
+        omega = pt.scalar()
+        Omega = pt.scalar()
+        incl = pt.scalar()
+        m_planet = pt.scalar()
+        t = pt.scalar()
+        orbit = KeplerianOrbit(
+            m_star=m_star,
+            r_star=1.0,
+            t0=0.0,
+            period=period,
+            ecc=ecc,
+            omega=omega,
+            Omega=Omega,
+            incl=incl,
+            m_planet=m_planet,
+        )
 
-    # True position
-    get_position = theano.function(
-        [t, m_star, period, ecc, omega, Omega, incl, m_planet],
-        orbit.get_planet_position([t], light_delay=False),
-    )
-
-    # Retarded position
-    get_retarded_position = theano.function(
-        [t, m_star, period, ecc, omega, Omega, incl, m_planet],
-        orbit.get_planet_position([t], light_delay=True),
-    )
-
-    # Retarded position (numerical)
-    def get_exact_retarded_position(t, *args):
-        def loss(params):
-            (ti,) = params
-            xr, yr, zr = get_position(ti, *args)
-            delay = (zr * u.Rsun / c).to(u.day).value
-            return (ti - delay - t) ** 2
-
-        tr = minimize(loss, t).x[0]
-        return get_position(tr, *args)
-
-    # Compare for 100 different orbits
-    np.random.seed(13)
-    for i in range(100):
-        m_star = 0.1 + np.random.random() * 1.9
-        period = np.random.random() * 500
-        ecc = np.random.random()
-        omega = np.random.random() * 2 * np.pi
-        Omega = np.random.random() * 2 * np.pi
-        incl = np.random.random() * 0.5 * np.pi
-        m_planet = np.random.random()
-        t = np.random.random() * period
-        args = (m_star, period, ecc, omega, Omega, incl, m_planet)
-        assert np.allclose(
-            np.reshape(get_retarded_position(t, *args), (-1,)),
-            np.reshape(get_exact_retarded_position(t, *args), (-1,)),
+        # True position
+        get_position = function(
+            [t, m_star, period, ecc, omega, Omega, incl, m_planet],
+            orbit.get_planet_position([t], light_delay=False),
         )
 
+        # Retarded position
+        get_retarded_position = function(
+            [t, m_star, period, ecc, omega, Omega, incl, m_planet],
+            orbit.get_planet_position([t], light_delay=True),
+        )
+
+        # Retarded position (numerical)
+        def get_exact_retarded_position(t, *args):
+            def loss(params):
+                (ti,) = params
+                xr, yr, zr = get_position(ti, *args)
+                delay = (zr * u.Rsun / c).to(u.day).value
+                return (ti - delay - t) ** 2
+
+            tr = minimize(loss, t).x[0]
+            return get_position(tr, *args)
+
+        # Compare for 100 different orbits
+        np.random.seed(13)
+        for i in range(100):
+            m_star = 0.1 + np.random.random() * 1.9
+            period = np.random.random() * 500
+            ecc = np.random.random()
+            omega = np.random.random() * 2 * np.pi
+            Omega = np.random.random() * 2 * np.pi
+            incl = np.random.random() * 0.5 * np.pi
+            m_planet = np.random.random()
+            t = np.random.random() * period
+            args = (m_star, period, ecc, omega, Omega, incl, m_planet)
+            assert np.allclose(
+                np.reshape(get_retarded_position(t, *args), (-1,)),
+                np.reshape(get_exact_retarded_position(t, *args), (-1,)),
+            )
+
 
 def test_light_delay_shape_two_planets_vector_t():
     orbit = KeplerianOrbit(period=[1.0, 2.0])
     t = np.linspace(0, 10, 50)
     x, y, z = orbit.get_planet_position(t, light_delay=False)
     xr, yr, zr = orbit.get_planet_position(t, light_delay=True)
     assert np.array_equal(x.shape.eval(), xr.shape.eval())
@@ -610,18 +611,18 @@
 def test_get_aor_from_transit_duration():
     duration = 0.12
     period = 10.1235
     b = 0.34
     ror = 0.06
     r_star = 0.7
 
-    dv = tt.as_tensor_variable(duration)
+    dv = pt.as_tensor_variable(duration)
     aor, jac = get_aor_from_transit_duration(dv, period, b, ror)
 
-    assert np.allclose(theano.grad(aor, dv).eval(), jac.eval())
+    assert np.allclose(grad(aor, dv).eval(), jac.eval())
 
     for orbit in [
         KeplerianOrbit(
             period=period, t0=0.0, b=b, a=r_star * aor, r_star=r_star
         ),
         KeplerianOrbit(
             period=period,
@@ -629,21 +630,21 @@
             b=b,
             duration=duration,
             r_star=r_star,
             ror=ror,
         ),
     ]:
         x, y, z = orbit.get_planet_position(0.5 * duration)
-        assert np.allclose(tt.sqrt(x**2 + y**2).eval(), r_star * (1 + ror))
+        assert np.allclose(pt.sqrt(x**2 + y**2).eval(), r_star * (1 + ror))
 
         x, y, z = orbit.get_planet_position(-0.5 * duration)
-        assert np.allclose(tt.sqrt(x**2 + y**2).eval(), r_star * (1 + ror))
+        assert np.allclose(pt.sqrt(x**2 + y**2).eval(), r_star * (1 + ror))
 
         x, y, z = orbit.get_planet_position(period + 0.5 * duration)
-        assert np.allclose(tt.sqrt(x**2 + y**2).eval(), r_star * (1 + ror))
+        assert np.allclose(pt.sqrt(x**2 + y**2).eval(), r_star * (1 + ror))
 
 
 @pytest.mark.filterwarnings("error::UserWarning")
 def test_duration_without_ror_warning():
     duration = 0.12
     period = 10.1235
     b = 0.34
@@ -663,36 +664,36 @@
 def test_jacobians():
     duration = 0.12
     period = 10.1235
     b = 0.34
     ror = 0.06
     r_star = 0.7
 
-    dv = tt.as_tensor_variable(duration)
+    dv = pt.as_tensor_variable(duration)
     orbit = KeplerianOrbit(
         period=period, t0=0.0, b=b, duration=dv, r_star=r_star, ror=ror
     )
     assert np.allclose(
         orbit.jacobians["duration"]["a"].eval(),
-        theano.grad(orbit.a, dv).eval(),
+        grad(orbit.a, dv).eval(),
     )
     assert np.allclose(
         orbit.jacobians["duration"]["a_planet"].eval(),
-        theano.grad(orbit.a_planet, dv).eval(),
+        grad(orbit.a_planet, dv).eval(),
     )
     assert np.allclose(
         orbit.jacobians["duration"]["a_star"].eval(),
-        theano.grad(orbit.a_star, dv).eval(),
+        grad(orbit.a_star, dv).eval(),
     )
     assert np.allclose(
         orbit.jacobians["duration"]["rho_star"].eval(),
-        theano.grad(orbit.rho_star, dv).eval(),
+        grad(orbit.rho_star, dv).eval(),
     )
 
-    bv = tt.as_tensor_variable(b)
+    bv = pt.as_tensor_variable(b)
     orbit = KeplerianOrbit(
         period=period, t0=0.0, b=bv, a=orbit.a, r_star=r_star, ror=ror
     )
     assert np.allclose(
         orbit.jacobians["b"]["cos_incl"].eval(),
-        theano.grad(orbit.cos_incl, bv).eval(),
+        grad(orbit.cos_incl, bv).eval(),
     )
```

### Comparing `exoplanet-0.5.3rc1/tests/orbits/simple_test.py` & `exoplanet-0.6.0rc2/tests/orbits/simple_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# -*- coding: utf-8 -*-
-
 import numpy as np
 import pytest
-from aesara_theano_fallback import aesara as theano
 
+from exoplanet.compat import function
 from exoplanet.light_curves import LimbDarkLightCurve
 from exoplanet.orbits import KeplerianOrbit, SimpleTransitOrbit
 
 
 def test_simple():
     period = 3.456
     t0 = 1.45
@@ -21,25 +19,25 @@
         < 0.5 * duration
     )
 
     orbit = SimpleTransitOrbit(
         period=period, duration=duration, t0=t0, b=b, r_star=r_star
     )
 
-    x, y, z = theano.function([], orbit.get_planet_position(t))()
+    x, y, z = function([], orbit.get_planet_position(t))()
     b_val = np.sqrt(x**2 + y**2)
     m = (b_val <= r_star) & (z > 0)
 
     assert np.all(m == m0)
 
     in_transit = orbit.in_transit(t).eval()
     assert np.all(b_val[in_transit] <= r_star)
     assert np.all(z[in_transit] > 0)
 
-    x, y, z = theano.function([], orbit.get_star_position(t))()
+    x, y, z = function([], orbit.get_star_position(t))()
     assert np.allclose(x, 0.0)
     assert np.allclose(y, 0.0)
     assert np.allclose(z, 0.0)
 
     with pytest.raises(NotImplementedError):
         orbit.get_planet_velocity(t)
```

### Comparing `exoplanet-0.5.3rc1/tests/orbits/ttv_test.py` & `exoplanet-0.6.0rc2/tests/orbits/ttv_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-# -*- coding: utf-8 -*-
-
 import numpy as np
-from aesara_theano_fallback import aesara as theano
 
+from exoplanet.compat import function
 from exoplanet.orbits.keplerian import KeplerianOrbit
 from exoplanet.orbits.ttv import TTVOrbit, compute_expected_transit_times
 
 
 def test_compute_expected_transit_times():
     periods = [10.5, 56.34]
     t0s = [45.3, 48.1]
@@ -31,15 +29,15 @@
     expected_times = compute_expected_transit_times(
         min_time, max_time, periods, t0s
     )
     ttvs = [0.01 * np.random.randn(len(t)) for t in expected_times]
     orbit = TTVOrbit(
         period=periods, t0=[t[0] for t in expected_times], ttvs=ttvs
     )
-    calc_times = theano.function([], orbit.transit_times)()
+    calc_times = function([], orbit.transit_times)()
     for i in range(len(expected_times)):
         assert np.allclose(calc_times[i], expected_times[i] + ttvs[i])
 
     orbit1 = TTVOrbit(transit_times=orbit.transit_times)
     orbit2 = TTVOrbit(period=orbit1.period, t0=orbit1.t0, ttvs=orbit1.ttvs)
     for i in range(len(expected_times)):
         assert np.allclose(
@@ -73,13 +71,13 @@
         "get_star_position",
         "get_planet_position",
         "get_relative_velocity",
         "get_star_velocity",
         "get_planet_velocity",
         "get_radial_velocity",
     ]:
-        expect = theano.function([], getattr(orbit0, arg)(time))()
-        calc1 = theano.function([], getattr(orbit1, arg)(time))()
-        calc2 = theano.function([], getattr(orbit2, arg)(time))()
+        expect = function([], getattr(orbit0, arg)(time))()
+        calc1 = function([], getattr(orbit1, arg)(time))()
+        calc2 = function([], getattr(orbit2, arg)(time))()
 
         assert np.allclose(expect, calc1), arg
         assert np.allclose(expect, calc2), arg
```

### Comparing `exoplanet-0.5.3rc1/tests/units_test.py` & `exoplanet-0.6.0rc2/tests/units_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 import astropy.units as u
 import numpy as np
 
 from exoplanet import units
 from exoplanet.orbits import KeplerianOrbit
```

### Comparing `exoplanet-0.5.3rc1/tox.ini` & `exoplanet-0.6.0rc2/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 [tox]
-envlist = py{38,39,310}-pymc{311,dev},lint,docs
+envlist = py{38,39,310},lint,docs
 
 [gh-actions]
 python =
     3.8: py38
     3.9: py39
     3.10: py310
 
-[gh-actions:env]
-PYMC_VERSION =
-    3.11: pymc311
-    dev: pymcdev
-
 [testenv]
 passenv = GITHUB_*
 deps =
     numpy<1.22
-    pymc311: pymc3~=3.11.0
-    pymcdev: https://github.com/pymc-devs/pymc/archive/v3.zip
 extras = test
 commands =
     pip freeze
     python -m coverage run -m pytest -v {posargs}
 
 [testenv:lint]
 skip_install = true
```

