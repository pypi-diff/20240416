# Comparing `tmp/lazy_schema-0.2.3.tar.gz` & `tmp/lazy_schema-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_schema-0.2.3.tar", max compression
+gzip compressed data, was "lazy_schema-0.2.4.tar", max compression
```

## Comparing `lazy_schema-0.2.3.tar` & `lazy_schema-0.2.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2948 2024-03-08 00:37:24.160180 lazy_schema-0.2.3/README.md
--rw-r--r--   0        0        0       71 2024-04-16 07:03:59.348863 lazy_schema-0.2.3/lazy_schema/__init__.py
--rw-r--r--   0        0        0     3680 2024-04-16 08:18:08.325296 lazy_schema-0.2.3/lazy_schema/schema.py
--rw-r--r--   0        0        0     2467 2024-04-16 08:17:10.844434 lazy_schema-0.2.3/lazy_schema/schema_pool.py
--rw-r--r--   0        0        0      278 2024-04-16 08:18:13.845378 lazy_schema-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3447 1970-01-01 00:00:00.000000 lazy_schema-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     2948 2024-03-08 00:37:24.160180 lazy_schema-0.2.4/README.md
+-rw-r--r--   0        0        0       71 2024-04-16 07:03:59.348863 lazy_schema-0.2.4/lazy_schema/__init__.py
+-rw-r--r--   0        0        0     3680 2024-04-16 08:18:08.325296 lazy_schema-0.2.4/lazy_schema/schema.py
+-rw-r--r--   0        0        0     2511 2024-04-16 08:21:31.384284 lazy_schema-0.2.4/lazy_schema/schema_pool.py
+-rw-r--r--   0        0        0      278 2024-04-16 08:21:38.836392 lazy_schema-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3447 1970-01-01 00:00:00.000000 lazy_schema-0.2.4/PKG-INFO
```

### Comparing `lazy_schema-0.2.3/README.md` & `lazy_schema-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `lazy_schema-0.2.3/lazy_schema/schema.py` & `lazy_schema-0.2.4/lazy_schema/schema.py`

 * *Files identical despite different names*

### Comparing `lazy_schema-0.2.3/lazy_schema/schema_pool.py` & `lazy_schema-0.2.4/lazy_schema/schema_pool.py`

 * *Files 22% similar despite different names*

```diff
@@ -33,22 +33,20 @@
         field_name="__name__",
         *args: Union[str, dict],
         __discrete__=False,
         __no_default__=False,
         __no_null__=False,
         **kwargs,
     ):
-        self.set(
+        return self.pymongo_query(
+            mongo_collection,
             name,
-            __load_document(
-                mongo_collection,
-                {
-                    field_name: name,
-                },
-            ),
+            {
+                field_name: name,
+            },
             *args,
             __discrete__=__discrete__,
             __no_default__=__no_default__,
             __no_null__=__no_null__,
             **kwargs,
         )
 
@@ -59,20 +57,22 @@
         query,
         *args: Union[str, dict],
         __discrete__=False,
         __no_default__=False,
         __no_null__=False,
         **kwargs,
     ):
-        self.set(
+        document = __load_document(mongo_collection, query)
+
+        if document == None:
+            raise Exception(f"Failed to retrieve schema '{name}'!")
+
+        return self.set(
             name,
-            __load_document(
-                mongo_collection,
-                query,
-            ),
+            document,
             *args,
             __discrete__=__discrete__,
             __no_default__=__no_default__,
             __no_null__=__no_null__,
             **kwargs,
         )
```

### Comparing `lazy_schema-0.2.3/PKG-INFO` & `lazy_schema-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-schema
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Author: MisterNyan
 Author-email: michael.edmund.wong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

