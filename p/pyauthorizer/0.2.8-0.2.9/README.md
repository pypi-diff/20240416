# Comparing `tmp/pyauthorizer-0.2.8.tar.gz` & `tmp/pyauthorizer-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyauthorizer-0.2.8.tar", last modified: Thu Jan 25 03:20:52 2024, max compression
+gzip compressed data, was "pyauthorizer-0.2.9.tar", last modified: Tue Jan 30 01:26:47 2024, max compression
```

## Comparing `pyauthorizer-0.2.8.tar` & `pyauthorizer-0.2.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 03:20:52.276882 pyauthorizer-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 03:20:52.268882 pyauthorizer-0.2.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 03:20:52.268882 pyauthorizer-0.2.8/.github/matchers/
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/.github/matchers/pylint.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 03:20:52.268882 pyauthorizer-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/.github/workflows/preview.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/.releaserc.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 03:20:52.268882 pyauthorizer-0.2.8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-01-25 03:20:52.276882 pyauthorizer-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 03:20:52.268882 pyauthorizer-0.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/docs/advance.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 03:20:52.268882 pyauthorizer-0.2.8/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/docs/api/pyauthorizer.encryptor.builtin.rst
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/docs/api/pyauthorizer.encryptor.rst
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/docs/api/pyauthorizer.rst
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/docs/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-25 03:20:52.276882 pyauthorizer-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 03:20:52.264882 pyauthorizer-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 03:20:52.272882 pyauthorizer-0.2.8/src/pyauthorizer/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/src/pyauthorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/src/pyauthorizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-25 03:20:52.000000 pyauthorizer-0.2.8/src/pyauthorizer/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/src/pyauthorizer/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/src/pyauthorizer/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 03:20:52.272882 pyauthorizer-0.2.8/src/pyauthorizer/encryptor/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/src/pyauthorizer/encryptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/src/pyauthorizer/encryptor/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 03:20:52.272882 pyauthorizer-0.2.8/src/pyauthorizer/encryptor/builtin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/src/pyauthorizer/encryptor/builtin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/src/pyauthorizer/encryptor/builtin/multiple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/src/pyauthorizer/encryptor/builtin/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/src/pyauthorizer/encryptor/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/src/pyauthorizer/encryptor/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/src/pyauthorizer/encryptor/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/src/pyauthorizer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/src/pyauthorizer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 03:20:52.272882 pyauthorizer-0.2.8/src/pyauthorizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-01-25 03:20:52.000000 pyauthorizer-0.2.8/src/pyauthorizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-01-25 03:20:52.000000 pyauthorizer-0.2.8/src/pyauthorizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 03:20:52.000000 pyauthorizer-0.2.8/src/pyauthorizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-25 03:20:52.000000 pyauthorizer-0.2.8/src/pyauthorizer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-25 03:20:52.000000 pyauthorizer-0.2.8/src/pyauthorizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-25 03:20:52.000000 pyauthorizer-0.2.8/src/pyauthorizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 03:20:52.272882 pyauthorizer-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/tests/test_encryptor_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-01-25 03:20:33.000000 pyauthorizer-0.2.8/tests/test_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 01:26:47.195868 pyauthorizer-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 01:26:47.187868 pyauthorizer-0.2.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 01:26:47.187868 pyauthorizer-0.2.9/.github/matchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/.github/matchers/pylint.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 01:26:47.187868 pyauthorizer-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/.github/workflows/preview.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/.releaserc.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 01:26:47.187868 pyauthorizer-0.2.9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-01-30 01:26:47.195868 pyauthorizer-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 01:26:47.191868 pyauthorizer-0.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/docs/advance.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 01:26:47.191868 pyauthorizer-0.2.9/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/docs/api/pyauthorizer.encryptor.builtin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/docs/api/pyauthorizer.encryptor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/docs/api/pyauthorizer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/docs/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 01:26:47.195868 pyauthorizer-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 01:26:47.183868 pyauthorizer-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 01:26:47.191868 pyauthorizer-0.2.9/src/pyauthorizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/src/pyauthorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/src/pyauthorizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-30 01:26:47.000000 pyauthorizer-0.2.9/src/pyauthorizer/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/src/pyauthorizer/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/src/pyauthorizer/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 01:26:47.191868 pyauthorizer-0.2.9/src/pyauthorizer/encryptor/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/src/pyauthorizer/encryptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/src/pyauthorizer/encryptor/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 01:26:47.191868 pyauthorizer-0.2.9/src/pyauthorizer/encryptor/builtin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/src/pyauthorizer/encryptor/builtin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/src/pyauthorizer/encryptor/builtin/multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/src/pyauthorizer/encryptor/builtin/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/src/pyauthorizer/encryptor/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/src/pyauthorizer/encryptor/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/src/pyauthorizer/encryptor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/src/pyauthorizer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/src/pyauthorizer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 01:26:47.195868 pyauthorizer-0.2.9/src/pyauthorizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-01-30 01:26:47.000000 pyauthorizer-0.2.9/src/pyauthorizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-01-30 01:26:47.000000 pyauthorizer-0.2.9/src/pyauthorizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 01:26:47.000000 pyauthorizer-0.2.9/src/pyauthorizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-30 01:26:47.000000 pyauthorizer-0.2.9/src/pyauthorizer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-30 01:26:47.000000 pyauthorizer-0.2.9/src/pyauthorizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-30 01:26:47.000000 pyauthorizer-0.2.9/src/pyauthorizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 01:26:47.195868 pyauthorizer-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/tests/test_encryptor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-01-30 01:26:28.000000 pyauthorizer-0.2.9/tests/test_package.py
```

### Comparing `pyauthorizer-0.2.8/.github/CONTRIBUTING.md` & `pyauthorizer-0.2.9/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/.github/matchers/pylint.json` & `pyauthorizer-0.2.9/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/.github/workflows/cd.yml` & `pyauthorizer-0.2.9/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/.github/workflows/ci.yml` & `pyauthorizer-0.2.9/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
       - name: Test package
         run: >-
           python -m pytest -ra --cov --cov-report=xml --cov-report=term
           --durations=20
 
       - name: Upload coverage report
-        uses: codecov/codecov-action@v3.1.4
+        uses: codecov/codecov-action@v3.1.5
 
   docs:
     name: Docs on ${{ matrix.runs-on }}
     strategy:
       fail-fast: false
       matrix:
         runs-on: [ubuntu-latest, windows-latest]
```

### Comparing `pyauthorizer-0.2.8/.github/workflows/preview.yml` & `pyauthorizer-0.2.9/.github/workflows/preview.yml`

 * *Files 23% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 concurrency:
   group: preview-${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 jobs:
   pages-preview:
     runs-on: ubuntu-latest
+    permissions:
+      contents: write
 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - uses: wntrblm/nox@2023.04.22
```

### Comparing `pyauthorizer-0.2.8/.gitignore` & `pyauthorizer-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/.pre-commit-config.yaml` & `pyauthorizer-0.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/.releaserc.js` & `pyauthorizer-0.2.9/.releaserc.js`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/.vscode/launch.json` & `pyauthorizer-0.2.9/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/CHANGELOG.md` & `pyauthorizer-0.2.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+## [0.2.9](https://github.com/msclock/pyauthorizer/compare/v0.2.8...v0.2.9) (2024-01-30)
+
+
+### Chores
+
+* change pypi badge with shields ([ea9180e](https://github.com/msclock/pyauthorizer/commit/ea9180e4670ec3538364ad29cc2a1b9dae6d287a))
+* **deps:** bump codecov/codecov-action from 3.1.4 to 3.1.5 ([#18](https://github.com/msclock/pyauthorizer/issues/18)) ([7168e7e](https://github.com/msclock/pyauthorizer/commit/7168e7e016d5e663fbf90e44894672c5c5da3e40))
+
+
+### Docs
+
+* fix typo ([626d918](https://github.com/msclock/pyauthorizer/commit/626d9183525a07cde7a172338f198ed6d727b073))
+* more comments ([5c93831](https://github.com/msclock/pyauthorizer/commit/5c938314df7b16cf48da2ab96a295f84fe0d311e))
+
 ## [0.2.8](https://github.com/msclock/pyauthorizer/compare/v0.2.7...v0.2.8) (2024-01-25)
 
 
 ### Performance
 
 * specify encryptor plugins group explicitly ([006ea6d](https://github.com/msclock/pyauthorizer/commit/006ea6d909ce7353ca44cf937e56c56d08eabb18))
```

### Comparing `pyauthorizer-0.2.8/LICENSE` & `pyauthorizer-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/PKG-INFO` & `pyauthorizer-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyauthorizer
-Version: 0.2.8
+Version: 0.2.9
 Summary: A simple authorizer for python project.
 Author-email: msclock <msclock@126.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/msclock/pyauthorizer
 Project-URL: Tracker, https://github.com/msclock/pyauthorizer/issues
 Project-URL: Documentation, https://github.com/msclock/pyauthorizer.git
 Project-URL: Source, https://github.com/msclock/pyauthorizer.git
@@ -58,15 +58,15 @@
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
 <!-- prettier-ignore-start -->
 [actions-badge]:            https://github.com/msclock/pyauthorizer/actions/workflows/ci.yml/badge.svg
 [actions-link]:             https://github.com/msclock/pyauthorizer/actions/workflows/ci.yml
 [pypi-link]:                https://pypi.org/project/pyauthorizer/
 [pypi-platforms]:           https://img.shields.io/pypi/pyversions/pyauthorizer
-[pypi-version]:             https://badge.fury.io/py/pyauthorizer.svg
+[pypi-version]:             https://img.shields.io/pypi/v/pyauthorizer?color
 <!-- prettier-ignore-end -->
 
 A simple authorizer for python project.
 
 In some cases, even for a scripting language like Python, it may be necessary to
 generate and validate tokens for specific use cases. The `pyauthorizer` provides
 a simple way to generate and validate licenses. Additionally, the built-in
```

### Comparing `pyauthorizer-0.2.8/README.md` & `pyauthorizer-0.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
 <!-- prettier-ignore-start -->
 [actions-badge]:            https://github.com/msclock/pyauthorizer/actions/workflows/ci.yml/badge.svg
 [actions-link]:             https://github.com/msclock/pyauthorizer/actions/workflows/ci.yml
 [pypi-link]:                https://pypi.org/project/pyauthorizer/
 [pypi-platforms]:           https://img.shields.io/pypi/pyversions/pyauthorizer
-[pypi-version]:             https://badge.fury.io/py/pyauthorizer.svg
+[pypi-version]:             https://img.shields.io/pypi/v/pyauthorizer?color
 <!-- prettier-ignore-end -->
 
 A simple authorizer for python project.
 
 In some cases, even for a scripting language like Python, it may be necessary to
 generate and validate tokens for specific use cases. The `pyauthorizer` provides
 a simple way to generate and validate licenses. Additionally, the built-in
```

### Comparing `pyauthorizer-0.2.8/docs/advance.md` & `pyauthorizer-0.2.9/docs/advance.md`

 * *Files 11% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 ````
 
 Assuming you’ve structured your plugin similarly to the example plugin, you can
 distribute it via PyPI.
 
 Congrats, you’ve now written and distributed your own pyauthorizer plugin!
 
-## Work as ports in nuitka
+## Work with nuitka
 
 For secure reasons, sources sometimes need to be converted to executables or
 shared modules that prevents them from being tampered with or leaked. This can
 be done with nuitka.
 
 More detailed information can be found in
 <https://msclock.gitlab.io/pytools/docs/nuitka.html>.
```

### Comparing `pyauthorizer-0.2.8/docs/api/pyauthorizer.encryptor.builtin.rst` & `pyauthorizer-0.2.9/docs/api/pyauthorizer.encryptor.builtin.rst`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/docs/api/pyauthorizer.encryptor.rst` & `pyauthorizer-0.2.9/docs/api/pyauthorizer.encryptor.rst`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/docs/api/pyauthorizer.rst` & `pyauthorizer-0.2.9/docs/api/pyauthorizer.rst`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/docs/conf.py` & `pyauthorizer-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/docs/getting_started.md` & `pyauthorizer-0.2.9/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/noxfile.py` & `pyauthorizer-0.2.9/noxfile.py`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/pyproject.toml` & `pyauthorizer-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/src/pyauthorizer/cli.py` & `pyauthorizer-0.2.9/src/pyauthorizer/cli.py`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/src/pyauthorizer/encryptor/base.py` & `pyauthorizer-0.2.9/src/pyauthorizer/encryptor/base.py`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/src/pyauthorizer/encryptor/builtin/multiple.py` & `pyauthorizer-0.2.9/src/pyauthorizer/encryptor/builtin/multiple.py`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/src/pyauthorizer/encryptor/builtin/simple.py` & `pyauthorizer-0.2.9/src/pyauthorizer/encryptor/builtin/simple.py`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/src/pyauthorizer/encryptor/interface.py` & `pyauthorizer-0.2.9/src/pyauthorizer/encryptor/interface.py`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/src/pyauthorizer/encryptor/plugin_manager.py` & `pyauthorizer-0.2.9/src/pyauthorizer/encryptor/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/src/pyauthorizer/encryptor/utils.py` & `pyauthorizer-0.2.9/src/pyauthorizer/encryptor/utils.py`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/src/pyauthorizer/exceptions.py` & `pyauthorizer-0.2.9/src/pyauthorizer/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/src/pyauthorizer.egg-info/PKG-INFO` & `pyauthorizer-0.2.9/src/pyauthorizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyauthorizer
-Version: 0.2.8
+Version: 0.2.9
 Summary: A simple authorizer for python project.
 Author-email: msclock <msclock@126.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/msclock/pyauthorizer
 Project-URL: Tracker, https://github.com/msclock/pyauthorizer/issues
 Project-URL: Documentation, https://github.com/msclock/pyauthorizer.git
 Project-URL: Source, https://github.com/msclock/pyauthorizer.git
@@ -58,15 +58,15 @@
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
 <!-- prettier-ignore-start -->
 [actions-badge]:            https://github.com/msclock/pyauthorizer/actions/workflows/ci.yml/badge.svg
 [actions-link]:             https://github.com/msclock/pyauthorizer/actions/workflows/ci.yml
 [pypi-link]:                https://pypi.org/project/pyauthorizer/
 [pypi-platforms]:           https://img.shields.io/pypi/pyversions/pyauthorizer
-[pypi-version]:             https://badge.fury.io/py/pyauthorizer.svg
+[pypi-version]:             https://img.shields.io/pypi/v/pyauthorizer?color
 <!-- prettier-ignore-end -->
 
 A simple authorizer for python project.
 
 In some cases, even for a scripting language like Python, it may be necessary to
 generate and validate tokens for specific use cases. The `pyauthorizer` provides
 a simple way to generate and validate licenses. Additionally, the built-in
```

### Comparing `pyauthorizer-0.2.8/src/pyauthorizer.egg-info/SOURCES.txt` & `pyauthorizer-0.2.9/src/pyauthorizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/tests/test_cli.py` & `pyauthorizer-0.2.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyauthorizer-0.2.8/tests/test_encryptor_utils.py` & `pyauthorizer-0.2.9/tests/test_encryptor_utils.py`

 * *Files identical despite different names*

