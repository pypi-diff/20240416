# Comparing `tmp/chess2vec-0.1.3a5.tar.gz` & `tmp/chess2vec-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.1.3a5.tar", max compression
+gzip compressed data, was "chess2vec-0.1.4.tar", max compression
```

## Comparing `chess2vec-0.1.3a5.tar` & `chess2vec-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.3a5/README.md
--rw-r--r--   0        0        0     4229 2024-04-16 20:16:30.752606 chess2vec-0.1.3a5/chess2vec/__init__.py
--rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.3a5/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
--rw-r--r--   0        0        0      740 2024-04-16 16:21:07.852284 chess2vec-0.1.3a5/chess2vec/_utils/sparse.py
--rw-r--r--   0        0        0      538 2024-04-16 16:46:49.087490 chess2vec-0.1.3a5/chess2vec/_utils/vector.py
--rw-r--r--   0        0        0      341 2024-04-16 20:16:38.462623 chess2vec-0.1.3a5/pyproject.toml
--rw-r--r--   0        0        0      525 1970-01-01 00:00:00.000000 chess2vec-0.1.3a5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.4/README.md
+-rw-r--r--   0        0        0     4375 2024-04-16 20:22:07.803404 chess2vec-0.1.4/chess2vec/__init__.py
+-rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.4/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
+-rw-r--r--   0        0        0      740 2024-04-16 16:21:07.852284 chess2vec-0.1.4/chess2vec/_utils/sparse.py
+-rw-r--r--   0        0        0      538 2024-04-16 16:46:49.087490 chess2vec-0.1.4/chess2vec/_utils/vector.py
+-rw-r--r--   0        0        0      365 2024-04-16 20:21:08.129926 chess2vec-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 chess2vec-0.1.4/PKG-INFO
```

### Comparing `chess2vec-0.1.3a5/chess2vec/__init__.py` & `chess2vec-0.1.4/chess2vec/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import chess
 import chess.pgn
 import numpy as np
 import scipy.sparse
 
 import chess2vec._utils.sparse as spu
 
+from alive_progress import alive_bar
+
 VEC_BLOCK = 64 * 64
 VEC_SIZE = 5 * VEC_BLOCK
 
 
 class PositionEncoder:
     def __init__(self) -> None:
         self.positions = []
@@ -53,25 +55,27 @@
             shape=(row_idx, VEC_SIZE),
         )
 
         self._actions_matrix = scipy.sparse.vstack([self._actions_matrix, mat])
         self.positions += list(x)
 
     def load_pgn(self, x: Iterable[str]):
-        for file in x:
-            with open(file) as pgn:
-                game = chess.pgn.read_game(pgn)
-
-                while game:
-                    board = game.board()
-                    pos = [board.fen()] + [
-                        board.push(move) or board.fen()
-                        for move in game.mainline_moves()
-                    ]
-                    self.load_fen(pos)
+        with alive_bar() as bar:
+            for file in x:
+                with open(file) as pgn:
+                    game = chess.pgn.read_game(pgn)
+                    bar()
+
+                    while game:
+                        board = game.board()
+                        pos = [board.fen()] + [
+                            board.push(move) or board.fen() or bar()
+                            for move in game.mainline_moves()
+                        ]
+                        self.load_fen(pos)
 
     def load_npz(self, x: Iterable[str]):
         for file in x:
             with np.load(file) as loaded:
                 indices = loaded["mat_indices"]
                 mat = scipy.sparse.csr_matrix(
                     (
```

### Comparing `chess2vec-0.1.3a5/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc` & `chess2vec-0.1.4/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.3a5/chess2vec/_utils/sparse.py` & `chess2vec-0.1.4/chess2vec/_utils/sparse.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.3a5/chess2vec/_utils/vector.py` & `chess2vec-0.1.4/chess2vec/_utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.3a5/PKG-INFO` & `chess2vec-0.1.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.1.3a5
+Version: 0.1.4
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: alive-progress (>=3.1.5,<4.0.0)
 Requires-Dist: chess (>=1.10.0,<2.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: scipy (>=1.13.0,<2.0.0)
 Description-Content-Type: text/markdown
```

