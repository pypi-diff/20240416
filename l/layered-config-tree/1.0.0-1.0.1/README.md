# Comparing `tmp/layered_config_tree-1.tar.gz` & `tmp/layered_config_tree-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layered_config_tree-1.tar", last modified: Fri Apr 12 22:12:02 2024, max compression
+gzip compressed data, was "layered_config_tree-1.0.1.tar", last modified: Tue Apr 16 19:57:38 2024, max compression
```

## Comparing `layered_config_tree-1.tar` & `layered_config_tree-1.0.1.tar`

### file list

```diff
@@ -1,50 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:02.058503 layered_config_tree-1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:02.054503 layered_config_tree-1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-12 22:11:51.000000 layered_config_tree-1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-12 22:11:51.000000 layered_config_tree-1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:02.054503 layered_config_tree-1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-12 22:11:51.000000 layered_config_tree-1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-12 22:11:51.000000 layered_config_tree-1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-12 22:11:51.000000 layered_config_tree-1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-12 22:11:51.000000 layered_config_tree-1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-12 22:11:51.000000 layered_config_tree-1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-12 22:11:51.000000 layered_config_tree-1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-12 22:11:51.000000 layered_config_tree-1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-12 22:11:51.000000 layered_config_tree-1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-12 22:11:51.000000 layered_config_tree-1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-12 22:12:02.058503 layered_config_tree-1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-12 22:11:51.000000 layered_config_tree-1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:02.054503 layered_config_tree-1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-12 22:11:51.000000 layered_config_tree-1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:02.054503 layered_config_tree-1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:02.054503 layered_config_tree-1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 22:11:51.000000 layered_config_tree-1/docs/source/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:02.054503 layered_config_tree-1/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-12 22:11:51.000000 layered_config_tree-1/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     7544 2024-04-12 22:11:51.000000 layered_config_tree-1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-12 22:11:51.000000 layered_config_tree-1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 22:11:51.000000 layered_config_tree-1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 22:12:02.058503 layered_config_tree-1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-12 22:11:51.000000 layered_config_tree-1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:02.054503 layered_config_tree-1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:02.058503 layered_config_tree-1/src/layered_config_tree/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-12 22:11:51.000000 layered_config_tree-1/src/layered_config_tree/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-12 22:11:51.000000 layered_config_tree-1/src/layered_config_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 22:12:01.000000 layered_config_tree-1/src/layered_config_tree/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-12 22:11:51.000000 layered_config_tree-1/src/layered_config_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19991 2024-04-12 22:11:51.000000 layered_config_tree-1/src/layered_config_tree/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:02.058503 layered_config_tree-1/src/layered_config_tree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-12 22:12:02.000000 layered_config_tree-1/src/layered_config_tree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-12 22:12:02.000000 layered_config_tree-1/src/layered_config_tree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 22:12:02.000000 layered_config_tree-1/src/layered_config_tree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 22:11:58.000000 layered_config_tree-1/src/layered_config_tree.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-12 22:12:02.000000 layered_config_tree-1/src/layered_config_tree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 22:12:02.000000 layered_config_tree-1/src/layered_config_tree.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:02.058503 layered_config_tree-1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:11:51.000000 layered_config_tree-1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-12 22:11:51.000000 layered_config_tree-1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    17194 2024-04-12 22:11:51.000000 layered_config_tree-1/tests/test_basic_functionality.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:12:02.058503 layered_config_tree-1/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-12 22:11:51.000000 layered_config_tree-1/tests/test_data/mock_model_specification.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-12 22:11:51.000000 layered_config_tree-1/tests/test_data/mock_model_specification.yml
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-12 22:11:51.000000 layered_config_tree-1/tests/test_ingestion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.698656 layered_config_tree-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.690656 layered_config_tree-1.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.690656 layered_config_tree-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/.github/workflows/update_readme.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-16 19:57:38.694656 layered_config_tree-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.690656 layered_config_tree-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.690656 layered_config_tree-1.0.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.690656 layered_config_tree-1.0.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/docs/source/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.690656 layered_config_tree-1.0.1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7544 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/python_versions.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:57:38.698656 layered_config_tree-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.686656 layered_config_tree-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.694656 layered_config_tree-1.0.1/src/layered_config_tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/src/layered_config_tree/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/src/layered_config_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 19:57:38.000000 layered_config_tree-1.0.1/src/layered_config_tree/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/src/layered_config_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19980 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/src/layered_config_tree/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.694656 layered_config_tree-1.0.1/src/layered_config_tree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-16 19:57:38.000000 layered_config_tree-1.0.1/src/layered_config_tree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-16 19:57:38.000000 layered_config_tree-1.0.1/src/layered_config_tree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:57:38.000000 layered_config_tree-1.0.1/src/layered_config_tree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:57:34.000000 layered_config_tree-1.0.1/src/layered_config_tree.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-16 19:57:38.000000 layered_config_tree-1.0.1/src/layered_config_tree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 19:57:38.000000 layered_config_tree-1.0.1/src/layered_config_tree.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.694656 layered_config_tree-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17155 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/tests/test_basic_functionality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.694656 layered_config_tree-1.0.1/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/tests/test_data/mock_model_specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/tests/test_data/mock_model_specification.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/tests/test_ingestion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/update_readme.py
```

### Comparing `layered_config_tree-1/.github/pull_request_template.md` & `layered_config_tree-1.0.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1/.github/workflows/build.yml` & `layered_config_tree-1.0.1/.github/workflows/build.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,39 @@
 # -----------------------------------------------------------------------------
 #   - invoked on push, pull_request, manual trigger, or schedule
-#   - test under at least 3 versions of python
+#   - test under all supported versions of python (see python_versions.json)
 # -----------------------------------------------------------------------------
 name: build
 on:
   push:
   pull_request:
   workflow_dispatch:
   schedule:
     - cron: "0 8 * * *"
 
 jobs:
+  get-python-versions:
+    runs-on: ubuntu-latest
+    steps:
+      - name: Checkout code
+        uses: actions/checkout@v2
+      - name: Install jq
+        run: sudo apt-get install jq
+      - name: Get Python versions
+        id: set-matrix
+        run: |
+          echo "MATRIX_RESULT=$(jq -c . python_versions.json)" >> $GITHUB_ENV
+    outputs:
+      matrix: ${{ env.MATRIX_RESULT }}
   build:
+    needs: get-python-versions
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.9", "3.10", "3.11"]
+        python-version: ${{ fromJSON(needs.get-python-versions.outputs.matrix) }}
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Print environment values
```

### Comparing `layered_config_tree-1/.github/workflows/deploy.yml` & `layered_config_tree-1.0.1/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1/.gitignore` & `layered_config_tree-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1/.readthedocs.yaml` & `layered_config_tree-1.0.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1/CODE_OF_CONDUCT.rst` & `layered_config_tree-1.0.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1/CONTRIBUTING.rst` & `layered_config_tree-1.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1/LICENSE.txt` & `layered_config_tree-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1/PKG-INFO` & `layered_config_tree-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layered_config_tree
-Version: 1.0.0
+Version: 1.0.1
 Summary: Layered Config Tree is a configuration structure which supports cascading layers.
 Home-page: https://github.com/ihmeuw/layered_config_tree
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -41,17 +41,21 @@
 
 ===================
 Layered Config Tree
 ===================
 
 Layered Config Tree is a configuration structure that supports cascading layers.
 
-**Layered Config Tree requires Python 3.8-3.11 to run**
+**Supported Python versions: 3.8, 3.9, 3.10, 3.11**
 
-You can build ``layered_config_tree`` from from source with
+You can install ``layered_config_tree`` from PyPI with pip:
+
+  ``> pip install layered_config_tree``
+
+or build it from from source:
 
   ``> git clone https://github.com/ihmeuw/layered_config_tree.git``
 
   ``> cd layered_config_tree``
 
   ``> conda create -n ENVIRONMENT_NAME python=3.11``
```

### Comparing `layered_config_tree-1/docs/Makefile` & `layered_config_tree-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1/docs/source/conf.py` & `layered_config_tree-1.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1/setup.py` & `layered_config_tree-1.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,32 @@
+import json
 import sys
 from pathlib import Path
 
+from packaging.version import parse
 from setuptools import find_packages, setup
 
-min_version, max_version = ((3, 8), "3.8"), ((3, 11), "3.11")
+with open("python_versions.json", "r") as f:
+    supported_python_versions = json.load(f)
 
-if not (min_version[0] <= sys.version_info[:2] <= max_version[0]):
-    # Python 3.5 does not support f-strings
+python_versions = [parse(v) for v in supported_python_versions]
+min_version = min(python_versions)
+max_version = max(python_versions)
+if not (
+    min_version <= parse(".".join([str(v) for v in sys.version_info[:2]])) <= max_version
+):
     py_version = ".".join([str(v) for v in sys.version_info[:3]])
+    # NOTE: Python 3.5 does not support f-strings
     error = (
         "\n----------------------------------------\n"
         "Error: Layered Config Tree runs under python {min_version}-{max_version}.\n"
         "You are running python {py_version}".format(
-            min_version=min_version[1], max_version=max_version[1], py_version=py_version
+            min_version=min_version.base_version,
+            max_version=max_version.base_version,
+            py_version=py_version,
         )
     )
     print(error, file=sys.stderr)
     sys.exit(1)
 
 
 if __name__ == "__main__":
```

### Comparing `layered_config_tree-1/src/layered_config_tree/exceptions.py` & `layered_config_tree-1.0.1/src/layered_config_tree/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 
 class ConfigurationError(Exception):
     """Base class for configuration errors."""
 
     def __init__(self, message: str, value_name: Optional[str]):
         super().__init__(message)
+        self.value_name = value_name
 
 
 class ConfigurationKeyError(ConfigurationError, KeyError):
     """Error raised when a configuration lookup fails."""
 
     pass
```

### Comparing `layered_config_tree-1/src/layered_config_tree/main.py` & `layered_config_tree-1.0.1/src/layered_config_tree/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 """
 
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
 import yaml
 
-from layered_config_tree.exceptions import (
+from layered_config_tree import (
     ConfigurationError,
     ConfigurationKeyError,
     DuplicatedConfigurationError,
 )
 
 
 class ConfigNode:
```

### Comparing `layered_config_tree-1/src/layered_config_tree.egg-info/PKG-INFO` & `layered_config_tree-1.0.1/src/layered_config_tree.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layered_config_tree
-Version: 1.0.0
+Version: 1.0.1
 Summary: Layered Config Tree is a configuration structure which supports cascading layers.
 Home-page: https://github.com/ihmeuw/layered_config_tree
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -41,17 +41,21 @@
 
 ===================
 Layered Config Tree
 ===================
 
 Layered Config Tree is a configuration structure that supports cascading layers.
 
-**Layered Config Tree requires Python 3.8-3.11 to run**
+**Supported Python versions: 3.8, 3.9, 3.10, 3.11**
 
-You can build ``layered_config_tree`` from from source with
+You can install ``layered_config_tree`` from PyPI with pip:
+
+  ``> pip install layered_config_tree``
+
+or build it from from source:
 
   ``> git clone https://github.com/ihmeuw/layered_config_tree.git``
 
   ``> cd layered_config_tree``
 
   ``> conda create -n ENVIRONMENT_NAME python=3.11``
```

### Comparing `layered_config_tree-1/src/layered_config_tree.egg-info/SOURCES.txt` & `layered_config_tree-1.0.1/src/layered_config_tree.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,22 @@
 CHANGELOG.rst
 CODE_OF_CONDUCT.rst
 CONTRIBUTING.rst
 LICENSE.txt
 MANIFEST.in
 README.rst
 pyproject.toml
+python_versions.json
 setup.py
+update_readme.py
 .github/CODEOWNERS
 .github/pull_request_template.md
 .github/workflows/build.yml
 .github/workflows/deploy.yml
+.github/workflows/update_readme.yml
 docs/Makefile
 docs/source/conf.py
 docs/source/index.rst
 docs/source/_static/style.css
 docs/source/_templates/layout.html
 src/layered_config_tree/__about__.py
 src/layered_config_tree/__init__.py
```

### Comparing `layered_config_tree-1/tests/conftest.py` & `layered_config_tree-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1/tests/test_basic_functionality.py` & `layered_config_tree-1.0.1/tests/test_basic_functionality.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import pickle
 import textwrap
 
 import pytest
 import yaml
 
-from layered_config_tree.exceptions import (
+from layered_config_tree import (
+    ConfigNode,
     ConfigurationError,
     ConfigurationKeyError,
     DuplicatedConfigurationError,
+    LayeredConfigTree,
 )
-from layered_config_tree.main import ConfigNode, LayeredConfigTree
 
 
 @pytest.fixture(params=list(range(1, 5)))
 def layers(request):
     return [f"layer_{i}" for i in range(1, request.param + 1)]
```

### Comparing `layered_config_tree-1/tests/test_ingestion.py` & `layered_config_tree-1.0.1/tests/test_ingestion.py`

 * *Files identical despite different names*

