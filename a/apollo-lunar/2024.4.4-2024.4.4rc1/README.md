# Comparing `tmp/apollo_lunar-2024.4.4.tar.gz` & `tmp/apollo_lunar-2024.4.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo_lunar-2024.4.4.tar", max compression
+gzip compressed data, was "apollo_lunar-2024.4.4rc1.tar", max compression
```

## Comparing `apollo_lunar-2024.4.4.tar` & `apollo_lunar-2024.4.4rc1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1089 2024-04-08 07:58:04.862661 apollo_lunar-2024.4.4/LICENSE
--rw-r--r--   0        0        0     4618 2024-04-08 07:58:04.862661 apollo_lunar-2024.4.4/README.md
--rw-r--r--   0        0        0       56 2024-04-08 07:58:04.862661 apollo_lunar-2024.4.4/bap/__init__.py
--rw-r--r--   0        0        0     6034 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/__init__.py
--rw-r--r--   0        0        0    12593 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/cli.py
--rw-r--r--   0        0        0     4502 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/config/__init__.py
--rw-r--r--   0        0        0      255 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/data/__init__.py
--rw-r--r--   0        0        0       58 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/data/batch/__init__.py
--rw-r--r--   0        0        0     1794 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/data/batch/batch.py
--rw-r--r--   0        0        0       99 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/data/batch/models/__init__.py
--rw-r--r--   0        0        0      421 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/data/batch/models/batch_models.py
--rw-r--r--   0        0        0       55 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/data/data/__init__.py
--rw-r--r--   0        0        0     8963 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/data/data/data.py
--rw-r--r--   0        0        0      103 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/data/datasets/__init__.py
--rw-r--r--   0        0        0     8959 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/data/datasets/dataset.py
--rw-r--r--   0        0        0      123 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/data/datasets/models/__init__.py
--rw-r--r--   0        0        0      856 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/data/datasets/models/dataset_models.py
--rw-r--r--   0        0        0      150 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/data/datasets/models/params/__init__.py
--rw-r--r--   0        0        0      845 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/data/datasets/models/params/dynamodb.py
--rw-r--r--   0        0        0       67 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/data/dynamodb/__init__.py
--rw-r--r--   0        0        0     2853 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/data/dynamodb/dynamodb.py
--rw-r--r--   0        0        0       58 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/data/query/__init__.py
--rw-r--r--   0        0        0     3340 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/data/query/query.py
--rw-r--r--   0        0        0     2768 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/lunar_client.py
--rw-r--r--   0        0        0      224 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/ml/__init__.py
--rw-r--r--   0        0        0     7845 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/ml/aidp_service.py
--rw-r--r--   0        0        0     6495 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/ml/edd_service.py
--rw-r--r--   0        0        0      740 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/ml/lunar_model.py
--rw-r--r--   0        0        0     4075 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/ml/model_registry.py
--rw-r--r--   0        0        0      201 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/rec/__init__.py
--rw-r--r--   0        0        0       64 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/rec/channels/__init__.py
--rw-r--r--   0        0        0     7391 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/rec/channels/channel.py
--rw-r--r--   0        0        0      123 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/rec/channels/models/__init__.py
--rw-r--r--   0        0        0      461 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/rec/channels/models/channel_models.py
--rw-r--r--   0        0        0       74 2024-04-08 07:58:04.866661 apollo_lunar-2024.4.4/lunar/rec/experiments/__init__.py
--rw-r--r--   0        0        0     9615 2024-04-08 07:58:04.870661 apollo_lunar-2024.4.4/lunar/rec/experiments/experiment.py
--rw-r--r--   0        0        0      144 2024-04-08 07:58:04.870661 apollo_lunar-2024.4.4/lunar/rec/experiments/models/__init__.py
--rw-r--r--   0        0        0     1768 2024-04-08 07:58:04.870661 apollo_lunar-2024.4.4/lunar/rec/experiments/models/experiment_models.py
--rw-r--r--   0        0        0       85 2024-04-08 07:58:04.870661 apollo_lunar-2024.4.4/lunar/rec/recommendations/__init__.py
--rw-r--r--   0        0        0      124 2024-04-08 07:58:04.870661 apollo_lunar-2024.4.4/lunar/rec/recommendations/models/__init__.py
--rw-r--r--   0        0        0      799 2024-04-08 07:58:04.870661 apollo_lunar-2024.4.4/lunar/rec/recommendations/models/recommendation_models.py
--rw-r--r--   0        0        0     2432 2024-04-08 07:58:04.870661 apollo_lunar-2024.4.4/lunar/rec/recommendations/recommendation.py
--rw-r--r--   0        0        0     1042 2024-04-08 07:58:04.870661 apollo_lunar-2024.4.4/pyproject.toml
--rw-r--r--   0        0        0     5541 1970-01-01 00:00:00.000000 apollo_lunar-2024.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-04 06:47:55.801702 apollo_lunar-2024.4.4rc1/LICENSE
+-rw-r--r--   0        0        0     4618 2024-04-04 06:47:55.801702 apollo_lunar-2024.4.4rc1/README.md
+-rw-r--r--   0        0        0       56 2024-04-04 06:47:55.801702 apollo_lunar-2024.4.4rc1/bap/__init__.py
+-rw-r--r--   0        0        0     6034 2024-04-04 06:47:55.801702 apollo_lunar-2024.4.4rc1/lunar/__init__.py
+-rw-r--r--   0        0        0    12593 2024-04-04 06:47:55.801702 apollo_lunar-2024.4.4rc1/lunar/cli.py
+-rw-r--r--   0        0        0     4502 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/config/__init__.py
+-rw-r--r--   0        0        0      255 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/__init__.py
+-rw-r--r--   0        0        0       58 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/batch/__init__.py
+-rw-r--r--   0        0        0     1794 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/batch/batch.py
+-rw-r--r--   0        0        0       99 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/batch/models/__init__.py
+-rw-r--r--   0        0        0      421 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/batch/models/batch_models.py
+-rw-r--r--   0        0        0       55 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/data/__init__.py
+-rw-r--r--   0        0        0     8963 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/data/data.py
+-rw-r--r--   0        0        0      103 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     8959 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/datasets/dataset.py
+-rw-r--r--   0        0        0      123 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/datasets/models/__init__.py
+-rw-r--r--   0        0        0      856 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/datasets/models/dataset_models.py
+-rw-r--r--   0        0        0      150 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/datasets/models/params/__init__.py
+-rw-r--r--   0        0        0      845 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/datasets/models/params/dynamodb.py
+-rw-r--r--   0        0        0       67 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/dynamodb/__init__.py
+-rw-r--r--   0        0        0     2853 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/dynamodb/dynamodb.py
+-rw-r--r--   0        0        0       58 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/query/__init__.py
+-rw-r--r--   0        0        0     3340 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/data/query/query.py
+-rw-r--r--   0        0        0     2768 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/lunar_client.py
+-rw-r--r--   0        0        0      224 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/ml/__init__.py
+-rw-r--r--   0        0        0     7845 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/ml/aidp_service.py
+-rw-r--r--   0        0        0     6495 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/ml/edd_service.py
+-rw-r--r--   0        0        0      740 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/ml/lunar_model.py
+-rw-r--r--   0        0        0     4075 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/ml/model_registry.py
+-rw-r--r--   0        0        0      201 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/__init__.py
+-rw-r--r--   0        0        0       64 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/channels/__init__.py
+-rw-r--r--   0        0        0     7391 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/channels/channel.py
+-rw-r--r--   0        0        0      123 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/channels/models/__init__.py
+-rw-r--r--   0        0        0      461 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/channels/models/channel_models.py
+-rw-r--r--   0        0        0       74 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/experiments/__init__.py
+-rw-r--r--   0        0        0     9615 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/experiments/experiment.py
+-rw-r--r--   0        0        0      144 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/experiments/models/__init__.py
+-rw-r--r--   0        0        0     1768 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/experiments/models/experiment_models.py
+-rw-r--r--   0        0        0       85 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/recommendations/__init__.py
+-rw-r--r--   0        0        0      124 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/recommendations/models/__init__.py
+-rw-r--r--   0        0        0      799 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/recommendations/models/recommendation_models.py
+-rw-r--r--   0        0        0     2432 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/lunar/rec/recommendations/recommendation.py
+-rw-r--r--   0        0        0     1045 2024-04-04 06:47:55.805702 apollo_lunar-2024.4.4rc1/pyproject.toml
+-rw-r--r--   0        0        0     5544 1970-01-01 00:00:00.000000 apollo_lunar-2024.4.4rc1/PKG-INFO
```

### Comparing `apollo_lunar-2024.4.4/LICENSE` & `apollo_lunar-2024.4.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.4.4/README.md` & `apollo_lunar-2024.4.4rc1/README.md`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.4.4/lunar/__init__.py` & `apollo_lunar-2024.4.4rc1/lunar/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.4.4/lunar/cli.py` & `apollo_lunar-2024.4.4rc1/lunar/cli.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.4.4/lunar/config/__init__.py` & `apollo_lunar-2024.4.4rc1/lunar/config/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.4.4/lunar/data/batch/batch.py` & `apollo_lunar-2024.4.4rc1/lunar/data/batch/batch.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.4.4/lunar/data/data/data.py` & `apollo_lunar-2024.4.4rc1/lunar/data/data/data.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.4.4/lunar/data/datasets/dataset.py` & `apollo_lunar-2024.4.4rc1/lunar/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.4.4/lunar/data/datasets/models/dataset_models.py` & `apollo_lunar-2024.4.4rc1/lunar/data/datasets/models/dataset_models.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.4.4/lunar/data/datasets/models/params/dynamodb.py` & `apollo_lunar-2024.4.4rc1/lunar/data/datasets/models/params/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.4.4/lunar/data/dynamodb/dynamodb.py` & `apollo_lunar-2024.4.4rc1/lunar/data/dynamodb/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.4.4/lunar/data/query/query.py` & `apollo_lunar-2024.4.4rc1/lunar/data/query/query.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.4.4/lunar/lunar_client.py` & `apollo_lunar-2024.4.4rc1/lunar/lunar_client.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.4.4/lunar/ml/aidp_service.py` & `apollo_lunar-2024.4.4rc1/lunar/ml/aidp_service.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.4.4/lunar/ml/edd_service.py` & `apollo_lunar-2024.4.4rc1/lunar/ml/edd_service.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.4.4/lunar/ml/lunar_model.py` & `apollo_lunar-2024.4.4rc1/lunar/ml/lunar_model.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.4.4/lunar/ml/model_registry.py` & `apollo_lunar-2024.4.4rc1/lunar/ml/model_registry.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.4.4/lunar/rec/channels/channel.py` & `apollo_lunar-2024.4.4rc1/lunar/rec/channels/channel.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.4.4/lunar/rec/experiments/experiment.py` & `apollo_lunar-2024.4.4rc1/lunar/rec/experiments/experiment.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.4.4/lunar/rec/experiments/models/experiment_models.py` & `apollo_lunar-2024.4.4rc1/lunar/rec/experiments/models/experiment_models.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.4.4/lunar/rec/recommendations/models/recommendation_models.py` & `apollo_lunar-2024.4.4rc1/lunar/rec/recommendations/models/recommendation_models.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.4.4/lunar/rec/recommendations/recommendation.py` & `apollo_lunar-2024.4.4rc1/lunar/rec/recommendations/recommendation.py`

 * *Files identical despite different names*

### Comparing `apollo_lunar-2024.4.4/pyproject.toml` & `apollo_lunar-2024.4.4rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apollo-lunar"
-version = "2024.4.4"
+version = "2024.4.4rc1"
 description = "A Python SDK/CLI for Lunar API"
 authors = ["Lunar module <lunar@sktio.io>"]
 readme = "README.md"
 license = "MIT"
 include = [
     "LICENSE",
 ]
```

### Comparing `apollo_lunar-2024.4.4/PKG-INFO` & `apollo_lunar-2024.4.4rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-lunar
-Version: 2024.4.4
+Version: 2024.4.4rc1
 Summary: A Python SDK/CLI for Lunar API
 License: MIT
 Author: Lunar module
 Author-email: lunar@sktio.io
 Requires-Python: >=3.8,<3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

