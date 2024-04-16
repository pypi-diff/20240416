# Comparing `tmp/simplepgsql-0.1.6.tar.gz` & `tmp/simplepgsql-0.1.7.tar.gz`

## Comparing `simplepgsql-0.1.6.tar` & `simplepgsql-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 simplepgsql-0.1.6/CHANGELOG.md
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 simplepgsql-0.1.6/requirements.txt
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 simplepgsql-0.1.6/run.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 simplepgsql-0.1.6/setup.cfg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simplepgsql-0.1.6/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simplepgsql-0.1.6/simplepgsql/README.md
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 simplepgsql-0.1.6/simplepgsql/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 simplepgsql-0.1.6/simplepgsql/src/__init__.py
--rw-r--r--   0        0        0    16068 2020-02-02 00:00:00.000000 simplepgsql-0.1.6/simplepgsql/src/simplepgsql.py
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 simplepgsql-0.1.6/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 simplepgsql-0.1.6/LICENSE
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 simplepgsql-0.1.6/README.md
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 simplepgsql-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    42748 2020-02-02 00:00:00.000000 simplepgsql-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/CHANGELOG.md
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/requirements.txt
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/run.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/setup.cfg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/simplepgsql/README.md
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/simplepgsql/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/simplepgsql/src/__init__.py
+-rw-r--r--   0        0        0    16154 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/simplepgsql/src/depr_simplepgsql.py
+-rw-r--r--   0        0        0    16275 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/simplepgsql/src/simplepgsql.py
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/README.md
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    42748 2020-02-02 00:00:00.000000 simplepgsql-0.1.7/PKG-INFO
```

### Comparing `simplepgsql-0.1.6/CHANGELOG.md` & `simplepgsql-0.1.7/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 ## [Unreleased]
 
+## [0.1.7] - 2024-04-16
+
+### Added
+1. It automatically creates and destroys the cursor. No need to use `with` to enter.
+
+### Removed/Deprecated
+1. DBConnect Class. It will still exist but new features will not be supported for backwards compatibility of versions. It is replaced by `SimplePgSQL` class. 
+
 ## [0.1.6] - 2024-03-04
 
 ### Bugfix
 1. fixed Breaking of IN/NOT IN usage. 
 
 ## [0.1.5] - 2024-02-28
```

### Comparing `simplepgsql-0.1.6/run.py` & `simplepgsql-0.1.7/run.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import pandas as pd
 from simplepgsql import DBConnect
+from simplepgsql import SimplePgSQL
 import configparser
 
 if __name__ == "__main__":
     # read data from config file
     config = configparser.ConfigParser()
     config.read("config.ini")
     conn_params = {
@@ -12,24 +13,34 @@
         "database": config['DB']['DB_NAME'],
         "user": config['DB']['DB_USER'].strip(),
         "password": config['DB']['DB_PASSWORD'].strip(),
         "port": config['DB']['DB_PORT'],
     }
     
   
-    # _query_params = {
-    #     "schema": "public",
-    #     "table_name": "film_list",
-    #     "columns": ["category", "price"],
-    #     "aggregate": {
-    #         "price": "SUM"
-    #     },
-    #     "conditions": {
-    #         "length": (60, ">")
-    #     },
-    #     "order_by": ("price", "DESC"),
-    #     "group_by": ["category", "price"],
-    #     "limit": 10,
-    # }
+    _query_params = {
+        "schema": "public",
+        "table_name": "film_list",
+        "columns": ["category", "price"],
+        "aggregate": {
+            "price": "SUM"
+        },
+        "conditions": {
+            "length": (60, ">")
+        },
+        "order_by": ("price", "DESC"),
+        "group_by": ["category", "price"],
+        "limit": 10,
+    }
+
+    # Using SimplePgSQL class
+    pgsql = SimplePgSQL(conn_params, return_type=pd.DataFrame)
+
+    q_results = pgsql.execute("SELECT category, price FROM film_list LIMIT 10;", columns=["category", "price"])
+    r_results = pgsql.read(**_query_params)
+    print(q_results)
+    print(r_results)
+    
+    # Deprecated method to query data DO NOT USE. For backward compatibility only
     with DBConnect(conn_params, return_type=pd.DataFrame) as cursor:
-        results = cursor.query("SELECT category, price FROM film_list LIMIT 10;", columns=["category", "price"])
-        print(results)
+        q_results = cursor.query("SELECT category, price FROM film_list LIMIT 10;", columns=["category", "price"])
+        r_results = cursor.read(**_query_params)
```

### Comparing `simplepgsql-0.1.6/simplepgsql/src/simplepgsql.py` & `simplepgsql-0.1.7/simplepgsql/src/depr_simplepgsql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from typing_extensions import deprecated
 import psycopg2
 import pandas as pd
 from psycopg2 import sql
 
-
+@deprecated("Use SimplePgSQL class instead")
 class DBConnect:
     def __init__(self, conn_params: dict, return_type: type = dict) -> None:
         """
         Initializes a DBConnect object.
 
         Parameters
         ----------
```

### Comparing `simplepgsql-0.1.6/.gitignore` & `simplepgsql-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `simplepgsql-0.1.6/LICENSE` & `simplepgsql-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `simplepgsql-0.1.6/README.md` & `simplepgsql-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `simplepgsql-0.1.6/pyproject.toml` & `simplepgsql-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 7369 6d70 6c65 7067 7371 6c22 0d0a   "simplepgsql"..
-00000070: 7665 7273 696f 6e20 3d20 2230 2e31 2e36  version = "0.1.6
+00000070: 7665 7273 696f 6e20 3d20 2230 2e31 2e37  version = "0.1.7
 00000080: 220d 0a64 6573 6372 6970 7469 6f6e 203d  "..description =
 00000090: 2022 5772 6170 7065 7220 6172 6f75 6e64   "Wrapper around
 000000a0: 2070 7379 636f 7067 3220 746f 2073 696d   psycopg2 to sim
 000000b0: 706c 6966 7920 7468 6520 7072 6f63 6573  plify the proces
 000000c0: 7320 6f66 2063 6f6e 6e65 6374 696e 6720  s of connecting 
 000000d0: 746f 2061 2050 6f73 7467 7265 5351 4c20  to a PostgreSQL 
 000000e0: 6461 7461 6261 7365 2061 6e64 2065 7865  database and exe
```

### Comparing `simplepgsql-0.1.6/PKG-INFO` & `simplepgsql-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: simplepgsql
-Version: 0.1.6
+Version: 0.1.7
 Summary: Wrapper around psycopg2 to simplify the process of connecting to a PostgreSQL database and executing queries.
 Project-URL: Repository, https://github.com/iamlrk/simple-pgsql
 Author-email: iamlrk <lepakshiramkiran@hotmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

