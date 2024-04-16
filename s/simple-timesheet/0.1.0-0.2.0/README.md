# Comparing `tmp/simple_timesheet-0.1.0.tar.gz` & `tmp/simple_timesheet-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_timesheet-0.1.0.tar", max compression
+gzip compressed data, was "simple_timesheet-0.2.0.tar", max compression
```

## Comparing `simple_timesheet-0.1.0.tar` & `simple_timesheet-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-03-06 09:07:53.498542 simple_timesheet-0.1.0/LICENSE
--rw-r--r--   0        0        0     1173 2024-03-06 11:36:35.282324 simple_timesheet-0.1.0/README.md
--rw-r--r--   0        0        0      434 2024-03-06 11:28:55.663797 simple_timesheet-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-06 09:14:18.893152 simple_timesheet-0.1.0/ts/__init__.py
--rwxr-xr-x   0        0        0       30 2024-03-06 11:25:39.098954 simple_timesheet-0.1.0/ts/__main__.py
--rw-r--r--   0        0        0     2676 2024-03-06 11:40:42.944393 simple_timesheet-0.1.0/ts/cli.py
--rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 simple_timesheet-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-06 09:07:53.498542 simple_timesheet-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1173 2024-03-06 11:36:35.282324 simple_timesheet-0.2.0/README.md
+-rw-r--r--   0        0        0      434 2024-04-16 18:02:18.059152 simple_timesheet-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-06 09:14:18.893152 simple_timesheet-0.2.0/ts/__init__.py
+-rwxr-xr-x   0        0        0       30 2024-03-06 11:25:39.098954 simple_timesheet-0.2.0/ts/__main__.py
+-rw-r--r--   0        0        0     3779 2024-04-16 18:02:08.978646 simple_timesheet-0.2.0/ts/cli.py
+-rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 simple_timesheet-0.2.0/PKG-INFO
```

### Comparing `simple_timesheet-0.1.0/LICENSE` & `simple_timesheet-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_timesheet-0.1.0/README.md` & `simple_timesheet-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `simple_timesheet-0.1.0/ts/cli.py` & `simple_timesheet-0.2.0/ts/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -37,14 +37,17 @@
     ctx.obj["db_file"] = db_file
 
 
 @cli.command()
 @click.argument("entry", type=str)
 @click.pass_context
 def add(ctx, entry):
+    """
+    Add an entry for today
+    """
     con = connect_db(ctx.obj["db_file"])
 
     cur = con.cursor()
     last_id = cur.execute("SELECT max(id) FROM timesheet").fetchone()[0]
     if last_id is None:
         next_id = 0
     else:
@@ -52,14 +55,56 @@
     cur.execute("INSERT INTO timesheet VALUES(?, ?, ?)", (next_id, date.today(), entry))
     con.commit()
     # con = sqlite3.connect(ctx.obj['db_file'])
 
 
 @cli.command()
 @click.pass_context
+def add_yesterday(ctx, entry):
+    """
+    Add an entry for yesterday
+    """
+    con = connect_db(ctx.obj["db_file"])
+
+    cur = con.cursor()
+    last_id = cur.execute("SELECT max(id) FROM timesheet").fetchone()[0]
+    if last_id is None:
+        next_id = 0
+    else:
+        next_id = last_id + 1
+    cur.execute(
+        "INSERT INTO timesheet VALUES(?, ?, ?)",
+        (next_id, date.today() - timedelta(1), entry),
+    )
+    con.commit()
+
+
+@cli.command()
+@click.argument("date", type=str)
+@click.argument("entry", type=str)
+@click.pass_context
+def add_date(ctx, date, entry):
+    """
+    Add an entry on a specific date in YYYY-MM-DD format
+    """
+    con = connect_db(ctx.obj["db_file"])
+
+    cur = con.cursor()
+    last_id = cur.execute("SELECT max(id) FROM timesheet").fetchone()[0]
+    if last_id is None:
+        next_id = 0
+    else:
+        next_id = last_id + 1
+    cur.execute("INSERT INTO timesheet VALUES(?, ?, ?)", (next_id, date, entry))
+    con.commit()
+    # con = sqlite3.connect(ctx.obj['db_file'])
+
+
+@cli.command()
+@click.pass_context
 def today(ctx):
     """
     Dump the timesheet string for today
     """
     con = connect_db(ctx.obj["db_file"])
     cur = con.cursor()
     ## fetch all the stuff for today
```

### Comparing `simple_timesheet-0.1.0/PKG-INFO` & `simple_timesheet-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-timesheet
-Version: 0.1.0
+Version: 0.2.0
 Summary: A CLI utility for adding entries to your timesheet
 License: Apache 2.0
 Author: Andrew Green
 Author-email: agreen@ebi.ac.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

