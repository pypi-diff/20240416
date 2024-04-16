# Comparing `tmp/suql-1.1.3.tar.gz` & `tmp/suql-1.1.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suql-1.1.3.tar", last modified: Mon Apr 15 23:44:39 2024, max compression
+gzip compressed data, was "suql-1.1.4a0.tar", last modified: Tue Apr 16 20:55:51 2024, max compression
```

## Comparing `suql-1.1.3.tar` & `suql-1.1.4a0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwx------   0 oval      (1000) users      (100)        0 2024-04-15 23:44:39.257372 suql-1.1.3/
--rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.1.3/LICENSE
--rw-------   0 oval      (1000) users      (100)     4882 2024-04-15 23:44:39.253372 suql-1.1.3/PKG-INFO
--rw-------   0 oval      (1000) users      (100)     4278 2024-04-15 19:06:57.000000 suql-1.1.3/README.md
--rw-------   0 oval      (1000) users      (100)       38 2024-04-15 23:44:39.257372 suql-1.1.3/setup.cfg
--rw-------   0 oval      (1000) users      (100)     1512 2024-04-15 23:42:54.000000 suql-1.1.3/setup.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-15 23:44:39.253372 suql-1.1.3/src/
-drwx------   0 oval      (1000) users      (100)        0 2024-04-15 23:44:39.253372 suql-1.1.3/src/suql/
--rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.1.3/src/suql/__init__.py
--rw-------   0 oval      (1000) users      (100)    17354 2024-04-07 06:37:06.000000 suql-1.1.3/src/suql/agent.py
--rw-------   0 oval      (1000) users      (100)    16980 2024-04-07 05:13:01.000000 suql-1.1.3/src/suql/faiss_embedding.py
--rw-------   0 oval      (1000) users      (100)     8591 2024-04-12 01:46:05.000000 suql-1.1.3/src/suql/free_text_fcns_server.py
--rw-------   0 oval      (1000) users      (100)     3591 2024-04-12 01:45:49.000000 suql-1.1.3/src/suql/postgresql_connection.py
--rw-------   0 oval      (1000) users      (100)     9642 2024-04-12 01:46:33.000000 suql-1.1.3/src/suql/prompt_continuation.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-15 23:44:39.253372 suql-1.1.3/src/suql/prompts/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.1.3/src/suql/prompts/__init__.py
--rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.1.3/src/suql/prompts/answer_qa.prompt
--rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.1.3/src/suql/prompts/field_classification.prompt
--rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.1.3/src/suql/prompts/if_db_classification.prompt
--rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.1.3/src/suql/prompts/opening_hours.prompt
--rw-------   0 oval      (1000) users      (100)     5574 2024-04-03 06:02:28.000000 suql-1.1.3/src/suql/prompts/parser_suql.prompt
--rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.1.3/src/suql/prompts/verification.prompt
--rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.1.3/src/suql/prompts/yelp_response_SQL.prompt
--rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.1.3/src/suql/prompts/yelp_response_no_results.prompt
-drwx------   0 oval      (1000) users      (100)        0 2024-04-15 23:44:39.253372 suql-1.1.3/src/suql/sql_free_text_support/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.1.3/src/suql/sql_free_text_support/__init__.py
--rw-------   0 oval      (1000) users      (100)    62548 2024-04-12 01:44:28.000000 suql-1.1.3/src/suql/sql_free_text_support/execute_free_text_sql.py
--rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.1.3/src/suql/utils.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-15 23:44:39.253372 suql-1.1.3/src/suql.egg-info/
--rw-r--r--   0 oval      (1000) users      (100)     4882 2024-04-15 23:44:39.000000 suql-1.1.3/src/suql.egg-info/PKG-INFO
--rw-------   0 oval      (1000) users      (100)      824 2024-04-15 23:44:39.000000 suql-1.1.3/src/suql.egg-info/SOURCES.txt
--rw-------   0 oval      (1000) users      (100)        1 2024-04-15 23:44:39.000000 suql-1.1.3/src/suql.egg-info/dependency_links.txt
--rw-------   0 oval      (1000) users      (100)      186 2024-04-15 23:44:39.000000 suql-1.1.3/src/suql.egg-info/requires.txt
--rw-------   0 oval      (1000) users      (100)        5 2024-04-15 23:44:39.000000 suql-1.1.3/src/suql.egg-info/top_level.txt
+drwx------   0 oval      (1000) users      (100)        0 2024-04-16 20:55:51.281867 suql-1.1.4a0/
+-rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.1.4a0/LICENSE
+-rw-------   0 oval      (1000) users      (100)     4884 2024-04-16 20:55:51.281867 suql-1.1.4a0/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)     4278 2024-04-15 19:06:57.000000 suql-1.1.4a0/README.md
+-rw-------   0 oval      (1000) users      (100)       38 2024-04-16 20:55:51.281867 suql-1.1.4a0/setup.cfg
+-rw-------   0 oval      (1000) users      (100)     1514 2024-04-16 20:10:07.000000 suql-1.1.4a0/setup.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-16 20:55:51.277867 suql-1.1.4a0/src/
+drwx------   0 oval      (1000) users      (100)        0 2024-04-16 20:55:51.277867 suql-1.1.4a0/src/suql/
+-rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.1.4a0/src/suql/__init__.py
+-rw-------   0 oval      (1000) users      (100)    17354 2024-04-07 06:37:06.000000 suql-1.1.4a0/src/suql/agent.py
+-rw-------   0 oval      (1000) users      (100)    17524 2024-04-16 03:55:43.000000 suql-1.1.4a0/src/suql/faiss_embedding.py
+-rw-------   0 oval      (1000) users      (100)     8591 2024-04-12 01:46:05.000000 suql-1.1.4a0/src/suql/free_text_fcns_server.py
+-rw-------   0 oval      (1000) users      (100)     3591 2024-04-12 01:45:49.000000 suql-1.1.4a0/src/suql/postgresql_connection.py
+-rw-------   0 oval      (1000) users      (100)     9642 2024-04-12 01:46:33.000000 suql-1.1.4a0/src/suql/prompt_continuation.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-16 20:55:51.281867 suql-1.1.4a0/src/suql/prompts/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.1.4a0/src/suql/prompts/__init__.py
+-rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.1.4a0/src/suql/prompts/answer_qa.prompt
+-rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.1.4a0/src/suql/prompts/field_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.1.4a0/src/suql/prompts/if_db_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.1.4a0/src/suql/prompts/opening_hours.prompt
+-rw-------   0 oval      (1000) users      (100)     5574 2024-04-03 06:02:28.000000 suql-1.1.4a0/src/suql/prompts/parser_suql.prompt
+-rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.1.4a0/src/suql/prompts/verification.prompt
+-rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.1.4a0/src/suql/prompts/yelp_response_SQL.prompt
+-rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.1.4a0/src/suql/prompts/yelp_response_no_results.prompt
+drwx------   0 oval      (1000) users      (100)        0 2024-04-16 20:55:51.281867 suql-1.1.4a0/src/suql/sql_free_text_support/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.1.4a0/src/suql/sql_free_text_support/__init__.py
+-rw-------   0 oval      (1000) users      (100)    63679 2024-04-16 20:09:35.000000 suql-1.1.4a0/src/suql/sql_free_text_support/execute_free_text_sql.py
+-rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.1.4a0/src/suql/utils.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-16 20:55:51.277867 suql-1.1.4a0/src/suql.egg-info/
+-rw-r--r--   0 oval      (1000) users      (100)     4884 2024-04-16 20:55:51.000000 suql-1.1.4a0/src/suql.egg-info/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)      824 2024-04-16 20:55:51.000000 suql-1.1.4a0/src/suql.egg-info/SOURCES.txt
+-rw-------   0 oval      (1000) users      (100)        1 2024-04-16 20:55:51.000000 suql-1.1.4a0/src/suql.egg-info/dependency_links.txt
+-rw-------   0 oval      (1000) users      (100)      186 2024-04-16 20:55:51.000000 suql-1.1.4a0/src/suql.egg-info/requires.txt
+-rw-------   0 oval      (1000) users      (100)        5 2024-04-16 20:55:51.000000 suql-1.1.4a0/src/suql.egg-info/top_level.txt
```

### Comparing `suql-1.1.3/LICENSE` & `suql-1.1.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `suql-1.1.3/PKG-INFO` & `suql-1.1.4a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.1.3
+Version: 1.1.4a0
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.1.3 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.4a0 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `suql-1.1.3/README.md` & `suql-1.1.4a0/README.md`

 * *Files identical despite different names*

### Comparing `suql-1.1.3/setup.py` & `suql-1.1.4a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 # Package metadata
 name = "suql"
-version = "1.1.3"
+version = "1.1.4a0"
 description = "Structured and Unstructured Query Language (SUQL) Python API"
 author = "Shicheng Liu"
 author_email = "shicheng@cs.stanford.edu"
 url = "https://github.com/stanford-oval/suql"
 
 # Specify the packages to include. You can use `find_packages` to automatically discover them.
 packages = find_packages(where="src")
```

### Comparing `suql-1.1.3/src/suql/agent.py` & `suql-1.1.4a0/src/suql/agent.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.3/src/suql/faiss_embedding.py` & `suql-1.1.4a0/src/suql/faiss_embedding.py`

 * *Files 6% similar despite different names*

```diff
@@ -480,13 +480,31 @@
         table_name="restaurants",
         primary_key_field_name="_id",
         free_text_field_name="popular_dishes",
         db_name="restaurants",
         user="select_user",
         password="select_user",
     )
+    embedding_store.add(
+        table_name="courses",
+        primary_key_field_name="course_id",
+        free_text_field_name="description",
+        db_name="course_assistant"
+    )
+    embedding_store.add(
+        table_name="ratings",
+        primary_key_field_name="rating_id",
+        free_text_field_name="reviews",
+        db_name="course_assistant"
+    )
+    embedding_store.add(
+        table_name="programs",
+        primary_key_field_name="program_id",
+        free_text_field_name="sheet",
+        db_name="course_assistant"
+    )
 
     # Set the server address, if running through command line
     host = "127.0.0.1"
-    port = 8501
+    port = 8509
 
     embedding_store.start_embedding_server(host=host, port=port)
```

### Comparing `suql-1.1.3/src/suql/free_text_fcns_server.py` & `suql-1.1.4a0/src/suql/free_text_fcns_server.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.3/src/suql/postgresql_connection.py` & `suql-1.1.4a0/src/suql/postgresql_connection.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.3/src/suql/prompt_continuation.py` & `suql-1.1.4a0/src/suql/prompt_continuation.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.3/src/suql/prompts/if_db_classification.prompt` & `suql-1.1.4a0/src/suql/prompts/if_db_classification.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.3/src/suql/prompts/opening_hours.prompt` & `suql-1.1.4a0/src/suql/prompts/opening_hours.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.3/src/suql/prompts/parser_suql.prompt` & `suql-1.1.4a0/src/suql/prompts/parser_suql.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.3/src/suql/prompts/yelp_response_SQL.prompt` & `suql-1.1.4a0/src/suql/prompts/yelp_response_SQL.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.3/src/suql/prompts/yelp_response_no_results.prompt` & `suql-1.1.4a0/src/suql/prompts/yelp_response_no_results.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.3/src/suql/sql_free_text_support/execute_free_text_sql.py` & `suql-1.1.4a0/src/suql/sql_free_text_support/execute_free_text_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,52 @@
 
 def _if_contains_free_text_fcn(node):
     visitor = _FreeTextFcnVisitor()
     visitor(node)
     return visitor.res
 
 
+def _extract_all_free_text_fcns(suql):
+    node = parse_sql(suql)
+    visitor = _ExtractAllFreeTextFncs()
+    visitor(node)
+    return visitor.res
+
+
+class _ExtractAllFreeTextFncs(Visitor):
+    def __init__(self) -> None:
+        super().__init__()
+        self._SET_FREE_TEXT_FCNS = _SET_FREE_TEXT_FCNS
+        self.res = []
+
+    def __call__(self, node):
+        self.node = node
+        super().__call__(node)
+
+    def visit_FuncCall(self, ancestors, node: pglast.ast.FuncCall):
+        for i in node.funcname:
+            if i.sval in self._SET_FREE_TEXT_FCNS:
+                query_lst = list(
+                    filter(lambda x: isinstance(x, A_Const), node.args)
+                )
+                assert len(query_lst) == 1
+                query = query_lst[0].val.sval
+
+                field_lst = list(
+                    filter(lambda x: isinstance(x, ColumnRef), node.args)
+                )
+                assert len(field_lst) == 1
+
+                field = tuple(map(lambda x: x.sval, field_lst[0].fields))
+                    
+                self.res.append(
+                    (field, query)
+                )
+
+
 class _TypeCastAnswer(Visitor):
     def __init__(self) -> None:
         super().__init__()
 
     def __call__(self, node):
         super().__call__(node)
```

### Comparing `suql-1.1.3/src/suql/utils.py` & `suql-1.1.4a0/src/suql/utils.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.3/src/suql.egg-info/PKG-INFO` & `suql-1.1.4a0/src/suql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.1.3
+Version: 1.1.4a0
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.1.3 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.4a0 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `suql-1.1.3/src/suql.egg-info/SOURCES.txt` & `suql-1.1.4a0/src/suql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

