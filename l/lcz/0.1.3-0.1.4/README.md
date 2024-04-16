# Comparing `tmp/lcz-0.1.3-py3-none-any.whl.zip` & `tmp/lcz-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 1266812 bytes, number of entries: 11
+Zip file size: 1266331 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      121 b- defN 24-Jan-24 08:08 lcz/__init__.py
 -rw-r--r--  2.0 unx      385 b- defN 24-Jan-24 07:57 lcz/backends.py
--rw-r--r--  2.0 unx      998 b- defN 24-Jan-24 08:06 lcz/main.py
+-rw-r--r--  2.0 unx     1012 b- defN 24-Apr-16 07:33 lcz/main.py
 -rw-r--r--  2.0 unx      472 b- defN 24-Jan-24 07:57 lcz/uci.py
 -rw-r--r--  2.0 unx       30 b- defN 24-Jan-24 08:06 lcz/weights/__init__.py
 -rwxr-xr-x  2.0 unx  1262607 b- defN 24-Jan-24 07:54 lcz/weights/maia-1900.pb.gz
 -rw-r--r--  2.0 unx      144 b- defN 24-Jan-24 08:06 lcz/weights/weights.py
--rw-r--r--  2.0 unx     1225 b- defN 24-Jan-24 08:48 lcz-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-24 08:48 lcz-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 24-Jan-24 08:48 lcz-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      799 b- defN 24-Jan-24 08:48 lcz-0.1.3.dist-info/RECORD
-11 files, 1266877 bytes uncompressed, 1265484 bytes compressed:  0.1%
+-rw-r--r--  2.0 unx      431 b- defN 24-Apr-16 07:34 lcz-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 07:34 lcz-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-16 07:34 lcz-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      799 b- defN 24-Apr-16 07:34 lcz-0.1.4.dist-info/RECORD
+11 files, 1266097 bytes uncompressed, 1265003 bytes compressed:  0.1%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: lcz/weights/maia-1900.pb.gz
 Comment: 
 
 Filename: lcz/weights/weights.py
 Comment: 
 
-Filename: lcz-0.1.3.dist-info/METADATA
+Filename: lcz-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: lcz-0.1.3.dist-info/WHEEL
+Filename: lcz-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: lcz-0.1.3.dist-info/top_level.txt
+Filename: lcz-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: lcz-0.1.3.dist-info/RECORD
+Filename: lcz-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lcz/main.py

```diff
@@ -1,22 +1,22 @@
-from typing import Annotated
+from typing import Annotated, Iterable
 import lczero.backends as lcz
 from .uci import Uci, lcz2uci
 from .backends import Backend, cached_backend
 from .weights import MAIA_PATH
 
 Prob = Annotated[float, 'probability']
 
 def preds(game: lcz.GameState, y: lcz.Output) -> dict[Uci, Prob]:
     return {
         lcz2uci(pred): prob
         for pred, prob in zip(game.moves(), y.p_softmax(*game.policy_indices()))
     }
 
-def eval(fens: list[str], weights_path: str = MAIA_PATH, backend: Backend = 'eigen') -> list[dict[Uci, Prob]]:
+def eval(fens: Iterable[str], weights_path: str = MAIA_PATH, backend: Backend = 'eigen') -> list[dict[Uci, Prob]]:
     """Given a batch of positions `fens`, returns a batch of dictionaries of uci moves to probabilities
     - e.g. `result[0] = { "g1f3": 0.4, "e2e4" : 0.5, ... }` (per each `fen` in `fens`)
     """
     bk = cached_backend(weights_path, backend=backend)
     games: list[lcz.GameState] = [lcz.GameState(fen) for fen in fens]
     X: list[lcz.Input] = [game.as_input(bk) for game in games]
     Y: list[lcz.Output] = bk.evaluate(*X)
```

## Comparing `lcz-0.1.3.dist-info/RECORD` & `lcz-0.1.4.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 lcz/__init__.py,sha256=RllJs2nSX6LFq94ZlGg7z5NpMzGznDyfN7ssTpgQQm4,121
 lcz/backends.py,sha256=ALCI6q1cV3QTjkC3SstfClMvARbD12r88fNF5lUAWok,385
-lcz/main.py,sha256=SSuzTU6bak9lWPaPlQ4sAI_uOxKHger9rHJ4GbmT4k8,998
+lcz/main.py,sha256=qji5sOCaEWlUElDPtdFPonmAGQFRFDFEHzjOgh7iEVY,1012
 lcz/uci.py,sha256=gi8p5BiT92zQu340aSP7z_-s-fnliYJ-F2Mf3OpIo3M,472
 lcz/weights/__init__.py,sha256=4vhXmpzM-GfkBflL9D-_ovvHq2UYNE5UhobxDSv1LLs,30
 lcz/weights/maia-1900.pb.gz,sha256=4vVl9C182fEiVX5txOuE5buu3O2h1ATcSF02EcfJehI,1262607
 lcz/weights/weights.py,sha256=5J2gitcveUxj6zNgkITKUBqU_ZBDqGsjY9fBCMz9DEU,144
-lcz-0.1.3.dist-info/METADATA,sha256=v1AoAAn9PtI22lqGFfsumjSv8nIIX1F3R0fXHQla2iw,1225
-lcz-0.1.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-lcz-0.1.3.dist-info/top_level.txt,sha256=a1s_B0d8bLvolHr9k0orkRper8CFy7K7wnTnEoLVixI,4
-lcz-0.1.3.dist-info/RECORD,,
+lcz-0.1.4.dist-info/METADATA,sha256=YSIM43r-qgkGeIUzs8bj5UDFxl_XKH6Jr71oyloVKic,431
+lcz-0.1.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+lcz-0.1.4.dist-info/top_level.txt,sha256=a1s_B0d8bLvolHr9k0orkRper8CFy7K7wnTnEoLVixI,4
+lcz-0.1.4.dist-info/RECORD,,
```

