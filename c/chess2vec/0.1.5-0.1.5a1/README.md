# Comparing `tmp/chess2vec-0.1.5.tar.gz` & `tmp/chess2vec-0.1.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.1.5.tar", max compression
+gzip compressed data, was "chess2vec-0.1.5a1.tar", max compression
```

## Comparing `chess2vec-0.1.5.tar` & `chess2vec-0.1.5a1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.5/README.md
--rw-r--r--   0        0        0     4534 2024-04-16 20:57:39.492311 chess2vec-0.1.5/chess2vec/__init__.py
--rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.5/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
--rw-r--r--   0        0        0      740 2024-04-16 16:21:07.852284 chess2vec-0.1.5/chess2vec/_utils/sparse.py
--rw-r--r--   0        0        0      538 2024-04-16 16:46:49.087490 chess2vec-0.1.5/chess2vec/_utils/vector.py
--rw-r--r--   0        0        0      365 2024-04-16 21:02:33.556559 chess2vec-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 chess2vec-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.5a1/README.md
+-rw-r--r--   0        0        0     4530 2024-04-16 21:07:11.287967 chess2vec-0.1.5a1/chess2vec/__init__.py
+-rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.5a1/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
+-rw-r--r--   0        0        0      740 2024-04-16 16:21:07.852284 chess2vec-0.1.5a1/chess2vec/_utils/sparse.py
+-rw-r--r--   0        0        0      538 2024-04-16 16:46:49.087490 chess2vec-0.1.5a1/chess2vec/_utils/vector.py
+-rw-r--r--   0        0        0      367 2024-04-16 21:07:29.854369 chess2vec-0.1.5a1/pyproject.toml
+-rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 chess2vec-0.1.5a1/PKG-INFO
```

### Comparing `chess2vec-0.1.5/chess2vec/__init__.py` & `chess2vec-0.1.5a1/chess2vec/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
                 )
 
                 positions = list(loaded["positions"])
 
             self._actions_matrix = scipy.sparse.vstack([self._actions_matrix, mat])
             self.positions += positions
 
-    def save_npz(self, file) -> None:
+    def save(self, file) -> None:
         np.savez_compressed(
             file,
             mat_indices=self._actions_matrix.indices,
             mat_indptr=self._actions_matrix.indptr,
             size=self.size,
             positions=self.positions,
         )
```

### Comparing `chess2vec-0.1.5/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc` & `chess2vec-0.1.5a1/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.5/chess2vec/_utils/sparse.py` & `chess2vec-0.1.5a1/chess2vec/_utils/sparse.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.5/chess2vec/_utils/vector.py` & `chess2vec-0.1.5a1/chess2vec/_utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.5/PKG-INFO` & `chess2vec-0.1.5a1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.1.5
+Version: 0.1.5a1
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

