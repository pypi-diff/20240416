# Comparing `tmp/sysrev-1.3.2.tar.gz` & `tmp/sysrev-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysrev-1.3.2.tar", last modified: Tue Apr 16 12:25:06 2024, max compression
+gzip compressed data, was "sysrev-1.3.3.tar", last modified: Tue Apr 16 14:16:51 2024, max compression
```

## Comparing `sysrev-1.3.2.tar` & `sysrev-1.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:25:06.192790 sysrev-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-16 12:25:06.192790 sysrev-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-16 12:24:51.000000 sysrev-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 12:25:06.192790 sysrev-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-16 12:24:51.000000 sysrev-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:25:06.192790 sysrev-1.3.2/sysrev/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-16 12:24:51.000000 sysrev-1.3.2/sysrev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-04-16 12:24:51.000000 sysrev-1.3.2/sysrev/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:25:06.192790 sysrev-1.3.2/sysrev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-16 12:25:06.000000 sysrev-1.3.2/sysrev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-16 12:25:06.000000 sysrev-1.3.2/sysrev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 12:25:06.000000 sysrev-1.3.2/sysrev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 12:25:06.000000 sysrev-1.3.2/sysrev.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 12:25:06.000000 sysrev-1.3.2/sysrev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 12:25:06.000000 sysrev-1.3.2/sysrev.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:25:06.192790 sysrev-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-16 12:24:51.000000 sysrev-1.3.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-16 12:24:51.000000 sysrev-1.3.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:16:51.244837 sysrev-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-16 14:16:51.244837 sysrev-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-16 14:16:45.000000 sysrev-1.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:16:51.244837 sysrev-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-16 14:16:45.000000 sysrev-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:16:51.240837 sysrev-1.3.3/sysrev/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-16 14:16:45.000000 sysrev-1.3.3/sysrev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-04-16 14:16:45.000000 sysrev-1.3.3/sysrev/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:16:51.244837 sysrev-1.3.3/sysrev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-16 14:16:51.000000 sysrev-1.3.3/sysrev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-16 14:16:51.000000 sysrev-1.3.3/sysrev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:16:51.000000 sysrev-1.3.3/sysrev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:16:51.000000 sysrev-1.3.3/sysrev.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 14:16:51.000000 sysrev-1.3.3/sysrev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 14:16:51.000000 sysrev-1.3.3/sysrev.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:16:51.244837 sysrev-1.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-16 14:16:45.000000 sysrev-1.3.3/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-16 14:16:45.000000 sysrev-1.3.3/tests/test_utils.py
```

### Comparing `sysrev-1.3.2/PKG-INFO` & `sysrev-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysrev
-Version: 1.3.2
+Version: 1.3.3
 Summary: get sysrev project data and use the sysrev api
 Home-page: https://github.com/sysrev/PySysrev
 Author: Thomas Luechtefeld
 Author-email: tom@insilica.co
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `sysrev-1.3.2/setup.py` & `sysrev-1.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Assuming your README file is in Markdown
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='sysrev',
-    version='1.3.2',
+    version='1.3.3',
     description='get sysrev project data and use the sysrev api',
     long_description=long_description,
     long_description_content_type='text/markdown',  # Specify the content type here
     url='https://github.com/sysrev/PySysrev',
     author='Thomas Luechtefeld',
     author_email='tom@insilica.co',
     packages=['sysrev'],
```

### Comparing `sysrev-1.3.2/sysrev/client.py` & `sysrev-1.3.3/sysrev/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,15 +89,20 @@
         c.execute('CREATE INDEX IF NOT EXISTS idx_labels_project_id ON labels (project_id);')
         c.execute('CREATE INDEX IF NOT EXISTS idx_article_label_user_id ON article_label (user_id);')
 
         # Commit changes and close connection
         conn.commit()
         conn.close()
 
+    # TODO - this could be made more efficient by checking sqlite state and updating the sysrev api
     def sync(self, client, project_id):
+        # check that db exists
+        if not pathlib.Path('.sr/sr.sqlite').exists():
+            self.create_sqlite_db()
+            
         project_info = client.get_project_info(project_id)
         
         labels = client.get_labels(project_id)
         labels_df = pd.DataFrame(labels)
         labels_df['definition'] = labels_df['definition'].apply(json.dumps)
         
         n_articles = project_info['result']['project']['stats']['articles']
```

### Comparing `sysrev-1.3.2/sysrev.egg-info/PKG-INFO` & `sysrev-1.3.3/sysrev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysrev
-Version: 1.3.2
+Version: 1.3.3
 Summary: get sysrev project data and use the sysrev api
 Home-page: https://github.com/sysrev/PySysrev
 Author: Thomas Luechtefeld
 Author-email: tom@insilica.co
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `sysrev-1.3.2/tests/test_client.py` & `sysrev-1.3.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `sysrev-1.3.2/tests/test_utils.py` & `sysrev-1.3.3/tests/test_utils.py`

 * *Files identical despite different names*

