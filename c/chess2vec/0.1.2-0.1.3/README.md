# Comparing `tmp/chess2vec-0.1.2.tar.gz` & `tmp/chess2vec-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.1.2.tar", max compression
+gzip compressed data, was "chess2vec-0.1.3.tar", max compression
```

## Comparing `chess2vec-0.1.2.tar` & `chess2vec-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.2/README.md
--rw-r--r--   0        0        0     4046 2024-04-16 19:55:55.091015 chess2vec-0.1.2/chess2vec/__init__.py
--rw-r--r--   0        0        0      740 2024-04-16 16:21:07.852284 chess2vec-0.1.2/chess2vec/_utils/sparse.py
--rw-r--r--   0        0        0      538 2024-04-16 16:46:49.087490 chess2vec-0.1.2/chess2vec/_utils/vector.py
--rw-r--r--   0        0        0      339 2024-04-16 19:28:46.276872 chess2vec-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 chess2vec-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.3/README.md
+-rw-r--r--   0        0        0     4048 2024-04-16 19:59:01.690957 chess2vec-0.1.3/chess2vec/__init__.py
+-rw-r--r--   0        0        0      740 2024-04-16 16:21:07.852284 chess2vec-0.1.3/chess2vec/_utils/sparse.py
+-rw-r--r--   0        0        0      538 2024-04-16 16:46:49.087490 chess2vec-0.1.3/chess2vec/_utils/vector.py
+-rw-r--r--   0        0        0      339 2024-04-16 19:59:26.094297 chess2vec-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 chess2vec-0.1.3/PKG-INFO
```

### Comparing `chess2vec-0.1.2/chess2vec/__init__.py` & `chess2vec-0.1.3/chess2vec/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         for file in x:
             with open(file) as pgn:
                 game = chess.pgn.read_game(pgn)
 
                 while game:
                     board = game.board()
                     pos = [board.fen()] + [
-                        board.push(move) or board.fen() for move in board.legal_moves
+                        board.push(move) or board.fen() for move in game.mainline_moves
                     ]
                     self.load_fen(pos)
 
     def load_npz(self, x: Iterable[str]):
         for file in x:
             with np.load(file) as loaded:
                 indices = loaded["mat_indices"]
```

### Comparing `chess2vec-0.1.2/chess2vec/_utils/sparse.py` & `chess2vec-0.1.3/chess2vec/_utils/sparse.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.2/chess2vec/_utils/vector.py` & `chess2vec-0.1.3/chess2vec/_utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.2/PKG-INFO` & `chess2vec-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

