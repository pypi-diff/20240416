# Comparing `tmp/lazy_mongo-0.2.2.tar.gz` & `tmp/lazy_mongo-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_mongo-0.2.2.tar", max compression
+gzip compressed data, was "lazy_mongo-0.2.3.tar", max compression
```

## Comparing `lazy_mongo-0.2.2.tar` & `lazy_mongo-0.2.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       40 2024-03-08 03:29:01.600206 lazy_mongo-0.2.2/README.md
--rw-r--r--   0        0        0      207 2024-03-22 03:18:21.246648 lazy_mongo-0.2.2/lazy_mongo/__init__.py
--rw-r--r--   0        0        0      234 2024-03-22 03:13:35.641590 lazy_mongo-0.2.2/lazy_mongo/insert_response.py
--rw-r--r--   0        0        0     1784 2024-03-27 05:12:25.619739 lazy_mongo-0.2.2/lazy_mongo/lazy_collection.py
--rw-r--r--   0        0        0     1818 2024-03-27 05:13:57.761621 lazy_mongo-0.2.2/lazy_mongo/lazy_database.py
--rw-r--r--   0        0        0     2406 2024-03-27 05:14:35.152714 lazy_mongo-0.2.2/lazy_mongo/lazy_mongo.py
--rw-r--r--   0        0        0      180 2024-03-22 03:13:43.334160 lazy_mongo-0.2.2/lazy_mongo/update_response.py
--rw-r--r--   0        0        0      296 2024-03-27 05:14:56.520186 lazy_mongo-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 lazy_mongo-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       40 2024-03-08 03:29:01.600206 lazy_mongo-0.2.3/README.md
+-rw-r--r--   0        0        0      207 2024-03-22 03:18:21.246648 lazy_mongo-0.2.3/lazy_mongo/__init__.py
+-rw-r--r--   0        0        0      265 2024-04-16 01:49:02.827730 lazy_mongo-0.2.3/lazy_mongo/insert_response.py
+-rw-r--r--   0        0        0     2180 2024-04-16 01:50:16.611945 lazy_mongo-0.2.3/lazy_mongo/lazy_collection.py
+-rw-r--r--   0        0        0     1818 2024-03-27 05:13:57.761621 lazy_mongo-0.2.3/lazy_mongo/lazy_database.py
+-rw-r--r--   0        0        0     2406 2024-03-27 05:14:35.152714 lazy_mongo-0.2.3/lazy_mongo/lazy_mongo.py
+-rw-r--r--   0        0        0      211 2024-04-16 01:49:06.275740 lazy_mongo-0.2.3/lazy_mongo/update_response.py
+-rw-r--r--   0        0        0      296 2024-04-16 01:52:03.912265 lazy_mongo-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 lazy_mongo-0.2.3/PKG-INFO
```

### Comparing `lazy_mongo-0.2.2/lazy_mongo/lazy_collection.py` & `lazy_mongo-0.2.3/lazy_mongo/lazy_collection.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Dict, NamedTuple
 from pymongo.collection import Collection
+from pymongo.errors import DuplicateKeyError
 from .update_response import UpdateResponse
 from .insert_response import InsertResponse
 
 
 class LazyCollection(NamedTuple):
     collection: Collection
 
@@ -29,14 +30,21 @@
             result = self.collection.insert_one(document)
 
             return InsertResponse(
                 ok=True,
                 result=result,
             )
 
+        except DuplicateKeyError as e:
+            return InsertResponse(
+                ok=False,
+                is_duplicate=True,
+                error=e,
+            )
+
         except Exception as e:
             return InsertResponse(
                 ok=False,
                 error=e,
             )
 
     def update_set_one(
@@ -53,14 +61,22 @@
                 upsert=False,
             )
 
             return UpdateResponse(
                 ok=True,
                 result=result,
             )
+
+        except DuplicateKeyError as e:
+            return UpdateResponse(
+                ok=False,
+                is_duplicate=True,
+                error=e,
+            )
+
         except Exception as e:
             return UpdateResponse(
                 ok=False,
                 error=e,
             )
 
     def count(
```

### Comparing `lazy_mongo-0.2.2/lazy_mongo/lazy_database.py` & `lazy_mongo-0.2.3/lazy_mongo/lazy_database.py`

 * *Files identical despite different names*

### Comparing `lazy_mongo-0.2.2/lazy_mongo/lazy_mongo.py` & `lazy_mongo-0.2.3/lazy_mongo/lazy_mongo.py`

 * *Files identical despite different names*

### Comparing `lazy_mongo-0.2.2/PKG-INFO` & `lazy_mongo-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-mongo
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: MisterNyan
 Author-email: michael.edmund.wong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

