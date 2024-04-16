# Comparing `tmp/quant2-0.1.2.tar.gz` & `tmp/quant2-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant2-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "quant2-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `quant2-0.1.2.tar` & `quant2-0.1.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      574 2024-04-06 14:41:03.615629 quant2-0.1.2/.gitignore
--rw-r--r--   0        0        0    11357 2024-03-20 11:12:02.832412 quant2-0.1.2/LICENSE
--rw-r--r--   0        0        0        7 2024-03-20 11:12:02.832412 quant2-0.1.2/README.md
--rw-r--r--   0        0        0      971 2024-04-14 08:14:34.409434 quant2-0.1.2/configs/stnetv3/stnetv3_table20240326_2201to2312.cfg
--rw-r--r--   0        0        0     1049 2024-04-12 08:57:23.226862 quant2-0.1.2/configs/stnetv4/stnetv4_table20240410_2201to2312.cfg
--rw-r--r--   0        0        0      664 2024-04-10 00:12:18.347578 quant2-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1841 2024-03-23 05:01:23.359992 quant2-0.1.2/quant/README.md
--rw-r--r--   0        0        0      559 2024-04-15 20:46:19.279693 quant2-0.1.2/quant/__init__.py
--rw-r--r--   0        0        0       67 2024-03-23 04:17:48.269987 quant2-0.1.2/quant/__main__.py
--rw-r--r--   0        0        0        0 2024-04-08 01:35:10.284089 quant2-0.1.2/quant/evaluate/__init__.py
--rw-r--r--   0        0        0     2646 2024-04-12 06:45:48.719809 quant2-0.1.2/quant/evaluate/table20240326.py
--rw-r--r--   0        0        0     2006 2024-04-12 04:48:31.980573 quant2-0.1.2/quant/evaluate/utils.py
--rw-r--r--   0        0        0      422 2024-03-23 04:21:50.819993 quant2-0.1.2/quant/football/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 14:09:03.305285 quant2-0.1.2/quant/football/data/__init__.py
--rw-r--r--   0        0        0     4348 2024-04-14 08:11:01.537268 quant2-0.1.2/quant/football/data/dataset.py
--rw-r--r--   0        0        0        0 2024-04-08 10:24:35.916611 quant2-0.1.2/quant/football/data/functional.py
--rw-r--r--   0        0        0     1336 2024-04-15 11:24:33.080117 quant2-0.1.2/quant/football/data/preprocessing.py
--rw-r--r--   0        0        0        0 2024-04-08 11:08:36.928001 quant2-0.1.2/quant/football/data/stats.py
--rw-r--r--   0        0        0     4560 2024-04-13 08:19:58.059662 quant2-0.1.2/quant/football/data/utils.py
--rw-r--r--   0        0        0        0 2024-04-11 16:55:37.649284 quant2-0.1.2/quant/football/infer/__init__.py
--rw-r--r--   0        0        0     1537 2024-04-11 17:24:14.938089 quant2-0.1.2/quant/football/infer/fastapi_app.py
--rw-r--r--   0        0        0      468 2024-04-11 16:55:50.160241 quant2-0.1.2/quant/football/infer/fastapi_app_test.py
--rw-r--r--   0        0        0     7798 2024-04-15 11:06:59.301368 quant2-0.1.2/quant/football/infer/football_infer_overunder_v1.py
--rw-r--r--   0        0        0      473 2024-04-11 16:56:07.430215 quant2-0.1.2/quant/football/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 04:22:28.629548 quant2-0.1.2/quant/football/models/mtnet.py
--rw-r--r--   0        0        0     6110 2024-04-11 17:12:37.365849 quant2-0.1.2/quant/football/models/stnet.py
--rw-r--r--   0        0        0      379 2024-04-14 08:54:29.067337 quant2-0.1.2/quant/football/transforms/__init__.py
--rw-r--r--   0        0        0     6592 2024-04-14 08:09:52.271038 quant2-0.1.2/quant/football/transforms/table20240326.py
--rw-r--r--   0        0        0     8511 2024-04-14 08:07:38.143730 quant2-0.1.2/quant/football/transforms/table20240410.py
--rw-r--r--   0        0        0     8795 2024-04-15 14:39:32.419111 quant2-0.1.2/quant/football/transforms/table20240414.py
--rw-r--r--   0        0        0     8336 2024-04-15 20:50:57.893655 quant2-0.1.2/quant/football/transforms/table20240415.py
--rw-r--r--   0        0        0        0 2024-03-31 10:26:04.538951 quant2-0.1.2/quant/layers/__init__.py
--rw-r--r--   0        0        0      483 2024-03-28 09:12:19.609652 quant2-0.1.2/quant/layers/layer_scale.py
--rw-r--r--   0        0        0     1070 2024-03-28 09:13:06.741829 quant2-0.1.2/quant/layers/mlp.py
--rw-r--r--   0        0        0     1314 2024-03-28 09:40:33.643889 quant2-0.1.2/quant/layers/normalization.py
--rw-r--r--   0        0        0      852 2024-03-28 09:16:09.540017 quant2-0.1.2/quant/layers/swiglu_ffn.py
--rw-r--r--   0        0        0        0 2024-04-03 13:03:10.745509 quant2-0.1.2/quant/utils/__init__.py
--rw-r--r--   0        0        0     1695 2024-04-11 16:56:25.721657 quant2-0.1.2/quant/utils/archive.py
--rw-r--r--   0        0        0     1884 2024-04-14 08:14:07.935771 quant2-0.1.2/quant/utils/config.py
--rw-r--r--   0        0        0     1047 2024-04-09 01:40:57.919653 quant2-0.1.2/quant/utils/io.py
--rw-r--r--   0        0        0     1006 2024-04-03 13:19:59.255567 quant2-0.1.2/quant/utils/logging.py
--rw-r--r--   0        0        0      182 2024-03-28 01:09:02.081511 quant2-0.1.2/tests/football/data/test_utils.py
--rw-r--r--   0        0        0     1632 2024-04-12 06:45:57.389803 quant2-0.1.2/tools/analysis_tools/analyze_cls_results.py
--rw-r--r--   0        0        0     2632 2024-04-15 16:14:46.557801 quant2-0.1.2/tools/experimental/make_dataset.py
--rw-r--r--   0        0        0     1580 2024-04-13 14:41:36.176420 quant2-0.1.2/tools/experimental/make_split.py
--rw-r--r--   0        0        0     6485 2024-04-15 11:07:06.081414 quant2-0.1.2/tools/experimental/nni_football.py
--rw-r--r--   0        0        0      476 2024-04-15 19:50:59.765841 quant2-0.1.2/tools/experimental/nni_football_config.yaml
--rw-r--r--   0        0        0     1556 2024-04-15 20:08:48.206604 quant2-0.1.2/tools/experimental/nni_football_config_search_space.json
--rw-r--r--   0        0        0      523 2024-04-14 02:37:47.884925 quant2-0.1.2/tools/experimental/nni_model.py
--rw-r--r--   0        0        0      441 2024-04-14 04:00:22.459245 quant2-0.1.2/tools/experimental/nni_model_config.yaml
--rw-r--r--   0        0        0     2855 2024-04-15 11:07:14.941468 quant2-0.1.2/tools/fb_cls_test.py
--rw-r--r--   0        0        0     6353 2024-04-15 11:07:20.811492 quant2-0.1.2/tools/fb_cls_train.py
--rw-r--r--   0        0        0     2187 1970-01-01 00:00:00.000000 quant2-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      574 2024-04-06 14:41:03.615629 quant2-0.1.3/.gitignore
+-rw-r--r--   0        0        0    11357 2024-03-20 11:12:02.832412 quant2-0.1.3/LICENSE
+-rw-r--r--   0        0        0        7 2024-03-20 11:12:02.832412 quant2-0.1.3/README.md
+-rw-r--r--   0        0        0      971 2024-04-14 08:14:34.409434 quant2-0.1.3/configs/stnetv3/stnetv3_table20240326_2201to2312.cfg
+-rw-r--r--   0        0        0     1049 2024-04-12 08:57:23.226862 quant2-0.1.3/configs/stnetv4/stnetv4_table20240410_2201to2312.cfg
+-rw-r--r--   0        0        0      664 2024-04-10 00:12:18.347578 quant2-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1841 2024-03-23 05:01:23.359992 quant2-0.1.3/quant/README.md
+-rw-r--r--   0        0        0      559 2024-04-15 21:05:06.872661 quant2-0.1.3/quant/__init__.py
+-rw-r--r--   0        0        0       67 2024-03-23 04:17:48.269987 quant2-0.1.3/quant/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-08 01:35:10.284089 quant2-0.1.3/quant/evaluate/__init__.py
+-rw-r--r--   0        0        0     2646 2024-04-12 06:45:48.719809 quant2-0.1.3/quant/evaluate/table20240326.py
+-rw-r--r--   0        0        0     2006 2024-04-12 04:48:31.980573 quant2-0.1.3/quant/evaluate/utils.py
+-rw-r--r--   0        0        0      422 2024-03-23 04:21:50.819993 quant2-0.1.3/quant/football/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 14:09:03.305285 quant2-0.1.3/quant/football/data/__init__.py
+-rw-r--r--   0        0        0     4348 2024-04-14 08:11:01.537268 quant2-0.1.3/quant/football/data/dataset.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:24:35.916611 quant2-0.1.3/quant/football/data/functional.py
+-rw-r--r--   0        0        0     1336 2024-04-15 11:24:33.080117 quant2-0.1.3/quant/football/data/preprocessing.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:08:36.928001 quant2-0.1.3/quant/football/data/stats.py
+-rw-r--r--   0        0        0     4560 2024-04-13 08:19:58.059662 quant2-0.1.3/quant/football/data/utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 16:55:37.649284 quant2-0.1.3/quant/football/infer/__init__.py
+-rw-r--r--   0        0        0     1537 2024-04-11 17:24:14.938089 quant2-0.1.3/quant/football/infer/fastapi_app.py
+-rw-r--r--   0        0        0      468 2024-04-11 16:55:50.160241 quant2-0.1.3/quant/football/infer/fastapi_app_test.py
+-rw-r--r--   0        0        0     7798 2024-04-15 11:06:59.301368 quant2-0.1.3/quant/football/infer/football_infer_overunder_v1.py
+-rw-r--r--   0        0        0      473 2024-04-11 16:56:07.430215 quant2-0.1.3/quant/football/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 04:22:28.629548 quant2-0.1.3/quant/football/models/mtnet.py
+-rw-r--r--   0        0        0     6110 2024-04-11 17:12:37.365849 quant2-0.1.3/quant/football/models/stnet.py
+-rw-r--r--   0        0        0      463 2024-04-15 20:54:36.028514 quant2-0.1.3/quant/football/transforms/__init__.py
+-rw-r--r--   0        0        0     6592 2024-04-14 08:09:52.271038 quant2-0.1.3/quant/football/transforms/table20240326.py
+-rw-r--r--   0        0        0     8511 2024-04-14 08:07:38.143730 quant2-0.1.3/quant/football/transforms/table20240410.py
+-rw-r--r--   0        0        0     8795 2024-04-15 14:39:32.419111 quant2-0.1.3/quant/football/transforms/table20240414.py
+-rw-r--r--   0        0        0     8336 2024-04-15 20:50:57.893655 quant2-0.1.3/quant/football/transforms/table20240415.py
+-rw-r--r--   0        0        0        0 2024-03-31 10:26:04.538951 quant2-0.1.3/quant/layers/__init__.py
+-rw-r--r--   0        0        0      483 2024-03-28 09:12:19.609652 quant2-0.1.3/quant/layers/layer_scale.py
+-rw-r--r--   0        0        0     1070 2024-03-28 09:13:06.741829 quant2-0.1.3/quant/layers/mlp.py
+-rw-r--r--   0        0        0     1314 2024-03-28 09:40:33.643889 quant2-0.1.3/quant/layers/normalization.py
+-rw-r--r--   0        0        0      852 2024-03-28 09:16:09.540017 quant2-0.1.3/quant/layers/swiglu_ffn.py
+-rw-r--r--   0        0        0        0 2024-04-03 13:03:10.745509 quant2-0.1.3/quant/utils/__init__.py
+-rw-r--r--   0        0        0     1695 2024-04-11 16:56:25.721657 quant2-0.1.3/quant/utils/archive.py
+-rw-r--r--   0        0        0     1884 2024-04-14 08:14:07.935771 quant2-0.1.3/quant/utils/config.py
+-rw-r--r--   0        0        0     1047 2024-04-09 01:40:57.919653 quant2-0.1.3/quant/utils/io.py
+-rw-r--r--   0        0        0     1006 2024-04-03 13:19:59.255567 quant2-0.1.3/quant/utils/logging.py
+-rw-r--r--   0        0        0      182 2024-03-28 01:09:02.081511 quant2-0.1.3/tests/football/data/test_utils.py
+-rw-r--r--   0        0        0     1632 2024-04-12 06:45:57.389803 quant2-0.1.3/tools/analysis_tools/analyze_cls_results.py
+-rw-r--r--   0        0        0     2632 2024-04-15 16:14:46.557801 quant2-0.1.3/tools/experimental/make_dataset.py
+-rw-r--r--   0        0        0     1580 2024-04-13 14:41:36.176420 quant2-0.1.3/tools/experimental/make_split.py
+-rw-r--r--   0        0        0     6485 2024-04-15 11:07:06.081414 quant2-0.1.3/tools/experimental/nni_football.py
+-rw-r--r--   0        0        0      476 2024-04-15 19:50:59.765841 quant2-0.1.3/tools/experimental/nni_football_config.yaml
+-rw-r--r--   0        0        0     1556 2024-04-15 20:08:48.206604 quant2-0.1.3/tools/experimental/nni_football_config_search_space.json
+-rw-r--r--   0        0        0      523 2024-04-14 02:37:47.884925 quant2-0.1.3/tools/experimental/nni_model.py
+-rw-r--r--   0        0        0      441 2024-04-14 04:00:22.459245 quant2-0.1.3/tools/experimental/nni_model_config.yaml
+-rw-r--r--   0        0        0     2855 2024-04-15 11:07:14.941468 quant2-0.1.3/tools/fb_cls_test.py
+-rw-r--r--   0        0        0     6353 2024-04-15 11:07:20.811492 quant2-0.1.3/tools/fb_cls_train.py
+-rw-r--r--   0        0        0     2187 1970-01-01 00:00:00.000000 quant2-0.1.3/PKG-INFO
```

### Comparing `quant2-0.1.2/.gitignore` & `quant2-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/LICENSE` & `quant2-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/configs/stnetv3/stnetv3_table20240326_2201to2312.cfg` & `quant2-0.1.3/configs/stnetv3/stnetv3_table20240326_2201to2312.cfg`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/configs/stnetv4/stnetv4_table20240410_2201to2312.cfg` & `quant2-0.1.3/configs/stnetv4/stnetv4_table20240410_2201to2312.cfg`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/pyproject.toml` & `quant2-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/quant/README.md` & `quant2-0.1.3/quant/README.md`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/quant/__init__.py` & `quant2-0.1.3/quant/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A collection of useful tools!"""
 import sys
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 help_doc_str = """\
 usage: quant [--version] [--help]
 
 shell command:
     quant -h
```

### Comparing `quant2-0.1.2/quant/evaluate/table20240326.py` & `quant2-0.1.3/quant/evaluate/table20240326.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/quant/evaluate/utils.py` & `quant2-0.1.3/quant/evaluate/utils.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/quant/football/data/dataset.py` & `quant2-0.1.3/quant/football/data/dataset.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/quant/football/data/preprocessing.py` & `quant2-0.1.3/quant/football/data/preprocessing.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/quant/football/data/utils.py` & `quant2-0.1.3/quant/football/data/utils.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/quant/football/infer/fastapi_app.py` & `quant2-0.1.3/quant/football/infer/fastapi_app.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/quant/football/infer/football_infer_overunder_v1.py` & `quant2-0.1.3/quant/football/infer/football_infer_overunder_v1.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/quant/football/models/stnet.py` & `quant2-0.1.3/quant/football/models/stnet.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/quant/football/transforms/table20240326.py` & `quant2-0.1.3/quant/football/transforms/table20240326.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/quant/football/transforms/table20240410.py` & `quant2-0.1.3/quant/football/transforms/table20240410.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/quant/football/transforms/table20240414.py` & `quant2-0.1.3/quant/football/transforms/table20240414.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/quant/football/transforms/table20240415.py` & `quant2-0.1.3/quant/football/transforms/table20240415.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/quant/layers/mlp.py` & `quant2-0.1.3/quant/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/quant/layers/normalization.py` & `quant2-0.1.3/quant/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/quant/layers/swiglu_ffn.py` & `quant2-0.1.3/quant/layers/swiglu_ffn.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/quant/utils/archive.py` & `quant2-0.1.3/quant/utils/archive.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/quant/utils/config.py` & `quant2-0.1.3/quant/utils/config.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/quant/utils/io.py` & `quant2-0.1.3/quant/utils/io.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/quant/utils/logging.py` & `quant2-0.1.3/quant/utils/logging.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/tools/analysis_tools/analyze_cls_results.py` & `quant2-0.1.3/tools/analysis_tools/analyze_cls_results.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/tools/experimental/make_dataset.py` & `quant2-0.1.3/tools/experimental/make_dataset.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/tools/experimental/make_split.py` & `quant2-0.1.3/tools/experimental/make_split.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/tools/experimental/nni_football.py` & `quant2-0.1.3/tools/experimental/nni_football.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/tools/experimental/nni_football_config_search_space.json` & `quant2-0.1.3/tools/experimental/nni_football_config_search_space.json`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/tools/experimental/nni_model.py` & `quant2-0.1.3/tools/experimental/nni_model.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/tools/fb_cls_test.py` & `quant2-0.1.3/tools/fb_cls_test.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/tools/fb_cls_train.py` & `quant2-0.1.3/tools/fb_cls_train.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.2/PKG-INFO` & `quant2-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant2
-Version: 0.1.2
+Version: 0.1.3
 Summary: A collection of useful tools!
 Author-email: Hejian <flystarhe@qq.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: prettytable
 Requires-Dist: scikit-learn
```

