# Comparing `tmp/database-common-tools-1.0.7.tar.gz` & `tmp/database-common-tools-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database-common-tools-1.0.7.tar", last modified: Mon Apr 15 02:57:38 2024, max compression
+gzip compressed data, was "database-common-tools-1.0.8.tar", last modified: Tue Apr 16 08:07:36 2024, max compression
```

## Comparing `database-common-tools-1.0.7.tar` & `database-common-tools-1.0.8.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-15 02:57:38.515877 database-common-tools-1.0.7/
--rw-r--r--   0 yangming   (501) staff       (20)     1066 2024-01-24 08:52:12.000000 database-common-tools-1.0.7/LICENSE
--rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-15 02:57:38.515358 database-common-tools-1.0.7/PKG-INFO
--rw-r--r--   0 yangming   (501) staff       (20)       23 2024-01-24 08:52:12.000000 database-common-tools-1.0.7/README.md
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-15 02:57:38.506814 database-common-tools-1.0.7/database_common_tools.egg-info/
--rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-15 02:57:38.000000 database-common-tools-1.0.7/database_common_tools.egg-info/PKG-INFO
--rw-r--r--   0 yangming   (501) staff       (20)      578 2024-04-15 02:57:38.000000 database-common-tools-1.0.7/database_common_tools.egg-info/SOURCES.txt
--rw-r--r--   0 yangming   (501) staff       (20)        1 2024-04-15 02:57:38.000000 database-common-tools-1.0.7/database_common_tools.egg-info/dependency_links.txt
--rw-r--r--   0 yangming   (501) staff       (20)       64 2024-04-15 02:57:38.000000 database-common-tools-1.0.7/database_common_tools.egg-info/requires.txt
--rw-r--r--   0 yangming   (501) staff       (20)       19 2024-04-15 02:57:38.000000 database-common-tools-1.0.7/database_common_tools.egg-info/top_level.txt
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-15 02:57:38.514295 database-common-tools-1.0.7/databasetools/
--rw-r--r--   0 yangming   (501) staff       (20)     1636 2024-01-25 08:25:09.000000 database-common-tools-1.0.7/databasetools/__init__.py
--rw-r--r--   0 yangming   (501) staff       (20)     1990 2024-01-24 09:06:09.000000 database-common-tools-1.0.7/databasetools/analysis_json.py
--rw-r--r--   0 yangming   (501) staff       (20)     1173 2024-01-24 09:06:09.000000 database-common-tools-1.0.7/databasetools/analysis_json_v2.py
--rw-r--r--   0 yangming   (501) staff       (20)     3191 2024-01-24 09:06:09.000000 database-common-tools-1.0.7/databasetools/data_analysis.py
--rw-r--r--   0 yangming   (501) staff       (20)     2806 2024-01-26 08:20:48.000000 database-common-tools-1.0.7/databasetools/data_analysis_v2.py
--rw-r--r--   0 yangming   (501) staff       (20)      331 2024-01-26 03:25:22.000000 database-common-tools-1.0.7/databasetools/kafka_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)     2180 2024-03-14 06:55:26.000000 database-common-tools-1.0.7/databasetools/mongo_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)      721 2024-01-26 07:55:44.000000 database-common-tools-1.0.7/databasetools/mt_wx_message.py
--rw-r--r--   0 yangming   (501) staff       (20)      279 2024-04-15 02:52:56.000000 database-common-tools-1.0.7/databasetools/mysql_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)     5458 2024-01-26 08:31:58.000000 database-common-tools-1.0.7/databasetools/redis_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)       38 2024-04-15 02:57:38.516065 database-common-tools-1.0.7/setup.cfg
--rw-r--r--   0 yangming   (501) staff       (20)     3904 2024-04-15 02:56:21.000000 database-common-tools-1.0.7/setup.py
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-15 02:57:38.514838 database-common-tools-1.0.7/test/
--rw-r--r--   0 yangming   (501) staff       (20)        0 2024-01-26 07:51:53.000000 database-common-tools-1.0.7/test/__init__.py
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-16 08:07:36.454096 database-common-tools-1.0.8/
+-rw-r--r--   0 yangming   (501) staff       (20)     1066 2024-01-24 08:52:12.000000 database-common-tools-1.0.8/LICENSE
+-rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-16 08:07:36.453375 database-common-tools-1.0.8/PKG-INFO
+-rw-r--r--   0 yangming   (501) staff       (20)       23 2024-01-24 08:52:12.000000 database-common-tools-1.0.8/README.md
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-16 08:07:36.440513 database-common-tools-1.0.8/database_common_tools.egg-info/
+-rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-16 08:07:36.000000 database-common-tools-1.0.8/database_common_tools.egg-info/PKG-INFO
+-rw-r--r--   0 yangming   (501) staff       (20)      682 2024-04-16 08:07:36.000000 database-common-tools-1.0.8/database_common_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 yangming   (501) staff       (20)        1 2024-04-16 08:07:36.000000 database-common-tools-1.0.8/database_common_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 yangming   (501) staff       (20)       85 2024-04-16 08:07:36.000000 database-common-tools-1.0.8/database_common_tools.egg-info/requires.txt
+-rw-r--r--   0 yangming   (501) staff       (20)       19 2024-04-16 08:07:36.000000 database-common-tools-1.0.8/database_common_tools.egg-info/top_level.txt
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-16 08:07:36.451751 database-common-tools-1.0.8/databasetools/
+-rw-r--r--   0 yangming   (501) staff       (20)     1636 2024-01-25 08:25:09.000000 database-common-tools-1.0.8/databasetools/__init__.py
+-rw-r--r--   0 yangming   (501) staff       (20)     1990 2024-01-24 09:06:09.000000 database-common-tools-1.0.8/databasetools/analysis_json.py
+-rw-r--r--   0 yangming   (501) staff       (20)     2090 2024-04-16 07:53:00.000000 database-common-tools-1.0.8/databasetools/analysis_json_v2.py
+-rw-r--r--   0 yangming   (501) staff       (20)     2508 2024-04-16 08:05:52.000000 database-common-tools-1.0.8/databasetools/analysis_json_v3.py
+-rw-r--r--   0 yangming   (501) staff       (20)     3191 2024-01-24 09:06:09.000000 database-common-tools-1.0.8/databasetools/data_analysis.py
+-rw-r--r--   0 yangming   (501) staff       (20)     3564 2024-04-16 06:59:31.000000 database-common-tools-1.0.8/databasetools/data_analysis_v2.py
+-rw-r--r--   0 yangming   (501) staff       (20)     4139 2024-04-16 08:04:03.000000 database-common-tools-1.0.8/databasetools/data_analysis_v3.py
+-rw-r--r--   0 yangming   (501) staff       (20)      331 2024-01-26 03:25:22.000000 database-common-tools-1.0.8/databasetools/kafka_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)     2180 2024-03-14 06:55:26.000000 database-common-tools-1.0.8/databasetools/mongo_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)      721 2024-01-26 07:55:44.000000 database-common-tools-1.0.8/databasetools/mt_wx_message.py
+-rw-r--r--   0 yangming   (501) staff       (20)      279 2024-04-15 02:52:56.000000 database-common-tools-1.0.8/databasetools/mysql_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)      939 2024-04-16 06:15:02.000000 database-common-tools-1.0.8/databasetools/opensearch_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)     5458 2024-01-26 08:31:58.000000 database-common-tools-1.0.8/databasetools/redis_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)       38 2024-04-16 08:07:36.454308 database-common-tools-1.0.8/setup.cfg
+-rw-r--r--   0 yangming   (501) staff       (20)     3932 2024-04-16 04:01:08.000000 database-common-tools-1.0.8/setup.py
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-16 08:07:36.452775 database-common-tools-1.0.8/test/
+-rw-r--r--   0 yangming   (501) staff       (20)        0 2024-01-26 07:51:53.000000 database-common-tools-1.0.8/test/__init__.py
```

### Comparing `database-common-tools-1.0.7/LICENSE` & `database-common-tools-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.7/PKG-INFO` & `database-common-tools-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-common-tools
-Version: 1.0.7
+Version: 1.0.8
 Summary: let message middleware and use database more easy
 Home-page: https://github.com/yangming9/database-common-tools.git
 Author: Coder Yang
 Author-email: yma91412@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `database-common-tools-1.0.7/database_common_tools.egg-info/PKG-INFO` & `database-common-tools-1.0.8/database_common_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-common-tools
-Version: 1.0.7
+Version: 1.0.8
 Summary: let message middleware and use database more easy
 Home-page: https://github.com/yangming9/database-common-tools.git
 Author: Coder Yang
 Author-email: yma91412@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `database-common-tools-1.0.7/databasetools/__init__.py` & `database-common-tools-1.0.8/databasetools/__init__.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.7/databasetools/analysis_json.py` & `database-common-tools-1.0.8/databasetools/analysis_json.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.7/databasetools/data_analysis.py` & `database-common-tools-1.0.8/databasetools/data_analysis.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.7/databasetools/data_analysis_v2.py` & `database-common-tools-1.0.8/databasetools/data_analysis_v2.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,25 +7,33 @@
 ##################################################
 FLD = dict()
 FLD['names'] = list()
 FLD['names'].append('necessity')  # 0
 FLD['names'].append('path')       # 1
 FLD['names'].append('type')       # 2
 FLD['names'].append('default')    # 3
+FLD['names'].append('toType')     # 4
 
 FLD['types'] = list()
 FLD['types'].append('string')         # 0
 FLD['types'].append('array')          # 1
 FLD['types'].append('object')         # 2
+FLD['types'].append('type2array')     # 3
 
 FLD['value'] = list()
 FLD['value'].append('')      # 0
 FLD['value'].append(list())  # 1
 FLD['value'].append(dict())  # 2
 
+FLD['data_type'] = list()
+FLD['data_type'].append(int)         # 0
+FLD['data_type'].append(float)       # 1
+FLD['data_type'].append(str)         # 2
+FLD['data_type'].append(list)        # 3
+
 
 ##################################################
 # src to dest doc analysis
 ##################################################
 # mapConfigFlag mapping配置标志 false 错误
 # fieldError 数据传输错误，缺少必要字段  true 错误
 def doc_fields_analysis(srcDoc, destDoc, _mapping):
@@ -35,14 +43,15 @@
     for _field, _map in _mapping.items():
         mapConfigFlag = True
         keyError = False
         necessity = _map.get(FLD['names'][0], False)
         if isinstance(_map, dict):
             path = _map.get(FLD['names'][1], None)
             _type = _map.get(FLD['names'][2], FLD['types'][0])
+            _toType = _map.get(FLD['names'][4], FLD['data_type'][2])
             if path:
                 if FLD['types'][0] == _type:
                     # init string
                     default_value = _map.get(FLD['names'][3], FLD['value'][0])
                     status, fieldValue = analysis_json_v2.dump_doc_field_str(srcDoc, path, default_value)
                     destDoc[_field] = fieldValue
                     if not status:
@@ -57,14 +66,21 @@
                 elif FLD['types'][2] == _type:
                     # init field object
                     default_value = _map.get(FLD['names'][3], FLD['value'][2])
                     status, fieldValue = analysis_json_v2.dump_doc_field_object(srcDoc, path, default_value)
                     destDoc[_field] = fieldValue
                     if not status:
                         keyError = True
+                elif FLD['types'][3] == _type:
+                    # init field string2array
+                    default_value = _map.get(FLD['names'][3], FLD['value'][3])
+                    status, fieldValue = analysis_json_v2.dump_doc_field_type2array(srcDoc, path, default_value, _toType)
+                    destDoc[_field] = fieldValue
+                    if not status:
+                        keyError = True
             else:
                 mapConfigFlag = False
         if not necessity and keyError:
             errorKeys.append(_field)
         if necessity and keyError:
             fieldError = keyError
             break
```

### Comparing `database-common-tools-1.0.7/databasetools/mongo_connect.py` & `database-common-tools-1.0.8/databasetools/mongo_connect.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.7/databasetools/mt_wx_message.py` & `database-common-tools-1.0.8/databasetools/mt_wx_message.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.7/databasetools/redis_connect.py` & `database-common-tools-1.0.8/databasetools/redis_connect.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.7/setup.py` & `database-common-tools-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,26 @@
 # Package meta-data.
 NAME = 'database-common-tools'
 DESCRIPTION = 'let message middleware and use database more easy'
 URL = 'https://github.com/yangming9/database-common-tools.git'
 EMAIL = 'yma91412@gmail.com'
 AUTHOR = 'Coder Yang'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.0.7'
+VERSION = '1.0.8'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
     'jsonpath',
     'pymongo',
     'redis',
     'setuptools',
     'kafka-python',
-    'pymysql'
+    'pymysql',
+    'elasticsearch==7.6.0'
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

