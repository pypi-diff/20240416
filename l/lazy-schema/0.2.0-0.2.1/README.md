# Comparing `tmp/lazy_schema-0.2.0.tar.gz` & `tmp/lazy_schema-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_schema-0.2.0.tar", max compression
+gzip compressed data, was "lazy_schema-0.2.1.tar", max compression
```

## Comparing `lazy_schema-0.2.0.tar` & `lazy_schema-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2948 2024-03-08 00:37:24.160180 lazy_schema-0.2.0/README.md
--rw-r--r--   0        0        0       63 2024-04-16 06:44:52.004546 lazy_schema-0.2.0/lazy_schema/__init__.py
--rw-r--r--   0        0        0     5288 2024-04-16 06:35:14.612996 lazy_schema-0.2.0/lazy_schema/schema.py
--rw-r--r--   0        0        0     1533 2024-04-16 06:47:03.328296 lazy_schema-0.2.0/lazy_schema/schema_pool.py
--rw-r--r--   0        0        0      278 2024-04-16 06:47:29.175205 lazy_schema-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3447 1970-01-01 00:00:00.000000 lazy_schema-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2948 2024-03-08 00:37:24.160180 lazy_schema-0.2.1/README.md
+-rw-r--r--   0        0        0       71 2024-04-16 07:03:59.348863 lazy_schema-0.2.1/lazy_schema/__init__.py
+-rw-r--r--   0        0        0     3516 2024-04-16 07:04:07.892748 lazy_schema-0.2.1/lazy_schema/schema.py
+-rw-r--r--   0        0        0     1039 2024-04-16 07:00:48.332307 lazy_schema-0.2.1/lazy_schema/schema_pool.py
+-rw-r--r--   0        0        0      278 2024-04-16 07:04:19.940591 lazy_schema-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3447 1970-01-01 00:00:00.000000 lazy_schema-0.2.1/PKG-INFO
```

### Comparing `lazy_schema-0.2.0/README.md` & `lazy_schema-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lazy_schema-0.2.0/lazy_schema/schema.py` & `lazy_schema-0.2.1/lazy_schema/schema.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,9 @@
 import json
-from typing import Any, Dict, NamedTuple
-
-
-SPECIAL_KEYWORDS = {
-    "__discrete__": False,
-    "__no_default__": False,
-    "__no_null__": False,
-}
+from typing import Any, NamedTuple
 
 
 class Schema(NamedTuple):
     all_fields: dict
     default_fields: dict
     discrete: bool
     no_default: bool
@@ -76,60 +69,36 @@
         """
         :__discrete__: When `true`, excludes fields with a `null` default value. Explicitly setting the value to `null` will include it.
 
         :__no_default__: When `true`, default values are excluded.
 
         :__no_null__: When `true`, `null` values will never be included.
         """
-        # Get all fields.
-
-        all_fields: dict[str, Any] = {}
-
-        for path in json_paths:
-            with open(path, "r") as f:
-                json_fields = json.loads(f.read())
-
-                for key in json_fields:
-                    all_fields[key] = json_fields[key]
-
-        for key in fields:
-            all_fields[key] = fields[key]
-
-        # Get default fields.
-
-        default_fields: dict[str, Any] = {}
-
-        for key in all_fields:
-            if key.startswith("__") and key.endswith("__"):
-                continue
-
-            default_fields[key] = all_fields[key]
-
-        # Create generator.
-
-        return Schema(
-            all_fields=all_fields,
-            default_fields=default_fields,
-            discrete=__discrete__,
-            no_default=__no_default__,
-            no_null=__no_null__,
+        return schema(
+            *json_paths,
+            __discrete__=__discrete__,
+            __no_default__=__no_default__,
+            __no_null__=__no_null__,
+            **fields,
         )
 
 
-def schema(*json_paths: str, **fields):
+def schema(
+    *json_paths: str,
+    __discrete__=False,
+    __no_default__=False,
+    __no_null__=False,
+    **fields,
+):
     """
-    __discrete__ = `False`: When `true`,
-    excludes fields with a `null` default value.
-    Explicitly setting the value to `null` will include it.
+    :__discrete__: When `true`, excludes fields with a `null` default value. Explicitly setting the value to `null` will include it.
 
-    __no_default__ = `False`: When `true`,
-    default values are excluded.
+    :__no_default__: When `true`, default values are excluded.
 
-    __no_null__ = `False`: When `true`,
-    `null` values will never be included.
+    :__no_null__: When `true`, `null` values will never be included.
     """
     # Get all fields.
 
     all_fields: dict[str, Any] = {}
 
     for path in json_paths:
         with open(path, "r") as f:
@@ -149,50 +118,14 @@
         if key.startswith("__") and key.endswith("__"):
             continue
 
         default_fields[key] = all_fields[key]
 
     # Create generator.
 
-    def schema(**kwargs) -> Dict[str, Any]:
-        # Get special keywords.
-
-        special_keywords = {}
-
-        for keyword in SPECIAL_KEYWORDS:
-            special_keywords[keyword] = kwargs.get(
-                keyword,
-                all_fields.get(
-                    keyword,
-                    SPECIAL_KEYWORDS[keyword],
-                ),
-            )
-
-        result = {}
-
-        if not special_keywords["__no_default__"]:
-            for key in default_fields:
-                value = default_fields[key]
-
-                if (
-                    special_keywords["__discrete__"] or special_keywords["__no_null__"]
-                ) and value == None:
-                    continue
-
-                if callable(value):
-                    result[key] = value()
-                else:
-                    result[key] = value
-
-        for key in kwargs:
-            if key.startswith("__") and key.endswith("__"):
-                continue
-
-            if key in default_fields:
-                if not special_keywords["__no_null__"] or kwargs[key] != None:
-                    result[key] = kwargs[key]
-            else:
-                raise Exception(f"Key '{key}' does not exist!")
-
-        return result
-
-    return schema
+    return Schema(
+        all_fields=all_fields,
+        default_fields=default_fields,
+        discrete=__discrete__,
+        no_default=__no_default__,
+        no_null=__no_null__,
+    )
```

### Comparing `lazy_schema-0.2.0/PKG-INFO` & `lazy_schema-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-schema
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: MisterNyan
 Author-email: michael.edmund.wong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

