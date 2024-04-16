# Comparing `tmp/tefs-0.3.1.tar.gz` & `tmp/tefs-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tefs-0.3.1.tar", last modified: Wed Apr  3 11:23:18 2024, max compression
+gzip compressed data, was "tefs-0.3.2.tar", last modified: Tue Apr 16 20:05:53 2024, max compression
```

## Comparing `tefs-0.3.1.tar` & `tefs-0.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:23:18.671984 tefs-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-03 11:21:11.000000 tefs-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-03 11:23:18.671984 tefs-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-03 11:21:11.000000 tefs-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-03 11:21:11.000000 tefs-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 11:23:18.671984 tefs-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:23:18.667984 tefs-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:23:18.667984 tefs-0.3.1/src/tefs/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 11:21:11.000000 tefs-0.3.1/src/tefs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20272 2024-04-03 11:21:11.000000 tefs-0.3.1/src/tefs/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-04-03 11:21:11.000000 tefs-0.3.1/src/tefs/estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-03 11:21:11.000000 tefs-0.3.1/src/tefs/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-03 11:21:11.000000 tefs-0.3.1/src/tefs/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:23:18.671984 tefs-0.3.1/src/tefs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-03 11:23:18.000000 tefs-0.3.1/src/tefs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-03 11:23:18.000000 tefs-0.3.1/src/tefs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:23:18.000000 tefs-0.3.1/src/tefs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 11:23:18.000000 tefs-0.3.1/src/tefs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 11:23:18.000000 tefs-0.3.1/src/tefs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:23:18.671984 tefs-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-03 11:21:11.000000 tefs-0.3.1/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-03 11:21:11.000000 tefs-0.3.1/tests/test_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:05:53.083637 tefs-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-16 20:04:42.000000 tefs-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-16 20:05:53.083637 tefs-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-16 20:04:42.000000 tefs-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-16 20:04:42.000000 tefs-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 20:05:53.083637 tefs-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:05:53.083637 tefs-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:05:53.083637 tefs-0.3.2/src/tefs/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 20:04:42.000000 tefs-0.3.2/src/tefs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20272 2024-04-16 20:04:42.000000 tefs-0.3.2/src/tefs/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-04-16 20:04:42.000000 tefs-0.3.2/src/tefs/estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-16 20:04:42.000000 tefs-0.3.2/src/tefs/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-16 20:04:42.000000 tefs-0.3.2/src/tefs/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:05:53.083637 tefs-0.3.2/src/tefs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-16 20:05:53.000000 tefs-0.3.2/src/tefs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-16 20:05:53.000000 tefs-0.3.2/src/tefs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:05:53.000000 tefs-0.3.2/src/tefs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 20:05:53.000000 tefs-0.3.2/src/tefs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 20:05:53.000000 tefs-0.3.2/src/tefs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:05:53.083637 tefs-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-16 20:04:42.000000 tefs-0.3.2/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-16 20:04:42.000000 tefs-0.3.2/tests/test_estimation.py
```

### Comparing `tefs-0.3.1/LICENSE` & `tefs-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tefs-0.3.1/PKG-INFO` & `tefs-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tefs
-Version: 0.3.1
+Version: 0.3.2
 Summary: Causal feature selection for time series data using transfer entropy
 Author-email: Teo Bucci <teobucci8@gmail.com>, Paolo Bonetti <paolo.bonetti@polimi.it>
 License: MIT License
         
         Copyright (c) 2024 Transfer Entropy Feature Selection
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,15 +22,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/teobucci/tefs
-Project-URL: Documentation, https://github.com/teobucci/tefs
+Project-URL: Documentation, https://teobucci.github.io/tefs/
 Project-URL: Repository, https://github.com/teobucci/tefs
 Keywords: tefs,transfer entropy,feature selection,causality,time series
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -46,16 +46,14 @@
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-green)](LICENSE)
 ![PyPI - Version](https://img.shields.io/pypi/v/tefs)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/tefs)
 
 This repository implements a causal feature selection algorithm based on transfer entropy. The algorithm is described in: Bonetti, P., Metelli, A. M., & Restelli, M. (2023, October 17). Causal Feature Selection via Transfer Entropy. (https://arxiv.org/abs/2310.11059).
 
-Requires Python 3.9 or later.
-
 ## Installation
 
 The package can be installed using pip:
 
 ```bash
 pip install tefs
 ```
```

### Comparing `tefs-0.3.1/README.md` & `tefs-0.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-green)](LICENSE)
 ![PyPI - Version](https://img.shields.io/pypi/v/tefs)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/tefs)
 
 This repository implements a causal feature selection algorithm based on transfer entropy. The algorithm is described in: Bonetti, P., Metelli, A. M., & Restelli, M. (2023, October 17). Causal Feature Selection via Transfer Entropy. (https://arxiv.org/abs/2310.11059).
 
-Requires Python 3.9 or later.
-
 ## Installation
 
 The package can be installed using pip:
 
 ```bash
 pip install tefs
 ```
```

### Comparing `tefs-0.3.1/pyproject.toml` & `tefs-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tefs"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
     { name = "Teo Bucci", email = "teobucci8@gmail.com" },
     { name = "Paolo Bonetti", email = "paolo.bonetti@polimi.it" },
 ]
 description = "Causal feature selection for time series data using transfer entropy"
 readme = "README.md"
 license = { file = "LICENSE" }
@@ -32,15 +32,15 @@
     "seaborn",
     "scikit-learn",
 ]
 requires-python = ">=3.9"
 
 [project.urls]
 Homepage = "https://github.com/teobucci/tefs"
-Documentation = "https://github.com/teobucci/tefs"
+Documentation = "https://teobucci.github.io/tefs/"
 Repository = "https://github.com/teobucci/tefs"
 
 [tool.pdm.dev-dependencies]
 docs = [
     "sphinx",
     "sphinx-rtd-theme",
     "myst-parser",
@@ -59,15 +59,15 @@
     "wheel",
     "twine",
     "build",
     "bumpver",
 ]
 
 [tool.bumpver]
-current_version = "0.3.1"
+current_version = "0.3.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `tefs-0.3.1/src/tefs/core.py` & `tefs-0.3.2/src/tefs/core.py`

 * *Files identical despite different names*

### Comparing `tefs-0.3.1/src/tefs/estimation.py` & `tefs-0.3.2/src/tefs/estimation.py`

 * *Files identical despite different names*

### Comparing `tefs-0.3.1/src/tefs/metrics.py` & `tefs-0.3.2/src/tefs/metrics.py`

 * *Files identical despite different names*

### Comparing `tefs-0.3.1/src/tefs.egg-info/PKG-INFO` & `tefs-0.3.2/src/tefs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tefs
-Version: 0.3.1
+Version: 0.3.2
 Summary: Causal feature selection for time series data using transfer entropy
 Author-email: Teo Bucci <teobucci8@gmail.com>, Paolo Bonetti <paolo.bonetti@polimi.it>
 License: MIT License
         
         Copyright (c) 2024 Transfer Entropy Feature Selection
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,15 +22,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/teobucci/tefs
-Project-URL: Documentation, https://github.com/teobucci/tefs
+Project-URL: Documentation, https://teobucci.github.io/tefs/
 Project-URL: Repository, https://github.com/teobucci/tefs
 Keywords: tefs,transfer entropy,feature selection,causality,time series
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -46,16 +46,14 @@
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-green)](LICENSE)
 ![PyPI - Version](https://img.shields.io/pypi/v/tefs)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/tefs)
 
 This repository implements a causal feature selection algorithm based on transfer entropy. The algorithm is described in: Bonetti, P., Metelli, A. M., & Restelli, M. (2023, October 17). Causal Feature Selection via Transfer Entropy. (https://arxiv.org/abs/2310.11059).
 
-Requires Python 3.9 or later.
-
 ## Installation
 
 The package can be installed using pip:
 
 ```bash
 pip install tefs
 ```
```

### Comparing `tefs-0.3.1/tests/test_core.py` & `tefs-0.3.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tefs-0.3.1/tests/test_estimation.py` & `tefs-0.3.2/tests/test_estimation.py`

 * *Files identical despite different names*

