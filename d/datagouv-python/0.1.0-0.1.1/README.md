# Comparing `tmp/datagouv_python-0.1.0.tar.gz` & `tmp/datagouv_python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagouv_python-0.1.0.tar", max compression
+gzip compressed data, was "datagouv_python-0.1.1.tar", max compression
```

## Comparing `datagouv_python-0.1.0.tar` & `datagouv_python-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2024-04-13 15:20:42.145253 datagouv_python-0.1.0/LICENSE
--rw-r--r--   0        0        0     1937 2024-04-15 18:41:15.142307 datagouv_python-0.1.0/README.md
--rw-r--r--   0        0        0      283 2024-04-15 06:43:06.307169 datagouv_python-0.1.0/datagouv/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 06:37:03.712875 datagouv_python-0.1.0/datagouv/api_client/__init__.py
--rw-r--r--   0        0        0     1202 2024-04-14 15:16:06.984989 datagouv_python-0.1.0/datagouv/api_client/_data_requestor.py
--rw-r--r--   0        0        0      350 2024-04-15 06:37:24.354131 datagouv_python-0.1.0/datagouv/api_client/_datagouv_client.py
--rw-r--r--   0        0        0     1456 2024-04-15 18:25:21.049046 datagouv_python-0.1.0/datagouv/api_client/_datasets_service.py
--rw-r--r--   0        0        0        0 2024-04-15 06:20:34.551164 datagouv_python-0.1.0/datagouv/downloader/__init__.py
--rw-r--r--   0        0        0      912 2024-04-15 18:45:33.019203 datagouv_python-0.1.0/datagouv/downloader/_resources_downloader.py
--rw-r--r--   0        0        0      767 2024-04-15 07:00:51.087557 datagouv_python-0.1.0/datagouv/downloader/_utils.py
--rw-r--r--   0        0        0      131 2024-04-14 15:05:59.938086 datagouv_python-0.1.0/datagouv/main.py
--rw-r--r--   0        0        0      467 2024-04-15 19:03:59.678846 datagouv_python-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 datagouv_python-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-13 15:20:42.145253 datagouv_python-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2112 2024-04-15 19:11:59.179304 datagouv_python-0.1.1/README.md
+-rw-r--r--   0        0        0      283 2024-04-15 06:43:06.307169 datagouv_python-0.1.1/datagouv/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 06:37:03.712875 datagouv_python-0.1.1/datagouv/api_client/__init__.py
+-rw-r--r--   0        0        0     1373 2024-04-15 19:12:30.887035 datagouv_python-0.1.1/datagouv/api_client/_data_requestor.py
+-rw-r--r--   0        0        0      350 2024-04-15 06:37:24.354131 datagouv_python-0.1.1/datagouv/api_client/_datagouv_client.py
+-rw-r--r--   0        0        0     1607 2024-04-15 19:08:41.405368 datagouv_python-0.1.1/datagouv/api_client/_datasets_service.py
+-rw-r--r--   0        0        0        0 2024-04-15 06:20:34.551164 datagouv_python-0.1.1/datagouv/downloader/__init__.py
+-rw-r--r--   0        0        0      912 2024-04-15 18:45:33.019203 datagouv_python-0.1.1/datagouv/downloader/_resources_downloader.py
+-rw-r--r--   0        0        0      767 2024-04-15 07:00:51.087557 datagouv_python-0.1.1/datagouv/downloader/_utils.py
+-rw-r--r--   0        0        0      131 2024-04-14 15:05:59.938086 datagouv_python-0.1.1/datagouv/main.py
+-rw-r--r--   0        0        0      467 2024-04-15 19:14:44.735850 datagouv_python-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2832 1970-01-01 00:00:00.000000 datagouv_python-0.1.1/PKG-INFO
```

### Comparing `datagouv_python-0.1.0/LICENSE` & `datagouv_python-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datagouv_python-0.1.0/README.md` & `datagouv_python-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -49,14 +49,28 @@
 ```
 poetry run start
 poetry run black datagouv/
 poetry run flake8
 ```
 
 ## Build
+
+### Process
+
+```bash
+poetry version [patch, minor, major]
+poetry install
+poetry build
+# Update CHANGELOG
+git commit -m "vX.X.X"
+git tag vX.X.X
+poetry deploy
+```
+
+### Details
 ```
 poetry version
 poetry version -s
 
 poetry version [patch, minor, major]
 ```
```

### Comparing `datagouv_python-0.1.0/datagouv/api_client/_data_requestor.py` & `datagouv_python-0.1.1/datagouv/api_client/_data_requestor.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,7 +40,13 @@
 
         response = requests.put(absolute_url, json=json, headers=self.headers)
 
         if response.status_code == 200:
             return response.json()
         else:
             return response
+
+    def delete(self, url):
+        absolute_url = f"{self.base_url}{url}"
+        response = requests.delete(absolute_url, headers=self.headers)
+
+        return response
```

### Comparing `datagouv_python-0.1.0/datagouv/api_client/_datasets_service.py` & `datagouv_python-0.1.1/datagouv/api_client/_datasets_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,40 +2,41 @@
 
 
 class DatasetsService(object):
     def __init__(self, options):
         self.options = options
         self.requestor = DataRequestor(self.options)
 
-    def search(self, query, options):
+    def search(self, query):
         url = f"/datasets?q={query}"
-
         return self.requestor.get(url)
 
     def get(self, dataset_id):
         url = f"/datasets/{dataset_id}"
-
         return self.requestor.get(url)
 
     def post_resource_file(self, dataset_id, filename):
         url = f"/datasets/{dataset_id}/upload"
-
         return self.requestor.post_file(url, filename)
 
     def put_resource_file(self, dataset_id, filename, resource_id):
         url = f"/datasets/{dataset_id}/resources/{resource_id}/upload"
-
         return self.requestor.post_file(url, filename)
 
     def put_resource(self, dataset_id, resource):
         resource_id = resource.get("id")
         url = f"/datasets/{dataset_id}/resources/{resource_id}"
 
         return self.requestor.put(url, resource)
 
+    def delete_resource(self, dataset_id, resource_id):
+        url = f"/datasets/{dataset_id}/resources/{resource_id}"
+
+        return self.requestor.delete(url)
+
     """
         only in api v2
         def get_resources(self, dataset_id, options={}):
         page = options.get('page', None)
         page_size = options.get('page_size', None)
 
         url = f"/datasets/{dataset_id}/resources?"#page={page}&page_size={page_size}"
```

### Comparing `datagouv_python-0.1.0/datagouv/downloader/_resources_downloader.py` & `datagouv_python-0.1.1/datagouv/downloader/_resources_downloader.py`

 * *Files identical despite different names*

### Comparing `datagouv_python-0.1.0/datagouv/downloader/_utils.py` & `datagouv_python-0.1.1/datagouv/downloader/_utils.py`

 * *Files identical despite different names*

### Comparing `datagouv_python-0.1.0/PKG-INFO` & `datagouv_python-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagouv-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: GPL-3.0-or-later
 Author: Maxime Pawlak
 Author-email: maxime.pawlak@amatek.fr
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -69,14 +69,28 @@
 ```
 poetry run start
 poetry run black datagouv/
 poetry run flake8
 ```
 
 ## Build
+
+### Process
+
+```bash
+poetry version [patch, minor, major]
+poetry install
+poetry build
+# Update CHANGELOG
+git commit -m "vX.X.X"
+git tag vX.X.X
+poetry deploy
+```
+
+### Details
 ```
 poetry version
 poetry version -s
 
 poetry version [patch, minor, major]
 ```
```

