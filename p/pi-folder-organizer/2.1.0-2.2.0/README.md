# Comparing `tmp/pi-folder-organizer-2.1.0.tar.gz` & `tmp/pi_folder_organizer-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pi-folder-organizer-2.1.0.tar", last modified: Fri Apr 12 15:20:56 2024, max compression
+gzip compressed data, was "pi_folder_organizer-2.2.0.tar", last modified: Tue Apr 16 15:58:00 2024, max compression
```

## Comparing `pi-folder-organizer-2.1.0.tar` & `pi_folder_organizer-2.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:20:56.378634 pi-folder-organizer-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-12 15:20:52.000000 pi-folder-organizer-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-12 15:20:56.378634 pi-folder-organizer-2.1.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2536 2024-04-12 15:20:52.000000 pi-folder-organizer-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:20:56.378634 pi-folder-organizer-2.1.0/pi_folder_organizer/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-12 15:20:52.000000 pi-folder-organizer-2.1.0/pi_folder_organizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-12 15:20:52.000000 pi-folder-organizer-2.1.0/pi_folder_organizer/_exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13779 2024-04-12 15:20:52.000000 pi-folder-organizer-2.1.0/pi_folder_organizer/pi_folder_organizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:20:56.378634 pi-folder-organizer-2.1.0/pi_folder_organizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-12 15:20:56.000000 pi-folder-organizer-2.1.0/pi_folder_organizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-12 15:20:56.000000 pi-folder-organizer-2.1.0/pi_folder_organizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:20:56.000000 pi-folder-organizer-2.1.0/pi_folder_organizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 15:20:56.000000 pi-folder-organizer-2.1.0/pi_folder_organizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:20:56.378634 pi-folder-organizer-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-12 15:20:52.000000 pi-folder-organizer-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:58:00.793553 pi_folder_organizer-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 15:57:57.000000 pi_folder_organizer-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-16 15:58:00.793553 pi_folder_organizer-2.2.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2536 2024-04-16 15:57:57.000000 pi_folder_organizer-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:58:00.793553 pi_folder_organizer-2.2.0/pi_folder_organizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-16 15:57:57.000000 pi_folder_organizer-2.2.0/pi_folder_organizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-16 15:57:57.000000 pi_folder_organizer-2.2.0/pi_folder_organizer/_exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13754 2024-04-16 15:57:57.000000 pi_folder_organizer-2.2.0/pi_folder_organizer/pi_folder_organizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:58:00.793553 pi_folder_organizer-2.2.0/pi_folder_organizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-16 15:58:00.000000 pi_folder_organizer-2.2.0/pi_folder_organizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-16 15:58:00.000000 pi_folder_organizer-2.2.0/pi_folder_organizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:58:00.000000 pi_folder_organizer-2.2.0/pi_folder_organizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 15:58:00.000000 pi_folder_organizer-2.2.0/pi_folder_organizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:58:00.793553 pi_folder_organizer-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-16 15:57:57.000000 pi_folder_organizer-2.2.0/setup.py
```

### Comparing `pi-folder-organizer-2.1.0/LICENSE` & `pi_folder_organizer-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pi-folder-organizer-2.1.0/PKG-INFO` & `pi_folder_organizer-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pi-folder-organizer
-Version: 2.1.0
+Version: 2.2.0
 Summary: A Python package for cleaning up cluttered files and organizing them into respective folders.
 Author: Qadeer Ahmad
 Author-email: mrqdeer1231122@gmail.com
 Keywords: python,file organization,file cleanup,cluttered files,folder management,data organization,file management,data cleanup,Python package,developer tools,data processing,file sorting,data structuring,automated file organization,Python library,data management,data handling,file optimization,data optimization
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pi-folder-organizer-2.1.0/README.md` & `pi_folder_organizer-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pi-folder-organizer-2.1.0/pi_folder_organizer/pi_folder_organizer.py` & `pi_folder_organizer-2.2.0/pi_folder_organizer/pi_folder_organizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,16 @@
                 "CodeFiles": [],
                 "ConfigurationFiles": [],
                 "SystemFiles": [],
                 "DatabaseFiles": [],
                 "LogFiles":[],
                 "FontsFiles":[],
                 "SerializedFiles": [],
-                "WebFiles": [],
-                "GitRepos": [],
+                "WebURLs": [],
+                
                 "AndroidAPKs": [],
                 "ISOsFiles":[],
                 "VirtualMachinesFiles":[],
                 "JupyterNotebooks":[],
                 "Others": []
             }
 
@@ -88,25 +88,25 @@
                 "MacSoftwares": (".app", ".dmg", ".pkg", ".bin", ".out", ".command",),
                 "CodeFiles": (".py",".nb",".php",".rb",".pl",".sh", ".js", ".html", ".css", ".m",".mlx", ".mojo", ".ts", ".cpp",".java",".c",".mltbx"),
                 "ConfigurationFiles": (".yaml",".yml",".config",".ini",".cfg","LICENSE",".cmd",".xml"),
                 "SystemFiles":('Dockerfile', '.gitignore', '.htaccess', 'hosts', 'fstab'),
                 "LogFiles": (".log",".syslog",".eventlog"),
                 "FontsFiles": (".woff",".woff2",".otf",".ttf",".ps",".pfb",".pfm",".font"),
                 "DatabaseFiles": (".sqlite",".db",".sql"),
-                "WebFiles": (".html",".htm",".shtml", ".xhtml"),
-                "GitRepos": (".git"),
+                "WebURLs": (".html",".htm",".shtml", ".xhtml"),
+                
                 "AndroidAPKs": (".apk",".xapk"),
                 "ISOsFiles": (".iso"),
                 "JupyterNotebooks": (".ipynb"),
                 "VirtualMachinesFiles": (".vbox-extpack",'.vdi', '.vmdk', '.vhd', '.vhdx', 
                         '.vdi.bz2', '.vmdk.gz', '.vhd.gz',
                         '.vbox', '.vbox-prev', '.vbox-extpack', '.ovf', '.ova',
                         '.vbox-snAPSHOT', '.sav',
                         '.log','.vbox-tmp', '.vdi-tmp', '.cdr'),
-                "SerializedFiles": (".json", ".pkl", ".npy", ".joblib")
+                "SerializedFiles": (".json", ".pkl", ".npy", ".joblib",".pth",".h5")
             }
 
     @staticmethod
     def __list_files(folder_path):
         files = []
         for dirpath, _, filenames in os.walk(folder_path):
             for file in filenames:
```

### Comparing `pi-folder-organizer-2.1.0/pi_folder_organizer.egg-info/PKG-INFO` & `pi_folder_organizer-2.2.0/pi_folder_organizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pi-folder-organizer
-Version: 2.1.0
+Version: 2.2.0
 Summary: A Python package for cleaning up cluttered files and organizing them into respective folders.
 Author: Qadeer Ahmad
 Author-email: mrqdeer1231122@gmail.com
 Keywords: python,file organization,file cleanup,cluttered files,folder management,data organization,file management,data cleanup,Python package,developer tools,data processing,file sorting,data structuring,automated file organization,Python library,data management,data handling,file optimization,data optimization
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pi-folder-organizer-2.1.0/setup.py` & `pi_folder_organizer-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '2.1.0'
+VERSION = '2.2.0'
 DESCRIPTION = "A Python package for cleaning up cluttered files and organizing them into respective folders."
 # Setting up
 setup(
     name="pi-folder-organizer",
     version=VERSION,
     author="Qadeer Ahmad",
     author_email="mrqdeer1231122@gmail.com",
```

