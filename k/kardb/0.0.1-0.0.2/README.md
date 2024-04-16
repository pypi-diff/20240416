# Comparing `tmp/kardb-0.0.1.tar.gz` & `tmp/kardb-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kardb-0.0.1.tar", last modified: Thu Apr 11 17:20:08 2024, max compression
+gzip compressed data, was "kardb-0.0.2.tar", last modified: Tue Apr 16 17:22:58 2024, max compression
```

## Comparing `kardb-0.0.1.tar` & `kardb-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 17:20:08.768872 kardb-0.0.1/
--rw-rw-rw-   0        0        0     1087 2024-04-03 15:08:46.000000 kardb-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      277 2024-04-11 17:20:08.768872 kardb-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2024-04-11 16:31:33.000000 kardb-0.0.1/README.md
--rw-rw-rw-   0        0        0       82 2024-04-11 16:43:29.000000 kardb-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-11 17:20:08.768872 kardb-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      354 2024-04-11 16:53:39.000000 kardb-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:20:08.753248 kardb-0.0.1/src/
--rw-rw-rw-   0        0        0        0 2024-04-03 15:13:07.000000 kardb-0.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:20:08.768872 kardb-0.0.1/src/kardb.egg-info/
--rw-rw-rw-   0        0        0      277 2024-04-11 17:20:08.000000 kardb-0.0.1/src/kardb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-04-11 17:20:08.000000 kardb-0.0.1/src/kardb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 17:20:08.000000 kardb-0.0.1/src/kardb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-11 17:20:08.000000 kardb-0.0.1/src/kardb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2024-04-11 17:20:08.000000 kardb-0.0.1/src/kardb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5662 2024-04-03 15:10:14.000000 kardb-0.0.1/src/kardb_local.py
--rw-rw-rw-   0        0        0     3148 2024-04-10 15:46:34.000000 kardb-0.0.1/src/kardb_mysql.py
+drwxrwxrwx   0        0        0        0 2024-04-16 17:22:58.691201 kardb-0.0.2/
+-rw-rw-rw-   0        0        0     1087 2024-04-03 15:08:46.000000 kardb-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      277 2024-04-16 17:22:58.691201 kardb-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2024-04-11 16:31:33.000000 kardb-0.0.2/README.md
+-rw-rw-rw-   0        0        0       82 2024-04-11 16:43:29.000000 kardb-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 17:22:58.691201 kardb-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      354 2024-04-16 17:07:48.000000 kardb-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 17:22:58.675599 kardb-0.0.2/src/
+-rw-rw-rw-   0        0        0        0 2024-04-03 15:13:07.000000 kardb-0.0.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 17:22:58.691201 kardb-0.0.2/src/kardb.egg-info/
+-rw-rw-rw-   0        0        0      277 2024-04-16 17:22:58.000000 kardb-0.0.2/src/kardb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-04-16 17:22:58.000000 kardb-0.0.2/src/kardb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 17:22:58.000000 kardb-0.0.2/src/kardb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-16 17:22:58.000000 kardb-0.0.2/src/kardb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2024-04-16 17:22:58.000000 kardb-0.0.2/src/kardb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5686 2024-04-16 17:16:41.000000 kardb-0.0.2/src/kardb_local.py
+-rw-rw-rw-   0        0        0     3435 2024-04-13 14:36:39.000000 kardb-0.0.2/src/kardb_mysql.py
```

### Comparing `kardb-0.0.1/LICENSE` & `kardb-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kardb-0.0.1/README.md` & `kardb-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `kardb-0.0.1/src/kardb_local.py` & `kardb-0.0.2/src/kardb_local.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         The document is set to be main. Either the directory is created if it does not exists or the file is loaded up.
         
         Args:
             dbname (str): The name of the database.
         """
         self.dbname = dbname
         self.docname = 'main'
+        self.data = {}
         self.createdirs()
         self.load()
 
 
     def load(self):
         """Loads the current document's data for usage. The data will be {} if the file does not exist.
         """
```

### Comparing `kardb-0.0.1/src/kardb_mysql.py` & `kardb-0.0.2/src/kardb_mysql.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,27 +100,38 @@
         query = f"""drop table {docname}"""
         self.mycursor.execute(query)
 
     def cacdoc(self, docname):
         self.createdoc(docname)
         self.changedoc(docname)
 
-    def updatedoc(self, branch):
-        self.data.update(branch)
+    def savedoc(self):
+        json_data = json.dumps(self.data)
+
+        query = f"""update {self.docname}
+        set data = '{json_data}'"""
+        self.mycursor.execute(query)
 
         self.db.commit()
 
-    def save(self):
-        changeddata = self.data.copy()
+    def updatedoc(self,branch = None):
+        if not (branch == None) :
+            changeddata = branch
+
+        else:
+            changeddata = self.data.copy()
 
         streamdata = self.loaddoc()
         if streamdata == None:
             streamdata = {}
 
         streamdata.update(changeddata)
         streamdata = json.dumps(streamdata)
 
         query = f"""update {self.docname}
-set data = '{streamdata}'"""
+        set data = '{streamdata}'"""
         self.mycursor.execute(query)
 
+        self.db.commit()
+
+    def commit(self):
         self.db.commit()
```

