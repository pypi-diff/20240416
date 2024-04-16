# Comparing `tmp/client_onedoc-0.0.8.tar.gz` & `tmp/client_onedoc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "client_onedoc-0.0.8.tar", last modified: Thu Mar 14 22:50:56 2024, max compression
+gzip compressed data, was "client_onedoc-0.0.9.tar", last modified: Thu Mar 14 23:07:52 2024, max compression
```

## Comparing `client_onedoc-0.0.8.tar` & `client_onedoc-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:50:56.903397 client_onedoc-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-03-14 22:50:56.903397 client_onedoc-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-03-14 22:50:43.000000 client_onedoc-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:50:56.903397 client_onedoc-0.0.8/client_onedoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-03-14 22:50:56.000000 client_onedoc-0.0.8/client_onedoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-14 22:50:56.000000 client_onedoc-0.0.8/client_onedoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 22:50:56.000000 client_onedoc-0.0.8/client_onedoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-14 22:50:56.000000 client_onedoc-0.0.8/client_onedoc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-14 22:50:56.000000 client_onedoc-0.0.8/client_onedoc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:50:56.903397 client_onedoc-0.0.8/onedoc/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-14 22:50:43.000000 client_onedoc-0.0.8/onedoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-03-14 22:50:43.000000 client_onedoc-0.0.8/onedoc/html_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-03-14 22:50:43.000000 client_onedoc-0.0.8/onedoc/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-03-14 22:50:43.000000 client_onedoc-0.0.8/onedoc/onedoc.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-14 22:50:43.000000 client_onedoc-0.0.8/onedoc/split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-03-14 22:50:43.000000 client_onedoc-0.0.8/onedoc/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-14 22:50:54.000000 client_onedoc-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 22:50:56.903397 client_onedoc-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 23:07:52.659750 client_onedoc-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-03-14 23:07:52.659750 client_onedoc-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-03-14 23:07:41.000000 client_onedoc-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 23:07:52.659750 client_onedoc-0.0.9/client_onedoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-03-14 23:07:52.000000 client_onedoc-0.0.9/client_onedoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-14 23:07:52.000000 client_onedoc-0.0.9/client_onedoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 23:07:52.000000 client_onedoc-0.0.9/client_onedoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-14 23:07:52.000000 client_onedoc-0.0.9/client_onedoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-14 23:07:52.000000 client_onedoc-0.0.9/client_onedoc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 23:07:52.659750 client_onedoc-0.0.9/onedoc/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-14 23:07:41.000000 client_onedoc-0.0.9/onedoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-03-14 23:07:41.000000 client_onedoc-0.0.9/onedoc/html_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-03-14 23:07:41.000000 client_onedoc-0.0.9/onedoc/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-03-14 23:07:41.000000 client_onedoc-0.0.9/onedoc/onedoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-14 23:07:41.000000 client_onedoc-0.0.9/onedoc/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-03-14 23:07:41.000000 client_onedoc-0.0.9/onedoc/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-14 23:07:50.000000 client_onedoc-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 23:07:52.659750 client_onedoc-0.0.9/setup.cfg
```

### Comparing `client_onedoc-0.0.8/PKG-INFO` & `client_onedoc-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: client_onedoc
-Version: 0.0.8
+Version: 0.0.9
 Summary: Onedoc SDK for Python
 Author-email: Pierre Dorge <pierre.dorge@onedoclabs.com>, Titouan Launay <titouan.launay@onedoclabs.com>
 Project-URL: Homepage, https://github.com/onedoclabs/onedoc
 Project-URL: Issues, https://github.com/OnedocLabs/onedoc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: client_onedoc Version: 0.0.8 Summary: Onedoc SDK
+Metadata-Version: 2.1 Name: client_onedoc Version: 0.0.9 Summary: Onedoc SDK
 for Python Author-email: Pierre Dorge
 onedoclabs.com>, Titouan Launay
 onedoclabs.com> Project-URL: Homepage, https://github.com/onedoclabs/onedoc
 Project-URL: Issues, https://github.com/OnedocLabs/onedoc/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown Requires-Dist: requests>=2.0 Requires-
```

### Comparing `client_onedoc-0.0.8/README.md` & `client_onedoc-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `client_onedoc-0.0.8/client_onedoc.egg-info/PKG-INFO` & `client_onedoc-0.0.9/client_onedoc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: client_onedoc
-Version: 0.0.8
+Version: 0.0.9
 Summary: Onedoc SDK for Python
 Author-email: Pierre Dorge <pierre.dorge@onedoclabs.com>, Titouan Launay <titouan.launay@onedoclabs.com>
 Project-URL: Homepage, https://github.com/onedoclabs/onedoc
 Project-URL: Issues, https://github.com/OnedocLabs/onedoc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: client_onedoc Version: 0.0.8 Summary: Onedoc SDK
+Metadata-Version: 2.1 Name: client_onedoc Version: 0.0.9 Summary: Onedoc SDK
 for Python Author-email: Pierre Dorge
 onedoclabs.com>, Titouan Launay
 onedoclabs.com> Project-URL: Homepage, https://github.com/onedoclabs/onedoc
 Project-URL: Issues, https://github.com/OnedocLabs/onedoc/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown Requires-Dist: requests>=2.0 Requires-
```

### Comparing `client_onedoc-0.0.8/onedoc/html_builder.py` & `client_onedoc-0.0.9/onedoc/html_builder.py`

 * *Files identical despite different names*

### Comparing `client_onedoc-0.0.8/onedoc/merge.py` & `client_onedoc-0.0.9/onedoc/merge.py`

 * *Files identical despite different names*

### Comparing `client_onedoc-0.0.8/onedoc/onedoc.py` & `client_onedoc-0.0.9/onedoc/onedoc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import requests
 import json
 
 from pikepdf import Pdf
 
-from .html_builder import _HtmlBuilder
-from .merge import merge as lib_merge
-from .split import split as lib_split
+from html_builder import _HtmlBuilder
+from merge import merge as lib_merge
+from split import split as lib_split
 
-from typing import Dict, Tuple, Union, List, Any, BinaryIO
+from typing import Dict, Tuple, Any, BinaryIO
 
 DEFAULT_FILE_OPTIONS = {
     "cacheControl": "3600",
     "contentType": "text/plain;charset=UTF-8",
     "upsert": False,
 }
```

### Comparing `client_onedoc-0.0.8/onedoc/split.py` & `client_onedoc-0.0.9/onedoc/split.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     :param page: The page number to split at. Pages before and including this page will be in the first document, and pages after will be in the second document.
     :return: A tuple containing the two split PDF documents.
     """
     pdf = Pdf.open(doc)
     pdf_a = Pdf.new()
     pdf_b = Pdf.new()
 
-    for i, page in enumerate(pdf.pages):
+    i = 0
+
+    for i, pdf_page in enumerate(pdf.pages):
         if i < page:
-            pdf_a.pages.append(page)
+            pdf_a.pages.append(pdf_page)
         else:
-            pdf_b.pages.append(page)
+            pdf_b.pages.append(pdf_page)
 
     return pdf_a, pdf_b
```

### Comparing `client_onedoc-0.0.8/onedoc/test.py` & `client_onedoc-0.0.9/onedoc/test.py`

 * *Files identical despite different names*

### Comparing `client_onedoc-0.0.8/pyproject.toml` & `client_onedoc-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "client_onedoc"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Pierre Dorge", email="pierre.dorge@onedoclabs.com" },
   { name="Titouan Launay", email="titouan.launay@onedoclabs.com" },
 ]
 description = "Onedoc SDK for Python"
 readme = "README.md"
 requires-python = ">=3.8"
```

