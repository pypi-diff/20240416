# Comparing `tmp/duckdb_engine-0.9.4.tar.gz` & `tmp/duckdb_engine-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckdb_engine-0.9.4.tar", max compression
+gzip compressed data, was "duckdb_engine-0.9.5.tar", max compression
```

## Comparing `duckdb_engine-0.9.4.tar` & `duckdb_engine-0.9.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1076 2023-12-09 04:05:38.115170 duckdb_engine-0.9.4/LICENSE.txt
--rw-r--r--   0        0        0     7002 2023-12-09 04:05:38.115170 duckdb_engine-0.9.4/README.md
--rw-r--r--   0        0        0        4 2023-12-09 04:05:38.115170 duckdb_engine-0.9.4/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/7210af19145ec2a8
--rw-r--r--   0        0        0        1 2023-12-09 04:05:38.115170 duckdb_engine-0.9.4/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/bec021b4f368e306
--rw-r--r--   0        0        0    20688 2023-12-09 04:05:38.115170 duckdb_engine-0.9.4/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz
--rw-r--r--   0        0        0    15500 2023-12-09 04:05:38.115170 duckdb_engine-0.9.4/duckdb_engine/__init__.py
--rw-r--r--   0        0        0     1096 2023-12-09 04:05:38.115170 duckdb_engine-0.9.4/duckdb_engine/config.py
--rw-r--r--   0        0        0        0 2023-12-09 04:05:38.115170 duckdb_engine-0.9.4/duckdb_engine/conftest.py
--rw-r--r--   0        0        0     5734 2023-12-09 04:05:38.119170 duckdb_engine-0.9.4/duckdb_engine/datatypes.py
--rw-r--r--   0        0        0        0 2023-12-09 04:05:38.119170 duckdb_engine-0.9.4/duckdb_engine/py.typed
--rw-r--r--   0        0        0        0 2023-12-09 04:05:38.119170 duckdb_engine-0.9.4/duckdb_engine/tests/__init__.py
--rw-r--r--   0        0        0     1401 2023-12-09 04:05:38.119170 duckdb_engine-0.9.4/duckdb_engine/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-12-09 04:05:38.119170 duckdb_engine-0.9.4/duckdb_engine/tests/snapshots/__init__.py
--rw-r--r--   0        0        0      338 2023-12-09 04:05:38.119170 duckdb_engine-0.9.4/duckdb_engine/tests/snapshots/snap_test_basic.py
--rw-r--r--   0        0        0    14043 2023-12-09 04:05:38.119170 duckdb_engine-0.9.4/duckdb_engine/tests/test_basic.py
--rw-r--r--   0        0        0     4035 2023-12-09 04:05:38.119170 duckdb_engine-0.9.4/duckdb_engine/tests/test_datatypes.py
--rw-r--r--   0        0        0      982 2023-12-09 04:05:38.119170 duckdb_engine-0.9.4/duckdb_engine/tests/test_ibis.py
--rw-r--r--   0        0        0     1407 2023-12-09 04:05:38.119170 duckdb_engine-0.9.4/duckdb_engine/tests/test_integration.py
--rw-r--r--   0        0        0     3946 2023-12-09 04:05:38.119170 duckdb_engine-0.9.4/duckdb_engine/tests/test_pandas.py
--rw-r--r--   0        0        0      257 2023-12-09 04:05:38.119170 duckdb_engine-0.9.4/duckdb_engine/tests/util.py
--rw-r--r--   0        0        0     1427 2023-12-09 04:05:38.119170 duckdb_engine-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     7946 1970-01-01 00:00:00.000000 duckdb_engine-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-12-21 03:37:31.032719 duckdb_engine-0.9.5/LICENSE.txt
+-rw-r--r--   0        0        0     7002 2023-12-21 03:37:31.032719 duckdb_engine-0.9.5/README.md
+-rw-r--r--   0        0        0        4 2023-12-21 03:37:31.032719 duckdb_engine-0.9.5/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/7210af19145ec2a8
+-rw-r--r--   0        0        0        1 2023-12-21 03:37:31.032719 duckdb_engine-0.9.5/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/bec021b4f368e306
+-rw-r--r--   0        0        0    20688 2023-12-21 03:37:31.032719 duckdb_engine-0.9.5/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz
+-rw-r--r--   0        0        0    19592 2023-12-21 03:37:31.036718 duckdb_engine-0.9.5/duckdb_engine/__init__.py
+-rw-r--r--   0        0        0     1096 2023-12-21 03:37:31.036718 duckdb_engine-0.9.5/duckdb_engine/config.py
+-rw-r--r--   0        0        0        0 2023-12-21 03:37:31.036718 duckdb_engine-0.9.5/duckdb_engine/conftest.py
+-rw-r--r--   0        0        0     5734 2023-12-21 03:37:31.036718 duckdb_engine-0.9.5/duckdb_engine/datatypes.py
+-rw-r--r--   0        0        0        0 2023-12-21 03:37:31.036718 duckdb_engine-0.9.5/duckdb_engine/py.typed
+-rw-r--r--   0        0        0        0 2023-12-21 03:37:31.036718 duckdb_engine-0.9.5/duckdb_engine/tests/__init__.py
+-rw-r--r--   0        0        0     1401 2023-12-21 03:37:31.036718 duckdb_engine-0.9.5/duckdb_engine/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-12-21 03:37:31.036718 duckdb_engine-0.9.5/duckdb_engine/tests/snapshots/__init__.py
+-rw-r--r--   0        0        0      338 2023-12-21 03:37:31.036718 duckdb_engine-0.9.5/duckdb_engine/tests/snapshots/snap_test_basic.py
+-rw-r--r--   0        0        0    15838 2023-12-21 03:37:31.036718 duckdb_engine-0.9.5/duckdb_engine/tests/test_basic.py
+-rw-r--r--   0        0        0     4035 2023-12-21 03:37:31.036718 duckdb_engine-0.9.5/duckdb_engine/tests/test_datatypes.py
+-rw-r--r--   0        0        0      982 2023-12-21 03:37:31.036718 duckdb_engine-0.9.5/duckdb_engine/tests/test_ibis.py
+-rw-r--r--   0        0        0     1407 2023-12-21 03:37:31.036718 duckdb_engine-0.9.5/duckdb_engine/tests/test_integration.py
+-rw-r--r--   0        0        0     3946 2023-12-21 03:37:31.036718 duckdb_engine-0.9.5/duckdb_engine/tests/test_pandas.py
+-rw-r--r--   0        0        0      257 2023-12-21 03:37:31.036718 duckdb_engine-0.9.5/duckdb_engine/tests/util.py
+-rw-r--r--   0        0        0     1427 2023-12-21 03:37:31.036718 duckdb_engine-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     7946 1970-01-01 00:00:00.000000 duckdb_engine-0.9.5/PKG-INFO
```

### Comparing `duckdb_engine-0.9.4/LICENSE.txt` & `duckdb_engine-0.9.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.9.4/README.md` & `duckdb_engine-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.9.4/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz` & `duckdb_engine-0.9.5/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.9.4/duckdb_engine/__init__.py` & `duckdb_engine-0.9.5/duckdb_engine/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,25 +17,32 @@
 import duckdb
 import sqlalchemy
 from packaging.version import Version
 from sqlalchemy import pool, text
 from sqlalchemy import types as sqltypes
 from sqlalchemy import util
 from sqlalchemy.dialects.postgresql import UUID
-from sqlalchemy.dialects.postgresql.base import PGDialect, PGInspector, PGTypeCompiler
+from sqlalchemy.dialects.postgresql.base import (
+    PGDialect,
+    PGIdentifierPreparer,
+    PGInspector,
+    PGTypeCompiler,
+)
 from sqlalchemy.dialects.postgresql.psycopg2 import PGDialect_psycopg2
 from sqlalchemy.engine.default import DefaultDialect
 from sqlalchemy.engine.reflection import cache
 from sqlalchemy.engine.url import URL
+from sqlalchemy.exc import NoSuchTableError
 from sqlalchemy.ext.compiler import compiles
+from sqlalchemy.sql.selectable import Select
 
 from .config import apply_config, get_core_config
 from .datatypes import ISCHEMA_NAMES, register_extension_types
 
-__version__ = "0.9.4"
+__version__ = "0.9.5"
 sqlalchemy_version = Version(sqlalchemy.__version__)
 duckdb_version: str = duckdb.__version__  # type: ignore[attr-defined]
 supports_attach: bool = Version(duckdb_version) >= Version("0.7.0")
 
 if TYPE_CHECKING:
     from sqlalchemy.base import Connection
     from sqlalchemy.engine.interfaces import _IndexDict
@@ -171,14 +178,46 @@
 def index_warning() -> None:
     warnings.warn(
         "duckdb-engine doesn't yet support reflection on indices",
         DuckDBEngineWarning,
     )
 
 
+class DuckDBIdentifierPreparer(PGIdentifierPreparer):
+    def _separate(self, name: Optional[str]) -> Tuple[Optional[Any], Optional[str]]:
+        """
+        Get database name and schema name from schema if it contains a database name
+            Format:
+              <db_name>.<schema_name>
+              db_name and schema_name are double quoted if contains spaces or double quotes
+        """
+        database_name, schema_name = None, name
+        if name is not None and "." in name:
+            database_name, schema_name = (
+                max(s) for s in re.findall(r'"([^.]+)"|([^.]+)', name)
+            )
+        return database_name, schema_name
+
+    def format_schema(self, name: str) -> str:
+        """Prepare a quoted schema name."""
+        database_name, schema_name = self._separate(name)
+        if database_name is None:
+            return self.quote(name)
+        return ".".join(self.quote(_n) for _n in [database_name, schema_name])
+
+    def quote_schema(self, schema: str, force: Any = None) -> str:
+        """
+        Conditionally quote a schema name.
+
+        :param schema: string schema name
+        :param force: unused
+        """
+        return self.format_schema(schema)
+
+
 class Dialect(PGDialect_psycopg2):
     name = "duckdb"
     driver = "duckdb_engine"
     _has_events = False
     supports_statement_cache = False
     supports_comments = False
     supports_sane_rowcount = False
@@ -196,14 +235,16 @@
             UUID: UUID,
         },
     )
     ischema_names = util.update_copy(
         PGDialect.ischema_names,
         ISCHEMA_NAMES,
     )
+    preparer = DuckDBIdentifierPreparer
+    identifier_preparer: DuckDBIdentifierPreparer
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         kwargs["use_native_hstore"] = False
         super().__init__(*args, **kwargs)
 
     def connect(self, *cargs: Any, **cparams: Any) -> "Connection":
         core_keys = get_core_config()
@@ -278,23 +319,52 @@
         (see https://docs.sqlalchemy.org/en/20/dialects/mssql.html#multipart-schema-names)
         """
 
         if not supports_attach:
             return super().get_schema_names(connection, **kw)
 
         s = """
-            SELECT database_name, schema_name AS npspname
+            SELECT database_name, schema_name AS nspname
             FROM duckdb_schemas()
             WHERE schema_name NOT LIKE 'pg\\_%' ESCAPE '\\'
-            ORDER BY database_name, npspname
+            ORDER BY database_name, nspname
             """
         rs = connection.execute(text(s))
 
         qs = self.identifier_preparer.quote_schema
-        return [f"{qs(db)}.{qs(schema)}" for (db, schema) in rs]
+        return [qs(".".join(nspname)) for nspname in rs]
+
+    def _build_query_where(
+        self,
+        table_name: Optional[str] = None,
+        schema_name: Optional[str] = None,
+        database_name: Optional[str] = None,
+    ) -> Tuple[str, Dict[str, str]]:
+        sql = ""
+        params = {}
+
+        # If no database name is provided, try to get it from the schema name
+        # specified as "<db name>.<schema name>"
+        # If only a schema name is found, database_name will return None
+        if database_name is None and schema_name is not None:
+            database_name, schema_name = self.identifier_preparer._separate(schema_name)
+
+        if table_name is not None:
+            sql += "AND table_name = :table_name\n"
+            params.update({"table_name": table_name})
+
+        if schema_name is not None:
+            sql += "AND schema_name = :schema_name\n"
+            params.update({"schema_name": schema_name})
+
+        if database_name is not None:
+            sql += "AND database_name = :database_name\n"
+            params.update({"database_name": database_name})
+
+        return sql, params
 
     @cache  # type: ignore[call-arg]
     def get_table_names(self, connection: "Connection", schema=None, **kw: "Any"):  # type: ignore[no-untyped-def]
         """
         Return unquoted database_name.schema_name unless either contains spaces or double quotes.
         In that case, escape double quotes and then wrap in double quotes.
         SQLAlchemy definition of a schema includes database name for databases like SQL Server (Ex: databasename.dbo)
@@ -305,40 +375,66 @@
             return super().get_table_names(connection, schema, **kw)
 
         s = """
             SELECT database_name, schema_name, table_name
             FROM duckdb_tables()
             WHERE schema_name NOT LIKE 'pg\\_%' ESCAPE '\\'
             """
-        params = {}
-        if schema is not None:
-            params = {"schema_name": schema}
-            if "." in schema:
-                # Get database name and schema name from schema if it contains a database name
-                # Format:
-                #   <db_name>.<schema_name>
-                #   db_name and schema_name are double quoted if contains spaces or double quotes
-                database_name, schema_name = (
-                    max(s) for s in re.findall(r'"([^.]+)"|([^.]+)', schema)
-                )
-                params = {"database_name": database_name, "schema_name": schema_name}
-                s += "AND database_name = :database_name\n"
-            s += "AND schema_name = :schema_name"
-
+        sql, params = self._build_query_where(schema_name=schema)
+        s += sql
         rs = connection.execute(text(s), params)
 
         return [
             table
             for (
                 db,
                 sc,
                 table,
             ) in rs
         ]
 
+    @cache  # type: ignore[call-arg]
+    def get_table_oid(  # type: ignore[no-untyped-def]
+        self,
+        connection: "Connection",
+        table_name: str,
+        schema: "Optional[str]" = None,
+        **kw: "Any",
+    ):
+        """Fetch the oid for (database.)schema.table_name.
+        The schema name can be formatted either as database.schema or just the schema name.
+        In the latter scenario the schema associated with the default database is used.
+        """
+        s = """
+            SELECT table_oid
+            FROM duckdb_tables()
+            WHERE schema_name NOT LIKE 'pg\\_%' ESCAPE '\\'
+            AND table_name = :table_name
+            """
+        sql, params = self._build_query_where(table_name=table_name, schema_name=schema)
+        s += sql
+
+        rs = connection.execute(text(s), params)
+        table_oid = rs.scalar()
+        if table_oid is None:
+            raise NoSuchTableError(table_name)
+        return table_oid
+
+    def has_table(
+        self,
+        connection: "Connection",
+        table_name: str,
+        schema: Optional[str] = None,
+        **kw: Any,
+    ) -> bool:
+        try:
+            return self.get_table_oid(connection, table_name, schema) is not None
+        except NoSuchTableError:
+            return False
+
     def get_indexes(
         self,
         connection: "Connection",
         table_name: str,
         schema: Optional[str] = None,
         **kw: Any,
     ) -> List["_IndexDict"]:
@@ -371,14 +467,37 @@
     def do_executemany(
         self, cursor: Any, statement: Any, parameters: Any, context: Optional[Any] = ...
     ) -> None:
         return DefaultDialect.do_executemany(
             self, cursor, statement, parameters, context
         )
 
+    def _pg_class_filter_scope_schema(
+        self,
+        query: Select,
+        schema: str,
+        scope: Any,
+        pg_class_table: Any = None,
+    ) -> Any:
+        # Don't scope by schema for now
+        if hasattr(super(), "_pg_class_filter_scope_schema"):
+            query = getattr(super(), "_pg_class_filter_scope_schema")(
+                query, schema=None, scope=scope, pg_class_table=pg_class_table
+            )
+            if schema is not None:
+                # Now let's scope by schema, but make sure we're not adding in the database name prefix
+                # This will not work if a schema or table name is not unique!
+                _, schema_name = self.identifier_preparer._separate(schema)
+                query = query.where(
+                    text("pg_namespace.nspname = :schema_name").bindparams(
+                        schema_name=schema_name
+                    )
+                )
+            return query
+
     # FIXME: this method is a hack around the fact that we use a single cursor for all queries inside a connection,
     #   and this is required to fix get_multi_columns
     def get_multi_columns(
         self,
         connection: "Connection",
         schema: Optional[str] = None,
         filter_names: Optional[Set[str]] = None,
```

### Comparing `duckdb_engine-0.9.4/duckdb_engine/config.py` & `duckdb_engine-0.9.5/duckdb_engine/config.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.9.4/duckdb_engine/datatypes.py` & `duckdb_engine-0.9.5/duckdb_engine/datatypes.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.9.4/duckdb_engine/tests/conftest.py` & `duckdb_engine-0.9.5/duckdb_engine/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.9.4/duckdb_engine/tests/test_basic.py` & `duckdb_engine-0.9.5/duckdb_engine/tests/test_basic.py`

 * *Files 7% similar despite different names*

```diff
@@ -158,30 +158,27 @@
 
     owner = session.query(Owner).one()  # act
 
     assert owner.owned.name == s
 
 
 def test_get_tables(inspector: Inspector) -> None:
-    assert inspector.get_table_names()
+    for table_name in inspector.get_table_names():
+        assert inspector.has_table(table_name)
     assert inspector.get_view_names() == []
 
 
 @mark.skipif(
     supports_attach is False,
     reason="ATTACH is not supported for DuckDB version < 0.7.0",
 )
 def test_get_schema_names(inspector: Inspector, session: Session) -> None:
     # Using multi-line strings because of all the single and double quotes flying around...
     cmds = [
         """CREATE SCHEMA "quack quack" """,
-        """ATTACH ':memory:' AS "daffy duck" """,
-        """CREATE SCHEMA "daffy duck"."quack quack" """,
-        """CREATE TABLE "daffy duck"."quack quack"."t1" (i INTEGER, j INTEGER);""",
-        """CREATE TABLE "daffy duck"."quack quack"."t2" (i INTEGER, j INTEGER);""",
         """CREATE SCHEMA "daffy duck"."you're "" despicable" """,
     ]
     for cmd in cmds:
         session.execute(text(cmd))
         session.commit()
 
     # Deliberately excluding pg_catalog schema (to align with Postgres)
@@ -199,20 +196,43 @@
             "system.main",
             "temp.information_schema",
             "temp.main",
         ]
     else:
         assert names == ["quack quack", "information_schema", "main", "temp"]
 
-    table_names = inspector.get_table_names(schema='"daffy duck"."quack quack"')
-    assert set(table_names) == {"t1", "t2"}
+
+@mark.skipif(
+    supports_attach is False,
+    reason="ATTACH is not supported for DuckDB version < 0.7.0",
+)
+def test_get_table_names(inspector: Inspector, session: Session) -> None:
+    # Using multi-line strings because of all the single and double quotes flying around...
+    cmds = [
+        """CREATE TABLE "daffy duck"."quack quack"."t2" (i INTEGER, j INTEGER);""",
+        """CREATE TABLE "t3" (i INTEGER, j INTEGER);""",
+        """CREATE SCHEMA "porky" """,
+        """CREATE TABLE "porky"."t4" (i INTEGER, j INTEGER);""",
+    ]
+    for cmd in cmds:
+        session.execute(text(cmd))
+        session.commit()
+
+    for schema, table_names in zip(
+        ['"daffy duck"."quack quack"', "main", "porky"], [["t1", "t2"], ["t3"], ["t4"]]
+    ):
+        _table_names = inspector.get_table_names(schema=schema)
+        assert set(_table_names).issuperset(set(table_names))
+        for _table_name in _table_names:
+            assert inspector.has_table(_table_name, schema)
 
     table_names_all = inspector.get_table_names()
-    assert "t1" in table_names_all
-    assert "t2" in table_names_all
+    assert set(table_names_all).issuperset({"t1", "t2", "t3", "t4"})
+    for table_name in table_names_all:
+        assert inspector.has_table(table_name)
 
 
 def test_get_views(engine: Engine) -> None:
     con = engine.connect()
     views = engine.dialect.get_view_names(con)
     assert views == []
 
@@ -245,41 +265,61 @@
         conn.execute(
             text("SELECT * FROM read_parquet('https://domain/path/to/file.parquet');")
         )
 
 
 @fixture
 def inspector(engine: Engine, session: Session) -> Inspector:
-    session.execute(text("create table test (id int);"))
-    session.commit()
+    cmds = [
+        """CREATE TABLE test (id INTEGER);""" """ATTACH ':memory:' AS "daffy duck" """,
+        """CREATE SCHEMA "daffy duck"."quack quack" """,
+        """CREATE TABLE "daffy duck"."quack quack"."t1" (i INTEGER, j INTEGER);""",
+    ]
+    for cmd in cmds:
+        session.execute(text(cmd))
+        session.commit()
 
     meta = MetaData()
     Table("test", meta)
 
     return inspect(engine)
 
 
-def test_get_columns(inspector: Inspector) -> None:
-    inspector.get_columns("test", None)
+def test_get_columns(inspector: Inspector, session: Session) -> None:
+    cols = inspector.get_columns("test", None)
+    assert len(cols) == 1
+    assert cols[0]["name"] == "id"
+    assert inspector.has_table("t1", '"daffy duck"."quack quack"')
+    cols1 = inspector.get_columns("t1", None)
+    cols2 = inspector.get_columns("t1", '"daffy duck"."quack quack"')
+    cols3 = inspector.get_columns("t1", "daffy duck.quack quack")
+    assert len(cols1) == 2
+    assert cols1[0]["name"] == "i"
+    assert cols1[1]["name"] == "j"
+    assert cols1[0]["name"] == cols2[0]["name"] == cols3[0]["name"]
+    assert cols1[1]["name"] == cols2[1]["name"] == cols3[1]["name"]
 
 
 def test_get_foreign_keys(inspector: Inspector) -> None:
-    inspector.get_foreign_keys("test", None)
+    assert inspector.get_foreign_keys("test", None) == []
+    assert inspector.get_foreign_keys("t1", '"daffy duck"."quack quack"') == []
 
 
 @mark.skipif(
     Version(sqlalchemy.__version__) < Version("2.0.0"),
     reason="2-arg pg_getconstraintdef not yet supported in duckdb",
 )
 def test_get_check_constraints(inspector: Inspector) -> None:
     assert inspector.get_check_constraints("test", None) == []
+    assert inspector.get_check_constraints("t1", '"daffy duck"."quack quack"') == []
 
 
 def test_get_unique_constraints(inspector: Inspector) -> None:
     inspector.get_unique_constraints("test", None)
+    inspector.get_unique_constraints("t1", '"daffy duck"."quack quack"')
 
 
 def test_reflect(session: Session, engine: Engine) -> None:
     session.execute(text("create table test (id int);"))
     session.commit()
 
     meta = MetaData()
```

### Comparing `duckdb_engine-0.9.4/duckdb_engine/tests/test_datatypes.py` & `duckdb_engine-0.9.5/duckdb_engine/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.9.4/duckdb_engine/tests/test_ibis.py` & `duckdb_engine-0.9.5/duckdb_engine/tests/test_ibis.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.9.4/duckdb_engine/tests/test_integration.py` & `duckdb_engine-0.9.5/duckdb_engine/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.9.4/duckdb_engine/tests/test_pandas.py` & `duckdb_engine-0.9.5/duckdb_engine/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.9.4/pyproject.toml` & `duckdb_engine-0.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "duckdb_engine"
-version = "0.9.4"
+version = "0.9.5"
 description = "SQLAlchemy driver for duckdb"
 authors = ["Elliana <me@mause.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Mause/duckdb_engine"
 
 [tool.poetry.urls]
```

### Comparing `duckdb_engine-0.9.4/PKG-INFO` & `duckdb_engine-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckdb_engine
-Version: 0.9.4
+Version: 0.9.5
 Summary: SQLAlchemy driver for duckdb
 Home-page: https://github.com/Mause/duckdb_engine
 License: MIT
 Author: Elliana
 Author-email: me@mause.me
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
```

