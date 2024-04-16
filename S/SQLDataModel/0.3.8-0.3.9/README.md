# Comparing `tmp/SQLDataModel-0.3.8.tar.gz` & `tmp/sqldatamodel-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLDataModel-0.3.8.tar", last modified: Sat Apr 13 00:44:59 2024, max compression
+gzip compressed data, was "sqldatamodel-0.3.9.tar", last modified: Sat Apr 13 23:09:09 2024, max compression
```

## Comparing `SQLDataModel-0.3.8.tar` & `sqldatamodel-0.3.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 00:44:59.879810 SQLDataModel-0.3.8/
--rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 SQLDataModel-0.3.8/LICENSE
--rw-rw-rw-   0        0        0    27267 2024-04-13 00:44:59.875540 SQLDataModel-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0    25395 2024-04-12 01:46:49.000000 SQLDataModel-0.3.8/README.md
--rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 SQLDataModel-0.3.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-13 00:44:59.880344 SQLDataModel-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     2400 2024-04-13 00:43:24.000000 SQLDataModel-0.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-13 00:44:58.584088 SQLDataModel-0.3.8/src/
-drwxrwxrwx   0        0        0        0 2024-04-13 00:44:59.719915 SQLDataModel-0.3.8/src/SQLDataModel/
--rw-rw-rw-   0        0        0     6899 2024-03-19 22:34:49.000000 SQLDataModel-0.3.8/src/SQLDataModel/ANSIColor.py
--rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 SQLDataModel-0.3.8/src/SQLDataModel/HTMLParser.py
--rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 SQLDataModel-0.3.8/src/SQLDataModel/JSONEncoder.py
--rw-rw-rw-   0        0        0   586081 2024-04-13 00:44:13.000000 SQLDataModel-0.3.8/src/SQLDataModel/SQLDataModel.py
--rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 SQLDataModel-0.3.8/src/SQLDataModel/StandardDeviation.py
--rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 SQLDataModel-0.3.8/src/SQLDataModel/__init__.py
--rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 SQLDataModel-0.3.8/src/SQLDataModel/converters.py
--rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 SQLDataModel-0.3.8/src/SQLDataModel/demo.py
--rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 SQLDataModel-0.3.8/src/SQLDataModel/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-13 00:44:59.831965 SQLDataModel-0.3.8/src/SQLDataModel/extensions/
--rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 SQLDataModel-0.3.8/src/SQLDataModel/extensions/__init__.py
--rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 SQLDataModel-0.3.8/src/SQLDataModel/extensions/str_utils.c
-drwxrwxrwx   0        0        0        0 2024-04-13 00:44:59.871228 SQLDataModel-0.3.8/src/SQLDataModel.egg-info/
--rw-rw-rw-   0        0        0    27267 2024-04-13 00:44:58.000000 SQLDataModel-0.3.8/src/SQLDataModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2024-04-13 00:44:58.000000 SQLDataModel-0.3.8/src/SQLDataModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 00:44:58.000000 SQLDataModel-0.3.8/src/SQLDataModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-13 00:44:58.000000 SQLDataModel-0.3.8/src/SQLDataModel.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-13 00:44:59.841962 SQLDataModel-0.3.8/tests/
--rw-rw-rw-   0        0        0    58321 2024-04-13 00:42:51.000000 SQLDataModel-0.3.8/tests/test_Future.py
--rw-rw-rw-   0        0        0    58324 2024-04-13 00:42:52.000000 SQLDataModel-0.3.8/tests/test_SQLDataModel.py
+drwxrwxrwx   0        0        0        0 2024-04-13 23:09:09.971355 sqldatamodel-0.3.9/
+-rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 sqldatamodel-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0    27267 2024-04-13 23:09:09.961354 sqldatamodel-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0    25395 2024-04-12 01:46:49.000000 sqldatamodel-0.3.9/README.md
+-rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 sqldatamodel-0.3.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-13 23:09:09.973357 sqldatamodel-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     2400 2024-04-13 23:07:32.000000 sqldatamodel-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 23:09:08.454230 sqldatamodel-0.3.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-13 23:09:09.643783 sqldatamodel-0.3.9/src/SQLDataModel/
+-rw-rw-rw-   0        0        0     6899 2024-03-19 22:34:49.000000 sqldatamodel-0.3.9/src/SQLDataModel/ANSIColor.py
+-rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 sqldatamodel-0.3.9/src/SQLDataModel/HTMLParser.py
+-rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 sqldatamodel-0.3.9/src/SQLDataModel/JSONEncoder.py
+-rw-rw-rw-   0        0        0   589857 2024-04-13 23:07:34.000000 sqldatamodel-0.3.9/src/SQLDataModel/SQLDataModel.py
+-rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 sqldatamodel-0.3.9/src/SQLDataModel/StandardDeviation.py
+-rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 sqldatamodel-0.3.9/src/SQLDataModel/__init__.py
+-rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 sqldatamodel-0.3.9/src/SQLDataModel/converters.py
+-rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 sqldatamodel-0.3.9/src/SQLDataModel/demo.py
+-rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 sqldatamodel-0.3.9/src/SQLDataModel/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-13 23:09:09.862411 sqldatamodel-0.3.9/src/SQLDataModel/extensions/
+-rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 sqldatamodel-0.3.9/src/SQLDataModel/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 sqldatamodel-0.3.9/src/SQLDataModel/extensions/str_utils.c
+drwxrwxrwx   0        0        0        0 2024-04-13 23:09:09.953354 sqldatamodel-0.3.9/src/SQLDataModel.egg-info/
+-rw-rw-rw-   0        0        0    27267 2024-04-13 23:09:08.000000 sqldatamodel-0.3.9/src/SQLDataModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2024-04-13 23:09:08.000000 sqldatamodel-0.3.9/src/SQLDataModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 23:09:08.000000 sqldatamodel-0.3.9/src/SQLDataModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-13 23:09:08.000000 sqldatamodel-0.3.9/src/SQLDataModel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 23:09:09.880410 sqldatamodel-0.3.9/tests/
+-rw-rw-rw-   0        0        0    59486 2024-04-13 23:06:52.000000 sqldatamodel-0.3.9/tests/test_Future.py
+-rw-rw-rw-   0        0        0    59489 2024-04-13 23:06:53.000000 sqldatamodel-0.3.9/tests/test_SQLDataModel.py
```

### Comparing `SQLDataModel-0.3.8/LICENSE` & `sqldatamodel-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.8/PKG-INFO` & `sqldatamodel-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.3.8
+Version: 0.3.9
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package
```

### Comparing `SQLDataModel-0.3.8/README.md` & `sqldatamodel-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.8/setup.py` & `sqldatamodel-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='SQLDataModel',  
-     version='0.3.8',
+     version='0.3.9',
      scripts=['src/SQLDataModel/SQLDataModel.py'] ,
      author='Ante Tonkovic-Capin',
      author_email='antetc@icloud.com',
      description='SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.',
      keywords=['SQL','ETL','dataframe','terminal tables','pretty print tables','sql2sql','data analysis','data science','data model','extract','transform','load','web scraping tables','data mining','html','html table parsing','apache arrow','pyarrow','pyarrow conversion','pyarrow to table','pyarrow to sql','pyarrow to csv','parquet file parsing','csv','csv parsing','markdown','markdown table parsing','latex','latex table parsing','delimited','delimited data parsing','file conversion','format conversion','terminal styling','table styling','from sqlite','to sqlite','from postgresql','to postgresql','sql to sql','excel','xlsx file','excel to sql','DataFrame package'],
      license_file='LICENSE',
      long_description=long_description,
```

### Comparing `SQLDataModel-0.3.8/src/SQLDataModel/ANSIColor.py` & `sqldatamodel-0.3.9/src/SQLDataModel/ANSIColor.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.8/src/SQLDataModel/HTMLParser.py` & `sqldatamodel-0.3.9/src/SQLDataModel/HTMLParser.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.8/src/SQLDataModel/JSONEncoder.py` & `sqldatamodel-0.3.9/src/SQLDataModel/JSONEncoder.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.8/src/SQLDataModel/SQLDataModel.py` & `sqldatamodel-0.3.9/src/SQLDataModel/SQLDataModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,23 +332,54 @@
                             SQLDataModel.ErrorFormat(f"TypeError: invalid type '{type(dtypes).__name__}', ``dtypes`` must be of type 'dict' with format of `{{'column':'dtype'}}` where 'dtype' must be a string representing a valid python datatype")
                         )
                     headers = list(dtypes.keys())
             had_data = False
             data = [tuple(None for _ in range(len(headers)))]
         else:
             had_data = True
-        if not isinstance(data, (list,tuple)) and had_data:
+        if not isinstance(data, (list,tuple,dict)) and had_data:  
             raise TypeError(
-                SQLDataModel.ErrorFormat(f"TypeError: type mismatch, '{type(data).__name__}' is not a valid type for data, which must be of type list or tuple")
+                SQLDataModel.ErrorFormat(f"TypeError: type mismatch, '{type(data).__name__}' is not a valid type for data, which must be of type list, tuple or dict")
                 )
         if len(data) < 1 and had_data:
             raise ValueError(
                 SQLDataModel.ErrorFormat(f"ValueError: data not found, data of length '{len(data)}' is insufficient to construct a valid model, additional rows of data required")
                 )
         if had_data:
+            if isinstance(data, dict) or isinstance(data[0], dict):
+                if isinstance(data, list):
+                    data = SQLDataModel.flatten_json(data)
+                rowwise = True if all(isinstance(x, int) for x in data.keys()) else False
+                if rowwise:
+                    col_count = len(data[next(iter(data))])
+                    if headers is None:
+                        headers = ['idx',*[f'{i}' for i in range(col_count)]] # get column count from first key value pair in provided dict
+                    elif (col_count) == len(headers):
+                        headers = ['idx',*headers]
+                    data = [tuple([k,*v]) for k,v in data.items()]
+                else:
+                    first_key_val = data[next(iter(data))]
+                    if isinstance(first_key_val, dict):
+                        inferred_headers = list(data.keys())
+                        data = [[data[col][val] for col in inferred_headers] for val in data.keys()]
+                    elif isinstance(first_key_val, (list,tuple)):
+                        inferred_headers = [k for k in data.keys()]
+                        column_count = len(inferred_headers)
+                        row_count = len(first_key_val)
+                        data = [x for x in data.values()]
+                        data = [tuple([data[j][row] for j in range(column_count)]) for row in range(row_count)]
+                        if headers is None:
+                            headers = inferred_headers
+                        else:
+                            if len(headers) + 1 == column_count:
+                                headers = ['idx',*headers]
+                    else:
+                        raise TypeError(
+                            SQLDataModel.ErrorFormat(f"TypeError: invalid dict values, received type '{type(first_key_val).__name__}' but expected dict values as one of type 'list', 'tuple' or 'dict'")
+                        )
             try:
                 _ = data[0]
             except Exception as e:
                 raise IndexError(
                     SQLDataModel.ErrorFormat(f"IndexError: data index error, data index provided does not exist for length '{len(data)}' due to '{e}'")
                     ) from None
             if not isinstance(data[0], (list,tuple)):
@@ -2587,58 +2618,99 @@
             ``SQLDataModel``: The SQLDataModel object created from the provided dictionary.
 
         Raises:
             ``TypeError``: If the provided dictionary values are not of type 'list', 'tuple', or 'dict'.
             ``ValueError``: If the provided data appears to be a list of dicts but is empty.
 
         Example::
-            
-            from SQLDataModel import SQLDataModel
 
-            # Sample data
-            data_dict = {1: [10, 'A'], 2: [20, 'B'], 3: [30, 'C']}
+            from SQLDataModel import SQLDataModel
+            
+            # Sample data with column orientation
+            data = {
+                'Name': ['Beth', 'John', 'Alice', 'Travis'], 
+                'Height': [172.4, 175.3, 162.0, 185.8],
+                'Age': [27, 30, 28, 35]
+            }
 
             # Create the model
-            sdm_obj = SQLDataModel.from_dict(data_dict)
+            sdm = SQLDataModel.from_dict(data)
 
-            # View output
-            print(sdm_obj)
+            # View it
+            print(sdm)
         
         This will output:
+
+        ```shell
+            ┌────────┬─────────┬─────┐
+            │ Name   │  Height │ Age │
+            ├────────┼─────────┼─────┤
+            │ Beth   │  172.40 │  27 │
+            │ John   │  175.30 │  30 │
+            │ Alice  │  162.00 │  28 │
+            │ Travis │  185.80 │  35 │
+            └────────┴─────────┴─────┘
+            [4 rows x 3 columns]
+        ```
+
+        We can also create a model using a dictionary with row orientation:
+        
+        ```python
+            from SQLDataModel import SQLDataModel
+
+            # Sample data with row orientation
+            data = {
+                 0: ['Mercury', 0.38]
+                ,1: ['Venus', 0.91]
+                ,2: ['Earth', 1.00]
+                ,3: ['Mars', 0.38]
+            }
+
+            # Create the model with custom headers
+            sdm = SQLDataModel.from_dict(data, headers=['Planet', 'Gravity'])
+
+            # View output
+            print(sdm)
+        ```
+
+        This will output the model created using row-wise dictionary data:
         
         ```shell            
-            ┌───┬───────┬───────┐
-            │   │ col_0 │ col_1 │
-            ├───┼───────┼───────┤
-            │ 1 │    10 │ A     │
-            │ 2 │    20 │ B     │
-            │ 3 │    30 │ C     │
-            └───┴───────┴───────┘
-            [3 rows x 2 columns]
+            ┌─────────┬─────────┐
+            │ Planet  │ Gravity │
+            ├─────────┼─────────┤
+            │ Mercury │    0.38 │
+            │ Venus   │    0.91 │
+            │ Earth   │    1.00 │
+            │ Mars    │    0.38 │
+            └─────────┴─────────┘
+            [4 rows x 2 columns]
         ```
 
         Note:
+            - Dictionaries in list like orientation can also be used with structures similar to JSON objects.
             - The method determines the structure of the SQLDataModel based on the format of the provided dictionary.
             - If the keys are integers, they are used as row indexes; otherwise, keys are used as headers.
-            
+            - See :meth:`SQLDataModel.to_dict()` for converting existing instances of ``SQLDataModel`` to dictionaries.
         """
         if isinstance(data, list):
             if len(data) < 1:
                 raise ValueError(
-                    SQLDataModel.ErrorFormat(f"ValueError: insufficient data length '{len(data)}', if ``data`` is of type 'list' at least 1 row is required for `from_dict()` method")
+                    SQLDataModel.ErrorFormat(f"ValueError: insufficient data length '{len(data)}', if `data` is of type 'list' at least 1 row is required for `from_dict()` method")
                 )
             if not isinstance(data[0], dict):
                 raise TypeError(
-                    SQLDataModel.ErrorFormat(f"TypeError: invalid type in list '{type(data[0].__name__)}', if ``data`` is of type 'list' its items must be of type 'dict' to use the `from_dict()` method")
+                    SQLDataModel.ErrorFormat(f"TypeError: invalid type in list '{type(data[0].__name__)}', if `data` is of type 'list' its items must be of type 'dict' to use the `from_dict()` method")
                 )
             return cls.from_json(data)
         rowwise = True if all(isinstance(x, int) for x in data.keys()) else False
         if rowwise:
-            headers = ['idx',*[f'{i}' for i in range(len(data[next(iter(data))]))]] # get column count from first key value pair in provided dict
-            return cls([tuple([k,*v]) for k,v in data.items()], headers, **kwargs)
+            if 'headers' not in kwargs:
+                kwargs['headers'] = ['idx',*[f'{i}' for i in range(len(data[next(iter(data))]))]] # get column count from first key value pair in provided dict
+            return cls([tuple([k,*v]) for k,v in data.items()], **kwargs)
         else:
             first_key_val = data[next(iter(data))]
             if isinstance(first_key_val, dict):
                 headers = list(data.keys())
                 data = [[data[col][val] for col in headers] for val in data.keys()]
             elif isinstance(first_key_val, (list,tuple)):
                 headers = [k for k in data.keys()]
@@ -2646,15 +2718,17 @@
                 row_count = len(first_key_val)
                 data = [x for x in data.values()]
                 data = [tuple([data[j][row] for j in range(column_count)]) for row in range(row_count)]
             else:
                 raise TypeError(
                     SQLDataModel.ErrorFormat(f"TypeError: invalid dict values, received type '{type(first_key_val).__name__}' but expected dict values as one of type 'list', 'tuple' or 'dict'")
                 )
-            return cls(data, headers, **kwargs)  
+            if 'headers' not in kwargs:
+                kwargs['headers'] = headers
+            return cls(data=data, **kwargs)  
 
     @classmethod
     def from_excel(cls, filename:str, worksheet:int|str=0, min_row:int|None=None, max_row:int|None=None, min_col:int|None=None, max_col:int|None=None, headers:list[str]=None, **kwargs) -> SQLDataModel:
         """
         Returns a new ``SQLDataModel`` instance from the specified Excel file.
 
         Parameters:
@@ -3832,15 +3906,14 @@
                 )
         if (obj_type := type(df).__name__) != 'DataFrame':
             raise TypeError(
                 SQLDataModel.ErrorFormat(f"TypeError: invalid type '{obj_type}', argument for `df` must be of type 'DataFrame'")
             )        
         return cls(data=df.rows(), headers=df.columns if headers is None else headers, **kwargs)
 
-
     @classmethod
     def from_pyarrow(cls, table, **kwargs) -> SQLDataModel:
         """
         Returns a new ``SQLDataModel`` instance from the provided Apache Arrow object.
 
         Parameters:
             ``table`` (pyarrow.lib.Table): Apache Arrow object from which to construct a new ``SQLDataModel`` object.
```

### Comparing `SQLDataModel-0.3.8/src/SQLDataModel/StandardDeviation.py` & `sqldatamodel-0.3.9/src/SQLDataModel/StandardDeviation.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.8/src/SQLDataModel/converters.py` & `sqldatamodel-0.3.9/src/SQLDataModel/converters.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.8/src/SQLDataModel/demo.py` & `sqldatamodel-0.3.9/src/SQLDataModel/demo.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.8/src/SQLDataModel/exceptions.py` & `sqldatamodel-0.3.9/src/SQLDataModel/exceptions.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.8/src/SQLDataModel/extensions/str_utils.c` & `sqldatamodel-0.3.9/src/SQLDataModel/extensions/str_utils.c`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.8/src/SQLDataModel.egg-info/PKG-INFO` & `sqldatamodel-0.3.9/src/SQLDataModel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.3.8
+Version: 0.3.9
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package
```

### Comparing `SQLDataModel-0.3.8/src/SQLDataModel.egg-info/SOURCES.txt` & `sqldatamodel-0.3.9/src/SQLDataModel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.8/tests/test_Future.py` & `sqldatamodel-0.3.9/tests/test_SQLDataModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime, os, tempfile, csv, sqlite3, random
 import pytest
 import pandas as pd
 import polars as pl
 import numpy as np
 from .random_data_generator import data_generator
-from future.SQLDataModel_future import SQLDataModel
+from src.SQLDataModel.SQLDataModel import SQLDataModel
 
 @pytest.fixture
 def sample_data() -> tuple[list[list], list[str]]:
     """Returns sample data in format `(data, headers)` to use for testing."""
     return data_generator(num_rows=120, float_precision=4, num_columns=8, seed=42, return_header_type='list', return_row_type='tuple', return_format='combined')
 
 @pytest.fixture
@@ -23,14 +23,36 @@
     input_data, input_headers = sample_data[1:], sample_data[0]
     input_rows, input_cols = len(input_data), len(input_data[0])
     sdm = SQLDataModel(data=input_data, headers=input_headers)
     assert sdm.row_count == input_rows and sdm.column_count == input_cols
     assert sdm.headers == input_headers
 
 @pytest.mark.core
+def test_init_dict(sample_data):
+    input_data, input_headers = sample_data[1:], sample_data[0]
+    ### dict with rows orientation ###
+    input_rows_dict = {i:list(row) for i, row in enumerate(input_data)}
+    sdm = SQLDataModel(data=input_rows_dict, headers=input_headers)
+    output_data, output_headers = sdm.data(), sdm.headers
+    assert output_headers == input_headers
+    assert output_data == input_data
+    ### dict with columns orientation ###
+    input_cols_dict = {f'{col}': [row[idx] for row in input_data] for idx,col in enumerate(input_headers)}
+    sdm = SQLDataModel(data=input_cols_dict, headers=input_headers)
+    output_data, output_headers = sdm.data(), sdm.headers
+    assert output_headers == input_headers
+    assert output_data == input_data    
+    ### json like list of dicts ###
+    input_list_dict = [{col:row[i] for i,col in enumerate(input_headers)} for row in input_data]    
+    sdm = SQLDataModel(data=input_list_dict, headers=input_headers)
+    output_data, output_headers = sdm.data(), sdm.headers
+    assert output_headers == input_headers
+    assert output_data == input_data        
+
+@pytest.mark.core
 def test_data(sample_data):
     input_data, input_headers = sample_data[1:], sample_data[0]
     sdm = SQLDataModel(data=input_data, headers=input_headers)
     out_data = sdm.data()
     assert all([input_data[i][j] == out_data[i][j] for j in range(len(input_data[0])) for i in range(len(input_data))])
 
 @pytest.mark.core
```

### Comparing `SQLDataModel-0.3.8/tests/test_SQLDataModel.py` & `sqldatamodel-0.3.9/tests/test_Future.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime, os, tempfile, csv, sqlite3, random
 import pytest
 import pandas as pd
 import polars as pl
 import numpy as np
 from .random_data_generator import data_generator
-from src.SQLDataModel.SQLDataModel import SQLDataModel
+from future.SQLDataModel_future import SQLDataModel
 
 @pytest.fixture
 def sample_data() -> tuple[list[list], list[str]]:
     """Returns sample data in format `(data, headers)` to use for testing."""
     return data_generator(num_rows=120, float_precision=4, num_columns=8, seed=42, return_header_type='list', return_row_type='tuple', return_format='combined')
 
 @pytest.fixture
@@ -23,14 +23,36 @@
     input_data, input_headers = sample_data[1:], sample_data[0]
     input_rows, input_cols = len(input_data), len(input_data[0])
     sdm = SQLDataModel(data=input_data, headers=input_headers)
     assert sdm.row_count == input_rows and sdm.column_count == input_cols
     assert sdm.headers == input_headers
 
 @pytest.mark.core
+def test_init_dict(sample_data):
+    input_data, input_headers = sample_data[1:], sample_data[0]
+    ### dict with rows orientation ###
+    input_rows_dict = {i:list(row) for i, row in enumerate(input_data)}
+    sdm = SQLDataModel(data=input_rows_dict, headers=input_headers)
+    output_data, output_headers = sdm.data(), sdm.headers
+    assert output_headers == input_headers
+    assert output_data == input_data
+    ### dict with columns orientation ###
+    input_cols_dict = {f'{col}': [row[idx] for row in input_data] for idx,col in enumerate(input_headers)}
+    sdm = SQLDataModel(data=input_cols_dict, headers=input_headers)
+    output_data, output_headers = sdm.data(), sdm.headers
+    assert output_headers == input_headers
+    assert output_data == input_data    
+    ### json like list of dicts ###
+    input_list_dict = [{col:row[i] for i,col in enumerate(input_headers)} for row in input_data]    
+    sdm = SQLDataModel(data=input_list_dict, headers=input_headers)
+    output_data, output_headers = sdm.data(), sdm.headers
+    assert output_headers == input_headers
+    assert output_data == input_data        
+
+@pytest.mark.core
 def test_data(sample_data):
     input_data, input_headers = sample_data[1:], sample_data[0]
     sdm = SQLDataModel(data=input_data, headers=input_headers)
     out_data = sdm.data()
     assert all([input_data[i][j] == out_data[i][j] for j in range(len(input_data[0])) for i in range(len(input_data))])
 
 @pytest.mark.core
```

