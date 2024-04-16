# Comparing `tmp/utubes-0.0.7.tar.gz` & `tmp/utubes-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utubes-0.0.7.tar", last modified: Tue Apr 16 15:15:14 2024, max compression
+gzip compressed data, was "utubes-0.0.8.tar", last modified: Tue Apr 16 20:21:51 2024, max compression
```

## Comparing `utubes-0.0.7.tar` & `utubes-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:15:14.382425 utubes-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 15:15:09.000000 utubes-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-16 15:15:14.382425 utubes-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-16 15:15:09.000000 utubes-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:15:14.378425 utubes-0.0.7/Utube/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 15:15:09.000000 utubes-0.0.7/Utube/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:15:14.378425 utubes-0.0.7/Utube/functions/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 15:15:09.000000 utubes-0.0.7/Utube/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-16 15:15:09.000000 utubes-0.0.7/Utube/functions/function01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:15:14.378425 utubes-0.0.7/Utube/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 15:15:09.000000 utubes-0.0.7/Utube/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:15:09.000000 utubes-0.0.7/Utube/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-16 15:15:09.000000 utubes-0.0.7/Utube/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:15:14.382425 utubes-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-16 15:15:09.000000 utubes-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:15:14.378425 utubes-0.0.7/utubes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-16 15:15:14.000000 utubes-0.0.7/utubes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-16 15:15:14.000000 utubes-0.0.7/utubes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:15:14.000000 utubes-0.0.7/utubes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:15:14.000000 utubes-0.0.7/utubes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 15:15:14.000000 utubes-0.0.7/utubes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:21:51.458017 utubes-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 20:21:47.000000 utubes-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-16 20:21:51.458017 utubes-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-16 20:21:47.000000 utubes-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:21:51.458017 utubes-0.0.8/Utube/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 20:21:47.000000 utubes-0.0.8/Utube/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:21:51.458017 utubes-0.0.8/Utube/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 20:21:47.000000 utubes-0.0.8/Utube/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-16 20:21:47.000000 utubes-0.0.8/Utube/functions/function01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:21:51.458017 utubes-0.0.8/Utube/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 20:21:47.000000 utubes-0.0.8/Utube/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:21:47.000000 utubes-0.0.8/Utube/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-16 20:21:47.000000 utubes-0.0.8/Utube/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 20:21:51.458017 utubes-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-16 20:21:47.000000 utubes-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:21:51.458017 utubes-0.0.8/utubes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-16 20:21:51.000000 utubes-0.0.8/utubes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-16 20:21:51.000000 utubes-0.0.8/utubes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:21:51.000000 utubes-0.0.8/utubes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:21:51.000000 utubes-0.0.8/utubes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 20:21:51.000000 utubes-0.0.8/utubes.egg-info/top_level.txt
```

### Comparing `utubes-0.0.7/LICENSE` & `utubes-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `utubes-0.0.7/PKG-INFO` & `utubes-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utubes
-Version: 0.0.7
+Version: 0.0.8
 Summary: ㅤ
 Home-page: https://github.com/Monisha
 License: MIT
 Keywords: python,youtube,extension
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -22,23 +22,25 @@
  📦 <a href="https://pypi.org/project/utubes" style="text-decoration:none;">YOUTUBE EXTENSIONS</a>
 </p>
 
 
 ## USAGE
 ```python
 async def main():
-    downloader = UDownloader()
-
     # EXAMPLE USAGE OF METHODS
     filelink = "YOUR_VIDEO_LINK"
-    progress = None  # YOUR PROGRESS HOOK FUNCTION
-    commands = {}    # YOUR COMMAND OPTIONS FOR YOUTUBEDL
+    progress = None # YOUR PROGRESS HOOK FUNCTION
+    commands = {"quiet": True, "no_warnings": True}
 
     # CALL METHODS USING AWAIT
-    metadata_result = await downloader.metadata(filelink, commands)
-    extinfos_result = await downloader.extracts(filelink, commands)
-    filename_result = await downloader.filename(filelink, commands)
-    download_result = await downloader.download(filelink, commands, progress)
+    metadata_result = await UDownloader.metadata(filelink, commands)
+    extinfos_result = await UDownloader.extracts(filelink, commands)
+    filename_result = await UDownloader.filename(filelink, commands)
+    download_result = await UDownloader.download(filelink, commands, progress)
+    print(metadata_result.result) # metadata_result.errors
+    print(extinfos_result.result) # extinfos_result.errors
+    print(filename_result.result) # filename_result.errors
+    print(download_result.status) # download_result.errors
     # DO SOMETHING WITH THE RESULTS
 
 asyncio.run(main())
 ```
```

#### html2text {}

```diff
@@ -1,19 +1,22 @@
-Metadata-Version: 2.1 Name: utubes Version: 0.0.7 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: utubes Version: 0.0.8 Summary: ã¤ Home-page:
 https://github.com/Monisha License: MIT Keywords: python,youtube,extension
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: License :: OSI Approved
 :: GNU Lesser General Public License v3 (LGPLv3) Requires-Python: ~=3.10
 Description-Content-Type: text/markdown License-File: LICENSE
                             ð¦ _Y_O_U_T_U_B_E_ _E_X_T_E_N_S_I_O_N_S
-## USAGE ```python async def main(): downloader = UDownloader() # EXAMPLE USAGE
-OF METHODS filelink = "YOUR_VIDEO_LINK" progress = None # YOUR PROGRESS HOOK
-FUNCTION commands = {} # YOUR COMMAND OPTIONS FOR YOUTUBEDL # CALL METHODS
-USING AWAIT metadata_result = await downloader.metadata(filelink, commands)
-extinfos_result = await downloader.extracts(filelink, commands) filename_result
-= await downloader.filename(filelink, commands) download_result = await
-downloader.download(filelink, commands, progress) # DO SOMETHING WITH THE
+## USAGE ```python async def main(): # EXAMPLE USAGE OF METHODS filelink =
+"YOUR_VIDEO_LINK" progress = None # YOUR PROGRESS HOOK FUNCTION commands =
+{"quiet": True, "no_warnings": True} # CALL METHODS USING AWAIT metadata_result
+= await UDownloader.metadata(filelink, commands) extinfos_result = await
+UDownloader.extracts(filelink, commands) filename_result = await
+UDownloader.filename(filelink, commands) download_result = await
+UDownloader.download(filelink, commands, progress) print
+(metadata_result.result) # metadata_result.errors print(extinfos_result.result)
+# extinfos_result.errors print(filename_result.result) # filename_result.errors
+print(download_result.status) # download_result.errors # DO SOMETHING WITH THE
 RESULTS asyncio.run(main()) ```
```

### Comparing `utubes-0.0.7/setup.py` & `utubes-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `utubes-0.0.7/utubes.egg-info/PKG-INFO` & `utubes-0.0.8/utubes.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utubes
-Version: 0.0.7
+Version: 0.0.8
 Summary: ㅤ
 Home-page: https://github.com/Monisha
 License: MIT
 Keywords: python,youtube,extension
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -22,23 +22,25 @@
  📦 <a href="https://pypi.org/project/utubes" style="text-decoration:none;">YOUTUBE EXTENSIONS</a>
 </p>
 
 
 ## USAGE
 ```python
 async def main():
-    downloader = UDownloader()
-
     # EXAMPLE USAGE OF METHODS
     filelink = "YOUR_VIDEO_LINK"
-    progress = None  # YOUR PROGRESS HOOK FUNCTION
-    commands = {}    # YOUR COMMAND OPTIONS FOR YOUTUBEDL
+    progress = None # YOUR PROGRESS HOOK FUNCTION
+    commands = {"quiet": True, "no_warnings": True}
 
     # CALL METHODS USING AWAIT
-    metadata_result = await downloader.metadata(filelink, commands)
-    extinfos_result = await downloader.extracts(filelink, commands)
-    filename_result = await downloader.filename(filelink, commands)
-    download_result = await downloader.download(filelink, commands, progress)
+    metadata_result = await UDownloader.metadata(filelink, commands)
+    extinfos_result = await UDownloader.extracts(filelink, commands)
+    filename_result = await UDownloader.filename(filelink, commands)
+    download_result = await UDownloader.download(filelink, commands, progress)
+    print(metadata_result.result) # metadata_result.errors
+    print(extinfos_result.result) # extinfos_result.errors
+    print(filename_result.result) # filename_result.errors
+    print(download_result.status) # download_result.errors
     # DO SOMETHING WITH THE RESULTS
 
 asyncio.run(main())
 ```
```

#### html2text {}

```diff
@@ -1,19 +1,22 @@
-Metadata-Version: 2.1 Name: utubes Version: 0.0.7 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: utubes Version: 0.0.8 Summary: ã¤ Home-page:
 https://github.com/Monisha License: MIT Keywords: python,youtube,extension
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: License :: OSI Approved
 :: GNU Lesser General Public License v3 (LGPLv3) Requires-Python: ~=3.10
 Description-Content-Type: text/markdown License-File: LICENSE
                             ð¦ _Y_O_U_T_U_B_E_ _E_X_T_E_N_S_I_O_N_S
-## USAGE ```python async def main(): downloader = UDownloader() # EXAMPLE USAGE
-OF METHODS filelink = "YOUR_VIDEO_LINK" progress = None # YOUR PROGRESS HOOK
-FUNCTION commands = {} # YOUR COMMAND OPTIONS FOR YOUTUBEDL # CALL METHODS
-USING AWAIT metadata_result = await downloader.metadata(filelink, commands)
-extinfos_result = await downloader.extracts(filelink, commands) filename_result
-= await downloader.filename(filelink, commands) download_result = await
-downloader.download(filelink, commands, progress) # DO SOMETHING WITH THE
+## USAGE ```python async def main(): # EXAMPLE USAGE OF METHODS filelink =
+"YOUR_VIDEO_LINK" progress = None # YOUR PROGRESS HOOK FUNCTION commands =
+{"quiet": True, "no_warnings": True} # CALL METHODS USING AWAIT metadata_result
+= await UDownloader.metadata(filelink, commands) extinfos_result = await
+UDownloader.extracts(filelink, commands) filename_result = await
+UDownloader.filename(filelink, commands) download_result = await
+UDownloader.download(filelink, commands, progress) print
+(metadata_result.result) # metadata_result.errors print(extinfos_result.result)
+# extinfos_result.errors print(filename_result.result) # filename_result.errors
+print(download_result.status) # download_result.errors # DO SOMETHING WITH THE
 RESULTS asyncio.run(main()) ```
```

