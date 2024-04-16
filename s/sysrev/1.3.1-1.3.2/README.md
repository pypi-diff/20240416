# Comparing `tmp/sysrev-1.3.1.tar.gz` & `tmp/sysrev-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysrev-1.3.1.tar", last modified: Mon Apr 15 20:21:23 2024, max compression
+gzip compressed data, was "sysrev-1.3.2.tar", last modified: Tue Apr 16 12:25:06 2024, max compression
```

## Comparing `sysrev-1.3.1.tar` & `sysrev-1.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:21:23.443531 sysrev-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-15 20:21:23.443531 sysrev-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-15 20:21:17.000000 sysrev-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:21:23.443531 sysrev-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-15 20:21:17.000000 sysrev-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:21:23.443531 sysrev-1.3.1/sysrev/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 20:21:17.000000 sysrev-1.3.1/sysrev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-04-15 20:21:17.000000 sysrev-1.3.1/sysrev/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:21:23.443531 sysrev-1.3.1/sysrev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-15 20:21:23.000000 sysrev-1.3.1/sysrev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-15 20:21:23.000000 sysrev-1.3.1/sysrev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:21:23.000000 sysrev-1.3.1/sysrev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:21:23.000000 sysrev-1.3.1/sysrev.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 20:21:23.000000 sysrev-1.3.1/sysrev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 20:21:23.000000 sysrev-1.3.1/sysrev.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:21:23.443531 sysrev-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-15 20:21:17.000000 sysrev-1.3.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-15 20:21:17.000000 sysrev-1.3.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:25:06.192790 sysrev-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-16 12:25:06.192790 sysrev-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-16 12:24:51.000000 sysrev-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 12:25:06.192790 sysrev-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-16 12:24:51.000000 sysrev-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:25:06.192790 sysrev-1.3.2/sysrev/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-16 12:24:51.000000 sysrev-1.3.2/sysrev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-04-16 12:24:51.000000 sysrev-1.3.2/sysrev/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:25:06.192790 sysrev-1.3.2/sysrev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-16 12:25:06.000000 sysrev-1.3.2/sysrev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-16 12:25:06.000000 sysrev-1.3.2/sysrev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 12:25:06.000000 sysrev-1.3.2/sysrev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 12:25:06.000000 sysrev-1.3.2/sysrev.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 12:25:06.000000 sysrev-1.3.2/sysrev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 12:25:06.000000 sysrev-1.3.2/sysrev.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:25:06.192790 sysrev-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-16 12:24:51.000000 sysrev-1.3.2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-16 12:24:51.000000 sysrev-1.3.2/tests/test_utils.py
```

### Comparing `sysrev-1.3.1/PKG-INFO` & `sysrev-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysrev
-Version: 1.3.1
+Version: 1.3.2
 Summary: get sysrev project data and use the sysrev api
 Home-page: https://github.com/sysrev/PySysrev
 Author: Thomas Luechtefeld
 Author-email: tom@insilica.co
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `sysrev-1.3.1/setup.py` & `sysrev-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Assuming your README file is in Markdown
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='sysrev',
-    version='1.3.1',
+    version='1.3.2',
     description='get sysrev project data and use the sysrev api',
     long_description=long_description,
     long_description_content_type='text/markdown',  # Specify the content type here
     url='https://github.com/sysrev/PySysrev',
     author='Thomas Luechtefeld',
     author_email='tom@insilica.co',
     packages=['sysrev'],
```

### Comparing `sysrev-1.3.1/sysrev/client.py` & `sysrev-1.3.2/sysrev/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -107,21 +107,41 @@
         article_labels = [lbl for lbls in article_labels for lbl in lbls]
         article_label_df = pd.DataFrame(article_labels)
         
         article_data = [{k: v for k, v in a.items() if k != 'labels'} for a in articles]
         article_data_df = pd.DataFrame(article_data)
         article_data_df['resolve'] = article_data_df['resolve'].apply(json.dumps)
         
+        article_info = []
+        for article_id in tqdm.tqdm(article_data_df['article-id'], total=n_articles):
+            article_info.append(client.get_article_info(project_id, article_id))
+        
+        full_texts = pd.DataFrame([{**ft} for a in article_info for ft in a['article'].get('full-texts', []) ])
+        full_texts.columns = [col.split('/')[-1] for col in full_texts.columns]
+        
+        auto_labels = pd.DataFrame([
+            {**{'article-id': a['article'].get('article-id'), 'label-id': label_id}, **details} for a in article_info
+            for label_id, details in a['article'].get('auto-labels', {}).items() ])
+        auto_labels['answer'] = auto_labels['answer'].apply(json.dumps)
+        
+        csl_citations = pd.DataFrame([
+            {**{k: json.dumps(v) if isinstance(v, (dict, list)) else v for k, v in item['itemData'].items()}, 
+             'article-id': a['article'].get('article-id')} 
+            for a in article_info for item in a['article'].get('csl-citation', {}).get('citationItems', [])])
+            
         # write everything to .sr/sr.sqlite
         conn = sqlite3.connect('.sr/sr.sqlite')
         
         # Writing data to tables
         labels_df.to_sql('labels', conn, if_exists='replace', index=False)
         article_label_df.to_sql('article_label', conn, if_exists='replace', index=False)
         article_data_df.to_sql('article_data', conn, if_exists='replace', index=False)
+        full_texts.to_sql('full_texts', conn, if_exists='replace', index=False)
+        auto_labels.to_sql('auto_labels', conn, if_exists='replace', index=False)
+        csl_citations.to_sql('csl_citations', conn, if_exists='replace', index=False)
         
         conn.close()
 class Client():
     
     def __init__(self, api_key, base_url="https://www.sysrev.com"):
         self.api_key = api_key
         self.base_url = base_url
@@ -181,15 +201,16 @@
             yield from articles  # Yield each article in the current batch
             offset += len(articles)
     
     def get_article_info(self, project_id, article_id):
         endpoint = f"{self.base_url}/api-json/article-info/{article_id}"
         headers = {"Authorization": f"Bearer {self.api_key}", "Content-Type": "application/json"}
         body = {"project-id": project_id,}
-        return requests.get(endpoint, headers=headers, json=body)
+        response = requests.get(endpoint, headers=headers, json=body)
+        return response.json()['result']
                    
     def upload_jsonlines(self, file_path, project_id):
         url = f"{self.base_url}/api-json/import-files/{project_id}"
         headers = {"Authorization": f"Bearer {self.api_key}"}
         
         # Prepare the file for upload
         with open(file_path, 'rb') as f:
```

### Comparing `sysrev-1.3.1/sysrev.egg-info/PKG-INFO` & `sysrev-1.3.2/sysrev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysrev
-Version: 1.3.1
+Version: 1.3.2
 Summary: get sysrev project data and use the sysrev api
 Home-page: https://github.com/sysrev/PySysrev
 Author: Thomas Luechtefeld
 Author-email: tom@insilica.co
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `sysrev-1.3.1/tests/test_client.py` & `sysrev-1.3.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `sysrev-1.3.1/tests/test_utils.py` & `sysrev-1.3.2/tests/test_utils.py`

 * *Files identical despite different names*

