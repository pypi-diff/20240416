# Comparing `tmp/utubes-0.0.4.tar.gz` & `tmp/utubes-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utubes-0.0.4.tar", last modified: Mon Apr 15 17:06:45 2024, max compression
+gzip compressed data, was "utubes-0.0.5.tar", last modified: Tue Apr 16 11:50:03 2024, max compression
```

## Comparing `utubes-0.0.4.tar` & `utubes-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:06:45.760714 utubes-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 17:06:39.000000 utubes-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-15 17:06:45.760714 utubes-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-15 17:06:39.000000 utubes-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:06:45.756714 utubes-0.0.4/Utube/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 17:06:39.000000 utubes-0.0.4/Utube/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:06:45.756714 utubes-0.0.4/Utube/functions/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-15 17:06:39.000000 utubes-0.0.4/Utube/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-15 17:06:39.000000 utubes-0.0.4/Utube/functions/function01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:06:45.756714 utubes-0.0.4/Utube/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 17:06:39.000000 utubes-0.0.4/Utube/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 17:06:39.000000 utubes-0.0.4/Utube/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-15 17:06:39.000000 utubes-0.0.4/Utube/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 17:06:45.760714 utubes-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-15 17:06:39.000000 utubes-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:06:45.760714 utubes-0.0.4/utubes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-15 17:06:45.000000 utubes-0.0.4/utubes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-15 17:06:45.000000 utubes-0.0.4/utubes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 17:06:45.000000 utubes-0.0.4/utubes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 17:06:45.000000 utubes-0.0.4/utubes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 17:06:45.000000 utubes-0.0.4/utubes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:50:03.114731 utubes-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 11:49:55.000000 utubes-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-16 11:50:03.114731 utubes-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-16 11:49:55.000000 utubes-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:50:03.114731 utubes-0.0.5/Utube/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 11:49:55.000000 utubes-0.0.5/Utube/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:50:03.114731 utubes-0.0.5/Utube/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 11:49:55.000000 utubes-0.0.5/Utube/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-16 11:49:55.000000 utubes-0.0.5/Utube/functions/function01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:50:03.114731 utubes-0.0.5/Utube/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 11:49:55.000000 utubes-0.0.5/Utube/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 11:49:55.000000 utubes-0.0.5/Utube/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-16 11:49:55.000000 utubes-0.0.5/Utube/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 11:50:03.114731 utubes-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-16 11:49:55.000000 utubes-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:50:03.114731 utubes-0.0.5/utubes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-16 11:50:03.000000 utubes-0.0.5/utubes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-16 11:50:03.000000 utubes-0.0.5/utubes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 11:50:03.000000 utubes-0.0.5/utubes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 11:50:02.000000 utubes-0.0.5/utubes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 11:50:03.000000 utubes-0.0.5/utubes.egg-info/top_level.txt
```

### Comparing `utubes-0.0.4/LICENSE` & `utubes-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `utubes-0.0.4/PKG-INFO` & `utubes-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utubes
-Version: 0.0.4
+Version: 0.0.5
 Summary: ㅤ
 Home-page: https://github.com/Monisha
 License: MIT
 Keywords: python,youtube,extension
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: utubes Version: 0.0.4 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: utubes Version: 0.0.5 Summary: ã¤ Home-page:
 https://github.com/Monisha License: MIT Keywords: python,youtube,extension
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: License :: OSI Approved
```

### Comparing `utubes-0.0.4/Utube/functions/function01.py` & `utubes-0.0.5/Utube/functions/function01.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,70 @@
 import asyncio
 from ..scripts.eo import Okeys
 from yt_dlp import YoutubeDL, DownloadError
-#======================================================================================================
+#=================================================================================================
 
-class Utube:
+class UDownloader:
 
     def __init__(self):
         self.fnames = None
         self.result = None
         self.errors = None
         self.status = True
         self.downdl = Okeys.DATA01
         self.runnes = asyncio.get_event_loop()
 
-#======================================================================================================
-
+#=================================================================================================
+    
     def download(self, link, command, progress):
         with YoutubeDL(command) as ydl:
             try:
                 filelink = [link]
                 ydl.add_progress_hook(progress)
                 ydl.download(filelink)
-            except DownloadError as erros:
-                self.errors = erros
+                return self.status
+            except DownloadError as errors:
+                self.errors = errors
                 self.status = False
-            except Exception as erros:
-                self.errors = erros
+                return self.status
+            except Exception as errors:
+                self.errors = errors
                 self.status = False
+                return self.status
 
-            return self.status
+#=================================================================================================
 
-#======================================================================================================
-    
     async def metadata(self, link, command):
         with YoutubeDL(command) as ydl:
             self.result = ydl.extract_info(link, download=False)
             return self.result
 
-#======================================================================================================
+#=================================================================================================
 
     async def extinfos(self, link, command):
         with YoutubeDL(command) as ydl:
             try:
                 self.result = ydl.extract_info(link, download=False)
-            except Exception as erros:
-                self.errors = erros
+                return self.result
+            except Exception as errors:
+                self.errors = errors
+                return self.errors
 
-            return self.result
-
-#======================================================================================================
+#=================================================================================================
 
     async def filename(self, link, command):
         with YoutubeDL(command) as ydl:
             try:
                 masteredata = await self.metadata(link, command)
                 self.fnames = ydl.prepare_filename(masteredata, outtmpl=self.downdl)
-            except Exception:
-                self.fnames = None
-
-            return self.fnames
+                return self.fnames
+            except Exception as errors:
+                self.errors = errors
+                return self.fnames
 
-#======================================================================================================
+#=================================================================================================
 
     async def start(self, link, command, progress):
         mainou = await self.runnes.run_in_executor(None, self.download, link, command, progress)
         return mainou
 
-#======================================================================================================
+#=================================================================================================
```

### Comparing `utubes-0.0.4/setup.py` & `utubes-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `utubes-0.0.4/utubes.egg-info/PKG-INFO` & `utubes-0.0.5/utubes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utubes
-Version: 0.0.4
+Version: 0.0.5
 Summary: ㅤ
 Home-page: https://github.com/Monisha
 License: MIT
 Keywords: python,youtube,extension
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: utubes Version: 0.0.4 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: utubes Version: 0.0.5 Summary: ã¤ Home-page:
 https://github.com/Monisha License: MIT Keywords: python,youtube,extension
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: License :: OSI Approved
```

