# Comparing `tmp/alphacube-0.1.3-py3-none-any.whl.zip` & `tmp/alphacube-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,16 @@
-Zip file size: 21672 bytes, number of entries: 12
--rw-rw-rw-  2.0 unx     6240 b- defN 24-Mar-16 05:30 alphacube/__init__.py
--rw-rw-rw-  2.0 unx     4972 b- defN 24-Mar-12 04:04 alphacube/_validator.py
--rw-rw-rw-  2.0 unx    15077 b- defN 24-Mar-12 04:13 alphacube/env.py
--rw-rw-rw-  2.0 unx     5520 b- defN 24-Mar-12 04:04 alphacube/model.py
--rw-rw-rw-  2.0 unx    13694 b- defN 24-Mar-12 04:04 alphacube/search.py
--rw-rw-rw-  2.0 unx     3807 b- defN 24-Mar-12 04:04 alphacube/solver.py
--rw-rw-rw-  2.0 unx     1067 b- defN 24-Mar-16 06:32 alphacube-0.1.3.dist-info/LICENSE
--rw-rw-rw-  2.0 unx     8242 b- defN 24-Mar-16 06:32 alphacube-0.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 24-Mar-16 06:32 alphacube-0.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 unx       44 b- defN 24-Mar-16 06:32 alphacube-0.1.3.dist-info/entry_points.txt
--rw-rw-rw-  2.0 unx       10 b- defN 24-Mar-16 06:32 alphacube-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      953 b- defN 24-Mar-16 06:32 alphacube-0.1.3.dist-info/RECORD
-12 files, 59718 bytes uncompressed, 20084 bytes compressed:  66.4%
+Zip file size: 24779 bytes, number of entries: 14
+-rw-rw-rw-  2.0 unx     5805 b- defN 24-Apr-16 06:22 alphacube/__init__.py
+-rw-rw-rw-  2.0 unx     5473 b- defN 24-Apr-16 06:05 alphacube/_evaluator.py
+-rw-rw-rw-  2.0 unx     5040 b- defN 24-Apr-15 06:08 alphacube/_validator.py
+-rw-rw-rw-  2.0 unx     4074 b- defN 24-Apr-16 06:05 alphacube/core.py
+-rw-rw-rw-  2.0 unx    18301 b- defN 24-Apr-16 01:36 alphacube/env.py
+-rw-rw-rw-  2.0 unx     5920 b- defN 24-Apr-16 04:55 alphacube/model.py
+-rw-rw-rw-  2.0 unx    12498 b- defN 24-Apr-16 05:18 alphacube/search.py
+-rw-rw-rw-  2.0 unx     1330 b- defN 24-Apr-16 06:06 alphacube/utils.py
+-rw-rw-rw-  2.0 unx     1067 b- defN 24-Apr-16 06:24 alphacube-0.1.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 unx     8266 b- defN 24-Apr-16 06:24 alphacube-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 24-Apr-16 06:24 alphacube-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       44 b- defN 24-Apr-16 06:24 alphacube-0.1.4.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 unx       10 b- defN 24-Apr-16 06:24 alphacube-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1106 b- defN 24-Apr-16 06:24 alphacube-0.1.4.dist-info/RECORD
+14 files, 69026 bytes uncompressed, 22961 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -1,37 +1,43 @@
 Filename: alphacube/__init__.py
 Comment: 
 
+Filename: alphacube/_evaluator.py
+Comment: 
+
 Filename: alphacube/_validator.py
 Comment: 
 
+Filename: alphacube/core.py
+Comment: 
+
 Filename: alphacube/env.py
 Comment: 
 
 Filename: alphacube/model.py
 Comment: 
 
 Filename: alphacube/search.py
 Comment: 
 
-Filename: alphacube/solver.py
+Filename: alphacube/utils.py
 Comment: 
 
-Filename: alphacube-0.1.3.dist-info/LICENSE
+Filename: alphacube-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: alphacube-0.1.3.dist-info/METADATA
+Filename: alphacube-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: alphacube-0.1.3.dist-info/WHEEL
+Filename: alphacube-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: alphacube-0.1.3.dist-info/entry_points.txt
+Filename: alphacube-0.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: alphacube-0.1.3.dist-info/top_level.txt
+Filename: alphacube-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: alphacube-0.1.3.dist-info/RECORD
+Filename: alphacube-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## alphacube/__init__.py

```diff
@@ -8,79 +8,58 @@
 - ``solve(*args, **kwargs)``: Solve a Rubik's Cube using the loaded solver.
 - ``cli()``: Command-line utility for solving a Rubik's Cube using AlphaCube.
 - ``set_verbose(loglevel=logging.INFO)``: Set the verbosity level of the logger.
 
 Example::
 
     import alphacube
-    alphacube.load(model_id="base")
+    alphacube.load("base")
     solution = alphacube.solve(format='moves', scramble="R U R' U'", beam_width=1024)
 
 """
 
-import logging
-from rich.console import Console
-from rich.logging import RichHandler
+from .utils import logger, logargs, set_verbose, device, dtype
 
-logger = logging.getLogger("rich")
-logger.propagate = False
-logger.addHandler(RichHandler(console=Console(stderr=True)))
-logger.setLevel(logging.WARNING)
-logargs = dict(extra={"markup": True})
-
-
-# Set up logging level
-def set_verbose(loglevel=logging.INFO):
-    """
-    Set the verbosity level of the logger.
-
-    Args:
-        loglevel (int): Logging level (e.g., logging.INFO, logging.DEBUG) to control the verbosity.
-
-    Returns:
-        None
-    """
-    global logger
-    logger.setLevel(loglevel)
+from ._validator import Input
+from .core import Solver
 
 
-from ._validator import Input
-from .solver import Solver
+solver = _solver = Solver()
 
-_solver = Solver()
+__all__ = ["load", "solve", "cli", "solver", "logger", "logargs", "set_verbose", "device", "dtype"]
 
 
-def load(model_id="small", *args, **kwargs):
+def load(model_id="small" if device.type == "cpu" else "large", *args, **kwargs):
     """
     Load the Rubik's Cube solver model.
 
     Args:
         model_id (str): Identifier for the model variant to load ("small", "base", or "large"). Default to `small`.
         *args, **kwargs: Arguments to configure model loading.
 
     Returns:
         None
     """
-    _solver.load(model_id, *args, **kwargs)
+    solver.load(model_id, *args, **kwargs)
 
 
 def solve(*args, **kwargs):
     """
     Solve a Rubik's Cube puzzle using the loaded solver model.
 
     Args:
         *args, **kwargs: Arguments to configure puzzle solving; passed down to ``alphacube.solver.Solver.__call__()`` and ``alphacube.search.beam_search``.
 
     Returns:
         dict | None: A dictionary containing solutions and performance metrics. None if failed.
     """
-    if _solver.model is None:
-        raise ValueError("Model not loaded. Call `load` with appropriate arguments first.")
+    if not hasattr(solver, "model"):
+        raise ValueError("Model not loaded. Call `load`  first.")
 
-    return _solver(*args, **kwargs)
+    return solver(*args, **kwargs)
 
 
 def list_models():
     """
     List the available model IDs.
 
     Returns:
@@ -130,19 +109,21 @@
                     "F": [4, 3, 2, 4, 5, 1, 1, 4, 3], \\
                     "B": [1, 5, 5, 0, 4, 3, 3, 2, 2] \\
                 }' \\
                 --beam_width 64
 
     :return: None
     """
-    from rich import print
-
     import argparse
 
-    parser = argparse.ArgumentParser(description="AlphaCube -- State-of-the-Art Rubik's Cube Solver")
+    from rich import print as rprint
+
+    parser = argparse.ArgumentParser(
+        description="AlphaCube -- State-of-the-Art Rubik's Cube Solver"
+    )
     parser.add_argument(
         "--model_id",
         "-m",
         type=str,
         default="small",
         help="ID of the model to solve a given scramble with (`small`, `base`, or `large`)",
     )
@@ -174,15 +155,15 @@
         help="Number of additional depths to explore during the search",
     )
     parser.add_argument(
         "--verbose",
         "-v",
         dest="loglevel",
         action="store_const",
-        const=logging.INFO,
+        const=20,
         help="Enable verbose output for tracking progress",
     )
     args = parser.parse_args()
 
     if args.loglevel:
         set_verbose(args.loglevel)
 
@@ -198,19 +179,16 @@
         scramble=args.scramble,
         beam_width=args.beam_width,
         extra_depths=args.extra_depths,
         ergonomic_bias=None,
     )
 
     # Load only once validated
-    _solver.load(model_id)
+    solver.load(model_id)
     # Solve
-    solutions = _solver(
+    solutions = solver(
         format=args.format,
         scramble=args.scramble,
         beam_width=args.beam_width,
         extra_depths=args.extra_depths,
     )
-    print(solutions)
-
-
-__all__ = ["load", "solve", "cli"]
+    rprint(solutions)
```

## alphacube/_validator.py

```diff
@@ -126,17 +126,21 @@
         format = values["format"]
         scramble = values["scramble"]
 
         if format == "moves":
             if isinstance(scramble, str):
                 scramble = scramble.split()
             scramble = [m.replace("2'", "2") for m in scramble]
-            invalid_moves = [m for m in scramble if not re.match(r"^[UDLRFBudlrfb'2]{1,2}$", m)]  # no wide moves -- yet
+            invalid_moves = [
+                m for m in scramble if not re.match(r"^[UDLRFBudlrfb'2]{1,2}$", m)
+            ]  # no wide moves -- yet
             if invalid_moves:
-                raise ValueError(f"Invalid move{'s' if len(invalid_moves) > 1 else ''} in `scramble`: {invalid_moves}")
+                raise ValueError(
+                    f"Invalid move{'s' if len(invalid_moves) > 1 else ''} in `scramble`: {invalid_moves}"
+                )
         elif format == "stickers":
             if isinstance(scramble, str):
                 scramble = json.loads(scramble.replace("\\\n", ""))
             if isinstance(scramble, dict):
                 sticker_colors = [scramble[face] for face in "UDLRBF"]
                 # Reset axes if centers are modified
                 center_indices = [stickers[4] for stickers in sticker_colors]
```

## alphacube/env.py

```diff
@@ -8,15 +8,15 @@
 """
 
 import os
 import random
 
 import numpy as np
 import torch
-from rich import print
+from rich import print as rprint
 
 
 class Cube3:
     """
     A class for 3x3x3 Rubik's Cube in Half-Turn Metric (HTM).
 
     This class provides methods to manipulate and solve a 3x3x3 Rubik's Cube using the half-turn metric.
@@ -102,61 +102,60 @@
         self.CENTER_INDICES = [4, 13, 22, 31, 40, 49]
         self.CENTERS_HAT = np.arange(0, 6, dtype=np.int64)
 
         """ For potential training with `__iter__` """
         self.max_depth = max_depth
         self.moves_ix = [self.moves.index(f + n) for f in faces for n in degrees]
 
-    def show(
-        self, flat=False, palette=["white", "yellow", "orange1", "red", "blue", "green"]
-    ):
+    def show(self, flat=False, palette=["white", "yellow", "orange1", "red", "blue", "green"]):
         """
         Display the cube's current state.
 
         Args:
             flat (bool): Whether to display the state in flat form.
             palette (list): List of colors for representing stickers.
         """
         palette = ["white", "black", "blue", "red", "pink1", "green"]
         state_by_face = self.state.reshape(6, 9)
         if not flat:
-            state_by_face = state_by_face[:, [2, 5, 8, 1, 4, 7, 0, 3, 6]].reshape(
-                6, 3, 3
-            )
+            state_by_face = state_by_face[:, [2, 5, 8, 1, 4, 7, 0, 3, 6]].reshape(6, 3, 3)
         state_by_face = str(state_by_face)
         for i, color in zip(range(6), palette):
             state_by_face = state_by_face.replace(str(i), f"[{color}]{i}[/{color}]")
-        print(state_by_face)
-        print()
+        rprint(state_by_face)
+        rprint()
 
-    def validate(self, centered=True):
+    def validate(self, state=None, centered=True):
         """
         Validate the cube's state and arrangement.
 
         Args:
             centered (bool): Whether centers should be centered or not.
 
         Raises:
             ValueError: If the cube's state or arrangement is invalid.
         """
+        if state is not None:
+            self.state[:] = state
+
         centers = self.state[self.CENTER_INDICES]
 
         if centered and not np.all(centers == self.CENTERS_HAT):
             # Must be [0, 1, 2, 3, 4, 5]
             raise ValueError("State is not *centered*.")
         if not centered and np.all(centers == self.CENTERS_HAT):
             # Must NOT be [0, 1, 2, 3, 4, 5]
             raise ValueError("State is unintendedly *centered*.")
 
         if not np.all(np.sort(centers) == self.CENTERS_HAT):
             # Must be [0, 1, 2, 3, 4, 5] when sorted
             self.show(flat=True)
             raise ValueError("Centers are not in the right order.")
         elif not np.all(np.sort(self.state) == self.GOAL):
-            print(np.sort(self.state).reshape(6, 9), "!= env.goal")
+            rprint(np.sort(self.state).reshape(6, 9), "!= env.goal")
             raise ValueError("Inconsistent number of colors.")
 
     def reset(self):
         """Resets the cube state to the solved state."""
         self.state = np.arange(0, 6 * 9, dtype=np.int64) // 9
 
     def reset_axes(self):
@@ -189,17 +188,15 @@
         """
         Apply a single move using move index for faster execution.
 
         Args:
             ix (int): Index of the move.
         """
         if ix < 18:
-            self.state[self.sticker_target_ix[ix]] = self.state[
-                self.sticker_source_ix[ix]
-            ]
+            self.state[self.sticker_target_ix[ix]] = self.state[self.sticker_source_ix[ix]]
         else:
             self.state[self.sticker_target_ix_wide[ix % 18]] = self.state[
                 self.sticker_source_ix_wide[ix % 18]
             ]
 
     def apply_scramble(self, scramble):
         """
@@ -225,17 +222,15 @@
                 if seq:
                     while True:
                         ix = random.choice(self.moves_ix)
                         # Skip subsequent moves on a same face
                         if ix // 3 == seq[-1] // 3:
                             continue
                         # Skip two moves on a same face with an opposite move in between
-                        if _ > 1 and (
-                            ix // 3 == seq[-2] // 3 and ix // 6 == seq[-1] // 6
-                        ):
+                        if _ > 1 and (ix // 3 == seq[-2] // 3 and ix // 6 == seq[-1] // 6):
                             continue
                         break
                 else:
                     ix = random.choice(self.moves_ix)
                 self.finger_ix(ix)
                 seq.append(ix)
                 # yield self.state, ix
@@ -249,38 +244,216 @@
         This method defines ``self.sticker_target`` and ``self.sticker_source`` to manage sticker colors (target is replaced by source).
         They define indices of target and source stickers so that the moves can be vectorized.
         """
         self.sticker_target, self.sticker_source = dict(), dict()
 
         self.sticker_replacement = {
             # Sticker A is replaced by another sticker at index B -> {A: B}
-            'U':{0: 6, 1: 3, 2: 0, 3: 7, 5: 1, 6: 8, 7: 5, 8: 2, 20: 47, 23: 50, 26: 53, 29: 38, 32: 41, 35: 44, 38: 20, 41: 23, 44: 26, 47: 29, 50: 32, 53: 35},
-            'D':{9: 15, 10: 12, 11: 9, 12: 16, 14: 10, 15: 17, 16: 14, 17: 11, 18: 36, 21: 39, 24: 42, 27: 45, 30: 48, 33: 51, 36: 27, 39: 30, 42: 33, 45: 18, 48: 21, 51: 24},
-            'L':{0: 44, 1: 43, 2: 42, 9: 45, 10: 46, 11: 47, 18: 24, 19: 21, 20: 18, 21: 25, 23: 19, 24: 26, 25: 23, 26: 20, 42: 11, 43: 10, 44: 9, 45: 0, 46: 1, 47: 2},
-            'R':{6: 51, 7: 52, 8: 53, 15: 38, 16: 37, 17: 36, 27: 33, 28: 30, 29: 27, 30: 34, 32: 28, 33: 35, 34: 32, 35: 29, 36: 8, 37: 7, 38: 6, 51: 15, 52: 16, 53: 17},
-            'B':{2: 35, 5: 34, 8: 33, 9: 20, 12: 19, 15: 18, 18: 2, 19: 5, 20: 8, 33: 9, 34: 12, 35: 15, 36: 42, 37: 39, 38: 36, 39: 43, 41: 37, 42: 44, 43: 41, 44: 38},
-            'F':{0: 24, 3: 25, 6: 26, 11: 27, 14: 28, 17: 29, 24: 17, 25: 14, 26: 11, 27: 6, 28: 3, 29: 0, 45: 51, 46: 48, 47: 45, 48: 52, 50: 46, 51: 53, 52: 50, 53: 47}
+            "U": {
+                0: 6,
+                1: 3,
+                2: 0,
+                3: 7,
+                5: 1,
+                6: 8,
+                7: 5,
+                8: 2,
+                20: 47,
+                23: 50,
+                26: 53,
+                29: 38,
+                32: 41,
+                35: 44,
+                38: 20,
+                41: 23,
+                44: 26,
+                47: 29,
+                50: 32,
+                53: 35,
+            },
+            "D": {
+                9: 15,
+                10: 12,
+                11: 9,
+                12: 16,
+                14: 10,
+                15: 17,
+                16: 14,
+                17: 11,
+                18: 36,
+                21: 39,
+                24: 42,
+                27: 45,
+                30: 48,
+                33: 51,
+                36: 27,
+                39: 30,
+                42: 33,
+                45: 18,
+                48: 21,
+                51: 24,
+            },
+            "L": {
+                0: 44,
+                1: 43,
+                2: 42,
+                9: 45,
+                10: 46,
+                11: 47,
+                18: 24,
+                19: 21,
+                20: 18,
+                21: 25,
+                23: 19,
+                24: 26,
+                25: 23,
+                26: 20,
+                42: 11,
+                43: 10,
+                44: 9,
+                45: 0,
+                46: 1,
+                47: 2,
+            },
+            "R": {
+                6: 51,
+                7: 52,
+                8: 53,
+                15: 38,
+                16: 37,
+                17: 36,
+                27: 33,
+                28: 30,
+                29: 27,
+                30: 34,
+                32: 28,
+                33: 35,
+                34: 32,
+                35: 29,
+                36: 8,
+                37: 7,
+                38: 6,
+                51: 15,
+                52: 16,
+                53: 17,
+            },
+            "B": {
+                2: 35,
+                5: 34,
+                8: 33,
+                9: 20,
+                12: 19,
+                15: 18,
+                18: 2,
+                19: 5,
+                20: 8,
+                33: 9,
+                34: 12,
+                35: 15,
+                36: 42,
+                37: 39,
+                38: 36,
+                39: 43,
+                41: 37,
+                42: 44,
+                43: 41,
+                44: 38,
+            },
+            "F": {
+                0: 24,
+                3: 25,
+                6: 26,
+                11: 27,
+                14: 28,
+                17: 29,
+                24: 17,
+                25: 14,
+                26: 11,
+                27: 6,
+                28: 3,
+                29: 0,
+                45: 51,
+                46: 48,
+                47: 45,
+                48: 52,
+                50: 46,
+                51: 53,
+                52: 50,
+                53: 47,
+            },
         }
         if self.allow_wide:
             # Slice moves
-            self.sticker_replacement.update({
-                # Definition: https://jperm.net/3x3/moves
-                "M": {49: 4, 4: 40, 40: 13, 13: 49, 50: 5, 5: 39, 39: 14, 14: 50, 48: 3, 3: 41, 41: 12, 12: 48},
-                "S": {31: 4, 4: 22, 22: 13, 13: 31, 32: 1, 1: 21, 21: 16, 16: 32, 30: 7, 7: 23, 23: 10, 10: 30},
-                "E": {49: 22, 22: 40, 40: 31, 31:49, 46: 19, 19:37, 37: 28, 28: 46, 52: 25, 25: 43, 43: 34, 34: 52},
-            })
+            self.sticker_replacement.update(
+                {
+                    # Definition: https://jperm.net/3x3/moves
+                    "M": {
+                        49: 4,
+                        4: 40,
+                        40: 13,
+                        13: 49,
+                        50: 5,
+                        5: 39,
+                        39: 14,
+                        14: 50,
+                        48: 3,
+                        3: 41,
+                        41: 12,
+                        12: 48,
+                    },
+                    "S": {
+                        31: 4,
+                        4: 22,
+                        22: 13,
+                        13: 31,
+                        32: 1,
+                        1: 21,
+                        21: 16,
+                        16: 32,
+                        30: 7,
+                        7: 23,
+                        23: 10,
+                        10: 30,
+                    },
+                    "E": {
+                        49: 22,
+                        22: 40,
+                        40: 31,
+                        31: 49,
+                        46: 19,
+                        19: 37,
+                        37: 28,
+                        28: 46,
+                        52: 25,
+                        25: 43,
+                        43: 34,
+                        34: 52,
+                    },
+                }
+            )
             # Wide moves
-            self.sticker_replacement.update({
-                "u": {**self.sticker_replacement['U'], **{v:k for k,v in self.sticker_replacement['E'].items()}},
-                "d": {**self.sticker_replacement['D'], **self.sticker_replacement['E']},
-                "l": {**self.sticker_replacement['L'], **self.sticker_replacement['M']},
-                "r": {**self.sticker_replacement['R'], **{v:k for k,v in self.sticker_replacement['M'].items()}},
-                "b": {**self.sticker_replacement['B'], **{v:k for k,v in self.sticker_replacement['S'].items()}},
-                "f": {**self.sticker_replacement['F'], **self.sticker_replacement['S']},
-            })
+            self.sticker_replacement.update(
+                {
+                    "u": {
+                        **self.sticker_replacement["U"],
+                        **{v: k for k, v in self.sticker_replacement["E"].items()},
+                    },
+                    "d": {**self.sticker_replacement["D"], **self.sticker_replacement["E"]},
+                    "l": {**self.sticker_replacement["L"], **self.sticker_replacement["M"]},
+                    "r": {
+                        **self.sticker_replacement["R"],
+                        **{v: k for k, v in self.sticker_replacement["M"].items()},
+                    },
+                    "b": {
+                        **self.sticker_replacement["B"],
+                        **{v: k for k, v in self.sticker_replacement["S"].items()},
+                    },
+                    "f": {**self.sticker_replacement["F"], **self.sticker_replacement["S"]},
+                }
+            )
 
         for m in self.moves:
             if len(m) == 1:
                 assert m in self.sticker_replacement
             else:
                 if "'" in m:
                     self.sticker_replacement[m] = {
@@ -328,39 +501,40 @@
     >>> for i, (batch_x, batch_y) in zip(range(1000), dl):
     >>>     batch_x, batch_y = batch_x.to(device), batch_y.device().reshape(-1)
     """
 
     def __init__(self, max_depth=20, num_workers=os.cpu_count()):
         self.num_workers = num_workers
         self.generators = [
-            iter(Cube3(allow_wide=False, max_depth=max_depth))
-            for _ in range(num_workers)
+            iter(Cube3(allow_wide=False, max_depth=max_depth)) for _ in range(num_workers)
         ]
 
     def __len__(self):
         return 0x7FFFFFFF  # max int possible with a single precision
 
     def __getitem__(self, i):
         return next(self.generators[i % self.num_workers])
 
 
 def get_dataloader(
-        batch_size,
-        num_workers=min(os.cpu_count(), 32),  # DataLoader slightly slows down beyond 32 CPU cores
-        max_depth=20,
-        **dl_kwargs
-    ):
+    batch_size,
+    num_workers=min(os.cpu_count(), 32),  # DataLoader slightly slows down beyond 32 CPU cores
+    max_depth=20,
+    **dl_kwargs,
+):
     """
     Create a DataLoader instance for generating random Rubik's Cube scrambles.
 
     Args:
         batch_size (int): The number of samples per batch.
         num_workers (int, optional): The number of worker processes to use for data loading.
             Defaults to the number of CPU cores or 32 (beyond which the return will diminish), whichever is smaller.
         max_depth (int, optional): The maximum depth of the scrambles. Defaults to 20.
         **dl_kwargs: Additional keyword arguments to pass to the DataLoader constructor.
 
     Returns:
         torch.utils.data.DataLoader: A DataLoader instance that yields batches of random scrambles.
     """
     ds = Dataset(max_depth=max_depth, num_workers=num_workers)
-    return torch.utils.data.DataLoader(ds, num_workers=num_workers, batch_size=batch_size, **dl_kwargs)
+    return torch.utils.data.DataLoader(
+        ds, num_workers=num_workers, batch_size=batch_size, **dl_kwargs
+    )
```

## alphacube/model.py

```diff
@@ -41,30 +41,32 @@
 
         os.makedirs(cache_dir, exist_ok=True)
         model_url = os.path.join("https://storage.googleapis.com/alphacube/", model_id + ".zip")
         logger.info(f"[grey50]Downloading AlphaCube ({model_id}) from {model_url}", **logargs)
         with requests.get(model_url, stream=True) as r:
             total_size = int(r.headers.get("Content-Length"))
             with Progress() as progress:
-                task = progress.add_task("[cyan]Downloading ...", total=total_size)
+                task = progress.add_task(
+                    f"[cyan]Downloading [bold]`{model_id}`[/bold]", total=total_size
+                )
                 with open(model_path, "wb") as output:
                     for chunk in r.iter_content(chunk_size=8192):
                         output.write(chunk)
-                        progress.update(task, completed=len(chunk))
+                        progress.update(task, advance=len(chunk))
         logger.info(f"[grey50]Saved to {model_path}", **logargs)
-        try:
-            state_dict = torch.load(model_path, map_location=torch.device("cpu"))
-        except Exception as e:
-            os.remove(model_path)
-            raise ValueError(
-                f"The model file appears to be broken, most likely because of permission error (deleted):\n{e}"
-            )
     else:
         logger.info(f"[grey50]Loading AlphaCube solver from cache at {model_path}", **logargs)
+    try:
         state_dict = torch.load(model_path, map_location=torch.device("cpu"))
+    except Exception as e:
+        os.remove(model_path)
+        raise ValueError(
+            "The model file appears to be broken and thus is deleted. "
+            f"This is most likely because of permission error (deleted):\n\t{e}"
+        )
 
     if model_id in ["small", "base", "large"]:
         module = Model_v1
         embed_dim, num_layers = {
             "small": (1024, 7),
             "base": (2048, 8),
             "large": (4096, 8),
@@ -120,16 +122,27 @@
     - Remove ReLU activation from the first layer (`embedding`), which had the dying ReLU problem.
     - Following the recent convention, the `embedding` layer does *not* count as one hidden layer.
     """
 
     def __init__(self, hidden_size=4096, num_hidden_layers=8, input_dim=324, output_dim=18):
         super(Model, self).__init__()
         self.embedding = nn.Linear(input_dim, hidden_size, bias=False)
-        self.layers = nn.ModuleList([LinearBlock(hidden_size, hidden_size) for i in range(num_hidden_layers)])
+        self.layers = nn.ModuleList(
+            [LinearBlock(hidden_size, hidden_size) for i in range(num_hidden_layers)]
+        )
         self.head = nn.Linear(hidden_size, output_dim, bias=False)
+        self.reset_parameters()
+
+    def reset_parameters(self):
+        nn.init.normal_(self.embedding.weight, std=1 / 54**0.5)  # There'll be 54 ones in a sample
+        for layer in self.layers:
+            nn.init.kaiming_normal_(layer.fc.weight)
+            if layer.fc.bias is not None:
+                nn.init.zeros_(layer.fc.bias)
+        nn.init.zeros_(self.head.weight)
 
     def forward(self, inputs):
         x = F.one_hot(inputs, 6).reshape(-1, 324).float()
         x = self.embedding(x)
         for layer in self.layers:
             x = layer(x)
         logits = self.head(x)
```

## alphacube/search.py

```diff
@@ -1,30 +1,62 @@
 """
 Beam Search Algorithm
 
 This module provides a function to perform beam search and find solutions for a given state.
 
 Function:
     ``beam_search``: Perform beam search to find solutions in a Rubik's Cube environment.
+
+Note:
+- `numba.jit` *slows down* operations like `_get_prune_idx` and `_map_state`
 """
 
 import time
-from contextlib import nullcontext
-
 import numpy as np
 import torch
-from rich import print
+from rich import print as rprint
+from contextlib import nullcontext
+
+from . import device, dtype, logger
 
-from . import logger
+MAX_BATCH_SIZE = 2**16  # The maximum number of states forward-pass through a DNN at a time.
 
-DEVICE = "cuda" if torch.cuda.is_available() else "mps" if torch.backends.mps.is_available() else "cpu"
-MAX_BATCH_SIZE = 2 ** 16  # The maximum number of states forward-pass through a DNN at a time.
+
+# Context: Use mixed precision training if GPU is available
+ctx = torch.autocast(device.type, dtype) if device.type != "cpu" else nullcontext()
 
 
 @torch.no_grad()
+def predict(model, batch_x, beam_width, ergonomic_bias, env):
+    batch_x = torch.from_numpy(batch_x).to(device)
+    with ctx:
+        if batch_x.shape[0] < MAX_BATCH_SIZE:
+            logits = model(batch_x)
+        else:
+            logits = torch.cat(
+                [
+                    model(split)
+                    for split in torch.tensor_split(
+                        batch_x,
+                        batch_x.shape[0] // MAX_BATCH_SIZE + 1,
+                    )
+                ]
+            )
+    batch_p = logits.softmax(-1) if beam_width > 1 else logits  # You can argmax from logits
+    batch_p = batch_p.detach().cpu().numpy()  # float32
+
+    # Apply ergonomic bias if given
+    if ergonomic_bias is not None:
+        if env.allow_wide:
+            batch_p = np.tile(batch_p, 2)
+        batch_p = np.multiply(batch_p, ergonomic_bias)
+
+    return batch_p
+
+
 def beam_search(
     env,
     model,
     beam_width,
     ergonomic_bias=None,
     extra_depths=0,
     max_depth=100,
@@ -58,231 +90,57 @@
             - 'time': The time taken (in seconds) to complete the search.
 
             If no solutions are found, returns None.
 
     """
 
     ## Setup ##
-
-    # Ensure that the model is set to evaluation mode
     model.eval()
-
-    # Initialize ergonomic bias if provided
-    if ergonomic_bias is not None:
-        # Zero-fill N/A and normalize to 1.
-        ergonomic_bias = np.array([ergonomic_bias.get(m, 0) for m in env.moves], dtype=np.half).reshape(1, -1)
-        if np.all(ergonomic_bias[:, 18:] == 0):
-            logger.info("All wide moves (e.g., r2, f2) seem to be 0 ── starting to solve only with flat moves...")
-            # If wide moves are disabled, switch to flat-move mode
-            env.allow_wide = False
-            env.moves_ix_inference = env.moves_ix_inference[:18]
-            ergonomic_bias = ergonomic_bias[:, :18]
-            logger.debug(f"{ergonomic_bias.shape=}")
-        ergonomic_bias /= ergonomic_bias.mean()
-        logger.debug(f"{ergonomic_bias=}")
-    else:
-        # There is no point in wide moves with no ergonomic bias
-        env.allow_wide = False
-        env.moves_ix_inference = env.moves_ix_inference[:18]
-
-    # Context: Use mixed precision training if GPU is available
-    ctx = torch.autocast(DEVICE, dtype=torch.float16) if DEVICE != 'cpu' else nullcontext()
+    ergonomic_bias, env = _reflect_setup(ergonomic_bias, env)
 
     # Initialize candidate paths and their corresponding states and estimated probabilities
-    candidates = {
-        "cumprod": np.array([1.0], dtype=np.half),  # Cumulative probability of candidate paths
-        "state": env.state[None, :],  # Current state
-        "path": np.array([[]], dtype=np.byte),  # Sequence of move indices constituting each path
-    }
-    solutions = {"solutions": [], "num_nodes": 0, "time": time.monotonic()}
+    candidates = dict(
+        # Sequences of move indices constituting each path
+        path=np.array([[]], dtype=np.byte),
+        # Cumulative probability of candidate paths
+        cumlogprob=np.array([0], dtype=np.single),
+        # Corresponding states
+        state=env.state[None, :],
+    )
+    solutions = dict(solutions=[], num_nodes=0, time=time.monotonic())
 
     # Debug utilities
 
-    def validate_state(i, centered=True):
-        env.state[:] = candidates["state"][i]
-        try:
-            env.validate(centered=centered)
-        except Exception:
-            print("[Path]")
-            print(" ".join([env.moves[_] for _ in candidates["path"][i, :]]))
-            print("[State]")
-            env.show(flat=True)
-            raise ValueError("State validation failed.")
-
-    if logger.level <= 10:
+    if logger.level < 20:
         logger.debug(f"{env.moves=}")
         logger.debug("env.state:")
         env.show(flat=True)
 
     ## Execute ##
-
     for depth in range(max_depth):
         if logger.level <= 20:
-            print(f"Current depth: {depth}", end="\r")
+            rprint(f"Current depth: {depth}", end="\r")
 
-        ### Get a probability distribution for each candidate state ###
-
-        with ctx:
-            # Compute batch probabilities
-            batch_x = torch.from_numpy(candidates["state"]).to(DEVICE)
-            if len(candidates["cumprod"]) < MAX_BATCH_SIZE:
-                logits = model(batch_x)
-            else:
-                logits = torch.cat(
-                    [
-                        model(split)
-                        for split in torch.tensor_split(
-                            batch_x,
-                            len(candidates["cumprod"]) // MAX_BATCH_SIZE + 1,
-                        )
-                    ]
-                )
-            batch_p = torch.nn.functional.softmax(logits, -1) if beam_width > 1 else logits
-            batch_p = batch_p.half().detach().cpu().numpy()
-
-        ### Evaluate each candidate base on cumprod ###
-
-        # Apply ergonomic bias if given
-        if ergonomic_bias is not None:
-            # Expand batch_p -> include wide moves
-            if env.allow_wide:
-                batch_p = np.tile(batch_p, 2)
-            batch_p = np.multiply(batch_p, ergonomic_bias)
-
-        # Calculate log-sum of the cumulative probability of each candidate path
-        # Equivalent to `candidates["cumprod"] = np.multiply(batch_p, candidates["cumprod"][:, None]).reshape(-1)`
-        with np.errstate(divide='ignore'):
-            candidates["cumprod"] = (candidates["cumprod"][:, None] + np.log(batch_p)).reshape(-1)
-
-        # Expand states & paths as the next-depth candidates
-        candidates["state"] = np.repeat(candidates["state"], len(env.moves_ix_inference), axis=0)
-        candidates["path"] = np.hstack(
-            (
-                np.repeat(candidates["path"], len(env.moves_ix_inference), axis=0),
-                np.tile(env.moves_ix_inference, batch_p.shape[0])[:, None],
-            )
+        # Get a probability distribution for each candidate state
+        batch_x = candidates["state"]
+        batch_p = predict(model, batch_x, beam_width, ergonomic_bias, env)
+        candidates = update_candidates(candidates, batch_p, env, depth, beam_width)
+
+        # For record, add the number of current candidates to the node count
+        solutions["num_nodes"] += candidates["path"].shape[0]
+
+        ## Check if solved any & also done ##
+        # Convert candidate states to bytes for goal collation;
+        # the variable `candidates_state_bytes` is also gonna be used to dedupe candidates at the bottom
+        candidates_state_bytes = np.array(
+            [bytes(c_state.tolist()) for c_state in candidates["state"]]
         )
 
-        # Prune candidates based on previous moves
-        if depth:
-            # Face indices
-            mod_first_last_moves = candidates["path"][:, -1] // 3
-            mod_second_last_moves = candidates["path"][:, -2] // 3
-            if env.allow_wide:
-                # Reduce wide group as ordinary group
-                mod_first_last_moves = mod_first_last_moves % 6
-                mod_second_last_moves = mod_second_last_moves % 6
-
-            # 1. Two subsequent moves on a same face
-            prune_idx = mod_second_last_moves == mod_first_last_moves
-            if depth > 1:
-                # Two moves on a same face with an opposite move in between
-                prune_idx = np.logical_or(
-                    prune_idx,
-                    np.logical_and(
-                        candidates["path"][:, -3] // 3 == mod_first_last_moves,
-                        mod_second_last_moves // 2 == mod_first_last_moves // 2,
-                    ),
-                )
-            candidates = {k: v[~prune_idx] for k, v in candidates.items()}
-
-        # Sort & select best k candidates
-        sorted_indices = np.argsort(-candidates["cumprod"])[:beam_width]
-        candidates = {k: v[sorted_indices] for k, v in candidates.items()}
-
-        ### Update states based on the expanded paths ###
-
-        if not env.allow_wide:
-            logger.debug("[ sticker replacement ]")
-            state_ix = np.arange(0, len(sorted_indices), dtype=np.intc)[:, None] * 54  # [[0], [54], [108], [162], ...]
-            move_indices = candidates["path"][:, -1]
-            target_ix = state_ix + env.sticker_target_ix[move_indices]
-            source_ix = state_ix + env.sticker_source_ix[move_indices]
-            if logger.level <= 10:
-                assert state_ix.ndim == 2 and move_indices.ndim == 1
-                logger.debug(f"{state_ix.shape=}\n{move_indices.shape=}")  # (8, 1)\n(8, )
-                logger.debug(f"{target_ix.shape=}\n{source_ix.shape=}")  # (8, 20)\n(8, 20)
-                for i in range(len(sorted_indices)):
-                    validate_state(i)
-            # Sticker replacement on the batch level (executed in the flattened view)
-            candidates["state"].flat[target_ix.flatten()] = candidates["state"].flat[source_ix.flatten()]
-            if logger.level <= 10:
-                for i in range(len(sorted_indices)):
-                    validate_state(i)
-        else:
-            # State transitions are split into two parts: flat moves and wide moves
-            # 1. Apply ordinary moves
-            indices_flat = np.argwhere(candidates["path"][:, -1] < 18)
-            if len(indices_flat):
-                logger.debug("[ Flat-move transition ]")
-                move_indices = candidates["path"][indices_flat, -1].flatten()
-
-                logger.debug(" - sticker replacement")
-                state_ix = indices_flat * 54
-                target_ix, source_ix = (
-                    state_ix + env.sticker_target_ix[move_indices],
-                    state_ix + env.sticker_source_ix[move_indices],
-                )
-                if logger.level <= 10:
-                    assert state_ix.ndim == 2 and move_indices.ndim == 1
-                    logger.debug(f"{state_ix.shape=}\n{move_indices.shape=}")  # (8, 1)\n(8, )
-                    logger.debug(f"{target_ix.shape=}\n{source_ix.shape=}")  # (8, 20)\n(8, 20)
-                    for i in indices_flat.flatten():
-                        validate_state(i)
-                candidates["state"].flat[target_ix.flatten()] = candidates["state"].flat[source_ix.flatten()]
-                if logger.level <= 10:
-                    for i in indices_flat.flatten():
-                        validate_state(i)
-
-            # 2. Apply wide moves
-            indices_wide = np.argwhere(candidates["path"][:, -1] > 17)
-            if len(indices_wide):
-                logger.debug("[ Wide-move transition ]")
-                move_indices = candidates["path"][indices_wide, -1].flatten() - 18
-
-                logger.debug(" - Sticker replacement")
-                state_ix = indices_wide * 54  # array([[  54], [ 162], [ 270], [ 378], [ 486], [ 594], [ 648] ...
-                target_ix = state_ix + env.sticker_target_ix_wide[move_indices]
-                source_ix = state_ix + env.sticker_source_ix_wide[move_indices]
-                if logger.level <= 10:
-                    assert state_ix.ndim == 2 and move_indices.ndim == 1
-                    logger.debug(f"{state_ix.shape=}\n{move_indices.shape=}")  # (8, 1)\n(8, )
-                    logger.debug(f"{target_ix.shape=}\n{source_ix.shape=}")  # (8, 20)\n(8, 20)
-                    for i in indices_flat.flatten():
-                        validate_state(i)
-                candidates["state"].flat[target_ix.flatten()] = candidates["state"].flat[source_ix.flatten()]
-                if logger.level <= 10:
-                    for i in indices_wide.flatten():
-                        validate_state(i, centered=False)
-
-                logger.debug(" - Reset color indices according to center colors after wide moves")
-                # 1. Get center colors
-                centers = candidates["state"][indices_wide, env.CENTER_INDICES]
-                indices_wide = indices_wide.flatten()  # can be flattened once sliced
-                # 2. Sort center indices, to which current colors are re-indexed.
-                mapping = np.argsort(centers, axis=1)
-                mapping_indices = np.arange(len(indices_wide))[:, None]
-                logger.debug(
-                    f"{mapping.shape=}\n{mapping_indices.shape=}\n{candidates['state'][indices_wide, :].shape=}"
-                )
-                candidates["state"][indices_wide, :] = mapping[mapping_indices, candidates["state"][indices_wide, :]]
-                if logger.level <= 10:
-                    for i in indices_wide:
-                        validate_state(i)
-
-        ### Check if solved & done ###
-
-        # Convert candidate states to bytes for goal collation AND uniqueness comparison
-        candidates_state_bytes = np.array([bytes(c_state.tolist()) for c_state in candidates["state"]])
-        is_solved = candidates_state_bytes == bytes(env.GOAL.tolist())
-        # Add the number of current candidates to the node count
-        solutions["num_nodes"] += len(sorted_indices)
-
-        # Check for solved states
-        solved_indices = np.where(is_solved)[0]
+        # Check for solved states; stringify & append to the list of solutions
+        solved_indices = np.where(candidates_state_bytes == bytes(env.GOAL.tolist()))[0]
         for c_ix in solved_indices:
             path = [env.moves[i] for i in candidates["path"][c_ix]]
             if path[:-2] not in [p[:-2] for p in solutions["solutions"]]:
                 solutions["solutions"].append(path)
 
         # Return when solutions found or max_depth reached
         if solutions["solutions"] and depth + 1 in [
@@ -290,17 +148,163 @@
             len(solutions["solutions"][0]) + extra_depths,
         ]:
             # Finally include the time taken
             solutions["time"] = time.monotonic() - solutions["time"]
             # Convert each list of solutions to string notation
             solutions["solutions"] = [" ".join(path) for path in solutions["solutions"]]
             if logger.level <= 20:
-                print()  # Avoid conflict with the current-depth log
+                rprint()  # To avoid conflict with the current-depth log
             return solutions
 
-        ### Otherwise, dedupe & pass to the next depth ###
-
+        # Otherwise, dedupe & pass to the next depth
         # Prune duplicated candidates based on their state uniqueness
         unique_indices = np.unique(candidates_state_bytes, return_index=True)[1]
         if len(solved_indices):
             unique_indices = np.setdiff1d(unique_indices, solved_indices)
         candidates = {k: v[unique_indices] for k, v in candidates.items()}
+
+
+def _reflect_setup(ergonomic_bias, env):
+    # Initialize ergonomic bias if provided
+    if ergonomic_bias is not None:
+        # Zero-fill N/A and normalize to 1.
+        ergonomic_bias = np.array(
+            [ergonomic_bias.get(m, 0) for m in env.moves], dtype=np.single
+        ).reshape(1, -1)
+        if np.all(ergonomic_bias[:, 18:] == 0):
+            logger.info(
+                "All wide moves (e.g., r2, f2) seem to be 0 ── starting to solve only with flat moves..."
+            )
+            # If wide moves are disabled, switch to flat-move mode
+            env.allow_wide = False
+            env.moves_ix_inference = env.moves_ix_inference[:18]
+            ergonomic_bias = ergonomic_bias[:, :18]
+            logger.debug(f"{ergonomic_bias.shape=}")
+        ergonomic_bias /= ergonomic_bias.mean()
+        logger.debug(f"{ergonomic_bias=}")
+    else:
+        # There is no point in wide moves with no ergonomic bias
+        env.allow_wide = False
+        env.moves_ix_inference = env.moves_ix_inference[:18]
+
+    return ergonomic_bias, env
+
+
+def update_candidates(candidates, batch_p, env, depth, beam_width):
+    # Accumulate the log-probability of each candidate path
+    # Non-log equivalent:
+    # `candidates["cumprob"] = np.multiply(batch_p, candidates["cumprob"][:, None]).reshape(-1)`
+    with np.errstate(divide="ignore"):
+        candidates["cumlogprob"] = (candidates["cumlogprob"][:, None] + np.log(batch_p)).reshape(-1)
+
+    # Expand states & paths as the next-depth candidates
+    candidates["state"] = np.repeat(candidates["state"], len(env.moves_ix_inference), axis=0)
+    candidates["path"] = np.hstack(
+        (
+            np.repeat(candidates["path"], len(env.moves_ix_inference), axis=0),
+            np.tile(env.moves_ix_inference, batch_p.shape[0])[:, None],
+        )
+    )
+
+    # Prune candidates based on previous moves
+    if depth:
+        prune_idx = _get_prune_idx(candidates["path"], env.allow_wide, depth)
+        candidates = {k: v[~prune_idx] for k, v in candidates.items()}
+
+    # Sort & select best k candidates
+    sorted_indices = np.argsort(-candidates["cumlogprob"])[:beam_width]
+    candidates = {k: v[sorted_indices] for k, v in candidates.items()}
+
+    # Update states based on the expanded paths ###
+    candidates["state"] = _update_states(candidates["state"], candidates["path"], env)
+    return candidates
+
+
+def _get_prune_idx(candidates_paths, allow_wide, depth):
+    # Face indices
+    mod_first_last_moves = candidates_paths[:, -1] // 3
+    mod_second_last_moves = candidates_paths[:, -2] // 3
+    if allow_wide:
+        # Reduce wide group as ordinary group
+        mod_first_last_moves = mod_first_last_moves % 6
+        mod_second_last_moves = mod_second_last_moves % 6
+
+    # 1. Two subsequent moves on a same face
+    prune_idx = mod_second_last_moves == mod_first_last_moves
+    if depth > 1:
+        # Two moves on a same face with an opposite move in between
+        prune_idx = np.logical_or(
+            prune_idx,
+            np.logical_and(
+                candidates_paths[:, -3] // 3 == mod_first_last_moves,
+                mod_second_last_moves // 2 == mod_first_last_moves // 2,
+            ),
+        )
+    return prune_idx
+
+
+def _update_states(candidate_states, candidate_paths, env):
+    if not env.allow_wide:
+        logger.debug("[ sticker replacement ]")
+        state_ix = (
+            np.arange(0, candidate_paths.shape[0], dtype=np.intc)[:, None] * 54
+        )  # [[0], [54], [108], [162], ...]
+        move_indices = candidate_paths[:, -1]
+        target_ix = state_ix + env.sticker_target_ix[move_indices]
+        source_ix = state_ix + env.sticker_source_ix[move_indices]
+        if logger.level <= 10:
+            assert state_ix.ndim == 2 and move_indices.ndim == 1
+            logger.debug(f"{state_ix.shape=}\n{move_indices.shape=}")  # (8, 1)\n(8, )
+            logger.debug(f"{target_ix.shape=}\n{source_ix.shape=}")  # (8, 20)\n(8, 20)
+            for i in range(candidate_paths.shape[0]):
+                env.validate(state=candidate_states[i], centered=True)
+        candidate_states = _map_state(candidate_states, target_ix, source_ix)
+        if logger.level <= 10:
+            for i in range(candidate_paths.shape[0]):
+                env.validate(state=candidate_states[i], centered=True)
+    else:
+        indices_flat = np.argwhere(candidate_paths[:, -1] < 18)
+        if len(indices_flat):
+            logger.debug("[ Flat-move transition ]")
+            move_indices = candidate_paths[indices_flat, -1].flatten()
+            logger.debug(" - sticker replacement")
+            state_ix = indices_flat * 54
+            target_ix, source_ix = (
+                state_ix + env.sticker_target_ix[move_indices],
+                state_ix + env.sticker_source_ix[move_indices],
+            )
+            candidate_states = _map_state(candidate_states, target_ix, source_ix)
+
+        indices_wide = np.argwhere(candidate_paths[:, -1] > 17)
+        if len(indices_wide):
+            logger.debug("[ Wide-move transition ]")
+            move_indices = candidate_paths[indices_wide, -1].flatten() - 18
+            logger.debug(" - Sticker replacement")
+            state_ix = indices_wide * 54
+            target_ix = state_ix + env.sticker_target_ix_wide[move_indices]
+            source_ix = state_ix + env.sticker_source_ix_wide[move_indices]
+
+            candidate_states = _map_state(candidate_states, target_ix, source_ix)
+
+            logger.debug(" - Reset color indices according to center colors after wide moves")
+            centers = candidate_states[indices_wide, env.CENTER_INDICES]
+            indices_wide = indices_wide.flatten()
+            mapping = np.argsort(centers, axis=1)
+            mapping_indices = np.arange(len(indices_wide))[:, None]
+            logger.debug(
+                f"{mapping.shape=}\n{mapping_indices.shape=}\n{candidate_states[indices_wide, :].shape=}"
+            )
+            candidate_states[indices_wide, :] = mapping[
+                mapping_indices, candidate_states[indices_wide, :]
+            ]
+    return candidate_states
+
+
+def _map_state(candidate_states, target_ix, source_ix):
+    # Sticker replacement on the batch level (executed in the flattened view)
+    flat_states = candidate_states.ravel()
+    flat_states[target_ix.flatten()] = flat_states[source_ix.flatten()]
+    candidate_states = flat_states.reshape(candidate_states.shape)
+    # Slightly faster than:
+    # candidate_states.flat[target_ix.flatten()] = candidate_states.flat[source_ix.flatten()]
+    # which also doesn't work with `numba.jit`
+    return candidate_states
```

## Comparing `alphacube/solver.py` & `alphacube/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,39 +6,44 @@
 Class:
 
 - ``Solver``: A class for managing Rubik's Cube configuration, solving model, and search function.
 
 Example::
 
     from alphacube.solver import Solver
-    solver = Solver() # Assigned to `alphacube._solver` at the package level.
+    solver = Solver() # Assigned to `alphacube.solver` at the package level.
     solver.load()
     solution = solver(format='moves', scramble="R U R' U'", beam_width=1024)
 
 """
 
 import torch
 
-from . import logargs, logger
+from . import logger, logargs, device
+
 from .env import Cube3
 from .model import load_model
 from .search import beam_search
-
-DEVICE = "cuda" if torch.cuda.is_available() else "mps" if torch.backends.mps.is_available() else "cpu"
+from ._evaluator import evaluate_search_efficiency, evaluate_temporal_performance
 
 
 class Solver:
     """
     A solver class for managing environment, model, and search configurations.
     Methods:
     - ``load``: Load the solver model and optimize it for CPU or GPU.
     - ``__call__``: Set up the cube state and pass it for solution using beam search.
     """
 
-    def load(self, model_id, prefer_gpu=True, quantize_on_cpu=True, jit_mode=False, *args, **kwargs):
+    evaluate_search_efficiency = evaluate_search_efficiency
+    evaluate_temporal_performance = evaluate_temporal_performance
+
+    def load(
+        self, model_id, prefer_gpu=True, quantize_on_cpu=True, jit_mode=False, *args, **kwargs
+    ):
         """
         Load the Rubik's Cube solver model and optimize it for CPU or GPU.
 
         Args:
             model_id (str): Identifier for the model variant to load ("small", "base", or "large").
             prefer_gpu (bool): Whether to prefer GPU if available.
             quantize_on_cpu (bool): Whether to quantize the model for CPU optimization.
@@ -46,27 +51,33 @@
             *args: Additional arguments for model loading.
             **kwargs: Additional keyword arguments for model loading and optimization.
 
         Returns:
             None
         """
         # Load the model (download if not yet)
-        self.model = load_model(model_id, *args, **kwargs)
-        if prefer_gpu and DEVICE != "cpu":
-            logger.info(f"[grey50]Running on {DEVICE.upper()}", **logargs)
-            self.model.to(DEVICE)
+        self.model_id = model_id
+        self.model = load_model(self.model_id, *args, **kwargs)
+        if prefer_gpu and device.type != "cpu":
+            logger.info(f"[grey50]Running on {device.type.upper()}", **logargs)
+            self.model.to(device)
         else:
             logger.info("[grey50]Running on CPU (no GPU found)", **logargs)
             if quantize_on_cpu:
-                logger.info("[grey50]Quantizing the model -- roughly 3x faster [italic]on CPU", **logargs)
-                self.model = torch.ao.quantization.quantize_dynamic(self.model, {torch.nn.Linear}, dtype=torch.qint8)
+                logger.info(
+                    "[grey50]Quantizing the model -- roughly 3x faster [italic]on CPU", **logargs
+                )
+                self.model = torch.ao.quantization.quantize_dynamic(
+                    self.model, {torch.nn.Linear}, dtype=torch.qint8
+                )
 
         if jit_mode:
             logger.info(
-                "[grey50]JIT-mode enabled -- [italic]potentially[/italic] faster than eager execution", **logargs
+                "[grey50]JIT-mode enabled -- [italic]potentially[/italic] faster than eager execution",
+                **logargs,
             )
             self.model = torch.jit.script(self.model)
 
         logger.info("[cyan]Initialized AlphaCube solver.", **logargs)
 
     def __call__(self, scramble, format="moves", allow_wide=True, **kwargs):
         """
```

## Comparing `alphacube-0.1.3.dist-info/LICENSE` & `alphacube-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `alphacube-0.1.3.dist-info/METADATA` & `alphacube-0.1.4.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphacube
-Version: 0.1.3
+Version: 0.1.4
 Summary: A powerful & flexible Rubik's Cube solver
 Author: Kyo Takano
 License: MIT License
         
         Copyright (c) 2023 Kyo Takano
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,14 +43,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch >=2.0.1
 Requires-Dist: numpy >=1.23.3
 Requires-Dist: rich >=13.0.1
 Requires-Dist: pydantic >=2.0.3
 Requires-Dist: requests >=2.28.2
+Requires-Dist: tqdm
 
 # AlphaCube
 
 AlphaCube is a powerful & flexible Rubik's Cube solver that extends [EfficientCube](https://github.com/kyo-takano/efficientcube). It uses a Deep Neural Network (DNN) to find optimal/near-optimal solutions for a given scrambled state.
 
 > [!NOTE]
 > **🎮 Try the interactive demo: [alphacube.dev](https://alphacube.dev)**
@@ -210,17 +211,18 @@
 > {
 >     'solutions': ["D F L' F' U2 B2 U F' L R2 B2 U D' F2 U2 R D'"],
 >     'num_nodes': 903448,
 >     'time': 20.46845487099995
 > }
 > ```
 
-Using a GPU provides an order of magnitude speedup over CPU especially for larger models.
+Using a GPU provides an order of magnitude speedup over CPUs, especially for larger models.
 
-> [!IMPORTANT] When running AlphaCube _on a CPU_, it's generally recommended to stick with the `"small"` model, as the larger `"base"` and `"large"` models would take considerably more time to find solutions.
+> [!IMPORTANT]
+> When running AlphaCube _on a CPU_, it's generally recommended to stick with the `"small"` model, as the larger `"base"` and `"large"` models would take considerably more time to find solutions.
 
 Please refer to our [documentation](https://alphacube.dev/docs) for more, especially ["Getting Started"](https://alphacube.dev/docs/getting-started/index.html)
 
 ## How It Works
 
 At the heart of AlphaCube lies a deep learning method described in ["Self-Supervision is All You Need for Solving Rubik's Cube" (TMLR'23)](https://openreview.net/forum?id=bnBeNFB27b), the official code of which is also available as [EfficientCube](https://github.com/kyo-takano/efficientcube).
```

