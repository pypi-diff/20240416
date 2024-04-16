# Comparing `tmp/motion_lake_client-0.0.8.tar.gz` & `tmp/motion_lake_client-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_lake_client-0.0.8.tar", last modified: Mon Apr 15 16:17:23 2024, max compression
+gzip compressed data, was "motion_lake_client-0.0.9.tar", last modified: Mon Apr 15 16:20:07 2024, max compression
```

## Comparing `motion_lake_client-0.0.8.tar` & `motion_lake_client-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-15 16:17:23.315645 motion_lake_client-0.0.8/
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      516 2024-04-05 16:21:57.000000 motion_lake_client-0.0.8/LICENSE
--rw-r--r--   0 gaspard   (1000) gaspard   (1000)     5774 2024-04-15 16:17:23.315645 motion_lake_client-0.0.8/PKG-INFO
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)     4591 2024-04-15 15:35:18.000000 motion_lake_client-0.0.8/README.md
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      744 2024-04-15 16:17:16.000000 motion_lake_client-0.0.8/pyproject.toml
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       38 2024-04-15 16:17:23.315645 motion_lake_client-0.0.8/setup.cfg
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       37 2024-04-05 16:27:42.000000 motion_lake_client-0.0.8/setup.py
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-15 16:17:23.315645 motion_lake_client-0.0.8/src/
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-15 16:17:23.315645 motion_lake_client-0.0.8/src/motion_lake_client/
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       22 2024-04-05 16:23:48.000000 motion_lake_client-0.0.8/src/motion_lake_client/__init__.py
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)    11808 2024-04-15 16:17:16.000000 motion_lake_client-0.0.8/src/motion_lake_client/client.py
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-15 16:17:23.315645 motion_lake_client-0.0.8/src/motion_lake_client.egg-info/
--rw-r--r--   0 gaspard   (1000) gaspard   (1000)     5774 2024-04-15 16:17:23.000000 motion_lake_client-0.0.8/src/motion_lake_client.egg-info/PKG-INFO
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      338 2024-04-15 16:17:23.000000 motion_lake_client-0.0.8/src/motion_lake_client.egg-info/SOURCES.txt
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        1 2024-04-15 16:17:23.000000 motion_lake_client-0.0.8/src/motion_lake_client.egg-info/dependency_links.txt
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        9 2024-04-15 16:17:23.000000 motion_lake_client-0.0.8/src/motion_lake_client.egg-info/requires.txt
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       19 2024-04-15 16:17:23.000000 motion_lake_client-0.0.8/src/motion_lake_client.egg-info/top_level.txt
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-15 16:20:07.014439 motion_lake_client-0.0.9/
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      516 2024-04-05 16:21:57.000000 motion_lake_client-0.0.9/LICENSE
+-rw-r--r--   0 gaspard   (1000) gaspard   (1000)     5774 2024-04-15 16:20:07.014439 motion_lake_client-0.0.9/PKG-INFO
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)     4591 2024-04-15 15:35:18.000000 motion_lake_client-0.0.9/README.md
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      744 2024-04-15 16:20:04.000000 motion_lake_client-0.0.9/pyproject.toml
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       38 2024-04-15 16:20:07.014439 motion_lake_client-0.0.9/setup.cfg
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       37 2024-04-05 16:27:42.000000 motion_lake_client-0.0.9/setup.py
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-15 16:20:07.014439 motion_lake_client-0.0.9/src/
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-15 16:20:07.014439 motion_lake_client-0.0.9/src/motion_lake_client/
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       22 2024-04-05 16:23:48.000000 motion_lake_client-0.0.9/src/motion_lake_client/__init__.py
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)    12136 2024-04-15 16:20:04.000000 motion_lake_client-0.0.9/src/motion_lake_client/client.py
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-15 16:20:07.014439 motion_lake_client-0.0.9/src/motion_lake_client.egg-info/
+-rw-r--r--   0 gaspard   (1000) gaspard   (1000)     5774 2024-04-15 16:20:07.000000 motion_lake_client-0.0.9/src/motion_lake_client.egg-info/PKG-INFO
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      338 2024-04-15 16:20:07.000000 motion_lake_client-0.0.9/src/motion_lake_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        1 2024-04-15 16:20:07.000000 motion_lake_client-0.0.9/src/motion_lake_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        9 2024-04-15 16:20:07.000000 motion_lake_client-0.0.9/src/motion_lake_client.egg-info/requires.txt
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       19 2024-04-15 16:20:07.000000 motion_lake_client-0.0.9/src/motion_lake_client.egg-info/top_level.txt
```

### Comparing `motion_lake_client-0.0.8/LICENSE` & `motion_lake_client-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `motion_lake_client-0.0.8/PKG-INFO` & `motion_lake_client-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-lake-client
-Version: 0.0.8
+Version: 0.0.9
 Summary: Motion Lake Client, a client for the Motion Lake API (a Mobility Data Lake)
 Author-email: Gaspard Merten <gaspard.mp.work@gmail.com>
 License: All Rights Reserved
         
         Copyright (c) 2024 Gaspard Merten
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
```

### Comparing `motion_lake_client-0.0.8/README.md` & `motion_lake_client-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `motion_lake_client-0.0.8/pyproject.toml` & `motion_lake_client-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "motion-lake-client"
-version = "0.0.8"
+version = "0.0.9"
 description = "Motion Lake Client, a client for the Motion Lake API (a Mobility Data Lake)"
 readme = "README.md"
 authors = [{ name = "Gaspard Merten", email = "gaspard.mp.work@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: Other/Proprietary License",
     "Programming Language :: Python",
```

### Comparing `motion_lake_client-0.0.8/src/motion_lake_client/client.py` & `motion_lake_client-0.0.9/src/motion_lake_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -287,67 +287,70 @@
         self,
         collection_name: str,
         min_datetime: datetime,
         max_datetime: datetime,
         ascending: bool,
         limit: int = None,
         offset: int = 0,
+        skip_data: bool = False,
     ) -> dict:
         min_datetime = min_datetime or MIN_DATE
         max_datetime = max_datetime or MAX_DATE
 
         return self.inner_client.query(
             collection_name,
             int(min_datetime.timestamp()),
             int(max_datetime.timestamp()),
             ascending,
             limit,
             offset,
+            skip_data,
         )
 
-    def get_last_items(self, collection_name: str, limit: int) -> List[Item]:
-        response = self.query(collection_name, MIN_DATE, datetime.now(), False, limit)
+    def get_last_items(self, collection_name: str, limit: int, skip_data: bool = False) -> List[Item]:
+        response = self.query(collection_name, MIN_DATE, datetime.now(), False, limit, 0, skip_data)
         return self._parse_results(response["results"])
 
-    def get_last_item(self, collection_name: str) -> Item:
-        results = self.get_last_items(collection_name, 1)
+    def get_last_item(self, collection_name: str, skip_data: bool = False) -> Item:
+        results = self.get_last_items(collection_name, 1, skip_data)
         return (results or [None])[0]
 
-    def get_first_items(self, collection_name: str, limit: int) -> List[Item]:
-        response = self.query(collection_name, MIN_DATE, datetime.now(), True, limit)
+    def get_first_items(self, collection_name: str, limit: int, skip_data: bool = False) -> List[Item]:
+        response = self.query(collection_name, MIN_DATE, datetime.now(), True, limit, 0, skip_data)
         return self._parse_results(response["results"])
 
-    def get_first_item(self, collection_name: str) -> Item:
-        items = self.get_first_items(collection_name, 1)
+    def get_first_item(self, collection_name: str, skip_data: bool = False) -> Item:
+        items = self.get_first_items(collection_name, 1, skip_data)
 
         return (items or [None])[0]
 
     def get_items_between(
         self,
         collection_name: str,
         min_datetime: datetime,
         max_datetime: datetime,
         ascending: bool = True,
         limit: int = None,
         offset: int = None,
+        skip_data: bool = False,
     ) -> List[Item]:
         response = self.query(
-            collection_name, min_datetime, max_datetime, ascending, limit, offset
+            collection_name, min_datetime, max_datetime, ascending, limit, offset, skip_data
         )
         return self._parse_results(response["results"])
 
     def get_items_before(
-        self, collection_name: str, date: datetime, limit: int
+        self, collection_name: str, date: datetime, limit: int, skip_data: bool = False
     ) -> List[Item]:
-        return self.get_items_between(collection_name, MIN_DATE, date, False, limit)
+        return self.get_items_between(collection_name, MIN_DATE, date, False, limit, 0, skip_data)
 
     def get_items_after(
-        self, collection_name: str, timestamp: datetime, limit: int
+        self, collection_name: str, timestamp: datetime, limit: int, skip_data: bool = False
     ) -> List[Item]:
-        return self.get_items_between(collection_name, timestamp, MAX_DATE, True, limit)
+        return self.get_items_between(collection_name, timestamp, MAX_DATE, True, limit, 0, skip_data)
 
     def get_collections(self) -> List[Collection]:
         return self.inner_client.get_collections()
 
     def advanced_query(
         self,
         collection_name: str,
```

### Comparing `motion_lake_client-0.0.8/src/motion_lake_client.egg-info/PKG-INFO` & `motion_lake_client-0.0.9/src/motion_lake_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-lake-client
-Version: 0.0.8
+Version: 0.0.9
 Summary: Motion Lake Client, a client for the Motion Lake API (a Mobility Data Lake)
 Author-email: Gaspard Merten <gaspard.mp.work@gmail.com>
 License: All Rights Reserved
         
         Copyright (c) 2024 Gaspard Merten
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
```

