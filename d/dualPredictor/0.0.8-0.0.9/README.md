# Comparing `tmp/dualPredictor-0.0.8.tar.gz` & `tmp/dualPredictor-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dualPredictor-0.0.8.tar", last modified: Wed Apr 10 11:34:04 2024, max compression
+gzip compressed data, was "dualPredictor-0.0.9.tar", last modified: Fri Apr 12 10:12:40 2024, max compression
```

## Comparing `dualPredictor-0.0.8.tar` & `dualPredictor-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:34:04.026487 dualPredictor-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-10 11:34:00.000000 dualPredictor-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-10 11:34:04.026487 dualPredictor-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-10 11:34:00.000000 dualPredictor-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:34:04.022487 dualPredictor-0.0.8/dualPredictor/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-10 11:34:00.000000 dualPredictor-0.0.8/dualPredictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-10 11:34:00.000000 dualPredictor-0.0.8/dualPredictor/dual_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-10 11:34:00.000000 dualPredictor-0.0.8/dualPredictor/model_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:34:04.026487 dualPredictor-0.0.8/dualPredictor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-10 11:34:04.000000 dualPredictor-0.0.8/dualPredictor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-10 11:34:04.000000 dualPredictor-0.0.8/dualPredictor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:34:04.000000 dualPredictor-0.0.8/dualPredictor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:34:04.000000 dualPredictor-0.0.8/dualPredictor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 11:34:04.000000 dualPredictor-0.0.8/dualPredictor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:34:04.026487 dualPredictor-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-10 11:34:01.000000 dualPredictor-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:12:40.128827 dualPredictor-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-12 10:12:36.000000 dualPredictor-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-12 10:12:40.128827 dualPredictor-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-12 10:12:36.000000 dualPredictor-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:12:40.124827 dualPredictor-0.0.9/dualPredictor/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-12 10:12:36.000000 dualPredictor-0.0.9/dualPredictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-12 10:12:36.000000 dualPredictor-0.0.9/dualPredictor/df_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-12 10:12:36.000000 dualPredictor-0.0.9/dualPredictor/dual_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-12 10:12:36.000000 dualPredictor-0.0.9/dualPredictor/model_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:12:40.128827 dualPredictor-0.0.9/dualPredictor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-12 10:12:40.000000 dualPredictor-0.0.9/dualPredictor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-12 10:12:40.000000 dualPredictor-0.0.9/dualPredictor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:12:40.000000 dualPredictor-0.0.9/dualPredictor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-12 10:12:40.000000 dualPredictor-0.0.9/dualPredictor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 10:12:40.000000 dualPredictor-0.0.9/dualPredictor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 10:12:40.128827 dualPredictor-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-12 10:12:36.000000 dualPredictor-0.0.9/setup.py
```

### Comparing `dualPredictor-0.0.8/LICENSE` & `dualPredictor-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dualPredictor-0.0.8/PKG-INFO` & `dualPredictor-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dualPredictor
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python package for simultaneous regression and binary classification for educational analytics.
 Home-page: https://github.com/098765d/dualPredictor.git
 Author: Dong
 Author-email: no@email.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -17,14 +17,15 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scikit-learn
 Requires-Dist: matplotlib
+Requires-Dist: shap
 Requires-Dist: seaborn
 
 # dualPredictor: An Open-Source Tool for Simultaneously Grade Prediction and At-Risk Student Classification
 
 by Dong, Cheng, and Kan
 
 ## Introduction
```

### Comparing `dualPredictor-0.0.8/README.md` & `dualPredictor-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dualPredictor-0.0.8/dualPredictor/dual_model.py` & `dualPredictor-0.0.9/dualPredictor/dual_model.py`

 * *Files identical despite different names*

### Comparing `dualPredictor-0.0.8/dualPredictor.egg-info/PKG-INFO` & `dualPredictor-0.0.9/dualPredictor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dualPredictor
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python package for simultaneous regression and binary classification for educational analytics.
 Home-page: https://github.com/098765d/dualPredictor.git
 Author: Dong
 Author-email: no@email.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -17,14 +17,15 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scikit-learn
 Requires-Dist: matplotlib
+Requires-Dist: shap
 Requires-Dist: seaborn
 
 # dualPredictor: An Open-Source Tool for Simultaneously Grade Prediction and At-Risk Student Classification
 
 by Dong, Cheng, and Kan
 
 ## Introduction
```

### Comparing `dualPredictor-0.0.8/setup.py` & `dualPredictor-0.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dualPredictor",
-    version="0.0.8",
+    version="0.0.9",
     author="Dong",
     author_email="no@email.com",
     description="A Python package for simultaneous regression and binary classification for educational analytics.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/098765d/dualPredictor.git",
     packages=find_packages(),
     install_requires=[
         "numpy",
         "scikit-learn",
         "matplotlib",
+        "shap",
         "seaborn",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
```

