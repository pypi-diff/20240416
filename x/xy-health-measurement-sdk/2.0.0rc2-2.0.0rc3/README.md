# Comparing `tmp/xy_health_measurement_sdk-2.0.0rc2.tar.gz` & `tmp/xy_health_measurement_sdk-2.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xy_health_measurement_sdk-2.0.0rc2.tar", last modified: Mon Apr 15 08:22:20 2024, max compression
+gzip compressed data, was "xy_health_measurement_sdk-2.0.0rc3.tar", last modified: Tue Apr 16 04:04:20 2024, max compression
```

## Comparing `xy_health_measurement_sdk-2.0.0rc2.tar` & `xy_health_measurement_sdk-2.0.0rc3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 colin     (1001) colin     (1001)        0 2024-04-15 08:22:20.057406 xy_health_measurement_sdk-2.0.0rc2/
--rw-rw-r--   0 colin     (1001) colin     (1001)     1087 2024-04-10 17:28:32.000000 xy_health_measurement_sdk-2.0.0rc2/LICENSE
--rw-rw-r--   0 colin     (1001) colin     (1001)       41 2024-04-10 17:46:29.000000 xy_health_measurement_sdk-2.0.0rc2/MANIFEST.in
--rw-r--r--   0 colin     (1001) colin     (1001)     1003 2024-04-15 08:22:20.057406 xy_health_measurement_sdk-2.0.0rc2/PKG-INFO
--rw-rw-r--   0 colin     (1001) colin     (1001)      208 2024-04-15 08:22:09.000000 xy_health_measurement_sdk-2.0.0rc2/README.md
--rw-rw-r--   0 colin     (1001) colin     (1001)      847 2024-04-15 07:58:42.000000 xy_health_measurement_sdk-2.0.0rc2/pyproject.toml
--rw-rw-r--   0 colin     (1001) colin     (1001)       38 2024-04-15 08:22:20.057406 xy_health_measurement_sdk-2.0.0rc2/setup.cfg
-drwxrwxr-x   0 colin     (1001) colin     (1001)        0 2024-04-15 08:22:20.045405 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/
--rw-rw-r--   0 colin     (1001) colin     (1001)     9586 2024-04-11 13:11:53.000000 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/FeatureExtractor.py
--rw-rw-r--   0 colin     (1001) colin     (1001)     5953 2024-04-11 11:58:16.000000 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/Measurement.py
--rw-rw-r--   0 colin     (1001) colin     (1001)     5731 2024-04-10 16:42:13.000000 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/MeasurerProcess.py
--rw-rw-r--   0 colin     (1001) colin     (1001)     5969 2024-04-15 07:38:24.000000 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/Rpcer.py
--rw-rw-r--   0 colin     (1001) colin     (1001)     6584 2024-04-15 07:56:20.000000 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/SignalProcessor.py
--rw-rw-r--   0 colin     (1001) colin     (1001)     4227 2024-04-11 10:16:07.000000 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/Utilities.py
--rw-rw-r--   0 colin     (1001) colin     (1001)        0 2024-03-27 14:25:44.000000 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/__init__.py
-drwxrwxr-x   0 colin     (1001) colin     (1001)        0 2024-04-15 08:22:20.049405 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/protos/
--rw-r--r--   0 colin     (1001) colin     (1001)     1943 2024-04-10 16:14:16.000000 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/protos/Category_pb2.py
--rw-r--r--   0 colin     (1001) colin     (1001)     4719 2024-04-10 16:14:16.000000 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/protos/Chunk_pb2.py
--rw-rw-r--   0 colin     (1001) colin     (1001)    12865 2024-04-10 16:14:16.000000 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/protos/Report_pb2.py
--rw-r--r--   0 colin     (1001) colin     (1001)     2339 2024-04-10 16:14:16.000000 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/protos/Validation_pb2.py
--rw-rw-r--   0 colin     (1001) colin     (1001)        0 2024-04-10 14:40:33.000000 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/protos/__init__.py
-drwxrwxr-x   0 colin     (1001) colin     (1001)        0 2024-04-15 08:22:20.049405 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/resources/
--rw-rw-r--   0 colin     (1001) colin     (1001)        0 2024-03-27 14:25:44.000000 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/resources/__init__.py
-drwxrwxr-x   0 colin     (1001) colin     (1001)        0 2024-04-15 08:22:20.057406 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/resources/__pycache__/
--rw-rw-r--   0 colin     (1001) colin     (1001)      189 2024-04-10 16:34:59.000000 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/resources/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 colin     (1001) colin     (1001)     4230 2024-04-11 10:03:52.000000 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/resources/config.json
--rw-rw-r--   0 colin     (1001) colin     (1001)  3758596 2024-03-28 16:58:49.000000 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/resources/face_landmarker.task
-drwxrwxr-x   0 colin     (1001) colin     (1001)        0 2024-04-15 08:22:20.057406 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk.egg-info/
--rw-r--r--   0 colin     (1001) colin     (1001)     1003 2024-04-15 08:22:20.000000 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 colin     (1001) colin     (1001)     1041 2024-04-15 08:22:20.000000 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 colin     (1001) colin     (1001)        1 2024-04-15 08:22:20.000000 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 colin     (1001) colin     (1001)       97 2024-04-15 08:22:20.000000 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk.egg-info/requires.txt
--rw-rw-r--   0 colin     (1001) colin     (1001)       26 2024-04-15 08:22:20.000000 xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 colin     (1001) colin     (1001)        0 2024-04-16 04:04:20.707481 xy_health_measurement_sdk-2.0.0rc3/
+-rw-rw-r--   0 colin     (1001) colin     (1001)     1087 2024-04-10 17:28:32.000000 xy_health_measurement_sdk-2.0.0rc3/LICENSE
+-rw-rw-r--   0 colin     (1001) colin     (1001)       41 2024-04-10 17:46:29.000000 xy_health_measurement_sdk-2.0.0rc3/MANIFEST.in
+-rw-r--r--   0 colin     (1001) colin     (1001)     1003 2024-04-16 04:04:20.707481 xy_health_measurement_sdk-2.0.0rc3/PKG-INFO
+-rw-rw-r--   0 colin     (1001) colin     (1001)      208 2024-04-15 08:24:48.000000 xy_health_measurement_sdk-2.0.0rc3/README.md
+-rw-rw-r--   0 colin     (1001) colin     (1001)      847 2024-04-16 03:50:10.000000 xy_health_measurement_sdk-2.0.0rc3/pyproject.toml
+-rw-rw-r--   0 colin     (1001) colin     (1001)       38 2024-04-16 04:04:20.707481 xy_health_measurement_sdk-2.0.0rc3/setup.cfg
+drwxrwxr-x   0 colin     (1001) colin     (1001)        0 2024-04-16 04:04:20.703482 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/
+-rw-rw-r--   0 colin     (1001) colin     (1001)     9586 2024-04-11 13:11:53.000000 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/FeatureExtractor.py
+-rw-rw-r--   0 colin     (1001) colin     (1001)     5953 2024-04-11 11:58:16.000000 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/Measurement.py
+-rw-rw-r--   0 colin     (1001) colin     (1001)     5731 2024-04-10 16:42:13.000000 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/MeasurerProcess.py
+-rw-rw-r--   0 colin     (1001) colin     (1001)     5969 2024-04-15 07:38:24.000000 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/Rpcer.py
+-rw-rw-r--   0 colin     (1001) colin     (1001)     6584 2024-04-15 07:56:20.000000 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/SignalProcessor.py
+-rw-rw-r--   0 colin     (1001) colin     (1001)     4245 2024-04-16 03:43:46.000000 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/Utilities.py
+-rw-rw-r--   0 colin     (1001) colin     (1001)        0 2024-03-27 14:25:44.000000 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/__init__.py
+drwxrwxr-x   0 colin     (1001) colin     (1001)        0 2024-04-16 04:04:20.703482 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/protos/
+-rw-r--r--   0 colin     (1001) colin     (1001)     1943 2024-04-10 16:14:16.000000 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/protos/Category_pb2.py
+-rw-r--r--   0 colin     (1001) colin     (1001)     4719 2024-04-10 16:14:16.000000 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/protos/Chunk_pb2.py
+-rw-rw-r--   0 colin     (1001) colin     (1001)    12865 2024-04-10 16:14:16.000000 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/protos/Report_pb2.py
+-rw-r--r--   0 colin     (1001) colin     (1001)     2339 2024-04-10 16:14:16.000000 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/protos/Validation_pb2.py
+-rw-rw-r--   0 colin     (1001) colin     (1001)        0 2024-04-10 14:40:33.000000 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/protos/__init__.py
+drwxrwxr-x   0 colin     (1001) colin     (1001)        0 2024-04-16 04:04:20.703482 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/resources/
+-rw-rw-r--   0 colin     (1001) colin     (1001)        0 2024-03-27 14:25:44.000000 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/resources/__init__.py
+drwxrwxr-x   0 colin     (1001) colin     (1001)        0 2024-04-16 04:04:20.707481 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/resources/__pycache__/
+-rw-rw-r--   0 colin     (1001) colin     (1001)      189 2024-04-10 16:34:59.000000 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/resources/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 colin     (1001) colin     (1001)     4230 2024-04-11 10:03:52.000000 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/resources/config.json
+-rw-rw-r--   0 colin     (1001) colin     (1001)  3758596 2024-03-28 16:58:49.000000 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/resources/face_landmarker.task
+drwxrwxr-x   0 colin     (1001) colin     (1001)        0 2024-04-16 04:04:20.707481 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk.egg-info/
+-rw-r--r--   0 colin     (1001) colin     (1001)     1003 2024-04-16 04:04:20.000000 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 colin     (1001) colin     (1001)     1041 2024-04-16 04:04:20.000000 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 colin     (1001) colin     (1001)        1 2024-04-16 04:04:20.000000 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 colin     (1001) colin     (1001)       97 2024-04-16 04:04:20.000000 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk.egg-info/requires.txt
+-rw-rw-r--   0 colin     (1001) colin     (1001)       26 2024-04-16 04:04:20.000000 xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk.egg-info/top_level.txt
```

### Comparing `xy_health_measurement_sdk-2.0.0rc2/LICENSE` & `xy_health_measurement_sdk-2.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `xy_health_measurement_sdk-2.0.0rc2/PKG-INFO` & `xy_health_measurement_sdk-2.0.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xy_health_measurement_sdk
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: 小阳心健康测量SDK
 Author-email: Colin Chang <zhangcheng@xymind.cn>
 Keywords: 健康测量,生理测量,情绪测量,健康风险,小阳科技
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `xy_health_measurement_sdk-2.0.0rc2/pyproject.toml` & `xy_health_measurement_sdk-2.0.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xy_health_measurement_sdk"
-version = "2.0.0rc2"
+version = "2.0.0rc3"
 keywords = ["健康测量", "生理测量", "情绪测量", "健康风险", "小阳科技"]
 description = "小阳心健康测量SDK"
 authors = [
     { name = "Colin Chang", email = "zhangcheng@xymind.cn" },
 ]
 readme = "README.md"
 requires-python = ">=3.8,<=3.11"
```

### Comparing `xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/FeatureExtractor.py` & `xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/FeatureExtractor.py`

 * *Files identical despite different names*

### Comparing `xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/Measurement.py` & `xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/Measurement.py`

 * *Files identical despite different names*

### Comparing `xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/MeasurerProcess.py` & `xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/MeasurerProcess.py`

 * *Files identical despite different names*

### Comparing `xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/Rpcer.py` & `xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/Rpcer.py`

 * *Files identical despite different names*

### Comparing `xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/SignalProcessor.py` & `xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/SignalProcessor.py`

 * *Files identical despite different names*

### Comparing `xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/Utilities.py` & `xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/Utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from multiprocessing import Value, Array
 from re import sub
 from .protos.Validation_pb2 import Validation, UnknownError
 
 
 class Utility(object):
     with resources_path('xy_health_measurement_sdk.resources', 'config.json') as config:
-        with open(config, 'r') as file:
+        with open(config, 'r', encoding='utf-8') as file:
             __config = load(file)
             __validation = __config['validation']
 
     @classmethod
     def get_validation(cls, code: Validation):
         # validation子节点配置会在业务中根据情况修改作为返回值
         # 深度拷贝可以防止业务修改影响全局默认配置
```

### Comparing `xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/protos/Category_pb2.py` & `xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/protos/Category_pb2.py`

 * *Files identical despite different names*

### Comparing `xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/protos/Chunk_pb2.py` & `xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/protos/Chunk_pb2.py`

 * *Files identical despite different names*

### Comparing `xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/protos/Report_pb2.py` & `xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/protos/Report_pb2.py`

 * *Files identical despite different names*

### Comparing `xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/protos/Validation_pb2.py` & `xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/protos/Validation_pb2.py`

 * *Files identical despite different names*

### Comparing `xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/resources/config.json` & `xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/resources/config.json`

 * *Files identical despite different names*

### Comparing `xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk/resources/face_landmarker.task` & `xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk/resources/face_landmarker.task`

 * *Files identical despite different names*

### Comparing `xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk.egg-info/PKG-INFO` & `xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xy_health_measurement_sdk
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: 小阳心健康测量SDK
 Author-email: Colin Chang <zhangcheng@xymind.cn>
 Keywords: 健康测量,生理测量,情绪测量,健康风险,小阳科技
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `xy_health_measurement_sdk-2.0.0rc2/xy_health_measurement_sdk.egg-info/SOURCES.txt` & `xy_health_measurement_sdk-2.0.0rc3/xy_health_measurement_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

