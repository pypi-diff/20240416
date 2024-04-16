# Comparing `tmp/lazy_schema-0.2.2.tar.gz` & `tmp/lazy_schema-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_schema-0.2.2.tar", max compression
+gzip compressed data, was "lazy_schema-0.2.3.tar", max compression
```

## Comparing `lazy_schema-0.2.2.tar` & `lazy_schema-0.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2948 2024-03-08 00:37:24.160180 lazy_schema-0.2.2/README.md
--rw-r--r--   0        0        0       71 2024-04-16 07:03:59.348863 lazy_schema-0.2.2/lazy_schema/__init__.py
--rw-r--r--   0        0        0     3680 2024-04-16 07:46:41.196442 lazy_schema-0.2.2/lazy_schema/schema.py
--rw-r--r--   0        0        0     1037 2024-04-16 07:49:42.224834 lazy_schema-0.2.2/lazy_schema/schema_pool.py
--rw-r--r--   0        0        0      278 2024-04-16 07:49:51.837296 lazy_schema-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3447 1970-01-01 00:00:00.000000 lazy_schema-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2948 2024-03-08 00:37:24.160180 lazy_schema-0.2.3/README.md
+-rw-r--r--   0        0        0       71 2024-04-16 07:03:59.348863 lazy_schema-0.2.3/lazy_schema/__init__.py
+-rw-r--r--   0        0        0     3680 2024-04-16 08:18:08.325296 lazy_schema-0.2.3/lazy_schema/schema.py
+-rw-r--r--   0        0        0     2467 2024-04-16 08:17:10.844434 lazy_schema-0.2.3/lazy_schema/schema_pool.py
+-rw-r--r--   0        0        0      278 2024-04-16 08:18:13.845378 lazy_schema-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3447 1970-01-01 00:00:00.000000 lazy_schema-0.2.3/PKG-INFO
```

### Comparing `lazy_schema-0.2.2/README.md` & `lazy_schema-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `lazy_schema-0.2.2/lazy_schema/schema.py` & `lazy_schema-0.2.3/lazy_schema/schema.py`

 * *Files identical despite different names*

### Comparing `lazy_schema-0.2.2/PKG-INFO` & `lazy_schema-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-schema
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

