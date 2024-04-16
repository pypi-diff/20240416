# Comparing `tmp/lazy_schema-0.1.0.tar.gz` & `tmp/lazy_schema-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_schema-0.1.0.tar", max compression
+gzip compressed data, was "lazy_schema-0.2.0.tar", max compression
```

## Comparing `lazy_schema-0.1.0.tar` & `lazy_schema-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     2948 2024-03-08 00:37:24.160180 lazy_schema-0.1.0/README.md
--rw-r--r--   0        0        0       27 2024-03-08 00:15:46.703621 lazy_schema-0.1.0/lazy_schema/__init__.py
--rw-r--r--   0        0        0     2323 2024-03-08 00:38:11.683373 lazy_schema-0.1.0/lazy_schema/schema.py
--rw-r--r--   0        0        0      278 2024-03-08 00:12:47.761701 lazy_schema-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3447 1970-01-01 00:00:00.000000 lazy_schema-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2948 2024-03-08 00:37:24.160180 lazy_schema-0.2.0/README.md
+-rw-r--r--   0        0        0       63 2024-04-16 06:44:52.004546 lazy_schema-0.2.0/lazy_schema/__init__.py
+-rw-r--r--   0        0        0     5288 2024-04-16 06:35:14.612996 lazy_schema-0.2.0/lazy_schema/schema.py
+-rw-r--r--   0        0        0     1533 2024-04-16 06:47:03.328296 lazy_schema-0.2.0/lazy_schema/schema_pool.py
+-rw-r--r--   0        0        0      278 2024-04-16 06:47:29.175205 lazy_schema-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3447 1970-01-01 00:00:00.000000 lazy_schema-0.2.0/PKG-INFO
```

### Comparing `lazy_schema-0.1.0/README.md` & `lazy_schema-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lazy_schema-0.1.0/PKG-INFO` & `lazy_schema-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-schema
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: MisterNyan
 Author-email: michael.edmund.wong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

