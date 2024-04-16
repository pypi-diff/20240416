# Comparing `tmp/dataflows_ckan-0.3.8.tar.gz` & `tmp/dataflows_ckan-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataflows_ckan-0.3.8.tar", max compression
+gzip compressed data, was "dataflows_ckan-0.3.9.tar", max compression
```

## Comparing `dataflows_ckan-0.3.8.tar` & `dataflows_ckan-0.3.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1114 2024-03-21 18:29:34.401196 dataflows_ckan-0.3.8/LICENSE.md
--rw-r--r--   0        0        0     1603 2024-03-21 18:29:34.401196 dataflows_ckan-0.3.8/README.md
--rw-r--r--   0        0        0       64 2024-03-21 18:29:34.401196 dataflows_ckan-0.3.8/dataflows_ckan/__init__.py
--rw-r--r--   0        0        0     1009 2024-03-21 18:29:34.401196 dataflows_ckan-0.3.8/dataflows_ckan/helpers.py
--rw-r--r--   0        0        0        0 2024-03-21 18:29:34.401196 dataflows_ckan-0.3.8/dataflows_ckan/processors/__init__.py
--rw-r--r--   0        0        0     7314 2024-03-21 18:29:34.401196 dataflows_ckan-0.3.8/dataflows_ckan/processors/dump_to_ckan.py
--rw-r--r--   0        0        0      868 2024-03-21 18:29:34.401196 dataflows_ckan-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     2388 1970-01-01 00:00:00.000000 dataflows_ckan-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1114 2024-04-16 13:28:36.354516 dataflows_ckan-0.3.9/LICENSE.md
+-rw-r--r--   0        0        0     1603 2024-04-16 13:28:36.354516 dataflows_ckan-0.3.9/README.md
+-rw-r--r--   0        0        0       64 2024-04-16 13:28:36.354516 dataflows_ckan-0.3.9/dataflows_ckan/__init__.py
+-rw-r--r--   0        0        0     1065 2024-04-16 13:28:36.354516 dataflows_ckan-0.3.9/dataflows_ckan/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-16 13:28:36.354516 dataflows_ckan-0.3.9/dataflows_ckan/processors/__init__.py
+-rw-r--r--   0        0        0     7314 2024-04-16 13:28:36.354516 dataflows_ckan-0.3.9/dataflows_ckan/processors/dump_to_ckan.py
+-rw-r--r--   0        0        0      868 2024-04-16 13:28:36.358517 dataflows_ckan-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     2388 1970-01-01 00:00:00.000000 dataflows_ckan-0.3.9/PKG-INFO
```

### Comparing `dataflows_ckan-0.3.8/LICENSE.md` & `dataflows_ckan-0.3.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dataflows_ckan-0.3.8/README.md` & `dataflows_ckan-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `dataflows_ckan-0.3.8/dataflows_ckan/helpers.py` & `dataflows_ckan-0.3.9/dataflows_ckan/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     response = requests.request(
         method=method, url=url, headers=headers, allow_redirects=True, **kwargs
     )
 
     try:
         return response.json()
     except json.decoder.JSONDecodeError:
-        log.error('Expected JSON in response from: {}'.format(url))
+        log.error('Expected JSON in response from: {}\nGot {}:\n{}'.format(url, response.status_code, response.text[:400]))
         raise
 
 
 def get_ckan_error(response):
     '''Return the error from a ckan json response, or None.'''
     ckan_error = None
     if not response['success'] and response['error']:
```

### Comparing `dataflows_ckan-0.3.8/dataflows_ckan/processors/dump_to_ckan.py` & `dataflows_ckan-0.3.9/dataflows_ckan/processors/dump_to_ckan.py`

 * *Files identical despite different names*

### Comparing `dataflows_ckan-0.3.8/pyproject.toml` & `dataflows_ckan-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataflows-ckan"
-version = "0.3.8"
+version = "0.3.9"
 description = "CKAN integration for Dataflows."
 authors = ["Paul Walsh <paul@walsh.co.il>", "Adam Kariv <adam.kariv@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `dataflows_ckan-0.3.8/PKG-INFO` & `dataflows_ckan-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataflows-ckan
-Version: 0.3.8
+Version: 0.3.9
 Summary: CKAN integration for Dataflows.
 License: MIT
 Author: Paul Walsh
 Author-email: paul@walsh.co.il
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

