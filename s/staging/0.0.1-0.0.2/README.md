# Comparing `tmp/staging-0.0.1.tar.gz` & `tmp/staging-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staging-0.0.1.tar", last modified: Thu Apr  4 12:00:11 2024, max compression
+gzip compressed data, was "staging-0.0.2.tar", last modified: Mon Apr 15 23:26:44 2024, max compression
```

## Comparing `staging-0.0.1.tar` & `staging-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:00:11.495849 staging-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-04 12:00:02.000000 staging-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-04 12:00:11.495849 staging-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-04 12:00:02.000000 staging-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-04 12:00:02.000000 staging-0.0.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:00:11.495849 staging-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:00:11.491849 staging-0.0.1/staging/
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-04 12:00:02.000000 staging-0.0.1/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-04 12:00:02.000000 staging-0.0.1/staging/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-04 12:00:02.000000 staging-0.0.1/staging/executable.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-04 12:00:02.000000 staging-0.0.1/staging/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-04 12:00:02.000000 staging-0.0.1/staging/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-04 12:00:02.000000 staging-0.0.1/staging/stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-04 12:00:02.000000 staging-0.0.1/staging/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:00:11.495849 staging-0.0.1/staging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-04 12:00:11.000000 staging-0.0.1/staging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-04 12:00:11.000000 staging-0.0.1/staging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:00:11.000000 staging-0.0.1/staging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-04 12:00:11.000000 staging-0.0.1/staging.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-04 12:00:11.000000 staging-0.0.1/staging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 12:00:11.000000 staging-0.0.1/staging.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:00:11.495849 staging-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-04 12:00:02.000000 staging-0.0.1/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:26:44.459068 staging-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-15 23:26:37.000000 staging-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-04-15 23:26:44.459068 staging-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-15 23:26:37.000000 staging-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-15 23:26:37.000000 staging-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-15 23:26:37.000000 staging-0.0.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 23:26:44.459068 staging-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:26:44.459068 staging-0.0.2/staging/
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-15 23:26:37.000000 staging-0.0.2/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-15 23:26:37.000000 staging-0.0.2/staging/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-15 23:26:37.000000 staging-0.0.2/staging/executable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-15 23:26:37.000000 staging-0.0.2/staging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-15 23:26:37.000000 staging-0.0.2/staging/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-15 23:26:37.000000 staging-0.0.2/staging/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-15 23:26:37.000000 staging-0.0.2/staging/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:26:44.459068 staging-0.0.2/staging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-04-15 23:26:44.000000 staging-0.0.2/staging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-15 23:26:44.000000 staging-0.0.2/staging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 23:26:44.000000 staging-0.0.2/staging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 23:26:44.000000 staging-0.0.2/staging.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-15 23:26:44.000000 staging-0.0.2/staging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 23:26:44.000000 staging-0.0.2/staging.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:26:44.459068 staging-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-15 23:26:37.000000 staging-0.0.2/tests/test_unit.py
```

### Comparing `staging-0.0.1/LICENSE` & `staging-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `staging-0.0.1/pyproject.toml` & `staging-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "staging"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name="Radoslaw Gryta", email="radek.gryta@gmail.com" },
 ]
 description = "Execute pipeline stages and steps"
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = ["CI", "CD", "stage", "step", "pipeline", "workflow", "automation", "orchestration", "execution", "staging"]
@@ -34,15 +34,15 @@
 
 [tool.setuptools.dynamic]
 optional-dependencies = { dev = {file = ["requirements_dev.txt"]} }
 
 ####### BUMPV #######
 
 [tool.bumpversion]
-current_version = "0.0.1"
+current_version = "0.0.2"
 allow_dirty = true
 commit = true
 message = "[Version {new_version}]"
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = "version = \"{current_version}\""
@@ -75,34 +75,34 @@
 
 [tool.pylint.format]
 max-line-length = 120
 
 
 ####### STAGING #######
 [tool.staging.steps]
-# Prepare
-package = { execute = "toml get --toml-path pyproject.toml project.name | tr '-' '_' | tr -d '\n'", output = "package" }
-# Clean
-clean = { execute = "rm -rf build dist staging.egg-info" }
 # Lint
 isort = { execute = "isort {flags} . tests", format = {flags = "flags"}}
 black = { execute = "black {flags} . tests", format = {flags = "flags"}}
 pylint = { execute = "pylint {package} tests", format = {package = "package"}}
 noprint = { execute = "noprint -ve {package} tests", format = {package = "package"}}
 # Test
 coverage = { prepare = "coverage run -m pytest -xv tests", execute = "coverage report -m --fail-under=30", cleanup = "coverage erase"}
 
 [tool.staging.stages.test]
 description = "Test the package"
-format = {flags="--check"}
 steps = [
-    {parallel = {steps = ["clean", "package"]}, continue_on_failure = true},
-    {parallel = {steps = ["isort", "black", "pylint", "noprint", "coverage"]}},
+    {step = "coverage"},
 ]
 
 [tool.staging.stages.format]
-description = "Format the package"
+description = "Reformat code"
 steps = [
-    {step = "clean", continue_on_failure = true},
-    {step = "isort", continue_on_failure = true},
-    {step = "black", continue_on_failure = true},
+    {step = "isort"},
+    {step = "black"},
 ]
+
+[tool.staging.stages.lint]
+description = "Check linting"
+format = {flags="--check", package="staging"}
+steps = [
+    {parallel = {steps = ["isort", "black", "pylint", "noprint"]}},
+]
```

### Comparing `staging-0.0.1/staging/__init__.py` & `staging-0.0.2/staging/__init__.py`

 * *Files identical despite different names*

### Comparing `staging-0.0.1/staging/config.py` & `staging-0.0.2/staging/config.py`

 * *Files identical despite different names*

### Comparing `staging-0.0.1/staging/parallel.py` & `staging-0.0.2/staging/parallel.py`

 * *Files identical despite different names*

### Comparing `staging-0.0.1/staging/stage.py` & `staging-0.0.2/staging/stage.py`

 * *Files identical despite different names*

### Comparing `staging-0.0.1/staging/step.py` & `staging-0.0.2/staging/step.py`

 * *Files identical despite different names*

