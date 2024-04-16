# Comparing `tmp/efriser-0.1.7.tar.gz` & `tmp/efriser-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efriser-0.1.7.tar", last modified: Mon Apr 15 06:00:16 2024, max compression
+gzip compressed data, was "efriser-0.1.8.tar", last modified: Tue Apr 16 09:13:40 2024, max compression
```

## Comparing `efriser-0.1.7.tar` & `efriser-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-15 06:00:16.813632 efriser-0.1.7/
--rw-rw-r--   0 douglas   (1000) douglas   (1000)     2357 2024-04-15 06:00:16.813632 efriser-0.1.7/PKG-INFO
--rw-rw-r--   0 douglas   (1000) douglas   (1000)     1871 2024-04-15 05:59:48.000000 efriser-0.1.7/README.md
-drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-15 06:00:16.813632 efriser-0.1.7/efris/
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      136 2024-04-13 19:20:15.000000 efriser-0.1.7/efris/__init__.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)     6242 2024-04-13 19:26:19.000000 efriser-0.1.7/efris/invoicing.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)    12249 2024-04-13 16:14:23.000000 efriser-0.1.7/efris/output_cleaner.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)        0 2024-04-13 12:16:02.000000 efriser-0.1.7/efris/payload.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)     1354 2024-04-13 12:28:02.000000 efriser-0.1.7/efris/services.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)     6816 2024-04-13 16:01:02.000000 efriser-0.1.7/efris/utils.py
-drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-15 06:00:16.813632 efriser-0.1.7/efriser.egg-info/
--rw-rw-r--   0 douglas   (1000) douglas   (1000)     2357 2024-04-15 06:00:16.000000 efriser-0.1.7/efriser.egg-info/PKG-INFO
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      283 2024-04-15 06:00:16.000000 efriser-0.1.7/efriser.egg-info/SOURCES.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)        1 2024-04-15 06:00:16.000000 efriser-0.1.7/efriser.egg-info/dependency_links.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)       17 2024-04-15 06:00:16.000000 efriser-0.1.7/efriser.egg-info/requires.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)        6 2024-04-15 06:00:16.000000 efriser-0.1.7/efriser.egg-info/top_level.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)       38 2024-04-15 06:00:16.813632 efriser-0.1.7/setup.cfg
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      721 2024-04-15 05:59:58.000000 efriser-0.1.7/setup.py
+drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-16 09:13:40.977408 efriser-0.1.8/
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)    17784 2024-04-16 09:13:40.977408 efriser-0.1.8/PKG-INFO
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)    17298 2024-04-16 09:07:55.000000 efriser-0.1.8/README.md
+drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-16 09:13:40.977408 efriser-0.1.8/efris/
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      113 2024-04-15 11:34:23.000000 efriser-0.1.8/efris/__init__.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)    11840 2024-04-16 08:33:38.000000 efriser-0.1.8/efris/invoicing.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)    12249 2024-04-15 10:01:21.000000 efriser-0.1.8/efris/output_cleaner.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)        0 2024-04-13 12:16:02.000000 efriser-0.1.8/efris/payload.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)     1354 2024-04-13 12:28:02.000000 efriser-0.1.8/efris/services.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      874 2024-04-16 07:59:39.000000 efriser-0.1.8/efris/test_invoicing.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)     7159 2024-04-16 09:09:50.000000 efriser-0.1.8/efris/utils.py
+drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-16 09:13:40.977408 efriser-0.1.8/efriser.egg-info/
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)    17784 2024-04-16 09:13:40.000000 efriser-0.1.8/efriser.egg-info/PKG-INFO
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      307 2024-04-16 09:13:40.000000 efriser-0.1.8/efriser.egg-info/SOURCES.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)        1 2024-04-16 09:13:40.000000 efriser-0.1.8/efriser.egg-info/dependency_links.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)       17 2024-04-16 09:13:40.000000 efriser-0.1.8/efriser.egg-info/requires.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)        6 2024-04-16 09:13:40.000000 efriser-0.1.8/efriser.egg-info/top_level.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)       38 2024-04-16 09:13:40.977408 efriser-0.1.8/setup.cfg
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      721 2024-04-16 09:12:51.000000 efriser-0.1.8/setup.py
```

### Comparing `efriser-0.1.7/efris/output_cleaner.py` & `efriser-0.1.8/efris/output_cleaner.py`

 * *Files identical despite different names*

### Comparing `efriser-0.1.7/efris/services.py` & `efriser-0.1.8/efris/services.py`

 * *Files identical despite different names*

### Comparing `efriser-0.1.7/efris/utils.py` & `efriser-0.1.8/efris/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -290,8 +290,23 @@
     "attachmentList": [{
         "fileName": "",
         "fileType": "",
         "fileContent": ""
     }]
 }
 
+    return data
+
+def product_upload_json():
+    data = {
+        "havePieceUnit": "101",
+        "goodsName": "",
+        "goodsCode": "",
+        "measureUnit": "",
+        "unitPrice": "",
+        "currency": "",
+        "commodityCategoryId": "",
+        "haveExciseTax": "",
+        "description": "",
+        "stockPrewarning": "",
+    }
     return data
```

### Comparing `efriser-0.1.7/setup.py` & `efriser-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='efriser',
-    version='0.1.7',
+    version='0.1.8',
     author='Douglas Ssekuwanda',
     author_email='cytixdoug@gmail.com',
     description='This is a python package to aid in fiscalisation of invoices with the Uganda Revenue Authority (URA) using the EFRIS API.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

