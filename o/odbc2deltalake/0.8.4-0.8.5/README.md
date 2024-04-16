# Comparing `tmp/odbc2deltalake-0.8.4.tar.gz` & `tmp/odbc2deltalake-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odbc2deltalake-0.8.4.tar", max compression
+gzip compressed data, was "odbc2deltalake-0.8.5.tar", max compression
```

## Comparing `odbc2deltalake-0.8.4.tar` & `odbc2deltalake-0.8.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1081 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/LICENSE
--rw-r--r--   0        0        0     3563 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/README.md
--rw-r--r--   0        0        0      126 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/__init__.py
--rw-r--r--   0        0        0    42950 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/db_to_delta.py
--rw-r--r--   0        0        0     3809 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/delta_logger.py
--rw-r--r--   0        0        0       38 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/destination/__init__.py
--rw-r--r--   0        0        0     2554 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/destination/azure.py
--rw-r--r--   0        0        0     2923 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/destination/azure_utils.py
--rw-r--r--   0        0        0     2541 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/destination/databricks.py
--rw-r--r--   0        0        0     1196 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/destination/destination.py
--rw-r--r--   0        0        0     1592 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/destination/file_system.py
--rw-r--r--   0        0        0     5458 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/metadata.py
--rw-r--r--   0        0        0     1221 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/odbc_utils.py
--rw-r--r--   0        0        0     1851 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/query.py
--rw-r--r--   0        0        0       38 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/reader/__init__.py
--rw-r--r--   0        0        0     7195 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/reader/odbc_reader.py
--rw-r--r--   0        0        0     1961 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/reader/reader.py
--rw-r--r--   0        0        0     4932 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/reader/spark_reader.py
--rw-r--r--   0        0        0     1976 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/sql_glot_utils.py
--rw-r--r--   0        0        0      951 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/sql_schema.py
--rw-r--r--   0        0        0        0 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/write_utils/__init__.py
--rw-r--r--   0        0        0     4757 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/odbc2deltalake/write_utils/restore_pk.py
--rw-r--r--   0        0        0     1373 2024-04-15 09:16:48.391728 odbc2deltalake-0.8.4/pyproject.toml
--rw-r--r--   0        0        0     4497 1970-01-01 00:00:00.000000 odbc2deltalake-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/LICENSE
+-rw-r--r--   0        0        0     3563 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/README.md
+-rw-r--r--   0        0        0      126 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/__init__.py
+-rw-r--r--   0        0        0    42985 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/db_to_delta.py
+-rw-r--r--   0        0        0     3809 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/delta_logger.py
+-rw-r--r--   0        0        0       38 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/destination/__init__.py
+-rw-r--r--   0        0        0     2554 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/destination/azure.py
+-rw-r--r--   0        0        0     2923 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/destination/azure_utils.py
+-rw-r--r--   0        0        0     2541 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/destination/databricks.py
+-rw-r--r--   0        0        0     1196 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/destination/destination.py
+-rw-r--r--   0        0        0     1592 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/destination/file_system.py
+-rw-r--r--   0        0        0     5458 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/metadata.py
+-rw-r--r--   0        0        0     1221 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/odbc_utils.py
+-rw-r--r--   0        0        0     1851 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/query.py
+-rw-r--r--   0        0        0       38 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/reader/__init__.py
+-rw-r--r--   0        0        0     7195 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/reader/odbc_reader.py
+-rw-r--r--   0        0        0     1961 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/reader/reader.py
+-rw-r--r--   0        0        0     4932 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/reader/spark_reader.py
+-rw-r--r--   0        0        0     1976 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/sql_glot_utils.py
+-rw-r--r--   0        0        0      951 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/sql_schema.py
+-rw-r--r--   0        0        0        0 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/write_utils/__init__.py
+-rw-r--r--   0        0        0     6107 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/write_utils/restore_pk.py
+-rw-r--r--   0        0        0     1373 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0     4497 1970-01-01 00:00:00.000000 odbc2deltalake-0.8.5/PKG-INFO
```

### Comparing `odbc2deltalake-0.8.4/LICENSE` & `odbc2deltalake-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.4/README.md` & `odbc2deltalake-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.4/odbc2deltalake/db_to_delta.py` & `odbc2deltalake-0.8.5/odbc2deltalake/db_to_delta.py`

 * *Files 0% similar despite different names*

```diff
@@ -516,26 +516,27 @@
     if last_pk_path and not reader.local_delta_table_exists(
         last_pk_path
     ):  # or do a full load?
         logger.warning(f"{table}: Primary keys missing, try to restore")
         try:
             from .write_utils.restore_pk import restore_last_pk
 
-            restore_sucess = restore_last_pk(
+            restore_success = restore_last_pk(
                 reader,
                 table,
                 destination,
                 delta_col,
                 pk_cols,
                 write_config=write_config,
+                logger=logger,
             )
         except Exception as e:
             logger.warning(f"{table}: Could not restore primary keys: {e}")
-            restore_sucess = False
-        if not restore_sucess:
+            restore_success = False
+        if not restore_success:
             logger.warning(f"{table}: No primary keys found, do a full load")
             do_full_load(
                 logger,
                 reader,
                 table,
                 delta_path=destination / "delta",
                 mode="append",
```

### Comparing `odbc2deltalake-0.8.4/odbc2deltalake/delta_logger.py` & `odbc2deltalake-0.8.5/odbc2deltalake/delta_logger.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.4/odbc2deltalake/destination/azure.py` & `odbc2deltalake-0.8.5/odbc2deltalake/destination/azure.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.4/odbc2deltalake/destination/azure_utils.py` & `odbc2deltalake-0.8.5/odbc2deltalake/destination/azure_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.4/odbc2deltalake/destination/databricks.py` & `odbc2deltalake-0.8.5/odbc2deltalake/destination/databricks.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.4/odbc2deltalake/destination/destination.py` & `odbc2deltalake-0.8.5/odbc2deltalake/destination/destination.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.4/odbc2deltalake/destination/file_system.py` & `odbc2deltalake-0.8.5/odbc2deltalake/destination/file_system.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.4/odbc2deltalake/metadata.py` & `odbc2deltalake-0.8.5/odbc2deltalake/metadata.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.4/odbc2deltalake/odbc_utils.py` & `odbc2deltalake-0.8.5/odbc2deltalake/odbc_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.4/odbc2deltalake/query.py` & `odbc2deltalake-0.8.5/odbc2deltalake/query.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.4/odbc2deltalake/reader/odbc_reader.py` & `odbc2deltalake-0.8.5/odbc2deltalake/reader/odbc_reader.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.4/odbc2deltalake/reader/reader.py` & `odbc2deltalake-0.8.5/odbc2deltalake/reader/reader.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.4/odbc2deltalake/reader/spark_reader.py` & `odbc2deltalake-0.8.5/odbc2deltalake/reader/spark_reader.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.4/odbc2deltalake/sql_glot_utils.py` & `odbc2deltalake-0.8.5/odbc2deltalake/sql_glot_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.4/odbc2deltalake/sql_schema.py` & `odbc2deltalake-0.8.5/odbc2deltalake/sql_schema.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.4/odbc2deltalake/write_utils/restore_pk.py` & `odbc2deltalake-0.8.5/odbc2deltalake/write_utils/restore_pk.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from odbc2deltalake.db_to_delta import (
     IS_DELETED_COL_NAME,
     IS_FULL_LOAD_COL_NAME,
     VALID_FROM_COL_NAME,
     DBDeltaPathConfigs,
     WriteConfig,
 )
+from odbc2deltalake.delta_logger import DeltaLogger
 from odbc2deltalake.destination.destination import Destination
 from odbc2deltalake.metadata import InformationSchemaColInfo
 from odbc2deltalake.reader.reader import DataSourceReader
 import sqlglot.expressions as ex
 import sqlglot as sg
 
 from odbc2deltalake.sql_glot_utils import count_limit_one
@@ -25,14 +26,15 @@
 def restore_last_pk(
     reader: DataSourceReader,
     table: table_name_type,
     destination: Destination,
     delta_col: InformationSchemaColInfo,
     pk_cols: list[InformationSchemaColInfo],
     write_config: WriteConfig,
+    logger: DeltaLogger,
 ):
     delta_path = destination / "delta"
     reader.local_register_update_view(delta_path, _temp_table(table))
 
     sq_valid_from = reader.local_execute_sql_to_py(
         sg.from_(ex.to_identifier(_temp_table(table)))
         .select(ex.func("max", ex.column(VALID_FROM_COL_NAME)).as_(VALID_FROM_COL_NAME))
@@ -41,38 +43,40 @@
     if sq_valid_from is None or len(sq_valid_from) == 0:
         return False
     latest_full_load_date = sq_valid_from[0][VALID_FROM_COL_NAME]
     reader.local_register_view(
         sg.from_(ex.table_(ex.to_identifier(_temp_table(table)), alias="tr"))
         .select(
             *(
-                [ex.column(write_config.get_target_name(c), "tr") for c in pk_cols]
-                + [ex.column(delta_col.column_name, "tr")]
-            )
+                [ex.column(write_config.get_target_name(c)) for c in pk_cols]
+                + [ex.column(delta_col.column_name), ex.column(VALID_FROM_COL_NAME)]
+            ),
+            copy=False
         )
         .where(
             ex.column(IS_FULL_LOAD_COL_NAME).eq(True)
             and ex.column(VALID_FROM_COL_NAME).eq(
                 ex.Subquery(
-                    this=ex.select(ex.func("MAX", ex.column(VALID_FROM_COL_NAME)))
-                    .from_(ex.table_(ex.to_identifier(_temp_table(table)), alias="tr"))
+                    this=ex.select(ex.func("MAX", ex.column(VALID_FROM_COL_NAME, "ts")))
+                    .from_(ex.table_(ex.to_identifier(_temp_table(table)), alias="ts"))
                     .where(ex.column(IS_FULL_LOAD_COL_NAME).eq(True))
                 )
             )
         ),
         "last_full_load",
     )
 
     sq = (
         sg.from_(ex.table_(_temp_table(table), alias="tr"))
         .select(
             *(
                 [ex.column(write_config.get_target_name(c), "tr") for c in pk_cols]
                 + [ex.column(write_config.get_target_name(delta_col), "tr")]
                 + [ex.column(IS_DELETED_COL_NAME, "tr")]
+                + [ex.column(VALID_FROM_COL_NAME, "tr")]
             )
         )
         .where(ex.column(VALID_FROM_COL_NAME) > ex.convert(latest_full_load_date))
     )
     sq = sq.qualify(
         ex.EQ(
             this=ex.Window(
@@ -91,41 +95,71 @@
                 ),
                 over="OVER",
             ),
             expression=ex.convert(1),
         )
     )
     reader.local_register_view(sq, "delta_after_full_load")
-    reader.local_register_view(
-        sq.from_("base")
-        .where(ex.column(IS_DELETED_COL_NAME))
+    last_pk_query = (
+        sg.from_("base")
+        .where(~ex.column(IS_DELETED_COL_NAME))
         .with_(
             "base",
             as_=ex.union(
-                left=sq.from_("delta_after_full_load").select("*"),
-                right=sq.from_(ex.table_("last_full_load", "f")).join(
-                    ex.table_("delta_after_full_load", "d"),
+                left=sg.from_(ex.table_("delta_after_full_load", alias="df")).select(
+                    *(
+                        [
+                            ex.column(write_config.get_target_name(c), "df")
+                            for c in pk_cols
+                        ]
+                        + [
+                            ex.column(write_config.get_target_name(delta_col), "df"),
+                            ex.column(IS_DELETED_COL_NAME, "df"),
+                        ]
+                    )
+                ),
+                right=sg.from_(ex.table_("last_full_load", alias="f"))
+                .select(
+                    *(
+                        [
+                            ex.column(write_config.get_target_name(c), "f")
+                            for c in pk_cols
+                        ]
+                        + [
+                            ex.column(write_config.get_target_name(delta_col), "f"),
+                            ex.convert(False).as_(IS_DELETED_COL_NAME),
+                        ]
+                    )
+                )
+                .join(
+                    ex.table_("delta_after_full_load", alias="d"),
                     join_type="anti",
                     on=ex.and_(
                         *[
                             ex.column(write_config.get_target_name(c), "f").eq(
                                 ex.column(write_config.get_target_name(c), "d")
                             )
                             for c in pk_cols
                         ]
                     ),
                 ),
                 distinct=False,
             ),
         )
-        .select(ex.Star(**{"except": [ex.column(IS_DELETED_COL_NAME)]})),
+        .select(ex.Star(**{"except": [ex.column(IS_DELETED_COL_NAME)]}), append=False)
+    )
+    logger.info(
+        "Restoring last pk version", sql=last_pk_query.sql(reader.query_dialect)
+    )
+    reader.local_register_view(
+        last_pk_query,
         "v_last_pk_version",
     )
     cnt = reader.local_execute_sql_to_py(count_limit_one("v_last_pk_version"))[0]["cnt"]
     if cnt == 0:
         return False
     reader.local_execute_sql_to_delta(
-        sq.from_("v_last_pk_version").select(ex.Star()),
+        sg.from_("v_last_pk_version").select(ex.Star()),
         destination / "delta_load" / DBDeltaPathConfigs.LATEST_PK_VERSION,
         mode="overwrite",
     )
     return True
```

### Comparing `odbc2deltalake-0.8.4/pyproject.toml` & `odbc2deltalake-0.8.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "odbc2deltalake"
-version = "0.8.4"
+version = "0.8.5"
 description = ""
 authors = ["Adrian Ehrsam <adrian.ehrsam@bmsuisse.ch>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = ">=1.10.0"
 pyodbc = { version = "^5.1.0", optional = true }
-deltalake2db = { version = ">=0.2.1", optional = true }
+deltalake2db = { version = ">=0.3.0", optional = true }
 arrow-odbc = { version = "^5.0.0", optional = true }
 deltalake = { version = ">=0.16.1", optional = true }
 duckdb = { version = ">=0.10.1", optional = true }
 azure-identity = { version = "^1.15.0", optional = true }
 adlfs = { version = "^2024.2.0", optional = true }
 sqlglot = "^23.0.5"
```

### Comparing `odbc2deltalake-0.8.4/PKG-INFO` & `odbc2deltalake-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odbc2deltalake
-Version: 0.8.4
+Version: 0.8.5
 Summary: 
 License: MIT
 Author: Adrian Ehrsam
 Author-email: adrian.ehrsam@bmsuisse.ch
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: local
 Provides-Extra: local-azure
 Requires-Dist: adlfs (>=2024.2.0,<2025.0.0) ; extra == "local-azure"
 Requires-Dist: arrow-odbc (>=5.0.0,<6.0.0) ; extra == "local"
 Requires-Dist: azure-identity (>=1.15.0,<2.0.0) ; extra == "local-azure"
 Requires-Dist: deltalake (>=0.16.1) ; extra == "local"
-Requires-Dist: deltalake2db (>=0.2.1) ; extra == "local"
+Requires-Dist: deltalake2db (>=0.3.0) ; extra == "local"
 Requires-Dist: duckdb (>=0.10.1) ; extra == "local"
 Requires-Dist: pydantic (>=1.10.0)
 Requires-Dist: pyodbc (>=5.1.0,<6.0.0) ; extra == "local"
 Requires-Dist: sqlglot (>=23.0.5,<24.0.0)
 Description-Content-Type: text/markdown
 
 # ODBC 2 Deltalake
```

