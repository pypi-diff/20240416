# Comparing `tmp/sql_metadata-2.8.0.tar.gz` & `tmp/sql_metadata-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_metadata-2.8.0.tar", max compression
+gzip compressed data, was "sql_metadata-2.9.0.tar", max compression
```

## Comparing `sql_metadata-2.8.0.tar` & `sql_metadata-2.9.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-04-20 17:44:13.205121 sql_metadata-2.8.0/LICENSE
--rw-r--r--   0        0        0     9003 2023-04-20 17:44:13.205121 sql_metadata-2.8.0/README.md
--rw-r--r--   0        0        0      895 2023-04-20 17:44:13.205121 sql_metadata-2.8.0/pyproject.toml
--rw-r--r--   0        0        0      264 2023-04-20 17:44:13.205121 sql_metadata-2.8.0/sql_metadata/__init__.py
--rw-r--r--   0        0        0     1311 2023-04-20 17:44:13.205121 sql_metadata-2.8.0/sql_metadata/compat.py
--rw-r--r--   0        0        0     2446 2023-04-20 17:44:13.205121 sql_metadata-2.8.0/sql_metadata/generalizator.py
--rw-r--r--   0        0        0     2498 2023-04-20 17:44:13.205121 sql_metadata-2.8.0/sql_metadata/keywords_lists.py
--rw-r--r--   0        0        0    42049 2023-04-20 17:44:13.205121 sql_metadata-2.8.0/sql_metadata/parser.py
--rw-r--r--   0        0        0    19115 2023-04-20 17:44:13.205121 sql_metadata-2.8.0/sql_metadata/token.py
--rw-r--r--   0        0        0      778 2023-04-20 17:44:13.205121 sql_metadata-2.8.0/sql_metadata/utils.py
--rw-r--r--   0        0        0     9749 1970-01-01 00:00:00.000000 sql_metadata-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-09-24 11:32:12.848024 sql_metadata-2.9.0/LICENSE
+-rw-r--r--   0        0        0     9003 2023-09-24 11:32:12.848024 sql_metadata-2.9.0/README.md
+-rw-r--r--   0        0        0      893 2023-09-24 11:32:12.848024 sql_metadata-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0      264 2023-09-24 11:32:12.848024 sql_metadata-2.9.0/sql_metadata/__init__.py
+-rw-r--r--   0        0        0     1311 2023-09-24 11:32:12.848024 sql_metadata-2.9.0/sql_metadata/compat.py
+-rw-r--r--   0        0        0     2446 2023-09-24 11:32:12.848024 sql_metadata-2.9.0/sql_metadata/generalizator.py
+-rw-r--r--   0        0        0     2574 2023-09-24 11:32:12.848024 sql_metadata-2.9.0/sql_metadata/keywords_lists.py
+-rw-r--r--   0        0        0    42396 2023-09-24 11:32:12.848024 sql_metadata-2.9.0/sql_metadata/parser.py
+-rw-r--r--   0        0        0    19115 2023-09-24 11:32:12.848024 sql_metadata-2.9.0/sql_metadata/token.py
+-rw-r--r--   0        0        0      778 2023-09-24 11:32:12.848024 sql_metadata-2.9.0/sql_metadata/utils.py
+-rw-r--r--   0        0        0     9745 1970-01-01 00:00:00.000000 sql_metadata-2.9.0/PKG-INFO
```

### Comparing `sql_metadata-2.8.0/LICENSE` & `sql_metadata-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sql_metadata-2.8.0/README.md` & `sql_metadata-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `sql_metadata-2.8.0/pyproject.toml` & `sql_metadata-2.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "sql_metadata"
-version = "2.8.0"
+version = "2.9.0"
 license="MIT"
 description = "Uses tokenized query returned by python-sqlparse and generates query metadata"
 authors = ["Maciej Brencz <maciej.brencz@gmail.com>", "Radosław Drążkiewicz <collerek@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/macbre/sql-metadata"
 repository = "https://github.com/macbre/sql-metadata"
 
 packages = [
     { include="sql_metadata" }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7.2"
+python = "^3.8"
 sqlparse = "^0.4.1"
 
 [tool.poetry.dev-dependencies]
-black = "^23.3"
+black = "^23.9"
 coverage = {extras = ["toml"], version = "^6.5"}
-pylint = "^2.17.2"
-pytest = "^7.3.1"
-pytest-cov = "^4.0.0"
+pylint = "^2.17.5"
+pytest = "^7.4.2"
+pytest-cov = "^4.1.0"
 coveralls = "^3.3.1"
 flake8 = "^5.0.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sql_metadata-2.8.0/sql_metadata/compat.py` & `sql_metadata-2.9.0/sql_metadata/compat.py`

 * *Files identical despite different names*

### Comparing `sql_metadata-2.8.0/sql_metadata/generalizator.py` & `sql_metadata-2.9.0/sql_metadata/generalizator.py`

 * *Files identical despite different names*

### Comparing `sql_metadata-2.8.0/sql_metadata/keywords_lists.py` & `sql_metadata-2.9.0/sql_metadata/keywords_lists.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 # these keywords are followed by columns reference
 from enum import Enum
 
 KEYWORDS_BEFORE_COLUMNS = {
     "SELECT",
     "WHERE",
+    "HAVING",
     "ORDERBY",
     "GROUPBY",
     "ON",
     "SET",
     "USING",
 }
 
@@ -24,14 +25,15 @@
     "INNERJOIN",
     "FULLJOIN",
     "FULLOUTERJOIN",
     "LEFTJOIN",
     "RIGHTJOIN",
     "LEFTOUTERJOIN",
     "RIGHTOUTERJOIN",
+    "NATURALJOIN",
     "INTO",
     "UPDATE",
     "TABLE",
 }
 
 # next statement beginning after with statement
 WITH_ENDING_KEYWORDS = {"UPDATE", "SELECT", "DELETE", "REPLACE", "INSERT"}
@@ -44,21 +46,23 @@
     "INNERJOIN",
     "FULLJOIN",
     "FULLOUTERJOIN",
     "LEFTJOIN",
     "RIGHTJOIN",
     "LEFTOUTERJOIN",
     "RIGHTOUTERJOIN",
+    "NATURALJOIN",
 }
 
 # section of a query in which column can exists
 # based on last normalized keyword
 COLUMNS_SECTIONS = {
     "SELECT": "select",
     "WHERE": "where",
+    "HAVING": "having",
     "ORDERBY": "order_by",
     "ON": "join",
     "USING": "join",
     "INTO": "insert",
     "SET": "update",
     "GROUPBY": "group_by",
 }
```

### Comparing `sql_metadata-2.8.0/sql_metadata/parser.py` & `sql_metadata-2.9.0/sql_metadata/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         self._values = None
         self._values_dict = None
 
         self._subquery_level = 0
         self._nested_level = 0
         self._parenthesis_level = 0
         self._open_parentheses: List[SQLToken] = []
+        self._preceded_keywords: List[SQLToken] = []
         self._aliases_to_check = None
         self._is_in_nested_function = False
         self._is_in_with_block = False
         self._with_columns_candidates = {}
         self._column_aliases_max_subquery_level = {}
 
         self.sqlparse_tokens = None
@@ -120,15 +121,15 @@
         self._query_type = SUPPORTED_QUERY_TYPES.get(switch, "UNSUPPORTED")
         if self._query_type == "UNSUPPORTED":
             self._logger.error("Not supported query type: %s", self._raw_query)
             raise ValueError("Not supported query type!")
         return self._query_type
 
     @property
-    def tokens(self) -> List[SQLToken]:
+    def tokens(self) -> List[SQLToken]:  # noqa: C901
         """
         Tokenizes the query
         """
         if self._tokens is not None:
             return self._tokens
 
         parsed = sqlparse.parse(self._query)
@@ -160,14 +161,16 @@
 
             if token.is_left_parenthesis:
                 token.token_type = TokenType.PARENTHESIS
                 self._determine_opening_parenthesis_type(token=token)
             elif token.is_right_parenthesis:
                 token.token_type = TokenType.PARENTHESIS
                 self._determine_closing_parenthesis_type(token=token)
+                if token.is_subquery_end:
+                    last_keyword = self._preceded_keywords.pop()
 
             last_keyword = self._determine_last_relevant_keyword(
                 token=token, last_keyword=last_keyword
             )
             token.is_in_nested_function = self._is_in_nested_function
             token.parenthesis_level = self._parenthesis_level
             tokens.append(token)
@@ -852,14 +855,15 @@
         """
         Determines the type of left parenthesis in query
         """
         if token.previous_token.normalized in SUBQUERY_PRECEDING_KEYWORDS:
             # inside subquery / derived table
             token.is_subquery_start = True
             self._subquery_level += 1
+            self._preceded_keywords.append(token.last_keyword_normalized)
             token.subquery_level = self._subquery_level
         elif token.previous_token.normalized in KEYWORDS_BEFORE_COLUMNS.union({","}):
             # we are in columns and in a column subquery definition
             token.is_column_definition_start = True
         elif (
             token.previous_token.is_as_keyword
             and token.last_keyword_normalized != "WINDOW"
@@ -966,14 +970,16 @@
         query = re.sub(r'"([^`]+?)"', r"`\1`", query)
         query = re.sub(r'"([^`]+?)"\."([^`]+?)"', r"`\1`.`\2`", query)
         query = re.sub(r"'.*?'", replace_back_quotes_in_string, query)
 
         return query
 
     def _determine_last_relevant_keyword(self, token: SQLToken, last_keyword: str):
+        if token.value == "," and token.last_keyword_normalized == "ON":
+            return "FROM"
         if token.is_keyword and "".join(token.normalized.split()) in RELEVANT_KEYWORDS:
             if (
                 not (
                     token.normalized == "FROM"
                     and token.get_nth_previous(3).normalized == "EXTRACT"
                 )
                 and not (
```

### Comparing `sql_metadata-2.8.0/sql_metadata/token.py` & `sql_metadata-2.9.0/sql_metadata/token.py`

 * *Files identical despite different names*

### Comparing `sql_metadata-2.8.0/sql_metadata/utils.py` & `sql_metadata-2.9.0/sql_metadata/utils.py`

 * *Files identical despite different names*

### Comparing `sql_metadata-2.8.0/PKG-INFO` & `sql_metadata-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: sql-metadata
-Version: 2.8.0
+Name: sql_metadata
+Version: 2.9.0
 Summary: Uses tokenized query returned by python-sqlparse and generates query metadata
 Home-page: https://github.com/macbre/sql-metadata
 License: MIT
 Author: Maciej Brencz
 Author-email: maciej.brencz@gmail.com
-Requires-Python: >=3.7.2,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: sqlparse (>=0.4.1,<0.5.0)
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: sql-metadata Version: 2.8.0 Summary: Uses tokenized
+Metadata-Version: 2.1 Name: sql_metadata Version: 2.9.0 Summary: Uses tokenized
 query returned by python-sqlparse and generates query metadata Home-page:
 https://github.com/macbre/sql-metadata License: MIT Author: Maciej Brencz
-Author-email: maciej.brencz@gmail.com Requires-Python: >=3.7.2,<4.0.0
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: sqlparse (>=0.4.1,<0.5.0) Project-URL: Repository, https://
-github.com/macbre/sql-metadata Description-Content-Type: text/markdown # sql-
-metadata [![PyPI](https://img.shields.io/pypi/v/sql_metadata.svg)](https://
+Author-email: maciej.brencz@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Dist: sqlparse (>=0.4.1,<0.5.0) Project-URL: Repository, https://github.com/
+macbre/sql-metadata Description-Content-Type: text/markdown # sql-metadata [!
+[PyPI](https://img.shields.io/pypi/v/sql_metadata.svg)](https://
 pypi.python.org/pypi/sql_metadata) [![Tests](https://github.com/macbre/sql-
 metadata/actions/workflows/python-ci.yml/badge.svg)](https://github.com/macbre/
 sql-metadata/actions/workflows/python-ci.yml) [![Coverage Status](https://
 coveralls.io/repos/github/macbre/sql-metadata/badge.svg?branch=master&1)]
 (https://coveralls.io/github/macbre/sql-metadata?branch=master) _[_C_o_d_e_ _s_t_y_l_e_:
 _b_l_a_c_k_][![Maintenance](https://img.shields.io/badge/maintained%3F-yes-
 green.svg)](https://github.com/macbre/sql-metadata/graphs/commit-activity) [!
```

