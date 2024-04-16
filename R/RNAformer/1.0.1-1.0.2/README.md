# Comparing `tmp/rnaformer-1.0.1.tar.gz` & `tmp/rnaformer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rnaformer-1.0.1.tar", last modified: Tue Apr 16 12:51:14 2024, max compression
+gzip compressed data, was "rnaformer-1.0.2.tar", last modified: Tue Apr 16 14:21:52 2024, max compression
```

## Comparing `rnaformer-1.0.1.tar` & `rnaformer-1.0.2.tar`

### file list

```diff
@@ -1,47 +1,12 @@
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-16 12:51:14.568684 rnaformer-1.0.1/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)    11347 2024-04-10 11:44:16.000000 rnaformer-1.0.1/LICENSE
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     4970 2024-04-16 12:51:14.568684 rnaformer-1.0.1/PKG-INFO
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     4381 2024-04-10 11:44:16.000000 rnaformer-1.0.1/README.md
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-16 12:51:14.564684 rnaformer-1.0.1/RNAformer/
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-16 12:51:14.564684 rnaformer-1.0.1/RNAformer/model/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3594 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/model/RNAformer.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     2020 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/model/RNAformer_block.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)      755 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/model/RNAformer_stack.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/model/__init__.py
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-16 12:51:14.564684 rnaformer-1.0.1/RNAformer/module/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/module/__init__.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)    13311 2024-04-15 21:52:05.000000 rnaformer-1.0.1/RNAformer/module/axial_attention.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)      940 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/module/axial_dropout.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3788 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/module/embedding.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3371 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/module/feed_forward.py
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-16 12:51:14.564684 rnaformer-1.0.1/RNAformer/pl_module/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/pl_module/__init__.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)    11243 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/pl_module/datamodule_rna.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     9104 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/pl_module/rna_folding_trainer.py
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-16 12:51:14.568684 rnaformer-1.0.1/RNAformer/rnaformer.egg-info/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     4970 2024-04-16 12:51:14.000000 rnaformer-1.0.1/RNAformer/rnaformer.egg-info/PKG-INFO
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     1119 2024-04-16 12:51:14.000000 rnaformer-1.0.1/RNAformer/rnaformer.egg-info/SOURCES.txt
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        1 2024-04-16 12:51:14.000000 rnaformer-1.0.1/RNAformer/rnaformer.egg-info/dependency_links.txt
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)       29 2024-04-16 12:51:14.000000 rnaformer-1.0.1/RNAformer/rnaformer.egg-info/top_level.txt
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-16 12:51:14.568684 rnaformer-1.0.1/RNAformer/utils/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)      164 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/utils/__init__.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     4062 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/utils/configuration.py
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-16 12:51:14.568684 rnaformer-1.0.1/RNAformer/utils/data/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/utils/data/__init__.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     5800 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/utils/data/rna.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     6566 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/utils/eval_predictions.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)      890 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/utils/folder_manager.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3656 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/utils/group_parameters.py
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-16 12:51:14.568684 rnaformer-1.0.1/RNAformer/utils/handler/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/utils/handler/__init__.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     2145 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/utils/handler/base_handler.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3478 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/utils/handler/checkpoint.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     1480 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/utils/handler/folder.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     2461 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/utils/instantiate.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3780 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/utils/logger.py
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-16 12:51:14.568684 rnaformer-1.0.1/RNAformer/utils/optim/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/utils/optim/__init__.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     1067 2024-04-10 11:44:16.000000 rnaformer-1.0.1/RNAformer/utils/optim/lr_schedule.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)      626 2024-04-16 12:50:40.000000 rnaformer-1.0.1/pyproject.toml
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)       38 2024-04-16 12:51:14.568684 rnaformer-1.0.1/setup.cfg
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)      278 2024-04-16 12:51:05.000000 rnaformer-1.0.1/setup.py
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-16 14:21:52.823467 rnaformer-1.0.2/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)    11347 2024-04-10 11:44:16.000000 rnaformer-1.0.2/LICENSE
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     4970 2024-04-16 14:21:52.823467 rnaformer-1.0.2/PKG-INFO
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     4381 2024-04-10 11:44:16.000000 rnaformer-1.0.2/README.md
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)      626 2024-04-16 14:21:24.000000 rnaformer-1.0.2/pyproject.toml
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-16 14:21:52.823467 rnaformer-1.0.2/rnaformer.egg-info/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     4970 2024-04-16 14:21:52.000000 rnaformer-1.0.2/rnaformer.egg-info/PKG-INFO
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)      173 2024-04-16 14:21:52.000000 rnaformer-1.0.2/rnaformer.egg-info/SOURCES.txt
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)        1 2024-04-16 14:21:52.000000 rnaformer-1.0.2/rnaformer.egg-info/dependency_links.txt
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)        1 2024-04-16 14:21:52.000000 rnaformer-1.0.2/rnaformer.egg-info/top_level.txt
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)       38 2024-04-16 14:21:52.823467 rnaformer-1.0.2/setup.cfg
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)      253 2024-04-16 14:20:11.000000 rnaformer-1.0.2/setup.py
```

### Comparing `rnaformer-1.0.1/LICENSE` & `rnaformer-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rnaformer-1.0.1/PKG-INFO` & `rnaformer-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rnaformer
-Version: 1.0.1
+Version: 1.0.2
 Summary: RNAformer: a simple single-sequence-based deep learning model for RNA secondary structure prediction.
 Author: Frederic Runge, Rolf Backofen, Frank Hutter
 Author-email: "Joerg K.H. Franke" <frankej@cs.uni-freiburg.de>, Ryan Koeksal <koeksalr@informatik.uni-freiburg.de>
 Project-URL: Homepage, https://github.com/automl/RNAformer
 Project-URL: Issues, https://github.com/automl/RNAformer/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

### Comparing `rnaformer-1.0.1/README.md` & `rnaformer-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rnaformer-1.0.1/RNAformer/rnaformer.egg-info/PKG-INFO` & `rnaformer-1.0.2/rnaformer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rnaformer
-Version: 1.0.1
+Version: 1.0.2
 Summary: RNAformer: a simple single-sequence-based deep learning model for RNA secondary structure prediction.
 Author: Frederic Runge, Rolf Backofen, Frank Hutter
 Author-email: "Joerg K.H. Franke" <frankej@cs.uni-freiburg.de>, Ryan Koeksal <koeksalr@informatik.uni-freiburg.de>
 Project-URL: Homepage, https://github.com/automl/RNAformer
 Project-URL: Issues, https://github.com/automl/RNAformer/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

### Comparing `rnaformer-1.0.1/pyproject.toml` & `rnaformer-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rnaformer"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Joerg K.H. Franke", email="frankej@cs.uni-freiburg.de" },
   { name="Frederic Runge"},
   { name="Ryan Koeksal", email="koeksalr@informatik.uni-freiburg.de" },
   { name="Rolf Backofen"},
   { name="Frank Hutter"},
 ]
```

