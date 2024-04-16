# Comparing `tmp/duo_game_lib-0.1.0.tar.gz` & `tmp/duo_game_lib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duo_game_lib-0.1.0.tar", max compression
+gzip compressed data, was "duo_game_lib-0.1.1.tar", max compression
```

## Comparing `duo_game_lib-0.1.0.tar` & `duo_game_lib-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      395 2024-04-11 14:27:43.287716 duo_game_lib-0.1.0/README.md
--rw-r--r--   0        0        0      526 2024-04-11 14:27:43.291716 duo_game_lib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 14:27:43.291716 duo_game_lib-0.1.0/src/duo_game_lib/__init__.py
--rw-r--r--   0        0        0     3113 2024-04-11 14:27:43.291716 duo_game_lib-0.1.0/src/duo_game_lib/game.py
--rw-r--r--   0        0        0      275 2024-04-11 14:27:43.291716 duo_game_lib-0.1.0/src/duo_game_lib/game_state.py
--rw-r--r--   0        0        0     1710 2024-04-11 14:27:43.291716 duo_game_lib-0.1.0/src/duo_game_lib/judge.py
--rw-r--r--   0        0        0     1409 2024-04-11 14:27:43.291716 duo_game_lib-0.1.0/src/duo_game_lib/move.py
--rw-r--r--   0        0        0      998 2024-04-11 14:27:43.291716 duo_game_lib-0.1.0/src/duo_game_lib/player.py
--rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 duo_game_lib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      395 2024-04-16 10:57:31.966615 duo_game_lib-0.1.1/README.md
+-rw-r--r--   0        0        0      526 2024-04-16 10:57:31.966615 duo_game_lib-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 10:57:31.966615 duo_game_lib-0.1.1/src/duo_game_lib/__init__.py
+-rw-r--r--   0        0        0     3124 2024-04-16 10:57:31.966615 duo_game_lib-0.1.1/src/duo_game_lib/game.py
+-rw-r--r--   0        0        0      275 2024-04-16 10:57:31.966615 duo_game_lib-0.1.1/src/duo_game_lib/game_state.py
+-rw-r--r--   0        0        0     1710 2024-04-16 10:57:31.966615 duo_game_lib-0.1.1/src/duo_game_lib/judge.py
+-rw-r--r--   0        0        0     1409 2024-04-16 10:57:31.966615 duo_game_lib-0.1.1/src/duo_game_lib/move.py
+-rw-r--r--   0        0        0      998 2024-04-16 10:57:31.966615 duo_game_lib-0.1.1/src/duo_game_lib/player.py
+-rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 duo_game_lib-0.1.1/PKG-INFO
```

### Comparing `duo_game_lib-0.1.0/pyproject.toml` & `duo_game_lib-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "duo-game-lib"
-version = "0.1.0"
+version = "0.1.1"
 description = "Logic for turn-based duo game"
 authors = ["game-ai-platform-team"]
 readme = "README.md"
 packages = [{ include = "duo_game_lib/**/*.py", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `duo_game_lib-0.1.0/src/duo_game_lib/game.py` & `duo_game_lib-0.1.1/src/duo_game_lib/game.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
                 state,
                 MoveMetadata(
                     elapsed_time,
                     self.__judge.analyze(),
                     player.get_and_reset_current_logs(),
                 ),
             )
-            self.__logger(move_object)
+            self.__logger(f"MOVE: {move_object}")
 
             previous_move = move
 
             if debug:
                 self.__print_debug_info(move_object)
 
             i += 1
```

### Comparing `duo_game_lib-0.1.0/src/duo_game_lib/judge.py` & `duo_game_lib-0.1.1/src/duo_game_lib/judge.py`

 * *Files identical despite different names*

### Comparing `duo_game_lib-0.1.0/src/duo_game_lib/move.py` & `duo_game_lib-0.1.1/src/duo_game_lib/move.py`

 * *Files identical despite different names*

### Comparing `duo_game_lib-0.1.0/src/duo_game_lib/player.py` & `duo_game_lib-0.1.1/src/duo_game_lib/player.py`

 * *Files identical despite different names*

### Comparing `duo_game_lib-0.1.0/PKG-INFO` & `duo_game_lib-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duo-game-lib
-Version: 0.1.0
+Version: 0.1.1
 Summary: Logic for turn-based duo game
 Author: game-ai-platform-team
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

