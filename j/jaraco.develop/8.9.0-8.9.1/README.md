# Comparing `tmp/jaraco.develop-8.9.0.tar.gz` & `tmp/jaraco.develop-8.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.develop-8.9.0.tar", last modified: Tue Mar 26 02:20:23 2024, max compression
+gzip compressed data, was "jaraco.develop-8.9.1.tar", last modified: Tue Mar 26 02:37:00 2024, max compression
```

## Comparing `jaraco.develop-8.9.0.tar` & `jaraco.develop-8.9.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:20:23.380009 jaraco.develop-8.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:20:23.372008 jaraco.develop-8.9.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:20:23.372008 jaraco.develop-8.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-03-26 02:20:23.380009 jaraco.develop-8.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:20:23.372008 jaraco.develop-8.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:20:23.368008 jaraco.develop-8.9.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:20:23.380009 jaraco.develop-8.9.0/jaraco/develop/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/jaraco/develop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/jaraco/develop/add-github-secret.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/jaraco/develop/add-github-secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/jaraco/develop/checkout-all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/jaraco/develop/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/jaraco/develop/cpython-sync.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/jaraco/develop/create-github-release.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/jaraco/develop/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/jaraco/develop/finalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     5953 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/jaraco/develop/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/jaraco/develop/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/jaraco/develop/indent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/jaraco/develop/init-azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/jaraco/develop/macos-build-python.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/jaraco/develop/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/jaraco/develop/print-meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/jaraco/develop/projects-run.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/jaraco/develop/pypi.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/jaraco/develop/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/jaraco/develop/rst-header-replace.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/jaraco/develop/rtd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/jaraco/develop/towncrier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/jaraco/develop/update-projects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:20:23.380009 jaraco.develop-8.9.0/jaraco.develop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-03-26 02:20:23.000000 jaraco.develop-8.9.0/jaraco.develop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-26 02:20:23.000000 jaraco.develop-8.9.0/jaraco.develop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 02:20:23.000000 jaraco.develop-8.9.0/jaraco.develop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-26 02:20:23.000000 jaraco.develop-8.9.0/jaraco.develop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-26 02:20:23.000000 jaraco.develop-8.9.0/jaraco.develop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-26 02:20:23.380009 jaraco.develop-8.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/todo.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-03-26 02:20:07.000000 jaraco.develop-8.9.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:37:00.231188 jaraco.develop-8.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:37:00.223188 jaraco.develop-8.9.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:37:00.223188 jaraco.develop-8.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-03-26 02:37:00.231188 jaraco.develop-8.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:37:00.223188 jaraco.develop-8.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:37:00.219188 jaraco.develop-8.9.1/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:37:00.227188 jaraco.develop-8.9.1/jaraco/develop/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/jaraco/develop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/jaraco/develop/add-github-secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/jaraco/develop/add-github-secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/jaraco/develop/checkout-all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/jaraco/develop/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/jaraco/develop/cpython-sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/jaraco/develop/create-github-release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/jaraco/develop/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/jaraco/develop/finalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5953 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/jaraco/develop/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/jaraco/develop/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/jaraco/develop/indent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/jaraco/develop/init-azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/jaraco/develop/macos-build-python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/jaraco/develop/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/jaraco/develop/print-meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/jaraco/develop/projects-run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/jaraco/develop/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/jaraco/develop/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/jaraco/develop/rst-header-replace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/jaraco/develop/rtd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/jaraco/develop/towncrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/jaraco/develop/update-projects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 02:37:00.227188 jaraco.develop-8.9.1/jaraco.develop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-03-26 02:37:00.000000 jaraco.develop-8.9.1/jaraco.develop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-26 02:37:00.000000 jaraco.develop-8.9.1/jaraco.develop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 02:37:00.000000 jaraco.develop-8.9.1/jaraco.develop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-26 02:37:00.000000 jaraco.develop-8.9.1/jaraco.develop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-26 02:37:00.000000 jaraco.develop-8.9.1/jaraco.develop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-26 02:37:00.231188 jaraco.develop-8.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/todo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-03-26 02:36:42.000000 jaraco.develop-8.9.1/tox.ini
```

### Comparing `jaraco.develop-8.9.0/.github/workflows/main.yml` & `jaraco.develop-8.9.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.9.0/LICENSE` & `jaraco.develop-8.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.9.0/NEWS.rst` & `jaraco.develop-8.9.1/NEWS.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v8.9.1
+======
+
+Bugfixes
+--------
+
+- In projects-run, flush stdout.
+
+
 v8.9.0
 ======
 
 Features
 --------
 
 - In projects-run, implemented selection and exclusion logic for tags and keywords.
```

### Comparing `jaraco.develop-8.9.0/PKG-INFO` & `jaraco.develop-8.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.develop
-Version: 8.9.0
+Version: 8.9.1
 Summary: Development utilities by jaraco
 Home-page: https://github.com/jaraco/jaraco.develop
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jaraco.develop-8.9.0/README.rst` & `jaraco.develop-8.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.9.0/conftest.py` & `jaraco.develop-8.9.1/conftest.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.9.0/docs/conf.py` & `jaraco.develop-8.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.9.0/jaraco/develop/add-github-secrets.py` & `jaraco.develop-8.9.1/jaraco/develop/add-github-secrets.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.9.0/jaraco/develop/compiler.py` & `jaraco.develop-8.9.1/jaraco/develop/compiler.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.9.0/jaraco/develop/cpython-sync.py` & `jaraco.develop-8.9.1/jaraco/develop/cpython-sync.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.9.0/jaraco/develop/filters.py` & `jaraco.develop-8.9.1/jaraco/develop/filters.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.9.0/jaraco/develop/git.py` & `jaraco.develop-8.9.1/jaraco/develop/git.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.9.0/jaraco/develop/github.py` & `jaraco.develop-8.9.1/jaraco/develop/github.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.9.0/jaraco/develop/indent.py` & `jaraco.develop-8.9.1/jaraco/develop/indent.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.9.0/jaraco/develop/init-azure.py` & `jaraco.develop-8.9.1/jaraco/develop/init-azure.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.9.0/jaraco/develop/macos-build-python.py` & `jaraco.develop-8.9.1/jaraco/develop/macos-build-python.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.9.0/jaraco/develop/merge.py` & `jaraco.develop-8.9.1/jaraco/develop/merge.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.9.0/jaraco/develop/projects-run.py` & `jaraco.develop-8.9.1/jaraco/develop/projects-run.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,11 +33,11 @@
 
 @autocommand.autocommand(__name__, parser=parser)
 def main(
     selectors: filters.Selectors,
     args=None,
 ):
     for project in filter(selectors, git.projects()):
-        print(project)
+        print(project, flush=True)
         with git.temp_checkout(project, quiet=True):
             subprocess.Popen(args).wait()
-        print()
+        print(flush=True)
```

### Comparing `jaraco.develop-8.9.0/jaraco/develop/repo.py` & `jaraco.develop-8.9.1/jaraco/develop/repo.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.9.0/jaraco/develop/rst-header-replace.py` & `jaraco.develop-8.9.1/jaraco/develop/rst-header-replace.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.9.0/jaraco/develop/towncrier.py` & `jaraco.develop-8.9.1/jaraco/develop/towncrier.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.9.0/jaraco/develop/update-projects.py` & `jaraco.develop-8.9.1/jaraco/develop/update-projects.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.9.0/jaraco.develop.egg-info/PKG-INFO` & `jaraco.develop-8.9.1/jaraco.develop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.develop
-Version: 8.9.0
+Version: 8.9.1
 Summary: Development utilities by jaraco
 Home-page: https://github.com/jaraco/jaraco.develop
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jaraco.develop-8.9.0/jaraco.develop.egg-info/SOURCES.txt` & `jaraco.develop-8.9.1/jaraco.develop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.9.0/pytest.ini` & `jaraco.develop-8.9.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.9.0/setup.cfg` & `jaraco.develop-8.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `jaraco.develop-8.9.0/tox.ini` & `jaraco.develop-8.9.1/tox.ini`

 * *Files identical despite different names*

