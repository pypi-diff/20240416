# Comparing `tmp/lazy_schema-0.2.1.tar.gz` & `tmp/lazy_schema-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_schema-0.2.1.tar", max compression
+gzip compressed data, was "lazy_schema-0.2.2.tar", max compression
```

## Comparing `lazy_schema-0.2.1.tar` & `lazy_schema-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2948 2024-03-08 00:37:24.160180 lazy_schema-0.2.1/README.md
--rw-r--r--   0        0        0       71 2024-04-16 07:03:59.348863 lazy_schema-0.2.1/lazy_schema/__init__.py
--rw-r--r--   0        0        0     3516 2024-04-16 07:04:07.892748 lazy_schema-0.2.1/lazy_schema/schema.py
--rw-r--r--   0        0        0     1039 2024-04-16 07:00:48.332307 lazy_schema-0.2.1/lazy_schema/schema_pool.py
--rw-r--r--   0        0        0      278 2024-04-16 07:04:19.940591 lazy_schema-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3447 1970-01-01 00:00:00.000000 lazy_schema-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2948 2024-03-08 00:37:24.160180 lazy_schema-0.2.2/README.md
+-rw-r--r--   0        0        0       71 2024-04-16 07:03:59.348863 lazy_schema-0.2.2/lazy_schema/__init__.py
+-rw-r--r--   0        0        0     3680 2024-04-16 07:46:41.196442 lazy_schema-0.2.2/lazy_schema/schema.py
+-rw-r--r--   0        0        0     1037 2024-04-16 07:49:42.224834 lazy_schema-0.2.2/lazy_schema/schema_pool.py
+-rw-r--r--   0        0        0      278 2024-04-16 07:49:51.837296 lazy_schema-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3447 1970-01-01 00:00:00.000000 lazy_schema-0.2.2/PKG-INFO
```

### Comparing `lazy_schema-0.2.1/README.md` & `lazy_schema-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `lazy_schema-0.2.1/lazy_schema/schema.py` & `lazy_schema-0.2.2/lazy_schema/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from typing import Any, NamedTuple
+from typing import Any, NamedTuple, Union
 
 
 class Schema(NamedTuple):
     all_fields: dict
     default_fields: dict
     discrete: bool
     no_default: bool
@@ -56,63 +56,68 @@
             else:
                 raise Exception(f"Key '{key}' does not exist!")
 
         return result
 
     @staticmethod
     def new(
-        *json_paths: str,
+        *args: Union[str, dict],
         __discrete__=False,
         __no_default__=False,
         __no_null__=False,
-        **fields,
+        **kwargs,
     ):
         """
         :__discrete__: When `true`, excludes fields with a `null` default value. Explicitly setting the value to `null` will include it.
 
         :__no_default__: When `true`, default values are excluded.
 
         :__no_null__: When `true`, `null` values will never be included.
         """
         return schema(
-            *json_paths,
+            *args,
             __discrete__=__discrete__,
             __no_default__=__no_default__,
             __no_null__=__no_null__,
-            **fields,
+            **kwargs,
         )
 
 
 def schema(
-    *json_paths: str,
+    *args: Union[str, dict],
     __discrete__=False,
     __no_default__=False,
     __no_null__=False,
-    **fields,
+    **kwargs,
 ):
     """
     :__discrete__: When `true`, excludes fields with a `null` default value. Explicitly setting the value to `null` will include it.
 
     :__no_default__: When `true`, default values are excluded.
 
     :__no_null__: When `true`, `null` values will never be included.
     """
     # Get all fields.
 
     all_fields: dict[str, Any] = {}
 
-    for path in json_paths:
-        with open(path, "r") as f:
-            json_fields = json.loads(f.read())
-
-            for key in json_fields:
-                all_fields[key] = json_fields[key]
+    for arg in args:
+        if isinstance(arg, str):
+            with open(arg, "r") as f:
+                json_fields = json.loads(f.read())
+
+                for key in json_fields:
+                    all_fields[key] = json_fields[key]
+
+        elif isinstance(arg, dict):
+            for key in arg:
+                all_fields[key] = arg[key]
 
-    for key in fields:
-        all_fields[key] = fields[key]
+    for key in kwargs:
+        all_fields[key] = kwargs[key]
 
     # Get default fields.
 
     default_fields: dict[str, Any] = {}
 
     for key in all_fields:
         if key.startswith("__") and key.endswith("__"):
```

### Comparing `lazy_schema-0.2.1/PKG-INFO` & `lazy_schema-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-schema
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: MisterNyan
 Author-email: michael.edmund.wong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

