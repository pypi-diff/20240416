# Comparing `tmp/augmented_matrix_solver-0.2.tar.gz` & `tmp/augmented_matrix_solver-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "augmented_matrix_solver-0.2.tar", last modified: Mon Apr 15 23:01:23 2024, max compression
+gzip compressed data, was "augmented_matrix_solver-0.3.tar", last modified: Tue Apr 16 17:23:54 2024, max compression
```

## Comparing `augmented_matrix_solver-0.2.tar` & `augmented_matrix_solver-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-15 23:01:23.294839 augmented_matrix_solver-0.2/
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-15 23:01:23.294434 augmented_matrix_solver-0.2/Augmented_Matrix_Solver.egg-info/
--rw-r--r--   0 yumengliu   (501) staff       (20)     1985 2024-04-15 23:01:23.000000 augmented_matrix_solver-0.2/Augmented_Matrix_Solver.egg-info/PKG-INFO
--rw-r--r--   0 yumengliu   (501) staff       (20)      362 2024-04-15 23:01:23.000000 augmented_matrix_solver-0.2/Augmented_Matrix_Solver.egg-info/SOURCES.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)        1 2024-04-15 23:01:23.000000 augmented_matrix_solver-0.2/Augmented_Matrix_Solver.egg-info/dependency_links.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)        6 2024-04-15 23:01:23.000000 augmented_matrix_solver-0.2/Augmented_Matrix_Solver.egg-info/requires.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)       17 2024-04-15 23:01:23.000000 augmented_matrix_solver-0.2/Augmented_Matrix_Solver.egg-info/top_level.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)     1068 2024-04-15 19:47:36.000000 augmented_matrix_solver-0.2/LICENSE
--rw-r--r--   0 yumengliu   (501) staff       (20)     1985 2024-04-15 23:01:23.294647 augmented_matrix_solver-0.2/PKG-INFO
--rw-r--r--   0 yumengliu   (501) staff       (20)      136 2024-04-15 22:06:06.000000 augmented_matrix_solver-0.2/README.md
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-15 23:01:23.293938 augmented_matrix_solver-0.2/augmented_matrix/
--rw-r--r--   0 yumengliu   (501) staff       (20)       32 2024-04-15 23:00:31.000000 augmented_matrix_solver-0.2/augmented_matrix/__init__.py
--rw-r--r--   0 yumengliu   (501) staff       (20)     3603 2024-04-15 23:00:19.000000 augmented_matrix_solver-0.2/augmented_matrix/augmented_matrix.py
--rw-r--r--   0 yumengliu   (501) staff       (20)      621 2024-04-15 23:01:15.000000 augmented_matrix_solver-0.2/pyproject.toml
--rw-r--r--   0 yumengliu   (501) staff       (20)       38 2024-04-15 23:01:23.294886 augmented_matrix_solver-0.2/setup.cfg
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-15 23:01:23.294176 augmented_matrix_solver-0.2/test/
--rw-r--r--   0 yumengliu   (501) staff       (20)     1706 2024-04-15 23:00:19.000000 augmented_matrix_solver-0.2/test/test_augmented_matrix.py
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-16 17:23:54.278234 augmented_matrix_solver-0.3/
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-16 17:23:54.277845 augmented_matrix_solver-0.3/Augmented_Matrix_Solver.egg-info/
+-rw-r--r--   0 yumengliu   (501) staff       (20)     2016 2024-04-16 17:23:54.000000 augmented_matrix_solver-0.3/Augmented_Matrix_Solver.egg-info/PKG-INFO
+-rw-r--r--   0 yumengliu   (501) staff       (20)      362 2024-04-16 17:23:54.000000 augmented_matrix_solver-0.3/Augmented_Matrix_Solver.egg-info/SOURCES.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)        1 2024-04-16 17:23:54.000000 augmented_matrix_solver-0.3/Augmented_Matrix_Solver.egg-info/dependency_links.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)        6 2024-04-16 17:23:54.000000 augmented_matrix_solver-0.3/Augmented_Matrix_Solver.egg-info/requires.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)       17 2024-04-16 17:23:54.000000 augmented_matrix_solver-0.3/Augmented_Matrix_Solver.egg-info/top_level.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)     1068 2024-04-15 19:47:36.000000 augmented_matrix_solver-0.3/LICENSE
+-rw-r--r--   0 yumengliu   (501) staff       (20)     2016 2024-04-16 17:23:54.278047 augmented_matrix_solver-0.3/PKG-INFO
+-rw-r--r--   0 yumengliu   (501) staff       (20)      168 2024-04-16 17:23:36.000000 augmented_matrix_solver-0.3/README.md
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-16 17:23:54.277218 augmented_matrix_solver-0.3/augmented_matrix/
+-rw-r--r--   0 yumengliu   (501) staff       (20)       32 2024-04-15 23:00:31.000000 augmented_matrix_solver-0.3/augmented_matrix/__init__.py
+-rw-r--r--   0 yumengliu   (501) staff       (20)     3603 2024-04-15 23:00:19.000000 augmented_matrix_solver-0.3/augmented_matrix/augmented_matrix.py
+-rw-r--r--   0 yumengliu   (501) staff       (20)      620 2024-04-16 17:23:36.000000 augmented_matrix_solver-0.3/pyproject.toml
+-rw-r--r--   0 yumengliu   (501) staff       (20)       38 2024-04-16 17:23:54.278277 augmented_matrix_solver-0.3/setup.cfg
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-16 17:23:54.277535 augmented_matrix_solver-0.3/test/
+-rw-r--r--   0 yumengliu   (501) staff       (20)     1706 2024-04-15 23:00:19.000000 augmented_matrix_solver-0.3/test/test_augmented_matrix.py
```

### Comparing `augmented_matrix_solver-0.2/Augmented_Matrix_Solver.egg-info/PKG-INFO` & `augmented_matrix_solver-0.3/Augmented_Matrix_Solver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Augmented-Matrix-Solver
-Version: 0.2
+Version: 0.3
 Summary: A package that solves augmented matrices into reduced echelon forms
 Author-email: Yumeng Liu <lym20041026@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,17 @@
         SOFTWARE.
 Project-URL: Repository, https://github.com/YumengLiu6044/GaussianElimination
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.12
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 
 This is a package that contains a class 
 for representing and solving augmented matrices
 of any dimension using Gauss-Jordan Elimination
+
+Requires python version >= 3.9
```

### Comparing `augmented_matrix_solver-0.2/LICENSE` & `augmented_matrix_solver-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `augmented_matrix_solver-0.2/PKG-INFO` & `augmented_matrix_solver-0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Augmented-Matrix-Solver
-Version: 0.2
+Version: 0.3
 Summary: A package that solves augmented matrices into reduced echelon forms
 Author-email: Yumeng Liu <lym20041026@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,17 @@
         SOFTWARE.
 Project-URL: Repository, https://github.com/YumengLiu6044/GaussianElimination
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.12
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 
 This is a package that contains a class 
 for representing and solving augmented matrices
 of any dimension using Gauss-Jordan Elimination
+
+Requires python version >= 3.9
```

### Comparing `augmented_matrix_solver-0.2/augmented_matrix/augmented_matrix.py` & `augmented_matrix_solver-0.3/augmented_matrix/augmented_matrix.py`

 * *Files identical despite different names*

### Comparing `augmented_matrix_solver-0.2/pyproject.toml` & `augmented_matrix_solver-0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "Augmented-Matrix-Solver"
-version = "0.2"
+version = "0.3"
 authors = [
   { name="Yumeng Liu", email="lym20041026@gmail.com" }
 ]
 description = "A package that solves augmented matrices into reduced echelon forms"
 readme = "README.md"
-requires-python = ">=3.12"
+requires-python = ">=3.9"
 dependencies= ['numpy']
 license= { file='LICENSE' }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `augmented_matrix_solver-0.2/test/test_augmented_matrix.py` & `augmented_matrix_solver-0.3/test/test_augmented_matrix.py`

 * *Files identical despite different names*

