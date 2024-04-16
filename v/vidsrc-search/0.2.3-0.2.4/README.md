# Comparing `tmp/vidsrc_search-0.2.3.tar.gz` & `tmp/vidsrc_search-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vidsrc_search-0.2.3.tar", last modified: Sun Apr 14 05:40:58 2024, max compression
+gzip compressed data, was "vidsrc_search-0.2.4.tar", last modified: Tue Apr 16 20:02:59 2024, max compression
```

## Comparing `vidsrc_search-0.2.3.tar` & `vidsrc_search-0.2.4.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-14 05:40:58.594907 vidsrc_search-0.2.3/
--rw-r--r--   0 Dev        (502) staff       (20)     1053 2024-04-11 00:33:35.000000 vidsrc_search-0.2.3/LICENSE
--rw-r--r--   0 Dev        (502) staff       (20)     1958 2024-04-14 05:40:58.594675 vidsrc_search-0.2.3/PKG-INFO
--rw-r--r--   0 Dev        (502) staff       (20)     1075 2024-04-12 02:57:47.000000 vidsrc_search-0.2.3/README.md
--rw-r--r--   0 Dev        (502) staff       (20)      977 2024-04-14 04:48:50.000000 vidsrc_search-0.2.3/pyproject.toml
--rw-r--r--   0 Dev        (502) staff       (20)       38 2024-04-14 05:40:58.594956 vidsrc_search-0.2.3/setup.cfg
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-14 05:40:58.590431 vidsrc_search-0.2.3/src/
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-14 05:40:58.592412 vidsrc_search-0.2.3/src/vidsrc_search/
--rw-r--r--   0 Dev        (502) staff       (20)     1238 2024-04-14 05:30:44.000000 vidsrc_search-0.2.3/src/vidsrc_search/__main__.py
--rw-r--r--   0 Dev        (502) staff       (20)     2111 2024-04-14 05:33:44.000000 vidsrc_search-0.2.3/src/vidsrc_search/argparsing.py
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-14 05:40:58.594138 vidsrc_search-0.2.3/src/vidsrc_search/core/
--rw-r--r--   0 Dev        (502) staff       (20)     2166 2024-04-14 01:25:38.000000 vidsrc_search-0.2.3/src/vidsrc_search/core/help.py
--rw-r--r--   0 Dev        (502) staff       (20)     8120 2024-04-14 05:40:13.000000 vidsrc_search-0.2.3/src/vidsrc_search/core/library.py
--rw-r--r--   0 Dev        (502) staff       (20)    10870 2024-04-14 05:39:44.000000 vidsrc_search-0.2.3/src/vidsrc_search/core/search.py
--rw-r--r--   0 Dev        (502) staff       (20)      677 2024-04-14 04:48:41.000000 vidsrc_search-0.2.3/src/vidsrc_search/core/version.py
--rw-r--r--   0 Dev        (502) staff       (20)      756 2024-04-14 01:08:30.000000 vidsrc_search-0.2.3/src/vidsrc_search/modules.py
--rw-r--r--   0 Dev        (502) staff       (20)     6584 2024-04-14 05:39:16.000000 vidsrc_search-0.2.3/src/vidsrc_search/utils.py
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-14 05:40:58.594421 vidsrc_search-0.2.3/src/vidsrc_search.egg-info/
--rw-r--r--   0 Dev        (502) staff       (20)     1958 2024-04-14 05:40:58.000000 vidsrc_search-0.2.3/src/vidsrc_search.egg-info/PKG-INFO
--rw-r--r--   0 Dev        (502) staff       (20)      530 2024-04-14 05:40:58.000000 vidsrc_search-0.2.3/src/vidsrc_search.egg-info/SOURCES.txt
--rw-r--r--   0 Dev        (502) staff       (20)        1 2024-04-14 05:40:58.000000 vidsrc_search-0.2.3/src/vidsrc_search.egg-info/dependency_links.txt
--rw-r--r--   0 Dev        (502) staff       (20)       62 2024-04-14 05:40:58.000000 vidsrc_search-0.2.3/src/vidsrc_search.egg-info/entry_points.txt
--rw-r--r--   0 Dev        (502) staff       (20)       34 2024-04-14 05:40:58.000000 vidsrc_search-0.2.3/src/vidsrc_search.egg-info/requires.txt
--rw-r--r--   0 Dev        (502) staff       (20)       14 2024-04-14 05:40:58.000000 vidsrc_search-0.2.3/src/vidsrc_search.egg-info/top_level.txt
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-16 20:02:59.502227 vidsrc_search-0.2.4/
+-rw-r--r--   0 Dev        (502) staff       (20)     1053 2024-04-15 17:13:28.000000 vidsrc_search-0.2.4/LICENSE
+-rw-r--r--   0 Dev        (502) staff       (20)     2996 2024-04-16 20:02:59.501926 vidsrc_search-0.2.4/PKG-INFO
+-rw-r--r--   0 Dev        (502) staff       (20)     2055 2024-04-16 07:34:13.000000 vidsrc_search-0.2.4/README.md
+-rw-r--r--   0 Dev        (502) staff       (20)     1027 2024-04-16 02:37:13.000000 vidsrc_search-0.2.4/pyproject.toml
+-rw-r--r--   0 Dev        (502) staff       (20)       38 2024-04-16 20:02:59.502297 vidsrc_search-0.2.4/setup.cfg
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-16 20:02:59.498072 vidsrc_search-0.2.4/src/
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-16 20:02:59.499738 vidsrc_search-0.2.4/src/vidsrc_search/
+-rw-r--r--   0 Dev        (502) staff       (20)     1279 2024-04-16 19:24:15.000000 vidsrc_search-0.2.4/src/vidsrc_search/__main__.py
+-rw-r--r--   0 Dev        (502) staff       (20)     2243 2024-04-16 02:57:09.000000 vidsrc_search-0.2.4/src/vidsrc_search/argparsing.py
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-16 20:02:59.501205 vidsrc_search-0.2.4/src/vidsrc_search/core/
+-rw-r--r--   0 Dev        (502) staff       (20)     2884 2024-04-16 19:50:55.000000 vidsrc_search-0.2.4/src/vidsrc_search/core/help.py
+-rw-r--r--   0 Dev        (502) staff       (20)    11007 2024-04-16 19:54:42.000000 vidsrc_search-0.2.4/src/vidsrc_search/core/library.py
+-rw-r--r--   0 Dev        (502) staff       (20)    11526 2024-04-16 19:18:36.000000 vidsrc_search-0.2.4/src/vidsrc_search/core/search.py
+-rw-r--r--   0 Dev        (502) staff       (20)      765 2024-04-16 19:17:32.000000 vidsrc_search-0.2.4/src/vidsrc_search/core/version.py
+-rw-r--r--   0 Dev        (502) staff       (20)     1019 2024-04-16 19:17:40.000000 vidsrc_search-0.2.4/src/vidsrc_search/modules.py
+-rw-r--r--   0 Dev        (502) staff       (20)     4946 2024-04-16 19:16:36.000000 vidsrc_search-0.2.4/src/vidsrc_search/term.py
+-rw-r--r--   0 Dev        (502) staff       (20)     5874 2024-04-16 19:23:26.000000 vidsrc_search-0.2.4/src/vidsrc_search/utils.py
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-16 20:02:59.501663 vidsrc_search-0.2.4/src/vidsrc_search.egg-info/
+-rw-r--r--   0 Dev        (502) staff       (20)     2996 2024-04-16 20:02:59.000000 vidsrc_search-0.2.4/src/vidsrc_search.egg-info/PKG-INFO
+-rw-r--r--   0 Dev        (502) staff       (20)      556 2024-04-16 20:02:59.000000 vidsrc_search-0.2.4/src/vidsrc_search.egg-info/SOURCES.txt
+-rw-r--r--   0 Dev        (502) staff       (20)        1 2024-04-16 20:02:59.000000 vidsrc_search-0.2.4/src/vidsrc_search.egg-info/dependency_links.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       62 2024-04-16 20:02:59.000000 vidsrc_search-0.2.4/src/vidsrc_search.egg-info/entry_points.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       77 2024-04-16 20:02:59.000000 vidsrc_search-0.2.4/src/vidsrc_search.egg-info/requires.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       14 2024-04-16 20:02:59.000000 vidsrc_search-0.2.4/src/vidsrc_search.egg-info/top_level.txt
```

### Comparing `vidsrc_search-0.2.3/LICENSE` & `vidsrc_search-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vidsrc_search-0.2.3/pyproject.toml` & `vidsrc_search-0.2.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vidsrc-search"
-version = "0.2.3"
+version = "0.2.4"
 description = "A pirate movie watcher written in Python"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
@@ -16,18 +16,19 @@
     "Topic :: Multimedia",
     "Topic :: Utilities",
     "Environment :: Console"
 ]
 
 keywords = ["movie", "video", "search"]
 dependencies = [
-    "aiohttp",
-    "thefuzz",
-    "tabulate",
-    "requests"
+    "aiohttp>=3.9.3",
+    "thefuzz>=0.22.1",
+    "tabulate>=0.9.0",
+    "requests>=2.31.0",
+    "tqdm>=4.66.2"
 ]
 
 requires-python = ">=3.8"
 
 [project.urls]
 Homepage = "https://github.com/SomedudeX/vidsrc-search"
 License = "https://github.com/SomedudeX/vidsrc-search/blob/main/LICENSE"
```

### Comparing `vidsrc_search-0.2.3/src/vidsrc_search/__main__.py` & `vidsrc_search-0.2.4/src/vidsrc_search/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
+import re
 import sys
 
 from . import utils
 from . import modules
 from . import argparsing
 
 from .argparsing import ArgumentsError
 
 
 def main() -> int:
     try:
-        utils.initialize()
         args = argparsing.parse_arguments(sys.argv)
+        utils.initialize(args)
         return modules.start(args)
     except UserWarning:
-        print(f"warning: vidsrc-search received user warning")
-        print(f"warning: vidsrc-search terminating with exit code 1")
+        print(f" • vidsrc-search received user warning")
+        print(f" • vidsrc-search terminating with exit code 1")
         return 1
     except KeyboardInterrupt:
-        print(f"\nwarning: vidsrc-search received keyboard interrupt")
-        print(f"warning: vidsrc-search terminating with exit code 1")
+        print(f"\n • vidsrc-search received keyboard interrupt")
+        print(f" • vidsrc-search terminating with exit code 1")
         return 1
     except ArgumentsError as e:
-        print(f"fatal: {e.message}")
-        print(f"fatal: vidsrc-search received an arguments error")
-        print(f"fatal: vidsrc-search terminating with exit code {e.code}")
+        print(f" • inapt arguments: {e.message}")
+        print(f" • vidsrc-search terminating with exit code {e.code}")
         return e.code
     except Exception as e:
-        print(f"fatal: {str(e).lower()}")
-        print(f"fatal: vidsrc-search received and unknown {type(e).__name__.lower()}")
-        print(f"fatal: vidsrc-search terminating with exit code 255")
+        name = re.sub(r"(?<!^)(?=[A-Z])", " ", type(e).__name__).lower()
+        print(f"\n • {str(e).lower()}")
+        print(f" • vidsrc-search received an unknown {name}")
+        print(f" • vidsrc-search terminating with exit code 255")
         return 255
     finally:
+        # Cleanup needs to happen no matter what
         utils.cleanup()
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vidsrc_search-0.2.3/src/vidsrc_search/argparsing.py` & `vidsrc_search-0.2.4/src/vidsrc_search/argparsing.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,24 +48,28 @@
 
 def parse_arguments(argv: List[str]) -> Dict[str, Any]:
     """Parse the arguments from sys.argv into a dictionary"""
     positionals, flags = split_arguments(argv[1:])
     parsed_arguments = {
         "module": [""],
         "raw": False,
-        "new": False
+        "new": False,
+        "dbg": False
     }
 
     if len(positionals) > 0:
         parsed_arguments["module"] = positionals
 
     for flag in flags:   # Mapping each command line flag to a dictionary key
         if flag == "--raw" or flag == "-r":
             parsed_arguments["raw"] = True
             continue
         if flag == "--new" or flag == "-n":
             parsed_arguments["new"] = True
             continue
+        if flag == "--debug" or flag == "-d":
+            parsed_arguments["dbg"] = True
+            continue
         if is_stacked_flag(flag):
             raise ArgumentsError(f"stacked flag '{flag}' not allowed", 1)
         raise ArgumentsError(f"invalid flag '{flag}' received", 1)
     return parsed_arguments
```

### Comparing `vidsrc_search-0.2.3/src/vidsrc_search/core/help.py` & `vidsrc_search-0.2.4/src/vidsrc_search/core/help.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,112 @@
-from typing import List
+from typing import Any, Dict, List
 
 from ..argparsing import ArgumentsError
+from ..term import Logger
+
+LogHelp = Logger()
 
 
 HELP = """\
 usage: vidsrc-search <command> [option] [flags]
 
 available commands:
     help        shows this menu
-    search      search a movie by name
+    version     displays version info
+    search      search a movie by its name
     library     actions regarding the movie lib
 
+optional flags:
+    -d, --debug enables debug logging and disables
+                certain features (e.g. progress bars)
+
 use 'vidsrc-search help <command>' for info on a
-specific command. arguments are strictly parsed in
-the order specified above\
+specific command. arguments are strictly parsed in the
+order specified above. when filing a bug report, please
+be sure to use the '--debug' flag in log.\
 """
 
 
 HELP_HELP = """\
 usage: vidsrc-search help [option]
 
 available options:
     help        shows detailed help for 'help'
+    version     shows detailed help for 'version'
     search      shows detailed help for 'search'
     library     shows detailed help for 'library'
 
 example usage:
     vidsrc-search help library
     vidsrc-search help help\
 """
 
 
+HELP_VERSION = """\
+usage: vidsrc-search version
+
+displays the program version and relevant system info.
+please include the output of this command when filing
+a bug report.
+
+example usage:
+    vidsrc-search version\
+"""
+
+
 HELP_SEARCH = """\
 usage: vidsrc-search search <option> [flags]
 
 required option:
     <str>       a movie title that you would like
                 vidsrc-search to search for
 
 optional flags:
-    --raw       when this flag is specified, the
-                program won't do any preprocessing
-                to the html
-    --new       when this flag is specified, the
-                program will re-cache the html to
-                your computer from vidsrc.to
+    -r, --raw   when this flag is specified, the
+                program will open the original website
+                instead of caching the html
+    -n, --new   when this flag is specified, the
+                program will re-cache the html to your
+                computer from vidsrc.to
 
 example usage:
     vidsrc-search search 'oppenheimer'
-    vidsrc-search search 'avatar'
+    vidsrc-search search 'avatar' --new
 
-the optional flags will have no effect with
-commands other than 'search'\
+the optional flags will have no effect with commands
+other than 'search'\
 """
 
 
 HELP_LIB = """\
 usage: vidsrc-search library <option>
 
 required options:
     size        prints the program's disk usage
     remove      removes the movies library
     download    downloads the latest movies library
                 from https://vidsrc.to
 
 example usage:
-    vidsrc-search library download\
+    vidsrc-search library download
+    vidsrc-search library remove\
 """
 
 
-def run_module(arguments: List[str]) -> None:
+def run_module(modules: List[str], args: Dict[str, Any]) -> None:
     """Runs the help module and prints help"""
-    if arguments == ["help", "library"]:
+    if modules == ["help", "library"]:
         print(HELP_LIB)
         return
-    if arguments == ["help", "search"]:
+    if modules == ["help", "search"]:
         print(HELP_SEARCH)
         return
-    if arguments == ["help", "help"]:
+    if modules == ["help", "version"]:
+        print(HELP_VERSION)
+        return
+    if modules == ["help", "help"]:
         print(HELP_HELP)
         return
-    if arguments == [""] or arguments == ["help"]:
+    if modules == [""] or modules == ["help"]:
         print(HELP)
         return
-    raise ArgumentsError(f"invalid arguments for command 'help' received: {' '.join(arguments)}")
+    raise ArgumentsError(f"invalid arguments for command 'help' received: {' '.join(modules)}")
```

### Comparing `vidsrc_search-0.2.3/src/vidsrc_search/core/search.py` & `vidsrc_search-0.2.4/src/vidsrc_search/core/search.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # Using classes for better organization
 
 import os
 import json
 import requests
 import webbrowser
 
+from .library import Library
 from .. import utils
+from .. import term
+from ..term import Logger
 from ..argparsing import ArgumentsError
-from .library import Library
 
 from typing import Any, Dict, List, Tuple, Union
 
 from tabulate import tabulate
 from thefuzz.fuzz import partial_ratio, ratio
 from html.parser import HTMLParser
 
+LogSearch = Logger()
+
+
 
 class FileProcessor(HTMLParser):
     """Processes the HTML file downloaded from vidsrc.to. This class is derived
     from the HTMLParser class in Python's standard library. See its
     documentation for more information.
 
     When calling the feed() function on an instance of this class, it will mark
@@ -46,14 +51,15 @@
         called. It will insert the current position (lineno and offset) to
         the start_positions if the tag is "bad"
         """
         if tag not in ["script"]:
             return
         for attr in attrs:
             if self.bad_script(attr):
+                LogSearch.log(f"bad start tag detected")
                 self._current_bad_script += 1
                 self.start_positions.append(self.getpos())
         return
 
     def handle_endtag(
         self,
         tag: Union[str, Any]
@@ -61,14 +67,15 @@
         """When an end tag is encountered, this function is automatically
         called. It will insert the current position (lineno and offset) to
         the end_positions if the tag is "bad"
         """
         if tag not in ["script"]:
             return
         if self._current_bad_script == 1:
+            LogSearch.log(f"bad end tag detected")
             self._current_bad_script = 0
             self.end_positions.append(self.getpos())
             self.positions_tag.append("</script>")
         if self._current_bad_script != 0:
             self._current_bad_script -= 1
         return
 
@@ -88,30 +95,32 @@
     """Library search related functions"""
 
     def __init__(
         self,
         query: str
     ) -> None:
         """Initializes a SearchManager object with a query"""
+        self.library = Library()
         self.query: str = query
         self.results: List[Dict] = []
         return
 
     def search_library(self) -> None:
         """Initiates a library search with the query specified during init"""
-        library = Library()
-        library.check_library()
-        with open(library.lib_path, "r") as f:
+        LogSearch.log(f"reading library")
+        with open(self.library.lib_path, "r") as f:
             library = f.read()
         library = json.loads(library)
 
+        LogSearch.log(f"checking library entries for potential match")
         for entry in library:
             self.check_entry(entry)
         self.sort_results()
 
+        LogSearch.log(f"processing matched entries")
         while len(self.results) > 20:
             del self.results[len(self.results) - 1]
         for index, result in enumerate(self.results):
             result["Index"] = f"[{index + 1}]"
             result["Match"] += "%"
         self.results.reverse()
         return
@@ -158,31 +167,36 @@
         query: str,
         args: Dict[str, Any]
     ) -> None:
         """Initializes a SearchHandler object"""
         self.query = query
         self.results = []
 
+        term.check_tty()
+
+        self.library = Library()
+        self.library.check_library()
+
         self.raw = args["raw"]
         self.new = args["new"]
         return
 
-
-    def begin_search(self) -> None:
+    def handle_search(self) -> None:
         """Handles searching the movie library"""
         self.process_query()
-        print(f"info: searching json library for '{self.query}'")
-        print(f"info: open raw website: {str(self.raw).lower()}")
-        print(f"info: recaching website: {str(self.new).lower()}")
+        print(f" • searching json library for '{self.query}'")
+        print(f" • open raw website: {str(self.raw).lower()}")
+        print(f" • recaching website: {str(self.new).lower()}")
+
         self.manager = SearchManager(self.query)
         self.manager.search_library()
         self.results = self.manager.results
         if len(self.results) == 0 :
-            print(f"info: '{self.query}' not found in movies library")
-            print(f"info: vidsrc-search terminating due to entry not found")
+            print(f" • '{self.query}' not found in movies library")
+            print(f" • vidsrc-search terminating due to entry not found")
             return
         self.print_movies()
         open_index = self.ask_open_index()
         self.show_movie(open_index)
         return
 
     def print_movies(self) -> None:
@@ -202,106 +216,109 @@
             try:
                 open_index = int(input(" > choose an index to open in browser: "))
                 if open_index <= 0 or open_index > len(self.results):
                     raise ValueError()
                 open_index = len(self.results) - open_index
                 return open_index
             except ValueError:
-                print("error: please enter a valid value")
+                print(" • please enter a valid value")
                 continue
 
     def show_movie(self, index: int) -> None:
         """Shows the movie chosen by the user in their browser"""
         SearchHandler.print_warning()
         utils.check_internet()
 
-        number = index + 1
+        LogSearch.log(f"gathering movie information from library")
         title = self.results[index]["Title"]
         url = self.results[index]["URL"]
         id = self.results[index]["IMDB ID"]
 
         if self.raw:
-            print(f"info: opening #{number} '{title}' in new browser window")
+            LogSearch.log("directly opening vidsrc link in browser")
+            print(f" • opening '{title}' in new browser tab")
             webbrowser.open(url)
             return
 
         if self.new or not os.path.exists(os.path.expanduser(f"~/.local/vidsrc-search/cache/{id}.html")):
             SearchHandler.cache_movie(url, f"~/.local/vidsrc-search/cache/{id}.html")
         SearchHandler.process_html(os.path.expanduser(f"~/.local/vidsrc-search/cache/{id}.html"))
-        print(f"info: opening #{number} '{title}' in new browser window")
+        print(f" • opening '{title}' in new browser tab")
         webbrowser.open("file://" + os.path.expanduser(f"~/.local/vidsrc-search/cache/{id}.html"))
         return
 
     def process_query(self) -> None:
         if len(self.query) < 1:
             return
         if self.query[0] == "'" and self.query[len(self.query) - 1] == "'":
             self.query = self.query[1:-1]
         return
 
     @staticmethod
     def print_warning() -> None:
         """Prints the warning before showing a movie"""
         print()
-        print("warning: the content of the movie is hosted on a third party site. the")
-        print("         site is not endorsed by the author or checked for its quality, ")
-        print("         content, or authenticity. the author of vidsrc-search disclaims")
-        print("         any responsibility, express or implied, of the consequences ")
-        print("         as a result your usage or dependence on the website provided ")
-        print("         through this tool. ")
-        print("warning: the following window shown will be the cached contents of vidsrc.to\n")
+        print(" • warning: the content of the movie is hosted on a third party site. the")
+        print("            site is not endorsed by the author or checked for its quality, ")
+        print("            content, or authenticity. the author of vidsrc-search disclaims")
+        print("            any responsibility, express or implied, of the consequences ")
+        print("            as a result your usage or dependence on the website provided ")
+        print("            through this tool. ")
+        print(" • warning: the following window shown will be the cached contents of vidsrc.to\n")
         affirm = input(" > i have read and understood the conditions above (Y/n) ")
         print()
         if not affirm == "Y":
-            print("info: terminating per user request")
+            print(" • terminating per user request")
             raise UserWarning
         return
 
     @staticmethod
     def cache_movie(url: str, path: str) -> None:
         """Caches a movie html to disk"""
         response = requests.get(url)
-        print(f"info: caching movie from remote html")
-        print(f"info: remote html request status code is {response.status_code}")
+        LogSearch.log(f"caching movie from '{url}'")
+        LogSearch.log(f"remote html response status code is {response.status_code}")
         with open(os.path.expanduser(path), "w") as f:
             f.write(response.content.decode())
-            print(f"info: finished caching html")
 
     @staticmethod
     def delete_substring(text, start_offset, end_offset):
         """Delete a section of the text from a start offset to an end offset"""
         deleted_text = text[:start_offset - 1] + text[end_offset + 1:]
         return deleted_text
 
     @staticmethod
     def process_html(path: str) -> None:
         """Processes the html file downloaded from vidsrc.to"""
-        print(f"info: processing html")
+        LogSearch.log(f"processing html by removing inapt elements")
+        detected = 0  # For debugging purposes
         with open(path, "r") as f:
             content = f.readlines()
             content = ''.join(content)
             while True:
                 parser = FileProcessor()
                 parser.feed(content)
                 if len(parser.positions_tag) == 0:
+                    LogSearch.log(f"removed {detected} inapt element(s)")
                     break
+                detected += 1
                 content = SearchHandler.delete_substring(
                     content,
                     parser.start_positions[0][1] + 1,
                     parser.end_positions[0][1] + len(parser.positions_tag[0]) - 1
                 )
 
-        print(f"info: writing processed html")
+        LogSearch.log(f"dumping processed html file")
         with open(path, "w") as f:
             f.write(content)
 
 
 def run_module(modules: List[str], args: Dict[str, Any]) -> None:
     """Runs the search module"""
     if len(modules) != 2:
         raise ArgumentsError(f"expected 1 argument for command 'search', got {len(modules) - 1} instead")
     if args["new"] and args["raw"]:
         raise ArgumentsError(f"'--new' and '--raw' are mutually exclusive flags")
     search = SearchHandler(modules[1], args)
-    search.begin_search()
+    search.handle_search()
     return
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vidsrc_search-0.2.3/src/vidsrc_search/core/version.py` & `vidsrc_search-0.2.4/src/vidsrc_search/core/version.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import platform
 
-from typing import List
+from typing import Any, Dict, List
+
 from ..argparsing import ArgumentsError
+from ..term import Logger
 
-__version__ = "v0.2.3"
+__version__ = "v0.2.4"
+LogVersion = Logger()
 
 
 def print_version() -> None:
     """Prints system information and the version of the program"""
-    print(f"vidsrc-search {__version__}")
-    print(f"{platform.python_implementation().lower()} {platform.python_version().lower()}")
-    print(f"{platform.platform(True, True).lower()} {platform.machine().lower()}")
+    print(f" • vidsrc-search {__version__}")
+    print(f" • {platform.python_implementation().lower()} {platform.python_version().lower()}")
+    print(f" • {platform.platform(True, True).lower()} {platform.machine().lower()}")
     return
 
 
-def run_module(arguments: List[str]):
+def run_module(module: List[str], args: Dict[str, Any]):
     """Runs the version module"""
-    if arguments == ["version"]:
+    if module == ["version"]:
         print_version()
         return
-    raise ArgumentsError(f"invalid arguments for command 'help' received: {' '.join(arguments)}")
+    raise ArgumentsError(f"invalid arguments for command 'help' received: {' '.join(module)}")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vidsrc_search-0.2.3/src/vidsrc_search/modules.py` & `vidsrc_search-0.2.4/src/vidsrc_search/modules.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,25 +2,32 @@
 
 from .core import help
 from .core import version
 from .core import library
 from .core import search
 
 from .argparsing import ArgumentsError
+from .utils import Logger
+
+LogModules = Logger()
 
 
 def start(args: Dict[str, Any]) -> int:
     """Runs the module parsed by argparsing.parse_arguments"""
     modules = args["module"]
     if modules[0] == "search":
+        LogModules.log("starting module search")
         search.run_module(modules, args)
         return 0
     if modules[0] == "library":
-        library.run_module(modules)
+        LogModules.log("starting module library")
+        library.run_module(modules, args)
         return 0
     if modules[0] == "version":
-        version.run_module(modules)
+        LogModules.log("starting module version")
+        version.run_module(modules, args)
         return 0
     if modules[0] == "help" or modules[0] == "":
-        help.run_module(modules)
+        LogModules.log("starting module help")
+        help.run_module(modules, args)
         return 0
     raise ArgumentsError(f"received invalid positional commands: {' '.join(args['module'])}")
```

### Comparing `vidsrc_search-0.2.3/src/vidsrc_search/utils.py` & `vidsrc_search-0.2.4/src/vidsrc_search/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,26 +6,30 @@
 import sys
 import json
 import shutil
 import asyncio
 import requests
 
 from typing import Any, Dict, List
-
+from .term import Logger
 from .core.library import RemovalManager
 
+LogUtils = Logger()
+
 
 def rmdir_recurse(path: str) -> None:
     """Uses shutil to delete directories recursively"""
     path = os.path.expanduser(path)
     if os.path.exists(path):
         shutil.rmtree(path)
     return
 
+
 def rmfile(path: str) -> None:
+    """Uses os.remove to delete a file"""
     path = os.path.expanduser(path)
     if os.path.exists(path):
         os.remove(path)
     return
 
 
 def get_file(path: str, extension: str) -> List[str]:
@@ -56,65 +60,79 @@
             return f"{total_size:.2f} {unit}"
         total_size /= 1024
     return f"{total_size:.2f} {units[len(units) - 1]}"
 
 
 def cleanup() -> None:
     """Removes buffer directories created during the execution of the program"""
+    LogUtils.log(f"performing program cleanup sequence")
     rmdir_recurse(os.path.expanduser("~/.config/pymovie")) # Pre v0.1.4 folder
     rmfile("~/.local/vidsrc-search/movie.json")
     rmfile("~/.local/vidsrc-search/tv.json")
     RemovalManager.remove_buffer()
     return
 
 
-def initialize() -> None:
+def initialize(args: Dict[str, Any]) -> None:
     """Called when the program first starts. Prepares program for execution"""
-    first_boot_check()
+    if args["dbg"]:
+        import platform
+        global LogUtils
+        from .core.version import __version__
+        from .term import enable_debug
+
+        enable_debug()
+        LogUtils.log(f"vidsrc-search {__version__}")
+        LogUtils.log(f"{platform.python_implementation().lower()} {platform.python_version().lower()}")
+        LogUtils.log(f"{platform.platform(True, True).lower()} {platform.machine().lower()}")
+    LogUtils.log("initializing directories")
     required_path_one = os.path.expanduser("~/.local/vidsrc-search/movie_buffer")
     required_path_two = os.path.expanduser("~/.local/vidsrc-search/tv_buffer")
     required_path_three = os.path.expanduser("~/.local/vidsrc-search/cache")
     os.makedirs(required_path_one, exist_ok=True)
     os.makedirs(required_path_two, exist_ok=True)
     os.makedirs(required_path_three, exist_ok=True)
 
     if sys.platform in ["win32", "cygwin", "msys"]:  # Windows has some issues with asyncio
+        LogUtils.log("patching windows asyncio")
         asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
     return
 
 
 def check_internet() -> None:
     """Verify computer internet connection"""
     try:
-        print("info: verifying internet connection")
         ping_url_one = "https://google.com"
         ping_url_two = "https://vidsrc.to"
+        LogUtils.log(f"checking internet connection by pinging {ping_url_one}")
         p1 = requests.get(ping_url_one, allow_redirects=False)
-        p2 = requests.get(ping_url_two, allow_redirects=False)
         p1.raise_for_status()
+        LogUtils.log(f"checking internet connection by pinging {ping_url_two}")
+        p2 = requests.get(ping_url_two, allow_redirects=False)
         p2.raise_for_status()
     except requests.exceptions.RequestException as e:
-        print(f"fatal: a network error occurred: {type(e).__name__.lower()} {str(e).lower()}")
-        print(f"fatal: vidsrc-search terminating with exit code 255")
+        name = re.sub(r"(?<!^)(?=[A-Z])", " ", type(e).__name__).lower()
+        print(f"• an unknown network error occurred: {name}")
+        print(f"• vidsrc-search terminating with exit code 255")
         sys.exit(255)
     return
 
 
 def unite_jsons(folder_path: str, dest_path: str, raw: bool = True) -> int:
     """Unites all movie/tv show json files from a folder and dumps them to
     another folder. Returns the number of entries parsed.
     """
     folder_path = os.path.expanduser(folder_path)
     dest_path = os.path.expanduser(dest_path)
+    LogUtils.log(f"uniting jsons from {folder_path} (raw={raw})")
+
     files = get_file(folder_path, ".json")
     for index, value in enumerate(files):
         files[index] = folder_path + value
 
-    print(f"info: uniting all jsons from '{folder_path}'")
-
     if raw:
         parsed_entries = []
         unparsed_entries = []
         for file in files:
             unparsed_entries.append(load_json(file))
         for entry in unparsed_entries:
             parsed_entries += parse_entry(entry)
@@ -122,18 +140,17 @@
         parsed_entries = []
         unparsed_entries = []
         for file in files:
             unparsed_entries.append(load_json(file))
         for item in unparsed_entries:
             parsed_entries += item
 
-    print(f"info: dumping united jsons to '{dest_path}'\n")
-
+    LogUtils.log(f"dumping united jsons to {dest_path}")
     with open(dest_path, "w") as file:
-        json.dump(parsed_entries, file, indent=4)
+        json.dump(parsed_entries, file)
     return len(parsed_entries)
 
 
 def load_json(path: str) -> List[Any]:
     """Loads a json file into a list and returns it. Returns an empty json file
     if the file does not exist or is invalid.
     """
@@ -147,37 +164,7 @@
 def parse_entry(page: Dict) -> List:
     """Parses an entry from a page downloaded from vidsrc"""
     ret: List = []
     for entry in page["result"]["items"]:
         if "embed_url_imdb" in entry:
             ret.append(entry)
     return ret
-
-
-def first_boot_check() -> None:
-    """Checks whether vidsrc-search is being booted up the first time"""
-    if not os.path.exists(os.path.expanduser("~/.local/vidsrc-search")):
-        print(
-            "\nit seems as though you are opening vidsrc-search for the first time.\n"
-            "because of this, you need to complete a ritual before proceeding. \n"
-            "please take your right hand and place it on your heart, and type the\n"
-            "following and press enter: "
-            "\n\n    'i solemnly swear that i am up to no good'"
-            "\n"
-        )
-
-        message = input(" > ")
-        if not message.lower() == "i solemnly swear that i am up to no good":
-            print("\nfatal: user failed to complete ritual")
-            print("fatal: vidsrc-search terminating with exit code 255")
-            sys.exit(255)
-        print("\ninfo: ritual successfully completed by user")
-        print("info: rerun vidsrc-search to gain access to the rest of the program")
-        print("info: vidsrc-search terminating with exit code 0")
-        required_path_one = os.path.expanduser("~/.local/vidsrc-search/movie_buffer")
-        required_path_two = os.path.expanduser("~/.local/vidsrc-search/tv_buffer")
-        required_path_three = os.path.expanduser("~/.local/vidsrc-search/cache")
-        os.makedirs(required_path_one, exist_ok=True)
-        os.makedirs(required_path_two, exist_ok=True)
-        os.makedirs(required_path_three, exist_ok=True)
-        sys.exit(0)
-    return
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vidsrc_search-0.2.3/src/vidsrc_search.egg-info/SOURCES.txt` & `vidsrc_search-0.2.4/src/vidsrc_search.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 src/vidsrc_search/__main__.py
 src/vidsrc_search/argparsing.py
 src/vidsrc_search/modules.py
+src/vidsrc_search/term.py
 src/vidsrc_search/utils.py
 src/vidsrc_search.egg-info/PKG-INFO
 src/vidsrc_search.egg-info/SOURCES.txt
 src/vidsrc_search.egg-info/dependency_links.txt
 src/vidsrc_search.egg-info/entry_points.txt
 src/vidsrc_search.egg-info/requires.txt
 src/vidsrc_search.egg-info/top_level.txt
```

