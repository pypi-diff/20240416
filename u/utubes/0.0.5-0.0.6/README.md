# Comparing `tmp/utubes-0.0.5.tar.gz` & `tmp/utubes-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utubes-0.0.5.tar", last modified: Tue Apr 16 11:50:03 2024, max compression
+gzip compressed data, was "utubes-0.0.6.tar", last modified: Tue Apr 16 14:09:51 2024, max compression
```

## Comparing `utubes-0.0.5.tar` & `utubes-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:50:03.114731 utubes-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 11:49:55.000000 utubes-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-16 11:50:03.114731 utubes-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-16 11:49:55.000000 utubes-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:50:03.114731 utubes-0.0.5/Utube/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 11:49:55.000000 utubes-0.0.5/Utube/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:50:03.114731 utubes-0.0.5/Utube/functions/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 11:49:55.000000 utubes-0.0.5/Utube/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-16 11:49:55.000000 utubes-0.0.5/Utube/functions/function01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:50:03.114731 utubes-0.0.5/Utube/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 11:49:55.000000 utubes-0.0.5/Utube/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 11:49:55.000000 utubes-0.0.5/Utube/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-16 11:49:55.000000 utubes-0.0.5/Utube/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 11:50:03.114731 utubes-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-16 11:49:55.000000 utubes-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:50:03.114731 utubes-0.0.5/utubes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-16 11:50:03.000000 utubes-0.0.5/utubes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-16 11:50:03.000000 utubes-0.0.5/utubes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 11:50:03.000000 utubes-0.0.5/utubes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 11:50:02.000000 utubes-0.0.5/utubes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 11:50:03.000000 utubes-0.0.5/utubes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:09:51.276024 utubes-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 14:09:46.000000 utubes-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-16 14:09:51.276024 utubes-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-16 14:09:46.000000 utubes-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:09:51.272024 utubes-0.0.6/Utube/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 14:09:46.000000 utubes-0.0.6/Utube/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:09:51.272024 utubes-0.0.6/Utube/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 14:09:46.000000 utubes-0.0.6/Utube/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-16 14:09:46.000000 utubes-0.0.6/Utube/functions/function01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:09:51.276024 utubes-0.0.6/Utube/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 14:09:46.000000 utubes-0.0.6/Utube/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:09:46.000000 utubes-0.0.6/Utube/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-16 14:09:46.000000 utubes-0.0.6/Utube/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:09:51.276024 utubes-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-16 14:09:46.000000 utubes-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:09:51.276024 utubes-0.0.6/utubes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-16 14:09:51.000000 utubes-0.0.6/utubes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-16 14:09:51.000000 utubes-0.0.6/utubes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:09:51.000000 utubes-0.0.6/utubes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:09:51.000000 utubes-0.0.6/utubes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 14:09:51.000000 utubes-0.0.6/utubes.egg-info/top_level.txt
```

### Comparing `utubes-0.0.5/LICENSE` & `utubes-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `utubes-0.0.5/PKG-INFO` & `utubes-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utubes
-Version: 0.0.5
+Version: 0.0.6
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
-Metadata-Version: 2.1 Name: utubes Version: 0.0.5 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: utubes Version: 0.0.6 Summary: ã¤ Home-page:
 https://github.com/Monisha License: MIT Keywords: python,youtube,extension
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: License :: OSI Approved
```

### Comparing `utubes-0.0.5/Utube/functions/function01.py` & `utubes-0.0.6/Utube/functions/function01.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 import asyncio
 from ..scripts.eo import Okeys
 from yt_dlp import YoutubeDL, DownloadError
 #=================================================================================================
 
+class UDMessages:
+    def __init__(self, **kwargs):
+        self.status = kwargs.get('status', True)
+        self.errors = kwargs.get('errors', None)
+        self.finame = kwargs.get('finame', None)
+        self.result = kwargs.get('result', None)
+
+#=================================================================================================
+
 class UDownloader:
 
     def __init__(self):
-        self.fnames = None
+        self.finame = None
         self.result = None
         self.errors = None
         self.status = True
         self.downdl = Okeys.DATA01
-        self.runnes = asyncio.get_event_loop()
 
 #=================================================================================================
     
-    def download(self, link, command, progress):
+    async def download(self, link, command, progress):
+        loop = asyncio.get_event_loop()
         with YoutubeDL(command) as ydl:
             try:
                 filelink = [link]
-                ydl.add_progress_hook(progress)
-                ydl.download(filelink)
+                ydl.add_progress_hook(progress)   
+                await loop.run_in_executor(None, ydl.download, filelink)
                 return self.status
             except DownloadError as errors:
                 self.errors = errors
                 self.status = False
                 return self.status
             except Exception as errors:
                 self.errors = errors
@@ -40,31 +49,31 @@
 
 #=================================================================================================
 
     async def extinfos(self, link, command):
         with YoutubeDL(command) as ydl:
             try:
                 self.result = ydl.extract_info(link, download=False)
-                return self.result
+                return UDMessages(result=self.result)
             except Exception as errors:
                 self.errors = errors
-                return self.errors
+                return UDMessages(errors=self.errors)
 
 #=================================================================================================
 
     async def filename(self, link, command):
         with YoutubeDL(command) as ydl:
             try:
                 masteredata = await self.metadata(link, command)
-                self.fnames = ydl.prepare_filename(masteredata, outtmpl=self.downdl)
-                return self.fnames
+                self.finame = ydl.prepare_filename(masteredata, outtmpl=self.downdl)
+                return UDMessages(finame=self.finame)
             except Exception as errors:
                 self.errors = errors
-                return self.fnames
+                return UDMessages(errors=self.errors)
 
 #=================================================================================================
 
     async def start(self, link, command, progress):
-        mainou = await self.runnes.run_in_executor(None, self.download, link, command, progress)
-        return mainou
+        mainou = await self.download(link, command, progress)
+        return UDMessages(status=mainou, errors=self.errors)
 
 #=================================================================================================
```

### Comparing `utubes-0.0.5/setup.py` & `utubes-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `utubes-0.0.5/utubes.egg-info/PKG-INFO` & `utubes-0.0.6/utubes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utubes
-Version: 0.0.5
+Version: 0.0.6
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
-Metadata-Version: 2.1 Name: utubes Version: 0.0.5 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: utubes Version: 0.0.6 Summary: ã¤ Home-page:
 https://github.com/Monisha License: MIT Keywords: python,youtube,extension
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: License :: OSI Approved
```

