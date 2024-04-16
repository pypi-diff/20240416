# Comparing `tmp/pasta_man-1.0.6.tar.gz` & `tmp/pasta_man-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasta_man-1.0.6.tar", last modified: Tue Apr 16 03:55:55 2024, max compression
+gzip compressed data, was "pasta_man-1.0.7.tar", last modified: Tue Apr 16 04:10:26 2024, max compression
```

## Comparing `pasta_man-1.0.6.tar` & `pasta_man-1.0.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 03:55:55.149762 pasta_man-1.0.6/
--rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-15 01:10:20.000000 pasta_man-1.0.6/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     7454 2024-04-16 03:55:55.149297 pasta_man-1.0.6/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     4978 2024-04-16 03:54:54.000000 pasta_man-1.0.6/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1486 2024-04-16 03:54:54.000000 pasta_man-1.0.6/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-16 03:55:55.149817 pasta_man-1.0.6/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 03:55:55.135477 pasta_man-1.0.6/src/
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 03:55:55.141610 pasta_man-1.0.6/src/pasta_man/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 01:10:20.000000 pasta_man-1.0.6/src/pasta_man/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)      129 2024-04-15 01:10:20.000000 pasta_man-1.0.6/src/pasta_man/__main__.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 03:55:55.145705 pasta_man-1.0.6/src/pasta_man/architectures/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 21:32:13.000000 pasta_man-1.0.6/src/pasta_man/architectures/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)    11479 2024-04-15 21:32:13.000000 pasta_man-1.0.6/src/pasta_man/architectures/gui.py
--rw-r--r--   0 d33pster   (501) staff       (20)     9911 2024-04-15 21:32:13.000000 pasta_man-1.0.6/src/pasta_man/architectures/targets.py
--rw-r--r--   0 d33pster   (501) staff       (20)      776 2024-04-15 01:10:20.000000 pasta_man-1.0.6/src/pasta_man/encryption.py
--rw-r--r--   0 d33pster   (501) staff       (20)      237 2024-04-15 01:10:20.000000 pasta_man-1.0.6/src/pasta_man/exceptions.py
--rwxr-xr-x   0 d33pster   (501) staff       (20)     3508 2024-04-16 03:54:54.000000 pasta_man-1.0.6/src/pasta_man/pasta_man.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 03:55:55.146778 pasta_man-1.0.6/src/pasta_man/self_launch_thread/
--rw-r--r--   0 d33pster   (501) staff       (20)     1160 2024-04-16 03:54:54.000000 pasta_man-1.0.6/src/pasta_man/self_launch_thread/Launcher.py
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 21:32:13.000000 pasta_man-1.0.6/src/pasta_man/self_launch_thread/__init__.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 03:55:55.148126 pasta_man-1.0.6/src/pasta_man/utilities/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 18:18:11.000000 pasta_man-1.0.6/src/pasta_man/utilities/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)      639 2024-04-15 18:18:11.000000 pasta_man-1.0.6/src/pasta_man/utilities/helptext.py
--rw-r--r--   0 d33pster   (501) staff       (20)     7579 2024-04-16 03:54:54.000000 pasta_man-1.0.6/src/pasta_man/utilities/pasta_menu.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 03:55:55.148700 pasta_man-1.0.6/src/pasta_man.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     7454 2024-04-16 03:55:55.000000 pasta_man-1.0.6/src/pasta_man.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      705 2024-04-16 03:55:55.000000 pasta_man-1.0.6/src/pasta_man.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-16 03:55:55.000000 pasta_man-1.0.6/src/pasta_man.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)      119 2024-04-16 03:55:55.000000 pasta_man-1.0.6/src/pasta_man.egg-info/entry_points.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       69 2024-04-16 03:55:55.000000 pasta_man-1.0.6/src/pasta_man.egg-info/requires.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       10 2024-04-16 03:55:55.000000 pasta_man-1.0.6/src/pasta_man.egg-info/top_level.txt
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 04:10:26.317580 pasta_man-1.0.7/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-15 01:10:20.000000 pasta_man-1.0.7/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     7454 2024-04-16 04:10:26.317182 pasta_man-1.0.7/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     4978 2024-04-16 04:07:37.000000 pasta_man-1.0.7/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1486 2024-04-16 04:07:53.000000 pasta_man-1.0.7/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-16 04:10:26.317638 pasta_man-1.0.7/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 04:10:26.301986 pasta_man-1.0.7/src/
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 04:10:26.308115 pasta_man-1.0.7/src/pasta_man/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 01:10:20.000000 pasta_man-1.0.7/src/pasta_man/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      129 2024-04-15 01:10:20.000000 pasta_man-1.0.7/src/pasta_man/__main__.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 04:10:26.313250 pasta_man-1.0.7/src/pasta_man/architectures/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 21:32:13.000000 pasta_man-1.0.7/src/pasta_man/architectures/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)    11489 2024-04-16 04:07:20.000000 pasta_man-1.0.7/src/pasta_man/architectures/gui.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     9911 2024-04-15 21:32:13.000000 pasta_man-1.0.7/src/pasta_man/architectures/targets.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      776 2024-04-15 01:10:20.000000 pasta_man-1.0.7/src/pasta_man/encryption.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      237 2024-04-15 01:10:20.000000 pasta_man-1.0.7/src/pasta_man/exceptions.py
+-rwxr-xr-x   0 d33pster   (501) staff       (20)     3518 2024-04-16 04:07:45.000000 pasta_man-1.0.7/src/pasta_man/pasta_man.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 04:10:26.314654 pasta_man-1.0.7/src/pasta_man/self_launch_thread/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1160 2024-04-16 03:54:54.000000 pasta_man-1.0.7/src/pasta_man/self_launch_thread/Launcher.py
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 21:32:13.000000 pasta_man-1.0.7/src/pasta_man/self_launch_thread/__init__.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 04:10:26.315964 pasta_man-1.0.7/src/pasta_man/utilities/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 18:18:11.000000 pasta_man-1.0.7/src/pasta_man/utilities/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      639 2024-04-15 18:18:11.000000 pasta_man-1.0.7/src/pasta_man/utilities/helptext.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     7579 2024-04-16 03:54:54.000000 pasta_man-1.0.7/src/pasta_man/utilities/pasta_menu.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-16 04:10:26.316617 pasta_man-1.0.7/src/pasta_man.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     7454 2024-04-16 04:10:26.000000 pasta_man-1.0.7/src/pasta_man.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      705 2024-04-16 04:10:26.000000 pasta_man-1.0.7/src/pasta_man.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-16 04:10:26.000000 pasta_man-1.0.7/src/pasta_man.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)      119 2024-04-16 04:10:26.000000 pasta_man-1.0.7/src/pasta_man.egg-info/entry_points.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       69 2024-04-16 04:10:26.000000 pasta_man-1.0.7/src/pasta_man.egg-info/requires.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       10 2024-04-16 04:10:26.000000 pasta_man-1.0.7/src/pasta_man.egg-info/top_level.txt
```

### Comparing `pasta_man-1.0.6/LICENSE` & `pasta_man-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.6/PKG-INFO` & `pasta_man-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta-man
-Version: 1.0.6
+Version: 1.0.7
 Summary: Password Manager
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>, Sairam Pimple <sairampimple003@gmail.com>, Shubham Narendra Singh <shubh1122000@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -131,15 +131,15 @@
 - cryptography
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man==1.0.6
+pip install pasta-man==1.0.7
 ```
 
 ## README before [#Usage](#usage)
 
 After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man>=1.0.4` -> `pasta-man` and `pasta-man-launcher`.
 
 - `pasta-man` Command
```

### Comparing `pasta_man-1.0.6/README.md` & `pasta_man-1.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 - cryptography
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man==1.0.6
+pip install pasta-man==1.0.7
 ```
 
 ## README before [#Usage](#usage)
 
 After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man>=1.0.4` -> `pasta-man` and `pasta-man-launcher`.
 
 - `pasta-man` Command
```

### Comparing `pasta_man-1.0.6/pyproject.toml` & `pasta_man-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pasta-man"
-version = "1.0.6"
+version = "1.0.7"
 description = "Password Manager"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Software Development",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `pasta_man-1.0.6/src/pasta_man/architectures/gui.py` & `pasta_man-1.0.7/src/pasta_man/architectures/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         
         self._makeFetch_()
     
     
     def copyToClipboard(self):
         
         # prepare alleged pass
-        allegedpass = simpledialog.askstring("Master Password", "Enter Master Password to copy password to clipboard: ")
+        allegedpass = simpledialog.askstring("Master Password", "Enter Master Password to copy password to clipboard: ", show='-')
         
         # get masterpass
         with open(jPath(str(Path.home()), '.pastaman', '.m'), 'rb') as m:
             masterpassword = m.read() # this is encrypted
         
         def decryptthread(masterpassword: str):
             denc = Encryption("pastaman".encode('ascii'), masterpassword.encode('ascii'))
```

### Comparing `pasta_man-1.0.6/src/pasta_man/architectures/targets.py` & `pasta_man-1.0.7/src/pasta_man/architectures/targets.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.6/src/pasta_man/encryption.py` & `pasta_man-1.0.7/src/pasta_man/encryption.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.6/src/pasta_man/pasta_man.py` & `pasta_man-1.0.7/src/pasta_man/pasta_man.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 # version info
-__version__ = "1.0.6"
+__version__ = "1.0.7"
 
 # import project specific modules
 from pasta_man.architectures.gui import pmanager
 from pasta_man.encryption import Encryption
 from pasta_man.exceptions import NoneTypeVariable, OptError
 from pasta_man.utilities.helptext import helptext
 
@@ -34,15 +34,15 @@
     dencb = denc.__unencryptedstring__
     sys.exit(0)
 
 def checkmfile(home = str(Path.home())) -> bytes:
     # --> find out if master password is defined -> .m file
     if not there(jPath(home, '.pastaman', '.m')):
         # ask dialog
-        masterpassword = simpledialog.askstring("User Input", "Enter Master Password: ")
+        masterpassword = simpledialog.askstring("User Input", "Enter Master Password: ", show='-')
         # check if it is empty or non
         if masterpassword=='' or masterpassword==None:
             raise NoneTypeVariable('Aborted.')
         # encode it
         masterpassword = masterpassword.encode('ascii')
         enct = threading.Thread(target=locker, args=(masterpassword.decode('ascii'),))
         enct.start()
```

### Comparing `pasta_man-1.0.6/src/pasta_man/self_launch_thread/Launcher.py` & `pasta_man-1.0.7/src/pasta_man/self_launch_thread/Launcher.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.6/src/pasta_man/utilities/helptext.py` & `pasta_man-1.0.7/src/pasta_man/utilities/helptext.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.6/src/pasta_man/utilities/pasta_menu.py` & `pasta_man-1.0.7/src/pasta_man/utilities/pasta_menu.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.6/src/pasta_man.egg-info/PKG-INFO` & `pasta_man-1.0.7/src/pasta_man.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta-man
-Version: 1.0.6
+Version: 1.0.7
 Summary: Password Manager
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>, Sairam Pimple <sairampimple003@gmail.com>, Shubham Narendra Singh <shubh1122000@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -131,15 +131,15 @@
 - cryptography
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man==1.0.6
+pip install pasta-man==1.0.7
 ```
 
 ## README before [#Usage](#usage)
 
 After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man>=1.0.4` -> `pasta-man` and `pasta-man-launcher`.
 
 - `pasta-man` Command
```

### Comparing `pasta_man-1.0.6/src/pasta_man.egg-info/SOURCES.txt` & `pasta_man-1.0.7/src/pasta_man.egg-info/SOURCES.txt`

 * *Files identical despite different names*

