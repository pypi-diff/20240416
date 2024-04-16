# Comparing `tmp/chess2vec-0.1.3a2.tar.gz` & `tmp/chess2vec-0.1.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.1.3a2.tar", max compression
+gzip compressed data, was "chess2vec-0.1.3a3.tar", max compression
```

## Comparing `chess2vec-0.1.3a2.tar` & `chess2vec-0.1.3a3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.3a2/README.md
--rw-r--r--   0        0        0     4074 2024-04-16 20:00:28.190990 chess2vec-0.1.3a2/chess2vec/__init__.py
--rw-r--r--   0        0        0      740 2024-04-16 16:21:07.852284 chess2vec-0.1.3a2/chess2vec/_utils/sparse.py
--rw-r--r--   0        0        0      538 2024-04-16 16:46:49.087490 chess2vec-0.1.3a2/chess2vec/_utils/vector.py
--rw-r--r--   0        0        0      341 2024-04-16 20:01:14.281020 chess2vec-0.1.3a2/pyproject.toml
--rw-r--r--   0        0        0      525 1970-01-01 00:00:00.000000 chess2vec-0.1.3a2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.3a3/README.md
+-rw-r--r--   0        0        0     4177 2024-04-16 20:03:56.767849 chess2vec-0.1.3a3/chess2vec/__init__.py
+-rw-r--r--   0        0        0      740 2024-04-16 16:21:07.852284 chess2vec-0.1.3a3/chess2vec/_utils/sparse.py
+-rw-r--r--   0        0        0      538 2024-04-16 16:46:49.087490 chess2vec-0.1.3a3/chess2vec/_utils/vector.py
+-rw-r--r--   0        0        0      341 2024-04-16 20:04:06.384528 chess2vec-0.1.3a3/pyproject.toml
+-rw-r--r--   0        0        0      525 1970-01-01 00:00:00.000000 chess2vec-0.1.3a3/PKG-INFO
```

### Comparing `chess2vec-0.1.3a2/chess2vec/__init__.py` & `chess2vec-0.1.3a3/chess2vec/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,20 +31,21 @@
                     move.to_square ^= 0x38
 
                 idx = 64 * move.from_square + move.to_square
 
                 match pt:
                     case chess.QUEEN:
                         columns += [VEC_BLOCK * 2 + idx, VEC_BLOCK * 3 + idx]
+                        rows += [row_idx, row_idx]
                     case chess.KING:
                         columns += [VEC_BLOCK * 4 + idx]
+                        rows.append(row_idx)
                     case _:
                         columns += [VEC_BLOCK * (pt - 1) + idx]
-
-                rows.append(row_idx)
+                        rows.append(row_idx)
 
             row_idx += 1
 
         mat = scipy.sparse.csr_matrix(
             (
                 np.ones_like(columns, dtype=np.uint8),
                 (rows, columns),
```

### Comparing `chess2vec-0.1.3a2/chess2vec/_utils/sparse.py` & `chess2vec-0.1.3a3/chess2vec/_utils/sparse.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.3a2/chess2vec/_utils/vector.py` & `chess2vec-0.1.3a3/chess2vec/_utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.3a2/PKG-INFO` & `chess2vec-0.1.3a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.1.3a2
+Version: 0.1.3a3
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

