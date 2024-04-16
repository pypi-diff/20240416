# Comparing `tmp/yaclog-1.1.2.tar.gz` & `tmp/yaclog-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaclog-1.1.2.tar", last modified: Thu Dec 29 08:37:23 2022, max compression
+gzip compressed data, was "yaclog-1.2.0.tar", last modified: Tue Apr 16 06:51:08 2024, max compression
```

## Comparing `yaclog-1.1.2.tar` & `yaclog-1.2.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 08:37:23.386104 yaclog-1.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 08:37:23.382104 yaclog-1.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2022-12-29 08:37:01.000000 yaclog-1.1.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 08:37:23.382104 yaclog-1.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2022-12-29 08:37:01.000000 yaclog-1.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2022-12-29 08:37:01.000000 yaclog-1.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      533 2022-12-29 08:37:01.000000 yaclog-1.1.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2022-12-29 08:37:01.000000 yaclog-1.1.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34353 2022-12-29 08:37:01.000000 yaclog-1.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2022-12-29 08:37:23.386104 yaclog-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2022-12-29 08:37:01.000000 yaclog-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 08:37:23.382104 yaclog-1.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 08:37:23.382104 yaclog-1.1.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 08:37:23.382104 yaclog-1.1.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/_static/icon-128.png
--rw-r--r--   0 runner    (1001) docker     (123)      394 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/_static/icon-16.png
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/_static/icon-256.png
--rw-r--r--   0 runner    (1001) docker     (123)      586 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/_static/icon-32.png
--rw-r--r--   0 runner    (1001) docker     (123)      578 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/_static/icon-48.png
--rw-r--r--   0 runner    (1001) docker     (123)      764 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/_static/icon-64.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 08:37:23.382104 yaclog-1.1.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)       32 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    29530 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/docs_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 08:37:23.386104 yaclog-1.1.2/docs/handbook/
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/handbook/changelog_files.md
--rw-r--r--   0 runner    (1001) docker     (123)      107 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/handbook/commands.md
--rw-r--r--   0 runner    (1001) docker     (123)      926 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/handbook/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/handbook/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      956 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      760 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 08:37:23.386104 yaclog-1.1.2/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/reference/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/reference/markdown.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-29 08:37:01.000000 yaclog-1.1.2/docs/reference/version.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11027 2022-12-29 08:37:01.000000 yaclog-1.1.2/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2022-12-29 08:37:01.000000 yaclog-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-29 08:37:23.386104 yaclog-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 08:37:23.386104 yaclog-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-29 08:37:01.000000 yaclog-1.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2022-12-29 08:37:01.000000 yaclog-1.1.2/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2022-12-29 08:37:01.000000 yaclog-1.1.2/tests/test_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    13006 2022-12-29 08:37:01.000000 yaclog-1.1.2/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 08:37:23.386104 yaclog-1.1.2/yaclog/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2022-12-29 08:37:01.000000 yaclog-1.1.2/yaclog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14074 2022-12-29 08:37:01.000000 yaclog-1.1.2/yaclog/changelog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 08:37:23.386104 yaclog-1.1.2/yaclog/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-29 08:37:01.000000 yaclog-1.1.2/yaclog/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11558 2022-12-29 08:37:01.000000 yaclog-1.1.2/yaclog/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2022-12-29 08:37:01.000000 yaclog-1.1.2/yaclog/cli/cargo_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)     5663 2022-12-29 08:37:01.000000 yaclog-1.1.2/yaclog/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2022-12-29 08:37:01.000000 yaclog-1.1.2/yaclog/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 08:37:23.386104 yaclog-1.1.2/yaclog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2022-12-29 08:37:23.000000 yaclog-1.1.2/yaclog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2022-12-29 08:37:23.000000 yaclog-1.1.2/yaclog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-29 08:37:23.000000 yaclog-1.1.2/yaclog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2022-12-29 08:37:23.000000 yaclog-1.1.2/yaclog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2022-12-29 08:37:23.000000 yaclog-1.1.2/yaclog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-29 08:37:23.000000 yaclog-1.1.2/yaclog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:51:08.285368 yaclog-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:51:08.281368 yaclog-1.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-16 06:50:50.000000 yaclog-1.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:51:08.281368 yaclog-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-16 06:50:50.000000 yaclog-1.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-16 06:50:50.000000 yaclog-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-16 06:50:50.000000 yaclog-1.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-16 06:50:50.000000 yaclog-1.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34353 2024-04-16 06:50:50.000000 yaclog-1.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-04-16 06:51:08.285368 yaclog-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-16 06:50:50.000000 yaclog-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:51:08.281368 yaclog-1.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:51:08.281368 yaclog-1.2.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:51:08.281368 yaclog-1.2.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/_static/icon-128.png
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/_static/icon-16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/_static/icon-256.png
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/_static/icon-32.png
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/_static/icon-48.png
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/_static/icon-64.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:51:08.281368 yaclog-1.2.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29530 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/docs_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:51:08.281368 yaclog-1.2.0/docs/handbook/
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/handbook/changelog_files.md
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/handbook/commands.md
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/handbook/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/handbook/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:51:08.281368 yaclog-1.2.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/reference/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/reference/markdown.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-16 06:50:50.000000 yaclog-1.2.0/docs/reference/version.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11027 2024-04-16 06:50:50.000000 yaclog-1.2.0/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-16 06:50:50.000000 yaclog-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 06:51:08.285368 yaclog-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:51:08.285368 yaclog-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 06:50:50.000000 yaclog-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-16 06:50:50.000000 yaclog-1.2.0/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-04-16 06:50:50.000000 yaclog-1.2.0/tests/test_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13553 2024-04-16 06:50:50.000000 yaclog-1.2.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:51:08.285368 yaclog-1.2.0/yaclog/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-16 06:50:50.000000 yaclog-1.2.0/yaclog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14074 2024-04-16 06:50:50.000000 yaclog-1.2.0/yaclog/changelog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:51:08.285368 yaclog-1.2.0/yaclog/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 06:50:50.000000 yaclog-1.2.0/yaclog/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-04-16 06:50:50.000000 yaclog-1.2.0/yaclog/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-16 06:50:50.000000 yaclog-1.2.0/yaclog/cli/cargo_toml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-16 06:50:50.000000 yaclog-1.2.0/yaclog/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-16 06:50:50.000000 yaclog-1.2.0/yaclog/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:51:08.285368 yaclog-1.2.0/yaclog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-04-16 06:51:08.000000 yaclog-1.2.0/yaclog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-16 06:51:08.000000 yaclog-1.2.0/yaclog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 06:51:08.000000 yaclog-1.2.0/yaclog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 06:51:08.000000 yaclog-1.2.0/yaclog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-16 06:51:08.000000 yaclog-1.2.0/yaclog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 06:51:08.000000 yaclog-1.2.0/yaclog.egg-info/top_level.txt
```

### Comparing `yaclog-1.1.2/.github/workflows/python-publish.yml` & `yaclog-1.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/.gitignore` & `yaclog-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/.readthedocs.yaml` & `yaclog-1.2.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/CHANGELOG.md` & `yaclog-1.2.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # Changelog
 
 All notable changes to this project will be documented in this file
 
+## Version 1.2.0 - 2024-04-16
+
+### Added
+
+- added the `-s` option to `yaclog release` to increment arbitrary version segments 
+- added the `-n` option to `yaclog release` to create a new release instead of releasing a new one
+- added the `-y` option to `yaclog release` to answer "yes" to all confirmation dialogs. Use with caution!
+
+
 ## Version 1.1.2 - 2022-12-29
 
 ### Changed
 
 - yaclog now only tries to use git when invoked with a command that needs it, meaning most sub commands can now be used on systems without git
```

### Comparing `yaclog-1.1.2/LICENSE.md` & `yaclog-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/PKG-INFO` & `yaclog-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaclog
-Version: 1.1.2
+Version: 1.2.0
 Summary: Yet another changelog CLI tool.
 Author-email: Andrew Cassidy <drewcassidy@me.com>
 Project-URL: Source, https://github.com/drewcassidy/yaclog
 Project-URL: Changelog, https://github.com/drewcassidy/yaclog/blob/main/CHANGELOG.md
 Project-URL: Docs, https://yaclog.readthedocs.io/
 Keywords: changelog,commandline,markdown
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,16 +17,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: docs
 License-File: LICENSE.md
+Requires-Dist: Click>=7.0
+Requires-Dist: GitPython>=3
+Requires-Dist: packaging>=20
+Requires-Dist: tomlkit>=0.11
+Provides-Extra: docs
+Requires-Dist: Sphinx>=3.5; extra == "docs"
+Requires-Dist: sphinx-click>=2.7; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: myst-parser>=0.14; extra == "docs"
 
 # Yaclog 
 
 [![Documentation Status](https://readthedocs.org/projects/yaclog/badge/?version=latest)](https://yaclog.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://github.com/drewcassidy/yaclog/actions/workflows/python-publish.yml/badge.svg)](https://github.com/drewcassidy/yaclog/actions/workflows/python-publish.yml)
 [![PyPI version](https://badge.fury.io/py/yaclog.svg)](https://badge.fury.io/py/yaclog)
```

### Comparing `yaclog-1.1.2/README.md` & `yaclog-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/docs/Makefile` & `yaclog-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/docs/_static/css/custom.css` & `yaclog-1.2.0/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/docs/_static/icon-128.png` & `yaclog-1.2.0/docs/_static/icon-128.png`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/docs/_static/icon-256.png` & `yaclog-1.2.0/docs/_static/icon-256.png`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/docs/_static/icon-32.png` & `yaclog-1.2.0/docs/_static/icon-32.png`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/docs/_static/icon-48.png` & `yaclog-1.2.0/docs/_static/icon-48.png`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/docs/_static/icon-64.png` & `yaclog-1.2.0/docs/_static/icon-64.png`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/docs/_templates/layout.html` & `yaclog-1.2.0/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/docs/conf.py` & `yaclog-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/docs/docs_logo.png` & `yaclog-1.2.0/docs/docs_logo.png`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/docs/favicon.ico` & `yaclog-1.2.0/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/docs/handbook/changelog_files.md` & `yaclog-1.2.0/docs/handbook/changelog_files.md`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/docs/handbook/getting_started.md` & `yaclog-1.2.0/docs/handbook/getting_started.md`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/docs/index.md` & `yaclog-1.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/docs/make.bat` & `yaclog-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/logo.png` & `yaclog-1.2.0/logo.png`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/pyproject.toml` & `yaclog-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/tests/common.py` & `yaclog-1.2.0/tests/common.py`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/tests/test_changelog.py` & `yaclog-1.2.0/tests/test_changelog.py`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/tests/test_cli.py` & `yaclog-1.2.0/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,19 @@
             runner.invoke(cli, ['entry', '-b', 'entry number 2'])
 
             result = runner.invoke(cli, ['release', '-p'])
             check_result(self, result)
             self.assertEqual(yaclog.read(location).versions[0].name, '1.0.1')
             self.assertIn('1.0.1', result.output)
 
+            result = runner.invoke(cli, ['release', '-y', '-s', 2])
+            check_result(self, result)
+            self.assertEqual(yaclog.read(location).versions[0].name, '1.0.2')
+            self.assertIn('1.0.2', result.output)
+
             runner.invoke(cli, ['entry', '-b', 'entry number 3'])
 
             result = runner.invoke(cli, ['release', '-m'])
             check_result(self, result)
             self.assertEqual(yaclog.read(location).versions[0].name, '1.1.0')
             self.assertIn('1.1.0', result.output)
 
@@ -190,14 +195,20 @@
             self.assertIn('3.0.0rc1', result.output)
 
             result = runner.invoke(cli, ['release', '-f'])
             check_result(self, result)
             self.assertEqual(yaclog.read(location).versions[0].name, '3.0.0')
             self.assertIn('3.0.0', result.output)
 
+            result = runner.invoke(cli, ['release', '-p', '-n'])
+            check_result(self, result)
+            self.assertEqual(yaclog.read(location).versions[0].name, '3.0.1')
+            self.assertEqual(yaclog.read(location).versions[1].name, '3.0.0')
+            self.assertIn('3.0.1', result.output)
+
     def test_commit(self):
         """Test committing and tagging releases"""
         runner = CliRunner()
 
         with runner.isolated_filesystem():
             repo = git.Repo.init(os.path.join(os.curdir, 'testing'))
             os.chdir('testing')
```

### Comparing `yaclog-1.1.2/yaclog/changelog.py` & `yaclog-1.2.0/yaclog/changelog.py`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/yaclog/cli/__main__.py` & `yaclog-1.2.0/yaclog/cli/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,30 +183,36 @@
 @cli.command(short_help='Release versions.')
 @click.option('-M', '--major', 'rel_seg', flag_value=0, type=int, default=None,
               help='Increment major version number.')
 @click.option('-m', '--minor', 'rel_seg', flag_value=1, type=int,
               help='Increment minor version number.')
 @click.option('-p', '--patch', 'rel_seg', flag_value=2, type=int,
               help='Increment patch number.')
+@click.option('-s', '--segment', 'rel_seg', type=int,
+              help='Increment nth segment of the version. For example, `--segment 2` is equivalent to `--patch`')
 @click.option('-a', '--alpha', 'pre_seg', flag_value='a', type=str, default=None,
               help='Increment alpha version number.')
 @click.option('-b', '--beta', 'pre_seg', flag_value='b', type=str,
               help='Increment beta version number.')
 @click.option('-r', '--rc', 'pre_seg', flag_value='rc', type=str,
               help='Increment release candidate version number.')
 @click.option('-f', '--full', 'pre_seg', flag_value='',
               help='Clear the prerelease value creating a full release.')
 @click.option('-c', '--commit', is_flag=True,
               help='Create a git commit tagged with the new version number. '
                    'If there are no changes to commit, the current commit will be tagged instead.')
 @click.option('-C', '--cargo', '-🦀', is_flag=True,
               help='Update the version in a Rust cargo.toml manifest file.')
+@click.option('-y', '--yes', is_flag=True,
+              help='Answer "yes" to all confirmation dialogs')
+@click.option('-n', '--new', is_flag=True,
+              help = 'Create a new version instead of renaming an existing one')
 @click.argument('version_name', metavar='VERSION', type=str, default=None, required=False)
 @click.pass_obj
-def release(obj: Changelog, version_name, rel_seg, pre_seg, commit, cargo):
+def release(obj: Changelog, version_name, rel_seg, pre_seg, commit, cargo, yes, new):
     """
     Release VERSION, or a version incremented from the last release.
 
     VERSION is the name of the version to release. If VERSION is not provided but increment options are, then the most
     recent valid PEP440 version number is used instead.
 
     The most recent version in the log will be renamed (except by the --commit option) by using the VERSION as well as
@@ -214,15 +220,18 @@
     other kinds of prerelease.
     """
 
     if rel_seg is None and pre_seg is None and not version_name and not commit and not cargo:
         click.echo('Nothing to release!')
         raise click.Abort
 
-    cur_version = obj.current_version()
+    if new:
+        cur_version = obj.add_version()
+    else:
+        cur_version = obj.current_version()
     old_name = cur_version.name
 
     if version_name:
         new_name = version_name
     else:
         for v in obj.versions:
             if v.version is not None:
@@ -231,19 +240,19 @@
         else:
             new_name = '0.0.0'
 
     if rel_seg is not None or pre_seg is not None:
         new_name = yaclog.version.increment_version(new_name, rel_seg, pre_seg)
 
     if new_name != old_name:
-        if yaclog.version.is_release(old_name):
+        if yaclog.version.is_release(old_name) and not yes:
             click.confirm(
-                f"Rename release version {click.style(old_name, fg='blue')} "
-                f"to {click.style(new_name, fg='blue')}?",
-                abort=True)
+            f"Rename release version {click.style(old_name, fg='blue')} "
+            f"to {click.style(new_name, fg='blue')}?",
+            abort=True)
 
         cur_version.name = new_name
         cur_version.date = datetime.datetime.utcnow().date()
 
         obj.write()
         click.echo(f"Renamed {click.style(old_name, fg='blue')} to {click.style(new_name, fg='blue')}")
 
@@ -279,15 +288,16 @@
         message.append(f"version {click.style(new_name, fg='blue')}?")
 
         if untracked > 0:
             message.append(click.style(
                 f"You have {untracked} untracked file{'s'[:untracked]} that will not be included!",
                 fg='red', bold=True))
 
-        click.confirm(' '.join(message), abort=True)
+        if not yes:
+            click.confirm(' '.join(message), abort=True)
 
         if tracked > 0:
             commit = repo.index.commit(f'Release {cur_version.name}\n\n{cur_version.body()}')
             click.echo(f"Created commit {click.style(repo.head.commit.hexsha[0:7], fg='green')}")
         else:
             commit = repo.head.commit
```

### Comparing `yaclog-1.1.2/yaclog/cli/cargo_toml.py` & `yaclog-1.2.0/yaclog/cli/cargo_toml.py`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/yaclog/markdown.py` & `yaclog-1.2.0/yaclog/markdown.py`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/yaclog/version.py` & `yaclog-1.2.0/yaclog/version.py`

 * *Files identical despite different names*

### Comparing `yaclog-1.1.2/yaclog.egg-info/PKG-INFO` & `yaclog-1.2.0/yaclog.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaclog
-Version: 1.1.2
+Version: 1.2.0
 Summary: Yet another changelog CLI tool.
 Author-email: Andrew Cassidy <drewcassidy@me.com>
 Project-URL: Source, https://github.com/drewcassidy/yaclog
 Project-URL: Changelog, https://github.com/drewcassidy/yaclog/blob/main/CHANGELOG.md
 Project-URL: Docs, https://yaclog.readthedocs.io/
 Keywords: changelog,commandline,markdown
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,16 +17,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: docs
 License-File: LICENSE.md
+Requires-Dist: Click>=7.0
+Requires-Dist: GitPython>=3
+Requires-Dist: packaging>=20
+Requires-Dist: tomlkit>=0.11
+Provides-Extra: docs
+Requires-Dist: Sphinx>=3.5; extra == "docs"
+Requires-Dist: sphinx-click>=2.7; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: myst-parser>=0.14; extra == "docs"
 
 # Yaclog 
 
 [![Documentation Status](https://readthedocs.org/projects/yaclog/badge/?version=latest)](https://yaclog.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://github.com/drewcassidy/yaclog/actions/workflows/python-publish.yml/badge.svg)](https://github.com/drewcassidy/yaclog/actions/workflows/python-publish.yml)
 [![PyPI version](https://badge.fury.io/py/yaclog.svg)](https://badge.fury.io/py/yaclog)
```

### Comparing `yaclog-1.1.2/yaclog.egg-info/SOURCES.txt` & `yaclog-1.2.0/yaclog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

