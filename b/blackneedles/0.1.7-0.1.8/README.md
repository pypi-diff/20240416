# Comparing `tmp/blackneedles-0.1.7.tar.gz` & `tmp/blackneedles-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackneedles-0.1.7.tar", max compression
+gzip compressed data, was "blackneedles-0.1.8.tar", max compression
```

## Comparing `blackneedles-0.1.7.tar` & `blackneedles-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1639 2024-04-05 21:51:01.835080 blackneedles-0.1.7/README.md
--rw-r--r--   0        0        0        0 2024-04-05 21:51:01.835080 blackneedles-0.1.7/blackneedles/__init__.py
--rw-r--r--   0        0        0     2601 2024-04-05 21:51:01.835080 blackneedles-0.1.7/blackneedles/__main__.py
--rw-r--r--   0        0        0        0 2024-04-05 21:51:01.835080 blackneedles-0.1.7/blackneedles/commands/__init__.py
--rw-r--r--   0        0        0      964 2024-04-05 21:51:01.835080 blackneedles-0.1.7/blackneedles/commands/compute_pool.py
--rw-r--r--   0        0        0     3472 2024-04-05 21:51:01.835080 blackneedles-0.1.7/blackneedles/commands/service.py
--rw-r--r--   0        0        0     2069 2024-04-05 21:51:01.835080 blackneedles-0.1.7/blackneedles/connection.py
--rw-r--r--   0        0        0     1301 2024-04-05 21:51:01.835080 blackneedles-0.1.7/blackneedles/console.py
--rw-r--r--   0        0        0        0 2024-04-05 21:51:01.835080 blackneedles-0.1.7/blackneedles/models/__init__.py
--rw-r--r--   0        0        0     1233 2024-04-05 21:51:01.835080 blackneedles-0.1.7/blackneedles/models/compute_pool.py
--rw-r--r--   0        0        0     3568 2024-04-05 21:51:01.835080 blackneedles-0.1.7/blackneedles/models/service.py
--rw-r--r--   0        0        0      455 2024-04-05 21:51:01.835080 blackneedles-0.1.7/blackneedles/procedures/grant_permissions.sql
--rw-r--r--   0        0        0     1749 2024-04-05 21:51:01.835080 blackneedles-0.1.7/blackneedles/procedures/monitoring_procedures.sql
--rw-r--r--   0        0        0       47 2024-04-05 21:51:01.835080 blackneedles-0.1.7/blackneedles/procedures/uninstall.sql
--rw-r--r--   0        0        0        0 2024-04-05 21:51:01.835080 blackneedles-0.1.7/blackneedles/utils/__init__.py
--rw-r--r--   0        0        0      730 2024-04-05 21:51:01.835080 blackneedles-0.1.7/blackneedles/utils/logs.py
--rw-r--r--   0        0        0      711 2024-04-05 21:51:02.339083 blackneedles-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 blackneedles-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1639 2024-04-15 21:28:16.970107 blackneedles-0.1.8/README.md
+-rw-r--r--   0        0        0     1383 2024-04-15 21:28:16.970107 blackneedles-0.1.8/blackneedles/__init__.py
+-rw-r--r--   0        0        0     1315 2024-04-15 21:28:16.970107 blackneedles-0.1.8/blackneedles/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-15 21:28:16.970107 blackneedles-0.1.8/blackneedles/commands/__init__.py
+-rw-r--r--   0        0        0      964 2024-04-15 21:28:16.970107 blackneedles-0.1.8/blackneedles/commands/compute_pool.py
+-rw-r--r--   0        0        0     3472 2024-04-15 21:28:16.970107 blackneedles-0.1.8/blackneedles/commands/service.py
+-rw-r--r--   0        0        0     2069 2024-04-15 21:28:16.970107 blackneedles-0.1.8/blackneedles/connection.py
+-rw-r--r--   0        0        0     1301 2024-04-15 21:28:16.970107 blackneedles-0.1.8/blackneedles/console.py
+-rw-r--r--   0        0        0        0 2024-04-15 21:28:16.970107 blackneedles-0.1.8/blackneedles/models/__init__.py
+-rw-r--r--   0        0        0     1233 2024-04-15 21:28:16.970107 blackneedles-0.1.8/blackneedles/models/compute_pool.py
+-rw-r--r--   0        0        0     3568 2024-04-15 21:28:16.970107 blackneedles-0.1.8/blackneedles/models/service.py
+-rw-r--r--   0        0        0      455 2024-04-15 21:28:16.970107 blackneedles-0.1.8/blackneedles/procedures/grant_permissions.sql
+-rw-r--r--   0        0        0     1749 2024-04-15 21:28:16.970107 blackneedles-0.1.8/blackneedles/procedures/monitoring_procedures.sql
+-rw-r--r--   0        0        0       47 2024-04-15 21:28:16.970107 blackneedles-0.1.8/blackneedles/procedures/uninstall.sql
+-rw-r--r--   0        0        0        0 2024-04-15 21:28:16.970107 blackneedles-0.1.8/blackneedles/utils/__init__.py
+-rw-r--r--   0        0        0      730 2024-04-15 21:28:16.970107 blackneedles-0.1.8/blackneedles/utils/logs.py
+-rw-r--r--   0        0        0      711 2024-04-15 21:28:17.470108 blackneedles-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 blackneedles-0.1.8/PKG-INFO
```

### Comparing `blackneedles-0.1.7/README.md` & `blackneedles-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.7/blackneedles/commands/compute_pool.py` & `blackneedles-0.1.8/blackneedles/commands/compute_pool.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.7/blackneedles/commands/service.py` & `blackneedles-0.1.8/blackneedles/commands/service.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.7/blackneedles/connection.py` & `blackneedles-0.1.8/blackneedles/connection.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.7/blackneedles/console.py` & `blackneedles-0.1.8/blackneedles/console.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.7/blackneedles/models/compute_pool.py` & `blackneedles-0.1.8/blackneedles/models/compute_pool.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.7/blackneedles/models/service.py` & `blackneedles-0.1.8/blackneedles/models/service.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.7/blackneedles/procedures/monitoring_procedures.sql` & `blackneedles-0.1.8/blackneedles/procedures/monitoring_procedures.sql`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.7/blackneedles/utils/logs.py` & `blackneedles-0.1.8/blackneedles/utils/logs.py`

 * *Files identical despite different names*

### Comparing `blackneedles-0.1.7/pyproject.toml` & `blackneedles-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blackneedles"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["Thiago F Pappacena <pappacena@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 # Note: snowflake-snowpark-python requires <3.12. Fix this once they support 3.12
 python = "^3.8,<3.12"
```

### Comparing `blackneedles-0.1.7/PKG-INFO` & `blackneedles-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackneedles
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: Thiago F Pappacena
 Author-email: pappacena@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

