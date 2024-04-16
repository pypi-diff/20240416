# Comparing `tmp/game-prediction2-0.1.6.tar.gz` & `tmp/game_prediction2-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "game-prediction2-0.1.6.tar", last modified: Sun Mar 31 13:35:50 2024, max compression
+gzip compressed data, was "game_prediction2-0.1.7.tar", last modified: Tue Apr 16 07:42:24 2024, max compression
```

## Comparing `game-prediction2-0.1.6.tar` & `game_prediction2-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-31 13:35:50.904186 game-prediction2-0.1.6/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-03-31 13:35:50.904186 game-prediction2-0.1.6/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-03-31 13:35:47.000000 game-prediction2-0.1.6/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-03-31 13:35:50.904186 game-prediction2-0.1.6/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-31 13:35:50.904186 game-prediction2-0.1.6/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-31 13:35:50.904186 game-prediction2-0.1.6/src/game_prediction2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       25 2024-03-16 14:22:46.000000 game-prediction2-0.1.6/src/game_prediction2/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-31 13:35:50.904186 game-prediction2-0.1.6/src/game_prediction2/beam/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      182 2024-03-21 06:01:10.000000 game-prediction2-0.1.6/src/game_prediction2/beam/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1901 2024-03-22 15:59:04.000000 game-prediction2-0.1.6/src/game_prediction2/beam/decoding.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1071 2024-03-21 06:01:14.000000 game-prediction2-0.1.6/src/game_prediction2/beam/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2033 2024-03-21 05:38:54.000000 game-prediction2-0.1.6/src/game_prediction2/beam/searching.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1643 2024-03-16 09:45:06.000000 game-prediction2-0.1.6/src/game_prediction2/beam/succs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      881 2024-03-21 06:01:45.000000 game-prediction2-0.1.6/src/game_prediction2/main.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-31 13:35:50.904186 game-prediction2-0.1.6/src/game_prediction2/util/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-03-16 09:09:26.000000 game-prediction2-0.1.6/src/game_prediction2/util/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-31 13:35:50.904186 game-prediction2-0.1.6/src/game_prediction2/util/aggregate/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       57 2024-03-15 19:06:22.000000 game-prediction2-0.1.6/src/game_prediction2/util/aggregate/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      737 2024-03-15 19:06:22.000000 game-prediction2-0.1.6/src/game_prediction2/util/aggregate/aggregate.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-31 13:35:50.904186 game-prediction2-0.1.6/src/game_prediction2/util/logprobs/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      120 2024-03-16 14:37:30.000000 game-prediction2-0.1.6/src/game_prediction2/util/logprobs/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2797 2024-03-31 13:35:28.000000 game-prediction2-0.1.6/src/game_prediction2/util/logprobs/logprobs.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-31 13:35:50.904186 game-prediction2-0.1.6/src/game_prediction2/util/predict/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       69 2024-03-16 14:37:48.000000 game-prediction2-0.1.6/src/game_prediction2/util/predict/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1187 2024-03-21 05:58:53.000000 game-prediction2-0.1.6/src/game_prediction2/util/predict/predict.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-31 13:35:50.904186 game-prediction2-0.1.6/src/game_prediction2.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-03-31 13:35:50.000000 game-prediction2-0.1.6/src/game_prediction2.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      799 2024-03-31 13:35:50.000000 game-prediction2-0.1.6/src/game_prediction2.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-03-31 13:35:50.000000 game-prediction2-0.1.6/src/game_prediction2.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       73 2024-03-31 13:35:50.000000 game-prediction2-0.1.6/src/game_prediction2.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       17 2024-03-31 13:35:50.000000 game-prediction2-0.1.6/src/game_prediction2.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 07:42:24.404857 game_prediction2-0.1.7/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-04-16 07:42:24.404857 game_prediction2-0.1.7/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-04-16 07:42:22.000000 game_prediction2-0.1.7/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-16 07:42:24.404857 game_prediction2-0.1.7/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 07:42:24.394862 game_prediction2-0.1.7/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 07:42:24.394862 game_prediction2-0.1.7/src/game_prediction2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       63 2024-04-16 07:38:55.000000 game_prediction2-0.1.7/src/game_prediction2/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 07:42:24.404857 game_prediction2-0.1.7/src/game_prediction2/beam/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      184 2024-04-16 07:36:22.000000 game_prediction2-0.1.7/src/game_prediction2/beam/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1933 2024-04-16 07:38:02.000000 game_prediction2-0.1.7/src/game_prediction2/beam/decoding.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1125 2024-04-16 07:37:30.000000 game_prediction2-0.1.7/src/game_prediction2/beam/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2061 2024-04-16 07:37:29.000000 game_prediction2-0.1.7/src/game_prediction2/beam/searching.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1686 2024-04-16 07:24:24.000000 game_prediction2-0.1.7/src/game_prediction2/beam/succs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      976 2024-04-16 07:35:57.000000 game_prediction2-0.1.7/src/game_prediction2/main.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 07:42:24.404857 game_prediction2-0.1.7/src/game_prediction2/util/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-03-16 09:09:26.000000 game_prediction2-0.1.7/src/game_prediction2/util/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 07:42:24.404857 game_prediction2-0.1.7/src/game_prediction2/util/aggregate/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       57 2024-03-15 19:06:22.000000 game_prediction2-0.1.7/src/game_prediction2/util/aggregate/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      737 2024-03-15 19:06:22.000000 game_prediction2-0.1.7/src/game_prediction2/util/aggregate/aggregate.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 07:42:24.404857 game_prediction2-0.1.7/src/game_prediction2/util/logprobs/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      133 2024-04-16 07:19:37.000000 game_prediction2-0.1.7/src/game_prediction2/util/logprobs/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3409 2024-04-16 07:27:38.000000 game_prediction2-0.1.7/src/game_prediction2/util/logprobs/logprobs.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 07:42:24.404857 game_prediction2-0.1.7/src/game_prediction2/util/predict/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      100 2024-04-16 07:25:13.000000 game_prediction2-0.1.7/src/game_prediction2/util/predict/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1468 2024-04-16 07:27:05.000000 game_prediction2-0.1.7/src/game_prediction2/util/predict/predict.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 07:42:24.404857 game_prediction2-0.1.7/src/game_prediction2.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-04-16 07:42:24.000000 game_prediction2-0.1.7/src/game_prediction2.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      799 2024-04-16 07:42:24.000000 game_prediction2-0.1.7/src/game_prediction2.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-16 07:42:24.000000 game_prediction2-0.1.7/src/game_prediction2.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       73 2024-04-16 07:42:24.000000 game_prediction2-0.1.7/src/game_prediction2.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       17 2024-04-16 07:42:24.000000 game_prediction2-0.1.7/src/game_prediction2.egg-info/top_level.txt
```

### Comparing `game-prediction2-0.1.6/pyproject.toml` & `game_prediction2-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "game-prediction2"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
     {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Game prediction, simplified. No edits, no GCP. Everything's just `AsyncIterables` in and out."
 dependencies = [
     "haskellian",
     "lcz",
```

### Comparing `game-prediction2-0.1.6/src/game_prediction2/beam/decoding.py` & `game_prediction2-0.1.7/src/game_prediction2/beam/decoding.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import AsyncIterable
 import numpy as np
 import ramda as R
-import haskellian as hk
-from haskellian import asynch as hka
+from haskellian.core import pipe
+import haskellian.iterables as hk
+import haskellian.asyn.iter as AI
 from .succs import Node, Child
 
 @R.curry
 def reconstruct(node: Node, max_depth: int | None = None, with_probs: bool = True) -> list[tuple[str, float]] | list[str]:
   """Reconstruct backwards from `node` (keeping log-probs as they are)
   - `max_depth`: limit of backward steps
   """
@@ -26,25 +27,25 @@
   exps = np.exp(logps)
   return list(zip(preds, exps))
 
 def convergence(beam: list[Node], max_depth: int | None = None) -> int:
   """Convergence point: ply back to which all lines of the `beam` agree on the best move
   - `max_depth`: limit of backward steps (from the current beam's ply)
   """
-  return hk.vpipe(
-    hk.map(reconstruct(max_depth=max_depth, with_probs=False), beam), # line of every beam
+  return pipe(
+    map(reconstruct(max_depth=max_depth, with_probs=False), beam), # line of every beam
     hk.transpose, # moves at every ply
     hk.map(set), # aka uniq
     hk.take_while(lambda uniq_preds: len(uniq_preds) == 1),
     list, len
 )
   
 async def decode(beams: AsyncIterable[list[Node]]) -> AsyncIterable[list[tuple[str, float]]]:
   last_converged = 0
   beam = None
-  async for ply, beam in hka.enumerate(beams):
+  async for ply, beam in AI.enumerate(beams):
     converged = convergence(beam, max_depth=ply-last_converged)
     if converged > 0:
       yield exp(reconstruct(beam[0], max_depth=ply-last_converged)[:converged])
       last_converged += converged
   if beam is not None:
     yield exp(reconstruct(beam[0], max_depth=max(ply-last_converged, 0)))
```

### Comparing `game-prediction2-0.1.6/src/game_prediction2/beam/main.py` & `game_prediction2-0.1.7/src/game_prediction2/beam/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import AsyncIterable, Unpack
+import haskellian.asyn.iter as AI
 from .succs import Logprob
-from .searching import search, Params
+from .searching import search, SearchParams
 from .decoding import decode
 
-
-def predict(logprobs: AsyncIterable[Logprob], **params: Unpack[Params]):
+@AI.lift
+def predict(logprobs: AsyncIterable[Logprob], **params: Unpack[SearchParams]):
   """Beam decoding across the forest of moves stemming from `start_fens`
   - Yields predictions as the beams converge (i.e. agree on a single move) or the search stops (because no legal moves have high enough probability)
     - Thus, a bigger `beam_width` can increase accuracy but also prediction time by more than a constant factor
     
   Params:
   - `logprobs[ply](san, piece)`: (OCR) log-probability of `san` (which captures `piece`) at `ply`
   - `uci_prior(fens)`: batched prior distribution of legal moves (defaults to using `MaiaChess` with `Leela Chess Zero`)
```

### Comparing `game-prediction2-0.1.6/src/game_prediction2/beam/succs.py` & `game_prediction2-0.1.7/src/game_prediction2/beam/succs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Protocol, Iterable, TypedDict
+from typing import Protocol, Iterable, TypedDict, NotRequired
 from dataclasses import dataclass
 import numpy as np
 import chess
 from chess_utils import CapturablePiece, parse, unchecked_san, captured_piece, fen_after
 
 class Logprob(Protocol):
   def __call__(self, san: str, captured_piece: CapturablePiece | None) -> float:
@@ -32,17 +32,17 @@
   def __init__(self, fen: str, logp: float, san: str, parent: Node, sum_logp = None):
     self.fen = fen
     self.sum_logp = sum_logp or logp + parent.sum_logp
     self.logp = logp
     self.san = san
     self.parent = parent
     
-class Params(TypedDict):
-  logp_min: float
-  ocr_logp_min: float
+class SuccParams(TypedDict):
+  logp_min: NotRequired[float]
+  ocr_logp_min: NotRequired[float]
 
 def successors(
   node: Node, uci_priors: dict[str, float], lp: Logprob, agg_lp: AggregateLogps,
   logp_min: float = np.log(0.02), logp_ocr_min: float = np.log(0.02),
 ) -> Iterable[Child]:
   board = chess.Board(node.fen)
   for uci, p_prior in uci_priors.items():
```

### Comparing `game-prediction2-0.1.6/src/game_prediction2/util/aggregate/aggregate.py` & `game_prediction2-0.1.7/src/game_prediction2/util/aggregate/aggregate.py`

 * *Files identical despite different names*

### Comparing `game-prediction2-0.1.6/src/game_prediction2/util/logprobs/logprobs.py` & `game_prediction2-0.1.7/src/game_prediction2/util/logprobs/logprobs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from editdistance import distance as edit_dist
 import numpy as np
-from chess_notation.represent import representations
+from pydantic import BaseModel
+from chess_notation.represent import representations, MotionStyles
+from chess_notation.styles import PawnCapture, PieceCapture
 from chess_notation.language import Language
 from chess_utils import CapturablePiece
 from ...beam import Logprob
 
 def pseudo_logp(word: str, top_preds: list[tuple[str, float]]) -> float:
   """Approximates the log probability of `word` given a subset of the best outputs `top_preds` of a model.
   - `top_preds :: [(Pred, Logprob)]`: the top-k predictions of a model with probability distribution `P`
@@ -21,29 +23,46 @@
   return max(
     (np.log(1 - dist/len(word)) + logp
     for pred, logp in top_preds if (dist := edit_dist(pred, word)) < min(len(word), len(pred))),
     default=-float('inf')
   )
   
 
-def max_pseudo_logp(san: str, captured_piece: CapturablePiece | None, top_preds: list[tuple[str, float]], langs: list[Language]) -> float:
+class Annotations(BaseModel):
+  lang: Language | None = None
+  pawn_capture: PawnCapture | None = None
+  piece_capture: PieceCapture | None = None
+
+  def motions(self) -> MotionStyles:
+    styles = MotionStyles()
+    if self.pawn_capture: styles.pawn_captures = [self.pawn_capture]
+    if self.piece_capture: styles.piece_captures = [self.piece_capture]
+    return styles
+  
+  def langs(self) -> list[Language] | None:
+    if self.lang is not None:
+      return [self.lang]
+    
+def max_pseudo_logp(san: str, captured_piece: CapturablePiece | None, top_preds: list[tuple[str, float]], ann: Annotations) -> float:
   """Max `pseudo_logp` across all possible representations of `san`"""
-  reprs = representations(san, captured_piece=captured_piece, languages=langs)
+  reprs = representations(san, motions=ann.motions(), captured_piece=captured_piece, languages=ann.langs() or ['CA', 'EN'])
   return max(pseudo_logp(r, top_preds) for r in reprs)
 
-def players_max_pseudo_logp(san: str, captured_piece: CapturablePiece | None, players_preds: tuple[list[tuple[str, float]], ...], players_langs: tuple[list[Language], ...]) -> float:
+def players_max_pseudo_logp(san: str, captured_piece: CapturablePiece | None, players_preds: list[list[tuple[str, float]]], annotations: list[Annotations] | None = None) -> float:
   """Max `max_pseudo_logp` across players"""
-  assert len(players_preds) == len(players_langs), f'ERROR: Inconsistent number of players: {len(players_preds)} preds, but {len(players_langs)} languages'
+  annotations = annotations or [Annotations() for _ in players_preds]
+  assert len(players_preds) == len(annotations), f'ERROR: Inconsistent number of players: {len(players_preds)} preds, but {len(annotations)} annotations'
   return max(
-    max_pseudo_logp(san, captured_piece, preds, langs)
-    for preds, langs in zip(players_preds, players_langs)
+    max_pseudo_logp(san, captured_piece, preds, ann)
+    for preds, ann in zip(players_preds, annotations)
   )
-  
-def logprob(players_preds: list[list[tuple[str, float]]]) -> Logprob:
-  """Wrapper around `players_max_pseudo_logp`, with predefined languages (a future API will completely exclude them, as they'll be auto-detected)"""
+
+
+def logprob(players_preds: list[list[tuple[str, float]]], annotations: list[Annotations] | None = None) -> Logprob:
+  """Curried version of `players_max_pseudo_logp`"""
   def _logprob(san: str, captured_piece: CapturablePiece | None):
-    return players_max_pseudo_logp(san, captured_piece, players_preds, [['CA'] for _ in players_preds])
+    return players_max_pseudo_logp(san, captured_piece, players_preds, annotations)
   return _logprob
   
 def weighted_geo_mean(logp: float, logq: float, a: float, b: float):
   """Weighted geometrical mean (`[p^a * q^b]^(1/(a+b))`) but in log-space"""
   return (a*logp + b*logq) / (a+b)
```

### Comparing `game-prediction2-0.1.6/src/game_prediction2.egg-info/SOURCES.txt` & `game_prediction2-0.1.7/src/game_prediction2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

