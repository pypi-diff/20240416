# Comparing `tmp/tej-tool-api-1.1.1rc4.tar.gz` & `tmp/tej_tool_api-1.1.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tej-tool-api-1.1.1rc4.tar", last modified: Mon Feb 26 07:20:07 2024, max compression
+gzip compressed data, was "tej_tool_api-1.1.2rc0.tar", last modified: Tue Apr 16 09:41:55 2024, max compression
```

## Comparing `tej-tool-api-1.1.1rc4.tar` & `tej_tool_api-1.1.2rc0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 07:20:07.855640 tej-tool-api-1.1.1rc4/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-26 07:19:56.000000 tej-tool-api-1.1.1rc4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-02-26 07:20:07.855640 tej-tool-api-1.1.1rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-02-26 07:19:56.000000 tej-tool-api-1.1.1rc4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 07:20:07.855640 tej-tool-api-1.1.1rc4/TejToolAPI/
--rw-r--r--   0 runner    (1001) docker     (127)    29371 2024-02-26 07:19:56.000000 tej-tool-api-1.1.1rc4/TejToolAPI/Map_Dask_API.py
--rw-r--r--   0 runner    (1001) docker     (127)    13543 2024-02-26 07:19:56.000000 tej-tool-api-1.1.1rc4/TejToolAPI/TejToolAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-02-26 07:19:56.000000 tej-tool-api-1.1.1rc4/TejToolAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-26 07:20:07.000000 tej-tool-api-1.1.1rc4/TejToolAPI/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-02-26 07:19:56.000000 tej-tool-api-1.1.1rc4/TejToolAPI/exchange_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-02-26 07:19:56.000000 tej-tool-api-1.1.1rc4/TejToolAPI/meta_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-02-26 07:19:56.000000 tej-tool-api-1.1.1rc4/TejToolAPI/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 07:20:07.855640 tej-tool-api-1.1.1rc4/TejToolAPI/tables/
--rw-r--r--   0 runner    (1001) docker     (127)    24887 2024-02-26 07:19:56.000000 tej-tool-api-1.1.1rc4/TejToolAPI/tables/all_meta.json
--rw-r--r--   0 runner    (1001) docker     (127)    62159 2024-02-26 07:19:56.000000 tej-tool-api-1.1.1rc4/TejToolAPI/tables/columns_group.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-26 07:19:56.000000 tej-tool-api-1.1.1rc4/TejToolAPI/tables/~$columns_group.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-26 07:19:56.000000 tej-tool-api-1.1.1rc4/TejToolAPI/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-02-26 07:19:56.000000 tej-tool-api-1.1.1rc4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 07:20:07.855640 tej-tool-api-1.1.1rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-02-26 07:19:56.000000 tej-tool-api-1.1.1rc4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 07:20:07.855640 tej-tool-api-1.1.1rc4/tej_tool_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-26 07:20:07.000000 tej-tool-api-1.1.1rc4/tej_tool_api.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:41:55.945784 tej_tool_api-1.1.2rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-16 09:41:55.945784 tej_tool_api-1.1.2rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:41:55.945784 tej_tool_api-1.1.2rc0/TejToolAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)    29372 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/TejToolAPI/Map_Dask_API.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13543 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/TejToolAPI/TejToolAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/TejToolAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-16 09:41:55.000000 tej_tool_api-1.1.2rc0/TejToolAPI/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/TejToolAPI/exchange_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/TejToolAPI/meta_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/TejToolAPI/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:41:55.945784 tej_tool_api-1.1.2rc0/TejToolAPI/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)    24887 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/TejToolAPI/tables/all_meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)    62159 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/TejToolAPI/tables/columns_group.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/TejToolAPI/tables/~$columns_group.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/TejToolAPI/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 09:41:55.945784 tej_tool_api-1.1.2rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:41:55.945784 tej_tool_api-1.1.2rc0/tej_tool_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-16 09:41:55.000000 tej_tool_api-1.1.2rc0/tej_tool_api.egg-info/SOURCES.txt
```

### Comparing `tej-tool-api-1.1.1rc4/PKG-INFO` & `tej_tool_api-1.1.2rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: tej-tool-api
-Version: 1.1.1rc4
+Version: 1.1.2rc0
 Summary: Package to fetch a large quantity of data from tejapi.
 Author: tej
 Author-email: tej@tej.com.tw
 Maintainer: tej api Development Team
 Maintainer-email: tej@tej.com.tw
+License: Apache-2.0
 Project-URL: homepage, https://api.tej.com.tw
 Project-URL: repository, https://github.com/tejtw/TEJ_TOOL_API
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Chinese (Traditional)
 Classifier: Programming Language :: Python
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ## 使用 Tool API 獲取數據(股價、財務、月營收、集保和股票屬性)
 ### 安裝套件
 ```python
 pip install tej-tool-api
 ```
```

### Comparing `tej-tool-api-1.1.1rc4/README.md` & `tej_tool_api-1.1.2rc0/README.md`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.1.1rc4/TejToolAPI/Map_Dask_API.py` & `tej_tool_api-1.1.2rc0/TejToolAPI/Map_Dask_API.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,15 +428,15 @@
     vectorized_annd_adjusted = np.vectorize(annd_adjusted)
 
     # 所有不同的發布日
     uni_dates = pd.to_datetime(data[annd].dropna().unique())
     # print(uni_dates)
 
     # 傳入 ExchangeCalendar 物件
-    result = vectorized_annd_adjusted(para.exc, uni_dates, False)
+    result = vectorized_annd_adjusted(para.exc, uni_dates, True)
 
     # Create a mapping dictionary
     dict_map = {uni_dates[i]:result[i] for i in range(len(result))}
 
     data[annd] = data[annd].map(dict_map)
     # print(data[annd])
     
@@ -723,8 +723,8 @@
                     key3 = self.fin_type,
                     paginate=True,
                     chinese_column_name=False,
                     opts={'columns': self.columns, 'sort':{'coid.asc', 'mdate.asc', 'annd.asc', 'no.asc'}} 
                     )
         
         return datasets
-        
+
```

### Comparing `tej-tool-api-1.1.1rc4/TejToolAPI/TejToolAPI.py` & `tej_tool_api-1.1.2rc0/TejToolAPI/TejToolAPI.py`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.1.1rc4/TejToolAPI/__init__.py` & `tej_tool_api-1.1.2rc0/TejToolAPI/__init__.py`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.1.1rc4/TejToolAPI/exchange_calendar.py` & `tej_tool_api-1.1.2rc0/TejToolAPI/exchange_calendar.py`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.1.1rc4/TejToolAPI/meta_types.py` & `tej_tool_api-1.1.2rc0/TejToolAPI/meta_types.py`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.1.1rc4/TejToolAPI/parameters.py` & `tej_tool_api-1.1.2rc0/TejToolAPI/parameters.py`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.1.1rc4/TejToolAPI/tables/all_meta.json` & `tej_tool_api-1.1.2rc0/TejToolAPI/tables/all_meta.json`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.1.1rc4/TejToolAPI/tables/columns_group.xlsx` & `tej_tool_api-1.1.2rc0/TejToolAPI/tables/columns_group.xlsx`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.1.1rc4/TejToolAPI/utils.py` & `tej_tool_api-1.1.2rc0/TejToolAPI/utils.py`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.1.1rc4/pyproject.toml` & `tej_tool_api-1.1.2rc0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     'Natural Language :: English',
     'Natural Language :: Chinese (Traditional)',
     'Programming Language :: Python',
     'Topic :: Office/Business :: Financial :: Investment',
     'Topic :: Scientific/Engineering :: Information Analysis',
 ]
 
+license = { text = 'Apache-2.0'}
+
 [tool.poetry.dependencies]
 # requires-python = '>=3.8'
 # dependencies = [
 #     'dask >= 2022.4.1',
 #     'pandas >= 1.2.5, <= 1.5.3',
 #     'tejapi >= 0.1.27',
 #     'xlrd >= 1.0.0',
```

