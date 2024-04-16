# Comparing `tmp/datasette_query_assistant-0.1a0.tar.gz` & `tmp/datasette_query_assistant-0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette_query_assistant-0.1a0.tar", last modified: Tue Apr 16 17:05:25 2024, max compression
+gzip compressed data, was "datasette_query_assistant-0.1a1.tar", last modified: Tue Apr 16 19:43:17 2024, max compression
```

## Comparing `datasette_query_assistant-0.1a0.tar` & `datasette_query_assistant-0.1a1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:25.891810 datasette_query_assistant-0.1a0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 17:05:19.000000 datasette_query_assistant-0.1a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-16 17:05:25.891810 datasette_query_assistant-0.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-16 17:05:19.000000 datasette_query_assistant-0.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:25.887810 datasette_query_assistant-0.1a0/datasette_query_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-04-16 17:05:19.000000 datasette_query_assistant-0.1a0/datasette_query_assistant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:25.891810 datasette_query_assistant-0.1a0/datasette_query_assistant/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-16 17:05:19.000000 datasette_query_assistant-0.1a0/datasette_query_assistant/templates/query_assistant.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:25.891810 datasette_query_assistant-0.1a0/datasette_query_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-16 17:05:25.000000 datasette_query_assistant-0.1a0/datasette_query_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-16 17:05:25.000000 datasette_query_assistant-0.1a0/datasette_query_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:05:25.000000 datasette_query_assistant-0.1a0/datasette_query_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-16 17:05:25.000000 datasette_query_assistant-0.1a0/datasette_query_assistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-16 17:05:25.000000 datasette_query_assistant-0.1a0/datasette_query_assistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 17:05:25.000000 datasette_query_assistant-0.1a0/datasette_query_assistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-16 17:05:19.000000 datasette_query_assistant-0.1a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 17:05:25.891810 datasette_query_assistant-0.1a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:25.891810 datasette_query_assistant-0.1a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-16 17:05:19.000000 datasette_query_assistant-0.1a0/tests/test_query_assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:43:17.862237 datasette_query_assistant-0.1a1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 19:43:10.000000 datasette_query_assistant-0.1a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-16 19:43:17.862237 datasette_query_assistant-0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-16 19:43:10.000000 datasette_query_assistant-0.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:43:17.862237 datasette_query_assistant-0.1a1/datasette_query_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-16 19:43:10.000000 datasette_query_assistant-0.1a1/datasette_query_assistant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:43:17.862237 datasette_query_assistant-0.1a1/datasette_query_assistant/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-16 19:43:10.000000 datasette_query_assistant-0.1a1/datasette_query_assistant/templates/query_assistant.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:43:17.862237 datasette_query_assistant-0.1a1/datasette_query_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-16 19:43:17.000000 datasette_query_assistant-0.1a1/datasette_query_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-16 19:43:17.000000 datasette_query_assistant-0.1a1/datasette_query_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:43:17.000000 datasette_query_assistant-0.1a1/datasette_query_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-16 19:43:17.000000 datasette_query_assistant-0.1a1/datasette_query_assistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-16 19:43:17.000000 datasette_query_assistant-0.1a1/datasette_query_assistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 19:43:17.000000 datasette_query_assistant-0.1a1/datasette_query_assistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-16 19:43:10.000000 datasette_query_assistant-0.1a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:43:17.862237 datasette_query_assistant-0.1a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:43:17.862237 datasette_query_assistant-0.1a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-16 19:43:10.000000 datasette_query_assistant-0.1a1/tests/test_query_assistant.py
```

### Comparing `datasette_query_assistant-0.1a0/LICENSE` & `datasette_query_assistant-0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette_query_assistant-0.1a0/PKG-INFO` & `datasette_query_assistant-0.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-query-assistant
-Version: 0.1a0
+Version: 0.1a1
 Summary: Query databases and tables with AI assistance
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-query-assistant
 Project-URL: Changelog, https://github.com/datasette/datasette-query-assistant/releases
 Project-URL: Issues, https://github.com/datasette/datasette-query-assistant/issues
 Project-URL: CI, https://github.com/datasette/datasette-query-assistant/actions
```

### Comparing `datasette_query_assistant-0.1a0/README.md` & `datasette_query_assistant-0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `datasette_query_assistant-0.1a0/datasette_query_assistant/__init__.py` & `datasette_query_assistant-0.1a1/datasette_query_assistant/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 async def get_schema(db, table=None):
     if table:
 
         def _related(conn):
             return get_related_tables(conn, table)
 
         tables = await db.execute_fn(_related)
+        tables.add(table)
         sql = SCHEMA_SQL_SPECIFIC.replace("PARAMS", ",".join("?" for _ in tables))
         return (await db.execute(sql, tuple(tables))).first()[0]
     else:
         return (await db.execute(SCHEMA_SQL)).first()[0]
 
 
 async def has_permission(datasette, actor, database):
```

### Comparing `datasette_query_assistant-0.1a0/datasette_query_assistant/templates/query_assistant.html` & `datasette_query_assistant-0.1a1/datasette_query_assistant/templates/query_assistant.html`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,18 @@
   </p>
   <p><textarea style="width: 80%; height: 3em;" name="question" id="id_question"></textarea>
   <p>
     <input type="hidden" name="csrftoken" value="{{ csrftoken() }}">
     <input type="hidden" name="table" value="{{ table }}">
     <input type="submit" value="Submit">
   </p>
+</form>
 
 <details><summary>Schema that will be passed to the model</summary>
 <pre>{{ schema }}</pre>
 </details>
 
 <script>
-  document.querySelector('textarea[name=question]').focus();
+  document.querySelector('#id_question').focus();
 </script>
 
 {% endblock %}
```

### Comparing `datasette_query_assistant-0.1a0/datasette_query_assistant.egg-info/PKG-INFO` & `datasette_query_assistant-0.1a1/datasette_query_assistant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-query-assistant
-Version: 0.1a0
+Version: 0.1a1
 Summary: Query databases and tables with AI assistance
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-query-assistant
 Project-URL: Changelog, https://github.com/datasette/datasette-query-assistant/releases
 Project-URL: Issues, https://github.com/datasette/datasette-query-assistant/issues
 Project-URL: CI, https://github.com/datasette/datasette-query-assistant/actions
```

### Comparing `datasette_query_assistant-0.1a0/pyproject.toml` & `datasette_query_assistant-0.1a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "datasette-query-assistant"
-version = "0.1a0"
+version = "0.1a1"
 description = "Query databases and tables with AI assistance"
 readme = "README.md"
 authors = [{name = "Simon Willison"}]
 license = {text = "Apache-2.0"}
 classifiers=[
     "Framework :: Datasette",
     "License :: OSI Approved :: Apache Software License"
```

### Comparing `datasette_query_assistant-0.1a0/tests/test_query_assistant.py` & `datasette_query_assistant-0.1a1/tests/test_query_assistant.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,51 @@
 from datasette.app import Datasette
 from datasette_query_assistant import get_related_tables
+import pytest_asyncio
 import pytest
 import sqlite_utils
 
 
-@pytest.mark.asyncio
-async def test_plugin_is_installed():
-    datasette = Datasette(memory=True)
-    response = await datasette.client.get("/-/plugins.json")
-    assert response.status_code == 200
-    installed_plugins = {p["name"] for p in response.json()}
-    assert "datasette-query-assistant" in installed_plugins
+@pytest_asyncio.fixture
+async def datasette():
+    ds = Datasette()
+    db = ds.add_memory_database("test")
+    await db.execute_write(
+        "create table if not exists foo (id integer primary key, name text)"
+    )
+    return ds
 
 
 def test_get_related_tables():
     db = sqlite_utils.Database(memory=True)
     db["foo.bar.baz"].insert({"id": 1}, pk="id")
     db["species"].insert({"id": 1, "name": "Dog"}, pk="id")
     db["animals"].insert(
         {"id": 1, "name": "Cleo", "species": 1},
         pk="id",
         foreign_keys=(("species", "species", "id"),),
     )
     assert get_related_tables(db.conn, "foo.bar.baz") == set()
     assert get_related_tables(db.conn, "species") == {"species", "animals"}
     assert get_related_tables(db.conn, "animals") == {"species", "animals"}
+
+
+@pytest.mark.asyncio
+async def test_database_assistant_page(datasette):
+    response = await datasette.client.get("/test/-/assistant")
+    assert response.status_code == 200
+    assert "Query assistant for test" in response.text
+    assert (
+        "<pre>CREATE TABLE foo (id integer primary key, name text)</pre>"
+        in response.text
+    )
+
+
+@pytest.mark.asyncio
+async def test_table_assistant_page(datasette):
+    response = await datasette.client.get("/test/-/assistant?table=foo")
+    assert response.status_code == 200
+    assert "Query assistant for foo" in response.text
+    assert (
+        "<pre>CREATE TABLE foo (id integer primary key, name text)</pre>"
+        in response.text
+    )
```

