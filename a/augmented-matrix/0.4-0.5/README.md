# Comparing `tmp/augmented_matrix-0.4.tar.gz` & `tmp/augmented_matrix-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "augmented_matrix-0.4.tar", last modified: Tue Apr 16 17:46:48 2024, max compression
+gzip compressed data, was "augmented_matrix-0.5.tar", last modified: Tue Apr 16 20:14:26 2024, max compression
```

## Comparing `augmented_matrix-0.4.tar` & `augmented_matrix-0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-16 17:46:48.921843 augmented_matrix-0.4/
--rw-r--r--   0 yumengliu   (501) staff       (20)     1068 2024-04-15 19:47:36.000000 augmented_matrix-0.4/LICENSE
--rw-r--r--   0 yumengliu   (501) staff       (20)     2009 2024-04-16 17:46:48.921640 augmented_matrix-0.4/PKG-INFO
--rw-r--r--   0 yumengliu   (501) staff       (20)      168 2024-04-16 17:23:36.000000 augmented_matrix-0.4/README.md
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-16 17:46:48.920247 augmented_matrix-0.4/augmented_matrix/
--rw-r--r--   0 yumengliu   (501) staff       (20)       32 2024-04-15 23:00:31.000000 augmented_matrix-0.4/augmented_matrix/__init__.py
--rw-r--r--   0 yumengliu   (501) staff       (20)     3603 2024-04-15 23:00:19.000000 augmented_matrix-0.4/augmented_matrix/augmented_matrix.py
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-16 17:46:48.921420 augmented_matrix-0.4/augmented_matrix.egg-info/
--rw-r--r--   0 yumengliu   (501) staff       (20)     2009 2024-04-16 17:46:48.000000 augmented_matrix-0.4/augmented_matrix.egg-info/PKG-INFO
--rw-r--r--   0 yumengliu   (501) staff       (20)      327 2024-04-16 17:46:48.000000 augmented_matrix-0.4/augmented_matrix.egg-info/SOURCES.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)        1 2024-04-16 17:46:48.000000 augmented_matrix-0.4/augmented_matrix.egg-info/dependency_links.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)        6 2024-04-16 17:46:48.000000 augmented_matrix-0.4/augmented_matrix.egg-info/requires.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)       17 2024-04-16 17:46:48.000000 augmented_matrix-0.4/augmented_matrix.egg-info/top_level.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)      613 2024-04-16 17:46:18.000000 augmented_matrix-0.4/pyproject.toml
--rw-r--r--   0 yumengliu   (501) staff       (20)       38 2024-04-16 17:46:48.921884 augmented_matrix-0.4/setup.cfg
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-16 17:46:48.921115 augmented_matrix-0.4/test/
--rw-r--r--   0 yumengliu   (501) staff       (20)     1706 2024-04-15 23:00:19.000000 augmented_matrix-0.4/test/test_augmented_matrix.py
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-16 20:14:26.848850 augmented_matrix-0.5/
+-rw-r--r--   0 yumengliu   (501) staff       (20)     1068 2024-04-15 19:47:36.000000 augmented_matrix-0.5/LICENSE
+-rw-r--r--   0 yumengliu   (501) staff       (20)     2009 2024-04-16 20:14:26.848667 augmented_matrix-0.5/PKG-INFO
+-rw-r--r--   0 yumengliu   (501) staff       (20)      168 2024-04-16 17:23:36.000000 augmented_matrix-0.5/README.md
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-16 20:14:26.846768 augmented_matrix-0.5/augmented_matrix/
+-rw-r--r--   0 yumengliu   (501) staff       (20)       32 2024-04-15 23:00:31.000000 augmented_matrix-0.5/augmented_matrix/__init__.py
+-rw-r--r--   0 yumengliu   (501) staff       (20)     4742 2024-04-16 20:10:39.000000 augmented_matrix-0.5/augmented_matrix/augmented_matrix.py
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-16 20:14:26.848462 augmented_matrix-0.5/augmented_matrix.egg-info/
+-rw-r--r--   0 yumengliu   (501) staff       (20)     2009 2024-04-16 20:14:26.000000 augmented_matrix-0.5/augmented_matrix.egg-info/PKG-INFO
+-rw-r--r--   0 yumengliu   (501) staff       (20)      327 2024-04-16 20:14:26.000000 augmented_matrix-0.5/augmented_matrix.egg-info/SOURCES.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)        1 2024-04-16 20:14:26.000000 augmented_matrix-0.5/augmented_matrix.egg-info/dependency_links.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)        6 2024-04-16 20:14:26.000000 augmented_matrix-0.5/augmented_matrix.egg-info/requires.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)       17 2024-04-16 20:14:26.000000 augmented_matrix-0.5/augmented_matrix.egg-info/top_level.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)      613 2024-04-16 19:08:09.000000 augmented_matrix-0.5/pyproject.toml
+-rw-r--r--   0 yumengliu   (501) staff       (20)       38 2024-04-16 20:14:26.849003 augmented_matrix-0.5/setup.cfg
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-16 20:14:26.848064 augmented_matrix-0.5/test/
+-rw-r--r--   0 yumengliu   (501) staff       (20)     2255 2024-04-16 20:10:05.000000 augmented_matrix-0.5/test/test_augmented_matrix.py
```

### Comparing `augmented_matrix-0.4/LICENSE` & `augmented_matrix-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `augmented_matrix-0.4/PKG-INFO` & `augmented_matrix-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augmented-matrix
-Version: 0.4
+Version: 0.5
 Summary: A package that solves augmented matrices into reduced echelon forms
 Author-email: Yumeng Liu <lym20041026@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `augmented_matrix-0.4/augmented_matrix/augmented_matrix.py` & `augmented_matrix-0.5/augmented_matrix/augmented_matrix.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,116 +1,148 @@
 import numpy as np
 
-NON_SIMPLIFIED = -1
-UPPER_TRIANGULAR = 0
-REDUCED_ECHELON = 1
-
 
 class NoSolutionError(Exception):
     pass
 
 
-class AugmentedMatrix(np.ndarray):
-    def __new__(cls, *args, **kwargs):
+class AugmentedMatrix:
+    def __init__(self, matrix, constraint=None, /, **kwargs):
+        if constraint is not None:
+            constraint = np.asarray(constraint, **kwargs)
+            matrix = np.append(matrix, [[i] for i in constraint], axis=1)
+
+        self._matrix = np.asarray(matrix, **kwargs)
+
+    @property
+    def matrix(self) -> np.ndarray:
+        """
+        :return: the augmented matrix
+        """
+        return self._matrix
 
-        return np.asarray(*args, **kwargs).view(cls)
+    def set_matrix(self, matrix):
+        self._matrix = matrix
 
-    def _check_valid_solution(self):
+    def check_valid_solution(self):
         """
         Checks if the matrix is consistent
-        :return:
+        :raises NoSolutionError: If the matrix is not consistent
         """
-        for row in self:
+        matrix = self._matrix
+        for row in matrix:
             if all(x == 0 for x in row[:-1]):
                 if row[-1] != 0:
                     raise NoSolutionError('No solution exists!')
 
-    def partial_pivot(self):
+    def check_upper_triangular(self) -> bool:
+        """
+        Checks if the matrix is in upper triangular form
+        :returns True: if the matrix is in upper triangular form
+        :returns False: if the matrix is not in upper triangular form
+        """
+        matrix = self._matrix
+        row, column = 0, 0
+        while row < (matrix.shape[0] - 1) and column < matrix.shape[1]:
+            if all(x == 0 for x in matrix[:, column][row + 1:]):
+                row += 1
+                column += 1
+            else:
+                return False
+
+        return True
+
+    def partial_pivot(self) -> np.ndarray:
         """
         Transforms the matrix into upper triangular form by partial pivoting
+
+        :return: the upper triangular form of the matrix
         """
+        matrix = self._matrix
         row, column = 0, 0
-        while row < (row_count := self.shape[0]) and column < self.shape[1]:
+        while row < (row_count := matrix.shape[0]) and column < matrix.shape[1]:
             # Use the highest absolute value as pivot
             max_row_index = row
-            for i in range(row, self.shape[0]):
-                if abs(self[i][column]) > abs(self[max_row_index][column]):
+            for i in range(row, matrix.shape[0]):
+                if abs(matrix[i][column]) > abs(matrix[max_row_index][column]):
                     max_row_index = i
 
-            self[[row, max_row_index]] = self[[max_row_index, row]]
+            matrix[[row, max_row_index]] = matrix[[max_row_index, row]]
 
-            pivot = self[row][column]
+            pivot = matrix[row][column]
             if pivot != 0:
                 for i in range(row + 1, row_count):
-                    leading_value = self[i][column]
+                    leading_value = matrix[i][column]
                     if leading_value == 0:
                         continue
                     factor = -1 * pivot / leading_value
-                    self[i] = factor * self[i] + self[row]
+                    matrix[i] = factor * matrix[i] + matrix[row]
 
             column += 1
             row = column
 
-    def _simplify_echelon(self):
+        self._matrix = matrix
+        return matrix
+
+    def simplify_echelon(self) -> np.ndarray:
         """
         Simplifies the upper triangular form so that the pivots are 1
         """
+        matrix = self._matrix
         # Simplify the echelon form
-        for row_index in range(self.shape[0]):
+        for row_index in range(matrix.shape[0]):
             pivot = 1
-            for element in self[row_index]:
+            for element in matrix[row_index]:
                 if element != 0:
                     pivot = element
                     break
-            self[row_index] = self[row_index] / pivot
+            matrix[row_index] = matrix[row_index] / pivot
 
-    def _get_state(self):
-        row, column = 0, 0
-        while row < (self.shape[0] - 1) and column < self.shape[1]:
-            if all(x == 0 for x in self[:, column][row+1:]):
-                row += 1
-                column += 1
-            else:
-                return NON_SIMPLIFIED
-
-        return UPPER_TRIANGULAR
+        self._matrix = matrix
+        return matrix
 
-    def reduce_echelon(self):
+    def reduce_echelon(self) -> np.ndarray:
         """
         Transforms the matrix from upper triangular form to reduced echelon form
         :raise: NoSolutionException: if the matrix has no solution
         """
-        if self._get_state() != UPPER_TRIANGULAR:
+        if not self.check_upper_triangular():
             self.partial_pivot()
 
-        self._check_valid_solution()
-        self._simplify_echelon()
+        self.check_valid_solution()
+        self.simplify_echelon()
 
-        for row_index in range(self.shape[0] - 1, -1, -1):
+        matrix = self._matrix
+        for row_index in range(matrix.shape[0] - 1, -1, -1):
             pivot_coord = None
-            for element_index in range(self.shape[1] - 1):
-                if self[row_index][element_index] != 0:
+            for element_index in range(matrix.shape[1] - 1):
+                if matrix[row_index][element_index] != 0:
                     pivot_coord = [row_index, element_index]
                     break
 
             if pivot_coord is None:
                 continue
             else:
                 for i in range(row_index):
-                    leading = self[i][pivot_coord[1]]
+                    leading = matrix[i][pivot_coord[1]]
                     if leading == 0:
                         continue
 
-                    pivot = self[pivot_coord[0]][pivot_coord[1]]
+                    pivot = matrix[pivot_coord[0]][pivot_coord[1]]
                     factor = -1 * leading / pivot
-                    self[i] = factor * self[pivot_coord[0]] + self[i]
+                    matrix[i] = factor * matrix[pivot_coord[0]] + matrix[i]
 
-    def solve(self):
+        self._matrix = matrix
+        return matrix
+
+    def solve(self) -> np.ndarray:
         """
         Solves the augmented matrix
-        :raise: NoSolutionException: if the matrix has no solution
+        :returns self._matrix: the row-reduced matrix
+        :raises NoSolutionException: if the matrix has no solution
         """
         self.partial_pivot()
         self.reduce_echelon()
+        return self._matrix
 
 
 __all__ = ['AugmentedMatrix', 'NoSolutionError']
```

### Comparing `augmented_matrix-0.4/augmented_matrix.egg-info/PKG-INFO` & `augmented_matrix-0.5/augmented_matrix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augmented-matrix
-Version: 0.4
+Version: 0.5
 Summary: A package that solves augmented matrices into reduced echelon forms
 Author-email: Yumeng Liu <lym20041026@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `augmented_matrix-0.4/pyproject.toml` & `augmented_matrix-0.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "augmented-matrix"
-version = "0.4"
+version = "0.5"
 authors = [
   { name="Yumeng Liu", email="lym20041026@gmail.com" }
 ]
 description = "A package that solves augmented matrices into reduced echelon forms"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies= ['numpy']
```

### Comparing `augmented_matrix-0.4/test/test_augmented_matrix.py` & `augmented_matrix-0.5/test/test_augmented_matrix.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 from fractions import Fraction
 
 
 class TestAugmentedMatrix(unittest.TestCase):
     def _to_fraction(self, original):
         return [[Fraction(j).limit_denominator() for j in i] for i in original]
 
-    def check_solution_equal(self, unsolved, expected):
-        m = AugmentedMatrix(self._to_fraction(unsolved))
+    def check_solution_equal(self, unsolved, expected, constraint=None):
+        if constraint is not None:
+            constraint = [Fraction(j).limit_denominator() for j in constraint]
+        m = AugmentedMatrix(self._to_fraction(unsolved), constraint)
         m.solve()
-        self.assertEqual(m.tolist(), self._to_fraction(expected))
+        self.assertEqual(m.matrix.tolist(), self._to_fraction(expected))
 
     def test_augmented_matrix(self):
         original_matrix = [
             [3, 5, -1, 10],
             [1, 4, 1, 7],
             [9, 0, 2, 1]
         ]
@@ -34,15 +36,15 @@
         ]))
         m.reduce_echelon()
         expected = [
             [1, 0, 0, -1],
             [0, 1, 0, 4],
             [0, 0, 1, -1]
         ]
-        self.assertEqual(m.tolist(), expected)
+        self.assertEqual(m.matrix.tolist(), expected)
 
     def test_augmented_matrix_no_solution(self):
         original = [
             [1, 2, 3],
             [1, 2, 4]
         ]
         with self.assertRaises(NoSolutionError):
@@ -55,10 +57,24 @@
         ]
         expected = [
             [1, 2, 3],
             [0, 0, 0]
         ]
         self.check_solution_equal(original_matrix, expected)
 
+    def test_augmented_matrix_with_constraint(self):
+        original_matrix = [
+            [3, 5, -1],
+            [1, 4, 1],
+            [9, 0, 2]
+        ]
+        constraint = [10, 7, 1]
+        expected = [
+            [1, 0, 0, 0.2],
+            [0, 1, 0, 1.8],
+            [0, 0, 1, -0.4]
+        ]
+        self.check_solution_equal(original_matrix, expected, constraint=constraint)
+
 
 if __name__ == '__main__':
     unittest.main()
```

