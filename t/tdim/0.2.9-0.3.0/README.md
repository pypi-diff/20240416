# Comparing `tmp/tdim-0.2.9.tar.gz` & `tmp/tdim-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdim-0.2.9.tar", last modified: Sun Mar 17 10:38:03 2024, max compression
+gzip compressed data, was "tdim-0.3.0.tar", last modified: Tue Apr 16 11:36:24 2024, max compression
```

## Comparing `tdim-0.2.9.tar` & `tdim-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-03-17 10:38:03.685706 tdim-0.2.9/
--rw-r--r--   0 davep      (501) staff       (20)     2387 2024-03-17 10:38:03.685653 tdim-0.2.9/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)     1108 2023-05-09 21:23:38.000000 tdim-0.2.9/README.md
--rw-r--r--   0 davep      (501) staff       (20)     1439 2024-03-17 10:38:03.685968 tdim-0.2.9/setup.cfg
--rw-r--r--   0 davep      (501) staff       (20)      334 2023-05-09 20:31:00.000000 tdim-0.2.9/setup.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-03-17 10:38:03.684718 tdim-0.2.9/tdim/
--rw-r--r--   0 davep      (501) staff       (20)      528 2024-03-17 10:37:16.000000 tdim-0.2.9/tdim/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)     2567 2024-03-17 10:35:39.000000 tdim-0.2.9/tdim/__main__.py
--rw-r--r--   0 davep      (501) staff       (20)        0 2023-05-09 20:31:19.000000 tdim-0.2.9/tdim/py.typed
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-03-17 10:38:03.685479 tdim-0.2.9/tdim.egg-info/
--rw-r--r--   0 davep      (501) staff       (20)     2387 2024-03-17 10:38:03.000000 tdim-0.2.9/tdim.egg-info/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)      246 2024-03-17 10:38:03.000000 tdim-0.2.9/tdim.egg-info/SOURCES.txt
--rw-r--r--   0 davep      (501) staff       (20)        1 2024-03-17 10:38:03.000000 tdim-0.2.9/tdim.egg-info/dependency_links.txt
--rw-r--r--   0 davep      (501) staff       (20)       43 2024-03-17 10:38:03.000000 tdim-0.2.9/tdim.egg-info/entry_points.txt
--rw-r--r--   0 davep      (501) staff       (20)       16 2024-03-17 10:38:03.000000 tdim-0.2.9/tdim.egg-info/requires.txt
--rw-r--r--   0 davep      (501) staff       (20)        5 2024-03-17 10:38:03.000000 tdim-0.2.9/tdim.egg-info/top_level.txt
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-16 11:36:24.830079 tdim-0.3.0/
+-rw-r--r--   0 davep      (501) staff       (20)     2530 2024-04-16 11:36:24.830017 tdim-0.3.0/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)     1251 2024-03-17 10:42:59.000000 tdim-0.3.0/README.md
+-rw-r--r--   0 davep      (501) staff       (20)     1439 2024-04-16 11:36:24.830369 tdim-0.3.0/setup.cfg
+-rw-r--r--   0 davep      (501) staff       (20)      334 2023-05-09 20:31:00.000000 tdim-0.3.0/setup.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-16 11:36:24.829018 tdim-0.3.0/tdim/
+-rw-r--r--   0 davep      (501) staff       (20)      528 2024-04-16 11:35:25.000000 tdim-0.3.0/tdim/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)     2615 2024-04-16 11:32:54.000000 tdim-0.3.0/tdim/__main__.py
+-rw-r--r--   0 davep      (501) staff       (20)        0 2023-05-09 20:31:19.000000 tdim-0.3.0/tdim/py.typed
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-16 11:36:24.829829 tdim-0.3.0/tdim.egg-info/
+-rw-r--r--   0 davep      (501) staff       (20)     2530 2024-04-16 11:36:24.000000 tdim-0.3.0/tdim.egg-info/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)      246 2024-04-16 11:36:24.000000 tdim-0.3.0/tdim.egg-info/SOURCES.txt
+-rw-r--r--   0 davep      (501) staff       (20)        1 2024-04-16 11:36:24.000000 tdim-0.3.0/tdim.egg-info/dependency_links.txt
+-rw-r--r--   0 davep      (501) staff       (20)       43 2024-04-16 11:36:24.000000 tdim-0.3.0/tdim.egg-info/entry_points.txt
+-rw-r--r--   0 davep      (501) staff       (20)       16 2024-04-16 11:36:24.000000 tdim-0.3.0/tdim.egg-info/requires.txt
+-rw-r--r--   0 davep      (501) staff       (20)        5 2024-04-16 11:36:24.000000 tdim-0.3.0/tdim.egg-info/top_level.txt
```

### Comparing `tdim-0.2.9/PKG-INFO` & `tdim-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdim
-Version: 0.2.9
+Version: 0.3.0
 Summary: A simple tool for displaying terminal dimensions
 Home-page: https://github.com/davep/tdim
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -31,24 +31,29 @@
 
 # tdim - Show and help size terminal dimensions
 
 A simple tool to help when I want to size any terminal "just so".
 
 ## Installation
 
-`tdim` can be installed with either `pip`
+### pipx
+
+The package can be installed using [`pipx`](https://pypa.github.io/pipx/):
 
 ```sh
-$ pip install tdim
+$ pipx install tdim
 ```
 
-or ideally `pipx`:
+### Homebrew
+
+The package is available via Homebrew. Use the following commands to install:
 
 ```sh
-$ pipx install tdim
+$ brew tap davep/homebrew
+$ brew install tdim
 ```
 
 ## Usage
 
 To run the tool, just run `tdim`. Once you run it up you'll see a simple
 display of the dimensions of your terminal. Resize your terminal and be
 amazed as the numbers change!
```

### Comparing `tdim-0.2.9/setup.cfg` & `tdim-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `tdim-0.2.9/tdim/__init__.py` & `tdim-0.3.0/tdim/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ######################################################################
 # Main app information.
 __author__ = "Dave Pearson"
 __copyright__ = "Copyright 2023-2024, Dave Pearson"
 __credits__ = ["Dave Pearson"]
 __maintainer__ = "Dave Pearson"
 __email__ = "davep@davep.org"
-__version__ = "0.2.9"
+__version__ = "0.3.0"
 __licence__ = "GPLv3+"
 
 ##############################################################################
 # Export the imports.
 __all__ = []
 
 ### __init__.py ends here
```

### Comparing `tdim-0.2.9/tdim/__main__.py` & `tdim-0.3.0/tdim/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         Binding("b", "border", "Show/hide the border"),
         Binding("escape", "quit", "Quit the application"),
         Binding("0", "clear", "Clear the target ratio"),
         Binding("1", "ratio( 16, 9 )", "16x9"),
         Binding("2", "ratio( 4, 3 )", "4x3"),
         Binding("3", "ratio( 2, 1 )", "2x1"),
         Binding("4", "ratio( 1, 1 )", "1x1"),
+        Binding("5", "ratio( 9, 16 )", "9x16"),
     ]
     """Bindings for the application."""
 
     def compose(self) -> ComposeResult:
         """Compose the child widgets."""
         with Container():
             yield Label()
```

### Comparing `tdim-0.2.9/tdim.egg-info/PKG-INFO` & `tdim-0.3.0/tdim.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdim
-Version: 0.2.9
+Version: 0.3.0
 Summary: A simple tool for displaying terminal dimensions
 Home-page: https://github.com/davep/tdim
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -31,24 +31,29 @@
 
 # tdim - Show and help size terminal dimensions
 
 A simple tool to help when I want to size any terminal "just so".
 
 ## Installation
 
-`tdim` can be installed with either `pip`
+### pipx
+
+The package can be installed using [`pipx`](https://pypa.github.io/pipx/):
 
 ```sh
-$ pip install tdim
+$ pipx install tdim
 ```
 
-or ideally `pipx`:
+### Homebrew
+
+The package is available via Homebrew. Use the following commands to install:
 
 ```sh
-$ pipx install tdim
+$ brew tap davep/homebrew
+$ brew install tdim
 ```
 
 ## Usage
 
 To run the tool, just run `tdim`. Once you run it up you'll see a simple
 display of the dimensions of your terminal. Resize your terminal and be
 amazed as the numbers change!
```

