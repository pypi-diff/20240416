# Comparing `tmp/datascope-experiments-0.0.81.tar.gz` & `tmp/datascope-experiments-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datascope-experiments-0.0.81.tar", last modified: Tue Apr 16 01:02:44 2024, max compression
+gzip compressed data, was "datascope-experiments-0.0.9.tar", last modified: Sat Jan  7 11:55:37 2023, max compression
```

## Comparing `datascope-experiments-0.0.81.tar` & `datascope-experiments-0.0.9.tar`

### file list

```diff
@@ -1,62 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:02:44.666211 datascope-experiments-0.0.81/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-16 01:02:44.666211 datascope-experiments-0.0.81/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:02:44.658211 datascope-experiments-0.0.81/datascope/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:02:44.658211 datascope-experiments-0.0.81/datascope/experiments/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:02:44.658211 datascope-experiments-0.0.81/datascope/experiments/baselines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/baselines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:02:44.658211 datascope-experiments-0.0.81/datascope/experiments/baselines/influence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/baselines/influence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/baselines/influence/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    33529 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/baselines/influence/genericNeuralNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/baselines/influence/hessians.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/baselines/influence/importance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/baselines/influence/logisticRegressionWithLBFGS.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:02:44.662211 datascope-experiments-0.0.81/datascope/experiments/baselines/matchingnet/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/baselines/matchingnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/baselines/matchingnet/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/baselines/matchingnet/few_shot_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/baselines/matchingnet/matchingnet_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/baselines/matchingnet/predesigned_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/baselines/matchingnet/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/baselines/matchingnet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:02:44.662211 datascope-experiments-0.0.81/datascope/experiments/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74781 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9655 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:02:44.662211 datascope-experiments-0.0.81/datascope/experiments/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21716 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/pipelines/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17287 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/pipelines/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/pipelines/postprocessors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/pipelines/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:02:44.662211 datascope-experiments-0.0.81/datascope/experiments/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48189 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/reports/aggregate_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:02:44.662211 datascope-experiments-0.0.81/datascope/experiments/scenarios/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/scenarios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48970 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/scenarios/base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6781 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/scenarios/compute_time.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26558 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/scenarios/data_discard.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16055 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/scenarios/datascope_scenario.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24365 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/scenarios/label_repair.py
--rw-r--r--   0 runner    (1001) docker     (127)     8795 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/scenarios/marginal_contribution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:02:44.662211 datascope-experiments-0.0.81/datascope/experiments/utility/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/utility/files.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/datascope/experiments/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:02:44.662211 datascope-experiments-0.0.81/datascope_experiments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-16 01:02:44.000000 datascope-experiments-0.0.81/datascope_experiments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-16 01:02:44.000000 datascope-experiments-0.0.81/datascope_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 01:02:44.000000 datascope-experiments-0.0.81/datascope_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-16 01:02:44.000000 datascope-experiments-0.0.81/datascope_experiments.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-16 01:02:44.000000 datascope-experiments-0.0.81/datascope_experiments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 01:02:44.000000 datascope-experiments-0.0.81/datascope_experiments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 01:02:44.666211 datascope-experiments-0.0.81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-16 01:01:45.000000 datascope-experiments-0.0.81/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.112194 datascope-experiments-0.0.9/datascope/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.112194 datascope-experiments-0.0.9/datascope/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/datascope/experiments/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42998 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/datascope/experiments/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/pipelines/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/pipelines/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/datascope/experiments/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36299 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/reports/aggregate_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/datascope/experiments/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46851 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/scenarios/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6636 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/scenarios/compute_time.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17443 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/scenarios/data_discard.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11559 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/scenarios/datascope_scenario.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18395 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/scenarios/label_repair.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/datascope_experiments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-01-07 11:55:37.000000 datascope-experiments-0.0.9/datascope_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-01-07 11:55:37.000000 datascope-experiments-0.0.9/datascope_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-07 11:55:37.000000 datascope-experiments-0.0.9/datascope_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-07 11:55:37.000000 datascope-experiments-0.0.9/datascope_experiments.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-07 11:55:37.000000 datascope-experiments-0.0.9/datascope_experiments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-07 11:55:37.000000 datascope-experiments-0.0.9/datascope_experiments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/setup.py
```

### Comparing `datascope-experiments-0.0.81/PKG-INFO` & `datascope-experiments-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datascope-experiments
-Version: 0.0.81
+Version: 0.0.9
 Summary: Module for running experiments on top of datascope.
 Home-page: https://ease.ml/datascope/
 Author-email: easeml@ds3lab.com
 License: MIT
 Description: # Experimental toolkit for ease.ml/datascope
         
         [![PyPI version](https://badge.fury.io/py/datascope-experiments.svg)](https://badge.fury.io/py/datascope-experiments)
```

### Comparing `datascope-experiments-0.0.81/datascope/experiments/datasets/__init__.py` & `datascope-experiments-0.0.9/datascope/experiments/datasets/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,42 @@
 from .base import (
     DatasetId,
     DatasetModality,
     Dataset,
-    TabularDatasetMixin,
-    ImageDatasetMixin,
-    TextDatasetMixin,
-    NoisyLabelDataset,
+    DirtyLabelDataset,
     BiasMethod,
     BiasedMixin,
-    BiasedNoisyLabelDataset,
-    AugmentableMixin,
+    BiasedDirtyLabelDataset,
     RandomDataset,
     UCI,
     FashionMNIST,
     TwentyNewsGroups,
-    Higgs,
-    DataPerfVision,
-    CifarN,
     DEFAULT_TRAINSIZE,
     DEFAULT_VALSIZE,
     DEFAULT_TESTSIZE,
     DEFAULT_NUMFEATURES,
     DEFAULT_BIAS_METHOD,
-    DEFAULT_AUGMENT_FACTOR,
-    DEFAULT_CACHE_DIR,
-    DEFAULT_BATCH_SIZE,
+    KEYWORD_REPLACEMENTS,
     preload_datasets,
-    batched_pipeline_transform,
-    save_cached_features,
-    load_cached_features,
 )
 
 __all__ = [
     "DatasetId",
     "DatasetModality",
     "Dataset",
-    "TabularDatasetMixin",
-    "ImageDatasetMixin",
-    "TextDatasetMixin",
-    "NoisyLabelDataset",
+    "DirtyLabelDataset",
     "BiasMethod",
     "BiasedMixin",
-    "BiasedNoisyLabelDataset",
-    "AugmentableMixin",
+    "BiasedDirtyLabelDataset",
     "RandomDataset",
     "UCI",
     "FashionMNIST",
     "TwentyNewsGroups",
-    "Higgs",
-    "DataPerfVision",
-    "CifarN",
     "load_dataset",
     "DEFAULT_TRAINSIZE",
     "DEFAULT_VALSIZE",
     "DEFAULT_TESTSIZE",
     "DEFAULT_NUMFEATURES",
     "DEFAULT_BIAS_METHOD",
-    "DEFAULT_AUGMENT_FACTOR",
-    "DEFAULT_CACHE_DIR",
-    "DEFAULT_BATCH_SIZE",
+    "KEYWORD_REPLACEMENTS",
     "preload_datasets",
-    "batched_pipeline_transform",
-    "save_cached_features",
-    "load_cached_features",
 ]
```

### Comparing `datascope-experiments-0.0.81/datascope/experiments/reports/aggregate_plot.py` & `datascope-experiments-0.0.9/datascope/experiments/reports/aggregate_plot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import re
 
 from enum import Enum
 from functools import partial
-from itertools import combinations, product
 from matplotlib.figure import Figure
 from matplotlib.ticker import EngFormatter, PercentFormatter
-from matplotlib.transforms import Bbox
-from numpy.typing import NDArray
-from scipy.sparse import lil_matrix
-from scipy.sparse.csgraph import connected_components
 from typing import Callable, Optional, Dict, Any, List, Union, TypeVar, Tuple
 
-from pandas import DataFrame, MultiIndex
-from pandas.core.groupby.generic import DataFrameGroupBy
+from pandas import DataFrame
 from pandas.core.groupby.groupby import GroupBy
 
 from ..scenarios import Report, Study, result, attribute
 
 COLOR_NAMES = ["blue", "red", "yellow", "green", "purple", "brown", "cyan", "pink"]
-COLORS = ["#2BBFD9", "#DF362A", "#FAC802", "#8AB365", "#C670D2", "#AE7E1E", "#008F6B", "#6839CC"]
+COLORS = ["#2BBFD9", "#DF362A", "#FAC802", "#8AB365", "#C670D2", "#C58F21", "#00AC9B", "#DB006A"]
 LABELS = {
     "random": "Random",
     "shapley-tmc": "Shapley TMC",
     "shapley-knn-single": "Shapley KNN Single",
     "shapley-knn-interactive": "Shapley KNN Interactive",
     "shapley-tmc-10": "Shapley TMC x10",
     "shapley-tmc-50": "Shapley TMC x50",
@@ -55,61 +49,46 @@
 class AggregationMode(str, Enum):
     MEDIAN_PERC_90 = "median-perc-90"
     MEDIAN_PERC_95 = "median-perc-95"
     MEDIAN_PERC_99 = "median-perc-99"
     MEAN_STD = "mean-std"
 
 
-VALUE_MEASURES: Dict[AggregationMode, Dict[str, Union[Callable, str]]] = {
+VALUE_MEASURES: Dict[AggregationMode, Dict[str, Callable]] = {
     AggregationMode.MEAN_STD: {
-        "mean": "mean",
-        "std": "std",
+        "mean": np.mean,
+        "std": np.std,
         "std-l": lambda x: np.mean(x) - np.std(x),
         "std-h": lambda x: np.mean(x) + np.std(x),
     },
     AggregationMode.MEDIAN_PERC_90: {
-        "median": "median",
+        "median": np.median,
         "95perc-l": partial(np.percentile, q=5),
         "95perc-h": partial(np.percentile, q=95),
     },
     AggregationMode.MEDIAN_PERC_95: {
-        "median": "median",
+        "median": np.median,
         "95perc-l": partial(np.percentile, q=2.5),
         "95perc-h": partial(np.percentile, q=97.5),
     },
     AggregationMode.MEDIAN_PERC_99: {
-        "median": "median",
+        "median": np.median,
         "95perc-l": partial(np.percentile, q=0.5),
         "95perc-h": partial(np.percentile, q=99.5),
     },
 }
 
 VALUE_MEASURE_C: Dict[AggregationMode, str] = {
     AggregationMode.MEAN_STD: "mean",
     AggregationMode.MEDIAN_PERC_90: "median",
     AggregationMode.MEDIAN_PERC_95: "median",
     AggregationMode.MEDIAN_PERC_99: "median",
 }
 
 
-class CrossAggregationMode(str, Enum):
-    MEAN_SQUARE_ERROR = "mse"
-    ROOT_MEAN_SQUARE_ERROR = "rmse"
-    MEAN_ABSOLUTE_ERROR = "mae"
-    MEAN_ABSOLUTE_PERCENTAGE_ERROR = "mape"
-
-
-CROSS_AGGREGATION_FUNCTIONS: Dict[CrossAggregationMode, Callable[[NDArray, NDArray], float]] = {
-    CrossAggregationMode.MEAN_SQUARE_ERROR: lambda x1, x2: np.square(x1 - x2).mean(),
-    CrossAggregationMode.ROOT_MEAN_SQUARE_ERROR: lambda x1, x2: np.sqrt(np.square(x1 - x2).mean()),
-    CrossAggregationMode.MEAN_ABSOLUTE_ERROR: lambda x1, x2: np.abs(x1 - x2).mean(),
-    CrossAggregationMode.MEAN_ABSOLUTE_PERCENTAGE_ERROR: lambda x1, x2: np.abs((x1 - x2) / (x1 + 1e-6)).mean(),
-}
-
-
 class SliceOp(str, Enum):
     COUNT = "count"
     FIRST = "first"
     LAST = "last"
     MAX = "max"
     MIN = "min"
     MEAN = "mean"
@@ -126,15 +105,14 @@
     SliceOp.MEAN: GroupBy.mean,
     SliceOp.STD: GroupBy.std,
     SliceOp.MEDIAN: GroupBy.median,
 }
 
 DEFAULT_LABEL_FORMAT = "{compare}"
 DEFAULT_FONTSIZE = 16
-DEFAULT_LINEWIDTH = 2.5
 
 
 def represent(x: Any):
     if isinstance(x, Enum):
         return repr(x.value)
     if isinstance(x, float):
         return "%.2f" % x
@@ -163,103 +141,44 @@
     aggmode: AggregationMode = AggregationMode.MEDIAN_PERC_95,
 ) -> DataFrame:
     if compare is None:
         compare = []
     value_measures = VALUE_MEASURES[aggmode]
 
     groupbycols = [index] + list(compare)
-    dataframe = dataframe[[index] + targetval + compare].dropna()
     values = [dataframe.groupby(groupbycols)[targetval].agg(f).add_suffix(":" + k) for (k, f) in value_measures.items()]
     dataframe = pd.concat(values, axis=1)
     dataframe.sort_index(inplace=True)
     if len(compare) > 0:
-        unstacked = dataframe.unstack()
-        dataframe = unstacked if isinstance(unstacked, DataFrame) else unstacked.to_frame()
-        assert isinstance(dataframe.columns, MultiIndex)
-        dataframe.columns = dataframe.columns.swaplevel().map(lambda x: tuple(str(xx) for xx in x)).map(">".join)
+        dataframe = dataframe.unstack()
+        dataframe.columns = dataframe.columns.swaplevel().map(">".join)
     return dataframe
 
 
 def summarize(
     dataframe: DataFrame,
     summarize: List[str],
     compare: Optional[List[str]] = None,
     summode: Optional[AggregationMode] = None,
 ) -> dict:
     if summode is None:
         summode = AggregationMode.MEAN_STD
     if compare is None:
         compare = []
     value_measures = VALUE_MEASURES[summode]
-    dataframe = dataframe[summarize + compare].dropna()
-    if len(compare) > 0:
-        summary_frames = [
-            dataframe.groupby(compare)[summarize].agg(f).add_suffix(":" + k) for (k, f) in value_measures.items()
-        ]
-        return pd.concat(summary_frames, axis=1).to_dict(orient="index")
-    else:
-        summary_series = [dataframe[summarize].agg(f).add_suffix(":" + k) for (k, f) in value_measures.items()]
-        return pd.concat(summary_series, axis=0).to_dict()
-
-
-def cross_aggregate(
-    dataframe: pd.DataFrame,
-    index: Optional[List[str]],
-    compare: List[str],
-    targetval: List[str],
-    crossaggover: List[str],
-    crossaggpairs: Optional[List[str]] = None,
-    crossaggmode: CrossAggregationMode = CrossAggregationMode.MEAN_ABSOLUTE_ERROR,
-):
-    # Pivot the table so that target values from different comparison values appear side by side.
-    index = [] if index is None else index
-    crossaggover = [x for x in crossaggover if x not in index]
-    assert index is not None
-    indexlen = len(index)
-    dataframe = dataframe.pivot(index=index + crossaggover, columns=compare, values=targetval)
-
-    # Produce a series of pairwise comparisons for each target value and then concatdaenate them into one dataframe.
-    method = CROSS_AGGREGATION_FUNCTIONS[crossaggmode]
-    correlation_parts = []
-    for val in targetval:
-        target: Union[DataFrame, DataFrameGroupBy] = dataframe[[val]]
-        if len(index) > 0:
-            assert isinstance(target, DataFrame)
-            target = target.groupby(index)
-        target = target.corr(method=method)  # type: ignore
-        target = target.stack(dropna=False, level=compare)  # type: ignore
-        target = target.droplevel(axis=0, level=1 if len(index) > 0 else 0)  # type: ignore
-        correlation_parts.append(target)
-    dataframe = pd.concat(correlation_parts, axis=1)
-
-    # Keep only a single instance of each pair.
-    if crossaggpairs is None or len(crossaggpairs) == 0:
-        comparevals = [sorted(dataframe[col].unique()) for col in compare]
-        crossaggpairs = [x[0] + x[1] for x in combinations(product(*comparevals), r=2)]
-    pairs = [tuple(x.replace("&", ",").split(",")) for x in crossaggpairs]
-    dataframe = dataframe[dataframe.index.map(lambda x: x[indexlen:] in pairs)]
-
-    # Move values from the index into regular columns.
-    n = len(compare)
-
-    def column_mapper(x: Tuple) -> Tuple:
-        result = tuple(x[:indexlen])
-        result += (",".join(str(x[i]) for i in range(-2 * n, -n)) + "&" + ",".join(str(x[i]) for i in range(-n, 0)),)
-        result += tuple([None for _ in range(2 * n - 1)])
-        return result
-
-    dataframe.index = dataframe.index.map(column_mapper)
-    dataframe.index = dataframe.index.droplevel(list(range(-2 * n + 1, 0)))
-    dataframe.index = dataframe.index.set_names(">".join(compare), level=-1 if len(index) > 0 else None)
-    dataframe = dataframe.reset_index()
-    return dataframe
+    groups = dataframe.groupby(compare) if len(compare) > 0 else dataframe
+    values = [groups[summarize].agg(f).add_suffix(":" + k) for (k, f) in value_measures.items()]
+    axis = 0 if len(compare) == 0 else 1
+    dataframe = pd.concat(values, axis=axis)
+    dataframe.sort_index(inplace=True)
+    return dataframe.to_dict(orient="index") if isinstance(dataframe, DataFrame) else dataframe.to_dict()
 
 
 def replace_keywords(source: str, keyword_replacements: Dict[str, str]) -> str:
-    for k, v in sorted(keyword_replacements.items(), key=lambda x: len(x[0]), reverse=True):
+    for k, v in sorted(keyword_replacements.items(), key=lambda x: len(x[1]), reverse=True):
         source = re.sub("(?<![a-zA-Z])%s(?![a-z-Z])" % k, v, source)
         # source = source.replace(k, v)
     return source
 
 
 def get_colors(keys: List[Tuple[str, ...]], colors: Optional[Dict[Tuple[str, ...], str]]) -> List[str]:
     available_default_colors = [
@@ -275,77 +194,14 @@
                 color = COLORS[COLOR_NAMES.index(color)]
             result_colors.append(color)
         else:
             result_colors.append(available_default_colors.pop(0))
     return result_colors
 
 
-def fix_text_positioning(texts: Union[List[plt.Text], List[plt.Annotation]], axes: plt.Axes) -> None:
-
-    # Get renderer from axes.
-    renderer = axes.figure.canvas.renderer  # type: ignore
-
-    # Extract bounding boxes of all text objects.
-    transforms = [text.get_transform() for text in texts]
-    bboxes = [text.get_window_extent(renderer) for text in texts]
-    # bboxes = [axes.transData.inverted().transform_bbox(bbox) for bbox in bboxes]
-    heights = np.array([bbox.y1 - bbox.y0 for bbox in bboxes])
-    vertical_positions = np.array([bbox.y0 for bbox in bboxes])
-
-    # # Draw a bounding rectangle of all objects using bboxes.
-    # for bbox in bboxes:
-    #     rect_bbox = axes.transData.inverted().transform_bbox(bbox)
-    #     axes.add_patch(
-    #         Rectangle(
-    #             (rect_bbox.xmin, rect_bbox.ymin),
-    #             rect_bbox.width,
-    #             rect_bbox.height,
-    #             fill=False,
-    #             edgecolor="red",
-    #             # transform=axes.transAxes,
-    #         )
-    #     )
-
-    # Find groups of texts that overlap.
-    overlaps = lil_matrix((len(bboxes), len(bboxes)), dtype=bool)
-    for i in range(len(bboxes)):
-        for j in range(i + 1, len(bboxes)):
-            if bboxes[i].overlaps(bboxes[j]):
-                overlaps[i, j] = True
-    n_components, labels = connected_components(csgraph=overlaps, directed=False, return_labels=True)
-    for i in range(n_components):
-        group = np.where(labels == i)[0]
-        if len(group) > 1:
-            # Reorder the group by vertical position.
-            group = group[np.argsort(vertical_positions[group])]
-
-            # Find the bounding box that covers the group and use it to adjust the position of the texts.
-            bbox = Bbox.union([bboxes[i] for i in group])
-            y_cur = (bbox.ymin + bbox.ymax) / 2 - np.sum(heights[group]) / 2 + heights[group[0]] / 2
-            for i in group:
-                text = texts[i]
-                _, y = transforms[i].inverted().transform((0, y_cur))
-                text.set_y(y)
-                y_cur += heights[i]
-
-    # Expand the axes to fit the new text positions.
-    bboxes = [text.get_window_extent(renderer) for text in texts]
-    bbox_union = Bbox.union(bboxes)
-    bbox_data_coords = axes.transData.inverted().transform_bbox(bbox_union)
-    # axes.update_datalim(bbox_union)
-    if bbox_data_coords.xmin < axes.get_xlim()[0]:
-        axes.set_xlim(xmin=bbox_data_coords.xmin)
-    if bbox_data_coords.xmax > axes.get_xlim()[1]:
-        axes.set_xlim(xmax=bbox_data_coords.xmax)
-    if bbox_data_coords.ymin < axes.get_ylim()[0]:
-        axes.set_ylim(ymin=bbox_data_coords.ymin)
-    if bbox_data_coords.ymax > axes.get_ylim()[1]:
-        axes.set_ylim(ymax=bbox_data_coords.ymax)
-
-
 def lineplot(
     dataframe: DataFrame,
     index: str,
     targetval: str,
     compare: Optional[List[str]] = None,
     compareorder: List[str] = [],
     colors: Optional[Dict[str, str]] = None,
@@ -354,15 +210,14 @@
     labelformat: Optional[str] = None,
     summary: Optional[dict] = None,
     keyword_replacements: Optional[Dict[str, str]] = None,
     axes: Optional[plt.Axes] = None,
     fontsize: int = DEFAULT_FONTSIZE,
     annotations: bool = False,
     dontcompare: Optional[str] = None,
-    linemarker: Optional[str] = None,
 ) -> Optional[Figure]:
     if compare is None:
         compare = []
     if labelformat is None:
         if len(compare) > 0:
             labelformat = "; ".join("%%(%s)s" % c for c in compare)
         else:
@@ -381,47 +236,41 @@
     else:
         comparison = [(targetval,)]
         dataframe.columns = dataframe.columns.map(lambda x: (targetval,) + tuple(x.split(":")))
     compareorder_unpacked = [tuple(x.split(",")) for x in compareorder]
     if len(compareorder_unpacked) > 0:
         comparison = sorted(
             comparison,
-            key=lambda x: (
-                compareorder_unpacked.index(x)
-                if compareorder_unpacked is not None and x in compareorder_unpacked
-                else len(comparison)
-            ),
+            key=lambda x: compareorder_unpacked.index(x)
+            if compareorder_unpacked is not None and x in compareorder_unpacked
+            else len(comparison),
         )
 
     figure: Optional[Figure] = None
     if axes is None:
         figure = plt.figure(figsize=(10, 8))
-        subplots = figure.subplots()
-        assert isinstance(subplots, plt.Axes)
-        axes = subplots
-    else:
-        figure = axes.get_figure()
-    assert figure is not None
+        axes = figure.subplots()
 
     labels: List[str] = []
     for i, comp in enumerate(comparison):
+        if ",".join(str(c) for c in comp) in dontcompare:
+            continue
         formatdict = dict(zip(compare, comp))
         if summary is not None:
             comp_summary = summary
             for c in comp:
                 comp_summary = comp_summary.get(c, comp_summary)
             formatdict.update(comp_summary)
         label = labelformat % formatdict
         label = replace_keywords(label, keyword_replacements)
         labels.append(label)
 
     centercol = VALUE_MEASURE_C[aggmode]
     split_colors = dict((tuple(k.split(",")), v) for (k, v) in colors.items()) if colors is not None else None
     comp_colors = get_colors(comparison, colors=split_colors)
-    texts = []
     for i, comp in enumerate(comparison):
         if ",".join(str(c) for c in comp) in dontcompare:
             continue
         cols: List[str] = dataframe[comp][targetval].columns.to_list()
         uppercol = next(c for c in cols if c.endswith("-h"))
         lowercol = next(c for c in cols if c.endswith("-l"))
         upper = dataframe[comp][targetval][uppercol].to_numpy()
@@ -429,73 +278,37 @@
         if errdisplay == ErrorDisplay.SHADE:
             axes.fill_between(dataframe.index.values, upper, lower, color=comp_colors[i], alpha=0.2)
         elif errdisplay == ErrorDisplay.BAR:
             center = dataframe[comp][targetval][centercol]
             xval = dataframe.index.values
             yval = center.to_numpy()
             yerr = np.abs(np.stack([lower, upper]) - yval)
-            axes.errorbar(
-                xval,
-                yval,
-                yerr=yerr,
-                fmt="o",
-                linewidth=DEFAULT_LINEWIDTH,
-                capsize=6,
-                color=comp_colors[i],
-                label=labels[i],
-            )
+            axes.errorbar(xval, yval, yerr=yerr, fmt="o", linewidth=2, capsize=6, color=comp_colors[i], label=labels[i])
             if annotations:
                 for x, y in zip(xval, yval):
-                    text = axes.annotate(
+                    axes.annotate(
                         "%.2f" % y,
                         xy=(x, y),
                         xytext=(fontsize * 0.5, 0),
                         textcoords="offset points",
                         fontsize=fontsize,
                         horizontalalignment="left",
                         verticalalignment="center",
-                        # arrowprops=dict(arrowstyle="-", color=comp_colors[i]),
                     )
-                    texts.append(text)
-
-    linedesc = list(zip(comparison, comp_colors, labels))
-    for comp, c, l in linedesc:
-        if ",".join(str(c) for c in comp) in dontcompare:
-            continue
-        ll = l if errdisplay != ErrorDisplay.BAR else None
-        axes.plot(
-            dataframe[comp][targetval][centercol],
-            color=c,
-            label=ll,
-            marker=linemarker,
-            markersize=4 * DEFAULT_LINEWIDTH,
-            linewidth=DEFAULT_LINEWIDTH,
-        )
 
-    # Plot a dashed line over the current lines to improve visibility of overlapping lines.
-    for comp, c, l in reversed(linedesc):
+    for i, comp in enumerate(comparison):
         if ",".join(str(c) for c in comp) in dontcompare:
             continue
-        axes.plot(dataframe[comp][targetval][centercol], color=c, linestyle=(0, (3, 3)), linewidth=DEFAULT_LINEWIDTH)
+        axes.plot(dataframe[comp][targetval][centercol], color=comp_colors[i], label=labels[i])
 
     # axes.set_xlim([dataframe.index.values[0], (dataframe.index.values[-1] - dataframe.index.values[0]) * 1.2])
     # axes.set_ylim([-0.2, 1])
     axes.set_ylabel(replace_keywords(targetval, keyword_replacements), fontsize=fontsize, wrap=True)
     axes.set_xlabel(replace_keywords(index, keyword_replacements), fontsize=fontsize, wrap=True)
     # axes.legend(loc="lower right", fontsize=fontsize, borderaxespad=0, edgecolor="black", fancybox=False)
-
-    axes.relim()
-
-    if len(texts) > 0:
-        figure.canvas.draw()
-        fix_text_positioning(texts, axes)
-
-    axes.autoscale_view(tight=True)
-    figure.canvas.draw()
-
     return figure
 
 
 T = TypeVar("T")
 
 
 def dictpivot(d: Dict, compare: List[str], prefix: Tuple[str, ...] = tuple()) -> Dict[Tuple[str, ...], Dict]:
@@ -546,99 +359,69 @@
     if keyword_replacements is None:
         keyword_replacements = {}
     if dontcompare is None:
         dontcompare = ""
     figure: Optional[Figure] = None
     if axes is None:
         figure = plt.figure(figsize=(10, 8))
-        subplots = figure.subplots()
-        assert isinstance(subplots, plt.Axes)
-        axes = subplots
-    else:
-        figure = axes.get_figure()
-    assert figure is not None
+        axes = figure.subplots()
 
     # x, y, yerr = [], [], []
     summary = dictpivot(summary, compare=compare)
     summary_items = list(summary.items())
 
+    comparison = [item[0] for item in summary_items]
+    split_colors = dict((tuple(k.split(",")), v) for (k, v) in colors.items()) if colors is not None else None
+    comp_colors = get_colors(comparison, colors=split_colors)
     compareorder_unpacked = [tuple(x.split(",")) for x in compareorder]
     if len(compareorder_unpacked) > 0:
         summary_items = sorted(
             summary_items,
-            key=lambda x: (
-                compareorder_unpacked.index(x[0])
-                if compareorder_unpacked is not None and x[0] in compareorder_unpacked
-                else len(summary_items)
-            ),
+            key=lambda x: compareorder_unpacked.index(x[0])
+            if compareorder_unpacked is not None and x[0] in compareorder_unpacked
+            else len(comparison),
         )
-
-    comparison = [item[0] for item in summary_items]
-    split_colors = dict((tuple(k.split(",")), v) for (k, v) in colors.items()) if colors is not None else None
-    comp_colors = get_colors(comparison, colors=split_colors)
-    texts = []
-
     for i, (comp, values) in enumerate(summary_items):
         if ",".join(str(c) for c in comp) in dontcompare:
             continue
         centercol = VALUE_MEASURE_C[aggmode]
         formatdict = dict(zip(compare, comp))
         label = labelformat % formatdict
         label = replace_keywords(label, keyword_replacements)
-        # xval = "; ".join(str(x) for x in comp)
+        xval = "; ".join(str(x) for x in comp)
         col = targetval + ":" + centercol
         yval = values[col]
 
         uppercol = next(c for c in values.keys() if c.endswith("-h"))
         lowercol = next(c for c in values.keys() if c.endswith("-l"))
         yerr = np.abs(np.array([[values[col] - values[lowercol]], [values[col] - values[uppercol]]]))
-        axes.errorbar(
-            [i],
-            [yval],
-            yerr=yerr,
-            fmt="o",
-            linewidth=DEFAULT_LINEWIDTH,
-            capsize=6,
-            color=comp_colors[i],
-            label=label,
-        )
+        axes.errorbar([xval], [yval], yerr=yerr, fmt="o", linewidth=2, capsize=6, color=comp_colors[i], label=label)
 
         if annotations:
-            text = axes.annotate(
+            axes.annotate(
                 "%.2f" % yval,
-                xy=(i, yval),
+                xy=(xval, yval),
                 xytext=(fontsize * 0.5, 0),
                 textcoords="offset points",
                 fontsize=fontsize,
                 horizontalalignment="left",
                 verticalalignment="center",
             )
-            texts.append(text)
 
     axes.set_ylabel(replace_keywords(targetval, keyword_replacements), fontsize=fontsize, wrap=True)
     axes.get_xaxis().set_ticks([])
-    axes.relim()
 
     # Squeeze xlimit.
     xlim = axes.get_xlim()
     xlim_delta = xlim[1] - xlim[0]
     axes.set_xlim((xlim[0] - xlim_delta * 0.1, xlim[1] + xlim_delta * 0.3))
     # axes.legend(
     #     loc="upper right", fontsize=fontsize, borderaxespad=0, edgecolor="black", fancybox=False, ncol=len(summary)
     # )
 
-    axes.relim()
-
-    if len(texts) > 0:
-        figure.canvas.draw()
-        fix_text_positioning(texts, axes)
-
-    axes.autoscale_view(tight=True)
-    figure.canvas.draw()
-
     return figure
 
 
 def dotplot(
     summary: dict,
     xtargetval: str,
     ytargetval: str,
@@ -667,106 +450,77 @@
     if keyword_replacements is None:
         keyword_replacements = {}
     if dontcompare is None:
         dontcompare = ""
     figure: Optional[Figure] = None
     if axes is None:
         figure = plt.figure(figsize=(10, 8))
-        subplots = figure.subplots()
-        assert isinstance(subplots, plt.Axes)
-        axes = subplots
-    else:
-        figure = axes.get_figure()
-    assert figure is not None
+        axes = figure.subplots()
 
     # x, y, yerr = [], [], []
     summary = dictpivot(summary, compare=compare)
     summary_items = list(summary.items())
 
+    comparison = [item[0] for item in summary_items]
+    split_colors = dict((tuple(k.split(",")), v) for (k, v) in colors.items()) if colors is not None else None
+    comp_colors = get_colors(comparison, colors=split_colors)
     compareorder_unpacked = [tuple(x.split(",")) for x in compareorder]
     if len(compareorder_unpacked) > 0:
         summary_items = sorted(
             summary_items,
-            key=lambda x: (
-                compareorder_unpacked.index(x[0])
-                if compareorder_unpacked is not None and x[0] in compareorder_unpacked
-                else len(summary_items)
-            ),
+            key=lambda x: compareorder_unpacked.index(x[0])
+            if compareorder_unpacked is not None and x[0] in compareorder_unpacked
+            else len(comparison),
         )
-
-    comparison = [item[0] for item in summary_items]
-    split_colors = dict((tuple(k.split(",")), v) for (k, v) in colors.items()) if colors is not None else None
-    comp_colors = get_colors(comparison, colors=split_colors)
-    texts = []
-
     for i, (comp, values) in enumerate(summary_items):
         if ",".join(str(c) for c in comp) in dontcompare:
             continue
         centercol = VALUE_MEASURE_C[aggmode]
         formatdict = dict(zip(compare, comp))
         label = labelformat % formatdict
         label = replace_keywords(label, keyword_replacements)
-        # xval = "; ".join(str(x) for x in comp)
+        xval = "; ".join(str(x) for x in comp)
         xcol = xtargetval + ":" + centercol
         xval = values[xcol]
         ycol = ytargetval + ":" + centercol
         yval = values[ycol]
 
         xuppercol = next(c for c in values.keys() if c.startswith(xtargetval) and c.endswith("-h"))
         xlowercol = next(c for c in values.keys() if c.startswith(xtargetval) and c.endswith("-l"))
         xerr = np.abs(np.array([[values[xcol] - values[xlowercol]], [values[xcol] - values[xuppercol]]]))
 
         yuppercol = next(c for c in values.keys() if c.startswith(ytargetval) and c.endswith("-h"))
         ylowercol = next(c for c in values.keys() if c.startswith(ytargetval) and c.endswith("-l"))
         yerr = np.abs(np.array([[values[ycol] - values[ylowercol]], [values[ycol] - values[yuppercol]]]))
         axes.errorbar(
-            [xval],
-            [yval],
-            xerr=xerr,
-            yerr=yerr,
-            fmt="o",
-            linewidth=DEFAULT_LINEWIDTH,
-            capsize=6,
-            color=comp_colors[i],
-            label=label,
+            [xval], [yval], xerr=xerr, yerr=yerr, fmt="o", linewidth=2, capsize=6, color=comp_colors[i], label=label
         )
 
         if annotations:
-            text = axes.annotate(
+            axes.annotate(
                 "%.2f" % yval,
                 xy=(xval, yval),
                 xytext=(fontsize * 0.5, 0),
                 textcoords="offset points",
                 fontsize=fontsize,
                 horizontalalignment="left",
                 verticalalignment="center",
             )
-            texts.append(text)
 
     axes.set_ylabel(replace_keywords(ytargetval, keyword_replacements), fontsize=fontsize, wrap=True)
     axes.set_xlabel(replace_keywords(xtargetval, keyword_replacements), fontsize=fontsize, wrap=True)
-    axes.relim()
 
     # Squeeze xlimit.
     # xlim = axes.get_xlim()
     # xlim_delta = xlim[1] - xlim[0]
     # axes.set_xlim((xlim[0] - xlim_delta * 0.1, xlim[1] + xlim_delta * 0.3))
     # axes.legend(
     #     loc="upper right", fontsize=fontsize, borderaxespad=0, edgecolor="black", fancybox=False, ncol=len(summary)
     # )
 
-    axes.relim()
-
-    if len(texts) > 0:
-        figure.canvas.draw()
-        fix_text_positioning(texts, axes)
-
-    axes.autoscale_view(tight=True)
-    figure.canvas.draw()
-
     return figure
 
 
 NONE_SYMBOL = "-"
 DEFAULT_PLOTSIZE = [10, 8]
 
 
@@ -810,82 +564,76 @@
     return spec
 
 
 def unpackdict(target: Dict[str, Union[Dict, Any]], prefix: str = "") -> Dict[str, Any]:
     result: Dict[str, Any] = {}
     for k, v in target.items():
         if isinstance(v, dict):
-            for kk, vv in unpackdict(v, prefix=str(k)).items():
+            for kk, vv in unpackdict(v, prefix=k).items():
                 key = ".".join(([] if prefix == "" else [prefix]) + [kk])
                 result[key] = vv
         else:
             key = ".".join(([] if prefix == "" else [prefix]) + [k])
             result[key] = v
     return result
 
 
 class AggregatePlot(Report, id="aggplot"):
     def __init__(
         self,
         study: Study,
-        dataframe: DataFrame,
-        partvals: Optional[Dict[str, Any]] = None,
-        id: Optional[str] = None,
         plot: Optional[Union[List[str], str]] = None,
         index: Optional[str] = None,
         targetval: Optional[Union[List[str], str]] = None,
         compare: Optional[Union[List[str], str]] = None,
         compareorder: Optional[List[str]] = None,
         colors: Optional[List[str]] = None,
         summarize: Optional[Union[List[str], str]] = None,
-        crossaggover: Optional[Union[List[str], str]] = None,
         sliceby: Optional[Union[List[str], str]] = None,
         sliceop: Optional[SliceOp] = None,
         resultfilter: Optional[str] = None,
         errdisplay: Optional[ErrorDisplay] = None,
         aggmode: Optional[AggregationMode] = None,
         summode: Optional[AggregationMode] = None,
-        crossaggmode: Optional[CrossAggregationMode] = None,
         xlogscale: Optional[Union[List[bool], bool]] = None,
         ylogscale: Optional[Union[List[bool], bool]] = None,
         xtickfmt: Optional[Union[List[TickFormat], TickFormat]] = None,
         ytickfmt: Optional[Union[List[TickFormat], TickFormat]] = None,
-        linemarker: Optional[Union[List[str], str]] = None,
         annotations: Optional[Union[List[bool], bool]] = None,
         dontcompare: Optional[Union[List[str], str]] = None,
+        groupby: Optional[Dict[str, Any]] = None,
         labelformat: Optional[str] = None,
         plotsize: Optional[List[int]] = None,
         fontsize: Optional[int] = None,
         usetex: Optional[bool] = True,
         legend: Optional[bool] = True,
         titleformat: Optional[List[str]] = None,
+        id: Optional[str] = None,
         **kwargs: Any,
     ) -> None:
-        super().__init__(study=study, dataframe=dataframe, id=id, partvals=partvals, **kwargs)
+        super().__init__(study, id=id, groupby=groupby, **kwargs)
         self._plot = ensurelist(plot, default=None)
         n_plots = len(self._plot)
         self._index = index
         self._targetval: List[str] = ensurelist(targetval, default=None)
         self._compare: List[str] = ensurelist(compare, default=None)
         self._compareorder: List[str] = compareorder if compareorder is not None else []
         self._colors: List[str] = colors if colors is not None else []
         self._summarize: List[str] = ensurelist(summarize, default=None)
-        self._crossaggover: List[str] = ensurelist(crossaggover, default=None)
+        self._filter = filter
         self._sliceby: List[str] = ensurelist(sliceby, default=None)
         self._sliceop = sliceop if sliceop is not None else SliceOp.FIRST
         self._resultfilter: Optional[str] = resultfilter
         self._errdisplay = errdisplay if errdisplay is not None else ErrorDisplay.SHADE
         self._aggmode = aggmode if aggmode is not None else AggregationMode.MEDIAN_PERC_95
         self._summode = summode if summode is not None else AggregationMode.MEDIAN_PERC_95
-        self._crossaggmode = crossaggmode if crossaggmode is not None else CrossAggregationMode.MEAN_ABSOLUTE_ERROR
         self._xlogscale: List[bool] = ensurelist(xlogscale, default=False, length=n_plots)
         self._ylogscale: List[bool] = ensurelist(ylogscale, default=False, length=n_plots)
         self._xtickfmt: List[TickFormat] = ensurelist(xtickfmt, default=TickFormat.DEFAULT, length=n_plots)
         self._ytickfmt: List[TickFormat] = ensurelist(ytickfmt, default=TickFormat.DEFAULT, length=n_plots)
-        self._linemarker: List[str] = ensurelist(linemarker, default="", length=n_plots)
         self._annotations: List[bool] = ensurelist(annotations, default=False, length=n_plots)
         self._dontcompare: List[str] = ensurelist(dontcompare, default=NONE_SYMBOL, length=n_plots)
 
         self._labelformat = (
             labelformat
             if labelformat is not None
             else (
@@ -898,15 +646,15 @@
         self._plotsize = plotsize if plotsize is not None else DEFAULT_PLOTSIZE
         if len(self._plotsize) != 2:
             raise ValueError("The plotsize must have two parameters: width and height.")
         self._fontsize = fontsize if fontsize is not None else DEFAULT_FONTSIZE
         self._usetex = usetex if usetex is not None else True
         self._legend = legend if legend is not None else True
         if titleformat is None:
-            titleformat = ["; ".join("%s=%%(%s)s" % (str(k).title(), str(k)) for k in self._partvals.keys())]
+            titleformat = [" ".join("%s=%%(%s)s" % (str(k).title(), str(k)) for k in self._groupby.keys())]
         self._titleformat = titleformat
 
         self._view: Optional[DataFrame] = None
         self._figure: Optional[Figure] = None
         self._summary: Optional[dict] = None
 
     @attribute
@@ -941,19 +689,14 @@
 
     @attribute
     def summarize(self) -> List[str]:
         """The attribute aggregate over the entire dataframe."""
         return self._summarize
 
     @attribute
-    def crossaggover(self) -> List[str]:
-        """The attributes that we use for joining the cross aggregation."""
-        return self._crossaggover
-
-    @attribute
     def sliceby(self) -> List[str]:
         """Slice along the index attribute by taking the first value in each slice plane.
         We use the given set of attributes to define a slice plane."""
         return self._sliceby
 
     @attribute
     def sliceop(self) -> SliceOp:
@@ -972,19 +715,14 @@
 
     @attribute
     def summode(self) -> AggregationMode:
         """The mode of summarization to apply."""
         return self._summode
 
     @attribute
-    def crossaggmode(self) -> CrossAggregationMode:
-        """The mode of cross aggregation to apply."""
-        return self._crossaggmode
-
-    @attribute
     def errdisplay(self) -> ErrorDisplay:
         """The method of displaying error bars."""
         return self._errdisplay
 
     @attribute
     def xlogscale(self) -> List[bool]:
         """Whether to represent the x-axis in the logarithmic scale."""
@@ -1002,19 +740,14 @@
 
     @attribute
     def ytickfmt(self) -> List[TickFormat]:
         """The tick formatting to use for the y-axis."""
         return self._ytickfmt
 
     @attribute
-    def linemarker(self) -> List[str]:
-        """The type of marker to use when plotting lines."""
-        return self._linemarker
-
-    @attribute
     def annotations(self) -> List[bool]:
         """Whether to add annotations to all points displayed."""
         return self._annotations
 
     @attribute
     def dontcompare(self) -> List[str]:
         """Space-separated list of comma separated lists of values that should not be compared."""
@@ -1050,130 +783,77 @@
 
     @attribute
     def titleformat(self) -> List[str]:
         """The formatted text to use in the title."""
         return self._titleformat
 
     def generate(self) -> None:
-        dataframe = self.dataframe
-        if self.resultfilter is not None:
-            dataframe = dataframe.query(self.resultfilter)
+        dataframe = filter(self.study.dataframe, attributes=self.groupby, resultfilter=self.resultfilter)
 
         keyword_replacements: Dict[str, str] = {}
         summarydict: Dict[str, str] = {}
-        if self.study is not None:
-            for scenario in self.study.scenarios:
-                keyword_replacements.update(scenario.keyword_replacements)
+        for scenario in self.study.scenarios:
+            keyword_replacements.update(scenario.keyword_replacements)
 
         if self.index is not None and len(self.targetval) > 0:
             if self._view is None:
-                agg_dataframe = dataframe
-
-                # If slicing was specified, then we slice the dataframe first.
-                if len(self.sliceby) > 0:
-                    groupattrs = self.sliceby + self.compare + [self.index]
-                    groupby = agg_dataframe.groupby(groupattrs)
-                    sliceop = SLICE_OPS[self.sliceop]
-                    agg_dataframe = sliceop(groupby)
-                    agg_dataframe.reset_index(inplace=True)
-
-                if len(self._crossaggover) > 0:
-                    agg_dataframe = cross_aggregate(
-                        dataframe=dataframe,
-                        index=[self.index],
-                        compare=self.compare,
-                        targetval=self.targetval,
-                        crossaggover=self._crossaggover,
-                        crossaggpairs=self._compareorder,
-                        crossaggmode=self._crossaggmode,
-                    )
-
                 self._view = aggregate(
-                    dataframe=agg_dataframe,
+                    dataframe=dataframe,
                     compare=self.compare,
                     index=self.index,
                     targetval=self.targetval,
                     aggmode=self.aggmode,
                 )
 
         if len(self.summarize) > 0:
-            if self._summary is None:
-                summ_dataframe = dataframe
 
-                # If slicing was specified, then we slice the dataframe first.
-                if len(self.sliceby) > 0:
-                    groupattrs = self.sliceby + self.compare
-                    groupby = summ_dataframe.groupby(groupattrs)
-                    sliceop = SLICE_OPS[self.sliceop]
-                    summ_dataframe = sliceop(groupby)
-                    summ_dataframe.reset_index(inplace=True)
-
-                if len(self._crossaggover) > 0:
-                    summ_dataframe = cross_aggregate(
-                        dataframe=summ_dataframe,
-                        index=None,
-                        compare=self.compare,
-                        targetval=self.targetval,
-                        crossaggover=self._crossaggover,
-                        crossaggpairs=self._compareorder,
-                        crossaggmode=self._crossaggmode,
-                    )
+            # If slicing was specified, then we slice the dataframe first.
+            if len(self.sliceby) > 0:
+                groupattrs = self.sliceby + self.compare
+                groupby = dataframe.groupby(groupattrs)
+                sliceop = SLICE_OPS[self.sliceop]
+                dataframe = sliceop(groupby)
+                dataframe.reset_index()
 
+            if self._summary is None:
                 self._summary = summarize(
-                    dataframe=summ_dataframe,
+                    dataframe=dataframe,
                     summarize=self.summarize,
                     compare=self.compare,
                     summode=self.summode,
                 )
             summarydict = dict((k, represent(v)) for (k, v) in unpackdict(self._summary).items())
 
         if len(self.plot) > 0:
             figsize = (len(self.plot) * self.plotsize[0], self.plotsize[1])
             self._figure = plt.figure(figsize=figsize)
-            formatdict = dict(**self.partvals)
+            formatdict = dict(**self.groupby)
             formatdict.update(summarydict)
             title = "\n".join(self.titleformat) % formatdict
             title = replace_keywords(title, keyword_replacements)
             plt.rc("text", usetex=self.usetex)
-            if not title.isspace():
-                self._figure.suptitle(title, fontsize=self.fontsize * 0.9)
-            subplots = self._figure.subplots(nrows=1, ncols=len(self.plot))
-            assert isinstance(subplots, np.ndarray) or isinstance(subplots, plt.Axes)
-            axes: NDArray = np.array([subplots]) if isinstance(subplots, plt.Axes) else subplots.flatten()
+            self._figure.suptitle(title, fontsize=self.fontsize * 1.2)
+            axes: plt.Axes = self._figure.subplots(nrows=1, ncols=len(self.plot))
+            if len(self.plot) == 1:
+                axes = np.array([axes])
+            axes = axes.flatten()
             colors = dict((x.split(":")[0], x.split(":")[1]) for x in self._colors) if len(self._colors) > 0 else None
 
             for i, plotspec in enumerate(self.plot):
                 plottype, target = parseplotspec(plotspec)
 
                 # Axes style.
                 axes[i].spines["top"].set_visible(False)
                 axes[i].spines["right"].set_visible(False)
                 axes[i].tick_params(axis="both", which="major", labelsize=self.fontsize)
 
-                if self.xlogscale[i]:
-                    axes[i].set_xscale("log")
-                if self.ylogscale[i]:
-                    axes[i].set_yscale("log")
-
-                if self.xtickfmt[i] == TickFormat.PERCENT:
-                    axes[i].xaxis.set_major_formatter(PercentFormatter(xmax=1.0, decimals=0))
-                elif self.xtickfmt[i] == TickFormat.ENG:
-                    axes[i].xaxis.set_major_formatter(EngFormatter(places=0, sep=""))
-                if self.ytickfmt[i] == TickFormat.PERCENT:
-                    axes[i].yaxis.set_major_formatter(PercentFormatter(xmax=1.0, decimals=0))
-                elif self.ytickfmt[i] == TickFormat.ENG:
-                    axes[i].yaxis.set_major_formatter(EngFormatter(places=0, sep=""))
-
                 if plottype == PlotType.LINE:
+
                     if self._index is None:
                         raise ValueError("An index must be specified when plotting line plots.")
-                    if self._view is None:
-                        raise ValueError(
-                            "An aggregate view must be generated for a line plot by specifying a targetval and index."
-                        )
 
                     lineplot(
                         self._view,
                         index=self._index,
                         targetval=target[0],
                         summary=self._summary,
                         compare=self._compare,
@@ -1183,17 +863,17 @@
                         labelformat=self._labelformat,
                         aggmode=self._aggmode,
                         keyword_replacements=keyword_replacements,
                         axes=axes[i],
                         fontsize=self.fontsize,
                         annotations=self._annotations[i],
                         dontcompare=self._dontcompare[i],
-                        linemarker=self._linemarker[i],
                     )
                 elif plottype == PlotType.BAR:
+
                     if self._summary is None:
                         raise ValueError("A bar plot can only be generated from a summary.")
 
                     barplot(
                         summary=self._summary,
                         targetval=target[0],
                         compare=self.compare,
@@ -1205,14 +885,15 @@
                         axes=axes[i],
                         fontsize=self.fontsize,
                         annotations=self._annotations[i],
                         dontcompare=self._dontcompare[i],
                     )
 
                 else:
+
                     if self._summary is None:
                         raise ValueError("A dot plot can only be generated from a summary.")
 
                     if len(target) != 2:
                         raise ValueError(
                             "A dot plot must be specified with two targets. One for the x-axis and one for the y-axis."
                         )
@@ -1229,14 +910,28 @@
                         keyword_replacements=keyword_replacements,
                         axes=axes[i],
                         fontsize=self.fontsize,
                         annotations=self._annotations[i],
                         dontcompare=self._dontcompare[i],
                     )
 
+                if self.xlogscale[i]:
+                    axes[i].set_xscale("log")
+                if self.ylogscale[i]:
+                    axes[i].set_yscale("log")
+
+                if self.xtickfmt[i] == TickFormat.PERCENT:
+                    axes[i].xaxis.set_major_formatter(PercentFormatter(xmax=1.0))
+                elif self.xtickfmt[i] == TickFormat.ENG:
+                    axes[i].xaxis.set_major_formatter(EngFormatter(places=0, sep=""))
+                if self.ytickfmt[i] == TickFormat.PERCENT:
+                    axes[i].yaxis.set_major_formatter(PercentFormatter(xmax=1.0))
+                elif self.ytickfmt[i] == TickFormat.ENG:
+                    axes[i].yaxis.set_major_formatter(EngFormatter(places=0, sep=""))
+
             if self._legend:
                 self._figure.subplots_adjust(bottom=0.25)
                 lines, labels = self._figure.axes[0].get_legend_handles_labels()
                 self._figure.legend(
                     lines,
                     labels,
                     loc="upper center",
```

### Comparing `datascope-experiments-0.0.81/datascope/experiments/scenarios/__init__.py` & `datascope-experiments-0.0.9/datascope/experiments/scenarios/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,43 +3,39 @@
     Study,
     Report,
     Backend,
     Queue as QueueProtocol,
     attribute,
     result,
     get_scenario_runner,
-    add_dynamic_arguments,
     DEFAULT_RESULTS_PATH,
     DEFAULT_RESULTS_SCENARIOS_PATH,
     DEFAULT_REPORTS_PATH,
     DEFAULT_STUDY_PATH,
     DEFAULT_BACKEND,
     DEFAULT_SLURM_JOBTIME,
     DEFAULT_SLURM_JOBMEMORY,
 )
 from .label_repair import LabelRepairScenario
 from .data_discard import DataDiscardScenario
 from .compute_time import ComputeTimeScenario
-from .marginal_contribution import MarginalContributionScenario
 
 __all__ = [
     "Scenario",
     "Study",
     "Report",
     "Backend",
     "QueueProtocol",
     "attribute",
     "result",
     "get_scenario_runner",
-    "add_dynamic_arguments",
     "DEFAULT_RESULTS_PATH",
     "DEFAULT_RESULTS_SCENARIOS_PATH",
     "DEFAULT_REPORTS_PATH",
     "DEFAULT_STUDY_PATH",
     "DEFAULT_BACKEND",
     "DEFAULT_SLURM_JOBTIME",
     "DEFAULT_SLURM_JOBMEMORY",
     "LabelRepairScenario",
     "DataDiscardScenario",
     "ComputeTimeScenario",
-    "MarginalContributionScenario",
 ]
```

### Comparing `datascope-experiments-0.0.81/datascope/experiments/scenarios/base.py` & `datascope-experiments-0.0.9/datascope/experiments/scenarios/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import argparse
 import collections.abc
 import datetime
 import gevent
 import gevent.signal
 import logging
 import logging.handlers
 import numpy as np
@@ -23,15 +22,15 @@
 import yaml
 import zerorpc
 
 from abc import ABC, abstractmethod
 from enum import Enum
 from glob import glob
 from inspect import signature
-from io import TextIOBase, StringIO, BytesIO, SEEK_END
+from io import TextIOBase, StringIO, SEEK_END
 from itertools import product
 from logging import Logger
 from matplotlib.figure import Figure
 from multiprocessing import Process, Queue as MultiprocessingQueue
 from numpy import ndarray
 from pandas import DataFrame
 from ray.util.multiprocessing import Pool
@@ -56,20 +55,23 @@
     overload,
     Union,
     Protocol,
 )
 
 
 class Queue(Protocol):
-    def get(self, block: bool = True, timeout: Optional[float] = None) -> Any: ...
+    def get(self, block: bool = True, timeout: Optional[float] = None) -> Any:
+        ...
 
-    def put(self, item: Any, block: bool = True, timeout: Optional[float] = None) -> None: ...
+    def put(self, item: Any, block: bool = True, timeout: Optional[float] = None) -> None:
+        ...
 
 
 class PropertyTag(property):
+
     domain: Optional[Iterable] = None
 
     @classmethod
     def get_properties(cls: Type[property], target: object) -> Dict[str, property]:
         res: Dict[str, property] = {}
         for name in dir(target):
             if hasattr(target, name):
@@ -82,15 +84,15 @@
 class attribute(PropertyTag):
     def __init__(
         self,
         fget: Optional[Callable[[Any], Any]] = None,
         fset: Optional[Callable[[Any, Any], None]] = None,
         fdel: Optional[Callable[[Any], None]] = None,
         doc: Optional[str] = None,
-        domain: Optional[Union[Iterable, Dict]] = None,
+        domain: Optional[Iterable] = None,
     ) -> None:
         super().__init__(fget, fset, fdel, doc)
         self.domain = domain
 
     def __call__(
         self,
         fget: Optional[Callable[[Any], Any]] = None,
@@ -111,14 +113,18 @@
     __isattribute__ = True
 
 
 class result(PropertyTag):
     __isresult__ = True
 
 
+# def extract_simpletype(target: object) -> type:
+#     pass
+
+
 def extract_enumtype(target: object) -> Optional[Type[Enum]]:
     if isinstance(target, type) and issubclass(target, Enum):
         return target
     else:
         origin = get_origin(target)
         if origin is not None:
             for arg in get_args(target):
@@ -149,15 +155,15 @@
 
 
 def get_property_domain(target: object, name: str) -> List[Any]:
     prop, getter = get_property_and_getter(target, name)
     sign = signature(getter)
     enum = extract_enumtype(sign.return_annotation)
     if isinstance(prop, PropertyTag) and prop.domain is not None:
-        return list(prop.domain.keys()) if isinstance(prop.domain, dict) else list(prop.domain)
+        return list(prop.domain)
     elif sign.return_annotation is bool:
         return [False, True]
     elif enum is None:
         return [None]
     else:
         return list(enum.__members__.values())
 
@@ -201,88 +207,14 @@
         value = [value]
     if ignore_none:
         return target_value is None or value == [None] or target_value in value
     else:
         return target_value in value
 
 
-def make_type_parser(target: Optional[type]) -> Callable[[str], Any]:
-    def parser(source: str) -> Any:
-        if target is None:
-            return source
-        result: Any = source
-        if issubclass(target, bool):
-            result = result in ["True", "true", "T", "t", "Yes", "yes", "y"]
-        elif issubclass(target, int):
-            result = int(result)
-        elif issubclass(target, float):
-            result = float(result)
-        elif issubclass(target, Enum):
-            result = target(result)
-        return result
-
-    return parser
-
-
-def add_dynamic_arguments(
-    parser: argparse.ArgumentParser,
-    targets: Iterable[type],
-    all_iterable: bool = False,
-    single_instance: bool = False,
-) -> None:
-    attribute_domains: Dict[str, Set[Any]] = {}
-    attribute_helpstrings: Dict[str, Optional[str]] = {}
-    attribute_types: Dict[str, Optional[type]] = {}
-    attribute_defaults: Dict[str, Optional[Any]] = {}
-    attribute_isiterable: Dict[str, bool] = {}
-
-    for cls in targets:
-        # Extract domain of scenario.
-        props = attribute.get_properties(cls)
-        domain = dict((name, set(get_property_domain(cls, name))) for name in props.keys())
-
-        # Include the new domain into the total domain.
-        for name, values in domain.items():
-            attribute_domains.setdefault(name, set()).update(values)
-
-        # Extract types of the scenario attributes.
-        types = dict((name, get_property_type(cls, name)) for name in props.keys())
-        attribute_types.update(types)
-
-        # Extract helpstrings of the scenario attributes.
-        helpstrings = dict((name, get_property_helpstring(cls, name)) for name in props.keys())
-        attribute_helpstrings.update(helpstrings)
-
-        # Extract types of the scenario attributes.
-        defaults = dict((name, get_property_default(cls, name)) for name in props.keys())
-        attribute_defaults.update(defaults)
-
-        # Set all attributes to be iterable when passed to get_instances.
-        isiterable = dict((name, True if all_iterable else get_property_isiterable(cls, name)) for name in props.keys())
-        attribute_isiterable.update(isiterable)
-
-    for name in attribute_domains:
-        default = attribute_defaults[name]
-        attribute_domain: Optional[List] = [x.value if isinstance(x, Enum) else x for x in attribute_domains[name]]
-        if attribute_domain == [None]:
-            attribute_domain = None
-        helpstring = attribute_helpstrings[name] or ("Scenario " + name + ".")
-        if default is None:
-            helpstring += " Default: [all]" if not single_instance else ""
-        else:
-            helpstring += " Default: %s" % str(default)
-        parser.add_argument(
-            "--%s" % name.replace("_", "-"),
-            help=helpstring,
-            type=make_type_parser(attribute_types[name]),
-            choices=attribute_domain,
-            nargs=(1 if single_instance else "+") if attribute_isiterable[name] else None,  # type: ignore
-        )
-
-
 def save_dict(source: Dict[str, Any], dirpath: str, basename: str, saveonly: Optional[Sequence[str]] = None) -> None:
     basedict: Dict[str, Any] = dict((k, v) for (k, v) in source.items() if type(v) in [int, float, bool, str])
     basedict.update(dict((k, v.value) for (k, v) in source.items() if isinstance(v, Enum)))
     if len(basedict) > 0:
         with open(os.path.join(dirpath, ".".join([basename, "yaml"])), "w") as f:
             yaml.safe_dump(basedict, f)
 
@@ -331,15 +263,15 @@
 
         if name == "":
             continue
 
         if ext == ".npy":
             res[name] = np.load(path)
         elif ext == ".csv":
-            res[name] = pd.read_csv(path, index_col=0)
+            res[name] = pd.read_csv(path)
         elif ext == ".yaml":
             with open(path) as f:
                 res[name] = yaml.safe_load(f)
         else:
             warnings.warn("File '%s' with unsupported extension '%s' will be ignored." % (path, ext))
 
     return res
@@ -422,16 +354,22 @@
             cls.pbars[event.id].close()
             del cls.pbars[event.id]
             # Ensure that bars get redrawn properly after they reshuffle due to closure of one of them.
             cls.refresh()
 
 
 class Scenario(ABC):
+
     scenarios: Dict[str, Type["Scenario"]] = {}
-    attribute_names: Set[str] = set()
+    scenario_domains: Dict[str, Dict[str, Set[Any]]] = {}
+    attribute_domains: Dict[str, Set[Any]] = {}
+    attribute_helpstrings: Dict[str, Optional[str]] = {}
+    attribute_types: Dict[str, Optional[type]] = {}
+    attribute_defaults: Dict[str, Optional[Any]] = {}
+    attribute_isiterable: Dict[str, bool] = {}
     _scenario: Optional[str] = None
 
     def __init__(self, id: Optional[str] = None, logstream: Optional[TextIOBase] = None, **kwargs: Any) -> None:
         super().__init__()
         self._id = id if id is not None else "".join(random.choices(string.ascii_lowercase + string.digits, k=10))
         self._logstream = logstream if logstream is not None else StringIO()
         self._progress = Progress(id=self._id)
@@ -444,18 +382,38 @@
         # Register scenario under the given name.
         cls._scenario = id
         Scenario.scenarios[id] = cls
         assert isinstance(Scenario.scenario, PropertyTag)
         assert isinstance(Scenario.scenario.domain, set)
         Scenario.scenario.domain.add(id)
 
-        # Extract scenario attribute names.
+        # Extract domain of scenario.
         props = attribute.get_properties(cls)
-        cls.attribute_names = set(props.keys())
-        Scenario.attribute_names.update(cls.attribute_names)
+        domain = dict((name, set(get_property_domain(cls, name))) for name in props.keys())
+        Scenario.scenario_domains[id] = domain
+
+        # Include the new domain into the total domain.
+        for name, values in domain.items():
+            Scenario.attribute_domains.setdefault(name, set()).update(values)
+
+        # Extract types of the scenario attributes.
+        types = dict((name, get_property_type(cls, name)) for name in props.keys())
+        Scenario.attribute_types.update(types)
+
+        # Extract helpstrings of the scenario attributes.
+        helpstrings = dict((name, get_property_helpstring(cls, name)) for name in props.keys())
+        Scenario.attribute_helpstrings.update(helpstrings)
+
+        # Extract types of the scenario attributes.
+        defaults = dict((name, get_property_default(cls, name)) for name in props.keys())
+        Scenario.attribute_defaults.update(defaults)
+
+        # Set all attributes to be iterable when passed to get_instances.
+        isiterable = dict((k, True) for k in props.keys())
+        Scenario.attribute_isiterable.update(isiterable)
 
     def run(self, progress_bar: bool = True, console_log: bool = True) -> None:
         # Set up logging.
         formatter = logging.Formatter("[%(asctime)s] [%(levelname)s] %(message)s")
         fh = logging.StreamHandler(self._logstream)
         fh.setFormatter(formatter)
         self.logger.addHandler(fh)
@@ -541,23 +499,23 @@
         if cls == Scenario:
             for id, scenario in Scenario.scenarios.items():
                 if kwargs.get("scenario", None) is None or id in kwargs["scenario"]:
                     for instance in scenario.get_instances(**kwargs):
                         yield instance
         else:
             domains = []
-            names = cls.attribute_names
+            names = Scenario.attribute_domains.keys()
             for name in names:
                 if name in kwargs and kwargs[name] is not None:
                     domain = kwargs[name]
                     if not isinstance(domain, Iterable):
                         domain = [domain]
                     domains.append(list(domain))
                 else:
-                    domains.append(get_property_domain(cls, name))
+                    domains.append(list(Scenario.attribute_domains[name]))
             for values in product(*domains):
                 attributes = dict((name, value) for (name, value) in zip(names, values) if value is not None)
                 if cls.is_valid_config(**attributes):
                     yield cls(**attributes)
 
     @classmethod
     def is_valid_config(cls, **attributes: Any) -> bool:
@@ -695,15 +653,14 @@
 def get_scenario_runner(
     queue: Optional[Queue] = None,
     catch_exceptions: bool = True,
     progress_bar: bool = True,
     console_log: bool = True,
     rerun: bool = False,
     pickled_queue: bool = False,
-    job_memory: Optional[str] = None,
 ) -> Callable[[Scenario], Scenario]:
     def _scenario_runner(scenario: Scenario) -> Scenario:
         try:
             scenario.progress.queue = queue
             scenario.progress.pickled = pickled_queue
             scenario.logger.setLevel(logging.DEBUG)
             qh: Optional[logging.Handler] = None
@@ -717,23 +674,14 @@
                 queue.put(payload)
             elif console_log:
                 formatter = logging.Formatter("[%(asctime)s] [%(levelname)s] [%(name)s] %(message)s")
                 ch = logging.StreamHandler(sys.stdout)
                 ch.setFormatter(formatter)
                 scenario.logger.addHandler(ch)
 
-            # Quickly consume a 70% of the given amount of memory for 10 seconds.
-            if job_memory is not None:
-                suffixes = {"G": 1024**3, "M": 1024**2, "K": 1024}
-                size = int(float(job_memory[:-1]) * suffixes[job_memory[-1]] * 0.7)
-                with BytesIO() as buffer:
-                    buffer.write(bytearray(os.urandom(size)))
-                    buffer.seek(0)
-                    time.sleep(10)
-
             if rerun or not scenario.completed:
                 if queue is not None:
                     scenario.run(progress_bar=progress_bar, console_log=False)
                 else:
                     with logging_redirect_tqdm(loggers=[scenario.logger]):
                         scenario.run(progress_bar=progress_bar, console_log=False)
             else:
@@ -810,15 +758,14 @@
     ) -> None:
         self._scenarios = scenarios
         self._id = id if id is not None else datetime.datetime.now().strftime("Study-%Y-%m-%d-%H-%M-%S")
         self._outpath = outpath
         self._scenario_path_format = scenario_path_format
         self._logstream = logstream if logstream is not None else StringIO()
         self._logger = logging.getLogger(self._id)
-        self._logger.setLevel(logging.DEBUG)
         self._verify_scenario_path(scenario_path_format, scenarios)
 
     @staticmethod
     def _status_monitor(
         queue: Queue,
         logger: Logger,
         study_queue: Optional[Queue] = None,
@@ -851,22 +798,20 @@
         console_log: bool = True,
         backend: Backend = DEFAULT_BACKEND,
         ray_address: Optional[str] = None,
         ray_numprocs: Optional[int] = None,
         slurm_jobtime: Optional[str] = DEFAULT_SLURM_JOBTIME,
         slurm_jobmemory: Optional[str] = DEFAULT_SLURM_JOBMEMORY,
         slurm_constraint: Optional[str] = None,
-        slurm_partition: Optional[str] = None,
-        slurm_maxjobs: Optional[int] = None,
-        slurm_args: Optional[str] = None,
         eventstream_host_ip: Optional[str] = None,
         eventstream_host_port: Optional[int] = None,
         eagersave: bool = True,
         **kwargs: Any
     ) -> None:
+
         # Set up logging.
         formatter = logging.Formatter("[%(asctime)s] [%(levelname)s] [%(name)s] %(message)s")
         fh = logging.StreamHandler(self._logstream)
         fh.setFormatter(formatter)
         self.logger.addHandler(fh)
         ch: Optional[logging.Handler] = None
         if console_log:
@@ -922,22 +867,23 @@
                     scenarios.append(scenario)
                     if pbar is not None:
                         pbar.update(1)
                     if eagersave:
                         self.save_scenario(scenario)
 
             elif backend == Backend.SLURM:
+
                 # If the host port was not specified, we look for the first free port.
                 if eventstream_host_port is None:
                     eventstream_host_port = get_free_port(DEFAULT_EVENTSTREAM_HOST_PORT)
 
                 # Set up the process that will host the queue RPC server.
                 # Reference: https://stackoverflow.com/a/21146917
                 def serve(queue: Queue) -> None:
-                    server = zerorpc.Server(queue, heartbeat=45)
+                    server = zerorpc.Server(queue, heartbeat=5)
                     assert eventstream_host_port is not None
                     server.bind("tcp://0.0.0.0:%d" % eventstream_host_port)
 
                     def stop_routine():
                         server.stop()
 
                     def stop_handler(number, frame):
@@ -958,68 +904,45 @@
                 monitor.start()
 
                 if eventstream_host_ip is None:
                     eventstream_host_ip = get_ip()
                 address = "tcp://%s:%d" % (eventstream_host_ip, eventstream_host_port)
                 self.logger.info("Status event monitor listening on " + address)
 
-                try:
-                    # Create a batch job on slurm for every scenario.
-                    scenarios_pending = len(self.scenarios)
-                    scenarios_running = 0
-                    for scenario in self.scenarios:
-                        scenarios_pending -= 1
-                        if scenario.completed:
-                            if pbar is not None:
-                                pbar.update(1)
-                        else:
-                            path = self.save_scenario(scenario)
-                            logpath = os.path.join(path, "slurm.log")
-                            run_command = "python -m datascope.experiments run-scenario -o %s -e %s -m %s" % (
-                                path,
-                                address,
-                                slurm_jobmemory,
-                            )
-                            slurm_command = "sbatch --job-name=%s" % self.id
-                            slurm_command += " --time=%s" % slurm_jobtime
-                            slurm_command += " --mem-per-cpu=%s" % slurm_jobmemory
-                            if slurm_constraint is not None:
-                                slurm_command += " --constraint=%s" % slurm_constraint
-                            if slurm_partition is not None:
-                                slurm_command += " --partition=%s" % slurm_partition
-                            if slurm_args is not None:
-                                slurm_command += " %s " % slurm_args
-                            slurm_command += " --output=%s" % logpath
-                            slurm_command += ' --wrap="%s"' % run_command
-                            result = subprocess.run(slurm_command, capture_output=True, shell=True)
-                            if result.returncode != 0:
-                                raise RuntimeError(
-                                    "Slurm sbatch command gave a non-zero return code. \nstdout:\n%r\nstderr:\n%r\n"
-                                    % (result.stdout, result.stderr)
-                                )
-                            scenarios_running += 1
-
-                        # Check if we need to wait for jobs to finish. We do that either when
-                        # the maximum number of allowed jobs has been reached
-                        # or if all jobs have been submitted but not all have finished yet.
-                        while (slurm_maxjobs is not None and scenarios_running > slurm_maxjobs) or (
-                            scenarios_pending <= 0 and scenarios_running > 0
-                        ):
-                            scenario_event: ScenarioEvent = study_queue.get()
-                            if scenario_event.type == ScenarioEvent.Type.COMPLETED:
-                                scenarios_running -= 1
-                                if pbar is not None:
-                                    pbar.update(1)
-
-                except (Exception, KeyboardInterrupt) as e:
-                    # Make sure to cancel all submitted slurm jobs in case of an exception or keyboard interrupt.
-                    self.logger.info("Running: scancel --name=%s" % self.id)
-                    subprocess.run(["scancel", "--name=%s" % self.id])
-                    self.logger.info("Slurm jobs canceled.")
-                    raise e
+                # Create a batch job on slurm for every scenario.
+                scenarios_running = len(self.scenarios)
+                for scenario in self.scenarios:
+                    if scenario.completed:
+                        scenarios_running -= 1
+                        if pbar is not None:
+                            pbar.update(1)
+                        continue
+                    path = self.save_scenario(scenario)
+                    logpath = os.path.join(path, "slurm.log")
+                    run_command = "python -m datascope.experiments run-scenario -o %s -e %s" % (path, address)
+                    slurm_command = "sbatch --job-name=datascope-experiment"
+                    slurm_command += " --time=%s" % slurm_jobtime
+                    slurm_command += " --mem-per-cpu=%s" % slurm_jobmemory
+                    if slurm_constraint is not None:
+                        slurm_command += " --constraint=%s" % slurm_constraint
+                    slurm_command += " --output=%s" % logpath
+                    slurm_command += ' --wrap="%s"' % run_command
+                    result = subprocess.run(slurm_command, capture_output=True, shell=True)
+                    if result.returncode != 0:
+                        raise RuntimeError(
+                            "Slurm sbatch command resulted in non-zero return code. \nstdout:\n%r\nstderr:\n%r\n"
+                            % (result.stdout, result.stderr)
+                        )
+
+                while scenarios_running > 0:
+                    scenario_event: ScenarioEvent = study_queue.get()
+                    if scenario_event.type == ScenarioEvent.Type.COMPLETED:
+                        scenarios_running -= 1
+                        if pbar is not None:
+                            pbar.update(1)
 
                 scenarios = Study.load_scenarios(self.path)
 
             self._scenarios = scenarios
 
             if pbar is not None:
                 pbar.close()
@@ -1056,14 +979,15 @@
         replacements = dict((name, get_property_value(scenario, name)) for name in attributes)
         exppath = self._scenario_path_format.format_map(replacements)
         full_exppath = os.path.join(self.path, "scenarios", exppath)
         scenario.save(full_exppath)
         return full_exppath
 
     def save(self, save_scenarios: bool = True) -> None:
+
         # Make directory that will contain the study.
         os.makedirs(self.path, exist_ok=True)
 
         # Write a marker file.
         markerpath = os.path.join(self.path, "study.yml")
         with open(markerpath, "w") as f:
             yaml.safe_dump({"id": self.id, "scenario_path_format": self.scenario_path_format}, f)
@@ -1080,14 +1004,24 @@
 
         # Iterate over all scenarios and compute their target paths.
         # attributes = re.findall(r"\{(.*?)\}", scenario_path)
         # scenario_paths: Set[str] = set()
         if save_scenarios:
             for scenario in self.scenarios:
                 self.save_scenario(scenario)
+                # replacements = dict((name, get_property_value(scenario, name)) for name in attributes)
+                # exppath = scenario_path.format_map(replacements)
+                # if exppath in scenario_paths:
+                #     raise ValueError(
+                #         "Provided scenario_path does not produce unique paths. The path '%s' caused a conflict."
+                #         % exppath
+                #     )
+                # scenario_paths.add(exppath)
+                # full_exppath = os.path.join(self.path, "scenarios", exppath)
+                # scenario.save(full_exppath)
 
     @classmethod
     def load_scenarios(cls, path: str) -> List[Scenario]:
         # Load all scenarios.
         scenarios: List[Scenario] = []
         for attpath in glob(os.path.join(path, "**/attributes.yaml"), recursive=True):
             exppath = os.path.dirname(attpath)
@@ -1167,20 +1101,20 @@
 
     @property
     def completed(self) -> bool:
         return all(exp.completed for exp in self.scenarios if isinstance(exp, Scenario))
 
     @property
     def scenarios(self) -> Table[Scenario]:
-        attributes = sorted(Scenario.attribute_names)
+        attributes = list(Scenario.attribute_domains.keys())
         return Table[Scenario](self._scenarios, attributes, "id")
 
     @property
     def dataframe(self) -> DataFrame:
-        df = pd.concat([s.dataframe.assign(scenario=s.scenario, id=s.id) for s in self.scenarios], ignore_index=True)
+        df = pd.concat([scenario.dataframe for scenario in self.scenarios], ignore_index=True)
         df.sort_index(inplace=True)
         return df
 
     def get_scenarios(self, **attributes: Dict[str, Any]) -> Sequence[Scenario]:
         res: List[Scenario] = []
         for exp in self.scenarios:
             if all(has_attribute_value(exp, name, value) for (name, value) in attributes.items() if hasattr(exp, name)):
@@ -1199,120 +1133,140 @@
     if isinstance(x, Enum):
         return str(x.value)
     else:
         return str(x)
 
 
 class Report(ABC):
+
     reports: Dict[str, Type["Report"]] = {}
+    report_domains: Dict[str, Dict[str, Set[Any]]] = {}
+    attribute_domains: Dict[str, Set[Any]] = {}
+    attribute_helpstrings: Dict[str, Optional[str]] = {}
+    attribute_types: Dict[str, Optional[type]] = {}
+    attribute_defaults: Dict[str, Optional[Any]] = {}
+    attribute_isiterable: Dict[str, bool] = {}
     _report: Optional[str] = None
 
     def __init__(
-        self,
-        study: Study,
-        dataframe: DataFrame,
-        id: Optional[str] = None,
-        partvals: Optional[Dict[str, Any]] = None,
-        **kwargs: Any
+        self, study: Study, id: Optional[str] = None, groupby: Optional[Dict[str, Any]] = None, **kwargs: Any
     ) -> None:
         super().__init__()
         self._study = study
-        self._dataframe = dataframe
         self._id = id if id is not None else "".join(random.choices(string.ascii_lowercase + string.digits, k=10))
-        self._partvals: Dict[str, Any] = {} if partvals is None else partvals
+        self._groupby: Dict[str, Any] = {} if groupby is None else groupby
 
     def __init_subclass__(cls: Type["Report"], id: str) -> None:
         cls._report = id
         cls.reports[id] = cls
 
+        # Extract domain of scenario.
+        props = attribute.get_properties(cls)
+        domain = dict((name, set(get_property_domain(cls, name))) for name in props.keys())
+        Report.report_domains[id] = domain
+
+        # Include the new domain into the total domain.
+        for name, values in domain.items():
+            Report.attribute_domains.setdefault(name, set()).update(values)
+
+        # Extract types of the scenario attributes.
+        types = dict((name, get_property_type(cls, name)) for name in props.keys())
+        Report.attribute_types.update(types)
+
+        # Extract helpstrings of the scenario attributes.
+        helpstrings = dict((name, get_property_helpstring(cls, name)) for name in props.keys())
+        Report.attribute_helpstrings.update(helpstrings)
+
+        # Extract types of the scenario attributes.
+        defaults = dict((name, get_property_default(cls, name)) for name in props.keys())
+        Report.attribute_defaults.update(defaults)
+
+        # Specify if attributes should be iterable when passed to get_instances.
+        Report.attribute_isiterable = dict((name, get_property_isiterable(cls, name)) for name in props.keys())
+        Report.attribute_isiterable["report"] = True  # We hard code that we allow multiple report argument values.
+
     @attribute
     def report(self) -> str:
         if self._report is None:
             raise ValueError("Cannot call this on an abstract class instance.")
         return self._report
 
     @attribute
     def id(self) -> str:
         """A unique identifier of the report."""
         return self._id
 
     @property
-    def partvals(self) -> Dict[str, Any]:
-        return self._partvals
+    def groupby(self) -> Dict[str, Any]:
+        return self._groupby
 
     @property
     def study(self) -> Study:
         return self._study
 
-    @property
-    def dataframe(self) -> DataFrame:
-        return self._dataframe
-
     @classmethod
     def is_valid_config(cls, **attributes: Any) -> bool:
         return True
 
     @abstractmethod
     def generate(self) -> None:
         raise NotImplementedError()
 
     def save(
         self,
         path: Optional[str] = None,
-        use_partvals: bool = True,
+        use_groupby: bool = True,
         use_id: bool = False,
         use_subdirs: bool = False,
         saveonly: Optional[Sequence[str]] = None,
     ) -> None:
         if path is None:
             path = os.path.join(self._study.path, "reports")
         basename = "report"
         if use_subdirs:
-            if use_partvals:
-                partvals = ["%s=%s" % (str(key), str(self._partvals[key])) for key in sorted(self.partvals.keys())]
-                path = os.path.join(path, *partvals)
+            if use_groupby:
+                groupby = ["%s=%s" % (str(key), str(self._groupby[key])) for key in sorted(self.groupby.keys())]
+                path = os.path.join(path, *groupby)
             if use_id:
                 path = os.path.join(path, self._id)
             if os.path.splitext(path)[1] != "":
                 raise ValueError("The provided path '%s' is not a valid directory path." % path)
         else:
-            if use_partvals:
-                partvals = [self._partvals[key] for key in sorted(self.partvals.keys())]
+            if use_groupby:
+                groupby = [self._groupby[key] for key in sorted(self.groupby.keys())]
                 basename = "_".join(
                     [basename]
-                    + ["%s=%s" % (str(key), stringify(self._partvals[key])) for key in sorted(self.partvals.keys())]
+                    + ["%s=%s" % (str(key), stringify(self._groupby[key])) for key in sorted(self.groupby.keys())]
                 )
             if use_id:
                 basename = basename + "_id=" + self._id
 
         os.makedirs(path, exist_ok=True)
 
         # Save results as separate files.
         props = result.get_properties(type(self))
         results = dict((name, prop.fget(self) if prop.fget is not None else None) for (name, prop) in props.items())
         save_dict(results, path, basename, saveonly=saveonly)
 
     @classmethod
     def get_instances(
-        cls: Type["Report"], study: Study, partby: Optional[Sequence[str]], **kwargs: Any
+        cls: Type["Report"], study: Study, groupby: Optional[Sequence[str]], **kwargs: Any
     ) -> Iterable["Report"]:
         if cls == Report:
             for id, report in Report.reports.items():
                 if kwargs.get("report", None) is None or id in kwargs["report"]:
-                    for instance in report.get_instances(study=study, partby=partby, **kwargs):
+                    for instance in report.get_instances(study=study, groupby=groupby, **kwargs):
                         yield instance
         else:
             # If grouping attributes were not specified, then we return only a single instance.
-            if partby is None or len(partby) == 0:
-                yield cls(study=study, dataframe=study.dataframe, **kwargs)
+            if groupby is None or len(groupby) == 0:
+                yield cls(study=study, **kwargs)
 
             else:
                 # Find distinct grouping attribute assignments.
                 all_values: List[Tuple] = []
-                partitioned = study.dataframe.groupby(partby)  # type: ignore
                 if len(study.scenarios) > 0:
-                    all_values = list(partitioned.groups.keys())
+                    all_values = list(study.dataframe.groupby(groupby).groups.keys())
 
                 for values in all_values:
-                    dataframe = partitioned.get_group(values)
-                    partvals = dict((k, v) for (k, v) in zip(partby, values))
-                    yield cls(study=study, dataframe=dataframe, partvals=partvals, **kwargs)
+                    groupby_values = dict((k, v) for (k, v) in zip(groupby, values))
+                    yield cls(study=study, groupby=groupby_values, **kwargs)
```

### Comparing `datascope-experiments-0.0.81/datascope/experiments/scenarios/compute_time.py` & `datascope-experiments-0.0.9/datascope/experiments/scenarios/compute_time.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,27 +6,24 @@
 from pandas import DataFrame
 from time import process_time_ns
 from typing import Any, Optional, Dict
 
 from .base import Scenario, attribute, result
 from .datascope_scenario import (
     RepairMethod,
-    ModelSpec,
-    MODEL_TYPES,
-    MODEL_KWARGS,
     IMPORTANCE_METHODS,
     MC_ITERATIONS,
     DEFAULT_SEED,
     DEFAULT_MODEL,
     DEFAULT_MC_TIMEOUT,
     KEYWORD_REPLACEMENTS,
     UtilityType,
 )
 from ..datasets import Dataset, DEFAULT_TRAINSIZE, DEFAULT_VALSIZE, DEFAULT_NUMFEATURES
-from ..pipelines import Pipeline, get_model
+from ..pipelines import Pipeline, ModelType, get_model
 
 DEFAULT_DATASET = "random"
 KEYWORD_REPLACEMENTS = {
     **KEYWORD_REPLACEMENTS,
     **{"trainsize": "Training Set Size", "valsize": "Validation Set Size", "numfeatures": "Number of Features"},
 }
 
@@ -34,15 +31,15 @@
 class ComputeTimeScenario(Scenario, id="compute-time"):
     def __init__(
         self,
         pipeline: str,
         method: RepairMethod,
         iteration: int,
         dataset: str = DEFAULT_DATASET,
-        model: ModelSpec = DEFAULT_MODEL,
+        model: ModelType = DEFAULT_MODEL,
         seed: int = DEFAULT_SEED,
         trainsize: int = DEFAULT_TRAINSIZE,
         valsize: int = DEFAULT_VALSIZE,
         numfeatures: int = DEFAULT_NUMFEATURES,
         mc_timeout: int = DEFAULT_MC_TIMEOUT,
         importance_cputime: Optional[float] = None,
         **kwargs: Any
@@ -70,26 +67,26 @@
         return result and super().is_valid_config(**attributes)
 
     @attribute(domain=[DEFAULT_DATASET])
     def dataset(self) -> str:
         """Dataset to use for training and validation."""
         return self._dataset
 
-    @attribute(domain=Pipeline.pipelines)
+    @attribute(domain=Pipeline.pipelines.keys())
     def pipeline(self) -> str:
         """Pipeline to use for feature extraction."""
         return self._pipeline
 
     @attribute
     def method(self) -> RepairMethod:
         """Method used to perform data repairs."""
         return self._method
 
     @attribute(domain=[None])
-    def model(self) -> ModelSpec:
+    def model(self) -> ModelType:
         """Model used to make predictions."""
         return self._model
 
     @attribute(domain=range(10))
     def iteration(self) -> int:
         """The ordinal number of the experiment repetition. Also serves as the random seed."""
         return self._iteration
@@ -138,54 +135,52 @@
                 timeout=[self.mc_timeout],
                 importance_cputime=[self.importance_cputime],
             )
         )
 
     @property
     def keyword_replacements(self) -> Dict[str, str]:
-        return {**KEYWORD_REPLACEMENTS, **Pipeline.summaries, **Dataset.summaries}
+        return {**KEYWORD_REPLACEMENTS, **Pipeline.summaries}
 
     def _run(self, progress_bar: bool = True, **kwargs: Any) -> None:
+
         # Load dataset.
         seed = self._seed + self._iteration
         dataset = Dataset.datasets[self.dataset](
             trainsize=self.trainsize, valsize=self.valsize, numfeatures=self.numfeatures, seed=seed
         )
         dataset.load()
         self.logger.debug(
             "Dataset '%s' loaded (trainsize=%d, valsize=%d).", self.dataset, dataset.trainsize, dataset.valsize
         )
 
         # Load the pipeline and process the data.
         pipeline = Pipeline.pipelines[self.pipeline].construct(dataset)
 
         # Initialize the model and utility.
-        model_type = MODEL_TYPES[self.model]
-        model_kwargs = MODEL_KWARGS[self.model]
-        model = get_model(model_type, **model_kwargs)
+        model = get_model(self.model)
         utility = SklearnModelAccuracy(model)
 
         # Compute importance scores and time it.
         importance_time_start = process_time_ns()
         n_units = dataset.units.shape[0]
         importance: Optional[ShapleyImportance] = None
         random = np.random.RandomState(seed=self._seed + self._iteration)
         if self.method == RepairMethod.RANDOM:
             list(random.rand(n_units))
         else:
             method = IMPORTANCE_METHODS[self.method]
             mc_iterations = MC_ITERATIONS[self.method]
             mc_preextract = RepairMethod.is_tmc_nonpipe(self.method)
+            provenance = np.array(np.nan)  # TODO: Remove this hack.
             importance = ShapleyImportance(
                 method=method,
                 utility=utility,
                 pipeline=pipeline,
                 mc_iterations=mc_iterations,
                 mc_timeout=self.mc_timeout,
                 mc_preextract=mc_preextract,
             )
-            importance.fit(dataset.X_train, dataset.y_train, dataset.metadata_train).score(
-                dataset.X_val, dataset.y_val, dataset.metadata_val
-            )
+            importance.fit(dataset.X_train, dataset.y_train, provenance=provenance).score(dataset.X_val, dataset.y_val)
         importance_time_end = process_time_ns()
         self._importance_cputime = (importance_time_end - importance_time_start) / 1e9
         self.logger.debug("Importance computed in: %s", str(timedelta(seconds=self._importance_cputime)))
```

### Comparing `datascope-experiments-0.0.81/datascope/experiments/scenarios/label_repair.py` & `datascope-experiments-0.0.9/datascope/experiments/scenarios/label_repair.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 from copy import deepcopy
 import numpy as np
 import pandas as pd
 
 from datascope.importance.common import (
-    JointUtility,
     SklearnModelAccuracy,
+    JointUtility,
     SklearnModelEqualizedOddsDifference,
-    SklearnModelRocAuc,
     Utility,
-    UtilityResult,
     compute_groupings,
 )
-from datascope.importance.importance import Importance
 from datascope.importance.shapley import ShapleyImportance
 from datetime import timedelta
-from numpy.typing import NDArray
 from time import process_time_ns
 from typing import Any, Iterable, List, Optional, Union, Dict
 
 from .base import attribute
 from .datascope_scenario import (
     DatascopeScenario,
     RepairMethod,
-    ModelSpec,
-    MODEL_TYPES,
-    MODEL_KWARGS,
     IMPORTANCE_METHODS,
     MC_ITERATIONS,
     DEFAULT_SEED,
     DEFAULT_CHECKPOINTS,
     DEFAULT_PROVIDERS,
     DEFAULT_MODEL,
     DEFAULT_REPAIR_GOAL,
@@ -37,25 +30,21 @@
     DEFAULT_NN_K,
     UtilityType,
     RepairGoal,
 )
 from ..datasets import (
     Dataset,
     BiasMethod,
-    BiasedNoisyLabelDataset,
-    NoisyLabelDataset,
-    AugmentableMixin,
-    TabularDatasetMixin,
-    ImageDatasetMixin,
+    BiasedDirtyLabelDataset,
+    DirtyLabelDataset,
     DEFAULT_TRAINSIZE,
     DEFAULT_VALSIZE,
     DEFAULT_TESTSIZE,
-    DEFAULT_CACHE_DIR,
 )
-from ..pipelines import Pipeline, FlattenPipeline, get_model, DistanceModelMixin
+from ..pipelines import Pipeline, ModelType, get_model
 
 
 DEFAULT_DIRTY_RATIO = 0.5
 DEFAULT_DIRTY_BIAS = 0.0
 KEYWORD_REPLACEMENTS = {
     "accuracy": "Accuracy",
     "accuracy_rel": "Relative Accuracy",
@@ -70,84 +59,75 @@
     def __init__(
         self,
         dataset: str,
         pipeline: str,
         method: RepairMethod,
         iteration: int,
         utility: UtilityType = UtilityType.ACCURACY,
-        model: ModelSpec = DEFAULT_MODEL,
-        postprocessor: Optional[str] = None,
+        model: ModelType = DEFAULT_MODEL,
         dirtyratio: float = DEFAULT_DIRTY_RATIO,
         dirtybias: float = DEFAULT_DIRTY_BIAS,
         seed: int = DEFAULT_SEED,
         trainsize: int = DEFAULT_TRAINSIZE,
         valsize: int = DEFAULT_VALSIZE,
         testsize: int = DEFAULT_TESTSIZE,
         mc_timeout: int = DEFAULT_MC_TIMEOUT,
         mc_tolerance: float = DEFAULT_MC_TOLERANCE,
         nn_k: int = DEFAULT_NN_K,
         checkpoints: int = DEFAULT_CHECKPOINTS,
         providers: int = DEFAULT_PROVIDERS,
         repairgoal: RepairGoal = DEFAULT_REPAIR_GOAL,
-        pipeline_cache_dir: str = DEFAULT_CACHE_DIR,
         evolution: Optional[pd.DataFrame] = None,
         importance_cputime: Optional[float] = None,
         **kwargs: Any
     ) -> None:
         kwargs.pop("biasmethod", None)
         super().__init__(
             dataset=dataset,
             pipeline=pipeline,
             method=method,
             utility=utility,
             iteration=iteration,
             model=model,
-            postprocessor=postprocessor,
             seed=seed,
             trainsize=trainsize,
             valsize=valsize,
             testsize=testsize,
             mc_timeout=mc_timeout,
             mc_tolerance=mc_tolerance,
             nn_k=nn_k,
             checkpoints=checkpoints,
             providers=providers,
             repairgoal=repairgoal,
             biasmethod=BiasMethod.Feature,
-            pipeline_cache_dir=pipeline_cache_dir,
             evolution=evolution,
             importance_cputime=importance_cputime,
             **kwargs
         )
         self._dirtyratio = dirtyratio
         self._dirtybias = dirtybias
 
     @classmethod
     def is_valid_config(cls, **attributes: Any) -> bool:
         result = True
         # if "method" in attributes:
         #     result = result and not RepairMethod.is_tmc_nonpipe(attributes["method"])
         if "dataset" in attributes:
             dataset_class = Dataset.datasets[attributes["dataset"]]
-            result = result and issubclass(dataset_class, NoisyLabelDataset)
+            result = result and issubclass(dataset_class, DirtyLabelDataset)
 
         if "repairgoal" not in attributes or attributes["repairgoal"] == RepairGoal.FAIRNESS:
             if "dataset" in attributes:
                 dataset = Dataset.datasets[attributes["dataset"]]()
-                result = result and isinstance(dataset, BiasedNoisyLabelDataset)
+                result = result and isinstance(dataset, BiasedDirtyLabelDataset)
         elif "repairgoal" in attributes and attributes["repairgoal"] == RepairGoal.ACCURACY:
             if "dataset" in attributes:
                 result = result and (attributes["dataset"] != "random")
             if "utility" in attributes:
-                result = result and attributes["utility"] in [UtilityType.ACCURACY, UtilityType.ROC_AUC]
-        if "method" in attributes and attributes["method"] == RepairMethod.KNN_Raw:
-            dataset_class = Dataset.datasets[attributes["dataset"]]
-            result = result and any(
-                issubclass(dataset_class, modality) for modality in [TabularDatasetMixin, ImageDatasetMixin]
-            )
+                result = result and attributes["utility"] == UtilityType.ACCURACY
         return result and super().is_valid_config(**attributes)
 
     @attribute
     def dirtyratio(self) -> float:
         """The proportion of examples that will have corrupted labels in label repair experiments."""
         return self._dirtyratio
 
@@ -158,33 +138,34 @@
 
     @property
     def keyword_replacements(self) -> Dict[str, str]:
         result = super().keyword_replacements
         return {**result, **KEYWORD_REPLACEMENTS}
 
     def _run(self, progress_bar: bool = True, **kwargs: Any) -> None:
+
         # Load dataset.
         seed = self._seed + self._iteration
         dataset = Dataset.datasets[self.dataset](
             trainsize=self.trainsize, valsize=self.valsize, testsize=self.testsize, seed=seed
         )
-        assert isinstance(dataset, NoisyLabelDataset)
+        assert isinstance(dataset, DirtyLabelDataset)
         dataset.load()
         self.logger.debug(
             "Dataset '%s' loaded (trainsize=%d, valsize=%d, testsize=%d).",
             self.dataset,
             dataset.trainsize,
             dataset.valsize,
             dataset.testsize,
         )
 
         # Compute sensitive feature groupings.
-        groupings_val: Optional[NDArray] = None
-        groupings_test: Optional[NDArray] = None
-        if isinstance(dataset, BiasedNoisyLabelDataset):
+        groupings_val: Optional[np.ndarray] = None
+        groupings_test: Optional[np.ndarray] = None
+        if isinstance(dataset, BiasedDirtyLabelDataset):
             groupings_val = compute_groupings(dataset.X_val, dataset.sensitive_feature)
             groupings_test = compute_groupings(dataset.X_test, dataset.sensitive_feature)
 
         # Create the dirty dataset and apply the data corruption.
         # dataset_dirty = deepcopy(dataset)
         # random = np.random.RandomState(seed=self._seed + self._iteration)
         # dirty_probs = [1 - self._dirtyratio, self._dirtyratio]
@@ -197,23 +178,18 @@
             probabilities = [float(i + 1) / dirty_providers for i in range(dirty_providers)]
             probabilities += [0.0 for _ in range(clean_providers)]
 
         if self.repairgoal == RepairGoal.ACCURACY:
             dataset_dirty = dataset.corrupt_labels(probabilities=probabilities)
             units_dirty = deepcopy(dataset_dirty.units_dirty)
         if self.repairgoal == RepairGoal.FAIRNESS:
-            assert isinstance(dataset, BiasedNoisyLabelDataset)
+            assert isinstance(dataset, BiasedDirtyLabelDataset)
             dataset_dirty = dataset.corrupt_labels_with_bias(probabilities=probabilities, groupbias=self.dirtybias)
             units_dirty = deepcopy(dataset_dirty.units_dirty)
 
-        if self.augment_factor > 0 and self.method != RepairMethod.KNN_Raw:
-            assert isinstance(dataset, AugmentableMixin) and isinstance(dataset_dirty, AugmentableMixin)
-            dataset.augment(factor=self.augment_factor, inplace=True)
-            dataset_dirty.augment(factor=self.augment_factor, inplace=True)
-
         # Load the pipeline and process the data.
         pipeline = Pipeline.pipelines[self.pipeline].construct(dataset)
         # X_train, y_train = dataset.X_train, dataset.y_train
         # X_val, y_val = dataset.X_val, dataset.y_val
         # X_train_dirty, y_train_dirty = dataset_dirty.X_train, dataset_dirty.y_train
         # assert X_train is not None and y_train is not None
         # assert X_train_dirty is not None and y_train_dirty is not None
@@ -237,188 +213,112 @@
         #     self.logger.debug("Need to reshape. New shape: %s", str(X_train.shape))
 
         # Construct binarized provenance matrix.
         # provenance = np.expand_dims(np.arange(dataset.trainsize, dtype=int), axis=(1, 2, 3))
         # provenance = np.pad(provenance, pad_width=((0, 0), (0, 0), (0, 0), (0, 1)))
         # provenance = binarize(provenance)
 
-        if self.eager_preprocessing:
-            dataset.apply(pipeline, cache_dir=self.pipeline_cache_dir, inplace=True)
-            dataset_dirty.apply(pipeline, cache_dir=self.pipeline_cache_dir, inplace=True)
-
         # Initialize the model and utility.
-        model_type = MODEL_TYPES[self.model]
-        model_kwargs = MODEL_KWARGS[self.model]
-        model = get_model(model_type, **model_kwargs)
+        model = get_model(self.model)
         # model_pipeline = deepcopy(pipeline)
         # pipeline.steps.append(("model", model))
         # if RepairMethod.is_pipe(self.method):
         #     model = model_pipeline
-        accuracy_utility = SklearnModelAccuracy(model, postprocessor=self.postprocessor)
-        roc_auc_utility = SklearnModelRocAuc(model, postprocessor=self.postprocessor)
+        accuracy_utility = SklearnModelAccuracy(model)
         eqodds_utility: Optional[SklearnModelEqualizedOddsDifference] = None
         if self.repairgoal == RepairGoal.FAIRNESS:
-            assert isinstance(dataset, BiasedNoisyLabelDataset)
+            assert isinstance(dataset, BiasedDirtyLabelDataset)
             eqodds_utility = SklearnModelEqualizedOddsDifference(
-                model,
-                sensitive_features=dataset.sensitive_feature,
-                groupings=groupings_test,
-                postprocessor=self.postprocessor,
+                model, sensitive_features=dataset.sensitive_feature, groupings=groupings_test
             )
 
         # target_model = model if RepairMethod.is_tmc_nonpipe(self.method) else pipeline
         target_utility: Utility
         if self.utility == UtilityType.ACCURACY:
-            target_utility = JointUtility(SklearnModelAccuracy(model, postprocessor=self.postprocessor), weights=[-1.0])
+            target_utility = JointUtility(SklearnModelAccuracy(model), weights=[-1.0])
             # target_utility = SklearnModelAccuracy(model)
         elif self.utility == UtilityType.EQODDS:
-            assert self.repairgoal == RepairGoal.FAIRNESS and isinstance(dataset, BiasedNoisyLabelDataset)
+            assert self.repairgoal == RepairGoal.FAIRNESS and isinstance(dataset, BiasedDirtyLabelDataset)
             target_utility = SklearnModelEqualizedOddsDifference(
-                model,
-                sensitive_features=dataset.sensitive_feature,
-                groupings=groupings_val,
-                postprocessor=self.postprocessor,
+                model, sensitive_features=dataset.sensitive_feature, groupings=groupings_val
             )
         elif self.utility == UtilityType.EQODDS_AND_ACCURACY:
-            assert self.repairgoal == RepairGoal.FAIRNESS and isinstance(dataset, BiasedNoisyLabelDataset)
+            assert self.repairgoal == RepairGoal.FAIRNESS and isinstance(dataset, BiasedDirtyLabelDataset)
             target_utility = JointUtility(
-                SklearnModelAccuracy(model, postprocessor=self.postprocessor),
+                SklearnModelAccuracy(model),
                 SklearnModelEqualizedOddsDifference(
-                    model,
-                    sensitive_features=dataset.sensitive_feature,
-                    groupings=groupings_val,
-                    postprocessor=self.postprocessor,
+                    model, sensitive_features=dataset.sensitive_feature, groupings=groupings_val
                 ),
                 weights=[-0.5, 0.5],
             )
-        elif self.utility == UtilityType.ROC_AUC:
-            target_utility = JointUtility(SklearnModelRocAuc(model, postprocessor=self.postprocessor), weights=[-1.0])
         else:
             raise ValueError("Unknown utility type '%s'." % repr(self.utility))
 
         # Compute importance scores and time it.
         importance_time_start = process_time_ns()
         n_units = dataset_dirty.units.shape[0]
-        importance: Optional[Importance] = None
+        importance: Optional[ShapleyImportance] = None
         importances: Optional[Iterable[float]] = None
         random = np.random.RandomState(seed=self._seed + self._iteration + 1)
         if self.method == RepairMethod.RANDOM:
             importances = list(random.rand(n_units))
-        elif self.method == RepairMethod.INFLUENCE:
-            from ..baselines.influence.importance import InfluenceImportance
-
-            dataset_f = dataset.apply(pipeline)
-            dataset_dirty_f = dataset_dirty.apply(pipeline)
-            importance = InfluenceImportance()
-            importances = importance.fit(
-                dataset_dirty_f.X_train, dataset_dirty_f.y_train, provenance=dataset_dirty_f.provenance
-            ).score(dataset_f.X_val, dataset_f.y_val)
-            importances = [-x for x in importances]
         else:
-            shapley_pipeline = pipeline if self.method != RepairMethod.KNN_Raw else FlattenPipeline()
             method = IMPORTANCE_METHODS[self.method]
             mc_iterations = MC_ITERATIONS[self.method]
             mc_preextract = RepairMethod.is_tmc_nonpipe(self.method)
             importance = ShapleyImportance(
                 method=method,
                 utility=target_utility,
-                pipeline=None if self.eager_preprocessing else shapley_pipeline,
+                pipeline=pipeline,
                 mc_iterations=mc_iterations,
                 mc_timeout=self.mc_timeout,
                 mc_tolerance=self.mc_tolerance,
                 mc_preextract=mc_preextract,
                 nn_k=self.nn_k,
                 logger=self.logger,
             )
-            if isinstance(model, DistanceModelMixin):
-                importance.nn_distance = model.distance
             importances = importance.fit(
-                dataset_dirty.X_train,
-                dataset_dirty.y_train,
-                dataset_dirty.metadata_train,
-                provenance=dataset_dirty.provenance,
-            ).score(dataset.X_val, dataset.y_val, dataset.metadata_val)
+                dataset_dirty.X_train, dataset_dirty.y_train, provenance=dataset_dirty.provenance
+            ).score(dataset.X_val, dataset.y_val)
         importance_time_end = process_time_ns()
         importance_cputime = (importance_time_end - importance_time_start) / 1e9
         self.logger.debug("Importance computed in: %s", str(timedelta(seconds=importance_cputime)))
         visited_units = np.zeros(n_units, dtype=bool)
         argsorted_importances = (-np.array(importances)).argsort()
         # argsorted_importances = np.ma.array(importances, mask=visited_units).argsort()
 
-        if self.augment_factor > 0 and self.method == RepairMethod.KNN_Raw:
-            assert isinstance(dataset, AugmentableMixin) and isinstance(dataset_dirty, AugmentableMixin)
-            dataset.augment(factor=self.augment_factor, inplace=True)
-            dataset_dirty.augment(factor=self.augment_factor, inplace=True)
-
         # Run the model to get initial score.
         # assert y_val is not None
-        dataset_f = dataset if self.eager_preprocessing else dataset.apply(pipeline, cache_dir=self.pipeline_cache_dir)
-        dataset_dirty_f = (
-            dataset_dirty
-            if self.eager_preprocessing
-            else dataset_dirty.apply(pipeline, cache_dir=self.pipeline_cache_dir)
-        )
-        eqodds_utility_result = UtilityResult()
+        dataset_f = dataset.apply(pipeline)
+        dataset_dirty_f = dataset_dirty.apply(pipeline)
+        eqodds: Optional[float] = None
         if eqodds_utility is not None:
-            eqodds_utility_result = eqodds_utility(
-                dataset_dirty_f.X_train,
-                dataset_dirty_f.y_train,
-                dataset_f.X_test,
-                dataset_f.y_test,
-                metadata_train=dataset_dirty_f.metadata_train,
-                metadata_test=dataset_f.metadata_test,
+            eqodds = eqodds_utility(
+                dataset_dirty_f.X_train, dataset_dirty_f.y_train, dataset_f.X_test, dataset_f.y_test
             )
-        accuracy_utility_result = accuracy_utility(
-            dataset_dirty_f.X_train,
-            dataset_dirty_f.y_train,
-            dataset_f.X_test,
-            dataset_f.y_test,
-            metadata_train=dataset_dirty_f.metadata_train,
-            metadata_test=dataset_f.metadata_test,
-        )
-        roc_auc_utility_result = roc_auc_utility(
-            dataset_dirty_f.X_train,
-            dataset_dirty_f.y_train,
-            dataset_f.X_test,
-            dataset_f.y_test,
-            metadata_train=dataset_dirty_f.metadata_train,
-            metadata_test=dataset_f.metadata_test,
+        accuracy = accuracy_utility(
+            dataset_dirty_f.X_train, dataset_dirty_f.y_train, dataset_f.X_test, dataset_f.y_test
         )
 
         # Update result table.
-        evolution = [
-            [
-                0.0,
-                eqodds_utility_result.score,
-                eqodds_utility_result.score,
-                accuracy_utility_result.score,
-                accuracy_utility_result.score,
-                roc_auc_utility_result.score,
-                roc_auc_utility_result.score,
-                0,
-                0.0,
-                0,
-                0.0,
-                0.0,
-            ]
-        ]
-        eqodds_start = eqodds_utility_result.score
-        accuracy_start = accuracy_utility_result.score
-        roc_auc_start = roc_auc_utility_result.score
+        evolution = [[0.0, eqodds, eqodds, accuracy, accuracy, 0, 0.0, 0, 0.0, 0.0]]
+        eqodds_start = eqodds
+        accuracy_start = accuracy
 
         # Set up progress bar.
         checkpoints = self.checkpoints if self.checkpoints > 0 and self.checkpoints < n_units else n_units
         n_units_per_checkpoint = round(n_units / checkpoints)
         if progress_bar:
             self.progress.start(total=checkpoints, desc="(id=%s) Repairs" % self.id)
         # pbar = None if not progress_bar else tqdm(total=dataset.trainsize, desc="%s Repairs" % str(self))
 
         # Iterate over the repair process.
         # visited_units = np.zeros(dataset.trainsize, dtype=bool)
         for i in range(checkpoints):
+
             # Determine indices of data examples that should be repaired given the unit with the highest importance.
             unvisited_units = np.invert(visited_units)
             target_units = argsorted_importances[unvisited_units[argsorted_importances]]
             if i + 1 < checkpoints:
                 target_units = target_units[:n_units_per_checkpoint]
             # target_query = np.zeros(n_units, dtype=int)
             # target_query[target_units] = 1
@@ -429,74 +329,54 @@
             # Repair the data example.
             # dataset_dirty.y_train[target_idx] = dataset.y_train[target_idx]
             visited_units[target_units] = True
             dataset_dirty.units_dirty[target_units] = False
 
             # Run the model.
             if eqodds_utility is not None:
-                eqodds_utility_result = eqodds_utility(
+                eqodds = eqodds_utility(
                     dataset_dirty_f.X_train,
                     dataset_dirty.y_train,
                     dataset_dirty_f.X_test,
                     dataset_dirty_f.y_test,
-                    metadata_train=dataset_dirty_f.metadata_train,
-                    metadata_test=dataset_dirty_f.metadata_test,
                 )
-            accuracy_utility_result = accuracy_utility(
-                dataset_dirty_f.X_train,
-                dataset_dirty.y_train,
-                dataset_dirty_f.X_test,
-                dataset_dirty_f.y_test,
-                metadata_train=dataset_dirty_f.metadata_train,
-                metadata_test=dataset_dirty_f.metadata_test,
-            )
-            roc_auc_utility_result = roc_auc_utility(
-                dataset_dirty_f.X_train,
-                dataset_dirty.y_train,
-                dataset_dirty_f.X_test,
-                dataset_dirty_f.y_test,
-                metadata_train=dataset_dirty_f.metadata_train,
-                metadata_test=dataset_dirty_f.metadata_test,
+            accuracy = accuracy_utility(
+                dataset_dirty_f.X_train, dataset_dirty.y_train, dataset_dirty_f.X_test, dataset_dirty_f.y_test
             )
 
             # self.logger.debug("Dirty units: %.2f", np.sum(dataset_dirty.units_dirty))
             # self.logger.debug("Same labels: %.2f", np.sum(dataset_dirty.y_train == dataset.y_train))
 
             # Update result table.
             steps_rel = (i + 1) / float(checkpoints)
             repaired = visited_units.sum(dtype=int)
             repaired_rel = repaired / float(n_units)
             discovered = np.logical_and(visited_units, units_dirty).sum(dtype=int)
             discovered_rel = discovered / units_dirty.sum(dtype=float)
             evolution.append(
                 [
                     steps_rel,
-                    eqodds_utility_result.score,
-                    eqodds_utility_result.score,
-                    accuracy_utility_result.score,
-                    accuracy_utility_result.score,
-                    roc_auc_utility_result.score,
-                    roc_auc_utility_result.score,
+                    eqodds,
+                    eqodds,
+                    accuracy,
+                    accuracy,
                     repaired,
                     repaired_rel,
                     discovered,
                     discovered_rel,
                     importance_cputime,
                 ]
             )
 
             # Recompute if needed.
             if importance is not None and self.method == RepairMethod.KNN_Interactive:
                 importance_time_start = process_time_ns()
                 importances = importance.fit(
-                    dataset_dirty.X_train,
-                    dataset_dirty.y_train,
-                    dataset_dirty.metadata_train,
-                    provenance=dataset_dirty.provenance,
-                ).score(dataset.X_val, dataset.y_val, dataset.metadata_val)
+                    dataset_dirty.X_train, dataset_dirty.y_train, provenance=dataset_dirty.provenance
+                ).score(dataset.X_val, dataset.y_val)
                 importance_time_end = process_time_ns()
                 importance_cputime += (importance_time_end - importance_time_start) / 1e9
                 argsorted_importances = (-np.array(importances)).argsort()
                 # argsorted_importances = np.ma.array(importances, mask=visited_units).argsort()
 
             # Update progress bar.
             if progress_bar:
@@ -507,46 +387,39 @@
             evolution,
             columns=[
                 "steps_rel",
                 "eqodds",
                 "eqodds_rel",
                 "accuracy",
                 "accuracy_rel",
-                "roc_auc",
-                "roc_auc_rel",
                 "repaired",
                 "repaired_rel",
                 "discovered",
                 "discovered_rel",
                 "importance_cputime",
             ],
         )
         self._evolution.index.name = "steps"
 
         # Recompute relative equalized odds (if we were keeping track of it).
         if eqodds_utility is not None:
-            eqodds_end = eqodds_utility_result.score
+            assert eqodds is not None and eqodds_start is not None
+            eqodds_end = eqodds
             eqqods_min = min(eqodds_start, eqodds_end)
             eqodds_delta = abs(eqodds_end - eqodds_start)
             self._evolution["eqodds_rel"] = self._evolution["eqodds_rel"].apply(
                 lambda x: (x - eqqods_min) / eqodds_delta
             )
         else:
             # Otherwise drop those columns.
             self._evolution.drop(["eqodds", "eqodds_rel"], axis=1, inplace=True)
 
-        # Recompute relative accuracy and ROC AUC.
-        accuracy_end = accuracy_utility_result.score
+        # Recompute relative accuracy.
+        accuracy_end = accuracy
         accuracy_delta = accuracy_end - accuracy_start
         self._evolution["accuracy_rel"] = self._evolution["accuracy_rel"].apply(
             lambda x: (x - accuracy_start) / accuracy_delta
         )
-        roc_auc_end = roc_auc_utility_result.score
-        roc_auc_min = min(roc_auc_start, roc_auc_end)
-        roc_auc_delta = abs(roc_auc_end - roc_auc_start)
-        self._evolution["roc_auc_rel"] = self._evolution["roc_auc_rel"].apply(
-            lambda x: (x - roc_auc_min) / roc_auc_delta
-        )
 
         # Close progress bar.
         if progress_bar:
             self.progress.close()
```

### Comparing `datascope-experiments-0.0.81/datascope_experiments.egg-info/PKG-INFO` & `datascope-experiments-0.0.9/datascope_experiments.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datascope-experiments
-Version: 0.0.81
+Version: 0.0.9
 Summary: Module for running experiments on top of datascope.
 Home-page: https://ease.ml/datascope/
 Author-email: easeml@ds3lab.com
 License: MIT
 Description: # Experimental toolkit for ease.ml/datascope
         
         [![PyPI version](https://badge.fury.io/py/datascope-experiments.svg)](https://badge.fury.io/py/datascope-experiments)
```

### Comparing `datascope-experiments-0.0.81/setup.py` & `datascope-experiments-0.0.9/setup.py`

 * *Files identical despite different names*

