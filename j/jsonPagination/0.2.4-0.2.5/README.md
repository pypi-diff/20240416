# Comparing `tmp/jsonpagination-0.2.4.tar.gz` & `tmp/jsonpagination-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonpagination-0.2.4.tar", last modified: Mon Apr 15 15:14:37 2024, max compression
+gzip compressed data, was "jsonpagination-0.2.5.tar", last modified: Tue Apr 16 14:54:02 2024, max compression
```

## Comparing `jsonpagination-0.2.4.tar` & `jsonpagination-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:14:37.619175 jsonpagination-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35239 2024-04-15 15:14:33.000000 jsonpagination-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8419 2024-04-15 15:14:37.619175 jsonpagination-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7896 2024-04-15 15:14:33.000000 jsonpagination-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:14:37.619175 jsonpagination-0.2.4/jsonPagination/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-15 15:14:33.000000 jsonpagination-0.2.4/jsonPagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-15 15:14:33.000000 jsonpagination-0.2.4/jsonPagination/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17183 2024-04-15 15:14:33.000000 jsonpagination-0.2.4/jsonPagination/paginator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:14:37.619175 jsonpagination-0.2.4/jsonPagination.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8419 2024-04-15 15:14:37.000000 jsonpagination-0.2.4/jsonPagination.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-15 15:14:37.000000 jsonpagination-0.2.4/jsonPagination.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:14:37.000000 jsonpagination-0.2.4/jsonPagination.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 15:14:37.000000 jsonpagination-0.2.4/jsonPagination.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 15:14:37.000000 jsonpagination-0.2.4/jsonPagination.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 15:14:37.619175 jsonpagination-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-15 15:14:33.000000 jsonpagination-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:54:02.009350 jsonpagination-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35239 2024-04-16 14:53:58.000000 jsonpagination-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8419 2024-04-16 14:54:02.009350 jsonpagination-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7896 2024-04-16 14:53:58.000000 jsonpagination-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:54:02.005350 jsonpagination-0.2.5/jsonPagination/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-16 14:53:58.000000 jsonpagination-0.2.5/jsonPagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-16 14:53:58.000000 jsonpagination-0.2.5/jsonPagination/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17030 2024-04-16 14:53:58.000000 jsonpagination-0.2.5/jsonPagination/paginator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:54:02.009350 jsonpagination-0.2.5/jsonPagination.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8419 2024-04-16 14:54:01.000000 jsonpagination-0.2.5/jsonPagination.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-16 14:54:02.000000 jsonpagination-0.2.5/jsonPagination.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:54:01.000000 jsonpagination-0.2.5/jsonPagination.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 14:54:01.000000 jsonpagination-0.2.5/jsonPagination.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 14:54:01.000000 jsonpagination-0.2.5/jsonPagination.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:54:02.009350 jsonpagination-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-16 14:53:58.000000 jsonpagination-0.2.5/setup.py
```

### Comparing `jsonpagination-0.2.4/LICENSE` & `jsonpagination-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonpagination-0.2.4/PKG-INFO` & `jsonpagination-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonPagination
-Version: 0.2.4
+Version: 0.2.5
 Summary: A versatile JSON data downloader with pagination and multithreading support.
 Home-page: https://github.com/pl0psec/jsonPagination
 Author: pl0psec
 Author-email: contact@pl0psec.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jsonpagination-0.2.4/README.md` & `jsonpagination-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `jsonpagination-0.2.4/jsonPagination/exceptions.py` & `jsonpagination-0.2.5/jsonPagination/exceptions.py`

 * *Files identical despite different names*

### Comparing `jsonpagination-0.2.4/jsonPagination/paginator.py` & `jsonpagination-0.2.5/jsonPagination/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,20 +82,19 @@
 
         # Use `current_page_field` if provided, otherwise default to `current_index_field`        
         self.pagination_field = current_page_field if current_page_field else current_index_field
         self.is_page_based = bool(current_page_field)
 
         self.items_field = items_field
         self.total_count_field = total_count_field
-        self.items_per_page = items_per_page or 10
 
         self.data_field = data_field
 
-        self.items_per_page = items_per_page
-        self.response_items_field = response_items_field or items_per_page
+        self.items_per_page = items_per_page or 50
+        self.response_items_field = response_items_field
         self.download_one_page_only = download_one_page_only
 
         # Threading
         self.max_threads = max_threads
         self.retry = 5
         self.retry_delay = retry_delay
 
@@ -328,22 +327,21 @@
         json_data = response.json()
         total_count = json_data.get(self.total_count_field)
         if total_count is None:
             self.logger.warning("Total count field missing, cannot paginate properly.")
             return self.flatten_json(json_data) if flatten_json else json_data
 
         # Set items_per_page based on the initial API call if not set
-        # if not self.items_per_page:
-            # self.items_per_page = json_data.get(self.items_field, 200)  # Default to 200 if not specified
+        if not self.items_per_page:
 
-        # Set items_per_page based on the response, dynamically choosing the field or defaulting as necessary         
-        if self.response_items_field and self.response_items_field in json_data:
-            self.items_per_page = json_data.get(self.response_items_field)
-        else:
-            self.items_per_page = json_data.get(self.items_field, 200)
+            # Set items_per_page based on the response, dynamically choosing the field or defaulting as necessary         
+            if self.response_items_field and self.response_items_field in json_data:
+                self.items_per_page = json_data.get(self.response_items_field)
+            else:
+                self.items_per_page = json_data.get(self.items_field, 200)
 
         # Determine pagination strategy
         if self.is_page_based:
             total_pages = 1 if self.download_one_page_only else max(-(-total_count // self.items_per_page), 1)
         else:  # Index-based pagination
             # Calculate how many sets of data (each of size 'items_per_page') are needed to cover 'total_count'
             total_pages = 1 if self.download_one_page_only else max(-(-total_count // self.items_per_page), 1)
```

### Comparing `jsonpagination-0.2.4/jsonPagination.egg-info/PKG-INFO` & `jsonpagination-0.2.5/jsonPagination.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonPagination
-Version: 0.2.4
+Version: 0.2.5
 Summary: A versatile JSON data downloader with pagination and multithreading support.
 Home-page: https://github.com/pl0psec/jsonPagination
 Author: pl0psec
 Author-email: contact@pl0psec.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jsonpagination-0.2.4/setup.py` & `jsonpagination-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Read the contents of your README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='jsonPagination',
-    version='0.2.4',
+    version='0.2.5',
     author='pl0psec',
     author_email='contact@pl0psec.com',
     description='A versatile JSON data downloader with pagination and multithreading support.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/pl0psec/jsonPagination',
     packages=find_packages(),
```

