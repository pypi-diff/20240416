# Comparing `tmp/deltalake2db-0.2.3.tar.gz` & `tmp/deltalake2db-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltalake2db-0.2.3.tar", max compression
+gzip compressed data, was "deltalake2db-0.3.0.tar", max compression
```

## Comparing `deltalake2db-0.2.3.tar` & `deltalake2db-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     2066 2024-03-26 10:51:45.010670 deltalake2db-0.2.3/README.md
--rw-r--r--   0        0        0      343 2024-03-26 10:51:45.010670 deltalake2db-0.2.3/deltalake2db/__init__.py
--rw-r--r--   0        0        0    14184 2024-03-26 10:51:45.010670 deltalake2db-0.2.3/deltalake2db/duckdb.py
--rw-r--r--   0        0        0     5466 2024-03-26 10:51:45.010670 deltalake2db-0.2.3/deltalake2db/polars.py
--rw-r--r--   0        0        0      963 2024-03-26 10:51:45.010670 deltalake2db-0.2.3/deltalake2db/protocol_check.py
--rw-r--r--   0        0        0     2661 2024-03-26 10:51:45.010670 deltalake2db-0.2.3/deltalake2db/sql_utils.py
--rw-r--r--   0        0        0      697 2024-03-26 10:51:45.010670 deltalake2db-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2539 1970-01-01 00:00:00.000000 deltalake2db-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     2066 2024-04-16 08:56:26.257312 deltalake2db-0.3.0/README.md
+-rw-r--r--   0        0        0      343 2024-04-16 08:56:26.257312 deltalake2db-0.3.0/deltalake2db/__init__.py
+-rw-r--r--   0        0        0    14504 2024-04-16 08:56:26.257312 deltalake2db-0.3.0/deltalake2db/duckdb.py
+-rw-r--r--   0        0        0      891 2024-04-16 08:56:26.257312 deltalake2db-0.3.0/deltalake2db/filter_by_meta.py
+-rw-r--r--   0        0        0     5989 2024-04-16 08:56:26.257312 deltalake2db-0.3.0/deltalake2db/polars.py
+-rw-r--r--   0        0        0      963 2024-04-16 08:56:26.257312 deltalake2db-0.3.0/deltalake2db/protocol_check.py
+-rw-r--r--   0        0        0     2608 2024-04-16 08:56:26.257312 deltalake2db-0.3.0/deltalake2db/sql_utils.py
+-rw-r--r--   0        0        0      697 2024-04-16 08:56:26.257312 deltalake2db-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2539 1970-01-01 00:00:00.000000 deltalake2db-0.3.0/PKG-INFO
```

### Comparing `deltalake2db-0.2.3/README.md` & `deltalake2db-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `deltalake2db-0.2.3/deltalake2db/duckdb.py` & `deltalake2db-0.3.0/deltalake2db/duckdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from collections.abc import Sequence
 import os
 from pathlib import Path
 from typing import TYPE_CHECKING, Callable
 from deltalake import DataType, Field
 from deltalake.schema import StructType, ArrayType, PrimitiveType, MapType
 import sqlglot.expressions as ex
+from deltalake2db.filter_by_meta import _can_filter
 import deltalake2db.sql_utils as squ
 
 if TYPE_CHECKING:
     from deltalake import DeltaTable
     import duckdb
 
 
@@ -231,16 +232,18 @@
 
 
 def create_view_for_delta(
     con: "duckdb.DuckDBPyConnection",
     delta_table: "DeltaTable | Path",
     view_name: str,
     overwrite=True,
+    *,
+    conditions: dict | None = None,
 ):
-    sql = get_sql_for_delta(delta_table, duck_con=con)
+    sql = get_sql_for_delta(delta_table, duck_con=con, conditions=conditions)
     assert '"' not in view_name
     if overwrite:
         con.execute(f'create or replace view "{view_name}" as {sql}')
     else:
         con.execute(f'create view "{view_name}" as {sql}')
 
 
@@ -279,14 +282,20 @@
         owns_con = True
     if dt.table_uri.startswith("az://") or dt.table_uri.startswith("abfss://"):
         apply_storage_options(duck_con, dt._storage_options, type="azure")  # type: ignore
 
     try:
 
         for ac in dt.get_add_actions(flatten=True).to_pylist():
+            if (
+                conditions is not None
+                and isinstance(conditions, dict)
+                and _can_filter(ac, conditions)
+            ):
+                continue
             if action_filter and not action_filter(ac):
                 continue
             fullpath = dt.table_uri.removesuffix("/") + "/" + ac["path"]
             with duck_con.cursor() as cur:
                 cur.execute(f"select name from parquet_schema('{fullpath}')")
                 cols: list[str] = [c[0] for c in cur.fetchall()]
             cols_sql: list[ex.Expression] = []
```

### Comparing `deltalake2db-0.2.3/deltalake2db/polars.py` & `deltalake2db-0.3.0/deltalake2db/polars.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from pathlib import Path
 from typing import TYPE_CHECKING
 
+from deltalake2db.filter_by_meta import _can_filter
+
 if TYPE_CHECKING:
     import polars as pl
 from deltalake import DeltaTable, Field, DataType
 from deltalake.exceptions import DeltaProtocolError
 from deltalake.schema import StructType, ArrayType, PrimitiveType, MapType
 import os
 
@@ -97,24 +99,32 @@
     elif dtype_str == "null":
         return pl.Null
     elif dtype_str == "timestampNtz":
         return pl.Datetime
     raise NotImplementedError(f"{dtype_str} not supported in polars currently")
 
 
-def scan_delta_union(delta_table: DeltaTable | Path) -> "pl.LazyFrame":
+def _filter_cond(f: "pl.LazyFrame", conditions: dict) -> "pl.LazyFrame":
+    return f.filter(**conditions)
+
+
+def scan_delta_union(
+    delta_table: DeltaTable | Path, conditions: dict | None = None
+) -> "pl.LazyFrame":
     import polars as pl
     from .protocol_check import check_is_supported
 
     if isinstance(delta_table, Path):
         delta_table = DeltaTable(delta_table)
     check_is_supported(delta_table)
     all_ds = []
     all_fields = delta_table.schema().fields
     for ac in delta_table.get_add_actions(flatten=True).to_pylist():
+        if conditions is not None and _can_filter(ac, conditions):
+            continue
         fullpath = os.path.join(delta_table.table_uri, ac["path"])
         base_ds = pl.scan_parquet(
             fullpath, storage_options=delta_table._storage_options
         )
         parquet_schema = base_ds.limit(0).schema
         selects = []
         for field in all_fields:
@@ -135,15 +145,20 @@
                 part_vl = ac["partition." + field.name]
                 selects.append(pl.lit(part_vl, pl_dtype).alias(field.name))
             elif (
                 field.metadata.get("delta.columnMapping.physicalName", field.name)
                 in parquet_schema
             ):
                 selects.append(_get_expr(None, field.type, field))
-
-        ds = base_ds.select(*selects)
+            else:
+                selects.append(pl.lit(None, pl_dtype).alias(field.name))
+        ds = (
+            _filter_cond(base_ds.select(*selects), conditions)
+            if conditions is not None
+            else base_ds.select(*selects)
+        )
         all_ds.append(ds)
     if len(all_ds) == 0:
         return pl.DataFrame(
             data=[], schema={f.name: _get_type(f.type) for f in all_fields}
         ).lazy()
     return pl.concat(all_ds, how="diagonal_relaxed")
```

### Comparing `deltalake2db-0.2.3/deltalake2db/protocol_check.py` & `deltalake2db-0.3.0/deltalake2db/protocol_check.py`

 * *Files identical despite different names*

### Comparing `deltalake2db-0.2.3/deltalake2db/sql_utils.py` & `deltalake2db-0.3.0/deltalake2db/sql_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 from typing import Sequence, Any, TypeVar
 import sqlglot.expressions as ex
 
 
 def read_parquet(
-    path: str | Path | list[Path]| list[str] | ex.Expression | list[ex.Expression],
+    path: str | Path | list[Path] | list[str] | ex.Expression | list[ex.Expression],
 ) -> ex.Expression:
     if isinstance(path, list):
         return ex.func(
             "read_parquet",
             ex.array(
                 *[
                     ex.Literal.string(str(p)) if isinstance(p, (str, Path)) else p
@@ -38,24 +38,22 @@
             selects[0], union(selects[1:], distinct=distinct), distinct=distinct
         )
 
 
 def filter_via_dict(conditions: dict[str, Any] | None):
     if not conditions or len(conditions) == 0:
         return None
-    return ex.and_(
-        *[
-            (
-                ex.EQ(this=ex.column(k, quoted=True), expression=ex.convert(v))
-                if v is not None
-                else ex.Is(this=ex.column(k, quoted=True), expression=ex.Null())
-            )
-            for k, v in conditions.items()
-        ]
-    )
+    return [
+        (
+            ex.EQ(this=ex.column(k, quoted=True), expression=ex.convert(v))
+            if v is not None
+            else ex.Is(this=ex.column(k, quoted=True), expression=ex.Null())
+        )
+        for k, v in conditions.items()
+    ]
 
 
 T = TypeVar("T", bound=ex.Query)
 
 
 def merge_ctes(select: T, other_select: ex.Select) -> T:
     new_select = select.copy()
```

### Comparing `deltalake2db-0.2.3/pyproject.toml` & `deltalake2db-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deltalake2db"
-version = "0.2.3"
+version = "0.3.0"
 description = ""
 authors = ["Adrian Ehrsam <adrian.ehrsam@bmsuisse.ch>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `deltalake2db-0.2.3/PKG-INFO` & `deltalake2db-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltalake2db
-Version: 0.2.3
+Version: 0.3.0
 Summary: 
 License: MIT
 Author: Adrian Ehrsam
 Author-email: adrian.ehrsam@bmsuisse.ch
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

