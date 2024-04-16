# Comparing `tmp/rai_test_utils-0.4.1.tar.gz` & `tmp/rai_test_utils-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rai_test_utils-0.4.1.tar", last modified: Thu Sep  7 23:08:17 2023, max compression
+gzip compressed data, was "rai_test_utils-0.4.2.tar", last modified: Tue Apr 16 05:49:53 2024, max compression
```

## Comparing `rai_test_utils-0.4.1.tar` & `rai_test_utils-0.4.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 23:08:17.784951 rai_test_utils-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2023-09-07 23:08:17.784951 rai_test_utils-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 23:08:17.780951 rai_test_utils-0.4.1/rai_test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/rai_test_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 23:08:17.780951 rai_test_utils-0.4.1/rai_test_utils/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/rai_test_utils/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 23:08:17.780951 rai_test_utils-0.4.1/rai_test_utils/datasets/tabular/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/rai_test_utils/datasets/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9343 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/rai_test_utils/datasets/tabular/classification_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/rai_test_utils/datasets/tabular/regression_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/rai_test_utils/datasets/tabular/timeseries_data_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 23:08:17.780951 rai_test_utils-0.4.1/rai_test_utils/datasets/vision/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/rai_test_utils/datasets/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7383 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/rai_test_utils/datasets/vision/object_detection_data_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 23:08:17.780951 rai_test_utils-0.4.1/rai_test_utils/models/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/rai_test_utils/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 23:08:17.780951 rai_test_utils-0.4.1/rai_test_utils/models/lightgbm/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/rai_test_utils/models/lightgbm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/rai_test_utils/models/lightgbm/lightgbm_model_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/rai_test_utils/models/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 23:08:17.780951 rai_test_utils-0.4.1/rai_test_utils/models/sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/rai_test_utils/models/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7972 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/rai_test_utils/models/sklearn/sklearn_model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 23:08:17.780951 rai_test_utils-0.4.1/rai_test_utils/models/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/rai_test_utils/models/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/rai_test_utils/models/torch/torch_model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 23:08:17.780951 rai_test_utils-0.4.1/rai_test_utils/models/xgboost/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/rai_test_utils/models/xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/rai_test_utils/models/xgboost/xgboost_model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 23:08:17.784951 rai_test_utils-0.4.1/rai_test_utils/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/rai_test_utils/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/rai_test_utils/utilities/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/rai_test_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 23:08:17.780951 rai_test_utils-0.4.1/rai_test_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2023-09-07 23:08:17.000000 rai_test_utils-0.4.1/rai_test_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2023-09-07 23:08:17.000000 rai_test_utils-0.4.1/rai_test_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-07 23:08:17.000000 rai_test_utils-0.4.1/rai_test_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2023-09-07 23:08:17.000000 rai_test_utils-0.4.1/rai_test_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-09-07 23:08:17.000000 rai_test_utils-0.4.1/rai_test_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-07 23:08:17.784951 rai_test_utils-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 23:08:17.784951 rai_test_utils-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6127 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/tests/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/tests/test_model_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2023-09-07 23:06:09.000000 rai_test_utils-0.4.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:49:53.161387 rai_test_utils-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-16 05:49:53.161387 rai_test_utils-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:49:53.157387 rai_test_utils-0.4.2/rai_test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/rai_test_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:49:53.157387 rai_test_utils-0.4.2/rai_test_utils/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/rai_test_utils/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:49:53.157387 rai_test_utils-0.4.2/rai_test_utils/datasets/tabular/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/rai_test_utils/datasets/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/rai_test_utils/datasets/tabular/classification_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/rai_test_utils/datasets/tabular/regression_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/rai_test_utils/datasets/tabular/timeseries_data_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:49:53.157387 rai_test_utils-0.4.2/rai_test_utils/datasets/vision/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/rai_test_utils/datasets/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/rai_test_utils/datasets/vision/object_detection_data_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:49:53.157387 rai_test_utils-0.4.2/rai_test_utils/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/rai_test_utils/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:49:53.161387 rai_test_utils-0.4.2/rai_test_utils/models/lightgbm/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/rai_test_utils/models/lightgbm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/rai_test_utils/models/lightgbm/lightgbm_model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/rai_test_utils/models/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:49:53.161387 rai_test_utils-0.4.2/rai_test_utils/models/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/rai_test_utils/models/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/rai_test_utils/models/sklearn/sklearn_model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:49:53.161387 rai_test_utils-0.4.2/rai_test_utils/models/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/rai_test_utils/models/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/rai_test_utils/models/torch/torch_model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:49:53.161387 rai_test_utils-0.4.2/rai_test_utils/models/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/rai_test_utils/models/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/rai_test_utils/models/xgboost/xgboost_model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:49:53.161387 rai_test_utils-0.4.2/rai_test_utils/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/rai_test_utils/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/rai_test_utils/utilities/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/rai_test_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:49:53.161387 rai_test_utils-0.4.2/rai_test_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-16 05:49:53.000000 rai_test_utils-0.4.2/rai_test_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-16 05:49:53.000000 rai_test_utils-0.4.2/rai_test_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 05:49:53.000000 rai_test_utils-0.4.2/rai_test_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-16 05:49:53.000000 rai_test_utils-0.4.2/rai_test_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 05:49:53.000000 rai_test_utils-0.4.2/rai_test_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 05:49:53.161387 rai_test_utils-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:49:53.161387 rai_test_utils-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/tests/test_model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-16 05:42:56.000000 rai_test_utils-0.4.2/tests/test_utils.py
```

### Comparing `rai_test_utils-0.4.1/LICENSE` & `rai_test_utils-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.4.1/PKG-INFO` & `rai_test_utils-0.4.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: rai_test_utils
-Version: 0.4.1
+Version: 0.4.2
 Summary: Common basic test utilities used across various RAI tools
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Gaurav Gupta
 Author-email: raiwidgets-maintain@microsoft.com
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: shap
@@ -26,15 +26,15 @@
 Provides-Extra: object-detection
 Requires-Dist: requests; extra == "object-detection"
 Requires-Dist: Pillow>=10.0.0; python_version > "3.7" and extra == "object-detection"
 Requires-Dist: Pillow<10.0.0; python_version <= "3.7" and extra == "object-detection"
 
 # Responsible AI test utilities for Python
 
-### This package has been tested with Python 3.6, 3.7, 3.8, 3.9 and 3.10
+### This package has been tested with Python 3.7, 3.8, 3.9, 3.10 and 3.11
 
 The Responsible AI Test Utilities package contains common testing utilities and functions shared across various RAI tools, including fairlearn, interpret-community, responsibleai, raiwidgets, ml-wrappers and other packages.
 
 Please see the main documentation website:
 https://responsibleaitoolbox.ai/
 
 The open source code can be found here:
```

### Comparing `rai_test_utils-0.4.1/README.md` & `rai_test_utils-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Responsible AI test utilities for Python
 
-### This package has been tested with Python 3.6, 3.7, 3.8, 3.9 and 3.10
+### This package has been tested with Python 3.7, 3.8, 3.9, 3.10 and 3.11
 
 The Responsible AI Test Utilities package contains common testing utilities and functions shared across various RAI tools, including fairlearn, interpret-community, responsibleai, raiwidgets, ml-wrappers and other packages.
 
 Please see the main documentation website:
 https://responsibleaitoolbox.ai/
 
 The open source code can be found here:
```

### Comparing `rai_test_utils-0.4.1/rai_test_utils/datasets/tabular/__init__.py` & `rai_test_utils-0.4.2/rai_test_utils/datasets/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.4.1/rai_test_utils/datasets/tabular/classification_data_utils.py` & `rai_test_utils-0.4.2/rai_test_utils/datasets/tabular/classification_data_utils.py`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.4.1/rai_test_utils/datasets/tabular/regression_data_utils.py` & `rai_test_utils-0.4.2/rai_test_utils/datasets/tabular/regression_data_utils.py`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.4.1/rai_test_utils/datasets/tabular/timeseries_data_utils.py` & `rai_test_utils-0.4.2/rai_test_utils/datasets/tabular/timeseries_data_utils.py`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.4.1/rai_test_utils/datasets/vision/object_detection_data_utils.py` & `rai_test_utils-0.4.2/rai_test_utils/datasets/vision/object_detection_data_utils.py`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.4.1/rai_test_utils/models/lightgbm/lightgbm_model_utils.py` & `rai_test_utils-0.4.2/rai_test_utils/models/lightgbm/lightgbm_model_utils.py`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.4.1/rai_test_utils/models/model_utils.py` & `rai_test_utils-0.4.2/rai_test_utils/models/model_utils.py`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.4.1/rai_test_utils/models/sklearn/__init__.py` & `rai_test_utils-0.4.2/rai_test_utils/models/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.4.1/rai_test_utils/models/sklearn/sklearn_model_utils.py` & `rai_test_utils-0.4.2/rai_test_utils/models/sklearn/sklearn_model_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Copyright (c) Microsoft Corporation
 # Licensed under the MIT License.
 
 import numpy as np
 import pandas as pd
+import sklearn
+from packaging import version
 from sklearn import svm
 from sklearn.compose import ColumnTransformer
 from sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
 from sklearn.impute import SimpleImputer
 from sklearn.linear_model import LogisticRegression
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.pipeline import Pipeline
@@ -123,26 +125,31 @@
     many_to_one_transformer = \
         FunctionTransformer(lambda x: conv(x.sum(axis=1)).reshape(-1, 1))
     many_to_many_transformer = \
         FunctionTransformer(lambda x: np.hstack(
             (conv(np.prod(x, axis=1)).reshape(-1, 1),
                 conv(np.prod(x, axis=1)**2).reshape(-1, 1))
         ))
+    # for older scikit-learn versions use sparse, for newer sparse_output:
+    if version.parse(sklearn.__version__) < version.parse('1.2'):
+        ohe_params = {"sparse": False}
+    else:
+        ohe_params = {"sparse_output": False}
     transformations = ColumnTransformer([
         ("age_fare_1", Pipeline(steps=[
             ('imputer', SimpleImputer(strategy='median')),
             ('scaler', StandardScaler())
         ]), ["age", "fare"]),
         ("age_fare_2", many_to_one_transformer, ["age", "fare"]),
         ("age_fare_3", many_to_many_transformer, ["age", "fare"]),
         ("embarked", Pipeline(steps=[
             ("imputer",
                 SimpleImputer(strategy='constant', fill_value='missing')),
-            ("encoder", OneHotEncoder(sparse=False))]), ["embarked"]),
-        ("sex_pclass", OneHotEncoder(sparse=False), ["sex", "pclass"])
+            ("encoder", OneHotEncoder(**ohe_params))]), ["embarked"]),
+        ("sex_pclass", OneHotEncoder(**ohe_params), ["sex", "pclass"])
     ])
     clf = Pipeline(steps=[('preprocessor', transformations),
                           ('classifier',
                            LogisticRegression(solver='lbfgs'))])
     clf.fit(X_train, y_train)
     return clf
```

### Comparing `rai_test_utils-0.4.1/rai_test_utils/models/torch/torch_model_utils.py` & `rai_test_utils-0.4.2/rai_test_utils/models/torch/torch_model_utils.py`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.4.1/rai_test_utils/models/xgboost/xgboost_model_utils.py` & `rai_test_utils-0.4.2/rai_test_utils/models/xgboost/xgboost_model_utils.py`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.4.1/rai_test_utils/utilities/utils.py` & `rai_test_utils-0.4.2/rai_test_utils/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.4.1/rai_test_utils.egg-info/PKG-INFO` & `rai_test_utils-0.4.2/rai_test_utils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
-Name: rai-test-utils
-Version: 0.4.1
+Name: rai_test_utils
+Version: 0.4.2
 Summary: Common basic test utilities used across various RAI tools
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Gaurav Gupta
 Author-email: raiwidgets-maintain@microsoft.com
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: shap
@@ -26,15 +26,15 @@
 Provides-Extra: object-detection
 Requires-Dist: requests; extra == "object-detection"
 Requires-Dist: Pillow>=10.0.0; python_version > "3.7" and extra == "object-detection"
 Requires-Dist: Pillow<10.0.0; python_version <= "3.7" and extra == "object-detection"
 
 # Responsible AI test utilities for Python
 
-### This package has been tested with Python 3.6, 3.7, 3.8, 3.9 and 3.10
+### This package has been tested with Python 3.7, 3.8, 3.9, 3.10 and 3.11
 
 The Responsible AI Test Utilities package contains common testing utilities and functions shared across various RAI tools, including fairlearn, interpret-community, responsibleai, raiwidgets, ml-wrappers and other packages.
 
 Please see the main documentation website:
 https://responsibleaitoolbox.ai/
 
 The open source code can be found here:
```

### Comparing `rai_test_utils-0.4.1/rai_test_utils.egg-info/SOURCES.txt` & `rai_test_utils-0.4.2/rai_test_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.4.1/setup.py` & `rai_test_utils-0.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,21 @@
     author="Gaurav Gupta",
     author_email="raiwidgets-maintain@microsoft.com",
     description="Common basic test utilities used across various RAI tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/microsoft/responsible-ai-toolbox",
     packages=setuptools.find_packages(),
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     install_requires=install_requires,
     extras_require=extras_require,
     classifiers=[
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 3 - Alpha"
     ]
 )
```

### Comparing `rai_test_utils-0.4.1/tests/test_data_utils.py` & `rai_test_utils-0.4.2/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.4.1/tests/test_model_utils.py` & `rai_test_utils-0.4.2/tests/test_model_utils.py`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.4.1/tests/test_utils.py` & `rai_test_utils-0.4.2/tests/test_utils.py`

 * *Files identical despite different names*

