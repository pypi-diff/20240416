# Comparing `tmp/emtl-0.1.0.tar.gz` & `tmp/emtl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emtl-0.1.0.tar", last modified: Thu Apr 11 14:46:06 2024, max compression
+gzip compressed data, was "emtl-0.1.1.tar", last modified: Tue Apr 16 09:38:57 2024, max compression
```

## Comparing `emtl-0.1.0.tar` & `emtl-0.1.1.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-11 14:46:06.979384 emtl-0.1.0/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      729 2024-04-11 14:14:37.000000 emtl-0.1.0/.bumpversion.cfg
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1930 2024-04-11 14:36:46.000000 emtl-0.1.0/.cookiecutterrc
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      172 2024-04-11 14:14:37.000000 emtl-0.1.0/.coveragerc
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      353 2024-04-11 14:14:37.000000 emtl-0.1.0/.editorconfig
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-11 14:46:06.979384 emtl-0.1.0/.github/
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-11 14:46:06.979384 emtl-0.1.0/.github/workflows/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     5643 2024-04-11 14:14:50.000000 emtl-0.1.0/.github/workflows/github-actions.yml
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      686 2024-04-11 14:16:44.000000 emtl-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      282 2024-04-11 14:14:37.000000 emtl-0.1.0/.readthedocs.yml
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       65 2024-04-11 14:14:37.000000 emtl-0.1.0/AUTHORS.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       86 2024-04-11 14:14:37.000000 emtl-0.1.0/CHANGELOG.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2274 2024-04-11 14:14:37.000000 emtl-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1112 2024-04-11 14:18:48.000000 emtl-0.1.0/LICENSE
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      427 2024-04-11 14:14:37.000000 emtl-0.1.0/MANIFEST.in
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2145 2024-04-11 14:46:06.979384 emtl-0.1.0/PKG-INFO
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2271 2024-04-11 14:14:37.000000 emtl-0.1.0/README.rst
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-11 14:46:06.979384 emtl-0.1.0/ci/
--rwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)     2867 2024-04-11 14:14:37.000000 emtl-0.1.0/ci/bootstrap.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       72 2024-04-11 14:14:37.000000 emtl-0.1.0/ci/requirements.txt
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-11 14:46:06.979384 emtl-0.1.0/ci/templates/
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-11 14:46:06.979384 emtl-0.1.0/ci/templates/.github/
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-11 14:46:06.979384 emtl-0.1.0/ci/templates/.github/workflows/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1965 2024-04-11 14:14:37.000000 emtl-0.1.0/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-11 14:46:06.979384 emtl-0.1.0/docs/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       28 2024-04-11 14:14:37.000000 emtl-0.1.0/docs/authors.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       30 2024-04-11 14:14:37.000000 emtl-0.1.0/docs/changelog.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      987 2024-04-11 14:14:37.000000 emtl-0.1.0/docs/conf.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       33 2024-04-11 14:14:37.000000 emtl-0.1.0/docs/contributing.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      244 2024-04-11 14:14:37.000000 emtl-0.1.0/docs/index.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       84 2024-04-11 14:14:37.000000 emtl-0.1.0/docs/installation.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       27 2024-04-11 14:14:37.000000 emtl-0.1.0/docs/readme.rst
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-11 14:46:06.979384 emtl-0.1.0/docs/reference/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      146 2024-04-11 14:14:37.000000 emtl-0.1.0/docs/reference/emtl.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       56 2024-04-11 14:14:37.000000 emtl-0.1.0/docs/reference/index.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       17 2024-04-11 14:14:37.000000 emtl-0.1.0/docs/requirements.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      109 2024-04-11 14:14:37.000000 emtl-0.1.0/docs/spelling_wordlist.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       98 2024-04-11 14:14:37.000000 emtl-0.1.0/docs/usage.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1352 2024-04-11 14:14:37.000000 emtl-0.1.0/pyproject.toml
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1174 2024-04-11 14:14:37.000000 emtl-0.1.0/pytest.ini
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       38 2024-04-11 14:46:06.979384 emtl-0.1.0/setup.cfg
--rwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)     2807 2024-04-11 14:14:37.000000 emtl-0.1.0/setup.py
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-11 14:46:06.979384 emtl-0.1.0/src/
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-11 14:46:06.979384 emtl-0.1.0/src/emtl/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       71 2024-04-11 14:14:37.000000 emtl-0.1.0/src/emtl/__init__.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      354 2024-04-11 14:14:37.000000 emtl-0.1.0/src/emtl/__main__.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      954 2024-04-11 14:14:37.000000 emtl-0.1.0/src/emtl/cli.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       45 2024-04-11 14:14:37.000000 emtl-0.1.0/src/emtl/core.py
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-11 14:46:06.979384 emtl-0.1.0/src/emtl/tests/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-11 14:14:37.000000 emtl-0.1.0/src/emtl/tests/__init__.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      123 2024-04-11 14:14:37.000000 emtl-0.1.0/src/emtl/tests/test_cli.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       85 2024-04-11 14:14:37.000000 emtl-0.1.0/src/emtl/tests/test_core.py
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-11 14:46:06.979384 emtl-0.1.0/src/emtl.egg-info/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2145 2024-04-11 14:46:06.000000 emtl-0.1.0/src/emtl.egg-info/PKG-INFO
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      927 2024-04-11 14:46:06.000000 emtl-0.1.0/src/emtl.egg-info/SOURCES.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        1 2024-04-11 14:46:06.000000 emtl-0.1.0/src/emtl.egg-info/dependency_links.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       37 2024-04-11 14:46:06.000000 emtl-0.1.0/src/emtl.egg-info/entry_points.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        1 2024-04-11 14:24:57.000000 emtl-0.1.0/src/emtl.egg-info/not-zip-safe
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        5 2024-04-11 14:46:06.000000 emtl-0.1.0/src/emtl.egg-info/top_level.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1695 2024-04-11 14:14:37.000000 emtl-0.1.0/tox.ini
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-16 09:38:57.053691 emtl-0.1.1/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      757 2024-04-16 09:19:18.000000 emtl-0.1.1/.bumpversion.cfg
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1901 2024-04-16 09:19:18.000000 emtl-0.1.1/.cookiecutterrc
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      149 2024-04-16 01:27:17.000000 emtl-0.1.1/.coveragerc
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      353 2024-04-16 01:27:17.000000 emtl-0.1.1/.editorconfig
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-16 09:38:57.053691 emtl-0.1.1/.github/
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-16 09:38:57.053691 emtl-0.1.1/.github/workflows/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2774 2024-04-16 07:03:41.000000 emtl-0.1.1/.github/workflows/github-actions.yml
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      734 2024-04-16 01:37:37.000000 emtl-0.1.1/.gitignore
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      686 2024-04-16 01:27:59.000000 emtl-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      282 2024-04-16 01:27:17.000000 emtl-0.1.1/.readthedocs.yml
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       65 2024-04-16 01:27:17.000000 emtl-0.1.1/AUTHORS.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       86 2024-04-16 01:27:17.000000 emtl-0.1.1/CHANGELOG.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2274 2024-04-16 01:27:17.000000 emtl-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1117 2024-04-16 01:42:17.000000 emtl-0.1.1/LICENSE
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1912 2024-04-16 09:38:57.053691 emtl-0.1.1/PKG-INFO
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2245 2024-04-16 09:19:18.000000 emtl-0.1.1/README.rst
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-16 09:38:57.053691 emtl-0.1.1/ci/
+-rwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)     2867 2024-04-16 01:27:17.000000 emtl-0.1.1/ci/bootstrap.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       72 2024-04-16 01:27:17.000000 emtl-0.1.1/ci/requirements.txt
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-16 09:38:57.053691 emtl-0.1.1/ci/templates/
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-16 09:38:57.053691 emtl-0.1.1/ci/templates/.github/
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-16 09:38:57.053691 emtl-0.1.1/ci/templates/.github/workflows/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2179 2024-04-16 01:27:17.000000 emtl-0.1.1/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-16 09:38:57.053691 emtl-0.1.1/docs/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       28 2024-04-16 01:27:17.000000 emtl-0.1.1/docs/authors.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       30 2024-04-16 01:27:17.000000 emtl-0.1.1/docs/changelog.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1109 2024-04-16 09:19:18.000000 emtl-0.1.1/docs/conf.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       33 2024-04-16 01:27:17.000000 emtl-0.1.1/docs/contributing.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      244 2024-04-16 01:27:17.000000 emtl-0.1.1/docs/index.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       84 2024-04-16 01:27:17.000000 emtl-0.1.1/docs/installation.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       27 2024-04-16 01:27:17.000000 emtl-0.1.1/docs/readme.rst
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-16 09:38:57.053691 emtl-0.1.1/docs/reference/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      146 2024-04-16 01:27:17.000000 emtl-0.1.1/docs/reference/emtl.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       56 2024-04-16 01:27:17.000000 emtl-0.1.1/docs/reference/index.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       17 2024-04-16 01:27:17.000000 emtl-0.1.1/docs/requirements.txt
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      109 2024-04-16 01:27:17.000000 emtl-0.1.1/docs/spelling_wordlist.txt
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       98 2024-04-16 01:27:17.000000 emtl-0.1.1/docs/usage.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1381 2024-04-16 01:27:17.000000 emtl-0.1.1/pyproject.toml
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1303 2024-04-16 01:27:17.000000 emtl-0.1.1/pytest.ini
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       38 2024-04-16 09:38:57.053691 emtl-0.1.1/setup.cfg
+-rwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)     2987 2024-04-16 09:19:18.000000 emtl-0.1.1/setup.py
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-16 09:38:57.053691 emtl-0.1.1/src/
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-16 09:38:57.053691 emtl-0.1.1/src/emtl/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       71 2024-04-16 09:19:18.000000 emtl-0.1.1/src/emtl/__init__.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      354 2024-04-16 01:27:17.000000 emtl-0.1.1/src/emtl/__main__.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      411 2024-04-16 09:38:57.000000 emtl-0.1.1/src/emtl/_version.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      954 2024-04-16 01:27:17.000000 emtl-0.1.1/src/emtl/cli.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       45 2024-04-16 01:27:17.000000 emtl-0.1.1/src/emtl/core.py
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-16 09:38:57.053691 emtl-0.1.1/src/emtl/tests/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-16 01:27:17.000000 emtl-0.1.1/src/emtl/tests/__init__.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      123 2024-04-16 01:27:17.000000 emtl-0.1.1/src/emtl/tests/test_cli.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       85 2024-04-16 01:27:17.000000 emtl-0.1.1/src/emtl/tests/test_core.py
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-16 09:38:57.053691 emtl-0.1.1/src/emtl.egg-info/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1912 2024-04-16 09:38:57.000000 emtl-0.1.1/src/emtl.egg-info/PKG-INFO
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      947 2024-04-16 09:38:57.000000 emtl-0.1.1/src/emtl.egg-info/SOURCES.txt
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        1 2024-04-16 09:38:57.000000 emtl-0.1.1/src/emtl.egg-info/dependency_links.txt
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       38 2024-04-16 09:38:57.000000 emtl-0.1.1/src/emtl.egg-info/entry_points.txt
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        1 2024-04-16 09:34:21.000000 emtl-0.1.1/src/emtl.egg-info/not-zip-safe
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        5 2024-04-16 09:38:57.000000 emtl-0.1.1/src/emtl.egg-info/top_level.txt
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1637 2024-04-16 06:27:08.000000 emtl-0.1.1/tox.ini
```

### Comparing `emtl-0.1.0/.bumpversion.cfg` & `emtl-0.1.1/.bumpversion.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [bumpversion]
-current_version = 0.1.0
+current_version = 0.1.1
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
-search = version="{current_version}"
-replace = version="{new_version}"
+search = "fallback_version": "{current_version}"
+replace = "fallback_version": "{new_version}"
 
 [bumpversion:file (badge):README.rst]
 search = /v{current_version}.svg
 replace = /v{new_version}.svg
 
 [bumpversion:file (link):README.rst]
-search = /v{current_version}...main
-replace = /v{new_version}...main
+search = /v{current_version}...master
+replace = /v{new_version}...master
 
 [bumpversion:file:docs/conf.py]
 search = version = release = "{current_version}"
 replace = version = release = "{new_version}"
 
 [bumpversion:file:src/emtl/__init__.py]
 search = __version__ = "{current_version}"
```

### Comparing `emtl-0.1.0/.cookiecutterrc` & `emtl-0.1.1/.cookiecutterrc`

 * *Files 9% similar despite different names*

```diff
@@ -27,35 +27,35 @@
     distribution_name: "emtl"
     email: "riiyzhou@gmail.com"
     formatter_quote_style: "double"
     full_name: "Eastmoney Trade Library"
     function_name: "emt"
     github_actions: "yes"
     github_actions_osx: "yes"
-    github_actions_windows: "yes"
+    github_actions_windows: "no"
     license: "MIT license"
     module_name: "core"
     package_name: "emtl"
     pre_commit: "yes"
     project_name: "emtl"
-    project_short_description: "An example package. Generated with cookiecutter-pylibrary."
+    project_short_description: "东方财富交易系统"
     pypi_badge: "yes"
     pypi_disable_upload: "no"
     release_date: "today"
     repo_hosting: "github.com"
     repo_hosting_domain: "github.com"
-    repo_main_branch: "main"
+    repo_main_branch: "master"
     repo_name: "emtl"
     repo_username: "riiy"
     scrutinizer: "no"
-    setup_py_uses_setuptools_scm: "no"
+    setup_py_uses_setuptools_scm: "yes"
     sphinx_docs: "yes"
     sphinx_docs_hosting: "https://emtl.readthedocs.io/"
     sphinx_doctest: "no"
     sphinx_theme: "furo"
-    test_matrix_separate_coverage: "no"
+    test_matrix_separate_coverage: "yes"
     tests_inside_package: "yes"
-    version: 0.1.0
+    version: "0.1.0"
     version_manager: "bump2version"
     website: "riiy.gihub.io/emtl"
     year_from: "2024"
-    year_to: "2024"
+    year_to: "2025"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `emtl-0.1.0/.pre-commit-config.yaml` & `emtl-0.1.1/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 #   pre-commit install --install-hooks
 # To update the versions:
 #   pre-commit autoupdate
 exclude: '^(\.tox|ci/templates|\.bumpversion\.cfg)(/|$)'
 # Note the order is intentional to avoid multiple passes of the hooks
 repos:
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.5
+    rev: v0.3.7
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix, --show-fixes]
   - repo: https://github.com/psf/black
-    rev: 24.3.0
+    rev: 24.4.0
     hooks:
       - id: black
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.6.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
```

### Comparing `emtl-0.1.0/CONTRIBUTING.rst` & `emtl-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `emtl-0.1.0/LICENSE` & `emtl-0.1.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 MIT License
 
-Copyright (c) 2024, Eastmoney Trade Library
+Copyright (c) 2024-2025, Eastmoney Trade Library
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice (including the next paragraph) shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `emtl-0.1.0/README.rst` & `emtl-0.1.1/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     :target: https://readthedocs.org/projects/emtl/
     :alt: Documentation Status
 
 .. |github-actions| image:: https://github.com/riiy/emtl/actions/workflows/github-actions.yml/badge.svg
     :alt: GitHub Actions Build Status
     :target: https://github.com/riiy/emtl/actions
 
-.. |codecov| image:: https://codecov.io/gh/riiy/emtl/branch/main/graphs/badge.svg?branch=main
+.. |codecov| image:: https://codecov.io/gh/riiy/emtl/branch/master/graphs/badge.svg?branch=master
     :alt: Coverage Status
     :target: https://app.codecov.io/github/riiy/emtl
 
 .. |version| image:: https://img.shields.io/pypi/v/emtl.svg
     :alt: PyPI Package latest release
     :target: https://pypi.org/project/emtl
 
@@ -37,36 +37,36 @@
     :alt: Supported versions
     :target: https://pypi.org/project/emtl
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/emtl.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/emtl
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/riiy/emtl/v0.1.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/riiy/emtl/v0.1.1.svg
     :alt: Commits since latest release
-    :target: https://github.com/riiy/emtl/compare/v0.1.0...main
+    :target: https://github.com/riiy/emtl/compare/v0.1.1...master
 
 
 
 .. end-badges
 
-An example package. Generated with cookiecutter-pylibrary.
+东方财富交易系统
 
 * Free software: MIT license
 
 Installation
 ============
 
 ::
 
     pip install emtl
 
 You can also install the in-development version with::
 
-    pip install https://github.com/riiy/emtl/archive/main.zip
+    pip install https://github.com/riiy/emtl/archive/master.zip
 
 
 Documentation
 =============
 
 
 https://emtl.readthedocs.io/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `emtl-0.1.0/ci/bootstrap.py` & `emtl-0.1.1/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `emtl-0.1.0/ci/templates/.github/workflows/github-actions.yml` & `emtl-0.1.1/ci/templates/.github/workflows/github-actions.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name: build
-on: [push, pull_request]
+on: [push, pull_request, workflow_dispatch]
 jobs:
   test:
     name: {{ '${{ matrix.name }}' }}
     runs-on: {{ '${{ matrix.os }}' }}
     timeout-minutes: 30
     strategy:
       fail-fast: false
@@ -28,15 +28,14 @@
 {% else %}
 {% set python %}{{ prefix[2] }}.{{ prefix[3:] }}{% endset %}
 {% set cpython %}cp{{ prefix[2:] }}{% endset %}
 {% set toxpython %}python{{ prefix[2] }}.{{ prefix[3:] }}{% endset %}
 {% endif %}
 {% for os, python_arch in [
     ['ubuntu', 'x64'],
-    ['windows', 'x64'],
     ['macos', 'x64'],
 ] %}
           - name: '{{ env }} ({{ os }})'
             python: '{{ python }}'
             toxpython: '{{ toxpython }}'
             python_arch: '{{ python_arch }}'
             tox_env: '{{ env }}'
@@ -59,7 +58,15 @@
         tox --version
         pip list --format=freeze
     - name: test
       env:
         TOXPYTHON: '{{ '${{ matrix.toxpython }}' }}'
       run: >
         tox -e {{ '${{ matrix.tox_env }}' }} -v
+  finish:
+    needs: test
+    if: {{ '${{ always() }}' }}
+    runs-on: ubuntu-latest
+    steps:
+    - uses: codecov/codecov-action@v3
+      with:
+        CODECOV_TOKEN: {% raw %}${{ secrets.CODECOV_TOKEN }}{% endraw %}
```

### Comparing `emtl-0.1.0/docs/conf.py` & `emtl-0.1.1/docs/conf.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,34 +8,40 @@
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
     "sphinx.ext.viewcode",
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "emtl"
-year = "2024"
+year = "2024-2025"
 author = "Eastmoney Trade Library"
 copyright = f"{year}, {author}"
-version = release = "0.1.0"
+try:
+    from pkg_resources import get_distribution
+
+    version = release = get_distribution("emtl").version
+except Exception:
+    import traceback
+
+    traceback.print_exc()
+    version = release = "0.1.1"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
-    "issue": ("https://github.com/riiy/emtl/issues/%s", "#"),
-    "pr": ("https://github.com/riiy/emtl/pull/%s", "PR #"),
+    "issue": ("https://github.com/riiy/emtl/issues/%s", "#%s"),
+    "pr": ("https://github.com/riiy/emtl/pull/%s", "PR #%s"),
 }
 
+html_theme = "furo"
 html_theme_options = {
     "githuburl": "https://github.com/riiy/emtl/",
 }
 
 html_use_smartypants = True
 html_last_updated_fmt = "%b %d, %Y"
 html_split_index = False
-html_sidebars = {
-    "**": ["searchbox.html", "globaltoc.html", "sourcelink.html"],
-}
 html_short_title = f"{project}-{version}"
 
 napoleon_use_ivar = True
 napoleon_use_rtype = False
 napoleon_use_param = False
```

### Comparing `emtl-0.1.0/pyproject.toml` & `emtl-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [build-system]
 requires = [
     "setuptools>=30.3.0",
+    "setuptools_scm>=3.3.1",
 ]
 
 [tool.ruff]
 extend-exclude = ["static", "ci/templates"]
 line-length = 140
 src = ["src", "tests"]
 target-version = "py38"
```

### Comparing `emtl-0.1.0/pytest.ini` & `emtl-0.1.1/pytest.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 [pytest]
 # If a pytest section is found in one of the possible config files
 # (pytest.ini, tox.ini or setup.cfg), then pytest will not look for any others,
 # so if you add a pytest config section elsewhere,
 # you will need to delete this section from setup.cfg.
 norecursedirs =
+    .git
+    .tox
+    .env
+    dist
+    build
     migrations
 
 python_files =
     test_*.py
     *_test.py
     tests.py
 addopts =
     -ra
     --strict-markers
+    --ignore=docs/conf.py
+    --ignore=setup.py
+    --ignore=ci
+    --ignore=.eggs
     --doctest-modules
     --doctest-glob=\*.rst
     --tb=short
     --pyargs
 # The order of these options matters. testpaths comes after addopts so that
 # emtl in testpaths is interpreted as
 # --pyargs emtl.
```

### Comparing `emtl-0.1.0/setup.py` & `emtl-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,69 +9,79 @@
 def read(*names, **kwargs):
     with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get("encoding", "utf8")) as fh:
         return fh.read()
 
 
 setup(
     name="emtl",
-    version="0.1.0",
+    use_scm_version={
+        "local_scheme": "dirty-tag",
+        "write_to": "src/emtl/_version.py",
+        "fallback_version": "0.1.1",
+    },
     license="MIT",
-    description="An example package. Generated with cookiecutter-pylibrary.",
+    description="东方财富交易系统",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
     author="Eastmoney Trade Library",
     author_email="riiyzhou@gmail.com",
     url="https://github.com/riiy/emtl",
     packages=find_packages("src"),
     package_dir={"": "src"},
     py_modules=[path.stem for path in Path("src").glob("*.py")],
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         # complete classifier list: http://pypi.python.org/pypi?%3Aaction=list_classifiers
-        "Development Status :: 5 - Production/Stable",
+        "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: Unix",
         "Operating System :: POSIX",
-        "Operating System :: Microsoft :: Windows",
+        # "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
+        # "Programming Language :: Python :: 3.8",
+        # "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Programming Language :: Python :: Implementation :: PyPy",
+        # "Programming Language :: Python :: Implementation :: PyPy",
         # uncomment if you test on these interpreters:
         # "Programming Language :: Python :: Implementation :: IronPython",
         # "Programming Language :: Python :: Implementation :: Jython",
         # "Programming Language :: Python :: Implementation :: Stackless",
         "Topic :: Utilities",
     ],
     project_urls={
         "Documentation": "https://emtl.readthedocs.io/",
         "Changelog": "https://emtl.readthedocs.io/en/latest/changelog.html",
         "Issue Tracker": "https://github.com/riiy/emtl/issues",
     },
     keywords=[
-        # eg: "keyword1", "keyword2", "keyword3",
+        "trade",
+        "东方财富",
+        "股票",
+        "交易",
     ],
     python_requires=">=3.8",
     install_requires=[
         # eg: "aspectlib==1.1.1", "six>=1.7",
     ],
     extras_require={
         # eg:
         #   "rst": ["docutils>=0.11"],
         #   ":python_version=='3.8'": ["backports.zoneinfo"],
     },
+    setup_requires=[
+        "setuptools_scm>=3.3.1",
+    ],
     entry_points={
         "console_scripts": [
             "emt = emtl.cli:run",
         ]
     },
 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `emtl-0.1.0/src/emtl/cli.py` & `emtl-0.1.1/src/emtl/cli.py`

 * *Files identical despite different names*

### Comparing `emtl-0.1.0/src/emtl.egg-info/SOURCES.txt` & `emtl-0.1.1/src/emtl.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 .bumpversion.cfg
 .cookiecutterrc
 .coveragerc
 .editorconfig
+.gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
-MANIFEST.in
 README.rst
 pyproject.toml
 pytest.ini
 setup.py
 tox.ini
 .github/workflows/github-actions.yml
 ci/bootstrap.py
@@ -28,14 +28,15 @@
 docs/requirements.txt
 docs/spelling_wordlist.txt
 docs/usage.rst
 docs/reference/emtl.rst
 docs/reference/index.rst
 src/emtl/__init__.py
 src/emtl/__main__.py
+src/emtl/_version.py
 src/emtl/cli.py
 src/emtl/core.py
 src/emtl.egg-info/PKG-INFO
 src/emtl.egg-info/SOURCES.txt
 src/emtl.egg-info/dependency_links.txt
 src/emtl.egg-info/entry_points.txt
 src/emtl.egg-info/not-zip-safe
```

### Comparing `emtl-0.1.0/tox.ini` & `emtl-0.1.1/tox.ini`

 * *Files 20% similar despite different names*

```diff
@@ -10,57 +10,56 @@
 
 ; a generative tox configuration, see: https://tox.wiki/en/latest/user_guide.html#generative-environments
 [tox]
 envlist =
     clean,
     check,
     docs,
-    {py38,py39,py310,py311,py312,pypy38,pypy39,pypy310},
+    {py310,py311,py312}-{cover,nocov},
     report
 ignore_basepython_conflict = true
 
 [testenv]
 basepython =
-    pypy38: {env:TOXPYTHON:pypy3.8}
-    pypy39: {env:TOXPYTHON:pypy3.9}
-    pypy310: {env:TOXPYTHON:pypy3.10}
-    py38: {env:TOXPYTHON:python3.8}
-    py39: {env:TOXPYTHON:python3.9}
     py310: {env:TOXPYTHON:python3.10}
     py311: {env:TOXPYTHON:python3.11}
     py312: {env:TOXPYTHON:python3.12}
     {bootstrap,clean,check,report,docs,codecov}: {env:TOXPYTHON:python3}
 setenv =
     PYTHONPATH={toxinidir}/tests
     PYTHONUNBUFFERED=yes
 passenv =
     *
-usedevelop = false
+usedevelop =
+    cover: true
+    nocov: false
 deps =
     pytest
-    pytest-cov
+    cover: pytest-cov
 commands =
-    {posargs:pytest --cov --cov-report=term-missing --cov-report=xml -vv }
+    nocov: {posargs:pytest -vv --ignore=src}
+    cover: {posargs:pytest --cov --cov-report=term-missing --cov-report=xml -vv}
 
 [testenv:check]
 deps =
     docutils
-    check-manifest
     pre-commit
     readme-renderer
     pygments
     isort
+    setuptools-scm
 skip_install = true
 commands =
     python setup.py check --strict --metadata --restructuredtext
-    check-manifest .
     pre-commit run --all-files --show-diff-on-failure
 
 [testenv:docs]
 usedevelop = true
+install_command =
+    python -m pip install --no-use-pep517 {opts} {packages}
 deps =
     -r{toxinidir}/docs/requirements.txt
 commands =
     sphinx-build {posargs:-E} -b html docs dist/docs
     sphinx-build -b linkcheck docs dist/docs
 
 [testenv:report]
```

