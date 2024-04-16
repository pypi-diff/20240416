# Comparing `tmp/visionai-data-format-1.3.1.tar.gz` & `tmp/visionai_data_format-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visionai-data-format-1.3.1.tar", last modified: Tue Mar 19 10:01:37 2024, max compression
+gzip compressed data, was "visionai_data_format-1.3.2.tar", last modified: Tue Apr 16 08:41:44 2024, max compression
```

## Comparing `visionai-data-format-1.3.1.tar` & `visionai_data_format-1.3.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-03-19 10:01:37.769099 visionai-data-format-1.3.1/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    23694 2024-03-19 10:01:37.768880 visionai-data-format-1.3.1/PKG-INFO
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    23316 2024-03-19 09:51:26.000000 visionai-data-format-1.3.1/README.md
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       38 2024-03-19 10:01:37.769145 visionai-data-format-1.3.1/setup.cfg
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      753 2024-03-19 09:51:26.000000 visionai-data-format-1.3.1/setup.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-03-19 10:01:37.760733 visionai-data-format-1.3.1/tests/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     2176 2023-12-21 03:02:35.000000 visionai-data-format-1.3.1/tests/test_schemas.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     8449 2024-02-06 03:21:26.000000 visionai-data-format-1.3.1/tests/test_validators.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-03-19 10:01:37.761872 visionai-data-format-1.3.1/visionai_data_format/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai-data-format-1.3.1/visionai_data_format/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     6751 2024-03-19 09:51:26.000000 visionai-data-format-1.3.1/visionai_data_format/convert_dataset.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-03-19 10:01:37.764394 visionai-data-format-1.3.1/visionai_data_format/converters/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      173 2024-03-19 09:51:26.000000 visionai-data-format-1.3.1/visionai_data_format/converters/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1729 2023-12-21 03:02:35.000000 visionai-data-format-1.3.1/visionai_data_format/converters/base.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    16423 2024-03-19 09:51:26.000000 visionai-data-format-1.3.1/visionai_data_format/converters/bdd_to_vai.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     9363 2024-03-19 09:51:26.000000 visionai-data-format-1.3.1/visionai_data_format/converters/coco_to_vai.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    16685 2024-03-19 08:30:06.000000 visionai-data-format-1.3.1/visionai_data_format/converters/kitti_to_vai.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     9675 2024-03-19 09:51:26.000000 visionai-data-format-1.3.1/visionai_data_format/converters/vai_to_coco.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-03-19 10:01:37.765339 visionai-data-format-1.3.1/visionai_data_format/exceptions/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      156 2023-12-21 03:02:35.000000 visionai-data-format-1.3.1/visionai_data_format/exceptions/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1405 2023-12-21 03:02:35.000000 visionai-data-format-1.3.1/visionai_data_format/exceptions/constants.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     5564 2023-12-21 03:02:35.000000 visionai-data-format-1.3.1/visionai_data_format/exceptions/error_messages.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1322 2023-12-21 03:02:35.000000 visionai-data-format-1.3.1/visionai_data_format/exceptions/visionai.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-03-19 10:01:37.766348 visionai-data-format-1.3.1/visionai_data_format/schemas/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai-data-format-1.3.1/visionai_data_format/schemas/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     2586 2023-12-21 03:02:35.000000 visionai-data-format-1.3.1/visionai_data_format/schemas/bdd_schema.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      679 2023-12-21 03:02:35.000000 visionai-data-format-1.3.1/visionai_data_format/schemas/coco_schema.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1727 2024-02-06 03:21:26.000000 visionai-data-format-1.3.1/visionai_data_format/schemas/common.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      994 2023-12-21 03:02:35.000000 visionai-data-format-1.3.1/visionai_data_format/schemas/ontology.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-03-19 10:01:37.766911 visionai-data-format-1.3.1/visionai_data_format/schemas/utils/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai-data-format-1.3.1/visionai_data_format/schemas/utils/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    50408 2024-02-06 03:21:26.000000 visionai-data-format-1.3.1/visionai_data_format/schemas/utils/validators.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    32093 2024-02-06 03:21:26.000000 visionai-data-format-1.3.1/visionai_data_format/schemas/visionai_schema.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-03-19 10:01:37.768261 visionai-data-format-1.3.1/visionai_data_format/utils/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai-data-format-1.3.1/visionai_data_format/utils/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1692 2023-12-21 03:02:35.000000 visionai-data-format-1.3.1/visionai_data_format/utils/calculation.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    10506 2023-12-21 03:02:35.000000 visionai-data-format-1.3.1/visionai_data_format/utils/checker.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      761 2023-12-21 03:02:35.000000 visionai-data-format-1.3.1/visionai_data_format/utils/classes.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      585 2023-12-21 03:02:35.000000 visionai-data-format-1.3.1/visionai_data_format/utils/common.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     4571 2023-12-21 03:02:35.000000 visionai-data-format-1.3.1/visionai_data_format/utils/converter.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     4059 2023-12-21 03:02:35.000000 visionai-data-format-1.3.1/visionai_data_format/utils/resize.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     4588 2023-12-21 03:02:35.000000 visionai-data-format-1.3.1/visionai_data_format/utils/validator.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     2308 2023-12-21 03:02:35.000000 visionai-data-format-1.3.1/visionai_data_format/vai_to_bdd.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     5917 2023-07-06 06:50:32.000000 visionai-data-format-1.3.1/visionai_data_format/vai_to_bdd_v2.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-03-19 10:01:37.768477 visionai-data-format-1.3.1/visionai_data_format.egg-info/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    23694 2024-03-19 10:01:37.000000 visionai-data-format-1.3.1/visionai_data_format.egg-info/PKG-INFO
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1548 2024-03-19 10:01:37.000000 visionai-data-format-1.3.1/visionai_data_format.egg-info/SOURCES.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        1 2024-03-19 10:01:37.000000 visionai-data-format-1.3.1/visionai_data_format.egg-info/dependency_links.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       45 2024-03-19 10:01:37.000000 visionai-data-format-1.3.1/visionai_data_format.egg-info/requires.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       21 2024-03-19 10:01:37.000000 visionai-data-format-1.3.1/visionai_data_format.egg-info/top_level.txt
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-04-16 08:41:44.305475 visionai_data_format-1.3.2/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    23694 2024-04-16 08:41:44.305170 visionai_data_format-1.3.2/PKG-INFO
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    23316 2024-03-19 09:51:26.000000 visionai_data_format-1.3.2/README.md
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       38 2024-04-16 08:41:44.305540 visionai_data_format-1.3.2/setup.cfg
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      753 2024-04-16 08:33:06.000000 visionai_data_format-1.3.2/setup.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-04-16 08:41:44.295613 visionai_data_format-1.3.2/tests/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     2176 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/tests/test_schemas.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     8449 2024-02-06 03:21:26.000000 visionai_data_format-1.3.2/tests/test_validators.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-04-16 08:41:44.296661 visionai_data_format-1.3.2/visionai_data_format/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     6751 2024-03-19 09:51:26.000000 visionai_data_format-1.3.2/visionai_data_format/convert_dataset.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-04-16 08:41:44.299739 visionai_data_format-1.3.2/visionai_data_format/converters/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      173 2024-03-19 09:51:26.000000 visionai_data_format-1.3.2/visionai_data_format/converters/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1729 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/converters/base.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    16423 2024-03-19 09:51:26.000000 visionai_data_format-1.3.2/visionai_data_format/converters/bdd_to_vai.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     9363 2024-03-19 09:51:26.000000 visionai_data_format-1.3.2/visionai_data_format/converters/coco_to_vai.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    16685 2024-03-19 08:30:06.000000 visionai_data_format-1.3.2/visionai_data_format/converters/kitti_to_vai.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     9675 2024-03-19 09:51:26.000000 visionai_data_format-1.3.2/visionai_data_format/converters/vai_to_coco.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-04-16 08:41:44.300718 visionai_data_format-1.3.2/visionai_data_format/exceptions/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      156 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/exceptions/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1405 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/exceptions/constants.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     5564 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/exceptions/error_messages.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1322 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/exceptions/visionai.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-04-16 08:41:44.301902 visionai_data_format-1.3.2/visionai_data_format/schemas/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/schemas/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     2586 2024-04-16 07:37:46.000000 visionai_data_format-1.3.2/visionai_data_format/schemas/bdd_schema.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      679 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/schemas/coco_schema.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1727 2024-02-06 03:21:26.000000 visionai_data_format-1.3.2/visionai_data_format/schemas/common.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      994 2024-04-16 08:33:06.000000 visionai_data_format-1.3.2/visionai_data_format/schemas/ontology.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-04-16 08:41:44.302461 visionai_data_format-1.3.2/visionai_data_format/schemas/utils/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/schemas/utils/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    50408 2024-04-16 07:40:00.000000 visionai_data_format-1.3.2/visionai_data_format/schemas/utils/validators.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    32093 2024-04-16 08:33:06.000000 visionai_data_format-1.3.2/visionai_data_format/schemas/visionai_schema.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-04-16 08:41:44.304303 visionai_data_format-1.3.2/visionai_data_format/utils/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/utils/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1692 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/utils/calculation.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    10506 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/utils/checker.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      761 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/utils/classes.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      585 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/utils/common.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     4571 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/utils/converter.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     4059 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/utils/resize.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     4588 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/utils/validator.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     2308 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/vai_to_bdd.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     5917 2023-07-06 06:50:32.000000 visionai_data_format-1.3.2/visionai_data_format/vai_to_bdd_v2.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-04-16 08:41:44.304560 visionai_data_format-1.3.2/visionai_data_format.egg-info/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    23694 2024-04-16 08:41:44.000000 visionai_data_format-1.3.2/visionai_data_format.egg-info/PKG-INFO
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1548 2024-04-16 08:41:44.000000 visionai_data_format-1.3.2/visionai_data_format.egg-info/SOURCES.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        1 2024-04-16 08:41:44.000000 visionai_data_format-1.3.2/visionai_data_format.egg-info/dependency_links.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       45 2024-04-16 08:41:44.000000 visionai_data_format-1.3.2/visionai_data_format.egg-info/requires.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       21 2024-04-16 08:41:44.000000 visionai_data_format-1.3.2/visionai_data_format.egg-info/top_level.txt
```

### Comparing `visionai-data-format-1.3.1/PKG-INFO` & `visionai_data_format-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visionai-data-format
-Version: 1.3.1
+Version: 1.3.2
 Summary: converter tool for visionai format
 Home-page: 
 Author: LinkerVision
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic==1.*
 Provides-Extra: test
```

### Comparing `visionai-data-format-1.3.1/README.md` & `visionai_data_format-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/tests/test_schemas.py` & `visionai_data_format-1.3.2/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/tests/test_validators.py` & `visionai_data_format-1.3.2/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/visionai_data_format/convert_dataset.py` & `visionai_data_format-1.3.2/visionai_data_format/convert_dataset.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/visionai_data_format/converters/base.py` & `visionai_data_format-1.3.2/visionai_data_format/converters/base.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/visionai_data_format/converters/bdd_to_vai.py` & `visionai_data_format-1.3.2/visionai_data_format/converters/bdd_to_vai.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/visionai_data_format/converters/coco_to_vai.py` & `visionai_data_format-1.3.2/visionai_data_format/converters/coco_to_vai.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/visionai_data_format/converters/kitti_to_vai.py` & `visionai_data_format-1.3.2/visionai_data_format/converters/kitti_to_vai.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/visionai_data_format/converters/vai_to_coco.py` & `visionai_data_format-1.3.2/visionai_data_format/converters/vai_to_coco.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/visionai_data_format/exceptions/constants.py` & `visionai_data_format-1.3.2/visionai_data_format/exceptions/constants.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/visionai_data_format/exceptions/error_messages.py` & `visionai_data_format-1.3.2/visionai_data_format/exceptions/error_messages.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/visionai_data_format/exceptions/visionai.py` & `visionai_data_format-1.3.2/visionai_data_format/exceptions/visionai.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/visionai_data_format/schemas/bdd_schema.py` & `visionai_data_format-1.3.2/visionai_data_format/schemas/bdd_schema.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/visionai_data_format/schemas/coco_schema.py` & `visionai_data_format-1.3.2/visionai_data_format/schemas/coco_schema.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/visionai_data_format/schemas/common.py` & `visionai_data_format-1.3.2/visionai_data_format/schemas/common.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/visionai_data_format/schemas/ontology.py` & `visionai_data_format-1.3.2/visionai_data_format/schemas/ontology.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     VEC = "vec"
     TEXT = "text"
     BINARY = "binary"
 
 
 class Attribute(BaseModel):
     type: AttributeType
-    value: Optional[List[Union[float, str, int]]] = None
+    value: Optional[List[Union[str, int, float]]] = None
 
     class Config:
         use_enum_values = True
 
 
 class OntologyInfo(BaseModel):
     attributes: Dict[StrictStr, Attribute] = None
```

### Comparing `visionai-data-format-1.3.1/visionai_data_format/schemas/utils/validators.py` & `visionai_data_format-1.3.2/visionai_data_format/schemas/utils/validators.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/visionai_data_format/schemas/visionai_schema.py` & `visionai_data_format-1.3.2/visionai_data_format/schemas/visionai_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,15 +287,15 @@
 class VecBaseNoName(ExcludedNoneBaseModel):
     attributes: Optional[Attributes] = None
     type: Optional[TypeRange] = Field(
         None,
         description="This attribute specifies whether the vector shall be"
         + " considered as a descriptor of individual values or as a definition of a range.",
     )
-    val: List[Union[float, int, str]] = Field(
+    val: List[Union[str, int, float]] = Field(
         ..., description="The values of the vector (list)."
     )
 
     class Config:
         use_enum_values = True
         extra = Extra.forbid
```

### Comparing `visionai-data-format-1.3.1/visionai_data_format/utils/calculation.py` & `visionai_data_format-1.3.2/visionai_data_format/utils/calculation.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/visionai_data_format/utils/checker.py` & `visionai_data_format-1.3.2/visionai_data_format/utils/checker.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/visionai_data_format/utils/classes.py` & `visionai_data_format-1.3.2/visionai_data_format/utils/classes.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/visionai_data_format/utils/common.py` & `visionai_data_format-1.3.2/visionai_data_format/utils/common.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/visionai_data_format/utils/converter.py` & `visionai_data_format-1.3.2/visionai_data_format/utils/converter.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/visionai_data_format/utils/resize.py` & `visionai_data_format-1.3.2/visionai_data_format/utils/resize.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/visionai_data_format/utils/validator.py` & `visionai_data_format-1.3.2/visionai_data_format/utils/validator.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/visionai_data_format/vai_to_bdd.py` & `visionai_data_format-1.3.2/visionai_data_format/vai_to_bdd.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/visionai_data_format/vai_to_bdd_v2.py` & `visionai_data_format-1.3.2/visionai_data_format/vai_to_bdd_v2.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.3.1/visionai_data_format.egg-info/PKG-INFO` & `visionai_data_format-1.3.2/visionai_data_format.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visionai-data-format
-Version: 1.3.1
+Version: 1.3.2
 Summary: converter tool for visionai format
 Home-page: 
 Author: LinkerVision
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic==1.*
 Provides-Extra: test
```

### Comparing `visionai-data-format-1.3.1/visionai_data_format.egg-info/SOURCES.txt` & `visionai_data_format-1.3.2/visionai_data_format.egg-info/SOURCES.txt`

 * *Files identical despite different names*

