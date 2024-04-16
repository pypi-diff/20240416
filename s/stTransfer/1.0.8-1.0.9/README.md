# Comparing `tmp/stTransfer-1.0.8.tar.gz` & `tmp/stTransfer-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stTransfer-1.0.8.tar", last modified: Fri Apr  5 17:10:23 2024, max compression
+gzip compressed data, was "stTransfer-1.0.9.tar", last modified: Mon Apr  8 09:28:32 2024, max compression
```

## Comparing `stTransfer-1.0.8.tar` & `stTransfer-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 zhoutao3 (29897) huadjyin (32795)        0 2024-04-05 17:09:11.721522 stTransfer-1.0.8/
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     1065 2024-02-28 07:25:00.000000 stTransfer-1.0.8/LICENSE
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     2291 2024-04-05 17:10:23.688504 stTransfer-1.0.8/PKG-INFO
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     1813 2024-02-29 10:01:56.000000 stTransfer-1.0.8/README.md
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)      160 2024-04-05 17:10:23.696684 stTransfer-1.0.8/setup.cfg
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     1165 2024-04-05 17:08:28.000000 stTransfer-1.0.8/setup.py
-drwxr-xr-x   0 zhoutao3 (29897) huadjyin (32795)        0 2024-04-05 17:09:11.662553 stTransfer-1.0.8/stTransfer/
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)       80 2024-02-28 08:07:48.000000 stTransfer-1.0.8/stTransfer/__init__.py
-drwxr-xr-x   0 zhoutao3 (29897) huadjyin (32795)        0 2024-04-05 17:09:11.712660 stTransfer-1.0.8/stTransfer/stTransfer/
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     7748 2024-03-14 05:57:47.000000 stTransfer-1.0.8/stTransfer/stTransfer/Transfer_entry.py
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)      179 2024-02-23 04:34:51.000000 stTransfer-1.0.8/stTransfer/stTransfer/__init__.py
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     8972 2024-04-05 16:04:49.000000 stTransfer-1.0.8/stTransfer/stTransfer/cell_type_ann_model.py
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     8599 2024-03-28 06:20:45.000000 stTransfer-1.0.8/stTransfer/stTransfer/scTrain_entry.py
-drwxr-xr-x   0 zhoutao3 (29897) huadjyin (32795)        0 2024-04-05 17:09:11.686704 stTransfer-1.0.8/stTransfer.egg-info/
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     2291 2024-04-05 17:10:23.000000 stTransfer-1.0.8/stTransfer.egg-info/PKG-INFO
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)      353 2024-04-05 17:10:23.000000 stTransfer-1.0.8/stTransfer.egg-info/SOURCES.txt
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)        1 2024-04-05 17:10:23.000000 stTransfer-1.0.8/stTransfer.egg-info/dependency_links.txt
--rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)       11 2024-04-05 17:10:23.000000 stTransfer-1.0.8/stTransfer.egg-info/top_level.txt
+drwxr-xr-x   0 zhoutao3 (29897) huadjyin (32795)        0 2024-04-08 09:27:19.254207 stTransfer-1.0.9/
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     1065 2024-02-28 07:25:00.000000 stTransfer-1.0.9/LICENSE
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     2817 2024-04-08 09:28:32.857003 stTransfer-1.0.9/PKG-INFO
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     1813 2024-02-29 10:01:56.000000 stTransfer-1.0.9/README.md
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)      160 2024-04-08 09:28:32.865260 stTransfer-1.0.9/setup.cfg
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     1632 2024-04-08 09:27:14.000000 stTransfer-1.0.9/setup.py
+drwxr-xr-x   0 zhoutao3 (29897) huadjyin (32795)        0 2024-04-08 09:27:19.197343 stTransfer-1.0.9/stTransfer/
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)       80 2024-02-28 08:07:48.000000 stTransfer-1.0.9/stTransfer/__init__.py
+drwxr-xr-x   0 zhoutao3 (29897) huadjyin (32795)        0 2024-04-08 09:27:19.245421 stTransfer-1.0.9/stTransfer/stTransfer/
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     7748 2024-03-14 05:57:47.000000 stTransfer-1.0.9/stTransfer/stTransfer/Transfer_entry.py
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)      179 2024-02-23 04:34:51.000000 stTransfer-1.0.9/stTransfer/stTransfer/__init__.py
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     8972 2024-04-05 16:04:49.000000 stTransfer-1.0.9/stTransfer/stTransfer/cell_type_ann_model.py
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     8599 2024-03-28 06:20:45.000000 stTransfer-1.0.9/stTransfer/stTransfer/scTrain_entry.py
+drwxr-xr-x   0 zhoutao3 (29897) huadjyin (32795)        0 2024-04-08 09:27:19.222082 stTransfer-1.0.9/stTransfer.egg-info/
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)     2817 2024-04-08 09:28:32.000000 stTransfer-1.0.9/stTransfer.egg-info/PKG-INFO
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)      386 2024-04-08 09:28:32.000000 stTransfer-1.0.9/stTransfer.egg-info/SOURCES.txt
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)        1 2024-04-08 09:28:32.000000 stTransfer-1.0.9/stTransfer.egg-info/dependency_links.txt
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)      286 2024-04-08 09:28:32.000000 stTransfer-1.0.9/stTransfer.egg-info/requires.txt
+-rw-r--r--   0 zhoutao3 (29897) huadjyin (32795)       11 2024-04-08 09:28:32.000000 stTransfer-1.0.9/stTransfer.egg-info/top_level.txt
```

### Comparing `stTransfer-1.0.8/LICENSE` & `stTransfer-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stTransfer-1.0.8/PKG-INFO` & `stTransfer-1.0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: stTransfer
-Version: 1.0.8
-Summary: Transfer learning for spatial transcriptomics data and single-cell RNA-seq data.
-Home-page: https://github.com/zepoch/stTransfer.git
-Author: zhoutao
-Author-email: zhotoa@foxmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # stTransfer
 
 [![python >= 3.8](https://img.shields.io/badge/python-3.8-brightgreen)](https://www.python.org/) 
 
 ### Installation      
 ```python
 pip install stTransfer
@@ -52,8 +38,8 @@
                           edge_weight=True, 
                           epochs=100, 
                           w_cls=50, 
                           w_dae=1., 
                           w_gae=1.,
                           gpu="0", 
                           save_path="/data/output") # output path
-```
+```
```

### Comparing `stTransfer-1.0.8/stTransfer/stTransfer/Transfer_entry.py` & `stTransfer-1.0.9/stTransfer/stTransfer/Transfer_entry.py`

 * *Files identical despite different names*

### Comparing `stTransfer-1.0.8/stTransfer/stTransfer/cell_type_ann_model.py` & `stTransfer-1.0.9/stTransfer/stTransfer/cell_type_ann_model.py`

 * *Files identical despite different names*

### Comparing `stTransfer-1.0.8/stTransfer/stTransfer/scTrain_entry.py` & `stTransfer-1.0.9/stTransfer/stTransfer/scTrain_entry.py`

 * *Files identical despite different names*

