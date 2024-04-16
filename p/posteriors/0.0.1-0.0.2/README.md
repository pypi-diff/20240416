# Comparing `tmp/posteriors-0.0.1.tar.gz` & `tmp/posteriors-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "posteriors-0.0.1.tar", last modified: Mon Apr 15 17:46:50 2024, max compression
+gzip compressed data, was "posteriors-0.0.2.tar", last modified: Tue Apr 16 18:00:00 2024, max compression
```

## Comparing `posteriors-0.0.1.tar` & `posteriors-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:46:50.392438 posteriors-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 17:46:46.000000 posteriors-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-15 17:46:50.392438 posteriors-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-15 17:46:46.000000 posteriors-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:46:50.388438 posteriors-0.0.1/posteriors/
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-15 17:46:46.000000 posteriors-0.0.1/posteriors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-15 17:46:46.000000 posteriors-0.0.1/posteriors/optim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-15 17:46:46.000000 posteriors-0.0.1/posteriors/torchopt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-15 17:46:46.000000 posteriors-0.0.1/posteriors/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    22478 2024-04-15 17:46:46.000000 posteriors-0.0.1/posteriors/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:46:50.392438 posteriors-0.0.1/posteriors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-15 17:46:50.000000 posteriors-0.0.1/posteriors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-15 17:46:50.000000 posteriors-0.0.1/posteriors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 17:46:50.000000 posteriors-0.0.1/posteriors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-15 17:46:50.000000 posteriors-0.0.1/posteriors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 17:46:50.000000 posteriors-0.0.1/posteriors.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-15 17:46:46.000000 posteriors-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 17:46:50.392438 posteriors-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:46:50.392438 posteriors-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-15 17:46:46.000000 posteriors-0.0.1/tests/test_optim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-15 17:46:46.000000 posteriors-0.0.1/tests/test_torchopt.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-15 17:46:46.000000 posteriors-0.0.1/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    16698 2024-04-15 17:46:46.000000 posteriors-0.0.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:00:00.548081 posteriors-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 17:59:55.000000 posteriors-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-16 18:00:00.548081 posteriors-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-16 17:59:55.000000 posteriors-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:00:00.544081 posteriors-0.0.2/posteriors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:00:00.548081 posteriors-0.0.2/posteriors/ekf/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/ekf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/ekf/diag_fisher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:00:00.548081 posteriors-0.0.2/posteriors/laplace/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/laplace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/laplace/dense_fisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/laplace/diag_fisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/optim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:00:00.548081 posteriors-0.0.2/posteriors/sgmcmc/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/sgmcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/sgmcmc/sghmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/sgmcmc/sgld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/torchopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22478 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:00:00.548081 posteriors-0.0.2/posteriors/vi/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/vi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/vi/diag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:00:00.548081 posteriors-0.0.2/posteriors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-16 18:00:00.000000 posteriors-0.0.2/posteriors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-16 18:00:00.000000 posteriors-0.0.2/posteriors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 18:00:00.000000 posteriors-0.0.2/posteriors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-16 18:00:00.000000 posteriors-0.0.2/posteriors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 18:00:00.000000 posteriors-0.0.2/posteriors.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-16 17:59:55.000000 posteriors-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 18:00:00.548081 posteriors-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:00:00.548081 posteriors-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-16 17:59:55.000000 posteriors-0.0.2/tests/test_optim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-16 17:59:55.000000 posteriors-0.0.2/tests/test_torchopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-16 17:59:55.000000 posteriors-0.0.2/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16698 2024-04-16 17:59:55.000000 posteriors-0.0.2/tests/test_utils.py
```

### Comparing `posteriors-0.0.1/LICENSE` & `posteriors-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `posteriors-0.0.1/PKG-INFO` & `posteriors-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posteriors
-Version: 0.0.1
+Version: 0.0.2
 Summary: Uncertainty quantification with PyTorch
 Author-email: Sam Duffield <sam@normalcomputing.ai>
 License: Apache-2.0
 Keywords: pytorch,uncertainty
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `posteriors-0.0.1/README.md` & `posteriors-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `posteriors-0.0.1/posteriors/__init__.py` & `posteriors-0.0.2/posteriors/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,7 +32,11 @@
 logger.setLevel(logging.ERROR)
 
 from posteriors import vi
 from posteriors import torchopt
 
 del logging
 del logger
+
+from importlib.metadata import version
+
+__version__ = version("posteriors")
```

### Comparing `posteriors-0.0.1/posteriors/optim.py` & `posteriors-0.0.2/posteriors/optim.py`

 * *Files identical despite different names*

### Comparing `posteriors-0.0.1/posteriors/torchopt.py` & `posteriors-0.0.2/posteriors/torchopt.py`

 * *Files identical despite different names*

### Comparing `posteriors-0.0.1/posteriors/types.py` & `posteriors-0.0.2/posteriors/types.py`

 * *Files identical despite different names*

### Comparing `posteriors-0.0.1/posteriors/utils.py` & `posteriors-0.0.2/posteriors/utils.py`

 * *Files identical despite different names*

### Comparing `posteriors-0.0.1/posteriors.egg-info/PKG-INFO` & `posteriors-0.0.2/posteriors.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posteriors
-Version: 0.0.1
+Version: 0.0.2
 Summary: Uncertainty quantification with PyTorch
 Author-email: Sam Duffield <sam@normalcomputing.ai>
 License: Apache-2.0
 Keywords: pytorch,uncertainty
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `posteriors-0.0.1/pyproject.toml` & `posteriors-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "posteriors"
-version = "0.0.1"
+version = "0.0.2"
 description = "Uncertainty quantification with PyTorch"
 readme = "README.md"
 requires-python =">=3.9"
 license = {text = "Apache-2.0"}
 authors = [
     {name = "Sam Duffield", email = "sam@normalcomputing.ai"},
 ]
@@ -17,12 +17,22 @@
 dependencies = ["torch>=2.0.0", "torchopt>=0.7.3", "optree>=0.10.0"]
 
 [project.optional-dependencies]
 test = ["pre-commit", "pytest-cov", "ruff"]
 docs = ["mkdocs", "mkdocs-material", "mkdocstrings[python]"]
 
 [tool.setuptools]
-packages = ["posteriors"]
+packages = [
+    "posteriors",
+    "posteriors.ekf",
+    "posteriors.laplace",
+    "posteriors.sgmcmc",
+    "posteriors.vi",
+]
 
 [tool.ruff]
 [tool.ruff.lint.per-file-ignores]
-"__init__.py" = ["F401", "F821", "E402"]
+"__init__.py" = ["F401", "F821", "E402"]
+
+[build-system]
+requires = ["setuptools>=64"]
+build-backend = "setuptools.build_meta"
```

### Comparing `posteriors-0.0.1/tests/test_optim.py` & `posteriors-0.0.2/tests/test_optim.py`

 * *Files identical despite different names*

### Comparing `posteriors-0.0.1/tests/test_torchopt.py` & `posteriors-0.0.2/tests/test_torchopt.py`

 * *Files identical despite different names*

### Comparing `posteriors-0.0.1/tests/test_types.py` & `posteriors-0.0.2/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `posteriors-0.0.1/tests/test_utils.py` & `posteriors-0.0.2/tests/test_utils.py`

 * *Files identical despite different names*

