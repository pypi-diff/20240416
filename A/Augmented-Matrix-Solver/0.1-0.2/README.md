# Comparing `tmp/augmented_matrix_solver-0.1.tar.gz` & `tmp/augmented_matrix_solver-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "augmented_matrix_solver-0.1.tar", last modified: Mon Apr 15 21:50:49 2024, max compression
+gzip compressed data, was "augmented_matrix_solver-0.2.tar", last modified: Mon Apr 15 23:01:23 2024, max compression
```

## Comparing `augmented_matrix_solver-0.1.tar` & `augmented_matrix_solver-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-15 21:50:49.635383 augmented_matrix_solver-0.1/
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-15 21:50:49.634997 augmented_matrix_solver-0.1/Augmented_Matrix_Solver.egg-info/
--rw-r--r--   0 yumengliu   (501) staff       (20)     1937 2024-04-15 21:50:49.000000 augmented_matrix_solver-0.1/Augmented_Matrix_Solver.egg-info/PKG-INFO
--rw-r--r--   0 yumengliu   (501) staff       (20)      362 2024-04-15 21:50:49.000000 augmented_matrix_solver-0.1/Augmented_Matrix_Solver.egg-info/SOURCES.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)        1 2024-04-15 21:50:49.000000 augmented_matrix_solver-0.1/Augmented_Matrix_Solver.egg-info/dependency_links.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)        6 2024-04-15 21:50:49.000000 augmented_matrix_solver-0.1/Augmented_Matrix_Solver.egg-info/requires.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)       17 2024-04-15 21:50:49.000000 augmented_matrix_solver-0.1/Augmented_Matrix_Solver.egg-info/top_level.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)     1068 2024-04-15 19:47:36.000000 augmented_matrix_solver-0.1/LICENSE
--rw-r--r--   0 yumengliu   (501) staff       (20)     1937 2024-04-15 21:50:49.635187 augmented_matrix_solver-0.1/PKG-INFO
--rw-r--r--   0 yumengliu   (501) staff       (20)       88 2024-04-15 19:16:47.000000 augmented_matrix_solver-0.1/README.md
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-15 21:50:49.634518 augmented_matrix_solver-0.1/augmented_matrix/
--rw-r--r--   0 yumengliu   (501) staff       (20)       46 2024-04-15 20:51:23.000000 augmented_matrix_solver-0.1/augmented_matrix/__init__.py
--rw-r--r--   0 yumengliu   (501) staff       (20)     3584 2024-04-15 21:37:44.000000 augmented_matrix_solver-0.1/augmented_matrix/augmented_matrix.py
--rw-r--r--   0 yumengliu   (501) staff       (20)      621 2024-04-15 21:50:46.000000 augmented_matrix_solver-0.1/pyproject.toml
--rw-r--r--   0 yumengliu   (501) staff       (20)       38 2024-04-15 21:50:49.635420 augmented_matrix_solver-0.1/setup.cfg
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-15 21:50:49.634738 augmented_matrix_solver-0.1/test/
--rw-r--r--   0 yumengliu   (501) staff       (20)     1769 2024-04-15 21:47:11.000000 augmented_matrix_solver-0.1/test/test_augmented_matrix.py
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-15 23:01:23.294839 augmented_matrix_solver-0.2/
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-15 23:01:23.294434 augmented_matrix_solver-0.2/Augmented_Matrix_Solver.egg-info/
+-rw-r--r--   0 yumengliu   (501) staff       (20)     1985 2024-04-15 23:01:23.000000 augmented_matrix_solver-0.2/Augmented_Matrix_Solver.egg-info/PKG-INFO
+-rw-r--r--   0 yumengliu   (501) staff       (20)      362 2024-04-15 23:01:23.000000 augmented_matrix_solver-0.2/Augmented_Matrix_Solver.egg-info/SOURCES.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)        1 2024-04-15 23:01:23.000000 augmented_matrix_solver-0.2/Augmented_Matrix_Solver.egg-info/dependency_links.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)        6 2024-04-15 23:01:23.000000 augmented_matrix_solver-0.2/Augmented_Matrix_Solver.egg-info/requires.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)       17 2024-04-15 23:01:23.000000 augmented_matrix_solver-0.2/Augmented_Matrix_Solver.egg-info/top_level.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)     1068 2024-04-15 19:47:36.000000 augmented_matrix_solver-0.2/LICENSE
+-rw-r--r--   0 yumengliu   (501) staff       (20)     1985 2024-04-15 23:01:23.294647 augmented_matrix_solver-0.2/PKG-INFO
+-rw-r--r--   0 yumengliu   (501) staff       (20)      136 2024-04-15 22:06:06.000000 augmented_matrix_solver-0.2/README.md
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-15 23:01:23.293938 augmented_matrix_solver-0.2/augmented_matrix/
+-rw-r--r--   0 yumengliu   (501) staff       (20)       32 2024-04-15 23:00:31.000000 augmented_matrix_solver-0.2/augmented_matrix/__init__.py
+-rw-r--r--   0 yumengliu   (501) staff       (20)     3603 2024-04-15 23:00:19.000000 augmented_matrix_solver-0.2/augmented_matrix/augmented_matrix.py
+-rw-r--r--   0 yumengliu   (501) staff       (20)      621 2024-04-15 23:01:15.000000 augmented_matrix_solver-0.2/pyproject.toml
+-rw-r--r--   0 yumengliu   (501) staff       (20)       38 2024-04-15 23:01:23.294886 augmented_matrix_solver-0.2/setup.cfg
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-15 23:01:23.294176 augmented_matrix_solver-0.2/test/
+-rw-r--r--   0 yumengliu   (501) staff       (20)     1706 2024-04-15 23:00:19.000000 augmented_matrix_solver-0.2/test/test_augmented_matrix.py
```

### Comparing `augmented_matrix_solver-0.1/Augmented_Matrix_Solver.egg-info/PKG-INFO` & `augmented_matrix_solver-0.2/Augmented_Matrix_Solver.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Augmented-Matrix-Solver
-Version: 0.1
+Version: 0.2
 Summary: A package that solves augmented matrices into reduced echelon forms
 Author-email: Yumeng Liu <lym20041026@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,7 +33,8 @@
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 
 This is a package that contains a class 
 for representing and solving augmented matrices
+of any dimension using Gauss-Jordan Elimination
```

### Comparing `augmented_matrix_solver-0.1/LICENSE` & `augmented_matrix_solver-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `augmented_matrix_solver-0.1/PKG-INFO` & `augmented_matrix_solver-0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Augmented-Matrix-Solver
-Version: 0.1
+Version: 0.2
 Summary: A package that solves augmented matrices into reduced echelon forms
 Author-email: Yumeng Liu <lym20041026@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,7 +33,8 @@
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 
 This is a package that contains a class 
 for representing and solving augmented matrices
+of any dimension using Gauss-Jordan Elimination
```

### Comparing `augmented_matrix_solver-0.1/augmented_matrix/augmented_matrix.py` & `augmented_matrix_solver-0.2/augmented_matrix/augmented_matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,8 +109,8 @@
         Solves the augmented matrix
         :raise: NoSolutionException: if the matrix has no solution
         """
         self.partial_pivot()
         self.reduce_echelon()
 
 
-__all__ = ['AugmentedMatrix']
+__all__ = ['AugmentedMatrix', 'NoSolutionError']
```

### Comparing `augmented_matrix_solver-0.1/pyproject.toml` & `augmented_matrix_solver-0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Augmented-Matrix-Solver"
-version = "0.1"
+version = "0.2"
 authors = [
   { name="Yumeng Liu", email="lym20041026@gmail.com" }
 ]
 description = "A package that solves augmented matrices into reduced echelon forms"
 readme = "README.md"
 requires-python = ">=3.12"
 dependencies= ['numpy']
```

### Comparing `augmented_matrix_solver-0.1/test/test_augmented_matrix.py` & `augmented_matrix_solver-0.2/test/test_augmented_matrix.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import unittest
 from augmented_matrix import *
 from fractions import Fraction
 
-from augmented_matrix.augmented_matrix import NoSolutionError
-
 
 class TestAugmentedMatrix(unittest.TestCase):
     def _to_fraction(self, original):
         return [[Fraction(j).limit_denominator() for j in i] for i in original]
 
     def check_solution_equal(self, unsolved, expected):
         m = AugmentedMatrix(self._to_fraction(unsolved))
```

