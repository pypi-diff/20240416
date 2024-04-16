# Comparing `tmp/ppx-1.3.0.tar.gz` & `tmp/ppx-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppx-1.3.0.tar", last modified: Sat Apr 30 06:30:08 2022, max compression
+gzip compressed data, was "ppx-1.4.2.tar", last modified: Tue Apr 16 17:45:46 2024, max compression
```

## Comparing `ppx-1.3.0.tar` & `ppx-1.4.2.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-30 06:30:08.282152 ppx-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-30 06:30:08.274152 ppx-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-30 06:30:08.278152 ppx-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-04-30 06:29:52.000000 ppx-1.3.0/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (121)      853 2022-04-30 06:29:52.000000 ppx-1.3.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-04-30 06:29:52.000000 ppx-1.3.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1294 2022-04-30 06:29:52.000000 ppx-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-04-30 06:29:52.000000 ppx-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-04-30 06:29:52.000000 ppx-1.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3256 2022-04-30 06:29:52.000000 ppx-1.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     4974 2022-04-30 06:29:52.000000 ppx-1.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     3447 2022-04-30 06:29:52.000000 ppx-1.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-04-30 06:29:52.000000 ppx-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6357 2022-04-30 06:30:08.282152 ppx-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5564 2022-04-30 06:29:52.000000 ppx-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-30 06:30:08.278152 ppx-1.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     3256 2022-04-30 06:29:52.000000 ppx-1.3.0/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     4974 2022-04-30 06:29:52.000000 ppx-1.3.0/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     3447 2022-04-30 06:29:52.000000 ppx-1.3.0/docs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-04-30 06:29:52.000000 ppx-1.3.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-30 06:30:08.278152 ppx-1.3.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     3083 2022-04-30 06:29:52.000000 ppx-1.3.0/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (121)    28123 2022-04-30 06:29:52.000000 ppx-1.3.0/docs/_static/ppx_dark.png
--rw-r--r--   0 runner    (1001) docker     (121)    14258 2022-04-30 06:29:52.000000 ppx-1.3.0/docs/ann_solo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-30 06:30:08.278152 ppx-1.3.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-04-30 06:29:52.000000 ppx-1.3.0/docs/api/functions.rst
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-04-30 06:29:52.000000 ppx-1.3.0/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-04-30 06:29:52.000000 ppx-1.3.0/docs/api/massive.rst
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-04-30 06:29:52.000000 ppx-1.3.0/docs/api/pride.rst
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-04-30 06:29:52.000000 ppx-1.3.0/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3123 2022-04-30 06:29:52.000000 ppx-1.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4916 2022-04-30 06:29:52.000000 ppx-1.3.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2975 2022-04-30 06:29:52.000000 ppx-1.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4545 2022-04-30 06:29:52.000000 ppx-1.3.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-30 06:30:08.278152 ppx-1.3.0/ppx/
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-04-30 06:29:52.000000 ppx-1.3.0/ppx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2142 2022-04-30 06:29:52.000000 ppx-1.3.0/ppx/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     6077 2022-04-30 06:29:52.000000 ppx-1.3.0/ppx/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)    10021 2022-04-30 06:29:52.000000 ppx-1.3.0/ppx/ftp.py
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-04-30 06:29:52.000000 ppx-1.3.0/ppx/massive.py
--rw-r--r--   0 runner    (1001) docker     (121)     3392 2022-04-30 06:29:52.000000 ppx-1.3.0/ppx/ppx.py
--rw-r--r--   0 runner    (1001) docker     (121)     5184 2022-04-30 06:29:52.000000 ppx-1.3.0/ppx/pride.py
--rw-r--r--   0 runner    (1001) docker     (121)     8129 2022-04-30 06:29:52.000000 ppx-1.3.0/ppx/project.py
--rw-r--r--   0 runner    (1001) docker     (121)     1225 2022-04-30 06:29:52.000000 ppx-1.3.0/ppx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-30 06:30:08.282152 ppx-1.3.0/ppx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6357 2022-04-30 06:30:07.000000 ppx-1.3.0/ppx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1306 2022-04-30 06:30:08.000000 ppx-1.3.0/ppx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-30 06:30:07.000000 ppx-1.3.0/ppx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-04-30 06:30:07.000000 ppx-1.3.0/ppx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-04-30 06:30:08.000000 ppx-1.3.0/ppx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-04-30 06:30:08.000000 ppx-1.3.0/ppx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-04-30 06:29:52.000000 ppx-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-04-30 06:30:08.282152 ppx-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-04-30 06:29:52.000000 ppx-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-30 06:30:08.282152 ppx-1.3.0/static/
--rw-r--r--   0 runner    (1001) docker     (121)     8134 2022-04-30 06:29:52.000000 ppx-1.3.0/static/ppx_light.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-30 06:30:08.282152 ppx-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-30 06:29:52.000000 ppx-1.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4319 2022-04-30 06:29:52.000000 ppx-1.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-30 06:30:08.282152 ppx-1.3.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)     5039 2022-04-30 06:29:52.000000 ppx-1.3.0/tests/data/params.xml
--rw-r--r--   0 runner    (1001) docker     (121)    11126 2022-04-30 06:29:52.000000 ppx-1.3.0/tests/data/pride_files_response.json
--rw-r--r--   0 runner    (1001) docker     (121)     3690 2022-04-30 06:29:52.000000 ppx-1.3.0/tests/data/pride_project_response.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-30 06:30:08.282152 ppx-1.3.0/tests/system_tests/
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-04-30 06:29:52.000000 ppx-1.3.0/tests/system_tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-30 06:30:08.282152 ppx-1.3.0/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-30 06:29:52.000000 ppx-1.3.0/tests/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-04-30 06:29:52.000000 ppx-1.3.0/tests/unit_tests/test_cloud.py
--rw-r--r--   0 runner    (1001) docker     (121)     1556 2022-04-30 06:29:52.000000 ppx-1.3.0/tests/unit_tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3017 2022-04-30 06:29:52.000000 ppx-1.3.0/tests/unit_tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (121)     2007 2022-04-30 06:29:52.000000 ppx-1.3.0/tests/unit_tests/test_find_project.py
--rw-r--r--   0 runner    (1001) docker     (121)      969 2022-04-30 06:29:52.000000 ppx-1.3.0/tests/unit_tests/test_list_projects.py
--rw-r--r--   0 runner    (1001) docker     (121)     1941 2022-04-30 06:29:52.000000 ppx-1.3.0/tests/unit_tests/test_massive.py
--rw-r--r--   0 runner    (1001) docker     (121)     6456 2022-04-30 06:29:52.000000 ppx-1.3.0/tests/unit_tests/test_pride.py
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-04-30 06:29:52.000000 ppx-1.3.0/tests/unit_tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.650948 ppx-1.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.638948 ppx-1.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.642948 ppx-1.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-16 17:45:31.000000 ppx-1.4.2/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-16 17:45:31.000000 ppx-1.4.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-16 17:45:31.000000 ppx-1.4.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-16 17:45:31.000000 ppx-1.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-16 17:45:31.000000 ppx-1.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-16 17:45:31.000000 ppx-1.4.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-16 17:45:31.000000 ppx-1.4.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-16 17:45:31.000000 ppx-1.4.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-16 17:45:31.000000 ppx-1.4.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-16 17:45:31.000000 ppx-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-16 17:45:46.650948 ppx-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-16 17:45:31.000000 ppx-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.642948 ppx-1.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.642948 ppx-1.4.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    28123 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/_static/ppx_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14258 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/ann_solo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.646948 ppx-1.4.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/api/functions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/api/massive.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/api/pride.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.646948 ppx-1.4.2/ppx/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-16 17:45:31.000000 ppx-1.4.2/ppx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-16 17:45:31.000000 ppx-1.4.2/ppx/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-16 17:45:31.000000 ppx-1.4.2/ppx/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-04-16 17:45:31.000000 ppx-1.4.2/ppx/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-16 17:45:31.000000 ppx-1.4.2/ppx/massive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-16 17:45:31.000000 ppx-1.4.2/ppx/ppx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-04-16 17:45:31.000000 ppx-1.4.2/ppx/pride.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-04-16 17:45:31.000000 ppx-1.4.2/ppx/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-16 17:45:31.000000 ppx-1.4.2/ppx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.650948 ppx-1.4.2/ppx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-16 17:45:46.000000 ppx-1.4.2/ppx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-16 17:45:46.000000 ppx-1.4.2/ppx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:45:46.000000 ppx-1.4.2/ppx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 17:45:46.000000 ppx-1.4.2/ppx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-16 17:45:46.000000 ppx-1.4.2/ppx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 17:45:46.000000 ppx-1.4.2/ppx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-16 17:45:31.000000 ppx-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 17:45:46.650948 ppx-1.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.646948 ppx-1.4.2/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-04-16 17:45:31.000000 ppx-1.4.2/static/ppx_light.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.646948 ppx-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.646948 ppx-1.4.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/data/params.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11126 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/data/pride_files_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/data/pride_project_response.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.646948 ppx-1.4.2/tests/system_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/system_tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.650948 ppx-1.4.2/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/unit_tests/test_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/unit_tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/unit_tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/unit_tests/test_find_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/unit_tests/test_list_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/unit_tests/test_massive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/unit_tests/test_pride.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/unit_tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/unit_tests/utils.py
```

### Comparing `ppx-1.3.0/.github/workflows/publish.yml` & `ppx-1.4.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ppx-1.3.0/.gitignore` & `ppx-1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ppx-1.3.0/CHANGELOG.md` & `ppx-1.4.2/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,32 @@
 # Changelog for ppx
 
+## [Unreleased]
+
+## [1.4.2]
+### Fixed
+- Fix Test status badge.
+
+## [1.4.1]
+### Fixed
+- Updated the ReadTheDocs configuration.
+
+## [1.4.0]
+### Changed
+- Linting and formatting is now performed with Ruff.
+- Migrated to pyproject.toml based build.
+
+### Fixed
+- Fixed MassIVE FTP URLs using the MassIVE PROXI API.
+- Fixed PRIDE FTP URLs... again.
+- Updated unit tests with new PRIDE FTP URLs.
+
 ## [1.3.0] - 2022-04-39
 ### Added
-- Support for cloud provider destinations. Thanks @sooheon! 
+- Support for cloud provider destinations. Thanks @sooheon!
 
 ## [1.2.6] - 2022-03-16
 ### Fixed
 - Some PRIDE projects were still not working due to their recent URL change.
   This patch makes the our hotfix from v1.2.3 more robust.
 
 ## [1.2.5] - 2021-11-05
@@ -37,58 +57,57 @@
 ## [1.2.1] - 2021-10-11
 ### Added
 - New `file_info()` method for MassIVE projects uses the GNPS API to get
   information about the files in a project.
 
 ## [1.2.0] - 2021-09-14
 ### Added
-- New `timeout` parameter for most functions and classes. This specifies the 
+- New `timeout` parameter for most functions and classes. This specifies the
   maximum amount of time to wait for a response from the server.
 
 ### Changed
 - The backend for MassIVE now uses the GNPS API to list files and projects,
-  only falling back to scraping the FTP server on failure. This should make 
+  only falling back to scraping the FTP server on failure. This should make
   it much faster. Thanks @mwang87!
 - Files and projects are now returned in sorted order.
 
 ### Fixed
-- Poor connections with PRIDE were leading to a number of occasional errors. 
-  Multiple reconnect attempts are now tried for a wider variety of FTP 
+- Poor connections with PRIDE were leading to a number of occasional errors.
+  Multiple reconnect attempts are now tried for a wider variety of FTP
   operations.
 
 ## [1.1.1] - 2021-07-02
 ### Fixed
 - Downloading files is now more robust. ppx will now retry FTP connections up
   to 10 times if the connection was dropped or refused.
-- Partial downloads are now continued automatically by comparing the local 
+- Partial downloads are now continued automatically by comparing the local
   file size to the remote file size.
 
 ## [1.1.0] - 2021-05-18
 ### Fixed
 - The PRIDE REST API was not yielding all of the available files on the their
   FTP server for a project. We changed the backend use the FTP server directly
   instead. **Note that this may change the number, identity, and order of the
   file that were previously returned for PRIDE projects!**
 - Small documentation updates.
-  
+
 ### Added
-- Caching of the remote files and directories found for a project. If a 
+- Caching of the remote files and directories found for a project. If a
   project's `fetch` attribute is `False`, then we'll rely on this cached
   data, so long as it is available. Setting `fetch=True` will always refresh
   the data from the repository.
 
-## [1.0.0] - 2021-05-14  
-### Changed  
+## [1.0.0] - 2021-05-14
+### Changed
 - **We did a complete rework of the API!** This will break nearly all previous
   code using ppx, but greatly improves its versatility.
   See the [docs](https://ppx.readthedocs.io) for more details
 - Updated the build to align with
   [PEP517](https://www.python.org/dev/peps/pep-0517/)
-  
+
 ### Added
-- A command line interface for downloading files from PRIDE and MassIVE 
+- A command line interface for downloading files from PRIDE and MassIVE
   projects.
 - Additional unit tests.
 - A ppx logo
 - This changelog.
 - ppx is now available on bioconda!
-
```

### Comparing `ppx-1.3.0/CODE_OF_CONDUCT.md` & `ppx-1.4.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ppx-1.3.0/CONTRIBUTING.md` & `ppx-1.4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ppx-1.3.0/LICENSE` & `ppx-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ppx-1.3.0/PKG-INFO` & `ppx-1.4.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,33 @@
-Metadata-Version: 2.1
-Name: ppx
-Version: 1.3.0
-Summary: A Python interface to proteomics data repositories
-Home-page: https://github.com/wfondrie/ppx
-Author: William E. Fondrie
-Author-email: fondriew@gmail.com
-License: Apache 2.0
-Project-URL: Documentation, https://ppx.readthedocs.io
-Project-URL: Bug Tracker, https://github.com/wfondrie/ppx/issues
-Project-URL: Discussion Board, https://github.com/wfondrie/ppx/discussions
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: dev
-License-File: LICENSE
-
 <img src="static/ppx_light.svg" width=300>
 
 # A Python interface to proteomics data repositories
 
 [![conda](https://img.shields.io/conda/vn/bioconda/ppx?color=green)](http://bioconda.github.io/recipes/ppx/README.html)
 [![PyPI](https://img.shields.io/pypi/v/ppx?color=green)](https://pypi.org/project/ppx/)
-[![tests](https://github.com/wfondrie/ppx/workflows/tests/badge.svg?branch=master)](https://github.com/wfondrie/ppx/actions?query=workflow%3Atests)[![Documentation Status](https://readthedocs.org/projects/ppx/badge/?version=latest)](https://ppx.readthedocs.io/en/latest/?badge=latest)  
+[![tests](https://github.com/wfondrie/ppx/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/wfondrie/ppx/actions/workflows/tests.yml)
+[![Documentation Status](https://readthedocs.org/projects/ppx/badge/?version=latest)](https://ppx.readthedocs.io/en/latest/?badge=latest)
+
+https://github.com/wfondrie/ppx/workflows/tests/badge.svg?branch=master
 
-## Overview  
+## Overview
 ppx provides a simple, programmatic means to access proteomics data that are
 publicly available in [ProteomeXchange](http://www.proteomexchange.org) partner
 repositories. ppx allows users to easily find and download files associated
 with projects in [PRIDE](https://www.ebi.ac.uk/pride/archive/) and
 [MassIVE](https://massive.ucsd.edu/ProteoSAFe/static/massive.jsp). In doing so,
 ppx promotes the reproducible analysis of proteomics data.
 
 For full documentation and examples, visit: https://ppx.readthedocs.io
 
-## Installation  
+## Installation
 ppx requires Python 3.6+ and depends upon the
 [requests](https://docs.python-requests.org/en/master/) and
 [tqdm](https://tqdm.github.io/) Python packages. ppx and any missing
-dependencies are easily installed with `pip` or with `conda` through the 
+dependencies are easily installed with `pip` or with `conda` through the
 [bioconda](https://bioconda.github.io/index.html) channel.
 
 Install with `conda`:
 
 ``` shell
 conda install -c bioconda ppx
 ```
@@ -59,15 +40,15 @@
 
 ## Configuration
 
 By default, ppx will download project files in the `.ppx` directory under the
 current user's home directory (`~/.ppx` on Linux and MacOS). There are several
 ways to specify different data directories:
 
-1. Change the ppx data directory for all future Python sessions by setting the 
+1. Change the ppx data directory for all future Python sessions by setting the
 `PPX_DATA_DIR` environment variable to your preferred directory.
 
 2. Change the ppx data directory for a Python session using the
 `ppx.set_data_dir()` function.
 
 3. Specify a data directory for a project using the `local` argument:
 
@@ -130,15 +111,15 @@
 
 ``` Python
 >>> proj.download("README.txt")
 # [PosixPath('/Users/wfondrie/.ppx/PXD000001/README.txt')]
 ```
 
 Once we've downloaded files, ppx no longer needs an internet connection to
-retrieve a project's local data. However, you will need to specify the 
+retrieve a project's local data. However, you will need to specify the
 repository in which the project data resides. If we start a new Python
 session, we can find our previous file easily:
 
 ``` Python
 >>> import ppx
 
 >>> proj = ppx.find_project("PXD000001", repo="PRIDE")
@@ -170,9 +151,7 @@
 ```
 
 ## If you are an R user...
 
 ppx was inspired the rpx R package by Laurent Gatto. Check it out on
 [Bioconductor](http://bioconductor.org/packages/release/bioc/html/rpx.html) and
 [GitHub](https://github.com/lgatto/rpx).
-
-
```

### Comparing `ppx-1.3.0/docs/CHANGELOG.md` & `ppx-1.4.2/docs/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,32 @@
 # Changelog for ppx
 
+## [Unreleased]
+
+## [1.4.2]
+### Fixed
+- Fix Test status badge.
+
+## [1.4.1]
+### Fixed
+- Updated the ReadTheDocs configuration.
+
+## [1.4.0]
+### Changed
+- Linting and formatting is now performed with Ruff.
+- Migrated to pyproject.toml based build.
+
+### Fixed
+- Fixed MassIVE FTP URLs using the MassIVE PROXI API.
+- Fixed PRIDE FTP URLs... again.
+- Updated unit tests with new PRIDE FTP URLs.
+
 ## [1.3.0] - 2022-04-39
 ### Added
-- Support for cloud provider destinations. Thanks @sooheon! 
+- Support for cloud provider destinations. Thanks @sooheon!
 
 ## [1.2.6] - 2022-03-16
 ### Fixed
 - Some PRIDE projects were still not working due to their recent URL change.
   This patch makes the our hotfix from v1.2.3 more robust.
 
 ## [1.2.5] - 2021-11-05
@@ -37,58 +57,57 @@
 ## [1.2.1] - 2021-10-11
 ### Added
 - New `file_info()` method for MassIVE projects uses the GNPS API to get
   information about the files in a project.
 
 ## [1.2.0] - 2021-09-14
 ### Added
-- New `timeout` parameter for most functions and classes. This specifies the 
+- New `timeout` parameter for most functions and classes. This specifies the
   maximum amount of time to wait for a response from the server.
 
 ### Changed
 - The backend for MassIVE now uses the GNPS API to list files and projects,
-  only falling back to scraping the FTP server on failure. This should make 
+  only falling back to scraping the FTP server on failure. This should make
   it much faster. Thanks @mwang87!
 - Files and projects are now returned in sorted order.
 
 ### Fixed
-- Poor connections with PRIDE were leading to a number of occasional errors. 
-  Multiple reconnect attempts are now tried for a wider variety of FTP 
+- Poor connections with PRIDE were leading to a number of occasional errors.
+  Multiple reconnect attempts are now tried for a wider variety of FTP
   operations.
 
 ## [1.1.1] - 2021-07-02
 ### Fixed
 - Downloading files is now more robust. ppx will now retry FTP connections up
   to 10 times if the connection was dropped or refused.
-- Partial downloads are now continued automatically by comparing the local 
+- Partial downloads are now continued automatically by comparing the local
   file size to the remote file size.
 
 ## [1.1.0] - 2021-05-18
 ### Fixed
 - The PRIDE REST API was not yielding all of the available files on the their
   FTP server for a project. We changed the backend use the FTP server directly
   instead. **Note that this may change the number, identity, and order of the
   file that were previously returned for PRIDE projects!**
 - Small documentation updates.
-  
+
 ### Added
-- Caching of the remote files and directories found for a project. If a 
+- Caching of the remote files and directories found for a project. If a
   project's `fetch` attribute is `False`, then we'll rely on this cached
   data, so long as it is available. Setting `fetch=True` will always refresh
   the data from the repository.
 
-## [1.0.0] - 2021-05-14  
-### Changed  
+## [1.0.0] - 2021-05-14
+### Changed
 - **We did a complete rework of the API!** This will break nearly all previous
   code using ppx, but greatly improves its versatility.
   See the [docs](https://ppx.readthedocs.io) for more details
 - Updated the build to align with
   [PEP517](https://www.python.org/dev/peps/pep-0517/)
-  
+
 ### Added
-- A command line interface for downloading files from PRIDE and MassIVE 
+- A command line interface for downloading files from PRIDE and MassIVE
   projects.
 - Additional unit tests.
 - A ppx logo
 - This changelog.
 - ppx is now available on bioconda!
-
```

### Comparing `ppx-1.3.0/docs/CODE_OF_CONDUCT.md` & `ppx-1.4.2/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ppx-1.3.0/docs/CONTRIBUTING.md` & `ppx-1.4.2/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ppx-1.3.0/docs/Makefile` & `ppx-1.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ppx-1.3.0/docs/_static/custom.css` & `ppx-1.4.2/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ppx-1.3.0/docs/_static/ppx_dark.png` & `ppx-1.4.2/docs/_static/ppx_dark.png`

 * *Files identical despite different names*

### Comparing `ppx-1.3.0/docs/ann_solo.ipynb` & `ppx-1.4.2/docs/ann_solo.ipynb`

 * *Files identical despite different names*

### Comparing `ppx-1.3.0/docs/api/index.rst` & `ppx-1.4.2/docs/api/index.rst`

 * *Files identical despite different names*

### Comparing `ppx-1.3.0/docs/conf.py` & `ppx-1.4.2/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-# -*- coding: utf-8 -*-
 #
 # Configuration file for the Sphinx documentation builder.
 #
 # This file does only contain a selection of the most common options. For a
 # full list see the documentation:
 # http://www.sphinx-doc.org/en/master/config
 
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
-import sys
 import subprocess
+import sys
 
 sys.path.insert(0, os.path.abspath(".."))
 
 try:
     import numpydoc
 except ModuleNotFoundError:
     subprocess.run(["pip", "install", "numpydoc"], check=True)
```

### Comparing `ppx-1.3.0/docs/examples.rst` & `ppx-1.4.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `ppx-1.3.0/docs/index.rst` & `ppx-1.4.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ppx-1.3.0/docs/usage.rst` & `ppx-1.4.2/docs/usage.rst`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 As of ppx v1.3.0, cloud paths can also be used as the data directory. This
 allows you to stream downloaded files to AWS S3, Google Cloud Storage, or Azure
 Blob Storage. To use a cloud storage provider, simply set the data directory to
 a cloud URI, such as :code:`s3://my-data-bucket/ppx` using any of the methods
 above. Please note that you'll also need to setup credentials for your cloud
 provider---see the `CloudPathLib documentation
-<https://cloudpathlib.drivendata.org/v0.6/authentication/>_` for details.
+<https://cloudpathlib.drivendata.org/v0.6/authentication/>`_ for details.
 
 Examples
 --------
 
 To begin, we first import the ppx package:
 
     >>> import ppx
@@ -84,15 +84,15 @@
 For more details about the available methods for a project, see our Python API
 documentation for the :py:class:`~ppx.PrideProject` and
 :py:class:`~ppx.MassiveProject` classes.
 
 Using Cloud Storage
 +++++++++++++++++++
 
-We use `CloudPathlib <https://cloudpathlib.drivendata.org/stable/>_` to power
+We use `CloudPathlib <https://cloudpathlib.drivendata.org/stable/>`_ to power
 support for AWS S3, Google Cloud Storage, and Azure Blob Storage. To use a
 cloud storage provider, create the bucket for ppx to use and set it as the ppx
 data directory.
 
 For example using AWS S3, we can save the files of a project to an S3 bucket:
 
     >>> proj = ppx.find_project("PXD000001", local="s3://my-bucket/PXD000001")
```

### Comparing `ppx-1.3.0/ppx/__init__.py` & `ppx-1.4.2/ppx/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """See the README for detailed documentation and examples."""
+
 try:
-    from importlib.metadata import version, PackageNotFoundError
+    from importlib.metadata import PackageNotFoundError, version
 
     try:
         __version__ = version(__name__)
     except PackageNotFoundError:
         pass
 
 except ImportError:
-    from pkg_resources import get_distribution, DistributionNotFound
+    from pkg_resources import DistributionNotFound, get_distribution
 
     try:
         __version__ = get_distribution(__name__).version
     except DistributionNotFound:
         pass
 
-from . import pride
-from . import massive
+from . import massive, pride
+from .config import get_data_dir, set_data_dir
 from .factory import find_project
-from .pride import PrideProject
 from .massive import MassiveProject
-from .config import get_data_dir, set_data_dir
+from .pride import PrideProject
```

### Comparing `ppx-1.3.0/ppx/config.py` & `ppx-1.4.2/ppx/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """This module contains the configuration details for ppx"""
-import os
+
 import logging
+import os
 from pathlib import Path
 
 from cloudpathlib import AnyPath
 
 LOGGER = logging.getLogger(__name__)
 
 
 class PPXConfig:
     """Configure the data directory for ppx
 
     Attributes
     ----------
     path : pathlib.Path object
+
     """
 
     def __init__(self):
         """Initialize the _PPXDataDir"""
         self._path = None
         self.path = os.getenv("PPX_DATA_DIR")
 
@@ -57,14 +59,15 @@
         path : str
             The path to resolve.
 
         Returns
         -------
         Path or CloudPath
             The resolved path.
+
         """
         path = AnyPath(path)
         try:
             path = path.expanduser().resolve()
         except AttributeError:
             pass
 
@@ -79,13 +82,14 @@
 def set_data_dir(path=None):
     """Set the ppx data directory.
 
     Parameters
     ----------
     path : str or pathlib.Path object, optional
         The path for ppx to use as its data directory.
+
     """
     config.path = path
 
 
 # Initialize the configuration when loaded:
 config = PPXConfig()
```

### Comparing `ppx-1.3.0/ppx/factory.py` & `ppx-1.4.2/ppx/factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+"""The PXDataset class and its associated methods.
+
+This is the foundation of the ppx package.
 """
-This module contains the PXDataset class and its associated methods,
-which are the foundation of the ppx package.
-"""
-import re
+
 import logging
+import re
 from urllib.parse import urlparse
 
 import requests
 
-from .pride import PrideProject
 from .massive import MassiveProject
+from .pride import PrideProject
 
 LOGGER = logging.getLogger(__name__)
 
 
 class PXDFactory:
     """Retrieve information about a ProteomeXchange project.
 
@@ -25,14 +26,15 @@
         The local data directory in which the project files will be
         downloaded. In addition to local paths, paths to AWS S3,
         Google Cloud Storage, or Azure Blob Storage can be used.
     fetch : bool, optional
         Should ppx check the remote repository for updated metadata?
     timeout : float, optional
         The maximum amount of time to wait for a server response.
+
     """
 
     rest = "http://proteomecentral.proteomexchange.org/cgi/GetDataset"
 
     repo_cv = {
         "MS:1002487": "MassIVE",
         "MS:1002632": "jPOST",
@@ -73,19 +75,19 @@
     @property
     def id(self):
         """The ProteomeXchange project identifier"""
         return self._id
 
     def find(self):
         """Find the dataset at the partner repository"""
-        kwargs = dict(
-            local=self._local,
-            fetch=self._fetch,
-            timeout=self._timeout,
-        )
+        kwargs = {
+            "local": self._local,
+            "fetch": self._fetch,
+            "timeout": self._timeout,
+        }
 
         if self._repo == "PRIDE":
             return PrideProject(self._repo_id, **kwargs)
 
         if self._repo == "MassIVE":
             return MassiveProject(self._repo_id, **kwargs)
 
@@ -152,21 +154,22 @@
     timeout : float, optional
         The maximum amount of time to wait for a server response
 
     Returns
     -------
     :py:class:`~ppx.PrideProject` or :py:class:`~ppx.MassiveProject`
         An object to interact with the project data in the repository.
+
     """
     identifier = str(identifier).upper()
     if repo is not None:
         repo = str(repo).lower()
 
     # User-specified:
-    kwargs = dict(local=local, fetch=fetch, timeout=timeout)
+    kwargs = {"local": local, "fetch": fetch, "timeout": timeout}
     if repo == "pride":
         return PrideProject(identifier, **kwargs)
 
     if repo == "massive":
         return MassiveProject(identifier, **kwargs)
 
     if repo is not None:
```

### Comparing `ppx-1.3.0/ppx/ftp.py` & `ppx-1.4.2/ppx/ftp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """General utilities for working with the repository FTP sites."""
+
 import logging
 import re
 import socket
-from ftplib import FTP, error_temp, error_perm
+from ftplib import FTP, error_perm, error_temp
 from functools import partial
 
 from cloudpathlib import CloudPath
 from cloudpathlib.exceptions import OverwriteNewerCloudError
 from tqdm.auto import tqdm
 
 from .utils import listify
@@ -47,14 +48,15 @@
         The url for the FTP connection.
     max_depth : int, optional
         The maximum resursion depth when looking for files.
     max_reconnects : int, optional
         The maximum number of reconnects to attempt during downloads.
     timeout : float, optional
         The maximum amount of time to wait for a response from the server.
+
     """
 
     def __init__(self, url, max_depth=4, max_reconnects=10, timeout=10.0):
         """Initialize an FTPParser"""
         if not url.startswith("ftp://"):
             raise ValueError("The URL does not appear to be an FTP server")
 
@@ -93,17 +95,17 @@
         """Try and execute a function, reconnecting on failure."""
         for _ in range(self.max_reconnects):
             try:
                 self._connect()
                 return func(*args, **kwargs)
 
             except (
+                TimeoutError,
                 ConnectionRefusedError,
                 ConnectionResetError,
-                socket.timeout,
                 socket.gaierror,
                 socket.herror,
                 error_temp,
                 error_perm,
                 EOFError,
                 OSError,
             ) as err:
@@ -127,14 +129,15 @@
             The file to download.
         out_file : pathlib.Path object
             The local file.
         silent : bool
             Disable the progress bar?
         force_ : bool
             Force the file to be redownloaded, even if it exists.
+
         """
         self.connect()
         size = self.connection.size(remote_file)
         pbar = tqdm(
             desc=str(remote_file),
             total=size,
             position=1,
@@ -178,14 +181,15 @@
         force_ : bool
             Force the file to be overwritten?
 
         Returns
         -------
         file object
             The opened for the file.
+
         """
         open_kwargs = {"mode": "wb+" if force_ else "ab+"}
         if isinstance(out_file, CloudPath):
             open_kwargs["force_overwrite_to_cloud"] = force_
 
         return out_file.open(**open_kwargs)
 
@@ -196,14 +200,15 @@
         ----------
         fname : str
             The remote file name.
         fhandle : file object
             The opened file object where the data will be written.
         pbar : tqdm.tqdm
             The tqdm progress bar to update.
+
         """
         write = partial(write_file, fhandle=fhandle, pbar=pbar)
         self.connection.retrbinary(f"RETR {fname}", write, rest=fhandle.tell())
         pbar.close()
 
     def _get_files(self):
         """Recursively list files from the FTP connection."""
@@ -239,14 +244,15 @@
             The file(s) to download.
         dest_dir : pathlib.Path or cloudpathlib.CloudPath object
             The destination directory. Can be a cloud storage bucket.
         force_ : bool
             Force the files to be redownloaded, even they already exist.
         silent : bool
             Disable the progress bar?
+
         """
         files = listify(files)
         out_files = []
         overall_pbar = partial(
             tqdm,
             desc="TOTAL",
             position=0,
@@ -298,21 +304,22 @@
 
 
 def parse_response(conn):
     """Parse the FTP server response.
 
     Parameters
     ----------
-    url : str
-        The url of the FTP server.
+    conn : Connection
+        The FTP server connection
 
     Returns
     -------
     files : list of str
     directories : list of str
+
     """
     lines = []
     conn.dir(lines.append)
 
     files = []
     dirs = []
     for line in lines:
@@ -337,12 +344,13 @@
     -------
     is_dir : bool
         Whether or not the line is a directory.
     name : str
         The file or directory name.
     date : date
         The modification date.
+
     """
     match = UNIX.fullmatch(line)
     is_dir = match[1] == "d" or match[1] == "l"
     name = match[8]
     return name, is_dir
```

### Comparing `ppx-1.3.0/ppx/massive.py` & `ppx-1.4.2/ppx/massive.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """MassIVE datasets."""
+
+import logging
 import re
 import socket
-import logging
-import xml.etree.ElementTree as ET
+import xml.etree.ElementTree as ET  # noqa: N817
 from pathlib import Path
 
 import requests
 
 from .ftp import FTPParser
 from .project import BaseProject
 
@@ -37,49 +38,65 @@
     local : Path object
     url : str
     title : str
     description : str
     metadata : dict
     fetch : bool
     timeout : float
+
     """
 
     _api = "https://gnps-datasetcache.ucsd.edu/datasette/database/filename.csv"
+    _proxy_api = "https://massive.ucsd.edu/ProteoSAFe/proxi/v0.1/datasets/"
 
     def __init__(self, msv_id, local=None, fetch=False, timeout=10.0):
         """Instantiate a MSVDataset object"""
         super().__init__(msv_id, local, fetch, timeout)
-        self._url = f"ftp://massive.ucsd.edu/{self.id}"
-        self._params = dict(
-            _stream="on",
-            _sort="filepath",
-            dataset__exact=self.id,
-            _size="max",
-        )
+        self._params = {
+            "_stream": "on",
+            "_sort": "filepath",
+            "dataset__exact": self.id,
+            "_size": "max",
+        }
 
     def _validate_id(self, identifier):
         """Validate a MassIVE identifier.
 
         Parameters
         ----------
         identifier : str
             The project identifier to validate.
 
         Returns
         -------
         str
             The validated identifier.
+
         """
         identifier = str(identifier).upper()
         if not re.match("(MSV|RMSV)[0-9]{9}", identifier):
             raise ValueError("Malformed MassIVE identifier.")
 
         return identifier
 
     @property
+    def url(self):
+        """The FTP URL of the dataset."""
+        if self._url is not None:
+            return self._url
+
+        res = requests.get(self._proxy_api + self.id, timeout=self.timeout)
+        for link in res.json()["datasetLink"]:
+            if link["accession"] == "MS:1002852":
+                self._url = link["value"]
+                return self._url
+
+        raise ValueError(f"No FTP link was found for {self.id}")
+
+    @property
     def metadata(self):
         """The project metadata as a dictionary."""
         if self._metadata is None:
             remote_file = "ccms_parameters/params.xml"
             metadata_file = self.local / remote_file
             try:
                 # Only fetch file if it doesn't exist and self.fetch is true:
@@ -118,26 +135,27 @@
             Use Unix wildcards to return specific files. For example,
             :code:`"*.mzML"` would return all of the mzML files.
 
         Returns
         -------
         list of str
             The remote files available for this project.
+
         """
         if self.fetch or self._remote_files is None:
             try:
                 info = self.file_info().splitlines()[1:]
                 self._remote_files = [
                     r.split(",")[0].split("/", 1)[1] for r in info
                 ]
                 assert self._remote_files
             except (
+                TimeoutError,
                 ConnectionRefusedError,
                 ConnectionResetError,
-                socket.timeout,
                 socket.gaierror,
                 socket.herror,
                 EOFError,
                 OSError,
                 AssertionError,
             ):
                 LOGGER.debug("Scraping the FTP server for files...")
@@ -153,14 +171,15 @@
     def file_info(self):
         """Retrieve information about the project files.
 
         Returns
         -------
         str
             Information about the files in a CSV format.
+
         """
         file_info_path = self.local / ".file_info.csv"
         if file_info_path.exists() and not self.fetch:
             with file_info_path.open("r") as ref:
                 return ref.read()
 
         res = requests.get(
@@ -188,28 +207,29 @@
     timeout : float, optional
         The maximum amount of time to wait for a response from the server.
 
     Returns
     -------
     list of str
         A list of MassIVE identifiers.
+
     """
     url = "https://gnps-datasetcache.ucsd.edu/datasette/database.csv"
-    params = dict(sql="select distinct dataset from filename", _size="max")
+    params = {"sql": "select distinct dataset from filename", "_size": "max"}
     try:
         res = requests.get(url, params, timeout=timeout).text.splitlines()[1:]
         res.sort()
         return res
 
     except (
+        TimeoutError,
         ConnectionRefusedError,
         ConnectionResetError,
-        socket.timeout,
         socket.gaierror,
         socket.herror,
         EOFError,
         OSError,
     ):
         LOGGER.debug("Scraping the FTP server for projects...")
 
-    parser = FTPParser("ftp://massive.ucsd.edu/", max_depth=0, timeout=timeout)
-    return parser.dirs
+    parser = FTPParser("ftp://massive.ucsd.edu/", max_depth=1, timeout=timeout)
+    return [d.split("/")[1] for d in parser.dirs if "/" in d]
```

### Comparing `ppx-1.3.0/ppx/ppx.py` & `ppx-1.4.2/ppx/ppx.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """The command line entry point for ppx"""
-import sys
+
 import logging
-from pathlib import Path
+import sys
 from argparse import ArgumentParser
+from pathlib import Path
 
-from . import __version__
-from . import find_project
+from . import __version__, find_project
 
 LOGGER = logging.getLogger(__name__)
 
 
 def get_parser():
     """Parse the command line arguments"""
-    desc = f"""Use this command line utility to download files from the PRIDE and MassIVE
-    proteomics repositories. The paths to the downloaded files are written to
-    stdout."""
+    desc = """Use this command line utility to download files from the PRIDE
+    and MassIVE proteomics repositories. The paths to the downloaded files are
+    written to stdout."""
 
     epilog = "More documentation and examples at: https://ppx.readthedocs.io"
     parser = ArgumentParser(description=desc, epilog=epilog)
 
     parser.add_argument(
         "identifier",
         type=str,
@@ -92,15 +92,15 @@
     proj = find_project(args.identifier, args.local, timeout=args.timeout)
     remote_files = proj.remote_files()
 
     if len(args.files) > 0:
         matches = set()
         passed = []
         for pat in args.files:
-            pat_match = set(f for f in remote_files if Path(f).match(pat))
+            pat_match = {f for f in remote_files if Path(f).match(pat)}
             passed.append(bool(pat_match))
             matches.update(pat_match)
 
         if not all(passed):
             failed = "  \n".join(
                 [f for f, p in zip(args.files, passed) if not p]
             )
```

### Comparing `ppx-1.3.0/ppx/pride.py` & `ppx-1.4.2/ppx/pride.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """A class for PRIDE datasets"""
-import re
+
 import json
+import re
 
 import requests
 
 from . import utils
 from .project import BaseProject
 
 
@@ -35,14 +36,15 @@
     description : str
     doi : str
     data_processing_protocol : str
     sample_processing_protocol : str
     metadata : dict
     fetch : bool
     timeout : float
+
     """
 
     rest = "https://www.ebi.ac.uk/pride/ws/archive/v2/projects/"
     file_rest = "https://www.ebi.ac.uk/pride/ws/archive/v2/files/byProject"
 
     def __init__(self, pride_id, local=None, fetch=False, timeout=10.0):
         """Instantiate a PrideDataset object"""
@@ -57,27 +59,31 @@
         identifier : str
             The project identifier to validate.
 
         Returns
         -------
         str
             The validated identifier
+
         """
         identifier = str(identifier).upper()
         if not re.match("P[RX]D[0-9]{6}", identifier):
             raise ValueError("Malformed PRIDE identifier.")
 
         return identifier
 
     @property
     def url(self):
         """The FTP address associated with this project."""
         if self._url is None:
             url = self.metadata["_links"]["datasetFtpUrl"]["href"]
 
+            # For whatever reason, this is added now mistakenly to some URLs...
+            url = url.replace("/generated", "")
+
             # Fix PRIDE URLs (Issue #18)
             fixes = [("", ""), ("/data/", "-"), ("pride.", "")]
             for fix in fixes:
                 url = url.replace(*fix)
                 try:
                     self._url = utils.test_url(url)
                 except requests.HTTPError as err:
@@ -160,14 +166,15 @@
     timeout : float, optional
         The maximum amount of time to wait for a response from the server.
 
     Returns
     -------
     list of str
         A list of PRIDE identifiers.
+
     """
     url = "https://www.ebi.ac.uk/pride/ws/archive/v2/misc/sitemap"
     res = requests.get(url, timeout=timeout)
     if res.status_code != 200:
         raise requests.HTTPError(f"Error {res.status_code}: {res.text})")
 
     res = [p.split("/")[-1] for p in res.text.splitlines()]
```

### Comparing `ppx-1.3.0/ppx/project.py` & `ppx-1.4.2/ppx/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """A base dataset class"""
-from pathlib import Path
+
 from abc import ABC, abstractmethod
+from pathlib import Path
 
 from cloudpathlib import AnyPath
 
 from . import utils
 from .config import config
 from .ftp import FTPParser
 
@@ -131,14 +132,15 @@
             Use Unix wildcards to return specific files. For example,
             :code:`"*peak"` would return all directories ending in "peak".
 
         Returns
         -------
         list of str
             The remote directories available for this project.
+
         """
         if self.fetch or self._remote_dirs is None:
             self._remote_dirs = self._parser.dirs
 
         if glob is not None:
             dirs = [d for d in self._remote_dirs if Path(d).match(glob)]
         else:
@@ -155,14 +157,15 @@
             Use Unix wildcards to return specific files. For example,
             :code:`"*.mzML"` would return all of the mzML files.
 
         Returns
         -------
         list of str
             The remote files available for this project.
+
         """
         if self.fetch or self._remote_files is None:
             self._remote_files = self._parser.files
 
         if glob is not None:
             files = [f for f in self._remote_files if Path(f).match(glob)]
         else:
@@ -179,14 +182,15 @@
             Use Unix wildcards to return specific files. For example,
             :code:`"*peak"` would return all directories ending in "peak".
 
         Returns
         -------
         list of str
             The local directories available for this project.
+
         """
         return [d for d in utils.glob(self.local, glob) if d.is_dir()]
 
     def local_files(self, glob=None):
         """List the local files associated with this project.
 
         Parameters
@@ -195,14 +199,15 @@
             Use Unix wildcards to return specific files. For example,
             :code:`"*.mzML"` would return all of the mzML files.
 
         Returns
         -------
         list of str
             The local files available for this project.
+
         """
         return [f for f in utils.glob(self.local, glob) if f.is_file()]
 
     def download(self, files, force_=False, silent=False):
         """Download files from the remote repository.
 
         These files are downloaded to this project's local data directory
@@ -252,14 +257,15 @@
     fetch : bool
         Overide the cached file if True
 
     Returns
     -------
     list of str
         The newly cached or loaded files.
+
     """
     if not fetch and files is None:
         if cache_file.exists():
             with cache_file.open() as ref:
                 return ref.read().splitlines()
         else:
             return None
```

### Comparing `ppx-1.3.0/ppx/utils.py` & `ppx-1.4.2/ppx/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 """Utility Functions"""
-from pathlib import Path
 
 import requests
-from cloudpathlib import CloudPath
-from cloudpathlib.exceptions import CloudPathNotImplementedError
 
 
 def listify(obj):
     """Turn an object into a list, but don't split strings"""
     try:
         assert not isinstance(obj, str)
         iter(obj)
@@ -25,14 +22,15 @@
     url : str
         The URL to test.
 
     Returns
     -------
     str
         The input URL.
+
     """
     http_url = url.replace("ftp://", "http://")
     if http_url[-1] != "/":
         http_url += "/"
 
     res = requests.head(http_url)
     if res.status_code != 200:
@@ -51,10 +49,11 @@
     pattern : str, optional
         The glob pattern.
 
     Returns
     -------
     list of Path or CloudPath
         The sorted list of files.
+
     """
     pattern = "**/[!.]*" if pattern is None else pattern
     return sorted(path.glob(pattern))
```

### Comparing `ppx-1.3.0/ppx.egg-info/SOURCES.txt` & `ppx-1.4.2/ppx.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 .readthedocs.yml
 CHANGELOG.md
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
-setup.py
-.github/workflows/black.yml
+.github/workflows/lint.yml
 .github/workflows/publish.yml
 .github/workflows/tests.yml
 docs/CHANGELOG.md
 docs/CODE_OF_CONDUCT.md
 docs/CONTRIBUTING.md
 docs/Makefile
 docs/ann_solo.ipynb
@@ -54,8 +52,9 @@
 tests/unit_tests/test_cloud.py
 tests/unit_tests/test_config.py
 tests/unit_tests/test_download.py
 tests/unit_tests/test_find_project.py
 tests/unit_tests/test_list_projects.py
 tests/unit_tests/test_massive.py
 tests/unit_tests/test_pride.py
+tests/unit_tests/test_utils.py
 tests/unit_tests/utils.py
```

### Comparing `ppx-1.3.0/static/ppx_light.svg` & `ppx-1.4.2/static/ppx_light.svg`

 * *Files identical despite different names*

### Comparing `ppx-1.3.0/tests/conftest.py` & `ppx-1.4.2/tests/conftest.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 We need:
 - To set the PPX_DATA_DIR environment variable to a temporary directory
 - A mock GET response from PRIDE
 - A mock GET response from ProteomeXchange
 - A mock FTP server response from PRIDE
 - A mock FTP server response from MassIVE
 """
+
+import ftplib
 import json
 import socket
-import ftplib
 
 import pytest
 import requests
-
 from cloudpathlib import implementation_registry
 from cloudpathlib.local import (
     LocalS3Client,
     LocalS3Path,
     local_s3_implementation,
 )
 
-
 import ppx
 
+
 # Set the PPX_DATA_DIRECTORY --------------------------------------------------
 @pytest.fixture(autouse=True)
 def ppx_data_dir(monkeypatch, tmp_path):
     """Set the PPX_DATA_DIR environment variable"""
     monkeypatch.setenv("PPX_DATA_DIR", str(tmp_path))
     ppx.set_data_dir()
```

### Comparing `ppx-1.3.0/tests/data/params.xml` & `ppx-1.4.2/tests/data/params.xml`

 * *Files identical despite different names*

### Comparing `ppx-1.3.0/tests/data/pride_files_response.json` & `ppx-1.4.2/tests/data/pride_files_response.json`

 * *Files identical despite different names*

### Comparing `ppx-1.3.0/tests/data/pride_project_response.json` & `ppx-1.4.2/tests/data/pride_project_response.json`

 * *Files identical despite different names*

### Comparing `ppx-1.3.0/tests/system_tests/test_cli.py` & `ppx-1.4.2/tests/system_tests/test_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 """Test the command line interface"""
-import subprocess
-from pathlib import Path
 
-import pytest
+import subprocess
 
 PXID = "PXD000001"
 MSVID = "MSV000087408"
 
 
 # pytest.mark.skip(reason="PRIDE conneciton instability")
 def test_pride(tmp_path):
     """Test the CLI for pride"""
     out_dir = tmp_path / PXID
     cmd = ["ppx", "-l", str(out_dir), "-t", "10", PXID, "*.txt"]
     subprocess.run(cmd, check=True)
-    print(list(out_dir.iterdir()))
 
 
 def test_massive(tmp_path):
     """Test the CLI for massive"""
     out_dir = tmp_path / MSVID
     cmd = ["ppx", "-l", str(out_dir), MSVID, "*/statistics.tsv"]
     subprocess.run(cmd, check=True)
```

### Comparing `ppx-1.3.0/tests/unit_tests/test_cloud.py` & `ppx-1.4.2/tests/unit_tests/test_cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Test using cloud locations"""
+
 from cloudpathlib import CloudPath
+
 import ppx
 
 from . import utils
 
 MSVID = "MSV000087408"
```

### Comparing `ppx-1.3.0/tests/unit_tests/test_config.py` & `ppx-1.4.2/tests/unit_tests/test_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Test the configuration"""
-import os
+
 from pathlib import Path
 
 import pytest
-import ppx
 from cloudpathlib import CloudPath
 
+import ppx
+
 PXID = "PXD000001"
 
 
 def test_reset_dir(monkeypatch):
     """Test resetting the data directory"""
     monkeypatch.delenv("PPX_DATA_DIR")
     ppx.set_data_dir()
```

### Comparing `ppx-1.3.0/tests/unit_tests/test_download.py` & `ppx-1.4.2/tests/unit_tests/test_download.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 """Test the download functionality of ppx
 
 These tests are in a separate file because they all require internet access.
 """
+
 from ftplib import FTP, error_temp
 
 import pytest
+
 import ppx
 
 from . import utils
 
 PXID = "PXD000001"
 MSVID = "MSV000087408"
 RMSVID = "RMSV000000253"
 
 
 def test_no_internet(monkeypatch):
     """Test what happens when connection is blocked"""
     proj = ppx.PrideProject(PXID, timeout=None)
-    remote_files = proj.remote_files()
+    proj.remote_files()
     fname = "F063721.dat-mztab.txt"
 
     def retrbinary(*args, **kwargs):
         raise OSError("Mock error")
 
     monkeypatch.setattr(FTP, "retrbinary", retrbinary)
     with pytest.raises(error_temp):
-        txt = proj.download(fname)
+        proj.download(fname)
 
 
 def test_pride_download(tmp_path):
     """Test downloading data from PRIDE"""
     proj = ppx.PrideProject(PXID)
     files = proj.local_files()
     assert files == []
@@ -61,26 +63,30 @@
     remote_files = proj.remote_files()
     assert len(remote_files) == 12
 
     remote_files = proj.remote_files("*.mzTab")
     assert len(remote_files) == 1
 
     proj.fetch = False
-    info = [l for l in proj.file_info().splitlines() if l]
+    info = [a for a in proj.file_info().splitlines() if a]
     assert len(info) == 13
 
     proj = ppx.MassiveProject(MSVID, fetch=True)
     proj._api = "blah"
     remote_files = proj.remote_files()
     assert len(remote_files) == 12
 
     # Keep this to test for HTTPErrors
     proj._api = "https://api.github.com/user"  # A dummy URL...
     proj.remote_files()
 
+
+@pytest.mark.skip("MassIVE API is currently broken for renalyses.")
+def test_massive_reanalysis(tmp_path):
+    """Test reanalyses."""
     proj = ppx.MassiveProject(RMSVID, fetch=True)
     remote_files = proj.remote_files("2019-06-03_mnchoi_64a990d7/**/*")
     assert len(remote_files) == 10
 
 
 def test_massive_download(tmp_path):
     """Test downloading data from massive"""
```

### Comparing `ppx-1.3.0/tests/unit_tests/test_find_project.py` & `ppx-1.4.2/tests/unit_tests/test_find_project.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Test finding projects"""
-import pytest
-import ppx
 
+import pytest
 from requests.exceptions import ConnectTimeout, ReadTimeout
 
+import ppx
+
 PXID = "PXD000001"
 MSVID = "MSV000087408"
 MSVPXD = "PXD025981"
 
 
 def test_pride_offline(block_internet, tmp_path):
     """Test pride project offline functionality"""
@@ -39,28 +40,29 @@
 
     proj = ppx.find_project(MSVID, fetch=True, repo="massive")
     assert proj.fetch
 
 
 # The following require internet access! --------------------------------------
 def test_pride_online():
-    """Test pride project resolution"""
+    """Test pride project resolution."""
     proj = ppx.find_project(PXID, timeout=10)
     assert isinstance(proj, ppx.PrideProject)
 
 
 def test_massive_project():
-    """Test massive project resolution"""
+    """Test massive project resolution."""
     proj = ppx.find_project(MSVID, timeout=10)
     assert isinstance(proj, ppx.MassiveProject)
 
 
 def test_massive_project_with_pxd():
+    """Test finding massive project with a PXD."""
     proj = ppx.find_project(MSVPXD, timeout=10)
     assert isinstance(proj, ppx.MassiveProject)
     assert proj.id == MSVID
 
 
 def test_timeout():
     """Try a value that is too small."""
     with pytest.raises((ConnectTimeout, ReadTimeout)):
-        proj = ppx.find_project(PXID, timeout=0.0000000000001)
+        ppx.find_project(PXID, timeout=0.0000000000001)
```

### Comparing `ppx-1.3.0/tests/unit_tests/test_list_projects.py` & `ppx-1.4.2/tests/unit_tests/test_list_projects.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Test that the list_projects() functions work"""
+
 import pytest
-import ppx
 import requests
 
+import ppx
+
 
 def test_pride():
     """Test that we can get pride projects"""
     proj = ppx.pride.list_projects()
     assert len(proj) > 10000
     assert all((p.startswith("PXD") or p.startswith("PRD")) for p in proj)
```

### Comparing `ppx-1.3.0/tests/unit_tests/test_massive.py` & `ppx-1.4.2/tests/unit_tests/test_massive.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Test MassIVE functionality w/o internet access"""
+
 import shutil
 from pathlib import Path
 
 import pytest
+
 import ppx
 
 MSVID = "MSV000087408"
 
 
 def test_init(tmp_path):
     """Test initialization"""
     proj = ppx.MassiveProject(MSVID)
-    url = "ftp://massive.ucsd.edu/MSV000087408"
+    url = f"ftp://massive.ucsd.edu/v03/{MSVID}"
     assert proj.id == MSVID
     assert proj.url == url
-    assert proj.local == tmp_path / "MSV000087408"
+    assert proj.local == tmp_path / MSVID
     assert not proj.fetch
 
     with pytest.raises(ValueError):
         ppx.MassiveProject("MSV;MaLiCiOuScOdE!")
 
     with pytest.raises(ValueError):
         ppx.MassiveProject("PXD0000087408")
```

### Comparing `ppx-1.3.0/tests/unit_tests/test_pride.py` & `ppx-1.4.2/tests/unit_tests/test_pride.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """Test PRIDE functionality w/o internet access"""
+
 import json
 from pathlib import Path
 
 import pytest
+import requests
+
 import ppx
 
 PXID = "PXD000001"
 
 
 def test_init(tmp_path):
     """Test initialization"""
     proj = ppx.PrideProject(PXID)
-    url = "ftp://ftp.pride.ebi.ac.uk/pride-archive/2012/03/PXD000001"
+    url = "ftp://ftp.pride.ebi.ac.uk/pride/data/archive/2012/03/PXD000001"
     assert proj.id == PXID
     assert proj.url == url
     assert proj.url == url  # Do again to get from cache
     assert proj.local == tmp_path / "PXD000001"
     assert not proj.fetch
 
     with pytest.raises(ValueError):
@@ -118,15 +121,14 @@
         "generated/PRIDE_Exp_Complete_Ac_22134.pride.mgf.gz",
         "generated/PRIDE_Exp_Complete_Ac_22134.pride.mztab.gz",
     ]
 
     assert files == true_files
 
     gzipped = proj.remote_files("*.gz")
-    print(gzipped)
     true_gzipped = [
         "PRIDE_Exp_Complete_Ac_22134.xml.gz",
         "PRIDE_Exp_mzData_Ac_22134.xml.gz",
         "generated/PRIDE_Exp_Complete_Ac_22134.pride.mgf.gz",
         "generated/PRIDE_Exp_Complete_Ac_22134.pride.mztab.gz",
     ]
     assert gzipped == true_gzipped
@@ -138,15 +140,15 @@
         "TMT_Erwinia_1uLSike_Top10HCD_isol2_45stepped_60min_01.mzXML",
         "TMT_Erwinia_1uLSike_Top10HCD_isol2_45stepped_60min_01.raw",
     ]
     assert ms_files == true_ms_files
     assert proj.remote_files("blah") == []
 
 
-def test_remote_files(mock_pride_project_response):
+def test_remote_dirs(mock_pride_project_response):
     """Test that listing remote directories works"""
     proj = ppx.PrideProject(PXID)
     dirs = proj.remote_dirs()
     assert dirs == ["generated"]
 
 
 def test_cached_remote_files(tmp_path, mock_pride_project_response):
@@ -193,7 +195,24 @@
     assert res == [f for f in local_files[0] if str(f).endswith("mzML")]
 
     res = proj.local_files("*.mzML")
     assert res == [tmp_path / "test_file.mzML"]
 
     res = proj.local_dirs("*0")
     assert res == [tmp_path / "test_dir0"]
+
+
+def test_broken_pride_links(tmp_path, monkeypatch):
+    """Test other types of links that PRIDE might use."""
+    proj = ppx.PrideProject(PXID)
+    url = "ftp://ftp.ebi.ac.uk/pride-archive/2012/03/PXD000001"
+    _ = proj.metadata
+
+    # Monkey patch test_url:
+    def mock_test_url(url):
+        if "ftp.ebi.ac.uk" not in url:
+            raise requests.HTTPError
+
+        return url
+
+    monkeypatch.setattr(ppx.utils, "test_url", mock_test_url)
+    assert proj.url == url
```

