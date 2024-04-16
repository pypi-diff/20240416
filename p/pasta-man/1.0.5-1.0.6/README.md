# Comparing `tmp/pasta_man-1.0.5.tar.gz` & `tmp/pasta_man-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasta_man-1.0.5.tar", last modified: Mon Apr 15 21:49:06 2024, max compression
+gzip compressed data, was "pasta_man-1.0.6.tar", last modified: Tue Apr 16 03:55:55 2024, max compression
```

## Comparing `pasta_man-1.0.5.tar` & `pasta_man-1.0.6.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 21:49:06.885342 pasta_man-1.0.5/
--rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-15 01:10:20.000000 pasta_man-1.0.5/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     7276 2024-04-15 21:49:06.884872 pasta_man-1.0.5/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     4800 2024-04-15 21:49:01.000000 pasta_man-1.0.5/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1506 2024-04-15 21:47:27.000000 pasta_man-1.0.5/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-15 21:49:06.885408 pasta_man-1.0.5/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 21:49:06.868864 pasta_man-1.0.5/src/
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 21:49:06.875312 pasta_man-1.0.5/src/pasta_man/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 01:10:20.000000 pasta_man-1.0.5/src/pasta_man/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)      129 2024-04-15 01:10:20.000000 pasta_man-1.0.5/src/pasta_man/__main__.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 21:49:06.880005 pasta_man-1.0.5/src/pasta_man/architectures/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 21:32:13.000000 pasta_man-1.0.5/src/pasta_man/architectures/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)    11479 2024-04-15 21:32:13.000000 pasta_man-1.0.5/src/pasta_man/architectures/gui.py
--rw-r--r--   0 d33pster   (501) staff       (20)     9911 2024-04-15 21:32:13.000000 pasta_man-1.0.5/src/pasta_man/architectures/targets.py
--rw-r--r--   0 d33pster   (501) staff       (20)      776 2024-04-15 01:10:20.000000 pasta_man-1.0.5/src/pasta_man/encryption.py
--rw-r--r--   0 d33pster   (501) staff       (20)      237 2024-04-15 01:10:20.000000 pasta_man-1.0.5/src/pasta_man/exceptions.py
--rwxr-xr-x   0 d33pster   (501) staff       (20)     3508 2024-04-15 21:47:27.000000 pasta_man-1.0.5/src/pasta_man/pasta_man.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 21:49:06.881920 pasta_man-1.0.5/src/pasta_man/self_launch_thread/
--rw-r--r--   0 d33pster   (501) staff       (20)      191 2024-04-15 21:32:13.000000 pasta_man-1.0.5/src/pasta_man/self_launch_thread/Launch.py
--rw-r--r--   0 d33pster   (501) staff       (20)      725 2024-04-15 21:47:27.000000 pasta_man-1.0.5/src/pasta_man/self_launch_thread/Launcher.py
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 21:32:13.000000 pasta_man-1.0.5/src/pasta_man/self_launch_thread/__init__.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 21:49:06.883534 pasta_man-1.0.5/src/pasta_man/utilities/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 18:18:11.000000 pasta_man-1.0.5/src/pasta_man/utilities/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)      639 2024-04-15 18:18:11.000000 pasta_man-1.0.5/src/pasta_man/utilities/helptext.py
--rw-r--r--   0 d33pster   (501) staff       (20)     7546 2024-04-15 18:18:11.000000 pasta_man-1.0.5/src/pasta_man/utilities/pasta_menu.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 21:49:06.884261 pasta_man-1.0.5/src/pasta_man.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     7276 2024-04-15 21:49:06.000000 pasta_man-1.0.5/src/pasta_man.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      748 2024-04-15 21:49:06.000000 pasta_man-1.0.5/src/pasta_man.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-15 21:49:06.000000 pasta_man-1.0.5/src/pasta_man.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)      139 2024-04-15 21:49:06.000000 pasta_man-1.0.5/src/pasta_man.egg-info/entry_points.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       69 2024-04-15 21:49:06.000000 pasta_man-1.0.5/src/pasta_man.egg-info/requires.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       10 2024-04-15 21:49:06.000000 pasta_man-1.0.5/src/pasta_man.egg-info/top_level.txt
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 03:55:55.149762 pasta_man-1.0.6/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-15 01:10:20.000000 pasta_man-1.0.6/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     7454 2024-04-16 03:55:55.149297 pasta_man-1.0.6/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     4978 2024-04-16 03:54:54.000000 pasta_man-1.0.6/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1486 2024-04-16 03:54:54.000000 pasta_man-1.0.6/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-16 03:55:55.149817 pasta_man-1.0.6/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 03:55:55.135477 pasta_man-1.0.6/src/
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 03:55:55.141610 pasta_man-1.0.6/src/pasta_man/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 01:10:20.000000 pasta_man-1.0.6/src/pasta_man/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      129 2024-04-15 01:10:20.000000 pasta_man-1.0.6/src/pasta_man/__main__.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 03:55:55.145705 pasta_man-1.0.6/src/pasta_man/architectures/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 21:32:13.000000 pasta_man-1.0.6/src/pasta_man/architectures/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)    11479 2024-04-15 21:32:13.000000 pasta_man-1.0.6/src/pasta_man/architectures/gui.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     9911 2024-04-15 21:32:13.000000 pasta_man-1.0.6/src/pasta_man/architectures/targets.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      776 2024-04-15 01:10:20.000000 pasta_man-1.0.6/src/pasta_man/encryption.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      237 2024-04-15 01:10:20.000000 pasta_man-1.0.6/src/pasta_man/exceptions.py
+-rwxr-xr-x   0 d33pster   (501) staff       (20)     3508 2024-04-16 03:54:54.000000 pasta_man-1.0.6/src/pasta_man/pasta_man.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 03:55:55.146778 pasta_man-1.0.6/src/pasta_man/self_launch_thread/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1160 2024-04-16 03:54:54.000000 pasta_man-1.0.6/src/pasta_man/self_launch_thread/Launcher.py
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 21:32:13.000000 pasta_man-1.0.6/src/pasta_man/self_launch_thread/__init__.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 03:55:55.148126 pasta_man-1.0.6/src/pasta_man/utilities/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 18:18:11.000000 pasta_man-1.0.6/src/pasta_man/utilities/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      639 2024-04-15 18:18:11.000000 pasta_man-1.0.6/src/pasta_man/utilities/helptext.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     7579 2024-04-16 03:54:54.000000 pasta_man-1.0.6/src/pasta_man/utilities/pasta_menu.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 03:55:55.148700 pasta_man-1.0.6/src/pasta_man.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     7454 2024-04-16 03:55:55.000000 pasta_man-1.0.6/src/pasta_man.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      705 2024-04-16 03:55:55.000000 pasta_man-1.0.6/src/pasta_man.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-16 03:55:55.000000 pasta_man-1.0.6/src/pasta_man.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)      119 2024-04-16 03:55:55.000000 pasta_man-1.0.6/src/pasta_man.egg-info/entry_points.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       69 2024-04-16 03:55:55.000000 pasta_man-1.0.6/src/pasta_man.egg-info/requires.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       10 2024-04-16 03:55:55.000000 pasta_man-1.0.6/src/pasta_man.egg-info/top_level.txt
```

### Comparing `pasta_man-1.0.5/LICENSE` & `pasta_man-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.5/PKG-INFO` & `pasta_man-1.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta-man
-Version: 1.0.5
+Version: 1.0.6
 Summary: Password Manager
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>, Sairam Pimple <sairampimple003@gmail.com>, Shubham Narendra Singh <shubh1122000@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -91,19 +91,19 @@
 
 ### Faster than basic tkinter apps
 `Pasta-Man` actively uses Threads to carry out intensive tasks in order to minimize GUI lag as well as have better performance than any basic app created through python tkinter lib.
 
 ### Themes
 User can now change Theme for the app from the Menu Bar. Default is `Arc`. Whatever theme the user chooses, It will be set as default and next time `Pasta-Man` is launched, that theme will be loaded.
 
-Themes can be changed using the MenuBar.
-<!-- 
+Themes can be changed using the MenuBar -
+
 <img src="images/MenuBar.png">
 
-###### <p align='center'>MenuBar Screenshot<p> -->
+###### <p align='center'>MenuBar Screenshot<p>
 
 #### Currently Supported Themes
 
 - Adapta
 - Arc
 - Aquativo
 - Black
@@ -131,20 +131,20 @@
 - cryptography
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man==1.0.5
+pip install pasta-man==1.0.6
 ```
 
 ## README before [#Usage](#usage)
 
-After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man==1.0.4` -> `pasta-man` and `pasta-man-launcher`.
+After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man>=1.0.4` -> `pasta-man` and `pasta-man-launcher`.
 
 - `pasta-man` Command
 
     - This command will launch `pasta-man` as a separate and independent process.
     
     - The terminal will be usable after `pasta-man` command is run.
     
@@ -174,7 +174,12 @@
 ## Uninstall
 
 Uninstall using pip
 
 ```bash
 pip uninstall pasta-man
 ```
+
+## Yanked Versions
+- _v1.0.5_
+    
+    `Major Bug`: After Threads Update and Threads Patch 1, There was a major bug where the code breaks while initializing the app for the first time.
```

### Comparing `pasta_man-1.0.5/README.md` & `pasta_man-1.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,19 +40,19 @@
 
 ### Faster than basic tkinter apps
 `Pasta-Man` actively uses Threads to carry out intensive tasks in order to minimize GUI lag as well as have better performance than any basic app created through python tkinter lib.
 
 ### Themes
 User can now change Theme for the app from the Menu Bar. Default is `Arc`. Whatever theme the user chooses, It will be set as default and next time `Pasta-Man` is launched, that theme will be loaded.
 
-Themes can be changed using the MenuBar.
-<!-- 
+Themes can be changed using the MenuBar -
+
 <img src="images/MenuBar.png">
 
-###### <p align='center'>MenuBar Screenshot<p> -->
+###### <p align='center'>MenuBar Screenshot<p>
 
 #### Currently Supported Themes
 
 - Adapta
 - Arc
 - Aquativo
 - Black
@@ -80,20 +80,20 @@
 - cryptography
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man==1.0.5
+pip install pasta-man==1.0.6
 ```
 
 ## README before [#Usage](#usage)
 
-After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man==1.0.4` -> `pasta-man` and `pasta-man-launcher`.
+After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man>=1.0.4` -> `pasta-man` and `pasta-man-launcher`.
 
 - `pasta-man` Command
 
     - This command will launch `pasta-man` as a separate and independent process.
     
     - The terminal will be usable after `pasta-man` command is run.
     
@@ -122,8 +122,13 @@
 
 ## Uninstall
 
 Uninstall using pip
 
 ```bash
 pip uninstall pasta-man
-```
+```
+
+## Yanked Versions
+- _v1.0.5_
+    
+    `Major Bug`: After Threads Update and Threads Patch 1, There was a major bug where the code breaks while initializing the app for the first time.
```

### Comparing `pasta_man-1.0.5/pyproject.toml` & `pasta_man-1.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pasta-man"
-version = "1.0.5"
+version = "1.0.6"
 description = "Password Manager"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Software Development",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -27,14 +27,14 @@
 ]
 maintainers = [
     {name = "Soumyo Deep Gupta", email = "deep.main.ac@gmail.com"}
 ]
 dependencies = ['cryptography', 'pandas', 'termcolor', 'tk', 'optioner>=1.5.2', 'pyperclip', 'ttkthemes']
 
 [project.scripts]
-pasta-man-launcher = "pasta_man.self_launch_thread.Launch:drumroll"
+pasta-man-launcher = "pasta_man.pasta_man:main"
 pasta-man = "pasta_man.self_launch_thread.Launcher:main"
 
 [project.urls]
 GitHub = 'https://github.com/d33pster/pasta-man'
 Issues = 'https://github.com/d33pster/pasta-man/issues'
 Documentation = 'https://d33pster.github.io/pasta-man/'
```

### Comparing `pasta_man-1.0.5/src/pasta_man/architectures/gui.py` & `pasta_man-1.0.6/src/pasta_man/architectures/gui.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.5/src/pasta_man/architectures/targets.py` & `pasta_man-1.0.6/src/pasta_man/architectures/targets.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.5/src/pasta_man/encryption.py` & `pasta_man-1.0.6/src/pasta_man/encryption.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.5/src/pasta_man/pasta_man.py` & `pasta_man-1.0.6/src/pasta_man/pasta_man.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 # version info
-__version__ = "1.0.5"
+__version__ = "1.0.6"
 
 # import project specific modules
 from pasta_man.architectures.gui import pmanager
 from pasta_man.encryption import Encryption
 from pasta_man.exceptions import NoneTypeVariable, OptError
 from pasta_man.utilities.helptext import helptext
```

### Comparing `pasta_man-1.0.5/src/pasta_man/utilities/helptext.py` & `pasta_man-1.0.6/src/pasta_man/utilities/helptext.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.5/src/pasta_man/utilities/pasta_menu.py` & `pasta_man-1.0.6/src/pasta_man/utilities/pasta_menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import ttkthemes.themed_style
 
 class __menu__:
     def __init__(self, menuparent: Menu):
         self.parent = menuparent
         
         # set style -> theme -> default: arc
+        self.defaultTheme = None
         if not there(jPath(str(Path.home()), '.pastaman', '.defaulttheme')):
             self.style:ttkthemes.themed_style.ThemedStyle = ttkthemes.themed_style.ThemedStyle(theme='arc')
         else:
             with open(jPath(str(Path.home()), '.pastaman', '.defaulttheme'), 'r') as theme:
                 self.defaultTheme = theme.read().replace('\n', '')
                 self.style:ttkthemes.themed_style.ThemedStyle = ttkthemes.themed_style.ThemedStyle(theme=self.defaultTheme)
```

### Comparing `pasta_man-1.0.5/src/pasta_man.egg-info/PKG-INFO` & `pasta_man-1.0.6/src/pasta_man.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta-man
-Version: 1.0.5
+Version: 1.0.6
 Summary: Password Manager
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>, Sairam Pimple <sairampimple003@gmail.com>, Shubham Narendra Singh <shubh1122000@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -91,19 +91,19 @@
 
 ### Faster than basic tkinter apps
 `Pasta-Man` actively uses Threads to carry out intensive tasks in order to minimize GUI lag as well as have better performance than any basic app created through python tkinter lib.
 
 ### Themes
 User can now change Theme for the app from the Menu Bar. Default is `Arc`. Whatever theme the user chooses, It will be set as default and next time `Pasta-Man` is launched, that theme will be loaded.
 
-Themes can be changed using the MenuBar.
-<!-- 
+Themes can be changed using the MenuBar -
+
 <img src="images/MenuBar.png">
 
-###### <p align='center'>MenuBar Screenshot<p> -->
+###### <p align='center'>MenuBar Screenshot<p>
 
 #### Currently Supported Themes
 
 - Adapta
 - Arc
 - Aquativo
 - Black
@@ -131,20 +131,20 @@
 - cryptography
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man==1.0.5
+pip install pasta-man==1.0.6
 ```
 
 ## README before [#Usage](#usage)
 
-After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man==1.0.4` -> `pasta-man` and `pasta-man-launcher`.
+After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man>=1.0.4` -> `pasta-man` and `pasta-man-launcher`.
 
 - `pasta-man` Command
 
     - This command will launch `pasta-man` as a separate and independent process.
     
     - The terminal will be usable after `pasta-man` command is run.
     
@@ -174,7 +174,12 @@
 ## Uninstall
 
 Uninstall using pip
 
 ```bash
 pip uninstall pasta-man
 ```
+
+## Yanked Versions
+- _v1.0.5_
+    
+    `Major Bug`: After Threads Update and Threads Patch 1, There was a major bug where the code breaks while initializing the app for the first time.
```

### Comparing `pasta_man-1.0.5/src/pasta_man.egg-info/SOURCES.txt` & `pasta_man-1.0.6/src/pasta_man.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,13 +11,12 @@
 src/pasta_man.egg-info/dependency_links.txt
 src/pasta_man.egg-info/entry_points.txt
 src/pasta_man.egg-info/requires.txt
 src/pasta_man.egg-info/top_level.txt
 src/pasta_man/architectures/__init__.py
 src/pasta_man/architectures/gui.py
 src/pasta_man/architectures/targets.py
-src/pasta_man/self_launch_thread/Launch.py
 src/pasta_man/self_launch_thread/Launcher.py
 src/pasta_man/self_launch_thread/__init__.py
 src/pasta_man/utilities/__init__.py
 src/pasta_man/utilities/helptext.py
 src/pasta_man/utilities/pasta_menu.py
```

