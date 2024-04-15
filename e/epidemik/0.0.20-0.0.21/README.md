# Comparing `tmp/epidemik-0.0.20.tar.gz` & `tmp/epidemik-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epidemik-0.0.20.tar", last modified: Sat Apr 13 16:10:52 2024, max compression
+gzip compressed data, was "epidemik-0.0.21.tar", last modified: Mon Apr 15 23:56:09 2024, max compression
```

## Comparing `epidemik-0.0.20.tar` & `epidemik-0.0.21.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:10:52.133417 epidemik-0.0.20/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-13 16:10:43.000000 epidemik-0.0.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-04-13 16:10:52.133417 epidemik-0.0.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-13 16:10:43.000000 epidemik-0.0.20/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-13 16:10:43.000000 epidemik-0.0.20/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 16:10:52.133417 epidemik-0.0.20/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:10:52.129418 epidemik-0.0.20/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:10:52.129418 epidemik-0.0.20/src/epidemik/
--rw-r--r--   0 runner    (1001) docker     (127)    18449 2024-04-13 16:10:43.000000 epidemik-0.0.20/src/epidemik/EpiModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    10417 2024-04-13 16:10:43.000000 epidemik-0.0.20/src/epidemik/MetaEpiModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-13 16:10:43.000000 epidemik-0.0.20/src/epidemik/NetworkEpiModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-13 16:10:43.000000 epidemik-0.0.20/src/epidemik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-13 16:10:43.000000 epidemik-0.0.20/src/epidemik/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:10:52.133417 epidemik-0.0.20/src/epidemik.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-04-13 16:10:52.000000 epidemik-0.0.20/src/epidemik.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-13 16:10:52.000000 epidemik-0.0.20/src/epidemik.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 16:10:52.000000 epidemik-0.0.20/src/epidemik.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-13 16:10:52.000000 epidemik-0.0.20/src/epidemik.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 16:10:52.000000 epidemik-0.0.20/src/epidemik.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:10:52.133417 epidemik-0.0.20/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-13 16:10:43.000000 epidemik-0.0.20/tests/tests_EpiModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-13 16:10:43.000000 epidemik-0.0.20/tests/tests_MetaEpiModel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:56:09.643789 epidemik-0.0.21/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-15 23:56:05.000000 epidemik-0.0.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-04-15 23:56:09.643789 epidemik-0.0.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-15 23:56:05.000000 epidemik-0.0.21/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-15 23:56:05.000000 epidemik-0.0.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 23:56:09.643789 epidemik-0.0.21/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:56:09.639789 epidemik-0.0.21/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:56:09.639789 epidemik-0.0.21/src/epidemik/
+-rw-r--r--   0 runner    (1001) docker     (127)    18449 2024-04-15 23:56:05.000000 epidemik-0.0.21/src/epidemik/EpiModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10417 2024-04-15 23:56:05.000000 epidemik-0.0.21/src/epidemik/MetaEpiModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-15 23:56:05.000000 epidemik-0.0.21/src/epidemik/NetworkEpiModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-15 23:56:05.000000 epidemik-0.0.21/src/epidemik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-15 23:56:05.000000 epidemik-0.0.21/src/epidemik/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:56:09.639789 epidemik-0.0.21/src/epidemik.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-04-15 23:56:09.000000 epidemik-0.0.21/src/epidemik.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-15 23:56:09.000000 epidemik-0.0.21/src/epidemik.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 23:56:09.000000 epidemik-0.0.21/src/epidemik.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 23:56:09.000000 epidemik-0.0.21/src/epidemik.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 23:56:09.000000 epidemik-0.0.21/src/epidemik.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:56:09.639789 epidemik-0.0.21/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-15 23:56:05.000000 epidemik-0.0.21/tests/tests_EpiModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-15 23:56:05.000000 epidemik-0.0.21/tests/tests_MetaEpiModel.py
```

### Comparing `epidemik-0.0.20/LICENSE` & `epidemik-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.20/PKG-INFO` & `epidemik-0.0.21/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: epidemik
-Version: 0.0.20
-Summary: A pakage to simulate compartmental epidemic models
+Version: 0.0.21
+Summary: A package to simulate compartmental epidemic models
 Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
 Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
+Project-URL: Documentation, https://epidemik.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.3
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: epidemik Version: 0.0.20 Summary: A pakage to
+Metadata-Version: 2.1 Name: epidemik Version: 0.0.21 Summary: A package to
 simulate compartmental epidemic models Author-email: Bruno GonÃ§alves
 data4sci.com> Project-URL: Homepage, https://github.com/DataForScience/epidemik
-Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: matplotlib>=3.3 Requires-Dist: networkx>=3 Requires-
-Dist: numpy>=1.20 Requires-Dist: pandas>=2.0 Requires-Dist: scipy>=1.10
-Requires-Dist: tqdm>=4
+Project-URL: Issues, https://github.com/DataForScience/epidemik/issues Project-
+URL: Documentation, https://epidemik.readthedocs.io/ Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Requires-Python: >=3.8
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+matplotlib>=3.3 Requires-Dist: networkx>=3 Requires-Dist: numpy>=1.20 Requires-
+Dist: pandas>=2.0 Requires-Dist: scipy>=1.10 Requires-Dist: tqdm>=4
     [https://raw.githubusercontent.com/DataForScience/epidemik/main/images/
                                  epidemik.png]
 # epidemik Compartmental Epidemic Models in Python --- ## Table of contents[![]
 (https://raw.githubusercontent.com/DataForScience/epidemik/main/images/
 pin.svg)](#toc) - [Installation](#installation) - [Tech Stack](#tech) - [Usage]
 (#usage) - [Contributing](#contributing) - [License](#license) --- ##
 Installation[![](https://raw.githubusercontent.com/DataForScience/epidemik/
```

### Comparing `epidemik-0.0.20/README.md` & `epidemik-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.20/pyproject.toml` & `epidemik-0.0.21/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "epidemik"
 dynamic = ["version"]
 authors = [
   { name="Bruno Gonçalves", email="bgoncalves@data4sci.com" },
 ]
-description = "A pakage to simulate compartmental epidemic models"
+description = "A package to simulate compartmental epidemic models"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
@@ -19,14 +19,15 @@
  "pandas>=2.0",
  "scipy>=1.10",
  "tqdm>=4"
 ]
 [project.urls]
 Homepage = "https://github.com/DataForScience/epidemik"
 Issues = "https://github.com/DataForScience/epidemik/issues"
+Documentation = "https://epidemik.readthedocs.io/"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.dynamic]
 version = {attr = "epidemik.__version__"}
```

### Comparing `epidemik-0.0.20/src/epidemik/EpiModel.py` & `epidemik-0.0.21/src/epidemik/EpiModel.py`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.20/src/epidemik/MetaEpiModel.py` & `epidemik-0.0.21/src/epidemik/MetaEpiModel.py`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.20/src/epidemik/NetworkEpiModel.py` & `epidemik-0.0.21/src/epidemik/NetworkEpiModel.py`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.20/src/epidemik.egg-info/PKG-INFO` & `epidemik-0.0.21/src/epidemik.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: epidemik
-Version: 0.0.20
-Summary: A pakage to simulate compartmental epidemic models
+Version: 0.0.21
+Summary: A package to simulate compartmental epidemic models
 Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
 Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
+Project-URL: Documentation, https://epidemik.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.3
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: epidemik Version: 0.0.20 Summary: A pakage to
+Metadata-Version: 2.1 Name: epidemik Version: 0.0.21 Summary: A package to
 simulate compartmental epidemic models Author-email: Bruno GonÃ§alves
 data4sci.com> Project-URL: Homepage, https://github.com/DataForScience/epidemik
-Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: matplotlib>=3.3 Requires-Dist: networkx>=3 Requires-
-Dist: numpy>=1.20 Requires-Dist: pandas>=2.0 Requires-Dist: scipy>=1.10
-Requires-Dist: tqdm>=4
+Project-URL: Issues, https://github.com/DataForScience/epidemik/issues Project-
+URL: Documentation, https://epidemik.readthedocs.io/ Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Requires-Python: >=3.8
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+matplotlib>=3.3 Requires-Dist: networkx>=3 Requires-Dist: numpy>=1.20 Requires-
+Dist: pandas>=2.0 Requires-Dist: scipy>=1.10 Requires-Dist: tqdm>=4
     [https://raw.githubusercontent.com/DataForScience/epidemik/main/images/
                                  epidemik.png]
 # epidemik Compartmental Epidemic Models in Python --- ## Table of contents[![]
 (https://raw.githubusercontent.com/DataForScience/epidemik/main/images/
 pin.svg)](#toc) - [Installation](#installation) - [Tech Stack](#tech) - [Usage]
 (#usage) - [Contributing](#contributing) - [License](#license) --- ##
 Installation[![](https://raw.githubusercontent.com/DataForScience/epidemik/
```

### Comparing `epidemik-0.0.20/tests/tests_EpiModel.py` & `epidemik-0.0.21/tests/tests_EpiModel.py`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.20/tests/tests_MetaEpiModel.py` & `epidemik-0.0.21/tests/tests_MetaEpiModel.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import unittest
 import pandas as pd
 from epidemik import MetaEpiModel
 from epidemik.utils import NotInitialized
 
 class MetaEpiModelTestCase(unittest.TestCase):
 	def setUp(self):
-		self.travel = pd.DataFrame({'A': [0.9, 0.1], 'B':[0.1, 0.9]}, index=["A", "B"])
-		self.population = pd.DataFrame({'Population':[100000, 10000]}, index=["A", "B"])
+		self.travel = pd.DataFrame({'A': [0.99, 0.1], 'B':[0.01, 0.9]}, index=["A", "B"])
+		self.population = pd.DataFrame({'Population':[100_000, 10_000]}, index=["A", "B"])
 
 		self.SIR = MetaEpiModel(self.travel, self.population)
 		self.beta = 0.3
 		self.mu = 0.1
 		self.SIR.add_interaction('S', 'I', 'I', self.beta)
 		self.SIR.add_spontaneous('I', 'R', self.mu)
```

