# Comparing `tmp/hypickle-1.1.4.tar.gz` & `tmp/hypickle-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypickle-1.1.4.tar", last modified: Mon Apr 15 01:23:53 2024, max compression
+gzip compressed data, was "hypickle-1.1.5.tar", last modified: Tue Apr 16 04:18:27 2024, max compression
```

## Comparing `hypickle-1.1.4.tar` & `hypickle-1.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:23:53.760522 hypickle-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-15 01:23:47.000000 hypickle-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-15 01:23:53.760522 hypickle-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-15 01:23:47.000000 hypickle-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:23:53.760522 hypickle-1.1.4/hypickle/
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-15 01:23:47.000000 hypickle-1.1.4/hypickle/Args.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-15 01:23:47.000000 hypickle-1.1.4/hypickle/Colours.py
--rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-04-15 01:23:47.000000 hypickle-1.1.4/hypickle/Files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-15 01:23:47.000000 hypickle-1.1.4/hypickle/Graphing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-04-15 01:23:47.000000 hypickle-1.1.4/hypickle/MyClasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-15 01:23:47.000000 hypickle-1.1.4/hypickle/Pit.py
--rw-r--r--   0 runner    (1001) docker     (127)    21662 2024-04-15 01:23:47.000000 hypickle-1.1.4/hypickle/Player.py
--rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-04-15 01:23:47.000000 hypickle-1.1.4/hypickle/ProcessingResults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-15 01:23:47.000000 hypickle-1.1.4/hypickle/Rank.py
--rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-04-15 01:23:47.000000 hypickle-1.1.4/hypickle/Utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:23:47.000000 hypickle-1.1.4/hypickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-15 01:23:47.000000 hypickle-1.1.4/hypickle/additional_friends.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-15 01:23:47.000000 hypickle-1.1.4/hypickle/bedwars.py
--rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-04-15 01:23:47.000000 hypickle-1.1.4/hypickle/hypixel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-15 01:23:47.000000 hypickle-1.1.4/hypickle/leveling.py
--rw-r--r--   0 runner    (1001) docker     (127)    12512 2024-04-15 01:23:47.000000 hypickle-1.1.4/hypickle/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:23:53.760522 hypickle-1.1.4/hypickle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-15 01:23:53.000000 hypickle-1.1.4/hypickle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-15 01:23:53.000000 hypickle-1.1.4/hypickle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 01:23:53.000000 hypickle-1.1.4/hypickle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 01:23:53.000000 hypickle-1.1.4/hypickle.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-15 01:23:53.000000 hypickle-1.1.4/hypickle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 01:23:53.000000 hypickle-1.1.4/hypickle.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-15 01:23:47.000000 hypickle-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 01:23:53.760522 hypickle-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:18:27.921513 hypickle-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 04:18:23.000000 hypickle-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-16 04:18:27.921513 hypickle-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-16 04:18:23.000000 hypickle-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:18:27.921513 hypickle-1.1.5/hypickle/
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-16 04:18:23.000000 hypickle-1.1.5/hypickle/Args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-04-16 04:18:23.000000 hypickle-1.1.5/hypickle/Colours.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-16 04:18:23.000000 hypickle-1.1.5/hypickle/Files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-16 04:18:23.000000 hypickle-1.1.5/hypickle/Graphing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-04-16 04:18:23.000000 hypickle-1.1.5/hypickle/MyClasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-04-16 04:18:23.000000 hypickle-1.1.5/hypickle/Pit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21626 2024-04-16 04:18:23.000000 hypickle-1.1.5/hypickle/Player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8994 2024-04-16 04:18:23.000000 hypickle-1.1.5/hypickle/ProcessingResults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-16 04:18:23.000000 hypickle-1.1.5/hypickle/Rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-04-16 04:18:23.000000 hypickle-1.1.5/hypickle/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 04:18:23.000000 hypickle-1.1.5/hypickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-16 04:18:23.000000 hypickle-1.1.5/hypickle/additional_friends.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-16 04:18:23.000000 hypickle-1.1.5/hypickle/bedwars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-04-16 04:18:23.000000 hypickle-1.1.5/hypickle/hypixel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-16 04:18:23.000000 hypickle-1.1.5/hypickle/leveling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12534 2024-04-16 04:18:23.000000 hypickle-1.1.5/hypickle/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:18:27.921513 hypickle-1.1.5/hypickle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-16 04:18:27.000000 hypickle-1.1.5/hypickle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-16 04:18:27.000000 hypickle-1.1.5/hypickle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 04:18:27.000000 hypickle-1.1.5/hypickle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 04:18:27.000000 hypickle-1.1.5/hypickle.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-16 04:18:27.000000 hypickle-1.1.5/hypickle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 04:18:27.000000 hypickle-1.1.5/hypickle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-16 04:18:23.000000 hypickle-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 04:18:27.921513 hypickle-1.1.5/setup.cfg
```

### Comparing `hypickle-1.1.4/LICENSE` & `hypickle-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.4/PKG-INFO` & `hypickle-1.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: hypickle
-Version: 1.1.4
+Version: 1.1.5
 Summary: A script that outputs realtime stats for custom lists of friends you create.
 Author-email: John Doknjas <jdoknjas@sfu.ca>
 Project-URL: Homepage, https://github.com/johndoknjas/hypixel-online-friends
 Keywords: hypickle,hypixel,pit,bedwars,friends,stats,api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.0
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: deepdiff
 Requires-Dist: mplcursors
 
@@ -57,14 +57,15 @@
 
 Open the root directory of the project in the terminal, and then:
   - `python3 main.py *args*` allows you to test any local changes you've made to the project.
   - `vulture .` will find unused code.
   - `mypy .` will typecheck.
   - `pylint *.py` will review the code for style.
   - `pydeps hypickle` will output a dependency graph of the project's modules.
-  - `python unused-funcs.py` is a basic script I wrote that attempts to find functions which are never/rarely used.
-  - `pytest tests.py` runs a few basic automated tests. Requires installing `pytest`. To run manual tests (output to
+  - `python my-linter.py` is a basic script I wrote that mainly attempts to find functions which are never/rarely used.
+  - `pytest tests.py` runs a few basic automated tests. To run manual tests (output to
     the screen needs to be judged by the tester), run `python tests.py`.
+  - `vermin hypickle` deduces the oldest version of python that works to run the project. The expected output is 3.8, corresponding with `requires-python = ">= 3.8"` in `pyproject.toml`.
 
 ### Acknowledgements:
 
 The `hypixel.py` and `leveling.py` files were originally from [Snuggle's repo](https://github.com/Snuggle/hypixel.py/). Since then I have made a number of modifications to them.
```

### Comparing `hypickle-1.1.4/README.md` & `hypickle-1.1.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
 Open the root directory of the project in the terminal, and then:
   - `python3 main.py *args*` allows you to test any local changes you've made to the project.
   - `vulture .` will find unused code.
   - `mypy .` will typecheck.
   - `pylint *.py` will review the code for style.
   - `pydeps hypickle` will output a dependency graph of the project's modules.
-  - `python unused-funcs.py` is a basic script I wrote that attempts to find functions which are never/rarely used.
-  - `pytest tests.py` runs a few basic automated tests. Requires installing `pytest`. To run manual tests (output to
+  - `python my-linter.py` is a basic script I wrote that mainly attempts to find functions which are never/rarely used.
+  - `pytest tests.py` runs a few basic automated tests. To run manual tests (output to
     the screen needs to be judged by the tester), run `python tests.py`.
+  - `vermin hypickle` deduces the oldest version of python that works to run the project. The expected output is 3.8, corresponding with `requires-python = ">= 3.8"` in `pyproject.toml`.
 
 ### Acknowledgements:
 
 The `hypixel.py` and `leveling.py` files were originally from [Snuggle's repo](https://github.com/Snuggle/hypixel.py/). Since then I have made a number of modifications to them.
```

### Comparing `hypickle-1.1.4/hypickle/Args.py` & `hypickle-1.1.5/hypickle/Args.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import List, Optional
+from __future__ import annotations
 import copy
 import re
 
 from . import Utils
 from . import Files
 
 class Args:
-    def __init__(self, args: List[str]):
+    def __init__(self, args: list[str]):
         assert re.split(r'/|\\', args[0])[-1] in ('main.py', 'hypickle')
         args = [arg if arg.endswith('.txt') else arg.lower() for arg in args[1:]]
         self._ARGS = Files.apply_aliases(args)
         self._ARG_KEYWORDS = ('all', 'friendsoffriends', 'justuuids', 'checkresults',
                               'diff', 'starsort', 'pitsort',
                               'fileoutput', 'updateuuids', 'matchingignsuuids',
                               'includemultiplayerfiles', 'keepfirstdictmultifiles',
@@ -25,21 +25,21 @@
         # These keywords are possible options the user can specify for using the program. All of these are
         # 'non-positional'; i.e., it doesn't matter where they appear in the user's command line argument list.
         # For 'positional' arguments, there are fewer (e.g., '-', 'friendedwhen', 'intersect').
         # They don't appear in this class, but are instead used directly in the logic for main.py.
         Utils.print_list(self.get_args(False), prepended_msg="self._ARGS list after applying aliases: ")
         self._validation_checks()
 
-    def get_args(self, remove_keywords_and_dates: bool) -> List[str]:
+    def get_args(self, remove_keywords_and_dates: bool) -> list[str]:
         args = copy.copy(self._ARGS)
         if remove_keywords_and_dates:
             args = Utils.remove_date_strings(Utils.list_subtract(args, self._ARG_KEYWORDS))
         return args
 
-    def get_keywords(self) -> List[str]:
+    def get_keywords(self) -> list[str]:
         return list(self._ARG_KEYWORDS)
 
     def find_friends_of_friends(self) -> bool:
         return 'friendsoffriends' in self._ARGS
 
     def just_online_friends(self) -> bool:
         return 'all' not in self._ARGS and not self.find_friends_of_friends()
@@ -55,15 +55,15 @@
 
     def sort_by_pit_rank(self) -> bool:
         return 'pitsort' in self._ARGS
 
     def just_uuids(self) -> bool:
         return 'justuuids' in self._ARGS
 
-    def date_cutoff(self) -> Optional[str]:
+    def date_cutoff(self) -> str | None:
         return Utils.get_date_string_if_exists(self._ARGS)
 
     def do_file_output(self) -> bool:
         return 'fileoutput' in self._ARGS
 
     def update_uuids(self) -> bool:
         return 'updateuuids' in self._ARGS
```

### Comparing `hypickle-1.1.4/hypickle/Colours.py` & `hypickle-1.1.5/hypickle/Colours.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from typing import Optional
 from enum import Enum
 import rich.console
 import rich.style
 
 from . import Utils
```

### Comparing `hypickle-1.1.4/hypickle/Files.py` & `hypickle-1.1.5/hypickle/Files.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Contains functions related to working with files. Only dependencies should be stuff in Utils.py,
 and stuff in this same file."""
 
+from __future__ import annotations
 import os
 import os.path
 import json
 import time
-from typing import Optional, Dict, List, Iterable, Tuple
+from typing import Optional, Iterable
 from copy import deepcopy
 import shutil
 import ntpath
 from string import whitespace
 
 from . import Utils
 
@@ -55,15 +56,15 @@
         with open(filepath, 'r') as f:
             return json.loads(f.read())
     except FileNotFoundError:
         # This could happen if the user gives a windows path when running the program with wsl. So try this:
         with open('results/' + ntpath.basename(filepath), 'r') as f:
             return json.loads(f.read())
 
-def update_uuids_file(ign_uuid_pairs: Dict[str, str]) -> None:
+def update_uuids_file(ign_uuid_pairs: dict[str, str]) -> None:
     """Updates the uuids.txt file with the ign_uuid_pairs param.
     If a uuid is found for an ign in uuids.txt that conflicts with a pair in the passed in param,
     it will be replaced. Also, this function will make a backup of uuids.txt before overwriting it."""
 
     if os.path.isfile(_UUIDS_FILENAME):
         shutil.copy(_UUIDS_FILENAME, create_file('uuids copy', 'old-uuids'))
     pairs = ign_uuid_pairs_in_uuids_txt(do_deepcopy=True)
@@ -74,15 +75,15 @@
             assert key == key.lower()
     print(f"{_UUIDS_FILENAME} now contains uuid-ign pairs for {len(pairs)} players.")
 
 def assertions_for_aliases(alias: str, meaning: str, keywords: Iterable[str]) -> None:
     assert alias not in keywords and not Utils.contains_whitespace(alias)
     assert '.txt' not in meaning and '.txt' not in alias
 
-def get_new_aliases_from_user(aliases: Dict[str, str], keywords: Iterable[str]) -> None:
+def get_new_aliases_from_user(aliases: dict[str, str], keywords: Iterable[str]) -> None:
     """Asks the user for new aliases, and updates the `aliases` parameter accordingly."""
     while True:
         alias = input("Enter alias (or 'done'/'stop' to quit): ").lower()
         if alias in ('done', 'stop', 'quit'):
             return
         meaning = input("Enter the text this alias stands for: ").lower()
         if meaning in ('del', 'delete', 'remove'):
@@ -100,33 +101,33 @@
             if input(f"To confirm replacing its meaning to be '{meaning}', enter y: ") not in ('y', 'Y'):
                 continue
         assertions_for_aliases(alias, meaning, keywords)
         aliases[alias] = meaning
         print()
 
 def add_new_ign_uuid_aliases(
-        aliases: Dict[str, str], ign_uuid_pairs: Iterable[Tuple[str, str]], keywords: Iterable[str]
+        aliases: dict[str, str], ign_uuid_pairs: Iterable[tuple[str, str]], keywords: Iterable[str]
     ) -> None:
     """Makes each ign an alias for its uuid, and adds it to `aliases` (if the ign is not
        already an existing alias)."""
     for ign, uuid in ((a.lower(), b.lower()) for a, b in ign_uuid_pairs):
         assert Utils.is_ign(ign) and Utils.is_uuid(uuid)
         assertions_for_aliases(ign, uuid, keywords)
         if ign in aliases:
             print(f"The alias {ign} already exists, so not replacing it.")
         else:
             aliases[ign] = uuid
 
 def update_aliases(
-        keywords: Iterable[str], ign_uuid_pairs: Optional[Iterable[Tuple[str, str]]] = None
+        keywords: Iterable[str], ign_uuid_pairs: Optional[Iterable[tuple[str, str]]] = None
     ) -> None:
     """ Updates aliases using user input if `ign_uuid_pairs` is None. Otherwise, goes through each
         2-tuple in `ign_uuid_pairs` and makes the ign (first elem) an alias for the uuid (second elem). """
     print_aliases()
-    aliases: Dict[str, str] = get_aliases_with_str_meanings()
+    aliases: dict[str, str] = get_aliases_with_str_meanings()
     aliases_copy = deepcopy(aliases)
     if ign_uuid_pairs is None:
         get_new_aliases_from_user(aliases, keywords)
     else:
         add_new_ign_uuid_aliases(aliases, ign_uuid_pairs, keywords)
 
     if os.path.isfile(_ALIASES_FILENAME):
@@ -137,41 +138,41 @@
 
     print_aliases(starting_phrase="\nNow")
     assert aliases == get_aliases_with_str_meanings()
     old_items, new_items = set(aliases_copy.items()), set(aliases.items())
     print(f"\nNew aliases - old aliases: {new_items - old_items}")
     print(f"Old aliases - new aliases: {old_items - new_items}")
 
-def get_aliases_with_str_meanings() -> Dict[str, str]:
+def get_aliases_with_str_meanings() -> dict[str, str]:
     """Does the same thing as `get_aliases()`, but each of the meanings is a string with words
        separated by spaces, rather than a list."""
     return {a: ' '.join(m) for a,m in get_aliases().items()}
 
-def get_aliases() -> Dict[str, List[str]]:
+def get_aliases() -> dict[str, list[str]]:
     """ Returns a list representing the aliases stored in aliases.txt. Each element of this list
         will be a tuple, where the first element is a string (the alias), and the second element
         is a list of strings (what the alias stands for). """
     if not os.path.isfile(_ALIASES_FILENAME):
         return {}
     with open(_ALIASES_FILENAME, 'r') as file:
-        lines: List[str] = file.read().splitlines()
-    aliases: Dict[str, List[str]] = {}
+        lines: list[str] = file.read().splitlines()
+    aliases: dict[str, list[str]] = {}
     for line in lines:
         split_line = [x.strip(whitespace + '"') for x in line.split('=')]
         assert line.count('=') == 1 and len(split_line) == 2 and line == line.lower()
         aliases[split_line[0]] = split_line[1].split()
     return aliases
 
 def print_aliases(starting_phrase: str = 'Currently') -> None:
     aliases = get_aliases()
     print(f"{starting_phrase} {len(aliases)} aliases:\n")
     for alias in aliases:
         print(f"{alias} = {aliases[alias]}")
     print()
 
-def apply_aliases(lst: List[str]) -> List[str]:
+def apply_aliases(lst: list[str]) -> list[str]:
     """Returns a new list that results from applying the aliases (in aliases.txt) to the strings in lst."""
     old_lst = lst
     for alias in (aliases := get_aliases()):
         lst = Utils.replace_in_list(lst, alias, aliases[alias])
     # If lst got updated, keep recursing (as some aliases may have aliases of their own):
     return apply_aliases(lst) if lst != old_lst else lst
```

### Comparing `hypickle-1.1.4/hypickle/Graphing.py` & `hypickle-1.1.5/hypickle/Graphing.py`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.4/hypickle/MyClasses.py` & `hypickle-1.1.5/hypickle/MyClasses.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 from __future__ import annotations
 
 from copy import deepcopy
-from typing import Optional, Union, List
+from typing import Optional
 import urllib3
 
 from . import Utils
 from .Args import Args
 
 _args: Optional[Args] = None
 
-def set_args(args: List[str]) -> None:
+def set_args(args: list[str]) -> None:
     global _args
     assert not _args
     _args = Args(args)
     if not _args.verify_requests():
         urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 def args() -> Args:
     assert _args
     return _args
 
 class UUID_Plus_Time:
     """This class encapsulates a UUID and a time (unix epoch), likely representing when
     the player was friended to the parent player."""
 
-    def __init__(self, uuid: str, time_val: Union[str, float, int, None]):
-        """time_val must be either a date string, or the unix epoch time in either seconds or milliseconds"""
+    def __init__(self, uuid: str, time_val: str | float | int | None):
+        """If `time_val` isn't None, it must be either a date string, or the
+           unix epoch time in seconds or milliseconds."""
         self._uuid: str = uuid
         self._unix_epoch_milliseconds: Optional[float] = None
         if isinstance(time_val, str):
             assert Utils.is_date_string(time_val)
             self._unix_epoch_milliseconds = Utils.date_to_epoch(time_val, False)
         elif isinstance(time_val, (float, int)):
             if Utils.is_in_milliseconds(time_val):
                 self._unix_epoch_milliseconds = time_val
             else:
                 self._unix_epoch_milliseconds = time_val * 1000
 
     def uuid(self) -> str:
         return self._uuid
 
-    def time_epoch_in_seconds(self) -> Optional[float]:
+    def time_epoch_in_seconds(self) -> float | None:
         return self._unix_epoch_milliseconds / 1000 if self._unix_epoch_milliseconds is not None else None
 
-    def time_epoch_in_milliseconds(self) -> Optional[float]:
+    def time_epoch_in_milliseconds(self) -> float | None:
         """Returns the time as a float representing the unix epoch time in milliseconds"""
         return self._unix_epoch_milliseconds
 
-    def date_string(self) -> Optional[str]:
+    def date_string(self) -> str | None:
         """Returns the time as a YYYY-MM-DD date string"""
         if self._unix_epoch_milliseconds is None:
             return None
         return Utils.epoch_to_date(self._unix_epoch_milliseconds, False)
 
     def sort_key(self) -> float:
         if self._unix_epoch_milliseconds is None:
@@ -86,28 +87,28 @@
         Specs.set_common_specs(not args().find_friends_of_friends())
         friendsfriendsSpecs = Specs(True, False, None, 2) if args().find_friends_of_friends() else None
         friendsSpecs = Specs(args().just_uuids(), args().just_online_friends(), friendsfriendsSpecs, 1)
         playerSpecs = Specs(False, False, friendsSpecs, 0)
         return playerSpecs
 
     def __init__(self, just_uuids: bool, player_must_be_online: bool,
-                 friends_specs: Optional[Specs], degrees_from_original_player: int):
+                 friends_specs: Specs | None, degrees_from_original_player: int):
         assert Specs._common_specs['set flag']
         self._just_uuids = just_uuids
         self._player_must_be_online = player_must_be_online
         self._friends_specs = deepcopy(friends_specs)
         self._degrees_from_original_player = degrees_from_original_player
 
     def just_uuids(self) -> bool:
         return self._just_uuids
 
     def required_online(self) -> bool:
         return self._player_must_be_online
 
-    def specs_for_friends(self) -> Optional[Specs]:
+    def specs_for_friends(self) -> Specs | None:
         return deepcopy(self._friends_specs)
 
     def degrees_from_root_player(self) -> int:
         return self._degrees_from_original_player
 
     def root_player(self) -> bool:
         return self._degrees_from_original_player == 0
```

### Comparing `hypickle-1.1.4/hypickle/Pit.py` & `hypickle-1.1.5/hypickle/Pit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from __future__ import annotations
 import math
-from typing import List, Optional, Tuple
+from typing import Optional
 
 from . import Utils
 
 """Some notes on how the pit leveling system works:
     - The PRESTIGE_XP values are the amount of total xp needed before each prestige.
     - Once a player prestiges, hypixel automatically gives them enough xp to go from level 0 to 1.
       E.g., 0-120 requires 65950 xp, while I-1 requires 65967 xp.
@@ -26,42 +27,42 @@
                1235293080, 1894793080, 5192293080,11787293080)
 # https://github.com/brooke-gill/pit/blob/307c126be78a5615b437205966dba13cbab3b787/xp2level.html#L93
 
 def total_xp_req_for_pres(prestige: int) -> int:
     """Returns the amount of total xp that must be earned before the specified prestige."""
     return 0 if prestige == 0 else PRESTIGE_XP[prestige-1]
 
-def total_xp_reqs_for_levels(prestige: int) -> List[int]:
+def total_xp_reqs_for_levels(prestige: int) -> list[int]:
     """Returns a list of size 120, containing the total xp to reach levels 1-120 of the specified prestige."""
     levels_xp_reqs = [total_xp_req_for_pres(prestige)] # this first element will be removed at the end of the function.
     for level in range(1, 121):
         prev_level_group_index = math.floor((level-1) / 10)
         additional_xp_needed_for_level = math.ceil(
             LVL_GROUP_MULTIPLIER[prev_level_group_index] * PRESTIGE_MULTIPLIER[prestige] / 100)
         levels_xp_reqs.append(additional_xp_needed_for_level + levels_xp_reqs[-1])
     if prestige == 0:
         levels_xp_reqs[1] = 0 # Workaround hypixel does for making 0 xp players be 0-1 and not 0-0.
     assert len(levels_xp_reqs) == 121
     return levels_xp_reqs[1:]
 
-def xp_percent_levels() -> List[float]:
+def xp_percent_levels() -> list[float]:
     """Returns a list of size 120, containing the percent through a prestige (in terms of xp)
        to reach a certain level."""
     pres = 1 # Any greater prestige works as well.
     xp_for_lvls = [xp - PRESTIGE_XP[pres-1] for xp in total_xp_reqs_for_levels(pres)]
     return [d * 100 for d in Utils.normalize_against_max_val(xp_for_lvls)]
 
 def get_xp_req_for_rank(pit_rank: str) -> int:
     """pit_rank should be of the form: *roman number/decimal number* *-* *decimal number from 1 to 120*
     Will return an int representing the total xp needed to reach it."""
     pres, lvl = Utils.get_prestige_from_pit_rank(pit_rank), Utils.get_level_from_pit_rank(pit_rank)
     return total_xp_reqs_for_levels(pres)[lvl-1]
 
 class PitStats:
-    def __init__(self, pit_xp: int, playtime_kills_deaths: Optional[Tuple[int,int,int]] = None):
+    def __init__(self, pit_xp: int, playtime_kills_deaths: Optional[tuple[int,int,int]] = None):
         """note: playtime measured in mins"""
         assert pit_xp >= 0
         self._pit_xp = pit_xp
         self._playtime_kills_deaths = playtime_kills_deaths
         """First elem stores the total pit playtime in mins, second elem is total #kills, third is total #deaths."""
         self._prestige = next(i for i, xp_req in enumerate(PRESTIGE_XP) if xp_req >= self._pit_xp)
```

### Comparing `hypickle-1.1.4/hypickle/Player.py` & `hypickle-1.1.5/hypickle/Player.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Optional, List, Union, Dict
+from typing import Optional, Union
 from copy import deepcopy
 from datetime import datetime
 import time
 
 from . import Utils
 from . import hypixel
 from .MyClasses import UUID_Plus_Time, Specs
@@ -33,27 +33,27 @@
                                   for d in dict_for_player.get('friends', [])
                               ],
                       specs=specs
                      )
 
     def __init__(self, uuid: str, time_friended_parent_player: Union[str, float, int, None] = None,
                  hypixel_object: Optional[hypixel.Player] = None, name: Optional[str] = None,
-                 friends: Union[List[UUID_Plus_Time], List[Player], None] = None, specs: Optional[Specs] = None,
+                 friends: Union[list[UUID_Plus_Time], list[Player], None] = None, specs: Optional[Specs] = None,
                  name_for_file_output: Optional[str] = None, will_exclude_friends: bool = False,
                  date_cutoff_for_friends: Optional[str] = None, will_intersect: bool = False,
-                 players_used_to_combine: Optional[List[Player]] = None):
+                 players_used_to_combine: Optional[list[Player]] = None):
         self._uuid_plus_time = UUID_Plus_Time(uuid, time_friended_parent_player)
         self._hypixel_object = hypixel_object
         self._name = name
         self._specs = deepcopy(specs)
         self._name_for_file_output = name_for_file_output
         self._will_exclude_friends = will_exclude_friends
         self._will_intersect = will_intersect
         self._date_cutoff_for_friends = date_cutoff_for_friends
-        self._friends: Optional[List[Player]] = None
+        self._friends: Optional[list[Player]] = None
         self._call_api_if_friends_empty_in_friends_getter: bool = True
         self._pit_stats: Optional[PitStats] = None
         self._players_used_to_combine = players_used_to_combine
         if friends is not None:
             self._set_friends(friends)
 
     def hypixel_object(self) -> hypixel.Player:
@@ -71,15 +71,15 @@
 
     def player_JSON(self) -> dict:
         return self.hypixel_object().JSON
 
     def uuid(self) -> str:
         return self._uuid_plus_time.uuid()
 
-    def time_friended_parent_player(self, date_format: str) -> Union[str, float, int, None]:
+    def time_friended_parent_player(self, date_format: str) -> str | float | int | None:
         """`date_format` must be 'date' or 's'
         Function will return the time the player friended the parent player.
         If there is no parent player (e.g., if player is the root player), None is returned."""
         assert date_format in ('date', 's')
         if date_format == 'date':
             return self._uuid_plus_time.date_string()
         return self._uuid_plus_time.time_epoch_in_seconds()
@@ -92,15 +92,15 @@
     def name_for_file_output(self) -> str:
         assert self._name_for_file_output is not None
         return self._name_for_file_output
 
     def set_name_for_file_output(self, name: str) -> None:
         self._name_for_file_output = name
 
-    def friends(self) -> List[Player]:
+    def friends(self) -> list[Player]:
         if not self._friends and self._call_api_if_friends_empty_in_friends_getter:
             self._set_friends(self.hypixel_object().getFriends())
         return self._friends if self._friends is not None else []
 
     def specs(self) -> Specs:
         assert self._specs is not None
         return deepcopy(self._specs)
@@ -134,18 +134,18 @@
 
     def percent_way_to_next_network_level(self) -> float:
         return leveling.getPercentageToNextLevel(self.get_network_xp())
 
     def percent_way_overall_to_given_network_level(self, target_level: int) -> float:
         return self.get_network_xp() / leveling.getTotalExpToLevelFloor(target_level)
 
-    def recent_games(self) -> List[Dict]:
+    def recent_games(self) -> list[dict]:
         return self.hypixel_object().getRecentGames()
 
-    def specs_for_friends(self) -> Optional[Specs]:
+    def specs_for_friends(self) -> Specs | None:
         return self.specs().specs_for_friends()
 
     def represents_same_person(self, other: Player) -> bool:
         return self.uuid() == other.uuid()
 
     def set_specs(self, specs: Specs) -> None:
         self._specs = specs
@@ -153,22 +153,22 @@
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Player):
             raise ValueError("'other' is not an instance of Player.")
         return (len(self.friends()) == len(other.friends()) and self.name() == other.name() and
                 self._specs == other._specs and self.uuid() == other.uuid() and
                 self.time_friended_parent_player('date') == other.time_friended_parent_player('date'))
 
-    def set_date_cutoff_for_friends(self, date_cutoff: Optional[str]) -> None:
+    def set_date_cutoff_for_friends(self, date_cutoff: str | None) -> None:
         """Sets self._date_cutoff_for_friends to the param, and then applies it to the friends list"""
         if date_cutoff:
             assert not self.will_exclude_friends()
         self._date_cutoff_for_friends = date_cutoff
         self.remove_friends_added_before_cutoff()
 
-    def date_cutoff_for_friends(self) -> Optional[str]:
+    def date_cutoff_for_friends(self) -> str | None:
         return self._date_cutoff_for_friends
 
     def remove_friends_added_before_cutoff(self) -> None:
         assert not self.will_exclude_friends()
         if not self._date_cutoff_for_friends or not self._friends:
             return
         self._friends = [f for f in self._friends if not
@@ -187,15 +187,15 @@
         if first_n is not None:
             assert 0 <= first_n <= len(self.friends())
             self._set_friends(self.friends()[:first_n])
         elif last_n is not None:
             assert 0 <= last_n <= len(self.friends())
             self._set_friends(self.friends()[-last_n:] if last_n > 0 else []) # type: ignore
 
-    def _set_friends(self, friends: Union[List[UUID_Plus_Time], List[Player], None]) -> None:
+    def _set_friends(self, friends: list[UUID_Plus_Time] | list[Player] | None) -> None:
         """Note that after this function has been called, if self.friends() is called later and
         self._friends happens to be None or [], the hypixel api won't be called to populate self._friends.
         The reasoning for this is that since self._set_friends() is being called now, it's assumed the
         caller wants self._friends to be equal to a certain value -- and None or [] are valid values
         if that's what the caller wants."""
 
         self._call_api_if_friends_empty_in_friends_getter = False
@@ -229,24 +229,24 @@
         """Returns whether this player's friends will be intersected with the friends (or exclude friends)
            list leading up to it in combine_players."""
         return self._will_intersect
 
     def set_will_intersect(self, will_intersect: bool) -> None:
         self._will_intersect = will_intersect
 
-    def in_player_list(self, players: List[Player]) -> bool:
+    def in_player_list(self, players: list[Player]) -> bool:
         """Returns whether the player is already represented in this players list."""
         return any(self.represents_same_person(p) for p in players)
 
     def get_stats_dict(self) -> dict:
         """Returns a dict with key-val pairs for uuid, name, fkdr, star, and pit_rank."""
         return {'uuid': self.uuid(), 'name': self.name(), 'fkdr': self.get_fkdr(),
                 'star': self.get_bw_star(), 'pit_rank': self.pit_rank_string()}
 
-    def print_dict_report(self, report: Dict, extra_text: str = '') -> None:
+    def print_dict_report(self, report: dict, extra_text: str = '') -> None:
         report = deepcopy(report)
         assert all(isinstance(v, (str,float,int)) for v in report.values())
         possible_keys = ('name', 'fkdr', 'star', 'pit_rank', 'uuid', 'time')
         assert {'uuid'} <= set(report.keys()) <= set(possible_keys)
         name, fkdr, star, pit_rank, uuid, time_friended = [report.get(k) for k in possible_keys]
         assert isinstance(uuid, str) # for mypy
         rank = None if (just_uuids := self.specs().just_uuids()) else self.network_rank()
@@ -406,23 +406,23 @@
 
     @staticmethod
     def _sort_func(d: dict, sort_key: str) -> int:
         if sort_key == "pit_rank":
             return Utils.pit_rank_to_num_for_sort(d.get("pit_rank", "0-1"))
         return d.get(sort_key, 0)
 
-    def polish_friends_list(self, friends_to_exclude: Union[List[Player], Dict[str, Player]]) -> None:
+    def polish_friends_list(self, friends_to_exclude: list[Player] | dict[str, Player]) -> None:
         """Will sort friends, remove duplicates, and remove any who appear in the friends_to_exclude param.
         Note that a Player object is treated as an equivalent/duplicate player if it has the same uuid as
         another Player. Other details (such as time friended parent player) can differ."""
         assert self._friends is not None
         self.remove_friends_added_before_cutoff() # Probably redundant
         self._set_friends(sorted(self.friends(), key=lambda f: f.time_friended_parent_player('s') or 0, reverse=True))
         self.remove_duplicate_friends()
-        if isinstance(friends_to_exclude, List):
+        if isinstance(friends_to_exclude, list):
             self._set_friends([f for f in self.friends() if not f.in_player_list(friends_to_exclude)])
         elif isinstance(friends_to_exclude, dict):
             self._set_friends([f for f in self.friends() if not f.uuid() in friends_to_exclude])
         else:
             raise ValueError("friends_to_exclude must be a list or dict of Players")
 
     def diff_f_lists(self, other: Player, list_friends: bool) -> None:
```

### Comparing `hypickle-1.1.4/hypickle/ProcessingResults.py` & `hypickle-1.1.5/hypickle/ProcessingResults.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,70 @@
 """Contains functions for dealing with reading from the results folder."""
 
+from __future__ import annotations
 import os
 from pathlib import Path
-from typing import Optional, List, Dict
+from typing import Optional
 from copy import deepcopy
 
 from . import Utils
 from . import Files
 from .MyClasses import UUID_Plus_Time
 from . import hypixel
 from .MyClasses import args
 
-_all_dicts_standard_files: Optional[List[dict]] = None
-_all_dicts_additional_friends_files: Optional[List[dict]] = None
-_all_dicts_unique_uuids: Optional[List[dict]] = None
-_ign_uuid_pairs_in_results: Optional[Dict[str, str]] = None
-_uuid_ign_pairs_in_results: Optional[Dict[str, str]] = None
+_all_dicts_standard_files: Optional[list[dict]] = None
+_all_dicts_additional_friends_files: Optional[list[dict]] = None
+_all_dicts_unique_uuids: Optional[list[dict]] = None
+_ign_uuid_pairs_in_results: Optional[dict[str, str]] = None
+_uuid_ign_pairs_in_results: Optional[dict[str, str]] = None
 
 _NON_TRIVIAL_KEYS = ('friends', 'name', 'fkdr', 'star', 'pit_rank')
 
-def ign_uuid_pairs_in_results(get_deepcopy: bool = False) -> Dict[str, str]:
+def ign_uuid_pairs_in_results(get_deepcopy: bool = False) -> dict[str, str]:
     global _ign_uuid_pairs_in_results
 
     if not _ign_uuid_pairs_in_results:
         _ign_uuid_pairs_in_results = {}
         for d in (get_all_dicts_in_results(False, True) + get_all_dicts_in_results(False, False)):
             _ign_uuid_pairs_in_results.update(Utils.get_all_ign_uuid_pairs_in_dict(d))
     return deepcopy(_ign_uuid_pairs_in_results) if get_deepcopy else _ign_uuid_pairs_in_results
 
-def uuid_ign_pairs_in_results(get_deepcopy: bool = False) -> Dict[str, str]:
+def uuid_ign_pairs_in_results(get_deepcopy: bool = False) -> dict[str, str]:
     global _uuid_ign_pairs_in_results
 
     if not _uuid_ign_pairs_in_results:
         _uuid_ign_pairs_in_results = {}
         for d in (get_all_dicts_in_results(False, True) + get_all_dicts_in_results(False, False)):
             _uuid_ign_pairs_in_results.update(Utils.get_all_ign_uuid_pairs_in_dict(d, False, True))
     return deepcopy(_uuid_ign_pairs_in_results) if get_deepcopy else _uuid_ign_pairs_in_results
 
-def check_results(uuid: Optional[str], ign: Optional[str]) -> None:
+def check_results(uuid: str | None, ign: str | None) -> None:
     """Traverses through the results folder and prints some stats and info. If a uuid and ign are provided,
        then some specific info about that player will be outputted as well. Note that whether multiplayer
        files are included depends on the cli args."""
     assert type(uuid) is type(ign)
 
     print(f"\n\n{len(_get_all_unique_uuids_in_results())} total unique uuids recorded in the results folder.")
-    all_dicts: List[dict] = get_all_dicts_unique_uuids_in_results()
+    all_dicts: list[dict] = get_all_dicts_unique_uuids_in_results()
     print(f"{len(all_dicts)} total players with non-trivial data stored in the results folder (excluding additional friends files).")
 
     for k in _NON_TRIVIAL_KEYS:
         dicts_with_key = [d for d in all_dicts if k in d]
         indent = "  "
         Utils.print_info_for_key(dicts_with_key, k, indent)
         if k != 'friends':
             continue
         if uuid and ign:
             friends_in_results = uuid in (d['uuid'] for d in dicts_with_key)
             print(f"{indent*2}Also, it's {str(friends_in_results).lower()} that " +
                   f"{ign}'s friends list in in the results folder.")
     print('\n\n')
 
-def get_all_dicts_in_results(get_deepcopy: bool = False, get_additional_friends: bool = False) -> List[dict]:
+def get_all_dicts_in_results(get_deepcopy: bool = False, get_additional_friends: bool = False) -> list[dict]:
     """Returns a flat list of non-trivial dicts, for all dicts/nested dicts found in the results folder.
        Note that there can be multiple dicts with the same uuid."""
     global _all_dicts_standard_files, _all_dicts_additional_friends_files
 
     all_dicts = _all_dicts_additional_friends_files if get_additional_friends else _all_dicts_standard_files
     if not all_dicts:
         all_dicts = []
@@ -74,51 +75,51 @@
         if get_additional_friends:
             _all_dicts_additional_friends_files = all_dicts
         else:
             _all_dicts_standard_files = all_dicts
     return deepcopy(all_dicts) if get_deepcopy else all_dicts
 
 def get_all_dicts_unique_uuids_in_results(get_deepcopy: bool = False,
-                                          must_have_times_friended: bool = False) -> List[dict]:
+                                          must_have_times_friended: bool = False) -> list[dict]:
     """Returns a flat list of non-trivial dicts (no more than one per uuid), for all dicts/nested dicts found in the
     results folder (excluding additional friends files). If multiple dicts have the same uuid, the one with
     the biggest friends list will be kept."""
     global _all_dicts_unique_uuids
 
     if not _all_dicts_unique_uuids:
         _all_dicts_unique_uuids = Utils.remove_dicts_duplicate_uuids(
             get_all_dicts_in_results(),
             must_have_times_friended=must_have_times_friended
         )
 
     return deepcopy(_all_dicts_unique_uuids) if get_deepcopy else _all_dicts_unique_uuids
 
 def get_best_f_list_for_player_in_results(uuid_or_ign: str,
-                                          must_have_times_friended: bool = False) -> List[UUID_Plus_Time]:
+                                          must_have_times_friended: bool = False) -> list[UUID_Plus_Time]:
     uuid = hypixel.get_uuid(uuid_or_ign)
     for d in get_all_dicts_unique_uuids_in_results(must_have_times_friended=must_have_times_friended):
         if d['uuid'] == uuid:
             # print(d['filename']) For debugging - will show you the filename the dict came from.
             return [UUID_Plus_Time(f['uuid'], f.get('time')) for f in d.get('friends', [])]
     return []
 
-def update_list_if_applicable(lst: List[UUID_Plus_Time], new_elem: UUID_Plus_Time) -> None:
+def update_list_if_applicable(lst: list[UUID_Plus_Time], new_elem: UUID_Plus_Time) -> None:
     """If no element in lst refers to the same person as elem, then elem will be appended at the end.
        Otherwise, elem will replace its duplicate, if it is more recent than it.
        The reference to the list itself will be modified by this function."""
     for i, element in enumerate(lst):
         if new_elem.refers_to_same_person(element):
             if new_elem.more_recent(element):
                 lst[i] = new_elem
             return
     lst.append(new_elem)
 
-def get_all_additional_friends_for_player(uuid_or_ign: str) -> List[UUID_Plus_Time]:
+def get_all_additional_friends_for_player(uuid_or_ign: str) -> list[UUID_Plus_Time]:
     uuid = hypixel.get_uuid(uuid_or_ign)
-    additional_friends: List[UUID_Plus_Time] = []
+    additional_friends: list[UUID_Plus_Time] = []
     for d in get_all_dicts_in_results(get_additional_friends=True):
         if d['uuid'] != uuid:
             continue
         for f in d.get('friends', []):
             current_friend = UUID_Plus_Time(f['uuid'], f.get('time'))
             update_list_if_applicable(additional_friends, current_friend)
     return additional_friends
@@ -135,19 +136,19 @@
     hits = []
     for d in get_all_dicts_in_results():
         if 'name' in d and d[param_key].lower() == uuid_or_ign.lower() and d[search_for] not in hits:
             print(d[search_for])
             hits.append(d[search_for])
     print()
 
-def _get_all_jsons_in_results(get_additional_friends: bool = False) -> List[dict]:
+def _get_all_jsons_in_results(get_additional_friends: bool = False) -> list[dict]:
     """Returns a list of dicts, where each dict represents the json each textfile stores."""
     if not os.path.isdir('results'):
         return []
-    all_jsons: List[dict] = []
+    all_jsons: list[dict] = []
     all_paths = sorted(Path('results').iterdir(), key=os.path.getmtime, reverse=True)
     all_files = [f.name for f in all_paths if _does_filename_meet_reqs(f.name, get_additional_friends)]
     for f in all_files:
         filename = os.path.join('results', f)
         is_multi_player_file = any(x in f for x in [' plus ', ' minus ', ' intersect '])
         if is_multi_player_file and not args().include_multi_player_files():
             continue
@@ -159,16 +160,16 @@
         all_jsons.append(json_in_file)
     return all_jsons
 
 def _does_filename_meet_reqs(f: str, for_additional_friends: bool = False) -> bool:
     required_start = 'Additional friends of' if for_additional_friends else 'Friends of'
     return f.startswith(required_start) and f.endswith('.txt')
 
-def _get_only_non_trivial_keys_in_dict(dicts: List[dict]) -> List[dict]:
+def _get_only_non_trivial_keys_in_dict(dicts: list[dict]) -> list[dict]:
     return [d for d in dicts if any(k in d for k in _NON_TRIVIAL_KEYS)]
 
-def _get_all_unique_uuids_in_results() -> List[str]:
+def _get_all_unique_uuids_in_results() -> list[str]:
     """Returns all uuids written at some point in the results folder - most will be friends of friends."""
     all_dicts = []
     for d in (get_all_dicts_in_results(False, True) + get_all_dicts_in_results(False, False)):
         all_dicts.extend(Utils.get_all_nested_dicts_in_dict(d))
     return Utils.remove_duplicates([d['uuid'] for d in all_dicts])
```

### Comparing `hypickle-1.1.4/hypickle/Rank.py` & `hypickle-1.1.5/hypickle/Rank.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from typing import Optional, Dict, Tuple
+from __future__ import annotations
 from dataclasses import dataclass
 from copy import deepcopy
 
 from .Colours import Hex, ColourSpecs, colour_print
 
 @dataclass
 class RankColours:
-    plus_colour: Optional[Hex]
+    plus_colour: Hex | None
     """Represents the colour of any '+' chars that may be present in the rank."""
-    player_name_brackets_colour: Optional[Hex]
+    player_name_brackets_colour: Hex | None
     """Represents the colour of the rank brackets and the player's name."""
-    rank_colour: Optional[Hex]
+    rank_colour: Hex | None
     """Represents the colour of the rank, excluding any potential '+' chars."""
 
 class RankMap:
-    _rank_map: Dict[Optional[str], Tuple[str, RankColours]] = {
+    _rank_map: dict[str | None, tuple[str, RankColours]] = {
         '§c[OWNER]': ('OWNER', RankColours(None, Hex.RED, Hex.RED)),
         'ADMIN': ('ADMIN', RankColours(None, Hex.RED, Hex.RED)),
         'GAME_MASTER': ('GM', RankColours(None, Hex.DARK_GREEN, Hex.DARK_GREEN)),
         'YOUTUBER': ('YOUTUBE', RankColours(None, Hex.RED, Hex.WHITE)),
         'VIP': ('VIP', RankColours(None, Hex.GREEN, Hex.GREEN)),
         'VIP_PLUS': ('VIP+', RankColours(Hex.GOLD, Hex.GREEN, Hex.GREEN)),
         'MVP': ('MVP', RankColours(None, Hex.AQUA, Hex.AQUA)),
         'MVP_PLUS': ('MVP+', RankColours(Hex.UNKNOWN, Hex.AQUA, Hex.AQUA)),
         'SUPERSTAR': ('MVP++', RankColours(Hex.UNKNOWN, Hex.UNKNOWN, Hex.UNKNOWN)),
         None: ('', RankColours(None, None, None))
     }
     @classmethod
-    def json_rank_info(cls, key: Optional[str]) -> Tuple[str, RankColours]:
+    def json_rank_info(cls, key: str | None) -> tuple[str, RankColours]:
         """Returns the display string for a rank (without the brackets), as well as a RankColours
            object detailing the colours to print in."""
         return deepcopy(cls._rank_map[key])
 
 class Rank:
     def __init__(self, json: dict) -> None:
         keys = ('prefix', 'rank', 'monthlyPackageRank', 'newPackageRank', 'packageRank')
@@ -44,31 +44,31 @@
 
     def rank(self, with_brackets_and_space: bool) -> str:
         """Returns the rank that's displayed ('VIP', 'MVP+', '', etc)"""
         if not with_brackets_and_space or self._display_rank == '':
             return self._display_rank
         return f"[{self._display_rank}] "
 
-    def rank_colour(self) -> Optional[Hex]:
+    def rank_colour(self) -> Hex | None:
         if self._colours.rank_colour == Hex.UNKNOWN:
             assert self._display_rank == 'MVP++'
             self._colours.rank_colour = (
                 Hex.AQUA if self._json.get('monthlyRankColor') == 'AQUA' else Hex.GOLD
             )
         return self._colours.rank_colour
 
-    def plus_colour(self) -> Optional[Hex]:
+    def plus_colour(self) -> Hex | None:
         if self._colours.plus_colour == Hex.UNKNOWN:
             assert self._display_rank in ('MVP+', 'MVP++')
             json_plus_colour = self._json.get('rankPlusColor')
             self._colours.plus_colour = (Hex.RED if json_plus_colour is None else
                                          next(c for c in Hex if json_plus_colour == c.name))
         return self._colours.plus_colour
 
-    def name_and_bracket_colour(self) -> Optional[Hex]:
+    def name_and_bracket_colour(self) -> Hex | None:
         if self._colours.player_name_brackets_colour == Hex.UNKNOWN:
             self._colours.player_name_brackets_colour = self.rank_colour()
         return self._colours.player_name_brackets_colour
 
     def print_rank(self) -> None:
         rank = self.rank(False)
         bracket_colour = self.name_and_bracket_colour()
```

### Comparing `hypickle-1.1.4/hypickle/Utils.py` & `hypickle-1.1.5/hypickle/Utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 """Functions in this file are the most general, and don't have dependencies on other files in the project."""
 
+from __future__ import annotations
 from datetime import datetime
 import time
-from typing import List, Optional, Union, Iterable, Any, Type
+from typing import Optional, Iterable, Any, Type
 from collections import OrderedDict
 from copy import deepcopy
 import math
 from pprint import pprint
 
-def list_subtract(main_list: List, subtract_elems: Iterable) -> List:
+def list_subtract(main_list: list, subtract_elems: Iterable) -> list:
     subtract_set = set(subtract_elems)
     return [x for x in main_list if x not in subtract_set]
 
-def remove_duplicates(lst: List) -> List:
+def remove_duplicates(lst: list) -> list:
     return list(OrderedDict.fromkeys(deepcopy(lst))) # regular dict works to maintain order for python >= 3.7
 
 def is_date_string(text: str) -> bool:
     try:
         datetime.strptime(text, '%Y-%m-%d')
     except ValueError:
         return False
     return True
 
-def print_list(lst: List, prepended_msg: str = "", separator: str = " ", appended_msg: str = "\n\n") -> None:
+def print_list(lst: list, prepended_msg: str = "", separator: str = " ", appended_msg: str = "\n\n") -> None:
     print(prepended_msg, end="")
     print(separator.join([str(x) for x in lst]), end=appended_msg)
 
 def trim_if_needed(text: str, limit: int = 200) -> str:
     if len(text) <= limit:
         return text
     side_lengths = int((limit - 5) / 2)
     return text[:side_lengths].strip() + ' ..... ' + text[-side_lengths:].strip()
 
-def remove_date_strings(lst: List[str]) -> List[str]:
+def remove_date_strings(lst: list[str]) -> list[str]:
     return [x for x in lst if not is_date_string(x)]
 
-def get_date_string_if_exists(lst: List[str]) -> Optional[str]:
+def get_date_string_if_exists(lst: list[str]) -> str | None:
     """If no date strings found, return None."""
     return next((x for x in lst if is_date_string(x)), None)
 
 def kdr_division(kills: int, deaths: int) -> float:
     return kills / deaths if deaths else float(kills)
 
 def date_to_epoch(date_string: str, in_seconds: bool) -> float:
     epoch = time.mktime(datetime.strptime(date_string, '%Y-%m-%d').timetuple())
     return epoch * 1000 if not in_seconds else epoch
 
 def epoch_to_date(epoch: float, epoch_in_seconds: bool) -> str:
     return datetime.fromtimestamp(epoch / 1000 if not epoch_in_seconds else epoch).strftime('%Y-%m-%d')
 
 def find_dict_for_given_player(d: dict, uuid_or_ign: str, make_deep_copy: bool = True,
-                               dict_must_have_friends_list: bool = True) -> Optional[dict]:
+                               dict_must_have_friends_list: bool = True) -> dict | None:
     """ d will be a dictionary read from a file in json format - it will have a uuid key, and possibly
     a name, fkdr, and friends key. The friends key would have a value that is a list of dictionaries,
     recursively following the same dictionary requirements."""
     if make_deep_copy:
         d = deepcopy(d)
     if ((is_uuid(uuid_or_ign) and d['uuid'] == uuid_or_ign) or
         (is_ign(uuid_or_ign) and 'name' in d and d['name'].lower() == uuid_or_ign.lower())):
@@ -91,65 +92,65 @@
             ign_uuid_pairs[d['uuid']] = name_lower
         else:
             ign_uuid_pairs[name_lower] = d['uuid']
     for friend_dict in d.get('friends', []):
         ign_uuid_pairs.update(get_all_ign_uuid_pairs_in_dict(friend_dict, False, get_uuid_ign_pairs_instead))
     return ign_uuid_pairs
 
-def get_all_nested_dicts_in_dict(d: dict, make_deepcopy: bool = False) -> List[dict]:
+def get_all_nested_dicts_in_dict(d: dict, make_deepcopy: bool = False) -> list[dict]:
     """Traverses through d and returns a list of d and all its nested friend dicts."""
     if make_deepcopy:
         d = deepcopy(d)
     dicts = [d] if 'exclude' not in d else []
     for friend_dict in d.get('friends', []):
         friend_dict['filename'] = d['filename']
         dicts.extend(get_all_nested_dicts_in_dict(friend_dict, make_deepcopy=False))
     return dicts
 
-def print_info_for_key(dicts: List[dict], k: str, indent: str) -> None:
+def print_info_for_key(dicts: list[dict], k: str, indent: str) -> None:
     k_for_print = k + ('s' if k == 'star' else '')
     print(f"{indent}{len(dicts)} players with their {k_for_print} recorded in results.")
     if k in ('star', 'fkdr', 'friends'):
         highest_dict = max(dicts, key=lambda d: len(d[k]) if k == 'friends' else d[k])
         highest_stat = len(highest_dict[k]) if k == 'friends' else highest_dict[k]
         name = f"{highest_dict['name']}, " if 'name' in highest_dict else ''
         print(f"{indent*2}Most {k_for_print}: {highest_stat} ({name}uuid {highest_dict['uuid']})")
 
-def does_first_have_more_friends(first: list, second: list) -> Optional[bool]:
+def does_first_have_more_friends(first: list, second: list) -> bool | None:
     """True returned if more, False returned if less, None returned if equal."""
     return True if len(first) > len(second) else (False if len(second) > len(first) else None)
 
-def does_first_record_times_better(first: list, second: list) -> Optional[bool]:
+def does_first_record_times_better(first: list, second: list) -> bool | None:
     """True returned if better, False returned if worse, None returned if equal."""
     first_has_times = len(first) > 0 and 'time' in first[0]
     second_has_times = len(second) > 0 and 'time' in second[0]
     return None if (first_has_times == second_has_times) else first_has_times
 
-def does_first_have_more_keys(first: dict, second: dict) -> Optional[bool]:
+def does_first_have_more_keys(first: dict, second: dict) -> bool | None:
     """True returned if more, False returned if less, None returned if equal."""
     return None if len(first.keys()) == len(second.keys()) else len(first.keys()) > len(second.keys())
 
 def is_first_dict_more_valuable(first: dict, second: dict, must_have_times_friended: bool) -> bool:
     """Returns true if the second dict should be replaced with the first dict, based off
        some criteria. This function is called by the 'remove_dicts_duplicate_uuids' function."""
     assert first['uuid'] == second['uuid']
     first_friends, second_friends = first.get('friends', []), second.get('friends', [])
 
-    comparisons: List[Optional[bool]] = [
+    comparisons: list[bool | None] = [
         does_first_have_more_friends(first_friends, second_friends),
         does_first_record_times_better(first_friends, second_friends),
         does_first_have_more_keys(first, second)
     ]
     if must_have_times_friended:
         comparisons[0], comparisons[1] = comparisons[1], comparisons[0]
 
     return next((b for b in comparisons if b is not None), False)
 
-def remove_dicts_duplicate_uuids(dicts: List[dict], make_deepcopy: bool = False,
-                                 must_have_times_friended: bool = False) -> List[dict]:
+def remove_dicts_duplicate_uuids(dicts: list[dict], make_deepcopy: bool = False,
+                                 must_have_times_friended: bool = False) -> list[dict]:
     """ For dicts with the same uuid, only one dict will be kept in the new list. The criteria
         for choosing which one are as follows (in order):
         - bigger friends list
         - records time added for friends
         - more keys in dict
         - The dict that came first in the `dicts` param
         Note that 1) and 2) are swapped, if the `must_have_times_friended` param is set to True. """
@@ -159,43 +160,43 @@
     for d in dicts:
         uuid = d['uuid']
         if (uuid not in dicts_unique_uuids or is_first_dict_more_valuable(d, dicts_unique_uuids[uuid],
         must_have_times_friended)):
             dicts_unique_uuids[uuid] = d
     return list(dicts_unique_uuids.values())
 
-def is_in_milliseconds(epoch_val: Union[float, int]) -> bool:
+def is_in_milliseconds(epoch_val: float | int) -> bool:
     """epoch_val is assumed to be in either seconds or milliseconds"""
     return epoch_val > 10_000_000_000
 
-def convert_to_seconds(time_val: Union[float, int, str, None]) -> float:
+def convert_to_seconds(time_val: float | int | str | None) -> float:
     """ Converts a datestring or epoch to epoch in seconds. If time_val is already an epoch, it must be
         in seconds or milliseconds form. """
     if time_val is None:
         return 0
     elif isinstance(time_val, str):
         assert is_date_string(time_val)
         return date_to_epoch(time_val, True)
     elif is_in_milliseconds(time_val):
         return time_val / 1000
     else:
         return time_val
 
-def is_older(time_one: Union[str, float, int, None], time_two: Union[str, float, int, None]) -> bool:
+def is_older(time_one: str | float | int | None, time_two: str | float | int | None) -> bool:
     """Returns true if time_one is more recent than time_two. time_one and time_two must each be either
        a datestring or epoch (in seconds/milliseconds)."""
     return convert_to_seconds(time_one) < convert_to_seconds(time_two)
 
 def get_current_date() -> str:
     return datetime.now().strftime('%Y-%m-%d')
 
-def replace_in_list(lst: List[str], elem_to_remove: str, list_to_insert: List[str]) -> List[str]:
+def replace_in_list(lst: list[str], elem_to_remove: str, list_to_insert: list[str]) -> list[str]:
     """Returns a new list, where any occurrences of `elem_to_remove` (case-insensitive) in `lst` are
        replaced with the elements in `list_to_insert`. `lst` will not be modified."""
-    replacement: List[str] = []
+    replacement: list[str] = []
     for s in lst:
         if s.lower() == elem_to_remove.lower():
             replacement.extend(list_to_insert)
         else:
             replacement.append(s)
     return replacement
 
@@ -248,15 +249,15 @@
 def round_up_to_closest_multiple(num: float, multiple_of: int) -> int:
     """E.g., calling with args (101, 50) would return 150."""
     return math.ceil(num / multiple_of) * multiple_of
 
 def percentify(d: float, decimal_places_to_round_to: int = 2) -> str:
     return f"{round(100*d, decimal_places_to_round_to)}%"
 
-def normalize_against_max_val(l: Iterable[float]) -> List[float]:
+def normalize_against_max_val(l: Iterable[float]) -> list[float]:
     max_val = max(l)
     return [i / max_val for i in l]
 
 def nested_get(d: dict, nested_keys: Iterable, default_val: Any, expected_type: Optional[Type] = None) -> Any:
     try:
         for k in nested_keys:
             d = d[k]
```

### Comparing `hypickle-1.1.4/hypickle/additional_friends.py` & `hypickle-1.1.5/hypickle/additional_friends.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import List
+from __future__ import annotations
 
 from . import Utils
 from . import hypixel
 from .MyClasses import Specs
 from . import Files
 from .Player import Player
 
-def get_friends_from_user(friends_specs: Specs) -> List[Player]:
-    friends: List[Player] = []
+def get_friends_from_user(friends_specs: Specs) -> list[Player]:
+    friends: list[Player] = []
     INPUT_MSG = "Enter the igns/uuids of new friends to add, separated by spaces (or enter 'done' to stop): "
     for i, user_input in enumerate(inputs := Files.apply_aliases(input(INPUT_MSG).split())):
         if user_input.lower() in ('done', 'stop'):
             assert i == len(inputs)-1
             return friends
         friends.append(Player(hypixel.get_uuid(user_input), specs=friends_specs,
                               time_friended_parent_player=Utils.get_current_date()))
```

### Comparing `hypickle-1.1.4/hypickle/bedwars.py` & `hypickle-1.1.5/hypickle/bedwars.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Based off https://github.com/Plancke/hypixel-php/blob/master/src/util/games/bedwars/ExpCalculator.php
 
+from __future__ import annotations
 from math import floor
 
 LEVELS_PER_PRESTIGE = 100
 XP_PER_EASY_LEVEL = (500, 1000, 2000, 3500)
 XP_PER_LEVEL = 5000
 NUM_EASY_LEVELS = len(XP_PER_EASY_LEVEL)
 XP_PER_PRESTIGE = sum(XP_PER_EASY_LEVEL) + XP_PER_LEVEL * (LEVELS_PER_PRESTIGE - NUM_EASY_LEVELS)
```

### Comparing `hypickle-1.1.4/hypickle/hypixel.py` & `hypickle-1.1.5/hypickle/hypixel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,32 @@
+from __future__ import annotations
+
 """ Simple Hypixel-API in Python, by Snuggle | 2017 to 2021 (https://github.com/Snuggle/hypixel.py/blob/main/hypixel.py)
     Modifications made by John (late 2022 to current) """
 __version__ = '0.8.0'
 # pylint: disable=C0103
 
 from random import choice
 from time import time, sleep
 from datetime import datetime, timedelta
-from typing import List, Optional, Tuple, Dict
+from typing import Optional
 import re
 import os.path
 import requests
 
 from .MyClasses import UUID_Plus_Time, args
 from . import Files
 from . import Utils
 from . import leveling
 from .Rank import Rank
 
 TIME_STARTED: float = time()
 num_api_calls_made: int = 0
 
-def make_request_url(typeOfRequest: str, uuid_or_ign: Optional[str]) -> str:
+def make_request_url(typeOfRequest: str, uuid_or_ign: str | None) -> str:
     assert (typeOfRequest == 'leaderboards') == (uuid_or_ign is None)
     requestURL = 'https://api.hypixel.net/' + typeOfRequest
     if uuid_or_ign is not None:
         if (query_param_name := 'uuid' if Utils.is_uuid(uuid_or_ign) else 'name') == 'name':
             assert typeOfRequest == 'player'
         requestURL += f"?{query_param_name}={uuid_or_ign}"
     return requestURL
@@ -112,15 +114,15 @@
 class HypixelAPIError(Exception):
     pass
 
 class Player:
     def __init__(self, uuid_or_ign: str) -> None:
         self.JSON = getJSON('player', get_uuid(uuid_or_ign, call_api_last_resort=False))
         self._rank = Rank(self.JSON)
-        self.updated_json: Optional[Tuple[dict, datetime]] = None
+        self.updated_json: Optional[tuple[dict, datetime]] = None
         """Stores the newest result of `getJSON('player')` that was updated from the previous call."""
         self.recent_games_visible: Optional[bool] = None
         """Recent games may not be visible if the player has turned off the api setting, or if they haven't
            played a game in roughly 3 days it seems."""
 
     def getName(self, extra_safety_check=True) -> str:
         """ Just return player's name. """
@@ -133,24 +135,24 @@
             + ". To disable this safety check, call this function with getName(extra_safety_check=False).")
         return sanitized_name
 
     def getUUID(self) -> str:
         """ This function returns a player's UUID. """
         return self.JSON['uuid']
 
-    def getFriends(self) -> List[UUID_Plus_Time]:
+    def getFriends(self) -> list[UUID_Plus_Time]:
         """ *Deprecated from Hypixel API*
             This function returns a list of the UUIDs of all the player's friends."""
         friends = []
         for friend in getJSON('friends', self.getUUID())['records']:
             friend_uuid = friend["uuidReceiver"] if friend["uuidReceiver"] != self.getUUID() else friend["uuidSender"]
             friends.append(UUID_Plus_Time(friend_uuid, friend['started']))
         return list(reversed(friends))
 
-    def isOnline(self, extra_online_checks: Tuple[bool, bool, bool]) -> bool:
+    def isOnline(self, extra_online_checks: tuple[bool, bool, bool]) -> bool:
         """ This function returns a bool representing whether the player is online.
             For `extra_online_checks`:
                 - The first bool is for players whose online status is shown. It determines whether to check
                   the current online statuses of players, irrespective of whether they were recorded as
                   online in the original self.JSON. So, this bool being true limits false negatives, at
                   the expense of more api calls.
                 - The second bool determines whether to call the api for the most recent json to see if
@@ -209,12 +211,12 @@
 
     def getExactNWLevel(self) -> float:
         return leveling.getExactLevel(self.getNetworkXP())
 
     def getNetworkRank(self) -> Rank:
         return self._rank
 
-    def getRecentGames(self) -> List[Dict]:
+    def getRecentGames(self) -> list[dict]:
         if self.recent_games_visible is False:
             return []
         self.recent_games_visible = bool(recent_games := getJSON('recentgames', self.getUUID())['games'])
         return recent_games
```

### Comparing `hypickle-1.1.4/hypickle/leveling.py` & `hypickle-1.1.5/hypickle/leveling.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # Based off https://github.com/Plancke/hypixel-php/blob/master/src/util/Leveling.php and
 # https://github.com/Snuggle/hypixel.py/blob/main/leveling.py
 
+from __future__ import annotations
 import math
-from typing import Optional, Callable, Tuple
+from typing import Optional, Callable
 
 class QuadraticFunc:
     def __init__(self, a: float, b: float, c: float,
                  req_for_x_vals: Optional[Callable[[float], bool]] = None,
                  req_for_y_vals: Optional[Callable[[float], bool]] = None):
         "Represents some function: y = ax^2 + bx + c"
         self.a, self.b, self.c = a, b, c
         self.req_for_x_vals, self.req_for_y_vals = req_for_x_vals, req_for_y_vals
 
     def y_val(self, x_val: float) -> float:
         if self.req_for_x_vals:
             assert self.req_for_x_vals(x_val)
         return self.a*x_val**2 + self.b*x_val + self.c
 
-    def x_vals(self, y_val: float) -> Tuple[float, float]:
+    def x_vals(self, y_val: float) -> tuple[float, float]:
         """Returns the roots of the equation when substituting `y_val` for y."""
         # Need to make a quadratic equation. Do this by substituting y_val for y,
         # then subtracting it from both sides. This just makes c become self.c - y.
         if self.req_for_y_vals:
             assert self.req_for_y_vals(y_val)
         a, b, c = self.a, self.b, self.c - y_val
         sqrt_exp = math.sqrt(b**2 - 4*a*c)
```

### Comparing `hypickle-1.1.4/hypickle/main.py` & `hypickle-1.1.5/hypickle/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from __future__ import annotations
 import sys
-from typing import List, Tuple, Optional
+from typing import Optional
 from itertools import permutations
 from copy import deepcopy
 
 from . import hypixel
 from . import MyClasses
 from .MyClasses import Specs, UUID_Plus_Time, args
 from . import Files
@@ -13,35 +14,35 @@
 from . import Utils
 from . import Pit
 from . import leveling
 from . import bedwars
 from . import Graphing
 from .Graphing import ScatterplotInfo
 
-def intersect_player_lists(l1: List[Player], l2: List[Player]) -> List[Player]:
+def intersect_player_lists(l1: list[Player], l2: list[Player]) -> list[Player]:
     return [p for p in l1 if p.in_player_list(l2)]
 
-def combine_players(info_on_players: List[Player]) -> Player:
+def combine_players(info_on_players: list[Player]) -> Player:
     """This function runs through the Player list and adds/subtracts/intersects f lists. Whether a Player's f list
     is used to add/subtract/intersect depends on the bool value of their player.will_exclude_friends()
     and player.will_intersect() functions.
     If a player's f list is used to intersect, it will intersect the entire friends list up to that point,
     either for playerFriends or exclude_friends.
     Order of operations:
         union, intersect (left to right for precedence amongst these)
         subtract
     """
     info_on_players = deepcopy(info_on_players)
     playerNameForFileOutput = info_on_players[0].name()
     playerUUID = info_on_players[0].uuid()
-    playerFriends: List[Player] = info_on_players[0].friends()
+    playerFriends: list[Player] = info_on_players[0].friends()
     playerSpecs = info_on_players[0].specs()
     date_cutoff_friends = info_on_players[0].date_cutoff_for_friends()
 
-    exclude_friends: List[Player] = []
+    exclude_friends: list[Player] = []
     for player in info_on_players[1:]:
         if player.will_exclude_friends():
             if player.will_intersect():
                 exclude_friends = intersect_player_lists(exclude_friends, player.friends())
                 playerNameForFileOutput += ' intersect ' + player.name()
             else:
                 exclude_friends.extend(player.friends())
@@ -57,37 +58,37 @@
     player = Player(playerUUID, friends=playerFriends, name_for_file_output=playerNameForFileOutput,
                     specs=playerSpecs, date_cutoff_for_friends=date_cutoff_friends,
                     players_used_to_combine=deepcopy(info_on_players)
                     if args().track_if_arg_players_online() else None)
     player.polish_friends_list(exclude_friends)
     return player
 
-def diff_f_lists(players: List[Player]) -> None:
+def diff_f_lists(players: list[Player]) -> None:
     """Runs through all pairs of players and outputs the diff of their f lists"""
     assert args().diff_f_lists()
     list_friends = input("Enter y to list out all the friends in each diff: ") in ('y', 'Y')
     print('\n\n')
     for p1, p2 in permutations(players, 2):
         p1.diff_f_lists(p2, list_friends)
 
-def get_players_from_args() -> Tuple[List[Player], List[str]]:
+def get_players_from_args() -> tuple[list[Player], list[str]]:
     """The first item in the tuple will be a list of Players.
        The second item will likely be empty for most use cases. However, if the caller wants this feature,
        it will be a list if uuid strings, where it's intended for each uuid to be checked for when they
        were friended by a Player in the first list."""
 
     specs = Specs.make_specs_object_and_initialize_common_specs()
     args_no_keywords_or_date = args().get_args(True)
-    players: List[Player] = []
+    players: list[Player] = []
     in_minus_symbol_section = False
     in_friended_when_section = False
     is_intersect_player = False
     FRIENDED_WHEN = 'friendedwhen'
     INTERSECT = 'intersect'
-    uuids_for_friended_when: List[str] = []
+    uuids_for_friended_when: list[str] = []
 
     for i, arg in enumerate(args_no_keywords_or_date):
         if in_minus_symbol_section or in_friended_when_section or is_intersect_player:
             assert not args().do_mini_program()
 
         if arg.endswith('.txt'):
             assert not in_friended_when_section
@@ -115,15 +116,15 @@
 
         if use_specific_textfile:
             assert not args().do_file_output()
             player = Player.make_player_from_json_textfile(args_no_keywords_or_date[i+1], arg, specs=specs)
         else:
             hypixel_obj = hypixel.Player(arg)
             uuid = hypixel_obj.getUUID()
-            all_friends: List[UUID_Plus_Time] = []
+            all_friends: list[UUID_Plus_Time] = []
             standard_friends = ProcessingResults.get_best_f_list_for_player_in_results(
                 uuid, must_have_times_friended=FRIENDED_WHEN in args_no_keywords_or_date
             )
             num_friends_msgs[0] = f"{len(standard_friends)} friends in biggest single friends list/file\n"
             if args().get_additional_friends():
                 all_friends = ProcessingResults.get_all_additional_friends_for_player(uuid)
                 num_friends_msgs[1] = f"{len(all_friends)} unique manually added friends\n"
@@ -145,20 +146,20 @@
         if not player.will_exclude_friends():
             player.set_date_cutoff_for_friends(args().date_cutoff())
         players.append(player)
         is_intersect_player = False
 
     return (players, uuids_for_friended_when)
 
-def output_player_jsons_to_file(players: List[Player]) -> None:
+def output_player_jsons_to_file(players: list[Player]) -> None:
     for player in players:
         Files.write_data_as_json_to_file(player.player_JSON(), "Player json for " + player.name(),
                                          "results/player-jsons")
 
-def friended_when_feature(players: List[Player], uuids_for_friended_when: List[str]) -> None:
+def friended_when_feature(players: list[Player], uuids_for_friended_when: list[str]) -> None:
     for player in players:
         for friend in player.friends():
             if friend.uuid() not in uuids_for_friended_when:
                 continue
             time_friended = friend.time_friended_parent_player('date')
             if time_friended is not None:
                 assert isinstance(time_friended, str)
@@ -213,15 +214,15 @@
             print(f"Keyword matches for '{substr}':\n" + '\n'.join(keyword_matches))
             ign_matches = sorted([ign for ign in ProcessingResults.ign_uuid_pairs_in_results()
                                   if substr in ign.lower()])
             print(f"\nPlayer name matches for '{substr}':\n" + '\n'.join(ign_matches) + '\n')
     else:
         assert False
 
-def main(argv: Optional[List[str]] = None) -> None:
+def main(argv: Optional[list[str]] = None) -> None:
     """When called as a script, `argv` is left as None and `sys.argv` is used.
        If calling main() programatically from another python file though, pass the args
        you want via `argv`."""
     MyClasses.set_args(argv if argv is not None else sys.argv)
 
     if args().do_mini_program():
         do_mini_program()
```

### Comparing `hypickle-1.1.4/hypickle.egg-info/PKG-INFO` & `hypickle-1.1.5/hypickle.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: hypickle
-Version: 1.1.4
+Version: 1.1.5
 Summary: A script that outputs realtime stats for custom lists of friends you create.
 Author-email: John Doknjas <jdoknjas@sfu.ca>
 Project-URL: Homepage, https://github.com/johndoknjas/hypixel-online-friends
 Keywords: hypickle,hypixel,pit,bedwars,friends,stats,api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.0
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: deepdiff
 Requires-Dist: mplcursors
 
@@ -57,14 +57,15 @@
 
 Open the root directory of the project in the terminal, and then:
   - `python3 main.py *args*` allows you to test any local changes you've made to the project.
   - `vulture .` will find unused code.
   - `mypy .` will typecheck.
   - `pylint *.py` will review the code for style.
   - `pydeps hypickle` will output a dependency graph of the project's modules.
-  - `python unused-funcs.py` is a basic script I wrote that attempts to find functions which are never/rarely used.
-  - `pytest tests.py` runs a few basic automated tests. Requires installing `pytest`. To run manual tests (output to
+  - `python my-linter.py` is a basic script I wrote that mainly attempts to find functions which are never/rarely used.
+  - `pytest tests.py` runs a few basic automated tests. To run manual tests (output to
     the screen needs to be judged by the tester), run `python tests.py`.
+  - `vermin hypickle` deduces the oldest version of python that works to run the project. The expected output is 3.8, corresponding with `requires-python = ">= 3.8"` in `pyproject.toml`.
 
 ### Acknowledgements:
 
 The `hypixel.py` and `leveling.py` files were originally from [Snuggle's repo](https://github.com/Snuggle/hypixel.py/). Since then I have made a number of modifications to them.
```

### Comparing `hypickle-1.1.4/hypickle.egg-info/SOURCES.txt` & `hypickle-1.1.5/hypickle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypickle-1.1.4/pyproject.toml` & `hypickle-1.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
-requires-python = ">= 3.0"
+requires-python = ">= 3.8"
 name = "hypickle"
-version = "1.1.4"
+version = "1.1.5"
 authors = [
   { name="John Doknjas", email="jdoknjas@sfu.ca" },
 ]
 description = "A script that outputs realtime stats for custom lists of friends you create."
 keywords = ["hypickle", "hypixel", "pit", "bedwars", "friends", "stats", "api"]
 dependencies = [
   "requests",
```

