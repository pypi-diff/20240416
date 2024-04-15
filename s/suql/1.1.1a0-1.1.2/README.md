# Comparing `tmp/suql-1.1.1a0.tar.gz` & `tmp/suql-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suql-1.1.1a0.tar", last modified: Thu Apr 11 05:10:46 2024, max compression
+gzip compressed data, was "suql-1.1.2.tar", last modified: Mon Apr 15 05:33:20 2024, max compression
```

## Comparing `suql-1.1.1a0.tar` & `suql-1.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwx------   0 oval      (1000) users      (100)        0 2024-04-11 05:10:46.182489 suql-1.1.1a0/
--rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.1.1a0/LICENSE
--rw-------   0 oval      (1000) users      (100)     4912 2024-04-11 05:10:46.182489 suql-1.1.1a0/PKG-INFO
--rw-------   0 oval      (1000) users      (100)     4306 2024-04-08 18:37:27.000000 suql-1.1.1a0/README.md
--rw-------   0 oval      (1000) users      (100)       38 2024-04-11 05:10:46.182489 suql-1.1.1a0/setup.cfg
--rw-------   0 oval      (1000) users      (100)     1535 2024-04-10 21:17:54.000000 suql-1.1.1a0/setup.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-11 05:10:46.166489 suql-1.1.1a0/src/
-drwx------   0 oval      (1000) users      (100)        0 2024-04-11 05:10:46.174489 suql-1.1.1a0/src/suql/
--rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.1.1a0/src/suql/__init__.py
--rw-------   0 oval      (1000) users      (100)    17354 2024-04-07 06:37:06.000000 suql-1.1.1a0/src/suql/agent.py
--rw-------   0 oval      (1000) users      (100)    16980 2024-04-07 05:13:01.000000 suql-1.1.1a0/src/suql/faiss_embedding.py
--rw-------   0 oval      (1000) users      (100)     8646 2024-04-06 00:50:57.000000 suql-1.1.1a0/src/suql/free_text_fcns_server.py
--rw-------   0 oval      (1000) users      (100)     4095 2024-04-03 06:02:28.000000 suql-1.1.1a0/src/suql/postgresql_connection.py
--rw-------   0 oval      (1000) users      (100)     9870 2024-04-10 21:17:41.000000 suql-1.1.1a0/src/suql/prompt_continuation.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-11 05:10:46.182489 suql-1.1.1a0/src/suql/prompts/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.1.1a0/src/suql/prompts/__init__.py
--rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.1.1a0/src/suql/prompts/answer_qa.prompt
--rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.1.1a0/src/suql/prompts/field_classification.prompt
--rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.1.1a0/src/suql/prompts/if_db_classification.prompt
--rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.1.1a0/src/suql/prompts/opening_hours.prompt
--rw-------   0 oval      (1000) users      (100)     5574 2024-04-03 06:02:28.000000 suql-1.1.1a0/src/suql/prompts/parser_suql.prompt
--rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.1.1a0/src/suql/prompts/verification.prompt
--rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.1.1a0/src/suql/prompts/yelp_response_SQL.prompt
--rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.1.1a0/src/suql/prompts/yelp_response_no_results.prompt
-drwx------   0 oval      (1000) users      (100)        0 2024-04-11 05:10:46.182489 suql-1.1.1a0/src/suql/sql_free_text_support/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.1.1a0/src/suql/sql_free_text_support/__init__.py
--rw-------   0 oval      (1000) users      (100)    62450 2024-04-11 05:09:58.000000 suql-1.1.1a0/src/suql/sql_free_text_support/execute_free_text_sql.py
--rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.1.1a0/src/suql/utils.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-11 05:10:46.174489 suql-1.1.1a0/src/suql.egg-info/
--rw-r--r--   0 oval      (1000) users      (100)     4912 2024-04-11 05:10:46.000000 suql-1.1.1a0/src/suql.egg-info/PKG-INFO
--rw-------   0 oval      (1000) users      (100)      824 2024-04-11 05:10:46.000000 suql-1.1.1a0/src/suql.egg-info/SOURCES.txt
--rw-------   0 oval      (1000) users      (100)        1 2024-04-11 05:10:46.000000 suql-1.1.1a0/src/suql.egg-info/dependency_links.txt
--rw-------   0 oval      (1000) users      (100)      200 2024-04-11 05:10:46.000000 suql-1.1.1a0/src/suql.egg-info/requires.txt
--rw-------   0 oval      (1000) users      (100)        5 2024-04-11 05:10:46.000000 suql-1.1.1a0/src/suql.egg-info/top_level.txt
+drwx------   0 oval      (1000) users      (100)        0 2024-04-15 05:33:20.494491 suql-1.1.2/
+-rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.1.2/LICENSE
+-rw-------   0 oval      (1000) users      (100)     4905 2024-04-15 05:33:20.494491 suql-1.1.2/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)     4301 2024-04-12 20:00:15.000000 suql-1.1.2/README.md
+-rw-------   0 oval      (1000) users      (100)       38 2024-04-15 05:33:20.494491 suql-1.1.2/setup.cfg
+-rw-------   0 oval      (1000) users      (100)     1512 2024-04-11 20:48:38.000000 suql-1.1.2/setup.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-15 05:33:20.486491 suql-1.1.2/src/
+drwx------   0 oval      (1000) users      (100)        0 2024-04-15 05:33:20.490491 suql-1.1.2/src/suql/
+-rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.1.2/src/suql/__init__.py
+-rw-------   0 oval      (1000) users      (100)    17354 2024-04-07 06:37:06.000000 suql-1.1.2/src/suql/agent.py
+-rw-------   0 oval      (1000) users      (100)    16980 2024-04-07 05:13:01.000000 suql-1.1.2/src/suql/faiss_embedding.py
+-rw-------   0 oval      (1000) users      (100)     8591 2024-04-12 01:46:05.000000 suql-1.1.2/src/suql/free_text_fcns_server.py
+-rw-------   0 oval      (1000) users      (100)     3591 2024-04-12 01:45:49.000000 suql-1.1.2/src/suql/postgresql_connection.py
+-rw-------   0 oval      (1000) users      (100)     9642 2024-04-12 01:46:33.000000 suql-1.1.2/src/suql/prompt_continuation.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-15 05:33:20.494491 suql-1.1.2/src/suql/prompts/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.1.2/src/suql/prompts/__init__.py
+-rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.1.2/src/suql/prompts/answer_qa.prompt
+-rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.1.2/src/suql/prompts/field_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.1.2/src/suql/prompts/if_db_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.1.2/src/suql/prompts/opening_hours.prompt
+-rw-------   0 oval      (1000) users      (100)     5574 2024-04-03 06:02:28.000000 suql-1.1.2/src/suql/prompts/parser_suql.prompt
+-rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.1.2/src/suql/prompts/verification.prompt
+-rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.1.2/src/suql/prompts/yelp_response_SQL.prompt
+-rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.1.2/src/suql/prompts/yelp_response_no_results.prompt
+drwx------   0 oval      (1000) users      (100)        0 2024-04-15 05:33:20.494491 suql-1.1.2/src/suql/sql_free_text_support/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.1.2/src/suql/sql_free_text_support/__init__.py
+-rw-------   0 oval      (1000) users      (100)    62548 2024-04-12 01:44:28.000000 suql-1.1.2/src/suql/sql_free_text_support/execute_free_text_sql.py
+-rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.1.2/src/suql/utils.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-15 05:33:20.490491 suql-1.1.2/src/suql.egg-info/
+-rw-r--r--   0 oval      (1000) users      (100)     4905 2024-04-15 05:33:20.000000 suql-1.1.2/src/suql.egg-info/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)      824 2024-04-15 05:33:20.000000 suql-1.1.2/src/suql.egg-info/SOURCES.txt
+-rw-------   0 oval      (1000) users      (100)        1 2024-04-15 05:33:20.000000 suql-1.1.2/src/suql.egg-info/dependency_links.txt
+-rw-------   0 oval      (1000) users      (100)      186 2024-04-15 05:33:20.000000 suql-1.1.2/src/suql.egg-info/requires.txt
+-rw-------   0 oval      (1000) users      (100)        5 2024-04-15 05:33:20.000000 suql-1.1.2/src/suql.egg-info/top_level.txt
```

### Comparing `suql-1.1.1a0/LICENSE` & `suql-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `suql-1.1.1a0/PKG-INFO` & `suql-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.1.1a0
+Version: 1.1.2
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -70,15 +70,15 @@
 
 ## Install from `pip`
 
 Ideal for integrating the SUQL compiler in a larger codebase / system. See [install_pip.md](https://github.com/stanford-oval/suql/blob/main/docs/install_pip.md) for details.
 
 ## Install from source
 
-Ideal for using this repo to build a SUQL-powered conversational interface to your data out-of-the-box, like the one for https://yelpbot.genie.stanford.edu discussed in the paper. See [docs/install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/install_source.md) for details.
+Ideal for using this repo to build a SUQL-powered conversational interface to your data out-of-the-box, like the one for https://yelpbot.genie.stanford.edu discussed in the paper. See [install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/install_source.md) for details.
 
 ## Agent tutorial
 
 Check out [conv_agent.md](https://github.com/stanford-oval/suql/blob/main/docs/conv_agent.md) for more information on best practices for using SUQL to power your conversational agent.
 
 # Bugs / Contribution
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.1.1a0 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.2 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
@@ -35,15 +35,15 @@
 https://arxiv.org/abs/2311.09818. # Installation / Usage tutorial There are two
 main ways of installing the SUQL library. ## Install from `pip` Ideal for
 integrating the SUQL compiler in a larger codebase / system. See
 [install_pip.md](https://github.com/stanford-oval/suql/blob/main/docs/
 install_pip.md) for details. ## Install from source Ideal for using this repo
 to build a SUQL-powered conversational interface to your data out-of-the-box,
 like the one for https://yelpbot.genie.stanford.edu discussed in the paper. See
-[docs/install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/
+[install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/
 install_source.md) for details. ## Agent tutorial Check out [conv_agent.md]
 (https://github.com/stanford-oval/suql/blob/main/docs/conv_agent.md) for more
 information on best practices for using SUQL to power your conversational
 agent. # Bugs / Contribution If you encounter a problem, first check
 [known_issues.md](https://github.com/stanford-oval/suql/blob/main/docs/
 known_issues.md). If it is not listed there, we welcome Issues and/or PRs! #
 Paper results To replicate our results on HybridQA and restaurants in our
```

### Comparing `suql-1.1.1a0/README.md` & `suql-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 ## Install from `pip`
 
 Ideal for integrating the SUQL compiler in a larger codebase / system. See [install_pip.md](https://github.com/stanford-oval/suql/blob/main/docs/install_pip.md) for details.
 
 ## Install from source
 
-Ideal for using this repo to build a SUQL-powered conversational interface to your data out-of-the-box, like the one for https://yelpbot.genie.stanford.edu discussed in the paper. See [docs/install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/install_source.md) for details.
+Ideal for using this repo to build a SUQL-powered conversational interface to your data out-of-the-box, like the one for https://yelpbot.genie.stanford.edu discussed in the paper. See [install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/install_source.md) for details.
 
 ## Agent tutorial
 
 Check out [conv_agent.md](https://github.com/stanford-oval/suql/blob/main/docs/conv_agent.md) for more information on best practices for using SUQL to power your conversational agent.
 
 # Bugs / Contribution
```

#### html2text {}

```diff
@@ -27,15 +27,15 @@
 https://arxiv.org/abs/2311.09818. # Installation / Usage tutorial There are two
 main ways of installing the SUQL library. ## Install from `pip` Ideal for
 integrating the SUQL compiler in a larger codebase / system. See
 [install_pip.md](https://github.com/stanford-oval/suql/blob/main/docs/
 install_pip.md) for details. ## Install from source Ideal for using this repo
 to build a SUQL-powered conversational interface to your data out-of-the-box,
 like the one for https://yelpbot.genie.stanford.edu discussed in the paper. See
-[docs/install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/
+[install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/
 install_source.md) for details. ## Agent tutorial Check out [conv_agent.md]
 (https://github.com/stanford-oval/suql/blob/main/docs/conv_agent.md) for more
 information on best practices for using SUQL to power your conversational
 agent. # Bugs / Contribution If you encounter a problem, first check
 [known_issues.md](https://github.com/stanford-oval/suql/blob/main/docs/
 known_issues.md). If it is not listed there, we welcome Issues and/or PRs! #
 Paper results To replicate our results on HybridQA and restaurants in our
```

### Comparing `suql-1.1.1a0/setup.py` & `suql-1.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from setuptools import find_packages, setup
 
 # Package metadata
 name = "suql"
-version = "1.1.1a0"
+version = "1.1.2"
 description = "Structured and Unstructured Query Language (SUQL) Python API"
 author = "Shicheng Liu"
 author_email = "shicheng@cs.stanford.edu"
 url = "https://github.com/stanford-oval/suql"
 
 # Specify the packages to include. You can use `find_packages` to automatically discover them.
 packages = find_packages(where="src")
 
 # Define your dependencies
 install_requires = [
-    'openai==1.3.2',
     'Jinja2==3.1.2',
     'Flask==2.3.2',
     'Flask-Cors==4.0.0',
     'Flask-RESTful==0.3.10',
     'requests==2.31.0',
     'spacy==3.7.4',
     'tiktoken==0.4.0',
```

### Comparing `suql-1.1.1a0/src/suql/agent.py` & `suql-1.1.2/src/suql/agent.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.1a0/src/suql/faiss_embedding.py` & `suql-1.1.2/src/suql/faiss_embedding.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.1a0/src/suql/free_text_fcns_server.py` & `suql-1.1.2/src/suql/free_text_fcns_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,14 @@
             max_tokens=200,
             temperature=0.0,
             stop_tokens=["\n"],
             postprocess=False,
         )
 
         res = {"result": continuation}
-        print(res)
         return res
 
     @app.route("/summary", methods=["POST"])
     def summary():
         """
         LLM-based summary function, set up as a server for PSQL to call.
         `summary(text)` is a syntactic sugar for `answer(text, 'what is the summary of this document?')`
@@ -118,15 +117,14 @@
         data["text"] : text to summarize upon.
 
         Returns:
         {
             "result" (str): summary function result
         }
         """
-        print(k)
         from suql.prompt_continuation import llm_generate
 
         data = request.get_json()
 
         if "text" not in data:
             return None
 
@@ -150,15 +148,14 @@
             max_tokens=200,
             temperature=0.0,
             stop_tokens=["\n"],
             postprocess=False,
         )
 
         res = {"result": continuation}
-        print(res)
         return res
 
     # start Flask server
     app.run(host=host, port=port)
 
 
 # Functions below are used by the restaurants application only.
```

### Comparing `suql-1.1.1a0/src/suql/postgresql_connection.py` & `suql-1.1.2/src/suql/postgresql_connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,14 @@
 def execute_sql_with_column_info(
     sql_query,
     database="restaurants",
     user="select_user",
     password="select_user",
     unprotected=False,
 ):
-    start_time = time.time()
     # Establish a connection to the PostgreSQL database
     conn = psycopg2.connect(
         database=database,
         user=user,
         password=password,
         host="127.0.0.1",
         port="5432",
@@ -91,15 +90,14 @@
     # Create a cursor object to execute SQL queries
     cursor = conn.cursor()
 
     cursor.execute("SET statement_timeout = 30000")  # Set timeout to 60 seconds
     conn.commit()
 
     try:
-        print("executing SQL {}".format(sql_query))
         # Execute the SQL query
         cursor.execute(sql_query)
 
         # Fetch all the results
         results = cursor.fetchall()
 
         column_names = [desc[0] for desc in cursor.description]
@@ -124,25 +122,12 @@
         if unprotected:
             raise e
         return [], []
 
     # Close the cursor and connection
     cursor.close()
     conn.close()
-    end_time = time.time()
-    elapsed_time = end_time - start_time
-    print(elapsed_time)
     return list(results), column_info
 
 
 if __name__ == "__main__":
-    print(execute_sql("SELECT * FROM restaurants LIMIT 1;"))
-    print(
-        execute_sql(
-            "SELECT reviews FROM restaurants WHERE name ILIKE 'Bistronomie by Baumé' LIMIT 1;"
-        )
-    )
-    print(
-        execute_sql(
-            "SELECT *, summary(reviews) FROM restaurants WHERE 'chef's table' = ANY (popular_dishes) AND location = 'Palo Alto' LIMIT 1;"
-        )
-    )
+    print(execute_sql("SELECT * FROM restaurants LIMIT 1;"))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `suql-1.1.1a0/src/suql/prompt_continuation.py` & `suql-1.1.2/src/suql/prompt_continuation.py`

 * *Files 3% similar despite different names*

```diff
@@ -172,22 +172,18 @@
                 self.traceback_str = traceback.format_exc()
 
     func_thread = FunctionThread(func, *args, **kwargs)
     func_thread.start()
     func_thread.join(timeout_sec)
 
     if func_thread.is_alive():
-        print(f"Function timed out after {timeout_sec} seconds.")
         return False, None
     elif func_thread.exception:
-        print(f"Function raised an exception: {func_thread.exception}")
-        print(func_thread.traceback_str)
         return False, None
     else:
-        print("Function finished successfully.")
         return True, func_thread.return_value
 
 
 def llm_generate(
     template_file: str,
     prompt_parameter_values: dict,
     engine,
```

### Comparing `suql-1.1.1a0/src/suql/prompts/if_db_classification.prompt` & `suql-1.1.2/src/suql/prompts/if_db_classification.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.1a0/src/suql/prompts/opening_hours.prompt` & `suql-1.1.2/src/suql/prompts/opening_hours.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.1a0/src/suql/prompts/parser_suql.prompt` & `suql-1.1.2/src/suql/prompts/parser_suql.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.1a0/src/suql/prompts/yelp_response_SQL.prompt` & `suql-1.1.2/src/suql/prompts/yelp_response_SQL.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.1a0/src/suql/prompts/yelp_response_no_results.prompt` & `suql-1.1.2/src/suql/prompts/yelp_response_no_results.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.1a0/src/suql/sql_free_text_support/execute_free_text_sql.py` & `suql-1.1.2/src/suql/sql_free_text_support/execute_free_text_sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,14 +256,15 @@
                     )
                     execute_sql(
                         f"INSERT INTO {tmp_table_name} VALUES ({placeholder_str})",
                         data=updated_results,
                         user=self.create_username,
                         password=self.create_userpswd,
                         commit_in_lieu_fetch=True,
+                        no_print=True
                     )
 
             # finally, modify the existing sql with tmp_table_name
             node.fromClause = (
                 RangeVar(relname=tmp_table_name, inh=True, relpersistence="p"),
             )
             node.whereClause = None
@@ -305,14 +306,15 @@
         for tmp_table_name in self.tmp_tables:
             drop_stmt = f"DROP TABLE {tmp_table_name}"
             execute_sql(
                 drop_stmt,
                 user=self.create_username,
                 password=self.create_userpswd,
                 commit_in_lieu_fetch=True,
+                no_print=True
             )
 
 
 class _PredicateMapping:
     def __init__(self) -> None:
         self.symbols2predicate = {}
         self.counter = 0
@@ -1668,15 +1670,15 @@
             max_verify
         )
         root = parse_sql(suql)
         visitor(root)
         second_sql = RawStream()(root)
         cache = visitor.serialize_cache()
 
-        return execute_sql(second_sql, user=select_username, password=select_userpswd)
+        return execute_sql(second_sql, user=select_username, password=select_userpswd, no_print=True)
     else:
         try:
             visitor = _SelectVisitor(
                 fts_fields,
                 embedding_server_address,
                 select_username,
                 select_userpswd,
@@ -1688,15 +1690,15 @@
             )
             root = parse_sql(suql)
             visitor(root)
             second_sql = RawStream()(root)
             cache = visitor.serialize_cache()
 
             results, column_names, cache = execute_sql(
-                second_sql, user=select_username, password=select_userpswd
+                second_sql, user=select_username, password=select_userpswd, no_print=True
             )
         except Exception as err:
             with open("_suql_error_log.txt", "a") as file:
                 file.write(f"==============\n")
                 file.write(f"{loggings}\n")
                 file.write(f"{suql}\n")
                 file.write(f"{str(err)}\n")
```

### Comparing `suql-1.1.1a0/src/suql/utils.py` & `suql-1.1.2/src/suql/utils.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.1a0/src/suql.egg-info/PKG-INFO` & `suql-1.1.2/src/suql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.1.1a0
+Version: 1.1.2
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -70,15 +70,15 @@
 
 ## Install from `pip`
 
 Ideal for integrating the SUQL compiler in a larger codebase / system. See [install_pip.md](https://github.com/stanford-oval/suql/blob/main/docs/install_pip.md) for details.
 
 ## Install from source
 
-Ideal for using this repo to build a SUQL-powered conversational interface to your data out-of-the-box, like the one for https://yelpbot.genie.stanford.edu discussed in the paper. See [docs/install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/install_source.md) for details.
+Ideal for using this repo to build a SUQL-powered conversational interface to your data out-of-the-box, like the one for https://yelpbot.genie.stanford.edu discussed in the paper. See [install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/install_source.md) for details.
 
 ## Agent tutorial
 
 Check out [conv_agent.md](https://github.com/stanford-oval/suql/blob/main/docs/conv_agent.md) for more information on best practices for using SUQL to power your conversational agent.
 
 # Bugs / Contribution
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.1.1a0 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.2 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
@@ -35,15 +35,15 @@
 https://arxiv.org/abs/2311.09818. # Installation / Usage tutorial There are two
 main ways of installing the SUQL library. ## Install from `pip` Ideal for
 integrating the SUQL compiler in a larger codebase / system. See
 [install_pip.md](https://github.com/stanford-oval/suql/blob/main/docs/
 install_pip.md) for details. ## Install from source Ideal for using this repo
 to build a SUQL-powered conversational interface to your data out-of-the-box,
 like the one for https://yelpbot.genie.stanford.edu discussed in the paper. See
-[docs/install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/
+[install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/
 install_source.md) for details. ## Agent tutorial Check out [conv_agent.md]
 (https://github.com/stanford-oval/suql/blob/main/docs/conv_agent.md) for more
 information on best practices for using SUQL to power your conversational
 agent. # Bugs / Contribution If you encounter a problem, first check
 [known_issues.md](https://github.com/stanford-oval/suql/blob/main/docs/
 known_issues.md). If it is not listed there, we welcome Issues and/or PRs! #
 Paper results To replicate our results on HybridQA and restaurants in our
```

### Comparing `suql-1.1.1a0/src/suql.egg-info/SOURCES.txt` & `suql-1.1.2/src/suql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

