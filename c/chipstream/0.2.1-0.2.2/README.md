# Comparing `tmp/chipstream-0.2.1.tar.gz` & `tmp/chipstream-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chipstream-0.2.1.tar", last modified: Tue Apr 16 08:30:21 2024, max compression
+gzip compressed data, was "chipstream-0.2.2.tar", last modified: Tue Apr 16 08:41:40 2024, max compression
```

## Comparing `chipstream-0.2.1.tar` & `chipstream-0.2.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:21.960731 chipstream-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:21.948731 chipstream-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:21.952731 chipstream-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-16 08:30:18.000000 chipstream-0.2.1/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-16 08:30:18.000000 chipstream-0.2.1/.github/workflows/deploy_github.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-16 08:30:18.000000 chipstream-0.2.1/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-16 08:30:18.000000 chipstream-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-16 08:30:18.000000 chipstream-0.2.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-16 08:30:18.000000 chipstream-0.2.1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-16 08:30:18.000000 chipstream-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-16 08:30:21.960731 chipstream-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-16 08:30:18.000000 chipstream-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:21.956731 chipstream-0.2.1/build-recipes/
--rw-r--r--   0 runner    (1001) docker     (127)    75281 2024-04-16 08:30:18.000000 chipstream-0.2.1/build-recipes/ChipStream.icns
--rw-r--r--   0 runner    (1001) docker     (127)   353118 2024-04-16 08:30:18.000000 chipstream-0.2.1/build-recipes/ChipStream.ico
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-16 08:30:18.000000 chipstream-0.2.1/build-recipes/ChipStreamLauncher.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-16 08:30:18.000000 chipstream-0.2.1/build-recipes/ChipStreamLauncherCLI.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-16 08:30:18.000000 chipstream-0.2.1/build-recipes/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-16 08:30:18.000000 chipstream-0.2.1/build-recipes/hook-chipstream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-16 08:30:18.000000 chipstream-0.2.1/build-recipes/macos_ChipStream.spec
--rwxr-xr-x   0 runner    (1001) docker     (127)     1981 2024-04-16 08:30:18.000000 chipstream-0.2.1/build-recipes/macos_build_app.sh
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 08:30:18.000000 chipstream-0.2.1/build-recipes/macos_build_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-16 08:30:18.000000 chipstream-0.2.1/build-recipes/win_ChipStream.spec
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 08:30:18.000000 chipstream-0.2.1/build-recipes/win_build_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-04-16 08:30:18.000000 chipstream-0.2.1/build-recipes/win_chipstream.iss_dummy
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-16 08:30:18.000000 chipstream-0.2.1/build-recipes/win_make_iss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:21.956731 chipstream-0.2.1/chipstream/
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-16 08:30:18.000000 chipstream-0.2.1/chipstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-16 08:30:21.000000 chipstream-0.2.1/chipstream/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:21.956731 chipstream-0.2.1/chipstream/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-16 08:30:18.000000 chipstream-0.2.1/chipstream/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-16 08:30:18.000000 chipstream-0.2.1/chipstream/cli/cli_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-16 08:30:18.000000 chipstream-0.2.1/chipstream/cli/cli_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-16 08:30:18.000000 chipstream-0.2.1/chipstream/cli/cli_proc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-16 08:30:18.000000 chipstream-0.2.1/chipstream/cli/cli_valid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:21.956731 chipstream-0.2.1/chipstream/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-16 08:30:18.000000 chipstream-0.2.1/chipstream/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:21.956731 chipstream-0.2.1/chipstream/gui/img/
--rw-r--r--   0 runner    (1001) docker     (127)    14396 2024-04-16 08:30:18.000000 chipstream-0.2.1/chipstream/gui/img/chipstream_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    13292 2024-04-16 08:30:18.000000 chipstream-0.2.1/chipstream/gui/main_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    13667 2024-04-16 08:30:18.000000 chipstream-0.2.1/chipstream/gui/main_window.ui
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-16 08:30:18.000000 chipstream-0.2.1/chipstream/gui/splash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-16 08:30:18.000000 chipstream-0.2.1/chipstream/gui/table_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     9702 2024-04-16 08:30:18.000000 chipstream-0.2.1/chipstream/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-16 08:30:18.000000 chipstream-0.2.1/chipstream/path_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:21.960731 chipstream-0.2.1/chipstream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-16 08:30:21.000000 chipstream-0.2.1/chipstream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-16 08:30:21.000000 chipstream-0.2.1/chipstream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:30:21.000000 chipstream-0.2.1/chipstream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 08:30:21.000000 chipstream-0.2.1/chipstream.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-16 08:30:21.000000 chipstream-0.2.1/chipstream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 08:30:21.000000 chipstream-0.2.1/chipstream.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:21.956731 chipstream-0.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:21.960731 chipstream-0.2.1/docs/artwork/
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-16 08:30:18.000000 chipstream-0.2.1/docs/artwork/chipstream_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-04-16 08:30:18.000000 chipstream-0.2.1/docs/artwork/chipstream_splash.png
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-16 08:30:18.000000 chipstream-0.2.1/docs/artwork/chipstream_splash.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-16 08:30:18.000000 chipstream-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-16 08:30:18.000000 chipstream-0.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 08:30:18.000000 chipstream-0.2.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-16 08:30:18.000000 chipstream-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 08:30:21.960731 chipstream-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:21.960731 chipstream-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-16 08:30:18.000000 chipstream-0.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:30:21.960731 chipstream-0.2.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)   154010 2024-04-16 08:30:18.000000 chipstream-0.2.1/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-16 08:30:18.000000 chipstream-0.2.1/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-16 08:30:18.000000 chipstream-0.2.1/tests/requirements-full.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 08:30:18.000000 chipstream-0.2.1/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-16 08:30:18.000000 chipstream-0.2.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-16 08:30:18.000000 chipstream-0.2.1/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-16 08:30:18.000000 chipstream-0.2.1/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-16 08:30:18.000000 chipstream-0.2.1/tests/test_path_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.254051 chipstream-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.242051 chipstream-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.242051 chipstream-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-16 08:41:34.000000 chipstream-0.2.2/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-16 08:41:34.000000 chipstream-0.2.2/.github/workflows/deploy_github.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-16 08:41:34.000000 chipstream-0.2.2/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-16 08:41:34.000000 chipstream-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-16 08:41:34.000000 chipstream-0.2.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-16 08:41:34.000000 chipstream-0.2.2/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-16 08:41:34.000000 chipstream-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-16 08:41:40.254051 chipstream-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-16 08:41:34.000000 chipstream-0.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.246050 chipstream-0.2.2/build-recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)    75281 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/ChipStream.icns
+-rw-r--r--   0 runner    (1001) docker     (127)   353118 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/ChipStream.ico
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/ChipStreamLauncher.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/ChipStreamLauncherCLI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/hook-chipstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/macos_ChipStream.spec
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1981 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/macos_build_app.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/macos_build_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/win_ChipStream.spec
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/win_build_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/win_chipstream.iss_dummy
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/win_make_iss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.246050 chipstream-0.2.2/chipstream/
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-16 08:41:40.000000 chipstream-0.2.2/chipstream/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.250050 chipstream-0.2.2/chipstream/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/cli/cli_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/cli/cli_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/cli/cli_proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/cli/cli_valid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.250050 chipstream-0.2.2/chipstream/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.250050 chipstream-0.2.2/chipstream/gui/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    14396 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/gui/img/chipstream_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13292 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/gui/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13667 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/gui/main_window.ui
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/gui/splash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/gui/table_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9702 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/path_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.254051 chipstream-0.2.2/chipstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-16 08:41:40.000000 chipstream-0.2.2/chipstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-16 08:41:40.000000 chipstream-0.2.2/chipstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:41:40.000000 chipstream-0.2.2/chipstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 08:41:40.000000 chipstream-0.2.2/chipstream.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-16 08:41:40.000000 chipstream-0.2.2/chipstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 08:41:40.000000 chipstream-0.2.2/chipstream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.250050 chipstream-0.2.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.250050 chipstream-0.2.2/docs/artwork/
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-16 08:41:34.000000 chipstream-0.2.2/docs/artwork/chipstream_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-04-16 08:41:34.000000 chipstream-0.2.2/docs/artwork/chipstream_splash.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-16 08:41:34.000000 chipstream-0.2.2/docs/artwork/chipstream_splash.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-16 08:41:34.000000 chipstream-0.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-16 08:41:34.000000 chipstream-0.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 08:41:34.000000 chipstream-0.2.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-16 08:41:34.000000 chipstream-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 08:41:40.254051 chipstream-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.254051 chipstream-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-16 08:41:34.000000 chipstream-0.2.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.254051 chipstream-0.2.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   154010 2024-04-16 08:41:34.000000 chipstream-0.2.2/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-16 08:41:34.000000 chipstream-0.2.2/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-16 08:41:34.000000 chipstream-0.2.2/tests/requirements-full.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 08:41:34.000000 chipstream-0.2.2/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-16 08:41:34.000000 chipstream-0.2.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-16 08:41:34.000000 chipstream-0.2.2/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-16 08:41:34.000000 chipstream-0.2.2/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-16 08:41:34.000000 chipstream-0.2.2/tests/test_path_cache.py
```

### Comparing `chipstream-0.2.1/.github/workflows/check.yml` & `chipstream-0.2.2/.github/workflows/check.yml`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,16 @@
         sudo /usr/bin/Xvfb $DISPLAY -screen 0 1280x1024x24 &
     - name: Install Python dependencies
       run: |
         # prerequisites
         python -m pip install --upgrade pip wheel
         python -m pip install coverage flake8 pytest
         # install base dependencies
+        # https://github.com/luispedro/mahotas/issues/144
+        pip install mahotas==1.4.13
         pip install .
         pip install -r tests/requirements.txt
         # show installed packages
         pip freeze
     - name: Install extended dependencies
       if: matrix.deps == 'all'
       run: |
```

### Comparing `chipstream-0.2.1/.github/workflows/deploy_github.yml` & `chipstream-0.2.2/.github/workflows/deploy_github.yml`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,16 @@
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install Python dependencies
       run: |
         python -m pip install --upgrade pip
         pip install setuptools wheel twine
+        # https://github.com/luispedro/mahotas/issues/144
+        pip install mahotas==1.4.13
         pip install .[cli,gui]
     - name: Build macOS app
       if: runner.os == 'macOS'
       working-directory: ./build-recipes
       run: |
         bash ./macos_build_app.sh ChipStream ${{ env.RELEASE_VERSION }}
     - name: Build windows executable
```

### Comparing `chipstream-0.2.1/.github/workflows/deploy_pypi.yml` & `chipstream-0.2.2/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/.gitignore` & `chipstream-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/LICENSE` & `chipstream-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/PKG-INFO` & `chipstream-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chipstream
-Version: 0.2.1
+Version: 0.2.2
 Summary: GUI for DC data postprocessing
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: GPL version 3.0 or later
 Project-URL: source, https://github.com/DC-Analysis/ChipStream
 Project-URL: tracker, https://github.com/DC-Analysis/ChipStream/issues
 Project-URL: documentation, https://chipstream.readthedocs.io/en/stable/
```

### Comparing `chipstream-0.2.1/README.rst` & `chipstream-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/build-recipes/ChipStream.icns` & `chipstream-0.2.2/build-recipes/ChipStream.icns`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/build-recipes/ChipStream.ico` & `chipstream-0.2.2/build-recipes/ChipStream.ico`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/build-recipes/Readme.md` & `chipstream-0.2.2/build-recipes/Readme.md`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/build-recipes/hook-chipstream.py` & `chipstream-0.2.2/build-recipes/hook-chipstream.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/build-recipes/macos_ChipStream.spec` & `chipstream-0.2.2/build-recipes/macos_ChipStream.spec`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/build-recipes/macos_build_app.sh` & `chipstream-0.2.2/build-recipes/macos_build_app.sh`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/build-recipes/win_ChipStream.spec` & `chipstream-0.2.2/build-recipes/win_ChipStream.spec`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/build-recipes/win_chipstream.iss_dummy` & `chipstream-0.2.2/build-recipes/win_chipstream.iss_dummy`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/build-recipes/win_make_iss.py` & `chipstream-0.2.2/build-recipes/win_make_iss.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/chipstream/__init__.py` & `chipstream-0.2.2/chipstream/__init__.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/chipstream/cli/cli_common.py` & `chipstream-0.2.2/chipstream/cli/cli_common.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/chipstream/cli/cli_main.py` & `chipstream-0.2.2/chipstream/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/chipstream/cli/cli_proc.py` & `chipstream-0.2.2/chipstream/cli/cli_proc.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/chipstream/cli/cli_valid.py` & `chipstream-0.2.2/chipstream/cli/cli_valid.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/chipstream/gui/__init__.py` & `chipstream-0.2.2/chipstream/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/chipstream/gui/img/chipstream_icon.png` & `chipstream-0.2.2/chipstream/gui/img/chipstream_icon.png`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/chipstream/gui/main_window.py` & `chipstream-0.2.2/chipstream/gui/main_window.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/chipstream/gui/main_window.ui` & `chipstream-0.2.2/chipstream/gui/main_window.ui`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/chipstream/gui/table_progress.py` & `chipstream-0.2.2/chipstream/gui/table_progress.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/chipstream/manager.py` & `chipstream-0.2.2/chipstream/manager.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/chipstream/path_cache.py` & `chipstream-0.2.2/chipstream/path_cache.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/chipstream.egg-info/PKG-INFO` & `chipstream-0.2.2/chipstream.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chipstream
-Version: 0.2.1
+Version: 0.2.2
 Summary: GUI for DC data postprocessing
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: GPL version 3.0 or later
 Project-URL: source, https://github.com/DC-Analysis/ChipStream
 Project-URL: tracker, https://github.com/DC-Analysis/ChipStream/issues
 Project-URL: documentation, https://chipstream.readthedocs.io/en/stable/
```

### Comparing `chipstream-0.2.1/chipstream.egg-info/SOURCES.txt` & `chipstream-0.2.2/chipstream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/docs/artwork/chipstream_icon.svg` & `chipstream-0.2.2/docs/artwork/chipstream_icon.svg`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/docs/artwork/chipstream_splash.png` & `chipstream-0.2.2/docs/artwork/chipstream_splash.png`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/docs/artwork/chipstream_splash.svg` & `chipstream-0.2.2/docs/artwork/chipstream_splash.svg`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/docs/conf.py` & `chipstream-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/pyproject.toml` & `chipstream-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/tests/conftest.py` & `chipstream-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip` & `chipstream-0.2.2/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/tests/helper_methods.py` & `chipstream-0.2.2/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/tests/test_cli.py` & `chipstream-0.2.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/tests/test_gui.py` & `chipstream-0.2.2/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/tests/test_manager.py` & `chipstream-0.2.2/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.1/tests/test_path_cache.py` & `chipstream-0.2.2/tests/test_path_cache.py`

 * *Files identical despite different names*

