# Comparing `tmp/flexible_classifier-0.0.12.tar.gz` & `tmp/flexible_classifier-0.0.2.tar.gz`

## Comparing `flexible_classifier-0.0.12.tar` & `flexible_classifier-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flexible_classifier-0.0.12/src/flexible_classifier/__init__.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 flexible_classifier-0.0.12/src/flexible_classifier/classifier.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flexible_classifier-0.0.12/tests/__init__.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 flexible_classifier-0.0.12/tests/test.py
--rw-r--r--   0        0        0   131249 2020-02-02 00:00:00.000000 flexible_classifier-0.0.12/tests/data/Test.csv
--rw-r--r--   0        0        0   425369 2020-02-02 00:00:00.000000 flexible_classifier-0.0.12/tests/data/Train.csv
--rw-r--r--   0        0        0   210076 2020-02-02 00:00:00.000000 flexible_classifier-0.0.12/tests/data/ds_salaries.csv
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 flexible_classifier-0.0.12/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 flexible_classifier-0.0.12/LICENSE
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 flexible_classifier-0.0.12/README.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 flexible_classifier-0.0.12/pyproject.toml
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 flexible_classifier-0.0.12/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flexible_classifier-0.0.2/src/flexible_classifier/__init__.py
+-rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 flexible_classifier-0.0.2/src/flexible_classifier/classifier.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flexible_classifier-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 flexible_classifier-0.0.2/tests/test.py
+-rw-r--r--   0        0        0   131249 2020-02-02 00:00:00.000000 flexible_classifier-0.0.2/tests/data/Test.csv
+-rw-r--r--   0        0        0   425369 2020-02-02 00:00:00.000000 flexible_classifier-0.0.2/tests/data/Train.csv
+-rw-r--r--   0        0        0   210076 2020-02-02 00:00:00.000000 flexible_classifier-0.0.2/tests/data/ds_salaries.csv
+-rw-r--r--   0        0        0 14856764 2020-02-02 00:00:00.000000 flexible_classifier-0.0.2/tests/data/tortilla_prices.csv
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 flexible_classifier-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 flexible_classifier-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 flexible_classifier-0.0.2/README.md
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 flexible_classifier-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 flexible_classifier-0.0.2/PKG-INFO
```

### Comparing `flexible_classifier-0.0.12/tests/data/Test.csv` & `flexible_classifier-0.0.2/tests/data/Test.csv`

 * *Files identical despite different names*

### Comparing `flexible_classifier-0.0.12/tests/data/Train.csv` & `flexible_classifier-0.0.2/tests/data/Train.csv`

 * *Files identical despite different names*

### Comparing `flexible_classifier-0.0.12/tests/data/ds_salaries.csv` & `flexible_classifier-0.0.2/tests/data/ds_salaries.csv`

 * *Files identical despite different names*

### Comparing `flexible_classifier-0.0.12/.gitignore` & `flexible_classifier-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `flexible_classifier-0.0.12/LICENSE` & `flexible_classifier-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flexible_classifier-0.0.12/README.md` & `flexible_classifier-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `flexible_classifier-0.0.12/pyproject.toml` & `flexible_classifier-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "flexible_classifier"
-version = "0.0.12"
+version = "0.0.2"
 authors = [
   { name="Marko Golovko", email="markgolovko@gmail.com" },
 ]
 description = "Classifier pipeline that can be used to train and evaluate classification models on various datasets"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
+  "numpy==1.24.0",
   "pandas==1.5.3",
   "scikit-learn==1.3.2",
+  "tensorflow==2.16.1",
 ]
 
 [project.urls]
 Homepage = "https://github.com/GameRuiner/classifier-pipeline"
 Issues = "https://github.com/GameRuiner/classifier-pipeline/issues"
```

### Comparing `flexible_classifier-0.0.12/PKG-INFO` & `flexible_classifier-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.3
 Name: flexible_classifier
-Version: 0.0.12
+Version: 0.0.2
 Summary: Classifier pipeline that can be used to train and evaluate classification models on various datasets
 Project-URL: Homepage, https://github.com/GameRuiner/classifier-pipeline
 Project-URL: Issues, https://github.com/GameRuiner/classifier-pipeline/issues
 Author-email: Marko Golovko <markgolovko@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: numpy==1.24.0
 Requires-Dist: pandas==1.5.3
 Requires-Dist: scikit-learn==1.3.2
+Requires-Dist: tensorflow==2.16.1
 Description-Content-Type: text/markdown
 
 # Flexible Classifier Pipeline
 
 This repository contains a flexible classifier pipeline that can be used to train and evaluate classification models on various datasets. The pipeline is designed to be versatile and easily adaptable to different datasets and classification tasks.
 
 ## Overview
```

