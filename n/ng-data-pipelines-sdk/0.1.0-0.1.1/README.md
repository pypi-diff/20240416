# Comparing `tmp/ng_data_pipelines_sdk-0.1.0.tar.gz` & `tmp/ng_data_pipelines_sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng_data_pipelines_sdk-0.1.0.tar", max compression
+gzip compressed data, was "ng_data_pipelines_sdk-0.1.1.tar", max compression
```

## Comparing `ng_data_pipelines_sdk-0.1.0.tar` & `ng_data_pipelines_sdk-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      106 2024-04-16 18:05:39.947866 ng_data_pipelines_sdk-0.1.0/README.md
--rw-r--r--   0        0        0       40 2024-04-16 18:05:39.947866 ng_data_pipelines_sdk-0.1.0/ng_data_pipelines_sdk/__init__.py
--rw-r--r--   0        0        0     4434 2024-04-16 18:05:39.947866 ng_data_pipelines_sdk-0.1.0/ng_data_pipelines_sdk/aws_interface.py
--rw-r--r--   0        0        0      231 2024-04-16 18:05:39.947866 ng_data_pipelines_sdk-0.1.0/ng_data_pipelines_sdk/custom_logger.py
--rw-r--r--   0        0        0    24305 2024-04-16 18:05:39.947866 ng_data_pipelines_sdk-0.1.0/ng_data_pipelines_sdk/dataframe_manager.py
--rw-r--r--   0        0        0     8365 2024-04-16 18:05:39.947866 ng_data_pipelines_sdk-0.1.0/ng_data_pipelines_sdk/interfaces.py
--rw-r--r--   0        0        0     2969 2024-04-16 18:05:39.947866 ng_data_pipelines_sdk-0.1.0/ng_data_pipelines_sdk/spark_manager.py
--rw-r--r--   0        0        0     3498 2024-04-16 18:05:39.947866 ng_data_pipelines_sdk-0.1.0/ng_data_pipelines_sdk/utils.py
--rw-r--r--   0        0        0      458 2024-04-16 18:05:39.948866 ng_data_pipelines_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-04-16 21:56:30.294954 ng_data_pipelines_sdk-0.1.1/README.md
+-rw-r--r--   0        0        0       40 2024-04-16 21:56:30.294954 ng_data_pipelines_sdk-0.1.1/ng_data_pipelines_sdk/__init__.py
+-rw-r--r--   0        0        0     4434 2024-04-16 21:56:30.294954 ng_data_pipelines_sdk-0.1.1/ng_data_pipelines_sdk/aws_interface.py
+-rw-r--r--   0        0        0      231 2024-04-16 21:56:30.295954 ng_data_pipelines_sdk-0.1.1/ng_data_pipelines_sdk/custom_logger.py
+-rw-r--r--   0        0        0    24305 2024-04-16 21:56:30.295954 ng_data_pipelines_sdk-0.1.1/ng_data_pipelines_sdk/dataframe_manager.py
+-rw-r--r--   0        0        0     8365 2024-04-16 21:56:30.295954 ng_data_pipelines_sdk-0.1.1/ng_data_pipelines_sdk/interfaces.py
+-rw-r--r--   0        0        0     2969 2024-04-16 21:56:30.295954 ng_data_pipelines_sdk-0.1.1/ng_data_pipelines_sdk/spark_manager.py
+-rw-r--r--   0        0        0     3498 2024-04-16 21:56:30.295954 ng_data_pipelines_sdk-0.1.1/ng_data_pipelines_sdk/utils.py
+-rw-r--r--   0        0        0      458 2024-04-16 21:56:30.295954 ng_data_pipelines_sdk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      559 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.1.1/PKG-INFO
```

### Comparing `ng_data_pipelines_sdk-0.1.0/ng_data_pipelines_sdk/aws_interface.py` & `ng_data_pipelines_sdk-0.1.1/ng_data_pipelines_sdk/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.0/ng_data_pipelines_sdk/dataframe_manager.py` & `ng_data_pipelines_sdk-0.1.1/ng_data_pipelines_sdk/dataframe_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.0/ng_data_pipelines_sdk/interfaces.py` & `ng_data_pipelines_sdk-0.1.1/ng_data_pipelines_sdk/interfaces.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.0/ng_data_pipelines_sdk/spark_manager.py` & `ng_data_pipelines_sdk-0.1.1/ng_data_pipelines_sdk/spark_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.0/ng_data_pipelines_sdk/utils.py` & `ng_data_pipelines_sdk-0.1.1/ng_data_pipelines_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.0/PKG-INFO` & `ng_data_pipelines_sdk-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 Metadata-Version: 2.1
 Name: ng-data-pipelines-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library for facilitating the development of data engineering pipelines
 Author: ng.cash
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.34.84,<2.0.0)
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: pyspark (>=3.5.0,<3.6.0)
 Description-Content-Type: text/markdown
 
 docker run --rm -it -d -e PYTHONPATH="/ng-data-pipelines-sdk" -v $pwd:/ng-data-pipelines-sdk pyspark-local
```

