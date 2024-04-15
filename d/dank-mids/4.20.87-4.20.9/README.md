# Comparing `tmp/dank_mids-4.20.87.tar.gz` & `tmp/dank_mids-4.20.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dank_mids-4.20.87.tar", last modified: Sun Apr 14 23:33:57 2024, max compression
+gzip compressed data, was "dank_mids-4.20.9.tar", last modified: Wed Oct 19 17:56:40 2022, max compression
```

## Comparing `dank_mids-4.20.87.tar` & `dank_mids-4.20.9.tar`

### file list

```diff
@@ -1,81 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:33:57.725025 dank_mids-4.20.87/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:33:57.713025 dank_mids-4.20.87/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:33:57.717025 dank_mids-4.20.87/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-14 23:33:41.000000 dank_mids-4.20.87/.github/workflows/deploy-docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-14 23:33:41.000000 dank_mids-4.20.87/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-14 23:33:41.000000 dank_mids-4.20.87/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-14 23:33:41.000000 dank_mids-4.20.87/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-14 23:33:41.000000 dank_mids-4.20.87/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-14 23:33:41.000000 dank_mids-4.20.87/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-14 23:33:57.725025 dank_mids-4.20.87/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-14 23:33:41.000000 dank_mids-4.20.87/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:33:57.717025 dank_mids-4.20.87/dank_mids/
--rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/ENVIRONMENT_VARIABLES.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/_demo_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/_envs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    39794 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/_uid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:33:57.721025 dank_mids-4.20.87/dank_mids/brownie_patch/
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/brownie_patch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/brownie_patch/call.py
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/brownie_patch/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/brownie_patch/overloaded.py
--rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/brownie_patch/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    11145 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:33:57.721025 dank_mids-4.20.87/dank_mids/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/helpers/_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/helpers/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7764 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/helpers/_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/semaphore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/semaphores.py
--rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-14 23:33:41.000000 dank_mids-4.20.87/dank_mids/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:33:57.725025 dank_mids-4.20.87/dank_mids.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-14 23:33:57.000000 dank_mids-4.20.87/dank_mids.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-14 23:33:57.000000 dank_mids-4.20.87/dank_mids.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 23:33:57.000000 dank_mids-4.20.87/dank_mids.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-14 23:33:57.000000 dank_mids-4.20.87/dank_mids.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-14 23:33:57.000000 dank_mids-4.20.87/dank_mids.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:33:57.721025 dank_mids-4.20.87/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-14 23:33:41.000000 dank_mids-4.20.87/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:33:57.713025 dank_mids-4.20.87/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:33:57.713025 dank_mids-4.20.87/docs/_build/html/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:33:57.721025 dank_mids-4.20.87/docs/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-04-14 23:33:41.000000 dank_mids-4.20.87/docs/_build/html/_static/alabaster.css
--rw-r--r--   0 runner    (1001) docker     (127)    15059 2024-04-14 23:33:41.000000 dank_mids-4.20.87/docs/_build/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-14 23:33:41.000000 dank_mids-4.20.87/docs/_build/html/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-14 23:33:41.000000 dank_mids-4.20.87/docs/_build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-14 23:33:41.000000 dank_mids-4.20.87/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-14 23:33:41.000000 dank_mids-4.20.87/docs/_build/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-14 23:33:41.000000 dank_mids-4.20.87/docs/_build/html/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-14 23:33:41.000000 dank_mids-4.20.87/docs/_build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-14 23:33:41.000000 dank_mids-4.20.87/docs/_build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-14 23:33:41.000000 dank_mids-4.20.87/docs/_build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-04-14 23:33:41.000000 dank_mids-4.20.87/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-14 23:33:41.000000 dank_mids-4.20.87/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-14 23:33:41.000000 dank_mids-4.20.87/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-14 23:33:41.000000 dank_mids-4.20.87/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-14 23:33:41.000000 dank_mids-4.20.87/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:33:57.721025 dank_mids-4.20.87/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-14 23:33:41.000000 dank_mids-4.20.87/examples/dank_brownie_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-14 23:33:41.000000 dank_mids-4.20.87/license
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-14 23:33:41.000000 dank_mids-4.20.87/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-14 23:33:41.000000 dank_mids-4.20.87/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-14 23:33:41.000000 dank_mids-4.20.87/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-14 23:33:57.725025 dank_mids-4.20.87/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-14 23:33:41.000000 dank_mids-4.20.87/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:33:57.725025 dank_mids-4.20.87/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 23:33:41.000000 dank_mids-4.20.87/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-14 23:33:41.000000 dank_mids-4.20.87/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-14 23:33:41.000000 dank_mids-4.20.87/tests/test_brownie_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-04-14 23:33:41.000000 dank_mids-4.20.87/tests/test_dank_mids.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:40.680519 dank_mids-4.20.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:40.676519 dank_mids-4.20.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:40.676519 dank_mids-4.20.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      545 2022-10-19 17:56:26.000000 dank_mids-4.20.9/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-10-19 17:56:26.000000 dank_mids-4.20.9/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      609 2022-10-19 17:56:26.000000 dank_mids-4.20.9/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-10-19 17:56:26.000000 dank_mids-4.20.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-10-19 17:56:40.680519 dank_mids-4.20.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-10-19 17:56:26.000000 dank_mids-4.20.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:40.680519 dank_mids-4.20.9/dank_mids/
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      560 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      331 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/_demo_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:40.680519 dank_mids-4.20.9/dank_mids/brownie_patch/
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/brownie_patch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3016 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/brownie_patch/call.py
+-rw-r--r--   0 runner    (1001) docker     (121)      981 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/brownie_patch/contract.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/brownie_patch/overloaded.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4784 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/call.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2971 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4685 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)      793 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      237 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)      995 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)      465 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/uid.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11199 2022-10-19 17:56:26.000000 dank_mids-4.20.9/dank_mids/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:40.680519 dank_mids-4.20.9/dank_mids.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-10-19 17:56:40.000000 dank_mids-4.20.9/dank_mids.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      874 2022-10-19 17:56:40.000000 dank_mids-4.20.9/dank_mids.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 17:56:40.000000 dank_mids-4.20.9/dank_mids.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-10-19 17:56:40.000000 dank_mids-4.20.9/dank_mids.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-19 17:56:40.000000 dank_mids-4.20.9/dank_mids.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-19 17:56:26.000000 dank_mids-4.20.9/license
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-10-19 17:56:26.000000 dank_mids-4.20.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-10-19 17:56:26.000000 dank_mids-4.20.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-10-19 17:56:26.000000 dank_mids-4.20.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-19 17:56:40.680519 dank_mids-4.20.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      778 2022-10-19 17:56:26.000000 dank_mids-4.20.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:40.680519 dank_mids-4.20.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 17:56:26.000000 dank_mids-4.20.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2022-10-19 17:56:26.000000 dank_mids-4.20.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2022-10-19 17:56:26.000000 dank_mids-4.20.9/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-10-19 17:56:26.000000 dank_mids-4.20.9/tests/test_brownie_patch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2310 2022-10-19 17:56:26.000000 dank_mids-4.20.9/tests/test_dank_mids.py
```

### Comparing `dank_mids-4.20.87/.github/workflows/mypy.yaml` & `dank_mids-4.20.9/.github/workflows/mypy.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 
     - name: Install MyPy
       run: |
         python -m pip install --upgrade pip
         pip install mypy types-requests
 
     - name: Run MyPy
-      run: mypy ./dank_mids --pretty --ignore-missing-imports --show-error-codes --show-error-context --no-warn-no-return
+      run: mypy ./dank_mids --pretty --ignore-missing-imports --show-error-codes --show-error-context
```

### Comparing `dank_mids-4.20.87/.github/workflows/pytest.yaml` & `dank_mids-4.20.9/.github/workflows/pytest.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -7,20 +7,18 @@
     paths:
       - '**.py'
       - '**/pytest.yaml'
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
+    #timeout-minutes: 10
     strategy:
-      fail-fast: false
       matrix:
         os: [ ubuntu-latest, macos-latest, windows-latest ]
-        pyversion: [ "3.8", "3.9", "3.10", "3.11", "3.12" ]
-        provider: [ "TENDERLY_PROVIDER", "LLAMA_ETH_RPC", "INFURA_PROVIDER", "ALCHEMY_PROVIDER" ]
         include:
         - os: ubuntu-latest
           path: ~/.cache/pip
         - os: macos-latest
           path: ~/Library/Caches/pip
         - os: windows-latest
           path: ~\AppData\Local\pip\Cache
@@ -28,24 +26,24 @@
     steps:
       - name: Check out repository code
         uses: actions/checkout@v2
 
       - name: Setup Python (faster than using Python container)
         uses: actions/setup-python@v2
         with:
-          python-version: ${{ matrix.pyversion }}
+          python-version: "3.9"
 
       - name: Install dependencies
         run: |
           pip install -r requirements.txt -r requirements-dev.txt
       
       - name: Setup brownie networks
         run: |
-          brownie networks modify mainnet host=${{ secrets[matrix.provider] }}
+          brownie networks modify mainnet host=${{ secrets.WEB3_PROVIDER }}
         continue-on-error: true
 
       - name: Run test suite
         env:
           PYTEST_NETWORK: mainnet
           ETHERSCAN_TOKEN: ${{ secrets.ETHERSCAN_TOKEN  }}
-        run: pytest --asyncio-task-timeout=3600
-      
+        run: pytest
+
```

### Comparing `dank_mids-4.20.87/.github/workflows/release.yaml` & `dank_mids-4.20.9/.github/workflows/release.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 on:
   push:
     branches:
       - dev
   release:
     branches:
       - master
-    types: [published]
 
 jobs:
   deploy:
     runs-on: ubuntu-20.04
 
     steps:
     - uses: actions/checkout@v2
```

### Comparing `dank_mids-4.20.87/dank_mids/brownie_patch/overloaded.py` & `dank_mids-4.20.9/dank_mids/brownie_patch/overloaded.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,31 @@
 import functools
 from types import MethodType
-from typing import Any, Dict, Optional, Tuple, Union
+from typing import Any, Coroutine, Dict, Optional, Tuple, Union
 
 from brownie import Contract
 from brownie.network.contract import ContractCall, ContractTx, OverloadedMethod
-from dank_mids.brownie_patch.call import _get_coroutine_fn, _skip_proc_pool
-from dank_mids.brownie_patch.types import ContractMethod
+from dank_mids.brownie_patch.call import _patch_call
 from web3 import Web3
 
 
 def _patch_overloaded_method(call: OverloadedMethod, w3: Web3) -> None:
-    # sourcery skip: avoid-builtin-shadow
     @functools.wraps(call)
     async def coroutine(
         self: Contract,
         *args: Tuple[Any,...],
         block_identifier: Optional[Union[int, str, bytes]] = None,
-        decimals: Optional[int] = None,
-        override: Optional[Dict[str, str]] = None,
+        override: Optional[Dict[str, str]] = None
     ) -> Any:
-        try:
-            fn = self._get_fn_from_args(args)
-        except ValueError as e:
-            if f"Contract has more than one function '.{call._name}" in str(e) and f"You must explicitly declare which function you are calling, e.g. .{call._name}" in str(e):
-                exc_str = str(e)
-                breakpoint = exc_str.find("(*args)")
-                raise ValueError(f"{exc_str[:breakpoint]}.coroutine{exc_str[breakpoint:]}")
-            raise e
-
-        kwargs = {"block_identifier": block_identifier, "decimals": decimals, "override": override}
+        fn = self._get_fn_from_args(args)
+        kwargs = {"block_identifier": block_identifier, "override": override}
         kwargs = {k: v for k, v in kwargs.items() if v is not None}
         return await fn.coroutine(*args, **kwargs)
 
-    for method in call.__dict__['methods'].values():
-        if isinstance(method, (ContractCall, ContractTx)):
-            method._skip_decoder_proc_pool = method._address in _skip_proc_pool
-            method.coroutine = MethodType(_get_coroutine_fn(w3, len(method.abi['inputs'])), method)
+    for args, method in call.__dict__['methods'].items():
+        if isinstance(method, ContractCall) or isinstance(method, ContractTx):
+            _patch_call(method, w3)
     # TODO implement this properly
         #elif isinstance(call, ContractTx):
             #_patch_tx(call, w3)
-
+    
     call.coroutine = MethodType(coroutine, call)
```

### Comparing `dank_mids-4.20.87/dank_mids/middleware.py` & `dank_mids-4.20.9/dank_mids/middleware.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 
-import logging
-from threading import Thread, current_thread
-from typing import Any, Callable, Dict, Tuple
+from typing import Any, Callable
 
 from web3 import Web3
-from web3.types import RPCEndpoint
+from web3.types import RPCEndpoint, RPCResponse
 
 from dank_mids.controller import DankMiddlewareController
 from dank_mids.types import AsyncMiddleware
 
-_controllers: Dict[Tuple[Web3, Thread], DankMiddlewareController] = {}
-
-logger = logging.getLogger(__name__)
 
 async def dank_middleware(
     make_request: Callable[[RPCEndpoint, Any], Any],
     web3: Web3
 ) -> AsyncMiddleware:
-    return DankMiddlewareController(web3)
+    dank_mids = DankMiddlewareController(web3)
+    async def middleware(method: RPCEndpoint, params: Any) -> RPCResponse:
+        if dank_mids.should_batch(method, params):
+            return await dank_mids(params)
+        return await make_request(method, params)
+    return middleware
```

### Comparing `dank_mids-4.20.87/license` & `dank_mids-4.20.9/license`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.87/setup.py` & `dank_mids-4.20.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # type: ignore
 
 from setuptools import find_packages, setup
 
-with open("requirements.txt", "r") as f:
-    requirements = list(map(str.strip, f.read().split("\n")))[:-1]
-
 setup(
     name='dank_mids',
     packages=find_packages(),
     use_scm_version={
         "root": ".",
         "relative_to": __file__,
         "local_scheme": "no-local-version",
         "version_scheme": "python-simplified-semver",
     },
     description='Multicall batching middleware for asynchronous scripts using web3.py',
     author='BobTheBuidler',
     author_email='bobthebuidlerdefi@gmail.com',
     url='https://github.com/BobTheBuidler/dank_mids',
     license='MIT',
-    install_requires=requirements,
+    install_requires=[
+        "bobs_lazy_logging>=0.0.4",
+        "eth_retry>=0.1.12",
+        "multicall>=0.6.2",
+    ],
     setup_requires=[
         'setuptools_scm',
     ],
     package_data={
         "dank_mids": ["py.typed"],
     },
 )
```

