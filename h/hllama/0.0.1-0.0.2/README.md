# Comparing `tmp/hllama-0.0.1-py3-none-any.whl.zip` & `tmp/hllama-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6078 bytes, number of entries: 7
--rw-rw-r--  2.0 unx       52 b- defN 24-Apr-16 01:22 hllama/__init__.py
+Zip file size: 6079 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx       52 b- defN 24-Apr-16 01:27 hllama/__init__.py
 -rw-rw-r--  2.0 unx     1006 b- defN 24-Apr-16 01:05 hllama/json_utils.py
--rw-rw-r--  2.0 unx    11357 b- defN 24-Apr-16 01:23 hllama-0.0.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx      643 b- defN 24-Apr-16 01:23 hllama-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-16 01:23 hllama-0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 24-Apr-16 01:23 hllama-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      530 b- defN 24-Apr-16 01:23 hllama-0.0.1.dist-info/RECORD
-7 files, 13687 bytes uncompressed, 5140 bytes compressed:  62.4%
+-rw-rw-r--  2.0 unx    11357 b- defN 24-Apr-16 01:28 hllama-0.0.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      643 b- defN 24-Apr-16 01:28 hllama-0.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-16 01:28 hllama-0.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 24-Apr-16 01:28 hllama-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      530 b- defN 24-Apr-16 01:28 hllama-0.0.2.dist-info/RECORD
+7 files, 13687 bytes uncompressed, 5141 bytes compressed:  62.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: hllama/__init__.py
 Comment: 
 
 Filename: hllama/json_utils.py
 Comment: 
 
-Filename: hllama-0.0.1.dist-info/LICENSE
+Filename: hllama-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: hllama-0.0.1.dist-info/METADATA
+Filename: hllama-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: hllama-0.0.1.dist-info/WHEEL
+Filename: hllama-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: hllama-0.0.1.dist-info/top_level.txt
+Filename: hllama-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: hllama-0.0.1.dist-info/RECORD
+Filename: hllama-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hllama/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 
 from hllama import json_utils
```

## Comparing `hllama-0.0.1.dist-info/LICENSE` & `hllama-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hllama-0.0.1.dist-info/METADATA` & `hllama-0.0.2.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hllama
-Version: 0.0.1
+Version: 0.0.2
 Summary: hllama provides some useful utility functions for LLM.
 Home-page: https://github.com/deep-diver/llmtoolbox
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: LLM,Large Language Model,Verification,Utility
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

