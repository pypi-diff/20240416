# Comparing `tmp/osparc_filecomms-0.9.dev3-py2.py3-none-any.whl.zip` & `tmp/osparc_filecomms-0.9.dev5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4361 bytes, number of entries: 8
--rw-r--r--  2.0 unx       65 b- defN 24-Feb-06 07:32 osparc_filecomms/__init__.py
--rw-r--r--  2.0 unx      419 b- defN 24-Feb-06 07:32 osparc_filecomms/_version.py
--rw-r--r--  2.0 unx     5532 b- defN 24-Feb-06 07:32 osparc_filecomms/handshakers.py
--rw-r--r--  2.0 unx      678 b- defN 24-Feb-06 07:32 osparc_filecomms-0.9.dev3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1111 b- defN 24-Feb-06 07:32 osparc_filecomms-0.9.dev3.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Feb-06 07:32 osparc_filecomms-0.9.dev3.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 24-Feb-06 07:32 osparc_filecomms-0.9.dev3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      705 b- defN 24-Feb-06 07:32 osparc_filecomms-0.9.dev3.dist-info/RECORD
-8 files, 8637 bytes uncompressed, 3111 bytes compressed:  64.0%
+Zip file size: 4363 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       65 b- defN 24-Feb-06 07:48 osparc_filecomms/__init__.py
+-rw-r--r--  2.0 unx      419 b- defN 24-Feb-06 07:48 osparc_filecomms/_version.py
+-rw-r--r--  2.0 unx     5630 b- defN 24-Feb-06 07:48 osparc_filecomms/handshakers.py
+-rw-r--r--  2.0 unx      678 b- defN 24-Feb-06 07:48 osparc_filecomms-0.9.dev5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1111 b- defN 24-Feb-06 07:48 osparc_filecomms-0.9.dev5.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Feb-06 07:48 osparc_filecomms-0.9.dev5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 24-Feb-06 07:48 osparc_filecomms-0.9.dev5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      705 b- defN 24-Feb-06 07:48 osparc_filecomms-0.9.dev5.dist-info/RECORD
+8 files, 8735 bytes uncompressed, 3113 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: osparc_filecomms/_version.py
 Comment: 
 
 Filename: osparc_filecomms/handshakers.py
 Comment: 
 
-Filename: osparc_filecomms-0.9.dev3.dist-info/LICENSE.txt
+Filename: osparc_filecomms-0.9.dev5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: osparc_filecomms-0.9.dev3.dist-info/METADATA
+Filename: osparc_filecomms-0.9.dev5.dist-info/METADATA
 Comment: 
 
-Filename: osparc_filecomms-0.9.dev3.dist-info/WHEEL
+Filename: osparc_filecomms-0.9.dev5.dist-info/WHEEL
 Comment: 
 
-Filename: osparc_filecomms-0.9.dev3.dist-info/top_level.txt
+Filename: osparc_filecomms-0.9.dev5.dist-info/top_level.txt
 Comment: 
 
-Filename: osparc_filecomms-0.9.dev3.dist-info/RECORD
+Filename: osparc_filecomms-0.9.dev5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## osparc_filecomms/_version.py

```diff
@@ -8,9 +8,9 @@
     VERSION_TUPLE = object
 
 version: str
 __version__: str
 __version_tuple__: VERSION_TUPLE
 version_tuple: VERSION_TUPLE
 
-__version__ = version = '0.9.dev3'
-__version_tuple__ = version_tuple = (0, 9, 'dev3')
+__version__ = version = '0.9.dev5'
+__version_tuple__ = version_tuple = (0, 9, 'dev5')
```

## osparc_filecomms/handshakers.py

```diff
@@ -2,15 +2,15 @@
 import json
 import time
 import pathlib as pl
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
-POLLING_INTERVAL = .1  # second
+POLLING_INTERVAL = 0.1  # second
 PRINT_POLLING_INTERVAL = 100  # number of polls before print
 
 
 class FileHandshaker:
     def __init__(
         self,
         self_uuid: str,
@@ -42,14 +42,17 @@
         self.handshake_input_path = (
             self.input_dir_path / self.handshake_filename
         )
 
     def shake(self):
         """Perform handshake with other service"""
 
+        if self.handshake_output_path.exists():
+            self.handshake_output_path.unlink()
+
         if self.is_initiator:
             return self.shake_initiator()
         else:
             return self.shake_receiver()
 
     def shake_initiator(self):
         """Shake hand by initiator"""
```

## Comparing `osparc_filecomms-0.9.dev3.dist-info/LICENSE.txt` & `osparc_filecomms-0.9.dev5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `osparc_filecomms-0.9.dev3.dist-info/METADATA` & `osparc_filecomms-0.9.dev5.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osparc_filecomms
-Version: 0.9.dev3
+Version: 0.9.dev5
 Summary: oSparc file communications
 Author: Werner Van Geit @ IT'IS Zurich
 License: Copyright (C) IT'IS Foundation - All Rights Reserved
         
         Written by Werner Van Geit <vangeit at itis.swiss>, 2023
         
         Unless required by applicable law or agreed to in writing,
```

