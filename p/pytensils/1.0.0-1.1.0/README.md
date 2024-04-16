# Comparing `tmp/pytensils-1.0.0.tar.gz` & `tmp/pytensils-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytensils-1.0.0.tar", last modified: Mon Mar 25 02:26:48 2024, max compression
+gzip compressed data, was "pytensils-1.1.0.tar", last modified: Tue Apr 16 21:34:54 2024, max compression
```

## Comparing `pytensils-1.0.0.tar` & `pytensils-1.1.0.tar`

### file list

```diff
@@ -1,45 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:26:48.164615 pytensils-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:26:48.156615 pytensils-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:26:48.160615 pytensils-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-03-25 02:26:43.000000 pytensils-1.0.0/.github/workflows/coverage-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-25 02:26:43.000000 pytensils-1.0.0/.github/workflows/publish-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-25 02:26:43.000000 pytensils-1.0.0/.github/workflows/unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-25 02:26:43.000000 pytensils-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-25 02:26:43.000000 pytensils-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20444 2024-03-25 02:26:48.164615 pytensils-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19396 2024-03-25 02:26:43.000000 pytensils-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:26:48.160615 pytensils-1.0.0/coverage/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-25 02:26:43.000000 pytensils-1.0.0/coverage/COVERAGE.md
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-25 02:26:43.000000 pytensils-1.0.0/coverage/coverage.svg
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-25 02:26:43.000000 pytensils-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:26:48.160615 pytensils-1.0.0/pytensils/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-25 02:26:43.000000 pytensils-1.0.0/pytensils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17334 2024-03-25 02:26:43.000000 pytensils-1.0.0/pytensils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    18664 2024-03-25 02:26:43.000000 pytensils-1.0.0/pytensils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-25 02:26:43.000000 pytensils-1.0.0/pytensils/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-03-25 02:26:43.000000 pytensils-1.0.0/pytensils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:26:48.164615 pytensils-1.0.0/pytensils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20444 2024-03-25 02:26:48.000000 pytensils-1.0.0/pytensils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-25 02:26:48.000000 pytensils-1.0.0/pytensils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 02:26:48.000000 pytensils-1.0.0/pytensils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-25 02:26:48.000000 pytensils-1.0.0/pytensils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-25 02:26:48.000000 pytensils-1.0.0/pytensils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-25 02:26:43.000000 pytensils-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-25 02:26:48.164615 pytensils-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:26:48.160615 pytensils-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 02:26:43.000000 pytensils-1.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:26:48.164615 pytensils-1.0.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-25 02:26:43.000000 pytensils-1.0.0/tests/resources/closes-on-exception-success.log
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-25 02:26:43.000000 pytensils-1.0.0/tests/resources/closes-on-exception.log
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-03-25 02:26:43.000000 pytensils-1.0.0/tests/resources/compare.log
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-25 02:26:43.000000 pytensils-1.0.0/tests/resources/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-25 02:26:43.000000 pytensils-1.0.0/tests/resources/config_invalid.json
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-25 02:26:43.000000 pytensils-1.0.0/tests/resources/config_validation_error.json
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-25 02:26:43.000000 pytensils-1.0.0/tests/resources/dtypes.json
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-03-25 02:26:43.000000 pytensils-1.0.0/tests/resources/example.log
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-03-25 02:26:43.000000 pytensils-1.0.0/tests/resources/test_config.log
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-25 02:26:43.000000 pytensils-1.0.0/tests/resources/validation.log
--rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-03-25 02:26:43.000000 pytensils-1.0.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7697 2024-03-25 02:26:43.000000 pytensils-1.0.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-25 02:26:43.000000 pytensils-1.0.0/tests/test_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-03-25 02:26:43.000000 pytensils-1.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.810531 pytensils-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.802530 pytensils-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.806531 pytensils-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-16 21:34:46.000000 pytensils-1.1.0/.github/workflows/coverage-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-16 21:34:46.000000 pytensils-1.1.0/.github/workflows/publish-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-16 21:34:46.000000 pytensils-1.1.0/.github/workflows/unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-16 21:34:46.000000 pytensils-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-16 21:34:46.000000 pytensils-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20444 2024-04-16 21:34:54.810531 pytensils-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19396 2024-04-16 21:34:46.000000 pytensils-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.806531 pytensils-1.1.0/coverage/
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-16 21:34:46.000000 pytensils-1.1.0/coverage/COVERAGE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-16 21:34:46.000000 pytensils-1.1.0/coverage/coverage.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-16 21:34:46.000000 pytensils-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.806531 pytensils-1.1.0/pytensils/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-16 21:34:46.000000 pytensils-1.1.0/pytensils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17503 2024-04-16 21:34:46.000000 pytensils-1.1.0/pytensils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-16 21:34:46.000000 pytensils-1.1.0/pytensils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20052 2024-04-16 21:34:46.000000 pytensils-1.1.0/pytensils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-16 21:34:46.000000 pytensils-1.1.0/pytensils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-16 21:34:46.000000 pytensils-1.1.0/pytensils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.810531 pytensils-1.1.0/pytensils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20444 2024-04-16 21:34:54.000000 pytensils-1.1.0/pytensils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-16 21:34:54.000000 pytensils-1.1.0/pytensils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 21:34:54.000000 pytensils-1.1.0/pytensils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-16 21:34:54.000000 pytensils-1.1.0/pytensils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 21:34:54.000000 pytensils-1.1.0/pytensils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-16 21:34:46.000000 pytensils-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-16 21:34:54.810531 pytensils-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.806531 pytensils-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:46.000000 pytensils-1.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.810531 pytensils-1.1.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-16 21:34:46.000000 pytensils-1.1.0/tests/resources/closes-on-exception-filenotfounderror.log
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-16 21:34:46.000000 pytensils-1.1.0/tests/resources/closes-on-exception-notimplementederror.log
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-16 21:34:46.000000 pytensils-1.1.0/tests/resources/closes-on-exception-oserror.log
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-16 21:34:46.000000 pytensils-1.1.0/tests/resources/closes-on-exception-success.log
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-16 21:34:46.000000 pytensils-1.1.0/tests/resources/closes-on-exception-typeerror.log
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-16 21:34:46.000000 pytensils-1.1.0/tests/resources/closes-on-exception-validationerror.log
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-16 21:34:46.000000 pytensils-1.1.0/tests/resources/closes-on-exception.log
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-16 21:34:46.000000 pytensils-1.1.0/tests/resources/compare.log
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-16 21:34:46.000000 pytensils-1.1.0/tests/resources/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-16 21:34:46.000000 pytensils-1.1.0/tests/resources/config_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-16 21:34:46.000000 pytensils-1.1.0/tests/resources/config_validation_error.json
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-16 21:34:46.000000 pytensils-1.1.0/tests/resources/dtypes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-16 21:34:46.000000 pytensils-1.1.0/tests/resources/example.log
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-16 21:34:46.000000 pytensils-1.1.0/tests/resources/test_config.log
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-16 21:34:46.000000 pytensils-1.1.0/tests/resources/validation.log
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-04-16 21:34:46.000000 pytensils-1.1.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11669 2024-04-16 21:34:46.000000 pytensils-1.1.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-16 21:34:46.000000 pytensils-1.1.0/tests/test_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-16 21:34:46.000000 pytensils-1.1.0/tests/test_utils.py
```

### Comparing `pytensils-1.0.0/.github/workflows/coverage-tests.yml` & `pytensils-1.1.0/.github/workflows/coverage-tests.yml`

 * *Files 7% similar despite different names*

```diff
@@ -18,20 +18,20 @@
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.10"]
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
       with:
         fetch-depth: 0
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install pytest coverage
@@ -47,15 +47,15 @@
       uses: tj-actions/coverage-badge-py@v2
 
     - name: Move coverage reports
       run: |
         mv coverage.svg ./coverage
 
     - name: Verify Changed files
-      uses: tj-actions/verify-changed-files@v16
+      uses: tj-actions/verify-changed-files@v19
       id: verify-changed-files
       with:
         files: ./coverage/coverage.svg
 
     - name: Commit & push coverage badge
       if: steps.verify-changed-files.outputs.files_changed == 'true'
       run: |
```

### Comparing `pytensils-1.0.0/.github/workflows/publish-pypi.yml` & `pytensils-1.1.0/.github/workflows/publish-pypi.yml`

 * *Files 19% similar despite different names*

```diff
@@ -16,20 +16,20 @@
       name: PyPI
       url: https://pypi.org/p/pytensils
     permissions:
       id-token: write
 
     steps:
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Set up Python
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v5
         with:
           python-version: '3.x'
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install build
```

### Comparing `pytensils-1.0.0/.github/workflows/unit-tests.yml` & `pytensils-1.1.0/.github/workflows/unit-tests.yml`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,20 @@
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
       with:
         fetch-depth: 0
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install flake8 pytest
```

### Comparing `pytensils-1.0.0/LICENSE` & `pytensils-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytensils-1.0.0/PKG-INFO` & `pytensils-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytensils
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python package that provides general utility functions for managing configuration, user-logging, directories and data-types as well as a basic run-time profiler.
 Home-page: https://github.com/thomaseleff/pytensils
 Author: Tom Eleff
 Author-email: tome18@comcast.net
 Project-URL: Issues, https://github.com/thomaseleff/pytensils/issues
 Project-URL: Releases, https://github.com/thomaseleff/pytensils/releases
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pytensils-1.0.0/README.md` & `pytensils-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pytensils-1.0.0/coverage/COVERAGE.md` & `pytensils-1.1.0/coverage/COVERAGE.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 | Name                      |    Stmts |     Miss |    Cover |   Missing |
 |-------------------------- | -------: | -------: | -------: | --------: |
-| pytensils/\_\_init\_\_.py |        6 |        0 |     100% |           |
-| pytensils/config.py       |      131 |        0 |     100% |           |
-| pytensils/logging.py      |      125 |        0 |     100% |           |
+| pytensils/\_\_init\_\_.py |        7 |        0 |     100% |           |
+| pytensils/config.py       |      129 |        0 |     100% |           |
+| pytensils/errors.py       |       21 |        0 |     100% |           |
+| pytensils/logging.py      |      137 |        0 |     100% |           |
 | pytensils/profiler.py     |       12 |        0 |     100% |           |
 | pytensils/utils.py        |       32 |        0 |     100% |           |
-|                 **TOTAL** |  **306** |    **0** | **100%** |           |
+|                 **TOTAL** |  **338** |    **0** | **100%** |           |
```

### Comparing `pytensils-1.0.0/coverage/coverage.svg` & `pytensils-1.1.0/coverage/coverage.svg`

 * *Files identical despite different names*

### Comparing `pytensils-1.0.0/pytensils/config.py` & `pytensils-1.1.0/pytensils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Information
 ---------------------------------------------------------------------
 Name        : config.py
 Location    : ~/
 Author      : Tom Eleff
 Published   : 2024-03-19
-Revised on  : 2024-03-24
+Revised on  : 2024-04-15
 
 Description
 ---------------------------------------------------------------------
 Contains the `class` methods for managing configuration.
 """
 
 import os
 import json
 import copy
 import pandas as pd
 from typing import Union, Tuple
-from pytensils import logging
+from pytensils import logging, errors
 
 # Private static variable(s)
 _MIN_DEPTH = 2
 
 
 class Handler():
 
@@ -68,24 +68,26 @@
                     header='Configuration validation'
                 )
                 self._LOGGING.write(
                     content='{%s} does not exist.' % (path),
                     level='ERROR'
                 )
                 self._LOGGING.close()
-                raise OSError(
+                raise errors.config.OSError(
                     'Path not found. See {%s} for more information.' % (
                         os.path.join(
                             self._LOGGING.path,
                             self._LOGGING.file_name
                         )
                     )
                 )
             else:
-                raise OSError('{%s} does not exist.' % (path))
+                raise errors.config.OSError(
+                    '{%s} does not exist.' % (path)
+                )
 
         # Validate the file-name
         if not create:
             if os.path.isfile(
                 os.path.join(path, file_name)
             ):
                 self.data = self.read()
@@ -103,24 +105,24 @@
                             path
                         ),
                         level='ERROR'
                     )
                     self._LOGGING.close()
 
                     # Raise exception
-                    raise FileNotFoundError(
+                    raise errors.config.FileNotFoundError(
                         'File not found. See {%s} for more information.' % (
                             os.path.join(
                                 self._LOGGING.path,
                                 self._LOGGING.file_name
                             )
                         )
                     )
                 else:
-                    raise FileNotFoundError(
+                    raise errors.config.FileNotFoundError(
                         '{%s} does not exist within {%s}.' % (
                             file_name,
                             path
                         )
                     )
 
     def read(self) -> dict:
@@ -179,27 +181,27 @@
                             self.file_name
                         ),
                         level='ERROR'
                     )
                     self._LOGGING.close()
 
                     # Raise exception
-                    raise TypeError(
+                    raise errors.config.TypeError(
                         ''.join([
                             'Invalid config-file format.',
                             ' See {%s} for more information.' % (
                                 os.path.join(
                                     self._LOGGING.path,
                                     self._LOGGING.file_name
                                 )
                             )
                         ])
                     )
                 else:
-                    raise TypeError(
+                    raise errors.config.TypeError(
                         "{%s} is not a valid '.json' config-file." % (
                             self.file_name
                         )
                     )
 
     def write(self):
         """ Writes a '.json' config-file.
@@ -332,15 +334,15 @@
             type(dict_object).__name__,
             parameter
         )
 
         if not isinstance(dict_object, dict):
             if self._LOGGING:
                 self._raise_general_validation_error(error_msg=error_msg)
-            raise ValidationError(error_msg)
+            raise errors.config.ValidationError(error_msg)
 
     def _validate_data(
         self,
         dict_object: dict,
         parameter: str
     ):
         """ Validates the data in `dict_object`.
@@ -356,15 +358,15 @@
             parameter
         )
 
         if not dict_object:
             if self._LOGGING:
                 self._raise_general_validation_error(error_msg=error_msg)
             else:
-                raise ValidationError(error_msg)
+                raise errors.config.ValidationError(error_msg)
 
     def _validate_depth(
         self,
         dict_object: dict,
         parameter: str
     ):
         """ Validates the depth of `dict_object`.
@@ -385,15 +387,15 @@
 
         if not logging._return_dictionary_depth(
             dict_object=dict_object
         ) >= _MIN_DEPTH:
             if self._LOGGING:
                 self._raise_general_validation_error(error_msg=error_msg)
             else:
-                raise ValidationError(error_msg)
+                raise errors.config.ValidationError(error_msg)
 
     def _validate_dtypes(
         self,
         dict_object: dict,
         dtype_object: dict
     ):
         """ Validates `dict_object` against the dtypes in `dtype_object`.
@@ -421,15 +423,15 @@
         if error:
             self.validation_errors = copy.deepcopy(dtype_errors)
 
             # Raise configuration dtype errors
             if self._LOGGING:
                 self._raise_dtype_validation_error(error_msg=error_msg)
             else:
-                raise ValidationError(
+                raise errors.config.ValidationError(
                     ''.join([
                         error_msg,
                         '\n%s' % (
                             json.dumps(dtype_errors, indent=2)
                         )
                     ])
                 )
@@ -451,15 +453,15 @@
         self._LOGGING.write(
             content=error_msg,
             level='ERROR'
         )
         self._LOGGING.close()
 
         # Raise exception
-        raise ValidationError(
+        raise errors.config.ValidationError(
             ''.join([
                 'Validation failed.',
                 ' See {%s} for more information.' % (
                     os.path.join(
                         self._LOGGING.path,
                         self._LOGGING.file_name
                     )
@@ -487,15 +489,15 @@
             content=self._convert_dtype_errors_to_df(
                 dict_object=self.validation_errors
             )
         )
         self._LOGGING.close()
 
         # Raise exception
-        raise ValidationError(
+        raise errors.config.ValidationError(
             ''.join([
                 'Validation failed.',
                 ' See {%s} for more information.' % (
                     os.path.join(
                         self._LOGGING.path,
                         self._LOGGING.file_name
                     )
@@ -578,11 +580,7 @@
                     )
                 ],
                 axis=0,
                 ignore_index=True
             )
 
         return df
-
-
-class ValidationError(Exception):
-    pass
```

### Comparing `pytensils-1.0.0/pytensils/logging.py` & `pytensils-1.1.0/pytensils/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 """
 Information
 ---------------------------------------------------------------------
 Name        : logging.py
 Location    : ~/
 Author      : Tom Eleff
 Published   : 2024-03-24
-Revised on  : .
+Revised on  : 2024-04-16
 
 Description
 ---------------------------------------------------------------------
 Contains the `class` methods for 'pretty' user-logging.
 """
 
 import os
 import textwrap
 import tabulate
 import inspect
 import datetime as dt
 import pytz
-import logging as clogging
+import logging
 import pandas as pd
+from pytensils import errors
 from typing import Union, Callable
 
 # Static variable(s)
 INDENT = 4
 LINE_LENGTH = 79
 TIMEZONE = 'America/New_York'
 
 # Private static variable(s)
 _MAX_DEPTH = 1
 
 # Setup CPython logging
-clogging.basicConfig(
-    level=clogging.DEBUG,
-    format='[DEBUG] %(message)s'
-)
+pytensils = logging.getLogger('pytensils')
+pytensils.setLevel(level=logging.DEBUG)
+debugger = logging.StreamHandler()
+debugger.setLevel(level=logging.DEBUG)
+debugger.setFormatter(fmt=logging.Formatter('[DEBUG] %(message)s'))
+pytensils.addHandler(hdlr=debugger)
 
 # Setup tabulate
 tabulate.PRESERVE_WHITESPACE = True
 
 
 class Handler():
 
@@ -58,15 +61,15 @@
         path : `str`
             Directory path to the folder that contains the `file_name` of the
                 log-file.
         file_name : `str`
             File name of the log-file.
         description : `str`
             Information about the executed Python job run.
-        metadata : `str`
+        metadata : `dict`
             Environment parameters to display as metadata about the executed
                 Python job run.
         create: `bool`
             `True` or `False`, creates an empty log-file, `file_name`
                 within `path` when `True`.
         debug_console: `bool`
             `True` or `False`, outputs the logging content to the console
@@ -301,25 +304,41 @@
             content=''.join(['-'*(self._LINE_LENGTH-self._INDENT-1), '\n'])
         )
 
     def close_on_exception(
         self,
         func: Callable
     ) -> Callable:
-        """ Logs any unhandled exception raised by the {func} passed.
+        """ Logs any unhandled exception raised by the `func` passed.
 
         Parameters
         ----------
         func : `Callable`
             Function object.
         """
 
         def wrapper(*args, **kwargs):
             try:
                 result = func(*args, **kwargs)
+
+            # Raise all `pytensils` exceptions
+            except errors.config.all() as e:
+                errors.config.raise_exception(
+                    msg=(
+                        'See {%s} for more information.' % (
+                            os.path.join(
+                                self.path,
+                                self.file_name
+                            )
+                        )
+                    ),
+                    exception=e
+                )
+
+            # Raise all other exceptions
             except Exception as e:
 
                 self.write_header(
                     header='Unhandled exception'
                 )
                 self.write(
                     content=(
@@ -464,15 +483,15 @@
                 [''.join(
                     [' '*self._INDENT, string]
                 ) for string in strings]
             )
 
         # Debug
         if self.debug_console:
-            clogging.debug(string.replace('\n', '\n[DEBUG] '))
+            pytensils.debug(string.replace('\n', '\n[DEBUG] '))
 
         return ''.join([string, '\n'])
 
     def _pretty_list(
         self,
         list_object: list
     ) -> str:
@@ -492,23 +511,22 @@
                 )
             ]
             + [
                 self._pretty_str(
                     string=''.join([
                         ' '*self._INDENT,
                         '- ',
-                        textwrap.shorten(
-                            text=str(item),
+                        self._pretty_textwrap(
+                            string=str(item),
                             width=(
                                 self._LINE_LENGTH
                                 - self._INDENT
                                 - self._INDENT
                                 - 3
-                            ),
-                            break_long_words=True
+                            )
                         )
                     ])
                 ) for item in list_object
             ]
         )
 
     def _pretty_dict(
@@ -538,25 +556,24 @@
                 + [
                     self._pretty_str(
                         string=''.join([
                             ' '*self._INDENT,
                             key,
                             ' '*(max_key_length-len(key)+self._INDENT),
                             ': ',
-                            textwrap.shorten(
-                                str(dict_object[key]),
+                            self._pretty_textwrap(
+                                string=str(dict_object[key]),
                                 width=(
                                     self._LINE_LENGTH
                                     - self._INDENT
                                     - self._INDENT
                                     - max_key_length
                                     - self._INDENT
                                     - 3
-                                ),
-                                break_long_words=True
+                                )
                             )
                         ])
                     ) for key in list(dict_object.keys())
                 ]
             )
         else:
             raise ValueError(
@@ -613,46 +630,73 @@
         if _return_dictionary_depth(
             dict_object=dict_object
         ) == _MAX_DEPTH:
             return True
         else:
             return False
 
+    def _pretty_textwrap(
+        self,
+        string: str,
+        width: int
+    ) -> str:
+        """ Returns a 'pretty' formatted shortened string.
+
+        Parameters
+        ----------
+        string : `str`
+            String to 'pretty' format.
+        width : `int`
+            The maximum width of the returned string.
+        """
+        if len(string) >= width and ' ' not in string:
+            return '[...]'.join(
+                [
+                    string[:(width-round(width/2)-5)],
+                    string[(len(string)-round(width/2)):]]
+            )
+        else:
+            return textwrap.shorten(
+                str(string),
+                width=width,
+                break_long_words=True
+            )
+
 
 def _validate_level(level: str):
     """ Validates the `level` scope for logging.
 
     Parameters
     ----------
-    level: `str`
+    level : `str`
         Any level available by `logging`.
 
             e.g., [
                 'CRITICAL',
                 'ERROR',
                 'WARNING',
                 'INFO',
                 'DEBUG',
                 'NOTSET'
             ]
     """
     try:
-        clogging._checkLevel(level=level)
+        logging._checkLevel(level=level)
     except ValueError:
         raise ValueError(
             'Invalid level {%s}.' % (level)
         )
 
 
 def _return_level_substring(level: str):
     """ Returns the substring corresponding to level.
 
     Parameters
     ----------
-    level: `str`
+    level : `str`
         Any level available by `logging`.
 
             e.g., [
                 'CRITICAL',
                 'ERROR',
                 'WARNING',
                 'INFO',
```

### Comparing `pytensils-1.0.0/pytensils/profiler.py` & `pytensils-1.1.0/pytensils/profiler.py`

 * *Files identical despite different names*

### Comparing `pytensils-1.0.0/pytensils/utils.py` & `pytensils-1.1.0/pytensils/utils.py`

 * *Files identical despite different names*

### Comparing `pytensils-1.0.0/pytensils.egg-info/PKG-INFO` & `pytensils-1.1.0/pytensils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytensils
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python package that provides general utility functions for managing configuration, user-logging, directories and data-types as well as a basic run-time profiler.
 Home-page: https://github.com/thomaseleff/pytensils
 Author: Tom Eleff
 Author-email: tome18@comcast.net
 Project-URL: Issues, https://github.com/thomaseleff/pytensils/issues
 Project-URL: Releases, https://github.com/thomaseleff/pytensils/releases
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pytensils-1.0.0/setup.cfg` & `pytensils-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytensils-1.0.0/tests/resources/closes-on-exception-success.log` & `pytensils-1.1.0/tests/resources/closes-on-exception-success.log`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
     Run information
     ---------------
     
     Generates close-on-exception content for `pytenstils.logging`
         functionality.
     
-        Start time    : 2024-03-24 17:33:18
+        Start time    : 2024-04-16 16:25:47
     
     --------------------------------------------------------------------------
     
     Run time
     --------
     
     Run-time performance summary.
     
-        Start time    : 17:33:18.617200
-        End time      : 17:33:18.751646
-        Run time      : 00:00:00.134446
+        Start time    : 16:25:47.013383
+        End time      : 16:25:47.118085
+        Run time      : 00:00:00.104702
 
     --------------------------------------------------------------------------
```

### Comparing `pytensils-1.0.0/tests/resources/closes-on-exception.log` & `pytensils-1.1.0/tests/resources/closes-on-exception-notimplementederror.log`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,35 @@
     Run information
     ---------------
     
     Generates close-on-exception content for `pytenstils.logging`
         functionality.
     
-        Start time    : 2024-03-24 17:33:18
+        Start time    : 2024-04-16 16:25:47
     
     --------------------------------------------------------------------------
     
     Unhandled exception
     -------------------
     
 *** CRITICAL: The process failed due to an unhandled exception.
 
-    >>> ZeroDivisionError: division by zero
+    >>> NotImplementedError: The exception {ValueError} is not implemented for
+        `pytensils.config`.
     
-        Filename       : T:\Documents\Projects\Pytensils\tests\test_logging.py
-        Line Number    : Line 322
-        Function       : divide_by_zero()
-        Exception      : ZeroDivisionError
+        Filename       : T:\Documents\Projects\Pytensils\pytensils\errors.py
+        Line Number    : Line 66
+        Function       : raise_exception()
+        Exception      : NotImplementedError
     
     --------------------------------------------------------------------------
     
     Run time
     --------
     
     Run-time performance summary.
     
-        Start time    : 17:33:18.819100
-        End time      : 17:33:19.108891
-        Run time      : 00:00:00.289791
+        Start time    : 16:25:47.784523
+        End time      : 16:25:48.040522
+        Run time      : 00:00:00.255999
 
     --------------------------------------------------------------------------
```

### Comparing `pytensils-1.0.0/tests/resources/compare.log` & `pytensils-1.1.0/tests/resources/compare.log`

 * *Files 7% similar despite different names*

```diff
@@ -25,34 +25,38 @@
     --------------------------------------------------------------------------
     
     Examples: `list`
     ----------------
     
     This is a list output.
     
+        - This string is longer than 89 characters and will be truncated [...]
+        - Thisstringislongerthan89chara[...]causinganemptystringtobedisplayed.
         - 0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 [...]
         - ['A', 'B', 'C']
         - ('A', 'B', 'C')
         - 1
         - 2
         - 3
     
     --------------------------------------------------------------------------
     
     Examples: `dict`
     ----------------
     
     This is a dictionary output.
     
-        A                      : a
-        B                      : b
-        123s                   : 0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 [...]
-        Nineteen characters    : 19
-        List                   : ['A', 'B', 'C']
-        Tupple                 : ('A', 'B', 'C')
+        A                              : a
+        B                              : b
+        With whitespace, > 89-chars    : This string is longer than 89 [...]
+        No whitespace, > 89-chars      : Thisstringislo[...]ringtobedisplayed.
+        123s                           : 0 1 2 3 4 5 6 7 8 9 10 11 12 13 [...]
+        Nineteen characters            : 19
+        List                           : ['A', 'B', 'C']
+        Tupple                         : ('A', 'B', 'C')
     
     --------------------------------------------------------------------------
     
     Examples: `pd.DataFrame`
     ------------------------
     
     This is a dataframe output.
```

### Comparing `pytensils-1.0.0/tests/resources/test_config.log` & `pytensils-1.1.0/tests/resources/test_config.log`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
     Run information
     ---------------
     
     Environment information summary.
     
-        Start time    : 2024-03-24 17:33:17
+        Start time    : 2024-04-16 16:25:45
     
     --------------------------------------------------------------------------
     
     Configuration validation
     ------------------------
     
 *** ERROR: Validation failed. The following parameter values are inconsistent
@@ -27,12 +27,12 @@
     --------------------------------------------------------------------------
     
     Run time
     --------
     
     Run-time performance summary.
     
-        Start time    : 17:33:17.722692
-        End time      : 17:33:17.875570
-        Run time      : 00:00:00.152878
+        Start time    : 16:25:45.955076
+        End time      : 16:25:46.129457
+        Run time      : 00:00:00.174381
 
     --------------------------------------------------------------------------
```

### Comparing `pytensils-1.0.0/tests/test_config.py` & `pytensils-1.1.0/tests/test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 Description
 ---------------------------------------------------------------------
 Tests methods within `pytensils.config`.
 """
 
 import os
 import pytest
-from pytensils import config, logging
+from pytensils import config, logging, errors
 
 PATH = os.path.join(
     os.path.dirname(__file__),
     'resources'
 )
 
 
@@ -212,82 +212,82 @@
     assert CONFIG_FIXTURE.validate(
         dtypes=DTYPES_FIXTURE.to_dict()
     )
     assert not CONFIG_FIXTURE.validation_errors
 
 
 def test_validate_instance_validationerror(CONFIG_FIXTURE: config.Handler):
-    with pytest.raises(config.ValidationError):
+    with pytest.raises(errors.config.ValidationError):
         CONFIG_FIXTURE._validate_instance(
             dict_object=['A', 'B', 'C"'],
             parameter='invalid-instance-dict-object'
         )
 
 
 def test_validate_instance_logging_validationerror(
     CONFIG_FIXTURE_WITH_LOGGING: config.Handler
 ):
-    with pytest.raises(config.ValidationError):
+    with pytest.raises(errors.config.ValidationError):
         CONFIG_FIXTURE_WITH_LOGGING._validate_instance(
             dict_object=['A', 'B', 'C"'],
             parameter='invalid-instance-dict-object'
         )
 
 
 def test_validate_data_validationerror(CONFIG_FIXTURE: config.Handler):
-    with pytest.raises(config.ValidationError):
+    with pytest.raises(errors.config.ValidationError):
         CONFIG_FIXTURE._validate_data(
             dict_object={},
             parameter='empty-dict-object'
         )
 
 
 def test_validate_data_logging_validationerror(
     CONFIG_FIXTURE_WITH_LOGGING: config.Handler
 ):
-    with pytest.raises(config.ValidationError):
+    with pytest.raises(errors.config.ValidationError):
         CONFIG_FIXTURE_WITH_LOGGING._validate_data(
             dict_object={},
             parameter='empty-dict-object'
         )
 
 
 def test_validate_depth_validationerror(CONFIG_FIXTURE: config.Handler):
-    with pytest.raises(config.ValidationError):
+    with pytest.raises(errors.config.ValidationError):
         CONFIG_FIXTURE._validate_depth(
             dict_object={'A': 'str'},
             parameter='invalid-depth-dict-object'
         )
 
 
 def test_validate_depth_logging_validationerror(
     CONFIG_FIXTURE_WITH_LOGGING: config.Handler
 ):
-    with pytest.raises(config.ValidationError):
+    with pytest.raises(errors.config.ValidationError):
         CONFIG_FIXTURE_WITH_LOGGING._validate_depth(
             dict_object={'A': 'str'},
             parameter='invalid-depth-dict-object'
         )
 
 
 def test_validate_dtypes_validationerror(
     CONFIG_VALIDATION_ERROR_FIXTURE: config.Handler,
     DTYPES_FIXTURE: config.Handler
 ):
-    with pytest.raises(config.ValidationError):
+    with pytest.raises(errors.config.ValidationError):
         CONFIG_VALIDATION_ERROR_FIXTURE.validate(
             dtypes=DTYPES_FIXTURE.to_dict()
         )
 
 
 def test_validate_dtypes_logging_validationerror(
     CONFIG_VALIDATION_ERROR_FIXTURE_WITH_LOGGING: config.Handler,
     DTYPES_FIXTURE: config.Handler
 ):
-    with pytest.raises(config.ValidationError):
+    with pytest.raises(errors.config.ValidationError):
         CONFIG_VALIDATION_ERROR_FIXTURE_WITH_LOGGING.validate(
             dtypes=DTYPES_FIXTURE.to_dict()
         )
 
 
 def test_write_success(tmp_path):
```

### Comparing `pytensils-1.0.0/tests/test_logging.py` & `pytensils-1.1.0/tests/test_logging.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Tests methods within `pytensils.logging`.
 """
 
 import os
 import pandas as pd
 import logging as clogging
 import pytest
-from pytensils import logging
+from pytensils import logging, errors
 
 PATH = os.path.join(
     os.path.dirname(__file__),
     'resources'
 )
 
 
@@ -40,14 +40,20 @@
         create=True,
         debug_console=False
     )
 
 
 def test_logging_success(LOGGING_FIXTURE: logging.Handler):
 
+    string = ''.join([
+        'This string is longer than 89 characters',
+        ' and will be truncated causing an empty string to be displayed.'
+    ])
+    string_no_whitespace = string.replace(' ', '')
+
     # Generate `str` test(s)
     LOGGING_FIXTURE.write_header(
         header='Examples: `str`'
     )
     LOGGING_FIXTURE.write(
         content='This is a critical error string',
         level='CRITICAL'
@@ -85,14 +91,16 @@
         divider=True
     )
     LOGGING_FIXTURE.write(
         content='This is a list output.'
     )
     LOGGING_FIXTURE.write(
         content=[
+            string,
+            string_no_whitespace,
             ' '.join(str(i) for i in list(range(52))),
             ['A', 'B', 'C'],
             ('A', 'B', 'C'),
             1,
             2,
             3,
         ]
@@ -106,14 +114,16 @@
     LOGGING_FIXTURE.write(
         content='This is a dictionary output.'
     )
     LOGGING_FIXTURE.write(
         content={
             'A': 'a',
             'B': 'b',
+            'With whitespace, > 89-chars': string,
+            'No whitespace, > 89-chars': string_no_whitespace,
             '123s': ' '.join(str(i) for i in list(range(52))),
             'Nineteen characters': 19,
             'List': ['A', 'B', 'C'],
             'Tupple': ('A', 'B', 'C')
         }
     )
 
@@ -148,19 +158,19 @@
     test.close()
     compare.close()
 
     # Assert both test and compare are the same length
     assert len(test_lines) == len(compare_lines)
 
     # Assert test and compare contain the same content
-    #   Skip lines 6, 72, 73, 74 as these contain
+    #   Skip lines 6, 76, 77, 78 as these contain
     #   date-time values that cannot be compared due
     #   to different execution windows.
     for index in range(len(test_lines)):
-        if index not in [6, 72, 73, 74]:
+        if index not in [6, 76, 77, 78]:
             assert test_lines[index] == compare_lines[index]
 
 
 def test_init_oserror():
     with pytest.raises(OSError):
         _ = logging.Handler(
             path=os.path.join(
@@ -318,7 +328,132 @@
         )
 
         @Logging.close_on_exception
         def divide_by_zero():
             return 1 / 0
 
         divide_by_zero()
+
+
+def test_logging_close_on_exception_oserror():
+    with pytest.raises(OSError):
+
+        # Initialize logging
+        Logging = logging.Handler(
+            path=PATH,
+            file_name='closes-on-exception-oserror.log',
+            description=''.join([
+                'Generates close-on-exception content for',
+                ' `pytenstils.logging` functionality.'
+            ]),
+            create=True,
+            debug_console=False
+        )
+
+        @Logging.close_on_exception
+        def raise_oserror():
+            errors.config.raise_exception(
+                msg='',
+                exception=errors.config.OSError()
+            )
+
+        raise_oserror()
+
+
+def test_logging_close_on_exception_filenotfounderror():
+    with pytest.raises(FileNotFoundError):
+
+        # Initialize logging
+        Logging = logging.Handler(
+            path=PATH,
+            file_name='closes-on-exception-filenotfounderror.log',
+            description=''.join([
+                'Generates close-on-exception content for',
+                ' `pytenstils.logging` functionality.'
+            ]),
+            create=True,
+            debug_console=False
+        )
+
+        @Logging.close_on_exception
+        def raise_filenotfounderror():
+            errors.config.raise_exception(
+                msg='',
+                exception=errors.config.FileNotFoundError()
+            )
+
+        raise_filenotfounderror()
+
+
+def test_logging_close_on_exception_typeerror():
+    with pytest.raises(TypeError):
+
+        # Initialize logging
+        Logging = logging.Handler(
+            path=PATH,
+            file_name='closes-on-exception-typeerror.log',
+            description=''.join([
+                'Generates close-on-exception content for',
+                ' `pytenstils.logging` functionality.'
+            ]),
+            create=True,
+            debug_console=False
+        )
+
+        @Logging.close_on_exception
+        def raise_typeerror():
+            errors.config.raise_exception(
+                msg='',
+                exception=errors.config.TypeError()
+            )
+
+        raise_typeerror()
+
+
+def test_logging_close_on_exception_validationerror():
+    with pytest.raises(errors.config.ValidationError):
+
+        # Initialize logging
+        Logging = logging.Handler(
+            path=PATH,
+            file_name='closes-on-exception-validationerror.log',
+            description=''.join([
+                'Generates close-on-exception content for',
+                ' `pytenstils.logging` functionality.'
+            ]),
+            create=True,
+            debug_console=False
+        )
+
+        @Logging.close_on_exception
+        def raise_validationerror():
+            errors.config.raise_exception(
+                msg='',
+                exception=errors.config.ValidationError()
+            )
+
+        raise_validationerror()
+
+
+def test_logging_close_on_exception_notimplementederror():
+    with pytest.raises(NotImplementedError):
+
+        # Initialize logging
+        Logging = logging.Handler(
+            path=PATH,
+            file_name='closes-on-exception-notimplementederror.log',
+            description=''.join([
+                'Generates close-on-exception content for',
+                ' `pytenstils.logging` functionality.'
+            ]),
+            create=True,
+            debug_console=False
+        )
+
+        @Logging.close_on_exception
+        def raise_notimplementederror():
+            errors.config.raise_exception(
+                msg='',
+                exception=ValueError()
+            )
+
+        raise_notimplementederror()
```

### Comparing `pytensils-1.0.0/tests/test_utils.py` & `pytensils-1.1.0/tests/test_utils.py`

 * *Files identical despite different names*

