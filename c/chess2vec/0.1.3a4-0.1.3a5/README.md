# Comparing `tmp/chess2vec-0.1.3a4.tar.gz` & `tmp/chess2vec-0.1.3a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.1.3a4.tar", max compression
+gzip compressed data, was "chess2vec-0.1.3a5.tar", max compression
```

## Comparing `chess2vec-0.1.3a4.tar` & `chess2vec-0.1.3a5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.3a4/README.md
--rw-r--r--   0        0        0     4269 2024-04-16 20:14:47.019039 chess2vec-0.1.3a4/chess2vec/__init__.py
--rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.3a4/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
--rw-r--r--   0        0        0      740 2024-04-16 16:21:07.852284 chess2vec-0.1.3a4/chess2vec/_utils/sparse.py
--rw-r--r--   0        0        0      538 2024-04-16 16:46:49.087490 chess2vec-0.1.3a4/chess2vec/_utils/vector.py
--rw-r--r--   0        0        0      341 2024-04-16 20:15:37.999153 chess2vec-0.1.3a4/pyproject.toml
--rw-r--r--   0        0        0      525 1970-01-01 00:00:00.000000 chess2vec-0.1.3a4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.3a5/README.md
+-rw-r--r--   0        0        0     4229 2024-04-16 20:16:30.752606 chess2vec-0.1.3a5/chess2vec/__init__.py
+-rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.3a5/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
+-rw-r--r--   0        0        0      740 2024-04-16 16:21:07.852284 chess2vec-0.1.3a5/chess2vec/_utils/sparse.py
+-rw-r--r--   0        0        0      538 2024-04-16 16:46:49.087490 chess2vec-0.1.3a5/chess2vec/_utils/vector.py
+-rw-r--r--   0        0        0      341 2024-04-16 20:16:38.462623 chess2vec-0.1.3a5/pyproject.toml
+-rw-r--r--   0        0        0      525 1970-01-01 00:00:00.000000 chess2vec-0.1.3a5/PKG-INFO
```

### Comparing `chess2vec-0.1.3a4/chess2vec/__init__.py` & `chess2vec-0.1.3a5/chess2vec/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,14 @@
                         rows.append(row_idx)
                     case _:
                         columns.append(VEC_BLOCK * (pt - 1) + idx)
                         rows.append(row_idx)
 
             row_idx += 1
 
-        print(len(rows), len(columns))
-
         mat = scipy.sparse.csr_matrix(
             (
                 np.ones_like(columns, dtype=np.uint8),
                 (rows, columns),
             ),
             shape=(row_idx, VEC_SIZE),
         )
```

### Comparing `chess2vec-0.1.3a4/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc` & `chess2vec-0.1.3a5/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.3a4/chess2vec/_utils/sparse.py` & `chess2vec-0.1.3a5/chess2vec/_utils/sparse.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.3a4/chess2vec/_utils/vector.py` & `chess2vec-0.1.3a5/chess2vec/_utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.3a4/PKG-INFO` & `chess2vec-0.1.3a5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.1.3a4
+Version: 0.1.3a5
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

